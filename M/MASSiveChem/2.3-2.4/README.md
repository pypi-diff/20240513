# Comparing `tmp/massivechem-2.3.tar.gz` & `tmp/massivechem-2.4.tar.gz`

## Comparing `massivechem-2.3.tar` & `massivechem-2.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 massivechem-2.3/insaturation.py
--rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 massivechem-2.3/molecule_image.png
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 massivechem-2.3/preliminary.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 massivechem-2.3/project_CH200.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-2.3/scripts.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 massivechem-2.3/setup.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 massivechem-2.3/subgroups.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 massivechem-2.3/.github/workflows/requirements.txt
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-2.3/.idea/misc.xml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-2.3/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-2.3/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-2.3/.idea/vcs.xml
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 massivechem-2.3/.idea/workspace.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-2.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 massivechem-2.3/Bokeh/Double plot bokeh.html
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 massivechem-2.3/Bokeh/Double plot bokeh.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 massivechem-2.3/Bokeh/Functional_group_display.html
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 massivechem-2.3/Bokeh/Functional_group_display.py
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 massivechem-2.3/Bokeh/Mol_display.html
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 massivechem-2.3/Bokeh/Mol_display.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 massivechem-2.3/Bokeh/molecule_image.png
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/Mol_display.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/Preliminary_v2.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/abundance.txt
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/abundance_simplified.txt
--rw-r--r--   0        0        0    24987 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/big_func.py
--rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/copy_file.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/functional_group_finder.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/functions.html
--rw-r--r--   0        0        0    26739 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/functions.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/molecule_image.png
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/names.txt
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-2.3/THOMAS_IS_BEST/test.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-2.3/Thomas/Copy_spectrometer.py
--rw-r--r--   0        0        0    49000 2020-02-02 00:00:00.000000 massivechem-2.3/Thomas/Thomas_return.html
--rw-r--r--   0        0        0    27616 2020-02-02 00:00:00.000000 massivechem-2.3/Thomas/Thomas_return_pyplot.html
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-2.3/Thomas/Thomas_return_pyplot.py
--rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 massivechem-2.3/Thomas/functions.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-2.3/Thomas/random_tests.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 massivechem-2.3/Thomas/tests.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-2.3/data/abundance.txt
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Acid_image.png
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Acyl_chloride_image.png
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Alcohol_image.png
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Aldehyde_image.png
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Alkene_image.png
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Alkyne_image.png
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Amide_image.png
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Amine_image.png
--rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Amino_acid_image.png
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Anhydride_image.png
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Azide_image.png
--rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Benzene_image.png
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Carbonate2_image.png
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Carbonate_image.png
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Disulfide_image.png
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Enamine2_image.png
--rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Enamine_2_image.png
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Enamine_image.png
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Enol_image.png
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Ester_image.png
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Ether_image.png
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Halogen_image.png
--rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Hemiacetal_image.png
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Imide_image.png
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Imine_image.png
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Ketone_image.png
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Nitrile_image.png
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Nitro_image.png
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Peroxide_image.png
--rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Phosphate_image.png
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Phosphine_image.png
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Proline_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Sulfides_image.png
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Sulfone_image.png
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Sulfonic_acid_image.png
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Sulfoxide_image.png
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Thio_ether_image.png
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Thioester_image.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-2.3/data/Functional groups images/Thiol_image.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-2.3/notebooks/test.ipynb
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 massivechem-2.3/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-2.3/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 massivechem-2.3/LICENSE.txt
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 massivechem-2.3/README.md
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 massivechem-2.3/pyproject.toml
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 massivechem-2.3/PKG-INFO
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 massivechem-2.4/insaturation.py
+-rw-r--r--   0        0        0     4750 2020-02-02 00:00:00.000000 massivechem-2.4/molecule_image.png
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 massivechem-2.4/preliminary.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 massivechem-2.4/project_CH200.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-2.4/scripts.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 massivechem-2.4/setup.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 massivechem-2.4/subgroups.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 massivechem-2.4/.github/workflows/requirements.txt
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-2.4/.idea/misc.xml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-2.4/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-2.4/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-2.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 massivechem-2.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-2.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    15981 2020-02-02 00:00:00.000000 massivechem-2.4/Bokeh/Double plot bokeh.html
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 massivechem-2.4/Bokeh/Double plot bokeh.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 massivechem-2.4/Bokeh/Functional_group_display.html
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 massivechem-2.4/Bokeh/Functional_group_display.py
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 massivechem-2.4/Bokeh/Mol_display.html
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 massivechem-2.4/Bokeh/Mol_display.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 massivechem-2.4/Bokeh/molecule_image.png
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/Mol_display.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/Preliminary_v2.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/abundance.txt
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/abundance_simplified.txt
+-rw-r--r--   0        0        0    24987 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/big_func.py
+-rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/copy_file.py
+-rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/functional_group_finder.py
+-rw-r--r--   0        0        0    10565 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/functions.html
+-rw-r--r--   0        0        0    29350 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/functions.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/molecule_image.png
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/names.txt
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 massivechem-2.4/THOMAS_IS_BEST/test.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-2.4/Thomas/Copy_spectrometer.py
+-rw-r--r--   0        0        0    49000 2020-02-02 00:00:00.000000 massivechem-2.4/Thomas/Thomas_return.html
+-rw-r--r--   0        0        0    27616 2020-02-02 00:00:00.000000 massivechem-2.4/Thomas/Thomas_return_pyplot.html
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-2.4/Thomas/Thomas_return_pyplot.py
+-rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 massivechem-2.4/Thomas/functions.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-2.4/Thomas/random_tests.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 massivechem-2.4/Thomas/tests.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-2.4/data/abundance.txt
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Acid_image.png
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Acyl_chloride_image.png
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Alcohol_image.png
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Aldehyde_image.png
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Alkene_image.png
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Alkyne_image.png
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Amide_image.png
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Amine_image.png
+-rw-r--r--   0        0        0     8353 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Amino_acid_image.png
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Anhydride_image.png
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Azide_image.png
+-rw-r--r--   0        0        0     8884 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Benzene_image.png
+-rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Carbonate2_image.png
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Carbonate_image.png
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Disulfide_image.png
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Enamine2_image.png
+-rw-r--r--   0        0        0     9081 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Enamine_2_image.png
+-rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Enamine_image.png
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Enol_image.png
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Ester_image.png
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Ether_image.png
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Halogen_image.png
+-rw-r--r--   0        0        0     8205 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Hemiacetal_image.png
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Imide_image.png
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Imine_image.png
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Ketone_image.png
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Nitrile_image.png
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Nitro_image.png
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Peroxide_image.png
+-rw-r--r--   0        0        0     8473 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Phosphate_image.png
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Phosphine_image.png
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Proline_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Sulfides_image.png
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Sulfone_image.png
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Sulfonic_acid_image.png
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Sulfoxide_image.png
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Thio_ether_image.png
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Thioester_image.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 massivechem-2.4/data/Functional groups images/Thiol_image.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-2.4/notebooks/test.ipynb
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 massivechem-2.4/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-2.4/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 massivechem-2.4/LICENSE.txt
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 massivechem-2.4/README.md
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 massivechem-2.4/pyproject.toml
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 massivechem-2.4/PKG-INFO
```

### Comparing `massivechem-2.3/insaturation.py` & `massivechem-2.4/insaturation.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/molecule_image.png` & `massivechem-2.4/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/preliminary.py` & `massivechem-2.4/preliminary.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/project_CH200.yml` & `massivechem-2.4/project_CH200.yml`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/subgroups.py` & `massivechem-2.4/subgroups.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/.idea/workspace.xml` & `massivechem-2.4/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Bokeh/Double plot bokeh.html` & `massivechem-2.4/Bokeh/Double plot bokeh.html`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Bokeh/Double plot bokeh.py` & `massivechem-2.4/Bokeh/Double plot bokeh.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             ticked_peaks.append(x_in[i])
 
     #creates the principal graph, mass spectrum of the molecule (interactive)
 
     p1 = figure(width=700, title=f'Mass spectrum of molecule')
     p1 = figure(x_axis_label = '[m/z]')
     p1 = figure(y_axis_label = 'Abundance')
+    p1.xaxis.axis_label = "[m/z]]"
     p1.height = 500
     p1.xaxis.ticker = FixedTicker(ticks=ticked_peaks)
     p1.add_tools(WheelPanTool(dimension="height"))
     p1.add_tools(WheelZoomTool(dimensions="height"))
     p1.line(x_in, y_in, line_width=1)
     p1.xaxis.major_label_orientation = "vertical"
```

### Comparing `massivechem-2.3/Bokeh/Functional_group_display.html` & `massivechem-2.4/Bokeh/Functional_group_display.html`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Bokeh/Functional_group_display.py` & `massivechem-2.4/Bokeh/Functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Bokeh/Mol_display.html` & `massivechem-2.4/Bokeh/Mol_display.html`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Bokeh/Mol_display.py` & `massivechem-2.4/Bokeh/Mol_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Bokeh/molecule_image.png` & `massivechem-2.4/Bokeh/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/Mol_display.py` & `massivechem-2.4/THOMAS_IS_BEST/Mol_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/Preliminary_v2.py` & `massivechem-2.4/THOMAS_IS_BEST/Preliminary_v2.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/abundance.txt` & `massivechem-2.4/THOMAS_IS_BEST/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/abundance_simplified.txt` & `massivechem-2.4/THOMAS_IS_BEST/abundance_simplified.txt`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/big_func.py` & `massivechem-2.4/THOMAS_IS_BEST/big_func.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/copy_file.py` & `massivechem-2.4/THOMAS_IS_BEST/copy_file.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/functional_group_finder.py` & `massivechem-2.4/THOMAS_IS_BEST/functional_group_finder.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/functions.py` & `massivechem-2.4/THOMAS_IS_BEST/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 #Imports
 
 from rdkit import Chem
 from rdkit.Chem import Draw
+
 import time
 import pandas as pd
+
 import numpy as np
+
 import matplotlib.pyplot as plt
+
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
+
 from bokeh.plotting import figure, show
 from bokeh.models import WheelPanTool, WheelZoomTool
+from bokeh.models import BoxAnnotation, CustomJS
 from bokeh.models.tickers import FixedTicker
+from bokeh.layouts import row
 
 
 
 def data_list_generator():
 
     #---------------------------------------------------------------------------------------------#
     '''
@@ -713,14 +720,87 @@
     if 'Peroxide' in functional_groups_contained:
         functional_groups_contained.remove('Ether')
         functional_groups_contained.remove('Ether')
     
     return functional_groups_contained
 
 
+def double_plot(x_in,y_in):
+    #---------------------------------------------------------------------------------------------#
+    '''
+    double_plot(x_in,y_in)
+    
+    Input: list of masses (x_in) and intensities (y_in)
+    
+    Output: 2 Bokeh graphs:
+            - One that shows the mass spectrum of the molecule to which the user can interact
+            -Another that is the same graph but shows where the user is zooming on the first graph
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    # tells where to put the graduation on the graph
+
+    ticked_peaks = []
+    for i in range(len(x_in)):
+        if y_in[i] > 0.0001:
+            ticked_peaks.append(x_in[i])
+
+    #creates the principal graph, mass spectrum of the molecule (interactive)
+
+    p1 = figure(width=700, title=f'Mass spectrum of molecule')
+    p1 = figure(x_axis_label = '[m/z]')
+    p1 = figure(y_axis_label = 'Abundance')
+    p1.xaxis.axis_label = "[m/z]"
+    p1.height = 500
+    p1.xaxis.ticker = FixedTicker(ticks=ticked_peaks)
+    p1.add_tools(WheelPanTool(dimension="height"))
+    p1.add_tools(WheelZoomTool(dimensions="height"))
+    p1.line(x_in, y_in, line_width=1)
+    p1.xaxis.major_label_orientation = "horizontal"
+
+     #creates the secondary graph, mass spectrum of the molecule (non-interactive)
+
+    p2 = figure(title="Simulated Mass Spectrum", x_axis_label='Mass [Th]', y_axis_label='Intensity')
+    p2 = figure(width=300, title=f'Mass spectrum of molecule')
+    p2 = figure(toolbar_location=None)
+    p2.height = 300
+    p2.line(x_in, y_in, legend_label="Mass spectrum", line_width=1)
+
+    #creates a tool in order that the second graph shows where the zoom is on the first one
+
+    box = BoxAnnotation(left=0, right=0, bottom=0, top=0,
+    fill_alpha=0.1, line_color='red', fill_color='cornflowerblue')
+
+    jscode = """
+        box[%r] = cb_obj.start
+        box[%r] = cb_obj.end
+    """
+
+    xcb = CustomJS(args=dict(box=box), code=jscode % ('left', 'right'))
+    ycb = CustomJS(args=dict(box=box), code=jscode % ('bottom', 'top'))
+
+    p1.x_range.js_on_change('start', xcb)
+    p1.x_range.js_on_change('end', xcb)
+    p1.y_range.js_on_change('start', ycb)
+    p1.y_range.js_on_change('end', ycb)
+
+    # adds the functionnality to the second figure
+
+    p2.add_layout(box)
+
+    # creates a layout that displays the 2 graphs
+
+    layout = row(p1, p2)
+    show(layout)
+
+    return layout
+
+
+
+
 
 
 
 
 #Actually makes code run
 
 
@@ -755,14 +835,14 @@
 end_time = time.time()
 
 duration = end_time-start_time
 
 #Plotter
 '''
 print(pyplot_plotter(x_axis, y_axis))'''
-print(bokeh_plotter(x_axis,y_axis))
+print(double_plot(x_axis,y_axis))
 '''print(functional_group_finder(mol_smi))
 print(f'Computation complete')
 print(f'Process took: {duration} s')'''
 
 print(functional_group_finder(mol_smi))
 print(SMILEs_interpreter('c1ccccc1CCBr'))
```

### Comparing `massivechem-2.3/THOMAS_IS_BEST/molecule_image.png` & `massivechem-2.4/THOMAS_IS_BEST/molecule_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/THOMAS_IS_BEST/test.py` & `massivechem-2.4/THOMAS_IS_BEST/test.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Thomas/Copy_spectrometer.py` & `massivechem-2.4/Thomas/Copy_spectrometer.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Thomas/Thomas_return.html` & `massivechem-2.4/Thomas/Thomas_return.html`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Thomas/Thomas_return_pyplot.html` & `massivechem-2.4/Thomas/Thomas_return_pyplot.html`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Thomas/Thomas_return_pyplot.py` & `massivechem-2.4/Thomas/Thomas_return_pyplot.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Thomas/functions.html` & `massivechem-2.4/Thomas/functions.html`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/Thomas/tests.py` & `massivechem-2.4/Thomas/tests.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/abundance.txt` & `massivechem-2.4/data/abundance.txt`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Acid_image.png` & `massivechem-2.4/data/Functional groups images/Acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Acyl_chloride_image.png` & `massivechem-2.4/data/Functional groups images/Acyl_chloride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Alcohol_image.png` & `massivechem-2.4/data/Functional groups images/Alcohol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Aldehyde_image.png` & `massivechem-2.4/data/Functional groups images/Aldehyde_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Alkene_image.png` & `massivechem-2.4/data/Functional groups images/Alkene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Alkyne_image.png` & `massivechem-2.4/data/Functional groups images/Alkyne_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Amide_image.png` & `massivechem-2.4/data/Functional groups images/Amide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Amine_image.png` & `massivechem-2.4/data/Functional groups images/Amine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Amino_acid_image.png` & `massivechem-2.4/data/Functional groups images/Amino_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Anhydride_image.png` & `massivechem-2.4/data/Functional groups images/Anhydride_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Azide_image.png` & `massivechem-2.4/data/Functional groups images/Azide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Benzene_image.png` & `massivechem-2.4/data/Functional groups images/Benzene_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Carbonate2_image.png` & `massivechem-2.4/data/Functional groups images/Carbonate2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Carbonate_image.png` & `massivechem-2.4/data/Functional groups images/Carbonate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Disulfide_image.png` & `massivechem-2.4/data/Functional groups images/Disulfide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Enamine2_image.png` & `massivechem-2.4/data/Functional groups images/Enamine2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Enamine_2_image.png` & `massivechem-2.4/data/Functional groups images/Enamine_2_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Enamine_image.png` & `massivechem-2.4/data/Functional groups images/Enamine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Enol_image.png` & `massivechem-2.4/data/Functional groups images/Enol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Ester_image.png` & `massivechem-2.4/data/Functional groups images/Ester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Ether_image.png` & `massivechem-2.4/data/Functional groups images/Ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Halogen_image.png` & `massivechem-2.4/data/Functional groups images/Halogen_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Hemiacetal_image.png` & `massivechem-2.4/data/Functional groups images/Hemiacetal_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Imide_image.png` & `massivechem-2.4/data/Functional groups images/Imide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Imine_image.png` & `massivechem-2.4/data/Functional groups images/Imine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Ketone_image.png` & `massivechem-2.4/data/Functional groups images/Ketone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Nitrile_image.png` & `massivechem-2.4/data/Functional groups images/Nitrile_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Nitro_image.png` & `massivechem-2.4/data/Functional groups images/Nitro_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Peroxide_image.png` & `massivechem-2.4/data/Functional groups images/Peroxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Phosphate_image.png` & `massivechem-2.4/data/Functional groups images/Phosphate_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Phosphine_image.png` & `massivechem-2.4/data/Functional groups images/Phosphine_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Proline_image.png` & `massivechem-2.4/data/Functional groups images/Proline_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Sulfides_image.png` & `massivechem-2.4/data/Functional groups images/Sulfides_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Sulfone_image.png` & `massivechem-2.4/data/Functional groups images/Sulfone_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Sulfonic_acid_image.png` & `massivechem-2.4/data/Functional groups images/Sulfonic_acid_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Sulfoxide_image.png` & `massivechem-2.4/data/Functional groups images/Sulfoxide_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Thio_ether_image.png` & `massivechem-2.4/data/Functional groups images/Thio_ether_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Thioester_image.png` & `massivechem-2.4/data/Functional groups images/Thioester_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/data/Functional groups images/Thiol_image.png` & `massivechem-2.4/data/Functional groups images/Thiol_image.png`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/src/MASSiveChem/MASSiveChem.py` & `massivechem-2.4/src/MASSiveChem/MASSiveChem.py`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/LICENSE.txt` & `massivechem-2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/README.md` & `massivechem-2.4/README.md`

 * *Files identical despite different names*

### Comparing `massivechem-2.3/pyproject.toml` & `massivechem-2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "MASSiveChem"
-version = "2.3"
+version = "2.4"
 description = "..."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["unsaturation", "Mass spectroscopy"]
 authors = [
   { name = "Thomas Christianson", email = "thomas.christiansson@epfl.ch" },
```

### Comparing `massivechem-2.3/PKG-INFO` & `massivechem-2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSiveChem
-Version: 2.3
+Version: 2.4
 Summary: ...
 Project-URL: Homepage, https://github.com/ThomasCsson/ppchem-project-Christiansson-Gonteri-Humery.git
 Author-email: Thomas Christianson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: Mass spectroscopy,unsaturation
 Classifier: Development Status :: 4 - Beta
```

