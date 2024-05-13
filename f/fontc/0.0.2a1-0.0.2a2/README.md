# Comparing `tmp/fontc-0.0.2a1.tar.gz` & `tmp/fontc-0.0.2a2.tar.gz`

## Comparing `fontc-0.0.2a1.tar` & `fontc-0.0.2a2.tar`

### file list

```diff
@@ -1,173 +1,172 @@
--rw-r--r--   0      501       20     1413 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/Cargo.toml
--rw-r--r--   0      501       20     5219 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/README.md
--rw-r--r--   0      501       20     1036 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/benches/parsing.rs
--rw-r--r--   0      501       20     6563 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/bin/compile.rs
--rw-r--r--   0      501       20     1598 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/bin/highlight.rs
--rw-r--r--   0      501       20     3559 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/bin/parse_test.rs
--rw-r--r--   0      501       20     2427 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/bin/ttx_test.rs
--rw-r--r--   0      501       20     3741 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/common/glyph_class.rs
--rw-r--r--   0      501       20     5732 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/common/glyph_map.rs
--rw-r--r--   0      501       20     3246 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/common.rs
--rw-r--r--   0      501       20    88121 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/compile_ctx.rs
--rw-r--r--   0      501       20     6792 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/compiler.rs
--rw-r--r--   0      501       20     2204 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/error.rs
--rw-r--r--   0      501       20     4647 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/feature_writer.rs
--rw-r--r--   0      501       20    24755 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/features.rs
--rw-r--r--   0      501       20     8873 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/glyph_range.rs
--rw-r--r--   0      501       20     1887 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/language_system.rs
--rw-r--r--   0      501       20    26387 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/lookups/contextual.rs
--rw-r--r--   0      501       20    22671 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/lookups/gpos_builders.rs
--rw-r--r--   0      501       20     8415 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/lookups/gsub_builders.rs
--rw-r--r--   0      501       20     4720 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/lookups/helpers.rs
--rw-r--r--   0      501       20    42617 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/lookups.rs
--rw-r--r--   0      501       20    12476 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/metrics.rs
--rw-r--r--   0      501       20     3285 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/opts.rs
--rw-r--r--   0      501       20     3725 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/output.rs
--rw-r--r--   0      501       20     2189 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/tables/base.rs
--rw-r--r--   0      501       20     5298 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/tables/gdef.rs
--rw-r--r--   0      501       20     5532 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/tables/name.rs
--rw-r--r--   0      501       20     4113 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/tables/os2.rs
--rw-r--r--   0      501       20     5347 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/tables/stat.rs
--rw-r--r--   0      501       20     2789 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/tables.rs
--rw-r--r--   0      501       20     2031 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/tags.rs
--rw-r--r--   0      501       20    58287 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/validate.rs
--rw-r--r--   0      501       20     8061 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile/variations.rs
--rw-r--r--   0      501       20     5229 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/compile.rs
--rw-r--r--   0      501       20     5999 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/diagnostic.rs
--rw-r--r--   0      501       20      624 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/lib.rs
--rw-r--r--   0      501       20    16381 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/context.rs
--rw-r--r--   0      501       20    10160 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/grammar/feature.rs
--rw-r--r--   0      501       20     9162 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/grammar/glyph.rs
--rw-r--r--   0      501       20     8103 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/grammar/gpos.rs
--rw-r--r--   0      501       20     7824 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/grammar/gsub.rs
--rw-r--r--   0      501       20    11835 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/grammar/metrics.rs
--rw-r--r--   0      501       20    11841 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/grammar/mod.rs
--rw-r--r--   0      501       20    19662 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/grammar/table.rs
--rw-r--r--   0      501       20     3307 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/grammar/variations.rs
--rw-r--r--   0      501       20    25328 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/lexer/lexeme.rs
--rw-r--r--   0      501       20     6748 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/lexer/token_set.rs
--rw-r--r--   0      501       20    13214 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/lexer.rs
--rw-r--r--   0      501       20    13148 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/parser.rs
--rw-r--r--   0      501       20    12900 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/source.rs
--rw-r--r--   0      501       20     1741 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse/tree.rs
--rw-r--r--   0      501       20     3528 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/parse.rs
--rw-r--r--   0      501       20     4712 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/tests/compile.rs
--rw-r--r--   0      501       20     4164 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/tests/parse.rs
--rw-r--r--   0      501       20       52 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/tests.rs
--rw-r--r--   0      501       20     8618 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/token_tree/cursor.rs
--rw-r--r--   0      501       20     4704 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/token_tree/edit.rs
--rw-r--r--   0      501       20    11526 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/token_tree/rewrite.rs
--rw-r--r--   0      501       20     2017 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/token_tree/stack.rs
--rw-r--r--   0      501       20    22316 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/token_tree/token.rs
--rw-r--r--   0      501       20    47941 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/token_tree/typed.rs
--rw-r--r--   0      501       20    20795 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/token_tree.rs
--rw-r--r--   0      501       20     7594 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/util/highlighting.rs
--rw-r--r--   0      501       20     3851 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/util/paths.rs
--rw-r--r--   0      501       20     8008 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/util/pretty_diff.rs
--rw-r--r--   0      501       20    26284 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/util/ttx.rs
--rw-r--r--   0      501       20      737 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fea-rs/src/util.rs
--rw-r--r--   0      501       20      869 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/Cargo.toml
--rw-r--r--   0      501       20      417 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/README.md
--rw-r--r--   0      501       20     1056 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/build.rs
--rw-r--r--   0      501       20  5067653 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/data/GlyphData.xml
--rw-r--r--   0      501       20  2926546 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/data/GlyphData_Ideographs.xml
--rw-r--r--   0      501       20      947 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/data/GlyphData_override_test.xml
--rw-r--r--   0      501       20      380 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/data/README.md
--rw-r--r--   0      501       20       81 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/data/VERSION
--rw-r--r--   0      501       20     1212 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/data/update.py
--rw-r--r--   0      501       20      821 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/src/error.rs
--rw-r--r--   0      501       20    98609 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/src/font.rs
--rw-r--r--   0      501       20    10744 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/src/glyphdata/glyphdata_impl.rs
--rw-r--r--   0      501       20    19710 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/src/glyphdata.rs
--rw-r--r--   0      501       20      304 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/src/lib.rs
--rw-r--r--   0      501       20    24558 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/src/plist.rs
--rw-r--r--   0      501       20    32909 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/src/propagate_anchors.rs
--rw-r--r--   0      501       20     1053 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/Cargo.toml
--rw-r--r--   0      501       20      271 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/README.md
--rw-r--r--   0      501       20     7181 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/avar.rs
--rw-r--r--   0      501       20     1813 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/cmap.rs
--rw-r--r--   0      501       20     4205 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/error.rs
--rw-r--r--   0      501       20      691 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/features/common.rs
--rw-r--r--   0      501       20    47114 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/features/kern.rs
--rw-r--r--   0      501       20    11842 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/features/marks.rs
--rw-r--r--   0      501       20     5050 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/features/ot_tags.rs
--rw-r--r--   0      501       20    11877 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/features/properties.rs
--rw-r--r--   0      501       20    23244 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/features.rs
--rw-r--r--   0      501       20     6620 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/font.rs
--rw-r--r--   0      501       20     4831 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/fvar.rs
--rw-r--r--   0      501       20    37227 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/glyphs.rs
--rw-r--r--   0      501       20     3586 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/gvar.rs
--rw-r--r--   0      501       20     7317 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/head.rs
--rw-r--r--   0      501       20     9069 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/hvar.rs
--rw-r--r--   0      501       20      310 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/lib.rs
--rw-r--r--   0      501       20    14201 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/metrics_and_limits.rs
--rw-r--r--   0      501       20    11306 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/mvar.rs
--rw-r--r--   0      501       20     1477 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/name.rs
--rw-r--r--   0      501       20    32175 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/orchestration.rs
--rw-r--r--   0      501       20    34761 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/os2.rs
--rw-r--r--   0      501       20     3776 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/paths.rs
--rw-r--r--   0      501       20     2011 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/post.rs
--rw-r--r--   0      501       20     2435 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/stat.rs
--rw-r--r--   0      501       20      930 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontbe/src/test_util.rs
--rw-r--r--   0      501       20      561 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/Cargo.toml
--rw-r--r--   0      501       20      452 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/README.md
--rw-r--r--   0      501       20     2688 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/build.rs
--rw-r--r--   0      501       20    27655 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/data/aglfn.txt
--rw-r--r--   0      501       20    78060 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/data/glyphlist.txt
--rw-r--r--   0      501       20     6710 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/src/agl.rs
--rw-r--r--   0      501       20    19926 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/src/coords.rs
--rw-r--r--   0      501       20      188 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/src/lib.rs
--rw-r--r--   0      501       20     9962 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/src/orchestration.rs
--rw-r--r--   0      501       20     6769 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/src/paths.rs
--rw-r--r--   0      501       20     4727 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/src/piecewise_linear_map.rs
--rw-r--r--   0      501       20     1993 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontdrasil/src/types.rs
--rw-r--r--   0      501       20      854 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs2fontir/Cargo.toml
--rw-r--r--   0      501       20      184 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs2fontir/README.md
--rw-r--r--   0      501       20       26 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs2fontir/src/lib.rs
--rw-r--r--   0      501       20    57821 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs2fontir/src/source.rs
--rw-r--r--   0      501       20    12432 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs2fontir/src/toir.rs
--rw-r--r--   0      501       20      946 2024-05-09 17:29:13.000000 fontc-0.0.2a1/ufo2fontir/Cargo.toml
--rw-r--r--   0      501       20      188 2024-05-09 17:29:13.000000 fontc-0.0.2a1/ufo2fontir/README.md
--rw-r--r--   0      501       20       30 2024-05-09 17:29:13.000000 fontc-0.0.2a1/ufo2fontir/src/lib.rs
--rw-r--r--   0      501       20    81135 2024-05-09 17:29:13.000000 fontc-0.0.2a1/ufo2fontir/src/source.rs
--rw-r--r--   0      501       20    10780 2024-05-09 17:29:13.000000 fontc-0.0.2a1/ufo2fontir/src/toir.rs
--rw-r--r--   0      501       20     1295 2024-05-09 17:29:13.000000 fontc-0.0.2a1/ufo2fontir/testdata/wght_var.designspace
--rw-r--r--   0      501       20      810 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontra2fontir/Cargo.toml
--rw-r--r--   0      501       20      207 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontra2fontir/README.md
--rw-r--r--   0      501       20    15733 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontra2fontir/src/fontra.rs
--rw-r--r--   0      501       20      325 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontra2fontir/src/lib.rs
--rw-r--r--   0      501       20    10816 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontra2fontir/src/source.rs
--rw-r--r--   0      501       20    10630 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontra2fontir/src/toir.rs
--rw-r--r--   0      501       20      949 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/Cargo.toml
--rw-r--r--   0      501       20      334 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/README.md
--rw-r--r--   0      501       20     7704 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/error.rs
--rw-r--r--   0      501       20    31884 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/glyph.rs
--rw-r--r--   0      501       20    81059 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/ir.rs
--rw-r--r--   0      501       20      156 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/lib.rs
--rw-r--r--   0      501       20    15993 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/orchestration.rs
--rw-r--r--   0      501       20     2617 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/paths.rs
--rw-r--r--   0      501       20     3426 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/serde.rs
--rw-r--r--   0      501       20     5978 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/source.rs
--rw-r--r--   0      501       20    13439 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/stateset.rs
--rw-r--r--   0      501       20    50736 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontir/src/variations.rs
--rw-r--r--   0      501       20      346 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/plist_derive/Cargo.toml
--rw-r--r--   0      501       20     2382 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/plist_derive/src/attrs.rs
--rw-r--r--   0      501       20     3109 2024-05-09 17:29:13.000000 fontc-0.0.2a1/glyphs-reader/plist_derive/src/lib.rs
--rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 fontc-0.0.2a1/fontc/Cargo.toml
--rw-r--r--   0      501       20      348 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/README.md
--rw-r--r--   0      501       20      278 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/build.rs
--rw-r--r--   0      501       20     7761 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/args.rs
--rw-r--r--   0      501       20    12794 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/change_detector.rs
--rw-r--r--   0      501       20     4073 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/config.rs
--rw-r--r--   0      501       20      722 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/error.rs
--rw-r--r--   0      501       20   101138 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/lib.rs
--rw-r--r--   0      501       20     3832 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/main.rs
--rw-r--r--   0      501       20    10457 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/timing.rs
--rw-r--r--   0      501       20     7305 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/work.rs
--rw-r--r--   0      501       20    33415 2024-05-09 17:29:13.000000 fontc-0.0.2a1/fontc/src/workload.rs
--rw-r--r--   0      501       20    60506 2024-05-09 17:32:34.000000 fontc-0.0.2a1/Cargo.lock
--rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 fontc-0.0.2a1/Cargo.toml
--rw-r--r--   0      501       20     1251 2024-05-09 17:29:13.000000 fontc-0.0.2a1/pyproject.toml
--rw-r--r--   0      501       20     7765 2024-05-09 17:29:13.000000 fontc-0.0.2a1/README.md
--rw-r--r--   0      501       20    11357 2024-05-09 17:29:13.000000 fontc-0.0.2a1/LICENSE
--rw-r--r--   0        0        0     8026 1970-01-01 00:00:00.000000 fontc-0.0.2a1/PKG-INFO
+-rw-r--r--   0      501       20     1413 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/Cargo.toml
+-rw-r--r--   0      501       20     5219 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/README.md
+-rw-r--r--   0      501       20     1036 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/benches/parsing.rs
+-rw-r--r--   0      501       20     6563 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/bin/compile.rs
+-rw-r--r--   0      501       20     1598 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/bin/highlight.rs
+-rw-r--r--   0      501       20     3559 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/bin/parse_test.rs
+-rw-r--r--   0      501       20     2427 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/bin/ttx_test.rs
+-rw-r--r--   0      501       20     3741 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/common/glyph_class.rs
+-rw-r--r--   0      501       20     5732 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/common/glyph_map.rs
+-rw-r--r--   0      501       20     3246 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/common.rs
+-rw-r--r--   0      501       20    88121 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/compile_ctx.rs
+-rw-r--r--   0      501       20     6792 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/compiler.rs
+-rw-r--r--   0      501       20     2204 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/error.rs
+-rw-r--r--   0      501       20     5683 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/feature_writer.rs
+-rw-r--r--   0      501       20    24755 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/features.rs
+-rw-r--r--   0      501       20     8873 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/glyph_range.rs
+-rw-r--r--   0      501       20     1887 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/language_system.rs
+-rw-r--r--   0      501       20    26387 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/lookups/contextual.rs
+-rw-r--r--   0      501       20    22671 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/lookups/gpos_builders.rs
+-rw-r--r--   0      501       20     8415 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/lookups/gsub_builders.rs
+-rw-r--r--   0      501       20     4720 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/lookups/helpers.rs
+-rw-r--r--   0      501       20    42617 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/lookups.rs
+-rw-r--r--   0      501       20    12476 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/metrics.rs
+-rw-r--r--   0      501       20     3285 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/opts.rs
+-rw-r--r--   0      501       20     3725 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/output.rs
+-rw-r--r--   0      501       20     2189 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/tables/base.rs
+-rw-r--r--   0      501       20     5298 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/tables/gdef.rs
+-rw-r--r--   0      501       20     5532 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/tables/name.rs
+-rw-r--r--   0      501       20     4113 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/tables/os2.rs
+-rw-r--r--   0      501       20     5347 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/tables/stat.rs
+-rw-r--r--   0      501       20     2789 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/tables.rs
+-rw-r--r--   0      501       20     2031 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/tags.rs
+-rw-r--r--   0      501       20    58287 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/validate.rs
+-rw-r--r--   0      501       20     8061 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile/variations.rs
+-rw-r--r--   0      501       20     5244 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/compile.rs
+-rw-r--r--   0      501       20     5999 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/diagnostic.rs
+-rw-r--r--   0      501       20      624 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/lib.rs
+-rw-r--r--   0      501       20    16381 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/context.rs
+-rw-r--r--   0      501       20    10160 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/grammar/feature.rs
+-rw-r--r--   0      501       20     9162 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/grammar/glyph.rs
+-rw-r--r--   0      501       20     8103 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/grammar/gpos.rs
+-rw-r--r--   0      501       20     7824 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/grammar/gsub.rs
+-rw-r--r--   0      501       20    11835 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/grammar/metrics.rs
+-rw-r--r--   0      501       20    11841 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/grammar/mod.rs
+-rw-r--r--   0      501       20    19662 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/grammar/table.rs
+-rw-r--r--   0      501       20     3307 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/grammar/variations.rs
+-rw-r--r--   0      501       20    25328 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/lexer/lexeme.rs
+-rw-r--r--   0      501       20     6748 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/lexer/token_set.rs
+-rw-r--r--   0      501       20    13214 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/lexer.rs
+-rw-r--r--   0      501       20    13148 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/parser.rs
+-rw-r--r--   0      501       20    12900 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/source.rs
+-rw-r--r--   0      501       20     1741 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse/tree.rs
+-rw-r--r--   0      501       20     3528 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/parse.rs
+-rw-r--r--   0      501       20     4712 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/tests/compile.rs
+-rw-r--r--   0      501       20     4164 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/tests/parse.rs
+-rw-r--r--   0      501       20       52 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/tests.rs
+-rw-r--r--   0      501       20     8618 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/token_tree/cursor.rs
+-rw-r--r--   0      501       20     4704 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/token_tree/edit.rs
+-rw-r--r--   0      501       20    11526 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/token_tree/rewrite.rs
+-rw-r--r--   0      501       20     2017 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/token_tree/stack.rs
+-rw-r--r--   0      501       20    22316 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/token_tree/token.rs
+-rw-r--r--   0      501       20    47941 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/token_tree/typed.rs
+-rw-r--r--   0      501       20    20795 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/token_tree.rs
+-rw-r--r--   0      501       20     7594 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/util/highlighting.rs
+-rw-r--r--   0      501       20     3851 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/util/paths.rs
+-rw-r--r--   0      501       20     8008 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/util/pretty_diff.rs
+-rw-r--r--   0      501       20    26284 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/util/ttx.rs
+-rw-r--r--   0      501       20      737 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fea-rs/src/util.rs
+-rw-r--r--   0      501       20      810 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontra2fontir/Cargo.toml
+-rw-r--r--   0      501       20      207 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontra2fontir/README.md
+-rw-r--r--   0      501       20    15733 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontra2fontir/src/fontra.rs
+-rw-r--r--   0      501       20      325 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontra2fontir/src/lib.rs
+-rw-r--r--   0      501       20    10816 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontra2fontir/src/source.rs
+-rw-r--r--   0      501       20    10630 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontra2fontir/src/toir.rs
+-rw-r--r--   0      501       20     1053 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/Cargo.toml
+-rw-r--r--   0      501       20      271 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/README.md
+-rw-r--r--   0      501       20     7181 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/avar.rs
+-rw-r--r--   0      501       20     1813 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/cmap.rs
+-rw-r--r--   0      501       20     4205 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/error.rs
+-rw-r--r--   0      501       20    47130 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/features/kern.rs
+-rw-r--r--   0      501       20    16093 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/features/marks.rs
+-rw-r--r--   0      501       20     5050 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/features/ot_tags.rs
+-rw-r--r--   0      501       20    11877 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/features/properties.rs
+-rw-r--r--   0      501       20    23190 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/features.rs
+-rw-r--r--   0      501       20     6620 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/font.rs
+-rw-r--r--   0      501       20     4831 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/fvar.rs
+-rw-r--r--   0      501       20    37227 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/glyphs.rs
+-rw-r--r--   0      501       20     3586 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/gvar.rs
+-rw-r--r--   0      501       20     7317 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/head.rs
+-rw-r--r--   0      501       20     9069 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/hvar.rs
+-rw-r--r--   0      501       20      310 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/lib.rs
+-rw-r--r--   0      501       20    14201 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/metrics_and_limits.rs
+-rw-r--r--   0      501       20    11306 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/mvar.rs
+-rw-r--r--   0      501       20     1477 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/name.rs
+-rw-r--r--   0      501       20    32165 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/orchestration.rs
+-rw-r--r--   0      501       20    34761 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/os2.rs
+-rw-r--r--   0      501       20     3776 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/paths.rs
+-rw-r--r--   0      501       20     2011 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/post.rs
+-rw-r--r--   0      501       20     2435 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/stat.rs
+-rw-r--r--   0      501       20      930 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontbe/src/test_util.rs
+-rw-r--r--   0      501       20      346 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/plist_derive/Cargo.toml
+-rw-r--r--   0      501       20     2382 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/plist_derive/src/attrs.rs
+-rw-r--r--   0      501       20     3109 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/plist_derive/src/lib.rs
+-rw-r--r--   0      501       20      949 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/Cargo.toml
+-rw-r--r--   0      501       20      334 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/README.md
+-rw-r--r--   0      501       20     7704 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/error.rs
+-rw-r--r--   0      501       20    31884 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/glyph.rs
+-rw-r--r--   0      501       20    81151 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/ir.rs
+-rw-r--r--   0      501       20      156 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/lib.rs
+-rw-r--r--   0      501       20    15993 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/orchestration.rs
+-rw-r--r--   0      501       20     2617 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/paths.rs
+-rw-r--r--   0      501       20     3426 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/serde.rs
+-rw-r--r--   0      501       20     5978 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/source.rs
+-rw-r--r--   0      501       20    13439 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/stateset.rs
+-rw-r--r--   0      501       20    50736 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontir/src/variations.rs
+-rw-r--r--   0      501       20      561 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/Cargo.toml
+-rw-r--r--   0      501       20      452 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/README.md
+-rw-r--r--   0      501       20     2688 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/build.rs
+-rw-r--r--   0      501       20    27655 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/data/aglfn.txt
+-rw-r--r--   0      501       20    78060 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/data/glyphlist.txt
+-rw-r--r--   0      501       20     6710 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/src/agl.rs
+-rw-r--r--   0      501       20    19926 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/src/coords.rs
+-rw-r--r--   0      501       20      188 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/src/lib.rs
+-rw-r--r--   0      501       20     9962 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/src/orchestration.rs
+-rw-r--r--   0      501       20     6769 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/src/paths.rs
+-rw-r--r--   0      501       20     4727 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/src/piecewise_linear_map.rs
+-rw-r--r--   0      501       20     1993 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontdrasil/src/types.rs
+-rw-r--r--   0      501       20      946 2024-05-13 12:47:46.000000 fontc-0.0.2a2/ufo2fontir/Cargo.toml
+-rw-r--r--   0      501       20      188 2024-05-13 12:47:46.000000 fontc-0.0.2a2/ufo2fontir/README.md
+-rw-r--r--   0      501       20       30 2024-05-13 12:47:46.000000 fontc-0.0.2a2/ufo2fontir/src/lib.rs
+-rw-r--r--   0      501       20    81135 2024-05-13 12:47:46.000000 fontc-0.0.2a2/ufo2fontir/src/source.rs
+-rw-r--r--   0      501       20    10780 2024-05-13 12:47:46.000000 fontc-0.0.2a2/ufo2fontir/src/toir.rs
+-rw-r--r--   0      501       20     1295 2024-05-13 12:47:46.000000 fontc-0.0.2a2/ufo2fontir/testdata/wght_var.designspace
+-rw-r--r--   0      501       20      854 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs2fontir/Cargo.toml
+-rw-r--r--   0      501       20      184 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs2fontir/README.md
+-rw-r--r--   0      501       20       26 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs2fontir/src/lib.rs
+-rw-r--r--   0      501       20    57821 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs2fontir/src/source.rs
+-rw-r--r--   0      501       20    12432 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs2fontir/src/toir.rs
+-rw-r--r--   0      501       20      869 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/Cargo.toml
+-rw-r--r--   0      501       20      417 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/README.md
+-rw-r--r--   0      501       20     1056 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/build.rs
+-rw-r--r--   0      501       20  5067653 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/data/GlyphData.xml
+-rw-r--r--   0      501       20  2926546 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/data/GlyphData_Ideographs.xml
+-rw-r--r--   0      501       20      947 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/data/GlyphData_override_test.xml
+-rw-r--r--   0      501       20      380 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/data/README.md
+-rw-r--r--   0      501       20       81 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/data/VERSION
+-rw-r--r--   0      501       20     1212 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/data/update.py
+-rw-r--r--   0      501       20      821 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/src/error.rs
+-rw-r--r--   0      501       20    98609 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/src/font.rs
+-rw-r--r--   0      501       20    10744 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/src/glyphdata/glyphdata_impl.rs
+-rw-r--r--   0      501       20    19710 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/src/glyphdata.rs
+-rw-r--r--   0      501       20      304 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/src/lib.rs
+-rw-r--r--   0      501       20    24558 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/src/plist.rs
+-rw-r--r--   0      501       20    32909 2024-05-13 12:47:46.000000 fontc-0.0.2a2/glyphs-reader/src/propagate_anchors.rs
+-rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 fontc-0.0.2a2/fontc/Cargo.toml
+-rw-r--r--   0      501       20      348 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/README.md
+-rw-r--r--   0      501       20      278 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/build.rs
+-rw-r--r--   0      501       20     7761 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/args.rs
+-rw-r--r--   0      501       20    12794 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/change_detector.rs
+-rw-r--r--   0      501       20     4073 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/config.rs
+-rw-r--r--   0      501       20      722 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/error.rs
+-rw-r--r--   0      501       20   101138 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/lib.rs
+-rw-r--r--   0      501       20     3832 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/main.rs
+-rw-r--r--   0      501       20    10457 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/timing.rs
+-rw-r--r--   0      501       20     7305 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/work.rs
+-rw-r--r--   0      501       20    33415 2024-05-13 12:47:46.000000 fontc-0.0.2a2/fontc/src/workload.rs
+-rw-r--r--   0      501       20    60506 2024-05-13 12:48:46.000000 fontc-0.0.2a2/Cargo.lock
+-rw-r--r--   0        0        0     1479 1970-01-01 00:00:00.000000 fontc-0.0.2a2/Cargo.toml
+-rw-r--r--   0      501       20     1251 2024-05-13 12:47:46.000000 fontc-0.0.2a2/pyproject.toml
+-rw-r--r--   0      501       20     7765 2024-05-13 12:47:46.000000 fontc-0.0.2a2/README.md
+-rw-r--r--   0      501       20    11357 2024-05-13 12:47:46.000000 fontc-0.0.2a2/LICENSE
+-rw-r--r--   0        0        0     8026 1970-01-01 00:00:00.000000 fontc-0.0.2a2/PKG-INFO
```

### Comparing `fontc-0.0.2a1/fea-rs/Cargo.toml` & `fontc-0.0.2a2/fea-rs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/README.md` & `fontc-0.0.2a2/fea-rs/README.md`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/benches/parsing.rs` & `fontc-0.0.2a2/fea-rs/benches/parsing.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/bin/compile.rs` & `fontc-0.0.2a2/fea-rs/src/bin/compile.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/bin/highlight.rs` & `fontc-0.0.2a2/fea-rs/src/bin/highlight.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/bin/parse_test.rs` & `fontc-0.0.2a2/fea-rs/src/bin/parse_test.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/bin/ttx_test.rs` & `fontc-0.0.2a2/fea-rs/src/bin/ttx_test.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/common/glyph_class.rs` & `fontc-0.0.2a2/fea-rs/src/common/glyph_class.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/common/glyph_map.rs` & `fontc-0.0.2a2/fea-rs/src/common/glyph_map.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/common.rs` & `fontc-0.0.2a2/fea-rs/src/common.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/compile_ctx.rs` & `fontc-0.0.2a2/fea-rs/src/compile/compile_ctx.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/compiler.rs` & `fontc-0.0.2a2/fea-rs/src/compile/compiler.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/error.rs` & `fontc-0.0.2a2/fea-rs/src/compile/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/feature_writer.rs` & `fontc-0.0.2a2/fea-rs/src/compile/feature_writer.rs`

 * *Files 11% similar despite different names*

```diff
@@ -42,14 +42,48 @@
     fn to_pos_lookup(
         flags: LookupFlag,
         filter_set: Option<FilterSetId>,
         subtables: Vec<Self>,
     ) -> ExternalGposLookup;
 }
 
+/// A lookup generated outside of user FEA
+///
+/// This will be merged into any user-provided features during compilation.
+#[derive(Debug, Default, Clone, PartialEq)]
+#[cfg_attr(feature = "serde", derive(serde::Serialize, serde::Deserialize))]
+pub struct PendingLookup<T> {
+    subtables: Vec<T>,
+    flags: LookupFlag,
+    mark_filter_set: Option<GlyphSet>,
+}
+
+impl<T> PendingLookup<T> {
+    /// Create a new lookup.
+    ///
+    /// This can later be added to the feature builder via [`FeatureBuilder::add_lookup`]
+    pub fn new(subtables: Vec<T>, flags: LookupFlag, mark_filter_set: Option<GlyphSet>) -> Self {
+        Self {
+            subtables,
+            flags,
+            mark_filter_set,
+        }
+    }
+
+    /// Return a reference to the subtables in this lookup.
+    pub fn subtables(&self) -> &[T] {
+        &self.subtables
+    }
+
+    /// Return the `LookupFlag` for this lookup.
+    pub fn flags(&self) -> LookupFlag {
+        self.flags
+    }
+}
+
 /// An externally created GPOS lookup.
 ///
 /// This only exists so that we can avoid making our internal types `pub`.
 pub struct ExternalGposLookup(PositionLookup);
 
 impl<'a> FeatureBuilder<'a> {
     pub(crate) fn new(
@@ -73,24 +107,25 @@
     }
 
     /// If the FEA text contained an explicit GDEF table block, return its contents
     pub fn gdef(&self) -> Option<&GdefBuilder> {
         self.tables.gdef.as_ref()
     }
 
-    /// Create a new lookup.
+    /// Add a lookup to the lookup list.
     ///
-    /// The `LookupId` that is returned can then be included in features
-    pub fn add_lookup<T: GposSubtableBuilder>(
-        &mut self,
-        flags: LookupFlag,
-        filter_set: Option<GlyphSet>,
-        subtables: Vec<T>,
-    ) -> LookupId {
-        let filter_set_id = filter_set.map(|cls| self.get_filter_set_id(cls));
+    /// The `LookupId` that is returned can then be included in features (i.e,
+    /// passed to [`add_feature`](Self::add_feature).)
+    pub fn add_lookup<T: GposSubtableBuilder>(&mut self, lookup: PendingLookup<T>) -> LookupId {
+        let PendingLookup {
+            subtables,
+            flags,
+            mark_filter_set,
+        } = lookup;
+        let filter_set_id = mark_filter_set.map(|cls| self.get_filter_set_id(cls));
         let lookup = T::to_pos_lookup(flags, filter_set_id, subtables);
         let next_id = LookupId::External(self.lookups.len());
         self.lookups.push((next_id, lookup.0));
         next_id
     }
 
     /// Add lookups to every default language system.
@@ -109,15 +144,14 @@
     /// which a feature is to be registered.
     pub fn add_feature(&mut self, key: FeatureKey, lookups: Vec<LookupId>) {
         self.features.entry(key).or_default().base = lookups;
     }
 
     fn get_filter_set_id(&mut self, cls: GlyphSet) -> FilterSetId {
         let next_id = self.filter_set_id_start + self.mark_filter_sets.len();
-        //.expect("too many filter sets");
         *self.mark_filter_sets.entry(cls).or_insert_with(|| {
             next_id
                 .try_into()
                 // is this in any way an expected error condition?
                 .expect("too many filter sets?")
         })
     }
```

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/features.rs` & `fontc-0.0.2a2/fea-rs/src/compile/features.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/glyph_range.rs` & `fontc-0.0.2a2/fea-rs/src/compile/glyph_range.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/language_system.rs` & `fontc-0.0.2a2/fea-rs/src/compile/language_system.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/lookups/contextual.rs` & `fontc-0.0.2a2/fea-rs/src/compile/lookups/contextual.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/lookups/gpos_builders.rs` & `fontc-0.0.2a2/fea-rs/src/compile/lookups/gpos_builders.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/lookups/gsub_builders.rs` & `fontc-0.0.2a2/fea-rs/src/compile/lookups/gsub_builders.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/lookups/helpers.rs` & `fontc-0.0.2a2/fea-rs/src/compile/lookups/helpers.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/lookups.rs` & `fontc-0.0.2a2/fea-rs/src/compile/lookups.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/metrics.rs` & `fontc-0.0.2a2/fea-rs/src/compile/metrics.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/opts.rs` & `fontc-0.0.2a2/fea-rs/src/compile/opts.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/output.rs` & `fontc-0.0.2a2/fea-rs/src/compile/output.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/tables/base.rs` & `fontc-0.0.2a2/fea-rs/src/compile/tables/base.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/tables/gdef.rs` & `fontc-0.0.2a2/fea-rs/src/compile/tables/gdef.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/tables/name.rs` & `fontc-0.0.2a2/fea-rs/src/compile/tables/name.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/tables/os2.rs` & `fontc-0.0.2a2/fea-rs/src/compile/tables/os2.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/tables/stat.rs` & `fontc-0.0.2a2/fea-rs/src/compile/tables/stat.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/tables.rs` & `fontc-0.0.2a2/fea-rs/src/compile/tables.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/tags.rs` & `fontc-0.0.2a2/fea-rs/src/compile/tags.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/validate.rs` & `fontc-0.0.2a2/fea-rs/src/compile/validate.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile/variations.rs` & `fontc-0.0.2a2/fea-rs/src/compile/variations.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/compile.rs` & `fontc-0.0.2a2/fea-rs/src/compile.rs`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     error::{FontGlyphOrderError, GlyphOrderError},
 };
 
 #[cfg(feature = "norad")]
 use self::error::UfoGlyphOrderError;
 
 pub use compiler::Compiler;
-pub use feature_writer::{FeatureBuilder, FeatureProvider, NopFeatureProvider};
+pub use feature_writer::{FeatureBuilder, FeatureProvider, NopFeatureProvider, PendingLookup};
 pub use language_system::LanguageSystem;
 pub use lookups::{
     Builder, FeatureKey, LookupId, MarkToBaseBuilder, MarkToMarkBuilder, PairPosBuilder,
     PreviouslyAssignedClass,
 };
 pub use metrics::{Anchor, ValueRecord};
 pub use opts::Opts;
```

### Comparing `fontc-0.0.2a1/fea-rs/src/diagnostic.rs` & `fontc-0.0.2a2/fea-rs/src/diagnostic.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/lib.rs` & `fontc-0.0.2a2/fea-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/context.rs` & `fontc-0.0.2a2/fea-rs/src/parse/context.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/grammar/feature.rs` & `fontc-0.0.2a2/fea-rs/src/parse/grammar/feature.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/grammar/glyph.rs` & `fontc-0.0.2a2/fea-rs/src/parse/grammar/glyph.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/grammar/gpos.rs` & `fontc-0.0.2a2/fea-rs/src/parse/grammar/gpos.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/grammar/gsub.rs` & `fontc-0.0.2a2/fea-rs/src/parse/grammar/gsub.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/grammar/metrics.rs` & `fontc-0.0.2a2/fea-rs/src/parse/grammar/metrics.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/grammar/mod.rs` & `fontc-0.0.2a2/fea-rs/src/parse/grammar/mod.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/grammar/table.rs` & `fontc-0.0.2a2/fea-rs/src/parse/grammar/table.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/grammar/variations.rs` & `fontc-0.0.2a2/fea-rs/src/parse/grammar/variations.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/lexer/lexeme.rs` & `fontc-0.0.2a2/fea-rs/src/parse/lexer/lexeme.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/lexer/token_set.rs` & `fontc-0.0.2a2/fea-rs/src/parse/lexer/token_set.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/lexer.rs` & `fontc-0.0.2a2/fea-rs/src/parse/lexer.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/parser.rs` & `fontc-0.0.2a2/fea-rs/src/parse/parser.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/source.rs` & `fontc-0.0.2a2/fea-rs/src/parse/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse/tree.rs` & `fontc-0.0.2a2/fea-rs/src/parse/tree.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/parse.rs` & `fontc-0.0.2a2/fea-rs/src/parse.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/tests/compile.rs` & `fontc-0.0.2a2/fea-rs/src/tests/compile.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/tests/parse.rs` & `fontc-0.0.2a2/fea-rs/src/tests/parse.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/token_tree/cursor.rs` & `fontc-0.0.2a2/fea-rs/src/token_tree/cursor.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/token_tree/edit.rs` & `fontc-0.0.2a2/fea-rs/src/token_tree/edit.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/token_tree/rewrite.rs` & `fontc-0.0.2a2/fea-rs/src/token_tree/rewrite.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/token_tree/stack.rs` & `fontc-0.0.2a2/fea-rs/src/token_tree/stack.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/token_tree/token.rs` & `fontc-0.0.2a2/fea-rs/src/token_tree/token.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/token_tree/typed.rs` & `fontc-0.0.2a2/fea-rs/src/token_tree/typed.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/token_tree.rs` & `fontc-0.0.2a2/fea-rs/src/token_tree.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/util/highlighting.rs` & `fontc-0.0.2a2/fea-rs/src/util/highlighting.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/util/paths.rs` & `fontc-0.0.2a2/fea-rs/src/util/paths.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/util/pretty_diff.rs` & `fontc-0.0.2a2/fea-rs/src/util/pretty_diff.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/util/ttx.rs` & `fontc-0.0.2a2/fea-rs/src/util/ttx.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fea-rs/src/util.rs` & `fontc-0.0.2a2/fea-rs/src/util.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/Cargo.toml` & `fontc-0.0.2a2/glyphs-reader/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/build.rs` & `fontc-0.0.2a2/glyphs-reader/build.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/data/GlyphData.xml` & `fontc-0.0.2a2/glyphs-reader/data/GlyphData.xml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/data/GlyphData_Ideographs.xml` & `fontc-0.0.2a2/glyphs-reader/data/GlyphData_Ideographs.xml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/data/GlyphData_override_test.xml` & `fontc-0.0.2a2/glyphs-reader/data/GlyphData_override_test.xml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/data/update.py` & `fontc-0.0.2a2/glyphs-reader/data/update.py`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/src/error.rs` & `fontc-0.0.2a2/glyphs-reader/src/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/src/font.rs` & `fontc-0.0.2a2/glyphs-reader/src/font.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/src/glyphdata/glyphdata_impl.rs` & `fontc-0.0.2a2/glyphs-reader/src/glyphdata/glyphdata_impl.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/src/glyphdata.rs` & `fontc-0.0.2a2/glyphs-reader/src/glyphdata.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/src/plist.rs` & `fontc-0.0.2a2/glyphs-reader/src/plist.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/src/propagate_anchors.rs` & `fontc-0.0.2a2/glyphs-reader/src/propagate_anchors.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/Cargo.toml` & `fontc-0.0.2a2/fontbe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/avar.rs` & `fontc-0.0.2a2/fontbe/src/avar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/cmap.rs` & `fontc-0.0.2a2/fontbe/src/cmap.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/error.rs` & `fontc-0.0.2a2/fontbe/src/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/features/kern.rs` & `fontc-0.0.2a2/fontbe/src/features/kern.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,25 +40,23 @@
     },
     orchestration::{
         AllKerningPairs, AnyWorkId, BeWork, Context, FeaRsKerns, KernAdjustments, KernFragment,
         KernPair, KernSide, WorkId,
     },
 };
 
-use super::{properties::CharMap, PendingLookup};
+use super::{properties::CharMap, PendingLookup, DFLT_LANG, DFLT_SCRIPT};
 
 /// On Linux it took ~0.01 ms per loop, try to get enough to make fan out worthwhile
 /// based on empirical testing
 const KERNS_PER_BLOCK: usize = 2048;
 const KERN: Tag = Tag::new(b"kern");
 // we don't currently compile this feature, but we will, and it is referenced
 // in places because our impl is based on fonttools.
 const DIST: Tag = Tag::new(b"dist");
-const DFLT_SCRIPT: Tag = Tag::new(b"DFLT");
-const DFLT_LANG: Tag = Tag::new(b"dflt");
 
 /// Accumulation of all the kerning from IR
 #[derive(Debug)]
 struct GatherIrKerningWork;
 
 /// A fragment of the kerning from IR that can run in parallel with other fragments
 #[derive(Debug)]
@@ -579,15 +577,15 @@
 }
 
 fn debug_ordered_lookups(
     features: &BTreeMap<FeatureKey, Vec<usize>>,
     lookups: &[PendingLookup<PairPosBuilder>],
 ) {
     for (i, lookup) in lookups.iter().enumerate() {
-        let total_rules = lookup.subtables.iter().map(|x| x.len()).sum::<usize>();
+        let total_rules = lookup.subtables().iter().map(|x| x.len()).sum::<usize>();
         log::trace!("lookup {i}, {total_rules} rules");
     }
 
     let mut feature_keys = features.keys().collect::<Vec<_>>();
     feature_keys.sort();
     for feature in feature_keys {
         let indices = features.get(feature).unwrap();
@@ -1139,33 +1137,37 @@
 
         let latn: BTreeSet<_> = [LATN].into_iter().collect();
 
         let cyr_rules = result.get(&cyrillic).unwrap();
         assert_eq!(
             cyr_rules
                 .iter()
-                .flat_map(|x| x.subtables.iter().map(|sub| sub.len()))
+                .flat_map(|x| x.subtables().iter().map(|sub| sub.len()))
                 .sum::<usize>(),
             1
         );
 
         let latn_rules = result.get(&latn).unwrap();
         assert_eq!(
             latn_rules
                 .iter()
-                .flat_map(|x| x.subtables.iter().map(|sub| sub.len()))
+                .flat_map(|x| x.subtables().iter().map(|sub| sub.len()))
                 .sum::<usize>(),
             2
         );
     }
 
     fn flags_and_rule_count(lookup: &PendingLookup<PairPosBuilder>) -> (LookupFlag, usize) {
         (
-            lookup.flags,
-            lookup.subtables.iter().map(|sub| sub.len()).sum::<usize>(),
+            lookup.flags(),
+            lookup
+                .subtables()
+                .iter()
+                .map(|sub| sub.len())
+                .sum::<usize>(),
         )
     }
 
     #[test]
     fn mark_to_base_kern() {
         const ACUTE_COMB: char = '\u{0301}';
         let charmap: MockCharMap = ['A', 'B', 'C', ACUTE_COMB].into_iter().collect();
```

### Comparing `fontc-0.0.2a1/fontbe/src/features/marks.rs` & `fontc-0.0.2a2/fontbe/src/features/marks.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,63 @@
 //! Generates a [FeaRsMarks] datastructure to be fed to fea-rs
 
-use std::collections::{BTreeMap, BTreeSet, HashMap, HashSet};
+use std::collections::{BTreeMap, BTreeSet, HashSet};
 
-use fea_rs::compile::{MarkToBaseBuilder, MarkToMarkBuilder};
+use fea_rs::{
+    compile::{MarkToBaseBuilder, MarkToMarkBuilder, NopFeatureProvider, NopVariationInfo},
+    typed::{AstNode, LanguageSystem},
+    Opts, ParseTree,
+};
 use fontdrasil::{
     orchestration::{Access, AccessBuilder, Work},
     types::GlyphName,
 };
 
 use ordered_float::OrderedFloat;
 use smol_str::SmolStr;
 use write_fonts::{
     tables::gdef::GlyphClassDef,
     types::{GlyphId, Tag},
 };
 
 use crate::{
     error::Error,
-    orchestration::{AnyWorkId, BeWork, Context, FeaRsMarks, WorkId},
+    orchestration::{AnyWorkId, BeWork, Context, FeaAst, FeaRsMarks, WorkId},
 };
 use fontir::{
-    ir::{self, AnchorKind, GlyphAnchors, GlyphOrder, StaticMetadata},
+    ir::{self, Anchor, AnchorKind, GlyphAnchors, GlyphOrder, StaticMetadata},
     orchestration::WorkId as FeWorkId,
 };
 
+use super::DFLT_SCRIPT;
+
 #[derive(Debug)]
 struct MarkWork {}
 
 pub fn create_mark_work() -> Box<BeWork> {
     Box::new(MarkWork {})
 }
 
 /// The canonical name shared for a given mark/base pair, e.g. `top` for `top`/`_top`
 type MarkGroupName = SmolStr;
 
-#[allow(dead_code)] // a few currently unused fields
 struct MarkLookupBuilder<'a> {
-    gdef_classes: Option<HashMap<GlyphId, GlyphClassDef>>,
+    // extracted from public.openTypeCatgories/GlyphData.xml or FEA
+    gdef_classes: BTreeMap<GlyphName, GlyphClassDef>,
     // pruned, only the anchors we are using
-    anchors: BTreeMap<GlyphName, Vec<&'a ir::Anchor>>,
+    anchor_lists: BTreeMap<GlyphName, Vec<&'a ir::Anchor>>,
     glyph_order: &'a GlyphOrder,
     static_metadata: &'a StaticMetadata,
-    fea_scripts: HashSet<Tag>,
+    // we don't currently use this, because just adding lookups to all scripts works?
+    _fea_scripts: HashSet<Tag>,
+    mark_glyphs: BTreeSet<GlyphName>,
 }
 
 /// The bases and marks in a particular group, e.g. "top" or "bottom"
-#[derive(Default, Clone, PartialEq)]
+#[derive(Default, Debug, Clone, PartialEq)]
 struct MarkGroup<'a> {
     bases: Vec<(GlyphName, &'a ir::Anchor)>,
     marks: Vec<(GlyphName, &'a ir::Anchor)>,
 }
 
 // a trait to abstract over two very similar builders
 trait MarkAttachmentBuilder: Default {
@@ -79,63 +87,86 @@
     }
 }
 
 impl<'a> MarkLookupBuilder<'a> {
     fn new(
         anchors: Vec<&'a GlyphAnchors>,
         glyph_order: &'a GlyphOrder,
-        gdef_classes: Option<HashMap<GlyphId, GlyphClassDef>>,
+        gdef_classes: BTreeMap<GlyphName, GlyphClassDef>,
         static_metadata: &'a StaticMetadata,
+        fea_scripts: HashSet<Tag>,
     ) -> Self {
         // first we want to narrow our input down to only anchors that are participating.
+        // in pythonland this is https://github.com/googlefonts/ufo2ft/blob/8e9e6eb66a/Lib/ufo2ft/featureWriters/markFeatureWriter.py#L380
         let mut pruned = BTreeMap::new();
-        let mut base_names = HashSet::new();
-        let mut mark_names = HashSet::new();
+        let mut base_groups = HashSet::new();
+        let mut mark_groups = HashSet::new();
+        let include = gdef_classes
+            .iter()
+            .filter_map(|(name, cls)| {
+                matches!(
+                    *cls,
+                    GlyphClassDef::Base | GlyphClassDef::Mark | GlyphClassDef::Ligature
+                )
+                .then_some(name)
+            })
+            .collect::<HashSet<_>>();
         for anchors in anchors {
             // skip anchors for non-export glyphs
             if !glyph_order.contains(&anchors.glyph_name) {
                 continue;
             }
+            // skip glyphs that are not mark/lig/base, if we have any defined categories
+            if !include.is_empty() && !include.contains(&anchors.glyph_name) {
+                continue;
+            }
             for anchor in &anchors.anchors {
                 match &anchor.kind {
-                    AnchorKind::Base(group) => {
-                        base_names.insert(group);
+                    AnchorKind::Base(group)
+                    | AnchorKind::Ligature {
+                        group_name: group, ..
+                    } => {
+                        base_groups.insert(group);
                     }
                     AnchorKind::Mark(group) => {
-                        mark_names.insert(group);
+                        mark_groups.insert(group);
                     }
-                    //TODO: ligatures
                     // skip non base/mark anchors
                     _ => continue,
                 }
                 pruned
                     .entry(anchors.glyph_name.clone())
                     .or_insert(Vec::new())
                     .push(anchor);
             }
         }
 
-        let used_groups = base_names.intersection(&mark_names).collect::<HashSet<_>>();
+        let used_groups = base_groups
+            .intersection(&mark_groups)
+            .collect::<HashSet<_>>();
         // we don't care about marks with no corresponding bases, & vice-versa see:
         // <https://github.com/googlefonts/ufo2ft/blob/6787e37e63530/Lib/ufo2ft/featureWriters/markFeatureWriter.py#L359>
         pruned.retain(|_, anchors| {
             anchors.retain(|anchor| {
                 anchor
                     .mark_group_name()
                     .map(|group| used_groups.contains(&group))
                     .unwrap_or(false)
             });
             !anchors.is_empty()
         });
+
+        let mark_glyphs = find_mark_glyphs(&pruned, &gdef_classes);
         Self {
-            gdef_classes,
-            anchors: pruned,
+            anchor_lists: pruned,
             glyph_order,
-            fea_scripts: Default::default(),
+            _fea_scripts: fea_scripts,
             static_metadata,
+            gdef_classes,
+            mark_glyphs,
         }
     }
 
     fn build(&self) -> Result<FeaRsMarks, Error> {
         let mark_base_groups = self.make_mark_to_base_groups();
         let mark_mark_groups = self.make_mark_to_mark_groups();
 
@@ -150,20 +181,16 @@
 
     fn make_lookups<T: MarkAttachmentBuilder>(
         &self,
         groups: BTreeMap<MarkGroupName, MarkGroup>,
     ) -> Result<Vec<T>, Error> {
         groups
             .into_iter()
+            .filter(|(_, group)| !(group.bases.is_empty() || group.marks.is_empty()))
             .map(|(group_name, group)| {
-                assert!(
-                    !group.bases.is_empty() && !group.marks.is_empty(),
-                    "prechecked"
-                );
-
                 let mut builder = T::default();
                 for (mark_name, anchor) in group.marks {
                     // we already filtered to only things in glyph order
                     let gid = self.glyph_order.glyph_id(&mark_name).unwrap();
                     let anchor = resolve_anchor(anchor, self.static_metadata, &mark_name)?;
                     builder.add_mark(gid, &group_name, anchor);
                 }
@@ -177,54 +204,61 @@
                 Ok(builder)
             })
             .collect()
     }
 
     fn make_mark_to_base_groups(&self) -> BTreeMap<MarkGroupName, MarkGroup<'a>> {
         let mut groups = BTreeMap::<_, MarkGroup>::new();
-        for (glyph_name, anchors) in &self.anchors {
+        for (glyph_name, anchors) in &self.anchor_lists {
+            let is_mark = self.mark_glyphs.contains(glyph_name);
+            // if we have explicit gdef classes and this is not an expilcit base
+            let is_not_base = !self.gdef_classes.is_empty()
+                && (self.gdef_classes.get(glyph_name)) != Some(&GlyphClassDef::Base);
+
+            let treat_as_base = !(is_mark | is_not_base);
             for anchor in anchors {
                 match &anchor.kind {
-                    fontir::ir::AnchorKind::Base(group) => groups
+                    fontir::ir::AnchorKind::Base(group) if treat_as_base => groups
                         .entry(group.clone())
                         .or_default()
                         .bases
                         .push((glyph_name.clone(), anchor)),
-                    fontir::ir::AnchorKind::Mark(group) => groups
+                    fontir::ir::AnchorKind::Mark(group) if is_mark => groups
                         .entry(group.clone())
                         .or_default()
                         .marks
                         .push((glyph_name.clone(), anchor)),
                     _ => continue,
                 }
             }
         }
         groups
     }
 
     fn make_mark_to_mark_groups(&self) -> BTreeMap<MarkGroupName, MarkGroup<'a>> {
         // first find the set of glyphs that are marks, i.e. have any mark attachment point.
         let (mark_glyphs, mark_anchors): (BTreeSet<_>, BTreeSet<_>) = self
-            .anchors
+            .anchor_lists
             .iter()
+            .filter(|(name, _)| self.mark_glyphs.contains(*name))
             .flat_map(|(name, anchors)| {
-                anchors.iter().filter_map(|anchor| {
+                anchors.iter().filter_map(move |anchor| {
                     if let AnchorKind::Mark(group) = &anchor.kind {
-                        Some((name.clone(), group.clone()))
+                        Some((name, group))
                     } else {
                         None
                     }
                 })
             })
             .unzip();
 
         // then iterate again, looking for glyphs that we have identified as marks,
         // but which also have participating base anchors
         let mut result = BTreeMap::<MarkGroupName, MarkGroup>::new();
-        for (glyph, glyph_anchors) in &self.anchors {
+        for (glyph, glyph_anchors) in &self.anchor_lists {
             if !mark_glyphs.contains(glyph) {
                 continue;
             }
 
             for anchor in glyph_anchors {
                 if let AnchorKind::Base(group) = &anchor.kind {
                     // only if this anchor is a base, AND we have a mark in the same group
@@ -237,15 +271,15 @@
                     }
                 }
             }
         }
 
         // then add the anchors for the mark glyphs, if they exist
         for mark in mark_glyphs {
-            let anchors = self.anchors.get(&mark).unwrap();
+            let anchors = self.anchor_lists.get(mark).unwrap();
             for anchor in anchors {
                 if let AnchorKind::Mark(group) = &anchor.kind {
                     // only add mark glyph if there is at least one base
                     if let Some(group) = result.get_mut(group) {
                         group.marks.push((mark.clone(), anchor))
                     }
                 }
@@ -260,38 +294,111 @@
         WorkId::Marks.into()
     }
 
     fn read_access(&self) -> Access<AnyWorkId> {
         AccessBuilder::new()
             .variant(FeWorkId::StaticMetadata)
             .variant(FeWorkId::GlyphOrder)
+            .variant(WorkId::FeaturesAst)
             .variant(FeWorkId::ALL_ANCHORS)
             .build()
     }
 
     /// Generate mark data structures.
     fn exec(&self, context: &Context) -> Result<(), Error> {
         let static_metadata = context.ir.static_metadata.get();
         let glyph_order = context.ir.glyph_order.get();
         let raw_anchors = context.ir.anchors.all();
+        let ast = context.fea_ast.get();
+        let gdef_classes = get_gdef_classes(&static_metadata, &ast, &glyph_order);
 
         let anchors = raw_anchors
             .iter()
             .map(|(_, anchors)| anchors.as_ref())
             .collect::<Vec<_>>();
 
-        let ctx = MarkLookupBuilder::new(anchors, &glyph_order, None, &static_metadata);
+        let fea_scripts = get_fea_scripts(&ast.ast);
+        // this code is roughly equivalent to what in pythonland happens in
+        // setContext: https://github.com/googlefonts/ufo2ft/blob/8e9e6eb66a/Lib/ufo2ft/featureWriters/markFeatureWriter.py#L322
+        let ctx = MarkLookupBuilder::new(
+            anchors,
+            &glyph_order,
+            gdef_classes,
+            &static_metadata,
+            fea_scripts,
+        );
         let all_marks = ctx.build()?;
 
         context.fea_rs_marks.set(all_marks);
 
         Ok(())
     }
 }
 
+// in py this is set during _groupMarkGlyphsByAnchor; we try to match that logic
+// https://github.com/googlefonts/ufo2ft/blob/8e9e6eb66/Lib/ufo2ft/featureWriters/markFeatureWriter.py#L412
+fn find_mark_glyphs(
+    anchors: &BTreeMap<GlyphName, Vec<&Anchor>>,
+    gdef_classes: &BTreeMap<GlyphName, GlyphClassDef>,
+) -> BTreeSet<GlyphName> {
+    anchors
+        .iter()
+        .filter(|(name, anchors)| {
+            (!gdef_classes.is_empty() && gdef_classes.get(*name) == Some(&GlyphClassDef::Mark))
+                && anchors.iter().any(|a| a.is_mark())
+        })
+        .map(|(name, _)| name.to_owned())
+        .collect()
+}
+
+fn get_fea_scripts(ast: &ParseTree) -> HashSet<Tag> {
+    ast.typed_root()
+        .statements()
+        .filter_map(LanguageSystem::cast)
+        .map(|langsys| langsys.script().to_raw())
+        .filter(|tag| *tag != DFLT_SCRIPT)
+        .collect()
+}
+
+fn get_gdef_classes(
+    meta: &StaticMetadata,
+    ast: &FeaAst,
+    glyph_order: &GlyphOrder,
+) -> BTreeMap<GlyphName, GlyphClassDef> {
+    let glyph_map = glyph_order.iter().cloned().collect();
+    // if we prefer classes defined in fea, compile the fea and see if we have any
+    if meta.gdef_categories.prefer_gdef_categories_in_fea {
+        if let Some(gdef_classes) =
+            fea_rs::compile::compile::<NopVariationInfo, NopFeatureProvider>(
+                &ast.ast,
+                &glyph_map,
+                None,
+                None,
+                Opts::new().compile_gpos(false),
+            )
+            .ok()
+            .and_then(|mut comp| comp.0.gdef_classes.take())
+        {
+            return gdef_classes
+                .into_iter()
+                .filter_map(|(g, cls)| {
+                    glyph_order
+                        .glyph_name(g.to_u16() as _)
+                        .cloned()
+                        .map(|name| (name, cls))
+                })
+                .collect();
+        }
+    }
+    // otherwise (we don't care about FEA or nothing is defined) we use the
+    // classes in StaticMetadata (which are from public.openTypeCategories or
+    // GlyphData.xml)
+    meta.gdef_categories.categories.clone()
+}
+
 fn resolve_anchor(
     anchor: &fontir::ir::Anchor,
     static_metadata: &StaticMetadata,
     glyph_name: &GlyphName, // just used for error reporting
 ) -> Result<fea_rs::compile::Anchor, Error> {
     let (x_values, y_values): (Vec<_>, Vec<_>) = anchor
         .positions
```

### Comparing `fontc-0.0.2a1/fontbe/src/features/ot_tags.rs` & `fontc-0.0.2a2/fontbe/src/features/ot_tags.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/features/properties.rs` & `fontc-0.0.2a2/fontbe/src/features/properties.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/features.rs` & `fontc-0.0.2a2/fontbe/src/features.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,18 @@
     time::Instant,
 };
 
 use log::{debug, error, trace, warn};
 use ordered_float::OrderedFloat;
 
 use fea_rs::{
-    compile::{error::CompilerError, Compilation, FeatureBuilder, FeatureProvider, VariationInfo},
+    compile::{
+        error::CompilerError, Compilation, FeatureBuilder, FeatureProvider, PendingLookup,
+        VariationInfo,
+    },
     parse::{FileSystemResolver, SourceLoadError, SourceResolver},
     DiagnosticSet, GlyphMap, Opts, ParseTree,
 };
 
 use fontir::{
     ir::{FeaturesSource, GlyphOrder, StaticMetadata},
     orchestration::{Flags, WorkId as FeWorkId},
@@ -36,24 +39,25 @@
 };
 
 use crate::{
     error::Error,
     orchestration::{AnyWorkId, BeWork, Context, FeaAst, FeaRsKerns, FeaRsMarks, WorkId},
 };
 
-mod common;
 mod kern;
 mod marks;
 mod ot_tags;
 mod properties;
 
-pub(crate) use common::PendingLookup;
 pub use kern::{create_gather_ir_kerning_work, create_kern_segment_work, create_kerns_work};
 pub use marks::create_mark_work;
 
+const DFLT_SCRIPT: Tag = Tag::new(b"DFLT");
+const DFLT_LANG: Tag = Tag::new(b"dflt");
+
 #[derive(Debug)]
 pub struct FeatureParsingWork {}
 
 #[derive(Debug)]
 pub struct FeatureCompilationWork {}
 
 // I did not want to make a struct
@@ -217,21 +221,15 @@
             return Ok(());
         }
         // convert the lookups into lookup ids
         let lookup_ids = self
             .kerning
             .lookups
             .iter()
-            .map(|lookup| {
-                builder.add_lookup(
-                    lookup.flags,
-                    lookup.mark_filter_set.clone(),
-                    lookup.subtables.clone(),
-                )
-            })
+            .map(|lookup| builder.add_lookup(lookup.clone()))
             .collect::<Vec<_>>();
 
         for (feature, ids) in &self.kerning.features {
             // get the generated lookup ids based on the stored lookup indices
             let ids = ids.iter().map(|idx| lookup_ids[*idx]).collect();
             builder.add_feature(*feature, ids);
         }
@@ -267,28 +265,28 @@
         // Build the actual mark base and mark mark constructs using fea-rs builders
 
         let mut mark_base_lookups = Vec::new();
         let mut mark_mark_lookups = Vec::new();
 
         for mark_base in marks.mark_base.iter() {
             // each mark to base it's own lookup, whch differs from fontmake
-            mark_base_lookups.push(builder.add_lookup(
-                LookupFlag::default(),
-                None,
+            mark_base_lookups.push(builder.add_lookup(PendingLookup::new(
                 vec![mark_base.to_owned()],
-            ));
+                LookupFlag::empty(),
+                None,
+            )));
         }
 
         // If a mark has anchors that are themselves marks what we got here is a mark to mark
         for mark_mark in marks.mark_mark.iter() {
-            mark_mark_lookups.push(builder.add_lookup(
+            mark_mark_lookups.push(builder.add_lookup(PendingLookup::new(
+                vec![mark_mark.to_owned()],
                 LookupFlag::default(),
                 None,
-                vec![mark_mark.to_owned()],
-            ));
+            )));
         }
 
         if !mark_base_lookups.is_empty() {
             builder.add_to_default_language_systems(Tag::new(b"mark"), &mark_base_lookups);
         }
         if !mark_mark_lookups.is_empty() {
             builder.add_to_default_language_systems(Tag::new(b"mkmk"), &mark_mark_lookups);
```

### Comparing `fontc-0.0.2a1/fontbe/src/font.rs` & `fontc-0.0.2a2/fontbe/src/font.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/fvar.rs` & `fontc-0.0.2a2/fontbe/src/fvar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/glyphs.rs` & `fontc-0.0.2a2/fontbe/src/glyphs.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/gvar.rs` & `fontc-0.0.2a2/fontbe/src/gvar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/head.rs` & `fontc-0.0.2a2/fontbe/src/head.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/hvar.rs` & `fontc-0.0.2a2/fontbe/src/hvar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/metrics_and_limits.rs` & `fontc-0.0.2a2/fontbe/src/metrics_and_limits.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/mvar.rs` & `fontc-0.0.2a2/fontbe/src/mvar.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/name.rs` & `fontc-0.0.2a2/fontbe/src/name.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/orchestration.rs` & `fontc-0.0.2a2/fontbe/src/orchestration.rs`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     io::{self, BufReader, BufWriter, Read, Write},
     path::{Path, PathBuf},
     sync::Arc,
 };
 
 use fea_rs::{
     compile::{
-        FeatureKey, MarkToBaseBuilder, MarkToMarkBuilder, PairPosBuilder,
+        FeatureKey, MarkToBaseBuilder, MarkToMarkBuilder, PairPosBuilder, PendingLookup,
         ValueRecord as ValueRecordBuilder,
     },
     GlyphMap, GlyphSet, ParseTree,
 };
 use fontdrasil::{
     coords::NormalizedLocation,
     orchestration::{Access, AccessControlList, Identifier, IdentifierDiscriminant, Work},
@@ -59,15 +59,15 @@
         variations::Tuple,
     },
     types::{F2Dot14, GlyphId, Tag},
     validate::Validate,
     FontWrite,
 };
 
-use crate::{error::Error, features::PendingLookup, paths::Paths};
+use crate::{error::Error, paths::Paths};
 
 type KernBlock = usize;
 
 /// Unique identifier of work.
 ///
 /// If there are no fields work is unique.
 /// Meant to be small and cheap to copy around.
```

### Comparing `fontc-0.0.2a1/fontbe/src/os2.rs` & `fontc-0.0.2a2/fontbe/src/os2.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/paths.rs` & `fontc-0.0.2a2/fontbe/src/paths.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/post.rs` & `fontc-0.0.2a2/fontbe/src/post.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/stat.rs` & `fontc-0.0.2a2/fontbe/src/stat.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontbe/src/test_util.rs` & `fontc-0.0.2a2/fontbe/src/test_util.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/Cargo.toml` & `fontc-0.0.2a2/fontdrasil/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/build.rs` & `fontc-0.0.2a2/fontdrasil/build.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/data/aglfn.txt` & `fontc-0.0.2a2/fontdrasil/data/aglfn.txt`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/data/glyphlist.txt` & `fontc-0.0.2a2/fontdrasil/data/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/src/agl.rs` & `fontc-0.0.2a2/fontdrasil/src/agl.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/src/coords.rs` & `fontc-0.0.2a2/fontdrasil/src/coords.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/src/orchestration.rs` & `fontc-0.0.2a2/fontdrasil/src/orchestration.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/src/paths.rs` & `fontc-0.0.2a2/fontdrasil/src/paths.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/src/piecewise_linear_map.rs` & `fontc-0.0.2a2/fontdrasil/src/piecewise_linear_map.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontdrasil/src/types.rs` & `fontc-0.0.2a2/fontdrasil/src/types.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs2fontir/Cargo.toml` & `fontc-0.0.2a2/glyphs2fontir/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs2fontir/src/source.rs` & `fontc-0.0.2a2/glyphs2fontir/src/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs2fontir/src/toir.rs` & `fontc-0.0.2a2/glyphs2fontir/src/toir.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/ufo2fontir/Cargo.toml` & `fontc-0.0.2a2/ufo2fontir/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/ufo2fontir/src/source.rs` & `fontc-0.0.2a2/ufo2fontir/src/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/ufo2fontir/src/toir.rs` & `fontc-0.0.2a2/ufo2fontir/src/toir.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/ufo2fontir/testdata/wght_var.designspace` & `fontc-0.0.2a2/ufo2fontir/testdata/wght_var.designspace`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontra2fontir/Cargo.toml` & `fontc-0.0.2a2/fontra2fontir/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontra2fontir/src/fontra.rs` & `fontc-0.0.2a2/fontra2fontir/src/fontra.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontra2fontir/src/source.rs` & `fontc-0.0.2a2/fontra2fontir/src/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontra2fontir/src/toir.rs` & `fontc-0.0.2a2/fontra2fontir/src/toir.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/Cargo.toml` & `fontc-0.0.2a2/fontir/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/src/error.rs` & `fontc-0.0.2a2/fontir/src/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/src/glyph.rs` & `fontc-0.0.2a2/fontir/src/glyph.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/src/ir.rs` & `fontc-0.0.2a2/fontir/src/ir.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1108,14 +1108,18 @@
         match &self.kind {
             AnchorKind::Base(group_name)
             | AnchorKind::Mark(group_name)
             | AnchorKind::Ligature { group_name, .. } => Some(group_name),
             _ => None,
         }
     }
+
+    pub fn is_mark(&self) -> bool {
+        matches!(self.kind, AnchorKind::Mark(_))
+    }
 }
 
 /// A type for building glyph anchors, reused by different backends
 #[derive(Debug, Clone)]
 pub struct AnchorBuilder {
     glyph_name: GlyphName,
     anchors: HashMap<SmolStr, HashMap<NormalizedLocation, Point>>,
```

### Comparing `fontc-0.0.2a1/fontir/src/orchestration.rs` & `fontc-0.0.2a2/fontir/src/orchestration.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/src/paths.rs` & `fontc-0.0.2a2/fontir/src/paths.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/src/serde.rs` & `fontc-0.0.2a2/fontir/src/serde.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/src/source.rs` & `fontc-0.0.2a2/fontir/src/source.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/src/stateset.rs` & `fontc-0.0.2a2/fontir/src/stateset.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontir/src/variations.rs` & `fontc-0.0.2a2/fontir/src/variations.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/plist_derive/src/attrs.rs` & `fontc-0.0.2a2/glyphs-reader/plist_derive/src/attrs.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/glyphs-reader/plist_derive/src/lib.rs` & `fontc-0.0.2a2/glyphs-reader/plist_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/Cargo.toml` & `fontc-0.0.2a2/fontc/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/args.rs` & `fontc-0.0.2a2/fontc/src/args.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/change_detector.rs` & `fontc-0.0.2a2/fontc/src/change_detector.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/config.rs` & `fontc-0.0.2a2/fontc/src/config.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/error.rs` & `fontc-0.0.2a2/fontc/src/error.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/lib.rs` & `fontc-0.0.2a2/fontc/src/lib.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/main.rs` & `fontc-0.0.2a2/fontc/src/main.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/timing.rs` & `fontc-0.0.2a2/fontc/src/timing.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/work.rs` & `fontc-0.0.2a2/fontc/src/work.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/fontc/src/workload.rs` & `fontc-0.0.2a2/fontc/src/workload.rs`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/Cargo.lock` & `fontc-0.0.2a2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "auto_impl"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7862e21c893d65a1650125d157eaeec691439379a1cee17ee49031b79236ada4"
@@ -338,15 +338,15 @@
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -474,15 +474,15 @@
 name = "displaydoc"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "dot2"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "855423f2158bcc73798b3b9a666ec4204597a72370dc91dbdb8e7f9519de8cc3"
@@ -769,15 +769,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -1029,15 +1029,15 @@
 [[package]]
 name = "icu_provider_macros"
 version = "1.4.0"
 source = "git+https://github.com/unicode-org/icu4x.git?rev=728eb44#728eb449584da57acc604466702a603c03a82e45"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "idna"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
@@ -1383,15 +1383,15 @@
 
 [[package]]
 name = "plist_derive"
 version = "0.1.0"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "plotters"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
@@ -1618,15 +1618,15 @@
  "cfg-if",
  "glob",
  "proc-macro2",
  "quote",
  "regex",
  "relative-path",
  "rustc_version",
- "syn 2.0.61",
+ "syn 2.0.63",
  "unicode-ident",
 ]
 
 [[package]]
 name = "rustc-demangle"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1703,15 +1703,15 @@
 name = "serde_derive"
 version = "1.0.201"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
@@ -1725,15 +1725,15 @@
 name = "serde_repr"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "serde_yaml"
 version = "0.9.34+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a8b1a1a2ebf674015cc02edccce75287f1a0130d394307b36743c2f5d504b47"
@@ -1812,32 +1812,32 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.61"
+version = "2.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c993ed8ccba56ae856363b1845da7266a7cb78e1d146c8a32d54b45a8b831fc9"
+checksum = "bf5be731623ca1a1fb7d8be6f261a3be6d3e2337b8a1f97be944d020c8fcb704"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "synstructure"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c8af7666ab7b6390ab78131fb5b0fce11d6b7a6951602017c35fa82800708971"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "temp-env"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96374855068f47402c3121c6eed88d29cb1de8f3ab27090e273e420bdabcf050"
@@ -1879,15 +1879,15 @@
 name = "thiserror-impl"
 version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2470041c06ec3ac1ab38d0356a6119054dedaea53e12fbefc0de730a1c08524"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
@@ -1975,15 +1975,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
 
 [[package]]
 name = "tokio-util"
 version = "0.6.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "36943ee01a6d67977dd3f84a5a1d2efeb4ada3a1ae771cadfaa535d9d9fc6507"
@@ -2156,15 +2156,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2178,15 +2178,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2422,15 +2422,15 @@
 [[package]]
 name = "yoke-derive"
 version = "0.7.3"
 source = "git+https://github.com/unicode-org/icu4x.git?rev=728eb44#728eb449584da57acc604466702a603c03a82e45"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
  "synstructure",
 ]
 
 [[package]]
 name = "zerofrom"
 version = "0.1.3"
 source = "git+https://github.com/unicode-org/icu4x.git?rev=728eb44#728eb449584da57acc604466702a603c03a82e45"
@@ -2441,15 +2441,15 @@
 [[package]]
 name = "zerofrom-derive"
 version = "0.1.3"
 source = "git+https://github.com/unicode-org/icu4x.git?rev=728eb44#728eb449584da57acc604466702a603c03a82e45"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
  "synstructure",
 ]
 
 [[package]]
 name = "zerovec"
 version = "0.10.1"
 source = "git+https://github.com/unicode-org/icu4x.git?rev=728eb44#728eb449584da57acc604466702a603c03a82e45"
@@ -2462,9 +2462,9 @@
 [[package]]
 name = "zerovec-derive"
 version = "0.10.1"
 source = "git+https://github.com/unicode-org/icu4x.git?rev=728eb44#728eb449584da57acc604466702a603c03a82e45"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.61",
+ "syn 2.0.63",
 ]
```

### Comparing `fontc-0.0.2a1/Cargo.toml` & `fontc-0.0.2a2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/pyproject.toml` & `fontc-0.0.2a2/pyproject.toml`

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
-version = "0.0.2a1"
+version = "0.0.2a2"
 # Ensure we use the workspace's top-level README.md for the sdist/wheel metadata
 # not the fontc crate's specific README.md
 readme = "README.md"
```

### Comparing `fontc-0.0.2a1/README.md` & `fontc-0.0.2a2/README.md`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/LICENSE` & `fontc-0.0.2a2/LICENSE`

 * *Files identical despite different names*

### Comparing `fontc-0.0.2a1/PKG-INFO` & `fontc-0.0.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fontc
-Version: 0.0.2a1
+Version: 0.0.2a2
 License-File: LICENSE
 Summary: A compiler for fonts.
 License: MIT/Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/googlefonts/fontc
 
 # fontc
```

