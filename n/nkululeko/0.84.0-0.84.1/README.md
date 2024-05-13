# Comparing `tmp/nkululeko-0.84.0.tar.gz` & `tmp/nkululeko-0.84.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.84.0.tar", last modified: Fri May  3 14:50:51 2024, max compression
+gzip compressed data, was "nkululeko-0.84.1.tar", last modified: Mon May 13 11:54:13 2024, max compression
```

## Comparing `nkululeko-0.84.0.tar` & `nkululeko-0.84.1.tar`

### file list

```diff
@@ -1,225 +1,226 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17618 2024-05-03 14:43:26.000000 nkululeko-0.84.0/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.84.0/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36346 2024-05-03 14:50:51.185131 nkululeko-0.84.0/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.84.0/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.149131 nkululeko-0.84.0/data/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/aesdd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/aesdd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/androids/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.84.0/data/androids/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/androids_orig/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.84.0/data/androids_orig/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/androids_test/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.84.0/data/androids_test/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/ased/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/ased/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.153131 nkululeko-0.84.0/data/asvp-esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.84.0/data/asvp-esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/baved/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.84.0/data/baved/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/cafe/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.84.0/data/cafe/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/clac/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/clac/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/cmu-mosei/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.84.0/data/cmu-mosei/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/demos/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/ekorpus/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.84.0/data/ekorpus/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emns/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/emns/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emofilm/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.84.0/data/emofilm/convert_to_16k.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.84.0/data/emofilm/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emorynlp/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.84.0/data/emorynlp/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emov-db/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.84.0/data/emov-db/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emovo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/emovo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.157131 nkululeko-0.84.0/data/emozionalmente/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.84.0/data/emozionalmente/create.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/enterface/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/enterface/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/esd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.84.0/data/esd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/gerparas/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.84.0/data/gerparas/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/iemocap/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/iemocap/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/jl/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/jl/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/jtes/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.84.0/data/jtes/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/meld/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/meld/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/mesd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/mesd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/mess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/mess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/mlendsnd/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.84.0/data/mlendsnd/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/msp-improv/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.84.0/data/msp-improv/process_database2.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/msp-podcast/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.84.0/data/msp-podcast/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/oreau2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/oreau2/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/portuguese/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.84.0/data/portuguese/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/ravdess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.84.0/data/ravdess/process_database.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.84.0/data/ravdess/process_database_speaker.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/savee/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/savee/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/shemo/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/shemo/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.173131 nkululeko-0.84.0/data/subesco/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/subesco/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/data/tess/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.84.0/data/tess/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/data/thorsten-emotional/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.84.0/data/thorsten-emotional/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/data/urdu/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.84.0/data/urdu/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/data/vivae/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.84.0/data/vivae/process_database.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.149131 nkululeko-0.84.0/docs/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/docs/source/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.84.0/docs/source/conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.149131 nkululeko-0.84.0/meta/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/meta/demos/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.84.0/meta/demos/demo_best_model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.84.0/meta/demos/my_experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.84.0/meta/demos/my_experiment_local.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.84.0/meta/demos/plot_faster_anim.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.84.0/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.84.0/nkululeko/aug_train.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.84.0/nkululeko/augment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.177131 nkululeko-0.84.0/nkululeko/augmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.84.0/nkululeko/augmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.84.0/nkululeko/augmenting/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.84.0/nkululeko/augmenting/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.84.0/nkululeko/augmenting/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3335 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/augmenting/resampler.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.181131 nkululeko-0.84.0/nkululeko/autopredict/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.84.0/nkululeko/autopredict/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_age.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_arousal.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_dominance.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_gender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_pesq.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_sdr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_stoi.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/autopredict/ap_valence.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/autopredict/estimate_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.84.0/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-03 14:50:26.000000 nkululeko-0.84.0/nkululeko/constants.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.181131 nkululeko-0.84.0/nkululeko/data/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.84.0/nkululeko/data/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.84.0/nkululeko/data/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.84.0/nkululeko/data/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.84.0/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.84.0/nkululeko/demo_feats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.84.0/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30225 2024-05-03 12:01:47.000000 nkululeko-0.84.0/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.84.0/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.84.0/nkululeko/export.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.181131 nkululeko-0.84.0/nkululeko/feat_extract/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.84.0/nkululeko/feat_extract/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_agender_agender.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_auddim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_hubert.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_mos.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_snr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_spectra.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_spkrec.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_squim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_wavlm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4576 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/feat_extract/feats_whisper.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.84.0/nkululeko/feat_extract/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.84.0/nkululeko/feat_extract/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.84.0/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.84.0/nkululeko/file_checker.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.84.0/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.84.0/nkululeko/glob_conf.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.181131 nkululeko-0.84.0/nkululeko/losses/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.84.0/nkululeko/losses/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.84.0/nkululeko/losses/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.84.0/nkululeko/losses/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9288 2024-04-25 13:02:38.000000 nkululeko-0.84.0/nkululeko/modelrunner.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko/models/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.84.0/nkululeko/models/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11601 2024-05-03 14:31:11.000000 nkululeko-0.84.0/nkululeko/models/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.84.0/nkululeko/models/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.84.0/nkululeko/models/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.84.0/nkululeko/models/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.84.0/nkululeko/models/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.84.0/nkululeko/models/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.84.0/nkululeko/models/model_lin_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9854 2024-05-03 14:29:13.000000 nkululeko-0.84.0/nkululeko/models/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.84.0/nkululeko/models/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.84.0/nkululeko/models/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.84.0/nkululeko/models/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.84.0/nkululeko/models/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.84.0/nkululeko/models/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.84.0/nkululeko/models/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.84.0/nkululeko/models/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.84.0/nkululeko/multidb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.84.0/nkululeko/nkuluflag.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.84.0/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.84.0/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/predict.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko/reporting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.84.0/nkululeko/reporting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.84.0/nkululeko/reporting/defines.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.84.0/nkululeko/reporting/latex_writer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.84.0/nkululeko/reporting/report.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.84.0/nkululeko/reporting/report_item.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.84.0/nkululeko/reporting/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.84.0/nkululeko/reporting/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2287 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/resample.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.84.0/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.84.0/nkululeko/segment.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko/segmenting/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.84.0/nkululeko/segmenting/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.84.0/nkululeko/segmenting/seg_inaspeechsegmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.84.0/nkululeko/segmenting/seg_silero.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.84.0/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.84.0/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.84.0/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3109 2024-05-03 14:39:48.000000 nkululeko-0.84.0/nkululeko/test_pretrain.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko/utils/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.84.0/nkululeko/utils/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.84.0/nkululeko/utils/files.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.84.0/nkululeko/utils/stats.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13068 2024-05-03 13:47:24.000000 nkululeko-0.84.0/nkululeko/utils/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36346 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5100 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-03 14:50:51.000000 nkululeko-0.84.0/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.84.0/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-03 14:50:51.185131 nkululeko-0.84.0/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.84.0/setup.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.149131 nkululeko-0.84.0/venv/
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-03 14:50:51.185131 nkululeko-0.84.0/venv/bin/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.84.0/venv/bin/activate_this.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.058281 nkululeko-0.84.1/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17692 2024-05-13 11:53:35.000000 nkululeko-0.84.1/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.84.1/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36420 2024-05-13 11:54:13.058281 nkululeko-0.84.1/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17457 2024-04-24 09:02:29.000000 nkululeko-0.84.1/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.038281 nkululeko-0.84.1/data/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/aesdd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1513 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/aesdd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/androids/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-30 12:19:59.000000 nkululeko-0.84.1/data/androids/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/androids_orig/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-08-20 18:21:45.000000 nkululeko-0.84.1/data/androids_orig/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/androids_test/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-09-19 12:01:52.000000 nkululeko-0.84.1/data/androids_test/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/ased/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1566 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/ased/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/asvp-esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1889 2023-09-06 07:54:15.000000 nkululeko-0.84.1/data/asvp-esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/baved/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1899 2023-09-12 12:11:50.000000 nkululeko-0.84.1/data/baved/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/cafe/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1520 2023-09-11 09:21:27.000000 nkululeko-0.84.1/data/cafe/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/clac/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1202 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/clac/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/cmu-mosei/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1805 2023-10-20 09:59:16.000000 nkululeko-0.84.1/data/cmu-mosei/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2058 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/demos/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/ekorpus/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1641 2023-09-12 12:11:50.000000 nkululeko-0.84.1/data/ekorpus/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emns/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2073 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/emns/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emofilm/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1305 2023-08-23 12:21:27.000000 nkululeko-0.84.1/data/emofilm/convert_to_16k.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1736 2023-08-23 06:49:28.000000 nkululeko-0.84.1/data/emofilm/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emorynlp/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1686 2023-09-20 08:48:00.000000 nkululeko-0.84.1/data/emorynlp/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emov-db/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1777 2023-12-19 12:05:21.000000 nkululeko-0.84.1/data/emov-db/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emovo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1595 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/emovo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/emozionalmente/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9348 2023-08-23 06:49:28.000000 nkululeko-0.84.1/data/emozionalmente/create.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/enterface/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2429 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/enterface/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/esd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1534 2023-09-11 09:21:27.000000 nkululeko-0.84.1/data/esd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/gerparas/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3023 2023-10-06 16:05:03.000000 nkululeko-0.84.1/data/gerparas/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/iemocap/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3041 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/iemocap/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/jl/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2022 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/jl/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/jtes/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1727 2023-10-04 08:46:04.000000 nkululeko-0.84.1/data/jtes/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/meld/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3694 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/meld/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/mesd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2053 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/mesd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/mess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1529 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/mess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/mlendsnd/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1714 2023-12-19 12:05:21.000000 nkululeko-0.84.1/data/mlendsnd/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/msp-improv/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2328 2023-08-23 06:49:28.000000 nkululeko-0.84.1/data/msp-improv/process_database2.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/msp-podcast/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-08-23 06:49:28.000000 nkululeko-0.84.1/data/msp-podcast/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/oreau2/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1557 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/oreau2/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/portuguese/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3892 2023-09-12 12:11:50.000000 nkululeko-0.84.1/data/portuguese/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.042281 nkululeko-0.84.1/data/ravdess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3612 2024-04-22 09:09:10.000000 nkululeko-0.84.1/data/ravdess/process_database.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3144 2023-10-06 16:05:03.000000 nkululeko-0.84.1/data/ravdess/process_database_speaker.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/savee/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1680 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/savee/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/shemo/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1624 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/shemo/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/subesco/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2991 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/subesco/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/tess/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1472 2023-09-11 09:21:27.000000 nkululeko-0.84.1/data/tess/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/thorsten-emotional/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1142 2023-09-06 07:54:15.000000 nkululeko-0.84.1/data/thorsten-emotional/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/urdu/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1803 2023-09-19 09:19:58.000000 nkululeko-0.84.1/data/urdu/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/data/vivae/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1209 2023-09-12 12:11:50.000000 nkululeko-0.84.1/data/vivae/process_database.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.038281 nkululeko-0.84.1/docs/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/docs/source/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3070 2024-04-22 09:09:10.000000 nkululeko-0.84.1/docs/source/conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.038281 nkululeko-0.84.1/meta/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.046281 nkululeko-0.84.1/meta/demos/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      617 2021-10-28 13:49:53.000000 nkululeko-0.84.1/meta/demos/demo_best_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1252 2022-12-07 09:32:42.000000 nkululeko-0.84.1/meta/demos/my_experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2022-12-15 16:06:58.000000 nkululeko-0.84.1/meta/demos/my_experiment_local.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      681 2021-10-28 13:49:53.000000 nkululeko-0.84.1/meta/demos/plot_faster_anim.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.050281 nkululeko-0.84.1/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-08-31 11:56:33.000000 nkululeko-0.84.1/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3194 2024-02-29 11:07:44.000000 nkululeko-0.84.1/nkululeko/aug_train.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3051 2024-02-29 11:04:02.000000 nkululeko-0.84.1/nkululeko/augment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.050281 nkululeko-0.84.1/nkululeko/augmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:16:55.000000 nkululeko-0.84.1/nkululeko/augmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2905 2023-12-29 16:48:37.000000 nkululeko-0.84.1/nkululeko/augmenting/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2669 2023-12-29 16:49:20.000000 nkululeko-0.84.1/nkululeko/augmenting/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1791 2023-09-07 11:33:33.000000 nkululeko-0.84.1/nkululeko/augmenting/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3542 2024-05-13 11:40:51.000000 nkululeko-0.84.1/nkululeko/augmenting/resampler.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.050281 nkululeko-0.84.1/nkululeko/autopredict/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:02.000000 nkululeko-0.84.1/nkululeko/autopredict/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1095 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_age.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_arousal.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1039 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_dominance.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1008 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_gender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1104 2023-12-19 11:16:16.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1137 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_pesq.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1185 2023-12-19 11:16:16.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_sdr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1107 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1184 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_stoi.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1024 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/autopredict/ap_valence.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5048 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/autopredict/estimate_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      969 2023-09-07 11:39:39.000000 nkululeko-0.84.1/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       39 2024-05-13 11:53:50.000000 nkululeko-0.84.1/nkululeko/constants.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.050281 nkululeko-0.84.1/nkululeko/data/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:06.000000 nkululeko-0.84.1/nkululeko/data/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    27650 2024-04-22 09:10:47.000000 nkululeko-0.84.1/nkululeko/data/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3884 2024-04-24 12:41:45.000000 nkululeko-0.84.1/nkululeko/data/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3232 2024-05-03 09:55:35.000000 nkululeko-0.84.1/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2025 2024-02-29 21:51:15.000000 nkululeko-0.84.1/nkululeko/demo_feats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4757 2024-05-03 09:56:14.000000 nkululeko-0.84.1/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    30225 2024-05-03 12:01:47.000000 nkululeko-0.84.1/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2609 2024-04-30 15:24:17.000000 nkululeko-0.84.1/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4632 2023-12-19 11:16:14.000000 nkululeko-0.84.1/nkululeko/export.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/feat_extract/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:10.000000 nkululeko-0.84.1/nkululeko/feat_extract/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3113 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3424 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_agender_agender.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12722 2024-05-03 14:41:56.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3162 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_auddim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3187 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3489 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5196 2024-04-24 17:12:28.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_hubert.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1622 2024-04-23 09:55:16.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2021 2023-12-19 11:16:16.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4174 2024-04-23 10:17:00.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_mos.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3978 2024-04-24 10:46:37.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4980 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3105 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_snr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3670 2024-04-23 09:59:48.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_spectra.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4803 2023-10-06 16:05:03.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_spkrec.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4617 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_squim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3228 2024-04-30 09:31:46.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5268 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4703 2024-04-24 17:06:22.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_wavlm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4576 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/feat_extract/feats_whisper.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1448 2024-04-23 09:16:18.000000 nkululeko-0.84.1/nkululeko/feat_extract/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21304 2024-04-15 13:57:11.000000 nkululeko-0.84.1/nkululeko/feat_extract/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3976 2024-04-23 11:13:33.000000 nkululeko-0.84.1/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3474 2023-12-19 11:16:14.000000 nkululeko-0.84.1/nkululeko/file_checker.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7222 2023-12-19 11:16:14.000000 nkululeko-0.84.1/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      525 2024-05-03 12:01:14.000000 nkululeko-0.84.1/nkululeko/glob_conf.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/losses/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:16.000000 nkululeko-0.84.1/nkululeko/losses/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      976 2023-09-07 11:37:43.000000 nkululeko-0.84.1/nkululeko/losses/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1309 2023-09-26 13:42:48.000000 nkululeko-0.84.1/nkululeko/losses/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9288 2024-04-25 13:02:38.000000 nkululeko-0.84.1/nkululeko/modelrunner.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/models/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:20.000000 nkululeko-0.84.1/nkululeko/models/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4910 2024-05-13 09:34:11.000000 nkululeko-0.84.1/nkululeko/models/finetune_model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11601 2024-05-03 14:31:11.000000 nkululeko-0.84.1/nkululeko/models/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2024-05-03 14:26:57.000000 nkululeko-0.84.1/nkululeko/models/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9954 2024-05-03 14:27:45.000000 nkululeko-0.84.1/nkululeko/models/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      649 2024-05-03 14:28:01.000000 nkululeko-0.84.1/nkululeko/models/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      599 2024-05-03 14:28:22.000000 nkululeko-0.84.1/nkululeko/models/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      610 2024-05-03 14:28:14.000000 nkululeko-0.84.1/nkululeko/models/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      422 2024-05-03 14:28:34.000000 nkululeko-0.84.1/nkululeko/models/model_lin_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9854 2024-05-03 14:29:13.000000 nkululeko-0.84.1/nkululeko/models/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10204 2024-05-03 14:28:58.000000 nkululeko-0.84.1/nkululeko/models/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      940 2024-05-03 14:29:24.000000 nkululeko-0.84.1/nkululeko/models/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      725 2024-05-03 14:29:39.000000 nkululeko-0.84.1/nkululeko/models/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      417 2024-05-03 14:30:08.000000 nkululeko-0.84.1/nkululeko/models/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      428 2024-05-03 14:29:56.000000 nkululeko-0.84.1/nkululeko/models/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      447 2024-05-03 14:33:39.000000 nkululeko-0.84.1/nkululeko/models/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      418 2024-05-03 14:34:29.000000 nkululeko-0.84.1/nkululeko/models/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5634 2024-04-23 14:42:13.000000 nkululeko-0.84.1/nkululeko/multidb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3725 2024-04-26 06:05:26.000000 nkululeko-0.84.1/nkululeko/nkuluflag.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1968 2024-04-23 12:35:01.000000 nkululeko-0.84.1/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    23276 2024-04-29 13:37:24.000000 nkululeko-0.84.1/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2409 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/predict.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/reporting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-10-13 10:14:37.000000 nkululeko-0.84.1/nkululeko/reporting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      648 2023-10-02 13:54:57.000000 nkululeko-0.84.1/nkululeko/reporting/defines.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1886 2023-12-19 13:13:44.000000 nkululeko-0.84.1/nkululeko/reporting/latex_writer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1060 2023-12-19 11:16:16.000000 nkululeko-0.84.1/nkululeko/reporting/report.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      533 2023-09-26 14:51:22.000000 nkululeko-0.84.1/nkululeko/reporting/report_item.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12841 2024-04-25 13:02:38.000000 nkululeko-0.84.1/nkululeko/reporting/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      742 2024-04-16 12:21:39.000000 nkululeko-0.84.1/nkululeko/reporting/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3354 2024-05-13 11:40:51.000000 nkululeko-0.84.1/nkululeko/resample.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7624 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4101 2024-01-31 12:20:11.000000 nkululeko-0.84.1/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4835 2024-02-29 11:06:43.000000 nkululeko-0.84.1/nkululeko/segment.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/segmenting/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:24.000000 nkululeko-0.84.1/nkululeko/segmenting/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1947 2023-09-07 11:39:09.000000 nkululeko-0.84.1/nkululeko/segmenting/seg_inaspeechsegmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3301 2023-12-19 11:16:15.000000 nkululeko-0.84.1/nkululeko/segmenting/seg_silero.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10047 2023-09-26 13:42:49.000000 nkululeko-0.84.1/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1677 2024-04-26 06:04:30.000000 nkululeko-0.84.1/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3237 2024-04-25 14:01:11.000000 nkululeko-0.84.1/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8131 2024-05-13 09:34:11.000000 nkululeko-0.84.1/nkululeko/test_pretrain.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko/utils/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-09-06 12:17:28.000000 nkululeko-0.84.1/nkululeko/utils/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4021 2023-09-20 08:48:00.000000 nkululeko-0.84.1/nkululeko/utils/files.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2829 2024-04-22 09:09:10.000000 nkululeko-0.84.1/nkululeko/utils/stats.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13816 2024-05-13 11:40:51.000000 nkululeko-0.84.1/nkululeko/utils/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    36420 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5135 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      298 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2024-05-13 11:54:13.000000 nkululeko-0.84.1/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.84.1/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1001 2024-05-13 11:54:13.058281 nkululeko-0.84.1/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.84.1/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.038281 nkululeko-0.84.1/venv/
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2024-05-13 11:54:13.054281 nkululeko-0.84.1/venv/bin/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1200 2023-12-29 19:06:16.000000 nkululeko-0.84.1/venv/bin/activate_this.py
```

### Comparing `nkululeko-0.84.0/CHANGELOG.md` & `nkululeko-0.84.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.84.1
+--------------
+* made resample independent of config file
+
 Version 0.84.0
 --------------
 * added SHAP analysis
 * started with finetuning
 
 Version 0.83.3
 --------------
```

### Comparing `nkululeko-0.84.0/LICENSE` & `nkululeko-0.84.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/PKG-INFO` & `nkululeko-0.84.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.84.0
+Version: 0.84.1
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.84.1
+--------------
+* made resample independent of config file
+
 Version 0.84.0
 --------------
 * added SHAP analysis
 * started with finetuning
 
 Version 0.83.3
 --------------
```

### Comparing `nkululeko-0.84.0/README.md` & `nkululeko-0.84.1/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/aesdd/process_database.py` & `nkululeko-0.84.1/data/aesdd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/androids/process_database.py` & `nkululeko-0.84.1/data/androids/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/androids_orig/process_database.py` & `nkululeko-0.84.1/data/androids_orig/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/androids_test/process_database.py` & `nkululeko-0.84.1/data/androids_test/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/ased/process_database.py` & `nkululeko-0.84.1/data/ased/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/asvp-esd/process_database.py` & `nkululeko-0.84.1/data/asvp-esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/baved/process_database.py` & `nkululeko-0.84.1/data/baved/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/cafe/process_database.py` & `nkululeko-0.84.1/data/cafe/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/clac/process_database.py` & `nkululeko-0.84.1/data/clac/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/cmu-mosei/process_database.py` & `nkululeko-0.84.1/data/cmu-mosei/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/demos/process_database.py` & `nkululeko-0.84.1/data/demos/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/ekorpus/process_database.py` & `nkululeko-0.84.1/data/ekorpus/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/emns/process_database.py` & `nkululeko-0.84.1/data/emns/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/emofilm/convert_to_16k.py` & `nkululeko-0.84.1/data/emofilm/convert_to_16k.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/emofilm/process_database.py` & `nkululeko-0.84.1/data/emofilm/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/emorynlp/process_database.py` & `nkululeko-0.84.1/data/emorynlp/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/emov-db/process_database.py` & `nkululeko-0.84.1/data/emov-db/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/emovo/process_database.py` & `nkululeko-0.84.1/data/emovo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/emozionalmente/create.py` & `nkululeko-0.84.1/data/emozionalmente/create.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/enterface/process_database.py` & `nkululeko-0.84.1/data/enterface/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/esd/process_database.py` & `nkululeko-0.84.1/data/esd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/gerparas/process_database.py` & `nkululeko-0.84.1/data/gerparas/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/iemocap/process_database.py` & `nkululeko-0.84.1/data/iemocap/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/jl/process_database.py` & `nkululeko-0.84.1/data/jl/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/jtes/process_database.py` & `nkululeko-0.84.1/data/jtes/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/meld/process_database.py` & `nkululeko-0.84.1/data/meld/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/mesd/process_database.py` & `nkululeko-0.84.1/data/mesd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/mess/process_database.py` & `nkululeko-0.84.1/data/mess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/mlendsnd/process_database.py` & `nkululeko-0.84.1/data/mlendsnd/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/msp-improv/process_database2.py` & `nkululeko-0.84.1/data/msp-improv/process_database2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/msp-podcast/process_database.py` & `nkululeko-0.84.1/data/msp-podcast/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/oreau2/process_database.py` & `nkululeko-0.84.1/data/oreau2/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/portuguese/process_database.py` & `nkululeko-0.84.1/data/portuguese/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/ravdess/process_database.py` & `nkululeko-0.84.1/data/ravdess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/ravdess/process_database_speaker.py` & `nkululeko-0.84.1/data/ravdess/process_database_speaker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/savee/process_database.py` & `nkululeko-0.84.1/data/savee/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/shemo/process_database.py` & `nkululeko-0.84.1/data/shemo/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/subesco/process_database.py` & `nkululeko-0.84.1/data/subesco/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/tess/process_database.py` & `nkululeko-0.84.1/data/tess/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/thorsten-emotional/process_database.py` & `nkululeko-0.84.1/data/thorsten-emotional/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/urdu/process_database.py` & `nkululeko-0.84.1/data/urdu/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/data/vivae/process_database.py` & `nkululeko-0.84.1/data/vivae/process_database.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/docs/source/conf.py` & `nkululeko-0.84.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/meta/demos/demo_best_model.py` & `nkululeko-0.84.1/meta/demos/demo_best_model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/meta/demos/my_experiment.py` & `nkululeko-0.84.1/meta/demos/my_experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/meta/demos/my_experiment_local.py` & `nkululeko-0.84.1/meta/demos/my_experiment_local.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/meta/demos/plot_faster_anim.py` & `nkululeko-0.84.1/meta/demos/plot_faster_anim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/aug_train.py` & `nkululeko-0.84.1/nkululeko/aug_train.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/augment.py` & `nkululeko-0.84.1/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/augmenting/augmenter.py` & `nkululeko-0.84.1/nkululeko/augmenting/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/augmenting/randomsplicer.py` & `nkululeko-0.84.1/nkululeko/augmenting/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/augmenting/randomsplicing.py` & `nkululeko-0.84.1/nkululeko/augmenting/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/augmenting/resampler.py` & `nkululeko-0.84.1/nkululeko/augmenting/resampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 import audformat
 import pandas as pd
 import torchaudio
 from nkululeko.utils.util import Util
 
 
 class Resampler:
-    def __init__(self, df, not_testing=True):
+    def __init__(self, df, replace, not_testing=True):
         self.SAMPLING_RATE = 16000
         self.df = df
         self.util = Util("resampler", has_config=not_testing)
         self.util.warn(f"all files might be resampled to {self.SAMPLING_RATE}")
         self.not_testing = not_testing
+        self.replace = eval(self.util.config_val(
+            "RESAMPLE", "replace", "False")) if not not_testing else replace
 
     def resample(self):
         files = self.df.index.get_level_values(0).values
-        replace = eval(self.util.config_val("RESAMPLE", "replace", "False"))
+        # replace = eval(self.util.config_val("RESAMPLE", "replace", "False"))
+        replace = self.replace
         if self.not_testing:
             store = self.util.get_path("store")
         else:
             store = "./"
         tmp_audio = "tmp_resample.wav"
         succes, error = 0, 0
         if not replace:
@@ -38,15 +41,16 @@
             # if f cannot be loaded, give warning and skip
             if signal.shape[0] == 0:
                 self.util.warn(f"cannot load {f}")
                 error += 1
                 continue
             if org_sr != self.SAMPLING_RATE:
                 self.util.debug(f"resampling {f} (sr = {org_sr})")
-                resampler = torchaudio.transforms.Resample(org_sr, self.SAMPLING_RATE)
+                resampler = torchaudio.transforms.Resample(
+                    org_sr, self.SAMPLING_RATE)
                 signal = resampler(signal)
                 if replace:
                     torchaudio.save(
                         os.path.splitext(f)[0] + ".wav",
                         signal,
                         self.SAMPLING_RATE,
                     )
@@ -55,15 +59,16 @@
                     torchaudio.save(new_file_name, signal, self.SAMPLING_RATE)
                     new_files.append(new_file_name)
                 succes += 1
         if not replace:
             self.df = self.df.set_index(
                 self.df.index.set_levels(new_files, level="file")
             )
-            target_file = self.util.config_val("RESAMPLE", "target", "resampled.csv")
+            target_file = self.util.config_val(
+                "RESAMPLE", "target", "resampled.csv")
             # remove encoded labels
             target = self.util.config_val("DATA", "target", "emotion")
             if "class_label" in self.df.columns:
                 self.df = self.df.drop(columns=[target])
                 self.df = self.df.rename(columns={"class_label": target})
             # save file
             self.df.to_csv(target_file)
```

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_age.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_age.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_arousal.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_arousal.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_dominance.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_dominance.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_gender.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_gender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_mos.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_pesq.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_pesq.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_sdr.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_sdr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_snr.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_stoi.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_stoi.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/ap_valence.py` & `nkululeko-0.84.1/nkululeko/autopredict/ap_valence.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/autopredict/estimate_snr.py` & `nkululeko-0.84.1/nkululeko/autopredict/estimate_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/cacheddataset.py` & `nkululeko-0.84.1/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/data/dataset.py` & `nkululeko-0.84.1/nkululeko/data/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/data/dataset_csv.py` & `nkululeko-0.84.1/nkululeko/data/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/demo.py` & `nkululeko-0.84.1/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/demo_feats.py` & `nkululeko-0.84.1/nkululeko/demo_feats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/demo_predictor.py` & `nkululeko-0.84.1/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/experiment.py` & `nkululeko-0.84.1/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/explore.py` & `nkululeko-0.84.1/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/export.py` & `nkululeko-0.84.1/nkululeko/export.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_agender.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_agender_agender.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_agender_agender.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_analyser.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_auddim.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_auddim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_audmodel.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_clap.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_hubert.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_hubert.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_import.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_mld.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_mos.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_mos.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_opensmile.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_oxbow.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_praat.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_snr.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_snr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_spectra.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_spectra.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_spkrec.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_spkrec.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_squim.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_squim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_trill.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_wav2vec2.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_wavlm.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_wavlm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feats_whisper.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feats_whisper.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/featureset.py` & `nkululeko-0.84.1/nkululeko/feat_extract/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feat_extract/feinberg_praat.py` & `nkululeko-0.84.1/nkululeko/feat_extract/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/feature_extractor.py` & `nkululeko-0.84.1/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/file_checker.py` & `nkululeko-0.84.1/nkululeko/file_checker.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/filter_data.py` & `nkululeko-0.84.1/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/glob_conf.py` & `nkululeko-0.84.1/nkululeko/glob_conf.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/losses/loss_ccc.py` & `nkululeko-0.84.1/nkululeko/losses/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/losses/loss_softf1loss.py` & `nkululeko-0.84.1/nkululeko/losses/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/modelrunner.py` & `nkululeko-0.84.1/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model.py` & `nkululeko-0.84.1/nkululeko/models/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model_cnn.py` & `nkululeko-0.84.1/nkululeko/models/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model_gmm.py` & `nkululeko-0.84.1/nkululeko/models/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model_knn.py` & `nkululeko-0.84.1/nkululeko/models/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model_knn_reg.py` & `nkululeko-0.84.1/nkululeko/models/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model_mlp.py` & `nkululeko-0.84.1/nkululeko/models/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model_mlp_regression.py` & `nkululeko-0.84.1/nkululeko/models/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model_svm.py` & `nkululeko-0.84.1/nkululeko/models/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/models/model_svr.py` & `nkululeko-0.84.1/nkululeko/models/model_svr.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/multidb.py` & `nkululeko-0.84.1/nkululeko/multidb.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/nkuluflag.py` & `nkululeko-0.84.1/nkululeko/nkuluflag.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/nkululeko.py` & `nkululeko-0.84.1/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/plots.py` & `nkululeko-0.84.1/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/predict.py` & `nkululeko-0.84.1/nkululeko/predict.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/reporting/defines.py` & `nkululeko-0.84.1/nkululeko/reporting/defines.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/reporting/latex_writer.py` & `nkululeko-0.84.1/nkululeko/reporting/latex_writer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/reporting/report.py` & `nkululeko-0.84.1/nkululeko/reporting/report.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/reporting/report_item.py` & `nkululeko-0.84.1/nkululeko/reporting/report_item.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/reporting/reporter.py` & `nkululeko-0.84.1/nkululeko/reporting/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/reporting/result.py` & `nkululeko-0.84.1/nkululeko/reporting/result.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/resample.py` & `nkululeko-0.84.1/nkululeko/resample.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,100 @@
 # resample.py
-# change the sampling rate for train and test splits
+# change the sampling rate for audio file or INI file (train, test, all)
 
 import argparse
 import configparser
 import os
-
 import pandas as pd
-
+import audformat
 from nkululeko.augmenting.resampler import Resampler
+from nkululeko.utils.util import Util
+
 from nkululeko.constants import VERSION
 from nkululeko.experiment import Experiment
-from nkululeko.utils.util import Util
 
 
 def main(src_dir):
     parser = argparse.ArgumentParser(
-        description="Call the nkululeko RESAMPLE  framework.")
-    parser.add_argument("--config", default="exp.ini",
+        description="Call the nkululeko RESAMPLE framework.")
+    parser.add_argument("--config", default=None,
                         help="The base configuration")
+    parser.add_argument("--file", default=None,
+                        help="The input audio file to resample")
+    parser.add_argument("--replace", action="store_true",
+                        help="Replace the original audio file")
+
     args = parser.parse_args()
-    if args.config is not None:
-        config_file = args.config
-    else:
-        config_file = f"{src_dir}/exp.ini"
 
-    # test if the configuration file exists
-    if not os.path.isfile(config_file):
-        print(f"ERROR: no such file: {config_file}")
+    if args.file is None and args.config is None:
+        print("ERROR: Either --file or --config argument must be provided.")
         exit()
 
-    # load one configuration per experiment
-    config = configparser.ConfigParser()
-    config.read(config_file)
-    # create a new experiment
-    expr = Experiment(config)
-    module = "resample"
-    expr.set_module(module)
-    util = Util(module)
-    util.debug(
-        f"running {expr.name} from config {config_file}, nkululeko version"
-        f" {VERSION}"
-    )
-
-    if util.config_val("EXP", "no_warnings", False):
-        import warnings
-
-        warnings.filterwarnings("ignore")
-
-    # load the data
-    expr.load_datasets()
-
-    # split into train and test
-    expr.fill_train_and_tests()
-    util.debug(
-        f"train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}")
-
-    sample_selection = util.config_val("RESAMPLE", "sample_selection", "all")
-    if sample_selection == "all":
-        df = pd.concat([expr.df_train, expr.df_test])
-    elif sample_selection == "train":
-        df = expr.df_train
-    elif sample_selection == "test":
-        df = expr.df_test
+    if args.file is not None:
+        # Load the audio file into a DataFrame
+        files = pd.Series([args.file])
+        df_sample = pd.DataFrame(index=files)
+        df_sample.index = audformat.utils.to_segmented_index(
+            df_sample.index, allow_nat=False
+        )
+
+        # Resample the audio file
+        util = Util("resampler", has_config=False)
+        util.debug(f"Resampling audio file: {args.file}")
+        rs = Resampler(df_sample, not_testing=True, replace=args.replace)
+        rs.resample()
     else:
-        util.error(
-            f"unknown selection specifier {sample_selection}, should be [all |"
-            " train | test]"
+        # Existing code for handling INI file
+        config_file = args.config
+
+        # Test if the configuration file exists
+        if not os.path.isfile(config_file):
+            print(f"ERROR: no such file: {config_file}")
+            exit()
+
+        # Load one configuration per experiment
+        config = configparser.ConfigParser()
+        config.read(config_file)
+        # Create a new experiment
+        expr = Experiment(config)
+        module = "resample"
+        expr.set_module(module)
+        util = Util(module)
+        util.debug(
+            f"running {expr.name} from config {config_file}, nkululeko version"
+            f" {VERSION}"
         )
-    util.debug(f"resampling {sample_selection}: {df.shape[0]} samples")
-    rs = Resampler(df)
-    rs.resample()
-    print("DONE")
+
+        if util.config_val("EXP", "no_warnings", False):
+            import warnings
+            warnings.filterwarnings("ignore")
+
+        # Load the data
+        expr.load_datasets()
+
+        # Split into train and test
+        expr.fill_train_and_tests()
+        util.debug(
+            f"train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}")
+
+        sample_selection = util.config_val(
+            "RESAMPLE", "sample_selection", "all")
+        if sample_selection == "all":
+            df = pd.concat([expr.df_train, expr.df_test])
+        elif sample_selection == "train":
+            df = expr.df_train
+        elif sample_selection == "test":
+            df = expr.df_test
+        else:
+            util.error(
+                f"unknown selection specifier {sample_selection}, should be [all |"
+                " train | test]"
+            )
+        util.debug(f"resampling {sample_selection}: {df.shape[0]} samples")
+        replace = util.config_val("RESAMPLE", "replace", "False")
+        rs = Resampler(df, replace=replace)
+        rs.resample()
 
 
 if __name__ == "__main__":
     cwd = os.path.dirname(os.path.abspath(__file__))
-    main(cwd)  # use this if you want to state the config file path on command line
+    main(cwd)
```

### Comparing `nkululeko-0.84.0/nkululeko/runmanager.py` & `nkululeko-0.84.1/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/scaler.py` & `nkululeko-0.84.1/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/segment.py` & `nkululeko-0.84.1/nkululeko/segment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/segmenting/seg_inaspeechsegmenter.py` & `nkululeko-0.84.1/nkululeko/segmenting/seg_inaspeechsegmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/segmenting/seg_silero.py` & `nkululeko-0.84.1/nkululeko/segmenting/seg_silero.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/syllable_nuclei.py` & `nkululeko-0.84.1/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/test.py` & `nkululeko-0.84.1/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/test_predictor.py` & `nkululeko-0.84.1/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/utils/files.py` & `nkululeko-0.84.1/nkululeko/utils/files.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/utils/stats.py` & `nkululeko-0.84.1/nkululeko/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/nkululeko/utils/util.py` & `nkululeko-0.84.1/nkululeko/utils/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,51 +29,66 @@
 
     def __init__(self, caller=None, has_config=True):
         if caller is not None:
             self.caller = caller
         else:
             self.caller = ""
         if has_config:
-            import nkululeko.glob_conf as glob_conf
-
-            self.config = glob_conf.config
-            self.got_data_roots = self.config_val("DATA", "root_folders", False)
-            if self.got_data_roots:
-                # if there is a global data rootfolder file, read from there
-                if not os.path.isfile(self.got_data_roots):
-                    self.error(f"no such file: {self.got_data_roots}")
-                self.data_roots = configparser.ConfigParser()
-                self.data_roots.read(self.got_data_roots)
-                # self.debug(f"getting data roots from {self.got_data_roots}")
+            try:
+                import nkululeko.glob_conf as glob_conf
+                self.config = glob_conf.config
+                self.got_data_roots = self.config_val(
+                    "DATA", "root_folders", False)
+                if self.got_data_roots:
+                    # if there is a global data rootfolder file, read from there
+                    if not os.path.isfile(self.got_data_roots):
+                        self.error(f"no such file: {self.got_data_roots}")
+                    self.data_roots = configparser.ConfigParser()
+                    self.data_roots.read(self.got_data_roots)
+            except (ModuleNotFoundError, AttributeError):
+                self.config = None
+                self.got_data_roots = False
 
     def get_path(self, entry):
         """
         This method allows the user to get the directory path for the given argument.
         """
-        root = os.path.join(self.config["EXP"]["root"], "")
-        name = self.config["EXP"]["name"]
-        try:
-            entryn = self.config["EXP"][entry]
-        except KeyError:
-            # some default values
+        if self.config is None:
+            # If no configuration file is provided, use default paths
             if entry == "fig_dir":
-                entryn = "./images/"
+                dir_name = "./images/"
             elif entry == "res_dir":
-                entryn = "./results/"
+                dir_name = "./results/"
             elif entry == "model_dir":
-                entryn = "./models/"
+                dir_name = "./models/"
             else:
-                entryn = "./store/"
+                dir_name = "./store/"
+        else:
+            root = os.path.join(self.config["EXP"]["root"], "")
+            name = self.config["EXP"]["name"]
+            try:
+                entryn = self.config["EXP"][entry]
+            except KeyError:
+                # some default values
+                if entry == "fig_dir":
+                    entryn = "./images/"
+                elif entry == "res_dir":
+                    entryn = "./results/"
+                elif entry == "model_dir":
+                    entryn = "./models/"
+                else:
+                    entryn = "./store/"
+
+            # Expand image, model and result directories with run index
+            if entry == "fig_dir" or entry == "res_dir" or entry == "model_dir":
+                run = self.config_val("EXP", "run", 0)
+                entryn = entryn + f"run_{run}/"
 
-        # Expand image, model and result directories with run index
-        if entry == "fig_dir" or entry == "res_dir" or entry == "model_dir":
-            run = self.config_val("EXP", "run", 0)
-            entryn = entryn + f"run_{run}/"
+            dir_name = f"{root}{name}/{entryn}"
 
-        dir_name = f"{root}{name}/{entryn}"
         audeer.mkdir(dir_name)
         return dir_name
 
     def config_val_data(self, dataset, key, default):
         """
         Retrieve a configuration value for datasets.
         If the value is present in the experiment configuration it will be used, else
@@ -97,15 +112,16 @@
                 except KeyError:
                     if not default in self.stopvals:
                         self.debug(
                             f"value for {key} not found, using default:" f" {default}"
                         )
                     return default
             if not default in self.stopvals:
-                self.debug(f"value for {key} not found, using default: {default}")
+                self.debug(
+                    f"value for {key} not found, using default: {default}")
             return default
 
     def set_config(self, config):
         self.config = config
 
     def get_save_name(self):
         """Return a relative path to a name to save the experiment"""
@@ -134,15 +150,16 @@
         audeer.mkdir(dir_name)
         return dir_name
 
     def make_segmented_index(self, df):
         if len(df) == 0:
             return df
         if not isinstance(df.index, pd.MultiIndex):
-            df.index = audformat.utils.to_segmented_index(df.index, allow_nat=False)
+            df.index = audformat.utils.to_segmented_index(
+                df.index, allow_nat=False)
         return df
 
     def _get_value_descript(self, section, name):
         if self.config_val(section, name, False):
             val = self.config_val(section, name, False)
             val = str(val).strip(".")
             return f"_{name}-{str(val)}"
@@ -239,27 +256,31 @@
 
     def check_df(self, i, df):
         """Check a dataframe"""
         print(f"check {i}: {df.shape}")
         print(df.head(1))
 
     def config_val(self, section, key, default):
+        if self.config is None:
+            return default
         try:
             return self.config[section][key]
         except KeyError:
-            if not default in self.stopvals:
-                self.debug(f"value for {key} not found, using default: {default}")
+            if default not in self.stopvals:
+                self.debug(
+                    f"value for {key} not found, using default: {default}")
             return default
 
     def config_val_list(self, section, key, default):
         try:
             return ast.literal_eval(self.config[section][key])
         except KeyError:
             if not default in self.stopvals:
-                self.debug(f"value for {key} not found, using default: {default}")
+                self.debug(
+                    f"value for {key} not found, using default: {default}")
             return default
 
     def continuous_to_categorical(self, series):
         """
         discretize a categorical variable.
         uses the labels and bins from the ini if present
```

### Comparing `nkululeko-0.84.0/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.84.1/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.84.0
+Version: 0.84.1
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -329,14 +329,18 @@
    year = {2022},
 }
 ```
 
 Changelog
 =========
 
+Version 0.84.1
+--------------
+* made resample independent of config file
+
 Version 0.84.0
 --------------
 * added SHAP analysis
 * started with finetuning
 
 Version 0.83.3
 --------------
```

### Comparing `nkululeko-0.84.0/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.84.1/nkululeko.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 nkululeko/feat_extract/feats_whisper.py
 nkululeko/feat_extract/featureset.py
 nkululeko/feat_extract/feinberg_praat.py
 nkululeko/losses/__init__.py
 nkululeko/losses/loss_ccc.py
 nkululeko/losses/loss_softf1loss.py
 nkululeko/models/__init__.py
+nkululeko/models/finetune_model.py
 nkululeko/models/model.py
 nkululeko/models/model_bayes.py
 nkululeko/models/model_cnn.py
 nkululeko/models/model_gmm.py
 nkululeko/models/model_knn.py
 nkululeko/models/model_knn_reg.py
 nkululeko/models/model_lin_reg.py
```

### Comparing `nkululeko-0.84.0/setup.cfg` & `nkululeko-0.84.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nkululeko-0.84.0/venv/bin/activate_this.py` & `nkululeko-0.84.1/venv/bin/activate_this.py`

 * *Files identical despite different names*

