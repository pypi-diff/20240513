# Comparing `tmp/powfacpy-0.1.6.tar.gz` & `tmp/powfacpy-0.2.0.tar.gz`

## Comparing `powfacpy-0.1.6.tar` & `powfacpy-0.2.0.tar`

### file list

```diff
@@ -1,183 +1,183 @@
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 powfacpy-0.1.6/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/.nojekyll
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/Makefile
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/_config.yml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/index.html
--rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/make.bat
--rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/api.doctree
--rw-r--r--   0        0        0    27723 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/environment.pickle
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/how_to_contribute.doctree
--rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/index.doctree
--rw-r--r--   0        0        0    24558 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/introduction.doctree
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/tutorials.doctree
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/generated/powerfactorypy.PFBaseInterface.doctree
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/generated/powerfactorypy.PFStringManipuilation.doctree
--rw-r--r--   0        0        0    54402 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFBaseInterface.doctree
--rw-r--r--   0        0        0    65508 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFDynSimInterface.doctree
--rw-r--r--   0        0        0    79988 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFPlotInterface.doctree
--rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFStringManipuilation.doctree
--rw-r--r--   0        0        0    71310 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFStudyCases.doctree
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/.buildinfo
--rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/api.html
--rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/genindex.html
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/how_to_contribute.html
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/index.html
--rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/introduction.html
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/objects.inv
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/search.html
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/searchindex.js
--rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/tutorials.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/api.rst.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/how_to_contribute.rst.txt
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/index.rst.txt
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/introduction.rst.txt
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/tutorials.rst.txt
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/generated/powerfactorypy.PFBaseInterface.rst.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/generated/powerfactorypy.PFStringManipuilation.rst.txt
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFBaseInterface.rst.txt
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFDynSimInterface.rst.txt
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFPlotInterface.rst.txt
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFStringManipuilation.rst.txt
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFStudyCases.rst.txt
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/basic.css
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/doctools.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/file.png
--rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/jquery-3.6.0.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/jquery.js
--rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/plus.png
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/pygments.css
--rw-r--r--   0        0        0    17120 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/searchtools.js
--rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/underscore-1.13.1.js
--rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/underscore.js
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/badge_only.css
--rw-r--r--   0        0        0   129674 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/theme.css
--rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/js/badge_only.js
--rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/js/html5shiv.min.js
--rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/_static/js/theme.js
--rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/generated/powerfactorypy.PFBaseInterface.html
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/generated/powerfactorypy.PFStringManipuilation.html
--rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/generated/powfacpy.PFBaseInterface.html
--rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/generated/powfacpy.PFDynSimInterface.html
--rw-r--r--   0        0        0    21709 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/generated/powfacpy.PFPlotInterface.html
--rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/generated/powfacpy.PFStringManipuilation.html
--rw-r--r--   0        0        0    19956 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/html/generated/powfacpy.PFStudyCases.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/api.rst
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/conf.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/how_to_contribute.rst
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/index.rst
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/introduction.rst
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/tutorials.rst
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/generated/powfacpy.PFBaseInterface.rst
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/generated/powfacpy.PFDynSimInterface.rst
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/generated/powfacpy.PFPlotInterface.rst
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/generated/powfacpy.PFStringManipuilation.rst
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 powfacpy-0.1.6/docs/source/generated/powfacpy.PFStudyCases.rst
--rw-r--r--   0        0        0    19795 2020-02-02 00:00:00.000000 powfacpy-0.1.6/power_factory_objects/CopyOfObjectsInTableOfContentsOfScriptingReference.txt
--rw-r--r--   0        0        0   260282 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmArea.txt
--rw-r--r--   0        0        0  1076903 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmAsm.txt
--rw-r--r--   0        0        0  1083370 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmAsmsc.txt
--rw-r--r--   0        0        0    72412 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmBoundary.txt
--rw-r--r--   0        0        0  1219126 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmCoup.txt
--rw-r--r--   0        0        0  1079205 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmGenstat.txt
--rw-r--r--   0        0        0   609076 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmIac.txt
--rw-r--r--   0        0        0  1381816 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmLne.txt
--rw-r--r--   0        0        0   799092 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmLod.txt
--rw-r--r--   0        0        0   757418 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmLodlv.txt
--rw-r--r--   0        0        0   799516 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmLodmv.txt
--rw-r--r--   0        0        0  1081229 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmPvsys.txt
--rw-r--r--   0        0        0    62660 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmSecctrl.txt
--rw-r--r--   0        0        0  1078265 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmShnt.txt
--rw-r--r--   0        0        0  1157076 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmSind.txt
--rw-r--r--   0        0        0    82348 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmStactrl.txt
--rw-r--r--   0        0        0  1144745 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmSym.txt
--rw-r--r--   0        0        0   334278 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmTerm.txt
--rw-r--r--   0        0        0  2031408 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmTr2.txt
--rw-r--r--   0        0        0  2991495 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmTr3.txt
--rw-r--r--   0        0        0   643288 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmVac.txt
--rw-r--r--   0        0        0  1473726 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmVsc.txt
--rw-r--r--   0        0        0  1093270 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmVscmono.txt
--rw-r--r--   0        0        0   762160 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmXnet.txt
--rw-r--r--   0        0        0   260960 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmZone.txt
--rw-r--r--   0        0        0  1258884 2020-02-02 00:00:00.000000 powfacpy-0.1.6/result_variables/ElmZpu.txt
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/__init__.py
--rw-r--r--   0        0        0    20180 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/active_project_interface.py
--rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/case_studies.py
--rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/database_interface.py
--rw-r--r--   0        0        0    12515 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/dyn_sim_interface.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/engineering_helpers.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/exceptions.py
--rw-r--r--   0        0        0    54130 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/folders_interface.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/functional_interface.py
--rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/grouping.py
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/model_exchange_interfaces.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/network_interface.py
--rw-r--r--   0        0        0   794654 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/pf_class_protocols.py
--rw-r--r--   0        0        0   791323 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/pf_class_protocols_old.py
--rw-r--r--   0        0        0    10996 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/pf_classes_protocol_generator.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/pf_elm_objects.py
--rw-r--r--   0        0        0    32949 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/plot_interface.py
--rw-r--r--   0        0        0  3460426 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/result_variables.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/result_variables_parser.py
--rw-r--r--   0        0        0    21278 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/results_interface.py
--rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/script_interface.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/string_manipulation.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 powfacpy-0.1.6/src/powfacpy/topology.py
--rw-r--r--   0        0        0    17926 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_active_project_interface.py
--rw-r--r--   0        0        0    14913 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_case_studies.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_database_interface.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_dyn_sim_interface.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_functional_interface.py
--rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_model_exchange_interfaces.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_network_interface.py
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_plot_interface.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_results_interface.py
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/test_script_interface.py
--rw-r--r--   0        0        0   294848 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_input/powfacpy_tests.pfd
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_input/simple_script.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_input/test_comtrade.cfg
--rw-r--r--   0        0        0    72000 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_input/test_comtrade.dat
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_output/.gitignore
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_output/file_from_embedded_script.py
--rw-r--r--   0        0        0   140282 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_output/powfacpy_single_file.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_output/test1.json
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_output/test2.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_output/test_get_object_attributes.json
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tests/tests_output/test_get_object_attributes_modified.json
--rw-r--r--   0        0        0    28980 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/getting_started.ipynb
--rw-r--r--   0        0        0   237127 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/simulation_and_plotting.ipynb
--rw-r--r--   0        0        0    19570 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/study_cases.ipynb
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/figures/cases_1.png
--rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/figures/cases_2.png
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/figures/legend_1.png
--rw-r--r--   0        0        0    17537 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/figures/object_path.png
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/figures/rebuild_button.png
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/figures/scenarios_1.png
--rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/figures/type_hints.png
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 powfacpy-0.1.6/tutorials/figures/variations_3.png
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 powfacpy-0.1.6/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 powfacpy-0.1.6/LICENSE
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 powfacpy-0.1.6/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 powfacpy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 powfacpy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 powfacpy-0.2.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/.nojekyll
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/_config.yml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/index.html
+-rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0     9315 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/api.doctree
+-rw-r--r--   0        0        0    27723 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/environment.pickle
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/how_to_contribute.doctree
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/index.doctree
+-rw-r--r--   0        0        0    24558 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/introduction.doctree
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/tutorials.doctree
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/generated/powerfactorypy.PFBaseInterface.doctree
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/generated/powerfactorypy.PFStringManipuilation.doctree
+-rw-r--r--   0        0        0    54402 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFBaseInterface.doctree
+-rw-r--r--   0        0        0    65508 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFDynSimInterface.doctree
+-rw-r--r--   0        0        0    79988 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFPlotInterface.doctree
+-rw-r--r--   0        0        0    12320 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFStringManipuilation.doctree
+-rw-r--r--   0        0        0    71310 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFStudyCases.doctree
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/.buildinfo
+-rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/api.html
+-rw-r--r--   0        0        0     5760 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/genindex.html
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/how_to_contribute.html
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/index.html
+-rw-r--r--   0        0        0     8336 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/introduction.html
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/objects.inv
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/search.html
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/searchindex.js
+-rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/tutorials.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/api.rst.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/how_to_contribute.rst.txt
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/introduction.rst.txt
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/tutorials.rst.txt
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/generated/powerfactorypy.PFBaseInterface.rst.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/generated/powerfactorypy.PFStringManipuilation.rst.txt
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFBaseInterface.rst.txt
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFDynSimInterface.rst.txt
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFPlotInterface.rst.txt
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFStringManipuilation.rst.txt
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFStudyCases.rst.txt
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0        0        0    15519 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/basic.css
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/doctools.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/file.png
+-rw-r--r--   0        0        0   288580 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/jquery-3.6.0.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/jquery.js
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/plus.png
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/pygments.css
+-rw-r--r--   0        0        0    17120 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/searchtools.js
+-rw-r--r--   0        0        0    68420 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/underscore-1.13.1.js
+-rw-r--r--   0        0        0    19530 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/underscore.js
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/badge_only.css
+-rw-r--r--   0        0        0   129674 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/theme.css
+-rw-r--r--   0        0        0    87624 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0        0        0    67312 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0        0        0    86288 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0        0        0    66444 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0        0        0   165742 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   444379 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    98024 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    77160 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0   323344 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0        0        0   193308 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0        0        0   309728 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0        0        0   184912 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0        0        0   328412 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0        0        0   195704 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0        0        0   309192 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0        0        0   182708 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/js/badge_only.js
+-rw-r--r--   0        0        0     4370 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/js/html5shiv.min.js
+-rw-r--r--   0        0        0     5023 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/_static/js/theme.js
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/generated/powerfactorypy.PFBaseInterface.html
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/generated/powerfactorypy.PFStringManipuilation.html
+-rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/generated/powfacpy.PFBaseInterface.html
+-rw-r--r--   0        0        0    18556 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/generated/powfacpy.PFDynSimInterface.html
+-rw-r--r--   0        0        0    21709 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/generated/powfacpy.PFPlotInterface.html
+-rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/generated/powfacpy.PFStringManipuilation.html
+-rw-r--r--   0        0        0    19956 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/html/generated/powfacpy.PFStudyCases.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/api.rst
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/conf.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/how_to_contribute.rst
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/index.rst
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/introduction.rst
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/tutorials.rst
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/generated/powfacpy.PFBaseInterface.rst
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/generated/powfacpy.PFDynSimInterface.rst
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/generated/powfacpy.PFPlotInterface.rst
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/generated/powfacpy.PFStringManipuilation.rst
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 powfacpy-0.2.0/docs/source/generated/powfacpy.PFStudyCases.rst
+-rw-r--r--   0        0        0    19795 2020-02-02 00:00:00.000000 powfacpy-0.2.0/power_factory_objects/CopyOfObjectsInTableOfContentsOfScriptingReference.txt
+-rw-r--r--   0        0        0   260282 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmArea.txt
+-rw-r--r--   0        0        0  1076903 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmAsm.txt
+-rw-r--r--   0        0        0  1083370 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmAsmsc.txt
+-rw-r--r--   0        0        0    72412 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmBoundary.txt
+-rw-r--r--   0        0        0  1219126 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmCoup.txt
+-rw-r--r--   0        0        0  1079205 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmGenstat.txt
+-rw-r--r--   0        0        0   609076 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmIac.txt
+-rw-r--r--   0        0        0  1381816 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmLne.txt
+-rw-r--r--   0        0        0   799092 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmLod.txt
+-rw-r--r--   0        0        0   757418 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmLodlv.txt
+-rw-r--r--   0        0        0   799516 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmLodmv.txt
+-rw-r--r--   0        0        0  1081229 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmPvsys.txt
+-rw-r--r--   0        0        0    62660 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmSecctrl.txt
+-rw-r--r--   0        0        0  1078265 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmShnt.txt
+-rw-r--r--   0        0        0  1157076 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmSind.txt
+-rw-r--r--   0        0        0    82348 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmStactrl.txt
+-rw-r--r--   0        0        0  1144745 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmSym.txt
+-rw-r--r--   0        0        0   334278 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmTerm.txt
+-rw-r--r--   0        0        0  2031408 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmTr2.txt
+-rw-r--r--   0        0        0  2991495 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmTr3.txt
+-rw-r--r--   0        0        0   643288 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmVac.txt
+-rw-r--r--   0        0        0  1473726 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmVsc.txt
+-rw-r--r--   0        0        0  1093270 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmVscmono.txt
+-rw-r--r--   0        0        0   762160 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmXnet.txt
+-rw-r--r--   0        0        0   260960 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmZone.txt
+-rw-r--r--   0        0        0  1258884 2020-02-02 00:00:00.000000 powfacpy-0.2.0/result_variables/ElmZpu.txt
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/__init__.py
+-rw-r--r--   0        0        0    20131 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/active_project_interface.py
+-rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/case_studies.py
+-rw-r--r--   0        0        0     6014 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/database_interface.py
+-rw-r--r--   0        0        0    12544 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/dyn_sim_interface.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/engineering_helpers.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/exceptions.py
+-rw-r--r--   0        0        0    54175 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/folders_interface.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/functional_interface.py
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/grouping.py
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/model_exchange_interfaces.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/network_interface.py
+-rw-r--r--   0        0        0   867650 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/pf_class_protocols.py
+-rw-r--r--   0        0        0   794654 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/pf_class_protocols_old.py
+-rw-r--r--   0        0        0    11085 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/pf_classes_protocol_generator.py
+-rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/pf_elm_objects.py
+-rw-r--r--   0        0        0    32949 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/plot_interface.py
+-rw-r--r--   0        0        0  3460426 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/result_variables.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/result_variables_parser.py
+-rw-r--r--   0        0        0    21278 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/results_interface.py
+-rw-r--r--   0        0        0    11416 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/script_interface.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/string_manipulation.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 powfacpy-0.2.0/src/powfacpy/topology.py
+-rw-r--r--   0        0        0    17928 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_active_project_interface.py
+-rw-r--r--   0        0        0    14913 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_case_studies.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_database_interface.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_dyn_sim_interface.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_functional_interface.py
+-rw-r--r--   0        0        0     5325 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_model_exchange_interfaces.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_network_interface.py
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_plot_interface.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_results_interface.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/test_script_interface.py
+-rw-r--r--   0        0        0   294848 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_input/powfacpy_tests.pfd
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_input/simple_script.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_input/test_comtrade.cfg
+-rw-r--r--   0        0        0    72000 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_input/test_comtrade.dat
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_output/.gitignore
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_output/file_from_embedded_script.py
+-rw-r--r--   0        0        0   140282 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_output/powfacpy_single_file.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_output/test1.json
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_output/test2.json
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_output/test_get_object_attributes.json
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tests/tests_output/test_get_object_attributes_modified.json
+-rw-r--r--   0        0        0    28980 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/getting_started.ipynb
+-rw-r--r--   0        0        0   237127 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/simulation_and_plotting.ipynb
+-rw-r--r--   0        0        0    19570 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/study_cases.ipynb
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/figures/cases_1.png
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/figures/cases_2.png
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/figures/legend_1.png
+-rw-r--r--   0        0        0    17537 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/figures/object_path.png
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/figures/rebuild_button.png
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/figures/scenarios_1.png
+-rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/figures/type_hints.png
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 powfacpy-0.2.0/tutorials/figures/variations_3.png
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 powfacpy-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 powfacpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 powfacpy-0.2.0/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 powfacpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 powfacpy-0.2.0/PKG-INFO
```

### Comparing `powfacpy-0.1.6/docs/Makefile` & `powfacpy-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/make.bat` & `powfacpy-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/api.doctree` & `powfacpy-0.2.0/docs/doctrees/api.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/environment.pickle` & `powfacpy-0.2.0/docs/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/how_to_contribute.doctree` & `powfacpy-0.2.0/docs/doctrees/how_to_contribute.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/index.doctree` & `powfacpy-0.2.0/docs/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/introduction.doctree` & `powfacpy-0.2.0/docs/doctrees/introduction.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/tutorials.doctree` & `powfacpy-0.2.0/docs/doctrees/tutorials.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/generated/powerfactorypy.PFBaseInterface.doctree` & `powfacpy-0.2.0/docs/doctrees/generated/powerfactorypy.PFBaseInterface.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/generated/powerfactorypy.PFStringManipuilation.doctree` & `powfacpy-0.2.0/docs/doctrees/generated/powerfactorypy.PFStringManipuilation.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFBaseInterface.doctree` & `powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFBaseInterface.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFDynSimInterface.doctree` & `powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFDynSimInterface.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFPlotInterface.doctree` & `powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFPlotInterface.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFStringManipuilation.doctree` & `powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFStringManipuilation.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/doctrees/generated/powfacpy.PFStudyCases.doctree` & `powfacpy-0.2.0/docs/doctrees/generated/powfacpy.PFStudyCases.doctree`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/api.html` & `powfacpy-0.2.0/docs/html/api.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/genindex.html` & `powfacpy-0.2.0/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/how_to_contribute.html` & `powfacpy-0.2.0/docs/html/how_to_contribute.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/index.html` & `powfacpy-0.2.0/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/introduction.html` & `powfacpy-0.2.0/docs/html/introduction.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/objects.inv` & `powfacpy-0.2.0/docs/html/objects.inv`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/search.html` & `powfacpy-0.2.0/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/searchindex.js` & `powfacpy-0.2.0/docs/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/tutorials.html` & `powfacpy-0.2.0/docs/html/tutorials.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_sources/introduction.rst.txt` & `powfacpy-0.2.0/docs/html/_sources/introduction.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_sources/tutorials.rst.txt` & `powfacpy-0.2.0/docs/html/_sources/tutorials.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_sources/generated/powerfactorypy.PFBaseInterface.rst.txt` & `powfacpy-0.2.0/docs/html/_sources/generated/powerfactorypy.PFBaseInterface.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFBaseInterface.rst.txt` & `powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFBaseInterface.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFDynSimInterface.rst.txt` & `powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFDynSimInterface.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFPlotInterface.rst.txt` & `powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFPlotInterface.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_sources/generated/powfacpy.PFStudyCases.rst.txt` & `powfacpy-0.2.0/docs/html/_sources/generated/powfacpy.PFStudyCases.rst.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/_sphinx_javascript_frameworks_compat.js` & `powfacpy-0.2.0/docs/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/basic.css` & `powfacpy-0.2.0/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/doctools.js` & `powfacpy-0.2.0/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/jquery-3.6.0.js` & `powfacpy-0.2.0/docs/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/jquery.js` & `powfacpy-0.2.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/language_data.js` & `powfacpy-0.2.0/docs/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/pygments.css` & `powfacpy-0.2.0/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/searchtools.js` & `powfacpy-0.2.0/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/underscore-1.13.1.js` & `powfacpy-0.2.0/docs/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/underscore.js` & `powfacpy-0.2.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/badge_only.css` & `powfacpy-0.2.0/docs/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/theme.css` & `powfacpy-0.2.0/docs/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `powfacpy-0.2.0/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `powfacpy-0.2.0/docs/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `powfacpy-0.2.0/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `powfacpy-0.2.0/docs/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.eot` & `powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.svg` & `powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.ttf` & `powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.woff` & `powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/fontawesome-webfont.woff2` & `powfacpy-0.2.0/docs/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/lato-bold-italic.woff` & `powfacpy-0.2.0/docs/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/lato-bold-italic.woff2` & `powfacpy-0.2.0/docs/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/lato-bold.woff` & `powfacpy-0.2.0/docs/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/lato-bold.woff2` & `powfacpy-0.2.0/docs/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/lato-normal-italic.woff` & `powfacpy-0.2.0/docs/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/lato-normal-italic.woff2` & `powfacpy-0.2.0/docs/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/lato-normal.woff` & `powfacpy-0.2.0/docs/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/css/fonts/lato-normal.woff2` & `powfacpy-0.2.0/docs/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/js/badge_only.js` & `powfacpy-0.2.0/docs/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/js/html5shiv-printshiv.min.js` & `powfacpy-0.2.0/docs/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/js/html5shiv.min.js` & `powfacpy-0.2.0/docs/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/_static/js/theme.js` & `powfacpy-0.2.0/docs/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/generated/powerfactorypy.PFBaseInterface.html` & `powfacpy-0.2.0/docs/html/generated/powerfactorypy.PFBaseInterface.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/generated/powerfactorypy.PFStringManipuilation.html` & `powfacpy-0.2.0/docs/html/generated/powerfactorypy.PFStringManipuilation.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/generated/powfacpy.PFBaseInterface.html` & `powfacpy-0.2.0/docs/html/generated/powfacpy.PFBaseInterface.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/generated/powfacpy.PFDynSimInterface.html` & `powfacpy-0.2.0/docs/html/generated/powfacpy.PFDynSimInterface.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/generated/powfacpy.PFPlotInterface.html` & `powfacpy-0.2.0/docs/html/generated/powfacpy.PFPlotInterface.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/generated/powfacpy.PFStringManipuilation.html` & `powfacpy-0.2.0/docs/html/generated/powfacpy.PFStringManipuilation.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/html/generated/powfacpy.PFStudyCases.html` & `powfacpy-0.2.0/docs/html/generated/powfacpy.PFStudyCases.html`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/source/conf.py` & `powfacpy-0.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/source/introduction.rst` & `powfacpy-0.2.0/docs/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/source/tutorials.rst` & `powfacpy-0.2.0/docs/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/source/generated/powfacpy.PFBaseInterface.rst` & `powfacpy-0.2.0/docs/source/generated/powfacpy.PFBaseInterface.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/source/generated/powfacpy.PFDynSimInterface.rst` & `powfacpy-0.2.0/docs/source/generated/powfacpy.PFDynSimInterface.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/source/generated/powfacpy.PFPlotInterface.rst` & `powfacpy-0.2.0/docs/source/generated/powfacpy.PFPlotInterface.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/docs/source/generated/powfacpy.PFStudyCases.rst` & `powfacpy-0.2.0/docs/source/generated/powfacpy.PFStudyCases.rst`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/power_factory_objects/CopyOfObjectsInTableOfContentsOfScriptingReference.txt` & `powfacpy-0.2.0/power_factory_objects/CopyOfObjectsInTableOfContentsOfScriptingReference.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmArea.txt` & `powfacpy-0.2.0/result_variables/ElmArea.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmAsm.txt` & `powfacpy-0.2.0/result_variables/ElmAsm.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmAsmsc.txt` & `powfacpy-0.2.0/result_variables/ElmAsmsc.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmBoundary.txt` & `powfacpy-0.2.0/result_variables/ElmBoundary.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmCoup.txt` & `powfacpy-0.2.0/result_variables/ElmCoup.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmGenstat.txt` & `powfacpy-0.2.0/result_variables/ElmGenstat.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmIac.txt` & `powfacpy-0.2.0/result_variables/ElmIac.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmLne.txt` & `powfacpy-0.2.0/result_variables/ElmLne.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmLod.txt` & `powfacpy-0.2.0/result_variables/ElmLod.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmLodlv.txt` & `powfacpy-0.2.0/result_variables/ElmLodlv.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmLodmv.txt` & `powfacpy-0.2.0/result_variables/ElmLodmv.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmPvsys.txt` & `powfacpy-0.2.0/result_variables/ElmPvsys.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmSecctrl.txt` & `powfacpy-0.2.0/result_variables/ElmSecctrl.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmShnt.txt` & `powfacpy-0.2.0/result_variables/ElmShnt.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmSind.txt` & `powfacpy-0.2.0/result_variables/ElmSind.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmStactrl.txt` & `powfacpy-0.2.0/result_variables/ElmStactrl.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmSym.txt` & `powfacpy-0.2.0/result_variables/ElmSym.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmTerm.txt` & `powfacpy-0.2.0/result_variables/ElmTerm.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmTr2.txt` & `powfacpy-0.2.0/result_variables/ElmTr2.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmTr3.txt` & `powfacpy-0.2.0/result_variables/ElmTr3.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmVac.txt` & `powfacpy-0.2.0/result_variables/ElmVac.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmVsc.txt` & `powfacpy-0.2.0/result_variables/ElmVsc.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmVscmono.txt` & `powfacpy-0.2.0/result_variables/ElmVscmono.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmXnet.txt` & `powfacpy-0.2.0/result_variables/ElmXnet.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmZone.txt` & `powfacpy-0.2.0/result_variables/ElmZone.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/result_variables/ElmZpu.txt` & `powfacpy-0.2.0/result_variables/ElmZpu.txt`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/active_project_interface.py` & `powfacpy-0.2.0/src/powfacpy/active_project_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,56 +98,55 @@
         case = self.app.GetActiveStudyCase()
         if case or not error_if_no_active_case:
             return case
         else:
             raise powfacpy.PFNoActiveStudyCaseError()
             
     def get_from_study_case(self,
-                            class_name: str,
-                            if_not_unique: str = "warning", if_no_study_case: str = "error") -> PFGeneral:
+                            name: str,
+                            if_not_unique: str = "warning", 
+                            if_no_study_case: str = "error") -> PFGeneral:
         """Get objects from active study case (similar to PF built-in function 'app.GetFromStudyCase()').
 
         Additionally, this method prints a warning or raises an exception if there is more than one object found in the study case and if no study case is activated.
 
         Args:
-            class_name (str): class name of the object (e.g. 'ElmRes'), optionally preceded by an object name without wildcards and a dot (e.g. 'All Calcualations.ElmRes')
+            name (str): class name of the object (e.g. 'ElmRes'), optionally preceded by an object name without wildcards and a dot (e.g. 'All Calcualations.ElmRes')
 
             if_not_unique (str, optional): Warn ('warning') or raise exception ('error') if there are more than one objets of class 'class_name'. Defaults to "warning".
 
             if_no_study_case (str, optional): Warn ('warning') or raise exception ('error') if no study case is active. Defaults to "error".
 
         Raises:
             powfacpy.PFNoActiveStudyCaseError: No study case activated
             TypeError: More than one object was found
 
         Returns:
             PFGeneral: Found or created object
         """
-        study_case = self.app.GetActiveStudyCase()
-        object = self.app.GetFromStudyCase(class_name)
-
-        if not study_case:
+        object = self.app.GetFromStudyCase(name)
+        
+        if if_no_study_case and not self.app.GetActiveStudyCase(): 
             if if_no_study_case == "warning":
-                warn("No study case activated. PowerFactory creates object of class_name in tmp folder, outside any study case.")
+                    warn("No study case activated. PowerFactory creates object of class_name in tmp folder, outside any study case.")
             elif if_no_study_case == "error":
                 raise powfacpy.PFNoActiveStudyCaseError()
-
-        if if_not_unique:
-            if not '.' in class_name:
-                search_string = "*." + class_name
+           
+        if if_not_unique and self.is_pf_class(name):
+            name = "*." + name
             all_objects_of_this_class = self.get_obj(
-                search_string, parent_folder=object.GetParent(), include_subfolders=False)
+                name, parent_folder=object.GetParent(), include_subfolders=False)
             if len(all_objects_of_this_class) > 1:
                 parent_path = self.get_path_of_object(object.GetParent())
                 if if_not_unique == "warning":
                     warn(
-                        f"The returned {class_name} object is not unique in its folder / in its study case: '{parent_path}'. Make sure that the correct {class_name} object is used.")
+                        f"The returned {name} object is not unique in the  study case: '{parent_path}'. Make sure that the correct {name} object is used.")
                 if if_not_unique == "error":
                     raise TypeError(
-                        f"The returned {class_name} object is not unique in its folder / in its study case: '{parent_path}'")
+                        f"The returned {name} object is not unique in its folder / in its study case: '{parent_path}'")
         return object
 
     def get_results_obj_from_initial_conditions_calc(self) -> ElmRes:
         """Get results object (ElmRes) from the initial conditions calculation object (ComInc). 
 
         This is the results object where results from time domain (RMS/EMT) simulation are written to.
```

### Comparing `powfacpy-0.1.6/src/powfacpy/case_studies.py` & `powfacpy-0.2.0/src/powfacpy/case_studies.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/database_interface.py` & `powfacpy-0.2.0/src/powfacpy/database_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/dyn_sim_interface.py` & `powfacpy-0.2.0/src/powfacpy/dyn_sim_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         
         overwrite (bool, optional): Overwrite existing event with same name. Defaults to True.
     """
     if not parent_folder:
       parent_folder = self.get_events_folder_from_initial_conditions_calc()
     event_obj = self.create_in_folder(name_incl_class, parent_folder, overwrite=overwrite)
     self.set_attr(event_obj, params)  
+    return event_obj
     
       
   def create_event(self, 
                    name_incl_class, 
                    params={}, 
                    parent_folder=None, 
                    overwrite=True):
@@ -111,15 +112,15 @@
       name_incl_class: Event name including the class.
       params: Paramter-values dictionary.
       parent_folder: If None, the events folder from the initial conditions calculation (ComInc) is used.
       overwrite: Oerwrite existing event with same name.
     """
     warn(f'{self.create_event.__name__} will be deprecated. Please use the method create_dyn_sim_event instead.',
              DeprecationWarning, stacklevel=2)
-    self.create_dyn_sim_event(name_incl_class, 
+    return self.create_dyn_sim_event(name_incl_class, 
                               params, 
                               parent_folder,
                               overwrite) 
    
 
   def get_dsl_model_parameter_names(self, dsl_model):
     """
```

### Comparing `powfacpy-0.1.6/src/powfacpy/engineering_helpers.py` & `powfacpy-0.2.0/src/powfacpy/engineering_helpers.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/exceptions.py` & `powfacpy-0.2.0/src/powfacpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/folders_interface.py` & `powfacpy-0.2.0/src/powfacpy/folders_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         """        
         start_obj_or_path = self._folder if not start_obj_or_path else self._handle_single_pf_object_or_path_input(start_obj_or_path)
         obj_or_path = start_obj_or_path.GetParent()
         if obj_or_path:
             if condition(obj_or_path):
                 return obj_or_path
             else:
-                return self.get_upstream_obj(obj_or_path, condition)
+                return self.get_upstream_obj(obj_or_path, condition, error_if_non_existent=error_if_non_existent)
         else:
             if error_if_non_existent:
                 raise Exception(
                     "There is no upstream object that fullfills the condition.")
             else:
                 return None
```

### Comparing `powfacpy-0.1.6/src/powfacpy/functional_interface.py` & `powfacpy-0.2.0/src/powfacpy/functional_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/grouping.py` & `powfacpy-0.2.0/src/powfacpy/grouping.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/model_exchange_interfaces.py` & `powfacpy-0.2.0/src/powfacpy/model_exchange_interfaces.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/network_interface.py` & `powfacpy-0.2.0/src/powfacpy/network_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/pf_class_protocols.py` & `powfacpy-0.2.0/src/powfacpy/pf_class_protocols_old.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/pf_class_protocols_old.py` & `powfacpy-0.2.0/src/powfacpy/pf_class_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,219 +2,219 @@
 """
 
 from typing import Protocol
 
 class PFGeneral(Protocol):
   """Class with general methods (see Section 'General Methods' in scripting reference. All other methods (except for PFApp) inherit from this class). 
   """
-  def MarkInGraphics(*args):
-    ...
-
-  def PasteCopy(*args):
+  def GetOperator(*args):
     ...
 
-  def ReportUnusedObjects(*args):
+  def ShowModalSelectTree(*args):
     ...
 
-  def IsNetworkDataFolder(*args):
+  def GetConnectionCount(*args):
     ...
 
-  def GetAttributeDescription(*args):
+  def GetAttributeShape(*args):
     ...
 
-  def GetSupplyingTransformers(*args):
+  def SwitchOff(*args):
     ...
 
-  def ContainsNonAsciiCharacters(*args):
+  def MarkInGraphics(*args):
     ...
 
-  def IsNode(*args):
+  def HasResults(*args):
     ...
 
-  def IsObjectActive(*args):
+  def IsCalcRelevant(*args):
     ...
 
-  def Isolate(*args):
+  def SearchObject(*args):
     ...
 
-  def GetFullName(*args):
+  def GetAttribute(*args):
     ...
 
-  def GetUnom(*args):
+  def GetAttributes(*args):
     ...
 
-  def GetAttributeLength(*args):
+  def ContainsNonAsciiCharacters(*args):
     ...
 
-  def GetNode(*args):
+  def IsNode(*args):
     ...
 
-  def GetRegion(*args):
+  def GetSystemGrounding(*args):
     ...
 
-  def Delete(*args):
+  def Move(*args):
     ...
 
-  def GetSupplyingSubstations(*args):
+  def GetOwner(*args):
     ...
 
-  def GetChildren(*args):
+  def GetFullName(*args):
     ...
 
-  def GetParent(*args):
+  def GetAttributeLength(*args):
     ...
 
-  def Energize(*args):
+  def GetSupplyingSubstations(*args):
     ...
 
-  def SetAttributes(*args):
+  def IsEnergized(*args):
     ...
 
-  def IsReducible(*args):
+  def SwitchOn(*args):
     ...
 
-  def IsDeleted(*args):
+  def IsObjectActive(*args):
     ...
 
-  def GetAttributeType(*args):
+  def PasteCopy(*args):
     ...
 
-  def GetContents(*args):
+  def GetSupplyingTransformers(*args):
     ...
 
-  def IsOutOfService(*args):
+  def SetAttribute(*args):
     ...
 
   def WriteChangesToDb(*args):
     ...
 
   def GetConnectedElements(*args):
     ...
 
-  def GetCombinedProjectSource(*args):
+  def GetUnom(*args):
     ...
 
-  def ShowModalSelectTree(*args):
+  def SetAttributeLength(*args):
     ...
 
-  def HasAttribute(*args):
+  def ShowEditDialog(*args):
     ...
 
-  def IsObjectModifiedByVariation(*args):
+  def GetAttributeUnit(*args):
     ...
 
-  def SetAttributeLength(*args):
+  def GetContents(*args):
     ...
 
-  def GetAttributeShape(*args):
+  def GetInom(*args):
     ...
 
-  def GetOperator(*args):
+  def GetCombinedProjectSource(*args):
     ...
 
-  def IsEnergized(*args):
+  def CreateObject(*args):
     ...
 
-  def GetControlledNode(*args):
+  def GetChildren(*args):
     ...
 
-  def AddCopy(*args):
+  def HasAttribute(*args):
     ...
 
-  def IsCalcRelevant(*args):
+  def Energize(*args):
     ...
 
-  def GetImpedance(*args):
+  def SetAttributeShape(*args):
     ...
 
-  def SetAttributeShape(*args):
+  def IsNetworkDataFolder(*args):
     ...
 
-  def SetAttribute(*args):
+  def SetAttributes(*args):
     ...
 
-  def ShowEditDialog(*args):
+  def GetClassName(*args):
     ...
 
-  def GetZeroImpedance(*args):
+  def Isolate(*args):
     ...
 
-  def GetClassName(*args):
+  def AddCopy(*args):
     ...
 
-  def GetAttribute(*args):
+  def GetSupplyingTrfstations(*args):
     ...
 
-  def ReplaceNonAsciiCharacters(*args):
+  def GetRegion(*args):
     ...
 
-  def SearchObject(*args):
+  def GetZeroImpedance(*args):
     ...
 
-  def CreateObject(*args):
+  def ReplaceNonAsciiCharacters(*args):
     ...
 
-  def GetCubicle(*args):
+  def IsShortCircuited(*args):
     ...
 
-  def SwitchOff(*args):
+  def ReportUnusedObjects(*args):
     ...
 
-  def ReportNonAsciiCharacters(*args):
+  def IsHidden(*args):
     ...
 
-  def Move(*args):
+  def IsOutOfService(*args):
     ...
 
-  def CopyData(*args):
+  def IsReducible(*args):
     ...
 
-  def GetConnectionCount(*args):
+  def GetAttributeDescription(*args):
     ...
 
   def PurgeUnusedObjects(*args):
     ...
 
-  def GetInom(*args):
+  def GetNode(*args):
     ...
 
-  def GetOwner(*args):
+  def GetReferences(*args):
     ...
 
-  def GetSupplyingTrfstations(*args):
+  def IsDeleted(*args):
     ...
 
-  def IsHidden(*args):
+  def CopyData(*args):
     ...
 
-  def IsInFeeder(*args):
+  def GetControlledNode(*args):
     ...
 
-  def HasResults(*args):
+  def ReportNonAsciiCharacters(*args):
     ...
 
-  def GetSystemGrounding(*args):
+  def GetImpedance(*args):
     ...
 
-  def GetAttributeUnit(*args):
+  def IsInFeeder(*args):
     ...
 
-  def GetAttributes(*args):
+  def GetParent(*args):
     ...
 
-  def SwitchOn(*args):
+  def GetAttributeType(*args):
     ...
 
-  def IsEarthed(*args):
+  def IsObjectModifiedByVariation(*args):
     ...
 
-  def GetReferences(*args):
+  def GetCubicle(*args):
     ...
 
-  def IsShortCircuited(*args):
+  def IsEarthed(*args):
+    ...
+
+  def Delete(*args):
     ...
 
 class PFApp(Protocol):
   __version__: str
 
 
   def ActivateProject(*args):
@@ -19147,14 +19147,17 @@
   updateRng: int
   "Global random number generator: Update global random number generator"
 
 
   def AttributeType(*args):
     ...
 
+  def CompileDynamicModelTypes(*args):
+    ...
+
   def Execute(*args):
     ...
 
   def HasReferences(*args):
     ...
 
   def ZeroDerivative(*args):
@@ -19736,14 +19739,17 @@
 
   def Compare(*args):
     ...
 
   def CompareActive(*args):
     ...
 
+  def CompareRecording(*args):
+    ...
+
   def Execute(*args):
     ...
 
   def ExecuteRecording(*args):
     ...
 
   def ExecuteWithActiveProject(*args):
@@ -20169,14 +20175,17 @@
 
   def AttributeType(*args):
     ...
 
   def Execute(*args):
     ...
 
+  def GetCertificatePath(*args):
+    ...
+
   def HasReferences(*args):
     ...
 
   def ReceiveData(*args):
     ...
 
   def SendData(*args):
@@ -27182,14 +27191,20 @@
 
   def HasReferences(*args):
     ...
 
   def MoveToLayer(*args):
     ...
 
+  def Orthogonalise(*args):
+    ...
+
+  def SnapToGrid(*args):
+    ...
+
   def __getattr__(*args):
     ...
 
 
 
 class IntGrfgroup(PFGeneral):
   charact: list
@@ -30156,14 +30171,17 @@
 
   def GetIntCalcres(*args):
     ...
 
   def HasReferences(*args):
     ...
 
+  def RemoveCurve(*args):
+    ...
+
   def __getattr__(*args):
     ...
 
 
 
 class PltLegend(PFGeneral):
   Internals: list
@@ -35612,14 +35630,3022 @@
     ...
 
   def HasReferences(*args):
     ...
 
   def __getattr__(*args):
     ...
+
+
+
+class ElmSecctrl(PFGeneral):
+  Kpf: float
+  "Active Power Exchange: Frequency Bias"
+  Pexmax: float
+  "Economic Dispatch: Maximum Power Interchange"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  cDisplayName: str
+  "Display Name"
+  cUserDefIndex: int
+  "User defined Index"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  cimRdfId: list
+  "RDF ID"
+  cmo: int
+  "Merit Order"
+  commissionDate: str
+  "Commissioning Date"
+  constr: int
+  "Year of Construction"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Active Power Exchange: Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  cvpp: list
+  "Active Power Percentage"
+  dReserve: float
+  "Economic Dispatch: Minimum Control Reserve"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  iComDate: int
+  "Commissioning Date"
+  iOPFCpsummax: int
+  "Max. Total Active Power Limit"
+  iOPFCpsummin: int
+  "Min. Total Active Power Limit"
+  iSchemeStatus: int
+  "Scheme Status"
+  i_net: int
+  "Control Mode"
+  i_pest: int
+  "Estimate Area Exchange Flow"
+  i_popt: int
+  "Optimise Area Exchange Flow"
+  iexchange: int
+  "Active Power Exchange: Exchange for"
+  imode: int
+  "Active Power Distribution"
+  loc_name: str
+  "Name"
+  manuf: str
+  "Manufacturer"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  pPmeas: object
+  "Active Power Exchange: Boundary/Zone/Area"
+  pid_: int
+  "ProjectID"
+  psetp: float
+  "Active Power Exchange: Power Setpoint"
+  psummax: float
+  "Max. Total Active Power Limit"
+  psummin: float
+  "Min. Total Active Power Limit"
+  psym: list
+  "Machines"
+  qdslCtrl: object
+  "Quasi-Dynamic Model"
+  rembar: object
+  "Busbar for Frequency Measurement"
+  root_id: object
+  "Original Location"
+  sernum: str
+  "Serial Number"
+  tid_: int
+  "TimeID"
+  vpp: list
+  "Active Power Percentage"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
+
+
+
+class ElmLod(PFGeneral):
+  Bc_hv: float
+  "HV Capacitance"
+  Bc_lv: float
+  "Additional LV Capacitance"
+  GPSlat: float
+  "Geographical Position: Latitude / Northing"
+  GPSlon: float
+  "Geographical Position: Longitude / Easting"
+  Iks: float
+  "Fault Contribution Scalable Fault Contribution: Transient Short-Circuit Current"
+  Iksfix: float
+  "Fault Contribution Fixed Fault Contribution: Transient Short-Circuit Level"
+  Iksfixmin: float
+  "Fixed Fault Contribution: Transient Short-Circuit Level"
+  Ikss: float
+  "Fault Contribution Scalable Fault Contribution: Subtransient Short-Circuit Current"
+  Ikssfix: float
+  "Fault Contribution Fixed Fault Contribution: Subtransient Short-Circuit Level"
+  Ikssfixmin: float
+  "Fault Contribution Fixed Fault Contribution: Subtransient Short-Circuit Level"
+  Inom: float
+  "Nominal Current"
+  Irated: float
+  "Harmonic Current Injections: Rated Current"
+  NrCust: int
+  "Number of connected customers"
+  OptCost: int
+  "Interruption costs: Unit"
+  Sks: float
+  "Fault Contribution Scalable Fault Contribution: Transient Short-Circuit Level"
+  Sksfix: float
+  "Fault Contribution Fixed Fault Contribution: Transient Short-Circuit Level"
+  Sksfixmin: float
+  "Fixed Fault Contribution: Transient Short-Circuit Level"
+  Skss: float
+  "Fault Contribution Scalable Fault Contribution: Subtransient Short-Circuit Level"
+  Skssfix: float
+  "Fault Contribution Fixed Fault Contribution: Subtransient Short-Circuit Level"
+  Skssfixmin: float
+  "Fault Contribution Fixed Fault Contribution: Subtransient Short-Circuit Level"
+  Strat: float
+  "Consider Load Transformer: Rated Power"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  bus1: object
+  "Terminal"
+  cBasedOn: float
+  "based on"
+  cDisplayName: str
+  "Display Name"
+  cTrans: float
+  "Load shedding/transfer (Transmission Option): Resulting"
+  cTypHmc: str
+  "Harmonic Current Injections: Type of Harmonic Sources"
+  cUserDefIndex: int
+  "User defined Index"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  cimRdfId: list
+  "RDF ID"
+  classif: str
+  "Load Classification:Agricultural:Domestic:Commercial:Industrial"
+  commissionDate: str
+  "Commissioning Date"
+  constr: int
+  "Year of Construction"
+  coslini: float
+  "Operating Point: Power Factor"
+  coslini_a: float
+  "cos(phi)(act.)"
+  coslinir: float
+  "Phase 1: Power Factor"
+  coslinir_a: float
+  "Ph 1:cos(phi)(act.)"
+  coslinis: float
+  "Phase 2: Power Factor"
+  coslinis_a: float
+  "Ph 2:cos(phi)(act.)"
+  coslinit: float
+  "Phase 3: Power Factor"
+  coslinit_a: float
+  "Ph 3:cos(phi)(act.)"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  ctotIks: float
+  "Fault Contribution: Total contribution (transient)"
+  ctotIksmin: float
+  "Total contribution (transient)"
+  ctotIkss: float
+  "Fault Contribution: Total contribution (subtransient)"
+  ctotIkssmin: float
+  "Fault Contribution: Total contribution (subtransient)"
+  ctotSks: float
+  "Fault Contribution: Total contribution (transient)"
+  ctotSksmin: float
+  "Total contribution (transient)"
+  ctotSkss: float
+  "Fault Contribution: Total contribution (subtransient)"
+  ctotSkssmin: float
+  "Fault Contribution: Total contribution (subtransient)"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  dpl1: float
+  "dpl1"
+  dpl2: float
+  "dpl2"
+  dpl3: float
+  "dpl3"
+  dpl4: float
+  "dpl4"
+  dpl5: float
+  "dpl5"
+  dudropLVfeed: float
+  "LV Voltage Changes: Maximum Voltage Drop (LV Grid)"
+  duriseLVfeed: float
+  "LV Voltage Changes: Maximum Voltage Rise (LV Grid)"
+  fSCDF: float
+  "Interruption costs: Scaling factor"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  iAstabint: int
+  "A-stable integration algorithm"
+  iComDate: int
+  "Commissioning Date"
+  iLoadTrf: int
+  "Consider Load Transformer"
+  iSchemeStatus: int
+  "Scheme Status"
+  iShedding: int
+  "Controls: Allow load shedding"
+  i_normPQext: int
+  "Pext, Qext input signals normalised to load flow voltage"
+  i_pini: int
+  "State Estimation Active/Reactive Power: Estimate Active Power"
+  i_prty: int
+  "Priority"
+  i_qini: int
+  "State Estimation Active/Reactive Power: Estimate Reactive Power"
+  i_rem: int
+  "Remote Control"
+  i_scale: int
+  "Operating Point: Adjusted by Load Scaling"
+  i_scaleini: int
+  "State Estimation Scaling Factor: Estimate Scaling Factor"
+  i_sym: int
+  "Balanced/Unbalanced"
+  icurref: int
+  "Harmonic Current Injections: Harmonic currents referred to"
+  iecShcModel: int
+  "Fault Contribution: Short-Circuit Model:Static converter-fed drive:Equivalent synchronous machine"
+  iecfltcont: int
+  "Fault Contribution"
+  ilini: float
+  "Operating Point: Current"
+  ilini_a: float
+  "I(act.)"
+  ilinir: float
+  "Phase 1: Current"
+  ilinir_a: float
+  "Ph 1:I(act.)"
+  ilinis: float
+  "Phase 2: Current"
+  ilinis_a: float
+  "Ph 2:I(act.)"
+  ilinit: float
+  "Phase 3: Current"
+  ilinit_a: float
+  "Ph 3:I(act.)"
+  iopt_type: int
+  "Allow Load-Ramp Event"
+  isCtrlLdShed: int
+  "Controls for Unit Commitment: Allow load shedding"
+  loc_name: str
+  "Name"
+  mode_inp: str
+  "Input Mode"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  pSCDF: object
+  "Interruption costs: Tariff"
+  pTrans: object
+  "Load shedding/transfer (Transmission Option): Alternative Supply (Load)"
+  p_cub: object
+  "Controlled Branch (Cubicle)"
+  p_direc: int
+  "Operating Point: Power Direction:P>=0:P<0"
+  p_direcr: int
+  "Phase 1: Power Direction:P>=0:P<0"
+  p_direcs: int
+  "Phase 2: Power Direction:P>=0:P<0"
+  p_direct: int
+  "Phase 3: Power Direction:P>=0:P<0"
+  pcontract: float
+  "Contracted Active Power"
+  pf_recap: int
+  "Operating Point: Power Factor:ind.:cap."
+  pf_recapr: int
+  "Phase 1: Power Factor:ind.:cap."
+  pf_recaps: int
+  "Phase 2: Power Factor:ind.:cap."
+  pf_recapt: int
+  "Phase 3: Power Factor:ind.:cap."
+  phmc: object
+  "Harmonic Current Injections: Harmonic Currents"
+  phtech: str
+  "Technology"
+  pid_: int
+  "ProjectID"
+  plini: float
+  "Operating Point: Active Power"
+  plini_a: float
+  "P(act.)"
+  plinir: float
+  "Phase 1: Active Power"
+  plinir_a: float
+  "Ph 1:P(act.)"
+  plinis: float
+  "Phase 2: Active Power"
+  plinis_a: float
+  "Ph 2:P(act.)"
+  plinit: float
+  "Phase 3: Active Power"
+  plinit_a: float
+  "Ph 3:P(act.)"
+  qdslCtrl: object
+  "Quasi-Dynamic Model"
+  qlini: float
+  "Operating Point: Reactive Power"
+  qlini_a: float
+  "Q(act.)"
+  qlinir: float
+  "Phase 1: Reactive Power"
+  qlinir_a: float
+  "Ph 1:Q(act.)"
+  qlinis: float
+  "Phase 2: Reactive Power"
+  qlinis_a: float
+  "Ph 2:Q(act.)"
+  qlinit: float
+  "Phase 3: Reactive Power"
+  qlinit_a: float
+  "Ph 3:Q(act.)"
+  r0: float
+  "Consider Load Transformer: r0"
+  r1Sbasepu: float
+  "r1(shc) (Sbase)"
+  r2Sbasepu: float
+  "r2(shc) (Sbase)"
+  ramp_type: int
+  "Allow Load-Ramp Event"
+  root_id: object
+  "Original Location"
+  rtox: float
+  "Fault Contribution: R to X'' ratio"
+  rtoxmin: float
+  "Fault Contribution: R to X'' ratio"
+  scale0: float
+  "Operating Point: Scaling Factor"
+  scale0_a: float
+  "Scaling Factor(act.)"
+  sernum: str
+  "Serial Number"
+  shed: int
+  "Load shedding/transfer (Transmission Option): Shedding steps:infinite:1:2:3:4:5:6:7:8:9:10"
+  shedcost: float
+  "Costs: Costs for load shedding"
+  shedmax: float
+  "Load shedding constraints for apparent power: Max. load shedding"
+  shedmin: float
+  "Load shedding constraints for apparent power: Min. load shedding"
+  slini: float
+  "Operating Point: Apparent Power"
+  slini_a: float
+  "S(act.)"
+  slinir: float
+  "Phase 1: Apparent Power"
+  slinir_a: float
+  "Ph 1:S(act.)"
+  slinis: float
+  "Phase 2: Apparent Power"
+  slinis_a: float
+  "Ph 2:S(act.)"
+  slinit: float
+  "Phase 3: Apparent Power"
+  slinit_a: float
+  "Ph 3:S(act.)"
+  tid_: int
+  "TimeID"
+  trans: float
+  "Load shedding/transfer (Transmission Option): Transferable"
+  typ_id: object
+  "Type"
+  u0: float
+  "Operating Point: Voltage"
+  x0: float
+  "Consider Load Transformer: x0"
+  x1sSbasepu: float
+  "x1'(shc) (Sbase)"
+  x1ssSbasepu: float
+  "x1''(shc) (Sbase)"
+  x2Sbasepu: float
+  "x2(shc) (Sbase)"
+  xt: float
+  "Load Transformer Reactance"
+  xtor: float
+  "Fault Contribution: X'' to R ratio"
+  xtormin: float
+  "Fault Contribution: X'' to R ratio"
+  zonefact: float
+  "Zone Scaling Factor:"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
+
+
+
+class ElmIac(PFGeneral):
+  B0: float
+  "Zero Sequence: Internal Susceptance, B0"
+  B1: float
+  "Positive Sequence: Internal Susceptance, B1"
+  B2: float
+  "Negative Sequence: Internal Susceptance, B2"
+  G0: float
+  "Zero Sequence: Internal Conductance, G0"
+  G1: float
+  "Positive Sequence: Internal Conductance, G1"
+  G2: float
+  "Negative Sequence: Internal Conductance, G2"
+  GPSlat: float
+  "Geographical Position: Latitude / Northing"
+  GPSlon: float
+  "Geographical Position: Longitude / Easting"
+  Inom: float
+  "Nominal Current"
+  Ir: float
+  "Rated Current"
+  Irated: float
+  "Harmonic Current Injections: Rated Current"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  bus1: object
+  "Terminal"
+  cDisplayName: str
+  "Display Name"
+  cTypHmc: str
+  "Harmonic Current Injections: Type of Harmonic Sources"
+  cUserDefIndex: int
+  "User defined Index"
+  c_pmod: object
+  "Model"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  commissionDate: str
+  "Commissioning Date"
+  constr: int
+  "Year of Construction"
+  cosimModel: int
+  "Used for Co-simulation"
+  cosini: float
+  "Positive Sequence: Power Factor"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  dcurdf: float
+  "Frequency Sweep Calculation only: Spectral Density of Current Magnitude"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  dphidf: float
+  "Frequency Sweep Calculation only: Spectral Density of Current Angle"
+  fchardcur: object
+  "Frequency Sweep Calculation only: Frequency Dependency"
+  fchardphi: object
+  "Frequency Sweep Calculation only: Frequency Dependency"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  iAstabint: int
+  "A-stable integration algorithm"
+  iComDate: int
+  "Commissioning Date"
+  iSchemeStatus: int
+  "Scheme Status"
+  i_cap: int
+  "Positive Sequence: Reactive Power:inductive:capacitive"
+  icurref: int
+  "Harmonic Current Injections: Harmonic currents referred to"
+  isetp: float
+  "Positive Sequence: Current Setpoint"
+  isetp0: float
+  "Zero Sequence: Current, Magnitude"
+  isetp2: float
+  "Negative Sequence: Current, Magnitude"
+  leadFinput: int
+  "Parameter event can be applied to: Frequency input:F0Hz (in Hz):f0 (in p.u.)"
+  leadIinput: int
+  "Parameter event can be applied to: Current input"
+  loc_name: str
+  "Name"
+  manuf: str
+  "Manufacturer"
+  nphase: int
+  "No. of Phases:1:3"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  phisetp0: float
+  "Zero Sequence: Current, Angle"
+  phisetp2: float
+  "Negative Sequence: Current, Angle"
+  phmc: object
+  "Harmonic Current Injections: Harmonic Currents"
+  pid_: int
+  "ProjectID"
+  qdslCtrl: object
+  "Quasi-Dynamic Model"
+  root_id: object
+  "Original Location"
+  sernum: str
+  "Serial Number"
+  tid_: int
+  "TimeID"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
+
+
+
+class ElmLodlv(PFGeneral):
+  GPSlat: float
+  "Geographical Position: Latitude / Northing"
+  GPSlon: float
+  "Geographical Position: Longitude / Easting"
+  NrCust: int
+  "Number of Customers"
+  OptCost: int
+  "Interruption costs: Unit"
+  UtilFactor: float
+  "Load per customer: Utilisation Factor"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  bus1: object
+  "Terminal"
+  cDisplayName: str
+  "Display Name"
+  cHasPartLod: int
+  "Partial Loads Present"
+  cNrCust: int
+  "Load per customer: Number of Customers"
+  cPartLod: list
+  "Partial Loads:"
+  cPmaxLV: float
+  "Active power, P, with coincidence"
+  cPrCust: float
+  "Load per customer: P/Customer"
+  cPsumLV: float
+  "Resulting values: Active power, P, theoretical"
+  cSav: float
+  "Load per customer: Average Load"
+  cSmax: float
+  "Load per customer: Max. Load per Customer"
+  cSmaxLV: float
+  "Resulting values: Apparent power, S, with coincidence"
+  cSsumLV: float
+  "Resulting values: Apparent power, S, theoretical"
+  cTrans: float
+  "Load shedding/transfer (Transmission Option): Resulting"
+  cUserDefIndex: int
+  "User defined Index"
+  ccosphi: float
+  "Load per customer: Power Factor"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  cimRdfId: list
+  "RDF ID"
+  classif: str
+  "Load Classification:Agricultural:Domestic:Commercial:Industrial"
+  commissionDate: str
+  "Commissioning Date"
+  constr: int
+  "Year of Construction"
+  coslini: float
+  "Base Load: Power Factor, cos(phi)"
+  coslini_a: float
+  "cos(phi)(act.)"
+  coslinir: float
+  "Base Load Phase 1: Power Factor, cos(phi)"
+  coslinir_a: float
+  "Ph 1:cos(phi)(act.)"
+  coslinis: float
+  "Base Load Phase 2: Power Factor, cos(phi)"
+  coslinis_a: float
+  "Ph 2:cos(phi)(act.)"
+  coslinit: float
+  "Base Load Phase 3: Power Factor, cos(phi)"
+  coslinit_a: float
+  "Ph 3:cos(phi)(act.)"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  cplinia: float
+  "Base Load: P, Load"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  dpl1: float
+  "dpl1"
+  dpl2: float
+  "dpl2"
+  dpl3: float
+  "dpl3"
+  dpl4: float
+  "dpl4"
+  dpl5: float
+  "dpl5"
+  dudropLVfeed: float
+  "LV Voltage Changes: Maximum Voltage Drop (LV Grid)"
+  duriseLVfeed: float
+  "LV Voltage Changes: Maximum Voltage Rise (LV Grid)"
+  elini: float
+  "Base Load: Yearly Energy"
+  fSCDF: float
+  "Interruption costs: Scaling factor"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  iBaseIsMax: int
+  "Individual power consumption: Use consumption as:Theoretical sum:Maximum per customer:Maximum with coincidence:Average (value for ginf)"
+  iCoincFrom: int
+  "Coincidence definition: Used coincidence definition:From type:Individual:None"
+  iComDate: int
+  "Commissioning Date"
+  iLV: int
+  "Coincidence definition: Consider coincidence"
+  iSchemeStatus: int
+  "Scheme Status"
+  iShedding: int
+  "Controls: Allow load shedding"
+  i_prty: int
+  "Priority"
+  i_scale: int
+  "Base Load: Adjusted by Load Scaling"
+  i_scalep: int
+  "Adjusted by Load Scaling"
+  i_sym: int
+  "Base Load: Balanced/Unbalanced:Balanced:Unbalanced"
+  iintgnd: int
+  "External Star Point"
+  ilini: float
+  "Base Load: Current, I"
+  ilini_a: float
+  "I(act.)"
+  ilinir: float
+  "Base Load Phase 1: Current, I"
+  ilinir_a: float
+  "Ph 1:I(act.)"
+  ilinis: float
+  "Base Load Phase 2: Current, I"
+  ilinis_a: float
+  "Ph 2:I(act.)"
+  ilinit: float
+  "Base Load Phase 3: Current, I"
+  ilinit_a: float
+  "Ph 3:I(act.)"
+  indivPower: int
+  "Individual power consumption"
+  iopt_inp: int
+  "Base Load: Input Mode"
+  iopt_type: int
+  "Allow Load-Ramp Event"
+  isCtrlLdShed: int
+  "Controls: Allow load shedding"
+  loc_name: str
+  "Name"
+  lodparts: list
+  "Partial Loads"
+  nphase: int
+  "No. of Phases:1:2:3"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pCoincDef: object
+  "Coincidence definition: Individual coincidence definition"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  pProfile: object
+  "Base Load: Consumption Profile"
+  pProfileRnd: float
+  "Active Power for Probabilistic Analysis, P"
+  pSCDF: object
+  "Interruption costs: Tariff"
+  pTrans: object
+  "Load shedding/transfer (Transmission Option): Alternative Supply (Load)"
+  pTypCoincDef: object
+  "Coincidence definition: Coincidence definition from type"
+  pcontract: float
+  "Contracted Active Power"
+  peakCorrFac: float
+  "Individual power consumption: Additional scaling factor"
+  pf_recap: int
+  "Base Load: Power Factor:ind.:cap."
+  pf_recapr: int
+  "Base Load Phase 1: Power Factor:ind.:cap."
+  pf_recaps: int
+  "Base Load Phase 2: Power Factor:ind.:cap."
+  pf_recapt: int
+  "Base Load Phase 3: Power Factor:ind.:cap."
+  phtech: int
+  "Technology"
+  pid_: int
+  "ProjectID"
+  plini: float
+  "Base Load: Active Power, P"
+  plini_a: float
+  "P(act.)"
+  plinir: float
+  "Base Load Phase 1: Active Power, P"
+  plinir_a: float
+  "Ph 1:P(act.)"
+  plinis: float
+  "Base Load Phase 2: Active Power, P"
+  plinis_a: float
+  "Ph 2:P(act.)"
+  plinit: float
+  "Base Load Phase 3: Active Power, P"
+  plinit_a: float
+  "Ph 3:P(act.)"
+  pnight: float
+  "Night Storage Heater: P"
+  pnight_a: float
+  "P(night)(act.)"
+  qdslCtrl: object
+  "Quasi-Dynamic Model"
+  root_id: object
+  "Original Location"
+  scale0: float
+  "Base Load: Scaling Factor"
+  scale0_a: float
+  "Scaling Factor(act.)"
+  sernum: str
+  "Serial Number"
+  shed: int
+  "Load shedding/transfer (Transmission Option): Shedding steps:infinite:1:2:3:4:5:6:7:8:9:10"
+  shedcost: float
+  "Costs: Costs for load shedding"
+  shedmax: float
+  "Constraints: Max. load shedding"
+  shedmin: float
+  "Constraints: Min. load shedding"
+  slini: float
+  "Base Load: Apparent Power, S"
+  slini_a: float
+  "S(act.)"
+  slinir: float
+  "Base Load Phase 1: Apparent Power, S"
+  slinir_a: float
+  "Ph 1:S(act.)"
+  slinis: float
+  "Base Load Phase 2: Apparent Power, S"
+  slinis_a: float
+  "Ph 2:S(act.)"
+  slinit: float
+  "Base Load Phase 3: Apparent Power, S"
+  slinit_a: float
+  "Ph 3:S(act.)"
+  tid_: int
+  "TimeID"
+  trans: float
+  "Load shedding/transfer (Transmission Option): Transferable"
+  typ_id: object
+  "Type"
+  ulini: float
+  "Base Load: Voltage, U(L-L)"
+  ulini_a: float
+  "U(L-L)(act.)"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
+
+
+
+class ElmLodmv(PFGeneral):
+  CCEarFr: float
+  "Failures of Transformer Double Earth Fault: Frequency of single earth faults"
+  CCEarProb: float
+  "Failures of Transformer Double Earth Fault: Conditional probability of a second earth fault"
+  CCEarRepMu: float
+  "Failures of Transformer Double Earth Fault: Repair duration"
+  FOD: float
+  "Failures of Transformer Transformer Failures: Forced Outage Duration"
+  FOE: float
+  "Failures of Transformer Transformer Failures: Forced Outage Expectancy"
+  FOR1: float
+  "Failures of Transformer Transformer Failures: Forced Complete Outage Rate"
+  GPSlat: float
+  "Geographical Position: Latitude / Northing"
+  GPSlon: float
+  "Geographical Position: Longitude / Easting"
+  Iksfix: float
+  "Fault Contribution Fixed Fault Contribution: Transient Short-Circuit Level"
+  Iksgen: float
+  "Fault Contribution Scalable Fault Contribution for Generation: Transient Short-Circuit Current"
+  Ikslod: float
+  "Fault Contribution Scalable Fault Contribution for Load: Transient Short-Circuit Current"
+  Ikssfix: float
+  "Fault Contribution Fixed Fault Contribution: Subtransient Short-Circuit Level"
+  Ikssgen: float
+  "Fault Contribution Scalable Fault Contribution for Generation: Subtransient Short-Circuit Current"
+  Iksslod: float
+  "Fault Contribution Scalable Fault Contribution for Load: Subtransient Short-Circuit Current"
+  Inom: float
+  "Nominal Current"
+  Irated: float
+  "Harmonic Current Injections: Rated Current"
+  NrCust: int
+  "Number of connected customers"
+  Pcu: float
+  "Series Reactor: Copper Losses"
+  Sksfix: float
+  "Fault Contribution Fixed Fault Contribution: Transient Short-Circuit Level"
+  Sksgen: float
+  "Fault Contribution Scalable Fault Contribution for Generation: Transient Short-Circuit Level"
+  Skslod: float
+  "Fault Contribution Scalable Fault Contribution for Load: Transient Short-Circuit Level"
+  Skssfix: float
+  "Fault Contribution Fixed Fault Contribution: Subtransient Short-Circuit Level"
+  Skssgen: float
+  "Fault Contribution Scalable Fault Contribution for Generation: Subtransient Short-Circuit Level"
+  Sksslod: float
+  "Fault Contribution Scalable Fault Contribution for Load: Subtransient Short-Circuit Level"
+  Srated: float
+  "Rated Power"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  bus1: object
+  "Terminal"
+  cDisplayName: str
+  "Display Name"
+  cTrans: float
+  "Load shedding/transfer (Transmission Option): Resulting"
+  cTypHmc: str
+  "Harmonic Current Injections: Type of Harmonic Sources"
+  cUserDefIndex: int
+  "User defined Index"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  ci_sym: int
+  "Balanced/Unbalanced"
+  cimRdfId: list
+  "RDF ID"
+  classif: str
+  "Load Classification:Agricultural:Domestic:Commercial:Industrial"
+  commissionDate: str
+  "Commissioning Date"
+  constr: int
+  "Year of Construction"
+  cosgini: float
+  "Operating Point: cos(phi), Generation"
+  cosgini_a: float
+  "cos(phi)(act.), Gen."
+  cosginir: float
+  "Phase 1: cos(phi), Generation"
+  cosginir_a: float
+  "Ph 1:cos(phi)(act.), Gen."
+  cosginis: float
+  "Phase 2: cos(phi), Generation"
+  cosginis_a: float
+  "Ph 2:cos(phi)(act.), Gen."
+  cosginit: float
+  "Phase 3: cos(phi), Generation"
+  cosginit_a: float
+  "Ph 3:cos(phi)(act.), Gen."
+  coslini: float
+  "Operating Point: cos(phi), Load"
+  coslini_a: float
+  "cos(phi)(act.)"
+  coslinir: float
+  "Phase 1: cos(phi), Load"
+  coslinir_a: float
+  "Ph 1:cos(phi)(act.)"
+  coslinis: float
+  "Phase 2: cos(phi), Load"
+  coslinis_a: float
+  "Ph 2:cos(phi)(act.)"
+  coslinit: float
+  "Phase 3: cos(phi), Load"
+  coslinit_a: float
+  "Ph 3:cos(phi)(act.)"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteo: object
+  "Meteo Station"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  cplinia: float
+  "Operating Point: P, Load"
+  csrated: float
+  "Rated Power"
+  ctotIks: float
+  "Fault Contribution: Total Transient Fault Contribution"
+  ctotIkss: float
+  "Fault Contribution: Total Subtransient Fault Contribution"
+  ctotSks: float
+  "Fault Contribution: Total Transient Fault Contribution"
+  ctotSkss: float
+  "Fault Contribution: Total Subtransient Fault Contribution"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  dpl1: float
+  "dpl1"
+  dpl2: float
+  "dpl2"
+  dpl3: float
+  "dpl3"
+  dpl4: float
+  "dpl4"
+  dpl5: float
+  "dpl5"
+  dsdtemp: float
+  "Temperature Gradient"
+  dudropLVfeed: float
+  "LV Voltage Changes: Maximum Voltage Drop (LV Grid)"
+  dudropTrf: float
+  "Voltage Change over Transformer: Transformer Voltage Drop in Consumption Case"
+  duriseLVfeed: float
+  "LV Voltage Changes: Maximum Voltage Rise (LV Grid)"
+  duriseTrf: float
+  "Voltage Change over Transformer: Transformer Voltage Rise in Production Case"
+  elini: float
+  "Operating Point: Yearly Energy"
+  fSCDF: float
+  "Interruption costs: Scaling factor"
+  fcharr1: object
+  "Norton Equivalent: Frequency-Dependence, r1(f)"
+  fcharx1: object
+  "Norton Equivalent: Frequency-Dependence, x1(f)"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  gscale: float
+  "Operating Point: Generation Scaling Factor"
+  gscale_a: float
+  "Gen. Scaling Factor(act.)"
+  iComDate: int
+  "Commissioning Date"
+  iSchemeStatus: int
+  "Scheme Status"
+  iShedding: int
+  "Controls: Allow load shedding"
+  i_csrc: int
+  "Load Model"
+  i_prty: int
+  "Priority"
+  i_pure: int
+  "Load Model"
+  i_scale: int
+  "Operating Point: Adjusted by Load Scaling"
+  i_sym: int
+  "Balanced/Unbalanced"
+  icurref: int
+  "Harmonic Current Injections: Harmonic currents referred to"
+  iopt_type: int
+  "Allow Load-Ramp Event"
+  iperfect: int
+  "Failures of Transformer: Ideal component"
+  isCtrlLdShed: int
+  "Controls: Allow load shedding"
+  loc_name: str
+  "Name"
+  mode_inp: str
+  "Input Mode"
+  nntap: int
+  "Tap: Tap Position"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pMeteo: object
+  "Meteo Station"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  pProfile: object
+  "Operating Point: Consumption Profile"
+  pProfileRnd: float
+  "Active Power for Probabilistic Analysis, P"
+  pSCDF: object
+  "Interruption costs: Tariff"
+  pStoch: object
+  "Failures of Transformer: Element model"
+  pTrans: object
+  "Load shedding/transfer (Transmission Option): Alternative Supply (Load)"
+  pTypStoch: object
+  "Failures of Transformer: Type model"
+  pcontract: float
+  "Contracted Active Power"
+  pf_recap: int
+  "Operating Point: cos(phi), Load:ind.:cap."
+  pf_recapr: int
+  "Phase 1: cos(phi), Load:ind.:cap."
+  pf_recaps: int
+  "Phase 2: cos(phi), Load:ind.:cap."
+  pf_recapt: int
+  "Phase 3: cos(phi), Load:ind.:cap."
+  pfg_recap: int
+  "Operating Point: cos(phi), Generation:ind.:cap."
+  pfg_recapr: int
+  "Phase 1: cos(phi), Generation:ind.:cap."
+  pfg_recaps: int
+  "Phase 2: cos(phi), Generation:ind.:cap."
+  pfg_recapt: int
+  "Phase 3: cos(phi), Generation:ind.:cap."
+  pgini: float
+  "Operating Point: P, Generation"
+  pgini_a: float
+  "Pgen(act.)"
+  pginir: float
+  "Phase 1: P, Generation"
+  pginir_a: float
+  "Ph 1:Pgen(act.)"
+  pginis: float
+  "Phase 2: P, Generation"
+  pginis_a: float
+  "Ph 2:Pgen(act.)"
+  pginit: float
+  "Phase 3: P, Generation"
+  pginit_a: float
+  "Ph 3:Pgen(act.)"
+  pgrd: float
+  "Capacitive/Inductive Reactive Power: QL/QC"
+  phmc: object
+  "Harmonic Current Injections: Harmonic Currents"
+  phtech: str
+  "Technology"
+  pid_: int
+  "ProjectID"
+  plini: float
+  "Operating Point: P, Load"
+  plini_a: float
+  "P(act.)"
+  plinir: float
+  "Phase 1: P, Load"
+  plinir_a: float
+  "Ph 1:P(act.)"
+  plinis: float
+  "Phase 2: P, Load"
+  plinis_a: float
+  "Ph 2:P(act.)"
+  plinit: float
+  "Phase 3: P, Load"
+  plinit_a: float
+  "Ph 3:P(act.)"
+  qcq: float
+  "Capacitive/Inductive Reactive Power: QC/Q"
+  qdslCtrl: object
+  "Quasi-Dynamic Model"
+  r1hmc: float
+  "Norton Equivalent: Resistance, r1"
+  r2: float
+  "Negative Sequence Impedance: Resistance r2"
+  root_id: object
+  "Original Location"
+  rtox: float
+  "Fault Contribution: R to X'' ratio"
+  scale0: float
+  "Operating Point: Load Scaling Factor"
+  scale0_a: float
+  "Scaling Factor(act.)"
+  sernum: str
+  "Serial Number"
+  sgini: float
+  "Operating Point: S, Generation"
+  sgini_a: float
+  "Sgen(act.)"
+  sginir: float
+  "Phase 1: S, Generation"
+  sginir_a: float
+  "Ph 1:Sgen(act.)"
+  sginis: float
+  "Phase 2: S, Generation"
+  sginis_a: float
+  "Ph 2:Sgen(act.)"
+  sginit: float
+  "Phase 3: S, Generation"
+  sginit_a: float
+  "Ph 3:Sgen(act.)"
+  shed: int
+  "Load shedding/transfer (Transmission Option): Shedding steps:infinite:1:2:3:4:5:6:7:8:9:10"
+  shedcost: float
+  "Costs: Costs for load shedding"
+  shedmax: float
+  "Constraints: Max. load shedding"
+  shedmin: float
+  "Constraints: Min. load shedding"
+  slini: float
+  "Operating Point: S, Load"
+  slini_a: float
+  "S(act.)"
+  slinir: float
+  "Phase 1: S, Load"
+  slinir_a: float
+  "Ph 1:S(act.)"
+  slinis: float
+  "Phase 2: S, Load"
+  slinis_a: float
+  "Ph 2:S(act.)"
+  slinit: float
+  "Phase 3: S, Load"
+  slinit_a: float
+  "Ph 3:S(act.)"
+  tid_: int
+  "TimeID"
+  trans: float
+  "Load shedding/transfer (Transmission Option): Transferable"
+  typ_id: object
+  "Type"
+  uk: float
+  "Series Reactor: Short Circuit Impedance"
+  x1hmc: float
+  "Norton Equivalent: Reactance, x1"
+  x2: float
+  "Negative Sequence Impedance: Reactance x2"
+  xtor: float
+  "Fault Contribution: X'' to R ratio"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
+
+
+
+class ElmSind(PFGeneral):
+  CCEarFr: float
+  "Failures Double Earth Fault: Frequency of single earth faults"
+  CCEarProb: float
+  "Failures Double Earth Fault: Conditional probability of a second earth fault"
+  CCEarRepMu: float
+  "Failures Double Earth Fault: Repair duration"
+  Curn: float
+  "Ratings: Rated Current"
+  FOD: float
+  "Failures: Forced Outage Duration"
+  FOE: float
+  "Failures: Forced Outage Expectancy"
+  FOR1: float
+  "Failures: Forced Outage Rate"
+  GPSlat: float
+  "Geographical Position: Latitude / Northing"
+  GPSlon: float
+  "Geographical Position: Longitude / Easting"
+  Inom: float
+  "Nominal Current"
+  InomPre: float
+  "Pre-fault nominal current"
+  Lf: float
+  "Frequency Dependencies: Inductance, L"
+  Lf0: float
+  "Frequency Dependencies: Inductance, L0"
+  Lwidth: float
+  "Hysteresis: Loop width"
+  Pcu: float
+  "Impedance: Copper Losses"
+  PsiresA: float
+  "Residual flux: Residual flux, ph. A"
+  PsiresB: float
+  "Residual flux: Residual flux, ph. B"
+  PsiresC: float
+  "Residual flux: Residual flux, ph. C"
+  R0toR1: float
+  "Zero sequence impedance: R0/R1 ratio"
+  Rf: float
+  "Frequency Dependencies: Resistance, R"
+  Rf0: float
+  "Frequency Dependencies: Resistance, R0"
+  Sn: float
+  "Ratings: Rated Power"
+  X0toX1: float
+  "Zero sequence impedance: X0/X1 ratio"
+  Zd: float
+  "Impedance: Impedance (absolute) Zd"
+  aFrolich: float
+  "Frolich equation coefficient a"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  bFrolich: float
+  "Frolich equation coefficient b"
+  bus1: object
+  "Terminal i"
+  bus2: object
+  "Terminal j"
+  cDisplayName: str
+  "Display Name"
+  cFrolich: float
+  "Frolich equation coefficient c"
+  cPsiresC: float
+  "Residual flux: Residual flux, ph. C"
+  cUserDefIndex: int
+  "User defined Index"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  cimRdfId: list
+  "RDF ID"
+  cknee: float
+  "Knee Current"
+  commissionDate: str
+  "Commissioning Date"
+  constr: int
+  "Year of Construction"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  emtLinSig: int
+  "Variable inductance/reactance via input signals"
+  fcharL: object
+  "Frequency Dependencies: L(f)"
+  fcharL0: object
+  "Frequency Dependencies: L0(f)"
+  fcharR: object
+  "Frequency Dependencies: R(f)"
+  fcharR0: object
+  "Frequency Dependencies: R0(f)"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  iAreaBus: int
+  "Area"
+  iAstabint: int
+  "A-stable integration algorithm"
+  iComDate: int
+  "Commissioning Date"
+  iFinalSlope: int
+  "Set final slope (peak values)"
+  iFit: int
+  "Data fitting:Piecewise linear:Frolich:Modified Frolich"
+  iHyster: int
+  "Hysteresis: Model:None:History Independent"
+  iInterPol: int
+  "Interpolation:spline:piecewise linear"
+  iLimb: int
+  "Core:&3&3 Limb:&5&5 Limb"
+  iResFlux: int
+  "Residual flux"
+  iSchemeStatus: int
+  "Scheme Status"
+  iZoneBus: int
+  "Zone"
+  iperfect: int
+  "Failures: Ideal component"
+  itrmt: int
+  "Type"
+  ksat: int
+  "Saturation Exponent"
+  loc_name: str
+  "Name"
+  lossAssign: int
+  "Loss assignment:according to grouping:uniformly distributed:to Terminal i:to Terminal j"
+  lrea: float
+  "Impedance: Inductance, L"
+  manuf: str
+  "Manufacturer"
+  maxload: float
+  "Thermal Loading Limit: Max. Loading"
+  mseFrolich: float
+  "Frolich equation, mean squared error"
+  nphases: int
+  "Phases:1:3"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  pRating: object
+  "Thermal Rating"
+  pStoch: object
+  "Failures: Element model"
+  pid_: int
+  "ProjectID"
+  psi0: float
+  "Knee Flux"
+  root_id: object
+  "Original Location"
+  rrea: float
+  "Impedance: Resistance, R"
+  satcue: list
+  "Current (RMS)"
+  satcur: list
+  "Current (peak)"
+  satflux: list
+  "Flux (peak)"
+  satvol: list
+  "Voltage (RMS)"
+  sernum: str
+  "Serial Number"
+  smoothfac: float
+  "Smoothing Factor"
+  systp: int
+  "System Type:AC:DC:AC/BI"
+  tid_: int
+  "TimeID"
+  ucn: float
+  "Ratings: Rated Voltage"
+  uk: float
+  "Impedance: Short-Circuit Voltage uk"
+  ukr: float
+  "Impedance: Short-Circuit Voltage (Re(uk)) ukr"
+  xmair: float
+  "Saturated Reactance"
+  xrea: float
+  "Impedance: Reactance, X"
+  xreapu: float
+  "Linear Reactance"
+  xsatFrolich: float
+  "Frolich equation saturated reactance (p.u.)"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
+
+
+
+class ElmVsc(PFGeneral):
+  Cdc: float
+  "Cell capacitor"
+  Cfilt: float
+  "2nd-Harmonic Filter: Capacitance, Cfilt"
+  Cvalve: float
+  "Transistor/diode parameter: Snubber capacitance"
+  GPSlat: float
+  "Geographical Position: Latitude / Northing"
+  GPSlon: float
+  "Geographical Position: Longitude / Easting"
+  Gdoff: float
+  "Antiparallel diodes: Off-conductance"
+  Goff: float
+  "Transistor/diode parameter: Off-conductance"
+  Gvalve: float
+  "Transistor/diode parameter: Snubber conductance"
+  IkPFmax: float
+  "Steady-state short-circuit current contribution: Maximum current"
+  IkPFmin: float
+  "Steady-state short-circuit current contribution: Minimum current"
+  Iks: float
+  "Fault contribution: Transient short-circuit current"
+  Ikss: float
+  "Max. fault contribution: Subtransient short-circuit current"
+  Ikss1PF: float
+  "Initial symmetrical short-circuit current contribution: Single-phase faults, Ik1PF"
+  Ikss2PF: float
+  "Initial symmetrical short-circuit current contribution: Two-phase faults, Ik2PF"
+  Ikss3PF: float
+  "Initial symmetrical short-circuit current contribution: Three-phase faults, Ik3PF"
+  Inom: float
+  "Nominal Current (AC)"
+  Inomdc: float
+  "Nominal Current (DC)"
+  Irated: float
+  "Harmonic source: Rated Current"
+  K: float
+  "DC-voltage dependent P-droop: K"
+  Kd: float
+  "Use integrated current controller: Kd: d-axis, proportional gain"
+  Kfactor: float
+  "Fault contribution: K factor"
+  Kpart: float
+  "Active power participation: Participation factor"
+  Kpf: float
+  "Prim. frequency bias"
+  Kpphi: float
+  "Angle difference dependent P-droop: Kpphi"
+  Kq: float
+  "Use integrated current controller: Kq: q-axis, proportional gain"
+  Lac: float
+  "Voltage source parameters: AC inductance"
+  Larm: float
+  "Arm reactor: Inductance, Larm"
+  Ldc: float
+  "Voltage source parameters: DC inductance"
+  Lfilt: float
+  "2nd-Harmonic Filter: Inductance, Lfilt"
+  NmmcSM: int
+  "Number of submodules per arm"
+  P_max: float
+  "Max."
+  Pcu: float
+  "Series reactor: Copper losses"
+  Pmax_uc: float
+  "Active power operational limits: Max."
+  Pmin_uc: float
+  "Active power operational limits: Min."
+  Pmmax: float
+  "Consider modulation index limit: Max. PWM factor"
+  Pnold: float
+  "Losses: No-load losses"
+  Pnom: float
+  "Active power operational limits: Pr(rated)"
+  Qmax_a: float
+  "Qmax(act.)"
+  Qmin_a: float
+  "Qmin(act.)"
+  R0hmc: float
+  "Norton equivalent: Resistance, R0h"
+  R0toR1: float
+  "Series reactor: R0/R1 ratio"
+  R0toR1ac: float
+  "Voltage source parameters: R0/R1 ratio"
+  R1hmc: float
+  "Norton equivalent: Resistance, R1h"
+  R2hmc: float
+  "Norton equivalent: Resistance, R2h"
+  Rac: float
+  "Voltage source parameters: AC resistance"
+  Rarm: float
+  "Arm reactor: Resistance, Rarm"
+  Rdc: float
+  "Voltage source parameters: DC resistance"
+  Rdon: float
+  "Antiparallel diodes: On-resistance"
+  Ron: float
+  "Transistor/diode parameter: On-resistance"
+  Sks: float
+  "Fault contribution: Transient short-circuit level"
+  Skss: float
+  "Max. fault contribution: Subtransient short-circuit level"
+  Snom: float
+  "Ratings: Rated power"
+  Td: float
+  "Use integrated current controller: Td: d-axis, integration time constant"
+  Tdeadtime: float
+  "Dead time"
+  Tq: float
+  "Use integrated current controller: Tq: q-axis, integration time constant"
+  Tsampling: float
+  "Sampling period"
+  Unom: float
+  "Ratings: Rated AC-voltage"
+  Unomdc: float
+  "Ratings: Rated DC-voltage (DC)"
+  X0hmc: float
+  "Norton equivalent: Reactance, X0h"
+  X0toX1: float
+  "Series reactor: X0/X1 ratio"
+  X0toX1ac: float
+  "Voltage source parameters: X0/X1 ratio"
+  X1hmc: float
+  "Norton equivalent: Reactance, X1h"
+  X2hmc: float
+  "Norton equivalent: Reactance, X2h"
+  Xd: float
+  "Commutation reactance"
+  aCategory: str
+  "Category"
+  aSubCategory: str
+  "Subcategory"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  busac: object
+  "Terminal AC"
+  busdm: object
+  "Terminal DC-"
+  busdp: object
+  "Terminal DC+"
+  cCategory: str
+  "Category"
+  cDisplayName: str
+  "Display Name"
+  cLarm1: float
+  "2nd-Harmonic Filter: Inductance, Larm1"
+  cQ_max: float
+  "Reactive power limits: Max."
+  cQ_min: float
+  "Reactive power limits: Min."
+  cSubCategory: str
+  "Subcategory"
+  cTypHmc: str
+  "Harmonic source: Type of Harmonic Sources"
+  cUserDefIndex: int
+  "User defined Index"
+  c_pmod: object
+  "Model"
+  c_psecc: object
+  "Ext. secondary controller"
+  c_pstac: object
+  "External station controller"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  cictrltp: int
+  "const.V:const.I:const.V (deprecated)"
+  cimRdfId: list
+  "RDF ID"
+  commissionDate: str
+  "Commissioning Date"
+  considerPset: int
+  "Angle difference dependent P-droop: Consider active power setpoint"
+  constr: int
+  "Year of Construction"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  ddroop: float
+  "AC Voltage Droop: Droop"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  fcharr0: object
+  "Norton equivalent: Frequency-dependence, r0h(f)"
+  fcharr1: object
+  "Norton equivalent: Frequency-dependence, r1h(f)"
+  fcharr2: object
+  "Norton equivalent: Frequency-dependence, r2h(f)"
+  fcharx0: object
+  "Norton equivalent: Frequency-dependence, x0h(f)"
+  fcharx1: object
+  "Norton equivalent: Frequency-dependence, x1h(f)"
+  fcharx2: object
+  "Norton equivalent: Frequency-dependence, x2h(f)"
+  fmod: float
+  "Modulation frequency"
+  fmodMmc: float
+  "Modulation: Modulation frequency"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  iAreaBus: int
+  "Area"
+  iArmFilt: int
+  "2nd-Harmonic Filter"
+  iAstabint: int
+  "A-stable integration algorithm"
+  iComDate: int
+  "Commissioning Date"
+  iNoShcContr: int
+  "No short-circuit contribution"
+  iPpart: int
+  "Active power participation"
+  iPphidrp: int
+  "Angle difference dependent P-droop"
+  iQorient: int
+  "Orientation:+P/Q flow:-P/Q flow"
+  iSchemeStatus: int
+  "Scheme Status"
+  iShcModel: int
+  "Short-circuit model:Equivalent synchronous machine:Dynamic voltage support:const.V:const.I:Full size converter"
+  iThiPWM: int
+  "Third harmonic injection"
+  iVIsource: int
+  "Independent AC and DC voltage/current source model"
+  iVacMax: int
+  "Consider modulation index limit"
+  iWindGen: int
+  "Wind generator model"
+  iZarmDCside: int
+  "Consider arm reactor on DC side"
+  iZoneBus: int
+  "Zone"
+  i_acdc: int
+  "Control mode:Vac-phi:Vdc-phi:PWM-phi:Vdc-Q:P-Vac:P-Q:Vdc-Vac:P-cos(phi):Vdc-cos(phi)"
+  i_ctrl: int
+  "Use integrated current controller"
+  i_det: int
+  "Model"
+  i_mod: int
+  "Modulation"
+  iconfed: int
+  "Static converter-fed drive"
+  ictrltp: int
+  "Model"
+  icurref: int
+  "Harmonic source: Harmonic currents referred to"
+  idroop: int
+  "DC-voltage dependent P-droop"
+  imax: float
+  "Fault contribution: Max. current"
+  isCtrlFixedToLdfVal: int
+  "Fix controls to Load Flow values"
+  isCtrlP: int
+  "Controls: Active Power"
+  isCtrlQ: int
+  "Controls: Reactive Power"
+  isLimPmax: int
+  "Active power operational limits: Max."
+  isLimPmaxOPF: int
+  "Active power operational limits: Max."
+  isLimPmin: int
+  "Active power operational limits: Min."
+  isLimPminOPF: int
+  "Active power operational limits: Min."
+  isLimQmax: int
+  "Reactive power limits: Max."
+  isLimQmaxOPF: int
+  "Reactive power limits: Max."
+  isLimQmin: int
+  "Reactive power limits: Min."
+  isLimQminOPF: int
+  "Reactive power limits: Min."
+  isOpfCtrlP: int
+  "Controls: Active Power"
+  isOpfCtrlQ: int
+  "Controls: Reactive Power"
+  ivacdroop: int
+  "AC-Voltage Droop:none:Q-Droop:Iq-Droop"
+  loc_name: str
+  "Name"
+  manuf: str
+  "Manufacturer"
+  mmcCmod: float
+  "Submodule capacitance"
+  mmcGcap: float
+  "Capacitor parallel conductance"
+  mmcModType: int
+  "Modulation"
+  mmcModel: int
+  "MMC model:Controlled voltage source:Average value:Aggregate arm:Detailed equivalent circuit"
+  nparnum: int
+  "Number of: parallel converters"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pFlicker: object
+  "Flicker coefficients"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  pQlimType: object
+  "Reactive power limits: Capability curve"
+  pSubModel: object
+  "Submodel"
+  p_b1phiu: object
+  "Angle difference dependent P-droop: Remote AC busbar"
+  p_b2phiu: object
+  "Angle difference dependent P-droop: Local AC busbar"
+  p_pctrl: object
+  "Controlled flow"
+  p_pmeas: object
+  "Active power participation: P(AC) measured at"
+  p_uctrl: object
+  "Controlled node (AC)"
+  p_uctrldc: object
+  "Controlled node (DC)"
+  pblocktrf: object
+  "Externally modelled unit transformer: Unit transformer"
+  penaltyCosts: float
+  "Penalty costs for redispatch"
+  pf_recap: int
+  "Power factor:ind.:cap."
+  pfsetp: float
+  "Power factor"
+  phisetp: float
+  "Phase setpoint"
+  phmc: object
+  "Harmonic source: Harmonic injections"
+  phmcv: object
+  "Harmonic source: Harmonic voltages"
+  pid_: int
+  "ProjectID"
+  pmd_max: float
+  "Upper limit of Pmd"
+  pmd_min: float
+  "Lower limit of Pmd"
+  pmq_max: float
+  "Upper limit of Pmq"
+  pmq_min: float
+  "Lower limit of Pmq"
+  pmsetp: float
+  "PWM factor"
+  priority: int
+  "Merit Order"
+  psetp: float
+  "Active power setpoint"
+  psutype: str
+  "Power station unit type"
+  q_max: float
+  "Reactive power limits: Max."
+  q_min: float
+  "Reactive power limits: Min."
+  qsetp: float
+  "Reactive power setpoint"
+  r0: float
+  "Additional zero sequence impedance: Resistance, r0"
+  r0hmc: float
+  "Norton equivalent: Resistance, r0h"
+  r0iec: float
+  "Zero sequence short-circuit impedance: Resistance, r0"
+  r1hmc: float
+  "Norton equivalent: Resistance, r1h"
+  r2: float
+  "Additional negative sequence impedance: Resistance, r2"
+  r2hmc: float
+  "Norton equivalent: Resistance, r2h"
+  r2iec: float
+  "Negative sequence short-circuit impedance: Resistance, r2"
+  r2shc: float
+  "Negative sequence short-circuit impedance: Resistance, r2"
+  resLossFactor: float
+  "Losses: Resistive loss factor"
+  root_id: object
+  "Original Location"
+  rtox: float
+  "Max. fault contribution: R to X'' ratio"
+  sampling: int
+  "Switch events:Precise crossing time:Fixed sampling period"
+  scaleQmax: float
+  "Reactive power limits: Scaling factor (max.)"
+  scaleQmin: float
+  "Reactive power limits: Scaling factor (min.)"
+  searchBlockTrf: int
+  "Externally modelled unit transformer"
+  sernum: str
+  "Serial Number"
+  shcDeadband: int
+  "Voltage deadband"
+  swtLossFactor: float
+  "Losses: Switching loss factor"
+  tid_: int
+  "TimeID"
+  uDeadband: float
+  "Voltage deadband: Deadband"
+  uk: float
+  "Series reactor: Short circuit impedance"
+  usetp: float
+  "AC voltage setpoint"
+  usetpdc: float
+  "DC voltage setpoint"
+  usp_max: float
+  "AC Voltage Droop Voltage setpoint limits: Max. voltage setpoint"
+  usp_min: float
+  "AC Voltage Droop Voltage setpoint limits: Min. voltage setpoint"
+  vsctype: int
+  "Converter type:Two-level converter:Half-bridge type MMC:Full-bridge type MMC"
+  x0: float
+  "Additional zero sequence impedance: Reactance, x0"
+  x0hmc: float
+  "Norton equivalent: Reactance, x0h"
+  x0iec: float
+  "Zero sequence short-circuit impedance: Reactance, x0"
+  x1hmc: float
+  "Norton equivalent: Reactance, x1h"
+  x2: float
+  "Additional negative sequence impedance: Reactance, x2"
+  x2hmc: float
+  "Norton equivalent: Reactance, x2h"
+  x2iec: float
+  "Negative sequence short-circuit impedance: Reactance, x2"
+  x2shc: float
+  "Negative sequence short-circuit impedance: Reactance, x2"
+  xtor: float
+  "Max. fault contribution: X'' to R ratio"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
+
+
+
+class ElmVscmono(PFGeneral):
+  Cdc: float
+  "Cell capacitor"
+  Cfilt: float
+  "2nd-Harmonic Filter: Capacitance, Cfilt"
+  Cvalve: float
+  "Transistor/diode parameter: Snubber capacitance"
+  GPSlat: float
+  "Geographical Position: Latitude / Northing"
+  GPSlon: float
+  "Geographical Position: Longitude / Easting"
+  Gdoff: float
+  "Antiparallel diodes: Off-conductance"
+  Goff: float
+  "Transistor/diode parameter: Off-conductance"
+  Gvalve: float
+  "Transistor/diode parameter: Snubber conductance"
+  IkPFmax: float
+  "Steady-state short-circuit current contribution: Maximum current"
+  IkPFmin: float
+  "Steady-state short-circuit current contribution: Minimum current"
+  Iks: float
+  "Fault contribution: Transient short-circuit current"
+  Ikss: float
+  "Max. fault contribution: Subtransient short-circuit current"
+  Ikss1PF: float
+  "Initial symmetrical short-circuit current contribution: Single-phase faults, Ik1PF"
+  Ikss2PF: float
+  "Initial symmetrical short-circuit current contribution: Two-phase faults, Ik2PF"
+  Ikss3PF: float
+  "Initial symmetrical short-circuit current contribution: Three-phase faults, Ik3PF"
+  Inom: float
+  "Nominal Current (AC)"
+  Inomdc: float
+  "Nominal Current (DC)"
+  Irated: float
+  "Harmonic source: Rated Current"
+  K: float
+  "DC-voltage dependent P-droop: K"
+  Kd: float
+  "Use integrated current controller: Kd: d-axis, proportional gain"
+  Kfactor: float
+  "Fault contribution: K factor"
+  Kpart: float
+  "Active power participation: Participation factor"
+  Kpf: float
+  "Prim. frequency bias"
+  Kpphi: float
+  "Angle difference dependent P-droop: Kpphi"
+  Kq: float
+  "Use integrated current controller: Kq: q-axis, proportional gain"
+  Lac: float
+  "Voltage source parameters: AC inductance"
+  Larm: float
+  "Arm reactor: Inductance, Larm"
+  Ldc: float
+  "Voltage source parameters: DC inductance"
+  Lfilt: float
+  "2nd-Harmonic Filter: Inductance, Lfilt"
+  NmmcSM: int
+  "Number of submodules per arm"
+  P_max: float
+  "Max."
+  Pcu: float
+  "Series reactor: Copper losses"
+  Pmax_uc: float
+  "Active power operational limits: Max."
+  Pmin_uc: float
+  "Active power operational limits: Min."
+  Pmmax: float
+  "Consider modulation index limit: Max. PWM factor"
+  Pnold: float
+  "Losses: No-load losses"
+  Pnom: float
+  "Active power operational limits: Pr(rated)"
+  Qmax_a: float
+  "Qmax(act.)"
+  Qmin_a: float
+  "Qmin(act.)"
+  R0hmc: float
+  "Norton equivalent: Resistance, R0h"
+  R0toR1: float
+  "Series reactor: R0/R1 ratio"
+  R0toR1ac: float
+  "Voltage source parameters: R0/R1 ratio"
+  R1hmc: float
+  "Norton equivalent: Resistance, R1h"
+  R2hmc: float
+  "Norton equivalent: Resistance, R2h"
+  Rac: float
+  "Voltage source parameters: AC resistance"
+  Rarm: float
+  "Arm reactor: Resistance, Rarm"
+  Rdc: float
+  "Voltage source parameters: DC resistance"
+  Rdon: float
+  "Antiparallel diodes: On-resistance"
+  Ron: float
+  "Transistor/diode parameter: On-resistance"
+  Sks: float
+  "Fault contribution: Transient short-circuit level"
+  Skss: float
+  "Max. fault contribution: Subtransient short-circuit level"
+  Snom: float
+  "Ratings: Rated power"
+  Td: float
+  "Use integrated current controller: Td: d-axis, integration time constant"
+  Tdeadtime: float
+  "Dead time"
+  Tq: float
+  "Use integrated current controller: Tq: q-axis, integration time constant"
+  Tsampling: float
+  "Sampling period"
+  Unom: float
+  "Ratings: Rated AC-voltage"
+  Unomdc: float
+  "Ratings: Rated DC-voltage (DC)"
+  X0hmc: float
+  "Norton equivalent: Reactance, X0h"
+  X0toX1: float
+  "Series reactor: X0/X1 ratio"
+  X0toX1ac: float
+  "Voltage source parameters: X0/X1 ratio"
+  X1hmc: float
+  "Norton equivalent: Reactance, X1h"
+  X2hmc: float
+  "Norton equivalent: Reactance, X2h"
+  Xd: float
+  "Commutation reactance"
+  aCategory: str
+  "Category"
+  aSubCategory: str
+  "Subcategory"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  busac: object
+  "Terminal AC"
+  busdc: object
+  "Terminal DC"
+  cCategory: str
+  "Category"
+  cDisplayName: str
+  "Display Name"
+  cLarm1: float
+  "2nd-Harmonic Filter: Inductance, Larm1"
+  cQ_max: float
+  "Reactive power limits: Max."
+  cQ_min: float
+  "Reactive power limits: Min."
+  cSubCategory: str
+  "Subcategory"
+  cTypHmc: str
+  "Harmonic source: Type of Harmonic Sources"
+  cUserDefIndex: int
+  "User defined Index"
+  c_pmod: object
+  "Model"
+  c_psecc: object
+  "Ext. secondary controller"
+  c_pstac: object
+  "External station controller"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  cictrltp: int
+  "const.V:const.I:const.V (deprecated)"
+  cimRdfId: list
+  "RDF ID"
+  commissionDate: str
+  "Commissioning Date"
+  considerPset: int
+  "Angle difference dependent P-droop: Consider active power setpoint"
+  constr: int
+  "Year of Construction"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  ddroop: float
+  "AC Voltage Droop: Droop"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  fcharr0: object
+  "Norton equivalent: Frequency-dependence, r0h(f)"
+  fcharr1: object
+  "Norton equivalent: Frequency-dependence, r1h(f)"
+  fcharr2: object
+  "Norton equivalent: Frequency-dependence, r2h(f)"
+  fcharx0: object
+  "Norton equivalent: Frequency-dependence, x0h(f)"
+  fcharx1: object
+  "Norton equivalent: Frequency-dependence, x1h(f)"
+  fcharx2: object
+  "Norton equivalent: Frequency-dependence, x2h(f)"
+  fmod: float
+  "Modulation frequency"
+  fmodMmc: float
+  "Modulation: Modulation frequency"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  iAreaBus: int
+  "Area"
+  iArmFilt: int
+  "2nd-Harmonic Filter"
+  iAstabint: int
+  "A-stable integration algorithm"
+  iComDate: int
+  "Commissioning Date"
+  iNoShcContr: int
+  "No short-circuit contribution"
+  iPpart: int
+  "Active power participation"
+  iPphidrp: int
+  "Angle difference dependent P-droop"
+  iQorient: int
+  "Orientation:+P/Q flow:-P/Q flow"
+  iSchemeStatus: int
+  "Scheme Status"
+  iShcModel: int
+  "Short-circuit model:Equivalent synchronous machine:Dynamic voltage support:const.V:const.I:Full size converter"
+  iThiPWM: int
+  "Third harmonic injection"
+  iVIsource: int
+  "Independent AC and DC voltage/current source model"
+  iVacMax: int
+  "Consider modulation index limit"
+  iWindGen: int
+  "Wind generator model"
+  iZarmDCside: int
+  "Consider arm reactor on DC side"
+  iZoneBus: int
+  "Zone"
+  i_acdc: int
+  "Control mode:Vac-phi:Vdc-phi:PWM-phi:Vdc-Q:P-Vac:P-Q:Vdc-Vac:P-cos(phi):Vdc-cos(phi)"
+  i_ctrl: int
+  "Use integrated current controller"
+  i_det: int
+  "Model"
+  i_mod: int
+  "Modulation"
+  iconfed: int
+  "Static converter-fed drive"
+  ictrltp: int
+  "Model"
+  icurref: int
+  "Harmonic source: Harmonic currents referred to"
+  idroop: int
+  "DC-voltage dependent P-droop"
+  imax: float
+  "Fault contribution: Max. current"
+  isCtrlFixedToLdfVal: int
+  "Fix controls to Load Flow values"
+  isCtrlP: int
+  "Controls: Active Power"
+  isCtrlQ: int
+  "Controls: Reactive Power"
+  isLimPmax: int
+  "Active power operational limits: Max."
+  isLimPmaxOPF: int
+  "Active power operational limits: Max."
+  isLimPmin: int
+  "Active power operational limits: Min."
+  isLimPminOPF: int
+  "Active power operational limits: Min."
+  isLimQmax: int
+  "Reactive power limits: Max."
+  isLimQmaxOPF: int
+  "Reactive power limits: Max."
+  isLimQmin: int
+  "Reactive power limits: Min."
+  isLimQminOPF: int
+  "Reactive power limits: Min."
+  isOpfCtrlP: int
+  "Controls: Active Power"
+  isOpfCtrlQ: int
+  "Controls: Reactive Power"
+  ivacdroop: int
+  "AC-Voltage Droop:none:Q-Droop:Iq-Droop"
+  loc_name: str
+  "Name"
+  manuf: str
+  "Manufacturer"
+  mmcCmod: float
+  "Submodule capacitance"
+  mmcGcap: float
+  "Capacitor parallel conductance"
+  mmcModType: int
+  "Modulation"
+  mmcModel: int
+  "MMC model:Controlled voltage source:Average value:Aggregate arm:Detailed equivalent circuit"
+  nparnum: int
+  "Number of: parallel converters"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pFlicker: object
+  "Flicker coefficients"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  pQlimType: object
+  "Reactive power limits: Capability curve"
+  pSubModel: object
+  "Submodel"
+  p_b1phiu: object
+  "Angle difference dependent P-droop: Remote AC busbar"
+  p_b2phiu: object
+  "Angle difference dependent P-droop: Local AC busbar"
+  p_pctrl: object
+  "Controlled flow"
+  p_pmeas: object
+  "Active power participation: P(AC) measured at"
+  p_uctrl: object
+  "Controlled node (AC)"
+  p_uctrldc: object
+  "Controlled node (DC)"
+  pblocktrf: object
+  "Externally modelled unit transformer: Unit transformer"
+  penaltyCosts: float
+  "Penalty costs for redispatch"
+  pf_recap: int
+  "Power factor:ind.:cap."
+  pfsetp: float
+  "Power factor"
+  phisetp: float
+  "Phase setpoint"
+  phmc: object
+  "Harmonic source: Harmonic injections"
+  phmcv: object
+  "Harmonic source: Harmonic voltages"
+  pid_: int
+  "ProjectID"
+  pmd_max: float
+  "Upper limit of Pmd"
+  pmd_min: float
+  "Lower limit of Pmd"
+  pmq_max: float
+  "Upper limit of Pmq"
+  pmq_min: float
+  "Lower limit of Pmq"
+  pmsetp: float
+  "PWM factor"
+  priority: int
+  "Merit Order"
+  psetp: float
+  "Active power setpoint"
+  psutype: str
+  "Power station unit type"
+  q_max: float
+  "Reactive power limits: Max."
+  q_min: float
+  "Reactive power limits: Min."
+  qsetp: float
+  "Reactive power setpoint"
+  r0: float
+  "Additional zero sequence impedance: Resistance, r0"
+  r0hmc: float
+  "Norton equivalent: Resistance, r0h"
+  r0iec: float
+  "Zero sequence short-circuit impedance: Resistance, r0"
+  r1hmc: float
+  "Norton equivalent: Resistance, r1h"
+  r2: float
+  "Additional negative sequence impedance: Resistance, r2"
+  r2hmc: float
+  "Norton equivalent: Resistance, r2h"
+  r2iec: float
+  "Negative sequence short-circuit impedance: Resistance, r2"
+  r2shc: float
+  "Negative sequence short-circuit impedance: Resistance, r2"
+  resLossFactor: float
+  "Losses: Resistive loss factor"
+  root_id: object
+  "Original Location"
+  rtox: float
+  "Max. fault contribution: R to X'' ratio"
+  sampling: int
+  "Switch events:Precise crossing time:Fixed sampling period"
+  scaleQmax: float
+  "Reactive power limits: Scaling factor (max.)"
+  scaleQmin: float
+  "Reactive power limits: Scaling factor (min.)"
+  searchBlockTrf: int
+  "Externally modelled unit transformer"
+  sernum: str
+  "Serial Number"
+  shcDeadband: int
+  "Voltage deadband"
+  swtLossFactor: float
+  "Losses: Switching loss factor"
+  tid_: int
+  "TimeID"
+  uDeadband: float
+  "Voltage deadband: Deadband"
+  uk: float
+  "Series reactor: Short circuit impedance"
+  usetp: float
+  "AC voltage setpoint"
+  usetpdc: float
+  "DC voltage setpoint"
+  usp_max: float
+  "AC Voltage Droop Voltage setpoint limits: Max. voltage setpoint"
+  usp_min: float
+  "AC Voltage Droop Voltage setpoint limits: Min. voltage setpoint"
+  vsctype: int
+  "Converter type:Two-level converter:Half-bridge type MMC:Full-bridge type MMC"
+  x0: float
+  "Additional zero sequence impedance: Reactance, x0"
+  x0hmc: float
+  "Norton equivalent: Reactance, x0h"
+  x0iec: float
+  "Zero sequence short-circuit impedance: Reactance, x0"
+  x1hmc: float
+  "Norton equivalent: Reactance, x1h"
+  x2: float
+  "Additional negative sequence impedance: Reactance, x2"
+  x2hmc: float
+  "Norton equivalent: Reactance, x2h"
+  x2iec: float
+  "Negative sequence short-circuit impedance: Reactance, x2"
+  x2shc: float
+  "Negative sequence short-circuit impedance: Reactance, x2"
+  xtor: float
+  "Max. fault contribution: X'' to R ratio"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
+
+
+
+class ElmZpu(PFGeneral):
+  GPSlat: float
+  "Geographical Position: Latitude / Northing"
+  GPSlon: float
+  "Geographical Position: Longitude / Easting"
+  Sn: float
+  "Rated Power"
+  ag: float
+  "Transformer Equivalent: Additional Phase Shift"
+  appr_modby: str
+  "Approval Information: Modified by"
+  appr_modif: int
+  "Approval Information: Modified"
+  appr_status: int
+  "Approval Information: Status"
+  bi0_pu: float
+  "Zero-Sequence conductance and susceptance: Susceptance i"
+  bi0s_pu: float
+  "Zero-Sequence conductance and susceptance: Susceptance i"
+  bi2_pu: float
+  "Negative-Sequence conductance and susceptance: Susceptance i"
+  bi2s_pu: float
+  "Negative-Sequence conductance and susceptance: Susceptance i"
+  bi_pu: float
+  "Positive-Sequence conductance and susceptance: Susceptance i"
+  bis_pu: float
+  "Positive-Sequence conductance and susceptance: Susceptance i"
+  bj0_pu: float
+  "Zero-Sequence conductance and susceptance: Susceptance j"
+  bj0s_pu: float
+  "Zero-Sequence conductance and susceptance: Susceptance j"
+  bj2_pu: float
+  "Negative-Sequence conductance and susceptance: Susceptance j"
+  bj2s_pu: float
+  "Negative-Sequence conductance and susceptance: Susceptance j"
+  bj_pu: float
+  "Positive-Sequence conductance and susceptance: Susceptance j"
+  bjs_pu: float
+  "Positive-Sequence conductance and susceptance: Susceptance j"
+  bus1: object
+  "Terminal i"
+  bus2: object
+  "Terminal j"
+  cDisplayName: str
+  "Display Name"
+  cUserDefIndex: int
+  "User defined Index"
+  charact: list
+  "Charact."
+  chr_name: str
+  "Characteristic Name"
+  ciDist: int
+  "Distance from infeed in number of buses"
+  ciDistAll: int
+  "Distance from infeed in number of buses including switches"
+  ciDistAllRoot: int
+  "Distance from first infeed in number of buses including switches"
+  ciDistRoot: int
+  "Distance from first infeed in number of buses"
+  ciEarthed: int
+  "Earthed"
+  ciEnergized: int
+  "Energized"
+  ciLater: int
+  "Lateral Index"
+  ciOutaged: int
+  "Planned Outage"
+  cimRdfId: list
+  "RDF ID"
+  commissionDate: str
+  "Commissioning Date"
+  constr: int
+  "Year of Construction"
+  cpArea: object
+  "Area"
+  cpBranch: object
+  "Branch"
+  cpFeed: object
+  "Feeder"
+  cpGrid: object
+  "Grid"
+  cpHeadFold: object
+  "Head Folder"
+  cpMeteostat: object
+  "Meteo Station"
+  cpOperator: object
+  "Operator"
+  cpOwner: object
+  "Owner"
+  cpSite: object
+  "Site"
+  cpSubstat: object
+  "Substation"
+  cpSupplySubstation: object
+  "Supplying Substation"
+  cpSupplyTransformer: object
+  "Supplying Transformer"
+  cpSupplyTrfStation: object
+  "Supplying Secondary Substation"
+  cpZone: object
+  "Zone"
+  dat_src: str
+  "Data source"
+  dataExtDesc: list
+  "Description"
+  dataExtUnit: list
+  "Unit"
+  desc: list
+  "Description"
+  doc_id: object
+  "Additional Data"
+  dpl1: float
+  "dpl1"
+  dpl2: float
+  "dpl2"
+  dpl3: float
+  "dpl3"
+  dpl4: float
+  "dpl4"
+  dpl5: float
+  "dpl5"
+  fold_id: object
+  "In Folder"
+  for_name: str
+  "Foreign Key"
+  gi0_pu: float
+  "Zero-Sequence conductance and susceptance: Conductance i"
+  gi0s_pu: float
+  "Zero-Sequence conductance and susceptance: Conductance i"
+  gi2_pu: float
+  "Negative-Sequence conductance and susceptance: Conductance i"
+  gi2s_pu: float
+  "Negative-Sequence conductance and susceptance: Conductance i"
+  gi_pu: float
+  "Positive-Sequence conductance and susceptance: Conductance i"
+  gis_pu: float
+  "Positive-Sequence conductance and susceptance: Conductance i"
+  gj0_pu: float
+  "Zero-Sequence conductance and susceptance: Conductance j"
+  gj0s_pu: float
+  "Zero-Sequence conductance and susceptance: Conductance j"
+  gj2_pu: float
+  "Negative-Sequence conductance and susceptance: Conductance j"
+  gj2s_pu: float
+  "Negative-Sequence conductance and susceptance: Conductance j"
+  gj_pu: float
+  "Positive-Sequence conductance and susceptance: Conductance j"
+  gjs_pu: float
+  "Positive-Sequence conductance and susceptance: Conductance j"
+  gnrl_modby: str
+  "Object modified by"
+  gnrl_modif: int
+  "Object modified"
+  iAreaBus: int
+  "Area"
+  iCapParallel: int
+  "Consider resistive and capacitive parts in parallel"
+  iComDate: int
+  "Commissioning Date"
+  iFreZ: int
+  "Use Frequency Related Impedance for X/R Ratio Calculation"
+  iSchemeStatus: int
+  "Scheme Status"
+  iZoneBus: int
+  "Zone"
+  iZshc: int
+  "Use same impedance as for load flow"
+  iequalz: int
+  "Use equal Impedances (zij = zji)"
+  iy2eqy1: int
+  "Use Admittance y2 = y1"
+  iy2eqy1s: int
+  "Use Admittance y2 = y1"
+  iz2eqz1: int
+  "Use Impedance z2 = z1"
+  iztreqz: int
+  "Transient = Subtransient Impedance"
+  loc_name: str
+  "Name"
+  manuf: str
+  "Manufacturer"
+  matZ: list
+  "Frequency related impedances i->j (Positive, Negative and Zero sequence)"
+  matZ1: list
+  "Frequency related impedances j->i (Positive, Negative and Zero sequence)"
+  nphases: int
+  "Phases:1:3"
+  nphshift: int
+  "Transformer Equivalent: Nominal Phase Shift"
+  oid_: int
+  "ObjectID"
+  outserv: int
+  "Out of Service"
+  pOperator: object
+  "Operator"
+  pOwner: object
+  "Owner"
+  pid_: int
+  "ProjectID"
+  r0_pu: float
+  "Zero-Sequence Impedance i-j: Real Part"
+  r0_pu_ji: float
+  "Zero-Sequence Impedance j-i: Real Part"
+  r0s_pu: float
+  "Zero-Sequence Impedance i-j: Real Part"
+  r0s_pu_ji: float
+  "Zero-Sequence Impedance j-i: Real Part"
+  r2_pu: float
+  "Negative-Sequence Impedance i-j: Real Part"
+  r2_pu_ji: float
+  "Negative-Sequence Impedance j-i: Real Part"
+  r2s_pu: float
+  "Negative-Sequence Impedance i-j: Real Part"
+  r2s_pu_ji: float
+  "Negative-Sequence Impedance j-i: Real Part"
+  r_pu: float
+  "Positive-Sequence Impedance i-j: Real Part"
+  r_pu_ji: float
+  "Positive-Sequence Impedance j-i: Real Part"
+  root_id: object
+  "Original Location"
+  rs_pu: float
+  "Subtransient Positive-Sequence Impedance i-j: Real Part"
+  rs_pu_ji: float
+  "Subtransient Positive-Sequence Impedance j-i: Real Part"
+  rstr_pu: float
+  "Transient Positive-Sequence Impedance i-j: Real Part"
+  rstr_pu_ji: float
+  "Transient Positive-Sequence Impedance j-i: Real Part"
+  sernum: str
+  "Serial Number"
+  tid_: int
+  "TimeID"
+  uratio: float
+  "Transformer Equivalent: Tap Ratio"
+  x0_pu: float
+  "Zero-Sequence Impedance i-j: Imaginary Part"
+  x0_pu_ji: float
+  "Zero-Sequence Impedance j-i: Imaginary Part"
+  x0s_pu: float
+  "Zero-Sequence Impedance i-j: Imaginary Part"
+  x0s_pu_ji: float
+  "Zero-Sequence Impedance j-i: Imaginary Part"
+  x2_pu: float
+  "Negative-Sequence Impedance i-j: Imaginary Part"
+  x2_pu_ji: float
+  "Negative-Sequence Impedance j-i: Imaginary Part"
+  x2s_pu: float
+  "Negative-Sequence Impedance i-j: Imaginary Part"
+  x2s_pu_ji: float
+  "Negative-Sequence Impedance j-i: Imaginary Part"
+  x_pu: float
+  "Positive-Sequence Impedance i-j: Imaginary Part"
+  x_pu_ji: float
+  "Positive-Sequence Impedance j-i: Imaginary Part"
+  xs_pu: float
+  "Subtransient Positive-Sequence Impedance i-j: Imaginary Part"
+  xs_pu_ji: float
+  "Subtransient Positive-Sequence Impedance j-i: Imaginary Part"
+  xstr_pu: float
+  "Transient Positive-Sequence Impedance i-j: Imaginary Part"
+  xstr_pu_ji: float
+  "Transient Positive-Sequence Impedance j-i: Imaginary Part"
+
+
+  def AttributeType(*args):
+    ...
+
+  def HasReferences(*args):
+    ...
+
+  def __getattr__(*args):
+    ...
 
 
 
 class IntPrj(PFGeneral):
   CTLimit: int
   "COMTRADE Data File import limit: Maximum Number of Files"
   CTLimitNum: int
```

### Comparing `powfacpy-0.1.6/src/powfacpy/pf_classes_protocol_generator.py` & `powfacpy-0.2.0/src/powfacpy/pf_classes_protocol_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 IMPORTANT: If you miss a class please add it to the 'missing_classes_that_are_not_in_scripting_reference' list below.
 
 
 This module is not used by other modules of powfacpy and has the sole purpose of creating the protocols.
 """
 
-missing_classes_that_are_not_in_scripting_reference = ["IntFolder", "ElmSite", "ComVstab", "ComMod", "ElmSecctrl"]
+missing_classes_that_are_not_in_scripting_reference = ["IntFolder", "ElmSite", "ComVstab", "ComMod", "ElmSecctrl", "ElmLod", "ElmIac", "ElmLodlv", "ElmLodmv", "ElmSind", "ElmVsc", "ElmVscmono", "ElmZpu"]
 
 
 import os 
 import keyword
 import sys
 import json
```

### Comparing `powfacpy-0.1.6/src/powfacpy/pf_elm_objects.py` & `powfacpy-0.2.0/src/powfacpy/pf_elm_objects.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/plot_interface.py` & `powfacpy-0.2.0/src/powfacpy/plot_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/result_variables.py` & `powfacpy-0.2.0/src/powfacpy/result_variables.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/result_variables_parser.py` & `powfacpy-0.2.0/src/powfacpy/result_variables_parser.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/results_interface.py` & `powfacpy-0.2.0/src/powfacpy/results_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/script_interface.py` & `powfacpy-0.2.0/src/powfacpy/script_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/string_manipulation.py` & `powfacpy-0.2.0/src/powfacpy/string_manipulation.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/src/powfacpy/topology.py` & `powfacpy-0.2.0/src/powfacpy/topology.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_active_project_interface.py` & `powfacpy-0.2.0/tests/test_active_project_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,9 +374,10 @@
     assert len(terminals_getobj) == len(terminals_calc_rel)
     
     with pytest.raises(powfacpy.PFNonExistingObjectError):    
         pfp.get_calc_relevant_obj("*.ElmTerm", 
                                   condition=lambda x: x.uknom > 5000)
 
 if __name__ == "__main__":
-    pytest.main([r"tests\test_active_project_interface.py::test_get_calc_relevant_obj"])
-    #pytest.main(([r"tests"]))
+    #pytest.main([r"tests\test_active_project_interface.py::test_get_calc_relevant_obj"])
+
+    pytest.main(([r"tests"]))
```

### Comparing `powfacpy-0.1.6/tests/test_case_studies.py` & `powfacpy-0.2.0/tests/test_case_studies.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_database_interface.py` & `powfacpy-0.2.0/tests/test_database_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_dyn_sim_interface.py` & `powfacpy-0.2.0/tests/test_dyn_sim_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_functional_interface.py` & `powfacpy-0.2.0/tests/test_functional_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_model_exchange_interfaces.py` & `powfacpy-0.2.0/tests/test_model_exchange_interfaces.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_network_interface.py` & `powfacpy-0.2.0/tests/test_network_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_plot_interface.py` & `powfacpy-0.2.0/tests/test_plot_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_results_interface.py` & `powfacpy-0.2.0/tests/test_results_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/test_script_interface.py` & `powfacpy-0.2.0/tests/test_script_interface.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/tests_input/powfacpy_tests.pfd` & `powfacpy-0.2.0/tests/tests_input/powfacpy_tests.pfd`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/tests_input/test_comtrade.cfg` & `powfacpy-0.2.0/tests/tests_input/test_comtrade.cfg`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/tests_input/test_comtrade.dat` & `powfacpy-0.2.0/tests/tests_input/test_comtrade.dat`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/tests_output/powfacpy_single_file.py` & `powfacpy-0.2.0/tests/tests_output/powfacpy_single_file.py`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/tests_output/test1.json` & `powfacpy-0.2.0/tests/tests_output/test1.json`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/tests_output/test2.json` & `powfacpy-0.2.0/tests/tests_output/test2.json`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/tests_output/test_get_object_attributes.json` & `powfacpy-0.2.0/tests/tests_output/test_get_object_attributes.json`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tests/tests_output/test_get_object_attributes_modified.json` & `powfacpy-0.2.0/tests/tests_output/test_get_object_attributes_modified.json`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/getting_started.ipynb` & `powfacpy-0.2.0/tutorials/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/simulation_and_plotting.ipynb` & `powfacpy-0.2.0/tutorials/simulation_and_plotting.ipynb`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/study_cases.ipynb` & `powfacpy-0.2.0/tutorials/study_cases.ipynb`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/figures/cases_1.png` & `powfacpy-0.2.0/tutorials/figures/cases_1.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/figures/cases_2.png` & `powfacpy-0.2.0/tutorials/figures/cases_2.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/figures/legend_1.png` & `powfacpy-0.2.0/tutorials/figures/legend_1.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/figures/object_path.png` & `powfacpy-0.2.0/tutorials/figures/object_path.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/figures/rebuild_button.png` & `powfacpy-0.2.0/tutorials/figures/rebuild_button.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/figures/scenarios_1.png` & `powfacpy-0.2.0/tutorials/figures/scenarios_1.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/figures/type_hints.png` & `powfacpy-0.2.0/tutorials/figures/type_hints.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/tutorials/figures/variations_3.png` & `powfacpy-0.2.0/tutorials/figures/variations_3.png`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/LICENSE` & `powfacpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/README.md` & `powfacpy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `powfacpy-0.1.6/pyproject.toml` & `powfacpy-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "powfacpy"
-version = "0.1.6"
+version = "0.2.0"
 authors = [
   { name="Sciemon", email="simon.eberlein@gmx.de" },
 ]
 description = "PowerFactory wrapper"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `powfacpy-0.1.6/PKG-INFO` & `powfacpy-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: powfacpy
-Version: 0.1.6
+Version: 0.2.0
 Summary: PowerFactory wrapper
 Project-URL: Homepage, https://github.com/FraunhIEE-UniKassel-PowSysStability/powfacpy
 Project-URL: Bug Tracker, https://github.com/FraunhIEE-UniKassel-PowSysStability/powfacpy/issues
 Author-email: Sciemon <simon.eberlein@gmx.de>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

