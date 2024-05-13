# Comparing `tmp/directory_structure_generator-1.0.2.tar.gz` & `tmp/directory_structure_generator-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directory_structure_generator-1.0.2.tar", last modified: Mon May 13 15:42:27 2024, max compression
+gzip compressed data, was "directory_structure_generator-1.0.3.tar", last modified: Mon May 13 16:22:12 2024, max compression
```

## Comparing `directory_structure_generator-1.0.2.tar` & `directory_structure_generator-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ahmedkhalil (939785259) 1494203198        0 2024-05-13 15:42:27.042679 directory_structure_generator-1.0.2/
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198     1069 2024-05-12 10:39:33.000000 directory_structure_generator-1.0.2/LICENSE
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198     3851 2024-05-13 15:42:27.042472 directory_structure_generator-1.0.2/PKG-INFO
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198     3267 2024-05-13 15:41:02.000000 directory_structure_generator-1.0.2/README.md
-drwxr-xr-x   0 ahmedkhalil (939785259) 1494203198        0 2024-05-13 15:42:27.040446 directory_structure_generator-1.0.2/directory_structure_generator/
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198      350 2024-05-13 15:14:13.000000 directory_structure_generator-1.0.2/directory_structure_generator/__init__.py
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198      896 2024-05-13 15:10:58.000000 directory_structure_generator-1.0.2/directory_structure_generator/__main__.py
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198      673 2024-05-13 10:43:17.000000 directory_structure_generator-1.0.2/directory_structure_generator/colors.py
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198     2702 2024-05-13 15:11:02.000000 directory_structure_generator-1.0.2/directory_structure_generator/generator.py
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198      785 2024-05-13 10:44:35.000000 directory_structure_generator-1.0.2/directory_structure_generator/icons.py
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198       66 2024-05-13 15:14:13.000000 directory_structure_generator-1.0.2/directory_structure_generator/run.py
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198     2336 2024-05-13 15:11:11.000000 directory_structure_generator-1.0.2/directory_structure_generator/utils.py
-drwxr-xr-x   0 ahmedkhalil (939785259) 1494203198        0 2024-05-13 15:42:27.042257 directory_structure_generator-1.0.2/directory_structure_generator.egg-info/
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198     3851 2024-05-13 15:42:27.000000 directory_structure_generator-1.0.2/directory_structure_generator.egg-info/PKG-INFO
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198      680 2024-05-13 15:42:27.000000 directory_structure_generator-1.0.2/directory_structure_generator.egg-info/SOURCES.txt
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198        1 2024-05-13 15:42:27.000000 directory_structure_generator-1.0.2/directory_structure_generator.egg-info/dependency_links.txt
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198       94 2024-05-13 15:42:27.000000 directory_structure_generator-1.0.2/directory_structure_generator.egg-info/entry_points.txt
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198        1 2024-05-13 15:36:59.000000 directory_structure_generator-1.0.2/directory_structure_generator.egg-info/not-zip-safe
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198        9 2024-05-13 15:42:27.000000 directory_structure_generator-1.0.2/directory_structure_generator.egg-info/requires.txt
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198       30 2024-05-13 15:42:27.000000 directory_structure_generator-1.0.2/directory_structure_generator.egg-info/top_level.txt
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198       38 2024-05-13 15:42:27.042722 directory_structure_generator-1.0.2/setup.cfg
--rw-r--r--   0 ahmedkhalil (939785259) 1494203198      937 2024-05-13 15:31:59.000000 directory_structure_generator-1.0.2/setup.py
+drwxr-xr-x   0 ahmedkhalil (939785259) 1494203198        0 2024-05-13 16:22:12.553072 directory_structure_generator-1.0.3/
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198     1069 2024-05-12 10:39:33.000000 directory_structure_generator-1.0.3/LICENSE
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198     3940 2024-05-13 16:22:12.552868 directory_structure_generator-1.0.3/PKG-INFO
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198     3356 2024-05-13 16:21:21.000000 directory_structure_generator-1.0.3/README.md
+drwxr-xr-x   0 ahmedkhalil (939785259) 1494203198        0 2024-05-13 16:22:12.550776 directory_structure_generator-1.0.3/directory_structure_generator/
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198      350 2024-05-13 15:14:13.000000 directory_structure_generator-1.0.3/directory_structure_generator/__init__.py
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198      937 2024-05-13 16:05:21.000000 directory_structure_generator-1.0.3/directory_structure_generator/__main__.py
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198      673 2024-05-13 10:43:17.000000 directory_structure_generator-1.0.3/directory_structure_generator/colors.py
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198     2369 2024-05-13 16:06:34.000000 directory_structure_generator-1.0.3/directory_structure_generator/generator.py
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198      785 2024-05-13 10:44:35.000000 directory_structure_generator-1.0.3/directory_structure_generator/icons.py
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198       66 2024-05-13 15:14:13.000000 directory_structure_generator-1.0.3/directory_structure_generator/run.py
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198     2757 2024-05-13 16:07:02.000000 directory_structure_generator-1.0.3/directory_structure_generator/utils.py
+drwxr-xr-x   0 ahmedkhalil (939785259) 1494203198        0 2024-05-13 16:22:12.552639 directory_structure_generator-1.0.3/directory_structure_generator.egg-info/
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198     3940 2024-05-13 16:22:12.000000 directory_structure_generator-1.0.3/directory_structure_generator.egg-info/PKG-INFO
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198      680 2024-05-13 16:22:12.000000 directory_structure_generator-1.0.3/directory_structure_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198        1 2024-05-13 16:22:12.000000 directory_structure_generator-1.0.3/directory_structure_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198       94 2024-05-13 16:22:12.000000 directory_structure_generator-1.0.3/directory_structure_generator.egg-info/entry_points.txt
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198        1 2024-05-13 15:36:59.000000 directory_structure_generator-1.0.3/directory_structure_generator.egg-info/not-zip-safe
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198        9 2024-05-13 16:22:12.000000 directory_structure_generator-1.0.3/directory_structure_generator.egg-info/requires.txt
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198       30 2024-05-13 16:22:12.000000 directory_structure_generator-1.0.3/directory_structure_generator.egg-info/top_level.txt
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198       38 2024-05-13 16:22:12.553118 directory_structure_generator-1.0.3/setup.cfg
+-rw-r--r--   0 ahmedkhalil (939785259) 1494203198      937 2024-05-13 16:11:49.000000 directory_structure_generator-1.0.3/setup.py
```

### Comparing `directory_structure_generator-1.0.2/LICENSE` & `directory_structure_generator-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `directory_structure_generator-1.0.2/PKG-INFO` & `directory_structure_generator-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,56 @@
-Metadata-Version: 2.1
-Name: directory_structure_generator
-Version: 1.0.2
-Summary: This script is used to generate a list of the project structure in a markdown format. It is useful for README.md files.
-Home-page: https://github.com/7oSkaaa/directory_structure_generator
-Author: Ahmed Hossam
-Author-email: ahmed.7oskaa@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: argparse
-
 # Directory Structure Generator Script
 
 ## Description
 
 This script is used to generate a list of the project structure in a markdown format. It is useful for README.md files.
 
-## Usage
+## Download
+
+- You can simply:
+    ```bash
+    pip install directory-structure-generator 
+    ```
+  
+- Or you can clone the repository:
 
-### pre-execution
+    ```bash
+    git clone git@github.com:7oSkaaa/directory_structure_generator.git
+    cd directory_structure_generator
+    python -m directory_structure_generator --path <path> --language <language> --sort <sort>
+    ```  
 
-- Update the `exclude.txt` file with the files and folders to exclude from the project structure list
+## Usage
 
 ### Command
 
-```bash
-python -m directory_structure_generator --path <path> --language <language> --sort <sort>
-```
+***We have two ways to use the script:***
+- **First way:** 
+  - Clone the repository
+  - Change the directory to the repository
+  - Run the script with the required arguments
+      ```bash
+      python -m directory_structure_generator --path <path> --exclude_dirs <dir_1> <dir_2> <dir_3> --language <language> --sort <sort>
+      ```
+- **Second way:**
+  - Install the package using pip
+  - Run the script with the required arguments
+    ```bash
+    python
+    from directory_structure_generator import directory_structure_generator
+    directory_structure_generator(path=<path>, exclude_dirs=[<dir_1>, <dir_2>, <dir_3>], language=<language>, sort=<sort>)
+    ```
 
 ### Arguments
 
 - `--path` : Path to the project folder
+- `--exclude_dirs` : List of directories to exclude from the project structure. Default is `[]`
 - `--language` : Language of the project. Default is `plaintext`
 - `--sort` : Sort the folders and files. Default is `False`
 
-### Example
-
-```bash
-python -m directory_structure_generator --path 'Users/ahmed_hossam/Codes' --language 'python' --sort 'True'
-```
-
 ## Output Example
 
 ### frontend-training-mp-feb24 folder structure
 
 ```js
 📁 frontend-training-mp-feb24
 ├───📄 App.js
@@ -92,30 +96,7 @@
 │   │   └───📄 index.jsx
 │   └───📁 services
 │   │   ├───📄 api.js
 │   │   ├───📄 cartService.js
 │   │   └───📄 productService.js
 └───📄 yarn.lock
 ```
-
-### How to use the script
-
-1. Open the terminal
-2. Navigate to the folder where the script is located
-3. Run the script with the required arguments
-4. Copy the output and paste it in the README.md file
-5. Commit the changes
-6. Push the changes to the repository
-7. Check the README.md file in the repository
-8. The project structure will be displayed in the markdown format
-
-### How to get the script
-
-1. Clone the repository
-
-    ```bash
-    git clone git@github.com:7oSkaaa/directory_structure_generator.git
-    ```
-
-2. Navigate to the folder where the script is located
-3. Run the script with the required arguments
-4. Copy the output and paste it in the README.md file
```

### Comparing `directory_structure_generator-1.0.2/directory_structure_generator/__main__.py` & `directory_structure_generator-1.0.3/directory_structure_generator/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .generator import directory_structure_generator
 from .utils import get_args
 
 
 def main():
     # Get the path to the folder to analyze from the CLI
     try:
-        path, language, sort = get_args()
+        path, exclude_dirs, language, sort = get_args()
 
         # Check if the sort argument is a boolean
         sort = True if sort.lower() == "true" else False
 
         print(f"{Colors.green}The arguments have been provided ✅{Colors.reset}")
     except SystemExit:
         print(f"{Colors.red}The arguments was not provided ❌{Colors.reset}")
@@ -21,12 +21,12 @@
 
     # Check if the path exists
     if not os.path.exists(path):
         print(f"{Colors.red}The path {path} does not exist. ❌{Colors.reset}")
         sys.exit(1)
 
     # Generate the folder structure and print it
-    directory_structure_generator(path=path, language=language, sort=sort)
+    directory_structure_generator(path=path, exclude_dirs=exclude_dirs, language=language, sort=sort)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `directory_structure_generator-1.0.2/directory_structure_generator/colors.py` & `directory_structure_generator-1.0.3/directory_structure_generator/colors.py`

 * *Files identical despite different names*

### Comparing `directory_structure_generator-1.0.2/directory_structure_generator/generator.py` & `directory_structure_generator-1.0.3/directory_structure_generator/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     try:
         dirs = os.listdir(path)
     except PermissionError:
         print(f"{Colors.red}Permission denied for {path} ❌{Colors.reset}")
         exit(1)
 
     # Remove the directories to exclude
-    dirs = [d for d in dirs if d not in exclude_dirs]
+    dirs = [d for d in dirs if d.lower() not in exclude_dirs]
 
     # Sort the directories and files alphabetically
     if sort:
         dirs.sort()
 
     # Create the path to add
     to_add = PATH * degree
@@ -52,28 +52,18 @@
 def folder_structure(path, exclude_dirs, sort=False):
     # Build the folder structure
     build_structure(path=path, exclude_dirs=exclude_dirs, degree=0, ends=0, sort=sort)
 
     return structure
 
 
-def directory_structure_generator(path=None, language=None, sort=False):
+def directory_structure_generator(path=None, exclude_dirs=None, language=None, sort=False):
     # starting the program
     print(f"{Colors.yellow}{Icons.loading} Starting the program...{Colors.reset}")
 
-    try:
-        # get directory to the path
-        directory = os.path.dirname(os.path.realpath(__file__))
-
-        # Get the directories to exclude
-        exclude_dirs = get_from_file(f"{directory}/exclude_dirs.txt")
-    except FileNotFoundError:
-        print(f"{Colors.red}The file exclude_dirs.txt was not found ❌{Colors.reset}")
-        sys.exit(1)
-
     global structure
 
     # Create the folder structure
     structure = folder_structure(path=path, exclude_dirs=exclude_dirs, sort=sort)
 
     # Remove the extras
     structure = remove_extras(structure)
```

### Comparing `directory_structure_generator-1.0.2/directory_structure_generator/icons.py` & `directory_structure_generator-1.0.3/directory_structure_generator/icons.py`

 * *Files identical despite different names*

### Comparing `directory_structure_generator-1.0.2/directory_structure_generator/utils.py` & `directory_structure_generator-1.0.3/directory_structure_generator/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,26 +62,40 @@
     )
     parser.add_argument(
         "--path",
         dest="path",
         default=os.getcwd(),
         help="The path to the folder to analyze.",
         required=False,
+        type=str,
+    )
+    parser.add_argument(
+        "--exclude_dirs",
+        dest="exclude_dirs",
+        default=[],
+        help="The directories to exclude from the structure separated by spaces.",
+        nargs="+",
+        required=False,
     )
     parser.add_argument(
         "--language",
         dest="language",
         default="plaintext",
         help="The language to use for the folder structure.",
         required=False,
+        type=str,
     )
     parser.add_argument(
         "--sort",
         dest="sort",
         default="False",
         help="Sort the directories and files alphabetically.",
         required=False,
+        type=str,
     )
     print(f"{Colors.yellow}{Icons.loading} Parsing the arguments...{Colors.reset}")
     args = parser.parse_args()  # Parse the arguments
 
-    return args.path, args.language, args.sort
+    # make all the directories to exclude lowercase
+    args.exclude_dirs = [d.lower() for d in args.exclude_dirs]
+
+    return args.path, args.exclude_dirs, args.language, args.sort
```

### Comparing `directory_structure_generator-1.0.2/directory_structure_generator.egg-info/PKG-INFO` & `directory_structure_generator-1.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory_structure_generator
-Version: 1.0.2
+Version: 1.0.3
 Summary: This script is used to generate a list of the project structure in a markdown format. It is useful for README.md files.
 Home-page: https://github.com/7oSkaaa/directory_structure_generator
 Author: Ahmed Hossam
 Author-email: ahmed.7oskaa@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,38 +15,57 @@
 
 # Directory Structure Generator Script
 
 ## Description
 
 This script is used to generate a list of the project structure in a markdown format. It is useful for README.md files.
 
-## Usage
+## Download
 
-### pre-execution
+- You can simply:
+    ```bash
+    pip install directory-structure-generator 
+    ```
+  
+- Or you can clone the repository:
 
-- Update the `exclude.txt` file with the files and folders to exclude from the project structure list
+    ```bash
+    git clone git@github.com:7oSkaaa/directory_structure_generator.git
+    cd directory_structure_generator
+    python -m directory_structure_generator --path <path> --language <language> --sort <sort>
+    ```  
+
+## Usage
 
 ### Command
 
-```bash
-python -m directory_structure_generator --path <path> --language <language> --sort <sort>
-```
+***We have two ways to use the script:***
+- **First way:** 
+  - Clone the repository
+  - Change the directory to the repository
+  - Run the script with the required arguments
+      ```bash
+      python -m directory_structure_generator --path <path> --exclude_dirs <dir_1> <dir_2> <dir_3> --language <language> --sort <sort>
+      ```
+- **Second way:**
+  - Install the package using pip
+  - Run the script with the required arguments
+    ```bash
+    python
+    from directory_structure_generator import directory_structure_generator
+    directory_structure_generator(path=<path>, exclude_dirs=[<dir_1>, <dir_2>, <dir_3>], language=<language>, sort=<sort>)
+    ```
 
 ### Arguments
 
 - `--path` : Path to the project folder
+- `--exclude_dirs` : List of directories to exclude from the project structure. Default is `[]`
 - `--language` : Language of the project. Default is `plaintext`
 - `--sort` : Sort the folders and files. Default is `False`
 
-### Example
-
-```bash
-python -m directory_structure_generator --path 'Users/ahmed_hossam/Codes' --language 'python' --sort 'True'
-```
-
 ## Output Example
 
 ### frontend-training-mp-feb24 folder structure
 
 ```js
 📁 frontend-training-mp-feb24
 ├───📄 App.js
@@ -92,30 +111,7 @@
 │   │   └───📄 index.jsx
 │   └───📁 services
 │   │   ├───📄 api.js
 │   │   ├───📄 cartService.js
 │   │   └───📄 productService.js
 └───📄 yarn.lock
 ```
-
-### How to use the script
-
-1. Open the terminal
-2. Navigate to the folder where the script is located
-3. Run the script with the required arguments
-4. Copy the output and paste it in the README.md file
-5. Commit the changes
-6. Push the changes to the repository
-7. Check the README.md file in the repository
-8. The project structure will be displayed in the markdown format
-
-### How to get the script
-
-1. Clone the repository
-
-    ```bash
-    git clone git@github.com:7oSkaaa/directory_structure_generator.git
-    ```
-
-2. Navigate to the folder where the script is located
-3. Run the script with the required arguments
-4. Copy the output and paste it in the README.md file
```

### Comparing `directory_structure_generator-1.0.2/directory_structure_generator.egg-info/SOURCES.txt` & `directory_structure_generator-1.0.3/directory_structure_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `directory_structure_generator-1.0.2/setup.py` & `directory_structure_generator-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="directory_structure_generator",
-    version="1.0.2",
+    version="1.0.3",
     author="Ahmed Hossam",
     author_email="ahmed.7oskaa@gmail.com",
     description="This script is used to generate a list of the project structure in a markdown format. It is useful for README.md files.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/7oSkaaa/directory_structure_generator",
     packages=find_packages(),
```

