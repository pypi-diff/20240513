# Comparing `tmp/gref4hsi-0.2.1.tar.gz` & `tmp/gref4hsi-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gref4hsi-0.2.1.tar", last modified: Tue Apr 16 13:34:07 2024, max compression
+gzip compressed data, was "gref4hsi-0.2.2.tar", last modified: Mon May 13 06:58:08 2024, max compression
```

## Comparing `gref4hsi-0.2.1.tar` & `gref4hsi-0.2.2.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 13:34:07.701548 gref4hsi-0.2.1/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    13807 2024-03-07 12:34:03.000000 gref4hsi-0.2.1/LICENCE.MD
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       79 2024-03-12 08:17:47.000000 gref4hsi-0.2.1/MANIFEST.in
--rw-r--r--   0 haavasl   (1000) haavasl   (1000)    19494 2024-04-16 13:34:07.701548 gref4hsi-0.2.1/PKG-INFO
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    18091 2024-04-16 05:06:29.000000 gref4hsi-0.2.1/README.md
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 13:34:07.701548 gref4hsi-0.2.1/gref4hsi/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      205 2024-03-07 12:34:03.000000 gref4hsi-0.2.1/gref4hsi/__init__.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 13:34:07.701548 gref4hsi-0.2.1/gref4hsi/scripts/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.2.1/gref4hsi/scripts/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    39631 2024-04-16 12:37:56.000000 gref4hsi-0.2.1/gref4hsi/scripts/coregistration.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    11541 2024-04-16 13:03:33.000000 gref4hsi-0.2.1/gref4hsi/scripts/georeference.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9507 2024-04-16 05:03:47.000000 gref4hsi-0.2.1/gref4hsi/scripts/orthorectification.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 13:34:07.701548 gref4hsi-0.2.1/gref4hsi/tests/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.2.1/gref4hsi/tests/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    13138 2024-04-16 13:18:38.000000 gref4hsi-0.2.1/gref4hsi/tests/specim_process.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1616 2024-04-16 05:03:47.000000 gref4hsi-0.2.1/gref4hsi/tests/test_main_hi.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8210 2024-04-16 06:58:50.000000 gref4hsi-0.2.1/gref4hsi/tests/test_main_uhi.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3000 2024-03-07 12:34:03.000000 gref4hsi-0.2.1/gref4hsi/tests/test_multi_ray_trace.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3684 2024-03-07 14:11:10.000000 gref4hsi-0.2.1/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 13:34:07.701548 gref4hsi-0.2.1/gref4hsi/utils/
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        0 2024-03-07 12:34:03.000000 gref4hsi-0.2.1/gref4hsi/utils/__init__.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1588 2024-04-16 06:58:50.000000 gref4hsi-0.2.1/gref4hsi/utils/colours.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     3143 2024-03-13 12:06:06.000000 gref4hsi-0.2.1/gref4hsi/utils/config_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    54217 2024-04-16 11:02:46.000000 gref4hsi-0.2.1/gref4hsi/utils/geometry_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    44611 2024-04-16 10:02:44.000000 gref4hsi-0.2.1/gref4hsi/utils/gis_tools.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    22763 2024-04-16 08:34:32.000000 gref4hsi-0.2.1/gref4hsi/utils/parsing_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     8706 2024-03-15 10:24:09.000000 gref4hsi-0.2.1/gref4hsi/utils/photogrammetry_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    23551 2024-03-14 09:13:50.000000 gref4hsi-0.2.1/gref4hsi/utils/radiometry.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    25630 2024-04-16 05:03:47.000000 gref4hsi-0.2.1/gref4hsi/utils/specim_parsing_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)    33111 2024-04-16 06:58:50.000000 gref4hsi-0.2.1/gref4hsi/utils/uhi_parsing_utils.py
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     9874 2024-04-16 05:03:47.000000 gref4hsi-0.2.1/gref4hsi/utils/visualize.py
-drwxrwxr-x   0 haavasl   (1000) haavasl   (1000)        0 2024-04-16 13:34:07.701548 gref4hsi-0.2.1/gref4hsi.egg-info/
--rw-r--r--   0 haavasl   (1000) haavasl   (1000)    19494 2024-04-16 13:34:07.000000 gref4hsi-0.2.1/gref4hsi.egg-info/PKG-INFO
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      933 2024-04-16 13:34:07.000000 gref4hsi-0.2.1/gref4hsi.egg-info/SOURCES.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        1 2024-04-16 13:34:07.000000 gref4hsi-0.2.1/gref4hsi.egg-info/dependency_links.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      188 2024-04-16 13:34:07.000000 gref4hsi-0.2.1/gref4hsi.egg-info/requires.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)        9 2024-04-16 13:34:07.000000 gref4hsi-0.2.1/gref4hsi.egg-info/top_level.txt
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)      106 2024-03-12 08:17:47.000000 gref4hsi-0.2.1/pyproject.toml
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)       38 2024-04-16 13:34:07.701548 gref4hsi-0.2.1/setup.cfg
--rw-rw-r--   0 haavasl   (1000) haavasl   (1000)     1567 2024-04-16 13:28:43.000000 gref4hsi-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.757146 gref4hsi-0.2.2/
+-rw-rw-rw-   0        0        0    14098 2024-03-04 11:54:34.000000 gref4hsi-0.2.2/LICENCE.MD
+-rw-rw-rw-   0        0        0       82 2024-03-06 12:25:35.000000 gref4hsi-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    20439 2024-05-13 06:58:08.756146 gref4hsi-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    18380 2024-04-15 13:37:53.000000 gref4hsi-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.728146 gref4hsi-0.2.2/gref4hsi/
+-rw-rw-rw-   0        0        0      213 2024-02-16 10:12:17.000000 gref4hsi-0.2.2/gref4hsi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.738146 gref4hsi-0.2.2/gref4hsi/scripts/
+-rw-rw-rw-   0        0        0        0 2023-11-01 06:48:25.000000 gref4hsi-0.2.2/gref4hsi/scripts/__init__.py
+-rw-rw-rw-   0        0        0    69548 2024-05-07 16:41:37.000000 gref4hsi-0.2.2/gref4hsi/scripts/coregistration.py
+-rw-rw-rw-   0        0        0    11589 2024-05-03 06:39:17.000000 gref4hsi-0.2.2/gref4hsi/scripts/georeference.py
+-rw-rw-rw-   0        0        0    11972 2024-04-24 07:00:32.000000 gref4hsi-0.2.2/gref4hsi/scripts/georeference.py.orig
+-rw-rw-rw-   0        0        0     9719 2024-05-02 08:38:08.000000 gref4hsi-0.2.2/gref4hsi/scripts/orthorectification.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.744147 gref4hsi-0.2.2/gref4hsi/tests/
+-rw-rw-rw-   0        0        0        0 2023-11-08 14:43:38.000000 gref4hsi-0.2.2/gref4hsi/tests/__init__.py
+-rw-rw-rw-   0        0        0    15091 2024-05-04 04:58:01.000000 gref4hsi-0.2.2/gref4hsi/tests/specim_process.py
+-rw-rw-rw-   0        0        0    14929 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/tests/specim_process.py.orig
+-rw-rw-rw-   0        0        0     1669 2024-04-15 13:37:53.000000 gref4hsi-0.2.2/gref4hsi/tests/test_main_hi.py
+-rw-rw-rw-   0        0        0     8441 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/tests/test_main_uhi.py
+-rw-rw-rw-   0        0        0     3108 2023-11-01 06:48:25.000000 gref4hsi-0.2.2/gref4hsi/tests/test_multi_ray_trace.py
+-rw-rw-rw-   0        0        0     3812 2024-03-12 08:07:09.000000 gref4hsi-0.2.2/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.754146 gref4hsi-0.2.2/gref4hsi/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-15 08:51:42.000000 gref4hsi-0.2.2/gref4hsi/utils/__init__.py
+-rw-rw-rw-   0        0        0     2147 2024-04-30 18:24:21.000000 gref4hsi-0.2.2/gref4hsi/utils/colours.py
+-rw-rw-rw-   0        0        0     3228 2024-03-17 07:44:28.000000 gref4hsi-0.2.2/gref4hsi/utils/config_utils.py
+-rw-rw-rw-   0        0        0    55635 2024-05-03 07:59:57.000000 gref4hsi-0.2.2/gref4hsi/utils/geometry_utils.py
+-rw-rw-rw-   0        0        0    49663 2024-05-03 08:37:15.000000 gref4hsi-0.2.2/gref4hsi/utils/gis_tools.py
+-rw-rw-rw-   0        0        0    23336 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/utils/parsing_utils.py
+-rw-rw-rw-   0        0        0     8963 2024-03-17 07:44:28.000000 gref4hsi-0.2.2/gref4hsi/utils/photogrammetry_utils.py
+-rw-rw-rw-   0        0        0    24256 2024-03-17 07:44:28.000000 gref4hsi-0.2.2/gref4hsi/utils/radiometry.py
+-rw-rw-rw-   0        0        0    26314 2024-04-25 19:08:38.000000 gref4hsi-0.2.2/gref4hsi/utils/specim_parsing_utils.py
+-rw-rw-rw-   0        0        0    33987 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/utils/uhi_parsing_utils.py
+-rw-rw-rw-   0        0        0    10142 2024-04-23 10:50:45.000000 gref4hsi-0.2.2/gref4hsi/utils/visualize.py
+drwxrwxrwx   0        0        0        0 2024-05-13 06:58:08.755146 gref4hsi-0.2.2/gref4hsi.egg-info/
+-rw-rw-rw-   0        0        0    20439 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1009 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      188 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 06:58:08.000000 gref4hsi-0.2.2/gref4hsi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-03-05 11:15:42.000000 gref4hsi-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 06:58:08.757146 gref4hsi-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1621 2024-05-13 06:57:32.000000 gref4hsi-0.2.2/setup.py
```

### Comparing `gref4hsi-0.2.1/LICENCE.MD` & `gref4hsi-0.2.2/LICENCE.MD`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-EUROPEAN UNION PUBLIC LICENCE v. 1.2
-                      EUPL © the European Union 2007, 2016
-
-This European Union Public Licence (the ‘EUPL’) applies to the Work (as
-defined below) which is provided under the terms of this Licence. Any use of
-the Work, other than as authorised under this Licence is prohibited (to the
-extent such use is covered by a right of the copyright holder of the Work).
-
-The Work is provided under the terms of this Licence when the Licensor (as
-defined below) has placed the following notice immediately following the
-copyright notice for the Work:
-
-        Licensed under the EUPL
-
-or has expressed by any other means his willingness to license under the EUPL.
-
-1. Definitions
-
-In this Licence, the following terms have the following meaning:
-
-- ‘The Licence’: this Licence.
-
-- ‘The Original Work’: the work or software distributed or communicated by the
-  Licensor under this Licence, available as Source Code and also as Executable
-  Code as the case may be.
-
-- ‘Derivative Works’: the works or software that could be created by the
-  Licensee, based upon the Original Work or modifications thereof. This
-  Licence does not define the extent of modification or dependence on the
-  Original Work required in order to classify a work as a Derivative Work;
-  this extent is determined by copyright law applicable in the country
-  mentioned in Article 15.
-
-- ‘The Work’: the Original Work or its Derivative Works.
-
-- ‘The Source Code’: the human-readable form of the Work which is the most
-  convenient for people to study and modify.
-
-- ‘The Executable Code’: any code which has generally been compiled and which
-  is meant to be interpreted by a computer as a program.
-
-- ‘The Licensor’: the natural or legal person that distributes or communicates
-  the Work under the Licence.
-
-- ‘Contributor(s)’: any natural or legal person who modifies the Work under
-  the Licence, or otherwise contributes to the creation of a Derivative Work.
-
-- ‘The Licensee’ or ‘You’: any natural or legal person who makes any usage of
-  the Work under the terms of the Licence.
-
-- ‘Distribution’ or ‘Communication’: any act of selling, giving, lending,
-  renting, distributing, communicating, transmitting, or otherwise making
-  available, online or offline, copies of the Work or providing access to its
-  essential functionalities at the disposal of any other natural or legal
-  person.
-
-2. Scope of the rights granted by the Licence
-
-The Licensor hereby grants You a worldwide, royalty-free, non-exclusive,
-sublicensable licence to do the following, for the duration of copyright
-vested in the Original Work:
-
-- use the Work in any circumstance and for all usage,
-- reproduce the Work,
-- modify the Work, and make Derivative Works based upon the Work,
-- communicate to the public, including the right to make available or display
-  the Work or copies thereof to the public and perform publicly, as the case
-  may be, the Work,
-- distribute the Work or copies thereof,
-- lend and rent the Work or copies thereof,
-- sublicense rights in the Work or copies thereof.
-
-Those rights can be exercised on any media, supports and formats, whether now
-known or later invented, as far as the applicable law permits so.
-
-In the countries where moral rights apply, the Licensor waives his right to
-exercise his moral right to the extent allowed by law in order to make
-effective the licence of the economic rights here above listed.
-
-The Licensor grants to the Licensee royalty-free, non-exclusive usage rights
-to any patents held by the Licensor, to the extent necessary to make use of
-the rights granted on the Work under this Licence.
-
-3. Communication of the Source Code
-
-The Licensor may provide the Work either in its Source Code form, or as
-Executable Code. If the Work is provided as Executable Code, the Licensor
-provides in addition a machine-readable copy of the Source Code of the Work
-along with each copy of the Work that the Licensor distributes or indicates,
-in a notice following the copyright notice attached to the Work, a repository
-where the Source Code is easily and freely accessible for as long as the
-Licensor continues to distribute or communicate the Work.
-
-4. Limitations on copyright
-
-Nothing in this Licence is intended to deprive the Licensee of the benefits
-from any exception or limitation to the exclusive rights of the rights owners
-in the Work, of the exhaustion of those rights or of other applicable
-limitations thereto.
-
-5. Obligations of the Licensee
-
-The grant of the rights mentioned above is subject to some restrictions and
-obligations imposed on the Licensee. Those obligations are the following:
-
-Attribution right: The Licensee shall keep intact all copyright, patent or
-trademarks notices and all notices that refer to the Licence and to the
-disclaimer of warranties. The Licensee must include a copy of such notices and
-a copy of the Licence with every copy of the Work he/she distributes or
-communicates. The Licensee must cause any Derivative Work to carry prominent
-notices stating that the Work has been modified and the date of modification.
-
-Copyleft clause: If the Licensee distributes or communicates copies of the
-Original Works or Derivative Works, this Distribution or Communication will be
-done under the terms of this Licence or of a later version of this Licence
-unless the Original Work is expressly distributed only under this version of
-the Licence — for example by communicating ‘EUPL v. 1.2 only’. The Licensee
-(becoming Licensor) cannot offer or impose any additional terms or conditions
-on the Work or Derivative Work that alter or restrict the terms of the
-Licence.
-
-Compatibility clause: If the Licensee Distributes or Communicates Derivative
-Works or copies thereof based upon both the Work and another work licensed
-under a Compatible Licence, this Distribution or Communication can be done
-under the terms of this Compatible Licence. For the sake of this clause,
-‘Compatible Licence’ refers to the licences listed in the appendix attached to
-this Licence. Should the Licensee's obligations under the Compatible Licence
-conflict with his/her obligations under this Licence, the obligations of the
-Compatible Licence shall prevail.
-
-Provision of Source Code: When distributing or communicating copies of the
-Work, the Licensee will provide a machine-readable copy of the Source Code or
-indicate a repository where this Source will be easily and freely available
-for as long as the Licensee continues to distribute or communicate the Work.
-
-Legal Protection: This Licence does not grant permission to use the trade
-names, trademarks, service marks, or names of the Licensor, except as required
-for reasonable and customary use in describing the origin of the Work and
-reproducing the content of the copyright notice.
-
-6. Chain of Authorship
-
-The original Licensor warrants that the copyright in the Original Work granted
-hereunder is owned by him/her or licensed to him/her and that he/she has the
-power and authority to grant the Licence.
-
-Each Contributor warrants that the copyright in the modifications he/she
-brings to the Work are owned by him/her or licensed to him/her and that he/she
-has the power and authority to grant the Licence.
-
-Each time You accept the Licence, the original Licensor and subsequent
-Contributors grant You a licence to their contributions to the Work, under the
-terms of this Licence.
-
-7. Disclaimer of Warranty
-
-The Work is a work in progress, which is continuously improved by numerous
-Contributors. It is not a finished work and may therefore contain defects or
-‘bugs’ inherent to this type of development.
-
-For the above reason, the Work is provided under the Licence on an ‘as is’
-basis and without warranties of any kind concerning the Work, including
-without limitation merchantability, fitness for a particular purpose, absence
-of defects or errors, accuracy, non-infringement of intellectual property
-rights other than copyright as stated in Article 6 of this Licence.
-
-This disclaimer of warranty is an essential part of the Licence and a
-condition for the grant of any rights to the Work.
-
-8. Disclaimer of Liability
-
-Except in the cases of wilful misconduct or damages directly caused to natural
-persons, the Licensor will in no event be liable for any direct or indirect,
-material or moral, damages of any kind, arising out of the Licence or of the
-use of the Work, including without limitation, damages for loss of goodwill,
-work stoppage, computer failure or malfunction, loss of data or any commercial
-damage, even if the Licensor has been advised of the possibility of such
-damage. However, the Licensor will be liable under statutory product liability
-laws as far such laws apply to the Work.
-
-9. Additional agreements
-
-While distributing the Work, You may choose to conclude an additional
-agreement, defining obligations or services consistent with this Licence.
-However, if accepting obligations, You may act only on your own behalf and on
-your sole responsibility, not on behalf of the original Licensor or any other
-Contributor, and only if You agree to indemnify, defend, and hold each
-Contributor harmless for any liability incurred by, or claims asserted against
-such Contributor by the fact You have accepted any warranty or additional
-liability.
-
-10. Acceptance of the Licence
-
-The provisions of this Licence can be accepted by clicking on an icon ‘I
-agree’ placed under the bottom of a window displaying the text of this Licence
-or by affirming consent in any other similar way, in accordance with the rules
-of applicable law. Clicking on that icon indicates your clear and irrevocable
-acceptance of this Licence and all of its terms and conditions.
-
-Similarly, you irrevocably accept this Licence and all of its terms and
-conditions by exercising any rights granted to You by Article 2 of this
-Licence, such as the use of the Work, the creation by You of a Derivative Work
-or the Distribution or Communication by You of the Work or copies thereof.
-
-11. Information to the public
-
-In case of any Distribution or Communication of the Work by means of
-electronic communication by You (for example, by offering to download the Work
-from a remote location) the distribution channel or media (for example, a
-website) must at least provide to the public the information requested by the
-applicable law regarding the Licensor, the Licence and the way it may be
-accessible, concluded, stored and reproduced by the Licensee.
-
-12. Termination of the Licence
-
-The Licence and the rights granted hereunder will terminate automatically upon
-any breach by the Licensee of the terms of the Licence.
-
-Such a termination will not terminate the licences of any person who has
-received the Work from the Licensee under the Licence, provided such persons
-remain in full compliance with the Licence.
-
-13. Miscellaneous
-
-Without prejudice of Article 9 above, the Licence represents the complete
-agreement between the Parties as to the Work.
-
-If any provision of the Licence is invalid or unenforceable under applicable
-law, this will not affect the validity or enforceability of the Licence as a
-whole. Such provision will be construed or reformed so as necessary to make it
-valid and enforceable.
-
-The European Commission may publish other linguistic versions or new versions
-of this Licence or updated versions of the Appendix, so far this is required
-and reasonable, without reducing the scope of the rights granted by the
-Licence. New versions of the Licence will be published with a unique version
-number.
-
-All linguistic versions of this Licence, approved by the European Commission,
-have identical value. Parties can take advantage of the linguistic version of
-their choice.
-
-14. Jurisdiction
-
-Without prejudice to specific agreement between parties,
-
-- any litigation resulting from the interpretation of this License, arising
-  between the European Union institutions, bodies, offices or agencies, as a
-  Licensor, and any Licensee, will be subject to the jurisdiction of the Court
-  of Justice of the European Union, as laid down in article 272 of the Treaty
-  on the Functioning of the European Union,
-
-- any litigation arising between other parties and resulting from the
-  interpretation of this License, will be subject to the exclusive
-  jurisdiction of the competent court where the Licensor resides or conducts
-  its primary business.
-
-15. Applicable Law
-
-Without prejudice to specific agreement between parties,
-
-- this Licence shall be governed by the law of the European Union Member State
-  where the Licensor has his seat, resides or has his registered office,
-
-- this licence shall be governed by Belgian law if the Licensor has no seat,
-  residence or registered office inside a European Union Member State.
-
-Appendix
-
-‘Compatible Licences’ according to Article 5 EUPL are:
-
-- GNU General Public License (GPL) v. 2, v. 3
-- GNU Affero General Public License (AGPL) v. 3
-- Open Software License (OSL) v. 2.1, v. 3.0
-- Eclipse Public License (EPL) v. 1.0
-- CeCILL v. 2.0, v. 2.1
-- Mozilla Public Licence (MPL) v. 2
-- GNU Lesser General Public Licence (LGPL) v. 2.1, v. 3
-- Creative Commons Attribution-ShareAlike v. 3.0 Unported (CC BY-SA 3.0) for
-  works other than software
-- European Union Public Licence (EUPL) v. 1.1, v. 1.2
-- Québec Free and Open-Source Licence — Reciprocity (LiLiQ-R) or Strong
-  Reciprocity (LiLiQ-R+).
-
-The European Commission may update this Appendix to later versions of the
-above licences without producing a new version of the EUPL, as long as they
-provide the rights granted in Article 2 of this Licence and protect the
-covered Source Code from exclusive appropriation.
-
-All other changes or additions to this Appendix require the production of a
-new EUPL version.
+EUROPEAN UNION PUBLIC LICENCE v. 1.2
+                      EUPL © the European Union 2007, 2016
+
+This European Union Public Licence (the ‘EUPL’) applies to the Work (as
+defined below) which is provided under the terms of this Licence. Any use of
+the Work, other than as authorised under this Licence is prohibited (to the
+extent such use is covered by a right of the copyright holder of the Work).
+
+The Work is provided under the terms of this Licence when the Licensor (as
+defined below) has placed the following notice immediately following the
+copyright notice for the Work:
+
+        Licensed under the EUPL
+
+or has expressed by any other means his willingness to license under the EUPL.
+
+1. Definitions
+
+In this Licence, the following terms have the following meaning:
+
+- ‘The Licence’: this Licence.
+
+- ‘The Original Work’: the work or software distributed or communicated by the
+  Licensor under this Licence, available as Source Code and also as Executable
+  Code as the case may be.
+
+- ‘Derivative Works’: the works or software that could be created by the
+  Licensee, based upon the Original Work or modifications thereof. This
+  Licence does not define the extent of modification or dependence on the
+  Original Work required in order to classify a work as a Derivative Work;
+  this extent is determined by copyright law applicable in the country
+  mentioned in Article 15.
+
+- ‘The Work’: the Original Work or its Derivative Works.
+
+- ‘The Source Code’: the human-readable form of the Work which is the most
+  convenient for people to study and modify.
+
+- ‘The Executable Code’: any code which has generally been compiled and which
+  is meant to be interpreted by a computer as a program.
+
+- ‘The Licensor’: the natural or legal person that distributes or communicates
+  the Work under the Licence.
+
+- ‘Contributor(s)’: any natural or legal person who modifies the Work under
+  the Licence, or otherwise contributes to the creation of a Derivative Work.
+
+- ‘The Licensee’ or ‘You’: any natural or legal person who makes any usage of
+  the Work under the terms of the Licence.
+
+- ‘Distribution’ or ‘Communication’: any act of selling, giving, lending,
+  renting, distributing, communicating, transmitting, or otherwise making
+  available, online or offline, copies of the Work or providing access to its
+  essential functionalities at the disposal of any other natural or legal
+  person.
+
+2. Scope of the rights granted by the Licence
+
+The Licensor hereby grants You a worldwide, royalty-free, non-exclusive,
+sublicensable licence to do the following, for the duration of copyright
+vested in the Original Work:
+
+- use the Work in any circumstance and for all usage,
+- reproduce the Work,
+- modify the Work, and make Derivative Works based upon the Work,
+- communicate to the public, including the right to make available or display
+  the Work or copies thereof to the public and perform publicly, as the case
+  may be, the Work,
+- distribute the Work or copies thereof,
+- lend and rent the Work or copies thereof,
+- sublicense rights in the Work or copies thereof.
+
+Those rights can be exercised on any media, supports and formats, whether now
+known or later invented, as far as the applicable law permits so.
+
+In the countries where moral rights apply, the Licensor waives his right to
+exercise his moral right to the extent allowed by law in order to make
+effective the licence of the economic rights here above listed.
+
+The Licensor grants to the Licensee royalty-free, non-exclusive usage rights
+to any patents held by the Licensor, to the extent necessary to make use of
+the rights granted on the Work under this Licence.
+
+3. Communication of the Source Code
+
+The Licensor may provide the Work either in its Source Code form, or as
+Executable Code. If the Work is provided as Executable Code, the Licensor
+provides in addition a machine-readable copy of the Source Code of the Work
+along with each copy of the Work that the Licensor distributes or indicates,
+in a notice following the copyright notice attached to the Work, a repository
+where the Source Code is easily and freely accessible for as long as the
+Licensor continues to distribute or communicate the Work.
+
+4. Limitations on copyright
+
+Nothing in this Licence is intended to deprive the Licensee of the benefits
+from any exception or limitation to the exclusive rights of the rights owners
+in the Work, of the exhaustion of those rights or of other applicable
+limitations thereto.
+
+5. Obligations of the Licensee
+
+The grant of the rights mentioned above is subject to some restrictions and
+obligations imposed on the Licensee. Those obligations are the following:
+
+Attribution right: The Licensee shall keep intact all copyright, patent or
+trademarks notices and all notices that refer to the Licence and to the
+disclaimer of warranties. The Licensee must include a copy of such notices and
+a copy of the Licence with every copy of the Work he/she distributes or
+communicates. The Licensee must cause any Derivative Work to carry prominent
+notices stating that the Work has been modified and the date of modification.
+
+Copyleft clause: If the Licensee distributes or communicates copies of the
+Original Works or Derivative Works, this Distribution or Communication will be
+done under the terms of this Licence or of a later version of this Licence
+unless the Original Work is expressly distributed only under this version of
+the Licence — for example by communicating ‘EUPL v. 1.2 only’. The Licensee
+(becoming Licensor) cannot offer or impose any additional terms or conditions
+on the Work or Derivative Work that alter or restrict the terms of the
+Licence.
+
+Compatibility clause: If the Licensee Distributes or Communicates Derivative
+Works or copies thereof based upon both the Work and another work licensed
+under a Compatible Licence, this Distribution or Communication can be done
+under the terms of this Compatible Licence. For the sake of this clause,
+‘Compatible Licence’ refers to the licences listed in the appendix attached to
+this Licence. Should the Licensee's obligations under the Compatible Licence
+conflict with his/her obligations under this Licence, the obligations of the
+Compatible Licence shall prevail.
+
+Provision of Source Code: When distributing or communicating copies of the
+Work, the Licensee will provide a machine-readable copy of the Source Code or
+indicate a repository where this Source will be easily and freely available
+for as long as the Licensee continues to distribute or communicate the Work.
+
+Legal Protection: This Licence does not grant permission to use the trade
+names, trademarks, service marks, or names of the Licensor, except as required
+for reasonable and customary use in describing the origin of the Work and
+reproducing the content of the copyright notice.
+
+6. Chain of Authorship
+
+The original Licensor warrants that the copyright in the Original Work granted
+hereunder is owned by him/her or licensed to him/her and that he/she has the
+power and authority to grant the Licence.
+
+Each Contributor warrants that the copyright in the modifications he/she
+brings to the Work are owned by him/her or licensed to him/her and that he/she
+has the power and authority to grant the Licence.
+
+Each time You accept the Licence, the original Licensor and subsequent
+Contributors grant You a licence to their contributions to the Work, under the
+terms of this Licence.
+
+7. Disclaimer of Warranty
+
+The Work is a work in progress, which is continuously improved by numerous
+Contributors. It is not a finished work and may therefore contain defects or
+‘bugs’ inherent to this type of development.
+
+For the above reason, the Work is provided under the Licence on an ‘as is’
+basis and without warranties of any kind concerning the Work, including
+without limitation merchantability, fitness for a particular purpose, absence
+of defects or errors, accuracy, non-infringement of intellectual property
+rights other than copyright as stated in Article 6 of this Licence.
+
+This disclaimer of warranty is an essential part of the Licence and a
+condition for the grant of any rights to the Work.
+
+8. Disclaimer of Liability
+
+Except in the cases of wilful misconduct or damages directly caused to natural
+persons, the Licensor will in no event be liable for any direct or indirect,
+material or moral, damages of any kind, arising out of the Licence or of the
+use of the Work, including without limitation, damages for loss of goodwill,
+work stoppage, computer failure or malfunction, loss of data or any commercial
+damage, even if the Licensor has been advised of the possibility of such
+damage. However, the Licensor will be liable under statutory product liability
+laws as far such laws apply to the Work.
+
+9. Additional agreements
+
+While distributing the Work, You may choose to conclude an additional
+agreement, defining obligations or services consistent with this Licence.
+However, if accepting obligations, You may act only on your own behalf and on
+your sole responsibility, not on behalf of the original Licensor or any other
+Contributor, and only if You agree to indemnify, defend, and hold each
+Contributor harmless for any liability incurred by, or claims asserted against
+such Contributor by the fact You have accepted any warranty or additional
+liability.
+
+10. Acceptance of the Licence
+
+The provisions of this Licence can be accepted by clicking on an icon ‘I
+agree’ placed under the bottom of a window displaying the text of this Licence
+or by affirming consent in any other similar way, in accordance with the rules
+of applicable law. Clicking on that icon indicates your clear and irrevocable
+acceptance of this Licence and all of its terms and conditions.
+
+Similarly, you irrevocably accept this Licence and all of its terms and
+conditions by exercising any rights granted to You by Article 2 of this
+Licence, such as the use of the Work, the creation by You of a Derivative Work
+or the Distribution or Communication by You of the Work or copies thereof.
+
+11. Information to the public
+
+In case of any Distribution or Communication of the Work by means of
+electronic communication by You (for example, by offering to download the Work
+from a remote location) the distribution channel or media (for example, a
+website) must at least provide to the public the information requested by the
+applicable law regarding the Licensor, the Licence and the way it may be
+accessible, concluded, stored and reproduced by the Licensee.
+
+12. Termination of the Licence
+
+The Licence and the rights granted hereunder will terminate automatically upon
+any breach by the Licensee of the terms of the Licence.
+
+Such a termination will not terminate the licences of any person who has
+received the Work from the Licensee under the Licence, provided such persons
+remain in full compliance with the Licence.
+
+13. Miscellaneous
+
+Without prejudice of Article 9 above, the Licence represents the complete
+agreement between the Parties as to the Work.
+
+If any provision of the Licence is invalid or unenforceable under applicable
+law, this will not affect the validity or enforceability of the Licence as a
+whole. Such provision will be construed or reformed so as necessary to make it
+valid and enforceable.
+
+The European Commission may publish other linguistic versions or new versions
+of this Licence or updated versions of the Appendix, so far this is required
+and reasonable, without reducing the scope of the rights granted by the
+Licence. New versions of the Licence will be published with a unique version
+number.
+
+All linguistic versions of this Licence, approved by the European Commission,
+have identical value. Parties can take advantage of the linguistic version of
+their choice.
+
+14. Jurisdiction
+
+Without prejudice to specific agreement between parties,
+
+- any litigation resulting from the interpretation of this License, arising
+  between the European Union institutions, bodies, offices or agencies, as a
+  Licensor, and any Licensee, will be subject to the jurisdiction of the Court
+  of Justice of the European Union, as laid down in article 272 of the Treaty
+  on the Functioning of the European Union,
+
+- any litigation arising between other parties and resulting from the
+  interpretation of this License, will be subject to the exclusive
+  jurisdiction of the competent court where the Licensor resides or conducts
+  its primary business.
+
+15. Applicable Law
+
+Without prejudice to specific agreement between parties,
+
+- this Licence shall be governed by the law of the European Union Member State
+  where the Licensor has his seat, resides or has his registered office,
+
+- this licence shall be governed by Belgian law if the Licensor has no seat,
+  residence or registered office inside a European Union Member State.
+
+Appendix
+
+‘Compatible Licences’ according to Article 5 EUPL are:
+
+- GNU General Public License (GPL) v. 2, v. 3
+- GNU Affero General Public License (AGPL) v. 3
+- Open Software License (OSL) v. 2.1, v. 3.0
+- Eclipse Public License (EPL) v. 1.0
+- CeCILL v. 2.0, v. 2.1
+- Mozilla Public Licence (MPL) v. 2
+- GNU Lesser General Public Licence (LGPL) v. 2.1, v. 3
+- Creative Commons Attribution-ShareAlike v. 3.0 Unported (CC BY-SA 3.0) for
+  works other than software
+- European Union Public Licence (EUPL) v. 1.1, v. 1.2
+- Québec Free and Open-Source Licence — Reciprocity (LiLiQ-R) or Strong
+  Reciprocity (LiLiQ-R+).
+
+The European Commission may update this Appendix to later versions of the
+above licences without producing a new version of the EUPL, as long as they
+provide the rights granted in Article 2 of this Licence and protect the
+covered Source Code from exclusive appropriation.
+
+All other changes or additions to this Appendix require the production of a
+new EUPL version.
```

### Comparing `gref4hsi-0.2.1/PKG-INFO` & `gref4hsi-0.2.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,333 +1,289 @@
-Metadata-Version: 2.1
-Name: gref4hsi
-Version: 0.2.1
-Summary: A Python package for for georeferencing and orthorectifying hyperspectral imagery
-Home-page: https://github.com/havardlovas/gref4hsi
-Author: Haavard Snefjellaa Loevaas
-Author-email: havard.s.lovas@ntnu.no
-License: EUPL-1.2
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE.MD
-Requires-Dist: opencv-python
-Requires-Dist: dill
-Requires-Dist: geopandas
-Requires-Dist: h5py
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: open3d
-Requires-Dist: pandas
-Requires-Dist: Pillow
-Requires-Dist: pymap3d
-Requires-Dist: pyproj
-Requires-Dist: pyvista
-Requires-Dist: pyvistaqt
-Requires-Dist: scikit-learn
-Requires-Dist: scipy
-Requires-Dist: shapely
-Requires-Dist: spectral
-Requires-Dist: xmltodict
-Requires-Dist: pykdtree
-Requires-Dist: trimesh
-Requires-Dist: rtree
-Requires-Dist: embreex
-Requires-Dist: ephem
-
-# gref4hsi - a toolchain for the georeferencing and orthorectification of hyperspectral pushbroom data. 
-This software was made with a special emphasis on georeferencing and orthorectification of hyperspectral imagery from drones and underwater robots. However, it is equally simple to use for airborne data, and probably even for satellite imagery (although modified approaches including analytical ellipsoid intersection may be better). There is also a coregistration module (at beta stage) which, given an accurate RGB orthomosaic, can optimize geometric parameters (static or time-varying) to align the data.
-The functionality in bullet form is:
-* georeference.py: The software currently supports direct georeferencing through CPU-accelerated ray tracing of push broom measurements onto terrain files including 3D triangular meshes (\*.ply), 2.5D raster DEM/DSM (e.g. \*.tif) and geoid models.
-* orthorectification.py: The software performs orthorectification (a form of image resampling) to any user specified projection (by EPSG code) and resolution. The default resampling strategy is north-east oriented rasters, but the software does support memory-optimally oriented rasters (smallest bounding rectangle). When you resample, you essentially figure out where to put measurements in a geographic grid. In the software, we resample the data cube, an RGB composite of the cube, but also ancillary data like intersection/sun geometries, pixel coordinates (in spatial dimension of imager) and timestamps.
-* coregistration.py: Given a reference RGB orthomosaic (e.g. from photo-matching) covering the area of the hyperspectral image, the coregistration module does SIFT-matching with the RGB composite (handling any differences in projection and raster transforms). The module also has an optimization component for using the matches to minimize the reprojection error. The user can select/toggle which parameters to optimize, including boresight angles, lever arms, camera model parameters or time-varying errors in position/orientation. Notably the module requires that the pixel-coordinates and timestamps are resampled, as done automatically in the orthorectification step.
-
-This README is a bit verbose, but is meant to act as a "tutorial" as well, and I recommend trying to understand as much as possible.
-
-## Installation instructions for Linux:
-The easiest approach is to use conda/mamba to get gdal and pip to install the package with the following commands (has been tested for python 3.8-3.10):
-```
-conda create -n my_env python=3.10 gdal rasterio
-conda activate my_env
-pip install gref4hsi 
-```
-
-## Installation instructions for Windows:
-Seamless installation for windows is, to my experience a bit more challenging because of gdal and rasterio. For python 3.10 you could run
-```
-conda create -n my_env python=3.10
-conda activate my_env
-pip install GDAL‑3.4.3‑cp310‑cp310‑win_amd64.whl
-pip install rasterio‑1.2.10‑cp310‑cp310‑win_amd64.whl
-pip install gref4hsi 
-```
-The wheel files are provided at [Christoph Gohlke's page](https://www.lfd.uci.edu/~gohlke/pythonlibs/). Examples for python 3.8 are given in the dependencies folder of the Github repo.
-
-## Getting started:
-To run the code you will most likely need to re-format your raw acquired hyperspectral data and navigation data. To start with I'd recommend creating a top folder "<mission_dir>" (e.g. a folder "/processed" under your sensor-proprietary raw data). An example is shown below.
-
-```
-<mission_dir>/
-├── configuration.ini
-├── Input
-│   ├── Calib
-│   │   └── HSI_2b.xml
-│   └── H5
-│       ├── 2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
-│       ├── 2022-08-31_0800_HSI_transectnr_0_chunknr_1.h5
-│       ├── 2022-08-31_0800_HSI_transectnr_1_chunknr_0.h5
-```
-
-
-You minimally need the following to successfully run georeferencing: a configuration file ("\*.ini"), a terrain model, a camera model ("\*.xml") and h5/hdf file (datacube + navigation data). To appropriately format/create these, I recommend creating a parser. An example parser for a specim hyperspectral imager + navigation system is added under gref4hsi/utils/specim_parsing_utils.py
-
-### Configuration file ("\*.ini"). 
-It is recommended to just go with the template and maybe change a few minor things, depending on need. A template is given in the Github repo under data/config_examples/configuration_template.ini. The file contains comments describing the entries. Take a careful look at all comments containing "Change" as these are relevant to adjust depending on your setup. If your imager records h5 data, adjusting the h5 paths (sections 'HDF.xxxx') is relevant too. Morover, we interface with the configuration in a dictionary-style manner:
-
-```
-# Make an object and read the config file for the mission
-config = configparser.ConfigParser()
-config.read(config_file_mission)
-
-# Access a specific configuration, e.g. the calibrated camera model of the imager
-hsi_calib_path = config['Absolute Paths']['hsi_calib_path'] # config[<section>][<config-entry>]
-```
-
-
-### Calibration file ("\*.xml")
-The *.xml file is our chosen camera model file and looks like this:
-```
-<?xml version="1.0" encoding="utf-8"?>
-<calibration>
-    <rx>0.0</rx>
-    <ry>0.0</ry>
-    <rz>-1.5707963267948966</rz>
-    <tx>0</tx>
-    <ty>0</ty>
-    <tz>0</tz>
-    <f>754.9669285377008</f>
-    <cx>255.00991757530994</cx>
-    <k1>-72.31892156971124</k1>
-    <k2>-389.57799574674084</k2>
-    <k3>4.075384496065511</k3>
-    <width>512</width>
-</calibration>
-```
-rx, ry and rz are the boresight angles in radians, while tx, ty and tz are lever arms in the vehicle body frame. They are used to transform vectors from the HSI camera frame to the vehicle body frame through:
-```
-rot_hsi_ref_eul = np.array([rz, ry, rx])
-
-R = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False).as_matrix() # Rotation matrix from HSI to body
-
-t = np.array([tx, ty, tz])
-
-X_hsi = np.array([x, y, z]) # some vector
-
-X_body =  R*X_hsi + t# the vector expressed in the body frame 
-```
-In our computation we use a frame convention akin to the camera frames in computer vision. This means that x-right, y-backward, and z-downward for a well aligned camera. In contrast the vehicle body frame follows the roll-pitch-yaw convention with x-forward, y-starboard, z-downward. This is why the rz is by default $\pm \pi/2$. The easiest if you are unsure of whether your scanner is flipped is to swap the sign rz.
-
-
-
-Moreover, the f represent the camera's focal length in pixels, width is the number of spatial pixels, while cx is the principal pixel. Often cx=(width+1)/2, e.g. if you have 5 pixels u = 1,..,5 the middle pixel is cx=3. In other words, our convention is to assign the cell centres of pixels as whole integers (starting at 1), in contrast to OpenCV which starts at 0.5. The k1, k2 are radial distortion coefficients, while k3 is a tangential coefficient. The camera model is adapted from [Sun et al. (2016)](https://opg.optica.org/ao/fulltext.cfm?uri=ao-55-25-6836&id=348983). Expressing a pixel on an undistorted image plane in the HSI frame is done through
-```
-u = np.random.randint(1, width + 1) # Pixel numbers left to right (value from 1 to width)
-
-# Pinhole part
-x_norm_pinhole = (u - cx) / f
-
-# Distortion part
-x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
-                  k2 * ((u - cx) / 1000) ** 3 + \
-                  k3 * ((u - cx) / 1000) ** 2) / f
-
-x_norm_hsi = x_norm_pinhole + x_norm_nonlin
-
-X_norm_hsi = np.array([x_norm_hsi, 0, 1]) # The pixel ray in the hsi frame
-```
-
-Of course most of these parameters are hard to guess for a HSI and there are two simple ways of finding them. The first way is to ignore distortions and assume you know the angular field of view (AFOV). Then you can calculate:
-
-$$f = \frac{width}{2tan(AFOV/2)}$$
-
-
-Besides that, you set cx=width/2, and remaining k's to zero. 
-
-The second approach to get the camera model is if you have an array describing the FOV (often from the manufacturer). 
-In our example above that would amount to a 512-length array, e.g. in degrees 
-```
-from gref4hsi.specim_parsing_utils import Specim
-
-# FOV array from manufacturer describing the view angle of each pixel
-fov = np.array([-19.1, -19.0 .... 19.0, 19.1]) # Length as number of pixels
-
-# Use static method to convert fov to parameters dictionary equivalent to xml file (with boresights and lever arms to zero)
-param_dict = Specim.fov_2_param(fov = specim_object.view_angles)
-
-# Write to an *.xml file
-param_dict['rz'] = rx
-param_dict['ry'] = ry
-param_dict['rx'] = rz
-
-# Vector from origin of HSI to body origin, expressed in body
-# User set
-t_hsi_body = config_specim.translation_body_to_hsi
-param_dict['tz'] = tx
-param_dict['ty'] = ty
-param_dict['tz'] = tz
-
-# Write dictionary to *.xml file
-CalibHSI(file_name_cal_xml= confic['Absolute Paths']['hsi_calib_path'], 
-                    mode = 'w', 
-                    param_dict = param_dict)
-```
-
-
-
-### Terrain files
-There are three allowable types ("model_export_type" in the configuration file), namely "ply_file" (a.k.a. mesh files), "dem_file" and "geoid". Example geoids are added under data/world/geoids/ including the global egm08 and a norwegian geoid. Your local geoid can probably be found from [geoids](https://www.agisoft.com/downloads/geoids/) or similar. Just ensure you add this path to the 'Absolute Paths' section in the configuration file. Similarly, if you choose "model_export_type = dem_file", you can use a terrain model from from your area as long as you add the path to the file in the 'Absolute Paths'. Remember that if the local terrain (dem file) is given wrt the geoid, you can plus them together in e.g. QGIS or simply add an approximate offset in python with rasterio. This is because the software expects DEMs giving the ellipsoid height of the terrain. Lastly, if the "ply_file", or 3D triangular mesh is the desired option, a path to this file must be added to the config file. It should be fairly easy to use any triangular mesh format even though the option suggests "\*.ply". 
-
-### The h5 files
-This format must comply with the h5 paths in the configuration file. All sections starting with "HDF.xxxx" are related to these paths. I realize that it is inconvenient to transform the format if your recorded data is in NETCDF, ENVI etc, but making this software I chose H5/HDF because of legacy and because of the flexibility of the mini-file system. The input structure (only mandatory entries) of the H5 files under mission_dir/Input/H5 is as follows (printed using h5tree in Linux):  
-```
-2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
-├── processed
-│   └── radiance
-│       ├── calibration
-│       │   ├── geometric # Optional
-│       │   │   └── view_angles
-│       │   ├── radiometric # Only if is_radiance = False
-│       │   │   ├── darkFrame
-│       │   │   └── radiometricFrame
-│       │   └── spectral 
-│       │       ├── band2Wavelength
-│       │       └── fwhm # Optional
-│       ├── dataCube 
-│       ├── exposureTime
-│       └── timestamp
-└── raw
-    └── nav
-        ├── euler_angles
-        ├── position_ecef
-        └── timestamp
-```
-Note that all these paths are parameters in the config file and you will now we will explain how to simply fill in this file tree using the config file. An example of format conversion is given under gref4hsi/utils/specim_parsing_utils.py where the raw format of the specim data and a navigation system is converted and written to the h5 format. The following code is taken from that script and shows how you can write all the necessary data to the appropriate h5 format. Assume that "specim_object" represents an object whose attributes are the datasets, meaning that e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
-
-```
-def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
-    with h5py.File(h5_filename, 'w', libver='latest') as f:
-        for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
-            #print(attribute_name)
-            dset = f.create_dataset(name=h5_hierarchy_item_path, 
-                                            data = getattr(specim_object, attribute_name))
-
-h5_dict_write = {'eul_zyx' : config['HDF.raw_nav']['eul_zyx'],
-            'position_ecef' : config['HDF.raw_nav']['position'],
-            'nav_timestamp' : config['HDF.raw_nav']['timestamp'],
-            'radiance_cube': config['HDF.hyperspectral']['datacube'],
-            't_exp_ms': config['HDF.hyperspectral']['exposuretime'],
-            'hsi_timestamps': config['HDF.hyperspectral']['timestamp'],
-            'view_angles': config['HDF.calibration']['view_angles'], # Optional
-            'wavelengths' : config['HDF.calibration']['band2wavelength'],
-            'fwhm' : config['HDF.calibration']['fwhm'], # Optional
-            'dark_frame' : config['HDF.calibration']['darkframe'], # Optional unless 'is_radiance' is False
-            'radiometric_frame' : config['HDF.calibration']['radiometricframe']} # Optional unless 'is_radiance' is False
-
-# The dictionary is equivalent to the tree view above (assuming configuration_template.ini):
-h5_dict_write = {
-  'eul_zyx':            'raw/nav/euler_angles',
-  'position_ecef':     'raw/nav/position_ecef',
-  'nav_timestamp':     'raw/nav/timestamp',
-  'radiance_cube':    'processed/radiance/dataCube',
-  't_exp_ms':          'processed/radiance/exposureTime',
-  'hsi_timestamps':   'processed/radiance/timestamp',
-  'view_angles':       'processed/radiance/calibration/geometric/view_angles',
-  'wavelengths':       'processed/radiance/calibration/spectral/band2Wavelength',
-  'fwhm':              'processed/radiance/calibration/spectral/fwhm',
-  'dark_frame':        'processed/radiance/calibration/radiometric/darkFrame',
-  'radiometric_frame': 'processed/radiance/calibration/radiometric/radiometricFrame'
-}
-
-# At last, write the data to a h5 file
-# In this case 'specim_object' is an object whoose attributes correspond to the above keys
-# e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write  the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
-specim_object_2_h5_file(h5_filename=h5_filename, h5_tree_dict=h5_dict_write, specim_object=specim_object)
-```
-My recommended approach would be that you create your own modified xxx_parsing_utils.py (feel free to send a pull request) which parses and writes your specific navigation data and hyperspectral data into the format.
-
-The last thing worth mentioning is the navigation data. The aforementioned specim_parsing_utils.py parses navigation data from messages, e.g.
-
-Positions from 
-"$GPGGA,125301.00,6335.47830829,N,00932.34206055,E,2,07,1.7,18.434,M,41.216,M,4.0,0123\*79"
-
-Orientations/attitude from messages like
-"$PASHR,125648.280,322.905,T,0.621,-0.114,,0.034,0.034,0.450,2,3\*1B"
-
-The above data log is read with the method (in the case you have a similar navigation format)
-
-```
-specim_object.read_nav_file(nav_file_path=nav_file_path, date = date_string)
-```
-
-Lastly, the data should be formatted as follows for writing:
-
-```
-import pymap3d as pm
-
-# If your nav system gave you geodetic positions, convert them to earth centered earth fixed (ECEF). Make sure to use ellipsoid height (not height above mean sea level (MSL) aka geoid)
-x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
-
-# Roll pitch yaw are ordered with in an unintuitive attribute name eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
-specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
-
-# The ECEF positions
-specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
-```
-
-Then the "specim_object_2_h5_file" puts the data into the right place.
-
-## Running the processing
-Once the above has been defined the processing can be run with a few lines of code (taken from gref4hsi/tests/test_main_specim.py):
-```
-from gref4hsi.scripts import georeference
-from gref4hsi.scripts import orthorectification
-from gref4hsi.utils import parsing_utils, specim_parsing_utils
-from gref4hsi.scripts import visualize
-
-
-# This function parses raw specim data including (spectral, radiometric, geometric) calibrations and nav data
-# into an h5 file. The nav data is written to "raw/nav/" subfolders, whereas hyperspectral data and calibration data 
-# written to "processed/hyperspectral/" and "processed/calibration/" subfolders. The camera model \*.xml file is also generated.
-# The script must be adapted to other 
-specim_parsing_utils.main(config=config,
-                          config_specim=config_specim_preprocess)
-
-# Interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
-config = parsing_utils.export_pose(config_file_mission)
-
-# Exports model
-parsing_utils.export_model(config_file_mission)
-
-# Georeference the line scans of the hyperspectral imager. Utilizes parsed data
-georeference.main(config_file_mission)
-
-# Orthorectify/resample datacube, RGB-composite and ancillary data
-orthorectification.main(config_file_mission)
-
-# Optional: coregistration
-# Match RGB composite to reference, find features and following data, ground control point (gcp) list, for each feature pair:
-# reference point 3D (from reference), position/orientation of vehicle (using resampled time) and pixel coordinate (using resampled pixel coordinate)
-coregistration.main(config_file_mission, mode='compare')
-
-# The gcp list allows reprojecting reference points and evaluate the reprojection error,
-# which is used to optimize static geometric parameters (e.g. boresight...) or dynamic geometric parameters (time-varying nav errors).
-coregistration.main(config_file_mission, mode='calibrate')
-```
-
+# gref4hsi - a toolchain for the georeferencing and orthorectification of hyperspectral pushbroom data. 
+This software was made with a special emphasis on georeferencing and orthorectification of hyperspectral imagery from drones and underwater robots. However, it is equally simple to use for airborne data, and probably even for satellite imagery (although modified approaches including analytical ellipsoid intersection may be better). There is also a coregistration module (at beta stage) which, given an accurate RGB orthomosaic, can optimize geometric parameters (static or time-varying) to align the data.
+The functionality in bullet form is:
+* georeference.py: The software currently supports direct georeferencing through CPU-accelerated ray tracing of push broom measurements onto terrain files including 3D triangular meshes (\*.ply), 2.5D raster DEM/DSM (e.g. \*.tif) and geoid models.
+* orthorectification.py: The software performs orthorectification (a form of image resampling) to any user specified projection (by EPSG code) and resolution. The default resampling strategy is north-east oriented rasters, but the software does support memory-optimally oriented rasters (smallest bounding rectangle). When you resample, you essentially figure out where to put measurements in a geographic grid. In the software, we resample the data cube, an RGB composite of the cube, but also ancillary data like intersection/sun geometries, pixel coordinates (in spatial dimension of imager) and timestamps.
+* coregistration.py: Given a reference RGB orthomosaic (e.g. from photo-matching) covering the area of the hyperspectral image, the coregistration module does SIFT-matching with the RGB composite (handling any differences in projection and raster transforms). The module also has an optimization component for using the matches to minimize the reprojection error. The user can select/toggle which parameters to optimize, including boresight angles, lever arms, camera model parameters or time-varying errors in position/orientation. Notably the module requires that the pixel-coordinates and timestamps are resampled, as done automatically in the orthorectification step.
+
+This README is a bit verbose, but is meant to act as a "tutorial" as well, and I recommend trying to understand as much as possible.
+
+## Installation instructions for Linux:
+The easiest approach is to use conda/mamba to get gdal and pip to install the package with the following commands (has been tested for python 3.8-3.10):
+```
+conda create -n my_env python=3.10 gdal rasterio
+conda activate my_env
+pip install gref4hsi 
+```
+
+## Installation instructions for Windows:
+Seamless installation for windows is, to my experience a bit more challenging because of gdal and rasterio. For python 3.10 you could run
+```
+conda create -n my_env python=3.10
+conda activate my_env
+pip install GDAL‑3.4.3‑cp310‑cp310‑win_amd64.whl
+pip install rasterio‑1.2.10‑cp310‑cp310‑win_amd64.whl
+pip install gref4hsi 
+```
+The wheel files are provided at [Christoph Gohlke's page](https://www.lfd.uci.edu/~gohlke/pythonlibs/). Examples for python 3.8 are given in the dependencies folder of the Github repo.
+
+## Getting started:
+To run the code you will most likely need to re-format your raw acquired hyperspectral data and navigation data. To start with I'd recommend creating a top folder "<mission_dir>" (e.g. a folder "/processed" under your sensor-proprietary raw data). An example is shown below.
+
+```
+<mission_dir>/
+├── configuration.ini
+├── Input
+│   ├── Calib
+│   │   └── HSI_2b.xml
+│   └── H5
+│       ├── 2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
+│       ├── 2022-08-31_0800_HSI_transectnr_0_chunknr_1.h5
+│       ├── 2022-08-31_0800_HSI_transectnr_1_chunknr_0.h5
+```
+
+
+You minimally need the following to successfully run georeferencing: a configuration file ("\*.ini"), a terrain model, a camera model ("\*.xml") and h5/hdf file (datacube + navigation data). To appropriately format/create these, I recommend creating a parser. An example parser for a specim hyperspectral imager + navigation system is added under gref4hsi/utils/specim_parsing_utils.py
+
+### Configuration file ("\*.ini"). 
+It is recommended to just go with the template and maybe change a few minor things, depending on need. A template is given in the Github repo under data/config_examples/configuration_template.ini. The file contains comments describing the entries. Take a careful look at all comments containing "Change" as these are relevant to adjust depending on your setup. If your imager records h5 data, adjusting the h5 paths (sections 'HDF.xxxx') is relevant too. Morover, we interface with the configuration in a dictionary-style manner:
+
+```
+# Make an object and read the config file for the mission
+config = configparser.ConfigParser()
+config.read(config_file_mission)
+
+# Access a specific configuration, e.g. the calibrated camera model of the imager
+hsi_calib_path = config['Absolute Paths']['hsi_calib_path'] # config[<section>][<config-entry>]
+```
+
+
+### Calibration file ("\*.xml")
+The *.xml file is our chosen camera model file and looks like this:
+```
+<?xml version="1.0" encoding="utf-8"?>
+<calibration>
+    <rx>0.0</rx>
+    <ry>0.0</ry>
+    <rz>-1.5707963267948966</rz>
+    <tx>0</tx>
+    <ty>0</ty>
+    <tz>0</tz>
+    <f>754.9669285377008</f>
+    <cx>255.00991757530994</cx>
+    <k1>-72.31892156971124</k1>
+    <k2>-389.57799574674084</k2>
+    <k3>4.075384496065511</k3>
+    <width>512</width>
+</calibration>
+```
+rx, ry and rz are the boresight angles in radians, while tx, ty and tz are lever arms in the vehicle body frame. They are used to transform vectors from the HSI camera frame to the vehicle body frame through:
+```
+rot_hsi_ref_eul = np.array([rz, ry, rx])
+
+R = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False).as_matrix() # Rotation matrix from HSI to body
+
+t = np.array([tx, ty, tz])
+
+X_hsi = np.array([x, y, z]) # some vector
+
+X_body =  R*X_hsi + t# the vector expressed in the body frame 
+```
+In our computation we use a frame convention akin to the camera frames in computer vision. This means that x-right, y-backward, and z-downward for a well aligned camera. In contrast the vehicle body frame follows the roll-pitch-yaw convention with x-forward, y-starboard, z-downward. This is why the rz is by default $\pm \pi/2$. The easiest if you are unsure of whether your scanner is flipped is to swap the sign rz.
+
+
+
+Moreover, the f represent the camera's focal length in pixels, width is the number of spatial pixels, while cx is the principal pixel. Often cx=(width+1)/2, e.g. if you have 5 pixels u = 1,..,5 the middle pixel is cx=3. In other words, our convention is to assign the cell centres of pixels as whole integers (starting at 1), in contrast to OpenCV which starts at 0.5. The k1, k2 are radial distortion coefficients, while k3 is a tangential coefficient. The camera model is adapted from [Sun et al. (2016)](https://opg.optica.org/ao/fulltext.cfm?uri=ao-55-25-6836&id=348983). Expressing a pixel on an undistorted image plane in the HSI frame is done through
+```
+u = np.random.randint(1, width + 1) # Pixel numbers left to right (value from 1 to width)
+
+# Pinhole part
+x_norm_pinhole = (u - cx) / f
+
+# Distortion part
+x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
+                  k2 * ((u - cx) / 1000) ** 3 + \
+                  k3 * ((u - cx) / 1000) ** 2) / f
+
+x_norm_hsi = x_norm_pinhole + x_norm_nonlin
+
+X_norm_hsi = np.array([x_norm_hsi, 0, 1]) # The pixel ray in the hsi frame
+```
+
+Of course most of these parameters are hard to guess for a HSI and there are two simple ways of finding them. The first way is to ignore distortions and assume you know the angular field of view (AFOV). Then you can calculate:
+
+$$f = \frac{width}{2tan(AFOV/2)}$$
+
+
+Besides that, you set cx=width/2, and remaining k's to zero. 
+
+The second approach to get the camera model is if you have an array describing the FOV (often from the manufacturer). 
+In our example above that would amount to a 512-length array, e.g. in degrees 
+```
+from gref4hsi.specim_parsing_utils import Specim
+
+# FOV array from manufacturer describing the view angle of each pixel
+fov = np.array([-19.1, -19.0 .... 19.0, 19.1]) # Length as number of pixels
+
+# Use static method to convert fov to parameters dictionary equivalent to xml file (with boresights and lever arms to zero)
+param_dict = Specim.fov_2_param(fov = specim_object.view_angles)
+
+# Write to an *.xml file
+param_dict['rz'] = rx
+param_dict['ry'] = ry
+param_dict['rx'] = rz
+
+# Vector from origin of HSI to body origin, expressed in body
+# User set
+t_hsi_body = config_specim.translation_body_to_hsi
+param_dict['tz'] = tx
+param_dict['ty'] = ty
+param_dict['tz'] = tz
+
+# Write dictionary to *.xml file
+CalibHSI(file_name_cal_xml= confic['Absolute Paths']['hsi_calib_path'], 
+                    mode = 'w', 
+                    param_dict = param_dict)
+```
+
+
+
+### Terrain files
+There are three allowable types ("model_export_type" in the configuration file), namely "ply_file" (a.k.a. mesh files), "dem_file" and "geoid". Example geoids are added under data/world/geoids/ including the global egm08 and a norwegian geoid. Your local geoid can probably be found from [geoids](https://www.agisoft.com/downloads/geoids/) or similar. Just ensure you add this path to the 'Absolute Paths' section in the configuration file. Similarly, if you choose "model_export_type = dem_file", you can use a terrain model from from your area as long as you add the path to the file in the 'Absolute Paths'. Remember that if the local terrain (dem file) is given wrt the geoid, you can plus them together in e.g. QGIS or simply add an approximate offset in python with rasterio. This is because the software expects DEMs giving the ellipsoid height of the terrain. Lastly, if the "ply_file", or 3D triangular mesh is the desired option, a path to this file must be added to the config file. It should be fairly easy to use any triangular mesh format even though the option suggests "\*.ply". 
+
+### The h5 files
+This format must comply with the h5 paths in the configuration file. All sections starting with "HDF.xxxx" are related to these paths. I realize that it is inconvenient to transform the format if your recorded data is in NETCDF, ENVI etc, but making this software I chose H5/HDF because of legacy and because of the flexibility of the mini-file system. The input structure (only mandatory entries) of the H5 files under mission_dir/Input/H5 is as follows (printed using h5tree in Linux):  
+```
+2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
+├── processed
+│   └── radiance
+│       ├── calibration
+│       │   ├── geometric # Optional
+│       │   │   └── view_angles
+│       │   ├── radiometric # Only if is_radiance = False
+│       │   │   ├── darkFrame
+│       │   │   └── radiometricFrame
+│       │   └── spectral 
+│       │       ├── band2Wavelength
+│       │       └── fwhm # Optional
+│       ├── dataCube 
+│       ├── exposureTime
+│       └── timestamp
+└── raw
+    └── nav
+        ├── euler_angles
+        ├── position_ecef
+        └── timestamp
+```
+Note that all these paths are parameters in the config file and you will now we will explain how to simply fill in this file tree using the config file. An example of format conversion is given under gref4hsi/utils/specim_parsing_utils.py where the raw format of the specim data and a navigation system is converted and written to the h5 format. The following code is taken from that script and shows how you can write all the necessary data to the appropriate h5 format. Assume that "specim_object" represents an object whose attributes are the datasets, meaning that e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
+
+```
+def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
+    with h5py.File(h5_filename, 'w', libver='latest') as f:
+        for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
+            #print(attribute_name)
+            dset = f.create_dataset(name=h5_hierarchy_item_path, 
+                                            data = getattr(specim_object, attribute_name))
+
+h5_dict_write = {'eul_zyx' : config['HDF.raw_nav']['eul_zyx'],
+            'position_ecef' : config['HDF.raw_nav']['position'],
+            'nav_timestamp' : config['HDF.raw_nav']['timestamp'],
+            'radiance_cube': config['HDF.hyperspectral']['datacube'],
+            't_exp_ms': config['HDF.hyperspectral']['exposuretime'],
+            'hsi_timestamps': config['HDF.hyperspectral']['timestamp'],
+            'view_angles': config['HDF.calibration']['view_angles'], # Optional
+            'wavelengths' : config['HDF.calibration']['band2wavelength'],
+            'fwhm' : config['HDF.calibration']['fwhm'], # Optional
+            'dark_frame' : config['HDF.calibration']['darkframe'], # Optional unless 'is_radiance' is False
+            'radiometric_frame' : config['HDF.calibration']['radiometricframe']} # Optional unless 'is_radiance' is False
+
+# The dictionary is equivalent to the tree view above (assuming configuration_template.ini):
+h5_dict_write = {
+  'eul_zyx':            'raw/nav/euler_angles',
+  'position_ecef':     'raw/nav/position_ecef',
+  'nav_timestamp':     'raw/nav/timestamp',
+  'radiance_cube':    'processed/radiance/dataCube',
+  't_exp_ms':          'processed/radiance/exposureTime',
+  'hsi_timestamps':   'processed/radiance/timestamp',
+  'view_angles':       'processed/radiance/calibration/geometric/view_angles',
+  'wavelengths':       'processed/radiance/calibration/spectral/band2Wavelength',
+  'fwhm':              'processed/radiance/calibration/spectral/fwhm',
+  'dark_frame':        'processed/radiance/calibration/radiometric/darkFrame',
+  'radiometric_frame': 'processed/radiance/calibration/radiometric/radiometricFrame'
+}
+
+# At last, write the data to a h5 file
+# In this case 'specim_object' is an object whoose attributes correspond to the above keys
+# e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write  the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
+specim_object_2_h5_file(h5_filename=h5_filename, h5_tree_dict=h5_dict_write, specim_object=specim_object)
+```
+My recommended approach would be that you create your own modified xxx_parsing_utils.py (feel free to send a pull request) which parses and writes your specific navigation data and hyperspectral data into the format.
+
+The last thing worth mentioning is the navigation data. The aforementioned specim_parsing_utils.py parses navigation data from messages, e.g.
+
+Positions from 
+"$GPGGA,125301.00,6335.47830829,N,00932.34206055,E,2,07,1.7,18.434,M,41.216,M,4.0,0123\*79"
+
+Orientations/attitude from messages like
+"$PASHR,125648.280,322.905,T,0.621,-0.114,,0.034,0.034,0.450,2,3\*1B"
+
+The above data log is read with the method (in the case you have a similar navigation format)
+
+```
+specim_object.read_nav_file(nav_file_path=nav_file_path, date = date_string)
+```
+
+Lastly, the data should be formatted as follows for writing:
+
+```
+import pymap3d as pm
+
+# If your nav system gave you geodetic positions, convert them to earth centered earth fixed (ECEF). Make sure to use ellipsoid height (not height above mean sea level (MSL) aka geoid)
+x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
+
+# Roll pitch yaw are ordered with in an unintuitive attribute name eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
+specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
+
+# The ECEF positions
+specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
+```
+
+Then the "specim_object_2_h5_file" puts the data into the right place.
+
+## Running the processing
+Once the above has been defined the processing can be run with a few lines of code (taken from gref4hsi/tests/test_main_specim.py):
+```
+from gref4hsi.scripts import georeference
+from gref4hsi.scripts import orthorectification
+from gref4hsi.utils import parsing_utils, specim_parsing_utils
+from gref4hsi.scripts import visualize
+
+
+# This function parses raw specim data including (spectral, radiometric, geometric) calibrations and nav data
+# into an h5 file. The nav data is written to "raw/nav/" subfolders, whereas hyperspectral data and calibration data 
+# written to "processed/hyperspectral/" and "processed/calibration/" subfolders. The camera model \*.xml file is also generated.
+# The script must be adapted to other 
+specim_parsing_utils.main(config=config,
+                          config_specim=config_specim_preprocess)
+
+# Interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
+config = parsing_utils.export_pose(config_file_mission)
+
+# Exports model
+parsing_utils.export_model(config_file_mission)
+
+# Georeference the line scans of the hyperspectral imager. Utilizes parsed data
+georeference.main(config_file_mission)
+
+# Orthorectify/resample datacube, RGB-composite and ancillary data
+orthorectification.main(config_file_mission)
+
+# Optional: coregistration
+# Match RGB composite to reference, find features and following data, ground control point (gcp) list, for each feature pair:
+# reference point 3D (from reference), position/orientation of vehicle (using resampled time) and pixel coordinate (using resampled pixel coordinate)
+coregistration.main(config_file_mission, mode='compare')
+
+# The gcp list allows reprojecting reference points and evaluate the reprojection error,
+# which is used to optimize static geometric parameters (e.g. boresight...) or dynamic geometric parameters (time-varying nav errors).
+coregistration.main(config_file_mission, mode='calibrate')
+```
+
```

### Comparing `gref4hsi-0.2.1/README.md` & `gref4hsi-0.2.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,289 +1,333 @@
-# gref4hsi - a toolchain for the georeferencing and orthorectification of hyperspectral pushbroom data. 
-This software was made with a special emphasis on georeferencing and orthorectification of hyperspectral imagery from drones and underwater robots. However, it is equally simple to use for airborne data, and probably even for satellite imagery (although modified approaches including analytical ellipsoid intersection may be better). There is also a coregistration module (at beta stage) which, given an accurate RGB orthomosaic, can optimize geometric parameters (static or time-varying) to align the data.
-The functionality in bullet form is:
-* georeference.py: The software currently supports direct georeferencing through CPU-accelerated ray tracing of push broom measurements onto terrain files including 3D triangular meshes (\*.ply), 2.5D raster DEM/DSM (e.g. \*.tif) and geoid models.
-* orthorectification.py: The software performs orthorectification (a form of image resampling) to any user specified projection (by EPSG code) and resolution. The default resampling strategy is north-east oriented rasters, but the software does support memory-optimally oriented rasters (smallest bounding rectangle). When you resample, you essentially figure out where to put measurements in a geographic grid. In the software, we resample the data cube, an RGB composite of the cube, but also ancillary data like intersection/sun geometries, pixel coordinates (in spatial dimension of imager) and timestamps.
-* coregistration.py: Given a reference RGB orthomosaic (e.g. from photo-matching) covering the area of the hyperspectral image, the coregistration module does SIFT-matching with the RGB composite (handling any differences in projection and raster transforms). The module also has an optimization component for using the matches to minimize the reprojection error. The user can select/toggle which parameters to optimize, including boresight angles, lever arms, camera model parameters or time-varying errors in position/orientation. Notably the module requires that the pixel-coordinates and timestamps are resampled, as done automatically in the orthorectification step.
-
-This README is a bit verbose, but is meant to act as a "tutorial" as well, and I recommend trying to understand as much as possible.
-
-## Installation instructions for Linux:
-The easiest approach is to use conda/mamba to get gdal and pip to install the package with the following commands (has been tested for python 3.8-3.10):
-```
-conda create -n my_env python=3.10 gdal rasterio
-conda activate my_env
-pip install gref4hsi 
-```
-
-## Installation instructions for Windows:
-Seamless installation for windows is, to my experience a bit more challenging because of gdal and rasterio. For python 3.10 you could run
-```
-conda create -n my_env python=3.10
-conda activate my_env
-pip install GDAL‑3.4.3‑cp310‑cp310‑win_amd64.whl
-pip install rasterio‑1.2.10‑cp310‑cp310‑win_amd64.whl
-pip install gref4hsi 
-```
-The wheel files are provided at [Christoph Gohlke's page](https://www.lfd.uci.edu/~gohlke/pythonlibs/). Examples for python 3.8 are given in the dependencies folder of the Github repo.
-
-## Getting started:
-To run the code you will most likely need to re-format your raw acquired hyperspectral data and navigation data. To start with I'd recommend creating a top folder "<mission_dir>" (e.g. a folder "/processed" under your sensor-proprietary raw data). An example is shown below.
-
-```
-<mission_dir>/
-├── configuration.ini
-├── Input
-│   ├── Calib
-│   │   └── HSI_2b.xml
-│   └── H5
-│       ├── 2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
-│       ├── 2022-08-31_0800_HSI_transectnr_0_chunknr_1.h5
-│       ├── 2022-08-31_0800_HSI_transectnr_1_chunknr_0.h5
-```
-
-
-You minimally need the following to successfully run georeferencing: a configuration file ("\*.ini"), a terrain model, a camera model ("\*.xml") and h5/hdf file (datacube + navigation data). To appropriately format/create these, I recommend creating a parser. An example parser for a specim hyperspectral imager + navigation system is added under gref4hsi/utils/specim_parsing_utils.py
-
-### Configuration file ("\*.ini"). 
-It is recommended to just go with the template and maybe change a few minor things, depending on need. A template is given in the Github repo under data/config_examples/configuration_template.ini. The file contains comments describing the entries. Take a careful look at all comments containing "Change" as these are relevant to adjust depending on your setup. If your imager records h5 data, adjusting the h5 paths (sections 'HDF.xxxx') is relevant too. Morover, we interface with the configuration in a dictionary-style manner:
-
-```
-# Make an object and read the config file for the mission
-config = configparser.ConfigParser()
-config.read(config_file_mission)
-
-# Access a specific configuration, e.g. the calibrated camera model of the imager
-hsi_calib_path = config['Absolute Paths']['hsi_calib_path'] # config[<section>][<config-entry>]
-```
-
-
-### Calibration file ("\*.xml")
-The *.xml file is our chosen camera model file and looks like this:
-```
-<?xml version="1.0" encoding="utf-8"?>
-<calibration>
-    <rx>0.0</rx>
-    <ry>0.0</ry>
-    <rz>-1.5707963267948966</rz>
-    <tx>0</tx>
-    <ty>0</ty>
-    <tz>0</tz>
-    <f>754.9669285377008</f>
-    <cx>255.00991757530994</cx>
-    <k1>-72.31892156971124</k1>
-    <k2>-389.57799574674084</k2>
-    <k3>4.075384496065511</k3>
-    <width>512</width>
-</calibration>
-```
-rx, ry and rz are the boresight angles in radians, while tx, ty and tz are lever arms in the vehicle body frame. They are used to transform vectors from the HSI camera frame to the vehicle body frame through:
-```
-rot_hsi_ref_eul = np.array([rz, ry, rx])
-
-R = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False).as_matrix() # Rotation matrix from HSI to body
-
-t = np.array([tx, ty, tz])
-
-X_hsi = np.array([x, y, z]) # some vector
-
-X_body =  R*X_hsi + t# the vector expressed in the body frame 
-```
-In our computation we use a frame convention akin to the camera frames in computer vision. This means that x-right, y-backward, and z-downward for a well aligned camera. In contrast the vehicle body frame follows the roll-pitch-yaw convention with x-forward, y-starboard, z-downward. This is why the rz is by default $\pm \pi/2$. The easiest if you are unsure of whether your scanner is flipped is to swap the sign rz.
-
-
-
-Moreover, the f represent the camera's focal length in pixels, width is the number of spatial pixels, while cx is the principal pixel. Often cx=(width+1)/2, e.g. if you have 5 pixels u = 1,..,5 the middle pixel is cx=3. In other words, our convention is to assign the cell centres of pixels as whole integers (starting at 1), in contrast to OpenCV which starts at 0.5. The k1, k2 are radial distortion coefficients, while k3 is a tangential coefficient. The camera model is adapted from [Sun et al. (2016)](https://opg.optica.org/ao/fulltext.cfm?uri=ao-55-25-6836&id=348983). Expressing a pixel on an undistorted image plane in the HSI frame is done through
-```
-u = np.random.randint(1, width + 1) # Pixel numbers left to right (value from 1 to width)
-
-# Pinhole part
-x_norm_pinhole = (u - cx) / f
-
-# Distortion part
-x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
-                  k2 * ((u - cx) / 1000) ** 3 + \
-                  k3 * ((u - cx) / 1000) ** 2) / f
-
-x_norm_hsi = x_norm_pinhole + x_norm_nonlin
-
-X_norm_hsi = np.array([x_norm_hsi, 0, 1]) # The pixel ray in the hsi frame
-```
-
-Of course most of these parameters are hard to guess for a HSI and there are two simple ways of finding them. The first way is to ignore distortions and assume you know the angular field of view (AFOV). Then you can calculate:
-
-$$f = \frac{width}{2tan(AFOV/2)}$$
-
-
-Besides that, you set cx=width/2, and remaining k's to zero. 
-
-The second approach to get the camera model is if you have an array describing the FOV (often from the manufacturer). 
-In our example above that would amount to a 512-length array, e.g. in degrees 
-```
-from gref4hsi.specim_parsing_utils import Specim
-
-# FOV array from manufacturer describing the view angle of each pixel
-fov = np.array([-19.1, -19.0 .... 19.0, 19.1]) # Length as number of pixels
-
-# Use static method to convert fov to parameters dictionary equivalent to xml file (with boresights and lever arms to zero)
-param_dict = Specim.fov_2_param(fov = specim_object.view_angles)
-
-# Write to an *.xml file
-param_dict['rz'] = rx
-param_dict['ry'] = ry
-param_dict['rx'] = rz
-
-# Vector from origin of HSI to body origin, expressed in body
-# User set
-t_hsi_body = config_specim.translation_body_to_hsi
-param_dict['tz'] = tx
-param_dict['ty'] = ty
-param_dict['tz'] = tz
-
-# Write dictionary to *.xml file
-CalibHSI(file_name_cal_xml= confic['Absolute Paths']['hsi_calib_path'], 
-                    mode = 'w', 
-                    param_dict = param_dict)
-```
-
-
-
-### Terrain files
-There are three allowable types ("model_export_type" in the configuration file), namely "ply_file" (a.k.a. mesh files), "dem_file" and "geoid". Example geoids are added under data/world/geoids/ including the global egm08 and a norwegian geoid. Your local geoid can probably be found from [geoids](https://www.agisoft.com/downloads/geoids/) or similar. Just ensure you add this path to the 'Absolute Paths' section in the configuration file. Similarly, if you choose "model_export_type = dem_file", you can use a terrain model from from your area as long as you add the path to the file in the 'Absolute Paths'. Remember that if the local terrain (dem file) is given wrt the geoid, you can plus them together in e.g. QGIS or simply add an approximate offset in python with rasterio. This is because the software expects DEMs giving the ellipsoid height of the terrain. Lastly, if the "ply_file", or 3D triangular mesh is the desired option, a path to this file must be added to the config file. It should be fairly easy to use any triangular mesh format even though the option suggests "\*.ply". 
-
-### The h5 files
-This format must comply with the h5 paths in the configuration file. All sections starting with "HDF.xxxx" are related to these paths. I realize that it is inconvenient to transform the format if your recorded data is in NETCDF, ENVI etc, but making this software I chose H5/HDF because of legacy and because of the flexibility of the mini-file system. The input structure (only mandatory entries) of the H5 files under mission_dir/Input/H5 is as follows (printed using h5tree in Linux):  
-```
-2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
-├── processed
-│   └── radiance
-│       ├── calibration
-│       │   ├── geometric # Optional
-│       │   │   └── view_angles
-│       │   ├── radiometric # Only if is_radiance = False
-│       │   │   ├── darkFrame
-│       │   │   └── radiometricFrame
-│       │   └── spectral 
-│       │       ├── band2Wavelength
-│       │       └── fwhm # Optional
-│       ├── dataCube 
-│       ├── exposureTime
-│       └── timestamp
-└── raw
-    └── nav
-        ├── euler_angles
-        ├── position_ecef
-        └── timestamp
-```
-Note that all these paths are parameters in the config file and you will now we will explain how to simply fill in this file tree using the config file. An example of format conversion is given under gref4hsi/utils/specim_parsing_utils.py where the raw format of the specim data and a navigation system is converted and written to the h5 format. The following code is taken from that script and shows how you can write all the necessary data to the appropriate h5 format. Assume that "specim_object" represents an object whose attributes are the datasets, meaning that e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
-
-```
-def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
-    with h5py.File(h5_filename, 'w', libver='latest') as f:
-        for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
-            #print(attribute_name)
-            dset = f.create_dataset(name=h5_hierarchy_item_path, 
-                                            data = getattr(specim_object, attribute_name))
-
-h5_dict_write = {'eul_zyx' : config['HDF.raw_nav']['eul_zyx'],
-            'position_ecef' : config['HDF.raw_nav']['position'],
-            'nav_timestamp' : config['HDF.raw_nav']['timestamp'],
-            'radiance_cube': config['HDF.hyperspectral']['datacube'],
-            't_exp_ms': config['HDF.hyperspectral']['exposuretime'],
-            'hsi_timestamps': config['HDF.hyperspectral']['timestamp'],
-            'view_angles': config['HDF.calibration']['view_angles'], # Optional
-            'wavelengths' : config['HDF.calibration']['band2wavelength'],
-            'fwhm' : config['HDF.calibration']['fwhm'], # Optional
-            'dark_frame' : config['HDF.calibration']['darkframe'], # Optional unless 'is_radiance' is False
-            'radiometric_frame' : config['HDF.calibration']['radiometricframe']} # Optional unless 'is_radiance' is False
-
-# The dictionary is equivalent to the tree view above (assuming configuration_template.ini):
-h5_dict_write = {
-  'eul_zyx':            'raw/nav/euler_angles',
-  'position_ecef':     'raw/nav/position_ecef',
-  'nav_timestamp':     'raw/nav/timestamp',
-  'radiance_cube':    'processed/radiance/dataCube',
-  't_exp_ms':          'processed/radiance/exposureTime',
-  'hsi_timestamps':   'processed/radiance/timestamp',
-  'view_angles':       'processed/radiance/calibration/geometric/view_angles',
-  'wavelengths':       'processed/radiance/calibration/spectral/band2Wavelength',
-  'fwhm':              'processed/radiance/calibration/spectral/fwhm',
-  'dark_frame':        'processed/radiance/calibration/radiometric/darkFrame',
-  'radiometric_frame': 'processed/radiance/calibration/radiometric/radiometricFrame'
-}
-
-# At last, write the data to a h5 file
-# In this case 'specim_object' is an object whoose attributes correspond to the above keys
-# e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write  the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
-specim_object_2_h5_file(h5_filename=h5_filename, h5_tree_dict=h5_dict_write, specim_object=specim_object)
-```
-My recommended approach would be that you create your own modified xxx_parsing_utils.py (feel free to send a pull request) which parses and writes your specific navigation data and hyperspectral data into the format.
-
-The last thing worth mentioning is the navigation data. The aforementioned specim_parsing_utils.py parses navigation data from messages, e.g.
-
-Positions from 
-"$GPGGA,125301.00,6335.47830829,N,00932.34206055,E,2,07,1.7,18.434,M,41.216,M,4.0,0123\*79"
-
-Orientations/attitude from messages like
-"$PASHR,125648.280,322.905,T,0.621,-0.114,,0.034,0.034,0.450,2,3\*1B"
-
-The above data log is read with the method (in the case you have a similar navigation format)
-
-```
-specim_object.read_nav_file(nav_file_path=nav_file_path, date = date_string)
-```
-
-Lastly, the data should be formatted as follows for writing:
-
-```
-import pymap3d as pm
-
-# If your nav system gave you geodetic positions, convert them to earth centered earth fixed (ECEF). Make sure to use ellipsoid height (not height above mean sea level (MSL) aka geoid)
-x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
-
-# Roll pitch yaw are ordered with in an unintuitive attribute name eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
-specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
-
-# The ECEF positions
-specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
-```
-
-Then the "specim_object_2_h5_file" puts the data into the right place.
-
-## Running the processing
-Once the above has been defined the processing can be run with a few lines of code (taken from gref4hsi/tests/test_main_specim.py):
-```
-from gref4hsi.scripts import georeference
-from gref4hsi.scripts import orthorectification
-from gref4hsi.utils import parsing_utils, specim_parsing_utils
-from gref4hsi.scripts import visualize
-
-
-# This function parses raw specim data including (spectral, radiometric, geometric) calibrations and nav data
-# into an h5 file. The nav data is written to "raw/nav/" subfolders, whereas hyperspectral data and calibration data 
-# written to "processed/hyperspectral/" and "processed/calibration/" subfolders. The camera model \*.xml file is also generated.
-# The script must be adapted to other 
-specim_parsing_utils.main(config=config,
-                          config_specim=config_specim_preprocess)
-
-# Interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
-config = parsing_utils.export_pose(config_file_mission)
-
-# Exports model
-parsing_utils.export_model(config_file_mission)
-
-# Georeference the line scans of the hyperspectral imager. Utilizes parsed data
-georeference.main(config_file_mission)
-
-# Orthorectify/resample datacube, RGB-composite and ancillary data
-orthorectification.main(config_file_mission)
-
-# Optional: coregistration
-# Match RGB composite to reference, find features and following data, ground control point (gcp) list, for each feature pair:
-# reference point 3D (from reference), position/orientation of vehicle (using resampled time) and pixel coordinate (using resampled pixel coordinate)
-coregistration.main(config_file_mission, mode='compare')
-
-# The gcp list allows reprojecting reference points and evaluate the reprojection error,
-# which is used to optimize static geometric parameters (e.g. boresight...) or dynamic geometric parameters (time-varying nav errors).
-coregistration.main(config_file_mission, mode='calibrate')
-```
-
+Metadata-Version: 2.1
+Name: gref4hsi
+Version: 0.2.2
+Summary: A Python package for for georeferencing and orthorectifying hyperspectral imagery
+Home-page: https://github.com/havardlovas/gref4hsi
+Author: Haavard Snefjellaa Loevaas
+Author-email: havard.s.lovas@ntnu.no
+License: EUPL-1.2
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE.MD
+Requires-Dist: opencv-python
+Requires-Dist: dill
+Requires-Dist: geopandas
+Requires-Dist: h5py
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: open3d
+Requires-Dist: pandas
+Requires-Dist: Pillow
+Requires-Dist: pymap3d
+Requires-Dist: pyproj
+Requires-Dist: pyvista
+Requires-Dist: pyvistaqt
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: shapely
+Requires-Dist: spectral
+Requires-Dist: xmltodict
+Requires-Dist: pykdtree
+Requires-Dist: trimesh
+Requires-Dist: rtree
+Requires-Dist: embreex
+Requires-Dist: ephem
+
+# gref4hsi - a toolchain for the georeferencing and orthorectification of hyperspectral pushbroom data. 
+This software was made with a special emphasis on georeferencing and orthorectification of hyperspectral imagery from drones and underwater robots. However, it is equally simple to use for airborne data, and probably even for satellite imagery (although modified approaches including analytical ellipsoid intersection may be better). There is also a coregistration module (at beta stage) which, given an accurate RGB orthomosaic, can optimize geometric parameters (static or time-varying) to align the data.
+The functionality in bullet form is:
+* georeference.py: The software currently supports direct georeferencing through CPU-accelerated ray tracing of push broom measurements onto terrain files including 3D triangular meshes (\*.ply), 2.5D raster DEM/DSM (e.g. \*.tif) and geoid models.
+* orthorectification.py: The software performs orthorectification (a form of image resampling) to any user specified projection (by EPSG code) and resolution. The default resampling strategy is north-east oriented rasters, but the software does support memory-optimally oriented rasters (smallest bounding rectangle). When you resample, you essentially figure out where to put measurements in a geographic grid. In the software, we resample the data cube, an RGB composite of the cube, but also ancillary data like intersection/sun geometries, pixel coordinates (in spatial dimension of imager) and timestamps.
+* coregistration.py: Given a reference RGB orthomosaic (e.g. from photo-matching) covering the area of the hyperspectral image, the coregistration module does SIFT-matching with the RGB composite (handling any differences in projection and raster transforms). The module also has an optimization component for using the matches to minimize the reprojection error. The user can select/toggle which parameters to optimize, including boresight angles, lever arms, camera model parameters or time-varying errors in position/orientation. Notably the module requires that the pixel-coordinates and timestamps are resampled, as done automatically in the orthorectification step.
+
+This README is a bit verbose, but is meant to act as a "tutorial" as well, and I recommend trying to understand as much as possible.
+
+## Installation instructions for Linux:
+The easiest approach is to use conda/mamba to get gdal and pip to install the package with the following commands (has been tested for python 3.8-3.10):
+```
+conda create -n my_env python=3.10 gdal rasterio
+conda activate my_env
+pip install gref4hsi 
+```
+
+## Installation instructions for Windows:
+Seamless installation for windows is, to my experience a bit more challenging because of gdal and rasterio. For python 3.10 you could run
+```
+conda create -n my_env python=3.10
+conda activate my_env
+pip install GDALâ€‘3.4.3â€‘cp310â€‘cp310â€‘win_amd64.whl
+pip install rasterioâ€‘1.2.10â€‘cp310â€‘cp310â€‘win_amd64.whl
+pip install gref4hsi 
+```
+The wheel files are provided at [Christoph Gohlke's page](https://www.lfd.uci.edu/~gohlke/pythonlibs/). Examples for python 3.8 are given in the dependencies folder of the Github repo.
+
+## Getting started:
+To run the code you will most likely need to re-format your raw acquired hyperspectral data and navigation data. To start with I'd recommend creating a top folder "<mission_dir>" (e.g. a folder "/processed" under your sensor-proprietary raw data). An example is shown below.
+
+```
+<mission_dir>/
+â”œâ”€â”€ configuration.ini
+â”œâ”€â”€ Input
+â”‚Â Â  â”œâ”€â”€ Calib
+â”‚Â Â  â”‚Â Â  â””â”€â”€ HSI_2b.xml
+â”‚Â Â  â””â”€â”€ H5
+â”‚Â Â      â”œâ”€â”€ 2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
+â”‚Â Â      â”œâ”€â”€ 2022-08-31_0800_HSI_transectnr_0_chunknr_1.h5
+â”‚Â Â      â”œâ”€â”€ 2022-08-31_0800_HSI_transectnr_1_chunknr_0.h5
+```
+
+
+You minimally need the following to successfully run georeferencing: a configuration file ("\*.ini"), a terrain model, a camera model ("\*.xml") and h5/hdf file (datacube + navigation data). To appropriately format/create these, I recommend creating a parser. An example parser for a specim hyperspectral imager + navigation system is added under gref4hsi/utils/specim_parsing_utils.py
+
+### Configuration file ("\*.ini"). 
+It is recommended to just go with the template and maybe change a few minor things, depending on need. A template is given in the Github repo under data/config_examples/configuration_template.ini. The file contains comments describing the entries. Take a careful look at all comments containing "Change" as these are relevant to adjust depending on your setup. If your imager records h5 data, adjusting the h5 paths (sections 'HDF.xxxx') is relevant too. Morover, we interface with the configuration in a dictionary-style manner:
+
+```
+# Make an object and read the config file for the mission
+config = configparser.ConfigParser()
+config.read(config_file_mission)
+
+# Access a specific configuration, e.g. the calibrated camera model of the imager
+hsi_calib_path = config['Absolute Paths']['hsi_calib_path'] # config[<section>][<config-entry>]
+```
+
+
+### Calibration file ("\*.xml")
+The *.xml file is our chosen camera model file and looks like this:
+```
+<?xml version="1.0" encoding="utf-8"?>
+<calibration>
+    <rx>0.0</rx>
+    <ry>0.0</ry>
+    <rz>-1.5707963267948966</rz>
+    <tx>0</tx>
+    <ty>0</ty>
+    <tz>0</tz>
+    <f>754.9669285377008</f>
+    <cx>255.00991757530994</cx>
+    <k1>-72.31892156971124</k1>
+    <k2>-389.57799574674084</k2>
+    <k3>4.075384496065511</k3>
+    <width>512</width>
+</calibration>
+```
+rx, ry and rz are the boresight angles in radians, while tx, ty and tz are lever arms in the vehicle body frame. They are used to transform vectors from the HSI camera frame to the vehicle body frame through:
+```
+rot_hsi_ref_eul = np.array([rz, ry, rx])
+
+R = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False).as_matrix() # Rotation matrix from HSI to body
+
+t = np.array([tx, ty, tz])
+
+X_hsi = np.array([x, y, z]) # some vector
+
+X_body =  R*X_hsi + t# the vector expressed in the body frame 
+```
+In our computation we use a frame convention akin to the camera frames in computer vision. This means that x-right, y-backward, and z-downward for a well aligned camera. In contrast the vehicle body frame follows the roll-pitch-yaw convention with x-forward, y-starboard, z-downward. This is why the rz is by default $\pm \pi/2$. The easiest if you are unsure of whether your scanner is flipped is to swap the sign rz.
+
+
+
+Moreover, the f represent the camera's focal length in pixels, width is the number of spatial pixels, while cx is the principal pixel. Often cx=(width+1)/2, e.g. if you have 5 pixels u = 1,..,5 the middle pixel is cx=3. In other words, our convention is to assign the cell centres of pixels as whole integers (starting at 1), in contrast to OpenCV which starts at 0.5. The k1, k2 are radial distortion coefficients, while k3 is a tangential coefficient. The camera model is adapted from [Sun et al. (2016)](https://opg.optica.org/ao/fulltext.cfm?uri=ao-55-25-6836&id=348983). Expressing a pixel on an undistorted image plane in the HSI frame is done through
+```
+u = np.random.randint(1, width + 1) # Pixel numbers left to right (value from 1 to width)
+
+# Pinhole part
+x_norm_pinhole = (u - cx) / f
+
+# Distortion part
+x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
+                  k2 * ((u - cx) / 1000) ** 3 + \
+                  k3 * ((u - cx) / 1000) ** 2) / f
+
+x_norm_hsi = x_norm_pinhole + x_norm_nonlin
+
+X_norm_hsi = np.array([x_norm_hsi, 0, 1]) # The pixel ray in the hsi frame
+```
+
+Of course most of these parameters are hard to guess for a HSI and there are two simple ways of finding them. The first way is to ignore distortions and assume you know the angular field of view (AFOV). Then you can calculate:
+
+$$f = \frac{width}{2tan(AFOV/2)}$$
+
+
+Besides that, you set cx=width/2, and remaining k's to zero. 
+
+The second approach to get the camera model is if you have an array describing the FOV (often from the manufacturer). 
+In our example above that would amount to a 512-length array, e.g. in degrees 
+```
+from gref4hsi.specim_parsing_utils import Specim
+
+# FOV array from manufacturer describing the view angle of each pixel
+fov = np.array([-19.1, -19.0 .... 19.0, 19.1]) # Length as number of pixels
+
+# Use static method to convert fov to parameters dictionary equivalent to xml file (with boresights and lever arms to zero)
+param_dict = Specim.fov_2_param(fov = specim_object.view_angles)
+
+# Write to an *.xml file
+param_dict['rz'] = rx
+param_dict['ry'] = ry
+param_dict['rx'] = rz
+
+# Vector from origin of HSI to body origin, expressed in body
+# User set
+t_hsi_body = config_specim.translation_body_to_hsi
+param_dict['tz'] = tx
+param_dict['ty'] = ty
+param_dict['tz'] = tz
+
+# Write dictionary to *.xml file
+CalibHSI(file_name_cal_xml= confic['Absolute Paths']['hsi_calib_path'], 
+                    mode = 'w', 
+                    param_dict = param_dict)
+```
+
+
+
+### Terrain files
+There are three allowable types ("model_export_type" in the configuration file), namely "ply_file" (a.k.a. mesh files), "dem_file" and "geoid". Example geoids are added under data/world/geoids/ including the global egm08 and a norwegian geoid. Your local geoid can probably be found from [geoids](https://www.agisoft.com/downloads/geoids/) or similar. Just ensure you add this path to the 'Absolute Paths' section in the configuration file. Similarly, if you choose "model_export_type = dem_file", you can use a terrain model from from your area as long as you add the path to the file in the 'Absolute Paths'. Remember that if the local terrain (dem file) is given wrt the geoid, you can plus them together in e.g. QGIS or simply add an approximate offset in python with rasterio. This is because the software expects DEMs giving the ellipsoid height of the terrain. Lastly, if the "ply_file", or 3D triangular mesh is the desired option, a path to this file must be added to the config file. It should be fairly easy to use any triangular mesh format even though the option suggests "\*.ply". 
+
+### The h5 files
+This format must comply with the h5 paths in the configuration file. All sections starting with "HDF.xxxx" are related to these paths. I realize that it is inconvenient to transform the format if your recorded data is in NETCDF, ENVI etc, but making this software I chose H5/HDF because of legacy and because of the flexibility of the mini-file system. The input structure (only mandatory entries) of the H5 files under mission_dir/Input/H5 is as follows (printed using h5tree in Linux):  
+```
+2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
+â”œâ”€â”€ processed
+â”‚   â””â”€â”€ radiance
+â”‚       â”œâ”€â”€ calibration
+â”‚       â”‚   â”œâ”€â”€ geometric # Optional
+â”‚       â”‚   â”‚   â””â”€â”€ view_angles
+â”‚       â”‚   â”œâ”€â”€ radiometric # Only if is_radiance = False
+â”‚       â”‚   â”‚   â”œâ”€â”€ darkFrame
+â”‚       â”‚   â”‚   â””â”€â”€ radiometricFrame
+â”‚       â”‚   â””â”€â”€ spectral 
+â”‚       â”‚       â”œâ”€â”€ band2Wavelength
+â”‚       â”‚       â””â”€â”€ fwhm # Optional
+â”‚       â”œâ”€â”€ dataCube 
+â”‚       â”œâ”€â”€ exposureTime
+â”‚       â””â”€â”€ timestamp
+â””â”€â”€ raw
+    â””â”€â”€ nav
+        â”œâ”€â”€ euler_angles
+        â”œâ”€â”€ position_ecef
+        â””â”€â”€ timestamp
+```
+Note that all these paths are parameters in the config file and you will now we will explain how to simply fill in this file tree using the config file. An example of format conversion is given under gref4hsi/utils/specim_parsing_utils.py where the raw format of the specim data and a navigation system is converted and written to the h5 format. The following code is taken from that script and shows how you can write all the necessary data to the appropriate h5 format. Assume that "specim_object" represents an object whose attributes are the datasets, meaning that e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
+
+```
+def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
+    with h5py.File(h5_filename, 'w', libver='latest') as f:
+        for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
+            #print(attribute_name)
+            dset = f.create_dataset(name=h5_hierarchy_item_path, 
+                                            data = getattr(specim_object, attribute_name))
+
+h5_dict_write = {'eul_zyx' : config['HDF.raw_nav']['eul_zyx'],
+            'position_ecef' : config['HDF.raw_nav']['position'],
+            'nav_timestamp' : config['HDF.raw_nav']['timestamp'],
+            'radiance_cube': config['HDF.hyperspectral']['datacube'],
+            't_exp_ms': config['HDF.hyperspectral']['exposuretime'],
+            'hsi_timestamps': config['HDF.hyperspectral']['timestamp'],
+            'view_angles': config['HDF.calibration']['view_angles'], # Optional
+            'wavelengths' : config['HDF.calibration']['band2wavelength'],
+            'fwhm' : config['HDF.calibration']['fwhm'], # Optional
+            'dark_frame' : config['HDF.calibration']['darkframe'], # Optional unless 'is_radiance' is False
+            'radiometric_frame' : config['HDF.calibration']['radiometricframe']} # Optional unless 'is_radiance' is False
+
+# The dictionary is equivalent to the tree view above (assuming configuration_template.ini):
+h5_dict_write = {
+  'eul_zyx':            'raw/nav/euler_angles',
+  'position_ecef':     'raw/nav/position_ecef',
+  'nav_timestamp':     'raw/nav/timestamp',
+  'radiance_cube':    'processed/radiance/dataCube',
+  't_exp_ms':          'processed/radiance/exposureTime',
+  'hsi_timestamps':   'processed/radiance/timestamp',
+  'view_angles':       'processed/radiance/calibration/geometric/view_angles',
+  'wavelengths':       'processed/radiance/calibration/spectral/band2Wavelength',
+  'fwhm':              'processed/radiance/calibration/spectral/fwhm',
+  'dark_frame':        'processed/radiance/calibration/radiometric/darkFrame',
+  'radiometric_frame': 'processed/radiance/calibration/radiometric/radiometricFrame'
+}
+
+# At last, write the data to a h5 file
+# In this case 'specim_object' is an object whoose attributes correspond to the above keys
+# e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write  the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
+specim_object_2_h5_file(h5_filename=h5_filename, h5_tree_dict=h5_dict_write, specim_object=specim_object)
+```
+My recommended approach would be that you create your own modified xxx_parsing_utils.py (feel free to send a pull request) which parses and writes your specific navigation data and hyperspectral data into the format.
+
+The last thing worth mentioning is the navigation data. The aforementioned specim_parsing_utils.py parses navigation data from messages, e.g.
+
+Positions from 
+"$GPGGA,125301.00,6335.47830829,N,00932.34206055,E,2,07,1.7,18.434,M,41.216,M,4.0,0123\*79"
+
+Orientations/attitude from messages like
+"$PASHR,125648.280,322.905,T,0.621,-0.114,,0.034,0.034,0.450,2,3\*1B"
+
+The above data log is read with the method (in the case you have a similar navigation format)
+
+```
+specim_object.read_nav_file(nav_file_path=nav_file_path, date = date_string)
+```
+
+Lastly, the data should be formatted as follows for writing:
+
+```
+import pymap3d as pm
+
+# If your nav system gave you geodetic positions, convert them to earth centered earth fixed (ECEF). Make sure to use ellipsoid height (not height above mean sea level (MSL) aka geoid)
+x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
+
+# Roll pitch yaw are ordered with in an unintuitive attribute name eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
+specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
+
+# The ECEF positions
+specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
+```
+
+Then the "specim_object_2_h5_file" puts the data into the right place.
+
+## Running the processing
+Once the above has been defined the processing can be run with a few lines of code (taken from gref4hsi/tests/test_main_specim.py):
+```
+from gref4hsi.scripts import georeference
+from gref4hsi.scripts import orthorectification
+from gref4hsi.utils import parsing_utils, specim_parsing_utils
+from gref4hsi.scripts import visualize
+
+
+# This function parses raw specim data including (spectral, radiometric, geometric) calibrations and nav data
+# into an h5 file. The nav data is written to "raw/nav/" subfolders, whereas hyperspectral data and calibration data 
+# written to "processed/hyperspectral/" and "processed/calibration/" subfolders. The camera model \*.xml file is also generated.
+# The script must be adapted to other 
+specim_parsing_utils.main(config=config,
+                          config_specim=config_specim_preprocess)
+
+# Interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
+config = parsing_utils.export_pose(config_file_mission)
+
+# Exports model
+parsing_utils.export_model(config_file_mission)
+
+# Georeference the line scans of the hyperspectral imager. Utilizes parsed data
+georeference.main(config_file_mission)
+
+# Orthorectify/resample datacube, RGB-composite and ancillary data
+orthorectification.main(config_file_mission)
+
+# Optional: coregistration
+# Match RGB composite to reference, find features and following data, ground control point (gcp) list, for each feature pair:
+# reference point 3D (from reference), position/orientation of vehicle (using resampled time) and pixel coordinate (using resampled pixel coordinate)
+coregistration.main(config_file_mission, mode='compare')
+
+# The gcp list allows reprojecting reference points and evaluate the reprojection error,
+# which is used to optimize static geometric parameters (e.g. boresight...) or dynamic geometric parameters (time-varying nav errors).
+coregistration.main(config_file_mission, mode='calibrate')
+```
+
```

### Comparing `gref4hsi-0.2.1/gref4hsi/scripts/georeference.py` & `gref4hsi-0.2.2/gref4hsi/scripts/georeference.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,299 +1,293 @@
-# Built-ins
-import configparser
-import json
-import os
-import sys
-
-# Third party
-from scipy.spatial.transform import Rotation as RotLib
-import numpy as np
-import pyvista as pv
-import h5py
-
-# Lib resources:
-from gref4hsi.utils.geometry_utils import CameraGeometry, CalibHSI
-from gref4hsi.utils.parsing_utils import Hyperspectral
-from gref4hsi.utils import visualize
-
-
-def cal_file_to_rays(filename_cal):
-        # See paper by Sun, Bo, et al. "Calibration of line-scan cameras for precision measurement." Applied optics 55.25 (2016): 6836-6843.
-        # Loads line camera parameters for the hyperspectral imager from an xml file.
-
-        # Certain imagers deliver geometry "per pixel". This can be resolved by fitting model parameters.
-        calHSI = CalibHSI(file_name_cal_xml=filename_cal)
-        f = calHSI.f
-        u_c = calHSI.cx
-
-        # Radial distortion parameters
-        k1 = calHSI.k1
-        k2 = calHSI.k2
-
-        # Tangential distortion parameters
-        k3 = calHSI.k3
-
-        # Translation (lever arm) of HSI with respect to vehicle frame
-        trans_x = calHSI.tx
-        trans_y = calHSI.ty
-        trans_z = calHSI.tz
-
-        # Rotation of HSI (boresight) with respect to vehicle navigation frame (often defined by IMU or RGB cam)
-        rot_x = calHSI.rx
-        rot_y = calHSI.ry
-        rot_z = calHSI.rz
-
-        # Number of pixels
-        n_pix = calHSI.w
-
-        # Define camera model array.
-        u = np.arange(1, n_pix + 1)
-
-        # Express uhi ray directions in uhi frame using line-camera model
-        x_norm_lin = (u - u_c) / f
-
-        x_norm_nonlin = -(k1 * ((u - u_c) / 1000) ** 5 + \
-                          k2 * ((u - u_c) / 1000) ** 3 + \
-                          k3 * ((u - u_c) / 1000) ** 2) / f
-
-        x_norm = x_norm_lin + x_norm_nonlin
-
-        p_dir = np.zeros((len(x_norm), 3))
-
-        # Rays are defined in the HI frame with positive z down
-        p_dir[:, 0] = x_norm
-        p_dir[:, 2] = 1
-
-        rot_hsi_ref_eul = np.array([rot_z, rot_y, rot_x])
-
-        rot_hsi_ref_obj = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False)
-
-        translation_ref_hsi = np.array([trans_x, trans_y, trans_z])
-
-        intrinsic_geometry_dict = {'translation_ref_hsi': translation_ref_hsi,
-                                   'rot_hsi_ref_obj': rot_hsi_ref_obj,
-                                   'ray_directions_local': p_dir}
-        
-        # Notably, one could compress the information by expressing the ray directions in the body frame
-
-        return intrinsic_geometry_dict
-
-def define_hsi_ray_geometry(pos_ref_ecef, quat_ref_ecef, time_pose, intrinsic_geometry_dict):
-        """Instantiate a camera geometry object from the h5 pose data"""
-
-
-        pos = pos_ref_ecef # Reference positions in ECEF
-        rot_obj = RotLib.from_quat(quat_ref_ecef) # Reference orientations wrt ECEF
-        
-        ray_directions_local = intrinsic_geometry_dict['ray_directions_local']
-        translation_ref_hsi = intrinsic_geometry_dict['translation_ref_hsi']
-        rot_hsi_ref_obj = intrinsic_geometry_dict['rot_hsi_ref_obj']
-
-        hsi_geometry = CameraGeometry(pos=pos, rot=rot_obj, time=time_pose, is_interpolated=True)
-        
-        
-        hsi_geometry.intrinsicTransformHSI(translation_ref_hsi=translation_ref_hsi, rot_hsi_ref_obj = rot_hsi_ref_obj)
-
-        hsi_geometry.defineRayDirections(dir_local = ray_directions_local)
-
-        return hsi_geometry
-
-def write_intersection_geometry_2_h5_file(hsi_geometry, config, h5_filename):
-    # Write all intersection data (ancilliary) that could be relevant
-    
-    dict_ancilliary = config['Georeferencing']
-    # Dictionary keys correspond to CameraGeometry attribute names (e.g. hsi_geometry.key), while values correspond to h5 data set paths.
-    
-    with h5py.File(h5_filename, 'a', libver='latest') as f:
-        for attribute_name, h5_hierarchy_item_path in dict_ancilliary.items():
-            if attribute_name != 'folder':
-                if h5_hierarchy_item_path in f:
-                    del f[h5_hierarchy_item_path]
-                dset = f.create_dataset(name=h5_hierarchy_item_path, 
-                                                data = getattr(hsi_geometry, attribute_name))
-
-
-# Function called to apply standard processing on a folder of files
-def main(iniPath, viz = False, use_coreg_param = False):
-    config = configparser.ConfigParser()
-    config.read(iniPath)
-
-    # Paths to 3D mesh ply file 
-    path_mesh = config['Absolute Paths']['model_path']
-
-    # Directory of H5 files
-    dir_r = config['Absolute Paths']['h5_folder']
-
-    
-
-    
-
-    # Timestamps here
-    h5_folder_time_pose = config['HDF.processed_nav']['timestamp']
-
-    # Use the regular parameters from nav system and manufacturer:
-    # The path to the XML file
-    hsi_cal_xml = config['Absolute Paths']['hsi_calib_path']
-
-    # Position is stored here in the H5 file
-    h5_folder_position_ecef = config['HDF.processed_nav']['position_ecef']
-
-    # Quaternion is stored here in the H5 file
-    h5_folder_quaternion_ecef = config['HDF.processed_nav']['quaternion_ecef']
-
-    if use_coreg_param:
-        print('Using coregistred parameters for georeferencing')
-
-        # Set the camera model to the calibrated one if it exists
-        hsi_cal_xml_coreg = config['Absolute Paths']['calib_file_coreg']
-        if os.path.exists(hsi_cal_xml_coreg):
-             hsi_cal_xml = hsi_cal_xml_coreg
-
-        # Optimized position
-        h5_folder_position_ecef_coreg = config['HDF.coregistration']['position_ecef']
-
-        # Quaternion 
-        h5_folder_quaternion_ecef_coreg = config['HDF.coregistration']['quaternion_ecef']
-        
-
-    
-    
-    
-    # The path to the Tide file (if necessary and available)
-    try:
-        path_tide = config['Absolute Paths']['tide_path']
-    except Exception as e:
-        path_tide = 'Undefined'
-    
-    # Maximal allowed ray length
-    max_ray_length = float(config['General']['max_ray_length'])
-
-    mesh = pv.read(path_mesh)
-
-    """metadata_mesh = {
-        "offset_x": offset_x,
-        "offset_y": offset_y,
-        "offset_z": offset_y,
-        "epsg_code": geocsc.to_epsg(),  # Example EPSG code, replace with your actual code
-        "data_type": str(mesh.points.dtype),  # Add other metadata entries here
-    }"""
-
-    model_meta_path = path_mesh.split('.')[0] + '_meta.json' 
-    with open(model_meta_path, "r") as f:
-        # Load the JSON data from the file
-        metadata_mesh = json.load(f)
-        mesh_off_x = metadata_mesh['offset_x']
-        mesh_off_y = metadata_mesh['offset_y']
-        mesh_off_z = metadata_mesh['offset_z']
-        # Mesh is translated by this much
-        mesh_trans = np.array([mesh_off_x, mesh_off_y, mesh_off_z]).astype(np.float64)
-
-    
-    print("\n################ Georeferencing: ################")
-    files = sorted(os.listdir(dir_r))
-    n_files= len(sorted(os.listdir(dir_r)))
-    file_count = 0
-    for filename in files:
-        if filename.endswith('h5') or filename.endswith('hdf'):
-
-            progress_perc = 100*file_count/n_files
-            print(f"Georeferencing file {file_count+1}/{n_files}, progress is {progress_perc} %")
-
-            # Path to hierarchical file
-            h5_filename = dir_r + filename
-
-            # Read h5 file
-            hyp = Hyperspectral(h5_filename, config)
-
-            if use_coreg_param:
-                 try:
-                    # Use the coregistred dataset if it exists
-                    print('Using coregistred position')
-                    pos_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                    dataset_name= h5_folder_position_ecef_coreg)
-                 except:
-                    # If not use the original
-                    pos_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                    dataset_name= h5_folder_position_ecef)
-                 try:
-                    # Use the coregistred quaternion-dataset if it exists
-                    print('Using coregistred quaternion')
-                    quat_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                    dataset_name= h5_folder_quaternion_ecef_coreg)
-                 except:
-                     # If not use the original
-                    quat_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                    dataset_name= h5_folder_quaternion_ecef)
-            else:
-
-                # Just use the regular navigation data
-                # If not use the original
-                pos_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                dataset_name= h5_folder_position_ecef)
-                # Extract the ecef orientations for each frame
-                quat_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                                dataset_name=h5_folder_quaternion_ecef)
-            # Extract the timestamps for each frame
-            time_pose = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                            dataset_name= h5_folder_time_pose)
-
-
-            # Using the cal file, we can define lever arm, boresight and camera model geometry (in dictionary)
-            intrinsic_geometry_dict = cal_file_to_rays(filename_cal=hsi_cal_xml)
-
-            
-            # Define the rays in ECEF for each frame. 
-            hsi_geometry = define_hsi_ray_geometry(pos_ref_ecef, 
-                                    quat_ref_ecef, 
-                                    time_pose,
-                                    intrinsic_geometry_dict = intrinsic_geometry_dict)
-
-            
-            hsi_geometry.intersect_with_mesh(mesh = mesh, max_ray_length=max_ray_length, mesh_trans = mesh_trans)
-            
-            # Computes the view angles in the local NED. Computationally intensive as local NED is defined for each intersection
-            hsi_geometry.compute_view_directions_local_tangent_plane()
-
-            # Computes the sun angles in the local NED. Computationally intensive as local NED is defined for each intersection
-            hsi_geometry.compute_sun_angles_local_tangent_plane()
-
-            hsi_geometry.compute_tide_level(path_tide, tide_format = 'NMA')
-
-            hsi_geometry.compute_elevation_mean_sealevel(source_epsg = config['Coordinate Reference Systems']['geocsc_epsg_export'], 
-                                                         geoid_path = config['Absolute Paths']['geoid_path'])
-            
-            write_intersection_geometry_2_h5_file(hsi_geometry=hsi_geometry, config = config, h5_filename=h5_filename)
-
-            hsi_geometry.write_rgb_point_cloud(config = config, hyp = hyp, transect_string = filename.split('.')[0])
-
-            if viz:
-                 visualize.show_projected_hsi_points(HSICameraGeometry=hsi_geometry, 
-                                                     config=config, 
-                                                     transect_string = filename.split('.')[0])
-
-            
-
-
-            
-            
-
-            #from scripts import visualize
-            #visualize.show_projected_hsi_points(HSICameraGeometry=hsi_geometry, config=config, transect_string = filename.split('.')[0])
-
-        file_count+=1
-            
-
-
-
-
-
-
-
-
-
-
-
-
-if __name__ == '__main__':
-    args = sys.argv[1:]
-    iniPath = args[0]
-    main(iniPath)
+# Built-ins
+import configparser
+import json
+import os
+import sys
+
+# Third party
+from scipy.spatial.transform import Rotation as RotLib
+import numpy as np
+import pyvista as pv
+import h5py
+
+# Lib resources:
+from gref4hsi.utils.geometry_utils import CameraGeometry, CalibHSI
+from gref4hsi.utils.parsing_utils import Hyperspectral
+from gref4hsi.utils import visualize
+
+
+def cal_file_to_rays(filename_cal):
+        # See paper by Sun, Bo, et al. "Calibration of line-scan cameras for precision measurement." Applied optics 55.25 (2016): 6836-6843.
+        # Loads line camera parameters for the hyperspectral imager from an xml file.
+
+        # Certain imagers deliver geometry "per pixel". This can be resolved by fitting model parameters.
+        calHSI = CalibHSI(file_name_cal_xml=filename_cal)
+        f = calHSI.f
+        cx = calHSI.cx
+
+        # Radial distortion parameters
+        k1 = calHSI.k1
+        k2 = calHSI.k2
+
+        # Tangential distortion parameters
+        k3 = calHSI.k3
+
+        # Translation (lever arm) of HSI with respect to vehicle frame
+        trans_x = calHSI.tx
+        trans_y = calHSI.ty
+        trans_z = calHSI.tz
+
+        # Rotation of HSI (boresight) with respect to vehicle navigation frame (often defined by IMU or RGB cam)
+        rot_x = calHSI.rx
+        rot_y = calHSI.ry
+        rot_z = calHSI.rz
+
+        # Number of pixels
+        n_pix = calHSI.w
+
+        # Define camera model array.
+        u = np.arange(0, n_pix) + 1
+
+        # Express uhi ray directions in uhi frame using line-camera model
+        x_norm_lin = (u - cx) / f
+
+        x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
+                          k2 * ((u - cx) / 1000) ** 3 + \
+                          k3 * ((u - cx) / 1000) ** 2) / f
+
+        x_norm = x_norm_lin + x_norm_nonlin
+
+        p_dir = np.zeros((len(x_norm), 3))
+
+        # Rays are defined in the HI frame with positive z down
+        p_dir[:, 0] = x_norm
+        p_dir[:, 2] = 1
+
+        rot_hsi_ref_eul = np.array([rot_z, rot_y, rot_x])
+
+        rot_hsi_ref_obj = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False)
+
+        translation_ref_hsi = np.array([trans_x, trans_y, trans_z])
+
+        intrinsic_geometry_dict = {'translation_ref_hsi': translation_ref_hsi,
+                                   'rot_hsi_ref_obj': rot_hsi_ref_obj,
+                                   'ray_directions_local': p_dir}
+        
+        # Notably, one could compress the information by expressing the ray directions in the body frame
+
+        return intrinsic_geometry_dict
+
+def define_hsi_ray_geometry(pos_ref_ecef, quat_ref_ecef, time_pose, intrinsic_geometry_dict):
+        """Instantiate a camera geometry object from the h5 pose data"""
+
+
+        pos = pos_ref_ecef # Reference positions in ECEF
+        rot_obj = RotLib.from_quat(quat_ref_ecef) # Reference orientations wrt ECEF
+        
+        ray_directions_local = intrinsic_geometry_dict['ray_directions_local']
+        translation_ref_hsi = intrinsic_geometry_dict['translation_ref_hsi']
+        rot_hsi_ref_obj = intrinsic_geometry_dict['rot_hsi_ref_obj']
+
+        hsi_geometry = CameraGeometry(pos=pos, rot=rot_obj, time=time_pose, is_interpolated=True)
+        
+        
+        hsi_geometry.intrinsicTransformHSI(translation_ref_hsi=translation_ref_hsi, rot_hsi_ref_obj = rot_hsi_ref_obj)
+
+        hsi_geometry.defineRayDirections(dir_local = ray_directions_local)
+
+        return hsi_geometry
+
+def write_intersection_geometry_2_h5_file(hsi_geometry, config, h5_filename):
+    # Write all intersection data (ancilliary) that could be relevant
+    
+    dict_ancilliary = config['Georeferencing']
+    # Dictionary keys correspond to CameraGeometry attribute names (e.g. hsi_geometry.key), while values correspond to h5 data set paths.
+    
+    with h5py.File(h5_filename, 'a', libver='latest') as f:
+        for attribute_name, h5_hierarchy_item_path in dict_ancilliary.items():
+            if attribute_name != 'folder':
+                if h5_hierarchy_item_path in f:
+                    del f[h5_hierarchy_item_path]
+                dset = f.create_dataset(name=h5_hierarchy_item_path, 
+                                                data = getattr(hsi_geometry, attribute_name))
+
+
+# Function called to apply standard processing on a folder of files
+def main(iniPath, viz = False, use_coreg_param = False):
+    config = configparser.ConfigParser()
+    config.read(iniPath)
+
+    # Paths to 3D mesh ply file 
+    path_mesh = config['Absolute Paths']['model_path']
+
+    # Directory of H5 files
+    dir_r = config['Absolute Paths']['h5_folder']
+
+    
+
+    
+
+    # Timestamps here
+    h5_folder_time_pose = config['HDF.processed_nav']['timestamp']
+
+    # Use the regular parameters from nav system and manufacturer:
+    # The path to the XML file
+    hsi_cal_xml = config['Absolute Paths']['hsi_calib_path']
+
+    # Position is stored here in the H5 file
+    h5_folder_position_ecef = config['HDF.processed_nav']['position_ecef']
+
+    # Quaternion is stored here in the H5 file
+    h5_folder_quaternion_ecef = config['HDF.processed_nav']['quaternion_ecef']
+
+    if use_coreg_param:
+        print('Using coregistred parameters for georeferencing')
+
+        # Set the camera model to the calibrated one if it exists
+        hsi_cal_xml_coreg = config['Absolute Paths']['calib_file_coreg']
+        if os.path.exists(hsi_cal_xml_coreg):
+             hsi_cal_xml = hsi_cal_xml_coreg
+
+        # Optimized position
+        h5_folder_position_ecef_coreg = config['HDF.coregistration']['position_ecef']
+
+        # Quaternion 
+        h5_folder_quaternion_ecef_coreg = config['HDF.coregistration']['quaternion_ecef']
+        
+
+    
+    
+    
+    # The path to the Tide file (if necessary and available)
+    try:
+        path_tide = config['Absolute Paths']['tide_path']
+    except Exception as e:
+        path_tide = 'Undefined'
+    
+    # Maximal allowed ray length
+    max_ray_length = float(config['General']['max_ray_length'])
+
+    mesh = pv.read(path_mesh)
+
+    model_meta_path = path_mesh.split('.')[0] + '_meta.json' 
+    with open(model_meta_path, "r") as f:
+        # Load the JSON data from the file
+        metadata_mesh = json.load(f)
+        mesh_off_x = metadata_mesh['offset_x']
+        mesh_off_y = metadata_mesh['offset_y']
+        mesh_off_z = metadata_mesh['offset_z']
+        # Mesh is translated by this much
+        mesh_trans = np.array([mesh_off_x, mesh_off_y, mesh_off_z]).astype(np.float64)
+
+    
+    print("\n################ Georeferencing: ################")
+    files = sorted(os.listdir(dir_r))
+    n_files= len(sorted(os.listdir(dir_r)))
+    file_count = 0
+    for filename in files:
+        if filename.endswith('h5') or filename.endswith('hdf'):
+
+            progress_perc = 100*file_count/n_files
+            print(f"Georeferencing file {file_count+1}/{n_files}, progress is {progress_perc} %")
+
+            # Path to hierarchical file
+            h5_filename = dir_r + filename
+
+            # Read h5 file
+            hyp = Hyperspectral(h5_filename, config)
+
+            if use_coreg_param:
+                 try:
+                    # Use the coregistred dataset if it exists
+                    print('Using coregistred position')
+                    pos_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                    dataset_name= h5_folder_position_ecef_coreg)
+                 except:
+                    # If not use the original
+                    pos_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                    dataset_name= h5_folder_position_ecef)
+                 try:
+                    # Use the coregistred quaternion-dataset if it exists
+                    print('Using coregistred quaternion')
+                    quat_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                    dataset_name= h5_folder_quaternion_ecef_coreg)
+                 except:
+                     # If not use the original
+                    quat_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                    dataset_name= h5_folder_quaternion_ecef)
+            else:
+
+                # Just use the regular navigation data
+                # If not use the original
+                pos_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                dataset_name= h5_folder_position_ecef)
+                # Extract the ecef orientations for each frame
+                quat_ref_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                                dataset_name=h5_folder_quaternion_ecef)
+            # Extract the timestamps for each frame
+            time_pose = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                            dataset_name= h5_folder_time_pose)
+
+
+            # Using the cal file, we can define lever arm, boresight and camera model geometry (in dictionary)
+            intrinsic_geometry_dict = cal_file_to_rays(filename_cal=hsi_cal_xml)
+
+            
+            # Define the rays in ECEF for each frame. 
+            hsi_geometry = define_hsi_ray_geometry(pos_ref_ecef, 
+                                    quat_ref_ecef, 
+                                    time_pose,
+                                    intrinsic_geometry_dict = intrinsic_geometry_dict)
+
+            
+            hsi_geometry.intersect_with_mesh(mesh = mesh, max_ray_length=max_ray_length, mesh_trans = mesh_trans)
+
+            print(f'Mesh translation is {mesh_trans}')
+            
+            # Computes the view angles in the local NED. Computationally intensive as local NED is defined for each intersection
+            hsi_geometry.compute_view_directions_local_tangent_plane()
+
+            # Computes the sun angles in the local NED. Computationally intensive as local NED is defined for each intersection
+            hsi_geometry.compute_sun_angles_local_tangent_plane()
+
+            hsi_geometry.compute_tide_level(path_tide, tide_format = 'NMA')
+
+            hsi_geometry.compute_elevation_mean_sealevel(source_epsg = config['Coordinate Reference Systems']['geocsc_epsg_export'], 
+                                                         geoid_path = config['Absolute Paths']['geoid_path'])
+            
+            write_intersection_geometry_2_h5_file(hsi_geometry=hsi_geometry, config = config, h5_filename=h5_filename)
+
+            hsi_geometry.write_rgb_point_cloud(config = config, hyp = hyp, transect_string = filename.split('.')[0])
+
+            if viz:
+                 visualize.show_projected_hsi_points(HSICameraGeometry=hsi_geometry, 
+                                                     config=config, 
+                                                     transect_string = filename.split('.')[0])
+
+            
+
+
+            
+            
+
+            #from scripts import visualize
+            #visualize.show_projected_hsi_points(HSICameraGeometry=hsi_geometry, config=config, transect_string = filename.split('.')[0])
+
+        file_count+=1
+            
+
+
+
+
+
+
+
+
+
+
+
+
+if __name__ == '__main__':
+    args = sys.argv[1:]
+    iniPath = args[0]
+    main(iniPath)
```

### Comparing `gref4hsi-0.2.1/gref4hsi/scripts/orthorectification.py` & `gref4hsi-0.2.2/gref4hsi/scripts/orthorectification.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-import configparser
-import os
-import sys
-from collections import namedtuple
-
-import matplotlib.pyplot as plt
-import numpy as np
-
-# Local resources:
-from gref4hsi.utils.gis_tools import GeoSpatialAbstractionHSI
-from gref4hsi.utils.parsing_utils import Hyperspectral
-
-
-
-def main(iniPath):
-    config = configparser.ConfigParser()
-    config.read(iniPath)
-
-    # Paths for input data
-    h5_folder = config['Absolute Paths']['h5_folder']
-
-    # Paths for output data:
-    # 1) The data cube locations
-    envi_cube_dir = config['Absolute Paths']['orthorectified_cube_folder']
-
-    # 2) The RGB composite locations
-    rgb_composite_dir = config['Absolute Paths']['rgb_composite_folder']
-
-    # 3) The ancillary data locations
-    anc_dir = config['Absolute Paths']['anc_folder']
-
-    # 3) The footprints
-    footprint_dir = config['Absolute Paths']['footprint_folder']
-
-    
-
-
-    # The necessary data from the H5 file for resampling the datacube and composite (fwhm is optional)
-    # ECEF point cloud from georeferencing.
-    h5_folder_point_cloud_ecef = config['Georeferencing']['points_ecef_crs']
-
-    # Radiance cube
-    h5_folder_radiance_cube = config['HDF.hyperspectral']['datacube']
-
-    # Wavelength centers for all bands
-    h5_folder_wavelength_centers = config['HDF.calibration']['band2wavelength']
-    
-    try:
-        h5_folder_wavelength_widths = config['HDF.calibration']['fwhm']
-    except:
-        h5_folder_wavelength_widths = 'undefined'
-
-    # The necessary data (a dictionary) from H5 file for resampling ancillary data (uses the same grid as datacube)
-    anc_dict = config['Georeferencing']
-
-    # Settings having to do with coordinate reference systems, described below
-    SettingsCRS = namedtuple('SettingsOrthorectification', ['epsg_geocsc', 
-                                                              'epsg_proj'])
-    
-    config_crs = SettingsCRS(epsg_geocsc=int(config['Coordinate Reference Systems']['geocsc_epsg_export']),
-                             # The epsg code of the geocentric coordinate system (ECEF)
-                             epsg_proj=int(config['Coordinate Reference Systems']['proj_epsg']),
-                             # The epsg code of the projected coordinate system (e.g. UTM 32 has epsg 32632 for wgs 84 ellipsoid)
-                             )
-
-    # Settings associated with orthorectification of datacube
-    SettingsOrtho = namedtuple('SettingsOrthorectification', ['ground_resolution', 
-                                                                            'wl_red', 
-                                                                            'wl_green', 
-                                                                            'wl_blue',
-                                                                            'nodata_value',
-                                                                            'raster_transform_method',
-                                                                            'resample_rgb_only',
-                                                                            'chunk_size_cube_GB',
-                                                                            'wavelength_unit',
-                                                                            'radiometric_unit',
-                                                                            'sensor_type',
-                                                                            'interleave'])
-    
-    config_ortho = SettingsOrtho(ground_resolution = float(config['Orthorectification']['resolutionHyperspectralMosaic']), 
-                                 # Rectified grid resolution in meters
-                              wl_red = float(config['General']['red_wave_length']), 
-                              # Red wavelength in <wavelength_unit>
-                              wl_green = float(config['General']['green_wave_length']), 
-                              # Green wavelength in <wavelength_unit>
-                              wl_blue = float(config['General']['blue_wave_length']), 
-                              # Blue wavelength in <wavelength_unit>
-                              raster_transform_method = config['Orthorectification']['raster_transform_method'], 
-                              # Describes what raster transform to use. Either "north_east" or "minimal_rectangle". 
-                              # Latter is fastest and most memory efficient, but support is lacking for several GIS software.
-                              nodata_value = int(config['Orthorectification']['nodata']),
-                              # The fill value for empty cells (select values not occcuring in cube or ancillary data)
-                              resample_rgb_only = eval(config['Orthorectification']['resample_rgb_only']),
-                              # Boolean being expressing whether to rectify only composite (true) or data cube and composite (false). True is fast.
-                              chunk_size_cube_GB = float(config['Orthorectification']['chunk_size_cube_GB']),
-                              # For large files, RAM issues could be a concern. For rectified files exeeding this size, data is written chunk-wize to a memory map.
-                              wavelength_unit = config['General']['wavelength_unit'],
-                              # Unit of wavelengths, often nanometer
-                              radiometric_unit = config['General']['radiometric_unit'],
-                              # Unit of radiance, often like <pfx1>Watts / ( [<pfx2>^2]meter^2 steradian <pfx3>meter). pfx means metric prefix.
-                              # <pfx1> relates to energy and is 1, milli (10e-3) or micro (10e-6)
-                              # <pfx2> relates to area and is 1 or centi (10e-2)
-                              # <pfx3> relates to wavelength and is micro (10e-6) or nano (10e-9)
-                              sensor_type = config['General']['sensor_type'],
-                              # Brand and model
-                              interleave = config['Orthorectification']['interleave']
-                              # ENVI interleave: either 'bsq', 'bip' or 'bil', see:
-                              # https://envi.geoscene.cn/help/Subsystems/envi/Content/ExploreImagery/ENVIImageFiles.htm
-                              )
-
-
-    print("\n################ Orthorectifying: ################")
-    files = sorted(os.listdir(h5_folder))
-    n_files= len(sorted(os.listdir(h5_folder)))
-    file_count = 0
-    for filename in files:
-        if filename.endswith('h5') or filename.endswith('hdf'):
-
-            progress_perc = 100*file_count/n_files
-            print(f"Orthorectifying file {file_count+1}/{n_files}, progress is {progress_perc} %")
-            # Path to hierarchical file
-            h5_filename = h5_folder + filename
-
-            # Read the 3D point cloud, radiance cube 
-            # Extract the point cloud
-            point_cloud_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                         dataset_name=h5_folder_point_cloud_ecef)
-            # Need the radiance cube for resampling
-            radiance_cube = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                         dataset_name=h5_folder_radiance_cube)
-        
-            wavelengths = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                            dataset_name=h5_folder_wavelength_centers)
-            try:
-                fwhm = Hyperspectral.get_dataset(h5_filename=h5_filename,
-                                                            dataset_name=h5_folder_wavelength_widths)
-            except KeyError:
-                fwhm = np.nan
-
-
-            # The code below is independent of the h5 file format. The exception is the writing of ancillary data to a form of datacube
-            # Generates an object for dealing with GIS operations
-            gisHSI = GeoSpatialAbstractionHSI(point_cloud=point_cloud_ecef, 
-                                              transect_string=filename.split('.')[0],
-                                              config_crs=config_crs)
-
-            # The point cloud is transformed to the projected system
-            gisHSI.transform_geocentric_to_projected(config_crs=config_crs)
-
-            # Calculate the footprint of hyperspectral data
-            gisHSI.footprint_to_shape_file(footprint_dir=footprint_dir)
-            
-            
-            
-            
-            gisHSI.resample_datacube(radiance_cube=radiance_cube,
-                                     wavelengths=wavelengths,
-                                     fwhm=fwhm,
-                                     envi_cube_dir=envi_cube_dir,
-                                     rgb_composite_dir=rgb_composite_dir,
-                                     config_ortho=config_ortho)
-
-            
-
-            # The ancilliary data is read from h5 files and converted into a datacube
-            if eval(config['Orthorectification']['resample_ancillary']): 
-                gisHSI.resample_ancillary(h5_filename=h5_filename, 
-                                        anc_dict = anc_dict, 
-                                        anc_dir = anc_dir,
-                                        interleave=config_ortho.interleave)
-        
-        file_count+=1
-if __name__ == '__main__':
-    args = sys.argv[1:]
-    iniPath = args[0]
+import configparser
+import os
+import sys
+from collections import namedtuple
+
+import matplotlib.pyplot as plt
+import numpy as np
+
+# Local resources:
+from gref4hsi.utils.gis_tools import GeoSpatialAbstractionHSI
+from gref4hsi.utils.parsing_utils import Hyperspectral
+
+
+
+def main(iniPath):
+    config = configparser.ConfigParser()
+    config.read(iniPath)
+
+    # Paths for input data
+    h5_folder = config['Absolute Paths']['h5_folder']
+
+    # Paths for output data:
+    # 1) The data cube locations
+    envi_cube_dir = config['Absolute Paths']['orthorectified_cube_folder']
+
+    # 2) The RGB composite locations
+    rgb_composite_dir = config['Absolute Paths']['rgb_composite_folder']
+
+    # 3) The ancillary data locations
+    anc_dir = config['Absolute Paths']['anc_folder']
+
+    # 3) The footprints
+    footprint_dir = config['Absolute Paths']['footprint_folder']
+
+    
+
+
+    # The necessary data from the H5 file for resampling the datacube and composite (fwhm is optional)
+    # ECEF point cloud from georeferencing.
+    h5_folder_point_cloud_ecef = config['Georeferencing']['points_ecef_crs']
+
+    # Radiance cube
+    h5_folder_radiance_cube = config['HDF.hyperspectral']['datacube']
+
+    # Wavelength centers for all bands
+    h5_folder_wavelength_centers = config['HDF.calibration']['band2wavelength']
+    
+    try:
+        h5_folder_wavelength_widths = config['HDF.calibration']['fwhm']
+    except:
+        h5_folder_wavelength_widths = 'undefined'
+
+    # The necessary data (a dictionary) from H5 file for resampling ancillary data (uses the same grid as datacube)
+    anc_dict = config['Ancillary']
+
+    # Settings having to do with coordinate reference systems, described below
+    SettingsCRS = namedtuple('SettingsOrthorectification', ['epsg_geocsc', 
+                                                              'epsg_proj'])
+    
+    config_crs = SettingsCRS(epsg_geocsc=int(config['Coordinate Reference Systems']['geocsc_epsg_export']),
+                             # The epsg code of the geocentric coordinate system (ECEF)
+                             epsg_proj=int(config['Coordinate Reference Systems']['proj_epsg']),
+                             # The epsg code of the projected coordinate system (e.g. UTM 32 has epsg 32632 for wgs 84 ellipsoid)
+                             )
+
+    # Settings associated with orthorectification of datacube
+    SettingsOrtho = namedtuple('SettingsOrthorectification', ['ground_resolution', 
+                                                                            'wl_red', 
+                                                                            'wl_green', 
+                                                                            'wl_blue',
+                                                                            'nodata_value',
+                                                                            'raster_transform_method',
+                                                                            'resample_rgb_only',
+                                                                            'chunk_size_cube_GB',
+                                                                            'wavelength_unit',
+                                                                            'radiometric_unit',
+                                                                            'sensor_type',
+                                                                            'interleave'])
+    
+    config_ortho = SettingsOrtho(ground_resolution = float(config['Orthorectification']['resolutionHyperspectralMosaic']), 
+                                 # Rectified grid resolution in meters
+                              wl_red = float(config['General']['red_wave_length']), 
+                              # Red wavelength in <wavelength_unit>
+                              wl_green = float(config['General']['green_wave_length']), 
+                              # Green wavelength in <wavelength_unit>
+                              wl_blue = float(config['General']['blue_wave_length']), 
+                              # Blue wavelength in <wavelength_unit>
+                              raster_transform_method = config['Orthorectification']['raster_transform_method'], 
+                              # Describes what raster transform to use. Either "north_east" or "minimal_rectangle". 
+                              # Latter is fastest and most memory efficient, but support is lacking for several GIS software.
+                              nodata_value = int(config['Orthorectification']['nodata']),
+                              # The fill value for empty cells (select values not occcuring in cube or ancillary data)
+                              resample_rgb_only = eval(config['Orthorectification']['resample_rgb_only']),
+                              # Boolean being expressing whether to rectify only composite (true) or data cube and composite (false). True is fast.
+                              chunk_size_cube_GB = float(config['Orthorectification']['chunk_size_cube_GB']),
+                              # For large files, RAM issues could be a concern. For rectified files exeeding this size, data is written chunk-wize to a memory map.
+                              wavelength_unit = config['General']['wavelength_unit'],
+                              # Unit of wavelengths, often nanometer
+                              radiometric_unit = config['General']['radiometric_unit'],
+                              # Unit of radiance, often like <pfx1>Watts / ( [<pfx2>^2]meter^2 steradian <pfx3>meter). pfx means metric prefix.
+                              # <pfx1> relates to energy and is 1, milli (10e-3) or micro (10e-6)
+                              # <pfx2> relates to area and is 1 or centi (10e-2)
+                              # <pfx3> relates to wavelength and is micro (10e-6) or nano (10e-9)
+                              sensor_type = config['General']['sensor_type'],
+                              # Brand and model
+                              interleave = config['Orthorectification']['interleave']
+                              # ENVI interleave: either 'bsq', 'bip' or 'bil', see:
+                              # https://envi.geoscene.cn/help/Subsystems/envi/Content/ExploreImagery/ENVIImageFiles.htm
+                              )
+
+
+    print("\n################ Orthorectifying: ################")
+    files = sorted(os.listdir(h5_folder))
+    n_files= len(sorted(os.listdir(h5_folder)))
+    file_count = 0
+    for filename in files:
+        if filename.endswith('h5') or filename.endswith('hdf'):
+
+            progress_perc = 100*file_count/n_files
+            print(f"Orthorectifying file {file_count+1}/{n_files}, progress is {progress_perc} %")
+            # Path to hierarchical file
+            h5_filename = h5_folder + filename
+
+            # Read the 3D point cloud, radiance cube 
+            # Extract the point cloud
+            point_cloud_ecef = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                         dataset_name=h5_folder_point_cloud_ecef)
+            # Need the radiance cube for resampling
+            radiance_cube = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                         dataset_name=h5_folder_radiance_cube)
+        
+            wavelengths = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                            dataset_name=h5_folder_wavelength_centers)
+            try:
+                fwhm = Hyperspectral.get_dataset(h5_filename=h5_filename,
+                                                            dataset_name=h5_folder_wavelength_widths)
+            except KeyError:
+                fwhm = np.nan
+
+
+            # The code below is independent of the h5 file format. The exception is the writing of ancillary data to a form of datacube
+            # Generates an object for dealing with GIS operations
+            gisHSI = GeoSpatialAbstractionHSI(point_cloud=point_cloud_ecef, 
+                                              transect_string=filename.split('.')[0],
+                                              config_crs=config_crs)
+
+            # The point cloud is transformed to the projected system
+            gisHSI.transform_geocentric_to_projected(config_crs=config_crs)
+
+            # Calculate the footprint of hyperspectral data
+            gisHSI.footprint_to_shape_file(footprint_dir=footprint_dir)
+            
+            
+            
+            # Resample imagery (RGB composite or both)
+            gisHSI.resample_datacube(radiance_cube=radiance_cube,
+                                     wavelengths=wavelengths,
+                                     fwhm=fwhm,
+                                     envi_cube_dir=envi_cube_dir,
+                                     rgb_composite_dir=rgb_composite_dir,
+                                     config_ortho=config_ortho)
+
+            
+
+            # The ancilliary data is read from h5 files and converted into a datacube
+            if eval(config['Orthorectification']['resample_ancillary']): 
+                gisHSI.resample_ancillary(h5_filename=h5_filename, 
+                                        anc_dict = anc_dict, 
+                                        anc_dir = anc_dir,
+                                        interleave=config_ortho.interleave)
+        
+        file_count+=1
+if __name__ == '__main__':
+    args = sys.argv[1:]
+    iniPath = args[0]
     main(iniPath)
```

### Comparing `gref4hsi-0.2.1/gref4hsi/tests/specim_process.py` & `gref4hsi-0.2.2/gref4hsi/tests/specim_process.py.orig`

 * *Files 19% similar despite different names*

```diff
@@ -1,249 +1,284 @@
-# Standard python library
-import configparser
-import sys
-import os
-import argparse
-from collections import namedtuple
-import pathlib
-import yaml
-
-if os.name == 'nt':
-    # Windows OS
-    base_fp = 'D:'
-    home = 'C:/Users/haavasl'
-elif os.name == 'posix':
-    # This Unix-like systems inl. Mac and fLinux
-    base_fp = '/media/haavasl/Expansion'
-    home = '/home/haavasl'
-
-# Use this if working with the github repo to do quick changes to the module
-module_path = os.path.join(home, 'VsCodeProjects/gref4hsi/')
-if module_path not in sys.path:
-    sys.path.append(module_path)
-
-# Local resources
-from gref4hsi.scripts import georeference, orthorectification, coregistration
-from gref4hsi.utils import parsing_utils, specim_parsing_utils
-from gref4hsi.utils import visualize
-from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths, customize_config
-
-
-import numpy as np
-
-"""
-This script is meant to be used for testing the processing pipeline of airborne HI data from the Specim AFX10 instrument.
-"""
-
-# Make it simple to swap when working a bit on windows and a bit on Linux
-
-
-
-def main(config_yaml, specim_mission_folder, geoid_path, config_template_path, lab_calibration_path, fast_mode = False):
-    # Read flight-specific yaml file
-    with open(config_yaml, 'r') as file:  
-        config_data = yaml.safe_load(file)
-    
-    
-    # assigning the arguments to variables for simple backwards compatibility
-    SPECIM_MISSION_FOLDER = specim_mission_folder
-    EPSG_CODE = config_data['mission_epsg']
-    RESOLUTION_ORTHOMOSAIC = config_data['resolution_orthomosaic']
-    CALIBRATION_DIRECTORY = lab_calibration_path
-    
-    
-    dem_fold = os.path.join(specim_mission_folder, "dem")
-
-    if not os.path.exists(dem_fold):
-        print('DEM folder does not exist so Geoid is used as terrain instead')
-        TERRAIN_TYPE = "geoid"
-    else:
-        if not os.listdir(dem_fold):
-            #print(f"The folder '{dem_fold}' is empty so Geoid is used as terrain instead.")
-            TERRAIN_TYPE = "geoid"
-        else:
-            # If there is a folder and it is not empty
-            # Find the only file that is there
-            files = [f for f in os.listdir(dem_fold) if f not in ('.', '..')]
-            DEM_PATH = os.path.join(dem_fold, files[0])
-            #print(f"The file '{DEM_PATH}' is used as terrain.")
-            TERRAIN_TYPE = "dem_file"
-    
-    
-    # Do coregistration if there is an orthomosaic to compare under "orthomosaic"
-    #do_coreg = True
-    ortho_ref_fold = os.path.join(specim_mission_folder, "orthomosaic")
-
-    if not os.path.exists(ortho_ref_fold):
-        print('Coregistration is not done, as there was no reference orthomosaic')
-        
-    else:
-        if not os.listdir(ortho_ref_fold):
-            print('Coregistration is not done, as there was no reference orthomosaic')
-        else:
-            # If there is a folder and it is not empty
-            # Find the only file that is there
-            ortho_ref_file = [f for f in os.listdir(ortho_ref_fold) if f not in ('.', '..')][0]
-            do_coreg = True
-            print(f"The file '{ortho_ref_file}' is used as as reference orthomosaic.")
-            
-    
-    
-    GEOID_PATH = geoid_path
-
-    # Settings associated with preprocessing of data from Specim Proprietary data to pipeline-compatible data
-    SettingsPreprocess = namedtuple('SettingsPreprocessing', ['dtype_datacube', 
-                                                                            'lines_per_chunk', 
-                                                                            'specim_raw_mission_dir',
-                                                                            'cal_dir',
-                                                                            'reformatted_missions_dir',
-                                                                            'rotation_matrix_hsi_to_body',
-                                                                            'translation_body_to_hsi',
-                                                                            'config_file_name'])
-
-    config_specim_preprocess = SettingsPreprocess(dtype_datacube = np.float32, # The data type for the datacube
-                                lines_per_chunk= 8000,  # Raw datacube is chunked into this many lines. GB_per_chunk = lines_per_chunk*n_pixels*n_bands*4 bytes
-                                specim_raw_mission_dir = SPECIM_MISSION_FOLDER, # Folder containing several mission
-                                cal_dir = CALIBRATION_DIRECTORY,  # Calibration directory holding all calibrations at all binning levels
-                                reformatted_missions_dir = os.path.join(SPECIM_MISSION_FOLDER, 'processed'), # The fill value for empty cells (select values not occcuring in cube or ancillary data)
-                                rotation_matrix_hsi_to_body = np.array([[0, 1, 0],
-                                                                        [-1, 0, 0],
-                                                                        [0, 0, 1]]), # Rotation matrix R rotating so that vec_body = R*vec_hsi.
-                                translation_body_to_hsi = np.array([0, 0, 0]), # Translation t so that vec_body_to_object = vec_hsi_to_object + t
-                                # For large files, RAM issues could be a concern. For rectified files exeeding this size, data is written chunk-wize to a memory map.
-                                config_file_name = 'configuration.ini')
-
-
-
-    # Where to place the config
-    DATA_DIR = config_specim_preprocess.reformatted_missions_dir
-    config_file_mission = os.path.join(DATA_DIR, 'configuration.ini')
-
-
-    # Set the data directory for the mission, and create empty folder structure
-    prepend_data_dir_to_relative_paths(config_path=config_template_path, DATA_DIR=DATA_DIR)
-
-    # Non-default settings
-    custom_config = {'General':
-                        {'mission_dir': DATA_DIR,
-                        'model_export_type': TERRAIN_TYPE, # Ray trace onto geoid
-                        'max_ray_length': 150}, # Max distance in meters from spectral imager to seafloor. Specim does not fly higher
-
-                    'Coordinate Reference Systems':
-                        {'proj_epsg' : EPSG_CODE, # The projected CRS UTM 32, common on mainland norway
-                        'geocsc_epsg_export' : 4978, # 3D cartesian system for earth consistent with GPS frame (but inconsistent with eurasian techtonic plate)
-                        'dem_epsg' : EPSG_CODE, # (Optional) If you have a DEM this can be used
-                        'pos_epsg_orig' : 4978}, # The CRS of the positioning data we deliver to the georeferencing
-
-                    'Orthorectification':
-                        {'resample_rgb_only': True, # True can be good choice for speed during DEV
-                         'resample_ancillary': True,
-                        'resolutionhyperspectralmosaic': RESOLUTION_ORTHOMOSAIC, # Resolution in m
-                        'raster_transform_method': 'north_east'}, # North-east oriented rasters.
-                    
-                    'HDF.raw_nav': {
-                        'rotation_reference_type' : 'eul_ZYX', # The vehicle orientations are given in Yaw, Pitch, Roll from the NAV system
-                        'is_global_rot' : False, # The vehicles orientations from NAV system are Yaw, Pitch, Roll
-                        'eul_is_degrees' : True}, # And given in degrees
-                    'Absolute Paths': {
-                        'geoid_path' : GEOID_PATH,
-                        #'geoid_path' : 'data/world/geoids/egm08_25.gtx',
-                        'dem_path' : DEM_PATH,
-                        'orthomosaic_reference_folder' : os.path.join(specim_mission_folder, "orthomosaic"),
-                        'ref_ortho_reshaped' : os.path.join(DATA_DIR, "Intermediate", "RefOrthoResampled"),
-                        'ref_gcp_path' : os.path.join(DATA_DIR, "Intermediate", "gcp.csv"),
-                        'calib_file_coreg' : os.path.join(DATA_DIR, "Output", "HSI_coreg.xml"),
-                        # (above) The georeferencing allows processing using norwegian geoid NN2000 and worldwide EGM2008. Also, use of seafloor terrain models are supported. '
-                        # At the moment refractive ray tracing is not implemented, but it could be relatively easy by first ray tracing with geoid+tide, 
-                        # and then ray tracing from water
-                        #'tide_path' : 'D:/HyperspectralDataAll/HI/2022-08-31-060000-Remoy-Specim/Input/tidevann_nn2000_NMA.txt'
-                        },
-                    
-                    # If coregistration is done, then the data must be stored after processing somewhere
-                    'HDF.coregistration': {
-                            'position_ecef': 'processed/coreg/position_ecef',
-                            'quaternion_ecef' : 'processed/coreg/quaternion_ecef'
-                        }
-                    
-    }
-
-    if TERRAIN_TYPE == 'geoid':
-        custom_config['Absolute Paths']['geoid_path'] = GEOID_PATH
-        #'geoid_path' : 'data/world/geoids/egm08_25.gtx'
-    elif TERRAIN_TYPE == 'dem_file':
-        custom_config['Absolute Paths']['dem_path'] = DEM_PATH
-
-    
-    # No need to orthorectify the data cube initially when coregistration with RGB composites is done
-    if do_coreg:
-        custom_config['Orthorectification']['resample_rgb_only'] = True
-    
-    # 
-    if fast_mode:
-        custom_config['Orthorectification']['resample_rgb_only'] = True
-        custom_config['Orthorectification']['resolutionhyperspectralmosaic'] = 1
-
-
-    # Customizes the config file according to settings
-    customize_config(config_path=config_file_mission, dict_custom=custom_config)
-
-
-    config = configparser.ConfigParser()
-    config.read(config_file_mission)
-
-    # This function parses raw specim data including (spectral, radiometric, geometric) calibrations and nav data
-    # into an h5 file. The nav data is written to "raw/nav/" subfolders, whereas hyperspectral data and calibration data 
-    # written to "processed/hyperspectral/" and "processed/calibration/" subfolders
-    """specim_parsing_utils.main(config=config,
-                              config_specim=config_specim_preprocess)"""
-    
-    """# Time interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
-    config = parsing_utils.export_pose(config_file_mission)
-    
-    # Formats model to triangular mesh and an earth centered earth fixed / geocentric coordinate system
-    parsing_utils.export_model(config_file_mission)
-
-    # Commenting out the georeference step is fine if it has been done
-
-    
-    ## Visualize the data 3D photo model from RGB images and the time-resolved positions/orientations
-    if ENABLE_VISUALIZE:
-        visualize.show_mesh_camera(config, show_mesh = True, show_pose = True, ref_frame='ENU')
-
-    # Georeference the line scans of the hyperspectral imager. Utilizes parsed data
-    georeference.main(config_file_mission)
-
-    orthorectification.main(config_file_mission)"""
-    # The coregistration compares to the reference and optimizes geometric parameters which are used to re-georeference.
-    if do_coreg:
-        # Optional: coregistration
-        # Match RGB composite to reference, find features and following data, ground control point (gcp) list, for each feature pair:
-        # reference point 3D (from reference), position/orientation of vehicle (using resampled time) and pixel coordinate (using resampled pixel coordinate)
-        #coregistration.main(config_file_mission, mode='compare')
-
-        # The gcp list allows reprojecting reference points and evaluate the reprojection error,
-        # which is used to optimize static geometric parameters (e.g. boresight, camera model...) or dynamic geometric parameters (time-varying nav errors).
-        # Settings are currently in coregistration script
-        #coregistration.main(config_file_mission, mode='calibrate')
-
-        # The final orthorectification can be conducted on the datacube too
-        custom_config['Orthorectification']['resample_rgb_only'] = True
-
-        # Georeference with coregistred parameters
-        georeference.main(config_file_mission, use_coreg_param=True)
-
-        orthorectification.main(config_file_mission)
-
-
-
-if __name__ == "__main__":
-    # Select a recording folder on drive
-    specim_mission_folder = os.path.join(base_fp, r"Specim/Missions/2022-08-31-Remoy/remoy_202208310800_ntnu_hyperspectral_74m")
-    
-    # Globally accessible files:
-    geoid_path = os.path.join(home, "VsCodeProjects/gref4hsi/data/world/geoids/egm08_25.gtx")
-    config_template_path = os.path.join(home, "VsCodeProjects/gref4hsi/data/config_examples/configuration_specim.ini")
-    lab_calibration_path = os.path.join(base_fp, "Specim/Lab_Calibrations")
-    
-    # The configuration file
-    config_yaml = os.path.join(specim_mission_folder, "config.seabee.yaml")
+# Standard python library
+import configparser
+import sys
+import os
+import argparse
+from collections import namedtuple
+import pathlib
+import yaml
+
+if os.name == 'nt':
+    # Windows OS
+    base_fp = 'D:'
+    home = 'C:/Users/haavasl'
+elif os.name == 'posix':
+    # This Unix-like systems inl. Mac and fLinux
+    base_fp = '/media/haavasl/Expansion'
+    home = '/home/haavasl'
+
+# Use this if working with the github repo to do quick changes to the module
+module_path = os.path.join(home, 'VsCodeProjects/gref4hsi/')
+if module_path not in sys.path:
+    sys.path.append(module_path)
+
+# Local resources
+from gref4hsi.scripts import georeference
+from gref4hsi.scripts import orthorectification
+from gref4hsi.scripts import coregistration
+from gref4hsi.utils import parsing_utils, specim_parsing_utils
+from gref4hsi.utils import visualize
+from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths, customize_config
+
+
+import numpy as np
+
+"""
+This script is meant to be used for testing the processing pipeline of airborne HI data from the Specim AFX10 instrument.
+"""
+
+# Make it simple to swap when working a bit on windows and a bit on Linux
+
+
+
+def main(config_yaml, specim_mission_folder, geoid_path, config_template_path, lab_calibration_path, fast_mode = False):
+    # Read flight-specific yaml file
+    with open(config_yaml, 'r') as file:  
+        config_data = yaml.safe_load(file)
+    
+    
+    # assigning the arguments to variables for simple backwards compatibility
+    SPECIM_MISSION_FOLDER = specim_mission_folder
+    EPSG_CODE = config_data['mission_epsg']
+    RESOLUTION_ORTHOMOSAIC = config_data['resolution_orthomosaic']
+    CALIBRATION_DIRECTORY = lab_calibration_path
+    
+    
+    dem_fold = os.path.join(specim_mission_folder, "dem")
+
+    if not os.path.exists(dem_fold):
+        print('DEM folder does not exist so Geoid is used as terrain instead')
+        TERRAIN_TYPE = "geoid"
+    else:
+        if not os.listdir(dem_fold):
+            #print(f"The folder '{dem_fold}' is empty so Geoid is used as terrain instead.")
+            TERRAIN_TYPE = "geoid"
+        else:
+            # If there is a folder and it is not empty
+            # Find the only file that is there
+            files = [f for f in os.listdir(dem_fold) if f not in ('.', '..')]
+            DEM_PATH = os.path.join(dem_fold, files[0])
+            #print(f"The file '{DEM_PATH}' is used as terrain.")
+            TERRAIN_TYPE = "dem_file"
+            print(DEM_PATH)
+    
+    
+    # Do coregistration if there is an orthomosaic to compare under "orthomosaic"
+    #do_coreg = True
+    ortho_ref_fold = os.path.join(specim_mission_folder, "orthomosaic")
+
+    if not os.path.exists(ortho_ref_fold):
+        print('Coregistration is not done, as there was no reference orthomosaic')
+        
+    else:
+        if not os.listdir(ortho_ref_fold):
+            print('Coregistration is not done, as there was no reference orthomosaic')
+        else:
+            # If there is a folder and it is not empty
+            # Find the only file that is there
+<<<<<<< HEAD:gref4hsi/tests/specim_process.py
+            ortho_ref_file = [f for f in os.listdir(ortho_ref_fold) if f not in ('.', '..')][0]
+=======
+            ortho_ref_file = [f for f in os.listdir(ortho_ref_fold) if f.endswith('tif')][0]
+>>>>>>> c05ae5e3c6473d21ada475ba36c3dffc7aca204b:gref4hsi/tests/test_main_specim.py
+            do_coreg = True
+            print(f"The file '{ortho_ref_file}' is used as as reference orthomosaic.")
+            
+    
+    
+    GEOID_PATH = geoid_path
+
+    # Settings associated with preprocessing of data from Specim Proprietary data to pipeline-compatible data
+    SettingsPreprocess = namedtuple('SettingsPreprocessing', ['dtype_datacube', 
+                                                                            'lines_per_chunk', 
+                                                                            'specim_raw_mission_dir',
+                                                                            'cal_dir',
+                                                                            'reformatted_missions_dir',
+                                                                            'rotation_matrix_hsi_to_body',
+                                                                            'translation_body_to_hsi',
+                                                                            'config_file_name'])
+
+    config_specim_preprocess = SettingsPreprocess(dtype_datacube = np.float32, # The data type for the datacube
+                                lines_per_chunk= 8000,  # Raw datacube is chunked into this many lines. GB_per_chunk = lines_per_chunk*n_pixels*n_bands*4 bytes
+                                specim_raw_mission_dir = SPECIM_MISSION_FOLDER, # Folder containing several mission
+                                cal_dir = CALIBRATION_DIRECTORY,  # Calibration directory holding all calibrations at all binning levels
+                                reformatted_missions_dir = os.path.join(SPECIM_MISSION_FOLDER, 'processed'), # The fill value for empty cells (select values not occcuring in cube or ancillary data)
+                                rotation_matrix_hsi_to_body = np.array([[0, 1, 0],
+                                                                        [-1, 0, 0],
+                                                                        [0, 0, 1]]), # Rotation matrix R rotating so that vec_body = R*vec_hsi.
+                                translation_body_to_hsi = np.array([0, 0, 0]), # Translation t so that vec_body_to_object = vec_hsi_to_object + t
+                                # For large files, RAM issues could be a concern. For rectified files exeeding this size, data is written chunk-wize to a memory map.
+                                config_file_name = 'configuration.ini')
+
+
+
+    # Where to place the config
+    DATA_DIR = config_specim_preprocess.reformatted_missions_dir
+    config_file_mission = os.path.join(DATA_DIR, 'configuration.ini')
+
+
+    # Set the data directory for the mission, and create empty folder structure
+    prepend_data_dir_to_relative_paths(config_path=config_template_path, DATA_DIR=DATA_DIR)
+
+    # Non-default settings
+    custom_config = {'General':
+                        {'mission_dir': DATA_DIR,
+                        'model_export_type': TERRAIN_TYPE, # Ray trace onto geoid
+                        'max_ray_length': 150}, # Max distance in meters from spectral imager to seafloor. Specim does not fly higher
+
+                    'Coordinate Reference Systems':
+                        {'proj_epsg' : EPSG_CODE, # The projected CRS UTM 32, common on mainland norway
+                        'geocsc_epsg_export' : 4978, # 3D cartesian system for earth consistent with GPS frame (but inconsistent with eurasian techtonic plate)
+                        'dem_epsg' : EPSG_CODE, # (Optional) If you have a DEM this can be used
+                        'pos_epsg_orig' : 4978}, # The CRS of the positioning data we deliver to the georeferencing
+
+                    'Orthorectification':
+                        {'resample_rgb_only': True, # True can be good choice for speed during DEV
+                         'resample_ancillary': True,
+                        'resolutionhyperspectralmosaic': RESOLUTION_ORTHOMOSAIC, # Resolution in m
+                        'raster_transform_method': 'north_east'}, # North-east oriented rasters.
+                    
+                    'HDF.raw_nav': {
+                        'rotation_reference_type' : 'eul_ZYX', # The vehicle orientations are given in Yaw, Pitch, Roll from the NAV system
+                        'is_global_rot' : False, # The vehicles orientations from NAV system are Yaw, Pitch, Roll
+                        'eul_is_degrees' : True}, # And given in degrees
+                    'Absolute Paths': {
+                        'geoid_path' : GEOID_PATH,
+                        #'geoid_path' : 'data/world/geoids/egm08_25.gtx',
+                        'dem_path' : DEM_PATH,
+                        'orthomosaic_reference_folder' : os.path.join(specim_mission_folder, "orthomosaic"),
+                        'ref_ortho_reshaped' : os.path.join(DATA_DIR, "Intermediate", "RefOrthoResampled"),
+                        'ref_gcp_path' : os.path.join(DATA_DIR, "Intermediate", "gcp.csv"),
+                        'calib_file_coreg' : os.path.join(DATA_DIR, "Output", "HSI_coreg.xml"),
+                        # (above) The georeferencing allows processing using norwegian geoid NN2000 and worldwide EGM2008. Also, use of seafloor terrain models are supported. '
+                        # At the moment refractive ray tracing is not implemented, but it could be relatively easy by first ray tracing with geoid+tide, 
+                        # and then ray tracing from water
+                        #'tide_path' : 'D:/HyperspectralDataAll/HI/2022-08-31-060000-Remoy-Specim/Input/tidevann_nn2000_NMA.txt'
+                        },
+                    
+                    # If coregistration is done, then the data must be stored after processing somewhere
+                    'HDF.coregistration': {
+                            'position_ecef': 'processed/coreg/position_ecef',
+                            'quaternion_ecef' : 'processed/coreg/quaternion_ecef'
+                        }
+                    
+    }
+
+    if TERRAIN_TYPE == 'geoid':
+        custom_config['Absolute Paths']['geoid_path'] = GEOID_PATH
+        #'geoid_path' : 'data/world/geoids/egm08_25.gtx'
+    elif TERRAIN_TYPE == 'dem_file':
+        custom_config['Absolute Paths']['dem_path'] = DEM_PATH
+
+    
+    # No need to orthorectify the data cube initially when coregistration with RGB composites is done
+    if do_coreg:
+        custom_config['Orthorectification']['resample_rgb_only'] = True
+    
+    # 
+    if fast_mode:
+        custom_config['Orthorectification']['resample_rgb_only'] = True
+        custom_config['Orthorectification']['resolutionhyperspectralmosaic'] = 1
+
+
+    # Customizes the config file according to settings
+    customize_config(config_path=config_file_mission, dict_custom=custom_config)
+
+
+    config = configparser.ConfigParser()
+    config.read(config_file_mission)
+
+    # This function parses raw specim data including (spectral, radiometric, geometric) calibrations and nav data
+    # into an h5 file. The nav data is written to "raw/nav/" subfolders, whereas hyperspectral data and calibration data 
+    # written to "processed/hyperspectral/" and "processed/calibration/" subfolders
+<<<<<<< HEAD:gref4hsi/tests/specim_process.py
+    specim_parsing_utils.main(config=config,
+                              config_specim=config_specim_preprocess)"""
+    
+    """# Time interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
+    config = parsing_utils.export_pose(config_file_mission)
+=======
+    model_path = config['Absolute Paths']['model_path']
+    
+    # If this folder exists, there is no need to repeat this step
+    """specim_parsing_utils.main(config=config,
+                                  config_specim=config_specim_preprocess)
+    
+    # Time interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
+    parsing_utils.export_pose(config_file_mission)
+>>>>>>> c05ae5e3c6473d21ada475ba36c3dffc7aca204b:gref4hsi/tests/test_main_specim.py
+    
+    if not os.path.exists(model_path):
+        parsing_utils.export_model(config_file_mission)
+
+    # Commenting out the georeference step is fine if it has been done
+
+    
+    ## Visualize the data 3D photo model from RGB images and the time-resolved positions/orientations
+<<<<<<< HEAD:gref4hsi/tests/specim_process.py
+    if ENABLE_VISUALIZE:
+        visualize.show_mesh_camera(config, show_mesh = True, show_pose = True, ref_frame='ENU')
+=======
+    
+>>>>>>> c05ae5e3c6473d21ada475ba36c3dffc7aca204b:gref4hsi/tests/test_main_specim.py
+
+    # Georeference the line scans of the hyperspectral imager.
+    georeference.main(config_file_mission)
+
+    orthorectification.main(config_file_mission)"""
+    # The coregistration compares to the reference and optimizes geometric parameters which are used to re-georeference.
+    if do_coreg:
+        # Optional: coregistration
+        # Match RGB composite to reference, find features and following data, ground control point (gcp) list, for each feature pair:
+        # reference point 3D (from reference), position/orientation of vehicle (using resampled time) and pixel coordinate (using resampled pixel coordinate)
+<<<<<<< HEAD:gref4hsi/tests/specim_process.py
+        #coregistration.main(config_file_mission, mode='compare')
+=======
+        """coregistration.main(config_file_mission, mode='compare')
+>>>>>>> c05ae5e3c6473d21ada475ba36c3dffc7aca204b:gref4hsi/tests/test_main_specim.py
+
+        # The gcp list allows reprojecting reference points and evaluate the reprojection error,
+        # which is used to optimize static geometric parameters (e.g. boresight, camera model...) or dynamic geometric parameters (time-varying nav errors).
+        # Settings are currently in coregistration script
+<<<<<<< HEAD:gref4hsi/tests/specim_process.py
+        #coregistration.main(config_file_mission, mode='calibrate')
+=======
+        coregistration.main(config_file_mission, mode='calibrate')"""
+>>>>>>> c05ae5e3c6473d21ada475ba36c3dffc7aca204b:gref4hsi/tests/test_main_specim.py
+
+        # The final orthorectification can be conducted on the datacube too
+        custom_config['Orthorectification']['resample_rgb_only'] = False
+
+        # No impact unless you rewrite the config
+        customize_config(config_path=config_file_mission, dict_custom=custom_config)
+
+        
+
+        # Georeference with coregistred parameters
+        georeference.main(config_file_mission, use_coreg_param=True)
+        
+        # And orthorectify
+        orthorectification.main(config_file_mission)
+
+
+if __name__ == "__main__":
+    # Select a recording folder on drive
+    specim_mission_folder = os.path.join(base_fp, r"Specim/Missions/2022-08-31-Remoy/remoy_202208311040_ntnu_hyperspectral_74m")
+    
+    # Globally accessible files:
+    geoid_path = os.path.join(home, "VsCodeProjects/gref4hsi/data/world/geoids/egm08_25.gtx")
+    config_template_path = os.path.join(home, "VsCodeProjects/gref4hsi/data/config_examples/configuration_specim.ini")
+    lab_calibration_path = os.path.join(base_fp, "Specim/Lab_Calibrations")
+    
+    # The configuration file
+    config_yaml = os.path.join(specim_mission_folder, "config.seabee.yaml")
     main(str(config_yaml), str(specim_mission_folder), geoid_path, config_template_path, lab_calibration_path)
```

### Comparing `gref4hsi-0.2.1/gref4hsi/tests/test_main_hi.py` & `gref4hsi-0.2.2/gref4hsi/tests/test_main_hi.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# Standard python library
-import configparser
-import sys
-import os
-
-# Local resources
-from scripts import georeference
-from scripts import orthorectification
-from utils import parsing_utils
-from gref4hsi.utils import visualize
-from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths
-
-"""
-This script is meant to be used for testing the processing pipeline of airborne HI data.
-""" 
-DATA_DIR = 'D:/HyperspectralDataAll/HI/2022-05-27-053505-NyAlesund-Flight8/'
-config_file = DATA_DIR + 'configuration.ini'
-# Set the data directory for the mission (locally where the data is stored)
-
-prepend_data_dir_to_relative_paths(config_path=config_file, DATA_DIR=DATA_DIR)
-
-config = configparser.ConfigParser()
-config.read(config_file)
-
-def main():
-    ## Extract pose.csv and model.ply data from Agisoft Metashape (photogrammetry software) through API.
-    ## Fails if you do not have an appropriate project.
-
-    # The minimum for georeferencing is to parse 1) Mesh model and 2) The pose of the reference
-    
-    #config = parsing_utils.export_pose(config_file)
-
-    config = configparser.ConfigParser()
-
-    config.read(config_file)
-
-    # Exports model
-    #parsing_utils.export_model(config_file)
-
-    ## Visualize the data 3D photo model from RGB images and the time-resolved positions/orientations
-    
-    #visualize.show_mesh_camera(config, show_mesh = True, show_pose = True)
-
-    # Georeference the line scans of the hyperspectral imager. Utilizes parsed data
-    
-    #georeference.main(config_file)
-
-    orthorectification.main(config_file)
-
-    #print('')
-
-
-if __name__ == "__main__":
+# Standard python library
+import configparser
+import sys
+import os
+
+# Local resources
+from scripts import georeference
+from scripts import orthorectification
+from utils import parsing_utils
+from gref4hsi.utils import visualize
+from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths
+
+"""
+This script is meant to be used for testing the processing pipeline of airborne HI data.
+""" 
+DATA_DIR = 'D:/HyperspectralDataAll/HI/2022-05-27-053505-NyAlesund-Flight8/'
+config_file = DATA_DIR + 'configuration.ini'
+# Set the data directory for the mission (locally where the data is stored)
+
+prepend_data_dir_to_relative_paths(config_path=config_file, DATA_DIR=DATA_DIR)
+
+config = configparser.ConfigParser()
+config.read(config_file)
+
+def main():
+    ## Extract pose.csv and model.ply data from Agisoft Metashape (photogrammetry software) through API.
+    ## Fails if you do not have an appropriate project.
+
+    # The minimum for georeferencing is to parse 1) Mesh model and 2) The pose of the reference
+    
+    #config = parsing_utils.export_pose(config_file)
+
+    config = configparser.ConfigParser()
+
+    config.read(config_file)
+
+    # Exports model
+    #parsing_utils.export_model(config_file)
+
+    ## Visualize the data 3D photo model from RGB images and the time-resolved positions/orientations
+    
+    #visualize.show_mesh_camera(config, show_mesh = True, show_pose = True)
+
+    # Georeference the line scans of the hyperspectral imager. Utilizes parsed data
+    
+    #georeference.main(config_file)
+
+    orthorectification.main(config_file)
+
+    #print('')
+
+
+if __name__ == "__main__":
     main()
```

### Comparing `gref4hsi-0.2.1/gref4hsi/tests/test_multi_ray_trace.py` & `gref4hsi-0.2.2/gref4hsi/tests/test_multi_ray_trace.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import time
-
-import numpy as np
-import pyvista as pv
-from pykdtree.kdtree import KDTree
-from pyvista import examples
-
-# Record the start time
-start_time = time.time()
-
-# Load data
-data = examples.load_random_hills()
-data.translate((10, 10, 10))
-
-# Create triangular plane (vertices [10, 0, 0], [0, 10, 0], [0, 0, 10])
-size = 10
-vertices = np.array([[size, 0, 0], [0, size, 0], [0, 0, size]])
-face = np.array([3, 0, 1, 2])
-
-planes = pv.PolyData(vertices, face)
-
-# Subdivide plane so we have multiple points to project to
-planes = planes.subdivide(8)
-
-# Get origins and normals
-origins = planes.cell_centers().points
-normals = planes.compute_normals(cell_normals=True, point_normals=False)["Normals"]
-
-# Vectorized Ray trace
-points, pt_inds, cell_inds = data.multi_ray_trace(
-    origins, normals
-)  # Must have rtree, trimesh, and pyembree installed
-
-# Filter based on distance threshold, if desired (mimics VTK ray_trace behavior)
-# threshold = 10  # Some threshold distance
-# distances = np.linalg.norm(origins[inds] - points, ord=2, axis=1)
-# inds = inds[distances <= threshold]
-
-tree = KDTree(data.points.astype(np.double))
-_, data_inds = tree.query(points)
-
-elevations = data.point_data["Elevation"][data_inds]
-
-# Mask points on planes
-planes.cell_data["Elevation"] = np.zeros((planes.n_cells,))
-planes.cell_data["Elevation"][pt_inds] = elevations
-planes.set_active_scalars("Elevation")  # Probably not necessary, but just in case
-
-# Create axes
-axis_length = 20
-tip_length = 0.25 / axis_length * 3
-tip_radius = 0.1 / axis_length * 3
-shaft_radius = 0.05 / axis_length * 3
-x_axis = pv.Arrow(
-    direction=(axis_length, 0, 0),
-    tip_length=tip_length,
-    tip_radius=tip_radius,
-    shaft_radius=shaft_radius,
-    scale="auto",
-)
-y_axis = pv.Arrow(
-    direction=(0, axis_length, 0),
-    tip_length=tip_length,
-    tip_radius=tip_radius,
-    shaft_radius=shaft_radius,
-    scale="auto",
-)
-z_axis = pv.Arrow(
-    direction=(0, 0, axis_length),
-    tip_length=tip_length,
-    tip_radius=tip_radius,
-    shaft_radius=shaft_radius,
-    scale="auto",
-)
-x_label = pv.PolyData([axis_length, 0, 0])
-y_label = pv.PolyData([0, axis_length, 0])
-z_label = pv.PolyData([0, 0, axis_length])
-x_label.point_data["label"] = [
-    "x",
-]
-y_label.point_data["label"] = [
-    "y",
-]
-z_label.point_data["label"] = [
-    "z",
-]
-
-
-# Calculate the elapsed time
-elapsed_time = time.time() - start_time
-
-# Print the elapsed time in seconds
-print(f"Elapsed Time: {elapsed_time:.2f} seconds")
-
-if elapsed_time < 2:
-    print('Test run took less than 2 seconds ==> Test passed')
-else:
-    print('Test run took more than 2 seconds ==> Test failed')
-# Plot results
-p = pv.Plotter()
-p.add_mesh(x_axis, color="r")
-p.add_point_labels(x_label, "label", show_points=False, font_size=24)
-p.add_mesh(y_axis, color="r")
-p.add_point_labels(y_label, "label", show_points=False, font_size=24)
-p.add_mesh(z_axis, color="r")
-p.add_point_labels(z_label, "label", show_points=False, font_size=24)
-p.add_mesh(data)
-p.add_mesh(planes)
+import time
+
+import numpy as np
+import pyvista as pv
+from pykdtree.kdtree import KDTree
+from pyvista import examples
+
+# Record the start time
+start_time = time.time()
+
+# Load data
+data = examples.load_random_hills()
+data.translate((10, 10, 10))
+
+# Create triangular plane (vertices [10, 0, 0], [0, 10, 0], [0, 0, 10])
+size = 10
+vertices = np.array([[size, 0, 0], [0, size, 0], [0, 0, size]])
+face = np.array([3, 0, 1, 2])
+
+planes = pv.PolyData(vertices, face)
+
+# Subdivide plane so we have multiple points to project to
+planes = planes.subdivide(8)
+
+# Get origins and normals
+origins = planes.cell_centers().points
+normals = planes.compute_normals(cell_normals=True, point_normals=False)["Normals"]
+
+# Vectorized Ray trace
+points, pt_inds, cell_inds = data.multi_ray_trace(
+    origins, normals
+)  # Must have rtree, trimesh, and pyembree installed
+
+# Filter based on distance threshold, if desired (mimics VTK ray_trace behavior)
+# threshold = 10  # Some threshold distance
+# distances = np.linalg.norm(origins[inds] - points, ord=2, axis=1)
+# inds = inds[distances <= threshold]
+
+tree = KDTree(data.points.astype(np.double))
+_, data_inds = tree.query(points)
+
+elevations = data.point_data["Elevation"][data_inds]
+
+# Mask points on planes
+planes.cell_data["Elevation"] = np.zeros((planes.n_cells,))
+planes.cell_data["Elevation"][pt_inds] = elevations
+planes.set_active_scalars("Elevation")  # Probably not necessary, but just in case
+
+# Create axes
+axis_length = 20
+tip_length = 0.25 / axis_length * 3
+tip_radius = 0.1 / axis_length * 3
+shaft_radius = 0.05 / axis_length * 3
+x_axis = pv.Arrow(
+    direction=(axis_length, 0, 0),
+    tip_length=tip_length,
+    tip_radius=tip_radius,
+    shaft_radius=shaft_radius,
+    scale="auto",
+)
+y_axis = pv.Arrow(
+    direction=(0, axis_length, 0),
+    tip_length=tip_length,
+    tip_radius=tip_radius,
+    shaft_radius=shaft_radius,
+    scale="auto",
+)
+z_axis = pv.Arrow(
+    direction=(0, 0, axis_length),
+    tip_length=tip_length,
+    tip_radius=tip_radius,
+    shaft_radius=shaft_radius,
+    scale="auto",
+)
+x_label = pv.PolyData([axis_length, 0, 0])
+y_label = pv.PolyData([0, axis_length, 0])
+z_label = pv.PolyData([0, 0, axis_length])
+x_label.point_data["label"] = [
+    "x",
+]
+y_label.point_data["label"] = [
+    "y",
+]
+z_label.point_data["label"] = [
+    "z",
+]
+
+
+# Calculate the elapsed time
+elapsed_time = time.time() - start_time
+
+# Print the elapsed time in seconds
+print(f"Elapsed Time: {elapsed_time:.2f} seconds")
+
+if elapsed_time < 2:
+    print('Test run took less than 2 seconds ==> Test passed')
+else:
+    print('Test run took more than 2 seconds ==> Test failed')
+# Plot results
+p = pv.Plotter()
+p.add_mesh(x_axis, color="r")
+p.add_point_labels(x_label, "label", show_points=False, font_size=24)
+p.add_mesh(y_axis, color="r")
+p.add_point_labels(y_label, "label", show_points=False, font_size=24)
+p.add_mesh(z_axis, color="r")
+p.add_point_labels(z_label, "label", show_points=False, font_size=24)
+p.add_mesh(data)
+p.add_mesh(planes)
 p.show()
```

### Comparing `gref4hsi-0.2.1/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py` & `gref4hsi-0.2.2/gref4hsi/tests/test_multi_ray_trace_no_pyembree.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-import time
-
-import numpy as np
-import pyvista as pv
-from pykdtree.kdtree import KDTree
-from pyvista import examples
-import trimesh
-
-# Record the start time
-start_time = time.time()
-
-# Load data
-data = examples.load_random_hills()
-data.translate((10, 10, 10))
-
-
-
-
-# Create triangular plane (vertices [10, 0, 0], [0, 10, 0], [0, 0, 10])
-size = 10
-vertices = np.array([[size, 0, 0], [0, size, 0], [0, 0, size]])
-face = np.array([3, 0, 1, 2])
-
-planes = pv.PolyData(vertices, face)
-
-# Subdivide plane so we have multiple points to project to
-planes = planes.subdivide(8)
-
-# Get origins and normals
-origins = planes.cell_centers().points
-normals = planes.compute_normals(cell_normals=True, point_normals=False)["Normals"]
-
-# Convert faces to nx3 format
-faces = data.faces.reshape(-1, 3)
-
-# Convert PolyData to trimesh.Trimesh
-data_mesh = trimesh.Trimesh(vertices=data.points, faces=faces)
-
-# Vectorized Ray trace
-"""points, pt_inds, cell_inds = data.multi_ray_trace(
-    origins, normals
-)"""  # Must have rtree, trimesh, and pyembree installed
-
-
-ray_mesh_intersector = trimesh.ray.ray_pyembree.RayMeshIntersector(geometry=data_mesh)
-
-# Perform ray tracing using trimesh.ray.intersects_id
-cell_inds, pt_inds, points = ray_mesh_intersector.intersects_id(ray_origins=origins,  
-                                                                ray_directions=normals, 
-                                                                multiple_hits=False,
-                                                                return_locations=True)
-
-
-# Filter based on distance threshold, if desired (mimics VTK ray_trace behavior)
-# threshold = 10  # Some threshold distance
-# distances = np.linalg.norm(origins[inds] - points, ord=2, axis=1)
-# inds = inds[distances <= threshold]
-
-tree = KDTree(data.points.astype(np.double))
-_, data_inds = tree.query(points)
-
-elevations = data.point_data["Elevation"][data_inds]
-
-# Mask points on planes
-planes.cell_data["Elevation"] = np.zeros((planes.n_cells,))
-planes.cell_data["Elevation"][pt_inds] = elevations
-planes.set_active_scalars("Elevation")  # Probably not necessary, but just in case
-
-# Create axes
-axis_length = 20
-tip_length = 0.25 / axis_length * 3
-tip_radius = 0.1 / axis_length * 3
-shaft_radius = 0.05 / axis_length * 3
-x_axis = pv.Arrow(
-    direction=(axis_length, 0, 0),
-    tip_length=tip_length,
-    tip_radius=tip_radius,
-    shaft_radius=shaft_radius,
-    scale="auto",
-)
-y_axis = pv.Arrow(
-    direction=(0, axis_length, 0),
-    tip_length=tip_length,
-    tip_radius=tip_radius,
-    shaft_radius=shaft_radius,
-    scale="auto",
-)
-z_axis = pv.Arrow(
-    direction=(0, 0, axis_length),
-    tip_length=tip_length,
-    tip_radius=tip_radius,
-    shaft_radius=shaft_radius,
-    scale="auto",
-)
-x_label = pv.PolyData([axis_length, 0, 0])
-y_label = pv.PolyData([0, axis_length, 0])
-z_label = pv.PolyData([0, 0, axis_length])
-x_label.point_data["label"] = [
-    "x",
-]
-y_label.point_data["label"] = [
-    "y",
-]
-z_label.point_data["label"] = [
-    "z",
-]
-
-
-# Calculate the elapsed time
-elapsed_time = time.time() - start_time
-
-# Print the elapsed time in seconds
-print(f"Elapsed Time: {elapsed_time:.2f} seconds")
-
-if elapsed_time < 2:
-    print('Test run took less than 2 seconds ==> Test passed')
-else:
-    print('Test run took more than 2 seconds ==> Test failed')
-# Plot results
-p = pv.Plotter()
-p.add_mesh(x_axis, color="r")
-p.add_point_labels(x_label, "label", show_points=False, font_size=24)
-p.add_mesh(y_axis, color="r")
-p.add_point_labels(y_label, "label", show_points=False, font_size=24)
-p.add_mesh(z_axis, color="r")
-p.add_point_labels(z_label, "label", show_points=False, font_size=24)
-p.add_mesh(data)
-p.add_mesh(planes)
+import time
+
+import numpy as np
+import pyvista as pv
+from pykdtree.kdtree import KDTree
+from pyvista import examples
+import trimesh
+
+# Record the start time
+start_time = time.time()
+
+# Load data
+data = examples.load_random_hills()
+data.translate((10, 10, 10))
+
+
+
+
+# Create triangular plane (vertices [10, 0, 0], [0, 10, 0], [0, 0, 10])
+size = 10
+vertices = np.array([[size, 0, 0], [0, size, 0], [0, 0, size]])
+face = np.array([3, 0, 1, 2])
+
+planes = pv.PolyData(vertices, face)
+
+# Subdivide plane so we have multiple points to project to
+planes = planes.subdivide(8)
+
+# Get origins and normals
+origins = planes.cell_centers().points
+normals = planes.compute_normals(cell_normals=True, point_normals=False)["Normals"]
+
+# Convert faces to nx3 format
+faces = data.faces.reshape(-1, 3)
+
+# Convert PolyData to trimesh.Trimesh
+data_mesh = trimesh.Trimesh(vertices=data.points, faces=faces)
+
+# Vectorized Ray trace
+"""points, pt_inds, cell_inds = data.multi_ray_trace(
+    origins, normals
+)"""  # Must have rtree, trimesh, and pyembree installed
+
+
+ray_mesh_intersector = trimesh.ray.ray_pyembree.RayMeshIntersector(geometry=data_mesh)
+
+# Perform ray tracing using trimesh.ray.intersects_id
+cell_inds, pt_inds, points = ray_mesh_intersector.intersects_id(ray_origins=origins,  
+                                                                ray_directions=normals, 
+                                                                multiple_hits=False,
+                                                                return_locations=True)
+
+
+# Filter based on distance threshold, if desired (mimics VTK ray_trace behavior)
+# threshold = 10  # Some threshold distance
+# distances = np.linalg.norm(origins[inds] - points, ord=2, axis=1)
+# inds = inds[distances <= threshold]
+
+tree = KDTree(data.points.astype(np.double))
+_, data_inds = tree.query(points)
+
+elevations = data.point_data["Elevation"][data_inds]
+
+# Mask points on planes
+planes.cell_data["Elevation"] = np.zeros((planes.n_cells,))
+planes.cell_data["Elevation"][pt_inds] = elevations
+planes.set_active_scalars("Elevation")  # Probably not necessary, but just in case
+
+# Create axes
+axis_length = 20
+tip_length = 0.25 / axis_length * 3
+tip_radius = 0.1 / axis_length * 3
+shaft_radius = 0.05 / axis_length * 3
+x_axis = pv.Arrow(
+    direction=(axis_length, 0, 0),
+    tip_length=tip_length,
+    tip_radius=tip_radius,
+    shaft_radius=shaft_radius,
+    scale="auto",
+)
+y_axis = pv.Arrow(
+    direction=(0, axis_length, 0),
+    tip_length=tip_length,
+    tip_radius=tip_radius,
+    shaft_radius=shaft_radius,
+    scale="auto",
+)
+z_axis = pv.Arrow(
+    direction=(0, 0, axis_length),
+    tip_length=tip_length,
+    tip_radius=tip_radius,
+    shaft_radius=shaft_radius,
+    scale="auto",
+)
+x_label = pv.PolyData([axis_length, 0, 0])
+y_label = pv.PolyData([0, axis_length, 0])
+z_label = pv.PolyData([0, 0, axis_length])
+x_label.point_data["label"] = [
+    "x",
+]
+y_label.point_data["label"] = [
+    "y",
+]
+z_label.point_data["label"] = [
+    "z",
+]
+
+
+# Calculate the elapsed time
+elapsed_time = time.time() - start_time
+
+# Print the elapsed time in seconds
+print(f"Elapsed Time: {elapsed_time:.2f} seconds")
+
+if elapsed_time < 2:
+    print('Test run took less than 2 seconds ==> Test passed')
+else:
+    print('Test run took more than 2 seconds ==> Test failed')
+# Plot results
+p = pv.Plotter()
+p.add_mesh(x_axis, color="r")
+p.add_point_labels(x_label, "label", show_points=False, font_size=24)
+p.add_mesh(y_axis, color="r")
+p.add_point_labels(y_label, "label", show_points=False, font_size=24)
+p.add_mesh(z_axis, color="r")
+p.add_point_labels(z_label, "label", show_points=False, font_size=24)
+p.add_mesh(data)
+p.add_mesh(planes)
 p.show()
```

### Comparing `gref4hsi-0.2.1/gref4hsi/utils/colours.py` & `gref4hsi-0.2.2/gref4hsi/utils/colours.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,53 @@
-
-import numpy as np
-
-import cv2 as cv
-
-class Image():
-    def __init__(self, array):
-        """Takes in an image array with nxmx3 of type uint8"""
-        self.image_array = array
-
-    def clahe_adjustment(self):
-        clahe = cv.createCLAHE(clipLimit=2.0, tileGridSize=(8, 8))
-        img = self.image_array
-        R = clahe.apply(img[:, :, 0]).reshape((img.shape[0], img.shape[1], 1))
-        G = clahe.apply(img[:, :, 1]).reshape((img.shape[0], img.shape[1], 1))
-        B = clahe.apply(img[:, :, 2]).reshape((img.shape[0], img.shape[1], 1))
-
-        self.clahe_adjusted = np.concatenate((R, G, B), axis=2)
-
-    def to_luma(self, gamma, image_array):
-        """Takes in an image array with nxmx3 of type uint8 and transforms it to luminance with or without gamma compensation"""
-        # Image is transformed into sRGB luminance
-        R = (image_array[:, :, 2] / 255)
-
-        G = (image_array[:, :, 1] / 255)
-
-        B = (image_array[:, :, 0] / 255)
-
-        # It is possible to apply a Gamma Conversion to the results as examplified below
-        if gamma:
-            R[R <= 0.04045] = R[R < 0.04045] / 12.92
-            R[R > 0.04045] = ((R[R > 0.04045] + 0.055) / 1.055) ** 2.4
-            G[G <= 0.04045] = G[G < 0.04045] / 12.92
-            G[G > 0.04045] = ((G[G > 0.04045] + 0.055) / 1.055) ** 2.4
-            B[B <= 0.04045] = B[B < 0.04045] / 12.92
-            B[B > 0.04045] = ((B[B > 0.04045] + 0.055) / 1.055) ** 2.4
-
-        # Linear approach for calculating CIE luminance rec. 709, ref Eq. (7).
-        self.luma_array =  0.2125 * R + 0.7154 * G + 0.0721 * B
-
+
+import numpy as np
+
+import cv2 as cv
+
+class Image():
+    def __init__(self, array):
+        """Takes in an image array with nxmx3 of type uint8"""
+        self.image_array = array
+
+    def clahe_adjustment(self, is_luma = False):
+        tile_size = 8
+        clip_lim = 3
+        clahe = cv.createCLAHE(clipLimit=clip_lim, tileGridSize=(tile_size, tile_size))
+        if is_luma:
+            img = (self.luma_array*255).astype(np.uint8) # 0->1
+
+            # Apply equalization and adjust luma array
+            self.luma_array = clahe.apply(img).reshape((img.shape[0], img.shape[1], 1))
+
+        else:
+            
+            img = self.image_array
+            R = clahe.apply(img[:, :, 0]).reshape((img.shape[0], img.shape[1], 1))
+            G = clahe.apply(img[:, :, 1]).reshape((img.shape[0], img.shape[1], 1))
+            B = clahe.apply(img[:, :, 2]).reshape((img.shape[0], img.shape[1], 1))
+
+            self.clahe_adjusted = np.concatenate((R, G, B), axis=2)
+
+    def to_luma(self, gamma, image_array, gamma_inverse = False, gamma_value = 0.45):
+        """Takes in an image array with nxmx3 of type uint8 and transforms it to luminance with or without gamma compensation"""
+        # Image is transformed into sRGB luminance
+        R = (image_array[:, :, 2] / 255)
+
+        G = (image_array[:, :, 1] / 255)
+
+        B = (image_array[:, :, 0] / 255)
+
+        # It is possible to apply a Gamma Conversion to the results as examplified below
+        if gamma:
+            R[R <= 0.04045] = R[R < 0.04045] / 12.92
+            R[R > 0.04045] = ((R[R > 0.04045] + 0.055) / 1.055) ** 2.4
+            G[G <= 0.04045] = G[G < 0.04045] / 12.92
+            G[G > 0.04045] = ((G[G > 0.04045] + 0.055) / 1.055) ** 2.4
+            B[B <= 0.04045] = B[B < 0.04045] / 12.92
+            B[B > 0.04045] = ((B[B > 0.04045] + 0.055) / 1.055) ** 2.4
+
+        # Linear approach for calculating CIE luminance rec. 709, ref Eq. (7).
+        self.luma_array =  0.2125 * R + 0.7154 * G + 0.0721 * B
+
+        if gamma_inverse:
+            self.luma_array = np.power(self.luma_array, gamma_value).clip(0,1)
+
```

### Comparing `gref4hsi-0.2.1/gref4hsi/utils/geometry_utils.py` & `gref4hsi-0.2.2/gref4hsi/utils/geometry_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1444 +1,1443 @@
-# Third party
-import numpy as np
-import numpy.matlib
-from osgeo import gdal, osr
-import rasterio
-from scipy.spatial.transform import Rotation as RotLib
-from scipy.spatial.transform import Slerp
-import open3d as o3d
-import xmltodict
-from pyproj import CRS, Transformer
-import pymap3d as pm
-import ephem
-import pandas as pd
-from scipy.interpolate import interp1d
-import pyvista as pv
-from shapely.geometry import Polygon, mapping, MultiPoint
-from rasterio.transform import from_origin
-from rasterio.windows import from_bounds
-from rasterio.windows import Window
-import trimesh
-
-# Python standard lib
-import os
-import time
-from datetime import datetime
-from dateutil import parser
-import json
-
-# A file were we define geometry and geometric transforms
-class CalibHSI:
-    def __init__(self, file_name_cal_xml, mode = 'r', param_dict = None):
-        """
-        :param file_name_cal_xml: str
-        File name of calibration file for line camera model
-        :param config: config
-        global configuration object.
-        :param mode: str
-        open file for reading (for general use) or writing (post calibration)
-        :param param_dict: dictionary:
-        dictionary with keys
-        "'rx', 'ry', 'rz', 'tx', 'ty', 'tz', 'cx', 'f', 'k1', 'k2', 'k3', 'width'"
-        """
-        if mode == 'r':
-            with open(file_name_cal_xml, 'r', encoding='utf-8') as file:
-                my_xml = file.read()
-            xml_dict = xmltodict.parse(my_xml)
-            self.calibrationHSI = xml_dict['calibration']
-
-            self.w = float(self.calibrationHSI['width'])
-            self.f = float(self.calibrationHSI['f'])
-            self.cx = float(self.calibrationHSI['cx'])
-
-            # Rotations
-            self.rx = float(self.calibrationHSI['rx'])
-            self.ry = float(self.calibrationHSI['ry'])
-            self.rz = float(self.calibrationHSI['rz'])
-
-
-            # Translations
-            self.tx = float(self.calibrationHSI['tx'])
-            self.ty = float(self.calibrationHSI['ty'])
-            self.tz = float(self.calibrationHSI['tz'])
-
-            # Distortions
-            self.k1 = float(self.calibrationHSI['k1'])
-            self.k2 = float(self.calibrationHSI['k2'])
-            self.k3 = float(self.calibrationHSI['k3'])
-        elif mode == 'w':
-            # Check if the file exists
-            if os.path.exists(file_name_cal_xml):
-                with open(file_name_cal_xml, 'r', encoding='utf-8') as file:
-                    my_xml = file.read()
-                xml_dict = xmltodict.parse(my_xml)
-            else:
-                # Create a new xml_dict with default structure
-                xml_dict = {'calibration': {}}
-
-            # Update xml_dict['calibration'] with values from param_dict
-            for key, value in param_dict.items():
-                xml_dict['calibration'][key] = value
-            with open(file_name_cal_xml, 'w') as fd:
-                fd.write(xmltodict.unparse(xml_dict))
-
-class CameraGeometry():
-    def __init__(self, pos, rot, time, is_interpolated = False):
-        
-        self.position_nav = pos
-        self.rotation_nav = rot
-
-        self.time = time
-        self.IsLocal = False
-        self.decoupled = True
-
-        if is_interpolated:
-            self.position_nav_interpolated = self.position_nav
-            self.rotation_nav_interpolated = self.rotation_nav
-
-
-
-    def interpolate(self, time_hsi, minIndRGB, maxIndRGB, extrapolate):
-        """"""
-        # A simple interpolation of transforms where all images should be aligned.
-        # Should also implement a more sensor fusion-like Kalman filter implementation
-        self.time_hsi = time_hsi
-        if self.decoupled == True:
-
-            if extrapolate == False:
-                time_interpolation = time_hsi[minIndRGB:maxIndRGB]
-                linearPositionInterpolator = interp1d(self.time, np.transpose(self.position_nav))
-                self.position_nav_interpolated = np.transpose(linearPositionInterpolator(time_interpolation))
-                linearSphericalInterpolator = Slerp(self.time, self.rotation_nav)
-                self.rotation_nav_interpolated = linearSphericalInterpolator(time_interpolation)
-            else:
-                # Extrapolation of position:
-                time_interpolation = time_hsi
-                linearPositionInterpolator = interp1d(self.time, np.transpose(self.position_nav), fill_value='extrapolate')
-                self.position_nav_interpolated = np.transpose(linearPositionInterpolator(time_interpolation))
-
-                # Extrapolation of orientation/rotation:
-
-                # Synthetizize additional frames
-                delta_rot_b1_b2 = (self.rotation_nav[-1].inv()) * (self.rotation_nav[-2])
-                delta_time_last = self.time[-1] - self.time[-2]
-                time_last = self.time[-1] + delta_time_last
-                rot_last = self.rotation_nav[-1] * (delta_rot_b1_b2.inv()) # Assuming a continuation of the rotation
-
-                # Rotation from second to first attitude
-                delta_rot_b1_b2 = (self.rotation_nav[0].inv()) * (self.rotation_nav[1])
-                delta_time_last = self.time[0] - self.time[1]
-                time_first = self.time[0] + delta_time_last # Subtraction
-                # Add the rotation from second to first attitude to the first attitude "continue" rotation
-                rot_first = self.rotation_nav[0] * (delta_rot_b1_b2.inv())  # Assuming a continuation of the rotation
-                time_concatenated = np.concatenate((np.array(time_first).reshape((1,-1)),
-                                                    self.time.reshape((1,-1)),
-                                                    np.array(time_last).reshape((1,-1))), axis = 1)\
-                    .reshape(-1).astype(np.float64)
-                rotation_list = [self.rotation_nav]
-                rotation_list.append(rot_last)
-                rotation_list.insert(0, rot_first)
-
-
-                rot_vec_first = rot_first.as_rotvec().reshape((1,-1))
-                rot_vec_mid = self.rotation_nav.as_rotvec()
-                rot_vec_last = rot_last.as_rotvec().reshape((1,-1))
-
-                rotation_vec_tot = np.concatenate((rot_vec_first, rot_vec_mid, rot_vec_last), axis = 0)
-
-                Rotation_tot = RotLib.from_rotvec(rotation_vec_tot)
-
-
-
-                time_concatenated = np.array(time_concatenated).astype(np.float64)
-
-                linearSphericalInterpolator = Slerp(time_concatenated, Rotation_tot)
-
-                self.rotation_nav_interpolated = linearSphericalInterpolator(time_interpolation)
-
-
-
-
-
-
-        else:
-            print('Proper interpolation of transformation with constant velocity and rotation has not yet been implemented')
-            print('See https://www.geometrictools.com/Documentation/InterpolationRigidMotions.pdf')
-            #self.rotation_nav_interpolated, self.PositionInterpolated = self.interpolateTransforms()
-    def intrinsicTransformHSI(self, translation_ref_hsi, rot_hsi_ref_obj):
-
-        # An intrinsic transform is a transformation to another reference frame on the moving body, i.e. the IMU or an RGB cam
-        self.position_ecef = self.position_nav_interpolated + self.rotation_nav_interpolated.apply(translation_ref_hsi)
-        
-        self.rotation_hsi_rgb = rot_hsi_ref_obj
-
-        # Composing rotations. See:
-        # https: // docs.scipy.org / doc / scipy / reference / generated / scipy.spatial.transform.Rotation.__mul__.html
-        self.rotation_hsi = self.rotation_nav_interpolated * self.rotation_hsi_rgb 
-
-        self.quaternion_ecef = self.rotation_hsi.as_quat()
-        
-    def localTransform(self, frame):
-        self.IsLocal = True
-        self.LocalTransformFrame = frame
-
-        if frame == 'ENU':
-            self.position_nav_interpolated = self.Rotation_ecef_enu*self.position_nav_interpolated
-            self.rotation_nav_interpolated = self.Rotation_ecef_enu*self.rotation_nav_interpolated
-            self.position_nav = self.Rotation_ecef_enu * self.position_nav
-            self.rotation_nav = self.Rotation_ecef_enu * self.rotation_nav
-            self.rotation_hsi = self.Rotation_ecef_enu * self.rotation_hsi
-            self.position_nav = self.Rotation_ecef_enu * self.position_ecef
-        elif frame == 'NED':
-            self.localPositionInterpolated = self.Rotation_ecef_ned*self.position_nav_interpolated
-            self.localRotationInterpolated = self.Rotation_ecef_ned*self.rotation_nav_interpolated
-            self.localPosition = self.Rotation_ecef_ned * self.position_nav
-            self.localRotation = self.Rotation_ecef_ned * self.rotation_nav
-            self.rotation_hsi = self.Rotation_ecef_ned * self.rotation_hsi
-            self.position_nav = self.Rotation_ecef_ned * self.position_ecef
-        else:
-            print('Frame must be ENU or NED')
-    def localTransformInverse(self):
-
-        if self.IsLocal:
-            self.IsLocal = False
-            if self.LocalTransformFrame == 'ENU':
-                self.position_nav_interpolated = self.Rotation_ecef_enu.inv()*self.position_nav_interpolated
-                self.rotation_nav_interpolated = self.Rotation_ecef_enu.inv()*self.rotation_nav_interpolated
-                self.position_nav = self.Rotation_ecef_enu.inv() * self.position_nav
-                self.rotation_nav = self.Rotation_ecef_enu.inv() * self.rotation_nav
-                self.rotation_hsi = self.Rotation_ecef_enu.inv() * self.rotation_hsi
-                self.position_nav = self.Rotation_ecef_enu.inv() * self.position_ecef
-            elif self.LocalTransformFrame == 'NED':
-                self.localPositionInterpolated = self.Rotation_ecef_ned.inv()* self.position_nav_interpolated
-                self.localRotationInterpolated = self.Rotation_ecef_ned.inv()*self.rotation_nav_interpolated
-                self.localPosition = self.Rotation_ecef_ned.inv() * self.position_nav
-                self.localRotation = self.Rotation_ecef_ned.inv() * self.rotation_nav
-                self.rotation_hsi = self.Rotation_ecef_ned.inv() * self.rotation_hsi
-                self.position_nav = self.Rotation_ecef_ned.inv() * self.position_ecef
-            else:
-                print('Frame must be ENU or NED')
-        else:
-            print('Poses are defined globally already')
-    def defineRayDirections(self, dir_local):
-        self.rayDirectionsLocal = dir_local
-
-        n = self.position_ecef.shape[0]
-        m = dir_local.shape[0]
-
-        self.rayDirectionsGlobal = np.zeros((n, m, 3))
-
-        for i in range(n):
-            self.rayDirectionsGlobal[i, :, :] = self.rotation_hsi[i].apply(dir_local)
-    def intersect_with_mesh(self, mesh, max_ray_length, mesh_trans):
-        """Intersects the rays of the camera with the 3D triangular mesh
-
-        :param mesh: A mesh object read via the pyvista library
-        :type mesh: Pyvista mesh
-        :param max_ray_length: The upper bound length of the camera rays (it is determined )
-        :type max_ray_length: _type_
-        :param mesh_trans: The offset of the mesh
-        :type mesh_trans: _type_
-        """
-
-        n = self.rayDirectionsGlobal.shape[0]
-        m = self.rayDirectionsGlobal.shape[1]
-
-        self.points_ecef_crs = np.zeros((n, m, 3), dtype=np.float64)
-        self.normals_ecef_crs = np.zeros((n, m, 3), dtype=np.float64)
-
-        # Duplicate multiple camera centres
-        start_ECEF = np.einsum('ijk, ik -> ijk', np.ones((n, m, 3), dtype=np.float64), self.position_ecef).reshape((-1,3))
-
-        # Subtract the mesh offset to avoid rounding errors and perform intersection tests with "small coordinates"
-        start = start_ECEF - mesh_trans
-
-        dir = (self.rayDirectionsGlobal * max_ray_length).reshape((-1,3))
-
-        
-        
-        start_time = time.time()
-
-
-        
-        try:
-            # This will only work if exact Python version is rigght and you have PyEmbree
-            points, rays, cells = mesh.multi_ray_trace(origins=start, directions=dir, first_point=True, retry=True)
-        except ImportError:
-            # If you instead use embreex, python>3.6 will do
-            
-            
-            # If the faces are 
-            faces = mesh.regular_faces
-
-            # Convert PolyData to trimesh.Trimesh
-            tri_mesh = trimesh.Trimesh(vertices=mesh.points, faces=faces)
-
-            # Define an intersector object
-            ray_mesh_intersector = trimesh.ray.ray_pyembree.RayMeshIntersector(geometry=tri_mesh)
-
-            # Intersect data
-            count = 0
-            cells, rays, points = ray_mesh_intersector.intersects_id(ray_origins=start,  
-                                                                ray_directions=dir, 
-                                                                multiple_hits=False,
-                                                                return_locations=True)
-            
-        n_points = int(np.size(points)/3)
-        n_rays = int(np.size(start)/3)
-        # Recurring is that 1- 10s of rays fail to detect intersections using Trimesh.
-        # A handy fix is to iterate the failed intersections using individual ray tracing
-        # This equivalent to the retry=True in 
-        # https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.PolyDataFilters.multi_ray_trace.html#pyvista.PolyDataFilters.multi_ray_trace
-        if n_points != n_rays:
-            n_missing = n_rays - n_points
-            print(f'Trimesh failed to find intersections for {n_missing} rays')
-            print(f'Ray tracing for these rays is retried in pyvista')
-
-            # Identify the missing intersections:
-            missing_rays = np.array(list( set(range(n_rays)) - set(rays) ))
-
-            # And ray trace them individually in VTK
-            for ray in missing_rays:
-                # Retry failed intersections with slow pyvista version
-                point, cell = mesh.ray_trace(start[ray,:], start[ray,:] + dir[ray,:], first_point=True)
-                cells = np.concatenate((cells, cell), axis=0)
-                points = np.concatenate((points, point.reshape((1,3))), axis=0)
-                rays = np.concatenate((rays, np.array([ray])), axis=0)
-            n_points = int(np.size(points)/3)
-            print('All rays successfully traced in VTK')
-
-        else:
-            print(f'All rays were successfully intersected with trimesh')
-            
-
-
-        stop_time = time.time()
-
-        normals = mesh.cell_normals[cells,:]
-
-        slit_image_number = np.floor(rays / m).astype(np.int32)
-
-        pixel_number = rays % m
-
-        
-
-
-        # Assign normals
-        self.points_ecef_crs[slit_image_number, pixel_number] = points + mesh_trans
-
-        self.normals_ecef_crs[slit_image_number, pixel_number] = normals
-
-        self.camera_to_seabed_ECEF = self.points_ecef_crs - start_ECEF.reshape((n, m, 3))
-
-
-        # Calculate
-        self.points_hsi_crs = np.zeros(self.camera_to_seabed_ECEF.shape)
-
-        self.normals_hsi_crs = np.zeros(self.normals_ecef_crs.shape)
-
-        self.depth_map = np.zeros((n, m))
-
-        # For local geometry (when vehicle fixed artificial light is used):
-        for i in range(n):
-            # Calculate vector from HSI to seabed in local coordinates (for artificial illumination)
-            self.points_hsi_crs[i, :, :] = (self.rotation_hsi[i].inv()).apply(self.camera_to_seabed_ECEF[i, :, :])
-
-            # Calculate surface normals of intersected triangles (for artificial illumination)
-            self.normals_hsi_crs[i,:,:] = (self.rotation_hsi[i].inv()).apply(self.normals_ecef_crs[i, :, :])
-
-            # Calculate a depth map (the z-component, 1D scanline)
-            self.depth_map[i, :] = self.points_hsi_crs[i, :, 2]/self.rayDirectionsLocal[:, 2]
-
-        
-
-        self.unix_time_grid = np.einsum('ijk, ik -> ijk', np.ones((n, m, 1), dtype=np.float64), self.time.reshape((-1,1)))
-        self.unix_time = self.unix_time_grid.reshape((-1, 1)) # Vector-form
-        self.pixel_nr_grid = np.matlib.repmat(np.arange(m), n, 1)
-        self.frame_nr_grid = np.matlib.repmat(np.arange(n).reshape(-1,1), 1, m)
-
-        
-    @staticmethod
-    def intersect_ray_with_earth_ellipsoid(p0, dir_hat, B):
-        """_summary_
-
-        :param p0: Ray origin
-        :type p0: (3,1) array of floats 
-        :param dir_hat: describing ray direction in some ECEF
-        :type dir_hat: (3,1) array of floats 
-        :param B: Ellipsoid matrix of earth so that (p0 + lam*dir_hat)' * B * (p0 + lam*dir_hat) = 1
-        :type B: (3, 3) matrix describing earth ellipsoid in some ECEF
-        """
-
-        # Solves equation lam^2 *(d_hat'B*d_hat) + lam * 2*(p0' * B* dir_hat) + (p0' *B* p0)= 1
-        a = np.transpose(dir_hat).dot(B.dot(dir_hat))
-        b = 2*np.transpose(p0).dot(B.dot(dir_hat))
-        c = np.transpose(p0).dot(B.dot(p0)) - 1
-
-        p = np.zeros(3)
-        p[0] = a
-        p[1] = b
-        p[2] = c
-
-        lam = np.roots(p)
-
-        hits = p0 + dir_hat*lam
-
-
-        return hits 
-
-    @staticmethod
-    def calculate_sun_directions(longitude, latitude, altitude, unix_time, degrees=True):
-        # Ensure all inputs are NumPy arrays
-        longitude = np.asarray(longitude).flatten()
-        latitude = np.asarray(latitude).flatten()
-        altitude = np.asarray(altitude).flatten()
-        unix_time = np.asarray(unix_time).flatten()
-
-        n = max(longitude.size, latitude.size, altitude.size, unix_time.size)
-
-        # If a single value is provided for any parameter, broadcast it to match the size of the other parameters
-        longitude = np.broadcast_to(longitude, (n,))
-        latitude = np.broadcast_to(latitude, (n,))
-        altitude = np.broadcast_to(altitude, (n,))
-        unix_time = np.broadcast_to(unix_time, (n,))
-
-        phi_s = np.zeros(n)
-        theta_s = np.zeros(n)
-
-        observer = ephem.Observer()
-
-        for i in range(n):
-            # Extract a single value from the arrays
-            observer.lon = str(longitude[i])
-            observer.lat = str(latitude[i])
-            observer.elev = altitude[i]
-            
-            sun = ephem.Sun()
-            observer.date = datetime.utcfromtimestamp(unix_time[i])
-            sun.compute(observer)
-
-            phi_s[i] = np.rad2deg(sun.az)
-            theta_s[i] = 90 - np.rad2deg(sun.alt)
-
-        if not degrees:
-            phi_s = np.deg2rad(phi_s)
-            theta_s = np.deg2rad(theta_s)
-
-        return phi_s, theta_s
-
-    def compute_view_directions_local_tangent_plane(self):
-        """Takes the intersection points and HSI camera positions and computes the angles from seabed to HSI with respect to the local tangent plane to the ellipsoid. 
-        """
-        n = self.rayDirectionsGlobal.shape[0]
-        m = self.rayDirectionsGlobal.shape[1]
-
-        self.seabed_to_camera_NED = np.zeros(self.camera_to_seabed_ECEF.shape)
-        self.normals_ned_crs = np.zeros(self.normals_ecef_crs.shape)
-        self.theta_v = np.zeros((n, m))
-        self.phi_v = np.zeros((n, m))
-
-        x_ecef = self.points_ecef_crs[:, :, 0].reshape((-1,1))
-        y_ecef = self.points_ecef_crs[:, :, 1].reshape((-1,1))
-        z_ecef = self.points_ecef_crs[:, :, 2].reshape((-1,1))
-        
-        lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
-
-        start = np.einsum('ijk, ik -> ijk', np.ones((n, m, 3), dtype=np.float64), self.position_ecef).reshape((-1,3))
-
-        x_hsi = start[:, 0].reshape((-1,1))
-        y_hsi = start[:, 1].reshape((-1,1))
-        z_hsi = start[:, 2].reshape((-1,1))
-
-        # Compute vectors from seabed intersections to HSI in NED
-        NED = pm.ecef2ned(x= x_hsi, y= y_hsi, z=z_hsi, lat0 = lats, lon0=lons, h0 = alts)
-
-        self.seabed_to_camera_NED = np.hstack((NED[0], NED[1], NED[2])).reshape((n, m, 3))
-
-        # For remote sensing with a sun-lit seafloor:
-        for i in range(n):
-            
-            R_ecef_2_ned = RotLib.from_matrix(rotation_matrix_ecef2ned(lon = lons[i], lat = lats[i]))
-
-            # Calculate vector from HSI to seabed in local tangent plane NED
-            #self.camera_to_seabed_NED[i, :, :] = R_ecef_2_ned.apply(self.camera_to_seabed_ECEF[i, :, :])
-
-            # Decompose vector to angles
-            polar = cartesian_to_polar(xyz = self.seabed_to_camera_NED[i,:,:])
-
-            self.theta_v[i, :] = polar[:,1]
-
-            self.phi_v[i, :] = polar[:,2]
-
-            # Calculate surface normals of intersected triangles (for artificial illumination)
-            self.normals_ned_crs[i, :, :] = R_ecef_2_ned.apply(self.normals_ecef_crs[i, :, :])
-
-            
-
-
-    def compute_sun_angles_local_tangent_plane(self):
-        n = self.rayDirectionsGlobal.shape[0]
-        m = self.rayDirectionsGlobal.shape[1]
-
-        x_ecef = self.points_ecef_crs[:, :, 0].reshape((-1,1))
-        y_ecef = self.points_ecef_crs[:, :, 1].reshape((-1,1)) 
-        z_ecef = self.points_ecef_crs[:, :, 2].reshape((-1,1))
-
-        lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
-
-        self.lats = lats
-        self.lons = lons
-        self.alts = alts
-
-        phi_s, theta_s = CameraGeometry.calculate_sun_directions(longitude = lons, latitude = lats, altitude = alts, unix_time = self.unix_time, degrees = True)
-
-        self.phi_s = phi_s.reshape((n, m, 1))
-
-        self.theta_s = theta_s.reshape((n, m, 1))
-
-        
-
-    def compute_elevation_mean_sealevel(self, source_epsg, geoid_path = 'data/world/geoids/egm08_25.gtx'):
-        n = self.rayDirectionsGlobal.shape[0]
-        m = self.rayDirectionsGlobal.shape[1]
-
-        x_ecef = self.position_ecef[:, 0].reshape((-1,1))
-        y_ecef = self.position_ecef[:, 1].reshape((-1,1))
-        z_ecef = self.position_ecef[:, 2].reshape((-1,1))
-
-        #lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
-
-        
-
-        alts_msl = CameraGeometry.elevation_msl(x_ecef, y_ecef, z_ecef, source_epsg=source_epsg, geoid_path = geoid_path)
-        
-
-        self.hsi_alts_msl = np.einsum('ijk, ik -> ijk', np.ones((n, m, 1), dtype=np.float32), alts_msl.reshape((-1,1)))
-
-        
-    
-    @staticmethod
-    def elevation_msl(x_ecef, y_ecef, z_ecef, source_epsg, geoid_path):
-        """_summary_
-
-        :param x_ecef: _description_
-        :type x_ecef: _type_
-        :param y_ecef: _description_
-        :type y_ecef: _type_
-        :param z_ecef: _description_
-        :type z_ecef: _type_
-        :param source_epsg: _description_
-        :type source_epsg: _type_
-        :param geoid_path: _description_
-        :type geoid_path: _type_
-        :return: _description_
-        :rtype: _type_
-        """
-        
-        with rasterio.open(geoid_path) as src:
-
-            source_crs = CRS.from_epsg(source_epsg)
-                
-            target_crs = src.crs
-
-            transformer = Transformer.from_crs(source_crs, target_crs)
-
-            (lat, lon, alt_ell) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
-
-            undulation = np.zeros(lat.shape)
-            # Compute undulation and orthometric height for each point (height above MSL)
-            
-            for i, x, y in zip(range(lat.size), lon, lat):
-                undulation[i] = next(src.sample([(float(x), float(y))]))[0]
-            
-
-        
-        alt_msl = alt_ell - undulation
-
-        return alt_msl
-
-
-
-    
-
-    def compute_tide_level(self, path_tide, tide_format, constant_height = 0):
-
-        n = self.rayDirectionsGlobal.shape[0]
-        m = self.rayDirectionsGlobal.shape[1]
-
-        if path_tide == 'Undefined':
-
-            self.hsi_tide_gridded = constant_height*np.ones((n, m, 1))
-
-        else:
-
-            if tide_format == 'NMA':
-                try:
-                    df_tide = pd.read_csv(path_tide, sep='\s+', parse_dates=[0], index_col=0, comment='#', date_parser=parser.parse)
-
-                    # Convert the datetime index to Unix time and add column
-                    df_tide['UnixTime'] = df_tide.index.astype('int64') // 10**9  # Convert nanoseconds to seconds
-
-                    tide_height_NN2000 = 0.01*df_tide['Observations'] # Since in cm
-
-                    tide_timestamp = df_tide['UnixTime']
-                    
-                    hsi_tide_interp = interp1d(x = tide_timestamp, y= tide_height_NN2000)(x = self.time)
-
-                    # Make into gridded form:
-                    self.hsi_tide_gridded = np.einsum('ijk, ik -> ijk', np.ones((n, m, 1), dtype=np.float64), hsi_tide_interp.reshape((-1,1)))
-                except:
-                    #print('No tide file was found!!')
-                    self.hsi_tide_gridded = constant_height*np.ones((n, m, 1))
-
-
-
-            else: # A Good place to write parsers for other formats
-                TypeError
-        
-    def write_rgb_point_cloud(self, config, hyp, transect_string, extrapolate = True, minInd = None, maxInd = None):
-        wl_red = float(config['General']['red_wave_length'])
-        wl_green = float(config['General']['green_wave_length'])
-        wl_blue = float(config['General']['blue_wave_length'])
-        dir_point_cloud = config['Absolute Paths']['rgb_point_cloud_folder']
-
-        wavelength_nm = np.array([wl_red, wl_green, wl_blue])
-
-        # Localize the appropriate band indices used for analysis
-        band_ind_R = np.argmin(np.abs(wavelength_nm[0] - hyp.band2Wavelength))
-        band_ind_G = np.argmin(np.abs(wavelength_nm[1] - hyp.band2Wavelength))
-        band_ind_B = np.argmin(np.abs(wavelength_nm[2] - hyp.band2Wavelength))
-
-        if extrapolate == False:
-            rgb = hyp.dataCubeRadiance[minInd:maxInd, :, [band_ind_R, band_ind_G, band_ind_B]]
-        else:
-            rgb = hyp.dataCubeRadiance[:, :, [band_ind_R, band_ind_G, band_ind_B]]
-
-
-        points = self.points_ecef_crs[self.points_ecef_crs != 0].reshape((-1,3))
-        rgb_points = (rgb[self.points_ecef_crs != 0] / rgb.max()).astype(np.float64).reshape((-1,3))
-        pcd = o3d.geometry.PointCloud()
-        pcd.points = o3d.utility.Vector3dVector(points)
-        pcd.colors = o3d.utility.Vector3dVector(rgb_points)
-        o3d.io.write_point_cloud(dir_point_cloud + transect_string + '.ply', pcd)
-
-
-    #def transformRays(self, rays):
-        # Rays are a n x m x 3 set of rays where n is each time step and coincides with the rotations and translations:
-
-class FeatureCalibrationObject():
-    def __init__(self, type, config):
-        self.config = config
-        self.type = type
-        self.HSIPositionFeature = [] # Function of feature line
-        self.HSIRotationFeature = [] #
-        self.isfirst = True
-
-    def load_cam_calibration(self, filename_cal, config):
-        calHSI = CalibHSI(file_name_cal_xml=filename_cal)  # Generates a calibration object
-        self.f = calHSI.f
-        self.v_c = calHSI.cx
-        self.k1 = calHSI.k1
-        self.k2 = calHSI.k2
-        self.k3 = calHSI.k3
-
-        self.trans_x = calHSI.tx
-        self.trans_y = calHSI.ty
-        self.trans_z = calHSI.tz
-
-        self.rot_x = calHSI.rx
-        self.rot_y = calHSI.ry
-        self.rot_z = calHSI.rz
-
-        
-
-        #if eval(config['General']['isFlippedRGB']):
-        #    self.trans_x *= -1
-        #    self.trans_y *= -1
-        #if eval(config['General']['isFlippedHSI']):
-        #    self.rot_z += np.pi
-
-
-    def appendGeometry(self, hsiGis, cameraGeometry, binning):
-        # Step 1: Define the global projected position of features
-        point_feature_gt = hsiGis.features_points
-        # Define the hsi pixel number
-        pixel = self.bilinearInterpolation(x1_x=hsiGis.x1_x_hsi, y1_y=hsiGis.y1_y_hsi, f_Q=hsiGis.v_datacube_hsi)
-        # Define the translation:
-        # First define the time stamp for the four lines:
-        line_nr = hsiGis.u_datacube_hsi.astype(np.int64)
-
-        trans_Q_00 = cameraGeometry.position_ecef[line_nr[:, 0]]
-        trans_Q_01 = cameraGeometry.position_ecef[line_nr[:, 1]]
-        trans_Q_10 = cameraGeometry.position_ecef[line_nr[:, 2]]
-        trans_Q_11 = cameraGeometry.position_ecef[line_nr[:, 3]]
-
-        translationHSI = self.bilinearInterpolationPosition(x1_x=hsiGis.x1_x_hsi, y1_y=hsiGis.y1_y_hsi, trans_Q_00=trans_Q_00, trans_Q_01=trans_Q_01, trans_Q_10=trans_Q_10,
-                                                              trans_Q_11=trans_Q_11)
-
-        rot_Q_00 = cameraGeometry.rotation_nav_interpolated[line_nr[:, 0]]
-        rot_Q_01 = cameraGeometry.rotation_nav_interpolated[line_nr[:, 1]]
-        rot_Q_10 = cameraGeometry.rotation_nav_interpolated[line_nr[:, 2]]
-        rot_Q_11 = cameraGeometry.rotation_nav_interpolated[line_nr[:, 3]]
-
-        rotationRGB = self.bilinearInterpolationRotation(x1_x=hsiGis.x1_x_hsi, y1_y=hsiGis.y1_y_hsi,
-                                                              rot_Q_00=rot_Q_00, rot_Q_10=rot_Q_10, rot_Q_01=rot_Q_01,
-                                                              rot_Q_11=rot_Q_11)
-        if self.isfirst:
-            self.point_feature_gt = point_feature_gt
-            self.pixel = pixel
-            self.translationHSI = translationHSI
-            self.rotationRGB = rotationRGB
-            self.binning = np.array([binning]).reshape((1,1))
-            self.diff = hsiGis.diff
-
-            self.isfirst = False
-        else:
-            # Add observations
-            self.diff = np.concatenate((self.diff, hsiGis.diff), axis = 0)
-            self.point_feature_gt = np.concatenate((self.point_feature_gt, point_feature_gt), axis = 0)
-            self.pixel = np.concatenate((self.pixel, pixel), axis = 0)
-            self.translationHSI = np.concatenate((self.translationHSI, translationHSI), axis = 0)
-            self.rotationRGB = np.concatenate((self.rotationRGB, rotationRGB), axis = 0)
-
-
-
-    #def defineRayDirections
-    def bilinearInterpolation(self, x1_x, y1_y, f_Q):
-
-
-        f_x_y1 = (1 - x1_x)*f_Q[:, 0] + x1_x*f_Q[:, 1]
-        f_x_y2 = (1 - x1_x) * f_Q[:, 2] + x1_x * f_Q[:, 3]
-
-        f_x_y = (1 - y1_y)*f_x_y1 + y1_y*f_x_y2
-
-        return f_x_y
-    def bilinearInterpolationPosition(self, x1_x, y1_y, trans_Q_00, trans_Q_01, trans_Q_10,
-                                                              trans_Q_11):
-
-        trans_tot = np.zeros(trans_Q_00.shape)
-        for i in range(3):
-
-            f_x_y1 = (1 - x1_x)*trans_Q_00[:, i] + x1_x*trans_Q_01[:, i]
-            f_x_y2 = (1 - x1_x) * trans_Q_10[:, i] + x1_x * trans_Q_11[:, i]
-
-            f_x_y = (1 - y1_y)*f_x_y1 + y1_y*f_x_y2
-            trans_tot[:, i] = f_x_y
-
-
-        return trans_tot
-
-    def bilinearInterpolationRotation(self, x1_x, y1_y, rot_Q_00, rot_Q_10, rot_Q_01, rot_Q_11):
-
-        # Define all rotations from rot_Q_00
-        delta_rot0_rot = np.zeros((4, x1_x.shape[0], 3))
-        # Define all relative rotations
-        delta_rot0_rot[1, :, :] = (rot_Q_01 * rot_Q_00.inv()).as_rotvec(degrees = False)
-        delta_rot0_rot[2, :, :] = (rot_Q_10 * rot_Q_00.inv()).as_rotvec(degrees = False)
-        delta_rot0_rot[3, :, :] = (rot_Q_11 * rot_Q_00.inv()).as_rotvec(degrees = False)
-
-        Q_rots_permuted = np.transpose(delta_rot0_rot, axes = [2, 1, 0])
-
-        rot_vec_final = np.zeros((3, x1_x.shape[0]))
-
-        for i  in range(3):
-            f_Q = Q_rots_permuted[i, :, :]
-            f_x_y1 = (1 - x1_x) * f_Q[:, 0] + x1_x * f_Q[:, 1]
-            f_x_y2 = (1 - x1_x) * f_Q[:, 2] + x1_x * f_Q[:, 3]
-
-            f_x_y = (1 - y1_y) * f_x_y1 + y1_y * f_x_y2
-
-            rot_vec_final[i, :] = f_x_y
-
-        delta_rot_interp = RotLib.from_rotvec(np.transpose(rot_vec_final))
-
-        # Compose the values to rot0
-        rot_tot = delta_rot_interp * rot_Q_00
-
-
-        return rot_tot
-
-    
-    # At the time of updated parameters
-    def reprojectFeaturesHSI(self):
-        rot_hsi_rgb = np.array([self.rot_z, self.rot_y, self.rot_x]) * 180 / np.pi
-
-        self.rotation_hsi_rgb = RotLib.from_euler('ZYX', rot_hsi_rgb, degrees=True)
-
-        self.rotation_hsi = self.rotationRGB * self.rotation_hsi_rgb # Composing rotations.
-
-        self.HSIToFeaturesGlobal = self.point_feature_gt - self.translationHSI
-
-        n = self.HSIToFeaturesGlobal.shape[0]
-
-        self.HSIToFeaturesLocal = np.zeros(self.HSIToFeaturesGlobal.shape)
-        for i in range(n):
-            self.HSIToFeaturesLocal[i, :] = (self.rotation_hsi[i].inv()).apply(
-                self.HSIToFeaturesGlobal[i, :])
-
-            self.HSIToFeaturesLocal[i, :] /= self.HSIToFeaturesLocal[i, 2]
-
-
-
-
-def compute_camera_rays_from_parameters(pixel_nr, cx, f, k1, k2, k3):
-    """_summary_
-
-    :param pixel_nr: _description_
-    :type pixel_nr: _type_
-    :param rot_x: _description_
-    :type rot_x: _type_
-    :param rot_y: _description_
-    :type rot_y: _type_
-    :param rot_z: _description_
-    :type rot_z: _type_
-    :param cx: _description_
-    :type cx: _type_
-    :param f: _description_
-    :type f: _type_
-    :param k1: _description_
-    :type k1: _type_
-    :param k2: _description_
-    :type k2: _type_
-    :param k3: _description_
-    :type k3: _type_
-    :return: _description_
-    :rtype: _type_
-    """
-
-    u = pixel_nr + 1
-
-    # Express uhi ray directions in uhi frame using line-camera model
-    x_norm_lin = (u - cx) / f
-
-    x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
-                        k2 * ((u - cx) / 1000) ** 3 + \
-                        k3 * ((u - cx) / 1000) ** 2) / f
-
-    x_norm = x_norm_lin + x_norm_nonlin
-
-    return x_norm
-
-
-def reproject_world_points_to_hsi_plane(trans_hsi_body, rot_hsi_body, pos_body, rot_body, points_world):
-    """Reprojects world points to local image plane coordinates (x_h, y_h, 1)
-
-    :param trans_hsi_body: lever arm from body center to hsi focal point
-    :type trans_hsi_body: _type_
-    :param rot_hsi_body: boresight rotation 
-    :type rot_hsi_body: Scipy rotation object
-    :param pos_body: The earth fixed earth centered position of the vehicle body centre
-    :type pos_body: _type_
-    :param rot_body: The rotation of the body in ECEF
-    :type rot_body: Scipy rotation object
-    :param points_world: World points in ECEF
-    :type points_world: _type_
-    :return: The reprojection coordinates
-    :rtype: ndarray(n, 3)
-    """
-
-    
-
-    # We compose the hypothesized boresight (rot_hsi_body) an lever arm (trans_hsi_body) to get the hypothesized position/orientation
-    # of the hyperspectral imager
-    rotation_hsi = rot_body * rot_hsi_body
-    position_hsi = pos_body + rot_body.apply(trans_hsi_body)
-
-    # Given the positions, the hsi-point vector can be expressed in ECEF
-    hsi_to_feature_global = points_world - position_hsi
-
-    # Number of features to iterate
-    n = hsi_to_feature_global.shape[0]
-
-    # We can now express the hsi-point vector in the HSI frame and normalize by the z component to find the image plane projection
-    hsi_to_feature_local = np.zeros(hsi_to_feature_global.shape)
-    for i in range(n):
-        # The vector expressed in HSI frame
-        hsi_to_feature_local[i, :] = (rotation_hsi[i].inv()).apply(hsi_to_feature_global[i, :])
-
-        # The vector normalized to lie on the virtual plane
-        hsi_to_feature_local[i, :] /= hsi_to_feature_local[i, 2]
-    
-    return hsi_to_feature_local
-
-
-
-
-def interpolate_poses(timestamp_from, pos_from, rot_from, timestamps_to, extrapolate = True):
-    """
-
-    :param timestamp_from:
-    Original timestamps
-    :param pos_from: numpy array (n,3)
-    Original positions
-    :param rot_from: Rotation-object (n rotations)
-    Original orientations
-    :param timestamps_to:
-    Timestamps desired for position and orientations
-    :return:
-    """
-    """
-    min_to = np.min(timestamps_to)
-    max_to = np.max(timestamps_to)
-
-    min_from = np.min(timestamp_from)
-    max_from = np.max(timestamp_from)
-
-    minInd = np.argmin(np.abs(min_from - timestamps_to))
-    maxInd = np.argmin(np.abs(max_from - timestamps_to))
-
-    # If navigation data aka "from" is made properly, min_from<<min_to, and max_from >> max_to
-    
-    if timestamps_to[minInd] < min_from:
-        minInd += 1
-    if timestamps_to[maxInd] > min_from: # So if the max index is 
-        maxInd -= 1
-    """
-
-    min_ind = 0
-    max_ind = timestamps_to.size
-
-
-    # Setting use_absolute_position to True means that position calculations are done with absolute
-    referenceGeometry = CameraGeometry(pos=pos_from,
-                               rot=rot_from,
-                               time=timestamp_from)
-
-    # We exploit a method from the camera object
-    referenceGeometry.interpolate(time_hsi=timestamps_to,
-                          minIndRGB=min_ind,
-                          maxIndRGB=max_ind,
-                          extrapolate=extrapolate)
-
-
-
-    position_to = referenceGeometry.position_nav_interpolated
-
-    quaternion_to = referenceGeometry.rotation_nav_interpolated.as_quat()
-
-    return position_to, quaternion_to
-
-
-
-
-def cartesian_to_polar(xyz):
-    """Converts from 3D cartesian coordinates to polar coordinates
-
-    :param xyz: _description_
-    :type xyz: (n,3) numpy array
-    :return: Radii, Elevations, Azimuths
-    :rtype: (n,3) numpy array of radii, theta, phi
-    """
-    polar = np.zeros(xyz.shape)
-    xy = xyz[:,0]**2 + xyz[:,1]**2
-    polar[:,0] = np.sqrt(xy + xyz[:,2]**2) # Radii
-    polar[:,1] = np.arctan2(np.sqrt(xy), np.abs(xyz[:,2])) # for elevation angle defined from Z-axis down [0-90]
-    polar[:,2] = np.arctan2(xyz[:,1], xyz[:,0]) # Azimuth
-
-    return polar
-
-
-
-
-
-
-
-
-
-
-def rotation_matrix_ecef2ned(lon, lat):
-    """
-    Computes the rotation matrix R from earth-fixed-earth centered (ECEF) to north-east-down (NED).
-    :param lat: float in range [-90, 90]
-    The latitude in degrees
-    :param lon: float in range [-180, 180]
-    :return R_ned_ecef: numpy array of shape (3,3)
-    rotation matrix ECEF to NED
-    """
-    R_ned_ecef = rot_mat_ned_2_ecef(lon=lon, lat=lat)
-    return np.transpose(R_ned_ecef)
-
-def rotation_matrix_ecef2enu(lon, lat):
-    l = np.deg2rad(lon)
-    mu = np.deg2rad(lat)
-
-    R_ecef_ned = rotation_matrix_ecef2ned(lon=lon, lat=lat)
-    R_ecef_enu = np.zeros(R_ecef_ned.shape)
-    #
-    R_ecef_enu[[0, 1]] = R_ecef_ned[[1, 0]] # Swap rows
-    R_ecef_enu[2] = -R_ecef_ned[2] # Switch signs to compensate for up and down
-
-
-    
-    return R_ecef_enu
-
-
-def convert_rotation_ned_2_ecef(rot_obj_ned, position, is_geodetic = True, epsg_pos = 4326):
-    """
-
-    :param rot_obj_:
-    :param position:
-    The position
-    :param is_geodetic: bool
-    Whether position is geodetic
-    :return:
-    """
-
-
-class GeoPose:
-    """
-    An object that allows to input positions with arbitrary CRS, and orientations either wrt ECEF or NED. As in other
-    places in the project, the orientations are abstracted with rotation objects. The main use case is formatting poses
-    to the correct CRS.
-    """
-    def __init__(self, timestamps, rot_obj, rot_ref, pos, pos_epsg):
-        self.timestamps = timestamps
-        if rot_ref == 'NED':
-            self.rot_obj_ned = rot_obj
-            self.rot_obj_ecef = None
-        elif rot_ref == 'ECEF':
-            self.rot_obj_ned = None
-            self.rot_obj_ecef = rot_obj
-        else:
-            print('This rotation reference is not supported')
-            TypeError
-
-        # Define position
-        self.position = pos
-        self.epsg = pos_epsg
-
-
-        self.lat = None
-        self.lon = None
-        self.hei = None
-
-        self.compute_geodetic_position()
-        self.compute_geocentric_orientation()
-        self.compute_ned_orientation()
-        self.compute_ned_2_ecef()
-
-
-    def compute_geodetic_position(self, epsg_geod = 4326):
-        """
-            Function for transforming positions to latitude longitude height
-            :param epsg_geod: int
-            EPSG code of the transformed geodetic coordinate system
-        """
-        # If geocentric position has not been defined.
-        from_CRS = CRS.from_epsg(self.epsg)
-        geod_CRS = CRS.from_epsg(epsg_geod)
-        transformer = Transformer.from_crs(from_CRS, geod_CRS)
-
-        x = self.position[:, 0].reshape((-1, 1))
-        y = self.position[:, 1].reshape((-1, 1))
-        z = self.position[:, 2].reshape((-1, 1))
-
-        (lat, lon, hei) = transformer.transform(xx=x, yy=y, zz=z)
-
-        self.epsg_geod = epsg_geod
-        self.lat = lat.reshape((self.position.shape[0], 1))
-        self.lon = lon.reshape((self.position.shape[0], 1))
-        self.hei = hei.reshape((self.position.shape[0], 1))
-
-    def compute_geocentric_position(self, epsg_geocsc):
-        """
-            Function for transforming positions to geocentric
-            :param epsg_geod: int
-            EPSG code of the transformed geodetic coordinate system
-        """
-
-        from_CRS = CRS.from_epsg(self.epsg)
-        geod_CRS = CRS.from_epsg(epsg_geocsc)
-        transformer = Transformer.from_crs(from_CRS, geod_CRS)
-
-        x = self.position[:, 0].reshape((-1, 1))
-        y = self.position[:, 1].reshape((-1, 1))
-        z = self.position[:, 2].reshape((-1, 1))
-
-        (x, y, z) = transformer.transform(xx=x, yy=y, zz=z)
-
-        self.pos_geocsc = np.concatenate((x, y, z), axis = 1)
-
-    def compute_geocentric_orientation(self):
-        if self.rot_obj_ecef == None:
-            # Define rotations from ned to ecef
-            if self.lat.any == None:
-                # Needed to encode rotation between NED and ECEF
-                self.compute_geodetic_position()
-
-            R_body_2_ned = self.rot_obj_ned
-            R_ned_2_ecef = self.compute_ned_2_ecef()
-            R_body_2_ecef = R_ned_2_ecef*R_body_2_ned
-
-            self.rot_obj_ecef = R_body_2_ecef
-
-        else:
-            pass
-
-    def compute_ned_orientation(self):
-        if self.rot_obj_ned == None:
-            # Define rotations from body to ecef
-            R_body_2_ecef = self.rot_obj_ecef
-
-            # Define rotation from ecef 2 ned
-            R_ecef_2_ned = self.compute_ned_2_ecef().inv()
-
-            # Compose
-            R_body_2_ned = R_ecef_2_ned*R_body_2_ecef
-
-            self.rot_obj_ned = R_body_2_ned
-
-
-        else:
-            pass
-
-    def compute_ned_2_ecef(self):
-
-        N = self.lat.shape[0]
-        rot_mats_ned_2_ecef = np.zeros((N, 3, 3), dtype=np.float64)
-        
-        for i in range(N):
-            rot_mats_ned_2_ecef[i,:,:] = rot_mat_ned_2_ecef(lat=self.lat[i], lon = self.lon[i])
-
-
-        self.rot_obj_ned_2_ecef = RotLib.from_matrix(rot_mats_ned_2_ecef)
-
-        return self.rot_obj_ned_2_ecef
-
-    
-
-
-def rot_mat_ned_2_ecef(lat, lon):
-    """
-    Computes the rotation matrix R from north-east-down (NED) to earth-fixed-earth centered (ECEF)
-    :param lat: float in range [-90, 90]
-    The latitude in degrees
-    :param lon: float in range [-180, 180]
-    :return R_ned_ecef: numpy array of shape (3,3)
-    rotation matrix from NED to ECEF
-    """
-
-    # Ensure lat and lon are scalar values
-    lat_scalar = lat[0] if isinstance(lat, np.ndarray) else lat
-    lon_scalar = lon[0] if isinstance(lon, np.ndarray) else lon
-
-    # Convert to radians
-    l = np.deg2rad(lon_scalar)
-    mu = np.deg2rad(lat_scalar)
-
-    # Compute rotation matrix
-    # TODO: add source
-    R_ned_ecef = np.array([[-np.cos(l) * np.sin(mu), -np.sin(l), -np.cos(l) * np.cos(mu)],
-                           [-np.sin(l) * np.sin(mu), np.cos(l), -np.sin(l) * np.cos(mu)],
-                           [np.cos(mu), 0, -np.sin(mu)]])
-    return R_ned_ecef
-
-
-def read_raster(filename, out_crs="EPSG:3857", use_z=False):
-    """Read a raster to a ``pyvista.StructuredGrid``.
-
-    This will handle coordinate transformations.
-    """
-    from rasterio import transform
-    import rioxarray
-    # Read in the data
-    data = rioxarray.open_rasterio(filename)
-    values = np.asarray(data)
-    data.rio.nodata
-    nans = values == data.rio.nodata
-    if np.any(nans):
-        # values = np.ma.masked_where(nans, values)
-        values[nans] = np.nan
-    # Make a mesh
-    xx, yy = np.meshgrid(data["x"], data["y"])
-    if use_z and values.shape[0] == 1:
-        # will make z-comp the values in the file
-        zz = values.reshape(xx.shape)
-    else:
-        # or this will make it flat
-        zz = np.zeros_like(xx)
-    mesh = pv.StructuredGrid(xx, yy, zz)
-    pts = mesh.points
-    lon, lat = transform(data.rio.crs, out_crs, pts[:, 0], pts[:, 1])
-    mesh.points[:, 0] = lon
-    mesh.points[:, 1] = lat
-    mesh["data"] = values.reshape(mesh.n_points, -1, order="F")
-    return mesh
-
-def dem_2_mesh(path_dem, model_path, config):
-    """
-    A function for converting a specified DEM to a 3D mesh model (*.vtk, *.ply or *.stl). 
-    Consequently, mesh should be thought of as 2.5D representation.
-    In the case 
-
-    :param path_dem: _description_
-    :type path_dem: _type_
-    :param model_path: _description_
-    :type model_path: _type_
-    :param config: _description_
-    :type config: _type_
-    """
-
-
-    # The desired CRS for the model must be same as positions, orientations
-    epsg_geocsc = config['Coordinate Reference Systems']['geocsc_epsg_export']
-
-    # Intermediate point cloud format
-    output_xyz = model_path.split(sep = '.')[0] + '.xyz'
-
-    # Open the input raster dataset
-    ds = gdal.Open(path_dem)
-
-    if ds is None:
-        print(f"Failed to open {path_dem}")
-    else:
-        # Read the first band (band index is 1)
-        band = ds.GetRasterBand(1)
-        no_data_value = band.GetNoDataValue()
-        if band is None:
-            print(f"Failed to open band 1 of {path_dem}")
-        else:
-            # Get the geotransform information to calculate coordinates
-            geotransform = ds.GetGeoTransform()
-            x_origin = geotransform[0]
-            y_origin = geotransform[3]
-            x_resolution = geotransform[1]
-            y_resolution = geotransform[5]
-            # Get the CRS information
-            spatial_reference = osr.SpatialReference(ds.GetProjection())
-
-            # Get the EPSG code
-            epsg_proj = None
-            if spatial_reference.IsProjected():
-                epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 1)
-                is_projected = True
-                config.set('Coordinate Reference Systems', 'dem_epsg', str(epsg_proj))
-            elif spatial_reference.IsGeographic():
-                epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 0)
-                proj = ds.GetProjection()
-                is_projected = False
-
-
-            # Automatically set
-            
-            
-            # Get the band's data as a NumPy array of float64 (important)
-            band_data = band.ReadAsArray().astype(np.float64)
-
-            # Create a mask to identify no-data values
-            mask = band_data != no_data_value
-
-            # Create and open the output XYZ file for writing if it does not exist:
-            if not os.path.exists(output_xyz):
-                with open(output_xyz, 'w') as xyz_file:
-                    # Write data to the XYZ file using the mask and calculated coordinates
-                    for y in range(ds.RasterYSize):
-                        for x in range(ds.RasterXSize):
-                            if mask[y, x]:
-                                x_coord = x_origin + x * x_resolution
-                                y_coord = y_origin + y * y_resolution
-                                xyz_file.write(f"{x_coord} {y_coord} {band_data[y, x]}\n")
-            else:
-                print('*.xyz already exists, ignoring re-creation')
-            # Clean up
-            ds = None
-            band = None
-    
-
-    points = np.loadtxt(output_xyz)
-    points_offset = np.mean(points, axis = 0)
-
-    # Create a pyvista point cloud object (just to avoid precision problems)
-    cloud = pv.PolyData(points-points_offset)
-    
-    # TODO: Apply patch to avoid crash for triangulation when using big DEM files
-    # Generate a mesh from points
-    mesh = cloud.delaunay_2d(progress_bar=True)
-
-    # Transform the mesh points from projected to geocentric ECEF.
-    geocsc = CRS.from_epsg(epsg_geocsc)
-
-    if epsg_proj == 'EPSG': # If a geographic CRS
-        pass
-    else:
-        proj = CRS.from_epsg(epsg_proj)
-
-    transformer = Transformer.from_crs(proj, geocsc)
-
-    # Convert to proper coordinates
-    points_proj = mesh.points + points_offset
-
-    if is_projected:
-        x_proj = points_proj[:, 0].reshape((-1, 1))
-        y_proj = points_proj[:, 1].reshape((-1, 1))
-    else:
-        x_proj = points_proj[:, 1].reshape((-1, 1))
-        y_proj = points_proj[:, 0].reshape((-1, 1))
-    
-    h_proj = points_proj[:, 2].reshape((-1, 1))
-
-    (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=x_proj, yy=y_proj, zz=h_proj)
-
-    # Introduce mesh offsets in ECEF sized numbers seem to cause troubles:
-    offset_x = np.mean(x_ecef.reshape(-1))
-    offset_y = np.mean(y_ecef.reshape(-1))
-    offset_z = np.mean(z_ecef.reshape(-1))
-
-    mesh.points[:, 0] = x_ecef.reshape(-1) - offset_x
-    mesh.points[:, 1] = y_ecef.reshape(-1) - offset_y
-    mesh.points[:, 2] = z_ecef.reshape(-1) - offset_z
-   
-
-    # Save mesh
-    mesh.save(model_path)
-    # Save mesh meta
-    # Define your metadata dictionary
-    metadata = {
-        "offset_x": offset_x,
-        "offset_y": offset_y,
-        "offset_z": offset_z,
-        "epsg_code": geocsc.to_epsg(),  # Example EPSG code, replace with your actual code
-        "data_type": str(mesh.points.dtype),  # Add other metadata entries here
-    }
-
-    model_meta_path = model_path.split('.')[0] + '_meta.json' 
-    # Open the file in write mode with proper indentation
-    with open(model_meta_path, "w") as f:
-        # Write the dictionary to the file using JSON dump
-        json.dump(metadata, f)
-
-
-def crop_geoid_to_pose(path_dem, config, geoid_path = 'data/world/geoids/egm08_25.gtx'):
-    # The desired CRS for the model must be same as positions, orientations
-    epsg_geocsc = config['Coordinate Reference Systems']['geocsc_epsg_export']
-
-    # Open the input raster dataset
-    
-    ds = gdal.Open(geoid_path)
-
-    df_pose = pd.read_csv(config['Absolute Paths']['pose_path'])
-
-    # Find CRS of DEM
-    spatial_reference = osr.SpatialReference(ds.GetProjection())
-
-
-    # Get the EPSG code
-    epsg_proj = None
-    if spatial_reference.IsProjected():
-        epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 1)
-    elif spatial_reference.IsGeographic():
-        epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 0)
-    
-    # Transform points to DEM CRS
-    geocsc = CRS.from_epsg(epsg_geocsc)
-    proj = ds.GetProjection()
-    transformer = Transformer.from_crs(geocsc, proj)
-
-    x_ecef = df_pose[' X'].values.reshape((-1, 1))
-    y_ecef = df_pose[' Y'].values.reshape((-1, 1))
-    z_ecef = df_pose[' Z'].values.reshape((-1, 1))
-
-    (x_proj, y_proj, z_proj) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
-
-    coords_horz = np.concatenate((x_proj.reshape((-1,1)), y_proj.reshape((-1,1))), axis = 1)
-
-    # Determine bounding rectangle ()
-    polygon = MultiPoint(coords_horz).envelope
-    # Corners
-    x, y = polygon.exterior.xy
-    x = np.array(x)
-    y = np.array(y)
-
-    # Determine padding
-    padding = float(config['General']['max_ray_length'])
-
-    if spatial_reference.IsProjected():
-        # Add padding to 
-        xmin = x.min() - padding
-        ymin = y.min() - padding
-        xmax = x.max() + padding
-        ymax = y.max() + padding
-    elif spatial_reference.IsGeographic():
-        # Must translate metric padding into increments in lon/lat
-        (x_new, y_new, z_new) = pm.enu2geodetic(e= np.array([-padding, padding]), n= np.array([-padding, padding]), u = 0, lon0=np.mean(y), lat0=np.mean(x), h0 = 0)
-        delta_x = x_new[1] - np.mean(x)
-        delta_y = y_new[1] - np.mean(y)
-
-        # Swap x and y because x, y above is latitude, longitude and Rasterio expects opposite
-        ymin = x.min() - delta_x
-        xmin = y.min() - delta_y
-        ymax = x.max() + delta_x
-        xmax = y.max() + delta_y
-
-        minx, miny, maxx, maxy = [xmin, ymin, xmax, ymax]  # Replace with actual coordinates
-
-        
-
-    # Crops the DEM to the appropriate bounds and writes a new file (Copies CRS info from Geoid)
-    crop_dem_from_bounds(minx, miny, maxx, maxy, dem_path_source=geoid_path, dem_path_target=path_dem)
-     
-
-
-def crop_dem_from_bounds(minx, miny, maxx, maxy, dem_path_source, dem_path_target):
-
-    dem_dataset = rasterio.open(dem_path_source)
-    res_x = dem_dataset.transform.a
-    res_y = -dem_dataset.transform.e
-
-    if maxx-minx < res_x:
-        minx += -res_x
-        maxx += res_x
-    
-    if maxy-miny < res_y:
-        miny += -res_y
-        maxy += res_y
-
-    window = from_bounds(minx, miny, maxx, maxy, dem_dataset.transform)
-
-    window = Window(window.col_off, window.row_off, np.ceil(window.width), np.ceil(window.height))
-
-    cropped_dem_data = dem_dataset.read(window=window)
-
-    # Update the transform based on the new window
-    new_transform = dem_dataset.window_transform(window)
-    new_height, new_width = cropped_dem_data.shape[1], cropped_dem_data.shape[2]
-
-    # Create a new dataset for the cropped DEM
-    cropped_dem_profile = dem_dataset.profile.copy()
-    cropped_dem_profile.update({
-        'width': new_width,
-        'height': new_height,
-        'transform': new_transform
-    })
-
-
-    with rasterio.open(dem_path_target, 'w', **cropped_dem_profile) as dst:
-        dst.write(cropped_dem_data)
-
-
-def position_transform_ecef_2_llh(position_ecef, epsg_from, epsg_to, config):
-    """
-    Function for transforming ECEF positions to latitude longitude height
-    :param position_ecef: numpy array floats (n,3)
-    :param epsg_from: int
-    EPSG code of the original geocentric coordinate system (ECEF)
-    :param epsg_to: int
-    EPSG code of the transformed geodetic coordinate system
-    :return lat_lon_hei: numpy array floats (n,3)
-    latitude, longitude ellipsoid height.
-    """
-    geocsc = CRS.from_epsg(epsg_from)
-    geod = CRS.from_epsg(epsg_to)
-    transformer = Transformer.from_crs(geocsc, geod)
-
-    x_ecef = position_ecef[:, 0].reshape((-1, 1))
-    y_ecef = position_ecef[:, 1].reshape((-1, 1))
-    z_ecef = position_ecef[:, 2].reshape((-1, 1))
-
-    (lat, lon, hei) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
-
-    lat_lon_hei = np.zeros(position_ecef.shape)
-    lat_lon_hei[:, 0] = lat.reshape((position_ecef.shape[0], 1))
-    lat_lon_hei[:, 1] = lon.reshape((position_ecef.shape[0], 1))
-    lat_lon_hei[:, 2] = hei.reshape((position_ecef.shape[0], 1))
-
-    return lat_lon_hei
+# Third party
+import numpy as np
+import numpy.matlib
+from osgeo import gdal, osr
+import rasterio
+from scipy.spatial.transform import Rotation as RotLib
+from scipy.spatial.transform import Slerp
+import open3d as o3d
+import xmltodict
+from pyproj import CRS, Transformer
+import pymap3d as pm
+import ephem
+import pandas as pd
+from scipy.interpolate import interp1d
+import pyvista as pv
+from shapely.geometry import Polygon, mapping, MultiPoint
+from rasterio.transform import from_origin
+from rasterio.windows import from_bounds
+from rasterio.windows import Window
+import trimesh
+
+# Python standard lib
+import os
+import time
+from datetime import datetime
+from dateutil import parser
+import json
+
+# A file were we define geometry and geometric transforms
+class CalibHSI:
+    def __init__(self, file_name_cal_xml, mode = 'r', param_dict = None):
+        """
+        :param file_name_cal_xml: str
+        File name of calibration file for line camera model
+        :param config: config
+        global configuration object.
+        :param mode: str
+        open file for reading (for general use) or writing (post calibration)
+        :param param_dict: dictionary:
+        dictionary with keys
+        "'rx', 'ry', 'rz', 'tx', 'ty', 'tz', 'cx', 'f', 'k1', 'k2', 'k3', 'width'"
+        """
+        if mode == 'r':
+            with open(file_name_cal_xml, 'r', encoding='utf-8') as file:
+                my_xml = file.read()
+            xml_dict = xmltodict.parse(my_xml)
+            self.calibrationHSI = xml_dict['calibration']
+
+            self.w = float(self.calibrationHSI['width'])
+            self.f = float(self.calibrationHSI['f'])
+            self.cx = float(self.calibrationHSI['cx'])
+
+            # Rotations
+            self.rx = float(self.calibrationHSI['rx'])
+            self.ry = float(self.calibrationHSI['ry'])
+            self.rz = float(self.calibrationHSI['rz'])
+
+
+            # Translations
+            self.tx = float(self.calibrationHSI['tx'])
+            self.ty = float(self.calibrationHSI['ty'])
+            self.tz = float(self.calibrationHSI['tz'])
+
+            # Distortions
+            self.k1 = float(self.calibrationHSI['k1'])
+            self.k2 = float(self.calibrationHSI['k2'])
+            self.k3 = float(self.calibrationHSI['k3'])
+        elif mode == 'w':
+            # Check if the file exists
+            if os.path.exists(file_name_cal_xml):
+                with open(file_name_cal_xml, 'r', encoding='utf-8') as file:
+                    my_xml = file.read()
+                xml_dict = xmltodict.parse(my_xml)
+            else:
+                # Create a new xml_dict with default structure
+                xml_dict = {'calibration': {}}
+
+            # Update xml_dict['calibration'] with values from param_dict
+            for key, value in param_dict.items():
+                xml_dict['calibration'][key] = value
+            with open(file_name_cal_xml, 'w') as fd:
+                fd.write(xmltodict.unparse(xml_dict))
+
+class CameraGeometry():
+    def __init__(self, pos, rot, time, is_interpolated = False):
+        
+        self.position_nav = pos
+        self.rotation_nav = rot
+
+        self.time = time
+        self.IsLocal = False
+        self.decoupled = True
+
+        if is_interpolated:
+            self.position_nav_interpolated = self.position_nav
+            self.rotation_nav_interpolated = self.rotation_nav
+
+
+
+    def interpolate(self, time_hsi, minIndRGB, maxIndRGB, extrapolate):
+        """"""
+        # A simple interpolation of transforms where all images should be aligned.
+        # Should also implement a more sensor fusion-like Kalman filter implementation
+        self.time_hsi = time_hsi
+        if self.decoupled == True:
+
+            if extrapolate == False:
+                time_interpolation = time_hsi[minIndRGB:maxIndRGB]
+                linearPositionInterpolator = interp1d(self.time, np.transpose(self.position_nav))
+                self.position_nav_interpolated = np.transpose(linearPositionInterpolator(time_interpolation))
+                linearSphericalInterpolator = Slerp(self.time, self.rotation_nav)
+                self.rotation_nav_interpolated = linearSphericalInterpolator(time_interpolation)
+            else:
+                # Extrapolation of position:
+                time_interpolation = time_hsi
+                linearPositionInterpolator = interp1d(self.time, np.transpose(self.position_nav), fill_value='extrapolate')
+                self.position_nav_interpolated = np.transpose(linearPositionInterpolator(time_interpolation))
+
+                # Extrapolation of orientation/rotation:
+
+                # Synthetizize additional frames
+                delta_rot_b1_b2 = (self.rotation_nav[-1].inv()) * (self.rotation_nav[-2])
+                delta_time_last = self.time[-1] - self.time[-2]
+                time_last = self.time[-1] + delta_time_last
+                rot_last = self.rotation_nav[-1] * (delta_rot_b1_b2.inv()) # Assuming a continuation of the rotation
+
+                # Rotation from second to first attitude
+                delta_rot_b1_b2 = (self.rotation_nav[0].inv()) * (self.rotation_nav[1])
+                delta_time_last = self.time[0] - self.time[1]
+                time_first = self.time[0] + delta_time_last # Subtraction
+                # Add the rotation from second to first attitude to the first attitude "continue" rotation
+                rot_first = self.rotation_nav[0] * (delta_rot_b1_b2.inv())  # Assuming a continuation of the rotation
+                time_concatenated = np.concatenate((np.array(time_first).reshape((1,-1)),
+                                                    self.time.reshape((1,-1)),
+                                                    np.array(time_last).reshape((1,-1))), axis = 1)\
+                    .reshape(-1).astype(np.float64)
+                rotation_list = [self.rotation_nav]
+                rotation_list.append(rot_last)
+                rotation_list.insert(0, rot_first)
+
+
+                rot_vec_first = rot_first.as_rotvec().reshape((1,-1))
+                rot_vec_mid = self.rotation_nav.as_rotvec()
+                rot_vec_last = rot_last.as_rotvec().reshape((1,-1))
+
+                rotation_vec_tot = np.concatenate((rot_vec_first, rot_vec_mid, rot_vec_last), axis = 0)
+
+                Rotation_tot = RotLib.from_rotvec(rotation_vec_tot)
+
+
+
+                time_concatenated = np.array(time_concatenated).astype(np.float64)
+
+                linearSphericalInterpolator = Slerp(time_concatenated, Rotation_tot)
+
+                self.rotation_nav_interpolated = linearSphericalInterpolator(time_interpolation)
+
+
+
+
+
+
+        else:
+            print('Proper interpolation of transformation with constant velocity and rotation has not yet been implemented')
+            print('See https://www.geometrictools.com/Documentation/InterpolationRigidMotions.pdf')
+            #self.rotation_nav_interpolated, self.PositionInterpolated = self.interpolateTransforms()
+    def intrinsicTransformHSI(self, translation_ref_hsi, rot_hsi_ref_obj):
+
+        # An intrinsic transform is a transformation to another reference frame on the moving body, i.e. the IMU or an RGB cam
+        self.position_ecef = self.position_nav_interpolated + self.rotation_nav_interpolated.apply(translation_ref_hsi)
+
+        # Composing rotations. See:
+        # https: // docs.scipy.org / doc / scipy / reference / generated / scipy.spatial.transform.Rotation.__mul__.html
+        self.rotation_hsi = self.rotation_nav_interpolated * rot_hsi_ref_obj
+
+        self.quaternion_ecef = self.rotation_hsi.as_quat()
+        
+    def localTransform(self, frame):
+        self.IsLocal = True
+        self.LocalTransformFrame = frame
+
+        if frame == 'ENU':
+            self.position_nav_interpolated = self.Rotation_ecef_enu*self.position_nav_interpolated
+            self.rotation_nav_interpolated = self.Rotation_ecef_enu*self.rotation_nav_interpolated
+            self.position_nav = self.Rotation_ecef_enu * self.position_nav
+            self.rotation_nav = self.Rotation_ecef_enu * self.rotation_nav
+            self.rotation_hsi = self.Rotation_ecef_enu * self.rotation_hsi
+            self.position_nav = self.Rotation_ecef_enu * self.position_ecef
+        elif frame == 'NED':
+            self.localPositionInterpolated = self.Rotation_ecef_ned*self.position_nav_interpolated
+            self.localRotationInterpolated = self.Rotation_ecef_ned*self.rotation_nav_interpolated
+            self.localPosition = self.Rotation_ecef_ned * self.position_nav
+            self.localRotation = self.Rotation_ecef_ned * self.rotation_nav
+            self.rotation_hsi = self.Rotation_ecef_ned * self.rotation_hsi
+            self.position_nav = self.Rotation_ecef_ned * self.position_ecef
+        else:
+            print('Frame must be ENU or NED')
+    def localTransformInverse(self):
+
+        if self.IsLocal:
+            self.IsLocal = False
+            if self.LocalTransformFrame == 'ENU':
+                self.position_nav_interpolated = self.Rotation_ecef_enu.inv()*self.position_nav_interpolated
+                self.rotation_nav_interpolated = self.Rotation_ecef_enu.inv()*self.rotation_nav_interpolated
+                self.position_nav = self.Rotation_ecef_enu.inv() * self.position_nav
+                self.rotation_nav = self.Rotation_ecef_enu.inv() * self.rotation_nav
+                self.rotation_hsi = self.Rotation_ecef_enu.inv() * self.rotation_hsi
+                self.position_nav = self.Rotation_ecef_enu.inv() * self.position_ecef
+            elif self.LocalTransformFrame == 'NED':
+                self.localPositionInterpolated = self.Rotation_ecef_ned.inv()* self.position_nav_interpolated
+                self.localRotationInterpolated = self.Rotation_ecef_ned.inv()*self.rotation_nav_interpolated
+                self.localPosition = self.Rotation_ecef_ned.inv() * self.position_nav
+                self.localRotation = self.Rotation_ecef_ned.inv() * self.rotation_nav
+                self.rotation_hsi = self.Rotation_ecef_ned.inv() * self.rotation_hsi
+                self.position_nav = self.Rotation_ecef_ned.inv() * self.position_ecef
+            else:
+                print('Frame must be ENU or NED')
+        else:
+            print('Poses are defined globally already')
+    def defineRayDirections(self, dir_local):
+        self.rayDirectionsLocal = dir_local
+
+        n = self.position_ecef.shape[0]
+        m = dir_local.shape[0]
+
+        self.rayDirectionsGlobal = np.zeros((n, m, 3))
+
+        # Converts data from local frame to global
+        for i in range(n):
+            self.rayDirectionsGlobal[i, :, :] = self.rotation_hsi[i].apply(dir_local)
+    def intersect_with_mesh(self, mesh, max_ray_length, mesh_trans):
+        """Intersects the rays of the camera with the 3D triangular mesh
+
+        :param mesh: A mesh object read via the pyvista library
+        :type mesh: Pyvista mesh
+        :param max_ray_length: The upper bound length of the camera rays (it is determined )
+        :type max_ray_length: _type_
+        :param mesh_trans: The offset of the mesh
+        :type mesh_trans: _type_
+        """
+
+        n = self.rayDirectionsGlobal.shape[0]
+        m = self.rayDirectionsGlobal.shape[1]
+
+        self.points_ecef_crs = np.zeros((n, m, 3), dtype=np.float64)
+        self.normals_ecef_crs = np.zeros((n, m, 3), dtype=np.float64)
+
+        # Duplicate multiple camera centres
+        start_ECEF = np.einsum('ijk, ik -> ijk', np.ones((n, m, 3), dtype=np.float64), self.position_ecef).reshape((-1,3))
+
+        # Subtract the mesh offset to avoid rounding errors and perform intersection tests with "small coordinates"
+        start = start_ECEF - mesh_trans
+
+        dir = (self.rayDirectionsGlobal * max_ray_length).reshape((-1,3))
+
+        
+        
+        start_time = time.time()
+
+
+        
+        try:
+            # This will only work if exact Python version is rigght and you have PyEmbree
+            points, rays, cells = mesh.multi_ray_trace(origins=start, directions=dir, first_point=True, retry=True)
+        except:
+            # If you instead use embreex, python>3.6 will do
+            
+            
+            # If the faces are 
+            faces = mesh.regular_faces
+
+            # Convert PolyData to trimesh.Trimesh
+            tri_mesh = trimesh.Trimesh(vertices=mesh.points, faces=faces)
+
+            # Define an intersector object
+            ray_mesh_intersector = trimesh.ray.ray_pyembree.RayMeshIntersector(geometry=tri_mesh)
+
+            # Intersect data
+            count = 0
+            cells, rays, points = ray_mesh_intersector.intersects_id(ray_origins=start,  
+                                                                ray_directions=dir, 
+                                                                multiple_hits=False,
+                                                                return_locations=True)
+            
+        n_points = int(np.size(points)/3)
+        n_rays = int(np.size(start)/3)
+        # Recurring is that 1- 10s of rays fail to detect intersections using Trimesh.
+        # A handy fix is to iterate the failed intersections using individual ray tracing
+        # This equivalent to the retry=True in 
+        # https://docs.pyvista.org/version/stable/api/core/_autosummary/pyvista.PolyDataFilters.multi_ray_trace.html#pyvista.PolyDataFilters.multi_ray_trace
+        if n_points != n_rays:
+            n_missing = n_rays - n_points
+            print(f'Trimesh failed to find intersections for {n_missing} rays')
+            print(f'Ray tracing for these rays is retried in pyvista')
+
+            # Identify the missing intersections:
+            missing_rays = np.array(list( set(range(n_rays)) - set(rays) ))
+
+            # And ray trace them individually in VTK
+            for ray in missing_rays:
+                # Retry failed intersections with slow pyvista version
+                point, cell = mesh.ray_trace(start[ray,:], start[ray,:] + dir[ray,:], first_point=True)
+                cells = np.concatenate((cells, cell), axis=0)
+                points = np.concatenate((points, point.reshape((1,3))), axis=0)
+                rays = np.concatenate((rays, np.array([ray])), axis=0)
+            n_points = int(np.size(points)/3)
+            print('All rays successfully traced in VTK')
+
+        else:
+            print(f'All rays were successfully intersected with trimesh')
+            
+
+
+        stop_time = time.time()
+
+        normals = mesh.cell_normals[cells,:]
+
+        slit_image_number = np.floor(rays / m).astype(np.int32)
+
+        pixel_number = rays % m
+
+        
+
+
+        # Assign normals
+        self.points_ecef_crs[slit_image_number, pixel_number] = points + mesh_trans
+
+        self.normals_ecef_crs[slit_image_number, pixel_number] = normals
+
+        self.camera_to_seabed_ECEF = self.points_ecef_crs - start_ECEF.reshape((n, m, 3))
+
+
+        # Calculate
+        self.points_hsi_crs = np.zeros(self.camera_to_seabed_ECEF.shape)
+
+        self.normals_hsi_crs = np.zeros(self.normals_ecef_crs.shape)
+
+        self.depth_map = np.zeros((n, m))
+
+        # For local geometry (when vehicle fixed artificial light is used):
+        for i in range(n):
+            # Calculate vector from HSI to seabed in local coordinates (for artificial illumination)
+            self.points_hsi_crs[i, :, :] = (self.rotation_hsi[i].inv()).apply(self.camera_to_seabed_ECEF[i, :, :])
+
+            # Calculate surface normals of intersected triangles (for artificial illumination)
+            self.normals_hsi_crs[i,:,:] = (self.rotation_hsi[i].inv()).apply(self.normals_ecef_crs[i, :, :])
+
+            # Calculate a depth map (the z-component, 1D scanline)
+            self.depth_map[i, :] = self.points_hsi_crs[i, :, 2]/self.rayDirectionsLocal[:, 2]
+
+        
+
+        self.unix_time_grid = np.einsum('ijk, ik -> ijk', np.ones((n, m, 1), dtype=np.float64), self.time.reshape((-1,1)))
+        self.unix_time = self.unix_time_grid.reshape((-1, 1)) # Vector-form
+        self.pixel_nr_grid = np.matlib.repmat(np.arange(m), n, 1)
+        self.frame_nr_grid = np.matlib.repmat(np.arange(n).reshape(-1,1), 1, m)
+
+        
+    @staticmethod
+    def intersect_ray_with_earth_ellipsoid(p0, dir_hat, B):
+        """_summary_
+
+        :param p0: Ray origin
+        :type p0: (3,1) array of floats 
+        :param dir_hat: describing ray direction in some ECEF
+        :type dir_hat: (3,1) array of floats 
+        :param B: Ellipsoid matrix of earth so that (p0 + lam*dir_hat)' * B * (p0 + lam*dir_hat) = 1
+        :type B: (3, 3) matrix describing earth ellipsoid in some ECEF
+        """
+
+        # Solves equation lam^2 *(d_hat'B*d_hat) + lam * 2*(p0' * B* dir_hat) + (p0' *B* p0)= 1
+        a = np.transpose(dir_hat).dot(B.dot(dir_hat))
+        b = 2*np.transpose(p0).dot(B.dot(dir_hat))
+        c = np.transpose(p0).dot(B.dot(p0)) - 1
+
+        p = np.zeros(3)
+        p[0] = a
+        p[1] = b
+        p[2] = c
+
+        lam = np.roots(p)
+
+        hits = p0 + dir_hat*lam
+
+
+        return hits 
+
+    @staticmethod
+    def calculate_sun_directions(longitude, latitude, altitude, unix_time, degrees=True):
+        # Ensure all inputs are NumPy arrays
+        longitude = np.asarray(longitude).flatten()
+        latitude = np.asarray(latitude).flatten()
+        altitude = np.asarray(altitude).flatten()
+        unix_time = np.asarray(unix_time).flatten()
+
+        n = max(longitude.size, latitude.size, altitude.size, unix_time.size)
+
+        # If a single value is provided for any parameter, broadcast it to match the size of the other parameters
+        longitude = np.broadcast_to(longitude, (n,))
+        latitude = np.broadcast_to(latitude, (n,))
+        altitude = np.broadcast_to(altitude, (n,))
+        unix_time = np.broadcast_to(unix_time, (n,))
+
+        phi_s = np.zeros(n)
+        theta_s = np.zeros(n)
+
+        observer = ephem.Observer()
+
+        for i in range(n):
+            # Extract a single value from the arrays
+            observer.lon = str(longitude[i])
+            observer.lat = str(latitude[i])
+            observer.elev = altitude[i]
+            
+            sun = ephem.Sun()
+            observer.date = datetime.utcfromtimestamp(unix_time[i])
+            sun.compute(observer)
+
+            phi_s[i] = np.rad2deg(sun.az)
+            theta_s[i] = 90 - np.rad2deg(sun.alt)
+
+        if not degrees:
+            phi_s = np.deg2rad(phi_s)
+            theta_s = np.deg2rad(theta_s)
+
+        return phi_s, theta_s
+
+    def compute_view_directions_local_tangent_plane(self):
+        """Takes the intersection points and HSI camera positions and computes the angles from seabed to HSI with respect to the local tangent plane to the ellipsoid. 
+        """
+        n = self.rayDirectionsGlobal.shape[0]
+        m = self.rayDirectionsGlobal.shape[1]
+
+        self.seabed_to_camera_NED = np.zeros(self.camera_to_seabed_ECEF.shape)
+        self.normals_ned_crs = np.zeros(self.normals_ecef_crs.shape)
+        self.theta_v = np.zeros((n, m))
+        self.phi_v = np.zeros((n, m))
+
+        x_ecef = self.points_ecef_crs[:, :, 0].reshape((-1,1))
+        y_ecef = self.points_ecef_crs[:, :, 1].reshape((-1,1))
+        z_ecef = self.points_ecef_crs[:, :, 2].reshape((-1,1))
+        
+        lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
+
+        start = np.einsum('ijk, ik -> ijk', np.ones((n, m, 3), dtype=np.float64), self.position_ecef).reshape((-1,3))
+
+        x_hsi = start[:, 0].reshape((-1,1))
+        y_hsi = start[:, 1].reshape((-1,1))
+        z_hsi = start[:, 2].reshape((-1,1))
+
+        # Compute vectors from seabed intersections to HSI in NED
+        NED = pm.ecef2ned(x= x_hsi, y= y_hsi, z=z_hsi, lat0 = lats, lon0=lons, h0 = alts)
+
+        self.seabed_to_camera_NED = np.hstack((NED[0], NED[1], NED[2])).reshape((n, m, 3))
+
+        # For remote sensing with a sun-lit seafloor:
+        for i in range(n):
+            
+            R_ecef_2_ned = RotLib.from_matrix(rotation_matrix_ecef2ned(lon = lons[i], lat = lats[i]))
+
+            # Calculate vector from HSI to seabed in local tangent plane NED
+            #self.camera_to_seabed_NED[i, :, :] = R_ecef_2_ned.apply(self.camera_to_seabed_ECEF[i, :, :])
+
+            # Decompose vector to angles
+            polar = cartesian_to_polar(xyz = self.seabed_to_camera_NED[i,:,:])
+
+            self.theta_v[i, :] = polar[:,1]
+
+            self.phi_v[i, :] = polar[:,2]
+
+            # Calculate surface normals of intersected triangles (for artificial illumination)
+            self.normals_ned_crs[i, :, :] = R_ecef_2_ned.apply(self.normals_ecef_crs[i, :, :])
+
+            
+
+
+    def compute_sun_angles_local_tangent_plane(self):
+        n = self.rayDirectionsGlobal.shape[0]
+        m = self.rayDirectionsGlobal.shape[1]
+
+        x_ecef = self.points_ecef_crs[:, :, 0].reshape((-1,1))
+        y_ecef = self.points_ecef_crs[:, :, 1].reshape((-1,1)) 
+        z_ecef = self.points_ecef_crs[:, :, 2].reshape((-1,1))
+
+        lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
+
+        self.lats = lats
+        self.lons = lons
+        self.alts = alts
+
+        phi_s, theta_s = CameraGeometry.calculate_sun_directions(longitude = lons, latitude = lats, altitude = alts, unix_time = self.unix_time, degrees = True)
+
+        self.phi_s = phi_s.reshape((n, m, 1))
+
+        self.theta_s = theta_s.reshape((n, m, 1))
+
+        
+
+    def compute_elevation_mean_sealevel(self, source_epsg, geoid_path = 'data/world/geoids/egm08_25.gtx'):
+        n = self.rayDirectionsGlobal.shape[0]
+        m = self.rayDirectionsGlobal.shape[1]
+
+        x_ecef = self.position_ecef[:, 0].reshape((-1,1))
+        y_ecef = self.position_ecef[:, 1].reshape((-1,1))
+        z_ecef = self.position_ecef[:, 2].reshape((-1,1))
+
+        #lats, lons, alts = pm.ecef2geodetic(x = x_ecef, y = y_ecef, z = z_ecef)
+
+        
+
+        alts_msl = CameraGeometry.elevation_msl(x_ecef, y_ecef, z_ecef, source_epsg=source_epsg, geoid_path = geoid_path)
+        
+
+        self.hsi_alts_msl = np.einsum('ijk, ik -> ijk', np.ones((n, m, 1), dtype=np.float32), alts_msl.reshape((-1,1)))
+
+        
+    
+    @staticmethod
+    def elevation_msl(x_ecef, y_ecef, z_ecef, source_epsg, geoid_path):
+        """_summary_
+
+        :param x_ecef: _description_
+        :type x_ecef: _type_
+        :param y_ecef: _description_
+        :type y_ecef: _type_
+        :param z_ecef: _description_
+        :type z_ecef: _type_
+        :param source_epsg: _description_
+        :type source_epsg: _type_
+        :param geoid_path: _description_
+        :type geoid_path: _type_
+        :return: _description_
+        :rtype: _type_
+        """
+        
+        with rasterio.open(geoid_path) as src:
+
+            source_crs = CRS.from_epsg(source_epsg)
+                
+            target_crs = src.crs
+
+            transformer = Transformer.from_crs(source_crs, target_crs)
+
+            (lat, lon, alt_ell) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
+
+            undulation = np.zeros(lat.shape)
+            # Compute undulation and orthometric height for each point (height above MSL)
+            
+            for i, x, y in zip(range(lat.size), lon, lat):
+                undulation[i] = next(src.sample([(float(x), float(y))]))[0]
+            
+
+        
+        alt_msl = alt_ell - undulation
+
+        return alt_msl
+
+
+
+    
+
+    def compute_tide_level(self, path_tide, tide_format, constant_height = 0):
+
+        n = self.rayDirectionsGlobal.shape[0]
+        m = self.rayDirectionsGlobal.shape[1]
+
+        if path_tide == 'Undefined':
+
+            self.hsi_tide_gridded = constant_height*np.ones((n, m, 1))
+
+        else:
+
+            if tide_format == 'NMA':
+                try:
+                    df_tide = pd.read_csv(path_tide, sep='\s+', parse_dates=[0], index_col=0, comment='#', date_parser=parser.parse)
+
+                    # Convert the datetime index to Unix time and add column
+                    df_tide['UnixTime'] = df_tide.index.astype('int64') // 10**9  # Convert nanoseconds to seconds
+
+                    tide_height_NN2000 = 0.01*df_tide['Observations'] # Since in cm
+
+                    tide_timestamp = df_tide['UnixTime']
+                    
+                    hsi_tide_interp = interp1d(x = tide_timestamp, y= tide_height_NN2000)(x = self.time)
+
+                    # Make into gridded form:
+                    self.hsi_tide_gridded = np.einsum('ijk, ik -> ijk', np.ones((n, m, 1), dtype=np.float64), hsi_tide_interp.reshape((-1,1)))
+                except:
+                    #print('No tide file was found!!')
+                    self.hsi_tide_gridded = constant_height*np.ones((n, m, 1))
+
+
+
+            else: # A Good place to write parsers for other formats
+                TypeError
+        
+    def write_rgb_point_cloud(self, config, hyp, transect_string, extrapolate = True, minInd = None, maxInd = None):
+        wl_red = float(config['General']['red_wave_length'])
+        wl_green = float(config['General']['green_wave_length'])
+        wl_blue = float(config['General']['blue_wave_length'])
+        dir_point_cloud = config['Absolute Paths']['rgb_point_cloud_folder']
+
+        wavelength_nm = np.array([wl_red, wl_green, wl_blue])
+
+        # Localize the appropriate band indices used for analysis
+        band_ind_R = np.argmin(np.abs(wavelength_nm[0] - hyp.band2Wavelength))
+        band_ind_G = np.argmin(np.abs(wavelength_nm[1] - hyp.band2Wavelength))
+        band_ind_B = np.argmin(np.abs(wavelength_nm[2] - hyp.band2Wavelength))
+
+        if extrapolate == False:
+            rgb = hyp.dataCubeRadiance[minInd:maxInd, :, [band_ind_R, band_ind_G, band_ind_B]]
+        else:
+            rgb = hyp.dataCubeRadiance[:, :, [band_ind_R, band_ind_G, band_ind_B]]
+
+
+        points = self.points_ecef_crs[self.points_ecef_crs != 0].reshape((-1,3))
+        rgb_points = (rgb[self.points_ecef_crs != 0] / rgb.max()).astype(np.float64).reshape((-1,3))
+        pcd = o3d.geometry.PointCloud()
+        pcd.points = o3d.utility.Vector3dVector(points)
+        pcd.colors = o3d.utility.Vector3dVector(rgb_points)
+        o3d.io.write_point_cloud(dir_point_cloud + transect_string + '.ply', pcd)
+
+
+    #def transformRays(self, rays):
+        # Rays are a n x m x 3 set of rays where n is each time step and coincides with the rotations and translations:
+
+class FeatureCalibrationObject():
+    def __init__(self, type, config):
+        self.config = config
+        self.type = type
+        self.HSIPositionFeature = [] # Function of feature line
+        self.HSIRotationFeature = [] #
+        self.isfirst = True
+
+    def load_cam_calibration(self, filename_cal, config):
+        calHSI = CalibHSI(file_name_cal_xml=filename_cal)  # Generates a calibration object
+        self.f = calHSI.f
+        self.v_c = calHSI.cx
+        self.k1 = calHSI.k1
+        self.k2 = calHSI.k2
+        self.k3 = calHSI.k3
+
+        self.trans_x = calHSI.tx
+        self.trans_y = calHSI.ty
+        self.trans_z = calHSI.tz
+
+        self.rot_x = calHSI.rx
+        self.rot_y = calHSI.ry
+        self.rot_z = calHSI.rz
+
+        
+
+        #if eval(config['General']['isFlippedRGB']):
+        #    self.trans_x *= -1
+        #    self.trans_y *= -1
+        #if eval(config['General']['isFlippedHSI']):
+        #    self.rot_z += np.pi
+
+
+    def appendGeometry(self, hsiGis, cameraGeometry, binning):
+        # Step 1: Define the global projected position of features
+        point_feature_gt = hsiGis.features_points
+        # Define the hsi pixel number
+        pixel = self.bilinearInterpolation(x1_x=hsiGis.x1_x_hsi, y1_y=hsiGis.y1_y_hsi, f_Q=hsiGis.v_datacube_hsi)
+        # Define the translation:
+        # First define the time stamp for the four lines:
+        line_nr = hsiGis.u_datacube_hsi.astype(np.int64)
+
+        trans_Q_00 = cameraGeometry.position_ecef[line_nr[:, 0]]
+        trans_Q_01 = cameraGeometry.position_ecef[line_nr[:, 1]]
+        trans_Q_10 = cameraGeometry.position_ecef[line_nr[:, 2]]
+        trans_Q_11 = cameraGeometry.position_ecef[line_nr[:, 3]]
+
+        translationHSI = self.bilinearInterpolationPosition(x1_x=hsiGis.x1_x_hsi, y1_y=hsiGis.y1_y_hsi, trans_Q_00=trans_Q_00, trans_Q_01=trans_Q_01, trans_Q_10=trans_Q_10,
+                                                              trans_Q_11=trans_Q_11)
+
+        rot_Q_00 = cameraGeometry.rotation_nav_interpolated[line_nr[:, 0]]
+        rot_Q_01 = cameraGeometry.rotation_nav_interpolated[line_nr[:, 1]]
+        rot_Q_10 = cameraGeometry.rotation_nav_interpolated[line_nr[:, 2]]
+        rot_Q_11 = cameraGeometry.rotation_nav_interpolated[line_nr[:, 3]]
+
+        rotationRGB = self.bilinearInterpolationRotation(x1_x=hsiGis.x1_x_hsi, y1_y=hsiGis.y1_y_hsi,
+                                                              rot_Q_00=rot_Q_00, rot_Q_10=rot_Q_10, rot_Q_01=rot_Q_01,
+                                                              rot_Q_11=rot_Q_11)
+        if self.isfirst:
+            self.point_feature_gt = point_feature_gt
+            self.pixel = pixel
+            self.translationHSI = translationHSI
+            self.rotationRGB = rotationRGB
+            self.binning = np.array([binning]).reshape((1,1))
+            self.diff = hsiGis.diff
+
+            self.isfirst = False
+        else:
+            # Add observations
+            self.diff = np.concatenate((self.diff, hsiGis.diff), axis = 0)
+            self.point_feature_gt = np.concatenate((self.point_feature_gt, point_feature_gt), axis = 0)
+            self.pixel = np.concatenate((self.pixel, pixel), axis = 0)
+            self.translationHSI = np.concatenate((self.translationHSI, translationHSI), axis = 0)
+            self.rotationRGB = np.concatenate((self.rotationRGB, rotationRGB), axis = 0)
+
+
+
+    #def defineRayDirections
+    def bilinearInterpolation(self, x1_x, y1_y, f_Q):
+
+
+        f_x_y1 = (1 - x1_x)*f_Q[:, 0] + x1_x*f_Q[:, 1]
+        f_x_y2 = (1 - x1_x) * f_Q[:, 2] + x1_x * f_Q[:, 3]
+
+        f_x_y = (1 - y1_y)*f_x_y1 + y1_y*f_x_y2
+
+        return f_x_y
+    def bilinearInterpolationPosition(self, x1_x, y1_y, trans_Q_00, trans_Q_01, trans_Q_10,
+                                                              trans_Q_11):
+
+        trans_tot = np.zeros(trans_Q_00.shape)
+        for i in range(3):
+
+            f_x_y1 = (1 - x1_x)*trans_Q_00[:, i] + x1_x*trans_Q_01[:, i]
+            f_x_y2 = (1 - x1_x) * trans_Q_10[:, i] + x1_x * trans_Q_11[:, i]
+
+            f_x_y = (1 - y1_y)*f_x_y1 + y1_y*f_x_y2
+            trans_tot[:, i] = f_x_y
+
+
+        return trans_tot
+
+    def bilinearInterpolationRotation(self, x1_x, y1_y, rot_Q_00, rot_Q_10, rot_Q_01, rot_Q_11):
+
+        # Define all rotations from rot_Q_00
+        delta_rot0_rot = np.zeros((4, x1_x.shape[0], 3))
+        # Define all relative rotations
+        delta_rot0_rot[1, :, :] = (rot_Q_01 * rot_Q_00.inv()).as_rotvec(degrees = False)
+        delta_rot0_rot[2, :, :] = (rot_Q_10 * rot_Q_00.inv()).as_rotvec(degrees = False)
+        delta_rot0_rot[3, :, :] = (rot_Q_11 * rot_Q_00.inv()).as_rotvec(degrees = False)
+
+        Q_rots_permuted = np.transpose(delta_rot0_rot, axes = [2, 1, 0])
+
+        rot_vec_final = np.zeros((3, x1_x.shape[0]))
+
+        for i  in range(3):
+            f_Q = Q_rots_permuted[i, :, :]
+            f_x_y1 = (1 - x1_x) * f_Q[:, 0] + x1_x * f_Q[:, 1]
+            f_x_y2 = (1 - x1_x) * f_Q[:, 2] + x1_x * f_Q[:, 3]
+
+            f_x_y = (1 - y1_y) * f_x_y1 + y1_y * f_x_y2
+
+            rot_vec_final[i, :] = f_x_y
+
+        delta_rot_interp = RotLib.from_rotvec(np.transpose(rot_vec_final))
+
+        # Compose the values to rot0
+        rot_tot = delta_rot_interp * rot_Q_00
+
+
+        return rot_tot
+
+    
+    # At the time of updated parameters
+    def reprojectFeaturesHSI(self):
+        rot_hsi_rgb = np.array([self.rot_z, self.rot_y, self.rot_x]) * 180 / np.pi
+
+        self.rotation_hsi_rgb = RotLib.from_euler('ZYX', rot_hsi_rgb, degrees=True)
+
+        self.rotation_hsi = self.rotationRGB * self.rotation_hsi_rgb # Composing rotations.
+
+        self.HSIToFeaturesGlobal = self.point_feature_gt - self.translationHSI
+
+        n = self.HSIToFeaturesGlobal.shape[0]
+
+        self.HSIToFeaturesLocal = np.zeros(self.HSIToFeaturesGlobal.shape)
+        for i in range(n):
+            self.HSIToFeaturesLocal[i, :] = (self.rotation_hsi[i].inv()).apply(
+                self.HSIToFeaturesGlobal[i, :])
+
+            self.HSIToFeaturesLocal[i, :] /= self.HSIToFeaturesLocal[i, 2]
+
+
+
+
+def compute_camera_rays_from_parameters(pixel_nr, cx, f, k1, k2, k3):
+    """_summary_
+
+    :param pixel_nr: _description_
+    :type pixel_nr: _type_
+    :param rot_x: _description_
+    :type rot_x: _type_
+    :param rot_y: _description_
+    :type rot_y: _type_
+    :param rot_z: _description_
+    :type rot_z: _type_
+    :param cx: _description_
+    :type cx: _type_
+    :param f: _description_
+    :type f: _type_
+    :param k1: _description_
+    :type k1: _type_
+    :param k2: _description_
+    :type k2: _type_
+    :param k3: _description_
+    :type k3: _type_
+    :return: _description_
+    :rtype: _type_
+    """
+
+    u = pixel_nr + 1
+
+    # Express uhi ray directions in uhi frame using line-camera model
+    x_norm_lin = (u - cx) / f
+
+    x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
+                        k2 * ((u - cx) / 1000) ** 3 + \
+                        k3 * ((u - cx) / 1000) ** 2) / f
+
+    x_norm = x_norm_lin + x_norm_nonlin
+
+    return x_norm
+
+
+def reproject_world_points_to_hsi_plane(trans_hsi_body, rot_hsi_body, pos_body, rot_body, points_world):
+    """Reprojects world points to local image plane coordinates (x_h, y_h, 1)
+
+    :param trans_hsi_body: lever arm from body center to hsi focal point
+    :type trans_hsi_body: _type_
+    :param rot_hsi_body: boresight rotation 
+    :type rot_hsi_body: Scipy rotation object
+    :param pos_body: The earth fixed earth centered position of the vehicle body centre
+    :type pos_body: _type_
+    :param rot_body: The rotation of the body in ECEF
+    :type rot_body: Scipy rotation object
+    :param points_world: World points in ECEF
+    :type points_world: _type_
+    :return: The reprojection coordinates
+    :rtype: ndarray(n, 3)
+    """
+
+    
+
+    # We compose the hypothesized boresight (rot_hsi_body) an lever arm (trans_hsi_body) to get the hypothesized position/orientation
+    # of the hyperspectral imager
+    rotation_hsi = rot_body * rot_hsi_body
+    position_hsi = pos_body + rot_body.apply(trans_hsi_body)
+
+    # Given the positions, the hsi-point vector can be expressed in ECEF
+    hsi_to_feature_global = points_world - position_hsi
+
+    # Number of features to iterate
+    n = hsi_to_feature_global.shape[0]
+
+    # We can now express the hsi-point vector in the HSI frame and normalize by the z component to find the image plane projection
+    hsi_to_feature_local = np.zeros(hsi_to_feature_global.shape)
+    for i in range(n):
+        # The vector expressed in HSI frame
+        hsi_to_feature_local[i, :] = (rotation_hsi[i].inv()).apply(hsi_to_feature_global[i, :])
+
+        # The vector normalized to lie on the virtual plane
+        hsi_to_feature_local[i, :] /= hsi_to_feature_local[i, 2]
+    
+    return hsi_to_feature_local
+
+
+
+
+def interpolate_poses(timestamp_from, pos_from, rot_from, timestamps_to, extrapolate = True):
+    """
+
+    :param timestamp_from:
+    Original timestamps
+    :param pos_from: numpy array (n,3)
+    Original positions
+    :param rot_from: Rotation-object (n rotations)
+    Original orientations
+    :param timestamps_to:
+    Timestamps desired for position and orientations
+    :return:
+    """
+    """
+    min_to = np.min(timestamps_to)
+    max_to = np.max(timestamps_to)
+
+    min_from = np.min(timestamp_from)
+    max_from = np.max(timestamp_from)
+
+    minInd = np.argmin(np.abs(min_from - timestamps_to))
+    maxInd = np.argmin(np.abs(max_from - timestamps_to))
+
+    # If navigation data aka "from" is made properly, min_from<<min_to, and max_from >> max_to
+    
+    if timestamps_to[minInd] < min_from:
+        minInd += 1
+    if timestamps_to[maxInd] > min_from: # So if the max index is 
+        maxInd -= 1
+    """
+
+    min_ind = 0
+    max_ind = timestamps_to.size
+
+
+    # Setting use_absolute_position to True means that position calculations are done with absolute
+    referenceGeometry = CameraGeometry(pos=pos_from,
+                               rot=rot_from,
+                               time=timestamp_from)
+
+    # We exploit a method from the camera object
+    referenceGeometry.interpolate(time_hsi=timestamps_to,
+                          minIndRGB=min_ind,
+                          maxIndRGB=max_ind,
+                          extrapolate=extrapolate)
+
+
+
+    position_to = referenceGeometry.position_nav_interpolated
+
+    quaternion_to = referenceGeometry.rotation_nav_interpolated.as_quat()
+
+    return position_to, quaternion_to
+
+
+
+
+def cartesian_to_polar(xyz):
+    """Converts from 3D cartesian coordinates to polar coordinates
+
+    :param xyz: _description_
+    :type xyz: (n,3) numpy array
+    :return: Radii, Elevations, Azimuths
+    :rtype: (n,3) numpy array of radii, theta, phi
+    """
+    polar = np.zeros(xyz.shape)
+    xy = xyz[:,0]**2 + xyz[:,1]**2
+    polar[:,0] = np.sqrt(xy + xyz[:,2]**2) # Radii
+    polar[:,1] = np.arctan2(np.sqrt(xy), np.abs(xyz[:,2])) # for elevation angle defined from Z-axis down [0-90]
+    polar[:,2] = np.arctan2(xyz[:,1], xyz[:,0]) # Azimuth
+
+    return polar
+
+
+
+
+
+
+
+
+
+
+def rotation_matrix_ecef2ned(lon, lat):
+    """
+    Computes the rotation matrix R from earth-fixed-earth centered (ECEF) to north-east-down (NED).
+    :param lat: float in range [-90, 90]
+    The latitude in degrees
+    :param lon: float in range [-180, 180]
+    :return R_ned_ecef: numpy array of shape (3,3)
+    rotation matrix ECEF to NED
+    """
+    R_ned_ecef = rot_mat_ned_2_ecef(lon=lon, lat=lat)
+    return np.transpose(R_ned_ecef)
+
+def rotation_matrix_ecef2enu(lon, lat):
+    l = np.deg2rad(lon)
+    mu = np.deg2rad(lat)
+
+    R_ecef_ned = rotation_matrix_ecef2ned(lon=lon, lat=lat)
+    R_ecef_enu = np.zeros(R_ecef_ned.shape)
+    #
+    R_ecef_enu[[0, 1]] = R_ecef_ned[[1, 0]] # Swap rows
+    R_ecef_enu[2] = -R_ecef_ned[2] # Switch signs to compensate for up and down
+
+
+    
+    return R_ecef_enu
+
+
+def convert_rotation_ned_2_ecef(rot_obj_ned, position, is_geodetic = True, epsg_pos = 4326):
+    """
+
+    :param rot_obj_:
+    :param position:
+    The position
+    :param is_geodetic: bool
+    Whether position is geodetic
+    :return:
+    """
+
+
+class GeoPose:
+    """
+    An object that allows to input positions with arbitrary CRS, and orientations either wrt ECEF or NED. As in other
+    places in the project, the orientations are abstracted with rotation objects. The main use case is formatting poses
+    to the correct CRS.
+    """
+    def __init__(self, timestamps, rot_obj, rot_ref, pos, pos_epsg):
+        self.timestamps = timestamps
+        if rot_ref == 'NED':
+            self.rot_obj_ned = rot_obj
+            self.rot_obj_ecef = None
+        elif rot_ref == 'ECEF':
+            self.rot_obj_ned = None
+            self.rot_obj_ecef = rot_obj
+        else:
+            print('This rotation reference is not supported')
+            TypeError
+
+        # Define position
+        self.position = pos
+        self.epsg = pos_epsg
+
+
+        self.lat = None
+        self.lon = None
+        self.hei = None
+
+        self.compute_geodetic_position()
+        self.compute_geocentric_orientation()
+        self.compute_ned_orientation()
+        self.compute_ned_2_ecef()
+
+
+    def compute_geodetic_position(self, epsg_geod = 4326):
+        """
+            Function for transforming positions to latitude longitude height
+            :param epsg_geod: int
+            EPSG code of the transformed geodetic coordinate system
+        """
+        # If geocentric position has not been defined.
+        from_CRS = CRS.from_epsg(self.epsg)
+        geod_CRS = CRS.from_epsg(epsg_geod)
+        transformer = Transformer.from_crs(from_CRS, geod_CRS)
+
+        x = self.position[:, 0].reshape((-1, 1))
+        y = self.position[:, 1].reshape((-1, 1))
+        z = self.position[:, 2].reshape((-1, 1))
+
+        (lat, lon, hei) = transformer.transform(xx=x, yy=y, zz=z)
+
+        self.epsg_geod = epsg_geod
+        self.lat = lat.reshape((self.position.shape[0], 1))
+        self.lon = lon.reshape((self.position.shape[0], 1))
+        self.hei = hei.reshape((self.position.shape[0], 1))
+
+    def compute_geocentric_position(self, epsg_geocsc):
+        """
+            Function for transforming positions to geocentric
+            :param epsg_geod: int
+            EPSG code of the transformed geodetic coordinate system
+        """
+
+        from_CRS = CRS.from_epsg(self.epsg)
+        geod_CRS = CRS.from_epsg(epsg_geocsc)
+        transformer = Transformer.from_crs(from_CRS, geod_CRS)
+
+        x = self.position[:, 0].reshape((-1, 1))
+        y = self.position[:, 1].reshape((-1, 1))
+        z = self.position[:, 2].reshape((-1, 1))
+
+        (x, y, z) = transformer.transform(xx=x, yy=y, zz=z)
+
+        self.pos_geocsc = np.concatenate((x, y, z), axis = 1)
+
+    def compute_geocentric_orientation(self):
+        if self.rot_obj_ecef == None:
+            # Define rotations from ned to ecef
+            if self.lat.any == None:
+                # Needed to encode rotation between NED and ECEF
+                self.compute_geodetic_position()
+
+            R_body_2_ned = self.rot_obj_ned
+            R_ned_2_ecef = self.compute_ned_2_ecef()
+            R_body_2_ecef = R_ned_2_ecef*R_body_2_ned
+
+            self.rot_obj_ecef = R_body_2_ecef
+
+        else:
+            pass
+
+    def compute_ned_orientation(self):
+        if self.rot_obj_ned == None:
+            # Define rotations from body to ecef
+            R_body_2_ecef = self.rot_obj_ecef
+
+            # Define rotation from ecef 2 ned
+            R_ecef_2_ned = self.compute_ned_2_ecef().inv()
+
+            # Compose
+            R_body_2_ned = R_ecef_2_ned*R_body_2_ecef
+
+            self.rot_obj_ned = R_body_2_ned
+
+
+        else:
+            pass
+
+    def compute_ned_2_ecef(self):
+
+        N = self.lat.shape[0]
+        rot_mats_ned_2_ecef = np.zeros((N, 3, 3), dtype=np.float64)
+        
+        for i in range(N):
+            rot_mats_ned_2_ecef[i,:,:] = rot_mat_ned_2_ecef(lat=self.lat[i], lon = self.lon[i])
+
+
+        self.rot_obj_ned_2_ecef = RotLib.from_matrix(rot_mats_ned_2_ecef)
+
+        return self.rot_obj_ned_2_ecef
+
+    
+
+
+def rot_mat_ned_2_ecef(lat, lon):
+    """
+    Computes the rotation matrix R from north-east-down (NED) to earth-fixed-earth centered (ECEF)
+    :param lat: float in range [-90, 90]
+    The latitude in degrees
+    :param lon: float in range [-180, 180]
+    :return R_ned_ecef: numpy array of shape (3,3)
+    rotation matrix from NED to ECEF
+    """
+
+    # Ensure lat and lon are scalar values
+    lat_scalar = lat[0] if isinstance(lat, np.ndarray) else lat
+    lon_scalar = lon[0] if isinstance(lon, np.ndarray) else lon
+
+    # Convert to radians
+    l = np.deg2rad(lon_scalar)
+    mu = np.deg2rad(lat_scalar)
+
+    # Compute rotation matrix
+    # TODO: add source
+    R_ned_ecef = np.array([[-np.cos(l) * np.sin(mu), -np.sin(l), -np.cos(l) * np.cos(mu)],
+                           [-np.sin(l) * np.sin(mu), np.cos(l), -np.sin(l) * np.cos(mu)],
+                           [np.cos(mu), 0, -np.sin(mu)]])
+    return R_ned_ecef
+
+
+def read_raster(filename, out_crs="EPSG:3857", use_z=False):
+    """Read a raster to a ``pyvista.StructuredGrid``.
+
+    This will handle coordinate transformations.
+    """
+    from rasterio import transform
+    import rioxarray
+    # Read in the data
+    data = rioxarray.open_rasterio(filename)
+    values = np.asarray(data)
+    data.rio.nodata
+    nans = values == data.rio.nodata
+    if np.any(nans):
+        # values = np.ma.masked_where(nans, values)
+        values[nans] = np.nan
+    # Make a mesh
+    xx, yy = np.meshgrid(data["x"], data["y"])
+    if use_z and values.shape[0] == 1:
+        # will make z-comp the values in the file
+        zz = values.reshape(xx.shape)
+    else:
+        # or this will make it flat
+        zz = np.zeros_like(xx)
+    mesh = pv.StructuredGrid(xx, yy, zz)
+    pts = mesh.points
+    lon, lat = transform(data.rio.crs, out_crs, pts[:, 0], pts[:, 1])
+    mesh.points[:, 0] = lon
+    mesh.points[:, 1] = lat
+    mesh["data"] = values.reshape(mesh.n_points, -1, order="F")
+    return mesh
+
+def dem_2_mesh(path_dem, model_path, config):
+    """
+    A function for converting a specified DEM to a 3D mesh model (*.vtk, *.ply or *.stl). 
+    Consequently, mesh should be thought of as 2.5D representation.
+    In the case 
+
+    :param path_dem: _description_
+    :type path_dem: _type_
+    :param model_path: _description_
+    :type model_path: _type_
+    :param config: _description_
+    :type config: _type_
+    """
+
+
+    # The desired CRS for the model must be same as positions, orientations
+    epsg_geocsc = config['Coordinate Reference Systems']['geocsc_epsg_export']
+
+    # Intermediate point cloud format
+    output_xyz = model_path.split(sep = '.')[0] + '.xyz'
+
+    # Open the input raster dataset
+    ds = gdal.Open(path_dem)
+
+    if ds is None:
+        print(f"Failed to open {path_dem}")
+    else:
+        # Read the first band (band index is 1)
+        band = ds.GetRasterBand(1)
+        no_data_value = band.GetNoDataValue()
+        if band is None:
+            print(f"Failed to open band 1 of {path_dem}")
+        else:
+            # Get the geotransform information to calculate coordinates
+            geotransform = ds.GetGeoTransform()
+            x_origin = geotransform[0]
+            y_origin = geotransform[3]
+            x_resolution = geotransform[1]
+            y_resolution = geotransform[5]
+            # Get the CRS information
+            spatial_reference = osr.SpatialReference(ds.GetProjection())
+
+            # Get the EPSG code
+            epsg_proj = None
+            if spatial_reference.IsProjected():
+                epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 1)
+                is_projected = True
+                config.set('Coordinate Reference Systems', 'dem_epsg', str(epsg_proj))
+            elif spatial_reference.IsGeographic():
+                epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 0)
+                proj = ds.GetProjection()
+                is_projected = False
+
+
+            # Automatically set
+            
+            
+            # Get the band's data as a NumPy array of float64 (important)
+            band_data = band.ReadAsArray().astype(np.float64)
+
+            # Create a mask to identify no-data values
+            mask = band_data != no_data_value
+
+            # Create and open the output XYZ file for writing if it does not exist:
+            if not os.path.exists(output_xyz):
+                with open(output_xyz, 'w') as xyz_file:
+                    # Write data to the XYZ file using the mask and calculated coordinates
+                    for y in range(ds.RasterYSize):
+                        for x in range(ds.RasterXSize):
+                            if mask[y, x]:
+                                x_coord = x_origin + x * x_resolution
+                                y_coord = y_origin + y * y_resolution
+                                xyz_file.write(f"{x_coord} {y_coord} {band_data[y, x]}\n")
+            else:
+                print('*.xyz already exists, ignoring re-creation')
+            # Clean up
+            ds = None
+            band = None
+    
+
+    points = np.loadtxt(output_xyz)
+    points_offset = np.mean(points, axis = 0)
+
+    # Create a pyvista point cloud object (just to avoid precision problems)
+    cloud = pv.PolyData(points-points_offset)
+    
+    # TODO: Apply patch to avoid crash for triangulation when using big DEM files
+    # Generate a mesh from points
+    mesh = cloud.delaunay_2d(progress_bar=True)
+
+    # Transform the mesh points from projected to geocentric ECEF.
+    geocsc = CRS.from_epsg(epsg_geocsc)
+
+    if epsg_proj == 'EPSG': # If a geographic CRS
+        pass
+    else:
+        proj = CRS.from_epsg(epsg_proj)
+
+    transformer = Transformer.from_crs(proj, geocsc)
+
+    # Convert to proper coordinates
+    points_proj = mesh.points + points_offset
+
+    if is_projected:
+        x_proj = points_proj[:, 0].reshape((-1, 1))
+        y_proj = points_proj[:, 1].reshape((-1, 1))
+    else:
+        x_proj = points_proj[:, 1].reshape((-1, 1))
+        y_proj = points_proj[:, 0].reshape((-1, 1))
+    
+    h_proj = points_proj[:, 2].reshape((-1, 1))
+
+    (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=x_proj, yy=y_proj, zz=h_proj)
+
+    # Introduce mesh offsets in ECEF sized numbers seem to cause troubles:
+    offset_x = np.mean(x_ecef.reshape(-1))
+    offset_y = np.mean(y_ecef.reshape(-1))
+    offset_z = np.mean(z_ecef.reshape(-1))
+
+    mesh.points[:, 0] = x_ecef.reshape(-1) - offset_x
+    mesh.points[:, 1] = y_ecef.reshape(-1) - offset_y
+    mesh.points[:, 2] = z_ecef.reshape(-1) - offset_z
+   
+
+    # Save mesh
+    mesh.save(model_path)
+    # Save mesh meta
+    # Define your metadata dictionary
+    metadata = {
+        "offset_x": offset_x,
+        "offset_y": offset_y,
+        "offset_z": offset_z,
+        "epsg_code": geocsc.to_epsg(),  # Example EPSG code, replace with your actual code
+        "data_type": str(mesh.points.dtype),  # Add other metadata entries here
+    }
+
+    model_meta_path = model_path.split('.')[0] + '_meta.json' 
+    # Open the file in write mode with proper indentation
+    with open(model_meta_path, "w") as f:
+        # Write the dictionary to the file using JSON dump
+        json.dump(metadata, f)
+
+
+def crop_geoid_to_pose(path_dem, config, geoid_path = 'data/world/geoids/egm08_25.gtx'):
+    # The desired CRS for the model must be same as positions, orientations
+    epsg_geocsc = config['Coordinate Reference Systems']['geocsc_epsg_export']
+
+    # Open the input raster dataset
+    
+    ds = gdal.Open(geoid_path)
+
+    df_pose = pd.read_csv(config['Absolute Paths']['pose_path'])
+
+    # Find CRS of DEM
+    spatial_reference = osr.SpatialReference(ds.GetProjection())
+
+
+    # Get the EPSG code
+    epsg_proj = None
+    if spatial_reference.IsProjected():
+        epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 1)
+    elif spatial_reference.IsGeographic():
+        epsg_proj = spatial_reference.GetAttrValue("AUTHORITY", 0)
+    
+    # Transform points to DEM CRS
+    geocsc = CRS.from_epsg(epsg_geocsc)
+    proj = ds.GetProjection()
+    transformer = Transformer.from_crs(geocsc, proj)
+
+    x_ecef = df_pose[' X'].values.reshape((-1, 1))
+    y_ecef = df_pose[' Y'].values.reshape((-1, 1))
+    z_ecef = df_pose[' Z'].values.reshape((-1, 1))
+
+    (x_proj, y_proj, z_proj) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
+
+    coords_horz = np.concatenate((x_proj.reshape((-1,1)), y_proj.reshape((-1,1))), axis = 1)
+
+    # Determine bounding rectangle ()
+    polygon = MultiPoint(coords_horz).envelope
+    # Corners
+    x, y = polygon.exterior.xy
+    x = np.array(x)
+    y = np.array(y)
+
+    # Determine padding
+    padding = float(config['General']['max_ray_length'])
+
+    if spatial_reference.IsProjected():
+        # Add padding to 
+        xmin = x.min() - padding
+        ymin = y.min() - padding
+        xmax = x.max() + padding
+        ymax = y.max() + padding
+    elif spatial_reference.IsGeographic():
+        # Must translate metric padding into increments in lon/lat
+        (x_new, y_new, z_new) = pm.enu2geodetic(e= np.array([-padding, padding]), n= np.array([-padding, padding]), u = 0, lon0=np.mean(y), lat0=np.mean(x), h0 = 0)
+        delta_x = x_new[1] - np.mean(x)
+        delta_y = y_new[1] - np.mean(y)
+
+        # Swap x and y because x, y above is latitude, longitude and Rasterio expects opposite
+        ymin = x.min() - delta_x
+        xmin = y.min() - delta_y
+        ymax = x.max() + delta_x
+        xmax = y.max() + delta_y
+
+        minx, miny, maxx, maxy = [xmin, ymin, xmax, ymax]  # Replace with actual coordinates
+
+        
+
+    # Crops the DEM to the appropriate bounds and writes a new file (Copies CRS info from Geoid)
+    crop_dem_from_bounds(minx, miny, maxx, maxy, dem_path_source=geoid_path, dem_path_target=path_dem)
+     
+
+
+def crop_dem_from_bounds(minx, miny, maxx, maxy, dem_path_source, dem_path_target):
+
+    dem_dataset = rasterio.open(dem_path_source)
+    res_x = dem_dataset.transform.a
+    res_y = -dem_dataset.transform.e
+
+    if maxx-minx < res_x:
+        minx += -res_x
+        maxx += res_x
+    
+    if maxy-miny < res_y:
+        miny += -res_y
+        maxy += res_y
+
+    window = from_bounds(minx, miny, maxx, maxy, dem_dataset.transform)
+
+    window = Window(window.col_off, window.row_off, np.ceil(window.width), np.ceil(window.height))
+
+    cropped_dem_data = dem_dataset.read(window=window)
+
+    # Update the transform based on the new window
+    new_transform = dem_dataset.window_transform(window)
+    new_height, new_width = cropped_dem_data.shape[1], cropped_dem_data.shape[2]
+
+    # Create a new dataset for the cropped DEM
+    cropped_dem_profile = dem_dataset.profile.copy()
+    cropped_dem_profile.update({
+        'width': new_width,
+        'height': new_height,
+        'transform': new_transform
+    })
+
+
+    with rasterio.open(dem_path_target, 'w', **cropped_dem_profile) as dst:
+        dst.write(cropped_dem_data)
+
+
+def position_transform_ecef_2_llh(position_ecef, epsg_from, epsg_to, config):
+    """
+    Function for transforming ECEF positions to latitude longitude height
+    :param position_ecef: numpy array floats (n,3)
+    :param epsg_from: int
+    EPSG code of the original geocentric coordinate system (ECEF)
+    :param epsg_to: int
+    EPSG code of the transformed geodetic coordinate system
+    :return lat_lon_hei: numpy array floats (n,3)
+    latitude, longitude ellipsoid height.
+    """
+    geocsc = CRS.from_epsg(epsg_from)
+    geod = CRS.from_epsg(epsg_to)
+    transformer = Transformer.from_crs(geocsc, geod)
+
+    x_ecef = position_ecef[:, 0].reshape((-1, 1))
+    y_ecef = position_ecef[:, 1].reshape((-1, 1))
+    z_ecef = position_ecef[:, 2].reshape((-1, 1))
+
+    (lat, lon, hei) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
+
+    lat_lon_hei = np.zeros(position_ecef.shape)
+    lat_lon_hei[:, 0] = lat.reshape((position_ecef.shape[0], 1))
+    lat_lon_hei[:, 1] = lon.reshape((position_ecef.shape[0], 1))
+    lat_lon_hei[:, 2] = hei.reshape((position_ecef.shape[0], 1))
+
+    return lat_lon_hei
```

### Comparing `gref4hsi-0.2.1/gref4hsi/utils/gis_tools.py` & `gref4hsi-0.2.2/gref4hsi/utils/gis_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1147 +1,1251 @@
-# Python standard lib
-import os
-from concurrent.futures import ThreadPoolExecutor
-
-# Third party
-import cv2 as cv
-import geopandas as gpd
-import matplotlib.pyplot as plt
-import numpy as np
-from pyproj import CRS, Transformer
-import rasterio
-from rasterio.features import geometry_mask
-from rasterio.warp import calculate_default_transform, reproject, Resampling
-from osgeo import gdal, osr
-from shapely.geometry import Polygon, mapping, MultiPoint
-from sklearn.neighbors import NearestNeighbors
-from spectral import envi
-import spectral as sp
-import h5py
-from scipy.spatial.transform import Rotation as RotLib
-
-# Lib modules
-from gref4hsi.utils.colours import Image as Imcol
-
-# ENVI datatype conversion dictionary
-dtype_dict = {1:np.uint8,
-             2:np.int16,
-             3:np.int32,
-             4:np.float32,
-             5:np.float64,
-             12:np.uint16,
-             13:np.uint32,
-             14:np.int64,
-             15:np.uint64}
-
-class GeoSpatialAbstractionHSI():
-    def __init__(self, point_cloud, transect_string, config_crs):
-        self.name = transect_string
-        self.points_geocsc = point_cloud
-
-        self.epsg_geocsc = config_crs.epsg_geocsc
-        
-        self.n_lines = point_cloud.shape[0]
-        self.n_pixels = point_cloud.shape[1]
-        self.n_bands = point_cloud.shape[1]
-
-        # A clean way of doing things would be to define 
-    def transform_geocentric_to_projected(self, config_crs):
-
-
-        
-        self.epsg_proj = config_crs.epsg_proj
-        self.crs = 'EPSG:' + str(self.epsg_proj)
-        
-        
-
-        self.points_proj  = np.zeros(self.points_geocsc.shape) # Remains same if it is local
-        
-        geocsc = CRS.from_epsg(self.epsg_geocsc)
-        proj = CRS.from_epsg(self.epsg_proj)
-        transformer = Transformer.from_crs(geocsc, proj)
-
-        x_ecef = self.points_geocsc[:,:,0].reshape((-1, 1))
-        y_ecef = self.points_geocsc[:, :, 1].reshape((-1, 1))
-        z_ecef = self.points_geocsc[:, :, 2].reshape((-1, 1))
-
-        
-
-        (east, north, hei) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
-
-        self.points_proj[:,:,0] = east.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
-        self.points_proj[:, :, 1] = north.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
-        self.points_proj[:, :, 2] = hei.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
-
-
-        
-
-
-    def footprint_to_shape_file(self, footprint_dir):
-        """Uses the georeferenced data points (in projected form) to describe the footprint as a shape file
-
-        :param footprint_dir: Where to put the shape files describing the footprint
-        :type footprint_dir: string
-        """
-        self.edge_start = self.points_proj[0, :, 0:2].reshape((-1,2))
-        self.edge_end = self.points_proj[-1, :, 0:2].reshape((-1,2))
-        self.side_1 = self.points_proj[:, 0, 0:2].reshape((-1,2))
-        self.side_2 = self.points_proj[:, -1, 0:2].reshape((-1,2))
-
-
-        # Do it clockwise
-        self.hull_line = np.concatenate((
-            self.edge_start,
-            self.side_2,
-            np.flip(self.edge_end, axis=0),
-            np.flip(self.side_1, axis = 0)
-
-        ), axis = 0)
-
-        # The swiped ground area is defined by the convex hull
-        self.footprint_shp = Polygon(self.hull_line).convex_hull
-
-        gdf = gpd.GeoDataFrame(geometry=[self.footprint_shp], crs=self.crs)
-
-        shape_path = footprint_dir + self.name + '.shp'
-
-        gdf.to_file(shape_path, driver='ESRI Shapefile')
-
-    def resample_datacube(self, radiance_cube, wavelengths, fwhm, envi_cube_dir, rgb_composite_dir, config_ortho):
-        """Resamples the radiance cube into a geographic grid based on the georeferencing
-
-        :param radiance_cube: The data cube of radiance with the corresponding radiometric_unit of the data
-        :type radiance_cube: Often an ndarray(n, m, k) where n-number of lines, m- number of pixels, and k-number of spectral bands
-        :param wavelengths: The band's centre wavelengths
-        :type wavelengths: ndarray(k, 1)
-        :param fwhm: Full Width Half Maximum, descibing the band's widths (often in nanometers)
-        :type fwhm: ndarray(k, 1)
-        :param envi_cube_dir: Directory to write data cubes
-        :type envi_cube_dir: string, path
-        :param rgb_composite_dir: Directory to write data cubes
-        :type rgb_composite_dir: string, path
-        :param config_ortho: The relevant configurations for orthorectification
-        :type config_ortho: Dictionary
-        """
-
-
-
-        
-        n_bands = len(wavelengths)
-        #
-        n = radiance_cube.shape[0]
-        m = radiance_cube.shape[1]
-        k = radiance_cube.shape[2] # Number of bands
-
-        bytes_per_entry = radiance_cube.itemsize
-        chunk_size_GB = config_ortho.chunk_size_cube_GB
-
-
-        # If chunking is to be applied, we can use square chunks. Round to the nearest thousand because of personal OCD
-        chunk_square_length = np.sqrt((chunk_size_GB*1024**3) / (k*bytes_per_entry))
-        self.chunk_square_length = int(np.round(chunk_square_length/1000)*1000)
-
-        if self.chunk_square_length == 0:
-            self.chunk_square_length = 1000
-
-        self.chunk_area = self.chunk_square_length**2
-
-        self.res = config_ortho.ground_resolution
-
-        wl_red = config_ortho.wl_red
-        wl_green = config_ortho.wl_green
-        wl_blue = config_ortho.wl_blue
-
-        raster_transform_method = config_ortho.raster_transform_method
-
-        # Set nodata value for ortho-products
-        nodata = config_ortho.nodata_value
-        self.nodata = nodata
-
-        rgb_composite_only = config_ortho.resample_rgb_only
-
-        
-
-        # Set custom RGB bands from *.ini file
-        band_ind_R = np.argmin(np.abs(wl_red - wavelengths))
-        band_ind_G = np.argmin(np.abs(wl_green - wavelengths))
-        band_ind_B = np.argmin(np.abs(wl_blue - wavelengths))
-
-        # To let ENVI pick up on which bands are used for red-green-blue vizualization
-        self.default_bands_string = '{ '+' , '.join([str(band_ind_R), str(band_ind_G), str(band_ind_B)]) + ' }'
-
-        # Some relevant metadata
-        metadata_ENVI = {
-            'description': 'Radiance converted, georeferenced data',
-            'unit': config_ortho.radiometric_unit,
-            'wavelength units': config_ortho.wavelength_unit,
-            'sensor type': config_ortho.sensor_type,
-            'default bands': self.default_bands_string,
-            'interleave': config_ortho.interleave,
-            'wavelengths': wavelengths
-        }
-        try:
-            # If vector form
-            if fwhm.any() == np.nan:
-                pass
-            else:
-                metadata_ENVI['fwhm'] = fwhm
-        except AttributeError:
-            # If scalar
-            if fwhm == np.nan:
-                pass
-            else:
-                metadata_ENVI['fwhm'] = fwhm
-
-            
-        
-        
-        # Extract relevant info from hyp object
-        datacube = radiance_cube[:, :, :].reshape((-1, n_bands))
-
-        # RBG Composite
-        rgb_cube = datacube[:, [band_ind_R, band_ind_G, band_ind_B]].reshape((-1, 3))
-
-        # Horizontal coordinates of intersections in projected CRS
-        coords = self.points_proj[:, :, 0:2].reshape((-1, 2))
-
-        del radiance_cube
-        
-        # The raster can be rotated optimally (which saves loads of memory) for transects that are long compared to width. 
-        # However, north-east oriented rasters is more supported by image visualization
-        transform, height, width, indexes, suffix, mask_nn = GeoSpatialAbstractionHSI.cube_to_raster_grid(coords, raster_transform_method, resolution = self.res)
-
-        # Make accessible as attribute because it can be to write ancillary data
-        self.indexes = indexes.copy()
-        self.transform = transform
-        self.width = width
-        self.height = height
-        self.suffix = suffix
-
-        # Create raster mask from the polygon describing the footprint (currently not used for anything)
-        #geoms = [mapping(self.footprint_shp)]
-        #mask = geometry_mask(geoms, out_shape=(height, width), transform=transform)
-
-        mask = mask_nn.reshape((height, width))
-        self.mask = mask
-
-        # Build datacube
-        if not rgb_composite_only:
-
-            # For the later processing, storing the mapping from the rectified grid to the raw datacube makes sense:
-            indexes_grid_unmasked = indexes.reshape((height, width))
-            # Mask indexes
-            indexes_grid_unmasked[mask == 1] = nodata
-
-            # Make masked indices accessible as these allow orthorectification of ancilliary data
-            self.index_grid_masked = indexes_grid_unmasked
-
-            # To do the writing of the rasters we use a memory map, and writes chunks at a time.
-            # For this writing process, we need to know all the below
-            memmap_gen_params = {
-                'indexes': indexes,
-                'index_grid_masked': self.index_grid_masked,
-                'mask': mask,
-                'nodata': nodata,
-                'height': height,
-                'width': width,
-                'datacube': datacube,
-                'chunk_area': self.chunk_area
-            }
-
-            GeoSpatialAbstractionHSI.write_datacube_ENVI(memmap_gen_params, 
-                                nodata, 
-                                transform, 
-                                datacube_path = envi_cube_dir + self.name + suffix, 
-                                wavelengths=wavelengths,
-                                fwhm=fwhm,
-                                metadata = metadata_ENVI,
-                                crs=self.crs,
-                                interleave = config_ortho.interleave)
-
-            
-
-        # Resample RGB image data 
-        ortho_rgb = rgb_cube[self.indexes, :].flatten()
-
-        # Reshape image
-        ortho_rgb = ortho_rgb.reshape((height, width, 3))
-    
-        # Mask RGB
-        ortho_rgb[mask == 1, :] = nodata
-
-        # Arange datacube or composite in rasterio-friendly structure
-        ortho_rgb = np.transpose(ortho_rgb, axes = [2, 0, 1])
-        
-        # Write pseudo-RGB composite to composite folder ../GIS/RGBComposites
-        with rasterio.open(rgb_composite_dir + self.name + suffix + '.tif', 'w', driver='GTiff',
-                                height=height, width=width, count=3, dtype=ortho_rgb.dtype,
-                                crs=self.crs, transform=transform, nodata=nodata) as dst:
-
-            dst.write(ortho_rgb)
-        
-    @staticmethod
-    def write_datacube_memmap(memmap_array, indexes, index_grid_masked, mask, nodata, height, width, datacube, chunk_area):  
-        
-
-        # Step 1: Initialize a Memory Map
-        n_bands = datacube.shape[1]
-
-        # In grid form, identify whether partitioning is needed
-        area_idx_grid = width*height
-
-        if area_idx_grid > chunk_area:
-            
-            # Subdivide along horizontal axis:
-            delta_width = int(chunk_area/height)
-            # Number of slices
-            num_delta_widths = int(width/delta_width) + 1
-
-            for i in range(num_delta_widths):
-                
-                if i != num_delta_widths-1:
-                    sub_indices = index_grid_masked[:, i*delta_width:(i+1)*delta_width].reshape((-1,1))
-                    dw = delta_width
-                    
-                else:
-                    sub_indices = index_grid_masked[:, i*delta_width:width].reshape((-1,1))
-                    dw = np.arange(i*delta_width, width).size
-                
-                # Only extraxt valid data:
-                sub_ortho_cube = np.ones((sub_indices.shape[0]*sub_indices.shape[1], n_bands))*nodata
-                
-                # From the grid, the only valid pixels are
-                valid_pixels = (sub_indices != nodata).reshape(-1)
-                valid_pixels_raw = sub_indices[valid_pixels].reshape(-1)
-                valid_pixels_geo = np.arange(sub_indices.size)[valid_pixels]
-
-                sub_ortho_cube[valid_pixels_geo, :] = datacube[valid_pixels_raw, :]
-
-                sub_ortho_cube = sub_ortho_cube.reshape((height, dw, n_bands))
-
-                # Form to Rasterio friendly
-                #sub_ortho_cube = np.transpose(sub_ortho_cube, axes=[2, 0, 1])
-
-                memmap_array[:, i*delta_width:i*delta_width + dw, :] = sub_ortho_cube
-            # Free memory
-            del datacube
-            del sub_ortho_cube
-        else:
-            # Resample
-            ortho_datacube = datacube[indexes, :]
-
-            # Free memory
-            del datacube
-
-            # Reshape to datacube form
-            ortho_datacube = ortho_datacube.reshape((height, width, n_bands))
-
-            # Mask
-            ortho_datacube[mask == 1, :] = nodata
-
-            # Form to Rasterio friendly
-            #ortho_datacube = np.transpose(ortho_datacube, axes=[2, 0, 1])
-
-            # Write to memory map
-            memmap_array[:] = ortho_datacube
-
-            # Free memory
-            del ortho_datacube
-
-        return  
-
-    def resample_ancillary(self, h5_filename, anc_dir, anc_dict, interleave = 'bsq'):
-
-        band_counter = 0
-        band_names = []
-
-        # Define one hyperspectral data to 
-        with h5py.File(h5_filename, 'r', libver='latest') as f:
-            for attribute_name, h5_hierarchy_item_path in anc_dict.items():
-                if attribute_name != 'folder':
-                    data = f[h5_hierarchy_item_path][()]
-
-
-                    if data.ndim == 2:
-                        if data.shape[1]  != self.n_pixels:
-                            # For data of shape n_lines x j, for example camera positions, reshape to n_lines x n_pixels x j
-                            j = data.shape[1]
-                            data = np.einsum('ijk, ik -> ijk', np.ones((self.n_lines, self.n_pixels, j), dtype=np.float64), data)
-                        else:
-                            # For data with dimension n_lines x n_pixels, add third dimension
-                            data = data.reshape((data.shape[0], data.shape[1], 1))
-
-                    data = data.astype(dtype = np.float64)
-                    
-                    # For first layer
-                    if band_counter == 0:
-                        anc_data_array = data
-                    # For other layers, concatenate with existing layers
-                    else:
-                        anc_data_array = np.concatenate((anc_data_array, data), axis = 2)
-
-                    # Necessary to modify for data with multiple bands
-                    k = data.shape[2]
-                    # If data has more than one band:
-                    if k > 1:
-                        for i in range(k):
-                            band_name_data = attribute_name + '_' + str(i)
-                            band_names.append(band_name_data)
-                    else:
-                        band_name_data = attribute_name
-                        band_names.append(band_name_data)
-                    
-                    band_counter += k
-                    
-                    
-            
-        
-        
-        metadata_anc = {
-            'description': 'Ancillary data',
-            'band names': '{ '+' , '.join(band_names) + ' }'
-        }
-        n_bands = band_counter
-
-        # Resample
-        anc_data_array = anc_data_array.reshape((-1, n_bands))
-        ortho_anc = anc_data_array[self.indexes.flatten(), :]
-
-        # Free memory
-        del anc_data_array
-
-        # Reshape to anc_cube form
-        ortho_anc = ortho_anc.reshape((self.height, self.width, n_bands))
-
-        # Mask
-        ortho_anc[self.mask == 1, :] = self.nodata
-
-        # Form to Rasterio friendly
-        ortho_anc = np.transpose(ortho_anc, axes=[2, 0, 1])
-
-        if not os.path.isdir(anc_dir):
-            os.mkdir(anc_dir)
-
-        GeoSpatialAbstractionHSI.write_ancillary_ENVI(ortho_anc, 
-                                                      nodata = self.nodata, 
-                                                      transform = self.transform, 
-                                                      crs = self.crs,
-                                                      anc_path = anc_dir + self.name + self.suffix,
-                                                      metadata=metadata_anc,
-                                                      interleave=interleave)
-
-        
-
-    @staticmethod
-    def cube_to_raster_grid(coords, raster_transform_method, resolution):
-        """Function that takes projected coordinates (e.g. UTM 32 east and north) of ray intersections and computes an image grid
-
-        :param coords: _description_
-        :type coords: _type_
-        :param raster_transform_method: How the raster grid is calculated. "north_east" is standard and defines a rectangle along north/east. "minimal_rectangle" is memory optimal as it finds the smallest enclosing rectangle that wraps the points.
-        :type raster_transform_method: _type_
-        :param resolution: _description_
-        :type resolution: _type_
-        :return: _description_
-        :rtype: _type_
-        """
-
-
-        if raster_transform_method == 'north_east':
-            # Creates the minimal area (and thus memory) rectangle around points
-            polygon = MultiPoint(coords).envelope
-
-            # extract coordinates
-            x, y = polygon.exterior.xy
-
-            suffix = '_north_east'
-            
-
-            
-        elif raster_transform_method == 'minimal_rectangle':
-            
-            # Creates the minimal area (and thus memory) rectangle around points
-            polygon = MultiPoint(coords).minimum_rotated_rectangle
-
-            # extract coordinates
-            x, y = polygon.exterior.xy
-
-            
-
-            suffix = '_rotated'
-
-        # Indices increase against the clock
-        # ul means upper left corner of polygon, ll means lower left and so on
-        idx_ul = 3
-        idx_ur = 2
-        idx_ll = 4
-
-        x_ul = x[idx_ul]
-        y_ul = y[idx_ul]
-
-        x_ur = x[idx_ur]
-        y_ur = y[idx_ur]
-
-        x_ll = x[idx_ll]
-        y_ll = y[idx_ll]
-
-        # The vector from the upper-left corner aka origin to the upper-right equals lambda*e_basis_x
-        e_basis_x = np.array([x_ur-x_ul, y_ur-y_ul]).reshape((2,1))
-        w_transect = np.linalg.norm(e_basis_x)
-        e_basis_x /= w_transect
-
-        # The y basis vector is the vector to the other edge
-        e_basis_y = np.array([x_ll-x_ul, y_ll-y_ul]).reshape((2,1))
-        h_transect = np.linalg.norm(e_basis_y)
-        e_basis_y /= h_transect
-        e_basis_y *= -1 # Ensuring right handedness (image storage y direction is opposite)
-
-        R = np.hstack((e_basis_x, e_basis_y)) # 2D rotation matrix by definition
-        
-        # Define origin/translation vector as the upper left corner
-        o = np.array([x[idx_ul], y[idx_ul]]).reshape((2))
-
-        # Transformation matrix rigid body 2D
-        Trb = np.zeros((3,3))
-        Trb[0:2,0:2] = R
-        Trb[0:2,2] = o
-        Trb[2,2] = 1
-
-        # We operate with same resolution in X and Y. Note that for "minimal_rectangle" X, Y are NOT East and North. 
-        s_x = resolution
-        s_y = resolution
-
-        S = np.diag(np.array([s_x, s_y, 1]))
-
-        # Reflection matrix to account for opposite row/up direction
-        Ref = np.diag(np.array([1, -1, 1]))
-
-        # The affine transform is then expressed:
-        Taff = Trb.dot(S).dot(Ref)
-
-        # The metric width and length of the transect can give us the number of pixels
-        width = int(np.ceil(w_transect/s_x))
-        height = int(np.ceil(h_transect/s_y))
-
-        # Rasterio operates with a conventional affine geotransform
-        a, b, c, d, e, f = Taff[0,0], Taff[0,1], Taff[0,2], Taff[1,0], Taff[1,1], Taff[1,2]
-        transform = rasterio.Affine(a, b, c, d, e, f)
-
-        # Define local orthographic pixel grid. Pixel centers reside at half coordinates.
-        xi, yi = np.meshgrid(np.arange(width) + 0.5, 
-                                np.arange(height) + 0.5)
-        # To get homogeneous vector (not an actual z coordinate)
-        zi = np.ones(xi.shape)
-
-        # Form homogeneous vectors (allows translation by multiplication)
-        x_r = np.vstack((xi.flatten(), yi.flatten(), zi.flatten())).T
-
-        # Map orthographic pixels to projected system
-        x_p = np.matmul(Taff, x_r.T).T 
-
-        # Make a point vector of grid points to be used in nearest neighbor
-        xy = np.vstack((x_p[:,0].flatten(), x_p[:,1].flatten())).T
-        
-        # Define NN search tree from intersection points
-        tree = NearestNeighbors(radius=resolution).fit(coords)
-
-        # Calculate the nearest intersection point (in "coords") for each grid cell ("xy").
-        
-        # Here we only use one neighbor, and indexes is a vector of len(xy) where an element indexes(i)
-        # says that the closest point to xy[i] is coords[indexes[i]]. Since coords is just a flattened/reshaped version of intersection points
-        #, the data cube can be resampled by datacube_flat=datacube.reshape((dim1*dim2, dim3)) and 
-        # geographic_datacube_flat = datacube.reshape((dim1_geo*dim2_geo, dim3)) so that geographic_datacube_flat = datacube_flat[indexes,:]
-        n_neighbors = 1
-        dist, indexes = tree.kneighbors(xy, n_neighbors)
-
-        # We can mask the data by allowing points within a radius of 2x the resolution
-        mask_nn = dist > 2*resolution
-        
-        return transform, height, width, indexes, suffix, mask_nn
-
-    @staticmethod
-    def write_datacube_ENVI(memmap_gen_params, nodata, transform, datacube_path, wavelengths, fwhm, metadata, interleave, crs):
-        """_summary_
-
-        :param ortho_datacube: _description_
-        :type ortho_datacube: _type_
-        :param nodata: _description_
-        :type nodata: _type_
-        :param transform: _description_
-        :type transform: _type_
-        :param datacube_path: _description_
-        :type datacube_path: _type_
-        :param wavelengths: _description_
-        :type wavelengths: _type_
-        :param fwhm: _description_
-        :type fwhm: _type_
-        :param envi_hdr_dict: _description_
-        :type envi_hdr_dict: _type_
-        """
-
-        nx = memmap_gen_params['height']
-        mx = memmap_gen_params['width']
-        k = memmap_gen_params['datacube'].shape[1] # is collapsed datacube
-
-        dtype_cube = memmap_gen_params['datacube'].dtype # is collapsed datacube
-
-        crs_rasterio = CRS.from_string(crs)
-
-        writer_type = "envi" # Hardcoded
-
-        # Make some simple modifications
-        data_file_path = datacube_path + '.' + interleave
-        header_file_path = datacube_path + '.hdr'
-
-        if os.path.exists(header_file_path):
-            return
-
-        # Clean the files generated by rasterio
-        def write_band(args):
-            band_data, index, dst = args
-            dst.write(band_data, index + 1)
-
-        
-        def write_band_gdal(args):
-            band_data, index, dst = args
-            dst.GetRasterBand(index + 1).WriteArray(band_data)
-        
-        if os.path.exists(data_file_path):
-            os.remove(data_file_path)
-            os.remove(header_file_path)
-
-        if writer_type == "rasterio":
-            # Assuming ortho_datacube is a 3D NumPy array with shape (k, nx, mx)
-            with rasterio.open(data_file_path, 'w', driver='ENVI', height=nx, width=mx, count=k, crs=crs_rasterio, dtype=dtype_cube, transform=transform, nodata=nodata) as dst:
-                
-                # Create a ThreadPoolExecutor with as many threads as bands
-                with ThreadPoolExecutor(max_workers=k) as executor:
-                    # Use executor.map to parallelize the band writing process
-                    executor.map(write_band, [(band_data, i, dst) for i, band_data in enumerate(ortho_datacube)])
-                
-            
-            header.pop('band names')
-
-            
-        
-        elif writer_type == "envi":
-            # Create metadata for the output raster dataset
-            crs_gdal = osr.SpatialReference()
-            
-            crs_gdal.ImportFromEPSG(int(crs.split(':')[1]))
-
-            # Create dummy file to exploit builtin driver
-            with rasterio.open(data_file_path, 'w', driver='ENVI', height=1, width=1, count=1, crs=crs, dtype=dtype_cube, transform=transform, nodata=nodata) as dst:
-                pass
-            
-            os.remove(data_file_path)
-
-            header = sp.io.envi.read_envi_header(datacube_path + '.hdr') # Open for extraction
-            
-            # Since dummy image was made as 1x1x1 data cube
-            metadata_dim = {
-                'lines': nx,
-                'samples': mx,
-                'bands': k
-            }
-
-            # Write all meta data to header
-            for meta_key, value in metadata_dim.items():
-                header[meta_key] = value
-
-            # Reshape the ortho_datacube to (nx, mx, k)
-            #ortho_datacube_reshaped = ortho_datacube.transpose(1, 2, 0)
-
-            # Create the output raster dataset
-            # Create ENVI image without using a context manager
-            dst = envi.create_image(datacube_path + '.hdr', interleave='bsq', metadata=header, force=True)
-
-            mm = dst.open_memmap(writable=True)
-
-            GeoSpatialAbstractionHSI.write_datacube_memmap(memmap_array=mm, **memmap_gen_params)
-
-            
-
-
-
-        
-        
-        
-        header = sp.io.envi.read_envi_header(datacube_path + '.hdr') # Open for extraction
-        header.pop('band names')
-
-        # Nobody in the history of the world could have come up with a more annoying bug.
-        # Apparently, the CRS string is written with white spaces by rasterio/GDAL, wheras it should have none.
-        header['coordinate system string'] = '{' + ",".join(header['coordinate system string']) + '}'
-        
-        # Write all meta_data to header
-        for meta_key, value in metadata.items():
-            header[meta_key] = value
-
-        sp.io.envi.write_envi_header(fileName=header_file_path, header_dict=header)
-
-    @staticmethod
-    def write_ancillary_ENVI(anc_data, nodata, transform, anc_path, metadata, interleave, crs):
-        """_summary_
-
-        :param anc_data: An ancilliary data cube 
-        :type anc_data: j x m x n where j are the number of bands, and m, n are the raster dimensions 
-        :param nodata: _description_
-        :type nodata: _type_
-        :param transform: _description_
-        :type transform: _type_
-        :param datacube_path: _description_
-        :type datacube_path: _type_
-        :param metadata: _description_
-        :type metadata: _type_
-        :param interleave: _description_
-        :type interleave: _type_
-        :param crs: _description_
-        :type crs: _type_
-        """
-        nx = anc_data.shape[1]
-        mx = anc_data.shape[2]
-        k = anc_data.shape[0]
-
-        # Make some simple modifications
-        data_file_path = anc_path + '.' + interleave
-        header_file_path = anc_path + '.hdr'
-
-        if os.path.exists(data_file_path):
-            os.remove(data_file_path)
-            os.remove(header_file_path)
-
-        # Hack to exploit rasterio's generation of map info
-
-        # Clean the files generated by rasterio
-        def write_band(args):
-            band_data, index, dst = args
-            dst.write(band_data, index + 1)
-
-        # Assuming ortho_datacube is a 3D NumPy array with shape (k, nx, mx)
-        with rasterio.open(data_file_path, 'w', driver='ENVI', height=nx, width=mx, count=k, crs=crs, dtype=anc_data.dtype, transform=transform, nodata=nodata) as dst:
-            # Create a ThreadPoolExecutor with as many threads as bands
-            with ThreadPoolExecutor(max_workers=k) as executor:
-                # Use executor.map to parallelize the band writing process
-                executor.map(write_band, [(band_data, i, dst) for i, band_data in enumerate(anc_data)])
-            
-        
-        header = sp.io.envi.read_envi_header(anc_path + '.hdr') # Open for modif
-
-        header.pop('band names') # Remove defaults
-
-        for meta_key, value in metadata.items():
-            header[meta_key] = value
-
-        sp.io.envi.write_envi_header(fileName=header_file_path, header_dict=header)
-
-    @staticmethod
-    def compare_hsi_composite_with_rgb_mosaic(hsi_composite_path, ref_ortho_reshaped_path):
-        """Compares an HSI orthomosaic """
-        
-        
-
-        
-        # The RGB orthomosaic after reshaping (the reference)
-        raster_rgb = gdal.Open(ref_ortho_reshaped_path, gdal.GA_Update)
-        xoff1, a1, b1, yoff1, d1, e1 = raster_rgb.GetGeoTransform()  # This should be equal
-        raster_rgb_array = np.array(raster_rgb.ReadAsArray())
-        R = raster_rgb_array[0, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
-        G = raster_rgb_array[1, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
-        B = raster_rgb_array[2, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
-        # del raster_array1
-        ortho_rgb = np.concatenate((R, G, B), axis=2)
-        rgb_image = Imcol(ortho_rgb)
-
-        # The HSI composite raster (the match)
-        raster_hsi = gdal.Open(hsi_composite_path)
-        raster_hsi_array = np.array(raster_hsi.ReadAsArray())
-        xoff2, a2, b2, yoff2, d2, e2 = raster_hsi.GetGeoTransform()
-        transform_pixel_projected = raster_hsi.GetGeoTransform()
-        R = raster_hsi_array[0, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
-        G = raster_hsi_array[1, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
-        B = raster_hsi_array[2, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
-        ortho_hsi = np.concatenate((R, G, B), axis=2)
-
-        # Some form of image processing
-        max_val = np.percentile(ortho_hsi.reshape(-1), 99)
-        ortho_hsi /= max_val
-        ortho_hsi[ortho_hsi > 1] = 1
-        ortho_hsi = (ortho_hsi * 255).astype(np.uint8)
-        ortho_hsi[ortho_hsi == 0] = 255
-        hsi_image = Imcol(ortho_hsi)
-
-        # Adjust Clahe
-        hsi_image.clahe_adjustment()
-        rgb_image.clahe_adjustment()
-
-        hsi_image.to_luma(gamma=False, image_array = hsi_image.clahe_adjusted)
-        rgb_image.to_luma(gamma=False, image_array= rgb_image.clahe_adjusted)
-
-        uv_vec_hsi, uv_vec_rgb, diff_AE_pixels = GeoSpatialAbstractionHSI.compute_sift_difference(hsi_image.luma_array, rgb_image.luma_array)
-
-
-        image_resolution = a2
-        diff_AE_meters = diff_AE_pixels*image_resolution
-        return uv_vec_hsi, uv_vec_rgb, diff_AE_meters, transform_pixel_projected
-
-
-    @staticmethod
-    def resample_rgb_ortho_to_hsi_ortho(ref_ortho_path, hsi_composite_path, ref_ortho_reshaped_path):
-        """Reproject RGB orthophoto to match the shape and projection of HSI raster.
-
-        Parameters
-        ----------
-        infile : (string) path to input file to reproject
-        match : (string) path to raster with desired shape and projection
-        outfile : (string) path to output file tif
-        """
-
-        infile = ref_ortho_path
-        match = hsi_composite_path
-        outfile = ref_ortho_reshaped_path
-        # open input
-        with rasterio.open(infile) as src:
-            src_transform = src.transform
-
-            # open input to match
-            with rasterio.open(match) as match:
-                dst_crs = match.crs
-
-                # calculate the output transform matrix
-                dst_transform, dst_width, dst_height = calculate_default_transform(
-                    src.crs,  # input CRS
-                    dst_crs,  # output CRS
-                    match.width,  # input width
-                    match.height,  # input height
-                    *match.bounds,  # unpacks input outer boundaries (left, bottom, right, top)
-                )
-
-            # set properties for output
-            dst_kwargs = src.meta.copy()
-            dst_kwargs.update({"crs": dst_crs,
-                               "transform": dst_transform,
-                               "width": dst_width,
-                               "height": dst_height,
-                               "nodata": 0})
-            
-            # open output
-            with rasterio.open(outfile, "w", **dst_kwargs) as dst:
-                # iterate through bands and write using reproject function
-                for i in range(1, src.count + 1):
-                    reproject(
-                        source=rasterio.band(src, i),
-                        destination=rasterio.band(dst, i),
-                        src_transform=src.transform,
-                        src_crs=src.crs,
-                        dst_transform=dst_transform,
-                        dst_crs=dst_crs,
-                        resampling=Resampling.cubic)
-
-    def resample_dem_to_hsi_ortho(dem_path, hsi_composite_path, dem_reshaped):
-        """Reproject a file to match the shape and projection of existing raster.
-
-        Parameters
-        ----------
-        infile : (string) path to input file to reproject
-        match : (string) path to raster with desired shape and projection
-        outfile : (string) path to output file tif
-        """
-
-        infile = dem_path
-        match = hsi_composite_path
-        outfile = dem_reshaped
-        # open input
-        with rasterio.open(infile) as src:
-            src_transform = src.transform
-
-            # open input to match
-            with rasterio.open(match) as match:
-                dst_crs = match.crs
-
-                # calculate the output transform matrix
-                dst_transform, dst_width, dst_height = calculate_default_transform(
-                    src.crs,  # input CRS
-                    dst_crs,  # output CRS
-                    match.width,  # input width
-                    match.height,  # input height
-                    *match.bounds,  # unpacks input outer boundaries (left, bottom, right, top)
-                )
-
-            # set properties for output
-            dst_kwargs = src.meta.copy()
-            dst_kwargs.update({"crs": dst_crs,
-                               "transform": dst_transform,
-                               "width": dst_width,
-                               "height": dst_height,
-                               "nodata": 0})
-            #print("Coregistered to shape:", dst_height, dst_width, '\n Affine', dst_transform)
-            # open output
-            with rasterio.open(outfile, "w", **dst_kwargs) as dst:
-                # iterate through bands and write using reproject function
-                for i in range(1, src.count + 1):
-                    reproject(
-                        source=rasterio.band(src, i),
-                        destination=rasterio.band(dst, i),
-                        src_transform=src.transform,
-                        src_crs=src.crs,
-                        dst_transform=dst_transform,
-                        dst_crs=dst_crs,
-                        resampling=Resampling.cubic)
-
-    @staticmethod
-    def compute_sift_difference(gray1, gray2):
-        """Simply matches two grayscale images using SIFT"""
-
-        gray1 = (gray1 - np.min(gray1)) / (np.max(gray1) - np.min(gray1))
-        gray2 = (gray2 - np.min(gray2)) / (np.max(gray2) - np.min(gray2))
-
-        gray1 = (gray1 * 255).astype(np.uint8)
-        gray2 = (gray2 * 255).astype(np.uint8)
-
-
-        # Find the keypoints and descriptors with SIFT
-        sift = cv.SIFT_create()
-        kp2, des2 = sift.detectAndCompute(gray2, None)
-        
-        kp1, des1 = sift.detectAndCompute(gray1, None)
-        FLANN_INDEX_KDTREE = 1
-        index_params = dict(algorithm=FLANN_INDEX_KDTREE, trees=5)
-        search_params = dict(checks=50)
-        flann = cv.FlannBasedMatcher(index_params, search_params)
-        matches = flann.knnMatch(des1, des2, k=2)
-        # store all the good matches as per Lowe's ratio test. We changed 0.8 to 0.85 to get more matches
-        good = []
-        for m, n in matches:
-            if m.distance < 0.80 * n.distance:
-                good.append(m)
-
-        draw_params = dict(matchColor=(0, 255, 0),  # draw matches in green color
-                           flags=2)
-
-        diff_u = np.zeros(len(good))
-        diff_v = np.zeros(len(good))
-        uv_vec_hsi = np.zeros((len(good), 2))
-        uv_vec_rgb = np.zeros((len(good), 2))
-        for i in range(len(good)):
-            idx2 = good[i].trainIdx
-            idx1 = good[i].queryIdx
-            uv1 = kp1[idx1].pt  # Slit image
-            uv2 = kp2[idx2].pt  # Orthomosaic
-            uv_vec_hsi[i,:] = uv1
-            uv_vec_rgb[i,:] = uv2
-
-            ## Conversion to global coordinates
-            diff_u[i] = uv2[0] - uv1[0]
-            diff_v[i] = uv2[1] - uv1[1]
-
-        img3 = cv.drawMatches(gray1, kp1, gray2, kp2, good, None, **draw_params)
-        #plt.imshow(img3, 'gray')
-        #plt.show()
-##
-        # The absolute errors
-        diff_AE = np.sqrt(diff_u ** 2 + diff_v ** 2)
-        
-        return uv_vec_hsi, uv_vec_rgb, diff_AE
-
-
-
-    def map_pixels_back_to_datacube(self, w_datacube):
-        """The projected formats can be transformed back with four integer transforms and interpolated accordingly"""
-        """As a simple strategy we perform bilinear interpolation"""
-
-        indexes_grid = np.flip(self.indexes.reshape((self.height_rectified, self.width_rectified)), axis = 0)
-
-        v = self.feature_uv_hsi[:, 0]
-        u = self.feature_uv_hsi[:, 1]
-
-        v_rgb = self.feature_uv_rgb[:, 0]
-        u_rgb = self.feature_uv_rgb[:, 1]
-
-        # Should transform rgb coordinates directly to world coordinates
-        ## Conversion to global coordinates
-        x = self.feature_uv_rgb[:, 0]
-        y = self.feature_uv_rgb[:, 1]
-
-        xoff, a, b, yoff, d, e = self.transform_pixel_projected
-
-
-        xp = a * x + b * y + xoff + 0.5*a # The origin of the image coordinate system is located at 0.5,0.5
-        yp = d * x + e * y + yoff + 0.5*e
-        zp = np.zeros(yp.shape)
-        for i in range(xp.shape[0]):
-            temp = [x for x in self.raster_dem.sample([(xp[i], yp[i])])]
-            zp[i] = float(temp[0])
-
-        if self.is_global != True:
-            self.features_points = np.concatenate((xp.reshape((-1,1)), yp.reshape((-1,1)), zp.reshape((-1,1))), axis = 1)
-        else:
-            geocsc = CRS.from_epsg(self.epsg_geocsc)
-            proj = CRS.from_epsg(self.epsg_proj)
-            transformer = Transformer.from_crs(proj, geocsc)
-            self.features_points = np.zeros((xp.shape[0], 3))
-
-
-
-            (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=xp, yy=yp, zz=zp)
-
-            self.features_points[:, 0] = x_ecef
-            self.features_points[:, 1] = y_ecef
-            self.features_points[:, 2] = z_ecef
-
-
-
-
-        #
-
-        self.v_datacube_hsi = np.zeros((v.shape[0], 4))
-        self.u_datacube_hsi = np.zeros((v.shape[0], 4))
-
-        # See wikipedia
-        for i in range(4):
-            if i == 0:
-                u1 = np.floor(u).astype(np.int32)  # row
-                v1 = np.floor(v).astype(np.int32)  # col
-            elif i == 1:
-                u1 = np.floor(u).astype(np.int32)  # row
-                v1 = np.ceil(v).astype(np.int32)  # col
-            elif i == 2:
-                u1 = np.ceil(u).astype(np.int32)  # row
-                v1 = np.floor(v).astype(np.int32)  # col
-            else:
-                u1 = np.ceil(u).astype(np.int32)  # row
-                v1 = np.ceil(v).astype(np.int32)  # col
-
-            ind_datacube_hsi = indexes_grid[u1, v1] # 1D Indexer til rå datakube
-
-            self.v_datacube_hsi[:, i] = ind_datacube_hsi % w_datacube
-            self.u_datacube_hsi[:, i]  = (ind_datacube_hsi - self.v_datacube_hsi[:, i]) / w_datacube
-
-
-        self.x1_x_hsi = v - np.floor(v)
-        self.y1_y_hsi = u - np.floor(u)
-
-        #self.x1_x_rgb = v_rgb - np.floor(v_rgb)
-        #self.y1_y_rgb = u_rgb - np.floor(u_rgb)
-
-
-    def compute_reference_points_ecef(uv_vec_ref, transform_pixel_projected, dem_resampled_path, epsg_proj, epsg_geocsc=4978):
-    
-    
-        """Computes ECEF reference points from a features detected on the orthomosaic and the DEM"""
-        x = uv_vec_ref[:, 0]
-        y = uv_vec_ref[:, 1]
-
-        # Sample the terrain raster to get a projected position of data 
-        raster_dem = rasterio.open(dem_resampled_path)
-        xoff, a, b, yoff, d, e = transform_pixel_projected
-
-        # Convert the pixel coordinates into true coordinates (e.g. UTM N/E)
-        xp = a * x + b * y + xoff + 0.5*a 
-        yp = d * x + e * y + yoff + 0.5*e
-        zp = np.zeros(yp.shape)
-        for i in range(xp.shape[0]):
-            temp = [x for x in raster_dem.sample([(xp[i], yp[i])])]
-            zp[i] = float(temp[0])
-
-        # Transform points to true 3D via pyproj
-        geocsc = CRS.from_epsg(epsg_geocsc)
-        proj = CRS.from_epsg(epsg_proj)
-        transformer = Transformer.from_crs(proj, geocsc)
-        ref_points_ecef = np.zeros((xp.shape[0], 3))
-        (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=xp, yy=yp, zz=zp)
-
-        ref_points_ecef[:, 0] = x_ecef
-        ref_points_ecef[:, 1] = y_ecef
-        ref_points_ecef[:, 2] = z_ecef
-        
-        return ref_points_ecef
-
-    def compute_position_orientation_features(uv_vec_hsi, pixel_nr_image, unix_time_image, position_ecef, quaternion_ecef, time_pose, nodata):
-        """Returns the positions, orientations and pixel numbers corresponding to the features. 
-        Also computes a feature mask identifying features that are invalid"""
-        rows = uv_vec_hsi[:, 1]
-        cols = uv_vec_hsi[:, 0]
-
-        # Determine mask
-        x0 = np.floor(cols).astype(int)
-        x1 = x0 + 1
-        y0 = np.floor(rows).astype(int)
-        y1 = y0 + 1
-
-        # All 4 neighbors (as used by bilinear interpolation) should be valid data points
-        feature_mask = np.all([pixel_nr_image[y0, x0].reshape(-1) != nodata,
-               pixel_nr_image[y1, x0].reshape(-1) != nodata,
-               pixel_nr_image[y0, x1].reshape(-1) != nodata,
-               pixel_nr_image[y1, x1].reshape(-1) != nodata], axis=0)
-
-
-        pixel_nr_vec = GeoSpatialAbstractionHSI.bilinear_interpolate(pixel_nr_image, x = cols, y = rows)
-        time_vec = GeoSpatialAbstractionHSI.bilinear_interpolate(unix_time_image, x = cols, y = rows)
-
-        pixel_vec_valid = pixel_nr_vec[feature_mask]
-        time_vec_valid = time_vec[feature_mask]
-
-        
-        from scipy.interpolate import interp1d
-        from gref4hsi.utils import geometry_utils as geom
-        
-
-        rotation_ecef = RotLib.from_quat(quaternion_ecef)
-
-        # Interpolates positions linearly and quaterinons by Slerp
-        position_vec, quaternion_vec = geom.interpolate_poses(time_pose, 
-                                            position_ecef, 
-                                            rotation_ecef,  
-                                            timestamps_to=time_vec_valid)
-        
-        return pixel_vec_valid, time_vec_valid, position_vec, quaternion_vec, feature_mask
-        
-
-        
-
-    @staticmethod
-    def feature_matches_to_GCP(features_hsi, features_ref, pixel_nr_raster, time_raster):
-        """Function to establish 2D feature positions u, j in raw cube, as well as true reference positions X, Y, Z
-
-        :param features_hsi: _description_
-        :type features_hsi: _type_
-        :param features_ref: _description_
-        :type features_ref: _type_
-        :param pixel_nr_raster: _description_
-        :type pixel_nr_raster: _type_
-        :param time_raster: _description_
-        :type time_raster: _type_
-        """
-
-        return None
-
-
-    # COPIED from https://stackoverflow.com/questions/12729228/simple-efficient-bilinear-interpolation-of-images-in-numpy-and-python
-    @staticmethod
-    def bilinear_interpolate(im, x, y):
-        
-        x = np.asarray(x)
-        y = np.asarray(y)
-
-        x0 = np.floor(x).astype(int)
-        x1 = x0 + 1
-        y0 = np.floor(y).astype(int)
-        y1 = y0 + 1
-
-        x0 = np.clip(x0, 0, im.shape[1]-1);
-        x1 = np.clip(x1, 0, im.shape[1]-1);
-        y0 = np.clip(y0, 0, im.shape[0]-1);
-        y1 = np.clip(y1, 0, im.shape[0]-1);
-
-        Ia = im[ y0, x0 ]
-        Ib = im[ y1, x0 ]
-        Ic = im[ y0, x1 ]
-        Id = im[ y1, x1 ]
-
-        wa = (x1-x) * (y1-y)
-        wb = (x1-x) * (y-y0)
-        wc = (x-x0) * (y1-y)
-        wd = (x-x0) * (y-y0)
-
-        return wa*Ia + wb*Ib + wc*Ic + wd*Id
-
+# Python standard lib
+import os
+from concurrent.futures import ThreadPoolExecutor
+
+# Third party
+import cv2 as cv
+import geopandas as gpd
+import matplotlib.pyplot as plt
+import numpy as np
+from pyproj import CRS, Transformer
+import rasterio
+from rasterio.features import geometry_mask
+from rasterio.warp import calculate_default_transform, reproject, Resampling
+from osgeo import gdal, osr
+from shapely.geometry import Polygon, mapping, MultiPoint
+from sklearn.neighbors import NearestNeighbors
+from spectral import envi
+import spectral as sp
+import h5py
+from scipy.spatial.transform import Rotation as RotLib
+
+# Lib modules
+from gref4hsi.utils.colours import Image as Imcol
+
+# ENVI datatype conversion dictionary
+dtype_dict = {1:np.uint8,
+             2:np.int16,
+             3:np.int32,
+             4:np.float32,
+             5:np.float64,
+             12:np.uint16,
+             13:np.uint32,
+             14:np.int64,
+             15:np.uint64}
+
+class GeoSpatialAbstractionHSI():
+    def __init__(self, point_cloud, transect_string, config_crs):
+        self.name = transect_string
+        self.points_geocsc = point_cloud
+
+        self.epsg_geocsc = config_crs.epsg_geocsc
+        
+        self.n_lines = point_cloud.shape[0]
+        self.n_pixels = point_cloud.shape[1]
+        self.n_bands = point_cloud.shape[1]
+
+        # A clean way of doing things would be to define 
+    def transform_geocentric_to_projected(self, config_crs):
+
+
+        
+        self.epsg_proj = config_crs.epsg_proj
+        self.crs = 'EPSG:' + str(self.epsg_proj)
+        
+        
+
+        self.points_proj  = np.zeros(self.points_geocsc.shape) # Remains same if it is local
+        
+        geocsc = CRS.from_epsg(self.epsg_geocsc)
+        proj = CRS.from_epsg(self.epsg_proj)
+        transformer = Transformer.from_crs(geocsc, proj)
+
+        x_ecef = self.points_geocsc[:,:,0].reshape((-1, 1))
+        y_ecef = self.points_geocsc[:, :, 1].reshape((-1, 1))
+        z_ecef = self.points_geocsc[:, :, 2].reshape((-1, 1))
+
+        
+
+        (east, north, hei) = transformer.transform(xx=x_ecef, yy=y_ecef, zz=z_ecef)
+
+        self.points_proj[:,:,0] = east.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
+        self.points_proj[:, :, 1] = north.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
+        self.points_proj[:, :, 2] = hei.reshape((self.points_proj.shape[0], self.points_proj.shape[1]))
+
+
+        
+
+
+    def footprint_to_shape_file(self, footprint_dir):
+        """Uses the georeferenced data points (in projected form) to describe the footprint as a shape file
+
+        :param footprint_dir: Where to put the shape files describing the footprint
+        :type footprint_dir: string
+        """
+        self.edge_start = self.points_proj[0, :, 0:2].reshape((-1,2))
+        self.edge_end = self.points_proj[-1, :, 0:2].reshape((-1,2))
+        self.side_1 = self.points_proj[:, 0, 0:2].reshape((-1,2))
+        self.side_2 = self.points_proj[:, -1, 0:2].reshape((-1,2))
+
+
+        # Do it clockwise
+        self.hull_line = np.concatenate((
+            self.edge_start,
+            self.side_2,
+            np.flip(self.edge_end, axis=0),
+            np.flip(self.side_1, axis = 0)
+
+        ), axis = 0)
+
+        # The swiped ground area is defined by the convex hull
+        self.footprint_shp = Polygon(self.hull_line).convex_hull
+
+        gdf = gpd.GeoDataFrame(geometry=[self.footprint_shp], crs=self.crs)
+
+        shape_path = footprint_dir + self.name + '.shp'
+
+        gdf.to_file(shape_path, driver='ESRI Shapefile')
+
+    def resample_datacube(self, radiance_cube, wavelengths, fwhm, envi_cube_dir, rgb_composite_dir, config_ortho):
+        """Resamples the radiance cube into a geographic grid based on the georeferencing
+
+        :param radiance_cube: The data cube of radiance with the corresponding radiometric_unit of the data
+        :type radiance_cube: Often an ndarray(n, m, k) where n-number of lines, m- number of pixels, and k-number of spectral bands
+        :param wavelengths: The band's centre wavelengths
+        :type wavelengths: ndarray(k, 1)
+        :param fwhm: Full Width Half Maximum, descibing the band's widths (often in nanometers)
+        :type fwhm: ndarray(k, 1)
+        :param envi_cube_dir: Directory to write data cubes
+        :type envi_cube_dir: string, path
+        :param rgb_composite_dir: Directory to write data cubes
+        :type rgb_composite_dir: string, path
+        :param config_ortho: The relevant configurations for orthorectification
+        :type config_ortho: Dictionary
+        """
+
+
+
+        
+        n_bands = len(wavelengths)
+        #
+        n = radiance_cube.shape[0]
+        m = radiance_cube.shape[1]
+        k = radiance_cube.shape[2] # Number of bands
+
+        bytes_per_entry = radiance_cube.itemsize
+        chunk_size_GB = config_ortho.chunk_size_cube_GB
+
+
+        # If chunking is to be applied, we can use square chunks. Round to the nearest thousand because of personal OCD
+        chunk_square_length = np.sqrt((chunk_size_GB*1024**3) / (k*bytes_per_entry))
+        self.chunk_square_length = int(np.round(chunk_square_length/1000)*1000)
+
+        if self.chunk_square_length == 0:
+            self.chunk_square_length = 1000
+
+        self.chunk_area = self.chunk_square_length**2
+
+        self.res = config_ortho.ground_resolution
+
+        wl_red = config_ortho.wl_red
+        wl_green = config_ortho.wl_green
+        wl_blue = config_ortho.wl_blue
+
+        raster_transform_method = config_ortho.raster_transform_method
+
+        # Set nodata value for ortho-products
+        nodata = config_ortho.nodata_value
+        self.nodata = nodata
+
+        rgb_composite_only = config_ortho.resample_rgb_only
+
+        
+
+        # Set custom RGB bands from *.ini file
+        band_ind_R = np.argmin(np.abs(wl_red - wavelengths))
+        band_ind_G = np.argmin(np.abs(wl_green - wavelengths))
+        band_ind_B = np.argmin(np.abs(wl_blue - wavelengths))
+
+        # To let ENVI pick up on which bands are used for red-green-blue vizualization
+        self.default_bands_string = '{ '+' , '.join([str(band_ind_R), str(band_ind_G), str(band_ind_B)]) + ' }'
+
+        # Some relevant metadata
+        metadata_ENVI = {
+            'description': 'Radiance converted, georeferenced data',
+            'unit': config_ortho.radiometric_unit,
+            'wavelength units': config_ortho.wavelength_unit,
+            'sensor type': config_ortho.sensor_type,
+            'default bands': self.default_bands_string,
+            'interleave': config_ortho.interleave,
+            'wavelengths': wavelengths
+        }
+        try:
+            # If vector form
+            if fwhm.any() == np.nan:
+                pass
+            else:
+                metadata_ENVI['fwhm'] = fwhm
+        except AttributeError:
+            # If scalar
+            if fwhm == np.nan:
+                pass
+            else:
+                metadata_ENVI['fwhm'] = fwhm
+
+            
+        
+        
+        # Extract relevant info from hyp object
+        datacube = radiance_cube[:, :, :].reshape((-1, n_bands))
+
+        # RBG Composite
+        rgb_cube = datacube[:, [band_ind_R, band_ind_G, band_ind_B]].reshape((-1, 3))
+
+        # Horizontal coordinates of intersections in projected CRS
+        coords = self.points_proj[:, :, 0:2].reshape((-1, 2))
+
+        del radiance_cube
+        
+        # The raster can be rotated optimally (which saves loads of memory) for transects that are long compared to width. 
+        # However, north-east oriented rasters is more supported by image visualization
+        transform, height, width, indexes, suffix, mask_nn = GeoSpatialAbstractionHSI.cube_to_raster_grid(coords, raster_transform_method, resolution = self.res)
+
+        # Make accessible as attribute because it can be to write ancillary data
+        self.indexes = indexes.copy()
+        self.transform = transform
+        self.width = width
+        self.height = height
+        self.suffix = suffix
+
+        # Create raster mask from the polygon describing the footprint (currently not used for anything)
+        #geoms = [mapping(self.footprint_shp)]
+        #mask = geometry_mask(geoms, out_shape=(height, width), transform=transform)
+
+        mask = mask_nn.reshape((height, width))
+        self.mask = mask
+
+        # Build datacube
+        if not rgb_composite_only:
+
+            # For the later processing, storing the mapping from the rectified grid to the raw datacube makes sense:
+            indexes_grid_unmasked = indexes.reshape((height, width))
+            # Mask indexes
+            indexes_grid_unmasked[mask == 1] = nodata
+
+            # Make masked indices accessible as these allow orthorectification of ancilliary data
+            self.index_grid_masked = indexes_grid_unmasked
+
+            # To do the writing of the rasters we use a memory map, and writes chunks at a time.
+            # For this writing process, we need to know all the below
+            memmap_gen_params = {
+                'indexes': indexes,
+                'index_grid_masked': self.index_grid_masked,
+                'mask': mask,
+                'nodata': nodata,
+                'height': height,
+                'width': width,
+                'datacube': datacube,
+                'chunk_area': self.chunk_area
+            }
+
+            GeoSpatialAbstractionHSI.write_datacube_ENVI(memmap_gen_params, 
+                                nodata, 
+                                transform, 
+                                datacube_path = envi_cube_dir + self.name + suffix, 
+                                wavelengths=wavelengths,
+                                fwhm=fwhm,
+                                metadata = metadata_ENVI,
+                                crs=self.crs,
+                                interleave = config_ortho.interleave)
+
+            
+
+        # Resample RGB image data 
+        ortho_rgb = rgb_cube[self.indexes, :].flatten()
+
+        # Reshape image
+        ortho_rgb = ortho_rgb.reshape((height, width, 3))
+    
+        # Mask RGB
+        ortho_rgb[mask == 1, :] = nodata
+
+        # Arange datacube or composite in rasterio-friendly structure
+        ortho_rgb = np.transpose(ortho_rgb, axes = [2, 0, 1])
+        
+        # Write pseudo-RGB composite to composite folder ../GIS/RGBComposites
+        with rasterio.open(rgb_composite_dir + self.name + suffix + '.tif', 'w', driver='GTiff',
+                                height=height, width=width, count=3, dtype=ortho_rgb.dtype,
+                                crs=self.crs, transform=transform, nodata=nodata) as dst:
+
+            dst.write(ortho_rgb)
+        
+    @staticmethod
+    def write_datacube_memmap(memmap_array, indexes, index_grid_masked, mask, nodata, height, width, datacube, chunk_area):  
+        """Function for writing data cube arrays to memory maps, effectively avoiding memory issues.
+
+        :param memmap_array: _description_
+        :type memmap_array: _type_
+        :param indexes: _description_
+        :type indexes: _type_
+        :param index_grid_masked: _description_
+        :type index_grid_masked: _type_
+        :param mask: _description_
+        :type mask: _type_
+        :param nodata: _description_
+        :type nodata: _type_
+        :param height: _description_
+        :type height: _type_
+        :param width: _description_
+        :type width: _type_
+        :param datacube: _description_
+        :type datacube: _type_
+        :param chunk_area: _description_
+        :type chunk_area: _type_
+        """
+
+        # How the hell is this logical?
+        n_bands = datacube.shape[1]
+
+        # In grid form, identify whether partitioning is needed
+        area_idx_grid = width*height
+
+        if area_idx_grid > chunk_area:
+            
+            # Subdivide along horizontal axis:
+            delta_width = int(chunk_area/height)
+            # Number of slices
+            num_delta_widths = int(width/delta_width) + 1
+            # Iterate slices
+            for i in range(num_delta_widths):
+                # Last slice has different thickness
+                if i != num_delta_widths-1:
+                    sub_indices = index_grid_masked[:, i*delta_width:(i+1)*delta_width].reshape((-1,1))
+                    dw = delta_width
+                    
+                else:
+                    sub_indices = index_grid_masked[:, i*delta_width:width].reshape((-1,1))
+                    dw = np.arange(i*delta_width, width).size
+                
+                # Only extraxt valid data:
+                sub_ortho_cube = np.ones((sub_indices.shape[0]*sub_indices.shape[1], n_bands))*nodata
+                
+                # From the grid, the only valid pixels are
+                valid_pixels = (sub_indices != nodata).reshape(-1)
+                valid_pixels_raw = sub_indices[valid_pixels].reshape(-1)
+                valid_pixels_geo = np.arange(sub_indices.size)[valid_pixels]
+
+                sub_ortho_cube[valid_pixels_geo, :] = datacube[valid_pixels_raw, :]
+
+                sub_ortho_cube = sub_ortho_cube.reshape((height, dw, n_bands))
+
+                # Form to Rasterio friendly
+                #sub_ortho_cube = np.transpose(sub_ortho_cube, axes=[2, 0, 1])
+
+                memmap_array[:, i*delta_width:i*delta_width + dw, :] = sub_ortho_cube
+            # Free memory
+            del datacube
+            del sub_ortho_cube
+        else:
+            # Resample
+            ortho_datacube = datacube[indexes, :]
+
+            # Free memory
+            del datacube
+
+            # Reshape to datacube form
+            ortho_datacube = ortho_datacube.reshape((height, width, n_bands))
+
+            # Mask
+            ortho_datacube[mask == 1, :] = nodata
+
+            # Form to Rasterio friendly
+            #ortho_datacube = np.transpose(ortho_datacube, axes=[2, 0, 1])
+
+            # Write to memory map
+            memmap_array[:] = ortho_datacube
+
+            # Free memory
+            del ortho_datacube
+
+        return  
+
+    def resample_ancillary(self, h5_filename, anc_dir, anc_dict, interleave = 'bsq'):
+
+        band_counter = 0
+        band_names = []
+
+        # Define one hyperspectral data to 
+        with h5py.File(h5_filename, 'r', libver='latest') as f:
+            for attribute_name, h5_hierarchy_item_path in anc_dict.items():
+                if attribute_name != 'folder':
+                    data = f[h5_hierarchy_item_path][()]
+
+
+                    if data.ndim == 2:
+                        if data.shape[1]  != self.n_pixels:
+                            # For data of shape n_lines x j, for example camera positions, reshape to n_lines x n_pixels x j
+                            j = data.shape[1]
+                            data = np.einsum('ijk, ik -> ijk', np.ones((self.n_lines, self.n_pixels, j), dtype=np.float64), data)
+                        else:
+                            # For data with dimension n_lines x n_pixels, add third dimension
+                            data = data.reshape((data.shape[0], data.shape[1], 1))
+
+                    data = data.astype(dtype = np.float64)
+                    
+                    # For first layer
+                    if band_counter == 0:
+                        anc_data_array = data
+                    # For other layers, concatenate with existing layers
+                    else:
+                        anc_data_array = np.concatenate((anc_data_array, data), axis = 2)
+
+                    # Necessary to modify for data with multiple bands
+                    k = data.shape[2]
+                    # If data has more than one band:
+                    if k > 1:
+                        for i in range(k):
+                            band_name_data = attribute_name + '_' + str(i)
+                            band_names.append(band_name_data)
+                    else:
+                        band_name_data = attribute_name
+                        band_names.append(band_name_data)
+                    
+                    band_counter += k
+                    
+                    
+            
+        
+        
+        metadata_anc = {
+            'description': 'Ancillary data',
+            'band names': '{ '+' , '.join(band_names) + ' }'
+        }
+        n_bands = band_counter
+
+        # Resample
+        anc_data_array = anc_data_array.reshape((-1, n_bands))
+        
+        # Grid of indices
+        indexes_grid_unmasked = self.indexes.reshape((self.height, self.width))
+
+        # Mask indexes
+        indexes_grid_unmasked[self.mask == 1] = self.nodata
+
+        # Make masked indices accessible as these allow orthorectification of ancilliary data
+        self.index_grid_masked = indexes_grid_unmasked
+
+        # Alternative 2
+        memmap_gen_params = {
+            'indexes': self.indexes,
+            'index_grid_masked': self.index_grid_masked,
+            'mask': self.mask,
+            'nodata': self.nodata,
+            'height': self.height,
+            'width': self.width,
+            'datacube': anc_data_array,
+            'chunk_area': self.chunk_area
+        }
+        
+        GeoSpatialAbstractionHSI.write_ancillary_ENVI_envi(nodata = self.nodata, 
+                                                    transform = self.transform, 
+                                                    crs = self.crs,
+                                                    anc_path = anc_dir + self.name + self.suffix,
+                                                    metadata = metadata_anc,
+                                                    interleave=interleave,
+                                                    memmap_gen_params=memmap_gen_params)
+
+        
+
+    @staticmethod
+    def cube_to_raster_grid(coords, raster_transform_method, resolution):
+        """Function that takes projected coordinates (e.g. UTM 32 east and north) of ray intersections and computes an image grid
+
+        :param coords: _description_
+        :type coords: _type_
+        :param raster_transform_method: How the raster grid is calculated. "north_east" is standard and defines a rectangle along north/east. "minimal_rectangle" is memory optimal as it finds the smallest enclosing rectangle that wraps the points.
+        :type raster_transform_method: _type_
+        :param resolution: _description_
+        :type resolution: _type_
+        :return: _description_
+        :rtype: _type_
+        """
+
+
+        if raster_transform_method == 'north_east':
+            # Creates the minimal area (and thus memory) rectangle around points
+            polygon = MultiPoint(coords).envelope
+
+            # extract coordinates
+            x, y = polygon.exterior.xy
+
+            suffix = '_north_east'
+            
+
+            
+        elif raster_transform_method == 'minimal_rectangle':
+            
+            # Creates the minimal area (and thus memory) rectangle around points
+            polygon = MultiPoint(coords).minimum_rotated_rectangle
+
+            # extract coordinates
+            x, y = polygon.exterior.xy
+
+            
+
+            suffix = '_rotated'
+
+        # Indices increase against the clock
+        # ul means upper left corner of polygon, ll means lower left and so on
+        idx_ul = 3
+        idx_ur = 2
+        idx_ll = 4
+
+        x_ul = x[idx_ul]
+        y_ul = y[idx_ul]
+
+        x_ur = x[idx_ur]
+        y_ur = y[idx_ur]
+
+        x_ll = x[idx_ll]
+        y_ll = y[idx_ll]
+
+        # The vector from the upper-left corner aka origin to the upper-right equals lambda*e_basis_x
+        e_basis_x = np.array([x_ur-x_ul, y_ur-y_ul]).reshape((2,1))
+        w_transect = np.linalg.norm(e_basis_x)
+        e_basis_x /= w_transect
+
+        # The y basis vector is the vector to the other edge
+        e_basis_y = np.array([x_ll-x_ul, y_ll-y_ul]).reshape((2,1))
+        h_transect = np.linalg.norm(e_basis_y)
+        e_basis_y /= h_transect
+        e_basis_y *= -1 # Ensuring right handedness (image storage y direction is opposite)
+
+        R = np.hstack((e_basis_x, e_basis_y)) # 2D rotation matrix by definition
+        
+        # Define origin/translation vector as the upper left corner
+        o = np.array([x[idx_ul], y[idx_ul]]).reshape((2))
+
+        # Transformation matrix rigid body 2D
+        Trb = np.zeros((3,3))
+        Trb[0:2,0:2] = R
+        Trb[0:2,2] = o
+        Trb[2,2] = 1
+
+        # We operate with same resolution in X and Y. Note that for "minimal_rectangle" X, Y are NOT East and North. 
+        s_x = resolution
+        s_y = resolution
+
+        S = np.diag(np.array([s_x, s_y, 1]))
+
+        # Reflection matrix to account for opposite row/up direction
+        Ref = np.diag(np.array([1, -1, 1]))
+
+        # The affine transform is then expressed:
+        Taff = Trb.dot(S).dot(Ref)
+
+        # The metric width and length of the transect can give us the number of pixels
+        width = int(np.ceil(w_transect/s_x))
+        height = int(np.ceil(h_transect/s_y))
+
+        # Rasterio operates with a conventional affine geotransform
+        a, b, c, d, e, f = Taff[0,0], Taff[0,1], Taff[0,2], Taff[1,0], Taff[1,1], Taff[1,2]
+        transform = rasterio.Affine(a, b, c, d, e, f)
+
+        # Define local orthographic pixel grid. Pixel centers reside at half coordinates.
+        xi, yi = np.meshgrid(np.arange(width) + 0.5, 
+                                np.arange(height) + 0.5)
+        # To get homogeneous vector (not an actual z coordinate)
+        zi = np.ones(xi.shape)
+
+        # Form homogeneous vectors (allows translation by multiplication)
+        x_r = np.vstack((xi.flatten(), yi.flatten(), zi.flatten())).T
+
+        # Map orthographic pixels to projected system
+        x_p = np.matmul(Taff, x_r.T).T 
+
+        # Make a point vector of grid points to be used in nearest neighbor
+        xy = np.vstack((x_p[:,0].flatten(), x_p[:,1].flatten())).T
+        
+        # Define NN search tree from intersection points
+        tree = NearestNeighbors(radius=resolution).fit(coords)
+
+        # Calculate the nearest intersection point (in "coords") for each grid cell ("xy").
+        
+        # Here we only use one neighbor, and indexes is a vector of len(xy) where an element indexes(i)
+        # says that the closest point to xy[i] is coords[indexes[i]]. Since coords is just a flattened/reshaped version of intersection points
+        #, the data cube can be resampled by datacube_flat=datacube.reshape((dim1*dim2, dim3)) and 
+        # geographic_datacube_flat = datacube.reshape((dim1_geo*dim2_geo, dim3)) so that geographic_datacube_flat = datacube_flat[indexes,:]
+        n_neighbors = 1
+        dist, indexes = tree.kneighbors(xy, n_neighbors)
+
+        # We can mask the data by allowing points within a radius of 2x the resolution
+        mask_nn = dist > 2*resolution
+        
+        return transform, height, width, indexes, suffix, mask_nn
+
+    @staticmethod
+    def write_datacube_ENVI(memmap_gen_params, nodata, transform, datacube_path, wavelengths, fwhm, metadata, interleave, crs):
+        """_summary_
+
+        :param ortho_datacube: _description_
+        :type ortho_datacube: _type_
+        :param nodata: _description_
+        :type nodata: _type_
+        :param transform: _description_
+        :type transform: _type_
+        :param datacube_path: _description_
+        :type datacube_path: _type_
+        :param wavelengths: _description_
+        :type wavelengths: _type_
+        :param fwhm: _description_
+        :type fwhm: _type_
+        :param envi_hdr_dict: _description_
+        :type envi_hdr_dict: _type_
+        """
+
+        nx = memmap_gen_params['height']
+        mx = memmap_gen_params['width']
+        k = memmap_gen_params['datacube'].shape[1] # is collapsed datacube
+
+        dtype_cube = memmap_gen_params['datacube'].dtype # is collapsed datacube
+
+        # Make some simple modifications
+        data_file_path = datacube_path + '.' + interleave
+        header_file_path = datacube_path + '.hdr'
+        
+
+        if os.path.exists(data_file_path):
+            os.remove(data_file_path)
+            os.remove(header_file_path)
+
+        
+        # Create metadata for the output raster dataset
+        crs_gdal = osr.SpatialReference()
+        
+        crs_gdal.ImportFromEPSG(int(crs.split(':')[1]))
+
+        # Create 1x1x1 dummy file to exploit builtin driver
+        with rasterio.open(data_file_path, 'w', driver='ENVI', height=1, width=1, count=1, crs=crs, dtype=dtype_cube, transform=transform, nodata=nodata) as dst:
+            pass
+
+        # Then remove 
+        os.remove(data_file_path)
+
+        header = sp.io.envi.read_envi_header(datacube_path + '.hdr') # Open for extraction
+        
+        # Since dummy image was made as 1x1x1 data cube
+        metadata_dim = {
+            'lines': nx,
+            'samples': mx,
+            'bands': k
+        }
+
+        # Write all meta data to header
+        for meta_key, value in metadata_dim.items():
+            header[meta_key] = value
+
+        # Reshape the ortho_datacube to (nx, mx, k)
+        #ortho_datacube_reshaped = ortho_datacube.transpose(1, 2, 0)
+
+        # Create the output raster dataset
+        # Create ENVI image without using a context manager
+        dst = envi.create_image(datacube_path + '.hdr', interleave='bsq', metadata=header, force=True)
+
+        mm = dst.open_memmap(writable=True)
+
+        GeoSpatialAbstractionHSI.write_datacube_memmap(memmap_array=mm, **memmap_gen_params)
+        
+        header = sp.io.envi.read_envi_header(datacube_path + '.hdr') # Open for extraction
+        header.pop('band names')
+
+        # Nobody in the history of the world could have come up with a more annoying bug.
+        # Apparently, the CRS string is written with white spaces by rasterio/GDAL, wheras it should have none.
+        header['coordinate system string'] = '{' + ",".join(header['coordinate system string']) + '}'
+        
+        # Write all meta_data to header
+        for meta_key, value in metadata.items():
+            header[meta_key] = value
+
+        sp.io.envi.write_envi_header(fileName=header_file_path, header_dict=header)
+
+    @staticmethod
+    def write_ancillary_ENVI(anc_data, nodata, transform, anc_path, metadata, interleave, crs):
+        """_summary_
+
+        :param anc_data: An ancilliary data cube 
+        :type anc_data: j x m x n where j are the number of bands, and m, n are the raster dimensions 
+        :param nodata: _description_
+        :type nodata: _type_
+        :param transform: _description_
+        :type transform: _type_
+        :param datacube_path: _description_
+        :type datacube_path: _type_
+        :param metadata: _description_
+        :type metadata: _type_
+        :param interleave: _description_
+        :type interleave: _type_
+        :param crs: _description_
+        :type crs: _type_
+        """
+        nx = anc_data.shape[1]
+        mx = anc_data.shape[2]
+        k = anc_data.shape[0]
+
+        # Make some simple modifications
+        data_file_path = anc_path + '.' + interleave
+        header_file_path = anc_path + '.hdr'
+
+        if os.path.exists(data_file_path):
+            os.remove(data_file_path)
+            os.remove(header_file_path)
+
+        # Hack to exploit rasterio's generation of map info
+
+        # Clean the files generated by rasterio
+        def write_band(args):
+            band_data, index, dst = args
+            dst.write(band_data, index + 1)
+
+        # Assuming ortho_datacube is a 3D NumPy array with shape (k, nx, mx)
+        with rasterio.open(data_file_path, 'w', driver='ENVI', height=nx, width=mx, count=k, crs=crs, dtype=anc_data.dtype, transform=transform, nodata=nodata) as dst:
+            # Create a ThreadPoolExecutor with as many threads as bands
+            with ThreadPoolExecutor(max_workers=k) as executor:
+                # Use executor.map to parallelize the band writing process
+                executor.map(write_band, [(band_data, i, dst) for i, band_data in enumerate(anc_data)])
+            
+        
+        header = sp.io.envi.read_envi_header(anc_path + '.hdr') # Open for modif
+
+        header.pop('band names') # Remove defaults
+
+        for meta_key, value in metadata.items():
+            header[meta_key] = value
+
+        sp.io.envi.write_envi_header(fileName=header_file_path, header_dict=header)
+
+    @staticmethod
+    def write_ancillary_ENVI_envi(nodata, transform, anc_path, metadata, interleave, crs, memmap_gen_params):
+        """_summary_
+
+        :param anc_data: An ancilliary data cube 
+        :type anc_data: j x m x n where j are the number of bands, and m, n are the raster dimensions 
+        :param nodata: _description_
+        :type nodata: _type_
+        :param transform: _description_
+        :type transform: _type_
+        :param datacube_path: _description_
+        :type datacube_path: _type_
+        :param metadata: _description_
+        :type metadata: _type_
+        :param interleave: _description_
+        :type interleave: _type_
+        :param crs: _description_
+        :type crs: _type_
+        """
+        nx = memmap_gen_params['height']
+        mx = memmap_gen_params['width']
+        k = memmap_gen_params['datacube'].shape[1] # is collapsed datacube
+
+        dtype_cube = memmap_gen_params['datacube'].dtype # is collapsed datacube
+        # Make some simple modifications
+        data_file_path = anc_path + '.' + interleave
+        header_file_path = anc_path + '.hdr'
+
+        #if os.path.exists(header_file_path):
+        #    return
+        
+
+        if os.path.exists(data_file_path):
+            os.remove(data_file_path)
+            os.remove(header_file_path)
+
+
+        # Create metadata for the output raster dataset
+        crs_gdal = osr.SpatialReference()
+        
+        crs_gdal.ImportFromEPSG(int(crs.split(':')[1]))
+
+        # Create 1x1x1 dummy file to exploit builtin driver
+        with rasterio.open(data_file_path, 'w', driver='ENVI', height=1, width=1, count=1, crs=crs, dtype=dtype_cube, transform=transform, nodata=nodata) as dst:
+            pass
+
+        # Then remove 
+        os.remove(data_file_path)
+
+        # Open for extraction
+        header = sp.io.envi.read_envi_header(anc_path + '.hdr')
+
+        # Since dummy image was made as 1x1x1 data cube
+        metadata_dim = {
+            'lines': nx,
+            'samples': mx,
+            'bands': k
+        }
+
+        # Write all dimensions to header
+        for meta_key, value in metadata_dim.items():
+            header[meta_key] = value
+        
+        # Create ENVI image without using a context manager
+        dst = envi.create_image(anc_path + '.hdr', interleave='bsq', metadata=header, force=True)
+
+        mm = dst.open_memmap(writable=True)
+
+        # Write to the memory map
+        GeoSpatialAbstractionHSI.write_datacube_memmap(memmap_array=mm, **memmap_gen_params)
+        
+        header = sp.io.envi.read_envi_header(anc_path + '.hdr') # Open for extraction
+        header.pop('band names')
+
+        # Nobody in the history of the world could have come up with a more annoying bug.
+        # Apparently, the CRS string is written with white spaces by rasterio/GDAL, wheras it should have none.
+        header['coordinate system string'] = '{' + ",".join(header['coordinate system string']) + '}'
+        
+        # Write all meta_data to header
+        for meta_key, value in metadata.items():
+            header[meta_key] = value
+
+        sp.io.envi.write_envi_header(fileName=header_file_path, header_dict=header)
+
+
+
+    @staticmethod
+    def compare_hsi_composite_with_rgb_mosaic(hsi_composite_path, ref_ortho_reshaped_path):
+        """Compares an HSI orthomosaic """
+        
+        
+
+        
+        # The RGB orthomosaic after reshaping (the reference)
+        raster_rgb = gdal.Open(ref_ortho_reshaped_path, gdal.GA_Update)
+        xoff1, a1, b1, yoff1, d1, e1 = raster_rgb.GetGeoTransform()  # This should be equal
+        raster_rgb_array = np.array(raster_rgb.ReadAsArray())
+        R = raster_rgb_array[0, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
+        G = raster_rgb_array[1, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
+        B = raster_rgb_array[2, :, :].reshape((raster_rgb_array.shape[1], raster_rgb_array.shape[2], 1))
+        # del raster_array1
+        ortho_rgb = np.concatenate((R, G, B), axis=2)
+        rgb_image = Imcol(ortho_rgb)
+
+        # The HSI composite raster (the match)
+        raster_hsi = gdal.Open(hsi_composite_path)
+        raster_hsi_array = np.array(raster_hsi.ReadAsArray())
+        xoff2, a2, b2, yoff2, d2, e2 = raster_hsi.GetGeoTransform()
+        transform_pixel_projected = raster_hsi.GetGeoTransform()
+        R = raster_hsi_array[0, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
+        G = raster_hsi_array[1, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
+        B = raster_hsi_array[2, :, :].reshape((raster_hsi_array.shape[1], raster_hsi_array.shape[2], 1))
+        ortho_hsi = np.concatenate((R, G, B), axis=2)
+
+        # Some form of image processing
+
+        no_data_value = raster_hsi.GetRasterBand(1).GetNoDataValue()
+
+        ortho_valid = ortho_hsi[ortho_hsi[:,:,0] != no_data_value]
+
+        # Iterate the colors
+        for i in range(3):
+            # Enhancing colors somewhat
+            max_val = np.percentile(ortho_valid[:,i].reshape(-1), 95)
+            min_val = 0
+            
+            mono_im = ortho_hsi[:,:,i]
+            ortho_hsi[:,:,i] = (mono_im-min_val)/(max_val - min_val)
+
+            # Remove out-of-bounds
+            ortho_hsi[mono_im > 1, i] = 1
+            ortho_hsi[mono_im < 0, i] = 0
+        
+        
+        
+        ortho_hsi = ortho_hsi * 255
+        ortho_hsi[ortho_hsi == 0] = 255
+        hsi_image = Imcol(ortho_hsi)
+
+        # Adjust Clahe
+        #hsi_image.clahe_adjustment()
+        rgb_image.clahe_adjustment()
+
+        # Radiance is equivalent to a linear "color space". We run it through an inverse gamma to match the RGB data
+        hsi_image.to_luma(gamma=False, 
+                          image_array = hsi_image.image_array, 
+                          gamma_inverse=True, 
+                          gamma_value=0.45)
+        
+        hsi_image.clahe_adjustment(is_luma = True)
+
+        rgb_image.to_luma(gamma=False, image_array= rgb_image.clahe_adjusted)
+
+        uv_vec_hsi, uv_vec_rgb, diff_AE_pixels = GeoSpatialAbstractionHSI.compute_sift_difference(hsi_image.luma_array, rgb_image.luma_array)
+
+
+        image_resolution = a2
+        diff_AE_meters = diff_AE_pixels*image_resolution
+        return uv_vec_hsi, uv_vec_rgb, diff_AE_meters, transform_pixel_projected
+
+
+    @staticmethod
+    def resample_rgb_ortho_to_hsi_ortho(ref_ortho_path, hsi_composite_path, ref_ortho_reshaped_path):
+        """Reproject RGB orthophoto to match the shape and projection of HSI raster.
+
+        Parameters
+        ----------
+        infile : (string) path to input file to reproject
+        match : (string) path to raster with desired shape and projection
+        outfile : (string) path to output file tif
+        """
+
+        infile = ref_ortho_path
+        match = hsi_composite_path
+        outfile = ref_ortho_reshaped_path
+        # open input
+        with rasterio.open(infile) as src:
+            src_transform = src.transform
+
+            # open input to match
+            with rasterio.open(match) as match:
+                dst_crs = match.crs
+
+                # calculate the output transform matrix
+                dst_transform, dst_width, dst_height = calculate_default_transform(
+                    src.crs,  # input CRS
+                    dst_crs,  # output CRS
+                    match.width,  # input width
+                    match.height,  # input height
+                    *match.bounds,  # unpacks input outer boundaries (left, bottom, right, top)
+                )
+
+            # set properties for output
+            dst_kwargs = src.meta.copy()
+            dst_kwargs.update({"crs": dst_crs,
+                               "transform": dst_transform,
+                               "width": dst_width,
+                               "height": dst_height,
+                               "nodata": 0})
+            
+            # open output
+            with rasterio.open(outfile, "w", **dst_kwargs) as dst:
+                # iterate through bands and write using reproject function
+                for i in range(1, src.count + 1):
+                    reproject(
+                        source=rasterio.band(src, i),
+                        destination=rasterio.band(dst, i),
+                        src_transform=src.transform,
+                        src_crs=src.crs,
+                        dst_transform=dst_transform,
+                        dst_crs=dst_crs,
+                        resampling=Resampling.cubic)
+
+    def resample_dem_to_hsi_ortho(dem_path, hsi_composite_path, dem_reshaped):
+        """Reproject a file to match the shape and projection of existing raster.
+
+        Parameters
+        ----------
+        infile : (string) path to input file to reproject
+        match : (string) path to raster with desired shape and projection
+        outfile : (string) path to output file tif
+        """
+
+        infile = dem_path
+        match = hsi_composite_path
+        outfile = dem_reshaped
+        # open input
+        with rasterio.open(infile) as src:
+            src_transform = src.transform
+
+            # open input to match
+            with rasterio.open(match) as match:
+                dst_crs = match.crs
+
+                # calculate the output transform matrix
+                dst_transform, dst_width, dst_height = calculate_default_transform(
+                    src.crs,  # input CRS
+                    dst_crs,  # output CRS
+                    match.width,  # input width
+                    match.height,  # input height
+                    *match.bounds,  # unpacks input outer boundaries (left, bottom, right, top)
+                )
+
+            # set properties for output
+            dst_kwargs = src.meta.copy()
+            dst_kwargs.update({"crs": dst_crs,
+                               "transform": dst_transform,
+                               "width": dst_width,
+                               "height": dst_height,
+                               "nodata": 0})
+            #print("Coregistered to shape:", dst_height, dst_width, '\n Affine', dst_transform)
+            # open output
+            with rasterio.open(outfile, "w", **dst_kwargs) as dst:
+                # iterate through bands and write using reproject function
+                for i in range(1, src.count + 1):
+                    reproject(
+                        source=rasterio.band(src, i),
+                        destination=rasterio.band(dst, i),
+                        src_transform=src.transform,
+                        src_crs=src.crs,
+                        dst_transform=dst_transform,
+                        dst_crs=dst_crs,
+                        resampling=Resampling.cubic)
+
+    @staticmethod
+    def compute_sift_difference(gray1, gray2):
+        """Simply matches two grayscale images using SIFT"""
+
+        gray1 = (gray1 - np.min(gray1)) / (np.max(gray1) - np.min(gray1))
+        gray2 = (gray2 - np.min(gray2)) / (np.max(gray2) - np.min(gray2))
+
+        gray1 = (gray1 * 255).astype(np.uint8)
+        gray2 = (gray2 * 255).astype(np.uint8)
+
+
+        # Find the keypoints and descriptors with SIFT
+        sift = cv.SIFT_create()
+        kp2, des2 = sift.detectAndCompute(gray2, None)
+        kp1, des1 = sift.detectAndCompute(gray1, None)
+
+
+        FLANN_INDEX_KDTREE = 1
+        index_params = dict(algorithm=FLANN_INDEX_KDTREE, trees=5)
+        search_params = dict(checks=50)
+        flann = cv.FlannBasedMatcher(index_params, search_params)
+        matches = flann.knnMatch(des1, des2, k=2)
+        
+        good = []
+        # https://docs.opencv.org/4.x/dc/dc3/tutorial_py_matcher.html
+        # store all the good matches as per Lowe's ratio test (0.7). 
+        # Cranking up gives more. We changed 0.8 to 0.85 to get more matches
+        for m, n in matches:
+            if m.distance < 0.75 * n.distance:
+                good.append(m)
+
+        draw_params = dict(matchColor=(0, 255, 0),  # draw matches in green color
+                           flags=2)
+
+        diff_u = np.zeros(len(good))
+        diff_v = np.zeros(len(good))
+        uv_vec_hsi = np.zeros((len(good), 2))
+        uv_vec_rgb = np.zeros((len(good), 2))
+        for i in range(len(good)):
+            idx2 = good[i].trainIdx
+            idx1 = good[i].queryIdx
+            uv1 = kp1[idx1].pt  # Slit image
+            uv2 = kp2[idx2].pt  # Orthomosaic
+            uv_vec_hsi[i,:] = uv1
+            uv_vec_rgb[i,:] = uv2
+
+            ## Conversion to global coordinates
+            diff_u[i] = uv2[0] - uv1[0]
+            diff_v[i] = uv2[1] - uv1[1]
+
+        img3 = cv.drawMatches(gray1, kp1, gray2, kp2, good, None, **draw_params)
+        """plt.imshow(img3, 'gray')
+        plt.show()"""
+        print(len(good))
+##
+        # The absolute errors
+        diff_AE = np.sqrt(diff_u ** 2 + diff_v ** 2)
+        
+        return uv_vec_hsi, uv_vec_rgb, diff_AE
+
+
+
+    def map_pixels_back_to_datacube(self, w_datacube):
+        """The projected formats can be transformed back with four integer transforms and interpolated accordingly"""
+        """As a simple strategy we perform bilinear interpolation"""
+
+        indexes_grid = np.flip(self.indexes.reshape((self.height_rectified, self.width_rectified)), axis = 0)
+
+        v = self.feature_uv_hsi[:, 0]
+        u = self.feature_uv_hsi[:, 1]
+
+        v_rgb = self.feature_uv_rgb[:, 0]
+        u_rgb = self.feature_uv_rgb[:, 1]
+
+        # Should transform rgb coordinates directly to world coordinates
+        ## Conversion to global coordinates
+        x = self.feature_uv_rgb[:, 0]
+        y = self.feature_uv_rgb[:, 1]
+
+        xoff, a, b, yoff, d, e = self.transform_pixel_projected
+
+
+        xp = a * x + b * y + xoff + 0.5*a # The origin of the image coordinate system is located at 0.5,0.5
+        yp = d * x + e * y + yoff + 0.5*e
+        zp = np.zeros(yp.shape)
+        for i in range(xp.shape[0]):
+            temp = [x for x in self.raster_dem.sample([(xp[i], yp[i])])]
+            zp[i] = float(temp[0])
+
+        if self.is_global != True:
+            self.features_points = np.concatenate((xp.reshape((-1,1)), yp.reshape((-1,1)), zp.reshape((-1,1))), axis = 1)
+        else:
+            geocsc = CRS.from_epsg(self.epsg_geocsc)
+            proj = CRS.from_epsg(self.epsg_proj)
+            transformer = Transformer.from_crs(proj, geocsc)
+            self.features_points = np.zeros((xp.shape[0], 3))
+
+
+
+            (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=xp, yy=yp, zz=zp)
+
+            self.features_points[:, 0] = x_ecef
+            self.features_points[:, 1] = y_ecef
+            self.features_points[:, 2] = z_ecef
+
+
+
+
+        #
+
+        self.v_datacube_hsi = np.zeros((v.shape[0], 4))
+        self.u_datacube_hsi = np.zeros((v.shape[0], 4))
+
+        # See wikipedia
+        for i in range(4):
+            if i == 0:
+                u1 = np.floor(u).astype(np.int32)  # row
+                v1 = np.floor(v).astype(np.int32)  # col
+            elif i == 1:
+                u1 = np.floor(u).astype(np.int32)  # row
+                v1 = np.ceil(v).astype(np.int32)  # col
+            elif i == 2:
+                u1 = np.ceil(u).astype(np.int32)  # row
+                v1 = np.floor(v).astype(np.int32)  # col
+            else:
+                u1 = np.ceil(u).astype(np.int32)  # row
+                v1 = np.ceil(v).astype(np.int32)  # col
+
+            ind_datacube_hsi = indexes_grid[u1, v1] # 1D Indexer til rå datakube
+
+            self.v_datacube_hsi[:, i] = ind_datacube_hsi % w_datacube
+            self.u_datacube_hsi[:, i]  = (ind_datacube_hsi - self.v_datacube_hsi[:, i]) / w_datacube
+
+
+        self.x1_x_hsi = v - np.floor(v)
+        self.y1_y_hsi = u - np.floor(u)
+
+        #self.x1_x_rgb = v_rgb - np.floor(v_rgb)
+        #self.y1_y_rgb = u_rgb - np.floor(u_rgb)
+
+
+    def compute_reference_points_ecef(uv_vec_ref, transform_pixel_projected, dem_resampled_path, epsg_proj, epsg_geocsc=4978):
+    
+    
+        """Computes ECEF reference points from a features detected on the orthomosaic and the DEM"""
+        x = uv_vec_ref[:, 0]
+        y = uv_vec_ref[:, 1]
+
+        # Sample the terrain raster to get a projected position of data 
+        raster_dem = rasterio.open(dem_resampled_path)
+        xoff, a, b, yoff, d, e = transform_pixel_projected
+
+        # Convert the pixel coordinates into true coordinates (e.g. UTM N/E)
+        xp = a * x + b * y + xoff + 0.5*a 
+        yp = d * x + e * y + yoff + 0.5*e
+        zp = np.zeros(yp.shape)
+        for i in range(xp.shape[0]):
+            temp = [x for x in raster_dem.sample([(xp[i], yp[i])])]
+            zp[i] = float(temp[0])
+
+        # Transform points to true 3D via pyproj
+        geocsc = CRS.from_epsg(epsg_geocsc)
+        proj = CRS.from_epsg(epsg_proj)
+        transformer = Transformer.from_crs(proj, geocsc)
+        ref_points_ecef = np.zeros((xp.shape[0], 3))
+        (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=xp, yy=yp, zz=zp)
+
+        ref_points_ecef[:, 0] = x_ecef
+        ref_points_ecef[:, 1] = y_ecef
+        ref_points_ecef[:, 2] = z_ecef
+        
+        return ref_points_ecef
+
+    def compute_position_orientation_features(uv_vec_hsi, pixel_nr_image, unix_time_image, position_ecef, quaternion_ecef, time_pose, nodata):
+        """Returns the positions, orientations and pixel numbers corresponding to the features. 
+        Also computes a feature mask identifying features that are invalid"""
+        rows = uv_vec_hsi[:, 1]
+        cols = uv_vec_hsi[:, 0]
+
+        # Determine mask
+        x0 = np.floor(cols).astype(int)
+        x1 = x0 + 1
+        y0 = np.floor(rows).astype(int)
+        y1 = y0 + 1
+
+        # All 4 neighbors (as used by bilinear interpolation) should be valid data points
+        feature_mask = np.all([pixel_nr_image[y0, x0].reshape(-1) != nodata,
+               pixel_nr_image[y1, x0].reshape(-1) != nodata,
+               pixel_nr_image[y0, x1].reshape(-1) != nodata,
+               pixel_nr_image[y1, x1].reshape(-1) != nodata], axis=0)
+
+
+        pixel_nr_vec = GeoSpatialAbstractionHSI.bilinear_interpolate(pixel_nr_image, x = cols, y = rows)
+        time_vec = GeoSpatialAbstractionHSI.bilinear_interpolate(unix_time_image, x = cols, y = rows)
+
+        pixel_vec_valid = pixel_nr_vec[feature_mask]
+        time_vec_valid = time_vec[feature_mask]
+
+        
+        from scipy.interpolate import interp1d
+        from gref4hsi.utils import geometry_utils as geom
+        
+
+        rotation_ecef = RotLib.from_quat(quaternion_ecef)
+
+        # Interpolates positions linearly and quaterinons by Slerp
+        position_vec, quaternion_vec = geom.interpolate_poses(time_pose, 
+                                            position_ecef, 
+                                            rotation_ecef,  
+                                            timestamps_to=time_vec_valid)
+        
+        return pixel_vec_valid, time_vec_valid, position_vec, quaternion_vec, feature_mask
+        
+
+        
+
+    @staticmethod
+    def feature_matches_to_GCP(features_hsi, features_ref, pixel_nr_raster, time_raster):
+        """Function to establish 2D feature positions u, j in raw cube, as well as true reference positions X, Y, Z
+
+        :param features_hsi: _description_
+        :type features_hsi: _type_
+        :param features_ref: _description_
+        :type features_ref: _type_
+        :param pixel_nr_raster: _description_
+        :type pixel_nr_raster: _type_
+        :param time_raster: _description_
+        :type time_raster: _type_
+        """
+
+        return None
+
+
+    # COPIED from https://stackoverflow.com/questions/12729228/simple-efficient-bilinear-interpolation-of-images-in-numpy-and-python
+    @staticmethod
+    def bilinear_interpolate(im, x, y):
+        
+        x = np.asarray(x)
+        y = np.asarray(y)
+
+        x0 = np.floor(x).astype(int)
+        x1 = x0 + 1
+        y0 = np.floor(y).astype(int)
+        y1 = y0 + 1
+
+        x0 = np.clip(x0, 0, im.shape[1]-1);
+        x1 = np.clip(x1, 0, im.shape[1]-1);
+        y0 = np.clip(y0, 0, im.shape[0]-1);
+        y1 = np.clip(y1, 0, im.shape[0]-1);
+
+        Ia = im[ y0, x0 ]
+        Ib = im[ y1, x0 ]
+        Ic = im[ y0, x1 ]
+        Id = im[ y1, x1 ]
+
+        wa = (x1-x) * (y1-y)
+        wb = (x1-x) * (y-y0)
+        wc = (x-x0) * (y1-y)
+        wd = (x-x0) * (y-y0)
+
+        return wa*Ia + wb*Ib + wc*Ic + wd*Id
+
```

### Comparing `gref4hsi-0.2.1/gref4hsi/utils/parsing_utils.py` & `gref4hsi-0.2.2/gref4hsi/utils/parsing_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,601 +1,600 @@
-# Python built-ins
-import sys
-import os
-import configparser
-from os import path
-
-# Third party libraries
-import numpy as np
-import pandas as pd
-from scipy.spatial.transform import Rotation as RotLib
-from scipy.spatial.transform import Rotation
-import h5py
-from scipy.spatial.transform import Rotation as RotLib
-import pandas as pd
-import pymap3d as pm
-from scipy.spatial.transform import Slerp
-from scipy.interpolate import interp1d
-from pyproj import CRS, Transformer
-
-# Local modules
-from gref4hsi.utils.geometry_utils import CameraGeometry, GeoPose
-from gref4hsi.utils.geometry_utils import rot_mat_ned_2_ecef, interpolate_poses
-from gref4hsi.utils.geometry_utils import dem_2_mesh, crop_geoid_to_pose
-
-
-class Hyperspectral:
-    """
-    Class for storing/accessing acquired hyperspectral data. One instance corresponds to a transect chunk (*.h5).
-    """
-    def __init__(self, filename, config, load_datacube = True):
-        """
-        Instantiate transect chunk object from chunk file name and config file.
-        :param filename: string
-        path to *.h5 file
-        :param config: config type
-        dictionary-like interface to configuration file
-        """
-        # Chunk filename
-        self.name = filename
-        # If errors arise due to improper dataset paths below, open the *.h5 file in hdfviewer and edit the path.
-        with h5py.File(filename, 'r', libver='latest') as self.f:
-            # TODO: Embed the paths from this special format into confic file
-            try:
-                dataCubePath = config['HDF.hyperspectral']['dataCube']
-            except:
-                pass
-            
-            try:
-                timestampHyperspectralPath = config['HDF.hyperspectral']['timestamp']
-                self.dataCubeTimeStamps = self.f[timestampHyperspectralPath][()]
-            except:
-                pass
-
-            try:
-                # The band center wavelengths
-                band2WavelengthPath = config['HDF.calibration']['band2Wavelength']
-                self.band2Wavelength = self.f[band2WavelengthPath][()]
-            except:
-                pass
-            
-            try:
-                # The band widths (if they exist)
-                fwhmPath = config['HDF.calibration']['fwhm']
-
-                self.fwhm = self.f[fwhmPath][()]
-            except:
-                pass
-
-            try:
-                # These should come together in the case that radiometric calibration should be done
-                radiometricFramePath = config['HDF.calibration']['radiometricFrame']
-                darkFramePath = config['HDF.calibration']['darkFrame']
-                exposureTimePath = config['HDF.hyperspectral']['exposureTime']
-                is_uhi = config['HDF']['is_uhi']
-
-                
-                if eval(is_uhi):
-                    self.t_exp = self.f[exposureTimePath][()][0] / 1000  # Recorded in milliseconds
-                else:
-                    self.t_exp = self.f[exposureTimePath][()] / 1000
-
-                self.darkFrame = self.f[darkFramePath][()]
-                self.radiometricFrame = self.f[radiometricFramePath][()]
-            except:
-                pass
-            
-            try:
-                RGBFramesPath = config['HDF.rgb']['rgbFrames']
-                timestampRGBPath = config['HDF.rgb']['timestamp']
-                try:
-                    # Extract RGB image data if available
-                    self.RGBTimeStamps = self.f[timestampRGBPath][()]
-                    self.RGBImgs = self.f[RGBFramesPath][()]
-                    self.n_imgs = self.RGBTimeStamps.shape[0]
-                except (UnboundLocalError, KeyError):
-                    pass
-            except:
-                pass
-            
-            
-
-            if load_datacube:
-                # To save memory, we made it an option to not load datacube
-                self.dataCube = self.f[dataCubePath][()]
-
-                self.n_scanlines = self.dataCube.shape[0]
-                self.n_pix = self.dataCube.shape[1]
-                self.n_bands = self.dataCube.shape[1]
-
-                # Calculate radiance cube if this is cube is not calibrated
-                self.digital_counts_2_radiance(config=config)
-
-            # Check if the dataset exists
-            processed_nav_folder = config['HDF.processed_nav']['folder']
-            
-            # Read the position da
-            if processed_nav_folder in self.f:
-                try:
-                    processed_nav_config = config['HDF.processed_nav']
-                    self.pos_ref = self.f[processed_nav_config['position_ecef']][()]
-                    self.quat_ref = self.f[processed_nav_config['quaternion_ecef']][()]
-                    self.pose_time = self.f[processed_nav_config['timestamp']][()]
-                except:
-                    pass
-            
-
-
-
-       
-
-            
-
-
-
-    def digital_counts_2_radiance(self, config):
-
-        # Only calibrate if data it is not already done
-        is_calibrated = eval(config['HDF.hyperspectral']['is_calibrated'])
-
-        if is_calibrated == is_calibrated:
-            self.dataCubeRadiance = self.dataCube.astype(np.float32)
-
-            # Add the radiance dataset
-            radiance_cube_path = config['HDF.hyperspectral']['dataCube']
-        else:
-            self.dataCubeRadiance = np.zeros(self.dataCube.shape, dtype = np.float32)
-            for i in range(self.dataCube.shape[0]):
-                self.dataCubeRadiance[i, :, :] = (self.dataCube[i, :, :] - self.darkFrame) / (
-                        self.radiometricFrame * self.t_exp)
-            
-            # Add the radiance dataset
-            radiance_cube_path = config['HDF.hyperspectral']['dataCube'] + '_radiance'
-            
-            # TODO: Write the radiance data to the h5 file
-            Hyperspectral.add_dataset(data = self.dataCubeRadiance, name=radiance_cube_path, h5_filename=self.name)
-        
-        config.set('HDF.hyperspectral', 'radiance_cube', radiance_cube_path)
-
-        # For memory efficiency
-        del self.dataCube
-
-        
-            
-            
-    
-    """def add_dataset(self, data, name):
-        
-        # The h5 file structure can be studied by unravelling the structure in Python or by using HDFview
-        with h5py.File(self.name, 'a', libver='latest') as self.f:
-            # Check if the dataset exists
-            if name in self.f:
-                del self.f[name]
-
-            dset = self.f.create_dataset(name=name, data = data)
-    """
-    
-    @staticmethod
-    def add_dataset(data, name, h5_filename):
-        """
-        Method to write a dataset to the h5 file
-        :param data: type any permitted (see h5py doc)
-        The data to be written
-        :param name: string
-        The path/name of the dataset
-        :param h5_filename: string
-        The path to the h5_file
-        :return: None
-        """
-        # The h5 file structure can be studied by unravelling the structure in Python or by using HDFview
-        with h5py.File(h5_filename, 'a', libver='latest') as f:
-            # Check if the dataset exists
-            if name in f:
-                del f[name]
-
-            dset = f.create_dataset(name=name, data = data)
-
-    """def get_dataset(self, dataset_name):
-        
-        Method to return a dataset by the name
-        :param dataset_name: string
-        The h5 dataset path
-        :return: dataset
-        Returns the queried dataset. Could be many datatypes, but mainly numpy arrays in our usage.
-        
-        # The h5 file structure can be studied by unravelling the structure in Python or by using HDFview
-        with h5py.File(self.name, 'a', libver='latest') as self.f:
-            dataset = self.f[dataset_name][()]
-        return dataset"""
-    @staticmethod
-    def get_dataset(h5_filename, dataset_name):
-        """equivalent to the method, except it does not need an instance of a Hyperspectral object
-
-        :param h5_filename: Path to h5/hdf file
-        :type h5_filename: string
-        :param dataset_name: h5 rooted path, e.g. processed/reflectance/remote_sensing_reflectance
-        :type dataset_name: string
-        :return: The dataset at the relevant location
-        :rtype: numpy array or other
-        """
-        # The h5 file structure can be studied by unravelling the structure in Python or by using HDFview
-        with h5py.File(h5_filename, 'a', libver='latest') as f:
-            dataset = f[dataset_name][()]
-        return dataset
-
-class DataLogger:
-    def __init__(self, filename, header):
-        self.filename = filename
-        # Generate file with header
-        with open(filename, 'w') as fh:
-            fh.write(header + '\n')
-
-    def append_data(self, data):
-        # Append data line to file
-        with open(self.filename, 'a') as fh:
-            # Generate data line to file
-            if data[0] != None:
-                line = ','.join([str(el) for el in data])
-
-                # Append line to file
-                fh.write(line + '\n')
-
-def ardupilot_extract_pose(config, iniPath):
-    
-    """
-        :param config: The processing configuration object (from */configuration.ini file)
-        :param iniPath: The path to */configuration.ini file
-        :return: 
-    """
-    
-    # Attitude retrieved from an ardupilot CSV
-    att_path = config['General']['ardupath'] + 'Att.csv'
-    df_att = pd.read_csv(att_path)
-
-    # Convert the DataFrame to a matrix (list of lists)
-    matrix_att = np.array(df_att.values.tolist())
-    
-    # Rotations in roll-pitch-yaw define the rotation of the vehicle's body frame (i.e. IMU)
-    Rotation = RotLib.from_euler("ZYX", np.flip(matrix_att[:,1:4], axis = 1), degrees=True)
-    time_rot = matrix_att[:,0]
-    
-    # Position retrieved from an ardupilot CSV
-    pos_path = config['General']['ardupath'] + 'pos.csv'
-    df_pos = pd.read_csv(pos_path)
-    matrix_pos = np.array(df_pos.values.tolist())
-
-    time_pos = matrix_pos[:, 0]
-    Position = matrix_pos[:, 1:4]
-
-    linearPositionInterpolator = interp1d(time_pos, np.transpose(Position), fill_value='extrapolate')
-    position_nav_interpolated = np.transpose(linearPositionInterpolator(time_rot))
-
-    pose_path = config['General']['ardupath'] + 'pose.csv'
-
-    config.set('General', 'pose_path', pose_path)
-
-    epsg_proj = 4326 # Standard
-    epsg_geocsc = config['General']['modelepsg']
-    # Transform the mesh points to ECEF.
-
-    geocsc = CRS.from_epsg(epsg_geocsc)
-    proj = CRS.from_epsg(epsg_proj)
-    transformer = Transformer.from_crs(proj, geocsc)
-
-    points_proj = position_nav_interpolated
-
-    lat = points_proj[:, 0].reshape((-1, 1))
-    lon = points_proj[:, 1].reshape((-1, 1))
-    hei = points_proj[:, 2].reshape((-1, 1))
-
-    (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=lat, yy=lon, zz=hei)
-
-    pos_geocsc = np.concatenate((x_ecef.reshape((-1,1)), y_ecef.reshape((-1,1)), z_ecef.reshape((-1,1))), axis = 1)
-
-    #dlogr = DataLogger(pose_path, 'CameraLabel, X, Y, Z, Roll, Pitch, Yaw, RotX, RotY, RotZ')
-
-
-
-    data_matrix = np.zeros((len(time_rot), 10))
-    for i in range(len(time_rot)):
-
-        # Ardupilot delivers geodetic positions (EPSG::
-        pos_geod = position_nav_interpolated[i, :]
-
-        # Define rotation matrix between local tangential plane (NED, North-East-Down) and Earth-Centered-Earth-Fixed (ECEF).
-        R_n_e = rot_mat_ned_2_ecef(lat=pos_geod[0], lon=pos_geod[1])
-
-        Rotation_n = RotLib.from_matrix(R_n_e)
-
-        Rotation_e = Rotation_n*Rotation[i] # Composing rotations
-
-        roll = matrix_att[i, 1]
-        pitch = matrix_att[i, 2]
-        yaw = matrix_att[i, 3]
-
-        
-
-        rotz, roty, rotx = Rotation_e.as_euler("ZYX", degrees=True)
-
-        pos = pos_geocsc[i,:]
-
-        data_matrix[i,:] = np.array([time_rot[i], pos[0], pos[1], pos[2], roll, pitch, yaw, rotx, roty, rotz])
-
-        #dlogr.append_data([time_rot[i], pos[0], pos[1], pos[2], roll, pitch, yaw, rotx, roty, rotz])
-
-
-
-    headers = ['Timestamp', ' X', ' Y', ' Z', ' Roll', ' Pitch', ' Yaw', ' RotX', ' RotY', ' RotZ']
-
-    # Create a DataFrame from the data_matrix and headers
-    df = pd.DataFrame(data_matrix, columns=headers)
-
-    # Save the DataFrame as a CSV file
-    df.to_csv(pose_path, index=False)
-
-    with open(iniPath, 'w') as configfile:
-        config.write(configfile)
-        
-    return config
-
-
-def reformat_h5_embedded_data_h5(config, config_file):
-    """
-                Parses pose from h5, interpolates and reformats. Writes the positions and orientations of hyperspectral frames to
-                    dataset under the /Nav folder
-
-                Args:
-                    config_file: The *.ini file containing the paths and configurations.
-
-                Returns:
-                    None: The function returns nothing.
-    """
-
-
-    # Traverse through h5 dir to append the data to file
-    h5_folder = config['Absolute Paths']['h5_folder']
-    is_first = True
-    for filename in sorted(os.listdir(h5_folder)):
-        
-        # Find the interesting prefixes
-        if filename.endswith('h5') or filename.endswith('hdf'):
-            # Identify the total path
-            path_hdf = h5_folder + filename
-
-            # Read out the data of a file
-            hyp = Hyperspectral(path_hdf, config, load_datacube = False)
-
-
-            # If rotation reference is quaternion:
-            # Alternatives quat, eul_ZYX
-            rotation_reference_type = config['HDF.raw_nav']['rotation_reference_type']
-            if rotation_reference_type == 'quat':
-                quaternion_ref = hyp.get_dataset(h5_filename=path_hdf, dataset_name=config['HDF.raw_nav']['quaternion'])
-                if quaternion_ref.shape[0] == 4:
-                    quaternion_ref = np.transpose(quaternion_ref)
-                
-            
-                quaternion_convention  = config['HDF.raw_nav']['quaternion_convention']
-
-                # If scalar-first convention
-                if quaternion_convention == 'wxyz':
-                    quat_temp = quaternion_ref
-                    quaternion_ref = np.roll(quaternion_ref, shift=-1, axis=1)
-                elif quaternion_convention == 'xyzw':
-                    # We use the xyzw convention for scipy, see:
-                    # https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.transform.Rotation.from_quat.html
-                    pass
-                else:
-                    raise ValueError("The quaternion convention must be defined")
-            elif rotation_reference_type == 'eul_ZYX':
-                eul_ref = hyp.get_dataset(h5_filename=path_hdf,dataset_name=config['HDF.raw_nav']['eul_ZYX'])
-                if eul_ref.shape[0] == 3:
-                    eul_ref = np.transpose(eul_ref)
-                eul_is_degrees = eval(config['HDF.raw_nav']['eul_is_degrees'])
-                
-                ## Assuming It is given as roll, pitch, yaw
-                eul_ZYX_ref = np.flip(eul_ref, axis = 1)
-                quaternion_ref = RotLib.from_euler(angles = eul_ZYX_ref, seq = 'ZYX', degrees = eul_is_degrees).as_quat()
-                
-            else:
-                raise ValueError("The rotation reference type must be defined as quat or eul_ZYX")
-
-
-            is_global_rot = eval(config['HDF.raw_nav']['is_global_rot'])
-
-            # Parse position
-            position_ref = hyp.get_dataset(h5_filename=path_hdf,dataset_name=config['HDF.raw_nav']['position'])
-            
-            if position_ref.shape[0] == 3:
-                position_ref = np.transpose(position_ref)
-
-
-            timestamps_imu = hyp.get_dataset(h5_filename=path_hdf, dataset_name=config['HDF.raw_nav']['timestamp'])\
-                .reshape(-1)
-
-
-            # The rotation of the reference
-            rot_obj = RotLib.from_quat(quaternion_ref)
-
-            timestamp_hsi = hyp.dataCubeTimeStamps.reshape(-1)
-
-            # Compute interpolated absolute positions positions and orientation:
-            position_interpolated, quaternion_interpolated = interpolate_poses(timestamp_from=timestamps_imu,
-                                                             pos_from=position_ref,
-                                                             rot_from=rot_obj,
-                                                             timestamps_to=timestamp_hsi)
-
-            # If the original orientations are with respect to (North-East-Down) NED
-            if not is_global_rot:
-                rot_ref = 'NED'
-            else:
-                rot_ref = 'ECEF'
-
-            # The positions supplied for the reference
-            pos_epsg_orig = config['Coordinate Reference Systems']['pos_epsg_orig']
-
-            # The positions supplied for exporting the model
-            pos_epsg_export = config['Coordinate Reference Systems']['geocsc_epsg_export']
-
-            # The interpolated rotation-object
-            rot_interpolated = RotLib.from_quat(quaternion_interpolated)
-
-            # For simple geo-pose for changing between formats.
-            geo_pose_ref = GeoPose(timestamps=timestamp_hsi,
-                                   rot_obj= rot_interpolated, 
-                                   rot_ref=rot_ref,
-                                   pos = position_interpolated, 
-                                   pos_epsg=pos_epsg_orig)
-
-            # Convert position to the epsg used for the 3D model
-            geo_pose_ref.compute_geocentric_position(epsg_geocsc=pos_epsg_export)
-
-
-            # Calculate the geodetic position using the WGS-84 (for conversion of orientations)
-            epsg_wgs84 = 4326
-            geo_pose_ref.compute_geodetic_position(epsg_geod=epsg_wgs84)
-
-            # Calculate ECEF orientation
-            geo_pose_ref.compute_geocentric_orientation()
-
-            # For readability, extract the position and orientation wrt ECEF
-            position_ref_ecef = geo_pose_ref.pos_geocsc
-            quaternion_ref_ecef = geo_pose_ref.rot_obj_ecef.as_quat()
-
-            # For stacking in CSV
-            rot_vec_ecef = geo_pose_ref.rot_obj_ecef.as_euler('ZYX', degrees=True)
-
-            partial_pose = np.concatenate((timestamp_hsi.reshape((-1,1)), position_ref_ecef, rot_vec_ecef), axis=1)
-            if is_first:
-                # Initialize
-                total_pose = partial_pose
-                # Ensure that flag is not raised again. Offsets should only be set once.
-                is_first = False
-            else:
-                # Concatenate/stack poses
-                total_pose = np.concatenate((total_pose, partial_pose), axis=0)
-                is_first = False
-            
-            
-
-            # Add camera position
-            position_ref_name = config['HDF.processed_nav']['position_ecef']
-            Hyperspectral.add_dataset(data=position_ref_ecef, name=position_ref_name, h5_filename=path_hdf)
-
-            # Add camera quaternion
-            quaternion_ref_name = config['HDF.processed_nav']['quaternion_ecef']
-            Hyperspectral.add_dataset(data=quaternion_ref_ecef, name=quaternion_ref_name, h5_filename=path_hdf)
-
-            # Add time stamps
-            time_stamps_name = config['HDF.processed_nav']['timestamp']
-            Hyperspectral.add_dataset(data=timestamp_hsi, name=time_stamps_name, h5_filename=path_hdf)
-
-
-            
-
-
-    headers = ['Timestamp', ' X', ' Y', ' Z', ' RotZ', ' RotY', ' RotX']
-
-    # Create a DataFrame from the data_matrix and headers
-    # Stores the entire pose path
-    df = pd.DataFrame(total_pose, columns=headers)
-
-    pose_path = config['Absolute Paths']['pose_path']
-
-    try:
-        # Save the DataFrame as a CSV file
-        df.to_csv(pose_path, index=False)
-    except:
-        # Extract directory
-        directory = os.path.dirname(pose_path)
-
-        # Check if directory doesn't exist and create it
-        if not os.path.exists(directory):
-            os.makedirs(directory)
-        
-        df.to_csv(pose_path, index=False)
-
-# The main script for aquiring pose.        
-def export_pose(config_file):
-    """
-        Parses pose and embeds it into the *.h5 file. Writes the positions and orientations of hyperspectral frames to
-            dataset under the /Nav folder
-
-        Args:
-            config_file: The *.ini file containing the paths and configurations.
-
-        Returns:
-            config: The function returns config object to allow that it is modified.
-    """
-    config = configparser.ConfigParser()
-    config.read(config_file)
-
-    # This file handles pose exports of various types
-    # As of now there are three types:
-
-    # 1) Agisoft, h5_embedded and independent_file
-    try:
-        pose_export_type = config['General']['pose_export_type']
-    except:
-        # Default to h5_embedded
-        pose_export_type = 'h5_embedded'
-
-    if pose_export_type == 'h5_embedded':
-        config = reformat_h5_embedded_data_h5(config=config,
-                                              config_file=config_file)
-    elif pose_export_type == 'independent_file':
-        print('There is no support for this export functionality! Fix immediately!')
-        config = -1
-    else:
-        print('File type: ' + pose_export_type + 'type is not defined!')
-        config = -1
-
-    return config
-    
-    
-def export_model(config_file):
-    """"""
-    config = configparser.ConfigParser()
-    config.read(config_file)
-
-    # This file handles model exports of various types
-    # As of now there are three types:
-    # 1) Agisoft, *.ply file/DEM and None
-    model_export_type = config['General']['model_export_type']
-
-    if model_export_type == 'agisoft':
-        agisoft_export_model(config_file=config_file)
-    elif model_export_type == 'ply_file':
-        # Nothing needs to be done then?
-        pass
-    elif model_export_type == 'dem_file':
-        file_path_dem = config['Absolute Paths']['dem_path']
-        file_path_3d_model = config['Absolute Paths']['model_path']
-        # Make new only once.
-
-        if os.path.exists(file_path_3d_model):
-            print('3D model already exists and overwriting is not supported')
-            pass
-        else:
-            dem_2_mesh(path_dem=file_path_dem, model_path=file_path_3d_model, config=config)
-
-    elif model_export_type == 'geoid':
-        file_path_dem = config['Absolute Paths']['dem_path']
-        file_path_geoid = config['Absolute Paths']['geoid_path']
-        file_path_3d_model = config['Absolute Paths']['model_path']
-
-        # Crop the DEM to appropriate size based on poses and maximum ray length
-        crop_geoid_to_pose(path_dem=file_path_dem, config=config, geoid_path=file_path_geoid)
-
-        # Make into a 3D model
-        dem_2_mesh(path_dem=file_path_dem, model_path=file_path_3d_model, config=config)
-
-
-
-
-
-
-
-if __name__ == "__main__":
-    # Here we could set up necessary steps on a high level. 
-    args = sys.argv[1:]
-    config_file = args[0]
+# Python built-ins
+import sys
+import os
+import configparser
+from os import path
+
+# Third party libraries
+import numpy as np
+import pandas as pd
+from scipy.spatial.transform import Rotation as RotLib
+from scipy.spatial.transform import Rotation
+import h5py
+from scipy.spatial.transform import Rotation as RotLib
+import pandas as pd
+import pymap3d as pm
+from scipy.spatial.transform import Slerp
+from scipy.interpolate import interp1d
+from pyproj import CRS, Transformer
+
+# Local modules
+from gref4hsi.utils.geometry_utils import CameraGeometry, GeoPose
+from gref4hsi.utils.geometry_utils import rot_mat_ned_2_ecef, interpolate_poses
+from gref4hsi.utils.geometry_utils import dem_2_mesh, crop_geoid_to_pose
+
+
+class Hyperspectral:
+    """
+    Class for storing/accessing acquired hyperspectral data. One instance corresponds to a transect chunk (*.h5).
+    """
+    def __init__(self, filename, config, load_datacube = True):
+        """
+        Instantiate transect chunk object from chunk file name and config file.
+        :param filename: string
+        path to *.h5 file
+        :param config: config type
+        dictionary-like interface to configuration file
+        """
+        # Chunk filename
+        self.name = filename
+        # If errors arise due to improper dataset paths below, open the *.h5 file in hdfviewer and edit the path.
+        with h5py.File(filename, 'r', libver='latest') as self.f:
+            # TODO: Embed the paths from this special format into confic file
+            try:
+                dataCubePath = config['HDF.hyperspectral']['dataCube']
+            except:
+                pass
+            
+            try:
+                timestampHyperspectralPath = config['HDF.hyperspectral']['timestamp']
+                self.dataCubeTimeStamps = self.f[timestampHyperspectralPath][()]
+            except:
+                pass
+
+            try:
+                # The band center wavelengths
+                band2WavelengthPath = config['HDF.calibration']['band2Wavelength']
+                self.band2Wavelength = self.f[band2WavelengthPath][()]
+            except:
+                pass
+            
+            try:
+                # The band widths (if they exist)
+                fwhmPath = config['HDF.calibration']['fwhm']
+
+                self.fwhm = self.f[fwhmPath][()]
+            except:
+                pass
+
+            try:
+                # These should come together in the case that radiometric calibration should be done
+                radiometricFramePath = config['HDF.calibration']['radiometricFrame']
+                darkFramePath = config['HDF.calibration']['darkFrame']
+                exposureTimePath = config['HDF.hyperspectral']['exposureTime']
+                is_uhi = config['HDF']['is_uhi']
+
+                
+                if eval(is_uhi):
+                    self.t_exp = self.f[exposureTimePath][()][0] / 1000  # Recorded in milliseconds
+                else:
+                    self.t_exp = self.f[exposureTimePath][()] / 1000
+
+                self.darkFrame = self.f[darkFramePath][()]
+                self.radiometricFrame = self.f[radiometricFramePath][()]
+            except:
+                pass
+            
+            try:
+                RGBFramesPath = config['HDF.rgb']['rgbFrames']
+                timestampRGBPath = config['HDF.rgb']['timestamp']
+                try:
+                    # Extract RGB image data if available
+                    self.RGBTimeStamps = self.f[timestampRGBPath][()]
+                    self.RGBImgs = self.f[RGBFramesPath][()]
+                    self.n_imgs = self.RGBTimeStamps.shape[0]
+                except (UnboundLocalError, KeyError):
+                    pass
+            except:
+                pass
+            
+            
+
+            if load_datacube:
+                # To save memory, we made it an option to not load datacube
+                self.dataCube = self.f[dataCubePath][()]
+
+                self.n_scanlines = self.dataCube.shape[0]
+                self.n_pix = self.dataCube.shape[1]
+                self.n_bands = self.dataCube.shape[1]
+
+                # Calculate radiance cube if this is cube is not calibrated
+                self.digital_counts_2_radiance(config=config)
+
+            # Check if the dataset exists
+            processed_nav_folder = config['HDF.processed_nav']['folder']
+            
+            # Read the position da
+            if processed_nav_folder in self.f:
+                try:
+                    processed_nav_config = config['HDF.processed_nav']
+                    self.pos_ref = self.f[processed_nav_config['position_ecef']][()]
+                    self.quat_ref = self.f[processed_nav_config['quaternion_ecef']][()]
+                    self.pose_time = self.f[processed_nav_config['timestamp']][()]
+                except:
+                    pass
+            
+
+
+
+       
+
+            
+
+
+
+    def digital_counts_2_radiance(self, config):
+
+        # Only calibrate if data it is not already done
+        is_calibrated = eval(config['HDF.hyperspectral']['is_calibrated'])
+
+        if is_calibrated == is_calibrated:
+            self.dataCubeRadiance = self.dataCube.astype(np.float32)
+
+            # Add the radiance dataset
+            radiance_cube_path = config['HDF.hyperspectral']['dataCube']
+        else:
+            self.dataCubeRadiance = np.zeros(self.dataCube.shape, dtype = np.float32)
+            for i in range(self.dataCube.shape[0]):
+                self.dataCubeRadiance[i, :, :] = (self.dataCube[i, :, :] - self.darkFrame) / (
+                        self.radiometricFrame * self.t_exp)
+            
+            # Add the radiance dataset
+            radiance_cube_path = config['HDF.hyperspectral']['dataCube'] + '_radiance'
+            
+            # TODO: Write the radiance data to the h5 file
+            Hyperspectral.add_dataset(data = self.dataCubeRadiance, name=radiance_cube_path, h5_filename=self.name)
+        
+        config.set('HDF.hyperspectral', 'radiance_cube', radiance_cube_path)
+
+        # For memory efficiency
+        del self.dataCube
+
+        
+            
+            
+    
+    """def add_dataset(self, data, name):
+        
+        # The h5 file structure can be studied by unravelling the structure in Python or by using HDFview
+        with h5py.File(self.name, 'a', libver='latest') as self.f:
+            # Check if the dataset exists
+            if name in self.f:
+                del self.f[name]
+
+            dset = self.f.create_dataset(name=name, data = data)
+    """
+    
+    @staticmethod
+    def add_dataset(data, name, h5_filename):
+        """
+        Method to write a dataset to the h5 file
+        :param data: type any permitted (see h5py doc)
+        The data to be written
+        :param name: string
+        The path/name of the dataset
+        :param h5_filename: string
+        The path to the h5_file
+        :return: None
+        """
+        # The h5 file structure can be studied by unravelling the structure in Python or by using HDFview
+        with h5py.File(h5_filename, 'a', libver='latest') as f:
+            # Check if the dataset exists
+            if name in f:
+                del f[name]
+
+            dset = f.create_dataset(name=name, data = data)
+
+    """def get_dataset(self, dataset_name):
+        
+        Method to return a dataset by the name
+        :param dataset_name: string
+        The h5 dataset path
+        :return: dataset
+        Returns the queried dataset. Could be many datatypes, but mainly numpy arrays in our usage.
+        
+        # The h5 file structure can be studied by unravelling the structure in Python or by using HDFview
+        with h5py.File(self.name, 'a', libver='latest') as self.f:
+            dataset = self.f[dataset_name][()]
+        return dataset"""
+    @staticmethod
+    def get_dataset(h5_filename, dataset_name):
+        """equivalent to the method, except it does not need an instance of a Hyperspectral object
+
+        :param h5_filename: Path to h5/hdf file
+        :type h5_filename: string
+        :param dataset_name: h5 rooted path, e.g. processed/reflectance/remote_sensing_reflectance
+        :type dataset_name: string
+        :return: The dataset at the relevant location
+        :rtype: numpy array or other
+        """
+        # The h5 file structure can be studied by unravelling the structure in Python or by using HDFview
+        with h5py.File(h5_filename, 'a', libver='latest') as f:
+            dataset = f[dataset_name][()]
+        return dataset
+
+class DataLogger:
+    def __init__(self, filename, header):
+        self.filename = filename
+        # Generate file with header
+        with open(filename, 'w') as fh:
+            fh.write(header + '\n')
+
+    def append_data(self, data):
+        # Append data line to file
+        with open(self.filename, 'a') as fh:
+            # Generate data line to file
+            if data[0] != None:
+                line = ','.join([str(el) for el in data])
+
+                # Append line to file
+                fh.write(line + '\n')
+
+def ardupilot_extract_pose(config, iniPath):
+    
+    """
+        :param config: The processing configuration object (from */configuration.ini file)
+        :param iniPath: The path to */configuration.ini file
+        :return: 
+    """
+    
+    # Attitude retrieved from an ardupilot CSV
+    att_path = config['General']['ardupath'] + 'Att.csv'
+    df_att = pd.read_csv(att_path)
+
+    # Convert the DataFrame to a matrix (list of lists)
+    matrix_att = np.array(df_att.values.tolist())
+    
+    # Rotations in roll-pitch-yaw define the rotation of the vehicle's body frame (i.e. IMU)
+    Rotation = RotLib.from_euler("ZYX", np.flip(matrix_att[:,1:4], axis = 1), degrees=True)
+    time_rot = matrix_att[:,0]
+    
+    # Position retrieved from an ardupilot CSV
+    pos_path = config['General']['ardupath'] + 'pos.csv'
+    df_pos = pd.read_csv(pos_path)
+    matrix_pos = np.array(df_pos.values.tolist())
+
+    time_pos = matrix_pos[:, 0]
+    Position = matrix_pos[:, 1:4]
+
+    linearPositionInterpolator = interp1d(time_pos, np.transpose(Position), fill_value='extrapolate')
+    position_nav_interpolated = np.transpose(linearPositionInterpolator(time_rot))
+
+    pose_path = config['General']['ardupath'] + 'pose.csv'
+
+    config.set('General', 'pose_path', pose_path)
+
+    epsg_proj = 4326 # Standard
+    epsg_geocsc = config['General']['modelepsg']
+    # Transform the mesh points to ECEF.
+
+    geocsc = CRS.from_epsg(epsg_geocsc)
+    proj = CRS.from_epsg(epsg_proj)
+    transformer = Transformer.from_crs(proj, geocsc)
+
+    points_proj = position_nav_interpolated
+
+    lat = points_proj[:, 0].reshape((-1, 1))
+    lon = points_proj[:, 1].reshape((-1, 1))
+    hei = points_proj[:, 2].reshape((-1, 1))
+
+    (x_ecef, y_ecef, z_ecef) = transformer.transform(xx=lat, yy=lon, zz=hei)
+
+    pos_geocsc = np.concatenate((x_ecef.reshape((-1,1)), y_ecef.reshape((-1,1)), z_ecef.reshape((-1,1))), axis = 1)
+
+    #dlogr = DataLogger(pose_path, 'CameraLabel, X, Y, Z, Roll, Pitch, Yaw, RotX, RotY, RotZ')
+
+
+
+    data_matrix = np.zeros((len(time_rot), 10))
+    for i in range(len(time_rot)):
+
+        # Ardupilot delivers geodetic positions (EPSG::
+        pos_geod = position_nav_interpolated[i, :]
+
+        # Define rotation matrix between local tangential plane (NED, North-East-Down) and Earth-Centered-Earth-Fixed (ECEF).
+        R_n_e = rot_mat_ned_2_ecef(lat=pos_geod[0], lon=pos_geod[1])
+
+        Rotation_n = RotLib.from_matrix(R_n_e)
+
+        Rotation_e = Rotation_n*Rotation[i] # Composing rotations
+
+        roll = matrix_att[i, 1]
+        pitch = matrix_att[i, 2]
+        yaw = matrix_att[i, 3]
+
+        
+
+        rotz, roty, rotx = Rotation_e.as_euler("ZYX", degrees=True)
+
+        pos = pos_geocsc[i,:]
+
+        data_matrix[i,:] = np.array([time_rot[i], pos[0], pos[1], pos[2], roll, pitch, yaw, rotx, roty, rotz])
+
+        #dlogr.append_data([time_rot[i], pos[0], pos[1], pos[2], roll, pitch, yaw, rotx, roty, rotz])
+
+
+
+    headers = ['Timestamp', ' X', ' Y', ' Z', ' Roll', ' Pitch', ' Yaw', ' RotX', ' RotY', ' RotZ']
+
+    # Create a DataFrame from the data_matrix and headers
+    df = pd.DataFrame(data_matrix, columns=headers)
+
+    # Save the DataFrame as a CSV file
+    df.to_csv(pose_path, index=False)
+
+    with open(iniPath, 'w') as configfile:
+        config.write(configfile)
+        
+    return config
+
+
+def reformat_h5_embedded_data_h5(config, config_file):
+    """
+                Parses pose from h5, interpolates and reformats. Writes the positions and orientations of hyperspectral frames to
+                    dataset under the /Nav folder
+
+                Args:
+                    config_file: The *.ini file containing the paths and configurations.
+
+                Returns:
+                    None: The function returns nothing.
+    """
+
+
+    # Traverse through h5 dir to append the data to file
+    h5_folder = config['Absolute Paths']['h5_folder']
+    is_first = True
+    for filename in sorted(os.listdir(h5_folder)):
+        
+        # Find the interesting prefixes
+        if filename.endswith('h5') or filename.endswith('hdf'):
+            # Identify the total path
+            path_hdf = h5_folder + filename
+
+            # Read out the data of a file
+            hyp = Hyperspectral(path_hdf, config, load_datacube = False)
+
+
+            # If rotation reference is quaternion:
+            # Alternatives quat, eul_ZYX
+            rotation_reference_type = config['HDF.raw_nav']['rotation_reference_type']
+            if rotation_reference_type == 'quat':
+                quaternion_ref = hyp.get_dataset(h5_filename=path_hdf, dataset_name=config['HDF.raw_nav']['quaternion'])
+                if quaternion_ref.shape[0] == 4:
+                    quaternion_ref = np.transpose(quaternion_ref)
+                
+            
+                quaternion_convention  = config['HDF.raw_nav']['quaternion_convention']
+
+                # If scalar-first convention
+                if quaternion_convention == 'wxyz':
+                    quat_temp = quaternion_ref
+                    quaternion_ref = np.roll(quaternion_ref, shift=-1, axis=1)
+                elif quaternion_convention == 'xyzw':
+                    # We use the xyzw convention for scipy, see:
+                    # https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.transform.Rotation.from_quat.html
+                    pass
+                else:
+                    raise ValueError("The quaternion convention must be defined")
+            elif rotation_reference_type == 'eul_ZYX':
+                eul_ref = hyp.get_dataset(h5_filename=path_hdf,dataset_name=config['HDF.raw_nav']['eul_ZYX'])
+                if eul_ref.shape[0] == 3:
+                    eul_ref = np.transpose(eul_ref)
+                eul_is_degrees = eval(config['HDF.raw_nav']['eul_is_degrees'])
+                
+                ## Assuming It is given as roll, pitch, yaw
+                eul_ZYX_ref = np.flip(eul_ref, axis = 1)
+                quaternion_ref = RotLib.from_euler(angles = eul_ZYX_ref, seq = 'ZYX', degrees = eul_is_degrees).as_quat()
+                
+            else:
+                raise ValueError("The rotation reference type must be defined as quat or eul_ZYX")
+
+
+            is_global_rot = eval(config['HDF.raw_nav']['is_global_rot'])
+
+            # Parse position
+            position_ref = hyp.get_dataset(h5_filename=path_hdf,dataset_name=config['HDF.raw_nav']['position'])
+            
+            if position_ref.shape[0] == 3:
+                position_ref = np.transpose(position_ref)
+
+
+            timestamps_imu = hyp.get_dataset(h5_filename=path_hdf, dataset_name=config['HDF.raw_nav']['timestamp'])\
+                .reshape(-1)
+
+
+            # The rotation of the reference
+            rot_obj = RotLib.from_quat(quaternion_ref)
+
+            timestamp_hsi = hyp.dataCubeTimeStamps.reshape(-1)
+
+            # Compute interpolated absolute positions positions and orientation:
+            position_interpolated, quaternion_interpolated = interpolate_poses(timestamp_from=timestamps_imu,
+                                                             pos_from=position_ref,
+                                                             rot_from=rot_obj,
+                                                             timestamps_to=timestamp_hsi)
+
+            # If the original orientations are with respect to (North-East-Down) NED
+            if not is_global_rot:
+                rot_ref = 'NED'
+            else:
+                rot_ref = 'ECEF'
+
+            # The positions supplied for the reference
+            pos_epsg_orig = config['Coordinate Reference Systems']['pos_epsg_orig']
+
+            # The positions supplied for exporting the model
+            pos_epsg_export = config['Coordinate Reference Systems']['geocsc_epsg_export']
+
+            # The interpolated rotation-object
+            rot_interpolated = RotLib.from_quat(quaternion_interpolated)
+
+            # For simple geo-pose for changing between formats.
+            geo_pose_ref = GeoPose(timestamps=timestamp_hsi,
+                                   rot_obj= rot_interpolated, 
+                                   rot_ref=rot_ref,
+                                   pos = position_interpolated, 
+                                   pos_epsg=pos_epsg_orig)
+
+            # Convert position to the epsg used for the 3D model
+            geo_pose_ref.compute_geocentric_position(epsg_geocsc=pos_epsg_export)
+
+
+            # Calculate the geodetic position using the WGS-84 (for conversion of orientations)
+            epsg_wgs84 = 4326
+            geo_pose_ref.compute_geodetic_position(epsg_geod=epsg_wgs84)
+
+            # Calculate ECEF orientation
+            geo_pose_ref.compute_geocentric_orientation()
+
+            # For readability, extract the position and orientation wrt ECEF
+            position_ref_ecef = geo_pose_ref.pos_geocsc
+            quaternion_ref_ecef = geo_pose_ref.rot_obj_ecef.as_quat()
+
+            # For stacking in CSV
+            rot_vec_ecef = geo_pose_ref.rot_obj_ecef.as_euler('ZYX', degrees=True)
+
+            partial_pose = np.concatenate((timestamp_hsi.reshape((-1,1)), position_ref_ecef, rot_vec_ecef), axis=1)
+            if is_first:
+                # Initialize
+                total_pose = partial_pose
+                # Ensure that flag is not raised again. Offsets should only be set once.
+                is_first = False
+            else:
+                # Concatenate/stack poses
+                total_pose = np.concatenate((total_pose, partial_pose), axis=0)
+                is_first = False
+            
+            
+
+            # Add camera position
+            position_ref_name = config['HDF.processed_nav']['position_ecef']
+            Hyperspectral.add_dataset(data=position_ref_ecef, name=position_ref_name, h5_filename=path_hdf)
+
+            # Add camera quaternion
+            quaternion_ref_name = config['HDF.processed_nav']['quaternion_ecef']
+            Hyperspectral.add_dataset(data=quaternion_ref_ecef, name=quaternion_ref_name, h5_filename=path_hdf)
+
+            # Add time stamps
+            time_stamps_name = config['HDF.processed_nav']['timestamp']
+            Hyperspectral.add_dataset(data=timestamp_hsi, name=time_stamps_name, h5_filename=path_hdf)
+
+
+            
+
+
+    headers = ['Timestamp', ' X', ' Y', ' Z', ' RotZ', ' RotY', ' RotX']
+
+    # Create a DataFrame from the data_matrix and headers
+    # Stores the entire pose path
+    df = pd.DataFrame(total_pose, columns=headers)
+
+    pose_path = config['Absolute Paths']['pose_path']
+
+    try:
+        # Save the DataFrame as a CSV file
+        df.to_csv(pose_path, index=False)
+    except:
+        # Extract directory
+        directory = os.path.dirname(pose_path)
+
+        # Check if directory doesn't exist and create it
+        if not os.path.exists(directory):
+            os.makedirs(directory)
+        
+        df.to_csv(pose_path, index=False)
+
+# The main script for aquiring pose.        
+def export_pose(config_file):
+    """
+        Parses pose and embeds it into the *.h5 file. Writes the positions and orientations of hyperspectral frames to
+            dataset under the /Nav folder
+
+        Args:
+            config_file: The *.ini file containing the paths and configurations.
+
+        Returns:
+            config: The function returns config object to allow that it is modified.
+    """
+    config = configparser.ConfigParser()
+    config.read(config_file)
+
+    # This file handles pose exports of various types
+    # As of now there are three types:
+
+    # 1) Agisoft, h5_embedded and independent_file
+    try:
+        pose_export_type = config['General']['pose_export_type']
+    except:
+        # Default to h5_embedded
+        pose_export_type = 'h5_embedded'
+
+    if pose_export_type == 'h5_embedded':
+        reformat_h5_embedded_data_h5(config=config,
+                                              config_file=config_file)
+    elif pose_export_type == 'independent_file':
+        print('There is no support for this export functionality! Fix immediately!')
+        config = -1
+    else:
+        print('File type: ' + pose_export_type + 'type is not defined!')
+        config = -1
+
+    
+    
+def export_model(config_file):
+    """"""
+    config = configparser.ConfigParser()
+    config.read(config_file)
+
+    # This file handles model exports of various types
+    # As of now there are three types:
+    # 1) Agisoft, *.ply file/DEM and None
+    model_export_type = config['General']['model_export_type']
+
+    if model_export_type == 'agisoft':
+        agisoft_export_model(config_file=config_file)
+    elif model_export_type == 'ply_file':
+        # Nothing needs to be done then?
+        pass
+    elif model_export_type == 'dem_file':
+        file_path_dem = config['Absolute Paths']['dem_path']
+        file_path_3d_model = config['Absolute Paths']['model_path']
+        # Make new only once.
+
+        if os.path.exists(file_path_3d_model):
+            print('3D model already exists and overwriting is not supported')
+            pass
+        else:
+            dem_2_mesh(path_dem=file_path_dem, model_path=file_path_3d_model, config=config)
+
+    elif model_export_type == 'geoid':
+        file_path_dem = config['Absolute Paths']['dem_path']
+        file_path_geoid = config['Absolute Paths']['geoid_path']
+        file_path_3d_model = config['Absolute Paths']['model_path']
+
+        # Crop the DEM to appropriate size based on poses and maximum ray length
+        crop_geoid_to_pose(path_dem=file_path_dem, config=config, geoid_path=file_path_geoid)
+
+        # Make into a 3D model
+        dem_2_mesh(path_dem=file_path_dem, model_path=file_path_3d_model, config=config)
+
+
+
+
+
+
+
+if __name__ == "__main__":
+    # Here we could set up necessary steps on a high level. 
+    args = sys.argv[1:]
+    config_file = args[0]
```

### Comparing `gref4hsi-0.2.1/gref4hsi/utils/radiometry.py` & `gref4hsi-0.2.2/gref4hsi/utils/radiometry.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,705 +1,705 @@
-
-
-
-
-from collections import namedtuple
-
-import numpy as np
-import pandas as pd
-from scipy.interpolate import interp1d
-from scipy.special import expi
-from scipy.special import erf
-from scipy.special import erfi
-from scipy.optimize import fsolve
-import matplotlib.pyplot as plt
-
-def fresnel(theta_i, n_i, n_t, is_transmittance, method):
-    # This is used for computing the transmittance at the interfaces
-    # First Snells:
-    if method == 1:
-        theta_t = np.arcsin((n_i / n_t)*np.sin(theta_i))
-
-        c_i = np.cos(theta_i)
-        c_t = np.cos(theta_t)
-
-        R_s = np.abs((n_i*c_i - n_t*c_t)/(n_i*c_i + n_t*c_t))**2
-
-        R_p = np.abs((n_i*c_t - n_t*c_i)/(n_i*c_t + n_t*c_i))**2
-
-        # Then snells:
-        R_F = 0.5*(R_s + R_p)
-
-
-    elif method == 2:
-        theta_t = np.arcsin((n_i / n_t) * np.sin(theta_i))
-
-        r1 = (np.sin(theta_i - theta_t)/np.sin(theta_i + theta_t))**2
-        r2 = (np.tan(theta_i - theta_t) / np.tan(theta_i + theta_t)) ** 2
-
-        R_F = 0.5 * (r1 + r2)
-    if is_transmittance:
-        return 1 - R_F
-    else:
-        return R_F
-
-
-
-
-def solid_angle_ratio(theta_w, n_w):
-    """Computes the in-air angle corresponding to an in-water angle using Snell's law"""
-    n_a = 1 # Approximate n_a = 1
-    theta_a = np.arcsin((n_w / n_a) * np.sin(theta_w)) # Snells law
-    return theta_a
-
-def immersion_factor(theta_w, n_w, n_g, pixel_nr):
-    """Calculates the immersion factor for imager with planar glass port in underwater hyperspectral imaging"""
-    n_a = 1
-
-    theta_a = np.arcsin((n_w / n_a) * np.sin(theta_w))
-
-    t_ag = fresnel(theta_i=theta_a, n_i = n_a, n_t = n_g, is_transmittance=1, method=1)
-
-    t_wg = fresnel(theta_i=theta_w, n_i=n_w, n_t=n_g, is_transmittance=1, method=1)
-
-    I_f_LU = ((n_w**2)/(n_a**2) ) * (t_ag/t_wg)
-
-    I_f = I_f_LU[pixel_nr.reshape(-1), :]
-
-    return I_f
-
-
-
-def radiance_conversion(RF, t_exp, pixel_nr):
-
-    rad_2_DN_LU = RF*t_exp
-
-    rad_2_DN = rad_2_DN_LU[pixel_nr.reshape(-1)] # Evaluate for relevant pixels
-    return rad_2_DN
-
-
-
-def beam_pattern(dir_s0, dir, sigma, I_0, I_hat):
-    n = dir.shape[0]
-    k = I_hat.shape[0]
-    # A gaussian beam pattern
-    dot_prod = np.dot(dir_s0, np.transpose(dir))
-
-    len_vec = np.linalg.norm(dir_s0)*np.linalg.norm(dir, axis = 1)
-
-    theta_si = np.arccos(dot_prod/len_vec)
-
-
-
-    z = (theta_si)/sigma
-
-    Intensity = I_0*np.exp(-0.5*z**2)
-
-    Intensity_Spectral = np.multiply(Intensity.reshape((-1, 1)), I_hat.reshape((1, -1)))
-
-    return Intensity/I_0, Intensity_Spectral
-
-def compute_gamma(dir, normals):
-    """Compute the angle between a normal vector and an incoming ray"""
-    dot_prod = np.einsum('ij, ij -> i', normals, -dir)
-    len_vec = np.linalg.norm(dir, axis = 1) * np.linalg.norm(normals, axis = 1)
-    gamma = np.arccos(dot_prod/len_vec)
-    return gamma.reshape((-1, 1))
-
-def compute_n_g(wlen):
-    n_g = 1.4424 + (7.1661/(wlen - 144.170))
-    return n_g
-
-def compute_n_w(wlen, method):
-    if method == 1:
-        n_w = 1.325147 + (6.6096/(wlen - 137.1924))
-    elif method == 2:
-        T = 10
-        a = -0.000001501562500
-        b = 0.000000107084865
-        c = -0.000042759374989
-        d = -0.000160475520686
-        e = 1.398067112092424
-        # Function of Slocum
-
-        n_w = a * T ** 2 + b * wlen ** 2 + c * T + d * wlen + e
-
-    return n_w
-
-def compute_scattering_integral(k, x):
-
-    Ei = expi(x = -2*x*k)
-
-    integral = -(2*k*x*Ei + np.exp(-k*x)) / x
-
-    return integral
-
-def compute_backscatter(B_p, b, b_w, b_p, d_pix, pos_seabed, p_si, dir_s0, sigma_l, I_0, I_hat, k, pixel_nr):
-    # Step 1 create a lookup table for pixelnumber and perp distance
-    z_res = 0.05
-
-    z_max = pos_seabed[:, 2].max()
-
-    # Partition
-    z = (np.arange(0, np.ceil(z_max/z_res) + 1)*z_res).reshape((-1, 1, 1))
-
-    r_si_b = z * d_pix - p_si # t by m by 3
-
-    l_si_b = np.linalg.norm(r_si_b, axis =2).reshape((r_si_b.shape[0], r_si_b.shape[1], 1)) # t by m by 1 or something
-
-    r_b_h = -z*d_pix # t by m by 3
-
-    l_b_h = np.linalg.norm(r_b_h, axis=2).reshape((r_si_b.shape[0], r_si_b.shape[1], 1))  # t by m by 1 or something
-
-    BP_norm, BP = beam_pattern(dir_s0=dir_s0, dir=r_si_b.reshape((-1, 3)), sigma=sigma_l, I_0=I_0, I_hat=I_hat).reshape((r_si_b.shape[0], r_si_b.shape[1], I_hat.shape[0]))
-
-    E_i = BP*(1/(l_si_b**2))*np.exp(-k*l_si_b) # Values of incident irradiance for all directions and all perpendicular
-
-
-    # distances t by m by k. Part of the integrand
-
-    # Compute psi for all t by m cells. Check that angles are on the right side of 90 deg
-
-    dot_prod = np.einsum('jk, ijk -> ij', d_pix, r_si_b)
-    len_vec = np.linalg.norm(d_pix, axis=1) * np.linalg.norm(r_si_b, axis=2)
-    psi = np.pi - np.arccos(dot_prod / len_vec)
-
-    beta_p_interp = fournier_forand(B_p)  # Assumed constant backscatter fraction across wl. Is a log-log interpolator
-
-    beta_p = np.exp( beta_p_interp(np.log(psi)) ).reshape((r_si_b.shape[0], r_si_b.shape[1], 1)) # Due to the interpolation in log-log domain. t by m
-
-    beta_w = compute_beta_w(psi).reshape((r_si_b.shape[0], r_si_b.shape[1], 1)) # t by m
-
-    beta_tot = (1/b)*(b_p*beta_p + b_w*beta_w) # t by m by k
-
-    integrand = E_i*beta_tot*np.exp(-k*l_b_h) # t by m by k
-
-    integral = np.cumsum(integrand, axis = 0)*z_res # Summing along the z axis weighted by z_res. Should return a t by m by k.
-
-
-
-    L_b_LU = b*integral # Should return a t by m by k.
-
-    # Can compute row of a given measurement by:
-    rows = np.round(pos_seabed[:, 2]/z_res).astype(np.int64).reshape(-1)
-    cols = pixel_nr.reshape(-1)
-
-    L_b = L_b_LU[rows, cols, :] # Returns the appropriate spectra n by k
-
-    #print(stop - start)
-
-    return L_b
-
-
-
-
-
-
-
-
-
-def compute_light_source_integral(sigma):
-    """Computes the relation between spectral radiant flux P [W] and peak intensity I_0 [W/sr] for a directionally gaussian beam
-    with sigma standard decviation"""
-    constant = np.exp(-0.5 * sigma ** 2) * sigma
-
-    term1 = -0.626657j * erf(0 + 0.707107j * sigma)
-    term2 = 0.626657j * erf(1.11072 / sigma + 0.707107j * sigma)
-    term3 = -0.626657 * erfi((0.707107 * (sigma ** 2 + 1.5708j)) / sigma)
-    term4 = 0.626657 * erfi(0.707107 * sigma + 0j)
-
-    return np.real(constant * (term1 + term2 + term3 + term4))*2*np.pi
-
-def fournier_forand(B_p):
-    """Calculates the phase function values for a given backscatter fraction"""
-
-    # Partition data into equal 100 bins from 10 degrees to 100:
-    logPsi = np.linspace(np.log(10*np.pi/180), np.log(180*np.pi/180), 100)
-    psi = np.exp(logPsi)
-    # Convert B_p to FF parameters
-    mu, n = compute_FF_params(B_p)
-    #
-    nu = (3 - mu) / 2
-
-    delta = (4 * (np.sin(psi / 2)) ** 2) / (3 * (n - 1) ** 2) # Correct, Mobley 2002 eq 2
-
-    delta_180 = 4 / (3 * (n - 1) ** 2)
-
-    beta_ff_t1 = 1 / (4 * np.pi * ((1 - delta) ** 2) * (delta ** nu))  # Coeff 1, correct
-
-    beta_ff_t2 = nu * (1 - delta) - (1 - delta ** nu) # Correct
-
-    beta_ff_t3 = delta * (1 - delta ** nu) - nu * (1 - delta) # *Correct
-
-    beta_ff_t4 = 1 / (np.sin(psi / 2) ** 2) # Correct
-
-    beta_ff_t5 = (1 - delta_180 ** nu) / (16 * np.pi * (delta_180 - 1) * delta_180 ** nu)
-
-    beta_ff_t6 = 3 * np.cos(psi) ** 2 - 1
-
-    beta_ff = beta_ff_t1 * (beta_ff_t2 + beta_ff_t3 * beta_ff_t4) \
-              + beta_ff_t5 * beta_ff_t6  ## Formula t1*(t2+t3*t4) + t5*t6
-
-    # Instantiate an interpolation object that describes the function
-    beta_ff_interp = interp1d(x = logPsi, y = np.log(beta_ff), kind = 'cubic', fill_value='extrapolate')
-
-    return beta_ff_interp
-
-def compute_FF_params(B_p):
-    mu_0 = 4 # Midpoint between max and min allowed values
-    mu = fsolve(eq_backscatter_param, mu_0, args = (B_p,))
-    n = 1.01 + 0.1542*(mu-3) # Eq 621, p 202 ocean optics
-    return mu, n
-
-    #
-
-def eq_backscatter_param(mu, B_p_true):
-    n = 1.01 + 0.1542*(mu-3) # Eq 621, p 202 ocean optics
-    nu = (3-mu)/2 # eq 2 mobley 2002
-
-    psi_90 = np.pi/2
-
-    delta_90 = (4/( 3*(n-1)**2 ))*np.sin(psi_90/2)**2  # eq 2 mobley 2002
-
-    num = (1 - delta_90**(nu+1) - 0.5*(1 - delta_90**nu))
-    den = (1 - delta_90)*delta_90**nu
-
-    B_p = 1 - num/den
-
-    return B_p_true - B_p
-
-
-
-def compute_beta_w(psi):
-    """The scattering phase function of pure water"""
-    # Psi is an array of scattering angles
-    # Analytical Formula from Ocean Optics p. 180
-    return 0.0608*(1 + 0.925*(np.cos(psi))**2)
-
-
-
-
-class Radiometry():
-    def __init__(self, config, data1, data2):
-        # Read in necessary information. i.e. water absorption and water scattering coefs
-        path_iop_water = 'C:/Users/haavasl/PycharmProjects/newGit/TautraReflectanceTools/Misc/iop_pure_water.txt'
-        df_light = pd.read_csv('C:/Users/haavasl/PycharmProjects/newGit/TautraReflectanceTools/Misc/DataMultiSeaLite.txt',
-                         header=None)
-
-        #df_light = pd.read_csv(
-        #    'C:/Users/haavasl/PycharmProjects/newGit/TautraReflectanceTools/Misc/Multi_SeaLite_spectrum.csv',
-        #    header=0)
-
-        df_iop = pd.read_csv(path_iop_water, header=9, sep=',') # Should be interpolated
-
-        df_coral = pd.read_csv(
-            'C:/Users\haavasl\PycharmProjects/newGit\TautraReflectanceTools\Misc\Coral_spectra_lab.csv', sep=';')
-
-        df_refl_plaque = pd.read_csv('C:/Users\haavasl\PycharmProjects/newGit\TautraReflectanceTools\Misc/reflectance_plaque.csv')
-
-        interpol_coral = interp1d(df_coral.iloc[:, 0].astype(np.float64),
-                                np.transpose(df_coral.iloc[:, 2:4].astype(np.float64)), fill_value='extrapolate')
-        interpol_iop = interp1d(df_iop.iloc[:, 0].astype(np.float64), np.transpose(df_iop.iloc[:, 1:3].astype(np.float64)))
-        interpol_light = interp1d(df_light.iloc[:, 0], np.transpose(df_light.iloc[:, 1]), fill_value='extrapolate')
-
-        interpol_refl = interp1d(df_refl_plaque.iloc[:, 0], np.transpose(df_refl_plaque.iloc[:, 1]))
-
-        refl_gt = interpol_refl(data1.bands)
-
-        I_hat = interpol_light(data1.bands) # Total spectral radiant flux
-        a_w, b_w = interpol_iop(data1.bands)
-        s1, s2 = interpol_coral(data1.bands)
-        refl_gt_coral = 0.5*(s1 + s2) # Mean of measurements
-
-        n_w = compute_n_w(wlen = data1.bands, method = 2)
-        n_g = compute_n_g(wlen = data1.bands)
-
-        # data contains RadData(rad = rad_2, points = points_local_2, normals=normals_local_2, pixel_nr=pixel_2, bands=bands_2, angles)
-
-        Var = namedtuple('Var', ['points1', 'normals1', 'pixel_nr1', 'bands1', 'angles1','RF1','t_exp1', 'points2', 'normals2', 'pixel_nr2', 'bands2', 'angles2', 'RF2', 't_exp2'])
-
-        self.Var =  Var(points1 = data1.points, normals1=data1.normals, pixel_nr1=data1.pixel_nr, bands1=data1.bands, angles1=data1.angles, RF1 = data1.RF, t_exp1 = data1.t_exp,
-                         points2 = data2.points, normals2=data2.normals, pixel_nr2=data2.pixel_nr, bands2=data2.bands, angles2=data2.angles, RF2 = data2.RF, t_exp2 = data2.t_exp)
-
-
-        # Structure the data in 1) constants, 2) measurements y, 3) variables x and 4) parameters beta
-        Meas = namedtuple('Meas', ['rad1', 'rad2'])
-        self.Meas = Meas(rad1 = data1.rad, rad2=data2.rad)
-
-
-
-        Const = namedtuple('Const', ['S', 'a_w', 'b_w', 'n_g', 'n_w', 'dir_s1', 'dir_s2', 'pos_s1', 'pos_s2', 'I_hat', 'refl_gt', 'refl_gt_coral'])
-        self.Const = Const(S = 0.015, a_w = a_w, b_w = b_w, n_g = n_g, n_w=n_w, dir_s1=np.array([0,0,1]), dir_s2=np.array([0,0,1]),
-                           pos_s1 = np.array([0.35, 0, 0]), pos_s2 = np.array([-0.35, 0, 0]), I_hat = I_hat, refl_gt= refl_gt, refl_gt_coral = refl_gt_coral)
-
-
-        Param = namedtuple('Param', ['G', 'X', 'Y', 'B_p', 'alpha', 'I_0', 'sigma_l', 'k_l'])
-        self.Param = Param(G = 0.1, X = 0.1, Y = 1, B_p=0.01, alpha = 0, I_0 = 1, sigma_l = 1, k_l = 0)
-    def run_forward_model(self, is_skogn, model = 'forward'):
-        #print('This function is yet to be made')
-        if model == 'two way':
-            self.refl_1 = self.two_way_model_simple(id = 1, is_skogn = is_skogn)
-            self.refl_2 = self.two_way_model_simple(id = 2, is_skogn = is_skogn)
-        if model == 'forward':
-            self.diff_dc1 = self.forward_model_simple(id=1, is_skogn=is_skogn)
-            self.diff_dc2 = self.forward_model_simple(id=2, is_skogn=is_skogn)
-
-
-
-            # Could also propagate the uncertainty into the model by perturbing
-
-
-    def set_parameters(self, G, X, Y, B_p, alpha, I_0, sigma_l, k_l):
-        #self.Param = Param(G=0.1, X=0.1, Y=1, alpha=0, I_0=1, sigma_l=1)
-        Param = namedtuple('Param', ['G', 'X', 'Y', 'B_p', 'alpha', 'I_0', 'sigma_l', 'k_l'])
-        self.Param = Param(G=G, X=X, Y=Y, B_p = B_p, alpha=alpha, I_0=I_0, sigma_l=sigma_l, k_l = k_l)
-
-
-
-
-
-    def two_way_model_simple(self, id, is_skogn):
-        # The formward model computes
-        # Parameters
-        G = self.Param.G
-        X = self.Param.X
-        Y = self.Param.Y
-        B_p = self.Param.B_p
-
-
-        I_0 = self.Param.I_0
-        sigma_l = self.Param.sigma_l
-        alpha = self.Param.alpha
-        #B_inf1 = self.Param.B_inf
-        #B_inf2 = self.Param.B_inf
-        #p1  = self.Param.p1
-        #p2 = self.Param.p2
-        #theta_s1 = self.Param.theta_s1
-
-
-        if id == 1:
-            # Measurements
-            L_air = self.Meas.rad1
-            # Variables
-            wlen = self.Var.bands1
-            pos_seabed = self.Var.points1
-            norm_vec = self.Var.normals1
-            theta_w_dot = self.Var.angles1
-            pixel_nr = self.Var.pixel_nr1
-        elif id == 2:
-            # Measurements
-            L_air = self.Meas.rad2
-            # Variables
-            wlen = self.Var.bands2
-            pos_seabed = self.Var.points2
-            norm_vec = self.Var.normals2
-            theta_w_dot = self.Var.angles2
-            pixel_nr = self.Var.pixel_nr2
-
-
-        # Constants
-        a_ph = 0
-        a_w = self.Const.a_w
-        b_w = self.Const.b_w
-        S = self.Const.S
-        dir_s10 = self.Const.dir_s1
-        dir_s20 = self.Const.dir_s2
-        pos_s1 = self.Const.pos_s1
-        pos_s2 = self.Const.pos_s2
-        n_w = self.Const.n_w.reshape((1, -1))
-        n_g = self.Const.n_g.reshape((1, -1))
-
-
-        I_hat_non_scaled = self.Const.I_hat
-
-
-        k_scale = self.Param.k_l
-
-        I_hat = I_hat_non_scaled * (1 +  k_scale*(wlen - wlen[100]))
-
-
-
-
-
-        # Eq. 9a)-9f)
-        b_bw = 0.5 * b_w #Water is isotrophic
-        a_g = G*np.exp(-S*(wlen - 440))
-        b_bp = X * (400 / wlen) ** Y
-        b_p = b_bp/B_p
-        a = a_w + a_ph + a_g
-        b = b_w + b_p
-
-        b_b = b_bw + b_bp
-
-        k = (a + b_b).reshape((1, -1))
-
-        import matplotlib.pyplot as plt
-
-        #plt.show()
-#
-        #plt.plot(wlen, I_hat*I_0)
-        #plt.show()
-        # Vector from source to bottom
-        dir_s1 = pos_seabed - pos_s1
-        dir_s2 = pos_seabed - pos_s2
-        # Length of those
-        R_s1 = np.linalg.norm(dir_s1, axis = 1).reshape((-1, 1))
-        R_s2 = np.linalg.norm(dir_s2, axis = 1).reshape((-1, 1))
-        # Length of camera-bottom vector
-        R_c = np.linalg.norm(pos_seabed, axis = 1).reshape((-1, 1))
-
-        # Returns an n by k vector where k are the spectral
-        BP1_norm, BP1 = beam_pattern(dir_s0=dir_s10, dir = dir_s1, sigma= sigma_l, I_0 = I_0, I_hat = I_hat)
-        BP2_norm, BP2 = beam_pattern(dir_s0=dir_s20, dir = dir_s2, sigma=sigma_l, I_0=I_0, I_hat = I_hat)
-
-        # Returns an n by 1 vector of cosines
-        gamma_s1 = compute_gamma(dir = dir_s1, normals = norm_vec)
-        gamma_s2 = compute_gamma(dir=dir_s2, normals = norm_vec)
-
-        if id == 1:
-            self.cos_gamma_s1_t1 = np.cos(gamma_s1)
-            self.cos_gamma_s2_t1 = np.cos(gamma_s2)
-            self.BP1_norm_t1 = BP1_norm
-            self.BP2_norm_t1 = BP2_norm
-            self.R_s1_t1 = R_s1
-            self.R_s2_t1 = R_s2
-
-        elif id == 2:
-            # Measurements
-            self.cos_gamma_s1_t2 = np.cos(gamma_s1)
-            self.cos_gamma_s2_t2 = np.cos(gamma_s2)
-            self.BP1_norm_t2 = BP1_norm
-            self.BP2_norm_t2 = BP2_norm
-            self.R_s1_t2 = R_s1
-            self.R_s2_t2 = R_s2
-
-        # Simple computation of incident light
-        E_i1 = BP1 * np.cos(gamma_s1) * np.exp(-k * R_s1) / (R_s1 ** 2)
-        E_i2 = BP2 * np.cos(gamma_s2) * np.exp(-k * R_s2) / (R_s2 ** 2)
-
-
-
-
-        import matplotlib.pyplot as plt
-
-
-        if is_skogn == False:
-            E_i = E_i1 + E_i2
-        else:
-            E_i = E_i1 # Only this light source that is illuminating the scene
-
-        # Calculate from measurement to seafloor
-        theta_w = theta_w_dot - alpha # Intersection angle with respect to glass
-
-        I_f = immersion_factor(theta_w=theta_w, n_w = n_w, n_g = n_g, pixel_nr = pixel_nr)
-
-        L_w = np.einsum('ij,ij -> ij', L_air, I_f)
-
-        #if id == 2:
-        #    from scipy.ndimage import gaussian_filter1d
-        #    plt.hist(L_air.reshape(-1), 100)
-        #    plt.show()
-
-        # Compute backscatter
-        include_backscatter = False
-        if include_backscatter:
-            x_pix = np.tan(theta_w_dot).reshape((-1, 1))
-            y_pix = np.zeros(x_pix.shape)
-            z_pix = np.ones(x_pix.shape)
-            d_pix = np.concatenate((x_pix, y_pix, z_pix), axis = 1)
-            k_bands = k.shape[1]
-
-            if is_skogn:
-                L_s1 = compute_backscatter(B_p=B_p, b=b.reshape((1, 1, k_bands)), b_w=b_w.reshape((1, 1, k_bands)),
-                                           b_p=b_p.reshape((1, 1, k_bands)), d_pix=d_pix, pos_seabed=pos_seabed,
-                                           p_si=pos_s1, dir_s0=dir_s10, sigma_l=sigma_l,
-                                           I_0=I_0, I_hat=I_hat, k=k.reshape((1, 1, k_bands)), pixel_nr=pixel_nr)
-                L_s = L_s1# The total scattered light
-            else:
-
-                L_s1 = compute_backscatter(B_p = B_p, b = b.reshape((1, 1, k_bands)), b_w = b_w.reshape((1, 1, k_bands)),
-                                           b_p = b_p.reshape((1, 1, k_bands)), d_pix = d_pix, pos_seabed = pos_seabed,
-                                           p_si = pos_s1, dir_s0 = dir_s10, sigma_l = sigma_l,
-                                           I_0 = I_0, I_hat = I_hat, k= k.reshape((1, 1, k_bands)), pixel_nr = pixel_nr)
-
-                L_s2 = compute_backscatter(B_p=B_p, b=b.reshape((1, 1, k_bands)), b_w=b_w.reshape((1, 1, k_bands)),
-                                           b_p=b_p.reshape((1, 1, k_bands)), d_pix=d_pix, pos_seabed=pos_seabed,
-                                           p_si=pos_s2, dir_s0=dir_s20, sigma_l=sigma_l,
-                                           I_0=I_0, I_hat=I_hat, k=k.reshape((1, 1, k_bands)), pixel_nr=pixel_nr)
-                L_s = L_s1 + L_s2  # The total scattered light
-
-
-
-        else:
-            L_s1 = 0
-            L_s2 = 0
-            L_s = L_s1 + L_s2
-
-        #poly_dir_1 = p1 * (theta_w_dot - theta_s1) ** 2 + p2
-        #poly_dir_2 = p1 * (theta_w_dot + theta_s1) ** 2 + p2
-
-        #L_s1 = I_0 * int_1 * b_b * poly_dir_1
-        #L_s2 = I_0 * int_2 * b_b * poly_dir_2
-
-
-
-        L_d = L_w - L_s # The direct light
-
-        #import matplotlib.pyplot as plt
-
-        L_r = L_d * np.exp(k * R_c) # Backwards attenuation
-        #plt.hist(R_c, 50)
-        #plt.show()
-        rho = np.pi * L_r / E_i
-
-        #print(np.sum(np.isnan(rho)))
-        #print(np.sum(np.isinf(rho)))
-        return rho
-
-    def forward_model_simple(self, id, is_skogn):
-        """This forward model propagates light for a set of Param. The error is evaluated in digital counts"""
-        ## IOP params
-        G = self.Param.G
-        X = self.Param.X
-        Y = self.Param.Y
-        # B
-
-        ## Light source params
-        I_0 = self.Param.I_0
-        sigma_l = self.Param.sigma_l
-
-        ## Immersion factor params
-        alpha = self.Param.alpha
-
-
-        if id == 1:
-            # Measurements
-            L_air = self.Meas.rad1
-
-            # Variables
-            wlen = self.Var.bands1
-            pos_seabed = self.Var.points1
-            norm_vec = self.Var.normals1
-            theta_w_dot = self.Var.angles1
-            pixel_nr = self.Var.pixel_nr1
-            RF = self.Var.RF1
-            t_exp = self.Var.t_exp1
-        elif id == 2:
-            # Measurements
-            L_air = self.Meas.rad2
-            # Variables
-            wlen = self.Var.bands2
-            pos_seabed = self.Var.points2
-            norm_vec = self.Var.normals2
-            theta_w_dot = self.Var.angles2
-            pixel_nr = self.Var.pixel_nr2
-            RF = self.Var.RF2
-            t_exp = self.Var.t_exp2
-
-
-        # Constants
-        a_ph = 0
-        a_w = self.Const.a_w
-        b_bw = self.Const.b_w
-        S = self.Const.S
-        dir_s10 = self.Const.dir_s1
-        dir_s20 = self.Const.dir_s2
-        pos_s1 = self.Const.pos_s1
-        pos_s2 = self.Const.pos_s2
-
-        n_w = self.Const.n_w.reshape((1, -1))
-        n_g = self.Const.n_g.reshape((1, -1))
-        #P_0 = self.Const.P_0 # Defines total Spectral flux in air
-        I_hat = self.Const.I_hat
-        rho_gt = self.Const.refl_gt.reshape((1, -1))
-
-        # IOP definitions from Lee
-        a_g = G*np.exp(-S*(wlen - 440))
-
-        a = a_w + a_ph + a_g
-
-        b_bp_dot = X*(400/wlen)**Y
-
-        b_b = b_bw + b_bp_dot # eq 18
-
-        k = (a + b_b).reshape((1, -1))
-
-
-        # Vector from source to bottom
-        dir_s1 = pos_seabed - pos_s1
-        dir_s2 = pos_seabed - pos_s2
-        # Length of those
-        R_s1 = np.linalg.norm(dir_s1, axis = 1).reshape((-1, 1))
-        R_s2 = np.linalg.norm(dir_s2, axis = 1).reshape((-1, 1))
-
-
-        import matplotlib.pyplot as plt
-
-
-        # Length of camera-bottom vector
-        R_c = np.linalg.norm(pos_seabed, axis = 1).reshape((-1, 1))
-
-        # Returns an n by k vector where k are the spectral
-        BP1_norm, BP1 = beam_pattern(dir_s0=dir_s10, dir = dir_s1, sigma= sigma_l, I_0 = I_0, I_hat = I_hat)
-        BP2_norm, BP2 = beam_pattern(dir_s0=dir_s20, dir = dir_s2, sigma=sigma_l, I_0=I_0, I_hat = I_hat)
-
-        # Returns an n by 1 vector of cosines
-        gamma_s1 = compute_gamma(dir = dir_s1, normals = norm_vec)
-        gamma_s2 = compute_gamma(dir=dir_s2, normals = norm_vec)
-
-        # Simple computation of incident light
-        E_i1 = BP1 * np.cos(gamma_s1) * np.exp(-k * R_s1) / (R_s1 ** 2)
-        E_i2 = BP2 * np.cos(gamma_s2) * np.exp(-k * R_s2) / (R_s2 ** 2)
-
-
-
-
-
-
-        if is_skogn == False:
-            E_i = E_i1 + E_i2
-        else:
-            E_i = E_i2
-
-
-
-        # Calculate reflected light:
-        L_r = (rho_gt/np.pi)*E_i
-
-        L_d = L_r*np.exp(-k*R_c)
-
-        # Compute backscatter
-        include_backscatter = False
-        if include_backscatter:
-            L_s1 = compute_scattering_integral(k, R_s1)
-            L_s2 = compute_scattering_integral(k, R_s2)
-        else:
-            L_s1 = 0
-            L_s2 = 0
-
-        L_s = L_s1 + L_s2
-
-        L_w = L_d + L_s
-
-        # Calculate from measurement to seafloor
-        theta_w = theta_w_dot - alpha  # Intersection angle with respect to glass
-
-        I_f = immersion_factor(theta_w=theta_w, n_w=n_w, n_g=n_g, pixel_nr=pixel_nr)
-
-        L_air_est = np.einsum('ij,ij -> ij', L_w, 1/I_f)
-
-        rad_2_DC = radiance_conversion(RF = RF, t_exp = t_exp, pixel_nr = pixel_nr)
-
-        DC_air_est = np.einsum('ij,ij -> ij', L_air_est, rad_2_DC)
-
-        DC_air_meas = np.einsum('ij,ij -> ij', L_air, rad_2_DC)
-
-        DC_diff = DC_air_meas - DC_air_est
-
-        return DC_diff
-    #    # The measurement is L_a meaning radiance in air
-#
-#
-    #    L_m = L_plus*I_f
-#
-
-
+
+
+
+
+from collections import namedtuple
+
+import numpy as np
+import pandas as pd
+from scipy.interpolate import interp1d
+from scipy.special import expi
+from scipy.special import erf
+from scipy.special import erfi
+from scipy.optimize import fsolve
+import matplotlib.pyplot as plt
+
+def fresnel(theta_i, n_i, n_t, is_transmittance, method):
+    # This is used for computing the transmittance at the interfaces
+    # First Snells:
+    if method == 1:
+        theta_t = np.arcsin((n_i / n_t)*np.sin(theta_i))
+
+        c_i = np.cos(theta_i)
+        c_t = np.cos(theta_t)
+
+        R_s = np.abs((n_i*c_i - n_t*c_t)/(n_i*c_i + n_t*c_t))**2
+
+        R_p = np.abs((n_i*c_t - n_t*c_i)/(n_i*c_t + n_t*c_i))**2
+
+        # Then snells:
+        R_F = 0.5*(R_s + R_p)
+
+
+    elif method == 2:
+        theta_t = np.arcsin((n_i / n_t) * np.sin(theta_i))
+
+        r1 = (np.sin(theta_i - theta_t)/np.sin(theta_i + theta_t))**2
+        r2 = (np.tan(theta_i - theta_t) / np.tan(theta_i + theta_t)) ** 2
+
+        R_F = 0.5 * (r1 + r2)
+    if is_transmittance:
+        return 1 - R_F
+    else:
+        return R_F
+
+
+
+
+def solid_angle_ratio(theta_w, n_w):
+    """Computes the in-air angle corresponding to an in-water angle using Snell's law"""
+    n_a = 1 # Approximate n_a = 1
+    theta_a = np.arcsin((n_w / n_a) * np.sin(theta_w)) # Snells law
+    return theta_a
+
+def immersion_factor(theta_w, n_w, n_g, pixel_nr):
+    """Calculates the immersion factor for imager with planar glass port in underwater hyperspectral imaging"""
+    n_a = 1
+
+    theta_a = np.arcsin((n_w / n_a) * np.sin(theta_w))
+
+    t_ag = fresnel(theta_i=theta_a, n_i = n_a, n_t = n_g, is_transmittance=1, method=1)
+
+    t_wg = fresnel(theta_i=theta_w, n_i=n_w, n_t=n_g, is_transmittance=1, method=1)
+
+    I_f_LU = ((n_w**2)/(n_a**2) ) * (t_ag/t_wg)
+
+    I_f = I_f_LU[pixel_nr.reshape(-1), :]
+
+    return I_f
+
+
+
+def radiance_conversion(RF, t_exp, pixel_nr):
+
+    rad_2_DN_LU = RF*t_exp
+
+    rad_2_DN = rad_2_DN_LU[pixel_nr.reshape(-1)] # Evaluate for relevant pixels
+    return rad_2_DN
+
+
+
+def beam_pattern(dir_s0, dir, sigma, I_0, I_hat):
+    n = dir.shape[0]
+    k = I_hat.shape[0]
+    # A gaussian beam pattern
+    dot_prod = np.dot(dir_s0, np.transpose(dir))
+
+    len_vec = np.linalg.norm(dir_s0)*np.linalg.norm(dir, axis = 1)
+
+    theta_si = np.arccos(dot_prod/len_vec)
+
+
+
+    z = (theta_si)/sigma
+
+    Intensity = I_0*np.exp(-0.5*z**2)
+
+    Intensity_Spectral = np.multiply(Intensity.reshape((-1, 1)), I_hat.reshape((1, -1)))
+
+    return Intensity/I_0, Intensity_Spectral
+
+def compute_gamma(dir, normals):
+    """Compute the angle between a normal vector and an incoming ray"""
+    dot_prod = np.einsum('ij, ij -> i', normals, -dir)
+    len_vec = np.linalg.norm(dir, axis = 1) * np.linalg.norm(normals, axis = 1)
+    gamma = np.arccos(dot_prod/len_vec)
+    return gamma.reshape((-1, 1))
+
+def compute_n_g(wlen):
+    n_g = 1.4424 + (7.1661/(wlen - 144.170))
+    return n_g
+
+def compute_n_w(wlen, method):
+    if method == 1:
+        n_w = 1.325147 + (6.6096/(wlen - 137.1924))
+    elif method == 2:
+        T = 10
+        a = -0.000001501562500
+        b = 0.000000107084865
+        c = -0.000042759374989
+        d = -0.000160475520686
+        e = 1.398067112092424
+        # Function of Slocum
+
+        n_w = a * T ** 2 + b * wlen ** 2 + c * T + d * wlen + e
+
+    return n_w
+
+def compute_scattering_integral(k, x):
+
+    Ei = expi(x = -2*x*k)
+
+    integral = -(2*k*x*Ei + np.exp(-k*x)) / x
+
+    return integral
+
+def compute_backscatter(B_p, b, b_w, b_p, d_pix, pos_seabed, p_si, dir_s0, sigma_l, I_0, I_hat, k, pixel_nr):
+    # Step 1 create a lookup table for pixelnumber and perp distance
+    z_res = 0.05
+
+    z_max = pos_seabed[:, 2].max()
+
+    # Partition
+    z = (np.arange(0, np.ceil(z_max/z_res) + 1)*z_res).reshape((-1, 1, 1))
+
+    r_si_b = z * d_pix - p_si # t by m by 3
+
+    l_si_b = np.linalg.norm(r_si_b, axis =2).reshape((r_si_b.shape[0], r_si_b.shape[1], 1)) # t by m by 1 or something
+
+    r_b_h = -z*d_pix # t by m by 3
+
+    l_b_h = np.linalg.norm(r_b_h, axis=2).reshape((r_si_b.shape[0], r_si_b.shape[1], 1))  # t by m by 1 or something
+
+    BP_norm, BP = beam_pattern(dir_s0=dir_s0, dir=r_si_b.reshape((-1, 3)), sigma=sigma_l, I_0=I_0, I_hat=I_hat).reshape((r_si_b.shape[0], r_si_b.shape[1], I_hat.shape[0]))
+
+    E_i = BP*(1/(l_si_b**2))*np.exp(-k*l_si_b) # Values of incident irradiance for all directions and all perpendicular
+
+
+    # distances t by m by k. Part of the integrand
+
+    # Compute psi for all t by m cells. Check that angles are on the right side of 90 deg
+
+    dot_prod = np.einsum('jk, ijk -> ij', d_pix, r_si_b)
+    len_vec = np.linalg.norm(d_pix, axis=1) * np.linalg.norm(r_si_b, axis=2)
+    psi = np.pi - np.arccos(dot_prod / len_vec)
+
+    beta_p_interp = fournier_forand(B_p)  # Assumed constant backscatter fraction across wl. Is a log-log interpolator
+
+    beta_p = np.exp( beta_p_interp(np.log(psi)) ).reshape((r_si_b.shape[0], r_si_b.shape[1], 1)) # Due to the interpolation in log-log domain. t by m
+
+    beta_w = compute_beta_w(psi).reshape((r_si_b.shape[0], r_si_b.shape[1], 1)) # t by m
+
+    beta_tot = (1/b)*(b_p*beta_p + b_w*beta_w) # t by m by k
+
+    integrand = E_i*beta_tot*np.exp(-k*l_b_h) # t by m by k
+
+    integral = np.cumsum(integrand, axis = 0)*z_res # Summing along the z axis weighted by z_res. Should return a t by m by k.
+
+
+
+    L_b_LU = b*integral # Should return a t by m by k.
+
+    # Can compute row of a given measurement by:
+    rows = np.round(pos_seabed[:, 2]/z_res).astype(np.int64).reshape(-1)
+    cols = pixel_nr.reshape(-1)
+
+    L_b = L_b_LU[rows, cols, :] # Returns the appropriate spectra n by k
+
+    #print(stop - start)
+
+    return L_b
+
+
+
+
+
+
+
+
+
+def compute_light_source_integral(sigma):
+    """Computes the relation between spectral radiant flux P [W] and peak intensity I_0 [W/sr] for a directionally gaussian beam
+    with sigma standard decviation"""
+    constant = np.exp(-0.5 * sigma ** 2) * sigma
+
+    term1 = -0.626657j * erf(0 + 0.707107j * sigma)
+    term2 = 0.626657j * erf(1.11072 / sigma + 0.707107j * sigma)
+    term3 = -0.626657 * erfi((0.707107 * (sigma ** 2 + 1.5708j)) / sigma)
+    term4 = 0.626657 * erfi(0.707107 * sigma + 0j)
+
+    return np.real(constant * (term1 + term2 + term3 + term4))*2*np.pi
+
+def fournier_forand(B_p):
+    """Calculates the phase function values for a given backscatter fraction"""
+
+    # Partition data into equal 100 bins from 10 degrees to 100:
+    logPsi = np.linspace(np.log(10*np.pi/180), np.log(180*np.pi/180), 100)
+    psi = np.exp(logPsi)
+    # Convert B_p to FF parameters
+    mu, n = compute_FF_params(B_p)
+    #
+    nu = (3 - mu) / 2
+
+    delta = (4 * (np.sin(psi / 2)) ** 2) / (3 * (n - 1) ** 2) # Correct, Mobley 2002 eq 2
+
+    delta_180 = 4 / (3 * (n - 1) ** 2)
+
+    beta_ff_t1 = 1 / (4 * np.pi * ((1 - delta) ** 2) * (delta ** nu))  # Coeff 1, correct
+
+    beta_ff_t2 = nu * (1 - delta) - (1 - delta ** nu) # Correct
+
+    beta_ff_t3 = delta * (1 - delta ** nu) - nu * (1 - delta) # *Correct
+
+    beta_ff_t4 = 1 / (np.sin(psi / 2) ** 2) # Correct
+
+    beta_ff_t5 = (1 - delta_180 ** nu) / (16 * np.pi * (delta_180 - 1) * delta_180 ** nu)
+
+    beta_ff_t6 = 3 * np.cos(psi) ** 2 - 1
+
+    beta_ff = beta_ff_t1 * (beta_ff_t2 + beta_ff_t3 * beta_ff_t4) \
+              + beta_ff_t5 * beta_ff_t6  ## Formula t1*(t2+t3*t4) + t5*t6
+
+    # Instantiate an interpolation object that describes the function
+    beta_ff_interp = interp1d(x = logPsi, y = np.log(beta_ff), kind = 'cubic', fill_value='extrapolate')
+
+    return beta_ff_interp
+
+def compute_FF_params(B_p):
+    mu_0 = 4 # Midpoint between max and min allowed values
+    mu = fsolve(eq_backscatter_param, mu_0, args = (B_p,))
+    n = 1.01 + 0.1542*(mu-3) # Eq 621, p 202 ocean optics
+    return mu, n
+
+    #
+
+def eq_backscatter_param(mu, B_p_true):
+    n = 1.01 + 0.1542*(mu-3) # Eq 621, p 202 ocean optics
+    nu = (3-mu)/2 # eq 2 mobley 2002
+
+    psi_90 = np.pi/2
+
+    delta_90 = (4/( 3*(n-1)**2 ))*np.sin(psi_90/2)**2  # eq 2 mobley 2002
+
+    num = (1 - delta_90**(nu+1) - 0.5*(1 - delta_90**nu))
+    den = (1 - delta_90)*delta_90**nu
+
+    B_p = 1 - num/den
+
+    return B_p_true - B_p
+
+
+
+def compute_beta_w(psi):
+    """The scattering phase function of pure water"""
+    # Psi is an array of scattering angles
+    # Analytical Formula from Ocean Optics p. 180
+    return 0.0608*(1 + 0.925*(np.cos(psi))**2)
+
+
+
+
+class Radiometry():
+    def __init__(self, config, data1, data2):
+        # Read in necessary information. i.e. water absorption and water scattering coefs
+        path_iop_water = 'C:/Users/haavasl/PycharmProjects/newGit/TautraReflectanceTools/Misc/iop_pure_water.txt'
+        df_light = pd.read_csv('C:/Users/haavasl/PycharmProjects/newGit/TautraReflectanceTools/Misc/DataMultiSeaLite.txt',
+                         header=None)
+
+        #df_light = pd.read_csv(
+        #    'C:/Users/haavasl/PycharmProjects/newGit/TautraReflectanceTools/Misc/Multi_SeaLite_spectrum.csv',
+        #    header=0)
+
+        df_iop = pd.read_csv(path_iop_water, header=9, sep=',') # Should be interpolated
+
+        df_coral = pd.read_csv(
+            'C:/Users\haavasl\PycharmProjects/newGit\TautraReflectanceTools\Misc\Coral_spectra_lab.csv', sep=';')
+
+        df_refl_plaque = pd.read_csv('C:/Users\haavasl\PycharmProjects/newGit\TautraReflectanceTools\Misc/reflectance_plaque.csv')
+
+        interpol_coral = interp1d(df_coral.iloc[:, 0].astype(np.float64),
+                                np.transpose(df_coral.iloc[:, 2:4].astype(np.float64)), fill_value='extrapolate')
+        interpol_iop = interp1d(df_iop.iloc[:, 0].astype(np.float64), np.transpose(df_iop.iloc[:, 1:3].astype(np.float64)))
+        interpol_light = interp1d(df_light.iloc[:, 0], np.transpose(df_light.iloc[:, 1]), fill_value='extrapolate')
+
+        interpol_refl = interp1d(df_refl_plaque.iloc[:, 0], np.transpose(df_refl_plaque.iloc[:, 1]))
+
+        refl_gt = interpol_refl(data1.bands)
+
+        I_hat = interpol_light(data1.bands) # Total spectral radiant flux
+        a_w, b_w = interpol_iop(data1.bands)
+        s1, s2 = interpol_coral(data1.bands)
+        refl_gt_coral = 0.5*(s1 + s2) # Mean of measurements
+
+        n_w = compute_n_w(wlen = data1.bands, method = 2)
+        n_g = compute_n_g(wlen = data1.bands)
+
+        # data contains RadData(rad = rad_2, points = points_local_2, normals=normals_local_2, pixel_nr=pixel_2, bands=bands_2, angles)
+
+        Var = namedtuple('Var', ['points1', 'normals1', 'pixel_nr1', 'bands1', 'angles1','RF1','t_exp1', 'points2', 'normals2', 'pixel_nr2', 'bands2', 'angles2', 'RF2', 't_exp2'])
+
+        self.Var =  Var(points1 = data1.points, normals1=data1.normals, pixel_nr1=data1.pixel_nr, bands1=data1.bands, angles1=data1.angles, RF1 = data1.RF, t_exp1 = data1.t_exp,
+                         points2 = data2.points, normals2=data2.normals, pixel_nr2=data2.pixel_nr, bands2=data2.bands, angles2=data2.angles, RF2 = data2.RF, t_exp2 = data2.t_exp)
+
+
+        # Structure the data in 1) constants, 2) measurements y, 3) variables x and 4) parameters beta
+        Meas = namedtuple('Meas', ['rad1', 'rad2'])
+        self.Meas = Meas(rad1 = data1.rad, rad2=data2.rad)
+
+
+
+        Const = namedtuple('Const', ['S', 'a_w', 'b_w', 'n_g', 'n_w', 'dir_s1', 'dir_s2', 'pos_s1', 'pos_s2', 'I_hat', 'refl_gt', 'refl_gt_coral'])
+        self.Const = Const(S = 0.015, a_w = a_w, b_w = b_w, n_g = n_g, n_w=n_w, dir_s1=np.array([0,0,1]), dir_s2=np.array([0,0,1]),
+                           pos_s1 = np.array([0.35, 0, 0]), pos_s2 = np.array([-0.35, 0, 0]), I_hat = I_hat, refl_gt= refl_gt, refl_gt_coral = refl_gt_coral)
+
+
+        Param = namedtuple('Param', ['G', 'X', 'Y', 'B_p', 'alpha', 'I_0', 'sigma_l', 'k_l'])
+        self.Param = Param(G = 0.1, X = 0.1, Y = 1, B_p=0.01, alpha = 0, I_0 = 1, sigma_l = 1, k_l = 0)
+    def run_forward_model(self, is_skogn, model = 'forward'):
+        #print('This function is yet to be made')
+        if model == 'two way':
+            self.refl_1 = self.two_way_model_simple(id = 1, is_skogn = is_skogn)
+            self.refl_2 = self.two_way_model_simple(id = 2, is_skogn = is_skogn)
+        if model == 'forward':
+            self.diff_dc1 = self.forward_model_simple(id=1, is_skogn=is_skogn)
+            self.diff_dc2 = self.forward_model_simple(id=2, is_skogn=is_skogn)
+
+
+
+            # Could also propagate the uncertainty into the model by perturbing
+
+
+    def set_parameters(self, G, X, Y, B_p, alpha, I_0, sigma_l, k_l):
+        #self.Param = Param(G=0.1, X=0.1, Y=1, alpha=0, I_0=1, sigma_l=1)
+        Param = namedtuple('Param', ['G', 'X', 'Y', 'B_p', 'alpha', 'I_0', 'sigma_l', 'k_l'])
+        self.Param = Param(G=G, X=X, Y=Y, B_p = B_p, alpha=alpha, I_0=I_0, sigma_l=sigma_l, k_l = k_l)
+
+
+
+
+
+    def two_way_model_simple(self, id, is_skogn):
+        # The formward model computes
+        # Parameters
+        G = self.Param.G
+        X = self.Param.X
+        Y = self.Param.Y
+        B_p = self.Param.B_p
+
+
+        I_0 = self.Param.I_0
+        sigma_l = self.Param.sigma_l
+        alpha = self.Param.alpha
+        #B_inf1 = self.Param.B_inf
+        #B_inf2 = self.Param.B_inf
+        #p1  = self.Param.p1
+        #p2 = self.Param.p2
+        #theta_s1 = self.Param.theta_s1
+
+
+        if id == 1:
+            # Measurements
+            L_air = self.Meas.rad1
+            # Variables
+            wlen = self.Var.bands1
+            pos_seabed = self.Var.points1
+            norm_vec = self.Var.normals1
+            theta_w_dot = self.Var.angles1
+            pixel_nr = self.Var.pixel_nr1
+        elif id == 2:
+            # Measurements
+            L_air = self.Meas.rad2
+            # Variables
+            wlen = self.Var.bands2
+            pos_seabed = self.Var.points2
+            norm_vec = self.Var.normals2
+            theta_w_dot = self.Var.angles2
+            pixel_nr = self.Var.pixel_nr2
+
+
+        # Constants
+        a_ph = 0
+        a_w = self.Const.a_w
+        b_w = self.Const.b_w
+        S = self.Const.S
+        dir_s10 = self.Const.dir_s1
+        dir_s20 = self.Const.dir_s2
+        pos_s1 = self.Const.pos_s1
+        pos_s2 = self.Const.pos_s2
+        n_w = self.Const.n_w.reshape((1, -1))
+        n_g = self.Const.n_g.reshape((1, -1))
+
+
+        I_hat_non_scaled = self.Const.I_hat
+
+
+        k_scale = self.Param.k_l
+
+        I_hat = I_hat_non_scaled * (1 +  k_scale*(wlen - wlen[100]))
+
+
+
+
+
+        # Eq. 9a)-9f)
+        b_bw = 0.5 * b_w #Water is isotrophic
+        a_g = G*np.exp(-S*(wlen - 440))
+        b_bp = X * (400 / wlen) ** Y
+        b_p = b_bp/B_p
+        a = a_w + a_ph + a_g
+        b = b_w + b_p
+
+        b_b = b_bw + b_bp
+
+        k = (a + b_b).reshape((1, -1))
+
+        import matplotlib.pyplot as plt
+
+        #plt.show()
+#
+        #plt.plot(wlen, I_hat*I_0)
+        #plt.show()
+        # Vector from source to bottom
+        dir_s1 = pos_seabed - pos_s1
+        dir_s2 = pos_seabed - pos_s2
+        # Length of those
+        R_s1 = np.linalg.norm(dir_s1, axis = 1).reshape((-1, 1))
+        R_s2 = np.linalg.norm(dir_s2, axis = 1).reshape((-1, 1))
+        # Length of camera-bottom vector
+        R_c = np.linalg.norm(pos_seabed, axis = 1).reshape((-1, 1))
+
+        # Returns an n by k vector where k are the spectral
+        BP1_norm, BP1 = beam_pattern(dir_s0=dir_s10, dir = dir_s1, sigma= sigma_l, I_0 = I_0, I_hat = I_hat)
+        BP2_norm, BP2 = beam_pattern(dir_s0=dir_s20, dir = dir_s2, sigma=sigma_l, I_0=I_0, I_hat = I_hat)
+
+        # Returns an n by 1 vector of cosines
+        gamma_s1 = compute_gamma(dir = dir_s1, normals = norm_vec)
+        gamma_s2 = compute_gamma(dir=dir_s2, normals = norm_vec)
+
+        if id == 1:
+            self.cos_gamma_s1_t1 = np.cos(gamma_s1)
+            self.cos_gamma_s2_t1 = np.cos(gamma_s2)
+            self.BP1_norm_t1 = BP1_norm
+            self.BP2_norm_t1 = BP2_norm
+            self.R_s1_t1 = R_s1
+            self.R_s2_t1 = R_s2
+
+        elif id == 2:
+            # Measurements
+            self.cos_gamma_s1_t2 = np.cos(gamma_s1)
+            self.cos_gamma_s2_t2 = np.cos(gamma_s2)
+            self.BP1_norm_t2 = BP1_norm
+            self.BP2_norm_t2 = BP2_norm
+            self.R_s1_t2 = R_s1
+            self.R_s2_t2 = R_s2
+
+        # Simple computation of incident light
+        E_i1 = BP1 * np.cos(gamma_s1) * np.exp(-k * R_s1) / (R_s1 ** 2)
+        E_i2 = BP2 * np.cos(gamma_s2) * np.exp(-k * R_s2) / (R_s2 ** 2)
+
+
+
+
+        import matplotlib.pyplot as plt
+
+
+        if is_skogn == False:
+            E_i = E_i1 + E_i2
+        else:
+            E_i = E_i1 # Only this light source that is illuminating the scene
+
+        # Calculate from measurement to seafloor
+        theta_w = theta_w_dot - alpha # Intersection angle with respect to glass
+
+        I_f = immersion_factor(theta_w=theta_w, n_w = n_w, n_g = n_g, pixel_nr = pixel_nr)
+
+        L_w = np.einsum('ij,ij -> ij', L_air, I_f)
+
+        #if id == 2:
+        #    from scipy.ndimage import gaussian_filter1d
+        #    plt.hist(L_air.reshape(-1), 100)
+        #    plt.show()
+
+        # Compute backscatter
+        include_backscatter = False
+        if include_backscatter:
+            x_pix = np.tan(theta_w_dot).reshape((-1, 1))
+            y_pix = np.zeros(x_pix.shape)
+            z_pix = np.ones(x_pix.shape)
+            d_pix = np.concatenate((x_pix, y_pix, z_pix), axis = 1)
+            k_bands = k.shape[1]
+
+            if is_skogn:
+                L_s1 = compute_backscatter(B_p=B_p, b=b.reshape((1, 1, k_bands)), b_w=b_w.reshape((1, 1, k_bands)),
+                                           b_p=b_p.reshape((1, 1, k_bands)), d_pix=d_pix, pos_seabed=pos_seabed,
+                                           p_si=pos_s1, dir_s0=dir_s10, sigma_l=sigma_l,
+                                           I_0=I_0, I_hat=I_hat, k=k.reshape((1, 1, k_bands)), pixel_nr=pixel_nr)
+                L_s = L_s1# The total scattered light
+            else:
+
+                L_s1 = compute_backscatter(B_p = B_p, b = b.reshape((1, 1, k_bands)), b_w = b_w.reshape((1, 1, k_bands)),
+                                           b_p = b_p.reshape((1, 1, k_bands)), d_pix = d_pix, pos_seabed = pos_seabed,
+                                           p_si = pos_s1, dir_s0 = dir_s10, sigma_l = sigma_l,
+                                           I_0 = I_0, I_hat = I_hat, k= k.reshape((1, 1, k_bands)), pixel_nr = pixel_nr)
+
+                L_s2 = compute_backscatter(B_p=B_p, b=b.reshape((1, 1, k_bands)), b_w=b_w.reshape((1, 1, k_bands)),
+                                           b_p=b_p.reshape((1, 1, k_bands)), d_pix=d_pix, pos_seabed=pos_seabed,
+                                           p_si=pos_s2, dir_s0=dir_s20, sigma_l=sigma_l,
+                                           I_0=I_0, I_hat=I_hat, k=k.reshape((1, 1, k_bands)), pixel_nr=pixel_nr)
+                L_s = L_s1 + L_s2  # The total scattered light
+
+
+
+        else:
+            L_s1 = 0
+            L_s2 = 0
+            L_s = L_s1 + L_s2
+
+        #poly_dir_1 = p1 * (theta_w_dot - theta_s1) ** 2 + p2
+        #poly_dir_2 = p1 * (theta_w_dot + theta_s1) ** 2 + p2
+
+        #L_s1 = I_0 * int_1 * b_b * poly_dir_1
+        #L_s2 = I_0 * int_2 * b_b * poly_dir_2
+
+
+
+        L_d = L_w - L_s # The direct light
+
+        #import matplotlib.pyplot as plt
+
+        L_r = L_d * np.exp(k * R_c) # Backwards attenuation
+        #plt.hist(R_c, 50)
+        #plt.show()
+        rho = np.pi * L_r / E_i
+
+        #print(np.sum(np.isnan(rho)))
+        #print(np.sum(np.isinf(rho)))
+        return rho
+
+    def forward_model_simple(self, id, is_skogn):
+        """This forward model propagates light for a set of Param. The error is evaluated in digital counts"""
+        ## IOP params
+        G = self.Param.G
+        X = self.Param.X
+        Y = self.Param.Y
+        # B
+
+        ## Light source params
+        I_0 = self.Param.I_0
+        sigma_l = self.Param.sigma_l
+
+        ## Immersion factor params
+        alpha = self.Param.alpha
+
+
+        if id == 1:
+            # Measurements
+            L_air = self.Meas.rad1
+
+            # Variables
+            wlen = self.Var.bands1
+            pos_seabed = self.Var.points1
+            norm_vec = self.Var.normals1
+            theta_w_dot = self.Var.angles1
+            pixel_nr = self.Var.pixel_nr1
+            RF = self.Var.RF1
+            t_exp = self.Var.t_exp1
+        elif id == 2:
+            # Measurements
+            L_air = self.Meas.rad2
+            # Variables
+            wlen = self.Var.bands2
+            pos_seabed = self.Var.points2
+            norm_vec = self.Var.normals2
+            theta_w_dot = self.Var.angles2
+            pixel_nr = self.Var.pixel_nr2
+            RF = self.Var.RF2
+            t_exp = self.Var.t_exp2
+
+
+        # Constants
+        a_ph = 0
+        a_w = self.Const.a_w
+        b_bw = self.Const.b_w
+        S = self.Const.S
+        dir_s10 = self.Const.dir_s1
+        dir_s20 = self.Const.dir_s2
+        pos_s1 = self.Const.pos_s1
+        pos_s2 = self.Const.pos_s2
+
+        n_w = self.Const.n_w.reshape((1, -1))
+        n_g = self.Const.n_g.reshape((1, -1))
+        #P_0 = self.Const.P_0 # Defines total Spectral flux in air
+        I_hat = self.Const.I_hat
+        rho_gt = self.Const.refl_gt.reshape((1, -1))
+
+        # IOP definitions from Lee
+        a_g = G*np.exp(-S*(wlen - 440))
+
+        a = a_w + a_ph + a_g
+
+        b_bp_dot = X*(400/wlen)**Y
+
+        b_b = b_bw + b_bp_dot # eq 18
+
+        k = (a + b_b).reshape((1, -1))
+
+
+        # Vector from source to bottom
+        dir_s1 = pos_seabed - pos_s1
+        dir_s2 = pos_seabed - pos_s2
+        # Length of those
+        R_s1 = np.linalg.norm(dir_s1, axis = 1).reshape((-1, 1))
+        R_s2 = np.linalg.norm(dir_s2, axis = 1).reshape((-1, 1))
+
+
+        import matplotlib.pyplot as plt
+
+
+        # Length of camera-bottom vector
+        R_c = np.linalg.norm(pos_seabed, axis = 1).reshape((-1, 1))
+
+        # Returns an n by k vector where k are the spectral
+        BP1_norm, BP1 = beam_pattern(dir_s0=dir_s10, dir = dir_s1, sigma= sigma_l, I_0 = I_0, I_hat = I_hat)
+        BP2_norm, BP2 = beam_pattern(dir_s0=dir_s20, dir = dir_s2, sigma=sigma_l, I_0=I_0, I_hat = I_hat)
+
+        # Returns an n by 1 vector of cosines
+        gamma_s1 = compute_gamma(dir = dir_s1, normals = norm_vec)
+        gamma_s2 = compute_gamma(dir=dir_s2, normals = norm_vec)
+
+        # Simple computation of incident light
+        E_i1 = BP1 * np.cos(gamma_s1) * np.exp(-k * R_s1) / (R_s1 ** 2)
+        E_i2 = BP2 * np.cos(gamma_s2) * np.exp(-k * R_s2) / (R_s2 ** 2)
+
+
+
+
+
+
+        if is_skogn == False:
+            E_i = E_i1 + E_i2
+        else:
+            E_i = E_i2
+
+
+
+        # Calculate reflected light:
+        L_r = (rho_gt/np.pi)*E_i
+
+        L_d = L_r*np.exp(-k*R_c)
+
+        # Compute backscatter
+        include_backscatter = False
+        if include_backscatter:
+            L_s1 = compute_scattering_integral(k, R_s1)
+            L_s2 = compute_scattering_integral(k, R_s2)
+        else:
+            L_s1 = 0
+            L_s2 = 0
+
+        L_s = L_s1 + L_s2
+
+        L_w = L_d + L_s
+
+        # Calculate from measurement to seafloor
+        theta_w = theta_w_dot - alpha  # Intersection angle with respect to glass
+
+        I_f = immersion_factor(theta_w=theta_w, n_w=n_w, n_g=n_g, pixel_nr=pixel_nr)
+
+        L_air_est = np.einsum('ij,ij -> ij', L_w, 1/I_f)
+
+        rad_2_DC = radiance_conversion(RF = RF, t_exp = t_exp, pixel_nr = pixel_nr)
+
+        DC_air_est = np.einsum('ij,ij -> ij', L_air_est, rad_2_DC)
+
+        DC_air_meas = np.einsum('ij,ij -> ij', L_air, rad_2_DC)
+
+        DC_diff = DC_air_meas - DC_air_est
+
+        return DC_diff
+    #    # The measurement is L_a meaning radiance in air
+#
+#
+    #    L_m = L_plus*I_f
+#
+
+
```

### Comparing `gref4hsi-0.2.1/gref4hsi/utils/specim_parsing_utils.py` & `gref4hsi-0.2.2/gref4hsi/utils/specim_parsing_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,650 +1,652 @@
-"""This script reads Specim data from default captures and reformats data to compatibility with pipeline"""
-# Python builtins
-from datetime import datetime, timedelta
-import os
-import glob
-from pathlib import Path
-
-# Third party libraries
-import numpy as np
-from pathlib import Path
-from spectral import envi
-import pandas as pd
-import h5py
-import pymap3d as pm
-from scipy.interpolate import interp1d
-from scipy.optimize import least_squares
-from scipy.spatial.transform import Rotation as RotLib
-
-# Library dependencies
-from gref4hsi.utils.geometry_utils import CalibHSI
-from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths
-
-ACTIVE_SENSOR_SPATIAL_PIXELS = 1024 # Constant for AFX10
-ACTIVE_SENSOR_SPECTRAL_PIXELS = 448 # Constant for AFX10
-
-class Specim():
-    def __init__(self, mission_path, config):
-        self.mission_path = mission_path # With slash end
-        self.config = config #
-    
-    @staticmethod
-    def fov_2_param(fov):
-        """
-        param fov: view angle of each pixel in degrees
-        returns: A dictionary of camera parameters
-        """
-        # Script for reading the FOV file and converting it to a camera model
-        def optimize_func(param, x_true, n_pix):
-
-            f = param[0]  # The focal length of the lens
-            k1 = param[1]  # The 1st Radial distortion
-            k2 = param[2]  # The 2nd Radial distortion
-            k3 = param[3]
-            c_x = param[4]
-            n_pix = x_true.size
-            #v_c = n_pix / 2 + 1
-            u = np.arange(1, n_pix + 1).reshape((-1,1))
-
-            x_norm_lin = (u - c_x) / f
-            # Distortion term if to be used
-            x_norm_nonlin = -(k1 * ((u - c_x) / 1000) ** 5 + \
-                            k2 * ((u - c_x) / 1000) ** 3 + \
-                            k3 * ((u - c_x) / 1000) ** 2) / f
-
-            
-            x_norm = x_norm_lin + x_norm_nonlin
-            diff_x = x_norm-x_true
-            return diff_x.reshape(-1)
-        
-        
-        theta_true = fov*np.pi/180
-
-        x_true = np.array(np.tan(theta_true)).reshape((-1, 1))
-
-        n_pix = x_true.size
-
-        # Total angular FOV is:
-        AFOV = np.abs(theta_true[0]) + np.abs(theta_true[-1])
-        f_0 = (n_pix/2)/(np.tan(AFOV/2))
-
-        param_0 = np.array([f_0, 0, 0, 0, 1 + n_pix/2])
-
-        res = least_squares(optimize_func, param_0, args = (x_true, n_pix), x_scale = 'jac')
-
-        param = res.x
-        f = param[0]  # The focal length of the lens
-        k1 = param[1]  # The 1st Radial distortion
-        k2 = param[2]  # The 2nd Radial distortion
-        k3 = param[3]  # The tangential distortion
-        c_x = param[4] # The 
-
-        # initialized to 0
-        rotation_x = 0
-        rotation_y = 0
-        rotation_z = 0
-        translation_x = 0
-        translation_y = 0
-        translation_z = 0
-
-        param_dict = {'rx':rotation_x,
-                      'ry':rotation_y,
-                      'rz':rotation_z,
-                      'tx':translation_x,
-                      'ty':translation_y,
-                      'tz':translation_z,
-                      'f': f,
-                      'cx': c_x,
-                      'k1': k1,
-                      'k2': k2,
-                      'k3': k3,
-                      'width': n_pix}
-        return param_dict
-
-    def read_fov_file(self, fov_file_path):
-        
-
-        
-
-        df_fov = pd.read_csv(fov_file_path, sep = ',', header = None)
-
-        fov_arr = df_fov.values[:, 1]
-
-        param_dict = Specim.fov_2_param(fov = fov_arr)
-        
-        file_name_calib = self.config['Absolute Paths']['hsi_calib_path']
-
-        CalibHSI(file_name_cal_xml=file_name_calib,
-                 mode = 'w', 
-                 param_dict = param_dict)
-
-    def read_nav_file(self, nav_file_path, date):
-        # Convert date string to datetime object
-        date_obj = datetime.strptime(date, "%Y-%m-%d")
-        # Open file for reading.
-        with open(nav_file_path, 'r') as nav_file:
-            count = 0
-            imu_data = []
-            gnss_data = []
-            sync_data = []
-            # Set to -1 to an if sentence to initialize to true
-            hsi_frame_nr_prev = -1
-            # Variable introduced to convert from cyclic HS frame counting to cumulative counts
-            restart_counts = 0
-
-            while True:
-                count += 1
-
-                # Get next line from file
-                line = nav_file.readline()
-
-                line_arr = line.split(sep = ',')
-
-                if line_arr[0] == '$PASHR':
-                    Timestamp_str = line_arr[1]
-                    sec = float(Timestamp_str[4:])
-                    minut = int(Timestamp_str[2:4])
-                    hour = int(Timestamp_str[0:2])
-
-                    # Create a timedelta object for the time
-                    time_delta = timedelta(hours=hour, minutes=minut, seconds=sec)
-
-                    # Calculate the total timedelta
-                    total_timedelta = date_obj + time_delta
-
-                    # Convert to UNIX timestamp (decimal UNIX time)
-                    unix_timestamp = (total_timedelta - datetime(1970, 1, 1)) / timedelta(seconds=1)
-
-                    TimestampAbs = unix_timestamp
-
-                    TimestampClock = date + '_' + Timestamp_str
-
-                    Yaw = float(line_arr[2]) # Heading wrt true north
-                    Roll = float(line_arr[4])
-                    Pitch = float(line_arr[5])# According to https://docs.novatel.com/OEM7/Content/SPAN_Logs/PASHR.htm
-
-
-                    sigmaRoll = float(line_arr[7])
-                    sigmaPitch = float(line_arr[8])  # According to https://docs.novatel.com/OEM7/Content/SPAN_Logs/PASHR.htm
-                    sigmaYaw = float(line_arr[9])
-
-                    #dlogr_imu.append_data(np.array([TimestampClock, TimestampAbs, Roll, Pitch, Yaw, sigmaRoll, sigmaPitch, sigmaYaw]))
-
-                    imu_data_row = {'TimestampClock':TimestampClock,
-                                     'TimestampAbs': TimestampAbs,
-                                     'Roll': Roll,
-                                     'Pitch': Pitch,
-                                     'Yaw': Yaw,
-                                     'sigmaRoll': sigmaRoll,
-                                     'sigmaPitch': sigmaPitch,
-                                     'sigmaYaw': sigmaYaw}
-                    imu_data.append(imu_data_row)
-
-                elif line_arr[0] == '$GNGGA' or line_arr[0] == '$GPGGA':
-                    Timestamp_str = line_arr[1]
-                    sec = float(Timestamp_str[4:])
-                    minut = float(Timestamp_str[2:4])
-                    hour = float(Timestamp_str[0:2])
-
-                    # Create a timedelta object for the time
-                    time_delta = timedelta(hours=hour, minutes=minut, seconds=sec)
-
-                    # Calculate the total timedelta
-                    total_timedelta = date_obj + time_delta
-
-                    # Convert to UNIX timestamp (decimal UNIX time)
-                    unix_timestamp = (total_timedelta - datetime(1970, 1, 1)) / timedelta(seconds=1)
-
-                    TimestampAbs = unix_timestamp
-
-                    TimestampClock = date + '_' + Timestamp_str
-
-                    LatDDMM_MM = float(line_arr[2]) # DDMM.mm
-                    LatInt = int(LatDDMM_MM/100)
-                    Lat = LatInt + (LatDDMM_MM - LatInt*100)/60
-
-
-                    LonDDDMM_MM = float(line_arr[4]) # DDDMM.mm
-                    LonInt = int(LonDDDMM_MM / 100)
-                    Lon = LonInt + (LonDDDMM_MM - LonInt * 100) / 60
-
-                    AltMSL = float(line_arr[9])
-                    AltGeoid = float(line_arr[11])  # According to https://docs.novatel.com/OEM7/Content/Logs/GPGGA.htm
-
-                    #dlogr_gnss.append_data(np.array([TimestampClock, TimestampAbs, Lon, Lat, AltMSL, AltGeoid]))
-                    gnss_data_row = {'TimestampClock':TimestampClock,
-                                     'TimestampAbs': TimestampAbs,
-                                     'Lon': Lon,
-                                     'Lat': Lat,
-                                     'AltMSL': AltMSL,
-                                     'AltGeoid': AltGeoid}
-                    gnss_data.append(gnss_data_row)
-                elif line_arr[0] == '$SPTSMP':
-                    """Recordings of time sync messages, tied to the hyperspectral frames"""
-                    hsi_frame_number_new = int(line_arr[2]) - 1 # Seems they start with a 1-base (like MATLAB)
-
-                    if hsi_frame_number_new < hsi_frame_nr_prev: # When frame counter resets
-                        restart_counts += (hsi_frame_nr_prev - hsi_frame_number_new) + self.metadata_obj.fps # 9950 + 50
-
-
-                    hsi_frame_number = hsi_frame_number_new
-                    hsi_frame_nr_prev = hsi_frame_number_new
-                    prev_time = TimestampAbs
-
-                    # In the file, fram counts go 1, 51, 101,... 9951, 1 ... in a cyclic manner. So to get cumulative counts we add the restart_counts
-                    sync_data_row = {'HsiFrameNum': hsi_frame_number + restart_counts,
-                                     'TimestampAbs': prev_time,
-                                     'TimestampClock': TimestampClock}
-                    sync_data.append(sync_data_row)
-
-
-
-
-                # if line is empty
-                # end of file is reached
-                if not line:
-                    break
-        
-        self.imu_data = imu_data
-        self.gnss_data = gnss_data
-        self.sync_data = sync_data
-
-"""Writer for the h5 file format using a dictionary. The user provides h5 hierarchy paths as values and keys are the names given to the attributes of the specim object.
-A similar write process could be applied to metadata."""
-def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
-    with h5py.File(h5_filename, 'w', libver='latest') as f:
-        for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
-            #print(attribute_name)
-            dset = f.create_dataset(name=h5_hierarchy_item_path, 
-                                            data = getattr(specim_object, attribute_name))            
-
-def add_byte_order_to_envi_header(header_file_path, byte_order_value):
-    """Function added to remedy lacking byte-order entry in header files of radiometric calibration data
-
-    :param header_file_path: _description_
-    :type header_file_path: _type_
-    :param byte_order_value: _description_
-    :type byte_order_value: _type_
-    """
-    # Read the existing ENVI header
-    with open(header_file_path, 'r') as f:
-        header_lines = f.readlines()
-
-    # Look for the line where you want to add "byte order"
-    for i, line in enumerate(header_lines):
-        if line.startswith('byte order'):
-            # If it already exists, update the value
-            header_lines[i] = f'byte order = {byte_order_value}\n'
-            break
-    else:
-        # If it doesn't exist, add it to the end of the header
-        header_lines.append(f'byte order = {byte_order_value}\n')
-
-    # Save the updated header
-    with open(header_file_path, 'w') as f:
-        f.writelines(header_lines)
-
-
-
-def main(config, config_specim):
-    
-    # Script that calibrates data and reforms to h5 file format.
-    dtype = config_specim.dtype_datacube
-    transect_chunk_size = config_specim.lines_per_chunk
-    cal_dir = config_specim.cal_dir
-   
-    mission_dir = config_specim.specim_raw_mission_dir
-
-    mission_name = Path(mission_dir).name
-    out_dir = config_specim.reformatted_missions_dir
-    config_file_path = os.path.join(out_dir, config_specim.config_file_name)
-
-    #prepend_data_dir_to_relative_paths(config_path=config_file_path, DATA_DIR=out_dir)
-
-    specim_object = Specim(mission_path=mission_dir, config=config)
-
-    # Patterns for searching data cube files
-    PATTERN_ENVI = '*.hdr'
-
-    # Expects the captured data to reside in capture subfolder
-    capture_dir = os.path.join(mission_dir, 'capture')
-
-    # Path for searching (avoid explicit )
-    search_path_envi = os.path.normpath(os.path.join(capture_dir, PATTERN_ENVI))
-    envi_hdr_file_path = glob.glob(search_path_envi)[0]
-
-    # Read out data
-    spectral_image_obj = envi.open(envi_hdr_file_path)
-
-    # Read all meta data from header file (currently hard coded, but could be avoided I guess)
-    class Metadata:
-        pass
-
-    metadata_obj = Metadata()
-    # Could do this in iteration, but it would need to specify type (I think)
-    metadata_obj.autodarkstartline = int(spectral_image_obj.metadata['autodarkstartline'])
-    metadata_obj.n_lines = int(spectral_image_obj.metadata['lines'])
-    metadata_obj.n_bands = int(spectral_image_obj.metadata['bands'])
-    metadata_obj.n_pix = int(spectral_image_obj.metadata['samples'])
-    metadata_obj.t_exp_ms = float(spectral_image_obj.metadata['tint'])
-    metadata_obj.fps = float(spectral_image_obj.metadata['fps'])
-    metadata_obj.description = spectral_image_obj.metadata['description']
-    metadata_obj.file_type = spectral_image_obj.metadata['file type']
-    metadata_obj.sensor_type = spectral_image_obj.metadata['sensor type']
-    metadata_obj.acquisition_date = spectral_image_obj.metadata['acquisition date']
-    metadata_obj.sensorid = spectral_image_obj.metadata['sensorid']
-    metadata_obj.interleave = spectral_image_obj.metadata['interleave']
-    metadata_obj.data_type = spectral_image_obj.metadata['data type']
-    
-    # Derived from knowledge of the sensor (sensor constants that could differ for other sensors)
-    metadata_obj.binning_spatial = int(ACTIVE_SENSOR_SPATIAL_PIXELS/metadata_obj.n_pix)
-    metadata_obj.binning_spectral = int(ACTIVE_SENSOR_SPECTRAL_PIXELS/metadata_obj.n_bands)
-
-    # Allow Specim Methods to access metadata
-    specim_object.metadata_obj = metadata_obj 
-    # -
-
-    # Based on the binning info, we can locate relevant calibration files, including 1) spectral, 2) geometric, 3) radiometric, and dark frame (from capture).
-    #
-    # We start with the spectral calibration:
-
-    # Comprehensive band info (center, fwhm) is found in "cal_dir/wlcal<spectral binning>b_fwhm.wls"
-    # Pattern follows structure
-    PATTERN_BAND_INFO = '*'+ str(metadata_obj.binning_spectral) + 'b_fwhm.wls'
-    # Linux-CLI search for file.
-    search_path_bands = os.path.normpath(os.path.join(cal_dir, PATTERN_BAND_INFO))
-    band_file_path = glob.glob(search_path_bands)[0]
-
-    # Read the file as csv (although it has no columns)
-    df_bands = pd.read_csv(band_file_path, header=None, sep = '\s+')
-    df_bands.columns = ['Wavelength_nm', 'FWHM_nm']
-
-    # Extract band data
-    specim_object.wavelengths = np.array(df_bands['Wavelength_nm'])
-    specim_object.fwhm = np.array(df_bands['FWHM_nm'])
-
-    # -
-
-    # We will here go through the loading of Specim geometric camera calibration. 
-    # The first step is to load the angular Field-of-View file (AFOV) from the manufacturer. 
-    # Then boresight angles and lever arms can be set, if relevant.
-
-    # +
-    # Pixel-directions is found in "cal_dir/FOV_****_<spatial binning>b.txt" 
-    PATTERN_FOV = 'FOV*' + '_' +  str(metadata_obj.binning_spatial) + 'b.txt'
-
-    # Search for fov file.
-    search_path_fov = os.path.normpath(os.path.join(cal_dir, PATTERN_FOV))
-    fov_file_path = glob.glob(search_path_fov)[0]
-
-    # Calculate a camera model (zero boresight) based on FOV file.
-    # Writes parameters to an *xml file specified by config
-
-    # Read fov data (one angle for each pixel)
-    df_fov = pd.read_csv(fov_file_path, header=None, sep = ',')
-
-    df_fov.columns = ['pixel_nr', 'view_angle_deg', 'Unknown']
-
-    specim_object.view_angles = np.array(df_fov['view_angle_deg'])
-    
-    # Simply converts view angles to camera parameters for a 1D line camera model
-    param_dict = Specim.fov_2_param(fov = specim_object.view_angles)
-    
-    # param_dict are the full camera model parameters, but defaults rotation matrix and translation
-
-    # User set rotation matrix
-    R_hsi_body = config_specim.rotation_matrix_hsi_to_body
-
-    r_zyx = RotLib.from_matrix(R_hsi_body).as_euler('ZYX', degrees=False)
-
-    # Euler angle representation (any other would do too)
-    param_dict['rz'] = r_zyx[0]
-    param_dict['ry'] = r_zyx[1]
-    param_dict['rx'] = r_zyx[2]
-
-    # Vector from origin of HSI to body origin, expressed in body
-    # User set
-    t_hsi_body = config_specim.translation_body_to_hsi
-    param_dict['tz'] = t_hsi_body[0]
-    param_dict['ty'] = t_hsi_body[1]
-    param_dict['tz'] = t_hsi_body[2]
-
-    camera_calib_xml_dir = config['Absolute Paths']['calib_folder']
-
-    file_name_xml = 'HSI_' + str(metadata_obj.binning_spatial) + 'b.xml'
-    xml_cal_write_path = camera_calib_xml_dir + file_name_xml
-
-    CalibHSI(file_name_cal_xml= xml_cal_write_path, 
-                    mode = 'w', 
-                    param_dict = param_dict)
-
-
-    # Set value in config file:
-    config.set('Relative Paths', 'hsi_calib_path', value = xml_cal_write_path)
-
-    
-
-    # Write the config object 
-    with open(config_file_path, 'w') as configfile:
-            config.write(configfile)
-    # -
-
-    
-
-
-    # The next step is to read in radiometric frame.
-
-    # +
-    """Extract radiometric frame from dedicated file"""
-
-    PATTERN_ENVI_CAL = '*_' +str(metadata_obj.binning_spectral) + 'x' +  str(metadata_obj.binning_spatial) + '.hdr'
-
-    search_path_envi_cal = os.path.normpath(os.path.join(cal_dir, PATTERN_ENVI_CAL))
-    ENVI_CAL_HDR_FILE_PATH = glob.glob(search_path_envi_cal)[0]
-
-    # For allowing spectral module to read
-    RAD_CAL_BYTE_ORDER = 0
-
-    add_byte_order_to_envi_header(header_file_path=ENVI_CAL_HDR_FILE_PATH, byte_order_value=RAD_CAL_BYTE_ORDER)
-
-    ENVI_CAL_IMAGE_FILE_PATH = ENVI_CAL_HDR_FILE_PATH.split('.')[0] + '.cal' # SPECTRAL does not expect this suffix by default
-
-    # For some reason, the byte order is needed
-    radiometric_image_obj = envi.open(ENVI_CAL_HDR_FILE_PATH, image = ENVI_CAL_IMAGE_FILE_PATH)
-
-    cal_n_lines = int(radiometric_image_obj.metadata['lines'])
-    cal_n_bands = int(radiometric_image_obj.metadata['bands'])
-    cal_n_pix = int(radiometric_image_obj.metadata['samples'])
-
-    # For calibration
-    radiometric_frame = radiometric_image_obj[:,:,:].reshape((cal_n_pix, cal_n_bands))
-
-    specim_object.radiometric_frame = radiometric_frame
-    # -
-
-    # The next step is to load the darkframes
-
-    # +
-    """1) Crop the hyperspectral data according to the start-stop lines. 2) Write datacube to appropriate directory"""
-    # To ensure that the plots actually do appear in this notebook:
-    # %matplotlib qt
-
-    # Establish dark frame data (at end of recording)
-    data_dark = spectral_image_obj[metadata_obj.autodarkstartline:metadata_obj.n_lines, :, :]
-    dark_frame = np.median(data_dark, axis = 0)
-
-    specim_object.dark_frame = dark_frame
-
-    # -
-
-    # The navigation data is given as messages is a *.nav file. Locate the file and parse it into a suitable format.
-
-    # +
-    # Extract the starting/stopping lines
-    START_STOP_DIR = os.path.join(mission_dir, 'start_stop_lines')
-    
-    # Allow software to function if start_stop_lines not specified
-    if not os.path.exists(START_STOP_DIR):
-        os.mkdir(START_STOP_DIR)
-        # Chunk according to chunk size
-        start_lines = np.arange(start=0,
-                                stop=metadata_obj.autodarkstartline, 
-                                step=transect_chunk_size)
-
-        stop_lines = np.arange(start=transect_chunk_size, 
-                               stop=metadata_obj.autodarkstartline + transect_chunk_size, 
-                               step=transect_chunk_size)
-        
-        stop_lines[-1] = metadata_obj.autodarkstartline # No need to georeference dark data
-
-        # Make dataframe
-        start_stop_data = {'line_start' : start_lines,
-                           'line_stop' : stop_lines}
-        
-        df_start_stop = pd.DataFrame(start_stop_data)
-
-        df_start_stop.to_csv(path_or_buf = os.path.join(START_STOP_DIR, 'start_stop_lines.txt'), sep=' ')
-
-
-
-    PATTERN_START_STOP = '*.txt'
-    
-
-    search_path_lines_start_stop = os.path.normpath(os.path.join(START_STOP_DIR, PATTERN_START_STOP))
-    LINES_START_STOP_FILE_PATH = glob.glob(search_path_lines_start_stop)[0]
-
-    df_start_stop = pd.read_csv(filepath_or_buffer=LINES_START_STOP_FILE_PATH, header=0, sep=' ')
-
-
-
-    # +
-    # Now read the *.nav file
-    NAV_PATTERN = '*.nav'
-
-    search_path_nav = os.path.normpath(os.path.join(capture_dir, NAV_PATTERN))
-    nav_file_path = glob.glob(search_path_nav)[0]
-
-    date_string = metadata_obj.acquisition_date.split(': ')[1] # yyyy-mm-dd
-    # Parse the position/orientation messages
-    specim_object.read_nav_file(nav_file_path=nav_file_path, date = date_string)
-
-
-
-    # -
-
-    # Calculate the frame timestamps from sync data
-
-    # +
-    
-
-
-    df_imu = pd.DataFrame(specim_object.imu_data)
-    df_gnss = pd.DataFrame(specim_object.gnss_data)
-    df_sync_hsi = pd.DataFrame(specim_object.sync_data)
-    
-    # Define the time stamps of HSI frames (special fix for Specim)
-    sync_frames = df_sync_hsi['HsiFrameNum']
-    sync_times = df_sync_hsi['TimestampAbs']
-    hsi_frames = np.arange(metadata_obj.autodarkstartline)
-    hsi_timestamps_total = interp1d(x = sync_frames, y = sync_times, fill_value = 'extrapolate')(x = hsi_frames)
-
-
-    # For ease, let us interpolate position data to imu time (allows one timestamp for nav data)
-    imu_time = df_imu['TimestampAbs']
-
-    # Drop the specified regular clock time (as it is not needed)
-    df_gnss = df_gnss.drop(columns=['TimestampClock'])
-
-    # Interpolate each column in GNSS data based on 'imu_time'
-    interpolated_values = {
-        column: np.interp(imu_time, df_gnss['TimestampAbs'], df_gnss[column])
-        for column in df_gnss.columns if column != 'TimestampAbs'
-    }
-
-    # Create a new DataFrame with the interpolated values
-    df_gnss_interpolated = pd.DataFrame({'time': imu_time, **interpolated_values})
-
-    # The position defined in geodetic coordinates
-    lat = np.array(df_gnss_interpolated['Lat']).reshape((-1,1))
-    lon = np.array(df_gnss_interpolated['Lon']).reshape((-1,1))
-    ellipsoid_height = np.array(df_gnss_interpolated['AltMSL'] + df_gnss_interpolated['AltGeoid']).reshape((-1,1))
-
-    # Assumes WGS-84 (default GNSS frame)
-    x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
-
-    # Lastly, calculate the roll, pitch, yaw
-    roll = np.array(df_imu['Roll']).reshape((-1,1))
-    pitch = np.array(df_imu['Pitch']).reshape((-1,1))
-    yaw = np.array(df_imu['Yaw']).reshape((-1,1))
-
-    # Roll pitch yaw are stacked in attribute eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
-    specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
-
-    # Position is stored as ECEF cartesian coordinates (mutually orthogonal axis) instead of spherioid-like lon, lat, alt
-    specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
-    specim_object.nav_timestamp = imu_time
-    specim_object.t_exp_ms = metadata_obj.t_exp_ms
-
-    # -
-
-    # Last preprocessing step is writing to h5 files. 
-    
-
-    h5_dict_write = {'eul_zyx' : config['HDF.raw_nav']['eul_zyx'],
-            'position_ecef' : config['HDF.raw_nav']['position'],
-            'nav_timestamp' : config['HDF.raw_nav']['timestamp'],
-            'radiance_cube': config['HDF.hyperspectral']['datacube'],
-            't_exp_ms': config['HDF.hyperspectral']['exposuretime'],
-            'hsi_timestamps': config['HDF.hyperspectral']['timestamp'],
-            'view_angles': config['HDF.calibration']['view_angles'],
-            'wavelengths' : config['HDF.calibration']['band2wavelength'],
-            'fwhm' : config['HDF.calibration']['fwhm'],
-            'dark_frame' : config['HDF.calibration']['darkframe'],
-            'radiometric_frame' : config['HDF.calibration']['radiometricframe']}
-
-    # Time to write all the data to a h5 file
-
-
-
-    # # Chunking the recording to user defined sizes and writing it to disk
-
-    # +
-    # Define h5 file name
-    h5_folder = config['Absolute Paths']['h5_folder']
-
-    # Each line in start_stop defines a transect
-    n_transects = df_start_stop.shape[0]
-    for transect_number in range(n_transects):
-        start_line = df_start_stop['line_start'][transect_number]
-        stop_line = df_start_stop['line_stop'][transect_number]
-
-        n_chunks = int(np.ceil((stop_line-start_line)/transect_chunk_size))
-
-        
-        for chunk_number in range(n_chunks):
-            chunk_start_idx = start_line + transect_chunk_size*chunk_number
-
-            if chunk_number == n_chunks-1:
-                chunk_stop_idx = stop_line
-            else:
-                chunk_stop_idx = chunk_start_idx + transect_chunk_size
-
-            #print(f'Chunk from line {chunk_start_idx} to line {chunk_stop_idx} is being written')
-            data_cube = spectral_image_obj[chunk_start_idx:chunk_stop_idx, :, :]
-            # Calibration equation
-            specim_object.radiance_cube = ( (data_cube - dark_frame)*radiometric_frame/(metadata_obj.t_exp_ms/1000) ).astype(dtype = dtype) # 4 Byte
-            specim_object.hsi_timestamps = hsi_timestamps_total[chunk_start_idx:chunk_stop_idx]
-
-            # Possible to name files with <PREFIX>_<time_start>_<Transect#>_<Chunk#>.h5
-            h5_filename = h5_folder + mission_name + '_transectnr_' + str(int(transect_number)) + '_chunknr_' + str(int(chunk_number)) + '.h5'
-
-            specim_object_2_h5_file(h5_filename=h5_filename, h5_tree_dict=h5_dict_write, specim_object=specim_object)
-
-
-
-
-
-
-
-
-
+"""This script reads Specim data from default captures and reformats data to compatibility with pipeline"""
+# Python builtins
+from datetime import datetime, timedelta
+import os
+import glob
+from pathlib import Path
+
+# Third party libraries
+import numpy as np
+from pathlib import Path
+from spectral import envi
+import pandas as pd
+import h5py
+import pymap3d as pm
+from scipy.interpolate import interp1d
+from scipy.optimize import least_squares
+from scipy.spatial.transform import Rotation as RotLib
+
+# Library dependencies
+from gref4hsi.utils.geometry_utils import CalibHSI
+from gref4hsi.utils.config_utils import prepend_data_dir_to_relative_paths
+
+ACTIVE_SENSOR_SPATIAL_PIXELS = 1024 # Constant for AFX10
+ACTIVE_SENSOR_SPECTRAL_PIXELS = 448 # Constant for AFX10
+
+class Specim():
+    def __init__(self, mission_path, config):
+        self.mission_path = mission_path # With slash end
+        self.config = config #
+    
+    @staticmethod
+    def fov_2_param(fov):
+        """
+        param fov: view angle of each pixel in degrees
+        returns: A dictionary of camera parameters
+        """
+        # Script for reading the FOV file and converting it to a camera model
+        def optimize_func(param, x_true, n_pix):
+
+            f = param[0]  # The focal length of the lens
+            k1 = param[1]  # The 1st Radial distortion
+            k2 = param[2]  # The 2nd Radial distortion
+            k3 = param[3]
+            c_x = param[4]
+            n_pix = x_true.size
+            #v_c = n_pix / 2 + 1
+            u = np.arange(1, n_pix + 1).reshape((-1,1))
+
+            x_norm_lin = (u - c_x) / f
+            # Distortion term if to be used
+            x_norm_nonlin = -(k1 * ((u - c_x) / 1000) ** 5 + \
+                            k2 * ((u - c_x) / 1000) ** 3 + \
+                            k3 * ((u - c_x) / 1000) ** 2) / f
+
+            
+            x_norm = x_norm_lin + x_norm_nonlin
+            diff_x = x_norm-x_true
+            return diff_x.reshape(-1)
+        
+        
+        theta_true = fov*np.pi/180
+
+        x_true = np.array(np.tan(theta_true)).reshape((-1, 1))
+
+        n_pix = x_true.size
+
+        # Total angular FOV is:
+        AFOV = np.abs(theta_true[0]) + np.abs(theta_true[-1])
+        f_0 = (n_pix/2)/(np.tan(AFOV/2))
+
+        param_0 = np.array([f_0, 0, 0, 0, 1 + n_pix/2])
+
+        res = least_squares(optimize_func, param_0, args = (x_true, n_pix), x_scale = 'jac')
+
+        param = res.x
+        f = param[0]  # The focal length of the lens
+        k1 = param[1]  # The 1st Radial distortion
+        k2 = param[2]  # The 2nd Radial distortion
+        k3 = param[3]  # The tangential distortion
+        c_x = param[4] # The 
+
+        # initialized to 0
+        rotation_x = 0
+        rotation_y = 0
+        rotation_z = 0
+        translation_x = 0
+        translation_y = 0
+        translation_z = 0
+
+        param_dict = {'rx':rotation_x,
+                      'ry':rotation_y,
+                      'rz':rotation_z,
+                      'tx':translation_x,
+                      'ty':translation_y,
+                      'tz':translation_z,
+                      'f': f,
+                      'cx': c_x,
+                      'k1': k1,
+                      'k2': k2,
+                      'k3': k3,
+                      'width': n_pix}
+        return param_dict
+
+    def read_fov_file(self, fov_file_path):
+        
+
+        
+
+        df_fov = pd.read_csv(fov_file_path, sep = ',', header = None)
+
+        fov_arr = df_fov.values[:, 1]
+
+        param_dict = Specim.fov_2_param(fov = fov_arr)
+        
+        file_name_calib = self.config['Absolute Paths']['hsi_calib_path']
+
+        CalibHSI(file_name_cal_xml=file_name_calib,
+                 mode = 'w', 
+                 param_dict = param_dict)
+
+    def read_nav_file(self, nav_file_path, date):
+        # Convert date string to datetime object
+        date_obj = datetime.strptime(date, "%Y-%m-%d")
+        # Open file for reading.
+        with open(nav_file_path, 'r') as nav_file:
+            count = 0
+            imu_data = []
+            gnss_data = []
+            sync_data = []
+            # Set to -1 to an if sentence to initialize to true
+            hsi_frame_nr_prev = -1
+            # Variable introduced to convert from cyclic HS frame counting to cumulative counts
+            restart_counts = 0
+
+            while True:
+                count += 1
+
+                # Get next line from file
+                line = nav_file.readline()
+
+                line_arr = line.split(sep = ',')
+
+                if line_arr[0] == '$PASHR':
+                    Timestamp_str = line_arr[1]
+                    sec = float(Timestamp_str[4:])
+                    minut = int(Timestamp_str[2:4])
+                    hour = int(Timestamp_str[0:2])
+
+                    # Create a timedelta object for the time
+                    time_delta = timedelta(hours=hour, minutes=minut, seconds=sec)
+
+                    # Calculate the total timedelta
+                    total_timedelta = date_obj + time_delta
+
+                    # Convert to UNIX timestamp (decimal UNIX time)
+                    unix_timestamp = (total_timedelta - datetime(1970, 1, 1)) / timedelta(seconds=1)
+
+                    TimestampAbs = unix_timestamp
+
+                    TimestampClock = date + '_' + Timestamp_str
+
+                    Yaw = float(line_arr[2]) # Heading wrt true north
+                    Roll = float(line_arr[4])
+                    Pitch = float(line_arr[5])# According to https://docs.novatel.com/OEM7/Content/SPAN_Logs/PASHR.htm
+
+
+                    sigmaRoll = float(line_arr[7])
+                    sigmaPitch = float(line_arr[8])  # According to https://docs.novatel.com/OEM7/Content/SPAN_Logs/PASHR.htm
+                    sigmaYaw = float(line_arr[9])
+
+                    #dlogr_imu.append_data(np.array([TimestampClock, TimestampAbs, Roll, Pitch, Yaw, sigmaRoll, sigmaPitch, sigmaYaw]))
+
+                    imu_data_row = {'TimestampClock':TimestampClock,
+                                     'TimestampAbs': TimestampAbs,
+                                     'Roll': Roll,
+                                     'Pitch': Pitch,
+                                     'Yaw': Yaw,
+                                     'sigmaRoll': sigmaRoll,
+                                     'sigmaPitch': sigmaPitch,
+                                     'sigmaYaw': sigmaYaw}
+                    imu_data.append(imu_data_row)
+
+                elif line_arr[0] == '$GNGGA' or line_arr[0] == '$GPGGA':
+                    Timestamp_str = line_arr[1]
+                    sec = float(Timestamp_str[4:])
+                    minut = float(Timestamp_str[2:4])
+                    hour = float(Timestamp_str[0:2])
+
+                    # Create a timedelta object for the time
+                    time_delta = timedelta(hours=hour, minutes=minut, seconds=sec)
+
+                    # Calculate the total timedelta
+                    total_timedelta = date_obj + time_delta
+
+                    # Convert to UNIX timestamp (decimal UNIX time)
+                    unix_timestamp = (total_timedelta - datetime(1970, 1, 1)) / timedelta(seconds=1)
+
+                    TimestampAbs = unix_timestamp
+
+                    TimestampClock = date + '_' + Timestamp_str
+
+                    LatDDMM_MM = float(line_arr[2]) # DDMM.mm
+                    LatInt = int(LatDDMM_MM/100)
+                    Lat = LatInt + (LatDDMM_MM - LatInt*100)/60
+
+
+                    LonDDDMM_MM = float(line_arr[4]) # DDDMM.mm
+                    LonInt = int(LonDDDMM_MM / 100)
+                    Lon = LonInt + (LonDDDMM_MM - LonInt * 100) / 60
+
+                    AltMSL = float(line_arr[9])
+                    AltGeoid = float(line_arr[11])  # According to https://docs.novatel.com/OEM7/Content/Logs/GPGGA.htm
+
+                    #dlogr_gnss.append_data(np.array([TimestampClock, TimestampAbs, Lon, Lat, AltMSL, AltGeoid]))
+                    gnss_data_row = {'TimestampClock':TimestampClock,
+                                     'TimestampAbs': TimestampAbs,
+                                     'Lon': Lon,
+                                     'Lat': Lat,
+                                     'AltMSL': AltMSL,
+                                     'AltGeoid': AltGeoid}
+                    gnss_data.append(gnss_data_row)
+                elif line_arr[0] == '$SPTSMP':
+                    """Recordings of time sync messages, tied to the hyperspectral frames"""
+                    hsi_frame_number_new = int(line_arr[2]) - 1 # Seems they start with a 1-base (like MATLAB)
+
+                    if hsi_frame_number_new < hsi_frame_nr_prev: # When frame counter resets
+                        restart_counts += (hsi_frame_nr_prev - hsi_frame_number_new) + self.metadata_obj.fps # 9950 + 50
+
+
+                    hsi_frame_number = hsi_frame_number_new
+                    hsi_frame_nr_prev = hsi_frame_number_new
+                    prev_time = TimestampAbs
+
+                    # In the file, fram counts go 1, 51, 101,... 9951, 1 ... in a cyclic manner. So to get cumulative counts we add the restart_counts
+                    sync_data_row = {'HsiFrameNum': hsi_frame_number + restart_counts,
+                                     'TimestampAbs': prev_time,
+                                     'TimestampClock': TimestampClock}
+                    sync_data.append(sync_data_row)
+
+
+
+
+                # if line is empty
+                # end of file is reached
+                if not line:
+                    break
+        
+        self.imu_data = imu_data
+        self.gnss_data = gnss_data
+        self.sync_data = sync_data
+
+"""Writer for the h5 file format using a dictionary. The user provides h5 hierarchy paths as values and keys are the names given to the attributes of the specim object.
+A similar write process could be applied to metadata."""
+def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
+    with h5py.File(h5_filename, 'w', libver='latest') as f:
+        for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
+            #print(attribute_name)
+            dset = f.create_dataset(name=h5_hierarchy_item_path, 
+                                            data = getattr(specim_object, attribute_name))            
+
+def add_byte_order_to_envi_header(header_file_path, byte_order_value):
+    """Function added to remedy lacking byte-order entry in header files of radiometric calibration data
+
+    :param header_file_path: _description_
+    :type header_file_path: _type_
+    :param byte_order_value: _description_
+    :type byte_order_value: _type_
+    """
+    # Read the existing ENVI header
+    with open(header_file_path, 'r') as f:
+        header_lines = f.readlines()
+
+    # Look for the line where you want to add "byte order"
+    for i, line in enumerate(header_lines):
+        if line.startswith('byte order'):
+            # If it already exists, update the value
+            header_lines[i] = f'byte order = {byte_order_value}\n'
+            break
+    else:
+        # If it doesn't exist, add it to the end of the header
+        header_lines.append(f'byte order = {byte_order_value}\n')
+
+    # Save the updated header
+    with open(header_file_path, 'w') as f:
+        f.writelines(header_lines)
+
+
+
+def main(config, config_specim):
+    
+    # Function that calibrates data and reforms to h5 file format.
+    dtype = config_specim.dtype_datacube
+    transect_chunk_size = config_specim.lines_per_chunk
+    cal_dir = config_specim.cal_dir
+   
+    mission_dir = config_specim.specim_raw_mission_dir
+
+    mission_name = Path(mission_dir).name
+    out_dir = config_specim.reformatted_missions_dir
+    config_file_path = os.path.join(out_dir, config_specim.config_file_name)
+
+    specim_object = Specim(mission_path=mission_dir, config=config)
+
+    # Patterns for searching data cube files
+    PATTERN_ENVI = '*.hdr'
+
+    # Expects the captured data to reside in capture subfolder
+    capture_dir = os.path.join(mission_dir, 'capture')
+
+    # Path for searching (avoid explicit )
+    search_path_envi = os.path.normpath(os.path.join(capture_dir, PATTERN_ENVI))
+    envi_hdr_file_path = glob.glob(search_path_envi)[0]
+
+    # Read out data
+    spectral_image_obj = envi.open(envi_hdr_file_path)
+
+    """import spectral as sp
+    rgb_im = spectral_image_obj[:,:,]
+    sp.imshow(spectral_image_obj, (73, 50, 24))"""
+
+    # Read all meta data from header file (currently hard coded, but could be avoided I guess)
+    class Metadata:
+        pass
+
+    metadata_obj = Metadata()
+    # Could do this in iteration, but it would need to specify type (I think)
+    metadata_obj.autodarkstartline = int(spectral_image_obj.metadata['autodarkstartline'])
+    metadata_obj.n_lines = int(spectral_image_obj.metadata['lines'])
+    metadata_obj.n_bands = int(spectral_image_obj.metadata['bands'])
+    metadata_obj.n_pix = int(spectral_image_obj.metadata['samples'])
+    metadata_obj.t_exp_ms = float(spectral_image_obj.metadata['tint'])
+    metadata_obj.fps = float(spectral_image_obj.metadata['fps'])
+    metadata_obj.description = spectral_image_obj.metadata['description']
+    metadata_obj.file_type = spectral_image_obj.metadata['file type']
+    metadata_obj.sensor_type = spectral_image_obj.metadata['sensor type']
+    metadata_obj.acquisition_date = spectral_image_obj.metadata['acquisition date']
+    metadata_obj.sensorid = spectral_image_obj.metadata['sensorid']
+    metadata_obj.interleave = spectral_image_obj.metadata['interleave']
+    metadata_obj.data_type = spectral_image_obj.metadata['data type']
+    
+    # Derived from knowledge of the sensor (sensor constants that could differ for other sensors)
+    metadata_obj.binning_spatial = int(ACTIVE_SENSOR_SPATIAL_PIXELS/metadata_obj.n_pix)
+    metadata_obj.binning_spectral = int(ACTIVE_SENSOR_SPECTRAL_PIXELS/metadata_obj.n_bands)
+
+    # Allow Specim Methods to access metadata
+    specim_object.metadata_obj = metadata_obj 
+    # -
+
+    # Based on the binning info, we can locate relevant calibration files, including 1) spectral, 2) geometric, 3) radiometric, and dark frame (from capture).
+    #
+    # We start with the spectral calibration:
+
+    # Comprehensive band info (center, fwhm) is found in "cal_dir/wlcal<spectral binning>b_fwhm.wls"
+    # Pattern follows structure
+    PATTERN_BAND_INFO = '*'+ str(metadata_obj.binning_spectral) + 'b_fwhm.wls'
+    # Linux-CLI search for file.
+    search_path_bands = os.path.normpath(os.path.join(cal_dir, PATTERN_BAND_INFO))
+    band_file_path = glob.glob(search_path_bands)[0]
+
+    # Read the file as csv (although it has no columns)
+    df_bands = pd.read_csv(band_file_path, header=None, sep = '\s+')
+    df_bands.columns = ['Wavelength_nm', 'FWHM_nm']
+
+    # Extract band data
+    specim_object.wavelengths = np.array(df_bands['Wavelength_nm'])
+    specim_object.fwhm = np.array(df_bands['FWHM_nm'])
+
+    # -
+
+    # We will here go through the loading of Specim geometric camera calibration. 
+    # The first step is to load the angular Field-of-View file (AFOV) from the manufacturer. 
+    # Then boresight angles and lever arms can be set, if relevant.
+
+    # +
+    # Pixel-directions is found in "cal_dir/FOV_****_<spatial binning>b.txt" 
+    PATTERN_FOV = 'FOV*' + '_' +  str(metadata_obj.binning_spatial) + 'b.txt'
+
+    # Search for fov file.
+    search_path_fov = os.path.normpath(os.path.join(cal_dir, PATTERN_FOV))
+    fov_file_path = glob.glob(search_path_fov)[0]
+
+    # Calculate a camera model (zero boresight) based on FOV file.
+    # Writes parameters to an *xml file specified by config
+
+    # Read fov data (one angle for each pixel)
+    df_fov = pd.read_csv(fov_file_path, header=None, sep = ',')
+
+    df_fov.columns = ['pixel_nr', 'view_angle_deg', 'Unknown']
+
+    specim_object.view_angles = np.array(df_fov['view_angle_deg'])
+    
+    # Simply converts view angles to camera parameters for a 1D line camera model
+    param_dict = Specim.fov_2_param(fov = specim_object.view_angles)
+    
+    # param_dict are the full camera model parameters, but defaults rotation matrix and translation
+
+    # User set rotation matrix
+    R_hsi_body = config_specim.rotation_matrix_hsi_to_body
+
+    r_zyx = RotLib.from_matrix(R_hsi_body).as_euler('ZYX', degrees=False)
+
+    # Euler angle representation (any other would do too)
+    param_dict['rz'] = r_zyx[0]
+    param_dict['ry'] = r_zyx[1]
+    param_dict['rx'] = r_zyx[2]
+
+    # Vector from origin of HSI to body origin, expressed in body
+    # User set
+    t_hsi_body = config_specim.translation_body_to_hsi
+    param_dict['tz'] = t_hsi_body[0]
+    param_dict['ty'] = t_hsi_body[1]
+    param_dict['tz'] = t_hsi_body[2]
+
+    camera_calib_xml_dir = config['Absolute Paths']['calib_folder']
+
+    file_name_xml = 'HSI_' + str(metadata_obj.binning_spatial) + 'b.xml'
+    xml_cal_write_path = camera_calib_xml_dir + file_name_xml
+
+    CalibHSI(file_name_cal_xml= xml_cal_write_path, 
+                    mode = 'w', 
+                    param_dict = param_dict)
+
+
+    # Set value in config file:
+    config.set('Relative Paths', 'hsi_calib_path', value = xml_cal_write_path)
+
+    
+
+    # Write the config object 
+    with open(config_file_path, 'w') as configfile:
+            config.write(configfile)
+    # -
+
+    
+
+
+    # The next step is to read in radiometric frame.
+
+    # +
+    """Extract radiometric frame from dedicated file"""
+
+    PATTERN_ENVI_CAL = '*_' +str(metadata_obj.binning_spectral) + 'x' +  str(metadata_obj.binning_spatial) + '.hdr'
+
+    search_path_envi_cal = os.path.normpath(os.path.join(cal_dir, PATTERN_ENVI_CAL))
+    ENVI_CAL_HDR_FILE_PATH = glob.glob(search_path_envi_cal)[0]
+
+    # For allowing spectral module to read
+    RAD_CAL_BYTE_ORDER = 0
+
+    add_byte_order_to_envi_header(header_file_path=ENVI_CAL_HDR_FILE_PATH, byte_order_value=RAD_CAL_BYTE_ORDER)
+
+    ENVI_CAL_IMAGE_FILE_PATH = ENVI_CAL_HDR_FILE_PATH.split('.')[0] + '.cal' # SPECTRAL does not expect this suffix by default
+
+    # For some reason, the byte order is needed
+    radiometric_image_obj = envi.open(ENVI_CAL_HDR_FILE_PATH, image = ENVI_CAL_IMAGE_FILE_PATH)
+
+    cal_n_lines = int(radiometric_image_obj.metadata['lines'])
+    cal_n_bands = int(radiometric_image_obj.metadata['bands'])
+    cal_n_pix = int(radiometric_image_obj.metadata['samples'])
+
+    # For calibration
+    radiometric_frame = radiometric_image_obj[:,:,:].reshape((cal_n_pix, cal_n_bands))
+
+    specim_object.radiometric_frame = radiometric_frame
+    # -
+
+    # The next step is to load the darkframes
+
+    # +
+    """1) Crop the hyperspectral data according to the start-stop lines. 2) Write datacube to appropriate directory"""
+    # To ensure that the plots actually do appear in this notebook:
+    # %matplotlib qt
+
+    # Establish dark frame data (at end of recording)
+    data_dark = spectral_image_obj[metadata_obj.autodarkstartline:metadata_obj.n_lines, :, :]
+    dark_frame = np.median(data_dark, axis = 0)
+
+    specim_object.dark_frame = dark_frame
+
+    # -
+
+    # The navigation data is given as messages is a *.nav file. Locate the file and parse it into a suitable format.
+
+    # +
+    # Extract the starting/stopping lines
+    START_STOP_DIR = os.path.join(mission_dir, 'start_stop_lines')
+    
+    # Allow software to function if start_stop_lines not specified
+    if not os.path.exists(START_STOP_DIR):
+        os.mkdir(START_STOP_DIR)
+        # Chunk according to chunk size
+        start_lines = np.arange(start=0,
+                                stop=metadata_obj.autodarkstartline, 
+                                step=transect_chunk_size)
+
+        stop_lines = np.arange(start=transect_chunk_size, 
+                               stop=metadata_obj.autodarkstartline + transect_chunk_size, 
+                               step=transect_chunk_size)
+        
+        stop_lines[-1] = metadata_obj.autodarkstartline # No need to georeference dark data
+
+        # Make dataframe
+        start_stop_data = {'line_start' : start_lines,
+                           'line_stop' : stop_lines}
+        
+        df_start_stop = pd.DataFrame(start_stop_data)
+
+        df_start_stop.to_csv(path_or_buf = os.path.join(START_STOP_DIR, 'start_stop_lines.txt'), sep=' ')
+
+
+
+    PATTERN_START_STOP = '*.txt'
+    
+
+    search_path_lines_start_stop = os.path.normpath(os.path.join(START_STOP_DIR, PATTERN_START_STOP))
+    LINES_START_STOP_FILE_PATH = glob.glob(search_path_lines_start_stop)[0]
+
+    df_start_stop = pd.read_csv(filepath_or_buffer=LINES_START_STOP_FILE_PATH, header=0, sep=' ')
+
+
+
+    # +
+    # Now read the *.nav file
+    NAV_PATTERN = '*.nav'
+
+    search_path_nav = os.path.normpath(os.path.join(capture_dir, NAV_PATTERN))
+    nav_file_path = glob.glob(search_path_nav)[0]
+
+    date_string = metadata_obj.acquisition_date.split(': ')[1] # yyyy-mm-dd
+    # Parse the position/orientation messages
+    specim_object.read_nav_file(nav_file_path=nav_file_path, date = date_string)
+
+
+
+    # -
+
+    # Calculate the frame timestamps from sync data
+
+    # +
+    
+
+
+    df_imu = pd.DataFrame(specim_object.imu_data)
+    df_gnss = pd.DataFrame(specim_object.gnss_data)
+    df_sync_hsi = pd.DataFrame(specim_object.sync_data)
+    
+    # Define the time stamps of HSI frames (special fix for Specim)
+    sync_frames = df_sync_hsi['HsiFrameNum']
+    sync_times = df_sync_hsi['TimestampAbs']
+    hsi_frames = np.arange(metadata_obj.autodarkstartline)
+    hsi_timestamps_total = interp1d(x = sync_frames, y = sync_times, fill_value = 'extrapolate')(x = hsi_frames)
+
+
+    # For ease, let us interpolate position data to imu time (allows one timestamp for nav data)
+    imu_time = df_imu['TimestampAbs']
+
+    # Drop the specified regular clock time (as it is not needed)
+    df_gnss = df_gnss.drop(columns=['TimestampClock'])
+
+    # Interpolate each column in GNSS data based on 'imu_time'
+    interpolated_values = {
+        column: np.interp(imu_time, df_gnss['TimestampAbs'], df_gnss[column])
+        for column in df_gnss.columns if column != 'TimestampAbs'
+    }
+
+    # Create a new DataFrame with the interpolated values
+    df_gnss_interpolated = pd.DataFrame({'time': imu_time, **interpolated_values})
+
+    # The position defined in geodetic coordinates
+    lat = np.array(df_gnss_interpolated['Lat']).reshape((-1,1))
+    lon = np.array(df_gnss_interpolated['Lon']).reshape((-1,1))
+    ellipsoid_height = np.array(df_gnss_interpolated['AltMSL'] + df_gnss_interpolated['AltGeoid']).reshape((-1,1))
+
+    # Assumes WGS-84 (default GNSS frame)
+    x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
+
+    # Lastly, calculate the roll, pitch, yaw
+    roll = np.array(df_imu['Roll']).reshape((-1,1))
+    pitch = np.array(df_imu['Pitch']).reshape((-1,1))
+    yaw = np.array(df_imu['Yaw']).reshape((-1,1))
+
+    # Roll pitch yaw are stacked in attribute eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
+    specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
+
+    # Position is stored as ECEF cartesian coordinates (mutually orthogonal axis) instead of spherioid-like lon, lat, alt
+    specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
+    specim_object.nav_timestamp = imu_time
+    specim_object.t_exp_ms = metadata_obj.t_exp_ms
+
+    # -
+
+    # Last preprocessing step is writing to h5 files. 
+    
+
+    h5_dict_write = {'eul_zyx' : config['HDF.raw_nav']['eul_zyx'],
+            'position_ecef' : config['HDF.raw_nav']['position'],
+            'nav_timestamp' : config['HDF.raw_nav']['timestamp'],
+            'radiance_cube': config['HDF.hyperspectral']['datacube'],
+            't_exp_ms': config['HDF.hyperspectral']['exposuretime'],
+            'hsi_timestamps': config['HDF.hyperspectral']['timestamp'],
+            'view_angles': config['HDF.calibration']['view_angles'],
+            'wavelengths' : config['HDF.calibration']['band2wavelength'],
+            'fwhm' : config['HDF.calibration']['fwhm'],
+            'dark_frame' : config['HDF.calibration']['darkframe'],
+            'radiometric_frame' : config['HDF.calibration']['radiometricframe']}
+
+    # Time to write all the data to a h5 file
+
+
+
+    # # Chunking the recording to user defined sizes and writing it to disk
+
+    # +
+    # Define h5 file name
+    h5_folder = config['Absolute Paths']['h5_folder']
+
+    # Each line in start_stop defines a transect
+    n_transects = df_start_stop.shape[0]
+    for transect_number in range(n_transects):
+        start_line = df_start_stop['line_start'][transect_number]
+        stop_line = df_start_stop['line_stop'][transect_number]
+
+        n_chunks = int(np.ceil((stop_line-start_line)/transect_chunk_size))
+
+        
+        for chunk_number in range(n_chunks):
+            chunk_start_idx = start_line + transect_chunk_size*chunk_number
+
+            if chunk_number == n_chunks-1:
+                chunk_stop_idx = stop_line
+            else:
+                chunk_stop_idx = chunk_start_idx + transect_chunk_size
+
+            #print(f'Chunk from line {chunk_start_idx} to line {chunk_stop_idx} is being written')
+            data_cube = spectral_image_obj[chunk_start_idx:chunk_stop_idx, :, :]
+            # Calibration equation
+            specim_object.radiance_cube = ( (data_cube - dark_frame)*radiometric_frame/(metadata_obj.t_exp_ms/1000) ).astype(dtype = dtype) # 4 Byte
+            specim_object.hsi_timestamps = hsi_timestamps_total[chunk_start_idx:chunk_stop_idx]
+
+            # Possible to name files with <PREFIX>_<time_start>_<Transect#>_<Chunk#>.h5
+            h5_filename = h5_folder + mission_name + '_transectnr_' + str(int(transect_number)) + '_chunknr_' + str(int(chunk_number)) + '.h5'
+
+            specim_object_2_h5_file(h5_filename=h5_filename, h5_tree_dict=h5_dict_write, specim_object=specim_object)
+
+
+
+
+
+
+
+
+
```

### Comparing `gref4hsi-0.2.1/gref4hsi/utils/uhi_parsing_utils.py` & `gref4hsi-0.2.2/gref4hsi/utils/uhi_parsing_utils.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,877 +1,877 @@
-# Python Built-ins
-import os
-import glob
-from datetime import datetime, timedelta, timezone
-from pyproj import CRS, Transformer
-
-# Third party libraries
-from scipy.interpolate import griddata
-import scipy.io as spio
-from scipy.interpolate import interp1d
-import h5py
-import numpy as np
-import pandas as pd
-import pymap3d as pm
-import rasterio
-from rasterio.transform import Affine
-from scipy.spatial.transform import Rotation as RotLib
-
-# Lib specific utilites
-from gref4hsi.utils.specim_parsing_utils import Specim
-from gref4hsi.utils.geometry_utils import CalibHSI
-
-
-"""Reader for the h5 file format in UHI context. The user provides h5 hierarchy paths as values and keys are the names given to the attributes """
-class HyperspectralLite:
-    def __init__(self, h5_filename, h5_tree_dict):
-        with h5py.File(h5_filename, 'r', libver='latest') as self.f:
-            for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
-                print(attribute_name)
-                # Allow there to not be any attribute
-                try:
-                    h5_item = self.f[h5_hierarchy_item_path][()]
-                except KeyError:
-                    pass
-                self.__setattr__(attribute_name, h5_item)
-
-
-
-
-class TimeData:
-    """Simple way of working with time referenced data. Supports unix and date_num at the moment"""
-    def __init__(self, time = None, value = None, time_format = 'date_num'):
-        if time is not None and any(time):
-            if time_format == 'date_num':
-                # Convert MATLAB-style datenum to Unix epoch
-                converted_times = np.zeros((time.shape))
-
-                for i, t in enumerate(time):
-                    # Convert to Unix timestamp
-                    unix_timestamp = datenum_to_unix_time(t)
-                    converted_times[i] = unix_timestamp
-                # Convert to Unix timestamp
-                self.time = converted_times
-
-            elif time_format == 'unix':
-                self.time = time
-            else:
-                AttributeError
-        else:
-            self.time = time
-            
-        self.value = value
-    def interpolate(self, time_interp):
-        self.time_interp = time_interp
-        self.value_interp = interp1d(x = self.time, y = self.value, kind='nearest', fill_value='extrapolate')(x=self.time_interp)
-            
-
-class NAV:
-    """Very simple object allowing for setting time-referenced nav data. Entities end up having four attributes:
-    time: Original time stamps
-    value: Values
-    time_interp: Time stamps interpolated (if interpolate has been run)
-    value_interp: Values interpolated (if interpolate has been run)
-    """
-    def __init__(self):
-        # Initialized to NONE to evoke exceptions
-        self.roll = TimeData()
-        self.pitch = TimeData()
-        self.yaw = TimeData()
-        self.pos_x = TimeData()
-        self.pos_y = TimeData()
-        self.lon = TimeData()
-        self.lat = TimeData()
-        self.pos_z = TimeData()
-        self.altitude = TimeData()
-    def interpolate(self, time_interp):
-        # Iterate through all TimeData objects in NAV and call interpolate method
-        for attr_name, time_data_obj in self.__dict__.items():
-            if isinstance(time_data_obj, TimeData):
-                time_data_obj.interpolate(time_interp)
-
-# +
-def loadmat(filename):
-    '''
-    this function should be called instead of direct spio.loadmat
-    as it cures the problem of not properly recovering python dictionaries
-    from mat files. It calls the function check keys to cure all entries
-    which are still mat-objects
-    '''
-    data = spio.loadmat(filename, struct_as_record=False, squeeze_me=True)
-    return _check_keys(data)
-
-def _check_keys(dict):
-    '''
-    checks if entries in dictionary are mat-objects. If yes
-    todict is called to change them to nested dictionaries
-    '''
-    for key in dict:
-        if isinstance(dict[key], spio.matlab.mat_struct):
-            dict[key] = _todict(dict[key])
-    return dict        
-
-def _todict(matobj):
-    '''
-    A recursive function which constructs from matobjects nested dictionaries
-    '''
-    dict = {}
-    for strg in matobj._fieldnames:
-        elem = matobj.__dict__[strg]
-        if isinstance(elem, spio.matlab.mat_struct):
-            dict[strg] = _todict(elem)
-        else:
-            dict[strg] = elem
-    return dict
-
-def datenum_to_unix_time(datenum):
-    """
-    Convert Matlab datenum into unix time.
-    :param datenum: Date in datenum format
-    :return:        unixtime corresponding to datenum.
-    """
-    days = datenum % 1
-    hours = days % 1 * 24
-    minutes = hours % 1 * 60
-    seconds = minutes % 1 * 60
-
-    dt = datetime.fromordinal(int(datenum)) \
-           + timedelta(days=int(days)) \
-           + timedelta(hours=int(hours)) \
-           + timedelta(minutes=int(minutes)) \
-           + timedelta(seconds=float(seconds)) \
-           - timedelta(days=366)
-    
-    # Defaults to selecting local time zone
-    dt_utc = dt.replace(tzinfo=timezone.utc)
-    unix_timestamp = datetime.timestamp(dt_utc)
-
-    return unix_timestamp
-
-def unix_to_date_and_time(unix_timestamps):
-    """
-    """
-    formatted_dates = [datetime.utcfromtimestamp(ts).strftime('%d.%m.%Y') for ts in unix_timestamps]
-    formatted_times = [datetime.utcfromtimestamp(ts).strftime('%H:%M:%S.%f')[:-3] for ts in unix_timestamps]
-
-    return formatted_dates, formatted_times
-
-def write_immersion_compatible_format_from_nav(nav, unix_times_rov, time_offset, nav_filename):
-        """
-        The format of immersion is as follows:"""
-        # Assuming that nav data is interpolated:
-        nav.interpolate(time_interp=unix_times_rov)
-        
-        # Account for the offset in time
-        hsi_times = unix_times_rov + time_offset
-
-        # Format of data to be fed into Immersion
-        # Date (dd.mm.yyyy), time (hh.mm.ss.ssss), Easting (m), Northing (m), Pitch (dd.ddd), roll (dd.ddd), Heading (dd.ddd), Depth (m.mm), Altitude (m.mm)
-        formatted_dates, formatted_times = unix_to_date_and_time(hsi_times)
-        data = {'Date': formatted_dates,
-                'Time': formatted_times,
-                'Easting': nav.pos_x.value_interp,
-                'Northing': nav.pos_y.value_interp,
-                'Pitch': nav.pitch.value_interp,
-                'Roll': nav.roll.value_interp,
-                'Heading': nav.yaw.value_interp,
-                'Depth': nav.pos_z.value_interp,
-                'Altitude': nav.altitude.value_interp}
-        
-        df = pd.DataFrame(data)
-        df.to_csv(nav_filename, index=False, header=False)
-
-def print_dict_tree_keys(dictionary, indent=0):
-    for key, value in dictionary.items():
-        print('  ' * indent + str(key))
-        if isinstance(value, dict):
-            print_dict_tree_keys(value, indent + 1)
-
-"""Writer (in append mode) for the h5 file format in UHI context. The user provides h5 hierarchy paths as values and keys are the names given to the attributes """
-def write_data_to_h5_file(h5_filename, h5_dict_write, h5_dict_data):
-    with h5py.File(h5_filename, 'a', libver='latest') as f:
-        for key, h5_folder in h5_dict_write.items():
-            # Check if the dataset exists
-            if h5_folder in f:
-                del f[h5_folder]
-
-            dset = f.create_dataset(name=h5_folder, 
-                                            data = h5_dict_data[key])
-            
-def immersion_filename_to_unix_time(immersion_file_name):
-
-        list_names = immersion_file_name.split('_') # The year format should start with 202* or 201*
-
-        result = [(entry,idx)  for (idx, entry) in enumerate(list_names) if entry.startswith(('202', '201'))]
-
-        entry = result[0][0]
-        idx = result[0][1]
-        year_month_date = entry
-        hour_min_sec = list_names[idx+1]
-
-        # Combine the date and time strings
-        combined_datetime_str = year_month_date + hour_min_sec
-
-        # Parse the combined string into a datetime object
-        dt = datetime.strptime(combined_datetime_str, '%Y%m%d%H%M%S')
-
-        dt_utc = dt.replace(tzinfo=timezone.utc)
-        unix_timestamp = datetime.timestamp(dt_utc)
-        return unix_timestamp
-
-
-
-def read_fov_file_to_param(LAB_CAL_DIR, binning_spatial):
-    ## The absolute last step of the journey is to setup calibration the calibration file. We can read the one specified by Ecotone;
-    
-    PATTERN_FOV = 'FOV*' +  str(binning_spatial) + 'b.txt'
-    # Search for fov file.
-    search_path_fov = os.path.normpath(os.path.join(LAB_CAL_DIR, PATTERN_FOV))
-    print(search_path_fov)
-    FOV_FILE_PATH = glob.glob(search_path_fov)[0]
-
-    fov_arr = np.array(pd.read_csv(FOV_FILE_PATH)['View_Angle_Deg'])
-    param_dict = Specim.fov_2_param(fov = fov_arr)
-
-    return param_dict
-
-def set_camera_model(config, config_file_path, config_uhi, model_type, binning_spatial, fov_arr = None):
-    """_summary_
-
-    :param config: _description_
-    :type config: _type_
-    :param config_file_path: _description_
-    :type config_file_path: _type_
-    :param config_uhi: _description_
-    :type config_uhi: _type_
-    :param model_type: ['cal_txt', 'embedded']
-    :type model_type: str
-    :param binning_spatial: _description_
-    :type binning_spatial: _type_
-    :param fov_arr: _description_, defaults to None
-    :type fov_arr: _type_, optional
-    """
-    if model_type == 'cal_txt':
-        # Assumes a csv file with column "View_Angle_Deg" holding the view angles
-        LAB_CAL_DIR = config['General']['lab_cal_dir'] # Where the fov file is
-        param_dict = read_fov_file_to_param(LAB_CAL_DIR=LAB_CAL_DIR, binning_spatial=binning_spatial)
-    elif model_type == 'embedded':
-        # Use supplied fov_array
-        param_dict = Specim.fov_2_param(fov = fov_arr)
-    else:
-        pass
-
-
-
-
-    # User set rotation matrix
-    R_hsi_body = config_uhi.rotation_matrix_hsi_to_body
-
-    r_zyx = RotLib.from_matrix(R_hsi_body).as_euler('ZYX', degrees=False)
-
-    # Euler angle representation (any other would do too)
-    param_dict['rz'] = r_zyx[0]
-    param_dict['ry'] = r_zyx[1]
-    param_dict['rx'] = r_zyx[2]
-
-    # Vector from origin of body to HSI
-    t_hsi_body = config_uhi.translation_body_to_hsi
-    param_dict['tz'] = t_hsi_body[0]
-    param_dict['ty'] = t_hsi_body[1]
-    param_dict['tz'] = t_hsi_body[2]
-
-    # Define where to write calibrated data
-    file_name_xml = 'HSI_' + str(binning_spatial) + 'b.xml'
-    CAMERA_CALIB_XML_DIR = config['Absolute Paths']['calib_folder']
-    xml_cal_write_path = CAMERA_CALIB_XML_DIR + file_name_xml
-
-
-    CalibHSI(file_name_cal_xml= xml_cal_write_path,  
-                        mode = 'w', 
-                        param_dict = param_dict)
-    
-    
-
-
-    # Set value in config file and update:
-    config.set('Relative Paths', 'hsi_calib_path', value = 'Input/Calib/' + file_name_xml)
-
-    with open(config_file_path, 'w') as configfile:
-            config.write(configfile)
-
-
-    
-
-def read_nav_from_mat(mat_filename):
-    """Function for reading mat data from the beast format into a NAV object"""
-    mat_contents = {}
-    mat_contents = loadmat(filename=mat_filename)
-
-    m_att = mat_contents['ATTENTION']
-    #m_att['SpotOnTime'][m_att['Note'] == 'UHI s1 start']
-
-    
-
-    
-    # +
-    """Cell defining all nav data of relevance"""
-
-    # For ease, read position orientation data into structs
-    nav = NAV()
-
-    nav.roll = TimeData(time = mat_contents['TELEMETRY']['SpotOnTime'], 
-                        value = mat_contents['TELEMETRY']['Roll'])
-
-    nav.pitch = TimeData(time = mat_contents['TELEMETRY']['SpotOnTime'], 
-                        value = mat_contents['TELEMETRY']['Pitch'])
-
-    nav.yaw = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
-                        value = mat_contents['POSITION_RENAV']['USBLCourse']) # The USBL course
-
-    nav.pos_x = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
-                        value = mat_contents['POSITION_RENAV']['x'])
-
-    nav.pos_y = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
-                        value = mat_contents['POSITION_RENAV']['y'])
-
-    nav.lat = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
-                        value = mat_contents['POSITION_RENAV']['Latitude'])
-
-    nav.lon = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
-                        value = mat_contents['POSITION_RENAV']['Longitude'])
-
-    nav.pos_z = TimeData(time = mat_contents['TELEMETRY']['SpotOnTime'], 
-                        value = mat_contents['TELEMETRY']['Depth'])
-
-    nav.altitude = TimeData(time = mat_contents['ALTIMETER']['SpotOnTime'], 
-                        value = mat_contents['ALTIMETER']['Altitude']) # Altimeter readings
-    
-    return nav
-
-def write_nav_data_to_h5(nav, time_offset, config, H5_FILE_PATH):
-    
-    # The time stamp used for writing
-    nav_timestamp_rov = nav.yaw.time
-
-    # Interpolate nav data to those times
-    nav.interpolate(time_interp=nav_timestamp_rov)
-
-    lon = nav.lon.value_interp
-    lat = nav.lat.value_interp
-    h = -nav.pos_z.value_interp # Depth is opposite of height
-
-    # Calculate the entire data using the specified lon, lat alt
-    x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = h, deg = True)
-
-    # Roll pitch yaw
-    roll = nav.roll.value_interp.reshape((-1,1))
-    pitch = nav.pitch.value_interp.reshape((-1,1))
-    yaw = nav.yaw.value_interp.reshape((-1,1))
-
-    # Euler triplet
-    eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
-
-    # Position ECEF
-    position_ecef = np.concatenate((x.reshape((-1,1)),y.reshape((-1,1)),z.reshape((-1,1))), axis = 1)
-
-    ##
-
-    # Append the time offset to nav data so that all h5 data is synced to UHI clock
-    hsi_synced_nav_timestamp_rov = nav_timestamp_rov + time_offset
-
-    nav_dict_h5_folders = {'eul_ZYX' : config['HDF.raw_nav']['eul_ZYX'],
-            'position_ecef' : config['HDF.raw_nav']['position'],
-            'nav_timestamp' : config['HDF.raw_nav']['timestamp']}
-
-    # Filling with the following data (all using the same time stamps)
-    invalid_rows = np.isnan(eul_zyx[:,2])
-    nav_dict_h5_data = {'eul_ZYX' : eul_zyx[~invalid_rows],
-            'position_ecef' : position_ecef[~invalid_rows],
-            'nav_timestamp' : hsi_synced_nav_timestamp_rov[~invalid_rows]}
-
-    # Update config object with this info
-    for key, value in nav_dict_h5_folders.items():
-        config.set('HDF.raw_nav', key, value = value)
-    # +
-    write_data_to_h5_file(H5_FILE_PATH, h5_dict_write=nav_dict_h5_folders, h5_dict_data=nav_dict_h5_data)
-
-def altimeter_data_to_point_cloud(nav, config_uhi, lat0, lon0, h0, true_time_hsi):
-    """Converts the pose + altimeter data to a point cloud using the geometry of the range sensor
-
-    :param nav: A Nav object containing UNIX time-stamped position, orientation and range measurements
-    :type nav: Nav object
-    :param config_uhi: A configuration object containing the altimeter's transform (rotation matrix and lever arm)
-    :type config_uhi: Named tuple
-    :param lat0: Latitude for north-east-down linearization
-    :type lat0: float
-    :param lon0: Longitude for north-east-down linearization
-    :type lon0: float
-    :param h0: Latitude for north-east-down linearization
-    :type h0: float
-    :param true_time_hsi: The time stamps of the hyperspectral imager
-    :type true_time_hsi: float
-    :return: point cloud of 
-    :rtype: _type_
-    """
-
-    # Number of altimeter samples
-    n = nav.altitude.value.size
-
-    # Interpolate all navigation data to the time of altimeter data
-    # TODO: avoid common interpolation of yaw, pitch, roll
-    nav.interpolate(time_interp=nav.altitude.time)
-
-    # Create augmented vector allowing 4x4 transformation matrices
-    alt_vec = np.zeros((4, n))
-    alt_vec[2] = nav.altitude.value # Ranges are captured along z-axis (by definition)
-    alt_vec[3] = 1
-
-    # Preallocate transform from altimeter to body frame
-    T_alt_body = np.zeros((4,4))
-    T_alt_body[3,3] = 1
-
-    # User specified altimeter position, orientation on the body
-    R_alt_body = config_uhi.rotation_matrix_alt_to_body
-    t_alt_body = config_uhi.translation_alt_to_body
-
-    # Insert in transormation matrix
-    T_alt_body[:3,:3] = R_alt_body
-    T_alt_body[:3, 3] = t_alt_body
-
-    # Transform ranges to body frame
-    alt_vec_body = np.matmul(T_alt_body.reshape((4,4)), alt_vec)
-
-    # -------------------------Define transformation from body to NED-----------------------------
-    roll = nav.roll.value_interp.reshape((-1,1))
-    pitch = nav.pitch.value_interp.reshape((-1,1))
-    yaw = nav.yaw.value_interp.reshape((-1,1))
-
-    eul_zyx_alt = np.concatenate((roll, pitch, yaw), axis = 1)
-
-
-    lat_alt = nav.lat.value_interp
-    lon_alt = nav.lon.value_interp
-    h_alt = -nav.pos_z.value_interp
-
-    # User specified values
-    lon0 = config_uhi.lon_lat_alt_origin[0]
-    lat0 = config_uhi.lon_lat_alt_origin[1]
-    h0 = config_uhi.lon_lat_alt_origin[2]
-
-    # Transform to local NED for working with vectors
-    north, east, down = pm.geodetic2ned(lat=lat_alt, lon = lon_alt, h = h_alt, lat0 = lat0, lon0=lon0, h0 = h0, deg = True)
-
-    # Account for the motion
-    R_mats_body_ned = RotLib.from_euler("ZYX", np.flip(eul_zyx_alt, axis=1), degrees=True).as_matrix()
-    t_body_ned = np.vstack((north, east, down)).T
-
-    # Set transformation matrices (one for each timestamp)
-    T_body_ned = np.zeros((n, 4,4))
-    T_body_ned[:, 3,3] = 1
-    T_body_ned[:, :3,:3] = R_mats_body_ned
-    T_body_ned[:, :3, 3] = t_body_ned
-
-    # ----------------------------------------------------------------------------------------------
-
-    # Transform ranges to NED
-    alt_vec_ned = np.einsum('ijk, ki->ji', T_body_ned, alt_vec_body)
-
-    # Transpose vectors (just out of preference)
-    altimeter_point_cloud = alt_vec_ned[0:3,:].T
-
-    # Select the points from an appropriate time interval
-    crit_1 = nav.altitude.time < true_time_hsi.max()
-    crit_2 = nav.altitude.time > true_time_hsi.min()
-
-    points_altimeter_transect = altimeter_point_cloud[(crit_1) & (crit_2)]
-
-    # Still the points are given in a form of NED
-
-    # NED is no frame for GIS, but an OK frame for certain vector operations.
-    # The above linearization is only accurate for small surveys such as those in UHI
-
-    return points_altimeter_transect
-
-def point_cloud_to_dem(points, config, resolution_dem, lon0, lat0, h0, method='nearest', smooth_DEM=True):
-    """Converts the sparse point cloud of altimeter data into a digital elevation model.
-
-    :param points: _description_
-    :type points: _type_
-    :param config: _description_
-    :type config: _type_
-    :param resolution_dem: _description_
-    :type resolution_dem: _type_
-    :param lon0: _description_
-    :type lon0: _type_
-    :param lat0: _description_
-    :type lat0: _type_
-    :param h0: _description_
-    :type h0: _type_
-    :param method: _description_, defaults to 'nearest'
-    :type method: str, optional
-    :param smooth_DEM: _description_, defaults to True
-    :type smooth_DEM: bool, optional
-    """
-    # The name of the digital elevation model
-    output_dem_path = config['Absolute Paths']['dem_path']
-
-    # The padding (ensuring that all rays hit the model)
-    pad_xy = float(config['General']['max_ray_length'])
-
-    x_coords = points[:,0]
-    y_coords = points[:,1]
-    z_values = points[:,2]
-
-    #-----------------------------------------------------Transform Extent and determing resolution, geotransform and grid--------------------------------------------------------
-    
-    # Determine the min/max coordinates with padding in the NED plane, and warp to projected grid.
-    x_min, x_max = x_coords.min() - pad_xy, x_coords.max() + pad_xy
-
-    y_min, y_max = y_coords.min() - pad_xy, y_coords.max() + pad_xy
-
-    extent_ned = np.array([[x_min, y_min],
-                          [x_min, y_max],
-                          [x_max, y_min],
-                          [x_max, y_max]])
-
-    # Transform to wgs 84, aka epsg 4326
-    lat_ext, lon_ext, h_ext = pm.ned2geodetic(n = extent_ned[:,0], e = extent_ned[:,1], d = extent_ned[:,1]*0 + z_values.mean(), lat0 = lat0, lon0=lon0, h0 = h0, deg = True)
-    
-    # Transform to desired CRS
-    epsg_wgs84 = 4326
-    dem_epsg = int(config['Coordinate Reference Systems']['dem_epsg'])
-
-    # Define transformer
-    crs_84 = CRS.from_epsg(epsg_wgs84)
-    crs_dem = CRS.from_epsg(dem_epsg)
-    transformer = Transformer.from_crs(crs_84, crs_dem)
-
-    # Transform extent
-    (x, y, z) = transformer.transform(xx=lat_ext, yy=lon_ext, zz=h_ext)
-
-    if crs_dem.is_geographic:
-
-        res_x = resolution_dem*(x.max() - x.min())/(x_max - x_min)
-        res_y = resolution_dem*(y.max() - y.min())/(y_max - y_min)
-        transform = Affine(a = res_y,
-                        b = 0,
-                        c = y.min(),
-                        d = 0,
-                        e = -res_x,
-                        f = x.max())
-        # Setup mesh grid
-        grid_y, grid_x = np.meshgrid(np.arange(y.min(), y.max(), res_y),
-                                np.arange(x.min(), x.max(), res_x))
-    elif crs_dem.is_projected:
-        # North is then Y
-        res_x = resolution_dem*(x.max() - x.min())/(y_max - y_min)
-        res_y = resolution_dem*(y.max() - y.min())/(x_max - x_min)
-        transform = Affine(a = res_x,
-                        b = 0,
-                        c = x.min(),
-                        d = 0,
-                        e = -res_y,
-                        f = y.max())
-        # Setup mesh grid
-        grid_x, grid_y = np.meshgrid(np.arange(x.min(), x.max(), res_x),
-                                np.arange(y.min(), y.max(), res_y))
-    #--------------------------------------------------------------------------------------------------------------------------------------------------------------------
-
-    # ---------------------------------------------------Transform point cloud------------------------------------------------------------------------------------------
-    
-    # Transform to wgs 84, aka epsg 4326
-    lat_pc, lon_pc, h_pc = pm.ned2geodetic(n = points[:,0], e = points[:,1], d = points[:,2], lat0 = lat0, lon0=lon0, h0 = h0, deg = True)
-    # Transform to target system
-    (x_pc, y_pc, z_pc) = transformer.transform(xx=lat_pc, yy=lon_pc, zz=h_pc)
-
-    points_pc_dem_crs = np.concatenate((x_pc.reshape((-1,1)),
-                                        y_pc.reshape((-1,1)),
-                                        z_pc.reshape((-1,1))), axis = 1)
-    
-
-    # ----------------------------------------------------------------------------------------------------------------------------------------------------------------------
-    
-    # Interpolate z-data to grid
-
-    if method == 'nearest':
-        grid_z = griddata(points_pc_dem_crs[:, :2], points_pc_dem_crs[:,2], (grid_x, grid_y), method='nearest')
-    elif method == 'IDW':
-        import pyinterp
-        mesh = pyinterp.RTree()
-
-        mesh.packing(points_pc_dem_crs[:, :2], points_pc_dem_crs[:,2])
-
-        idw, neighbors = mesh.inverse_distance_weighting(
-        np.vstack((grid_x.ravel(), grid_y.ravel())).T,
-        within=False,  # Extrapolation is forbidden
-        k=11,  # We are looking for at most 11 neighbors
-        num_threads=0)
-
-        grid_z = idw.reshape(grid_x.shape)
-
-
-    if smooth_DEM == True:
-        from scipy import ndimage
-        # Smooths by 4 pixel units
-        sigma_x = 4
-        sigma_y = 4
-        grid_z = ndimage.gaussian_filter(grid_z, sigma=(sigma_y, sigma_x))
-        
-
-    
-    # Writes to a file
-    with rasterio.open(output_dem_path, 'w', driver='GTiff', height=grid_z.shape[0],
-                    width=grid_z.shape[1], count=1, dtype='float64', crs='EPSG:' + str(dem_epsg),
-                    transform=transform) as dst:
-        dst.write(grid_z, 1)
-
-
-
-
-def uhi_beast(config, config_uhi):
-    MISSION_PATH = config['General']['mission_dir'] # Where h5 data is 
-    
-
-    # For writing
-    config_file_path = os.path.join(MISSION_PATH, 'configuration.ini')
-
-    SPATIAL_PIXELS = 1936 # Same for almost all UHI
-    
-
-    INPUT_DIR = MISSION_PATH + 'Input/'
-
-    h5_folder = config['Absolute Paths']['h5_folder']
-    H5_PATTERN = '*.h5'
-
-    MAT_DIR = INPUT_DIR
-    MAT_PATTERN = '*.mat'
-
-    # Locate mat file with nav data 
-    search_path_mat = os.path.normpath(os.path.join(MAT_DIR, MAT_PATTERN))
-    MAT_FILE_PATHS = glob.glob(search_path_mat)
-    MAT_PATH = MAT_FILE_PATHS[0] # Assuming there is only one
-
-    nav = read_nav_from_mat(mat_filename=MAT_PATH)
-
-    
-
-    # Search the h5 folder (these are the files to iterate)
-    search_path_h5 = os.path.normpath(os.path.join(h5_folder, H5_PATTERN))
-    H5_FILE_PATHS = glob.glob(search_path_h5)
-
-    number_of_h5_files = len(H5_FILE_PATHS)
-
-    h5_dict_read = {'radiance_cube': config['HDF.hyperspectral']['datacube'],
-            'hsi_frames_timestamp': config['HDF.hyperspectral']['timestamp'],
-            'fov': config['HDF.calibration']['fov'],
-            'wavelengths' : config['HDF.calibration']['band2wavelength'],
-            #'rgb_frames' : config['HDF.rgb']['rgb_frames'],
-            #'rgb_timestamp' : config['HDF.rgb']['rgb_timestamp']
-            }
-    
-    time_offset = config_uhi.time_offset_sec
-    lon0, lat0, alt0 = config_uhi.lon_lat_alt_origin
-
-    # from gref4hsi.utils.photogrammetry_utils import Photogrammetry
-    # agisoft_object = Photogrammetry(project_folder = MISSION_PATH, software_type='agisoft')
-    # TODO:: Add support for concurrent camera given that images are contained in a h5 folder. 
-    # Should interface towards ODM as well
-
-    for h5_index in range(number_of_h5_files):
-        H5_FILE_PATH = H5_FILE_PATHS[h5_index]
-
-        # Read the specified entries
-        hyp = HyperspectralLite(h5_filename=H5_FILE_PATH, h5_tree_dict=h5_dict_read)
-
-        if h5_index == 0:
-            # Camera model is set once, assuming same spatial binning throughout
-            binning_spatial = int(np.round(SPATIAL_PIXELS/hyp.radiance_cube.shape[1]))
-            # Sets camera model with user specified boresight ...
-            set_camera_model(config=config, 
-                             config_file_path = config_file_path, 
-                             config_uhi=config_uhi, 
-                             model_type = 'cal_txt', 
-                             binning_spatial = binning_spatial)
-
-        true_time_hsi = hyp.hsi_frames_timestamp - time_offset
-
-        # Interpolate nav to roll time, IMU time (considered nav timestamp)
-
-        ## write nav data to h5 file
-        write_nav_data_to_h5(nav, time_offset, config, H5_FILE_PATH)
-        
-        # Build a point cloud
-        point_cloud_altimeter = altimeter_data_to_point_cloud(nav=nav, 
-                                                              config_uhi=config_uhi, 
-                                                              true_time_hsi = true_time_hsi, 
-                                                              lon0=lon0, 
-                                                              lat0=lat0, 
-                                                              h0=alt0)
-        if h5_index == 0:
-            point_cloud_altimeter_total = point_cloud_altimeter
-        else:
-            point_cloud_altimeter_total = np.append(point_cloud_altimeter_total, point_cloud_altimeter, axis = 0)
-        
-
-
-        """# If desirable to write to Agisoft type format
-        if config_uhi.agisoft_process:
-            nav_rgb = nav
-            nav_rgb.interpolate(time_interp=hyp.rgb_timestamp)
-
-            # Prepare for SfM/photogrammetry processing
-            try:
-                agisoft_object.export_rgb_from_h5(h5_folder=H5_FILE_PATH, 
-                                            rgb_image_cube = hyp.rgb_frames, 
-                                            nav_rgb = nav_rgb,
-                                            rgb_write_dir=config['Absolute Paths']['rgbimagedir'],
-                                            pos_acc = np.array([1, 1, 0.05]), 
-                                            rot_acc = np.array([1, 1, 5]))
-            except:
-                pass # If no RGB data, move forward"""
-        
-        
-        
-        print(H5_FILE_PATH)
-    
-    # Use the total point cloud to make a DEM
-    
-
-    if config_uhi.agisoft_process:
-        agisoft_object.load_photos_and_reference()
-
-
-
-
-
-    point_cloud_to_dem(point_cloud_altimeter_total, 
-                                 config, 
-                                 resolution_dem = config_uhi.resolution_dem, 
-                                 lon0=lon0, 
-                                 lat0=lat0, 
-                                 h0=alt0)
-
-
-
-
-def uhi_dbe(config, config_uhi):
-    """Preparing data for the UHI-2x blueye edition (almost copy of beast)
-
-    :param config: _description_
-    :type config: _type_
-    :param config_uhi: _description_
-    :type config_uhi: _type_
-    """
-    MISSION_PATH = config['General']['mission_dir'] # Where h5 data is 
-    
-
-    # For writing
-    config_file_path = os.path.join(MISSION_PATH, 'configuration.ini')
-
-    SPATIAL_PIXELS = 1936 # Same for almost all UHI
-    
-
-    INPUT_DIR = MISSION_PATH + 'Input/'
-
-    h5_folder = config['Absolute Paths']['h5_folder']
-    H5_PATTERN = '*.h5'
-
-    MAT_DIR = INPUT_DIR
-    MAT_PATTERN = '*.mat'
-
-    # Locate mat file with nav data 
-    search_path_mat = os.path.normpath(os.path.join(MAT_DIR, MAT_PATTERN))
-    MAT_FILE_PATHS = glob.glob(search_path_mat)
-    MAT_PATH = MAT_FILE_PATHS[0] # Assuming there is only one
-
-
-    # TODO: replace with how you read in data from DVL/H5 folders
-    nav = read_nav_from_mat(mat_filename=MAT_PATH)
-
-    
-
-    # Search the h5 folder (these are the files to iterate)
-    search_path_h5 = os.path.normpath(os.path.join(h5_folder, H5_PATTERN))
-    H5_FILE_PATHS = glob.glob(search_path_h5)
-
-    number_of_h5_files = len(H5_FILE_PATHS)
-
-    h5_dict_read = {'radiance_cube': config['HDF.hyperspectral']['datacube'],
-            'hsi_frames_timestamp': config['HDF.hyperspectral']['timestamp'],
-            'fov': config['HDF.calibration']['fov'],
-            'wavelengths' : config['HDF.calibration']['band2wavelength'],
-            #'rgb_frames' : config['HDF.rgb']['rgb_frames'],
-            #'rgb_timestamp' : config['HDF.rgb']['rgb_timestamp']
-            }
-    
-    time_offset = config_uhi.time_offset_sec
-    lon0, lat0, alt0 = config_uhi.lon_lat_alt_origin
-
-    # from gref4hsi.utils.photogrammetry_utils import Photogrammetry
-    # agisoft_object = Photogrammetry(project_folder = MISSION_PATH, software_type='agisoft')
-    # TODO:: Add support for concurrent camera given that images are contained in a h5 folder. 
-    # Should interface towards ODM as well
-
-    for h5_index in range(number_of_h5_files):
-        H5_FILE_PATH = H5_FILE_PATHS[h5_index]
-
-        # Read the specified entries
-        hyp = HyperspectralLite(h5_filename=H5_FILE_PATH, h5_tree_dict=h5_dict_read)
-
-        if h5_index == 0:
-            # Camera model is set once, assuming same spatial binning throughout
-            binning_spatial = int(np.round(SPATIAL_PIXELS/hyp.radiance_cube.shape[1]))
-            
-            # Extract from the hyperspectral object
-            fov_arr = hyp.fov
-
-            # Sets camera model with user specified boresight ...
-            set_camera_model(config=config, 
-                             config_file_path = config_file_path, 
-                             config_uhi=config_uhi, 
-                             model_type = 'embedded', 
-                             binning_spatial = binning_spatial,
-                             fov_arr=fov_arr)
-
-        true_time_hsi = hyp.hsi_frames_timestamp - time_offset
-
-        # Interpolate nav to roll time, IMU time (considered nav timestamp)
-
-        ## write nav data to h5 file
-        write_nav_data_to_h5(nav, time_offset, config, H5_FILE_PATH)
-        
-        # Build a point cloud
-        point_cloud_altimeter = altimeter_data_to_point_cloud(nav = nav, 
-                                                              config_uhi=config_uhi, 
-                                                              true_time_hsi = true_time_hsi, 
-                                                              lon0=lon0, 
-                                                              lat0=lat0, 
-                                                              h0=alt0)
-        if h5_index == 0:
-            point_cloud_altimeter_total = point_cloud_altimeter
-        else:
-            point_cloud_altimeter_total = np.append(point_cloud_altimeter_total, point_cloud_altimeter, axis = 0)
-        
-        
-        
-        print(H5_FILE_PATH)
-    
-    # Use the total point cloud to make a DEM
-    
-
-    if config_uhi.agisoft_process:
-        agisoft_object.load_photos_and_reference()
-
-
-
-
-
-    point_cloud_to_dem(point_cloud_altimeter_total, 
-                                 config, 
-                                 resolution_dem = config_uhi.resolution_dem, 
-                                 lon0=lon0, 
-                                 lat0=lat0, 
-                                 h0=alt0)
-
-        
-
+# Python Built-ins
+import os
+import glob
+from datetime import datetime, timedelta, timezone
+from pyproj import CRS, Transformer
+
+# Third party libraries
+from scipy.interpolate import griddata
+import scipy.io as spio
+from scipy.interpolate import interp1d
+import h5py
+import numpy as np
+import pandas as pd
+import pymap3d as pm
+import rasterio
+from rasterio.transform import Affine
+from scipy.spatial.transform import Rotation as RotLib
+
+# Lib specific utilites
+from gref4hsi.utils.specim_parsing_utils import Specim
+from gref4hsi.utils.geometry_utils import CalibHSI
+
+
+"""Reader for the h5 file format in UHI context. The user provides h5 hierarchy paths as values and keys are the names given to the attributes """
+class HyperspectralLite:
+    def __init__(self, h5_filename, h5_tree_dict):
+        with h5py.File(h5_filename, 'r', libver='latest') as self.f:
+            for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
+                print(attribute_name)
+                # Allow there to not be any attribute
+                try:
+                    h5_item = self.f[h5_hierarchy_item_path][()]
+                except KeyError:
+                    pass
+                self.__setattr__(attribute_name, h5_item)
+
+
+
+
+class TimeData:
+    """Simple way of working with time referenced data. Supports unix and date_num at the moment"""
+    def __init__(self, time = None, value = None, time_format = 'date_num'):
+        if time is not None and any(time):
+            if time_format == 'date_num':
+                # Convert MATLAB-style datenum to Unix epoch
+                converted_times = np.zeros((time.shape))
+
+                for i, t in enumerate(time):
+                    # Convert to Unix timestamp
+                    unix_timestamp = datenum_to_unix_time(t)
+                    converted_times[i] = unix_timestamp
+                # Convert to Unix timestamp
+                self.time = converted_times
+
+            elif time_format == 'unix':
+                self.time = time
+            else:
+                AttributeError
+        else:
+            self.time = time
+            
+        self.value = value
+    def interpolate(self, time_interp):
+        self.time_interp = time_interp
+        self.value_interp = interp1d(x = self.time, y = self.value, kind='nearest', fill_value='extrapolate')(x=self.time_interp)
+            
+
+class NAV:
+    """Very simple object allowing for setting time-referenced nav data. Entities end up having four attributes:
+    time: Original time stamps
+    value: Values
+    time_interp: Time stamps interpolated (if interpolate has been run)
+    value_interp: Values interpolated (if interpolate has been run)
+    """
+    def __init__(self):
+        # Initialized to NONE to evoke exceptions
+        self.roll = TimeData()
+        self.pitch = TimeData()
+        self.yaw = TimeData()
+        self.pos_x = TimeData()
+        self.pos_y = TimeData()
+        self.lon = TimeData()
+        self.lat = TimeData()
+        self.pos_z = TimeData()
+        self.altitude = TimeData()
+    def interpolate(self, time_interp):
+        # Iterate through all TimeData objects in NAV and call interpolate method
+        for attr_name, time_data_obj in self.__dict__.items():
+            if isinstance(time_data_obj, TimeData):
+                time_data_obj.interpolate(time_interp)
+
+# +
+def loadmat(filename):
+    '''
+    this function should be called instead of direct spio.loadmat
+    as it cures the problem of not properly recovering python dictionaries
+    from mat files. It calls the function check keys to cure all entries
+    which are still mat-objects
+    '''
+    data = spio.loadmat(filename, struct_as_record=False, squeeze_me=True)
+    return _check_keys(data)
+
+def _check_keys(dict):
+    '''
+    checks if entries in dictionary are mat-objects. If yes
+    todict is called to change them to nested dictionaries
+    '''
+    for key in dict:
+        if isinstance(dict[key], spio.matlab.mat_struct):
+            dict[key] = _todict(dict[key])
+    return dict        
+
+def _todict(matobj):
+    '''
+    A recursive function which constructs from matobjects nested dictionaries
+    '''
+    dict = {}
+    for strg in matobj._fieldnames:
+        elem = matobj.__dict__[strg]
+        if isinstance(elem, spio.matlab.mat_struct):
+            dict[strg] = _todict(elem)
+        else:
+            dict[strg] = elem
+    return dict
+
+def datenum_to_unix_time(datenum):
+    """
+    Convert Matlab datenum into unix time.
+    :param datenum: Date in datenum format
+    :return:        unixtime corresponding to datenum.
+    """
+    days = datenum % 1
+    hours = days % 1 * 24
+    minutes = hours % 1 * 60
+    seconds = minutes % 1 * 60
+
+    dt = datetime.fromordinal(int(datenum)) \
+           + timedelta(days=int(days)) \
+           + timedelta(hours=int(hours)) \
+           + timedelta(minutes=int(minutes)) \
+           + timedelta(seconds=float(seconds)) \
+           - timedelta(days=366)
+    
+    # Defaults to selecting local time zone
+    dt_utc = dt.replace(tzinfo=timezone.utc)
+    unix_timestamp = datetime.timestamp(dt_utc)
+
+    return unix_timestamp
+
+def unix_to_date_and_time(unix_timestamps):
+    """
+    """
+    formatted_dates = [datetime.utcfromtimestamp(ts).strftime('%d.%m.%Y') for ts in unix_timestamps]
+    formatted_times = [datetime.utcfromtimestamp(ts).strftime('%H:%M:%S.%f')[:-3] for ts in unix_timestamps]
+
+    return formatted_dates, formatted_times
+
+def write_immersion_compatible_format_from_nav(nav, unix_times_rov, time_offset, nav_filename):
+        """
+        The format of immersion is as follows:"""
+        # Assuming that nav data is interpolated:
+        nav.interpolate(time_interp=unix_times_rov)
+        
+        # Account for the offset in time
+        hsi_times = unix_times_rov + time_offset
+
+        # Format of data to be fed into Immersion
+        # Date (dd.mm.yyyy), time (hh.mm.ss.ssss), Easting (m), Northing (m), Pitch (dd.ddd), roll (dd.ddd), Heading (dd.ddd), Depth (m.mm), Altitude (m.mm)
+        formatted_dates, formatted_times = unix_to_date_and_time(hsi_times)
+        data = {'Date': formatted_dates,
+                'Time': formatted_times,
+                'Easting': nav.pos_x.value_interp,
+                'Northing': nav.pos_y.value_interp,
+                'Pitch': nav.pitch.value_interp,
+                'Roll': nav.roll.value_interp,
+                'Heading': nav.yaw.value_interp,
+                'Depth': nav.pos_z.value_interp,
+                'Altitude': nav.altitude.value_interp}
+        
+        df = pd.DataFrame(data)
+        df.to_csv(nav_filename, index=False, header=False)
+
+def print_dict_tree_keys(dictionary, indent=0):
+    for key, value in dictionary.items():
+        print('  ' * indent + str(key))
+        if isinstance(value, dict):
+            print_dict_tree_keys(value, indent + 1)
+
+"""Writer (in append mode) for the h5 file format in UHI context. The user provides h5 hierarchy paths as values and keys are the names given to the attributes """
+def write_data_to_h5_file(h5_filename, h5_dict_write, h5_dict_data):
+    with h5py.File(h5_filename, 'a', libver='latest') as f:
+        for key, h5_folder in h5_dict_write.items():
+            # Check if the dataset exists
+            if h5_folder in f:
+                del f[h5_folder]
+
+            dset = f.create_dataset(name=h5_folder, 
+                                            data = h5_dict_data[key])
+            
+def immersion_filename_to_unix_time(immersion_file_name):
+
+        list_names = immersion_file_name.split('_') # The year format should start with 202* or 201*
+
+        result = [(entry,idx)  for (idx, entry) in enumerate(list_names) if entry.startswith(('202', '201'))]
+
+        entry = result[0][0]
+        idx = result[0][1]
+        year_month_date = entry
+        hour_min_sec = list_names[idx+1]
+
+        # Combine the date and time strings
+        combined_datetime_str = year_month_date + hour_min_sec
+
+        # Parse the combined string into a datetime object
+        dt = datetime.strptime(combined_datetime_str, '%Y%m%d%H%M%S')
+
+        dt_utc = dt.replace(tzinfo=timezone.utc)
+        unix_timestamp = datetime.timestamp(dt_utc)
+        return unix_timestamp
+
+
+
+def read_fov_file_to_param(LAB_CAL_DIR, binning_spatial):
+    ## The absolute last step of the journey is to setup calibration the calibration file. We can read the one specified by Ecotone;
+    
+    PATTERN_FOV = 'FOV*' +  str(binning_spatial) + 'b.txt'
+    # Search for fov file.
+    search_path_fov = os.path.normpath(os.path.join(LAB_CAL_DIR, PATTERN_FOV))
+    print(search_path_fov)
+    FOV_FILE_PATH = glob.glob(search_path_fov)[0]
+
+    fov_arr = np.array(pd.read_csv(FOV_FILE_PATH)['View_Angle_Deg'])
+    param_dict = Specim.fov_2_param(fov = fov_arr)
+
+    return param_dict
+
+def set_camera_model(config, config_file_path, config_uhi, model_type, binning_spatial, fov_arr = None):
+    """_summary_
+
+    :param config: _description_
+    :type config: _type_
+    :param config_file_path: _description_
+    :type config_file_path: _type_
+    :param config_uhi: _description_
+    :type config_uhi: _type_
+    :param model_type: ['cal_txt', 'embedded']
+    :type model_type: str
+    :param binning_spatial: _description_
+    :type binning_spatial: _type_
+    :param fov_arr: _description_, defaults to None
+    :type fov_arr: _type_, optional
+    """
+    if model_type == 'cal_txt':
+        # Assumes a csv file with column "View_Angle_Deg" holding the view angles
+        LAB_CAL_DIR = config['General']['lab_cal_dir'] # Where the fov file is
+        param_dict = read_fov_file_to_param(LAB_CAL_DIR=LAB_CAL_DIR, binning_spatial=binning_spatial)
+    elif model_type == 'embedded':
+        # Use supplied fov_array
+        param_dict = Specim.fov_2_param(fov = fov_arr)
+    else:
+        pass
+
+
+
+
+    # User set rotation matrix
+    R_hsi_body = config_uhi.rotation_matrix_hsi_to_body
+
+    r_zyx = RotLib.from_matrix(R_hsi_body).as_euler('ZYX', degrees=False)
+
+    # Euler angle representation (any other would do too)
+    param_dict['rz'] = r_zyx[0]
+    param_dict['ry'] = r_zyx[1]
+    param_dict['rx'] = r_zyx[2]
+
+    # Vector from origin of body to HSI
+    t_hsi_body = config_uhi.translation_body_to_hsi
+    param_dict['tz'] = t_hsi_body[0]
+    param_dict['ty'] = t_hsi_body[1]
+    param_dict['tz'] = t_hsi_body[2]
+
+    # Define where to write calibrated data
+    file_name_xml = 'HSI_' + str(binning_spatial) + 'b.xml'
+    CAMERA_CALIB_XML_DIR = config['Absolute Paths']['calib_folder']
+    xml_cal_write_path = CAMERA_CALIB_XML_DIR + file_name_xml
+
+
+    CalibHSI(file_name_cal_xml= xml_cal_write_path,  
+                        mode = 'w', 
+                        param_dict = param_dict)
+    
+    
+
+
+    # Set value in config file and update:
+    config.set('Relative Paths', 'hsi_calib_path', value = 'Input/Calib/' + file_name_xml)
+
+    with open(config_file_path, 'w') as configfile:
+            config.write(configfile)
+
+
+    
+
+def read_nav_from_mat(mat_filename):
+    """Function for reading mat data from the beast format into a NAV object"""
+    mat_contents = {}
+    mat_contents = loadmat(filename=mat_filename)
+
+    m_att = mat_contents['ATTENTION']
+    #m_att['SpotOnTime'][m_att['Note'] == 'UHI s1 start']
+
+    
+
+    
+    # +
+    """Cell defining all nav data of relevance"""
+
+    # For ease, read position orientation data into structs
+    nav = NAV()
+
+    nav.roll = TimeData(time = mat_contents['TELEMETRY']['SpotOnTime'], 
+                        value = mat_contents['TELEMETRY']['Roll'])
+
+    nav.pitch = TimeData(time = mat_contents['TELEMETRY']['SpotOnTime'], 
+                        value = mat_contents['TELEMETRY']['Pitch'])
+
+    nav.yaw = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
+                        value = mat_contents['POSITION_RENAV']['USBLCourse']) # The USBL course
+
+    nav.pos_x = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
+                        value = mat_contents['POSITION_RENAV']['x'])
+
+    nav.pos_y = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
+                        value = mat_contents['POSITION_RENAV']['y'])
+
+    nav.lat = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
+                        value = mat_contents['POSITION_RENAV']['Latitude'])
+
+    nav.lon = TimeData(time = mat_contents['POSITION_RENAV']['SpotOnTime'], 
+                        value = mat_contents['POSITION_RENAV']['Longitude'])
+
+    nav.pos_z = TimeData(time = mat_contents['TELEMETRY']['SpotOnTime'], 
+                        value = mat_contents['TELEMETRY']['Depth'])
+
+    nav.altitude = TimeData(time = mat_contents['ALTIMETER']['SpotOnTime'], 
+                        value = mat_contents['ALTIMETER']['Altitude']) # Altimeter readings
+    
+    return nav
+
+def write_nav_data_to_h5(nav, time_offset, config, H5_FILE_PATH):
+    
+    # The time stamp used for writing
+    nav_timestamp_rov = nav.yaw.time
+
+    # Interpolate nav data to those times
+    nav.interpolate(time_interp=nav_timestamp_rov)
+
+    lon = nav.lon.value_interp
+    lat = nav.lat.value_interp
+    h = -nav.pos_z.value_interp # Depth is opposite of height
+
+    # Calculate the entire data using the specified lon, lat alt
+    x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = h, deg = True)
+
+    # Roll pitch yaw
+    roll = nav.roll.value_interp.reshape((-1,1))
+    pitch = nav.pitch.value_interp.reshape((-1,1))
+    yaw = nav.yaw.value_interp.reshape((-1,1))
+
+    # Euler triplet
+    eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
+
+    # Position ECEF
+    position_ecef = np.concatenate((x.reshape((-1,1)),y.reshape((-1,1)),z.reshape((-1,1))), axis = 1)
+
+    ##
+
+    # Append the time offset to nav data so that all h5 data is synced to UHI clock
+    hsi_synced_nav_timestamp_rov = nav_timestamp_rov + time_offset
+
+    nav_dict_h5_folders = {'eul_ZYX' : config['HDF.raw_nav']['eul_ZYX'],
+            'position_ecef' : config['HDF.raw_nav']['position'],
+            'nav_timestamp' : config['HDF.raw_nav']['timestamp']}
+
+    # Filling with the following data (all using the same time stamps)
+    invalid_rows = np.isnan(eul_zyx[:,2])
+    nav_dict_h5_data = {'eul_ZYX' : eul_zyx[~invalid_rows],
+            'position_ecef' : position_ecef[~invalid_rows],
+            'nav_timestamp' : hsi_synced_nav_timestamp_rov[~invalid_rows]}
+
+    # Update config object with this info
+    for key, value in nav_dict_h5_folders.items():
+        config.set('HDF.raw_nav', key, value = value)
+    # +
+    write_data_to_h5_file(H5_FILE_PATH, h5_dict_write=nav_dict_h5_folders, h5_dict_data=nav_dict_h5_data)
+
+def altimeter_data_to_point_cloud(nav, config_uhi, lat0, lon0, h0, true_time_hsi):
+    """Converts the pose + altimeter data to a point cloud using the geometry of the range sensor
+
+    :param nav: A Nav object containing UNIX time-stamped position, orientation and range measurements
+    :type nav: Nav object
+    :param config_uhi: A configuration object containing the altimeter's transform (rotation matrix and lever arm)
+    :type config_uhi: Named tuple
+    :param lat0: Latitude for north-east-down linearization
+    :type lat0: float
+    :param lon0: Longitude for north-east-down linearization
+    :type lon0: float
+    :param h0: Latitude for north-east-down linearization
+    :type h0: float
+    :param true_time_hsi: The time stamps of the hyperspectral imager
+    :type true_time_hsi: float
+    :return: point cloud of 
+    :rtype: _type_
+    """
+
+    # Number of altimeter samples
+    n = nav.altitude.value.size
+
+    # Interpolate all navigation data to the time of altimeter data
+    # TODO: avoid common interpolation of yaw, pitch, roll
+    nav.interpolate(time_interp=nav.altitude.time)
+
+    # Create augmented vector allowing 4x4 transformation matrices
+    alt_vec = np.zeros((4, n))
+    alt_vec[2] = nav.altitude.value # Ranges are captured along z-axis (by definition)
+    alt_vec[3] = 1
+
+    # Preallocate transform from altimeter to body frame
+    T_alt_body = np.zeros((4,4))
+    T_alt_body[3,3] = 1
+
+    # User specified altimeter position, orientation on the body
+    R_alt_body = config_uhi.rotation_matrix_alt_to_body
+    t_alt_body = config_uhi.translation_alt_to_body
+
+    # Insert in transormation matrix
+    T_alt_body[:3,:3] = R_alt_body
+    T_alt_body[:3, 3] = t_alt_body
+
+    # Transform ranges to body frame
+    alt_vec_body = np.matmul(T_alt_body.reshape((4,4)), alt_vec)
+
+    # -------------------------Define transformation from body to NED-----------------------------
+    roll = nav.roll.value_interp.reshape((-1,1))
+    pitch = nav.pitch.value_interp.reshape((-1,1))
+    yaw = nav.yaw.value_interp.reshape((-1,1))
+
+    eul_zyx_alt = np.concatenate((roll, pitch, yaw), axis = 1)
+
+
+    lat_alt = nav.lat.value_interp
+    lon_alt = nav.lon.value_interp
+    h_alt = -nav.pos_z.value_interp
+
+    # User specified values
+    lon0 = config_uhi.lon_lat_alt_origin[0]
+    lat0 = config_uhi.lon_lat_alt_origin[1]
+    h0 = config_uhi.lon_lat_alt_origin[2]
+
+    # Transform to local NED for working with vectors
+    north, east, down = pm.geodetic2ned(lat=lat_alt, lon = lon_alt, h = h_alt, lat0 = lat0, lon0=lon0, h0 = h0, deg = True)
+
+    # Account for the motion
+    R_mats_body_ned = RotLib.from_euler("ZYX", np.flip(eul_zyx_alt, axis=1), degrees=True).as_matrix()
+    t_body_ned = np.vstack((north, east, down)).T
+
+    # Set transformation matrices (one for each timestamp)
+    T_body_ned = np.zeros((n, 4,4))
+    T_body_ned[:, 3,3] = 1
+    T_body_ned[:, :3,:3] = R_mats_body_ned
+    T_body_ned[:, :3, 3] = t_body_ned
+
+    # ----------------------------------------------------------------------------------------------
+
+    # Transform ranges to NED
+    alt_vec_ned = np.einsum('ijk, ki->ji', T_body_ned, alt_vec_body)
+
+    # Transpose vectors (just out of preference)
+    altimeter_point_cloud = alt_vec_ned[0:3,:].T
+
+    # Select the points from an appropriate time interval
+    crit_1 = nav.altitude.time < true_time_hsi.max()
+    crit_2 = nav.altitude.time > true_time_hsi.min()
+
+    points_altimeter_transect = altimeter_point_cloud[(crit_1) & (crit_2)]
+
+    # Still the points are given in a form of NED
+
+    # NED is no frame for GIS, but an OK frame for certain vector operations.
+    # The above linearization is only accurate for small surveys such as those in UHI
+
+    return points_altimeter_transect
+
+def point_cloud_to_dem(points, config, resolution_dem, lon0, lat0, h0, method='nearest', smooth_DEM=True):
+    """Converts the sparse point cloud of altimeter data into a digital elevation model.
+
+    :param points: _description_
+    :type points: _type_
+    :param config: _description_
+    :type config: _type_
+    :param resolution_dem: _description_
+    :type resolution_dem: _type_
+    :param lon0: _description_
+    :type lon0: _type_
+    :param lat0: _description_
+    :type lat0: _type_
+    :param h0: _description_
+    :type h0: _type_
+    :param method: _description_, defaults to 'nearest'
+    :type method: str, optional
+    :param smooth_DEM: _description_, defaults to True
+    :type smooth_DEM: bool, optional
+    """
+    # The name of the digital elevation model
+    output_dem_path = config['Absolute Paths']['dem_path']
+
+    # The padding (ensuring that all rays hit the model)
+    pad_xy = float(config['General']['max_ray_length'])
+
+    x_coords = points[:,0]
+    y_coords = points[:,1]
+    z_values = points[:,2]
+
+    #-----------------------------------------------------Transform Extent and determing resolution, geotransform and grid--------------------------------------------------------
+    
+    # Determine the min/max coordinates with padding in the NED plane, and warp to projected grid.
+    x_min, x_max = x_coords.min() - pad_xy, x_coords.max() + pad_xy
+
+    y_min, y_max = y_coords.min() - pad_xy, y_coords.max() + pad_xy
+
+    extent_ned = np.array([[x_min, y_min],
+                          [x_min, y_max],
+                          [x_max, y_min],
+                          [x_max, y_max]])
+
+    # Transform to wgs 84, aka epsg 4326
+    lat_ext, lon_ext, h_ext = pm.ned2geodetic(n = extent_ned[:,0], e = extent_ned[:,1], d = extent_ned[:,1]*0 + z_values.mean(), lat0 = lat0, lon0=lon0, h0 = h0, deg = True)
+    
+    # Transform to desired CRS
+    epsg_wgs84 = 4326
+    dem_epsg = int(config['Coordinate Reference Systems']['dem_epsg'])
+
+    # Define transformer
+    crs_84 = CRS.from_epsg(epsg_wgs84)
+    crs_dem = CRS.from_epsg(dem_epsg)
+    transformer = Transformer.from_crs(crs_84, crs_dem)
+
+    # Transform extent
+    (x, y, z) = transformer.transform(xx=lat_ext, yy=lon_ext, zz=h_ext)
+
+    if crs_dem.is_geographic:
+
+        res_x = resolution_dem*(x.max() - x.min())/(x_max - x_min)
+        res_y = resolution_dem*(y.max() - y.min())/(y_max - y_min)
+        transform = Affine(a = res_y,
+                        b = 0,
+                        c = y.min(),
+                        d = 0,
+                        e = -res_x,
+                        f = x.max())
+        # Setup mesh grid
+        grid_y, grid_x = np.meshgrid(np.arange(y.min(), y.max(), res_y),
+                                np.arange(x.min(), x.max(), res_x))
+    elif crs_dem.is_projected:
+        # North is then Y
+        res_x = resolution_dem*(x.max() - x.min())/(y_max - y_min)
+        res_y = resolution_dem*(y.max() - y.min())/(x_max - x_min)
+        transform = Affine(a = res_x,
+                        b = 0,
+                        c = x.min(),
+                        d = 0,
+                        e = -res_y,
+                        f = y.max())
+        # Setup mesh grid
+        grid_x, grid_y = np.meshgrid(np.arange(x.min(), x.max(), res_x),
+                                np.arange(y.min(), y.max(), res_y))
+    #--------------------------------------------------------------------------------------------------------------------------------------------------------------------
+
+    # ---------------------------------------------------Transform point cloud------------------------------------------------------------------------------------------
+    
+    # Transform to wgs 84, aka epsg 4326
+    lat_pc, lon_pc, h_pc = pm.ned2geodetic(n = points[:,0], e = points[:,1], d = points[:,2], lat0 = lat0, lon0=lon0, h0 = h0, deg = True)
+    # Transform to target system
+    (x_pc, y_pc, z_pc) = transformer.transform(xx=lat_pc, yy=lon_pc, zz=h_pc)
+
+    points_pc_dem_crs = np.concatenate((x_pc.reshape((-1,1)),
+                                        y_pc.reshape((-1,1)),
+                                        z_pc.reshape((-1,1))), axis = 1)
+    
+
+    # ----------------------------------------------------------------------------------------------------------------------------------------------------------------------
+    
+    # Interpolate z-data to grid
+
+    if method == 'nearest':
+        grid_z = griddata(points_pc_dem_crs[:, :2], points_pc_dem_crs[:,2], (grid_x, grid_y), method='nearest')
+    elif method == 'IDW':
+        import pyinterp
+        mesh = pyinterp.RTree()
+
+        mesh.packing(points_pc_dem_crs[:, :2], points_pc_dem_crs[:,2])
+
+        idw, neighbors = mesh.inverse_distance_weighting(
+        np.vstack((grid_x.ravel(), grid_y.ravel())).T,
+        within=False,  # Extrapolation is forbidden
+        k=11,  # We are looking for at most 11 neighbors
+        num_threads=0)
+
+        grid_z = idw.reshape(grid_x.shape)
+
+
+    if smooth_DEM == True:
+        from scipy import ndimage
+        # Smooths by 4 pixel units
+        sigma_x = 4
+        sigma_y = 4
+        grid_z = ndimage.gaussian_filter(grid_z, sigma=(sigma_y, sigma_x))
+        
+
+    
+    # Writes to a file
+    with rasterio.open(output_dem_path, 'w', driver='GTiff', height=grid_z.shape[0],
+                    width=grid_z.shape[1], count=1, dtype='float64', crs='EPSG:' + str(dem_epsg),
+                    transform=transform) as dst:
+        dst.write(grid_z, 1)
+
+
+
+
+def uhi_beast(config, config_uhi):
+    MISSION_PATH = config['General']['mission_dir'] # Where h5 data is 
+    
+
+    # For writing
+    config_file_path = os.path.join(MISSION_PATH, 'configuration.ini')
+
+    SPATIAL_PIXELS = 1936 # Same for almost all UHI
+    
+
+    INPUT_DIR = MISSION_PATH + 'Input/'
+
+    h5_folder = config['Absolute Paths']['h5_folder']
+    H5_PATTERN = '*.h5'
+
+    MAT_DIR = INPUT_DIR
+    MAT_PATTERN = '*.mat'
+
+    # Locate mat file with nav data 
+    search_path_mat = os.path.normpath(os.path.join(MAT_DIR, MAT_PATTERN))
+    MAT_FILE_PATHS = glob.glob(search_path_mat)
+    MAT_PATH = MAT_FILE_PATHS[0] # Assuming there is only one
+
+    nav = read_nav_from_mat(mat_filename=MAT_PATH)
+
+    
+
+    # Search the h5 folder (these are the files to iterate)
+    search_path_h5 = os.path.normpath(os.path.join(h5_folder, H5_PATTERN))
+    H5_FILE_PATHS = glob.glob(search_path_h5)
+
+    number_of_h5_files = len(H5_FILE_PATHS)
+
+    h5_dict_read = {'radiance_cube': config['HDF.hyperspectral']['datacube'],
+            'hsi_frames_timestamp': config['HDF.hyperspectral']['timestamp'],
+            'fov': config['HDF.calibration']['fov'],
+            'wavelengths' : config['HDF.calibration']['band2wavelength'],
+            #'rgb_frames' : config['HDF.rgb']['rgb_frames'],
+            #'rgb_timestamp' : config['HDF.rgb']['rgb_timestamp']
+            }
+    
+    time_offset = config_uhi.time_offset_sec
+    lon0, lat0, alt0 = config_uhi.lon_lat_alt_origin
+
+    # from gref4hsi.utils.photogrammetry_utils import Photogrammetry
+    # agisoft_object = Photogrammetry(project_folder = MISSION_PATH, software_type='agisoft')
+    # TODO:: Add support for concurrent camera given that images are contained in a h5 folder. 
+    # Should interface towards ODM as well
+
+    for h5_index in range(number_of_h5_files):
+        H5_FILE_PATH = H5_FILE_PATHS[h5_index]
+
+        # Read the specified entries
+        hyp = HyperspectralLite(h5_filename=H5_FILE_PATH, h5_tree_dict=h5_dict_read)
+
+        if h5_index == 0:
+            # Camera model is set once, assuming same spatial binning throughout
+            binning_spatial = int(np.round(SPATIAL_PIXELS/hyp.radiance_cube.shape[1]))
+            # Sets camera model with user specified boresight ...
+            set_camera_model(config=config, 
+                             config_file_path = config_file_path, 
+                             config_uhi=config_uhi, 
+                             model_type = 'cal_txt', 
+                             binning_spatial = binning_spatial)
+
+        true_time_hsi = hyp.hsi_frames_timestamp - time_offset
+
+        # Interpolate nav to roll time, IMU time (considered nav timestamp)
+
+        ## write nav data to h5 file
+        write_nav_data_to_h5(nav, time_offset, config, H5_FILE_PATH)
+        
+        # Build a point cloud
+        point_cloud_altimeter = altimeter_data_to_point_cloud(nav=nav, 
+                                                              config_uhi=config_uhi, 
+                                                              true_time_hsi = true_time_hsi, 
+                                                              lon0=lon0, 
+                                                              lat0=lat0, 
+                                                              h0=alt0)
+        if h5_index == 0:
+            point_cloud_altimeter_total = point_cloud_altimeter
+        else:
+            point_cloud_altimeter_total = np.append(point_cloud_altimeter_total, point_cloud_altimeter, axis = 0)
+        
+
+
+        """# If desirable to write to Agisoft type format
+        if config_uhi.agisoft_process:
+            nav_rgb = nav
+            nav_rgb.interpolate(time_interp=hyp.rgb_timestamp)
+
+            # Prepare for SfM/photogrammetry processing
+            try:
+                agisoft_object.export_rgb_from_h5(h5_folder=H5_FILE_PATH, 
+                                            rgb_image_cube = hyp.rgb_frames, 
+                                            nav_rgb = nav_rgb,
+                                            rgb_write_dir=config['Absolute Paths']['rgbimagedir'],
+                                            pos_acc = np.array([1, 1, 0.05]), 
+                                            rot_acc = np.array([1, 1, 5]))
+            except:
+                pass # If no RGB data, move forward"""
+        
+        
+        
+        print(H5_FILE_PATH)
+    
+    # Use the total point cloud to make a DEM
+    
+
+    if config_uhi.agisoft_process:
+        agisoft_object.load_photos_and_reference()
+
+
+
+
+
+    point_cloud_to_dem(point_cloud_altimeter_total, 
+                                 config, 
+                                 resolution_dem = config_uhi.resolution_dem, 
+                                 lon0=lon0, 
+                                 lat0=lat0, 
+                                 h0=alt0)
+
+
+
+
+def uhi_dbe(config, config_uhi):
+    """Preparing data for the UHI-2x blueye edition (almost copy of beast)
+
+    :param config: _description_
+    :type config: _type_
+    :param config_uhi: _description_
+    :type config_uhi: _type_
+    """
+    MISSION_PATH = config['General']['mission_dir'] # Where h5 data is 
+    
+
+    # For writing
+    config_file_path = os.path.join(MISSION_PATH, 'configuration.ini')
+
+    SPATIAL_PIXELS = 1936 # Same for almost all UHI
+    
+
+    INPUT_DIR = MISSION_PATH + 'Input/'
+
+    h5_folder = config['Absolute Paths']['h5_folder']
+    H5_PATTERN = '*.h5'
+
+    MAT_DIR = INPUT_DIR
+    MAT_PATTERN = '*.mat'
+
+    # Locate mat file with nav data 
+    search_path_mat = os.path.normpath(os.path.join(MAT_DIR, MAT_PATTERN))
+    MAT_FILE_PATHS = glob.glob(search_path_mat)
+    MAT_PATH = MAT_FILE_PATHS[0] # Assuming there is only one
+
+
+    # TODO: replace with how you read in data from DVL/H5 folders
+    nav = read_nav_from_mat(mat_filename=MAT_PATH)
+
+    
+
+    # Search the h5 folder (these are the files to iterate)
+    search_path_h5 = os.path.normpath(os.path.join(h5_folder, H5_PATTERN))
+    H5_FILE_PATHS = glob.glob(search_path_h5)
+
+    number_of_h5_files = len(H5_FILE_PATHS)
+
+    h5_dict_read = {'radiance_cube': config['HDF.hyperspectral']['datacube'],
+            'hsi_frames_timestamp': config['HDF.hyperspectral']['timestamp'],
+            'fov': config['HDF.calibration']['fov'],
+            'wavelengths' : config['HDF.calibration']['band2wavelength'],
+            #'rgb_frames' : config['HDF.rgb']['rgb_frames'],
+            #'rgb_timestamp' : config['HDF.rgb']['rgb_timestamp']
+            }
+    
+    time_offset = config_uhi.time_offset_sec
+    lon0, lat0, alt0 = config_uhi.lon_lat_alt_origin
+
+    # from gref4hsi.utils.photogrammetry_utils import Photogrammetry
+    # agisoft_object = Photogrammetry(project_folder = MISSION_PATH, software_type='agisoft')
+    # TODO:: Add support for concurrent camera given that images are contained in a h5 folder. 
+    # Should interface towards ODM as well
+
+    for h5_index in range(number_of_h5_files):
+        H5_FILE_PATH = H5_FILE_PATHS[h5_index]
+
+        # Read the specified entries
+        hyp = HyperspectralLite(h5_filename=H5_FILE_PATH, h5_tree_dict=h5_dict_read)
+
+        if h5_index == 0:
+            # Camera model is set once, assuming same spatial binning throughout
+            binning_spatial = int(np.round(SPATIAL_PIXELS/hyp.radiance_cube.shape[1]))
+            
+            # Extract from the hyperspectral object
+            fov_arr = hyp.fov
+
+            # Sets camera model with user specified boresight ...
+            set_camera_model(config=config, 
+                             config_file_path = config_file_path, 
+                             config_uhi=config_uhi, 
+                             model_type = 'embedded', 
+                             binning_spatial = binning_spatial,
+                             fov_arr=fov_arr)
+
+        true_time_hsi = hyp.hsi_frames_timestamp - time_offset
+
+        # Interpolate nav to roll time, IMU time (considered nav timestamp)
+
+        ## write nav data to h5 file
+        write_nav_data_to_h5(nav, time_offset, config, H5_FILE_PATH)
+        
+        # Build a point cloud
+        point_cloud_altimeter = altimeter_data_to_point_cloud(nav = nav, 
+                                                              config_uhi=config_uhi, 
+                                                              true_time_hsi = true_time_hsi, 
+                                                              lon0=lon0, 
+                                                              lat0=lat0, 
+                                                              h0=alt0)
+        if h5_index == 0:
+            point_cloud_altimeter_total = point_cloud_altimeter
+        else:
+            point_cloud_altimeter_total = np.append(point_cloud_altimeter_total, point_cloud_altimeter, axis = 0)
+        
+        
+        
+        print(H5_FILE_PATH)
+    
+    # Use the total point cloud to make a DEM
+    
+
+    if config_uhi.agisoft_process:
+        agisoft_object.load_photos_and_reference()
+
+
+
+
+
+    point_cloud_to_dem(point_cloud_altimeter_total, 
+                                 config, 
+                                 resolution_dem = config_uhi.resolution_dem, 
+                                 lon0=lon0, 
+                                 lat0=lat0, 
+                                 h0=alt0)
+
+        
+
```

### Comparing `gref4hsi-0.2.1/gref4hsi/utils/visualize.py` & `gref4hsi-0.2.2/gref4hsi/utils/visualize.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,268 +1,268 @@
-import pyvista as pv
-from pyvistaqt import BackgroundPlotter
-import pandas as pd
-import numpy as np
-from scipy.spatial.transform import Rotation
-import open3d as o3d
-import pymap3d as pm
-# A simple visualization of various types of data
-from gref4hsi.utils.geometry_utils import rotation_matrix_ecef2ned, rotation_matrix_ecef2enu
-
-def show_mesh_camera(config, show_mesh = True, show_pose = True, ref_frame = 'ECEF'):
-    """
-    # Reads the mesh file and pose info, and plots the trajectory next to the mesh.
-
-    :param config: Dictionary-like (configuration) object
-    :return: Nothing
-
-    """
-
-
-    # Todo: encode show mesh camera to use h5-embedded data? Or is this a loss of performance?
-    mesh_path = config['Absolute Paths']['model_path']
-    try:
-        texture_path = config['Absolute Paths']['tex_path']
-    except KeyError:
-        texture_path = None
-        
-    pose_path = config['Absolute Paths']['pose_path']
-
-
-    pose = pd.read_csv(
-        pose_path, sep=',',
-        header=0)
-
-    points_cam_ecef = np.concatenate( (pose[" X"].values.reshape((-1,1)), pose[" Y"].values.reshape((-1,1)), pose[" Z"].values.reshape((-1,1))), axis = 1)
-    use_local = False
-    if use_local == True:
-        eul_cam = np.concatenate((pose[" Yaw"].values.reshape((-1, 1)),
-                                  pose[" Pitch"].values.reshape((-1, 1)),
-                                  pose[" Roll"].values.reshape((-1, 1))), axis=1)
-    else:
-        eul_cam = np.concatenate( (pose[" RotZ"].values.reshape((-1,1)), pose[" RotY"].values.reshape((-1,1)), pose[" RotX"].values.reshape((-1,1))), axis = 1)
-
-
-    R_body_to_ecef = Rotation.from_euler("ZYX", eul_cam, degrees=True)
-    
-
-    # Read the mesh
-    mesh = pv.read(mesh_path)
-    if ref_frame == 'NED':
-        x = np.mean(points_mesh_ecef[:,0])
-        y = np.mean(points_mesh_ecef[:,1])
-        z = np.mean(points_mesh_ecef[:,2])
-        
-        lat0, lon0, hei0 = pm.ecef2geodetic(x, y, z, deg=True)
-        R_ecef_to_ned = Rotation.from_matrix(rotation_matrix_ecef2ned(lon=lon0, lat=lat0))
-
-        R_body_to_ned = R_ecef_to_ned*R_body_to_ecef
-        rotMats = R_body_to_ned.as_matrix()
-
-        points_mesh_ecef = mesh.points
-
-        # Next part is to make a NED
-        x_cam, y_cam, z_cam = pm.ecef2ned(x = points_cam_ecef[:,0], y = points_cam_ecef[:,1], z = points_cam_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
-
-        points_cam = np.concatenate((x_cam.reshape((-1,1)), y_cam.reshape((-1,1)), z_cam.reshape((-1,1))), axis = 1)
-
-        x_mesh, y_mesh, z_mesh = pm.ecef2ned(x = points_mesh_ecef[:,0], y = points_mesh_ecef[:,1], z = points_mesh_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
-
-        points_mesh = np.concatenate((x_mesh.reshape((-1,1)), y_mesh.reshape((-1,1)), z_mesh.reshape((-1,1))), axis = 1)
-
-        mesh.points = points_mesh
-
-
-    elif ref_frame == 'ENU':
-        lat0, lon0, hei0 = pm.ecef2geodetic(x, y, z, deg=True)
-        R_ecef_to_enu = Rotation.from_matrix(rotation_matrix_ecef2enu(lon=lon0, lat=lat0))
-
-        R_body_to_enu = R_ecef_to_enu*R_body_to_ecef
-        rotMats = R_body_to_enu.as_matrix()
-
-        points_mesh_ecef = mesh.points
-
-        # Next part is to make a NED
-        x_cam, y_cam, z_cam = pm.ecef2enu(x = points_cam_ecef[:,0], y = points_cam_ecef[:,1], z = points_cam_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
-
-        points_cam = np.concatenate((x_cam.reshape((-1,1)), y_cam.reshape((-1,1)), z_cam.reshape((-1,1))), axis = 1)
-
-        x_mesh, y_mesh, z_mesh = pm.ecef2enu(x = points_mesh_ecef[:,0], y = points_mesh_ecef[:,1], z = points_mesh_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
-
-        points_mesh = np.concatenate((x_mesh.reshape((-1,1)), y_mesh.reshape((-1,1)), z_mesh.reshape((-1,1))), axis = 1)
-        mesh.points = points_mesh
-    
-    else:
-        rotMats = R_body_to_ecef.as_matrix()
-        points_cam = points_cam_ecef
-
-
-    
-
-    p = BackgroundPlotter(window_size=(600, 400))
-    
-    if show_mesh:
-        if texture_path != None:
-            tex = pv.read_texture(texture_path)
-            p.add_mesh(mesh, texture=tex)
-        else:
-            p.add_mesh(mesh)
-
-    if show_pose:
-        p.add_points(points_cam, render_points_as_spheres=True,
-                        point_size=1)
-        directionX = rotMats[:, :, 0]
-        directionY = rotMats[:, :, 1]
-        directionZ = rotMats[:, :, 2]
-        step = 10
-        scale = np.linalg.norm(np.max(points_cam, axis = 0)-np.min(points_cam, axis = 0), axis=0)
-        p.add_arrows(points_cam[::step], directionX[::step], mag = 0.1*scale, color = 'red')
-        p.add_arrows(points_cam[::step], directionY[::step], mag=0.1*scale, color= 'green')
-        p.add_arrows(points_cam[::step], directionZ[::step], mag=0.1*scale, color= 'blue')
-    p.show()
-    p.app.exec_()
-
-def show_camera_geometry(CameraGeometry, config):
-    mesh_path = config['General']['model_path']
-    texture_path = config['General']['tex_path']
-
-
-
-
-    rotMats = CameraGeometry.rotation_hsi.as_matrix()
-
-    points_cam = CameraGeometry.position_ecef
-
-    mesh = pv.read(mesh_path)
-    tex = pv.read_texture(texture_path)
-
-    p = BackgroundPlotter(window_size=(600, 400))
-
-    p.add_mesh(mesh, texture=tex)
-    p.add_points(points_cam, render_points_as_spheres=True,
-                      point_size=1)
-    directionX = rotMats[:, :, 0]
-    directionY = rotMats[:, :, 1]
-    directionZ = rotMats[:, :, 2]
-    step = 10
-    p.add_arrows(points_cam[::step], directionX[::step], mag = 0.25, color= 'red')
-    p.add_arrows(points_cam[::step], directionY[::step], mag=0.25, color= 'green')
-    p.add_arrows(points_cam[::step], directionZ[::step], mag=0.25, color= 'blue')
-
-
-    # Add direction vectors in cyan to show FOV
-    direction1 = CameraGeometry.rayDirectionsGlobal[:, 0, :]
-    direction2 = CameraGeometry.rayDirectionsGlobal[:, -1, :]
-
-    p.add_arrows(points_cam[::step], direction1[::step], mag=1, color='cyan')
-    p.add_arrows(points_cam[::step], direction2[::step], mag=1, color='yellow')
-
-    p.show()
-    p.app.exec_()
-
-def show_projected_hsi_points(HSICameraGeometry, config, transect_string):
-    mesh_path = config['Absolute Paths']['model_path']
-    
-    point_cloud_path = config['Absolute Paths']['rgb_point_cloud_folder'] + transect_string + '.ply'
-
-    rotMats = HSICameraGeometry.rotation_hsi.as_matrix()
-    points_cam = HSICameraGeometry.position_ecef
-
-    mesh = pv.read(mesh_path)
-
-    try:
-        texture_path = config['Absolute Paths']['tex_path']
-        tex = pv.read_texture(texture_path)
-    except:
-        pass
-    p = BackgroundPlotter(window_size=(600, 400))
-
-    p.add_mesh(mesh)
-    p.add_points(points_cam, render_points_as_spheres=True,
-                 point_size=2, color = 'black')
-    directionX = rotMats[:, :, 0]
-    directionY = rotMats[:, :, 1]
-    directionZ = rotMats[:, :, 2]
-    step = 100
-    p.add_arrows(points_cam[::step], directionX[::step], mag=0.25, color='red')
-    p.add_arrows(points_cam[::step], directionY[::step], mag=0.25, color='green')
-    p.add_arrows(points_cam[::step], directionZ[::step], mag=0.25, color='blue')
-
-    # Add the points from intersections
-    #points_intersection = HSICameraGeometry.projection[::step, ::step, :].reshape((-1,3))
-
-    #p.add_points(points_intersection, render_points_as_spheres=True,
-    #             point_size=1)
-
-
-    pcd = o3d.io.read_point_cloud(point_cloud_path)
-    color_arr = np.asarray(pcd.colors)
-    hyp_pcl = pv.read(point_cloud_path)
-    hyp_pcl['colors'] = color_arr
-    p.add_mesh(hyp_pcl, scalars='colors', rgb=True, point_size=2)
-
-    p.show()
-    p.app.exec_()
-
-def show_point_clouds(pathPcl1, pathPcl2, ind1 = None, ind2 = None, hyp1 = None, hyp2 = None):
-
-    if ind1 == None:
-        p = BackgroundPlotter(window_size=(600, 400))
-        pcd = o3d.io.read_point_cloud(pathPcl1)
-        color_arr = np.asarray(pcd.colors)
-        p.set_background(color='white', top=None)
-        #color_arr[:, 0] = (color_arr[:, 0] - color_arr[:, 0].min()) / (color_arr[:, 0].max() - color_arr[:, 0].min())
-        #color_arr[:, 1] = (color_arr[:, 1] - color_arr[:, 1].min()) / (color_arr[:, 1].max() - color_arr[:, 1].min())
-        #color_arr[:, 2] = (color_arr[:, 2] - color_arr[:, 2].min()) / (color_arr[:, 2].max() - color_arr[:, 2].min())
-        hyp_pcl = pv.read(pathPcl1)
-        hyp_pcl['colors'] = color_arr
-        p.add_mesh(hyp_pcl, scalars='colors', rgb=True, point_size=2)
-
-        pcd = o3d.io.read_point_cloud(pathPcl2)
-        color_arr = np.asarray(pcd.colors)
-
-
-        #color_arr[:, 0] = (color_arr[:, 0] - color_arr[:, 0].min()) / (color_arr[:, 0].max() - color_arr[:, 0].min())
-        #color_arr[:, 1] = (color_arr[:, 1] - color_arr[:, 1].min()) / (color_arr[:, 1].max() - color_arr[:, 1].min())
-        #color_arr[:, 2] = (color_arr[:, 2] - color_arr[:, 2].min()) / (color_arr[:, 2].max() - color_arr[:, 2].min())
-
-        hyp_pcl2 = pv.read(pathPcl2)
-        hyp_pcl2['colors'] = color_arr
-        p.add_mesh(hyp_pcl2, scalars='colors', rgb=True, point_size=2)
-
-        p.add_points(hyp1.position_hsi, render_points_as_spheres=True,
-                     point_size=1)
-        p.add_points(hyp2.position_hsi, render_points_as_spheres=True,
-                     point_size=1)
-
-        p.show()
-        p.app.exec_()
-    else:
-        p = BackgroundPlotter(window_size=(600, 400))
-        pcd = o3d.io.read_point_cloud(pathPcl1)
-        color_arr = np.asarray(pcd.colors)
-        hyp_pcl = pv.read(pathPcl1)
-        hyp_pcl['colors'] = color_arr
-        p.add_mesh(hyp_pcl, scalars='colors', rgb=True, point_size=2)
-
-        pcd = o3d.io.read_point_cloud(pathPcl2)
-        color_arr = np.asarray(pcd.colors)
-        hyp_pcl2 = pv.read(pathPcl2)
-        hyp_pcl2['colors'] = color_arr
-        p.add_mesh(hyp_pcl2, scalars='colors', rgb=True, point_size=2)
-
-        p.show()
-        p.app.exec_()
-
-
-
-
-def main():
-    show_mesh_camera()
-
-
-
-
-if __name__ == '__main__':
-    main()
-
-
+import pyvista as pv
+from pyvistaqt import BackgroundPlotter
+import pandas as pd
+import numpy as np
+from scipy.spatial.transform import Rotation
+import open3d as o3d
+import pymap3d as pm
+# A simple visualization of various types of data
+from gref4hsi.utils.geometry_utils import rotation_matrix_ecef2ned, rotation_matrix_ecef2enu
+
+def show_mesh_camera(config, show_mesh = True, show_pose = True, ref_frame = 'ECEF'):
+    """
+    # Reads the mesh file and pose info, and plots the trajectory next to the mesh.
+
+    :param config: Dictionary-like (configuration) object
+    :return: Nothing
+
+    """
+
+
+    # Todo: encode show mesh camera to use h5-embedded data? Or is this a loss of performance?
+    mesh_path = config['Absolute Paths']['model_path']
+    try:
+        texture_path = config['Absolute Paths']['tex_path']
+    except KeyError:
+        texture_path = None
+        
+    pose_path = config['Absolute Paths']['pose_path']
+
+
+    pose = pd.read_csv(
+        pose_path, sep=',',
+        header=0)
+
+    points_cam_ecef = np.concatenate( (pose[" X"].values.reshape((-1,1)), pose[" Y"].values.reshape((-1,1)), pose[" Z"].values.reshape((-1,1))), axis = 1)
+    use_local = False
+    if use_local == True:
+        eul_cam = np.concatenate((pose[" Yaw"].values.reshape((-1, 1)),
+                                  pose[" Pitch"].values.reshape((-1, 1)),
+                                  pose[" Roll"].values.reshape((-1, 1))), axis=1)
+    else:
+        eul_cam = np.concatenate( (pose[" RotZ"].values.reshape((-1,1)), pose[" RotY"].values.reshape((-1,1)), pose[" RotX"].values.reshape((-1,1))), axis = 1)
+
+
+    R_body_to_ecef = Rotation.from_euler("ZYX", eul_cam, degrees=True)
+    
+
+    # Read the mesh
+    mesh = pv.read(mesh_path)
+    if ref_frame == 'NED':
+        x = np.mean(points_mesh_ecef[:,0])
+        y = np.mean(points_mesh_ecef[:,1])
+        z = np.mean(points_mesh_ecef[:,2])
+        
+        lat0, lon0, hei0 = pm.ecef2geodetic(x, y, z, deg=True)
+        R_ecef_to_ned = Rotation.from_matrix(rotation_matrix_ecef2ned(lon=lon0, lat=lat0))
+
+        R_body_to_ned = R_ecef_to_ned*R_body_to_ecef
+        rotMats = R_body_to_ned.as_matrix()
+
+        points_mesh_ecef = mesh.points
+
+        # Next part is to make a NED
+        x_cam, y_cam, z_cam = pm.ecef2ned(x = points_cam_ecef[:,0], y = points_cam_ecef[:,1], z = points_cam_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
+
+        points_cam = np.concatenate((x_cam.reshape((-1,1)), y_cam.reshape((-1,1)), z_cam.reshape((-1,1))), axis = 1)
+
+        x_mesh, y_mesh, z_mesh = pm.ecef2ned(x = points_mesh_ecef[:,0], y = points_mesh_ecef[:,1], z = points_mesh_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
+
+        points_mesh = np.concatenate((x_mesh.reshape((-1,1)), y_mesh.reshape((-1,1)), z_mesh.reshape((-1,1))), axis = 1)
+
+        mesh.points = points_mesh
+
+
+    elif ref_frame == 'ENU':
+        lat0, lon0, hei0 = pm.ecef2geodetic(x, y, z, deg=True)
+        R_ecef_to_enu = Rotation.from_matrix(rotation_matrix_ecef2enu(lon=lon0, lat=lat0))
+
+        R_body_to_enu = R_ecef_to_enu*R_body_to_ecef
+        rotMats = R_body_to_enu.as_matrix()
+
+        points_mesh_ecef = mesh.points
+
+        # Next part is to make a NED
+        x_cam, y_cam, z_cam = pm.ecef2enu(x = points_cam_ecef[:,0], y = points_cam_ecef[:,1], z = points_cam_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
+
+        points_cam = np.concatenate((x_cam.reshape((-1,1)), y_cam.reshape((-1,1)), z_cam.reshape((-1,1))), axis = 1)
+
+        x_mesh, y_mesh, z_mesh = pm.ecef2enu(x = points_mesh_ecef[:,0], y = points_mesh_ecef[:,1], z = points_mesh_ecef[:,2], lon0=lon0, lat0=lat0, h0=hei0)
+
+        points_mesh = np.concatenate((x_mesh.reshape((-1,1)), y_mesh.reshape((-1,1)), z_mesh.reshape((-1,1))), axis = 1)
+        mesh.points = points_mesh
+    
+    else:
+        rotMats = R_body_to_ecef.as_matrix()
+        points_cam = points_cam_ecef
+
+
+    
+
+    p = BackgroundPlotter(window_size=(600, 400))
+    
+    if show_mesh:
+        if texture_path != None:
+            tex = pv.read_texture(texture_path)
+            p.add_mesh(mesh, texture=tex)
+        else:
+            p.add_mesh(mesh)
+
+    if show_pose:
+        p.add_points(points_cam, render_points_as_spheres=True,
+                        point_size=1)
+        directionX = rotMats[:, :, 0]
+        directionY = rotMats[:, :, 1]
+        directionZ = rotMats[:, :, 2]
+        step = 10
+        scale = np.linalg.norm(np.max(points_cam, axis = 0)-np.min(points_cam, axis = 0), axis=0)
+        p.add_arrows(points_cam[::step], directionX[::step], mag = 0.1*scale, color = 'red')
+        p.add_arrows(points_cam[::step], directionY[::step], mag=0.1*scale, color= 'green')
+        p.add_arrows(points_cam[::step], directionZ[::step], mag=0.1*scale, color= 'blue')
+    p.show()
+    p.app.exec_()
+
+def show_camera_geometry(CameraGeometry, config):
+    mesh_path = config['General']['model_path']
+    texture_path = config['General']['tex_path']
+
+
+
+
+    rotMats = CameraGeometry.rotation_hsi.as_matrix()
+
+    points_cam = CameraGeometry.position_ecef
+
+    mesh = pv.read(mesh_path)
+    tex = pv.read_texture(texture_path)
+
+    p = BackgroundPlotter(window_size=(600, 400))
+
+    p.add_mesh(mesh, texture=tex)
+    p.add_points(points_cam, render_points_as_spheres=True,
+                      point_size=1)
+    directionX = rotMats[:, :, 0]
+    directionY = rotMats[:, :, 1]
+    directionZ = rotMats[:, :, 2]
+    step = 10
+    p.add_arrows(points_cam[::step], directionX[::step], mag = 0.25, color= 'red')
+    p.add_arrows(points_cam[::step], directionY[::step], mag=0.25, color= 'green')
+    p.add_arrows(points_cam[::step], directionZ[::step], mag=0.25, color= 'blue')
+
+
+    # Add direction vectors in cyan to show FOV
+    direction1 = CameraGeometry.rayDirectionsGlobal[:, 0, :]
+    direction2 = CameraGeometry.rayDirectionsGlobal[:, -1, :]
+
+    p.add_arrows(points_cam[::step], direction1[::step], mag=1, color='cyan')
+    p.add_arrows(points_cam[::step], direction2[::step], mag=1, color='yellow')
+
+    p.show()
+    p.app.exec_()
+
+def show_projected_hsi_points(HSICameraGeometry, config, transect_string):
+    mesh_path = config['Absolute Paths']['model_path']
+    
+    point_cloud_path = config['Absolute Paths']['rgb_point_cloud_folder'] + transect_string + '.ply'
+
+    rotMats = HSICameraGeometry.rotation_hsi.as_matrix()
+    points_cam = HSICameraGeometry.position_ecef
+
+    mesh = pv.read(mesh_path)
+
+    try:
+        texture_path = config['Absolute Paths']['tex_path']
+        tex = pv.read_texture(texture_path)
+    except:
+        pass
+    p = BackgroundPlotter(window_size=(600, 400))
+
+    p.add_mesh(mesh)
+    p.add_points(points_cam, render_points_as_spheres=True,
+                 point_size=2, color = 'black')
+    directionX = rotMats[:, :, 0]
+    directionY = rotMats[:, :, 1]
+    directionZ = rotMats[:, :, 2]
+    step = 100
+    p.add_arrows(points_cam[::step], directionX[::step], mag=0.25, color='red')
+    p.add_arrows(points_cam[::step], directionY[::step], mag=0.25, color='green')
+    p.add_arrows(points_cam[::step], directionZ[::step], mag=0.25, color='blue')
+
+    # Add the points from intersections
+    #points_intersection = HSICameraGeometry.projection[::step, ::step, :].reshape((-1,3))
+
+    #p.add_points(points_intersection, render_points_as_spheres=True,
+    #             point_size=1)
+
+
+    pcd = o3d.io.read_point_cloud(point_cloud_path)
+    color_arr = np.asarray(pcd.colors)
+    hyp_pcl = pv.read(point_cloud_path)
+    hyp_pcl['colors'] = color_arr
+    p.add_mesh(hyp_pcl, scalars='colors', rgb=True, point_size=2)
+
+    p.show()
+    p.app.exec_()
+
+def show_point_clouds(pathPcl1, pathPcl2, ind1 = None, ind2 = None, hyp1 = None, hyp2 = None):
+
+    if ind1 == None:
+        p = BackgroundPlotter(window_size=(600, 400))
+        pcd = o3d.io.read_point_cloud(pathPcl1)
+        color_arr = np.asarray(pcd.colors)
+        p.set_background(color='white', top=None)
+        #color_arr[:, 0] = (color_arr[:, 0] - color_arr[:, 0].min()) / (color_arr[:, 0].max() - color_arr[:, 0].min())
+        #color_arr[:, 1] = (color_arr[:, 1] - color_arr[:, 1].min()) / (color_arr[:, 1].max() - color_arr[:, 1].min())
+        #color_arr[:, 2] = (color_arr[:, 2] - color_arr[:, 2].min()) / (color_arr[:, 2].max() - color_arr[:, 2].min())
+        hyp_pcl = pv.read(pathPcl1)
+        hyp_pcl['colors'] = color_arr
+        p.add_mesh(hyp_pcl, scalars='colors', rgb=True, point_size=2)
+
+        pcd = o3d.io.read_point_cloud(pathPcl2)
+        color_arr = np.asarray(pcd.colors)
+
+
+        #color_arr[:, 0] = (color_arr[:, 0] - color_arr[:, 0].min()) / (color_arr[:, 0].max() - color_arr[:, 0].min())
+        #color_arr[:, 1] = (color_arr[:, 1] - color_arr[:, 1].min()) / (color_arr[:, 1].max() - color_arr[:, 1].min())
+        #color_arr[:, 2] = (color_arr[:, 2] - color_arr[:, 2].min()) / (color_arr[:, 2].max() - color_arr[:, 2].min())
+
+        hyp_pcl2 = pv.read(pathPcl2)
+        hyp_pcl2['colors'] = color_arr
+        p.add_mesh(hyp_pcl2, scalars='colors', rgb=True, point_size=2)
+
+        p.add_points(hyp1.position_hsi, render_points_as_spheres=True,
+                     point_size=1)
+        p.add_points(hyp2.position_hsi, render_points_as_spheres=True,
+                     point_size=1)
+
+        p.show()
+        p.app.exec_()
+    else:
+        p = BackgroundPlotter(window_size=(600, 400))
+        pcd = o3d.io.read_point_cloud(pathPcl1)
+        color_arr = np.asarray(pcd.colors)
+        hyp_pcl = pv.read(pathPcl1)
+        hyp_pcl['colors'] = color_arr
+        p.add_mesh(hyp_pcl, scalars='colors', rgb=True, point_size=2)
+
+        pcd = o3d.io.read_point_cloud(pathPcl2)
+        color_arr = np.asarray(pcd.colors)
+        hyp_pcl2 = pv.read(pathPcl2)
+        hyp_pcl2['colors'] = color_arr
+        p.add_mesh(hyp_pcl2, scalars='colors', rgb=True, point_size=2)
+
+        p.show()
+        p.app.exec_()
+
+
+
+
+def main():
+    show_mesh_camera()
+
+
+
+
+if __name__ == '__main__':
+    main()
+
+
```

### Comparing `gref4hsi-0.2.1/gref4hsi.egg-info/PKG-INFO` & `gref4hsi-0.2.2/gref4hsi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,333 +1,333 @@
-Metadata-Version: 2.1
-Name: gref4hsi
-Version: 0.2.1
-Summary: A Python package for for georeferencing and orthorectifying hyperspectral imagery
-Home-page: https://github.com/havardlovas/gref4hsi
-Author: Haavard Snefjellaa Loevaas
-Author-email: havard.s.lovas@ntnu.no
-License: EUPL-1.2
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE.MD
-Requires-Dist: opencv-python
-Requires-Dist: dill
-Requires-Dist: geopandas
-Requires-Dist: h5py
-Requires-Dist: matplotlib
-Requires-Dist: numpy
-Requires-Dist: open3d
-Requires-Dist: pandas
-Requires-Dist: Pillow
-Requires-Dist: pymap3d
-Requires-Dist: pyproj
-Requires-Dist: pyvista
-Requires-Dist: pyvistaqt
-Requires-Dist: scikit-learn
-Requires-Dist: scipy
-Requires-Dist: shapely
-Requires-Dist: spectral
-Requires-Dist: xmltodict
-Requires-Dist: pykdtree
-Requires-Dist: trimesh
-Requires-Dist: rtree
-Requires-Dist: embreex
-Requires-Dist: ephem
-
-# gref4hsi - a toolchain for the georeferencing and orthorectification of hyperspectral pushbroom data. 
-This software was made with a special emphasis on georeferencing and orthorectification of hyperspectral imagery from drones and underwater robots. However, it is equally simple to use for airborne data, and probably even for satellite imagery (although modified approaches including analytical ellipsoid intersection may be better). There is also a coregistration module (at beta stage) which, given an accurate RGB orthomosaic, can optimize geometric parameters (static or time-varying) to align the data.
-The functionality in bullet form is:
-* georeference.py: The software currently supports direct georeferencing through CPU-accelerated ray tracing of push broom measurements onto terrain files including 3D triangular meshes (\*.ply), 2.5D raster DEM/DSM (e.g. \*.tif) and geoid models.
-* orthorectification.py: The software performs orthorectification (a form of image resampling) to any user specified projection (by EPSG code) and resolution. The default resampling strategy is north-east oriented rasters, but the software does support memory-optimally oriented rasters (smallest bounding rectangle). When you resample, you essentially figure out where to put measurements in a geographic grid. In the software, we resample the data cube, an RGB composite of the cube, but also ancillary data like intersection/sun geometries, pixel coordinates (in spatial dimension of imager) and timestamps.
-* coregistration.py: Given a reference RGB orthomosaic (e.g. from photo-matching) covering the area of the hyperspectral image, the coregistration module does SIFT-matching with the RGB composite (handling any differences in projection and raster transforms). The module also has an optimization component for using the matches to minimize the reprojection error. The user can select/toggle which parameters to optimize, including boresight angles, lever arms, camera model parameters or time-varying errors in position/orientation. Notably the module requires that the pixel-coordinates and timestamps are resampled, as done automatically in the orthorectification step.
-
-This README is a bit verbose, but is meant to act as a "tutorial" as well, and I recommend trying to understand as much as possible.
-
-## Installation instructions for Linux:
-The easiest approach is to use conda/mamba to get gdal and pip to install the package with the following commands (has been tested for python 3.8-3.10):
-```
-conda create -n my_env python=3.10 gdal rasterio
-conda activate my_env
-pip install gref4hsi 
-```
-
-## Installation instructions for Windows:
-Seamless installation for windows is, to my experience a bit more challenging because of gdal and rasterio. For python 3.10 you could run
-```
-conda create -n my_env python=3.10
-conda activate my_env
-pip install GDAL‑3.4.3‑cp310‑cp310‑win_amd64.whl
-pip install rasterio‑1.2.10‑cp310‑cp310‑win_amd64.whl
-pip install gref4hsi 
-```
-The wheel files are provided at [Christoph Gohlke's page](https://www.lfd.uci.edu/~gohlke/pythonlibs/). Examples for python 3.8 are given in the dependencies folder of the Github repo.
-
-## Getting started:
-To run the code you will most likely need to re-format your raw acquired hyperspectral data and navigation data. To start with I'd recommend creating a top folder "<mission_dir>" (e.g. a folder "/processed" under your sensor-proprietary raw data). An example is shown below.
-
-```
-<mission_dir>/
-├── configuration.ini
-├── Input
-│   ├── Calib
-│   │   └── HSI_2b.xml
-│   └── H5
-│       ├── 2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
-│       ├── 2022-08-31_0800_HSI_transectnr_0_chunknr_1.h5
-│       ├── 2022-08-31_0800_HSI_transectnr_1_chunknr_0.h5
-```
-
-
-You minimally need the following to successfully run georeferencing: a configuration file ("\*.ini"), a terrain model, a camera model ("\*.xml") and h5/hdf file (datacube + navigation data). To appropriately format/create these, I recommend creating a parser. An example parser for a specim hyperspectral imager + navigation system is added under gref4hsi/utils/specim_parsing_utils.py
-
-### Configuration file ("\*.ini"). 
-It is recommended to just go with the template and maybe change a few minor things, depending on need. A template is given in the Github repo under data/config_examples/configuration_template.ini. The file contains comments describing the entries. Take a careful look at all comments containing "Change" as these are relevant to adjust depending on your setup. If your imager records h5 data, adjusting the h5 paths (sections 'HDF.xxxx') is relevant too. Morover, we interface with the configuration in a dictionary-style manner:
-
-```
-# Make an object and read the config file for the mission
-config = configparser.ConfigParser()
-config.read(config_file_mission)
-
-# Access a specific configuration, e.g. the calibrated camera model of the imager
-hsi_calib_path = config['Absolute Paths']['hsi_calib_path'] # config[<section>][<config-entry>]
-```
-
-
-### Calibration file ("\*.xml")
-The *.xml file is our chosen camera model file and looks like this:
-```
-<?xml version="1.0" encoding="utf-8"?>
-<calibration>
-    <rx>0.0</rx>
-    <ry>0.0</ry>
-    <rz>-1.5707963267948966</rz>
-    <tx>0</tx>
-    <ty>0</ty>
-    <tz>0</tz>
-    <f>754.9669285377008</f>
-    <cx>255.00991757530994</cx>
-    <k1>-72.31892156971124</k1>
-    <k2>-389.57799574674084</k2>
-    <k3>4.075384496065511</k3>
-    <width>512</width>
-</calibration>
-```
-rx, ry and rz are the boresight angles in radians, while tx, ty and tz are lever arms in the vehicle body frame. They are used to transform vectors from the HSI camera frame to the vehicle body frame through:
-```
-rot_hsi_ref_eul = np.array([rz, ry, rx])
-
-R = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False).as_matrix() # Rotation matrix from HSI to body
-
-t = np.array([tx, ty, tz])
-
-X_hsi = np.array([x, y, z]) # some vector
-
-X_body =  R*X_hsi + t# the vector expressed in the body frame 
-```
-In our computation we use a frame convention akin to the camera frames in computer vision. This means that x-right, y-backward, and z-downward for a well aligned camera. In contrast the vehicle body frame follows the roll-pitch-yaw convention with x-forward, y-starboard, z-downward. This is why the rz is by default $\pm \pi/2$. The easiest if you are unsure of whether your scanner is flipped is to swap the sign rz.
-
-
-
-Moreover, the f represent the camera's focal length in pixels, width is the number of spatial pixels, while cx is the principal pixel. Often cx=(width+1)/2, e.g. if you have 5 pixels u = 1,..,5 the middle pixel is cx=3. In other words, our convention is to assign the cell centres of pixels as whole integers (starting at 1), in contrast to OpenCV which starts at 0.5. The k1, k2 are radial distortion coefficients, while k3 is a tangential coefficient. The camera model is adapted from [Sun et al. (2016)](https://opg.optica.org/ao/fulltext.cfm?uri=ao-55-25-6836&id=348983). Expressing a pixel on an undistorted image plane in the HSI frame is done through
-```
-u = np.random.randint(1, width + 1) # Pixel numbers left to right (value from 1 to width)
-
-# Pinhole part
-x_norm_pinhole = (u - cx) / f
-
-# Distortion part
-x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
-                  k2 * ((u - cx) / 1000) ** 3 + \
-                  k3 * ((u - cx) / 1000) ** 2) / f
-
-x_norm_hsi = x_norm_pinhole + x_norm_nonlin
-
-X_norm_hsi = np.array([x_norm_hsi, 0, 1]) # The pixel ray in the hsi frame
-```
-
-Of course most of these parameters are hard to guess for a HSI and there are two simple ways of finding them. The first way is to ignore distortions and assume you know the angular field of view (AFOV). Then you can calculate:
-
-$$f = \frac{width}{2tan(AFOV/2)}$$
-
-
-Besides that, you set cx=width/2, and remaining k's to zero. 
-
-The second approach to get the camera model is if you have an array describing the FOV (often from the manufacturer). 
-In our example above that would amount to a 512-length array, e.g. in degrees 
-```
-from gref4hsi.specim_parsing_utils import Specim
-
-# FOV array from manufacturer describing the view angle of each pixel
-fov = np.array([-19.1, -19.0 .... 19.0, 19.1]) # Length as number of pixels
-
-# Use static method to convert fov to parameters dictionary equivalent to xml file (with boresights and lever arms to zero)
-param_dict = Specim.fov_2_param(fov = specim_object.view_angles)
-
-# Write to an *.xml file
-param_dict['rz'] = rx
-param_dict['ry'] = ry
-param_dict['rx'] = rz
-
-# Vector from origin of HSI to body origin, expressed in body
-# User set
-t_hsi_body = config_specim.translation_body_to_hsi
-param_dict['tz'] = tx
-param_dict['ty'] = ty
-param_dict['tz'] = tz
-
-# Write dictionary to *.xml file
-CalibHSI(file_name_cal_xml= confic['Absolute Paths']['hsi_calib_path'], 
-                    mode = 'w', 
-                    param_dict = param_dict)
-```
-
-
-
-### Terrain files
-There are three allowable types ("model_export_type" in the configuration file), namely "ply_file" (a.k.a. mesh files), "dem_file" and "geoid". Example geoids are added under data/world/geoids/ including the global egm08 and a norwegian geoid. Your local geoid can probably be found from [geoids](https://www.agisoft.com/downloads/geoids/) or similar. Just ensure you add this path to the 'Absolute Paths' section in the configuration file. Similarly, if you choose "model_export_type = dem_file", you can use a terrain model from from your area as long as you add the path to the file in the 'Absolute Paths'. Remember that if the local terrain (dem file) is given wrt the geoid, you can plus them together in e.g. QGIS or simply add an approximate offset in python with rasterio. This is because the software expects DEMs giving the ellipsoid height of the terrain. Lastly, if the "ply_file", or 3D triangular mesh is the desired option, a path to this file must be added to the config file. It should be fairly easy to use any triangular mesh format even though the option suggests "\*.ply". 
-
-### The h5 files
-This format must comply with the h5 paths in the configuration file. All sections starting with "HDF.xxxx" are related to these paths. I realize that it is inconvenient to transform the format if your recorded data is in NETCDF, ENVI etc, but making this software I chose H5/HDF because of legacy and because of the flexibility of the mini-file system. The input structure (only mandatory entries) of the H5 files under mission_dir/Input/H5 is as follows (printed using h5tree in Linux):  
-```
-2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
-├── processed
-│   └── radiance
-│       ├── calibration
-│       │   ├── geometric # Optional
-│       │   │   └── view_angles
-│       │   ├── radiometric # Only if is_radiance = False
-│       │   │   ├── darkFrame
-│       │   │   └── radiometricFrame
-│       │   └── spectral 
-│       │       ├── band2Wavelength
-│       │       └── fwhm # Optional
-│       ├── dataCube 
-│       ├── exposureTime
-│       └── timestamp
-└── raw
-    └── nav
-        ├── euler_angles
-        ├── position_ecef
-        └── timestamp
-```
-Note that all these paths are parameters in the config file and you will now we will explain how to simply fill in this file tree using the config file. An example of format conversion is given under gref4hsi/utils/specim_parsing_utils.py where the raw format of the specim data and a navigation system is converted and written to the h5 format. The following code is taken from that script and shows how you can write all the necessary data to the appropriate h5 format. Assume that "specim_object" represents an object whose attributes are the datasets, meaning that e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
-
-```
-def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
-    with h5py.File(h5_filename, 'w', libver='latest') as f:
-        for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
-            #print(attribute_name)
-            dset = f.create_dataset(name=h5_hierarchy_item_path, 
-                                            data = getattr(specim_object, attribute_name))
-
-h5_dict_write = {'eul_zyx' : config['HDF.raw_nav']['eul_zyx'],
-            'position_ecef' : config['HDF.raw_nav']['position'],
-            'nav_timestamp' : config['HDF.raw_nav']['timestamp'],
-            'radiance_cube': config['HDF.hyperspectral']['datacube'],
-            't_exp_ms': config['HDF.hyperspectral']['exposuretime'],
-            'hsi_timestamps': config['HDF.hyperspectral']['timestamp'],
-            'view_angles': config['HDF.calibration']['view_angles'], # Optional
-            'wavelengths' : config['HDF.calibration']['band2wavelength'],
-            'fwhm' : config['HDF.calibration']['fwhm'], # Optional
-            'dark_frame' : config['HDF.calibration']['darkframe'], # Optional unless 'is_radiance' is False
-            'radiometric_frame' : config['HDF.calibration']['radiometricframe']} # Optional unless 'is_radiance' is False
-
-# The dictionary is equivalent to the tree view above (assuming configuration_template.ini):
-h5_dict_write = {
-  'eul_zyx':            'raw/nav/euler_angles',
-  'position_ecef':     'raw/nav/position_ecef',
-  'nav_timestamp':     'raw/nav/timestamp',
-  'radiance_cube':    'processed/radiance/dataCube',
-  't_exp_ms':          'processed/radiance/exposureTime',
-  'hsi_timestamps':   'processed/radiance/timestamp',
-  'view_angles':       'processed/radiance/calibration/geometric/view_angles',
-  'wavelengths':       'processed/radiance/calibration/spectral/band2Wavelength',
-  'fwhm':              'processed/radiance/calibration/spectral/fwhm',
-  'dark_frame':        'processed/radiance/calibration/radiometric/darkFrame',
-  'radiometric_frame': 'processed/radiance/calibration/radiometric/radiometricFrame'
-}
-
-# At last, write the data to a h5 file
-# In this case 'specim_object' is an object whoose attributes correspond to the above keys
-# e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write  the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
-specim_object_2_h5_file(h5_filename=h5_filename, h5_tree_dict=h5_dict_write, specim_object=specim_object)
-```
-My recommended approach would be that you create your own modified xxx_parsing_utils.py (feel free to send a pull request) which parses and writes your specific navigation data and hyperspectral data into the format.
-
-The last thing worth mentioning is the navigation data. The aforementioned specim_parsing_utils.py parses navigation data from messages, e.g.
-
-Positions from 
-"$GPGGA,125301.00,6335.47830829,N,00932.34206055,E,2,07,1.7,18.434,M,41.216,M,4.0,0123\*79"
-
-Orientations/attitude from messages like
-"$PASHR,125648.280,322.905,T,0.621,-0.114,,0.034,0.034,0.450,2,3\*1B"
-
-The above data log is read with the method (in the case you have a similar navigation format)
-
-```
-specim_object.read_nav_file(nav_file_path=nav_file_path, date = date_string)
-```
-
-Lastly, the data should be formatted as follows for writing:
-
-```
-import pymap3d as pm
-
-# If your nav system gave you geodetic positions, convert them to earth centered earth fixed (ECEF). Make sure to use ellipsoid height (not height above mean sea level (MSL) aka geoid)
-x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
-
-# Roll pitch yaw are ordered with in an unintuitive attribute name eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
-specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
-
-# The ECEF positions
-specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
-```
-
-Then the "specim_object_2_h5_file" puts the data into the right place.
-
-## Running the processing
-Once the above has been defined the processing can be run with a few lines of code (taken from gref4hsi/tests/test_main_specim.py):
-```
-from gref4hsi.scripts import georeference
-from gref4hsi.scripts import orthorectification
-from gref4hsi.utils import parsing_utils, specim_parsing_utils
-from gref4hsi.scripts import visualize
-
-
-# This function parses raw specim data including (spectral, radiometric, geometric) calibrations and nav data
-# into an h5 file. The nav data is written to "raw/nav/" subfolders, whereas hyperspectral data and calibration data 
-# written to "processed/hyperspectral/" and "processed/calibration/" subfolders. The camera model \*.xml file is also generated.
-# The script must be adapted to other 
-specim_parsing_utils.main(config=config,
-                          config_specim=config_specim_preprocess)
-
-# Interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
-config = parsing_utils.export_pose(config_file_mission)
-
-# Exports model
-parsing_utils.export_model(config_file_mission)
-
-# Georeference the line scans of the hyperspectral imager. Utilizes parsed data
-georeference.main(config_file_mission)
-
-# Orthorectify/resample datacube, RGB-composite and ancillary data
-orthorectification.main(config_file_mission)
-
-# Optional: coregistration
-# Match RGB composite to reference, find features and following data, ground control point (gcp) list, for each feature pair:
-# reference point 3D (from reference), position/orientation of vehicle (using resampled time) and pixel coordinate (using resampled pixel coordinate)
-coregistration.main(config_file_mission, mode='compare')
-
-# The gcp list allows reprojecting reference points and evaluate the reprojection error,
-# which is used to optimize static geometric parameters (e.g. boresight...) or dynamic geometric parameters (time-varying nav errors).
-coregistration.main(config_file_mission, mode='calibrate')
-```
-
+Metadata-Version: 2.1
+Name: gref4hsi
+Version: 0.2.2
+Summary: A Python package for for georeferencing and orthorectifying hyperspectral imagery
+Home-page: https://github.com/havardlovas/gref4hsi
+Author: Haavard Snefjellaa Loevaas
+Author-email: havard.s.lovas@ntnu.no
+License: EUPL-1.2
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE.MD
+Requires-Dist: opencv-python
+Requires-Dist: dill
+Requires-Dist: geopandas
+Requires-Dist: h5py
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: open3d
+Requires-Dist: pandas
+Requires-Dist: Pillow
+Requires-Dist: pymap3d
+Requires-Dist: pyproj
+Requires-Dist: pyvista
+Requires-Dist: pyvistaqt
+Requires-Dist: scikit-learn
+Requires-Dist: scipy
+Requires-Dist: shapely
+Requires-Dist: spectral
+Requires-Dist: xmltodict
+Requires-Dist: pykdtree
+Requires-Dist: trimesh
+Requires-Dist: rtree
+Requires-Dist: embreex
+Requires-Dist: ephem
+
+# gref4hsi - a toolchain for the georeferencing and orthorectification of hyperspectral pushbroom data. 
+This software was made with a special emphasis on georeferencing and orthorectification of hyperspectral imagery from drones and underwater robots. However, it is equally simple to use for airborne data, and probably even for satellite imagery (although modified approaches including analytical ellipsoid intersection may be better). There is also a coregistration module (at beta stage) which, given an accurate RGB orthomosaic, can optimize geometric parameters (static or time-varying) to align the data.
+The functionality in bullet form is:
+* georeference.py: The software currently supports direct georeferencing through CPU-accelerated ray tracing of push broom measurements onto terrain files including 3D triangular meshes (\*.ply), 2.5D raster DEM/DSM (e.g. \*.tif) and geoid models.
+* orthorectification.py: The software performs orthorectification (a form of image resampling) to any user specified projection (by EPSG code) and resolution. The default resampling strategy is north-east oriented rasters, but the software does support memory-optimally oriented rasters (smallest bounding rectangle). When you resample, you essentially figure out where to put measurements in a geographic grid. In the software, we resample the data cube, an RGB composite of the cube, but also ancillary data like intersection/sun geometries, pixel coordinates (in spatial dimension of imager) and timestamps.
+* coregistration.py: Given a reference RGB orthomosaic (e.g. from photo-matching) covering the area of the hyperspectral image, the coregistration module does SIFT-matching with the RGB composite (handling any differences in projection and raster transforms). The module also has an optimization component for using the matches to minimize the reprojection error. The user can select/toggle which parameters to optimize, including boresight angles, lever arms, camera model parameters or time-varying errors in position/orientation. Notably the module requires that the pixel-coordinates and timestamps are resampled, as done automatically in the orthorectification step.
+
+This README is a bit verbose, but is meant to act as a "tutorial" as well, and I recommend trying to understand as much as possible.
+
+## Installation instructions for Linux:
+The easiest approach is to use conda/mamba to get gdal and pip to install the package with the following commands (has been tested for python 3.8-3.10):
+```
+conda create -n my_env python=3.10 gdal rasterio
+conda activate my_env
+pip install gref4hsi 
+```
+
+## Installation instructions for Windows:
+Seamless installation for windows is, to my experience a bit more challenging because of gdal and rasterio. For python 3.10 you could run
+```
+conda create -n my_env python=3.10
+conda activate my_env
+pip install GDALâ€‘3.4.3â€‘cp310â€‘cp310â€‘win_amd64.whl
+pip install rasterioâ€‘1.2.10â€‘cp310â€‘cp310â€‘win_amd64.whl
+pip install gref4hsi 
+```
+The wheel files are provided at [Christoph Gohlke's page](https://www.lfd.uci.edu/~gohlke/pythonlibs/). Examples for python 3.8 are given in the dependencies folder of the Github repo.
+
+## Getting started:
+To run the code you will most likely need to re-format your raw acquired hyperspectral data and navigation data. To start with I'd recommend creating a top folder "<mission_dir>" (e.g. a folder "/processed" under your sensor-proprietary raw data). An example is shown below.
+
+```
+<mission_dir>/
+â”œâ”€â”€ configuration.ini
+â”œâ”€â”€ Input
+â”‚Â Â  â”œâ”€â”€ Calib
+â”‚Â Â  â”‚Â Â  â””â”€â”€ HSI_2b.xml
+â”‚Â Â  â””â”€â”€ H5
+â”‚Â Â      â”œâ”€â”€ 2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
+â”‚Â Â      â”œâ”€â”€ 2022-08-31_0800_HSI_transectnr_0_chunknr_1.h5
+â”‚Â Â      â”œâ”€â”€ 2022-08-31_0800_HSI_transectnr_1_chunknr_0.h5
+```
+
+
+You minimally need the following to successfully run georeferencing: a configuration file ("\*.ini"), a terrain model, a camera model ("\*.xml") and h5/hdf file (datacube + navigation data). To appropriately format/create these, I recommend creating a parser. An example parser for a specim hyperspectral imager + navigation system is added under gref4hsi/utils/specim_parsing_utils.py
+
+### Configuration file ("\*.ini"). 
+It is recommended to just go with the template and maybe change a few minor things, depending on need. A template is given in the Github repo under data/config_examples/configuration_template.ini. The file contains comments describing the entries. Take a careful look at all comments containing "Change" as these are relevant to adjust depending on your setup. If your imager records h5 data, adjusting the h5 paths (sections 'HDF.xxxx') is relevant too. Morover, we interface with the configuration in a dictionary-style manner:
+
+```
+# Make an object and read the config file for the mission
+config = configparser.ConfigParser()
+config.read(config_file_mission)
+
+# Access a specific configuration, e.g. the calibrated camera model of the imager
+hsi_calib_path = config['Absolute Paths']['hsi_calib_path'] # config[<section>][<config-entry>]
+```
+
+
+### Calibration file ("\*.xml")
+The *.xml file is our chosen camera model file and looks like this:
+```
+<?xml version="1.0" encoding="utf-8"?>
+<calibration>
+    <rx>0.0</rx>
+    <ry>0.0</ry>
+    <rz>-1.5707963267948966</rz>
+    <tx>0</tx>
+    <ty>0</ty>
+    <tz>0</tz>
+    <f>754.9669285377008</f>
+    <cx>255.00991757530994</cx>
+    <k1>-72.31892156971124</k1>
+    <k2>-389.57799574674084</k2>
+    <k3>4.075384496065511</k3>
+    <width>512</width>
+</calibration>
+```
+rx, ry and rz are the boresight angles in radians, while tx, ty and tz are lever arms in the vehicle body frame. They are used to transform vectors from the HSI camera frame to the vehicle body frame through:
+```
+rot_hsi_ref_eul = np.array([rz, ry, rx])
+
+R = RotLib.from_euler(seq = 'ZYX', angles = rot_hsi_ref_eul, degrees=False).as_matrix() # Rotation matrix from HSI to body
+
+t = np.array([tx, ty, tz])
+
+X_hsi = np.array([x, y, z]) # some vector
+
+X_body =  R*X_hsi + t# the vector expressed in the body frame 
+```
+In our computation we use a frame convention akin to the camera frames in computer vision. This means that x-right, y-backward, and z-downward for a well aligned camera. In contrast the vehicle body frame follows the roll-pitch-yaw convention with x-forward, y-starboard, z-downward. This is why the rz is by default $\pm \pi/2$. The easiest if you are unsure of whether your scanner is flipped is to swap the sign rz.
+
+
+
+Moreover, the f represent the camera's focal length in pixels, width is the number of spatial pixels, while cx is the principal pixel. Often cx=(width+1)/2, e.g. if you have 5 pixels u = 1,..,5 the middle pixel is cx=3. In other words, our convention is to assign the cell centres of pixels as whole integers (starting at 1), in contrast to OpenCV which starts at 0.5. The k1, k2 are radial distortion coefficients, while k3 is a tangential coefficient. The camera model is adapted from [Sun et al. (2016)](https://opg.optica.org/ao/fulltext.cfm?uri=ao-55-25-6836&id=348983). Expressing a pixel on an undistorted image plane in the HSI frame is done through
+```
+u = np.random.randint(1, width + 1) # Pixel numbers left to right (value from 1 to width)
+
+# Pinhole part
+x_norm_pinhole = (u - cx) / f
+
+# Distortion part
+x_norm_nonlin = -(k1 * ((u - cx) / 1000) ** 5 + \
+                  k2 * ((u - cx) / 1000) ** 3 + \
+                  k3 * ((u - cx) / 1000) ** 2) / f
+
+x_norm_hsi = x_norm_pinhole + x_norm_nonlin
+
+X_norm_hsi = np.array([x_norm_hsi, 0, 1]) # The pixel ray in the hsi frame
+```
+
+Of course most of these parameters are hard to guess for a HSI and there are two simple ways of finding them. The first way is to ignore distortions and assume you know the angular field of view (AFOV). Then you can calculate:
+
+$$f = \frac{width}{2tan(AFOV/2)}$$
+
+
+Besides that, you set cx=width/2, and remaining k's to zero. 
+
+The second approach to get the camera model is if you have an array describing the FOV (often from the manufacturer). 
+In our example above that would amount to a 512-length array, e.g. in degrees 
+```
+from gref4hsi.specim_parsing_utils import Specim
+
+# FOV array from manufacturer describing the view angle of each pixel
+fov = np.array([-19.1, -19.0 .... 19.0, 19.1]) # Length as number of pixels
+
+# Use static method to convert fov to parameters dictionary equivalent to xml file (with boresights and lever arms to zero)
+param_dict = Specim.fov_2_param(fov = specim_object.view_angles)
+
+# Write to an *.xml file
+param_dict['rz'] = rx
+param_dict['ry'] = ry
+param_dict['rx'] = rz
+
+# Vector from origin of HSI to body origin, expressed in body
+# User set
+t_hsi_body = config_specim.translation_body_to_hsi
+param_dict['tz'] = tx
+param_dict['ty'] = ty
+param_dict['tz'] = tz
+
+# Write dictionary to *.xml file
+CalibHSI(file_name_cal_xml= confic['Absolute Paths']['hsi_calib_path'], 
+                    mode = 'w', 
+                    param_dict = param_dict)
+```
+
+
+
+### Terrain files
+There are three allowable types ("model_export_type" in the configuration file), namely "ply_file" (a.k.a. mesh files), "dem_file" and "geoid". Example geoids are added under data/world/geoids/ including the global egm08 and a norwegian geoid. Your local geoid can probably be found from [geoids](https://www.agisoft.com/downloads/geoids/) or similar. Just ensure you add this path to the 'Absolute Paths' section in the configuration file. Similarly, if you choose "model_export_type = dem_file", you can use a terrain model from from your area as long as you add the path to the file in the 'Absolute Paths'. Remember that if the local terrain (dem file) is given wrt the geoid, you can plus them together in e.g. QGIS or simply add an approximate offset in python with rasterio. This is because the software expects DEMs giving the ellipsoid height of the terrain. Lastly, if the "ply_file", or 3D triangular mesh is the desired option, a path to this file must be added to the config file. It should be fairly easy to use any triangular mesh format even though the option suggests "\*.ply". 
+
+### The h5 files
+This format must comply with the h5 paths in the configuration file. All sections starting with "HDF.xxxx" are related to these paths. I realize that it is inconvenient to transform the format if your recorded data is in NETCDF, ENVI etc, but making this software I chose H5/HDF because of legacy and because of the flexibility of the mini-file system. The input structure (only mandatory entries) of the H5 files under mission_dir/Input/H5 is as follows (printed using h5tree in Linux):  
+```
+2022-08-31_0800_HSI_transectnr_0_chunknr_0.h5
+â”œâ”€â”€ processed
+â”‚   â””â”€â”€ radiance
+â”‚       â”œâ”€â”€ calibration
+â”‚       â”‚   â”œâ”€â”€ geometric # Optional
+â”‚       â”‚   â”‚   â””â”€â”€ view_angles
+â”‚       â”‚   â”œâ”€â”€ radiometric # Only if is_radiance = False
+â”‚       â”‚   â”‚   â”œâ”€â”€ darkFrame
+â”‚       â”‚   â”‚   â””â”€â”€ radiometricFrame
+â”‚       â”‚   â””â”€â”€ spectral 
+â”‚       â”‚       â”œâ”€â”€ band2Wavelength
+â”‚       â”‚       â””â”€â”€ fwhm # Optional
+â”‚       â”œâ”€â”€ dataCube 
+â”‚       â”œâ”€â”€ exposureTime
+â”‚       â””â”€â”€ timestamp
+â””â”€â”€ raw
+    â””â”€â”€ nav
+        â”œâ”€â”€ euler_angles
+        â”œâ”€â”€ position_ecef
+        â””â”€â”€ timestamp
+```
+Note that all these paths are parameters in the config file and you will now we will explain how to simply fill in this file tree using the config file. An example of format conversion is given under gref4hsi/utils/specim_parsing_utils.py where the raw format of the specim data and a navigation system is converted and written to the h5 format. The following code is taken from that script and shows how you can write all the necessary data to the appropriate h5 format. Assume that "specim_object" represents an object whose attributes are the datasets, meaning that e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
+
+```
+def specim_object_2_h5_file(h5_filename, h5_tree_dict, specim_object):
+    with h5py.File(h5_filename, 'w', libver='latest') as f:
+        for attribute_name, h5_hierarchy_item_path in h5_tree_dict.items():
+            #print(attribute_name)
+            dset = f.create_dataset(name=h5_hierarchy_item_path, 
+                                            data = getattr(specim_object, attribute_name))
+
+h5_dict_write = {'eul_zyx' : config['HDF.raw_nav']['eul_zyx'],
+            'position_ecef' : config['HDF.raw_nav']['position'],
+            'nav_timestamp' : config['HDF.raw_nav']['timestamp'],
+            'radiance_cube': config['HDF.hyperspectral']['datacube'],
+            't_exp_ms': config['HDF.hyperspectral']['exposuretime'],
+            'hsi_timestamps': config['HDF.hyperspectral']['timestamp'],
+            'view_angles': config['HDF.calibration']['view_angles'], # Optional
+            'wavelengths' : config['HDF.calibration']['band2wavelength'],
+            'fwhm' : config['HDF.calibration']['fwhm'], # Optional
+            'dark_frame' : config['HDF.calibration']['darkframe'], # Optional unless 'is_radiance' is False
+            'radiometric_frame' : config['HDF.calibration']['radiometricframe']} # Optional unless 'is_radiance' is False
+
+# The dictionary is equivalent to the tree view above (assuming configuration_template.ini):
+h5_dict_write = {
+  'eul_zyx':            'raw/nav/euler_angles',
+  'position_ecef':     'raw/nav/position_ecef',
+  'nav_timestamp':     'raw/nav/timestamp',
+  'radiance_cube':    'processed/radiance/dataCube',
+  't_exp_ms':          'processed/radiance/exposureTime',
+  'hsi_timestamps':   'processed/radiance/timestamp',
+  'view_angles':       'processed/radiance/calibration/geometric/view_angles',
+  'wavelengths':       'processed/radiance/calibration/spectral/band2Wavelength',
+  'fwhm':              'processed/radiance/calibration/spectral/fwhm',
+  'dark_frame':        'processed/radiance/calibration/radiometric/darkFrame',
+  'radiometric_frame': 'processed/radiance/calibration/radiometric/radiometricFrame'
+}
+
+# At last, write the data to a h5 file
+# In this case 'specim_object' is an object whoose attributes correspond to the above keys
+# e.g. specim_object.radiance_cube is the 3D datacube, and the method 'specim_object_2_h5_file' will write  the data cube to the h5-path specified in configuration section 'HDF.hyperspectral' by entry 'datacube'
+specim_object_2_h5_file(h5_filename=h5_filename, h5_tree_dict=h5_dict_write, specim_object=specim_object)
+```
+My recommended approach would be that you create your own modified xxx_parsing_utils.py (feel free to send a pull request) which parses and writes your specific navigation data and hyperspectral data into the format.
+
+The last thing worth mentioning is the navigation data. The aforementioned specim_parsing_utils.py parses navigation data from messages, e.g.
+
+Positions from 
+"$GPGGA,125301.00,6335.47830829,N,00932.34206055,E,2,07,1.7,18.434,M,41.216,M,4.0,0123\*79"
+
+Orientations/attitude from messages like
+"$PASHR,125648.280,322.905,T,0.621,-0.114,,0.034,0.034,0.450,2,3\*1B"
+
+The above data log is read with the method (in the case you have a similar navigation format)
+
+```
+specim_object.read_nav_file(nav_file_path=nav_file_path, date = date_string)
+```
+
+Lastly, the data should be formatted as follows for writing:
+
+```
+import pymap3d as pm
+
+# If your nav system gave you geodetic positions, convert them to earth centered earth fixed (ECEF). Make sure to use ellipsoid height (not height above mean sea level (MSL) aka geoid)
+x, y, z = pm.geodetic2ecef(lat = lat, lon = lon, alt = ellipsoid_height, deg=True)
+
+# Roll pitch yaw are ordered with in an unintuitive attribute name eul_zyx. The euler angles with rotation order ZYX are Yaw Pitch Roll
+specim_object.eul_zyx = np.concatenate((roll, pitch, yaw), axis = 1)
+
+# The ECEF positions
+specim_object.position_ecef = np.concatenate((x,y,z), axis = 1)
+```
+
+Then the "specim_object_2_h5_file" puts the data into the right place.
+
+## Running the processing
+Once the above has been defined the processing can be run with a few lines of code (taken from gref4hsi/tests/test_main_specim.py):
+```
+from gref4hsi.scripts import georeference
+from gref4hsi.scripts import orthorectification
+from gref4hsi.utils import parsing_utils, specim_parsing_utils
+from gref4hsi.scripts import visualize
+
+
+# This function parses raw specim data including (spectral, radiometric, geometric) calibrations and nav data
+# into an h5 file. The nav data is written to "raw/nav/" subfolders, whereas hyperspectral data and calibration data 
+# written to "processed/hyperspectral/" and "processed/calibration/" subfolders. The camera model \*.xml file is also generated.
+# The script must be adapted to other 
+specim_parsing_utils.main(config=config,
+                          config_specim=config_specim_preprocess)
+
+# Interpolates and reformats the pose (of the vehicle body) to "processed/nav/" folder.
+config = parsing_utils.export_pose(config_file_mission)
+
+# Exports model
+parsing_utils.export_model(config_file_mission)
+
+# Georeference the line scans of the hyperspectral imager. Utilizes parsed data
+georeference.main(config_file_mission)
+
+# Orthorectify/resample datacube, RGB-composite and ancillary data
+orthorectification.main(config_file_mission)
+
+# Optional: coregistration
+# Match RGB composite to reference, find features and following data, ground control point (gcp) list, for each feature pair:
+# reference point 3D (from reference), position/orientation of vehicle (using resampled time) and pixel coordinate (using resampled pixel coordinate)
+coregistration.main(config_file_mission, mode='compare')
+
+# The gcp list allows reprojecting reference points and evaluate the reprojection error,
+# which is used to optimize static geometric parameters (e.g. boresight...) or dynamic geometric parameters (time-varying nav errors).
+coregistration.main(config_file_mission, mode='calibrate')
+```
+
```

### Comparing `gref4hsi-0.2.1/gref4hsi.egg-info/SOURCES.txt` & `gref4hsi-0.2.2/gref4hsi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 gref4hsi.egg-info/SOURCES.txt
 gref4hsi.egg-info/dependency_links.txt
 gref4hsi.egg-info/requires.txt
 gref4hsi.egg-info/top_level.txt
 gref4hsi/scripts/__init__.py
 gref4hsi/scripts/coregistration.py
 gref4hsi/scripts/georeference.py
+gref4hsi/scripts/georeference.py.orig
 gref4hsi/scripts/orthorectification.py
 gref4hsi/tests/__init__.py
 gref4hsi/tests/specim_process.py
+gref4hsi/tests/specim_process.py.orig
 gref4hsi/tests/test_main_hi.py
 gref4hsi/tests/test_main_uhi.py
 gref4hsi/tests/test_multi_ray_trace.py
 gref4hsi/tests/test_multi_ray_trace_no_pyembree.py
 gref4hsi/utils/__init__.py
 gref4hsi/utils/colours.py
 gref4hsi/utils/config_utils.py
```

### Comparing `gref4hsi-0.2.1/setup.py` & `gref4hsi-0.2.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import pathlib
-import setuptools
-
-setuptools.setup(
-    name='gref4hsi',
-    version='0.2.1',    
-    description='A Python package for for georeferencing and orthorectifying hyperspectral imagery',
-    long_description=pathlib.Path("README.md").read_text(),
-    long_description_content_type = "text/markdown",
-    url='https://github.com/havardlovas/gref4hsi',
-    author='Haavard Snefjellaa Loevaas',
-    author_email='havard.s.lovas@ntnu.no',
-    license='EUPL-1.2',
-    install_requires=[
-        "opencv-python",
-        "dill",
-        "geopandas",
-        "h5py",
-        "matplotlib",
-        "numpy",
-        "open3d",
-        "pandas",
-        "Pillow",
-        "pymap3d",
-        "pyproj",
-        "pyvista",
-        "pyvistaqt",
-        "scikit-learn",
-        "scipy",
-        "shapely",
-        "spectral",
-        "xmltodict",
-        "pykdtree",
-        "trimesh",
-        "rtree",
-        "embreex",
-        "ephem"
-    ],
-
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)',  
-        'Operating System :: Microsoft :: Windows :: Windows 10',        
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-    ],
-    python_requires='>3.7',
-    packages=setuptools.find_packages(),
-    include_package_data=True
-)
+import pathlib
+import setuptools
+
+setuptools.setup(
+    name='gref4hsi',
+    version='0.2.2',    
+    description='A Python package for for georeferencing and orthorectifying hyperspectral imagery',
+    long_description=pathlib.Path("README.md").read_text(),
+    long_description_content_type = "text/markdown",
+    url='https://github.com/havardlovas/gref4hsi',
+    author='Haavard Snefjellaa Loevaas',
+    author_email='havard.s.lovas@ntnu.no',
+    license='EUPL-1.2',
+    install_requires=[
+        "opencv-python",
+        "dill",
+        "geopandas",
+        "h5py",
+        "matplotlib",
+        "numpy",
+        "open3d",
+        "pandas",
+        "Pillow",
+        "pymap3d",
+        "pyproj",
+        "pyvista",
+        "pyvistaqt",
+        "scikit-learn",
+        "scipy",
+        "shapely",
+        "spectral",
+        "xmltodict",
+        "pykdtree",
+        "trimesh",
+        "rtree",
+        "embreex",
+        "ephem"
+    ],
+
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)',  
+        'Operating System :: Microsoft :: Windows :: Windows 10',        
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+    ],
+    python_requires='>3.7',
+    packages=setuptools.find_packages(),
+    include_package_data=True
+)
```

