# Comparing `tmp/nxstools-3.9.0.tar.gz` & `tmp/nxstools-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nxstools-3.9.0.tar", last modified: Tue Jun  8 08:46:59 2021, max compression
+gzip compressed data, was "nxstools-4.0.0.tar", last modified: Mon May 13 08:58:33 2024, max compression
```

## Comparing `nxstools-3.9.0.tar` & `nxstools-4.0.0.tar`

### file list

```diff
@@ -1,180 +1,380 @@
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/
--rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-03-04 09:18:25.000000 nxstools-3.9.0/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) irc         (39)      203 2016-11-17 08:47:01.000000 nxstools-3.9.0/MANIFEST.in
--rw-r--r--   0 jkotan   (15949) irc         (39)     5126 2021-06-08 08:46:59.000000 nxstools-3.9.0/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     2918 2019-10-11 17:04:12.000000 nxstools-3.9.0/README.rst
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/man/
--rw-r--r--   0 jkotan   (15949) irc         (39)    11288 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxscollect.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     4981 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxsconfig.1
--rw-r--r--   0 jkotan   (15949) irc         (39)    18340 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxscreate.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     2287 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxsdata.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     6583 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxsetup.1
--rw-r--r--   0 jkotan   (15949) irc         (39)     3067 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxsfileinfo.1
--rw-r--r--   0 jkotan   (15949) irc         (39)   272377 2021-06-08 08:44:41.000000 nxstools-3.9.0/man/nxstools.1
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       73 2016-03-02 14:46:03.000000 nxstools-3.9.0/nxscollect
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       71 2016-11-02 14:11:38.000000 nxstools-3.9.0/nxsconfig
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       72 2016-11-08 13:51:28.000000 nxstools-3.9.0/nxscreate
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2016-04-21 09:21:42.000000 nxstools-3.9.0/nxsdata
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2019-02-22 09:13:56.000000 nxstools-3.9.0/nxsetup
--rwxr-xr-x   0 jkotan   (15949) irc         (39)       75 2016-11-08 13:51:28.000000 nxstools-3.9.0/nxsfileinfo
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools/
--rw-r--r--   0 jkotan   (15949) irc         (39)      921 2019-02-06 13:31:32.000000 nxstools-3.9.0/nxstools/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3423 2021-01-18 12:05:16.000000 nxstools-3.9.0/nxstools/filenamegenerator.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    28443 2021-04-08 11:45:01.000000 nxstools-3.9.0/nxstools/filewriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    55982 2021-04-08 11:45:01.000000 nxstools-3.9.0/nxstools/h5cppwriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    45483 2021-04-08 11:45:01.000000 nxstools-3.9.0/nxstools/h5pywriter.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3263 2019-02-06 13:31:32.000000 nxstools-3.9.0/nxstools/nxsargparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    64920 2021-04-15 09:36:00.000000 nxstools-3.9.0/nxstools/nxscollect.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    61405 2021-05-04 14:44:37.000000 nxstools-3.9.0/nxstools/nxsconfig.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    55939 2021-04-20 05:41:15.000000 nxstools-3.9.0/nxstools/nxscreate.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    74548 2021-04-28 07:36:39.000000 nxstools-3.9.0/nxstools/nxscreator.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    11192 2019-02-06 13:31:32.000000 nxstools-3.9.0/nxstools/nxsdata.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    14561 2021-02-25 11:17:48.000000 nxstools-3.9.0/nxstools/nxsdevicetools.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    55814 2021-04-13 16:06:43.000000 nxstools-3.9.0/nxstools/nxsetup.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    17779 2021-02-12 09:59:39.000000 nxstools-3.9.0/nxstools/nxsfileinfo.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     8150 2021-02-12 09:59:39.000000 nxstools-3.9.0/nxstools/nxsfileparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    35155 2021-05-04 14:44:37.000000 nxstools-3.9.0/nxstools/nxsparser.py
--rw-r--r--   0 jkotan   (15949) irc         (39)    24266 2021-02-22 12:08:03.000000 nxstools-3.9.0/nxstools/nxsxml.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools/pyeval/
--rw-r--r--   0 jkotan   (15949) irc         (39)      848 2021-05-17 13:16:49.000000 nxstools-3.9.0/nxstools/pyeval/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1922 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/pyeval/absorber.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3906 2021-05-17 13:16:49.000000 nxstools-3.9.0/nxstools/pyeval/beamtimeid.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3234 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/common.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2307 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/dalsa.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3224 2021-05-21 09:01:40.000000 nxstools-3.9.0/nxstools/pyeval/datasignal.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2063 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/dcm.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     4551 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/eigerdectris.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     6553 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/lambdavds.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2876 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/limaccd.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     3894 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/lmbd.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1722 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/marccd.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1897 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/pyeval/mssar.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2279 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/mythen.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2629 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/pco.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2975 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/pe.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     5841 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/pilatus.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     1551 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/pyeval/qbpm.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2253 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/pyeval/tangovimba.py
--rw-r--r--   0 jkotan   (15949) irc         (39)      911 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/release.py
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools/xmltemplates/
--rw-r--r--   0 jkotan   (15949) irc         (39)    56094 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/__init__.py
--rw-r--r--   0 jkotan   (15949) irc         (39)     2183 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/absorber.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      272 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/absorber_foil.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      287 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/absorber_thickness.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1995 2020-01-17 09:16:53.000000 nxstools-3.9.0/nxstools/xmltemplates/beamstop.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/beamtime_id.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      453 2021-05-17 13:16:49.000000 nxstools-3.9.0/nxstools/xmltemplates/beamtimeid.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      258 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/beamtimeid.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     6163 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/chcut.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      239 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/chcut_crystal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      337 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/chcut_unitcalibration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      156 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/chemical_formula.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)       96 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/collect2.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      119 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/collect3.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      143 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/collect4.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      166 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/collect5.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      189 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/collect6.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      213 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/common2_common.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      236 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/common3_common.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3334 2021-04-15 09:36:00.000000 nxstools-3.9.0/nxstools/xmltemplates/dalsa.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      463 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/dalsa_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      598 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      525 2021-04-28 11:00:14.000000 nxstools-3.9.0/nxstools/xmltemplates/dalsavds_nrexposedframes_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      506 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/datasignal.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)    11075 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/dcm.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      230 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/dcm_crystal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      236 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/dcm_reflection.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      246 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/dcm_unitcalibration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      189 2019-09-25 14:14:28.000000 nxstools-3.9.0/nxstools/xmltemplates/default.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2247 2021-02-12 09:59:39.000000 nxstools-3.9.0/nxstools/xmltemplates/defaultinstrument.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      428 2019-09-25 14:15:25.000000 nxstools-3.9.0/nxstools/xmltemplates/defaultsample.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      392 2021-05-21 08:27:26.000000 nxstools-3.9.0/nxstools/xmltemplates/defaultsignal.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1183 2021-04-28 08:22:24.000000 nxstools-3.9.0/nxstools/xmltemplates/detectorlive.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2356 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/eigerdectris.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      319 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/eigerdectris_description_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      375 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/eigerdectris_stepindex.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      609 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/eigerdectris_triggermode_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)       49 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/empty.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      228 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/end_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      909 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/keithley.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4685 2021-04-14 10:31:17.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4955 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      481 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m1_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m1_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      481 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m2_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m2_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      481 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m3_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda2m_m3_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      599 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      345 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/lambda_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4643 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      307 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      342 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_framenumbers_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      342 2021-04-20 19:07:23.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      339 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_savefilename_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      911 2021-05-21 09:51:13.000000 nxstools-3.9.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4056 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      413 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      421 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      679 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      295 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_xpixelsize.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      295 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/limaccd_ypixelsize.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3223 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/maia.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1313 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/maiadimension.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1170 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/maiaflux.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1502 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/marccd.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      431 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/marccd_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1628 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/mcaxia.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      263 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/msnsar_env.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      262 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/mssar_env.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3353 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/mythen.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3563 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/mythen2.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      279 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/mythen_filestartnumber.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      431 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/mythen_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      264 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/nexdatas_configuration.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      212 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/nexdatas_version.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     3755 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/pco.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      278 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pco_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      391 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pco_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      549 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pco_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4332 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      270 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      313 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector_fileindex_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      494 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2493 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      278 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus100k_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      276 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus1m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      276 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus2m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      278 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus300k_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      276 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus6m_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      278 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus_description.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      400 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus_filestartnum_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      393 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus_mxparameters_cb.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      558 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/pilatus_postrun.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2028 2020-05-05 09:17:06.000000 nxstools-3.9.0/nxstools/xmltemplates/pinhole.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      560 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/pointdet.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2186 2021-02-22 12:08:03.000000 nxstools-3.9.0/nxstools/xmltemplates/qbpm.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      265 2021-05-19 17:11:12.000000 nxstools-3.9.0/nxstools/xmltemplates/qbpm_foil.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      207 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/sample_name.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      596 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/samplehkl.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      311 2020-01-15 17:35:29.000000 nxstools-3.9.0/nxstools/xmltemplates/sardanaenvironment.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/signal_axes.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/signal_name.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      393 2021-05-21 08:27:26.000000 nxstools-3.9.0/nxstools/xmltemplates/signalname.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     4050 2020-05-05 09:17:06.000000 nxstools-3.9.0/nxstools/xmltemplates/slit.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      920 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/source.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      209 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/start_time.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     1395 2019-09-25 10:30:34.000000 nxstools-3.9.0/nxstools/xmltemplates/tangovimba.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      503 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/tangovimba_external_data.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      598 2021-06-08 08:41:43.000000 nxstools-3.9.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)      134 2019-09-25 10:15:20.000000 nxstools-3.9.0/nxstools/xmltemplates/title.ds.xml
--rw-r--r--   0 jkotan   (15949) irc         (39)     2369 2020-02-06 16:05:03.000000 nxstools-3.9.0/nxstools/xmltemplates/undulator.xml
-drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/
--rw-r--r--   0 jkotan   (15949) irc         (39)     5126 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) irc         (39)     6151 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 18:35:39.000000 nxstools-3.9.0/nxstools.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) irc         (39)       45 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)        9 2021-06-08 08:46:59.000000 nxstools-3.9.0/nxstools.egg-info/top_level.txt
--rw-r--r--   0 jkotan   (15949) irc         (39)      201 2021-06-08 08:46:59.000000 nxstools-3.9.0/setup.cfg
--rw-r--r--   0 jkotan   (15949) irc         (39)     4372 2021-05-17 13:16:49.000000 nxstools-3.9.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.985999 nxstools-4.0.0/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.833997 nxstools-4.0.0/.ci/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.833997 nxstools-4.0.0/.ci/debian10_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3614 2023-01-30 11:59:31.000000 nxstools-4.0.0/.ci/debian10_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.837997 nxstools-4.0.0/.ci/debian10_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3642 2023-01-30 11:59:31.000000 nxstools-4.0.0/.ci/debian10_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.837997 nxstools-4.0.0/.ci/debian11_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2976 2023-01-30 11:59:31.000000 nxstools-4.0.0/.ci/debian11_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.837997 nxstools-4.0.0/.ci/debian9_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3598 2023-01-30 11:59:31.000000 nxstools-4.0.0/.ci/debian9_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.837997 nxstools-4.0.0/.ci/debian9_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3612 2023-01-30 11:59:31.000000 nxstools-4.0.0/.ci/debian9_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5204 2024-04-24 09:15:54.000000 nxstools-4.0.0/.ci/install.sh
+-rw-r--r--   0 jkotan   (15949) irc         (39)      677 2023-10-27 08:48:03.000000 nxstools-4.0.0/.ci/run.sh
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.837997 nxstools-4.0.0/.ci/ubuntu18.04_py2/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3191 2023-01-30 11:59:31.000000 nxstools-4.0.0/.ci/ubuntu18.04_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.837997 nxstools-4.0.0/.ci/ubuntu18.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3188 2023-01-30 11:59:31.000000 nxstools-4.0.0/.ci/ubuntu18.04_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.837997 nxstools-4.0.0/.ci/ubuntu20.04_py3/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3801 2023-02-06 19:31:51.000000 nxstools-4.0.0/.ci/ubuntu20.04_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) irc         (39)      185 2022-10-12 15:26:51.000000 nxstools-4.0.0/.flake8
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.829997 nxstools-4.0.0/.github/
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.837997 nxstools-4.0.0/.github/workflows/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2095 2024-05-13 08:57:45.000000 nxstools-4.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       83 2014-03-04 09:18:25.000000 nxstools-4.0.0/.gitignore
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35147 2014-03-04 09:18:25.000000 nxstools-4.0.0/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) irc         (39)    46235 2024-05-13 08:57:45.000000 nxstools-4.0.0/ChangeLog
+-rw-r--r--   0 jkotan   (15949) irc         (39)      203 2016-11-17 08:47:01.000000 nxstools-4.0.0/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4824 2024-05-13 08:58:33.985999 nxstools-4.0.0/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3543 2023-11-08 19:31:46.000000 nxstools-4.0.0/README.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.845997 nxstools-4.0.0/doc/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6770 2016-04-26 12:17:18.000000 nxstools-4.0.0/doc/Makefile
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14330 2023-11-09 13:02:28.000000 nxstools-4.0.0/doc/conf.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      484 2023-11-09 13:02:37.000000 nxstools-4.0.0/doc/index.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6705 2016-04-26 12:17:18.000000 nxstools-4.0.0/doc/make.bat
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11174 2023-11-09 13:02:37.000000 nxstools-4.0.0/doc/nxscollect.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3909 2023-11-09 13:02:37.000000 nxstools-4.0.0/doc/nxsconfig.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)    19089 2024-02-21 21:28:01.000000 nxstools-4.0.0/doc/nxscreate.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1244 2023-11-09 13:02:37.000000 nxstools-4.0.0/doc/nxsdata.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7020 2024-04-12 10:12:47.000000 nxstools-4.0.0/doc/nxsetup.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)    15854 2024-01-04 17:09:29.000000 nxstools-4.0.0/doc/nxsfileinfo.rst
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3241 2024-05-13 08:57:45.000000 nxstools-4.0.0/doc/nxstools.rst
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.845997 nxstools-4.0.0/man/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11417 2024-05-13 08:57:45.000000 nxstools-4.0.0/man/nxscollect.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4989 2024-05-13 08:57:45.000000 nxstools-4.0.0/man/nxsconfig.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)    22445 2024-05-13 08:57:45.000000 nxstools-4.0.0/man/nxscreate.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2288 2024-05-13 08:57:45.000000 nxstools-4.0.0/man/nxsdata.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8616 2024-05-13 08:57:45.000000 nxstools-4.0.0/man/nxsetup.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)    17461 2024-05-13 08:57:45.000000 nxstools-4.0.0/man/nxsfileinfo.1
+-rw-r--r--   0 jkotan   (15949) irc         (39)   428821 2024-05-13 08:57:45.000000 nxstools-4.0.0/man/nxstools.1
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       73 2016-03-02 14:46:03.000000 nxstools-4.0.0/nxscollect
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       71 2016-11-02 14:11:38.000000 nxstools-4.0.0/nxsconfig
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       72 2016-11-08 13:51:28.000000 nxstools-4.0.0/nxscreate
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2016-04-21 09:21:42.000000 nxstools-4.0.0/nxsdata
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       67 2019-02-22 09:13:56.000000 nxstools-4.0.0/nxsetup
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)       75 2016-11-08 13:51:28.000000 nxstools-4.0.0/nxsfileinfo
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.853997 nxstools-4.0.0/nxstools/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      899 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3401 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/filenamegenerator.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    31327 2024-05-13 08:57:45.000000 nxstools-4.0.0/nxstools/filewriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    59098 2024-05-13 08:57:45.000000 nxstools-4.0.0/nxstools/h5cppwriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    47629 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/h5pywriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    57100 2024-05-13 08:57:45.000000 nxstools-4.0.0/nxstools/h5rediswriter.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3241 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/nxsargparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    64898 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/nxscollect.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    61440 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/nxsconfig.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    65063 2024-02-21 21:28:01.000000 nxstools-4.0.0/nxstools/nxscreate.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   111677 2024-02-21 21:28:01.000000 nxstools-4.0.0/nxstools/nxscreator.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11170 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/nxsdata.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14584 2024-05-13 08:57:45.000000 nxstools-4.0.0/nxstools/nxsdevicetools.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    67628 2024-04-12 10:12:47.000000 nxstools-4.0.0/nxstools/nxsetup.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   188157 2024-02-09 08:24:05.000000 nxstools-4.0.0/nxstools/nxsfileinfo.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    27916 2024-05-08 07:07:07.000000 nxstools-4.0.0/nxstools/nxsfileparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    35902 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/nxsparser.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    25209 2023-11-09 13:02:28.000000 nxstools-4.0.0/nxstools/nxsxml.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.853997 nxstools-4.0.0/nxstools/ontology/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5583 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/ontology/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   191838 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/ontology/ontology.json
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.861997 nxstools-4.0.0/nxstools/pyeval/
+-rw-r--r--   0 jkotan   (15949) irc         (39)      848 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1922 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/absorber.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5617 2022-12-12 11:56:25.000000 nxstools-4.0.0/nxstools/pyeval/beamtimeid.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2119 2022-11-02 12:53:27.000000 nxstools-4.0.0/nxstools/pyeval/cobold.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3836 2022-11-02 07:07:13.000000 nxstools-4.0.0/nxstools/pyeval/common.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2307 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/dalsa.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7272 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/dalsavds.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7304 2023-07-05 09:24:53.000000 nxstools-4.0.0/nxstools/pyeval/datasignal.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2063 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/dcm.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4561 2024-02-19 12:22:32.000000 nxstools-4.0.0/nxstools/pyeval/eigerdectris.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10653 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/lambdavds.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2876 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/limaccd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3894 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/lmbd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1722 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/marccd.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1897 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/mssar.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2279 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/mythen.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2629 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/pco.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2975 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/pe.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5841 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/pilatus.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1551 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/qbpm.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7449 2024-01-02 20:17:43.000000 nxstools-4.0.0/nxstools/pyeval/scdataset.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    14955 2024-02-21 21:28:01.000000 nxstools-4.0.0/nxstools/pyeval/secop.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2253 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/tangovimba.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2888 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/pyeval/timestamp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2502 2024-05-13 08:57:45.000000 nxstools-4.0.0/nxstools/redisutils.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      889 2024-05-13 08:57:45.000000 nxstools-4.0.0/nxstools/release.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.901998 nxstools-4.0.0/nxstools/xmltemplates/
+-rw-r--r--   0 jkotan   (15949) irc         (39)    66661 2024-02-21 21:28:01.000000 nxstools-4.0.0/nxstools/xmltemplates/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2183 2022-12-06 15:35:05.000000 nxstools-4.0.0/nxstools/xmltemplates/absorber.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      272 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/absorber_foil.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      287 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/absorber_thickness.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2002 2022-11-25 10:06:49.000000 nxstools-4.0.0/nxstools/xmltemplates/beamstop.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      171 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/beamtime_filename.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/beamtime_id.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      443 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/beamtimefname.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      330 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/beamtimefname.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      436 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/beamtimeid.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      258 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/beamtimeid.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6163 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/chcut.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      282 2022-11-08 06:33:42.000000 nxstools-4.0.0/nxstools/xmltemplates/chcut_crystal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      358 2022-11-08 06:33:42.000000 nxstools-4.0.0/nxstools/xmltemplates/chcut_unitcalibration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      156 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/chemical_formula.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      216 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/client_start_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      732 2022-11-02 12:07:43.000000 nxstools-4.0.0/nxstools/xmltemplates/cobold.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1694 2022-11-02 12:07:43.000000 nxstools-4.0.0/nxstools/xmltemplates/coboldhisto.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      324 2022-11-02 12:07:43.000000 nxstools-4.0.0/nxstools/xmltemplates/coboldhisto_timeofflight.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       96 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/collect2.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      119 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/collect3.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      143 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/collect4.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      166 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/collect5.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      189 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/collect6.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      214 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/common2_common.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      237 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/common3_common.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3334 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/dalsa.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      438 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/dalsa_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      599 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3375 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/dalsavds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/dalsavds_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      354 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/dalsavds_nrexposedframes_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      336 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/dalsavds_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1088 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/dalsavds_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      597 2022-11-02 07:59:08.000000 nxstools-4.0.0/nxstools/xmltemplates/dataaxessignal.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      506 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/datasignal.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11075 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/dcm.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      230 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/dcm_crystal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      236 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/dcm_reflection.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      246 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/dcm_unitcalibration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      189 2019-09-25 14:14:28.000000 nxstools-4.0.0/nxstools/xmltemplates/default.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      502 2023-07-05 09:24:53.000000 nxstools-4.0.0/nxstools/xmltemplates/defaultaxes.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2702 2024-05-13 08:57:45.000000 nxstools-4.0.0/nxstools/xmltemplates/defaultinstrument.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      428 2019-09-25 14:15:25.000000 nxstools-4.0.0/nxstools/xmltemplates/defaultsample.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      441 2023-07-05 09:24:53.000000 nxstools-4.0.0/nxstools/xmltemplates/defaultsignal.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      274 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/description.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      246 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/descriptiontext.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1183 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/detectorlive.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2356 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/eigerdectris.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      320 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/eigerdectris_description_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      370 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/eigerdectris_stepindex.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      555 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/eigerdectris_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)       49 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/empty.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      228 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/end_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      168 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/experiment_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      304 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/groupsecop.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      403 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/groupsecop_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      909 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/keithley.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4545 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4815 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda2m.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda2m_m1_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda2m_m1_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda2m_m2_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda2m_m2_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      456 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda2m_m3_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      348 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda2m_m3_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      566 2023-02-14 07:32:53.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      345 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/lambda_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4643 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      307 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavds_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      337 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavds_framenumbers_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavds_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      334 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavds_savefilename_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      858 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4612 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavdsnm.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      342 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavdsnm_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      877 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/lambdavdsnm_triggermode_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4056 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/limaccd.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      413 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/limaccd_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      412 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/limaccd_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      646 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/limaccd_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      295 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/limaccd_xpixelsize.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      295 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/limaccd_ypixelsize.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3223 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/maia.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1313 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/maiadimension.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1170 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/maiaflux.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1502 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/marccd.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      414 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/marccd_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1628 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/mcaxia.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      263 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/msnsar_env.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      262 2023-02-14 17:32:17.000000 nxstools-4.0.0/nxstools/xmltemplates/mssar_env.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3353 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/mythen.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3563 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/mythen2.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      280 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/mythen_filestartnumber.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      410 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/mythen_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      264 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/nexdatas_configuration.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      236 2022-11-08 06:33:42.000000 nxstools-4.0.0/nxstools/xmltemplates/nexdatas_version.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      301 2022-12-06 18:19:56.000000 nxstools-4.0.0/nxstools/xmltemplates/parametercopymap.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3755 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/pco.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      278 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/pco_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      382 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pco_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      520 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pco_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4332 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/perkinelmerdetector.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      271 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/perkinelmerdetector_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      307 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/perkinelmerdetector_fileindex_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      469 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/perkinelmerdetector_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2493 2022-10-26 05:57:42.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      279 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus100k_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus1m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus2m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      279 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus300k_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      277 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus6m_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      278 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      391 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus_filestartnum_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      383 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus_mxparameters_cb.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      529 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/pilatus_postrun.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2028 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/pinhole.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      560 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/pointdet.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2186 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/qbpm.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      265 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/qbpm_foil.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      160 2023-01-12 10:09:54.000000 nxstools-4.0.0/nxstools/xmltemplates/sample_description.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      327 2024-02-20 16:16:42.000000 nxstools-4.0.0/nxstools/xmltemplates/sample_env_links.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      326 2024-02-20 16:16:42.000000 nxstools-4.0.0/nxstools/xmltemplates/sample_log_links.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      207 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/sample_name.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      309 2024-02-21 10:18:02.000000 nxstools-4.0.0/nxstools/xmltemplates/sample_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      315 2023-01-12 10:09:54.000000 nxstools-4.0.0/nxstools/xmltemplates/sampledescription.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      296 2023-01-12 10:09:54.000000 nxstools-4.0.0/nxstools/xmltemplates/sampledescriptiontext.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      315 2024-02-21 21:28:01.000000 nxstools-4.0.0/nxstools/xmltemplates/sampleenv_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      596 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/samplehkl.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      311 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/sardanaenvironment.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      271 2024-02-19 15:12:24.000000 nxstools-4.0.0/nxstools/xmltemplates/secop.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      371 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/secop_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/signal_axes.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      146 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/signal_name.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      384 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/signalname.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      259 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/singlesecop.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      359 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/singlesecop_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5066 2023-02-28 12:36:19.000000 nxstools-4.0.0/nxstools/xmltemplates/slit.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      920 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/source.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      209 2022-10-20 05:49:21.000000 nxstools-4.0.0/nxstools/xmltemplates/start_time.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      247 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/start_timestamp.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      321 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/starttime.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      308 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/starttime.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      274 2022-10-19 07:07:03.000000 nxstools-4.0.0/nxstools/xmltemplates/tango.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1395 2019-09-25 10:30:34.000000 nxstools-4.0.0/nxstools/xmltemplates/tangovimba.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      478 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/tangovimba_external_data.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      603 2022-10-25 19:40:52.000000 nxstools-4.0.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      134 2019-09-25 10:15:20.000000 nxstools-4.0.0/nxstools/xmltemplates/title.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2369 2022-10-12 15:26:51.000000 nxstools-4.0.0/nxstools/xmltemplates/undulator.xml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.853997 nxstools-4.0.0/nxstools.egg-info/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4824 2024-05-13 08:58:33.000000 nxstools-4.0.0/nxstools.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11755 2024-05-13 08:58:33.000000 nxstools-4.0.0/nxstools.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2024-05-13 08:58:33.000000 nxstools-4.0.0/nxstools.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        1 2019-10-10 18:35:39.000000 nxstools-4.0.0/nxstools.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) irc         (39)       41 2024-05-13 08:58:33.000000 nxstools-4.0.0/nxstools.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)        9 2024-05-13 08:58:33.000000 nxstools-4.0.0/nxstools.egg-info/top_level.txt
+-rw-r--r--   0 jkotan   (15949) irc         (39)      201 2024-05-13 08:58:33.985999 nxstools-4.0.0/setup.cfg
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4733 2024-05-13 08:58:06.000000 nxstools-4.0.0/setup.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.961999 nxstools-4.0.0/test/
+-rw-r--r--   0 jkotan   (15949) irc         (39)   344154 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/FileWriterH5CppH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   179723 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/FileWriterH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   172755 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/FileWriterH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   215920 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/H5CppWriter_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   181022 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/H5PYWriter_test.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    12534 2022-11-15 13:21:44.000000 nxstools-4.0.0/test/MacroServer2
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    12534 2022-11-15 13:21:44.000000 nxstools-4.0.0/test/MacroServer3
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6333 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/MacroServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1378 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCollectH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1375 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCollectH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   286941 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCollect_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   312641 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSConfig_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateClientDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateClientDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2513 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateClientDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5158 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateClientDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4692 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateClientDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateClientDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    23938 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateClientDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1505 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateCompDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1512 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateCompDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2469 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateCompDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4986 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateCompDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11295 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateCompFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1512 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateCompFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   106092 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateCompFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    24689 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateCompare_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateDeviceDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateDeviceDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2513 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateDeviceDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10662 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateDeviceDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    12050 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateDeviceDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateDeviceDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13367 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateDeviceDSFS4_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    52028 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateDeviceDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2024-03-27 12:55:16.000000 nxstools-4.0.0/test/NXSCreateOnlineCPDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineCPDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3140 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineCPDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5112 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineCPDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    20755 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineCPFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineCPFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   118294 2024-03-27 14:00:23.000000 nxstools-4.0.0/test/NXSCreateOnlineCPFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1532 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1619 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSDBE2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1597 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSDBE_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3282 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5193 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8102 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1540 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    70429 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateOnlineDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1519 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreatePoolDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreatePoolDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3178 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreatePoolDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5044 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreatePoolDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     8582 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreatePoolDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreatePoolDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    43545 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreatePoolDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   111513 2023-12-18 11:00:31.000000 nxstools-4.0.0/test/NXSCreatePyEvalH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1483 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreatePyEvalH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateStdCompDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1665 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateStdCompDBE2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1642 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateStdCompDBE_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1582 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateStdCompDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     3181 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateStdCompDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5116 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateStdCompDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    13494 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateStdCompFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1589 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateStdCompFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    74098 2024-05-13 08:57:45.000000 nxstools-4.0.0/test/NXSCreateStdCompFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1526 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateTangoDSDB2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateTangoDSDBR2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     2502 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateTangoDSDBR_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5019 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateTangoDSDB_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     6160 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateTangoDSFS2_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1533 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateTangoDSFS3_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    51953 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreateTangoDSFS_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7127 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSCreate_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    92377 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSData_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1386 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSFileInfoH5Cpp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1383 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSFileInfoH5PY_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   568895 2024-02-08 19:21:48.000000 nxstools-4.0.0/test/NXSFileInfo_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     1147 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/NXSTools_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)   223693 2024-03-27 14:00:23.000000 nxstools-4.0.0/test/NXSetUp_test.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4543 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/ServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)    10230 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/TestPool.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     5183 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/TestPoolSetUp.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    55523 2022-11-15 13:21:44.000000 nxstools-4.0.0/test/TestServer2
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    55525 2022-11-15 13:21:44.000000 nxstools-4.0.0/test/TestServer3
+-rw-r--r--   0 jkotan   (15949) irc         (39)    11787 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/TestServerSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4582 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/WriterSetUp.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      937 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/__init__.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)      945 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/__main__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4476 2023-11-09 13:02:28.000000 nxstools-4.0.0/test/checks.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.977999 nxstools-4.0.0/test/files/
+-rw-r--r--   0 jkotan   (15949) irc         (39)   101011 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/files/test_file.cbf
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/files/test_file.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/files/test_file0.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/files/test_file1.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/files/test_file2.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/files/test_file3.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/files/test_file4.tif
+-rw-r--r--   0 jkotan   (15949) irc         (39)   383956 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/files/test_file5.tif
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)    18658 2024-05-13 08:57:45.000000 nxstools-4.0.0/test/main.py
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.981999 nxstools-4.0.0/test/nxsextrasp00/
+-rw-r--r--   0 jkotan   (15949) irc         (39)     4449 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/nxsextrasp00/__init__.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)      143 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/nxsextrasp00/collect4.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      258 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/nxsextrasp00/common4_common.ds.xml
+-rw-r--r--   0 jkotan   (15949) irc         (39)      565 2022-10-12 15:26:51.000000 nxstools-4.0.0/test/nxsextrasp00/mymca.xml
+drwxr-xr-x   0 jkotan   (15949) irc         (39)        0 2024-05-13 08:58:33.981999 nxstools-4.0.0/tests/
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     2802 2023-11-09 13:02:28.000000 nxstools-4.0.0/tests/simpleXMLAScan.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     2449 2023-11-09 13:02:28.000000 nxstools-4.0.0/tests/simpleXMLCScan.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     2411 2023-11-09 13:02:28.000000 nxstools-4.0.0/tests/simpleXMLScan.py
+-rw-r--r--   0 jkotan   (15949) irc         (39)     7217 2023-11-09 13:02:28.000000 nxstools-4.0.0/tests/testNXSxml.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     5304 2023-11-09 13:02:28.000000 nxstools-4.0.0/tests/testXMLCreator.py
+-rwxr-xr-x   0 jkotan   (15949) irc         (39)     7425 2023-11-09 13:02:28.000000 nxstools-4.0.0/tests/testXMLtrigger.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nxstools-3.9.0/COPYRIGHT` & `nxstools-4.0.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/README.rst` & `nxstools-4.0.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,128 @@
 Welcome to nxstools's documentation!
 ====================================
 
+
+|github workflow|
+|docs|
+|Pypi Version|
+|Python Versions|
+
+.. |github workflow| image:: https://github.com/nexdatas/nxstools/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/nexdatas/nxstools/actions
+   :alt:
+
+.. |docs| image:: https://img.shields.io/badge/Documentation-webpages-ADD8E6.svg
+   :target: https://nexdatas.github.io/nxstools/index.html
+   :alt:
+
+.. |Pypi Version| image:: https://img.shields.io/pypi/v/nxstools.svg
+                  :target: https://pypi.python.org/pypi/nxstools
+                  :alt:
+
+.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/nxstools.svg
+                     :target: https://pypi.python.org/pypi/nxstools/
+                     :alt:
+
+
 Authors: Jan Kotanski
 
 ------------
 Introduction
 ------------
 
 Configuration tools for NeXDaTaS Tango Servers consists of the following command-line scripts:
 
-- `nxscollect <https://nexdatas.github.io/tools/nxscollect.html>`__ uploads external images into the NeXus/HDF5 file
-- `nxsconfig <https://nexdatas.github.io/tools/nxsconfig.html>`__ reads NeXus Configuration Server settings
-- `nxscreate <https://nexdatas.github.io/tools/nxscreate.html>`__ creates NeXus Configuration components
-- `nxsdata <https://nexdatas.github.io/tools/nxsdata.html>`__ runs NeXus Data Writer
-- `nxsfileinfo <https://nexdatas.github.io/tools/nxsfileinfo.html>`__ shows nedadata of the NeXus/HDF5 file
-- `nxsetup <https://nexdatas.github.io/tools/nxsetup.html>`__ setups NeXDaTaS Tango Server environment
+- `nxscollect <https://nexdatas.github.io/nxstools/nxscollect.html>`__ uploads external images into the NeXus/HDF5 file
+- `nxsconfig <https://nexdatas.github.io/nxstools/nxsconfig.html>`__ reads NeXus Configuration Server settings
+- `nxscreate <https://nexdatas.github.io/nxstools/nxscreate.html>`__ creates NeXus Configuration components
+- `nxsdata <https://nexdatas.github.io/nxstools/nxsdata.html>`__ runs NeXus Data Writer
+- `nxsfileinfo <https://nexdatas.github.io/nxstools/nxsfileinfo.html>`__ shows metadata of the NeXus/HDF5 file
+- `nxsetup <https://nexdatas.github.io/nxstools/nxsetup.html>`__ setups NeXDaTaS Tango Server environment
 
-as well as the `nxstools <https://nexdatas.github.io/tools/nxstools.html>`__ package which allows perform these operations
+as well as the `nxstools <https://nexdatas.github.io/nxstools/nxstools.html>`__ package which allows perform these operations
 directly from a python code.
 
-| Source code: https://github.com/nexdatas/tools
-| Web page: https://nexdatas.github.io/tools
+| Source code: https://github.com/nexdatas/nxstools
+| Web page: https://nexdatas.github.io/nxstools
 | NexDaTaS Web page: https://nexdatas.github.io
 
 ------------
 Installation
 ------------
 
 Install the dependencies:
 
-|    PyTango, sphinx
+|    pninexus or h5py, numpy, tango, sphinx
 
 From sources
 """"""""""""
 
 Download the latest NXS Tools version from
 
-|    https://github.com/nexdatas/tools
+|    https://github.com/nexdatas/nxstools
 
 Extract sources and run
 
 .. code-block:: console
 
 	  $ python setup.py install
 
 Debian packages
 """""""""""""""
 
-Debian `stretch`, `jessie` (and `wheezy`)  or Ubuntu `bionic` (and `xenial`) packages can be found in the HDRI repository.
+Debian `bookworm`, `bullseye`, `buster`  or Ubuntu `lunar`, `jammy`, `focal` packages can be found in the HDRI repository.
 
 To install the debian packages, add the PGP repository key
 
 .. code-block:: console
 
 	  $ sudo su
-	  $ wget -q -O - http://repos.pni-hdri.de/debian_repo.pub.gpg | apt-key add -
+	  $ curl -s http://repos.pni-hdri.de/debian_repo.pub.gpg | gpg --no-default-keyring --keyring gnupg-ring:/etc/apt/trusted.gpg.d/debian-hdri-repo.gpg --import
+	  $ chmod 644 /etc/apt/trusted.gpg.d/debian-hdri-repo.gpg
 
 and then download the corresponding source list
 
 .. code-block:: console
 
 	  $ cd /etc/apt/sources.list.d
-	  $ wget http://repos.pni-hdri.de/stretch-pni-hdri.list
+	  $ wget http://repos.pni-hdri.de/bookworm-pni-hdri.list
 
-For releases (>= 2.61.0) to insall python2 scripts
+To install nxstools scripts
 
 .. code-block:: console
 
 	  $ apt-get update
 	  $ apt-get install nxstools
 
-and for python3 scripts
+or
 
 .. code-block:: console
 
 	  $ apt-get update
 	  $ apt-get install nxstools3
 
+for older python3 releases.
 
-For older releases
+To install only the python3 package
 
 .. code-block:: console
 
 	  $ apt-get update
-	  $ apt-get install python-nxstools
-
-and
-
-.. code-block:: console
-
 	  $ apt-get install python3-nxstools
 
-if exists.
-
-To instal other NexDaTaS packages
+and for python2
 
 .. code-block:: console
 
-	  $ apt-get install python-nxswriter nxsconfigserver-db python-nxsconfigserver nxsconfigtool
-
-and
-
-.. code-block:: console
+	  $ apt-get update
+	  $ apt-get install python-nxstools
 
-	  $ apt-get install python-nxsrecselector nxselector python-sardana-nxsrecorder
+if exists.
 
-for Component Selector and Sardana related packages.
 
 From pip
 """"""""
 
 To install it from pip you can
 
 .. code-block:: console
```

### Comparing `nxstools-3.9.0/man/nxsconfig.1` & `nxstools-4.0.0/man/nxsconfig.1`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSCONFIG" "1" "Jun 08, 2021" "3.9" "NXSTools"
-.SH NAME
-nxsconfig \- read NeXus Configuration Server settings
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,14 +23,17 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "NXSCONFIG" "1" "May 12, 2024" "4.0" "NXSTools"
+.SH NAME
+nxsconfig \- read NeXus Configuration Server settings
 .SH DESCRIPTION
 .sp
 The nxsconfig program
 is a command\-line interface to NXS Configuration Tango Server.
 It allows one to read XML configuration datasources
 and components. It also gives possibility to
 perform the process of component merging.
@@ -58,103 +58,103 @@
 .TP
 .B list \-d [\-s <config_server>] [\-n]
 list names of available datasources
 .TP
 .B list \-r [\-s <config_server>] [\-n]
 list names of available profiles
 .TP
-.B show [\-s <config_server>] [\-m] [\-o <dir>] component_name1 component_name2 …
+.B show [\-s <config_server>] [\-m] [\-o <dir>] component_name1 component_name2 ...
 show components with given names
 .TP
-.B show \-d [\-s <config_server>]  [\-o <dir>] dsource_name1 dsource_name2 …
+.B show \-d [\-s <config_server>]  [\-o <dir>] dsource_name1 dsource_name2 ...
 show datasources with given names
 .TP
-.B show \-r [\-s <config_server>]  [\-o <dir>] profile_name1 profile_name2 …
+.B show \-r [\-s <config_server>]  [\-o <dir>] profile_name1 profile_name2 ...
 show profiles with given names
 .TP
-.B upload [\-s <config_server>] [\-m] [\-i <dir>] [\-f] component_name1 component_name2 …
+.B upload [\-s <config_server>] [\-m] [\-i <dir>] [\-f] component_name1 component_name2 ...
 load components from given files
 .TP
-.B upload \-d [\-s <config_server>]  [\-i <dir>] [\-f] dsource_name1 dsource_name2 …
+.B upload \-d [\-s <config_server>]  [\-i <dir>] [\-f] dsource_name1 dsource_name2 ...
 load datasources from given files
 .TP
-.B upload \-r [\-s <config_server>]  [\-i <dir>] [\-f] profile_name1 profile_name2 …
+.B upload \-r [\-s <config_server>]  [\-i <dir>] [\-f] profile_name1 profile_name2 ...
 load profiles from given files
 .TP
-.B get [\-s <config_server>]  [\-n] component_name1 component_name2 …
+.B get [\-s <config_server>]  [\-n] component_name1 component_name2 ...
 get merged configuration of components
 .TP
-.B delete [\-s <config_server>] [\-f] component_name1 component_name2 …
+.B delete [\-s <config_server>] [\-f] component_name1 component_name2 ...
 delete components with given names
 .TP
-.B delete \-d [\-s <config_server>] [\-f] dsource_name1 dsource_name2 …
+.B delete \-d [\-s <config_server>] [\-f] dsource_name1 dsource_name2 ...
 delete datasources with given names
 .TP
-.B delete \-r [\-s <config_server>] [\-f] profile_name1 profile_name2 …
+.B delete \-r [\-s <config_server>] [\-f] profile_name1 profile_name2 ...
 delete profiles with given names
 .TP
-.B sources [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 …
+.B sources [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 ...
 get a list of component datasources
 .TP
-.B components [\-s <config_server>] [\-n] component_name1 component_name2 …
+.B components [\-s <config_server>] [\-n] component_name1 component_name2 ...
 get a list of dependent components
 .TP
-.B variables [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 …
+.B variables [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 ...
 get a list of component variables
 .TP
 .B data [\-s <config_server>] json_data
 set values of component variables
 .TP
 .B record [\-s <config_server>] [\-n] component_name1
 get a list of datasource record names from component
 .TP
 .B record \-d [\-s <config_server>] [\-n] datasource_name1
 get a list of datasource record names
 .TP
 .B servers [\-s <config_server/host>] [\-n]
 get lists of configuration servers from the current tango host
 .TP
-.B describe [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
+.B describe [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
 show all parameters of given components
 .TP
-.B describe|info \-d [\-s <config_server>] [\-n] dsource_name1 dsource_name2 …
+.B describe|info \-d [\-s <config_server>] [\-n] dsource_name1 dsource_name2 ...
 show all parameters of given datasources
 .TP
-.B info [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
+.B info [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
 show source parameters of given components
 .TP
-.B info \-r [\-s <config_server>]  [\-n] profile_name1 profile_name2 …
+.B info \-r [\-s <config_server>]  [\-n] profile_name1 profile_name2 ...
 show general parameters of given profiles
 .TP
-.B geometry [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
+.B geometry [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
 show transformation parameters of given components
 .UNINDENT
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-s \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-s \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.B \-d\fP,\fB  \-\-datasources
+.B  \-d\fP,\fB  \-\-datasources
 perform operation on datasources
 .TP
-.B \-m\fP,\fB  \-\-mandatory
+.B  \-m\fP,\fB  \-\-mandatory
 make use mandatory components as well
 .TP
-.B \-p\fP,\fB  \-\-private
-make use private components, i.e. starting with ‘__’
+.B  \-p\fP,\fB  \-\-private
+make use private components, i.e. starting with \(aq__\(aq
 .TP
-.B \-n\fP,\fB  \-\-no\-newlines
+.B  \-n\fP,\fB  \-\-no\-newlines
 split result with space characters
 .TP
-.B \-f\fP,\fB  \-\-force
+.B  \-f\fP,\fB  \-\-force
 do not ask
 .UNINDENT
 .UNINDENT
 .SH EXAMPLE
 .INDENT 0.0
 .INDENT 3.5
 .sp
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nxstools-3.9.0/man/nxscreate.1` & `nxstools-4.0.0/man/nxscreate.1`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSCREATE" "1" "Jun 08, 2021" "3.9" "NXSTools"
-.SH NAME
-nxscreate \- create NeXus Configuration component
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,14 +23,17 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "NXSCREATE" "1" "May 12, 2024" "4.0" "NXSTools"
+.SH NAME
+nxscreate \- create NeXus Configuration component
 .SH DESCRIPTION
 .sp
 The nxscreate program allows one to create simple datasources and components.
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -41,15 +41,15 @@
 .ft C
 nxscreate  <command> [ <options>]  [<arg1> [<arg2>  ...]]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-The following commands are available: clientds, tangods, deviceds, onlineds, onlinecp, comp.
+The following commands are available: clientds, tangods, deviceds, onlineds, onlinecp, poolds, stdcomp, comp, secopcp, compare.
 .SH NXSCREATE CLIENTDS
 .sp
 It creates a set of CLIENT datasources.
 .SS Synopsis
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -62,54 +62,54 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device\-prefix\fB= DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device\-prefix\fB= DEVICE
 device prefix, i.e. exp_c (mandatory w/o <name1>)
 .TP
-.BI \-f \ FIRST\fP,\fB \ \-\-first\fB= FIRST
+.BI \-f \ FIRST\fR,\fB \ \-\-first\fB= FIRST
 first index (mandatory w/o <name1>)
 .TP
-.BI \-l \ LAST\fP,\fB \ \-\-last\fB= LAST
+.BI \-l \ LAST\fR,\fB \ \-\-last\fB= LAST
 last index (mandatory w/o <name1>)
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing datasources
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-s \ DSOURCE\fP,\fB \ \-\-datasource\-prefix\fB= DSOURCE
+.BI \-s \ DSOURCE\fR,\fB \ \-\-datasource\-prefix\fB= DSOURCE
 datasource prefix, i.e. counter (useful for avoiding duplicated datasource names)
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.B \-m\fP,\fB  \-\-minimal_device
-device name without first ‘0’
+.B  \-m\fP,\fB  \-\-minimal_device
+device name without first \(aq0\(aq
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -139,71 +139,71 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
-default <datasource> is ‘exp_mot’
+default <datasource> is \(aqexp_mot\(aq
 .IP \(bu 2
 default <host>, <port> are taken from <server>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device\-prefix\fB= DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device\-prefix\fB= DEVICE
 device prefix, i.e. exp_c (mandatory)
 .TP
-.BI \-f \ FIRST\fP,\fB \ \-\-first\fB= FIRST
+.BI \-f \ FIRST\fR,\fB \ \-\-first\fB= FIRST
 first index
 .TP
-.BI \-l \ LAST\fP,\fB \ \-\-last\fB= LAST
+.BI \-l \ LAST\fR,\fB \ \-\-last\fB= LAST
 last index
 .TP
-.BI \-a \ ATTRIBUTE\fP,\fB \ \-\-attribute\fB= ATTRIBUTE
+.BI \-a \ ATTRIBUTE\fR,\fB \ \-\-attribute\fB= ATTRIBUTE
 tango attribute name
 .TP
-.BI \-s \ DATASOURCE\fP,\fB \ \-\-datasource\-prefix\fB= DATASOURCE
+.BI \-s \ DATASOURCE\fR,\fB \ \-\-datasource\-prefix\fB= DATASOURCE
 datasource\-prefix (useful for avoiding duplicated
 datasource names)
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing datasources
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-u \ HOST\fP,\fB \ \-\-host\fB= HOST
+.BI \-u \ HOST\fR,\fB \ \-\-host\fB= HOST
 tango host name
 .TP
-.BI \-t \ PORT\fP,\fB \ \-\-port\fB= PORT
+.BI \-t \ PORT\fR,\fB \ \-\-port\fB= PORT
 tango host port
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.BI \-g \ GROUP\fP,\fB \ \-\-group\fB= GROUP
+.BI \-g \ GROUP\fR,\fB \ \-\-group\fB= GROUP
 device group name
 .TP
-.BI \-e \ ELEMENTTYPE\fP,\fB \ \-\-elementtype\fB= ELEMENTTYPE
+.BI \-e \ ELEMENTTYPE\fR,\fB \ \-\-elementtype\fB= ELEMENTTYPE
 element type, i.e. attribute, property or command
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -237,56 +237,56 @@
 .IP \(bu 2
 without <dv_attr1>: datasources for all attributes are created
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
-default <datasource> is ‘exp_mot’
+default <datasource> is \(aqexp_mot\(aq
 .IP \(bu 2
 default <host>, <port> are taken from <server>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device\fB= DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device\fB= DEVICE
 device, i.e. p09/pilatus300k/01 (mandatory)
 .TP
-.BI \-o \ DATASOURCE\fP,\fB \ \-\-datasource\-prefix\fB= DATASOURCE
+.BI \-o \ DATASOURCE\fR,\fB \ \-\-datasource\-prefix\fB= DATASOURCE
 datasource\-prefix
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-s \ HOST\fP,\fB \ \-\-host\fB= HOST
+.BI \-s \ HOST\fR,\fB \ \-\-host\fB= HOST
 tango host name
 .TP
-.BI \-t \ PORT\fP,\fB \ \-\-port\fB= PORT
+.BI \-t \ PORT\fR,\fB \ \-\-port\fB= PORT
 tango host port
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.B \-n\fP,\fB  \-\-no\-group
-don’t create common group with a name of datasource
+.B  \-n\fP,\fB  \-\-no\-group
+don\(aqt create common group with a name of datasource
 prefix
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -317,53 +317,53 @@
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 with \-d <directory>: datasources are created on the local filesystem
 .IP \(bu 2
 without \-b or \-d <directory>: run in the test mode
 .IP \(bu 2
-default <inputFile> is ‘/online_dir/online.xml’
+default <inputFile> is \(aq/online_dir/online.xml\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .sp
 \fIonlineds\fP overwrites existing datasources
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store components in Configuration Server database
 .TP
-.B \-t\fP,\fB  \-\-noclientlike
+.B  \-t\fP,\fB  \-\-noclientlike
 set motor tango datasources to be non __CLIENT__ like
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output directory where datasources will be saved
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-e \ EXTERNAL\fP,\fB \ \-\-external\fB= EXTERNAL
+.BI \-e \ EXTERNAL\fR,\fB \ \-\-external\fB= EXTERNAL
 external configuration server
 .TP
-.BI \-p \ XMLPACKAGE\fP,\fB \ \-\-xml\-package\fB= XMLPACKAGE
+.BI \-p \ XMLPACKAGE\fR,\fB \ \-\-xml\-package\fB= XMLPACKAGE
 xml template package
 .TP
-.B \-\-verbose
+.B  \-\-verbose
 printout verbose mode
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -395,49 +395,49 @@
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 with \-d <directory>: datasources are created on the local filesystem
 .IP \(bu 2
 without \-b or \-d <directory>: run in the test mode
 .IP \(bu 2
-default <channel> is ‘ALL’
+default <channel> is \(aqALL\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
 default <pool> is taken from Tango DB
 .UNINDENT
 .sp
 \fIpoolds\fP overwrites existing datasources
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store components in Configuration Server database
 .TP
-.B \-t\fP,\fB  \-\-noclientlike
+.B  \-t\fP,\fB  \-\-noclientlike
 set motor tango datasources to be non __CLIENT__ like
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output directory where datasources will be saved
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-p \ POOL\fP,\fB \ \-\-pool\fB= POOL
+.BI \-p \ POOL\fR,\fB \ \-\-pool\fB= POOL
 sardana pool device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -466,78 +466,78 @@
 nxscreate onlinecp [options] inputFile
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-without ‘\-c <component>’: show a list of possible components
+without \(aq\-c <component>\(aq: show a list of possible components
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
-default <inputFile> is ‘/online_dir/online.xml’
+default <inputFile> is \(aq/online_dir/online.xml\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-c \ COMPONENT\fP,\fB \ \-\-component\fB= COMPONENT
+.BI \-c \ COMPONENT\fR,\fB \ \-\-component\fB= COMPONENT
 component namerelated to the device name from
 <inputFile>
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-t \ CPTYPE\fP,\fB \ \-\-type \ CPTYPE
+.BI \-t \ CPTYPE\fR,\fB \ \-\-type \ CPTYPE
 component type
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device \ DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device \ DEVICE
 device, i.e. p09/pilatus300k/01
 .TP
-.BI \-u \ HOST\fP,\fB \ \-\-host \ HOST
+.BI \-u \ HOST\fR,\fB \ \-\-host \ HOST
 tango host name
 .TP
-.BI \-w \ PORT\fP,\fB \ \-\-port \ PORT
+.BI \-w \ PORT\fR,\fB \ \-\-port \ PORT
 tango host port
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing component
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-e \ EXTERNAL\fP,\fB \ \-\-external\fB= EXTERNAL
+.BI \-e \ EXTERNAL\fR,\fB \ \-\-external\fB= EXTERNAL
 external configuration server
 .TP
-.BI \-p \ XMLPACKAGE\fP,\fB \ \-\-xml\-package\fB= XMLPACKAGE
+.BI \-p \ XMLPACKAGE\fR,\fB \ \-\-xml\-package\fB= XMLPACKAGE
 xml template package
 .TP
-.BI \-y \ ENTRYNAME\fP,\fB \ \-\-entryname \ ENTRYNAME
+.BI \-y \ ENTRYNAME\fR,\fB \ \-\-entryname \ ENTRYNAME
 entry group name (prefix)
 .TP
-.BI \-i \ INSNAME\fP,\fB \ \-\-insname \ INSNAME
+.BI \-i \ INSNAME\fR,\fB \ \-\-insname \ INSNAME
 instrument group name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -566,68 +566,68 @@
 nxscreate stdcomp [options] [name1 value1 [name2 value2] ...]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-without ‘\-t <type>’: show a list of possible component types
+without \(aq\-t <type>\(aq: show a list of possible component types
 .IP \(bu 2
-with ‘\-t <type>  and without \-c <component>: show a list of component variables for the given component type
+with \(aq\-t <type>  and without \-c <component>: show a list of component variables for the given component type
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
-[name1 value1 [name2 value2] …] sequence  defines component variable values
+[name1 value1 [name2 value2] ...] sequence  defines component variable values
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-c \ COMPONENT\fP,\fB \ \-\-component\fB= COMPONENT
+.BI \-c \ COMPONENT\fR,\fB \ \-\-component\fB= COMPONENT
 component name
 .TP
-.BI \-t \ CPTYPE\fP,\fB \ \-\-type\fB= CPTYPE
+.BI \-t \ CPTYPE\fR,\fB \ \-\-type\fB= CPTYPE
 component type
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-p \ XMLPACKAGE\fP,\fB \ \-\-xml\-package\fB= XMLPACKAGE
+.BI \-p \ XMLPACKAGE\fR,\fB \ \-\-xml\-package\fB= XMLPACKAGE
 xml template package
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing component
 .TP
-.B \-m\fP,\fB  \-\-mandatory
+.B  \-m\fP,\fB  \-\-mandatory
 set the component as mandatory
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-e \ EXTERNAL\fP,\fB \ \-\-external\fB= EXTERNAL
+.BI \-e \ EXTERNAL\fR,\fB \ \-\-external\fB= EXTERNAL
 external configuration server
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-y \ ENTRYNAME\fP,\fB \ \-\-entryname \ ENTRYNAME
+.BI \-y \ ENTRYNAME\fR,\fB \ \-\-entryname \ ENTRYNAME
 entry group name (prefix)
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -657,94 +657,233 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
 default <strategy> is step
 .IP \(bu 2
 default <type> is NX_FLOAT
 .IP \(bu 2
 default <chunk> is SCALAR
 .IP \(bu 2
-default <nexuspath> is “/$var.entryname#’scan’$var.serialno:NXentry/instrument/collection/”
+default <nexuspath> is \(dq/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/instrument/collection/\(dq
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device\-prefix\fB= DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device\-prefix\fB= DEVICE
 device prefix, i.e. exp_c
 .TP
-.BI \-f \ FIRST\fP,\fB \ \-\-first\fB= FIRST
+.BI \-f \ FIRST\fR,\fB \ \-\-first\fB= FIRST
 first index
 .TP
-.BI \-l \ LAST\fP,\fB \ \-\-last\fB= LAST
+.BI \-l \ LAST\fR,\fB \ \-\-last\fB= LAST
 last index
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing components
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output component directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-n \ NEXUSPATH\fP,\fB \ \-\-nexuspath\fB= NEXUSPATH
+.BI \-n \ NEXUSPATH\fR,\fB \ \-\-nexuspath\fB= NEXUSPATH
 nexus path with field name
 .TP
-.BI \-g \ STRATEGY\fP,\fB \ \-\-strategy\fB= STRATEGY
+.BI \-g \ STRATEGY\fR,\fB \ \-\-strategy\fB= STRATEGY
 writing strategy, i.e. STEP, INIT, FINAL, POSTRUN
 .TP
-.BI \-s \ DATASOURCE\fP,\fB \ \-\-datasource\-prefix \ DATASOURCE
+.BI \-s \ DATASOURCE\fR,\fB \ \-\-datasource\-prefix \ DATASOURCE
 datasource\-prefix or datasourcename
 .TP
-.BI \-t \ TYPE\fP,\fB \ \-\-type\fB= TYPE
+.BI \-t \ TYPE\fR,\fB \ \-\-type\fB= TYPE
 nexus type of the field
 .TP
-.BI \-u \ UNITS\fP,\fB \ \-\-units\fB= UNITS
+.BI \-u \ UNITS\fR,\fB \ \-\-units\fB= UNITS
 nexus units of the field
 .TP
-.B \-k\fP,\fB  \-\-links
+.B  \-k\fP,\fB  \-\-links
 create datasource links
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store components in Configuration Server database
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-c \ CHUNK\fP,\fB \ \-\-chunk\fB= CHUNK
+.BI \-c \ CHUNK\fR,\fB \ \-\-chunk\fB= CHUNK
 chunk format, i.e. SCALAR, SPECTRUM, IMAGE
 .TP
-.B \-m\fP,\fB  \-\-minimal_device
-device name without first ‘0’
+.B  \-m\fP,\fB  \-\-minimal_device
+device name without first \(aq0\(aq
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 nxscreate comp counter
 nxscreate comp \-f1 \-l3 \-v exp_c \-b
 nxscreate comp lambda \-d /home/user/xmldir/
-nxscreate comp \-n "/\e$var.entryname#\(aqscan\(aq\e$var.serialno:NXentry/instrument/sis3302:NXdetector/collection:NXcollection/\(aq \-v sis3302_1_roi \-f1 \-l4  \-g STEP \-t NX_FLOAT64 \-k \-b \-m
-nxscreate comp \-n "/\e$var.entryname#\(aqscan\(aq\e$var.serialno:NXentry/instrument/eh1_mca01:NXdetector/data" eh1_mca01 \-g STEP \-t NX_FLOAT64 \-i \-b \-c SPECTRUM
+nxscreate comp \-n \(dq/\e$var.entryname#\(aqscan\(aq\e$var.serialno:NXentry/instrument/sis3302:NXdetector/collection:NXcollection/\(aq \-v sis3302_1_roi \-f1 \-l4  \-g STEP \-t NX_FLOAT64 \-k \-b \-m
+nxscreate comp \-n \(dq/\e$var.entryname#\(aqscan\(aq\e$var.serialno:NXentry/instrument/eh1_mca01:NXdetector/data\(dq eh1_mca01 \-g STEP \-t NX_FLOAT64 \-i \-b \-c SPECTRUM
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SH NXSCREATE SECOPCP
+.sp
+It creates a  component or components describing modules of the secop node.
+.SS Synopsis
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxscreate secopcp [\-h] [\-l] [\-o] [\-a] [\-q] [\-w] [\-c COMPONENT] [\-e PARAMSTRATEGY] [\-g STRATEGY] [\-m TIMEOUT] [\-s SAMPLENAME] [\-s SAMPLEENVNAME] [\-k MEANINGS] [\-v ENVIRONMENTS] [\-f FIRST] [\-z TRANSATTRS] [\-p XMLPACKAGE] [\-y ENTRYNAME] [\-i INSNAME] [\-d DIRECTORY] [\-j JSON] [\-x FILE] [\-n] [\-b] [\-u HOST] [\-t PORT] [\-r SERVER] [component_name ...]
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.IP \(bu 2
+with \-b: datasources are created in Configuration Server database
+.IP \(bu 2
+without \-b: datasources are created on the local filesystem in \-d <directory>
+.IP \(bu 2
+default <port> is 5000
+.UNINDENT
+.INDENT 0.0
+.TP
+.B Options:
+.INDENT 7.0
+.TP
+.B  \-h\fP,\fB  \-\-help
+show this help message and exit
+.TP
+.B  \-l\fP,\fB  \-\-list
+list modules of the given node
+.TP
+.B  \-o\fP,\fB  \-\-overwrite
+overwrite existing components
+.TP
+.B  \-a\fP,\fB  \-\-can\-fail
+can fail strategy flag
+.TP
+.B  \-q\fP,\fB  \-\-dynamic
+create dynamic links
+.TP
+.B  \-\-sample\-nxdata
+create NXdata in NXsample
+.TP
+.BI \-c \ COMPONENT\fR,\fB \ \-\-component \ COMPONENT
+component namesecop component name
+.TP
+.BI \-e \ PARAMSTRATEGY\fR,\fB \ \-\-param\-strategy \ PARAMSTRATEGY
+sensor parameter strategy, i.e. INIT, STEP or FINAL, default: INIT
+.TP
+.BI \-g \ STRATEGY\fR,\fB \ \-\-strategy \ STRATEGY
+sensor value strategy, i.e. INIT, STEP or FINAL, default: INIT
+.TP
+.BI \-m \ TIMEOUT\fR,\fB \ \-\-timeout \ TIMEOUT
+sensor minimum timeout default: 0.001
+.TP
+.BI \-s \ SAMPLENAME\fR,\fB \ \-\-sample \ SAMPLENAME
+sample name
+.TP
+.BI \-w \ SAMPLEENVNAME\fR,\fB \ \-\-sample\-environment \ SAMPLEENVNAME
+sample environment name
+.TP
+.BI \-k \ MEANINGS\fR,\fB \ \-\-links \ MEANINGS
+NXlog links of physical quantities to sensors
+separated by comman. Default:
+\(aqtemperature,magnetic_field,electric_field,stress_field,pressure\(aq
+.TP
+.BI \-v \ ENVIRONMENTS\fR,\fB \ \-\-environments \ ENVIRONMENTS
+NXenvironment links of physical quantities separated
+by comman. Default: \(aqtemperature,magnetic_field\(aq
+.TP
+.BI \-f \ FIRST\fR,\fB \ \-\-first \ FIRST
+first linked targets separated by comman
+.TP
+.BI \-z \ TRANSATTRS\fR,\fB \ \-\-transformation\-attributes \ TRANSATTRS
+a JSON dictionary with transformation parameters i.e, \(dqtransformation_type\(dq, \(dqvector\(dq, \(dqdepends_on\(dq. Default:
+{\(dqrotation_z\(dq:{\(dqtransformation_type\(dq:\(dqrotation\(dq,\(dqvector\(dq:[0,\-1,0]}}
+.TP
+.BI \-p \ XMLPACKAGE\fR,\fB \ \-\-xml\-package \ XMLPACKAGE
+xml template package
+.TP
+.BI \-y \ ENTRYNAME\fR,\fB \ \-\-entryname \ ENTRYNAME
+entry group name (prefix)
+.TP
+.BI \-i \ INSNAME\fR,\fB \ \-\-insname \ INSNAME
+instrument group name
+.TP
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory \ DIRECTORY
+output component directory
+.TP
+.BI \-j \ JSON\fR,\fB \ \-\-json\-file \ JSON
+json configuration file
+.TP
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix \ FILE
+file prefix, i.e. counter
+.TP
+.B  \-n\fP,\fB  \-\-nolower
+do not change aliases into lower case
+.TP
+.B  \-b\fP,\fB  \-\-database
+store components in Configuration Server database
+.TP
+.BI \-u \ HOST\fR,\fB \ \-\-host \ HOST
+secop host name
+.TP
+.BI \-t \ PORT\fR,\fB \ \-\-port \ PORT
+secop host port
+.TP
+.BI \-r \ SERVER\fR,\fB \ \-\-server \ SERVER
+configuration server device name
+.UNINDENT
+.UNINDENT
+.SS Example
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxscreate secopcp
+nxscreate secopcp \-l
+
+    \- list all modules of the given node
+
+nxscreate secopcp \-c temp_node \-d . \-j secop_node.json
+
+    \- create the all secop components in the local directory for the node configured with the json file
+
+nxscreate secopcp T \-t 5001 \-b
+
+    \- create the component for the T secop module  in the NXSConfigServer database for the node on the port 5000
+
+nxscreate secopcp \-d /home/user/xmldir/
+
+    \- create the all secop components in the given directory
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SH NXSCREATE COMPARE
 .sp
 It compares two online.xml files
@@ -757,28 +896,28 @@
 nxscreate compare [\-h] [\-n] online_file [online_file]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-default: second <online_file> is ‘/online_dir/online.xml’ if only file is given
+default: second <online_file> is \(aq/online_dir/online.xml\(aq if only file is given
 .UNINDENT
 .INDENT 0.0
 .TP
 .B positional arguments:
 online_file    online.xml files
 .TP
 .B optional arguments:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nxstools-3.9.0/man/nxsdata.1` & `nxstools-4.0.0/man/nxsdata.1`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSDATA" "1" "Jun 08, 2021" "3.9" "NXSTools"
-.SH NAME
-nxsdata \- run NeXus Data Writer
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,14 +23,17 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "NXSDATA" "1" "May 12, 2024" "4.0" "NXSTools"
+.SH NAME
+nxsdata \- run NeXus Data Writer
 .SH DESCRIPTION
 .sp
 The nxsdata program is a command\-line interface to Nexus Data Tango Server.
 Program allows one to store NeXuS Data in H5 files.
 The writer provides storing data from other Tango devices, various databases
 as well as passed by a user client via JSON strings.
 .SH SYNOPSIS
@@ -73,18 +73,18 @@
 .B servers [\-s <nexus_server/host>]
 get lists of tango data servers from the current tango host
 .UNINDENT
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-s \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-s \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 tango data server device name
 .UNINDENT
 .UNINDENT
 .SH EXAMPLE
 .INDENT 0.0
 .INDENT 3.5
 .sp
```

### Comparing `nxstools-3.9.0/man/nxsetup.1` & `nxstools-4.0.0/man/nxsetup.1`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSETUP" "1" "Jun 08, 2021" "3.9" "NXSTools"
-.SH NAME
-nxsetup \- set NeXDaTaS Tango Server environment up
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,14 +23,17 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "NXSETUP" "1" "May 12, 2024" "4.0" "NXSTools"
+.SH NAME
+nxsetup \- set NeXDaTaS Tango Server environment up
 .SH DESCRIPTION
 .sp
 The nxsetup is is a command\-line setup tool for NeXus servers.  It allows to set NXSDataWriter, NXSConfigServer and NXSRecSelector in Tango environment, restart them or change property names.
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -63,51 +63,66 @@
 
 optional arguments:
   \-h, \-\-help            show this help message and exit
   \-b BEAMLINE, \-\-beamline BEAMLINE
                         name of the beamline ( default: \(aqnxs\(aq )
   \-m MASTERHOST, \-\-masterHost MASTERHOST
                         the host that stores the Mg ( default: <localhost> )
+  \-c CONFIGHOST, \-\-confighost CONFIGHOST
+                        the host to run the config server ( default: <mysqlhost> )
+  \-r RUNHOST, \-\-runhost RUNHOST
+                        the host to run the server ( default: localhost )
   \-u USER, \-\-user USER  the local user ( default: \(aqtango\(aq )
   \-d DBNAME, \-\-database DBNAME
                         the database name ( default: \(aqnxsconfig\(aq)
   \-j CSJSON, \-\-csjson CSJSON
                         JSONSettings for the configuration server. ( default:
-                        \(aq{"host": "localhost","db": <DBNAME>, "use_unicode":
-                        true\(aq, "read_default_file": <MY_CNF_FILE>}\(aq where
-                        <MY_CNF_FILE> stays for "/home/<USER>/.my.cnf" or
-                        "/var/lib/nxsconfigserver/.my.cnf" )
+                        \(aq{\(dqhost\(dq: \(dqlocalhost\(dq,\(dqdb\(dq: <DBNAME>, \(dquse_unicode\(dq:
+                        true\(aq, \(dqread_default_file\(dq: <MY_CNF_FILE>}\(aq where
+                        <MY_CNF_FILE> stays for \(dq/home/<USER>/.my.cnf\(dq or
+                        \(dq/var/lib/nxsconfigserver/.my.cnf\(dq )
+  \-k CLASSNAME, \-\-class\-name CLASSNAME
+                        tango server class name
+  \-y PROPJSON, \-\-json\-device\-properties PROPJSON
+                        JSON tango device properties ( default: \(aq{}\(aq )
+  \-t, \-\-postpone        do not start the server
 
  examples:
        nxsetup set
        nxsetup set \-b p09 \-m haso228 \-u p09user \-d nxsconfig NXSConfigServer
+       nxsetup set NexusWriter/haso228  \-k NexusWriter  \-y \(aq{\(dqp00/bliss_nexuswriter/test_session\(dq:{\(dqsession\(dq:\(dqtest_session\(dq,\(dqbeacon_host\(dq:\(dqhaso228:25000\(dq}}\(aq  \-t
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SH NXSETUP RESTART
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-usage: nxsetup restart [\-h] [\-l LEVEL] [server_name [server_name ...]]
+   usage: nxsetup restart [\-h] [\-l LEVEL] [server_name [server_name ...]]
 
-restart tango server
+   restart tango server
 
-positional arguments:
-  server_name           server names, e.g.: NXSRecSelector NXSDataWriter/TDW1
+   positional arguments:
+     server_name           server names, e.g.: NXSRecSelector NXSDataWriter/TDW1
 
-optional arguments:
-  \-h, \-\-help            show this help message and exit
-  \-l LEVEL, \-\-level LEVEL
-                        startup level
+   optional arguments:
+     \-h, \-\-help            show this help message and exit
+     \-l LEVEL, \-\-level LEVEL
+                           startup level
+     \-z TIMEOUT, \-\-timeout TIMEOUT
+                           timeout in seconds
+     \-e, \-\-no\-wait         do not wait
 
- examples:
-       nxsetup restart Pool/haso228 \-l 2
+examples:
+
+    examples:
+          nxsetup restart Pool/haso228 \-l 2
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SH NXSETUP START
 .INDENT 0.0
 .INDENT 3.5
@@ -121,14 +136,17 @@
 positional arguments:
   server_name           server names, e.g.: NXSRecSelector NXSDataWriter/TDW1
 
 optional arguments:
   \-h, \-\-help            show this help message and exit
   \-l LEVEL, \-\-level LEVEL
                         startup level
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+  \-e, \-\-no\-wait         do not wait
 
  examples:
        nxsetup start Pool/haso228 \-l 2
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
@@ -150,14 +168,39 @@
 
  examples:
        nxsetup stop Pool/haso228
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
+.SH NXSETUP WAIT
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+usage: nxsetup wait [\-h] [server_name [server_name ...]]
+
+stop tango server
+
+positional arguments:
+  server_name           server names, e.g.: NXSRecSelector NXSDataWriter/TDW1
+
+optional arguments:
+  \-h, \-\-help            show this help message and exit
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+
+
+ examples:
+       nxsetup wait Pool/haso228
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
 .SH NXSETUP MOVE-PROP
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 usage: nxsetup move\-prop [\-h] [\-n NEWNAME] [\-o OLDNAME]
@@ -171,14 +214,17 @@
 optional arguments:
   \-h, \-\-help            show this help message and exit
   \-n NEWNAME, \-\-newname NEWNAME
                         (new) property name
   \-o OLDNAME, \-\-oldname OLDNAME
                         old property name
   \-t, \-\-postpone        do not restart the server
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+  \-e, \-\-no\-wait         do not wait
 
  examples:
        nxsetup move\-prop \-n DefaultPreselectedComponents \-o DefaultAutomaticComponents NXSRecSelector
        nxsetup move\-prop \-t \-n DefaultPreselectedComponents  \-o DefaultAutomaticComponents NXSRecSelector
 .ft P
 .fi
 .UNINDENT
@@ -200,20 +246,23 @@
 optional arguments:
   \-h, \-\-help            show this help message and exit
   \-n NEWNAME, \-\-newname NEWNAME
                         (new) property name
   \-w PROPVALUE, \-\-propvalue PROPVALUE
                         new property value
   \-t, \-\-postpone        do not restart the server
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+  \-e, \-\-no\-wait         do not wait
 
 
  examples:
-       nxsetup change\-prop \-n ClientRecordKeys \-t \-w "[\e"phoibos_scan_command\e",\e"phoibos_scan_comment\e"]" NXSRecSelector/r228
-       nxsetup change\-prop \-n DefaultPreselectedComponents \-w "[\e"pinhole1\e",\e"slit2\e"]" NXSRecSelector/r228
-       nxsetup change\-prop \-n StartDsPath \-w "[\e"/usr/bin\e",\e"/usr/lib/tango\e"]" Starter
+       nxsetup change\-prop \-n ClientRecordKeys \-t \-w \(dq[\e\(dqphoibos_scan_command\e\(dq,\e\(dqphoibos_scan_comment\e\(dq]\(dq NXSRecSelector/r228
+       nxsetup change\-prop \-n DefaultPreselectedComponents \-w \(dq[\e\(dqpinhole1\e\(dq,\e\(dqslit2\e\(dq]\(dq NXSRecSelector/r228
+       nxsetup change\-prop \-n StartDsPath \-w \(dq[\e\(dq/usr/bin\e\(dq,\e\(dq/usr/lib/tango\e\(dq]\(dq Starter
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SH NXSETUP ADD-RECORDER-PATH
 .INDENT 0.0
 .INDENT 3.5
@@ -226,14 +275,19 @@
 
 positional arguments:
   recorder_path  sardana recorder path
 
 optional arguments:
   \-h, \-\-help     show this help message and exit
   \-t, \-\-postpone  do not restart the server
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+  \-e, \-\-no\-wait         do not wait
+  \-i INSTANCE, \-\-instance INSTANCE
+                        macroserver instance name, i.e. haso ( default: \(aq*\(aq)
  examples:
        nxsetup add\-recorder\-path /usr/share/pyshared/sardananxsrecorder
        nxsetup add\-recorder\-path \-t /usr/share/pyshared/sardananxsrecorder
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
```

### Comparing `nxstools-3.9.0/man/nxstools.1` & `nxstools-4.0.0/man/nxstools.1`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 .\" Man page generated from reStructuredText.
 .
-.TH "NXSTOOLS" "1" "Jun 08, 2021" "3.9" "NXSTools"
-.SH NAME
-nxstools \- nxstools Documentation
 .
 .nr rst2man-indent-level 0
 .
 .de1 rstReportMargin
 \\$1 \\n[an-margin]
 level \\n[rst2man-indent-level]
 level margin: \\n[rst2man-indent\\n[rst2man-indent-level]]
@@ -26,14 +23,22 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
+.TH "NXSTOOLS" "1" "May 12, 2024" "4.0" "NXSTools"
+.SH NAME
+nxstools \- nxstools Documentation
+.sp
+\fI\%\fP
+\fI\%\fP
+\fI\%\fP
+\fI\%\fP
 .sp
 Authors: Jan Kotanski
 .SH INTRODUCTION
 .sp
 Configuration tools for NeXDaTaS Tango Servers consists of the following command\-line scripts:
 .INDENT 0.0
 .IP \(bu 2
@@ -41,39 +46,39 @@
 .IP \(bu 2
 \fI\%nxsconfig\fP reads NeXus Configuration Server settings
 .IP \(bu 2
 \fI\%nxscreate\fP creates NeXus Configuration components
 .IP \(bu 2
 \fI\%nxsdata\fP runs NeXus Data Writer
 .IP \(bu 2
-\fI\%nxsfileinfo\fP shows nedadata of the NeXus/HDF5 file
+\fI\%nxsfileinfo\fP shows metadata of the NeXus/HDF5 file
 .IP \(bu 2
 \fI\%nxsetup\fP setups NeXDaTaS Tango Server environment
 .UNINDENT
 .sp
 as well as the \fI\%nxstools\fP package which allows perform these operations
 directly from a python code.
 .nf
-Source code: \fI\%https://github.com/nexdatas/tools\fP
-Web page: \fI\%https://nexdatas.github.io/tools\fP
+Source code: \fI\%https://github.com/nexdatas/nxstools\fP
+Web page: \fI\%https://nexdatas.github.io/nxstools\fP
 NexDaTaS Web page: \fI\%https://nexdatas.github.io\fP
 .fi
 .sp
 .SH INSTALLATION
 .sp
 Install the dependencies:
 .nf
-PyTango, sphinx
+pninexus or h5py, numpy, tango, sphinx
 .fi
 .sp
 .SS From sources
 .sp
 Download the latest NXS Tools version from
 .nf
-\fI\%https://github.com/nexdatas/tools\fP
+\fI\%https://github.com/nexdatas/nxstools\fP
 .fi
 .sp
 .sp
 Extract sources and run
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -82,120 +87,98 @@
 $ python setup.py install
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS Debian packages
 .sp
-Debian \fIstretch\fP, \fIjessie\fP (and \fIwheezy\fP)  or Ubuntu \fIbionic\fP (and \fIxenial\fP) packages can be found in the HDRI repository.
+Debian \fIbookworm\fP, \fIbullseye\fP, \fIbuster\fP  or Ubuntu \fIlunar\fP, \fIjammy\fP, \fIfocal\fP packages can be found in the HDRI repository.
 .sp
 To install the debian packages, add the PGP repository key
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 $ sudo su
-$ wget \-q \-O \- http://repos.pni\-hdri.de/debian_repo.pub.gpg | apt\-key add \-
+$ curl \-s http://repos.pni\-hdri.de/debian_repo.pub.gpg | gpg \-\-no\-default\-keyring \-\-keyring gnupg\-ring:/etc/apt/trusted.gpg.d/debian\-hdri\-repo.gpg \-\-import
+$ chmod 644 /etc/apt/trusted.gpg.d/debian\-hdri\-repo.gpg
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
 and then download the corresponding source list
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 $ cd /etc/apt/sources.list.d
-$ wget http://repos.pni\-hdri.de/stretch\-pni\-hdri.list
+$ wget http://repos.pni\-hdri.de/bookworm\-pni\-hdri.list
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-For releases (>= 2.61.0) to insall python2 scripts
+To install nxstools scripts
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 $ apt\-get update
 $ apt\-get install nxstools
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-and for python3 scripts
+or
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 $ apt\-get update
 $ apt\-get install nxstools3
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-For older releases
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-$ apt\-get update
-$ apt\-get install python\-nxstools
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
+for older python3 releases.
 .sp
-and
+To install only the python3 package
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
+$ apt\-get update
 $ apt\-get install python3\-nxstools
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-if exists.
-.sp
-To instal other NexDaTaS packages
+and for python2
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-$ apt\-get install python\-nxswriter nxsconfigserver\-db python\-nxsconfigserver nxsconfigtool
-.ft P
-.fi
-.UNINDENT
-.UNINDENT
-.sp
-and
-.INDENT 0.0
-.INDENT 3.5
-.sp
-.nf
-.ft C
-$ apt\-get install python\-nxsrecselector nxselector python\-sardana\-nxsrecorder
+$ apt\-get update
+$ apt\-get install python\-nxstools
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-for Component Selector and Sardana related packages.
+if exists.
 .SS From pip
 .sp
 To install it from pip you can
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -248,55 +231,55 @@
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-c \ COMPRESSION\fP,\fB \ \-\-compression \ COMPRESSION
+.BI \-c \ COMPRESSION\fR,\fB \ \-\-compression \ COMPRESSION
 deflate compression rate from 0 to 9 (default: 2) or
-<filterid>:opt1,opt2,… e.g. \-c 32008:0,2 for
+<filterid>:opt1,opt2,... e.g. \-c 32008:0,2 for
 bitshuffle with lz4
 .TP
-.BI \-p \ PATH\fP,\fB \ \-\-path \ PATH
+.BI \-p \ PATH\fR,\fB \ \-\-path \ PATH
 nexus path for the output field, e.g.
 /scan/instrument/pilatus/data
 .TP
-.BI \-i \ INPUTFILES\fP,\fB \ \-\-input_files \ INPUTFILES
+.BI \-i \ INPUTFILES\fR,\fB \ \-\-input_files \ INPUTFILES
 input data files defined with a pattern or separated
-by ‘,’ e.g.’scan_%05d.tif:0:100’
+by \(aq,\(aq e.g.\(aqscan_%05d.tif:0:100\(aq
 .TP
 .BI \-\-separator \ SEPARATOR
-input data files separator (default: ‘,’)
+input data files separator (default: \(aq,\(aq)
 .TP
 .BI \-\-dtype \ DATATYPE
 datatype of input data \- only for raw data, e.g.
-‘uint8’
+\(aquint8\(aq
 .TP
 .BI \-\-shape \ SHAPE
 shape of input data \- only for raw data, e.g.
-‘[4096,2048]’
+\(aq[4096,2048]\(aq
 .TP
-.B \-s\fP,\fB  \-\-skip_missing
+.B  \-s\fP,\fB  \-\-skip_missing
 skip missing files
 .TP
-.B \-r\fP,\fB  \-\-replace_nexus_file
+.B  \-r\fP,\fB  \-\-replace_nexus_file
 if it is set the old file is not copied into a file
 with .__nxscollect__old__* extension
 .TP
-.B \-\-test
+.B  \-\-test
 execute in the test mode
 .TP
-.B \-\-h5py
+.B  \-\-h5py
 use h5py module as a nexus reader/writer
 .TP
-.B \-\-h5cpp
+.B  \-\-h5cpp
 use h5cpp module as a nexus reader/writer
 .UNINDENT
 .UNINDENT
 .SS Examples of nxscollect append
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -329,34 +312,34 @@
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-n \ NAME\fP,\fB \ \-\-name \ NAME
+.BI \-n \ NAME\fR,\fB \ \-\-name \ NAME
 link name
 .TP
-.BI \-t \ TARGET\fP,\fB \ \-\-target \ TARGET
+.BI \-t \ TARGET\fR,\fB \ \-\-target \ TARGET
 link target with the file name if external
 .TP
-.B \-r\fP,\fB  \-\-replace_nexus_file
+.B  \-r\fP,\fB  \-\-replace_nexus_file
 if it is set the old file is not copied into a file
 with .__nxscollect__old__* extension
 .TP
-.B \-\-test
+.B  \-\-test
 execute in the test mode
 .TP
-.B \-\-h5py
+.B  \-\-h5py
 use h5py module as a nexus reader/writer
 .TP
-.B \-\-h5cpp
+.B  \-\-h5cpp
 use h5cpp module as a nexus reader
 .UNINDENT
 .UNINDENT
 .SS Examples of nxscollect link
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -392,124 +375,124 @@
 nexus_file_path_field    nexus files with the nexus directory and a field name  to create the VDS field
 .sp
 Options:
 .INDENT 0.0
 .INDENT 3.5
 .INDENT 0.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-t \ DTYPE\fP,\fB \ \-\-dtype \ DTYPE
-datatype of the VDS field, e.g. ‘uint8’
+.BI \-t \ DTYPE\fR,\fB \ \-\-dtype \ DTYPE
+datatype of the VDS field, e.g. \(aquint8\(aq
 .TP
-.BI \-s \ SHAPE\fP,\fB \ \-\-shape \ SHAPE
-shape of the VDS field, e.g. ‘[U,4096,2048]’ or
-U,4096,2048 where U means span along the field’
+.BI \-s \ SHAPE\fR,\fB \ \-\-shape \ SHAPE
+shape of the VDS field, e.g. \(aq[U,4096,2048]\(aq or
+U,4096,2048 where U means span along the field\(aq
 .TP
-.BI \-f \ FILLVALUE\fP,\fB \ \-\-fill\-value \ FILLVALUE
+.BI \-f \ FILLVALUE\fR,\fB \ \-\-fill\-value \ FILLVALUE
 fill value for the gaps, default is 0
 .TP
-.BI \-e \ TARGETFIELDS\fP,\fB \ \-\-target\-fields \ TARGETFIELDS
+.BI \-e \ TARGETFIELDS\fR,\fB \ \-\-target\-fields \ TARGETFIELDS
 external fields with their NeXus file paths defined
-with a pattern or separated by ‘,’
-e.g.’scan_123/lambda_%05d.nxs://entry/data/\fI\%data:0:3\fP’
+with a pattern or separated by \(aq,\(aq
+e.g.\(aqscan_123/lambda_%05d.nxs://entry/data/\fI\%data:0:3\fP\(aq
 .TP
 .BI \-\-separator \ SEPARATOR
-input data files separator (default: ‘,’)
+input data files separator (default: \(aq,\(aq)
 .TP
-.BI \-p \ SHAPES\fP,\fB \ \-\-shapes \ SHAPES
+.BI \-p \ SHAPES\fR,\fB \ \-\-shapes \ SHAPES
 shapes in the VDS layout hyperslab for the
 corresponding target fields with coordinates sepatated
-by ‘,’ and different fields separated by ‘;’, ‘:’ or
-spaces e.g.’,,;,300,;,600,0’ where an empty coordinate
+by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
+spaces e.g.\(aq,,;,300,;,600,0\(aq where an empty coordinate
 means 0
 .TP
-.BI \-o \ OFFSETS\fP,\fB \ \-\-offsets \ OFFSETS
+.BI \-o \ OFFSETS\fR,\fB \ \-\-offsets \ OFFSETS
 offsets in the VDS layout hyperslab for the
 corresponding target fields with coordinates sepatated
-by ‘,’ and different fields separated by ‘;’, ‘:’ or
-spaces e.g.’,,;,300,;,600,0’ where an empty coordinate
+by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
+spaces e.g.\(aq,,;,300,;,600,0\(aq where an empty coordinate
 means 0
 .TP
-.BI \-b \ BLOCKS\fP,\fB \ \-\-blocks \ BLOCKS
+.BI \-b \ BLOCKS\fR,\fB \ \-\-blocks \ BLOCKS
 block sizes in the VDS layout hyperslab for the
 corresponding target fields with coordinates sepatated
-by ‘,’ and different fields separated by ‘;’, ‘:’ or
-spaces e.g. ‘,256,512;,256,512;,256,512’ where an
+by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
+spaces e.g. \(aq,256,512;,256,512;,256,512\(aq where an
 empty coordinate means 1
 .TP
-.BI \-c \ COUNTS\fP,\fB \ \-\-counts \ COUNTS
+.BI \-c \ COUNTS\fR,\fB \ \-\-counts \ COUNTS
 count numbers in the VDS layout hyperslabfor the
 corresponding target fields with coordinates sepatated
-by ‘,’ and different fields separated by ‘;’, ‘:’ or
-spaces e.g. ‘,1,1;,1,1;,1,1’ where an empty coordinate
+by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
+spaces e.g. \(aq,1,1;,1,1;,1,1\(aq where an empty coordinate
 means span along the layout
 .TP
-.BI \-d \ STRIDES\fP,\fB \ \-\-strides \ STRIDES
+.BI \-d \ STRIDES\fR,\fB \ \-\-strides \ STRIDES
 stride sizes in the VDS layout hyperslabfor the
 corresponding target fields with coordinates sepatated
-by ‘,’ and different fields separated by ‘;’, ‘:’ or
-spaces e.g. ‘,,;,,;,,’ where an empty coordinate means
+by \(aq,\(aq and different fields separated by \(aq;\(aq, \(aq:\(aq or
+spaces e.g. \(aq,,;,,;,,\(aq where an empty coordinate means
 1
 .TP
-.BI \-l \ SLICES\fP,\fB \ \-\-slices \ SLICES
+.BI \-l \ SLICES\fR,\fB \ \-\-slices \ SLICES
 mapping slices in the VDS layoutfor the corresponding
-target fields with coordinates sepatated by ‘,’ and
-different fields separated by ‘;’ or spaces e.g.
-‘:,0:50,: :,50:100,:’ where U means span along the
+target fields with coordinates sepatated by \(aq,\(aq and
+different fields separated by \(aq;\(aq or spaces e.g.
+\(aq:,0:50,: :,50:100,:\(aq where U means span along the
 layout
 .TP
-.BI \-P \ TARGETSHAPES\fP,\fB \ \-\-target\-shapes \ TARGETSHAPES
-field shapes with coordinates sepatated by ‘,’ and
-different fields separated by ‘;’, ‘:’ or spaces
-e.g.’,,;,300,;,600,0’
+.BI \-P \ TARGETSHAPES\fR,\fB \ \-\-target\-shapes \ TARGETSHAPES
+field shapes with coordinates sepatated by \(aq,\(aq and
+different fields separated by \(aq;\(aq, \(aq:\(aq or spaces
+e.g.\(aq,,;,300,;,600,0\(aq
 .TP
-.BI \-O \ TARGETOFFSETS\fP,\fB \ \-\-target\-offsets \ TARGETOFFSETS
+.BI \-O \ TARGETOFFSETS\fR,\fB \ \-\-target\-offsets \ TARGETOFFSETS
 offsets in the view hyperslab of target fieldswith
-coordinates sepatated by ‘,’ and different fields
-separated by ‘;’, ‘:’ or spaces e.g.’,,;,300,;,600,0’
+coordinates sepatated by \(aq,\(aq and different fields
+separated by \(aq;\(aq, \(aq:\(aq or spaces e.g.\(aq,,;,300,;,600,0\(aq
 where an empty coordinate means 0
 .TP
-.BI \-B \ TARGETBLOCKS\fP,\fB \ \-\-target\-blocks \ TARGETBLOCKS
+.BI \-B \ TARGETBLOCKS\fR,\fB \ \-\-target\-blocks \ TARGETBLOCKS
 block sizes in the view hyperslab of target fields
-with coordinates sepatated by ‘,’ and different fields
-separated by ‘;’, ‘:’ or spaces e.g.
-‘,256,512;,256,512;,256,512’ where an empty coordinate
+with coordinates sepatated by \(aq,\(aq and different fields
+separated by \(aq;\(aq, \(aq:\(aq or spaces e.g.
+\(aq,256,512;,256,512;,256,512\(aq where an empty coordinate
 means 1
 .TP
-.BI \-C \ TARGETCOUNTS\fP,\fB \ \-\-target\-counts \ TARGETCOUNTS
+.BI \-C \ TARGETCOUNTS\fR,\fB \ \-\-target\-counts \ TARGETCOUNTS
 count numbers in the view hyperslab of target fields
-with coordinates sepatated by ‘,’ and different fields
-separated by ‘;’, ‘:’ or spaces e.g. ‘,1,1;,1,1;,1,1’
+with coordinates sepatated by \(aq,\(aq and different fields
+separated by \(aq;\(aq, \(aq:\(aq or spaces e.g. \(aq,1,1;,1,1;,1,1\(aq
 where an empty coordinate means span along the layout
 .TP
-.BI \-D \ TARGETSTRIDES\fP,\fB \ \-\-target\-strides \ TARGETSTRIDES
+.BI \-D \ TARGETSTRIDES\fR,\fB \ \-\-target\-strides \ TARGETSTRIDES
 stride sizes numbers in the view hyperslab of target
-fields with coordinates sepatated by ‘,’ and different
-fields separated by ‘;’, ‘:’ or spaces e.g. ‘,,;,,;,,’
+fields with coordinates sepatated by \(aq,\(aq and different
+fields separated by \(aq;\(aq, \(aq:\(aq or spaces e.g. \(aq,,;,,;,,\(aq
 where an empty coordinate means 1
 .TP
-.BI \-L \ TARGETSLICES\fP,\fB \ \-\-target\-slices \ TARGETSLICES
+.BI \-L \ TARGETSLICES\fR,\fB \ \-\-target\-slices \ TARGETSLICES
 view slices of target fields with coordinates
-sepatated by ‘,’ and different fields separated by ‘;’
-or spaces e.g. ‘:,0:50,: :,0:50,:’ where U means span
+sepatated by \(aq,\(aq and different fields separated by \(aq;\(aq
+or spaces e.g. \(aq:,0:50,: :,0:50,:\(aq where U means span
 along the layout
 .TP
-.B \-r\fP,\fB  \-\-replace\-nexus\-file
+.B  \-r\fP,\fB  \-\-replace\-nexus\-file
 if it is set the old file is not copied into a file
 with .__nxscollect__old__* extension
 .TP
-.B \-\-test
+.B  \-\-test
 execute in the test mode
 .TP
-.B \-\-h5cpp
+.B  \-\-h5cpp
 use h5cpp module as a nexus reader
 .TP
-.B \-\-h5py
+.B  \-\-h5py
 use h5py module as a nexus reader/writer
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .SS Examples of nxscollect vds
 .INDENT 0.0
 .INDENT 3.5
@@ -563,103 +546,103 @@
 .TP
 .B list \-d [\-s <config_server>] [\-n]
 list names of available datasources
 .TP
 .B list \-r [\-s <config_server>] [\-n]
 list names of available profiles
 .TP
-.B show [\-s <config_server>] [\-m] [\-o <dir>] component_name1 component_name2 …
+.B show [\-s <config_server>] [\-m] [\-o <dir>] component_name1 component_name2 ...
 show components with given names
 .TP
-.B show \-d [\-s <config_server>]  [\-o <dir>] dsource_name1 dsource_name2 …
+.B show \-d [\-s <config_server>]  [\-o <dir>] dsource_name1 dsource_name2 ...
 show datasources with given names
 .TP
-.B show \-r [\-s <config_server>]  [\-o <dir>] profile_name1 profile_name2 …
+.B show \-r [\-s <config_server>]  [\-o <dir>] profile_name1 profile_name2 ...
 show profiles with given names
 .TP
-.B upload [\-s <config_server>] [\-m] [\-i <dir>] [\-f] component_name1 component_name2 …
+.B upload [\-s <config_server>] [\-m] [\-i <dir>] [\-f] component_name1 component_name2 ...
 load components from given files
 .TP
-.B upload \-d [\-s <config_server>]  [\-i <dir>] [\-f] dsource_name1 dsource_name2 …
+.B upload \-d [\-s <config_server>]  [\-i <dir>] [\-f] dsource_name1 dsource_name2 ...
 load datasources from given files
 .TP
-.B upload \-r [\-s <config_server>]  [\-i <dir>] [\-f] profile_name1 profile_name2 …
+.B upload \-r [\-s <config_server>]  [\-i <dir>] [\-f] profile_name1 profile_name2 ...
 load profiles from given files
 .TP
-.B get [\-s <config_server>]  [\-n] component_name1 component_name2 …
+.B get [\-s <config_server>]  [\-n] component_name1 component_name2 ...
 get merged configuration of components
 .TP
-.B delete [\-s <config_server>] [\-f] component_name1 component_name2 …
+.B delete [\-s <config_server>] [\-f] component_name1 component_name2 ...
 delete components with given names
 .TP
-.B delete \-d [\-s <config_server>] [\-f] dsource_name1 dsource_name2 …
+.B delete \-d [\-s <config_server>] [\-f] dsource_name1 dsource_name2 ...
 delete datasources with given names
 .TP
-.B delete \-r [\-s <config_server>] [\-f] profile_name1 profile_name2 …
+.B delete \-r [\-s <config_server>] [\-f] profile_name1 profile_name2 ...
 delete profiles with given names
 .TP
-.B sources [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 …
+.B sources [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 ...
 get a list of component datasources
 .TP
-.B components [\-s <config_server>] [\-n] component_name1 component_name2 …
+.B components [\-s <config_server>] [\-n] component_name1 component_name2 ...
 get a list of dependent components
 .TP
-.B variables [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 …
+.B variables [\-s <config_server>] [\-m] [\-n] component_name1 component_name2 ...
 get a list of component variables
 .TP
 .B data [\-s <config_server>] json_data
 set values of component variables
 .TP
 .B record [\-s <config_server>] [\-n] component_name1
 get a list of datasource record names from component
 .TP
 .B record \-d [\-s <config_server>] [\-n] datasource_name1
 get a list of datasource record names
 .TP
 .B servers [\-s <config_server/host>] [\-n]
 get lists of configuration servers from the current tango host
 .TP
-.B describe [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
+.B describe [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
 show all parameters of given components
 .TP
-.B describe|info \-d [\-s <config_server>] [\-n] dsource_name1 dsource_name2 …
+.B describe|info \-d [\-s <config_server>] [\-n] dsource_name1 dsource_name2 ...
 show all parameters of given datasources
 .TP
-.B info [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
+.B info [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
 show source parameters of given components
 .TP
-.B info \-r [\-s <config_server>]  [\-n] profile_name1 profile_name2 …
+.B info \-r [\-s <config_server>]  [\-n] profile_name1 profile_name2 ...
 show general parameters of given profiles
 .TP
-.B geometry [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 …
+.B geometry [\-s <config_server>] [\-m | \-p] [\-n] component_name1 component_name2 ...
 show transformation parameters of given components
 .UNINDENT
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-s \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-s \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.B \-d\fP,\fB  \-\-datasources
+.B  \-d\fP,\fB  \-\-datasources
 perform operation on datasources
 .TP
-.B \-m\fP,\fB  \-\-mandatory
+.B  \-m\fP,\fB  \-\-mandatory
 make use mandatory components as well
 .TP
-.B \-p\fP,\fB  \-\-private
-make use private components, i.e. starting with ‘__’
+.B  \-p\fP,\fB  \-\-private
+make use private components, i.e. starting with \(aq__\(aq
 .TP
-.B \-n\fP,\fB  \-\-no\-newlines
+.B  \-n\fP,\fB  \-\-no\-newlines
 split result with space characters
 .TP
-.B \-f\fP,\fB  \-\-force
+.B  \-f\fP,\fB  \-\-force
 do not ask
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -684,15 +667,15 @@
 .ft C
 nxscreate  <command> [ <options>]  [<arg1> [<arg2>  ...]]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-The following commands are available: clientds, tangods, deviceds, onlineds, onlinecp, comp.
+The following commands are available: clientds, tangods, deviceds, onlineds, onlinecp, poolds, stdcomp, comp, secopcp, compare.
 .SS nxscreate clientds
 .sp
 It creates a set of CLIENT datasources.
 .SS Synopsis
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -705,54 +688,54 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device\-prefix\fB= DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device\-prefix\fB= DEVICE
 device prefix, i.e. exp_c (mandatory w/o <name1>)
 .TP
-.BI \-f \ FIRST\fP,\fB \ \-\-first\fB= FIRST
+.BI \-f \ FIRST\fR,\fB \ \-\-first\fB= FIRST
 first index (mandatory w/o <name1>)
 .TP
-.BI \-l \ LAST\fP,\fB \ \-\-last\fB= LAST
+.BI \-l \ LAST\fR,\fB \ \-\-last\fB= LAST
 last index (mandatory w/o <name1>)
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing datasources
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-s \ DSOURCE\fP,\fB \ \-\-datasource\-prefix\fB= DSOURCE
+.BI \-s \ DSOURCE\fR,\fB \ \-\-datasource\-prefix\fB= DSOURCE
 datasource prefix, i.e. counter (useful for avoiding duplicated datasource names)
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.B \-m\fP,\fB  \-\-minimal_device
-device name without first ‘0’
+.B  \-m\fP,\fB  \-\-minimal_device
+device name without first \(aq0\(aq
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -782,71 +765,71 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
-default <datasource> is ‘exp_mot’
+default <datasource> is \(aqexp_mot\(aq
 .IP \(bu 2
 default <host>, <port> are taken from <server>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device\-prefix\fB= DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device\-prefix\fB= DEVICE
 device prefix, i.e. exp_c (mandatory)
 .TP
-.BI \-f \ FIRST\fP,\fB \ \-\-first\fB= FIRST
+.BI \-f \ FIRST\fR,\fB \ \-\-first\fB= FIRST
 first index
 .TP
-.BI \-l \ LAST\fP,\fB \ \-\-last\fB= LAST
+.BI \-l \ LAST\fR,\fB \ \-\-last\fB= LAST
 last index
 .TP
-.BI \-a \ ATTRIBUTE\fP,\fB \ \-\-attribute\fB= ATTRIBUTE
+.BI \-a \ ATTRIBUTE\fR,\fB \ \-\-attribute\fB= ATTRIBUTE
 tango attribute name
 .TP
-.BI \-s \ DATASOURCE\fP,\fB \ \-\-datasource\-prefix\fB= DATASOURCE
+.BI \-s \ DATASOURCE\fR,\fB \ \-\-datasource\-prefix\fB= DATASOURCE
 datasource\-prefix (useful for avoiding duplicated
 datasource names)
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing datasources
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-u \ HOST\fP,\fB \ \-\-host\fB= HOST
+.BI \-u \ HOST\fR,\fB \ \-\-host\fB= HOST
 tango host name
 .TP
-.BI \-t \ PORT\fP,\fB \ \-\-port\fB= PORT
+.BI \-t \ PORT\fR,\fB \ \-\-port\fB= PORT
 tango host port
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.BI \-g \ GROUP\fP,\fB \ \-\-group\fB= GROUP
+.BI \-g \ GROUP\fR,\fB \ \-\-group\fB= GROUP
 device group name
 .TP
-.BI \-e \ ELEMENTTYPE\fP,\fB \ \-\-elementtype\fB= ELEMENTTYPE
+.BI \-e \ ELEMENTTYPE\fR,\fB \ \-\-elementtype\fB= ELEMENTTYPE
 element type, i.e. attribute, property or command
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -880,56 +863,56 @@
 .IP \(bu 2
 without <dv_attr1>: datasources for all attributes are created
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
-default <datasource> is ‘exp_mot’
+default <datasource> is \(aqexp_mot\(aq
 .IP \(bu 2
 default <host>, <port> are taken from <server>
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device\fB= DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device\fB= DEVICE
 device, i.e. p09/pilatus300k/01 (mandatory)
 .TP
-.BI \-o \ DATASOURCE\fP,\fB \ \-\-datasource\-prefix\fB= DATASOURCE
+.BI \-o \ DATASOURCE\fR,\fB \ \-\-datasource\-prefix\fB= DATASOURCE
 datasource\-prefix
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-s \ HOST\fP,\fB \ \-\-host\fB= HOST
+.BI \-s \ HOST\fR,\fB \ \-\-host\fB= HOST
 tango host name
 .TP
-.BI \-t \ PORT\fP,\fB \ \-\-port\fB= PORT
+.BI \-t \ PORT\fR,\fB \ \-\-port\fB= PORT
 tango host port
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.B \-n\fP,\fB  \-\-no\-group
-don’t create common group with a name of datasource
+.B  \-n\fP,\fB  \-\-no\-group
+don\(aqt create common group with a name of datasource
 prefix
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -960,53 +943,53 @@
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 with \-d <directory>: datasources are created on the local filesystem
 .IP \(bu 2
 without \-b or \-d <directory>: run in the test mode
 .IP \(bu 2
-default <inputFile> is ‘/online_dir/online.xml’
+default <inputFile> is \(aq/online_dir/online.xml\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .sp
 \fIonlineds\fP overwrites existing datasources
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store components in Configuration Server database
 .TP
-.B \-t\fP,\fB  \-\-noclientlike
+.B  \-t\fP,\fB  \-\-noclientlike
 set motor tango datasources to be non __CLIENT__ like
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output directory where datasources will be saved
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-e \ EXTERNAL\fP,\fB \ \-\-external\fB= EXTERNAL
+.BI \-e \ EXTERNAL\fR,\fB \ \-\-external\fB= EXTERNAL
 external configuration server
 .TP
-.BI \-p \ XMLPACKAGE\fP,\fB \ \-\-xml\-package\fB= XMLPACKAGE
+.BI \-p \ XMLPACKAGE\fR,\fB \ \-\-xml\-package\fB= XMLPACKAGE
 xml template package
 .TP
-.B \-\-verbose
+.B  \-\-verbose
 printout verbose mode
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1038,49 +1021,49 @@
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 with \-d <directory>: datasources are created on the local filesystem
 .IP \(bu 2
 without \-b or \-d <directory>: run in the test mode
 .IP \(bu 2
-default <channel> is ‘ALL’
+default <channel> is \(aqALL\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
 default <pool> is taken from Tango DB
 .UNINDENT
 .sp
 \fIpoolds\fP overwrites existing datasources
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store components in Configuration Server database
 .TP
-.B \-t\fP,\fB  \-\-noclientlike
+.B  \-t\fP,\fB  \-\-noclientlike
 set motor tango datasources to be non __CLIENT__ like
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output directory where datasources will be saved
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-p \ POOL\fP,\fB \ \-\-pool\fB= POOL
+.BI \-p \ POOL\fR,\fB \ \-\-pool\fB= POOL
 sardana pool device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1109,78 +1092,78 @@
 nxscreate onlinecp [options] inputFile
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-without ‘\-c <component>’: show a list of possible components
+without \(aq\-c <component>\(aq: show a list of possible components
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
-default <inputFile> is ‘/online_dir/online.xml’
+default <inputFile> is \(aq/online_dir/online.xml\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-c \ COMPONENT\fP,\fB \ \-\-component\fB= COMPONENT
+.BI \-c \ COMPONENT\fR,\fB \ \-\-component\fB= COMPONENT
 component namerelated to the device name from
 <inputFile>
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-t \ CPTYPE\fP,\fB \ \-\-type \ CPTYPE
+.BI \-t \ CPTYPE\fR,\fB \ \-\-type \ CPTYPE
 component type
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device \ DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device \ DEVICE
 device, i.e. p09/pilatus300k/01
 .TP
-.BI \-u \ HOST\fP,\fB \ \-\-host \ HOST
+.BI \-u \ HOST\fR,\fB \ \-\-host \ HOST
 tango host name
 .TP
-.BI \-w \ PORT\fP,\fB \ \-\-port \ PORT
+.BI \-w \ PORT\fR,\fB \ \-\-port \ PORT
 tango host port
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing component
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-e \ EXTERNAL\fP,\fB \ \-\-external\fB= EXTERNAL
+.BI \-e \ EXTERNAL\fR,\fB \ \-\-external\fB= EXTERNAL
 external configuration server
 .TP
-.BI \-p \ XMLPACKAGE\fP,\fB \ \-\-xml\-package\fB= XMLPACKAGE
+.BI \-p \ XMLPACKAGE\fR,\fB \ \-\-xml\-package\fB= XMLPACKAGE
 xml template package
 .TP
-.BI \-y \ ENTRYNAME\fP,\fB \ \-\-entryname \ ENTRYNAME
+.BI \-y \ ENTRYNAME\fR,\fB \ \-\-entryname \ ENTRYNAME
 entry group name (prefix)
 .TP
-.BI \-i \ INSNAME\fP,\fB \ \-\-insname \ INSNAME
+.BI \-i \ INSNAME\fR,\fB \ \-\-insname \ INSNAME
 instrument group name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1209,68 +1192,68 @@
 nxscreate stdcomp [options] [name1 value1 [name2 value2] ...]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-without ‘\-t <type>’: show a list of possible component types
+without \(aq\-t <type>\(aq: show a list of possible component types
 .IP \(bu 2
-with ‘\-t <type>  and without \-c <component>: show a list of component variables for the given component type
+with \(aq\-t <type>  and without \-c <component>: show a list of component variables for the given component type
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
-[name1 value1 [name2 value2] …] sequence  defines component variable values
+[name1 value1 [name2 value2] ...] sequence  defines component variable values
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-c \ COMPONENT\fP,\fB \ \-\-component\fB= COMPONENT
+.BI \-c \ COMPONENT\fR,\fB \ \-\-component\fB= COMPONENT
 component name
 .TP
-.BI \-t \ CPTYPE\fP,\fB \ \-\-type\fB= CPTYPE
+.BI \-t \ CPTYPE\fR,\fB \ \-\-type\fB= CPTYPE
 component type
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-p \ XMLPACKAGE\fP,\fB \ \-\-xml\-package\fB= XMLPACKAGE
+.BI \-p \ XMLPACKAGE\fR,\fB \ \-\-xml\-package\fB= XMLPACKAGE
 xml template package
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing component
 .TP
-.B \-m\fP,\fB  \-\-mandatory
+.B  \-m\fP,\fB  \-\-mandatory
 set the component as mandatory
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store datasources in Configuration Server database
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output datasource directory
 .TP
-.BI \-e \ EXTERNAL\fP,\fB \ \-\-external\fB= EXTERNAL
+.BI \-e \ EXTERNAL\fR,\fB \ \-\-external\fB= EXTERNAL
 external configuration server
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-y \ ENTRYNAME\fP,\fB \ \-\-entryname \ ENTRYNAME
+.BI \-y \ ENTRYNAME\fR,\fB \ \-\-entryname \ ENTRYNAME
 entry group name (prefix)
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1300,94 +1283,233 @@
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
 with \-b: datasources are created in Configuration Server database
 .IP \(bu 2
 without \-b: datasources are created on the local filesystem in \-d <directory>
 .IP \(bu 2
-default <directory> is ‘.’
+default <directory> is \(aq.\(aq
 .IP \(bu 2
 default <server> is taken from Tango DB
 .IP \(bu 2
 default <strategy> is step
 .IP \(bu 2
 default <type> is NX_FLOAT
 .IP \(bu 2
 default <chunk> is SCALAR
 .IP \(bu 2
-default <nexuspath> is “/$var.entryname#’scan’$var.serialno:NXentry/instrument/collection/”
+default <nexuspath> is \(dq/$var.entryname#\(aqscan\(aq$var.serialno:NXentry/instrument/collection/\(dq
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-v \ DEVICE\fP,\fB \ \-\-device\-prefix\fB= DEVICE
+.BI \-v \ DEVICE\fR,\fB \ \-\-device\-prefix\fB= DEVICE
 device prefix, i.e. exp_c
 .TP
-.BI \-f \ FIRST\fP,\fB \ \-\-first\fB= FIRST
+.BI \-f \ FIRST\fR,\fB \ \-\-first\fB= FIRST
 first index
 .TP
-.BI \-l \ LAST\fP,\fB \ \-\-last\fB= LAST
+.BI \-l \ LAST\fR,\fB \ \-\-last\fB= LAST
 last index
 .TP
-.B \-o\fP,\fB  \-\-overwrite
+.B  \-o\fP,\fB  \-\-overwrite
 overwrite existing components
 .TP
-.BI \-d \ DIRECTORY\fP,\fB \ \-\-directory\fB= DIRECTORY
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory\fB= DIRECTORY
 output component directory
 .TP
-.BI \-x \ FILE\fP,\fB \ \-\-file\-prefix\fB= FILE
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix\fB= FILE
 file prefix, i.e. counter
 .TP
-.BI \-n \ NEXUSPATH\fP,\fB \ \-\-nexuspath\fB= NEXUSPATH
+.BI \-n \ NEXUSPATH\fR,\fB \ \-\-nexuspath\fB= NEXUSPATH
 nexus path with field name
 .TP
-.BI \-g \ STRATEGY\fP,\fB \ \-\-strategy\fB= STRATEGY
+.BI \-g \ STRATEGY\fR,\fB \ \-\-strategy\fB= STRATEGY
 writing strategy, i.e. STEP, INIT, FINAL, POSTRUN
 .TP
-.BI \-s \ DATASOURCE\fP,\fB \ \-\-datasource\-prefix \ DATASOURCE
+.BI \-s \ DATASOURCE\fR,\fB \ \-\-datasource\-prefix \ DATASOURCE
 datasource\-prefix or datasourcename
 .TP
-.BI \-t \ TYPE\fP,\fB \ \-\-type\fB= TYPE
+.BI \-t \ TYPE\fR,\fB \ \-\-type\fB= TYPE
 nexus type of the field
 .TP
-.BI \-u \ UNITS\fP,\fB \ \-\-units\fB= UNITS
+.BI \-u \ UNITS\fR,\fB \ \-\-units\fB= UNITS
 nexus units of the field
 .TP
-.B \-k\fP,\fB  \-\-links
+.B  \-k\fP,\fB  \-\-links
 create datasource links
 .TP
-.B \-b\fP,\fB  \-\-database
+.B  \-b\fP,\fB  \-\-database
 store components in Configuration Server database
 .TP
-.BI \-r \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-r \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 configuration server device name
 .TP
-.BI \-c \ CHUNK\fP,\fB \ \-\-chunk\fB= CHUNK
+.BI \-c \ CHUNK\fR,\fB \ \-\-chunk\fB= CHUNK
 chunk format, i.e. SCALAR, SPECTRUM, IMAGE
 .TP
-.B \-m\fP,\fB  \-\-minimal_device
-device name without first ‘0’
+.B  \-m\fP,\fB  \-\-minimal_device
+device name without first \(aq0\(aq
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 nxscreate comp counter
 nxscreate comp \-f1 \-l3 \-v exp_c \-b
 nxscreate comp lambda \-d /home/user/xmldir/
-nxscreate comp \-n "/\e$var.entryname#\(aqscan\(aq\e$var.serialno:NXentry/instrument/sis3302:NXdetector/collection:NXcollection/\(aq \-v sis3302_1_roi \-f1 \-l4  \-g STEP \-t NX_FLOAT64 \-k \-b \-m
-nxscreate comp \-n "/\e$var.entryname#\(aqscan\(aq\e$var.serialno:NXentry/instrument/eh1_mca01:NXdetector/data" eh1_mca01 \-g STEP \-t NX_FLOAT64 \-i \-b \-c SPECTRUM
+nxscreate comp \-n \(dq/\e$var.entryname#\(aqscan\(aq\e$var.serialno:NXentry/instrument/sis3302:NXdetector/collection:NXcollection/\(aq \-v sis3302_1_roi \-f1 \-l4  \-g STEP \-t NX_FLOAT64 \-k \-b \-m
+nxscreate comp \-n \(dq/\e$var.entryname#\(aqscan\(aq\e$var.serialno:NXentry/instrument/eh1_mca01:NXdetector/data\(dq eh1_mca01 \-g STEP \-t NX_FLOAT64 \-i \-b \-c SPECTRUM
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS nxscreate secopcp
+.sp
+It creates a  component or components describing modules of the secop node.
+.SS Synopsis
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxscreate secopcp [\-h] [\-l] [\-o] [\-a] [\-q] [\-w] [\-c COMPONENT] [\-e PARAMSTRATEGY] [\-g STRATEGY] [\-m TIMEOUT] [\-s SAMPLENAME] [\-s SAMPLEENVNAME] [\-k MEANINGS] [\-v ENVIRONMENTS] [\-f FIRST] [\-z TRANSATTRS] [\-p XMLPACKAGE] [\-y ENTRYNAME] [\-i INSNAME] [\-d DIRECTORY] [\-j JSON] [\-x FILE] [\-n] [\-b] [\-u HOST] [\-t PORT] [\-r SERVER] [component_name ...]
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.IP \(bu 2
+with \-b: datasources are created in Configuration Server database
+.IP \(bu 2
+without \-b: datasources are created on the local filesystem in \-d <directory>
+.IP \(bu 2
+default <port> is 5000
+.UNINDENT
+.INDENT 0.0
+.TP
+.B Options:
+.INDENT 7.0
+.TP
+.B  \-h\fP,\fB  \-\-help
+show this help message and exit
+.TP
+.B  \-l\fP,\fB  \-\-list
+list modules of the given node
+.TP
+.B  \-o\fP,\fB  \-\-overwrite
+overwrite existing components
+.TP
+.B  \-a\fP,\fB  \-\-can\-fail
+can fail strategy flag
+.TP
+.B  \-q\fP,\fB  \-\-dynamic
+create dynamic links
+.TP
+.B  \-\-sample\-nxdata
+create NXdata in NXsample
+.TP
+.BI \-c \ COMPONENT\fR,\fB \ \-\-component \ COMPONENT
+component namesecop component name
+.TP
+.BI \-e \ PARAMSTRATEGY\fR,\fB \ \-\-param\-strategy \ PARAMSTRATEGY
+sensor parameter strategy, i.e. INIT, STEP or FINAL, default: INIT
+.TP
+.BI \-g \ STRATEGY\fR,\fB \ \-\-strategy \ STRATEGY
+sensor value strategy, i.e. INIT, STEP or FINAL, default: INIT
+.TP
+.BI \-m \ TIMEOUT\fR,\fB \ \-\-timeout \ TIMEOUT
+sensor minimum timeout default: 0.001
+.TP
+.BI \-s \ SAMPLENAME\fR,\fB \ \-\-sample \ SAMPLENAME
+sample name
+.TP
+.BI \-w \ SAMPLEENVNAME\fR,\fB \ \-\-sample\-environment \ SAMPLEENVNAME
+sample environment name
+.TP
+.BI \-k \ MEANINGS\fR,\fB \ \-\-links \ MEANINGS
+NXlog links of physical quantities to sensors
+separated by comman. Default:
+\(aqtemperature,magnetic_field,electric_field,stress_field,pressure\(aq
+.TP
+.BI \-v \ ENVIRONMENTS\fR,\fB \ \-\-environments \ ENVIRONMENTS
+NXenvironment links of physical quantities separated
+by comman. Default: \(aqtemperature,magnetic_field\(aq
+.TP
+.BI \-f \ FIRST\fR,\fB \ \-\-first \ FIRST
+first linked targets separated by comman
+.TP
+.BI \-z \ TRANSATTRS\fR,\fB \ \-\-transformation\-attributes \ TRANSATTRS
+a JSON dictionary with transformation parameters i.e, \(dqtransformation_type\(dq, \(dqvector\(dq, \(dqdepends_on\(dq. Default:
+{\(dqrotation_z\(dq:{\(dqtransformation_type\(dq:\(dqrotation\(dq,\(dqvector\(dq:[0,\-1,0]}}
+.TP
+.BI \-p \ XMLPACKAGE\fR,\fB \ \-\-xml\-package \ XMLPACKAGE
+xml template package
+.TP
+.BI \-y \ ENTRYNAME\fR,\fB \ \-\-entryname \ ENTRYNAME
+entry group name (prefix)
+.TP
+.BI \-i \ INSNAME\fR,\fB \ \-\-insname \ INSNAME
+instrument group name
+.TP
+.BI \-d \ DIRECTORY\fR,\fB \ \-\-directory \ DIRECTORY
+output component directory
+.TP
+.BI \-j \ JSON\fR,\fB \ \-\-json\-file \ JSON
+json configuration file
+.TP
+.BI \-x \ FILE\fR,\fB \ \-\-file\-prefix \ FILE
+file prefix, i.e. counter
+.TP
+.B  \-n\fP,\fB  \-\-nolower
+do not change aliases into lower case
+.TP
+.B  \-b\fP,\fB  \-\-database
+store components in Configuration Server database
+.TP
+.BI \-u \ HOST\fR,\fB \ \-\-host \ HOST
+secop host name
+.TP
+.BI \-t \ PORT\fR,\fB \ \-\-port \ PORT
+secop host port
+.TP
+.BI \-r \ SERVER\fR,\fB \ \-\-server \ SERVER
+configuration server device name
+.UNINDENT
+.UNINDENT
+.SS Example
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxscreate secopcp
+nxscreate secopcp \-l
+
+    \- list all modules of the given node
+
+nxscreate secopcp \-c temp_node \-d . \-j secop_node.json
+
+    \- create the all secop components in the local directory for the node configured with the json file
+
+nxscreate secopcp T \-t 5001 \-b
+
+    \- create the component for the T secop module  in the NXSConfigServer database for the node on the port 5000
+
+nxscreate secopcp \-d /home/user/xmldir/
+
+    \- create the all secop components in the given directory
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS nxscreate compare
 .sp
 It compares two online.xml files
@@ -1400,28 +1522,28 @@
 nxscreate compare [\-h] [\-n] online_file [online_file]
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .IP \(bu 2
-default: second <online_file> is ‘/online_dir/online.xml’ if only file is given
+default: second <online_file> is \(aq/online_dir/online.xml\(aq if only file is given
 .UNINDENT
 .INDENT 0.0
 .TP
 .B positional arguments:
 online_file    online.xml files
 .TP
 .B optional arguments:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.B \-n\fP,\fB  \-\-nolower
+.B  \-n\fP,\fB  \-\-nolower
 do not change aliases into lower case
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1477,18 +1599,18 @@
 .B servers [\-s <nexus_server/host>]
 get lists of tango data servers from the current tango host
 .UNINDENT
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-s \ SERVER\fP,\fB \ \-\-server\fB= SERVER
+.BI \-s \ SERVER\fR,\fB \ \-\-server\fB= SERVER
 tango data server device name
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1511,15 +1633,15 @@
 .ft C
 nxsfileinfo <command> [options] <nexus_file_name>
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .sp
-The following commands are available: general, field
+The following commands are available: general, field, metadata, origdatablock, sample, instrument, attachment
 .SS nxsfileinfo general
 .sp
 It shows general information for he nexus file.
 .SS Synopsis
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1531,21 +1653,21 @@
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.B \-\-h5py
+.B  \-\-h5py
 use h5py module as a nexus reader
 .TP
-.B \-\-h5cpp
+.B  \-\-h5cpp
 use h5cpp module as a nexus reader
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
@@ -1561,53 +1683,605 @@
 It shows field information for the nexus file.
 .SS Synopsis
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-Usage: nxsfileinfo field <file_name>
+Usage: nxsfileinfo field [options]  <file_name>
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B Options:
 .INDENT 7.0
 .TP
-.B \-h\fP,\fB  \-\-help
+.B  \-h\fP,\fB  \-\-help
 show this help message and exit
 .TP
-.BI \-c \ HEADERS\fP,\fB \ \-\-columns\fB= HEADERS
+.BI \-c \ HEADERS\fR,\fB \ \-\-columns\fB= HEADERS
 names of column to be shown (separated by commas without spaces). The possible names are: depends_on, dtype, full_path, nexus_path, nexus_type, shape, source, source_name, source_type, strategy, trans_type, trans_offset, trans_vector, units, value
 .TP
-.BI \-f \ FILTERS\fP,\fB \ \-\-filters\fB= FILTERS
-full_path filters (separated by commas without spaces). Default: ‘*’. E.g. ‘\fI:NXsample/\fP’
+.BI \-f \ FILTERS\fR,\fB \ \-\-filters\fB= FILTERS
+full_path filters (separated by commas without spaces). Default: \(aq*\(aq. E.g. \(aq\fI:NXsample/\fP\(aq
 .TP
-.BI \-v \ VALUES\fP,\fB \ \-\-values\fB= VALUES
+.BI \-v \ VALUES\fR,\fB \ \-\-values\fB= VALUES
 field names which value should be stored (separated by commas without spaces). Default: depends_on
 .TP
-.B \-g\fP,\fB  \-\-geometry
+.B  \-g\fP,\fB  \-\-geometry
 show fields with geometry full_path filters, i.e. \fI:NXtransformations/\fP,*/depends_on. It works only when \-f is not defined
 .TP
-.B \-s\fP,\fB  \-\-source
+.B  \-s\fP,\fB  \-\-source
 show datasource parameters
 .TP
-.B \-\-h5py
+.B  \-\-h5py
 use h5py module as a nexus reader
+.TP
+.B  \-\-h5cpp
+use h5cpp module as a nexus reader
 .UNINDENT
 .UNINDENT
 .SS Example
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 nxsfileinfo field /tmp/saxs_ref1_02.nxs
+nxsfileinfo field /user/data/myfile.nxs \-g
+nxsfileinfo field /user/data/myfile.nxs \-s
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS nxsfileinfo metadata
+.sp
+It shows metadata of the nexus file.
+.SS Synopsis
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+Usage: nxsfileinfo metadata [options] <file_name>
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B Options:
+.INDENT 7.0
+.TP
+.B  \-h\fP,\fB  \-\-help
+show this help message and exit
+.TP
+.BI \-a \ ATTRS\fR,\fB \ \-\-attributes \ ATTRS
+names of field or group attributes to be show (separated by commas without spaces). The default takes all attributes
+.TP
+.BI \-n \ NATTRS\fR,\fB \ \-\-hidden\-attributes \ NATTRS
+names of field or group attributes to be hidden (separated by commas without spaces). The default: \(aqnexdatas_source,nexdatas_strategy\(aq
+.TP
+.BI \-v \ VALUES\fR,\fB \ \-\-values \ VALUES
+field names of more dimensional datasets which value should be shown (separated by commas without spaces)
+.TP
+.BI \-z \ KEYWORDS\fR,\fB \ \-\-keywords \ KEYWORDS
+dataset keywords separated by commas.
+.TP
+.BI \-w \ OWNERGROUP\fR,\fB \ \-\-owner\-group \ OWNERGROUP
+owner group name. Default is {beamtimeid}\-part
+.TP
+.BI \-c \ ACCESSGROUPS\fR,\fB \ \-\-access\-groups \ ACCESSGROUPS
+access group names separated by commas. Default is
+{beamtimeid}\-clbt,{beamtimeId}\-dmgt,{beamline}dmgt
+.TP
+.BI \-g \ GROUP_POSTFIX\fR,\fB \ \-\-group\-postfix \ GROUP_POSTFIX
+postfix to be added to NeXus group name. The default: \(aqParameters\(aq
+.TP
+.BI \-t \ ENTRYCLASSES\fR,\fB \ \-\-entry\-classes \ ENTRYCLASSES
+names of entry NX_class to be shown (separated by commas without spaces). If name is \(aq\(aq all groups are shown. The default: \(aqNXentry\(aq
+.TP
+.BI \-e \ ENTRYNAMES\fR,\fB \ \-\-entry\-names \ ENTRYNAMES
+names of entry groups to be shown (separated by commas without spaces). If name is \(aq\(aq all groups are shown. The default: \(aq\(aq
+.TP
+.B  \-m\fP,\fB  \-\-raw\-metadata
+do not store NXentry as scientificMetadata
+.TP
+.B  \-\-add\-empty\-units
+add empty units for fields without units
+.TP
+.B  \-\-oned
+add 1d values to scientificMetadata
+.TP
+.BI \-\-max\-oned\-size \ MAXONEDSIZE
+add min and max (or first and last) values of 1d records to scientificMetadata if its size excides \-\-max\-oned\-size value
+.TP
+.BI \-p \ PID\fR,\fB \ \-\-pid \ PID
+dataset pid
+.TP
+.BI \-i \ BEAMTIMEID\fR,\fB \ \-\-beamtimeid \ BEAMTIMEID
+beamtime id
+.TP
+.B  \-u\fP,\fB  \-\-pid\-with\-uuid
+generate pid with uuid
+.TP
+.B  \-f\fP,\fB  \-\-pid\-with\-filename
+generate pid with file name
+.TP
+.BI \-q \ TECHNIQUES\fR,\fB \ \-\-techniques \ TECHNIQUES
+names of techniques (separated by commas without
+spaces).The default: \(aq\(aq
+.TP
+.BI \-j \ SAMPLEID\fR,\fB \ \-\-sample\-id \ SAMPLEID
+sampleId
+.TP
+.B  \-\-sample\-id\-from\-name
+get sampleId from the sample name
+.TP
+.BI \-y \ INSTRUMENTID\fR,\fB \ \-\-instrument\-id \ INSTRUMENTID
+instrumentId
+.TP
+.B  \-\-raw\-instrument\-id
+leave raw instrument id
+.TP
+.BI \-b \ BEAMTIMEMETA\fR,\fB \ \-\-beamtime\-meta \ BEAMTIMEMETA
+beamtime metadata file
+.TP
+.BI \-s \ SCIENTIFICMETA\fR,\fB \ \-\-scientific\-meta \ SCIENTIFICMETA
+scientific metadata file
+.TP
+.BI \-o \ OUTPUT\fR,\fB \ \-\-output \ OUTPUT
+output scicat metadata file
+.TP
+.BI \-r \ RELPATH\fR,\fB \ \-\-relative\-path \ RELPATH
+relative path to the scan files
+.TP
+.BI \-x \ CHMOD\fR,\fB \ \-\-chmod \ CHMOD
+json metadata file mod bits, e.g. 0o662
+.TP
+.BI \-\-copy\-map \ COPYMAP
+json or yaml map {output: input} or [[output, input],]
+or a text file list to re\-arrange metadata
+.TP
+.BI \-\-copy\-map\-field \ COPYMAPFIELD
+field json or yaml with map {output: input} or [[output, input],]
+or a text file list to re\-arrange metadata. The default:
+\(aqscientificMetadata.nxsfileinfo_parameters.copymap.value\(aq
+.TP
+.B  \-\-copy\-map\-error
+Raise an error when the copy map file does not exist
+.TP
+.BI \-\-copy\-map\-file \ COPYMAPFILE
+json or yaml file containing the copy map, see also \-\-copy\-map
+.TP
+.BI \-f \ FILEFORMAT\fR,\fB \ \-\-file\-format \ FILEFORMAT
+input file format, e.g. \(aqnxs\(aq. Default is defined by the file extension
+.TP
+.B  \-\-proposal\-as\-proposal
+Store the DESY proposal as the SciCat proposal
+.TP
+.B  \-\-h5py
+use h5py module as a nexus reader
+.TP
+.B  \-\-h5cpp
+use h5cpp module as a nexus reader
+.UNINDENT
+.UNINDENT
+.SS Example
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxsfileinfo metadata /user/data/myfile.nxs
+nxsfileinfo metadata /user/data/myfile.fio
+nxsfileinfo metadata /user/data/myfile.nxs \-p \(aqGroup\(aq
+nxsfileinfo metadata /user/data/myfile.nxs \-s
+nxsfileinfo metadata /user/data/myfile.nxs \-a units,NX_class
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS nxsfileinfo origdatablock
+.sp
+It generates description of all scan files
+.SS Synopsis
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+Usage: nxsfileinfo origdatablock [options] <scan_name>
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B Options:
+.INDENT 7.0
+.TP
+.B  \-h\fP,\fB  \-\-help
+show this help message and exit
+.TP
+.BI \-p \ PID\fR,\fB \ \-\-pid \ PID
+dataset pid
+.TP
+.BI \-o \ OUTPUT\fR,\fB \ \-\-output \ OUTPUT
+output scicat metadata file
+.TP
+.BI \-w \ OWNERGROUP\fR,\fB \ \-\-owner\-group \ OWNERGROUP
+owner group name. Default is {beamtimeid}\-part
+.TP
+.BI \-c \ ACCESSGROUPS\fR,\fB \ \-\-access\-groups \ ACCESSGROUPS
+access group names separated by commas. Default is
+{beamtimeid}\-clbt,{beamtimeId}\-dmgt
+.TP
+.BI \-s \ SKIP\fR,\fB \ \-\-skip \ SKIP
+filters for files to be skipped (separated by commas
+without spaces). Default: \(aq\(aq. E.g.
+\(aq\fI\&.pyc,\fP~\(aq
+.TP
+.BI \-a \ ADD\fR,\fB \ \-\-add \ ADD
+list of files to be added (separated by commas
+without spaces). Default: \(aq\(aq. E.g.
+\(aqscan1.nxs,scan2.nxs\(aq
+.TP
+.BI \-r \ RELPATH\fR,\fB \ \-\-relative\-path \ RELPATH
+relative path to the scan files
+.TP
+.BI \-x \ CHMOD\fR,\fB \ \-\-chmod \ CHMOD
+json metadata file mod bits, e.g. 0o662
+.UNINDENT
+.UNINDENT
+.SS Example
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxsfileinfo origdatablock /user/data/scan_12345
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS nxsfileinfo sample
+.sp
+It generates description of sample
+.SS Synopsis
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+Usage: nxsfileinfo sample [options]
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B Options:
+.INDENT 7.0
+.TP
+.B  \-h\fP,\fB  \-\-help
+show this help message and exit
+.TP
+.BI \-s \ SAMPLEID\fR,\fB \ \-\-sample\-id \ SAMPLEID
+sample id
+.TP
+.BI \-i \ BEAMTIMEID\fR,\fB \ \-\-beamtimeid \ BEAMTIMEID
+beamtime id
+.TP
+.BI \-b \ BEAMLINE\fR,\fB \ \-\-beamline \ BEAMLINE
+beamline
+.TP
+.BI \-d \ DESCRIPTION\fR,\fB \ \-\-description \ DESCRIPTION
+sample description
+.TP
+.BI \-r \ OWNER\fR,\fB \ \-\-owner \ OWNER
+sample owner
+.TP
+.B  \-p\fP,\fB  \-\-published
+sample is published
+.TP
+.BI \-w \ OWNERGROUP\fR,\fB \ \-\-owner\-group \ OWNERGROUP
+owner group name. Default is {beamtimeid}\-dmgt
+.TP
+.BI \-c \ ACCESSGROUPS\fR,\fB \ \-\-access\-groups \ ACCESSGROUPS
+access group names separated by commas. Default is {be
+amtimeId}\-dmgt,{beamtimeid}\-clbt,{beamtimeId}\-part,{be
+amline}dmgt,{beamline}staff
+.TP
+.BI \-x \ CHMOD\fR,\fB \ \-\-chmod \ CHMOD
+json metadata file mod bits, e.g. 0o662
+.TP
+.BI \-m \ CHARACTERISTICSMETA\fR,\fB \ \-\-sample\-characteristics \ CHARACTERISTICSMETA
+sample characteristics metadata file
+.TP
+.BI \-o \ OUTPUT\fR,\fB \ \-\-output \ OUTPUT
+output scicat metadata file
+.UNINDENT
+.UNINDENT
+.SS Example
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxsfileinfo sample \-i petra3/h2o/234234 \-d \(aqHH water\(aq \-s ~/cm.json
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS nxsfileinfo instrument
+.sp
+It generates description of instrument
+.SS Synopsis
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+Usage: nxsfileinfo instrument [options]
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B Options:
+.INDENT 7.0
+.TP
+.B  \-h\fP,\fB  \-\-help
+show this help message and exit
+.TP
+.BI \-p \ PID\fR,\fB \ \-\-pid \ PID
+instrument pid
+.TP
+.BI \-n \ NAME\fR,\fB \ \-\-name \ NAME
+instrument name
+.TP
+.BI \-i \ BEAMTIMEID\fR,\fB \ \-\-beamtimeid \ BEAMTIMEID
+beamtime id
+.TP
+.BI \-b \ BEAMLINE\fR,\fB \ \-\-beamline \ BEAMLINE
+beamline
+.TP
+.BI \-w \ OWNERGROUP\fR,\fB \ \-\-owner\-group \ OWNERGROUP
+owner group name. Default is {beamtimeid}\-dmgt
+.TP
+.BI \-c \ ACCESSGROUPS\fR,\fB \ \-\-access\-groups \ ACCESSGROUPS
+access group names separated by commas. Default is {be
+amtimeId}\-dmgt,{beamtimeid}\-clbt,{beamtimeId}\-part,{be
+amline}dmgt,{beamline}staff
+.TP
+.BI \-x \ CHMOD\fR,\fB \ \-\-chmod \ CHMOD
+json metadata file mod bits, e.g. 0o662
+.TP
+.BI \-m \ CUSTOMMETA\fR,\fB \ \-\-custom\-metadata \ CUSTOMMETA
+instrument characteristics metadata file
+.TP
+.BI \-o \ OUTPUT\fR,\fB \ \-\-output \ OUTPUT
+output scicat metadata file
+.UNINDENT
+.UNINDENT
+.SS Example
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxsfileinfo instrument \-p /petra3/p00 \-n P00 \-m ~/cm.json
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS nxsfileinfo attachment
+.sp
+It generates description of attachment
+.SS Synopsis
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+Usage: nxsfileinfo attachment [options] <image_file|scan_file>
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B Options:
+.INDENT 7.0
+.TP
+.B  \-h\fP,\fB  \-\-help
+show this help message and exit
+.TP
+.BI \-a \ ATID\fR,\fB \ \-\-id \ ATID
+attachment id
+.TP
+.BI \-t \ CAPTION\fR,\fB \ \-\-caption \ CAPTION
+caption text
+.TP
+.BI \-i \ BEAMTIMEID\fR,\fB \ \-\-beamtimeid \ BEAMTIMEID
+beamtime id
+.TP
+.BI \-b \ BEAMLINE\fR,\fB \ \-\-beamline \ BEAMLINE
+beamline
+.TP
+.BI \-r \ OWNER\fR,\fB \ \-\-owner \ OWNER
+attachment owner
+.TP
+.BI \-w \ OWNERGROUP\fR,\fB \ \-\-owner\-group \ OWNERGROUP
+owner group name. Default is {beamtimeid}\-dmgt
+.TP
+.BI \-c \ ACCESSGROUPS\fR,\fB \ \-\-access\-groups \ ACCESSGROUPS
+access group names separated by commas. Default is {be
+amtimeId}\-dmgt,{beamtimeid}\-clbt,{beamtimeId}\-part,{be
+amline}dmgt,{beamline}staff
+.TP
+.BI \-f \ FILEFORMAT\fR,\fB \ \-\-file\-format \ FILEFORMAT
+input file format, e.g. \(aqnxs\(aq. Default is defined by
+the file extension
+.TP
+.B  \-\-h5py
+use h5py module as a nexus reader
+.TP
+.B  \-\-h5cpp
+use h5cpp module as a nexus reader
+.TP
+.BI \-x \ CHMOD\fR,\fB \ \-\-chmod \ CHMOD
+json metadata file mod bits, e.g. 0o662
+.TP
+.BI \-s \ SIGNALS\fR,\fB \ \-\-signals \ SIGNALS
+signals data name(s) separated by comma
+.TP
+.BI \-e \ AXES\fR,\fB \ \-\-axes \ AXES
+axis/axes data name(s) separated by comma
+.TP
+.BI \-q \ SCANCMDAXES\fR,\fB \ \-\-scan\-command\-axes \ SCANCMDAXES
+a JSON dictionary with scan\-command axes to override,
+axis/axes data name(s) separated by comma for
+detectors and by semicolon for more plots. Default:
+{\(dqhklscan\(dq:\(dqh;k;l\(dq,\(dqqscan\(dq:\(dqqz;qpar\(dq}
+.TP
+.BI \-m \ FRAME\fR,\fB \ \-\-frame \ FRAME
+a frame number for if more 2D images in the data
+.TP
+.BI \-\-signal\-label \ SLABEL
+signal label
+.TP
+.BI \-\-xlabel \ XLABEL
+x\-axis label
+.TP
+.BI \-\-ylabel \ YLABEL
+y\-axis label
+.TP
+.B  \-u\fP,\fB  \-\-override
+override NeXus entries by script parameters
+.TP
+.B  \-\-parameters\-in\-caption
+add plot paramters to the caption
+.TP
+.BI \-n \ NEXUSPATH\fR,\fB \ \-\-nexus\-path \ NEXUSPATH
+base nexus path to element to be shown.
+If th path is \(aq\(aq the default group is shown. The default: \(aq\(aq
+.TP
+.BI \-o \ OUTPUT\fR,\fB \ \-\-output \ OUTPUT
+output scicat metadata file
+.UNINDENT
+.UNINDENT
+.SS Example
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxsfileinfo attachment \-b p00 \-i 2342342 \-t \(aqHH water\(aq \-o ~/at1.json thumbnail.png
+nxsfileinfo attachment \-b p00 \-i 2342342 \-t \(aqHH water\(aq \-o ~/at2.json \-s pilatus myscan_00123.nxs
+nxsfileinfo attachment \-b p00 \-i 2342342 \-t \(aqHH water\(aq \-o ~/at2.json  myscan_00124.fio
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.SS nxsfileinfo groupmetadata
+.sp
+It groups scan metadata to one dataset
+.SS Synopsis
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+Usage: nxsfileinfo groupmetadata [options] [groupname]
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B Options:
+.INDENT 7.0
+.TP
+.B  \-h\fP,\fB  \-\-help
+show this help message and exit
+.TP
+.BI \-p \ PID\fR,\fB \ \-\-pid \ PID
+dataset pid
+.TP
+.B  \-\-raw
+raw dataset type
+.TP
+.BI \-i \ BEAMTIMEID\fR,\fB \ \-\-beamtimeid
+BEAMTIMEID beamtime id
+.TP
+.B  \-s\fP,\fB  \-\-skip\-group\-datablock
+skip group datablock
+.TP
+.B  \-w\fP,\fB  \-\-allow\-duplication
+allow to merge metadata with duplicated pid
+.TP
+.B  \-q\fP,\fB  \-\-raw
+raw dataset type
+.TP
+.B  \-f\fP,\fB  \-\-write\-files
+write output to files
+.TP
+.BI \-k \ SCICATVERSION\fR,\fB \ \-\-scicat\-version \ SCICATVERSION
+major scicat version metadata
+.TP
+.BI \-x \ CHMOD\fR,\fB \ \-\-chmod \ CHMOD
+json metadata file mod bits, e.g. 0o662
+.TP
+.BI \-g \ GROUPMAP\fR,\fB \ \-\-group\-map \ GROUPMAP
+json or yaml map of {output: input} or [[output,
+input],] or a text file list to re\-arrange metadata
+.TP
+.B  \-e\fP,\fB  \-\-group\-map\-error
+Raise an error when the group map file does not exist
+.TP
+.BI \-r \ GROUPMAPFILE\fR,\fB \ \-\-group\-map\-file \ GROUPMAPFILE
+json or yaml file containing the copy map, see also
+.TP
+.BI \-m \ METADATAFILE\fR,\fB \ \-\-metadata \ METADATAFILE
+json metadata file
+.TP
+.BI \-d \ ORIGDATABLOCKFILE\fR,\fB \ \-\-origdatablock \ ORIGDATABLOCKFILE
+json origmetadata file
+.TP
+.BI \-a \ ATTACHMENTFILE\fR,\fB \ \-\-attachment \ ATTACHMENTFILE
+json attachment file
+.TP
+.BI \-o \ OUTPUT\fR,\fB \ \-\-output \ OUTPUT
+output scicat group metadata file
+.TP
+.BI \-l \ DBOUTPUT\fR,\fB \ \-\-datablock\-output \ DBOUTPUT
+output scicat group datablocks list file
+.TP
+.BI \-t \ ATOUTPUT\fR,\fB \ \-\-attachment\-output \ ATOUTPUT
+output scicat group attachments list file
+.UNINDENT
+.UNINDENT
+.SS Example
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+nxsfileinfo groupmetadata \-o /user/data/myscan.scan.json  \-t /user/data/myscan.attachment.json  \-l /user/data/myscan.origdatablock.json  \-c /home/user/group_config.txt  \-m /user/data/myscan_00023.scan.json  \-d /user/data/myscan_00023.origdatablock.json  \-a /user/data/myscan_00023.attachment.json
+
+nxsfileinfo groupmetadata myscan_m001  \-m /user/data/myscan_00021.scan.json \-c /home/user/group_config.txt
+
+nxsfileinfo groupmetadata  myscan_m001  \-c /home/user/group_config.txt  \-m /user/data/myscan_00023.scan.json  \-d /user/data/myscan_00023.origdatablock.json  \-a /user/data/myscan_00023.attachment.json
+
+nxsfileinfo groupmetadata  \-m /user/data/myscan_00023.scan.json  \-d /user/data/myscan_00023.origdatablock.json  \-c /home/user/group_config.txt
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SH NXSETUP
 .SS Description
 .sp
@@ -1642,51 +2316,66 @@
 
 optional arguments:
   \-h, \-\-help            show this help message and exit
   \-b BEAMLINE, \-\-beamline BEAMLINE
                         name of the beamline ( default: \(aqnxs\(aq )
   \-m MASTERHOST, \-\-masterHost MASTERHOST
                         the host that stores the Mg ( default: <localhost> )
+  \-c CONFIGHOST, \-\-confighost CONFIGHOST
+                        the host to run the config server ( default: <mysqlhost> )
+  \-r RUNHOST, \-\-runhost RUNHOST
+                        the host to run the server ( default: localhost )
   \-u USER, \-\-user USER  the local user ( default: \(aqtango\(aq )
   \-d DBNAME, \-\-database DBNAME
                         the database name ( default: \(aqnxsconfig\(aq)
   \-j CSJSON, \-\-csjson CSJSON
                         JSONSettings for the configuration server. ( default:
-                        \(aq{"host": "localhost","db": <DBNAME>, "use_unicode":
-                        true\(aq, "read_default_file": <MY_CNF_FILE>}\(aq where
-                        <MY_CNF_FILE> stays for "/home/<USER>/.my.cnf" or
-                        "/var/lib/nxsconfigserver/.my.cnf" )
+                        \(aq{\(dqhost\(dq: \(dqlocalhost\(dq,\(dqdb\(dq: <DBNAME>, \(dquse_unicode\(dq:
+                        true\(aq, \(dqread_default_file\(dq: <MY_CNF_FILE>}\(aq where
+                        <MY_CNF_FILE> stays for \(dq/home/<USER>/.my.cnf\(dq or
+                        \(dq/var/lib/nxsconfigserver/.my.cnf\(dq )
+  \-k CLASSNAME, \-\-class\-name CLASSNAME
+                        tango server class name
+  \-y PROPJSON, \-\-json\-device\-properties PROPJSON
+                        JSON tango device properties ( default: \(aq{}\(aq )
+  \-t, \-\-postpone        do not start the server
 
  examples:
        nxsetup set
        nxsetup set \-b p09 \-m haso228 \-u p09user \-d nxsconfig NXSConfigServer
+       nxsetup set NexusWriter/haso228  \-k NexusWriter  \-y \(aq{\(dqp00/bliss_nexuswriter/test_session\(dq:{\(dqsession\(dq:\(dqtest_session\(dq,\(dqbeacon_host\(dq:\(dqhaso228:25000\(dq}}\(aq  \-t
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS nxsetup restart
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
-usage: nxsetup restart [\-h] [\-l LEVEL] [server_name [server_name ...]]
+   usage: nxsetup restart [\-h] [\-l LEVEL] [server_name [server_name ...]]
 
-restart tango server
+   restart tango server
 
-positional arguments:
-  server_name           server names, e.g.: NXSRecSelector NXSDataWriter/TDW1
+   positional arguments:
+     server_name           server names, e.g.: NXSRecSelector NXSDataWriter/TDW1
 
-optional arguments:
-  \-h, \-\-help            show this help message and exit
-  \-l LEVEL, \-\-level LEVEL
-                        startup level
+   optional arguments:
+     \-h, \-\-help            show this help message and exit
+     \-l LEVEL, \-\-level LEVEL
+                           startup level
+     \-z TIMEOUT, \-\-timeout TIMEOUT
+                           timeout in seconds
+     \-e, \-\-no\-wait         do not wait
 
- examples:
-       nxsetup restart Pool/haso228 \-l 2
+examples:
+
+    examples:
+          nxsetup restart Pool/haso228 \-l 2
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS nxsetup start
 .INDENT 0.0
 .INDENT 3.5
@@ -1700,14 +2389,17 @@
 positional arguments:
   server_name           server names, e.g.: NXSRecSelector NXSDataWriter/TDW1
 
 optional arguments:
   \-h, \-\-help            show this help message and exit
   \-l LEVEL, \-\-level LEVEL
                         startup level
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+  \-e, \-\-no\-wait         do not wait
 
  examples:
        nxsetup start Pool/haso228 \-l 2
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
@@ -1729,14 +2421,39 @@
 
  examples:
        nxsetup stop Pool/haso228
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
+.SS nxsetup wait
+.INDENT 0.0
+.INDENT 3.5
+.sp
+.nf
+.ft C
+usage: nxsetup wait [\-h] [server_name [server_name ...]]
+
+stop tango server
+
+positional arguments:
+  server_name           server names, e.g.: NXSRecSelector NXSDataWriter/TDW1
+
+optional arguments:
+  \-h, \-\-help            show this help message and exit
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+
+
+ examples:
+       nxsetup wait Pool/haso228
+.ft P
+.fi
+.UNINDENT
+.UNINDENT
 .SS nxsetup move\-prop
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
 .ft C
 usage: nxsetup move\-prop [\-h] [\-n NEWNAME] [\-o OLDNAME]
@@ -1750,14 +2467,17 @@
 optional arguments:
   \-h, \-\-help            show this help message and exit
   \-n NEWNAME, \-\-newname NEWNAME
                         (new) property name
   \-o OLDNAME, \-\-oldname OLDNAME
                         old property name
   \-t, \-\-postpone        do not restart the server
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+  \-e, \-\-no\-wait         do not wait
 
  examples:
        nxsetup move\-prop \-n DefaultPreselectedComponents \-o DefaultAutomaticComponents NXSRecSelector
        nxsetup move\-prop \-t \-n DefaultPreselectedComponents  \-o DefaultAutomaticComponents NXSRecSelector
 .ft P
 .fi
 .UNINDENT
@@ -1779,20 +2499,23 @@
 optional arguments:
   \-h, \-\-help            show this help message and exit
   \-n NEWNAME, \-\-newname NEWNAME
                         (new) property name
   \-w PROPVALUE, \-\-propvalue PROPVALUE
                         new property value
   \-t, \-\-postpone        do not restart the server
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+  \-e, \-\-no\-wait         do not wait
 
 
  examples:
-       nxsetup change\-prop \-n ClientRecordKeys \-t \-w "[\e"phoibos_scan_command\e",\e"phoibos_scan_comment\e"]" NXSRecSelector/r228
-       nxsetup change\-prop \-n DefaultPreselectedComponents \-w "[\e"pinhole1\e",\e"slit2\e"]" NXSRecSelector/r228
-       nxsetup change\-prop \-n StartDsPath \-w "[\e"/usr/bin\e",\e"/usr/lib/tango\e"]" Starter
+       nxsetup change\-prop \-n ClientRecordKeys \-t \-w \(dq[\e\(dqphoibos_scan_command\e\(dq,\e\(dqphoibos_scan_comment\e\(dq]\(dq NXSRecSelector/r228
+       nxsetup change\-prop \-n DefaultPreselectedComponents \-w \(dq[\e\(dqpinhole1\e\(dq,\e\(dqslit2\e\(dq]\(dq NXSRecSelector/r228
+       nxsetup change\-prop \-n StartDsPath \-w \(dq[\e\(dq/usr/bin\e\(dq,\e\(dq/usr/lib/tango\e\(dq]\(dq Starter
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SS nxsetup add\-recorder\-path
 .INDENT 0.0
 .INDENT 3.5
@@ -1805,52 +2528,5168 @@
 
 positional arguments:
   recorder_path  sardana recorder path
 
 optional arguments:
   \-h, \-\-help     show this help message and exit
   \-t, \-\-postpone  do not restart the server
+  \-z TIMEOUT, \-\-timeout TIMEOUT
+                        timeout in seconds
+  \-e, \-\-no\-wait         do not wait
+  \-i INSTANCE, \-\-instance INSTANCE
+                        macroserver instance name, i.e. haso ( default: \(aq*\(aq)
  examples:
        nxsetup add\-recorder\-path /usr/share/pyshared/sardananxsrecorder
        nxsetup add\-recorder\-path \-t /usr/share/pyshared/sardananxsrecorder
 .ft P
 .fi
 .UNINDENT
 .UNINDENT
 .SH NXSTOOLS PACKAGE
 .SS Submodules
+.SS nxstools.filenamegenerator module
+.sp
+Filename generator
+.INDENT 0.0
+.TP
+.B class  nxstools.filenamegenerator.FilenameGenerator(fname_template, start_index=0, stop_index=None)
+Bases: \fI\%object\fP
+.sp
+Generate image file names
+.sp
+(c) Copyright 2015 Eugen Wintersberger <\fI\%eugen.wintersberger@gmail.com\fP>
+(c) Copyright 2015 DESY
+This file is part of nx2img.
+.sp
+nx2img is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 2 of the License, or
+(at your option) any later version.
+.sp
+nx2img is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+.sp
+You should have received a copy of the GNU General Public License
+along with nx2img.  If not, see <\fI\%http://www.gnu.org/licenses/\fP>.
+.sp
+Generator class creating image file names.
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfname_template\fP (\fI\%str\fP) \-\- file name template
+.IP \(bu 2
+\fBstart_index\fP (\fI\%int\fP) \-\- file start index
+.IP \(bu 2
+\fBstop_index\fP (\fI\%int\fP) \-\- file stop index
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B file_index
+(\fI\%int\fP) file start index
+.UNINDENT
+.INDENT 7.0
+.TP
+.B file_template
+(\fI\%str\fP) file name template
+.UNINDENT
+.INDENT 7.0
+.TP
+.B static  from_slice(file_template)
+Static factory method to create a filename_generator instance
+from a sliced user input
+.INDENT 7.0
+.TP
+.B Parameters
+\fBfile_template\fP (\fI\%str\fP) \-\- file template
+.TP
+.B Returns
+filename generator object
+.TP
+.B Return type
+\fI\%FilenameGenerator\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B stop_index
+(\fI\%int\fP) file stop index
+.UNINDENT
+.UNINDENT
+.SS nxstools.filewriter module
+.sp
+Provides abstraction for file writer
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTAttribute(h5object, tparent=None)
+Bases: \fI\%FTObject\fP
+.sp
+virtual file tree attribute
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fI\%FTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  dtype
+attribute data type
+.INDENT 7.0
+.TP
+.B Returns
+attribute data type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B read()
+read attribute value
+.INDENT 7.0
+.TP
+.B Returns
+python object
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  shape
+attribute shape
+.INDENT 7.0
+.TP
+.B Returns
+attribute shape
+.TP
+.B Return type
+\fI\%list\fP < \fI\%int\fP >
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B write(o)
+write attribute value
+.INDENT 7.0
+.TP
+.B Parameters
+\fBo\fP (\fI\%any\fP) \-\- python object
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTAttributeManager(h5object, tparent=None)
+Bases: \fI\%FTObject\fP
+.sp
+file tree attribute
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fI\%FTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create(name, dtype, shape=None, overwrite=False)
+create a new attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- attribute name
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBshape\fP (\fBlist\(ga< :obj:\(gaint\fP>) \-\- attribute shape
+.IP \(bu 2
+\fBoverwrite\fP (\fI\%bool\fP) \-\- overwrite flag
+.UNINDENT
+.TP
+.B Returns
+attribute object
+.TP
+.B Return type
+\fBFTAtribute\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B names()
+key values
+.INDENT 7.0
+.TP
+.B Returns
+attribute names
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen attribute
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTDataFilter(h5object=None, tparent=None)
+Bases: \fI\%FTObject\fP
+.sp
+file tree data filter
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fI\%FTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  availability
+getter for filter availability
+.INDENT 7.0
+.TP
+.B Returns
+filter availability
+.TP
+.B Return type
+\fI\%tuple\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  filterid
+getter for compression filter id
+.INDENT 7.0
+.TP
+.B Returns
+compression rate
+.TP
+.B Return type
+\fI\%int\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  name
+getter for filter name
+.INDENT 7.0
+.TP
+.B Returns
+filter name
+.TP
+.B Return type
+\fI\%tuple\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  options
+getter for compression options
+.INDENT 7.0
+.TP
+.B Returns
+compression options
+.TP
+.B Return type
+\fI\%tuple\fP <\fI\%int\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  rate
+getter for compression rate
+.INDENT 7.0
+.TP
+.B Returns
+compression rate
+.TP
+.B Return type
+\fI\%int\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  shuffle
+getter for compression shuffle
+.INDENT 7.0
+.TP
+.B Returns
+compression shuffle
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTDeflate(h5object=None, tparent=None)
+Bases: \fI\%FTDataFilter\fP
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fI\%FTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTField(h5object, tparent=None)
+Bases: \fI\%FTObject\fP
+.sp
+file writer field
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fI\%FTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  attributes
+return the attribute manager
+.INDENT 7.0
+.TP
+.B Returns
+attribute manager
+.TP
+.B Return type
+\fI\%FTAttributeManager\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  dtype
+field data type
+.INDENT 7.0
+.TP
+.B Returns
+field data type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B grow(dim=0, ext=1)
+grow the field
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBdim\fP (\fI\%int\fP) \-\- growing dimension
+.IP \(bu 2
+\fBdim\fP \-\- size of the grow
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B read()
+read the field value
+.INDENT 7.0
+.TP
+.B Returns
+h5 object
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B refresh()
+refresh the field
+.INDENT 7.0
+.TP
+.B Returns
+refreshed
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  shape
+field shape
+.INDENT 7.0
+.TP
+.B Returns
+field shape
+.TP
+.B Return type
+\fI\%list\fP < \fI\%int\fP >
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  size
+field size
+.INDENT 7.0
+.TP
+.B Returns
+field size
+.TP
+.B Return type
+\fI\%int\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B write(o)
+write the field value
+.INDENT 7.0
+.TP
+.B Parameters
+\fBo\fP (\fI\%any\fP) \-\- h5 object
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTFile(h5object, filename)
+Bases: \fI\%FTObject\fP
+.sp
+file tree file
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBwriter\fP (\fBPNIWriter\fP or \fBH5PYWriter\fP
+or \fBH5CppWriter\fP) \-\- writer module
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B classmethod  currenttime()
+returns current time string
+.INDENT 7.0
+.TP
+.B Returns
+current time
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B default_field()
+field pointed by default attributes
+.INDENT 7.0
+.TP
+.B Returns
+field pointed by default attributes
+.TP
+.B Return type
+\fI\%FTField\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B flush()
+flash the data
+.UNINDENT
+.INDENT 7.0
+.TP
+.B hasswmr()
+if has swmr_mode
+.INDENT 7.0
+.TP
+.B Returns
+has swmr_mode
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B name
+(\fI\%str\fP) file name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  readonly
+check if file is readonly
+.INDENT 7.0
+.TP
+.B Returns
+readonly flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen(readonly=False, swmr=False, libver=None)
+reopen attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBswmr\fP (\fI\%bool\fP) \-\- swmr flag
+.IP \(bu 2
+\fBlibver\fP (\fI\%str\fP) \-\- library version, default: \(aqlatest\(aq
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B root()
+root object
+.INDENT 7.0
+.TP
+.B Returns
+parent object
+.TP
+.B Return type
+\fI\%FTGroup\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTGroup(h5object, tparent=None)
+Bases: \fI\%FTObject\fP
+.sp
+file tree group
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fI\%FTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  attributes
+return the attribute manager
+.INDENT 7.0
+.TP
+.B Returns
+attribute manager
+.TP
+.B Return type
+\fI\%FTAttributeManager\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_field(name, type_code, shape=None, chunk=None, dfilter=None)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBn\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBtype_code\fP (\fI\%str\fP) \-\- nexus field type
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBchunk\fP (\fI\%list\fP < \fI\%int\fP >) \-\- chunk
+.IP \(bu 2
+\fBdfilter\fP (\fI\%FTDeflate\fP) \-\- filter deflater
+.UNINDENT
+.TP
+.B Returns
+file tree field
+.TP
+.B Return type
+\fI\%FTField\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_group(n, nxclass=\(aq\(aq)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBn\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBnxclass\fP (\fI\%str\fP) \-\- group type
+.UNINDENT
+.TP
+.B Returns
+file tree group
+.TP
+.B Return type
+\fI\%FTGroup\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_virtual_field(name, layout, fillvalue=None)
+creates a virtual filed tres element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBlayout\fP (\fBH5CppFieldLayout\fP) \-\- virual field layout
+.IP \(bu 2
+\fBfillvalue\fP (\fI\%int\fP or \fBnp.ndarray\fP) \-\- fill value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B default_field(signals=None, nexuspath=None)
+field pointed by default attributes
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBaxes\fP \-\- axes names
+.IP \(bu 2
+\fBentryname\fP (\fI\%str\fP) \-\- base nexus path to be opened
+.UNINDENT
+.TP
+.B Returns
+field pointed by default attributes
+.TP
+.B Return type
+\fI\%FTField\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B exists(name)
+if child exists
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- child name
+.TP
+.B Returns
+existing flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B names()
+read the child names
+.INDENT 7.0
+.TP
+.B Returns
+h5 object
+.TP
+.B Return type
+\fI\%list\fP <\fIstr\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B open(name)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- element name
+.TP
+.B Returns
+file tree object
+.TP
+.B Return type
+\fI\%FTObject\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B open_link(name)
+open a file tree element as link
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- element name
+.TP
+.B Returns
+file tree object
+.TP
+.B Return type
+\fI\%FTObject\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  size
+group size
+.INDENT 7.0
+.TP
+.B Returns
+group size
+.TP
+.B Return type
+\fI\%int\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B stepsperfile
+(\fI\%int\fP) steps per file
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTHyperslab(offset=None, block=None, count=None, stride=None)
+Bases: \fI\%object\fP
+.sp
+hyperslab class
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoffset\fP (\fI\%tuple\fP <\fI\%int\fP>) \-\- a list of offsets
+.IP \(bu 2
+\fBblock\fP (\fI\%tuple\fP <\fI\%int\fP>) \-\- a list of blocks
+.IP \(bu 2
+\fBcount\fP (\fI\%tuple\fP <\fI\%int\fP>) \-\- a list of counts
+.IP \(bu 2
+\fBstride\fP (\fI\%tuple\fP <\fI\%int\fP>) \-\- a list of strides
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTLink(h5object, tparent=None)
+Bases: \fI\%FTObject\fP
+.sp
+file tree link
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fI\%FTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B refresh()
+refresh the link
+.INDENT 7.0
+.TP
+.B Returns
+refreshed
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  target_path
+target path
+.INDENT 7.0
+.TP
+.B Returns
+target path
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTObject(h5object, tparent=None)
+Bases: \fI\%object\fP
+.sp
+virtual file tree object
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fI\%FTObject\fP) \-\- tree parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B append(child)
+append child weakref
+.INDENT 7.0
+.TP
+.B Parameters
+\fBtparent\fP (\fI\%FTObject\fP) \-\- tree parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close element
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  h5object
+provide object of native library
+.INDENT 7.0
+.TP
+.B Returns
+h5 object
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if attribute is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  parent
+return the parent object
+.INDENT 7.0
+.TP
+.B Returns
+file tree group
+.TP
+.B Return type
+\fI\%FTGroup\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reload()
+reload a list of valid children
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTTargetFieldView(h5object=None)
+Bases: \fI\%FTObject\fP
+.sp
+target field view for VDS
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.filewriter.FTVirtualFieldLayout(h5object=None)
+Bases: \fI\%FTObject\fP
+.sp
+virtual field layout
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.UNINDENT
+.INDENT 7.0
+.TP
+.B add(key, source, sourcekey=None)
+add target field to layout
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBkey\fP (\fI\%tuple\fP) \-\- slide or selection
+.IP \(bu 2
+\fBsource\fP (\fI\%FTTargetFieldView\fP) \-\- target field
+.IP \(bu 2
+\fBsourcekey\fP (\fI\%tuple\fP) \-\- slide or selection
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.create_file(filename, overwrite=False, **pars)
+create a new file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBoverwrite\fP (\fI\%bool\fP) \-\- overwrite flag
+.IP \(bu 2
+\fBpars\fP (\fI\%dict\fP < \fI\%str\fP, \fI\%str\fP>) \-\- parameters
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%FTFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.data_filter(parent=None)
+create deflate filter
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fI\%FTObject\fP) \-\- parent object
+.TP
+.B Returns
+deflate filter object
+.TP
+.B Return type
+\fI\%FTDeflate\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.deflate_filter(parent=None)
+create deflate filter
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fI\%FTObject\fP) \-\- parent object
+.TP
+.B Returns
+deflate filter object
+.TP
+.B Return type
+\fI\%FTDeflate\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.first(array)
+get first element if the only
+.INDENT 7.0
+.TP
+.B Parameters
+\fBarray\fP (\fI\%any\fP) \-\- numpy array
+.TP
+.B Returns
+first element of the array
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.get_links(parent)
+get links
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fI\%FTObject\fP) \-\- parent object
+.TP
+.B Returns
+list of link objects
+.TP
+.B Return type
+.INDENT 7.0
+.TP
+.B obj
+\fIlist\fP <\fI\%FTLink\fP>
+.UNINDENT
+
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.link(target, parent, name)
+create link
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBtarget\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBparent\fP (\fI\%FTObject\fP) \-\- parent object
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- link name
+.UNINDENT
+.TP
+.B Returns
+link object
+.TP
+.B Return type
+\fI\%FTLink\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.load_file(membuffer, filename=None, readonly=False, **pars)
+load a file from memory byte buffer
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBmembuffer\fP (\fI\%bytes\fP or \fI\%io.BytesIO\fP) \-\- memory buffer
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBpars\fP (\fI\%dict\fP < \fI\%str\fP, \fI\%str\fP>) \-\- parameters
+.UNINDENT
+.TP
+.B Returns
+file objects
+.TP
+.B Return type
+\fBH5PYFile\fP or \fBH5CppFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.open_file(filename, readonly=False, **pars)
+open the new file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBpars\fP (\fI\%dict\fP < \fI\%str\fP, \fI\%str\fP>) \-\- parameters
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%FTFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.setwriter(wr)
+sets writer
+.INDENT 7.0
+.TP
+.B Parameters
+\fBwr\fP (\fBPNIWriter\fP or \fBH5PYWriter\fP or \fBH5CppWriter\fP) \-\- writer module
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.target_field_view(filename, fieldpath, shape, dtype=None, maxshape=None, parent=None)
+create target field view for VDS
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBfieldpath\fP (\fI\%str\fP) \-\- nexus field path
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBparent\fP (\fI\%FTObject\fP) \-\- parent object
+.UNINDENT
+.TP
+.B Returns
+target field object
+.TP
+.B Return type
+\fI\%FTTargetFieldView\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.unlimited(parent=None)
+return dataspace UNLIMITED variable for the current writer module
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fI\%FTObject\fP) \-\- parent object
+.TP
+.B Returns
+dataspace UNLIMITED variable
+.TP
+.B Return type
+\fBh5cpp.dataspace.UNLIMITED\fP or \fBh5py.UNLIMITED\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.virtual_field_layout(shape, dtype, maxshape=None, parent=None)
+creates a virtual field layout for a VDS file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBparent\fP (\fI\%FTObject\fP) \-\- parent object
+.UNINDENT
+.TP
+.B Returns
+virtual layout
+.TP
+.B Return type
+\fI\%FTVirtualFieldLayout\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.filewriter.writerlock  =  <unlocked _thread.lock object>
+(\fI\%threading.Lock\fP) writer module
+.UNINDENT
+.SS nxstools.h5cppwriter module
+.sp
+Provides h5cpp file writer
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppAttribute(h5object, tparent=None)
+Bases: \fI\%FTAttribute\fP
+.sp
+file tree attribute
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  dtype
+field data type
+.INDENT 7.0
+.TP
+.B Returns
+field data type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if attribute is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B name
+(\fI\%str\fP) object name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B path
+(\fI\%str\fP) object nexus path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B read()
+read attribute value
+.INDENT 7.0
+.TP
+.B Returns
+python object
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  shape
+attribute shape
+.INDENT 7.0
+.TP
+.B Returns
+attribute shape
+.TP
+.B Return type
+\fI\%list\fP < \fI\%int\fP >
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B write(o)
+write attribute value
+.INDENT 7.0
+.TP
+.B Parameters
+\fBo\fP (\fI\%any\fP) \-\- python object
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppAttributeManager(h5object, tparent=None)
+Bases: \fI\%FTAttributeManager\fP
+.sp
+file tree attribute
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close attribure manager
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create(name, dtype, shape=None, overwrite=False)
+create a new attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- attribute name
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- attribute shape
+.IP \(bu 2
+\fBoverwrite\fP (\fI\%bool\fP) \-\- overwrite flag
+.UNINDENT
+.TP
+.B Returns
+attribute object
+.TP
+.B Return type
+\fBH5CppAtribute\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if link is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B name
+(\fI\%str\fP) object name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B names()
+key values
+.INDENT 7.0
+.TP
+.B Returns
+attribute names
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B path
+(\fI\%str\fP) object nexus path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen field
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppDataFilter(h5object=None, tparent=None)
+Bases: \fI\%FTDataFilter\fP
+.sp
+file tree deflate
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppDeflate(h5object=None, tparent=None)
+Bases: \fI\%H5CppDataFilter\fP
+.sp
+deflate filter
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppField(h5object, tparent=None)
+Bases: \fI\%FTField\fP
+.sp
+file tree file
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  attributes
+return the attribute manager
+.INDENT 7.0
+.TP
+.B Returns
+attribute manager
+.TP
+.B Return type
+\fI\%H5CppAttributeManager\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close field
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  dtype
+field data type
+.INDENT 7.0
+.TP
+.B Returns
+field data type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B grow(dim=0, ext=1)
+grow the field
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBdim\fP (\fI\%int\fP) \-\- growing dimension
+.IP \(bu 2
+\fBdim\fP \-\- size of the grow
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if field is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B name
+(\fI\%str\fP) object name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B path
+(\fI\%str\fP) object nexus path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B read()
+read the field value
+.INDENT 7.0
+.TP
+.B Returns
+h5 object
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B refresh()
+refresh the field
+.INDENT 7.0
+.TP
+.B Returns
+refreshed
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen field
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  shape
+field shape
+.INDENT 7.0
+.TP
+.B Returns
+field shape
+.TP
+.B Return type
+\fI\%list\fP < \fI\%int\fP >
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  size
+field size
+.INDENT 7.0
+.TP
+.B Returns
+field size
+.TP
+.B Return type
+\fI\%int\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B write(o)
+write the field value
+.INDENT 7.0
+.TP
+.B Parameters
+\fBo\fP (\fI\%any\fP) \-\- h5 object
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppFile(h5object, filename)
+Bases: \fI\%FTFile\fP
+.sp
+file tree file
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close file
+.UNINDENT
+.INDENT 7.0
+.TP
+.B filename
+(\fI\%str\fP) nexus file name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B flush()
+flash the data
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if file is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B path
+(\fI\%str\fP) object nexus path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  readonly
+check if file is readonly
+.INDENT 7.0
+.TP
+.B Returns
+readonly flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen(readonly=False, swmr=False, libver=None)
+reopen file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBswmr\fP (\fI\%bool\fP) \-\- swmr flag
+.IP \(bu 2
+\fBlibver\fP (\fI\%str\fP) \-\- library version, default: \(aqlatest\(aq
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B root()
+root object
+.INDENT 7.0
+.TP
+.B Returns
+parent object
+.TP
+.B Return type
+\fI\%H5CppGroup\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppGroup(h5object, tparent=None)
+Bases: \fI\%FTGroup\fP
+.sp
+file tree group
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- tree parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B class  H5CppGroupIter(group)
+Bases: \fI\%object\fP
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBgroup\fP \-\- group object
+.UNINDENT
+.INDENT 7.0
+.TP
+.B next()
+the next attribute
+.INDENT 7.0
+.TP
+.B Returns
+attribute object
+.TP
+.B Return type
+\fBFTAtribute\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  attributes
+return the attribute manager
+.INDENT 7.0
+.TP
+.B Returns
+attribute manager
+.TP
+.B Return type
+\fI\%H5CppAttributeManager\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close group
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_field(name, type_code, shape=None, chunk=None, dfilter=None)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBn\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBtype_code\fP (\fI\%str\fP) \-\- nexus field type
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBchunk\fP (\fI\%list\fP < \fI\%int\fP >) \-\- chunk
+.IP \(bu 2
+\fBdfilter\fP (\fI\%H5CppDataFilter\fP) \-\- filter deflater
+.UNINDENT
+.TP
+.B Returns
+file tree field
+.TP
+.B Return type
+\fI\%H5CppField\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_group(n, nxclass=None)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBn\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBnxclass\fP (\fI\%str\fP) \-\- group type
+.UNINDENT
+.TP
+.B Returns
+file tree group
+.TP
+.B Return type
+\fI\%H5CppGroup\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_virtual_field(name, layout, fillvalue=0)
+creates a virtual filed tres element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- field name
+.IP \(bu 2
+\fBlayout\fP (\fBH5CppFieldLayout\fP) \-\- virual field layout
+.IP \(bu 2
+\fBfillvalue\fP (\fI\%int\fP or \fBnp.ndarray\fP) \-\- fill value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B exists(name)
+if child exists
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- child name
+.TP
+.B Returns
+existing flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if field is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B name
+(\fI\%str\fP) object name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B names()
+read the child names
+.INDENT 7.0
+.TP
+.B Returns
+h5 object
+.TP
+.B Return type
+\fI\%list\fP <\fIstr\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B open(name)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- element name
+.TP
+.B Returns
+file tree object
+.TP
+.B Return type
+\fBFTObject\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B open_link(name)
+open a file tree element as link
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- element name
+.TP
+.B Returns
+file tree object
+.TP
+.B Return type
+\fBFTObject\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B path
+(\fI\%str\fP) object nexus path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen group
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  size
+group size
+.INDENT 7.0
+.TP
+.B Returns
+group size
+.TP
+.B Return type
+\fI\%int\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppLink(h5object, tparent=None)
+Bases: \fI\%FTLink\fP
+.sp
+file tree link
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close group
+.UNINDENT
+.INDENT 7.0
+.TP
+.B classmethod  getfilename(obj)
+provides a filename from h5 node
+.INDENT 7.0
+.TP
+.B Parameters
+\fBobj\fP (\fBFTObject\fP) \-\- h5 node
+.TP
+.B Returns
+file name
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if link is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B name
+(\fI\%str\fP) object name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B path
+(\fI\%str\fP) object nexus path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B refresh()
+refresh the field
+.INDENT 7.0
+.TP
+.B Returns
+refreshed
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen field
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  target_path
+target path
+.INDENT 7.0
+.TP
+.B Returns
+target path
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppTargetFieldView(filename, fieldpath, shape, dtype=None, maxshape=None)
+Bases: \fI\%FTTargetFieldView\fP
+.sp
+target field for VDS
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBfieldpath\fP (\fI\%str\fP) \-\- nexus field path
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B fieldpath
+(\fI\%str\fP) nexus field path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B filename
+(\fI\%str\fP) directory and file name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B maxshape
+(\fI\%list\fP < \fI\%int\fP >) maximal shape
+.UNINDENT
+.INDENT 7.0
+.TP
+.B shape
+(\fI\%list\fP < \fI\%int\fP >) shape
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5cppwriter.H5CppVirtualFieldLayout(h5object, shape, dtype=None, maxshape=None)
+Bases: \fI\%FTVirtualFieldLayout\fP
+.sp
+virtual field layout
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B add(key, source, sourcekey=None, shape=None)
+add target field to layout
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBkey\fP (\fI\%tuple\fP) \-\- slide
+.IP \(bu 2
+\fBsource\fP (\fBH5PYTargetFieldView\fP) \-\- target field view
+.IP \(bu 2
+\fBsourcekey\fP (\fI\%tuple\fP) \-\- slide or selection
+.IP \(bu 2
+\fBshape\fP (\fI\%tuple\fP) \-\- target shape in the layout
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B maxshape
+(\fI\%list\fP < \fI\%int\fP >) maximal shape
+.UNINDENT
+.INDENT 7.0
+.TP
+.B shape
+(\fI\%list\fP < \fI\%int\fP >) shape
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.create_file(filename, overwrite=False, libver=None, swmr=None)
+create a new file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBoverwrite\fP (\fI\%bool\fP) \-\- overwrite flag
+.IP \(bu 2
+\fBlibver\fP (\fI\%str\fP) \-\- library version: \(aqlastest\(aq or \(aqearliest\(aq
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%H5CppFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.data_filter(filterid=None, name=None, options=None, availability=None, shuffle=None, rate=None)
+create data filter
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilterid\fP (\fI\%int\fP) \-\- hdf5 filter id
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- filter name
+.IP \(bu 2
+\fBoptions\fP (\fI\%tuple\fP <\fI\%int\fP>) \-\- filter cd values
+.IP \(bu 2
+\fBavailability\fP (\fI\%str\fP) \-\- filter availability i.e. \(aqoptional\(aq or \(aqmandatory\(aq
+.IP \(bu 2
+\fBshuffle\fP (\fI\%bool\fP) \-\- filter shuffle
+.IP \(bu 2
+\fBrate\fP (\fI\%bool\fP) \-\- filter shuffle
+.UNINDENT
+.TP
+.B Returns
+data filter object
+.TP
+.B Return type
+\fI\%H5CppDataFilter\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.deflate_filter(rate=None, shuffle=None, availability=None)
+create data filter
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBrate\fP (\fI\%bool\fP) \-\- filter shuffle
+.IP \(bu 2
+\fBshuffle\fP (\fI\%bool\fP) \-\- filter shuffle
+.UNINDENT
+.TP
+.B Returns
+deflate filter object
+.TP
+.B Return type
+\fI\%H5CppDataFilter\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.get_links(parent)
+get links
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.TP
+.B Returns
+list of link objects
+.TP
+.B Returns
+link object
+.TP
+.B Return type
+.INDENT 7.0
+.TP
+.B obj
+\fIlist\fP <\fI\%H5CppLink\fP>
+.UNINDENT
+
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.is_image_file_supported()
+provides if loading of image files are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if loading of image files are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.is_unlimited_vds_supported()
+provides if unlimited vds are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if unlimited vds are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.is_vds_supported()
+provides if vds are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if vds are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.link(target, parent, name)
+create link
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBtarget\fP (\fI\%str\fP) \-\- nexus path name
+.IP \(bu 2
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- link name
+.UNINDENT
+.TP
+.B Returns
+link object
+.TP
+.B Return type
+\fI\%H5CppLink\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.load_file(membuffer, filename=None, readonly=False, **pars)
+load a file from memory byte buffer
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBmembuffer\fP (\fI\%bytes\fP or \fI\%io.BytesIO\fP) \-\- memory buffer
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBpars\fP (\fI\%dict\fP < \fI\%str\fP, \fI\%str\fP>) \-\- parameters
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fBH5PYFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.nptype(dtype)
+converts to numpy types
+.INDENT 7.0
+.TP
+.B Parameters
+\fBdtype\fP (\fI\%str\fP) \-\- h5 writer type type
+.TP
+.B Returns
+nupy type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.open_file(filename, readonly=False, libver=None, swmr=False)
+open the new file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBlibver\fP (\fI\%str\fP) \-\- library version: \(aqlastest\(aq or \(aqearliest\(aq
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%H5CppFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.target_field_view(filename, fieldpath, shape, dtype=None, maxshape=None)
+create target field view for VDS
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBfieldpath\fP (\fI\%str\fP) \-\- nexus field path
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.TP
+.B Returns
+target field view object
+.TP
+.B Return type
+\fI\%H5CppTargetFieldView\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.unlimited(parent=None)
+return dataspace UNLIMITED variable for the current writer module
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.TP
+.B Returns
+dataspace UNLIMITED variable
+.TP
+.B Return type
+\fBh5cpp.dataspace.UNLIMITED\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.unlimited_selection(sel, shape)
+checks if hyperslab is unlimited
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBsel\fP (\fBfilewriter.FTHyperslab\fP) \-\- hyperslab selection
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP) \-\- give shape
+.UNINDENT
+.TP
+.B Returns
+if hyperslab is unlimited list
+.TP
+.B Return type
+\fI\%list\fP <\fI\%bool\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5cppwriter.virtual_field_layout(shape, dtype, maxshape=None)
+creates a virtual field layout for a VDS file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.TP
+.B Returns
+virtual layout
+.TP
+.B Return type
+\fI\%H5CppVirtualFieldLayout\fP
+.UNINDENT
+.UNINDENT
+.SS nxstools.h5pywriter module
+.sp
+Provides h5py file writer
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYAttribute(h5object, tparent=None)
+Bases: \fI\%FTAttribute\fP
+.sp
+file tree attribute
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  dtype
+attribute data type
+.INDENT 7.0
+.TP
+.B Returns
+attribute data type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if field is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B read()
+read attribute value
+.INDENT 7.0
+.TP
+.B Returns
+python object
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen attribute
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  shape
+attribute shape
+.INDENT 7.0
+.TP
+.B Returns
+attribute shape
+.TP
+.B Return type
+\fI\%list\fP < \fI\%int\fP >
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B write(o)
+write attribute value
+.INDENT 7.0
+.TP
+.B Parameters
+\fBo\fP (\fI\%any\fP) \-\- python object
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYAttributeManager(h5object, tparent=None)
+Bases: \fI\%FTAttributeManager\fP
+.sp
+file tree attribute
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B class  H5PYAttrIter(manager)
+Bases: \fI\%object\fP
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBmanager\fP (\fI\%H5PYAttributeManager\fP) \-\- attribute manager
+.UNINDENT
+.INDENT 7.0
+.TP
+.B next()
+the next attribute
+.INDENT 7.0
+.TP
+.B Returns
+attribute object
+.TP
+.B Return type
+\fBFTAtribute\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close attribure manager
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create(name, dtype, shape=None, overwrite=False)
+create a new attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- attribute name
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- attribute shape
+.IP \(bu 2
+\fBoverwrite\fP (\fI\%bool\fP) \-\- overwrite flag
+.UNINDENT
+.TP
+.B Returns
+attribute object
+.TP
+.B Return type
+\fBH5PYAtribute\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if link is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B name
+(\fI\%str\fP) object name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B names()
+key values
+.INDENT 7.0
+.TP
+.B Returns
+attribute names
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B path
+(\fI\%str\fP) object nexus path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen field
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYDataFilter(h5object=None, tparent=None)
+Bases: \fI\%FTDataFilter\fP
+.sp
+file tree data filter
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYDeflate(h5object=None, tparent=None)
+Bases: \fI\%H5PYDataFilter\fP
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYField(h5object, tparent=None)
+Bases: \fI\%FTField\fP
+.sp
+file writer field
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  attributes
+return the attribute manager
+.INDENT 7.0
+.TP
+.B Returns
+attribute manager
+.TP
+.B Return type
+\fI\%H5PYAttributeManager\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close field
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  dtype
+field data type
+.INDENT 7.0
+.TP
+.B Returns
+field data type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B grow(dim=0, ext=1)
+grow the field
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBdim\fP (\fI\%int\fP) \-\- growing dimension
+.IP \(bu 2
+\fBdim\fP \-\- size of the grow
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if group is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B read()
+read the field value
+.INDENT 7.0
+.TP
+.B Returns
+h5 object
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B refresh()
+refresh the field
+.INDENT 7.0
+.TP
+.B Returns
+refreshed
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen field
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  shape
+field shape
+.INDENT 7.0
+.TP
+.B Returns
+field shape
+.TP
+.B Return type
+\fI\%list\fP < \fI\%int\fP >
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  size
+field size
+.INDENT 7.0
+.TP
+.B Returns
+field size
+.TP
+.B Return type
+\fI\%int\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B write(o)
+write the field value
+.INDENT 7.0
+.TP
+.B Parameters
+\fBo\fP (\fI\%any\fP) \-\- h5 object
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYFile(h5object, filename)
+Bases: \fI\%FTFile\fP
+.sp
+file tree file
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close file
+.UNINDENT
+.INDENT 7.0
+.TP
+.B flush()
+flash the data
+.UNINDENT
+.INDENT 7.0
+.TP
+.B hasswmr()
+if has swmr_mode
+.INDENT 7.0
+.TP
+.B Returns
+has swmr_mode
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if group is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B path
+(\fI\%str\fP) object nexus path
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  readonly
+check if file is readonly
+.INDENT 7.0
+.TP
+.B Returns
+readonly flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen(readonly=False, swmr=False, libver=None)
+reopen file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBswmr\fP (\fI\%bool\fP) \-\- swmr flag
+.IP \(bu 2
+\fBlibver\fP (\fI\%str\fP) \-\- library version, default: \(aqlatest\(aq
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B root()
+root object
+.INDENT 7.0
+.TP
+.B Returns
+parent object
+.TP
+.B Return type
+\fI\%H5PYGroup\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYGroup(h5object, tparent=None)
+Bases: \fI\%FTGroup\fP
+.sp
+file tree group
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B class  H5PYGroupIter(group)
+Bases: \fI\%object\fP
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBgroup\fP \-\- group object
+.UNINDENT
+.INDENT 7.0
+.TP
+.B next()
+the next attribute
+.INDENT 7.0
+.TP
+.B Returns
+attribute object
+.TP
+.B Return type
+\fBFTAtribute\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  attributes
+return the attribute manager
+.INDENT 7.0
+.TP
+.B Returns
+attribute manager
+.TP
+.B Return type
+\fI\%H5PYAttributeManager\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close group
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_field(name, type_code, shape=None, chunk=None, dfilter=None)
+creates a field tree element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBtype_code\fP (\fI\%str\fP) \-\- nexus field type
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBchunk\fP (\fI\%list\fP < \fI\%int\fP >) \-\- chunk
+.IP \(bu 2
+\fBdfilter\fP (\fI\%H5PYDataFilter\fP) \-\- filter deflater
+.UNINDENT
+.TP
+.B Returns
+file tree field
+.TP
+.B Return type
+\fI\%H5PYField\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_group(n, nxclass=\(aq\(aq)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBn\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBnxclass\fP (\fI\%str\fP) \-\- group type
+.UNINDENT
+.TP
+.B Returns
+file tree group
+.TP
+.B Return type
+\fI\%H5PYGroup\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_virtual_field(name, layout, fillvalue=None)
+creates a virtual filed tres element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBlayout\fP (\fBH5PYFieldLayout\fP) \-\- virual field layout
+.IP \(bu 2
+\fBfillvalue\fP (\fI\%int\fP) \-\- fill value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B exists(name)
+if child exists
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- child name
+.TP
+.B Returns
+existing flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if group is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B names()
+read the child names
+.INDENT 7.0
+.TP
+.B Returns
+h5 object
+.TP
+.B Return type
+\fI\%list\fP <\fIstr\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B open(name)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- element name
+.TP
+.B Returns
+file tree object
+.TP
+.B Return type
+\fBFTObject\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B open_link(name)
+open a file tree element as link
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- element name
+.TP
+.B Returns
+file tree object
+.TP
+.B Return type
+\fBFTObject\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen file
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  size
+group size
+.INDENT 7.0
+.TP
+.B Returns
+group size
+.TP
+.B Return type
+\fI\%int\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYLink(h5object, tparent=None)
+Bases: \fI\%FTLink\fP
+.sp
+file tree link
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close group
+.UNINDENT
+.INDENT 7.0
+.TP
+.B classmethod  getfilename(obj)
+provides a filename from h5 node
+.INDENT 7.0
+.TP
+.B Parameters
+\fBobj\fP (\fBFTObject\fP) \-\- h5 node
+.TP
+.B Returns
+file name
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  is_valid
+check if link is valid
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B read()
+read object value
+.INDENT 7.0
+.TP
+.B Returns
+valid flag
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B refresh()
+refresh the field
+.INDENT 7.0
+.TP
+.B Returns
+refreshed
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B reopen()
+reopen field
+.UNINDENT
+.INDENT 7.0
+.TP
+.B setname(name)
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  target_path
+target path
+.INDENT 7.0
+.TP
+.B Returns
+target path
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYTargetFieldView(h5object, shape)
+Bases: \fI\%FTTargetFieldView\fP
+.sp
+target field view for VDS
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B shape
+(\fI\%list\fP < \fI\%int\fP >) shape
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5pywriter.H5PYVirtualFieldLayout(h5object, shape)
+Bases: \fI\%FTVirtualFieldLayout\fP
+.sp
+virtual field layout
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B add(key, source, sourcekey=None, shape=None)
+add target field to layout
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBkey\fP (\fI\%tuple\fP) \-\- slide
+.IP \(bu 2
+\fBsource\fP (\fI\%H5PYTargetFieldView\fP) \-\- target field view
+.IP \(bu 2
+\fBsourcekey\fP (\fI\%tuple\fP) \-\- slide or selection
+.IP \(bu 2
+\fBshape\fP (\fI\%tuple\fP) \-\- target shape in the layout
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B shape
+(\fI\%list\fP < \fI\%int\fP >) shape
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.create_file(filename, overwrite=False, **pars)
+create a new file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBoverwrite\fP (\fI\%bool\fP) \-\- overwrite flag
+.IP \(bu 2
+\fBpars\fP (\fI\%dict\fP < \fI\%str\fP, \fI\%str\fP>) \-\- parameters
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%H5PYFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.data_filter(filterid=None, name=None, options=None, availability=None, shuffle=None, rate=None)
+create data filter
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilterid\fP (\fI\%int\fP) \-\- hdf5 filter id
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- filter name
+.IP \(bu 2
+\fBoptions\fP (\fI\%tuple\fP <\fI\%int\fP>) \-\- filter cd values
+.IP \(bu 2
+\fBavailability\fP (\fI\%str\fP) \-\- filter availability i.e. \(aqoptional\(aq or \(aqmandatory\(aq
+.IP \(bu 2
+\fBshuffle\fP (\fI\%bool\fP) \-\- filter shuffle
+.IP \(bu 2
+\fBrate\fP (\fI\%bool\fP) \-\- filter shuffle
+.UNINDENT
+.TP
+.B Returns
+deflate filter object
+.TP
+.B Return type
+\fI\%H5PYDataFilter\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.deflate_filter(rate=None, shuffle=None, availability=None)
+create data filter
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBrate\fP (\fI\%bool\fP) \-\- filter shuffle
+.IP \(bu 2
+\fBshuffle\fP (\fI\%bool\fP) \-\- filter shuffle
+.UNINDENT
+.TP
+.B Returns
+deflate filter object
+.TP
+.B Return type
+\fBH5CppDataFilter\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.get_links(parent)
+get links
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.TP
+.B Returns
+list of link objects
+.TP
+.B Returns
+link object
+.TP
+.B Return type
+.INDENT 7.0
+.TP
+.B obj
+\fIlist\fP <\fI\%H5PYLink\fP>
+.UNINDENT
+
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.is_image_file_supported()
+provides if loading of image files are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if loading of image files are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.is_mbs_supported()
+provides if MultiBlockSlice are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if MultiBlockSlice are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.is_strings_as_bytes()
+provides if string read to bytes
+.INDENT 7.0
+.TP
+.B Retruns
+if string read to bytes
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.is_unlimited_vds_supported()
+provides if unlimited vds are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if unlimited vds are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.is_vds_supported()
+provides if VDS are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if VDS are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.link(target, parent, name)
+create link
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBtarget\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- link name
+.UNINDENT
+.TP
+.B Returns
+link object
+.TP
+.B Return type
+\fI\%H5PYLink\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.load_file(membuffer, filename=None, readonly=False, **pars)
+load a file from memory byte buffer
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBmembuffer\fP (\fI\%bytes\fP or \fI\%io.BytesIO\fP) \-\- memory buffer
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBpars\fP (\fI\%dict\fP < \fI\%str\fP, \fI\%str\fP>) \-\- parameters
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%H5PYFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.nptype(dtype)
+converts to numpy types
+.INDENT 7.0
+.TP
+.B Parameters
+\fBdtype\fP (\fI\%str\fP) \-\- h5 writer type type
+.TP
+.B Returns
+nupy type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.open_file(filename, readonly=False, **pars)
+open the new file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBpars\fP (\fI\%dict\fP < \fI\%str\fP, \fI\%str\fP>) \-\- parameters
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%H5PYFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.target_field_view(filename, fieldpath, shape, dtype=None, maxshape=None)
+create target field view for VDS
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBfieldpath\fP (\fI\%str\fP) \-\- nexus field path
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.TP
+.B Returns
+target field view object
+.TP
+.B Return type
+\fBFTTargetFieldView\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.unlimited(parent=None)
+return dataspace UNLIMITED variable for the current writer module
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.TP
+.B Returns
+dataspace UNLIMITED variable
+.TP
+.B Return type
+\fBh5py.h5s.UNLIMITED\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.unlimited_selection(sel, shape)
+checks if hyperslab is unlimited
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBsel\fP (\fBfilewriter.FTHyperslab\fP) \-\- hyperslab selection
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP) \-\- give shape
+.UNINDENT
+.TP
+.B Returns
+if hyperslab is unlimited list
+.TP
+.B Return type
+\fI\%list\fP <\fI\%bool\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5pywriter.virtual_field_layout(shape, dtype, maxshape=None)
+creates a virtual field layout for a VDS file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.TP
+.B Returns
+virtual layout
+.TP
+.B Return type
+\fBFTVirtualFieldLayout\fP
+.UNINDENT
+.UNINDENT
+.SS nxstools.h5rediswriter module
+.sp
+Provides redis h5cpp file writer
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisAttribute(h5object=None, tparent=None, h5imp=None)
+Bases: \fI\%H5CppAttribute\fP
+.sp
+file tree attribute
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTAttribute\fP) \-\- h5 implementation attribute
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisAttributeManager(h5object=None, tparent=None, h5imp=None)
+Bases: \fI\%H5CppAttributeManager\fP
+.sp
+file tree attribute
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTAttributeManager\fP) \-\- h5 implementation attributemanager
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create(name, dtype, shape=None, overwrite=False)
+create a new attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- attribute name
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- attribute shape
+.IP \(bu 2
+\fBoverwrite\fP (\fI\%bool\fP) \-\- overwrite flag
+.UNINDENT
+.TP
+.B Returns
+attribute object
+.TP
+.B Return type
+\fI\%H5RedisAttribute\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisDataFilter(h5object=None, tparent=None, h5imp=None)
+Bases: \fI\%H5CppDataFilter\fP
+.sp
+file tree deflate
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTDataFilter\fP) \-\- h5 implementation data filter
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisDeflate(h5object=None, tparent=None, h5imp=None)
+Bases: \fI\%H5RedisDataFilter\fP
+.sp
+deflate filter
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTDataFilter\fP) \-\- h5 implementation data filter
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisField(h5object=None, tparent=None, h5imp=None)
+Bases: \fI\%H5CppField\fP
+.sp
+file tree file
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTField\fP) \-\- h5 implementation field
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B append_devices(value, keys=None)
+append device parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- device value
+.IP \(bu 2
+\fBkeys\fP \-\- device parameter keys
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B append_scaninfo(value, keys=None, direct=False)
+append scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- scan parameter value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  attributes
+return the attribute manager
+.INDENT 7.0
+.TP
+.B Returns
+attribute manager
+.TP
+.B Return type
+\fBH5CppAttributeManager\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_channels(value, keys=None)
+get scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+\fBkeys\fP \-\- device parameter keys
+.TP
+.B Returns value
+device parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_devices(value, keys=None)
+get scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+\fBkeys\fP \-\- device parameter keys
+.TP
+.B Returns value
+device parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_scaninfo(keys=None, direct=False)
+get scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+\fBkeys\fP \-\- scan parameter value
+.TP
+.B Returns value
+scan parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_command(command, *args, **kwargs)
+set scan attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBcommand\fP (\fI\%str\fP) \-\- scan command
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP <\fIany\fP>) \-\- function list arguments
+.IP \(bu 2
+\fBkwargs\fP (\fI\%dict\fP <\fI\%str\fP , \fIany\fP>) \-\- function dict arguments
+.UNINDENT
+.TP
+.B Returns
+scan command value
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_getattr(attr)
+get scan attribute
+.INDENT 7.0
+.TP
+.B Parameters
+\fBattr\fP (\fI\%str\fP) \-\- scan attr
+.TP
+.B Returns
+scan attr value
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_setattr(attr, value)
+set attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBattr\fP (\fI\%str\fP) \-\- scan attr
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan attr value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_channels(value, keys=None)
+set device parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- device parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- device parameter keys
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_devices(value, keys=None)
+set device parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- device parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- device parameter keys
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_scan(scan)
+scan object
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBscan\fP \-\- scan object
+.IP \(bu 2
+\fBtype\fP \-\- \fBScan\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_scaninfo(value, keys=None, direct=False)
+set scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- scan parameter value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisFile(h5object=None, filename=None, h5imp=None, redisurl=None)
+Bases: \fI\%H5CppFile\fP
+.sp
+file tree file
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTFile\fP) \-\- h5 implementation file
+.IP \(bu 2
+\fBredisurl\fP (\fI\%str\fP) \-\- redis url string
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B append_devices(value, keys=None)
+append device info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- device parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- device parameter value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B append_scaninfo(value, keys=None, direct=False)
+append scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- scan parameter value
+.IP \(bu 2
+\fBdirect\fP (\fI\%any\fP) \-\- scan info direct flag
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_channels(keys=None)
+get channel info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+\fBkeys\fP \-\- channel parameter keys
+.TP
+.B Returns value
+channel parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_devices(keys=None)
+get devices info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+\fBkeys\fP \-\- device parameter keys
+.TP
+.B Returns value
+device parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_scaninfo(keys=None, direct=False)
+get scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBkeys\fP \-\- scan parameter value
+.IP \(bu 2
+\fBdirect\fP (\fI\%any\fP) \-\- scan info direct flag
+.UNINDENT
+.TP
+.B Returns value
+scan parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B prepare()
+start scan
+.UNINDENT
+.INDENT 7.0
+.TP
+.B root()
+root object
+.INDENT 7.0
+.TP
+.B Returns
+parent object
+.TP
+.B Return type
+\fI\%H5RedisGroup\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_command(command, *args, **kwargs)
+set scan attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBcommand\fP (\fI\%str\fP) \-\- scan command
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP <\fIany\fP>) \-\- function list arguments
+.IP \(bu 2
+\fBkwargs\fP (\fI\%dict\fP <\fI\%str\fP , \fIany\fP>) \-\- function dict arguments
+.UNINDENT
+.TP
+.B Returns
+scan command value
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_getattr(attr)
+get scan attribute
+.INDENT 7.0
+.TP
+.B Parameters
+\fBattr\fP (\fI\%str\fP) \-\- scan attr
+.TP
+.B Returns
+scan attr value
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_setattr(attr, value)
+set attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBattr\fP (\fI\%str\fP) \-\- scan attr
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan attr value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_channels(value, keys=None)
+set channel info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- channel parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- channel parameter keys
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_devices(value, keys=None)
+set device info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- device parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- device parameter keys
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_entryname(entryname)
+set entry name
+.INDENT 7.0
+.TP
+.B Parameters
+\fBentryname\fP (\fI\%str\fP) \-\- entry name
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_insname(insname)
+set instrument name
+.INDENT 7.0
+.TP
+.B Parameters
+\fBinsname\fP (\fI\%str\fP) \-\- instrument name
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_scan(scan)
+scan object
+.INDENT 7.0
+.TP
+.B Parameters
+\fBscan\fP (\fBScan\fP) \-\- scan object
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_scaninfo(value, keys=None, direct=False)
+set scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- scan parameter value
+.IP \(bu 2
+\fBdirect\fP (\fI\%any\fP) \-\- scan info direct flag
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B start()
+start scan
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisGroup(h5object=None, tparent=None, h5imp=None, nxclass=None)
+Bases: \fI\%H5CppGroup\fP
+.sp
+file tree group
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- tree parent
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTGroup\fP) \-\- h5 implementation group
+.IP \(bu 2
+\fBredis\fP (\fI\%any\fP) \-\- redis object
+.IP \(bu 2
+\fBnxclass\fP (\fI\%str\fP) \-\- nxclass
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B class  H5RedisGroupIter(group=None)
+Bases: \fI\%object\fP
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBgroup\fP (\fI\%H5RedisGroup\fP) \-\- group object
+.UNINDENT
+.INDENT 7.0
+.TP
+.B next()
+the next attribute
+.INDENT 7.0
+.TP
+.B Returns
+attribute object
+.TP
+.B Return type
+\fBFTAtribute\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B append_devices(value, keys=None)
+append device parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- device value
+.IP \(bu 2
+\fBkeys\fP \-\- device parameter keys
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B append_scaninfo(value, keys=None, direct=False)
+append scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- scan parameter keys
+.IP \(bu 2
+\fBdirect\fP (\fI\%any\fP) \-\- scan info direct flag
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B property  attributes
+return the attribute manager
+.INDENT 7.0
+.TP
+.B Returns
+attribute manager
+.TP
+.B Return type
+\fBH5CppAttributeManager\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B close()
+close the group
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_field(name, type_code, shape=None, chunk=None, dfilter=None)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBn\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBtype_code\fP (\fI\%str\fP) \-\- nexus field type
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBchunk\fP (\fI\%list\fP < \fI\%int\fP >) \-\- chunk
+.IP \(bu 2
+\fBdfilter\fP (\fBH5CppDataFilter\fP) \-\- filter deflater
+.UNINDENT
+.TP
+.B Returns
+file tree field
+.TP
+.B Return type
+\fI\%H5RedisField\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_group(n, nxclass=None)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBn\fP (\fI\%str\fP) \-\- group name
+.IP \(bu 2
+\fBnxclass\fP (\fI\%str\fP) \-\- group type
+.UNINDENT
+.TP
+.B Returns
+file tree group
+.TP
+.B Return type
+\fI\%H5RedisGroup\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create_virtual_field(name, layout, fillvalue=0)
+creates a virtual filed tres element
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- field name
+.IP \(bu 2
+\fBlayout\fP (\fBH5CppFieldLayout\fP) \-\- virual field layout
+.IP \(bu 2
+\fBfillvalue\fP (\fI\%int\fP or \fBnp.ndarray\fP) \-\- fill value
+.UNINDENT
+.TP
+.B Returns
+file tree field
+.TP
+.B Return type
+\fI\%H5RedisField\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_channels(value, keys=None)
+get scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+\fBkeys\fP \-\- device parameter keys
+.TP
+.B Returns value
+device parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_devices(value, keys=None)
+get scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+\fBkeys\fP \-\- device parameter keys
+.TP
+.B Returns value
+device parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B get_scaninfo(keys=None, direct=False)
+get scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBkeys\fP \-\- scan parameter keys
+.IP \(bu 2
+\fBdirect\fP (\fI\%any\fP) \-\- scan info direct flag
+.UNINDENT
+.TP
+.B Returns value
+scan parameter value
+.TP
+.B Rtype value
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B open(name)
+open a file tree element
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- element name
+.TP
+.B Returns
+file tree object
+.TP
+.B Return type
+\fI\%H5RedisLink\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B open_link(name)
+open a file tree element as link
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- element name
+.TP
+.B Returns
+file tree object
+.TP
+.B Return type
+\fI\%H5RedisLink\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_command(command, *args, **kwargs)
+set scan attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBcommand\fP (\fI\%str\fP) \-\- scan command
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP <\fIany\fP>) \-\- function list arguments
+.IP \(bu 2
+\fBkwargs\fP (\fI\%dict\fP <\fI\%str\fP , \fIany\fP>) \-\- function dict arguments
+.UNINDENT
+.TP
+.B Returns
+scan command value
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_getattr(attr)
+get scan attribute
+.INDENT 7.0
+.TP
+.B Parameters
+\fBattr\fP (\fI\%str\fP) \-\- scan attr
+.TP
+.B Returns
+scan attr value
+.TP
+.B Return type
+\fI\%any\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scan_setattr(attr, value)
+set attribute
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBattr\fP (\fI\%str\fP) \-\- scan attr
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan attr value
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_channels(value, keys=None)
+set device parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- device parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- device parameter keys
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_devices(value, keys=None)
+set device parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- device parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- device parameter keys
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_entryname(entryname)
+set entry name
+.INDENT 7.0
+.TP
+.B Parameters
+\fBentryname\fP (\fI\%str\fP) \-\- entry name
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_insname(insname)
+set instrument name
+.INDENT 7.0
+.TP
+.B Parameters
+\fBinsname\fP (\fI\%str\fP) \-\- instrument name
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_scan(scan)
+scan object
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBscan\fP \-\- scan object
+.IP \(bu 2
+\fBtype\fP \-\- \fBScan\fP
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B set_scaninfo(value, keys=None, direct=False)
+set scan info parameters
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBvalue\fP (\fI\%any\fP) \-\- scan parameter value
+.IP \(bu 2
+\fBkeys\fP \-\- scan parameter keys
+.IP \(bu 2
+\fBdirect\fP (\fI\%any\fP) \-\- scan info direct flag
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisLink(h5object=None, tparent=None, h5imp=None)
+Bases: \fI\%H5CppLink\fP
+.sp
+file tree link
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBtparent\fP (\fBFTObject\fP) \-\- treee parent
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisTargetFieldView(filename=None, fieldpath=None, shape=None, dtype=None, maxshape=None, h5imp=None)
+Bases: \fI\%H5CppTargetFieldView\fP
+.sp
+target field for VDS
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBfieldpath\fP (\fI\%str\fP) \-\- nexus field path
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTTargetFieldView\fP) \-\- h5 implementation targetfieldview
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.h5rediswriter.H5RedisVirtualFieldLayout(h5object=None, shape=None, dtype=None, maxshape=None, h5imp=None)
+Bases: \fI\%H5CppVirtualFieldLayout\fP
+.sp
+virtual field layout
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBh5object\fP (\fI\%any\fP) \-\- h5 object
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBh5imp\fP (\fBfilewriter.FTVirtualFieldLayout\fP) \-\- h5 implementation  virtual field layout
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.create_file(filename, overwrite=False, redisurl=None, **pars)
+create a new file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBoverwrite\fP (\fI\%bool\fP) \-\- overwrite flag
+.IP \(bu 2
+\fBlibver\fP (\fI\%str\fP) \-\- library version: \(aqlastest\(aq or \(aqearliest\(aq
+.IP \(bu 2
+\fBredisurl\fP (\fI\%str\fP) \-\- redis URL
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%H5RedisFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.data_filter(filterid=None, name=None, options=None, availability=None, shuffle=None, rate=None)
+create data filter
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilterid\fP (\fI\%int\fP) \-\- hdf5 filter id
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- filter name
+.IP \(bu 2
+\fBoptions\fP (\fI\%tuple\fP <\fI\%int\fP>) \-\- filter cd values
+.IP \(bu 2
+\fBavailability\fP (\fI\%str\fP) \-\- filter availability i.e. \(aqoptional\(aq or \(aqmandatory\(aq
+.IP \(bu 2
+\fBshuffle\fP (\fI\%bool\fP) \-\- filter shuffle
+.IP \(bu 2
+\fBrate\fP (\fI\%bool\fP) \-\- filter shuffle
+.UNINDENT
+.TP
+.B Returns
+data filter object
+.TP
+.B Return type
+\fI\%H5RedisDataFilter\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.deflate_filter(rate=None, shuffle=None, availability=None)
+create data filter
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBrate\fP (\fI\%bool\fP) \-\- filter shuffle
+.IP \(bu 2
+\fBshuffle\fP (\fI\%bool\fP) \-\- filter shuffle
+.UNINDENT
+.TP
+.B Returns
+deflate filter object
+.TP
+.B Return type
+\fI\%H5RedisDataFilter\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.get_links(parent)
+get links
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.TP
+.B Returns
+list of link objects
+.TP
+.B Returns
+link object
+.TP
+.B Return type
+.INDENT 7.0
+.TP
+.B obj
+\fIlist\fP <\fI\%H5RedisLink\fP>
+.UNINDENT
+
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.is_image_file_supported()
+provides if loading of image files are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if loading of image files are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.is_unlimited_vds_supported()
+provides if unlimited vds are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if unlimited vds are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.is_vds_supported()
+provides if vds are supported
+.INDENT 7.0
+.TP
+.B Retruns
+if vds are supported
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.link(target, parent, name)
+create link
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBtarget\fP (\fI\%str\fP) \-\- nexus path name
+.IP \(bu 2
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- link name
+.UNINDENT
+.TP
+.B Returns
+link object
+.TP
+.B Return type
+\fI\%H5RedisLink\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.load_file(membuffer, filename=None, readonly=False, **pars)
+load a file from memory byte buffer
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBmembuffer\fP (\fI\%bytes\fP or \fI\%io.BytesIO\fP) \-\- memory buffer
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBpars\fP (\fI\%dict\fP < \fI\%str\fP, \fI\%str\fP>) \-\- parameters
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%H5RedisFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.nptype(dtype)
+converts to numpy types
+.INDENT 7.0
+.TP
+.B Parameters
+\fBdtype\fP (\fI\%str\fP) \-\- h5 writer type type
+.TP
+.B Returns
+nupy type
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.open_file(filename, readonly=False, redisurl=None, **pars)
+open the new file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBreadonly\fP (\fI\%bool\fP) \-\- readonly flag
+.IP \(bu 2
+\fBredisurl\fP (\fI\%str\fP) \-\- redis URL
+.IP \(bu 2
+\fBlibver\fP (\fI\%str\fP) \-\- library version: \(aqlastest\(aq or \(aqearliest\(aq
+.UNINDENT
+.TP
+.B Returns
+file object
+.TP
+.B Return type
+\fI\%H5RedisFile\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.target_field_view(filename, fieldpath, shape, dtype=None, maxshape=None)
+create target field view for VDS
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- file name
+.IP \(bu 2
+\fBfieldpath\fP (\fI\%str\fP) \-\- nexus field path
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.TP
+.B Returns
+target field view object
+.TP
+.B Return type
+\fI\%H5RedisTargetFieldView\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.unlimited(parent=None)
+return dataspace UNLIMITED variable for the current writer module
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparent\fP (\fBFTObject\fP) \-\- parent object
+.TP
+.B Returns
+dataspace UNLIMITED variable
+.TP
+.B Return type
+\fBh5cpp.dataspace.UNLIMITED\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.unlimited_selection(sel, shape)
+checks if hyperslab is unlimited
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBsel\fP (\fBfilewriter.FTHyperslab\fP) \-\- hyperslab selection
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP) \-\- give shape
+.UNINDENT
+.TP
+.B Returns
+if hyperslab is unlimited list
+.TP
+.B Return type
+\fI\%list\fP <\fI\%bool\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.h5rediswriter.virtual_field_layout(shape, dtype, maxshape=None)
+creates a virtual field layout for a VDS file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.IP \(bu 2
+\fBdtype\fP (\fI\%str\fP) \-\- attribute type
+.IP \(bu 2
+\fBmaxshape\fP (\fI\%list\fP < \fI\%int\fP >) \-\- shape
+.UNINDENT
+.TP
+.B Returns
+virtual layout
+.TP
+.B Return type
+\fI\%H5RedisVirtualFieldLayout\fP
+.UNINDENT
+.UNINDENT
+.SS nxstools.nxsargparser module
+.sp
+NeXus tool argumen parser
+.INDENT 0.0
+.TP
+.B exception  nxstools.nxsargparser.ErrorException
+Bases: \fI\%Exception\fP
+.sp
+error parser exception
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxsargparser.NXSArgParser(**kwargs)
+Bases: \fI\%ArgumentParser\fP
+.sp
+Argument parser with error exception
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBkwargs\fP \-\- \fI\%argparse.ArgumentParser\fP
+parameter dictionary
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createSubParsers()
+creates command\-line parameters parser
+.INDENT 7.0
+.TP
+.B Returns
+command runner
+.TP
+.B Return type
+\fI\%Runner\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B error(message)
+error handler
+.INDENT 7.0
+.TP
+.B Parameters
+\fBmessage\fP (\fI\%str\fP) \-\- error message
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxsargparser.Runner(parser)
+Bases: \fI\%object\fP
+.sp
+abstract runner
+.sp
+parser creator
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+parser creator
+.UNINDENT
+.INDENT 7.0
+.TP
+.B description  =  \(aqabstract runner\(aq
+(\fI\%str\fP) command description
+.UNINDENT
+.INDENT 7.0
+.TP
+.B epilog  =  None
+(\fI\%str\fP) command epilog
+.UNINDENT
+.INDENT 7.0
+.TP
+.B postauto()
+parser creator after autocomplete run
+.UNINDENT
+.INDENT 7.0
+.TP
+.B run(options)
+run commandthe main program function
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.UNINDENT
+.UNINDENT
+.UNINDENT
 .SS nxstools.nxscollect module
 .sp
 Command\-line tool to merge images of external file\-formats
 into the master NeXus file
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.Collector(nexusfilename, compression=2, skipmissing=False, storeold=False, testmode=False, writer=None)
+.B class  nxstools.nxscollect.Collector(nexusfilename, compression=2, skipmissing=False, storeold=False, testmode=False, writer=None)
 Bases: \fI\%object\fP
 .sp
 Collector merge images of external file\-formats
 into the master NeXus file
 .sp
 The constructor creates the collector object
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBnexusfilename\fP (\fI\%str\fP) – the nexus file name
+\fBnexusfilename\fP (\fI\%str\fP) \-\- the nexus file name
 .IP \(bu 2
-\fBcompression\fP (\fI\%int\fP) – compression rate
+\fBcompression\fP (\fI\%int\fP) \-\- compression rate
 .IP \(bu 2
-\fBskipmissing\fP (\fI\%bool\fP) – if skip missing images
+\fBskipmissing\fP (\fI\%bool\fP) \-\- if skip missing images
 .IP \(bu 2
-\fBstoreold\fP (\fI\%bool\fP) – if backup the input file
+\fBstoreold\fP (\fI\%bool\fP) \-\- if backup the input file
 .IP \(bu 2
-\fBtestmode\fP (\fI\%bool\fP) – if run in a test mode
+\fBtestmode\fP (\fI\%bool\fP) \-\- if run in a test mode
 .IP \(bu 2
-\fBwriter\fP (\fI\%str\fP) – the writer module
+\fBwriter\fP (\fI\%str\fP) \-\- the writer module
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B collect(path=None, inputfiles=None, datatype=None, shape=None)
 creates a temporary file,
 collects the all image files defined by hdf5
@@ -1858,376 +7697,376 @@
 to the origin one if the action was successful
 or appends specific data if path and inputfiles are given
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBpath\fP (\fI\%str\fP) – nexus path of the data field
+\fBpath\fP (\fI\%str\fP) \-\- nexus path of the data field
 .IP \(bu 2
-\fBinputfiles\fP (\fI\%list\fP <\fI\%str\fP>) – a list of file strings
+\fBinputfiles\fP (\fI\%list\fP <\fI\%str\fP>) \-\- a list of file strings
 .IP \(bu 2
-\fBdatatype\fP (\fI\%str\fP) – field data type
+\fBdatatype\fP (\fI\%str\fP) \-\- field data type
 .IP \(bu 2
-\fBshape\fP (\fI\%list\fP <\fI\%int\fP >) – field shape
+\fBshape\fP (\fI\%list\fP <\fI\%int\fP >) \-\- field shape
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.Execute(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscollect.Execute(parser)
+Bases: \fI\%Runner\fP
 .sp
 Execute runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqappend images to the master file\(aq
+.B description  =  \(aqappend images to the master file\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " examples:\en       nxscollect append \-c1 /tmp/gpfs/raw/scan_234.nxs \en\en       nxscollect append \-c32008:0,2 /ramdisk/scan_123.nxs \en\en       nxscollect append \-\-test /tmp/gpfs/raw/scan_234.nxs \en\en       nxscollect append scan_234.nxs \-\-path /scan/instrument/pilatus/data  \-\-input\-files \(aqscan_%05d.tif:0:100\(aq \en"
+.B epilog  =  \(dq examples:\en       nxscollect append \-c1 /tmp/gpfs/raw/scan_234.nxs \en\en       nxscollect append \-c32008:0,2 /ramdisk/scan_123.nxs \en\en       nxscollect append \-\-test /tmp/gpfs/raw/scan_234.nxs \en\en       nxscollect append scan_234.nxs \-\-path /scan/instrument/pilatus/data  \-\-input\-files \(aqscan_%05d.tif:0:100\(aq \en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.LayoutField(target, hyperslab=None)
+.B class  nxstools.nxscollect.LayoutField(target, hyperslab=None)
 Bases: \fI\%object\fP
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBhyperslab\fP (\fBfilewriter.FTHyperslab\fP) – target field object
+\fBhyperslab\fP (\fBfilewriter.FTHyperslab\fP) \-\- target field object
 .IP \(bu 2
-\fBhyperslab\fP – field hyperslab or slices
+\fBhyperslab\fP \-\- field hyperslab or slices
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B hyperslab = None
+.B hyperslab
 \fBfilewriter.FTHyperslab\fP layout hyperslab or slices
 .UNINDENT
 .INDENT 7.0
 .TP
-.B shape = None
+.B shape
 \fI\%tuple\fP vds shape in layout
 .UNINDENT
 .INDENT 7.0
 .TP
-.B slices = None
+.B slices
 \fI\%list\fP <\fI\%slice\fP>
 .UNINDENT
 .INDENT 7.0
 .TP
-.B target = None
+.B target
 \fI\%TargetFieldView\fP target field object
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.Link(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscollect.Link(parser)
+Bases: \fI\%Runner\fP
 .sp
 Execute runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate an external or internal link in the master file\(aq
+.B description  =  \(aqcreate an external or internal link in the master file\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxscollect link scan_234.nxs://entry/instrument/lambda \-\-name data \-\-target scan_234/lambda.nxs://entry/data/data \en\enscan_234.nxs://entry/instrument/eiger:NXdetector   \-\-target scan_234/eiger.nxs://entry/data/data \en\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxscollect link scan_234.nxs://entry/instrument/lambda \-\-name data \-\-target scan_234/lambda.nxs://entry/data/data \en\enscan_234.nxs://entry/instrument/eiger:NXdetector   \-\-target scan_234/eiger.nxs://entry/data/data \en\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.Linker(nexusfilepath, target, name=None, storeold=False, testmode=False, writer=None)
+.B class  nxstools.nxscollect.Linker(nexusfilepath, target, name=None, storeold=False, testmode=False, writer=None)
 Bases: \fI\%object\fP
 .sp
 Create external and internal links of NeXus files
 .sp
 The constructor creates the collector object
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBnexusfilepath\fP (\fI\%str\fP) – the nexus file name and nexus path
+\fBnexusfilepath\fP (\fI\%str\fP) \-\- the nexus file name and nexus path
 .IP \(bu 2
-\fBtarget\fP (\fI\%str\fP) – the nexus file name and nexus path
+\fBtarget\fP (\fI\%str\fP) \-\- the nexus file name and nexus path
 .IP \(bu 2
-\fBstoreold\fP (\fI\%bool\fP) – if backup the input file
+\fBstoreold\fP (\fI\%bool\fP) \-\- if backup the input file
 .IP \(bu 2
-\fBtestmode\fP (\fI\%bool\fP) – if run in a test mode
+\fBtestmode\fP (\fI\%bool\fP) \-\- if run in a test mode
 .IP \(bu 2
-\fBwriter\fP (\fI\%str\fP) – the writer module
+\fBwriter\fP (\fI\%str\fP) \-\- the writer module
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B link()
 creates NeXus link
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.TargetFieldView(filename, path, shape=None, hyperslab=None, maxshape=None)
+.B class  nxstools.nxscollect.TargetFieldView(filename, path, shape=None, hyperslab=None, maxshape=None)
 Bases: \fI\%object\fP
 .sp
 target field map
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBfilename\fP (\fI\%str\fP) – file name
+\fBfilename\fP (\fI\%str\fP) \-\- file name
 .IP \(bu 2
-\fBpath\fP (\fI\%str\fP) – nexus field path with its name
+\fBpath\fP (\fI\%str\fP) \-\- nexus field path with its name
 .IP \(bu 2
-\fBshape\fP (\fI\%list\fP <\fI\%int\fP>) – field shape
+\fBshape\fP (\fI\%list\fP <\fI\%int\fP>) \-\- field shape
 .IP \(bu 2
-\fBhyperslab\fP (\fBfilewriter.FTHyperslab\fP) – field hyperslab or slices
+\fBhyperslab\fP (\fBfilewriter.FTHyperslab\fP) \-\- field hyperslab or slices
 .IP \(bu 2
-\fBmaxshape\fP (\fI\%list\fP <\fI\%int\fP>) – maximal field shape
+\fBmaxshape\fP (\fI\%list\fP <\fI\%int\fP>) \-\- maximal field shape
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B filename = None
+.B filename
 \fI\%str\fP file name
 .UNINDENT
 .INDENT 7.0
 .TP
-.B hyperslab = None
+.B hyperslab
 \fBfilewriter.FTHyperslab\fP field hyperslab or slices
 .UNINDENT
 .INDENT 7.0
 .TP
-.B maxshape = None
+.B maxshape
 \fI\%list\fP <\fI\%int\fP> field maximal shape
 .UNINDENT
 .INDENT 7.0
 .TP
-.B path = None
+.B path
 \fI\%str\fP nexus field path with its name
 .UNINDENT
 .INDENT 7.0
 .TP
-.B shape = None
+.B shape
 \fI\%list\fP <\fI\%int\fP> field shape
 .UNINDENT
 .INDENT 7.0
 .TP
-.B slices = None
+.B slices
 \fI\%list\fP <\fI\%slice\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.TargetFieldsLayout(exfieldpaths=\(aq\(aq, exfieldshapes=\(aq\(aq, shapes=None, separator=\(aq, \(aq)
+.B class  nxstools.nxscollect.TargetFieldsLayout(exfieldpaths=\(aq\(aq, exfieldshapes=\(aq\(aq, shapes=None, separator=\(aq,\(aq)
 Bases: \fI\%list\fP
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBexfieldpaths\fP (\fI\%str\fP) – target field paths
+\fBexfieldpaths\fP (\fI\%str\fP) \-\- target field paths
 .IP \(bu 2
-\fBexfieldshapes\fP (\fI\%str\fP) – target field shapes
+\fBexfieldshapes\fP (\fI\%str\fP) \-\- target field shapes
 .IP \(bu 2
-\fBshapes\fP (\fBlist\(ga<:obj:\(gatuple\(ga<:obj:\(gaint\fP> >) – target field shapes
+\fBshapes\fP (\fBlist\(ga<:obj:\(gatuple\(ga<:obj:\(gaint\fP> >) \-\- target field shapes
 .IP \(bu 2
-\fBexfieldpaths\fP – separator of field path strings
+\fBexfieldpaths\fP \-\- separator of field path strings
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B add_layout_hyperslabs(offsets, blocks, counts, strides)
 add layout hyperslabs
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoffsets\fP (\fI\%str\fP) – layout offsets
+\fBoffsets\fP (\fI\%str\fP) \-\- layout offsets
 .IP \(bu 2
-\fBblocks\fP (\fI\%str\fP) – layout blocks
+\fBblocks\fP (\fI\%str\fP) \-\- layout blocks
 .IP \(bu 2
-\fBcounts\fP (\fI\%str\fP) – layout counts
+\fBcounts\fP (\fI\%str\fP) \-\- layout counts
 .IP \(bu 2
-\fBstrides\fP (\fI\%str\fP) – layout strides
+\fBstrides\fP (\fI\%str\fP) \-\- layout strides
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B add_layout_slices(slices)
 add layout slices
 .INDENT 7.0
 .TP
 .B Parameters
-\fBslices\fP (\fI\%str\fP) – layout slices
+\fBslices\fP (\fI\%str\fP) \-\- layout slices
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B add_target_hyperslabs(offsets, blocks, counts, strides)
 add target hyperslabs
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoffsets\fP (\fI\%str\fP) – target offsets
+\fBoffsets\fP (\fI\%str\fP) \-\- target offsets
 .IP \(bu 2
-\fBblocks\fP (\fI\%str\fP) – target blocks
+\fBblocks\fP (\fI\%str\fP) \-\- target blocks
 .IP \(bu 2
-\fBcounts\fP (\fI\%str\fP) – target counts
+\fBcounts\fP (\fI\%str\fP) \-\- target counts
 .IP \(bu 2
-\fBstrides\fP (\fI\%str\fP) – target strides
+\fBstrides\fP (\fI\%str\fP) \-\- target strides
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B add_target_slices(slices)
 add taget slices
 .INDENT 7.0
 .TP
 .B Parameters
-\fBslices\fP (\fI\%str\fP) – target slices
+\fBslices\fP (\fI\%str\fP) \-\- target slices
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.VDS(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscollect.VDS(parser)
+Bases: \fI\%Runner\fP
 .sp
 Execute runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate a virual dataset in the master file\(aq
+.B description  =  \(aqcreate a virual dataset in the master file\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " examples:\en\en       nxscollect vds scan_234.nxs://entry/instrument/eiger/data  \-\-shape \(aq1000,2048,1024\(aq \-\-dtype uint32  \-\-target\-fields \(aqeiger_%05d.nxs://entry/data/data:1:10\(aq \-\-shapes \(aq100,,:100,,:100,,:100,,:100,,:100,,:100,,:100,,:100,,:100,,\(aq   \-\-offsets \(aq0,,:100,,:200,,:300,,:400,,:500,,:600,,:700,,:800,,:900,,\(aq \en\en\en           \- creates VDS (shape [1000,2048,1024]) of ten nexus files (shape [100,2048,1024]) merged in their first dimension\en\en\en\en       nxscollect vds scan_234.nxs://entry/instrument/lambda/data  \-\-shape \(aq100,300,762\(aq \-\-dtype uint32  \-\-target\-fields \(aqlambda_%05d.nxs://entry/data/data:0:2\(aq \-\-shapes \(aq,,250:,,250:,,250\(aq   \-\-offsets \(aq,,:,,256:,,512\(aq  \-\-counts \(aqU,,:U,,:U,,\(aq \-f 1 \en\en\en           \- creates VDS (shape [100,300,762]) of three nexus files (shape [100,300,250]) merged in their third dimension,\en               separated with a 6 pixel gap of 1 values and unlimited first dimension\en\en\en\en       nxscollect vds scan_234.nxs://entry/instrument/percival/data  \-\-shape \(aq4000,1600,2000\(aq \-\-dtype int16  \-\-target\-fields \(aqpercival_%05d.nxs://entry/data/data:1:4\(aq \-\-shapes \(aq1000,,:1000,,:1000,,:1000,,\(aq   \-\-offsets \(aq0,,:1,,:2,,:3,,\(aq  \-\-counts \(aqU,,:U,,:U,,:U,,\(aq \-\-strides \(aq4,,:4,,:4,,:4,,\(aq \en\en\en           \- creates VDS (shape [1000,1600,2000]) of three nexus files (shape [1000,1600,2000])\en                merged in their the first dimension with interlaying frames\en                and unlimited first dimension\en\en\en\en"
+.B epilog  =  \(dq examples:\en\en       nxscollect vds scan_234.nxs://entry/instrument/eiger/data  \-\-shape \(aq1000,2048,1024\(aq \-\-dtype uint32  \-\-target\-fields \(aqeiger_%05d.nxs://entry/data/data:1:10\(aq \-\-shapes \(aq100,,:100,,:100,,:100,,:100,,:100,,:100,,:100,,:100,,:100,,\(aq   \-\-offsets \(aq0,,:100,,:200,,:300,,:400,,:500,,:600,,:700,,:800,,:900,,\(aq \en\en\en           \- creates VDS (shape [1000,2048,1024]) of ten nexus files (shape [100,2048,1024]) merged in their first dimension\en\en\en\en       nxscollect vds scan_234.nxs://entry/instrument/lambda/data  \-\-shape \(aq100,300,762\(aq \-\-dtype uint32  \-\-target\-fields \(aqlambda_%05d.nxs://entry/data/data:0:2\(aq \-\-shapes \(aq,,250:,,250:,,250\(aq   \-\-offsets \(aq,,:,,256:,,512\(aq  \-\-counts \(aqU,,:U,,:U,,\(aq \-f 1 \en\en\en           \- creates VDS (shape [100,300,762]) of three nexus files (shape [100,300,250]) merged in their third dimension,\en               separated with a 6 pixel gap of 1 values and unlimited first dimension\en\en\en\en       nxscollect vds scan_234.nxs://entry/instrument/percival/data  \-\-shape \(aq4000,1600,2000\(aq \-\-dtype int16  \-\-target\-fields \(aqpercival_%05d.nxs://entry/data/data:1:4\(aq \-\-shapes \(aq1000,,:1000,,:1000,,:1000,,\(aq   \-\-offsets \(aq0,,:1,,:2,,:3,,\(aq  \-\-counts \(aqU,,:U,,:U,,:U,,\(aq \-\-strides \(aq4,,:4,,:4,,:4,,\(aq \en\en\en           \- creates VDS (shape [1000,1600,2000]) of three nexus files (shape [1000,1600,2000])\en                merged in their the first dimension with interlaying frames\en                and unlimited first dimension\en\en\en\en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscollect.VirtualDataset(nexusfilepath, options, writer=None)
+.B class  nxstools.nxscollect.VirtualDataset(nexusfilepath, options, writer=None)
 Bases: \fI\%object\fP
 .sp
 Create virtual dataset in the master NeXus files
 .sp
 The constructor creates the collector object
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBnexusfilepath\fP (\fI\%str\fP) – the nexus file name and nexus path
+\fBnexusfilepath\fP (\fI\%str\fP) \-\- the nexus file name and nexus path
 .IP \(bu 2
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .IP \(bu 2
-\fBwriter\fP (\fI\%str\fP) – the writer module
+\fBwriter\fP (\fI\%str\fP) \-\- the writer module
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates VDS
 .UNINDENT
@@ -2235,15 +8074,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.crdtoint(crd)
 convert coorinate to int or  None or Unlimited
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcrd\fP (\fIcordinate as string\fP) – cordinate as string
+\fBcrd\fP (\fIcordinate as string\fP) \-\- cordinate as string
 .TP
 .B Returns
 converted coordinate
 .TP
 .B Return type
 \fI\%int\fP
 .UNINDENT
@@ -2251,15 +8090,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.filegenerator(filestr, pattern=None)
 provides file name generator from file string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBfilestr\fP – file string
+\fBfilestr\fP \-\- file string
 .TP
 .B Type
 filestr: \fI\%str\fP
 .TP
 .B Returns
 file name generator or a list of file names
 .TP
@@ -2269,24 +8108,24 @@
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.getcompression(compression)
 .INDENT 7.0
 .TP
 .B converts compression string to a deflate level parameter
-or list with [filterid, opt1, opt2, …]
+or list with [filterid, opt1, opt2, ...]
 .UNINDENT
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcompression\fP (\fI\%str\fP) – compression string
+\fBcompression\fP (\fI\%str\fP) \-\- compression string
 .TP
 .B Returns
 deflate level parameter
-or list with [filterid, opt1, opt2, …]
+or list with [filterid, opt1, opt2, ...]
 .TP
 .B Return type
 \fI\%int\fP or \fI\%list\fP < \fI\%int\fP > or \fINone\fP
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
@@ -2296,15 +8135,15 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.splitcoords(crdstr)
 splits coordinate string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcrdstr\fP (\fIcordinate string\fP) – cordinate string
+\fBcrdstr\fP (\fIcordinate string\fP) \-\- cordinate string
 .TP
 .B Returns
 a list ofr coordinates in tuples
 .TP
 .B Return type
 \fI\%list\fP <\fI\%tuple\fP < \fI\%int\fP >>
 .UNINDENT
@@ -2312,103 +8151,103 @@
 .INDENT 0.0
 .TP
 .B nxstools.nxscollect.splitslices(crdstr)
 splits coordinate string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcrdstr\fP (\fIcordinate string\fP) – cordinate string
+\fBcrdstr\fP (\fIcordinate string\fP) \-\- cordinate string
 .TP
 .B Returns
 a list ofr coordinates in tuples
 .TP
 .B Return type
 \fI\%list\fP <\fI\%tuple\fP < \fI\%int\fP >>
 .UNINDENT
 .UNINDENT
 .SS nxstools.nxsconfig module
 .sp
 Command\-line tool for ascess to the nexdatas configuration server
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Components(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Components(parser)
+Bases: \fI\%Runner\fP
 .sp
 Components runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget a list of dependent components\(aq
+.B description  =  \(aqget a list of dependent components\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig components dcm\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig components dcm\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.ConfigServer(device, nonewline=False)
+.B class  nxstools.nxsconfig.ConfigServer(device, nonewline=False)
 Bases: \fI\%object\fP
 .sp
 configuration server adapter
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) – device name of the configuration server
+\fBdevice\fP (\fI\%str\fP) \-\- device name of the configuration server
 .IP \(bu 2
-\fBnonewline\fP (\fI\%bool\fP) – if the output should not be separated
+\fBnonewline\fP (\fI\%bool\fP) \-\- if the output should not be separated
 by the new line character
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B char = None
+.B char
 (\fI\%str\fP) spliting character
 .UNINDENT
 .INDENT 7.0
 .TP
 .B componentsCmd(components)
 lists components of the components
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) – given components
+\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) \-\- given components
 .TP
 .B Returns
 list of component names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
@@ -2416,15 +8255,15 @@
 .INDENT 7.0
 .TP
 .B dataCmd(args)
 provides varaible values
 .INDENT 7.0
 .TP
 .B Parameters
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .TP
 .B Returns
 JSON with variables
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2434,21 +8273,21 @@
 .B deleteCmd(ds, args, ask=True, profiles=False)
 delete the DB items
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) – flag set True for datasources
+\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .IP \(bu 2
-\fBask\fP (\fI\%bool\fP) – ask flag
+\fBask\fP (\fI\%bool\fP) \-\- ask flag
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
 .UNINDENT
 .TP
 .B Returns
 list of XML items
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2459,25 +8298,25 @@
 .B describeCmd(ds, args, md, pr, headers=None, filters=None)
 provides description of configuration elements
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) – flag set True for datasources
+\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .IP \(bu 2
-\fBmd\fP (\fI\%bool\fP) – flag set True for mandatory components
+\fBmd\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
 .IP \(bu 2
-\fBpr\fP (\fI\%str\fP) – flag set True for private components
+\fBpr\fP (\fI\%str\fP) \-\- flag set True for private components
 .IP \(bu 2
-\fBpr\fP – column headers
+\fBpr\fP \-\- column headers
 .IP \(bu 2
-\fBfilters\fP (\fI\%str\fP) – filters for first column names separated by comma
+\fBfilters\fP (\fI\%str\fP) \-\- filters for first column names separated by comma
 .UNINDENT
 .TP
 .B Returns
 list with description
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2488,19 +8327,19 @@
 .B geometryCmd(args, md, pr)
 provides geometry info for given elements
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .IP \(bu 2
-\fBmd\fP (\fI\%bool\fP) – flag set True for mandatory components
+\fBmd\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
 .IP \(bu 2
-\fBpr\fP (\fI\%bool\fP) – flag set True for private components
+\fBpr\fP (\fI\%bool\fP) \-\- flag set True for private components
 .UNINDENT
 .TP
 .B Returns
 list with description
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2509,15 +8348,15 @@
 .INDENT 7.0
 .TP
 .B getCmd(args)
 provides final configuration
 .INDENT 7.0
 .TP
 .B Parameters
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .TP
 .B Returns
 XML configuration string
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2527,23 +8366,23 @@
 .B infoCmd(ds, args, md, pr, profiles)
 Provides info for given elements
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) – flag set True for datasources
+\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .IP \(bu 2
-\fBmd\fP (\fI\%bool\fP) – flag set True for mandatory components
+\fBmd\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
 .IP \(bu 2
-\fBpr\fP (\fI\%bool\fP) – flag set True for private components
+\fBpr\fP (\fI\%bool\fP) \-\- flag set True for private components
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
 .UNINDENT
 .TP
 .B Returns
 list with description
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2554,21 +8393,21 @@
 .B listCmd(ds, mandatory=False, private=False, profiles=False)
 lists the DB item names
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) – flag set True for datasources
+\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
 .IP \(bu 2
-\fBmandatory\fP (\fI\%bool\fP) – flag set True for mandatory components
+\fBmandatory\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
 .IP \(bu 2
-\fBprivate\fP (\fI\%bool\fP) – flag set True for components starting with ‘__’
+\fBprivate\fP (\fI\%bool\fP) \-\- flag set True for components starting with \(aq__\(aq
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
 .UNINDENT
 .TP
 .B Returns
 list op item names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2577,15 +8416,15 @@
 .INDENT 7.0
 .TP
 .B mergeCmd(args)
 provides merged components
 .INDENT 7.0
 .TP
 .B Parameters
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .TP
 .B Returns
 XML configuration string with merged components
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -2595,17 +8434,17 @@
 .B recordCmd(ds, name)
 lists datasources of the component
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) – flag set True for datasources
+\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) – given component or datasource
+\fBname\fP (\fI\%str\fP) \-\- given component or datasource
 .UNINDENT
 .TP
 .B Returns
 list of record names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2616,23 +8455,23 @@
 .B showCmd(ds, args, mandatory=False, profiles=False, directory=None)
 shows the DB items
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) – flag set True for datasources
+\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .IP \(bu 2
-\fBmandatory\fP (\fI\%bool\fP) – flag set True for mandatory components
+\fBmandatory\fP (\fI\%bool\fP) \-\- flag set True for mandatory components
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
 .IP \(bu 2
-\fBdirectory\fP (\fI\%str\fP) – output file directory
+\fBdirectory\fP (\fI\%str\fP) \-\- output file directory
 .UNINDENT
 .TP
 .B Returns
 list of XML items
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2641,15 +8480,15 @@
 .INDENT 7.0
 .TP
 .B sourcesCmd(components, mandatory=False)
 lists datasources of the components
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) – given components
+\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) \-\- given components
 .TP
 .B Returns
 list of datasource names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
@@ -2659,27 +8498,27 @@
 .B uploadCmd(ds, args, force=False, profiles=False, directory=\(aq.\(aq, mandatory=False, external=None)
 upload the DB items from files
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBds\fP (\fI\%bool\fP) – flag set True for datasources
+\fBds\fP (\fI\%bool\fP) \-\- flag set True for datasources
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) – list of item names
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of item names
 .IP \(bu 2
-\fBforce\fP (\fI\%bool\fP) – force flag
+\fBforce\fP (\fI\%bool\fP) \-\- force flag
 .IP \(bu 2
-\fBprofiles\fP (\fI\%bool\fP) – flag set True for profiles
+\fBprofiles\fP (\fI\%bool\fP) \-\- flag set True for profiles
 .IP \(bu 2
-\fBdirectory\fP (\fI\%str\fP) – input file directory
+\fBdirectory\fP (\fI\%str\fP) \-\- input file directory
 .IP \(bu 2
-\fBmandatory\fP (\fI\%bool\fP) – mandatory flag
+\fBmandatory\fP (\fI\%bool\fP) \-\- mandatory flag
 .IP \(bu 2
-\fBexternal\fP (\fI\%str\fP) – external import type
+\fBexternal\fP (\fI\%str\fP) \-\- external import type
 .UNINDENT
 .TP
 .B Returns
 list of XML items
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
@@ -2688,644 +8527,645 @@
 .INDENT 7.0
 .TP
 .B variablesCmd(components, mandatory=False)
 lists variable of the components
 .INDENT 7.0
 .TP
 .B Parameters
-\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) – given components
+\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) \-\- given components
 .TP
 .B Returns
 list of datasource names
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Data(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Data(parser)
+Bases: \fI\%Runner\fP
 .sp
 Data runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget/set values of component variables\(aq
+.B description  =  \(aqget/set values of component variables\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig data \en       nxsconfig data \e\(aq{"sample_name":"H2O"}\e\(aq\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig data \en       nxsconfig data \e\(aq{\(dqsample_name\(dq:\(dqH2O\(dq}\e\(aq\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Delete(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Delete(parser)
+Bases: \fI\%Runner\fP
 .sp
 Show runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqdelete components, datasources or profiles with given names from ConfigServer\(aq
+.B description  =  \(aqdelete components, datasources or profiles with given names from ConfigServer\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig delete pilatus1a\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig delete pilatus1a\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Describe(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Describe(parser)
+Bases: \fI\%Runner\fP
 .sp
 Describe runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqshow all parameters of given components or datasources\(aq
+.B description  =  \(aqshow all parameters of given components or datasources\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig describe pilatus\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig describe pilatus\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Geometry(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Geometry(parser)
+Bases: \fI\%Runner\fP
 .sp
 List runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqshow transformation parameters of given components or datasources\(aq
+.B description  =  \(aqshow transformation parameters of given components or datasources\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig geometry dcm\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig geometry dcm\en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Get(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Get(parser)
+Bases: \fI\%Runner\fP
 .sp
 Get runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget full configuration of components\(aq
+.B description  =  \(aqget full configuration of components\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig get  dcm source slit1 slit2\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig get  dcm source slit1 slit2\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Info(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Info(parser)
+Bases: \fI\%Runner\fP
 .sp
 List runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqshow general parameters of given components, datasources or profile\(aq
+.B description  =  \(aqshow general parameters of given components, datasources or profile\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig info slit1\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig info slit1\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.List(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.List(parser)
+Bases: \fI\%Runner\fP
 .sp
 List runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqlist names of available components, datasources or profiles\(aq
+.B description  =  \(aqlist names of available components, datasources or profiles\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig list\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig list\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Merge(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Merge(parser)
+Bases: \fI\%Runner\fP
 .sp
 Merge runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget merged configuration of components or datasources\(aq
+.B description  =  \(aqget merged configuration of components or datasources\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig merge  slit1 dcm \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig merge  slit1 dcm \en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Record(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Record(parser)
+Bases: \fI\%Runner\fP
 .sp
 Record runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget a list of datasource record names for components or datasources\(aq
+.B description  =  \(aqget a list of datasource record names for components or datasources\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig record \-d exp_mot01 \en       nxsconfig record dcm \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig record \-d exp_mot01 \en       nxsconfig record dcm \en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Servers(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Servers(parser)
+Bases: \fI\%Runner\fP
 .sp
 Servers runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget a list of configuration servers from the current tango host\(aq
+.B description  =  \(aqget a list of configuration servers from the current tango host\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig servers\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig servers\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Show(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Show(parser)
+Bases: \fI\%Runner\fP
 .sp
 Show runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqshow (or write to files) components, datasources or profiles with given names\(aq
+.B description  =  \(aqshow (or write to files) components, datasources or profiles with given names\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig show dcm\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig show dcm\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Sources(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Sources(parser)
+Bases: \fI\%Runner\fP
 .sp
 Sources runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget a list of component datasources\(aq
+.B description  =  \(aqget a list of component datasources\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig sources slit1\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig sources slit1\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Upload(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Upload(parser)
+Bases: \fI\%Runner\fP
 .sp
 Store runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqupload components, datasources or profiles with given names from locale filesystem into ConfigServer\(aq
+.B description  =  \(aqupload components, datasources or profiles with given names from locale filesystem into ConfigServer\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig upload exp_c01 exp_c02\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig upload exp_c01 exp_c02\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsconfig.Variables(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsconfig.Variables(parser)
+Bases: \fI\%Runner\fP
 .sp
 Variables runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget a list of component variables\(aq
+.B description  =  \(aqget a list of component variables\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsconfig variables dcm\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsconfig variables dcm\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -3337,496 +9177,1201 @@
 the main program function
 .UNINDENT
 .SS nxstools.nxscreate module
 .sp
 Command\-line tool for creating NXSConfigServer configuration of Nexus Files
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.ClientDS(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.ClientDS(parser)
+Bases: \fI\%Runner\fP
 .sp
 clientds runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 parser creator
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate client datasources\(aq
+.B description  =  \(aqcreate client datasources\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = "\en * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en            <server> is taken from Tango DB\en\en examples:\en\en       nxscreate clientds starttime \-b  \en\en           \- create the \(aqstarttime\(aq datasource of the \(aqCLIENT\(aq type with the \(aqstarttime\(aq record name\en               and upload them to the NXSConfigServer database \en\en       nxscreate clientds title \-d /home/user/xmldir \en\en           \- create the \(aqtitle\(aq datasource of the \(aqCLIENT\(aq type with the \(aqtitle\(aq record name\en               in the \(aq/home/user/xmldir\(aq directory\en\en       nxscreate clientds \-v exp_c \-f1 \-l4 \-b  \en\en           \- create the \(aqexp_c01\(aq, \(aqexp_c02\(aq, \(aqexp_c03\(aq, \(aqexp_c04\(aq datasources of the \(aqCLIENT\(aq type\en               with the corresponding \(aqexp_c0? record names\en               and upload them to the NXSConfigServer database \en               where \(aq?\(aq is 1, 2, 3, 4 respectively \en\en       nxscreate clientds \-v hasppXX:10000/expchan/vfcadc_exp/ \-f5 \-l8  \-m \-b \-s exp_vfc\en\en           \- create the \(aqexp_vfc05\(aq, \(aqexp_vfc06\(aq, \(aqexp_vfc07\(aq, \(aqexp_vfc08\(aq datasources of the \(aqCLIENT\(aq type\en               with the corresponding \(aqhasppXX:10000/expchan/vfcadc_exp/?\(aq record names\en               and upload them to the NXSConfigServer database \en               where \(aq?\(aq is 5, 6, 7, 8 respectively \en\en"
+.B epilog  =  \(dq\en * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en            <server> is taken from Tango DB\en\en examples:\en\en       nxscreate clientds starttime \-b  \en\en           \- create the \(aqstarttime\(aq datasource of the \(aqCLIENT\(aq type with the \(aqstarttime\(aq record name\en               and upload them to the NXSConfigServer database \en\en       nxscreate clientds title \-d /home/user/xmldir \en\en           \- create the \(aqtitle\(aq datasource of the \(aqCLIENT\(aq type with the \(aqtitle\(aq record name\en               in the \(aq/home/user/xmldir\(aq directory\en\en       nxscreate clientds \-v exp_c \-f1 \-l4 \-b  \en\en           \- create the \(aqexp_c01\(aq, \(aqexp_c02\(aq, \(aqexp_c03\(aq, \(aqexp_c04\(aq datasources of the \(aqCLIENT\(aq type\en               with the corresponding \(aqexp_c0? record names\en               and upload them to the NXSConfigServer database \en               where \(aq?\(aq is 1, 2, 3, 4 respectively \en\en       nxscreate clientds \-v hasppXX:10000/expchan/vfcadc_exp/ \-f5 \-l8  \-m \-b \-s exp_vfc\en\en           \- create the \(aqexp_vfc05\(aq, \(aqexp_vfc06\(aq, \(aqexp_vfc07\(aq, \(aqexp_vfc08\(aq datasources of the \(aqCLIENT\(aq type\en               with the corresponding \(aqhasppXX:10000/expchan/vfcadc_exp/?\(aq record names\en               and upload them to the NXSConfigServer database \en               where \(aq?\(aq is 5, 6, 7, 8 respectively \en\en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.Comp(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.Comp(parser)
+Bases: \fI\%Runner\fP
 .sp
 comp runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate simple components\(aq
+.B description  =  \(aqcreate simple components\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq * with \-b: components are created (without datasources) in Configuration Server database\en * without \-b: components are created (without datasources) on the local filesystem in \-d <directory> \en * default: <directory> is \e\(aq.\e\(aq \en            <server> is taken from Tango DB\en            <strategy> is step\en            <type> is NX_FLOAT\en            <chunk> is SCALAR\en            <nexuspath> is "/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument/collection/"\en\en examples:\en\en       nxscreate comp counter \en\en           \- create the \e\(aqcounter\e\(aq component in the local directory \en               which sets fetching data in the \e\(aqSTEP\e\(aq mode from a \e\(aqcounter\e\(aq datasource to \en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/collection:NXcollection/counter\e\(aq \en\en       nxscreate comp \-f5 \-l7 \-v exp_c \-b \en\en           \- create the \e\(aqexp_c05\e\(aq, \e\(aqexp_c06\e\(aq \e\(aqexp_c07\e\(aq components in the NXSConfigServer database \en               which set fetching data in the \e\(aqSTEP\e\(aq mode from  corresponding \e\(aqexp_c0?\e\(aq datasources to corresponding\en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/collection:NXcollection/exp_c0?\e\(aq\en                where \e\(aq?\e\(aq is 5, 6, 7 respectively \en\en       nxscreate comp lambda \-d /home/user/xmldir/ \en\en           \- create the \e\(aqlambda\e\(aq component in the \e\(aq/home/user/xmldir/\e\(aq directory \en               which sets fetching data in the \e\(aqSTEP\e\(aq mode from a \e\(aqlambda\e\(aq datasource to \en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/collection:NXcollection/lambda\e\(aq \en\en       nxscreate comp \-n "/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument/sis3302:NXdetector/collection:NXcollection/" \-v sis3302_1_roi \-f1 \-l3  \-g FINAL \-t NX_FLOAT64 \-k \-b \-m \en\en           \- create the \e\(aqsis3302_1_roi1\e\(aq, sis3302_1_roi2\e\(aq, sis3302_1_roi3\e\(aq components in the NXSConfigServer database \en               which set fetching data in the \e\(aqFINAL\e\(aq mode from corresponding \e\(aqsis3302_1_roi?\e\(aq datasources to corresponding\en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/sis3302:NXdetector/collection:NXcollection/sis3302_1_roi?\e\(aq\en               float64 fields and creates corresponding\en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/data:NXdata/sis3302_1_roi?\e\(aq links\en               where \e\(aq?\e\(aq is 1, 2, 3 respectively \en\en       nxscreate comp \-n "/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument/eh1_mca01:NXdetector/data" eh1_mca01 \-g STEP \-t NX_FLOAT64 \-i \-b \-c SPECTRUM\en\en           \- create the \e\(aqeh1_mca01\e\(aq component in the NXSConfigServer database \en               which set fetching STECTRUM data in the \e\(aqSTEP\e\(aq mode from a \e\(aqeh1_mca01\e\(aq datasource to \en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/eh1_mca01:NXdetector/data\en               float64 fields and creates \en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/data:NXdata/eh1_mca01\e\(aq links\en\en\en\(aq
+.B epilog  =  \(aq * with \-b: components are created (without datasources) in Configuration Server database\en * without \-b: components are created (without datasources) on the local filesystem in \-d <directory> \en * default: <directory> is \e\(aq.\e\(aq \en            <server> is taken from Tango DB\en            <strategy> is step\en            <type> is NX_FLOAT\en            <chunk> is SCALAR\en            <nexuspath> is \(dq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument/collection/\(dq\en\en examples:\en\en       nxscreate comp counter \en\en           \- create the \e\(aqcounter\e\(aq component in the local directory \en               which sets fetching data in the \e\(aqSTEP\e\(aq mode from a \e\(aqcounter\e\(aq datasource to \en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/collection:NXcollection/counter\e\(aq \en\en       nxscreate comp \-f5 \-l7 \-v exp_c \-b \en\en           \- create the \e\(aqexp_c05\e\(aq, \e\(aqexp_c06\e\(aq \e\(aqexp_c07\e\(aq components in the NXSConfigServer database \en               which set fetching data in the \e\(aqSTEP\e\(aq mode from  corresponding \e\(aqexp_c0?\e\(aq datasources to corresponding\en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/collection:NXcollection/exp_c0?\e\(aq\en                where \e\(aq?\e\(aq is 5, 6, 7 respectively \en\en       nxscreate comp lambda \-d /home/user/xmldir/ \en\en           \- create the \e\(aqlambda\e\(aq component in the \e\(aq/home/user/xmldir/\e\(aq directory \en               which sets fetching data in the \e\(aqSTEP\e\(aq mode from a \e\(aqlambda\e\(aq datasource to \en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/collection:NXcollection/lambda\e\(aq \en\en       nxscreate comp \-n \(dq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument/sis3302:NXdetector/collection:NXcollection/\(dq \-v sis3302_1_roi \-f1 \-l3  \-g FINAL \-t NX_FLOAT64 \-k \-b \-m \en\en           \- create the \e\(aqsis3302_1_roi1\e\(aq, sis3302_1_roi2\e\(aq, sis3302_1_roi3\e\(aq components in the NXSConfigServer database \en               which set fetching data in the \e\(aqFINAL\e\(aq mode from corresponding \e\(aqsis3302_1_roi?\e\(aq datasources to corresponding\en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/sis3302:NXdetector/collection:NXcollection/sis3302_1_roi?\e\(aq\en               float64 fields and creates corresponding\en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/data:NXdata/sis3302_1_roi?\e\(aq links\en               where \e\(aq?\e\(aq is 1, 2, 3 respectively \en\en       nxscreate comp \-n \(dq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument/eh1_mca01:NXdetector/data\(dq eh1_mca01 \-g STEP \-t NX_FLOAT64 \-i \-b \-c SPECTRUM\en\en           \- create the \e\(aqeh1_mca01\e\(aq component in the NXSConfigServer database \en               which set fetching STECTRUM data in the \e\(aqSTEP\e\(aq mode from a \e\(aqeh1_mca01\e\(aq datasource to \en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/instrument:NXinstrument/eh1_mca01:NXdetector/data\en               float64 fields and creates \en               \e\(aq/\e\e$var.entryname#\e\(aqscan\e\(aq\e\e$var.serialno:NXentry/data:NXdata/eh1_mca01\e\(aq links\en\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.Compare(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.Compare(parser)
+Bases: \fI\%Runner\fP
 .sp
 compare runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcompare two online.xml files\(aq
+.B description  =  \(aqcompare two online.xml files\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " * default: second file <online_file> is \(aq/online_dir/online.xml\(aq \en            if only file is given\en\en examples:\en\en       nxscreate compare online.xml \en\en           \- compare \(aqonline.xml\(aq to \(aq/online_dir/online.xml\en\(aq \en       nxscreate compare /online_dir/online_040.xml online.xml \en\en           \- compare \(aq/online_dir/online_040.xml\(aq to \(aqonline.xml\(aq\en"
+.B epilog  =  \(dq * default: second file <online_file> is \(aq/online_dir/online.xml\(aq \en            if only file is given\en\en examples:\en\en       nxscreate compare online.xml \en\en           \- compare \(aqonline.xml\(aq to \(aq/online_dir/online.xml\en\(aq \en       nxscreate compare /online_dir/online_040.xml online.xml \en\en           \- compare \(aq/online_dir/online_040.xml\(aq to \(aqonline.xml\(aq\en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.DeviceDS(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.DeviceDS(parser)
+Bases: \fI\%Runner\fP
 .sp
 deviceds runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate datasources for all device attributes\(aq
+.B description  =  \(aqcreate datasources for all device attributes\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " * without <dv_attr1>: datasources for all attributes are created\en * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en            <server> is taken from Tango DB\en            <datasource> is \(aqexp_mot\(aq \en            <host>, <port> are taken from <server>\en\en examples:\en\en       nxscreate deviceds  \-v p09/pilatus/haso228k \en\en           \- create datasources of the \(aqTANGO\(aq type\en               for all attribute of \(aqp09/pilatus/haso228k\(aq tango device\en               in the local file directory database \en\en       nxscreate deviceds  \-v p09/lambda2m/haso228k \-uhaslambda \-b \en\en           \- create datasources of the \(aqTANGO\(aq type\en               for all attribute of \(aqp09/lambda2m/haso228k\(aq tango device\en               with their hostname \(aqhaslambda\(aq \en               and upload them to the NXSConfigServer database \en\en       nxscreate deviceds  \-v p09/pilatus300k/haso228k \-b \-s pilatus300k_ RoI Energy ExposureTime\en\en           \- create datasources of the \(aqTANGO\(aq type\en               for RoI Energy ExposureTime attribute of \(aqp09/lambda2m/haso228k\(aq tango device\en               with the \(aqpilatus300k_\(aq datasource prefix \en               and upload them to the NXSConfigServer database \en\en"
+.B epilog  =  \(dq * without <dv_attr1>: datasources for all attributes are created\en * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en            <server> is taken from Tango DB\en            <datasource> is \(aqexp_mot\(aq \en            <host>, <port> are taken from <server>\en\en examples:\en\en       nxscreate deviceds  \-v p09/pilatus/haso228k \en\en           \- create datasources of the \(aqTANGO\(aq type\en               for all attribute of \(aqp09/pilatus/haso228k\(aq tango device\en               in the local file directory database \en\en       nxscreate deviceds  \-v p09/lambda2m/haso228k \-uhaslambda \-b \en\en           \- create datasources of the \(aqTANGO\(aq type\en               for all attribute of \(aqp09/lambda2m/haso228k\(aq tango device\en               with their hostname \(aqhaslambda\(aq \en               and upload them to the NXSConfigServer database \en\en       nxscreate deviceds  \-v p09/pilatus300k/haso228k \-b \-s pilatus300k_ RoI Energy ExposureTime\en\en           \- create datasources of the \(aqTANGO\(aq type\en               for RoI Energy ExposureTime attribute of \(aqp09/lambda2m/haso228k\(aq tango device\en               with the \(aqpilatus300k_\(aq datasource prefix \en               and upload them to the NXSConfigServer database \en\en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.OnlineCP(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.OnlineCP(parser)
+Bases: \fI\%Runner\fP
 .sp
 onlinecp runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate component from online.xml file\(aq
+.B description  =  \(aqcreate component from online.xml file\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " * without \(aq\-c <component>\(aq: show a list of possible components\en * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en * default: <inputFile> is \(aq/online_dir/online.xml\(aq \en            <server> is taken from Tango DB\en\en examples:\en\en       nxscreate onlinecp  \en\en           \- list possible components which can be created from online.xml \en\en       nxscreate onlinecp \-c pilatus \-b \en\en           \- create the \(aqpilatus\(aq component and its datasources\en               in the NXSConfigServer database\en\en       nxscreate onlinecp \-c lambda \-d /home/user/xmldir/ \en\en           \- create the \(aqlambda\(aq component and its datasources\en               in the \(aq/home/user/xmldir/\(aq directory\en\en       nxscreate onlinecp \-c lmbd \-t lambda \-b \en\en           \- create the \(aqlmbd\(aq component of \(aqlambda\(aq type and its datasources\en               in the NXSConfigServer database\en\en\en       nxscreate onlinecp \-c lmbd \-t lambda  \-v p00/lmbd/1 \-u haso000 \-w 10000 \-b \en\en           \- create the \(aqlmbd\(aq component of \(aqlambda\(aq type and its datasources without online.xml\en               in the NXSConfigServer database\en\en"
+.B epilog  =  \(dq * without \(aq\-c <component>\(aq: show a list of possible components\en * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en * default: <inputFile> is \(aq/online_dir/online.xml\(aq \en            <server> is taken from Tango DB\en\en examples:\en\en       nxscreate onlinecp  \en\en           \- list possible components which can be created from online.xml \en\en       nxscreate onlinecp \-c pilatus \-b \en\en           \- create the \(aqpilatus\(aq component and its datasources\en               in the NXSConfigServer database\en\en       nxscreate onlinecp \-c lambda \-d /home/user/xmldir/ \en\en           \- create the \(aqlambda\(aq component and its datasources\en               in the \(aq/home/user/xmldir/\(aq directory\en\en       nxscreate onlinecp \-c lmbd \-t lambda \-b \en\en           \- create the \(aqlmbd\(aq component of \(aqlambda\(aq type and its datasources\en               in the NXSConfigServer database\en\en\en       nxscreate onlinecp \-c lmbd \-t lambda  \-v p00/lmbd/1 \-u haso000 \-w 10000 \-b \en\en           \- create the \(aqlmbd\(aq component of \(aqlambda\(aq type and its datasources without online.xml\en               in the NXSConfigServer database\en\en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.OnlineDS(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.OnlineDS(parser)
+Bases: \fI\%Runner\fP
 .sp
 onlineds runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate datasources from online.xml file\(aq
+.B description  =  \(aqcreate datasources from online.xml file\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " * with \-b: datasources are created in Configuration Server database\en * with \-d <directory>: datasources are created on the local filesystem\en * without \-b or \-d <directory>: run in the test mode\en * default: <inputFile> is \(aq/online_dir/online.xml\(aq \en            <server> is taken from Tango DB\en\en \(gaonlineds\(ga overwrites existing datasources\en\en examples:\en\en       nxscreate onlineds \-b  \en\en           \- create datasources from online.xml file \en               and upload them to the NXSConfigServer database \en\en       nxscreate onlineds \-b \-t \en\en           \- like above but set motor tango datasources to \en               be no __CLIENT__ like\en\en       nxscreate onlineds \-d /home/user/xmldir \en\en           \- create datasources from online.xml file \en               and save them in the \(aq/home/user/xmldir\(aq directory \en\en       nxscreate onlineds \en\en           \- run the command in test mode without creating datasources \en"
+.B epilog  =  \(dq * with \-b: datasources are created in Configuration Server database\en * with \-d <directory>: datasources are created on the local filesystem\en * without \-b or \-d <directory>: run in the test mode\en * default: <inputFile> is \(aq/online_dir/online.xml\(aq \en            <server> is taken from Tango DB\en\en \(gaonlineds\(ga overwrites existing datasources\en\en examples:\en\en       nxscreate onlineds \-b  \en\en           \- create datasources from online.xml file \en               and upload them to the NXSConfigServer database \en\en       nxscreate onlineds \-b \-t \en\en           \- like above but set motor tango datasources to \en               be no __CLIENT__ like\en\en       nxscreate onlineds \-d /home/user/xmldir \en\en           \- create datasources from online.xml file \en               and save them in the \(aq/home/user/xmldir\(aq directory \en\en       nxscreate onlineds \en\en           \- run the command in test mode without creating datasources \en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxstools.nxscreate.PYTANGO = True
+.B nxstools.nxscreate.PYTANGO  =  True
 (\fI\%bool\fP) True if PyTango available
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.PoolDS(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.PoolDS(parser)
+Bases: \fI\%Runner\fP
 .sp
 poolds runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate datasources from sardana pool device\(aq
+.B description  =  \(aqcreate datasources from sardana pool device\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " * with \-b: datasources are created in Configuration Server database\en * with \-d <directory>: datasources are created on the local filesystem\en * without \-b or \-d <directory>: run in the test mode\en * default: <channel> is \(aqALL\(aq \en            <server> is taken from Tango DB\en\en            <pool> is taken from Tango DB\en\en \(gapoolds\(ga overwrites existing datasources\en\en examples:\en\en       nxscreate poolds \-b  \en\en           \- create all datasources defined in the local Pool \en               and upload them to the NXSConfigServer database \en\en       nxscreate poolds \-b \-t \en\en           \- like above but set motor tango datasources to \en               be no __CLIENT__ like\en\en       nxscreate poolds \-d . \-p p09/pool/haso228 \en\en           \- create all datasources defined in the \(aqp09/pool/haso228\(aq Pool \en               and save them in the local directory \en\en       nxscreate poolds \-b Motor CTExpChannel \en\en           \- create datasources of \(aqMotor\(aq and CTExpChannel classes \en               defined in the local Pool \en               and upload them to the NXSConfigServer database \en\en       nxscreate poolds \-b mot01 mot03 \en\en           \- create \(aqmot01\(aq and \(aqmot03\(aq datasources\en               defined in the local Pool \en               and upload them to the NXSConfigServer database \en\en       nxscreate poolds \en\en           \- run the command in test mode without creating datasources \en"
+.B epilog  =  \(dq * with \-b: datasources are created in Configuration Server database\en * with \-d <directory>: datasources are created on the local filesystem\en * without \-b or \-d <directory>: run in the test mode\en * default: <channel> is \(aqALL\(aq \en            <server> is taken from Tango DB\en\en            <pool> is taken from Tango DB\en\en \(gapoolds\(ga overwrites existing datasources\en\en examples:\en\en       nxscreate poolds \-b  \en\en           \- create all datasources defined in the local Pool \en               and upload them to the NXSConfigServer database \en\en       nxscreate poolds \-b \-t \en\en           \- like above but set motor tango datasources to \en               be no __CLIENT__ like\en\en       nxscreate poolds \-d . \-p p09/pool/haso228 \en\en           \- create all datasources defined in the \(aqp09/pool/haso228\(aq Pool \en               and save them in the local directory \en\en       nxscreate poolds \-b Motor CTExpChannel \en\en           \- create datasources of \(aqMotor\(aq and CTExpChannel classes \en               defined in the local Pool \en               and upload them to the NXSConfigServer database \en\en       nxscreate poolds \-b mot01 mot03 \en\en           \- create \(aqmot01\(aq and \(aqmot03\(aq datasources\en               defined in the local Pool \en               and upload them to the NXSConfigServer database \en\en       nxscreate poolds \en\en           \- run the command in test mode without creating datasources \en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.StdComp(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.SECoPCP(parser)
+Bases: \fI\%Runner\fP
+.sp
+secop component runner
+.sp
+parser creator
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates parser
+.UNINDENT
+.INDENT 7.0
+.TP
+.B description  =  \(aqcreate secop components\(aq
+(\fI\%str\fP) command description
+.UNINDENT
+.INDENT 7.0
+.TP
+.B epilog  =  \(dq * with \-b: components are created (without datasources) in Configuration Server database\en * without \-b: components are created (without datasources) on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en            <port> is 5001\en\en examples:\en\en       nxscreate secopcp \en       nxscreate secopcp \-l \en\en           \- list all modules of the given node \en\en       nxscreate secopcp \-c temp_node \-d . \-j secopn_node.json \en\en           \- create the all secop components in the local directory for the node configured with the json file \en\en       nxscreate secopcp T \-t 5001 \-b \en\en           \- create the component for the T secop module  in the NXSConfigServer database for the node on the port 5000 \en\en       nxscreate secopcp \-d /home/user/xmldir/ \en\en           \- create the all secop components in the given directory\en\en\(dq
+(\fI\%str\fP) command epilog
+.UNINDENT
+.INDENT 7.0
+.TP
+.B run(options)
+the main program function
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreate.StdComp(parser)
+Bases: \fI\%Runner\fP
 .sp
 stdcomp runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate component from the standard templates\(aq
+.B description  =  \(aqcreate component from the standard templates\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " * without \(aq\-t <type>\(aq: show a list of possible component types\en * with \(aq\-t <type>  and without \-c <component>: show a list of component variables for the given component type\en * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en * [name1 value1 [name2 value2] ...] sequence  defines component variable values \en\en examples:\en\en       nxscreate stdcomp  \en\en           \- list possible component types\en               from the \(aqnxstools.xmltemplates\(aq package\en\en       nxscreate stdcomp  \-p nxsextrasp00  \en\en           \- list possible component types from the \(aqnxsextrasp00\(aq package\en\en       nxscreate stdcomp  \-t source \en\en           \- list a description of \(aqsource\(aq component variables\en\en       nxscreate stdcomp  \-t default  \-c default  \-m  \-b\en\en           \- create \(aqdefault\(aq component  of the \(aqdefault\(aq type\en               in the NXSConfigServer database and set it as mandatory\en\en       nxscreate stdcomp  \-t slit  \-c front_slit1   xgap slt1x  ygap slt1y\en\en           \- create \(aqfront_slit1\(aq component  of the \(aqslit\(aq type\en               where variables xgap=\(aqslt1x\(aq and ygap=\(aqslt1and\(aq in the local directory \en\en       nxscreate stdcomp  \-p nxsextrasp08  \-t analyzer  \-c analyzer1  v anav  roll anaroll  \-b\en\en           \- create \(aqanalyzer1\(aq component of the \(aqanalyzer type\(aq\en               where variables v=\(aqanav\(aq and roll=\(aqamaroll\(aq in the NXSConfigServer database\en"
+.B epilog  =  \(dq * without \(aq\-t <type>\(aq: show a list of possible component types\en * with \(aq\-t <type>  and without \-c <component>: show a list of component variables for the given component type\en * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en * [name1 value1 [name2 value2] ...] sequence  defines component variable values \en\en examples:\en\en       nxscreate stdcomp  \en\en           \- list possible component types\en               from the \(aqnxstools.xmltemplates\(aq package\en\en       nxscreate stdcomp  \-p nxsextrasp00  \en\en           \- list possible component types from the \(aqnxsextrasp00\(aq package\en\en       nxscreate stdcomp  \-t source \en\en           \- list a description of \(aqsource\(aq component variables\en\en       nxscreate stdcomp  \-t default  \-c default  \-m  \-b\en\en           \- create \(aqdefault\(aq component  of the \(aqdefault\(aq type\en               in the NXSConfigServer database and set it as mandatory\en\en       nxscreate stdcomp  \-t slit  \-c front_slit1   xgap slt1x  ygap slt1y\en\en           \- create \(aqfront_slit1\(aq component  of the \(aqslit\(aq type\en               where variables xgap=\(aqslt1x\(aq and ygap=\(aqslt1and\(aq in the local directory \en\en       nxscreate stdcomp  \-p nxsextrasp08  \-t analyzer  \-c analyzer1  v anav  roll anaroll  \-b\en\en           \- create \(aqanalyzer1\(aq component of the \(aqanalyzer type\(aq\en               where variables v=\(aqanav\(aq and roll=\(aqamaroll\(aq in the NXSConfigServer database\en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreate.TangoDS(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxscreate.TangoDS(parser)
+Bases: \fI\%Runner\fP
 .sp
 tangods runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate tango datasources\(aq
+.B description  =  \(aqcreate tango datasources\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = " * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en            <server> is taken from Tango DB\en            <datasource> is \(aqexp_mot\(aq \en            <host>, <port> are taken from <server>\en\en examples:\en\en       nxscreate tangods \-f1 \-l2 \-v p09/motor/exp. \-s exp_mot \en\en           \- create the \(aqexp_mot01\(aq and \(aqexp_mot02\(aq datasources of the \(aqTANGO\(aq type\en               with the corresponding \(aqp09/motor/exp.0?\(aq device names\en               and \(aqPosition\(aq tango attribute names in the local directory\en               where \(aq?\(aq is 1, 2 respectively \en\en       nxscreate tangods \-f1 \-l32 \-v p02/motor/eh1a. \-s exp_mot \-b \en\en           \- create the \(aqexp_mot01\(aq, ... ,\(aqexp_mot32\(aq datasources of the \(aqTANGO\(aq type\en               with the corresponding \(aqp09/motor/eh1a.??\(aq device names\en               while their attribute name is \(aqPosition\(aq  and upload them to the NXSConfigServer database\en               where \(aq??\(aq is 01, 02, ... ,32 respectively \en\en       nxscreate tangods \-v petra/globals/keyword \-s source_current \-u haso228 \-t 10000 \e\e \en                         \-a BeamCurrent \-b \-r p09/nxsconfigserver/haso228 \-o \-g __CLIENT__\en\en           \- create the a \(aqsource_current\(aq datasource of the \(aqTANGO\(aq type belonging to the \(aq__CLIENT__\(aq group \en               with the \(aqpetra/globals/keyword\(aq device name\en               while their attribute name is \(aqBeamCurrent\(aq, \en               their hostname is \(aqhaso228\(aq, their tango port is \(aq10000\(aq\en               and upload them to the NXSConfigServer \(aqp09/nxsconfigserver/haso228\(aq database\en\en       nxscreate tangods \-f1 \-l8  \-v pXX/slt/exp. \-s slt_exp_ \-u hasppXX.desy.de \-b \en\en           \- create the \(aqslt_exp_01\(aq, ... ,\(aqslt_exp_08\(aq datasources of the \(aqTANGO\(aq type\en               with the corresponding \(aqpXX/slt/exp.0?\(aq device names\en               while their attribute name is \(aqPosition\(aq, \en               their hostname is \(aqhasppXX.desy.de\(aq  and upload them to the NXSConfigServer database\en               where \(aq??\(aq is 1, 2, ... ,8 respectively \en\en"
+.B epilog  =  \(dq * with \-b: datasources are created in Configuration Server database\en * without \-b: datasources are created on the local filesystem in \-d <directory> \en * default: <directory> is \(aq.\(aq \en            <server> is taken from Tango DB\en            <datasource> is \(aqexp_mot\(aq \en            <host>, <port> are taken from <server>\en\en examples:\en\en       nxscreate tangods \-f1 \-l2 \-v p09/motor/exp. \-s exp_mot \en\en           \- create the \(aqexp_mot01\(aq and \(aqexp_mot02\(aq datasources of the \(aqTANGO\(aq type\en               with the corresponding \(aqp09/motor/exp.0?\(aq device names\en               and \(aqPosition\(aq tango attribute names in the local directory\en               where \(aq?\(aq is 1, 2 respectively \en\en       nxscreate tangods \-f1 \-l32 \-v p02/motor/eh1a. \-s exp_mot \-b \en\en           \- create the \(aqexp_mot01\(aq, ... ,\(aqexp_mot32\(aq datasources of the \(aqTANGO\(aq type\en               with the corresponding \(aqp09/motor/eh1a.??\(aq device names\en               while their attribute name is \(aqPosition\(aq  and upload them to the NXSConfigServer database\en               where \(aq??\(aq is 01, 02, ... ,32 respectively \en\en       nxscreate tangods \-v petra/globals/keyword \-s source_current \-u haso228 \-t 10000 \e\e \en                         \-a BeamCurrent \-b \-r p09/nxsconfigserver/haso228 \-o \-g __CLIENT__\en\en           \- create the a \(aqsource_current\(aq datasource of the \(aqTANGO\(aq type belonging to the \(aq__CLIENT__\(aq group \en               with the \(aqpetra/globals/keyword\(aq device name\en               while their attribute name is \(aqBeamCurrent\(aq, \en               their hostname is \(aqhaso228\(aq, their tango port is \(aq10000\(aq\en               and upload them to the NXSConfigServer \(aqp09/nxsconfigserver/haso228\(aq database\en\en       nxscreate tangods \-f1 \-l8  \-v pXX/slt/exp. \-s slt_exp_ \-u hasppXX.desy.de \-b \en\en           \- create the \(aqslt_exp_01\(aq, ... ,\(aqslt_exp_08\(aq datasources of the \(aqTANGO\(aq type\en               with the corresponding \(aqpXX/slt/exp.0?\(aq device names\en               while their attribute name is \(aqPosition\(aq, \en               their hostname is \(aqhasppXX.desy.de\(aq  and upload them to the NXSConfigServer database\en               where \(aq??\(aq is 1, 2, ... ,8 respectively \en\en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxscreate.main()
 the main program function
 .UNINDENT
+.SS nxstools.nxscreator module
+.sp
+Command\-line tool for creating to the nexdatas configuration server
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.CPCreator(options, args, printouts=True)
+Bases: \fI\%Creator\fP
+.sp
+component creator of all online.xml complex devices
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B components
+(\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) component xml dictionary
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates components of all online.xml complex devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createXMLs()
+creates component xmls of all online.xml complex devices
+abstract method
+.UNINDENT
+.INDENT 7.0
+.TP
+.B datasources
+(\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) datasource xml dictionary
+.UNINDENT
+.INDENT 7.0
+.TP
+.B xmlpackage
+(\fI\%str\fP) xml template component package
+.UNINDENT
+.INDENT 7.0
+.TP
+.B xmltemplatepath
+(\fI\%str\fP) xml template component package path
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B exception  nxstools.nxscreator.CPExistsException
+Bases: \fI\%Exception\fP
+.sp
+Component already exists exception
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.ClientDSCreator(options, args, printouts=True)
+Bases: \fI\%Creator\fP
+.sp
+client datasource creator
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates a client datasource xml and stores it in DB or filesytem
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.CompareOnlineDS(options, args, printouts=True)
+Bases: \fI\%object\fP
+.sp
+comparing tool for online.xml files
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B args
+(\fI\%list\fP < \fI\%str\fP >) creator arguments
+.UNINDENT
+.INDENT 7.0
+.TP
+.B compare()
+.UNINDENT
+.INDENT 7.0
+.TP
+.B options
+(\fBoptparse.Values\fP) creator options
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.ComponentCreator(options, args, printouts=True)
+Bases: \fI\%Creator\fP
+.sp
+component creator
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates a component xml and stores it in DB or filesytem
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.Creator(options, args, printouts=True)
+Bases: \fI\%object\fP
+.sp
+configuration server adapter
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B args
+(\fI\%list\fP < \fI\%str\fP >) creator arguments
+.UNINDENT
+.INDENT 7.0
+.TP
+.B options
+(\fBoptparse.Values\fP) creator options
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B exception  nxstools.nxscreator.DSExistsException
+Bases: \fI\%Exception\fP
+.sp
+DataSource already exists exception
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.Device
+Bases: \fI\%object\fP
+.sp
+device from online.xml
+.INDENT 7.0
+.TP
+.B attribute
+(\fI\%str\fP) attribute name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B compare(dv)
+.UNINDENT
+.INDENT 7.0
+.TP
+.B dtype
+(\fI\%str\fP) device type
+.UNINDENT
+.INDENT 7.0
+.TP
+.B findAttribute(tangohost, clientlike=False)
+sets attribute and datasource group of online.xml device
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBtangohost\fP (\fI\%str\fP) \-\- tango host
+.IP \(bu 2
+\fBclientlike\fP (\fI\%bool\fP) \-\- tango motors to be client like
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B findDevice(tangohost)
+sets sardana device name and sardana host/port of online.xml device
+.INDENT 7.0
+.TP
+.B Parameters
+\fBtangohost\fP (\fI\%str\fP) \-\- tango host
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B group
+(\fI\%str\fP) datasource tango group
+.UNINDENT
+.INDENT 7.0
+.TP
+.B host
+(\fI\%str\fP) host without port
+.UNINDENT
+.INDENT 7.0
+.TP
+.B hostname
+(\fI\%str\fP) host name with port
+.UNINDENT
+.INDENT 7.0
+.TP
+.B module
+(\fI\%str\fP) device module
+.UNINDENT
+.INDENT 7.0
+.TP
+.B name
+(\fI\%str\fP) device name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B port
+(\fI\%str\fP) port
+.UNINDENT
+.INDENT 7.0
+.TP
+.B sardanahostname
+(\fI\%str\fP) sardana host name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B sardananame
+(\fI\%str\fP) sardana name with port
+.UNINDENT
+.INDENT 7.0
+.TP
+.B sdevice
+(\fI\%str\fP) sardana device name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B setSardanaName(tolower)
+sets sardana name
+.INDENT 7.0
+.TP
+.B Parameters
+\fBtolower\fP (\fI\%bool\fP) \-\- If True name in lowercase
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B shost
+(\fI\%str\fP) sardana host without port
+.UNINDENT
+.INDENT 7.0
+.TP
+.B splitHostPort()
+spilts host name from port
+.UNINDENT
+.INDENT 7.0
+.TP
+.B sport
+(\fI\%str\fP) sardana tango port
+.UNINDENT
+.INDENT 7.0
+.TP
+.B tdevice
+(\fI\%str\fP) tango device name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B thost
+(\fI\%str\fP) tango host without port
+.UNINDENT
+.INDENT 7.0
+.TP
+.B tolower()
+converts \fIname\fP, \fImodule\fP, \fItdevice\fP, \fIhostname\fP into lower case
+.UNINDENT
+.INDENT 7.0
+.TP
+.B tport
+(\fI\%str\fP) tango port
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.DeviceDSCreator(options, args, printouts=True)
+Bases: \fI\%Creator\fP
+.sp
+device datasource creator
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates a tango datasources xml of given device
+and stores it in DB or filesytem
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.OnlineCPCreator(options, args, printouts=True)
+Bases: \fI\%CPCreator\fP
+.sp
+component creator of online components
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createXMLs()
+creates component xmls of all online.xml complex devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B listcomponents()
+provides a list of components with xml templates
+.INDENT 7.0
+.TP
+.B Returns
+list of components with xml templates
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP >
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B listcomponenttypes()
+provides a list of standard component types
+.INDENT 7.0
+.TP
+.B Returns
+list of standard component types
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.OnlineDSCreator(options, args, printouts=True)
+Bases: \fI\%Creator\fP
+.sp
+datasource creator of all online.xml simple devices
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates datasources of all online.xml simple devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createXMLs()
+creates datasource xmls of all online.xml simple devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B datasources
+(\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) datasource xml dictionary
+.UNINDENT
+.INDENT 7.0
+.TP
+.B xmlpackage
+(\fI\%str\fP) xml template component package
+.UNINDENT
+.INDENT 7.0
+.TP
+.B xmltemplatepath
+(\fI\%str\fP) xml template component package path
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxscreator.PYTANGO  =  True
+(\fI\%bool\fP) True if PyTango available
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.PoolDSCreator(options, args, printouts=True)
+Bases: \fI\%Creator\fP
+.sp
+datasource creator of all sardana pool acquisition channels
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates datasources of all online.xml simple devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createXMLs()
+creates datasource xmls of all online.xml simple devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B datasources
+(\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) datasource xml dictionary
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.SECoPCPCreator(options, args, printouts=True)
+Bases: \fI\%CPCreator\fP
+.sp
+component creator of secop components
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates components of all online.xml complex devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createSECoPDS(dsname, message, group=None, access=None, host=None, port=None, timeout=None)
+create SECoP datasource
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBdsname\fP (\fI\%str\fP) \-\- datasource name
+.IP \(bu 2
+\fBmessage\fP (\fI\%str\fP) \-\- secop command
+.IP \(bu 2
+\fBgroup\fP (\fI\%str\fP) \-\- secop group name
+.IP \(bu 2
+\fBaccess\fP (\fI\%str\fP) \-\- secop attribute access list
+.IP \(bu 2
+\fBhost\fP (\fI\%str\fP) \-\- secop host name
+.IP \(bu 2
+\fBport\fP (\fI\%str\fP or \fI\%float\fP) \-\- secop port name
+.IP \(bu 2
+\fBport\fP \-\- minimum timeout
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createSECoPLinkDS(entryname, samplename, sampleenvname, meanings, environments)
+create SECoP datasource
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBentryname\fP (\fI\%str\fP) \-\- secop entry name
+.IP \(bu 2
+\fBsamplename\fP (\fI\%str\fP) \-\- secop sample name
+.IP \(bu 2
+\fBsampleenvname\fP (\fI\%str\fP) \-\- secop sample name
+.IP \(bu 2
+\fBmeanings\fP (\fI\%str\fP) \-\- secop meanings list
+.IP \(bu 2
+\fBenvironments\fP (\fI\%str\fP) \-\- secop environments list
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createXMLs()
+creates component xmls of all online.xml complex devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B listmodules()
+provides a list of modules for the secop node
+.INDENT 7.0
+.TP
+.B Returns
+list of modules for the secop node
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP >
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.StandardCPCreator(options, args, printouts=True)
+Bases: \fI\%CPCreator\fP
+.sp
+component creator of standard templates
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createXMLs()
+creates component xmls of all online.xml complex devices
+.UNINDENT
+.INDENT 7.0
+.TP
+.B listcomponenttypes()
+provides a list of standard component types
+.INDENT 7.0
+.TP
+.B Returns
+list of standard component types
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B listcomponentvariables()
+provides a list of standard component types
+.INDENT 7.0
+.TP
+.B Returns
+list of standard component types
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxscreator.TangoDSCreator(options, args, printouts=True)
+Bases: \fI\%Creator\fP
+.sp
+tango datasource creator
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBoptions\fP (\fBoptparse.Values\fP) \-\- command options
+.IP \(bu 2
+\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) \-\- command arguments
+.IP \(bu 2
+\fBprintouts\fP (\fI\%bool\fP) \-\- if printout is enable
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates a tango datasource xml and stores it in DB or filesytem
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B exception  nxstools.nxscreator.WrongParameterError
+Bases: \fI\%Exception\fP
+.sp
+wrong parameter exception
+.UNINDENT
 .SS nxstools.nxsdata module
 .sp
 Command\-line tool to ascess to Tango Data Server
 .INDENT 0.0
 .TP
-.B class nxstools.nxsdata.CloseEntry(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsdata.CloseEntry(parser)
+Bases: \fI\%Runner\fP
 .sp
 CloseEntry runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqclose the current entry\(aq
+.B description  =  \(aqclose the current entry\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsdata closeentry \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsdata closeentry \en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsdata.CloseFile(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsdata.CloseFile(parser)
+Bases: \fI\%Runner\fP
 .sp
 CloseFile runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqclose the current file\(aq
+.B description  =  \(aqclose the current file\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsdata closefile \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsdata closefile \en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsdata.NexusServer(device)
+.B class  nxstools.nxsdata.NexusServer(device)
 Bases: \fI\%object\fP
 .sp
 configuration server adapter
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdevice\fP (\fI\%str\fP) – device name of configuration server
+\fBdevice\fP (\fI\%str\fP) \-\- device name of configuration server
 .UNINDENT
 .INDENT 7.0
 .TP
 .B closeEntry()
 closes the entry
 .UNINDENT
 .INDENT 7.0
@@ -3837,510 +10382,822 @@
 .INDENT 7.0
 .TP
 .B openEntry(xmlconfig)
 opens an entry
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlconfig\fP (\fI\%str\fP) – xml configuration string
+\fBxmlconfig\fP (\fI\%str\fP) \-\- xml configuration string
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B openFile(filename)
 opens the h5 file
 .INDENT 7.0
 .TP
 .B Parameters
-\fBfilename\fP (\fI\%str\fP) – h5 file name
+\fBfilename\fP (\fI\%str\fP) \-\- h5 file name
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B record(jsondata)
 records one step
 .INDENT 7.0
 .TP
 .B Parameters
-\fBjsondata\fP (\fI\%str\fP) – step JSON data
+\fBjsondata\fP (\fI\%str\fP) \-\- step JSON data
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setData(jsondata)
 sets the global JSON data
 .INDENT 7.0
 .TP
 .B Parameters
-\fBjsondata\fP (\fI\%str\fP) – global JSON data
+\fBjsondata\fP (\fI\%str\fP) \-\- global JSON data
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B tdwServer = None
+.B tdwServer
 (\fBPyTango.DeviceProxy\fP) NeXus writer device proxy
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsdata.OpenEntry(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsdata.OpenEntry(parser)
+Bases: \fI\%Runner\fP
 .sp
 OpenEntry runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqcreate new entry\(aq
+.B description  =  \(aqcreate new entry\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsdata openentry ... \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsdata openentry ... \en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsdata.OpenFile(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsdata.OpenFile(parser)
+Bases: \fI\%Runner\fP
 .sp
 OpenFile runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqopen a new H5 file\(aq
+.B description  =  \(aqopen a new H5 file\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsdata openfile /tmp/watertest.nxs \en       nxsdata openfile \-s p02/tangodataserver/exp.01  /user/data/myfile.h5\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsdata openfile /tmp/watertest.nxs \en       nxsdata openfile \-s p02/tangodataserver/exp.01  /user/data/myfile.h5\en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 parser creator after autocomplete run
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsdata.Record(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsdata.Record(parser)
+Bases: \fI\%Runner\fP
 .sp
 Record runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqrecord one step with step JSON data\(aq
+.B description  =  \(aqrecord one step with step JSON data\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsdata record ... \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsdata record ... \en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsdata.Servers(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsdata.Servers(parser)
+Bases: \fI\%Runner\fP
 .sp
 Servers runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqget lists of tango data servers from the current tango host\(aq
+.B description  =  \(aqget lists of tango data servers from the current tango host\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsdata servers \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsdata servers \en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsdata.SetData(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsdata.SetData(parser)
+Bases: \fI\%Runner\fP
 .sp
 SetData runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqassign global JSON data\(aq
+.B description  =  \(aqassign global JSON data\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsdata setdata ... \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsdata setdata ... \en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsdata.main()
 the main program function
 .UNINDENT
+.SS nxstools.nxsdevicetools module
+.sp
+NDTS TANGO device tools
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.PYTANGO  =  True
+(\fI\%bool\fP) True if tango available
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxsdevicetools.PackageHandler(packagename=\(aqnxstools.xmltemplates\(aq)
+Bases: \fI\%object\fP
+.sp
+xml templates package loader
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBpackagename\fP (\fI\%str\fP) \-\- full package name
+.UNINDENT
+.INDENT 7.0
+.TP
+.B loadXMLTemplates(packagename)
+load xml template module variables
+.INDENT 7.0
+.TP
+.B Parameters
+\fBpackagename\fP (\fI\%str\fP) \-\- full package name
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.checkServer(name=\(aqNXSConfigServer\(aq)
+provides server device name if only one or error in the other case
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- server name
+.TP
+.B Returns
+server device name or empty string if error appears
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.ctModules  =  [\(aqmca8715roi\(aq, \(aqonedroi\(aq, \(aqsis3820\(aq, \(aqsis3302roi\(aq, \(aqxmcd\(aq, \(aqvfcadc\(aq, \(aqmythenroi\(aq, \(aqmhzdaqp01\(aq, \(aqdgg2\(aq, \(aqtangoattributectctrl\(aq]
+(\fI\%list\fP <\fI\%str\fP>) counter/timer modules
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.findClassName(server, name)
+finds class name
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- device name
+.TP
+.B Returns
+class name
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.generateDeviceNames(prefix, first, last, minimal=False)
+generates device names
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBprefix\fP (\fI\%str\fP) \-\- device name prefix
+.IP \(bu 2
+\fBfirst\fP (\fI\%int\fP) \-\- first device index
+.IP \(bu 2
+\fBlast\fP (\fI\%int\fP) \-\- last device index
+.UNINDENT
+.TP
+.B Returns
+device names
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.getAttributes(device, host=None, port=10000)
+provides a list of device attributes
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBdevice\fP (\fI\%str\fP) \-\- tango device name
+.IP \(bu 2
+\fBhost\fP (\fI\%str\fP) \-\- device host
+.IP \(bu 2
+\fBport\fP (\fI\%int\fP) \-\- device port
+.UNINDENT
+.TP
+.B Returns
+list of device attributes
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.getClassName(devicename)
+provides device class name
+.INDENT 7.0
+.TP
+.B Parameters
+\fBdevicename\fP (\fI\%str\fP) \-\- device name
+.TP
+.B Returns
+class name
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.getDataSourceComponents(server, verbose=False)
+gets datasource components
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBserver\fP (\fI\%str\fP) \-\- configuration server
+.IP \(bu 2
+\fBverbose\fP (\fI\%bool\fP) \-\- additional printouts
+.UNINDENT
+.TP
+.B Returns
+dictionary with datasource components
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fI\%list\fP <\fI\%str\fP>>
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.getServerTangoHost(server)
+fetches the server tango_host:tango_port
+.INDENT 7.0
+.TP
+.B Parameters
+\fBserver\fP (\fI\%str\fP) \-\- tango server
+.TP
+.B Returns
+tango host
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.getServers(name=\(aqNXSConfigServer\(aq)
+provides server device names
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- server instance name
+.TP
+.B Returns
+list of the server device names
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.ioRegModules  =  [\(aqsis3610\(aq]
+(\fI\%list\fP <\fI\%str\fP>) IO register modules
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.listServers(server, name=\(aqNXSConfigServer\(aq)
+finds server names
+.INDENT 7.0
+.TP
+.B Parameters
+\fBname\fP (\fI\%str\fP) \-\- server instance name
+.TP
+.B Returns
+server list
+.TP
+.B Return type
+\fI\%list\fP <\fI\%str\fP>
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.moduleMultiAttributes  =  {\(aqcobold\(aq: [\(aqBinSize\(aq, \(aqExposureTime\(aq], \(aqdalsa\(aq: [\(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqTriggerMode\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqExtendedExposure\(aq, \(aqBinComment\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqFramesReceived\(aq, \(aqFrameRate\(aq, \(aqFramesPerNXFile\(aq, \(aqNXFileCompression\(aq, \(aqTurboMode\(aq, \(aqImageEnc\(aq, \(aqViewingMode\(aq, \(aqThrashedBuffers\(aq, \(aqFramesToAcquire\(aq, \(aqAcquisitionFrameCount\(aq, \(aqAcquisitionMode\(aq, \(aqAcquisitionFrameMode\(aq, \(aqLinearityEqualizer\(aq, \(aqNrExposedFrames\(aq, \(aqNrOffsetFrames\(aq, \(aqOffset\(aq, \(aqPixelFormat\(aq, \(aqReadOutMode\(aq, \(aqStandby\(aq, \(aqSumScheme\(aq], \(aqdalsavds\(aq: [\(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqTriggerMode\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqExtendedExposure\(aq, \(aqBinComment\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqFramesReceived\(aq, \(aqFrameRate\(aq, \(aqFramesPerNXFile\(aq, \(aqNXFileCompression\(aq, \(aqTurboMode\(aq, \(aqImageEnc\(aq, \(aqViewingMode\(aq, \(aqThrashedBuffers\(aq, \(aqFramesToAcquire\(aq, \(aqAcquisitionFrameCount\(aq, \(aqAcquisitionMode\(aq, \(aqAcquisitionFrameMode\(aq, \(aqLinearityEqualizer\(aq, \(aqNrExposedFrames\(aq, \(aqNrOffsetFrames\(aq, \(aqOffset\(aq, \(aqPixelFormat\(aq, \(aqReadOutMode\(aq, \(aqStandby\(aq, \(aqSumScheme\(aq], \(aqeigerdectris\(aq: [\(aqTriggerMode\(aq, \(aqNbTriggers\(aq, \(aqDescription\(aq, \(aqNbImages\(aq, \(aqBitDepth\(aq, \(aqReadoutTime\(aq, \(aqCountTime\(aq, \(aqEnergyThreshold\(aq, \(aqFrameTime\(aq, \(aqRateCorrectionEnabled\(aq, \(aqFlatFieldEnabled\(aq, \(aqTemperature\(aq, \(aqAutoSummationEnabled\(aq, \(aqHumidity\(aq, \(aqPhotonEnergy\(aq, \(aqWavelength\(aq], \(aqlambda\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq, \(aqTranslations\(aq], \(aqlambda2m\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqOpMode\(aq, \(aqTranslations\(aq], \(aqlambdavds\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq, \(aqTranslations\(aq], \(aqlambdavdsnm\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq, \(aqTranslations\(aq], \(aqlimaccd\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqlimaccds\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqmaiadimension\(aq: [\(aqName\(aq, \(aqPositionSource\(aq, \(aqPixelPitch\(aq, \(aqPixelOrigin\(aq, \(aqPixelHysteresis\(aq, \(aqPositionUnit\(aq, \(aqPixelCoordExtent\(aq], \(aqmaiaflux\(aq: [\(aqFluxCoeff\(aq, \(aqFluxName\(aq, \(aqFluxUnit\(aq, \(aqFluxSource\(aq], \(aqmaiainterlock\(aq: [\(aqBiasPeltierInterlock\(aq, \(aqBiasPeltierInterlockUptime\(aq, \(aqPressure\(aq], \(aqmaialogger\(aq: [\(aqRunNumber\(aq], \(aqmaiaprocessing\(aq: [\(aqGaintrimEnable\(aq, \(aqLineariseEnable\(aq, \(aqPhotonEnable\(aq, \(aqPileupRejectEnable\(aq, \(aqPixelEnable\(aq, \(aqThrottleEnable\(aq], \(aqmaiasensor\(aq: [\(aqBiasVoltage\(aq, \(aqLeakageCurrent\(aq, \(aqPeltierCurrent\(aq, \(aqWaterTemperature\(aq, \(aqDetectorTemperature\(aq, \(aqMosfetTemperature\(aq, \(aqIdentity\(aq], \(aqmarccd\(aq: [\(aqFrameShift\(aq, \(aqSavingDirectory\(aq, \(aqSavingPostfix\(aq, \(aqSavingPrefix\(aq], \(aqmca_xia\(aq: [\(aqICR\(aq, \(aqOCR\(aq], \(aqmca_xia@pool\(aq: [\(aqCountsRoI\(aq, \(aqRoIEnd\(aq, \(aqRoIStart\(aq], \(aqmythen\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqRoI1\(aq, \(aqRoI2\(aq], \(aqmythen2\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqEnergy\(aq, \(aqNbFrames\(aq, \(aqRoI1End\(aq, \(aqRoI2End\(aq, \(aqRoI1Start\(aq, \(aqRoI2Start\(aq, \(aqThreshold\(aq], \(aqpco\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpco4000\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpcoedge\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpedetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmer\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmerdetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqpilatus\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus100k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus1m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus2m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus300k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus6m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqtangovimba\(aq: [\(aqWidth\(aq, \(aqWidthMax\(aq, \(aqTriggerSource\(aq, \(aqPixelFormat\(aq, \(aqOffsetY\(aq, \(aqOffsetX\(aq, \(aqHeightMax\(aq, \(aqHeight\(aq, \(aqGainRaw\(aq, \(aqExposureTimeAbs\(aq, \(aqAcquisitionFrameRateAbs\(aq, \(aqAcquisitionFrameRateLimit\(aq, \(aqStreamBytesPerSecond\(aq, \(aqBinComment\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqMaxLoad\(aq, \(aqReadMode\(aq, \(aqTuneMode\(aq, \(aqViewingMode\(aq]}
+(\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
+important attributes of modules
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.moduleTemplateFiles  =  {\(aqcobold\(aq: [\(aqcobold.xml\(aq], \(aqdalsa\(aq: [\(aqdalsa.xml\(aq, \(aqdalsa_nxdata.ds.xml\(aq, \(aqdalsa_external_data.ds.xml\(aq], \(aqdalsavds\(aq: [\(aqdalsavds.xml\(aq, \(aqdalsavds_nxdata.ds.xml\(aq, \(aqdalsavds_triggermode_cb.ds.xml\(aq, \(aqdalsavds_filestartnum_cb.ds.xml\(aq, \(aqdalsavds_nrexposedframes_cb.ds.xml\(aq], \(aqeigerdectris\(aq: [\(aqeigerdectris.xml\(aq, \(aqeigerdectris_stepindex.ds.xml\(aq, \(aqeigerdectris_description_cb.ds.xml\(aq, \(aqeigerdectris_triggermode_cb.ds.xml\(aq], \(aqlambda\(aq: [\(aqlambda.xml\(aq, \(aqlambda_nxdata.ds.xml\(aq, \(aqlambda_external_data.ds.xml\(aq], \(aqlambda2m\(aq: [\(aqlambda2m.xml\(aq, \(aqlambda2m_m1_nxdata.ds.xml\(aq, \(aqlambda2m_m2_nxdata.ds.xml\(aq, \(aqlambda2m_m3_nxdata.ds.xml\(aq, \(aqlambda2m_m1_external_data.ds.xml\(aq, \(aqlambda2m_m2_external_data.ds.xml\(aq, \(aqlambda2m_m3_external_data.ds.xml\(aq], \(aqlambdavds\(aq: [\(aqlambdavds.xml\(aq, \(aqlambdavds_nxdata.ds.xml\(aq, \(aqlambdavds_description.ds.xml\(aq, \(aqlambdavds_triggermode_cb.ds.xml\(aq, \(aqlambdavds_framenumbers_cb.ds.xml\(aq, \(aqlambdavds_savefilename_cb.ds.xml\(aq], \(aqlambdavdsnm\(aq: [\(aqlambdavdsnm.xml\(aq, \(aqlambdavdsnm_triggermode_cb.ds.xml\(aq, \(aqlambdavdsnm_nxdata.ds.xml\(aq], \(aqlimaccd\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqlimaccds\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqmarccd\(aq: [\(aqmarccd.xml\(aq, \(aqmarccd_postrun.ds.xml\(aq], \(aqmca_xia\(aq: [\(aqmcaxia.xml\(aq], \(aqmythen\(aq: [\(aqmythen.xml\(aq, \(aqmythen_postrun.ds.xml\(aq, \(aqmythen_filestartnumber.ds.xml\(aq], \(aqmythen2\(aq: [\(aqmythen2.xml\(aq], \(aqpco\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpco4000\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpcoedge\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpedetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmer\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmerdetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqpilatus\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus100k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus100k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus1m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus1m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus2m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus300k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus300k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus6m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqtangovimba\(aq: [\(aqtangovimba.xml\(aq, \(aqtangovimba_nxdata.ds.xml\(aq, \(aqtangovimba_external_data.ds.xml\(aq]}
+(\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
+xml template files of modules
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.motorModules  =  [\(aqabsbox\(aq, \(aqmotor_tango\(aq, \(aqkohzu\(aq, \(aqsmchydra\(aq, \(aqlom\(aq, \(aqoms58\(aq, \(aqe6c\(aq, \(aqomsmaxv\(aq, \(aqspk\(aq, \(aqpie710\(aq, \(aqpie712\(aq, \(aqe6c_p09_eh2\(aq, \(aqsmaract\(aq]
+(\fI\%list\fP <\fI\%str\fP>) modules of motors
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.oneDModules  =  [\(aqmca_xia\(aq]
+(\fI\%list\fP <\fI\%str\fP>) modules of 1D detectors
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.openServer(device)
+opens connection to the configuration server
+.INDENT 7.0
+.TP
+.B Parameters
+\fBconfiguration\fP (\fI\%str\fP) \-\- server device name
+.TP
+.B Returns
+configuration server proxy
+.TP
+.B Return type
+\fI\%tango.DeviceProxy\fP
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.standardComponentTemplateFiles  =  {\(aqabsorber\(aq: [\(aqabsorber_foil.ds.xml\(aq, \(aqabsorber_thickness.ds.xml\(aq, \(aqabsorber.xml\(aq], \(aqbeamstop\(aq: [\(aqbeamstop.xml\(aq], \(aqbeamtimefname\(aq: [\(aqbeamtimefname.xml\(aq, \(aqbeamtimefname.ds.xml\(aq, \(aqstart_time.ds.xml\(aq], \(aqbeamtimeid\(aq: [\(aqbeamtimeid.xml\(aq, \(aqbeamtimeid.ds.xml\(aq, \(aqstart_time.ds.xml\(aq], \(aqchcut\(aq: [\(aqchcut.xml\(aq, \(aqchcut_unitcalibration.ds.xml\(aq, \(aqchcut_crystal.ds.xml\(aq], \(aqcoboldhisto\(aq: [\(aqcoboldhisto.xml\(aq, \(aqcoboldhisto_timeofflight.ds.xml\(aq], \(aqcollect2\(aq: [\(aqcollect2.xml\(aq], \(aqcollect3\(aq: [\(aqcollect3.xml\(aq], \(aqcollect4\(aq: [\(aqcollect4.xml\(aq], \(aqcollect5\(aq: [\(aqcollect5.xml\(aq], \(aqcollect6\(aq: [\(aqcollect6.xml\(aq], \(aqcommon2\(aq: [\(aqcommon2_common.ds.xml\(aq], \(aqcommon3\(aq: [\(aqcommon3_common.ds.xml\(aq], \(aqdataaxessignal\(aq: [\(aqdataaxessignal.xml\(aq, \(aqdefaultsignal.ds.xml\(aq, \(aqdefaultaxes.ds.xml\(aq, \(aqsignal_name.ds.xml\(aq, \(aqsignalname.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqdatasignal\(aq: [\(aqdatasignal.xml\(aq, \(aqdefaultsignal.ds.xml\(aq, \(aqsignal_name.ds.xml\(aq, \(aqsignalname.ds.xml\(aq, \(aqsignal_axes.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqdcm\(aq: [\(aqdcm.xml\(aq, \(aqdcm_reflection.ds.xml\(aq, \(aqdcm_unitcalibration.ds.xml\(aq, \(aqdcm_crystal.ds.xml\(aq], \(aqdefault\(aq: [\(aqdefault.xml\(aq, \(aqdefaultsample.xml\(aq, \(aqdefaultinstrument.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqbeamtime_filename.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultinstrument\(aq: [\(aqdefaultinstrument.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqbeamtime_filename.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultsample\(aq: [\(aqdefaultsample.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq], \(aqdescription\(aq: [\(aqdescription.xml\(aq, \(aqexperiment_description.ds.xml\(aq], \(aqdescriptiontext\(aq: [\(aqdescriptiontext.xml\(aq], \(aqdetectorlive\(aq: [\(aqdetectorlive.xml\(aq], \(aqempty\(aq: [\(aqempty.xml\(aq], \(aqgroupsecop\(aq: [\(aqgroupsecop.ds.xml\(aq, \(aqgroupsecop_time.ds.xml\(aq, \(aqclient_start_time.ds.xml\(aq, \(aqsample_env_links.ds.xml\(aq, \(aqsample_log_links.ds.xml\(aq], \(aqkeithley\(aq: [\(aqkeithley.xml\(aq], \(aqmaia\(aq: [\(aqmaia.xml\(aq, \(aqempty.xml\(aq], \(aqmaiadimension\(aq: [\(aqmaiadimension.xml\(aq], \(aqmaiaflux\(aq: [\(aqmaiaflux.xml\(aq], \(aqmsnsar\(aq: [\(aqmsnsar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqmssar\(aq: [\(aqmssar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqparametercopymap\(aq: [\(aqparametercopymap.xml\(aq], \(aqpinhole\(aq: [\(aqpinhole.xml\(aq], \(aqpointdet\(aq: [\(aqpointdet.xml\(aq], \(aqqbpm\(aq: [\(aqqbpm_foil.ds.xml\(aq, \(aqqbpm.xml\(aq], \(aqsampledescription\(aq: [\(aqsampledescription.xml\(aq, \(aqsample_description.ds.xml\(aq], \(aqsampledescriptiontext\(aq: [\(aqsampledescriptiontext.xml\(aq], \(aqsamplehkl\(aq: [\(aqsamplehkl.xml\(aq], \(aqsecop\(aq: [\(aqsecop.ds.xml\(aq, \(aqsecop_time.ds.xml\(aq, \(aqclient_start_time.ds.xml\(aq, \(aqsample_env_links.ds.xml\(aq, \(aqsample_log_links.ds.xml\(aq], \(aqsecoplinks\(aq: [\(aqsample_env_links.ds.xml\(aq, \(aqsample_log_links.ds.xml\(aq, \(aqsample_nxdata.ds.xml\(aq, \(aqsampleenv_nxdata.ds.xml\(aq], \(aqsinglesecop\(aq: [\(aqsinglesecop.ds.xml\(aq, \(aqsinglesecop_time.ds.xml\(aq, \(aqclient_start_time.ds.xml\(aq, \(aqsample_env_links.ds.xml\(aq, \(aqsample_log_links.ds.xml\(aq], \(aqslit\(aq: [\(aqslit.xml\(aq], \(aqsource\(aq: [\(aqsource.xml\(aq], \(aqstarttime\(aq: [\(aqstarttime.xml\(aq, \(aqstarttime.ds.xml\(aq, \(aqstart_timestamp.ds.xml\(aq, \(aqclient_start_time.ds.xml\(aq], \(aqtango\(aq: [\(aqtango.ds.xml\(aq], \(aqundulator\(aq: [\(aqundulator.xml\(aq]}
+(\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
+xml template files of modules
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.standardComponentVariables  =  {\(aqabsorber\(aq: {\(aqattenfactor\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqattenuation factor (datasource)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqfoil\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil type, i.e. standard <cpname>_foil (datasource)\(aq}, \(aqfoillist\(aq: {\(aqdefault\(aq: \(aq[\(dqAg\(dq, \(dqAg\(dq, \(dqAg\(dq, \(dqAg\(dq, \(dq\(dq, \(dqAl\(dq, \(dqAl\(dq, \(dqAl\(dq, \(dqAl\(dq]\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqposition\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqwhich sliders are in [bitarray] MANDATORY (datasource)\(aq}, \(aqthickness\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil thickness, i.e. standard <cpname>_thickness (datasource)\(aq}, \(aqthicknesslist\(aq: {\(aqdefault\(aq: \(aq[0.5, 0.05, 0.025, 0.0125, 0, 0.1, 0.3, 0.5, 1.0]\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(dqtransformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)\(dq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}}, \(aqbeamstop\(aq: {\(aqdescription\(aq: {\(aqdefault\(aq: \(aqcircular\(aq, \(aqdoc\(aq: \(aq circular or  rectangular (string)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqxsign\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(dqhorizontal position sign, e.g. \(aq\-\(aq (string)\(dq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}, \(aqz\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqzname\(aq: {\(aqdefault\(aq: \(aqz\(aq, \(aqdoc\(aq: \(aqalong the beam position name (string)\(aq}}, \(aqbeamtimefname\(aq: {\(aqcommissiondir\(aq: {\(aqdefault\(aq: \(aq/gpfs/commissioning\(aq, \(aqdoc\(aq: \(aqcommission file directory (string)\(aq}, \(aqcommissionpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqcommission file postfix (string)\(aq}, \(aqcommissionprefix\(aq: {\(aqdefault\(aq: \(aqcommissioning\-metadata\-\(aq, \(aqdoc\(aq: \(aqcommission file prefix (string)\(aq}, \(aqcurrentdir\(aq: {\(aqdefault\(aq: \(aq/gpfs/current\(aq, \(aqdoc\(aq: \(aqbeamtime file directory (string)\(aq}, \(aqcurrentpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqbeamtime file postfix (string)\(aq}, \(aqcurrentprefix\(aq: {\(aqdefault\(aq: \(aqbeamtime\-metadata\-\(aq, \(aqdoc\(aq: \(aqbeamtime file prefix (string)\(aq}, \(aqlocaldir\(aq: {\(aqdefault\(aq: \(aq/gpfs/local\(aq, \(aqdoc\(aq: \(aqlocal file directory (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}}, \(aqbeamtimeid\(aq: {\(aqcommissiondir\(aq: {\(aqdefault\(aq: \(aq/gpfs/commissioning\(aq, \(aqdoc\(aq: \(aqcommission file directory (string)\(aq}, \(aqcommissionpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqcommission file postfix (string)\(aq}, \(aqcommissionprefix\(aq: {\(aqdefault\(aq: \(aqcommissioning\-metadata\-\(aq, \(aqdoc\(aq: \(aqcommission file prefix (string)\(aq}, \(aqcurrentdir\(aq: {\(aqdefault\(aq: \(aq/gpfs/current\(aq, \(aqdoc\(aq: \(aqbeamtime file directory (string)\(aq}, \(aqcurrentpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqbeamtime file postfix (string)\(aq}, \(aqcurrentprefix\(aq: {\(aqdefault\(aq: \(aqbeamtime\-metadata\-\(aq, \(aqdoc\(aq: \(aqbeamtime file prefix (string)\(aq}, \(aqlocaldir\(aq: {\(aqdefault\(aq: \(aq/gpfs/local\(aq, \(aqdoc\(aq: \(aqlocal file directory (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}}, \(aqchcut\(aq: {\(aqbraggangle\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbragg angle (datasource)\(aq}, \(aqbragganglename\(aq: {\(aqdefault\(aq: \(aqbragg\(aq, \(aqdoc\(aq: \(aqbragg angle name  (string)\(aq}, \(aqchcutdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqFMBOxfDCMEnergy tango device name (string)\(aq}, \(aqcrystal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq type of crystal i.e. 0\->Si111,1\->Si311,2\->Si111 ChannelCut  (datasource)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsynchronized monochromator energy (datasource)\(aq}, \(aqenergyfmb\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmonochromator energy (datasource)\(aq}, \(aqjack1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfirst vertical jack of table (datasource)\(aq}, \(aqjack1name\(aq: {\(aqdefault\(aq: \(aqjack1\(aq, \(aqdoc\(aq: \(aqfirst vertical jack name of table (string)\(aq}, \(aqjack2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond vertical jack of table (datasource)\(aq}, \(aqjack2name\(aq: {\(aqdefault\(aq: \(aqjack2\(aq, \(aqdoc\(aq: \(aqsecond vertical jack name of table (string)\(aq}, \(aqjack3\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthird vertical jack of table (datasource)\(aq}, \(aqjack3name\(aq: {\(aqdefault\(aq: \(aqjack3\(aq, \(aqdoc\(aq: \(aqthird vertical jack name of table (string)\(aq}, \(aqlat\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the first cristal (datasource)\(aq}, \(aqlatname\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the first cristal (string)\(aq}, \(aqoxfordhorizontal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq horizontal translation (datasource)\(aq}, \(aqpara\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance between the crystals (string)\(aq}, \(aqparaname\(aq: {\(aqdefault\(aq: \(aqpara\(aq, \(aqdoc\(aq: \(aqbeam parallel translation name of the second cristal (string)\(aq}, \(aqreflection\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqreflection from string (datasource)\(aq}, \(aqtable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position of table (datasource)\(aq}, \(aqtablename\(aq: {\(aqdefault\(aq: \(aqtable\(aq, \(aqdoc\(aq: \(aqvertical position name of table (string)\(aq}, \(aqtheta\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta angle (datasource)\(aq}, \(aqthetaname\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta angle name (string)\(aq}, \(aqunitcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq unit calibration from dcmmotor (datasource)\(aq}, \(aqusage\(aq: {\(aqdefault\(aq: \(aqBragg\(aq, \(aqdoc\(aq: \(aqthe crystall usage, e.g. Laue (string)\(aq}, \(aqyaw\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the first cristal (datasource)\(aq}, \(aqyawname\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the first cristal (string)\(aq}}, \(aqcoboldhisto\(aq: {\(aqbinsize\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbin size of histogram data (datasource)\(aq}, \(aqexposuretime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqexposure time for histogram data (datasource)\(aq}, \(aqhistogram\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhistogram data (datasource)\(aq}}, \(aqcollect2\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}}, \(aqcollect3\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect4\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect5\(aq: {\(aqfifth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fifth component to collect MANDATORY (datasource)\(aq}, \(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect6\(aq: {\(aqfifth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fifth component to collect MANDATORY (datasource)\(aq}, \(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqsixth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the sixth component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcommon2\(aq: {\(aqdds\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdefault read datasource name MANDATORY (datasource)\(aq}, \(aqods\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqoptional detasource name MANDATORY (datasource)\(aq}}, \(aqcommon3\(aq: {\(aqdds\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdefault read datasource name MANDATORY (datasource)\(aq}, \(aqods1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfist optional detasource name MANDATORY (datasource)\(aq}, \(aqods2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond optional detasource name MANDATORY (datasource)\(aq}}, \(aqdataaxessignal\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqaxes\(aq: {\(aqdefault\(aq: \(aqdefaultaxes\(aq, \(aqdoc\(aq: \(aqlist of data axes field names (datasource)\(aq}, \(aqdefaultattrs\(aq: {\(aqdefault\(aq: \(aqFalse\(aq, \(aqdoc\(aq: \(aqadd default attributes (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmacroserver sardana device name MANDATORY (string)\(aq}, \(aqnchannelstoskip\(aq: {\(aqdefault\(aq: \(aq0\(aq, \(aqdoc\(aq: \(aqnumber of mg channels to skip (string)\(aq}, \(aqsardanasignal\(aq: {\(aqdefault\(aq: \(aqSignalCounter\(aq, \(aqdoc\(aq: \(aqsignal sardana variable name (string)\(aq}, \(aqsignal\(aq: {\(aqdefault\(aq: \(aqdefaultsignal\(aq, \(aqdoc\(aq: \(aqdata signal field name (datasource)\(aq}}, \(aqdatasignal\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqaxes\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdata axes field name(s) (datasource)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmacroserver sardana device name MANDATORY (string)\(aq}, \(aqnchannelstoskip\(aq: {\(aqdefault\(aq: \(aq0\(aq, \(aqdoc\(aq: \(aqnumber of mg channels to skip (string)\(aq}, \(aqsardanasignal\(aq: {\(aqdefault\(aq: \(aqSignalCounter\(aq, \(aqdoc\(aq: \(aqsignal sardana variable name (string)\(aq}, \(aqsignal\(aq: {\(aqdefault\(aq: \(aqdefaultsignal\(aq, \(aqdoc\(aq: \(aqdata signal field name (datasource)\(aq}}, \(aqdcm\(aq: {\(aqbend1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbending of the first cristal (datasource)\(aq}, \(aqbend2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbending of the second cristal (datasource)\(aq}, \(aqbraggangle\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbragg angle (datasource)\(aq}, \(aqbragganglename\(aq: {\(aqdefault\(aq: \(aqbragg\(aq, \(aqdoc\(aq: \(aqbragg angle name  (string)\(aq}, \(aqchi2dependson\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqthe depends_on field of the second cristal chi, e.g. phi (string)\(aq}, \(aqcrystal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtype of crystal i.e. 0\->Si111,1\->Si311,2\->Si111 ChannelCut (datasource)\(aq}, \(aqdcmdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqFMBOxfDCMEnergy tango device (string)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsynchronized monochromator energy (datasource)\(aq}, \(aqenergyfmb\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmonochromator energy (datasource)\(aq}, \(aqexitoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq exit offset (datasource)\(aq}, \(aqjack1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfirst vertical jack of table (datasource)\(aq}, \(aqjack1name\(aq: {\(aqdefault\(aq: \(aqjack1\(aq, \(aqdoc\(aq: \(aqfirst vertical jack name of table (string)\(aq}, \(aqjack2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond vertical jack of table (datasource)\(aq}, \(aqjack2name\(aq: {\(aqdefault\(aq: \(aqjack2\(aq, \(aqdoc\(aq: \(aqsecond vertical jack name of table (string)\(aq}, \(aqjack3\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthird vertical jack of table (datasource)\(aq}, \(aqjack3name\(aq: {\(aqdefault\(aq: \(aqjack3\(aq, \(aqdoc\(aq: \(aqthird vertical jack name of table (string)\(aq}, \(aqlat\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the first cristal (datasource)\(aq}, \(aqlat2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the second cristal (datasource)\(aq}, \(aqlat2name\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the second cristal (string)\(aq}, \(aqlatname\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the first cristal (string)\(aq}, \(aqoxfordhorizontal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq horizontal translation (datasource)\(aq}, \(aqpar2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbeam parallel translation of the second cristal (datasource)\(aq}, \(aqpar2name\(aq: {\(aqdefault\(aq: \(aqpara\(aq, \(aqdoc\(aq: \(aqbeam parallel translation name of the second cristal (string)\(aq}, \(aqperp2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical translation of the second cristal (datasource)\(aq}, \(aqperp2name\(aq: {\(aqdefault\(aq: \(aqperp\(aq, \(aqdoc\(aq: \(aqvertical translation name of the second cristal (string)\(aq}, \(aqphi1dependson\(aq: {\(aqdefault\(aq: \(aq../../transformations/bragg\(aq, \(aqdoc\(aq: \(aqthe depends_on field of the first cristal phi, e.g. theta (string)\(aq}, \(aqpitch1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta rotation of the first cristal (datasource)\(aq}, \(aqpitch1name\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta rotation name of the first cristal (string)\(aq}, \(aqpitch2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta rotation of the second cristal (datasource)\(aq}, \(aqpitch2name\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta rotation name of the second cristal (string)\(aq}, \(aqroll1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchi rotation of the first cristal (datasource)\(aq}, \(aqroll1name\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqchi rotation name of the first cristal (string)\(aq}, \(aqroll2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchi rotation of the second cristal (datasource)\(aq}, \(aqroll2name\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqchi rotation name of the second cristal (string)\(aq}, \(aqtable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position of table (datasource)\(aq}, \(aqtablename\(aq: {\(aqdefault\(aq: \(aqtable\(aq, \(aqdoc\(aq: \(aqvertical position name of table (string)\(aq}, \(aqtheta\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta angle (datasource)\(aq}, \(aqthetaname\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta angle name (string)\(aq}, \(aqtopdependson2\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqthe first transformation of the second crystal, e.g. lat (string)\(aq}, \(aqunitcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqunit calibration from dcmmotor (datasource)\(aq}, \(aqusage\(aq: {\(aqdefault\(aq: \(aqBragg\(aq, \(aqdoc\(aq: \(aqthe crystall usage, e.g. Laue (string)\(aq}, \(aqyaw\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the first cristal (datasource)\(aq}, \(aqyaw2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the second cristal (datasource)\(aq}, \(aqyaw2name\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the second cristal (string)\(aq}, \(aqyawname\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the first cristal (string)\(aq}}, \(aqdefault\(aq: {\(aq__configdevice__\(aq: {\(aqdefault\(aq: \(aqnxs/configserver/localhost\(aq, \(aqdoc\(aq: \(aqconfiguration server device name (string)\(aq}, \(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqcontrol\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgroup name of the monitor (string)\(aq}, \(aqlongname\(aq: {\(aqdefault\(aq: \(aqP09 Resonant Scattering and Diffraction beamline\(aq, \(aqdoc\(aq: \(aqbeamline long name (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}, \(aqsourcename\(aq: {\(aqdefault\(aq: \(aqPETRA III\(aq, \(aqdoc\(aq: \(aqsource name (string)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqdefaultinstrument\(aq: {\(aq__configdevice__\(aq: {\(aqdefault\(aq: \(aqnxs/configserver/localhost\(aq, \(aqdoc\(aq: \(aqconfiguration server device name (string)\(aq}, \(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqcontrol\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgroup name of the monitor (string)\(aq}, \(aqlongname\(aq: {\(aqdefault\(aq: \(aqP09 Resonant Scattering and Diffraction beamline\(aq, \(aqdoc\(aq: \(aqbeamline long name (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}, \(aqsourcename\(aq: {\(aqdefault\(aq: \(aqPETRA III\(aq, \(aqdoc\(aq: \(aqsource name (string)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqdefaultsample\(aq: {}, \(aqdescription\(aq: {}, \(aqdescriptiontext\(aq: {\(aqdescription\(aq: {\(aqdefault\(aq: \(aqscan\(aq, \(aqdoc\(aq: \(aqscan technique (string)\(aq}}, \(aqdetectorlive\(aq: {\(aqdatatype\(aq: {\(aqdefault\(aq: \(aqNX_UINT32\(aq, \(aqdoc\(aq: \(aqlist of devices (string)\(aq}, \(aqdetectordata\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdetector live data (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqdetector\(aq, \(aqdoc\(aq: \(aqlist of devices (string)\(aq}}, \(aqempty\(aq: {}, \(aqgroupsecop\(aq: {\(aqaccess\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop access list (string)\(aq}, \(aqgroup\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop group name (string)\(aq}, \(aqhost\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop host name (string)\(aq}, \(aqmessage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop command MANDATORY (string)\(aq}, \(aqport\(aq: {\(aqdefault\(aq: \(aq5000\(aq, \(aqdoc\(aq: \(aqsecop port name (string)\(aq}, \(aqtimeout\(aq: {\(aqdefault\(aq: \(aq0.0001\(aq, \(aqdoc\(aq: \(aqsecop timeout (string)\(aq}}, \(aqkeithley\(aq: {\(aqcurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqcurrent in A (datasource)\(aq}, \(aqgain\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgain in V/A (datasource)\(aq}, \(aqrisetime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqrise time (datasource)\(aq}, \(aqsourvoltlevel\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsource voltage level in V (datasource)\(aq}, \(aqvoltage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvoltage in V (datasource)\(aq}}, \(aqmaia\(aq: {\(aqchillersetpoint\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchiller set point temperature in Celsus (datasource)\(aq}, \(aqchiptemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdetector chip temperature sensor for maia in Celsus (datasource)\(aq}, \(aqgaintrimenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgaintrim enable status for maia (datasource)\(aq}, \(aqidentity\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsensor identity for maia (datasource)\(aq}, \(aqinterlockpressure\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock pressure for maia in mbar (datasource)\(aq}, \(aqleakagecurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleakage current sensor for maia in A (datasource)\(aq}, \(aqlineariseenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqlinearise enable status for maia (datasource)\(aq}, \(aqmaiadimensions\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia dimensions component name (component)\(aq}, \(aqmaiafluxes\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia fluxes component name (component)\(aq}, \(aqmaiastage\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia stage component name (component)\(aq}, \(aqmosfettemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmosfet temperature sensor for maia in Celsus (datasource)\(aq}, \(aqpeltiercurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpeltier current sensor for maia in A (datasource)\(aq}, \(aqphotonenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphoton enable status for maia (datasource)\(aq}, \(aqpileuprejectionenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpileup rejection enable status for maia (datasource)\(aq}, \(aqpixelenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel enable status for maia (datasource)\(aq}, \(aqpressure\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgas pressure in mbar (datasource)\(aq}, \(aqrunnumber\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqrun number of maia (datasource)\(aq}, \(aqstatus\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock status for maia (datasource)\(aq}, \(aqthrottleenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthrottle enable status for maia (datasource)\(aq}, \(aquptime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock uptime for maia (datasource)\(aq}, \(aqvoltagesetpoint\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvoltage set point temperature in Celsus (datasource)\(aq}, \(aqwatertemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqwater temperature sensor for maia in Celsus (datasource)\(aq}}, \(aqmaiadimension\(aq: {\(aqdetname\(aq: {\(aqdefault\(aq: \(aqmaia\(aq, \(aqdoc\(aq: \(aqdetector (alias) name (string)\(aq}, \(aqdimname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdimension name for maia (datasource)\(aq}, \(aqdname\(aq: {\(aqdefault\(aq: \(aqdimension\(aq, \(aqdoc\(aq: \(aqdimension name group (string)\(aq}, \(aqhysteresis\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel hysteresis of dimension for maia (datasource)\(aq}, \(aqnumberofpixels\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnumber of pixels of dimension for maia (datasource)\(aq}, \(aqorigin\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel origin of dimension for maia (datasource)\(aq}, \(aqpixelpitch\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel pitch of dimension for maia (datasource)\(aq}, \(aqpositionsource\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqposition source of dimension for maia (datasource)\(aq}, \(aqunit\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqposition units of dimension for maia (datasource)\(aq}}, \(aqmaiaflux\(aq: {\(aqcoefficient\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux coefficient  for maia (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqmaia\(aq, \(aqdoc\(aq: \(aqdetector (alias) name (string)\(aq}, \(aqfluxname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux name for maia (datasource)\(aq}, \(aqfname\(aq: {\(aqdefault\(aq: \(aqfluxdevice\(aq, \(aqdoc\(aq: \(aqflux name group (string)\(aq}, \(aqkeithleydevice\(aq: {\(aqdefault\(aq: \(aqkeithley\(aq, \(aqdoc\(aq: \(aqkeithley device name (string)\(aq}, \(aqsource\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux source for maia (datasource)\(aq}, \(aqunit\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux unit for maia (datasource)\(aq}, \(aqvfcfactor\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvfc conversion factor (datasource)\(aq}}, \(aqmsnsar\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana device name MANDATORY (string)\(aq}, \(aqvarname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnested sardana environment variable name  MANDATORY (string)\(aq}}, \(aqmssar\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmacroserver sardana device name MANDATORY (string)\(aq}, \(aqvarname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment variable name MANDATORY (string)\(aq}}, \(aqparametercopymap\(aq: {\(aqcopymap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqyaml dictionary with {output: input} copy map (string)\(aq}, \(aqparameter\(aq: {\(aqdefault\(aq: \(aqcopymap\(aq, \(aqdoc\(aq: \(aqparameter name of copymap (string)\(aq}, \(aqprogram\(aq: {\(aqdefault\(aq: \(aqnxsfileinfo_parameters\(aq, \(aqdoc\(aq: \(aqgroup name of NXparameters (string)\(aq}}, \(aqpinhole\(aq: {\(aqdiameter\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpinhole diameter (datasource)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqxsign\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(dqhorizontal position sign, e.g. \(aq\-\(aq (string)\(dq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}, \(aqz\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqalong the beam position (datasource)\(aq}, \(aqzname\(aq: {\(aqdefault\(aq: \(aqz\(aq, \(aqdoc\(aq: \(aqalong the beam position name (string)\(aq}}, \(aqpointdet\(aq: {\(aqdata\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdiode data (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqdetector\(aq, \(aqdoc\(aq: \(aqdetector group name (string)\(aq}}, \(aqqbpm\(aq: {\(aqdependsony\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqthe  depends_on y field value,  e.g. distance (string)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqfoil\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil type, i.e. standard <cpname>_foil (datasource)\(aq}, \(aqfoilpos\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil position MANDATORY (datasource)\(aq}, \(aqfoilposdict\(aq: {\(aqdefault\(aq: \(aq{\(dqTi\(dq: 43, \(dqNi\(dq: 23, \(dqOut\(dq: 3}\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}}, \(aqsampledescription\(aq: {\(aqsname\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqsampledescriptiontext\(aq: {\(aqdescription\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqsample description or sampleId (string)\(aq}, \(aqsname\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqsamplehkl\(aq: {\(aqh\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqh position in hkl space (datasource)\(aq}, \(aqk\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqk position in hkl space (datasource)\(aq}, \(aql\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aql position in hkl space (datasource)\(aq}, \(aqpsi\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpsi angle position of analyzer (datasource)\(aq}, \(aqsname\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqsecop\(aq: {\(aqhost\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop host name (string)\(aq}, \(aqmessage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop command MANDATORY (string)\(aq}, \(aqport\(aq: {\(aqdefault\(aq: \(aq5000\(aq, \(aqdoc\(aq: \(aqsecop port name (string)\(aq}, \(aqtimeout\(aq: {\(aqdefault\(aq: \(aq0.0001\(aq, \(aqdoc\(aq: \(aqsecop timeout (string)\(aq}}, \(aqsecoplinks\(aq: {\(aqenvironments\(aq: {\(aqdefault\(aq: \(aqtemperature,magnetic_field\(aq, \(aqdoc\(aq: \(aqsecop environment link lists MANDATORY (string)\(aq}, \(aqmeanings\(aq: {\(aqdefault\(aq: \(aqtemperature,magnetic_field,electric_field,stress_field,pressure\(aq, \(aqdoc\(aq: \(aqsecop meanings link lists MANDATORY (string)\(aq}, \(aqsampleenvname\(aq: {\(aqdefault\(aq: \(aqsample_environment\(aq, \(aqdoc\(aq: \(aqsample environment group name (string)\(aq}, \(aqsamplename\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqsinglesecop\(aq: {\(aqhost\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop host name (string)\(aq}, \(aqmessage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop command MANDATORY (string)\(aq}, \(aqport\(aq: {\(aqdefault\(aq: \(aq5000\(aq, \(aqdoc\(aq: \(aqsecop port name (string)\(aq}, \(aqtimeout\(aq: {\(aqdefault\(aq: \(aq0.0001\(aq, \(aqdoc\(aq: \(aqsecop timeout (string)\(aq}}, \(aqslit\(aq: {\(aqbottom\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbottom blade position (datasource)\(aq}, \(aqbottomclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbottom blade closed position (datasource)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqleft\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleft blade position (datasource)\(aq}, \(aqleftclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleft blade closed position (datasource)\(aq}, \(aqright\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqright blade position (datasource)\(aq}, \(aqrightclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqright blade closed position (datasource)\(aq}, \(aqtop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtop blade position (datasource)\(aq}, \(aqtopclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtop blade closed position (datasource)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(dqtransformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)\(dq}, \(aqxgap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal gap (datasource)\(aq}, \(aqxoffdependson\(aq: {\(aqdefault\(aq: \(aqy_offset\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqxoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal offset (datasource)\(aq}, \(aqxoffsetcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal offset calibration (datasource)\(aq}, \(aqxoffsetcalibrationname\(aq: {\(aqdefault\(aq: \(aqx_offset_calibration\(aq, \(aqdoc\(aq: \(aqhorizontal offset calibration name (string)\(aq}, \(aqxoffsetname\(aq: {\(aqdefault\(aq: \(aqx_offset\(aq, \(aqdoc\(aq: \(aqhorizontal offset name (string)\(aq}, \(aqygap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical gap (datasource)\(aq}, \(aqyoffdependson\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqyoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertiacal offset (datasource)\(aq}, \(aqyoffsetcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertiacal offset calibration (datasource)\(aq}, \(aqyoffsetcalibrationname\(aq: {\(aqdefault\(aq: \(aqy_offset_calibration\(aq, \(aqdoc\(aq: \(aqvertiacal offset calibration name (string)\(aq}, \(aqyoffsetname\(aq: {\(aqdefault\(aq: \(aqy_offset\(aq, \(aqdoc\(aq: \(aqvertiacal offset name (string)\(aq}}, \(aqsource\(aq: {\(aqbeamcurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqring beam current (datasource)\(aq}, \(aqbunchmode\(aq: {\(aqdefault\(aq: \(aqMulti Bunch\(aq, \(aqdoc\(aq: \(aqbunch mode (string)\(aq}, \(aqnumberofbunches\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnumber of source bunches (datasource)\(aq}, \(aqsourceenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqring beam energy (datasource)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqstarttime\(aq: {}, \(aqtango\(aq: {\(aqattribute\(aq: {\(aqdefault\(aq: \(aqPosition\(aq, \(aqdoc\(aq: \(aqtango device attribute (string)\(aq}, \(aqdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtango device MANDATORY (string)\(aq}}, \(aqundulator\(aq: {\(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance from the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name from the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator energy (datasource)\(aq}, \(aqgap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqseparation between opposing pairs of magnetic pole (datasource)\(aq}, \(aqgapunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqgap units (string)\(aq}, \(aqharmonic\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator harmonic (datasource)\(aq}, \(aqlength\(aq: {\(aqdefault\(aq: \(aq2\(aq, \(aqdoc\(aq: \(aqlength of insertion device in meters (string)\(aq}, \(aqshift\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator shift (datasource)\(aq}, \(aqshiftunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqshift units (string)\(aq}, \(aqspeed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator speed (datasource)\(aq}, \(aqspeedunits\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqspeed units (string)\(aq}, \(aqtaper\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgap difference between upstream and downstream ends of the insertion device (datasource)\(aq}, \(aqtaperunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqgap units (string)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(dqtransformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)\(dq}, \(aqtype\(aq: {\(aqdefault\(aq: \(aqundulator\(aq, \(aqdoc\(aq: \(aqundulator or wiggler (string)\(aq}, \(aquname\(aq: {\(aqdefault\(aq: \(aqinsertion_device\(aq, \(aqdoc\(aq: \(aqinsertion_device group name (string)\(aq}}}
+(\fI\%dict\fP <\fI\%str\fP , \fI\%dict\fP <\fI\%str\fP , \fI\%str\fP > >)
+standard component template variables
+and its [default value, doc string]
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.storeComponent(name, xml, server, mandatory=False)
+stores components in Configuration Server
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- component name
+.IP \(bu 2
+\fBxml\fP (\fI\%str\fP) \-\- component xml string
+.IP \(bu 2
+\fBserver\fP (\fI\%str\fP) \-\- configuration server
+.IP \(bu 2
+\fBmandatory\fP (\fI\%bool\fP) \-\- set component as mandatory
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.storeDataSource(name, xml, server)
+stores datasources in Configuration Server
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBname\fP (\fI\%str\fP) \-\- datasource name
+.IP \(bu 2
+\fBxml\fP (\fI\%str\fP) \-\- datasource xml string
+.IP \(bu 2
+\fBserver\fP (\fI\%str\fP) \-\- configuration server
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.twoDModules  =  [\(aqpilatus100k\(aq, \(aqpilatus300k\(aq, \(aqpilatus1m\(aq, \(aqpilatus2m\(aq, \(aqpilatus6m\(aq, \(aqpco4000\(aq, \(aqperkinelmerdetector\(aq, \(aqlambda\(aq, \(aqpedetector\(aq, \(aqperkinelmer\(aq, \(aqpco\(aq, \(aqpcoedge\(aq, \(aqmarccd\(aq, \(aqperkinelmer\(aq, \(aqlcxcamera\(aq, \(aqlimaccd\(aq, \(aqeigerpsi\(aq, \(aqeigerdectris\(aq]
+(\fI\%list\fP <\fI\%str\fP>) modules of 2d detectors
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.xmlPackageHandler  =  <nxstools.nxsdevicetools.PackageHandler object>
+(\fI\%PackageHandler\fP) xml template package handler
+.UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsdevicetools.zeroDModules  =  [\(aqtip830\(aq]
+(\fI\%list\fP <\fI\%str\fP>) modules of 0D detectors
+.UNINDENT
 .SS nxstools.nxsetup module
 .sp
 Set Up NeXus Tango Servers
 .INDENT 0.0
 .TP
-.B class nxstools.nxsetup.AddRecorderPath(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsetup.AddRecorderPath(parser)
+Bases: \fI\%Runner\fP
 .sp
 add\-recorder\-path runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqadd\-recorder\-path into MacroServer(s) property\(aq
+.B description  =  \(aqadd\-recorder\-path into MacroServer(s) property\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsetup add\-recorder\-path /usr/share/pyshared/sardananxsrecorder\en       nxsetup add\-recorder\-path \-t /usr/share/pyshared/sardananxsrecorder\en       nxsetup add\-recorder\-path /usr/share/pyshared/sardananxsrecorder \-i haso\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsetup add\-recorder\-path /usr/share/pyshared/sardananxsrecorder\en       nxsetup add\-recorder\-path \-t /usr/share/pyshared/sardananxsrecorder\en       nxsetup add\-recorder\-path /usr/share/pyshared/sardananxsrecorder \-i haso\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsetup.ChangeProp(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsetup.ChangeProp(parser)
+Bases: \fI\%Runner\fP
 .sp
 change\-prop runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqchange property value\(aq
+.B description  =  \(aqchange property value\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsetup change\-prop \-n ClientRecordKeys \-t \-w "[\e\e"phoibos_scan_command\e\e",\e\e"phoibos_scan_comment\e\e"]" NXSRecSelector/r228\en       nxsetup change\-prop \-n DefaultPreselectedComponents \-w "[\e\e"pinhole1\e\e",\e\e"slit2\e\e"]" NXSRecSelector/r228\en       nxsetup change\-prop \-n StartDsPath \-w "[\e\e"/usr/bin\e\e",\e\e"/usr/lib/tango\e\e"]" Starter\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsetup change\-prop \-n ClientRecordKeys \-t \-w \(dq[\e\e\(dqphoibos_scan_command\e\e\(dq,\e\e\(dqphoibos_scan_comment\e\e\(dq]\(dq NXSRecSelector/r228\en       nxsetup change\-prop \-n DefaultPreselectedComponents \-w \(dq[\e\e\(dqpinhole1\e\e\(dq,\e\e\(dqslit2\e\e\(dq]\(dq NXSRecSelector/r228\en       nxsetup change\-prop \-n StartDsPath \-w \(dq[\e\e\(dq/usr/bin\e\e\(dq,\e\e\(dq/usr/lib/tango\e\e\(dq]\(dq Starter\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsetup.MoveProp(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsetup.MoveProp(parser)
+Bases: \fI\%Runner\fP
 .sp
 move\-prop runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqchange property name\(aq
+.B description  =  \(aqchange property name\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsetup move\-prop \-n DefaultPreselectedComponents \-o DefaultAutomaticComponents NXSRecSelector\en       nxsetup move\-prop \-t \-n DefaultPreselectedComponents  \-o DefaultAutomaticComponents NXSRecSelector\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsetup move\-prop \-n DefaultPreselectedComponents \-o DefaultAutomaticComponents NXSRecSelector\en       nxsetup move\-prop \-t \-n DefaultPreselectedComponents  \-o DefaultAutomaticComponents NXSRecSelector\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsetup.Restart(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsetup.Restart(parser)
+Bases: \fI\%Runner\fP
 .sp
 restart runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqrestart tango server\(aq
+.B description  =  \(aqrestart tango server\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsetup restart Pool/haso228 \-l 2\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsetup restart Pool/haso228 \-l 2\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsetup.Set(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsetup.Set(parser)
+Bases: \fI\%Runner\fP
 .sp
 set runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqset up NXSConfigServer NXSDataWriter and NXSRecSelector servers\(aq
+.B description  =  \(aqset up NXSConfigServer NXSDataWriter and NXSRecSelector servers\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsetup set\en       nxsetup set \-b p09 \-m haso228 \-u p09user \-d nxsconfig NXSConfigServer\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsetup set\en       nxsetup set \-b p09 \-m haso228 \-u p09user \-d nxsconfig NXSConfigServer\en       nxsetup set NexusWriter/haso228  \-k NexusWriter  \-y \e\(aq{\(dqp00/bliss_nexuswriter/test_session\(dq:{\(dqsession\(dq:\(dqtest_session\(dq,\(dqbeacon_host\(dq:\(dqhaso228:25000\(dq}}\e\(aq  \-t\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsetup.SetUp
+.B class  nxstools.nxsetup.SetUp
 Bases: \fI\%object\fP
 .sp
 setup NXSDataWriter, NXSConfigServer and NXSRecSelector Tango servers
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B changePropertyName(server, oldname, newname, sclass=None)
 changes property name
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) – server name
+\fBserver\fP (\fI\%str\fP) \-\- server name
 .IP \(bu 2
-\fBoldname\fP (\fI\%str\fP) – old property name
+\fBoldname\fP (\fI\%str\fP) \-\- old property name
 .IP \(bu 2
-\fBnewname\fP (\fI\%str\fP) – new property name
+\fBnewname\fP (\fI\%str\fP) \-\- new property name
 .IP \(bu 2
-\fBsclass\fP (\fI\%str\fP) – server class name
+\fBsclass\fP (\fI\%str\fP) \-\- server class name
 .UNINDENT
 .TP
 .B Returns
 True if property name was changed
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4351,21 +11208,21 @@
 .B changePropertyValue(server, newname, newvalue, sclass=None)
 changes/sets property value
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) – server name
+\fBserver\fP (\fI\%str\fP) \-\- server name
 .IP \(bu 2
-\fBnewvalue\fP (\fI\%str\fP) – new property value
+\fBnewvalue\fP (\fI\%str\fP) \-\- new property value
 .IP \(bu 2
-\fBnewname\fP (\fI\%str\fP) – new property name
+\fBnewname\fP (\fI\%str\fP) \-\- new property name
 .IP \(bu 2
-\fBsclass\fP (\fI\%str\fP) – server class name
+\fBsclass\fP (\fI\%str\fP) \-\- server class name
 .UNINDENT
 .TP
 .B Returns
 True if property name was changed
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4376,175 +11233,224 @@
 .B changeRecorderPath(path, instance=None)
 adds a new recorder path
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBpath\fP (\fI\%str\fP) – new recorder path
+\fBpath\fP (\fI\%str\fP) \-\- new recorder path
 .IP \(bu 2
-\fBinstance\fP (\fI\%str\fP) – MacroServer instance name
+\fBinstance\fP (\fI\%str\fP) \-\- MacroServer instance name
 .UNINDENT
 .TP
 .B Returns
 True if record path was added
 .TP
 .B Return type
 \fI\%bool\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B createConfigServer(beamline, masterhost, jsonsettings=None)
+.B createConfigServer(beamline, masterhost, jsonsettings=None, hostname=None, postpone=False)
 creates configuration server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBbeamline\fP (\fI\%str\fP) – beamline name
+\fBbeamline\fP (\fI\%str\fP) \-\- beamline name
 .IP \(bu 2
-\fBmasterhost\fP (\fI\%str\fP) – master host of data writer
+\fBmasterhost\fP (\fI\%str\fP) \-\- master host of data writer
 .IP \(bu 2
-\fBjsonsettings\fP (\fI\%str\fP) – connection settings to DB in json
+\fBjsonsettings\fP (\fI\%str\fP) \-\- connection settings to DB in json
+.IP \(bu 2
+\fBhostname\fP (\fI\%str\fP) \-\- host to run the config server
+.IP \(bu 2
+\fBpostpone\fP (\fI\%bool\fP) \-\- postpone starting flag
 .UNINDENT
 .TP
 .B Returns
 True if server was created
 .TP
 .B Return type
 \fI\%bool\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B createDataWriter(beamline, masterhost)
+.B createDataWriter(beamline, masterhost, postpone=False)
 creates data writer
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBbeamline\fP (\fI\%str\fP) – beamline name
+\fBbeamline\fP (\fI\%str\fP) \-\- beamline name
+.IP \(bu 2
+\fBmasterhost\fP (\fI\%str\fP) \-\- master host of data writer
 .IP \(bu 2
-\fBmasterhost\fP (\fI\%str\fP) – master host of data writer
+\fBpostpone\fP (\fI\%bool\fP) \-\- postpone starting flag
 .UNINDENT
 .TP
 .B Returns
 True if server was created
 .TP
 .B Return type
 \fI\%bool\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B createSelector(beamline, masterhost, writer=None, cserver=None)
+.B createSelector(beamline, masterhost, writer=None, cserver=None, postpone=False)
 creates selector server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBbeamline\fP (\fI\%str\fP) – beamline name
+\fBbeamline\fP (\fI\%str\fP) \-\- beamline name
+.IP \(bu 2
+\fBmasterhost\fP (\fI\%str\fP) \-\- master host of data writer
+.IP \(bu 2
+\fBwriter\fP (\fI\%str\fP) \-\- writer device name
+.IP \(bu 2
+\fBcserver\fP (\fI\%str\fP) \-\- configuration server device name
+.IP \(bu 2
+\fBpostpone\fP (\fI\%bool\fP) \-\- postpone starting flag
+.UNINDENT
+.TP
+.B Returns
+True if server was created
+.TP
+.B Return type
+\fI\%bool\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B createServer(server_name, beamline, masterhost, hostname=None, class_name=None, jsondeviceproperties=None, postpone=False)
+creates tango server in DB
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBserver_name\fP (\fI\%str\fP) \-\- server name
+.IP \(bu 2
+\fBbeamline\fP (\fI\%str\fP) \-\- beamline name
+.IP \(bu 2
+\fBmasterhost\fP (\fI\%str\fP) \-\- master host of data writer
+.IP \(bu 2
+\fBhostname\fP (\fI\%str\fP) \-\- host to run the config server
 .IP \(bu 2
-\fBmasterhost\fP (\fI\%str\fP) – master host of data writer
+\fBclass_name\fP \-\- class name
 .IP \(bu 2
-\fBwriter\fP (\fI\%str\fP) – writer device name
+\fBjsondeviceproperties\fP (\fI\%str\fP) \-\- json device properties
 .IP \(bu 2
-\fBcserver\fP (\fI\%str\fP) – configuration server device name
+\fBpostpone\fP (\fI\%bool\fP) \-\- postpone starting flag
 .UNINDENT
 .TP
 .B Returns
 True if server was created
 .TP
 .B Return type
 \fI\%bool\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B cserver_name = None
+.B cserver_name
 (\fI\%str\fP) NeXus config server device name
 .UNINDENT
 .INDENT 7.0
 .TP
-.B db = None
-(\fBPyTango.Database\fP) tango database server
+.B db
+(\fI\%tango.Database\fP) tango database server
 .UNINDENT
 .INDENT 7.0
 .TP
 .B getStarterName(host)
 restarts server
 .INDENT 7.0
 .TP
 .B Parameters
-\fBhost\fP (\fI\%str\fP) – server host name
+\fBhost\fP (\fI\%str\fP) \-\- server host name
 .TP
 .B Returns
 starter device name
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B restartServer(name, host=None, level=None, restart=True)
+.B killServer(server)
+.UNINDENT
+.INDENT 7.0
+.TP
+.B restartServer(name, host=None, level=None, restart=True, stopstart=True, wait=True, timeout=None)
 restarts server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) – server name
+\fBname\fP (\fI\%str\fP) \-\- server name
+.IP \(bu 2
+\fBhost\fP (\fI\%str\fP) \-\- server host name
+.IP \(bu 2
+\fBlevel\fP (\fI\%int\fP) \-\- start up level
+.IP \(bu 2
+\fBrestart\fP (\fI\%bool\fP) \-\- if server should be restarted
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) – server host name
+\fBstopstart\fP (\fI\%bool\fP) \-\- if server should be stopped and started
 .IP \(bu 2
-\fBlevel\fP (\fI\%int\fP) – start up level
+\fBwait\fP (\fI\%bool\fP) \-\- script should wait for the server
 .IP \(bu 2
-\fBrestart\fP (\fI\%bool\fP) – if server should be restarted
+\fBtimeout\fP (\fI\%float\fP) \-\- timeout for  start
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B stopServer(name, host=None)
 restarts server
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) – server name
+\fBname\fP (\fI\%str\fP) \-\- server name
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) – server host name
+\fBhost\fP (\fI\%str\fP) \-\- server host name
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B waitServerNotRunning(server=None, device=None, adminproxy=None, maxcnt=1000, verbose=True, waitforproc=True)
 wait until device is exported and server is running
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) – server name, check if running when not None
+\fBserver\fP (\fI\%str\fP) \-\- server name, check if running when not None
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) – device name, check if exported when not None
+\fBdevice\fP (\fI\%str\fP) \-\- device name, check if exported when not None
 .IP \(bu 2
-\fBadminproxy\fP (\fI\%tango.DeviceProxy\fP) – Starter device proxy
+\fBadminproxy\fP (\fI\%tango.DeviceProxy\fP) \-\- Starter device proxy
 .IP \(bu 2
-\fBmaxcnt\fP (\fI\%int\fP) – maximal waiting time in 10ms
+\fBmaxcnt\fP (\fI\%int\fP) \-\- maximal waiting time in 10ms
 .IP \(bu 2
-\fBverbose\fP (\fI\%bool\fP) – verbose mode
+\fBverbose\fP (\fI\%bool\fP) \-\- verbose mode
 .IP \(bu 2
-\fBwaitforproc\fP – wait for process list update
+\fBwaitforproc\fP \-\- wait for process list update
 .UNINDENT
 .TP
 .B Returns
 True if server is running
 .TP
 .B Return type
 \fI\%bool\fP
@@ -4555,747 +11461,960 @@
 .B waitServerRunning(server=None, device=None, adminproxy=None, maxcnt=1000, verbose=True, waitforproc=True)
 wait until device is exported and server is running
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBserver\fP (\fI\%str\fP) – server name, check if running when not None
+\fBserver\fP (\fI\%str\fP) \-\- server name, check if running when not None
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) – device name, check if exported when not None
+\fBdevice\fP (\fI\%str\fP) \-\- device name, check if exported when not None
 .IP \(bu 2
-\fBadminproxy\fP (\fI\%tango.DeviceProxy\fP) – Starter device proxy
+\fBadminproxy\fP (\fI\%tango.DeviceProxy\fP) \-\- Starter device proxy
 .IP \(bu 2
-\fBmaxcnt\fP (\fI\%int\fP) – maximal waiting time in 10ms
+\fBmaxcnt\fP (\fI\%int\fP) \-\- maximal waiting time in 10ms
 .IP \(bu 2
-\fBverbose\fP (\fI\%bool\fP) – verbose mode
+\fBverbose\fP (\fI\%bool\fP) \-\- verbose mode
 .IP \(bu 2
-\fBwaitforproc\fP – wait for process list update
+\fBwaitforproc\fP \-\- wait for process list update
 .UNINDENT
 .TP
 .B Returns
 True if server is running
 .TP
 .B Return type
 \fI\%bool\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B writer_name = None
+.B writer_name
 (\fI\%str\fP) NeXus writer device name
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsetup.Start(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsetup.Start(parser)
+Bases: \fI\%Runner\fP
 .sp
 start runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqstart tango server\(aq
+.B description  =  \(aqstart tango server\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsetup start Pool/haso228 \-l 2\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsetup start Pool/haso228 \-l 2\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsetup.Stop(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsetup.Stop(parser)
+Bases: \fI\%Runner\fP
 .sp
 Stop runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates parser
+.UNINDENT
+.INDENT 7.0
+.TP
+.B description  =  \(aqstop tango server\(aq
+(\fI\%str\fP) command description
+.UNINDENT
+.INDENT 7.0
+.TP
+.B epilog  =  \(aq examples:\en       nxsetup stop Pool/haso228 \en\en\(aq
+(\fI\%str\fP) command epilog
+.UNINDENT
+.INDENT 7.0
+.TP
+.B run(options)
+the main program function
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxsetup.Wait(parser)
+Bases: \fI\%Runner\fP
+.sp
+start runner
+.sp
+parser creator
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqstop tango server\(aq
+.B description  =  \(aqwait for tango server\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsetup stop Pool/haso228 \en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsetup wait Pool/haso228 \-z 30\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxstools.nxsetup.knownHosts = {\(aqcfeld\-pcx27083\(aq: {\(aqbeamline\(aq: \(aqcfeld\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqcfeld\-pcx27083\(aq, \(aquser\(aq: \(aqritzkowf\(aq}, \(aqhas6117b\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhas6117b\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhascmexp\(aq: {\(aqbeamline\(aq: \(aqcmexp\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhascmexp\(aq, \(aquser\(aq: \(aqcmexp\(aq}, \(aqhasdelay\(aq: {\(aqbeamline\(aq: \(aqdelay\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasdelay\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasdelay2\(aq: {\(aqbeamline\(aq: \(aqdelsauto\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasdelay2\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasep211eh\(aq: {\(aqbeamline\(aq: \(aqp211\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep211eh\(aq, \(aquser\(aq: \(aqp211user\(aq}, \(aqhasep212lab\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212lab\(aq, \(aquser\(aq: \(aqp212user\(aq}, \(aqhasep212oh\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212oh\(aq, \(aquser\(aq: \(aqp212user\(aq}, \(aqhasep22ch1\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22ch1\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep22ch2\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22ch2\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep22oh\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22oh\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep23ch\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23ch\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep23dev\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23dev\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep23eh\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23eh\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep24\(aq: {\(aqbeamline\(aq: \(aqp24\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep24\(aq, \(aquser\(aq: \(aqp24user\(aq}, \(aqhasep24eh1\(aq: {\(aqbeamline\(aq: \(aqp24\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep24eh1\(aq, \(aquser\(aq: \(aqp24user\(aq}, \(aqhasfmirr\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfmirr\(aq, \(aquser\(aq: \(aqmusixusr\(aq}, \(aqhasfpgm1\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfpgm1\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhasfvls\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfvls\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhaskmusixtng\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaskmusixtng\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhasmfmc\(aq: {\(aqbeamline\(aq: \(aqfmc\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmfmc\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasmlqj\(aq: {\(aqbeamline\(aq: \(aqlqj\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmlqj\(aq, \(aquser\(aq: \(aqlqjuser\(aq}, \(aqhasmrixs\(aq: {\(aqbeamline\(aq: \(aqrix\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmrixs\(aq, \(aquser\(aq: \(aqrixuser\(aq}, \(aqhasnp61ch1\(aq: {\(aqbeamline\(aq: \(aqp61\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp61ch1\(aq, \(aquser\(aq: \(aqp61user\(aq}, \(aqhasnp64\(aq: {\(aqbeamline\(aq: \(aqp64\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp64\(aq, \(aquser\(aq: \(aqp64user\(aq}, \(aqhasnp64oh\(aq: {\(aqbeamline\(aq: \(aqp64\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp64oh\(aq, \(aquser\(aq: \(aqp64user\(aq}, \(aqhasnp65\(aq: {\(aqbeamline\(aq: \(aqp65\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp65\(aq, \(aquser\(aq: \(aqp65user\(aq}, \(aqhasnp66\(aq: {\(aqbeamline\(aq: \(aqp66\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp66\(aq, \(aquser\(aq: \(aqp66user\(aq}, \(aqhaso107d1\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107d1\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso107klx\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107klx\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso107tk\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107tk\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso111n\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso111n\(aq, \(aquser\(aq: \(aqtnunez\(aq}, \(aqhaso111o\(aq: {\(aqbeamline\(aq: \(aqp09\(aq}, \(aqhaso111tb\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso111tb\(aq, \(aquser\(aq: \(aqtnunez\(aq}, \(aqhaso113b\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso113b\(aq, \(aquser\(aq: \(aqblume\(aq}, \(aqhaso113u\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso113u\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso204n\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso204n\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhaso213p\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso213p\(aq, \(aquser\(aq: \(aqspiec\(aq}, \(aqhaso224w\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso224w\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaso228jk\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso228jk\(aq, \(aquser\(aq: \(aqjkotan\(aq}, \(aqhaso232s\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp232s\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhasodlsauto\(aq: {\(aqbeamline\(aq: \(aqdlsauto\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasodlsauto\(aq, \(aquser\(aq: \(aqdlsuser\(aq}, \(aqhasp029rack\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasp029rack\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhasp068xlab\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasp068xlab\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspecsicl4\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspecsicl4\(aq, \(aquser\(aq: \(aqlacluser\(aq}, \(aqhaspllabcl1\(aq: {\(aqbeamline\(aq: \(aqllab\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspllabcl1\(aq, \(aquser\(aq: \(aqlacluser\(aq}, \(aqhaspp01eh1\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh1\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp01eh2\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh2\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp01eh3\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh3\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp021ch1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021ch1\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp021ch1a\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021ch1a\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp021jenkins\(aq: {\(aqbeamline\(aq: \(aqp021\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021jenkins\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp022ch\(aq: {\(aqbeamline\(aq: \(aqp022\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp022ch\(aq, \(aquser\(aq: \(aqp022user\(aq}, \(aqhaspp02ch1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch1\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02ch1a\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch1a\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02ch2\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch2\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02lakl\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02lakl\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02oh1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02oh1\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp03\(aq: {\(aqbeamline\(aq: \(aqp03\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp03\(aq, \(aquser\(aq: \(aqp03user\(aq}, \(aqhaspp03nano\(aq: {\(aqbeamline\(aq: \(aqp03nano\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp03nano\(aq, \(aquser\(aq: \(aqp03nano\(aq}, \(aqhaspp04exp1\(aq: {\(aqbeamline\(aq: \(aqp04\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp04exp1\(aq, \(aquser\(aq: \(aqp04user\(aq}, \(aqhaspp04exp2\(aq: {\(aqbeamline\(aq: \(aqp04\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp04exp2\(aq, \(aquser\(aq: \(aqp04user\(aq}, \(aqhaspp06ctrl\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06ctrl\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp06mc01\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06mc01\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp06nc1\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06nc1\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp07eh2\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp07eh2\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhaspp08\(aq: {\(aqbeamline\(aq: \(aqp08\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp08\(aq, \(aquser\(aq: \(aqp08user\(aq}, \(aqhaspp08lisa2\(aq: {\(aqbeamline\(aq: \(aqp08\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp08lisa2\(aq, \(aquser\(aq: \(aqp08user\(aq}, \(aqhaspp09\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp09dif\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09dif\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp09haxps\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09maxps\(aq, \(aquser\(aq: \(aqp09haxps\(aq}, \(aqhaspp09mag\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09mag\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp10e1\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10e1\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10e2\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10e2\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10lab\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10lab\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10lcx\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10lcx\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp11oh\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11oh\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp11sardana\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11sardana\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp11user02\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11user02\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp212oh\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212oh\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21eh2\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep21eh2\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21eh3\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep21eh3\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21lab\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp21lab\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhastodt\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhastodt\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhzgpp07eh1\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh1\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhzgpp07eh3\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh3\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhzgpp07eh4\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh4\(aq, \(aquser\(aq: \(aqp07user\(aq}}
+.B nxstools.nxsetup.knownHosts  =  {\(aqcfeld\-pcx27083\(aq: {\(aqbeamline\(aq: \(aqcfeld\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqcfeld\-pcx27083\(aq, \(aquser\(aq: \(aqritzkowf\(aq}, \(aqhas6117b\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhas6117b\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhascmexp\(aq: {\(aqbeamline\(aq: \(aqcmexp\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhascmexp\(aq, \(aquser\(aq: \(aqcmexp\(aq}, \(aqhasdelay\(aq: {\(aqbeamline\(aq: \(aqdelay\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasdelay\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasdelay2\(aq: {\(aqbeamline\(aq: \(aqdelsauto\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasdelay2\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasep211eh\(aq: {\(aqbeamline\(aq: \(aqp211\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep211eh\(aq, \(aquser\(aq: \(aqp211user\(aq}, \(aqhasep212lab\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212lab\(aq, \(aquser\(aq: \(aqp212user\(aq}, \(aqhasep212oh\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212oh\(aq, \(aquser\(aq: \(aqp212user\(aq}, \(aqhasep22ch1\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22ch1\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep22ch2\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22ch2\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep22oh\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep22oh\(aq, \(aquser\(aq: \(aqp22user\(aq}, \(aqhasep23ch\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23ch\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep23dev\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23dev\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep23eh\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep23eh\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhasep24\(aq: {\(aqbeamline\(aq: \(aqp24\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep24\(aq, \(aquser\(aq: \(aqp24user\(aq}, \(aqhasep24eh1\(aq: {\(aqbeamline\(aq: \(aqp24\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep24eh1\(aq, \(aquser\(aq: \(aqp24user\(aq}, \(aqhasfmirr\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfmirr\(aq, \(aquser\(aq: \(aqmusixusr\(aq}, \(aqhasfpgm1\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfpgm1\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhasfvls\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasfvls\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhaskmusixtng\(aq: {\(aqbeamline\(aq: \(aqflash\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaskmusixtng\(aq, \(aquser\(aq: \(aqvuvfuser\(aq}, \(aqhasmfmc\(aq: {\(aqbeamline\(aq: \(aqfmc\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmfmc\(aq, \(aquser\(aq: \(aqdelayusr\(aq}, \(aqhasmlqj\(aq: {\(aqbeamline\(aq: \(aqlqj\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmlqj\(aq, \(aquser\(aq: \(aqlqjuser\(aq}, \(aqhasmrixs\(aq: {\(aqbeamline\(aq: \(aqrix\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasmrixs\(aq, \(aquser\(aq: \(aqrixuser\(aq}, \(aqhasnp61ch1\(aq: {\(aqbeamline\(aq: \(aqp61\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp61ch1\(aq, \(aquser\(aq: \(aqp61user\(aq}, \(aqhasnp64\(aq: {\(aqbeamline\(aq: \(aqp64\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp64\(aq, \(aquser\(aq: \(aqp64user\(aq}, \(aqhasnp64oh\(aq: {\(aqbeamline\(aq: \(aqp64\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp64oh\(aq, \(aquser\(aq: \(aqp64user\(aq}, \(aqhasnp65\(aq: {\(aqbeamline\(aq: \(aqp65\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp65\(aq, \(aquser\(aq: \(aqp65user\(aq}, \(aqhasnp66\(aq: {\(aqbeamline\(aq: \(aqp66\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasnp66\(aq, \(aquser\(aq: \(aqp66user\(aq}, \(aqhaso107d1\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107d1\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso107klx\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107klx\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso107tk\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso107tk\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso111n\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso111n\(aq, \(aquser\(aq: \(aqtnunez\(aq}, \(aqhaso111o\(aq: {\(aqbeamline\(aq: \(aqp09\(aq}, \(aqhaso111tb\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso111tb\(aq, \(aquser\(aq: \(aqtnunez\(aq}, \(aqhaso113b\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso113b\(aq, \(aquser\(aq: \(aqblume\(aq}, \(aqhaso113u\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso113u\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhaso204n\(aq: {\(aqbeamline\(aq: \(aqp23\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso204n\(aq, \(aquser\(aq: \(aqp23user\(aq}, \(aqhaso213p\(aq: {\(aqbeamline\(aq: \(aqp22\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso213p\(aq, \(aquser\(aq: \(aqspiec\(aq}, \(aqhaso224w\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso224w\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaso228jk\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaso228jk\(aq, \(aquser\(aq: \(aqjkotan\(aq}, \(aqhaso232s\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp232s\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhasodlsauto\(aq: {\(aqbeamline\(aq: \(aqdlsauto\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasodlsauto\(aq, \(aquser\(aq: \(aqdlsuser\(aq}, \(aqhasp029rack\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasp029rack\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhasp068xlab\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasp068xlab\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspecsicl4\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspecsicl4\(aq, \(aquser\(aq: \(aqlacluser\(aq}, \(aqhaspllabcl1\(aq: {\(aqbeamline\(aq: \(aqllab\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspllabcl1\(aq, \(aquser\(aq: \(aqlacluser\(aq}, \(aqhaspp01eh1\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh1\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp01eh2\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh2\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp01eh3\(aq: {\(aqbeamline\(aq: \(aqp01\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp01eh3\(aq, \(aquser\(aq: \(aqp01user\(aq}, \(aqhaspp021ch1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021ch1\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp021ch1a\(aq: {\(aqbeamline\(aq: \(aqp021\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021ch1a\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp021jenkins\(aq: {\(aqbeamline\(aq: \(aqp021\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp021jenkins\(aq, \(aquser\(aq: \(aqp021user\(aq}, \(aqhaspp022ch\(aq: {\(aqbeamline\(aq: \(aqp022\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp022ch\(aq, \(aquser\(aq: \(aqp022user\(aq}, \(aqhaspp022chms\(aq: {\(aqbeamline\(aq: \(aqp022\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp022chms\(aq, \(aquser\(aq: \(aqp022user\(aq}, \(aqhaspp02ch1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch1\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02ch1a\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch1a\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02ch2\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02ch2\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02lakl\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02lakl\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp02oh1\(aq: {\(aqbeamline\(aq: \(aqp02\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp02oh1\(aq, \(aquser\(aq: \(aqp02user\(aq}, \(aqhaspp03\(aq: {\(aqbeamline\(aq: \(aqp03\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp03\(aq, \(aquser\(aq: \(aqp03user\(aq}, \(aqhaspp03nano\(aq: {\(aqbeamline\(aq: \(aqp03nano\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp03nano\(aq, \(aquser\(aq: \(aqp03nano\(aq}, \(aqhaspp04exp1\(aq: {\(aqbeamline\(aq: \(aqp04\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp04exp1\(aq, \(aquser\(aq: \(aqp04user\(aq}, \(aqhaspp04exp2\(aq: {\(aqbeamline\(aq: \(aqp04\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp04exp2\(aq, \(aquser\(aq: \(aqp04user\(aq}, \(aqhaspp06ctrl\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06ctrl\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp06mc01\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06mc01\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp06nc1\(aq: {\(aqbeamline\(aq: \(aqp06\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp06nc1\(aq, \(aquser\(aq: \(aqp06user\(aq}, \(aqhaspp07eh2\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp07eh2\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhaspp08\(aq: {\(aqbeamline\(aq: \(aqp08\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp08\(aq, \(aquser\(aq: \(aqp08user\(aq}, \(aqhaspp08lisa2\(aq: {\(aqbeamline\(aq: \(aqp08\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp08lisa2\(aq, \(aquser\(aq: \(aqp08user\(aq}, \(aqhaspp09\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp09dif\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09dif\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp09haxps\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09maxps\(aq, \(aquser\(aq: \(aqp09haxps\(aq}, \(aqhaspp09mag\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp09mag\(aq, \(aquser\(aq: \(aqp09user\(aq}, \(aqhaspp10e1\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10e1\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10e2\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10e2\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10lab\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10lab\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp10lcx\(aq: {\(aqbeamline\(aq: \(aqp10\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp10lcx\(aq, \(aquser\(aq: \(aqp10user\(aq}, \(aqhaspp11oh\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11oh\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp11sardana\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11sardana\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp11user02\(aq: {\(aqbeamline\(aq: \(aqp11\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp11user02\(aq, \(aquser\(aq: \(aqp11user\(aq}, \(aqhaspp212oh\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep212oh\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21eh2\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep21eh2\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21eh3\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhasep21eh3\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhaspp21lab\(aq: {\(aqbeamline\(aq: \(aqp21\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhaspp21lab\(aq, \(aquser\(aq: \(aqp21user\(aq}, \(aqhastodt\(aq: {\(aqbeamline\(aq: \(aqp09\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhastodt\(aq, \(aquser\(aq: \(aqkracht\(aq}, \(aqhzgpp07eh1\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh1\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhzgpp07eh3\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh3\(aq, \(aquser\(aq: \(aqp07user\(aq}, \(aqhzgpp07eh4\(aq: {\(aqbeamline\(aq: \(aqp07\(aq, \(aqdbname\(aq: \(aqnxsconfig\(aq, \(aqmasterhost\(aq: \(aqhzgpp07eh4\(aq, \(aquser\(aq: \(aqp07user\(aq}}
 (\fI\%dict\fP <\fI\%dict\fP <\fI\%str\fP , \fI\%str\fP > > )
 all SardanaHosts and DataBaseHosts should be known
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsetup.main()
 the main program function
 .UNINDENT
-.SS nxstools.nxscreator module
+.SS nxstools.nxsfileinfo module
 .sp
-Command\-line tool for creating to the nexdatas configuration server
+Command\-line tool for showing meta data from Nexus Files
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreator.CPCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.Creator\fP
+.B class  nxstools.nxsfileinfo.Attachment(parser)
+Bases: \fI\%Runner\fP
 .sp
-component creator of all online.xml complex devices
+Attachment runner
 .sp
-constructor
+parser creator
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+.UNINDENT
+.INDENT 7.0
+.TP
+.B attachment(root, options)
+get metadata from nexus and beamtime file
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) – command arguments
+\fBroot\fP (\fBfilewriter.FTGroup\fP) \-\- nexus file root
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
-.UNINDENT
-.INDENT 7.0
 .TP
-.B components = None
-(\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) component xml dictionary
+.B Returns
+atttachment metadata
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
-creates components of all online.xml complex devices
+creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B createXMLs()
-creates component xmls of all online.xml complex devices
-abstract method
+.B description  =  \(aqgenerate description of attachment\(aq
+(\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B datasources = None
-(\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) datasource xml dictionary
+.B epilog  =  \(dq examples:\en       nxsfileinfo attachment \-b p00 \-i 2342342 \-t \(aqHH water\(aq \-o ~/at1.json thumbnail.png \en       nxsfileinfo attachment \-b p00 \-i 2342342 \-t \(aqHH water\(aq \-o ~/at2.json \-s pilatus myscan_00123.nxs \en       nxsfileinfo attachment \-b p00 \-i 2342342 \-t \(aqHH water\(aq \-o ~/at2.json  myscan_00124.fio \en\en\(dq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
-.B xmlpackage = None
-(\fI\%str\fP) xml template component package
+.B postauto()
+parser creator after autocomplete run
 .UNINDENT
 .INDENT 7.0
 .TP
-.B xmltemplatepath = None
-(\fI\%str\fP) xml template component package path
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
+.B run(options)
+the main program function
+.INDENT 7.0
 .TP
-.B exception nxstools.nxscreator.CPExistsException
-Bases: \fI\%Exception\fP
-.sp
-Component already exists exception
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
+.B Returns
+output information
+.TP
+.B Return type
+\fI\%str\fP
 .UNINDENT
-.INDENT 0.0
+.UNINDENT
+.INDENT 7.0
 .TP
-.B class nxstools.nxscreator.ClientDSCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.Creator\fP
-.sp
-client datasource creator
-.sp
-constructor
+.B show(root, options)
+the main function
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+\fBroot\fP (\fBfilewriter.FTGroup\fP) \-\- nexus file root
 .UNINDENT
 .UNINDENT
-.INDENT 7.0
-.TP
-.B create()
-creates a client datasource xml and stores it in DB or filesytem
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreator.CompareOnlineDS(options, args, printouts=True)
+.B class  nxstools.nxsfileinfo.BeamtimeLoader(options)
 Bases: \fI\%object\fP
 .sp
-comparing tool for online.xml files
-.sp
-constructor
+loader constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.UNINDENT
+.INDENT 7.0
+.TP
+.B append_copymap_field(metadata, cmap, clist, cmapfield=None)
+overwrite metadata with dictionary
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
+\fBmetadata\fP (\fI\%dict\fP <\fI\%str\fP, \fIany\fP>) \-\- metadata dictionary to merge in
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
+\fBcmap\fP (\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>) \-\- overwrite dictionary
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+\fBclist\fP (\fI\%list\fP < [\fI\%str\fP, \fI\%str\fP] >) \-\- copy list to overwrite metadata
+.IP \(bu 2
+\fBcmapfield\fP (\fI\%str\fP) \-\- copy map nexus field
+.UNINDENT
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B args = None
-(\fI\%list\fP < \fI\%str\fP >) creator arguments
+.B btmdmap  =  {}
 .UNINDENT
 .INDENT 7.0
 .TP
-.B compare()
+.B copylist  =  [[\(aqcreationTime\(aq, \(aqendTime\(aq]]
 .UNINDENT
 .INDENT 7.0
 .TP
-.B options = None
-(\fBoptparse.Values\fP) creator options
+.B copymap  =  {\(aqdescription\(aq: \(aqscientificMetadata.title.value\(aq, \(aqendTime\(aq: \(aqscientificMetadata.end_time.value\(aq, \(aqscientificMetadata.ScanCommand\(aq: \(aqscientificMetadata.program_name.scan_command\(aq}
 .UNINDENT
+.INDENT 7.0
+.TP
+.B cre  =  {\(aqaccessGroups\(aq: [], \(aqclassification\(aq: [], \(aqcreatedAt\(aq: [], \(aqcreatedBy\(aq: [], \(aqcreationTime\(aq: [], \(aqdataFormat\(aq: [], \(aqdatasetName\(aq: [], \(aqdatasetlifecycle\(aq: [], \(aqhistory\(aq: [], \(aqinstrumentId\(aq: [], \(aqisPublished\(aq: [\(aqfalse\(aq], \(aqkeywords\(aq: [], \(aqlicense\(aq: [], \(aqnumberOfFiles\(aq: [], \(aqnumberOfFilesArchived\(aq: [], \(aqorcidOfOwner\(aq: \(aqORCID of owner https://orcid.org if available\(aq, \(aqownerGroup\(aq: [], \(aqpackedSize\(aq: [], \(aqpublisheddataId\(aq: [], \(aqsampleId\(aq: [], \(aqscientificMetadata\(aq: {}, \(aqsize\(aq: [], \(aqsourceFolderHost\(aq: [], \(aqtechniques\(aq: [], \(aqupdatedAt\(aq: [], \(aqupdatedBy\(aq: [], \(aqvalidationStatus\(aq: [], \(aqversion\(aq: []}
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B class nxstools.nxscreator.ComponentCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.Creator\fP
-.sp
-component creator
-.sp
-constructor
+.B dr  =  {\(aqapplicant.*\(aq: [], \(aqbeamlineAlias\(aq: [], \(aqeventStart\(aq: [], \(aqleader\(aq: [], \(aqonlineAnalysis\(aq: [], \(aqpi.*\(aq: [], \(aqproposalType\(aq: [], \(aqusers\(aq: []}
+.UNINDENT
+.INDENT 7.0
+.TP
+.B facilityalias  =  {\(aqPETRA III\(aq: \(aqpetra3\(aq, \(aqPETRA IV\(aq: \(aqpetra4\(aq}
+.UNINDENT
+.INDENT 7.0
+.TP
+.B generate_techniques(techniques, techniques_pids=None)
+generate technique dictionary
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
+\fBtechniques\fP (\fI\%list\fP <\fI\%str\fP>) \-\- a list of techniques splitted by comma
 .IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
-.IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+\fBtechniques_pids\fP (\fI\%list\fP <\fI\%str\fP>) \-\- a list of technique pids splitted by comma
+.UNINDENT
+.TP
+.B Returns
+technique dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIobjstr\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B create()
-creates a component xml and stores it in DB or filesytem
+.B merge(metadata)
+update metadata with dictionary
+.INDENT 7.0
+.TP
+.B Parameters
+\fBmetadata\fP (\fI\%dict\fP <\fI\%str\fP, \fIany\fP>) \-\- metadata dictionary to merge in
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
 .UNINDENT
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B class nxstools.nxscreator.Creator(options, args, printouts=True)
-Bases: \fI\%object\fP
-.sp
-configuration server adapter
-.sp
-constructor
+.B merge_copy_lists(clist)
+merge copy lists
 .INDENT 7.0
 .TP
 .B Parameters
-.INDENT 7.0
-.IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
-.IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+\fBclist\fP \-\- overwrite copy list
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%list\fP < [\fI\%str\fP, \fI\%str\fP] >
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B args = None
-(\fI\%list\fP < \fI\%str\fP >) creator arguments
-.UNINDENT
+.B merge_copy_maps(cmap)
+merge copy maps
 .INDENT 7.0
 .TP
-.B options = None
-(\fBoptparse.Values\fP) creator options
+.B Parameters
+\fBcmap\fP (\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>) \-\- overwrite dictionary
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
 .UNINDENT
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B exception nxstools.nxscreator.DSExistsException
-Bases: \fI\%Exception\fP
-.sp
-DataSource already exists exception
+.B newbtmdmap  =  {\(aqcontactEmail\(aq: [\(aqpi.email\(aq, \(aqapplicant.email\(aq], \(aqdescription\(aq: [\(aqtitle\(aq], \(aqendTime\(aq: [\(aqeventEnd\(aq], \(aqowner\(aq: [\(aqleader.lastname\(aq, \(aqapplicant.lastname\(aq], \(aqownerEmail\(aq: [\(aqleader.email\(aq, \(aqapplicant.email\(aq], \(aqprincipalInvestigator\(aq: [\(aqapplicant.email\(aq], \(aqproposalId\(aq: [\(aqbeamtimeId\(aq], \(aqsourceFolder\(aq: [\(aqcorePath\(aq]}
 .UNINDENT
-.INDENT 0.0
-.TP
-.B class nxstools.nxscreator.Device
-Bases: \fI\%object\fP
-.sp
-device from online.xml
 .INDENT 7.0
 .TP
-.B attribute
-(\fI\%str\fP) attribute name
+.B oldbtmdmap  =  {\(aqcreatedAt\(aq: [\(aqgenerated\(aq], \(aqupdatedAt\(aq: [\(aqgenerated\(aq]}
 .UNINDENT
 .INDENT 7.0
 .TP
-.B compare(dv)
-.UNINDENT
+.B overwrite(metadata, cmap=None, clist=None, cmapfield=None)
+overwrite metadata with dictionary
 .INDENT 7.0
 .TP
-.B dtype
-(\fI\%str\fP) device type
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBmetadata\fP (\fI\%dict\fP <\fI\%str\fP, \fIany\fP>) \-\- metadata dictionary to merge in
+.IP \(bu 2
+\fBcmap\fP (\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>) \-\- copy map to overwrite dictionary
+.IP \(bu 2
+\fBclist\fP (\fI\%list\fP < [\fI\%str\fP, \fI\%str\fP] >) \-\- copy list to overwrite metadata
+.IP \(bu 2
+\fBcmapfield\fP (\fI\%str\fP) \-\- copy map nexus field
+.UNINDENT
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
+.UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B findAttribute(tangohost, clientlike=False)
-sets attribute and datasource group of online.xml device
+.B remove_metadata(metadata, cmap=None, clist=None, cmapfield=None)
+.INDENT 7.0
+.TP
+.B remove metadata with dictionary with empty input or output
+in the copy map
+.UNINDENT
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBtangohost\fP (\fI\%str\fP) – tango host
+\fBmetadata\fP (\fI\%dict\fP <\fI\%str\fP, \fIany\fP>) \-\- metadata dictionary to merge in
 .IP \(bu 2
-\fBclientlike\fP (\fI\%bool\fP) – tango motors to be client like
+\fBcmap\fP (\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>) \-\- overwrite dictionary
+.IP \(bu 2
+\fBclist\fP (\fI\%list\fP < [\fI\%str\fP, \fI\%str\fP] >) \-\- copy list to overwrite metadata
+.IP \(bu 2
+\fBcmapfield\fP (\fI\%str\fP) \-\- copy map nexus field
 .UNINDENT
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B findDevice(tangohost)
-sets sardana device name and sardana host/port of online.xml device
+.B run()
+runner for DESY beamtime file parser
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtangohost\fP (\fI\%str\fP) – tango host
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B group
-(\fI\%str\fP) datasource tango group
+.B strcre  =  {\(aqaccessGroups\(aq: [\(aq{beamtimeId}\-dmgt\(aq, \(aq{beamtimeId}\-clbt\(aq, \(aq{beamtimeId}\-part\(aq, \(aq{beamline}dmgt\(aq, \(aq{beamline}staff\(aq], \(aqcreationLocation\(aq: \(aq/DESY/{facility}/{beamlineAlias}\(aq, \(aqinstrumentId\(aq: \(aq/{facility}/{beamline}\(aq, \(aqisPublished\(aq: False, \(aqkeywords\(aq: [\(aqscan\(aq], \(aqownerGroup\(aq: \(aq{beamtimeId}\-dmgt\(aq, \(aqtype\(aq: \(aqraw\(aq}
 .UNINDENT
 .INDENT 7.0
 .TP
-.B host
-(\fI\%str\fP) host without port
-.UNINDENT
+.B update_instrumentid(metadata)
+update instrument id
 .INDENT 7.0
 .TP
-.B hostname
-(\fI\%str\fP) host name with port
+.B Parameters
+\fBmetadata\fP (\fI\%dict\fP <\fI\%str\fP, \fIany\fP>) \-\- metadata dictionary to merge in
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
+.UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B module
-(\fI\%str\fP) device module
-.UNINDENT
+.B update_pid(metadata, filename=None, puuid=False, pfname=False, beamtimeid=None)
+update pid metadata with dictionary
 .INDENT 7.0
 .TP
-.B name
-(\fI\%str\fP) device name
-.UNINDENT
+.B Parameters
 .INDENT 7.0
+.IP \(bu 2
+\fBmetadata\fP (\fI\%dict\fP <\fI\%str\fP, \fIany\fP>) \-\- metadata dictionary to merge in
+.IP \(bu 2
+\fBfilename\fP (\fI\%str\fP) \-\- nexus filename
+.IP \(bu 2
+\fBpuuid\fP (\fI\%bool\fP) \-\- pid with uuid
+.IP \(bu 2
+\fBpfname\fP (\fI\%bool\fP) \-\- pid with file name
+.UNINDENT
 .TP
-.B port
-(\fI\%str\fP) port
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
+.UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B sardanahostname
-(\fI\%str\fP) sardana host name
-.UNINDENT
+.B update_sampleid(metadata, sampleid=None, sidfromname=False)
+update sampleid
 .INDENT 7.0
 .TP
-.B sardananame
-(\fI\%str\fP) sardana name with port
-.UNINDENT
+.B Parameters
 .INDENT 7.0
+.IP \(bu 2
+\fBmetadata\fP (\fI\%dict\fP <\fI\%str\fP, \fIany\fP>) \-\- metadata dictionary to merge in
+.IP \(bu 2
+\fBsampleid\fP (\fI\%str\fP) \-\- sample id
+.IP \(bu 2
+\fBsidfromname\fP (\fI\%bool\fP) \-\- sample id from its name
+.UNINDENT
 .TP
-.B sdevice
-(\fI\%str\fP) sardana device name
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
+.UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B setSardanaName(tolower)
-sets sardana name
+.B update_techniques(metadata, techniques=None)
+update techniques
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtolower\fP (\fI\%bool\fP) – If True name in lowercase
+.INDENT 7.0
+.IP \(bu 2
+\fBmetadata\fP (\fI\%dict\fP <\fI\%str\fP, \fIany\fP>) \-\- metadata dictionary to merge in
+.IP \(bu 2
+\fBtechniques\fP (\fI\%str\fP) \-\- a list of techniques splitted by comma
+.UNINDENT
+.TP
+.B Returns
+metadata dictionary
+.TP
+.B Return type
+\fI\%dict\fP <\fI\%str\fP, \fIany\fP>
 .UNINDENT
 .UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxsfileinfo.Field(parser)
+Bases: \fI\%Runner\fP
+.sp
+Field runner
+.sp
+parser creator
 .INDENT 7.0
 .TP
-.B shost
-(\fI\%str\fP) sardana host without port
+.B Parameters
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B splitHostPort()
-spilts host name from port
+.B create()
+creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B sport
-(\fI\%str\fP) sardana tango port
+.B description  =  \(aqshow field information for the nexus file\(aq
+(\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B tdevice
-(\fI\%str\fP) tango device name
+.B epilog  =  \(aq examples:\en       nxsfileinfo field /user/data/myfile.nxs\en       nxsfileinfo field /user/data/myfile.nxs \-g\en       nxsfileinfo field /user/data/myfile.nxs \-s\en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
-.B thost
-(\fI\%str\fP) tango host without port
+.B postauto()
+parser creator after autocomplete run
 .UNINDENT
 .INDENT 7.0
 .TP
-.B tolower()
-converts \fIname\fP, \fImodule\fP, \fItdevice\fP, \fIhostname\fP into lower case
-.UNINDENT
+.B run(options)
+the main program function
 .INDENT 7.0
 .TP
-.B tport
-(\fI\%str\fP) tango port
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
+.B Returns
+output information
+.TP
+.B Return type
+\fI\%str\fP
 .UNINDENT
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B class nxstools.nxscreator.DeviceDSCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.Creator\fP
-.sp
-device datasource creator
-.sp
-constructor
+.B show(root, options)
+the main function
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+\fBroot\fP (class:\fIfilewriter.FTGroup\fP) \-\- nexus file root
 .UNINDENT
 .UNINDENT
-.INDENT 7.0
-.TP
-.B create()
-creates a tango datasources xml of given device
-and stores it in DB or filesytem
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreator.OnlineCPCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.CPCreator\fP
+.B class  nxstools.nxsfileinfo.General(parser)
+Bases: \fI\%Runner\fP
 .sp
-component creator of online components
+General runner
 .sp
-constructor
+parser creator
 .INDENT 7.0
 .TP
 .B Parameters
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+.UNINDENT
 .INDENT 7.0
-.IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
-.IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+.TP
+.B create()
+creates parser
 .UNINDENT
+.INDENT 7.0
+.TP
+.B description  =  \(aqshow general information for the nexus file\(aq
+(\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B createXMLs()
-creates component xmls of all online.xml complex devices
+.B epilog  =  \(aq examples:\en       nxsfileinfo general /user/data/myfile.nxs\en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
-.B listcomponents()
-provides a list of components with xml templates
+.B classmethod  parseentry(entry, description)
+parse entry of nexus file
 .INDENT 7.0
 .TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBentry\fP (\fBfilewriter.FTGroup\fP) \-\- nexus entry node
+.IP \(bu 2
+\fBdescription\fP (\fI\%list\fP <\fI\%dict\fP <\fI\%str\fP, \fIany\fP > >) \-\- dict description list
+.UNINDENT
+.TP
 .B Returns
-list of components with xml templates
+(key, value) name pair of table headers
 .TP
 .B Return type
-\fI\%list\fP <\fI\%str\fP >
+[\fI\%str\fP, \fI\%str\fP]
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B listcomponenttypes()
-provides a list of standard component types
+.B postauto()
+parser creator after autocomplete run
+.UNINDENT
+.INDENT 7.0
+.TP
+.B run(options)
+the main program function
 .INDENT 7.0
 .TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
 .B Returns
-list of standard component types
+output information
 .TP
 .B Return type
-\fI\%list\fP <\fI\%str\fP>
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B show(root)
+show general informations
+.INDENT 7.0
+.TP
+.B Parameters
+\fBroot\fP (class:\fIfilewriter.FTGroup\fP) \-\- nexus file root
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreator.OnlineDSCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.Creator\fP
+.B class  nxstools.nxsfileinfo.GroupMetadata(parser)
+Bases: \fI\%Runner\fP
 .sp
-datasource creator of all online.xml simple devices
+Group Metadata runner
 .sp
-constructor
+parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-.INDENT 7.0
-.IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) – command arguments
-.IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
-.UNINDENT
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
-creates datasources of all online.xml simple devices
+creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B createXMLs()
-creates datasource xmls of all online.xml simple devices
+.B description  =  \(aqgroup scan metadata information\(aq
+(\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B datasources = None
-(\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) datasource xml dictionary
+.B dicttype  =  [\(aqDict\(aq, \(aqD\(aq, \(aqd\(aq, \(aqdict\(aq]
 .UNINDENT
 .INDENT 7.0
 .TP
-.B xmlpackage = None
-(\fI\%str\fP) xml template component package
+.B endpointstype  =  [\(aqEndpoints\(aq, \(aqendpoints\(aq, \(aqE\(aq, \(aqe\(aq]
 .UNINDENT
 .INDENT 7.0
 .TP
-.B xmltemplatepath = None
-(\fI\%str\fP) xml template component package path
+.B epilog  =  \(aq examples:\en       nxsfileinfo groupmetadata \-o /user/data/myscan.scan.json  \-t /user/data/myscan.attachment.json  \-l /user/data/myscan.origdatablock.json  \-c /home/user/group_config.txt  \-m /user/data/myscan_00023.scan.json  \-d /user/data/myscan_00023.origdatablock.json  \-a /user/data/myscan_00023.attachment.json \en \en       nxsfileinfo groupmetadata myscan_m001  \-m /user/data/myscan_00021.scan.json\en  \-c /home/user/group_config.txt  \en \en       nxsfileinfo groupmetadata  myscan_m001  \-c /home/user/group_config.txt  \-m /user/data/myscan_00023.scan.json  \-d /user/data/myscan_00023.origdatablock.json  \-a /user/data/myscan_00023.attachment.json  \en \en       nxsfileinfo groupmetadata  \-m /user/data/myscan_00023.scan.json  \-d /user/data/myscan_00023.origdatablock.json  \-c /home/user/group_config.txt  \en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
+.INDENT 7.0
+.TP
+.B firstlasttype  =  [\(aqFirstLast\(aq, \(aqfirstlast\(aq]
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B nxstools.nxscreator.PYTANGO = True
-(\fI\%bool\fP) True if PyTango available
+.B firsttype  =  [\(aqFirst\(aq, \(aqfirst\(aq, \(aqf\(aq, \(aqF\(aq]
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B class nxstools.nxscreator.PoolDSCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.Creator\fP
-.sp
-datasource creator of all sardana pool acquisition channels
-.sp
-constructor
+.B classmethod  groupmetadata(options)
+group scan metadata
 .INDENT 7.0
 .TP
 .B Parameters
-.INDENT 7.0
-.IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP <\fI\%str\fP >) – command arguments
-.IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
+.B Returns
+[grouped metadata,
+grouped origdatablocks,
+grouped attachments]
+.TP
+.B Return type
+[\fI\%str\fP,:obj:\fIstr\fP, \fI\%str\fP]
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B create()
-creates datasources of all online.xml simple devices
+.B lasttype  =  [\(aqLast\(aq, \(aqlast\(aq, \(aql\(aq, \(aqL\(aq]
 .UNINDENT
 .INDENT 7.0
 .TP
-.B createXMLs()
-creates datasource xmls of all online.xml simple devices
+.B listtype  =  [\(aqList\(aq, \(aqL\(aq, \(aql\(aq, \(aqlist\(aq]
 .UNINDENT
 .INDENT 7.0
 .TP
-.B datasources = None
-(\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP >) datasource xml dictionary
+.B maxtype  =  [\(aqMax\(aq, \(aqmax\(aq]
 .UNINDENT
-.UNINDENT
-.INDENT 0.0
-.TP
-.B class nxstools.nxscreator.StandardCPCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.CPCreator\fP
-.sp
-component creator of standard templates
-.sp
-constructor
 .INDENT 7.0
 .TP
-.B Parameters
+.B minmaxtype  =  [\(aqMinMax\(aq, \(aqM\(aq, \(aqm\(aq, \(aqminmax\(aq]
+.UNINDENT
 .INDENT 7.0
-.IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
-.IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+.TP
+.B mintype  =  [\(aqMin\(aq, \(aqmin\(aq]
 .UNINDENT
+.INDENT 7.0
+.TP
+.B postauto()
+parser creator after autocomplete run
 .UNINDENT
 .INDENT 7.0
 .TP
-.B createXMLs()
-creates component xmls of all online.xml complex devices
+.B rangetype  =  [\(aqRange\(aq, \(aqR\(aq, \(aqr\(aq, \(aqrangle\(aq]
 .UNINDENT
 .INDENT 7.0
 .TP
-.B listcomponenttypes()
-provides a list of standard component types
+.B run(options)
+the main program function
 .INDENT 7.0
 .TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
 .B Returns
-list of standard component types
+output information
 .TP
 .B Return type
-\fI\%list\fP <\fI\%str\fP>
+\fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B listcomponentvariables()
-provides a list of standard component types
+.B show(options)
+the main function
 .INDENT 7.0
 .TP
-.B Returns
-list of standard component types
-.TP
-.B Return type
-\fI\%list\fP <\fI\%str\fP>
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .UNINDENT
 .UNINDENT
+.INDENT 7.0
+.TP
+.B uniquelisttype  =  [\(aqUniqueList\(aq, \(aqU\(aq, \(aqu\(aq, \(aquniquelist\(aq]
+.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxscreator.TangoDSCreator(options, args, printouts=True)
-Bases: \fI\%nxstools.nxscreator.Creator\fP
+.B class  nxstools.nxsfileinfo.Instrument(parser)
+Bases: \fI\%Runner\fP
 .sp
-tango datasource creator
+Instrument runner
 .sp
-constructor
+parser creator
 .INDENT 7.0
 .TP
 .B Parameters
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+.UNINDENT
 .INDENT 7.0
-.IP \(bu 2
-\fBoptions\fP (\fBoptparse.Values\fP) – command options
-.IP \(bu 2
-\fBargs\fP (\fI\%list\fP < \fI\%str\fP >) – command arguments
-.IP \(bu 2
-\fBprintouts\fP (\fI\%bool\fP) – if printout is enable
+.TP
+.B create()
+creates parser
 .UNINDENT
+.INDENT 7.0
+.TP
+.B description  =  \(aqgenerate description of instrument\(aq
+(\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B create()
-creates a tango datasource xml and stores it in DB or filesytem
+.B epilog  =  \(aq examples:\en       nxsfileinfo instrument \-p /petra3/p00 \-n P00 \-m ~/cm.json \en\en\(aq
+(\fI\%str\fP) command epilog
 .UNINDENT
+.INDENT 7.0
+.TP
+.B instrument(options)
+create instrument metadata
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
+.B Returns
+output information
+.TP
+.B Return type
+\fI\%str\fP
 .UNINDENT
-.INDENT 0.0
+.UNINDENT
+.INDENT 7.0
 .TP
-.B exception nxstools.nxscreator.WrongParameterError
-Bases: \fI\%Exception\fP
-.sp
-wrong parameter exception
+.B postauto()
+parser creator after autocomplete run
+.UNINDENT
+.INDENT 7.0
+.TP
+.B run(options)
+the main program function
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
+.B Returns
+output information
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B show(options)
+the main function
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.UNINDENT
+.UNINDENT
 .UNINDENT
-.SS nxstools.nxsfileinfo module
-.sp
-Command\-line tool for showing meta data from Nexus Files
 .INDENT 0.0
 .TP
-.B class nxstools.nxsfileinfo.Field(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsfileinfo.Metadata(parser)
+Bases: \fI\%Runner\fP
 .sp
-Field runner
+Metadata runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqshow field information for the nexus file\(aq
+.B description  =  \(aqshow metadata information for the nexus file\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsfileinfo field /user/data/myfile.nxs\en       nxsfileinfo field /user/data/myfile.nxs \-g\en       nxsfileinfo field /user/data/myfile.nxs \-s\en\en\(aq
+.B epilog  =  \(dq examples:\en       nxsfileinfo metadata /user/data/myfile.nxs\en       nxsfileinfo metadata /user/data/myfile.fio\en       nxsfileinfo metadata /user/data/myfile.nxs \-p \(aqGroup\(aq\en       nxsfileinfo metadata /user/data/myfile.nxs \-s\en       nxsfileinfo metadata /user/data/myfile.nxs \-a units,NX_class\en\en\(dq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
+.B classmethod  metadata(root, options)
+get metadata from nexus and beamtime file
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBroot\fP (\fBfilewriter.FTGroup\fP) \-\- nexus file root
+.IP \(bu 2
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.UNINDENT
+.TP
+.B Returns
+nexus file root metadata
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
 .B postauto()
 parser creator after autocomplete run
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
@@ -5305,438 +12424,662 @@
 .B show(root, options)
 the main function
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .IP \(bu 2
-\fBroot\fP (class:\fIfilewriter.FTGroup\fP) – nexus file root
+\fBroot\fP (\fBfilewriter.FTGroup\fP) \-\- nexus file root
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsfileinfo.General(parser)
-Bases: \fI\%nxstools.nxsargparser.Runner\fP
+.B class  nxstools.nxsfileinfo.OrigDatablock(parser)
+Bases: \fI\%Runner\fP
 .sp
-General runner
+OrigDatablock runner
 .sp
 parser creator
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
 .UNINDENT
 .INDENT 7.0
 .TP
 .B create()
 creates parser
 .UNINDENT
 .INDENT 7.0
 .TP
-.B description = \(aqshow general information for the nexus file\(aq
+.B datablock(options)
+dump scan datablock JSON
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
+.B Returns
+output information
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B datafiles(scanpath, scdir, scfiles, relpath, filters=None)
+.UNINDENT
+.INDENT 7.0
+.TP
+.B description  =  \(aqgenerate description of all scan files\(aq
 (\fI\%str\fP) command description
 .UNINDENT
 .INDENT 7.0
 .TP
-.B epilog = \(aq examples:\en       nxsfileinfo general /user/data/myfile.nxs\en\en\(aq
+.B epilog  =  \(aq examples:\en       nxsfileinfo origdatablock /user/data/scan_12345\en\en\(aq
 (\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod parseentry(entry, description)
-parse entry of nexus file
+.B filterout(fpath, filters)
+.UNINDENT
 .INDENT 7.0
 .TP
-.B Parameters
+.B isotime(tme)
+returns iso time string
 .INDENT 7.0
-.IP \(bu 2
-\fBentry\fP (\fBfilewriter.FTGroup\fP) – nexus entry node
-.IP \(bu 2
-\fBdescription\fP (\fI\%list\fP <\fI\%dict\fP <\fI\%str\fP, \fIany\fP > >) – dict description list
+.TP
+.B Returns
+iso time
+.TP
+.B Return type
+\fI\%str\fP
 .UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B postauto()
+parser creator after autocomplete run
+.UNINDENT
+.INDENT 7.0
+.TP
+.B run(options)
+the main program function
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
-(key, value) name pair of table headers
+output information
 .TP
 .B Return type
-[\fI\%str\fP, \fI\%str\fP]
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B show(options)
+the main function
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxsfileinfo.Sample(parser)
+Bases: \fI\%Runner\fP
+.sp
+Sample runner
+.sp
+parser creator
+.INDENT 7.0
+.TP
+.B Parameters
+\fBparser\fP (\fBNXSFileInfoArgParser\fP) \-\- option parser
+.UNINDENT
+.INDENT 7.0
+.TP
+.B create()
+creates parser
 .UNINDENT
+.INDENT 7.0
+.TP
+.B description  =  \(aqgenerate description of sample\(aq
+(\fI\%str\fP) command description
+.UNINDENT
+.INDENT 7.0
+.TP
+.B epilog  =  \(dq examples:\en       nxsfileinfo sample \-i petra3/h2o/234234 \-d \(aqHH water\(aq \-s ~/cm.json \en\en\(dq
+(\fI\%str\fP) command epilog
 .UNINDENT
 .INDENT 7.0
 .TP
 .B postauto()
 parser creator after autocomplete run
 .UNINDENT
 .INDENT 7.0
 .TP
 .B run(options)
 the main program function
 .INDENT 7.0
 .TP
 .B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
 .TP
 .B Returns
 output information
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B show(root)
-show general informations
+.B sample(options)
+create sample metadata
 .INDENT 7.0
 .TP
 .B Parameters
-\fBroot\fP (class:\fIfilewriter.FTGroup\fP) – nexus file root
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.TP
+.B Returns
+output information
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
+.INDENT 7.0
+.TP
+.B show(options)
+the main function
+.INDENT 7.0
+.TP
+.B Parameters
+\fBoptions\fP (\fI\%argparse.Namespace\fP) \-\- parser options
+.UNINDENT
 .UNINDENT
 .UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsfileinfo.getlist(text)
+.INDENT 7.0
+.TP
+.B converts a text string to a list of lists
+with respect to newline and space characters
+.UNINDENT
+.INDENT 7.0
+.TP
+.B Parameters
+\fBtext\fP (\fI\%str\fP) \-\- parser options
+.TP
+.B Returns
+a list of list
+.TP
+.B Return type
+\fI\%list\fP < \fBlist\(ga<:obj:\(gastr\fP> >
+.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsfileinfo.main()
 the main program function
 .UNINDENT
+.INDENT 0.0
+.TP
+.B nxstools.nxsfileinfo.splittext(text, lmax=68)
+split text to lines
+.INDENT 7.0
+.TP
+.B Parameters
+.INDENT 7.0
+.IP \(bu 2
+\fBtext\fP (\fI\%str\fP) \-\- parser options
+.IP \(bu 2
+\fBlmax\fP (\fI\%int\fP) \-\- maximal line length
+.UNINDENT
+.TP
+.B Returns
+split text
+.TP
+.B Return type
+\fI\%str\fP
+.UNINDENT
+.UNINDENT
 .SS nxstools.nxsfileparser module
 .sp
 NeXus main metadata viewer
 .INDENT 0.0
 .TP
-.B class nxstools.nxsfileparser.NXSFileParser(root)
+.B class  nxstools.nxsfileparser.FIOFileParser(root)
+Bases: \fI\%object\fP
+.sp
+Metadata parser for FIO files
+.sp
+constructor
+.INDENT 7.0
+.TP
+.B Parameters
+\fBroot\fP (\fI\%str\fP) \-\- fio file content
+.UNINDENT
+.INDENT 7.0
+.TP
+.B columns
+(\fI\%dict\fP <\fI\%str\fP, \fIany\fP>)  columns dictionary
+.UNINDENT
+.INDENT 7.0
+.TP
+.B group_postfix
+(\fI\%str\fP) group postfix
+.UNINDENT
+.INDENT 7.0
+.TP
+.B parseMeta()
+parses the file and creates the filtered description list
+.UNINDENT
+.UNINDENT
+.INDENT 0.0
+.TP
+.B class  nxstools.nxsfileparser.NXSFileParser(root)
 Bases: \fI\%object\fP
 .sp
 Metadata parser for NeXus files
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBroot\fP (\fBfilewriter.FTGroup\fP) – nexus root node
+\fBroot\fP (\fBfilewriter.FTGroup\fP) \-\- nexus root node
+.UNINDENT
+.INDENT 7.0
+.TP
+.B emptyunits
+(\fI\%bool\fP) add empty units
 .UNINDENT
 .INDENT 7.0
 .TP
-.B filters = None
+.B filters
 (\fBlist\(ga< :obj:\(gastr\fP>)  filters for \fIfull_path\fP names
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod getpath(path)
+.B classmethod  getpath(path)
 converts full_path with NX_classes into nexus_path
 .INDENT 7.0
 .TP
 .B Parameters
-\fBpath\fP (\fI\%str\fP) – nexus full_path
+\fBpath\fP (\fI\%str\fP) \-\- nexus full_path
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
+.B group_postfix
+(\fI\%str\fP) group postfix
+.UNINDENT
+.INDENT 7.0
+.TP
 .B parse()
 parses the file and creates the filtered description list
 .UNINDENT
 .INDENT 7.0
 .TP
-.B valuestostore = None
+.B parseMeta()
+parses the file and creates the filtered description list
+.UNINDENT
+.INDENT 7.0
+.TP
+.B scientific
+(\fI\%bool\fP) store NXentries as scientificMetadata
+.UNINDENT
+.INDENT 7.0
+.TP
+.B valuestostore
 (\fBlist\(ga< :obj:\(gastr\fP>)  field names which value should be stored
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsfileparser.getdsname(xmlstring)
 provides datasource name from datasource xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlstring\fP (\fI\%str\fP) – datasource xml string
+\fBxmlstring\fP (\fI\%str\fP) \-\- datasource xml string
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsfileparser.getdssource(xmlstring)
 provides source from datasource xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlstring\fP (\fI\%str\fP) – datasource xml string
+\fBxmlstring\fP (\fI\%str\fP) \-\- datasource xml string
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
 .B nxstools.nxsfileparser.getdstype(xmlstring)
 provides datasource type from datasource xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlstring\fP (\fI\%str\fP) – datasource xml string
+\fBxmlstring\fP (\fI\%str\fP) \-\- datasource xml string
 .UNINDENT
 .UNINDENT
-.SS nxstools.nxsargparser module
-.sp
-NeXus tool argumen parser
 .INDENT 0.0
 .TP
-.B exception nxstools.nxsargparser.ErrorException
-Bases: \fI\%Exception\fP
-.sp
-error parser exception
+.B nxstools.nxsfileparser.infNaN2None(obj)
+replace inf and NaN to None
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsargparser.NXSArgParser(**kwargs)
-Bases: \fI\%argparse.ArgumentParser\fP
-.sp
-Argument parser with error exception
-.sp
-constructor
+.B nxstools.nxsfileparser.isoDate(text)
+convert date to iso format
 .INDENT 7.0
 .TP
 .B Parameters
-\fBkwargs\fP – \fI\%argparse.ArgumentParser\fP
-parameter dictionary
-.UNINDENT
-.INDENT 7.0
-.TP
-.B createSubParsers()
-creates command\-line parameters parser
-.INDENT 7.0
+\fBtext\fP (\fI\%str\fP) \-\- date text to convert
 .TP
 .B Returns
-command runner
+date in iso format
 .TP
 .B Return type
-\fI\%Runner\fP
-.UNINDENT
-.UNINDENT
-.INDENT 7.0
-.TP
-.B error(message)
-error handler
-.INDENT 7.0
-.TP
-.B Parameters
-\fBmessage\fP (\fI\%str\fP) – error message
-.UNINDENT
+\fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsargparser.Runner(parser)
-Bases: \fI\%object\fP
+.B class  nxstools.nxsfileparser.numpyEncoder(*, skipkeys=False, ensure_ascii=True, check_circular=True, allow_nan=True, sort_keys=False, indent=None, separators=None, default=None)
+Bases: \fBJSONEncoder\fP
 .sp
-abstract runner
+numpy json encoder with list
 .sp
-parser creator
-.INDENT 7.0
-.TP
-.B Parameters
-\fBparser\fP (\fBNXSFileInfoArgParser\fP) – option parser
-.UNINDENT
+Constructor for JSONEncoder, with sensible defaults.
+.sp
+If skipkeys is false, then it is a TypeError to attempt
+encoding of keys that are not str, int, float or None.  If
+skipkeys is True, such items are simply skipped.
+.sp
+If ensure_ascii is true, the output is guaranteed to be str
+objects with all incoming non\-ASCII characters escaped.  If
+ensure_ascii is false, the output can contain non\-ASCII characters.
+.sp
+If check_circular is true, then lists, dicts, and custom encoded
+objects will be checked for circular references during encoding to
+prevent an infinite recursion (which would cause an RecursionError).
+Otherwise, no such check takes place.
+.sp
+If allow_nan is true, then NaN, Infinity, and \-Infinity will be
+encoded as such.  This behavior is not JSON specification compliant,
+but is consistent with most JavaScript based encoders and decoders.
+Otherwise, it will be a ValueError to encode such floats.
+.sp
+If sort_keys is true, then the output of dictionaries will be
+sorted by key; this is useful for regression tests to ensure
+that JSON serializations can be compared on a day\-to\-day basis.
+.sp
+If indent is a non\-negative integer, then JSON array
+elements and object members will be pretty\-printed with that
+indent level.  An indent level of 0 will only insert newlines.
+None is the most compact representation.
+.sp
+If specified, separators should be an (item_separator, key_separator)
+tuple.  The default is (\(aq, \(aq, \(aq: \(aq) if \fIindent\fP is \fBNone\fP and
+(\(aq,\(aq, \(aq: \(aq) otherwise.  To get the most compact JSON representation,
+you should specify (\(aq,\(aq, \(aq:\(aq) to eliminate whitespace.
+.sp
+If specified, default is a function that gets called for objects
+that can\(aqt otherwise be serialized.  It should return a JSON encodable
+version of the object or raise a \fBTypeError\fP\&.
 .INDENT 7.0
 .TP
-.B create()
-parser creator
-.UNINDENT
+.B default(obj)
+default encoder
 .INDENT 7.0
 .TP
-.B description = \(aqabstract runner\(aq
-(\fI\%str\fP) command description
+.B Parameters
+\fBobj\fP (\fI\%object\fP or \fIany\fP) \-\- numpy array object
 .UNINDENT
-.INDENT 7.0
-.TP
-.B epilog = None
-(\fI\%str\fP) command epilog
 .UNINDENT
-.INDENT 7.0
-.TP
-.B postauto()
-parser creator after autocomplete run
 .UNINDENT
-.INDENT 7.0
+.INDENT 0.0
 .TP
-.B run(options)
-run commandthe main program function
+.B class  nxstools.nxsfileparser.numpyEncoderNull(*, skipkeys=False, ensure_ascii=True, check_circular=True, allow_nan=True, sort_keys=False, indent=None, separators=None, default=None)
+Bases: \fI\%numpyEncoder\fP
+.sp
+numpy json encoder with list with nan/inf to null
+.sp
+Constructor for JSONEncoder, with sensible defaults.
+.sp
+If skipkeys is false, then it is a TypeError to attempt
+encoding of keys that are not str, int, float or None.  If
+skipkeys is True, such items are simply skipped.
+.sp
+If ensure_ascii is true, the output is guaranteed to be str
+objects with all incoming non\-ASCII characters escaped.  If
+ensure_ascii is false, the output can contain non\-ASCII characters.
+.sp
+If check_circular is true, then lists, dicts, and custom encoded
+objects will be checked for circular references during encoding to
+prevent an infinite recursion (which would cause an RecursionError).
+Otherwise, no such check takes place.
+.sp
+If allow_nan is true, then NaN, Infinity, and \-Infinity will be
+encoded as such.  This behavior is not JSON specification compliant,
+but is consistent with most JavaScript based encoders and decoders.
+Otherwise, it will be a ValueError to encode such floats.
+.sp
+If sort_keys is true, then the output of dictionaries will be
+sorted by key; this is useful for regression tests to ensure
+that JSON serializations can be compared on a day\-to\-day basis.
+.sp
+If indent is a non\-negative integer, then JSON array
+elements and object members will be pretty\-printed with that
+indent level.  An indent level of 0 will only insert newlines.
+None is the most compact representation.
+.sp
+If specified, separators should be an (item_separator, key_separator)
+tuple.  The default is (\(aq, \(aq, \(aq: \(aq) if \fIindent\fP is \fBNone\fP and
+(\(aq,\(aq, \(aq: \(aq) otherwise.  To get the most compact JSON representation,
+you should specify (\(aq,\(aq, \(aq:\(aq) to eliminate whitespace.
+.sp
+If specified, default is a function that gets called for objects
+that can\(aqt otherwise be serialized.  It should return a JSON encodable
+version of the object or raise a \fBTypeError\fP\&.
 .INDENT 7.0
 .TP
-.B Parameters
-\fBoptions\fP (\fI\%argparse.Namespace\fP) – parser options
-.UNINDENT
+.B encode(obj, *args, **kwargs)
+Return a JSON string representation of a Python data structure.
+.sp
+.nf
+.ft C
+>>> from json.encoder import JSONEncoder
+>>> JSONEncoder().encode({\(dqfoo\(dq: [\(dqbar\(dq, \(dqbaz\(dq]})
+\(aq{\(dqfoo\(dq: [\(dqbar\(dq, \(dqbaz\(dq]}\(aq
+.ft P
+.fi
 .UNINDENT
 .UNINDENT
 .SS nxstools.nxsparser module
 .sp
 Command\-line tool for ascess to the nexdatas configuration server
 .INDENT 0.0
 .TP
-.B class nxstools.nxsparser.ESRFConverter
+.B class  nxstools.nxsparser.ESRFConverter
 Bases: \fI\%object\fP
 .sp
 ESRF xml configuration converter
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B convert(text)
 converts ESRF xml configuration to nxsdatawriter format
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtext\fP (\fI\%str\fP) – input xml string
+\fBtext\fP (\fI\%str\fP) \-\- input xml string
 .TP
 .B Returns
 output xml string
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsparser.ParserTools
+.B class  nxstools.nxsparser.ParserTools
 Bases: \fI\%object\fP
 .sp
 configuration server adapter
 .INDENT 7.0
 .TP
-.B classmethod getRecord(node)
+.B classmethod  getRecord(node)
 fetches record name or query from datasource node
 .INDENT 7.0
 .TP
 .B Parameters
-\fBnode\fP (\fBlxml.etree.Element\fP) – datasource node
+\fBnode\fP (\fBlxml.etree.Element\fP) \-\- datasource node
 .TP
 .B Returns
 record name or query
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod mergeDefinitions(xmls)
+.B classmethod  mergeDefinitions(xmls)
 .INDENT 7.0
 .TP
 .B merges the xmls list of definitions xml strings
 to one output xml string
 .UNINDENT
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmls\fP (\fI\%list\fP <\fI\%str\fP>) – a list of xml string with definitions
+\fBxmls\fP (\fI\%list\fP <\fI\%str\fP>) \-\- a list of xml string with definitions
 .TP
 .B Returns
 one output xml string
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod parseAttributes(xmlc)
+.B classmethod  parseAttributes(xmlc)
 provides datasources and its records from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) – xml string
+\fBxmlc\fP (\fI\%str\fP) \-\- xml string
 .TP
 .B Returns
 list of datasource descriptions
 .TP
 .B Return type
 \fI\%list\fP < \fI\%dict\fP <\fI\%str\fP, \fIany\fP> >
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod parseDataSources(xmlc)
+.B classmethod  parseDataSources(xmlc)
 provides datasources and its records from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) – xml string
+\fBxmlc\fP (\fI\%str\fP) \-\- xml string
 .TP
 .B Returns
 list of datasource descriptions
 .TP
 .B Return type
 \fI\%list\fP <\fI\%dict\fP <\fI\%str\fP, \fI\%str\fP>>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod parseFields(xmlc)
+.B classmethod  parseFields(xmlc)
 provides datasources and its records from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) – xml string
+\fBxmlc\fP (\fI\%str\fP) \-\- xml string
 .TP
 .B Returns
 list of datasource descriptions
 .TP
 .B Return type
 \fI\%list\fP < \fI\%dict\fP <\fI\%str\fP, \fIany\fP> >
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod parseLinks(xmlc)
+.B classmethod  parseLinks(xmlc)
 provides datasources and its records from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) – xml string
+\fBxmlc\fP (\fI\%str\fP) \-\- xml string
 .TP
 .B Returns
 list of datasource descriptions
 .TP
 .B Return type
 \fI\%list\fP < \fI\%dict\fP <\fI\%str\fP, \fIany\fP> >
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B classmethod parseRecord(xmlc)
+.B classmethod  parseRecord(xmlc)
 provides source record from xml string
 .INDENT 7.0
 .TP
 .B Parameters
-\fBxmlc\fP (\fI\%str\fP) – xml string
+\fBxmlc\fP (\fI\%str\fP) \-\- xml string
 .TP
 .B Returns
 source record
 .TP
 .B Return type
 \fI\%str\fP
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsparser.TableDictTools(description, nonone=None)
+.B class  nxstools.nxsparser.TableDictTools(description, nonone=None)
 Bases: \fI\%object\fP
 .sp
 configuration server adapter
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) – description list
+\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) \-\- description list
 .IP \(bu 2
-\fBnonone\fP (\fI\%list\fP <\fI\%str\fP>) – list of parameters which have to exist to be shown
+\fBnonone\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of parameters which have to exist to be shown
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B generateList()
 generate row lists of table
 .INDENT 7.0
@@ -5746,49 +13089,49 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B headers = None
+.B headers
 (\fI\%list\fP <\fI\%str\fP>)
 headers
 .UNINDENT
 .INDENT 7.0
 .TP
-.B title = None
+.B title
 (\fI\%str\fP) table title
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsparser.TableTools(description, nonone=None, headers=None, filters=None)
+.B class  nxstools.nxsparser.TableTools(description, nonone=None, headers=None, filters=None)
 Bases: \fI\%object\fP
 .sp
 configuration server adapter
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) – description list
+\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) \-\- description list
 .IP \(bu 2
-\fBnonone\fP (\fI\%list\fP <\fI\%str\fP>) – list of parameters which have to exist to be shown
+\fBnonone\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of parameters which have to exist to be shown
 .IP \(bu 2
-\fBheaders\fP (\fI\%list\fP <\fI\%str\fP>) – list of output parameters
+\fBheaders\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of output parameters
 .IP \(bu 2
-\fBfilters\fP (\fI\%list\fP <\fI\%str\fP>) – filters for first column names
+\fBfilters\fP (\fI\%list\fP <\fI\%str\fP>) \-\- filters for first column names
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B filters = None
+.B filters
 (\fI\%list\fP <\fI\%str\fP>) filter list
 .UNINDENT
 .INDENT 7.0
 .TP
 .B generateList()
 generate row lists of table
 .INDENT 7.0
@@ -5798,972 +13141,706 @@
 .TP
 .B Return type
 \fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B headers = None
+.B headers
 (\fI\%list\fP <\fI\%str\fP>) table headers
 .UNINDENT
 .INDENT 7.0
 .TP
 .B loadDescription(description)
 loads description
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) – description list
+\fBdescription\fP (\fI\%list\fP <\fI\%str\fP>) \-\- description list
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B title = None
+.B title
 (\fI\%str\fP) table title
 .UNINDENT
 .UNINDENT
 .SS nxstools.nxsxml module
 .sp
 Creator of XML configuration files
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NAttr(parent, nameAttr, typeAttr=\(aq\(aq)
-Bases: \fI\%nxstools.nxsxml.NTag\fP
+.B class  nxstools.nxsxml.NAttr(parent, nameAttr, typeAttr=\(aq\(aq)
+Bases: \fI\%NTag\fP
 .sp
 Attribute tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) – name attribute
+\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) – type attribute
+\fBtypeAttr\fP (\fI\%str\fP) \-\- type attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setStrategy(mode=\(aqSTEP\(aq, trigger=None, value=None, canfail=None)
 sets the attribute strategy
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBmode\fP (\fI\%str\fP) – mode data writing, i.e. INIT, STEP, FINAL, POSTRUN
+\fBmode\fP (\fI\%str\fP) \-\- mode data writing, i.e. INIT, STEP, FINAL, POSTRUN
 .IP \(bu 2
-\fBtrigger\fP (\fI\%str\fP) – for asynchronous writting,
+\fBtrigger\fP (\fI\%str\fP) \-\- for asynchronous writting,
 e.g. with different subentries
 .IP \(bu 2
-\fBvalue\fP (\fI\%str\fP) – label for postrun mode
+\fBvalue\fP (\fI\%str\fP) \-\- label for postrun mode
 .IP \(bu 2
-\fBcanfail\fP (\fI\%bool\fP) – can fail strategy flag
+\fBcanfail\fP (\fI\%bool\fP) \-\- can fail strategy flag
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NDSource(parent)
-Bases: \fI\%nxstools.nxsxml.NTag\fP
+.B class  nxstools.nxsxml.NDSource(parent)
+Bases: \fI\%NTag\fP
 .sp
 Source tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addDoc(doc)
 adds doc tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdoc\fP (\fI\%str\fP) – doc tag content
+\fBdoc\fP (\fI\%str\fP) \-\- doc tag content
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B initClient(name, recordName)
 sets paramters for Client data
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) – name of datasource
+\fBname\fP (\fI\%str\fP) \-\- name of datasource
 .IP \(bu 2
-\fBrecordName\fP (\fI\%str\fP) – name of the data object
+\fBrecordName\fP (\fI\%str\fP) \-\- name of the data object
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B initDBase(name, dbtype, query, dbname=None, rank=None, mycnf=None, user=None, passwd=None, dsn=None, mode=None, host=None, port=None)
 sets parameters of DataBase
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) – name of datasource
+\fBname\fP (\fI\%str\fP) \-\- name of datasource
 .IP \(bu 2
-\fBdbname\fP (\fI\%str\fP) – name of used DataBase
+\fBdbname\fP (\fI\%str\fP) \-\- name of used DataBase
 .IP \(bu 2
-\fBquery\fP (\fI\%str\fP) – database query
+\fBquery\fP (\fI\%str\fP) \-\- database query
 .IP \(bu 2
-\fBdbtype\fP (\fI\%str\fP) – type of the database, i.e. MYSQL, PGSQL, ORACLE
+\fBdbtype\fP (\fI\%str\fP) \-\- type of the database, i.e. MYSQL, PGSQL, ORACLE
 .IP \(bu 2
-\fBrank\fP (\fI\%str\fP) – rank of the query output, i.e. SCALAR, SPECTRUM, IMAGE
+\fBrank\fP (\fI\%str\fP) \-\- rank of the query output, i.e. SCALAR, SPECTRUM, IMAGE
 .IP \(bu 2
-\fBmycnf\fP (\fI\%str\fP) – MYSQL config file
+\fBmycnf\fP (\fI\%str\fP) \-\- MYSQL config file
 .IP \(bu 2
-\fBuser\fP (\fI\%str\fP) – database user name
+\fBuser\fP (\fI\%str\fP) \-\- database user name
 .IP \(bu 2
-\fBpasswd\fP (\fI\%str\fP) – database user password
+\fBpasswd\fP (\fI\%str\fP) \-\- database user password
 .IP \(bu 2
-\fBdsn\fP (\fI\%str\fP) – DSN string to initialize ORACLE and PGSQL databases
+\fBdsn\fP (\fI\%str\fP) \-\- DSN string to initialize ORACLE and PGSQL databases
 .IP \(bu 2
-\fBmode\fP (\fI\%str\fP) – mode for ORACLE databases, i.e. SYSDBA or SYSOPER
+\fBmode\fP (\fI\%str\fP) \-\- mode for ORACLE databases, i.e. SYSDBA or SYSOPER
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) – name of the host
+\fBhost\fP (\fI\%str\fP) \-\- name of the host
 .IP \(bu 2
-\fBport\fP (\fI\%str\fP) – port number
+\fBport\fP (\fI\%str\fP) \-\- port number
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B initTango(name, device, memberType, recordName, host=None, port=None, encoding=None, group=None)
 sets paramters for Tango device
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) – name of datasource
+\fBname\fP (\fI\%str\fP) \-\- name of datasource
 .IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) – device name
+\fBdevice\fP (\fI\%str\fP) \-\- device name
 .IP \(bu 2
-\fBmemberType\fP (\fI\%str\fP) – type of the data object, i.e. attribute,
+\fBmemberType\fP (\fI\%str\fP) \-\- type of the data object, i.e. attribute,
 property, command
 .IP \(bu 2
-\fBrecordName\fP (\fI\%str\fP) – name of the data object
+\fBrecordName\fP (\fI\%str\fP) \-\- name of the data object
 .IP \(bu 2
-\fBhost\fP (\fI\%str\fP) – host name
+\fBhost\fP (\fI\%str\fP) \-\- host name
 .IP \(bu 2
-\fBport\fP (\fI\%str\fP) – port
+\fBport\fP (\fI\%str\fP) \-\- port
 .IP \(bu 2
-\fBencoding\fP (\fI\%str\fP) – encoding of DevEncoded data
+\fBencoding\fP (\fI\%str\fP) \-\- encoding of DevEncoded data
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NDeviceGroup(parent, deviceName, nameAttr, typeAttr=\(aq\(aq, commands=True, blackAttrs=None)
-Bases: \fI\%nxstools.nxsxml.NGroup\fP
+.B class  nxstools.nxsxml.NDeviceGroup(parent, deviceName, nameAttr, typeAttr=\(aq\(aq, commands=True, blackAttrs=None)
+Bases: \fI\%NGroup\fP
 .sp
 Tango device tag creator
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .IP \(bu 2
-\fBdeviceName\fP (\fI\%str\fP) – tango device name
+\fBdeviceName\fP (\fI\%str\fP) \-\- tango device name
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) – name attribute
+\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) – type attribute
+\fBtypeAttr\fP (\fI\%str\fP) \-\- type attribute
 .IP \(bu 2
-\fBcommands\fP (\fI\%bool\fP) – if we call the commands
+\fBcommands\fP (\fI\%bool\fP) \-\- if we call the commands
 .IP \(bu 2
-\fBblackAttrs\fP (\fI\%list\fP <\fI\%str\fP>) – list of excluded attributes
+\fBblackAttrs\fP (\fI\%list\fP <\fI\%str\fP>) \-\- list of excluded attributes
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B nTypes = [\(aqNX_CHAR\(aq, \(aqNX_BOOLEAN\(aq, \(aqNX_INT32\(aq, \(aqNX_INT32\(aq, \(aqNX_FLOAT32\(aq, \(aqNX_FLOAT64\(aq, \(aqNX_UINT32\(aq, \(aqNX_UINT32\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_INT32\(aq, \(aqNX_INT32\(aq, \(aqNX_FLOAT32\(aq, \(aqNX_FLOAT64\(aq, \(aqNX_UINT32\(aq, \(aqNX_UINT32\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_BOOLEAN\(aq, \(aqNX_CHAR\(aq, \(aqNX_INT64\(aq, \(aqNX_UINT64\(aq, \(aqNX_INT64\(aq, \(aqNX_UINT64\(aq, \(aqNX_INT32\(aq, \(aqNX_CHAR\(aq]
+.B nTypes  =  [\(aqNX_CHAR\(aq, \(aqNX_BOOLEAN\(aq, \(aqNX_INT32\(aq, \(aqNX_INT32\(aq, \(aqNX_FLOAT32\(aq, \(aqNX_FLOAT64\(aq, \(aqNX_UINT32\(aq, \(aqNX_UINT32\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_INT32\(aq, \(aqNX_INT32\(aq, \(aqNX_FLOAT32\(aq, \(aqNX_FLOAT64\(aq, \(aqNX_UINT32\(aq, \(aqNX_UINT32\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_CHAR\(aq, \(aqNX_BOOLEAN\(aq, \(aqNX_CHAR\(aq, \(aqNX_INT64\(aq, \(aqNX_UINT64\(aq, \(aqNX_INT64\(aq, \(aqNX_UINT64\(aq, \(aqNX_INT32\(aq, \(aqNX_CHAR\(aq]
 (\fI\%list\fP <\fI\%str\fP>) NeXuS types corresponding to the Tango types
 .UNINDENT
 .INDENT 7.0
 .TP
-.B tTypes = [\(aqDevVoid\(aq, \(aqDevBoolean\(aq, \(aqDevShort\(aq, \(aqDevLong\(aq, \(aqDevFloat\(aq, \(aqDevDouble\(aq, \(aqDevUShort\(aq, \(aqDevULong\(aq, \(aqDevString\(aq, \(aqDevVarCharArray\(aq, \(aqDevVarShortArray\(aq, \(aqDevVarLongArray\(aq, \(aqDevVarFloatArray\(aq, \(aqDevVarDoubleArray\(aq, \(aqDevVarUShortArray\(aq, \(aqDevVarULongArray\(aq, \(aqDevVarStringArray\(aq, \(aqDevVarLongStringArray\(aq, \(aqDevVarDoubleStringArray\(aq, \(aqDevState\(aq, \(aqConstDevString\(aq, \(aqDevVarBooleanArray\(aq, \(aqDevUChar\(aq, \(aqDevLong64\(aq, \(aqDevULong64\(aq, \(aqDevVarLong64Array\(aq, \(aqDevVarULong64Array\(aq, \(aqDevInt\(aq, \(aqDevEncoded\(aq]
+.B tTypes  =  [\(aqDevVoid\(aq, \(aqDevBoolean\(aq, \(aqDevShort\(aq, \(aqDevLong\(aq, \(aqDevFloat\(aq, \(aqDevDouble\(aq, \(aqDevUShort\(aq, \(aqDevULong\(aq, \(aqDevString\(aq, \(aqDevVarCharArray\(aq, \(aqDevVarShortArray\(aq, \(aqDevVarLongArray\(aq, \(aqDevVarFloatArray\(aq, \(aqDevVarDoubleArray\(aq, \(aqDevVarUShortArray\(aq, \(aqDevVarULongArray\(aq, \(aqDevVarStringArray\(aq, \(aqDevVarLongStringArray\(aq, \(aqDevVarDoubleStringArray\(aq, \(aqDevState\(aq, \(aqConstDevString\(aq, \(aqDevVarBooleanArray\(aq, \(aqDevUChar\(aq, \(aqDevLong64\(aq, \(aqDevULong64\(aq, \(aqDevVarLong64Array\(aq, \(aqDevVarULong64Array\(aq, \(aqDevInt\(aq, \(aqDevEncoded\(aq]
 (\fI\%list\fP < \fI\%str\fP>) Tango types
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NDim(parent, indexAttr, valueAttr)
-Bases: \fI\%nxstools.nxsxml.NTag\fP
+.B class  nxstools.nxsxml.NDim(parent, indexAttr, valueAttr)
+Bases: \fI\%NTag\fP
 .sp
 Dim tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .IP \(bu 2
-\fBindexAttr\fP (\fI\%str\fP) – index attribute
+\fBindexAttr\fP (\fI\%str\fP) \-\- index attribute
 .IP \(bu 2
-\fBvalueAttr\fP (\fI\%str\fP) – value attribute
+\fBvalueAttr\fP (\fI\%str\fP) \-\- value attribute
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NDimensions(parent, rankAttr)
-Bases: \fI\%nxstools.nxsxml.NTag\fP
+.B class  nxstools.nxsxml.NDimensions(parent, rankAttr)
+Bases: \fI\%NTag\fP
 .sp
 Dimensions tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .IP \(bu 2
-\fBrankAttr\fP (\fI\%str\fP) – rank attribute
+\fBrankAttr\fP (\fI\%str\fP) \-\- rank attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B dim(indexAttr, valueAttr)
 adds dim tag
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBindexAttr\fP (\fI\%str\fP) – index attribute
+\fBindexAttr\fP (\fI\%str\fP) \-\- index attribute
 .IP \(bu 2
-\fBvalueAttr\fP (\fI\%str\fP) – value attribute
+\fBvalueAttr\fP (\fI\%str\fP) \-\- value attribute
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B dims = None
+.B dims
 (\fI\%dict\fP <\fI\%str\fP, \fI\%NDim\fP>)
 container with dim tag wrapper
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NField(parent, nameAttr, typeAttr=\(aq\(aq)
-Bases: \fI\%nxstools.nxsxml.NTag\fP
+.B class  nxstools.nxsxml.NField(parent, nameAttr, typeAttr=\(aq\(aq)
+Bases: \fI\%NTag\fP
 .sp
 Field tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) – name attribute
+\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) – type attribute
+\fBtypeAttr\fP (\fI\%str\fP) \-\- type attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addAttr(attrName, attrType, attrValue=\(aq\(aq)
 adds attribute tag
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBattrName\fP (\fI\%str\fP) – name attribute
+\fBattrName\fP (\fI\%str\fP) \-\- name attribute
 .IP \(bu 2
-\fBattrType\fP (\fI\%str\fP) – type attribute
+\fBattrType\fP (\fI\%str\fP) \-\- type attribute
 .IP \(bu 2
-\fBattrValue\fP (\fI\%str\fP) – content of the attribute tag
+\fBattrValue\fP (\fI\%str\fP) \-\- content of the attribute tag
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addDoc(doc)
 adds doc tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdoc\fP (\fI\%str\fP) – doc tag content
+\fBdoc\fP (\fI\%str\fP) \-\- doc tag content
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setStrategy(mode=\(aqSTEP\(aq, trigger=None, value=None, grows=None, compression=False, rate=None, shuffle=None, canfail=None, compression_opts=None)
 sets the field strategy
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBmode\fP (\fI\%str\fP) – mode data writing, i.e. INIT, STEP, FINAL, POSTRUN
+\fBmode\fP (\fI\%str\fP) \-\- mode data writing, i.e. INIT, STEP, FINAL, POSTRUN
 .IP \(bu 2
-\fBtrigger\fP (\fI\%str\fP) – for asynchronous writting,
+\fBtrigger\fP (\fI\%str\fP) \-\- for asynchronous writting,
 e.g. with different subentries
 .IP \(bu 2
-\fBvalue\fP (\fI\%str\fP) – label for postrun mode
+\fBvalue\fP (\fI\%str\fP) \-\- label for postrun mode
 .IP \(bu 2
-\fBgrows\fP (\fI\%str\fP) – growing dimension
+\fBgrows\fP (\fI\%str\fP) \-\- growing dimension
 .IP \(bu 2
-\fBcompression\fP (\fI\%str\fP) – flag if compression shuold be applied
+\fBcompression\fP (\fI\%str\fP) \-\- flag if compression shuold be applied
 .IP \(bu 2
-\fBrate\fP (\fI\%str\fP) – compression rate
+\fBrate\fP (\fI\%str\fP) \-\- compression rate
 .IP \(bu 2
-\fBshuffle\fP (\fI\%str\fP) – flag if compression shuffle
+\fBshuffle\fP (\fI\%str\fP) \-\- flag if compression shuffle
 .IP \(bu 2
-\fBcanfail\fP (\fI\%bool\fP) – can fail strategy flag
+\fBcanfail\fP (\fI\%bool\fP) \-\- can fail strategy flag
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setUnits(unitsAttr)
 sets the field unit
 .INDENT 7.0
 .TP
 .B Parameters
-\fBunitsAttr\fP (\fI\%str\fP) – the field unit
+\fBunitsAttr\fP (\fI\%str\fP) \-\- the field unit
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NGroup(parent, nameAttr, typeAttr=\(aq\(aq)
-Bases: \fI\%nxstools.nxsxml.NTag\fP
+.B class  nxstools.nxsxml.NGroup(parent, nameAttr, typeAttr=\(aq\(aq)
+Bases: \fI\%NTag\fP
 .sp
 Group tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) – name attribute
+\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) – type attribute
+\fBtypeAttr\fP (\fI\%str\fP) \-\- type attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addAttr(attrName, attrType, attrValue=\(aq\(aq)
 adds attribute: tag
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBattrName\fP (\fI\%str\fP) – name attribute
+\fBattrName\fP (\fI\%str\fP) \-\- name attribute
 .IP \(bu 2
-\fBattrType\fP (\fI\%str\fP) – type attribute
+\fBattrType\fP (\fI\%str\fP) \-\- type attribute
 .IP \(bu 2
-\fBattrValue\fP (\fI\%str\fP) – content of the attribute tag
+\fBattrValue\fP (\fI\%str\fP) \-\- content of the attribute tag
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addDoc(doc)
 adds doc tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdoc\fP (\fI\%str\fP) – doc tag content
+\fBdoc\fP (\fI\%str\fP) \-\- doc tag content
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NLink(parent, nameAttr, gTarget)
-Bases: \fI\%nxstools.nxsxml.NTag\fP
+.B class  nxstools.nxsxml.NLink(parent, nameAttr, gTarget)
+Bases: \fI\%NTag\fP
 .sp
 Link tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) – name attribute
+\fBnameAttr\fP (\fI\%str\fP) \-\- name attribute
 .IP \(bu 2
-\fBgTarget\fP (\fI\%str\fP) – target attribute
+\fBgTarget\fP (\fI\%str\fP) \-\- target attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addDoc(doc)
 adds doc tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBdoc\fP (\fI\%str\fP) – doc tag content
+\fBdoc\fP (\fI\%str\fP) \-\- doc tag content
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.NTag(parent, tagName, nameAttr=\(aq\(aq, typeAttr=\(aq\(aq)
+.B class  nxstools.nxsxml.NTag(parent, tagName, nameAttr=\(aq\(aq, typeAttr=\(aq\(aq)
 Bases: \fI\%object\fP
 .sp
 tag wrapper
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBparent\fP (\fI\%NTag\fP) – parent tag element
+\fBparent\fP (\fI\%NTag\fP) \-\- parent tag element
 .IP \(bu 2
-\fBtagName\fP (\fI\%str\fP) – tag name
+\fBtagName\fP (\fI\%str\fP) \-\- tag name
 .IP \(bu 2
-\fBnameAttr\fP (\fI\%str\fP) – value of name attribute
+\fBnameAttr\fP (\fI\%str\fP) \-\- value of name attribute
 .IP \(bu 2
-\fBtypeAttr\fP (\fI\%str\fP) – value of type attribute
+\fBtypeAttr\fP (\fI\%str\fP) \-\- value of type attribute
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addTagAttr(name, value)
 adds tag attribute
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBname\fP (\fI\%str\fP) – attribute name
+\fBname\fP (\fI\%str\fP) \-\- attribute name
 .IP \(bu 2
-\fBvalue\fP (\fI\%str\fP) – attribute value
+\fBvalue\fP (\fI\%str\fP) \-\- attribute value
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
 .B addText(text)
 adds tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtext\fP (\fI\%str\fP) – tag content
+\fBtext\fP (\fI\%str\fP) \-\- tag content
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B elem = None
+.B elem
 (\fBlxml.etree.Element\fP) tag element from etree
 .UNINDENT
 .INDENT 7.0
 .TP
 .B setText(text)
 sets tag content
 .INDENT 7.0
 .TP
 .B Parameters
-\fBtext\fP (\fI\%str\fP) – tag content
+\fBtext\fP (\fI\%str\fP) \-\- tag content
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B class nxstools.nxsxml.XMLFile(fname)
+.B class  nxstools.nxsxml.XMLFile(fname)
 Bases: \fI\%object\fP
 .sp
 XML file object
 .sp
 constructor
 .INDENT 7.0
 .TP
 .B Parameters
-\fBfname\fP (\fI\%str\fP) – XML file name
+\fBfname\fP (\fI\%str\fP) \-\- XML file name
 .UNINDENT
 .INDENT 7.0
 .TP
 .B dump()
 dumps XML structure into the XML file
 .INDENT 7.0
 .TP
 .B Brief
 It opens XML file, calls prettyPrint and closes the XML file
 .UNINDENT
 .UNINDENT
 .INDENT 7.0
 .TP
-.B elem = None
+.B elem
 (\fBlxml.etree.Element\fP) XML root instance
 .UNINDENT
 .INDENT 7.0
 .TP
-.B fname = None
+.B fname
 (\fI\%str\fP) XML file name
 .UNINDENT
 .INDENT 7.0
 .TP
 .B prettyPrint(etNode=None)
 prints pretty XML making use of etree
 .INDENT 7.0
 .TP
 .B Parameters
-\fBetNode\fP (\fBlxml.etree.Element\fP) – node
-.UNINDENT
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsxml.main()
-the main function
-.UNINDENT
-.SS nxstools.nxsdevicetools module
-.sp
-NDTS TANGO device tools
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.PYTANGO = True
-(\fI\%bool\fP) True if PyTango available
-.UNINDENT
-.INDENT 0.0
-.TP
-.B class nxstools.nxsdevicetools.PackageHandler(packagename=\(aqnxstools.xmltemplates\(aq)
-Bases: \fI\%object\fP
-.sp
-xml templates package loader
-.sp
-constructor
-.INDENT 7.0
-.TP
-.B Parameters
-\fBpackagename\fP (\fI\%str\fP) – full package name
-.UNINDENT
-.INDENT 7.0
-.TP
-.B loadXMLTemplates(packagename)
-load xml template module variables
-.INDENT 7.0
-.TP
-.B Parameters
-\fBpackagename\fP (\fI\%str\fP) – full package name
-.UNINDENT
+\fBetNode\fP (\fBlxml.etree.Element\fP) \-\- node
 .UNINDENT
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.checkServer(name=\(aqNXSConfigServer\(aq)
-provides server device name if only one or error in the other case
 .INDENT 7.0
 .TP
-.B Parameters
-\fBname\fP (\fI\%str\fP) – server name
-.TP
-.B Returns
-server device name or empty string if error appears
-.TP
-.B Return type
-\fI\%str\fP
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.ctModules = [\(aqmca8715roi\(aq, \(aqonedroi\(aq, \(aqsis3820\(aq, \(aqsis3302roi\(aq, \(aqxmcd\(aq, \(aqvfcadc\(aq, \(aqmythenroi\(aq, \(aqmhzdaqp01\(aq, \(aqdgg2\(aq, \(aqtangoattributectctrl\(aq]
-(\fI\%list\fP <\fI\%str\fP>) counter/timer modules
-.UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.findClassName(server, name)
-finds class name
-.INDENT 7.0
-.TP
-.B Parameters
-\fBname\fP (\fI\%str\fP) – device name
-.TP
-.B Returns
-class name
-.TP
-.B Return type
-\fI\%str\fP
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.generateDeviceNames(prefix, first, last, minimal=False)
-generates device names
+.B setDependencies(components, entry=None)
+sets tag content
 .INDENT 7.0
 .TP
 .B Parameters
 .INDENT 7.0
 .IP \(bu 2
-\fBprefix\fP (\fI\%str\fP) – device name prefix
-.IP \(bu 2
-\fBfirst\fP (\fI\%int\fP) – first device index
+\fBcomponents\fP (\fI\%list\fP <\fI\%str\fP>) \-\- component dependencies
 .IP \(bu 2
-\fBlast\fP (\fI\%int\fP) – last device index
+\fBentry\fP (\fBlxml.etree.Element\fP) \-\- entry node
 .UNINDENT
-.TP
-.B Returns
-device names
-.TP
-.B Return type
-\fI\%list\fP <\fI\%str\fP>
 .UNINDENT
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.getAttributes(device, host=None, port=10000)
-provides a list of device attributes
-.INDENT 7.0
-.TP
-.B Parameters
-.INDENT 7.0
-.IP \(bu 2
-\fBdevice\fP (\fI\%str\fP) – tango device name
-.IP \(bu 2
-\fBhost\fP (\fI\%str\fP) – device host
-.IP \(bu 2
-\fBport\fP (\fI\%int\fP) – device port
-.UNINDENT
-.TP
-.B Returns
-list of device attributes
-.TP
-.B Return type
-\fI\%list\fP <\fI\%str\fP>
-.UNINDENT
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxstools.nxsdevicetools.getClassName(devicename)
-provides device class name
-.INDENT 7.0
-.TP
-.B Parameters
-\fBdevicename\fP (\fI\%str\fP) – device name
-.TP
-.B Returns
-class name
-.TP
-.B Return type
-\fI\%str\fP
-.UNINDENT
+.B nxstools.nxsxml.main()
+the main function
 .UNINDENT
+.SS nxstools.release module
+.sp
+NXS tools release version
+.SS nxstools.redisutils module
+.sp
+Provides redis utils
 .INDENT 0.0
 .TP
-.B nxstools.nxsdevicetools.getDataSourceComponents(server, verbose=False)
-gets datasource components
+.B class  nxstools.redisutils.DESYIdentityModel(*, pk:  \fI\%Optional\fP[\fI\%str\fP]  =  None, name:  \fI\%str\fP, number:  \fI\%int\fP, data_policy:  \fI\%str\fP, beamline:  \fI\%Optional\fP[\fI\%str\fP]  =  None, session:  \fI\%Optional\fP[\fI\%str\fP]  =  None, proposal:  \fI\%Optional\fP[\fI\%str\fP]  =  None, collection:  \fI\%Optional\fP[\fI\%str\fP]  =  None, dataset:  \fI\%Optional\fP[\fI\%str\fP]  =  None, path:  \fI\%Optional\fP[\fI\%str\fP]  =  None, **extra_data:  \fI\%Any\fP)
+Bases: \fBHashModel\fP
+.sp
+Institute specific information used to link scans
+in Redis to external services.
+.sp
+Create a new model by parsing and validating input data from keyword arguments.
+.sp
+Raises ValidationError if the input data cannot be parsed to form a valid model.
 .INDENT 7.0
 .TP
-.B Parameters
+.B class  Meta
+Bases: \fI\%object\fP
 .INDENT 7.0
-.IP \(bu 2
-\fBserver\fP (\fI\%str\fP) – configuration server
-.IP \(bu 2
-\fBverbose\fP (\fI\%bool\fP) – additional printouts
-.UNINDENT
-.TP
-.B Returns
-dictionary with datasource components
 .TP
-.B Return type
-\fI\%dict\fP <\fI\%str\fP, \fI\%list\fP <\fI\%str\fP>>
-.UNINDENT
+.B database  =  <blissdata.redis_engine.identities._UninitializedRedis object>
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.getServerTangoHost(server)
-fetches the server tango_host:tango_port
 .INDENT 7.0
 .TP
-.B Parameters
-\fBserver\fP (\fI\%str\fP) – tango server
-.TP
-.B Returns
-tango host
-.TP
-.B Return type
-\fI\%str\fP
-.UNINDENT
+.B encoding  =  \(aqutf\-8\(aq
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.getServers(name=\(aqNXSConfigServer\(aq)
-provides server device names
 .INDENT 7.0
 .TP
-.B Parameters
-\fBname\fP (\fI\%str\fP) – server instance name
-.TP
-.B Returns
-list of the server device names
-.TP
-.B Return type
-\fI\%list\fP <\fI\%str\fP>
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.ioRegModules = [\(aqsis3610\(aq]
-(\fI\%list\fP <\fI\%str\fP>) IO register modules
+.B global_key_prefix  =  \(aqesrf\(aq
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.listServers(server, name=\(aqNXSConfigServer\(aq)
-finds server names
 .INDENT 7.0
 .TP
-.B Parameters
-\fBname\fP (\fI\%str\fP) – server instance name
-.TP
-.B Returns
-server list
-.TP
-.B Return type
-\fI\%list\fP <\fI\%str\fP>
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.moduleMultiAttributes = {\(aqdalsa\(aq: [\(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqTriggerMode\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqExtendedExposure\(aq, \(aqBinComment\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqFramesReceived\(aq, \(aqFrameRate\(aq, \(aqFramesPerNXFile\(aq, \(aqNXFileCompression\(aq, \(aqTurboMode\(aq, \(aqImageEnc\(aq, \(aqViewingMode\(aq, \(aqThrashedBuffers\(aq, \(aqFramesToAcquire\(aq, \(aqAcquisitionFrameCount\(aq, \(aqAcquisitionMode\(aq, \(aqAcquisitionFrameMode\(aq, \(aqLinearityEqualizer\(aq, \(aqNrExposedFrames\(aq, \(aqNrOffsetFrames\(aq, \(aqOffset\(aq, \(aqPixelFormat\(aq, \(aqReadOutMode\(aq, \(aqStandby\(aq, \(aqSumScheme\(aq], \(aqeigerdectris\(aq: [\(aqTriggerMode\(aq, \(aqNbTriggers\(aq, \(aqDescription\(aq, \(aqNbImages\(aq, \(aqBitDepth\(aq, \(aqReadoutTime\(aq, \(aqCountTime\(aq, \(aqEnergyThreshold\(aq, \(aqFrameTime\(aq, \(aqRateCorrectionEnabled\(aq, \(aqFlatFieldEnabled\(aq, \(aqTemperature\(aq, \(aqAutoSummationEnabled\(aq, \(aqHumidity\(aq, \(aqPhotonEnergy\(aq, \(aqWavelength\(aq], \(aqlambda\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq], \(aqlambda2m\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqOpMode\(aq], \(aqlambdavds\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq], \(aqlimaccd\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqlimaccds\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqmaiadimension\(aq: [\(aqName\(aq, \(aqPositionSource\(aq, \(aqPixelPitch\(aq, \(aqPixelOrigin\(aq, \(aqPixelHysteresis\(aq, \(aqPositionUnit\(aq, \(aqPixelCoordExtent\(aq], \(aqmaiaflux\(aq: [\(aqFluxCoeff\(aq, \(aqFluxName\(aq, \(aqFluxUnit\(aq, \(aqFluxSource\(aq], \(aqmaiainterlock\(aq: [\(aqBiasPeltierInterlock\(aq, \(aqBiasPeltierInterlockUptime\(aq, \(aqPressure\(aq], \(aqmaialogger\(aq: [\(aqRunNumber\(aq], \(aqmaiaprocessing\(aq: [\(aqGaintrimEnable\(aq, \(aqLineariseEnable\(aq, \(aqPhotonEnable\(aq, \(aqPileupRejectEnable\(aq, \(aqPixelEnable\(aq, \(aqThrottleEnable\(aq], \(aqmaiasensor\(aq: [\(aqBiasVoltage\(aq, \(aqLeakageCurrent\(aq, \(aqPeltierCurrent\(aq, \(aqWaterTemperature\(aq, \(aqDetectorTemperature\(aq, \(aqMosfetTemperature\(aq, \(aqIdentity\(aq], \(aqmarccd\(aq: [\(aqFrameShift\(aq, \(aqSavingDirectory\(aq, \(aqSavingPostfix\(aq, \(aqSavingPrefix\(aq], \(aqmca_xia\(aq: [\(aqICR\(aq, \(aqOCR\(aq], \(aqmca_xia@pool\(aq: [\(aqCountsRoI\(aq, \(aqRoIEnd\(aq, \(aqRoIStart\(aq], \(aqmythen\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqRoI1\(aq, \(aqRoI2\(aq], \(aqmythen2\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqEnergy\(aq, \(aqNbFrames\(aq, \(aqRoI1End\(aq, \(aqRoI2End\(aq, \(aqRoI1Start\(aq, \(aqRoI2Start\(aq, \(aqThreshold\(aq], \(aqpco\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpco4000\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpcoedge\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpedetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmer\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmerdetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqpilatus\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus100k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus1m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus2m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus300k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus6m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqtangovimba\(aq: [\(aqWidth\(aq, \(aqWidthMax\(aq, \(aqTriggerSource\(aq, \(aqPixelFormat\(aq, \(aqOffsetY\(aq, \(aqOffsetX\(aq, \(aqHeightMax\(aq, \(aqHeight\(aq, \(aqGainRaw\(aq, \(aqExposureTimeAbs\(aq, \(aqAcquisitionFrameRateAbs\(aq, \(aqAcquisitionFrameRateLimit\(aq, \(aqStreamBytesPerSecond\(aq, \(aqBinComment\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqMaxLoad\(aq, \(aqReadMode\(aq, \(aqTuneMode\(aq, \(aqViewingMode\(aq]}
-(\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
-important attributes of modules
+.B index_name  =  \(aqesrf:id:index\(aq
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.moduleTemplateFiles = {\(aqdalsa\(aq: [\(aqdalsa.xml\(aq, \(aqdalsa_nxdata.ds.xml\(aq, \(aqdalsa_external_data.ds.xml\(aq], \(aqeigerdectris\(aq: [\(aqeigerdectris.xml\(aq, \(aqeigerdectris_stepindex.ds.xml\(aq, \(aqeigerdectris_description_cb.ds.xml\(aq, \(aqeigerdectris_triggermode_cb.ds.xml\(aq], \(aqlambda\(aq: [\(aqlambda.xml\(aq, \(aqlambda_nxdata.ds.xml\(aq, \(aqlambda_external_data.ds.xml\(aq], \(aqlambda2m\(aq: [\(aqlambda2m.xml\(aq, \(aqlambda2m_m1_nxdata.ds.xml\(aq, \(aqlambda2m_m2_nxdata.ds.xml\(aq, \(aqlambda2m_m3_nxdata.ds.xml\(aq, \(aqlambda2m_m1_external_data.ds.xml\(aq, \(aqlambda2m_m2_external_data.ds.xml\(aq, \(aqlambda2m_m3_external_data.ds.xml\(aq], \(aqlambdavds\(aq: [\(aqlambdavds.xml\(aq, \(aqlambdavds_nxdata.ds.xml\(aq, \(aqlambdavds_description.ds.xml\(aq, \(aqlambdavds_triggermode_cb.ds.xml\(aq, \(aqlambdavds_framenumbers_cb.ds.xml\(aq, \(aqlambdavds_savefilename_cb.ds.xml\(aq], \(aqlimaccd\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqlimaccds\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqmarccd\(aq: [\(aqmarccd.xml\(aq, \(aqmarccd_postrun.ds.xml\(aq], \(aqmca_xia\(aq: [\(aqmcaxia.xml\(aq], \(aqmythen\(aq: [\(aqmythen.xml\(aq, \(aqmythen_postrun.ds.xml\(aq, \(aqmythen_filestartnumber.ds.xml\(aq], \(aqmythen2\(aq: [\(aqmythen2.xml\(aq], \(aqpco\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpco4000\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpcoedge\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpedetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmer\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmerdetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqpilatus\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus100k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus100k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus1m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus1m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus2m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus300k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus300k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus6m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqtangovimba\(aq: [\(aqtangovimba.xml\(aq, \(aqtangovimba_nxdata.ds.xml\(aq, \(aqtangovimba_external_data.ds.xml\(aq]}
-(\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
-xml template files of modules
-.UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B nxstools.nxsdevicetools.motorModules = [\(aqabsbox\(aq, \(aqmotor_tango\(aq, \(aqkohzu\(aq, \(aqsmchydra\(aq, \(aqlom\(aq, \(aqoms58\(aq, \(aqe6c\(aq, \(aqomsmaxv\(aq, \(aqspk\(aq, \(aqpie710\(aq, \(aqpie712\(aq, \(aqe6c_p09_eh2\(aq, \(aqsmaract\(aq]
-(\fI\%list\fP <\fI\%str\fP>) modules of motors
+.B model_key_prefix  =  \(aqid\(aq
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B nxstools.nxsdevicetools.oneDModules = [\(aqmca_xia\(aq]
-(\fI\%list\fP <\fI\%str\fP>) modules of 1D detectors
+.B primary_key  =  PrimaryKey(name=\(aqpk\(aq, field=ModelField(name=\(aqpk\(aq, type=Optional[str], required=False, default=None))
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.openServer(device)
-opens connection to the configuration server
 .INDENT 7.0
 .TP
-.B Parameters
-\fBconfiguration\fP (\fI\%str\fP) – server device name
-.TP
-.B Returns
-configuration server proxy
-.TP
-.B Return type
-\fBPyTango.DeviceProxy\fP
+.B primary_key_creator_cls
+alias of \fBUlidPrimaryKey\fP
 .UNINDENT
-.UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B nxstools.nxsdevicetools.standardComponentTemplateFiles = {\(aqabsorber\(aq: [\(aqabsorber_foil.ds.xml\(aq, \(aqabsorber_thickness.ds.xml\(aq, \(aqabsorber.xml\(aq], \(aqbeamstop\(aq: [\(aqbeamstop.xml\(aq], \(aqbeamtimeid\(aq: [\(aqbeamtimeid.xml\(aq, \(aqbeamtimeid.ds.xml\(aq, \(aqstart_time.ds.xml\(aq], \(aqchcut\(aq: [\(aqchcut.xml\(aq, \(aqchcut_unitcalibration.ds.xml\(aq, \(aqchcut_crystal.ds.xml\(aq], \(aqcollect2\(aq: [\(aqcollect2.xml\(aq], \(aqcollect3\(aq: [\(aqcollect3.xml\(aq], \(aqcollect4\(aq: [\(aqcollect4.xml\(aq], \(aqcollect5\(aq: [\(aqcollect5.xml\(aq], \(aqcollect6\(aq: [\(aqcollect6.xml\(aq], \(aqcommon2\(aq: [\(aqcommon2_common.ds.xml\(aq], \(aqcommon3\(aq: [\(aqcommon3_common.ds.xml\(aq], \(aqdatasignal\(aq: [\(aqdatasignal.xml\(aq, \(aqdefaultsignal.ds.xml\(aq, \(aqsignal_name.ds.xml\(aq, \(aqsignalname.ds.xml\(aq, \(aqsignal_axes.ds.xml\(aq], \(aqdcm\(aq: [\(aqdcm.xml\(aq, \(aqdcm_reflection.ds.xml\(aq, \(aqdcm_unitcalibration.ds.xml\(aq, \(aqdcm_crystal.ds.xml\(aq], \(aqdefault\(aq: [\(aqdefault.xml\(aq, \(aqdefaultsample.xml\(aq, \(aqdefaultinstrument.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultinstrument\(aq: [\(aqdefaultinstrument.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultsample\(aq: [\(aqdefaultsample.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq], \(aqdetectorlive\(aq: [\(aqdetectorlive.xml\(aq], \(aqempty\(aq: [\(aqempty.xml\(aq], \(aqkeithley\(aq: [\(aqkeithley.xml\(aq], \(aqmaia\(aq: [\(aqmaia.xml\(aq, \(aqempty.xml\(aq], \(aqmaiadimension\(aq: [\(aqmaiadimension.xml\(aq], \(aqmaiaflux\(aq: [\(aqmaiaflux.xml\(aq], \(aqmsnsar\(aq: [\(aqmsnsar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqmssar\(aq: [\(aqmssar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqpinhole\(aq: [\(aqpinhole.xml\(aq], \(aqpointdet\(aq: [\(aqpointdet.xml\(aq], \(aqqbpm\(aq: [\(aqqbpm_foil.ds.xml\(aq, \(aqqbpm.xml\(aq], \(aqsamplehkl\(aq: [\(aqsamplehkl.xml\(aq], \(aqslit\(aq: [\(aqslit.xml\(aq], \(aqsource\(aq: [\(aqsource.xml\(aq], \(aqundulator\(aq: [\(aqundulator.xml\(aq]}
-(\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
-xml template files of modules
+.B primary_key_pattern  =  \(aq{pk}\(aq
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.standardComponentVariables = {\(aqabsorber\(aq: {\(aqattenfactor\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqattenuation factor (datasource)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqfoil\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil type, i.e. standard <cpname>_foil (datasource)\(aq}, \(aqfoillist\(aq: {\(aqdefault\(aq: \(aq["Ag", "Ag", "Ag", "Ag", "", "Al", "Al", "Al", "Al"]\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqposition\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqwhich sliders are in [bitarray] MANDATORY (datasource)\(aq}, \(aqthickness\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil thickness, i.e. standard <cpname>_thickness (datasource)\(aq}, \(aqthicknesslist\(aq: {\(aqdefault\(aq: \(aq[0.5, 0.05, 0.025, 0.0125, 0, 0.1, 0.3, 0.5, 1.0]\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: "transformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)"}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}}, \(aqbeamstop\(aq: {\(aqdescription\(aq: {\(aqdefault\(aq: \(aqcircular\(aq, \(aqdoc\(aq: \(aq circular or  rectangular (string)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqxsign\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: "horizontal position sign, e.g. \(aq\-\(aq (string)"}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}, \(aqz\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqzname\(aq: {\(aqdefault\(aq: \(aqz\(aq, \(aqdoc\(aq: \(aqalong the beam position name (string)\(aq}}, \(aqbeamtimeid\(aq: {\(aqcommissiondir\(aq: {\(aqdefault\(aq: \(aq/gpfs/commissioning\(aq, \(aqdoc\(aq: \(aqcommission file directory (string)\(aq}, \(aqcommissionpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqcommission file postfix (string)\(aq}, \(aqcommissionprefix\(aq: {\(aqdefault\(aq: \(aqcommissioning\-metadata\-\(aq, \(aqdoc\(aq: \(aqcommission file prefix (string)\(aq}, \(aqcurrentdir\(aq: {\(aqdefault\(aq: \(aq/gpfs/current\(aq, \(aqdoc\(aq: \(aqbeamtime file directory (string)\(aq}, \(aqcurrentpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqbeamtime file postfix (string)\(aq}, \(aqcurrentprefix\(aq: {\(aqdefault\(aq: \(aqbeamtime\-metadata\-\(aq, \(aqdoc\(aq: \(aqbeamtime file prefix (string)\(aq}, \(aqlocaldir\(aq: {\(aqdefault\(aq: \(aq/gpfs/local\(aq, \(aqdoc\(aq: \(aqlocal file directory (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}}, \(aqchcut\(aq: {\(aqbraggangle\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbragg angle (datasource)\(aq}, \(aqbragganglename\(aq: {\(aqdefault\(aq: \(aqbragg\(aq, \(aqdoc\(aq: \(aqbragg angle name  (string)\(aq}, \(aqchcutdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqFMBOxfDCMEnergy tango device name (string)\(aq}, \(aqcrystal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq type of crystal i.e. 0\->Si111,1\->Si311,2\->Si111 ChannelCut  (datasource)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsynchronized monochromator energy (datasource)\(aq}, \(aqenergyfmb\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmonochromator energy (datasource)\(aq}, \(aqjack1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfirst vertical jack of table (datasource)\(aq}, \(aqjack1name\(aq: {\(aqdefault\(aq: \(aqjack1\(aq, \(aqdoc\(aq: \(aqfirst vertical jack name of table (string)\(aq}, \(aqjack2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond vertical jack of table (datasource)\(aq}, \(aqjack2name\(aq: {\(aqdefault\(aq: \(aqjack2\(aq, \(aqdoc\(aq: \(aqsecond vertical jack name of table (string)\(aq}, \(aqjack3\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthird vertical jack of table (datasource)\(aq}, \(aqjack3name\(aq: {\(aqdefault\(aq: \(aqjack3\(aq, \(aqdoc\(aq: \(aqthird vertical jack name of table (string)\(aq}, \(aqlat\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the first cristal (datasource)\(aq}, \(aqlatname\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the first cristal (string)\(aq}, \(aqoxfordhorizontal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq horizontal translation (datasource)\(aq}, \(aqpara\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance between the crystals (string)\(aq}, \(aqparaname\(aq: {\(aqdefault\(aq: \(aqpara\(aq, \(aqdoc\(aq: \(aqbeam parallel translation name of the second cristal (string)\(aq}, \(aqreflection\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqreflection from string (datasource)\(aq}, \(aqtable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position of table (datasource)\(aq}, \(aqtablename\(aq: {\(aqdefault\(aq: \(aqtable\(aq, \(aqdoc\(aq: \(aqvertical position name of table (string)\(aq}, \(aqtheta\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta angle (datasource)\(aq}, \(aqthetaname\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta angle name (string)\(aq}, \(aqunitcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq unit calibration from dcmmotor (datasource)\(aq}, \(aqusage\(aq: {\(aqdefault\(aq: \(aqBragg\(aq, \(aqdoc\(aq: \(aqthe crystall usage, e.g. Laue (string)\(aq}, \(aqyaw\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the first cristal (datasource)\(aq}, \(aqyawname\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the first cristal (string)\(aq}}, \(aqcollect2\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}}, \(aqcollect3\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect4\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect5\(aq: {\(aqfifth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fifth component to collect MANDATORY (datasource)\(aq}, \(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect6\(aq: {\(aqfifth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fifth component to collect MANDATORY (datasource)\(aq}, \(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqsixth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the sixth component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcommon2\(aq: {\(aqdds\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdefault read datasource name MANDATORY (datasource)\(aq}, \(aqods\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqoptional detasource name MANDATORY (datasource)\(aq}}, \(aqcommon3\(aq: {\(aqdds\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdefault read datasource name MANDATORY (datasource)\(aq}, \(aqods1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfist optional detasource name MANDATORY (datasource)\(aq}, \(aqods2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond optional detasource name MANDATORY (datasource)\(aq}}, \(aqdatasignal\(aq: {\(aqaxes\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdata axes field name(s) (string)\(aq}, \(aqsignal\(aq: {\(aqdefault\(aq: \(aqdefaultsignal\(aq, \(aqdoc\(aq: \(aqdata signal field name (string)\(aq}}, \(aqdcm\(aq: {\(aqbend1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbending of the first cristal (datasource)\(aq}, \(aqbend2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbending of the second cristal (datasource)\(aq}, \(aqbraggangle\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbragg angle (datasource)\(aq}, \(aqbragganglename\(aq: {\(aqdefault\(aq: \(aqbragg\(aq, \(aqdoc\(aq: \(aqbragg angle name  (string)\(aq}, \(aqchi2dependson\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqthe depends_on field of the second cristal chi, e.g. phi (string)\(aq}, \(aqcrystal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtype of crystal i.e. 0\->Si111,1\->Si311,2\->Si111 ChannelCut (datasource)\(aq}, \(aqdcmdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqFMBOxfDCMEnergy tango device (string)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsynchronized monochromator energy (datasource)\(aq}, \(aqenergyfmb\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmonochromator energy (datasource)\(aq}, \(aqexitoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq exit offset (datasource)\(aq}, \(aqjack1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfirst vertical jack of table (datasource)\(aq}, \(aqjack1name\(aq: {\(aqdefault\(aq: \(aqjack1\(aq, \(aqdoc\(aq: \(aqfirst vertical jack name of table (string)\(aq}, \(aqjack2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond vertical jack of table (datasource)\(aq}, \(aqjack2name\(aq: {\(aqdefault\(aq: \(aqjack2\(aq, \(aqdoc\(aq: \(aqsecond vertical jack name of table (string)\(aq}, \(aqjack3\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthird vertical jack of table (datasource)\(aq}, \(aqjack3name\(aq: {\(aqdefault\(aq: \(aqjack3\(aq, \(aqdoc\(aq: \(aqthird vertical jack name of table (string)\(aq}, \(aqlat\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the first cristal (datasource)\(aq}, \(aqlat2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the second cristal (datasource)\(aq}, \(aqlat2name\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the second cristal (string)\(aq}, \(aqlatname\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the first cristal (string)\(aq}, \(aqoxfordhorizontal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq horizontal translation (datasource)\(aq}, \(aqpar2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbeam parallel translation of the second cristal (datasource)\(aq}, \(aqpar2name\(aq: {\(aqdefault\(aq: \(aqpara\(aq, \(aqdoc\(aq: \(aqbeam parallel translation name of the second cristal (string)\(aq}, \(aqperp2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical translation of the second cristal (datasource)\(aq}, \(aqperp2name\(aq: {\(aqdefault\(aq: \(aqperp\(aq, \(aqdoc\(aq: \(aqvertical translation name of the second cristal (string)\(aq}, \(aqphi1dependson\(aq: {\(aqdefault\(aq: \(aq../../transformations/bragg\(aq, \(aqdoc\(aq: \(aqthe depends_on field of the first cristal phi, e.g. theta (string)\(aq}, \(aqpitch1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta rotation of the first cristal (datasource)\(aq}, \(aqpitch1name\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta rotation name of the first cristal (string)\(aq}, \(aqpitch2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta rotation of the second cristal (datasource)\(aq}, \(aqpitch2name\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta rotation name of the second cristal (string)\(aq}, \(aqroll1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchi rotation of the first cristal (datasource)\(aq}, \(aqroll1name\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqchi rotation name of the first cristal (string)\(aq}, \(aqroll2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchi rotation of the second cristal (datasource)\(aq}, \(aqroll2name\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqchi rotation name of the second cristal (string)\(aq}, \(aqtable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position of table (datasource)\(aq}, \(aqtablename\(aq: {\(aqdefault\(aq: \(aqtable\(aq, \(aqdoc\(aq: \(aqvertical position name of table (string)\(aq}, \(aqtheta\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta angle (datasource)\(aq}, \(aqthetaname\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta angle name (string)\(aq}, \(aqtopdependson2\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqthe first transformation of the second crystal, e.g. lat (string)\(aq}, \(aqunitcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqunit calibration from dcmmotor (datasource)\(aq}, \(aqusage\(aq: {\(aqdefault\(aq: \(aqBragg\(aq, \(aqdoc\(aq: \(aqthe crystall usage, e.g. Laue (string)\(aq}, \(aqyaw\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the first cristal (datasource)\(aq}, \(aqyaw2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the second cristal (datasource)\(aq}, \(aqyaw2name\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the second cristal (string)\(aq}, \(aqyawname\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the first cristal (string)\(aq}}, \(aqdefault\(aq: {\(aq__configdevice__\(aq: {\(aqdefault\(aq: \(aqnxs/configserver/localhost\(aq, \(aqdoc\(aq: \(aqconfiguration server device name (string)\(aq}, \(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqcontrol\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgroup name of the monitor (string)\(aq}, \(aqlongname\(aq: {\(aqdefault\(aq: \(aqP09 Resonant Scattering and Diffraction beamline\(aq, \(aqdoc\(aq: \(aqbeamline long name (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}, \(aqsourcename\(aq: {\(aqdefault\(aq: \(aqPETRA III\(aq, \(aqdoc\(aq: \(aqsource name (string)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqdefaultinstrument\(aq: {\(aq__configdevice__\(aq: {\(aqdefault\(aq: \(aqnxs/configserver/localhost\(aq, \(aqdoc\(aq: \(aqconfiguration server device name (string)\(aq}, \(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqcontrol\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgroup name of the monitor (string)\(aq}, \(aqlongname\(aq: {\(aqdefault\(aq: \(aqP09 Resonant Scattering and Diffraction beamline\(aq, \(aqdoc\(aq: \(aqbeamline long name (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}, \(aqsourcename\(aq: {\(aqdefault\(aq: \(aqPETRA III\(aq, \(aqdoc\(aq: \(aqsource name (string)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqdefaultsample\(aq: {}, \(aqdetectorlive\(aq: {\(aqdatatype\(aq: {\(aqdefault\(aq: \(aqNX_UINT32\(aq, \(aqdoc\(aq: \(aqlist of devices (string)\(aq}, \(aqdetectordata\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdetector live data (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqdetector\(aq, \(aqdoc\(aq: \(aqlist of devices (string)\(aq}}, \(aqempty\(aq: {}, \(aqkeithley\(aq: {\(aqcurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqcurrent in A (datasource)\(aq}, \(aqgain\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgain in V/A (datasource)\(aq}, \(aqrisetime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqrise time (datasource)\(aq}, \(aqsourvoltlevel\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsource voltage level in V (datasource)\(aq}, \(aqvoltage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvoltage in V (datasource)\(aq}}, \(aqmaia\(aq: {\(aqchillersetpoint\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchiller set point temperature in Celsus (datasource)\(aq}, \(aqchiptemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdetector chip temperature sensor for maia in Celsus (datasource)\(aq}, \(aqgaintrimenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgaintrim enable status for maia (datasource)\(aq}, \(aqidentity\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsensor identity for maia (datasource)\(aq}, \(aqinterlockpressure\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock pressure for maia in mbar (datasource)\(aq}, \(aqleakagecurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleakage current sensor for maia in A (datasource)\(aq}, \(aqlineariseenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqlinearise enable status for maia (datasource)\(aq}, \(aqmaiadimensions\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia dimensions component name (component)\(aq}, \(aqmaiafluxes\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia fluxes component name (component)\(aq}, \(aqmaiastage\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia stage component name (component)\(aq}, \(aqmosfettemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmosfet temperature sensor for maia in Celsus (datasource)\(aq}, \(aqpeltiercurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpeltier current sensor for maia in A (datasource)\(aq}, \(aqphotonenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphoton enable status for maia (datasource)\(aq}, \(aqpileuprejectionenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpileup rejection enable status for maia (datasource)\(aq}, \(aqpixelenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel enable status for maia (datasource)\(aq}, \(aqpressure\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgas pressure in mbar (datasource)\(aq}, \(aqrunnumber\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqrun number of maia (datasource)\(aq}, \(aqstatus\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock status for maia (datasource)\(aq}, \(aqthrottleenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthrottle enable status for maia (datasource)\(aq}, \(aquptime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock uptime for maia (datasource)\(aq}, \(aqvoltagesetpoint\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvoltage set point temperature in Celsus (datasource)\(aq}, \(aqwatertemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqwater temperature sensor for maia in Celsus (datasource)\(aq}}, \(aqmaiadimension\(aq: {\(aqdetname\(aq: {\(aqdefault\(aq: \(aqmaia\(aq, \(aqdoc\(aq: \(aqdetector (alias) name (string)\(aq}, \(aqdimname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdimension name for maia (datasource)\(aq}, \(aqdname\(aq: {\(aqdefault\(aq: \(aqdimension\(aq, \(aqdoc\(aq: \(aqdimension name group (string)\(aq}, \(aqhysteresis\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel hysteresis of dimension for maia (datasource)\(aq}, \(aqnumberofpixels\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnumber of pixels of dimension for maia (datasource)\(aq}, \(aqorigin\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel origin of dimension for maia (datasource)\(aq}, \(aqpixelpitch\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel pitch of dimension for maia (datasource)\(aq}, \(aqpositionsource\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqposition source of dimension for maia (datasource)\(aq}, \(aqunit\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqposition units of dimension for maia (datasource)\(aq}}, \(aqmaiaflux\(aq: {\(aqcoefficient\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux coefficient  for maia (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqmaia\(aq, \(aqdoc\(aq: \(aqdetector (alias) name (string)\(aq}, \(aqfluxname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux name for maia (datasource)\(aq}, \(aqfname\(aq: {\(aqdefault\(aq: \(aqfluxdevice\(aq, \(aqdoc\(aq: \(aqflux name group (string)\(aq}, \(aqkeithleydevice\(aq: {\(aqdefault\(aq: \(aqkeithley\(aq, \(aqdoc\(aq: \(aqkeithley device name (string)\(aq}, \(aqsource\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux source for maia (datasource)\(aq}, \(aqunit\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux unit for maia (datasource)\(aq}, \(aqvfcfactor\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvfc conversion factor (datasource)\(aq}}, \(aqmsnsar\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana device name MANDATORY (string)\(aq}, \(aqvarname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnested sardana environment variable name  MANDATORY (string)\(aq}}, \(aqmssar\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmacroserver sardana device name MANDATORY (string)\(aq}, \(aqvarname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment variable name MANDATORY (string)\(aq}}, \(aqpinhole\(aq: {\(aqdiameter\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpinhole diameter (datasource)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqxsign\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: "horizontal position sign, e.g. \(aq\-\(aq (string)"}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}, \(aqz\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqalong the beam position (datasource)\(aq}, \(aqzname\(aq: {\(aqdefault\(aq: \(aqz\(aq, \(aqdoc\(aq: \(aqalong the beam position name (string)\(aq}}, \(aqpointdet\(aq: {\(aqdata\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdiode data (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqdetector\(aq, \(aqdoc\(aq: \(aqdetector group name (string)\(aq}}, \(aqqbpm\(aq: {\(aqdependsony\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqthe  depends_on y field value,  e.g. distance (string)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqfoil\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil type, i.e. standard <cpname>_foil (datasource)\(aq}, \(aqfoilpos\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil position MANDATORY (datasource)\(aq}, \(aqfoilposdict\(aq: {\(aqdefault\(aq: \(aq{"Ti": 43, "Ni": 23, "Out": 3}\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}}, \(aqsamplehkl\(aq: {\(aqh\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqh position in hkl space (datasource)\(aq}, \(aqk\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqk position in hkl space (datasource)\(aq}, \(aql\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aql position in hkl space (datasource)\(aq}, \(aqpsi\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpsi angle position of analyzer (datasource)\(aq}, \(aqsname\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqslit\(aq: {\(aqbottom\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbottom blade position (datasource)\(aq}, \(aqbottomclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbottom blade closed position (datasource)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqleft\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleft blade position (datasource)\(aq}, \(aqleftclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleft blade closed position (datasource)\(aq}, \(aqright\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqright blade position (datasource)\(aq}, \(aqrightclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqright blade closed position (datasource)\(aq}, \(aqtop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtop blade position (datasource)\(aq}, \(aqtopclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtop blade closed position (datasource)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: "transformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)"}, \(aqxgap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal gap (datasource)\(aq}, \(aqxoffdependson\(aq: {\(aqdefault\(aq: \(aqy_offset\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqxoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal offset (datasource)\(aq}, \(aqxoffsetcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal offset calibration (datasource)\(aq}, \(aqxoffsetcalibrationname\(aq: {\(aqdefault\(aq: \(aqx_offset_calibration\(aq, \(aqdoc\(aq: \(aqhorizontal offset calibration name (string)\(aq}, \(aqxoffsetname\(aq: {\(aqdefault\(aq: \(aqx_offset\(aq, \(aqdoc\(aq: \(aqhorizontal offset name (string)\(aq}, \(aqygap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical gap (datasource)\(aq}, \(aqyoffdependson\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqyoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertiacal offset (datasource)\(aq}, \(aqyoffsetcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertiacal offset calibration (datasource)\(aq}, \(aqyoffsetcalibrationname\(aq: {\(aqdefault\(aq: \(aqy_offset_calibration\(aq, \(aqdoc\(aq: \(aqvertiacal offset calibration name (string)\(aq}, \(aqyoffsetname\(aq: {\(aqdefault\(aq: \(aqy_offset\(aq, \(aqdoc\(aq: \(aqvertiacal offset name (string)\(aq}}, \(aqsource\(aq: {\(aqbeamcurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqring beam current (datasource)\(aq}, \(aqbunchmode\(aq: {\(aqdefault\(aq: \(aqMulti Bunch\(aq, \(aqdoc\(aq: \(aqbunch mode (string)\(aq}, \(aqnumberofbunches\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnumber of source bunches (datasource)\(aq}, \(aqsourceenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqring beam energy (datasource)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqundulator\(aq: {\(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance from the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name from the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator energy (datasource)\(aq}, \(aqgap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqseparation between opposing pairs of magnetic pole (datasource)\(aq}, \(aqgapunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqgap units (string)\(aq}, \(aqharmonic\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator harmonic (datasource)\(aq}, \(aqlength\(aq: {\(aqdefault\(aq: \(aq2\(aq, \(aqdoc\(aq: \(aqlength of insertion device in meters (string)\(aq}, \(aqshift\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator shift (datasource)\(aq}, \(aqshiftunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqshift units (string)\(aq}, \(aqspeed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator speed (datasource)\(aq}, \(aqspeedunits\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqspeed units (string)\(aq}, \(aqtaper\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgap difference between upstream and downstream ends of the insertion device (datasource)\(aq}, \(aqtaperunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqgap units (string)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: "transformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)"}, \(aqtype\(aq: {\(aqdefault\(aq: \(aqundulator\(aq, \(aqdoc\(aq: \(aqundulator or wiggler (string)\(aq}, \(aquname\(aq: {\(aqdefault\(aq: \(aqinsertion_device\(aq, \(aqdoc\(aq: \(aqinsertion_device group name (string)\(aq}}}
-(\fI\%dict\fP <\fI\%str\fP , \fI\%dict\fP <\fI\%str\fP , \fI\%str\fP > >)
-standard component template variables
-and its [default value, doc string]
 .UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.storeComponent(name, xml, server, mandatory=False)
-stores components in Configuration Server
 .INDENT 7.0
 .TP
-.B Parameters
-.INDENT 7.0
-.IP \(bu 2
-\fBname\fP (\fI\%str\fP) – component name
-.IP \(bu 2
-\fBxml\fP (\fI\%str\fP) – component xml string
-.IP \(bu 2
-\fBserver\fP (\fI\%str\fP) – configuration server
-.IP \(bu 2
-\fBmandatory\fP (\fI\%bool\fP) – set component as mandatory
+.B beamline:  \fI\%Union\fP[\fI\%str\fP,  \fI\%None\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
-.UNINDENT
-.UNINDENT
-.INDENT 0.0
-.TP
-.B nxstools.nxsdevicetools.storeDataSource(name, xml, server)
-stores datasources in Configuration Server
 .INDENT 7.0
 .TP
-.B Parameters
-.INDENT 7.0
-.IP \(bu 2
-\fBname\fP (\fI\%str\fP) – datasource name
-.IP \(bu 2
-\fBxml\fP (\fI\%str\fP) – datasource xml string
-.IP \(bu 2
-\fBserver\fP (\fI\%str\fP) – configuration server
-.UNINDENT
+.B collection:  \fI\%Union\fP[\fI\%str\fP,  \fI\%None\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
-.UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B nxstools.nxsdevicetools.twoDModules = [\(aqpilatus100k\(aq, \(aqpilatus300k\(aq, \(aqpilatus1m\(aq, \(aqpilatus2m\(aq, \(aqpilatus6m\(aq, \(aqpco4000\(aq, \(aqperkinelmerdetector\(aq, \(aqlambda\(aq, \(aqpedetector\(aq, \(aqperkinelmer\(aq, \(aqpco\(aq, \(aqpcoedge\(aq, \(aqmarccd\(aq, \(aqperkinelmer\(aq, \(aqlcxcamera\(aq, \(aqlimaccd\(aq, \(aqeigerpsi\(aq, \(aqeigerdectris\(aq]
-(\fI\%list\fP <\fI\%str\fP>) modules of 2d detectors
+.B data_policy:  \fI\%Union\fP[\fI\%str\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B nxstools.nxsdevicetools.xmlPackageHandler = <nxstools.nxsdevicetools.PackageHandler object>
-(\fI\%PackageHandler\fP) xml template package handler
+.B dataset:  \fI\%Union\fP[\fI\%str\fP,  \fI\%None\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
-.INDENT 0.0
+.INDENT 7.0
 .TP
-.B nxstools.nxsdevicetools.zeroDModules = [\(aqtip830\(aq]
-(\fI\%list\fP <\fI\%str\fP>) modules of 0D detectors
+.B name:  \fI\%Union\fP[\fI\%str\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
-.SS nxstools.filenamegenerator module
-.sp
-Filename generator
-.INDENT 0.0
-.TP
-.B class nxstools.filenamegenerator.FilenameGenerator(fname_template, start_index=0, stop_index=None)
-Bases: \fI\%object\fP
-.sp
-Generate image file names
-.sp
-(c) Copyright 2015 Eugen Wintersberger <\fI\%eugen.wintersberger@gmail.com\fP>
-(c) Copyright 2015 DESY
-This file is part of nx2img.
-.sp
-nx2img is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 2 of the License, or
-(at your option) any later version.
-.sp
-nx2img is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-.sp
-You should have received a copy of the GNU General Public License
-along with nx2img.  If not, see <\fI\%http://www.gnu.org/licenses/\fP>.
-.sp
-Generator class creating image file names.
 .INDENT 7.0
 .TP
-.B Parameters
-.INDENT 7.0
-.IP \(bu 2
-\fBfname_template\fP (\fI\%str\fP) – file name template
-.IP \(bu 2
-\fBstart_index\fP (\fI\%int\fP) – file start index
-.IP \(bu 2
-\fBstop_index\fP (\fI\%int\fP) – file stop index
-.UNINDENT
+.B number:  \fI\%Union\fP[\fI\%int\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
 .INDENT 7.0
 .TP
-.B file_index = None
-(\fI\%int\fP) file start index
+.B path:  \fI\%Union\fP[\fI\%str\fP,  \fI\%None\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
 .INDENT 7.0
 .TP
-.B file_template = None
-(\fI\%str\fP) file name template
+.B pk:  \fI\%Union\fP[\fI\%str\fP,  \fI\%None\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
 .INDENT 7.0
 .TP
-.B static from_slice(file_template)
-Static factory method to create a filename_generator instance
-from a sliced user input
+.B proposal:  \fI\%Union\fP[\fI\%str\fP,  \fI\%None\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
+.UNINDENT
 .INDENT 7.0
 .TP
-.B Parameters
-\fBfile_template\fP (\fI\%str\fP) – file template
-.TP
-.B Returns
-filename generator object
-.TP
-.B Return type
-\fI\%FilenameGenerator\fP
+.B session:  \fI\%Union\fP[\fI\%str\fP,  \fI\%None\fP,  ExpressionProxy]  =  <redis_om.model.model.ExpressionProxy object>
 .UNINDENT
 .UNINDENT
-.INDENT 7.0
+.INDENT 0.0
 .TP
-.B stop_index = None
-(\fI\%int\fP) file stop index
+.B nxstools.redisutils.getDataStore(redisURL)
 .UNINDENT
-.UNINDENT
-.SS nxstools.release module
-.sp
-NXS tools release version
 .SS Module contents
 .sp
 NXS tools
 .sp
 xml templates
 .INDENT 0.0
 .TP
-.B nxstools.xmltemplates.moduleMultiAttributes = {\(aqdalsa\(aq: [\(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqTriggerMode\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqExtendedExposure\(aq, \(aqBinComment\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqFramesReceived\(aq, \(aqFrameRate\(aq, \(aqFramesPerNXFile\(aq, \(aqNXFileCompression\(aq, \(aqTurboMode\(aq, \(aqImageEnc\(aq, \(aqViewingMode\(aq, \(aqThrashedBuffers\(aq, \(aqFramesToAcquire\(aq, \(aqAcquisitionFrameCount\(aq, \(aqAcquisitionMode\(aq, \(aqAcquisitionFrameMode\(aq, \(aqLinearityEqualizer\(aq, \(aqNrExposedFrames\(aq, \(aqNrOffsetFrames\(aq, \(aqOffset\(aq, \(aqPixelFormat\(aq, \(aqReadOutMode\(aq, \(aqStandby\(aq, \(aqSumScheme\(aq], \(aqeigerdectris\(aq: [\(aqTriggerMode\(aq, \(aqNbTriggers\(aq, \(aqDescription\(aq, \(aqNbImages\(aq, \(aqBitDepth\(aq, \(aqReadoutTime\(aq, \(aqCountTime\(aq, \(aqEnergyThreshold\(aq, \(aqFrameTime\(aq, \(aqRateCorrectionEnabled\(aq, \(aqFlatFieldEnabled\(aq, \(aqTemperature\(aq, \(aqAutoSummationEnabled\(aq, \(aqHumidity\(aq, \(aqPhotonEnergy\(aq, \(aqWavelength\(aq], \(aqlambda\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq], \(aqlambda2m\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqOpMode\(aq], \(aqlambdavds\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq], \(aqlimaccd\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqlimaccds\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqmaiadimension\(aq: [\(aqName\(aq, \(aqPositionSource\(aq, \(aqPixelPitch\(aq, \(aqPixelOrigin\(aq, \(aqPixelHysteresis\(aq, \(aqPositionUnit\(aq, \(aqPixelCoordExtent\(aq], \(aqmaiaflux\(aq: [\(aqFluxCoeff\(aq, \(aqFluxName\(aq, \(aqFluxUnit\(aq, \(aqFluxSource\(aq], \(aqmaiainterlock\(aq: [\(aqBiasPeltierInterlock\(aq, \(aqBiasPeltierInterlockUptime\(aq, \(aqPressure\(aq], \(aqmaialogger\(aq: [\(aqRunNumber\(aq], \(aqmaiaprocessing\(aq: [\(aqGaintrimEnable\(aq, \(aqLineariseEnable\(aq, \(aqPhotonEnable\(aq, \(aqPileupRejectEnable\(aq, \(aqPixelEnable\(aq, \(aqThrottleEnable\(aq], \(aqmaiasensor\(aq: [\(aqBiasVoltage\(aq, \(aqLeakageCurrent\(aq, \(aqPeltierCurrent\(aq, \(aqWaterTemperature\(aq, \(aqDetectorTemperature\(aq, \(aqMosfetTemperature\(aq, \(aqIdentity\(aq], \(aqmarccd\(aq: [\(aqFrameShift\(aq, \(aqSavingDirectory\(aq, \(aqSavingPostfix\(aq, \(aqSavingPrefix\(aq], \(aqmca_xia\(aq: [\(aqICR\(aq, \(aqOCR\(aq], \(aqmca_xia@pool\(aq: [\(aqCountsRoI\(aq, \(aqRoIEnd\(aq, \(aqRoIStart\(aq], \(aqmythen\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqRoI1\(aq, \(aqRoI2\(aq], \(aqmythen2\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqEnergy\(aq, \(aqNbFrames\(aq, \(aqRoI1End\(aq, \(aqRoI2End\(aq, \(aqRoI1Start\(aq, \(aqRoI2Start\(aq, \(aqThreshold\(aq], \(aqpco\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpco4000\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpcoedge\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpedetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmer\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmerdetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqpilatus\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus100k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus1m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus2m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus300k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus6m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqtangovimba\(aq: [\(aqWidth\(aq, \(aqWidthMax\(aq, \(aqTriggerSource\(aq, \(aqPixelFormat\(aq, \(aqOffsetY\(aq, \(aqOffsetX\(aq, \(aqHeightMax\(aq, \(aqHeight\(aq, \(aqGainRaw\(aq, \(aqExposureTimeAbs\(aq, \(aqAcquisitionFrameRateAbs\(aq, \(aqAcquisitionFrameRateLimit\(aq, \(aqStreamBytesPerSecond\(aq, \(aqBinComment\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqMaxLoad\(aq, \(aqReadMode\(aq, \(aqTuneMode\(aq, \(aqViewingMode\(aq]}
+.B nxstools.xmltemplates.moduleMultiAttributes  =  {\(aqcobold\(aq: [\(aqBinSize\(aq, \(aqExposureTime\(aq], \(aqdalsa\(aq: [\(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqTriggerMode\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqExtendedExposure\(aq, \(aqBinComment\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqFramesReceived\(aq, \(aqFrameRate\(aq, \(aqFramesPerNXFile\(aq, \(aqNXFileCompression\(aq, \(aqTurboMode\(aq, \(aqImageEnc\(aq, \(aqViewingMode\(aq, \(aqThrashedBuffers\(aq, \(aqFramesToAcquire\(aq, \(aqAcquisitionFrameCount\(aq, \(aqAcquisitionMode\(aq, \(aqAcquisitionFrameMode\(aq, \(aqLinearityEqualizer\(aq, \(aqNrExposedFrames\(aq, \(aqNrOffsetFrames\(aq, \(aqOffset\(aq, \(aqPixelFormat\(aq, \(aqReadOutMode\(aq, \(aqStandby\(aq, \(aqSumScheme\(aq], \(aqdalsavds\(aq: [\(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqTriggerMode\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqExtendedExposure\(aq, \(aqBinComment\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqFramesReceived\(aq, \(aqFrameRate\(aq, \(aqFramesPerNXFile\(aq, \(aqNXFileCompression\(aq, \(aqTurboMode\(aq, \(aqImageEnc\(aq, \(aqViewingMode\(aq, \(aqThrashedBuffers\(aq, \(aqFramesToAcquire\(aq, \(aqAcquisitionFrameCount\(aq, \(aqAcquisitionMode\(aq, \(aqAcquisitionFrameMode\(aq, \(aqLinearityEqualizer\(aq, \(aqNrExposedFrames\(aq, \(aqNrOffsetFrames\(aq, \(aqOffset\(aq, \(aqPixelFormat\(aq, \(aqReadOutMode\(aq, \(aqStandby\(aq, \(aqSumScheme\(aq], \(aqeigerdectris\(aq: [\(aqTriggerMode\(aq, \(aqNbTriggers\(aq, \(aqDescription\(aq, \(aqNbImages\(aq, \(aqBitDepth\(aq, \(aqReadoutTime\(aq, \(aqCountTime\(aq, \(aqEnergyThreshold\(aq, \(aqFrameTime\(aq, \(aqRateCorrectionEnabled\(aq, \(aqFlatFieldEnabled\(aq, \(aqTemperature\(aq, \(aqAutoSummationEnabled\(aq, \(aqHumidity\(aq, \(aqPhotonEnergy\(aq, \(aqWavelength\(aq], \(aqlambda\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq, \(aqTranslations\(aq], \(aqlambda2m\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqOpMode\(aq, \(aqTranslations\(aq], \(aqlambdavds\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq, \(aqTranslations\(aq], \(aqlambdavdsnm\(aq: [\(aqTriggerMode\(aq, \(aqShutterTime\(aq, \(aqDelayTime\(aq, \(aqFrameNumbers\(aq, \(aqThreadNo\(aq, \(aqEnergyThreshold\(aq, \(aqOperatingMode\(aq, \(aqConfigFilePath\(aq, \(aqSaveAllImages\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqFilePreExt\(aq, \(aqFilePostfix\(aq, \(aqSaveFilePath\(aq, \(aqSaveFileName\(aq, \(aqLatestImageNumber\(aq, \(aqLiveMode\(aq, \(aqTotalLossFrames\(aq, \(aqCompressorShuffle\(aq, \(aqCompressionRate\(aq, \(aqCompressionEnabled\(aq, \(aqLayout\(aq, \(aqShutterTimeMax\(aq, \(aqShutterTimeMin\(aq, \(aqWidth\(aq, \(aqHeight\(aq, \(aqDepth\(aq, \(aqLiveFrameNo\(aq, \(aqDistortionCorrection\(aq, \(aqLiveLastImageData\(aq, \(aqFramesPerFile\(aq, \(aqOpMode\(aq, \(aqTranslations\(aq], \(aqlimaccd\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqlimaccds\(aq: [\(aqcamera_type\(aq, \(aqcamera_pixelsize\(aq, \(aqcamera_model\(aq, \(aqacq_mode\(aq, \(aqacq_nb_frames\(aq, \(aqacq_trigger_mode\(aq, \(aqlast_image_saved\(aq, \(aqlatency_time\(aq, \(aqacc_max_expo_time\(aq, \(aqacc_expo_time\(aq, \(aqacc_time_mode\(aq, \(aqacc_dead_time\(aq, \(aqacc_live_time\(aq, \(aqsaving_mode\(aq, \(aqsaving_directory\(aq, \(aqsaving_prefix\(aq, \(aqsaving_suffix\(aq, \(aqsaving_next_number\(aq, \(aqsaving_format\(aq, \(aqsaving_frame_per_file\(aq, \(aqimage_type\(aq, \(aqimage_width\(aq, \(aqimage_height\(aq, \(aqimage_sizes\(aq, \(aqimage_roi\(aq, \(aqimage_bin\(aq, \(aqimage_flip\(aq, \(aqimage_rotation\(aq, \(aqshutter_mode\(aq, \(aqshutter_open_time\(aq], \(aqmaiadimension\(aq: [\(aqName\(aq, \(aqPositionSource\(aq, \(aqPixelPitch\(aq, \(aqPixelOrigin\(aq, \(aqPixelHysteresis\(aq, \(aqPositionUnit\(aq, \(aqPixelCoordExtent\(aq], \(aqmaiaflux\(aq: [\(aqFluxCoeff\(aq, \(aqFluxName\(aq, \(aqFluxUnit\(aq, \(aqFluxSource\(aq], \(aqmaiainterlock\(aq: [\(aqBiasPeltierInterlock\(aq, \(aqBiasPeltierInterlockUptime\(aq, \(aqPressure\(aq], \(aqmaialogger\(aq: [\(aqRunNumber\(aq], \(aqmaiaprocessing\(aq: [\(aqGaintrimEnable\(aq, \(aqLineariseEnable\(aq, \(aqPhotonEnable\(aq, \(aqPileupRejectEnable\(aq, \(aqPixelEnable\(aq, \(aqThrottleEnable\(aq], \(aqmaiasensor\(aq: [\(aqBiasVoltage\(aq, \(aqLeakageCurrent\(aq, \(aqPeltierCurrent\(aq, \(aqWaterTemperature\(aq, \(aqDetectorTemperature\(aq, \(aqMosfetTemperature\(aq, \(aqIdentity\(aq], \(aqmarccd\(aq: [\(aqFrameShift\(aq, \(aqSavingDirectory\(aq, \(aqSavingPostfix\(aq, \(aqSavingPrefix\(aq], \(aqmca_xia\(aq: [\(aqICR\(aq, \(aqOCR\(aq], \(aqmca_xia@pool\(aq: [\(aqCountsRoI\(aq, \(aqRoIEnd\(aq, \(aqRoIStart\(aq], \(aqmythen\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqRoI1\(aq, \(aqRoI2\(aq], \(aqmythen2\(aq: [\(aqCounts1\(aq, \(aqCounts2\(aq, \(aqCountsMax\(aq, \(aqCountsTotal\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFileIndex\(aq, \(aqFilePrefix\(aq, \(aqData\(aq, \(aqEnergy\(aq, \(aqNbFrames\(aq, \(aqRoI1End\(aq, \(aqRoI2End\(aq, \(aqRoI1Start\(aq, \(aqRoI2Start\(aq, \(aqThreshold\(aq], \(aqpco\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpco4000\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpcoedge\(aq: [\(aqDelayTime\(aq, \(aqExposureTime\(aq, \(aqNbFrames\(aq, \(aqTriggerMode\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqBinning_x\(aq, \(aqBinning_y\(aq, \(aqROI_x_min\(aq, \(aqROI_x_max\(aq, \(aqROI_y_min\(aq, \(aqROI_y_max\(aq, \(aqPixelrate\(aq, \(aqADCs\(aq, \(aqCoolingTemp\(aq, \(aqCoolingTempSet\(aq, \(aqImageTimeStamp\(aq, \(aqRecorderMode\(aq], \(aqpedetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmer\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqperkinelmerdetector\(aq: [\(aqBinningMode\(aq, \(aqFileIndex\(aq, \(aqExposureTime\(aq, \(aqSkippedAtStart\(aq, \(aqSummedSaveImages\(aq, \(aqSkippedBetweenSaved\(aq, \(aqFilesAfterTrigger\(aq, \(aqFilesBeforeTrigger\(aq, \(aqSummedDarkImages\(aq, \(aqOutputDirectory\(aq, \(aqFilePattern\(aq, \(aqFileName\(aq, \(aqLogFile\(aq, \(aqUserComment1\(aq, \(aqCameraGain\(aq, \(aqUserComment2\(aq, \(aqUserComment3\(aq, \(aqUserComment4\(aq, \(aqSaveRawImages\(aq, \(aqSaveDarkImages\(aq, \(aqPerformIntegration\(aq, \(aqSaveIntegratedData\(aq, \(aqSaveSubtracted\(aq, \(aqPerformDarkSubtraction\(aq], \(aqpilatus\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus100k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus1m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus2m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus300k\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqpilatus6m\(aq: [\(aqDelayTime\(aq, \(aqExposurePeriod\(aq, \(aqExposureTime\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileStartNum\(aq, \(aqLastImageTaken\(aq, \(aqNbExposures\(aq, \(aqNbFrames\(aq, \(aqMXparameters\(aq], \(aqtangovimba\(aq: [\(aqWidth\(aq, \(aqWidthMax\(aq, \(aqTriggerSource\(aq, \(aqPixelFormat\(aq, \(aqOffsetY\(aq, \(aqOffsetX\(aq, \(aqHeightMax\(aq, \(aqHeight\(aq, \(aqGainRaw\(aq, \(aqExposureTimeAbs\(aq, \(aqAcquisitionFrameRateAbs\(aq, \(aqAcquisitionFrameRateLimit\(aq, \(aqStreamBytesPerSecond\(aq, \(aqBinComment\(aq, \(aqFileDir\(aq, \(aqFilePostfix\(aq, \(aqFilePrefix\(aq, \(aqFileSaving\(aq, \(aqFileStartNum\(aq, \(aqFramesProcessed\(aq, \(aqImage16\(aq, \(aqImage8\(aq, \(aqImageRaw\(aq, \(aqMaxLoad\(aq, \(aqReadMode\(aq, \(aqTuneMode\(aq, \(aqViewingMode\(aq]}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
 important attributes of modules
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxstools.xmltemplates.moduleTemplateFiles = {\(aqdalsa\(aq: [\(aqdalsa.xml\(aq, \(aqdalsa_nxdata.ds.xml\(aq, \(aqdalsa_external_data.ds.xml\(aq], \(aqeigerdectris\(aq: [\(aqeigerdectris.xml\(aq, \(aqeigerdectris_stepindex.ds.xml\(aq, \(aqeigerdectris_description_cb.ds.xml\(aq, \(aqeigerdectris_triggermode_cb.ds.xml\(aq], \(aqlambda\(aq: [\(aqlambda.xml\(aq, \(aqlambda_nxdata.ds.xml\(aq, \(aqlambda_external_data.ds.xml\(aq], \(aqlambda2m\(aq: [\(aqlambda2m.xml\(aq, \(aqlambda2m_m1_nxdata.ds.xml\(aq, \(aqlambda2m_m2_nxdata.ds.xml\(aq, \(aqlambda2m_m3_nxdata.ds.xml\(aq, \(aqlambda2m_m1_external_data.ds.xml\(aq, \(aqlambda2m_m2_external_data.ds.xml\(aq, \(aqlambda2m_m3_external_data.ds.xml\(aq], \(aqlambdavds\(aq: [\(aqlambdavds.xml\(aq, \(aqlambdavds_nxdata.ds.xml\(aq, \(aqlambdavds_description.ds.xml\(aq, \(aqlambdavds_triggermode_cb.ds.xml\(aq, \(aqlambdavds_framenumbers_cb.ds.xml\(aq, \(aqlambdavds_savefilename_cb.ds.xml\(aq], \(aqlimaccd\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqlimaccds\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqmarccd\(aq: [\(aqmarccd.xml\(aq, \(aqmarccd_postrun.ds.xml\(aq], \(aqmca_xia\(aq: [\(aqmcaxia.xml\(aq], \(aqmythen\(aq: [\(aqmythen.xml\(aq, \(aqmythen_postrun.ds.xml\(aq, \(aqmythen_filestartnumber.ds.xml\(aq], \(aqmythen2\(aq: [\(aqmythen2.xml\(aq], \(aqpco\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpco4000\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpcoedge\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpedetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmer\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmerdetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqpilatus\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus100k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus100k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus1m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus1m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus2m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus300k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus300k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus6m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqtangovimba\(aq: [\(aqtangovimba.xml\(aq, \(aqtangovimba_nxdata.ds.xml\(aq, \(aqtangovimba_external_data.ds.xml\(aq]}
+.B nxstools.xmltemplates.moduleTemplateFiles  =  {\(aqcobold\(aq: [\(aqcobold.xml\(aq], \(aqdalsa\(aq: [\(aqdalsa.xml\(aq, \(aqdalsa_nxdata.ds.xml\(aq, \(aqdalsa_external_data.ds.xml\(aq], \(aqdalsavds\(aq: [\(aqdalsavds.xml\(aq, \(aqdalsavds_nxdata.ds.xml\(aq, \(aqdalsavds_triggermode_cb.ds.xml\(aq, \(aqdalsavds_filestartnum_cb.ds.xml\(aq, \(aqdalsavds_nrexposedframes_cb.ds.xml\(aq], \(aqeigerdectris\(aq: [\(aqeigerdectris.xml\(aq, \(aqeigerdectris_stepindex.ds.xml\(aq, \(aqeigerdectris_description_cb.ds.xml\(aq, \(aqeigerdectris_triggermode_cb.ds.xml\(aq], \(aqlambda\(aq: [\(aqlambda.xml\(aq, \(aqlambda_nxdata.ds.xml\(aq, \(aqlambda_external_data.ds.xml\(aq], \(aqlambda2m\(aq: [\(aqlambda2m.xml\(aq, \(aqlambda2m_m1_nxdata.ds.xml\(aq, \(aqlambda2m_m2_nxdata.ds.xml\(aq, \(aqlambda2m_m3_nxdata.ds.xml\(aq, \(aqlambda2m_m1_external_data.ds.xml\(aq, \(aqlambda2m_m2_external_data.ds.xml\(aq, \(aqlambda2m_m3_external_data.ds.xml\(aq], \(aqlambdavds\(aq: [\(aqlambdavds.xml\(aq, \(aqlambdavds_nxdata.ds.xml\(aq, \(aqlambdavds_description.ds.xml\(aq, \(aqlambdavds_triggermode_cb.ds.xml\(aq, \(aqlambdavds_framenumbers_cb.ds.xml\(aq, \(aqlambdavds_savefilename_cb.ds.xml\(aq], \(aqlambdavdsnm\(aq: [\(aqlambdavdsnm.xml\(aq, \(aqlambdavdsnm_triggermode_cb.ds.xml\(aq, \(aqlambdavdsnm_nxdata.ds.xml\(aq], \(aqlimaccd\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqlimaccds\(aq: [\(aqlimaccd.xml\(aq, \(aqlimaccd_postrun.ds.xml\(aq, \(aqlimaccd_xpixelsize.ds.xml\(aq, \(aqlimaccd_ypixelsize.ds.xml\(aq, \(aqlimaccd_description.ds.xml\(aq, \(aqlimaccd_filestartnum_cb.ds.xml\(aq], \(aqmarccd\(aq: [\(aqmarccd.xml\(aq, \(aqmarccd_postrun.ds.xml\(aq], \(aqmca_xia\(aq: [\(aqmcaxia.xml\(aq], \(aqmythen\(aq: [\(aqmythen.xml\(aq, \(aqmythen_postrun.ds.xml\(aq, \(aqmythen_filestartnumber.ds.xml\(aq], \(aqmythen2\(aq: [\(aqmythen2.xml\(aq], \(aqpco\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpco4000\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpcoedge\(aq: [\(aqpco.xml\(aq, \(aqpco_postrun.ds.xml\(aq, \(aqpco_description.ds.xml\(aq, \(aqpco_filestartnum_cb.ds.xml\(aq], \(aqpedetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmer\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqperkinelmerdetector\(aq: [\(aqperkinelmerdetector.xml\(aq, \(aqperkinelmerdetector_postrun.ds.xml\(aq, \(aqperkinelmerdetector_description.ds.xml\(aq, \(aqperkinelmerdetector_fileindex_cb.ds.xml\(aq], \(aqpilatus\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus100k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus100k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus1m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus1m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus2m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus300k\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus300k_description.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqpilatus6m\(aq: [\(aqpilatus.xml\(aq, \(aqpilatus_postrun.ds.xml\(aq, \(aqpilatus_mxparameters_cb.ds.xml\(aq, \(aqpilatus6m_description.ds.xml\(aq, \(aqpilatus_filestartnum_cb.ds.xml\(aq], \(aqtangovimba\(aq: [\(aqtangovimba.xml\(aq, \(aqtangovimba_nxdata.ds.xml\(aq, \(aqtangovimba_external_data.ds.xml\(aq]}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
 xml template files of modules
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxstools.xmltemplates.standardComponentTemplateFiles = {\(aqabsorber\(aq: [\(aqabsorber_foil.ds.xml\(aq, \(aqabsorber_thickness.ds.xml\(aq, \(aqabsorber.xml\(aq], \(aqbeamstop\(aq: [\(aqbeamstop.xml\(aq], \(aqbeamtimeid\(aq: [\(aqbeamtimeid.xml\(aq, \(aqbeamtimeid.ds.xml\(aq, \(aqstart_time.ds.xml\(aq], \(aqchcut\(aq: [\(aqchcut.xml\(aq, \(aqchcut_unitcalibration.ds.xml\(aq, \(aqchcut_crystal.ds.xml\(aq], \(aqcollect2\(aq: [\(aqcollect2.xml\(aq], \(aqcollect3\(aq: [\(aqcollect3.xml\(aq], \(aqcollect4\(aq: [\(aqcollect4.xml\(aq], \(aqcollect5\(aq: [\(aqcollect5.xml\(aq], \(aqcollect6\(aq: [\(aqcollect6.xml\(aq], \(aqcommon2\(aq: [\(aqcommon2_common.ds.xml\(aq], \(aqcommon3\(aq: [\(aqcommon3_common.ds.xml\(aq], \(aqdatasignal\(aq: [\(aqdatasignal.xml\(aq, \(aqdefaultsignal.ds.xml\(aq, \(aqsignal_name.ds.xml\(aq, \(aqsignalname.ds.xml\(aq, \(aqsignal_axes.ds.xml\(aq], \(aqdcm\(aq: [\(aqdcm.xml\(aq, \(aqdcm_reflection.ds.xml\(aq, \(aqdcm_unitcalibration.ds.xml\(aq, \(aqdcm_crystal.ds.xml\(aq], \(aqdefault\(aq: [\(aqdefault.xml\(aq, \(aqdefaultsample.xml\(aq, \(aqdefaultinstrument.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultinstrument\(aq: [\(aqdefaultinstrument.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultsample\(aq: [\(aqdefaultsample.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq], \(aqdetectorlive\(aq: [\(aqdetectorlive.xml\(aq], \(aqempty\(aq: [\(aqempty.xml\(aq], \(aqkeithley\(aq: [\(aqkeithley.xml\(aq], \(aqmaia\(aq: [\(aqmaia.xml\(aq, \(aqempty.xml\(aq], \(aqmaiadimension\(aq: [\(aqmaiadimension.xml\(aq], \(aqmaiaflux\(aq: [\(aqmaiaflux.xml\(aq], \(aqmsnsar\(aq: [\(aqmsnsar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqmssar\(aq: [\(aqmssar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqpinhole\(aq: [\(aqpinhole.xml\(aq], \(aqpointdet\(aq: [\(aqpointdet.xml\(aq], \(aqqbpm\(aq: [\(aqqbpm_foil.ds.xml\(aq, \(aqqbpm.xml\(aq], \(aqsamplehkl\(aq: [\(aqsamplehkl.xml\(aq], \(aqslit\(aq: [\(aqslit.xml\(aq], \(aqsource\(aq: [\(aqsource.xml\(aq], \(aqundulator\(aq: [\(aqundulator.xml\(aq]}
+.B nxstools.xmltemplates.standardComponentTemplateFiles  =  {\(aqabsorber\(aq: [\(aqabsorber_foil.ds.xml\(aq, \(aqabsorber_thickness.ds.xml\(aq, \(aqabsorber.xml\(aq], \(aqbeamstop\(aq: [\(aqbeamstop.xml\(aq], \(aqbeamtimefname\(aq: [\(aqbeamtimefname.xml\(aq, \(aqbeamtimefname.ds.xml\(aq, \(aqstart_time.ds.xml\(aq], \(aqbeamtimeid\(aq: [\(aqbeamtimeid.xml\(aq, \(aqbeamtimeid.ds.xml\(aq, \(aqstart_time.ds.xml\(aq], \(aqchcut\(aq: [\(aqchcut.xml\(aq, \(aqchcut_unitcalibration.ds.xml\(aq, \(aqchcut_crystal.ds.xml\(aq], \(aqcoboldhisto\(aq: [\(aqcoboldhisto.xml\(aq, \(aqcoboldhisto_timeofflight.ds.xml\(aq], \(aqcollect2\(aq: [\(aqcollect2.xml\(aq], \(aqcollect3\(aq: [\(aqcollect3.xml\(aq], \(aqcollect4\(aq: [\(aqcollect4.xml\(aq], \(aqcollect5\(aq: [\(aqcollect5.xml\(aq], \(aqcollect6\(aq: [\(aqcollect6.xml\(aq], \(aqcommon2\(aq: [\(aqcommon2_common.ds.xml\(aq], \(aqcommon3\(aq: [\(aqcommon3_common.ds.xml\(aq], \(aqdataaxessignal\(aq: [\(aqdataaxessignal.xml\(aq, \(aqdefaultsignal.ds.xml\(aq, \(aqdefaultaxes.ds.xml\(aq, \(aqsignal_name.ds.xml\(aq, \(aqsignalname.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqdatasignal\(aq: [\(aqdatasignal.xml\(aq, \(aqdefaultsignal.ds.xml\(aq, \(aqsignal_name.ds.xml\(aq, \(aqsignalname.ds.xml\(aq, \(aqsignal_axes.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqdcm\(aq: [\(aqdcm.xml\(aq, \(aqdcm_reflection.ds.xml\(aq, \(aqdcm_unitcalibration.ds.xml\(aq, \(aqdcm_crystal.ds.xml\(aq], \(aqdefault\(aq: [\(aqdefault.xml\(aq, \(aqdefaultsample.xml\(aq, \(aqdefaultinstrument.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqbeamtime_filename.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultinstrument\(aq: [\(aqdefaultinstrument.xml\(aq, \(aqbeamtime_id.ds.xml\(aq, \(aqbeamtime_filename.ds.xml\(aq, \(aqstart_time.ds.xml\(aq, \(aqend_time.ds.xml\(aq, \(aqnexdatas_version.ds.xml\(aq, \(aqnexdatas_configuration.ds.xml\(aq, \(aqtitle.ds.xml\(aq], \(aqdefaultsample\(aq: [\(aqdefaultsample.xml\(aq, \(aqsample_name.ds.xml\(aq, \(aqchemical_formula.ds.xml\(aq], \(aqdescription\(aq: [\(aqdescription.xml\(aq, \(aqexperiment_description.ds.xml\(aq], \(aqdescriptiontext\(aq: [\(aqdescriptiontext.xml\(aq], \(aqdetectorlive\(aq: [\(aqdetectorlive.xml\(aq], \(aqempty\(aq: [\(aqempty.xml\(aq], \(aqgroupsecop\(aq: [\(aqgroupsecop.ds.xml\(aq, \(aqgroupsecop_time.ds.xml\(aq, \(aqclient_start_time.ds.xml\(aq, \(aqsample_env_links.ds.xml\(aq, \(aqsample_log_links.ds.xml\(aq], \(aqkeithley\(aq: [\(aqkeithley.xml\(aq], \(aqmaia\(aq: [\(aqmaia.xml\(aq, \(aqempty.xml\(aq], \(aqmaiadimension\(aq: [\(aqmaiadimension.xml\(aq], \(aqmaiaflux\(aq: [\(aqmaiaflux.xml\(aq], \(aqmsnsar\(aq: [\(aqmsnsar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqmssar\(aq: [\(aqmssar_env.ds.xml\(aq, \(aqsardanaenvironment.ds.xml\(aq], \(aqparametercopymap\(aq: [\(aqparametercopymap.xml\(aq], \(aqpinhole\(aq: [\(aqpinhole.xml\(aq], \(aqpointdet\(aq: [\(aqpointdet.xml\(aq], \(aqqbpm\(aq: [\(aqqbpm_foil.ds.xml\(aq, \(aqqbpm.xml\(aq], \(aqsampledescription\(aq: [\(aqsampledescription.xml\(aq, \(aqsample_description.ds.xml\(aq], \(aqsampledescriptiontext\(aq: [\(aqsampledescriptiontext.xml\(aq], \(aqsamplehkl\(aq: [\(aqsamplehkl.xml\(aq], \(aqsecop\(aq: [\(aqsecop.ds.xml\(aq, \(aqsecop_time.ds.xml\(aq, \(aqclient_start_time.ds.xml\(aq, \(aqsample_env_links.ds.xml\(aq, \(aqsample_log_links.ds.xml\(aq], \(aqsecoplinks\(aq: [\(aqsample_env_links.ds.xml\(aq, \(aqsample_log_links.ds.xml\(aq, \(aqsample_nxdata.ds.xml\(aq, \(aqsampleenv_nxdata.ds.xml\(aq], \(aqsinglesecop\(aq: [\(aqsinglesecop.ds.xml\(aq, \(aqsinglesecop_time.ds.xml\(aq, \(aqclient_start_time.ds.xml\(aq, \(aqsample_env_links.ds.xml\(aq, \(aqsample_log_links.ds.xml\(aq], \(aqslit\(aq: [\(aqslit.xml\(aq], \(aqsource\(aq: [\(aqsource.xml\(aq], \(aqstarttime\(aq: [\(aqstarttime.xml\(aq, \(aqstarttime.ds.xml\(aq, \(aqstart_timestamp.ds.xml\(aq, \(aqclient_start_time.ds.xml\(aq], \(aqtango\(aq: [\(aqtango.ds.xml\(aq], \(aqundulator\(aq: [\(aqundulator.xml\(aq]}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%list\fP <\fI\%str\fP> >)
 xml template files of modules
 .UNINDENT
 .INDENT 0.0
 .TP
-.B nxstools.xmltemplates.standardComponentVariables = {\(aqabsorber\(aq: {\(aqattenfactor\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqattenuation factor (datasource)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqfoil\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil type, i.e. standard <cpname>_foil (datasource)\(aq}, \(aqfoillist\(aq: {\(aqdefault\(aq: \(aq["Ag", "Ag", "Ag", "Ag", "", "Al", "Al", "Al", "Al"]\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqposition\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqwhich sliders are in [bitarray] MANDATORY (datasource)\(aq}, \(aqthickness\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil thickness, i.e. standard <cpname>_thickness (datasource)\(aq}, \(aqthicknesslist\(aq: {\(aqdefault\(aq: \(aq[0.5, 0.05, 0.025, 0.0125, 0, 0.1, 0.3, 0.5, 1.0]\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: "transformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)"}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}}, \(aqbeamstop\(aq: {\(aqdescription\(aq: {\(aqdefault\(aq: \(aqcircular\(aq, \(aqdoc\(aq: \(aq circular or  rectangular (string)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqxsign\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: "horizontal position sign, e.g. \(aq\-\(aq (string)"}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}, \(aqz\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqzname\(aq: {\(aqdefault\(aq: \(aqz\(aq, \(aqdoc\(aq: \(aqalong the beam position name (string)\(aq}}, \(aqbeamtimeid\(aq: {\(aqcommissiondir\(aq: {\(aqdefault\(aq: \(aq/gpfs/commissioning\(aq, \(aqdoc\(aq: \(aqcommission file directory (string)\(aq}, \(aqcommissionpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqcommission file postfix (string)\(aq}, \(aqcommissionprefix\(aq: {\(aqdefault\(aq: \(aqcommissioning\-metadata\-\(aq, \(aqdoc\(aq: \(aqcommission file prefix (string)\(aq}, \(aqcurrentdir\(aq: {\(aqdefault\(aq: \(aq/gpfs/current\(aq, \(aqdoc\(aq: \(aqbeamtime file directory (string)\(aq}, \(aqcurrentpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqbeamtime file postfix (string)\(aq}, \(aqcurrentprefix\(aq: {\(aqdefault\(aq: \(aqbeamtime\-metadata\-\(aq, \(aqdoc\(aq: \(aqbeamtime file prefix (string)\(aq}, \(aqlocaldir\(aq: {\(aqdefault\(aq: \(aq/gpfs/local\(aq, \(aqdoc\(aq: \(aqlocal file directory (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}}, \(aqchcut\(aq: {\(aqbraggangle\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbragg angle (datasource)\(aq}, \(aqbragganglename\(aq: {\(aqdefault\(aq: \(aqbragg\(aq, \(aqdoc\(aq: \(aqbragg angle name  (string)\(aq}, \(aqchcutdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqFMBOxfDCMEnergy tango device name (string)\(aq}, \(aqcrystal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq type of crystal i.e. 0\->Si111,1\->Si311,2\->Si111 ChannelCut  (datasource)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsynchronized monochromator energy (datasource)\(aq}, \(aqenergyfmb\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmonochromator energy (datasource)\(aq}, \(aqjack1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfirst vertical jack of table (datasource)\(aq}, \(aqjack1name\(aq: {\(aqdefault\(aq: \(aqjack1\(aq, \(aqdoc\(aq: \(aqfirst vertical jack name of table (string)\(aq}, \(aqjack2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond vertical jack of table (datasource)\(aq}, \(aqjack2name\(aq: {\(aqdefault\(aq: \(aqjack2\(aq, \(aqdoc\(aq: \(aqsecond vertical jack name of table (string)\(aq}, \(aqjack3\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthird vertical jack of table (datasource)\(aq}, \(aqjack3name\(aq: {\(aqdefault\(aq: \(aqjack3\(aq, \(aqdoc\(aq: \(aqthird vertical jack name of table (string)\(aq}, \(aqlat\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the first cristal (datasource)\(aq}, \(aqlatname\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the first cristal (string)\(aq}, \(aqoxfordhorizontal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq horizontal translation (datasource)\(aq}, \(aqpara\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance between the crystals (string)\(aq}, \(aqparaname\(aq: {\(aqdefault\(aq: \(aqpara\(aq, \(aqdoc\(aq: \(aqbeam parallel translation name of the second cristal (string)\(aq}, \(aqreflection\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqreflection from string (datasource)\(aq}, \(aqtable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position of table (datasource)\(aq}, \(aqtablename\(aq: {\(aqdefault\(aq: \(aqtable\(aq, \(aqdoc\(aq: \(aqvertical position name of table (string)\(aq}, \(aqtheta\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta angle (datasource)\(aq}, \(aqthetaname\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta angle name (string)\(aq}, \(aqunitcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq unit calibration from dcmmotor (datasource)\(aq}, \(aqusage\(aq: {\(aqdefault\(aq: \(aqBragg\(aq, \(aqdoc\(aq: \(aqthe crystall usage, e.g. Laue (string)\(aq}, \(aqyaw\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the first cristal (datasource)\(aq}, \(aqyawname\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the first cristal (string)\(aq}}, \(aqcollect2\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}}, \(aqcollect3\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect4\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect5\(aq: {\(aqfifth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fifth component to collect MANDATORY (datasource)\(aq}, \(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect6\(aq: {\(aqfifth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fifth component to collect MANDATORY (datasource)\(aq}, \(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqsixth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the sixth component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcommon2\(aq: {\(aqdds\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdefault read datasource name MANDATORY (datasource)\(aq}, \(aqods\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqoptional detasource name MANDATORY (datasource)\(aq}}, \(aqcommon3\(aq: {\(aqdds\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdefault read datasource name MANDATORY (datasource)\(aq}, \(aqods1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfist optional detasource name MANDATORY (datasource)\(aq}, \(aqods2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond optional detasource name MANDATORY (datasource)\(aq}}, \(aqdatasignal\(aq: {\(aqaxes\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdata axes field name(s) (string)\(aq}, \(aqsignal\(aq: {\(aqdefault\(aq: \(aqdefaultsignal\(aq, \(aqdoc\(aq: \(aqdata signal field name (string)\(aq}}, \(aqdcm\(aq: {\(aqbend1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbending of the first cristal (datasource)\(aq}, \(aqbend2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbending of the second cristal (datasource)\(aq}, \(aqbraggangle\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbragg angle (datasource)\(aq}, \(aqbragganglename\(aq: {\(aqdefault\(aq: \(aqbragg\(aq, \(aqdoc\(aq: \(aqbragg angle name  (string)\(aq}, \(aqchi2dependson\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqthe depends_on field of the second cristal chi, e.g. phi (string)\(aq}, \(aqcrystal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtype of crystal i.e. 0\->Si111,1\->Si311,2\->Si111 ChannelCut (datasource)\(aq}, \(aqdcmdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqFMBOxfDCMEnergy tango device (string)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsynchronized monochromator energy (datasource)\(aq}, \(aqenergyfmb\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmonochromator energy (datasource)\(aq}, \(aqexitoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq exit offset (datasource)\(aq}, \(aqjack1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfirst vertical jack of table (datasource)\(aq}, \(aqjack1name\(aq: {\(aqdefault\(aq: \(aqjack1\(aq, \(aqdoc\(aq: \(aqfirst vertical jack name of table (string)\(aq}, \(aqjack2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond vertical jack of table (datasource)\(aq}, \(aqjack2name\(aq: {\(aqdefault\(aq: \(aqjack2\(aq, \(aqdoc\(aq: \(aqsecond vertical jack name of table (string)\(aq}, \(aqjack3\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthird vertical jack of table (datasource)\(aq}, \(aqjack3name\(aq: {\(aqdefault\(aq: \(aqjack3\(aq, \(aqdoc\(aq: \(aqthird vertical jack name of table (string)\(aq}, \(aqlat\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the first cristal (datasource)\(aq}, \(aqlat2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the second cristal (datasource)\(aq}, \(aqlat2name\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the second cristal (string)\(aq}, \(aqlatname\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the first cristal (string)\(aq}, \(aqoxfordhorizontal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq horizontal translation (datasource)\(aq}, \(aqpar2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbeam parallel translation of the second cristal (datasource)\(aq}, \(aqpar2name\(aq: {\(aqdefault\(aq: \(aqpara\(aq, \(aqdoc\(aq: \(aqbeam parallel translation name of the second cristal (string)\(aq}, \(aqperp2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical translation of the second cristal (datasource)\(aq}, \(aqperp2name\(aq: {\(aqdefault\(aq: \(aqperp\(aq, \(aqdoc\(aq: \(aqvertical translation name of the second cristal (string)\(aq}, \(aqphi1dependson\(aq: {\(aqdefault\(aq: \(aq../../transformations/bragg\(aq, \(aqdoc\(aq: \(aqthe depends_on field of the first cristal phi, e.g. theta (string)\(aq}, \(aqpitch1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta rotation of the first cristal (datasource)\(aq}, \(aqpitch1name\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta rotation name of the first cristal (string)\(aq}, \(aqpitch2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta rotation of the second cristal (datasource)\(aq}, \(aqpitch2name\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta rotation name of the second cristal (string)\(aq}, \(aqroll1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchi rotation of the first cristal (datasource)\(aq}, \(aqroll1name\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqchi rotation name of the first cristal (string)\(aq}, \(aqroll2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchi rotation of the second cristal (datasource)\(aq}, \(aqroll2name\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqchi rotation name of the second cristal (string)\(aq}, \(aqtable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position of table (datasource)\(aq}, \(aqtablename\(aq: {\(aqdefault\(aq: \(aqtable\(aq, \(aqdoc\(aq: \(aqvertical position name of table (string)\(aq}, \(aqtheta\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta angle (datasource)\(aq}, \(aqthetaname\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta angle name (string)\(aq}, \(aqtopdependson2\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqthe first transformation of the second crystal, e.g. lat (string)\(aq}, \(aqunitcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqunit calibration from dcmmotor (datasource)\(aq}, \(aqusage\(aq: {\(aqdefault\(aq: \(aqBragg\(aq, \(aqdoc\(aq: \(aqthe crystall usage, e.g. Laue (string)\(aq}, \(aqyaw\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the first cristal (datasource)\(aq}, \(aqyaw2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the second cristal (datasource)\(aq}, \(aqyaw2name\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the second cristal (string)\(aq}, \(aqyawname\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the first cristal (string)\(aq}}, \(aqdefault\(aq: {\(aq__configdevice__\(aq: {\(aqdefault\(aq: \(aqnxs/configserver/localhost\(aq, \(aqdoc\(aq: \(aqconfiguration server device name (string)\(aq}, \(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqcontrol\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgroup name of the monitor (string)\(aq}, \(aqlongname\(aq: {\(aqdefault\(aq: \(aqP09 Resonant Scattering and Diffraction beamline\(aq, \(aqdoc\(aq: \(aqbeamline long name (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}, \(aqsourcename\(aq: {\(aqdefault\(aq: \(aqPETRA III\(aq, \(aqdoc\(aq: \(aqsource name (string)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqdefaultinstrument\(aq: {\(aq__configdevice__\(aq: {\(aqdefault\(aq: \(aqnxs/configserver/localhost\(aq, \(aqdoc\(aq: \(aqconfiguration server device name (string)\(aq}, \(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqcontrol\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgroup name of the monitor (string)\(aq}, \(aqlongname\(aq: {\(aqdefault\(aq: \(aqP09 Resonant Scattering and Diffraction beamline\(aq, \(aqdoc\(aq: \(aqbeamline long name (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}, \(aqsourcename\(aq: {\(aqdefault\(aq: \(aqPETRA III\(aq, \(aqdoc\(aq: \(aqsource name (string)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqdefaultsample\(aq: {}, \(aqdetectorlive\(aq: {\(aqdatatype\(aq: {\(aqdefault\(aq: \(aqNX_UINT32\(aq, \(aqdoc\(aq: \(aqlist of devices (string)\(aq}, \(aqdetectordata\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdetector live data (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqdetector\(aq, \(aqdoc\(aq: \(aqlist of devices (string)\(aq}}, \(aqempty\(aq: {}, \(aqkeithley\(aq: {\(aqcurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqcurrent in A (datasource)\(aq}, \(aqgain\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgain in V/A (datasource)\(aq}, \(aqrisetime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqrise time (datasource)\(aq}, \(aqsourvoltlevel\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsource voltage level in V (datasource)\(aq}, \(aqvoltage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvoltage in V (datasource)\(aq}}, \(aqmaia\(aq: {\(aqchillersetpoint\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchiller set point temperature in Celsus (datasource)\(aq}, \(aqchiptemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdetector chip temperature sensor for maia in Celsus (datasource)\(aq}, \(aqgaintrimenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgaintrim enable status for maia (datasource)\(aq}, \(aqidentity\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsensor identity for maia (datasource)\(aq}, \(aqinterlockpressure\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock pressure for maia in mbar (datasource)\(aq}, \(aqleakagecurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleakage current sensor for maia in A (datasource)\(aq}, \(aqlineariseenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqlinearise enable status for maia (datasource)\(aq}, \(aqmaiadimensions\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia dimensions component name (component)\(aq}, \(aqmaiafluxes\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia fluxes component name (component)\(aq}, \(aqmaiastage\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia stage component name (component)\(aq}, \(aqmosfettemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmosfet temperature sensor for maia in Celsus (datasource)\(aq}, \(aqpeltiercurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpeltier current sensor for maia in A (datasource)\(aq}, \(aqphotonenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphoton enable status for maia (datasource)\(aq}, \(aqpileuprejectionenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpileup rejection enable status for maia (datasource)\(aq}, \(aqpixelenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel enable status for maia (datasource)\(aq}, \(aqpressure\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgas pressure in mbar (datasource)\(aq}, \(aqrunnumber\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqrun number of maia (datasource)\(aq}, \(aqstatus\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock status for maia (datasource)\(aq}, \(aqthrottleenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthrottle enable status for maia (datasource)\(aq}, \(aquptime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock uptime for maia (datasource)\(aq}, \(aqvoltagesetpoint\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvoltage set point temperature in Celsus (datasource)\(aq}, \(aqwatertemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqwater temperature sensor for maia in Celsus (datasource)\(aq}}, \(aqmaiadimension\(aq: {\(aqdetname\(aq: {\(aqdefault\(aq: \(aqmaia\(aq, \(aqdoc\(aq: \(aqdetector (alias) name (string)\(aq}, \(aqdimname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdimension name for maia (datasource)\(aq}, \(aqdname\(aq: {\(aqdefault\(aq: \(aqdimension\(aq, \(aqdoc\(aq: \(aqdimension name group (string)\(aq}, \(aqhysteresis\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel hysteresis of dimension for maia (datasource)\(aq}, \(aqnumberofpixels\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnumber of pixels of dimension for maia (datasource)\(aq}, \(aqorigin\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel origin of dimension for maia (datasource)\(aq}, \(aqpixelpitch\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel pitch of dimension for maia (datasource)\(aq}, \(aqpositionsource\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqposition source of dimension for maia (datasource)\(aq}, \(aqunit\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqposition units of dimension for maia (datasource)\(aq}}, \(aqmaiaflux\(aq: {\(aqcoefficient\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux coefficient  for maia (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqmaia\(aq, \(aqdoc\(aq: \(aqdetector (alias) name (string)\(aq}, \(aqfluxname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux name for maia (datasource)\(aq}, \(aqfname\(aq: {\(aqdefault\(aq: \(aqfluxdevice\(aq, \(aqdoc\(aq: \(aqflux name group (string)\(aq}, \(aqkeithleydevice\(aq: {\(aqdefault\(aq: \(aqkeithley\(aq, \(aqdoc\(aq: \(aqkeithley device name (string)\(aq}, \(aqsource\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux source for maia (datasource)\(aq}, \(aqunit\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux unit for maia (datasource)\(aq}, \(aqvfcfactor\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvfc conversion factor (datasource)\(aq}}, \(aqmsnsar\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana device name MANDATORY (string)\(aq}, \(aqvarname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnested sardana environment variable name  MANDATORY (string)\(aq}}, \(aqmssar\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmacroserver sardana device name MANDATORY (string)\(aq}, \(aqvarname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment variable name MANDATORY (string)\(aq}}, \(aqpinhole\(aq: {\(aqdiameter\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpinhole diameter (datasource)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqxsign\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: "horizontal position sign, e.g. \(aq\-\(aq (string)"}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}, \(aqz\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqalong the beam position (datasource)\(aq}, \(aqzname\(aq: {\(aqdefault\(aq: \(aqz\(aq, \(aqdoc\(aq: \(aqalong the beam position name (string)\(aq}}, \(aqpointdet\(aq: {\(aqdata\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdiode data (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqdetector\(aq, \(aqdoc\(aq: \(aqdetector group name (string)\(aq}}, \(aqqbpm\(aq: {\(aqdependsony\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqthe  depends_on y field value,  e.g. distance (string)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqfoil\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil type, i.e. standard <cpname>_foil (datasource)\(aq}, \(aqfoilpos\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil position MANDATORY (datasource)\(aq}, \(aqfoilposdict\(aq: {\(aqdefault\(aq: \(aq{"Ti": 43, "Ni": 23, "Out": 3}\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}}, \(aqsamplehkl\(aq: {\(aqh\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqh position in hkl space (datasource)\(aq}, \(aqk\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqk position in hkl space (datasource)\(aq}, \(aql\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aql position in hkl space (datasource)\(aq}, \(aqpsi\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpsi angle position of analyzer (datasource)\(aq}, \(aqsname\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqslit\(aq: {\(aqbottom\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbottom blade position (datasource)\(aq}, \(aqbottomclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbottom blade closed position (datasource)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqleft\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleft blade position (datasource)\(aq}, \(aqleftclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleft blade closed position (datasource)\(aq}, \(aqright\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqright blade position (datasource)\(aq}, \(aqrightclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqright blade closed position (datasource)\(aq}, \(aqtop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtop blade position (datasource)\(aq}, \(aqtopclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtop blade closed position (datasource)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: "transformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)"}, \(aqxgap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal gap (datasource)\(aq}, \(aqxoffdependson\(aq: {\(aqdefault\(aq: \(aqy_offset\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqxoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal offset (datasource)\(aq}, \(aqxoffsetcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal offset calibration (datasource)\(aq}, \(aqxoffsetcalibrationname\(aq: {\(aqdefault\(aq: \(aqx_offset_calibration\(aq, \(aqdoc\(aq: \(aqhorizontal offset calibration name (string)\(aq}, \(aqxoffsetname\(aq: {\(aqdefault\(aq: \(aqx_offset\(aq, \(aqdoc\(aq: \(aqhorizontal offset name (string)\(aq}, \(aqygap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical gap (datasource)\(aq}, \(aqyoffdependson\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqyoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertiacal offset (datasource)\(aq}, \(aqyoffsetcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertiacal offset calibration (datasource)\(aq}, \(aqyoffsetcalibrationname\(aq: {\(aqdefault\(aq: \(aqy_offset_calibration\(aq, \(aqdoc\(aq: \(aqvertiacal offset calibration name (string)\(aq}, \(aqyoffsetname\(aq: {\(aqdefault\(aq: \(aqy_offset\(aq, \(aqdoc\(aq: \(aqvertiacal offset name (string)\(aq}}, \(aqsource\(aq: {\(aqbeamcurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqring beam current (datasource)\(aq}, \(aqbunchmode\(aq: {\(aqdefault\(aq: \(aqMulti Bunch\(aq, \(aqdoc\(aq: \(aqbunch mode (string)\(aq}, \(aqnumberofbunches\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnumber of source bunches (datasource)\(aq}, \(aqsourceenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqring beam energy (datasource)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqundulator\(aq: {\(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance from the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name from the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator energy (datasource)\(aq}, \(aqgap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqseparation between opposing pairs of magnetic pole (datasource)\(aq}, \(aqgapunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqgap units (string)\(aq}, \(aqharmonic\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator harmonic (datasource)\(aq}, \(aqlength\(aq: {\(aqdefault\(aq: \(aq2\(aq, \(aqdoc\(aq: \(aqlength of insertion device in meters (string)\(aq}, \(aqshift\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator shift (datasource)\(aq}, \(aqshiftunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqshift units (string)\(aq}, \(aqspeed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator speed (datasource)\(aq}, \(aqspeedunits\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqspeed units (string)\(aq}, \(aqtaper\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgap difference between upstream and downstream ends of the insertion device (datasource)\(aq}, \(aqtaperunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqgap units (string)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: "transformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)"}, \(aqtype\(aq: {\(aqdefault\(aq: \(aqundulator\(aq, \(aqdoc\(aq: \(aqundulator or wiggler (string)\(aq}, \(aquname\(aq: {\(aqdefault\(aq: \(aqinsertion_device\(aq, \(aqdoc\(aq: \(aqinsertion_device group name (string)\(aq}}}
+.B nxstools.xmltemplates.standardComponentVariables  =  {\(aqabsorber\(aq: {\(aqattenfactor\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqattenuation factor (datasource)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqfoil\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil type, i.e. standard <cpname>_foil (datasource)\(aq}, \(aqfoillist\(aq: {\(aqdefault\(aq: \(aq[\(dqAg\(dq, \(dqAg\(dq, \(dqAg\(dq, \(dqAg\(dq, \(dq\(dq, \(dqAl\(dq, \(dqAl\(dq, \(dqAl\(dq, \(dqAl\(dq]\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqposition\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqwhich sliders are in [bitarray] MANDATORY (datasource)\(aq}, \(aqthickness\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil thickness, i.e. standard <cpname>_thickness (datasource)\(aq}, \(aqthicknesslist\(aq: {\(aqdefault\(aq: \(aq[0.5, 0.05, 0.025, 0.0125, 0, 0.1, 0.3, 0.5, 1.0]\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(dqtransformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)\(dq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}}, \(aqbeamstop\(aq: {\(aqdescription\(aq: {\(aqdefault\(aq: \(aqcircular\(aq, \(aqdoc\(aq: \(aq circular or  rectangular (string)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqxsign\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(dqhorizontal position sign, e.g. \(aq\-\(aq (string)\(dq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}, \(aqz\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqzname\(aq: {\(aqdefault\(aq: \(aqz\(aq, \(aqdoc\(aq: \(aqalong the beam position name (string)\(aq}}, \(aqbeamtimefname\(aq: {\(aqcommissiondir\(aq: {\(aqdefault\(aq: \(aq/gpfs/commissioning\(aq, \(aqdoc\(aq: \(aqcommission file directory (string)\(aq}, \(aqcommissionpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqcommission file postfix (string)\(aq}, \(aqcommissionprefix\(aq: {\(aqdefault\(aq: \(aqcommissioning\-metadata\-\(aq, \(aqdoc\(aq: \(aqcommission file prefix (string)\(aq}, \(aqcurrentdir\(aq: {\(aqdefault\(aq: \(aq/gpfs/current\(aq, \(aqdoc\(aq: \(aqbeamtime file directory (string)\(aq}, \(aqcurrentpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqbeamtime file postfix (string)\(aq}, \(aqcurrentprefix\(aq: {\(aqdefault\(aq: \(aqbeamtime\-metadata\-\(aq, \(aqdoc\(aq: \(aqbeamtime file prefix (string)\(aq}, \(aqlocaldir\(aq: {\(aqdefault\(aq: \(aq/gpfs/local\(aq, \(aqdoc\(aq: \(aqlocal file directory (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}}, \(aqbeamtimeid\(aq: {\(aqcommissiondir\(aq: {\(aqdefault\(aq: \(aq/gpfs/commissioning\(aq, \(aqdoc\(aq: \(aqcommission file directory (string)\(aq}, \(aqcommissionpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqcommission file postfix (string)\(aq}, \(aqcommissionprefix\(aq: {\(aqdefault\(aq: \(aqcommissioning\-metadata\-\(aq, \(aqdoc\(aq: \(aqcommission file prefix (string)\(aq}, \(aqcurrentdir\(aq: {\(aqdefault\(aq: \(aq/gpfs/current\(aq, \(aqdoc\(aq: \(aqbeamtime file directory (string)\(aq}, \(aqcurrentpostfix\(aq: {\(aqdefault\(aq: \(aq.json\(aq, \(aqdoc\(aq: \(aqbeamtime file postfix (string)\(aq}, \(aqcurrentprefix\(aq: {\(aqdefault\(aq: \(aqbeamtime\-metadata\-\(aq, \(aqdoc\(aq: \(aqbeamtime file prefix (string)\(aq}, \(aqlocaldir\(aq: {\(aqdefault\(aq: \(aq/gpfs/local\(aq, \(aqdoc\(aq: \(aqlocal file directory (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}}, \(aqchcut\(aq: {\(aqbraggangle\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbragg angle (datasource)\(aq}, \(aqbragganglename\(aq: {\(aqdefault\(aq: \(aqbragg\(aq, \(aqdoc\(aq: \(aqbragg angle name  (string)\(aq}, \(aqchcutdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqFMBOxfDCMEnergy tango device name (string)\(aq}, \(aqcrystal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq type of crystal i.e. 0\->Si111,1\->Si311,2\->Si111 ChannelCut  (datasource)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsynchronized monochromator energy (datasource)\(aq}, \(aqenergyfmb\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmonochromator energy (datasource)\(aq}, \(aqjack1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfirst vertical jack of table (datasource)\(aq}, \(aqjack1name\(aq: {\(aqdefault\(aq: \(aqjack1\(aq, \(aqdoc\(aq: \(aqfirst vertical jack name of table (string)\(aq}, \(aqjack2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond vertical jack of table (datasource)\(aq}, \(aqjack2name\(aq: {\(aqdefault\(aq: \(aqjack2\(aq, \(aqdoc\(aq: \(aqsecond vertical jack name of table (string)\(aq}, \(aqjack3\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthird vertical jack of table (datasource)\(aq}, \(aqjack3name\(aq: {\(aqdefault\(aq: \(aqjack3\(aq, \(aqdoc\(aq: \(aqthird vertical jack name of table (string)\(aq}, \(aqlat\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the first cristal (datasource)\(aq}, \(aqlatname\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the first cristal (string)\(aq}, \(aqoxfordhorizontal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq horizontal translation (datasource)\(aq}, \(aqpara\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance between the crystals (string)\(aq}, \(aqparaname\(aq: {\(aqdefault\(aq: \(aqpara\(aq, \(aqdoc\(aq: \(aqbeam parallel translation name of the second cristal (string)\(aq}, \(aqreflection\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqreflection from string (datasource)\(aq}, \(aqtable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position of table (datasource)\(aq}, \(aqtablename\(aq: {\(aqdefault\(aq: \(aqtable\(aq, \(aqdoc\(aq: \(aqvertical position name of table (string)\(aq}, \(aqtheta\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta angle (datasource)\(aq}, \(aqthetaname\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta angle name (string)\(aq}, \(aqunitcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq unit calibration from dcmmotor (datasource)\(aq}, \(aqusage\(aq: {\(aqdefault\(aq: \(aqBragg\(aq, \(aqdoc\(aq: \(aqthe crystall usage, e.g. Laue (string)\(aq}, \(aqyaw\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the first cristal (datasource)\(aq}, \(aqyawname\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the first cristal (string)\(aq}}, \(aqcoboldhisto\(aq: {\(aqbinsize\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbin size of histogram data (datasource)\(aq}, \(aqexposuretime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqexposure time for histogram data (datasource)\(aq}, \(aqhistogram\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhistogram data (datasource)\(aq}}, \(aqcollect2\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}}, \(aqcollect3\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect4\(aq: {\(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect5\(aq: {\(aqfifth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fifth component to collect MANDATORY (datasource)\(aq}, \(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcollect6\(aq: {\(aqfifth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fifth component to collect MANDATORY (datasource)\(aq}, \(aqfirst\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the first component to collect MANDATORY (datasource)\(aq}, \(aqfourth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the fourth component to collect MANDATORY (datasource)\(aq}, \(aqsecond\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the second component to collect MANDATORY (datasource)\(aq}, \(aqsixth\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the sixth component to collect MANDATORY (datasource)\(aq}, \(aqthird\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqname of the third component to collect MANDATORY (datasource)\(aq}}, \(aqcommon2\(aq: {\(aqdds\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdefault read datasource name MANDATORY (datasource)\(aq}, \(aqods\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqoptional detasource name MANDATORY (datasource)\(aq}}, \(aqcommon3\(aq: {\(aqdds\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdefault read datasource name MANDATORY (datasource)\(aq}, \(aqods1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfist optional detasource name MANDATORY (datasource)\(aq}, \(aqods2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond optional detasource name MANDATORY (datasource)\(aq}}, \(aqdataaxessignal\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqaxes\(aq: {\(aqdefault\(aq: \(aqdefaultaxes\(aq, \(aqdoc\(aq: \(aqlist of data axes field names (datasource)\(aq}, \(aqdefaultattrs\(aq: {\(aqdefault\(aq: \(aqFalse\(aq, \(aqdoc\(aq: \(aqadd default attributes (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmacroserver sardana device name MANDATORY (string)\(aq}, \(aqnchannelstoskip\(aq: {\(aqdefault\(aq: \(aq0\(aq, \(aqdoc\(aq: \(aqnumber of mg channels to skip (string)\(aq}, \(aqsardanasignal\(aq: {\(aqdefault\(aq: \(aqSignalCounter\(aq, \(aqdoc\(aq: \(aqsignal sardana variable name (string)\(aq}, \(aqsignal\(aq: {\(aqdefault\(aq: \(aqdefaultsignal\(aq, \(aqdoc\(aq: \(aqdata signal field name (datasource)\(aq}}, \(aqdatasignal\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqaxes\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdata axes field name(s) (datasource)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmacroserver sardana device name MANDATORY (string)\(aq}, \(aqnchannelstoskip\(aq: {\(aqdefault\(aq: \(aq0\(aq, \(aqdoc\(aq: \(aqnumber of mg channels to skip (string)\(aq}, \(aqsardanasignal\(aq: {\(aqdefault\(aq: \(aqSignalCounter\(aq, \(aqdoc\(aq: \(aqsignal sardana variable name (string)\(aq}, \(aqsignal\(aq: {\(aqdefault\(aq: \(aqdefaultsignal\(aq, \(aqdoc\(aq: \(aqdata signal field name (datasource)\(aq}}, \(aqdcm\(aq: {\(aqbend1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbending of the first cristal (datasource)\(aq}, \(aqbend2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbending of the second cristal (datasource)\(aq}, \(aqbraggangle\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbragg angle (datasource)\(aq}, \(aqbragganglename\(aq: {\(aqdefault\(aq: \(aqbragg\(aq, \(aqdoc\(aq: \(aqbragg angle name  (string)\(aq}, \(aqchi2dependson\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqthe depends_on field of the second cristal chi, e.g. phi (string)\(aq}, \(aqcrystal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtype of crystal i.e. 0\->Si111,1\->Si311,2\->Si111 ChannelCut (datasource)\(aq}, \(aqdcmdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqFMBOxfDCMEnergy tango device (string)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsynchronized monochromator energy (datasource)\(aq}, \(aqenergyfmb\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmonochromator energy (datasource)\(aq}, \(aqexitoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq exit offset (datasource)\(aq}, \(aqjack1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfirst vertical jack of table (datasource)\(aq}, \(aqjack1name\(aq: {\(aqdefault\(aq: \(aqjack1\(aq, \(aqdoc\(aq: \(aqfirst vertical jack name of table (string)\(aq}, \(aqjack2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecond vertical jack of table (datasource)\(aq}, \(aqjack2name\(aq: {\(aqdefault\(aq: \(aqjack2\(aq, \(aqdoc\(aq: \(aqsecond vertical jack name of table (string)\(aq}, \(aqjack3\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthird vertical jack of table (datasource)\(aq}, \(aqjack3name\(aq: {\(aqdefault\(aq: \(aqjack3\(aq, \(aqdoc\(aq: \(aqthird vertical jack name of table (string)\(aq}, \(aqlat\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the first cristal (datasource)\(aq}, \(aqlat2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal lattice translation of the second cristal (datasource)\(aq}, \(aqlat2name\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the second cristal (string)\(aq}, \(aqlatname\(aq: {\(aqdefault\(aq: \(aqlat\(aq, \(aqdoc\(aq: \(aqhorizontal lattice translation name of the first cristal (string)\(aq}, \(aqoxfordhorizontal\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq horizontal translation (datasource)\(aq}, \(aqpar2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbeam parallel translation of the second cristal (datasource)\(aq}, \(aqpar2name\(aq: {\(aqdefault\(aq: \(aqpara\(aq, \(aqdoc\(aq: \(aqbeam parallel translation name of the second cristal (string)\(aq}, \(aqperp2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical translation of the second cristal (datasource)\(aq}, \(aqperp2name\(aq: {\(aqdefault\(aq: \(aqperp\(aq, \(aqdoc\(aq: \(aqvertical translation name of the second cristal (string)\(aq}, \(aqphi1dependson\(aq: {\(aqdefault\(aq: \(aq../../transformations/bragg\(aq, \(aqdoc\(aq: \(aqthe depends_on field of the first cristal phi, e.g. theta (string)\(aq}, \(aqpitch1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta rotation of the first cristal (datasource)\(aq}, \(aqpitch1name\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta rotation name of the first cristal (string)\(aq}, \(aqpitch2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta rotation of the second cristal (datasource)\(aq}, \(aqpitch2name\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta rotation name of the second cristal (string)\(aq}, \(aqroll1\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchi rotation of the first cristal (datasource)\(aq}, \(aqroll1name\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqchi rotation name of the first cristal (string)\(aq}, \(aqroll2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchi rotation of the second cristal (datasource)\(aq}, \(aqroll2name\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqchi rotation name of the second cristal (string)\(aq}, \(aqtable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position of table (datasource)\(aq}, \(aqtablename\(aq: {\(aqdefault\(aq: \(aqtable\(aq, \(aqdoc\(aq: \(aqvertical position name of table (string)\(aq}, \(aqtheta\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtheta angle (datasource)\(aq}, \(aqthetaname\(aq: {\(aqdefault\(aq: \(aqtheta\(aq, \(aqdoc\(aq: \(aqtheta angle name (string)\(aq}, \(aqtopdependson2\(aq: {\(aqdefault\(aq: \(aqchi\(aq, \(aqdoc\(aq: \(aqthe first transformation of the second crystal, e.g. lat (string)\(aq}, \(aqunitcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqunit calibration from dcmmotor (datasource)\(aq}, \(aqusage\(aq: {\(aqdefault\(aq: \(aqBragg\(aq, \(aqdoc\(aq: \(aqthe crystall usage, e.g. Laue (string)\(aq}, \(aqyaw\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the first cristal (datasource)\(aq}, \(aqyaw2\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphi rotation of the second cristal (datasource)\(aq}, \(aqyaw2name\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the second cristal (string)\(aq}, \(aqyawname\(aq: {\(aqdefault\(aq: \(aqphi\(aq, \(aqdoc\(aq: \(aqphi rotation name of the first cristal (string)\(aq}}, \(aqdefault\(aq: {\(aq__configdevice__\(aq: {\(aqdefault\(aq: \(aqnxs/configserver/localhost\(aq, \(aqdoc\(aq: \(aqconfiguration server device name (string)\(aq}, \(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqcontrol\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgroup name of the monitor (string)\(aq}, \(aqlongname\(aq: {\(aqdefault\(aq: \(aqP09 Resonant Scattering and Diffraction beamline\(aq, \(aqdoc\(aq: \(aqbeamline long name (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}, \(aqsourcename\(aq: {\(aqdefault\(aq: \(aqPETRA III\(aq, \(aqdoc\(aq: \(aqsource name (string)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqdefaultinstrument\(aq: {\(aq__configdevice__\(aq: {\(aqdefault\(aq: \(aqnxs/configserver/localhost\(aq, \(aqdoc\(aq: \(aqconfiguration server device name (string)\(aq}, \(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqcontrol\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgroup name of the monitor (string)\(aq}, \(aqlongname\(aq: {\(aqdefault\(aq: \(aqP09 Resonant Scattering and Diffraction beamline\(aq, \(aqdoc\(aq: \(aqbeamline long name (string)\(aq}, \(aqshortname\(aq: {\(aqdefault\(aq: \(aqP09\(aq, \(aqdoc\(aq: \(aqbeamline short name (string)\(aq}, \(aqsourcename\(aq: {\(aqdefault\(aq: \(aqPETRA III\(aq, \(aqdoc\(aq: \(aqsource name (string)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqdefaultsample\(aq: {}, \(aqdescription\(aq: {}, \(aqdescriptiontext\(aq: {\(aqdescription\(aq: {\(aqdefault\(aq: \(aqscan\(aq, \(aqdoc\(aq: \(aqscan technique (string)\(aq}}, \(aqdetectorlive\(aq: {\(aqdatatype\(aq: {\(aqdefault\(aq: \(aqNX_UINT32\(aq, \(aqdoc\(aq: \(aqlist of devices (string)\(aq}, \(aqdetectordata\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdetector live data (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqdetector\(aq, \(aqdoc\(aq: \(aqlist of devices (string)\(aq}}, \(aqempty\(aq: {}, \(aqgroupsecop\(aq: {\(aqaccess\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop access list (string)\(aq}, \(aqgroup\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop group name (string)\(aq}, \(aqhost\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop host name (string)\(aq}, \(aqmessage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop command MANDATORY (string)\(aq}, \(aqport\(aq: {\(aqdefault\(aq: \(aq5000\(aq, \(aqdoc\(aq: \(aqsecop port name (string)\(aq}, \(aqtimeout\(aq: {\(aqdefault\(aq: \(aq0.0001\(aq, \(aqdoc\(aq: \(aqsecop timeout (string)\(aq}}, \(aqkeithley\(aq: {\(aqcurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqcurrent in A (datasource)\(aq}, \(aqgain\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgain in V/A (datasource)\(aq}, \(aqrisetime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqrise time (datasource)\(aq}, \(aqsourvoltlevel\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsource voltage level in V (datasource)\(aq}, \(aqvoltage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvoltage in V (datasource)\(aq}}, \(aqmaia\(aq: {\(aqchillersetpoint\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqchiller set point temperature in Celsus (datasource)\(aq}, \(aqchiptemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdetector chip temperature sensor for maia in Celsus (datasource)\(aq}, \(aqgaintrimenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgaintrim enable status for maia (datasource)\(aq}, \(aqidentity\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsensor identity for maia (datasource)\(aq}, \(aqinterlockpressure\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock pressure for maia in mbar (datasource)\(aq}, \(aqleakagecurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleakage current sensor for maia in A (datasource)\(aq}, \(aqlineariseenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqlinearise enable status for maia (datasource)\(aq}, \(aqmaiadimensions\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia dimensions component name (component)\(aq}, \(aqmaiafluxes\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia fluxes component name (component)\(aq}, \(aqmaiastage\(aq: {\(aqdefault\(aq: \(aqempty\(aq, \(aqdoc\(aq: \(aqmaia stage component name (component)\(aq}, \(aqmosfettemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmosfet temperature sensor for maia in Celsus (datasource)\(aq}, \(aqpeltiercurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpeltier current sensor for maia in A (datasource)\(aq}, \(aqphotonenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqphoton enable status for maia (datasource)\(aq}, \(aqpileuprejectionenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpileup rejection enable status for maia (datasource)\(aq}, \(aqpixelenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel enable status for maia (datasource)\(aq}, \(aqpressure\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgas pressure in mbar (datasource)\(aq}, \(aqrunnumber\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqrun number of maia (datasource)\(aq}, \(aqstatus\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock status for maia (datasource)\(aq}, \(aqthrottleenable\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthrottle enable status for maia (datasource)\(aq}, \(aquptime\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqinterlock uptime for maia (datasource)\(aq}, \(aqvoltagesetpoint\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvoltage set point temperature in Celsus (datasource)\(aq}, \(aqwatertemperature\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqwater temperature sensor for maia in Celsus (datasource)\(aq}}, \(aqmaiadimension\(aq: {\(aqdetname\(aq: {\(aqdefault\(aq: \(aqmaia\(aq, \(aqdoc\(aq: \(aqdetector (alias) name (string)\(aq}, \(aqdimname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdimension name for maia (datasource)\(aq}, \(aqdname\(aq: {\(aqdefault\(aq: \(aqdimension\(aq, \(aqdoc\(aq: \(aqdimension name group (string)\(aq}, \(aqhysteresis\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel hysteresis of dimension for maia (datasource)\(aq}, \(aqnumberofpixels\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnumber of pixels of dimension for maia (datasource)\(aq}, \(aqorigin\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel origin of dimension for maia (datasource)\(aq}, \(aqpixelpitch\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpixel pitch of dimension for maia (datasource)\(aq}, \(aqpositionsource\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqposition source of dimension for maia (datasource)\(aq}, \(aqunit\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqposition units of dimension for maia (datasource)\(aq}}, \(aqmaiaflux\(aq: {\(aqcoefficient\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux coefficient  for maia (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqmaia\(aq, \(aqdoc\(aq: \(aqdetector (alias) name (string)\(aq}, \(aqfluxname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux name for maia (datasource)\(aq}, \(aqfname\(aq: {\(aqdefault\(aq: \(aqfluxdevice\(aq, \(aqdoc\(aq: \(aqflux name group (string)\(aq}, \(aqkeithleydevice\(aq: {\(aqdefault\(aq: \(aqkeithley\(aq, \(aqdoc\(aq: \(aqkeithley device name (string)\(aq}, \(aqsource\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux source for maia (datasource)\(aq}, \(aqunit\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqflux unit for maia (datasource)\(aq}, \(aqvfcfactor\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvfc conversion factor (datasource)\(aq}}, \(aqmsnsar\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana device name MANDATORY (string)\(aq}, \(aqvarname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnested sardana environment variable name  MANDATORY (string)\(aq}}, \(aqmssar\(aq: {\(aq__tangohost__\(aq: {\(aqdefault\(aq: \(aqlocalhost\(aq, \(aqdoc\(aq: \(aqtango host (string)\(aq}, \(aq__tangoport__\(aq: {\(aqdefault\(aq: \(aq10000\(aq, \(aqdoc\(aq: \(aqtango port (string)\(aq}, \(aqmsenv\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment (datasource)\(aq}, \(aqmssardanadevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqmacroserver sardana device name MANDATORY (string)\(aq}, \(aqvarname\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsardana environment variable name MANDATORY (string)\(aq}}, \(aqparametercopymap\(aq: {\(aqcopymap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqyaml dictionary with {output: input} copy map (string)\(aq}, \(aqparameter\(aq: {\(aqdefault\(aq: \(aqcopymap\(aq, \(aqdoc\(aq: \(aqparameter name of copymap (string)\(aq}, \(aqprogram\(aq: {\(aqdefault\(aq: \(aqnxsfileinfo_parameters\(aq, \(aqdoc\(aq: \(aqgroup name of NXparameters (string)\(aq}}, \(aqpinhole\(aq: {\(aqdiameter\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpinhole diameter (datasource)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqxsign\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(dqhorizontal position sign, e.g. \(aq\-\(aq (string)\(dq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}, \(aqz\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqalong the beam position (datasource)\(aq}, \(aqzname\(aq: {\(aqdefault\(aq: \(aqz\(aq, \(aqdoc\(aq: \(aqalong the beam position name (string)\(aq}}, \(aqpointdet\(aq: {\(aqdata\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdiode data (datasource)\(aq}, \(aqdetname\(aq: {\(aqdefault\(aq: \(aqdetector\(aq, \(aqdoc\(aq: \(aqdetector group name (string)\(aq}}, \(aqqbpm\(aq: {\(aqdependsony\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqthe  depends_on y field value,  e.g. distance (string)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqfoil\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil type, i.e. standard <cpname>_foil (datasource)\(aq}, \(aqfoilpos\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqfoil position MANDATORY (datasource)\(aq}, \(aqfoilposdict\(aq: {\(aqdefault\(aq: \(aq{\(dqTi\(dq: 43, \(dqNi\(dq: 23, \(dqOut\(dq: 3}\(aq, \(aqdoc\(aq: \(aqfoil_type position json dictionary (string)\(aq}, \(aqx\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal position (datasource)\(aq}, \(aqxname\(aq: {\(aqdefault\(aq: \(aqx\(aq, \(aqdoc\(aq: \(aqhorizontal position name (string)\(aq}, \(aqy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical position (datasource)\(aq}, \(aqyname\(aq: {\(aqdefault\(aq: \(aqy\(aq, \(aqdoc\(aq: \(aqvertical position name (string)\(aq}}, \(aqsampledescription\(aq: {\(aqsname\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqsampledescriptiontext\(aq: {\(aqdescription\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqsample description or sampleId (string)\(aq}, \(aqsname\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqsamplehkl\(aq: {\(aqh\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqh position in hkl space (datasource)\(aq}, \(aqk\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqk position in hkl space (datasource)\(aq}, \(aql\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aql position in hkl space (datasource)\(aq}, \(aqpsi\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqpsi angle position of analyzer (datasource)\(aq}, \(aqsname\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqsecop\(aq: {\(aqhost\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop host name (string)\(aq}, \(aqmessage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop command MANDATORY (string)\(aq}, \(aqport\(aq: {\(aqdefault\(aq: \(aq5000\(aq, \(aqdoc\(aq: \(aqsecop port name (string)\(aq}, \(aqtimeout\(aq: {\(aqdefault\(aq: \(aq0.0001\(aq, \(aqdoc\(aq: \(aqsecop timeout (string)\(aq}}, \(aqsecoplinks\(aq: {\(aqenvironments\(aq: {\(aqdefault\(aq: \(aqtemperature,magnetic_field\(aq, \(aqdoc\(aq: \(aqsecop environment link lists MANDATORY (string)\(aq}, \(aqmeanings\(aq: {\(aqdefault\(aq: \(aqtemperature,magnetic_field,electric_field,stress_field,pressure\(aq, \(aqdoc\(aq: \(aqsecop meanings link lists MANDATORY (string)\(aq}, \(aqsampleenvname\(aq: {\(aqdefault\(aq: \(aqsample_environment\(aq, \(aqdoc\(aq: \(aqsample environment group name (string)\(aq}, \(aqsamplename\(aq: {\(aqdefault\(aq: \(aqsample\(aq, \(aqdoc\(aq: \(aqsample group name (string)\(aq}}, \(aqsinglesecop\(aq: {\(aqhost\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop host name (string)\(aq}, \(aqmessage\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqsecop command MANDATORY (string)\(aq}, \(aqport\(aq: {\(aqdefault\(aq: \(aq5000\(aq, \(aqdoc\(aq: \(aqsecop port name (string)\(aq}, \(aqtimeout\(aq: {\(aqdefault\(aq: \(aq0.0001\(aq, \(aqdoc\(aq: \(aqsecop timeout (string)\(aq}}, \(aqslit\(aq: {\(aqbottom\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbottom blade position (datasource)\(aq}, \(aqbottomclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqbottom blade closed position (datasource)\(aq}, \(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance for the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name for the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqleft\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleft blade position (datasource)\(aq}, \(aqleftclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqleft blade closed position (datasource)\(aq}, \(aqright\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqright blade position (datasource)\(aq}, \(aqrightclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqright blade closed position (datasource)\(aq}, \(aqtop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtop blade position (datasource)\(aq}, \(aqtopclosed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtop blade closed position (datasource)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(dqtransformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)\(dq}, \(aqxgap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal gap (datasource)\(aq}, \(aqxoffdependson\(aq: {\(aqdefault\(aq: \(aqy_offset\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqxoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal offset (datasource)\(aq}, \(aqxoffsetcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqhorizontal offset calibration (datasource)\(aq}, \(aqxoffsetcalibrationname\(aq: {\(aqdefault\(aq: \(aqx_offset_calibration\(aq, \(aqdoc\(aq: \(aqhorizontal offset calibration name (string)\(aq}, \(aqxoffsetname\(aq: {\(aqdefault\(aq: \(aqx_offset\(aq, \(aqdoc\(aq: \(aqhorizontal offset name (string)\(aq}, \(aqygap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertical gap (datasource)\(aq}, \(aqyoffdependson\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqyoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertiacal offset (datasource)\(aq}, \(aqyoffsetcalibration\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqvertiacal offset calibration (datasource)\(aq}, \(aqyoffsetcalibrationname\(aq: {\(aqdefault\(aq: \(aqy_offset_calibration\(aq, \(aqdoc\(aq: \(aqvertiacal offset calibration name (string)\(aq}, \(aqyoffsetname\(aq: {\(aqdefault\(aq: \(aqy_offset\(aq, \(aqdoc\(aq: \(aqvertiacal offset name (string)\(aq}}, \(aqsource\(aq: {\(aqbeamcurrent\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqring beam current (datasource)\(aq}, \(aqbunchmode\(aq: {\(aqdefault\(aq: \(aqMulti Bunch\(aq, \(aqdoc\(aq: \(aqbunch mode (string)\(aq}, \(aqnumberofbunches\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqnumber of source bunches (datasource)\(aq}, \(aqsourceenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqring beam energy (datasource)\(aq}, \(aqsrcname\(aq: {\(aqdefault\(aq: \(aqsource\(aq, \(aqdoc\(aq: \(aqsource group name (string)\(aq}}, \(aqstarttime\(aq: {}, \(aqtango\(aq: {\(aqattribute\(aq: {\(aqdefault\(aq: \(aqPosition\(aq, \(aqdoc\(aq: \(aqtango device attribute (string)\(aq}, \(aqdevice\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqtango device MANDATORY (string)\(aq}}, \(aqundulator\(aq: {\(aqdependstop\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqthe first transformation, e.g. distance (string)\(aq}, \(aqdistance\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqdistance from the sample in m, e.g. 0 (string)\(aq}, \(aqdistancename\(aq: {\(aqdefault\(aq: \(aqdistance\(aq, \(aqdoc\(aq: \(aqdistance name from the sample in m, e.g. 0 (string)\(aq}, \(aqdistanceoffset\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aq3\-vector distance offset in m, e.g. sample\-source offset if the distance is taken from the source (string)\(aq}, \(aqenergy\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator energy (datasource)\(aq}, \(aqgap\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqseparation between opposing pairs of magnetic pole (datasource)\(aq}, \(aqgapunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqgap units (string)\(aq}, \(aqharmonic\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator harmonic (datasource)\(aq}, \(aqlength\(aq: {\(aqdefault\(aq: \(aq2\(aq, \(aqdoc\(aq: \(aqlength of insertion device in meters (string)\(aq}, \(aqshift\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator shift (datasource)\(aq}, \(aqshiftunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqshift units (string)\(aq}, \(aqspeed\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqundulator speed (datasource)\(aq}, \(aqspeedunits\(aq: {\(aqdefault\(aq: \(aq\(aq, \(aqdoc\(aq: \(aqspeed units (string)\(aq}, \(aqtaper\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(aqgap difference between upstream and downstream ends of the insertion device (datasource)\(aq}, \(aqtaperunits\(aq: {\(aqdefault\(aq: \(aqmm\(aq, \(aqdoc\(aq: \(aqgap units (string)\(aq}, \(aqtransformations\(aq: {\(aqdefault\(aq: None, \(aqdoc\(aq: \(dqtransformations group name i.e. \(aqtransformations\(aq. If it is  not set it is not created (string)\(dq}, \(aqtype\(aq: {\(aqdefault\(aq: \(aqundulator\(aq, \(aqdoc\(aq: \(aqundulator or wiggler (string)\(aq}, \(aquname\(aq: {\(aqdefault\(aq: \(aqinsertion_device\(aq, \(aqdoc\(aq: \(aqinsertion_device group name (string)\(aq}}}
 (\fI\%dict\fP <\fI\%str\fP , \fI\%dict\fP <\fI\%str\fP , \fI\%str\fP > >)
 standard component template variables
 and its [default value, doc string]
 .UNINDENT
+.sp
+pyeval functions
 .INDENT 0.0
 .IP \(bu 2
-genindex
+\fI\%Index\fP
 .IP \(bu 2
-modindex
+\fI\%Module Index\fP
 .IP \(bu 2
-search
+\fI\%Search Page\fP
 .UNINDENT
 .SH AUTHOR
 Jan Kotanski
 .SH COPYRIGHT
 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 
 GNU GENERAL PUBLIC LICENSE, version 3
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nxstools-3.9.0/nxstools/__init__.py` & `nxstools-4.0.0/nxstools/release.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -13,13 +12,11 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-"""  NXS tools """
+"""  NXS tools release version"""
 
-#: package version
-from .release import __version__
-
-__all__ = ["__version__"]
+#: (:obj:`str`) package version
+__version__ = "4.0.0"
```

### Comparing `nxstools-3.9.0/nxstools/filenamegenerator.py` & `nxstools-4.0.0/nxstools/filenamegenerator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
```

### Comparing `nxstools-3.9.0/nxstools/filewriter.py` & `nxstools-4.0.0/nxstools/filewriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2017 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -295,21 +294,21 @@
 class FTHyperslab(object):
     """ hyperslab class """
 
     def __init__(self, offset=None, block=None, count=None, stride=None):
         """ constructor
 
         :param offset: a list of offsets
-        :type offset: :tuple:`int`
+        :type offset: :obj:`tuple` <:obj:`int`>
         :param block: a list of blocks
-        :type block: :tuple:`int`
+        :type block: :obj:`tuple` <:obj:`int`>
         :param count: a list of counts
-        :type count: :tuple:`int`
+        :type count: :obj:`tuple` <:obj:`int`>
         :param stride: a list of strides
-        :type stride: :tuple:`int`
+        :type stride: :obj:`tuple` <:obj:`int`>
         """
         self.offset = offset
         self.block = block
         self.count = count
         self.stride = stride
 
     def __eq__(self, other):
@@ -444,15 +443,21 @@
     :returns: first element of the array
     :type array: :obj:`any`
     """
     try:
         if isinstance(array, numpy.ndarray) and len(array) == 1:
             return array[0]
     except Exception:
-        pass
+        try:
+            if hasattr(array, "all"):
+                array = array.all()
+                if hasattr(array, "decode"):
+                    return array.decode()
+        except Exception:
+            pass
     return array
 
 
 class FTFile(FTObject):
 
     """ file tree file
     """
@@ -518,88 +523,30 @@
     def currenttime(cls):
         """ returns current time string
 
         :returns: current time
         :rtype: :obj:`str`
         """
         tzone = time.tzname[0]
-        tz = pytz.timezone(tzone)
+        try:
+            tz = pytz.timezone(tzone)
+        except Exception:
+            import tzlocal
+            tz = tzlocal.get_localzone()
         fmt = '%Y-%m-%dT%H:%M:%S.%f%z'
         starttime = tz.localize(datetime.datetime.now())
         return str(starttime.strftime(fmt))
 
     def default_field(self):
         """ field pointed by default attributes
 
         :returns: field pointed by default attributes
         :rtype: :class:`FTField`
         """
-        node = self.root()
-        searching = True
-        while searching:
-            attrs = node.attributes
-            if hasattr(node, "names") and "default" in attrs.names():
-                nname = attrs["default"].read()
-                if isinstance(nname, numpy.ndarray) and len(nname):
-                    nname = nname[0]
-                if nname in node.names():
-                    node = node.open(nname)
-                    continue
-            searching = False
-        if hasattr(node, "names"):
-            attrs = node.attributes
-            if "signal" in attrs.names():
-                nname = attrs["signal"].read()
-                if isinstance(nname, numpy.ndarray) and len(nname):
-                    nname = nname[0]
-                if nname in node.names():
-                    node = node.open(nname)
-        if not hasattr(node, "names"):
-            return node
-
-        for cnm in ["NXentry", "NXdata", "NXmonitor", "NXlog"]:
-            names = node.names()
-            if cnm[2:] in names:
-                snames = [cnm[2:]]
-            else:
-                snames = []
-            snames.extend(sorted([nm for nm in names if nm != cnm[2:]]))
-            for nn in snames:
-                nd = node.open(nn)
-                if not hasattr(nd, "attributes"):
-                    continue
-                attrs = nd.attributes
-                if "NX_class" in attrs.names():
-                    nname = attrs["NX_class"].read()
-                    if isinstance(nname, numpy.ndarray) and len(nname):
-                        nname = nname[0]
-                    if nname in cnm:
-                        node = nd
-                        break
-        if hasattr(node, "names") and hasattr(node, "attributes"):
-            attrs = node.attributes
-            if "signal" in attrs.names():
-                nname = attrs["signal"].read()
-                if isinstance(nname, numpy.ndarray) and len(nname):
-                    nname = nname[0]
-                if nname in node.names():
-                    node = node.open(nname)
-        if not hasattr(node, "names"):
-            return node
-        while hasattr(node, "names") and "data" in node.names():
-            node = node.open("data")
-        if hasattr(node, "names"):
-            for nn in sorted(node.names()):
-                nd = node.open(nn)
-                if not hasattr(nd, "names"):
-                    node = nd
-                    break
-        if not hasattr(node, "names"):
-            return node
-        return None
+        return self.root().default_field()
 
 
 class FTGroup(FTObject):
 
     """ file tree group
     """
 
@@ -708,14 +655,119 @@
         """
 
     def reopen(self):
         """ reopen attribute
         """
         FTObject._reopen(self)
 
+    def default_field(self, signals=None, nexuspath=None):
+        """ field pointed by default attributes
+
+        :type signals: :obj:`list`<:obj:`str`>
+        :param axes: axes names
+        :param entryname: base nexus path to be opened
+        :type entryname: :obj:`str`
+        :returns: field pointed by default attributes
+        :rtype: :class:`FTField`
+        """
+
+        node = self
+        searching = True
+        nexuspath = nexuspath or ""
+        groups = [n for n in nexuspath.split("/") if n]
+        while searching:
+            nname = None
+            if hasattr(node, "names"):
+                gname = ""
+                if groups:
+                    gname = groups.pop(0)
+                if gname in node.names():
+                    node = node.open(gname)
+                    continue
+                else:
+                    groups = []
+                attrs = node.attributes
+                if "default" in attrs.names():
+                    nname = attrs["default"].read()
+                    if isinstance(nname, numpy.ndarray) and len(nname):
+                        nname = nname[0]
+                    if nname in node.names():
+                        node = node.open(nname)
+                        continue
+            searching = False
+        if not hasattr(node, "names"):
+            return node
+        if hasattr(node, "names"):
+            if groups:
+                gname = groups.pop(0)
+            if gname in node.names():
+                node = node.open(gname)
+                if not hasattr(node, "names"):
+                    return node
+            else:
+                groups = []
+                attrs = node.attributes
+                if "signal" in attrs.names():
+                    nname = attrs["signal"].read()
+                    if isinstance(nname, numpy.ndarray) and len(nname):
+                        nname = nname[0]
+                    if nname in node.names():
+                        node = node.open(nname)
+                    if not hasattr(node, "names"):
+                        return node
+
+        for cnm in ["NXentry", "NXdata", "NXmonitor", "NXlog"]:
+            names = node.names()
+            if cnm[2:] in names:
+                snames = [cnm[2:]]
+            else:
+                snames = []
+            snames.extend(sorted([nm for nm in names if nm != cnm[2:]]))
+            for nn in snames:
+                nd = node.open(nn)
+                if not hasattr(nd, "attributes"):
+                    continue
+                attrs = nd.attributes
+                if "NX_class" in attrs.names():
+                    nname = attrs["NX_class"].read()
+                    if isinstance(nname, numpy.ndarray) and len(nname):
+                        nname = nname[0]
+                    if nname in cnm:
+                        node = nd
+                        break
+        if hasattr(node, "names") and hasattr(node, "attributes"):
+            attrs = node.attributes
+            if "signal" in attrs.names():
+                nname = attrs["signal"].read()
+                if isinstance(nname, numpy.ndarray) and len(nname):
+                    nname = nname[0]
+                if nname in node.names():
+                    node = node.open(nname)
+        if not hasattr(node, "names"):
+            return node
+        while hasattr(node, "names") and "data" in node.names():
+            node = node.open("data")
+        if hasattr(node, "names"):
+            if signals:
+                for signal in signals:
+                    if signal in node.names():
+                        nd = node.open(signal)
+                        if not hasattr(signal, "names"):
+                            node = nd
+                            break
+        if hasattr(node, "names"):
+            for nn in sorted(node.names()):
+                nd = node.open(nn)
+                if not hasattr(nd, "names"):
+                    node = nd
+                    break
+        if not hasattr(node, "names"):
+            return node
+        return None
+
 
 class FTVirtualFieldLayout(FTObject):
 
     """ virtual field layout """
 
     def __init__(self, h5object=None):
         """ constructor
@@ -913,17 +965,57 @@
         """
         FTObject.__init__(self, h5object, tparent)
         #: (:obj:`bool`) compression shuffle
         self._shuffle = False
         #: (:obj:`int`) compression rate
         self._rate = 0
         #: (:obj:`int`) compression filter id
-        self._filterid = 1
+        self._filterid = 0
         #: (:obj:`tuple` <:obj:`int`>) compression options
         self._options = tuple()
+        #: (:obj:`str`) filter name
+        self._name = ""
+        #: (:obj:`str`) filter availability
+        self._availability = ""
+
+    @property
+    def name(self):
+        """ getter for filter name
+
+        :returns: filter name
+        :rtype: :obj:`tuple` <:obj:`str`>
+        """
+        return self._name
+
+    @name.setter
+    def name(self, value):
+        """ setter for filter name
+
+        :param value: filter name
+        :type value: :obj:`tuple` <:obj:`str`>
+        """
+        self._name = value
+
+    @property
+    def availability(self):
+        """ getter for filter availability
+
+        :returns: filter availability
+        :rtype: :obj:`tuple` <:obj:`str`>
+        """
+        return self._availability
+
+    @availability.setter
+    def availability(self, value):
+        """ setter for filter availability
+
+        :param value: filter availability
+        :type value: :obj:`tuple` <:obj:`str`>
+        """
+        self._availability = value
 
     @property
     def options(self):
         """ getter for compression options
 
         :returns: compression options
         :rtype: :obj:`tuple` <:obj:`int`>
@@ -1091,24 +1183,24 @@
         :type o: :obj:`any`
         """
 
     def __setitem__(self, t, o):
         """ write attribute value
 
         :param t: slice tuple
-        :type t: :obj:`tuple`
+        :type t: :obj:`tuple` <:obj:`int`>
         :param o: python object
         :type o: :obj:`any`
         """
 
     def __getitem__(self, t):
         """ read attribute value
 
         :param t: slice tuple
-        :type t: :obj:`tuple`
+        :type t: :obj:`tuple` <:obj:`int`>
         :returns: python object
         :rtype: :obj:`any`
         """
 
     @property
     def dtype(self):
         """ attribute data type
```

### Comparing `nxstools-3.9.0/nxstools/h5cppwriter.py` & `nxstools-4.0.0/nxstools/h5cppwriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2017 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -470,24 +469,68 @@
     :rtype: :obj: `list` <:class:`H5CppLink`>
     """
     lks = parent.h5object.links
     links = [H5CppLink(e, parent) for e in lks]
     return links
 
 
-def data_filter():
-    """ create deflate filter
-
+def data_filter(filterid=None, name=None, options=None, availability=None,
+                shuffle=None, rate=None):
+    """ create data filter
+
+    :param filterid: hdf5 filter id
+    :type filterid: :obj:`int`
+    :param name: filter name
+    :type name: :obj:`str`
+    :param options: filter cd values
+    :type options: :obj:`tuple` <:obj:`int`>
+    :param availability: filter availability i.e. 'optional' or 'mandatory'
+    :type availability: :obj:`str`
+    :param shuffle: filter shuffle
+    :type shuffle: :obj:`bool`
+    :param rate: filter shuffle
+    :type rate: :obj:`bool`
+    :returns: data filter object
+    :rtype: :class:`H5CppDataFilter`
+    """
+    dtf = H5CppDataFilter()
+    if filterid:
+        dtf.filterid = filterid
+    if name:
+        dtf.name = name
+    if shuffle:
+        dtf.shuffle = shuffle
+    if rate:
+        dtf.rate = rate
+    if options:
+        dtf.options = options
+    if availability:
+        dtf.availability = availability
+    return dtf
+
+
+def deflate_filter(rate=None, shuffle=None, availability=None):
+    """ create data filter
+
+    :param rate: filter shuffle
+    :type rate: :obj:`bool`
+    :param shuffle: filter shuffle
+    :type shuffle: :obj:`bool`
     :returns: deflate filter object
     :rtype: :class:`H5CppDataFilter`
     """
-    return H5CppDataFilter(h5cpp.filter.Deflate())
-
-
-deflate_filter = data_filter
+    dtf = H5CppDataFilter()
+    dtf.filterid = 1
+    dtf.name = "deflate"
+    if shuffle:
+        dtf.shuffle = shuffle
+    dtf.rate = rate or 2
+    if availability:
+        dtf.availability = availability
+    return dtf
 
 
 def target_field_view(filename, fieldpath, shape,
                       dtype=None, maxshape=None):
     """ create target field view for VDS
 
     :param filename: file name
@@ -538,14 +581,16 @@
         :type h5object: :obj:`any`
         :param filename:  file name
         :type filename: :obj:`str`
         """
         filewriter.FTFile.__init__(self, h5object, filename)
         #: (:obj:`str`) object nexus path
         self.path = None
+        #: (:obj:`str`) nexus file name
+        self.filename = filename
         if hasattr(h5object, "path"):
             self.path = h5object.path
 
     def root(self):
         """ root object
 
         :returns: parent object
@@ -649,15 +694,15 @@
         #: (:obj:`str`) object nexus path
         self.path = u""
         #: (:obj:`str`) object name
         self.name = None
         if hasattr(h5object, "link"):
             self.name = h5object.link.path.name
             if tparent and tparent.path:
-                if isinstance(tparent, H5CppFile):
+                if hasattr(tparent, "root"):
                     if self.name == ".":
                         self.path = u"/"
                     else:
                         self.path = u"/" + self.name
                 else:
                     if tparent.path.endswith("/"):
                         self.path = tparent.path
@@ -792,24 +837,56 @@
                 pTh[_tostr(type_code)], dataspace,
                 dcpl=dcpl), self)
         else:
             shape = shape or [1]
             dataspace = h5cpp.dataspace.Simple(
                 tuple(shape), tuple([h5cpp.dataspace.UNLIMITED] * len(shape)))
             if dfilter:
-                if dfilter.filterid == 1:
-                    h5object = dfilter.h5object
-                    h5object.level = dfilter.rate
-                else:
-                    h5object = h5cpp.filter.ExternalFilter(
-                        dfilter.filterid, list(dfilter.options))
-                h5object(dcpl)
-                if dfilter.shuffle:
-                    sfilter = h5cpp.filter.Shuffle()
-                    sfilter(dcpl)
+                if not isinstance(dfilter, list):
+                    dfilter = [dfilter]
+                for dfl in dfilter:
+                    if dfl.shuffle:
+                        sfilter = h5cpp.filter.Shuffle()
+                        sfilter(dcpl)
+                    h5object = None
+                    if dfl.rate:
+                        h5object = h5cpp.filter.Deflate(dfl.rate)
+                    elif dfl.filterid > 0:
+                        h5object = h5cpp.filter.ExternalFilter(
+                            dfl.filterid, list(dfl.options), dfl.name)
+                    elif dfl.name == "shuffle":
+                        h5object = h5cpp.filter.Shuffle()
+                    elif dfl.name == "deflate":
+                        if dfl.options:
+                            dfl.rate = dfl.options[0]
+                        h5object = h5cpp.filter.Deflate(dfl.rate)
+                    elif dfl.name == "nbit":
+                        h5object = h5cpp.filter.NBit()
+                    elif dfl.name == "fletcher32":
+                        h5object = h5cpp.filter.Fletcher32()
+                    elif dfl.name == "szip":
+                        h5object = h5cpp.filter.SZip()
+                        if dfl.options:
+                            h5object.option_mask = dfl.options[0]
+                        if len(dfl.options) > 1:
+                            h5object.pixel_per_block = dfl.options[1]
+                    elif dfl.name == "scaleoffset":
+                        h5object = h5cpp.filter.ScaleOffset()
+                        if dfl.options:
+                            h5object.scale_type = dfl.options[0]
+                        if len(dfl.options) > 1:
+                            h5object.scale_factor = dfl.options[1]
+
+                    if h5object:
+                        if dfl.availability:
+                            h5object(dcpl)
+                        elif dfl.availability == "optional":
+                            h5object(dcpl, h5cpp.filter.Availability.OPTIONALY)
+                        else:
+                            h5object(dcpl, h5cpp.filter.Availability.MANDATORY)
             if chunk is None and shape is not None:
                 chunk = [(dm if dm != 0 else 1) for dm in shape]
             dcpl.layout = h5cpp.property.DatasetLayout.CHUNKED
             dcpl.chunk = tuple(chunk)
             return H5CppField(h5cpp.node.Dataset(
                 self._h5object, h5cpp.Path(name),
                 pTh[_tostr(type_code)], dataspace,
@@ -840,15 +917,15 @@
 
         if self._h5object.is_valid:
             self._h5object.close()
 
     def reopen(self):
         """ reopen group
         """
-        if isinstance(self._tparent, H5CppFile):
+        if hasattr(self._tparent.h5object, "root"):
             self._h5object = self._tparent.h5object.root()
         else:
             try:
                 self._h5object = self._tparent.h5object.get_group(
                     h5cpp.Path(self.name))
             except Exception as e:
                 print(str(e))
@@ -1273,16 +1350,16 @@
         :rtype: :obj:`str`
         """
         filename = ""
         while not filename:
             par = obj.parent
             if par is None:
                 break
-            if isinstance(par, H5CppFile):
-                filename = par.name
+            if hasattr(par, "filename"):
+                filename = par.filename
                 break
             else:
                 obj = par
         return filename
 
     @property
     def target_path(self):
@@ -1392,15 +1469,15 @@
             else:
                 eview = h5cpp.dataspace.View(sds)
         else:
             eview = h5cpp.dataspace.View(sds)
         fname = source.filename
         path = h5cpp.Path(source.fieldpath)
         self._h5object.add(h5cpp.property.VirtualDataMap(
-            lview, fname, path, eview))
+            lview, str(fname), path, eview))
 
 
 class H5CppTargetFieldView(filewriter.FTTargetFieldView):
 
     """ target field for VDS """
 
     def __init__(self, filename, fieldpath, shape, dtype=None, maxshape=None):
@@ -1469,15 +1546,17 @@
         :rtype: :class:`H5CppAtribute`
         """
         at = None
         names = [att.name for att in self._h5object]
         if name in names:
             if overwrite:
                 try:
-                    if str(self[name].dtype) == _tostr(dtype):
+                    pass
+                    if str(self[name].dtype) == _tostr(dtype) \
+                       and self[name].shape == shape:
                         at = self._h5object[name]
                 except Exception as e:
                     print(str(e))
                 if at is None:
                     self._h5object.remove(name)
             else:
                 raise Exception("Attribute %s exists" % name)
```

### Comparing `nxstools-3.9.0/nxstools/h5pywriter.py` & `nxstools-4.0.0/nxstools/h5pywriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -392,24 +391,68 @@
     """
 
     return [H5PYLink(
         parent.h5object.get(name, getlink=True), parent).setname(name)
         for name in parent.names()]
 
 
-def data_filter():
-    """ create deflate filter
-
+def data_filter(filterid=None, name=None, options=None, availability=None,
+                shuffle=None, rate=None):
+    """ create data filter
+
+    :param filterid: hdf5 filter id
+    :type filterid: :obj:`int`
+    :param name: filter name
+    :type name: :obj:`str`
+    :param options: filter cd values
+    :type options: :obj:`tuple` <:obj:`int`>
+    :param availability: filter availability i.e. 'optional' or 'mandatory'
+    :type availability: :obj:`str`
+    :param shuffle: filter shuffle
+    :type shuffle: :obj:`bool`
+    :param rate: filter shuffle
+    :type rate: :obj:`bool`
     :returns: deflate filter object
     :rtype: :class:`H5PYDataFilter`
     """
-    return H5PYDataFilter()
-
-
-deflate_filter = data_filter
+    dtf = H5PYDataFilter()
+    if filterid:
+        dtf.filterid = filterid
+    if name:
+        dtf.name = name
+    if shuffle:
+        dtf.shuffle = shuffle
+    if rate:
+        dtf.rate = rate
+    if options:
+        dtf.options = options
+    if availability:
+        dtf.availability = availability
+    return dtf
+
+
+def deflate_filter(rate=None, shuffle=None, availability=None):
+    """ create data filter
+
+    :param rate: filter shuffle
+    :type rate: :obj:`bool`
+    :param shuffle: filter shuffle
+    :type shuffle: :obj:`bool`
+    :returns: deflate filter object
+    :rtype: :class:`H5CppDataFilter`
+    """
+    dtf = H5PYDataFilter()
+    dtf.filterid = 1
+    dtf.name = "deflate"
+    if shuffle:
+        dtf.shuffle = shuffle
+    dtf.rate = rate or 2
+    if availability:
+        dtf.availability = availability
+    return dtf
 
 
 def target_field_view(filename, fieldpath, shape,
                       dtype=None, maxshape=None):
     """ create target field view for VDS
 
     :param filename: file name
@@ -720,45 +763,61 @@
         """
         if type_code in ['string', b'string']:
             type_code = h5py.special_dtype(vlen=unicode)
             # type_code = h5py.special_dtype(vlen=bytes)
         if type_code == h5py.special_dtype(vlen=unicode) and \
            shape is None and chunk is None:
             return H5PYField(
-                self._h5object.create_dataset(name, (), type_code), self)
+                self._h5object.create_dataset(name,  (), type_code), self)
 
         shape = shape or [1]
+        f = None
         mshape = [None for _ in shape] or (None,)
         if dfilter:
-            if dfilter.filterid == 1:
+            if isinstance(dfilter, list):
+                if len(dfilter) == 2 and dfilter[0] and \
+                   (dfilter[0].shuffle or dfilter[0].name == "shuffle"
+                        or dfilter[0].filterid == 4) \
+                        and not dfilter[0].rate:
+                    dfilter = dfilter[1]
+                    dfilter.shuffle = True
+                elif len(dfilter) == 1:
+                    dfilter = dfilter[0]
+                else:
+                    raise Exception("Filter pipes not supported by h5py. "
+                                    "Please change to h5cpp")
+            if dfilter.filterid == 1 or dfilter.name == "deflate" or \
+               dfilter.rate:
+                if dfilter.options and dfilter.options[0]:
+                    dfilter.rate = dfilter.options[0]
                 f = H5PYField(
                     self._h5object.create_dataset(
                         name, shape, type_code,
                         chunks=(tuple(chunk)
                                 if chunk is not None else None),
                         compression="gzip",
                         compression_opts=(
                             dfilter.options[0]
                             if dfilter.options
                             else dfilter.rate),
                         shuffle=dfilter.shuffle, maxshape=mshape
                     ),
                     self)
-            else:
+            elif dfilter.filterid > 0 or dfilter.name:
                 f = H5PYField(
                     self._h5object.create_dataset(
                         name, shape, type_code,
                         chunks=(tuple(chunk)
                                 if chunk is not None else None),
-                        compression=dfilter.filterid,
+                        compression=(dfilter.filterid or dfilter.name),
                         compression_opts=tuple(dfilter.options),
                         shuffle=dfilter.shuffle, maxshape=mshape
                     ),
                     self)
-        else:
+        if not f:
             f = H5PYField(
                 self._h5object.create_dataset(
                     name, shape, type_code,
                     chunks=(tuple(chunk)
                             if chunk is not None else None),
                     maxshape=mshape
                 ),
```

### Comparing `nxstools-3.9.0/nxstools/nxsargparser.py` & `nxstools-4.0.0/nxstools/nxsargparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
```

### Comparing `nxstools-3.9.0/nxstools/nxscollect.py` & `nxstools-4.0.0/nxstools/nxscollect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
```

### Comparing `nxstools-3.9.0/nxstools/nxsconfig.py` & `nxstools-4.0.0/nxstools/nxsconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -22,19 +21,22 @@
 import sys
 import os
 import argparse
 import json
 from .nxsparser import ParserTools, TableTools, TableDictTools, ESRFConverter
 from .nxsargparser import (Runner, NXSArgParser, ErrorException)
 from .nxsdevicetools import (checkServer, listServers, openServer)
-#: (:obj:`bool`) True if PyTango available
+#: (:obj:`bool`) True if tango available
 
 PYTANGO = False
 try:
-    import PyTango
+    try:
+        import tango
+    except Exception:
+        import PyTango as tango
     PYTANGO = True
 except Exception:
     pass
 
 if sys.version_info > (3,):
     raw_input = input
 
@@ -51,15 +53,15 @@
         :type device: :obj:`str`
         :param nonewline: if the output should not be separated
                           by the new line character
         :type nonewline: :obj:`bool`
         """
         #: (:obj:`str`) spliting character
         self.char = " " if nonewline else "\n"
-        #: (:class:`PyTango.DeviceProxy`) configuration server proxy
+        #: (:class:`tango.DeviceProxy`) configuration server proxy
         self._cnfServer = openServer(device)
         self._cnfServer.Open()
 
     def listCmd(self, ds, mandatory=False, private=False, profiles=False):
         """ lists the DB item names
 
         :param ds: flag set True for datasources
@@ -1586,24 +1588,24 @@
         parg.extend([p.strip() for p in pipe])
         if hasattr(options, "args"):
             options.args[:] = parg
 
     try:
         result = runners[options.subparser].run(options)
 
-        # except PyTango.DevFailed as
+        # except tango.DevFailed as
     except Exception as e:
         if isinstance(e, EOFError) \
            and str(e).startswith("EOF when reading a line"):
             sys.stderr.write("Error: %s. Consider to use the "
                              "--force option \n" % str(e))
             sys.stderr.flush()
             sys.exit(255)
 
-        if PYTANGO and isinstance(e, PyTango.DevFailed):
+        if PYTANGO and isinstance(e, tango.DevFailed):
             # print(str((e.args[0]).desc))
             if str((e.args[0]).desc).startswith(
                     "NonregisteredDBRecordError: The datasource "):
                 mydss = str((e.args[0]).desc)[43:].split()
                 if not mydss or not mydss[0]:
                     mydss = ["UKNOWN"]
                 sys.stderr.write(
```

### Comparing `nxstools-3.9.0/nxstools/nxscreate.py` & `nxstools-4.0.0/nxstools/nxscreate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -27,22 +26,25 @@
 
 from nxstools.nxsargparser import (Runner, NXSArgParser, ErrorException)
 from nxstools.nxsdevicetools import (
     checkServer, getAttributes, getServerTangoHost)
 from nxstools.nxscreator import (
     TangoDSCreator, ClientDSCreator, WrongParameterError,
     DeviceDSCreator, OnlineDSCreator, OnlineCPCreator, CPExistsException,
-    DSExistsException,
+    DSExistsException, SECoPCPCreator,
     StandardCPCreator, ComponentCreator, CompareOnlineDS, PoolDSCreator)
 
 
 #: (:obj:`bool`) True if PyTango available
 PYTANGO = False
 try:
-    __import__("PyTango")
+    try:
+        __import__("tango")
+    except Exception:
+        __import__("PyTango")
     PYTANGO = True
 except Exception:
     pass
 
 
 class TangoDS(Runner):
 
@@ -1144,14 +1146,19 @@
 
         parser.add_argument(
             "-m", "--minimal-device", action="store_true",
             default=False, dest="minimal",
             help="device name without first '0'")
 
         parser.add_argument(
+            "-e", "--depends",
+            help="list of component dependencies separated by ','",
+            dest="depends", default="")
+
+        parser.add_argument(
             'args', metavar='component_name',
             type=str, nargs='*',
             help='component names to be created')
 
         return parser
 
     def run(self, options):
@@ -1184,14 +1191,204 @@
         except WrongParameterError as e:
             sys.stderr.write(str(e))
             sys.stderr.flush()
             parser.print_help()
             sys.exit(255)
 
 
+class SECoPCP(Runner):
+
+    """ secop component runner"""
+    #: (:obj:`str`) command description
+    description = "create secop components"
+    #: (:obj:`str`) command epilog
+    epilog = "" \
+        + " * with -b: components are created (without datasources)" \
+        + " in Configuration Server database\n" \
+        + " * without -b: components are created (without datasources)" \
+        + " on the local filesystem in -d <directory> \n" \
+        + " * default: <directory> is '.' \n" \
+        + "            <port> is 5001\n" \
+        + "\n" \
+        + " examples:\n" \
+        + "\n" \
+        + "       nxscreate secopcp \n" \
+        + "       nxscreate secopcp -l \n" \
+        + "\n" \
+        + "           - list all modules of the given node \n" \
+        + "\n" \
+        + "       nxscreate secopcp -c temp_node -d . -j secopn_node.json \n" \
+        + "\n" \
+        + "           - create the all secop components" \
+        + " in the local directory for the node configured" \
+        + " with the json file \n" \
+        + "\n" \
+        + "       nxscreate secopcp T -t 5001 -b \n" \
+        + "\n" \
+        + "           - create the component for the T secop module " \
+        + " in the NXSConfigServer database for the node on the port 5000 \n" \
+        + "\n" \
+        + "       nxscreate secopcp -d /home/user/xmldir/ \n" \
+        + "\n" \
+        + "           - create the all secop components" \
+        + " in the given directory\n" \
+        + "\n"
+
+    def create(self):
+        """ creates parser
+        """
+        parser = self._parser
+        parser.add_argument("-l", "--list", action="store_true",
+                            default=False, dest="listmodules",
+                            help="list modules of the given node")
+        parser.add_argument("-o", "--overwrite", action="store_true",
+                            default=False, dest="overwrite",
+                            help="overwrite existing components")
+        parser.add_argument("-a", "--can-fail", action="store_true",
+                            default=False, dest="canfail",
+                            help="can fail strategy flag")
+        parser.add_argument("-q", "--dynamic", action="store_true",
+                            default=False, dest="dynamiclinks",
+                            help="create dynamic links")
+        parser.add_argument("--sample-nxdata", action="store_true",
+                            default=False, dest="samplenxdata",
+                            help="create NXdata in NXsample")
+        parser.add_argument("-c", "--component",
+                            help="component name" +
+                            "secop component name",
+                            dest="component", default="")
+        parser.add_argument("-e", "--param-strategy",
+                            help="sensor parameter strategy, " +
+                            "i.e. INIT, STEP or FINAL, " +
+                            "default: INIT",
+                            dest="paramstrategy", default="INIT")
+        parser.add_argument("-g", "--strategy",
+                            help="sensor value strategy, " +
+                            "i.e. INIT, STEP or FINAL, " +
+                            "default: INIT",
+                            dest="strategy", default="INIT")
+        parser.add_argument("-m", "--timeout",
+                            help="sensor minimum timeout " +
+                            "default: 0.001",
+                            dest="timeout", default=0.001)
+        parser.add_argument("-s", "--sample",
+                            help="sample name",
+                            dest="samplename", default="sample")
+        parser.add_argument("-w", "--sample-environment",
+                            help="sample environment name",
+                            dest="sampleenvname",
+                            default="sample_environment")
+        parser.add_argument("-k", "--links",
+                            help="NXlog links of physical "
+                            "quantities to sensors "
+                            "separated by comman. Default: "
+                            "'temperature,magnetic_field,"
+                            "electric_field,"
+                            "stress_field,pressure'",
+                            dest="meanings",
+                            default="temperature,magnetic_field,"
+                            "electric_field,"
+                            "stress_field,pressure")
+        parser.add_argument("-v", "--environments",
+                            help="NXenvironment links of physical quantities "
+                            "separated by comman. "
+                            "Default: 'temperature,magnetic_field'",
+                            dest="environments",
+                            default="temperature,magnetic_field")
+        parser.add_argument("-f", "--first",
+                            help="first linked targets separated by comman",
+                            dest="first", default="")
+        parser.add_argument(
+            "-z", "--transformation-attributes", dest="transattrs",
+            default='{"rotation_z":'
+            '{"transformation_type":"rotation","vector":[0,1,0]}}',
+            help=("a JSON dictionary with transformation parameters i.e, "
+                  '"transformation_type", "vector", "depends_on".'
+                  ' Default: {"rotation_z":'
+                  '{"transformation_type":"rotation","vector":[0,1,0]}}'))
+        parser.add_argument("-p", "--xml-package", dest="xmlpackage",
+                            help="xml template package")
+        parser.add_argument("-y", "--entryname", dest="entryname",
+                            help="entry group name (prefix)", default="scan")
+        parser.add_argument("-i", "--insname", dest="insname",
+                            help="instrument group name", default="instrument")
+        parser.add_argument("-d", "--directory",
+                            help="output component directory",
+                            dest="directory")
+        parser.add_argument("-j", "--json-file",
+                            help="json configuration file",
+                            dest="json")
+        parser.add_argument("-x", "--file-prefix",
+                            help="file prefix, i.e. counter",
+                            dest="file", default="")
+        parser.add_argument("-n", "--nolower", action="store_false",
+                            default=True, dest="lower",
+                            help="do not change aliases into lower case")
+
+        parser.add_argument("-b", "--database", action="store_true",
+                            default=False, dest="database",
+                            help="store components in "
+                            "Configuration Server database")
+        parser.add_argument("-u", "--host",
+                            help="secop host name",
+                            dest="host", default="")
+        parser.add_argument("-t", "--port",
+                            help="secop host port",
+                            dest="port", default="5000")
+        parser.add_argument("-r", "--server", dest="server",
+                            help="configuration server device name")
+
+        parser.add_argument('args', metavar='component_name',
+                            type=str, nargs='*',
+                            help='component names to be created')
+
+        return parser
+
+    def run(self, options):
+        """ the main program function
+
+        :param options: parser options
+        :type options: :class:`argparse.Namespace`
+        """
+        args = options.args or []
+        parser = self._parser
+        if options.database and not options.server:
+            if not PYTANGO:
+                sys.stderr.write("Info: No PyTango installed\n")
+                sys.stderr.flush()
+                sys.exit(255)
+
+            options.server = checkServer()
+            if not options.server:
+                parser.print_help()
+                sys.exit(0)
+
+        if not options.listmodules:
+            if not options.database and not options.directory:
+                options.listmodules = True
+            elif options.database:
+                print("CONFIG SERVER: %s" % options.server)
+            else:
+                print("OUTPUT DIRECTORY: %s" % options.directory)
+
+        creator = SECoPCPCreator(options, args)
+        try:
+            if options.listmodules:
+                modules = creator.listmodules()
+                if modules:
+                    print("MODULES:\n %s" % " ".join(modules))
+            else:
+                creator.create()
+        except WrongParameterError as e:
+            sys.stderr.write(str(e))
+            sys.stderr.flush()
+            parser.print_help()
+            sys.exit(255)
+
+
 class ClientDS(Runner):
 
     """ clientds runner"""
     #: (:obj:`str`) command description
     description = "create client datasources"
 
     #: (:obj:`str`) command epilog
@@ -1353,14 +1550,15 @@
                          ('tangods', TangoDS),
                          ('deviceds', DeviceDS),
                          ('onlinecp', OnlineCP),
                          ('onlineds', OnlineDS),
                          ('poolds', PoolDS),
                          ('stdcomp', StdComp),
                          ('comp', Comp),
+                         ('secopcp', SECoPCP),
                          ('compare', Compare)]
     runners = parser.createSubParsers()
 
     try:
         options = parser.parse_args()
     except ErrorException as e:
         sys.stderr.write("Error: %s\n" % str(e))
```

### Comparing `nxstools-3.9.0/nxstools/nxscreator.py` & `nxstools-4.0.0/nxstools/nxscreator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -20,39 +19,75 @@
 """ Command-line tool for creating to the nexdatas configuration server """
 
 import copy
 import os.path
 import json
 import sys
 
+from operator import itemgetter
+
 import lxml.etree as etree
 import xml.etree.ElementTree as et
 from lxml.etree import XMLParser
 
 from nxstools.nxsdevicetools import (
     storeDataSource, getDataSourceComponents, storeComponent,
     moduleAttributes, motorModules,
     generateDeviceNames, getServerTangoHost,
     openServer, findClassName,
     xmlPackageHandler)
 from nxstools.nxsxml import (XMLFile, NDSource, NGroup, NField, NLink,
-                             NDimensions)
+                             NAttr, NDimensions)
+from nxstools.pyeval.secop import secop_cmd
 
 #: (:obj:`bool`) True if PyTango available
 PYTANGO = False
 try:
-    import PyTango
+    try:
+        import tango
+    except Exception:
+        import PyTango as tango
     PYTANGO = True
 except Exception:
     pass
 
 if sys.version_info > (3,):
     basestring = str
     unicode = str
 
+npTn = {"double": "NX_FLOAT64",
+        "int": "NX_INT64",
+        "string": "NX_CHAR",
+        "bool": "NX_BOOLEAN"}
+
+mnTme = {
+    "temperature": "temperature",
+    "temperature_regulation": "temperature",
+    "magneticfield": "magnetic_field",
+    "electricfield": "electric_field",
+    "pressure": "pressure",
+    "flowrate": "flow",
+
+    # not defined in NeXus yet
+    # "humidity": "humidity",
+    # "viscosity": "viscosity",
+    # "concentration": "concentration",
+    # "rotation_z": "rotation_z",
+
+    # not defined in secop yet
+    "ph": "pH",
+    "conductivity": "conductivity",
+    "resistance": "resistance",
+    "voltage": "voltage",
+    "surfacepressure": "surface_pressure",
+    "stress": "stress",
+    "strain": "strain",
+    "shear": "shear",
+  }
+
 
 class CPExistsException(Exception):
 
     """ Component already exists exception
     """
 
 
@@ -84,29 +119,35 @@
     """ provides xml content of the whole node
 
     :param node: DOM node
     :type node: :class:`xml.dom.Node`
     :returns: xml content string
     :rtype: :obj:`str`
     """
-    xml = _tostr(et.tostring(node, encoding='utf8', method='xml'))
+    if sys.version_info > (3,):
+        xml = _tostr(et.tostring(node, encoding='unicode', method='xml'))
+    else:
+        xml = _tostr(et.tostring(node, encoding='utf8', method='xml'))
     if xml.startswith("<?xml version='1.0' encoding='utf8'?>"):
         xml = str(xml[38:])
     return xml
 
 
 def _simpletoxml(node):
     """ provides xml content of the whole node
 
     :param node: DOM node
     :type node: :class:`xml.dom.Node`
     :returns: xml content string
     :rtype: :obj:`str`
     """
-    return _tostr(et.tostring(node, encoding='utf8', method='xml'))
+    if sys.version_info > (3,):
+        return _tostr(et.tostring(node, encoding='unicode', method='xml'))
+    else:
+        return _tostr(et.tostring(node, encoding='utf8', method='xml'))
 
 
 class Device(object):
 
     """ device from online.xml
     """
     __slots__ = [
@@ -195,15 +236,15 @@
         """
         mhost = self.sardanahostname or tangohost
         self.sdevice = None
         self.shost = None
         self.sport = None
         if PYTANGO:
             try:
-                dp = PyTango.DeviceProxy(str("%s/%s" % (mhost, self.name)))
+                dp = tango.DeviceProxy(str("%s/%s" % (mhost, self.name)))
                 mdevice = str(dp.name())
 
                 #  self.hostname = mhost
                 self.shost = mhost.split(":")[0]
                 if len(mhost.split(":")) > 1:
                     self.sport = mhost.split(":")[1]
 
@@ -231,18 +272,18 @@
             if self.attribute is None:
                 self.attribute = 'Position'
             if clientlike:
                 self.group = '__CLIENT__'
         elif PYTANGO and self.module in moduleAttributes:
             try:
                 try:
-                    dp = PyTango.DeviceProxy(
+                    dp = tango.DeviceProxy(
                         str("%s/%s" % (mhost, self.sardananame)))
                 except Exception:
-                    dp = PyTango.DeviceProxy(str("%s/%s" % (mhost, self.name)))
+                    dp = tango.DeviceProxy(str("%s/%s" % (mhost, self.name)))
                 mdevice = str(dp.name())
 
                 sarattr = moduleAttributes[self.module][0]
                 if not sarattr or \
                    sarattr not in dp.get_attribute_list():
                     raise Exception("Missing attribute: Value")
                 self.hostname = mhost
@@ -485,15 +526,16 @@
                         pathlist.append((nlist[0], "NX" + nlist[0]))
 
             pathlist.append((spath[-1], None))
         return pathlist
 
     @classmethod
     def __createTree(cls, df, nexuspath, name, nexusType,
-                     strategy, units, link, chunk, canfail=None):
+                     strategy, units, link, chunk, canfail=None,
+                     depends=None):
         """ create nexus node tree
 
         :param df: definition parent node
         :type df: :class:'nxstools.nxsxml.XMLFile'
         :param nexuspath: nexus path
         :type nexuspath: :obj:`str`
         :param name: name
@@ -506,14 +548,16 @@
         :type units: :obj:`str`
         :param links: if create link
         :type links: :obj:`bool`
         :param chunk: chunk size, e.g. `SCALAR`, `SPECTRUM` or `IMAGE`
         :type chunk: :obj:`str`
         :param canfail: can fail strategy flag
         :type canfail: :obj:`bool`
+        :param depends: a list of component dependencies separated by ','
+        :type depends: :obj:`str`
         """
 
         pathlist = cls.__patheval(nexuspath)
         entry = None
         parent = df
         for path in pathlist[:-1]:
             child = NGroup(parent, path[0], path[1])
@@ -536,19 +580,23 @@
                 npath = (nexuspath + name) \
                     if nexuspath[-1] == '/' else nexuspath
                 data = NGroup(entry, "data", "NXdata")
                 if link > 1:
                     NLink(data, name, npath)
                 else:
                     NLink(data, fname, npath)
+        if depends:
+            deps = [dp for dp in depends.split(",") if dp]
+            if deps:
+                df.setDependencies(deps, entry)
 
     @classmethod
     def _createComponent(cls, name, directory, fileprefix, nexuspath,
                          strategy, nexusType, units, links, server, chunk,
-                         dsname, canfail=None):
+                         dsname, canfail=None, depends=None):
         """ creates component file
 
         :param name: component name
         :type name: :obj:`str`
         :param directory: output file directory
         :type directory: :obj:`str`
         :param fileprefix: file name prefix
@@ -567,20 +615,22 @@
         :type server: :obj:`str`
         :returns: component xml
         :rtype: :obj:`str`
         :param dsname: datasource name
         :type dsname: :obj:`str`
         :param canfail: can fail strategy flag
         :type canfail: :obj:`bool`
+        :param depends: a list of component dependencies separated by ','
+        :type depends: :obj:`str`
         """
         defpath = "/$var.entryname#'scan'$var.serialno:NXentry/instrument" \
                   + "/collection/%s" % (dsname or name)
         df = XMLFile("%s/%s%s.xml" % (directory, fileprefix, name))
         cls.__createTree(df, nexuspath or defpath, dsname or name, nexusType,
-                         strategy, units, links, chunk, canfail)
+                         strategy, units, links, chunk, canfail, depends)
 
         xml = df.prettyPrint()
         if server:
             storeComponent(name, xml, server)
         elif directory is not None and fileprefix is not None:
             df.dump()
         return xml
@@ -721,15 +771,16 @@
                 self.options.strategy,
                 self.options.type,
                 self.options.units,
                 int(self.options.fieldlinks) + 2 * int(
                     self.options.sourcelinks),
                 self.options.server if self.options.database else None,
                 self.options.chunk, dsname,
-                self.options.canfail
+                self.options.canfail,
+                self.options.depends
             )
 
 
 class TangoDSCreator(Creator):
 
     """ tango datasource creator
     """
@@ -1429,17 +1480,18 @@
                 dv.dtype = self._getChildText(device, "type")
                 dv.module = self._getChildText(device, "module")
                 dv.tdevice = self._getChildText(device, "device")
                 dv.hostname = self._getChildText(device, "hostname")
                 dv.sardananame = self._getChildText(device, "sardananame")
                 dv.sardanahostname = self._getChildText(
                     device, "sardanahostname")
-                if name not in dct.keys():
-                    dct[dv.sardananame or name] = []
-                dct[dv.sardananame or name].append(dv)
+                sname = dv.sardananame or name
+                if sname not in dct.keys():
+                    dct[sname] = []
+                dct[sname].append(dv)
         return dct
 
     def compare(self):
         if self._printouts:
             print("Comparing: %s\n" % " ".join(self.args))
         dct1 = self._load(self.args[0])
         dct2 = self._load(self.args[1])
@@ -1719,14 +1771,843 @@
                                 self._printAction(mdv)
                                 if xmlfile.endswith(".ds.xml"):
                                     self.datasources[newname] = xml
                                 else:
                                     self.components[newname] = xml
 
 
+class SECoPCPCreator(CPCreator):
+
+    """ component creator of secop components
+    """
+
+    def __init__(self, options, args, printouts=True):
+        """ constructor
+
+        :param options: command options
+        :type options: :class:`optparse.Values`
+        :param args: command arguments
+        :type args: :obj:`list` < :obj:`str` >
+        :param printouts: if printout is enable
+        :type printouts: :obj:`bool`
+        """
+        CPCreator.__init__(self, options, args, printouts)
+
+    def _printAction(self, name, ds=False):
+        """ prints out information about the performed action
+
+        :param name: component name
+        :type name: :obj:`str`
+        """
+        if self._printouts:
+            if hasattr(self.options, "database") and \
+               self.options.database:
+                print("CREATING '%s' of secop on '%s'" % (
+                    name,
+                    self.options.server))
+            else:
+                ext = ".ds" if ds else ""
+                print("CREATING '%s' of secop in '%s/%s%s%s.xml'" % (
+                    name,
+                    self.options.directory,
+                    self.options.file,
+                    name, ext))
+
+    def listmodules(self):
+        """ provides a list of modules for the secop node
+
+        :returns: list of modules for the secop node
+        :rtype: :obj:`list` <:obj:`str` >
+        """
+        names = []
+        conf = {}
+        if self.options.json:
+            with open(self.options.json) as fl:
+                conf = json.load(fl)
+        else:
+            conf = secop_cmd(
+                "describe", self.options.host, int(self.options.port)) or {}
+        modules = conf.get("modules", {})
+        if modules:
+            names = [mname for mname in modules.keys()]
+        # print(json.dumps(conf))
+        return names
+
+    def __createSECoPTree(self, df, name, conf, samplename=None,
+                          sampleenvname=None,
+                          modulenames=None, canfail=None,
+                          environments=None,
+                          meanings=None, first=None, transattrs=None,
+                          dynamiclinks=False, samplenxdata=False):
+        """ create nexus node tree
+
+        :param df: definition parent node
+        :type df: :class:'nxstools.nxsxml.XMLFile'
+        :param name: node name
+        :type name: :obj:`str`
+        :param conf: secop configuration
+        :type conf: :obj:`dict`
+        :param samplename: sample name
+        :type samplename: :obj:`str`
+        :param sampleenvname: sample environment name
+        :type sampleenvname: :obj:`str`
+        :param modulenames: module names
+        :typae modulenames: :obj:`list` <:obj:`str`>
+        :param canfail: can fail strategy flag
+        :type canfail: :obj:`bool`
+        :param environments: environments to link separated by comman
+        :type environments: :obj:`str`
+        :param meanings: physical quantity meaning to link separated by comman
+        :type meanings: :obj:`str`
+        :param first: first targets to link separated by comman
+        :type first: :obj:`str`
+        :param transattrs: JSON dictionary with transformation attributes
+        :type transattrs: :obj:`str`
+        :param dynamiclinks: dynamic links flag
+        :type dynamiclinks: :obj:`bool`
+        :param samplenxdata: sample nxdata
+        :type samplenxdata: :obj:`bool`
+        """
+        ename = "$var.entryname#'$(__entryname__)'$var.serialno".replace(
+                    "$(__entryname__)", (self.options.entryname or "scan"))
+        entry = NGroup(df, ename, "NXentry")
+        samplename = samplename or "sample"
+        sampleenvname = sampleenvname or "sample_environment"
+        sample = NGroup(entry, samplename, "NXsample")
+        field = NField(sample, 'type', 'NX_CHAR')
+        field.setText("sample")
+        field.setStrategy('INIT')
+
+        sampleenv = NGroup(entry, sampleenvname, "NXsample")
+        field = NField(sampleenv, 'type', 'NX_CHAR')
+        field.setText("sample environment")
+        field.setStrategy('INIT')
+
+        modules = conf.get("modules", {})
+        senv = None
+        seenv = None
+
+        for mname, mconf in modules.items():
+            if mname and (not senv or not seenv):
+                if not modulenames or mname in modulenames:
+                    if not senv and "meaning" in mconf.keys():
+                        senv = NGroup(sample, name or "environment",
+                                      "NXenvironment")
+                    if not seenv and "meaning" not in mconf.keys():
+                        seenv = NGroup(sampleenv, name or "environment",
+                                       "NXenvironment")
+        envs = [senv, seenv]
+        for env in envs:
+            if env:
+                if 'equipment_id' in conf.keys():
+                    field = NField(env, 'name', 'NX_CHAR')
+                    field.setText("%s" % str(conf['equipment_id']))
+                    field.setStrategy('INIT')
+                if name or 'equipment_id' in conf.keys():
+                    field = NField(env, 'short_name', 'NX_CHAR')
+                    if name:
+                        field.setText("%s" % str(name))
+                    elif 'equipment_id' in conf.keys():
+                        field.setText("%s" % str(conf['equipment_id']))
+                    field.setStrategy('INIT')
+                if 'firmware' in conf.keys() or 'version' in conf.keys():
+                    field = NField(env, 'type', 'NX_CHAR')
+                    txt = ""
+                    if 'firmware' in conf.keys():
+                        txt = str(conf['firmware'])
+                    if 'version' in conf.keys():
+                        if txt:
+                            txt = "%s (%s)" % (txt, str(conf['version']))
+                        else:
+                            txt = "(%s)" % (str(conf['version']))
+                    field.setText(txt)
+                    field.setStrategy('INIT')
+                if 'description' in conf.keys():
+                    field = NField(env, 'description', 'NX_CHAR')
+                    field.setText("%s" % str(conf['description']))
+                    field.setStrategy('INIT')
+
+        targets = (first or "").split(",")
+        lmeanings = (meanings or "").split(",")
+        lenvironments = (environments or "").split(",")
+        try:
+            trattrs = json.loads(transattrs or "{}")
+        except Exception:
+            trattrs = {}
+        links = {}
+        for mname, mconf in modules.items():
+            if mname:
+                if not modulenames or mname in modulenames:
+                    lk = self.__createSECoPSensor(
+                        senv, seenv, mname, mconf, name, canfail, samplename,
+                        sampleenvname, trattrs)
+                    if lk and isinstance(lk, dict):
+                        links.update(lk)
+        ename = \
+            "$var.entryname#'$(__entryname__)'" \
+            "$var.serialno".replace(
+                "$(__entryname__)",
+                (self.options.entryname or "scan"))
+        created = []
+        created_trans = []
+        trans = None
+        for tg in targets:
+            try:
+                stg = "/".join(tg.split("/")[-3:])
+            except Exception:
+                stg = None
+            if tg in links.keys() or stg and stg in links.keys():
+                mn = links[tg][0]
+                NLink(sample, mn, tg)
+                created.append(mn)
+
+        llinks = sorted([(tg, mns[0], mns[1]) for tg, mns in links.items()],
+                        key=itemgetter(2), reverse=True)
+        if dynamiclinks or samplenxdata:
+            self.createSECoPLinkDS(
+                ename, samplename, sampleenvname,
+                meanings or "", environments or "")
+        if dynamiclinks:
+            ae = sample.addAttr(
+                'secop_env_links', "NX_CHAR",
+                "$datasources.sample_env_links")
+            ae.setStrategy("FINAL")
+            al = sample.addAttr(
+                'secop_log_links', "NX_CHAR",
+                "$datasources.sample_log_links")
+            al.setStrategy("FINAL")
+        if samplenxdata:
+            al = sample.addAttr(
+                'sample_nxdata', "NX_CHAR",
+                "$datasources.sample_nxdata")
+            al.setStrategy("FINAL")
+            al = sampleenv.addAttr(
+                'sampleenv_nxdata', "NX_CHAR",
+                "$datasources.sampleenv_nxdata")
+            al.setStrategy("FINAL")
+
+        for target, mn, semn in llinks:
+            starget = target.split("/")
+            if not dynamiclinks:
+                if mn in lenvironments and "%s_env" % mn not in created:
+                    env = NGroup(
+                        sample, "%s_env" % mn, "NXenvironment")
+
+                    NLink(env, starget[-2], "/".join(starget[:-1]))
+                    NLink(env, "description",
+                          "/".join(starget[:-2]) + "/description")
+                    NLink(env, "name",
+                          "/".join(starget[:-2]) + "/name")
+                    NLink(env, "short_name",
+                          "/".join(starget[:-2]) + "/short_name")
+                    NLink(env, "type", "/".join(starget[:-2]) + "/type")
+                    created.append("%s_env" % mn)
+                if mn in lmeanings and mn not in created:
+                    NLink(sample, mn, target)
+                    created.append(mn)
+
+            if mn in trattrs.keys():
+                nm = "%s_%s" % (starget[-3], starget[-2])
+                if nm not in created_trans:
+                    if trans is None:
+                        trans = NGroup(
+                            sample, "transformations", "NXtransformations")
+                    NLink(trans, nm, target + "/value")
+                    created_trans.append(nm)
+
+    def __createSECoPSensor(self, senv, seenv, name, conf, nodename,
+                            canfail=None, samplename="sample",
+                            sampleenvname="sample_environment",
+                            trattrs=None):
+        """ create nexus node tree
+
+        :param senv: definition parent node
+        :type senv: :class:'nxstools.nxsxml.XMLFile'
+        :param seenv: definition parent node
+        :type seenv: :class:'nxstools.nxsxml.XMLFile'
+        :param name: sensor name
+        :type name: :obj:`str`
+        :param conf: secop configuration
+        :type conf: :obj:`dict`
+        :param nodename: node name
+        :type nodename: :obj:`str`
+        :param canfail: can fail strategy flag
+        :type canfail: :obj:`bool`
+        :param samplename: sample group name i.e. sample
+        :type samplename: :obj:`str`
+        :param sampleenvname: sample environment group name
+        :type sampleenvname: :obj:`str`
+        :param trattrs: dictionary with transformation attributes
+        :type trattrs: :obj:`dict` <:obj:`str`,:obj:`dict` <:obj:`str`,`and`>>
+        :returns: links targets and meaning names
+        :rtype: :obj:`dict`< :obj:`str`, (:obj:`str`, :obj:`str`) >
+        """
+        if 'meaning' in conf.keys():
+            meaning = conf['meaning']
+            env = senv
+            basename = samplename
+        else:
+            meaning = None
+            env = seenv
+            basename = sampleenvname
+
+        links = {}
+        trattrs = trattrs or {}
+        mgr = NGroup(env, name, "NXsensor")
+        if 'description' in conf.keys():
+            field = NField(mgr, 'name', 'NX_CHAR')
+            field.setText("%s" % str(name))
+            field.setStrategy('INIT')
+        semeaning = None
+        if 'meaning' in conf.keys():
+            meaning = conf['meaning']
+            semeaning = meaning
+            importance = None
+            if isinstance(meaning, list):
+                if len(meaning) > 1:
+                    try:
+                        importance = int(meaning[1])
+                    except Exception:
+                        importance = None
+                if len(meaning) > 0:
+                    meaning = meaning[0]
+            if meaning in mnTme.keys():
+                meaning = mnTme[meaning]
+                field = NField(mgr, 'measurement', 'NX_CHAR')
+                field.setText(meaning)
+                field.setStrategy('INIT')
+                if importance is not None:
+                    mimp = NAttr(field, "secop_importance", "NX_INT32")
+                    mimp.setText(str(importance))
+
+        if 'implementation' in conf.keys():
+            field = NField(mgr, 'model', 'NX_CHAR')
+            field.setText("%s" % str(conf['implementation']))
+            field.setStrategy('INIT')
+        if 'description' in conf.keys():
+            field = NField(mgr, 'description', 'NX_CHAR')
+            field.setText("%s" % str(conf['description']))
+            field.setStrategy('INIT')
+        params = conf.get("accessibles", {})
+        if params:
+            par = NGroup(mgr, "parameters", "NXcollection")
+            for pname, pconf in params.items():
+                if pname:
+                    if pname == "value":
+                        di = pconf.get("datainfo")
+                        if di:
+                            dtype = di.get("type")
+                            nxtype = npTn.get(dtype, "NX_CHAR")
+                            units = di.get("unit")
+                            minval = di.get("min")
+                            maxval = di.get("max")
+                        log = NGroup(mgr, "value_log", "NXlog")
+                        field = NField(log, 'value', nxtype)
+                        if meaning:
+                            ename = \
+                                "$var.entryname#'$(__entryname__)'" \
+                                "$var.serialno".replace(
+                                    "$(__entryname__)",
+                                    (self.options.entryname or "scan"))
+                            target = "/%s/%s/%s/%s/value_log" % \
+                                (ename, basename, nodename, name)
+                            links[target] = (meaning, semeaning)
+                        dsname = "%s_%s" % (nodename, name)
+                        timedsname = "%s_%s_time" % (nodename, name)
+                        if self.options.lower:
+                            dsname = dsname.lower()
+                            timedsname = timedsname.lower()
+                        self.createSECoPDS(dsname,
+                                           "read %s:%s" % (name, pname),
+                                           dsname, "[0]")
+                        field.setText("$datasources.%s" % dsname)
+                        if units:
+                            field.setUnits(units)
+                        if meaning and meaning in trattrs.keys():
+                            try:
+                                attrs = dict(trattrs[meaning])
+                            except Exception:
+                                attrs = {}
+                            for nm, vl in attrs.items():
+                                if isinstance(vl, list):
+                                    if vl and isinstance(vl[0], str):
+                                        vct = NAttr(field, nm, "NX_CHAR")
+                                        vct.setText("\n ".join(vl))
+                                    else:
+                                        vct = NAttr(field, nm, "NX_FLOAT64")
+                                        vct.setText(
+                                            " ".join([str(st) for st in vl]))
+                                    d = NDimensions(vct, "1")
+                                    d.dim("1", str(len(vl)))
+                                    vct.setStrategy("INIT")
+                                else:
+                                    field.addTagAttr(nm, vl)
+                        strategy = self.options.strategy
+                        field.setStrategy(strategy)
+                        field = NField(log, 'time', "NX_FLOAT64")
+                        field.setText(
+                            "$datasources.%s" % timedsname)
+                        at = field.addAttr(
+                            'start', "NX_DATE_TIME",
+                            "$datasources.client_start_time")
+                        at.setStrategy("INIT")
+                        field.setUnits("s")
+                        field.setStrategy(strategy)
+                        if minval:
+                            field = NField(log, 'minimal_value', nxtype)
+                            field.setStrategy('INIT')
+                            field.setText(str(minval))
+                            if units:
+                                field.setUnits(units)
+                        if maxval:
+                            field = NField(log, 'maximal_value', nxtype)
+                            field.setStrategy('INIT')
+                            field.setText(str(maxval))
+                            if units:
+                                field.setUnits(units)
+                    elif pname == "status":
+                        self.__createSECoPParam(
+                            par, pname, pconf, nodename, name, canfail,
+                            "[0,0]", "int")
+                    else:
+                        self.__createSECoPParam(
+                            par, pname, pconf, nodename, name, canfail)
+                        if pname == "target":
+                            ename = \
+                                "$var.entryname#'$(__entryname__)'" \
+                                "$var.serialno".replace(
+                                    "$(__entryname__)",
+                                    (self.options.entryname or "scan"))
+                            NLink(mgr, "value",
+                                  "/%s/%s/%s/%s/parameters/target/value" %
+                                  (ename, basename, nodename, name))
+        return links
+
+    def __createSECoPParam(self, par, name, conf, nodename, modname,
+                           canfail=None, access=None, accesstype=None):
+        """ create nexus node tree
+
+        :param env: definition parent node
+        :type env: :class:'nxstools.nxsxml.XMLFile'
+        :param name: parameter name
+        :type name: :obj:`str`
+        :param conf: secop configuration
+        :type conf: :obj:`dict`
+        :param nodename: node name
+        :type nodename: :obj:`str`
+        :param modname: sensor name
+        :type modname: :obj:`str`
+        :param canfail: can fail strategy flag
+        :type canfail: :obj:`bool`
+        """
+        di = conf.get("datainfo")
+        if di:
+            dtype = di.get("type")
+            if dtype == "command":
+                return
+            if dtype not in npTn.keys() and not access:
+                return
+            nxtype = npTn.get(dtype, "NX_CHAR")
+            if accesstype in npTn.keys():
+                nxtype = npTn.get(accesstype)
+            units = di.get("unit")
+            minval = di.get("min")
+            maxval = di.get("max")
+        access = access or "[0]"
+        log = NGroup(par, name, "NXlog")
+        field = NField(log, "value", nxtype)
+        dsname = "%s_%s_%s" % (nodename, modname, name)
+        timedsname = "%s_%s_%s_time" % (nodename, modname, name)
+        if self.options.lower:
+            dsname = dsname.lower()
+            timedsname = timedsname.lower()
+        field.setText("$datasources.%s" % (dsname))
+        pstrategy = self.options.paramstrategy
+        self.createSECoPDS(dsname,
+                           "read %s:%s" % (modname, name),
+                           dsname, access)
+        field.setStrategy(pstrategy)
+        if units:
+            field.setUnits(units)
+        field = NField(log, 'time', "NX_FLOAT64")
+        field.setText(
+            "$datasources.%s" % timedsname)
+        at = field.addAttr(
+            'start', "NX_DATE_TIME", "$datasources.client_start_time")
+        at.setStrategy("INIT")
+        field.setUnits("s")
+        field.setStrategy(pstrategy)
+        if minval:
+            field = NField(log, 'minimal_value', nxtype)
+            field.setStrategy('INIT')
+            field.setText(str(minval))
+            if units:
+                field.setUnits(units)
+        if maxval:
+            field = NField(log, 'maximal_value', nxtype)
+            field.setStrategy('INIT')
+            field.setText(str(maxval))
+            if units:
+                field.setUnits(units)
+
+    def createXMLs(self):
+        """ creates component xmls of all online.xml complex devices
+        """
+        self.datasources = {}
+        self.components = {}
+        cpnames = self.args
+        conf = {}
+        if self.options.json:
+            with open(self.options.json) as fl:
+                conf = json.load(fl)
+        else:
+            conf = secop_cmd(
+                "describe", self.options.host, int(self.options.port))
+        if isinstance(conf, dict):
+            # dump = \
+            #     json.dumps(conf, sort_keys=True, indent=4)
+            # print("%s" % dump)
+            cpname = self.options.component
+            if 'description' in conf.keys() and not cpname:
+                eid = str(conf['equipment_id']).split(".")
+                if eid and eid[0]:
+                    cpname = eid[0]
+                else:
+                    des = str(conf['description']).split("\n")
+                    if des and des[0]:
+                        cpname = des[0]
+                cpname = cpname.replace("[", "").\
+                    replace("]", "_").replace(",", "_")
+                if not cpname:
+                    cpname = "secop"
+            fname = "%s%s.xml" % (self.options.file, cpname)
+            if self.options.lower:
+                fname = fname.lower()
+                cpname = cpname.lower()
+            df = XMLFile("%s/%s" % (self.options.directory, fname))
+            self.__createSECoPTree(df, cpname, conf, self.options.samplename,
+                                   self.options.sampleenvname,
+                                   cpnames, self.options.canfail,
+                                   self.options.environments,
+                                   self.options.meanings,
+                                   self.options.first,
+                                   self.options.transattrs,
+                                   self.options.dynamiclinks,
+                                   self.options.samplenxdata)
+            self._printAction(cpname)
+            self.components[cpname] = df.prettyPrint()
+
+    def createSECoPDS(self, dsname, message, group=None, access=None,
+                      host=None, port=None, timeout=None):
+        """ create SECoP datasource
+
+        :param dsname: datasource name
+        :type dsname: :obj:`str`
+        :param message: secop command
+        :type message: :obj:`str`
+        :param group: secop group name
+        :type group: :obj:`str`
+        :param access: secop attribute access list
+        :type access: :obj:`str`
+        :param host: secop host name
+        :type host: :obj:`str`
+        :param port: secop port name
+        :type port: :obj:`str` or :obj:`int`
+        :param port: minimum timeout
+        :type port: :obj:`str` or :obj:`float`
+        """
+        if access is not None and group is not None:
+            module = 'groupsecop'
+        elif group is not None:
+            module = 'secop'
+        else:
+            module = 'singlesecop'
+
+        if module in self.xmlpackage.standardComponentTemplateFiles:
+            xmlfiles = self.xmlpackage.standardComponentTemplateFiles[module]
+        else:
+            if os.path.isfile("%s/%s.xml" % (self.xmltemplatepath, module)):
+                xmlfiles = ["%s.xml" % module]
+        params = {}
+
+        host = self.options.host if host is None else host
+        port = self.options.port if port is None else port
+        timeout = str(self.options.timeout) \
+            if timeout is None else str(timeout)
+        if host is not None:
+            params["host"] = host
+        if port is not None:
+            params["port"] = str(port)
+        if message:
+            params["message"] = message
+        if timeout:
+            params["timeout"] = timeout
+        if access:
+            params["access"] = access
+        if group:
+            params["group"] = group
+        if self.options.lower:
+            dsname = dsname.lower()
+
+        for xmlfile in xmlfiles:
+            # print(xmlfile)
+            newname = self._replaceName(xmlfile, dsname, module)
+            with open(
+                    '%s/%s' % (
+                        self.xmltemplatepath, xmlfile), "r"
+            ) as content_file:
+                xmlcontent = content_file.read()
+                xml = xmlcontent.replace("$(name)", dsname)
+                missing = []
+                for var, desc in self.xmlpackage.standardComponentVariables[
+                        module].items():
+                    if var in params.keys():
+                        xml = xml.replace("$(%s)" % var, params[var])
+                    elif desc["default"] is not None:
+                        xml = xml.replace("$(%s)" % var, desc["default"])
+                    else:
+                        missing.append(var)
+                if missing:
+                    if sys.version_info > (3,):
+                        root = et.fromstring(
+                            bytes(xml, "UTF-8"),
+                            parser=XMLParser(collect_ids=False))
+                    else:
+                        root = et.fromstring(
+                            xml,
+                            parser=XMLParser(collect_ids=False))
+                    nodes = root.findall(".//attribute")
+                    nodes.extend(root.findall(".//field"))
+                    nodes.extend(root.findall(".//link"))
+                    grnodes = root.findall(".//group")
+                    for node in nodes:
+                        text = self.__getText(node)
+                        for ms in missing:
+                            label = "$(%s)" % ms
+                            if label in text:
+                                parent = node.getparent()
+                                parent.remove(node)
+                                break
+                    for node in grnodes:
+                        text = node.attrib["name"]
+                        if text and "$(" in text:
+                            for ms in missing:
+                                label = "$(%s)" % ms
+                                if label in text:
+                                    parent = node.getparent()
+                                    parent.remove(node)
+                                    break
+                    xml = _simpletoxml(root)
+                    if self._printouts:
+                        print("MISSING %s" % missing)
+                    errors = []
+                    for var in missing:
+                        if "s.$(%s)" % var in xml:
+                            errors.append(var)
+                    if errors:
+                        print(
+                            "WARNING: %s cannot be created without %s"
+                            % (var, errors))
+                        continue
+
+                    for var in missing:
+                        xml = xml.replace("$(%s)" % var, "")
+                    lines = xml.split('\n')
+                    xml = '\n'.join([x for x in lines if len(x.strip())])
+                if xmlfile.endswith(".ds.xml"):
+                    self._printAction(newname, True)
+                    self.datasources[newname] = xml
+                else:
+                    self._printAction(newname)
+                    self.components[newname] = xml
+
+    def createSECoPLinkDS(self, entryname, samplename, sampleenvname,
+                          meanings, environments):
+        """ create SECoP datasource
+
+        :param entryname: secop entry name
+        :type entryname: :obj:`str`
+        :param samplename: secop sample name
+        :type samplename: :obj:`str`
+        :param sampleenvname: secop sample name
+        :type sampleenvname: :obj:`str`
+        :param meanings: secop meanings list
+        :type meanings: :obj:`str`
+        :param environments: secop environments list
+        :type environments: :obj:`str`
+        """
+        module = 'secoplinks'
+        dsname = "secop"
+
+        if module in self.xmlpackage.standardComponentTemplateFiles:
+            xmlfiles = self.xmlpackage.standardComponentTemplateFiles[module]
+        else:
+            if os.path.isfile("%s/%s.xml" % (self.xmltemplatepath, module)):
+                xmlfiles = ["%s.xml" % module]
+        params = {}
+
+        params["entryname"] = entryname
+        params["samplename"] = samplename
+        params["sampleenvname"] = sampleenvname
+        params["meanings"] = meanings
+        params["environments"] = environments
+        if self.options.lower:
+            dsname = dsname.lower()
+
+        for xmlfile in xmlfiles:
+            # print(xmlfile)
+            newname = self._replaceName(xmlfile, dsname, module)
+            with open(
+                    '%s/%s' % (
+                        self.xmltemplatepath, xmlfile), "r"
+            ) as content_file:
+                xmlcontent = content_file.read()
+                xml = xmlcontent.replace("$(name)", dsname).replace(
+                    "$(__entryname__)",
+                    (self.options.entryname or "scan")).replace(
+                        "$(__insname__)",
+                        (self.options.insname
+                         or "instrument"))
+                missing = []
+                for var, desc in self.xmlpackage.standardComponentVariables[
+                        module].items():
+                    if var in params.keys():
+                        xml = xml.replace("$(%s)" % var, params[var])
+                    elif desc["default"] is not None:
+                        xml = xml.replace("$(%s)" % var, desc["default"])
+                    else:
+                        missing.append(var)
+                if missing:
+                    if sys.version_info > (3,):
+                        root = et.fromstring(
+                            bytes(xml, "UTF-8"),
+                            parser=XMLParser(collect_ids=False))
+                    else:
+                        root = et.fromstring(
+                            xml,
+                            parser=XMLParser(collect_ids=False))
+                    nodes = root.findall(".//attribute")
+                    nodes.extend(root.findall(".//field"))
+                    nodes.extend(root.findall(".//link"))
+                    grnodes = root.findall(".//group")
+                    for node in nodes:
+                        text = self.__getText(node)
+                        for ms in missing:
+                            label = "$(%s)" % ms
+                            if label in text:
+                                parent = node.getparent()
+                                parent.remove(node)
+                                break
+                    for node in grnodes:
+                        text = node.attrib["name"]
+                        if text and "$(" in text:
+                            for ms in missing:
+                                label = "$(%s)" % ms
+                                if label in text:
+                                    parent = node.getparent()
+                                    parent.remove(node)
+                                    break
+                    xml = _simpletoxml(root)
+                    if self._printouts:
+                        print("MISSING %s" % missing)
+                    errors = []
+                    for var in missing:
+                        if "s.$(%s)" % var in xml:
+                            errors.append(var)
+                    if errors:
+                        print(
+                            "WARNING: %s cannot be created without %s"
+                            % (var, errors))
+                        continue
+
+                    for var in missing:
+                        xml = xml.replace("$(%s)" % var, "")
+                    lines = xml.split('\n')
+                    xml = '\n'.join([x for x in lines if len(x.strip())])
+                if xmlfile.endswith(".ds.xml"):
+                    self._printAction(newname, True)
+                    self.datasources[newname] = xml
+                else:
+                    self._printAction(newname)
+                    self.components[newname] = xml
+
+    def create(self):
+        """ creates components of all online.xml complex devices
+        """
+        cpnames = self.args
+        for cpname in cpnames:
+            if hasattr(self.options, "database") and \
+               self.options.database:
+                server = self.options.server
+                if not self.options.overwrite:
+                    if self._areComponentsAvailable(
+                            [cpname], server, self.options.lower):
+                        raise CPExistsException(
+                            "Component '%s' already exists." % cpname)
+            elif not self.options.overwrite:
+                existing = self._componentFilesExist(
+                    [cpname], self.options.file, self.options.directory)
+                if existing:
+                    raise CPExistsException(
+                        "Component files '%s' already exist." % existing)
+
+        self.createXMLs()
+        if not self.datasources and not self.components:
+            raise CPExistsException(
+                "Warning: Components %s cannot be created" % cpnames)
+        server = self.options.server
+        if hasattr(self.options, "database") and \
+           self.options.database:
+            for dsname, dsxml in self.datasources.items():
+                storeDataSource(dsname, dsxml, server)
+            for cpname, cpxml in self.components.items():
+                mand = False
+                if hasattr(self.options, "mandatory") and \
+                   self.options.mandatory:
+                    mand = True
+                storeComponent(cpname, cpxml, server, mand)
+        else:
+            for dsname, dsxml in self.datasources.items():
+                with open("%s/%s%s.ds.xml" % (
+                        self.options.directory,
+                        self.options.file, dsname), "w") as myfile:
+                    myfile.write(dsxml)
+            for cpname, cpxml in self.components.items():
+                # print(cpname)
+                with open("%s/%s%s.xml" % (
+                        self.options.directory,
+                        self.options.file, cpname), "w") as myfile:
+                    # print("%s/%s%s.xml" % (
+                    #     self.options.directory,
+                    #     self.options.file, cpname))
+                    myfile.write(cpxml)
+
+    @classmethod
+    def _replaceName(cls, filename, cpname, module=None):
+        """ replaces name prefix of xml templates files
+
+        :param filename: template filename
+        :type filename: :obj:`str`
+        :param cpname: output prefix
+        :type cpname: :obj:`str`
+        :param module: module name
+        :type module: :obj:`str`
+        :returns: output filename
+        :rtype: :obj:`str`
+        """
+        if filename.endswith(".ds.xml"):
+            filename = filename[:-7]
+        elif filename.endswith(".xml"):
+            filename = filename[:-4]
+        sname = filename.split("_")
+        if not module or module == sname[0]:
+            sname[0] = cpname
+        return "_".join(sname)
+
+
 class StandardCPCreator(CPCreator):
 
     """ component creator of standard templates
     """
 
     def __init__(self, options, args, printouts=True):
         """ constructor
@@ -1806,15 +2687,15 @@
         xmlfiles = []
         if module in self.xmlpackage.standardComponentTemplateFiles:
             xmlfiles = self.xmlpackage.standardComponentTemplateFiles[module]
         else:
             if os.path.isfile("%s/%s.xml" % (self.xmltemplatepath, module)):
                 xmlfiles = ["%s.xml" % module]
         for xmlfile in xmlfiles:
-            print(xmlfile)
+            # print(xmlfile)
             newname = self._replaceName(xmlfile, cpname, module)
             with open(
                     '%s/%s' % (
                         self.xmltemplatepath, xmlfile), "r"
             ) as content_file:
                 xmlcontent = content_file.read()
                 xml = xmlcontent.replace("$(name)", cpname).replace(
```

### Comparing `nxstools-3.9.0/nxstools/nxsdata.py` & `nxstools-4.0.0/nxstools/nxsdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
```

### Comparing `nxstools-3.9.0/nxstools/nxsdevicetools.py` & `nxstools-4.0.0/nxstools/nxsdevicetools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -151,18 +150,21 @@
 #: (:obj:`list` <:obj:`str`>) modules of 1D detectors
 oneDModules = ['mca_xia']
 
 #: (:obj:`list` <:obj:`str`>) IO register modules
 ioRegModules = ['sis3610']
 
 
-#: (:obj:`bool`) True if PyTango available
+#: (:obj:`bool`) True if tango available
 PYTANGO = False
 try:
-    import PyTango
+    try:
+        import tango
+    except Exception:
+        import PyTango as tango
     PYTANGO = True
 except Exception:
     pass
 
 
 for mn in motorModules:
     moduleAttributes[mn] = ['Position', 'Position']
@@ -204,52 +206,52 @@
     :type host: :obj:`str`
     :param port: device port
     :type port: :obj:`int`
     :returns: list of device attributes
     :rtype: :obj:`list` <:obj:`str`>
     """
     if host:
-        dp = PyTango.DeviceProxy("%s:%s/%s" % (host, port, device))
+        dp = tango.DeviceProxy("%s:%s/%s" % (host, port, device))
     else:
-        dp = PyTango.DeviceProxy(device)
+        dp = tango.DeviceProxy(device)
     attr = dp.attribute_list_query()
     return [at.name for at in attr if at.name not in ['State', 'Status']]
 
 
 def openServer(device):
     """ opens connection to the configuration server
 
     :param configuration: server device name
     :type configuration: :obj:`str`
     :returns: configuration server proxy
-    :rtype: :class:`PyTango.DeviceProxy`
+    :rtype: :class:`tango.DeviceProxy`
     """
     found = False
     cnt = 0
     # spliting character
     try:
         #: configuration server proxy
-        cnfServer = PyTango.DeviceProxy(device)
-    except PyTango.DevFailed:
+        cnfServer = tango.DeviceProxy(device)
+    except tango.DevFailed:
         found = True
 
     if found:
         sys.stderr.write(
             "Error: Cannot connect to the server: %s\n" % device)
         sys.stderr.flush()
         sys.exit(0)
 
     while not found and cnt < 1000:
         if cnt > 1:
-            time.sleep(0.01)
+            time.sleep(0.02)
         try:
-            if cnfServer.state() != PyTango.DevState.RUNNING:
+            if cnfServer.state() != tango.DevState.RUNNING:
                 found = True
-        except PyTango.DevFailed:
-            time.sleep(0.01)
+        except tango.DevFailed:
+            time.sleep(0.02)
             found = False
         cnt += 1
 
     if not found:
         sys.stderr.write("Error: Setting up %s takes to long\n" % device)
         sys.stderr.flush()
         sys.exit(0)
@@ -282,15 +284,15 @@
     :rtype: :obj:`str`
     """
     if server:
         proxy = openServer(server)
         host = proxy.get_db_host()
         port = proxy.get_db_port()
     else:
-        db = PyTango.Database()
+        db = tango.Database()
         host = db.get_db_host().split(".")[0]
         port = db.get_db_port()
     shost = str(host).split(".")
     if len(shost) > 0:
         host = shost[0]
     return "%s:%s" % (host, port)
 
@@ -361,15 +363,15 @@
 
     :param devicename: device name
     :type devicename: :obj:`str`
     :returns: class name
     :rtype: :obj:`str`
    """
     try:
-        db = PyTango.Database()
+        db = tango.Database()
     except Exception:
         sys.stderr.write(
             "Info: Cannot connect to %s" % devicename
             + " on host %s\n" % os.environ['TANGO_HOST'])
         sys.stderr.flush()
         return ""
 
@@ -382,15 +384,15 @@
     :param name: server instance name
     :type name: :obj:`str`
     :returns: list of the server device names
     :rtype: :obj:`list` <:obj:`str`>
     """
 
     try:
-        db = PyTango.Database()
+        db = tango.Database()
     except Exception:
         sys.stderr.write(
             "Error: Cannot connect to %s" % name
             + " on host %s\n" % os.environ['TANGO_HOST'])
         sys.stderr.flush()
         return ""
 
@@ -404,15 +406,15 @@
     :param server: remove tango server device name
     :type server: :obj:`str`
     :param func: executed function
     :type func: :obj:`instancemethod`
     :param args: function list arguments
     :type args: :obj:`list` <`and`>
     :param kwargs: function dict arguments
-    :type args: :obj:`dict` <:obj:`str` , `any`>
+    :type kwargs: :obj:`dict` <:obj:`str` , `any`>
     :returns: function result
     :rtype: `any`
     """
     lserver = None
     localtango = None
     if server and ":" in server and server.strip():
         lserver = server.split("/")[0]
```

### Comparing `nxstools-3.9.0/nxstools/nxsetup.py` & `nxstools-4.0.0/nxstools/nxsetup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -16,20 +15,25 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """ Set Up NeXus Tango Servers"""
 
 import socket
-import PyTango
 import os
 import sys
 import time
 import json
 import argparse
+import subprocess
+
+try:
+    import tango
+except Exception:
+    import PyTango as tango
 
 from nxstools.nxsargparser import (Runner, NXSArgParser, ErrorException)
 
 #: (:obj:`str`) host name
 _hostname = socket.gethostname()
 
 
@@ -85,28 +89,30 @@
                    'user': 'p01user', 'dbname': 'nxsconfig'},
     'haspp01eh2': {'beamline': 'p01', 'masterhost': 'haspp01eh2',
                    'user': 'p01user', 'dbname': 'nxsconfig'},
     'haspp01eh3': {'beamline': 'p01', 'masterhost': 'haspp01eh3',
                    'user': 'p01user', 'dbname': 'nxsconfig'},
     'haspp02ch1a': {'beamline': 'p02', 'masterhost': 'haspp02ch1a',
                     'user': 'p02user', 'dbname': 'nxsconfig'},
-    'haspp021ch1a': {'beamline': 'p02', 'masterhost': 'haspp021ch1a',
+    'haspp021ch1a': {'beamline': 'p021', 'masterhost': 'haspp021ch1a',
                      'user': 'p021user', 'dbname': 'nxsconfig'},
     'haspp02ch1': {'beamline': 'p02', 'masterhost': 'haspp02ch1',
                    'user': 'p02user', 'dbname': 'nxsconfig'},
     'haspp021ch1': {'beamline': 'p02', 'masterhost': 'haspp021ch1',
                     'user': 'p021user', 'dbname': 'nxsconfig'},
     'haspp02ch2': {'beamline': 'p02', 'masterhost': 'haspp02ch2',
                    'user': 'p02user', 'dbname': 'nxsconfig'},
     'haspp02oh1': {'beamline': 'p02', 'masterhost': 'haspp02oh1',
                    'user': 'p02user', 'dbname': 'nxsconfig'},
     'haspp02lakl': {'beamline': 'p02', 'masterhost': 'haspp02lakl',
                     'user': 'p02user', 'dbname': 'nxsconfig'},
     'haspp022ch': {'beamline': 'p022', 'masterhost': 'haspp022ch',
                    'user': 'p022user', 'dbname': 'nxsconfig'},
+    'haspp022chms': {'beamline': 'p022', 'masterhost': 'haspp022chms',
+                     'user': 'p022user', 'dbname': 'nxsconfig'},
     'haso224w': {'beamline': 'p02', 'masterhost': 'haso224w',
                  'user': 'p021user', 'dbname': 'nxsconfig'},
     'haso232s': {'beamline': 'p02', 'masterhost': 'haspp232s',
                  'user': 'p02user', 'dbname': 'nxsconfig'},
     'haspp021jenkins': {'beamline': 'p021', 'masterhost': 'haspp021jenkins',
                         'user': 'p021user', 'dbname': 'nxsconfig'},
     'haspp03': {'beamline': 'p03', 'masterhost': 'haspp03',
@@ -227,16 +233,16 @@
     """ setup NXSDataWriter, NXSConfigServer and NXSRecSelector Tango servers
     """
 
     def __init__(self):
         """ constructor
         """
         try:
-            #: (:class:`PyTango.Database`) tango database server
-            self.db = PyTango.Database()
+            #: (:class:`tango.Database`) tango database server
+            self.db = tango.Database()
         except Exception:
             print("Can't connect to tango database on %s" %
                   os.getenv('TANGO_HOST'))
             sys.exit(255)
 
         #: (:obj:`str`) NeXus writer device name
         self.writer_name = None
@@ -418,35 +424,35 @@
                     if verbose:
                         sys.stdout.write(".")
                         sys.stdout.flush()
                     adminproxy.UpdateServersInfo()
                     # running = adminproxy.RunningServers
                     running = adminproxy.DevGetRunningServers(True)
                     if server in running:
-                        time.sleep(0.01)
+                        time.sleep(0.02)
                         cnt += 1
                         continue
                     else:
                         running = False
                 if device:
                     if verbose:
                         sys.stdout.write(".")
                         sys.stdout.flush()
                     exl = self.db.get_device_exported(device)
                     if device in exl.value_string:
-                        time.sleep(0.01)
+                        time.sleep(0.02)
                         cnt += 1
                         continue
                 found = False
                 if verbose:
                     if device or server:
                         print(" %s is not working" % (device or server))
             except Exception as e:
                 print(str(e))
-                time.sleep(0.01)
+                time.sleep(0.02)
                 found = True
             cnt += 1
         if waitforproc:
             time.sleep(1.5)
         return found
 
     def waitServerRunning(self, server=None, device=None,
@@ -477,64 +483,107 @@
             try:
                 if device and not exported:
                     if verbose:
                         sys.stdout.write(".")
                         sys.stdout.flush()
                     exl = self.db.get_device_exported(device)
                     if device not in exl.value_string:
-                        time.sleep(0.01)
+                        time.sleep(0.02)
                         cnt += 1
                         continue
                     else:
                         exported = True
                 if server is not None and adminproxy is not None:
                     if verbose:
                         sys.stdout.write(".")
                         sys.stdout.flush()
                     adminproxy.UpdateServersInfo()
                     # running = adminproxy.RunningServers
                     running = adminproxy.DevGetRunningServers(True)
                     if server not in running:
-                        time.sleep(0.01)
+                        time.sleep(0.02)
                         cnt += 1
                         continue
                 found = True
                 if verbose:
                     if device or server:
                         print(" %s is working" % (device or server))
             except Exception as e:
                 print(str(e))
-                time.sleep(0.01)
+                time.sleep(0.02)
                 found = False
             cnt += 1
         if waitforproc:
             time.sleep(1.5)
         return found
 
-    def restartServer(self, name, host=None, level=None, restart=True):
+    def killServer(self, server):
+        sserver = server.split("/")
+        if len(sserver) > 1:
+            sname = sserver[0]
+            instance = sserver[1]
+        if sys.version_info > (3,):
+            with subprocess.Popen(
+                    "ps -ef | grep '%s %s' | grep -v grep"
+                    % (sname, instance),
+                    stdout=subprocess.PIPE, shell=True) as proc:
+
+                pipe = proc.stdout
+                res = str(pipe.read(), "utf8").split("\n")
+                for r in res:
+                    sr = r.split()
+                    if len(sr) > 2:
+                        subprocess.call(
+                            "kill -9 %s" % sr[1], stderr=subprocess.PIPE,
+                            shell=True)
+                pipe.close()
+        else:
+            pipe = subprocess.Popen(
+                "ps -ef | grep '%s %s' | grep -v grep"
+                % (sname, instance),
+                stdout=subprocess.PIPE, shell=True).stdout
+
+            res = str(pipe.read()).split("\n")
+            for r in res:
+                sr = r.split()
+                if len(sr) > 2:
+                    subprocess.call(
+                        "kill -9 %s" % sr[1], stderr=subprocess.PIPE,
+                        shell=True)
+            pipe.close()
+
+    def restartServer(self, name, host=None, level=None,
+                      restart=True, stopstart=True, wait=True,
+                      timeout=None):
         """ restarts server
 
         :param name: server name
         :type name: :obj:`str`
         :param host: server host name
         :type host: :obj:`str`
         :param level: start up level
         :type level: :obj:`int`
         :param restart:  if server should be restarted
         :type restart: :obj:`bool`
+        :param stopstart:  if server should be stopped and started
+        :type stopstart: :obj:`bool`
+        :param wait:  script should wait for the server
+        :type wait: :obj:`bool`
+        :param timeout: timeout for  start
+        :type timeout: :obj:`float`
         """
         if name:
             admin = self.getStarterName(host)
             if not admin:
                 raise Exception("Starter tango server is not running")
             if admin:
                 servers = None
                 started = None
                 try:
-                    adminproxy = PyTango.DeviceProxy(admin)
+                    adminproxy = tango.DeviceProxy(admin)
                     adminproxy.UpdateServersInfo()
                     servers = self.__registered_servers()
                     started = adminproxy.DevGetRunningServers(True)
                 except Exception:
                     pass
                 if servers:
                     for vl in set(servers):
@@ -547,45 +596,60 @@
                                 cname = svl
                             else:
                                 cname = svl.split('/')[0]
                             if cname == name:
                                 if level is not None:
                                     self._changeLevel(
                                         svl, level, tohigher=False)
-                                if started and svl in started:
+                                problems = False
+                                if stopstart:
+                                    if started and svl in started:
+                                        try:
+                                            # adminproxy.HardKillServer(svl)
+                                            adminproxy.DevStop(svl)
+                                            # self.killServer(svl)
+                                        except Exception:
+                                            adminproxy.HardKillServer(svl)
+                                        problems = self.waitServerNotRunning(
+                                            svl, None, adminproxy,
+                                            verbose=None)
+                                        if problems:
+                                            self.killServer(svl)
+                                            print("Server Running")
+                                        sys.stdout.write(
+                                            "Restarting: %s" % svl)
+                                    else:
+                                        sys.stdout.write("Starting: %s" % svl)
+                                    sys.stdout.flush()
+                                    problems = True
+                                    counter = 0
+                                    while problems and counter < 100:
+                                        try:
+                                            sys.stdout.write('.')
+                                            sys.stdout.flush()
+                                            adminproxy.DevStart(svl)
+                                            problems = False
+                                        except Exception:
+                                            counter += 1
+                                            time.sleep(0.4)
+                                if wait:
                                     try:
-                                        adminproxy.DevStop(svl)
+                                        maxcnt = int(float(timeout)/0.2)
                                     except Exception:
-                                        adminproxy.HardKillServer(svl)
-                                    problems = self.waitServerNotRunning(
-                                        svl, None, adminproxy, verbose=None)
+                                        maxcnt = 1000
+                                    problems = not self.waitServerRunning(
+                                        svl, None, adminproxy, maxcnt) \
+                                        or problems
                                     if problems:
-                                        print("Server Running")
-                                    sys.stdout.write("Restarting: %s" % svl)
+                                        print("%s was not restarted" % svl)
+                                        print("Warning: "
+                                              "Process with the server"
+                                              "instance could be suspended")
                                 else:
-                                    sys.stdout.write("Starting: %s" % svl)
-                                sys.stdout.flush()
-                                problems = True
-                                counter = 0
-                                while problems and counter < 100:
-                                    try:
-                                        sys.stdout.write('.')
-                                        sys.stdout.flush()
-                                        adminproxy.DevStart(svl)
-                                        problems = False
-                                    except Exception:
-                                        counter += 1
-                                        time.sleep(0.2)
-                                problems = not self.waitServerRunning(
-                                    svl, None, adminproxy) or problems
-                                print(" ")
-                                if problems:
-                                    print("%s was not restarted" % svl)
-                                    print("Warning: Process with the server"
-                                          "instance could be suspended")
+                                    print("")
 
     def __exported_servers(self):
         """ returns Servers for exported devices
 
         :rtype: :obj:`list` <:obj:`str`>
         :returns: server list
         """
@@ -618,15 +682,15 @@
             admin = self.getStarterName(host)
             if not admin:
                 raise Exception("Starter tango server is not running")
             if admin:
                 servers = None
                 started = None
                 try:
-                    adminproxy = PyTango.DeviceProxy(admin)
+                    adminproxy = tango.DeviceProxy(admin)
                     adminproxy.UpdateServersInfo()
                     started = adminproxy.DevGetRunningServers(True)
                     servers = self.__registered_servers()
                 except Exception:
                     pass
                 if servers:
                     for vl in set(servers):
@@ -665,40 +729,42 @@
         """
         sinfo = self.db.get_server_info(name)
         if not tohigher or level > sinfo.level:
             sinfo.level = level
         self.db.put_server_info(sinfo)
         return True
 
-    def _startupServer(self, new, level, host, ctrl, device):
+    def _startupServer(self, new, level, host, ctrl, device, postpone=False):
         """ starts the server up
 
         :param new: new server name
         :type new: :obj:`str`
         :param level: startup level
         :type level: :obj:`int`
         :param host: tango host name
         :type host: :obj:`str`
         :param ctrl: control mode
         :type ctrl: :obj:`str`
         :param device: device name
         :type device: :obj:`str`
+        :param postpone: postpone start server
+        :type postpone: :obj:`bool`
         :returns: True if server was started up
         :rtype: :obj:`bool`
         """
         server = self.db.get_server_class_list(new)
         if len(server) == 0:
             sys.stderr.write('Server ' + new.split('/')[0]
                              + ' not defined in database\n')
             sys.stderr.flush()
             return False
         admin = self.getStarterName(host)
         if not admin:
             raise Exception("Starter tango server is not running")
-        adminproxy = PyTango.DeviceProxy(admin)
+        adminproxy = tango.DeviceProxy(admin)
         startdspaths = self.db.get_device_property(
             admin,
             "StartDsPath")["StartDsPath"]
         if '/usr/bin' not in startdspaths:
             if startdspaths:
                 startdspaths = [p for p in startdspaths if p]
             else:
@@ -713,32 +779,35 @@
         sinfo.host = host
         sinfo.mode = ctrl
         sinfo.level = level
         self.db.put_server_info(sinfo)
         adminproxy.UpdateServersInfo()
         running = adminproxy.DevGetRunningServers(True)
         # running = adminproxy.RunningServers
-        if new not in running:
+        if new not in running and not postpone:
             adminproxy.DevStart(new)
         else:
             print("%s NOT STARTED" % new)
 
         adminproxy.UpdateServersInfo()
 
-        sys.stdout.write("waiting for server ")
-        sys.stdout.flush()
-        return self.waitServerRunning(new, device, adminproxy)
+        if not postpone:
+            sys.stdout.write("waiting for server ")
+            sys.stdout.flush()
+            return self.waitServerRunning(new, device, adminproxy)
 
-    def createDataWriter(self, beamline, masterhost):
+    def createDataWriter(self, beamline, masterhost, postpone=False):
         """ creates data writer
 
         :param beamline: beamline name
         :type beamline: :obj:`str`
         :param masterhost: master host of data writer
         :type masterhost: :obj:`str`
+        :param postpone: postpone starting flag
+        :type postpone: :obj:`bool`
         :returns: True if server was created
         :rtype: :obj:`bool`
         """
         if not beamline:
             print("createDataWriter: no beamline given ")
             return False
         if not masterhost:
@@ -753,15 +822,15 @@
         if server_name not in self.db.get_server_list(server_name):
             print("creating: %s" % server_name)
 
             if server_name in self.db.get_server_list(server_name):
                 print("createDataWriter: DB contains already %s" % server_name)
                 return False
 
-            di = PyTango.DbDevInfo()
+            di = tango.DbDevInfo()
             di.name = self.writer_name
             di._class = class_name
             di.server = server_name
 
             self.db.add_device(di)
             self.db.put_device_property(self.writer_name,
                                         {'NumberOfThreads': 100})
@@ -770,27 +839,109 @@
               self.db.get_device_class_list(server_name).value_string):
             print("\ncreateDataWriter: %s already exists. "
                   "To change its device name please remove it." % server_name)
             return False
 
         hostname = socket.gethostname()
 
-        self._startupServer(full_class_name, 1, hostname, 1, self.writer_name)
+        self._startupServer(full_class_name, 1, hostname, 1, self.writer_name,
+                            postpone)
 
         return True
 
-    def createConfigServer(self, beamline, masterhost, jsonsettings=None):
+    def createServer(self, server_name, beamline, masterhost, hostname=None,
+                     class_name=None, jsondeviceproperties=None,
+                     postpone=False):
+        """ creates tango server in DB
+
+        :param server_name: server name
+        :type server_name: :obj:`str`
+        :param beamline: beamline name
+        :type beamline: :obj:`str`
+        :param masterhost: master host of data writer
+        :type masterhost: :obj:`str`
+        :param hostname: host to run the config server
+        :type hostname: :obj:`str`
+        :param class_name: class name
+        :type clas_name: :obj:`str`
+        :param jsondeviceproperties: json device properties
+        :type jsondeviceproperties: :obj:`str`
+        :param postpone: postpone starting flag
+        :type postpone: :obj:`bool`
+        :returns: True if server was created
+        :rtype: :obj:`bool`
+        """
+        if not beamline:
+            print("createServer: no beamline given ")
+            return False
+        if not masterhost:
+            print("createServer: no masterhost given ")
+            return False
+
+        if "/" not in server_name:
+            server_name = server_name + '/' + masterhost
+        server = server_name.split("/")[0]
+        if not class_name:
+            class_name = server
+        self.device_name = "%s/%s/%s" % (beamline, server.lower(), masterhost)
+        if server_name not in self.db.get_server_list(server_name):
+            print("creating: %s" % server_name)
+
+            if server_name in self.db.get_server_list(server_name):
+                print("createDataWriter: DB contains already %s" % server_name)
+                return False
+
+            try:
+                properties = dict(json.loads(jsondeviceproperties))
+            except Exception:
+                print("\ncreateServer: properties cannot be load")
+                properties = {}
+            if not properties:
+                properties = {self.__device_name: {}}
+
+            print("PROP", properties)
+            for dv, props in properties.items():
+                di = tango.DbDevInfo()
+                di.name = dv
+                di._class = class_name
+                di.server = server_name
+                self.db.add_device(di)
+                try:
+                    self.db.put_device_property(dv, props)
+                except Exception:
+                    print("\ncreateServer: properties cannot be added")
+
+        elif (self.device_name not in
+              self.db.get_device_class_list(server_name).value_string):
+            print("\ncreateServer: %s already exists. "
+                  "To change its device name please remove it." % server_name)
+            return False
+
+        if not hostname:
+            hostname = socket.gethostname()
+
+        self._startupServer(server_name, 1, hostname, 1, self.device_name,
+                            postpone)
+
+        return True
+
+    def createConfigServer(self, beamline, masterhost, jsonsettings=None,
+                           hostname=None, postpone=False):
         """ creates configuration server
 
         :param beamline: beamline name
         :type beamline: :obj:`str`
         :param masterhost: master host of data writer
         :type masterhost: :obj:`str`
         :param jsonsettings: connection settings to DB in json
         :type jsonsettings: :obj:`str`
+        :param hostname: host to run the config server
+        :type hostname: :obj:`str`
+        :param postpone: postpone starting flag
+        :type postpone: :obj:`bool`
         :returns: True if server was created
         :rtype: :obj:`bool`
         """
         if not beamline:
             print("createConfigServer: no beamline given ")
             return False
         if not masterhost:
@@ -805,75 +956,81 @@
             print("creating: %s" % server_name)
 
             if server_name in self.db.get_server_list(server_name):
                 print("createConfigServer: DB contains already %s"
                       % server_name)
                 return False
 
-            di = PyTango.DbDevInfo()
+            di = tango.DbDevInfo()
             di.name = self.cserver_name
             di._class = class_name
             di.server = server_name
 
             self.db.add_device(di)
             self.db.put_device_property(
                 self.cserver_name, {'VersionLabel': '%s@%s' % (
                     beamline.upper(), masterhost.upper())})
         elif (self.cserver_name not in
               self.db.get_device_class_list(server_name).value_string):
             print("\ncreateConfigServer: %s already exists. "
                   "To change its device name please remove it." % server_name)
             return False
 
-        hostname = self.db.get_db_host().split(".")[0]
+        if not hostname:
+            hostname = self.db.get_db_host().split(".")[0]
 
-        self._startupServer(server_name, 1, hostname, 1, self.cserver_name)
+        self._startupServer(server_name, 1, hostname, 1, self.cserver_name,
+                            postpone)
 
-        dp = PyTango.DeviceProxy(self.cserver_name)
-        if dp.state() != PyTango.DevState.ON:
-            dp.Close()
-        if jsonsettings:
-            dp = PyTango.DeviceProxy(self.cserver_name)
-            dp.JSONSettings = jsonsettings
-        try:
-            dp.Open()
-        except Exception:
+        if not postpone:
+            dp = tango.DeviceProxy(self.cserver_name)
+            if dp.state() != tango.DevState.ON:
+                dp.Close()
+            if jsonsettings:
+                dp = tango.DeviceProxy(self.cserver_name)
+                dp.JSONSettings = jsonsettings
             try:
-                jsettings = json.loads(jsonsettings)
-                jsettings['read_default_file'] = \
-                    '/var/lib/nxsconfigserver/.my.cnf'
-                dp.JSONSettings = str(json.dumps(jsettings))
                 dp.Open()
             except Exception:
                 try:
+                    jsettings = json.loads(jsonsettings)
                     jsettings['read_default_file'] = \
                         '/var/lib/nxsconfigserver/.my.cnf'
                     dp.JSONSettings = str(json.dumps(jsettings))
                     dp.Open()
                 except Exception:
-                    print("createConfigServer: "
-                          "%s cannot connect the"
-                          " database with JSONSettings: \n%s " % (
-                              self.cserver_name, jsonsettings))
-                    print("try to change the settings")
-                    return False
+                    try:
+                        jsettings['read_default_file'] = \
+                            '/var/lib/nxsconfigserver/.my.cnf'
+                        dp.JSONSettings = str(json.dumps(jsettings))
+                        dp.Open()
+                    except Exception:
+                        print("createConfigServer: "
+                              "%s cannot connect the"
+                              " database with JSONSettings: \n%s " % (
+                                  self.cserver_name, jsonsettings))
+                        print("try to change the settings")
+                        return False
 
         return True
 
-    def createSelector(self, beamline, masterhost, writer=None, cserver=None):
+    def createSelector(self, beamline, masterhost, writer=None, cserver=None,
+                       postpone=False):
         """ creates selector server
 
         :param beamline: beamline name
         :type beamline: :obj:`str`
         :param masterhost: master host of data writer
         :type masterhost: :obj:`str`
         :param writer: writer device name
         :type writer: :obj:`str`
         :param cserver: configuration server device name
         :type cserver: :obj:`str`
+        :param postpone: postpone starting flag
+        :type postpone: :obj:`bool`
         :returns: True if server was created
         :rtype: :obj:`bool`
         """
         if not beamline:
             print("createSelector: no beamline given ")
             return False
         if not masterhost:
@@ -892,38 +1049,40 @@
         if server_name not in self.db.get_server_list(server_name):
             print("creating: %s" % server_name)
 
             if server_name in self.db.get_server_list(server_name):
                 print("createSelector: DB contains already %s" % server_name)
                 return False
 
-            di = PyTango.DbDevInfo()
+            di = tango.DbDevInfo()
             di.name = device_name
             di._class = class_name
             di.server = server_name
             self.db.add_device(di)
 
         elif (device_name not in
               self.db.get_device_class_list(server_name).value_string):
             print("\ncreateSelector: %s already exists. "
                   "To change its device name please remove it." % server_name)
             return False
 
         hostname = socket.gethostname()
 
-        self._startupServer(full_class_name, 4, hostname, 1, device_name)
+        self._startupServer(full_class_name, 4, hostname, 1,
+                            device_name, postpone)
 
-        if self.writer_name or self.cserver_name:
-            dp = PyTango.DeviceProxy(device_name)
-            dp.ping()
-            self.waitServerRunning(None, device_name)
-            if self.cserver_name:
-                dp.configDevice = self.cserver_name
-            if self.writer_name:
-                dp.writerDevice = self.writer_name
+        if not postpone:
+            if self.writer_name or self.cserver_name:
+                dp = tango.DeviceProxy(device_name)
+                dp.ping()
+                self.waitServerRunning(None, device_name)
+                if self.cserver_name:
+                    dp.configDevice = self.cserver_name
+                if self.writer_name:
+                    dp.writerDevice = self.writer_name
         return True
 
 
 class Set(Runner):
 
     """ set runner"""
 
@@ -932,14 +1091,18 @@
                   + "and NXSRecSelector servers"
     #: (:obj:`str`) command epilog
     epilog = "" \
         + " examples:\n" \
         + "       nxsetup set\n" \
         + "       nxsetup set -b p09 -m haso228 -u p09user " \
         + "-d nxsconfig NXSConfigServer\n" \
+        + "       nxsetup set NexusWriter/haso228  -k NexusWriter  " \
+        + "-y '{\"p00/bliss_nexuswriter/test_session\":" \
+        + "{\"session\":\"test_session\"," \
+        + "\"beacon_host\":\"haso228:25000\"}}'  -t\n" \
         + "\n"
 
     def create(self):
         """ creates parser
         """
         parser = self._parser
         parser.add_argument(
@@ -947,14 +1110,22 @@
             dest="beamline", help="name of the beamline"
             " ( default: 'nxs' )")
         parser.add_argument(
             "-m", "--masterhost", action="store",
             dest="masterhost", help="the host that stores the Mg"
             " ( default: <localhost> )")
         parser.add_argument(
+            "-c", "--confighost", action="store",
+            dest="confighost", help="the host run the config server"
+            " ( default: <mysqlhost> )")
+        parser.add_argument(
+            "-r", "--runhost", action="store",
+            dest="runhost", help="the host to run the server"
+            " ( default: localhost )")
+        parser.add_argument(
             "-u", "--user", action="store",
             dest="user", help="the local user"
             " ( default: 'tango' )")
         parser.add_argument(
             "-d", "--database", action="store",
             dest="dbname", help="the database name"
             "  ( default: 'nxsconfig')")
@@ -965,14 +1136,26 @@
             "( default: '{\"host\": \"localhost\",\"db\": <DBNAME>,"
             " \"use_unicode\": true,"
             " \"read_default_file\": <MY_CNF_FILE>}'"
             "  where <MY_CNF_FILE> stays for"
             " \"/home/<USER>/.my.cnf\""
             " or \"/var/lib/nxsconfigserver/.my.cnf\" )")
         parser.add_argument(
+            "-k", "--class-name", action="store",
+            dest="classname", help="tango server class name")
+        parser.add_argument(
+            "-y", "--json-device-properties", action="store",
+            dest="propjson",
+            help="JSON tango device properties "
+            "( default: '{}' )")
+        parser.add_argument(
+            "-t", "--postpone", action="store_true",
+            default=False, dest="postpone",
+            help="do not start the server")
+        parser.add_argument(
             'args', metavar='server_name',
             type=str, nargs='*',
             help='server names, e.g.: NXSRecSelector NXSConfigServer')
 
     def run(self, options):
         """ the main program function
 
@@ -1026,32 +1209,53 @@
                     masterhost=options.masterhost):
                 print("startup failed to create the nexus data writer")
                 sys.exit(255)
 
         if options.csjson:
             jsonsettings = options.csjson
         else:
-            jsonsettings = '{"host":"localhost","db":"%s",' % options.dbname \
+            jsonsettings = '{"db":"%s",' % options.dbname \
                 + ' "read_default_file":"/home/%s/.my.cnf",' % options.user \
                 + ' "use_unicode":true}'
 
+        if options.propjson:
+            jsondeviceproperties = options.propjson
+        else:
+            jsondeviceproperties = '{}'
+
         if not args or "NXSConfigServer" in args:
             if not setUp.createConfigServer(
                     beamline=options.beamline,
                     masterhost=options.masterhost,
-                    jsonsettings=jsonsettings):
+                    jsonsettings=jsonsettings,
+                    hostname=options.confighost,
+                    postpone=options.postpone):
                 print("startup failed to create the nexus config server")
                 sys.exit(255)
 
         if not args or "NXSRecSelector" in args:
             if not setUp.createSelector(
                     beamline=options.beamline,
-                    masterhost=options.masterhost):
+                    masterhost=options.masterhost,
+                    postpone=options.postpone):
                 print("startup failed to create the nexus selector server")
                 sys.exit(255)
+        for arg in args:
+            if arg not in ["NXSDataWriter", "NXSRecSelector",
+                           "NXSConfigServer"]:
+                if not setUp.createServer(
+                        arg,
+                        beamline=options.beamline,
+                        masterhost=options.masterhost,
+                        hostname=options.runhost,
+                        class_name=options.classname,
+                        jsondeviceproperties=jsondeviceproperties,
+                        postpone=options.postpone):
+                    print("startup failed to create the %s server" % arg)
+                    sys.exit(255)
 
 
 class Start(Runner):
 
     """ start runner"""
 
     #: (:obj:`str`) command description
@@ -1066,14 +1270,21 @@
         """ creates parser
         """
         parser = self._parser
         parser.add_argument(
             "-l", "--level", action="store", type=int, default=-1,
             dest="level", help="startup level")
         parser.add_argument(
+            "-z", "--timeout", action="store", type=float, default=None,
+            dest="timeout", help="timeout in seconds")
+        parser.add_argument(
+            "-e", "--no-wait", action="store_true",
+            default=False, dest="nowait",
+            help="do not wait")
+        parser.add_argument(
             'args', metavar='server_name',
             type=str, nargs='*',
             help='server names, e.g.: NXSRecSelector NXSDataWriter/TDW1')
 
     def run(self, options):
         """ the main program function
 
@@ -1084,15 +1295,56 @@
         setUp = SetUp()
         servers = args if args else [
             "NXSConfigServer", "NXSRecSelector", "NXSDataWriter"]
         for server in servers:
             setUp.restartServer(
                 server,
                 level=(options.level if options.level > -1 else None),
-                restart=False)
+                restart=False, timeout=options.timeout,
+                wait=(not options.nowait))
+
+
+class Wait(Runner):
+
+    """ start runner"""
+
+    #: (:obj:`str`) command description
+    description = "wait for tango server"
+    #: (:obj:`str`) command epilog
+    epilog = "" \
+        + " examples:\n" \
+        + "       nxsetup wait Pool/haso228 -z 30\n" \
+        + "\n"
+
+    def create(self):
+        """ creates parser
+        """
+        parser = self._parser
+        parser.add_argument(
+            "-z", "--timeout", action="store", type=float, default=None,
+            dest="timeout", help="timeout in seconds")
+        parser.add_argument(
+            'args', metavar='server_name',
+            type=str, nargs='*',
+            help='server names, e.g.: NXSRecSelector NXSDataWriter/TDW1')
+
+    def run(self, options):
+        """ the main program function
+
+        :param options: parser options
+        :type options: :class:`argparse.Namespace`
+        """
+        args = options.args or []
+        setUp = SetUp()
+        servers = args if args else [
+            "NXSConfigServer", "NXSRecSelector", "NXSDataWriter"]
+        for server in servers:
+            setUp.restartServer(
+                server,
+                restart=False, stopstart=False, timeout=options.timeout)
 
 
 class MoveProp(Runner):
 
     """ move-prop runner"""
 
     #: (:obj:`str`) command description
@@ -1117,14 +1369,21 @@
             "-o", "--oldname", action="store",
             dest="oldname", help="old property name")
         parser.add_argument(
             "-t", "--postpone", action="store_true",
             default=False, dest="postpone",
             help="do not restart the server")
         parser.add_argument(
+            "-z", "--timeout", action="store", type=float, default=None,
+            dest="timeout", help="timeout in seconds")
+        parser.add_argument(
+            "-e", "--no-wait", action="store_true",
+            default=False, dest="nowait",
+            help="do not wait")
+        parser.add_argument(
             'args', metavar='server_name',
             type=str, nargs='*',
             help='server names, e.g.: NXSRecSelector NXSDataWriter/TDW1')
 
     def run(self, options):
         """ the main program function
 
@@ -1138,15 +1397,17 @@
             sys.exit(255)
         servers = args or []
         setUp = SetUp()
         for server in servers:
             if setUp.changePropertyName(
                     server, options.oldname, options.newname):
                 if not options.postpone:
-                    setUp.restartServer(server)
+                    setUp.restartServer(
+                        server, timeout=options.timeout,
+                        wait=(not options.nowait))
 
 
 class ChangeProp(Runner):
 
     """ change-prop runner"""
 
     #: (:obj:`str`) command description
@@ -1174,14 +1435,21 @@
             "-w", "--propvalue", action="store",
             dest="propvalue", help="new property value")
         parser.add_argument(
             "-t", "--postpone", action="store_true",
             default=False, dest="postpone",
             help="do not restart the server")
         parser.add_argument(
+            "-z", "--timeout", action="store", type=float, default=None,
+            dest="timeout", help="timeout in seconds")
+        parser.add_argument(
+            "-e", "--no-wait", action="store_true",
+            default=False, dest="nowait",
+            help="do not wait")
+        parser.add_argument(
             'args', metavar='server_name',
             type=str, nargs='*',
             help='server names, e.g.: NXSRecSelector NXSDataWriter/TDW1')
 
     def run(self, options):
         """ the main program function
 
@@ -1195,15 +1463,17 @@
             sys.exit(255)
         servers = args or []
         setUp = SetUp()
         for server in servers:
             if setUp.changePropertyValue(
                     server, options.newname, options.propvalue):
                 if not options.postpone:
-                    setUp.restartServer(server)
+                    setUp.restartServer(
+                        server,
+                        timeout=options.timeout, wait=(not options.nowait))
 
 
 class AddRecorderPath(Runner):
 
     """ add-recorder-path runner"""
 
     #: (:obj:`str`) command description
@@ -1224,18 +1494,25 @@
         """
         parser = self._parser
         parser.add_argument(
             "-t", "--postpone", action="store_true",
             default=False, dest="postpone",
             help="do not restart the server")
         parser.add_argument(
+            "-z", "--timeout", action="store", type=float, default=None,
+            dest="timeout", help="timeout in seconds")
+        parser.add_argument(
+            "-e", "--no-wait", action="store_true",
+            default=False, dest="nowait",
+            help="do not wait")
+        parser.add_argument(
             "-i", "--instance", action="store",
             dest="instance",
             help="macroserver instance name, i.e. haso"
-            " ( default: '*'")
+            " ( default: '*')")
 
     def postauto(self):
         """ creates parser
         """
         parser = self._parser
         parser.add_argument(
             'recpath', metavar='recorder_path',
@@ -1255,15 +1532,16 @@
         if setUp.changeRecorderPath(
                 options.recpath[0], options.instance):
             if not options.postpone:
                 if options.instance != "*":
                     ms = "MacroServer/%s" % options.instance
                 else:
                     ms = "MacroServer"
-                setUp.restartServer(ms)
+                setUp.restartServer(ms, timeout=options.timeout,
+                                    wait=(not options.nowait))
 
 
 class Restart(Runner):
 
     """ restart runner"""
 
     #: (:obj:`str`) command description
@@ -1278,14 +1556,21 @@
         """ creates parser
         """
         parser = self._parser
         parser.add_argument(
             "-l", "--level", action="store", type=int, default=-1,
             dest="level", help="startup level")
         parser.add_argument(
+            "-z", "--timeout", action="store", type=float, default=None,
+            dest="timeout", help="timeout in seconds")
+        parser.add_argument(
+            "-e", "--no-wait", action="store_true",
+            default=False, dest="nowait",
+            help="do not wait")
+        parser.add_argument(
             'args', metavar='server_name',
             type=str, nargs='*',
             help='server names, e.g.: NXSRecSelector NXSDataWriter/TDW1')
 
     def run(self, options):
         """ the main program function
 
@@ -1294,15 +1579,16 @@
         """
         args = options.args or []
         setUp = SetUp()
         servers = args if args else [
             "NXSConfigServer", "NXSRecSelector", "NXSDataWriter"]
         for server in servers:
             setUp.restartServer(
-                server, level=(options.level if options.level > -1 else None))
+                server, level=(options.level if options.level > -1 else None),
+                timeout=options.timeout, wait=(not options.nowait))
 
 
 class Stop(Runner):
 
     """ Stop runner"""
 
     #: (:obj:`str`) command description
@@ -1387,14 +1673,15 @@
         description=description, epilog=epilog,
         formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.cmdrunners = [
         ('set', Set),
         ('restart', Restart),
         ('start', Start),
         ('stop', Stop),
+        ('wait', Wait),
         ('move-prop', MoveProp),
         ('change-prop', ChangeProp),
         ('add-recorder-path', AddRecorderPath),
     ]
     runners = parser.createSubParsers()
 
     try:
```

### Comparing `nxstools-3.9.0/nxstools/nxsparser.py` & `nxstools-4.0.0/nxstools/nxsparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -64,18 +63,21 @@
     """ provides xml content of the whole node
 
     :param node: DOM node
     :type node: :class:`xml.dom.Node`
     :returns: xml content string
     :rtype: :obj:`str`
     """
-    xml = _tostr(et.tostring(node, encoding='utf8', method='xml'))
+    if sys.version_info > (3,):
+        xml = _tostr(et.tostring(node, encoding='unicode', method='xml'))
+    else:
+        xml = _tostr(et.tostring(node, encoding='utf8', method='xml'))
     if xml.startswith("<?xml version='1.0' encoding='utf8'?>"):
         xml = str(xml[38:])
-        return xml
+    return xml
 
 
 class ESRFConverter(object):
     """ ESRF xml configuration converter """
 
     def __init__(self):
         """ constructor """
@@ -179,14 +181,15 @@
 
         :param node: datasource node
         :type node: :class:`lxml.etree.Element`
         :returns: record name or query
         :rtype: :obj:`str`
         """
         withRec = ["CLIENT", "TANGO"]
+        withResult = ["PYEVAL"]
         withQuery = ["DB"]
         if node.tag == 'datasource':
             dsource = node
         else:
             dsource = node.find(".//datasource")
         dstype = dsource.attrib["type"]
         res = ''
@@ -222,16 +225,28 @@
                         else:
                             res = '%s/%s%s%s' % (dname, prefix, rname, surfix)
                     else:
                         res = rname
                 return res
         elif dstype and dstype in withQuery:
             query = dsource.find(".//query")
-            if len(query) and query.strip():
-                return query.strip() or ""
+            if len(query.text) and query.text.strip():
+                return query.text.strip() or ""
+        elif dstype and dstype in withResult:
+            result = dsource.findall("result")
+            cresult = dsource.find(".//result")
+            if result is not None and len(result) > 0:
+                rname = result[0].get("name", "result")
+                tres = "ds.%s = " % rname
+                if len(cresult.text) and cresult.text.strip():
+                    teres = cresult.text.strip() or ""
+                    lres = teres.split("\n")
+                    for re in lres:
+                        if re.strip().startswith(tres):
+                            res = re.strip()[len(tres):]
         return res
 
     @classmethod
     def mergeDefinitions(cls, xmls):
         """ merges the xmls list of definitions xml strings
             to one output xml string
```

### Comparing `nxstools-3.9.0/nxstools/nxsxml.py` & `nxstools-4.0.0/nxstools/nxsxml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #   This file is part of nexdatas - Tango Server for NeXus data writer
 #
 #    Copyright (C) 2012-2018 DESY, Jan Kotanski <jkotan@mail.desy.de>
 #
 #    nexdatas is free software: you can redistribute it and/or modify
 #    it under the terms of the GNU General Public License as published by
 #    the Free Software Foundation, either version 3 of the License, or
@@ -16,15 +15,18 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """  Creator of XML configuration files """
 
 
-import PyTango
+try:
+    import tango
+except Exception:
+    import PyTango as tango
 import sys
 
 import lxml.etree
 
 
 if sys.version_info > (3,):
     unicode = str
@@ -598,16 +600,16 @@
         :type typeAttr: :obj:`str`
         :param commands: if we call the commands
         :type commands: :obj:`bool`
         :param blackAttrs: list of excluded attributes
         :type blackAttrs: :obj:`list` <:obj:`str`>
         """
         NGroup.__init__(self, parent, nameAttr, typeAttr)
-        #: (:class:`PyTango.DeviceProxy`) device proxy
-        self._proxy = PyTango.DeviceProxy(deviceName)
+        #: (:class:`tango.DeviceProxy`) device proxy
+        self._proxy = tango.DeviceProxy(deviceName)
         #: (:obj:`dict` <:obj:`str`, :class:`NTag`>) fields of the device
         self._fields = {}
         #: (:obj:`list` <:obj:`str`>) blacklist for Attributes
         self._blackAttrs = blackAttrs if blackAttrs else []
         #: (:obj:`str`) the device name
         self._deviceName = deviceName
 
@@ -732,22 +734,50 @@
     def prettyPrint(self, etNode=None):
         """prints pretty XML making use of etree
 
         :param etNode: node
         :type etNode: :class:`lxml.etree.Element`
         """
         node = etNode if etNode is not None else self.elem
-        xmls = _tostr(
-            lxml.etree.tostring(
-                node, encoding='utf8',
-                method='xml', pretty_print=True))
+        if sys.version_info > (3,):
+            xmls = _tostr(
+                lxml.etree.tostring(
+                    node, encoding='unicode',
+                    method='xml', pretty_print=True))
+        else:
+            xmls = _tostr(
+                lxml.etree.tostring(
+                    node, encoding='utf8',
+                    method='xml', pretty_print=True))
         if not xmls.startswith("<?xml"):
             xmls = "<?xml version='1.0' encoding='utf8'?>\n" + xmls
         return xmls
 
+    def setDependencies(self, components, entry=None):
+        """ sets tag content
+
+        :param components: component dependencies
+        :type components: :obj:`list` <:obj:`str`>
+        :param entry: entry node
+        :type entry: :class:`lxml.etree.Element`
+        """
+        text = "\n"
+        for cp in components:
+            text += "$components.%s\n" % cp
+        if entry is not None:
+            if entry.elem.tail is not None:
+                entry.elem.tail += text
+            else:
+                entry.elem.tail = text
+        else:
+            if self.elem.text:
+                self.elem.text += text
+            else:
+                self.elem.text = text
+
     def dump(self):
         """ dumps XML structure into the XML file
 
         :brief: It opens XML file, calls prettyPrint and closes the XML file
         """
         with open(self.fname, "w") as myfile:
             myfile.write(self.prettyPrint(self.elem))
```

### Comparing `nxstools-3.9.0/nxstools/pyeval/__init__.py` & `nxstools-4.0.0/nxstools/pyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/absorber.py` & `nxstools-4.0.0/nxstools/pyeval/absorber.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/beamtimeid.py` & `nxstools-4.0.0/nxstools/pyeval/beamtimeid.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """  pyeval helper functions for beamtimeid """
 
 import os
 import socket
 
 
 def beamtimeid(commonblock, starttime, shortname, compath, curpath, locpath,
-               curprefix, curext, comprefix, comext):
+               curprefix, curext, comprefix, comext, strip=True):
     """ code for beamtimeid  datasource
 
     :param commonblock: commonblock of nxswriter
     :type commonblock: :obj:`dict`<:obj:`str`, `any`>
     :param starttime:  start time
     :type starttime: :obj:`str`
     :param shortname:  short name of beamline
@@ -61,25 +61,31 @@
     if fpath.startswith(curpath):
         try:
             if os.path.isdir(curpath):
                 btml = [fl for fl in os.listdir(curpath)
                         if (fl.startswith(curprefix)
                             and fl.endswith(curext))]
             if btml:
-                result = btml[0][len(curprefix):-len(curext)]
+                if strip:
+                    result = btml[0][len(curprefix):-len(curext)]
+                else:
+                    result = os.path.join(os.path.abspath(curpath), btml[0])
         except Exception:
             pass
     if not result and fpath.startswith(compath):
         try:
             if os.path.isdir(compath):
                 btml = [fl for fl in os.listdir(compath)
                         if (fl.startswith(comprefix)
                             and fl.endswith(comext))]
             if btml:
-                result = btml[0][len(comprefix):-len(comext)]
+                if strip:
+                    result = btml[0][len(comprefix):-len(comext)]
+                else:
+                    result = os.path.join(os.path.abspath(compath), btml[0])
         except Exception:
             pass
     if not result:
         try:
             dirpath = os.path.dirname(fpath)
             while dirpath.startswith(locpath):
                 if os.path.isdir(dirpath):
@@ -90,15 +96,55 @@
                         result = btml[0][len(curprefix):-len(curext)]
                         break
                     else:
                         btml = [fl for fl in os.listdir(dirpath)
                                 if (fl.startswith(comprefix)
                                     and fl.endswith(comext))]
                         if btml:
-                            result = btml[0][len(comprefix):-len(comext)]
+                            if strip:
+                                result = btml[0][len(comprefix):-len(comext)]
+                            else:
+                                result = os.path.join(
+                                    os.path.abspath(locpath), btml[0])
                             break
                 dirpath, tail = os.path.split(dirpath)
         except Exception:
             pass
     if not result:
-        result = "%s_%s@%s" % (shortname, starttime, socket.gethostname())
+        if strip:
+            result = "%s_%s@%s" % (shortname, starttime, socket.gethostname())
+        else:
+            result = ""
     return result
+
+
+def beamtime_filename(commonblock, starttime, shortname,
+                      compath, curpath, locpath,
+                      curprefix, curext, comprefix, comext):
+    """ code for beamtimeid  datasource
+
+    :param commonblock: commonblock of nxswriter
+    :type commonblock: :obj:`dict`<:obj:`str`, `any`>
+    :param starttime:  start time
+    :type starttime: :obj:`str`
+    :param shortname:  short name of beamline
+    :type shortname: :obj:`str`
+    :param compath:  commission directory
+    :type compath: :obj:`str`
+    :param curpath:  current directory
+    :type curpath: :obj:`str`
+    :param locpath:  local directory
+    :type locpath: :obj:`str`
+    :param curprefix:  current prefix
+    :type curprefix: :obj:`str`
+    :param curext:  current postfix
+    :type curext: :obj:`str`
+    :param comprefix:  commission prefix
+    :type comprefix: :obj:`str`
+    :param comext:  commission postfix
+    :type comext: :obj:`str`
+    :returns:   beamtime id
+    :rtype: :obj:`str`
+    """
+    return beamtimeid(commonblock,
+                      starttime, shortname, compath, curpath, locpath,
+                      curprefix, curext, comprefix, comext, strip=False)
```

### Comparing `nxstools-3.9.0/nxstools/pyeval/common.py` & `nxstools-4.0.0/nxstools/pyeval/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -98,7 +98,30 @@
     :rtype: :obj:`str`
     """
     if name not in commonblock:
         commonblock[name] = [int(value)]
     else:
         commonblock[name].append(int(value))
     return value
+
+
+def blockitem_addint_safe(commonblock, name, value):
+    """ add block item to commonblock with default 0
+
+    :param commonblock: commonblock of nxswriter
+    :type commonblock: :obj:`dict`<:obj:`str`, `any`>
+    :param name: name of block item
+    :type name: :obj:`str`
+    :param value:  item value
+    :type value: :obj:`str`
+    :returns:   item value
+    :rtype: :obj:`str`
+    """
+    try:
+        value = int(value)
+    except Exception:
+        value = 0
+    if name not in commonblock:
+        commonblock[name] = [value]
+    else:
+        commonblock[name].append(value)
+    return value
```

### Comparing `nxstools-3.9.0/nxstools/pyeval/dalsa.py` & `nxstools-4.0.0/nxstools/pyeval/dalsa.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/dcm.py` & `nxstools-4.0.0/nxstools/pyeval/dcm.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/eigerdectris.py` & `nxstools-4.0.0/nxstools/pyeval/eigerdectris.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             spf = root.stepsperfile
             cfid = root.currentfileid
         if root.h5object.__class__.__name__ == "File":
             import nxstools.h5pywriter as nxw
         else:
             import nxstools.h5cppwriter as nxw
     else:
-        raise("Writer cannot be found")
+        raise Exception("Writer cannot be found")
     en = root.open(entryname)
     dt = en.open("data")
     ins = en.open(insname)
     det = ins.open(name)
     col = det.open("collection")
     for nbf in range(1, nbfiles+1):
         if spf > 0 and cfid > 0:
```

### Comparing `nxstools-3.9.0/nxstools/pyeval/lambdavds.py` & `nxstools-4.0.0/nxstools/pyeval/dalsavds.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,164 +13,186 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-"""  pyeval helper functions for lambdavds """
+"""  pyeval helper functions for dalsa """
 
-try:
-    from . import common
-except Exception:
-    import common
 
-
-def savefilename_cb(commonblock, savefilename, savefilename_str):
-    """ code for savefilename_cb  datasource
-
-    :param commonblock: commonblock of nxswriter
-    :type commonblock: :obj:`dict`<:obj:`str`, `any`>
-    :param savefilename:  name of saved file
-    :type savefilename: :obj:`str`
-    :param savefilename_str: name of savefilename datasource
-    :type savefilename_str: :obj:`str`
-    :returns:   name of saved file
-    :rtype: :obj:`str`
-    """
-    return common.blockitem_add(
-        commonblock, savefilename_str, savefilename)
-
-
-def framenumbers_cb(commonblock, framenumbers, framenumbers_str):
-    """ code for triggermode_cb  datasource
-
-    :param commonblock: commonblock of nxswriter
-    :type commonblock: :obj:`dict`<:obj:`str`, `any`>
-    :param framenumbers:  number of frames
-    :type framenumbers: :obj:`str` or :obj:`int`
-    :param framenumbers_str: name of framenumbers datasource
-    :type framenumbers_str: :obj:`str`
-    :returns:  number of frames
-    :rtype: :obj:`str` or :obj:`int`
-    """
-    return common.blockitem_addint(
-        commonblock, framenumbers_str, framenumbers)
-
-
-def triggermode_cb(commonblock, name, triggermode, saveallimages,
-                   framesperfile, height, width, opmode,
-                   filepostfix, savefilename_str, framenumbers_str,
-                   filename_str, entry_str):
-    """ code for triggermode_cb  datasource
+def triggermode(commonblock, name,
+                filedir, fileprefix, filepostfix, filestartnum, filesaving,
+                triggermode, framespernxfile, pixelformat, height, width,
+                acquisitionmode, acquisitionframecount,
+                filestartnum_str, nrexposedframes_str,
+                filename, entryname, insname):
+    """ code for external_data datasource
 
     :param commonblock: commonblock of nxswriter
     :type commonblock: :obj:`dict`<:obj:`str`, `any`>
-    :param name: component name
+    :param name: detector name
     :type name: :obj:`str`
-    :param triggermode:  trigger mode
-    :type triggermode: :obj:`int` or :obj:`str`
-    :param saveallimages: save all images flag
-    :type saveallimages: :obj:`int` or :obj:`bool`
-    :param height: height of the image
+    :param filedir: file directory
+    :type filedir: :obj:`str`
+    :param fileprefix: file prefix
+    :type fileprefix: :obj:`str`
+    :param filepostfix: file postfix
+    :type filepostfix: :obj:`str`
+    :param filestartnum: file start number
+    :type filestartnum: :obj:`int`
+    :param filesaving: file saving flag
+    :type filesaving: :obj:`int` or :obj:`bool`
+    :param triggermode: trigger mode
+    :type triggermode: :obj:`str`
+    :param framespernxfile: frames per nexus file
+    :type framespernxfile: :obj:`int`
+    :param pixelformat: pixel format
+    :type pixelformat: :obj:`str`
+    :param height: image height
     :type height: :obj:`int`
-    :param framesperfile: a number of frames per fiel
-    :type framesperfile: :obj:`int`
-    :param height: height of the image
-    :type height: :obj:`int`
-    :param width: width of the image
+    :param width: image width
     :type width: :obj:`int`
-    :param opmode: operation mode,
-                   i.e. 1="int8", 6="int8", 12="int16", 24="int32"
-    :type opmode:  :obj:`int`
-    :param filepostfix: filename postfix
-    :type filepostfix:  :obj:`str`
-    :param savefilename_str: name of savefilename datasource
-    :type savefilename_str: :obj:`str`
-    :param framenumbers_str: name of framenumbers datasource
-    :type framenumbers_str: :obj:`str`
-    :param filename_str: file name
-    :type filename_str: :obj:`str`
-    :param entry_str: entry name
-    :type entry_str: :obj:`str`
-    :returns:  triggermode
-    :rtype: :obj:`str` or :obj:`int`
+    :param acquisitionmode: acquisition mode
+    :type acquisitionmode: :obj:`str`
+    :param acquisitionframecount: acquisition frame count
+    :type acquisitionframecount: :obj:`str`
+    :param filestartnum_str: filestartnum name string
+    :type filestartnum_str: :obj:`str`
+    :param nrexposedframes_str: nrexposedframes name string
+    :type nrexposedframes_str: :obj:`str`
+    :param filename: file name
+    :type filename: :obj:`str`
+    :param entryname: entry name
+    :type entryname: :obj:`str`
+    :param insname: instrument name
+    :type insname: :obj:`str`
+    :returns: trigger mode
+    :rtype: :obj:`str`
     """
+    result = triggermode
 
-    if saveallimages:
-
+    if filesaving:
         if "__root__" in commonblock.keys():
             root = commonblock["__root__"]
-        filenames = []
-        framesnumbers = []
-        if savefilename_str in commonblock:
-            filenames = commonblock[savefilename_str]
-        if framenumbers_str in commonblock:
-            framesnumbers = commonblock[framenumbers_str]
-        fln = min(len(framesnumbers), len(filenames))
+        # filenames = []
+        filestartnumbers = []
+        if filestartnum_str in commonblock:
+            filestartnumbers = commonblock[filestartnum_str]
+        if nrexposedframes_str in commonblock:
+            nrexposedframes = commonblock[nrexposedframes_str]
+        flen = len(filestartnumbers)
+        frlen = nrexposedframes[-1] if nrexposedframes else 0
+
+        lastfilenumber = filestartnumbers[-1] if filestartnumbers else 0
 
-        filesframes = []
-        lastfile = None
         totalframenumbers = 0
-        for fi in range(fln):
-            if lastfile != filenames[fi]:
-                filesframes.append((filenames[fi], framesnumbers[fi]))
-                lastfile = filenames[fi]
-                totalframenumbers += framesnumbers[fi]
-        dtm = {1: "int8", 6: "int8", 12: "int16", 24: "int32"}
+
+        mode = acquisitionmode
+        framecount = acquisitionframecount
+        filesizes = []
+        totalframenumbers = []
+        nbfiles = 0
+        if mode in ["MultiFrame"]:
+            totalframenumbers = flen * framecount
+            if 1 > framespernxfile or framespernxfile > framecount:
+                filesizes = [framecount] * (flen)
+                nbfiles = len(filesizes)
+                lastfilenbframes = framecount
+            else:
+                fsizes = []
+                filesizes = []
+                nbfiles = 0
+                nfiles = (framecount + 1) // framespernxfile + 1
+                lastfilenbframes = framecount % framespernxfile
+                print(nfiles)
+                if nfiles:
+                    fsizes = [framespernxfile] * (nfiles - 1)
+                if lastfilenbframes:
+                    fsizes.append(lastfilenbframes)
+                for i in range(nfiles):
+                    filesizes = filesizes + fsizes
+                nbfiles = nfiles * len(fsizes)
+
+        elif mode in ["SingleFrame"]:
+            totalframenumbers = flen
+            filesizes = [1 for _ in range(flen)]
+            nbfiles = len(filesizes)
+            lastfilenbframes = nbfiles
+        elif mode in ["Continuous"]:
+            totalframenumbers = frlen
+            if 1 > framespernxfile or framespernxfile > frlen:
+                filesizes = [frlen]
+                nbfiles = len(filesizes)
+                lastfilenbframes = frlen
+            else:
+                nbfiles = (frlen + 1) // framespernxfile + 1
+                lastfilenbframes = frlen % framespernxfile
+                filesizes = []
+                if nbfiles:
+                    filesizes = [framespernxfile] * (nbfiles - 1)
+                if lastfilenbframes:
+                    filesizes.append(lastfilenbframes)
+
+        dtm = {
+            "Mono8": "uint8",
+            "Mono8Signed": "int8",
+            "Mono10": "uint16",
+            "Mono12": "uint16",
+            "Mono10Packed": "uint16",
+            "Mono12Packed": "uint16",
+            "Mono14": "uint16",
+            "Mono16": "uint16",
+            "Mono16Signed": "int16",
+            "BayerGR10": "uint16",
+            "BayerRG10": "uint16",
+            "BayerGB10": "uint16",
+            "BayerBG10": "uint16",
+            "BayerGR12": "uint16",
+            "BayerRG12": "uint16",
+            "BayerGB12": "uint16",
+            "BayerBG12": "uint16",
+        }
+
         try:
-            dtype = dtm[opmode]
+            dtype = dtm[pixelformat]
         except Exception:
-            dtype = "int32"
+            dtype = "uint8"
 
-        if filename_str:
-            path = (filename_str).split("/")[-1].split(".")[0] + "/"
+        if filename:
+            path = filename.split("/")[-1].split(".")[0] + "/"
         else:
             path = ""
 
         if "__root__" in commonblock.keys():
             root = commonblock["__root__"]
             if root.h5object.__class__.__name__ == "File":
                 import nxstools.h5pywriter as nxw
             else:
                 import nxstools.h5cppwriter as nxw
         else:
-            raise("Writer cannot be found")
+            raise Exception("Writer cannot be found")
 
-        en = root.open(entry_str)
-        ins = en.open("instrument")
+        en = root.open(entryname)
+        ins = en.open(insname)
         det = ins.open(name)
         npath = "/entry/instrument/detector/data"
 
         vfl = nxw.virtual_field_layout(
             [totalframenumbers, height, width], dtype)
-
-        foffset = 0
-        for savefilename, framenumbers in filesframes:
-            if framenumbers > 0 and framesperfile > 10:
-                nbfiles = (framenumbers - 1) // framesperfile + 1
-                lastfilenbframes = framenumbers - (nbfiles - 1) * framesperfile
-            elif framenumbers > 0:
-                nbfiles = 1
-                lastfilenbframes = framenumbers
-            else:
-                nbfiles = 0
-                lastfilenbframes = 0
-
-            if nbfiles > 0:
-                for nbf in range(0, nbfiles):
-                    if framenumbers > framesperfile and framesperfile > 10:
-                        connector = "_part%05d." % nbf
-                    else:
-                        connector = "."
-                    filename = path + name + "/" + str(savefilename) \
-                        + connector + str(filepostfix)
-                    ln = framesperfile if nbf + 1 != nbfiles \
-                        else lastfilenbframes
-                    ef = nxw.target_field_view(
-                        filename, npath, [ln, height, width], dtype)
-                    vfl[
-                        (foffset + nbf * framesperfile):
-                        (foffset + nbf * framesperfile + ln), :, :] = ef
-                foffset += framenumbers
+        firstfilenumber = lastfilenumber - nbfiles
+        if nbfiles > 0:
+            i1 = 0
+            i2 = 0
+            for nbf in range(firstfilenumber, lastfilenumber):
+                ln = filesizes[nbf - firstfilenumber]
+                i1 = i2
+                i2 = i2 + ln
+                connector = "_%05d." % nbf
+                filename = path + name + "/" + str(fileprefix) + connector + \
+                    str(filepostfix)
+                ef = nxw.target_field_view(
+                    filename, npath, [ln, height, width], dtype)
+                vfl[i1: i2, :, :] = ef
         det.create_virtual_field("data", vfl)
-    return triggermode
+
+    return result
```

### Comparing `nxstools-3.9.0/nxstools/pyeval/limaccd.py` & `nxstools-4.0.0/nxstools/pyeval/limaccd.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/lmbd.py` & `nxstools-4.0.0/nxstools/pyeval/lmbd.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/marccd.py` & `nxstools-4.0.0/nxstools/pyeval/marccd.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/mssar.py` & `nxstools-4.0.0/nxstools/pyeval/mssar.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/mythen.py` & `nxstools-4.0.0/nxstools/pyeval/mythen.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/pco.py` & `nxstools-4.0.0/nxstools/pyeval/pco.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/pe.py` & `nxstools-4.0.0/nxstools/pyeval/pe.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/pilatus.py` & `nxstools-4.0.0/nxstools/pyeval/pilatus.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/qbpm.py` & `nxstools-4.0.0/nxstools/pyeval/qbpm.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/pyeval/tangovimba.py` & `nxstools-4.0.0/nxstools/pyeval/tangovimba.py`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/release.py` & `nxstools-4.0.0/test/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,13 +11,12 @@
 #    nexdatas is distributed in the hope that it will be useful,
 #    but WITHOUT ANY WARRANTY; without even the implied warranty of
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
-#
-
-"""  NXS tools release version"""
+# \package mcs nexdatas
+# \file __init__.py
+# package constructor
 
-#: (:obj:`str`) package version
-__version__ = "3.9.0"
+""" Tests for Implementation of  NexDaTaS Tools"""
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/__init__.py` & `nxstools-4.0.0/nxstools/xmltemplates/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,24 +112,119 @@
             'doc': "pixel enable status for maia (datasource)"
         },
         'throttleenable': {
             'default': None,
             'doc': "throttle enable status for maia (datasource)"
         },
     },
+    'secop': {
+        'host': {
+            'default': None,
+            'doc': "secop host name (string)"
+        },
+        'port': {
+            'default': '5000',
+            'doc': "secop port name (string)"
+        },
+        'message': {
+            'default': None,
+            'doc': "secop command MANDATORY (string)"
+        },
+        'timeout': {
+            'default': '0.0001',
+            'doc': "secop timeout (string)"
+        },
+    },
+    'secoplinks': {
+        'meanings': {
+            'default': "temperature,magnetic_field,electric_field,"
+            "stress_field,pressure",
+            'doc': "secop meanings link lists MANDATORY (string)"
+        },
+        'environments': {
+            'default': "temperature,magnetic_field",
+            'doc': "secop environment link lists MANDATORY (string)"
+        },
+        'samplename': {
+            'default': 'sample',
+            'doc': "sample group name (string)"
+        },
+        'sampleenvname': {
+            'default': 'sample_environment',
+            'doc': "sample environment group name (string)"
+        },
+    },
+    'groupsecop': {
+        'host': {
+            'default': None,
+            'doc': "secop host name (string)"
+        },
+        'port': {
+            'default': '5000',
+            'doc': "secop port name (string)"
+        },
+        'message': {
+            'default': None,
+            'doc': "secop command MANDATORY (string)"
+        },
+        'timeout': {
+            'default': '0.0001',
+            'doc': "secop timeout (string)"
+        },
+        'group': {
+            'default': None,
+            'doc': "secop group name (string)"
+        },
+        'access': {
+            'default': None,
+            'doc': "secop access list (string)"
+        },
+    },
+    'singlesecop': {
+        'host': {
+            'default': None,
+            'doc': "secop host name (string)"
+        },
+        'port': {
+            'default': '5000',
+            'doc': "secop port name (string)"
+        },
+        'message': {
+            'default': None,
+            'doc': "secop command MANDATORY (string)"
+        },
+        'timeout': {
+            'default': '0.0001',
+            'doc': "secop timeout (string)"
+        },
+    },
     'pointdet': {
         'data': {
             'default': None,
             'doc': "diode data (datasource)"
         },
         'detname': {
             'default': 'detector',
             'doc': "detector group name (string)"
         },
     },
+    'coboldhisto': {
+        'histogram': {
+            'default': None,
+            'doc': "histogram data (datasource)"
+        },
+        'binsize': {
+            'default': None,
+            'doc': "bin size of histogram data (datasource)"
+        },
+        'exposuretime': {
+            'default': None,
+            'doc': "exposure time for histogram data (datasource)"
+        },
+    },
     'maiaflux': {
         'detname': {
             'default': "maia",
             'doc': "detector (alias) name (string)"
         },
         'fname': {
             'default': "fluxdevice",
@@ -753,14 +848,26 @@
         },
         'transformations': {
             'default': None,
             'doc': "transformations group name i.e. 'transformations'. "
             "If it is  not set it is not created (string)"
         },
     },
+    'tango': {
+        'device': {
+            'default': None,
+            'doc': "tango device MANDATORY (string)"
+        },
+        'attribute': {
+            'default': 'Position',
+            'doc': "tango device attribute (string)"
+        },
+    },
+    'starttime': {
+    },
     'beamtimeid': {
         'shortname': {
             'default': "P09",
             'doc': "beamline short name (string)"
         },
         'currentdir': {
             'default': "/gpfs/current",
@@ -787,14 +894,48 @@
             'doc': "commission file prefix (string)"
         },
         'commissionpostfix': {
             'default': ".json",
             'doc': "commission file postfix (string)"
         },
     },
+    'beamtimefname': {
+        'shortname': {
+            'default': "P09",
+            'doc': "beamline short name (string)"
+        },
+        'currentdir': {
+            'default': "/gpfs/current",
+            'doc': "beamtime file directory (string)"
+        },
+        'localdir': {
+            'default': "/gpfs/local",
+            'doc': "local file directory (string)"
+        },
+        'currentprefix': {
+            'default': "beamtime-metadata-",
+            'doc': "beamtime file prefix (string)"
+        },
+        'currentpostfix': {
+            'default': ".json",
+            'doc': "beamtime file postfix (string)"
+        },
+        'commissiondir': {
+            'default': "/gpfs/commissioning",
+            'doc': "commission file directory (string)"
+        },
+        'commissionprefix': {
+            'default': "commissioning-metadata-",
+            'doc': "commission file prefix (string)"
+        },
+        'commissionpostfix': {
+            'default': ".json",
+            'doc': "commission file postfix (string)"
+        },
+    },
     'default': {
         'control': {
             'default': None,
             'doc': "group name of the monitor (string)"
         },
         'shortname': {
             'default': "P09",
@@ -824,19 +965,120 @@
             'default': 'source',
             'doc': "source group name (string)"
         },
     },
     'datasignal': {
         'signal': {
             'default': 'defaultsignal',
-            'doc': "data signal field name (string)"
+            'doc': "data signal field name (datasource)"
+        },
+        'axes': {
+            'default': None,
+            'doc': "data axes field name(s) (datasource)"
+        },
+        'nchannelstoskip': {
+            'default': '0',
+            'doc': "number of mg channels to skip (string)"
+        },
+        'sardanasignal': {
+            'default': 'SignalCounter',
+            'doc': "signal sardana variable name (string)"
+        },
+        'msenv': {
+            'default': None,
+            'doc': "sardana environment (datasource)"
+        },
+        'mssardanadevice': {
+            'default': None,
+            'doc': "macroserver sardana device name MANDATORY (string)"
+        },
+        '__tangohost__': {
+            'default': "localhost",
+            'doc': "tango host (string)"
+        },
+        '__tangoport__': {
+            'default': "10000",
+            'doc': "tango port (string)"
+        },
+    },
+    'parametercopymap': {
+        'program': {
+            'default': 'nxsfileinfo_parameters',
+            'doc': "group name of NXparameters (string)"
+        },
+        'parameter': {
+            'default': 'copymap',
+            'doc': "parameter name of copymap (string)"
+        },
+        'copymap': {
+            'default': None,
+            'doc': "yaml dictionary with {output: input} copy map (string)"
+        },
+    },
+    'dataaxessignal': {
+        'signal': {
+            'default': 'defaultsignal',
+            'doc': "data signal field name (datasource)"
+        },
+        'sardanasignal': {
+            'default': 'SignalCounter',
+            'doc': "signal sardana variable name (string)"
         },
         'axes': {
+            'default': 'defaultaxes',
+            'doc': "list of data axes field names (datasource)"
+        },
+        'nchannelstoskip': {
+            'default': '0',
+            'doc': "number of mg channels to skip (string)"
+        },
+        'msenv': {
+            'default': None,
+            'doc': "sardana environment (datasource)"
+        },
+        'mssardanadevice': {
             'default': None,
-            'doc': "data axes field name(s) (string)"
+            'doc': "macroserver sardana device name MANDATORY (string)"
+        },
+        '__tangohost__': {
+            'default': "localhost",
+            'doc': "tango host (string)"
+        },
+        '__tangoport__': {
+            'default': "10000",
+            'doc': "tango port (string)"
+        },
+        'defaultattrs': {
+            'default': "False",
+            'doc': "add default attributes (string)"
+        },
+
+    },
+    'descriptiontext': {
+        'description': {
+            'default': "scan",
+            'doc': "scan technique (string)"
+        },
+    },
+    'description': {
+    },
+    'sampledescriptiontext': {
+        'sname': {
+            'default': 'sample',
+            'doc': "sample group name (string)"
+        },
+        'description': {
+            'default': "",
+            'doc': "sample description or sampleId (string)"
+        },
+    },
+    'sampledescription': {
+        'sname': {
+            'default': 'sample',
+            'doc': "sample group name (string)"
         },
     },
     'defaultinstrument': {
         'control': {
             'default': None,
             'doc': "group name of the monitor (string)"
         },
@@ -1293,29 +1535,85 @@
 #: (:obj:`dict` <:obj:`str` , :obj:`list` <:obj:`str`> >)
 #:     xml template files of modules
 standardComponentTemplateFiles = {
     'qbpm': [
         'qbpm_foil.ds.xml',
         'qbpm.xml',
     ],
+    'parametercopymap': [
+        'parametercopymap.xml',
+    ],
+    'secop': [
+        'secop.ds.xml',
+        'secop_time.ds.xml',
+        'client_start_time.ds.xml',
+        'sample_env_links.ds.xml',
+        'sample_log_links.ds.xml',
+    ],
+    'secoplinks': [
+        'sample_env_links.ds.xml',
+        'sample_log_links.ds.xml',
+        'sample_nxdata.ds.xml',
+        'sampleenv_nxdata.ds.xml',
+    ],
+    'singlesecop': [
+        'singlesecop.ds.xml',
+        'singlesecop_time.ds.xml',
+        'client_start_time.ds.xml',
+        'sample_env_links.ds.xml',
+        'sample_log_links.ds.xml',
+    ],
+    'groupsecop': [
+        'groupsecop.ds.xml',
+        'groupsecop_time.ds.xml',
+        'client_start_time.ds.xml',
+        'sample_env_links.ds.xml',
+        'sample_log_links.ds.xml',
+    ],
     'slit': ['slit.xml'],
     'source': ['source.xml'],
     'undulator': ['undulator.xml'],
     'beamtimeid': [
         'beamtimeid.xml',
         'beamtimeid.ds.xml',
         'start_time.ds.xml',
     ],
+    'starttime': [
+        'starttime.xml',
+        'starttime.ds.xml',
+        'start_timestamp.ds.xml',
+        'client_start_time.ds.xml',
+    ],
+    'beamtimefname': [
+        'beamtimefname.xml',
+        'beamtimefname.ds.xml',
+        'start_time.ds.xml',
+    ],
+    'description': [
+        'description.xml',
+        'experiment_description.ds.xml',
+    ],
+    'descriptiontext': [
+        'descriptiontext.xml',
+    ],
+    'sampledescription': [
+        'sampledescription.xml',
+        'sample_description.ds.xml',
+    ],
+    'sampledescriptiontext': [
+        'sampledescriptiontext.xml',
+    ],
     'default': [
         'default.xml',
         'defaultsample.xml',
         'defaultinstrument.xml',
         'sample_name.ds.xml',
         'chemical_formula.ds.xml',
         'beamtime_id.ds.xml',
+        'beamtime_filename.ds.xml',
         'start_time.ds.xml',
         'end_time.ds.xml',
         'nexdatas_version.ds.xml',
         'nexdatas_configuration.ds.xml',
         'title.ds.xml',
     ],
     'defaultsample': [
@@ -1325,18 +1623,28 @@
     ],
     'datasignal': [
         'datasignal.xml',
         'defaultsignal.ds.xml',
         'signal_name.ds.xml',
         'signalname.ds.xml',
         'signal_axes.ds.xml',
+        'sardanaenvironment.ds.xml',
+    ],
+    'dataaxessignal': [
+        'dataaxessignal.xml',
+        'defaultsignal.ds.xml',
+        'defaultaxes.ds.xml',
+        'signal_name.ds.xml',
+        'signalname.ds.xml',
+        'sardanaenvironment.ds.xml',
     ],
     'defaultinstrument': [
         'defaultinstrument.xml',
         'beamtime_id.ds.xml',
+        'beamtime_filename.ds.xml',
         'start_time.ds.xml',
         'end_time.ds.xml',
         'nexdatas_version.ds.xml',
         'nexdatas_configuration.ds.xml',
         'title.ds.xml',
     ],
     'dcm': [
@@ -1377,14 +1685,17 @@
     ],
     'collect6': [
         'collect6.xml',
     ],
     'common2': [
         'common2_common.ds.xml',
     ],
+    'tango': [
+        'tango.ds.xml',
+    ],
     'common3': [
         'common3_common.ds.xml',
     ],
     'detectorlive': [
         'detectorlive.xml',
     ],
     'msnsar': [
@@ -1411,20 +1722,26 @@
     ],
     'samplehkl': [
         'samplehkl.xml'
     ],
     'pointdet': [
         'pointdet.xml',
     ],
+    'coboldhisto': [
+        'coboldhisto.xml',
+        'coboldhisto_timeofflight.ds.xml',
+    ],
+
 }
 
 #: (:obj:`dict` <:obj:`str` , :obj:`list` <:obj:`str`> >)
 #:     xml template files of modules
 moduleTemplateFiles = {
     'mythen2': ['mythen2.xml'],
+    'cobold': ['cobold.xml'],
     'mythen': ['mythen.xml',
                'mythen_postrun.ds.xml',
                'mythen_filestartnumber.ds.xml'],
     'pilatus100k': ['pilatus.xml',
                     'pilatus_postrun.ds.xml',
                     'pilatus100k_description.ds.xml',
                     'pilatus_mxparameters_cb.ds.xml',
@@ -1489,14 +1806,22 @@
                   'lambdavds_savefilename_cb.ds.xml'],
     'tangovimba': ['tangovimba.xml',
                    'tangovimba_nxdata.ds.xml',
                    'tangovimba_external_data.ds.xml'],
     'dalsa': ['dalsa.xml',
               'dalsa_nxdata.ds.xml',
               'dalsa_external_data.ds.xml'],
+    'dalsavds': ['dalsavds.xml',
+                 'dalsavds_nxdata.ds.xml',
+                 'dalsavds_triggermode_cb.ds.xml',
+                 'dalsavds_filestartnum_cb.ds.xml',
+                 'dalsavds_nrexposedframes_cb.ds.xml'],
+    'lambdavdsnm': ['lambdavdsnm.xml',
+                    'lambdavdsnm_triggermode_cb.ds.xml',
+                    'lambdavdsnm_nxdata.ds.xml'],
     'lambda2m': ['lambda2m.xml',
                  'lambda2m_m1_nxdata.ds.xml',
                  'lambda2m_m2_nxdata.ds.xml',
                  'lambda2m_m3_nxdata.ds.xml',
                  'lambda2m_m1_external_data.ds.xml',
                  'lambda2m_m2_external_data.ds.xml',
                  'lambda2m_m3_external_data.ds.xml'],
@@ -1668,35 +1993,45 @@
         'TriggerMode', 'ShutterTime', 'DelayTime', 'FrameNumbers', 'ThreadNo',
         'EnergyThreshold', 'OperatingMode', 'ConfigFilePath', 'SaveAllImages',
         'FilePrefix', 'FileStartNum', 'FilePreExt', 'FilePostfix',
         'SaveFilePath', 'SaveFileName', 'LatestImageNumber', 'LiveMode',
         'TotalLossFrames', 'CompressorShuffle', 'CompressionRate',
         'CompressionEnabled', 'Layout', 'ShutterTimeMax', 'ShutterTimeMin',
         'Width', 'Height', 'Depth', 'LiveFrameNo', 'DistortionCorrection',
-        'LiveLastImageData', 'FramesPerFile', 'OpMode'
+        'LiveLastImageData', 'FramesPerFile', 'OpMode', 'Translations'
     ],
     'lambdavds': [
         'TriggerMode', 'ShutterTime', 'DelayTime', 'FrameNumbers', 'ThreadNo',
         'EnergyThreshold', 'OperatingMode', 'ConfigFilePath', 'SaveAllImages',
         'FilePrefix', 'FileStartNum', 'FilePreExt', 'FilePostfix',
         'SaveFilePath', 'SaveFileName', 'LatestImageNumber', 'LiveMode',
         'TotalLossFrames', 'CompressorShuffle', 'CompressionRate',
         'CompressionEnabled', 'Layout', 'ShutterTimeMax', 'ShutterTimeMin',
         'Width', 'Height', 'Depth', 'LiveFrameNo', 'DistortionCorrection',
-        'LiveLastImageData', 'FramesPerFile', 'OpMode'
+        'LiveLastImageData', 'FramesPerFile', 'OpMode', 'Translations'
+    ],
+    'lambdavdsnm': [
+        'TriggerMode', 'ShutterTime', 'DelayTime', 'FrameNumbers', 'ThreadNo',
+        'EnergyThreshold', 'OperatingMode', 'ConfigFilePath', 'SaveAllImages',
+        'FilePrefix', 'FileStartNum', 'FilePreExt', 'FilePostfix',
+        'SaveFilePath', 'SaveFileName', 'LatestImageNumber', 'LiveMode',
+        'TotalLossFrames', 'CompressorShuffle', 'CompressionRate',
+        'CompressionEnabled', 'Layout', 'ShutterTimeMax', 'ShutterTimeMin',
+        'Width', 'Height', 'Depth', 'LiveFrameNo', 'DistortionCorrection',
+        'LiveLastImageData', 'FramesPerFile', 'OpMode', 'Translations'
     ],
     'lambda2m': [
         'TriggerMode', 'ShutterTime', 'DelayTime', 'FrameNumbers', 'ThreadNo',
         'EnergyThreshold', 'OperatingMode', 'ConfigFilePath', 'SaveAllImages',
         'FilePrefix', 'FileStartNum', 'FilePreExt', 'FilePostfix',
         'SaveFilePath', 'SaveFileName', 'LatestImageNumber', 'LiveMode',
         'TotalLossFrames', 'CompressorShuffle', 'CompressionRate',
         'CompressionEnabled', 'Layout', 'ShutterTimeMax', 'ShutterTimeMin',
         'Width', 'Height', 'Depth', 'LiveFrameNo', 'DistortionCorrection',
-        'LiveLastImageData', 'OpMode'
+        'LiveLastImageData', 'OpMode', 'Translations'
     ],
     'pedetector': [
         'BinningMode', 'FileIndex', 'ExposureTime', 'SkippedAtStart',
         'SummedSaveImages', 'SkippedBetweenSaved', 'FilesAfterTrigger',
         'FilesBeforeTrigger', 'SummedDarkImages', 'OutputDirectory',
         'FilePattern', 'FileName', 'LogFile', 'UserComment1', 'CameraGain',
         'UserComment2', 'UserComment3', 'UserComment4', 'SaveRawImages',
@@ -1713,14 +2048,17 @@
     ],
     'mythen2': [
         'Counts1', 'Counts2', 'CountsMax', 'CountsTotal', 'ExposureTime',
         'FileDir', 'FileIndex', 'FilePrefix', 'Data',
         'Energy', 'NbFrames', 'RoI1End', 'RoI2End', 'RoI1Start', 'RoI2Start',
         'Threshold'
     ],
+    'cobold': [
+        'BinSize', 'ExposureTime'
+    ],
     'marccd': [
         'FrameShift', 'SavingDirectory', 'SavingPostfix', 'SavingPrefix'],
     'eigerdectris': [
         'TriggerMode', 'NbTriggers', 'Description', 'NbImages', 'BitDepth',
         'ReadoutTime', 'CountTime', 'EnergyThreshold', 'FrameTime',
         'RateCorrectionEnabled', 'FlatFieldEnabled', 'Temperature',
         'AutoSummationEnabled', 'Humidity', 'PhotonEnergy', 'Wavelength',
@@ -1738,12 +2076,24 @@
         'FileDir', 'FilePostfix', 'FilePrefix', 'FileSaving', 'FileStartNum',
         'TriggerMode', 'Width', 'Height', 'ExtendedExposure',
         'BinComment',
         'FramesProcessed', 'Image16', 'Image8', 'ImageRaw',
         'FramesReceived', 'FrameRate', 'FramesPerNXFile', 'NXFileCompression',
         'TurboMode', 'ImageEnc', 'ViewingMode',
         'ThrashedBuffers', 'FramesToAcquire',
+        'AcquisitionFrameCount', 'AcquisitionMode', 'AcquisitionFrameMode',
+        'LinearityEqualizer', 'NrExposedFrames', 'NrOffsetFrames',
+        'Offset', 'PixelFormat', 'ReadOutMode', 'Standby', 'SumScheme'
+    ],
+    'dalsavds': [
+        'FileDir', 'FilePostfix', 'FilePrefix', 'FileSaving', 'FileStartNum',
+        'TriggerMode', 'Width', 'Height', 'ExtendedExposure',
+        'BinComment',
+        'FramesProcessed', 'Image16', 'Image8', 'ImageRaw',
+        'FramesReceived', 'FrameRate', 'FramesPerNXFile', 'NXFileCompression',
+        'TurboMode', 'ImageEnc', 'ViewingMode',
+        'ThrashedBuffers', 'FramesToAcquire',
         'AcquisitionFrameCount', 'AcquisitionMode', 'AcquisitionFrameMode',
         'LinearityEqualizer', 'NrExposedFrames', 'NrOffsetFrames',
         'Offset', 'PixelFormat', 'ReadOutMode', 'Standby', 'SumScheme'
     ],
 }
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/absorber.xml` & `nxstools-4.0.0/nxstools/xmltemplates/absorber.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/beamstop.xml` & `nxstools-4.0.0/nxstools/xmltemplates/beamstop.xml`

 * *Files 5% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/beamstop.xml` & `nxstools-4.0.0/nxstools/xmltemplates/beamstop.xml`

```diff
@@ -4,15 +4,15 @@
     <group type="NXinstrument" name="$(__insname__)">
       <group type="NXbeam_stop" name="$(name)">
         <field type="NX_CHAR" name="description">
           <strategy mode="INIT"/>
           $(description)
         </field>
         <field type="NX_CHAR" name="depends_on">
-          transformations/y
+          transformations/$(yname)
           <strategy mode="INIT"/>
         </field>
         <group type="NXtransformations" name="transformations">
           <field depends_on="$(xname)" units="mm" type="NX_FLOAT64" name="$(yname)">
             <strategy mode="INIT"/>
             $datasources.$(y)
             <attribute type="NX_CHAR" name="transformation_type">
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/chcut.xml` & `nxstools-4.0.0/nxstools/xmltemplates/chcut.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/dalsa.xml` & `nxstools-4.0.0/nxstools/xmltemplates/dalsa.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/dalsa_nxdata.ds.xml`

 * *Format-specific differences are supported for XML files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: XML 1.0 document, ASCII text*

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 00000170: 290a 2020 2020 2020 2020 6473 2e72 6573  ).        ds.res
 00000180: 756c 7420 3d20 2224 7661 722e 656e 7472  ult = "$var.entr
 00000190: 796e 616d 6523 2724 285f 5f65 6e74 7279  yname#'$(__entry
 000001a0: 6e61 6d65 5f5f 2927 2476 6172 2e73 6572  name__)'$var.ser
 000001b0: 6961 6c6e 6f3a 4e58 656e 7472 792f 2428  ialno:NXentry/$(
 000001c0: 5f5f 696e 736e 616d 655f 5f29 2f24 286e  __insname__)/$(n
 000001d0: 616d 6529 5f65 7874 6572 6e61 6c3a 4e58  ame)_external:NX
-000001e0: 6465 7465 6374 6f72 2f64 6174 6122 3c2f  detector/data"</
-000001f0: 7265 7375 6c74 3e0a 2024 6461 7461 736f  result>. $dataso
-00000200: 7572 6365 732e 2428 6e61 6d65 295f 6669  urces.$(name)_fi
-00000210: 6c65 7072 6566 6978 0a20 2464 6174 6173  leprefix. $datas
-00000220: 6f75 7263 6573 2e24 286e 616d 6529 5f66  ources.$(name)_f
-00000230: 696c 6570 6f73 7466 6978 3c2f 6461 7461  ilepostfix</data
-00000240: 736f 7572 6365 3e0a 3c2f 6465 6669 6e69  source>.</defini
-00000250: 7469 6f6e 3e0a                           tion>.
+000001e0: 6465 7465 6374 6f72 2f64 6174 6122 0a3c  detector/data".<
+000001f0: 2f72 6573 756c 743e 0a20 2464 6174 6173  /result>. $datas
+00000200: 6f75 7263 6573 2e24 286e 616d 6529 5f66  ources.$(name)_f
+00000210: 696c 6570 7265 6669 780a 2024 6461 7461  ileprefix. $data
+00000220: 736f 7572 6365 732e 2428 6e61 6d65 295f  sources.$(name)_
+00000230: 6669 6c65 706f 7374 6669 783c 2f64 6174  filepostfix</dat
+00000240: 6173 6f75 7263 653e 0a3c 2f64 6566 696e  asource>.</defin
+00000250: 6974 696f 6e3e 0a                        ition>.
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/dcm.xml` & `nxstools-4.0.0/nxstools/xmltemplates/dcm.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/defaultinstrument.xml` & `nxstools-4.0.0/nxstools/xmltemplates/defaultinstrument.xml`

 * *Files 7% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/defaultinstrument.xml` & `nxstools-4.0.0/nxstools/xmltemplates/defaultinstrument.xml`

```diff
@@ -3,14 +3,18 @@
   <group type="NXentry" name="$var.entryname#'$(__entryname__)'$var.serialno">
     <field type="NX_CHAR" name="experiment_identifier">
       <doc>Beamtime ID. From this ID everything else can be derived from the DESY databases including the Proposal as well as the scientists performing the experiment, the local contact, and so on.
 
 The beamtime ID at DESY is an 8 digit number.R</doc>
       <strategy mode="INIT"/>
       $datasources.beamtime_id
+      <attribute type="NX_CHAR" name="beamtime_filename">
+        <strategy mode="INIT"/>
+        $datasources.beamtime_filename
+      </attribute>
     </field>
     <field type="NX_DATE_TIME" name="start_time">
       <doc>time stamp when the experiment has started.</doc>
       <strategy mode="INIT"/>
       $datasources.start_time
     </field>
     <field type="NX_DATE_TIME" name="end_time">
@@ -46,15 +50,15 @@
         </field>
       </group>
       <field short_name="$(shortname)" type="NX_CHAR" name="name">
         $(longname)
         <strategy mode="INIT"/>
       </field>
     </group>
-    <field scan_command="$var.scan_title" scan_id="$var.scan_id" type="NX_CHAR" name="program_name">
+    <field scan_command="$var.scan_title" scan_id="$var.scan_id" npoints="$var.npoints" count_time="$var.count_time" beamtime_id="$var.beamtime_id" measurement_group="$var.measurement_group" measurement_group_channels="$var.mgchannels" nexus_components="$var.nexus_components" nexus_step_datasources="$var.nexus_step_datasources" nexus_init_datasources="$var.nexus_init_datasources" type="NX_CHAR" name="program_name">
       NexDaTaS
       <attribute type="NX_CHAR" name="version">
         <strategy mode="INIT"/>
         $datasources.nexdatas_version
       </attribute>
       <attribute type="NX_CHAR" name="configuration">
         <strategy mode="INIT"/>
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/detectorlive.xml` & `nxstools-4.0.0/nxstools/xmltemplates/detectorlive.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/eigerdectris.xml` & `nxstools-4.0.0/nxstools/xmltemplates/eigerdectris.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/keithley.xml` & `nxstools-4.0.0/nxstools/xmltemplates/keithley.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambda.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambda.xml`

 * *Files 2% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambda.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambda.xml`

```diff
@@ -25,18 +25,14 @@
             <strategy mode="FINAL"/>
             $datasources.$(name)_triggermode
           </field>
           <field units="ms" type="NX_FLOAT64" name="shutter_time">
             <strategy mode="FINAL"/>
             $datasources.$(name)_shuttertime
           </field>
-          <field units="ms" type="NX_FLOAT64" name="delay_time">
-            <strategy mode="FINAL"/>
-            $datasources.$(name)_delaytime
-          </field>
           <field type="NX_INT64" name="frame_numbers">
             <strategy mode="FINAL"/>
             $datasources.$(name)_framenumbers
           </field>
           <field type="NX_BOOLEAN" name="save_all_images">
             <strategy mode="FINAL"/>
             $datasources.$(name)_saveallimages
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambda2m.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambda2m.xml`

 * *Files 1% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambda2m.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambda2m.xml`

```diff
@@ -25,18 +25,14 @@
             <strategy mode="FINAL"/>
             $datasources.$(name)_triggermode
           </field>
           <field units="ms" type="NX_FLOAT64" name="shutter_time">
             <strategy mode="FINAL"/>
             $datasources.$(name)_shuttertime
           </field>
-          <field units="ms" type="NX_FLOAT64" name="delay_time">
-            <strategy mode="FINAL"/>
-            $datasources.$(name)_delaytime
-          </field>
           <field type="NX_INT64" name="frame_numbers">
             <strategy mode="FINAL"/>
             $datasources.$(name)_framenumbers
           </field>
           <field type="NX_BOOLEAN" name="save_all_images">
             <strategy mode="FINAL"/>
             $datasources.$(name)_saveallimages
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambda_external_data.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/pco_postrun.ds.xml`

 * *Files 24% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambda_external_data.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/pco_postrun.ds.xml`

```diff
@@ -1,20 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <definition>
-  <datasource type="PYEVAL" name="$(name)_external_data">
-    <result name="result">from nxstools.pyeval import lmbd
-ds.result = lmbd.external_data(
-    commonblock,
-    &quot;$(name)&quot;,
-    ds.$(name)_savefilename,
-    ds.$(name)_saveallimages,
-    ds.$(name)_framesperfile,
-    ds.$(name)_framenumbers,
-    ds.$(name)_filepostfix,
-    &quot;$var.filename&quot;)</result>
-    $datasources.$(name)_savefilename
- $datasources.$(name)_saveallimages
- $datasources.$(name)_framesperfile
- $datasources.$(name)_framenumbers
+  <datasource type="PYEVAL" name="$(name)_postrun">
+    <result name="result">from nxstools.pyeval import pco
+ds.result = pco.postrun(commonblock, ds.$(name)_filestartnum, ds.$(name)_filedir, ds.$(name)_nbframes, ds.$(name)_filepostfix, ds.$(name)_fileprefix, &quot;$(name)_filestartnum&quot;)</result>
+    $datasources.$(name)_filestartnum
+ $datasources.$(name)_filedir
+ $datasources.$(name)_nbframes
  $datasources.$(name)_filepostfix
+ $datasources.$(name)_fileprefix
   </datasource>
 </definition>
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambdavds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambdavds.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml`

 * *Files 9% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambdavds_triggermode_cb.ds.xml`

```diff
@@ -1,25 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <definition>
   <datasource type="PYEVAL" name="$(name)_triggermode_cb">
     <result name="result">from nxstools.pyeval import lambdavds
-ds.result = lambdavds.triggermode_cb(
-    commonblock,
-    &quot;$(name)&quot;,
-    ds.$(name)_triggermode,
-    ds.$(name)_saveallimages,
-    ds.$(name)_framesperfile,
-    ds.$(name)_height,
-    ds.$(name)_width,
-    ds.$(name)_opmode,
-    ds.$(name)_filepostfix,
-    &quot;$(name)_savefilename&quot;,
-    &quot;$(name)_framenumbers&quot;,
-    &quot;$var.filename&quot;,
-    &quot;$var.entryname#'$(__entryname__)'$var.serialno&quot;)</result>
+ds.result = lambdavds.triggermode_cb(commonblock, &quot;$(name)&quot;, ds.$(name)_triggermode, ds.$(name)_saveallimages, ds.$(name)_framesperfile, ds.$(name)_height, ds.$(name)_width, ds.$(name)_opmode, ds.$(name)_filepostfix, &quot;$(name)_savefilename&quot;, &quot;$(name)_framenumbers&quot;, &quot;$var.filename&quot;, &quot;$var.entryname#'$(__entryname__)'$var.serialno&quot;)</result>
     $datasources.$(name)_triggermode
     $datasources.$(name)_opmode
     $datasources.$(name)_savefilename
     $datasources.$(name)_saveallimages
     $datasources.$(name)_framesperfile
     $datasources.$(name)_framenumbers
     $datasources.$(name)_filepostfix
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/limaccd.xml` & `nxstools-4.0.0/nxstools/xmltemplates/limaccd.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/limaccd_postrun.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambda_external_data.ds.xml`

 * *Files 20% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/limaccd_postrun.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/lambda_external_data.ds.xml`

```diff
@@ -1,21 +1,12 @@
 <?xml version="1.0" encoding="utf-8"?>
 <definition>
-  <datasource type="PYEVAL" name="$(name)_postrun">
-    <result name="result">from nxstools.pyeval import limaccd
-ds.result = limaccd.postrun(
-    commonblock,
-    ds.$(name)_saving_next_number,
-    ds.$(name)_saving_directory,
-    ds.$(name)_saving_suffix,
-    ds.$(name)_acq_nb_frames,
-    ds.$(name)_saving_format,
-    ds.$(name)_saving_prefix,
-    &quot;$(name)_saving_next_number&quot;)</result>
-    $datasources.$(name)_saving_next_number
- $datasources.$(name)_saving_directory
- $datasources.$(name)_saving_suffix
- $datasources.$(name)_acq_nb_frames
- $datasources.$(name)_saving_format
- $datasources.$(name)_saving_prefix
+  <datasource type="PYEVAL" name="$(name)_external_data">
+    <result name="result">from nxstools.pyeval import lmbd
+ds.result = lmbd.external_data(commonblock, &quot;$(name)&quot;, ds.$(name)_savefilename, ds.$(name)_saveallimages, ds.$(name)_framesperfile, ds.$(name)_framenumbers, ds.$(name)_filepostfix, &quot;$var.filename&quot;)</result>
+    $datasources.$(name)_savefilename
+ $datasources.$(name)_saveallimages
+ $datasources.$(name)_framesperfile
+ $datasources.$(name)_framenumbers
+ $datasources.$(name)_filepostfix
   </datasource>
 </definition>
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/maia.xml` & `nxstools-4.0.0/nxstools/xmltemplates/maia.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/maiadimension.xml` & `nxstools-4.0.0/nxstools/xmltemplates/maiadimension.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/maiaflux.xml` & `nxstools-4.0.0/nxstools/xmltemplates/maiaflux.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/marccd.xml` & `nxstools-4.0.0/nxstools/xmltemplates/marccd.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/mcaxia.xml` & `nxstools-4.0.0/nxstools/xmltemplates/mcaxia.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/mythen.xml` & `nxstools-4.0.0/nxstools/xmltemplates/mythen.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/mythen2.xml` & `nxstools-4.0.0/nxstools/xmltemplates/mythen2.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/pco.xml` & `nxstools-4.0.0/nxstools/xmltemplates/pco.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/pco_postrun.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml`

 * *Files 27% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/pco_postrun.ds.xml` & `nxstools-4.0.0/nxstools/xmltemplates/tangovimba_nxdata.ds.xml`

```diff
@@ -1,19 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <definition>
-  <datasource type="PYEVAL" name="$(name)_postrun">
-    <result name="result">from nxstools.pyeval import pco
-ds.result = pco.postrun(
-    commonblock,
-    ds.$(name)_filestartnum,
-    ds.$(name)_filedir,
-    ds.$(name)_nbframes,
-    ds.$(name)_filepostfix,
-    ds.$(name)_fileprefix,
-    &quot;$(name)_filestartnum&quot;)</result>
-    $datasources.$(name)_filestartnum
- $datasources.$(name)_filedir
- $datasources.$(name)_nbframes
+  <datasource type="PYEVAL" name="$(name)_nxdata">
+    <result name="result">ds.result = &quot;&quot;
+if ds.$(name)_fileprefix and ds.$(name)_filepostfix:
+    postfix = str(ds.$(name)_filepostfix)
+    if not postfix.startswith(&quot;.&quot;):
+        postfix = &quot;.&quot; + postfix
+    if postfix in [&quot;.nxs&quot;, &quot;.nx&quot;]:
+        prefix = str(ds.$(name)_fileprefix)
+        ds.result = &quot;$var.entryname#'$(__entryname__)'$var.serialno:NXentry/$(__insname__)/$(name)_external:NXdetector/data&quot;</result>
+    $datasources.$(name)_fileprefix
  $datasources.$(name)_filepostfix
- $datasources.$(name)_fileprefix
   </datasource>
 </definition>
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/perkinelmerdetector.xml` & `nxstools-4.0.0/nxstools/xmltemplates/perkinelmerdetector.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/pilatus.xml` & `nxstools-4.0.0/nxstools/xmltemplates/pilatus.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/pinhole.xml` & `nxstools-4.0.0/nxstools/xmltemplates/pinhole.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/pointdet.xml` & `nxstools-4.0.0/nxstools/xmltemplates/pointdet.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/qbpm.xml` & `nxstools-4.0.0/nxstools/xmltemplates/qbpm.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/samplehkl.xml` & `nxstools-4.0.0/nxstools/xmltemplates/samplehkl.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/slit.xml` & `nxstools-4.0.0/nxstools/xmltemplates/slit.xml`

 * *Files 12% similar despite different names*

#### Comparing `nxstools-3.9.0/nxstools/xmltemplates/slit.xml` & `nxstools-4.0.0/nxstools/xmltemplates/slit.xml`

```diff
@@ -25,31 +25,59 @@
           <strategy mode="INIT"/>
           $datasources.$(xgap)
         </field>
         <field units="mm" type="NX_FLOAT" name="y_gap">
           <strategy mode="INIT"/>
           $datasources.$(ygap)
         </field>
-        <field units="mm" type="NX_FLOAT" name="right">
-          <strategy mode="INIT"/>
-          $datasources.$(right)
-        </field>
-        <field units="mm" type="NX_FLOAT" name="top">
-          <strategy mode="INIT"/>
-          $datasources.$(top)
-        </field>
-        <field units="mm" type="NX_FLOAT" name="bottom">
-          <strategy mode="INIT"/>
-          $datasources.$(bottom)
-        </field>
-        <field units="mm" type="NX_FLOAT" name="left">
-          <strategy mode="INIT"/>
-          $datasources.$(left)
-        </field>
         <group type="NXtransformations" name="transformations">
+          <field units="mm" type="NX_FLOAT" name="right" transformation_type="translation">
+            <attribute type="NX_FLOAT64" name="vector">
+              1 0 0
+              <dimensions rank="1">
+                <dim value="3" index="1"/>
+              </dimensions>
+              <strategy mode="INIT"/>
+            </attribute>
+            <strategy mode="INIT"/>
+            $datasources.$(right)
+          </field>
+          <field units="mm" type="NX_FLOAT" name="top" transformation_type="translation">
+            <attribute type="NX_FLOAT64" name="vector">
+              0 1 0
+              <dimensions rank="1">
+                <dim value="3" index="1"/>
+              </dimensions>
+              <strategy mode="INIT"/>
+            </attribute>
+            <strategy mode="INIT"/>
+            $datasources.$(top)
+          </field>
+          <field units="mm" type="NX_FLOAT" name="bottom" transformation_type="translation">
+            <attribute type="NX_FLOAT64" name="vector">
+              0 1 0
+              <dimensions rank="1">
+                <dim value="3" index="1"/>
+              </dimensions>
+              <strategy mode="INIT"/>
+            </attribute>
+            <strategy mode="INIT"/>
+            $datasources.$(bottom)
+          </field>
+          <field units="mm" type="NX_FLOAT" name="left" transformation_type="translation">
+            <attribute type="NX_FLOAT64" name="vector">
+              1 0 0
+              <dimensions rank="1">
+                <dim value="3" index="1"/>
+              </dimensions>
+              <strategy mode="INIT"/>
+            </attribute>
+            <strategy mode="INIT"/>
+            $datasources.$(left)
+          </field>
           <field dependson="$(xoffdependson)" units="mm" type="NX_FLOAT" name="$(xoffsetname)" transformation_type="translation">
             <attribute type="NX_FLOAT64" name="vector">
               1 0 0
               <dimensions rank="1">
                 <dim value="3" index="1"/>
               </dimensions>
               <strategy mode="INIT"/>
```

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/source.xml` & `nxstools-4.0.0/nxstools/xmltemplates/source.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/tangovimba.xml` & `nxstools-4.0.0/nxstools/xmltemplates/tangovimba.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/nxstools/xmltemplates/undulator.xml` & `nxstools-4.0.0/nxstools/xmltemplates/undulator.xml`

 * *Files identical despite different names*

### Comparing `nxstools-3.9.0/setup.py` & `nxstools-4.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #    GNU General Public License for more details.
 #
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
-""" setup.py for command-line tools """
+""" setup.py for command-line nxstools """
 
 import os
 import sys
 from setuptools import setup
 # from setuptools.command.build_py import build_py
 # from distutils.core import setup
 from distutils.core import Command
@@ -36,21 +36,25 @@
 IPKG = __import__(PKG)
 
 needs_pytest = set(['test']).intersection(sys.argv)
 pytest_runner = ['pytest-runner'] if needs_pytest else []
 
 install_requires = [
     'argcomplete',
-    'h5py',
     'pytz',
     'numpy>1.6.0',
     'lxml',
-    'fabio',
+    # 'fabio',
+    'pyyaml',
+    # 'pil',
+    # 'matplotlib',
     # 'pytango',
     # 'pninexus',
+    # 'h5py',
+    # 'blissdata',
 ]
 
 
 def read(fname):
     """reading a file
 
     :param fname: file name
@@ -82,48 +86,54 @@
         errno = subprocess.call([sys.executable, 'test'])
         raise SystemExit(errno)
 
 
 release = IPKG.__version__
 version = ".".join(release.split(".")[:2])
 name = "NXSTools"
-author = "Jan Kotanski, Eugen Wintersberger , Halil Pasic",
-glicense = "GNU GENERAL PUBLIC LICENSE, version 3",
+author = "Jan Kotanski, Eugen Wintersberger , Halil Pasic"
+glicense = "GNU GENERAL PUBLIC LICENSE version 3"
 
 #: metadata for distutils
 SETUPDATA = dict(
     name="nxstools",
     version=IPKG.__version__,
     author=author,
     author_email="jankotan@gmail.com, eugen.wintersberger@gmail.com, "
     + "halil.pasic@gmail.com",
     maintainer="Jan Kotanski, Eugen Wintersberger , Halil Pasic",
     maintainer_email="jankotan@gmail.com, eugen.wintersberger@gmail.com, "
     + "halil.pasic@gmail.com",
     license=glicense,
     description=("Configuration tools for NeXDaTaS Tango Servers"),
     keywords="configuration writer Tango component nexus data",
-    url="http://github.com/nexdatas/tools",
+    url="http://github.com/nexdatas/nxstools",
     platforms=("Linux"),
     install_requires=install_requires,
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 2.7',
+        # 'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
+        # 'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
-    packages=["nxstools", "nxstools.xmltemplates", "nxstools.pyeval"],
-    package_data={'nxstools.xmltemplates': ['*.xml']},
+    packages=["nxstools", "nxstools.xmltemplates", "nxstools.pyeval",
+              "nxstools.ontology"],
+    package_data={'nxstools.xmltemplates': ['*.xml'],
+                  'nxstools.ontology': ['*.json']},
     scripts=[
         'nxsconfig',
         'nxsdata',
         'nxscreate',
         'nxscollect',
         'nxsetup',
         'nxsfileinfo',
```

