# Comparing `tmp/symbolica-0.4.0.tar.gz` & `tmp/symbolica-0.5.0.tar.gz`

## Comparing `symbolica-0.4.0.tar` & `symbolica-0.5.0.tar`

### file list

```diff
@@ -1,83 +1,87 @@
--rw-r--r--   0        0        0     1885 1970-01-01 00:00:00.000000 symbolica-0.4.0/Cargo.toml
--rw-r--r--   0     1000     1000      747 2024-04-15 13:33:10.000000 symbolica-0.4.0/.github/workflows/coverage.yml
--rw-r--r--   0     1000     1000     1118 2024-04-15 13:33:10.000000 symbolica-0.4.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0     1000     1000       19 2023-06-16 10:52:31.000000 symbolica-0.4.0/.gitignore
--rw-r--r--   0     1000     1000    34783 2024-04-15 13:34:00.000000 symbolica-0.4.0/Cargo.lock
--rw-r--r--   0     1000     1000      812 2023-09-07 13:11:55.000000 symbolica-0.4.0/License.md
--rw-r--r--   0     1000     1000     4118 2024-04-15 13:33:47.000000 symbolica-0.4.0/Readme.md
--rw-r--r--   0     1000     1000      422 2024-01-25 12:49:23.000000 symbolica-0.4.0/build.rs
--rw-r--r--   0     1000     1000      351 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/builder.rs
--rw-r--r--   0     1000     1000      730 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/coefficient_ring.rs
--rw-r--r--   0     1000     1000     1049 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/collect.rs
--rw-r--r--   0     1000     1000      414 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/derivative.rs
--rw-r--r--   0     1000     1000     1161 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/evaluate.rs
--rw-r--r--   0     1000     1000      170 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/expansion.rs
--rw-r--r--   0     1000     1000     3945 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/factorization.rs
--rw-r--r--   0     1000     1000     1447 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/fibonacci.rs
--rw-r--r--   0     1000     1000     2368 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/fuel_backend.rs
--rw-r--r--   0     1000     1000     1182 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/groebner_basis.rs
--rw-r--r--   0     1000     1000     1362 2024-03-18 08:47:11.000000 symbolica-0.4.0/examples/numerical_integration.rs
--rw-r--r--   0     1000     1000   191454 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/optimize.rs
--rw-r--r--   0     1000     1000   191166 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/optimize_multiple.rs
--rw-r--r--   0     1000     1000     1329 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/partial_fraction.rs
--rw-r--r--   0     1000     1000      622 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/partition.rs
--rw-r--r--   0     1000     1000     1332 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/pattern_match.rs
--rw-r--r--   0     1000     1000     2795 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/pattern_restrictions.rs
--rw-r--r--   0     1000     1000     1700 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/polynomial.rs
--rw-r--r--   0     1000     1000     1180 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/polynomial_gcd.rs
--rw-r--r--   0     1000     1000      306 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/rational_polynomial.rs
--rw-r--r--   0     1000     1000      678 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/rational_reconstruction.rs
--rw-r--r--   0     1000     1000      315 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/replace_all.rs
--rw-r--r--   0     1000     1000      796 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/replace_once.rs
--rw-r--r--   0     1000     1000     2402 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/solve_linear_system.rs
--rw-r--r--   0     1000     1000      607 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/streaming.rs
--rw-r--r--   0     1000     1000      267 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/taylor_series.rs
--rw-r--r--   0     1000     1000     1340 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/tree_replace.rs
--rw-r--r--   0     1000     1000      495 2024-04-15 13:33:10.000000 symbolica-0.4.0/examples/tree_walk.rs
--rw-r--r--   0     1000     1000    21600 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/api/cpp.rs
--rw-r--r--   0     1000     1000     7147 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/api/mathematica.rs
--rw-r--r--   0     1000     1000   187916 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/api/python.rs
--rw-r--r--   0     1000     1000      117 2023-09-07 13:11:55.000000 symbolica-0.4.0/src/api.rs
--rw-r--r--   0     1000     1000    15177 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/atom/coefficient.rs
--rw-r--r--   0     1000     1000    35254 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/atom/representation.rs
--rw-r--r--   0     1000     1000    28974 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/atom.rs
--rw-r--r--   0     1000     1000    34916 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/coefficient.rs
--rw-r--r--   0     1000     1000    16302 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/collect.rs
--rw-r--r--   0     1000     1000    10821 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/combinatorics.rs
--rw-r--r--   0     1000     1000    17673 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/derivative.rs
--rw-r--r--   0     1000     1000     8476 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/domains/algebraic_number.rs
--rw-r--r--   0     1000     1000    34619 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/domains/factorized_rational_polynomial.rs
--rw-r--r--   0     1000     1000    31997 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/domains/finite_field.rs
--rw-r--r--   0     1000     1000    20789 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/domains/float.rs
--rw-r--r--   0     1000     1000    48186 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/domains/integer.rs
--rw-r--r--   0     1000     1000    28850 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/domains/rational.rs
--rw-r--r--   0     1000     1000    45363 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/domains/rational_polynomial.rs
--rw-r--r--   0     1000     1000     3134 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/domains.rs
--rw-r--r--   0     1000     1000     6653 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/evaluate.rs
--rw-r--r--   0     1000     1000    11394 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/expand.rs
--rw-r--r--   0     1000     1000    90552 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/id.rs
--rw-r--r--   0     1000     1000    17826 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/lib.rs
--rw-r--r--   0     1000     1000    44215 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/normalize.rs
--rw-r--r--   0     1000     1000    40419 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/numerical_integration.rs
--rw-r--r--   0     1000     1000    46451 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/parser.rs
--rw-r--r--   0     1000     1000    71732 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/poly/evaluate.rs
--rw-r--r--   0     1000     1000   111965 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/poly/factor.rs
--rwxr-xr-x   0     1000     1000   112076 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/poly/gcd.rs
--rw-r--r--   0     1000     1000    33344 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/poly/groebner.rs
--rwxr-xr-x   0     1000     1000   117561 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/poly/polynomial.rs
--rw-r--r--   0     1000     1000    19317 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/poly/resultant.rs
--rw-r--r--   0     1000     1000    30216 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/poly/univariate.rs
--rw-r--r--   0     1000     1000    61378 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/poly.rs
--rw-r--r--   0     1000     1000    45304 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/printer.rs
--rw-r--r--   0     1000     1000     5986 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/solve.rs
--rw-r--r--   0     1000     1000    14133 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/state.rs
--rw-r--r--   0     1000     1000     5476 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/streaming.rs
--rw-r--r--   0     1000     1000    26269 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/tensors/matrix.rs
--rw-r--r--   0     1000     1000       16 2024-03-18 08:47:11.000000 symbolica-0.4.0/src/tensors.rs
--rw-r--r--   0     1000     1000    23550 2024-04-15 13:33:10.000000 symbolica-0.4.0/src/transformer.rs
--rw-r--r--   0     1000     1000      796 2024-01-25 12:49:23.000000 symbolica-0.4.0/src/utils.rs
--rw-r--r--   0     1000     1000    88323 2024-04-15 13:33:10.000000 symbolica-0.4.0/symbolica.pyi
--rw-r--r--   0     1000     1000     2298 2024-04-15 13:33:10.000000 symbolica-0.4.0/tests/pattern_matching.rs
--rw-r--r--   0     1000     1000   418688 2024-04-15 13:33:10.000000 symbolica-0.4.0/tests/rational_polynomial.rs
--rw-r--r--   0     1000     1000      755 2024-04-15 13:37:31.000000 symbolica-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 symbolica-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 symbolica-0.5.0/Cargo.toml
+-rw-r--r--   0     1000     1000      747 2024-04-15 13:33:10.000000 symbolica-0.5.0/.github/workflows/coverage.yml
+-rw-r--r--   0     1000     1000     1118 2024-04-15 13:33:10.000000 symbolica-0.5.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0     1000     1000       19 2023-06-16 10:52:31.000000 symbolica-0.5.0/.gitignore
+-rw-r--r--   0     1000     1000    35757 2024-05-13 10:09:46.000000 symbolica-0.5.0/Cargo.lock
+-rw-r--r--   0     1000     1000     6428 2024-05-13 10:07:07.000000 symbolica-0.5.0/Contributing.md
+-rw-r--r--   0     1000     1000      812 2023-09-07 13:11:55.000000 symbolica-0.5.0/License.md
+-rw-r--r--   0     1000     1000     4118 2024-05-13 10:09:18.000000 symbolica-0.5.0/Readme.md
+-rw-r--r--   0     1000     1000      422 2024-01-25 12:49:23.000000 symbolica-0.5.0/build.rs
+-rw-r--r--   0     1000     1000      351 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/builder.rs
+-rw-r--r--   0     1000     1000      730 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/coefficient_ring.rs
+-rw-r--r--   0     1000     1000     1049 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/collect.rs
+-rw-r--r--   0     1000     1000      414 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/derivative.rs
+-rw-r--r--   0     1000     1000     1161 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/evaluate.rs
+-rw-r--r--   0     1000     1000      170 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/expansion.rs
+-rw-r--r--   0     1000     1000     3945 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/factorization.rs
+-rw-r--r--   0     1000     1000     1447 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/fibonacci.rs
+-rw-r--r--   0     1000     1000     2368 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/fuel_backend.rs
+-rw-r--r--   0     1000     1000     1182 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/groebner_basis.rs
+-rw-r--r--   0     1000     1000     1362 2024-03-18 08:47:11.000000 symbolica-0.5.0/examples/numerical_integration.rs
+-rw-r--r--   0     1000     1000   191454 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/optimize.rs
+-rw-r--r--   0     1000     1000   191166 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/optimize_multiple.rs
+-rw-r--r--   0     1000     1000     1329 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/partial_fraction.rs
+-rw-r--r--   0     1000     1000      622 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/partition.rs
+-rw-r--r--   0     1000     1000     1332 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/pattern_match.rs
+-rw-r--r--   0     1000     1000     2795 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/pattern_restrictions.rs
+-rw-r--r--   0     1000     1000     1700 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/polynomial.rs
+-rw-r--r--   0     1000     1000     1180 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/polynomial_gcd.rs
+-rw-r--r--   0     1000     1000      306 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/rational_polynomial.rs
+-rw-r--r--   0     1000     1000      678 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/rational_reconstruction.rs
+-rw-r--r--   0     1000     1000      315 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/replace_all.rs
+-rw-r--r--   0     1000     1000      796 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/replace_once.rs
+-rw-r--r--   0     1000     1000      263 2024-05-13 10:07:07.000000 symbolica-0.5.0/examples/series.rs
+-rw-r--r--   0     1000     1000     2402 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/solve_linear_system.rs
+-rw-r--r--   0     1000     1000      711 2024-05-13 10:07:07.000000 symbolica-0.5.0/examples/streaming.rs
+-rw-r--r--   0     1000     1000     1340 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/tree_replace.rs
+-rw-r--r--   0     1000     1000      495 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/tree_walk.rs
+-rw-r--r--   0     1000     1000    21600 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/api/cpp.rs
+-rw-r--r--   0     1000     1000     7147 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/api/mathematica.rs
+-rw-r--r--   0     1000     1000   191049 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/api/python.rs
+-rw-r--r--   0     1000     1000      117 2023-09-07 13:11:55.000000 symbolica-0.5.0/src/api.rs
+-rw-r--r--   0     1000     1000    22708 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/atom/coefficient.rs
+-rw-r--r--   0     1000     1000    40768 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/atom/representation.rs
+-rw-r--r--   0     1000     1000    30720 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/atom.rs
+-rw-r--r--   0     1000     1000    35828 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/coefficient.rs
+-rw-r--r--   0     1000     1000    17680 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/collect.rs
+-rw-r--r--   0     1000     1000    10821 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/combinatorics.rs
+-rw-r--r--   0     1000     1000    24367 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/derivative.rs
+-rw-r--r--   0     1000     1000     8476 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/algebraic_number.rs
+-rw-r--r--   0     1000     1000     3704 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/domains/atom.rs
+-rw-r--r--   0     1000     1000    34619 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/factorized_rational_polynomial.rs
+-rw-r--r--   0     1000     1000    31997 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/finite_field.rs
+-rw-r--r--   0     1000     1000    20789 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/float.rs
+-rw-r--r--   0     1000     1000    48681 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/domains/integer.rs
+-rw-r--r--   0     1000     1000    28980 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/domains/rational.rs
+-rw-r--r--   0     1000     1000    45363 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/rational_polynomial.rs
+-rw-r--r--   0     1000     1000     3148 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/domains.rs
+-rw-r--r--   0     1000     1000     6653 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/evaluate.rs
+-rw-r--r--   0     1000     1000    12470 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/expand.rs
+-rw-r--r--   0     1000     1000    90392 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/id.rs
+-rw-r--r--   0     1000     1000    17802 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/lib.rs
+-rw-r--r--   0     1000     1000    49791 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/normalize.rs
+-rw-r--r--   0     1000     1000    40419 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/numerical_integration.rs
+-rw-r--r--   0     1000     1000    46095 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/parser.rs
+-rw-r--r--   0     1000     1000    71732 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/evaluate.rs
+-rw-r--r--   0     1000     1000   111965 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/factor.rs
+-rwxr-xr-x   0     1000     1000   112252 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/poly/gcd.rs
+-rw-r--r--   0     1000     1000    33344 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/groebner.rs
+-rwxr-xr-x   0     1000     1000   118681 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/poly/polynomial.rs
+-rw-r--r--   0     1000     1000    19317 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/resultant.rs
+-rw-r--r--   0     1000     1000    30161 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/poly/series.rs
+-rw-r--r--   0     1000     1000    30216 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/univariate.rs
+-rw-r--r--   0     1000     1000    61699 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/poly.rs
+-rw-r--r--   0     1000     1000    45472 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/printer.rs
+-rw-r--r--   0     1000     1000     5986 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/solve.rs
+-rw-r--r--   0     1000     1000    23961 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/state.rs
+-rw-r--r--   0     1000     1000    15822 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/streaming.rs
+-rw-r--r--   0     1000     1000    26269 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/tensors/matrix.rs
+-rw-r--r--   0     1000     1000       16 2024-03-18 08:47:11.000000 symbolica-0.5.0/src/tensors.rs
+-rw-r--r--   0     1000     1000    23774 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/transformer.rs
+-rw-r--r--   0     1000     1000      641 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/utils.rs
+-rw-r--r--   0     1000     1000    91441 2024-05-13 10:07:07.000000 symbolica-0.5.0/symbolica.pyi
+-rw-r--r--   0     1000     1000     1639 2024-05-13 10:07:07.000000 symbolica-0.5.0/tests/import_export.rs
+-rw-r--r--   0     1000     1000     2298 2024-04-15 13:33:10.000000 symbolica-0.5.0/tests/pattern_matching.rs
+-rw-r--r--   0     1000     1000   418688 2024-04-15 13:33:10.000000 symbolica-0.5.0/tests/rational_polynomial.rs
+-rw-r--r--   0     1000     1000      755 2024-05-13 10:09:18.000000 symbolica-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 symbolica-0.5.0/PKG-INFO
```

### Comparing `symbolica-0.4.0/Cargo.toml` & `symbolica-0.5.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 edition = "2021"
 keywords = ["algebra", "symbolic", "manipulation", "mathematics", "physics"]
 license-file = "License.md"
 name = "symbolica"
 readme = "Readme.md"
 repository = "https://github.com/benruijl/symbolica"
 rust-version = "1.73"
-version = "0.4.0"
+version = "0.5.0"
 
 [profile.release]
 codegen-units = 1
 lto = true
 
 [profile.dev-optim]
 inherits = "dev"
@@ -45,15 +45,17 @@
 [dependencies.rug]
 default-features = false
 features = ["integer", "rational"]
 version = "1.23"
 
 [dependencies]
 ahash = "0.8.7"
+append-only-vec = "0.1"
 bincode = {version = "1.3", optional = true}
+brotli = "5.0"
 byteorder = "1.5"
 bytes = "1.5"
 colored = "2.1"
 dyn-clone = "1.0"
 once_cell = "1.19"
 rand = "0.8.5"
 rand_xoshiro = "0.6"
@@ -63,8 +65,7 @@
 smallvec = "1.13"
 smartstring = "1.0"
 tikv-jemallocator = {version = "0.5.4", optional = true}
 tinyjson = "2.5"
 tracing = {version = "0.1", features = ["max_level_trace", "release_max_level_warn"]}
 wide = "0.7"
 wolfram-library-link = {version = "0.2.9", optional = true}
-append-only-vec = "0.1"
```

### Comparing `symbolica-0.4.0/.github/workflows/coverage.yml` & `symbolica-0.5.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/.github/workflows/publish_pypi.yml` & `symbolica-0.5.0/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/Cargo.lock` & `symbolica-0.5.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,29 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "alloc-no-stdlib"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cc7bb162ec39d46ab1ca8c77bf72e890535becd1751bb45f64c597edb4c8c6b3"
+
+[[package]]
+name = "alloc-stdlib"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94fb8275041c72129eb51b7d0322c29b8387a0386127718b096429201a5d6ece"
+dependencies = [
+ "alloc-no-stdlib",
+]
+
+[[package]]
 name = "append-only-vec"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3cb8f874ecf419dd8165d0279746de966cb8966636d028845e3bd65d519812a"
 
 [[package]]
 name = "autocfg"
@@ -90,14 +105,35 @@
 [[package]]
 name = "bitflags"
 version = "2.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
 
 [[package]]
+name = "brotli"
+version = "5.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19483b140a7ac7174d34b5a581b406c64f84da5409d3e09cf4fff604f9270e67"
+dependencies = [
+ "alloc-no-stdlib",
+ "alloc-stdlib",
+ "brotli-decompressor",
+]
+
+[[package]]
+name = "brotli-decompressor"
+version = "4.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6221fe77a248b9117d431ad93761222e1cf8ff282d9d1d5d9f53d6299a1cf76"
+dependencies = [
+ "alloc-no-stdlib",
+ "alloc-stdlib",
+]
+
+[[package]]
 name = "bytemuck"
 version = "1.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed2490600f404f2b94c167e31d3ed1d5f3c225a0f3b80230053b3e0b7b962bd9"
 
 [[package]]
 name = "byteorder"
@@ -794,19 +830,20 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "symbolica"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "ahash",
  "append-only-vec",
  "bincode",
+ "brotli",
  "byteorder",
  "bytes",
  "colored",
  "dyn-clone",
  "once_cell",
  "pyo3",
  "rand",
```

### Comparing `symbolica-0.4.0/License.md` & `symbolica-0.5.0/License.md`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/Readme.md` & `symbolica-0.5.0/Readme.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ## Rust
 
 If you want to use Symbolica as a library in Rust, simply include it in the `Cargo.toml`:
 
 ```toml
 [dependencies]
-symbolica = "0.4"
+symbolica = "0.5"
 ```
 
 # Examples
 
 Below we list some examples of the features of Symbolica. Check the [guide](https://symbolica.io/docs/) for a complete overview.
 
 ### Pattern matching
```

#### html2text {}

```diff
@@ -14,15 +14,15 @@
 (probably) already know, by using Symbolica's bindings to Python, Rust and C++:
 [A demo of Symbolica]# Installation Visit the [Get Started](https://
 symbolica.io/docs/get_started.html) page for detailed installation
 instructions. ## Python Symbolica can be installed for Python >3.5 using `pip`:
 ```sh pip install symbolica ``` The installation may take some time on Mac OS
 and Windows, as it may have to compile Symbolica. ## Rust If you want to use
 Symbolica as a library in Rust, simply include it in the `Cargo.toml`: ```toml
-[dependencies] symbolica = "0.4" ``` # Examples Below we list some examples of
+[dependencies] symbolica = "0.5" ``` # Examples Below we list some examples of
 the features of Symbolica. Check the [guide](https://symbolica.io/docs/) for a
 complete overview. ### Pattern matching Variables ending with a `_` are
 wildcards that match to any subexpression. In the following example we try to
 match the pattern `f(w1_,w2_)`: ```python from symbolica import Expression x,
 y, w1_, w2_ = Expression.vars('x','y','w1_','w2_') f = Expression.fun('f') e =
 f(3,x)*y**2+5 r = e.replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2)) print(r) ```
 which yields `y^2*f(2,x^2)+5`. ### Solving a linear system Solve a linear
```

### Comparing `symbolica-0.4.0/examples/coefficient_ring.rs` & `symbolica-0.5.0/examples/coefficient_ring.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/collect.rs` & `symbolica-0.5.0/examples/collect.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/evaluate.rs` & `symbolica-0.5.0/examples/evaluate.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/factorization.rs` & `symbolica-0.5.0/examples/factorization.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/fibonacci.rs` & `symbolica-0.5.0/examples/fibonacci.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/fuel_backend.rs` & `symbolica-0.5.0/examples/fuel_backend.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/groebner_basis.rs` & `symbolica-0.5.0/examples/groebner_basis.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/numerical_integration.rs` & `symbolica-0.5.0/examples/numerical_integration.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/optimize.rs` & `symbolica-0.5.0/examples/optimize.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/optimize_multiple.rs` & `symbolica-0.5.0/examples/optimize_multiple.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/partial_fraction.rs` & `symbolica-0.5.0/examples/partial_fraction.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/partition.rs` & `symbolica-0.5.0/examples/partition.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/pattern_match.rs` & `symbolica-0.5.0/examples/pattern_match.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/pattern_restrictions.rs` & `symbolica-0.5.0/examples/pattern_restrictions.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/polynomial.rs` & `symbolica-0.5.0/examples/polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/polynomial_gcd.rs` & `symbolica-0.5.0/examples/polynomial_gcd.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/rational_reconstruction.rs` & `symbolica-0.5.0/examples/rational_reconstruction.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/replace_once.rs` & `symbolica-0.5.0/examples/replace_once.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/solve_linear_system.rs` & `symbolica-0.5.0/examples/solve_linear_system.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/examples/tree_replace.rs` & `symbolica-0.5.0/examples/tree_replace.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/api/cpp.rs` & `symbolica-0.5.0/src/api/cpp.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/api/mathematica.rs` & `symbolica-0.5.0/src/api/mathematica.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/api/python.rs` & `symbolica-0.5.0/src/api/python.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,92 @@
 use std::{
     borrow::Borrow,
+    fs::File,
     hash::{Hash, Hasher},
-    ops::Neg,
+    io::BufWriter,
+    ops::{Deref, Neg},
     sync::Arc,
 };
 
 use ahash::HashMap;
+use brotli::CompressorWriter;
 use pyo3::{
     exceptions::{self, PyIndexError},
     pyclass,
     pyclass::CompareOp,
     pyfunction, pymethods, pymodule,
     types::{PyBytes, PyComplex, PyLong, PyModule, PyTuple, PyType},
     wrap_pyfunction, FromPyObject, IntoPy, PyErr, PyObject, PyRef, PyResult, Python,
 };
 use rug::Complete;
 use self_cell::self_cell;
 use smallvec::SmallVec;
 use smartstring::{LazyCompact, SmartString};
 
 use crate::{
-    atom::{Atom, AtomView, ListIterator, Symbol},
+    atom::{Atom, AtomType, AtomView, ListIterator, Symbol},
     domains::{
+        atom::AtomField,
         finite_field::{ToFiniteField, Zp},
         float::Complex,
         integer::{Integer, IntegerRing, Z},
         rational::{Rational, RationalField, Q},
         rational_polynomial::{
             FromNumeratorAndDenominator, RationalPolynomial, RationalPolynomialField,
         },
         Ring,
     },
     evaluate::EvaluationFn,
     id::{
-        AtomType, Condition, Match, MatchSettings, MatchStack, Pattern, PatternAtomTreeIterator,
+        Condition, Match, MatchSettings, MatchStack, Pattern, PatternAtomTreeIterator,
         PatternRestriction, ReplaceIterator, WildcardAndRestriction,
     },
     numerical_integration::{ContinuousGrid, DiscreteGrid, Grid, MonteCarloRng, Sample},
     parser::Token,
     poly::{
         evaluate::{
             InstructionEvaluator, InstructionSetMode, InstructionSetModeCPPSettings,
             InstructionSetPrinter,
         },
         factor::Factorize,
         groebner::GroebnerBasis,
         polynomial::MultivariatePolynomial,
+        series::Series,
         GrevLexOrder, LexOrder, Variable, INLINED_EXPONENTS,
     },
     printer::{
         AtomPrinter, MatrixPrinter, PolynomialPrinter, PrintOptions, RationalPolynomialPrinter,
     },
     state::{FunctionAttribute, RecycledAtom, State, Workspace},
-    streaming::TermStreamer,
+    streaming::{TermStreamer, TermStreamerConfig},
     tensors::matrix::Matrix,
     transformer::{StatsOptions, Transformer, TransformerError},
     LicenseManager,
 };
 
 #[pymodule]
 fn symbolica(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<PythonExpression>()?;
-    m.add_class::<PythonFunction>()?;
     m.add_class::<PythonPattern>()?;
     m.add_class::<PythonPolynomial>()?;
     m.add_class::<PythonIntegerPolynomial>()?;
     m.add_class::<PythonFiniteFieldPolynomial>()?;
     m.add_class::<PythonRationalPolynomial>()?;
     m.add_class::<PythonRationalPolynomialSmallExponent>()?;
     m.add_class::<PythonFiniteFieldRationalPolynomial>()?;
     m.add_class::<PythonMatrix>()?;
     m.add_class::<PythonNumericalIntegrator>()?;
     m.add_class::<PythonSample>()?;
     m.add_class::<PythonAtomType>()?;
     m.add_class::<PythonAtomTree>()?;
     m.add_class::<PythonInstructionEvaluator>()?;
     m.add_class::<PythonRandomNumberGenerator>()?;
+    m.add_class::<PythonPatternRestriction>()?;
+    m.add_class::<PythonTermStreamer>()?;
+    m.add_class::<PythonSeries>()?;
 
     m.add_function(wrap_pyfunction!(get_version, m)?)?;
     m.add_function(wrap_pyfunction!(is_licensed, m)?)?;
     m.add_function(wrap_pyfunction!(set_license_key, m)?)?;
     m.add_function(wrap_pyfunction!(request_hobbyist_license, m)?)?;
     m.add_function(wrap_pyfunction!(request_trial_license, m)?)?;
     m.add_function(wrap_pyfunction!(request_sublicense, m)?)?;
@@ -144,15 +151,15 @@
 #[pyfunction]
 fn get_offline_license_key() -> PyResult<String> {
     LicenseManager::get_offline_license_key().map_err(exceptions::PyValueError::new_err)
 }
 
 /// Specifies the type of the atom.
 #[derive(Clone, Copy)]
-#[pyclass(name = "AtomType")]
+#[pyclass(name = "AtomType", module = "symbolica")]
 pub enum PythonAtomType {
     Num,
     Var,
     Fn,
     Add,
     Mul,
     Pow,
@@ -169,15 +176,15 @@
 ///
 /// The tail contains the child atoms:
 /// - the summand for type `Add`
 /// - the factors for type `Mul`
 /// - the base and exponent for type `Pow`
 /// - the function arguments for type `Fn`
 #[derive(Clone)]
-#[pyclass(name = "AtomTree")]
+#[pyclass(name = "AtomTree", module = "symbolica")]
 pub struct PythonAtomTree {
     /// The type of this atom.
     #[pyo3(get)]
     pub atom_type: PythonAtomType,
     /// The string data of this atom.
     #[pyo3(get)]
     pub head: Option<String>,
@@ -236,92 +243,99 @@
     Literal(ConvertibleToExpression),
     Pattern(PythonPattern),
 }
 
 impl ConvertibleToPattern {
     pub fn to_pattern(self) -> PyResult<PythonPattern> {
         match self {
-            Self::Literal(l) => Ok(PythonPattern {
-                expr: Arc::new(l.to_expression().expr.as_view().into_pattern()),
-            }),
+            Self::Literal(l) => Ok(l.to_expression().expr.as_view().into_pattern().into()),
             Self::Pattern(e) => Ok(e),
         }
     }
 }
 
 /// Operations that transform an expression.
-#[pyclass(name = "Transformer")]
+#[pyclass(name = "Transformer", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonPattern {
-    pub expr: Arc<Pattern>,
+    pub expr: Pattern,
+}
+
+impl From<Pattern> for PythonPattern {
+    fn from(expr: Pattern) -> Self {
+        PythonPattern { expr }
+    }
 }
 
 macro_rules! append_transformer {
     ($self:ident,$t:expr) => {
         if let Pattern::Transformer(b) = $self.expr.borrow() {
             let mut t = b.clone();
             t.1.push($t);
-            Ok(PythonPattern {
-                expr: Arc::new(Pattern::Transformer(t)),
-            })
+            Ok(Pattern::Transformer(t).into())
         } else {
             // pattern is not a transformer yet (but may have subtransformers)
-            Ok(PythonPattern {
-                expr: Arc::new(Pattern::Transformer(Box::new((
-                    Some($self.expr.as_ref().clone()),
-                    vec![$t],
-                )))),
-            })
+            Ok(Pattern::Transformer(Box::new((Some($self.expr.clone()), vec![$t]))).into())
         }
     };
 }
 
 #[pymethods]
 impl PythonPattern {
     /// Create a new transformer for a term provided by `Expression.map`.
     #[new]
     pub fn new() -> PythonPattern {
-        PythonPattern {
-            expr: Arc::new(Pattern::Transformer(Box::new((None, vec![])))),
-        }
+        Pattern::Transformer(Box::new((None, vec![]))).into()
     }
 
     /// Create a transformer that expands products and powers.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x, x_ = Expression.vars('x', 'x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x, x_ = Expression.symbols('x', 'x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f((x+1)**2).replace_all(f(x_), x_.transform().expand())
     /// >>> print(e)
-    pub fn expand(&self) -> PyResult<PythonPattern> {
-        return append_transformer!(self, Transformer::Expand);
+    pub fn expand(&self, var: Option<ConvertibleToExpression>) -> PyResult<PythonPattern> {
+        if let Some(var) = var {
+            let id = if let AtomView::Var(x) = var.to_expression().expr.as_view() {
+                x.get_symbol()
+            } else {
+                return Err(exceptions::PyValueError::new_err(
+                    "Expansion must be done wrt a variable or function name",
+                ));
+            };
+
+            return append_transformer!(self, Transformer::Expand(Some(id)));
+        } else {
+            return append_transformer!(self, Transformer::Expand(None));
+        }
     }
 
     /// Create a transformer that computes the product of a list of arguments.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x__ = Expression.var('x__')
-    /// >>> f = Expression.fun('f')
+    /// >>> x__ = Expression.symbol('x__')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(2,3).replace_all(f(x__), x__.transform().prod())
     /// >>> print(e)
     pub fn prod(&self) -> PyResult<PythonPattern> {
         return append_transformer!(self, Transformer::Product);
     }
 
     /// Create a transformer that computes the sum of a list of arguments.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x__ = Expression.var('x__')
-    /// >>> f = Expression.fun('f')
+    /// >>> x__ = Expression.symbol('x__')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(2,3).replace_all(f(x__), x__.transform().sum())
     /// >>> print(e)
     pub fn sum(&self) -> PyResult<PythonPattern> {
         return append_transformer!(self, Transformer::Sum);
     }
 
     /// Create a transformer that returns the number of arguments.
@@ -330,44 +344,44 @@
     /// If `only_for_arg_fun` is `True`, only count the number of arguments
     /// in the `arg()` function and return 1 if the input is not `arg`.
     /// This is useful for obtaining the length of a range during pattern matching.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x__ = Expression.var('x__')
-    /// >>> f = Expression.fun('f')
+    /// >>> x__ = Expression.symbol('x__')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(2,3,4).replace_all(f(x__), x__.transform().nargs())
     /// >>> print(e)
     #[pyo3(signature = (only_for_arg_fun = false))]
     pub fn nargs(&self, only_for_arg_fun: bool) -> PyResult<PythonPattern> {
         return append_transformer!(self, Transformer::ArgCount(only_for_arg_fun));
     }
 
     /// Create a transformer that sorts a list of arguments.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(3,2,1).replace_all(f(x_), x_.transform().sort())
     /// >>> print(e)
     pub fn sort(&self) -> PyResult<PythonPattern> {
         return append_transformer!(self, Transformer::Sort);
     }
 
     /// Create a transformer that removes elements from a list if they occur
     /// earlier in the list as well.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x__ = Expression.var('x__')
-    /// >>> f = Expression.fun('f')
+    /// >>> x__ = Expression.symbol('x__')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(1,2,1,2).replace_all(f(x__), x__.transform().deduplicate())
     /// >>> print(e)
     ///
     /// Yields `f(1,2)`.
     pub fn deduplicate(&self) -> PyResult<PythonPattern> {
         return append_transformer!(self, Transformer::Deduplicate);
     }
@@ -384,16 +398,16 @@
     }
 
     /// Create a transformer that split a sum or product into a list of arguments.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x, x__ = Expression.vars('x', 'x__')
-    /// >>> f = Expression.fun('f')
+    /// >>> x, x__ = Expression.symbols('x', 'x__')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = (x + 1).replace_all(x__, f(x__.transform().split()))
     /// >>> print(e)
     pub fn split(&self) -> PyResult<PythonPattern> {
         return append_transformer!(self, Transformer::Split);
     }
 
     /// Create a transformer that partitions a list of arguments into named bins of a given length,
@@ -406,16 +420,16 @@
     /// if possible.
     ///
     /// Note that the functions names to be provided for the bin names must be generated through `Expression.var`.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x_, f_id, g_id = Expression.vars('x_', 'f', 'g')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_, f_id, g_id = Expression.symbols('x__', 'f', 'g')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(1,2,1,3).replace_all(f(x_), x_.transform().partitions([(f_id, 2), (g_id, 1), (f_id, 1)]))
     /// >>> print(e)
     ///
     /// yields:
     /// ```
     /// 2*f(1)*f(1,2)*g(3)+2*f(1)*f(1,3)*g(2)+2*f(1)*f(2,3)*g(1)+f(2)*f(1,1)*g(3)+2*f(2)*f(1,3)*g(1)+f(3)*f(1,1)*g(2)+2*f(3)*f(1,2)*g(1)
     /// ```
@@ -425,15 +439,15 @@
         bins: Vec<(ConvertibleToPattern, usize)>,
         fill_last: bool,
         repeat: bool,
     ) -> PyResult<PythonPattern> {
         let mut conv_bins = vec![];
 
         for (x, len) in bins {
-            let id = match &*x.to_pattern()?.expr {
+            let id = match &x.to_pattern()?.expr {
                 Pattern::Literal(x) => {
                     if let AtomView::Var(x) = x.as_view() {
                         x.get_symbol()
                     } else {
                         return Err(exceptions::PyValueError::new_err(
                             "Derivative must be taken wrt a variable",
                         ));
@@ -454,25 +468,25 @@
     }
 
     /// Create a transformer that generates all permutations of a list of arguments.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x_, f_id = Expression.vars('x_', 'f')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_, f_id = Expression.symbols('x__', 'f')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(1,2,1,2).replace_all(f(x_), x_.transform().permutations(f_id))
     /// >>> print(e)
     ///
     /// yields:
     /// ```
     /// 4*f(1,1,2,2)+4*f(1,2,1,2)+4*f(1,2,2,1)+4*f(2,1,1,2)+4*f(2,1,2,1)+4*f(2,2,1,1)
     /// ```
     pub fn permutations(&self, function_name: ConvertibleToPattern) -> PyResult<PythonPattern> {
-        let id = match &*function_name.to_pattern()?.expr {
+        let id = match &function_name.to_pattern()?.expr {
             Pattern::Literal(x) => {
                 if let AtomView::Var(x) = x.as_view() {
                     x.get_symbol()
                 } else {
                     return Err(exceptions::PyValueError::new_err(
                         "Derivative must be taken wrt a variable",
                     ));
@@ -490,22 +504,22 @@
     }
 
     /// Create a transformer that apply a function `f`.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, Transformer
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(2).replace_all(f(x_), x_.transform().map(lambda r: r**2))
     /// >>> print(e)
     pub fn map(&self, f: PyObject) -> PyResult<PythonPattern> {
         let transformer = Transformer::Map(Box::new(move |expr, out| {
             let expr = PythonExpression {
-                expr: Arc::new(expr.to_owned()),
+                expr: expr.to_owned(),
             };
 
             let res = Python::with_gil(|py| {
                 f.call(py, (expr,), None)
                     .map_err(|e| {
                         TransformerError::ValueError(format!("Bad callback function: {}", e))
                     })?
@@ -532,16 +546,16 @@
 
     /// Create a transformer that applies a transformer chain to every argument of the `arg()` function.
     /// If the input is not `arg()`, the transformer is applied to the input.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x = Expression.var('x')
-    /// >>> f = Expression.fun('f')
+    /// >>> x = Expression.symbol('x')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = (1+x).transform().split().for_each(Transformer().map(f)).execute()
     #[pyo3(signature = (*transformers))]
     pub fn for_each(&self, transformers: &PyTuple) -> PyResult<PythonPattern> {
         let mut rep_chain = vec![];
         // fuse all sub-transformers into one chain
         for r in transformers {
             let p = r.extract::<PythonPattern>()?;
@@ -566,16 +580,16 @@
 
     /// Create a transformer that checks for a Python interrupt,
     /// such as ctrl-c and aborts the current transformer.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import *
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> f(10).transform().repeat(Transformer().replace_all(
     /// >>> f(x_), f(x_+1)).check_interrupt()).execute()
     pub fn check_interrupt(&self) -> PyResult<PythonPattern> {
         let transformer = Transformer::Map(Box::new(move |expr, out| {
             out.set_from_view(&expr);
             Python::with_gil(|py| py.check_signals()).map_err(|_| TransformerError::Interrupt)
         }));
@@ -584,16 +598,16 @@
     }
 
     /// Create a transformer that keeps executing the transformer chain until the input equals the output.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = Expression.parse("f(5)")
     /// >>> e = e.transform().repeat(
     /// >>>     Transformer().expand(),
     /// >>>     Transformer().replace_all(f(x_), f(x_ - 1) + f(x_ - 2), x_.req_gt(1))
     /// >>> ).execute()
     #[pyo3(signature = (*transformers))]
     pub fn repeat(&self, transformers: &PyTuple) -> PyResult<PythonPattern> {
@@ -622,16 +636,16 @@
 
     /// Chain several transformers. `chain(A,B,C)` is the same as `A.B.C`,
     /// where `A`, `B`, `C` are transformers.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = Expression.parse("f(5)")
     /// >>> e = e.transform().repeat(
     /// >>>     Transformer().expand(),
     /// >>>     Transformer().replace_all(f(x_), f(x_ - 1) + f(x_ - 2), x_.req_gt(1))
     /// >>> ).execute()
     #[pyo3(signature = (*transformers))]
     pub fn chain(&self, transformers: &PyTuple) -> PyResult<PythonPattern> {
@@ -652,30 +666,28 @@
                         "Transformers in a repeat must be unbound. Use Transformer() to create it.",
                     ));
                 }
 
                 ts.1.extend_from_slice(&t.1);
             }
 
-            Ok(PythonPattern {
-                expr: Arc::new(Pattern::Transformer(ts)),
-            })
+            Ok(Pattern::Transformer(ts).into())
         } else {
             Err(exceptions::PyValueError::new_err(
                 "Pattern must be a transformer",
             ))
         }
     }
 
     /// Execute the transformer.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x = Expression.var('x')
+    /// >>> x = Expression.symbol('x')
     /// >>> e = (x+1)**5
     /// >>> e = e.transform().expand().execute()
     /// >>> print(e)
     pub fn execute(&self) -> PyResult<PythonExpression> {
         let mut out = Atom::default();
         Workspace::get_local()
             .with(|workspace| {
@@ -688,22 +700,20 @@
             .map_err(|e| match e {
                 TransformerError::Interrupt => {
                     exceptions::PyKeyboardInterrupt::new_err("Interrupted by user")
                 }
                 TransformerError::ValueError(v) => exceptions::PyValueError::new_err(v),
             })?;
 
-        Ok(PythonExpression {
-            expr: Arc::new(out),
-        })
+        Ok(out.into())
     }
 
     /// Create a transformer that derives `self` w.r.t the variable `x`.
     pub fn derivative(&self, x: ConvertibleToPattern) -> PyResult<PythonPattern> {
-        let id = match &*x.to_pattern()?.expr {
+        let id = match &x.to_pattern()?.expr {
             Pattern::Literal(x) => {
                 if let AtomView::Var(x) = x.as_view() {
                     x.get_symbol()
                 } else {
                     return Err(exceptions::PyValueError::new_err(
                         "Derivative must be taken wrt a variable",
                     ));
@@ -716,48 +726,54 @@
                 ))
             }
         };
 
         return append_transformer!(self, Transformer::Derivative(id));
     }
 
-    /// Create a transformer that Taylor expands in `x` around `expansion_point` to depth `depth`.
-    pub fn taylor_series(
+    /// Create a transformer that series expands in `x` around `expansion_point` to depth `depth`.
+    #[pyo3(signature = (x, expansion_point, depth, depth_denom = 1))]
+    pub fn series(
         &self,
         x: ConvertibleToExpression,
         expansion_point: ConvertibleToExpression,
-        depth: u32,
+        depth: i64,
+        depth_denom: i64,
     ) -> PyResult<PythonPattern> {
         let id = if let AtomView::Var(x) = x.to_expression().expr.as_view() {
             x.get_symbol()
         } else {
             return Err(exceptions::PyValueError::new_err(
                 "Derivative must be taken wrt a variable",
             ));
         };
 
         return append_transformer!(
             self,
-            Transformer::TaylorSeries(id, (*expansion_point.to_expression().expr).clone(), depth,)
+            Transformer::Series(
+                id,
+                expansion_point.to_expression().expr.clone(),
+                (depth, depth_denom).into(),
+            )
         );
     }
 
     /// Create a transformer that replaces all patterns matching the left-hand side `self` by the right-hand side `rhs`.
     /// Restrictions on pattern can be supplied through `cond`. The settings `non_greedy_wildcards` can be used to specify
     /// wildcards that try to match as little as possible.
     ///
     /// The `level_range` specifies the `[min,max]` level at which the pattern is allowed to match.
     /// The first level is 0 and the level is increased when going into a function or one level deeper in the expression tree,
     /// depending on `level_is_tree_depth`.
     ///
     /// Examples
     /// --------
     ///
-    /// >>> x, w1_, w2_ = Expression.vars('x','w1_','w2_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x, w1_, w2_ = Expression.symbols('x','w1_','w2_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(3,x)
     /// >>> r = e.transform().replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2), (w1_ >= 1) & w2_.is_var())
     /// >>> print(r)
     pub fn replace_all(
         &self,
         lhs: ConvertibleToPattern,
         rhs: ConvertibleToPattern,
@@ -793,18 +809,17 @@
         if let Some(level_is_tree_depth) = level_is_tree_depth {
             settings.level_is_tree_depth = level_is_tree_depth;
         }
 
         return append_transformer!(
             self,
             Transformer::ReplaceAll(
-                (*lhs.to_pattern()?.expr).clone(),
-                (*rhs.to_pattern()?.expr).clone(),
-                cond.map(|r| r.condition.as_ref().clone())
-                    .unwrap_or_default(),
+                lhs.to_pattern()?.expr.clone(),
+                rhs.to_pattern()?.expr.clone(),
+                cond.map(|r| r.condition.clone()).unwrap_or_default(),
                 settings,
             )
         );
     }
 
     /// Create a transformer that prints the expression.
     ///
@@ -857,16 +872,16 @@
     }
 
     /// Print statistics of a transformer, tagging it with `tag`.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = Expression.parse("f(5)")
     /// >>> e = e.transform().stats('replace', Transformer().replace_all(f(x_), 1)).execute()
     ///
     /// yields
     /// ```log
     /// Stats for replace:
     ///     In  │ 1 │  10.00 B │
@@ -906,17 +921,15 @@
 
     /// Add this transformer to `other`, returning the result.
     pub fn __add__(&self, rhs: ConvertibleToPattern) -> PyResult<PythonPattern> {
         let res = Workspace::get_local().with(|workspace| {
             Ok::<Pattern, PyErr>(self.expr.add(&rhs.to_pattern()?.expr, workspace))
         })?;
 
-        Ok(PythonPattern {
-            expr: Arc::new(res),
-        })
+        Ok(res.into())
     }
 
     /// Add this transformer to `other`, returning the result.
     pub fn __radd__(&self, rhs: ConvertibleToPattern) -> PyResult<PythonPattern> {
         self.__add__(rhs)
     }
 
@@ -933,33 +946,29 @@
 
     /// Add this transformer to `other`, returning the result.
     pub fn __mul__(&self, rhs: ConvertibleToPattern) -> PyResult<PythonPattern> {
         let res = Workspace::get_local().with(|workspace| {
             Ok::<Pattern, PyErr>(self.expr.mul(&rhs.to_pattern()?.expr, workspace))
         });
 
-        Ok(PythonPattern {
-            expr: Arc::new(res?),
-        })
+        Ok(res?.into())
     }
 
     /// Add this transformer to `other`, returning the result.
     pub fn __rmul__(&self, rhs: ConvertibleToPattern) -> PyResult<PythonPattern> {
         self.__mul__(rhs)
     }
 
     /// Divide this transformer by `other`, returning the result.
     pub fn __truediv__(&self, rhs: ConvertibleToPattern) -> PyResult<PythonPattern> {
         let res = Workspace::get_local().with(|workspace| {
             Ok::<Pattern, PyErr>(self.expr.div(&rhs.to_pattern()?.expr, workspace))
         });
 
-        Ok(PythonPattern {
-            expr: Arc::new(res?),
-        })
+        Ok(res?.into())
     }
 
     /// Divide `other` by this transformer, returning the result.
     pub fn __rtruediv__(&self, rhs: ConvertibleToPattern) -> PyResult<PythonPattern> {
         rhs.to_pattern()?
             .__truediv__(ConvertibleToPattern::Pattern(self.clone()))
     }
@@ -975,17 +984,15 @@
                 "Optional number argument not supported",
             ));
         }
 
         let res = Workspace::get_local()
             .with(|workspace| Ok::<_, PyErr>(self.expr.pow(&rhs.to_pattern()?.expr, workspace)));
 
-        Ok(PythonPattern {
-            expr: Arc::new(res?),
-        })
+        Ok(res?.into())
     }
 
     /// Take `base` to power `self`, returning the result.
     pub fn __rpow__(
         &self,
         rhs: ConvertibleToPattern,
         number: Option<i64>,
@@ -1009,81 +1016,108 @@
     }
 
     /// Negate the current transformer, returning the result.
     pub fn __neg__(&self) -> PyResult<PythonPattern> {
         let res =
             Workspace::get_local().with(|workspace| Ok::<Pattern, PyErr>(self.expr.neg(workspace)));
 
-        Ok(PythonPattern {
-            expr: Arc::new(res?),
-        })
+        Ok(res?.into())
     }
 }
 
 /// A Symbolica expression.
 ///
 /// Supports standard arithmetic operations, such
 /// as addition and multiplication.
 ///
 /// Examples
 /// --------
-/// >>> x = Expression.var('x')
+/// >>> x = Expression.symbol('x')
 /// >>> e = x**2 + 2 - x + 1 / x**4
 /// >>> print(e)
-#[pyclass(name = "Expression")]
+///
+/// Attributes
+/// ----------
+/// E: Expression
+///     Euler's number `e`.
+/// PI: Expression
+///     The mathematical constant `π`.
+/// I: Expression
+///     The mathematical constant `i`, where `i^2 = -1`.
+/// COEFF: Expression
+///     The built-in function that converts a rational polynomial to a coefficient.
+/// COS: Expression
+///     The built-in cosine function.
+/// SIN: Expression
+///     The built-in sine function.
+/// EXP: Expression
+///     The built-in exponential function.
+/// LOG: Expression
+///     The built-in logarithm function.
+#[pyclass(name = "Expression", module = "symbolica")]
 #[derive(Clone, PartialEq, Eq, Hash)]
 pub struct PythonExpression {
-    pub expr: Arc<Atom>,
+    pub expr: Atom,
+}
+
+impl From<Atom> for PythonExpression {
+    fn from(expr: Atom) -> Self {
+        PythonExpression { expr }
+    }
+}
+
+impl Deref for PythonExpression {
+    type Target = Atom;
+
+    fn deref(&self) -> &Self::Target {
+        &self.expr
+    }
 }
 
 /// A restriction on wildcards.
-#[pyclass(name = "PatternRestriction")]
+#[pyclass(name = "PatternRestriction", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonPatternRestriction {
-    pub condition: Arc<Condition<WildcardAndRestriction>>,
+    pub condition: Condition<WildcardAndRestriction>,
+}
+
+impl From<Condition<WildcardAndRestriction>> for PythonPatternRestriction {
+    fn from(condition: Condition<WildcardAndRestriction>) -> Self {
+        PythonPatternRestriction { condition }
+    }
 }
 
 #[pymethods]
 impl PythonPatternRestriction {
     /// Create a new pattern restriction that is the logical 'and' operation between two restrictions (i.e., both should hold).
     pub fn __and__(&self, other: Self) -> PythonPatternRestriction {
-        PythonPatternRestriction {
-            condition: Arc::new(self.condition.as_ref().clone() & other.condition.as_ref().clone()),
-        }
+        (self.condition.clone() & other.condition.clone()).into()
     }
 
     /// Create a new pattern restriction that is the logical 'or' operation between two restrictions (i.e., one of the two should hold).
     pub fn __or__(&self, other: Self) -> PythonPatternRestriction {
-        PythonPatternRestriction {
-            condition: Arc::new(self.condition.as_ref().clone() | other.condition.as_ref().clone()),
-        }
+        (self.condition.clone() | other.condition.clone()).into()
     }
 
     /// Create a new pattern restriction that takes the logical 'not' of the current restriction.
     pub fn __invert__(&self) -> PythonPatternRestriction {
-        PythonPatternRestriction {
-            condition: Arc::new(!self.condition.as_ref().clone()),
-        }
+        (!self.condition.clone()).into()
     }
 }
 
 impl<'a> FromPyObject<'a> for ConvertibleToExpression {
     fn extract(ob: &'a pyo3::PyAny) -> PyResult<Self> {
         if let Ok(a) = ob.extract::<PythonExpression>() {
             Ok(ConvertibleToExpression(a))
         } else if let Ok(num) = ob.extract::<i64>() {
-            Ok(ConvertibleToExpression(PythonExpression {
-                expr: Arc::new(Atom::new_num(num)),
-            }))
+            Ok(ConvertibleToExpression(Atom::new_num(num).into()))
         } else if let Ok(num) = ob.extract::<&PyLong>() {
             let a = format!("{}", num);
             let i = Integer::from_large(rug::Integer::parse(&a).unwrap().complete());
-            Ok(ConvertibleToExpression(PythonExpression {
-                expr: Arc::new(Atom::new_num(i)),
-            }))
+            Ok(ConvertibleToExpression(Atom::new_num(i).into()))
         } else {
             Err(exceptions::PyValueError::new_err(
                 "Cannot convert to expression",
             ))
         }
     }
 }
@@ -1094,16 +1128,14 @@
             match a.expr.as_view() {
                 AtomView::Var(v) => Ok(v.get_symbol()),
                 e => Err(exceptions::PyValueError::new_err(format!(
                     "Expected variable instead of {}",
                     e
                 ))),
             }
-        } else if let Ok(a) = ob.extract::<PythonFunction>() {
-            Ok(a.id)
         } else {
             Err(exceptions::PyValueError::new_err("Not a valid variable"))
         }
     }
 }
 
 impl<'a> FromPyObject<'a> for Variable {
@@ -1150,35 +1182,33 @@
                 if v.get_wildcard_level() == 0 {
                     return Err(exceptions::PyTypeError::new_err(
                         "Only wildcards can be restricted.",
                     ));
                 }
 
                 Ok(PythonPatternRestriction {
-                    condition: Arc::new(
-                        (
-                            name,
-                            PatternRestriction::Filter(Box::new(move |v: &Match| {
-                                let k = num.expr.as_view();
-
-                                if let Match::Single(m) = v {
-                                    if !$cmp_any_atom {
-                                        if let AtomView::Num(_) = m {
-                                            return m.cmp(&k).$c();
-                                        }
-                                    } else {
+                    condition: (
+                        name,
+                        PatternRestriction::Filter(Box::new(move |v: &Match| {
+                            let k = num.expr.as_view();
+
+                            if let Match::Single(m) = v {
+                                if !$cmp_any_atom {
+                                    if let AtomView::Num(_) = m {
                                         return m.cmp(&k).$c();
                                     }
+                                } else {
+                                    return m.cmp(&k).$c();
                                 }
+                            }
 
-                                false
-                            })),
-                        )
-                            .into(),
-                    ),
+                            false
+                        })),
+                    )
+                        .into(),
                 })
             }
             _ => Err(exceptions::PyTypeError::new_err(
                 "Only wildcards can be restricted.",
             )),
         }
     }};
@@ -1217,123 +1247,138 @@
                 return Err(exceptions::PyTypeError::new_err(
                     "Only wildcards can be restricted.",
                 ));
             }
         };
 
         Ok(PythonPatternRestriction {
-            condition: Arc::new(
-                (
-                    id,
-                    PatternRestriction::Cmp(
-                        other_id,
-                        Box::new(move |m1: &Match, m2: &Match| {
-                            if let Match::Single(a1) = m1 {
-                                if let Match::Single(a2) = m2 {
-                                    if !$cmp_any_atom {
-                                        if let AtomView::Num(_) = a1 {
-                                            if let AtomView::Num(_) = a2 {
-                                                return a1.cmp(a2).$c();
-                                            }
+            condition: (
+                id,
+                PatternRestriction::Cmp(
+                    other_id,
+                    Box::new(move |m1: &Match, m2: &Match| {
+                        if let Match::Single(a1) = m1 {
+                            if let Match::Single(a2) = m2 {
+                                if !$cmp_any_atom {
+                                    if let AtomView::Num(_) = a1 {
+                                        if let AtomView::Num(_) = a2 {
+                                            return a1.cmp(a2).$c();
                                         }
-                                    } else {
-                                        return a1.cmp(a2).$c();
                                     }
+                                } else {
+                                    return a1.cmp(a2).$c();
                                 }
                             }
-                            false
-                        }),
-                    ),
-                )
-                    .into(),
-            ),
+                        }
+                        false
+                    }),
+                ),
+            )
+                .into(),
         })
     }};
 }
 
 #[pymethods]
 impl PythonExpression {
-    /// Create a Symbolica expression that is a single variable.
+    /// Create a new symbol from a `name`. Symbols carry information about their attributes.
+    /// The symbol can signal that it is symmetric if it is used as a function
+    /// using `is_symmetric=True`, antisymmetric using `is_antisymmetric=True`, and
+    /// multilinear using `is_linear=True`. If no attributes
+    /// are specified, the attributes are inherited from the symbol if it was already defined,
+    /// otherwise all attributes are set to `false`.
     ///
-    /// Examples
-    /// --------
-    /// >>> var_x = Expression.var('x')
-    /// >>> print(var_x)
-    /// x
-    ///
-    #[classmethod]
-    pub fn var(_cls: &PyType, name: &str) -> PyResult<PythonExpression> {
-        // TODO: check if the name meets the requirements
-        let id = State::get_symbol(name);
-        let var = Atom::new_var(id);
-
-        Ok(PythonExpression {
-            expr: Arc::new(var),
-        })
-    }
-
-    /// Create a Symbolica variable for every name in `*names`.
-    #[pyo3(signature = (*args,))]
-    #[classmethod]
-    pub fn vars(_cls: &PyType, args: &PyTuple) -> PyResult<Vec<PythonExpression>> {
-        let mut result = Vec::with_capacity(args.len());
-
-        for a in args {
-            // TODO: check if the name meets the requirements
-            let name = a.extract::<&str>()?;
-            let id = State::get_symbol(name);
-            let var = Atom::new_var(id);
-
-            result.push(PythonExpression {
-                expr: Arc::new(var),
-            });
-        }
-
-        Ok(result)
-    }
-
-    /// Create a new Symbolica function with a given name.
+    /// Once attributes are defined on a symbol, they cannot be redefined later.
     ///
     /// Examples
     /// --------
-    /// >>> f = Expression.fun('f')
+    /// Define a regular symbol and use it as a variable:
+    /// >>> f = Expression.symbol('x')
+    /// >>> e = x**2 + 5
+    /// >>> print(e)
+    /// x**2 + 5
+    ///
+    /// Define a regular symbol and use it as a function:
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(1,2)
     /// >>> print(e)
     /// f(1,2)
     ///
     /// Define a symmetric function:
-    /// >>> f = Expression.fun('f', is_symmetric=True)
+    /// >>> f = Expression.symbol('f', is_symmetric=True)
     /// >>> e = f(2,1)
     /// >>> print(e)
     /// f(1,2)
     ///
     /// Define a linear and symmetric function:
-    /// >>> p1, p2, p3, p4 = Expression.vars('p1', 'p2', 'p3', 'p4')
-    /// >>> dot = Expression.fun('dot', is_symmetric=True, is_linear=True)
+    /// >>> p1, p2, p3, p4 = Expression.symbols('p1', 'p2', 'p3', 'p4')
+    /// >>> dot = Expression.symbol('dot', is_symmetric=True, is_linear=True)
     /// >>> e = dot(p2+2*p3,p1+3*p2-p3)
     /// dot(p1,p2)+2*dot(p1,p3)+3*dot(p2,p2)-dot(p2,p3)+6*dot(p2,p3)-2*dot(p3,p3)
     #[classmethod]
-    pub fn fun(
+    pub fn symbol(
         _cls: &PyType,
         name: &str,
         is_symmetric: Option<bool>,
         is_antisymmetric: Option<bool>,
         is_linear: Option<bool>,
-    ) -> PyResult<PythonFunction> {
-        PythonFunction::__new__(name, is_symmetric, is_antisymmetric, is_linear)
+    ) -> PyResult<Self> {
+        if is_symmetric.is_none() && is_antisymmetric.is_none() && is_linear.is_none() {
+            return Ok(Atom::new_var(State::get_symbol(name)).into());
+        }
+
+        if is_symmetric == Some(true) && is_antisymmetric == Some(true) {
+            Err(exceptions::PyValueError::new_err(
+                "Function cannot be both symmetric and antisymmetric",
+            ))?;
+        }
+
+        let mut opts = vec![];
+
+        if let Some(true) = is_symmetric {
+            opts.push(FunctionAttribute::Symmetric);
+        }
+
+        if let Some(true) = is_antisymmetric {
+            opts.push(FunctionAttribute::Antisymmetric);
+        }
+
+        if let Some(true) = is_linear {
+            opts.push(FunctionAttribute::Linear);
+        }
+
+        let id = State::get_symbol_with_attributes(name, &opts)
+            .map_err(|e| exceptions::PyTypeError::new_err(e.to_string()))?;
+
+        Ok(Atom::new_var(id).into())
     }
 
-    /// Create a Symbolica function for every name in `*names`.
-    #[pyo3(signature = (*args,))]
+    /// Create a Symbolica symbol for every name in `*names`. See `Expression.symbol` for more information.
+    ///
+    /// Examples
+    /// --------
+    /// >>> f, x = Expression.symbols('x', 'f')
+    /// >>> e = f(1,x)
+    /// >>> print(e)
+    /// f(1,x)
+    #[pyo3(signature = (*args,is_symmetric=None,is_antisymmetric=None,is_linear=None))]
     #[classmethod]
-    pub fn funs(_cls: &PyType, args: &PyTuple) -> PyResult<Vec<PythonFunction>> {
+    pub fn symbols(
+        cls: &PyType,
+        args: &PyTuple,
+        is_symmetric: Option<bool>,
+        is_antisymmetric: Option<bool>,
+        is_linear: Option<bool>,
+    ) -> PyResult<Vec<PythonExpression>> {
         let mut result = Vec::with_capacity(args.len());
+
         for a in args {
             let name = a.extract::<&str>()?;
-            result.push(PythonFunction::__new__(name, None, None, None)?);
+            let s = Self::symbol(cls, name, is_symmetric, is_antisymmetric, is_linear)?;
+            result.push(s);
         }
 
         Ok(result)
     }
 
     /// Create a new Symbolica number from an int or a float.
     /// A floating point number is converted to its rational number equivalent,
@@ -1353,102 +1398,123 @@
     pub fn num(
         _cls: &PyType,
         py: Python,
         num: PyObject,
         max_denom: Option<usize>,
     ) -> PyResult<PythonExpression> {
         if let Ok(num) = num.extract::<i64>(py) {
-            Ok(PythonExpression {
-                expr: Arc::new(Atom::new_num(num)),
-            })
+            Ok(Atom::new_num(num).into())
         } else if let Ok(num) = num.extract::<&PyLong>(py) {
             let a = format!("{}", num);
             PythonExpression::parse(_cls, &a)
         } else if let Ok(f) = num.extract::<f64>(py) {
             if !f.is_finite() {
                 return Err(exceptions::PyValueError::new_err("Number must be finite"));
             }
 
             let mut r: Rational = f.into();
             if let Some(max_denom) = max_denom {
                 r = r.truncate_denominator(&(max_denom as u64).into())
             }
 
-            Ok(PythonExpression {
-                expr: Arc::new(Atom::new_num(r)),
-            })
+            Ok(Atom::new_num(r).into())
         } else {
             Err(exceptions::PyValueError::new_err("Not a valid number"))
         }
     }
 
     /// Euler's number `e`.
     #[classattr]
     #[pyo3(name = "E")]
     pub fn e() -> PythonExpression {
-        PythonExpression {
-            expr: Arc::new(Atom::new_var(State::E)),
-        }
+        Atom::new_var(State::E).into()
     }
 
     /// The mathematical constant `π`.
     #[classattr]
     #[pyo3(name = "PI")]
     pub fn pi() -> PythonExpression {
-        PythonExpression {
-            expr: Arc::new(Atom::new_var(State::PI)),
-        }
+        Atom::new_var(State::PI).into()
     }
 
     /// The mathematical constant `i`, where
     /// `i^2 = -1`.
     #[classattr]
     #[pyo3(name = "I")]
     pub fn i() -> PythonExpression {
-        PythonExpression {
-            expr: Arc::new(Atom::new_var(State::I)),
-        }
+        Atom::new_var(State::I).into()
+    }
+
+    /// The built-in function that converts a rational polynomial to a coefficient.
+    #[classattr]
+    #[pyo3(name = "COEFF")]
+    pub fn coeff() -> PythonExpression {
+        Atom::new_var(State::COEFF).into()
+    }
+
+    /// The built-in cosine function.
+    #[classattr]
+    #[pyo3(name = "COS")]
+    pub fn cos() -> PythonExpression {
+        Atom::new_var(State::COS).into()
+    }
+
+    /// The built-in sine function.
+    #[classattr]
+    #[pyo3(name = "SIN")]
+    pub fn sin() -> PythonExpression {
+        Atom::new_var(State::SIN).into()
+    }
+
+    /// The built-in exponential function.
+    #[classattr]
+    #[pyo3(name = "EXP")]
+    pub fn exp() -> PythonExpression {
+        Atom::new_var(State::EXP).into()
+    }
+
+    /// The built-in logarithm function.
+    #[classattr]
+    #[pyo3(name = "LOG")]
+    pub fn log() -> PythonExpression {
+        Atom::new_var(State::LOG).into()
     }
 
     /// Return all defined symbol names (function names and variables).
     #[classmethod]
     pub fn get_all_symbol_names(_cls: &PyType) -> PyResult<Vec<String>> {
-        Ok(State::symbol_iter().map(|x| x.to_string()).collect())
+        Ok(State::symbol_iter().map(|(_, x)| x.to_string()).collect())
     }
 
     /// Parse a Symbolica expression from a string.
     ///
     /// Parameters
     /// ----------
-    /// input: str
-    ///     An input string. UTF-8 character are allowed.
+    /// input: str An input string. UTF-8 character are allowed.
     ///
     /// Examples
     /// --------
     /// >>> e = Expression.parse('x^2+y+y*4')
     /// >>> print(e)
     /// x^2+5*y
     ///
     /// Raises
     /// ------
     /// ValueError
     ///     If the input is not a valid Symbolica expression.
     ///
     #[classmethod]
-    pub fn parse(_cls: &PyType, arg: &str) -> PyResult<PythonExpression> {
-        let e = Atom::parse(arg).map_err(exceptions::PyValueError::new_err)?;
-
-        Ok(PythonExpression { expr: Arc::new(e) })
+    pub fn parse(_cls: &PyType, input: &str) -> PyResult<PythonExpression> {
+        let e = Atom::parse(input).map_err(exceptions::PyValueError::new_err)?;
+        Ok(e.into())
     }
 
     /// Copy the expression.
     pub fn __copy__(&self) -> PythonExpression {
-        PythonExpression {
-            expr: Arc::new((*self.expr).clone()),
-        }
+        self.expr.clone().into()
     }
 
     /// Convert the expression into a human-readable string.
     pub fn __str__(&self) -> PyResult<String> {
         Ok(format!("{}", AtomPrinter::new(self.expr.as_view())))
     }
 
@@ -1560,17 +1626,15 @@
             _ => Ok(None),
         }
     }
 
     /// Add this expression to `other`, returning the result.
     pub fn __add__(&self, rhs: ConvertibleToExpression) -> PyResult<PythonExpression> {
         let rhs = rhs.to_expression();
-        Ok(PythonExpression {
-            expr: Arc::new(self.expr.as_ref() + rhs.expr.as_ref()),
-        })
+        Ok((self.expr.as_ref() + rhs.expr.as_ref()).into())
     }
 
     /// Add this expression to `other`, returning the result.
     pub fn __radd__(&self, rhs: ConvertibleToExpression) -> PyResult<PythonExpression> {
         self.__add__(rhs)
     }
 
@@ -1584,30 +1648,26 @@
         rhs.to_expression()
             .__add__(ConvertibleToExpression(self.__neg__()?))
     }
 
     /// Add this expression to `other`, returning the result.
     pub fn __mul__(&self, rhs: ConvertibleToExpression) -> PyResult<PythonExpression> {
         let rhs = rhs.to_expression();
-        Ok(PythonExpression {
-            expr: Arc::new(self.expr.as_ref() * rhs.expr.as_ref()),
-        })
+        Ok((self.expr.as_ref() * rhs.expr.as_ref()).into())
     }
 
     /// Add this expression to `other`, returning the result.
     pub fn __rmul__(&self, rhs: ConvertibleToExpression) -> PyResult<PythonExpression> {
         self.__mul__(rhs)
     }
 
     /// Divide this expression by `other`, returning the result.
     pub fn __truediv__(&self, rhs: ConvertibleToExpression) -> PyResult<PythonExpression> {
         let rhs = rhs.to_expression();
-        Ok(PythonExpression {
-            expr: Arc::new(self.expr.as_ref() / rhs.expr.as_ref()),
-        })
+        Ok((self.expr.as_ref() / rhs.expr.as_ref()).into())
     }
 
     /// Divide `other` by this expression, returning the result.
     pub fn __rtruediv__(&self, rhs: ConvertibleToExpression) -> PyResult<PythonExpression> {
         rhs.to_expression()
             .__truediv__(ConvertibleToExpression(self.clone()))
     }
@@ -1621,17 +1681,15 @@
         if number.is_some() {
             return Err(exceptions::PyValueError::new_err(
                 "Optional number argument not supported",
             ));
         }
 
         let rhs = rhs.to_expression();
-        Ok(PythonExpression {
-            expr: Arc::new(self.expr.pow(&rhs.expr)),
-        })
+        Ok(self.expr.pow(&rhs.expr).into())
     }
 
     /// Take `base` to power `self`, returning the result.
     pub fn __rpow__(
         &self,
         rhs: ConvertibleToExpression,
         number: Option<i64>,
@@ -1652,56 +1710,127 @@
         Err(exceptions::PyTypeError::new_err(
             "Cannot xor an expression. Did you mean to write a power? Use ** instead, i.e. x**2",
         ))
     }
 
     /// Negate the current expression, returning the result.
     pub fn __neg__(&self) -> PyResult<PythonExpression> {
-        Ok(PythonExpression {
-            expr: Arc::new(-self.expr.as_ref()),
-        })
+        Ok((-self.expr.as_ref()).into())
     }
 
     /// Return the length of the atom.
     fn __len__(&self) -> usize {
         match self.expr.as_view() {
             AtomView::Add(a) => a.get_nargs(),
             AtomView::Mul(a) => a.get_nargs(),
             AtomView::Fun(a) => a.get_nargs(),
             _ => 1,
         }
     }
 
+    /// Create a Symbolica expression or transformer by calling the function with appropriate arguments.
+    ///
+    /// Examples
+    /// -------
+    /// >>> x = Expression.symbols('x')
+    /// >>> f = Expression.symbol('f')
+    /// >>> e = f(3,x)
+    /// >>> print(e)
+    /// f(3,x)
+    #[pyo3(signature = (*args,))]
+    pub fn __call__(&self, args: &PyTuple, py: Python) -> PyResult<PyObject> {
+        let id = match self.expr.as_view() {
+            AtomView::Var(v) => v.get_symbol(),
+            _ => {
+                return Err(exceptions::PyTypeError::new_err(
+                    "Only symbols can be called as functions",
+                ))
+            }
+        };
+
+        pub enum ExpressionOrTransformer {
+            Expression(PythonExpression),
+            Transformer(ConvertibleToPattern),
+        }
+
+        let mut fn_args = Vec::with_capacity(args.len());
+
+        for arg in args {
+            if let Ok(a) = arg.extract::<ConvertibleToExpression>() {
+                fn_args.push(ExpressionOrTransformer::Expression(a.to_expression()));
+            } else if let Ok(a) = arg.extract::<ConvertibleToPattern>() {
+                fn_args.push(ExpressionOrTransformer::Transformer(a));
+            } else {
+                let msg = format!("Unknown type: {}", arg.get_type().name().unwrap());
+                return Err(exceptions::PyTypeError::new_err(msg));
+            }
+        }
+
+        if fn_args
+            .iter()
+            .all(|x| matches!(x, ExpressionOrTransformer::Expression(_)))
+        {
+            // simplify to literal expression
+            Workspace::get_local().with(|workspace| {
+                let mut fun_b = workspace.new_atom();
+                let fun = fun_b.to_fun(id);
+
+                for x in fn_args {
+                    if let ExpressionOrTransformer::Expression(a) = x {
+                        fun.add_arg(a.expr.as_view());
+                    }
+                }
+
+                let mut out = Atom::default();
+                fun_b.as_view().normalize(workspace, &mut out);
+
+                Ok(PythonExpression::from(out).into_py(py))
+            })
+        } else {
+            // convert all wildcards back from literals
+            let mut transformer_args = Vec::with_capacity(args.len());
+            for arg in fn_args {
+                match arg {
+                    ExpressionOrTransformer::Transformer(t) => {
+                        transformer_args.push(t.to_pattern()?.expr.clone());
+                    }
+                    ExpressionOrTransformer::Expression(a) => {
+                        transformer_args.push(a.expr.as_view().into_pattern().clone());
+                    }
+                }
+            }
+
+            let p = Pattern::Fn(id, transformer_args);
+            Ok(PythonPattern::from(p).into_py(py))
+        }
+    }
+
     /// Convert the input to a transformer, on which subsequent transformations can be applied.
     pub fn transform(&self) -> PyResult<PythonPattern> {
-        Ok(PythonPattern {
-            expr: Arc::new(Pattern::Transformer(Box::new((
-                Some(self.expr.into_pattern()),
-                vec![],
-            )))),
-        })
+        Ok(Pattern::Transformer(Box::new((Some(self.expr.into_pattern()), vec![]))).into())
     }
 
     /// Get the `idx`th component of the expression.
     fn __getitem__(&self, idx: isize) -> PyResult<PythonExpression> {
         let slice = match self.expr.as_view() {
             AtomView::Add(a) => a.to_slice(),
             AtomView::Mul(m) => m.to_slice(),
             AtomView::Fun(f) => f.to_slice(),
             AtomView::Pow(p) => p.to_slice(),
             _ => Err(PyIndexError::new_err("Cannot access child of leaf node"))?,
         };
 
         if idx.unsigned_abs() < slice.len() {
-            Ok(PythonExpression {
-                expr: Arc::new(if idx < 0 {
-                    slice.get(slice.len() - idx.abs() as usize).to_owned()
-                } else {
-                    slice.get(idx as usize).to_owned()
-                }),
+            Ok(if idx < 0 {
+                slice
+                    .get(slice.len() - idx.abs() as usize)
+                    .to_owned()
+                    .into()
+            } else {
+                slice.get(idx as usize).to_owned().into()
             })
         } else {
             Err(PyIndexError::new_err(format!(
                 "Index {} out of bounds: the atom only has {} children.",
                 idx,
                 slice.len(),
             )))
@@ -1720,32 +1849,30 @@
                 if v.get_wildcard_level() == 0 {
                     return Err(exceptions::PyTypeError::new_err(
                         "Only wildcards can be restricted.",
                     ));
                 }
 
                 Ok(PythonPatternRestriction {
-                    condition: Arc::new(
-                        (name, PatternRestriction::Length(min_length, max_length)).into(),
-                    ),
+                    condition: (name, PatternRestriction::Length(min_length, max_length)).into(),
                 })
             }
             _ => Err(exceptions::PyTypeError::new_err(
                 "Only wildcards can be restricted.",
             )),
         }
     }
 
     /// Create a pattern restriction that tests the type of the atom.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression, AtomType
-    /// >>> x, x_ = Expression.vars('x', 'x_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x, x_ = Expression.symbols('x', 'x_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(x)*f(2)*f(f(3))
     /// >>> e = e.replace_all(f(x_), 1, x_.req_type(AtomType.Num))
     /// >>> print(e)
     ///
     /// Yields `f(x)*f(1)`.
     pub fn req_type(&self, atom_type: PythonAtomType) -> PyResult<PythonPatternRestriction> {
         match self.expr.as_view() {
@@ -1754,28 +1881,26 @@
                 if v.get_wildcard_level() == 0 {
                     return Err(exceptions::PyTypeError::new_err(
                         "Only wildcards can be restricted.",
                     ));
                 }
 
                 Ok(PythonPatternRestriction {
-                    condition: Arc::new(
-                        (
-                            name,
-                            PatternRestriction::IsAtomType(match atom_type {
-                                PythonAtomType::Num => AtomType::Num,
-                                PythonAtomType::Var => AtomType::Var,
-                                PythonAtomType::Add => AtomType::Add,
-                                PythonAtomType::Mul => AtomType::Mul,
-                                PythonAtomType::Pow => AtomType::Pow,
-                                PythonAtomType::Fn => AtomType::Fun,
-                            }),
-                        )
-                            .into(),
-                    ),
+                    condition: (
+                        name,
+                        PatternRestriction::IsAtomType(match atom_type {
+                            PythonAtomType::Num => AtomType::Num,
+                            PythonAtomType::Var => AtomType::Var,
+                            PythonAtomType::Add => AtomType::Add,
+                            PythonAtomType::Mul => AtomType::Mul,
+                            PythonAtomType::Pow => AtomType::Pow,
+                            PythonAtomType::Fn => AtomType::Fun,
+                        }),
+                    )
+                        .into(),
                 })
             }
             _ => Err(exceptions::PyTypeError::new_err(
                 "Only wildcards can be restricted.",
             )),
         }
     }
@@ -1789,15 +1914,15 @@
                 if v.get_wildcard_level() == 0 {
                     return Err(exceptions::PyTypeError::new_err(
                         "Only wildcards can be restricted.",
                     ));
                 }
 
                 Ok(PythonPatternRestriction {
-                    condition: Arc::new((name, PatternRestriction::IsLiteralWildcard(name)).into()),
+                    condition: (name, PatternRestriction::IsLiteralWildcard(name)).into(),
                 })
             }
             _ => Err(exceptions::PyTypeError::new_err(
                 "Only wildcards can be restricted.",
             )),
         }
     }
@@ -1846,16 +1971,16 @@
     /// When the option `cmp_any_atom` is set to `True`, this function compares atoms
     /// of any type. The result depends on the internal ordering and may change between
     /// different Symbolica versions.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(1)*f(2)*f(3)
     /// >>> e = e.replace_all(f(x_), 1, x_.req_lt(2))
     #[pyo3(signature =(other, cmp_any_atom = false))]
     pub fn req_lt(
         &self,
         other: ConvertibleToExpression,
         cmp_any_atom: bool,
@@ -1869,16 +1994,16 @@
     /// When the option `cmp_any_atom` is set to `True`, this function compares atoms
     /// of any type. The result depends on the internal ordering and may change between
     /// different Symbolica versions.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(1)*f(2)*f(3)
     /// >>> e = e.replace_all(f(x_), 1, x_.req_gt(2))
     #[pyo3(signature =(other, cmp_any_atom = false))]
     pub fn req_gt(
         &self,
         other: ConvertibleToExpression,
         cmp_any_atom: bool,
@@ -1892,16 +2017,16 @@
     /// When the option `cmp_any_atom` is set to `True`, this function compares atoms
     /// of any type. The result depends on the internal ordering and may change between
     /// different Symbolica versions.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(1)*f(2)*f(3)
     /// >>> e = e.replace_all(f(x_), 1, x_.req_le(2))
     #[pyo3(signature =(other, cmp_any_atom = false))]
     pub fn req_le(
         &self,
         other: ConvertibleToExpression,
         cmp_any_atom: bool,
@@ -1915,16 +2040,16 @@
     /// When the option `cmp_any_atom` is set to `True`, this function compares atoms
     /// of any type. The result depends on the internal ordering and may change between
     /// different Symbolica versions.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(1)*f(2)*f(3)
     /// >>> e = e.replace_all(f(x_), 1, x_.req_ge(2))
     #[pyo3(signature =(other, cmp_any_atom = false))]
     pub fn req_ge(
         &self,
         other: ConvertibleToExpression,
         cmp_any_atom: bool,
@@ -1934,16 +2059,16 @@
 
     /// Create a new pattern restriction that calls the function `filter_fn` with the matched
     /// atom that should return a boolean. If true, the pattern matches.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(1)*f(2)*f(3)
     /// >>> e = e.replace_all(f(x_), 1, x_.req(lambda m: m == 2 or m == 3))
     pub fn req(&self, filter_fn: PyObject) -> PyResult<PythonPatternRestriction> {
         let id = match self.expr.as_view() {
             AtomView::Var(v) => {
                 let name = v.get_symbol();
                 if v.get_wildcard_level() == 0 {
@@ -1957,52 +2082,46 @@
                 return Err(exceptions::PyTypeError::new_err(
                     "Only wildcards can be restricted.",
                 ));
             }
         };
 
         Ok(PythonPatternRestriction {
-            condition: Arc::new(
-                (
-                    id,
-                    PatternRestriction::Filter(Box::new(move |m| {
-                        let data = PythonExpression {
-                            expr: Arc::new({
-                                let mut a = Atom::default();
-                                m.to_atom(&mut a);
-                                a
-                            }),
-                        };
+            condition: (
+                id,
+                PatternRestriction::Filter(Box::new(move |m| {
+                    let mut a = Atom::default();
+                    m.to_atom(&mut a);
+                    let data: PythonExpression = a.into();
 
-                        Python::with_gil(|py| {
-                            filter_fn
-                                .call(py, (data,), None)
-                                .expect("Bad callback function")
-                                .extract::<bool>(py)
-                                .expect("Pattern filter does not return a boolean")
-                        })
-                    })),
-                )
-                    .into(),
-            ),
+                    Python::with_gil(|py| {
+                        filter_fn
+                            .call(py, (data,), None)
+                            .expect("Bad callback function")
+                            .extract::<bool>(py)
+                            .expect("Pattern filter does not return a boolean")
+                    })
+                })),
+            )
+                .into(),
         })
     }
 
     /// Create a pattern restriction that passes when the wildcard is smaller than another wildcard.
     /// If the matched wildcards are not a numbers, the pattern fails.
     ///
     /// When the option `cmp_any_atom` is set to `True`, this function compares atoms
     /// of any type. The result depends on the internal ordering and may change between
     /// different Symbolica versions.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_, y_ = Expression.var('x_', 'y_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_, y_ = Expression.symbol('x_', 'y_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(1,2)
     /// >>> e = e.replace_all(f(x_,y_), 1, x_.req_cmp_lt(y_))
     #[pyo3(signature =(other, cmp_any_atom = false))]
     pub fn req_cmp_lt(
         &self,
         other: PythonExpression,
         cmp_any_atom: bool,
@@ -2016,16 +2135,16 @@
     /// When the option `cmp_any_atom` is set to `True`, this function compares atoms
     /// of any type. The result depends on the internal ordering and may change between
     /// different Symbolica versions.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_, y_ = Expression.var('x_', 'y_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_, y_ = Expression.symbol('x_', 'y_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(2,1)
     /// >>> e = e.replace_all(f(x_,y_), 1, x_.req_cmp_gt(y_))
     #[pyo3(signature =(other, cmp_any_atom = false))]
     pub fn req_cmp_gt(
         &self,
         other: PythonExpression,
         cmp_any_atom: bool,
@@ -2039,16 +2158,16 @@
     /// When the option `cmp_any_atom` is set to `True`, this function compares atoms
     /// of any type. The result depends on the internal ordering and may change between
     /// different Symbolica versions.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_, y_ = Expression.var('x_', 'y_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_, y_ = Expression.symbol('x_', 'y_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(1,2)
     /// >>> e = e.replace_all(f(x_,y_), 1, x_.req_cmp_le(y_))
     #[pyo3(signature =(other, cmp_any_atom = false))]
     pub fn req_cmp_le(
         &self,
         other: PythonExpression,
         cmp_any_atom: bool,
@@ -2062,16 +2181,16 @@
     /// When the option `cmp_any_atom` is set to `True`, this function compares atoms
     /// of any type. The result depends on the internal ordering and may change between
     /// different Symbolica versions.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_, y_ = Expression.var('x_', 'y_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_, y_ = Expression.symbol('x_', 'y_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(2,1)
     /// >>> e = e.replace_all(f(x_,y_), 1, x_.req_cmp_ge(y_))
     #[pyo3(signature =(other, cmp_any_atom = false))]
     pub fn req_cmp_ge(
         &self,
         other: PythonExpression,
         cmp_any_atom: bool,
@@ -2081,16 +2200,16 @@
 
     /// Create a new pattern restriction that calls the function `cmp_fn` with another the matched
     /// atom and the match atom of the `other` wildcard that should return a boolean. If true, the pattern matches.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x_, y_ = Expression.vars('x_', 'y_')
-    /// >>> f = Expression.fun("f")
+    /// >>> x_, y_ = Expression.symbols('x_', 'y_')
+    /// >>> f = Expression.symbol("f")
     /// >>> e = f(1)*f(2)*f(3)
     /// >>> e = e.replace_all(f(x_)*f(y_), 1, x_.req_cmp(y_, lambda m1, m2: m1 + m2 == 4))
     pub fn req_cmp(
         &self,
         other: PythonExpression,
         cmp_fn: PyObject,
     ) -> PyResult<PythonPatternRestriction> {
@@ -2125,48 +2244,37 @@
                 return Err(exceptions::PyTypeError::new_err(
                     "Only wildcards can be restricted.",
                 ));
             }
         };
 
         Ok(PythonPatternRestriction {
-            condition: Arc::new(
-                (
-                    id,
-                    PatternRestriction::Cmp(
-                        other_id,
-                        Box::new(move |m1, m2| {
-                            let data1 = PythonExpression {
-                                expr: Arc::new({
-                                    let mut a = Atom::default();
-                                    m1.to_atom(&mut a);
-                                    a
-                                }),
-                            };
-
-                            let data2 = PythonExpression {
-                                expr: Arc::new({
-                                    let mut a = Atom::default();
-                                    m2.to_atom(&mut a);
-                                    a
-                                }),
-                            };
-
-                            Python::with_gil(|py| {
-                                cmp_fn
-                                    .call(py, (data1, data2), None)
-                                    .expect("Bad callback function")
-                                    .extract::<bool>(py)
-                                    .expect("Pattern comparison does not return a boolean")
-                            })
-                        }),
-                    ),
-                )
-                    .into(),
-            ),
+            condition: (
+                id,
+                PatternRestriction::Cmp(
+                    other_id,
+                    Box::new(move |m1, m2| {
+                        let mut a = Atom::default();
+                        m1.to_atom(&mut a);
+                        let data1: PythonExpression = a.clone().into();
+
+                        m2.to_atom(&mut a);
+                        let data2: PythonExpression = a.into();
+
+                        Python::with_gil(|py| {
+                            cmp_fn
+                                .call(py, (data1, data2), None)
+                                .expect("Bad callback function")
+                                .extract::<bool>(py)
+                                .expect("Pattern comparison does not return a boolean")
+                        })
+                    }),
+                ),
+            )
+                .into(),
         })
     }
 
     /// Create an iterator over all atoms in the expression.
     fn __iter__(&self) -> PyResult<PythonAtomIterator> {
         match self.expr.as_view() {
             AtomView::Add(_) | AtomView::Mul(_) | AtomView::Fun(_) | AtomView::Pow(_) => {}
@@ -2180,26 +2288,27 @@
 
         Ok(PythonAtomIterator::from_expr(self.clone()))
     }
 
     /// Map the transformations to every term in the expression.
     /// The execution happen in parallel.
     ///
-    /// No new functions or variables can be defined and no new
-    /// expressions can be parsed inside the map. Doing so will
-    /// result in a deadlock.
-    ///
     /// Examples
     /// --------
-    /// >>> x, x_ = Expression.vars('x', 'x_')
+    /// >>> x, x_ = Expression.symbols('x', 'x_')
     /// >>> e = (1+x)**2
     /// >>> r = e.map(Transformer().expand().replace_all(x, 6))
     /// >>> print(r)
-    pub fn map(&self, op: PythonPattern, py: Python) -> PyResult<PythonExpression> {
-        let t = match op.expr.as_ref() {
+    pub fn map(
+        &self,
+        op: PythonPattern,
+        py: Python,
+        n_cores: Option<usize>,
+    ) -> PyResult<PythonExpression> {
+        let t = match &op.expr {
             Pattern::Transformer(t) => {
                 if t.0.is_some() {
                     return Err(exceptions::PyValueError::new_err(
                         "Transformer is bound to expression. Use Transformer() instead."
                             .to_string(),
                     ));
                 }
@@ -2212,38 +2321,44 @@
             }
         };
 
         // release the GIL as Python functions may be called from
         // within the term mapper
         let mut stream = py.allow_threads(move || {
             // map every term in the expression
-            let stream = TermStreamer::new_from((*self.expr).clone());
-            let m = stream.map(|workspace, x| {
+            let mut stream = TermStreamer::<CompressorWriter<_>>::new(TermStreamerConfig {
+                n_cores: n_cores.unwrap_or(1),
+                ..Default::default()
+            });
+            stream.push(self.expr.clone());
+
+            let m = stream.map(|x| {
                 let mut out = Atom::default();
-                // TODO: capture and abort the parallel run
-                Transformer::execute(x.as_view(), &t, workspace, &mut out).unwrap_or_else(|e| {
-                    panic!("Transformer failed during parallel execution: {:?}", e)
+                Workspace::get_local().with(|ws| {
+                    Transformer::execute(x.as_view(), &t, ws, &mut out).unwrap_or_else(|e| {
+                        // TODO: capture and abort the parallel run
+                        panic!("Transformer failed during parallel execution: {:?}", e)
+                    });
                 });
                 out
             });
             Ok::<_, PyErr>(m)
         })?;
 
         let b = stream.to_expression();
 
-        Ok(PythonExpression { expr: Arc::new(b) })
+        Ok(b.into())
     }
 
     /// Set the coefficient ring to contain the variables in the `vars` list.
     /// This will move all variables into a rational polynomial function.
 
     /// Parameters
     /// ----------
-    /// vars : List[Expression]
-    ///         A list of variables
+    /// vars: List[Expression] A list of variables
     pub fn set_coefficient_ring(&self, vars: Vec<PythonExpression>) -> PyResult<PythonExpression> {
         let mut var_map = vec![];
         for v in vars {
             match v.expr.as_view() {
                 AtomView::Var(v) => var_map.push(v.get_symbol().into()),
                 e => {
                     Err(exceptions::PyValueError::new_err(format!(
@@ -2252,42 +2367,55 @@
                     )))?;
                 }
             }
         }
 
         let b = self.expr.as_view().set_coefficient_ring(&Arc::new(var_map));
 
-        Ok(PythonExpression { expr: Arc::new(b) })
+        Ok(b.into())
     }
 
-    /// Expand the expression.
-    pub fn expand(&self) -> PyResult<PythonExpression> {
-        let b = self.expr.as_view().expand();
-        Ok(PythonExpression { expr: Arc::new(b) })
+    /// Expand the expression. Optionally, expand in `var` only.
+    pub fn expand(&self, var: Option<ConvertibleToExpression>) -> PyResult<PythonExpression> {
+        if let Some(var) = var {
+            let id = if let AtomView::Var(x) = var.to_expression().expr.as_view() {
+                x.get_symbol()
+            } else {
+                return Err(exceptions::PyValueError::new_err(
+                    "Expansion must be done wrt a variable or function name",
+                ));
+            };
+
+            let b = self.expr.as_view().expand_in(id);
+            Ok(b.into())
+        } else {
+            let b = self.expr.as_view().expand();
+            Ok(b.into())
+        }
     }
 
     /// Collect terms involving the same power of `x`, where `x` is a variable or function name.
     /// Return the list of key-coefficient pairs and the remainder that matched no key.
     ///
     /// Both the *key* (the quantity collected in) and its coefficient can be mapped using
     /// `key_map` and `coeff_map` respectively.
     ///
     /// Examples
     /// --------
     ///
     /// >>> from symbolica import Expression
-    /// >>> x, y = Expression.vars('x', 'y')
+    /// >>> x, y = Expression.symbols('x', 'y')
     /// >>> e = 5*x + x * y + x**2 + 5
     /// >>>
     /// >>> print(e.collect(x))
     ///
     /// yields `x^2+x*(y+5)+5`.
     ///
     /// >>> from symbolica import Expression
-    /// >>> x, y = Expression.vars('x', 'y')
+    /// >>> x, y = Expression.symbols('x', 'y')
     /// >>> exp, coeff = Expression.funs('var', 'coeff')
     /// >>> e = 5*x + x * y + x**2 + 5
     /// >>>
     /// >>> print(e.collect(x, key_map=lambda x: exp(x), coeff_map=lambda x: coeff(x)))
     ///
     /// yields `var(1)*coeff(5)+var(x)*coeff(y+5)+var(x^2)*coeff(1)`.
     pub fn collect(
@@ -2305,17 +2433,15 @@
         };
 
         let b = self.expr.as_view().collect(
             id,
             if let Some(key_map) = key_map {
                 Some(Box::new(move |key, out| {
                     Python::with_gil(|py| {
-                        let key = PythonExpression {
-                            expr: Arc::new(key.to_owned()),
-                        };
+                        let key: PythonExpression = key.to_owned().into();
 
                         out.set_from_view(
                             &key_map
                                 .call(py, (key,), None)
                                 .expect("Bad callback function")
                                 .extract::<PythonExpression>(py)
                                 .expect("Key map should return an expression")
@@ -2326,17 +2452,15 @@
                 }))
             } else {
                 None
             },
             if let Some(coeff_map) = coeff_map {
                 Some(Box::new(move |coeff, out| {
                     Python::with_gil(|py| {
-                        let coeff = PythonExpression {
-                            expr: Arc::new(coeff.to_owned()),
-                        };
+                        let coeff: PythonExpression = coeff.to_owned().into();
 
                         out.set_from_view(
                             &coeff_map
                                 .call(py, (coeff,), None)
                                 .expect("Bad callback function")
                                 .extract::<PythonExpression>(py)
                                 .expect("Coeff map should return an expression")
@@ -2346,47 +2470,47 @@
                     });
                 }))
             } else {
                 None
             },
         );
 
-        Ok(PythonExpression { expr: Arc::new(b) })
+        Ok(b.into())
     }
 
     /// Collect terms involving the literal occurrence of `x`.
     ///
     /// Examples
     /// --------
     ///
     /// from symbolica import Expression
     /// >>>
-    /// >>> x, y = Expression.vars('x', 'y')
+    /// >>> x, y = Expression.symbols('x', 'y')
     /// >>> e = 5*x + x * y + x**2 + y*x**2
     /// >>> print(e.coefficient(x**2))
     ///
     /// yields
     ///
     /// ```
     /// y + 1
     /// ```
     pub fn coefficient(&self, x: ConvertibleToExpression) -> PythonExpression {
         let r = self.expr.coefficient(x.to_expression().expr.as_view());
-        PythonExpression { expr: Arc::new(r) }
+        r.into()
     }
 
     /// Collect terms involving the same power of `x`, where `x` is a variable or function name.
     /// Return the list of key-coefficient pairs and the remainder that matched no key.
     ///
     /// Examples
     /// --------
     ///
     /// from symbolica import Expression
     /// >>>
-    /// >>> x, y = Expression.vars('x', 'y')
+    /// >>> x, y = Expression.symbols('x', 'y')
     /// >>> e = 5*x + x * y + x**2 + 5
     /// >>>
     /// >>> for a in e.coefficient_list(x):
     /// >>>     print(a[0], a[1])
     ///
     /// yields
     ///
@@ -2407,40 +2531,24 @@
             ));
         };
 
         let (list, rest) = self.expr.coefficient_list(id);
 
         let mut py_list: Vec<_> = list
             .into_iter()
-            .map(|e| {
-                (
-                    PythonExpression {
-                        expr: Arc::new(e.0.to_owned()),
-                    },
-                    PythonExpression {
-                        expr: Arc::new(e.1),
-                    },
-                )
-            })
+            .map(|e| (e.0.to_owned().into(), e.1.into()))
             .collect();
 
         if let Atom::Num(n) = &rest {
             if n.to_num_view().is_zero() {
                 return Ok(py_list);
             }
         }
 
-        py_list.push((
-            PythonExpression {
-                expr: Arc::new(Atom::new_num(1)),
-            },
-            PythonExpression {
-                expr: Arc::new(rest),
-            },
-        ));
+        py_list.push((Atom::new_num(1).into(), rest.into()));
 
         Ok(py_list)
     }
 
     /// Derive the expression w.r.t the variable `x`.
     pub fn derivative(&self, x: ConvertibleToExpression) -> PyResult<PythonExpression> {
         let id = if let AtomView::Var(x) = x.to_expression().expr.as_view() {
@@ -2449,59 +2557,64 @@
             return Err(exceptions::PyValueError::new_err(
                 "Derivative must be taken wrt a variable",
             ));
         };
 
         let b = self.expr.derivative(id);
 
-        Ok(PythonExpression { expr: Arc::new(b) })
+        Ok(b.into())
     }
 
-    /// Taylor expand in `x` around `expansion_point` to depth `depth`.
+    /// Series expand in `x` around `expansion_point` to depth `depth`.
     ///
-    /// Example
+    /// Examples
     /// -------
     /// >>> from symbolica import Expression
-    /// >>> x, y = Expression.vars('x', 'y')
-    /// >>> f = Expression.fun('f')
+    /// >>> x, y = Expression.symbols('x', 'y')
+    /// >>> f = Expression.symbol('f')
     /// >>>
     /// >>> e = 2* x**2 * y + f(x)
-    /// >>> e = e.taylor_series(x, 0, 2)
+    /// >>> e = e.series(x, 0, 2)
     /// >>>
     /// >>> print(e)
     ///
     /// yields `f(0)+x*der(1,f(0))+1/2*x^2*(der(2,f(0))+4*y)`.
-    pub fn taylor_series(
+    #[pyo3(signature = (x, expansion_point, depth, depth_denom = 1))]
+    pub fn series(
         &self,
         x: ConvertibleToExpression,
         expansion_point: ConvertibleToExpression,
-        depth: u32,
-    ) -> PyResult<PythonExpression> {
+        depth: i64,
+        depth_denom: i64,
+    ) -> PyResult<PythonSeries> {
         let id = if let AtomView::Var(x) = x.to_expression().expr.as_view() {
             x.get_symbol()
         } else {
             return Err(exceptions::PyValueError::new_err(
                 "Derivative must be taken wrt a variable",
             ));
         };
 
-        let b = self
-            .expr
-            .taylor_series(id, expansion_point.to_expression().expr.as_view(), depth);
-
-        Ok(PythonExpression { expr: Arc::new(b) })
+        match self.expr.series(
+            id,
+            expansion_point.to_expression().expr.as_view(),
+            (depth, depth_denom).into(),
+        ) {
+            Ok(s) => Ok(PythonSeries { series: s }),
+            Err(e) => Err(exceptions::PyValueError::new_err(format!("{}", e))),
+        }
     }
 
     /// Compute the partial fraction decomposition in `x`.
     ///
     /// Examples
     /// --------
     ///
     /// >>> from symbolica import Expression
-    /// >>> x = Expression.var('x')
+    /// >>> x = Expression.symbol('x')
     /// >>> p = Expression.parse('1/((x+y)*(x^2+x*y+1)(x+1))')
     /// >>> print(p.apart(x))
     pub fn apart(&self, x: PythonExpression) -> PyResult<PythonExpression> {
         let poly = self.expr.to_rational_polynomial::<_, _, u32>(&Q, &Z, None);
         let x = poly
             .get_variables()
             .iter()
@@ -2524,30 +2637,28 @@
             for f in fs {
                 a.extend(f.to_expression().as_view());
             }
 
             res.as_view().normalize(ws, &mut rn);
         });
 
-        Ok(PythonExpression { expr: Arc::new(rn) })
+        Ok(rn.into())
     }
 
     /// Write the expression over a common denominator.
     ///
     /// Examples
     /// --------
     ///
     /// >>> from symbolica import Expression
     /// >>> p = Expression.parse('v1^2/2+v1^3/v4*v2+v3/(1+v4)')
     /// >>> print(p.together())
     pub fn together(&self) -> PyResult<PythonExpression> {
         let poly = self.expr.to_rational_polynomial::<_, _, u32>(&Q, &Z, None);
-        Ok(PythonExpression {
-            expr: Arc::new(poly.to_expression()),
-        })
+        Ok(poly.to_expression().into())
     }
 
     /// Convert the expression to a polynomial, optionally, with the variables and the ordering specified in `vars`.
     /// All non-polynomial elements will be converted to new independent variables.
     pub fn to_polynomial(&self, vars: Option<Vec<PythonExpression>>) -> PyResult<PythonPolynomial> {
         let mut var_map = vec![];
         if let Some(vm) = vars {
@@ -2567,15 +2678,15 @@
         let var_map = if var_map.is_empty() {
             None
         } else {
             Some(Arc::new(var_map))
         };
 
         Ok(PythonPolynomial {
-            poly: Arc::new(self.expr.to_polynomial(&Q, var_map)),
+            poly: self.expr.to_polynomial(&Q, var_map),
         })
     }
 
     /// Convert the expression to a rational polynomial, optionally, with the variable ordering specified in `vars`.
     /// The latter is useful if it is known in advance that more variables may be added in the future to the
     /// rational polynomial through composition with other rational polynomials.
     ///
@@ -2607,15 +2718,15 @@
         let var_map = if var_map.is_empty() {
             None
         } else {
             Some(Arc::new(var_map))
         };
 
         Ok(PythonRationalPolynomial {
-            poly: Arc::new(self.expr.to_rational_polynomial(&Q, &Z, var_map)),
+            poly: self.expr.to_rational_polynomial(&Q, &Z, var_map),
         })
     }
 
     /// Similar to [PythonExpression::to_rational_polynomial()], but the power of each variable limited to 255.
     pub fn to_rational_polynomial_small_exponent(
         &self,
         vars: Option<Vec<PythonExpression>>,
@@ -2638,46 +2749,46 @@
         let var_map = if var_map.is_empty() {
             None
         } else {
             Some(Arc::new(var_map))
         };
 
         Ok(PythonRationalPolynomialSmallExponent {
-            poly: Arc::new(self.expr.to_rational_polynomial(&Q, &Z, var_map)),
+            poly: self.expr.to_rational_polynomial(&Q, &Z, var_map),
         })
     }
 
     /// Return an iterator over the pattern `self` matching to `lhs`.
     /// Restrictions on pattern can be supplied through `cond`.
     ///
     /// Examples
     /// --------
     ///
-    /// >>> x, x_ = Expression.vars('x','x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x, x_ = Expression.symbols('x','x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(x)*f(1)*f(2)*f(3)
     /// >>> for match in e.match(f(x_)):
     /// >>>    for map in match:
     /// >>>        print(map[0],'=', map[1])
     #[pyo3(name = "r#match")]
     pub fn pattern_match(
         &self,
         lhs: ConvertibleToPattern,
         cond: Option<PythonPatternRestriction>,
         level_range: Option<(usize, Option<usize>)>,
         level_is_tree_depth: Option<bool>,
     ) -> PyResult<PythonMatchIterator> {
         let conditions = cond
             .map(|r| r.condition.clone())
-            .unwrap_or(Arc::new(Condition::default()));
-        let settings = Arc::new(MatchSettings {
+            .unwrap_or(Condition::default());
+        let settings = MatchSettings {
             level_range: level_range.unwrap_or((0, None)),
             level_is_tree_depth: level_is_tree_depth.unwrap_or(false),
             ..MatchSettings::default()
-        });
+        };
         Ok(PythonMatchIterator::new(
             (
                 lhs.to_pattern()?.expr,
                 self.expr.clone(),
                 conditions,
                 settings,
             ),
@@ -2694,16 +2805,16 @@
     /// The first level is 0 and the level is increased when going into a function or one level deeper in the expression tree,
     /// depending on `level_is_tree_depth`.
     ///
     /// Examples
     /// --------
     ///
     /// >>> from symbolica import Expression
-    /// >>> x_ = Expression.var('x_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x_ = Expression.symbol('x_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(1)*f(2)*f(3)
     /// >>> for r in e.replace(f(x_), f(x_ + 1)):
     /// >>>     print(r)
     ///
     /// Yields:
     /// ```
     /// f(2)*f(2)*f(3)
@@ -2716,20 +2827,20 @@
         rhs: ConvertibleToPattern,
         cond: Option<PythonPatternRestriction>,
         level_range: Option<(usize, Option<usize>)>,
         level_is_tree_depth: Option<bool>,
     ) -> PyResult<PythonReplaceIterator> {
         let conditions = cond
             .map(|r| r.condition.clone())
-            .unwrap_or(Arc::new(Condition::default()));
-        let settings = Arc::new(MatchSettings {
+            .unwrap_or(Condition::default());
+        let settings = MatchSettings {
             level_range: level_range.unwrap_or((0, None)),
             level_is_tree_depth: level_is_tree_depth.unwrap_or(false),
             ..MatchSettings::default()
-        });
+        };
 
         Ok(PythonReplaceIterator::new(
             (
                 lhs.to_pattern()?.expr,
                 self.expr.clone(),
                 rhs.to_pattern()?.expr,
                 conditions,
@@ -2749,19 +2860,34 @@
     /// depending on `level_is_tree_depth`.
     ///
     /// The entire operation can be repeated until there are no more matches using `repeat=True`.
     ///
     /// Examples
     /// --------
     ///
-    /// >>> x, w1_, w2_ = Expression.vars('x','w1_','w2_')
-    /// >>> f = Expression.fun('f')
+    /// >>> x, w1_, w2_ = Expression.symbols('x','w1_','w2_')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = f(3,x)
     /// >>> r = e.replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2), (w1_ >= 1) & w2_.is_var())
     /// >>> print(r)
+    ///
+    /// Parameters
+    /// ----------
+    /// pattern: Transformer | Expression | int
+    ///     The pattern to match.
+    /// rhs: Transformer | Expression | int
+    ///     The right-hand side to replace the matched subexpression with.
+    /// cond: Optional[PatternRestriction]
+    ///     Conditions on the pattern.
+    /// level_range: (int, int), optional
+    ///     Specifies the `[min,max]` level at which the pattern is allowed to match. The first level is 0 and the level is increased when going into a function or one level deeper in the expression tree, depending on `level_is_tree_depth`.
+    /// level_is_tree_depth: bool, optional
+    ///     If set to `True`, the level is increased when going one level deeper in the expression tree.
+    /// repeat: bool, optional
+    ///     If set to `True`, the entire operation will be repeated until there are no more matches.
     pub fn replace_all(
         &self,
         pattern: ConvertibleToPattern,
         rhs: ConvertibleToPattern,
         cond: Option<PythonPatternRestriction>,
         non_greedy_wildcards: Option<Vec<PythonExpression>>,
         level_range: Option<(usize, Option<usize>)>,
@@ -2802,39 +2928,37 @@
         let mut expr_ref = self.expr.as_view();
 
         let mut out = RecycledAtom::new();
         let mut out2 = RecycledAtom::new();
         while pattern.replace_all_into(
             expr_ref,
             rhs,
-            cond.as_ref().map(|r| r.condition.as_ref()),
+            cond.as_ref().map(|r| &r.condition),
             Some(&settings),
             &mut out,
         ) {
             if !repeat.unwrap_or(false) {
                 break;
             }
 
             std::mem::swap(&mut out, &mut out2);
             expr_ref = out2.as_view();
         }
 
-        Ok(PythonExpression {
-            expr: Arc::new(out.into_inner()),
-        })
+        Ok(out.into_inner().into())
     }
 
     /// Solve a linear system in the variables `variables`, where each expression
     /// in the system is understood to yield 0.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x, y, c = Expression.vars('x', 'y', 'c')
-    /// >>> f = Expression.fun('f')
+    /// >>> x, y, c = Expression.symbols('x', 'y', 'c')
+    /// >>> f = Expression.symbol('f')
     /// >>> x_r, y_r = Expression.solve_linear_system([f(c)*x + y/c - 1, y-c/2], [x, y])
     /// >>> print('x =', x_r, ', y =', y_r)
     #[classmethod]
     pub fn solve_linear_system(
         _cls: &PyType,
         system: Vec<ConvertibleToExpression>,
         variables: Vec<PythonExpression>,
@@ -2855,28 +2979,25 @@
             }
         }
 
         let res = AtomView::solve_linear_system::<u16>(&system_b, &vars).map_err(|e| {
             exceptions::PyValueError::new_err(format!("Could not solve system: {}", e))
         })?;
 
-        Ok(res
-            .into_iter()
-            .map(|x| PythonExpression { expr: Arc::new(x) })
-            .collect())
+        Ok(res.into_iter().map(|x| x.into()).collect())
     }
 
     /// Evaluate the expression, using a map of all the constants and
     /// user functions to a float.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x = Expression.var('x')
-    /// >>> f = Expression.fun('f')
+    /// >>> x = Expression.symbol('x')
+    /// >>> f = Expression.symbol('f')
     /// >>> e = Expression.parse('cos(x)')*3 + f(x,2)
     /// >>> print(e.evaluate({x: 1}, {f: lambda args: args[0]+args[1]}))
     pub fn evaluate(
         &self,
         constants: HashMap<PythonExpression, f64>,
         functions: HashMap<Variable, PyObject>,
     ) -> PyResult<f64> {
@@ -2921,15 +3042,15 @@
 
     /// Evaluate the expression, using a map of all the variables and
     /// user functions to a complex number.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
-    /// >>> x, y = Expression.vars('x', 'y')
+    /// >>> x, y = Expression.symbols('x', 'y')
     /// >>> e = Expression.parse('sqrt(x)')*y
     /// >>> print(e.evaluate_complex({x: 1 + 2j, y: 4 + 3j}, {}))
     pub fn evaluate_complex<'py>(
         &self,
         py: Python<'py>,
         constants: HashMap<PythonExpression, Complex<f64>>,
         functions: HashMap<Variable, PyObject>,
@@ -2978,231 +3099,276 @@
             .expr
             .as_view()
             .evaluate(&constants, &functions, &mut cache);
         Ok(PyComplex::from_doubles(py, r.re, r.im))
     }
 }
 
-/// A function class for python that constructs an `Expression` when called with arguments.
-/// This allows to write:
-/// ```python
-/// f = Expression.fun("f")
-/// e = f(1,2,3)
-/// ```
-#[pyclass(name = "Function")]
-#[derive(Clone)]
-pub struct PythonFunction {
-    id: Symbol,
+/// A series expansion class.
+///
+/// Supports standard arithmetic operations, such
+/// as addition and multiplication.
+///
+/// Examples
+/// --------
+/// >>> x = Expression.symbol('x')
+/// >>> s = Expression.parse("(1-cos(x))/sin(x)").series(x, 0, 4)
+/// >>> print(s)
+#[pyclass(name = "Series", module = "symbolica")]
+pub struct PythonSeries {
+    pub series: Series<AtomField>,
 }
 
 #[pymethods]
-impl PythonFunction {
-    /// Create a new function from a `name`. Can be turned into a symmetric function
-    /// using `is_symmetric=True` or into an antisymmetric function using `is_antisymmetric=True`.
-    /// The function can be made multilinear using `is_linear=True`.
-    ///
-    /// Once attributes are defined on a function, they cannot be redefined later.
-    #[new]
-    pub fn __new__(
-        name: &str,
-        is_symmetric: Option<bool>,
-        is_antisymmetric: Option<bool>,
-        is_linear: Option<bool>,
-    ) -> PyResult<Self> {
-        if is_symmetric.is_none() && is_antisymmetric.is_none() && is_linear.is_none() {
-            return Ok(PythonFunction {
-                id: State::get_symbol(name),
-            });
-        }
+impl PythonSeries {
+    /// Add this series to `other`, returning the result.
+    pub fn __add__(&self, rhs: &Self) -> PyResult<Self> {
+        Ok(Self {
+            series: &self.series + &rhs.series,
+        })
+    }
 
-        if is_symmetric == Some(true) && is_antisymmetric == Some(true) {
-            Err(exceptions::PyValueError::new_err(
-                "Function cannot be both symmetric and antisymmetric",
-            ))?;
-        }
+    pub fn __sub__(&self, rhs: &Self) -> PyResult<Self> {
+        Ok(Self {
+            series: &self.series - &rhs.series,
+        })
+    }
 
-        let mut opts = vec![];
+    pub fn __mul__(&self, rhs: &Self) -> PyResult<Self> {
+        Ok(Self {
+            series: &self.series * &rhs.series,
+        })
+    }
 
-        if let Some(true) = is_symmetric {
-            opts.push(FunctionAttribute::Symmetric);
-        }
+    pub fn __truediv__(&self, rhs: &Self) -> PyResult<Self> {
+        Ok(Self {
+            series: &self.series / &rhs.series,
+        })
+    }
 
-        if let Some(true) = is_antisymmetric {
-            opts.push(FunctionAttribute::Antisymmetric);
+    pub fn __pow__(&self, rhs: i64, m: Option<i64>) -> PyResult<Self> {
+        if m.is_some() {
+            return Err(exceptions::PyValueError::new_err(
+                "Optional number argument not supported",
+            ));
         }
 
-        if let Some(true) = is_linear {
-            opts.push(FunctionAttribute::Linear);
+        Ok(Self {
+            series: self.series.rpow((rhs, 1).into()),
+        })
+    }
+
+    pub fn __neg__(&self) -> Self {
+        Self {
+            series: -self.series.clone(),
         }
+    }
 
-        let id = State::get_symbol_with_attributes(name, &opts)
-            .map_err(|e| exceptions::PyTypeError::new_err(e.to_string()))?;
+    pub fn __str__(&self) -> PyResult<String> {
+        Ok(format!("{}", self.series))
+    }
 
-        Ok(PythonFunction { id })
+    pub fn sin(&self) -> PyResult<Self> {
+        Ok(Self {
+            series: self
+                .series
+                .sin()
+                .map_err(|e| exceptions::PyValueError::new_err(e))?,
+        })
     }
 
-    /// The built-in function that converts a rational polynomial to a coefficient.
-    #[classattr]
-    #[pyo3(name = "COEFF")]
-    pub fn coeff() -> PythonFunction {
-        PythonFunction { id: State::COEFF }
+    pub fn cos(&self) -> PyResult<Self> {
+        Ok(Self {
+            series: self
+                .series
+                .cos()
+                .map_err(|e| exceptions::PyValueError::new_err(e))?,
+        })
     }
 
-    /// The built-in cosine function.
-    #[classattr]
-    #[pyo3(name = "COS")]
-    pub fn cos() -> PythonFunction {
-        PythonFunction { id: State::COS }
+    pub fn exp(&self) -> PyResult<Self> {
+        Ok(Self {
+            series: self
+                .series
+                .exp()
+                .map_err(|e| exceptions::PyValueError::new_err(e))?,
+        })
     }
 
-    /// The built-in sine function.
-    #[classattr]
-    #[pyo3(name = "SIN")]
-    pub fn sin() -> PythonFunction {
-        PythonFunction { id: State::SIN }
+    pub fn log(&self) -> PyResult<Self> {
+        Ok(Self {
+            series: self
+                .series
+                .log()
+                .map_err(|e| exceptions::PyValueError::new_err(e))?,
+        })
     }
 
-    /// The built-in exponential function.
-    #[classattr]
-    #[pyo3(name = "EXP")]
-    pub fn exp() -> PythonFunction {
-        PythonFunction { id: State::EXP }
+    pub fn pow(&self, num: i64, den: i64) -> PyResult<Self> {
+        Ok(Self {
+            series: self.series.rpow((num, den).into()),
+        })
     }
 
-    /// The built-in logarithm function.
-    #[classattr]
-    #[pyo3(name = "LOG")]
-    pub fn log() -> PythonFunction {
-        PythonFunction { id: State::LOG }
+    pub fn spow(&self, pow: &Self) -> PyResult<Self> {
+        Ok(Self {
+            series: self
+                .series
+                .pow(&pow.series)
+                .map_err(|e| exceptions::PyValueError::new_err(e))?,
+        })
     }
 
-    /// Returns `True` iff this function is symmetric.
-    pub fn is_symmetric(&self) -> bool {
-        self.id.is_symmetric()
+    /// Convert the series into an expression.
+    pub fn to_expression(&self) -> PythonExpression {
+        self.series.to_atom().into()
     }
+}
 
-    /// Create a Symbolica expression or transformer by calling the function with appropriate arguments.
-    ///
-    /// Examples
-    /// -------
-    /// >>> x = Expression.vars('x')
-    /// >>> f = Expression.fun('f')
-    /// >>> e = f(3,x)
-    /// >>> print(e)
-    /// f(3,x)
-    #[pyo3(signature = (*args,))]
-    pub fn __call__(&self, args: &PyTuple, py: Python) -> PyResult<PyObject> {
-        pub enum ExpressionOrTransformer {
-            Expression(PythonExpression),
-            Transformer(ConvertibleToPattern),
-        }
+/// A Symbolica term streamer.
+#[pyclass(name = "TermStreamer", module = "symbolica")]
+pub struct PythonTermStreamer {
+    pub stream: TermStreamer<CompressorWriter<BufWriter<File>>>,
+}
 
-        let mut fn_args = Vec::with_capacity(args.len());
+#[pymethods]
+impl PythonTermStreamer {
+    /// Create a new term streamer with a given path for its files,
+    /// the maximum size of the memory buffer and the number of cores.
+    #[new]
+    pub fn __new__(
+        path: Option<&str>,
+        max_mem_bytes: Option<usize>,
+        n_cores: Option<usize>,
+    ) -> PyResult<Self> {
+        let d = TermStreamerConfig::default();
 
-        for arg in args {
-            if let Ok(a) = arg.extract::<ConvertibleToExpression>() {
-                fn_args.push(ExpressionOrTransformer::Expression(a.to_expression()));
-            } else if let Ok(a) = arg.extract::<ConvertibleToPattern>() {
-                fn_args.push(ExpressionOrTransformer::Transformer(a));
-            } else {
-                let msg = format!("Unknown type: {}", arg.get_type().name().unwrap());
-                return Err(exceptions::PyTypeError::new_err(msg));
-            }
-        }
+        Ok(PythonTermStreamer {
+            stream: TermStreamer::new(TermStreamerConfig {
+                n_cores: n_cores.unwrap_or(d.n_cores),
+                max_mem_bytes: max_mem_bytes.unwrap_or(d.max_mem_bytes),
+                path: path.map(|x| x.into()).unwrap_or(d.path),
+            }),
+        })
+    }
 
-        if fn_args
-            .iter()
-            .all(|x| matches!(x, ExpressionOrTransformer::Expression(_)))
-        {
-            // simplify to literal expression
-            Workspace::get_local().with(|workspace| {
-                let mut fun_b = workspace.new_atom();
-                let fun = fun_b.to_fun(self.id);
+    /// Add this expression to `other`, returning the result.
+    pub fn __add__(&mut self, rhs: &mut Self) -> PyResult<Self> {
+        Ok(Self {
+            stream: &mut self.stream + &mut rhs.stream,
+        })
+    }
 
-                for x in fn_args {
-                    if let ExpressionOrTransformer::Expression(a) = x {
-                        fun.add_arg(a.expr.as_view());
-                    }
-                }
+    pub fn __iadd__(&mut self, rhs: &mut Self) {
+        self.stream += &mut rhs.stream;
+    }
 
-                let mut out = Atom::default();
-                fun_b.as_view().normalize(workspace, &mut out);
+    pub fn get_byte_size(&self) -> usize {
+        self.stream.get_byte_size()
+    }
 
-                Ok(PythonExpression {
-                    expr: Arc::new(out),
-                }
-                .into_py(py))
-            })
-        } else {
-            // convert all wildcards back from literals
-            let mut transformer_args = Vec::with_capacity(args.len());
-            for arg in fn_args {
-                match arg {
-                    ExpressionOrTransformer::Transformer(t) => {
-                        transformer_args.push(t.to_pattern()?.expr.as_ref().clone());
-                    }
-                    ExpressionOrTransformer::Expression(a) => {
-                        transformer_args.push(a.expr.as_view().into_pattern().clone());
-                    }
+    /// Add an expression to the term streamer.
+    pub fn push(&mut self, expr: PythonExpression) {
+        self.stream.push(expr.expr.clone());
+    }
+
+    /// Sort and fuse all terms in the streamer.
+    pub fn normalize(&mut self) {
+        self.stream.normalize();
+    }
+
+    /// Convert the term stream into an expression. This may exceed the available memory.
+    pub fn to_expression(&mut self) -> PythonExpression {
+        self.stream.to_expression().into()
+    }
+
+    /// Map the transformations to every term in the streamer.
+    pub fn map(&mut self, op: PythonPattern, py: Python) -> PyResult<Self> {
+        let t = match &op.expr {
+            Pattern::Transformer(t) => {
+                if t.0.is_some() {
+                    return Err(exceptions::PyValueError::new_err(
+                        "Transformer is bound to expression. Use Transformer() instead."
+                            .to_string(),
+                    ));
                 }
+                &t.1
+            }
+            _ => {
+                return Err(exceptions::PyValueError::new_err(
+                    "Operation must of a transformer".to_string(),
+                ));
             }
+        };
 
-            let p = Pattern::Fn(self.id, transformer_args);
-            Ok(PythonPattern { expr: Arc::new(p) }.into_py(py))
-        }
+        // release the GIL as Python functions may be called from
+        // within the term mapper
+        py.allow_threads(move || {
+            // map every term in the expression
+            let m = self.stream.map(|x| {
+                let mut out = Atom::default();
+                Workspace::get_local().with(|ws| {
+                    Transformer::execute(x.as_view(), &t, ws, &mut out).unwrap_or_else(|e| {
+                        // TODO: capture and abort the parallel run
+                        panic!("Transformer failed during parallel execution: {:?}", e)
+                    });
+                });
+                out
+            });
+            Ok::<_, PyErr>(m)
+        })
+        .map(|x| PythonTermStreamer { stream: x })
     }
 }
 
 self_cell!(
-    #[pyclass]
+    #[pyclass(module = "symbolica")]
     pub struct PythonAtomIterator {
-        owner: Arc<Atom>,
+        owner: Atom,
         #[covariant]
         dependent: ListIterator,
     }
 );
 
 impl PythonAtomIterator {
     /// Create a self-referential structure for the iterator.
     pub fn from_expr(expr: PythonExpression) -> PythonAtomIterator {
-        PythonAtomIterator::new(expr.expr, |expr| match expr.as_view() {
+        PythonAtomIterator::new(expr.expr.clone(), |expr| match expr.as_view() {
             AtomView::Add(a) => a.iter(),
             AtomView::Mul(m) => m.iter(),
             AtomView::Fun(f) => f.iter(),
             _ => unreachable!(),
         })
     }
 }
 
 #[pymethods]
 impl PythonAtomIterator {
     fn __next__(&mut self) -> Option<PythonExpression> {
         self.with_dependent_mut(|_, i| {
-            i.next().map(|e| PythonExpression {
-                expr: Arc::new({
-                    let mut owned = Atom::default();
-                    owned.set_from_view(&e);
-                    owned
-                }),
+            i.next().map(|e| {
+                let mut owned = Atom::default();
+                owned.set_from_view(&e);
+                owned.into()
             })
         })
     }
 }
 
 type OwnedMatch = (
-    Arc<Pattern>,
-    Arc<Atom>,
-    Arc<Condition<WildcardAndRestriction>>,
-    Arc<MatchSettings>,
+    Pattern,
+    Atom,
+    Condition<WildcardAndRestriction>,
+    MatchSettings,
 );
 type MatchIterator<'a> = PatternAtomTreeIterator<'a, 'a>;
 
 self_cell!(
     /// An iterator over matches.
-    #[pyclass]
+    #[pyclass(module = "symbolica")]
     pub struct PythonMatchIterator {
         owner: OwnedMatch,
         #[not_covariant]
         dependent: MatchIterator,
     }
 );
 
@@ -3216,45 +3382,38 @@
     /// Return the next match.
     fn __next__(&mut self) -> Option<HashMap<PythonExpression, PythonExpression>> {
         self.with_dependent_mut(|_, i| {
             i.next().map(|(_, _, _, matches)| {
                 matches
                     .into_iter()
                     .map(|m| {
-                        (
-                            PythonExpression {
-                                expr: Arc::new(Atom::new_var(m.0)),
-                            },
-                            PythonExpression {
-                                expr: Arc::new({
-                                    let mut a = Atom::default();
-                                    m.1.to_atom(&mut a);
-                                    a
-                                }),
-                            },
-                        )
+                        (Atom::new_var(m.0).into(), {
+                            let mut a = Atom::default();
+                            m.1.to_atom(&mut a);
+                            a.into()
+                        })
                     })
                     .collect()
             })
         })
     }
 }
 
 type OwnedReplace = (
-    Arc<Pattern>,
-    Arc<Atom>,
-    Arc<Pattern>,
-    Arc<Condition<WildcardAndRestriction>>,
-    Arc<MatchSettings>,
+    Pattern,
+    Atom,
+    Pattern,
+    Condition<WildcardAndRestriction>,
+    MatchSettings,
 );
 type ReplaceIteratorOne<'a> = ReplaceIterator<'a, 'a>;
 
 self_cell!(
     /// An iterator over all single replacements.
-    #[pyclass]
+    #[pyclass(module = "symbolica")]
     pub struct PythonReplaceIterator {
         owner: OwnedReplace,
         #[not_covariant]
         dependent: ReplaceIteratorOne,
     }
 );
 
@@ -3269,26 +3428,24 @@
     fn __next__(&mut self) -> PyResult<Option<PythonExpression>> {
         self.with_dependent_mut(|_, i| {
             let mut out = Atom::default();
 
             if i.next(&mut out).is_none() {
                 Ok(None)
             } else {
-                Ok::<_, PyErr>(Some(PythonExpression {
-                    expr: Arc::new(out),
-                }))
+                Ok::<_, PyErr>(Some(out.into()))
             }
         })
     }
 }
 
-#[pyclass(name = "Polynomial")]
+#[pyclass(name = "Polynomial", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonPolynomial {
-    pub poly: Arc<MultivariatePolynomial<RationalField, u16>>,
+    pub poly: MultivariatePolynomial<RationalField, u16>,
 }
 
 #[pymethods]
 impl PythonPolynomial {
     /// Parse a polynomial with rational coefficients from a string.
     /// The input must be written in an expanded format and a list of all
     /// the variables must be provided.
@@ -3317,15 +3474,15 @@
         }
 
         let e = Token::parse(arg)
             .map_err(exceptions::PyValueError::new_err)?
             .to_polynomial(&Q, &Arc::new(var_map), &var_name_map)
             .map_err(exceptions::PyValueError::new_err)?;
 
-        Ok(Self { poly: Arc::new(e) })
+        Ok(Self { poly: e })
     }
 
     /// Convert the polynomial to a polynomial with integer coefficients, if possible.
     pub fn to_integer_polynomial(&self) -> PyResult<PythonIntegerPolynomial> {
         let mut poly_int =
             MultivariatePolynomial::new(&Z, Some(self.poly.nterms()), self.poly.variables.clone());
 
@@ -3349,24 +3506,22 @@
                 }
                 new_exponent.push(*e as u8);
             }
 
             poly_int.append_monomial(t.coefficient.numerator(), &new_exponent);
         }
 
-        Ok(PythonIntegerPolynomial {
-            poly: Arc::new(poly_int),
-        })
+        Ok(PythonIntegerPolynomial { poly: poly_int })
     }
 
     /// Convert the coefficients of the polynomial to a finite field with prime `prime`.
     pub fn to_finite_field(&self, prime: u32) -> PythonFiniteFieldPolynomial {
         let f = Zp::new(prime);
         PythonFiniteFieldPolynomial {
-            poly: Arc::new(self.poly.map_coeff(|c| c.to_finite_field(&f), f.clone())),
+            poly: self.poly.map_coeff(|c| c.to_finite_field(&f), f.clone()),
         }
     }
 
     /// Optimize the polynomial for evaluation using `iterations` number of iterations.
     /// The optimized output can be exported in a C++ format using `to_file`.
     ///
     /// Returns an evaluator for the polynomial.
@@ -3393,15 +3548,15 @@
                 ),
             )
             .unwrap();
         }
 
         let o_f64 = o.convert::<f64>();
         Ok(PythonInstructionEvaluator {
-            instr: Arc::new(o_f64.evaluator()),
+            instr: o_f64.evaluator(),
         })
     }
 
     /// Compute the Groebner basis of a polynomial system.
     ///
     /// If `grevlex=True`, reverse graded lexicographical ordering is used,
     /// otherwise the ordering is lexicographical.
@@ -3434,34 +3589,31 @@
                 .map(|p| p.poly.reorder::<GrevLexOrder>())
                 .collect();
             let gb = GroebnerBasis::new(&grevlex_ideal, print_stats);
 
             gb.system
                 .into_iter()
                 .map(|p| Self {
-                    poly: Arc::new(p.reorder::<LexOrder>()),
+                    poly: p.reorder::<LexOrder>(),
                 })
                 .collect()
         } else {
-            let ideal: Vec<_> = system.iter().map(|p| p.poly.as_ref().clone()).collect();
+            let ideal: Vec<_> = system.iter().map(|p| p.poly.clone()).collect();
             let gb = GroebnerBasis::new(&ideal, print_stats);
-            gb.system
-                .into_iter()
-                .map(|p| Self { poly: Arc::new(p) })
-                .collect()
+            gb.system.into_iter().map(|p| Self { poly: p }).collect()
         }
     }
 
     /// Integrate the polynomial in `x`.
     ///
     /// Examples
     /// --------
     ///
     /// >>> from symbolica import Expression
-    /// >>> x = Expression.var('x')
+    /// >>> x = Expression.symbol('x')
     /// >>> p = Expression.parse('x^2+2').to_polynomial()
     /// >>> print(p.integrate(x))
     pub fn integrate(&self, x: PythonExpression) -> PyResult<Self> {
         let x = self
             .poly
             .get_vars_ref()
             .iter()
@@ -3472,58 +3624,56 @@
             })
             .ok_or(exceptions::PyValueError::new_err(format!(
                 "Variable {} not found in polynomial",
                 x.__str__()?
             )))?;
 
         Ok(Self {
-            poly: Arc::new(self.poly.integrate(x)),
+            poly: self.poly.integrate(x),
         })
     }
 
     /// Convert the polynomial to an expression.
     ///
     /// Examples
     /// --------
     ///
     /// >>> from symbolica import Expression
-    /// >>> x = Expression.var('x')
+    /// >>> x = Expression.symbol('x')
     /// >>> e = Expression.parse('x*y+2*x+x^2')
     /// >>> p = e.to_polynomial()
     /// >>> print(e - p.to_expression())
     pub fn to_expression(&self) -> PyResult<PythonExpression> {
-        Ok(PythonExpression {
-            expr: Arc::new(self.poly.to_expression()),
-        })
+        Ok(self.poly.to_expression().into())
     }
 }
 
-#[pyclass(name = "Evaluator")]
+#[pyclass(name = "Evaluator", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonInstructionEvaluator {
-    pub instr: Arc<InstructionEvaluator<f64>>,
+    pub instr: InstructionEvaluator<f64>,
 }
 
 #[pymethods]
 impl PythonInstructionEvaluator {
     /// Evaluate the polynomial for multiple inputs and return the result.
     fn evaluate(&self, inputs: Vec<Vec<f64>>) -> Vec<f64> {
-        let mut eval = (*self.instr).clone();
+        let mut eval = self.instr.clone();
 
         inputs
             .iter()
             .map(|s| eval.evaluate_with_input(s)[0])
             .collect()
     }
 }
 
-#[pyclass(name = "IntegerPolynomial")]
+#[pyclass(name = "IntegerPolynomial", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonIntegerPolynomial {
-    pub poly: Arc<MultivariatePolynomial<IntegerRing, u8>>,
+    pub poly: MultivariatePolynomial<IntegerRing, u8>,
 }
 
 #[pymethods]
 impl PythonIntegerPolynomial {
     /// Parse a polynomial with integer coefficients from a string.
     /// The input must be written in an expanded format and a list of all
     /// the variables must be provided.
@@ -3551,38 +3701,36 @@
         }
 
         let e = Token::parse(arg)
             .map_err(exceptions::PyValueError::new_err)?
             .to_polynomial(&Z, &Arc::new(var_map), &var_name_map)
             .map_err(exceptions::PyValueError::new_err)?;
 
-        Ok(Self { poly: Arc::new(e) })
+        Ok(Self { poly: e })
     }
 
     /// Convert the polynomial to an expression.
     ///
     /// Examples
     /// --------
     ///
     /// >>> from symbolica import Expression
     /// >>> e = Expression.parse('x*y+2*x+x^2')
     /// >>> p = e.to_polynomial()
     /// >>> print((e - p.to_expression()).expand())
     pub fn to_expression(&self) -> PyResult<PythonExpression> {
-        Ok(PythonExpression {
-            expr: Arc::new(self.poly.to_expression()),
-        })
+        Ok(self.poly.to_expression().into())
     }
 }
 
 /// A Symbolica polynomial over finite fields.
-#[pyclass(name = "FiniteFieldPolynomial")]
+#[pyclass(name = "FiniteFieldPolynomial", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonFiniteFieldPolynomial {
-    pub poly: Arc<MultivariatePolynomial<Zp, u16>>,
+    pub poly: MultivariatePolynomial<Zp, u16>,
 }
 
 #[pymethods]
 impl PythonFiniteFieldPolynomial {
     /// Parse a polynomial with integer coefficients from a string.
     /// The input must be written in an expanded format and a list of all
     /// the variables must be provided.
@@ -3610,15 +3758,15 @@
         }
 
         let e = Token::parse(arg)
             .map_err(exceptions::PyValueError::new_err)?
             .to_polynomial(&Zp::new(prime), &Arc::new(var_map), &var_name_map)
             .map_err(exceptions::PyValueError::new_err)?;
 
-        Ok(Self { poly: Arc::new(e) })
+        Ok(Self { poly: e })
     }
 
     /// Compute the Groebner basis of a polynomial system.
     ///
     /// If `grevlex=True`, reverse graded lexicographical ordering is used,
     /// otherwise the ordering is lexicographical.
     ///
@@ -3637,34 +3785,31 @@
                 .map(|p| p.poly.reorder::<GrevLexOrder>())
                 .collect();
             let gb = GroebnerBasis::new(&grevlex_ideal, print_stats);
 
             gb.system
                 .into_iter()
                 .map(|p| Self {
-                    poly: Arc::new(p.reorder::<LexOrder>()),
+                    poly: p.reorder::<LexOrder>(),
                 })
                 .collect()
         } else {
-            let ideal: Vec<_> = system.iter().map(|p| p.poly.as_ref().clone()).collect();
+            let ideal: Vec<_> = system.iter().map(|p| p.poly.clone()).collect();
             let gb = GroebnerBasis::new(&ideal, print_stats);
-            gb.system
-                .into_iter()
-                .map(|p| Self { poly: Arc::new(p) })
-                .collect()
+            gb.system.into_iter().map(|p| Self { poly: p }).collect()
         }
     }
 
     /// Integrate the polynomial in `x`.
     ///
     /// Examples
     /// --------
     ///
     /// >>> from symbolica import Expression
-    /// >>> x = Expression.var('x')
+    /// >>> x = Expression.symbol('x')
     /// >>> p = Expression.parse('x^2+2').to_polynomial()
     /// >>> print(p.integrate(x))
     pub fn integrate(&self, x: PythonExpression) -> PyResult<Self> {
         let x = self
             .poly
             .get_vars_ref()
             .iter()
@@ -3675,15 +3820,15 @@
             })
             .ok_or(exceptions::PyValueError::new_err(format!(
                 "Variable {} not found in polynomial",
                 x.__str__()?
             )))?;
 
         Ok(Self {
-            poly: Arc::new(self.poly.integrate(x)),
+            poly: self.poly.integrate(x),
         })
     }
 }
 
 macro_rules! generate_methods {
     ($type:ty, $exp_type:ty) => {
         #[pymethods]
@@ -3722,15 +3867,15 @@
                     }
                 }
             }
 
             /// Copy the polynomial.
             pub fn __copy__(&self) -> Self {
                 Self {
-                    poly: Arc::new((*self.poly).clone()),
+                    poly: self.poly.clone(),
                 }
             }
 
             /// Convert the polynomial into a human-readable string, with tunable settings.
             ///
             /// Examples
             /// --------
@@ -3814,129 +3959,125 @@
             /// Get the list of variables in the internal ordering of the polynomial.
             pub fn get_var_list(&self) -> PyResult<Vec<PythonExpression>> {
                 let mut var_list = vec![];
 
                 for x in self.poly.get_vars_ref() {
                     match x {
                         Variable::Symbol(x) => {
-                            var_list.push(PythonExpression {
-                                expr: Arc::new(Atom::new_var(*x)),
-                            });
+                            var_list.push(Atom::new_var(*x).into());
                         }
                         Variable::Temporary(_) => {
                             Err(exceptions::PyValueError::new_err(format!(
                                 "Temporary variable in polynomial",
                             )))?;
                         }
                         Variable::Function(_, a) | Variable::Other(a) => {
-                            var_list.push(PythonExpression {
-                                expr: a.clone(),
-                            });
+                            var_list.push(a.as_ref().clone().into());
                         }
                     }
                 }
 
                 Ok(var_list)
             }
 
             /// Add two polynomials `self and `rhs`, returning the result.
             pub fn __add__(&self, rhs: Self) -> Self {
                 if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
                     Self {
-                        poly: Arc::new((*self.poly).clone() + (*rhs.poly).clone()),
+                        poly: self.poly.clone() + rhs.poly.clone(),
                     }
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Self {
-                        poly: Arc::new(new_self + new_rhs),
+                        poly: new_self + new_rhs,
                     }
                 }
             }
 
             /// Subtract polynomials `rhs` from `self`, returning the result.
             pub fn __sub__(&self, rhs: Self) -> Self {
                 self.__add__(rhs.__neg__())
             }
 
             /// Multiply two polynomials `self and `rhs`, returning the result.
             pub fn __mul__(&self, rhs: Self) -> Self {
                 if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
                     Self {
-                        poly: Arc::new(&*self.poly * &*rhs.poly),
+                        poly: &self.poly * &rhs.poly,
                     }
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Self {
-                        poly: Arc::new(new_self * &new_rhs),
+                        poly: new_self * &new_rhs,
                     }
                 }
             }
 
             /// Divide the polynomial `self` by `rhs` if possible, returning the result.
             pub fn __truediv__(&self, rhs: Self) -> PyResult<Self> {
                 let (q, r) = if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
                     self.poly.quot_rem(&rhs.poly, false)
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
 
                     new_self.quot_rem(&new_rhs, false)
                 };
 
                 if r.is_zero() {
-                    Ok(Self { poly: Arc::new(q) })
+                    Ok(Self { poly: q })
                 } else {
                     Err(exceptions::PyValueError::new_err(format!(
                         "The division has a remainder: {}",
                         r
                     )))
                 }
             }
 
             /// Divide `self` by `rhs`, returning the quotient and remainder.
             pub fn quot_rem(&self, rhs: Self) -> (Self, Self) {
                 if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
                     let (q, r) = self.poly.quot_rem(&rhs.poly, false);
 
-                    (Self { poly: Arc::new(q) }, Self { poly: Arc::new(r) })
+                    (Self { poly: q }, Self { poly: r })
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
 
                     let (q, r) = new_self.quot_rem(&new_rhs, false);
 
-                    (Self { poly: Arc::new(q) }, Self { poly: Arc::new(r) })
+                    (Self { poly: q }, Self { poly: r })
                 }
             }
 
             /// Negate the polynomial.
             pub fn __neg__(&self) -> Self {
                 Self {
-                    poly: Arc::new((*self.poly).clone().neg()),
+                    poly: self.poly.clone().neg(),
                 }
             }
 
             /// Compute the greatest common divisor (GCD) of two polynomials.
             pub fn gcd(&self, rhs: Self) -> Self {
                 if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
                     Self {
-                        poly: Arc::new(self.poly.gcd(&rhs.poly)),
+                        poly: self.poly.gcd(&rhs.poly),
                     }
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Self {
-                        poly: Arc::new(new_self.gcd(&new_rhs)),
+                        poly: new_self.gcd(&new_rhs),
                     }
                 }
             }
 
             /// Compute the resultant of two polynomials with respect to the variable `var`.
             pub fn resultant(&self, rhs: Self, var: PythonExpression) -> PyResult<Self> {
                 let x = self.poly.get_vars_ref().iter().position(|v| match (v, var.expr.as_view()) {
@@ -3950,26 +4091,26 @@
 
 
                 if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
                     let self_uni = self.poly.to_univariate(x);
                     let rhs_uni = rhs.poly.to_univariate(x);
 
                     Ok(Self {
-                        poly: Arc::new(self_uni.resultant_prs(&rhs_uni)),
+                        poly: self_uni.resultant_prs(&rhs_uni),
                     })
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
 
                     let self_uni = new_self.to_univariate(x);
                     let rhs_uni = new_rhs.to_univariate(x);
 
                     Ok(Self {
-                        poly: Arc::new(self_uni.resultant_prs(&rhs_uni)),
+                        poly: self_uni.resultant_prs(&rhs_uni),
                     })
                 }
             }
 
             /// Compute the square-free factorization of the polynomial.
             ///
             /// Examples
@@ -3980,15 +4121,15 @@
             /// >>> print('Square-free factorization of {}:'.format(p))
             /// >>> for f, exp in p.factor_square_free():
             /// >>>     print('\t({})^{}'.format(f, exp))
             pub fn factor_square_free(&self) -> Vec<(Self, usize)> {
                 self.poly
                     .square_free_factorization()
                     .into_iter()
-                    .map(|(f, p)| (Self { poly: Arc::new(f) }, p))
+                    .map(|(f, p)| (Self { poly: f }, p))
                     .collect()
             }
 
             /// Factorize the polynomial.
             ///
             /// Examples
             /// --------
@@ -3998,83 +4139,83 @@
             /// >>> print('Factorization of {}:'.format(p))
             /// >>> for f, exp in p.factor():
             /// >>>     print('\t({})^{}'.format(f, exp))
             pub fn factor(&self) -> Vec<(Self, usize)> {
                 self.poly
                     .factor()
                     .into_iter()
-                    .map(|(f, p)| (Self { poly: Arc::new(f) }, p))
+                    .map(|(f, p)| (Self { poly: f }, p))
                     .collect()
             }
 
             /// Take a derivative in `x`.
             ///
             /// Examples
             /// --------
             ///
             /// >>> from symbolica import Expression
-            /// >>> x = Expression.var('x')
+            /// >>> x = Expression.symbol('x')
             /// >>> p = Expression.parse('x^2+2').to_polynomial()
             /// >>> print(p.derivative(x))
             pub fn derivative(&self, x: PythonExpression) -> PyResult<Self> {
                 let x = self.poly.get_vars_ref().iter().position(|v| match (v, x.expr.as_view()) {
                     (Variable::Symbol(y), AtomView::Var(vv)) => *y == vv.get_symbol(),
                     (Variable::Function(_, f) | Variable::Other(f), a) => f.as_view() == a,
                     _ => false,
                 }).ok_or(exceptions::PyValueError::new_err(format!(
                     "Variable {} not found in polynomial",
                     x.__str__()?
                 )))?;
 
-                Ok(Self { poly: Arc::new(self.poly.derivative(x))})
+                Ok(Self { poly: self.poly.derivative(x)})
             }
 
             /// Get the content, i.e., the GCD of the coefficients.
             ///
             /// Examples
             /// --------
             ///
             /// >>> from symbolica import Expression
             /// >>> p = Expression.parse('3x^2+6x+9').to_polynomial()
             /// >>> print(p.content())
             pub fn content(&self) -> PyResult<Self> {
-                Ok(Self { poly: Arc::new(self.poly.constant(self.poly.content()))})
+                Ok(Self { poly: self.poly.constant(self.poly.content())})
             }
 
             /// Get the coefficient list in `x`.
             ///
             /// Examples
             /// --------
             ///
             /// >>> from symbolica import Expression
-            /// >>> x = Expression.var('x')
+            /// >>> x = Expression.symbol('x')
             /// >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
             /// >>> for n, pp in p.coefficient_list(x):
             /// >>>     print(n, pp)
             pub fn coefficient_list(&self, var: PythonExpression) -> PyResult<Vec<(usize, Self)>> {
                 let x = self.poly.get_vars_ref().iter().position(|v| match (v, var.expr.as_view()) {
                     (Variable::Symbol(y), AtomView::Var(vv)) => *y == vv.get_symbol(),
                     (Variable::Function(_, f) | Variable::Other(f), a) => f.as_view() == a,
                     _ => false,
                 }).ok_or(exceptions::PyValueError::new_err(format!(
                     "Variable {} not found in polynomial",
                     var.__str__()?
                 )))?;
 
                 Ok(self.poly.to_univariate_polynomial_list(x).into_iter()
-                    .map(|(f, p)| (p as usize, Self { poly: Arc::new(f) })).collect())
+                    .map(|(f, p)| (p as usize, Self { poly: f })).collect())
             }
 
             /// Replace the variable `x` with a polynomial `v`.
             ///
             /// Examples
             /// --------
             ///
             /// >>> from symbolica import Expression
-            /// >>> x = Expression.var('x')
+            /// >>> x = Expression.symbol('x')
             /// >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
             /// >>> r = Expression.parse('y+1').to_polynomial())
             /// >>> p.replace(x, r)
             pub fn replace(&self, x: PythonExpression, v: Self) -> PyResult<Self> {
                 let id = match x.expr.as_view() {
                     AtomView::Var(x) => {
                         x.get_symbol()
@@ -4092,82 +4233,77 @@
                 }).ok_or(exceptions::PyValueError::new_err(format!(
                     "Variable {} not found in polynomial",
                     x.__str__()?
                 )))?;
 
                 if self.poly.get_vars_ref() == v.poly.get_vars_ref() {
                     Ok(Self {
-                        poly: Arc::new(self.poly.replace_with_poly(x, &v.poly))
+                        poly: self.poly.replace_with_poly(x, &v.poly)
                     })
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*v.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = v.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Ok(Self {
-                        poly: Arc::new(new_self.replace_with_poly(x, &new_rhs))
+                        poly: new_self.replace_with_poly(x, &new_rhs)
                     })
                 }
             }
         }
     };
 }
 
 generate_methods!(PythonPolynomial, u16);
 generate_methods!(PythonIntegerPolynomial, u8);
 generate_methods!(PythonFiniteFieldPolynomial, u16);
 
 /// A Symbolica rational polynomial.
-#[pyclass(name = "RationalPolynomial")]
+#[pyclass(name = "RationalPolynomial", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonRationalPolynomial {
-    pub poly: Arc<RationalPolynomial<IntegerRing, u16>>,
+    pub poly: RationalPolynomial<IntegerRing, u16>,
 }
 
 #[pymethods]
 impl PythonRationalPolynomial {
     /// Create a new rational polynomial from a numerator and denominator polynomial.
     #[new]
     pub fn __new__(num: &PythonPolynomial, den: &PythonPolynomial) -> Self {
         Self {
-            poly: Arc::new(RationalPolynomial::from_num_den(
-                (*num.poly).clone(),
-                (*den.poly).clone(),
-                &Z,
-                true,
-            )),
+            poly: RationalPolynomial::from_num_den(num.poly.clone(), den.poly.clone(), &Z, true),
         }
     }
 
     /// Convert the coefficients to finite fields with prime `prime`.
     pub fn to_finite_field(&self, prime: u32) -> PythonFiniteFieldRationalPolynomial {
         PythonFiniteFieldRationalPolynomial {
-            poly: Arc::new(self.poly.to_finite_field(&Zp::new(prime))),
+            poly: self.poly.to_finite_field(&Zp::new(prime)),
         }
     }
 
     /// Get the numerator.
     pub fn numerator(&self) -> PythonPolynomial {
         PythonPolynomial {
-            poly: Arc::new((&self.poly.numerator).into()),
+            poly: (&self.poly.numerator).into(),
         }
     }
 
     /// Get the denominator.
     pub fn denominator(&self) -> PythonPolynomial {
         PythonPolynomial {
-            poly: Arc::new((&self.poly.denominator).into()),
+            poly: (&self.poly.denominator).into(),
         }
     }
 }
 
 /// A Symbolica rational polynomial with variable powers limited to 255.
-#[pyclass(name = "RationalPolynomialSmallExponent")]
+#[pyclass(name = "RationalPolynomialSmallExponent", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonRationalPolynomialSmallExponent {
-    pub poly: Arc<RationalPolynomial<IntegerRing, u8>>,
+    pub poly: RationalPolynomial<IntegerRing, u8>,
 }
 
 macro_rules! generate_rat_parse {
     ($type:ty) => {
         #[pymethods]
         impl $type {
             /// Parse a rational polynomial from a string.
@@ -4196,43 +4332,41 @@
                 }
 
                 let e = Token::parse(arg)
                     .map_err(exceptions::PyValueError::new_err)?
                     .to_rational_polynomial(&Q, &Z, &Arc::new(var_map), &var_name_map)
                     .map_err(exceptions::PyValueError::new_err)?;
 
-                Ok(Self { poly: Arc::new(e) })
+                Ok(Self { poly: e })
             }
 
             /// Convert the rational polynomial to an expression.
             ///
             /// Examples
             /// --------
             ///
             /// >>> from symbolica import Expression
             /// >>> e = Expression.parse('(x*y+2*x+x^2)/(1+y^2+x^7)')
             /// >>> p = e.to_rational_polynomial()
             /// >>> print((e - p.to_expression()).expand())
             pub fn to_expression(&self) -> PyResult<PythonExpression> {
-                Ok(PythonExpression {
-                    expr: Arc::new(self.poly.to_expression()),
-                })
+                Ok(self.poly.to_expression().into())
             }
         }
     };
 }
 
 generate_rat_parse!(PythonRationalPolynomial);
 generate_rat_parse!(PythonRationalPolynomialSmallExponent);
 
 /// A Symbolica rational polynomial over finite fields.
-#[pyclass(name = "FiniteFieldRationalPolynomial")]
+#[pyclass(name = "FiniteFieldRationalPolynomial", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonFiniteFieldRationalPolynomial {
-    pub poly: Arc<RationalPolynomial<Zp, u16>>,
+    pub poly: RationalPolynomial<Zp, u16>,
 }
 
 #[pymethods]
 impl PythonFiniteFieldRationalPolynomial {
     /// Parse a rational polynomial from a string.
     /// The list of all the variables must be provided.
     ///
@@ -4260,27 +4394,27 @@
 
         let field = Zp::new(prime);
         let e = Token::parse(arg)
             .map_err(exceptions::PyValueError::new_err)?
             .to_rational_polynomial(&field, &field, &Arc::new(var_map), &var_name_map)
             .map_err(exceptions::PyValueError::new_err)?;
 
-        Ok(Self { poly: Arc::new(e) })
+        Ok(Self { poly: e })
     }
 }
 
 // TODO: unify with polynomial methods
 macro_rules! generate_rat_methods {
     ($type:ty) => {
         #[pymethods]
         impl $type {
             /// Copy the rational polynomial.
             pub fn __copy__(&self) -> Self {
                 Self {
-                    poly: Arc::new((*self.poly).clone()),
+                    poly: self.poly.clone(),
                 }
             }
 
             /// Compare two polynomials.
             fn __richcmp__(&self, other: &Self, op: CompareOp) -> PyResult<bool> {
                 match op {
                     CompareOp::Eq => Ok(self.poly == other.poly),
@@ -4307,27 +4441,23 @@
             /// Get the list of variables in the internal ordering of the polynomial.
             pub fn get_var_list(&self) -> PyResult<Vec<PythonExpression>> {
                 let mut var_list = vec![];
 
                 for x in self.poly.get_variables().iter() {
                     match x {
                         Variable::Symbol(x) => {
-                            var_list.push(PythonExpression {
-                                expr: Arc::new(Atom::new_var(*x)),
-                            });
+                            var_list.push(Atom::new_var(*x).into());
                         }
                         Variable::Temporary(_) => {
                             Err(exceptions::PyValueError::new_err(format!(
                                 "Temporary variable in polynomial",
                             )))?;
                         }
                         Variable::Function(_, a) | Variable::Other(a) => {
-                            var_list.push(PythonExpression {
-                                expr: a.clone(),
-                            });
+                            var_list.push(a.as_ref().clone().into());
                         }
                     }
                 }
 
                 Ok(var_list)
             }
 
@@ -4354,104 +4484,104 @@
                 ))
             }
 
             /// Add two rational polynomials `self and `rhs`, returning the result.
             pub fn __add__(&self, rhs: Self) -> Self {
                 if self.poly.get_variables() == rhs.poly.get_variables() {
                     Self {
-                        poly: Arc::new(&*self.poly + &*rhs.poly),
+                        poly: &self.poly + &rhs.poly,
                     }
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Self {
-                        poly: Arc::new(&new_self + &new_rhs),
+                        poly: &new_self + &new_rhs,
                     }
                 }
             }
 
             /// Subtract rational polynomials `rhs` from `self`, returning the result.
             pub fn __sub__(&self, rhs: Self) -> Self {
                 if self.poly.get_variables() == rhs.poly.get_variables() {
                     Self {
-                        poly: Arc::new(&*self.poly - &*rhs.poly),
+                        poly: &self.poly - &rhs.poly,
                     }
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Self {
-                        poly: Arc::new(&new_self - &new_rhs),
+                        poly: &new_self - &new_rhs,
                     }
                 }
             }
 
             /// Multiply two rational polynomials `self and `rhs`, returning the result.
             pub fn __mul__(&self, rhs: Self) -> Self {
                 if self.poly.get_variables() == rhs.poly.get_variables() {
                     Self {
-                        poly: Arc::new(&*self.poly * &*rhs.poly),
+                        poly: &self.poly * &rhs.poly,
                     }
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Self {
-                        poly: Arc::new(&new_self * &new_rhs),
+                        poly: &new_self * &new_rhs,
                     }
                 }
             }
 
             /// Divide the rational polynomial `self` by `rhs` if possible, returning the result.
             pub fn __truediv__(&self, rhs: Self) -> Self {
                 if self.poly.get_variables() == rhs.poly.get_variables() {
                     Self {
-                        poly: Arc::new(&*self.poly * &*rhs.poly),
+                        poly: &self.poly * &rhs.poly,
                     }
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Self {
-                        poly: Arc::new(&new_self / &new_rhs),
+                        poly: &new_self / &new_rhs,
                     }
                 }
             }
 
             /// Negate the rational polynomial.
             pub fn __neg__(&self) -> Self {
                 Self {
-                    poly: Arc::new((*self.poly).clone().neg()),
+                    poly: self.poly.clone().neg(),
                 }
             }
 
             /// Compute the greatest common divisor (GCD) of two rational polynomials.
             pub fn gcd(&self, rhs: Self) -> Self {
                 if self.poly.get_variables() == rhs.poly.get_variables() {
                     Self {
-                        poly: Arc::new(self.poly.gcd(&rhs.poly)),
+                        poly: self.poly.gcd(&rhs.poly),
                     }
                 } else {
-                    let mut new_self = (*self.poly).clone();
-                    let mut new_rhs = (*rhs.poly).clone();
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
                     Self {
-                        poly: Arc::new(new_self.gcd(&new_rhs)),
+                        poly: new_self.gcd(&new_rhs),
                     }
                 }
             }
 
             /// Compute the partial fraction decomposition in `x`.
             ///
             /// Examples
             /// --------
             ///
             /// >>> from symbolica import Expression
-            /// >>> x = Expression.var('x')
+            /// >>> x = Expression.symbol('x')
             /// >>> p = Expression.parse('1/((x+y)*(x^2+x*y+1)(x+1))').to_rational_polynomial()
             /// >>> for pp in p.apart(x):
             /// >>>     print(pp)
             pub fn apart(&self, x: PythonExpression) -> PyResult<Vec<Self>> {
                 let id = match x.expr.as_view() {
                     AtomView::Var(x) => {
                         x.get_symbol()
@@ -4468,15 +4598,15 @@
                     _ => false,
                 }).ok_or(exceptions::PyValueError::new_err(format!(
                     "Variable {} not found in polynomial",
                     x.__str__()?
                 )))?;
 
                 Ok(self.poly.apart(x).into_iter()
-                    .map(|f| Self { poly: Arc::new(f) }).collect())
+                    .map(|f| Self { poly: f }).collect())
             }
         }
     };
 }
 
 generate_rat_methods!(PythonRationalPolynomial);
 generate_rat_methods!(PythonRationalPolynomialSmallExponent);
@@ -4493,43 +4623,41 @@
         match self {
             Self::Literal(l) => Ok(l),
             Self::Expression(e) => {
                 let expr = &e.to_expression().expr;
 
                 let poly = expr.to_rational_polynomial(&Q, &Z, None);
 
-                Ok(PythonRationalPolynomial {
-                    poly: Arc::new(poly),
-                })
+                Ok(PythonRationalPolynomial { poly })
             }
         }
     }
 }
 
 #[derive(FromPyObject)]
 pub enum ScalarOrMatrix {
     Scalar(ConvertibleToRationalPolynomial),
     Matrix(PythonMatrix),
 }
 
 /// A Symbolica matrix with rational polynomial coefficients.
-#[pyclass(name = "Matrix")]
+#[pyclass(name = "Matrix", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonMatrix {
-    pub matrix: Arc<Matrix<RationalPolynomialField<IntegerRing, u16>>>,
+    pub matrix: Matrix<RationalPolynomialField<IntegerRing, u16>>,
 }
 
 impl PythonMatrix {
     fn unify(&self, rhs: &PythonMatrix) -> (PythonMatrix, PythonMatrix) {
         if self.matrix.field == rhs.matrix.field {
             return (self.clone(), rhs.clone());
         }
 
-        let mut new_self = self.matrix.as_ref().clone();
-        let mut new_rhs = rhs.matrix.as_ref().clone();
+        let mut new_self = self.matrix.clone();
+        let mut new_rhs = rhs.matrix.clone();
 
         let mut zero = self.matrix.field.zero();
 
         zero.unify_variables(&mut new_rhs[(0, 0)]);
         new_self.field = RationalPolynomialField::new(Z, zero.numerator.get_vars());
         new_rhs.field = new_self.field.clone();
 
@@ -4538,51 +4666,43 @@
             zero.unify_variables(e);
         }
         for e in &mut new_rhs.data {
             zero.unify_variables(e);
         }
 
         (
-            PythonMatrix {
-                matrix: Arc::new(new_self),
-            },
-            PythonMatrix {
-                matrix: Arc::new(new_rhs),
-            },
+            PythonMatrix { matrix: new_self },
+            PythonMatrix { matrix: new_rhs },
         )
     }
 
     fn unify_scalar(
         &self,
         rhs: &PythonRationalPolynomial,
     ) -> (PythonMatrix, PythonRationalPolynomial) {
         if self.matrix.field == RationalPolynomialField::new(Z, rhs.poly.numerator.get_vars()) {
             return (self.clone(), rhs.clone());
         }
 
-        let mut new_self = self.matrix.as_ref().clone();
-        let mut new_rhs = rhs.poly.as_ref().clone();
+        let mut new_self = self.matrix.clone();
+        let mut new_rhs = rhs.poly.clone();
 
         let mut zero = self.matrix.field.zero();
 
         zero.unify_variables(&mut new_rhs);
         new_self.field = RationalPolynomialField::new(Z, zero.numerator.get_vars());
 
         // now update every element
         for e in &mut new_self.data {
             zero.unify_variables(e);
         }
 
         (
-            PythonMatrix {
-                matrix: Arc::new(new_self),
-            },
-            PythonRationalPolynomial {
-                poly: Arc::new(new_rhs),
-            },
+            PythonMatrix { matrix: new_self },
+            PythonRationalPolynomial { poly: new_rhs },
         )
     }
 }
 
 #[pymethods]
 impl PythonMatrix {
     /// Create a new zeroed matrix with `nrows` rows and `ncols` columns.
@@ -4591,36 +4711,33 @@
         if nrows == 0 || ncols == 0 {
             return Err(exceptions::PyValueError::new_err(
                 "The matrix must have at least one row and one column",
             ));
         }
 
         Ok(PythonMatrix {
-            matrix: Arc::new(Matrix::new(
+            matrix: Matrix::new(
                 nrows,
                 ncols,
                 RationalPolynomialField::new(Z, Arc::new(vec![])),
-            )),
+            ),
         })
     }
 
     /// Create a new square matrix with `nrows` rows and ones on the main diagonal and zeroes elsewhere.
     #[classmethod]
     pub fn identity(_cls: &PyType, nrows: u32) -> PyResult<PythonMatrix> {
         if nrows == 0 {
             return Err(exceptions::PyValueError::new_err(
                 "The matrix must have at least one row and one column",
             ));
         }
 
         Ok(PythonMatrix {
-            matrix: Arc::new(Matrix::identity(
-                nrows,
-                RationalPolynomialField::new(Z, Arc::new(vec![])),
-            )),
+            matrix: Matrix::identity(nrows, RationalPolynomialField::new(Z, Arc::new(vec![]))),
         })
     }
 
     /// Create a new matrix with the scalars `diag` on the main diagonal and zeroes elsewhere.
     #[classmethod]
     pub fn eye(
         _cls: &PyType,
@@ -4630,29 +4747,29 @@
             return Err(exceptions::PyValueError::new_err(
                 "The diagonal must have at least one entry",
             ));
         }
 
         let mut diag: Vec<_> = diag
             .into_iter()
-            .map(|x| Ok(x.to_rational_polynomial()?.poly.as_ref().clone()))
+            .map(|x| Ok(x.to_rational_polynomial()?.poly.clone()))
             .collect::<PyResult<_>>()?;
 
         // unify the entries
         let (first, rest) = diag.split_first_mut().unwrap();
         for _ in 0..2 {
             for x in &mut *rest {
                 first.unify_variables(x);
             }
         }
 
         let field = RationalPolynomialField::new(Z, first.numerator.get_vars());
 
         Ok(PythonMatrix {
-            matrix: Arc::new(Matrix::eye(&diag, field)),
+            matrix: Matrix::eye(&diag, field),
         })
     }
 
     /// Create a new row vector from a list of scalars.
     #[classmethod]
     pub fn vec(
         _cls: &PyType,
@@ -4662,29 +4779,29 @@
             return Err(exceptions::PyValueError::new_err(
                 "The matrix must have at least one row and one column",
             ));
         }
 
         let mut entries: Vec<_> = entries
             .into_iter()
-            .map(|x| Ok(x.to_rational_polynomial()?.poly.as_ref().clone()))
+            .map(|x| Ok(x.to_rational_polynomial()?.poly.clone()))
             .collect::<PyResult<_>>()?;
 
         // unify the entries
         let (first, rest) = entries.split_first_mut().unwrap();
         for _ in 0..2 {
             for x in &mut *rest {
                 first.unify_variables(x);
             }
         }
 
         let field = RationalPolynomialField::new(Z, first.numerator.get_vars());
 
         Ok(PythonMatrix {
-            matrix: Arc::new(Matrix::new_vec(entries, field)),
+            matrix: Matrix::new_vec(entries, field),
         })
     }
 
     /// Create a new row vector from a list of scalars.
     #[classmethod]
     pub fn from_linear(
         _cls: &PyType,
@@ -4696,33 +4813,30 @@
             return Err(exceptions::PyValueError::new_err(
                 "The matrix must have at least one row and one column",
             ));
         }
 
         let mut entries: Vec<_> = entries
             .into_iter()
-            .map(|x| Ok(x.to_rational_polynomial()?.poly.as_ref().clone()))
+            .map(|x| Ok(x.to_rational_polynomial()?.poly.clone()))
             .collect::<PyResult<_>>()?;
 
         // unify the entries
         let (first, rest) = entries.split_first_mut().unwrap();
         for _ in 0..2 {
             for x in &mut *rest {
                 first.unify_variables(x);
             }
         }
 
         let field = RationalPolynomialField::new(Z, first.numerator.get_vars());
 
         Ok(PythonMatrix {
-            matrix: Arc::new(
-                Matrix::from_linear(entries, nrows, ncols, field).map_err(|e| {
-                    exceptions::PyValueError::new_err(format!("Invalid matrix: {}", e))
-                })?,
-            ),
+            matrix: Matrix::from_linear(entries, nrows, ncols, field)
+                .map_err(|e| exceptions::PyValueError::new_err(format!("Invalid matrix: {}", e)))?,
         })
     }
 
     /// Create a new matrix from a 2-dimensional vector of scalars.
     #[classmethod]
     pub fn from_nested(
         cls: &PyType,
@@ -4767,100 +4881,91 @@
     pub fn is_diagonal(&self) -> bool {
         self.matrix.is_diagonal()
     }
 
     /// Return the transpose of the matrix.
     pub fn transpose(&self) -> PythonMatrix {
         PythonMatrix {
-            matrix: Arc::new(self.matrix.transpose()),
+            matrix: self.matrix.transpose(),
         }
     }
 
     /// Return the inverse of the matrix, if it exists.
     pub fn inv(&self) -> PyResult<PythonMatrix> {
         Ok(PythonMatrix {
-            matrix: Arc::new(
-                self.matrix
-                    .inv()
-                    .map_err(|e| exceptions::PyValueError::new_err(format!("{}", e)))?,
-            ),
+            matrix: self
+                .matrix
+                .inv()
+                .map_err(|e| exceptions::PyValueError::new_err(format!("{}", e)))?,
         })
     }
 
     /// Return the determinant of the matrix.
     pub fn det(&self) -> PyResult<PythonRationalPolynomial> {
         Ok(PythonRationalPolynomial {
-            poly: Arc::new(
-                self.matrix
-                    .det()
-                    .map_err(|e| exceptions::PyValueError::new_err(format!("{}", e)))?,
-            ),
+            poly: self
+                .matrix
+                .det()
+                .map_err(|e| exceptions::PyValueError::new_err(format!("{}", e)))?,
         })
     }
 
     /// Solve `A * x = b` for `x`, where `A` is the current matrix.
     pub fn solve(&self, b: PythonMatrix) -> PyResult<PythonMatrix> {
         let (new_self, new_rhs) = self.unify(&b);
         Ok(PythonMatrix {
-            matrix: Arc::new(
-                new_self
-                    .matrix
-                    .solve(&new_rhs.matrix)
-                    .map_err(|e| exceptions::PyValueError::new_err(format!("{}", e)))?,
-            ),
+            matrix: new_self
+                .matrix
+                .solve(&new_rhs.matrix)
+                .map_err(|e| exceptions::PyValueError::new_err(format!("{}", e)))?,
         })
     }
 
     /// Get the content of the matrix, i.e. the gcd of all entries.
     pub fn content(&self) -> PythonRationalPolynomial {
         PythonRationalPolynomial {
-            poly: Arc::new(self.matrix.content()),
+            poly: self.matrix.content(),
         }
     }
 
     /// Construct the same matrix, but with the content removed.
     pub fn primitive_part(&self) -> PythonMatrix {
         PythonMatrix {
-            matrix: Arc::new(self.matrix.primitive_part()),
+            matrix: self.matrix.primitive_part(),
         }
     }
 
     /// Apply a function `f` to every entry of the matrix.
     pub fn map(&self, f: PyObject) -> PyResult<PythonMatrix> {
         let data = self
             .matrix
             .data
             .iter()
             .map(|x| {
-                let expr = PythonRationalPolynomial {
-                    poly: Arc::new(x.clone()),
-                };
+                let expr = PythonRationalPolynomial { poly: x.clone() };
 
                 Python::with_gil(|py| {
                     Ok(f.call1(py, (expr,))
                         .map_err(|e| e)?
                         .extract::<ConvertibleToRationalPolynomial>(py)?
                         .to_rational_polynomial()?
                         .poly
-                        .as_ref()
                         .clone())
                 })
             })
             .collect::<PyResult<_>>()?;
 
         Ok(PythonMatrix {
-            matrix: Arc::new(
-                Matrix::from_linear(
-                    data,
-                    self.matrix.nrows,
-                    self.matrix.ncols,
-                    self.matrix.field.clone(),
-                )
-                .unwrap(),
-            ),
+            matrix: Matrix::from_linear(
+                data,
+                self.matrix.nrows,
+                self.matrix.ncols,
+                self.matrix.field.clone(),
+            )
+            .unwrap(),
         })
     }
 
     fn __getitem__(&self, mut idx: (isize, isize)) -> PyResult<PythonRationalPolynomial> {
         if idx.0 < 0 {
             idx.0 += self.matrix.nrows() as isize;
         }
@@ -4869,15 +4974,15 @@
         }
 
         if idx.0 as usize >= self.matrix.nrows() || idx.1 as usize >= self.matrix.ncols() {
             return Err(exceptions::PyIndexError::new_err("Index out of bounds"));
         }
 
         Ok(PythonRationalPolynomial {
-            poly: Arc::new(self.matrix[(idx.0 as u32, idx.1 as u32)].clone()),
+            poly: self.matrix[(idx.0 as u32, idx.1 as u32)].clone(),
         })
     }
 
     /// Convert the matrix into a LaTeX string.
     pub fn to_latex(&self) -> PyResult<String> {
         Ok(format!(
             "$${}$$",
@@ -4895,28 +5000,28 @@
             ))),
         }
     }
 
     /// Copy the matrix.
     pub fn __copy__(&self) -> Self {
         Self {
-            matrix: Arc::new((*self.matrix).clone()),
+            matrix: self.matrix.clone(),
         }
     }
 
     /// Convert the matrix into a human-readable string.
     pub fn __str__(&self) -> PyResult<String> {
         Ok(format!("{}", self.matrix))
     }
 
     /// Add this matrix to `rhs`, returning the result.
     pub fn __add__(&self, rhs: PythonMatrix) -> PythonMatrix {
         let (new_self, new_rhs) = self.unify(&rhs);
         PythonMatrix {
-            matrix: Arc::new(&*new_self.matrix + &*new_rhs.matrix),
+            matrix: &new_self.matrix + &new_rhs.matrix,
         }
     }
 
     ///  Subtract `rhs` from this matrix, returning the result.
     pub fn __sub__(&self, rhs: PythonMatrix) -> PythonMatrix {
         self.__add__(rhs.__neg__())
     }
@@ -4924,35 +5029,35 @@
     /// Add this matrix to `rhs`, returning the result.
     pub fn __mul__(&self, rhs: ScalarOrMatrix) -> PyResult<PythonMatrix> {
         match rhs {
             ScalarOrMatrix::Scalar(s) => {
                 let (new_self, new_rhs) = self.unify_scalar(&s.to_rational_polynomial()?);
 
                 Ok(Self {
-                    matrix: Arc::new(new_self.matrix.mul_scalar(&new_rhs.poly)),
+                    matrix: new_self.matrix.mul_scalar(&new_rhs.poly),
                 })
             }
             ScalarOrMatrix::Matrix(m) => {
                 let (new_self, new_rhs) = self.unify(&m);
                 Ok(PythonMatrix {
-                    matrix: Arc::new(&*new_self.matrix * &*new_rhs.matrix),
+                    matrix: &new_self.matrix * &new_rhs.matrix,
                 })
             }
         }
     }
 
     /// Add this matrix to `rhs`, returning the result.
     pub fn __rmul__(&self, rhs: ConvertibleToRationalPolynomial) -> PyResult<PythonMatrix> {
         self.__mul__(ScalarOrMatrix::Scalar(rhs))
     }
 
     /// Divide the matrix by the scalar, returning the result.
     pub fn __truediv__(&self, rhs: ConvertibleToRationalPolynomial) -> PyResult<PythonMatrix> {
         Ok(PythonMatrix {
-            matrix: Arc::new(self.matrix.div_scalar(&rhs.to_rational_polynomial()?.poly)),
+            matrix: self.matrix.div_scalar(&rhs.to_rational_polynomial()?.poly),
         })
     }
 
     /// Returns a warning that `**` should be used instead of `^` for taking a power.
     pub fn __xor__(&self, _rhs: PyObject) -> PyResult<PythonMatrix> {
         Err(exceptions::PyTypeError::new_err(
             "Cannot xor a matrix. Did you mean to write a power? Use ** instead, i.e. x**2",
@@ -4965,22 +5070,22 @@
             "Cannot xor a matrix. Did you mean to write a power? Use ** instead, i.e. x**2",
         ))
     }
 
     /// Negate the matrix, returning the result.
     pub fn __neg__(&self) -> PythonMatrix {
         PythonMatrix {
-            matrix: Arc::new(-self.matrix.as_ref().clone()),
+            matrix: -self.matrix.clone(),
         }
     }
 }
 
 /// A sample from the Symbolica integrator. It could consist of discrete layers,
 /// accessible with `d` (empty when there are not discrete layers), and the final continous layer `c` if it is present.
-#[pyclass(name = "Sample")]
+#[pyclass(name = "Sample", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonSample {
     #[pyo3(get)]
     /// The weights the integrator assigned to this sample point, given in descending order:
     /// first the discrete layer weights and then the continuous layer weight.
     weights: Vec<f64>,
     #[pyo3(get)]
@@ -5048,15 +5153,15 @@
 }
 
 /// A reproducible, fast, non-cryptographic random number generator suitable for parallel Monte Carlo simulations.
 /// A `seed` has to be set, which can be any `u64` number (small numbers work just as well as large numbers).
 ///
 /// Each thread or instance generating samples should use the same `seed` but a different `stream_id`,
 /// which is an instance counter starting at 0.
-#[pyclass(name = "RandomNumberGenerator")]
+#[pyclass(name = "RandomNumberGenerator", module = "symbolica")]
 struct PythonRandomNumberGenerator {
     state: MonteCarloRng,
 }
 
 #[pymethods]
 impl PythonRandomNumberGenerator {
     /// Create a new random number generator with a given `seed` and `stream_id`. For parallel runs,
@@ -5065,15 +5170,15 @@
     fn new(seed: u64, stream_id: usize) -> Self {
         Self {
             state: MonteCarloRng::new(seed, stream_id),
         }
     }
 }
 
-#[pyclass(name = "NumericalIntegrator")]
+#[pyclass(name = "NumericalIntegrator", module = "symbolica")]
 #[derive(Clone)]
 struct PythonNumericalIntegrator {
     grid: Grid<f64>,
 }
 
 #[pymethods]
 impl PythonNumericalIntegrator {
```

### Comparing `symbolica-0.4.0/src/atom/representation.rs` & `symbolica-0.5.0/src/atom/representation.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 use byteorder::{LittleEndian, WriteBytesExt};
 use bytes::{Buf, BufMut};
-use std::cmp::Ordering;
+use std::{
+    cmp::Ordering,
+    io::{Read, Write},
+};
 
-use crate::coefficient::{Coefficient, CoefficientView};
+use crate::{
+    coefficient::{Coefficient, CoefficientView},
+    state::{StateMap, Workspace},
+};
 
 use super::{
     coefficient::{PackedRationalNumberReader, PackedRationalNumberWriter},
-    AtomView, SliceType, Symbol,
+    Atom, AtomView, SliceType, Symbol,
 };
 
 const NUM_ID: u8 = 1;
 const VAR_ID: u8 = 2;
 const FUN_ID: u8 = 3;
 const MUL_ID: u8 = 4;
 const ADD_ID: u8 = 5;
@@ -19,19 +25,61 @@
 const NOT_NORMALIZED: u8 = 0b10000000;
 const VAR_WILDCARD_LEVEL_MASK: u8 = 0b00011000;
 const VAR_WILDCARD_LEVEL_1: u8 = 0b00001000;
 const VAR_WILDCARD_LEVEL_2: u8 = 0b00010000;
 const VAR_WILDCARD_LEVEL_3: u8 = 0b00011000;
 const FUN_SYMMETRIC_FLAG: u8 = 0b00100000;
 const FUN_LINEAR_FLAG: u8 = 0b01000000;
+const VAR_ANTISYMMETRIC_FLAG: u8 = 0b10000000;
 const FUN_ANTISYMMETRIC_FLAG: u64 = 1 << 32; // stored in the function id
 const MUL_HAS_COEFF_FLAG: u8 = 0b01000000;
 
 pub type RawAtom = Vec<u8>;
 
+impl Atom {
+    /// Read from a binary stream. The format is the byte-length first
+    /// followed by the data.
+    pub(crate) fn read<R: Read>(&mut self, mut source: R) -> Result<(), std::io::Error> {
+        let mut dest = std::mem::replace(self, Atom::Empty).into_raw();
+
+        // should also set whether rat poly coefficient needs to be converted
+        let mut flags_buf = [0; 1];
+        let mut size_buf = [0; 8];
+
+        source.read_exact(&mut flags_buf)?;
+        source.read_exact(&mut size_buf)?;
+
+        let n_size = u64::from_le_bytes(size_buf);
+
+        dest.extend(size_buf);
+        dest.resize(n_size as usize, 0);
+        source.read_exact(&mut dest)?;
+
+        unsafe {
+            match dest[0] & TYPE_MASK {
+                NUM_ID => *self = Atom::Num(Num::from_raw(dest)),
+                VAR_ID => *self = Atom::Var(Var::from_raw(dest)),
+                FUN_ID => *self = Atom::Fun(Fun::from_raw(dest)),
+                MUL_ID => *self = Atom::Mul(Mul::from_raw(dest)),
+                ADD_ID => *self = Atom::Add(Add::from_raw(dest)),
+                POW_ID => *self = Atom::Pow(Pow::from_raw(dest)),
+                _ => unreachable!("Unknown type {}", dest[0]),
+            }
+        }
+
+        Ok(())
+    }
+
+    pub fn import<R: Read>(source: R, state_map: &StateMap) -> Result<Atom, std::io::Error> {
+        let mut a = Atom::new();
+        a.read(source)?;
+        Ok(a.as_view().rename(state_map))
+    }
+}
+
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
 pub struct Num {
     data: RawAtom,
 }
 
 impl Num {
     #[inline(always)]
@@ -109,71 +157,71 @@
         AtomView::Num(self.to_num_view())
     }
 
     #[inline(always)]
     pub fn into_raw(self) -> RawAtom {
         self.data
     }
+
+    #[inline(always)]
+    pub(crate) unsafe fn from_raw(raw: RawAtom) -> Num {
+        Num { data: raw }
+    }
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
 pub struct Var {
     data: RawAtom,
 }
 
 impl Var {
     #[inline]
     pub fn new(symbol: Symbol) -> Var {
-        let mut buffer = Vec::new();
-
-        match symbol.wildcard_level {
-            0 => buffer.put_u8(VAR_ID),
-            1 => buffer.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_1),
-            2 => buffer.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_2),
-            _ => buffer.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_3),
-        }
-
-        (symbol.id as u64, 1).write_packed(&mut buffer);
-        Var { data: buffer }
+        Self::new_into(symbol, RawAtom::new())
     }
 
     #[inline]
-    pub fn new_into(symbol: Symbol, mut buffer: RawAtom) -> Var {
-        buffer.clear();
-
-        match symbol.wildcard_level {
-            0 => buffer.put_u8(VAR_ID),
-            1 => buffer.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_1),
-            2 => buffer.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_2),
-            _ => buffer.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_3),
-        }
-
-        (symbol.id as u64, 1).write_packed(&mut buffer);
-        Var { data: buffer }
+    pub fn new_into(symbol: Symbol, buffer: RawAtom) -> Var {
+        let mut f = Var { data: buffer };
+        f.set_from_symbol(symbol);
+        f
     }
 
     #[inline]
     pub fn from_view_into(a: &VarView<'_>, mut buffer: RawAtom) -> Var {
         buffer.clear();
         buffer.extend(a.data);
         Var { data: buffer }
     }
 
     #[inline]
-    pub fn set_from_symbol(&mut self, id: Symbol) {
+    pub fn set_from_symbol(&mut self, symbol: Symbol) {
         self.data.clear();
 
-        match id.wildcard_level {
-            0 => self.data.put_u8(VAR_ID),
-            1 => self.data.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_1),
-            2 => self.data.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_2),
-            _ => self.data.put_u8(VAR_ID | VAR_WILDCARD_LEVEL_3),
+        let mut flags = VAR_ID;
+        match symbol.wildcard_level {
+            0 => {}
+            1 => flags |= VAR_WILDCARD_LEVEL_1,
+            2 => flags |= VAR_WILDCARD_LEVEL_2,
+            _ => flags |= VAR_WILDCARD_LEVEL_3,
         }
 
-        (id.id as u64, 1).write_packed(&mut self.data);
+        if symbol.is_symmetric {
+            flags |= FUN_SYMMETRIC_FLAG;
+        }
+        if symbol.is_linear {
+            flags |= FUN_LINEAR_FLAG;
+        }
+        if symbol.is_antisymmetric {
+            flags |= VAR_ANTISYMMETRIC_FLAG;
+        }
+
+        self.data.put_u8(flags);
+
+        (symbol.id as u64, 1).write_packed(&mut self.data);
     }
 
     #[inline]
     pub fn to_var_view(&self) -> VarView {
         VarView { data: &self.data }
     }
 
@@ -193,14 +241,19 @@
         self.to_var_view().get_symbol()
     }
 
     #[inline(always)]
     pub fn into_raw(self) -> RawAtom {
         self.data
     }
+
+    #[inline(always)]
+    pub(crate) unsafe fn from_raw(raw: RawAtom) -> Var {
+        Var { data: raw }
+    }
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
 pub struct Fun {
     data: RawAtom,
 }
 
@@ -338,14 +391,19 @@
         self.to_fun_view().get_nargs()
     }
 
     #[inline(always)]
     pub fn into_raw(self) -> RawAtom {
         self.data
     }
+
+    #[inline(always)]
+    pub(crate) unsafe fn from_raw(raw: RawAtom) -> Fun {
+        Fun { data: raw }
+    }
 }
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
 pub struct Pow {
     data: RawAtom,
 }
 
@@ -397,14 +455,19 @@
         AtomView::Pow(self.to_pow_view())
     }
 
     #[inline(always)]
     pub fn into_raw(self) -> RawAtom {
         self.data
     }
+
+    #[inline(always)]
+    pub(crate) unsafe fn from_raw(raw: RawAtom) -> Pow {
+        Pow { data: raw }
+    }
 }
 
 #[derive(Clone, PartialEq, Eq, Hash)]
 pub struct Mul {
     data: RawAtom,
 }
 
@@ -573,14 +636,19 @@
         self.to_mul_view().get_nargs()
     }
 
     #[inline(always)]
     pub fn into_raw(self) -> RawAtom {
         self.data
     }
+
+    #[inline(always)]
+    pub(crate) unsafe fn from_raw(raw: RawAtom) -> Mul {
+        Mul { data: raw }
+    }
 }
 
 #[derive(Clone, PartialEq, Eq, Hash)]
 pub struct Add {
     data: RawAtom,
 }
 
@@ -596,19 +664,15 @@
         Self::new_into(RawAtom::new())
     }
 
     #[inline]
     pub(crate) fn new_into(mut buffer: RawAtom) -> Add {
         buffer.clear();
         buffer.put_u8(ADD_ID | NOT_NORMALIZED);
-        buffer.put_u32_le(0_u32);
-        (0u64, 1).write_packed(&mut buffer);
-        let len = buffer.len() as u32 - 1 - 4;
-        (&mut buffer[1..]).put_u32_le(len);
-
+        (0u64, 0).write_packed(&mut buffer);
         Add { data: buffer }
     }
 
     #[inline]
     pub fn from_view_into(a: &AddView<'_>, mut buffer: RawAtom) -> Add {
         buffer.clear();
         buffer.extend(a.data);
@@ -623,63 +687,52 @@
             self.data[0] &= !NOT_NORMALIZED;
         }
     }
 
     pub(crate) fn extend(&mut self, other: AtomView<'_>) {
         self.data[0] |= NOT_NORMALIZED;
 
-        // may increase size of the num of args
-        let mut c = &self.data[1 + 4..];
-
-        let buf_pos = 1 + 4;
+        let mut c = &self.data[1..];
 
         let mut n_args;
         (n_args, _, c) = c.get_frac_u64();
 
-        let old_size = unsafe { c.as_ptr().offset_from(self.data.as_ptr()) } as usize - 1 - 4;
+        let old_header_size = unsafe { c.as_ptr().offset_from(self.data.as_ptr()) } as usize;
 
         let new_slice = match other {
             AtomView::Add(m) => m.to_slice(),
             _ => ListSlice::from_one(other),
         };
 
+        for child in new_slice.iter() {
+            self.data.extend_from_slice(child.get_data());
+        }
+
         n_args += new_slice.len() as u64;
 
-        let new_size = (n_args, 1).get_packed_size() as usize;
+        let new_len = self.data.len() - old_header_size;
+        let new_header_size = (n_args, new_len as u64).get_packed_size() as usize + 1;
 
-        match new_size.cmp(&old_size) {
+        match new_header_size.cmp(&old_header_size) {
             Ordering::Equal => {}
             Ordering::Less => {
-                self.data.copy_within(1 + 4 + old_size.., 1 + 4 + new_size);
-                self.data.resize(self.data.len() - old_size + new_size, 0);
+                self.data.copy_within(old_header_size.., new_header_size);
+                self.data
+                    .resize(self.data.len() - old_header_size + new_header_size, 0);
             }
             Ordering::Greater => {
                 let old_len = self.data.len();
-                self.data.resize(old_len + new_size - old_size, 0);
                 self.data
-                    .copy_within(1 + 4 + old_size..old_len, 1 + 4 + new_size);
+                    .resize(old_len + new_header_size - old_header_size, 0);
+                self.data
+                    .copy_within(old_header_size..old_len, new_header_size);
             }
         }
 
-        // size should be ok now
-        (n_args, 1).write_packed_fixed(&mut self.data[1 + 4..1 + 4 + new_size]);
-
-        for child in new_slice.iter() {
-            self.data.extend_from_slice(child.get_data());
-        }
-
-        let new_buf_pos = self.data.len();
-
-        let mut cursor = &mut self.data[1..];
-
-        assert!(new_buf_pos - buf_pos < u32::MAX as usize, "Term too large");
-
-        cursor
-            .write_u32::<LittleEndian>((new_buf_pos - buf_pos) as u32)
-            .unwrap();
+        (n_args, new_len as u64).write_packed_fixed(&mut self.data[1..new_header_size]);
     }
 
     #[inline(always)]
     pub fn to_add_view(&self) -> AddView {
         AddView { data: &self.data }
     }
 
@@ -699,14 +752,19 @@
         self.to_add_view().get_nargs()
     }
 
     #[inline(always)]
     pub fn into_raw(self) -> RawAtom {
         self.data
     }
+
+    #[inline(always)]
+    pub(crate) unsafe fn from_raw(raw: RawAtom) -> Add {
+        Add { data: raw }
+    }
 }
 
 impl<'a> VarView<'a> {
     #[inline]
     pub fn to_owned(&self) -> Var {
         Var::from_view_into(self, Vec::new())
     }
@@ -721,17 +779,20 @@
         buffer.clear();
         buffer.extend(self.data);
         Var { data: buffer }
     }
 
     #[inline(always)]
     pub fn get_symbol(&self) -> Symbol {
-        Symbol::init_var(
+        Symbol::init_fn(
             self.data[1..].get_frac_i64().0 as u32,
             self.get_wildcard_level(),
+            self.data[0] & FUN_SYMMETRIC_FLAG != 0,
+            self.data[0] & VAR_ANTISYMMETRIC_FLAG != 0,
+            self.data[0] & FUN_LINEAR_FLAG != 0,
         )
     }
 
     #[inline(always)]
     pub fn get_wildcard_level(&self) -> u8 {
         match self.data[0] & VAR_WILDCARD_LEVEL_MASK {
             0 => 0,
@@ -1126,25 +1187,24 @@
     #[inline(always)]
     pub(crate) fn is_normalized(&self) -> bool {
         (self.data[0] & NOT_NORMALIZED) == 0
     }
 
     #[inline(always)]
     pub fn get_nargs(&self) -> usize {
-        self.data[1 + 4..].get_frac_i64().0 as usize
+        self.data[1..].get_frac_u64().0 as usize
     }
 
     #[inline]
     pub fn iter(&self) -> ListIterator<'a> {
         let mut c = self.data;
         c.get_u8();
-        c.get_u32_le(); // size
 
         let n_args;
-        (n_args, _, c) = c.get_frac_i64();
+        (n_args, _, c) = c.get_frac_u64();
 
         ListIterator {
             data: c,
             length: n_args as u32,
         }
     }
 
@@ -1152,18 +1212,17 @@
     pub fn as_view(&self) -> AtomView<'a> {
         AtomView::Add(*self)
     }
 
     pub fn to_slice(&self) -> ListSlice<'a> {
         let mut c = self.data;
         c.get_u8();
-        c.get_u32_le(); // size
 
         let n_args;
-        (n_args, _, c) = c.get_frac_i64();
+        (n_args, _, c) = c.get_frac_u64();
 
         ListSlice {
             data: c,
             length: n_args as usize,
             slice_type: SliceType::Add,
         }
     }
@@ -1192,14 +1251,109 @@
             AtomView::Var(v) => v.data,
             AtomView::Fun(f) => f.data,
             AtomView::Pow(p) => p.data,
             AtomView::Mul(t) => t.data,
             AtomView::Add(e) => e.data,
         }
     }
+
+    /// Write the expression to a binary stream. The format is the byte-length first
+    /// followed by the data. To import the expression in new session, also export the [`State`].
+    #[inline(always)]
+    pub fn write<W: Write>(&self, mut dest: W) -> Result<(), std::io::Error> {
+        let d = self.get_data();
+        dest.write_u8(0)?;
+        dest.write_u64::<LittleEndian>(d.len() as u64)?;
+        dest.write_all(d)
+    }
+
+    pub(crate) fn rename(&self, state_map: &StateMap) -> Atom {
+        Workspace::get_local().with(|ws| {
+            let mut a = ws.new_atom();
+            self.rename_no_norm(state_map, ws, &mut a);
+            let mut r = Atom::new();
+            a.as_view().normalize(ws, &mut r);
+            r
+        })
+    }
+
+    fn rename_no_norm(&self, state_map: &StateMap, ws: &Workspace, out: &mut Atom) {
+        match self {
+            AtomView::Num(n) => match n.get_coeff_view() {
+                CoefficientView::FiniteField(e, i) => {
+                    if let Some(s) = state_map.finite_fields.get(&i) {
+                        out.to_num(Coefficient::FiniteField(e, *s));
+                    } else {
+                        out.set_from_view(self);
+                    }
+                }
+                CoefficientView::RationalPolynomial(r) => {
+                    let (old_id, _, _) = r.0.get_frac_u64();
+
+                    if let Some(nv) = state_map.variables_lists.get(&old_id) {
+                        let mut rr = r.deserialize();
+                        rr.numerator.variables = nv.clone();
+                        rr.denominator.variables = nv.clone();
+                        out.to_num(Coefficient::RationalPolynomial(rr));
+                    } else {
+                        out.set_from_view(self);
+                    }
+                }
+                _ => out.set_from_view(self),
+            },
+            AtomView::Var(v) => {
+                if let Some(s) = state_map.symbols.get(&v.get_symbol().get_id()) {
+                    out.to_var(*s);
+                } else {
+                    out.set_from_view(self);
+                }
+            }
+            AtomView::Fun(f) => {
+                if let Some(s) = state_map.symbols.get(&f.get_symbol().get_id()) {
+                    let nf = out.to_fun(*s);
+
+                    let mut na = ws.new_atom();
+                    for a in f.iter() {
+                        a.rename_no_norm(state_map, ws, &mut na);
+                        nf.add_arg(na.as_view());
+                    }
+                } else {
+                    out.set_from_view(self);
+                }
+            }
+            AtomView::Pow(p) => {
+                let (b, e) = p.get_base_exp();
+
+                let mut nb = ws.new_atom();
+                b.rename_no_norm(state_map, ws, &mut nb);
+                let mut ne = ws.new_atom();
+                e.rename_no_norm(state_map, ws, &mut ne);
+
+                out.to_pow(nb.as_view(), ne.as_view());
+            }
+            AtomView::Mul(m) => {
+                let nm = out.to_mul();
+
+                let mut na = ws.new_atom();
+                for a in m.iter() {
+                    a.rename_no_norm(state_map, ws, &mut na);
+                    nm.extend(na.as_view());
+                }
+            }
+            AtomView::Add(add) => {
+                let nm = out.to_add();
+
+                let mut na = ws.new_atom();
+                for a in add.iter() {
+                    a.rename_no_norm(state_map, ws, &mut na);
+                    nm.extend(na.as_view());
+                }
+            }
+        }
+    }
 }
 
 #[derive(Debug, Copy, Clone)]
 pub struct ListIterator<'a> {
     data: &'a [u8],
     length: u32,
 }
@@ -1224,18 +1378,23 @@
         // can be used instead of storing the byte length of an atom
         let mut skip_count = 1;
         loop {
             match cur_id {
                 NUM_ID | VAR_ID => {
                     self.data = self.data.skip_rational();
                 }
-                FUN_ID | MUL_ID | ADD_ID => {
+                FUN_ID | MUL_ID => {
                     let n_size = self.data.get_u32_le();
                     self.data.advance(n_size as usize);
                 }
+                ADD_ID => {
+                    let (_, size, np) = self.data.get_frac_u64();
+                    self.data = np;
+                    self.data.advance(size as usize);
+                }
                 POW_ID => {
                     skip_count += 2;
                 }
                 _ => unreachable!("Bad id"),
             }
 
             skip_count -= 1;
@@ -1278,18 +1437,23 @@
         while skip_count > 0 {
             skip_count -= 1;
 
             match pos.get_u8() & TYPE_MASK {
                 NUM_ID | VAR_ID => {
                     pos = pos.skip_rational();
                 }
-                FUN_ID | MUL_ID | ADD_ID => {
+                FUN_ID | MUL_ID => {
                     let n_size = pos.get_u32_le();
                     pos.advance(n_size as usize);
                 }
+                ADD_ID => {
+                    let (_, size, np) = pos.get_frac_u64();
+                    pos = np;
+                    pos.advance(size as usize);
+                }
                 POW_ID => {
                     skip_count += 2;
                 }
                 _ => unreachable!("Bad id"),
             }
         }
         pos
```

### Comparing `symbolica-0.4.0/src/atom.rs` & `symbolica-0.5.0/src/atom.rs`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,24 @@
             f.write_str("_")?;
         }
         Ok(())
     }
 }
 
 #[derive(Debug, Clone, Copy, PartialEq, Eq)]
+pub enum AtomType {
+    Num,
+    Var,
+    Add,
+    Mul,
+    Pow,
+    Fun,
+}
+
+#[derive(Debug, Clone, Copy, PartialEq, Eq)]
 pub enum SliceType {
     Add,
     Mul,
     Arg,
     One,
     Pow,
     Empty,
@@ -226,14 +236,32 @@
         a
     }
 
     pub fn clone_into(&self, target: &mut Atom) {
         target.set_from_view(self);
     }
 
+    #[inline]
+    pub fn is_zero(&self) -> bool {
+        if let AtomView::Num(n) = self {
+            n.is_zero()
+        } else {
+            false
+        }
+    }
+
+    #[inline]
+    pub fn is_one(&self) -> bool {
+        if let AtomView::Num(n) = self {
+            n.is_one()
+        } else {
+            false
+        }
+    }
+
     /// Add two atoms and return the buffer that contains the unnormalized result.
     fn add_no_norm(&self, workspace: &Workspace, rhs: AtomView<'_>) -> RecycledAtom {
         let mut e = workspace.new_atom();
         let a = e.to_add();
 
         // TODO: check if self or rhs is add
         a.extend(*self);
@@ -352,14 +380,15 @@
 pub enum Atom {
     Num(Num),
     Var(Var),
     Fun(Fun),
     Pow(Pow),
     Mul(Mul),
     Add(Add),
+    #[doc(hidden)]
     Empty, // for internal use
 }
 
 impl Default for Atom {
     /// Create an atom that represents the number 0.
     #[inline]
     fn default() -> Self {
@@ -405,14 +434,26 @@
 
 impl From<Fun> for Atom {
     fn from(n: Fun) -> Atom {
         Atom::Fun(n)
     }
 }
 
+impl PartialOrd for Atom {
+    fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
+        Some(self.cmp(other))
+    }
+}
+
+impl Ord for Atom {
+    fn cmp(&self, other: &Self) -> Ordering {
+        self.as_view().cmp(&other.as_view())
+    }
+}
+
 impl Atom {
     /// Create an atom that represents the number 0.
     pub fn new() -> Atom {
         Atom::default()
     }
 
     /// Parse and atom from a string.
@@ -427,14 +468,24 @@
 
     #[inline]
     pub fn new_num<T: Into<Coefficient>>(num: T) -> Atom {
         Num::new(num.into()).into()
     }
 
     #[inline]
+    pub fn is_zero(&self) -> bool {
+        self.as_view().is_zero()
+    }
+
+    #[inline]
+    pub fn is_one(&self) -> bool {
+        self.as_view().is_one()
+    }
+
+    #[inline]
     pub fn to_num(&mut self, coeff: Coefficient) -> &mut Num {
         let buffer = std::mem::replace(self, Atom::Empty).into_raw();
         *self = Atom::Num(Num::new_into(coeff, buffer));
         if let Atom::Num(n) = self {
             n
         } else {
             unreachable!()
@@ -658,14 +709,44 @@
             base.as_atom_view()
                 .pow_no_norm(ws, self.as_view())
                 .as_view()
                 .normalize(ws, &mut t);
             t.into_inner()
         })
     }
+
+    /// Add the atoms in `args`.
+    pub fn add_many<'a, T: AsAtomView<'a> + Copy>(args: &[T]) -> Atom {
+        let mut out = Atom::new();
+        Workspace::get_local().with(|ws| {
+            let mut t = ws.new_atom();
+            let add = t.to_add();
+            for a in args {
+                add.extend(a.as_atom_view());
+            }
+
+            t.as_view().normalize(ws, &mut out);
+        });
+        out
+    }
+
+    /// Multiply the atoms in `args`.
+    pub fn mul_many<'a, T: AsAtomView<'a> + Copy>(args: &[T]) -> Atom {
+        let mut out = Atom::new();
+        Workspace::get_local().with(|ws| {
+            let mut t = ws.new_atom();
+            let add = t.to_mul();
+            for a in args {
+                add.extend(a.as_atom_view());
+            }
+
+            t.as_view().normalize(ws, &mut out);
+        });
+        out
+    }
 }
 
 impl std::ops::Add<Atom> for &Atom {
     type Output = Atom;
 
     fn add(self, mut rhs: Atom) -> Atom {
         Workspace::get_local().with(|ws| {
@@ -1046,27 +1127,27 @@
     };
 
     #[test]
     fn debug() {
         let x = Atom::parse("v1+f1(v2)").unwrap();
         assert_eq!(
             format!("{:?}", x),
-            "AddView { data: [5, 15, 0, 0, 0, 1, 2, 2, 1, 12, 3, 5, 0, 0, 0, 1, 42, 2, 1, 13] }"
+            "AddView { data: [5, 17, 2, 13, 2, 1, 12, 3, 5, 0, 0, 0, 1, 42, 2, 1, 13] }"
         );
         assert_eq!(
             x.get_all_symbols(true),
             [
                 State::get_symbol("v1"),
                 State::get_symbol("v2"),
                 State::get_symbol("f1")
             ]
             .into_iter()
             .collect(),
         );
-        assert_eq!(x.as_view().get_byte_size(), 20);
+        assert_eq!(x.as_view().get_byte_size(), 17);
     }
 
     #[test]
     fn composition() {
         let v1 = Atom::parse("v1").unwrap();
         let v2 = Atom::parse("v2").unwrap();
         let f1_id = State::get_symbol("f1");
```

### Comparing `symbolica-0.4.0/src/coefficient.rs` & `symbolica-0.5.0/src/coefficient.rs`

 * *Files 2% similar despite different names*

```diff
@@ -250,21 +250,24 @@
             num.neg_assign();
         }
 
         MultiPrecisionRational::from((num, den))
     }
 }
 
+#[derive(Debug, Copy, Clone, PartialEq, Eq)]
+pub struct SerializedRationalPolynomial<'a>(pub &'a [u8]);
+
 /// A view of a coefficient that keeps GMP rationals serialized.
 #[derive(Debug, Copy, Clone, PartialEq, Eq)]
 pub enum CoefficientView<'a> {
     Natural(i64, i64),
     Large(SerializedRational<'a>),
     FiniteField(FiniteFieldElement<u64>, FiniteFieldIndex),
-    RationalPolynomial(&'a RationalPolynomial<IntegerRing, u16>),
+    RationalPolynomial(SerializedRationalPolynomial<'a>),
 }
 
 impl ConvertToRing for RationalField {
     #[inline]
     fn element_from_integer(&self, number: Integer) -> Self::Element {
         number.into()
     }
@@ -405,15 +408,17 @@
     }
 
     pub fn to_owned(&self) -> Coefficient {
         match self {
             CoefficientView::Natural(num, den) => Coefficient::Rational((*num, *den).into()),
             CoefficientView::Large(r) => Coefficient::Rational(r.to_rat().into()),
             CoefficientView::FiniteField(num, field) => Coefficient::FiniteField(*num, *field),
-            CoefficientView::RationalPolynomial(p) => Coefficient::RationalPolynomial((*p).clone()),
+            CoefficientView::RationalPolynomial(p) => {
+                Coefficient::RationalPolynomial(p.deserialize())
+            }
         }
     }
 
     pub fn pow(&self, other: &CoefficientView<'_>) -> (Coefficient, Coefficient) {
         // TODO: normalize 4^1/3 to 2^(2/3)?
         match (self, other) {
             (&CoefficientView::Natural(mut n1, mut d1), &CoefficientView::Natural(mut n2, d2)) => {
@@ -444,22 +449,22 @@
             }
             (&CoefficientView::RationalPolynomial(r), &CoefficientView::Natural(n2, d2)) => {
                 if n2.unsigned_abs() > u32::MAX as u64 {
                     panic!("Power is too large: {}", n2);
                 }
 
                 if n2 < 0 {
-                    let r = r.clone().inv();
+                    let r = r.deserialize().inv();
                     (
                         Coefficient::RationalPolynomial(r.pow(n2.unsigned_abs())),
                         (1, d2).into(),
                     )
                 } else {
                     (
-                        Coefficient::RationalPolynomial(r.pow(n2 as u64)),
+                        Coefficient::RationalPolynomial(r.deserialize().pow(n2 as u64)),
                         (1, d2).into(),
                     )
                 }
             }
             (&CoefficientView::Large(r), &CoefficientView::Natural(n2, d2)) => {
                 if n2.unsigned_abs() > u32::MAX as u64 {
                     panic!("Power is too large: {}", n2);
@@ -568,39 +573,40 @@
                 panic!("Cannot add finite field to non-finite number. Convert other number first?");
             }
             (_, CoefficientView::FiniteField(_, _)) => {
                 panic!("Cannot add finite field to non-finite number. Convert other number first?");
             }
             (CoefficientView::Natural(n, d), CoefficientView::RationalPolynomial(p))
             | (CoefficientView::RationalPolynomial(p), CoefficientView::Natural(n, d)) => {
-                let r = (*p).clone();
+                let r = p.deserialize();
                 let r2 = RationalPolynomial {
-                    numerator: p.numerator.constant(Integer::Natural(n)),
-                    denominator: p.denominator.constant(Integer::Natural(d)),
+                    numerator: r.numerator.constant(Integer::Natural(n)),
+                    denominator: r.denominator.constant(Integer::Natural(d)),
                 };
                 Coefficient::RationalPolynomial(&r + &r2)
             }
             (CoefficientView::Large(l), CoefficientView::RationalPolynomial(p))
             | (CoefficientView::RationalPolynomial(p), CoefficientView::Large(l)) => {
-                let r = (*p).clone();
+                let r = p.deserialize();
                 let (n, d) = l.to_rat().into_numer_denom();
                 let r2 = RationalPolynomial {
-                    numerator: p.numerator.constant(Integer::from_large(n)),
-                    denominator: p.denominator.constant(Integer::from_large(d)),
+                    numerator: r.numerator.constant(Integer::from_large(n)),
+                    denominator: r.denominator.constant(Integer::from_large(d)),
                 };
                 Coefficient::RationalPolynomial(&r + &r2)
             }
             (CoefficientView::RationalPolynomial(p1), CoefficientView::RationalPolynomial(p2)) => {
+                let mut p1 = p1.deserialize();
+                let mut p2 = p2.deserialize();
+
                 let r = if p1.get_variables() != p2.get_variables() {
-                    let mut p1 = (*p1).clone();
-                    let mut p2 = (*p2).clone();
                     p1.unify_variables(&mut p2);
                     &p1 + &p2
                 } else {
-                    p1 + p2
+                    &p1 + &p2
                 };
 
                 if r.is_constant() {
                     (r.numerator.lcoeff(), r.denominator.lcoeff()).into()
                 } else {
                     Coefficient::RationalPolynomial(r)
                 }
@@ -639,43 +645,43 @@
                 panic!("Cannot multiply finite field to non-finite number. Convert other number first?");
             }
             (_, CoefficientView::FiniteField(_, _)) => {
                 panic!("Cannot multiply finite field to non-finite number. Convert other number first?");
             }
             (CoefficientView::Natural(n, d), CoefficientView::RationalPolynomial(p))
             | (CoefficientView::RationalPolynomial(p), CoefficientView::Natural(n, d)) => {
-                let mut r = (*p).clone();
+                let mut r = p.deserialize();
                 let (n, d) = (Integer::Natural(n), Integer::Natural(d));
 
                 let gcd1 = Z.gcd(&n, &r.denominator.content());
                 let gcd2 = Z.gcd(&d, &r.numerator.content());
                 r.numerator = r.numerator.div_coeff(&gcd2).mul_coeff(n.div(&gcd1));
                 r.denominator = r.denominator.div_coeff(&gcd1).mul_coeff(d.div(&gcd2));
                 Coefficient::RationalPolynomial(r)
             }
             (CoefficientView::Large(l), CoefficientView::RationalPolynomial(p))
             | (CoefficientView::RationalPolynomial(p), CoefficientView::Large(l)) => {
-                let mut r = (*p).clone();
+                let mut r = p.deserialize();
                 let (n, d) = l.to_rat().into_numer_denom();
                 let (n, d) = (Integer::from_large(n), Integer::from_large(d));
 
                 let gcd1 = Z.gcd(&n, &r.denominator.content());
                 let gcd2 = Z.gcd(&d, &r.numerator.content());
                 r.numerator = r.numerator.div_coeff(&gcd2).mul_coeff(n.div(&gcd1));
                 r.denominator = r.denominator.div_coeff(&gcd1).mul_coeff(d.div(&gcd2));
                 Coefficient::RationalPolynomial(r)
             }
             (CoefficientView::RationalPolynomial(p1), CoefficientView::RationalPolynomial(p2)) => {
+                let mut p1 = p1.deserialize();
+                let mut p2 = p2.deserialize();
                 let r = if p1.get_variables() != p2.get_variables() {
-                    let mut p1 = (*p1).clone();
-                    let mut p2 = (*p2).clone();
                     p1.unify_variables(&mut p2);
                     &p1 * &p2
                 } else {
-                    p1 * p2
+                    &p1 * &p2
                 };
 
                 if r.is_constant() {
                     (r.numerator.lcoeff(), r.denominator.lcoeff()).into()
                 } else {
                     Coefficient::RationalPolynomial(r)
                 }
@@ -694,20 +700,21 @@
             }
             CoefficientView::Large(r1) => (r1.to_rat() + other).into(),
             CoefficientView::FiniteField(n1, i1) => {
                 let f = State::get_finite_field(i1);
                 Coefficient::FiniteField(f.add(&n1, &f.element_from_coefficient(other.into())), i1)
             }
             CoefficientView::RationalPolynomial(p) => {
+                let p = p.deserialize();
                 let a = RationalPolynomial {
                     numerator: p.numerator.constant(Integer::Natural(other)),
                     denominator: p.denominator.constant(Integer::Natural(1)),
                 };
 
-                Coefficient::RationalPolynomial(p + &a)
+                Coefficient::RationalPolynomial(&p + &a)
             }
         }
     }
 }
 
 impl Atom {
     pub fn set_coefficient_ring(&self, vars: &Arc<Vec<Variable>>) -> Atom {
@@ -729,14 +736,15 @@
         vars: &Arc<Vec<Variable>>,
         workspace: &Workspace,
         out: &mut Atom,
     ) -> bool {
         match self {
             AtomView::Num(n) => {
                 if let CoefficientView::RationalPolynomial(r) = n.get_coeff_view() {
+                    let r = r.deserialize();
                     let old_var_map = r.get_variables();
                     if old_var_map != vars {
                         if old_var_map.iter().all(|x| vars.contains(x)) {
                             // upgrade the polynomial if no variables got removed
                             let mut r = r.clone();
                             let order: SmallVec<[Option<usize>; INLINED_EXPONENTS]> = vars
                                 .iter()
@@ -891,14 +899,34 @@
 #[cfg(test)]
 mod test {
     use std::sync::Arc;
 
     use crate::{atom::Atom, domains::rational::Rational, state::State};
 
     #[test]
+    fn coeff_conversion() {
+        let expr = Atom::parse("v1*coeff(v2+v3/v4)+v1*coeff(v2)").unwrap();
+        let res = Atom::parse("coeff((v3+2*v2*v4)/v4)*v1").unwrap();
+        assert_eq!(expr - &res, Atom::new());
+    }
+
+    #[test]
+    fn coeff_conversion_large() {
+        let expr = Atom::parse(
+            "coeff(-8123781237821378123128937128937211238971238*v2-1289378192371289372891378127893)",
+        )
+        .unwrap();
+        let res = Atom::parse(
+            "1289378192371289372891378127893+8123781237821378123128937128937211238971238*coeff(v2)",
+        )
+        .unwrap();
+        assert_eq!(expr + &res, Atom::new());
+    }
+
+    #[test]
     fn coefficient_ring() {
         let expr = Atom::parse("v1*v3+v1*(v2+2)^-1*(v2+v3+1)").unwrap();
 
         let v2 = State::get_symbol("v2");
         let expr_yz =
             expr.set_coefficient_ring(&Arc::new(vec![v2.into(), State::get_symbol("v3").into()]));
```

### Comparing `symbolica-0.4.0/src/collect.rs` & `symbolica-0.5.0/src/collect.rs`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         out: &mut Atom,
     ) {
         self.as_view().collect_into(x, key_map, coeff_map, out)
     }
 
     /// Collect terms involving the same power of `x`, where `x` is a variable or function name.
     /// Return the list of key-coefficient pairs and the remainder that matched no key.
-    pub fn coefficient_list(&self, x: Symbol) -> (Vec<(AtomView<'_>, Atom)>, Atom) {
+    pub fn coefficient_list(&self, x: Symbol) -> (Vec<(Atom, Atom)>, Atom) {
         Workspace::get_local().with(|ws| self.as_view().coefficient_list_with_ws(x, ws))
     }
 
     /// Collect terms involving the literal occurrence of `x`.
     pub fn coefficient<'a, T: AsAtomView<'a>>(&self, x: T) -> Atom {
         Workspace::get_local().with(|ws| self.as_view().coefficient_with_ws(x.as_atom_view(), ws))
     }
@@ -152,15 +152,15 @@
                 mul.extend(coeff.as_view());
             }
 
             add.extend(mul_h.as_view());
         }
 
         for (key, coeff) in h {
-            map_key_coeff(key, coeff, workspace, &key_map, &coeff_map, add);
+            map_key_coeff(key.as_view(), coeff, workspace, &key_map, &coeff_map, add);
         }
 
         if key_map.is_some() {
             let key = workspace.new_num(1);
             map_key_coeff(key.as_view(), rest, workspace, &key_map, &coeff_map, add);
         } else if let Some(coeff_map) = coeff_map {
             let mut handle = workspace.new_atom();
@@ -171,52 +171,64 @@
         }
 
         add_h.as_view().normalize(workspace, out);
     }
 
     /// Collect terms involving the same power of `x`, where `x` is a variable or function name.
     /// Return the list of key-coefficient pairs and the remainder that matched no key.
-    pub fn coefficient_list(&self, x: Symbol) -> (Vec<(AtomView<'a>, Atom)>, Atom) {
+    pub fn coefficient_list(&self, x: Symbol) -> (Vec<(Atom, Atom)>, Atom) {
         Workspace::get_local().with(|ws| self.coefficient_list_with_ws(x, ws))
     }
 
     /// Collect terms involving the same power of `x`, where `x` is a variable or function name.
     /// Return the list of key-coefficient pairs and the remainder that matched no key.
     pub fn coefficient_list_with_ws(
         &self,
         x: Symbol,
         workspace: &Workspace,
-    ) -> (Vec<(AtomView<'a>, Atom)>, Atom) {
+    ) -> (Vec<(Atom, Atom)>, Atom) {
         let mut h = HashMap::default();
         let mut rest = workspace.new_atom();
         let mut rest_add = rest.to_add();
 
-        match self {
+        let mut expanded = workspace.new_atom();
+        self.expand_with_ws_into(workspace, Some(x), &mut expanded);
+
+        match expanded.as_view() {
             AtomView::Add(a) => {
                 for arg in a.iter() {
                     arg.collect_factor_list(x, workspace, &mut h, &mut rest_add)
                 }
             }
-            _ => self.collect_factor_list(x, workspace, &mut h, &mut rest_add),
+            _ => expanded
+                .as_view()
+                .collect_factor_list(x, workspace, &mut h, &mut rest_add),
         }
 
         let mut rest_norm = Atom::new();
         rest.as_view().normalize(workspace, &mut rest_norm);
 
         let mut r: Vec<_> = h
             .into_iter()
             .map(|(k, v)| {
-                (k, {
-                    let mut a = Atom::new();
-                    v.as_view().normalize(workspace, &mut a);
-                    a
-                })
+                (
+                    {
+                        let mut a = Atom::new();
+                        a.set_from_view(&k);
+                        a
+                    },
+                    {
+                        let mut a = Atom::new();
+                        v.as_view().normalize(workspace, &mut a);
+                        a
+                    },
+                )
             })
             .collect();
-        r.sort_unstable_by_key(|(a, _)| *a);
+        r.sort_unstable_by(|(a, _), (b, _)| a.as_view().cmp(&b.as_view()));
 
         (r, rest_norm)
     }
 
     /// Check if a factor contains `x` at the ground level.
     #[inline]
     fn has_key(&self, x: Symbol) -> bool {
@@ -338,14 +350,34 @@
                         } else {
                             mul.extend(a);
                         }
                     }
 
                     coeff.extend(collected.as_view());
                 }
+
+                if let AtomView::Mul(y) = x {
+                    // check if all factors occur
+                    for xx in y.iter() {
+                        if !m.iter().any(|a| a == xx) {
+                            return;
+                        }
+                    }
+
+                    let mut collected = workspace.new_atom();
+                    let mul = collected.to_mul();
+
+                    for xx in m.iter() {
+                        if !y.iter().any(|a| a == xx) {
+                            mul.extend(xx);
+                        }
+                    }
+
+                    coeff.extend(collected.as_view());
+                }
             }
             _ => {
                 if *self == x {
                     // add the coefficient 1
                     let collected = workspace.new_num(1);
                     coeff.extend(collected.as_view());
                 }
@@ -420,15 +452,15 @@
             (Atom::parse("v1^2").unwrap(), Atom::parse("1").unwrap()),
             (Atom::parse("v1^3").unwrap(), Atom::parse("1").unwrap()),
         ];
         let res_rest = Atom::parse("v2^2+f1(5,v1)+2").unwrap();
 
         let res_ref = res
             .iter()
-            .map(|(a, b)| (a.as_view(), b.clone()))
+            .map(|(a, b)| (a.clone(), b.clone()))
             .collect::<Vec<_>>();
 
         assert_eq!(r, res_ref);
         assert_eq!(rest, res_rest);
     }
 
     #[test]
@@ -439,14 +471,25 @@
         let out = input.collect(x, None, None);
 
         let ref_out = Atom::parse("v1^2+v1^3+v2^2+f1(5,v1)+v1*(5*v2+v3+1)+2").unwrap();
         assert_eq!(out, ref_out)
     }
 
     #[test]
+    fn collect_nested() {
+        let input = Atom::parse("(1+v1)^2*v1+(1+v2)^100").unwrap();
+        let x = State::get_symbol("v1");
+
+        let out = input.collect(x, None, None);
+
+        let ref_out = Atom::parse("v1+2*v1^2+v1^3+(v2+1)^100").unwrap();
+        assert_eq!(out, ref_out)
+    }
+
+    #[test]
     fn collect_wrap() {
         let input = Atom::parse("v1*(1+v3)+v1*5*v2+f1(5,v1)+2+v2^2+v1^2+v1^3").unwrap();
         let x = State::get_symbol("v1");
         let key = State::get_symbol("f3");
         let coeff = State::get_symbol("f4");
         println!("> Collect in x with wrapping:");
         let out = input.collect(
```

### Comparing `symbolica-0.4.0/src/combinatorics.rs` & `symbolica-0.5.0/src/combinatorics.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/domains/algebraic_number.rs` & `symbolica-0.5.0/src/domains/algebraic_number.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/domains/factorized_rational_polynomial.rs` & `symbolica-0.5.0/src/domains/factorized_rational_polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/domains/finite_field.rs` & `symbolica-0.5.0/src/domains/finite_field.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/domains/float.rs` & `symbolica-0.5.0/src/domains/float.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/domains/integer.rs` & `symbolica-0.5.0/src/domains/integer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -328,14 +328,22 @@
     }
 
     #[inline]
     pub fn one() -> Integer {
         Integer::Natural(1)
     }
 
+    #[inline]
+    pub fn to_i64(&self) -> Option<i64> {
+        match self {
+            Integer::Natural(n) => Some(*n as i64),
+            _ => None,
+        }
+    }
+
     pub fn abs(&self) -> Integer {
         match self {
             Integer::Natural(n) => {
                 if *n == i64::MIN {
                     Integer::Double((*n as i128).abs())
                 } else {
                     Integer::Natural(n.abs())
@@ -453,14 +461,62 @@
                     Integer::Large(MultiPrecisionInteger::from(*n1).pow(e))
                 }
             }
             Integer::Large(r) => Integer::Large(r.pow(e).into()),
         }
     }
 
+    pub fn gcd(&self, b: &Integer) -> Integer {
+        match (self, b) {
+            (Integer::Natural(n1), Integer::Natural(n2)) => {
+                let gcd = utils::gcd_signed(*n1, *n2);
+                if gcd == i64::MAX as u64 + 1 {
+                    // n1 == n2 == u64::MIN
+                    Integer::Double(gcd as i128)
+                } else {
+                    Integer::Natural(gcd as i64)
+                }
+            }
+            (Integer::Natural(n1), Integer::Large(r2))
+            | (Integer::Large(r2), Integer::Natural(n1)) => {
+                let r1 = MultiPrecisionInteger::from(*n1);
+                Integer::from_large(r1.gcd(r2))
+            }
+            (Integer::Large(r1), Integer::Large(r2)) => Integer::from_large(r1.clone().gcd(r2)),
+            (Integer::Natural(r1), Integer::Double(r2))
+            | (Integer::Double(r2), Integer::Natural(r1)) => {
+                Integer::from_double(utils::gcd_signed_i128(*r1 as i128, *r2) as i128)
+            }
+            (Integer::Double(r1), Integer::Double(r2)) => {
+                let gcd = utils::gcd_signed_i128(*r1, *r2);
+                if gcd == i128::MAX as u128 + 1 {
+                    Integer::Large(MultiPrecisionInteger::from(gcd))
+                } else {
+                    Integer::from_double(gcd as i128)
+                }
+            }
+            (Integer::Double(r1), Integer::Large(r2)) => {
+                Integer::from_large(MultiPrecisionInteger::from(*r1).clone().gcd(r2))
+            }
+            (Integer::Large(r1), Integer::Double(r2)) => {
+                Integer::from_large(r1.clone().gcd(&MultiPrecisionInteger::from(*r2)))
+            }
+        }
+    }
+
+    /// Compute the least common multiple of two integers.
+    pub fn lcm(&self, b: &Integer) -> Integer {
+        let g = self.gcd(b);
+        if g.is_zero() {
+            Integer::zero()
+        } else {
+            (self / &g) * b
+        }
+    }
+
     /// Use Garner's algorithm for the Chinese remainder theorem
     /// to reconstruct an `x` that satisfies `n1 = x % p1` and `n2 = x % p2`.
     /// The `x` will be in the range `[-p1*p2/2,p1*p2/2]`.
     pub fn chinese_remainder(n1: Integer, n2: Integer, p1: Integer, p2: Integer) -> Integer {
         // make sure n1 < n2
         if match (&n1, &n2) {
             (Integer::Natural(n1), Integer::Natural(n2)) => n1 > n2,
@@ -837,49 +893,15 @@
                 let r = a.clone().div_rem_euc(MultiPrecisionInteger::from(*b));
                 (Integer::from_large(r.0), Integer::from_large(r.1))
             }
         }
     }
 
     fn gcd(&self, a: &Self::Element, b: &Self::Element) -> Self::Element {
-        match (a, b) {
-            (Integer::Natural(n1), Integer::Natural(n2)) => {
-                let gcd = utils::gcd_signed(*n1, *n2);
-                if gcd == i64::MAX as u64 + 1 {
-                    // n1 == n2 == u64::MIN
-                    Integer::Double(gcd as i128)
-                } else {
-                    Integer::Natural(gcd as i64)
-                }
-            }
-            (Integer::Natural(n1), Integer::Large(r2))
-            | (Integer::Large(r2), Integer::Natural(n1)) => {
-                let r1 = MultiPrecisionInteger::from(*n1);
-                Integer::from_large(r1.gcd(r2))
-            }
-            (Integer::Large(r1), Integer::Large(r2)) => Integer::from_large(r1.clone().gcd(r2)),
-            (Integer::Natural(r1), Integer::Double(r2))
-            | (Integer::Double(r2), Integer::Natural(r1)) => {
-                Integer::from_double(utils::gcd_signed_i128(*r1 as i128, *r2) as i128)
-            }
-            (Integer::Double(r1), Integer::Double(r2)) => {
-                let gcd = utils::gcd_signed_i128(*r1, *r2);
-                if gcd == i128::MAX as u128 + 1 {
-                    Integer::Large(MultiPrecisionInteger::from(gcd))
-                } else {
-                    Integer::from_double(gcd as i128)
-                }
-            }
-            (Integer::Double(r1), Integer::Large(r2)) => {
-                Integer::from_large(MultiPrecisionInteger::from(*r1).clone().gcd(r2))
-            }
-            (Integer::Large(r1), Integer::Double(r2)) => {
-                Integer::from_large(r1.clone().gcd(&MultiPrecisionInteger::from(*r2)))
-            }
-        }
+        a.gcd(b)
     }
 }
 
 impl<'b> Add<&'b Integer> for Integer {
     type Output = Integer;
 
     #[inline(always)]
```

### Comparing `symbolica-0.4.0/src/domains/rational.rs` & `symbolica-0.5.0/src/domains/rational.rs`

 * *Files 1% similar despite different names*

```diff
@@ -802,14 +802,20 @@
         let a = &self.numerator() * &other.denominator();
         let b = &self.denominator() * &other.numerator();
 
         a.partial_cmp(&b)
     }
 }
 
+impl Ord for Rational {
+    fn cmp(&self, other: &Self) -> std::cmp::Ordering {
+        self.partial_cmp(other).unwrap()
+    }
+}
+
 impl Add<Rational> for Rational {
     type Output = Rational;
 
     fn add(self, other: Rational) -> Self::Output {
         Q.add(&self, &other)
     }
 }
```

### Comparing `symbolica-0.4.0/src/domains/rational_polynomial.rs` & `symbolica-0.5.0/src/domains/rational_polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/domains.rs` & `symbolica-0.5.0/src/domains.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 pub mod algebraic_number;
+pub mod atom;
 pub mod factorized_rational_polynomial;
 pub mod finite_field;
 pub mod float;
 pub mod integer;
 pub mod rational;
 pub mod rational_polynomial;
```

### Comparing `symbolica-0.4.0/src/evaluate.rs` & `symbolica-0.5.0/src/evaluate.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/expand.rs` & `symbolica-0.5.0/src/expand.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,96 @@
 use std::ops::DerefMut;
 
 use smallvec::SmallVec;
 
 use crate::{
-    atom::{Atom, AtomView},
+    atom::{Atom, AtomView, Symbol},
     coefficient::CoefficientView,
     combinatorics::CombinationWithReplacementIterator,
     domains::integer::Integer,
     state::{RecycledAtom, Workspace},
 };
 
 impl Atom {
     /// Expand an expression.
     pub fn expand(&self) -> Atom {
         self.as_view().expand()
     }
 
+    /// Expand an expression in the variable `var`.
+    pub fn expand_in(&self, var: Symbol) -> Atom {
+        self.as_view().expand_in(var)
+    }
+
     /// Expand an expression, returning `true` iff the expression changed.
     pub fn expand_into(&self, out: &mut Atom) -> bool {
-        self.as_view().expand_into(out)
+        self.as_view().expand_into(None, out)
     }
 }
 
 impl<'a> AtomView<'a> {
     /// Expand an expression.
     pub fn expand(&self) -> Atom {
         Workspace::get_local().with(|ws| {
             let mut a = ws.new_atom();
-            self.expand_with_ws_into(ws, &mut a);
+            self.expand_with_ws_into(ws, None, &mut a);
+            a.into_inner()
+        })
+    }
+
+    /// Expand an expression.
+    pub fn expand_in(&self, var: Symbol) -> Atom {
+        Workspace::get_local().with(|ws| {
+            let mut a = ws.new_atom();
+            self.expand_with_ws_into(ws, Some(var), &mut a);
             a.into_inner()
         })
     }
 
     /// Expand an expression, returning `true` iff the expression changed.
-    pub fn expand_into(&self, out: &mut Atom) -> bool {
-        Workspace::get_local().with(|ws| self.expand_with_ws_into(ws, out))
+    pub fn expand_into(&self, var: Option<Symbol>, out: &mut Atom) -> bool {
+        Workspace::get_local().with(|ws| self.expand_with_ws_into(ws, var, out))
     }
 
     /// Expand an expression, returning `true` iff the expression changed.
-    pub fn expand_with_ws_into(&self, workspace: &Workspace, out: &mut Atom) -> bool {
-        let changed = self.expand_no_norm(workspace, out);
+    pub fn expand_with_ws_into(
+        &self,
+        workspace: &Workspace,
+        var: Option<Symbol>,
+        out: &mut Atom,
+    ) -> bool {
+        let changed = self.expand_no_norm(workspace, var, out);
 
         if changed {
             let mut a = workspace.new_atom();
             out.as_view().normalize(workspace, &mut a);
             std::mem::swap(out, &mut a);
         }
 
         changed
     }
 
     /// Expand an expression, but do not normalize the result.
-    fn expand_no_norm(&self, workspace: &Workspace, out: &mut Atom) -> bool {
+    fn expand_no_norm(&self, workspace: &Workspace, var: Option<Symbol>, out: &mut Atom) -> bool {
+        if let Some(s) = var {
+            if !self.contains_symbol(s) {
+                out.set_from_view(self);
+                return false;
+            }
+        }
+
         match self {
             AtomView::Pow(p) => {
                 let (base, exp) = p.get_base_exp();
 
                 let mut new_base = workspace.new_atom();
-                let mut changed = base.expand_with_ws_into(workspace, &mut new_base);
+                let mut changed = base.expand_with_ws_into(workspace, var, &mut new_base);
 
                 let mut new_exp = workspace.new_atom();
-                changed |= exp.expand_with_ws_into(workspace, &mut new_exp);
+                changed |= exp.expand_with_ws_into(workspace, var, &mut new_exp);
 
                 let (negative, num) = 'get_num: {
                     if let AtomView::Num(n) = new_exp.as_view() {
                         if let CoefficientView::Natural(n, 1) = n.get_coeff_view() {
                             if n.unsigned_abs() <= u32::MAX as u64 {
                                 break 'get_num (n < 0, n.unsigned_abs() as u32);
                             }
@@ -104,17 +130,19 @@
                             }
                         }
 
                         let mut normalized_child = workspace.new_atom();
                         hh.as_view().normalize(workspace, &mut normalized_child);
 
                         let mut expanded_child = workspace.new_atom();
-                        normalized_child
-                            .as_view()
-                            .expand_with_ws_into(workspace, &mut expanded_child);
+                        normalized_child.as_view().expand_with_ws_into(
+                            workspace,
+                            var,
+                            &mut expanded_child,
+                        );
 
                         let coeff_f = Integer::multinom(new_term);
                         if coeff_f != Integer::one() {
                             let mut coeff_h = workspace.new_atom();
                             coeff_h.to_num(coeff_f.into());
 
                             if let Atom::Mul(m) = expanded_child.deref_mut() {
@@ -177,15 +205,15 @@
                 let mut changed = false;
 
                 let mut sum: SmallVec<[RecycledAtom; 10]> = SmallVec::new();
                 let mut new_sum: SmallVec<[RecycledAtom; 10]> = SmallVec::new();
 
                 for arg in m.iter() {
                     let mut new_arg = workspace.new_atom();
-                    changed |= arg.expand_with_ws_into(workspace, &mut new_arg);
+                    changed |= arg.expand_with_ws_into(workspace, var, &mut new_arg);
 
                     // expand (1+x)*y
                     if let AtomView::Add(a) = new_arg.as_view() {
                         changed = true;
 
                         for child in a.iter() {
                             for s in &sum {
@@ -251,15 +279,15 @@
             AtomView::Add(a) => {
                 let mut changed = false;
 
                 let add = out.to_add();
 
                 let mut new_arg = workspace.new_atom();
                 for arg in a.iter() {
-                    changed |= arg.expand_no_norm(workspace, &mut new_arg);
+                    changed |= arg.expand_no_norm(workspace, var, &mut new_arg);
                     add.extend(new_arg.as_view());
                 }
 
                 add.set_normalized(!changed);
                 changed
             }
             _ => {
@@ -268,15 +296,15 @@
             }
         }
     }
 }
 
 #[cfg(test)]
 mod test {
-    use crate::atom::Atom;
+    use crate::{atom::Atom, state::State};
 
     #[test]
     fn exponent() {
         let exp = Atom::parse("(1+v1+v2)^4").unwrap().expand();
         let res = Atom::parse("4*v1+4*v2+6*v1^2+4*v1^3+v1^4+6*v2^2+4*v2^3+v2^4+12*v1*v2+12*v1*v2^2+4*v1*v2^3+12*v1^2*v2+6*v1^2*v2^2+4*v1^3*v2+1").unwrap();
         assert_eq!(exp, res);
     }
@@ -297,8 +325,17 @@
 
     #[test]
     fn mul_pow_neg() {
         let exp = Atom::parse("(v1*v2*2)^-3").unwrap().expand();
         let res = Atom::parse("8^-1*v1^-3*v2^-3").unwrap();
         assert_eq!(exp, res);
     }
+
+    #[test]
+    fn expand_in_var() {
+        let exp = Atom::parse("(1+v1)^2+(1+v2)^100")
+            .unwrap()
+            .expand_in(State::get_symbol("v1"));
+        let res = Atom::parse("1+2*v1+v1^2+(v2+1)^100").unwrap();
+        assert_eq!(exp, res);
+    }
 }
```

### Comparing `symbolica-0.4.0/src/id.rs` & `symbolica-0.5.0/src/id.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use ahash::HashSet;
 use dyn_clone::DynClone;
 
 use crate::{
-    atom::{representation::ListSlice, Atom, AtomView, Num, SliceType, Symbol},
+    atom::{representation::ListSlice, Atom, AtomType, AtomView, Num, SliceType, Symbol},
     state::{State, Workspace},
     transformer::{Transformer, TransformerError},
 };
 
 #[derive(Clone)]
 pub enum Pattern {
     Literal(Atom),
@@ -937,24 +937,14 @@
 dyn_clone::clone_trait_object!(FilterFn);
 impl<T: Clone + Send + Sync + for<'a, 'b> Fn(&'a Match<'b>) -> bool> FilterFn for T {}
 
 pub trait CmpFn: for<'a, 'b> Fn(&Match<'_>, &Match<'_>) -> bool + DynClone + Send + Sync {}
 dyn_clone::clone_trait_object!(CmpFn);
 impl<T: Clone + Send + Sync + for<'a, 'b> Fn(&Match<'_>, &Match<'_>) -> bool> CmpFn for T {}
 
-#[derive(Debug, Clone, Copy, PartialEq, Eq)]
-pub enum AtomType {
-    Num,
-    Var,
-    Add,
-    Mul,
-    Pow,
-    Fun,
-}
-
 /// Restrictions for a wildcard. Note that a length restriction
 /// applies at any level and therefore
 /// `x_*f(x_) : length(x) == 2`
 /// does not match to `x*y*f(x*y)`, since the pattern `x_` has length
 /// 1 inside the function argument.
 pub enum PatternRestriction {
     Length(usize, Option<usize>), // min-max range
@@ -1298,16 +1288,15 @@
                 }
                 SliceType::Empty => {
                     let f = out.to_fun(State::ARG);
                     f.set_normalized(true);
                 }
             },
             Self::FunctionName(n) => {
-                let f = out.to_fun(*n);
-                f.set_normalized(true);
+                out.to_var(*n);
             }
         }
     }
 }
 
 /// Settings related to pattern matching.
 #[derive(Default, Clone)]
```

### Comparing `symbolica-0.4.0/src/lib.rs` & `symbolica-0.5.0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -29,30 +29,30 @@
     time::{Duration, SystemTime},
 };
 
 use colored::Colorize;
 use once_cell::sync::OnceCell;
 use tinyjson::JsonValue;
 
-pub mod api;
+mod api;
 pub mod atom;
 pub mod coefficient;
-pub mod collect;
+mod collect;
 pub mod combinatorics;
-pub mod derivative;
+mod derivative;
 pub mod domains;
 pub mod evaluate;
-pub mod expand;
+mod expand;
 pub mod id;
-pub mod normalize;
+mod normalize;
 pub mod numerical_integration;
 pub mod parser;
 pub mod poly;
 pub mod printer;
-pub mod solve;
+mod solve;
 pub mod state;
 pub mod streaming;
 pub mod tensors;
 pub mod transformer;
 pub mod utils;
 
 #[cfg(feature = "faster_alloc")]
```

### Comparing `symbolica-0.4.0/src/normalize.rs` & `symbolica-0.5.0/src/normalize.rs`

 * *Files 6% similar despite different names*

```diff
@@ -267,29 +267,102 @@
                 } else {
                     f1.fast_cmp(*f2)
                 }
             }
             (AtomView::Add(_), _) | (_, AtomView::Add(_)) => unreachable!("Cannot have nested add"),
         }
     }
+
+    /// Simplify logs in the argument of the exponential function.
+    fn simplify_exp_log(&self, ws: &Workspace, out: &mut Atom) -> bool {
+        if let AtomView::Fun(f) = self {
+            if f.get_symbol() == State::LOG && f.get_nargs() == 1 {
+                out.set_from_view(&f.iter().next().unwrap());
+                return true;
+            }
+        }
+
+        if let AtomView::Mul(m) = self {
+            let mut found_index = None;
+            for (i, a) in m.iter().enumerate() {
+                if a.simplify_exp_log(ws, out) {
+                    if found_index.is_some() {
+                        return false;
+                    }
+
+                    found_index = Some(i);
+                }
+            }
+
+            if let Some(i) = found_index {
+                let mut mm = ws.new_atom();
+                let mmm = mm.to_mul();
+                for (j, a) in m.iter().enumerate() {
+                    if j != i {
+                        mmm.extend(a);
+                    }
+                }
+
+                let mut b = ws.new_atom();
+                b.to_pow(out.as_view(), mm.as_view());
+
+                b.as_view().normalize(ws, out);
+                return true;
+            } else {
+                return false;
+            }
+        }
+
+        if let AtomView::Add(a) = self {
+            // all terms must simplify
+            let mut mm = ws.new_atom();
+            let m = mm.to_mul();
+
+            let mut aa = ws.new_atom();
+            let aaa = aa.to_add();
+
+            let mut changed = false;
+            for a in a.iter() {
+                if a.simplify_exp_log(ws, out) {
+                    changed = true;
+                    m.extend(out.as_view());
+                } else {
+                    aaa.extend(a);
+                }
+            }
+
+            if changed {
+                let mut new_exp = ws.new_atom();
+                // TODO: change to e^()
+                new_exp.to_fun(State::EXP).add_arg(aa.as_view());
+
+                m.extend(new_exp.as_view());
+
+                mm.as_view().normalize(ws, out);
+            }
+
+            return changed;
+        }
+
+        false
+    }
 }
 
 impl Atom {
     /// Merge two factors if possible. If this function returns `true`, `self`
     /// will have been updated by the merge from `other` and `other` should be discarded.
     /// If the function return `false`, no merge was possible and no modifications were made.
     fn merge_factors(
         &mut self,
         other: &mut Self,
         helper: &mut Self,
-
         workspace: &Workspace,
     ) -> bool {
-        // x^a * x^b = x^(a + b)
         if let Atom::Pow(p1) = self {
+            // x^a * x^b = x^(a + b)
             if let Atom::Pow(p2) = other {
                 let (base2, exp2) = p2.to_pow_view().get_base_exp();
 
                 let (base1, exp1) = p1.to_pow_view().get_base_exp();
 
                 if base1 != base2 {
                     return false;
@@ -317,14 +390,48 @@
                 new_exp.extend(exp2);
                 let mut helper2 = workspace.new_atom();
                 helper.as_view().normalize(workspace, &mut helper2);
                 p1.set_from_base_and_exp(base2, helper2.as_view());
                 p1.set_normalized(true);
                 return true;
             }
+
+            // x^n * x = x^(n+1)
+            let pv = p1.to_pow_view();
+            let (base, exp) = pv.get_base_exp();
+
+            if other.as_view() == base {
+                if let AtomView::Num(n) = &exp {
+                    let new_exp = n.get_coeff_view() + 1;
+
+                    if new_exp.is_zero() {
+                        self.to_num(1.into());
+                    } else if new_exp == 1.into() {
+                        self.set_from_view(&other.as_view());
+                    } else {
+                        let num = helper.to_num(new_exp);
+                        self.to_pow(other.as_view(), AtomView::Num(num.to_num_view()));
+                    }
+                } else {
+                    other.to_num(1.into());
+
+                    let new_exp = helper.to_add();
+                    new_exp.extend(other.as_view());
+                    new_exp.extend(exp);
+                    let mut helper2 = workspace.new_atom();
+                    helper.as_view().normalize(workspace, &mut helper2);
+                    other.to_pow(base, helper2.as_view());
+                    std::mem::swap(self, other);
+                }
+
+                self.set_normalized(true);
+                return true;
+            }
+
+            return false;
         }
 
         // x * x^n = x^(n+1)
         if let Atom::Pow(p) = other {
             let pv = p.to_pow_view();
             let (base, exp) = pv.get_base_exp();
 
@@ -576,14 +683,15 @@
             return;
         }
 
         match self {
             AtomView::Mul(t) => {
                 let mut atom_test_buf: SmallVec<[_; 20]> = SmallVec::new();
 
+                let mut is_zero = false;
                 for a in t.iter() {
                     let mut handle = workspace.new_atom();
 
                     if a.needs_normalization() {
                         a.normalize(workspace, &mut handle);
                     } else {
                         handle.set_from_view(&a);
@@ -598,36 +706,42 @@
                             if let AtomView::Num(n) = c {
                                 if n.is_one() {
                                     continue;
                                 }
 
                                 if n.is_zero() {
                                     out.to_num(Coefficient::zero());
-                                    return;
+                                    is_zero = true;
+                                    continue; // do not return as we may encounter 0/0
                                 }
                             }
 
                             atom_test_buf.push(handle);
                         }
                     } else {
                         if let AtomView::Num(n) = handle.as_view() {
                             if n.is_one() {
                                 continue;
                             }
 
                             if n.is_zero() {
                                 out.to_num(Coefficient::zero());
-                                return;
+                                is_zero = true;
+                                continue;
                             }
                         }
 
                         atom_test_buf.push(handle);
                     }
                 }
 
+                if is_zero {
+                    return;
+                }
+
                 atom_test_buf.sort_by(|a, b| a.as_view().cmp_factors(&b.as_view()));
 
                 if !atom_test_buf.is_empty() {
                     let out_mul = out.to_mul();
 
                     let mut last_buf = atom_test_buf.remove(0);
 
@@ -760,14 +874,26 @@
                                 out.set_from_view(&buffer.as_view());
                                 return;
                             }
                         }
                     }
                 }
 
+                if id == State::EXP && out_f.to_fun_view().get_nargs() == 1 {
+                    let arg = out_f.to_fun_view().iter().next().unwrap();
+                    // simplify logs inside exp
+                    if arg.contains_symbol(State::LOG) {
+                        let mut buffer = workspace.new_atom();
+                        if arg.simplify_exp_log(workspace, &mut buffer) {
+                            out.set_from_view(&buffer.as_view());
+                        }
+                        return;
+                    }
+                }
+
                 // try to turn the argument into a number
                 if id == State::COEFF && out_f.to_fun_view().get_nargs() == 1 {
                     let arg = out_f.to_fun_view().iter().next().unwrap();
                     if let AtomView::Num(_) = arg {
                         let mut buffer = workspace.new_atom();
                         buffer.set_from_view(&arg);
                         out.set_from_view(&buffer.as_view());
@@ -945,14 +1071,19 @@
                     exp.normalize(workspace, &mut exp_handle);
                 } else {
                     // TODO: prevent copy
                     exp_handle.set_from_view(&exp);
                 };
 
                 'pow_simplify: {
+                    if base_handle.is_one() {
+                        out.to_num(1.into());
+                        break 'pow_simplify;
+                    }
+
                     if let AtomView::Num(e) = exp_handle.as_view() {
                         let exp_num = e.get_coeff_view();
                         if exp_num == CoefficientView::Natural(0, 1) {
                             // x^0 = 1
                             out.to_num(1.into());
                             break 'pow_simplify;
                         } else if exp_num == CoefficientView::Natural(1, 1) {
@@ -1002,37 +1133,45 @@
                                         out.to_pow(new_base.as_view(), new_exp.as_view());
                                     }
 
                                     break 'pow_simplify;
                                 }
                             }
                         } else if let AtomView::Pow(p_base) = base_handle.as_view() {
-                            // simplify x^2^3
-                            let (p_base_base, p_base_exp) = p_base.get_base_exp();
-                            if let AtomView::Num(n) = p_base_exp {
-                                let new_exp = n.get_coeff_view() * exp_num;
+                            if exp_num.is_integer() {
+                                // rewrite (x^y)^3 as x^(3*y)
+                                let (p_base_base, p_base_exp) = p_base.get_base_exp();
+
+                                let mut mul_h = workspace.new_atom();
+                                let mul = mul_h.to_mul();
+                                mul.extend(p_base_exp);
+                                mul.extend(exp_handle.as_view());
+                                let mut exp_h = workspace.new_atom();
+                                mul.as_view().normalize(workspace, &mut exp_h);
 
-                                if new_exp == 1.into() {
-                                    out.set_from_view(&p_base_base);
-                                    break 'pow_simplify;
+                                mul_h.to_pow(p_base_base, exp_h.as_view());
+                                mul_h.as_view().normalize(workspace, out);
+                                break 'pow_simplify;
+                            }
+                        } else if let AtomView::Mul(m) = base_handle.as_view() {
+                            // rewrite (x*y)^2 as x^2*y^2
+                            if exp_num.is_integer() {
+                                let mut mul_h = workspace.new_atom();
+                                let mul = mul_h.to_mul();
+                                for arg in m.iter() {
+                                    let mut pow_h = workspace.new_atom();
+                                    pow_h.to_pow(arg, exp_handle.as_view());
+                                    mul.extend(pow_h.as_view());
                                 }
 
-                                exp_handle.to_num(new_exp);
-
-                                let p = out.to_pow(p_base_base, exp_handle.as_view());
-                                p.set_normalized(true);
-
+                                mul_h.as_view().normalize(workspace, out);
                                 break 'pow_simplify;
                             }
-                        } else if let AtomView::Mul(_) = base_handle.as_view() {
-                            // TODO: turn (x*y)^2 into x^2*y^2?
-                            // for now, expand() needs to be used
                         }
                     }
-
                     out.to_pow(base_handle.as_view(), exp_handle.as_view());
                 }
 
                 out.set_normalized(true);
             }
             AtomView::Add(a) => {
                 let mut new_sum = workspace.new_atom();
@@ -1132,14 +1271,32 @@
 }
 
 #[cfg(test)]
 mod test {
     use crate::{atom::Atom, state::State};
 
     #[test]
+    fn pow_apart() {
+        let res = Atom::parse("v1*(v1*v2*v3)^-5").unwrap();
+        let refr = Atom::parse("v1^-4*v2^-5*v3^-5").unwrap();
+        assert_eq!(res, refr);
+    }
+
+    #[test]
+    fn pow_simplify() {
+        assert_eq!(Atom::parse("1^(1/2)"), Atom::parse("1"));
+        assert_eq!(
+            format!("{}", Atom::parse("(v1^2)^v2").unwrap()),
+            "(v1^2)^v2"
+        );
+        assert_eq!(Atom::parse("(v1^v2)^2"), Atom::parse("v1^(2*v2)"));
+        assert_eq!(Atom::parse("(v1^(1/2))^2"), Atom::parse("v1"));
+    }
+
+    #[test]
     fn linear_symmetric() {
         let res = Atom::parse("fsl1(v2+2*v3,v1+3*v2-v3)").unwrap();
         let refr =
             Atom::parse("fsl1(v1,v2)+2*fsl1(v1,v3)+3*fsl1(v2,v2)+5*fsl1(v2,v3)-2*fsl1(v3,v3)")
                 .unwrap();
         assert_eq!(res, refr);
     }
```

### Comparing `symbolica-0.4.0/src/numerical_integration.rs` & `symbolica-0.5.0/src/numerical_integration.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/parser.rs` & `symbolica-0.5.0/src/parser.rs`

 * *Files 2% similar despite different names*

```diff
@@ -348,24 +348,30 @@
                 self
             ))
         }
     }
 
     /// Parse the token into an atom.
     pub fn to_atom(&self, workspace: &Workspace) -> Result<Atom, String> {
-        let mut atom = Atom::default();
+        let mut atom = workspace.new_atom();
 
-        let mut state = State::get_global_state().write().unwrap();
-        self.to_atom_with_output(&mut state, workspace, &mut atom)?;
+        {
+            let mut state = State::get_global_state().write().unwrap();
+            // do not normalize to prevent potential deadlocks
+            self.to_atom_with_output_no_norm(&mut state, workspace, &mut atom)?;
+        }
+
+        let mut out = Atom::new();
+        atom.as_view().normalize(workspace, &mut out);
 
-        Ok(atom)
+        Ok(out)
     }
 
     /// Parse the token into the atom `out`.
-    fn to_atom_with_output(
+    fn to_atom_with_output_no_norm(
         &self,
         state: &mut State,
         workspace: &Workspace,
         out: &mut Atom,
     ) -> Result<(), String> {
         match self {
             Token::Number(n) => match n.parse::<Integer>() {
@@ -375,94 +381,81 @@
                 Err(e) => return Err(format!("Could not parse number: {}", e)),
             },
             Token::ID(x) => {
                 out.to_var(state.get_symbol_impl(x));
             }
             Token::Op(_, _, op, args) => match op {
                 Operator::Mul => {
-                    let mut mul_h = workspace.new_atom();
-                    let mul = mul_h.to_mul();
+                    let mul = out.to_mul();
 
                     let mut atom = workspace.new_atom();
                     for a in args {
-                        a.to_atom_with_output(state, workspace, &mut atom)?;
+                        a.to_atom_with_output_no_norm(state, workspace, &mut atom)?;
                         mul.extend(atom.as_view());
                     }
-
-                    mul_h.as_view().normalize(workspace, out);
                 }
                 Operator::Add => {
-                    let mut add_h = workspace.new_atom();
-                    let add = add_h.to_add();
+                    let add = out.to_add();
 
                     let mut atom = workspace.new_atom();
                     for a in args {
-                        a.to_atom_with_output(state, workspace, &mut atom)?;
+                        a.to_atom_with_output_no_norm(state, workspace, &mut atom)?;
                         add.extend(atom.as_view());
                     }
-
-                    add_h.as_view().normalize(workspace, out);
                 }
                 Operator::Pow => {
                     // pow is right associative
                     args.last()
                         .unwrap()
-                        .to_atom_with_output(state, workspace, out)?;
+                        .to_atom_with_output_no_norm(state, workspace, out)?;
                     for a in args.iter().rev().skip(1) {
                         let mut cur_base = workspace.new_atom();
-                        a.to_atom_with_output(state, workspace, &mut cur_base)?;
+                        a.to_atom_with_output_no_norm(state, workspace, &mut cur_base)?;
 
                         let mut pow_h = workspace.new_atom();
                         pow_h.to_pow(cur_base.as_view(), out.as_view());
-                        pow_h.as_view().normalize(workspace, out);
+                        out.set_from_view(&pow_h.as_view());
                     }
                 }
                 Operator::Argument => return Err("Unexpected argument operator".into()),
                 Operator::Neg => {
                     debug_assert!(args.len() == 1);
 
                     let mut base = workspace.new_atom();
-                    args[0].to_atom_with_output(state, workspace, &mut base)?;
+                    args[0].to_atom_with_output_no_norm(state, workspace, &mut base)?;
 
                     let num = workspace.new_num(-1);
 
-                    let mut mul_h = workspace.new_atom();
-                    let mul = mul_h.to_mul();
+                    let mul = out.to_mul();
                     mul.extend(base.as_view());
                     mul.extend(num.as_view());
-                    mul_h.as_view().normalize(workspace, out);
                 }
                 Operator::Inv => {
                     debug_assert!(args.len() == 1);
 
                     let mut base = workspace.new_atom();
-                    args[0].to_atom_with_output(state, workspace, &mut base)?;
+                    args[0].to_atom_with_output_no_norm(state, workspace, &mut base)?;
 
                     let num = workspace.new_num(-1);
 
-                    let mut pow_h = workspace.new_atom();
-                    pow_h.to_pow(base.as_view(), num.as_view());
-                    pow_h.as_view().normalize(workspace, out);
+                    out.to_pow(base.as_view(), num.as_view());
                 }
             },
             Token::Fn(_, args) => {
                 let name = match &args[0] {
                     Token::ID(s) => s,
                     _ => unreachable!(),
                 };
 
-                let mut fun_h = workspace.new_atom();
-                let fun = fun_h.to_fun(state.get_symbol_impl(name));
+                let fun = out.to_fun(state.get_symbol_impl(name));
                 let mut atom = workspace.new_atom();
                 for a in args.iter().skip(1) {
-                    a.to_atom_with_output(state, workspace, &mut atom)?;
+                    a.to_atom_with_output_no_norm(state, workspace, &mut atom)?;
                     fun.add_arg(atom.as_view());
                 }
-
-                fun_h.as_view().normalize(workspace, out);
             }
             x => return Err(format!("Unexpected token {}", x)),
         }
 
         Ok(())
     }
 
@@ -1168,16 +1161,16 @@
     use crate::{atom::Atom, domains::integer::Z, parser::Token, state::State};
 
     #[test]
     fn pow() {
         let input = Atom::parse("v1^v2^v3^3").unwrap();
         assert_eq!(format!("{}", input), "v1^v2^v3^3");
 
-        let input = Atom::parse("(v1^v2)^3").unwrap();
-        assert_eq!(format!("{}", input), "(v1^v2)^3");
+        let input = Atom::parse("(v1^v2)^v3").unwrap();
+        assert_eq!(format!("{}", input), "(v1^v2)^v3");
     }
 
     #[test]
     fn unary() {
         let input = Atom::parse("-x^z").unwrap();
         assert_eq!(format!("{}", input), "-x^z");
```

### Comparing `symbolica-0.4.0/src/poly/evaluate.rs` & `symbolica-0.5.0/src/poly/evaluate.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/poly/factor.rs` & `symbolica-0.5.0/src/poly/factor.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/poly/gcd.rs` & `symbolica-0.5.0/src/poly/gcd.rs`

 * *Files 0% similar despite different names*

```diff
@@ -2869,25 +2869,28 @@
 
                     let gmc_a = &mut gm.coefficients[t];
 
                     // apply CRT to each integer coefficient in the algebraic number ring
                     let mut gpc_pos = 0;
                     let mut gmc_pos = 0;
                     for i in 0..a.field.poly().degree(0) {
-                        let gpc = if i == gpc.poly.exponents(gpc_pos)[0] {
-                            gpc_pos += 1;
-                            Integer::from_finite_field(
-                                &finite_field,
-                                gpc.poly.coefficients[gpc_pos - 1],
-                            )
-                        } else {
-                            Integer::zero()
-                        };
+                        let gpc =
+                            if gpc_pos < gpc.poly.nterms() && i == gpc.poly.exponents(gpc_pos)[0] {
+                                gpc_pos += 1;
+                                Integer::from_finite_field(
+                                    &finite_field,
+                                    gpc.poly.coefficients[gpc_pos - 1],
+                                )
+                            } else {
+                                Integer::zero()
+                            };
 
-                        let gpm = if i == gmc_a.poly.exponents(gmc_pos)[0] {
+                        let gpm = if gmc_pos < gmc_a.poly.nterms()
+                            && i == gmc_a.poly.exponents(gmc_pos)[0]
+                        {
                             gmc_pos += 1;
                             let r = &gmc_a.poly.coefficients[gmc_pos - 1];
                             if r.is_negative() {
                                 r + &m
                             } else {
                                 r.clone()
                             }
```

### Comparing `symbolica-0.4.0/src/poly/groebner.rs` & `symbolica-0.5.0/src/poly/groebner.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/poly/polynomial.rs` & `symbolica-0.5.0/src/poly/polynomial.rs`

 * *Files 1% similar despite different names*

```diff
@@ -285,14 +285,26 @@
             exponents,
             field: self.field.clone(),
             variables: self.variables.clone(),
             _phantom: PhantomData,
         }
     }
 
+    /// Constructs a polynomial with a single term that is a variable.
+    #[inline]
+    pub fn variable(&self, var: &Variable) -> Result<Self, &'static str> {
+        if let Some(pos) = self.variables.iter().position(|v| v == var) {
+            let mut exp = vec![E::zero(); self.nvars()];
+            exp[pos] = E::one();
+            Ok(self.monomial(self.field.one(), exp))
+        } else {
+            Err("Variable not found")
+        }
+    }
+
     /// Get the ith monomial
     pub fn to_monomial_view(&self, i: usize) -> MonomialView<F, E> {
         assert!(i < self.nterms());
 
         MonomialView {
             coefficient: &self.coefficients[i],
             exponents: self.exponents(i),
@@ -513,14 +525,36 @@
         let rend = r.len();
         for i in 0..nterms / 2 {
             l[i * nvars..(i + 1) * nvars]
                 .swap_with_slice(&mut r[rend - (i + 1) * nvars..rend - i * nvars]);
         }
     }
 
+    /// Add a variable to the polynomial if it is not already present.
+    pub fn add_variable(&mut self, var: &Variable) {
+        if self.variables.iter().any(|v| v == var) {
+            return;
+        }
+
+        let l = self.variables.len();
+
+        let mut new_exp = vec![E::zero(); (l + 1) * self.nterms()];
+
+        if l > 0 {
+            for (en, e) in new_exp.chunks_mut(l + 1).zip(self.exponents.chunks(l)) {
+                en[..l].copy_from_slice(e);
+            }
+        }
+
+        let mut new_vars = self.variables.as_ref().clone();
+        new_vars.push(var.clone());
+        self.variables = Arc::new(new_vars);
+        self.exponents = new_exp;
+    }
+
     /// Check if the polynomial is sorted and has only non-zero coefficients
     pub fn check_consistency(&self) {
         assert_eq!(self.coefficients.len(), self.nterms());
         assert_eq!(self.exponents.len(), self.nterms() * self.nvars());
 
         for c in &self.coefficients {
             if F::is_zero(c) {
```

### Comparing `symbolica-0.4.0/src/poly/resultant.rs` & `symbolica-0.5.0/src/poly/resultant.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/poly/univariate.rs` & `symbolica-0.5.0/src/poly/univariate.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/poly.rs` & `symbolica-0.5.0/src/poly.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 pub mod evaluate;
 pub mod factor;
 pub mod gcd;
 pub mod groebner;
 pub mod polynomial;
 pub mod resultant;
+pub mod series;
 pub mod univariate;
 
 use std::borrow::Cow;
 use std::cmp::Ordering::{self, Equal};
 use std::fmt::{Debug, Display};
 use std::hash::Hash;
 use std::iter::Sum;
@@ -389,14 +390,22 @@
         match self {
             Variable::Symbol(v) => format!("{}", State::get_name(*v)),
             Variable::Temporary(t) => format!("_TMP_{}", *t),
             Variable::Function(_, a) | Variable::Other(a) => format!("{}", a),
         }
     }
 
+    pub fn to_atom(&self) -> Atom {
+        match self {
+            Variable::Symbol(s) => Atom::new_var(*s),
+            Variable::Function(_, a) | Variable::Other(a) => a.as_ref().clone(),
+            Variable::Temporary(_) => panic!("Cannot convert a temporary variable to an atom"),
+        }
+    }
+
     /// Check if the symbol `symbol` appears at most once in the variable map.
     /// For example, `[x,f(x)]` is not independent in `x`, but `[x,y]` is.
     pub fn is_independent_symbol(variables: &[Variable], symbol: Symbol) -> bool {
         let mut seen = false;
 
         for v in variables {
             match v {
```

### Comparing `symbolica-0.4.0/src/printer.rs` & `symbolica-0.5.0/src/printer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -367,15 +367,15 @@
                     ff.from_element(&num),
                     ff.get_prime()
                 ))
             }
             CoefficientView::RationalPolynomial(p) => f.write_fmt(format_args!(
                 "[{}]",
                 RationalPolynomialPrinter {
-                    poly: p,
+                    poly: &p.deserialize(),
                     opts: *opts,
                     add_parentheses: false,
                 }
             )),
         }
     }
 }
@@ -1402,15 +1402,20 @@
     }
 
     #[test]
     fn factorized_rational_polynomials() {
         let a = Atom::parse("15 x^2 / ((1+x)(x+2))")
             .unwrap()
             .to_factorized_rational_polynomial::<_, _, u8>(&Z, &Z, None);
-        assert_eq!(format!("{}", a), "15*x^2/((1+x)(2+x))");
+        assert!(
+            format!("{}", a) == "15*x^2/((1+x)(2+x))" || format!("{}", a) == "15*x^2/((2+x)(1+x))"
+        );
 
         let a = Atom::parse("(15 x^2 + 6) / ((1+x)(x+2))")
             .unwrap()
             .to_factorized_rational_polynomial::<_, _, u8>(&Z, &Z, None);
-        assert_eq!(format!("{}", a), "3*(2+5*x^2)/((1+x)(2+x))");
+        assert!(
+            format!("{}", a) == "3*(2+5*x^2)/((1+x)(2+x))"
+                || format!("{}", a) == "3*(2+5*x^2)/((2+x)(1+x))"
+        );
     }
 }
```

### Comparing `symbolica-0.4.0/src/solve.rs` & `symbolica-0.5.0/src/solve.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/tensors/matrix.rs` & `symbolica-0.5.0/src/tensors/matrix.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/src/transformer.rs` & `symbolica-0.5.0/src/transformer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 use std::time::Instant;
 
 use crate::{
     atom::{Atom, AtomView, Symbol},
     coefficient::{Coefficient, CoefficientView},
     combinatorics::{partitions, unique_permutations},
+    domains::rational::Rational,
     id::{Condition, MatchSettings, Pattern, WildcardAndRestriction},
     printer::{AtomPrinter, PrintOptions},
     state::{State, Workspace},
 };
 use ahash::HashMap;
 use colored::Colorize;
 use dyn_clone::DynClone;
@@ -57,19 +58,19 @@
     Interrupt,
 }
 
 /// Operations that take a pattern as the input and produce an expression
 #[derive(Clone)]
 pub enum Transformer {
     /// Expand the rhs.
-    Expand,
+    Expand(Option<Symbol>),
     /// Derive the rhs w.r.t a variable.
     Derivative(Symbol),
     /// Derive the rhs w.r.t a variable.
-    TaylorSeries(Symbol, Atom, u32),
+    Series(Symbol, Atom, Rational),
     /// Apply find-and-replace on the rhs.
     ReplaceAll(
         Pattern,
         Pattern,
         Condition<WildcardAndRestriction>,
         MatchSettings,
     ),
@@ -98,15 +99,15 @@
     Stats(StatsOptions, Vec<Transformer>),
     FromNumber,
 }
 
 impl std::fmt::Debug for Transformer {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         match self {
-            Transformer::Expand => f.debug_tuple("Expand").finish(),
+            Transformer::Expand(s) => f.debug_tuple("Expand").field(s).finish(),
             Transformer::Derivative(x) => f.debug_tuple("Derivative").field(x).finish(),
             Transformer::ReplaceAll(pat, rhs, ..) => {
                 f.debug_tuple("ReplaceAll").field(pat).field(rhs).finish()
             }
             Transformer::Product => f.debug_tuple("Product").finish(),
             Transformer::Sum => f.debug_tuple("Sum").finish(),
             Transformer::ArgCount(p) => f.debug_tuple("ArgCount").field(p).finish(),
@@ -118,15 +119,15 @@
                 .field(g)
                 .field(b1)
                 .field(b2)
                 .finish(),
             Transformer::Sort => f.debug_tuple("Sort").finish(),
             Transformer::Deduplicate => f.debug_tuple("Deduplicate").finish(),
             Transformer::Permutations(i) => f.debug_tuple("Permutations").field(i).finish(),
-            Transformer::TaylorSeries(x, point, d) => f
+            Transformer::Series(x, point, d) => f
                 .debug_tuple("TaylorSeries")
                 .field(x)
                 .field(point)
                 .field(d)
                 .finish(),
             Transformer::Repeat(r) => f.debug_tuple("Repeat").field(r).finish(),
             Transformer::Print(p) => f.debug_tuple("Print").field(p).finish(),
@@ -189,28 +190,26 @@
                             ff.as_view().normalize(workspace, out);
                             continue;
                         }
                     }
 
                     Self::execute(input, t, workspace, out)?;
                 }
-                Transformer::Expand => {
-                    input.expand_with_ws_into(workspace, out);
+                Transformer::Expand(s) => {
+                    input.expand_with_ws_into(workspace, *s, out);
                 }
                 Transformer::Derivative(x) => {
                     input.derivative_with_ws_into(*x, workspace, out);
                 }
-                Transformer::TaylorSeries(x, expansion_point, depth) => {
-                    input.taylor_series_with_ws_into(
-                        *x,
-                        expansion_point.as_view(),
-                        *depth,
-                        workspace,
-                        out,
-                    );
+                Transformer::Series(x, expansion_point, depth) => {
+                    if let Ok(s) = input.series(*x, expansion_point.as_view(), depth.clone()) {
+                        s.to_atom_into(out);
+                    } else {
+                        out.set_from_view(&input);
+                    }
                 }
                 Transformer::ReplaceAll(pat, rhs, cond, settings) => {
                     pat.replace_all_with_ws_into(
                         input,
                         rhs,
                         workspace,
                         cond.into(),
@@ -481,15 +480,19 @@
                         Instant::now().duration_since(t),
                         width = in_nterms_s.len().max(out_nterms_s.len()).min(6),
                     );
                 }
                 Transformer::FromNumber => {
                     if let AtomView::Num(n) = input {
                         if let CoefficientView::RationalPolynomial(r) = n.get_coeff_view() {
-                            r.to_expression_with_map(workspace, &HashMap::default(), out);
+                            r.deserialize().to_expression_with_map(
+                                workspace,
+                                &HashMap::default(),
+                                out,
+                            );
                             continue;
                         }
                     }
 
                     out.set_from_view(&input);
                 }
             }
@@ -516,15 +519,15 @@
         let p = Atom::parse("(1+v1)^2").unwrap();
 
         let mut out = Atom::new();
         Workspace::get_local().with(|ws| {
             Transformer::execute(
                 p.as_view(),
                 &[
-                    Transformer::Expand,
+                    Transformer::Expand(Some(State::get_symbol("v1"))),
                     Transformer::Derivative(State::get_symbol("v1")),
                 ],
                 ws,
                 &mut out,
             )
             .unwrap()
         });
@@ -550,31 +553,31 @@
 
         let r = Atom::parse("3").unwrap();
         assert_eq!(out, r);
     }
 
     #[test]
     fn product_series() {
-        let p = Atom::parse("arg(x,x+1,3)").unwrap();
+        let p = Atom::parse("arg(v1,v1+1,3)").unwrap();
 
         let mut out = Atom::new();
         Workspace::get_local().with(|ws| {
             Transformer::execute(
                 p.as_view(),
                 &[
                     Transformer::Product,
-                    Transformer::TaylorSeries(State::get_symbol("x"), Atom::new_num(1), 3),
+                    Transformer::Series(State::get_symbol("v1"), Atom::new_num(1), 3.into()),
                 ],
                 ws,
                 &mut out,
             )
             .unwrap()
         });
 
-        let r = Atom::parse("3*(x-1)^2+9*(x-1)+6").unwrap();
+        let r = Atom::parse("3*(v1-1)^2+9*(v1-1)+6").unwrap();
         assert_eq!(out, r);
     }
 
     #[test]
     fn sort_deduplicate() {
         let p = Atom::parse("f1(3,2,1,3)").unwrap();
```

### Comparing `symbolica-0.4.0/symbolica.pyi` & `symbolica-0.5.0/symbolica.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -78,76 +78,121 @@
     A Symbolica expression.
 
     Supports standard arithmetic operations, such
     as addition and multiplication.
 
     Examples
     --------
-    >>> x = Expression.var('x')
+    >>> x = Expression.symbol('x')
     >>> e = x**2 + 2 - x + 1 / x**4
     >>> print(e)
     """
 
     E: Expression
     """Euler's number `e`."""
 
     PI: Expression
     """The mathematical constant `π`."""
 
     I: Expression
     """The mathematical constant `i`, where `i^2 = -1`."""
 
-    @classmethod
-    def var(_cls, name: str) -> Expression:
-        """
-        Create a Symbolica expression that is a single variable.
+    COEFF: Expression
+    """The built-in function that convert a rational polynomials to a coefficient."""
 
-        Examples
-        --------
-        >>> var_x = Expression.var('x')
-        >>> print(var_x)
-        x
-        """
+    COS: Expression
+    """The built-in cosine function."""
 
-    @classmethod
-    def vars(_cls, *names: str) -> Sequence[Expression]:
-        """
-        Create a Symbolica variable for every name in `*names`.
-        """
+    SIN: Expression
+    """The built-in sine function."""
+
+    EXP: Expression
+    """The built-in exponential function."""
+
+    LOG: Expression
+    """The built-in logarithm function."""
 
     @classmethod
-    def fun(_cls, name: str, is_symmetric: bool = False, is_antisymmetric: bool = False, is_linear: bool = False) -> Function:
+    def symbol(_cls, name: str, is_symmetric: Optional[bool] = None, is_antisymmetric: Optional[bool] = None, is_linear: Optional[bool] = None) -> Expression:
         """
-        Create a new Symbolica function with a given name.
+        Create a new symbol from a `name`. Symbols carry information about their attributes.
+        The symbol can signal that it is symmetric if it is used as a function
+        using `is_symmetric=True`, antisymmetric using `is_antisymmetric=True`, and
+        multilinear using `is_linear=True`. If no attributes
+        are specified, the attributes are inherited from the symbol if it was already defined,
+        otherwise all attributes are set to `false`.
+
+        Once attributes are defined on a symbol, they cannot be redefined later.
 
         Examples
         --------
-        >>> f = Expression.fun('f')
+        Define a regular symbol and use it as a variable:
+        >>> f = Expression.symbol('x')
+        >>> e = x**2 + 5
+        >>> print(e)
+        x**2 + 5
+
+        Define a regular symbol and use it as a function:
+        >>> f = Expression.symbol('f')
         >>> e = f(1,2)
         >>> print(e)
         f(1,2)
 
 
         Define a symmetric function:
-        >>> f = Expression.fun('f', is_symmetric=True)
+        >>> f = Expression.symbol('f', is_symmetric=True)
         >>> e = f(2,1)
         >>> print(e)
         f(1,2)
 
+
         Define a linear and symmetric function:
-        >>> p1, p2, p3, p4 = Expression.vars('p1', 'p2', 'p3', 'p4')
-        >>> dot = Expression.fun('dot', is_symmetric=True, is_linear=True)
+        >>> p1, p2, p3, p4 = Expression.symbols('p1', 'p2', 'p3', 'p4')
+        >>> dot = Expression.symbol('dot', is_symmetric=True, is_linear=True)
         >>> e = dot(p2+2*p3,p1+3*p2-p3)
         dot(p1,p2)+2*dot(p1,p3)+3*dot(p2,p2)-dot(p2,p3)+6*dot(p2,p3)-2*dot(p3,p3)
         """
 
     @classmethod
-    def funs(_cls, *names: str) -> Sequence[Function]:
+    def symbols(_cls, *names: str, is_symmetric: Optional[bool] = None, is_antisymmetric: Optional[bool] = None, is_linear: Optional[bool] = None) -> Sequence[Expression]:
+        """
+        Create a Symbolica symbol for every name in `*names`. See `Expression.symbol` for more information.
+
+        Examples
+        --------
+        >>> f, x = Expression.symbols('x', 'f')
+        >>> e = f(1,x)
+        >>> print(e)
+        f(1,x)
+        """
+
+    @overload
+    def __call__(self, *args: Expression | int) -> Expression:
+        """
+        Create a Symbolica expression or transformer by calling the function with appropriate arguments.
+
+        Examples
+        -------
+        >>> x, f = Expression.symbols('x', 'f')
+        >>> e = f(3,x)
+        >>> print(e)
+        f(3,x)
+        """
+
+    @overload
+    def __call__(self, *args: Transformer | Expression | int) -> Transformer:
         """
-        Create a Symbolica function for every name in `*names`.
+        Create a Symbolica expression or transformer by calling the function with appropriate arguments.
+
+        Examples
+        -------
+        >>> x, f = Expression.symbols('x', 'f')
+        >>> e = f(3,x)
+        >>> print(e)
+        f(3,x)
         """
 
     @classmethod
     def num(_cls, num: int | float, max_denom: Optional[int] = None) -> Expression:
         """Create a new Symbolica number from an int or a float.
         A floating point number is converted to its rational number equivalent,
         but it can also be truncated by specifying the maximal denominator value.
@@ -341,16 +386,16 @@
     def req_type(self, atom_type: AtomType) -> PatternRestriction:
         """
         Create a pattern restriction that tests the type of the atom.
 
         Examples
         --------
         >>> from symbolica import Expression, AtomType
-        >>> x, x_ = Expression.vars('x', 'x_')
-        >>> f = Expression.fun("f")
+        >>> x, x_ = Expression.symbols('x', 'x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(x)*f(2)*f(f(3))
         >>> e = e.replace_all(f(x_), 1, x_.req_type(AtomType.Num))
         >>> print(e)
 
         Yields `f(x)*f(1)`.
         """
 
@@ -367,16 +412,16 @@
         """
         Create a new pattern restriction that calls the function `filter_fn` with the matched
         atom that should return a boolean. If true, the pattern matches.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun("f")
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1)*f(2)*f(3)
         >>> e = e.replace_all(f(x_), 1, x_.req(lambda m: m == 2 or m == 3))
         """
 
     def req_cmp(
         self,
         other: Expression | int,
@@ -385,16 +430,16 @@
         """
         Create a new pattern restriction that calls the function `cmp_fn` with another the matched
         atom and the match atom of the `other` wildcard that should return a boolean. If true, the pattern matches.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_, y_ = Expression.vars('x_', 'y_')
-        >>> f = Expression.fun("f")
+        >>> x_, y_ = Expression.symbols('x_', 'y_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1)*f(2)*f(3)
         >>> e = e.replace_all(f(x_)*f(y_), 1, x_.req_cmp(y_, lambda m1, m2: m1 + m2 == 4))
         """
 
     def req_lt(self, num: Expression | int, cmp_any_atom=False) -> PatternRestriction:
         """Create a pattern restriction that passes when the wildcard is smaller than a number `num`.
         If the matched wildcard is not a number, the pattern fails.
@@ -402,16 +447,16 @@
         When the option `cmp_any_atom` is set to `True`, this function compares atoms
         of any type. The result depends on the internal ordering and may change between
         different Symbolica versions.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun("f")
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1)*f(2)*f(3)
         >>> e = e.replace_all(f(x_), 1, x_.req_lt(2))
         """
 
     def req_gt(self, num: Expression | int, cmp_any_atom=False) -> PatternRestriction:
         """Create a pattern restriction that passes when the wildcard is greater than a number `num`.
         If the matched wildcard is not a number, the pattern fails.
@@ -419,16 +464,16 @@
         When the option `cmp_any_atom` is set to `True`, this function compares atoms
         of any type. The result depends on the internal ordering and may change between
         different Symbolica versions.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun("f")
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1)*f(2)*f(3)
         >>> e = e.replace_all(f(x_), 1, x_.req_gt(2))
         """
 
     def req_le(self, num: Expression | int, cmp_any_atom=False) -> PatternRestriction:
         """Create a pattern restriction that passes when the wildcard is smaller than or equal to a number `num`.
         If the matched wildcard is not a number, the pattern fails.
@@ -436,16 +481,16 @@
         When the option `cmp_any_atom` is set to `True`, this function compares atoms
         of any type. The result depends on the internal ordering and may change between
         different Symbolica versions.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun("f")
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1)*f(2)*f(3)
         >>> e = e.replace_all(f(x_), 1, x_.req_le(2))
         """
 
     def req_ge(self, num: Expression | int, cmp_any_atom=False) -> PatternRestriction:
         """Create a pattern restriction that passes when the wildcard is greater than or equal to a number `num`.
         If the matched wildcard is not a number, the pattern fails.
@@ -453,16 +498,16 @@
         When the option `cmp_any_atom` is set to `True`, this function compares atoms
         of any type. The result depends on the internal ordering and may change between
         different Symbolica versions.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun("f")
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1)*f(2)*f(3)
         >>> e = e.replace_all(f(x_), 1, x_.req_ge(2))
         """
 
     def req_cmp_lt(self, num: Expression, cmp_any_atom=False) -> PatternRestriction:
         """Create a pattern restriction that passes when the wildcard is smaller than another wildcard.
         If the matched wildcards are not a numbers, the pattern fails.
@@ -470,16 +515,16 @@
         When the option `cmp_any_atom` is set to `True`, this function compares atoms
         of any type. The result depends on the internal ordering and may change between
         different Symbolica versions.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_, y_ = Expression.var('x_', 'y_')
-        >>> f = Expression.fun("f")
+        >>> x_, y_ = Expression.symbol('x_', 'y_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1,2)
         >>> e = e.replace_all(f(x_,y_), 1, x_.req_cmp_lt(y_))
         """
 
     def req_cmp_gt(self, num: Expression, cmp_any_atom=False) -> PatternRestriction:
         """Create a pattern restriction that passes when the wildcard is greater than another wildcard.
         If the matched wildcards are not a numbers, the pattern fails.
@@ -487,16 +532,16 @@
         When the option `cmp_any_atom` is set to `True`, this function compares atoms
         of any type. The result depends on the internal ordering and may change between
         different Symbolica versions.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_, y_ = Expression.var('x_', 'y_')
-        >>> f = Expression.fun("f")
+        >>> x_, y_ = Expression.symbol('x_', 'y_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1,2)
         >>> e = e.replace_all(f(x_,y_), 1, x_.req_cmp_gt(y_))
         """
 
     def req_cmp_le(self, num: Expression, cmp_any_atom=False) -> PatternRestriction:
         """Create a pattern restriction that passes when the wildcard is smaller than or equal to another wildcard.
         If the matched wildcards are not a numbers, the pattern fails.
@@ -504,16 +549,16 @@
         When the option `cmp_any_atom` is set to `True`, this function compares atoms
         of any type. The result depends on the internal ordering and may change between
         different Symbolica versions.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_, y_ = Expression.var('x_', 'y_')
-        >>> f = Expression.fun("f")
+        >>> x_, y_ = Expression.symbol('x_', 'y_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1,2)
         >>> e = e.replace_all(f(x_,y_), 1, x_.req_cmp_le(y_))
         """
 
     def req_cmp_ge(self, num: Expression, cmp_any_atom=False) -> PatternRestriction:
         """Create a pattern restriction that passes when the wildcard is greater than or equal to another wildcard.
         If the matched wildcards are not a numbers, the pattern fails.
@@ -521,16 +566,16 @@
         When the option `cmp_any_atom` is set to `True`, this function compares atoms
         of any type. The result depends on the internal ordering and may change between
         different Symbolica versions.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_, y_ = Expression.var('x_', 'y_')
-        >>> f = Expression.fun("f")
+        >>> x_, y_ = Expression.symbol('x_', 'y_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1,2)
         >>> e = e.replace_all(f(x_,y_), 1, x_.req_cmp_ge(y_))
         """
 
     def __eq__(self, other: Expression | int) -> bool:
         """
         Compare two expressions.
@@ -580,15 +625,15 @@
 
         No new functions or variables can be defined and no new
         expressions can be parsed inside the map. Doing so will
         result in a deadlock.
 
         Examples
         --------
-        >>> x, x_ = Expression.vars('x', 'x_')
+        >>> x, x_ = Expression.symbols('x', 'x_')
         >>> e = (1+x)**2
         >>> r = e.map(Transformer().expand().replace_all(x, 6))
         >>> print(r)
         """
 
     def set_coefficient_ring(self, vars: Sequence[Expression]) -> Expression:
         """
@@ -597,17 +642,17 @@
 
         Parameters
         ----------
         vars : Sequence[Expression]
                 A list of variables
         """
 
-    def expand(self) -> Expression:
+    def expand(self, var: Optional[Expression] = None) -> Expression:
         """
-        Expand the expression.
+        Expand the expression. Optionally, expand in `var` only.
         """
 
     def collect(
         self,
         x: Expression,
         key_map: Optional[Callable[[Expression], Expression]] = None,
         coeff_map: Optional[Callable[[Expression], Expression]] = None,
@@ -618,23 +663,23 @@
 
         Both the key (the quantity collected in) and its coefficient can be mapped using
         `key_map` and `coeff_map` respectively.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x, y = Expression.vars('x', 'y')
+        >>> x, y = Expression.symbols('x', 'y')
         >>> e = 5*x + x * y + x**2 + 5
         >>>
         >>> print(e.collect(x))
 
         yields `x^2+x*(y+5)+5`.
 
         >>> from symbolica import Expression
-        >>> x, y = Expression.vars('x', 'y')
+        >>> x, y = Expression.symbols('x', 'y')
         >>> var, coeff = Expression.funs('var', 'coeff')
         >>> e = 5*x + x * y + x**2 + 5
         >>>
         >>> print(e.collect(x, key_map=lambda x: var(x), coeff_map=lambda x: coeff(x)))
 
         yields `var(1)*coeff(5)+var(x)*coeff(y+5)+var(x^2)*coeff(1)`.
 
@@ -650,15 +695,15 @@
         """Collect terms involving the same power of `x`, where `x` is a variable or function name.
         Return the list of key-coefficient pairs and the remainder that matched no key.
 
         Examples
         --------
 
         >>> from symbolica import *
-        >>> x, y = Expression.vars('x', 'y')
+        >>> x, y = Expression.symbols('x', 'y')
         >>> e = 5*x + x * y + x**2 + 5
         >>>
         >>> for a in e.coefficient_list(x):
         >>>     print(a[0], a[1])
 
         yields
         ```
@@ -671,44 +716,45 @@
     def coefficient(self, x: Expression) -> Expression:
         """Collect terms involving the literal occurrence of `x`.
 
         Examples
         --------
 
         >>> from symbolica import *
-        >>> x, y = Expression.vars('x', 'y')
+        >>> x, y = Expression.symbols('x', 'y')
         >>> e = 5*x + x * y + x**2 + y*x**2
         >>> print(e.coefficient(x**2))
 
         yields
 
         ```
         y + 1
         ```
         """
 
     def derivative(self, x: Expression) -> Expression:
         """Derive the expression w.r.t the variable `x`."""
 
-    def taylor_series(
+    def series(
         self,
         x: Expression,
         expansion_point: Expression | int,
         depth: int,
-    ) -> Expression:
-        """Taylor expand in `x` around `expansion_point` to depth `depth`."""
+        depth_denom: int = 1,
+    ) -> Series:
+        """Series expand in `x` around `expansion_point` to depth `depth`."""
 
     def apart(self, x: Expression) -> Expression:
         """Compute the partial fraction decomposition in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('1/((x+y)*(x^2+x*y+1)(x+1))')
         >>> print(p.apart(x))
         """
 
     def together(self) -> Expression:
         """Write the expression over a common denominator.
 
@@ -762,16 +808,16 @@
         The `level_range` specifies the `[min,max]` level at which the pattern is allowed to match.
         The first level is 0 and the level is increased when going into a function or one level deeper in the expression tree,
         depending on `level_is_tree_depth`.
 
         Examples
         --------
 
-        >>> x, x_ = Expression.vars('x','x_')
-        >>> f = Expression.fun('f')
+        >>> x, x_ = Expression.symbols('x','x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(x)*f(1)*f(2)*f(3)
         >>> for match in e.match(f(x_)):
         >>>    for map in match:
         >>>        print(map[0],'=', map[1])
         """
 
     def replace(
@@ -786,16 +832,16 @@
         Return an iterator over the replacement of the pattern `self` on `lhs` by `rhs`.
         Restrictions on pattern can be supplied through `cond`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun('f')
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(1)*f(2)*f(3)
         >>> for r in e.replace(f(x_), f(x_ + 1)):
         >>>     print(r)
 
         Yields:
         ```
         f(2)*f(2)*f(3)
@@ -824,16 +870,16 @@
     ) -> Expression:
         """
         Replace all subexpressions matching the pattern `pattern` by the right-hand side `rhs`.
 
         Examples
         --------
 
-        >>> x, w1_, w2_ = Expression.vars('x','w1_','w2_')
-        >>> f = Expression.fun('f')
+        >>> x, w1_, w2_ = Expression.symbols('x','w1_','w2_')
+        >>> f = Expression.symbol('f')
         >>> e = f(3,x)
         >>> r = e.replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2), (w1_ >= 1) & w2_.is_var())
         >>> print(r)
 
         Parameters
         ----------
         self: The expression to match and replace on.
@@ -854,45 +900,45 @@
     ) -> Sequence[Expression]:
         """Solve a linear system in the variables `variables`, where each expression
         in the system is understood to yield 0.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x, y, c = Expression.vars('x', 'y', 'c')
-        >>> f = Expression.fun('f')
+        >>> x, y, c = Expression.symbols('x', 'y', 'c')
+        >>> f = Expression.symbol('f')
         >>> x_r, y_r = Expression.solve_linear_system([f(c)*x + y/c - 1, y-c/2], [x, y])
         >>> print('x =', x_r, ', y =', y_r)
         """
 
     def evaluate(
-        self, constants: dict[Expression, float], funs: dict[Expression | Function, Callable[[Sequence[float]], float]]
+        self, constants: dict[Expression, float], funs: dict[Expression, Callable[[Sequence[float]], float]]
     ) -> float:
         """Evaluate the expression, using a map of all the variables and
         user functions to a float.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
-        >>> f = Expression.fun('f')
+        >>> x = Expression.symbol('x')
+        >>> f = Expression.symbol('f')
         >>> e = Expression.parse('cos(x)')*3 + f(x,2)
         >>> print(e.evaluate({x: 1}, {f: lambda args: args[0]+args[1]}))
         """
 
     def evaluate_complex(
-        self, constants: dict[Expression, float | complex], funs: dict[Expression | Function, Callable[[Sequence[complex]], float | complex]]
+        self, constants: dict[Expression, float | complex], funs: dict[Expression, Callable[[Sequence[complex]], float | complex]]
     ) -> complex:
         """Evaluate the expression, using a map of all the variables and
         user functions to a complex number.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x, y = Expression.vars('x', 'y')
+        >>> x, y = Expression.symbols('x', 'y')
         >>> e = Expression.parse('sqrt(x)')*y
         >>> print(e.evaluate_complex({x: 1 + 2j, y: 4 + 3j}, {}))
         """
 
 
 class PatternRestriction:
     """A restriction on wildcards."""
@@ -907,111 +953,52 @@
         """Create a new pattern restriction that takes the logical 'not' of the current restriction."""
 
 
 class CompareOp:
     """One of the following comparison operators: `<`,`>`,`<=`,`>=`,`==`,`!=`."""
 
 
-class Function:
-    """A Symbolica function. Will turn into an expression or a transformer when called with arguments."""
-
-    COEFF: Function
-    """The built-in function that convert a rational polynomials to a coefficient."""
-
-    COS: Function
-    """The built-in cosine function."""
-
-    SIN: Function
-    """The built-in sine function."""
-
-    EXP: Function
-    """The built-in exponential function."""
-
-    LOG: Function
-    """The built-in logarithm function."""
-
-    def __new__(_cls, name: str, is_symmetric: Optional[bool], is_antisymmetric: Optional[bool], is_linear: Optional[bool]) -> Function:
-        """
-        Create a new function from a `name`. Can be turned into a symmetric function
-        using `is_symmetric=True` or into an antisymmetric function using `is_antisymmetric=True`.
-        The function can be made multilinear using `is_linear=True`.
-
-        Once attributes are defined on a function, they cannot be redefined later.
-        """
-
-    def is_symmetric(self) -> bool:
-        """Returns `True` iff this function is symmetric."""
-
-    @overload
-    def __call__(self, *args: Expression | int) -> Expression:
-        """
-        Create a Symbolica expression or transformer by calling the function with appropriate arguments.
-
-        Examples
-        -------
-        >>> x = Expression.vars('x')
-        >>> f = Expression.fun('f')
-        >>> e = f(3,x)
-        >>> print(e)
-        f(3,x)
-        """
-
-    @overload
-    def __call__(self, *args: Transformer | Expression | int) -> Transformer:
-        """
-        Create a Symbolica expression or transformer by calling the function with appropriate arguments.
-
-        Examples
-        -------
-        >>> x = Expression.vars('x')
-        >>> f = Expression.fun('f')
-        >>> e = f(3,x)
-        >>> print(e)
-        f(3,x)
-        """
-
-
 class Transformer:
     """Operations that transform an expression."""
 
     def __new__(_cls) -> Transformer:
         """Create a new transformer for a term provided by `Expression.map`."""
 
-    def expand(self) -> Transformer:
+    def expand(self, var: Optional[Expression] = None) -> Transformer:
         """Create a transformer that expands products and powers.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x, x_ = Expression.vars('x', 'x_')
-        >>> f = Expression.fun('f')
+        >>> x, x_ = Expression.symbols('x', 'x_')
+        >>> f = Expression.symbol('f')
         >>> e = f((x+1)**2).replace_all(f(x_), x_.transform().expand())
         >>> print(e)
         """
 
     def prod(self) -> Transformer:
         """Create a transformer that computes the product of a list of arguments.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x__ = Expression.var('x__')
-        >>> f = Expression.fun('f')
+        >>> x__ = Expression.symbol('x__')
+        >>> f = Expression.symbol('f')
         >>> e = f(2,3).replace_all(f(x__), x__.transform().prod())
         >>> print(e)
         """
 
     def sum(self) -> Transformer:
         """Create a transformer that computes the sum of a list of arguments.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x__ = Expression.var('x__')
-        >>> f = Expression.fun('f')
+        >>> x__ = Expression.symbol('x__')
+        >>> f = Expression.symbol('f')
         >>> e = f(2,3).replace_all(f(x__), x__.transform().sum())
         >>> print(e)
         """
 
     def nargs(self, only_for_arg_fun: bool = False) -> Transformer:
         """Create a transformer that returns the number of arguments.
         If the argument is not a function, return 0.
@@ -1019,41 +1006,41 @@
         If `only_for_arg_fun` is `True`, only count the number of arguments
         in the `arg()` function and return 1 if the input is not `arg`.
         This is useful for obtaining the length of a range during pattern matching.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x__ = Expression.var('x__')
-        >>> f = Expression.fun('f')
+        >>> x__ = Expression.symbol('x__')
+        >>> f = Expression.symbol('f')
         >>> e = f(2,3,4).replace_all(f(x__), x__.transform().nargs())
         >>> print(e)
         """
 
     def sort(self) -> Transformer:
         """Create a transformer that sorts a list of arguments.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x__ = Expression.var('x__')
-        >>> f = Expression.fun('f')
+        >>> x__ = Expression.symbol('x__')
+        >>> f = Expression.symbol('f')
         >>> e = f(3,2,1).replace_all(f(x__), x__.transform().sort())
         >>> print(e)
         """
 
     def deduplicate(self) -> Transformer:
         """Create a transformer that removes elements from a list if they occur
         earlier in the list as well.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x__ = Expression.var('x__')
-        >>> f = Expression.fun('f')
+        >>> x__ = Expression.symbol('x__')
+        >>> f = Expression.symbol('f')
         >>> e = f(1,2,1,2).replace_all(f(x__), x__.transform().deduplicate())
         >>> print(e)
 
         Yields `f(1,2)`.
         """
 
     def from_coeff(self) -> Transformer:
@@ -1068,16 +1055,16 @@
 
     def split(self) -> Transformer:
         """Create a transformer that split a sum or product into a list of arguments.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x, x__ = Expression.vars('x', 'x__')
-        >>> f = Expression.fun('f')
+        >>> x, x__ = Expression.symbols('x', 'x__')
+        >>> f = Expression.symbol('f')
         >>> e = (x + 1).replace_all(x__, f(x_.transform().split()))
         >>> print(e)
         """
 
     def partitions(
         self,
         bins: Sequence[Tuple[Transformer | Expression, int]],
@@ -1094,16 +1081,16 @@
         if possible.
 
         Note that the functions names to be provided for the bin names must be generated through `Expression.var`.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x_, f_id, g_id = Expression.vars('x_', 'f', 'g')
-        >>> f = Expression.fun('f')
+        >>> x_, f_id, g_id = Expression.symbols('x__', 'f', 'g')
+        >>> f = Expression.symbol('f')
         >>> e = f(1,2,1,3).replace_all(f(x_), x_.transform().partitions([(f_id, 2), (g_id, 1), (f_id, 1)]))
         >>> print(e)
 
         yields:
         ```
         2*f(1)*f(1,2)*g(3)+2*f(1)*f(1,3)*g(2)+2*f(1)*f(2,3)*g(1)+f(2)*f(1,1)*g(3)+2*f(2)*f(1,3)*g(1)+f(3)*f(1,1)*g(2)+2*f(3)*f(1,2)*g(1)
         ```
@@ -1111,16 +1098,16 @@
 
     def permutations(self, function_name: Transformer | Expression) -> Transformer:
         """Create a transformer that generates all permutations of a list of arguments.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x_, f_id = Expression.vars('x_', 'f')
-        >>> f = Expression.fun('f')
+        >>> x_, f_id = Expression.symbols('x__', 'f')
+        >>> f = Expression.symbol('f')
         >>> e = f(1,2,1,2).replace_all(f(x_), x_.transform().permutations(f_id)
         >>> print(e)
 
         yields:
         ```
         4*f(1,1,2,2)+4*f(1,2,1,2)+4*f(1,2,2,1)+4*f(2,1,1,2)+4*f(2,1,2,1)+4*f(2,2,1,1)
         ```
@@ -1128,109 +1115,110 @@
 
     def map(self, f: Callable[[Expression], Expression | int]) -> Transformer:
         """Create a transformer that applies a Python function.
 
         Examples
         --------
         >>> from symbolica import Expression, Transformer
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun('f')
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = f(2).replace_all(f(x_), x_.transform().map(lambda r: r**2))
         >>> print(e)
         """
 
     def for_each(self, *transformers: Transformer) -> Transformer:
         """Create a transformer that applies a transformer chain to every argument of the `arg()` function.
         If the input is not `arg()`, the transformer is applied to the input.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
-        >>> f = Expression.fun('f')
+        >>> x = Expression.symbol('x')
+        >>> f = Expression.symbol('f')
         >>> e = (1+x).transform().split().for_each(Transformer().map(f)).execute()
         """
 
     def check_interrupt(self) -> Transformer:
         """Create a transformer that checks for a Python interrupt,
         such as ctrl-c and aborts the current transformer.
 
         Examples
         --------
         >>> from symbolica import *
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun('f')
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> f(10).transform().repeat(Transformer().replace_all(
         >>> f(x_), f(x_+1)).check_interrupt()).execute()
         """
 
     def repeat(self, *transformers: Transformer) -> Transformer:
         """Create a transformer that repeatedly executes the arguments in order
         until there are no more changes.
         The output from one transformer is inserted into the next.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun('f')
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = Expression.parse("f(5)")
         >>> e = e.transform().repeat(
         >>>     Transformer().expand(),
         >>>     Transformer().replace_all(f(x_), f(x_ - 1) + f(x_ - 2), x_.req_gt(1))
         >>> ).execute()
         """
 
     def chain(self, *transformers: Transformer) -> Transformer:
         """Chain several transformers. `chain(A,B,C)` is the same as `A.B.C`,
         where `A`, `B`, `C` are transformers.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun('f')
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = Expression.parse("f(5)")
         >>> e = e.transform().chain(
         >>>     Transformer().expand(),
         >>>     Transformer().replace_all(f(x_), f(5))
         >>> ).execute()
         """
 
     def execute(self) -> Expression:
         """Execute the transformer.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> e = (x+1)**5
         >>> e = e.transform().expand().execute()
         >>> print(e)
         """
 
     def derivative(self, x: Transformer | Expression) -> Transformer:
         """Create a transformer that derives `self` w.r.t the variable `x`."""
 
-    def taylor_series(
+    def series(
         self,
         x: Expression,
         expansion_point: Expression,
         depth: int,
-    ) -> Expression:
-        """Create a transformer that Taylor expands in `x` around `expansion_point` to depth `depth`.
+        depth_denom: int = 1,
+    ) -> Transformer:
+        """Create a transformer that series expands in `x` around `expansion_point` to depth `depth`.
 
-        Example
+        Examples
         -------
         >>> from symbolica import Expression
-        >>> x, y = Expression.vars('x', 'y')
-        >>> f = Expression.fun('f')
+        >>> x, y = Expression.symbols('x', 'y')
+        >>> f = Expression.symbol('f')
         >>>
         >>> e = 2* x**2 * y + f(x)
-        >>> e = e.taylor_series(x, 0, 2)
+        >>> e = e.series(x, 0, 2)
         >>>
         >>> print(e)
 
         yields `f(0)+x*der(1,f(0))+1/2*x^2*(der(2,f(0))+4*y)`.
         """
 
     def replace_all(
@@ -1244,16 +1232,16 @@
     ) -> Transformer:
         """
         Create a transformer that replaces all subexpressions matching the pattern `pat` by the right-hand side `rhs`.
 
         Examples
         --------
 
-        >>> x, w1_, w2_ = Expression.vars('x','w1_','w2_')
-        >>> f = Expression.fun('f')
+        >>> x, w1_, w2_ = Expression.symbols('x','w1_','w2_')
+        >>> f = Expression.symbol('f')
         >>> e = f(3,x)
         >>> r = e.transform().replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2), (w1_ >= 1) & w2_.is_var())
         >>> print(r)
 
         Parameters
         ----------
         pat: The pattern to match.
@@ -1296,16 +1284,16 @@
     ) -> Transformer:
         """
         Print statistics of a transformer, tagging it with `tag`.
 
         Examples
         --------
         >>> from symbolica import Expression
-        >>> x_ = Expression.var('x_')
-        >>> f = Expression.fun('f')
+        >>> x_ = Expression.symbol('x_')
+        >>> f = Expression.symbol('f')
         >>> e = Expression.parse("f(5)")
         >>> e = e.transform().stats('replace', Transformer().replace_all(f(x_), 1)).execute()
 
         yields
         ```log
         Stats for replace:
             In  │ 1 │  10.00 B │
@@ -1375,14 +1363,98 @@
 
     def __neg__(self) -> Transformer:
         """
         Negate the current transformer, returning the result.
         """
 
 
+class Series:
+    """
+    A series expansion class.
+
+    Supports standard arithmetic operations, such
+    as addition and multiplication.
+
+    Examples
+    --------
+    >>> x = Expression.symbol('x')
+    >>> s = Expression.parse("(1-cos(x))/sin(x)").series(x, 0, 4)
+    >>> print(s)
+    """
+
+    def __add__(self, other: Series) -> Series:
+        """Add two series together, returning the result."""
+
+    def __sub__(self, other: Series) -> Series:
+        """Subtract `other` from `self`, returning the result."""
+
+    def __mul__(self, other: Series) -> Series:
+        """Multiply two series together, returning the result."""
+
+    def __truediv__(self, other: Series) -> Series:
+        """Divide `self` by `other`, returning the result."""
+
+    def __pow__(self, exp: int) -> Series:
+        """Raise the series to the power of `exp`, returning the result."""
+
+    def __neg__(self) -> Series:
+        """Negate the series."""
+
+    def sin(self) -> Series:
+        """Compute the sine of the series, returning the result."""
+
+    def cos(self) -> Series:
+        """Compute the cosine of the series, returning the result."""
+
+    def exp(self) -> Series:
+        """Compute the exponential of the series, returning the result."""
+
+    def log(self) -> Series:
+        """Compute the natural logarithm of the series, returning the result."""
+
+    def pow(self, num: int, den: int) -> Series:
+        """Raise the series to the power of `num/den`, returning the result."""
+
+    def spow(self, exp: Series) -> Series:
+        """Raise the series to the power of `exp`, returning the result."""
+
+    def to_expression(self) -> Expression:
+        """Convert the term stream into an expression. This may exceed the available memory."""
+
+
+class TermStreamer:
+    def __new__(_cls, path: Optional[str] = None,
+                max_mem_bytes: Optional[int] = None,
+                n_cores: Optional[int] = None) -> TermStreamer:
+        """Create a new term streamer with a given path for its files,
+           the maximum size of the memory buffer and the number of cores.
+        """
+
+    def __add__(self, other: TermStreamer) -> TermStreamer:
+        """Add two term streamers together, returning the result."""
+
+    def __iadd__(self, other: TermStreamer) -> None:
+        """Add another term streamer to this one."""
+
+    def get_byte_size(self) -> int:
+        """Get the byte size of the term streamer."""
+
+    def push(self, expr: Expression) -> None:
+        """Push an expresssion to the term streamer."""
+
+    def normalize(self) -> None:
+        """Sort and fuse all terms in the streamer."""
+
+    def to_expression(self) -> Expression:
+        """Convert the term stream into an expression. This may exceed the available memory."""
+
+    def map(self, f: Transformer) -> TermStreamer:
+        """Apply a transformer to all terms in the streamer."""
+
+
 class MatchIterator:
     """An iterator over matches."""
 
     def __iter__(self) -> MatchIterator:
         """Create the iterator."""
 
     def __next__(self) -> dict[Expression, Expression]:
@@ -1529,27 +1601,27 @@
     def derivative(self, x: Expression) -> Polynomial:
         """Take a derivative in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x^2+2').to_polynomial()
         >>> print(p.derivative(x))
         """
 
     def integrate(self, x: Expression) -> Polynomial:
         """Integrate the polynomial in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x^2+2').to_polynomial()
         >>> print(p.integrate(x))
         """
 
     def content(self) -> Polynomial:
         """Get the content, i.e., the GCD of the coefficients.
 
@@ -1564,15 +1636,15 @@
     def coefficient_list(self, x: Expression) -> list[Tuple[int, Polynomial]]:
         """Get the coefficient list in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
         >>> for n, pp in p.coefficient_list(x):
         >>>     print(n, pp)
         """
 
     @classmethod
     def groebner_basis(_cls, system: list[Polynomial], grevlex: bool = True, print_stats: bool = False) -> list[Polynomial]:
@@ -1612,15 +1684,15 @@
     def replace(self, x: Expression, v: Polynomial) -> Polynomial:
         """Replace the variable `x` with a polynomial `v`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
         >>> r = Expression.parse('y+1').to_polynomial())
         >>> p.replace(x, r)
         """
 
 
 class IntegerPolynomial:
@@ -1741,15 +1813,15 @@
     def derivative(self, x: Expression) -> IntegerPolynomial:
         """Take a derivative in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x^2+2').to_polynomial().to_integer_polynomial()
         >>> print(p.derivative(x))
         """
 
     def content(self) -> IntegerPolynomial:
         """Get the content, i.e., the GCD of the coefficients.
 
@@ -1764,15 +1836,15 @@
     def coefficient_list(self, x: Expression) -> list[Tuple[int, IntegerPolynomial]]:
         """Get the coefficient list in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial().to_integer_polynomial()
         >>> for n, pp in p.coefficient_list(x):
         >>>     print(n, pp)
         """
 
     def to_expression(self) -> Expression:
         """ Convert the polynomial to an expression.
@@ -1789,15 +1861,15 @@
     def replace(self, x: Expression, v: Polynomial) -> Polynomial:
         """Replace the variable `x` with a polynomial `v`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
         >>> r = Expression.parse('y+1').to_polynomial())
         >>> p.replace(x, r)
         """
 
 
 class FiniteFieldPolynomial:
@@ -1926,27 +1998,27 @@
     def derivative(self, x: Expression) -> FiniteFieldPolynomial:
         """Take a derivative in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x^2+2').to_polynomial()
         >>> print(p.derivative(x))
         """
 
     def integrate(self, x: Expression) -> FiniteFieldPolynomial:
         """Integrate the polynomial in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x^2+2').to_polynomial()
         >>> print(p.integrate(x))
         """
 
     def content(self) -> FiniteFieldPolynomial:
         """Get the content, i.e., the GCD of the coefficients.
 
@@ -1961,15 +2033,15 @@
     def coefficient_list(self, x: Expression) -> list[Tuple[int, FiniteFieldPolynomial]]:
         """Get the coefficient list in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
         >>> for n, pp in p.coefficient_list(x):
         >>>     print(n, pp)
         """
 
     @classmethod
     def groebner_basis(_cls, system: list[FiniteFieldPolynomial], grevlex: bool = True, print_stats: bool = False) -> list[FiniteFieldPolynomial]:
@@ -1997,15 +2069,15 @@
     def replace(self, x: Expression, v: Polynomial) -> Polynomial:
         """Replace the variable `x` with a polynomial `v`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
         >>> r = Expression.parse('y+1').to_polynomial())
         >>> p.replace(x, r)
         """
 
 
 class RationalPolynomial:
@@ -2086,15 +2158,15 @@
     def apart(self, x: Expression) -> List[RationalPolynomial]:
         """Compute the partial fraction decomposition in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('1/((x+y)*(x^2+x*y+1)(x+1))').to_rational_polynomial()
         >>> for pp in p.apart(x):
         >>>     print(pp)
         """
 
 
 class RationalPolynomialSmallExponent:
@@ -2173,15 +2245,15 @@
     def apart(self, x: Expression) -> List[RationalPolynomialSmallExponent]:
         """Compute the partial fraction decomposition in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('1/((x+y)*(x^2+x*y+1)(x+1))').to_rational_polynomial()
         >>> for pp in p.apart(x):
         >>>     print(pp)
         """
 
 
 class FiniteFieldRationalPolynomial:
@@ -2241,15 +2313,15 @@
     def apart(self, x: Expression) -> List[FiniteFieldRationalPolynomial]:
         """Compute the partial fraction decomposition in `x`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
-        >>> x = Expression.var('x')
+        >>> x = Expression.symbol('x')
         >>> p = Expression.parse('1/((x+y)*(x^2+x*y+1)(x+1))').to_rational_polynomial()
         >>> for pp in p.apart(x):
         >>>     print(pp)
         """
 
 
 class Matrix:
```

### Comparing `symbolica-0.4.0/tests/pattern_matching.rs` & `symbolica-0.5.0/tests/pattern_matching.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/tests/rational_polynomial.rs` & `symbolica-0.5.0/tests/rational_polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.4.0/pyproject.toml` & `symbolica-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 summary = "Symbolica is a blazing fast computer algebra system"
 description = "Symbolica is a blazing fast computer algebra system"
 keywords = ["math", "algebra", "polynomial", "expression", "manipulation"]
 license = {file = "License.md"}
 name = "symbolica"
 readme = "Readme.md"
-version = "0.4.0"
+version = "0.5.0"
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Rust",
   "Topic :: Scientific/Engineering :: Mathematics",
 ]
```

### Comparing `symbolica-0.4.0/PKG-INFO` & `symbolica-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: symbolica
-Version: 0.4.0
+Version: 0.5.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 License-File: License.md
 License-File: License.md
 Summary: Symbolica is a blazing fast computer algebra system
 Keywords: math,algebra,polynomial,expression,manipulation
@@ -62,15 +62,15 @@
 
 ## Rust
 
 If you want to use Symbolica as a library in Rust, simply include it in the `Cargo.toml`:
 
 ```toml
 [dependencies]
-symbolica = "0.4"
+symbolica = "0.5"
 ```
 
 # Examples
 
 Below we list some examples of the features of Symbolica. Check the [guide](https://symbolica.io/docs/) for a complete overview.
 
 ### Pattern matching
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: symbolica Version: 0.4.0 Classifier: Development
+Metadata-Version: 2.3 Name: symbolica Version: 0.5.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Programming Language :: Rust Classifier: Topic
 :: Scientific/Engineering :: Mathematics License-File: License.md License-File:
 License.md Summary: Symbolica is a blazing fast computer algebra system
 Keywords: math,algebra,polynomial,expression,manipulation Author: Ben Ruijl
 Author-email: benruyl@gmail.com Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: homepage, https://symbolica.io Project-
 URL: repository, https://github.com/benruijl/symbolica
@@ -22,15 +22,15 @@
 (probably) already know, by using Symbolica's bindings to Python, Rust and C++:
 [A demo of Symbolica]# Installation Visit the [Get Started](https://
 symbolica.io/docs/get_started.html) page for detailed installation
 instructions. ## Python Symbolica can be installed for Python >3.5 using `pip`:
 ```sh pip install symbolica ``` The installation may take some time on Mac OS
 and Windows, as it may have to compile Symbolica. ## Rust If you want to use
 Symbolica as a library in Rust, simply include it in the `Cargo.toml`: ```toml
-[dependencies] symbolica = "0.4" ``` # Examples Below we list some examples of
+[dependencies] symbolica = "0.5" ``` # Examples Below we list some examples of
 the features of Symbolica. Check the [guide](https://symbolica.io/docs/) for a
 complete overview. ### Pattern matching Variables ending with a `_` are
 wildcards that match to any subexpression. In the following example we try to
 match the pattern `f(w1_,w2_)`: ```python from symbolica import Expression x,
 y, w1_, w2_ = Expression.vars('x','y','w1_','w2_') f = Expression.fun('f') e =
 f(3,x)*y**2+5 r = e.replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2)) print(r) ```
 which yields `y^2*f(2,x^2)+5`. ### Solving a linear system Solve a linear
```

