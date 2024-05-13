# Comparing `tmp/slint-1.6.0a7.tar.gz` & `tmp/slint-1.6.0a8.tar.gz`

## Comparing `slint-1.6.0a7.tar` & `slint-1.6.0a8.tar`

### file list

```diff
@@ -1,894 +1,897 @@
--rw-r--r--   0     1001      127      738 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/README.md
--rw-r--r--   0     1001      127    19345 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/macros/lib.rs
--rw-r--r--   0     1001      127     1955 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/README.md
--rw-r--r--   0     1001      127    15614 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/calloop_backend/input.rs
--rw-r--r--   0     1001      127    11770 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/calloop_backend.rs
--rw-r--r--   0     1001      127     8655 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/display/gbmdisplay.rs
--rw-r--r--   0     1001      127     2955 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/display/swdisplay.rs
--rw-r--r--   0     1001      127     9345 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/display/vulkandisplay.rs
--rw-r--r--   0     1001      127     3237 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/display.rs
--rw-r--r--   0     1001      127    11904 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/drmoutput.rs
--rw-r--r--   0     1001      127     6253 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/fullscreenwindowadapter.rs
--rw-r--r--   0     1001      127     2022 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/lib.rs
--rw-r--r--   0     1001      127      365 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/mouse-pointer.svg
--rw-r--r--   0     1001      127      882 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/noop_backend.rs
--rw-r--r--   0     1001      127     7507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/renderer/femtovg.rs
--rw-r--r--   0     1001      127     6654 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/linuxkms/renderer/skia.rs
--rw-r--r--   0     1001      127     1913 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/Cargo.toml
--rw-r--r--   0     1001      127    10280 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127    16830 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/CC-BY-ND-4.0.txt
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      537 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/README.md
--rw-r--r--   0     1001      127     2420 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/build.rs
--rw-r--r--   0     1001      127    16358 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/builtin_macros.rs
--rw-r--r--   0     1001      127    18500 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/builtins.slint
--rw-r--r--   0     1001      127    19681 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/diagnostics.rs
--rw-r--r--   0     1001      127     2636 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/embedded_resources.rs
--rw-r--r--   0     1001      127    69892 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/expression_tree.rs
--rw-r--r--   0     1001      127     4420 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/fileaccess.rs
--rw-r--r--   0     1001      127   141177 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/generator/cpp.rs
--rw-r--r--   0     1001      127   123809 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/generator/rust.rs
--rw-r--r--   0     1001      127    19509 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/generator.rs
--rw-r--r--   0     1001      127    32752 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/langtype.rs
--rw-r--r--   0     1001      127    21425 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/layout.rs
--rw-r--r--   0     1001      127    15374 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/lexer.rs
--rw-r--r--   0     1001      127     9358 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/lib.rs
--rw-r--r--   0     1001      127     7020 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/literals.rs
--rw-r--r--   0     1001      127    31386 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/expression.rs
--rw-r--r--   0     1001      127    13532 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/item_tree.rs
--rw-r--r--   0     1001      127    40541 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/lower_expression.rs
--rw-r--r--   0     1001      127    31938 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/lower_to_item_tree.rs
--rw-r--r--   0     1001      127     6503 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/optim_passes/count_property_use.rs
--rw-r--r--   0     1001      127     6269 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/optim_passes/inline_expressions.rs
--rw-r--r--   0     1001      127    11380 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr/pretty_print.rs
--rw-r--r--   0     1001      127      654 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/llr.rs
--rw-r--r--   0     1001      127    11758 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/load_builtins.rs
--rw-r--r--   0     1001      127    39783 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/lookup.rs
--rw-r--r--   0     1001      127     7518 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/namedreference.rs
--rw-r--r--   0     1001      127   103277 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/object_tree.rs
--rw-r--r--   0     1001      127    10913 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/document.rs
--rw-r--r--   0     1001      127    21286 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/element.rs
--rw-r--r--   0     1001      127    14696 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/expressions.rs
--rw-r--r--   0     1001      127     3102 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/statements.rs
--rw-r--r--   0     1001      127     4561 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser/type.rs
--rw-r--r--   0     1001      127    36378 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser.rs
--rw-r--r--   0     1001      127     3949 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/apply_default_properties_from_style.rs
--rw-r--r--   0     1001      127    22379 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/binding_analysis.rs
--rw-r--r--   0     1001      127     1587 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/border_radius.rs
--rw-r--r--   0     1001      127     1793 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/check_expressions.rs
--rw-r--r--   0     1001      127     1941 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/check_public_api.rs
--rw-r--r--   0     1001      127     2309 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/check_rotation.rs
--rw-r--r--   0     1001      127     4580 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/clip.rs
--rw-r--r--   0     1001      127     2464 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_custom_fonts.rs
--rw-r--r--   0     1001      127     1933 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_globals.rs
--rw-r--r--   0     1001      127     1150 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_init_code.rs
--rw-r--r--   0     1001      127     4172 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_structs_and_enums.rs
--rw-r--r--   0     1001      127     1690 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/collect_subcomponents.rs
--rw-r--r--   0     1001      127     8043 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/compile_paths.rs
--rw-r--r--   0     1001      127     9466 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/const_propagation.rs
--rw-r--r--   0     1001      127     6155 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/deduplicate_property_read.rs
--rw-r--r--   0     1001      127    18877 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/default_geometry.rs
--rw-r--r--   0     1001      127    16260 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/embed_glyphs.rs
--rw-r--r--   0     1001      127    14883 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/embed_images.rs
--rw-r--r--   0     1001      127     5157 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/ensure_window.rs
--rw-r--r--   0     1001      127     6270 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/flickable.rs
--rw-r--r--   0     1001      127    11618 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/focus_handling.rs
--rw-r--r--   0     1001      127     4318 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/generate_item_indices.rs
--rw-r--r--   0     1001      127     6709 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/infer_aliases_types.rs
--rw-r--r--   0     1001      127    21455 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/inlining.rs
--rw-r--r--   0     1001      127     3241 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_absolute_coordinates.rs
--rw-r--r--   0     1001      127     3268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_accessibility.rs
--rw-r--r--   0     1001      127     1697 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_component_container.rs
--rw-r--r--   0     1001      127    31672 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_layout.rs
--rw-r--r--   0     1001      127     5565 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_popups.rs
--rw-r--r--   0     1001      127     5182 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_property_to_element.rs
--rw-r--r--   0     1001      127     6916 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_shadows.rs
--rw-r--r--   0     1001      127     9988 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_states.rs
--rw-r--r--   0     1001      127     8355 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_tabwidget.rs
--rw-r--r--   0     1001      127     2000 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/lower_text_input_interface.rs
--rw-r--r--   0     1001      127     6185 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/materialize_fake_properties.rs
--rw-r--r--   0     1001      127     7514 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/move_declarations.rs
--rw-r--r--   0     1001      127     2749 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/optimize_useless_rectangles.rs
--rw-r--r--   0     1001      127     4231 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/purity_check.rs
--rw-r--r--   0     1001      127     9197 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/remove_aliases.rs
--rw-r--r--   0     1001      127    19427 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/remove_return.rs
--rw-r--r--   0     1001      127     1656 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/remove_unused_properties.rs
--rw-r--r--   0     1001      127     5145 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/repeater_component.rs
--rw-r--r--   0     1001      127     5620 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/resolve_native_classes.rs
--rw-r--r--   0     1001      127    71031 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/resolving.rs
--rw-r--r--   0     1001      127     3046 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/unique_id.rs
--rw-r--r--   0     1001      127     4210 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/visible.rs
--rw-r--r--   0     1001      127     2961 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes/z_order.rs
--rw-r--r--   0     1001      127    10741 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/passes.rs
--rw-r--r--   0     1001      127    18378 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/pathutils.rs
--rw-r--r--   0     1001      127     8812 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/consistent_styles.rs
--rw-r--r--   0     1001      127     1237 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/accessibility/accessible_properties.slint
--rw-r--r--   0     1001      127     1774 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop1.slint
--rw-r--r--   0     1001      127     1826 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop2.slint
--rw-r--r--   0     1001      127      924 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_function.slint
--rw-r--r--   0     1001      127      643 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint
--rw-r--r--   0     1001      127     2458 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint
--rw-r--r--   0     1001      127     1854 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint
--rw-r--r--   0     1001      127     1144 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint
--rw-r--r--   0     1001      127     2120 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint
--rw-r--r--   0     1001      127      488 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_mappointtowindow.slint
--rw-r--r--   0     1001      127      923 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_self.slint
--rw-r--r--   0     1001      127      942 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/animate.slint
--rw-r--r--   0     1001      127      230 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/array.slint
--rw-r--r--   0     1001      127      788 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/assign.slint
--rw-r--r--   0     1001      127      585 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/box_shadow.slint
--rw-r--r--   0     1001      127     1021 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/children_placeholder.slint
--rw-r--r--   0     1001      127      301 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/children_placeholder_2.slint
--rw-r--r--   0     1001      127      663 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/clip.slint
--rw-r--r--   0     1001      127      492 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/comments.slint
--rw-r--r--   0     1001      127     2078 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/dialog.slint
--rw-r--r--   0     1001      127      631 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/dialog2.slint
--rw-r--r--   0     1001      127      499 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/double_binding.slint
--rw-r--r--   0     1001      127      270 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/double_color.slint
--rw-r--r--   0     1001      127     1137 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/duplicated_id.slint
--rw-r--r--   0     1001      127     1340 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/easing.slint
--rw-r--r--   0     1001      127      383 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/easing_not_called.slint
--rw-r--r--   0     1001      127      156 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/empty.slint
--rw-r--r--   0     1001      127      526 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/enums.slint
--rw-r--r--   0     1001      127      441 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/for.slint
--rw-r--r--   0     1001      127      492 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/image.slint
--rw-r--r--   0     1001      127      450 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/inline_component.slint
--rw-r--r--   0     1001      127      895 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/item_as_property.slint
--rw-r--r--   0     1001      127      465 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/layout.slint
--rw-r--r--   0     1001      127     1958 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/layout2.slint
--rw-r--r--   0     1001      127     2188 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/linear-gradient.slint
--rw-r--r--   0     1001      127      470 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/object_in_binding.slint
--rw-r--r--   0     1001      127      538 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/opacity.slint
--rw-r--r--   0     1001      127      905 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/parse_error.slint
--rw-r--r--   0     1001      127      535 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/path.slint
--rw-r--r--   0     1001      127     1114 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/path_commands.slint
--rw-r--r--   0     1001      127      541 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/path_for.slint
--rw-r--r--   0     1001      127     1056 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/percent.slint
--rw-r--r--   0     1001      127      707 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/popup.slint
--rw-r--r--   0     1001      127      333 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/property_animation.slint
--rw-r--r--   0     1001      127      983 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/property_declaration.slint
--rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/property_declaration_in_component.slint
--rw-r--r--   0     1001      127     1786 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/radial-gradient.slint
--rw-r--r--   0     1001      127      837 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/return.slint
--rw-r--r--   0     1001      127     1850 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/rotation.slint
--rw-r--r--   0     1001      127      456 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/rust-attr.slint
--rw-r--r--   0     1001      127     1781 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/self_assign.slint
--rw-r--r--   0     1001      127     1413 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/signal.slint
--rw-r--r--   0     1001      127     4436 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions.slint
--rw-r--r--   0     1001      127      711 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions2.slint
--rw-r--r--   0     1001      127      748 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions3.slint
--rw-r--r--   0     1001      127      731 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_two_way.slint
--rw-r--r--   0     1001      127      731 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/sub_elements.slint
--rw-r--r--   0     1001      127      218 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/supersimple.slint
--rw-r--r--   0     1001      127      467 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/svg_path.slint
--rw-r--r--   0     1001      127     1600 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/tr.slint
--rw-r--r--   0     1001      127     3038 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/tr2.slint
--rw-r--r--   0     1001      127     1108 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/type_declaration.slint
--rw-r--r--   0     1001      127     1391 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/basic/unknown_item.slint
--rw-r--r--   0     1001      127      457 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/callbacks/init.slint
--rw-r--r--   0     1001      127      552 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/callbacks/property-changes.slint
--rw-r--r--   0     1001      127      671 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/component_container.slint
--rw-r--r--   0     1001      127     1202 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/listview.slint
--rw-r--r--   0     1001      127      601 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/popup.slint
--rw-r--r--   0     1001      127      538 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget.slint
--rw-r--r--   0     1001      127      898 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget2.slint
--rw-r--r--   0     1001      127      474 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget3.slint
--rw-r--r--   0     1001      127      436 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/export_duplicates.slint
--rw-r--r--   0     1001      127      623 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/reexport_duplicate.slint
--rw-r--r--   0     1001      127      326 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/root_compo_export.slint
--rw-r--r--   0     1001      127      289 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/root_compo_export2.slint
--rw-r--r--   0     1001      127      332 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/single_global_missing_export.slint
--rw-r--r--   0     1001      127      288 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/exports/unused_compo.slint
--rw-r--r--   0     1001      127     1464 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/arithmetic_op.slint
--rw-r--r--   0     1001      127     1261 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/clamp.slint
--rw-r--r--   0     1001      127      999 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/comparison_operator.slint
--rw-r--r--   0     1001      127     1473 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/condition_operator.slint
--rw-r--r--   0     1001      127     3442 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/image-url.slint
--rw-r--r--   0     1001      127     1090 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/image-url2.slint
--rw-r--r--   0     1001      127     1355 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/minmax.slint
--rw-r--r--   0     1001      127      654 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/percent2.slint
--rw-r--r--   0     1001      127      456 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/strings.slint
--rw-r--r--   0     1001      127     1221 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/expressions/unary_op.slint
--rw-r--r--   0     1001      127      387 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_invalid.slint
--rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_not_called.slint
--rw-r--r--   0     1001      127      705 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_wrong_args.slint
--rw-r--r--   0     1001      127     1707 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint
--rw-r--r--   0     1001      127      592 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/functions/function_double_qualified.slint
--rw-r--r--   0     1001      127     1814 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions.slint
--rw-r--r--   0     1001      127     2990 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions_call.slint
--rw-r--r--   0     1001      127     3353 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions_purity.slint
--rw-r--r--   0     1001      127      597 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/bug_2719.slint
--rw-r--r--   0     1001      127     1018 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint
--rw-r--r--   0     1001      127      407 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/cyclic_import.slint
--rw-r--r--   0     1001      127      441 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/error_in_import.slint
--rw-r--r--   0     1001      127      252 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/error_in_import2.slint
--rw-r--r--   0     1001      127      295 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/error_in_import3.slint
--rw-r--r--   0     1001      127      410 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/font.slint
--rw-r--r--   0     1001      127      393 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_builtin.slint
--rw-r--r--   0     1001      127      411 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_error2.slint
--rw-r--r--   0     1001      127      944 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_errors.slint
--rw-r--r--   0     1001      127      207 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error1.slint
--rw-r--r--   0     1001      127      221 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error2.slint
--rw-r--r--   0     1001      127      238 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error3.slint
--rw-r--r--   0     1001      127      239 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error4.slint
--rw-r--r--   0     1001      127      503 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_parse_error5.slint
--rw-r--r--   0     1001      127      472 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/invalid_export.slint
--rw-r--r--   0     1001      127      379 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/imports/visibility_errors.slint
--rw-r--r--   0     1001      127      703 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/layout/if_in_grid.slint
--rw-r--r--   0     1001      127      441 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/layout/if_in_grid_row.slint
--rw-r--r--   0     1001      127      586 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/layout/min_max_conflict.slint
--rw-r--r--   0     1001      127      655 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/layout/spacing.slint
--rw-r--r--   0     1001      127      477 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/absolute-position.slint
--rw-r--r--   0     1001      127      691 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/array_index.slint
--rw-r--r--   0     1001      127      594 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias.slint
--rw-r--r--   0     1001      127      641 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias2.slint
--rw-r--r--   0     1001      127     1087 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias3.slint
--rw-r--r--   0     1001      127      255 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias_issue4938.slint
--rw-r--r--   0     1001      127      376 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_not_called.slint
--rw-r--r--   0     1001      127      433 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_return.slint
--rw-r--r--   0     1001      127     1814 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/color.slint
--rw-r--r--   0     1001      127     3112 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/conversion.slint
--rw-r--r--   0     1001      127     1807 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/dashes.slint
--rw-r--r--   0     1001      127     1250 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/deprecated_property.slint
--rw-r--r--   0     1001      127     1138 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/enum.slint
--rw-r--r--   0     1001      127     2598 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/for_lookup.slint
--rw-r--r--   0     1001      127     1211 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/global.slint
--rw-r--r--   0     1001      127      621 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/if.slint
--rw-r--r--   0     1001      127      920 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/issue_1461.slint
--rw-r--r--   0     1001      127     1287 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/property.slint
--rw-r--r--   0     1001      127     1704 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint
--rw-r--r--   0     1001      127     1439 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/signal_arg.slint
--rw-r--r--   0     1001      127     1444 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding.slint
--rw-r--r--   0     1001      127     1220 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint
--rw-r--r--   0     1001      127      392 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding_model.slint
--rw-r--r--   0     1001      127      903 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint
--rw-r--r--   0     1001      127     2695 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/input_output.slint
--rw-r--r--   0     1001      127     3062 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/input_output2.slint
--rw-r--r--   0     1001      127      593 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/new_component.slint
--rw-r--r--   0     1001      127     1020 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/new_lookup.slint
--rw-r--r--   0     1001      127     8651 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint
--rw-r--r--   0     1001      127      252 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/children_placeholder0.slint
--rw-r--r--   0     1001      127      263 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/export0.slint
--rw-r--r--   0     1001      127      219 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/export1.slint
--rw-r--r--   0     1001      127      362 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if0.slint
--rw-r--r--   0     1001      127      278 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if1.slint
--rw-r--r--   0     1001      127      285 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if2.slint
--rw-r--r--   0     1001      127      224 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if3.slint
--rw-r--r--   0     1001      127      361 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/if4.slint
--rw-r--r--   0     1001      127      398 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/property1.slint
--rw-r--r--   0     1001      127      902 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/property2.slint
--rw-r--r--   0     1001      127      846 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/state1.slint
--rw-r--r--   0     1001      127      244 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/state2.slint
--rw-r--r--   0     1001      127      307 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/state3.slint
--rw-r--r--   0     1001      127      707 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/struct.slint
--rw-r--r--   0     1001      127     9418 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/syntax_tests.rs
--rw-r--r--   0     1001      127      156 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/custom_style/TestStyle/std-widgets.slint
--rw-r--r--   0     1001      127      278 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/dependency_local.slint
--rw-r--r--   0     1001      127      393 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/dependency_test_main.slint
--rw-r--r--   0     1001      127      503 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/bug_2719_import.slint
--rw-r--r--   0     1001      127      461 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/bug_3674_alias_from_invalid_import.slint
--rw-r--r--   0     1001      127      262 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/dependency_from_incpath.slint
--rw-r--r--   0     1001      127      205 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/local_helper_type.slint
--rw-r--r--   0     1001      127      237 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/should_fail.slint
--rw-r--r--   0     1001      127      320 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/should_fail2.slint
--rw-r--r--   0     1001      127      280 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/should_fail3.slint
--rw-r--r--   0     1001      127      491 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/incpath/should_fail4.slint
--rw-r--r--   0     1001      127      208 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/library/dependency_from_library.slint
--rw-r--r--   0     1001      127      243 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/library/lib.slint
--rw-r--r--   0     1001      127      214 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/library/library_helper_type.slint
--rw-r--r--   0     1001      127      324 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/recursive_import1.slint
--rw-r--r--   0     1001      127      395 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/recursive_import2.slint
--rw-r--r--   0     1001      127      450 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/tests/typeloader/some_rust_file.rs
--rw-r--r--   0     1001      127    43496 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/typeloader.rs
--rw-r--r--   0     1001      127    19774 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/typeregister.rs
--rw-r--r--   0     1001      127    14083 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg
--rw-r--r--   0     1001      127    14073 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg
--rw-r--r--   0     1001      127     2358 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/combobox-base.slint
--rw-r--r--   0     1001      127     3861 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/common.slint
--rw-r--r--   0     1001      127     3266 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/lineedit-base.slint
--rw-r--r--   0     1001      127     4288 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/listview.slint
--rw-r--r--   0     1001      127     3926 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/slider-base.slint
--rw-r--r--   0     1001      127     2427 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/spinbox-base.slint
--rw-r--r--   0     1001      127     2510 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/spinner-base.slint
--rw-r--r--   0     1001      127     1202 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/standardbutton.slint
--rw-r--r--   0     1001      127     1080 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/common/tabwidget-base.slint
--rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic/std-widgets.slint
--rw-r--r--   0     1001      127      308 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/_arrow_down.svg
--rw-r--r--   0     1001      127      284 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/_arrow_up.svg
--rw-r--r--   0     1001      127      413 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/_check-mark.svg
--rw-r--r--   0     1001      127      148 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/_pane_down.svg
--rw-r--r--   0     1001      127     2760 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/button.slint
--rw-r--r--   0     1001      127     2726 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/checkbox.slint
--rw-r--r--   0     1001      127     3057 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/combobox.slint
--rw-r--r--   0     1001      127     4437 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/components.slint
--rw-r--r--   0     1001      127     1000 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/layouts.slint
--rw-r--r--   0     1001      127     2886 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/lineedit.slint
--rw-r--r--   0     1001      127      988 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/progressindicator.slint
--rw-r--r--   0     1001      127     5065 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/scrollview.slint
--rw-r--r--   0     1001      127     2930 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/slider.slint
--rw-r--r--   0     1001      127     3327 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/spinbox.slint
--rw-r--r--   0     1001      127      733 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2126 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     3420 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/styling.slint
--rw-r--r--   0     1001      127     2861 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/switch.slint
--rw-r--r--   0     1001      127     9124 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/tableview.slint
--rw-r--r--   0     1001      127     6075 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/tabwidget.slint
--rw-r--r--   0     1001      127     4438 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-dark/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-light/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cosmic-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino/std-widgets.slint
--rw-r--r--   0     1001      127      513 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_arrow-down.svg
--rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_arrow-up.svg
--rw-r--r--   0     1001      127      780 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_check-mark.svg
--rw-r--r--   0     1001      127      623 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_chevron-down.svg
--rw-r--r--   0     1001      127      601 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_chevron-up.svg
--rw-r--r--   0     1001      127      918 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_down.svg
--rw-r--r--   0     1001      127      489 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_dropdown.svg
--rw-r--r--   0     1001      127      849 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_left.svg
--rw-r--r--   0     1001      127      815 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_right.svg
--rw-r--r--   0     1001      127     1135 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_up.svg
--rw-r--r--   0     1001      127     5181 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/button.slint
--rw-r--r--   0     1001      127     4547 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/checkbox.slint
--rw-r--r--   0     1001      127     5646 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/combobox.slint
--rw-r--r--   0     1001      127     3145 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/components.slint
--rw-r--r--   0     1001      127     1103 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/layouts.slint
--rw-r--r--   0     1001      127     3180 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/lineedit.slint
--rw-r--r--   0     1001      127     1404 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/progressindicator.slint
--rw-r--r--   0     1001      127     5563 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/scrollview.slint
--rw-r--r--   0     1001      127     3097 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/slider.slint
--rw-r--r--   0     1001      127     5483 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/spinbox.slint
--rw-r--r--   0     1001      127      739 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2216 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     4541 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/styling.slint
--rw-r--r--   0     1001      127     4097 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/switch.slint
--rw-r--r--   0     1001      127     8959 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/tableview.slint
--rw-r--r--   0     1001      127     5493 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/tabwidget.slint
--rw-r--r--   0     1001      127     6640 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-dark/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-light/color-scheme.slint
--rw-r--r--   0     1001      127      332 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      215 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/cupertino-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent/std-widgets.slint
--rw-r--r--   0     1001      127      513 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_arrow-down.svg
--rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_arrow-up.svg
--rw-r--r--   0     1001      127      780 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_check-mark.svg
--rw-r--r--   0     1001      127      623 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_chevron-down.svg
--rw-r--r--   0     1001      127      601 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_chevron-up.svg
--rw-r--r--   0     1001      127      918 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_down.svg
--rw-r--r--   0     1001      127      489 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_dropdown.svg
--rw-r--r--   0     1001      127      849 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_left.svg
--rw-r--r--   0     1001      127      815 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_right.svg
--rw-r--r--   0     1001      127     1135 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/_up.svg
--rw-r--r--   0     1001      127     4607 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/button.slint
--rw-r--r--   0     1001      127     3883 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/checkbox.slint
--rw-r--r--   0     1001      127     3773 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/combobox.slint
--rw-r--r--   0     1001      127     3363 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/components.slint
--rw-r--r--   0     1001      127      877 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/groupbox.slint
--rw-r--r--   0     1001      127      632 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/layouts.slint
--rw-r--r--   0     1001      127     3499 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/lineedit.slint
--rw-r--r--   0     1001      127     1023 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/progressindicator.slint
--rw-r--r--   0     1001      127     6590 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/scrollview.slint
--rw-r--r--   0     1001      127     3734 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/slider.slint
--rw-r--r--   0     1001      127     3992 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/spinbox.slint
--rw-r--r--   0     1001      127      733 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/spinner.slint
--rw-r--r--   0     1001      127     1524 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2126 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     6248 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/styling.slint
--rw-r--r--   0     1001      127     4616 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/switch.slint
--rw-r--r--   0     1001      127     9561 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/tableview.slint
--rw-r--r--   0     1001      127     5493 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/tabwidget.slint
--rw-r--r--   0     1001      127     4935 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-base/textedit.slint
--rw-r--r--   0     1001      127      257 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-dark/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-light/color-scheme.slint
--rw-r--r--   0     1001      127      329 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      212 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/fluent-light/std-widgets.slint
--rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material/color-scheme.slint
--rw-r--r--   0     1001      127      347 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material/std-widgets.slint
--rw-r--r--   0     1001      127      163 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_arrow-downward.svg
--rw-r--r--   0     1001      127      115 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_arrow-drop-down.svg
--rw-r--r--   0     1001      127      115 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_arrow-drop-up.svg
--rw-r--r--   0     1001      127      161 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_arrow-upward.svg
--rw-r--r--   0     1001      127      150 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_check-mark.svg
--rw-r--r--   0     1001      127      145 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/_expand-more.svg
--rw-r--r--   0     1001      127     3288 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/button.slint
--rw-r--r--   0     1001      127     5664 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/checkbox.slint
--rw-r--r--   0     1001      127     3452 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/combobox.slint
--rw-r--r--   0     1001      127     4712 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/components.slint
--rw-r--r--   0     1001      127     1477 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/groupbox.slint
--rw-r--r--   0     1001      127      633 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/layouts.slint
--rw-r--r--   0     1001      127     2866 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/lineedit.slint
--rw-r--r--   0     1001      127     1010 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/progressindicator.slint
--rw-r--r--   0     1001      127     5014 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/scrollview.slint
--rw-r--r--   0     1001      127     4146 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/slider.slint
--rw-r--r--   0     1001      127     5090 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/spinbox.slint
--rw-r--r--   0     1001      127      737 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/spinner.slint
--rw-r--r--   0     1001      127     1373 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/std-widgets-base.slint
--rw-r--r--   0     1001      127     2213 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/std-widgets-impl.slint
--rw-r--r--   0     1001      127     3651 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/styling.slint
--rw-r--r--   0     1001      127     6174 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/switch.slint
--rw-r--r--   0     1001      127     8186 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/tableview.slint
--rw-r--r--   0     1001      127     4886 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-base/tabwidget.slint
--rw-r--r--   0     1001      127      257 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-dark/color-scheme.slint
--rw-r--r--   0     1001      127      331 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-dark/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-dark/std-widgets.slint
--rw-r--r--   0     1001      127      258 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-light/color-scheme.slint
--rw-r--r--   0     1001      127      331 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-light/std-widgets-impl.slint
--rw-r--r--   0     1001      127      214 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/material-light/std-widgets.slint
--rw-r--r--   0     1001      127     1736 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/button.slint
--rw-r--r--   0     1001      127      350 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/checkbox.slint
--rw-r--r--   0     1001      127     1707 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/combobox.slint
--rw-r--r--   0     1001      127      582 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/groupbox.slint
--rw-r--r--   0     1001      127     2384 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/internal-scrollview.slint
--rw-r--r--   0     1001      127      613 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/layouts.slint
--rw-r--r--   0     1001      127     2377 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/lineedit.slint
--rw-r--r--   0     1001      127      307 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/progressindicator.slint
--rw-r--r--   0     1001      127     1026 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/scrollview.slint
--rw-r--r--   0     1001      127      447 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/slider.slint
--rw-r--r--   0     1001      127      859 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/spinbox.slint
--rw-r--r--   0     1001      127     1265 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/spinner.slint
--rw-r--r--   0     1001      127      374 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/std-widgets-impl.slint
--rw-r--r--   0     1001      127     1475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/std-widgets.slint
--rw-r--r--   0     1001      127      346 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/switch.slint
--rw-r--r--   0     1001      127     5310 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/tableview.slint
--rw-r--r--   0     1001      127     1564 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/widgets/qt/tabwidget.slint
--rw-r--r--   0     1001      127     1126 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     8815 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      635 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/README.md
--rw-r--r--   0     1001      127     7636 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/builtin_structs.rs
--rw-r--r--   0     1001      127    19656 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/enums.rs
--rw-r--r--   0     1001      127     8311 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/key_codes.rs
--rw-r--r--   0     1001      127     1322 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/lib.rs
--rw-r--r--   0     1001      127   757076 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/sharedfontdb/DejaVuSans.ttf
--rw-r--r--   0     1001      127      145 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/sharedfontdb/DejaVuSans.ttf.license
--rw-r--r--   0     1001      127     4526 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/sharedfontdb/fontconfig.rs
--rw-r--r--   0     1001      127     7491 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/common/sharedfontdb.rs
--rw-r--r--   0     1001      127      630 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/Cargo.toml
--rw-r--r--   0     1001      127      610 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/CHANGELOG.md
--rw-r--r--   0     1001      127    10280 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      492 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/README.md
--rw-r--r--   0     1001      127     6982 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/src/lib.rs
--rw-r--r--   0     1001      127     4766 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/tests/test_field_offset.rs
--rw-r--r--   0     1001      127      826 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/Cargo.toml
--rw-r--r--   0     1001      127     4705 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/README.md
--rw-r--r--   0     1001      127      845 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/ffi.rs
--rw-r--r--   0     1001      127     2990 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/internal_tests.rs
--rw-r--r--   0     1001      127     1695 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/lib.rs
--rw-r--r--   0     1001      127     5754 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/search_api.rs
--rw-r--r--   0     1001      127     6991 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/testing/testing_backend.rs
--rw-r--r--   0     1001      127      571 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/macro/Cargo.toml
--rw-r--r--   0     1001      127    10280 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/macro/LICENSES/MIT.txt
--rw-r--r--   0     1001      127    31632 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/macro/macro.rs
--rw-r--r--   0     1001      127     1919 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/README.md
--rw-r--r--   0     1001      127    26501 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/fonts.rs
--rw-r--r--   0     1001      127     9732 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/images.rs
--rw-r--r--   0     1001      127    61993 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/itemrenderer.rs
--rw-r--r--   0     1001      127    23205 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/femtovg/lib.rs
--rw-r--r--   0     1001      127     2370 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      872 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/README.md
--rw-r--r--   0     1001      127     2014 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/build.rs
--rw-r--r--   0     1001      127     5859 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/selector/lib.rs
--rw-r--r--   0     1001      127      623 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/Cargo.toml
--rw-r--r--   0     1001      127     1796 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/CHANGELOG.md
--rw-r--r--   0     1001      127    10280 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/LICENSES/Apache-2.0.txt
--rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/LICENSES/MIT.txt
--rw-r--r--   0     1001      127      399 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/README.md
--rw-r--r--   0     1001      127     3723 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/src/compile_fail_tests.rs
--rw-r--r--   0     1001      127    18776 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/src/lib.rs
--rw-r--r--   0     1001      127    18973 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/src/vrc.rs
--rw-r--r--   0     1001      127     9552 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/tests/test_vrc.rs
--rw-r--r--   0     1001      127     5359 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/vtable/tests/test_vtable.rs
--rw-r--r--   0     1001      127      471 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser-test-macro/Cargo.toml
--rw-r--r--   0     1001      127      887 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser-test-macro/README.md
--rw-r--r--   0     1001      127     5619 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/compiler/parser-test-macro/lib.rs
--rw-r--r--   0     1001      127     4483 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      532 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/README.md
--rw-r--r--   0     1001      127     2766 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/accessibility.rs
--rw-r--r--   0     1001      127    13996 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/animations.rs
--rw-r--r--   0     1001      127    38650 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/api.rs
--rw-r--r--   0     1001      127     5210 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/callbacks.rs
--rw-r--r--   0     1001      127     2586 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/component_factory.rs
--rw-r--r--   0     1001      127     2926 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/context.rs
--rw-r--r--   0     1001      127     7695 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/future.rs
--rw-r--r--   0     1001      127     2503 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/bitmapfont.rs
--rw-r--r--   0     1001      127    14664 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/border_radius.rs
--rw-r--r--   0     1001      127     4038 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/boxshadowcache.rs
--rw-r--r--   0     1001      127    14919 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/brush.rs
--rw-r--r--   0     1001      127    17436 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/color.rs
--rw-r--r--   0     1001      127     7064 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/image/cache.rs
--rw-r--r--   0     1001      127     2528 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/image/htmlimage.rs
--rw-r--r--   0     1001      127     3408 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/image/svg.rs
--rw-r--r--   0     1001      127    48855 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/image.rs
--rw-r--r--   0     1001      127    15911 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/path.rs
--rw-r--r--   0     1001      127     6978 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics/rendering_metrics_collector.rs
--rw-r--r--   0     1001      127     8249 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/graphics.rs
--rw-r--r--   0     1001      127    33891 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/input.rs
--rw-r--r--   0     1001      127     8604 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/item_focus.rs
--rw-r--r--   0     1001      127    32977 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/item_rendering.rs
--rw-r--r--   0     1001      127    68108 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/item_tree.rs
--rw-r--r--   0     1001      127     8608 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/component_container.rs
--rw-r--r--   0     1001      127    17039 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/flickable.rs
--rw-r--r--   0     1001      127     8722 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/image.rs
--rw-r--r--   0     1001      127     5377 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/path.rs
--rw-r--r--   0     1001      127    65922 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items/text.rs
--rw-r--r--   0     1001      127    46637 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/items.rs
--rw-r--r--   0     1001      127    27945 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/layout.rs
--rw-r--r--   0     1001      127     3347 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/lengths.rs
--rw-r--r--   0     1001      127     2237 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/lib.rs
--rw-r--r--   0     1001      127    47643 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/model/adapters.rs
--rw-r--r--   0     1001      127     6658 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/model/model_peer.rs
--rw-r--r--   0     1001      127    47304 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/model.rs
--rw-r--r--   0     1001      127    16009 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/platform.rs
--rw-r--r--   0     1001      127     7794 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/properties/change_tracker.rs
--rw-r--r--   0     1001      127    18894 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/properties/ffi.rs
--rw-r--r--   0     1001      127    38401 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/properties/properties_animations.rs
--rw-r--r--   0     1001      127    59846 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/properties.rs
--rw-r--r--   0     1001      127     5015 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/renderer.rs
--rw-r--r--   0     1001      127    10886 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/rtti.rs
--rw-r--r--   0     1001      127    21418 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/sharedvector.rs
--rw-r--r--   0     1001      127     2865 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/slice.rs
--rw-r--r--   0     1001      127    28862 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/draw_functions.rs
--rw-r--r--   0     1001      127     3465 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fixed.rs
--rw-r--r--   0     1001      127     4673 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fonts/pixelfont.rs
--rw-r--r--   0     1001      127     3859 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fonts/systemfonts.rs
--rw-r--r--   0     1001      127     7334 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fonts/vectorfont.rs
--rw-r--r--   0     1001      127     5915 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer/fonts.rs
--rw-r--r--   0     1001      127   108310 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/software_renderer.rs
--rw-r--r--   0     1001      127    13307 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/string.rs
--rw-r--r--   0     1001      127     4182 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/tests.rs
--rw-r--r--   0     1001      127    12929 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/fragments.rs
--rw-r--r--   0     1001      127     3222 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/glyphclusters.rs
--rw-r--r--   0     1001      127     1234 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/linebreak_simple.rs
--rw-r--r--   0     1001      127     1260 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/linebreak_unicode.rs
--rw-r--r--   0     1001      127    15364 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/linebreaker.rs
--rw-r--r--   0     1001      127    13512 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout/shaping.rs
--rw-r--r--   0     1001      127    24952 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/textlayout.rs
--rw-r--r--   0     1001      127    31757 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/timers.rs
--rw-r--r--   0     1001      127     8992 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/translations.rs
--rw-r--r--   0     1001      127     1884 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/unsafe_single_threaded.rs
--rw-r--r--   0     1001      127    63165 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core/window.rs
--rw-r--r--   0     1001      127     3852 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     2320 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/README.md
--rw-r--r--   0     1001      127    22398 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/accesskit.rs
--rw-r--r--   0     1001      127      474 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/build.rs
--rw-r--r--   0     1001      127    30209 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/event_loop.rs
--rw-r--r--   0     1001      127    16654 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/lib.rs
--rw-r--r--   0     1001      127     8046 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/renderer/femtovg/glcontext.rs
--rw-r--r--   0     1001      127     2131 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/renderer/femtovg.rs
--rw-r--r--   0     1001      127     4558 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/renderer/skia.rs
--rw-r--r--   0     1001      127     6824 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/renderer/sw.rs
--rw-r--r--   0     1001      127    14717 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/wasm_input_helper.rs
--rw-r--r--   0     1001      127    32085 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/winit/winitwindowadapter.rs
--rw-r--r--   0     1001      127     2855 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/README.md
--rw-r--r--   0     1001      127      673 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/build.rs
--rw-r--r--   0     1001      127     6875 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/cached_image.rs
--rw-r--r--   0     1001      127    14877 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/d3d_surface.rs
--rw-r--r--   0     1001      127    37207 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/itemrenderer.rs
--rw-r--r--   0     1001      127    23253 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/lib.rs
--rw-r--r--   0     1001      127     6372 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/metal_surface.rs
--rw-r--r--   0     1001      127    15370 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/opengl_surface.rs
--rw-r--r--   0     1001      127     4611 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/software_surface.rs
--rw-r--r--   0     1001      127    11843 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/textlayout.rs
--rw-r--r--   0     1001      127    17420 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/renderers/skia/vulkan_surface.rs
--rw-r--r--   0     1001      127      706 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/macro/Cargo.toml
--rw-r--r--   0     1001      127    12200 2024-05-03 06:06:50.000000 slint-1.6.0a7/helper_crates/const-field-offset/macro/macro.rs
--rw-r--r--   0     1001      127     6405 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127    68256 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/api.rs
--rw-r--r--   0     1001      127    86334 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/dynamic_item_tree.rs
--rw-r--r--   0     1001      127     7555 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/dynamic_type.rs
--rw-r--r--   0     1001      127    75104 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/eval.rs
--rw-r--r--   0     1001      127    12240 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/eval_layout.rs
--rw-r--r--   0     1001      127    31460 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/ffi.rs
--rw-r--r--   0     1001      127     9875 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/global_component.rs
--rw-r--r--   0     1001      127     5912 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/highlight.rs
--rw-r--r--   0     1001      127     3029 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/lib.rs
--rw-r--r--   0     1001      127     1425 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/migration.rs
--rw-r--r--   0     1001      127     1809 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/tests.rs
--rw-r--r--   0     1001      127     2301 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/interpreter/value_model.rs
--rw-r--r--   0     1001      127     9909 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127     1078 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/LICENSES/MIT.txt
--rw-r--r--   0     1001      127     1881 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/README.md
--rw-r--r--   0     1001      127     5140 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/android.rs
--rw-r--r--   0     1001      127      548 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/compile_fail_tests.rs
--rw-r--r--   0     1001      127     9447 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/building.md
--rw-r--r--   0     1001      127     7147 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/development.md
--rw-r--r--   0     1001      127     2881 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/install_qt.md
--rw-r--r--   0     1001      127        5 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/.gitignore
--rw-r--r--   0     1001      127     1013 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/README.md
--rw-r--r--   0     1001      127      261 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/book.toml
--rw-r--r--   0     1001      127      810 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt
--rw-r--r--   0     1001      127      515 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md
--rw-r--r--   0     1001      127      268 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/appwindow.slint
--rw-r--r--   0     1001      127     1216 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/conclusion.md
--rw-r--r--   0     1001      127     1337 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md
--rw-r--r--   0     1001      127     2039 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md
--rw-r--r--   0     1001      127     2483 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md
--rw-r--r--   0     1001      127     2126 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/getting_started.md
--rw-r--r--   0     1001      127      477 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/README.md
--rw-r--r--   0     1001      127     1122 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg
--rw-r--r--   0     1001      127     3210 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/at.png
--rw-r--r--   0     1001      127      971 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg
--rw-r--r--   0     1001      127     2265 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png
--rw-r--r--   0     1001      127     1577 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg
--rw-r--r--   0     1001      127     2613 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png
--rw-r--r--   0     1001      127      837 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg
--rw-r--r--   0     1001      127     1540 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png
--rw-r--r--   0     1001      127      485 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cloud-solid.svg
--rw-r--r--   0     1001      127     1454 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png
--rw-r--r--   0     1001      127     2614 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg
--rw-r--r--   0     1001      127     2894 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png
--rw-r--r--   0     1001      127     1252 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg
--rw-r--r--   0     1001      127     2497 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png
--rw-r--r--   0     1001      127     6059 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png
--rw-r--r--   0     1001      127      467 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/video-solid.svg
--rw-r--r--   0     1001      127     1073 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/video.png
--rw-r--r--   0     1001      127     1060 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md
--rw-r--r--   0     1001      127      953 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/introduction.md
--rw-r--r--   0     1001      127     2800 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp
--rw-r--r--   0     1001      127      300 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_initial.cpp
--rw-r--r--   0     1001      127      877 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp
--rw-r--r--   0     1001      127     2636 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint
--rw-r--r--   0     1001      127     2130 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md
--rw-r--r--   0     1001      127      425 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tile.slint
--rw-r--r--   0     1001      127     2221 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint
--rw-r--r--   0     1001      127     2760 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md
--rw-r--r--   0     1001      127      262 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/book.toml
--rw-r--r--   0     1001      127      527 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/SUMMARY.md
--rw-r--r--   0     1001      127     1223 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/conclusion.md
--rw-r--r--   0     1001      127     1191 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md
--rw-r--r--   0     1001      127     2034 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md
--rw-r--r--   0     1001      127     2031 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md
--rw-r--r--   0     1001      127     1515 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/getting_started.md
--rw-r--r--   0     1001      127      477 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/README.md
--rw-r--r--   0     1001      127     1122 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg
--rw-r--r--   0     1001      127     3210 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/at.png
--rw-r--r--   0     1001      127      971 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg
--rw-r--r--   0     1001      127     2265 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png
--rw-r--r--   0     1001      127     1577 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg
--rw-r--r--   0     1001      127     2613 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png
--rw-r--r--   0     1001      127      837 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg
--rw-r--r--   0     1001      127     1540 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bus.png
--rw-r--r--   0     1001      127      485 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cloud-solid.svg
--rw-r--r--   0     1001      127     1454 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cloud.png
--rw-r--r--   0     1001      127     2614 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg
--rw-r--r--   0     1001      127     2894 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cogs.png
--rw-r--r--   0     1001      127     1252 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg
--rw-r--r--   0     1001      127     2497 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png
--rw-r--r--   0     1001      127     6059 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png
--rw-r--r--   0     1001      127      467 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/video-solid.svg
--rw-r--r--   0     1001      127     1073 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/video.png
--rw-r--r--   0     1001      127     1060 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md
--rw-r--r--   0     1001      127      960 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/introduction.md
--rw-r--r--   0     1001      127     1797 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_game_logic.js
--rw-r--r--   0     1001      127      275 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_initial.js
--rw-r--r--   0     1001      127      631 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js
--rw-r--r--   0     1001      127      265 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory.slint
--rw-r--r--   0     1001      127     2636 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint
--rw-r--r--   0     1001      127     2079 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tile.md
--rw-r--r--   0     1001      127      425 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tile.slint
--rw-r--r--   0     1001      127     2221 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint
--rw-r--r--   0     1001      127      202 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/package.json
--rw-r--r--   0     1001      127     2747 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md
--rw-r--r--   0     1001      127      262 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/rust/book.toml
--rw-r--r--   0     1001      127     3821 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/theme/head.hbs
--rw-r--r--   0     1001      127       84 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/theme/highlight.css
--rw-r--r--   0     1001      127      282 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/quickstart/theme/highlight.js
--rw-r--r--   0     1001      127      386 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/Pipfile
--rw-r--r--   0     1001      127      256 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/_static/theme_tweak.css
--rw-r--r--   0     1001      127      190 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/_templates/base.html
--rw-r--r--   0     1001      127     4339 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/conf.py
--rw-r--r--   0     1001      127      811 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/index.rst
--rw-r--r--   0     1001      127     7746 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md
--rw-r--r--   0     1001      127     1061 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_qt.md
--rw-r--r--   0     1001      127     1692 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_winit.md
--rw-r--r--   0     1001      127     7431 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md
--rw-r--r--   0     1001      127     6034 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md
--rw-r--r--   0     1001      127     3816 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/style.md
--rw-r--r--   0     1001      127     1095 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/introduction/index.md
--rw-r--r--   0     1001      127     2287 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/introduction/supported_platforms.md
--rw-r--r--   0     1001      127     1418 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/callbacks.md
--rw-r--r--   0     1001      127    42035 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/elements.md
--rw-r--r--   0     1001      127      975 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/functions.md
--rw-r--r--   0     1001      127     3227 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/globals.md
--rw-r--r--   0     1001      127      267 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/index.rst
--rw-r--r--   0     1001      127     3567 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/namespaces.md
--rw-r--r--   0     1001      127     1144 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/container.md
--rw-r--r--   0     1001      127     2165 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/file.md
--rw-r--r--   0     1001      127     2315 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/focus.md
--rw-r--r--   0     1001      127     1232 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/fonts.md
--rw-r--r--   0     1001      127      262 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/index.rst
--rw-r--r--   0     1001      127    13939 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/layouting.md
--rw-r--r--   0     1001      127     1787 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/purity.md
--rw-r--r--   0     1001      127     7822 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/translations.md
--rw-r--r--   0     1001      127     2235 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/index.rst
--rw-r--r--   0     1001      127     2270 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/animations.md
--rw-r--r--   0     1001      127     1627 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/callbacks.md
--rw-r--r--   0     1001      127      326 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/comments.md
--rw-r--r--   0     1001      127      492 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/conditions.md
--rw-r--r--   0     1001      127     1792 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/expressions.md
--rw-r--r--   0     1001      127     1821 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/functions.md
--rw-r--r--   0     1001      127     2776 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/globals.md
--rw-r--r--   0     1001      127      413 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/identifiers.md
--rw-r--r--   0     1001      127      402 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/index.rst
--rw-r--r--   0     1001      127      851 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md
--rw-r--r--   0     1001      127     3946 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/modules.md
--rw-r--r--   0     1001      127     5168 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/properties.md
--rw-r--r--   0     1001      127     1470 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/repetitions.md
--rw-r--r--   0     1001      127      658 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/statements.md
--rw-r--r--   0     1001      127     2210 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/states.md
--rw-r--r--   0     1001      127    17651 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/types.md
--rw-r--r--   0     1001      127      299 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/aboutslint.md
--rw-r--r--   0     1001      127     1469 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/button.md
--rw-r--r--   0     1001      127     1035 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/checkbox.md
--rw-r--r--   0     1001      127     1087 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/combobox.md
--rw-r--r--   0     1001      127      251 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/gridbox.md
--rw-r--r--   0     1001      127      741 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/groupbox.md
--rw-r--r--   0     1001      127      337 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/horizontalbox.md
--rw-r--r--   0     1001      127      569 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/index.rst
--rw-r--r--   0     1001      127     2460 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/lineedit.md
--rw-r--r--   0     1001      127     1293 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/listview.md
--rw-r--r--   0     1001      127      801 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md
--rw-r--r--   0     1001      127     1976 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/scrollview.md
--rw-r--r--   0     1001      127     1145 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/slider.md
--rw-r--r--   0     1001      127      866 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/spinbox.md
--rw-r--r--   0     1001      127      805 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/spinner.md
--rw-r--r--   0     1001      127     1071 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md
--rw-r--r--   0     1001      127     1489 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md
--rw-r--r--   0     1001      127     2176 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md
--rw-r--r--   0     1001      127     1037 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/switch.md
--rw-r--r--   0     1001      127      800 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md
--rw-r--r--   0     1001      127     2301 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/textedit.md
--rw-r--r--   0     1001      127      335 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/verticalbox.md
--rw-r--r--   0     1001      127      565 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/widgets.md
--rw-r--r--   0     1001      127      364 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/recipes/button_native.slint
--rw-r--r--   0     1001      127    28191 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/reference/src/recipes/recipes.md
--rw-r--r--   0     1001      127     3821 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/resources/slint-docs-highlight.html
--rw-r--r--   0     1001      127     5521 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/resources/slint-docs-preview.html
--rw-r--r--   0     1001      127    14477 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/site/index.html
--rw-r--r--   0     1001      127     3880 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/testing.md
--rw-r--r--   0     1001      127     1698 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/torizon.md
--rw-r--r--   0     1001      127     3775 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs/triage.md
--rw-r--r--   0     1001      127     6705 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/docs.rs
--rw-r--r--   0     1001      127    14341 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/lib.rs
--rw-r--r--   0     1001      127    20004 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/mcu.md
--rw-r--r--   0     1001      127     7565 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/private_unstable_api.rs
--rw-r--r--   0     1001      127     8976 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/tests/partial_renderer.rs
--rw-r--r--   0     1001      127      890 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/tests/show_strongref.rs
--rw-r--r--   0     1001      127     1147 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/tests/simple_macro.rs
--rw-r--r--   0     1001      127     2491 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/tests/spawn_local.rs
--rw-r--r--   0     1001      127     2557 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/slint/type-mappings.md
--rw-r--r--   0     1001      127     1109 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      740 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/README.md
--rw-r--r--   0     1001      127    34583 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/androidwindowadapter.rs
--rw-r--r--   0     1001      127     4464 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/build.rs
--rw-r--r--   0     1001      127    18055 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/java/SlintAndroidJavaHelper.java
--rw-r--r--   0     1001      127    18156 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/javahelper.rs
--rw-r--r--   0     1001      127     6133 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/android-activity/lib.rs
--rw-r--r--   0     1001      127      768 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127    15366 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/rs/build/lib.rs
--rw-r--r--   0     1001      127     1383 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      507 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/README.md
--rw-r--r--   0     1001      127    10783 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/accessible_generated.rs
--rw-r--r--   0     1001      127     2995 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/build.rs
--rw-r--r--   0     1001      127    27433 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/key_generated.rs
--rw-r--r--   0     1001      127    10534 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/lib.rs
--rw-r--r--   0     1001      127    32981 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_accessible.rs
--rw-r--r--   0     1001      127    21040 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/button.rs
--rw-r--r--   0     1001      127     6862 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/checkbox.rs
--rw-r--r--   0     1001      127     9594 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/combobox.rs
--rw-r--r--   0     1001      127     8992 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/groupbox.rs
--rw-r--r--   0     1001      127     5930 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/lineedit.rs
--rw-r--r--   0     1001      127     8178 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/listviewitem.rs
--rw-r--r--   0     1001      127     7422 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/palette.rs
--rw-r--r--   0     1001      127     4945 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/progress_indicator.rs
--rw-r--r--   0     1001      127    19794 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/scrollview.rs
--rw-r--r--   0     1001      127    13940 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/slider.rs
--rw-r--r--   0     1001      127    12535 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/spinbox.rs
--rw-r--r--   0     1001      127     8594 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/stylemetrics.rs
--rw-r--r--   0     1001      127     5637 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/tableheadersection.rs
--rw-r--r--   0     1001      127    22417 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets/tabwidget.rs
--rw-r--r--   0     1001      127    12967 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_widgets.rs
--rw-r--r--   0     1001      127   107271 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/backends/qt/qt_window.rs
--rw-r--r--   0     1001      127      532 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/Cargo.toml
--rw-r--r--   0     1001      127    34670 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0     1001      127     3475 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
--rw-r--r--   0     1001      127    14063 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md
--rw-r--r--   0     1001      127      590 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/README.md
--rw-r--r--   0     1001      127     7310 2024-05-03 06:06:50.000000 slint-1.6.0a7/internal/core-macros/lib.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 slint-1.6.0a7/api/python/Cargo.toml
--rw-r--r--   0     1001      127       11 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/.gitignore
--rw-r--r--   0     1001      127     7730 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/README.md
--rw-r--r--   0     1001      127     4367 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/brush.rs
--rw-r--r--   0     1001      127     3303 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/errors.rs
--rw-r--r--   0     1001      127     1399 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/image.rs
--rw-r--r--   0     1001      127    10939 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/interpreter.rs
--rw-r--r--   0     1001      127     1421 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/lib.rs
--rw-r--r--   0     1001      127     6300 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/models.rs
--rw-r--r--   0     1001      127      348 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/noxfile.py
--rw-r--r--   0     1001      127     7729 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/slint/__init__.py
--rw-r--r--   0     1001      127     1889 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/slint/models.py
--rw-r--r--   0     1001      127     1164 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_brush.py
--rw-r--r--   0     1001      127     1019 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_callback_decorators.py
--rw-r--r--   0     1001      127     2369 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_compiler.py
--rw-r--r--   0     1001      127     1095 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_gc.py
--rw-r--r--   0     1001      127     6577 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_instance.py
--rw-r--r--   0     1001      127     1597 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_load_file.py
--rw-r--r--   0     1001      127      905 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_load_file.slint
--rw-r--r--   0     1001      127      687 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_loader.py
--rw-r--r--   0     1001      127     3589 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_models.py
--rw-r--r--   0     1001      127      832 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/tests/test_timers.py
--rw-r--r--   0     1001      127     2415 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/timer.rs
--rw-r--r--   0     1001      127     4717 2024-05-03 06:06:50.000000 slint-1.6.0a7/api/python/value.rs
--rw-r--r--   0     1001      127   207946 2024-05-03 06:06:59.000000 slint-1.6.0a7/Cargo.lock
--rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 slint-1.6.0a7/Cargo.toml
--rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 slint-1.6.0a7/pyproject.toml
--rw-r--r--   0     1001      127     7729 2024-05-03 06:06:50.000000 slint-1.6.0a7/slint/__init__.py
--rw-r--r--   0     1001      127     1889 2024-05-03 06:06:50.000000 slint-1.6.0a7/slint/models.py
--rw-r--r--   0        0        0     9277 1970-01-01 00:00:00.000000 slint-1.6.0a7/PKG-INFO
+-rw-r--r--   0     1001      127     2389 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/selector/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/selector/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      872 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/selector/README.md
+-rw-r--r--   0     1001      127     2065 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/selector/build.rs
+-rw-r--r--   0     1001      127     5859 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/selector/lib.rs
+-rw-r--r--   0     1001      127      532 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core-macros/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core-macros/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      590 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core-macros/README.md
+-rw-r--r--   0     1001      127     7310 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core-macros/lib.rs
+-rw-r--r--   0     1001      127      706 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/macro/Cargo.toml
+-rw-r--r--   0     1001      127    12200 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/macro/macro.rs
+-rw-r--r--   0     1001      127     1685 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      740 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/README.md
+-rw-r--r--   0     1001      127    34583 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/androidwindowadapter.rs
+-rw-r--r--   0     1001      127     4464 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/build.rs
+-rw-r--r--   0     1001      127    18055 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/java/SlintAndroidJavaHelper.java
+-rw-r--r--   0     1001      127    18156 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/javahelper.rs
+-rw-r--r--   0     1001      127     6305 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/android-activity/lib.rs
+-rw-r--r--   0     1001      127     2855 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/README.md
+-rw-r--r--   0     1001      127     1037 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/build.rs
+-rw-r--r--   0     1001      127     6875 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/cached_image.rs
+-rw-r--r--   0     1001      127    14877 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/d3d_surface.rs
+-rw-r--r--   0     1001      127    37207 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/itemrenderer.rs
+-rw-r--r--   0     1001      127    23253 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/lib.rs
+-rw-r--r--   0     1001      127     6372 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/metal_surface.rs
+-rw-r--r--   0     1001      127    15370 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/opengl_surface.rs
+-rw-r--r--   0     1001      127     4611 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/software_surface.rs
+-rw-r--r--   0     1001      127    11843 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/textlayout.rs
+-rw-r--r--   0     1001      127    17420 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/skia/vulkan_surface.rs
+-rw-r--r--   0     1001      127     4502 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      532 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/README.md
+-rw-r--r--   0     1001      127     2766 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/accessibility.rs
+-rw-r--r--   0     1001      127    13996 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/animations.rs
+-rw-r--r--   0     1001      127    38650 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/api.rs
+-rw-r--r--   0     1001      127      349 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/build.rs
+-rw-r--r--   0     1001      127     5210 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/callbacks.rs
+-rw-r--r--   0     1001      127     2586 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/component_factory.rs
+-rw-r--r--   0     1001      127     2936 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/context.rs
+-rw-r--r--   0     1001      127     7695 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/future.rs
+-rw-r--r--   0     1001      127     2503 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/bitmapfont.rs
+-rw-r--r--   0     1001      127    14664 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/border_radius.rs
+-rw-r--r--   0     1001      127     4038 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/boxshadowcache.rs
+-rw-r--r--   0     1001      127    14919 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/brush.rs
+-rw-r--r--   0     1001      127    17436 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/color.rs
+-rw-r--r--   0     1001      127     7064 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/image/cache.rs
+-rw-r--r--   0     1001      127     2528 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/image/htmlimage.rs
+-rw-r--r--   0     1001      127     3408 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/image/svg.rs
+-rw-r--r--   0     1001      127    48855 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/image.rs
+-rw-r--r--   0     1001      127    15911 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/path.rs
+-rw-r--r--   0     1001      127     6978 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics/rendering_metrics_collector.rs
+-rw-r--r--   0     1001      127     8249 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/graphics.rs
+-rw-r--r--   0     1001      127    33891 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/input.rs
+-rw-r--r--   0     1001      127     8604 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/item_focus.rs
+-rw-r--r--   0     1001      127    32976 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/item_rendering.rs
+-rw-r--r--   0     1001      127    68108 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/item_tree.rs
+-rw-r--r--   0     1001      127     8608 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/items/component_container.rs
+-rw-r--r--   0     1001      127    17039 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/items/flickable.rs
+-rw-r--r--   0     1001      127     8722 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/items/image.rs
+-rw-r--r--   0     1001      127     5377 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/items/path.rs
+-rw-r--r--   0     1001      127    65922 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/items/text.rs
+-rw-r--r--   0     1001      127    46637 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/items.rs
+-rw-r--r--   0     1001      127    27945 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/layout.rs
+-rw-r--r--   0     1001      127     3347 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/lengths.rs
+-rw-r--r--   0     1001      127     2237 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/lib.rs
+-rw-r--r--   0     1001      127    47643 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/model/adapters.rs
+-rw-r--r--   0     1001      127     6658 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/model/model_peer.rs
+-rw-r--r--   0     1001      127    47304 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/model.rs
+-rw-r--r--   0     1001      127    16009 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/platform.rs
+-rw-r--r--   0     1001      127     7794 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/properties/change_tracker.rs
+-rw-r--r--   0     1001      127    18894 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/properties/ffi.rs
+-rw-r--r--   0     1001      127    38401 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/properties/properties_animations.rs
+-rw-r--r--   0     1001      127    59846 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/properties.rs
+-rw-r--r--   0     1001      127     5015 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/renderer.rs
+-rw-r--r--   0     1001      127    10886 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/rtti.rs
+-rw-r--r--   0     1001      127    21418 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/sharedvector.rs
+-rw-r--r--   0     1001      127     2865 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/slice.rs
+-rw-r--r--   0     1001      127    28862 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/software_renderer/draw_functions.rs
+-rw-r--r--   0     1001      127     3465 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/software_renderer/fixed.rs
+-rw-r--r--   0     1001      127     4673 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/software_renderer/fonts/pixelfont.rs
+-rw-r--r--   0     1001      127     3859 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/software_renderer/fonts/systemfonts.rs
+-rw-r--r--   0     1001      127     7334 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/software_renderer/fonts/vectorfont.rs
+-rw-r--r--   0     1001      127     5915 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/software_renderer/fonts.rs
+-rw-r--r--   0     1001      127   108310 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/software_renderer.rs
+-rw-r--r--   0     1001      127    13307 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/string.rs
+-rw-r--r--   0     1001      127     4182 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/tests.rs
+-rw-r--r--   0     1001      127    12929 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/textlayout/fragments.rs
+-rw-r--r--   0     1001      127     3222 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/textlayout/glyphclusters.rs
+-rw-r--r--   0     1001      127     1234 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/textlayout/linebreak_simple.rs
+-rw-r--r--   0     1001      127     1260 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/textlayout/linebreak_unicode.rs
+-rw-r--r--   0     1001      127    15364 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/textlayout/linebreaker.rs
+-rw-r--r--   0     1001      127    13512 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/textlayout/shaping.rs
+-rw-r--r--   0     1001      127    24952 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/textlayout.rs
+-rw-r--r--   0     1001      127    31757 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/timers.rs
+-rw-r--r--   0     1001      127     8992 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/translations.rs
+-rw-r--r--   0     1001      127     2876 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/unsafe_single_threaded.rs
+-rw-r--r--   0     1001      127    63165 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/core/window.rs
+-rw-r--r--   0     1001      127     1383 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/README.md
+-rw-r--r--   0     1001      127    10783 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/accessible_generated.rs
+-rw-r--r--   0     1001      127     3046 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/build.rs
+-rw-r--r--   0     1001      127    27433 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/key_generated.rs
+-rw-r--r--   0     1001      127    10534 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/lib.rs
+-rw-r--r--   0     1001      127    32981 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_accessible.rs
+-rw-r--r--   0     1001      127    21040 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/button.rs
+-rw-r--r--   0     1001      127     6862 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/checkbox.rs
+-rw-r--r--   0     1001      127     9594 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/combobox.rs
+-rw-r--r--   0     1001      127     8992 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/groupbox.rs
+-rw-r--r--   0     1001      127     5930 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/lineedit.rs
+-rw-r--r--   0     1001      127     8178 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/listviewitem.rs
+-rw-r--r--   0     1001      127     7422 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/palette.rs
+-rw-r--r--   0     1001      127     4945 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/progress_indicator.rs
+-rw-r--r--   0     1001      127    19794 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/scrollview.rs
+-rw-r--r--   0     1001      127    14001 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/slider.rs
+-rw-r--r--   0     1001      127    12535 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/spinbox.rs
+-rw-r--r--   0     1001      127     8594 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/stylemetrics.rs
+-rw-r--r--   0     1001      127     5637 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/tableheadersection.rs
+-rw-r--r--   0     1001      127    22417 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets/tabwidget.rs
+-rw-r--r--   0     1001      127    12967 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_widgets.rs
+-rw-r--r--   0     1001      127   107271 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/qt/qt_window.rs
+-rw-r--r--   0     1001      127      826 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/testing/Cargo.toml
+-rw-r--r--   0     1001      127     4705 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/testing/README.md
+-rw-r--r--   0     1001      127      845 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/testing/ffi.rs
+-rw-r--r--   0     1001      127     2990 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/testing/internal_tests.rs
+-rw-r--r--   0     1001      127     1695 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/testing/lib.rs
+-rw-r--r--   0     1001      127     7111 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/testing/search_api.rs
+-rw-r--r--   0     1001      127     6991 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/testing/testing_backend.rs
+-rw-r--r--   0     1001      127     1126 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     8815 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      635 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/README.md
+-rw-r--r--   0     1001      127     7636 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/builtin_structs.rs
+-rw-r--r--   0     1001      127    19656 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/enums.rs
+-rw-r--r--   0     1001      127     8311 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/key_codes.rs
+-rw-r--r--   0     1001      127     1322 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/lib.rs
+-rw-r--r--   0     1001      127   757076 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/sharedfontdb/DejaVuSans.ttf
+-rw-r--r--   0     1001      127      145 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/sharedfontdb/DejaVuSans.ttf.license
+-rw-r--r--   0     1001      127     4526 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/sharedfontdb/fontconfig.rs
+-rw-r--r--   0     1001      127     7491 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/common/sharedfontdb.rs
+-rw-r--r--   0     1001      127      630 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/Cargo.toml
+-rw-r--r--   0     1001      127      610 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/CHANGELOG.md
+-rw-r--r--   0     1001      127    10280 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      492 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/README.md
+-rw-r--r--   0     1001      127     6982 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/src/lib.rs
+-rw-r--r--   0     1001      127     4766 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/const-field-offset/tests/test_field_offset.rs
+-rw-r--r--   0     1001      127      623 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/Cargo.toml
+-rw-r--r--   0     1001      127     1796 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/CHANGELOG.md
+-rw-r--r--   0     1001      127    10280 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      399 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/README.md
+-rw-r--r--   0     1001      127     3723 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/src/compile_fail_tests.rs
+-rw-r--r--   0     1001      127    18776 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/src/lib.rs
+-rw-r--r--   0     1001      127    18973 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/src/vrc.rs
+-rw-r--r--   0     1001      127     9552 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/tests/test_vrc.rs
+-rw-r--r--   0     1001      127     5359 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/tests/test_vtable.rs
+-rw-r--r--   0     1001      127      768 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/build/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/build/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127    15366 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/build/lib.rs
+-rw-r--r--   0     1001      127      571 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/macro/Cargo.toml
+-rw-r--r--   0     1001      127    10280 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127     1078 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/macro/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127    31635 2024-05-13 09:35:19.000000 slint-1.6.0a8/helper_crates/vtable/macro/macro.rs
+-rw-r--r--   0     1001      127      471 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser-test-macro/Cargo.toml
+-rw-r--r--   0     1001      127      887 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser-test-macro/README.md
+-rw-r--r--   0     1001      127     5619 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser-test-macro/lib.rs
+-rw-r--r--   0     1001      127    10200 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127     1881 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/README.md
+-rw-r--r--   0     1001      127     5252 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/android.rs
+-rw-r--r--   0     1001      127      548 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/compile_fail_tests.rs
+-rw-r--r--   0     1001      127     9447 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/building.md
+-rw-r--r--   0     1001      127     7147 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/development.md
+-rw-r--r--   0     1001      127     2881 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/install_qt.md
+-rw-r--r--   0     1001      127        5 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/.gitignore
+-rw-r--r--   0     1001      127     1013 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/README.md
+-rw-r--r--   0     1001      127      261 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/book.toml
+-rw-r--r--   0     1001      127      810 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt
+-rw-r--r--   0     1001      127      515 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md
+-rw-r--r--   0     1001      127      268 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/appwindow.slint
+-rw-r--r--   0     1001      127     1216 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/conclusion.md
+-rw-r--r--   0     1001      127     1337 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md
+-rw-r--r--   0     1001      127     2039 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md
+-rw-r--r--   0     1001      127     2483 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md
+-rw-r--r--   0     1001      127     2126 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/getting_started.md
+-rw-r--r--   0     1001      127      477 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/README.md
+-rw-r--r--   0     1001      127     1122 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg
+-rw-r--r--   0     1001      127     3210 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/at.png
+-rw-r--r--   0     1001      127      971 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg
+-rw-r--r--   0     1001      127     2265 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png
+-rw-r--r--   0     1001      127     1577 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg
+-rw-r--r--   0     1001      127     2613 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png
+-rw-r--r--   0     1001      127      837 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg
+-rw-r--r--   0     1001      127     1540 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png
+-rw-r--r--   0     1001      127      485 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/cloud-solid.svg
+-rw-r--r--   0     1001      127     1454 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png
+-rw-r--r--   0     1001      127     2614 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg
+-rw-r--r--   0     1001      127     2894 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png
+-rw-r--r--   0     1001      127     1252 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg
+-rw-r--r--   0     1001      127     2497 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png
+-rw-r--r--   0     1001      127     6059 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png
+-rw-r--r--   0     1001      127      467 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/video-solid.svg
+-rw-r--r--   0     1001      127     1073 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/video.png
+-rw-r--r--   0     1001      127     1060 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md
+-rw-r--r--   0     1001      127      953 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/introduction.md
+-rw-r--r--   0     1001      127     2800 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp
+-rw-r--r--   0     1001      127      300 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/main_initial.cpp
+-rw-r--r--   0     1001      127      877 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp
+-rw-r--r--   0     1001      127     2636 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint
+-rw-r--r--   0     1001      127     2130 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md
+-rw-r--r--   0     1001      127      425 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/memory_tile.slint
+-rw-r--r--   0     1001      127     2221 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint
+-rw-r--r--   0     1001      127     2760 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md
+-rw-r--r--   0     1001      127      262 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/book.toml
+-rw-r--r--   0     1001      127      527 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/SUMMARY.md
+-rw-r--r--   0     1001      127     1223 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/conclusion.md
+-rw-r--r--   0     1001      127     1191 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md
+-rw-r--r--   0     1001      127     2034 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md
+-rw-r--r--   0     1001      127     2031 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md
+-rw-r--r--   0     1001      127     1515 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/getting_started.md
+-rw-r--r--   0     1001      127      477 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/README.md
+-rw-r--r--   0     1001      127     1122 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg
+-rw-r--r--   0     1001      127     3210 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/at.png
+-rw-r--r--   0     1001      127      971 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg
+-rw-r--r--   0     1001      127     2265 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png
+-rw-r--r--   0     1001      127     1577 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg
+-rw-r--r--   0     1001      127     2613 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png
+-rw-r--r--   0     1001      127      837 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg
+-rw-r--r--   0     1001      127     1540 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/bus.png
+-rw-r--r--   0     1001      127      485 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/cloud-solid.svg
+-rw-r--r--   0     1001      127     1454 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/cloud.png
+-rw-r--r--   0     1001      127     2614 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg
+-rw-r--r--   0     1001      127     2894 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/cogs.png
+-rw-r--r--   0     1001      127     1252 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg
+-rw-r--r--   0     1001      127     2497 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png
+-rw-r--r--   0     1001      127     6059 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png
+-rw-r--r--   0     1001      127      467 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/video-solid.svg
+-rw-r--r--   0     1001      127     1073 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/video.png
+-rw-r--r--   0     1001      127     1060 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md
+-rw-r--r--   0     1001      127      960 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/introduction.md
+-rw-r--r--   0     1001      127     1797 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/main_game_logic.js
+-rw-r--r--   0     1001      127      275 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/main_initial.js
+-rw-r--r--   0     1001      127      631 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js
+-rw-r--r--   0     1001      127      265 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/memory.slint
+-rw-r--r--   0     1001      127     2636 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint
+-rw-r--r--   0     1001      127     2079 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/memory_tile.md
+-rw-r--r--   0     1001      127      425 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/memory_tile.slint
+-rw-r--r--   0     1001      127     2221 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint
+-rw-r--r--   0     1001      127      202 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/package.json
+-rw-r--r--   0     1001      127     2747 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md
+-rw-r--r--   0     1001      127      262 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/rust/book.toml
+-rw-r--r--   0     1001      127     3821 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/theme/head.hbs
+-rw-r--r--   0     1001      127       84 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/theme/highlight.css
+-rw-r--r--   0     1001      127      282 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/quickstart/theme/highlight.js
+-rw-r--r--   0     1001      127      386 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/Pipfile
+-rw-r--r--   0     1001      127      256 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/_static/theme_tweak.css
+-rw-r--r--   0     1001      127      190 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/_templates/base.html
+-rw-r--r--   0     1001      127     4339 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/conf.py
+-rw-r--r--   0     1001      127      811 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/index.rst
+-rw-r--r--   0     1001      127     7746 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md
+-rw-r--r--   0     1001      127     1469 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/backend_qt.md
+-rw-r--r--   0     1001      127     1932 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/backend_winit.md
+-rw-r--r--   0     1001      127     7431 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md
+-rw-r--r--   0     1001      127     6034 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md
+-rw-r--r--   0     1001      127     3816 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/style.md
+-rw-r--r--   0     1001      127     1095 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/introduction/index.md
+-rw-r--r--   0     1001      127     2287 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/introduction/supported_platforms.md
+-rw-r--r--   0     1001      127     1418 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/callbacks.md
+-rw-r--r--   0     1001      127    42035 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/elements.md
+-rw-r--r--   0     1001      127      975 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/functions.md
+-rw-r--r--   0     1001      127     3227 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/globals.md
+-rw-r--r--   0     1001      127      267 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/index.rst
+-rw-r--r--   0     1001      127     3586 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/namespaces.md
+-rw-r--r--   0     1001      127     1144 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/container.md
+-rw-r--r--   0     1001      127     2165 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/file.md
+-rw-r--r--   0     1001      127     2315 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/focus.md
+-rw-r--r--   0     1001      127     1232 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/fonts.md
+-rw-r--r--   0     1001      127      262 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/index.rst
+-rw-r--r--   0     1001      127    13939 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/layouting.md
+-rw-r--r--   0     1001      127     1787 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/purity.md
+-rw-r--r--   0     1001      127     7822 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/translations.md
+-rw-r--r--   0     1001      127     2235 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/index.rst
+-rw-r--r--   0     1001      127     2270 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/animations.md
+-rw-r--r--   0     1001      127     1627 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/callbacks.md
+-rw-r--r--   0     1001      127      326 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/comments.md
+-rw-r--r--   0     1001      127      492 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/conditions.md
+-rw-r--r--   0     1001      127     1792 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/expressions.md
+-rw-r--r--   0     1001      127     1821 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/functions.md
+-rw-r--r--   0     1001      127     2776 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/globals.md
+-rw-r--r--   0     1001      127      413 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/identifiers.md
+-rw-r--r--   0     1001      127      402 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/index.rst
+-rw-r--r--   0     1001      127      851 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md
+-rw-r--r--   0     1001      127     3946 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/modules.md
+-rw-r--r--   0     1001      127     5168 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/properties.md
+-rw-r--r--   0     1001      127     1470 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/repetitions.md
+-rw-r--r--   0     1001      127      658 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/statements.md
+-rw-r--r--   0     1001      127     2210 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/states.md
+-rw-r--r--   0     1001      127    17651 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/types.md
+-rw-r--r--   0     1001      127      299 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/aboutslint.md
+-rw-r--r--   0     1001      127     1469 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/button.md
+-rw-r--r--   0     1001      127     1035 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/checkbox.md
+-rw-r--r--   0     1001      127     1087 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/combobox.md
+-rw-r--r--   0     1001      127      251 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/gridbox.md
+-rw-r--r--   0     1001      127      741 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/groupbox.md
+-rw-r--r--   0     1001      127      337 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/horizontalbox.md
+-rw-r--r--   0     1001      127      569 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/index.rst
+-rw-r--r--   0     1001      127     2460 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/lineedit.md
+-rw-r--r--   0     1001      127     1293 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/listview.md
+-rw-r--r--   0     1001      127      801 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md
+-rw-r--r--   0     1001      127     1976 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/scrollview.md
+-rw-r--r--   0     1001      127     1145 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/slider.md
+-rw-r--r--   0     1001      127      866 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/spinbox.md
+-rw-r--r--   0     1001      127      805 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/spinner.md
+-rw-r--r--   0     1001      127     1071 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md
+-rw-r--r--   0     1001      127     1489 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md
+-rw-r--r--   0     1001      127     2176 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md
+-rw-r--r--   0     1001      127     1037 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/switch.md
+-rw-r--r--   0     1001      127      800 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md
+-rw-r--r--   0     1001      127     2301 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/textedit.md
+-rw-r--r--   0     1001      127      335 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/verticalbox.md
+-rw-r--r--   0     1001      127      565 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/widgets.md
+-rw-r--r--   0     1001      127      364 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/recipes/button_native.slint
+-rw-r--r--   0     1001      127    28191 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/reference/src/recipes/recipes.md
+-rw-r--r--   0     1001      127     3821 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/resources/slint-docs-highlight.html
+-rw-r--r--   0     1001      127     5521 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/resources/slint-docs-preview.html
+-rw-r--r--   0     1001      127    14477 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/site/index.html
+-rw-r--r--   0     1001      127     3880 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/testing.md
+-rw-r--r--   0     1001      127     1698 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/torizon.md
+-rw-r--r--   0     1001      127     3775 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs/triage.md
+-rw-r--r--   0     1001      127     6705 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/docs.rs
+-rw-r--r--   0     1001      127    14419 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/lib.rs
+-rw-r--r--   0     1001      127    20004 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/mcu.md
+-rw-r--r--   0     1001      127     7565 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/private_unstable_api.rs
+-rw-r--r--   0     1001      127     8976 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/tests/partial_renderer.rs
+-rw-r--r--   0     1001      127      890 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/tests/show_strongref.rs
+-rw-r--r--   0     1001      127     1147 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/tests/simple_macro.rs
+-rw-r--r--   0     1001      127     2491 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/tests/spawn_local.rs
+-rw-r--r--   0     1001      127     2557 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/slint/type-mappings.md
+-rw-r--r--   0     1001      127     1931 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      507 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/README.md
+-rw-r--r--   0     1001      127    15614 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/calloop_backend/input.rs
+-rw-r--r--   0     1001      127    11770 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/calloop_backend.rs
+-rw-r--r--   0     1001      127     8655 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/display/gbmdisplay.rs
+-rw-r--r--   0     1001      127     2955 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/display/swdisplay.rs
+-rw-r--r--   0     1001      127     9345 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/display/vulkandisplay.rs
+-rw-r--r--   0     1001      127     3237 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/display.rs
+-rw-r--r--   0     1001      127    11904 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/drmoutput.rs
+-rw-r--r--   0     1001      127     6253 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/fullscreenwindowadapter.rs
+-rw-r--r--   0     1001      127     2022 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/lib.rs
+-rw-r--r--   0     1001      127      365 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/mouse-pointer.svg
+-rw-r--r--   0     1001      127      882 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/noop_backend.rs
+-rw-r--r--   0     1001      127     7507 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/renderer/femtovg.rs
+-rw-r--r--   0     1001      127     6654 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/linuxkms/renderer/skia.rs
+-rw-r--r--   0     1001      127     1913 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/Cargo.toml
+-rw-r--r--   0     1001      127    10280 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/LICENSES/Apache-2.0.txt
+-rw-r--r--   0     1001      127    16830 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/LICENSES/CC-BY-ND-4.0.txt
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     1078 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/LICENSES/MIT.txt
+-rw-r--r--   0     1001      127      537 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/README.md
+-rw-r--r--   0     1001      127     2486 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/build.rs
+-rw-r--r--   0     1001      127    17516 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/builtin_macros.rs
+-rw-r--r--   0     1001      127    18500 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/builtins.slint
+-rw-r--r--   0     1001      127    19681 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/diagnostics.rs
+-rw-r--r--   0     1001      127     2636 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/embedded_resources.rs
+-rw-r--r--   0     1001      127    70005 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/expression_tree.rs
+-rw-r--r--   0     1001      127     4420 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/fileaccess.rs
+-rw-r--r--   0     1001      127   141236 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/generator/cpp.rs
+-rw-r--r--   0     1001      127   123809 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/generator/rust.rs
+-rw-r--r--   0     1001      127    19509 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/generator.rs
+-rw-r--r--   0     1001      127    32752 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/langtype.rs
+-rw-r--r--   0     1001      127    21425 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/layout.rs
+-rw-r--r--   0     1001      127    15374 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/lexer.rs
+-rw-r--r--   0     1001      127     9358 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/lib.rs
+-rw-r--r--   0     1001      127     7020 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/literals.rs
+-rw-r--r--   0     1001      127    31386 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/llr/expression.rs
+-rw-r--r--   0     1001      127    13532 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/llr/item_tree.rs
+-rw-r--r--   0     1001      127    40541 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/llr/lower_expression.rs
+-rw-r--r--   0     1001      127    31937 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/llr/lower_to_item_tree.rs
+-rw-r--r--   0     1001      127     6503 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/llr/optim_passes/count_property_use.rs
+-rw-r--r--   0     1001      127     6269 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/llr/optim_passes/inline_expressions.rs
+-rw-r--r--   0     1001      127    11380 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/llr/pretty_print.rs
+-rw-r--r--   0     1001      127      654 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/llr.rs
+-rw-r--r--   0     1001      127    11761 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/load_builtins.rs
+-rw-r--r--   0     1001      127    39782 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/lookup.rs
+-rw-r--r--   0     1001      127     7518 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/namedreference.rs
+-rw-r--r--   0     1001      127   103450 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/object_tree.rs
+-rw-r--r--   0     1001      127    10913 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser/document.rs
+-rw-r--r--   0     1001      127    21286 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser/element.rs
+-rw-r--r--   0     1001      127    14696 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser/expressions.rs
+-rw-r--r--   0     1001      127     3102 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser/statements.rs
+-rw-r--r--   0     1001      127     4561 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser/type.rs
+-rw-r--r--   0     1001      127    36374 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/parser.rs
+-rw-r--r--   0     1001      127     3949 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/apply_default_properties_from_style.rs
+-rw-r--r--   0     1001      127    22379 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/binding_analysis.rs
+-rw-r--r--   0     1001      127     1587 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/border_radius.rs
+-rw-r--r--   0     1001      127     1793 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/check_expressions.rs
+-rw-r--r--   0     1001      127     1941 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/check_public_api.rs
+-rw-r--r--   0     1001      127     2309 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/check_rotation.rs
+-rw-r--r--   0     1001      127     4580 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/clip.rs
+-rw-r--r--   0     1001      127     2464 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/collect_custom_fonts.rs
+-rw-r--r--   0     1001      127     1933 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/collect_globals.rs
+-rw-r--r--   0     1001      127     1150 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/collect_init_code.rs
+-rw-r--r--   0     1001      127     4172 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/collect_structs_and_enums.rs
+-rw-r--r--   0     1001      127     1690 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/collect_subcomponents.rs
+-rw-r--r--   0     1001      127     8043 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/compile_paths.rs
+-rw-r--r--   0     1001      127     9466 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/const_propagation.rs
+-rw-r--r--   0     1001      127     6155 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/deduplicate_property_read.rs
+-rw-r--r--   0     1001      127    18877 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/default_geometry.rs
+-rw-r--r--   0     1001      127    16263 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/embed_glyphs.rs
+-rw-r--r--   0     1001      127    14883 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/embed_images.rs
+-rw-r--r--   0     1001      127     5157 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/ensure_window.rs
+-rw-r--r--   0     1001      127     6270 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/flickable.rs
+-rw-r--r--   0     1001      127    11618 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/focus_handling.rs
+-rw-r--r--   0     1001      127     4318 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/generate_item_indices.rs
+-rw-r--r--   0     1001      127     6712 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/infer_aliases_types.rs
+-rw-r--r--   0     1001      127    21516 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/inlining.rs
+-rw-r--r--   0     1001      127     3241 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_absolute_coordinates.rs
+-rw-r--r--   0     1001      127     3268 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_accessibility.rs
+-rw-r--r--   0     1001      127     1697 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_component_container.rs
+-rw-r--r--   0     1001      127    31672 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_layout.rs
+-rw-r--r--   0     1001      127     6740 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_popups.rs
+-rw-r--r--   0     1001      127     5182 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_property_to_element.rs
+-rw-r--r--   0     1001      127     6919 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_shadows.rs
+-rw-r--r--   0     1001      127     9988 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_states.rs
+-rw-r--r--   0     1001      127     8355 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_tabwidget.rs
+-rw-r--r--   0     1001      127     2000 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/lower_text_input_interface.rs
+-rw-r--r--   0     1001      127     6310 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/materialize_fake_properties.rs
+-rw-r--r--   0     1001      127     7514 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/move_declarations.rs
+-rw-r--r--   0     1001      127     2749 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/optimize_useless_rectangles.rs
+-rw-r--r--   0     1001      127     4231 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/purity_check.rs
+-rw-r--r--   0     1001      127     9197 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/remove_aliases.rs
+-rw-r--r--   0     1001      127    19427 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/remove_return.rs
+-rw-r--r--   0     1001      127     1656 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/remove_unused_properties.rs
+-rw-r--r--   0     1001      127     5145 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/repeater_component.rs
+-rw-r--r--   0     1001      127     5615 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/resolve_native_classes.rs
+-rw-r--r--   0     1001      127    71031 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/resolving.rs
+-rw-r--r--   0     1001      127     3049 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/unique_id.rs
+-rw-r--r--   0     1001      127     4210 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/visible.rs
+-rw-r--r--   0     1001      127     2961 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes/z_order.rs
+-rw-r--r--   0     1001      127    10740 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/passes.rs
+-rw-r--r--   0     1001      127    18378 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/pathutils.rs
+-rw-r--r--   0     1001      127     8812 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/consistent_styles.rs
+-rw-r--r--   0     1001      127     1237 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/accessibility/accessible_properties.slint
+-rw-r--r--   0     1001      127     1774 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop1.slint
+-rw-r--r--   0     1001      127     1826 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop2.slint
+-rw-r--r--   0     1001      127      924 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_function.slint
+-rw-r--r--   0     1001      127      643 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint
+-rw-r--r--   0     1001      127     2458 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint
+-rw-r--r--   0     1001      127     1854 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint
+-rw-r--r--   0     1001      127     1144 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint
+-rw-r--r--   0     1001      127     2120 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint
+-rw-r--r--   0     1001      127      488 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_mappointtowindow.slint
+-rw-r--r--   0     1001      127      923 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_self.slint
+-rw-r--r--   0     1001      127      942 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/animate.slint
+-rw-r--r--   0     1001      127      230 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/array.slint
+-rw-r--r--   0     1001      127      788 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/assign.slint
+-rw-r--r--   0     1001      127      585 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/box_shadow.slint
+-rw-r--r--   0     1001      127     1021 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/children_placeholder.slint
+-rw-r--r--   0     1001      127      301 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/children_placeholder_2.slint
+-rw-r--r--   0     1001      127      663 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/clip.slint
+-rw-r--r--   0     1001      127      492 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/comments.slint
+-rw-r--r--   0     1001      127     2078 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/dialog.slint
+-rw-r--r--   0     1001      127      631 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/dialog2.slint
+-rw-r--r--   0     1001      127      499 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/double_binding.slint
+-rw-r--r--   0     1001      127      270 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/double_color.slint
+-rw-r--r--   0     1001      127     1137 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/duplicated_id.slint
+-rw-r--r--   0     1001      127     1340 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/easing.slint
+-rw-r--r--   0     1001      127      383 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/easing_not_called.slint
+-rw-r--r--   0     1001      127      156 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/empty.slint
+-rw-r--r--   0     1001      127      526 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/enums.slint
+-rw-r--r--   0     1001      127      441 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/for.slint
+-rw-r--r--   0     1001      127      492 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/image.slint
+-rw-r--r--   0     1001      127      450 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/inline_component.slint
+-rw-r--r--   0     1001      127      895 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/item_as_property.slint
+-rw-r--r--   0     1001      127      465 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/layout.slint
+-rw-r--r--   0     1001      127     1958 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/layout2.slint
+-rw-r--r--   0     1001      127     2188 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/linear-gradient.slint
+-rw-r--r--   0     1001      127      470 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/object_in_binding.slint
+-rw-r--r--   0     1001      127      538 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/opacity.slint
+-rw-r--r--   0     1001      127      905 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/parse_error.slint
+-rw-r--r--   0     1001      127      535 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/path.slint
+-rw-r--r--   0     1001      127     1114 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/path_commands.slint
+-rw-r--r--   0     1001      127      541 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/path_for.slint
+-rw-r--r--   0     1001      127     1056 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/percent.slint
+-rw-r--r--   0     1001      127      707 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/popup.slint
+-rw-r--r--   0     1001      127      333 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/property_animation.slint
+-rw-r--r--   0     1001      127      983 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/property_declaration.slint
+-rw-r--r--   0     1001      127      268 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/property_declaration_in_component.slint
+-rw-r--r--   0     1001      127     1786 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/radial-gradient.slint
+-rw-r--r--   0     1001      127      837 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/return.slint
+-rw-r--r--   0     1001      127     1850 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/rotation.slint
+-rw-r--r--   0     1001      127      456 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/rust-attr.slint
+-rw-r--r--   0     1001      127     1781 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/self_assign.slint
+-rw-r--r--   0     1001      127     1529 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/signal.slint
+-rw-r--r--   0     1001      127     4436 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/states_transitions.slint
+-rw-r--r--   0     1001      127      711 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/states_transitions2.slint
+-rw-r--r--   0     1001      127      748 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/states_transitions3.slint
+-rw-r--r--   0     1001      127      731 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/states_two_way.slint
+-rw-r--r--   0     1001      127      731 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/sub_elements.slint
+-rw-r--r--   0     1001      127      218 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/supersimple.slint
+-rw-r--r--   0     1001      127      467 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/svg_path.slint
+-rw-r--r--   0     1001      127     1600 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/tr.slint
+-rw-r--r--   0     1001      127     3038 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/tr2.slint
+-rw-r--r--   0     1001      127     1108 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/type_declaration.slint
+-rw-r--r--   0     1001      127     1391 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/basic/unknown_item.slint
+-rw-r--r--   0     1001      127      457 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/callbacks/init.slint
+-rw-r--r--   0     1001      127      552 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/callbacks/property-changes.slint
+-rw-r--r--   0     1001      127      671 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/elements/component_container.slint
+-rw-r--r--   0     1001      127     1202 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/elements/listview.slint
+-rw-r--r--   0     1001      127      601 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/elements/popup.slint
+-rw-r--r--   0     1001      127      470 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/elements/popup2.slint
+-rw-r--r--   0     1001      127      538 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/elements/tabwidget.slint
+-rw-r--r--   0     1001      127      898 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/elements/tabwidget2.slint
+-rw-r--r--   0     1001      127      474 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/elements/tabwidget3.slint
+-rw-r--r--   0     1001      127      436 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/exports/export_duplicates.slint
+-rw-r--r--   0     1001      127      623 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/exports/reexport_duplicate.slint
+-rw-r--r--   0     1001      127      326 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/exports/root_compo_export.slint
+-rw-r--r--   0     1001      127      289 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/exports/root_compo_export2.slint
+-rw-r--r--   0     1001      127      332 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/exports/single_global_missing_export.slint
+-rw-r--r--   0     1001      127      288 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/exports/unused_compo.slint
+-rw-r--r--   0     1001      127     1464 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/arithmetic_op.slint
+-rw-r--r--   0     1001      127     1261 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/clamp.slint
+-rw-r--r--   0     1001      127      999 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/comparison_operator.slint
+-rw-r--r--   0     1001      127     1473 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/condition_operator.slint
+-rw-r--r--   0     1001      127     3442 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/image-url.slint
+-rw-r--r--   0     1001      127     1090 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/image-url2.slint
+-rw-r--r--   0     1001      127     1486 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/math-macro.slint
+-rw-r--r--   0     1001      127     1355 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/minmax.slint
+-rw-r--r--   0     1001      127      654 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/percent2.slint
+-rw-r--r--   0     1001      127      456 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/strings.slint
+-rw-r--r--   0     1001      127     1221 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/expressions/unary_op.slint
+-rw-r--r--   0     1001      127      387 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/focus/focus_invalid.slint
+-rw-r--r--   0     1001      127     1078 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/focus/focus_not_called.slint
+-rw-r--r--   0     1001      127      705 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/focus/focus_wrong_args.slint
+-rw-r--r--   0     1001      127     1707 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint
+-rw-r--r--   0     1001      127      592 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/functions/function_double_qualified.slint
+-rw-r--r--   0     1001      127     1814 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/functions/functions.slint
+-rw-r--r--   0     1001      127     2990 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/functions/functions_call.slint
+-rw-r--r--   0     1001      127     3353 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/functions/functions_purity.slint
+-rw-r--r--   0     1001      127      597 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/bug_2719.slint
+-rw-r--r--   0     1001      127     1018 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint
+-rw-r--r--   0     1001      127      407 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/cyclic_import.slint
+-rw-r--r--   0     1001      127      441 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/error_in_import.slint
+-rw-r--r--   0     1001      127      252 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/error_in_import2.slint
+-rw-r--r--   0     1001      127      295 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/error_in_import3.slint
+-rw-r--r--   0     1001      127      410 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/font.slint
+-rw-r--r--   0     1001      127      393 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_builtin.slint
+-rw-r--r--   0     1001      127      411 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_error2.slint
+-rw-r--r--   0     1001      127      944 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_errors.slint
+-rw-r--r--   0     1001      127      207 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_parse_error1.slint
+-rw-r--r--   0     1001      127      221 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_parse_error2.slint
+-rw-r--r--   0     1001      127      238 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_parse_error3.slint
+-rw-r--r--   0     1001      127      239 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_parse_error4.slint
+-rw-r--r--   0     1001      127      503 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_parse_error5.slint
+-rw-r--r--   0     1001      127      472 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/invalid_export.slint
+-rw-r--r--   0     1001      127      379 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/imports/visibility_errors.slint
+-rw-r--r--   0     1001      127      703 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/layout/if_in_grid.slint
+-rw-r--r--   0     1001      127      441 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/layout/if_in_grid_row.slint
+-rw-r--r--   0     1001      127      586 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/layout/min_max_conflict.slint
+-rw-r--r--   0     1001      127      655 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/layout/spacing.slint
+-rw-r--r--   0     1001      127      477 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/absolute-position.slint
+-rw-r--r--   0     1001      127      691 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/array_index.slint
+-rw-r--r--   0     1001      127      594 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_alias.slint
+-rw-r--r--   0     1001      127      641 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_alias2.slint
+-rw-r--r--   0     1001      127     1221 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_alias3.slint
+-rw-r--r--   0     1001      127      255 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_alias_issue4938.slint
+-rw-r--r--   0     1001      127      376 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_not_called.slint
+-rw-r--r--   0     1001      127      433 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_return.slint
+-rw-r--r--   0     1001      127     1814 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/color.slint
+-rw-r--r--   0     1001      127     3112 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/conversion.slint
+-rw-r--r--   0     1001      127     1807 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/dashes.slint
+-rw-r--r--   0     1001      127     1250 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/deprecated_property.slint
+-rw-r--r--   0     1001      127     1138 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/enum.slint
+-rw-r--r--   0     1001      127     2598 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/for_lookup.slint
+-rw-r--r--   0     1001      127     1211 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/global.slint
+-rw-r--r--   0     1001      127      621 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/if.slint
+-rw-r--r--   0     1001      127      920 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/issue_1461.slint
+-rw-r--r--   0     1001      127     1287 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/property.slint
+-rw-r--r--   0     1001      127     1704 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint
+-rw-r--r--   0     1001      127     1439 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/signal_arg.slint
+-rw-r--r--   0     1001      127     1444 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/two_way_binding.slint
+-rw-r--r--   0     1001      127     1220 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint
+-rw-r--r--   0     1001      127      392 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/lookup/two_way_binding_model.slint
+-rw-r--r--   0     1001      127      903 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint
+-rw-r--r--   0     1001      127     2695 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/input_output.slint
+-rw-r--r--   0     1001      127     3062 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/input_output2.slint
+-rw-r--r--   0     1001      127      593 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/new_component.slint
+-rw-r--r--   0     1001      127     1020 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/new_lookup.slint
+-rw-r--r--   0     1001      127     8651 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint
+-rw-r--r--   0     1001      127      252 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/children_placeholder0.slint
+-rw-r--r--   0     1001      127      263 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/export0.slint
+-rw-r--r--   0     1001      127      219 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/export1.slint
+-rw-r--r--   0     1001      127      362 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/if0.slint
+-rw-r--r--   0     1001      127      278 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/if1.slint
+-rw-r--r--   0     1001      127      285 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/if2.slint
+-rw-r--r--   0     1001      127      224 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/if3.slint
+-rw-r--r--   0     1001      127      361 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/if4.slint
+-rw-r--r--   0     1001      127      398 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/property1.slint
+-rw-r--r--   0     1001      127      902 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/property2.slint
+-rw-r--r--   0     1001      127      846 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/state1.slint
+-rw-r--r--   0     1001      127      244 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/state2.slint
+-rw-r--r--   0     1001      127      307 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/state3.slint
+-rw-r--r--   0     1001      127      707 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/struct.slint
+-rw-r--r--   0     1001      127     9418 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/syntax_tests.rs
+-rw-r--r--   0     1001      127      156 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/custom_style/TestStyle/std-widgets.slint
+-rw-r--r--   0     1001      127      278 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/dependency_local.slint
+-rw-r--r--   0     1001      127      393 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/dependency_test_main.slint
+-rw-r--r--   0     1001      127      503 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/incpath/bug_2719_import.slint
+-rw-r--r--   0     1001      127      461 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/incpath/bug_3674_alias_from_invalid_import.slint
+-rw-r--r--   0     1001      127      262 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/incpath/dependency_from_incpath.slint
+-rw-r--r--   0     1001      127      205 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/incpath/local_helper_type.slint
+-rw-r--r--   0     1001      127      237 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/incpath/should_fail.slint
+-rw-r--r--   0     1001      127      320 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/incpath/should_fail2.slint
+-rw-r--r--   0     1001      127      280 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/incpath/should_fail3.slint
+-rw-r--r--   0     1001      127      491 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/incpath/should_fail4.slint
+-rw-r--r--   0     1001      127      208 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/library/dependency_from_library.slint
+-rw-r--r--   0     1001      127      243 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/library/lib.slint
+-rw-r--r--   0     1001      127      214 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/library/library_helper_type.slint
+-rw-r--r--   0     1001      127      324 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/recursive_import1.slint
+-rw-r--r--   0     1001      127      395 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/recursive_import2.slint
+-rw-r--r--   0     1001      127      450 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/tests/typeloader/some_rust_file.rs
+-rw-r--r--   0     1001      127    43496 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/typeloader.rs
+-rw-r--r--   0     1001      127    19774 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/typeregister.rs
+-rw-r--r--   0     1001      127    14083 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg
+-rw-r--r--   0     1001      127    14073 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg
+-rw-r--r--   0     1001      127     2358 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/combobox-base.slint
+-rw-r--r--   0     1001      127     3861 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/common.slint
+-rw-r--r--   0     1001      127     3266 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/lineedit-base.slint
+-rw-r--r--   0     1001      127     4288 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/listview.slint
+-rw-r--r--   0     1001      127     3968 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/slider-base.slint
+-rw-r--r--   0     1001      127     2427 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/spinbox-base.slint
+-rw-r--r--   0     1001      127     2510 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/spinner-base.slint
+-rw-r--r--   0     1001      127     1202 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/standardbutton.slint
+-rw-r--r--   0     1001      127     1080 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/common/tabwidget-base.slint
+-rw-r--r--   0     1001      127      268 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic/std-widgets.slint
+-rw-r--r--   0     1001      127      308 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/_arrow_down.svg
+-rw-r--r--   0     1001      127      284 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/_arrow_up.svg
+-rw-r--r--   0     1001      127      413 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/_check-mark.svg
+-rw-r--r--   0     1001      127      148 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/_pane_down.svg
+-rw-r--r--   0     1001      127     2760 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/button.slint
+-rw-r--r--   0     1001      127     2726 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/checkbox.slint
+-rw-r--r--   0     1001      127     3057 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/combobox.slint
+-rw-r--r--   0     1001      127     4437 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/components.slint
+-rw-r--r--   0     1001      127     1000 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/layouts.slint
+-rw-r--r--   0     1001      127     2886 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/lineedit.slint
+-rw-r--r--   0     1001      127      988 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5065 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/scrollview.slint
+-rw-r--r--   0     1001      127     2930 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/slider.slint
+-rw-r--r--   0     1001      127     3327 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/spinbox.slint
+-rw-r--r--   0     1001      127      733 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2126 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     3420 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/styling.slint
+-rw-r--r--   0     1001      127     2861 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/switch.slint
+-rw-r--r--   0     1001      127     9124 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/tableview.slint
+-rw-r--r--   0     1001      127     6075 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/tabwidget.slint
+-rw-r--r--   0     1001      127     4438 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-light/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cosmic-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino/std-widgets.slint
+-rw-r--r--   0     1001      127      513 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_arrow-down.svg
+-rw-r--r--   0     1001      127      507 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_arrow-up.svg
+-rw-r--r--   0     1001      127      780 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_check-mark.svg
+-rw-r--r--   0     1001      127      623 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_chevron-down.svg
+-rw-r--r--   0     1001      127      601 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_chevron-up.svg
+-rw-r--r--   0     1001      127      918 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_down.svg
+-rw-r--r--   0     1001      127      489 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_dropdown.svg
+-rw-r--r--   0     1001      127      849 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_left.svg
+-rw-r--r--   0     1001      127      815 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_right.svg
+-rw-r--r--   0     1001      127     1135 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_up.svg
+-rw-r--r--   0     1001      127     5181 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/button.slint
+-rw-r--r--   0     1001      127     4547 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/checkbox.slint
+-rw-r--r--   0     1001      127     5646 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/combobox.slint
+-rw-r--r--   0     1001      127     3145 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/components.slint
+-rw-r--r--   0     1001      127     1103 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/layouts.slint
+-rw-r--r--   0     1001      127     3180 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/lineedit.slint
+-rw-r--r--   0     1001      127     1404 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5563 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/scrollview.slint
+-rw-r--r--   0     1001      127     3097 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/slider.slint
+-rw-r--r--   0     1001      127     5483 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/spinbox.slint
+-rw-r--r--   0     1001      127      739 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2216 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     4541 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/styling.slint
+-rw-r--r--   0     1001      127     4097 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/switch.slint
+-rw-r--r--   0     1001      127     8959 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/tableview.slint
+-rw-r--r--   0     1001      127     5493 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/tabwidget.slint
+-rw-r--r--   0     1001      127     6640 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-light/color-scheme.slint
+-rw-r--r--   0     1001      127      332 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      215 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/cupertino-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent/std-widgets.slint
+-rw-r--r--   0     1001      127      513 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_arrow-down.svg
+-rw-r--r--   0     1001      127      507 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_arrow-up.svg
+-rw-r--r--   0     1001      127      780 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_check-mark.svg
+-rw-r--r--   0     1001      127      623 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_chevron-down.svg
+-rw-r--r--   0     1001      127      601 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_chevron-up.svg
+-rw-r--r--   0     1001      127      918 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_down.svg
+-rw-r--r--   0     1001      127      489 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_dropdown.svg
+-rw-r--r--   0     1001      127      849 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_left.svg
+-rw-r--r--   0     1001      127      815 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_right.svg
+-rw-r--r--   0     1001      127     1135 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/_up.svg
+-rw-r--r--   0     1001      127     4607 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/button.slint
+-rw-r--r--   0     1001      127     3883 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/checkbox.slint
+-rw-r--r--   0     1001      127     3773 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/combobox.slint
+-rw-r--r--   0     1001      127     3363 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/components.slint
+-rw-r--r--   0     1001      127      877 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/groupbox.slint
+-rw-r--r--   0     1001      127      632 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/layouts.slint
+-rw-r--r--   0     1001      127     3499 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/lineedit.slint
+-rw-r--r--   0     1001      127     1023 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/progressindicator.slint
+-rw-r--r--   0     1001      127     6590 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/scrollview.slint
+-rw-r--r--   0     1001      127     3734 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/slider.slint
+-rw-r--r--   0     1001      127     3992 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/spinbox.slint
+-rw-r--r--   0     1001      127      733 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/spinner.slint
+-rw-r--r--   0     1001      127     1524 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2126 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     6248 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/styling.slint
+-rw-r--r--   0     1001      127     4616 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/switch.slint
+-rw-r--r--   0     1001      127     9561 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/tableview.slint
+-rw-r--r--   0     1001      127     5493 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/tabwidget.slint
+-rw-r--r--   0     1001      127     4935 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-base/textedit.slint
+-rw-r--r--   0     1001      127      257 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-light/color-scheme.slint
+-rw-r--r--   0     1001      127      329 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      212 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/fluent-light/std-widgets.slint
+-rw-r--r--   0     1001      127      268 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material/color-scheme.slint
+-rw-r--r--   0     1001      127      347 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material/std-widgets.slint
+-rw-r--r--   0     1001      127      163 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/_arrow-downward.svg
+-rw-r--r--   0     1001      127      115 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/_arrow-drop-down.svg
+-rw-r--r--   0     1001      127      115 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/_arrow-drop-up.svg
+-rw-r--r--   0     1001      127      161 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/_arrow-upward.svg
+-rw-r--r--   0     1001      127      150 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/_check-mark.svg
+-rw-r--r--   0     1001      127      145 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/_expand-more.svg
+-rw-r--r--   0     1001      127     3288 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/button.slint
+-rw-r--r--   0     1001      127     5664 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/checkbox.slint
+-rw-r--r--   0     1001      127     3452 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/combobox.slint
+-rw-r--r--   0     1001      127     4712 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/components.slint
+-rw-r--r--   0     1001      127     1477 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/groupbox.slint
+-rw-r--r--   0     1001      127      633 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/layouts.slint
+-rw-r--r--   0     1001      127     2866 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/lineedit.slint
+-rw-r--r--   0     1001      127     1010 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/progressindicator.slint
+-rw-r--r--   0     1001      127     5014 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/scrollview.slint
+-rw-r--r--   0     1001      127     4146 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/slider.slint
+-rw-r--r--   0     1001      127     5090 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/spinbox.slint
+-rw-r--r--   0     1001      127      737 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/spinner.slint
+-rw-r--r--   0     1001      127     1373 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/std-widgets-base.slint
+-rw-r--r--   0     1001      127     2213 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     3651 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/styling.slint
+-rw-r--r--   0     1001      127     6174 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/switch.slint
+-rw-r--r--   0     1001      127     8186 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/tableview.slint
+-rw-r--r--   0     1001      127     4886 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-base/tabwidget.slint
+-rw-r--r--   0     1001      127      257 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-dark/color-scheme.slint
+-rw-r--r--   0     1001      127      331 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-dark/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-dark/std-widgets.slint
+-rw-r--r--   0     1001      127      258 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-light/color-scheme.slint
+-rw-r--r--   0     1001      127      331 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-light/std-widgets-impl.slint
+-rw-r--r--   0     1001      127      214 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/material-light/std-widgets.slint
+-rw-r--r--   0     1001      127     1736 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/button.slint
+-rw-r--r--   0     1001      127      350 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/checkbox.slint
+-rw-r--r--   0     1001      127     1707 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/combobox.slint
+-rw-r--r--   0     1001      127      582 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/groupbox.slint
+-rw-r--r--   0     1001      127     2384 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/internal-scrollview.slint
+-rw-r--r--   0     1001      127      613 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/layouts.slint
+-rw-r--r--   0     1001      127     2377 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/lineedit.slint
+-rw-r--r--   0     1001      127      307 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/progressindicator.slint
+-rw-r--r--   0     1001      127     1026 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/scrollview.slint
+-rw-r--r--   0     1001      127      447 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/slider.slint
+-rw-r--r--   0     1001      127      859 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/spinbox.slint
+-rw-r--r--   0     1001      127     1265 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/spinner.slint
+-rw-r--r--   0     1001      127      374 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/std-widgets-impl.slint
+-rw-r--r--   0     1001      127     1475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/std-widgets.slint
+-rw-r--r--   0     1001      127      346 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/switch.slint
+-rw-r--r--   0     1001      127     5310 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/tableview.slint
+-rw-r--r--   0     1001      127     1564 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/compiler/widgets/qt/tabwidget.slint
+-rw-r--r--   0     1001      127     3852 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127     2320 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/README.md
+-rw-r--r--   0     1001      127    22398 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/accesskit.rs
+-rw-r--r--   0     1001      127      646 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/build.rs
+-rw-r--r--   0     1001      127    30209 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/event_loop.rs
+-rw-r--r--   0     1001      127    16654 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/lib.rs
+-rw-r--r--   0     1001      127     8046 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/renderer/femtovg/glcontext.rs
+-rw-r--r--   0     1001      127     2131 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/renderer/femtovg.rs
+-rw-r--r--   0     1001      127     4558 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/renderer/skia.rs
+-rw-r--r--   0     1001      127     6824 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/renderer/sw.rs
+-rw-r--r--   0     1001      127    14717 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/wasm_input_helper.rs
+-rw-r--r--   0     1001      127    32303 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/backends/winit/winitwindowadapter.rs
+-rw-r--r--   0     1001      127     1919 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/README.md
+-rw-r--r--   0     1001      127    26501 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/fonts.rs
+-rw-r--r--   0     1001      127     9732 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/images.rs
+-rw-r--r--   0     1001      127    61993 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/itemrenderer.rs
+-rw-r--r--   0     1001      127    23205 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/renderers/femtovg/lib.rs
+-rw-r--r--   0     1001      127     6405 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127    68256 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/api.rs
+-rw-r--r--   0     1001      127    86327 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/dynamic_item_tree.rs
+-rw-r--r--   0     1001      127     7555 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/dynamic_type.rs
+-rw-r--r--   0     1001      127    75094 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/eval.rs
+-rw-r--r--   0     1001      127    12240 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/eval_layout.rs
+-rw-r--r--   0     1001      127    31460 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/ffi.rs
+-rw-r--r--   0     1001      127     9875 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/global_component.rs
+-rw-r--r--   0     1001      127     5912 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/highlight.rs
+-rw-r--r--   0     1001      127     3112 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/lib.rs
+-rw-r--r--   0     1001      127     1425 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/migration.rs
+-rw-r--r--   0     1001      127     1809 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/tests.rs
+-rw-r--r--   0     1001      127     2301 2024-05-13 09:35:19.000000 slint-1.6.0a8/internal/interpreter/value_model.rs
+-rw-r--r--   0     1001      127      738 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/macros/Cargo.toml
+-rw-r--r--   0     1001      127    34670 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/macros/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0     1001      127     3475 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md
+-rw-r--r--   0     1001      127    14063 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md
+-rw-r--r--   0     1001      127      507 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/macros/README.md
+-rw-r--r--   0     1001      127    19345 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/rs/macros/lib.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 slint-1.6.0a8/api/python/Cargo.toml
+-rw-r--r--   0     1001      127       11 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/.gitignore
+-rw-r--r--   0     1001      127     7730 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/README.md
+-rw-r--r--   0     1001      127     4367 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/brush.rs
+-rw-r--r--   0     1001      127     3303 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/errors.rs
+-rw-r--r--   0     1001      127     1399 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/image.rs
+-rw-r--r--   0     1001      127    10939 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/interpreter.rs
+-rw-r--r--   0     1001      127     1421 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/lib.rs
+-rw-r--r--   0     1001      127     6300 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/models.rs
+-rw-r--r--   0     1001      127      348 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/noxfile.py
+-rw-r--r--   0     1001      127     7729 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/slint/__init__.py
+-rw-r--r--   0     1001      127     1889 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/slint/models.py
+-rw-r--r--   0     1001      127     1164 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_brush.py
+-rw-r--r--   0     1001      127     1019 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_callback_decorators.py
+-rw-r--r--   0     1001      127     2369 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_compiler.py
+-rw-r--r--   0     1001      127     1095 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_gc.py
+-rw-r--r--   0     1001      127     6577 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_instance.py
+-rw-r--r--   0     1001      127     1597 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_load_file.py
+-rw-r--r--   0     1001      127      905 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_load_file.slint
+-rw-r--r--   0     1001      127      687 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_loader.py
+-rw-r--r--   0     1001      127     3589 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_models.py
+-rw-r--r--   0     1001      127      832 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/tests/test_timers.py
+-rw-r--r--   0     1001      127     2415 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/timer.rs
+-rw-r--r--   0     1001      127     4717 2024-05-13 09:35:19.000000 slint-1.6.0a8/api/python/value.rs
+-rw-r--r--   0     1001      127   209023 2024-05-13 09:35:19.000000 slint-1.6.0a8/Cargo.lock
+-rw-r--r--   0        0        0     4140 1970-01-01 00:00:00.000000 slint-1.6.0a8/Cargo.toml
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 slint-1.6.0a8/pyproject.toml
+-rw-r--r--   0     1001      127     7729 2024-05-13 09:35:19.000000 slint-1.6.0a8/slint/__init__.py
+-rw-r--r--   0     1001      127     1889 2024-05-13 09:35:19.000000 slint-1.6.0a8/slint/models.py
+-rw-r--r--   0        0        0     9277 1970-01-01 00:00:00.000000 slint-1.6.0a8/PKG-INFO
```

### Comparing `slint-1.6.0a7/api/rs/macros/Cargo.toml` & `slint-1.6.0a8/api/rs/macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/macros/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/backends/selector/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/macros/lib.rs` & `slint-1.6.0a8/api/rs/macros/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/Cargo.toml` & `slint-1.6.0a8/internal/backends/linuxkms/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 rust-version.workspace = true
 version.workspace = true
 
 [lib]
 path = "lib.rs"
 
 [features]
-renderer-skia = ["renderer-skia-vulkan", "renderer-skia-opengl"]
+renderer-skia = ["renderer-skia-opengl"]
 renderer-skia-vulkan = ["i-slint-renderer-skia/vulkan", "vulkano"]
 renderer-skia-opengl = ["i-slint-renderer-skia/opengl", "drm", "gbm", "gbm-sys", "glutin", "raw-window-handle"]
 renderer-femtovg = ["i-slint-renderer-femtovg", "drm", "gbm", "gbm-sys", "glutin", "raw-window-handle"]
 libseat = ["dep:libseat"]
 
 #default = ["renderer-skia", "renderer-femtovg"]
 default = []
```

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/core-macros/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/LICENSES/MIT.txt` & `slint-1.6.0a8/helper_crates/const-field-offset/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/calloop_backend/input.rs` & `slint-1.6.0a8/internal/backends/linuxkms/calloop_backend/input.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/calloop_backend.rs` & `slint-1.6.0a8/internal/backends/linuxkms/calloop_backend.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/display/gbmdisplay.rs` & `slint-1.6.0a8/internal/backends/linuxkms/display/gbmdisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/display/swdisplay.rs` & `slint-1.6.0a8/internal/backends/linuxkms/display/swdisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/display/vulkandisplay.rs` & `slint-1.6.0a8/internal/backends/linuxkms/display/vulkandisplay.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/display.rs` & `slint-1.6.0a8/internal/backends/linuxkms/display.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/drmoutput.rs` & `slint-1.6.0a8/internal/backends/linuxkms/drmoutput.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/fullscreenwindowadapter.rs` & `slint-1.6.0a8/internal/backends/linuxkms/fullscreenwindowadapter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/lib.rs` & `slint-1.6.0a8/internal/backends/linuxkms/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/noop_backend.rs` & `slint-1.6.0a8/internal/backends/linuxkms/noop_backend.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/renderer/femtovg.rs` & `slint-1.6.0a8/internal/backends/linuxkms/renderer/femtovg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/linuxkms/renderer/skia.rs` & `slint-1.6.0a8/internal/backends/linuxkms/renderer/skia.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/Cargo.toml` & `slint-1.6.0a8/internal/compiler/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/LICENSES/Apache-2.0.txt` & `slint-1.6.0a8/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/LICENSES/CC-BY-ND-4.0.txt` & `slint-1.6.0a8/internal/compiler/LICENSES/CC-BY-ND-4.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/LICENSES/MIT.txt` & `slint-1.6.0a8/helper_crates/vtable/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/README.md` & `slint-1.6.0a8/internal/compiler/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/build.rs` & `slint-1.6.0a8/internal/compiler/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 use std::fs::read_dir;
 use std::io::{BufWriter, Write};
 use std::path::{Path, PathBuf};
 
 fn main() -> std::io::Result<()> {
+    println!("cargo:rustc-check-cfg=cfg(slint_debug_property)");
+
     let mut library_dir = PathBuf::from(std::env::var_os("CARGO_MANIFEST_DIR").unwrap());
     library_dir.push("widgets");
 
     println!("cargo:rerun-if-changed={}", library_dir.display());
 
     let output_file_path = Path::new(&std::env::var_os("OUT_DIR").unwrap())
         .join(Path::new("included_library").with_extension("rs"));
```

### Comparing `slint-1.6.0a7/internal/compiler/builtin_macros.rs` & `slint-1.6.0a8/internal/compiler/builtin_macros.rs`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     diag: &mut BuildDiagnostics,
 ) -> Expression {
     match mac {
         BuiltinMacroFunction::Min => min_max_macro(n, MinMaxOp::Min, sub_expr.collect(), diag),
         BuiltinMacroFunction::Max => min_max_macro(n, MinMaxOp::Max, sub_expr.collect(), diag),
         BuiltinMacroFunction::Clamp => clamp_macro(n, sub_expr.collect(), diag),
         BuiltinMacroFunction::Mod => mod_macro(n, sub_expr.collect(), diag),
+        BuiltinMacroFunction::Abs => abs_macro(n, sub_expr.collect(), diag),
         BuiltinMacroFunction::Debug => debug_macro(n, sub_expr.collect(), diag),
         BuiltinMacroFunction::CubicBezier => {
             let mut has_error = None;
             let expected_argument_type_error =
                 "Arguments to cubic bezier curve must be number literal";
             // FIXME: this is not pretty to be handling there.
             // Maybe "cubic_bezier" should be a function that is lowered later
@@ -179,14 +180,55 @@
             }
             .into(),
             to: common_ty.clone(),
         }
     }
 }
 
+fn abs_macro(
+    node: Option<NodeOrToken>,
+    args: Vec<(Expression, Option<NodeOrToken>)>,
+    diag: &mut BuildDiagnostics,
+) -> Expression {
+    if args.len() != 1 {
+        diag.push_error("Needs 1 argument".into(), &node);
+        return Expression::Invalid;
+    }
+    let ty = args[0].0.ty();
+    let ty = if ty.default_unit().is_some() || matches!(ty, Type::UnitProduct(_)) {
+        ty
+    } else {
+        Type::Float32
+    };
+
+    let source_location = node.map(|n| n.to_source_location());
+    let function = Box::new(Expression::BuiltinFunctionReference(
+        BuiltinFunction::Abs,
+        source_location.clone(),
+    ));
+    if matches!(ty, Type::Float32) {
+        let arguments =
+            args.into_iter().map(|(e, n)| e.maybe_convert_to(ty.clone(), &n, diag)).collect();
+        Expression::FunctionCall { function, arguments, source_location }
+    } else {
+        Expression::Cast {
+            from: Expression::FunctionCall {
+                function,
+                arguments: args
+                    .into_iter()
+                    .map(|(a, _)| Expression::Cast { from: a.into(), to: Type::Float32 })
+                    .collect(),
+                source_location,
+            }
+            .into(),
+            to: ty,
+        }
+    }
+}
+
 fn rgb_macro(
     node: Option<NodeOrToken>,
     args: Vec<(Expression, Option<NodeOrToken>)>,
     diag: &mut BuildDiagnostics,
 ) -> Expression {
     if args.len() < 3 || args.len() > 4 {
         diag.push_error(
@@ -235,25 +277,16 @@
     if args.len() < 3 || args.len() > 4 {
         diag.push_error(
             format!("This function needs 3 or 4 arguments, but {} were provided", args.len()),
             &node,
         );
         return Expression::Invalid;
     }
-    let mut arguments: Vec<_> = args
-        .into_iter()
-        .enumerate()
-        .map(|(i, (expr, n))| {
-            if i < 3 {
-                expr.maybe_convert_to(Type::Float32, &n, diag)
-            } else {
-                expr.maybe_convert_to(Type::Float32, &n, diag)
-            }
-        })
-        .collect();
+    let mut arguments: Vec<_> =
+        args.into_iter().map(|(expr, n)| expr.maybe_convert_to(Type::Float32, &n, diag)).collect();
     if arguments.len() < 4 {
         arguments.push(Expression::NumberLiteral(1., Unit::None))
     }
     Expression::FunctionCall {
         function: Box::new(Expression::BuiltinFunctionReference(
             BuiltinFunction::Hsv,
             node.as_ref().map(|t| t.to_source_location()),
```

### Comparing `slint-1.6.0a7/internal/compiler/builtins.slint` & `slint-1.6.0a8/internal/compiler/builtins.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/diagnostics.rs` & `slint-1.6.0a8/internal/compiler/diagnostics.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/embedded_resources.rs` & `slint-1.6.0a8/internal/compiler/embedded_resources.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/expression_tree.rs` & `slint-1.6.0a8/internal/compiler/expression_tree.rs`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,16 @@
     Min,
     /// Transform `max(a, b, c, ..., z)` into  a series of conditional expression and comparisons
     Max,
     /// Transforms `clamp(v, min, max)` into a series of min/max calls
     Clamp,
     /// Add the right conversion operations so that the return type is the same as the argument type
     Mod,
+    /// Add the right conversion operations so that the return type is the same as the argument type
+    Abs,
     CubicBezier,
     /// The argument can be r,g,b,a or r,g,b and they can be percentages or integer.
     /// transform the argument so it is always rgb(r, g, b, a) with r, g, b between 0 and 255.
     Rgb,
     Hsv,
     /// transform `debug(a, b, c)` into debug `a + " " + b + " " + c`
     Debug,
@@ -1483,15 +1485,15 @@
     ///
     /// Also the animation is taken if the other don't have one, and the two ways binding
     /// are taken into account.
     ///
     /// Returns true if the other expression was taken
     pub fn merge_with(&mut self, other: &Self) -> bool {
         if self.animation.is_none() {
-            self.animation = other.animation.clone();
+            self.animation.clone_from(&other.animation);
         }
         let has_binding = self.has_binding();
         self.two_way_bindings.extend_from_slice(&other.two_way_bindings);
         if !has_binding {
             self.priority = other.priority;
             self.expression = other.expression.clone();
             true
```

### Comparing `slint-1.6.0a7/internal/compiler/fileaccess.rs` & `slint-1.6.0a8/internal/compiler/fileaccess.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/generator/cpp.rs` & `slint-1.6.0a8/internal/compiler/generator/cpp.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3127,30 +3127,31 @@
                 let window = access_window_field(ctx);
                 let focus_item = access_item_rc(pr, ctx);
                 format!("{}.set_focus_item({}, false);", window, focus_item)
             } else {
                 panic!("internal error: invalid args to ClearFocusItem {:?}", arguments)
             }
         }
-        /*  std::from_chars is unfortunately not yet implemented in gcc
+        /* std::from_chars is unfortunately not yet implemented in all stdlib compiler we support.
+         * And std::strtod depends on the locale. Use slint_string_to_float implemented in Rust
         BuiltinFunction::StringIsFloat => {
             "[](const auto &a){ double v; auto r = std::from_chars(std::begin(a), std::end(a), v); return r.ptr == std::end(a); }"
                 .into()
         }
         BuiltinFunction::StringToFloat => {
             "[](const auto &a){ double v; auto r = std::from_chars(std::begin(a), std::end(a), v); return r.ptr == std::end(a) ? v : 0; }"
                 .into()
         }*/
         BuiltinFunction::StringIsFloat => {
             ctx.generator_state.conditional_includes.cstdlib.set(true);
-            format!("[](const auto &a){{ auto e1 = std::end(a); auto e2 = const_cast<char*>(e1); std::strtod(std::begin(a), &e2); return e1 == e2; }}({})", a.next().unwrap())
+            format!("[](const auto &a){{ float res = 0; return slint::cbindgen_private::slint_string_to_float(&a, &res); }}({})", a.next().unwrap())
         }
         BuiltinFunction::StringToFloat => {
             ctx.generator_state.conditional_includes.cstdlib.set(true);
-            format!("[](const auto &a){{ auto e1 = std::end(a); auto e2 = const_cast<char*>(e1); auto r = std::strtod(std::begin(a), &e2); return e1 == e2 ? r : 0; }}({})", a.next().unwrap())
+            format!("[](const auto &a){{ float res = 0; slint::cbindgen_private::slint_string_to_float(&a, &res); return res; }}({})", a.next().unwrap())
         }
         BuiltinFunction::ColorRgbaStruct => {
             format!("{}.to_argb_uint()", a.next().unwrap())
         }
         BuiltinFunction::ColorHsvaStruct => {
             format!("{}.to_hsva()", a.next().unwrap())
         }
```

### Comparing `slint-1.6.0a7/internal/compiler/generator/rust.rs` & `slint-1.6.0a8/internal/compiler/generator/rust.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/generator.rs` & `slint-1.6.0a8/internal/compiler/generator.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/langtype.rs` & `slint-1.6.0a8/internal/compiler/langtype.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/layout.rs` & `slint-1.6.0a8/internal/compiler/layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/lexer.rs` & `slint-1.6.0a8/internal/compiler/lexer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/lib.rs` & `slint-1.6.0a8/internal/compiler/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/literals.rs` & `slint-1.6.0a8/internal/compiler/literals.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/llr/expression.rs` & `slint-1.6.0a8/internal/compiler/llr/expression.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/llr/item_tree.rs` & `slint-1.6.0a8/internal/compiler/llr/item_tree.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/llr/lower_expression.rs` & `slint-1.6.0a8/internal/compiler/llr/lower_expression.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/llr/lower_to_item_tree.rs` & `slint-1.6.0a8/internal/compiler/llr/lower_to_item_tree.rs`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
             // TODO: we also want to split by type (role/string/...)
             let enum_value =
                 crate::generator::to_pascal_case(key.strip_prefix("accessible-").unwrap());
             accessible_prop.push((*elem.item_index.get().unwrap(), enum_value, nr.clone()));
         }
 
         for (prop, expr) in &elem.change_callbacks {
-            change_callbacks.push((NamedReference::new(&element, prop), expr.borrow().clone()));
+            change_callbacks.push((NamedReference::new(element, prop), expr.borrow().clone()));
         }
 
         Some(element.clone())
     });
     let ctx = ExpressionContext { mapping: &mapping, state, parent: parent_context, component };
     crate::generator::handle_property_bindings_init(component, |e, p, binding| {
         let nr = NamedReference::new(e, p);
```

### Comparing `slint-1.6.0a7/internal/compiler/llr/optim_passes/count_property_use.rs` & `slint-1.6.0a8/internal/compiler/llr/optim_passes/count_property_use.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/llr/optim_passes/inline_expressions.rs` & `slint-1.6.0a8/internal/compiler/llr/optim_passes/inline_expressions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/llr/pretty_print.rs` & `slint-1.6.0a8/internal/compiler/llr/pretty_print.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/llr.rs` & `slint-1.6.0a8/internal/compiler/llr.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/load_builtins.rs` & `slint-1.6.0a8/internal/compiler/load_builtins.rs`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
                 let a = identifier_text(&s.Element().QualifiedName().unwrap()).unwrap();
                 let t = natives[&a].clone();
                 (a, ElementType::Builtin(t))
             })
             .collect();
         if let Some(builtin_name) = exports.get(&id) {
             if !matches!(&base, Base::Global) {
-                builtin.name = builtin_name.clone();
+                builtin.name.clone_from(&builtin_name);
                 register.add_builtin(Rc::new(builtin));
             } else {
                 let glob = Rc::new(Component {
                     id: builtin_name.clone(),
                     root_element: Rc::new(RefCell::new(Element {
                         base_type: ElementType::Builtin(Rc::new(builtin)),
                         ..Default::default()
```

### Comparing `slint-1.6.0a7/internal/compiler/lookup.rs` & `slint-1.6.0a8/internal/compiler/lookup.rs`

 * *Files 0% similar despite different names*

```diff
@@ -492,20 +492,20 @@
                     .borrow()
                     .builtin_type()
                     .map_or(false, |x| x.is_internal && x.name == name)
                     && !ctx.type_register.expose_internal_types
                 {
                     None
                 } else {
-                    return Some(LookupResult::Expression {
+                    Some(LookupResult::Expression {
                         expression: Expression::ElementReference(Rc::downgrade(&c.root_element)),
                         deprecated: (name == "StyleMetrics"
                             && !ctx.type_register.expose_internal_types)
                             .then(|| "Palette".to_string()),
-                    });
+                    })
                 }
             }
             _ => None,
         }
     }
 }
 
@@ -782,15 +782,15 @@
         let sl = || t.as_ref().map(|t| t.to_source_location());
         let mut f = |n, e: Expression| f(n, e.into());
         None.or_else(|| f("mod", BuiltinMacroReference(BuiltinMacroFunction::Mod, t.clone())))
             .or_else(|| f("round", BuiltinFunctionReference(BuiltinFunction::Round, sl())))
             .or_else(|| f("ceil", BuiltinFunctionReference(BuiltinFunction::Ceil, sl())))
             .or_else(|| f("floor", BuiltinFunctionReference(BuiltinFunction::Floor, sl())))
             .or_else(|| f("clamp", BuiltinMacroReference(BuiltinMacroFunction::Clamp, t.clone())))
-            .or_else(|| f("abs", BuiltinFunctionReference(BuiltinFunction::Abs, sl())))
+            .or_else(|| f("abs", BuiltinMacroReference(BuiltinMacroFunction::Abs, t.clone())))
             .or_else(|| f("sqrt", BuiltinFunctionReference(BuiltinFunction::Sqrt, sl())))
             .or_else(|| f("max", BuiltinMacroReference(BuiltinMacroFunction::Max, t.clone())))
             .or_else(|| f("min", BuiltinMacroReference(BuiltinMacroFunction::Min, t.clone())))
             .or_else(|| f("sin", BuiltinFunctionReference(BuiltinFunction::Sin, sl())))
             .or_else(|| f("cos", BuiltinFunctionReference(BuiltinFunction::Cos, sl())))
             .or_else(|| f("tan", BuiltinFunctionReference(BuiltinFunction::Tan, sl())))
             .or_else(|| f("asin", BuiltinFunctionReference(BuiltinFunction::ASin, sl())))
```

### Comparing `slint-1.6.0a7/internal/compiler/namedreference.rs` & `slint-1.6.0a8/internal/compiler/namedreference.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/object_tree.rs` & `slint-1.6.0a8/internal/compiler/object_tree.rs`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,17 @@
     pub init_code: RefCell<InitCode>,
 
     /// The list of used extra types used (recursively) by this root component.
     /// (This only make sense on the root component)
     pub used_types: RefCell<UsedSubTypes>,
     pub popup_windows: RefCell<Vec<PopupWindow>>,
 
+    /// This component actually inherits PopupWindow (although that has been changed to a Window by the lower_popups pass)
+    pub inherits_popup_window: Cell<bool>,
+
     /// The names under which this component should be accessible
     /// if it is a global singleton and exported.
     pub exported_global_names: RefCell<Vec<ExportedName>>,
 
     /// The list of properties (name and type) declared as private in the component.
     /// This is used to issue better error in the generated code if the property is used.
     pub private_properties: RefCell<Vec<(String, Type)>>,
@@ -1042,30 +1045,14 @@
             let name =
                 unwrap_or_continue!(parser::identifier_text(&sig_decl.DeclaredIdentifier()); diag);
 
             let pure = Some(
                 sig_decl.child_token(SyntaxKind::Identifier).map_or(false, |t| t.text() == "pure"),
             );
 
-            if let Some(csn) = sig_decl.TwoWayBinding() {
-                r.bindings
-                    .insert(name.clone(), BindingExpression::new_uncompiled(csn.into()).into());
-                r.property_declarations.insert(
-                    name,
-                    PropertyDeclaration {
-                        property_type: Type::InferredCallback,
-                        node: Some(sig_decl.into()),
-                        visibility: PropertyVisibility::InOut,
-                        pure,
-                        ..Default::default()
-                    },
-                );
-                continue;
-            }
-
             let PropertyLookupResult {
                 resolved_name: existing_name,
                 property_type: maybe_existing_prop_type,
                 ..
             } = r.lookup_property(&name);
             if !matches!(maybe_existing_prop_type, Type::Invalid) {
                 if matches!(maybe_existing_prop_type, Type::Callback { .. }) {
@@ -1088,14 +1075,30 @@
                         ),
                         &sig_decl.DeclaredIdentifier(),
                     );
                 }
                 continue;
             }
 
+            if let Some(csn) = sig_decl.TwoWayBinding() {
+                r.bindings
+                    .insert(name.clone(), BindingExpression::new_uncompiled(csn.into()).into());
+                r.property_declarations.insert(
+                    name,
+                    PropertyDeclaration {
+                        property_type: Type::InferredCallback,
+                        node: Some(sig_decl.into()),
+                        visibility: PropertyVisibility::InOut,
+                        pure,
+                        ..Default::default()
+                    },
+                );
+                continue;
+            }
+
             let args = sig_decl.Type().map(|node_ty| type_from_node(node_ty, diag, tr)).collect();
             let return_type = sig_decl
                 .ReturnType()
                 .map(|ret_ty| Box::new(type_from_node(ret_ty.Type(), diag, tr)));
             r.property_declarations.insert(
                 name,
                 PropertyDeclaration {
@@ -1408,15 +1411,15 @@
                                 (ne, Expression::Uncompiled(s.BindingExpression().into()), s)
                             })
                     })
                     .collect(),
             };
             for trs in state.Transition() {
                 let mut t = Transition::from_node(trs, &r, tr, diag);
-                t.state_id = s.id.clone();
+                t.state_id.clone_from(&s.id);
                 r.borrow_mut().transitions.push(t);
             }
             r.borrow_mut().states.push(s);
         }
 
         for ts in node.Transitions() {
             if !is_legacy_syntax {
@@ -2617,12 +2620,12 @@
     // (should be removed by const propagation in the llr)
     injected_parent_mut.property_declarations.insert(
         "dummy".into(),
         PropertyDeclaration { property_type: Type::LogicalLength, ..Default::default() },
     );
     let mut old_elem_mut = old_elem.borrow_mut();
     injected_parent_mut.default_fill_parent = std::mem::take(&mut old_elem_mut.default_fill_parent);
-    injected_parent_mut.geometry_props = old_elem_mut.geometry_props.clone();
+    injected_parent_mut.geometry_props.clone_from(&old_elem_mut.geometry_props);
     drop(injected_parent_mut);
     old_elem_mut.geometry_props.as_mut().unwrap().x = NamedReference::new(injected_parent, "dummy");
     old_elem_mut.geometry_props.as_mut().unwrap().y = NamedReference::new(injected_parent, "dummy");
 }
```

### Comparing `slint-1.6.0a7/internal/compiler/parser/document.rs` & `slint-1.6.0a8/internal/compiler/parser/document.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/parser/element.rs` & `slint-1.6.0a8/internal/compiler/parser/element.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/parser/expressions.rs` & `slint-1.6.0a8/internal/compiler/parser/expressions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/parser/statements.rs` & `slint-1.6.0a8/internal/compiler/parser/statements.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/parser/type.rs` & `slint-1.6.0a8/internal/compiler/parser/type.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/parser.rs` & `slint-1.6.0a8/internal/compiler/parser.rs`

 * *Files 0% similar despite different names*

```diff
@@ -553,15 +553,15 @@
         /// consume everything until reaching a token of this kind
         fn until(&mut self, kind: SyntaxKind) {
             let mut parens = 0;
             let mut braces = 0;
             let mut brackets = 0;
             loop {
                 match self.nth(0).kind() {
-                    k @ _ if k == kind && parens == 0 && braces == 0 && brackets == 0 => break,
+                    k if k == kind && parens == 0 && braces == 0 && brackets == 0 => break,
                     SyntaxKind::Eof => break,
                     SyntaxKind::LParent => parens += 1,
                     SyntaxKind::LBrace => braces += 1,
                     SyntaxKind::LBracket => brackets += 1,
                     SyntaxKind::RParent if parens == 0 => break,
                     SyntaxKind::RParent => parens -= 1,
                     SyntaxKind::RBrace if braces == 0 => break,
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/apply_default_properties_from_style.rs` & `slint-1.6.0a8/internal/compiler/passes/apply_default_properties_from_style.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/binding_analysis.rs` & `slint-1.6.0a8/internal/compiler/passes/binding_analysis.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/border_radius.rs` & `slint-1.6.0a8/internal/compiler/passes/border_radius.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/check_expressions.rs` & `slint-1.6.0a8/internal/compiler/passes/check_expressions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/check_public_api.rs` & `slint-1.6.0a8/internal/compiler/passes/check_public_api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/check_rotation.rs` & `slint-1.6.0a8/internal/compiler/passes/check_rotation.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/clip.rs` & `slint-1.6.0a8/internal/compiler/passes/clip.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/collect_custom_fonts.rs` & `slint-1.6.0a8/internal/compiler/passes/collect_custom_fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/collect_globals.rs` & `slint-1.6.0a8/internal/compiler/passes/collect_globals.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/collect_init_code.rs` & `slint-1.6.0a8/internal/compiler/passes/collect_init_code.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/collect_structs_and_enums.rs` & `slint-1.6.0a8/internal/compiler/passes/collect_structs_and_enums.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/collect_subcomponents.rs` & `slint-1.6.0a8/internal/compiler/passes/collect_subcomponents.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/compile_paths.rs` & `slint-1.6.0a8/internal/compiler/passes/compile_paths.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/const_propagation.rs` & `slint-1.6.0a8/internal/compiler/passes/const_propagation.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/deduplicate_property_read.rs` & `slint-1.6.0a8/internal/compiler/passes/deduplicate_property_read.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/default_geometry.rs` & `slint-1.6.0a8/internal/compiler/passes/default_geometry.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/embed_glyphs.rs` & `slint-1.6.0a8/internal/compiler/passes/embed_glyphs.rs`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
     #[cfg(not(any(
         target_family = "windows",
         target_os = "macos",
         target_os = "ios",
         target_arch = "wasm32"
     )))]
     {
-        fallback_families = fontdb.fontconfig_fallback_families.clone();
+        fallback_families.clone_from(&fontdb.fontconfig_fallback_families);
     }
 
     let fallback_fonts = fallback_families
         .iter()
         .filter_map(|fallback_family| {
             fontdb
                 .query(&fontdb::Query {
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/embed_images.rs` & `slint-1.6.0a8/internal/compiler/passes/embed_images.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/ensure_window.rs` & `slint-1.6.0a8/internal/compiler/passes/ensure_window.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/flickable.rs` & `slint-1.6.0a8/internal/compiler/passes/flickable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/focus_handling.rs` & `slint-1.6.0a8/internal/compiler/passes/focus_handling.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/generate_item_indices.rs` & `slint-1.6.0a8/internal/compiler/passes/generate_item_indices.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/infer_aliases_types.rs` & `slint-1.6.0a8/internal/compiler/passes/infer_aliases_types.rs`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     let mut ty = Type::Invalid;
     if let Some(nr) = &nr {
         let element = nr.element();
         let same_element = Rc::ptr_eq(&element, elem);
         if same_element && nr.name() == prop {
             diag.push_error(
-                format!("Cannot alias to itself"),
+                "Cannot alias to itself".to_string(),
                 &elem.borrow().property_declarations[prop].type_node(),
             );
             return;
         }
         ty = nr.ty();
         if matches!(ty, Type::InferredCallback | Type::InferredProperty) {
             if same_element {
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/inlining.rs` & `slint-1.6.0a8/internal/compiler/passes/inlining.rs`

 * *Files 0% similar despite different names*

```diff
@@ -327,14 +327,15 @@
         child_insertion_point: component_to_duplicate.child_insertion_point.clone(),
         init_code: component_to_duplicate.init_code.clone(),
         used_types: Default::default(),
         popup_windows: Default::default(),
         exported_global_names: component_to_duplicate.exported_global_names.clone(),
         is_root_component: Default::default(),
         private_properties: Default::default(),
+        inherits_popup_window: core::cell::Cell::new(false),
     };
 
     let new_component = Rc::new(new_component);
     let weak = Rc::downgrade(&new_component);
     recurse_elem(&new_component.root_element, &(), &mut |e, _| {
         e.borrow_mut().enclosing_component = weak.clone()
     });
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_absolute_coordinates.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_absolute_coordinates.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_accessibility.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_accessibility.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_component_container.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_component_container.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_layout.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_popups.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_popups.rs`

 * *Files 14% similar despite different names*

```diff
@@ -18,41 +18,53 @@
 ) {
     let window_type = type_register.lookup_builtin_element("Window").unwrap();
 
     recurse_elem_including_sub_components_no_borrow(
         component,
         &None,
         &mut |elem, parent_element: &Option<ElementRc>| {
-            let is_popup = matches!(&elem.borrow().base_type, ElementType::Builtin(base_type) if base_type.name == "PopupWindow");
+            let is_popup = match &elem.borrow().base_type {
+                ElementType::Builtin(base_type) => base_type.name == "PopupWindow",
+                ElementType::Component(base_type) => base_type.inherits_popup_window.get(),
+                _ => false,
+            };
+
             if is_popup {
                 lower_popup_window(elem, parent_element.as_ref(), &window_type, diag);
             }
             Some(elem.clone())
         },
     )
 }
 
 fn lower_popup_window(
     popup_window_element: &ElementRc,
     parent_element: Option<&ElementRc>,
     window_type: &ElementType,
     diag: &mut BuildDiagnostics,
 ) {
+    let parent_component = popup_window_element.borrow().enclosing_component.upgrade().unwrap();
     let parent_element = match parent_element {
         None => {
-            diag.push_error(
-                "PopupWindow cannot be the top level".into(),
-                &*popup_window_element.borrow(),
-            );
+            if parent_component.is_root_component.get() {
+                diag.push_error(
+                    "PopupWindow cannot be the top level".into(),
+                    &*popup_window_element.borrow(),
+                );
+                return;
+            }
+            if matches!(popup_window_element.borrow().base_type, ElementType::Builtin(_)) {
+                popup_window_element.borrow_mut().base_type = window_type.clone();
+            }
+            parent_component.inherits_popup_window.set(true);
             return;
         }
         Some(parent_element) => parent_element,
     };
 
-    let parent_component = popup_window_element.borrow().enclosing_component.upgrade().unwrap();
     if Rc::ptr_eq(&parent_component.root_element, popup_window_element) {
         diag.push_error(
             "PopupWindow cannot be directly repeated or conditional".into(),
             &*popup_window_element.borrow(),
         );
         return;
     }
@@ -63,33 +75,50 @@
     debug_assert_eq!(
         parent_element.borrow().children.len() + 1,
         old_size,
         "Exactly one child must be removed (the popup itself)"
     );
     parent_element.borrow_mut().has_popup_child = true;
 
-    popup_window_element.borrow_mut().base_type = window_type.clone();
+    if matches!(popup_window_element.borrow().base_type, ElementType::Builtin(_)) {
+        popup_window_element.borrow_mut().base_type = window_type.clone();
+    }
+
+    const CLOSE_ON_CLICK: &str = "close-on-click";
+    let close_on_click = popup_window_element.borrow_mut().bindings.remove(CLOSE_ON_CLICK);
+    let close_on_click = close_on_click
+        .map(|b| {
+            let b = b.into_inner();
+            (b.expression, b.span)
+        })
+        .or_else(|| {
+            let mut base = popup_window_element.borrow().base_type.clone();
+            while let ElementType::Component(b) = base {
+                base = b.root_element.borrow().base_type.clone();
+                if let Some(binding) = b.root_element.borrow().bindings.get(CLOSE_ON_CLICK) {
+                    let b = binding.borrow();
+                    return Some((b.expression.clone(), b.span.clone()));
+                }
+            }
+            None
+        });
 
-    let close_on_click =
-        match popup_window_element.borrow_mut().bindings.remove("close-on-click").map_or_else(
-            || Ok(true),
-            |binding| match binding.borrow().expression {
-                Expression::BoolLiteral(value) => Ok(value),
-                _ => Err(binding.borrow().span.clone()),
-            },
-        ) {
-            Ok(coc) => coc,
-            Err(location) => {
+    let close_on_click = match close_on_click {
+        Some((expr, location)) => match expr {
+            Expression::BoolLiteral(value) => value,
+            _ => {
                 diag.push_error(
                     "The close-on-click property only supports constants at the moment".into(),
                     &location,
                 );
                 return;
             }
-        };
+        },
+        None => true,
+    };
 
     let popup_comp = Rc::new(Component {
         root_element: popup_window_element.clone(),
         parent_element: Rc::downgrade(parent_element),
         ..Component::default()
     });
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_property_to_element.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_property_to_element.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_shadows.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_shadows.rs`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,14 @@
                     Some(element) => element,
                     None => {
                         elem.borrow_mut().children.push(child);
                         continue;
                     }
                 };
 
-                shadow_elem.geometry_props = child.borrow().geometry_props.clone();
+                shadow_elem.geometry_props.clone_from(&child.borrow().geometry_props);
                 elem.borrow_mut().children.push(ElementRc::new(shadow_elem.into()));
             }
             elem.borrow_mut().children.push(child);
         }
     });
 }
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_states.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_states.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_tabwidget.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_tabwidget.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/lower_text_input_interface.rs` & `slint-1.6.0a8/internal/compiler/passes/lower_text_input_interface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/materialize_fake_properties.rs` & `slint-1.6.0a8/internal/compiler/passes/materialize_fake_properties.rs`

 * *Files 4% similar despite different names*

```diff
@@ -99,14 +99,17 @@
         ElementType::Global | ElementType::Error => false,
     };
 
     if !has_declared_property {
         let ty = crate::typeregister::reserved_property(prop).property_type;
         if ty != Type::Invalid {
             return Some(ty);
+        } else if prop == "close-on-click" {
+            // PopupWindow::close-on-click
+            return Some(Type::Bool);
         }
     }
     None
 }
 
 /// Returns true if the property is declared in this element or parent
 /// (as opposed to being implicitly declared)
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/move_declarations.rs` & `slint-1.6.0a8/internal/compiler/passes/move_declarations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/optimize_useless_rectangles.rs` & `slint-1.6.0a8/internal/compiler/passes/optimize_useless_rectangles.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/purity_check.rs` & `slint-1.6.0a8/internal/compiler/passes/purity_check.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/remove_aliases.rs` & `slint-1.6.0a8/internal/compiler/passes/remove_aliases.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/remove_return.rs` & `slint-1.6.0a8/internal/compiler/passes/remove_return.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/remove_unused_properties.rs` & `slint-1.6.0a8/internal/compiler/passes/remove_unused_properties.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/repeater_component.rs` & `slint-1.6.0a8/internal/compiler/passes/repeater_component.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/resolve_native_classes.rs` & `slint-1.6.0a8/internal/compiler/passes/resolve_native_classes.rs`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     properties_used: impl Iterator<Item = &'a String>,
 ) -> Rc<NativeClass> {
     let mut minimal_class = class.clone();
     while let Some(class) = minimal_class.parent.clone() {
         minimal_class = class;
     }
     let (_min_distance, minimal_class) = properties_used.fold(
-        (std::usize::MAX, minimal_class),
+        (usize::MAX, minimal_class),
         |(current_distance, current_class), prop_name| {
             let (prop_distance, prop_class) = lookup_property_distance(class.clone(), prop_name);
 
             if prop_distance < current_distance {
                 (prop_distance, prop_class)
             } else {
                 (current_distance, current_class)
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/resolving.rs` & `slint-1.6.0a8/internal/compiler/passes/resolving.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/unique_id.rs` & `slint-1.6.0a8/internal/compiler/passes/unique_id.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 /// Give globals unique name
 fn rename_globals(component: &Rc<Component>, mut count: u32) {
     for g in &component.used_types.borrow().globals {
         count += 1;
         let mut root = g.root_element.borrow_mut();
         if matches!(&root.base_type, ElementType::Builtin(_)) {
             // builtin global keeps its name
-            root.id = g.id.clone();
+            root.id.clone_from(&g.id);
         } else if let Some(s) = g.exported_global_names.borrow().first() {
             root.id = s.to_string();
         } else {
             root.id = format!("{}-{}", g.id, count);
         }
     }
 }
```

### Comparing `slint-1.6.0a7/internal/compiler/passes/visible.rs` & `slint-1.6.0a8/internal/compiler/passes/visible.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes/z_order.rs` & `slint-1.6.0a8/internal/compiler/passes/z_order.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/passes.rs` & `slint-1.6.0a8/internal/compiler/passes.rs`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             .import_component("std-widgets.slint", "StyleMetrics", &mut build_diags_to_ignore)
             .await
             .unwrap_or_else(|| panic!("can't load style metrics"))
     };
 
     let global_type_registry = type_loader.global_type_registry.clone();
     let root_component = &doc.root_component;
+    root_component.is_root_component.set(true);
     run_import_passes(doc, type_loader, diag);
     check_public_api::check_public_api(doc, diag);
 
     collect_subcomponents::collect_subcomponents(root_component);
     for component in (root_component.used_types.borrow().sub_components.iter())
         .chain(std::iter::once(root_component))
     {
@@ -267,16 +268,14 @@
                 root_component,
                 std::iter::once(doc).chain(type_loader.all_documents()),
                 type_loader.compiler_config.embed_resources
                     == crate::EmbedResourcesKind::EmbedAllResources,
             );
         }
     }
-
-    root_component.is_root_component.set(true);
 }
 
 /// Run the passes on imported documents
 pub fn run_import_passes(
     doc: &crate::object_tree::Document,
     type_loader: &crate::typeloader::TypeLoader,
     diag: &mut crate::diagnostics::BuildDiagnostics,
```

### Comparing `slint-1.6.0a7/internal/compiler/pathutils.rs` & `slint-1.6.0a8/internal/compiler/pathutils.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/consistent_styles.rs` & `slint-1.6.0a8/internal/compiler/tests/consistent_styles.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/accessibility/accessible_properties.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/accessibility/accessible_properties.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop1.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop1.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_function.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_function.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_issue_772.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_layout.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_layout2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_layout3.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_layout4.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/analysis/binding_loop_self.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/analysis/binding_loop_self.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/animate.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/animate.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/assign.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/assign.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/box_shadow.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/box_shadow.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/children_placeholder.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/children_placeholder.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/clip.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/clip.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/dialog.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/dialog.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/dialog2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/dialog2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/duplicated_id.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/duplicated_id.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/easing.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/easing.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/enums.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/enums.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/item_as_property.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/item_as_property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/layout2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/layout2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/linear-gradient.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/linear-gradient.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/opacity.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/opacity.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/parse_error.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/parse_error.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/path.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/path.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/path_commands.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/path_commands.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/path_for.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/path_for.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/percent.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/percent.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/popup.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/popup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/property_declaration.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/property_declaration.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/radial-gradient.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/radial-gradient.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/return.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/return.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/rotation.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/rotation.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/self_assign.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/self_assign.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/signal.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/signal.slint`

 * *Files 9% similar despite different names*

```diff
@@ -48,8 +48,11 @@
 
     property <bool> pressed;
     callback pressed;
 //           ^error{Cannot declare callback 'pressed' when a property with the same name exists}
 
     callback init;
 //           ^error{Cannot override callback 'init'}
+
+    callback width;
+//           ^error{Cannot declare callback 'width' when a property with the same name exists}
 }
```

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/states_transitions.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/states_transitions2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_transitions3.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/states_transitions3.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/states_two_way.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/states_two_way.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/sub_elements.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/sub_elements.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/tr.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/tr.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/tr2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/tr2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/type_declaration.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/type_declaration.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/basic/unknown_item.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/basic/unknown_item.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/callbacks/property-changes.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/callbacks/property-changes.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/elements/component_container.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/elements/component_container.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/elements/listview.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/elements/listview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/elements/popup.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/elements/popup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/elements/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/elements/tabwidget2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/elements/tabwidget2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/exports/reexport_duplicate.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/exports/reexport_duplicate.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/arithmetic_op.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/arithmetic_op.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/clamp.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/clamp.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/comparison_operator.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/comparison_operator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/condition_operator.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/condition_operator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/image-url.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/image-url.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/image-url2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/image-url2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/minmax.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/minmax.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/percent2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/percent2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/expressions/unary_op.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/expressions/unary_op.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_not_called.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/focus/focus_not_called.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/focus/focus_wrong_args.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/focus/focus_wrong_args.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/focus/initial_focus_non_input.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/functions/function_double_qualified.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/functions/function_double_qualified.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/functions/functions.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions_call.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/functions/functions_call.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/functions/functions_purity.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/functions/functions_purity.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/imports/bug_2719.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/imports/bug_2719.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/imports/bug_3674_alias-from-broken-import.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/imports/import_errors.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/imports/import_errors.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/layout/if_in_grid.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/layout/if_in_grid.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/layout/min_max_conflict.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/layout/min_max_conflict.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/layout/spacing.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/layout/spacing.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/array_index.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/array_index.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_alias.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_alias2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/callback_alias3.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/callback_alias3.slint`

 * *Files 22% similar despite different names*

```diff
@@ -26,9 +26,12 @@
     Sub {
         compute_alias(a, b, c) => {
             debug(b); // FIXME: one should actually check that the connection has the right amount of arguments
 //                ^error{Unknown unqualified identifier 'b'}
             return "hello";
 //          ^error{Cannot convert string to int}
         }
+
+        callback x <=> compute_alias;
+//               ^error{Cannot declare callback 'x' when a property with the same name exists}
     }
 }
```

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/color.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/color.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/conversion.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/conversion.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/dashes.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/dashes.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/deprecated_property.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/deprecated_property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/enum.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/enum.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/for_lookup.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/for_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/global.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/global.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/if.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/if.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/issue_1461.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/issue_1461.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/property.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/property.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/recover_id_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/signal_arg.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/signal_arg.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/two_way_binding.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/lookup/two_way_binding_infer.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/deprecated_syntax.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/input_output.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/input_output.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/input_output2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/input_output2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/new_component.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/new_component.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/new_lookup.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/new_lookup.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/new_syntax/two_way_input_output.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/property2.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/property2.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/state1.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/state1.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax/parse_error/struct.slint` & `slint-1.6.0a8/internal/compiler/tests/syntax/parse_error/struct.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/tests/syntax_tests.rs` & `slint-1.6.0a8/internal/compiler/tests/syntax_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/typeloader.rs` & `slint-1.6.0a8/internal/compiler/typeloader.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/typeregister.rs` & `slint-1.6.0a8/internal/compiler/typeregister.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg` & `slint-1.6.0a8/internal/compiler/widgets/common/MadeWithSlint-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg` & `slint-1.6.0a8/internal/compiler/widgets/common/MadeWithSlint-logo-light.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/combobox-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/combobox-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/common.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/common.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/lineedit-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/lineedit-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/listview.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/listview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/slider-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/slider-base.slint`

 * *Files 1% similar despite different names*

```diff
@@ -28,24 +28,23 @@
 
     touch-area := TouchArea {
         property <float> pressed-value;
 
         width: 100%;
         height: 100%;
 
-        clicked => {
-            released(root.value);
-        }
-
         pointer-event(event) => {
             if (event.button != PointerEventButton.left) {
                 return;
             }
 
             if (event.kind == PointerEventKind.up) {
+                if (root.handle-pressed) {
+                    root.released(root.value);
+                }
                 root.handle-pressed = false;
                 return;
             }
 
 
             if (!root.handle-has-hover) {
                 root.set-value((!root.vertical ? root.size-to-value(touch-area.mouse-x, root.width) :
```

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/spinbox-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/spinbox-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/spinner-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/spinner-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/standardbutton.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/standardbutton.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/common/tabwidget-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/common/tabwidget-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/button.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/checkbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/combobox.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/components.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/groupbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/layouts.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/lineedit.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/progressindicator.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/scrollview.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/slider.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/spinbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/spinner.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/std-widgets-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/styling.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/switch.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/tableview.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/tabwidget.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cosmic-base/textedit.slint` & `slint-1.6.0a8/internal/compiler/widgets/cosmic-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_arrow-down.svg` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_arrow-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_check-mark.svg` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_check-mark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_chevron-down.svg` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_chevron-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_chevron-up.svg` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_chevron-up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_down.svg` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_left.svg` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_left.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_right.svg` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_right.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/_up.svg` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/_up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/button.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/checkbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/combobox.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/components.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/groupbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/layouts.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/lineedit.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/progressindicator.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/scrollview.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/slider.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/spinbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/spinner.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/std-widgets-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/styling.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/switch.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/tableview.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/tabwidget.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/cupertino-base/textedit.slint` & `slint-1.6.0a8/internal/compiler/widgets/cupertino-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_arrow-down.svg` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/_arrow-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_check-mark.svg` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/_check-mark.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_chevron-down.svg` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/_chevron-down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_chevron-up.svg` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/_chevron-up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_down.svg` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/_down.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_left.svg` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/_left.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_right.svg` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/_right.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/_up.svg` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/_up.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/button.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/checkbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/combobox.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/components.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/groupbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/layouts.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/lineedit.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/progressindicator.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/scrollview.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/slider.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/spinbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/spinner.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/std-widgets-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/std-widgets-impl.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/styling.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/switch.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/tableview.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/tabwidget.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/fluent-base/textedit.slint` & `slint-1.6.0a8/internal/compiler/widgets/fluent-base/textedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/button.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/checkbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/checkbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/combobox.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/components.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/components.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/groupbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/layouts.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/lineedit.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/progressindicator.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/progressindicator.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/scrollview.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/slider.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/slider.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/spinbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/spinner.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/std-widgets-base.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/std-widgets-base.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/std-widgets-impl.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/std-widgets-impl.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/styling.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/styling.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/switch.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/switch.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/tableview.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/material-base/tabwidget.slint` & `slint-1.6.0a8/internal/compiler/widgets/material-base/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/button.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/button.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/combobox.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/combobox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/groupbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/groupbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/internal-scrollview.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/internal-scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/layouts.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/layouts.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/lineedit.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/lineedit.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/scrollview.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/scrollview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/spinbox.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/spinbox.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/spinner.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/spinner.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/std-widgets.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/std-widgets.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/tableview.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/tableview.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/widgets/qt/tabwidget.slint` & `slint-1.6.0a8/internal/compiler/widgets/qt/tabwidget.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/Cargo.toml` & `slint-1.6.0a8/internal/common/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/renderers/skia/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt` & `slint-1.6.0a8/internal/common/LICENSES/LicenseRef-DejaVu-Font.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/README.md` & `slint-1.6.0a8/internal/common/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/builtin_structs.rs` & `slint-1.6.0a8/internal/common/builtin_structs.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/enums.rs` & `slint-1.6.0a8/internal/common/enums.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/key_codes.rs` & `slint-1.6.0a8/internal/common/key_codes.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/lib.rs` & `slint-1.6.0a8/internal/common/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/sharedfontdb/DejaVuSans.ttf` & `slint-1.6.0a8/internal/common/sharedfontdb/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/sharedfontdb/fontconfig.rs` & `slint-1.6.0a8/internal/common/sharedfontdb/fontconfig.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/common/sharedfontdb.rs` & `slint-1.6.0a8/internal/common/sharedfontdb.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/const-field-offset/Cargo.toml` & `slint-1.6.0a8/helper_crates/const-field-offset/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/const-field-offset/CHANGELOG.md` & `slint-1.6.0a8/helper_crates/const-field-offset/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/const-field-offset/LICENSES/Apache-2.0.txt` & `slint-1.6.0a8/helper_crates/vtable/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/const-field-offset/LICENSES/MIT.txt` & `slint-1.6.0a8/helper_crates/vtable/macro/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/const-field-offset/src/lib.rs` & `slint-1.6.0a8/helper_crates/const-field-offset/src/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/const-field-offset/tests/test_field_offset.rs` & `slint-1.6.0a8/helper_crates/const-field-offset/tests/test_field_offset.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/testing/Cargo.toml` & `slint-1.6.0a8/internal/backends/testing/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/testing/README.md` & `slint-1.6.0a8/internal/backends/testing/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/testing/ffi.rs` & `slint-1.6.0a8/internal/backends/testing/ffi.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/testing/internal_tests.rs` & `slint-1.6.0a8/internal/backends/testing/internal_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/testing/lib.rs` & `slint-1.6.0a8/internal/backends/testing/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/testing/search_api.rs` & `slint-1.6.0a8/internal/backends/testing/search_api.rs`

 * *Files 16% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     ) -> impl Iterator<Item = Self> {
         // dirty way to get the ItemTreeRc:
         let item_tree = WindowInner::from_pub(component.window()).component();
         let result = search_item(&item_tree, |item| {
             item.accessible_string_property(AccessibleStringProperty::Label)
                 .is_some_and(|x| x == label)
         });
-        result.into_iter().map(|x| ElementHandle(x))
+        result.into_iter().map(ElementHandle)
     }
 
     /// Invokes the default accessible action on the element. For example a `MyButton` element might declare
     /// an accessible default action that simulates a click, as in the following example:
     ///
     /// ```slint,no-preview
     /// component MyButton {
@@ -92,14 +92,38 @@
     /// property if it is declared in your Slint code.
     pub fn set_accessible_value(&self, value: impl Into<SharedString>) {
         if let Some(item) = self.0.upgrade() {
             item.accessible_action(&AccessibilityAction::SetValue(value.into()))
         }
     }
 
+    /// Returns the value of the element's `accessible-value-maximum` property, if present.
+    pub fn accessible_value_maximum(&self) -> Option<f32> {
+        self.0.upgrade().and_then(|item| {
+            item.accessible_string_property(AccessibleStringProperty::ValueMaximum)
+                .and_then(|item| item.parse().ok())
+        })
+    }
+
+    /// Returns the value of the element's `accessible-value-minimum` property, if present.
+    pub fn accessible_value_minimum(&self) -> Option<f32> {
+        self.0.upgrade().and_then(|item| {
+            item.accessible_string_property(AccessibleStringProperty::ValueMinimum)
+                .and_then(|item| item.parse().ok())
+        })
+    }
+
+    /// Returns the value of the element's `accessible-value-step` property, if present.
+    pub fn accessible_value_step(&self) -> Option<f32> {
+        self.0.upgrade().and_then(|item| {
+            item.accessible_string_property(AccessibleStringProperty::ValueStep)
+                .and_then(|item| item.parse().ok())
+        })
+    }
+
     /// Returns the value of the `accessible-label` property, if present.
     pub fn accessible_label(&self) -> Option<SharedString> {
         self.0
             .upgrade()
             .and_then(|item| item.accessible_string_property(AccessibleStringProperty::Label))
     }
 
@@ -114,14 +138,22 @@
     pub fn accessible_checked(&self) -> Option<bool> {
         self.0
             .upgrade()
             .and_then(|item| item.accessible_string_property(AccessibleStringProperty::Checked))
             .and_then(|item| item.parse().ok())
     }
 
+    /// Returns the value of the `accessible-checkable` property, if present
+    pub fn accessible_checkable(&self) -> Option<bool> {
+        self.0
+            .upgrade()
+            .and_then(|item| item.accessible_string_property(AccessibleStringProperty::Checkable))
+            .and_then(|item| item.parse().ok())
+    }
+
     /// Returns the size of the element in logical pixels. This corresponds to the value of the `width` and
     /// `height` properties in Slint code. Returns a zero size if the element is not valid.
     pub fn size(&self) -> i_slint_core::api::LogicalSize {
         self.0
             .upgrade()
             .map(|item| {
                 let g = item.geometry();
```

### Comparing `slint-1.6.0a7/internal/backends/testing/testing_backend.rs` & `slint-1.6.0a8/internal/backends/testing/testing_backend.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/macro/Cargo.toml` & `slint-1.6.0a8/helper_crates/vtable/macro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt` & `slint-1.6.0a8/helper_crates/vtable/macro/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/macro/LICENSES/MIT.txt` & `slint-1.6.0a8/api/rs/slint/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/macro/macro.rs` & `slint-1.6.0a8/helper_crates/vtable/macro/macro.rs`

 * *Files 1% similar despite different names*

```diff
@@ -392,15 +392,15 @@
 
             // Add extern "C" if it isn't there
             if let Some(a) = &f.abi {
                 if !a.name.as_ref().map(|s| s.value() == "C").unwrap_or(false) {
                     return Error::new(a.span(), "invalid ABI").to_compile_error().into();
                 }
             } else {
-                f.abi = sig_extern.abi.clone();
+                f.abi.clone_from(&sig_extern.abi);
             }
 
             let mut wrap_trait_call = None;
             if !has_self {
                 sig.generics = Generics {
                     where_clause: Some(parse_str("where Self : Sized").unwrap()),
                     ..Default::default()
```

### Comparing `slint-1.6.0a7/internal/renderers/femtovg/Cargo.toml` & `slint-1.6.0a8/internal/renderers/femtovg/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/core/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/core/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/femtovg/fonts.rs` & `slint-1.6.0a8/internal/renderers/femtovg/fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/femtovg/images.rs` & `slint-1.6.0a8/internal/renderers/femtovg/images.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/femtovg/itemrenderer.rs` & `slint-1.6.0a8/internal/renderers/femtovg/itemrenderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/femtovg/lib.rs` & `slint-1.6.0a8/internal/renderers/femtovg/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/selector/Cargo.toml` & `slint-1.6.0a8/internal/backends/selector/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 authors.workspace = true
 edition.workspace = true
 homepage.workspace = true
 license.workspace = true
 repository.workspace = true
 rust-version.workspace = true
 version.workspace = true
+build = "build.rs"
 
 [lib]
 path = "lib.rs"
 
 [features]
 backend-winit = ["backend-winit-x11", "backend-winit-wayland"]
 backend-winit-x11 = ["i-slint-backend-winit/x11"]
```

### Comparing `slint-1.6.0a7/internal/backends/selector/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/backends/qt/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/selector/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/selector/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/selector/README.md` & `slint-1.6.0a8/internal/backends/selector/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/selector/build.rs` & `slint-1.6.0a8/internal/backends/selector/build.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 use std::path::Path;
 
 fn main() {
+    println!("cargo:rustc-check-cfg=cfg(no_qt)");
+
     // This is part code tries to detect automatically what default style to use and tries to
     // use the native style automatically if Qt is available.
     //
     // The way this work is this
     // 1. `qttypes`' crate's build script already detects Qt and set the DEP_QT_VERSION
     // 2. The qt rendering backend's build script will check if the qttype crates found Qt and
     //    look at the SLINT_NO_QT env variable, and sets the DEP_i_slint_backend_qt_SUPPORTS_NATIVE_STYLE
```

### Comparing `slint-1.6.0a7/internal/backends/selector/lib.rs` & `slint-1.6.0a8/internal/backends/selector/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/Cargo.toml` & `slint-1.6.0a8/helper_crates/vtable/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/CHANGELOG.md` & `slint-1.6.0a8/helper_crates/vtable/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/LICENSES/Apache-2.0.txt` & `slint-1.6.0a8/internal/compiler/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/LICENSES/MIT.txt` & `slint-1.6.0a8/internal/backends/linuxkms/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/src/compile_fail_tests.rs` & `slint-1.6.0a8/helper_crates/vtable/src/compile_fail_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/src/lib.rs` & `slint-1.6.0a8/helper_crates/vtable/src/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/src/vrc.rs` & `slint-1.6.0a8/helper_crates/vtable/src/vrc.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/tests/test_vrc.rs` & `slint-1.6.0a8/helper_crates/vtable/tests/test_vrc.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/vtable/tests/test_vtable.rs` & `slint-1.6.0a8/helper_crates/vtable/tests/test_vtable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/parser-test-macro/README.md` & `slint-1.6.0a8/internal/compiler/parser-test-macro/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/compiler/parser-test-macro/lib.rs` & `slint-1.6.0a8/internal/compiler/parser-test-macro/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/Cargo.toml` & `slint-1.6.0a8/internal/core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 homepage.workspace = true
 keywords.workspace = true
 license.workspace = true
 repository.workspace = true
 rust-version.workspace = true
 version.workspace = true
 categories = ["gui", "development-tools", "no-std"]
+build = "build.rs"
 
 [lib]
 path = "lib.rs"
 
 [features]
 ffi = [] # Expose C ABI
 libm = ["num-traits/libm", "euclid/libm"]
```

### Comparing `slint-1.6.0a7/internal/core/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/common/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/common/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/common/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/README.md` & `slint-1.6.0a8/internal/core/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/accessibility.rs` & `slint-1.6.0a8/internal/core/accessibility.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/animations.rs` & `slint-1.6.0a8/internal/core/animations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/api.rs` & `slint-1.6.0a8/internal/core/api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/callbacks.rs` & `slint-1.6.0a8/internal/core/callbacks.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/component_factory.rs` & `slint-1.6.0a8/internal/core/component_factory.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/context.rs` & `slint-1.6.0a8/internal/core/context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 use crate::Property;
 #[cfg(not(feature = "std"))]
 use alloc::boxed::Box;
 use alloc::rc::Rc;
 
 thread_local! {
     pub(crate) static GLOBAL_CONTEXT : once_cell::unsync::OnceCell<SlintContext>
-        = once_cell::unsync::OnceCell::new()
+        = const { once_cell::unsync::OnceCell::new() }
 }
 
 pub(crate) struct SlintContextInner {
     pub(crate) platform: Box<dyn Platform>,
     pub(crate) window_count: core::cell::RefCell<isize>,
     /// This property is read by all translations, and marked dirty when the language change
     /// so that every translated string gets re-translated
```

### Comparing `slint-1.6.0a7/internal/core/future.rs` & `slint-1.6.0a8/internal/core/future.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/bitmapfont.rs` & `slint-1.6.0a8/internal/core/graphics/bitmapfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/border_radius.rs` & `slint-1.6.0a8/internal/core/graphics/border_radius.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/boxshadowcache.rs` & `slint-1.6.0a8/internal/core/graphics/boxshadowcache.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/brush.rs` & `slint-1.6.0a8/internal/core/graphics/brush.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/color.rs` & `slint-1.6.0a8/internal/core/graphics/color.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/image/cache.rs` & `slint-1.6.0a8/internal/core/graphics/image/cache.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/image/htmlimage.rs` & `slint-1.6.0a8/internal/core/graphics/image/htmlimage.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/image/svg.rs` & `slint-1.6.0a8/internal/core/graphics/image/svg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/image.rs` & `slint-1.6.0a8/internal/core/graphics/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/path.rs` & `slint-1.6.0a8/internal/core/graphics/path.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics/rendering_metrics_collector.rs` & `slint-1.6.0a8/internal/core/graphics/rendering_metrics_collector.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/graphics.rs` & `slint-1.6.0a8/internal/core/graphics.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/input.rs` & `slint-1.6.0a8/internal/core/input.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/item_focus.rs` & `slint-1.6.0a8/internal/core/item_focus.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/item_rendering.rs` & `slint-1.6.0a8/internal/core/item_rendering.rs`

 * *Files 0% similar despite different names*

```diff
@@ -481,15 +481,15 @@
         }
         let mut i = 0;
         while i < self.count {
             let r = &self.rectangles[i];
             if r.contains_box(&b) {
                 // the rectangle is already in the union
                 return;
-            } else if b.contains_box(&r) {
+            } else if b.contains_box(r) {
                 self.rectangles.swap(i, self.count - 1);
                 self.count -= 1;
                 continue;
             }
             i += 1;
         }
```

### Comparing `slint-1.6.0a7/internal/core/item_tree.rs` & `slint-1.6.0a8/internal/core/item_tree.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/items/component_container.rs` & `slint-1.6.0a8/internal/core/items/component_container.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/items/flickable.rs` & `slint-1.6.0a8/internal/core/items/flickable.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/items/image.rs` & `slint-1.6.0a8/internal/core/items/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/items/path.rs` & `slint-1.6.0a8/internal/core/items/path.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/items/text.rs` & `slint-1.6.0a8/internal/core/items/text.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/items.rs` & `slint-1.6.0a8/internal/core/items.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/layout.rs` & `slint-1.6.0a8/internal/core/layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/lengths.rs` & `slint-1.6.0a8/internal/core/lengths.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/lib.rs` & `slint-1.6.0a8/internal/core/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/model/adapters.rs` & `slint-1.6.0a8/internal/core/model/adapters.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/model/model_peer.rs` & `slint-1.6.0a8/internal/core/model/model_peer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/model.rs` & `slint-1.6.0a8/internal/core/model.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/platform.rs` & `slint-1.6.0a8/internal/core/platform.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/properties/change_tracker.rs` & `slint-1.6.0a8/internal/core/properties/change_tracker.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/properties/ffi.rs` & `slint-1.6.0a8/internal/core/properties/ffi.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/properties/properties_animations.rs` & `slint-1.6.0a8/internal/core/properties/properties_animations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/properties.rs` & `slint-1.6.0a8/internal/core/properties.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/renderer.rs` & `slint-1.6.0a8/internal/core/renderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/rtti.rs` & `slint-1.6.0a8/internal/core/rtti.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/sharedvector.rs` & `slint-1.6.0a8/internal/core/sharedvector.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/slice.rs` & `slint-1.6.0a8/internal/core/slice.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/software_renderer/draw_functions.rs` & `slint-1.6.0a8/internal/core/software_renderer/draw_functions.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/software_renderer/fixed.rs` & `slint-1.6.0a8/internal/core/software_renderer/fixed.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/software_renderer/fonts/pixelfont.rs` & `slint-1.6.0a8/internal/core/software_renderer/fonts/pixelfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/software_renderer/fonts/systemfonts.rs` & `slint-1.6.0a8/internal/core/software_renderer/fonts/systemfonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/software_renderer/fonts/vectorfont.rs` & `slint-1.6.0a8/internal/core/software_renderer/fonts/vectorfont.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/software_renderer/fonts.rs` & `slint-1.6.0a8/internal/core/software_renderer/fonts.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/software_renderer.rs` & `slint-1.6.0a8/internal/core/software_renderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/string.rs` & `slint-1.6.0a8/internal/core/string.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/tests.rs` & `slint-1.6.0a8/internal/core/tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/textlayout/fragments.rs` & `slint-1.6.0a8/internal/core/textlayout/fragments.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/textlayout/glyphclusters.rs` & `slint-1.6.0a8/internal/core/textlayout/glyphclusters.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/textlayout/linebreak_simple.rs` & `slint-1.6.0a8/internal/core/textlayout/linebreak_simple.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/textlayout/linebreak_unicode.rs` & `slint-1.6.0a8/internal/core/textlayout/linebreak_unicode.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/textlayout/linebreaker.rs` & `slint-1.6.0a8/internal/core/textlayout/linebreaker.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/textlayout/shaping.rs` & `slint-1.6.0a8/internal/core/textlayout/shaping.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/textlayout.rs` & `slint-1.6.0a8/internal/core/textlayout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/timers.rs` & `slint-1.6.0a8/internal/core/timers.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/translations.rs` & `slint-1.6.0a8/internal/core/translations.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core/unsafe_single_threaded.rs` & `slint-1.6.0a8/internal/core/unsafe_single_threaded.rs`

 * *Files 22% similar despite different names*

```diff
@@ -2,23 +2,52 @@
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 //! Unsafe module that is only enabled when the `std` feature is off.
 //! It re-implements the thread_local macro with statics
 
 #![allow(unsafe_code)]
 #[macro_export]
-macro_rules! thread_local_ {
-    ($(#[$($meta:tt)*])* $vis:vis static $ident:ident : $ty:ty = $expr:expr) => {
+macro_rules! SLINT__thread_local_inner {
+    ($(#[$($meta:tt)*])* $vis:vis $ident:ident $ty:ty $block:block) => {
         $(#[$($meta)*])*
         $vis static $ident: crate::unsafe_single_threaded::FakeThreadStorage<$ty> = {
-            fn init() -> $ty { $expr }
+            fn init() -> $ty $block
             crate::unsafe_single_threaded::FakeThreadStorage::new(init)
         };
     };
 }
+
+#[macro_export]
+macro_rules! thread_local_ {
+    // Taken from stdlib!
+
+    // empty (base case for the recursion)
+    () => {};
+
+    ($(#[$attr:meta])* $vis:vis static $name:ident: $t:ty = const $init:block; $($rest:tt)*) => (
+        $crate::SLINT__thread_local_inner!($(#[$attr])* $vis $name $t $init);
+        $crate::thread_local!($($rest)*);
+    );
+
+    ($(#[$attr:meta])* $vis:vis static $name:ident: $t:ty = const $init:block) => (
+        $crate::SLINT__thread_local_inner!($(#[$attr])* $vis $name $t $init);
+    );
+
+    // process multiple declarations
+    ($(#[$attr:meta])* $vis:vis static $name:ident: $t:ty = $init:expr; $($rest:tt)*) => (
+        $crate::SLINT__thread_local_inner!($(#[$attr])* $vis $name $t  { $init });
+        $crate::thread_local!($($rest)*);
+    );
+
+    // handle a single declaration
+    ($(#[$attr:meta])* $vis:vis static $name:ident: $t:ty = $init:expr) => (
+        $crate::SLINT__thread_local_inner!($(#[$attr])* $vis $name $t { $init });
+    );
+}
+
 pub struct FakeThreadStorage<T, F = fn() -> T>(once_cell::unsync::OnceCell<T>, F);
 impl<T, F> FakeThreadStorage<T, F> {
     pub const fn new(f: F) -> Self {
         Self(once_cell::unsync::OnceCell::new(), f)
     }
 }
 impl<T> FakeThreadStorage<T> {
```

### Comparing `slint-1.6.0a7/internal/core/window.rs` & `slint-1.6.0a8/internal/core/window.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/Cargo.toml` & `slint-1.6.0a8/internal/backends/winit/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/api/rs/build/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/README.md` & `slint-1.6.0a8/internal/backends/winit/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/accesskit.rs` & `slint-1.6.0a8/internal/backends/winit/accesskit.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/event_loop.rs` & `slint-1.6.0a8/internal/backends/winit/event_loop.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/lib.rs` & `slint-1.6.0a8/internal/backends/winit/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -81,18 +81,18 @@
     }
 }
 
 fn default_renderer_factory(
     window_builder: winit::window::WindowBuilder,
 ) -> Result<(Box<dyn WinitCompatibleRenderer>, Rc<winit::window::Window>), PlatformError> {
     cfg_if::cfg_if! {
-        if #[cfg(feature = "renderer-femtovg")] {
-            renderer::femtovg::GlutinFemtoVGRenderer::new(window_builder)
-        } else if #[cfg(enable_skia_renderer)] {
+        if #[cfg(enable_skia_renderer)] {
             renderer::skia::WinitSkiaRenderer::new(window_builder)
+        } else if #[cfg(feature = "renderer-femtovg")] {
+            renderer::femtovg::GlutinFemtoVGRenderer::new(window_builder)
         } else if #[cfg(feature = "renderer-software")] {
             renderer::sw::WinitSoftwareRenderer::new(window_builder)
         } else {
             compile_error!("Please select a feature to build with the winit backend: `renderer-femtovg`, `renderer-skia`, `renderer-skia-opengl`, `renderer-skia-vulkan` or `renderer-software`");
         }
     }
 }
```

### Comparing `slint-1.6.0a7/internal/backends/winit/renderer/femtovg/glcontext.rs` & `slint-1.6.0a8/internal/backends/winit/renderer/femtovg/glcontext.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/renderer/femtovg.rs` & `slint-1.6.0a8/internal/backends/winit/renderer/femtovg.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/renderer/skia.rs` & `slint-1.6.0a8/internal/backends/winit/renderer/skia.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/renderer/sw.rs` & `slint-1.6.0a8/internal/backends/winit/renderer/sw.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/wasm_input_helper.rs` & `slint-1.6.0a8/internal/backends/winit/wasm_input_helper.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/winit/winitwindowadapter.rs` & `slint-1.6.0a8/internal/backends/winit/winitwindowadapter.rs`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,19 @@
             #[cfg(enable_accesskit)]
             accesskit_adapter: crate::accesskit::AccessKitAdapter::new(
                 self_weak.clone(),
                 &winit_window,
             ),
         });
 
-        let id = self_rc.winit_window().id();
+        let winit_window = self_rc.winit_window();
+        if let Err(e) = self_rc.renderer.resumed(&winit_window) {
+            i_slint_core::debug_log!("Error initialing renderer in winit backend with window: {e}");
+        }
+        let id = winit_window.id();
         crate::event_loop::register_window(id, (self_rc.clone()) as _);
 
         let scale_factor = std::env::var("SLINT_SCALE_FACTOR")
             .ok()
             .and_then(|x| x.parse::<f32>().ok())
             .filter(|f| *f > 0.)
             .unwrap_or_else(|| self_rc.winit_window().scale_factor() as f32);
```

### Comparing `slint-1.6.0a7/internal/renderers/skia/Cargo.toml` & `slint-1.6.0a8/internal/renderers/skia/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/api/rs/slint/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/cached_image.rs` & `slint-1.6.0a8/internal/renderers/skia/cached_image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/d3d_surface.rs` & `slint-1.6.0a8/internal/renderers/skia/d3d_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/itemrenderer.rs` & `slint-1.6.0a8/internal/renderers/skia/itemrenderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/lib.rs` & `slint-1.6.0a8/internal/renderers/skia/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/metal_surface.rs` & `slint-1.6.0a8/internal/renderers/skia/metal_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/opengl_surface.rs` & `slint-1.6.0a8/internal/renderers/skia/opengl_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/software_surface.rs` & `slint-1.6.0a8/internal/renderers/skia/software_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/textlayout.rs` & `slint-1.6.0a8/internal/renderers/skia/textlayout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/renderers/skia/vulkan_surface.rs` & `slint-1.6.0a8/internal/renderers/skia/vulkan_surface.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/const-field-offset/macro/Cargo.toml` & `slint-1.6.0a8/helper_crates/const-field-offset/macro/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/helper_crates/const-field-offset/macro/macro.rs` & `slint-1.6.0a8/helper_crates/const-field-offset/macro/macro.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/Cargo.toml` & `slint-1.6.0a8/internal/interpreter/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/backends/linuxkms/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/backends/linuxkms/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/api.rs` & `slint-1.6.0a8/internal/interpreter/api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/dynamic_item_tree.rs` & `slint-1.6.0a8/internal/interpreter/dynamic_item_tree.rs`

 * *Files 0% similar despite different names*

```diff
@@ -970,15 +970,15 @@
             debug_assert_eq!(self.original_elements.len(), self.tree_array.len());
             self.items_types.insert(
                 item.id.clone(),
                 ItemWithinItemTree { offset, rtti: rt.clone(), elem: rc_item.clone() },
             );
             for (prop, expr) in &item.change_callbacks {
                 self.change_callbacks.push((
-                    NamedReference::new(&rc_item, prop),
+                    NamedReference::new(rc_item, prop),
                     Expression::CodeBlock(expr.borrow().clone()),
                 ));
             }
         }
 
         fn enter_component(
             &mut self,
@@ -1809,15 +1809,15 @@
 
 extern "C" fn subtree_index(component: ItemTreeRefPin) -> usize {
     generativity::make_guard!(guard);
     let instance_ref = unsafe { InstanceRef::from_pin_ref(component, guard) };
     if let Ok(value) = instance_ref.description.get_property(component, SPECIAL_PROPERTY_INDEX) {
         value.try_into().unwrap()
     } else {
-        core::usize::MAX
+        usize::MAX
     }
 }
 
 unsafe extern "C" fn parent_node(component: ItemTreeRefPin, result: &mut ItemWeak) {
     generativity::make_guard!(guard);
     let instance_ref = InstanceRef::from_pin_ref(component, guard);
```

### Comparing `slint-1.6.0a7/internal/interpreter/dynamic_type.rs` & `slint-1.6.0a8/internal/interpreter/dynamic_type.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/eval.rs` & `slint-1.6.0a8/internal/interpreter/eval.rs`

 * *Files 1% similar despite different names*

```diff
@@ -932,26 +932,26 @@
             }
         }
         BuiltinFunction::Rgb => {
             let r: i32 = eval_expression(&arguments[0], local_context).try_into().unwrap();
             let g: i32 = eval_expression(&arguments[1], local_context).try_into().unwrap();
             let b: i32 = eval_expression(&arguments[2], local_context).try_into().unwrap();
             let a: f32 = eval_expression(&arguments[3], local_context).try_into().unwrap();
-            let r: u8 = r.max(0).min(255) as u8;
-            let g: u8 = g.max(0).min(255) as u8;
-            let b: u8 = b.max(0).min(255) as u8;
-            let a: u8 = (255. * a).max(0.).min(255.) as u8;
+            let r: u8 = r.clamp(0, 255) as u8;
+            let g: u8 = g.clamp(0, 255) as u8;
+            let b: u8 = b.clamp(0, 255) as u8;
+            let a: u8 = (255. * a).clamp(0., 255.) as u8;
             Value::Brush(Brush::SolidColor(Color::from_argb_u8(a, r, g, b)))
         }
         BuiltinFunction::Hsv => {
             let h: f32 = eval_expression(&arguments[0], local_context).try_into().unwrap();
             let s: f32 = eval_expression(&arguments[1], local_context).try_into().unwrap();
             let v: f32 = eval_expression(&arguments[2], local_context).try_into().unwrap();
             let a: f32 = eval_expression(&arguments[3], local_context).try_into().unwrap();
-            let a = (1. * a).max(0.).min(1.);
+            let a = (1. * a).clamp(0., 1.);
             Value::Brush(Brush::SolidColor(Color::from_hsva(h, s, v, a)))
         }
         BuiltinFunction::ColorScheme => match local_context.component_instance {
             ComponentInstance::InstanceRef(component) => component
                 .window_adapter()
                 .internal(corelib::InternalToken)
                 .map_or(ColorScheme::Unknown, |x| x.color_scheme())
```

### Comparing `slint-1.6.0a7/internal/interpreter/eval_layout.rs` & `slint-1.6.0a8/internal/interpreter/eval_layout.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/ffi.rs` & `slint-1.6.0a8/internal/interpreter/ffi.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/global_component.rs` & `slint-1.6.0a8/internal/interpreter/global_component.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/highlight.rs` & `slint-1.6.0a8/internal/interpreter/highlight.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/lib.rs` & `slint-1.6.0a8/internal/interpreter/lib.rs`

 * *Files 5% similar despite different names*

```diff
@@ -82,13 +82,17 @@
 #[cfg(feature = "highlight")]
 pub mod highlight;
 mod value_model;
 
 #[doc(inline)]
 pub use api::*;
 
+#[cfg(feature = "internal")]
+#[doc(hidden)]
+pub use eval::default_value_for_type;
+
 /// (Re-export from corelib.)
 #[doc(inline)]
 pub use i_slint_core::{Brush, Color, SharedString, SharedVector};
 
 #[cfg(test)]
 mod tests;
```

### Comparing `slint-1.6.0a7/internal/interpreter/migration.rs` & `slint-1.6.0a8/internal/interpreter/migration.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/tests.rs` & `slint-1.6.0a8/internal/interpreter/tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/interpreter/value_model.rs` & `slint-1.6.0a8/internal/interpreter/value_model.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/Cargo.toml` & `slint-1.6.0a8/api/rs/slint/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -160,15 +160,18 @@
 backend-linuxkms = ["i-slint-backend-selector/backend-linuxkms", "std"]
 
 ## KMS with Vulkan or EGL and libinput on Linux are used to render the application in full screen mode, without any
 ## windowing system. (Experimental)
 backend-linuxkms-noseat = ["i-slint-backend-selector/backend-linuxkms-noseat", "std"]
 
 ## Use the backend based on the [android-activity](https://docs.rs/android-activity) crate. (Using it's native activity feature)
-backend-android-activity-05 = ["i-slint-backend-android-activity/native-activity"]
+backend-android-activity-06 = ["i-slint-backend-android-activity/native-activity", "i-slint-backend-android-activity/aa-06"]
+
+## **Deprecated** Use previous version of android-activity. This is mutually exclusive with `backend-android-activity-06`.
+backend-android-activity-05 = ["i-slint-backend-android-activity/native-activity", "i-slint-backend-android-activity/aa-05"]
 
 [dependencies]
 i-slint-core = { workspace = true }
 slint-macros = { workspace = true }
 i-slint-backend-selector = { workspace = true }
 
 const-field-offset = { version = "0.1.2", path = "../../../helper_crates/const-field-offset" }
```

### Comparing `slint-1.6.0a7/api/rs/slint/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/compiler/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/compiler/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/compiler/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/LICENSES/MIT.txt` & `slint-1.6.0a8/internal/compiler/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/README.md` & `slint-1.6.0a8/api/rs/slint/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 The most basic "Hello world" application can be achieved with a few lines of code:
 
 In your `Cargo.toml` add:
 
 ```toml
 [dependencies]
-slint = "1.5.0"
+slint = "1.6.0"
 ```
 
 And in your `main.rs`:
 
 ```rust,no_run
 slint::slint!{
     export component HelloWorld {
```

### Comparing `slint-1.6.0a7/api/rs/slint/android.rs` & `slint-1.6.0a8/api/rs/slint/android.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 //! Android backend.
 //!
-//! **Note:** This module is only available on Android with the "backend-android-activity-05" feature
+//! **Note:** This module is only available on Android with the "backend-android-activity-06" feature
 //!
 //! Slint uses the [android-activity crate](https://github.com/rust-mobile/android-activity) as a backend.
 //!
 //! For convenience, Slint re-exports the content of the [`android-activity`](https://docs.rs/android-activity)  under `slint::android::android_activity`.
 //!
 //! As with every application using the android-activity crate, the entry point to your app will be the `android_main` function.
 //! From that function, you can call [`slint::android::init`](init()) or [`slint::android::init_with_event_listener`](init_with_event_listener)
@@ -29,23 +29,23 @@
 //!             Text { text: "Hello World"; }
 //!         }
 //!     }
 //!     MainWindow::new().unwrap().run().unwrap();
 //! }
 //! ```
 //!
-//! That function must be in a `cdylib` library, and you should enable the "backend-android-activity-05"`
+//! That function must be in a `cdylib` library, and you should enable the "backend-android-activity-06"`
 //! feature of the slint crate in your Cargo.toml:
 //!
 //! ```toml
 //! [lib]
 //! crate-type = ["cdylib"]
 //!
 //! [dependencies]
-//! slint = { version = "1.5", features = ["backend-android-activity-05"] }
+//! slint = { version = "1.6", features = ["backend-android-activity-06"] }
 //! ```
 //!
 //! ## Building and Deploying
 //!
 //! To build and deploy your application, we suggest the usage of [cargo-apk](https://github.com/rust-mobile/cargo-apk),
 //! a cargo subcommand that allows you to build, sign, and deploy Android APKs made in Rust.
 //!
@@ -59,18 +59,24 @@
 //! Please ensure that you have the Android NDK and SDK installed and properly set up in your development environment for the above command to work as expected.
 //! For detailed instructions on how to set up the Android NDK and SDK, please refer to the [Android Developer's guide](https://developer.android.com/studio/projects/install-ndk).
 //! The `ANDROID_HOME` and `ANDROID_NDK_ROOT` environment variable need to be set to the right path.
 //!
 //! Note Slint does not require a specific build tool and can work with others, such as [xbuild](https://github.com/rust-mobile/xbuild).
 
 /// Re-export of the android-activity crate.
-#[cfg(all(target_os = "android", feature = "backend-android-activity-05"))]
+#[cfg(all(
+    target_os = "android",
+    any(feature = "backend-android-activity-05", feature = "backend-android-activity-06")
+))]
 pub use i_slint_backend_android_activity::android_activity;
 
-#[cfg(not(all(target_os = "android", feature = "backend-android-activity-05")))]
+#[cfg(not(all(
+    target_os = "android",
+    any(feature = "backend-android-activity-05", feature = "backend-android-activity-06")
+)))]
 /// Re-export of the [android-activity](https://docs.rs/android-activity) crate.
 pub mod android_activity {
     #[doc(hidden)]
     pub struct AndroidApp;
     #[doc(hidden)]
     pub struct PollEvent<'a>(&'a ());
 }
@@ -79,30 +85,30 @@
 #[doc(no_inline)]
 pub use android_activity::AndroidApp;
 
 use crate::platform::SetPlatformError;
 
 /// Initializes the Android backend.
 ///
-/// **Note:** This function is only available on Android with the "backend-android-activity-05" feature
+/// **Note:** This function is only available on Android with the "backend-android-activity-06" feature
 ///
 /// This function must be called from the `android_main` function before any call to Slint that needs a backend.
 ///
 /// See the [module documentation](self) for an example on how to create Android application.
 ///
 /// See also [`init_with_event_listener`]
 pub fn init(app: android_activity::AndroidApp) -> Result<(), SetPlatformError> {
     crate::platform::set_platform(Box::new(i_slint_backend_android_activity::AndroidPlatform::new(
         app,
     )))
 }
 
 /// Similar to [`init()`], which allow to listen to android-activity's event
 ///
-/// **Note:** This function is only available on Android with the "backend-android-activity-05" feature
+/// **Note:** This function is only available on Android with the "backend-android-activity-06" feature
 ///
 /// The listener argument is a function that takes a [`android_activity::PollEvent`](https://docs.rs/android-activity/latest/android_activity/enum.PollEvent.html)
 ///
 /// # Example
 ///
 /// ```rust
 /// # #[cfg(target_os = "android")]
```

### Comparing `slint-1.6.0a7/api/rs/slint/compile_fail_tests.rs` & `slint-1.6.0a8/api/rs/slint/compile_fail_tests.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/building.md` & `slint-1.6.0a8/api/rs/slint/docs/building.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/development.md` & `slint-1.6.0a8/api/rs/slint/docs/development.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/install_qt.md` & `slint-1.6.0a8/api/rs/slint/docs/install_qt.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/README.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/conclusion.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/conclusion.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/creating_the_tiles_from_cpp.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/from_one_to_multiple_tiles.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/game_logic_in_cpp.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/getting_started.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/at-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/at.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/at.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/balance-scale.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/bus-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/bus.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/cloud.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/cogs-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/cogs.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/motorcycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/tile_logo.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/icons/video.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/icons/video.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/ideas_for_the_reader.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/introduction.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/introduction.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/main_game_logic.cpp`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/main_tiles_from_cpp.cpp`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/memory_game_logic.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/memory_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/memory_tiles_from_cpp.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/cpp/src/polishing_the_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/SUMMARY.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/conclusion.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/conclusion.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/creating_the_tiles_from_js.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/from_one_to_multiple_tiles.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/game_logic_in_js.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/getting_started.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/getting_started.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/at-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/at.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/at.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/balance-scale-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/balance-scale.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/bicycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/bicycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/bus-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/bus.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/bus.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cloud.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/cloud.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/cogs-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/cogs.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/cogs.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/motorcycle-solid.svg`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/motorcycle.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/tile_logo.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/icons/video.png` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/icons/video.png`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/ideas_for_the_reader.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/introduction.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/introduction.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_game_logic.js` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/main_game_logic.js`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/main_tiles_from_js.js`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/memory_game_logic.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tile.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/memory_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/memory_tiles_from_cpp.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/node/src/polishing_the_tile.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/quickstart/theme/head.hbs` & `slint-1.6.0a8/api/rs/slint/docs/quickstart/theme/head.hbs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/conf.py` & `slint-1.6.0a8/api/rs/slint/docs/reference/conf.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/index.rst` & `slint-1.6.0a8/api/rs/slint/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/backend_linuxkms.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backend_winit.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/backend_winit.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 |---------------|---------------------------------------------|------------------------------------------|
 | FemtoVG       | OpenGL                                      | `winit-femtovg`                          |
 | Skia          | OpenGL, Metal, Direct3D, Software-rendering | `winit-skia`                             |
 | Skia Software | Software-only rendering with Skia           | `winit-skia-software`                    |
 | Skia OpenGL   | OpenGL rendering with Skia                  | `winit-skia-opengl`                      |
 | software      | Software-rendering, no GPU required         | `winit-software`                         |
 
+If no renderer is explicitly set, the backend will first try to use the Skia renderer, if it was enabled at compile time.
+If that fails, it will fall back to the FemtoVG renderer, and if that also fails, it will use the software renderer.
+
 
 ## Configuration Options
 
 The Winit backend reads and interprets the following environment variables:
 
 | Name               | Accepted Values | Description                                                        |
 |--------------------|-----------------|--------------------------------------------------------------------|
```

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/backends_and_renderers.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/debugging_techniques.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/advanced/style.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/advanced/style.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/introduction/index.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/introduction/index.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/introduction/supported_platforms.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/introduction/supported_platforms.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/callbacks.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/callbacks.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/elements.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/elements.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/functions.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/functions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/globals.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/globals.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/builtins/namespaces.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/builtins/namespaces.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,17 @@
 -   **`Stop`**
 -   **`Menu`**
 
 ## `Math`
 
 These functions are available both in the global scope and in the `Math` namespace.
 
-### `abs(float) -> float`
+### `abs(T) -> T`
 
-Return the absolute value.
+Return the absolute value, where T is a numeric type.
 
 ### `acos(float) -> angle`, `asin(float) -> angle`, `atan(float) -> angle`, `cos(angle) -> float`, `sin(angle) -> float`, `tan(angle) -> float`
 
 The trigonometry function. Note that the should be typed with `deg` or `rad` unit
 (for example `cos(90deg)` or `sin(slider.value * 1deg)`).
 
 ### `ceil(float) -> int` and `floor(float) -> int`
```

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/container.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/container.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/file.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/file.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/focus.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/focus.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/fonts.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/fonts.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/layouting.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/layouting.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/purity.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/purity.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/concepts/translations.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/concepts/translations.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/index.rst` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/animations.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/animations.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/callbacks.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/callbacks.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/expressions.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/expressions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/functions.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/functions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/globals.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/globals.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/legacy_syntax.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/modules.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/modules.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/properties.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/properties.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/repetitions.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/repetitions.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/statements.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/statements.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/states.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/states.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/syntax/types.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/syntax/types.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/button.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/button.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/checkbox.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/checkbox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/combobox.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/combobox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/groupbox.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/groupbox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/index.rst` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/index.rst`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/lineedit.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/lineedit.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/listview.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/listview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/progressindicator.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/scrollview.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/scrollview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/slider.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/slider.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/spinbox.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/spinbox.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/spinner.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/spinner.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/standardbutton.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/standardlistview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/standardtableview.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/switch.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/switch.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/tabwidget.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/textedit.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/textedit.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/language/widgets/widgets.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/language/widgets/widgets.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/reference/src/recipes/recipes.md` & `slint-1.6.0a8/api/rs/slint/docs/reference/src/recipes/recipes.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/resources/slint-docs-highlight.html` & `slint-1.6.0a8/api/rs/slint/docs/resources/slint-docs-highlight.html`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/resources/slint-docs-preview.html` & `slint-1.6.0a8/api/rs/slint/docs/resources/slint-docs-preview.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <!--
     This file is used to add preview of the `.slint` snippets in the generated rustdoc documentation.
     It can be injected via the `--html-in-header slint-docs-preview.html` option of rustdoc.
 -->
 <script type="module">
     "use strict";
-    //import * as slint from 'https://releases.slint.dev/0.x.0/wasm-interpreter/slint_wasm_interpreter.js';
-    //const editor_url = "https://releases.slint.dev/0.x.0/editor/";
-    import * as slint from 'https://snapshots.slint.dev/master/wasm-interpreter/slint_wasm_interpreter.js';
-    const editor_url = "https://snapshots.slint.dev/master/editor/";
+    import * as slint from 'https://releases.slint.dev/1.6.0/wasm-interpreter/slint_wasm_interpreter.js';
+    const editor_url = "https://releases.slint.dev/1.6.0/editor/";
+    //import * as slint from 'https://snapshots.slint.dev/master/wasm-interpreter/slint_wasm_interpreter.js';
+    //const editor_url = "https://snapshots.slint.dev/master/editor/";
     // keep them alive
     var all_instances = new Array;
 
     async function render_or_error(source, div) {
         let canvas_id = 'canvas_' + Math.random().toString(36).substr(2, 9);
         let canvas = document.createElement("canvas");
         canvas.id = canvas_id;
```

### Comparing `slint-1.6.0a7/api/rs/slint/docs/site/index.html` & `slint-1.6.0a8/api/rs/slint/docs/site/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         <meta name="author" content="SixtyFPS GmbH" />
 
         <!--====== Favicon Icon ======-->
         <link rel="shortcut icon" href="https://slint.dev/assets/img/favicon.ico">
         <link rel="icon" type="image/x-icon" href="https://slint.dev/assets/img/favicon.svg">
 
         <!-- ===== All CSS files ===== -->
-        <link rel="stylesheet" href="https://slint.dev/assets/css/style.css?v=1.12.0" />
+        <link rel="stylesheet" href="https://slint.dev/assets/css/style.css?v=1.12.2" />
         
 
         <!-- ===== Header from individual pages ===== -->
         
         <title>Slint Developer Documentation</title>
         <meta name="description" content="The developer documentation page of Slint." />
```

### Comparing `slint-1.6.0a7/api/rs/slint/docs/testing.md` & `slint-1.6.0a8/api/rs/slint/docs/testing.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/torizon.md` & `slint-1.6.0a8/api/rs/slint/docs/torizon.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs/triage.md` & `slint-1.6.0a8/api/rs/slint/docs/triage.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/docs.rs` & `slint-1.6.0a8/api/rs/slint/docs.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/lib.rs` & `slint-1.6.0a8/api/rs/slint/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,19 @@
 ```toml
 [package]
 ...
 build = "build.rs"
 edition = "2021"
 
 [dependencies]
-slint = "1.5.0"
+slint = "1.6.0"
 ...
 
 [build-dependencies]
-slint-build = "1.5.0"
+slint-build = "1.6.0"
 ```
 
 Use the API of the slint-build crate in the `build.rs` file:
 
 ```rust,no_run
 fn main() {
     slint_build::compile("ui/hello.slint").unwrap();
@@ -314,15 +314,21 @@
     #[cfg(all(feature = "renderer-femtovg", not(target_os = "android")))]
     pub mod femtovg_renderer {
         pub use i_slint_renderer_femtovg::FemtoVGRenderer;
         pub use i_slint_renderer_femtovg::OpenGLInterface;
     }
 }
 
-#[cfg(any(doc, all(target_os = "android", feature = "backend-android-activity-05")))]
+#[cfg(any(
+    doc,
+    all(
+        target_os = "android",
+        any(feature = "backend-android-activity-05", feature = "backend-android-activity-06")
+    )
+))]
 pub mod android;
 
 /// Helper type that helps checking that the generated code is generated for the right version
 #[doc(hidden)]
 #[allow(non_camel_case_types)]
 pub struct VersionCheck_1_6_0;
```

### Comparing `slint-1.6.0a7/api/rs/slint/mcu.md` & `slint-1.6.0a8/api/rs/slint/mcu.md`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ## Changes to `Cargo.toml`
 
 Start by adding a dependency to the `slint` and the `slint-build` crates to your `Cargo.toml` using the `cargo` command:
 
 Start with the `slint` crate like this:
 
 ```sh
-cargo add slint@1.5.0 --no-default-features --features "compat-1-2 unsafe-single-threaded libm"
+cargo add slint@1.6.0 --no-default-features --features "compat-1-2 unsafe-single-threaded libm"
 ```
 
 The default features of the `slint` crate are tailored towards hosted environments and includes the "std" feature. In bare metal environments,
 you need to disable the default features.
 
 In the snippet above, three features are selected:
 
@@ -47,15 +47,15 @@
 It might be necessary to enable the [Feature resolver version 2](https://doc.rust-lang.org/cargo/reference/features.html#feature-resolver-version-2)
 in your Cargo.toml if you notice that your dependencies are attempting to build with `std` support even when disabled.
 This is the default when using the Rust 2021 Edition, but not if you use a workspace.
 
 Then add the `slint-build` crate as a build dependency:
 
 ```sh
-cargo add --build slint-build@1.5.0
+cargo add --build slint-build@1.6.0
 ```
 
 For reference: These are the relevant parts of your `Cargo.toml` file,
 ready to use Slint:
 
 ```toml
 [package]
@@ -63,19 +63,19 @@
 ## Edition 2021 or later enables the feature resolver version 2.
 edition = "2021"
 
 [dependencies]
 ## ... your other dependencies
 
 [dependencies.slint]
-version = "1.5.0"
+version = "1.6.0"
 default-features = false
 features = ["compat-1-2", "unsafe-single-threaded", "libm"]
 [build-dependencies]
-slint-build = "1.5.0"
+slint-build = "1.6.0"
 ```
 
 ## Changes to `build.rs`
 
 Next, write a build script to compile the `.slint` files to Rust code for embedding into the program binary, using the `slint-build` crate:
 
 ```rust,no_run
```

### Comparing `slint-1.6.0a7/api/rs/slint/private_unstable_api.rs` & `slint-1.6.0a8/api/rs/slint/private_unstable_api.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/tests/partial_renderer.rs` & `slint-1.6.0a8/api/rs/slint/tests/partial_renderer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/tests/show_strongref.rs` & `slint-1.6.0a8/api/rs/slint/tests/show_strongref.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/tests/simple_macro.rs` & `slint-1.6.0a8/api/rs/slint/tests/simple_macro.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/tests/spawn_local.rs` & `slint-1.6.0a8/api/rs/slint/tests/spawn_local.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/slint/type-mappings.md` & `slint-1.6.0a8/api/rs/slint/type-mappings.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/Cargo.toml` & `slint-1.6.0a8/api/rs/build/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 # Copyright © SixtyFPS GmbH <info@slint.dev>
 # SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 [package]
-name = "i-slint-backend-android-activity"
-description = "OpenGL rendering backend for Slint"
+name = "slint-build"
+description = "Helper for Slint build script"
 authors.workspace = true
 edition.workspace = true
-homepage.workspace = true
+homepage = "https://slint.rs"
+keywords.workspace = true
 license.workspace = true
 repository.workspace = true
 rust-version.workspace = true
 version.workspace = true
+categories = ["gui", "rendering::engine", "development-tools::build-utils"]
 
 [lib]
 path = "lib.rs"
 
 [features]
-game-activity = ["android-activity/game-activity"]
-native-activity = ["android-activity/native-activity"]
+default = []
 
-[target.'cfg(target_os = "android")'.dependencies]
-i-slint-renderer-skia = { workspace = true }
-i-slint-core = { workspace = true, features = ["std"] }
-raw-window-handle = { version = "0.5.2" }
-android-activity = { version = "0.5" }
-ndk = { version = "0.8.0", features = ["rwh_05"] }
-jni = { version = "0.21", features = ["invocation"] }
+[dependencies]
+i-slint-compiler = { workspace = true, features = ["default", "rust", "display-diagnostics", "software-renderer"] }
 
-[package.metadata.docs.rs]
-targets = [
-    "aarch64-linux-android",
-    "armv7-linux-androideabi",
-    "i686-linux-android",
-    "x86_64-linux-android",
-]
-features = ["native-activity"]
+spin_on = "0.1"
+thiserror = "1"
+toml_edit = { workspace = true }
```

### Comparing `slint-1.6.0a7/internal/backends/android-activity/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/backends/winit/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/backends/winit/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/backends/winit/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/README.md` & `slint-1.6.0a8/internal/backends/android-activity/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/androidwindowadapter.rs` & `slint-1.6.0a8/internal/backends/android-activity/androidwindowadapter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/build.rs` & `slint-1.6.0a8/internal/backends/android-activity/build.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/java/SlintAndroidJavaHelper.java` & `slint-1.6.0a8/internal/backends/android-activity/java/SlintAndroidJavaHelper.java`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/javahelper.rs` & `slint-1.6.0a8/internal/backends/android-activity/javahelper.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/android-activity/lib.rs` & `slint-1.6.0a8/internal/backends/android-activity/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,21 @@
 #![doc(html_logo_url = "https://slint.dev/logo/slint-logo-square-light.svg")]
 #![cfg_attr(not(target_os = "android"), allow(rustdoc::broken_intra_doc_links))]
 #![cfg(target_os = "android")]
 
 mod androidwindowadapter;
 mod javahelper;
 
+#[cfg(all(not(feature = "aa-06"), feature = "aa-05"))]
+pub use android_activity_05 as android_activity;
+#[cfg(feature = "aa-06")]
+pub use android_activity_06 as android_activity;
+
+pub use android_activity::AndroidApp;
 use android_activity::PollEvent;
-pub use android_activity::{self, AndroidApp};
 use androidwindowadapter::AndroidWindowAdapter;
 use core::ops::ControlFlow;
 use i_slint_core::api::{EventLoopError, PlatformError};
 use i_slint_core::platform::{Clipboard, WindowAdapter};
 use i_slint_renderer_skia::SkiaRendererExt;
 use std::cell::RefCell;
 use std::rc::{Rc, Weak};
```

### Comparing `slint-1.6.0a7/api/rs/build/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/renderers/femtovg/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/build/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/build/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/renderers/femtovg/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/rs/build/lib.rs` & `slint-1.6.0a8/api/rs/build/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 
 ```toml
 [package]
 ...
 build = "build.rs"
 
 [dependencies]
-slint = "1.5.0"
+slint = "1.6.0"
 ...
 
 [build-dependencies]
-slint-build = "1.5.0"
+slint-build = "1.6.0"
 ```
 
 In the `build.rs` file:
 
 ```ignore
 fn main() {
     slint_build::compile("ui/hello.slint").unwrap();
```

### Comparing `slint-1.6.0a7/internal/backends/qt/Cargo.toml` & `slint-1.6.0a8/internal/backends/qt/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/internal/interpreter/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/internal/interpreter/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/internal/interpreter/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/accessible_generated.rs` & `slint-1.6.0a8/internal/backends/qt/accessible_generated.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/build.rs` & `slint-1.6.0a8/internal/backends/qt/build.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // Copyright © SixtyFPS GmbH <info@slint.dev>
 // SPDX-License-Identifier: GPL-3.0-only OR LicenseRef-Slint-Royalty-free-1.2 OR LicenseRef-Slint-commercial
 
 // cSpell: ignore listviewitem stylemetrics
 
 #[cfg(feature = "enable")]
 fn main() {
+    println!("cargo:rustc-check-cfg=cfg(no_qt)");
+
     println!("cargo:rerun-if-env-changed=SLINT_NO_QT");
     if std::env::var("TARGET").map_or(false, |t| t.starts_with("wasm"))
         || std::env::var("SLINT_NO_QT").is_ok()
     {
         println!("cargo:rustc-cfg=no_qt");
         return;
     }
```

### Comparing `slint-1.6.0a7/internal/backends/qt/key_generated.rs` & `slint-1.6.0a8/internal/backends/qt/key_generated.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/lib.rs` & `slint-1.6.0a8/internal/backends/qt/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_accessible.rs` & `slint-1.6.0a8/internal/backends/qt/qt_accessible.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/button.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/button.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/checkbox.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/checkbox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/combobox.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/combobox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/groupbox.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/groupbox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/lineedit.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/lineedit.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/listviewitem.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/listviewitem.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/palette.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/palette.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/progress_indicator.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/progress_indicator.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/scrollview.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/scrollview.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/slider.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/slider.rs`

 * *Files 1% similar despite different names*

```diff
@@ -213,16 +213,18 @@
                 }
                 data.pressed_x = if vertical { pos.y as f32 } else { pos.x as f32 };
                 data.pressed = 1;
                 data.pressed_val = self.value();
                 InputEventResult::GrabMouse
             }
             MouseEvent::Exit | MouseEvent::Released { button: PointerEventButton::Left, .. } => {
+                if data.pressed != 0 {
+                    Self::FIELD_OFFSETS.released.apply_pin(self).call(&(self.value(),));
+                }
                 data.pressed = 0;
-                Self::FIELD_OFFSETS.released.apply_pin(self).call(&(self.value(),));
                 InputEventResult::EventAccepted
             }
             MouseEvent::Moved { position: pos } => {
                 let (coord, size) =
                     if vertical { (pos.y, size.height) } else { (pos.x, size.width) };
                 if data.pressed != 0 {
                     // FIXME: use QStyle::subControlRect to find out the actual size of the groove
```

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/spinbox.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/spinbox.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/stylemetrics.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/stylemetrics.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/tableheadersection.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/tableheadersection.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets/tabwidget.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets/tabwidget.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_widgets.rs` & `slint-1.6.0a8/internal/backends/qt/qt_widgets.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/backends/qt/qt_window.rs` & `slint-1.6.0a8/internal/backends/qt/qt_window.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core-macros/Cargo.toml` & `slint-1.6.0a8/internal/core-macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core-macros/LICENSES/GPL-3.0-only.txt` & `slint-1.6.0a8/api/rs/macros/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core-macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md` & `slint-1.6.0a8/api/rs/macros/LICENSES/LicenseRef-Slint-Royalty-free-1.2.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core-macros/LICENSES/LicenseRef-Slint-commercial.md` & `slint-1.6.0a8/api/rs/macros/LICENSES/LicenseRef-Slint-commercial.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core-macros/README.md` & `slint-1.6.0a8/internal/core-macros/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/internal/core-macros/lib.rs` & `slint-1.6.0a8/internal/core-macros/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/Cargo.toml` & `slint-1.6.0a8/api/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/README.md` & `slint-1.6.0a8/api/python/README.md`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/brush.rs` & `slint-1.6.0a8/api/python/brush.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/errors.rs` & `slint-1.6.0a8/api/python/errors.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/image.rs` & `slint-1.6.0a8/api/python/image.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/interpreter.rs` & `slint-1.6.0a8/api/python/interpreter.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/lib.rs` & `slint-1.6.0a8/api/python/lib.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/models.rs` & `slint-1.6.0a8/api/python/models.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/slint/__init__.py` & `slint-1.6.0a8/api/python/slint/__init__.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/slint/models.py` & `slint-1.6.0a8/api/python/slint/models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_brush.py` & `slint-1.6.0a8/api/python/tests/test_brush.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_callback_decorators.py` & `slint-1.6.0a8/api/python/tests/test_callback_decorators.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_compiler.py` & `slint-1.6.0a8/api/python/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_gc.py` & `slint-1.6.0a8/api/python/tests/test_gc.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_instance.py` & `slint-1.6.0a8/api/python/tests/test_instance.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_load_file.py` & `slint-1.6.0a8/api/python/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_load_file.slint` & `slint-1.6.0a8/api/python/tests/test_load_file.slint`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_loader.py` & `slint-1.6.0a8/api/python/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_models.py` & `slint-1.6.0a8/api/python/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/tests/test_timers.py` & `slint-1.6.0a8/api/python/tests/test_timers.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/timer.rs` & `slint-1.6.0a8/api/python/timer.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/api/python/value.rs` & `slint-1.6.0a8/api/python/value.rs`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/Cargo.lock` & `slint-1.6.0a8/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 dependencies = [
  "chrono",
  "slint",
 ]
 
 [[package]]
 name = "ab_glyph"
-version = "0.2.25"
+version = "0.2.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f90148830dac590fac7ccfe78ec4a8ea404c60f75a24e16407a71f0f40de775"
+checksum = "2e53b0a3d5760cd2ba9b787ae0c6440ad18ee294ff71b05e3381c900a7d16cfd"
 dependencies = [
  "ab_glyph_rasterizer",
  "owned_ttf_parser",
 ]
 
 [[package]]
 name = "ab_glyph_rasterizer"
@@ -189,17 +189,38 @@
  "bitflags 2.5.0",
  "cc",
  "cesu8",
  "jni",
  "jni-sys",
  "libc",
  "log",
- "ndk",
+ "ndk 0.8.0",
  "ndk-context",
- "ndk-sys",
+ "ndk-sys 0.5.0+25.2.9519653",
+ "num_enum 0.7.2",
+ "thiserror",
+]
+
+[[package]]
+name = "android-activity"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef6978589202a00cd7e118380c448a08b6ed394c3a8df3a430d0898e3a42d046"
+dependencies = [
+ "android-properties",
+ "bitflags 2.5.0",
+ "cc",
+ "cesu8",
+ "jni",
+ "jni-sys",
+ "libc",
+ "log",
+ "ndk 0.9.0",
+ "ndk-context",
+ "ndk-sys 0.6.0+11769913",
  "num_enum 0.7.2",
  "thiserror",
 ]
 
 [[package]]
 name = "android-properties"
 version = "0.2.2"
@@ -268,17 +289,17 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "25bdb32cbbdce2b519a9cd7df3a678443100e265d5e25ca763b7572a5104f5f3"
 
 [[package]]
 name = "arrayref"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
 
@@ -311,17 +332,17 @@
 dependencies = [
  "event-listener 2.5.3",
  "futures-core",
 ]
 
 [[package]]
 name = "async-channel"
-version = "2.2.1"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "136d4d23bcc79e27423727b36823d86233aad06dfea531837b038394d11e9928"
+checksum = "9f2776ead772134d55b62dd45e59a79e21612d85d0af729b8b7d3967d601a62a"
 dependencies = [
  "concurrent-queue",
  "event-listener 5.3.0",
  "event-listener-strategy 0.5.2",
  "futures-core",
  "pin-project-lite",
 ]
@@ -473,15 +494,15 @@
 name = "async-recursion"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b43422f69d8ff38f95f1b2bb76517c91589a924d1559a0e935d7c8ce0274c11"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "async-signal"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "afe66191c335039c7bb78f99dc7520b0cbb166b3a1cb33a03f53d8a1c6f2afda"
@@ -508,15 +529,15 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "atomic-polyfill"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cf2bce30dfe09ef0bfaef228b9d414faaf7e563035494d7fe092dba54b300f4"
@@ -589,22 +610,22 @@
 version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1899bfcfd9340ceea3533ea157360ba8fa864354eccbceab58e1006ecab35393"
 dependencies = [
  "derive_utils",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "az"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
 
@@ -694,15 +715,15 @@
  "log",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.60",
+ "syn 2.0.63",
  "which 4.4.2",
 ]
 
 [[package]]
 name = "bit_field"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -841,15 +862,15 @@
 name = "bytemuck_derive"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
@@ -917,17 +938,17 @@
  "syn 1.0.109",
  "tempfile",
  "toml 0.5.11",
 ]
 
 [[package]]
 name = "cc"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "065a29261d53ba54260972629f9ca6bffa69bac13cd1fed61420f7fa68b9f8bd"
+checksum = "099a5357d84c4c61eb35fc8eafa9a79a902c2f76911e5747ced4e032edd8d9b4"
 dependencies = [
  "jobserver",
  "libc",
  "once_cell",
 ]
 
 [[package]]
@@ -965,17 +986,17 @@
 name = "cfg_aliases"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
 
 [[package]]
 name = "cfg_aliases"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77e53693616d3075149f4ead59bdeecd204ac6b8192d8969757601b74bddf00f"
+checksum = "613afe47fcd5fac7ccf1db93babcb082c5994d996f20b8b159f2ad1658eb5724"
 
 [[package]]
 name = "cgl"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ced0551234e87afee12411d535648dd89d2e7f34c78b753395567aff3d447ff"
 dependencies = [
@@ -1005,52 +1026,52 @@
  "glob",
  "libc",
  "libloading 0.8.3",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.4"
+version = "4.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
+checksum = "1e578d6ec4194633722ccf9544794b71b1385c3c027efe0c55db226fc880865c"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.5.2"
+version = "4.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
+checksum = "4df4df40ec50c46000231c914968278b1eb05098cf8f1b3a518a95030e71d1c7"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
- "strsim 0.11.1",
+ "strsim",
  "terminal_size",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.5.4"
+version = "4.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
+checksum = "cf9804afaaf59a91e75b022a30fb7229a7901f60c755489cc61c9b423b836442"
 dependencies = [
- "heck 0.5.0",
+ "heck 0.4.1",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.7.0"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
+checksum = "702fc72eb24e5a1e48ce58027a675bc24edd52096d5397d4aea7c6dd9eca0bd1"
 
 [[package]]
 name = "clipboard-win"
 version = "3.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fdf5e01086b6be750428ba4a40619f847eb2e95756eee84b18e06e5f0b50342"
 dependencies = [
@@ -1176,15 +1197,15 @@
 name = "const-field-offset-macro"
 version = "0.1.5"
 dependencies = [
  "const-field-offset",
  "memoffset 0.9.1",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "const_format"
 version = "0.2.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3a214c7af3d04997541b18d432afaff4c455e79e2029079647e72fc2bd27673"
@@ -1391,15 +1412,15 @@
  "core-foundation-sys",
  "coreaudio-rs",
  "dasp_sample",
  "jni",
  "js-sys",
  "libc",
  "mach2",
- "ndk",
+ "ndk 0.8.0",
  "ndk-context",
  "oboe",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "windows",
 ]
@@ -1420,42 +1441,42 @@
 checksum = "0e361fae2caf9758164b24da3eedd7f7d7451be30d90d8e7b5d2be29a2f0cf5b"
 dependencies = [
  "cc",
  "cpp_common",
  "lazy_static",
  "proc-macro2",
  "regex",
- "syn 2.0.60",
+ "syn 2.0.63",
  "unicode-xid",
 ]
 
 [[package]]
 name = "cpp_common"
 version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e1a2532e4ed4ea13031c13bc7bc0dbca4aae32df48e9d77f0d1e743179f2ea1"
 dependencies = [
  "lazy_static",
  "proc-macro2",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "cpp_macros"
 version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "47ec9cc90633446f779ef481a9ce5a0077107dd5b87016440448d908625a83fd"
 dependencies = [
  "aho-corasick",
  "byteorder",
  "cpp_common",
  "lazy_static",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "cpufeatures"
 version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
@@ -1583,15 +1604,15 @@
 [[package]]
 name = "ctor"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "edb49164822f3ee45b17acd4a208cfc1251410cf0cad9a833234c9890774dd9f"
 dependencies = [
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "cursor-icon"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96a6ac251f4a2aca6b3f91340350eab87ae57c3f127ffeb585e92bd336717991"
@@ -1612,27 +1633,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
- "strsim 0.10.0",
- "syn 2.0.60",
+ "strsim",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "dasp_sample"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c87e182de0887fd5361989c677c4e8f5000cd9491d6d563161a8f3a5519fc7f"
@@ -1665,15 +1686,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "18bdc7a7b92ac413e19e95240e75d3a73a8d8e78aa24a594c22cbb4d44b4bbda"
 dependencies = [
  "defmt-parser",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "defmt-parser"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff4a5fefe330e8d7f31b16a318f9ce81000d8e35e69b93eae154d16d2278f70f"
@@ -1719,15 +1740,15 @@
 name = "derive_utils"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61bb5a1014ce6dfc2a378578509abe775a5aa06bff584a547555d9efdb81b926"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
@@ -1778,17 +1799,17 @@
  "byte-slice-cast",
  "display-interface",
  "embedded-hal",
 ]
 
 [[package]]
 name = "dissimilar"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "440d59c0c6d96354061909b4769b2ca03868dbaee203e7b779d9021ebbde3058"
+checksum = "59f8e79d1fbf76bdfbde321e902714bf6c49df88a7dda6fc682fc2979226962d"
 
 [[package]]
 name = "divan"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0d567df2c9c2870a43f3f2bd65aaeb18dbce1c18f217c3e564b4fbaeb3ee56c"
 dependencies = [
@@ -1804,15 +1825,15 @@
 name = "divan-macros"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27540baf49be0d484d8f0130d7d8da3011c32a44d4fc873368154f1510e574a2"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "dlib"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "330c60081dcc4c72131f8eb70510f1ac07223e5d4163db481a04a0befcffa412"
@@ -2075,15 +2096,15 @@
 name = "enumflags2_derive"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c785274071b1b420972453b306eeca06acf4633829db4223b58a2a8c5953bc4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "env_filter"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a009aa4810eb158359dda09d0c87378e4bbb89b5a801f016885a4707ba24f7ea"
@@ -2109,17 +2130,17 @@
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "esp-alloc"
@@ -2186,15 +2207,15 @@
 checksum = "d4cdf19581f9b0bb2b57b1549a2e639342825344b52f34048ddb29c46efa30de"
 dependencies = [
  "darling",
  "proc-macro-crate 1.3.1",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "esp-println"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "678ad508e8e61561eccee27003a5033901fe07fe8700508c324849b3df930ef5"
@@ -2599,15 +2620,15 @@
 name = "foreign-types-macros"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a5c6c585bc94aaf2c7b51dd4c2ba22680844aba4c687be581871a6f518c5742"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
@@ -2668,27 +2689,27 @@
 name = "frunk_derives"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fa992f1656e1707946bbba340ad244f0814009ef8c0118eb7b658395f19a2e"
 dependencies = [
  "frunk_proc_macro_helpers",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "frunk_proc_macro_helpers"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "35b54add839292b743aeda6ebedbd8b11e93404f902c56223e51b9ec18a13d2c"
 dependencies = [
  "frunk_core",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "ft5336"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "432cd93aa1378ad78d4e1048e9dba7622cfde09f04eb9b261ca6dcf0d358a3d4"
@@ -2785,15 +2806,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -2892,17 +2913,17 @@
 dependencies = [
  "libc",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -2995,15 +3016,15 @@
 checksum = "0bb0228f477c0900c880fd78c8759b95c7636dbd7842707f49e132378aa2acdc"
 dependencies = [
  "heck 0.4.1",
  "proc-macro-crate 2.0.0",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "glib-sys"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "063ce2eb6a8d0ea93d2bf8ba1957e78dbab6be1c2220dd3daca57d5a9d869898"
@@ -3118,15 +3139,15 @@
  "futures-util",
  "glib",
  "gstreamer-sys",
  "itertools 0.12.1",
  "libc",
  "muldiv",
  "num-integer",
- "num-rational 0.4.1",
+ "num-rational 0.4.2",
  "option-operations",
  "paste",
  "pin-project-lite",
  "pretty-hex",
  "smallvec",
  "thiserror",
 ]
@@ -3448,19 +3469,21 @@
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "i-slint-backend-android-activity"
 version = "1.6.0"
 dependencies = [
- "android-activity",
+ "android-activity 0.5.2",
+ "android-activity 0.6.0",
  "i-slint-core",
  "i-slint-renderer-skia",
  "jni",
- "ndk",
+ "ndk 0.8.0",
+ "ndk 0.9.0",
  "raw-window-handle 0.5.2",
 ]
 
 [[package]]
 name = "i-slint-backend-linuxkms"
 version = "1.6.0"
 dependencies = [
@@ -3526,15 +3549,15 @@
 name = "i-slint-backend-winit"
 version = "1.6.0"
 dependencies = [
  "accesskit",
  "accesskit_winit",
  "bytemuck",
  "cfg-if",
- "cfg_aliases 0.2.0",
+ "cfg_aliases 0.2.1",
  "cocoa",
  "const-field-offset",
  "copypasta",
  "derive_more",
  "glutin",
  "glutin-winit",
  "i-slint-common",
@@ -3654,15 +3677,15 @@
 ]
 
 [[package]]
 name = "i-slint-core-macros"
 version = "1.6.0"
 dependencies = [
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "i-slint-parser-test-macro"
 version = "1.6.0"
 dependencies = [
  "quote",
@@ -3701,15 +3724,15 @@
 [[package]]
 name = "i-slint-renderer-skia"
 version = "1.6.0"
 dependencies = [
  "ash",
  "bytemuck",
  "cfg-if",
- "cfg_aliases 0.2.0",
+ "cfg_aliases 0.2.1",
  "cocoa",
  "const-field-offset",
  "core-foundation",
  "core-graphics-types",
  "derive_more",
  "foreign-types 0.5.0",
  "glow",
@@ -4526,17 +4549,17 @@
 name = "mutex-trait"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4bb1638d419e12f8b1c43d9e639abd0d1424285bdea2f76aa231e233c63cd3a"
 
 [[package]]
 name = "napi"
-version = "2.16.4"
+version = "2.16.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da1edd9510299935e4f52a24d1e69ebd224157e3e962c6c847edec5c2e4f786f"
+checksum = "dfc300228808a0e6aea5a58115c82889240bcf8dab16fc25ad675b33e454b368"
 dependencies = [
  "bitflags 2.5.0",
  "ctor",
  "napi-derive",
  "napi-sys",
  "once_cell",
 ]
@@ -4545,39 +4568,39 @@
 name = "napi-build"
 version = "2.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1c0f5d67ee408a4685b61f5ab7e58605c8ae3f2b4189f0127d804ff13d5560a"
 
 [[package]]
 name = "napi-derive"
-version = "2.16.3"
+version = "2.16.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5a6de411b6217dbb47cd7a8c48684b162309ff48a77df9228c082400dd5b030"
+checksum = "4bb613535cde46cff231e53cd819c1694a32d48946bc2dda6b41174ace52ac08"
 dependencies = [
  "cfg-if",
  "convert_case 0.6.0",
  "napi-derive-backend",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "napi-derive-backend"
-version = "1.0.65"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3e35868d43b178b0eb9c17bd018960b1b5dd1732a7d47c23debe8f5c4caf498"
+checksum = "da041b19246ab4240998774e987fd9a7d92cc7406b91b5eddb6691e81feac044"
 dependencies = [
  "convert_case 0.6.0",
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
- "semver 1.0.22",
- "syn 2.0.60",
+ "semver 1.0.23",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "napi-sys"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "427802e8ec3a734331fec1035594a210ce1ff4dc5bc1950530920ab717964ea3"
@@ -4623,22 +4646,37 @@
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2076a31b7010b17a38c01907c45b945e8f11495ee4dd588309718901b1f7a5b7"
 dependencies = [
  "bitflags 2.5.0",
  "jni-sys",
  "log",
- "ndk-sys",
+ "ndk-sys 0.5.0+25.2.9519653",
  "num_enum 0.7.2",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.1",
  "thiserror",
 ]
 
 [[package]]
+name = "ndk"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3f42e7bbe13d351b6bead8286a43aac9534b82bd3cc43e47037f012ebfd62d4"
+dependencies = [
+ "bitflags 2.5.0",
+ "jni-sys",
+ "log",
+ "ndk-sys 0.6.0+11769913",
+ "num_enum 0.7.2",
+ "raw-window-handle 0.5.2",
+ "thiserror",
+]
+
+[[package]]
 name = "ndk-context"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "27b02d87554356db9e9a873add8782d4ea6e3e58ea071a9adb9a2e8ddb884a8b"
 
 [[package]]
 name = "ndk-sys"
@@ -4646,14 +4684,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c196769dd60fd4f363e11d948139556a344e79d451aeb2fa2fd040738ef7691"
 dependencies = [
  "jni-sys",
 ]
 
 [[package]]
+name = "ndk-sys"
+version = "0.6.0+11769913"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee6cda3051665f1fb8d9e08fc35c96d5a244fb1be711a03b71118828afc9a873"
+dependencies = [
+ "jni-sys",
+]
+
+[[package]]
 name = "nix"
 version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "598beaf3cc6fdd9a5dfb1630c2800c7acd31df7aaf0f565796fba2b53ca1af1b"
 dependencies = [
  "bitflags 1.3.2",
  "cfg-if",
@@ -4725,31 +4772,31 @@
 name = "num-derive"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed3955f1a9c7c0c15e092f9c887db08b1fc683305fdf6eb6684f22555355e202"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
@@ -4761,28 +4808,27 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -4828,15 +4874,15 @@
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
 dependencies = [
  "proc-macro-crate 3.1.0",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "objc"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "915b1b472bc21c53464d6c8461c9d3af805ba1ef837e1cac254428f4a77177b1"
@@ -4924,15 +4970,15 @@
 [[package]]
 name = "oboe"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8b61bebd49e5d43f5f8cc7ee2891c16e0f41ec7954d36bcb6c14c5e0de867fb"
 dependencies = [
  "jni",
- "ndk",
+ "ndk 0.8.0",
  "ndk-context",
  "num-derive",
  "num-traits",
  "oboe-sys",
 ]
 
 [[package]]
@@ -4993,15 +5039,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -5044,19 +5090,19 @@
 dependencies = [
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "owned_ttf_parser"
-version = "0.20.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4586edfe4c648c71797a74c84bacb32b52b212eff5dfe2bb9f2c599844023e7"
+checksum = "6b41438d2fc63c46c74a2203bf5ccd82c41ba04347b2fcf5754f230b167067d5"
 dependencies = [
- "ttf-parser 0.20.0",
+ "ttf-parser 0.21.1",
 ]
 
 [[package]]
 name = "panic-probe"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa6fa5645ef5a760cd340eaa92af9c1ce131c8c09e7f8926d8a24b59d26652b9"
@@ -5092,17 +5138,17 @@
  "redox_syscall 0.5.1",
  "smallvec",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "pathfinder_geometry"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b7e7b4ea703700ce73ebf128e1450eb69c3a8329199ffbfb9b2a0418e5ad3"
 dependencies = [
@@ -5150,15 +5196,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -5184,17 +5230,17 @@
  "arrayvec",
  "num_enum 0.5.11",
  "paste",
 ]
 
 [[package]]
 name = "piper"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "668d31b1c4eba19242f2088b2bf3316b82ca31082a8335764db4e083db7485d4"
+checksum = "464db0c665917b13ebb5d453ccdec4add5658ee1adc7affc7677615356a8afaf"
 dependencies = [
  "atomic-waker",
  "fastrand 2.1.0",
  "futures-io",
 ]
 
 [[package]]
@@ -5316,20 +5362,20 @@
 name = "pretty-hex"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbc83ee4a840062f368f9096d80077a9841ec117e17e7f700df81958f1451254"
 
 [[package]]
 name = "prettyplease"
-version = "0.2.19"
+version = "0.2.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ac2cf0f2e4f42b49f5ffd07dae8d746508ef7526c13940e5f524012ae6c6550"
+checksum = "5f12335488a2f3b0a83b14edad48dca9879ce89b2edd10e80237e4e852dd645e"
 dependencies = [
  "proc-macro2",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "printerdemo"
 version = "1.6.0"
 dependencies = [
  "chrono",
@@ -5408,17 +5454,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.2.0"
@@ -5484,28 +5530,28 @@
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "qoi"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f6d64c71eb498fe9eae14ce4ec935c555749aef511cca85b5568910d6e48001"
@@ -5517,15 +5563,15 @@
 name = "qttypes"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d405b0934e4176fb264d6ca597e5c8c2fba562fa155cba681ca160c1eb7edc6e"
 dependencies = [
  "cpp",
  "cpp_build",
- "semver 1.0.22",
+ "semver 1.0.23",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
@@ -5859,17 +5905,17 @@
  "cortex-m-rt",
  "critical-section",
  "vcell",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -5884,15 +5930,15 @@
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
- "semver 1.0.22",
+ "semver 1.0.23",
 ]
 
 [[package]]
 name = "rustix"
 version = "0.37.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea8ca367a3a01fe35e6943c400addf443c0f57670e6ec51196f71a4b8762dd2"
@@ -5939,34 +5985,34 @@
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
  "base64 0.21.7",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.5.0"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "beb461507cee2c2ff151784c52762cf4d9ff6a61f3e80968600ed24fa837fa54"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.102.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.15"
+version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
+checksum = "092474d1a01ea8278f69e6a358998405fae5b8b963ddaeb2b0b04a128bf1dfb0"
 
 [[package]]
 name = "rustybuzz"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88117946aa1bfb53c2ae0643ceac6506337f44887f8c9fbfb43587b1cc52ba49"
 dependencies = [
@@ -5978,17 +6024,17 @@
  "unicode-ccc",
  "unicode-properties",
  "unicode-script",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -6033,30 +6079,30 @@
  "memmap2 0.9.4",
  "smithay-client-toolkit",
  "tiny-skia",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
+checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
@@ -6065,17 +6111,17 @@
 checksum = "1d7eb9ef2c18661902cc47e535f9bc51b78acd254da71d375c2f6720d9a40403"
 dependencies = [
  "semver-parser",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+checksum = "61697e0a1c7e512e84a621326239844a24d8207b4669b41bc18b32ea5cbf988b"
 
 [[package]]
 name = "semver-parser"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388a1df253eca08550bef6c72392cfe7c30914bf41df5269b68cbd6ff8f570a3"
 
@@ -6083,17 +6129,17 @@
 name = "send_wrapper"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd0b0ec5f1c1ca621c432a25813d8d60c88abe6d3e08a3eb9cf37d97a0fe3d73"
 
 [[package]]
 name = "serde"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
+checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.6.5"
@@ -6103,43 +6149,43 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.200"
+version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
+checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_repr"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "serde_spanned"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
@@ -6521,15 +6567,15 @@
 name = "smart-default"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0eb01866308440fc64d6c44d9e86c5cc17adfe33c4d6eed55da9145044d0ffc1"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "smithay-client-toolkit"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "922fd3eeab3bd820d76537ce8f582b1cf951eceb5475c28500c7457d9d17f53a"
@@ -6736,20 +6782,14 @@
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
-name = "strsim"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
-
-[[package]]
 name = "strum"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "063e6045c0e62079840579a7e47a355ae92f60eb74daaf156fb1e84ba164e63f"
 
 [[package]]
 name = "strum"
@@ -6788,41 +6828,41 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "strum_macros"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "svgtypes"
-version = "0.15.0"
+version = "0.15.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d97ca9a891c9c70da8139ac9d8e8ea36a210fa21bb50eccd75d4a9561c83e87f"
+checksum = "fae3064df9b89391c9a76a0425a69d124aee9c5c28455204709e72c39868a43c"
 dependencies = [
  "kurbo",
  "siphasher",
 ]
 
 [[package]]
 name = "syn"
@@ -6833,17 +6873,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.60"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -7015,30 +7055,30 @@
 name = "text-size"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f18aa187839b2bdb1ad2fa35ead8c4c2976b64e4363c386d45ac0f7ee85c9233"
 
 [[package]]
 name = "thiserror"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
+checksum = "579e9083ca58dd9dcf91a9923bb9054071b9ebbd800b342194c9feb0ee89fc18"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
+checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
@@ -7147,39 +7187,38 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
 dependencies = [
  "native-tls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "toml"
 version = "0.5.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
@@ -7247,15 +7286,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
 dependencies = [
  "indexmap 2.2.6",
  "serde",
  "serde_spanned",
  "toml_datetime",
- "winnow 0.6.7",
+ "winnow 0.6.8",
 ]
 
 [[package]]
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
@@ -7275,15 +7314,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -7316,14 +7355,20 @@
 [[package]]
 name = "ttf-parser"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17f77d76d837a7830fe1d4f12b7b4ba4192c1888001c7164257e4bc6d21d96b4"
 
 [[package]]
+name = "ttf-parser"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c591d83f69777866b9126b24c6dd9a18351f177e49d625920d19f989fd31cf8"
+
+[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "ucs2"
@@ -7623,15 +7668,15 @@
 
 [[package]]
 name = "vtable-macro"
 version = "0.2.0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
  "vtable",
 ]
 
 [[package]]
 name = "vulkano"
 version = "0.34.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -7658,17 +7703,17 @@
  "smallvec",
  "thread_local",
  "vk-parse",
 ]
 
 [[package]]
 name = "waker-fn"
-version = "1.1.1"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3c4517f54858c779bbcbf228f4fca63d121bf85fbecb2dc578cdf4a39395690"
+checksum = "317211a0dc0ceedd78fb2ca9a44aed3d7b9b26f81870d485c07122b4350673b7"
 
 [[package]]
 name = "walkdir"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
@@ -7708,15 +7753,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -7742,15 +7787,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -8036,26 +8081,26 @@
 name = "windows-implement"
 version = "0.53.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "942ac266be9249c84ca862f0a164a39533dc2f6f33dc98ec89c8da99b82ea0bd"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "windows-interface"
 version = "0.53.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da33557140a288fae4e1d5f8873aaf9eb6613a9cf82c3e070223ff177f598b60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "windows-result"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "749f0da9cc72d82e600d8d2e44cadd0b9eedb9038f71a1c58556ac1c5791813b"
@@ -8271,30 +8316,30 @@
 [[package]]
 name = "winit"
 version = "0.29.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d59ad965a635657faf09c8f062badd885748428933dad8e8bdd64064d92e5ca"
 dependencies = [
  "ahash",
- "android-activity",
+ "android-activity 0.5.2",
  "atomic-waker",
  "bitflags 2.5.0",
  "bytemuck",
  "calloop",
  "cfg_aliases 0.1.1",
  "core-foundation",
  "core-graphics 0.23.2",
  "cursor-icon",
  "icrate 0.0.4",
  "js-sys",
  "libc",
  "log",
  "memmap2 0.9.4",
- "ndk",
- "ndk-sys",
+ "ndk 0.8.0",
+ "ndk-sys 0.5.0+25.2.9519653",
  "objc2 0.4.1",
  "once_cell",
  "orbclient",
  "percent-encoding",
  "raw-window-handle 0.5.2",
  "raw-window-handle 0.6.1",
  "redox_syscall 0.3.5",
@@ -8324,17 +8369,17 @@
 checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.6.7"
+version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14b9415ee827af173ebb3f15f9083df5a122eb93572ec28741fb153356ea2578"
+checksum = "c3c52e9c97a68071b23e836c9380edae937f17b9c4667bd021973efc689f618d"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
@@ -8565,15 +8610,15 @@
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "082cdede098bbec9af15b0e74085e5f3d16f2923597de7aed7b8112003af2da7"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "yeslogic-fontconfig-sys"
 version = "3.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f2bbd69036d397ebbff671b1b8e4d918610c181c5a16073b96f984a38d08c386"
@@ -8648,30 +8693,30 @@
  "serde",
  "static_assertions",
  "zvariant",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.60",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "zeroize"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
```

### Comparing `slint-1.6.0a7/Cargo.toml` & `slint-1.6.0a8/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 i-slint-core = { version = "=1.6.0", path = "internal/core", default-features = false }
 i-slint-core-macros = { version = "=1.6.0", path = "internal/core-macros", default-features = false }
 i-slint-renderer-femtovg = { version = "=1.6.0", path = "internal/renderers/femtovg", default-features = false }
 i-slint-renderer-skia = { version = "=1.6.0", path = "internal/renderers/skia", default-features = false }
 slint = { version = "=1.6.0", path = "api/rs/slint", default-features = false }
 slint-build = { version = "=1.6.0", path = "api/rs/build", default-features = false }
 slint-cpp = { version = "=1.6.0", path = "api/cpp", default-features = false }
-slint-interpreter = { version = "=1.6.0", path = "internal/interpreter", default_features = false }
+slint-interpreter = { version = "=1.6.0", path = "internal/interpreter", default-features = false }
 slint-macros = { version = "=1.6.0", path = "api/rs/macros", default-features = false }
 
 vtable = { version = "0.2", path = "helper_crates/vtable", default-features = false }
 
 bytemuck = { version = "1.13.1" }
 cbindgen = { version = "0.26", default-features = false }
 css-color-parser2 = { version = "1.0.1" }
```

### Comparing `slint-1.6.0a7/pyproject.toml` & `slint-1.6.0a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["maturin>=1,<2"]
 build-backend = "maturin"
 
 [project]
 name = "slint"
-version = "1.6.0a7"
+version = "1.6.0a8"
 requires-python = ">= 3.10"
 authors = [
     {name = "Slint Team", email = "info@slint.dev"},
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: MacOS X",
```

### Comparing `slint-1.6.0a7/slint/__init__.py` & `slint-1.6.0a8/slint/__init__.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/slint/models.py` & `slint-1.6.0a8/slint/models.py`

 * *Files identical despite different names*

### Comparing `slint-1.6.0a7/PKG-INFO` & `slint-1.6.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: slint
-Version: 1.6.0a7
+Version: 1.6.0a8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: MacOS X
 Classifier: Environment :: X11 Applications
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
```

