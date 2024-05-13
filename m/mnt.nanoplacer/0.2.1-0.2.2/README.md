# Comparing `tmp/mnt.nanoplacer-0.2.1.tar.gz` & `tmp/mnt_nanoplacer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnt.nanoplacer-0.2.1.tar", last modified: Thu Jan 18 16:52:07 2024, max compression
+gzip compressed data, was "mnt_nanoplacer-0.2.2.tar", last modified: Mon May 13 09:45:59 2024, max compression
```

## Comparing `mnt.nanoplacer-0.2.1.tar` & `mnt_nanoplacer-0.2.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.547186 mnt.nanoplacer-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.499186 mnt.nanoplacer-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.499186 mnt.nanoplacer-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-01-18 16:52:07.543186 mnt.nanoplacer-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.495186 mnt.nanoplacer-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.503186 mnt.nanoplacer-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    70113 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/docs/_static/lbr.png
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/docs/_static/mnt_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/docs/_static/mnt_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 16:52:07.547186 mnt.nanoplacer-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.499186 mnt.nanoplacer-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.503186 mnt.nanoplacer-0.2.1/src/mnt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.503186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.499186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.531186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/
--rw-r--r--   0 runner    (1001) docker     (127)    44749 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/adder.v
--rw-r--r--   0 runner    (1001) docker     (127)   491036 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/arbiter.v
--rw-r--r--   0 runner    (1001) docker     (127)   139420 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/bar.v
--rw-r--r--   0 runner    (1001) docker     (127)    30030 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/cavlc.v
--rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/ctrl.v
--rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/dec.v
--rw-r--r--   0 runner    (1001) docker     (127)  2537203 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/div.v
--rw-r--r--   0 runner    (1001) docker     (127) 10153688 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/hyp.v
--rw-r--r--   0 runner    (1001) docker     (127)    54911 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/i2c.v
--rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/int2float.v
--rw-r--r--   0 runner    (1001) docker     (127)  1372592 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/log2.v
--rw-r--r--   0 runner    (1001) docker     (127)   132676 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/max.v
--rw-r--r--   0 runner    (1001) docker     (127)  1158136 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/multiplier.v
--rw-r--r--   0 runner    (1001) docker     (127)    38989 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/priority.v
--rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/router.v
--rw-r--r--   0 runner    (1001) docker     (127)   214688 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/sin.v
--rw-r--r--   0 runner    (1001) docker     (127)  1087553 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/sqrt.v
--rw-r--r--   0 runner    (1001) docker     (127)   783980 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/square.v
--rw-r--r--   0 runner    (1001) docker     (127)   600136 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/voter.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.535186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/
--rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c1355.v
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c17.v
--rw-r--r--   0 runner    (1001) docker     (127)    15006 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c1908.v
--rw-r--r--   0 runner    (1001) docker     (127)    29248 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c2670.v
--rw-r--r--   0 runner    (1001) docker     (127)    37970 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c3540.v
--rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c432.v
--rw-r--r--   0 runner    (1001) docker     (127)    14628 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c499.v
--rw-r--r--   0 runner    (1001) docker     (127)    70010 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c5315.v
--rw-r--r--   0 runner    (1001) docker     (127)    91913 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c6288.v
--rw-r--r--   0 runner    (1001) docker     (127)    83840 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c7552.v
--rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c880.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.539186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/
--rwxr-xr-x   0 runner    (1001) docker     (127)      222 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/1bitAdderAOIG.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/1bitAdderMaj.v
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/FA.v
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/FS.v
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/HA.v
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/HS.v
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/RCA2.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/b1_r2.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/clpl.v
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/mux21.v
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/mux41.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/newtag.v
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/par_check.v
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/par_gen.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/t.v
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/xnor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/xor2.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      560 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/xor5R.v
--rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/xor5_r1.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.539186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderAOIG.v
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderMaj.v
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/2bitAdderMaj.v
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/b1_r2.v
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/c17.v
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/clpl.v
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/cm82a_5.v
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/majority.v
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/majority_5_r1.v
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/newtag.v
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/parity.v
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/t.v
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/t_5.v
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/xor.v
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/xor5Maj.v
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/xor5_r1.v
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.543186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/trindade16/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/trindade16/FA.v
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/trindade16/HA.v
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/trindade16/mux21.v
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/trindade16/par_check.v
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/trindade16/par_gen.v
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/trindade16/xnor2.v
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/trindade16/xor2.v
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.543186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23902 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/nano_placement_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.543186 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/utils/layout_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/utils/placement_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.543186 mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-01-18 16:52:07.000000 mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-01-18 16:52:07.000000 mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 16:52:07.000000 mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-18 16:52:07.000000 mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-18 16:52:07.000000 mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-18 16:52:07.000000 mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:52:07.543186 mnt.nanoplacer-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-01-18 16:51:58.000000 mnt.nanoplacer-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9590 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.369051 mnt_nanoplacer-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    70113 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/docs/_static/lbr.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/docs/_static/mnt_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/docs/_static/mnt_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:45:59.413051 mnt_nanoplacer-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.369051 mnt_nanoplacer-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/src/mnt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.373051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.369051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.397051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/
+-rw-r--r--   0 runner    (1001) docker     (127)    44749 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/adder.v
+-rw-r--r--   0 runner    (1001) docker     (127)   491036 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/arbiter.v
+-rw-r--r--   0 runner    (1001) docker     (127)   139420 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/bar.v
+-rw-r--r--   0 runner    (1001) docker     (127)    30030 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/cavlc.v
+-rw-r--r--   0 runner    (1001) docker     (127)     7607 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/ctrl.v
+-rw-r--r--   0 runner    (1001) docker     (127)    19319 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/dec.v
+-rw-r--r--   0 runner    (1001) docker     (127)  2537203 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/div.v
+-rw-r--r--   0 runner    (1001) docker     (127) 10153688 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/hyp.v
+-rw-r--r--   0 runner    (1001) docker     (127)    54911 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/i2c.v
+-rw-r--r--   0 runner    (1001) docker     (127)     9468 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/int2float.v
+-rw-r--r--   0 runner    (1001) docker     (127)  1372592 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/log2.v
+-rw-r--r--   0 runner    (1001) docker     (127)   132676 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/max.v
+-rw-r--r--   0 runner    (1001) docker     (127)  1158136 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/multiplier.v
+-rw-r--r--   0 runner    (1001) docker     (127)    38989 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/priority.v
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/router.v
+-rw-r--r--   0 runner    (1001) docker     (127)   214688 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/sin.v
+-rw-r--r--   0 runner    (1001) docker     (127)  1087553 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/sqrt.v
+-rw-r--r--   0 runner    (1001) docker     (127)   783980 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/square.v
+-rw-r--r--   0 runner    (1001) docker     (127)   600136 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/voter.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.401051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/
+-rw-r--r--   0 runner    (1001) docker     (127)    18623 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c1355.v
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c17.v
+-rw-r--r--   0 runner    (1001) docker     (127)    15006 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c1908.v
+-rw-r--r--   0 runner    (1001) docker     (127)    29248 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c2670.v
+-rw-r--r--   0 runner    (1001) docker     (127)    37970 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c3540.v
+-rw-r--r--   0 runner    (1001) docker     (127)     7536 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c432.v
+-rw-r--r--   0 runner    (1001) docker     (127)    14628 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c499.v
+-rw-r--r--   0 runner    (1001) docker     (127)    70010 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c5315.v
+-rw-r--r--   0 runner    (1001) docker     (127)    91913 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c6288.v
+-rw-r--r--   0 runner    (1001) docker     (127)    83840 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c7552.v
+-rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c880.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.405051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      222 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/1bitAdderAOIG.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      489 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/1bitAdderMaj.v
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/FA.v
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/FS.v
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/HA.v
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/HS.v
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/RCA2.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      332 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/b1_r2.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      525 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/clpl.v
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/mux21.v
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/mux41.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      428 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/newtag.v
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/par_check.v
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/par_gen.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      294 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/t.v
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xnor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xor2.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      560 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xor5R.v
+-rwxr-xr-x   0 runner    (1001) docker     (127)      479 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xor5_r1.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderAOIG.v
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderMaj.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/2bitAdderMaj.v
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/b1_r2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/c17.v
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/clpl.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/cm82a_5.v
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/majority.v
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/majority_5_r1.v
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/newtag.v
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/parity.v
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/t.v
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/t_5.v
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor.v
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor5Maj.v
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor5_r1.v
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/FA.v
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/HA.v
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/mux21.v
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/par_check.v
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/par_gen.v
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/xnor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/trindade16/xor2.v
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23940 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/nano_placement_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/layout_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/placement_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9590 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 09:45:59.000000 mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:59.409051 mnt_nanoplacer-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-13 09:45:54.000000 mnt_nanoplacer-0.2.2/tests/test_utils.py
```

### Comparing `mnt.nanoplacer-0.2.1/.github/dependabot.yml` & `mnt_nanoplacer-0.2.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/.github/release-drafter.yml` & `mnt_nanoplacer-0.2.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/.github/workflows/codeql.yml` & `mnt_nanoplacer-0.2.2/.github/workflows/codeql.yml`

 * *Files 12% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         language: [javascript, python]
 
     steps:
       - name: Checkout
         uses: actions/checkout@v4
 
       - name: Initialize CodeQL
-        uses: github/codeql-action/init@v2
+        uses: github/codeql-action/init@v3
         with:
           languages: ${{ matrix.language }}
           queries: +security-and-quality
 
       - name: Autobuild
-        uses: github/codeql-action/autobuild@v2
+        uses: github/codeql-action/autobuild@v3
 
       - name: Perform CodeQL Analysis
-        uses: github/codeql-action/analyze@v2
+        uses: github/codeql-action/analyze@v3
         with:
           category: "/language:${{ matrix.language }}"
```

### Comparing `mnt.nanoplacer-0.2.1/.github/workflows/deploy.yml` & `mnt_nanoplacer-0.2.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/.gitignore` & `mnt_nanoplacer-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/.pre-commit-config.yaml` & `mnt_nanoplacer-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/LICENSE` & `mnt_nanoplacer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/PKG-INFO` & `mnt_nanoplacer-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnt.nanoplacer
-Version: 0.2.1
+Version: 0.2.2
 Summary: NanoPlaceR - An open-source framework for placement and routing of Field-coupled Nanotechnologies based on reinforcement learning.
 Author-email: Simon Hofmann <simon.t.hofmann@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Chair for Design Automation, TU Munich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -194,17 +194,17 @@
 ```
 
 # References
 
 In case you are using NanoPlaceR in your work, we would be thankful if you referred to it by citing the following publication:
 
 ```bibtex
-@INPROCEEDINGS{hofmann2023nanoplacer,
+@INPROCEEDINGS{hofmann2024nanoplacer,
   author        = {S. Hofmann and M. Walter and L. Servadei and R. Wille},
-  title         = {{Late Breaking Results From Hybrid Design Automation for Field-coupled Nanotechnologies}},
-  booktitle     = {{Design Automation Conference (DAC)}},
-  year          = {2023},
+  title         = {{Thinking Outside the Clock: Physical Design for Field-coupled Nanocomputing with Deep Reinforcement Learning}},
+  booktitle     = {{2024 25th International Symposium on Quality Electronic Design (ISQED)}},
+  year          = {2024},
 }
 ```
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
```

### Comparing `mnt.nanoplacer-0.2.1/README.md` & `mnt_nanoplacer-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -131,17 +131,17 @@
 ```
 
 # References
 
 In case you are using NanoPlaceR in your work, we would be thankful if you referred to it by citing the following publication:
 
 ```bibtex
-@INPROCEEDINGS{hofmann2023nanoplacer,
+@INPROCEEDINGS{hofmann2024nanoplacer,
   author        = {S. Hofmann and M. Walter and L. Servadei and R. Wille},
-  title         = {{Late Breaking Results From Hybrid Design Automation for Field-coupled Nanotechnologies}},
-  booktitle     = {{Design Automation Conference (DAC)}},
-  year          = {2023},
+  title         = {{Thinking Outside the Clock: Physical Design for Field-coupled Nanocomputing with Deep Reinforcement Learning}},
+  booktitle     = {{2024 25th International Symposium on Quality Electronic Design (ISQED)}},
+  year          = {2024},
 }
 ```
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
```

### Comparing `mnt.nanoplacer-0.2.1/docs/_static/lbr.png` & `mnt_nanoplacer-0.2.2/docs/_static/lbr.png`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/docs/_static/mnt_dark.svg` & `mnt_nanoplacer-0.2.2/docs/_static/mnt_dark.svg`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/docs/_static/mnt_light.svg` & `mnt_nanoplacer-0.2.2/docs/_static/mnt_light.svg`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/pyproject.toml` & `mnt_nanoplacer-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/adder.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/adder.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/arbiter.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/arbiter.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/bar.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/bar.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/cavlc.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/cavlc.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/ctrl.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/ctrl.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/dec.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/dec.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/div.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/div.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/hyp.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/hyp.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/i2c.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/i2c.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/int2float.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/int2float.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/log2.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/log2.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/max.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/max.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/multiplier.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/multiplier.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/priority.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/priority.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/router.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/router.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/sin.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/sin.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/sqrt.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/sqrt.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/square.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/square.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/EPFL/voter.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/EPFL/voter.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c1355.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c1355.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c1908.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c1908.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c2670.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c2670.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c3540.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c3540.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c432.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c432.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c499.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c499.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c5315.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c5315.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c6288.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c6288.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c7552.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c7552.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/ISCAS85/c880.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/ISCAS85/c880.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/RCA2.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/RCA2.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/clpl.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/clpl.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/TOY/xor5R.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/TOY/xor5R.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderMaj.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/1bitAdderMaj.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/2bitAdderMaj.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/2bitAdderMaj.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/clpl.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/clpl.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/cm82a_5.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/cm82a_5.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/majority.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/majority.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/majority_5_r1.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/majority_5_r1.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/newtag.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/newtag.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/parity.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/parity.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/xor5Maj.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor5Maj.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/benchmarks/fontes18/xor5_r1.v` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/benchmarks/fontes18/xor5_r1.v`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/main.py` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import argparse
 import os
 from pathlib import Path
 
 from sb3_contrib import MaskablePPO
 from sb3_contrib.common.maskable.policies import MaskableActorCriticPolicy
-from sb3_contrib.common.maskable.utils import get_action_masks
 
 from mnt.nanoplacer.placement_envs.nano_placement_env import NanoPlacementEnv
 from mnt.nanoplacer.placement_envs.utils import layout_dimensions
 
 
 def create_layout(
     benchmark: str = "trindade16",
@@ -77,33 +76,14 @@
     model.save(
         os.path.join(
             "models",
             f"ppo_{technology}_{function}_{'ROW' if technology == 'SiDB' else clocking_scheme}",
         )
     )
 
-    # reset environment
-    obs, info = env.reset()
-    terminated = False
-
-    while not terminated:
-        # calculate infeasible layout positions
-        action_masks = get_action_masks(env)
-
-        # Predict coordinate for next gate based on the gate to be placed and the action mask
-        action, _states = model.predict(obs, action_masks=action_masks, deterministic=True)
-
-        # place gate, route it and receive reward of +1 if successful, 0 else
-        # placement is terminated if no further feasible placement is possible
-        obs, reward, terminated, truncated, info = env.step(action)
-
-        # print current layout
-        if verbose == 1:
-            env.render()
-
 
 def start():
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "-b",
         "--benchmark",
         type=str,
```

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/nano_placement_env.py` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/nano_placement_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,14 +496,15 @@
 
                 if not possible:
                     self.placement_possible = False
         mask_occupied = self.occupied_tiles.flatten(order="F") == 0
         mask = possible_positions_nodes.flatten(order="F") == 0
         if not any(mask):
             self.placement_possible = False
+            return [True] * len(mask)
         return [mask[i] & mask_occupied[i] for i in range(len(mask))]
 
     def calculate_reward(self, x: int, y: int, placed_node: bool) -> tuple[float, bool]:
         """Calculate reward based on whether a node was placed or not.
         If a node was placed, reward is scaled by the location on the layout if the 2DDWave clocking scheme is used.
 
         :param x:              X-coordinate of the placed gate
```

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/utils/layout_dimensions.py` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/layout_dimensions.py`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt/nanoplacer/placement_envs/utils/placement_utils.py` & `mnt_nanoplacer-0.2.2/src/mnt/nanoplacer/placement_envs/utils/placement_utils.py`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/PKG-INFO` & `mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnt.nanoplacer
-Version: 0.2.1
+Version: 0.2.2
 Summary: NanoPlaceR - An open-source framework for placement and routing of Field-coupled Nanotechnologies based on reinforcement learning.
 Author-email: Simon Hofmann <simon.t.hofmann@tum.de>
 License: MIT License
         
         Copyright (c) 2023 Chair for Design Automation, TU Munich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -194,17 +194,17 @@
 ```
 
 # References
 
 In case you are using NanoPlaceR in your work, we would be thankful if you referred to it by citing the following publication:
 
 ```bibtex
-@INPROCEEDINGS{hofmann2023nanoplacer,
+@INPROCEEDINGS{hofmann2024nanoplacer,
   author        = {S. Hofmann and M. Walter and L. Servadei and R. Wille},
-  title         = {{Late Breaking Results From Hybrid Design Automation for Field-coupled Nanotechnologies}},
-  booktitle     = {{Design Automation Conference (DAC)}},
-  year          = {2023},
+  title         = {{Thinking Outside the Clock: Physical Design for Field-coupled Nanocomputing with Deep Reinforcement Learning}},
+  booktitle     = {{2024 25th International Symposium on Quality Electronic Design (ISQED)}},
+  year          = {2024},
 }
 ```
 
 [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
```

### Comparing `mnt.nanoplacer-0.2.1/src/mnt.nanoplacer.egg-info/SOURCES.txt` & `mnt_nanoplacer-0.2.2/src/mnt.nanoplacer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/tests/test_env.py` & `mnt_nanoplacer-0.2.2/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/tests/test_main.py` & `mnt_nanoplacer-0.2.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mnt.nanoplacer-0.2.1/tests/test_utils.py` & `mnt_nanoplacer-0.2.2/tests/test_utils.py`

 * *Files identical despite different names*

