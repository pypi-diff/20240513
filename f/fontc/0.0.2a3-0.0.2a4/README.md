# Comparing `tmp/fontc-0.0.2a3.tar.gz` & `tmp/fontc-0.0.2a4.tar.gz`

## Comparing `fontc-0.0.2a3.tar` & `fontc-0.0.2a4.tar`

### file list

```diff
@@ -1,172 +1,172 @@
--rw-r--r--   0      501       20      854 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs2fontir/Cargo.toml
--rw-r--r--   0      501       20      184 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs2fontir/README.md
--rw-r--r--   0      501       20       26 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs2fontir/src/lib.rs
--rw-r--r--   0      501       20    57821 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs2fontir/src/source.rs
--rw-r--r--   0      501       20    12432 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs2fontir/src/toir.rs
--rw-r--r--   0      501       20      346 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/plist_derive/Cargo.toml
--rw-r--r--   0      501       20     2382 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/plist_derive/src/attrs.rs
--rw-r--r--   0      501       20     3109 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/plist_derive/src/lib.rs
--rw-r--r--   0      501       20      561 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/Cargo.toml
--rw-r--r--   0      501       20      452 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/README.md
--rw-r--r--   0      501       20     2688 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/build.rs
--rw-r--r--   0      501       20    27655 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/data/aglfn.txt
--rw-r--r--   0      501       20    78060 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/data/glyphlist.txt
--rw-r--r--   0      501       20     6710 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/src/agl.rs
--rw-r--r--   0      501       20    19926 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/src/coords.rs
--rw-r--r--   0      501       20      188 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/src/lib.rs
--rw-r--r--   0      501       20     9962 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/src/orchestration.rs
--rw-r--r--   0      501       20     6769 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/src/paths.rs
--rw-r--r--   0      501       20     4727 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/src/piecewise_linear_map.rs
--rw-r--r--   0      501       20     1993 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontdrasil/src/types.rs
--rw-r--r--   0      501       20      946 2024-05-13 12:58:10.000000 fontc-0.0.2a3/ufo2fontir/Cargo.toml
--rw-r--r--   0      501       20      188 2024-05-13 12:58:10.000000 fontc-0.0.2a3/ufo2fontir/README.md
--rw-r--r--   0      501       20       30 2024-05-13 12:58:10.000000 fontc-0.0.2a3/ufo2fontir/src/lib.rs
--rw-r--r--   0      501       20    81135 2024-05-13 12:58:10.000000 fontc-0.0.2a3/ufo2fontir/src/source.rs
--rw-r--r--   0      501       20    10780 2024-05-13 12:58:10.000000 fontc-0.0.2a3/ufo2fontir/src/toir.rs
--rw-r--r--   0      501       20     1295 2024-05-13 12:58:10.000000 fontc-0.0.2a3/ufo2fontir/testdata/wght_var.designspace
--rw-r--r--   0      501       20     1413 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/Cargo.toml
--rw-r--r--   0      501       20     5219 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/README.md
--rw-r--r--   0      501       20     1036 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/benches/parsing.rs
--rw-r--r--   0      501       20     6563 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/bin/compile.rs
--rw-r--r--   0      501       20     1598 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/bin/highlight.rs
--rw-r--r--   0      501       20     3559 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/bin/parse_test.rs
--rw-r--r--   0      501       20     2427 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/bin/ttx_test.rs
--rw-r--r--   0      501       20     3741 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/common/glyph_class.rs
--rw-r--r--   0      501       20     5732 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/common/glyph_map.rs
--rw-r--r--   0      501       20     3246 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/common.rs
--rw-r--r--   0      501       20    88121 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/compile_ctx.rs
--rw-r--r--   0      501       20     6792 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/compiler.rs
--rw-r--r--   0      501       20     2204 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/error.rs
--rw-r--r--   0      501       20     5683 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/feature_writer.rs
--rw-r--r--   0      501       20    24755 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/features.rs
--rw-r--r--   0      501       20     8873 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/glyph_range.rs
--rw-r--r--   0      501       20     1887 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/language_system.rs
--rw-r--r--   0      501       20    26387 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/lookups/contextual.rs
--rw-r--r--   0      501       20    22671 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/lookups/gpos_builders.rs
--rw-r--r--   0      501       20     8415 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/lookups/gsub_builders.rs
--rw-r--r--   0      501       20     4720 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/lookups/helpers.rs
--rw-r--r--   0      501       20    42617 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/lookups.rs
--rw-r--r--   0      501       20    12476 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/metrics.rs
--rw-r--r--   0      501       20     3285 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/opts.rs
--rw-r--r--   0      501       20     3725 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/output.rs
--rw-r--r--   0      501       20     2189 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/tables/base.rs
--rw-r--r--   0      501       20     5298 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/tables/gdef.rs
--rw-r--r--   0      501       20     5532 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/tables/name.rs
--rw-r--r--   0      501       20     4113 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/tables/os2.rs
--rw-r--r--   0      501       20     5347 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/tables/stat.rs
--rw-r--r--   0      501       20     2789 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/tables.rs
--rw-r--r--   0      501       20     2031 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/tags.rs
--rw-r--r--   0      501       20    58287 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/validate.rs
--rw-r--r--   0      501       20     8061 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile/variations.rs
--rw-r--r--   0      501       20     5244 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/compile.rs
--rw-r--r--   0      501       20     5999 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/diagnostic.rs
--rw-r--r--   0      501       20      624 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/lib.rs
--rw-r--r--   0      501       20    16381 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/context.rs
--rw-r--r--   0      501       20    10160 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/grammar/feature.rs
--rw-r--r--   0      501       20     9162 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/grammar/glyph.rs
--rw-r--r--   0      501       20     8103 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/grammar/gpos.rs
--rw-r--r--   0      501       20     7824 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/grammar/gsub.rs
--rw-r--r--   0      501       20    11835 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/grammar/metrics.rs
--rw-r--r--   0      501       20    11841 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/grammar/mod.rs
--rw-r--r--   0      501       20    19662 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/grammar/table.rs
--rw-r--r--   0      501       20     3307 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/grammar/variations.rs
--rw-r--r--   0      501       20    25328 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/lexer/lexeme.rs
--rw-r--r--   0      501       20     6748 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/lexer/token_set.rs
--rw-r--r--   0      501       20    13214 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/lexer.rs
--rw-r--r--   0      501       20    13148 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/parser.rs
--rw-r--r--   0      501       20    12900 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/source.rs
--rw-r--r--   0      501       20     1741 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse/tree.rs
--rw-r--r--   0      501       20     3528 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/parse.rs
--rw-r--r--   0      501       20     4712 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/tests/compile.rs
--rw-r--r--   0      501       20     4164 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/tests/parse.rs
--rw-r--r--   0      501       20       52 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/tests.rs
--rw-r--r--   0      501       20     8618 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/token_tree/cursor.rs
--rw-r--r--   0      501       20     4704 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/token_tree/edit.rs
--rw-r--r--   0      501       20    11526 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/token_tree/rewrite.rs
--rw-r--r--   0      501       20     2017 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/token_tree/stack.rs
--rw-r--r--   0      501       20    22316 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/token_tree/token.rs
--rw-r--r--   0      501       20    47941 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/token_tree/typed.rs
--rw-r--r--   0      501       20    20795 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/token_tree.rs
--rw-r--r--   0      501       20     7594 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/util/highlighting.rs
--rw-r--r--   0      501       20     3851 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/util/paths.rs
--rw-r--r--   0      501       20     8008 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/util/pretty_diff.rs
--rw-r--r--   0      501       20    26284 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/util/ttx.rs
--rw-r--r--   0      501       20      737 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fea-rs/src/util.rs
--rw-r--r--   0      501       20     1053 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/Cargo.toml
--rw-r--r--   0      501       20      271 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/README.md
--rw-r--r--   0      501       20     7181 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/avar.rs
--rw-r--r--   0      501       20     1813 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/cmap.rs
--rw-r--r--   0      501       20     4205 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/error.rs
--rw-r--r--   0      501       20    47130 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/features/kern.rs
--rw-r--r--   0      501       20    16093 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/features/marks.rs
--rw-r--r--   0      501       20     5050 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/features/ot_tags.rs
--rw-r--r--   0      501       20    11877 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/features/properties.rs
--rw-r--r--   0      501       20    23190 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/features.rs
--rw-r--r--   0      501       20     6620 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/font.rs
--rw-r--r--   0      501       20     4831 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/fvar.rs
--rw-r--r--   0      501       20    37227 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/glyphs.rs
--rw-r--r--   0      501       20     3586 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/gvar.rs
--rw-r--r--   0      501       20     7317 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/head.rs
--rw-r--r--   0      501       20     9069 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/hvar.rs
--rw-r--r--   0      501       20      310 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/lib.rs
--rw-r--r--   0      501       20    14201 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/metrics_and_limits.rs
--rw-r--r--   0      501       20    11306 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/mvar.rs
--rw-r--r--   0      501       20     1477 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/name.rs
--rw-r--r--   0      501       20    32165 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/orchestration.rs
--rw-r--r--   0      501       20    34761 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/os2.rs
--rw-r--r--   0      501       20     3776 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/paths.rs
--rw-r--r--   0      501       20     2011 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/post.rs
--rw-r--r--   0      501       20     2435 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/stat.rs
--rw-r--r--   0      501       20      930 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontbe/src/test_util.rs
--rw-r--r--   0      501       20      810 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontra2fontir/Cargo.toml
--rw-r--r--   0      501       20      207 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontra2fontir/README.md
--rw-r--r--   0      501       20    15733 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontra2fontir/src/fontra.rs
--rw-r--r--   0      501       20      325 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontra2fontir/src/lib.rs
--rw-r--r--   0      501       20    10816 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontra2fontir/src/source.rs
--rw-r--r--   0      501       20    10630 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontra2fontir/src/toir.rs
--rw-r--r--   0      501       20      869 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/Cargo.toml
--rw-r--r--   0      501       20      417 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/README.md
--rw-r--r--   0      501       20     1056 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/build.rs
--rw-r--r--   0      501       20  5067653 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/data/GlyphData.xml
--rw-r--r--   0      501       20  2926546 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/data/GlyphData_Ideographs.xml
--rw-r--r--   0      501       20      947 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/data/GlyphData_override_test.xml
--rw-r--r--   0      501       20      380 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/data/README.md
--rw-r--r--   0      501       20       81 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/data/VERSION
--rw-r--r--   0      501       20     1212 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/data/update.py
--rw-r--r--   0      501       20      821 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/src/error.rs
--rw-r--r--   0      501       20    98609 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/src/font.rs
--rw-r--r--   0      501       20    10744 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/src/glyphdata/glyphdata_impl.rs
--rw-r--r--   0      501       20    19710 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/src/glyphdata.rs
--rw-r--r--   0      501       20      304 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/src/lib.rs
--rw-r--r--   0      501       20    24558 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/src/plist.rs
--rw-r--r--   0      501       20    32909 2024-05-13 12:58:09.000000 fontc-0.0.2a3/glyphs-reader/src/propagate_anchors.rs
--rw-r--r--   0      501       20      949 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/Cargo.toml
--rw-r--r--   0      501       20      334 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/README.md
--rw-r--r--   0      501       20     7704 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/error.rs
--rw-r--r--   0      501       20    31884 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/glyph.rs
--rw-r--r--   0      501       20    81151 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/ir.rs
--rw-r--r--   0      501       20      156 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/lib.rs
--rw-r--r--   0      501       20    15993 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/orchestration.rs
--rw-r--r--   0      501       20     2617 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/paths.rs
--rw-r--r--   0      501       20     3426 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/serde.rs
--rw-r--r--   0      501       20     5978 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/source.rs
--rw-r--r--   0      501       20    13439 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/stateset.rs
--rw-r--r--   0      501       20    50736 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontir/src/variations.rs
--rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 fontc-0.0.2a3/fontc/Cargo.toml
--rw-r--r--   0      501       20      348 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/README.md
--rw-r--r--   0      501       20      278 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/build.rs
--rw-r--r--   0      501       20     7761 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/args.rs
--rw-r--r--   0      501       20    12794 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/change_detector.rs
--rw-r--r--   0      501       20     4073 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/config.rs
--rw-r--r--   0      501       20      722 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/error.rs
--rw-r--r--   0      501       20   101138 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/lib.rs
--rw-r--r--   0      501       20     3832 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/main.rs
--rw-r--r--   0      501       20    10457 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/timing.rs
--rw-r--r--   0      501       20     7305 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/work.rs
--rw-r--r--   0      501       20    33415 2024-05-13 12:58:09.000000 fontc-0.0.2a3/fontc/src/workload.rs
--rw-r--r--   0      501       20    60506 2024-05-13 12:59:01.000000 fontc-0.0.2a3/Cargo.lock
--rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 fontc-0.0.2a3/Cargo.toml
--rw-r--r--   0      501       20     1251 2024-05-13 12:58:09.000000 fontc-0.0.2a3/pyproject.toml
--rw-r--r--   0      501       20     7765 2024-05-13 12:58:09.000000 fontc-0.0.2a3/README.md
--rw-r--r--   0      501       20    11357 2024-05-13 12:58:09.000000 fontc-0.0.2a3/LICENSE
--rw-r--r--   0        0        0     8026 1970-01-01 00:00:00.000000 fontc-0.0.2a3/PKG-INFO
+-rw-r--r--   0      501       20     1413 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/Cargo.toml
+-rw-r--r--   0      501       20     5219 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/README.md
+-rw-r--r--   0      501       20     1036 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/benches/parsing.rs
+-rw-r--r--   0      501       20     6563 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/bin/compile.rs
+-rw-r--r--   0      501       20     1598 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/bin/highlight.rs
+-rw-r--r--   0      501       20     3559 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/bin/parse_test.rs
+-rw-r--r--   0      501       20     2427 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/bin/ttx_test.rs
+-rw-r--r--   0      501       20     3741 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/common/glyph_class.rs
+-rw-r--r--   0      501       20     5732 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/common/glyph_map.rs
+-rw-r--r--   0      501       20     3246 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/common.rs
+-rw-r--r--   0      501       20    88121 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/compile_ctx.rs
+-rw-r--r--   0      501       20     6792 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/compiler.rs
+-rw-r--r--   0      501       20     2204 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/error.rs
+-rw-r--r--   0      501       20     5683 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/feature_writer.rs
+-rw-r--r--   0      501       20    24755 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/features.rs
+-rw-r--r--   0      501       20     8873 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/glyph_range.rs
+-rw-r--r--   0      501       20     1887 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/language_system.rs
+-rw-r--r--   0      501       20    26387 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/lookups/contextual.rs
+-rw-r--r--   0      501       20    22671 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/lookups/gpos_builders.rs
+-rw-r--r--   0      501       20     8415 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/lookups/gsub_builders.rs
+-rw-r--r--   0      501       20     4720 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/lookups/helpers.rs
+-rw-r--r--   0      501       20    42617 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/lookups.rs
+-rw-r--r--   0      501       20    12476 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/metrics.rs
+-rw-r--r--   0      501       20     3285 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/opts.rs
+-rw-r--r--   0      501       20     3725 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/output.rs
+-rw-r--r--   0      501       20     2189 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/tables/base.rs
+-rw-r--r--   0      501       20     5298 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/tables/gdef.rs
+-rw-r--r--   0      501       20     5532 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/tables/name.rs
+-rw-r--r--   0      501       20     4113 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/tables/os2.rs
+-rw-r--r--   0      501       20     5347 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/tables/stat.rs
+-rw-r--r--   0      501       20     2789 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/tables.rs
+-rw-r--r--   0      501       20     2031 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/tags.rs
+-rw-r--r--   0      501       20    58287 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/validate.rs
+-rw-r--r--   0      501       20     8061 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile/variations.rs
+-rw-r--r--   0      501       20     5244 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/compile.rs
+-rw-r--r--   0      501       20     5999 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/diagnostic.rs
+-rw-r--r--   0      501       20      624 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/lib.rs
+-rw-r--r--   0      501       20    16381 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/context.rs
+-rw-r--r--   0      501       20    10160 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/grammar/feature.rs
+-rw-r--r--   0      501       20     9162 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/grammar/glyph.rs
+-rw-r--r--   0      501       20     8103 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/grammar/gpos.rs
+-rw-r--r--   0      501       20     7824 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/grammar/gsub.rs
+-rw-r--r--   0      501       20    11835 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/grammar/metrics.rs
+-rw-r--r--   0      501       20    11841 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/grammar/mod.rs
+-rw-r--r--   0      501       20    19662 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/grammar/table.rs
+-rw-r--r--   0      501       20     3307 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/grammar/variations.rs
+-rw-r--r--   0      501       20    25328 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/lexer/lexeme.rs
+-rw-r--r--   0      501       20     6748 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/lexer/token_set.rs
+-rw-r--r--   0      501       20    13214 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/lexer.rs
+-rw-r--r--   0      501       20    13148 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/parser.rs
+-rw-r--r--   0      501       20    12900 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/source.rs
+-rw-r--r--   0      501       20     1741 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse/tree.rs
+-rw-r--r--   0      501       20     3528 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/parse.rs
+-rw-r--r--   0      501       20     4712 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/tests/compile.rs
+-rw-r--r--   0      501       20     4164 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/tests/parse.rs
+-rw-r--r--   0      501       20       52 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/tests.rs
+-rw-r--r--   0      501       20     8618 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/token_tree/cursor.rs
+-rw-r--r--   0      501       20     4704 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/token_tree/edit.rs
+-rw-r--r--   0      501       20    11526 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/token_tree/rewrite.rs
+-rw-r--r--   0      501       20     2017 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/token_tree/stack.rs
+-rw-r--r--   0      501       20    22316 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/token_tree/token.rs
+-rw-r--r--   0      501       20    47941 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/token_tree/typed.rs
+-rw-r--r--   0      501       20    20795 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/token_tree.rs
+-rw-r--r--   0      501       20     7594 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/util/highlighting.rs
+-rw-r--r--   0      501       20     3851 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/util/paths.rs
+-rw-r--r--   0      501       20     8008 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/util/pretty_diff.rs
+-rw-r--r--   0      501       20    26284 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/util/ttx.rs
+-rw-r--r--   0      501       20      737 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fea-rs/src/util.rs
+-rw-r--r--   0      501       20      346 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/plist_derive/Cargo.toml
+-rw-r--r--   0      501       20     2382 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/plist_derive/src/attrs.rs
+-rw-r--r--   0      501       20     3109 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/plist_derive/src/lib.rs
+-rw-r--r--   0      501       20      946 2024-05-13 13:16:50.000000 fontc-0.0.2a4/ufo2fontir/Cargo.toml
+-rw-r--r--   0      501       20      188 2024-05-13 13:16:50.000000 fontc-0.0.2a4/ufo2fontir/README.md
+-rw-r--r--   0      501       20       30 2024-05-13 13:16:50.000000 fontc-0.0.2a4/ufo2fontir/src/lib.rs
+-rw-r--r--   0      501       20    81135 2024-05-13 13:16:50.000000 fontc-0.0.2a4/ufo2fontir/src/source.rs
+-rw-r--r--   0      501       20    10780 2024-05-13 13:16:50.000000 fontc-0.0.2a4/ufo2fontir/src/toir.rs
+-rw-r--r--   0      501       20     1295 2024-05-13 13:16:50.000000 fontc-0.0.2a4/ufo2fontir/testdata/wght_var.designspace
+-rw-r--r--   0      501       20      854 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs2fontir/Cargo.toml
+-rw-r--r--   0      501       20      184 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs2fontir/README.md
+-rw-r--r--   0      501       20       26 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs2fontir/src/lib.rs
+-rw-r--r--   0      501       20    57821 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs2fontir/src/source.rs
+-rw-r--r--   0      501       20    12432 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs2fontir/src/toir.rs
+-rw-r--r--   0      501       20      949 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/Cargo.toml
+-rw-r--r--   0      501       20      334 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/README.md
+-rw-r--r--   0      501       20     7704 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/error.rs
+-rw-r--r--   0      501       20    31884 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/glyph.rs
+-rw-r--r--   0      501       20    81151 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/ir.rs
+-rw-r--r--   0      501       20      156 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/lib.rs
+-rw-r--r--   0      501       20    15993 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/orchestration.rs
+-rw-r--r--   0      501       20     2617 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/paths.rs
+-rw-r--r--   0      501       20     3426 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/serde.rs
+-rw-r--r--   0      501       20     5978 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/source.rs
+-rw-r--r--   0      501       20    13439 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/stateset.rs
+-rw-r--r--   0      501       20    50736 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontir/src/variations.rs
+-rw-r--r--   0      501       20      810 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontra2fontir/Cargo.toml
+-rw-r--r--   0      501       20      207 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontra2fontir/README.md
+-rw-r--r--   0      501       20    15733 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontra2fontir/src/fontra.rs
+-rw-r--r--   0      501       20      325 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontra2fontir/src/lib.rs
+-rw-r--r--   0      501       20    10816 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontra2fontir/src/source.rs
+-rw-r--r--   0      501       20    10630 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontra2fontir/src/toir.rs
+-rw-r--r--   0      501       20      869 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/Cargo.toml
+-rw-r--r--   0      501       20      417 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/README.md
+-rw-r--r--   0      501       20     1056 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/build.rs
+-rw-r--r--   0      501       20  5067653 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/data/GlyphData.xml
+-rw-r--r--   0      501       20  2926546 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/data/GlyphData_Ideographs.xml
+-rw-r--r--   0      501       20      947 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/data/GlyphData_override_test.xml
+-rw-r--r--   0      501       20      380 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/data/README.md
+-rw-r--r--   0      501       20       81 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/data/VERSION
+-rw-r--r--   0      501       20     1212 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/data/update.py
+-rw-r--r--   0      501       20      821 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/src/error.rs
+-rw-r--r--   0      501       20    98609 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/src/font.rs
+-rw-r--r--   0      501       20    10744 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/src/glyphdata/glyphdata_impl.rs
+-rw-r--r--   0      501       20    19710 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/src/glyphdata.rs
+-rw-r--r--   0      501       20      304 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/src/lib.rs
+-rw-r--r--   0      501       20    24558 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/src/plist.rs
+-rw-r--r--   0      501       20    32909 2024-05-13 13:16:50.000000 fontc-0.0.2a4/glyphs-reader/src/propagate_anchors.rs
+-rw-r--r--   0      501       20      561 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/Cargo.toml
+-rw-r--r--   0      501       20      452 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/README.md
+-rw-r--r--   0      501       20     2688 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/build.rs
+-rw-r--r--   0      501       20    27655 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/data/aglfn.txt
+-rw-r--r--   0      501       20    78060 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/data/glyphlist.txt
+-rw-r--r--   0      501       20     6710 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/src/agl.rs
+-rw-r--r--   0      501       20    19926 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/src/coords.rs
+-rw-r--r--   0      501       20      188 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/src/lib.rs
+-rw-r--r--   0      501       20     9962 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/src/orchestration.rs
+-rw-r--r--   0      501       20     6769 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/src/paths.rs
+-rw-r--r--   0      501       20     4727 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/src/piecewise_linear_map.rs
+-rw-r--r--   0      501       20     1993 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontdrasil/src/types.rs
+-rw-r--r--   0      501       20     1053 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/Cargo.toml
+-rw-r--r--   0      501       20      271 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/README.md
+-rw-r--r--   0      501       20     7181 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/avar.rs
+-rw-r--r--   0      501       20     1813 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/cmap.rs
+-rw-r--r--   0      501       20     4205 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/error.rs
+-rw-r--r--   0      501       20    47130 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/features/kern.rs
+-rw-r--r--   0      501       20    16093 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/features/marks.rs
+-rw-r--r--   0      501       20     5050 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/features/ot_tags.rs
+-rw-r--r--   0      501       20    11877 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/features/properties.rs
+-rw-r--r--   0      501       20    23190 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/features.rs
+-rw-r--r--   0      501       20     6620 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/font.rs
+-rw-r--r--   0      501       20     4831 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/fvar.rs
+-rw-r--r--   0      501       20    37227 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/glyphs.rs
+-rw-r--r--   0      501       20     3586 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/gvar.rs
+-rw-r--r--   0      501       20     7317 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/head.rs
+-rw-r--r--   0      501       20     9069 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/hvar.rs
+-rw-r--r--   0      501       20      310 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/lib.rs
+-rw-r--r--   0      501       20    14201 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/metrics_and_limits.rs
+-rw-r--r--   0      501       20    11306 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/mvar.rs
+-rw-r--r--   0      501       20     1477 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/name.rs
+-rw-r--r--   0      501       20    32165 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/orchestration.rs
+-rw-r--r--   0      501       20    34761 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/os2.rs
+-rw-r--r--   0      501       20     3776 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/paths.rs
+-rw-r--r--   0      501       20     2011 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/post.rs
+-rw-r--r--   0      501       20     2435 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/stat.rs
+-rw-r--r--   0      501       20      930 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontbe/src/test_util.rs
+-rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 fontc-0.0.2a4/fontc/Cargo.toml
+-rw-r--r--   0      501       20      348 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/README.md
+-rw-r--r--   0      501       20      278 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/build.rs
+-rw-r--r--   0      501       20     7761 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/args.rs
+-rw-r--r--   0      501       20    12794 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/change_detector.rs
+-rw-r--r--   0      501       20     4073 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/config.rs
+-rw-r--r--   0      501       20      722 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/error.rs
+-rw-r--r--   0      501       20   101138 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/lib.rs
+-rw-r--r--   0      501       20     3832 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/main.rs
+-rw-r--r--   0      501       20    10457 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/timing.rs
+-rw-r--r--   0      501       20     7305 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/work.rs
+-rw-r--r--   0      501       20    33415 2024-05-13 13:16:50.000000 fontc-0.0.2a4/fontc/src/workload.rs
+-rw-r--r--   0      501       20    60506 2024-05-13 13:20:36.000000 fontc-0.0.2a4/Cargo.lock
+-rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 fontc-0.0.2a4/Cargo.toml
+-rw-r--r--   0      501       20     1251 2024-05-13 13:16:50.000000 fontc-0.0.2a4/pyproject.toml
+-rw-r--r--   0      501       20     7765 2024-05-13 13:16:50.000000 fontc-0.0.2a4/README.md
+-rw-r--r--   0      501       20    11357 2024-05-13 13:16:50.000000 fontc-0.0.2a4/LICENSE
+-rw-r--r--   0        0        0     8026 1970-01-01 00:00:00.000000 fontc-0.0.2a4/PKG-INFO
```

### Comparing `fontc-0.0.2a3/glyphs2fontir/Cargo.toml` & `fontc-0.0.2a4/glyphs2fontir/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs2fontir/src/source.rs` & `fontc-0.0.2a4/glyphs2fontir/src/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs2fontir/src/toir.rs` & `fontc-0.0.2a4/glyphs2fontir/src/toir.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/plist_derive/src/attrs.rs` & `fontc-0.0.2a4/glyphs-reader/plist_derive/src/attrs.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/plist_derive/src/lib.rs` & `fontc-0.0.2a4/glyphs-reader/plist_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/Cargo.toml` & `fontc-0.0.2a4/fontdrasil/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/build.rs` & `fontc-0.0.2a4/fontdrasil/build.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/data/aglfn.txt` & `fontc-0.0.2a4/fontdrasil/data/aglfn.txt`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/data/glyphlist.txt` & `fontc-0.0.2a4/fontdrasil/data/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/src/agl.rs` & `fontc-0.0.2a4/fontdrasil/src/agl.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/src/coords.rs` & `fontc-0.0.2a4/fontdrasil/src/coords.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/src/orchestration.rs` & `fontc-0.0.2a4/fontdrasil/src/orchestration.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/src/paths.rs` & `fontc-0.0.2a4/fontdrasil/src/paths.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/src/piecewise_linear_map.rs` & `fontc-0.0.2a4/fontdrasil/src/piecewise_linear_map.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontdrasil/src/types.rs` & `fontc-0.0.2a4/fontdrasil/src/types.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/ufo2fontir/Cargo.toml` & `fontc-0.0.2a4/ufo2fontir/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/ufo2fontir/src/source.rs` & `fontc-0.0.2a4/ufo2fontir/src/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/ufo2fontir/src/toir.rs` & `fontc-0.0.2a4/ufo2fontir/src/toir.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/ufo2fontir/testdata/wght_var.designspace` & `fontc-0.0.2a4/ufo2fontir/testdata/wght_var.designspace`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/Cargo.toml` & `fontc-0.0.2a4/fea-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/README.md` & `fontc-0.0.2a4/fea-rs/README.md`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/benches/parsing.rs` & `fontc-0.0.2a4/fea-rs/benches/parsing.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/bin/compile.rs` & `fontc-0.0.2a4/fea-rs/src/bin/compile.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/bin/highlight.rs` & `fontc-0.0.2a4/fea-rs/src/bin/highlight.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/bin/parse_test.rs` & `fontc-0.0.2a4/fea-rs/src/bin/parse_test.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/bin/ttx_test.rs` & `fontc-0.0.2a4/fea-rs/src/bin/ttx_test.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/common/glyph_class.rs` & `fontc-0.0.2a4/fea-rs/src/common/glyph_class.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/common/glyph_map.rs` & `fontc-0.0.2a4/fea-rs/src/common/glyph_map.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/common.rs` & `fontc-0.0.2a4/fea-rs/src/common.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/compile_ctx.rs` & `fontc-0.0.2a4/fea-rs/src/compile/compile_ctx.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/compiler.rs` & `fontc-0.0.2a4/fea-rs/src/compile/compiler.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/error.rs` & `fontc-0.0.2a4/fea-rs/src/compile/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/feature_writer.rs` & `fontc-0.0.2a4/fea-rs/src/compile/feature_writer.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/features.rs` & `fontc-0.0.2a4/fea-rs/src/compile/features.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/glyph_range.rs` & `fontc-0.0.2a4/fea-rs/src/compile/glyph_range.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/language_system.rs` & `fontc-0.0.2a4/fea-rs/src/compile/language_system.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/lookups/contextual.rs` & `fontc-0.0.2a4/fea-rs/src/compile/lookups/contextual.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/lookups/gpos_builders.rs` & `fontc-0.0.2a4/fea-rs/src/compile/lookups/gpos_builders.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/lookups/gsub_builders.rs` & `fontc-0.0.2a4/fea-rs/src/compile/lookups/gsub_builders.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/lookups/helpers.rs` & `fontc-0.0.2a4/fea-rs/src/compile/lookups/helpers.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/lookups.rs` & `fontc-0.0.2a4/fea-rs/src/compile/lookups.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/metrics.rs` & `fontc-0.0.2a4/fea-rs/src/compile/metrics.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/opts.rs` & `fontc-0.0.2a4/fea-rs/src/compile/opts.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/output.rs` & `fontc-0.0.2a4/fea-rs/src/compile/output.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/tables/base.rs` & `fontc-0.0.2a4/fea-rs/src/compile/tables/base.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/tables/gdef.rs` & `fontc-0.0.2a4/fea-rs/src/compile/tables/gdef.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/tables/name.rs` & `fontc-0.0.2a4/fea-rs/src/compile/tables/name.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/tables/os2.rs` & `fontc-0.0.2a4/fea-rs/src/compile/tables/os2.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/tables/stat.rs` & `fontc-0.0.2a4/fea-rs/src/compile/tables/stat.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/tables.rs` & `fontc-0.0.2a4/fea-rs/src/compile/tables.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/tags.rs` & `fontc-0.0.2a4/fea-rs/src/compile/tags.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/validate.rs` & `fontc-0.0.2a4/fea-rs/src/compile/validate.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile/variations.rs` & `fontc-0.0.2a4/fea-rs/src/compile/variations.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/compile.rs` & `fontc-0.0.2a4/fea-rs/src/compile.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/diagnostic.rs` & `fontc-0.0.2a4/fea-rs/src/diagnostic.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/lib.rs` & `fontc-0.0.2a4/fea-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/context.rs` & `fontc-0.0.2a4/fea-rs/src/parse/context.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/grammar/feature.rs` & `fontc-0.0.2a4/fea-rs/src/parse/grammar/feature.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/grammar/glyph.rs` & `fontc-0.0.2a4/fea-rs/src/parse/grammar/glyph.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/grammar/gpos.rs` & `fontc-0.0.2a4/fea-rs/src/parse/grammar/gpos.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/grammar/gsub.rs` & `fontc-0.0.2a4/fea-rs/src/parse/grammar/gsub.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/grammar/metrics.rs` & `fontc-0.0.2a4/fea-rs/src/parse/grammar/metrics.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/grammar/mod.rs` & `fontc-0.0.2a4/fea-rs/src/parse/grammar/mod.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/grammar/table.rs` & `fontc-0.0.2a4/fea-rs/src/parse/grammar/table.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/grammar/variations.rs` & `fontc-0.0.2a4/fea-rs/src/parse/grammar/variations.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/lexer/lexeme.rs` & `fontc-0.0.2a4/fea-rs/src/parse/lexer/lexeme.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/lexer/token_set.rs` & `fontc-0.0.2a4/fea-rs/src/parse/lexer/token_set.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/lexer.rs` & `fontc-0.0.2a4/fea-rs/src/parse/lexer.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/parser.rs` & `fontc-0.0.2a4/fea-rs/src/parse/parser.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/source.rs` & `fontc-0.0.2a4/fea-rs/src/parse/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse/tree.rs` & `fontc-0.0.2a4/fea-rs/src/parse/tree.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/parse.rs` & `fontc-0.0.2a4/fea-rs/src/parse.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/tests/compile.rs` & `fontc-0.0.2a4/fea-rs/src/tests/compile.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/tests/parse.rs` & `fontc-0.0.2a4/fea-rs/src/tests/parse.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/token_tree/cursor.rs` & `fontc-0.0.2a4/fea-rs/src/token_tree/cursor.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/token_tree/edit.rs` & `fontc-0.0.2a4/fea-rs/src/token_tree/edit.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/token_tree/rewrite.rs` & `fontc-0.0.2a4/fea-rs/src/token_tree/rewrite.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/token_tree/stack.rs` & `fontc-0.0.2a4/fea-rs/src/token_tree/stack.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/token_tree/token.rs` & `fontc-0.0.2a4/fea-rs/src/token_tree/token.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/token_tree/typed.rs` & `fontc-0.0.2a4/fea-rs/src/token_tree/typed.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/token_tree.rs` & `fontc-0.0.2a4/fea-rs/src/token_tree.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/util/highlighting.rs` & `fontc-0.0.2a4/fea-rs/src/util/highlighting.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/util/paths.rs` & `fontc-0.0.2a4/fea-rs/src/util/paths.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/util/pretty_diff.rs` & `fontc-0.0.2a4/fea-rs/src/util/pretty_diff.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/util/ttx.rs` & `fontc-0.0.2a4/fea-rs/src/util/ttx.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fea-rs/src/util.rs` & `fontc-0.0.2a4/fea-rs/src/util.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/Cargo.toml` & `fontc-0.0.2a4/fontbe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/avar.rs` & `fontc-0.0.2a4/fontbe/src/avar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/cmap.rs` & `fontc-0.0.2a4/fontbe/src/cmap.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/error.rs` & `fontc-0.0.2a4/fontbe/src/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/features/kern.rs` & `fontc-0.0.2a4/fontbe/src/features/kern.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/features/marks.rs` & `fontc-0.0.2a4/fontbe/src/features/marks.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/features/ot_tags.rs` & `fontc-0.0.2a4/fontbe/src/features/ot_tags.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/features/properties.rs` & `fontc-0.0.2a4/fontbe/src/features/properties.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/features.rs` & `fontc-0.0.2a4/fontbe/src/features.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/font.rs` & `fontc-0.0.2a4/fontbe/src/font.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/fvar.rs` & `fontc-0.0.2a4/fontbe/src/fvar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/glyphs.rs` & `fontc-0.0.2a4/fontbe/src/glyphs.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/gvar.rs` & `fontc-0.0.2a4/fontbe/src/gvar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/head.rs` & `fontc-0.0.2a4/fontbe/src/head.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/hvar.rs` & `fontc-0.0.2a4/fontbe/src/hvar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/metrics_and_limits.rs` & `fontc-0.0.2a4/fontbe/src/metrics_and_limits.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/mvar.rs` & `fontc-0.0.2a4/fontbe/src/mvar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/name.rs` & `fontc-0.0.2a4/fontbe/src/name.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/orchestration.rs` & `fontc-0.0.2a4/fontbe/src/orchestration.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/os2.rs` & `fontc-0.0.2a4/fontbe/src/os2.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/paths.rs` & `fontc-0.0.2a4/fontbe/src/paths.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/post.rs` & `fontc-0.0.2a4/fontbe/src/post.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/stat.rs` & `fontc-0.0.2a4/fontbe/src/stat.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontbe/src/test_util.rs` & `fontc-0.0.2a4/fontbe/src/test_util.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontra2fontir/Cargo.toml` & `fontc-0.0.2a4/fontra2fontir/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontra2fontir/src/fontra.rs` & `fontc-0.0.2a4/fontra2fontir/src/fontra.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontra2fontir/src/source.rs` & `fontc-0.0.2a4/fontra2fontir/src/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontra2fontir/src/toir.rs` & `fontc-0.0.2a4/fontra2fontir/src/toir.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/Cargo.toml` & `fontc-0.0.2a4/glyphs-reader/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/build.rs` & `fontc-0.0.2a4/glyphs-reader/build.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/data/GlyphData.xml` & `fontc-0.0.2a4/glyphs-reader/data/GlyphData.xml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/data/GlyphData_Ideographs.xml` & `fontc-0.0.2a4/glyphs-reader/data/GlyphData_Ideographs.xml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/data/GlyphData_override_test.xml` & `fontc-0.0.2a4/glyphs-reader/data/GlyphData_override_test.xml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/data/update.py` & `fontc-0.0.2a4/glyphs-reader/data/update.py`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/src/error.rs` & `fontc-0.0.2a4/glyphs-reader/src/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/src/font.rs` & `fontc-0.0.2a4/glyphs-reader/src/font.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/src/glyphdata/glyphdata_impl.rs` & `fontc-0.0.2a4/glyphs-reader/src/glyphdata/glyphdata_impl.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/src/glyphdata.rs` & `fontc-0.0.2a4/glyphs-reader/src/glyphdata.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/src/plist.rs` & `fontc-0.0.2a4/glyphs-reader/src/plist.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/glyphs-reader/src/propagate_anchors.rs` & `fontc-0.0.2a4/glyphs-reader/src/propagate_anchors.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/Cargo.toml` & `fontc-0.0.2a4/fontir/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/error.rs` & `fontc-0.0.2a4/fontir/src/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/glyph.rs` & `fontc-0.0.2a4/fontir/src/glyph.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/ir.rs` & `fontc-0.0.2a4/fontir/src/ir.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/orchestration.rs` & `fontc-0.0.2a4/fontir/src/orchestration.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/paths.rs` & `fontc-0.0.2a4/fontir/src/paths.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/serde.rs` & `fontc-0.0.2a4/fontir/src/serde.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/source.rs` & `fontc-0.0.2a4/fontir/src/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/stateset.rs` & `fontc-0.0.2a4/fontir/src/stateset.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontir/src/variations.rs` & `fontc-0.0.2a4/fontir/src/variations.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/Cargo.toml` & `fontc-0.0.2a4/fontc/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/args.rs` & `fontc-0.0.2a4/fontc/src/args.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/change_detector.rs` & `fontc-0.0.2a4/fontc/src/change_detector.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/config.rs` & `fontc-0.0.2a4/fontc/src/config.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/error.rs` & `fontc-0.0.2a4/fontc/src/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/lib.rs` & `fontc-0.0.2a4/fontc/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/main.rs` & `fontc-0.0.2a4/fontc/src/main.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/timing.rs` & `fontc-0.0.2a4/fontc/src/timing.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/work.rs` & `fontc-0.0.2a4/fontc/src/work.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/fontc/src/workload.rs` & `fontc-0.0.2a4/fontc/src/workload.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/Cargo.lock` & `fontc-0.0.2a4/Cargo.lock`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/Cargo.toml` & `fontc-0.0.2a4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/pyproject.toml` & `fontc-0.0.2a4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 # maturin merges the metadata from Cargo.toml with the pyproject.toml's below,
 # which takes precedence and overrides Cargo.toml
 [project]
 # 'name' key is required for [project]
 name = "fontc"
 # comment out 'version' to use the same as Cargo.toml, only override if needed
 # (e.g. for a post-release to fix some packaging issues with a previous release)
-version = "0.0.2a3"
+version = "0.0.2a4"
 # Ensure we use the workspace's top-level README.md for the sdist/wheel metadata
 # not the fontc crate's specific README.md
 readme = "README.md"
```

### Comparing `fontc-0.0.2a3/README.md` & `fontc-0.0.2a4/README.md`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/LICENSE` & `fontc-0.0.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a3/PKG-INFO` & `fontc-0.0.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fontc
-Version: 0.0.2a3
+Version: 0.0.2a4
 License-File: LICENSE
 Summary: A compiler for fonts.
 License: MIT/Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/googlefonts/fontc
 
 # fontc
```

