# Comparing `tmp/operationbattleshipcommonutilities-0.4.7.tar.gz` & `tmp/OperationBattleshipCommonUtilities-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operationbattleshipcommonutilities-0.4.7.tar", last modified: Thu May  2 13:25:17 2024, max compression
+gzip compressed data, was "OperationBattleshipCommonUtilities-0.4.8.tar", last modified: Mon May 13 14:00:15 2024, max compression
```

## Comparing `operationbattleshipcommonutilities-0.4.7.tar` & `OperationBattleshipCommonUtilities-0.4.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 13:25:17.513588 operationbattleshipcommonutilities-0.4.7/
--rw-rw-rw-   0        0        0    11558 2024-03-23 16:54:02.000000 operationbattleshipcommonutilities-0.4.7/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-02 13:25:17.505623 operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/
--rw-rw-rw-   0        0        0     3177 2024-05-02 13:25:17.000000 operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3177 2024-04-29 00:43:47.000000 operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/PKG-INFO-DESKTOP-QHT5QD9
--rw-rw-rw-   0        0        0     1251 2024-05-02 13:25:17.000000 operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 13:25:17.000000 operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-02 13:25:17.000000 operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2024-05-02 13:25:17.000000 operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3177 2024-05-02 13:25:17.508625 operationbattleshipcommonutilities-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     2571 2024-03-08 06:05:09.000000 operationbattleshipcommonutilities-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 13:25:17.503623 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/
--rw-rw-rw-   0        0        0     4579 2024-04-30 13:45:27.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/ApifyJobsCaller.py
--rw-rw-rw-   0        0        0     2601 2024-04-01 21:52:27.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/CandidateRequirementsDao.py
--rw-rw-rw-   0        0        0     6557 2024-04-30 13:36:40.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/CompanyDao.py
--rw-rw-rw-   0        0        0     3143 2024-04-01 21:48:50.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/FailureLogger.py
--rw-rw-rw-   0        0        0     1513 2024-04-01 23:24:18.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/GenaricDatabaseDao.py
--rw-rw-rw-   0        0        0     2219 2024-04-01 21:47:52.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/GeographyHelper.py
--rw-rw-rw-   0        0        0     3365 2024-04-01 21:47:37.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobKeyWordsDao.py
--rw-rw-rw-   0        0        0     5843 2024-05-01 13:34:36.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobPostingDao.py
--rw-rw-rw-   0        0        0     1706 2024-04-01 21:39:48.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobResponsibilitiesDao.py
--rw-rw-rw-   0        0        0     2848 2024-04-01 21:39:04.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobSkillsDao.py
--rw-rw-rw-   0        0        0     1887 2024-05-02 13:23:41.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
--rw-rw-rw-   0        0        0      613 2024-03-12 04:49:56.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/NomicAICaller.py
--rw-rw-rw-   0        0        0     1087 2024-02-15 03:50:23.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/OpenAICaller.py
--rw-rw-rw-   0        0        0     3332 2024-04-23 05:20:23.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/PineConeDatabaseCaller.py
--rw-rw-rw-   0        0        0        0 2024-01-26 02:28:14.000000 operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-02 13:25:17.513588 operationbattleshipcommonutilities-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-05-02 13:24:27.000000 operationbattleshipcommonutilities-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:15.541355 OperationBattleshipCommonUtilities-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:15.537356 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:00:15.000000 OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-13 14:00:15.541355 OperationBattleshipCommonUtilities-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:15.541355 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/ApifyJobsCaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CandidateRequirementsDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CompanyDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CompanyDaoOld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/FailureLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/GenaricDatabaseDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/GeographyHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobKeyWordsDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobPostingDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobResponsibilitiesDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobSkillsDao.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobTitleCategoryClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/NomicAICaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/OpenAICaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/PineConeDatabaseCaller.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:00:15.541355 OperationBattleshipCommonUtilities-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-13 14:00:05.000000 OperationBattleshipCommonUtilities-0.4.8/setup.py
```

### Comparing `operationbattleshipcommonutilities-0.4.7/LICENSE` & `OperationBattleshipCommonUtilities-0.4.8/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/PKG-INFO` & `OperationBattleshipCommonUtilities-0.4.8/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,32 @@
-Metadata-Version: 2.1
-Name: OperationBattleshipCommonUtilities
-Version: 0.4.7
-Summary: Classes and Utilities that are shared in the Operation Battleship Application
-Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
-Author: Matthew Caraway
-Author-email: matthew@CarawayLabs.com
-License: Apache-2.0 license
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: python-dotenv
-Requires-Dist: apify-client
-Requires-Dist: pandas
-Requires-Dist: psycopg2
-Requires-Dist: nomic
-Requires-Dist: openai
-Requires-Dist: pinecone-client
-
-# Common Utilities
-Operation Battleship is spread among several different repositories. We've got the data pipeline and also the microservices deployed to Digital Ocean that provide the job recomendations for the job applicants. In order to follow basic engineering practices and support modular code, we have split out some of the common and shared classes into their own repo. 
-
-## Files and Classes
-Here's a quick list of the files that are in the Common Utilities and a short description for each file.
-
-- ApifyJobsCaller.py
-    This file is the one that interacts directly with the Apify SDK. No other instances of the Apify dependency should exist outside this Python class
-
-- CandidateRequirementsDao.py
-    This Python script is a data access object (DAO) for managing candidate requirements data in a PostgreSQL database. It includes a method for inserting multiple records from a DataFrame into the Candidate_Requirements table in the database. The script uses environment variables for database connection parameters, ensuring secure handling of sensitive data.
-
-- CompanyDao.py
-    This Python script is a data access object (DAO) for managing company data in a PostgreSQL database. It includes methods for checking if a company exists in the database, retrieving a companyâ€™s UUID by its LinkedIn URL, and inserting new company data from a DataFrame into the Companies table.
-
-- FailureLogger.py
-    This Python script is designed to handle and log instances where a Language Learning Model (LLM) fails to generate a well-formed JSON response. It saves the LLM response and the associated job title to disk for later analysis, aiding in the identification of potential issues with job postings.
-
-- GenaricDatabaseDao.py
-    This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
-
-- GeographyHelper.py
-    This Python script, GeographyHelper, is designed to parse and extract city and state information from a given string. It uses regular expressions to match patterns and returns the results as a DataFrame, making it useful for processing and standardizing geographical data.
-
-- JobKeyWordsDao.py
-    This Python script defines a class JobKeyWordsDao that connects to a PostgreSQL database and inserts job keywords from a pandas DataFrame into the â€˜Job_Keywordsâ€™ table. It uses environment variables for secure database access and includes logging for execution tracking.
-
-- JobPostingDao.py
-
-- JobTitleCategoryClassifier.py
-
-- OpenAICaller.py
+# Common Utilities
+Operation Battleship is spread among several different repositories. We've got the data pipeline and also the microservices deployed to Digital Ocean that provide the job recomendations for the job applicants. In order to follow basic engineering practices and support modular code, we have split out some of the common and shared classes into their own repo. 
+
+## Files and Classes
+Here's a quick list of the files that are in the Common Utilities and a short description for each file.
+
+- ApifyJobsCaller.py
+    This file is the one that interacts directly with the Apify SDK. No other instances of the Apify dependency should exist outside this Python class
+
+- CandidateRequirementsDao.py
+    This Python script is a data access object (DAO) for managing candidate requirements data in a PostgreSQL database. It includes a method for inserting multiple records from a DataFrame into the Candidate_Requirements table in the database. The script uses environment variables for database connection parameters, ensuring secure handling of sensitive data.
+
+- CompanyDao.py
+    This Python script is a data access object (DAO) for managing company data in a PostgreSQL database. It includes methods for checking if a company exists in the database, retrieving a company’s UUID by its LinkedIn URL, and inserting new company data from a DataFrame into the Companies table.
+
+- FailureLogger.py
+    This Python script is designed to handle and log instances where a Language Learning Model (LLM) fails to generate a well-formed JSON response. It saves the LLM response and the associated job title to disk for later analysis, aiding in the identification of potential issues with job postings.
+
+- GenaricDatabaseDao.py
+    This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
+
+- GeographyHelper.py
+    This Python script, GeographyHelper, is designed to parse and extract city and state information from a given string. It uses regular expressions to match patterns and returns the results as a DataFrame, making it useful for processing and standardizing geographical data.
+
+- JobKeyWordsDao.py
+    This Python script defines a class JobKeyWordsDao that connects to a PostgreSQL database and inserts job keywords from a pandas DataFrame into the ‘Job_Keywords’ table. It uses environment variables for secure database access and includes logging for execution tracking.
+
+- JobPostingDao.py
+
+- JobTitleCategoryClassifier.py
+
+- OpenAICaller.py
```

### Comparing `operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/PKG-INFO-DESKTOP-QHT5QD9` & `OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,43 @@
-Metadata-Version: 2.1
-Name: OperationBattleshipCommonUtilities
-Version: 0.4.5
-Summary: Classes and Utilities that are shared in the Operation Battleship Application
-Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
-Author: Matthew Caraway
-Author-email: matthew@CarawayLabs.com
-License: Apache-2.0 license
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: python-dotenv
-Requires-Dist: apify-client
-Requires-Dist: pandas
-Requires-Dist: psycopg2
-Requires-Dist: nomic
-Requires-Dist: openai
-Requires-Dist: pinecone-client
-
-# Common Utilities
-Operation Battleship is spread among several different repositories. We've got the data pipeline and also the microservices deployed to Digital Ocean that provide the job recomendations for the job applicants. In order to follow basic engineering practices and support modular code, we have split out some of the common and shared classes into their own repo. 
-
-## Files and Classes
-Here's a quick list of the files that are in the Common Utilities and a short description for each file.
-
-- ApifyJobsCaller.py
-    This file is the one that interacts directly with the Apify SDK. No other instances of the Apify dependency should exist outside this Python class
-
-- CandidateRequirementsDao.py
-    This Python script is a data access object (DAO) for managing candidate requirements data in a PostgreSQL database. It includes a method for inserting multiple records from a DataFrame into the Candidate_Requirements table in the database. The script uses environment variables for database connection parameters, ensuring secure handling of sensitive data.
-
-- CompanyDao.py
-    This Python script is a data access object (DAO) for managing company data in a PostgreSQL database. It includes methods for checking if a company exists in the database, retrieving a companyâ€™s UUID by its LinkedIn URL, and inserting new company data from a DataFrame into the Companies table.
-
-- FailureLogger.py
-    This Python script is designed to handle and log instances where a Language Learning Model (LLM) fails to generate a well-formed JSON response. It saves the LLM response and the associated job title to disk for later analysis, aiding in the identification of potential issues with job postings.
-
-- GenaricDatabaseDao.py
-    This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
-
-- GeographyHelper.py
-    This Python script, GeographyHelper, is designed to parse and extract city and state information from a given string. It uses regular expressions to match patterns and returns the results as a DataFrame, making it useful for processing and standardizing geographical data.
-
-- JobKeyWordsDao.py
-    This Python script defines a class JobKeyWordsDao that connects to a PostgreSQL database and inserts job keywords from a pandas DataFrame into the â€˜Job_Keywordsâ€™ table. It uses environment variables for secure database access and includes logging for execution tracking.
-
-- JobPostingDao.py
-
-- JobTitleCategoryClassifier.py
-
-- OpenAICaller.py
+Metadata-Version: 2.1
+Name: OperationBattleshipCommonUtilities
+Version: 0.4.8
+Summary: Classes and Utilities that are shared in the Operation Battleship Application
+Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
+Author: Matthew Caraway
+Author-email: matthew@CarawayLabs.com
+License: Apache-2.0 license
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Common Utilities
+Operation Battleship is spread among several different repositories. We've got the data pipeline and also the microservices deployed to Digital Ocean that provide the job recomendations for the job applicants. In order to follow basic engineering practices and support modular code, we have split out some of the common and shared classes into their own repo. 
+
+## Files and Classes
+Here's a quick list of the files that are in the Common Utilities and a short description for each file.
+
+- ApifyJobsCaller.py
+    This file is the one that interacts directly with the Apify SDK. No other instances of the Apify dependency should exist outside this Python class
+
+- CandidateRequirementsDao.py
+    This Python script is a data access object (DAO) for managing candidate requirements data in a PostgreSQL database. It includes a method for inserting multiple records from a DataFrame into the Candidate_Requirements table in the database. The script uses environment variables for database connection parameters, ensuring secure handling of sensitive data.
+
+- CompanyDao.py
+    This Python script is a data access object (DAO) for managing company data in a PostgreSQL database. It includes methods for checking if a company exists in the database, retrieving a company’s UUID by its LinkedIn URL, and inserting new company data from a DataFrame into the Companies table.
+
+- FailureLogger.py
+    This Python script is designed to handle and log instances where a Language Learning Model (LLM) fails to generate a well-formed JSON response. It saves the LLM response and the associated job title to disk for later analysis, aiding in the identification of potential issues with job postings.
+
+- GenaricDatabaseDao.py
+    This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
+
+- GeographyHelper.py
+    This Python script, GeographyHelper, is designed to parse and extract city and state information from a given string. It uses regular expressions to match patterns and returns the results as a DataFrame, making it useful for processing and standardizing geographical data.
+
+- JobKeyWordsDao.py
+    This Python script defines a class JobKeyWordsDao that connects to a PostgreSQL database and inserts job keywords from a pandas DataFrame into the ‘Job_Keywords’ table. It uses environment variables for secure database access and includes logging for execution tracking.
+
+- JobPostingDao.py
+
+- JobTitleCategoryClassifier.py
+
+- OpenAICaller.py
```

### Comparing `operationbattleshipcommonutilities-0.4.7/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt` & `OperationBattleshipCommonUtilities-0.4.8/OperationBattleshipCommonUtilities.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 README.md
 setup.py
 OperationBattleshipCommonUtilities.egg-info/PKG-INFO
-OperationBattleshipCommonUtilities.egg-info/PKG-INFO-DESKTOP-QHT5QD9
 OperationBattleshipCommonUtilities.egg-info/SOURCES.txt
 OperationBattleshipCommonUtilities.egg-info/dependency_links.txt
 OperationBattleshipCommonUtilities.egg-info/requires.txt
 OperationBattleshipCommonUtilities.egg-info/top_level.txt
 operation_battleship_common_utilities/ApifyJobsCaller.py
 operation_battleship_common_utilities/CandidateRequirementsDao.py
 operation_battleship_common_utilities/CompanyDao.py
+operation_battleship_common_utilities/CompanyDaoOld.py
 operation_battleship_common_utilities/FailureLogger.py
 operation_battleship_common_utilities/GenaricDatabaseDao.py
 operation_battleship_common_utilities/GeographyHelper.py
 operation_battleship_common_utilities/JobKeyWordsDao.py
 operation_battleship_common_utilities/JobPostingDao.py
 operation_battleship_common_utilities/JobResponsibilitiesDao.py
 operation_battleship_common_utilities/JobSkillsDao.py
```

### Comparing `operationbattleshipcommonutilities-0.4.7/PKG-INFO` & `OperationBattleshipCommonUtilities-0.4.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,43 @@
-Metadata-Version: 2.1
-Name: OperationBattleshipCommonUtilities
-Version: 0.4.7
-Summary: Classes and Utilities that are shared in the Operation Battleship Application
-Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
-Author: Matthew Caraway
-Author-email: matthew@CarawayLabs.com
-License: Apache-2.0 license
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: python-dotenv
-Requires-Dist: apify-client
-Requires-Dist: pandas
-Requires-Dist: psycopg2
-Requires-Dist: nomic
-Requires-Dist: openai
-Requires-Dist: pinecone-client
-
-# Common Utilities
-Operation Battleship is spread among several different repositories. We've got the data pipeline and also the microservices deployed to Digital Ocean that provide the job recomendations for the job applicants. In order to follow basic engineering practices and support modular code, we have split out some of the common and shared classes into their own repo. 
-
-## Files and Classes
-Here's a quick list of the files that are in the Common Utilities and a short description for each file.
-
-- ApifyJobsCaller.py
-    This file is the one that interacts directly with the Apify SDK. No other instances of the Apify dependency should exist outside this Python class
-
-- CandidateRequirementsDao.py
-    This Python script is a data access object (DAO) for managing candidate requirements data in a PostgreSQL database. It includes a method for inserting multiple records from a DataFrame into the Candidate_Requirements table in the database. The script uses environment variables for database connection parameters, ensuring secure handling of sensitive data.
-
-- CompanyDao.py
-    This Python script is a data access object (DAO) for managing company data in a PostgreSQL database. It includes methods for checking if a company exists in the database, retrieving a companyâ€™s UUID by its LinkedIn URL, and inserting new company data from a DataFrame into the Companies table.
-
-- FailureLogger.py
-    This Python script is designed to handle and log instances where a Language Learning Model (LLM) fails to generate a well-formed JSON response. It saves the LLM response and the associated job title to disk for later analysis, aiding in the identification of potential issues with job postings.
-
-- GenaricDatabaseDao.py
-    This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
-
-- GeographyHelper.py
-    This Python script, GeographyHelper, is designed to parse and extract city and state information from a given string. It uses regular expressions to match patterns and returns the results as a DataFrame, making it useful for processing and standardizing geographical data.
-
-- JobKeyWordsDao.py
-    This Python script defines a class JobKeyWordsDao that connects to a PostgreSQL database and inserts job keywords from a pandas DataFrame into the â€˜Job_Keywordsâ€™ table. It uses environment variables for secure database access and includes logging for execution tracking.
-
-- JobPostingDao.py
-
-- JobTitleCategoryClassifier.py
-
-- OpenAICaller.py
+Metadata-Version: 2.1
+Name: OperationBattleshipCommonUtilities
+Version: 0.4.8
+Summary: Classes and Utilities that are shared in the Operation Battleship Application
+Home-page: https://github.com/CarawayLabs/OperationBattleshipCommonUtilities
+Author: Matthew Caraway
+Author-email: matthew@CarawayLabs.com
+License: Apache-2.0 license
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Common Utilities
+Operation Battleship is spread among several different repositories. We've got the data pipeline and also the microservices deployed to Digital Ocean that provide the job recomendations for the job applicants. In order to follow basic engineering practices and support modular code, we have split out some of the common and shared classes into their own repo. 
+
+## Files and Classes
+Here's a quick list of the files that are in the Common Utilities and a short description for each file.
+
+- ApifyJobsCaller.py
+    This file is the one that interacts directly with the Apify SDK. No other instances of the Apify dependency should exist outside this Python class
+
+- CandidateRequirementsDao.py
+    This Python script is a data access object (DAO) for managing candidate requirements data in a PostgreSQL database. It includes a method for inserting multiple records from a DataFrame into the Candidate_Requirements table in the database. The script uses environment variables for database connection parameters, ensuring secure handling of sensitive data.
+
+- CompanyDao.py
+    This Python script is a data access object (DAO) for managing company data in a PostgreSQL database. It includes methods for checking if a company exists in the database, retrieving a company’s UUID by its LinkedIn URL, and inserting new company data from a DataFrame into the Companies table.
+
+- FailureLogger.py
+    This Python script is designed to handle and log instances where a Language Learning Model (LLM) fails to generate a well-formed JSON response. It saves the LLM response and the associated job title to disk for later analysis, aiding in the identification of potential issues with job postings.
+
+- GenaricDatabaseDao.py
+    This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
+
+- GeographyHelper.py
+    This Python script, GeographyHelper, is designed to parse and extract city and state information from a given string. It uses regular expressions to match patterns and returns the results as a DataFrame, making it useful for processing and standardizing geographical data.
+
+- JobKeyWordsDao.py
+    This Python script defines a class JobKeyWordsDao that connects to a PostgreSQL database and inserts job keywords from a pandas DataFrame into the ‘Job_Keywords’ table. It uses environment variables for secure database access and includes logging for execution tracking.
+
+- JobPostingDao.py
+
+- JobTitleCategoryClassifier.py
+
+- OpenAICaller.py
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/ApifyJobsCaller.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/ApifyJobsCaller.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-"""
-
-This Python script, which is the sole interface with the Apify SDK in this project, is designed to fetch job data from the Apify Job Crawler. It contains the ApifyJobsCaller class with methods to execute new job crawlers, retrieve product manager jobs, and fetch all jobs for a given set of companies.
-
-The execute_new_jobs_crawler method is the primary function that interacts with the Apify SDK. It accepts a job title and duration as parameters, prepares the actor input based on the duration, runs the actor, fetches the data, and stores it in a list. The data is then saved to a JSON file in the RawCollections directory.
-
-The get_product_manager_jobs and get_all_jobs_for_companies methods are placeholders for fetching specific job data. The former is intended to retrieve all product manager jobs, while the latter is designed to return all jobs for a given list of companies.
-
-This script uses environment variables for sensitive data like the Apify token, which should be stored in a .env file in the same directory.
-"""
-
-import os
-
-import json
-import logging
-import random
-import string
-from datetime import datetime
-from dotenv import load_dotenv
-from apify_client import ApifyClient
-
-
-load_dotenv('.env')
-
-# Configure logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-
-class ApifyJobsCaller:
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-
-
-    
-    #This function will call the Apify Python SDK and run the job. It requires a job title. 
-    #The expectation is that this is the only function that actually calls the API SDK. 
-    def execute_new_jobs_crawler(self, job_title_name, duration):
-        logging.info(f"Beginning the process for collecting {job_title_name} jobs from Apify Job Crawlerin")
-
-        apifytokenFromEnv = os.getenv("APIFY_CLIENT_TOKEN")  # Ensure correct environment variable name
-        client = ApifyClient(apifytokenFromEnv)
-
-        # Prepare the Actor input based on duration
-        publishedAt = ""  # Default to empty, assuming it handles 'anytime' if not provided
-        if duration == 1:
-            publishedAt = "r86400"  # last 24 hours
-        elif duration == 7: 
-            publishedAt = "r604800"  # last week
-        elif duration == 30:
-            publishedAt = "r2592000"  # last month
-        elif duration == 100:
-            publishedAt = None  # Set to None for clarity, indicating no value
-
-        logging.info(f"Based on the args, we have set publishedAt value for Apify Caller to: {publishedAt}")
-
-        # Prepare the run_input, conditionally adding 'publishedAt' only if it's not None
-        run_input = {
-            "location": "United States",
-            "rows": 1000,
-            "title": job_title_name
-        }
-
-        if publishedAt is not None:
-            run_input["publishedAt"] = publishedAt
-        # Run the Actor and wait for it to finish
-        run = client.actor("BHzefUZlZRKWxkTck").call(run_input=run_input)
-
-        # Fetch the data and store it in a list
-        data_list = []
-        for item in client.dataset(run["defaultDatasetId"]).iterate_items():
-            data_list.append(item)
-
-        # Ensure RawCollections folder exists
-        raw_collections_folder = os.path.join("C:/Users/caraw/OneDrive/Documents/PythonProjects/OperationBattleshipParent/OperationBattleshipDataPipeline/RawCollections")
-
-        os.makedirs(raw_collections_folder, exist_ok=True)
-
-        # Generate file name as a random 4 digit string. Save as json. 
-        randomString = ''.join(random.choices(string.ascii_lowercase, k=4))
-        file_name = f'{randomString}.json'  # Concatenate for the file name
-
-        # Construct the full file path
-        full_file_path = os.path.join(raw_collections_folder, file_name)
-
-        # Write the list to the file in JSON format
-        with open(full_file_path, 'w') as file:
-            json.dump(data_list, file, indent=4)
-
-        logging.info(f"Data saved to {full_file_path}")
-        
-        return full_file_path
-
-
-    #This function gets all of the Product Manager Jobs. 
-    def get_product_manager_jobs(self):
-
-        return
-            
-
-    
-    #When given a collection of company names, find all the jobs open for this company.
-    #Returns a JSON of Jobs from Apify
-    def get_all_jobs_for_companies(self, compmany_dataframe):
-
-        print("You;ve enetered the get all jobs for company method")
-
-        return 
+"""
+
+This Python script, which is the sole interface with the Apify SDK in this project, is designed to fetch job data from the Apify Job Crawler. It contains the ApifyJobsCaller class with methods to execute new job crawlers, retrieve product manager jobs, and fetch all jobs for a given set of companies.
+
+The execute_new_jobs_crawler method is the primary function that interacts with the Apify SDK. It accepts a job title and duration as parameters, prepares the actor input based on the duration, runs the actor, fetches the data, and stores it in a list. The data is then saved to a JSON file in the RawCollections directory.
+
+The get_product_manager_jobs and get_all_jobs_for_companies methods are placeholders for fetching specific job data. The former is intended to retrieve all product manager jobs, while the latter is designed to return all jobs for a given list of companies.
+
+This script uses environment variables for sensitive data like the Apify token, which should be stored in a .env file in the same directory.
+"""
+
+import os
+
+import json
+import logging
+import random
+import string
+from datetime import datetime
+from dotenv import load_dotenv
+from apify_client import ApifyClient
+
+
+load_dotenv('.env')
+
+# Configure logging
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+
+class ApifyJobsCaller:
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+
+
+    
+    #This function will call the Apify Python SDK and run the job. It requires a job title. 
+    #The expectation is that this is the only function that actually calls the API SDK. 
+    def execute_new_jobs_crawler(self, job_title_name, duration):
+        logging.info(f"Beginning the process for collecting {job_title_name} jobs from Apify Job Crawlerin")
+
+        apifytokenFromEnv = os.getenv("APIFY_CLIENT_TOKEN")  # Ensure correct environment variable name
+        client = ApifyClient(apifytokenFromEnv)
+
+        # Prepare the Actor input based on duration
+        publishedAt = ""  # Default to empty, assuming it handles 'anytime' if not provided
+        if duration == 1:
+            publishedAt = "r86400"  # last 24 hours
+        elif duration == 7: 
+            publishedAt = "r604800"  # last week
+        elif duration == 30:
+            publishedAt = "r2592000"  # last month
+        elif duration == 100:
+            publishedAt = None  # Set to None for clarity, indicating no value
+
+        logging.info(f"Based on the args, we have set publishedAt value for Apify Caller to: {publishedAt}")
+
+        # Prepare the run_input, conditionally adding 'publishedAt' only if it's not None
+        run_input = {
+            "location": "United States",
+            "rows": 1000,
+            "title": job_title_name
+        }
+
+        if publishedAt is not None:
+            run_input["publishedAt"] = publishedAt
+        # Run the Actor and wait for it to finish
+        run = client.actor("BHzefUZlZRKWxkTck").call(run_input=run_input)
+
+        # Fetch the data and store it in a list
+        data_list = []
+        for item in client.dataset(run["defaultDatasetId"]).iterate_items():
+            data_list.append(item)
+
+        # Ensure RawCollections folder exists
+        raw_collections_folder = os.path.join("C:/Users/caraw/OneDrive/Documents/PythonProjects/OperationBattleshipParent/OperationBattleshipDataPipeline/RawCollections")
+
+        os.makedirs(raw_collections_folder, exist_ok=True)
+
+        # Generate file name as a random 4 digit string. Save as json. 
+        randomString = ''.join(random.choices(string.ascii_lowercase, k=4))
+        file_name = f'{randomString}.json'  # Concatenate for the file name
+
+        # Construct the full file path
+        full_file_path = os.path.join(raw_collections_folder, file_name)
+
+        # Write the list to the file in JSON format
+        with open(full_file_path, 'w') as file:
+            json.dump(data_list, file, indent=4)
+
+        logging.info(f"Data saved to {full_file_path}")
+        
+        return full_file_path
+
+
+    #This function gets all of the Product Manager Jobs. 
+    def get_product_manager_jobs(self):
+
+        return
+            
+
+    
+    #When given a collection of company names, find all the jobs open for this company.
+    #Returns a JSON of Jobs from Apify
+    def get_all_jobs_for_companies(self, compmany_dataframe):
+
+        print("You;ve enetered the get all jobs for company method")
+
+        return
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/CandidateRequirementsDao.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CandidateRequirementsDao.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-"""
-This Python script is designed to interact with a PostgreSQL database to insert job candidate requirements data. It contains the CandidateRequirementsDao class, which has a method insertRequirementsForJobPosting.
-
-The insertRequirementsForJobPosting method accepts a DataFrame containing multiple records of candidate requirements. Each record is inserted into the Candidate_Requirements table in the database. The method establishes a connection to the database using environment variables, prepares an SQL insert statement, and iterates over the DataFrame to insert each row into the database.
-
-In case of any exceptions during the database operation, the method prints the error message and ensures the database connection is closed.
-
-This script uses environment variables for sensitive data like the host, database name, user, password, and port, which should be stored in a .env file in the same directory. 
-"""
-
-import os
-from datetime import datetime
-import uuid
-import logging
-from dotenv import load_dotenv
-import pandas as pd
-import psycopg2
-
-load_dotenv('.env')
-
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-
-class CandidateRequirementsDao:
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-    def insertRequirementsForJobPosting(self, candidateRequirementsDataFrame):
-        """
-        When given a dataframe that has multiple records, this function will insert each record into the DB. 
-        """
-
-        conn = psycopg2.connect(
-        host=os.getenv("host"),
-        database=os.getenv("database"),
-        user=os.getenv("digitalOcean"),
-        password=os.getenv("password"),
-        port=os.getenv("port")
-        )
-        try:
-            cur = conn.cursor()
-
-            sql_insert_query = "INSERT INTO Candidate_Requirements (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
-
-            for index, row in candidateRequirementsDataFrame.iterrows():
-
-                # Convert UUID to string before insertion
-                job_posting_id_str = str(row['job_posting_id'])
-                unique_id_str = str(row['unique_id'])
-                data = (job_posting_id_str, unique_id_str, row['item'])
-                cur.execute(sql_insert_query, data)
-
-            conn.commit()
-
-            cur.close()
-            conn.close()
-
-            return "Update successful!"
-
-        except Exception as e:
-            logging.error("Database connection error:", e)
-            conn.close()
+"""
+This Python script is designed to interact with a PostgreSQL database to insert job candidate requirements data. It contains the CandidateRequirementsDao class, which has a method insertRequirementsForJobPosting.
+
+The insertRequirementsForJobPosting method accepts a DataFrame containing multiple records of candidate requirements. Each record is inserted into the Candidate_Requirements table in the database. The method establishes a connection to the database using environment variables, prepares an SQL insert statement, and iterates over the DataFrame to insert each row into the database.
+
+In case of any exceptions during the database operation, the method prints the error message and ensures the database connection is closed.
+
+This script uses environment variables for sensitive data like the host, database name, user, password, and port, which should be stored in a .env file in the same directory. 
+"""
+
+import os
+from datetime import datetime
+import uuid
+import logging
+from dotenv import load_dotenv
+import pandas as pd
+import psycopg2
+
+load_dotenv('.env')
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+
+class CandidateRequirementsDao:
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+    def insertRequirementsForJobPosting(self, candidateRequirementsDataFrame):
+        """
+        When given a dataframe that has multiple records, this function will insert each record into the DB. 
+        """
+
+        conn = psycopg2.connect(
+        host=os.getenv("host"),
+        database=os.getenv("database"),
+        user=os.getenv("digitalOcean"),
+        password=os.getenv("password"),
+        port=os.getenv("port")
+        )
+        try:
+            cur = conn.cursor()
+
+            sql_insert_query = "INSERT INTO Candidate_Requirements (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
+
+            for index, row in candidateRequirementsDataFrame.iterrows():
+
+                # Convert UUID to string before insertion
+                job_posting_id_str = str(row['job_posting_id'])
+                unique_id_str = str(row['unique_id'])
+                data = (job_posting_id_str, unique_id_str, row['item'])
+                cur.execute(sql_insert_query, data)
+
+            conn.commit()
+
+            cur.close()
+            conn.close()
+
+            return "Update successful!"
+
+        except Exception as e:
+            logging.error("Database connection error:", e)
+            conn.close()
             return None
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/CompanyDao.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/CompanyDaoOld.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-"""
-This Python script defines a CompanyDao class that provides an interface for interacting with a PostgreSQL database that stores company data. The class includes methods for executing generic SQL commands, retrieving all companies, getting a company’s UUID by its LinkedIn URL, checking if a company exists in the database by its LinkedIn URL, and inserting new company data into the database. The script uses environment variables for secure database connection and includes logging for tracking operations and errors. The CompanyDao class is initialized with no arguments, and each method within the class serves a specific purpose related to the manipulation and retrieval of company data from the database. The script is designed to be used as a data access object in a larger application where company data needs to be stored and retrieved.
-
-"""
-
-import os
-import uuid
-from dotenv import load_dotenv
-import pandas as pd
-import psycopg2
-import logging
-
-load_dotenv()
-
-# Configure logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-
-class CompanyDao:
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-    def genericSQL(sqlString):
-
-        return
-
-
-    """
-    TODO: This function will need actual logic
-    
-    """
-    def get_all_companies():
-
-        companyDataFrame = []
-
-        return companyDataFrame
-    
-    """
-    When given a URL for the Company's LinkedIn Page, we want to get the UUID from the Companies Table. 
-    """
-    def getCompanyUuidByLinkedInUrl(self, companyLinkedinUrl):
-        try:
-            
-            conn = psycopg2.connect(
-                host=os.getenv("host"),
-                database=os.getenv("database"),
-                user=os.getenv("digitalOcean"),  
-                password=os.getenv("password"),
-                port=os.getenv("port")
-            )
-            cur = conn.cursor()
-            
-            cur.execute("SELECT company_id FROM Companies WHERE linkedin_url = %s", (companyLinkedinUrl,))
-            
-            rows = cur.fetchall()
-            
-            cur.close()
-            conn.close()
-
-            if rows:
-                return rows[0][0]  
-            else:
-                logging.error(f"Error in getting Company ID. We always expect an ID in this function. Failed for: {companyLinkedinUrl} ")
-                return None  
-
-        except Exception as e:
-            
-            logging.error("Database connection error:", e)
-            logging.error(f"Database error in CompanyDao.getCompanyUuidByLinkedInUrl for Company at: {companyLinkedinUrl} ")
-            if 'conn' in locals():
-                conn.close()
-            return None
-    
-    """
-    This function will check the company table and determine if this table contains any records with this company URL. 
-
-    """
-    def doesCompanyExist(self, linkedInCompanyUrl):
-        
-        conn = psycopg2.connect(
-            host=os.getenv("host"),
-            database=os.getenv("database"),
-            user=os.getenv("digitalOcean"),
-            password=os.getenv("password"),
-            port=os.getenv("port")
-            )
-        try:
-
-            cur = conn.cursor()
-            
-            cur.execute("SELECT * FROM companies WHERE linkedin_url = %s", (linkedInCompanyUrl, ))    
-            
-            rows = cur.fetchall()
-            cur.close()
-            conn.close()
-
-            return len(rows) > 0
-
-        except Exception as e:
-            
-            logging.error("Database connection error:", e)
-            logging.error(f"Database error in CompanyDao.doesCompanyExist for Company at: {linkedInCompanyUrl} ")           
-            
-            if 'conn' in locals():
-                conn.close()
-            return False  
-    
-
-    def insertCompany(self, companyDataFrame):
-        conn = None
-        try:
-            conn = psycopg2.connect(
-                host=os.getenv("host"),
-                database=os.getenv("database"),
-                user=os.getenv("digitalOcean"),
-                password=os.getenv("password"),
-                port=os.getenv("port")
-            )
-            cur = conn.cursor()
-
-            insert_sql = """
-            INSERT INTO Companies (
-                company_id, company_name, company_website, linkedin_url, industry, 
-                num_employees, ownership_type, about_webpage, careers_page, 
-                home_page_summary, about_page_summary, linkedin_company_summary, 
-                has_datascience, has_product_operations
-            ) VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s)
-            """
-
-            row = companyDataFrame.iloc[0].apply(lambda x: str(x) if isinstance(x, uuid.UUID) else x)
-            cur.execute(insert_sql, tuple(row))
-
-            conn.commit()
-
-            cur.close()
-            conn.close()
-
-            return
-
-        except Exception as e:
-            logging.error("Database connection error:", e)
-            logging.error(f"Database error in CompanyDao.insertCompany for Company at: {companyDataFrame['company_name']} ")  
-            if conn:
-                conn.close()
-            return
-        
-    def getCompanyNameByCompanyId(self, company_id):
-
-        try:
-
-            conn = psycopg2.connect(
-                host=os.getenv("host"),
-                database=os.getenv("database"),
-                user=os.getenv("digitalOcean"),  
-                password=os.getenv("password"),
-                port=os.getenv("port")
-            )
-            
-            cur = conn.cursor()
-            
-            cur.execute("SELECT company_name FROM Companies WHERE company_id = %s", (company_id,))
-            
-            rows = cur.fetchall()
-            
-            cur.close()
-            conn.close()
-
-            if rows:
-                return rows[0][0]  
-            else:
-                logging.error(f"Error in getting Company Name. We always expect an name in this function. Failed for company id: {company_id} ")
-                return None  
-
-        except Exception as e:
-            logging.error("Database connection error:", e)
-            logging.error(f"Database error in CompanyDao.getCompanyNameByCompanyId for Company at: {company_id} ")
-            
-            if 'conn' in locals():
-                conn.close()
-            return None
-
-
-    
+"""
+This Python script defines a CompanyDao class that provides an interface for interacting with a PostgreSQL database that stores company data. The class includes methods for executing generic SQL commands, retrieving all companies, getting a company’s UUID by its LinkedIn URL, checking if a company exists in the database by its LinkedIn URL, and inserting new company data into the database. The script uses environment variables for secure database connection and includes logging for tracking operations and errors. The CompanyDao class is initialized with no arguments, and each method within the class serves a specific purpose related to the manipulation and retrieval of company data from the database. The script is designed to be used as a data access object in a larger application where company data needs to be stored and retrieved.
+
+"""
+
+import os
+import uuid
+from dotenv import load_dotenv
+import pandas as pd
+import psycopg2
+import logging
+
+load_dotenv()
+
+# Configure logging
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+
+class CompanyDao:
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+    def genericSQL(sqlString):
+
+        return
+
+
+    """
+    TODO: This function will need actual logic
+    
+    """
+    def get_all_companies():
+
+        companyDataFrame = []
+
+        return companyDataFrame
+    
+    """
+    When given a URL for the Company's LinkedIn Page, we want to get the UUID from the Companies Table. 
+    """
+    def getCompanyUuidByLinkedInUrl(self, companyLinkedinUrl):
+        try:
+            
+            conn = psycopg2.connect(
+                host=os.getenv("host"),
+                database=os.getenv("database"),
+                user=os.getenv("digitalOcean"),  
+                password=os.getenv("password"),
+                port=os.getenv("port")
+            )
+            cur = conn.cursor()
+            
+            cur.execute("SELECT company_id FROM Companies WHERE linkedin_url = %s", (companyLinkedinUrl,))
+            
+            rows = cur.fetchall()
+            
+            cur.close()
+            conn.close()
+
+            if rows:
+                return rows[0][0]  
+            else:
+                logging.error(f"Error in getting Company ID. We always expect an ID in this function. Failed for: {companyLinkedinUrl} ")
+                return None  
+
+        except Exception as e:
+            
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in CompanyDao.getCompanyUuidByLinkedInUrl for Company at: {companyLinkedinUrl} ")
+            if 'conn' in locals():
+                conn.close()
+            return None
+    
+    """
+    This function will check the company table and determine if this table contains any records with this company URL. 
+
+    """
+    def doesCompanyExist(self, linkedInCompanyUrl):
+        
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+            )
+        try:
+
+            cur = conn.cursor()
+            
+            cur.execute("SELECT * FROM companies WHERE linkedin_url = %s", (linkedInCompanyUrl, ))    
+            
+            rows = cur.fetchall()
+            cur.close()
+            conn.close()
+
+            return len(rows) > 0
+
+        except Exception as e:
+            
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in CompanyDao.doesCompanyExist for Company at: {linkedInCompanyUrl} ")           
+            
+            if 'conn' in locals():
+                conn.close()
+            return False  
+    
+
+    def insertCompany(self, companyDataFrame):
+        conn = None
+        try:
+            conn = psycopg2.connect(
+                host=os.getenv("host"),
+                database=os.getenv("database"),
+                user=os.getenv("digitalOcean"),
+                password=os.getenv("password"),
+                port=os.getenv("port")
+            )
+            cur = conn.cursor()
+
+            insert_sql = """
+            INSERT INTO Companies (
+                company_id, company_name, company_website, linkedin_url, industry, 
+                num_employees, ownership_type, about_webpage, careers_page, 
+                home_page_summary, about_page_summary, linkedin_company_summary, 
+                has_datascience, has_product_operations
+            ) VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s)
+            """
+
+            row = companyDataFrame.iloc[0].apply(lambda x: str(x) if isinstance(x, uuid.UUID) else x)
+            cur.execute(insert_sql, tuple(row))
+
+            conn.commit()
+
+            cur.close()
+            conn.close()
+
+            return
+
+        except Exception as e:
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in CompanyDao.insertCompany for Company at: {companyDataFrame['company_name']} ")  
+            if conn:
+                conn.close()
+            return
+        
+    def getCompanyNameByCompanyId(self, company_id):
+
+        try:
+
+            conn = psycopg2.connect(
+                host=os.getenv("host"),
+                database=os.getenv("database"),
+                user=os.getenv("digitalOcean"),  
+                password=os.getenv("password"),
+                port=os.getenv("port")
+            )
+            
+            cur = conn.cursor()
+            
+            cur.execute("SELECT company_name FROM Companies WHERE company_id = %s", (company_id,))
+            
+            rows = cur.fetchall()
+            
+            cur.close()
+            conn.close()
+
+            if rows:
+                return rows[0][0]  
+            else:
+                logging.error(f"Error in getting Company Name. We always expect an name in this function. Failed for company id: {company_id} ")
+                return None  
+
+        except Exception as e:
+            logging.error("Database connection error:", e)
+            logging.error(f"Database error in CompanyDao.getCompanyNameByCompanyId for Company at: {company_id} ")
+            
+            if 'conn' in locals():
+                conn.close()
+            return None
+
+
+
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/FailureLogger.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/FailureLogger.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-"""
-This Python script defines a FailureLogger class that logs failed responses from a Language Learning Model (LLM) and the associated job record to disk for later analysis. The script is designed to handle situations where the LLM fails to create a well-formed JSON response. In such cases, the LLM response and the job title are saved to disk in a new folder within the ‘llmFailures’ directory. Each new folder is named with a random 5-digit string for uniqueness. The LLM response is saved as a JSON file, and the job record is saved as a CSV file. The script uses environment variables for secure operations and includes logging for tracking operations and errors. The FailureLogger class is initialized with no arguments, and the logFailedLlmJsonResponse method takes two arguments: the job record and the LLM response.
-"""
-
-import os
-import json
-import logging
-import random
-from dotenv import load_dotenv
-import csv
-
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-load_dotenv('.env')
-
-class FailureLogger:
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-        self.base_failure_dir = 'llmFailures'
-        # Ensure the base directory exists
-        if not os.path.exists(self.base_failure_dir):
-            os.makedirs(self.base_failure_dir)
-            logging.info(f"Created base directory for failures: {self.base_failure_dir}")
-
-    def logFailedLlmJsonResponse(self, job_record, languageModelResponse):
-        """
-        We will create a new folder in the llmFailures Folder. The new folder will be a random 5 digit string.
-        In the folder we will save the languageModelResponse as a JSON file. Filename is llmResponse.json
-        In the folder we will save the job_record to CSV. The name is created from the job_record[job_title]
-        """
-        logging.info("Logging information about the failed job posting enrichment to disk.")
-
-        # Generate a random 5-digit string
-        folder_name = ''.join(random.choices('0123456789', k=5))
-        folder_path = os.path.join(self.base_failure_dir, folder_name)
-        
-        # Create the new folder
-        os.makedirs(folder_path, exist_ok=True)
-
-        # Save the languageModelResponse as a JSON file
-        llm_response_path = os.path.join(folder_path, 'llmResponse.json')
-        with open(llm_response_path, 'w') as f:
-            json.dump(languageModelResponse, f, indent=4)
-        logging.info(f"Saved language model response to {llm_response_path}")
-
-        # Convert job_record to CSV and save
-        job_title_safe = ''.join(e for e in job_record['job_title'] if e.isalnum() or e in [' ', '_', '-']).rstrip()
-        job_record_path = os.path.join(folder_path, f"{job_title_safe}.csv")
-        with open(job_record_path, mode='w', newline='', encoding='utf-8') as csvfile:
-            writer = csv.writer(csvfile)
-            writer.writerow(job_record.keys())
-            writer.writerow(job_record.values())
-        logging.info(f"Saved job record to {job_record_path}")
-
-        return 
+"""
+This Python script defines a FailureLogger class that logs failed responses from a Language Learning Model (LLM) and the associated job record to disk for later analysis. The script is designed to handle situations where the LLM fails to create a well-formed JSON response. In such cases, the LLM response and the job title are saved to disk in a new folder within the ‘llmFailures’ directory. Each new folder is named with a random 5-digit string for uniqueness. The LLM response is saved as a JSON file, and the job record is saved as a CSV file. The script uses environment variables for secure operations and includes logging for tracking operations and errors. The FailureLogger class is initialized with no arguments, and the logFailedLlmJsonResponse method takes two arguments: the job record and the LLM response.
+"""
+
+import os
+import json
+import logging
+import random
+from dotenv import load_dotenv
+import csv
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+load_dotenv('.env')
+
+class FailureLogger:
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+        self.base_failure_dir = 'llmFailures'
+        # Ensure the base directory exists
+        if not os.path.exists(self.base_failure_dir):
+            os.makedirs(self.base_failure_dir)
+            logging.info(f"Created base directory for failures: {self.base_failure_dir}")
+
+    def logFailedLlmJsonResponse(self, job_record, languageModelResponse):
+        """
+        We will create a new folder in the llmFailures Folder. The new folder will be a random 5 digit string.
+        In the folder we will save the languageModelResponse as a JSON file. Filename is llmResponse.json
+        In the folder we will save the job_record to CSV. The name is created from the job_record[job_title]
+        """
+        logging.info("Logging information about the failed job posting enrichment to disk.")
+
+        # Generate a random 5-digit string
+        folder_name = ''.join(random.choices('0123456789', k=5))
+        folder_path = os.path.join(self.base_failure_dir, folder_name)
+        
+        # Create the new folder
+        os.makedirs(folder_path, exist_ok=True)
+
+        # Save the languageModelResponse as a JSON file
+        llm_response_path = os.path.join(folder_path, 'llmResponse.json')
+        with open(llm_response_path, 'w') as f:
+            json.dump(languageModelResponse, f, indent=4)
+        logging.info(f"Saved language model response to {llm_response_path}")
+
+        # Convert job_record to CSV and save
+        job_title_safe = ''.join(e for e in job_record['job_title'] if e.isalnum() or e in [' ', '_', '-']).rstrip()
+        job_record_path = os.path.join(folder_path, f"{job_title_safe}.csv")
+        with open(job_record_path, mode='w', newline='', encoding='utf-8') as csvfile:
+            writer = csv.writer(csvfile)
+            writer.writerow(job_record.keys())
+            writer.writerow(job_record.values())
+        logging.info(f"Saved job record to {job_record_path}")
+
+        return
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/GenaricDatabaseDao.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/GenaricDatabaseDao.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-"""
-This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
-
-TODO: Implement this class and update other scripts to call this instead. 
-
-"""
-
-import os
-from datetime import datetime
-import uuid
-import logging
-from dotenv import load_dotenv
-import pandas as pd
-import psycopg2
-
-load_dotenv('.env')
-
-
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-class GenaricDatabaseDao:
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-    def execute_select_command(self, sql_statement):
-        conn = psycopg2.connect(
-            host=os.getenv("host"),
-            database=os.getenv("database"),
-            user=os.getenv("digitalOcean"),
-            password=os.getenv("password"),
-            port=os.getenv("port")
-            )
-        try:
-            cur = conn.cursor()
-            
-            cur.execute(sql_statement)
-
-            rows = cur.fetchall()
-
-            df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
-
-            cur.close()
-            conn.close()
-
-            return df
-
-        except Exception as e:
-            logging.error("Database error:", e)
-            conn.close()
-            return None
-    
-    def execute_update_command(sql_statement, data):
-
-        return
-    
-    def execute_insert_command(sql_statement, data):
-
+"""
+This script is intended to be the only class that actually calls the PostGres DB. All other DAO Classes will reference this Class. 
+
+TODO: Implement this class and update other scripts to call this instead. 
+
+"""
+
+import os
+from datetime import datetime
+import uuid
+import logging
+from dotenv import load_dotenv
+import pandas as pd
+import psycopg2
+
+load_dotenv('.env')
+
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+class GenaricDatabaseDao:
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+    def execute_select_command(self, sql_statement):
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+            )
+        try:
+            cur = conn.cursor()
+            
+            cur.execute(sql_statement)
+
+            rows = cur.fetchall()
+
+            df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
+
+            cur.close()
+            conn.close()
+
+            return df
+
+        except Exception as e:
+            logging.error("Database error:", e)
+            conn.close()
+            return None
+    
+    def execute_update_command(sql_statement, data):
+
+        return
+    
+    def execute_insert_command(sql_statement, data):
+
         return
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/GeographyHelper.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/GeographyHelper.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-"""
-This script defines the GeographyHelper class, which provides functionality for parsing and extracting city and state information from a given string. The class uses regular expressions to match patterns and returns the results as a pandas DataFrame. It is designed to help standardize geographical data for further processing or analysis.
-
-"""
-import logging
-import re
-import pandas as pd
-
-
-
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-class GeographyHelper :
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-
-    def getCityState(self, cityStateString):
-
-        # Regular expression to match the patterns "City, State" or "State, Country"
-        pattern = re.compile(r"([A-Za-z\s\-]+)(?:, )?([A-Z]{2})?")
-
-        # Apply the pattern to the string
-        match = pattern.match(cityStateString)
-
-        # Initialize city and state as None
-        city, state = None, None
-
-        if match:
-            # If the first group (city/region) is a known state or 'United States', set it as state
-            if match.group(1).strip() in ["United States"] or match.group(1).strip() in us_states:
-                state = match.group(1).strip()
-            else:
-                city = match.group(1).strip()
-                state = match.group(2)
-
-        # Return the results as a DataFrame
-        return pd.DataFrame({"city": [city], "state": [state]})
-
-us_states = ["Alabama", "Alaska", "Arizona", "Arkansas", "California", "Colorado",
-            "Connecticut", "Delaware", "Florida", "Georgia", "Hawaii", "Idaho", "Illinois",
-            "Indiana", "Iowa", "Kansas", "Kentucky", "Louisiana", "Maine", "Maryland",
-            "Massachusetts", "Michigan", "Minnesota", "Mississippi", "Missouri", "Montana",
-            "Nebraska", "Nevada", "New Hampshire", "New Jersey", "New Mexico", "New York",
-            "North Carolina", "North Dakota", "Ohio", "Oklahoma", "Oregon", "Pennsylvania",
-            "Rhode Island", "South Carolina", "South Dakota", "Tennessee", "Texas", "Utah",
-            "Vermont", "Virginia", "Washington", "West Virginia", "Wisconsin", "Wyoming"]
+"""
+This script defines the GeographyHelper class, which provides functionality for parsing and extracting city and state information from a given string. The class uses regular expressions to match patterns and returns the results as a pandas DataFrame. It is designed to help standardize geographical data for further processing or analysis.
+
+"""
+import logging
+import re
+import pandas as pd
+
+
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+class GeographyHelper :
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+
+    def getCityState(self, cityStateString):
+
+        # Regular expression to match the patterns "City, State" or "State, Country"
+        pattern = re.compile(r"([A-Za-z\s\-]+)(?:, )?([A-Z]{2})?")
+
+        # Apply the pattern to the string
+        match = pattern.match(cityStateString)
+
+        # Initialize city and state as None
+        city, state = None, None
+
+        if match:
+            # If the first group (city/region) is a known state or 'United States', set it as state
+            if match.group(1).strip() in ["United States"] or match.group(1).strip() in us_states:
+                state = match.group(1).strip()
+            else:
+                city = match.group(1).strip()
+                state = match.group(2)
+
+        # Return the results as a DataFrame
+        return pd.DataFrame({"city": [city], "state": [state]})
+
+us_states = ["Alabama", "Alaska", "Arizona", "Arkansas", "California", "Colorado",
+            "Connecticut", "Delaware", "Florida", "Georgia", "Hawaii", "Idaho", "Illinois",
+            "Indiana", "Iowa", "Kansas", "Kentucky", "Louisiana", "Maine", "Maryland",
+            "Massachusetts", "Michigan", "Minnesota", "Mississippi", "Missouri", "Montana",
+            "Nebraska", "Nevada", "New Hampshire", "New Jersey", "New Mexico", "New York",
+            "North Carolina", "North Dakota", "Ohio", "Oklahoma", "Oregon", "Pennsylvania",
+            "Rhode Island", "South Carolina", "South Dakota", "Tennessee", "Texas", "Utah",
+            "Vermont", "Virginia", "Washington", "West Virginia", "Wisconsin", "Wyoming"]
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobKeyWordsDao.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobKeyWordsDao.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-"""
-This script defines the JobKeyWordsDao class, which provides functionality for inserting job keywords into a database. The class uses the psycopg2 library to connect to a PostgreSQL database and execute SQL queries. It reads job keywords from a pandas DataFrame and inserts each record into the 'Job_Keywords' table in the database. The script uses environment variables to securely access database credentials. Logging is configured for tracking the execution of the script.
-"""
-import os
-from datetime import datetime
-import uuid
-import logging
-from dotenv import load_dotenv
-import pandas as pd
-import psycopg2
-
-load_dotenv('.env')
-
-
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-class JobKeyWordsDao :
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-
-    def insertJobKeyWordsForJobPosting(self, jobKeyWordsDataFrame):
-        """
-        When given a dataframe that has multiple records, this function will insert each record into the DB. 
-        """
-
-        conn = psycopg2.connect(
-            host=os.getenv("host"),
-            database=os.getenv("database"),
-            user=os.getenv("digitalOcean"),
-            password=os.getenv("password"),
-            port=os.getenv("port")
-        )
-        try:
-            cur = conn.cursor()
-
-            sql_insert_query = "INSERT INTO Job_Keywords (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
-
-            for index, row in jobKeyWordsDataFrame.iterrows():
-
-                # Convert UUID to string before insertion
-                job_posting_id_str = str(row['job_posting_id'])
-                unique_id_str = str(row['unique_id'])
-                data = (job_posting_id_str, unique_id_str, row['item'])
-                cur.execute(sql_insert_query, data)
-                
-            
-            conn.commit()
-
-            cur.close()
-            conn.close()
-
-            return "Update successful!"
-
-        except Exception as e:
-            logging.error("Database connection error:", e)
-            conn.close()
-            return None
-        
-
-
-    def getKeywordsForJobID(self, job_posting_id):
-
-        """
-        This function calls the Job Keywords Table to find all the records that have the given job_posting_id 
-        
-        Returns the list as a Pandas DataFrame
-        """
-
-        conn = psycopg2.connect(
-            host=os.getenv("host"),
-            database=os.getenv("database"),
-            user=os.getenv("digitalOcean"),
-            password=os.getenv("password"),
-            port=os.getenv("port")
-        )
-        try:
-
-            cur = conn.cursor()
-            
-            sql_select_query = "SELECT * FROM job_keywords WHERE job_posting_id = %s"
-            cur.execute(sql_select_query, (job_posting_id,))  
-
-            rows = cur.fetchall()
-
-            if rows:
-                df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
-            else:
-                df = pd.DataFrame()
-
-            cur.close()
-            conn.close()
-
-            return df
-
-        except Exception as e:
-            logging.error(f"Database connection error in getSkillsForJobID: {e}")
-            conn.close()
-            return pd.DataFrame()  
+"""
+This script defines the JobKeyWordsDao class, which provides functionality for inserting job keywords into a database. The class uses the psycopg2 library to connect to a PostgreSQL database and execute SQL queries. It reads job keywords from a pandas DataFrame and inserts each record into the 'Job_Keywords' table in the database. The script uses environment variables to securely access database credentials. Logging is configured for tracking the execution of the script.
+"""
+import os
+from datetime import datetime
+import uuid
+import logging
+from dotenv import load_dotenv
+import pandas as pd
+import psycopg2
+
+load_dotenv('.env')
+
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+class JobKeyWordsDao :
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+
+    def insertJobKeyWordsForJobPosting(self, jobKeyWordsDataFrame):
+        """
+        When given a dataframe that has multiple records, this function will insert each record into the DB. 
+        """
+
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+        )
+        try:
+            cur = conn.cursor()
+
+            sql_insert_query = "INSERT INTO Job_Keywords (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
+
+            for index, row in jobKeyWordsDataFrame.iterrows():
+
+                # Convert UUID to string before insertion
+                job_posting_id_str = str(row['job_posting_id'])
+                unique_id_str = str(row['unique_id'])
+                data = (job_posting_id_str, unique_id_str, row['item'])
+                cur.execute(sql_insert_query, data)
+                
+            
+            conn.commit()
+
+            cur.close()
+            conn.close()
+
+            return "Update successful!"
+
+        except Exception as e:
+            logging.error("Database connection error:", e)
+            conn.close()
+            return None
+        
+
+
+    def getKeywordsForJobID(self, job_posting_id):
+
+        """
+        This function calls the Job Keywords Table to find all the records that have the given job_posting_id 
+        
+        Returns the list as a Pandas DataFrame
+        """
+
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+        )
+        try:
+
+            cur = conn.cursor()
+            
+            sql_select_query = "SELECT * FROM job_keywords WHERE job_posting_id = %s"
+            cur.execute(sql_select_query, (job_posting_id,))  
+
+            rows = cur.fetchall()
+
+            if rows:
+                df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
+            else:
+                df = pd.DataFrame()
+
+            cur.close()
+            conn.close()
+
+            return df
+
+        except Exception as e:
+            logging.error(f"Database connection error in getSkillsForJobID: {e}")
+            conn.close()
+            return pd.DataFrame()
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobPostingDao.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobPostingDao.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import os
-from datetime import datetime
-import uuid
-import logging
-from dotenv import load_dotenv
-import pandas as pd
-import psycopg2
-
-load_dotenv('.env')
-
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-class JobPostingDao:
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-    def _get_connection(self):
-        return psycopg2.connect(
-            host=os.getenv("host"),
-            database=os.getenv("database"),
-            user=os.getenv("digitalOcean"),
-            password=os.getenv("password"),
-            port=os.getenv("port")
-        )
-
-    def execute_db_command(self, sql_statement, data=None):
-        conn = self._get_connection()
-        try:
-            cur = conn.cursor()
-            cur.execute(sql_statement, data)
-            if sql_statement.strip().lower().startswith("select"):
-                result = pd.DataFrame(cur.fetchall(), columns=[desc[0] for desc in cur.description])
-            else:
-                conn.commit()
-                result = "Success"
-            cur.close()
-        except Exception as e:
-            logging.error("Database error:", e)
-            result = None
-        finally:
-            conn.close()
-        return result
-
-    def getAllDataScienceOrProductCategorizedJobs(self):
-        sql = "SELECT * FROM job_postings WHERE job_category IN ('Product_Management', 'Data_Science')"
-        return self.execute_db_command(sql)
-
-    def getAllProductManagerJobs(self):
-        sql = "SELECT * FROM job_postings WHERE (job_title ILIKE '%AI%' OR job_title ILIKE '%Product Manager%')"
-        return self.execute_db_command(sql)
-
-    def updateLinkedInJobRecordUpdatedDate(self, jobUrl):
-        sql = """
-        UPDATE job_postings
-        SET job_last_collected_date = %s
-        WHERE posting_url = %s;
-        """
-        todaysDate = datetime.now().replace(hour=0, minute=0, second=0, microsecond=0).strftime('%Y-%m-%d %H:%M:%S')
-        data = (todaysDate, jobUrl)
-        return self.execute_db_command(sql, data)
-
-    def update_job_posting(self, job_posting):
-        set_sql = ', '.join([f"{col} = %s" for col in job_posting.index if col != 'job_posting_id'])
-        sql = f"""
-        UPDATE job_postings
-        SET {set_sql}
-        WHERE job_posting_id = %s;
-        """
-        data = tuple(job_posting[col] for col in job_posting.index if col != 'job_posting_id') + (job_posting['job_posting_id'],)
-        return self.execute_db_command(sql, data)
-
-    def fetchPmJobsRequiringEnrichment(self):
-        sql = "SELECT * FROM job_postings WHERE (job_title ILIKE '%AI%' OR job_title ILIKE '%Product Manager%') AND is_ai IS NULL ORDER BY job_posting_date DESC"
-        return self.execute_db_command(sql)
-
-    def fetchJobsRequiringEnrichment(self):
-        sql = "SELECT * FROM job_postings WHERE is_ai IS NULL"
-        return self.execute_db_command(sql)
-
-    def checkIfJobExists(self, cleanedLinkedInJobURL):
-        sql = "SELECT * FROM job_postings WHERE posting_url = %s"
-        result = self.execute_db_command(sql, (cleanedLinkedInJobURL,))
-        return len(result) > 0 if result is not None else False
-
-    def insertNewJobRecord(self, jobpostingDataFrame):
-        sql = """
-        INSERT INTO job_postings (
-            job_posting_id, company_id, posting_url, posting_source, posting_source_id, job_title,
-            full_posting_description, job_description, is_ai, job_salary, job_posting_company_information, 
-            job_posting_date, job_insertion_date, job_last_collected_date, job_active, city, state
-        ) VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s)
-        """
-        row = jobpostingDataFrame.iloc[0].apply(lambda x: str(x) if isinstance(x, uuid.UUID) else x)
-        return self.execute_db_command(sql, tuple(row))
-
-    def getAllJobs(self):
-        sql = "SELECT * FROM job_postings"
-        return self.execute_db_command(sql)
-
-    def getActiveJobsIdsAsDataFrame(self):
-        sql = "SELECT * FROM job_postings WHERE job_active = TRUE"
-        return self.execute_db_command(sql)
-
-    def getJobByJobPostingId(self, job_posting_id):
-        sql = "SELECT * FROM job_postings WHERE job_posting_id = %s"
-        return self.execute_db_command(sql, (job_posting_id,))
-
-    def getUncategorizedJobs(self):
-        sql = "SELECT * FROM job_postings WHERE job_category IS NULL"
-        return self.execute_db_command(sql)
-
-    def getjobsFromListOfJobsIds(self, dataframeOfJobIds):
-        job_ids_tuple = tuple(dataframeOfJobIds['job_posting_id'].tolist())
-        sql = """
-        SELECT
-            c.company_name,
-            c.linkedin_url,
-            jp.job_title,
-            jp.posting_url,
-            jp.full_posting_description,
-            jp.job_description,
-            jp.is_ai,
-            jp.is_genai,
-            jp.salary_low,
-            jp.salary_midpoint,
-            jp.salary_high,
-            jp.job_salary,
-            jp.job_category,
-            jp.job_posting_date,
-            jp.job_posting_id AS job_posting_id,
-            jp.company_id,
-            jp.posting_source,
-            jp.posting_source_id,
-            jp.job_posting_company_information,
-            jp.job_insertion_date,
-            jp.job_last_collected_date,
-            jp.job_active,
-            jp.city,
-            jp.state,
-            jp.job_skills,
-            jp.is_ai_justification,
-            jp.work_location_type
-        FROM
-            job_postings jp
-        JOIN
-            companies c ON jp.company_id = c.company_id
-        WHERE
-            jp.job_posting_id IN %s;
-        """
+import os
+from datetime import datetime
+import uuid
+import logging
+from dotenv import load_dotenv
+import pandas as pd
+import psycopg2
+
+load_dotenv('.env')
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+class JobPostingDao:
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+    def _get_connection(self):
+        return psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+        )
+
+    def execute_db_command(self, sql_statement, data=None):
+        conn = self._get_connection()
+        try:
+            cur = conn.cursor()
+            cur.execute(sql_statement, data)
+            if sql_statement.strip().lower().startswith("select"):
+                result = pd.DataFrame(cur.fetchall(), columns=[desc[0] for desc in cur.description])
+            else:
+                conn.commit()
+                result = "Success"
+            cur.close()
+        except Exception as e:
+            logging.error(f"Database error: {e}\nSQL Statement: {sql_statement}\nData: {data}")
+            result = None
+        finally:
+            conn.close()
+        return result
+
+    def getAllDataScienceOrProductCategorizedJobs(self):
+        sql = "SELECT * FROM job_postings WHERE job_category IN ('Product_Management', 'Data_Science')"
+        return self.execute_db_command(sql)
+
+    def getAllProductManagerJobs(self):
+        sql = "SELECT * FROM job_postings WHERE (job_title ILIKE '%AI%' OR job_title ILIKE '%Product Manager%')"
+        return self.execute_db_command(sql)
+
+    def updateLinkedInJobRecordUpdatedDate(self, jobUrl):
+        sql = """
+        UPDATE job_postings
+        SET job_last_collected_date = %s
+        WHERE posting_url = %s;
+        """
+        todaysDate = datetime.now().replace(hour=0, minute=0, second=0, microsecond=0).strftime('%Y-%m-%d %H:%M:%S')
+        data = (todaysDate, jobUrl)
+        return self.execute_db_command(sql, data)
+
+    def update_job_posting(self, job_posting):
+        set_sql = ', '.join([f"{col} = %s" for col in job_posting.index if col != 'job_posting_id'])
+        sql = f"""
+        UPDATE job_postings
+        SET {set_sql}
+        WHERE job_posting_id = %s;
+        """
+        data = tuple(job_posting[col] for col in job_posting.index if col != 'job_posting_id') + (job_posting['job_posting_id'],)
+        return self.execute_db_command(sql, data)
+
+    def fetchPmJobsRequiringEnrichment(self):
+        sql = "SELECT * FROM job_postings WHERE (job_title ILIKE '%AI%' OR job_title ILIKE '%Product Manager%') AND is_ai IS NULL ORDER BY job_posting_date DESC"
+        return self.execute_db_command(sql)
+
+    def fetchJobsRequiringEnrichment(self):
+        sql = "SELECT * FROM job_postings WHERE is_ai IS NULL"
+        return self.execute_db_command(sql)
+
+    def checkIfJobExists(self, cleanedLinkedInJobURL):
+        sql = "SELECT * FROM job_postings WHERE posting_url = %s"
+        result = self.execute_db_command(sql, (cleanedLinkedInJobURL,))
+        return len(result) > 0 if result is not None else False
+
+    def insertNewJobRecord(self, jobpostingDataFrame):
+        sql = """
+        INSERT INTO job_postings (
+            job_posting_id, company_id, posting_url, posting_source, posting_source_id, job_title,
+            full_posting_description, job_description, is_ai, job_salary, job_posting_company_information, 
+            job_posting_date, job_insertion_date, job_last_collected_date, job_active, city, state
+        ) VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s, %s)
+        """
+        row = jobpostingDataFrame.iloc[0].apply(lambda x: str(x) if isinstance(x, uuid.UUID) else x)
+        return self.execute_db_command(sql, tuple(row))
+
+    def getAllJobs(self):
+        sql = "SELECT * FROM job_postings"
+        return self.execute_db_command(sql)
+
+    def getActiveJobsIdsAsDataFrame(self):
+        sql = "SELECT * FROM job_postings WHERE job_active = TRUE"
+        return self.execute_db_command(sql)
+
+    def getJobByJobPostingId(self, job_posting_id):
+        sql = "SELECT * FROM job_postings WHERE job_posting_id = %s"
+        return self.execute_db_command(sql, (job_posting_id,))
+
+    def getUncategorizedJobs(self):
+        sql = "SELECT * FROM job_postings WHERE job_category IS NULL"
+        return self.execute_db_command(sql)
+
+    def getjobsFromListOfJobsIds(self, dataframeOfJobIds):
+        job_ids_tuple = tuple(dataframeOfJobIds['job_posting_id'].tolist())
+        sql = """
+        SELECT
+            c.company_name,
+            c.linkedin_url,
+            jp.job_title,
+            jp.posting_url,
+            jp.full_posting_description,
+            jp.job_description,
+            jp.is_ai,
+            jp.is_genai,
+            jp.salary_low,
+            jp.salary_midpoint,
+            jp.salary_high,
+            jp.job_salary,
+            jp.job_category,
+            jp.job_posting_date,
+            jp.job_posting_id AS job_posting_id,
+            jp.company_id,
+            jp.posting_source,
+            jp.posting_source_id,
+            jp.job_posting_company_information,
+            jp.job_insertion_date,
+            jp.job_last_collected_date,
+            jp.job_active,
+            jp.city,
+            jp.state,
+            jp.job_skills,
+            jp.is_ai_justification,
+            jp.work_location_type
+        FROM
+            job_postings jp
+        JOIN
+            companies c ON jp.company_id = c.company_id
+        WHERE
+            jp.job_posting_id IN %s;
+        """
         return self.execute_db_command(sql, (job_ids_tuple,))
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobResponsibilitiesDao.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobResponsibilitiesDao.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import os
-from datetime import datetime
-import uuid
-import logging
-from dotenv import load_dotenv
-import pandas as pd
-import psycopg2
-
-load_dotenv('.env')
-
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-class JobResponsibilitiesDao :
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-
-    def insertJobResponsibilitiesForJobPosting(self, jobResponsibilitiesDataFrame):
-        """
-        When given a dataframe that has multiple records, this function will insert each record into the DB. 
-        """
-
-        conn = psycopg2.connect(
-            host=os.getenv("host"),
-            database=os.getenv("database"),
-            user=os.getenv("digitalOcean"),
-            password=os.getenv("password"),
-            port=os.getenv("port")
-        )
-        try:
-            cur = conn.cursor()
-
-            sql_insert_query = "INSERT INTO Job_Responsibilities (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
-
-            for index, row in jobResponsibilitiesDataFrame.iterrows():
-
-                # Convert UUID to string before insertion
-                job_posting_id_str = str(row['job_posting_id'])
-                unique_id_str = str(row['unique_id'])
-                data = (job_posting_id_str, unique_id_str, row['item'])
-                cur.execute(sql_insert_query, data)
-                
-            conn.commit()
-
-            cur.close()
-            conn.close()
-
-            return "Update successful!"
-
-        except Exception as e:
-            logging.error("Database connection error:", e)
-            conn.close()
-            return None
+import os
+from datetime import datetime
+import uuid
+import logging
+from dotenv import load_dotenv
+import pandas as pd
+import psycopg2
+
+load_dotenv('.env')
+
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+class JobResponsibilitiesDao :
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+
+    def insertJobResponsibilitiesForJobPosting(self, jobResponsibilitiesDataFrame):
+        """
+        When given a dataframe that has multiple records, this function will insert each record into the DB. 
+        """
+
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+        )
+        try:
+            cur = conn.cursor()
+
+            sql_insert_query = "INSERT INTO Job_Responsibilities (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
+
+            for index, row in jobResponsibilitiesDataFrame.iterrows():
+
+                # Convert UUID to string before insertion
+                job_posting_id_str = str(row['job_posting_id'])
+                unique_id_str = str(row['unique_id'])
+                data = (job_posting_id_str, unique_id_str, row['item'])
+                cur.execute(sql_insert_query, data)
+                
+            conn.commit()
+
+            cur.close()
+            conn.close()
+
+            return "Update successful!"
+
+        except Exception as e:
+            logging.error("Database connection error:", e)
+            conn.close()
+            return None
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobSkillsDao.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobSkillsDao.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import os
-import logging
-from dotenv import load_dotenv
-import pandas as pd
-import psycopg2
-
-load_dotenv('.env')
-
-# Configure logging
-logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
-
-
-class JobSkillsDao :
-    def __init__(self):
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-
-    def insertSkillsForJobPosting(self, jobSkillsDataFrame):
-        """
-        When given a dataframe that has multiple records, this function will insert each record into the DB. 
-        """
-
-        conn = psycopg2.connect(
-            host=os.getenv("host"),
-            database=os.getenv("database"),
-            user=os.getenv("digitalOcean"),
-            password=os.getenv("password"),
-            port=os.getenv("port")
-        )
-        try:
-            cur = conn.cursor()
-
-            sql_insert_query = "INSERT INTO Job_Skills (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
-
-            for index, row in jobSkillsDataFrame.iterrows():
-
-                # Convert UUID to string before insertion
-                job_posting_id_str = str(row['job_posting_id'])
-                unique_id_str = str(row['unique_id'])
-                data = (job_posting_id_str, unique_id_str, row['item'])
-                cur.execute(sql_insert_query, data)
-                
-                
-            conn.commit()
-
-            cur.close()
-            conn.close()
-
-            return "Update successful!"
-
-        except Exception as e:
-            logging.error("Database connection error:", e)
-            conn.close()
-            return None
-        
-
-    def getSkillsForJobID(self, job_posting_id):
-
-        """
-        This function calls the Job Skills Table to find all the records that have the given job_posting_id 
-        
-        Returns the list as a Pandas DataFrame
-        """
-
-        conn = psycopg2.connect(
-            host=os.getenv("host"),
-            database=os.getenv("database"),
-            user=os.getenv("digitalOcean"),
-            password=os.getenv("password"),
-            port=os.getenv("port")
-        )
-        try:
-
-            cur = conn.cursor()
-            
-            sql_select_query = "SELECT * FROM job_skills WHERE job_posting_id = %s"
-            cur.execute(sql_select_query, (job_posting_id,))  
-
-            rows = cur.fetchall()
-
-            if rows:
-                df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
-            else:
-                df = pd.DataFrame()
-
-            cur.close()
-            conn.close()
-
-            return df
-
-        except Exception as e:
-            logging.error(f"Database connection error in getSkillsForJobID: {e}")
-            conn.close()
-            return pd.DataFrame()  
-        
+import os
+import logging
+from dotenv import load_dotenv
+import pandas as pd
+import psycopg2
+
+load_dotenv('.env')
+
+# Configure logging
+logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
+
+
+class JobSkillsDao :
+    def __init__(self):
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+
+    def insertSkillsForJobPosting(self, jobSkillsDataFrame):
+        """
+        When given a dataframe that has multiple records, this function will insert each record into the DB. 
+        """
+
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+        )
+        try:
+            cur = conn.cursor()
+
+            sql_insert_query = "INSERT INTO Job_Skills (job_posting_id, unique_id, item) VALUES (%s, %s, %s)"
+
+            for index, row in jobSkillsDataFrame.iterrows():
+
+                # Convert UUID to string before insertion
+                job_posting_id_str = str(row['job_posting_id'])
+                unique_id_str = str(row['unique_id'])
+                data = (job_posting_id_str, unique_id_str, row['item'])
+                cur.execute(sql_insert_query, data)
+                
+                
+            conn.commit()
+
+            cur.close()
+            conn.close()
+
+            return "Update successful!"
+
+        except Exception as e:
+            logging.error("Database connection error:", e)
+            conn.close()
+            return None
+        
+
+    def getSkillsForJobID(self, job_posting_id):
+
+        """
+        This function calls the Job Skills Table to find all the records that have the given job_posting_id 
+        
+        Returns the list as a Pandas DataFrame
+        """
+
+        conn = psycopg2.connect(
+            host=os.getenv("host"),
+            database=os.getenv("database"),
+            user=os.getenv("digitalOcean"),
+            password=os.getenv("password"),
+            port=os.getenv("port")
+        )
+        try:
+
+            cur = conn.cursor()
+            
+            sql_select_query = "SELECT * FROM job_skills WHERE job_posting_id = %s"
+            cur.execute(sql_select_query, (job_posting_id,))  
+
+            rows = cur.fetchall()
+
+            if rows:
+                df = pd.DataFrame(rows, columns=[desc[0] for desc in cur.description])
+            else:
+                df = pd.DataFrame()
+
+            cur.close()
+            conn.close()
+
+            return df
+
+        except Exception as e:
+            logging.error(f"Database connection error in getSkillsForJobID: {e}")
+            conn.close()
+            return pd.DataFrame()  
+
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/JobTitleCategoryClassifier.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/JobTitleCategoryClassifier.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-"""
-When given a Job Title, this class is responsible for loading a CSV and then using it as a map to locate the specific category for this job_title
-
-Example Categories:
-- Product_Management
-- Data_Science
-- Engineerging
-- Operations
-- Business_Analyst
-- Project_Management
-- User_Experience
-- Business_Development
-- Customer_Success
-- Marketing
-- Sales
-- Executive_Role
-- Retail
-- Food_Services
-- Other
-"""
-
-
-import logging
-from dotenv import load_dotenv
-import pandas as pd
-
-load_dotenv('.env')
-
-logging.basicConfig(level=logging.INFO)  
-
-
-class JobTitleCategoryClassifier:
-    def __init__(self):
-        logging.basicConfig(level=logging.INFO)  # Ensure logger is set up
-        self.logger = logging.getLogger(__name__)  # Get a logger for this class
-        self.logger.info(f"{self.__class__.__name__} class initialized")
-        self.data_frame = pd.read_csv('CommonUtilities/Configuration/JobCategories.csv')
-        
-
-    def get_job_category(self, job_title):
-        """
-        Load the CSV Configuration File as a Pandas DataFrame.
-        Relative Path = CommonUtilities\Configuration\JobCategories.csv
-        Check to see if the Job title is listed in the data frame and then use the job category. 
-        Return whatever category has been found. 
-        
-        If not found, log a message and return category of Unknown.
-        """
-
-        # Attempt to find the job title in the DataFrame
-        result = self.data_frame[self.data_frame['job_title'].str.lower() == job_title.lower()]
-        
-        if not result.empty:
-            # If found, return the corresponding category
-            return result['job_category'].iloc[0]
-        else:
-            # If not found, log a message and return "Unknown"
-            self.logger.info(f"job_title '{job_title}' not found.")
+"""
+When given a Job Title, this class is responsible for loading a CSV and then using it as a map to locate the specific category for this job_title
+
+Example Categories:
+- Product_Management
+- Data_Science
+- Engineerging
+- Operations
+- Business_Analyst
+- Project_Management
+- User_Experience
+- Business_Development
+- Customer_Success
+- Marketing
+- Sales
+- Executive_Role
+- Retail
+- Food_Services
+- Other
+"""
+
+
+import logging
+from dotenv import load_dotenv
+import pandas as pd
+
+load_dotenv('.env')
+
+logging.basicConfig(level=logging.INFO)  
+
+
+class JobTitleCategoryClassifier:
+    def __init__(self):
+        logging.basicConfig(level=logging.INFO)  # Ensure logger is set up
+        self.logger = logging.getLogger(__name__)  # Get a logger for this class
+        self.logger.info(f"{self.__class__.__name__} class initialized")
+        self.data_frame = pd.read_csv('CommonUtilities/Configuration/JobCategories.csv')
+        
+
+    def get_job_category(self, job_title):
+        """
+        Load the CSV Configuration File as a Pandas DataFrame.
+        Relative Path = CommonUtilities\Configuration\JobCategories.csv
+        Check to see if the Job title is listed in the data frame and then use the job category. 
+        Return whatever category has been found. 
+        
+        If not found, log a message and return category of Unknown.
+        """
+
+        # Attempt to find the job title in the DataFrame
+        result = self.data_frame[self.data_frame['job_title'].str.lower() == job_title.lower()]
+        
+        if not result.empty:
+            # If found, return the corresponding category
+            return result['job_category'].iloc[0]
+        else:
+            # If not found, log a message and return "Unknown"
+            self.logger.info(f"job_title '{job_title}' not found.")
             return "Unknown"
```

### Comparing `operationbattleshipcommonutilities-0.4.7/operation_battleship_common_utilities/PineConeDatabaseCaller.py` & `OperationBattleshipCommonUtilities-0.4.8/operation_battleship_common_utilities/PineConeDatabaseCaller.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import logging
-import os
-import datetime
-from dotenv import load_dotenv
-from pinecone import Pinecone, ServerlessSpec
-
-load_dotenv('.env')
-
-
-class PineConeDatabaseCaller:
-
-    def __init__(self, api_key):
-        self.pc = Pinecone(api_key=api_key)  # Initialize Pinecone client with your API key
-        logging.info(f"{self.__class__.__name__} class initialized")
-
-        return
-    
-    def createIndexIfDoesntExist(self, indexName):
-        """
-        Checks to see if this index exists in Pinecone. If it does, then just return.
-        If the index does not yet exist, create it. 
-        """
-        if indexName not in self.pc.list_indexes().names():
-            self.pc.create_index(name=indexName, 
-                                 dimension=768,
-                                 metric='cosine',
-                                 spec=ServerlessSpec(
-                                    cloud="aws",
-                                    region="us-west-2"
-                                    ) 
-                                 )
-            logging.info(f"Index {indexName} created.")
-        else:
-            logging.info(f"Index {indexName} already exists.")
-
-        return
-
-    
-    # ...
-    def upsertEmbeddings(self, indexName, namespace, embeddingsDictionary):
-        index = self.pc.Index(indexName)
-        vectors = []
-        for id, data in embeddingsDictionary.items():
-
-            
-            # Ensure embedding is a flat list of floats
-            embedding = data['embedding']
-            if isinstance(embedding[0], list):  # Checks if the first element is a list, indicating a nested structure
-                logging.debug(f"Datatype of the first element in the embedding: {type(embedding[0])}")
-                embedding = embedding[0]  # Assumes the embedding is the first element of the list
-            
-            vectors.append({
-                'id': id,
-                'values': embedding,
-                'metadata': data['metadata']
-            })
-        upsert_response = index.upsert(vectors, namespace=namespace)
-        return upsert_response
-        
-    def query(self, embeddedResume, numberOfNeighbors, indexName, namespace, numberOfDays=45):
-        # Calculate the date to filter job postings
-        job_posting_date_cutoff = self.getIntegerValueForDayFilter(numberOfDays)
-
-        index = self.pc.Index(indexName)
-
-        # Applying the job_posting_date filter
-        result = index.query(
-            namespace=namespace,
-            vector=embeddedResume,
-            filter={"job_posting_date": {"$gte": job_posting_date_cutoff}},  # Adjust this filter as per your requirements
-            top_k=numberOfNeighbors,
-            include_metadata=True
-        )
-
-        return result
-
-    def getIntegerValueForDayFilter(self, numberOfDays):
-        """
-        Calculate the number of days since the Unix epoch for the date numberOfDays ago.
-        """
-        today = datetime.date.today()
-        cutoff_date = today - datetime.timedelta(days=numberOfDays)
-        epoch_start = datetime.date(1970, 1, 1)
-        days_since_epoch = (cutoff_date - epoch_start).days
-        logging.debug(f"Computed days since epoch for cutoff: {days_since_epoch}")
+import logging
+import os
+import datetime
+from dotenv import load_dotenv
+from pinecone import Pinecone, ServerlessSpec
+
+load_dotenv('.env')
+
+
+class PineConeDatabaseCaller:
+
+    def __init__(self, api_key):
+        self.pc = Pinecone(api_key=api_key)  # Initialize Pinecone client with your API key
+        logging.info(f"{self.__class__.__name__} class initialized")
+
+        return
+    
+    def createIndexIfDoesntExist(self, indexName):
+        """
+        Checks to see if this index exists in Pinecone. If it does, then just return.
+        If the index does not yet exist, create it. 
+        """
+        if indexName not in self.pc.list_indexes().names():
+            self.pc.create_index(name=indexName, 
+                                 dimension=768,
+                                 metric='cosine',
+                                 spec=ServerlessSpec(
+                                    cloud="aws",
+                                    region="us-west-2"
+                                    ) 
+                                 )
+            logging.info(f"Index {indexName} created.")
+        else:
+            logging.info(f"Index {indexName} already exists.")
+
+        return
+
+    
+    # ...
+    def upsertEmbeddings(self, indexName, namespace, embeddingsDictionary):
+        index = self.pc.Index(indexName)
+        vectors = []
+        for id, data in embeddingsDictionary.items():
+
+            
+            # Ensure embedding is a flat list of floats
+            embedding = data['embedding']
+            if isinstance(embedding[0], list):  # Checks if the first element is a list, indicating a nested structure
+                logging.debug(f"Datatype of the first element in the embedding: {type(embedding[0])}")
+                embedding = embedding[0]  # Assumes the embedding is the first element of the list
+            
+            vectors.append({
+                'id': id,
+                'values': embedding,
+                'metadata': data['metadata']
+            })
+        upsert_response = index.upsert(vectors, namespace=namespace)
+        return upsert_response
+        
+    def query(self, embeddedResume, numberOfNeighbors, indexName, namespace, numberOfDays=45):
+        # Calculate the date to filter job postings
+        job_posting_date_cutoff = self.getIntegerValueForDayFilter(numberOfDays)
+
+        index = self.pc.Index(indexName)
+
+        # Applying the job_posting_date filter
+        result = index.query(
+            namespace=namespace,
+            vector=embeddedResume,
+            filter={"job_posting_date": {"$gte": job_posting_date_cutoff}},  # Adjust this filter as per your requirements
+            top_k=numberOfNeighbors,
+            include_metadata=True
+        )
+
+        return result
+
+    def getIntegerValueForDayFilter(self, numberOfDays):
+        """
+        Calculate the number of days since the Unix epoch for the date numberOfDays ago.
+        """
+        today = datetime.date.today()
+        cutoff_date = today - datetime.timedelta(days=numberOfDays)
+        epoch_start = datetime.date(1970, 1, 1)
+        days_since_epoch = (cutoff_date - epoch_start).days
+        logging.debug(f"Computed days since epoch for cutoff: {days_since_epoch}")
         return days_since_epoch
```

### Comparing `operationbattleshipcommonutilities-0.4.7/setup.py` & `OperationBattleshipCommonUtilities-0.4.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='OperationBattleshipCommonUtilities',
-    version='0.4.7',
-    packages=find_packages(),
-    license='Apache-2.0 license',
-    description='Classes and Utilities that are shared in the Operation Battleship Application',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
-    author='Matthew Caraway',
-    author_email='matthew@CarawayLabs.com',
-    url='https://github.com/CarawayLabs/OperationBattleshipCommonUtilities',
-    install_requires=[
-        'python-dotenv',
-        'apify-client',
-        'pandas',
-        'psycopg2',
-        'nomic',
-        'openai',
-        'pinecone-client',
-    ],
-)
+from setuptools import setup, find_packages
+
+setup(
+    name='OperationBattleshipCommonUtilities',
+    version='0.4.8',
+    packages=find_packages(),
+    license='Apache-2.0 license',
+    description='Classes and Utilities that are shared in the Operation Battleship Application',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    author='Matthew Caraway',
+    author_email='matthew@CarawayLabs.com',
+    url='https://github.com/CarawayLabs/OperationBattleshipCommonUtilities',
+    install_requires=[
+        'python-dotenv',
+        'apify-client',
+        'pandas',
+        'psycopg2',
+        'nomic',
+        'openai',
+        'pinecone-client',
+    ],
+)
```

