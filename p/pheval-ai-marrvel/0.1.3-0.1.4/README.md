# Comparing `tmp/pheval_ai_marrvel-0.1.3.tar.gz` & `tmp/pheval_ai_marrvel-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheval_ai_marrvel-0.1.3.tar", max compression
+gzip compressed data, was "pheval_ai_marrvel-0.1.4.tar", max compression
```

## Comparing `pheval_ai_marrvel-0.1.3.tar` & `pheval_ai_marrvel-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2472 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/README.md
--rw-r--r--   0        0        0      875 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/__init__.py
--rw-r--r--   0        0        0      211 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/cli.py
--rw-r--r--   0        0        0        0 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/post_process/__init__.py
--rw-r--r--   0        0        0      546 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/post_process/post_process.py
--rw-r--r--   0        0        0     5688 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/post_process/post_process_results_format.py
--rw-r--r--   0        0        0        0 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/prepare/__init__.py
--rw-r--r--   0        0        0      248 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/prepare/prepare.py
--rw-r--r--   0        0        0     1182 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/prepare/prepare_input.py
--rw-r--r--   0        0        0        0 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/run/__init__.py
--rw-r--r--   0        0        0     2571 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/run/create_apptainer_commands.py
--rw-r--r--   0        0        0      505 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/run/run.py
--rw-r--r--   0        0        0     1354 2024-05-11 13:02:46.231831 pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/runner.py
--rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 pheval_ai_marrvel-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1635 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/README.md
+-rw-r--r--   0        0        0      875 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/__init__.py
+-rw-r--r--   0        0        0      213 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/cli.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/post_process/__init__.py
+-rw-r--r--   0        0        0     1016 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/post_process/post_process.py
+-rw-r--r--   0        0        0     6542 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/post_process/post_process_results_format.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/prepare/__init__.py
+-rw-r--r--   0        0        0      406 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/prepare/prepare.py
+-rw-r--r--   0        0        0     1843 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/prepare/prepare_input.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/run/__init__.py
+-rw-r--r--   0        0        0     4220 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/run/create_apptainer_commands.py
+-rw-r--r--   0        0        0      827 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/run/run.py
+-rw-r--r--   0        0        0     1376 2024-05-13 12:51:34.257419 pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/runner.py
+-rw-r--r--   0        0        0     2076 1970-01-01 00:00:00.000000 pheval_ai_marrvel-0.1.4/PKG-INFO
```

### Comparing `pheval_ai_marrvel-0.1.3/pyproject.toml` & `pheval_ai_marrvel-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pheval-ai-marrvel"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>"]
 readme = "README.md"
 packages = [{include = "pheval_ai_marrvel", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/post_process/post_process_results_format.py` & `pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/post_process/post_process_results_format.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     Read the raw result file.
 
     Args:
         raw_result_path(Path): Path to the raw result file.
 
     Returns:
-        List[dict]: Contents of the raw result file.
+        pl.DataFrame: Contents of the raw result file.
     """
     raw_result = pl.read_csv(raw_result_path)
     raw_result = raw_result.rename({"Unnamed: 0": "variant"})
     return raw_result.select(pl.col(["variant", "predict", "geneSymbol"]))
 
 
 class ConvertToPhEvalResult:
@@ -77,26 +77,62 @@
         Returns:
             str: The gene identifier.
         """
         return self.gene_identifier_updater.find_identifier(self._obtain_gene_symbol(result_entry))
 
     @staticmethod
     def obtain_chrom(variant_str: str) -> str:
+        """
+        Obtain the chromosome from the variant entry.
+
+        Args:
+            variant_str (str): Variant entry.
+
+        Returns:
+            str: The chromosome.
+        """
         return variant_str.split("-")[0]
 
     @staticmethod
     def obtain_pos(variant_str: str) -> int:
+        """
+        Obtain the position from the variant entry.
+
+        Args:
+            variant_str (str): Variant entry.
+
+        Returns:
+            int: The position.
+        """
         return int(variant_str.split("-")[1])
 
     @staticmethod
     def obtain_ref(variant_str: str) -> str:
+        """
+        Obtain the reference allele from the variant entry.
+
+        Args:
+            variant_str (str): Variant entry.
+
+        Returns:
+            str: The reference allele.
+        """
         return variant_str.split("-")[2]
 
     @staticmethod
     def obtain_alt(variant_str: str) -> str:
+        """
+        Obtain the alternate allele from the variant entry.
+
+        Args:
+            variant_str (str): Variant entry.
+
+        Returns:
+            str: The alternate allele.
+        """
         return variant_str.split("-")[3]
 
     def extract_pheval_gene_requirements(self) -> List[PhEvalGeneResult]:
         """
         Extract the data required to produce PhEval gene output.
 
         Returns:
@@ -120,14 +156,15 @@
         Returns:
             List[PhEvalVariantResult]: List of PhEvalVariantResult objects.
         """
         pheval_result = []
         for result_entry in self.raw_result.rows(named=True):
             pheval_result.append(
                 PhEvalVariantResult(
+                    score=self._obtain_score(result_entry),
                     chromosome=self.obtain_chrom(result_entry["variant"]),
                     start=self.obtain_pos(result_entry["variant"]),
                     end=calculate_end_pos(
                         self.obtain_pos(result_entry["variant"]),
                         self.obtain_ref(result_entry["variant"]),
                     ),
                     ref=self.obtain_ref(result_entry["variant"]),
@@ -135,15 +172,15 @@
                 )
             )
         return pheval_result
 
 
 def create_standardised_results(raw_results_dir: Path, output_dir: Path) -> None:
     """
-    Create PhEval gene tsv output from raw results.
+    Create PhEval gene and variant tsv output from raw results.
 
     Args:
         raw_results_dir (Path): Path to the raw results directory.
         output_dir (Path): Path to the output directory.
     """
     gene_identifier_updator = GeneIdentifierUpdater(
         gene_identifier="ensembl_id", hgnc_data=create_hgnc_dict()
```

### Comparing `pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/prepare/prepare_input.py` & `pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/prepare/prepare_input.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,30 +2,59 @@
 
 from phenopackets import Phenopacket
 from pheval.utils.file_utils import all_files
 from pheval.utils.phenopacket_utils import PhenopacketUtil, phenopacket_reader
 
 
 def obtain_observed_hpo_ids(phenopacket: Phenopacket) -> str:
+    """
+    Obtain observed hpo ids from a Phenopacket.
+
+    Args:
+        phenopacket (Phenopacket): Phenopacket object.
+
+    Returns:
+        str: Observed hpo ids.
+    """
     observed_phenotypes = PhenopacketUtil(phenopacket).observed_phenotypic_features()
     observed_hpo_ids = [hpo_id.type.id for hpo_id in observed_phenotypes]
     observed_hpo_ids = "\n".join(observed_hpo_ids)
     return observed_hpo_ids
 
 
 def write_txt_input(observed_hpo_ids: str, output_file_name: Path) -> None:
+    """
+    Write observed hpo ids to a txt file.
+
+    Args:
+        observed_hpo_ids (str): Observed hpo ids.
+        output_file_name (str): Output file name.
+    """
     with open(output_file_name, "w") as f:
         f.write(observed_hpo_ids)
     f.close()
 
 
 def write_observed_hpo_ids(phenopacket_path: Path, testdata_dir: Path) -> None:
+    """
+    Write observed hpo ids to a txt file.
+
+    Args:
+        phenopacket_path (Path): Phenopacket path.
+        testdata_dir (Path): Path to test data directory.
+    """
     phenopacket = phenopacket_reader(phenopacket_path)
     observed_hpo_ids = obtain_observed_hpo_ids(phenopacket)
     write_txt_input(
         observed_hpo_ids, Path(testdata_dir).joinpath(f"hpo_ids/{phenopacket_path.stem}.txt")
     )
 
 
 def write_input_txt_files(testdata_dir: Path) -> None:
+    """
+    Write observed hpo ids to txt files for a corpus.
+
+    Args:
+        testdata_dir (Path): Path to test data directory.
+    """
     for phenopacket_path in all_files(Path(testdata_dir).joinpath("phenopackets")):
         write_observed_hpo_ids(phenopacket_path, testdata_dir)
```

### Comparing `pheval_ai_marrvel-0.1.3/src/pheval_ai_marrvel/runner.py` & `pheval_ai_marrvel-0.1.4/src/pheval_ai_marrvel/runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     tmp_dir: Path
     output_dir: Path
     config_file: Path
     version: str
 
     def prepare(self):
         """
-        Pre-process any data and inputs necessary to run the tool.
+        Pre-process phenopackets into tool accepted format.
         """
-        print("preparing")
+        print("creating HPO txt files from phenopackets")
         prepare_inputs(testdata_dir=self.testdata_dir)
 
     def run(self):
         """
-        Run the tool to produce the raw output.
+        Run AI-MARRVEL to produce the raw output.
         """
-        print("running with fake predictor")
+        print("running with AI-MARRVEL")
         run_commands(
             tool_input_commands_dir=self.tool_input_commands_dir,
             testdata_dir=self.testdata_dir,
             input_dir=self.input_dir,
             output_dir=self.output_dir,
         )
```

