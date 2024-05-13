# Comparing `tmp/easy_configer-2.3.2.tar.gz` & `tmp/easy_configer-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_configer-2.3.2.tar", last modified: Thu Apr  4 14:37:13 2024, max compression
+gzip compressed data, was "dist/easy_configer-2.5.0.tar", last modified: Mon May 13 13:17:01 2024, max compression
```

## Comparing `easy_configer-2.3.2.tar` & `easy_configer-2.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 14:37:14.922305 easy_configer-2.3.2/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21683 2024-04-04 14:37:14.921301 easy_configer-2.3.2/PKG-INFO
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21094 2024-04-04 14:34:44.000000 easy_configer-2.3.2/README.md
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 14:37:14.847288 easy_configer-2.3.2/easy_configer/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    14856 2024-04-04 09:04:41.000000 easy_configer-2.3.2/easy_configer/Configer.py
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     5021 2024-04-04 09:04:41.000000 easy_configer-2.3.2/easy_configer/IO_Converter.py
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 14:37:14.909292 easy_configer-2.3.2/easy_configer/utils/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     2059 2024-04-04 09:04:41.000000 easy_configer-2.3.2/easy_configer/utils/Container.py
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     4801 2024-04-04 09:04:41.000000 easy_configer-2.3.2/easy_configer/utils/Type_Convertor.py
-drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-04-04 14:37:14.887290 easy_configer-2.3.2/easy_configer.egg-info/
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21683 2024-04-04 14:37:14.000000 easy_configer-2.3.2/easy_configer.egg-info/PKG-INFO
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)      293 2024-04-04 14:37:14.000000 easy_configer-2.3.2/easy_configer.egg-info/SOURCES.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)        1 2024-04-04 14:37:14.000000 easy_configer-2.3.2/easy_configer.egg-info/dependency_links.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)       34 2024-04-04 14:37:14.000000 easy_configer-2.3.2/easy_configer.egg-info/top_level.txt
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)       38 2024-04-04 14:37:14.923291 easy_configer-2.3.2/setup.cfg
--rwxrwxrwx   0 joseph    (1000) joseph    (1000)     1057 2024-04-04 14:37:07.000000 easy_configer-2.3.2/setup.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-05-13 13:17:01.703822 easy_configer-2.5.0/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    22294 2024-05-13 13:17:01.701846 easy_configer-2.5.0/PKG-INFO
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    21705 2024-05-13 13:16:32.000000 easy_configer-2.5.0/README.md
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-05-13 13:17:01.636820 easy_configer-2.5.0/easy_configer/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    14500 2024-05-13 13:09:46.000000 easy_configer-2.5.0/easy_configer/Configer.py
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     5021 2024-05-13 13:09:46.000000 easy_configer-2.5.0/easy_configer/IO_Converter.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-05-13 13:17:01.691823 easy_configer-2.5.0/easy_configer/utils/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     2059 2024-05-13 13:09:46.000000 easy_configer-2.5.0/easy_configer/utils/Container.py
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     7250 2024-05-13 13:09:46.000000 easy_configer-2.5.0/easy_configer/utils/Type_Convertor.py
+drwxrwxrwx   0 joseph    (1000) joseph    (1000)        0 2024-05-13 13:17:01.671838 easy_configer-2.5.0/easy_configer.egg-info/
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)    22294 2024-05-13 13:17:01.000000 easy_configer-2.5.0/easy_configer.egg-info/PKG-INFO
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)      293 2024-05-13 13:17:01.000000 easy_configer-2.5.0/easy_configer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)        1 2024-05-13 13:17:01.000000 easy_configer-2.5.0/easy_configer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)       34 2024-05-13 13:17:01.000000 easy_configer-2.5.0/easy_configer.egg-info/top_level.txt
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)       38 2024-05-13 13:17:01.703822 easy_configer-2.5.0/setup.cfg
+-rwxrwxrwx   0 joseph    (1000) joseph    (1000)     1057 2024-05-13 13:10:39.000000 easy_configer-2.5.0/setup.py
```

### Comparing `easy_configer-2.3.2/PKG-INFO` & `easy_configer-2.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-Metadata-Version: 2.1
-Name: easy_configer
-Version: 2.3.2
-Summary: An easy way for configurating python program by the given config file or config str
-Home-page: https://github.com/HuangChiEn/easy_config
-Author: JosefHuang
-Author-email: a3285556aa@gmail.com
-License: MIT
-Keywords: configuration,commendline argument,argument
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 # Project description
-#### easy_configer version : 2.3.2
+#### easy_configer version : 2.5.0
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
 ![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
@@ -69,21 +53,22 @@
 
 * support arguments interpolation!!
 
 * support config conversion, which turn easy_config into the other kind of config package (omegaconf, argparse, ..., etc.)
 
 * support hierachical configurating system with dynamic override ~
 
+* better support for argument intepolation (inline-intepolation is allowed now ~)
+
 ---
 
 ### Newly update features 🚀
-1. Enable all test case (automatically ci by git-action)
-2. Support dot-access of any arguments
-3. Consistent import syntax.. 
-4. New document is released ~
+1. Single-line python code execution via ${...} in config file
+2. Integrate argument intepolation via ${cfg} with special object
+3. Integrate enviroment variable intepolation via ${env} with special object
 
 ---
 
 ### Bug Fixed 🐛
 #### Fix-up import syntax.. plz open an issue if you find a bug ~
 ---
 
@@ -151,29 +136,29 @@
     serv_host = '127.0.0.1'  
     serv_port = 9478@int    # specific type is also allowed!!
     api_keys = {'TW_REGION':'SV92VS92N20', 'US_REGION':'W92N8WN029N2'}
     
     # define 'hierachical' arguments :
     # the 'section' is the key of accessing dict value and could be defined as follows :
     [db_setup]
-        db_host = $serv_host
+        db_host = ${cfg.serv_host}:80@str
         # first `export mongo_port=5566` in your bash, then support os.env interpolation!
-        db_port = $Env.mongo_port  
+        db_port = ${env.mongo_port}  
         snap_shot = True
     
     # and then define second section for backend server..
     [bknd_srv]
         load_8bit = True
         async_req = True
         chat_mode = 'inference'
         model_type = 'LlaMa2.0'
         [bknd_srv.mod_params]
             log_hist = False
             tempeture = 1e-4
-            model_mode = $bknd_srv.chat_mode  # hierachical args interpolation
+            model_mode = ${cfg.bknd_srv.chat_mode}  # hierachical args interpolation
     
 <br>
 
 Now, we're free to launch the chatbot via `python quick_start.py` (*quick_start.py in work directory*)!
 However, you can also override the arguemnts via commendline `python quick_start.py serv_port=7894`
     
     import sys
@@ -223,23 +208,23 @@
 ### More detail tutorial about each topic is as follows :
 
 #### **2. How to declare hierachical config**
 There have two kind of way to prepare the arguments in easy-config : we can either define flatten argument or groupping the multiple arguments in an hierachical manner (begin from second level). In most of time, we define the flatten argument as global setup, and arrange the rest of arguments into the corresponding dictionary for easy to assign it to the subroutine.  
 
 #### Let's give a deep-learning example ~
 #### *hier_cfg.ini in work directory*
-
+    root_dir = '/workspace'
     glb_seed = 42
     exp_id = '0001'
 
     # we call '...' in [...] as section name,
     # i.e. we can assign dict dataset to subroutine by `build_dataset(**cfg.dataset)`, just such easy!!
     [dataset]   
         service_port = 65536
-        path = '/data/kitti'
+        path = "${cfg.root_dir}/data/kitti"
         # of course, nested dict is also supported! it just the native python dictionary in dictionary!
         [dataset.loader]
             batch_size = 32
 
     [model]
         [model.backbone]
             mod_typ = 'resnet'
@@ -277,40 +262,44 @@
         mod = build_model(**cfger.model)
         ... # get torch Trainer
         Trainer(mod).fit(ds)
 
 However, the syntax of above config file could be improved, isn't it !? For example, the batch_size is defined twice under `dataset.loader` and `train_cfg`, so as layer seed. Moreover, path is defined as python string, it need to be further converted by Path object in python standard package. Could we regist our customized data type for easy-config ?
 #### Glade to say : Yes! it's possible to elegantly deal with above mentioned issue. We can solve the first issue by using argument interpolation, and solve the second issue by using the customized register!!
 
-#### *config interpolation with $ symbol* and  *customized register method `regist_cnvtor`*
-> Currently we support interpolation mechnaism to interpolate **ANY** arguemnts belong the different level of nested dictionary. Moreover, we also support **$Env** for accessing enviroment variables exported in bash!!
+#### Thanks to *python format-string via ${...}* and  *customized register method `regist_cnvtor`*. **See below example**
+> Currently we support interpolation mechnaism to interpolate *ANY* arguemnts belong the different level of nested dictionary by using **\${cfg}**. Moreover, we also support **\${env}** for accessing enviroment variables exported in bash!!
 
     # For convience, we define string-config!
     def get_str_cfg():
         ''' # `export glb_seed=42` in bash!!
-            glb_seed = $Env.glb_seed
+            glb_seed = ${env.glb_seed}
             exp_id = '0001'
 
             [dataset]   
                 service_port = 65536
 
                 # Don't forgot to regist Path object first and the typename will be the given name!!
                 path = {'path':'/data/kitti'}@pyPath
                 
                 [dataset.loader]
                     batch_size = 32
+                    secrete_seed = 55688
 
             [model]
                 [model.backbone]
                     mod_typ = 'resnet'
                     [model.backbone.optimizer]
-                        lay_seed = $glb_seed
+                        # aweason! but we can do more crazy stuff ~
+                        lay_seed = ${cfg.glb_seed}
+                        # 'cfg' is used to access the config, feel free to access any arguments defined previsouly!!
+                        string_seed = "The secrete string in data loader is ${cfg.dataset.loader.secrete_seed}!!"
             
             [train_cfg]
-                batch_size = $dataset.loader.batch_size
+                batch_size = ${cfg.dataset.loader.batch_size}
                 [train_cfg.opt]
                     opt_typ = 'Adam'
                     lr = 1e-4
                     sched = 'cos_anneal'
         '''
 
     # main_block 
@@ -397,15 +386,15 @@
         batch_size = 32@int
     
     # ./root/config/model_config.ini
     [model.backbone]
         mod_typ = 'resnet'
         [model.backbone.optimizer]
         # and yes, interpolation is still valid "after" the reference argument is declared!
-            lay_seed = $glb_seed  
+            lay_seed = ${cfg.glb_seed}
 
 
 #### **6. Config Operation**
 Config operation is one of the core technique for dynamic configuration system!!
 In the following example, you can see that the merging config system already provided a impressive hierachical merging funtionality! 
 
 > For example, `ghyu.opop.add` in cfg_a can be replaced by the cfg_b in **same** section with the same variable name, while the different namespace keep their variable safely ~ so the value of `ghyu.opop.add` will be 67 and `ghyu.opop.tueo.inpo` refer the flatten variable `inpo` and the value will be 46.
@@ -421,15 +410,15 @@
             [test.ggap]
                 gtgt = haha@str
 
         [ghyu]
             [ghyu.opop]
                 add = 32@int
                 [ghyu.opop.tueo]
-                    salt = $inpo
+                    salt = ${cfg.inpo}
 
         # Cell cfg written by Josef-Huang..
         '''
 
     def build_cfg_text_b():
         return '''
         # Initial config file :
@@ -564,8 +553,8 @@
 MIT License. More information of each term, please see LICENSE.md
 
 ### Author 
 Josef-Huang, a3285556aa@gmail.com 
 
 ### Footer
 ~ Hope God bless everyone in the world to know his word ~ <br>
-**The fear of the LORD is the beginning of knowledge; fools despise wisdom and instruction. by Proverbs 1:7**
+**The fear of the LORD is the beginning of knowledge; fools despise wisdom and instruction. by Proverbs 1:7**
```

### Comparing `easy_configer-2.3.2/README.md` & `easy_configer-2.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,25 @@
+Metadata-Version: 2.1
+Name: easy_configer
+Version: 2.5.0
+Summary: An easy way for configurating python program by the given config file or config str
+Home-page: https://github.com/HuangChiEn/easy_config
+Author: JosefHuang
+Author-email: a3285556aa@gmail.com
+License: MIT
+Keywords: configuration,commendline argument,argument
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 # Project description
-#### easy_configer version : 2.3.2
+#### easy_configer version : 2.5.0
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
 ![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
@@ -53,21 +69,22 @@
 
 * support arguments interpolation!!
 
 * support config conversion, which turn easy_config into the other kind of config package (omegaconf, argparse, ..., etc.)
 
 * support hierachical configurating system with dynamic override ~
 
+* better support for argument intepolation (inline-intepolation is allowed now ~)
+
 ---
 
 ### Newly update features 🚀
-1. Enable all test case (automatically ci by git-action)
-2. Support dot-access of any arguments
-3. Consistent import syntax.. 
-4. New document is released ~
+1. Single-line python code execution via ${...} in config file
+2. Integrate argument intepolation via ${cfg} with special object
+3. Integrate enviroment variable intepolation via ${env} with special object
 
 ---
 
 ### Bug Fixed 🐛
 #### Fix-up import syntax.. plz open an issue if you find a bug ~
 ---
 
@@ -135,29 +152,29 @@
     serv_host = '127.0.0.1'  
     serv_port = 9478@int    # specific type is also allowed!!
     api_keys = {'TW_REGION':'SV92VS92N20', 'US_REGION':'W92N8WN029N2'}
     
     # define 'hierachical' arguments :
     # the 'section' is the key of accessing dict value and could be defined as follows :
     [db_setup]
-        db_host = $serv_host
+        db_host = ${cfg.serv_host}:80@str
         # first `export mongo_port=5566` in your bash, then support os.env interpolation!
-        db_port = $Env.mongo_port  
+        db_port = ${env.mongo_port}  
         snap_shot = True
     
     # and then define second section for backend server..
     [bknd_srv]
         load_8bit = True
         async_req = True
         chat_mode = 'inference'
         model_type = 'LlaMa2.0'
         [bknd_srv.mod_params]
             log_hist = False
             tempeture = 1e-4
-            model_mode = $bknd_srv.chat_mode  # hierachical args interpolation
+            model_mode = ${cfg.bknd_srv.chat_mode}  # hierachical args interpolation
     
 <br>
 
 Now, we're free to launch the chatbot via `python quick_start.py` (*quick_start.py in work directory*)!
 However, you can also override the arguemnts via commendline `python quick_start.py serv_port=7894`
     
     import sys
@@ -207,23 +224,23 @@
 ### More detail tutorial about each topic is as follows :
 
 #### **2. How to declare hierachical config**
 There have two kind of way to prepare the arguments in easy-config : we can either define flatten argument or groupping the multiple arguments in an hierachical manner (begin from second level). In most of time, we define the flatten argument as global setup, and arrange the rest of arguments into the corresponding dictionary for easy to assign it to the subroutine.  
 
 #### Let's give a deep-learning example ~
 #### *hier_cfg.ini in work directory*
-
+    root_dir = '/workspace'
     glb_seed = 42
     exp_id = '0001'
 
     # we call '...' in [...] as section name,
     # i.e. we can assign dict dataset to subroutine by `build_dataset(**cfg.dataset)`, just such easy!!
     [dataset]   
         service_port = 65536
-        path = '/data/kitti'
+        path = "${cfg.root_dir}/data/kitti"
         # of course, nested dict is also supported! it just the native python dictionary in dictionary!
         [dataset.loader]
             batch_size = 32
 
     [model]
         [model.backbone]
             mod_typ = 'resnet'
@@ -261,40 +278,44 @@
         mod = build_model(**cfger.model)
         ... # get torch Trainer
         Trainer(mod).fit(ds)
 
 However, the syntax of above config file could be improved, isn't it !? For example, the batch_size is defined twice under `dataset.loader` and `train_cfg`, so as layer seed. Moreover, path is defined as python string, it need to be further converted by Path object in python standard package. Could we regist our customized data type for easy-config ?
 #### Glade to say : Yes! it's possible to elegantly deal with above mentioned issue. We can solve the first issue by using argument interpolation, and solve the second issue by using the customized register!!
 
-#### *config interpolation with $ symbol* and  *customized register method `regist_cnvtor`*
-> Currently we support interpolation mechnaism to interpolate **ANY** arguemnts belong the different level of nested dictionary. Moreover, we also support **$Env** for accessing enviroment variables exported in bash!!
+#### Thanks to *python format-string via ${...}* and  *customized register method `regist_cnvtor`*. **See below example**
+> Currently we support interpolation mechnaism to interpolate *ANY* arguemnts belong the different level of nested dictionary by using **\${cfg}**. Moreover, we also support **\${env}** for accessing enviroment variables exported in bash!!
 
     # For convience, we define string-config!
     def get_str_cfg():
         ''' # `export glb_seed=42` in bash!!
-            glb_seed = $Env.glb_seed
+            glb_seed = ${env.glb_seed}
             exp_id = '0001'
 
             [dataset]   
                 service_port = 65536
 
                 # Don't forgot to regist Path object first and the typename will be the given name!!
                 path = {'path':'/data/kitti'}@pyPath
                 
                 [dataset.loader]
                     batch_size = 32
+                    secrete_seed = 55688
 
             [model]
                 [model.backbone]
                     mod_typ = 'resnet'
                     [model.backbone.optimizer]
-                        lay_seed = $glb_seed
+                        # aweason! but we can do more crazy stuff ~
+                        lay_seed = ${cfg.glb_seed}
+                        # 'cfg' is used to access the config, feel free to access any arguments defined previsouly!!
+                        string_seed = "The secrete string in data loader is ${cfg.dataset.loader.secrete_seed}!!"
             
             [train_cfg]
-                batch_size = $dataset.loader.batch_size
+                batch_size = ${cfg.dataset.loader.batch_size}
                 [train_cfg.opt]
                     opt_typ = 'Adam'
                     lr = 1e-4
                     sched = 'cos_anneal'
         '''
 
     # main_block 
@@ -381,15 +402,15 @@
         batch_size = 32@int
     
     # ./root/config/model_config.ini
     [model.backbone]
         mod_typ = 'resnet'
         [model.backbone.optimizer]
         # and yes, interpolation is still valid "after" the reference argument is declared!
-            lay_seed = $glb_seed  
+            lay_seed = ${cfg.glb_seed}
 
 
 #### **6. Config Operation**
 Config operation is one of the core technique for dynamic configuration system!!
 In the following example, you can see that the merging config system already provided a impressive hierachical merging funtionality! 
 
 > For example, `ghyu.opop.add` in cfg_a can be replaced by the cfg_b in **same** section with the same variable name, while the different namespace keep their variable safely ~ so the value of `ghyu.opop.add` will be 67 and `ghyu.opop.tueo.inpo` refer the flatten variable `inpo` and the value will be 46.
@@ -405,15 +426,15 @@
             [test.ggap]
                 gtgt = haha@str
 
         [ghyu]
             [ghyu.opop]
                 add = 32@int
                 [ghyu.opop.tueo]
-                    salt = $inpo
+                    salt = ${cfg.inpo}
 
         # Cell cfg written by Josef-Huang..
         '''
 
     def build_cfg_text_b():
         return '''
         # Initial config file :
@@ -548,8 +569,8 @@
 MIT License. More information of each term, please see LICENSE.md
 
 ### Author 
 Josef-Huang, a3285556aa@gmail.com 
 
 ### Footer
 ~ Hope God bless everyone in the world to know his word ~ <br>
-**The fear of the LORD is the beginning of knowledge; fools despise wisdom and instruction. by Proverbs 1:7**
+**The fear of the LORD is the beginning of knowledge; fools despise wisdom and instruction. by Proverbs 1:7**
```

### Comparing `easy_configer-2.3.2/easy_configer/Configer.py` & `easy_configer-2.5.0/easy_configer/Configer.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,26 +164,17 @@
     def __get_declr_dict(self, cfg_str:str) -> dict : 
         if self.__split_chr not in cfg_str:
             raise RuntimeError("Configuration Error : Split character '{0}'" \
                                 " not found in '{1}'".format(self.__split_chr, cfg_str))
         
         try:
             var_name, val_str = cfg_str.split(self.__split_chr)
-            # support '$' notation for hierachical args interpolation!
-            if val_str[0] == '$':
-                val_str = val_str[1:]
-                if 'ENV' in val_str:   # to be honest, i don't think we should have to resolve complex object except os.env
-                    env_key = val_str.split('.')[-1]
-                    intep_val = os.environ[env_key]
-                else:    
-                    sec_ptr, sec_key = self.__idx_sec_by_dot(val_str)
-                    intep_val = sec_ptr[sec_key]
-                var_val = intep_val
-            else:
-                var_val = self.__typ_cnvt.convert(val_str)
+            # we support '${...}' for "single-line python code execution" in Type_Convertor, 
+            #   then, we can use it to build "config-resolve", "hierachical args interpolation"!!
+            var_val = self.__typ_cnvt.convert(val_str, self)
         except:
             raise RuntimeError("Configuration Error : Invalid config string ' {0}' ".format(cfg_str))
 
         return { var_name : var_val }
 
     # core function of config parser
     def __cfg_parser(self, raw_cfg_text:str):
@@ -231,14 +222,15 @@
 
                 # assign the val_dict into the corresponding section!
                 if cur_sec_keys != '':
                     idx_sec, idx_sec_key = self.__idx_sec_by_dot(cur_sec_keys)
                     idx_sec[idx_sec_key].update( val_dict )
                 # assign the val_dict as 'flatten' arguments 
                 else: # Note that flatten args IS NOT AttributeDict!
+                    
                     self.__dict__.update( val_dict )
                     
         # Update the namespace value via commend-line input 
         if self.__cmd_args:
             self.args_from_cmd()
 
     def args_from_cmd(self):
```

### Comparing `easy_configer-2.3.2/easy_configer/IO_Converter.py` & `easy_configer-2.5.0/easy_configer/IO_Converter.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.3.2/easy_configer/utils/Container.py` & `easy_configer-2.5.0/easy_configer/utils/Container.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.3.2/easy_configer.egg-info/PKG-INFO` & `easy_configer-2.5.0/easy_configer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: easy-configer
-Version: 2.3.2
+Version: 2.5.0
 Summary: An easy way for configurating python program by the given config file or config str
 Home-page: https://github.com/HuangChiEn/easy_config
 Author: JosefHuang
 Author-email: a3285556aa@gmail.com
 License: MIT
 Keywords: configuration,commendline argument,argument
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Project description
-#### easy_configer version : 2.3.2
+#### easy_configer version : 2.5.0
 ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/HuangChiEn/easy_config/main.yaml?branch=master&event=push&style=for-the-badge&label=unittest&color=green)
 
 ![easy-configer logo](https://raw.githubusercontent.com/HuangChiEn/easy_config/master/assets/logo.png)
 
 ---
 
 ### Configeruating the program in an easy-way 
@@ -69,21 +69,22 @@
 
 * support arguments interpolation!!
 
 * support config conversion, which turn easy_config into the other kind of config package (omegaconf, argparse, ..., etc.)
 
 * support hierachical configurating system with dynamic override ~
 
+* better support for argument intepolation (inline-intepolation is allowed now ~)
+
 ---
 
 ### Newly update features 🚀
-1. Enable all test case (automatically ci by git-action)
-2. Support dot-access of any arguments
-3. Consistent import syntax.. 
-4. New document is released ~
+1. Single-line python code execution via ${...} in config file
+2. Integrate argument intepolation via ${cfg} with special object
+3. Integrate enviroment variable intepolation via ${env} with special object
 
 ---
 
 ### Bug Fixed 🐛
 #### Fix-up import syntax.. plz open an issue if you find a bug ~
 ---
 
@@ -151,29 +152,29 @@
     serv_host = '127.0.0.1'  
     serv_port = 9478@int    # specific type is also allowed!!
     api_keys = {'TW_REGION':'SV92VS92N20', 'US_REGION':'W92N8WN029N2'}
     
     # define 'hierachical' arguments :
     # the 'section' is the key of accessing dict value and could be defined as follows :
     [db_setup]
-        db_host = $serv_host
+        db_host = ${cfg.serv_host}:80@str
         # first `export mongo_port=5566` in your bash, then support os.env interpolation!
-        db_port = $Env.mongo_port  
+        db_port = ${env.mongo_port}  
         snap_shot = True
     
     # and then define second section for backend server..
     [bknd_srv]
         load_8bit = True
         async_req = True
         chat_mode = 'inference'
         model_type = 'LlaMa2.0'
         [bknd_srv.mod_params]
             log_hist = False
             tempeture = 1e-4
-            model_mode = $bknd_srv.chat_mode  # hierachical args interpolation
+            model_mode = ${cfg.bknd_srv.chat_mode}  # hierachical args interpolation
     
 <br>
 
 Now, we're free to launch the chatbot via `python quick_start.py` (*quick_start.py in work directory*)!
 However, you can also override the arguemnts via commendline `python quick_start.py serv_port=7894`
     
     import sys
@@ -223,23 +224,23 @@
 ### More detail tutorial about each topic is as follows :
 
 #### **2. How to declare hierachical config**
 There have two kind of way to prepare the arguments in easy-config : we can either define flatten argument or groupping the multiple arguments in an hierachical manner (begin from second level). In most of time, we define the flatten argument as global setup, and arrange the rest of arguments into the corresponding dictionary for easy to assign it to the subroutine.  
 
 #### Let's give a deep-learning example ~
 #### *hier_cfg.ini in work directory*
-
+    root_dir = '/workspace'
     glb_seed = 42
     exp_id = '0001'
 
     # we call '...' in [...] as section name,
     # i.e. we can assign dict dataset to subroutine by `build_dataset(**cfg.dataset)`, just such easy!!
     [dataset]   
         service_port = 65536
-        path = '/data/kitti'
+        path = "${cfg.root_dir}/data/kitti"
         # of course, nested dict is also supported! it just the native python dictionary in dictionary!
         [dataset.loader]
             batch_size = 32
 
     [model]
         [model.backbone]
             mod_typ = 'resnet'
@@ -277,40 +278,44 @@
         mod = build_model(**cfger.model)
         ... # get torch Trainer
         Trainer(mod).fit(ds)
 
 However, the syntax of above config file could be improved, isn't it !? For example, the batch_size is defined twice under `dataset.loader` and `train_cfg`, so as layer seed. Moreover, path is defined as python string, it need to be further converted by Path object in python standard package. Could we regist our customized data type for easy-config ?
 #### Glade to say : Yes! it's possible to elegantly deal with above mentioned issue. We can solve the first issue by using argument interpolation, and solve the second issue by using the customized register!!
 
-#### *config interpolation with $ symbol* and  *customized register method `regist_cnvtor`*
-> Currently we support interpolation mechnaism to interpolate **ANY** arguemnts belong the different level of nested dictionary. Moreover, we also support **$Env** for accessing enviroment variables exported in bash!!
+#### Thanks to *python format-string via ${...}* and  *customized register method `regist_cnvtor`*. **See below example**
+> Currently we support interpolation mechnaism to interpolate *ANY* arguemnts belong the different level of nested dictionary by using **\${cfg}**. Moreover, we also support **\${env}** for accessing enviroment variables exported in bash!!
 
     # For convience, we define string-config!
     def get_str_cfg():
         ''' # `export glb_seed=42` in bash!!
-            glb_seed = $Env.glb_seed
+            glb_seed = ${env.glb_seed}
             exp_id = '0001'
 
             [dataset]   
                 service_port = 65536
 
                 # Don't forgot to regist Path object first and the typename will be the given name!!
                 path = {'path':'/data/kitti'}@pyPath
                 
                 [dataset.loader]
                     batch_size = 32
+                    secrete_seed = 55688
 
             [model]
                 [model.backbone]
                     mod_typ = 'resnet'
                     [model.backbone.optimizer]
-                        lay_seed = $glb_seed
+                        # aweason! but we can do more crazy stuff ~
+                        lay_seed = ${cfg.glb_seed}
+                        # 'cfg' is used to access the config, feel free to access any arguments defined previsouly!!
+                        string_seed = "The secrete string in data loader is ${cfg.dataset.loader.secrete_seed}!!"
             
             [train_cfg]
-                batch_size = $dataset.loader.batch_size
+                batch_size = ${cfg.dataset.loader.batch_size}
                 [train_cfg.opt]
                     opt_typ = 'Adam'
                     lr = 1e-4
                     sched = 'cos_anneal'
         '''
 
     # main_block 
@@ -397,15 +402,15 @@
         batch_size = 32@int
     
     # ./root/config/model_config.ini
     [model.backbone]
         mod_typ = 'resnet'
         [model.backbone.optimizer]
         # and yes, interpolation is still valid "after" the reference argument is declared!
-            lay_seed = $glb_seed  
+            lay_seed = ${cfg.glb_seed}
 
 
 #### **6. Config Operation**
 Config operation is one of the core technique for dynamic configuration system!!
 In the following example, you can see that the merging config system already provided a impressive hierachical merging funtionality! 
 
 > For example, `ghyu.opop.add` in cfg_a can be replaced by the cfg_b in **same** section with the same variable name, while the different namespace keep their variable safely ~ so the value of `ghyu.opop.add` will be 67 and `ghyu.opop.tueo.inpo` refer the flatten variable `inpo` and the value will be 46.
@@ -421,15 +426,15 @@
             [test.ggap]
                 gtgt = haha@str
 
         [ghyu]
             [ghyu.opop]
                 add = 32@int
                 [ghyu.opop.tueo]
-                    salt = $inpo
+                    salt = ${cfg.inpo}
 
         # Cell cfg written by Josef-Huang..
         '''
 
     def build_cfg_text_b():
         return '''
         # Initial config file :
```

### Comparing `easy_configer-2.3.2/setup.py` & `easy_configer-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # read the contents of your README file
 this_directory = abspath(dirname(__file__))
 with open(join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='easy_configer',
-    version='2.3.2',
+    version='2.5.0',
     description='An easy way for configurating python program by the given config file or config str',
     author='JosefHuang',
     author_email='a3285556aa@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/HuangChiEn/easy_config',
```

