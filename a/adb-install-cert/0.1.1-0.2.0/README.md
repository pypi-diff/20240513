# Comparing `tmp/adb_install_cert-0.1.1.tar.gz` & `tmp/adb_install_cert-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb_install_cert-0.1.1.tar", max compression
+gzip compressed data, was "adb_install_cert-0.2.0.tar", max compression
```

## Comparing `adb_install_cert-0.1.1.tar` & `adb_install_cert-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1054 2024-05-10 07:45:48.050958 adb_install_cert-0.1.1/LICENSE
--rw-r--r--   0        0        0     3057 2024-05-10 11:02:20.841570 adb_install_cert-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-10 06:21:42.189085 adb_install_cert-0.1.1/adb_install_cert/__init__.py
--rw-r--r--   0        0        0     5396 2024-05-10 12:56:26.434622 adb_install_cert-0.1.1/adb_install_cert/__main__.py
--rw-r--r--   0        0        0     3471 2024-05-10 12:52:20.975812 adb_install_cert-0.1.1/adb_install_cert/utils.py
--rw-r--r--   0        0        0      507 2024-05-10 12:58:57.314319 adb_install_cert-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3640 1970-01-01 00:00:00.000000 adb_install_cert-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2024-05-10 07:45:48.050958 adb_install_cert-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3616 2024-05-13 11:24:38.906625 adb_install_cert-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 06:21:42.189085 adb_install_cert-0.2.0/adb_install_cert/__init__.py
+-rw-r--r--   0        0        0     8340 2024-05-13 12:03:02.999234 adb_install_cert-0.2.0/adb_install_cert/__main__.py
+-rw-r--r--   0        0        0     3973 2024-05-13 12:10:58.755376 adb_install_cert-0.2.0/adb_install_cert/utils.py
+-rw-r--r--   0        0        0      507 2024-05-13 09:31:00.709058 adb_install_cert-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4199 1970-01-01 00:00:00.000000 adb_install_cert-0.2.0/PKG-INFO
```

### Comparing `adb_install_cert-0.1.1/LICENSE` & `adb_install_cert-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adb_install_cert-0.1.1/README.md` & `adb_install_cert-0.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,99 +1,112 @@
 # adb-install-cert (root required)
 
 This script automatically detect android version and choose preffered way to install certificate to system store.
 
+If you want manually install certificate (or just want to explore, how to do that) see [my guide](./guide/README.md)
+
 ## Quick start
 
 Change path to pem certificate and run:
 
 ```sh
 nix --extra-experimental-features "nix-command flakes" run "github:sysraccoon/adb-install-cert" -- --pem-cert ~/path/to/cert.pem
 ```
 
-## PyPi installation
+## pip installation
 
 ```sh
-pip install adb-install-cert
+pip3 install adb-install-cert
 ```
 
 ## NixOS flake installation
 
-```
+```nix
 # flake.nix
 
 {
     nixpkgs.url = "github:nixos/nixpkgs?ref=nixos-unstable";
     inputs.adb-install-cert.url = "github:sysraccoon/adb-install-cert";
     # ...
 
-    outputs = { self, nixpkgs, ... } @ inputs {
+    outputs = { self, nixpkgs, adb-install-cert, ... } {
         nixosConfigurations.HOSTNAME = nixpkgs.lib.nixosSystem rec {
             system = "x86_64-linux";
             specialArgs = { inherit self system; };
             modules = [
                 {
                     environment.systemPackages = [
-                        self.inputs.adb-install-cert.packages.${system}.adb-install-cert;
+                        adb-install-cert.packages.${system}.adb-install-cert;
                     ];
                 }
             ];
         };
     };
 }
 ```
 
 ## Home-Manager flake installation
 
-```
+```nix
 # flake.nix
 {   
     nixpkgs.url = "github:nixos/nixpkgs?ref=nixos-unstable";
     home-manager = {
       url = "github:nix-community/home-manager";
       inputs.nixpkgs.follows = "nixpkgs";
     };
     inputs.adb-install-cert.url = "github:sysraccoon/adb-install-cert";
     # ...
 
-    outputs = { self, nixpkgs, ... } @ inputs {
+    outputs = { self, nixpkgs, adb-install-cert, ... } {
         homeConfigurations.USERNAME = home-manager.lib.homeManagerConfiguration rec {
             system = "x86_64-linux";
             specialArgs = { inherit self system; };
             modules = [
                 {
                     home.packages = [
-                        self.inputs.adb-install-cert.packages.${system}.adb-install-cert;
+                        adb-install-cert.packages.${system}.adb-install-cert;
                     ];
                 }
             ];
         };
     };
 }
 
 ```
 
 ## Usage
 
 After installation, you can plug your device and run:
 
+```sh
+$ adb-install-cert --cert ~/path/to/cert.pem
+```
+
+If certificate format detect incorrectly, pass it directly (only `der` and `pem` support):
+```sh
+$ adb-install-cert --cert ~/path/to/cert.crt --cert-format der
+```
+
+By default `adb-install-cert` automatically select installation mode, based on android version.
+If you want override it, pass `--mode` option (see `--help` or read technical description below for more information):
 ```
-$ adb-install-cert --pem-cert ~/path/to/cert.pem
+$ adb-install-cert --cert ~/path/to/cert.pem --mode temporary
 ```
 
 If multiple devices present, you can specify one by serial:
 
 ```
-$ adb-install-cert --pem-cert ~/path/to/cert.pem --device-serial some-serial
+$ adb-install-cert --cert ~/path/to/cert.pem --device-serial some-serial
 ```
 
 As alternative, you can use environment variables, as described [here](https://github.com/openatx/adbutils?tab=readme-ov-file#environment):
 
 ```
-$ ANDROID_SERIAL=emulator-5556 adb-install-cert --pem-cert ~/path/to/cert.pem
+$ ANDROID_SERIAL=emulator-5556 adb-install-cert --cert ~/path/to/cert.pem
 ```
 
 ## Technical Description
 
 **Before Android 10**, **permanent installation** of a certificate is possible by remounting the root directory in read-write mode. These changes may require a device reboot.
 
 **Starting with Android 10**, the root system is available in read-only mode. To install a certificate, the utility uses remounting `/system/etc/security/cacerts` directory in `tmpfs` with a preliminary copy of all existing certificates. **After a reboot, the changes will be reset and the utility will need to be reused**.
```

### Comparing `adb_install_cert-0.1.1/PKG-INFO` & `adb_install_cert-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-install-cert
-Version: 0.1.1
+Version: 0.2.0
 Summary: Install certificates to android system store
 License: MIT
 Author: sysraccoon
 Author-email: sysraccoon@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,102 +15,115 @@
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Description-Content-Type: text/markdown
 
 # adb-install-cert (root required)
 
 This script automatically detect android version and choose preffered way to install certificate to system store.
 
+If you want manually install certificate (or just want to explore, how to do that) see [my guide](./guide/README.md)
+
 ## Quick start
 
 Change path to pem certificate and run:
 
 ```sh
 nix --extra-experimental-features "nix-command flakes" run "github:sysraccoon/adb-install-cert" -- --pem-cert ~/path/to/cert.pem
 ```
 
-## PyPi installation
+## pip installation
 
 ```sh
-pip install adb-install-cert
+pip3 install adb-install-cert
 ```
 
 ## NixOS flake installation
 
-```
+```nix
 # flake.nix
 
 {
     nixpkgs.url = "github:nixos/nixpkgs?ref=nixos-unstable";
     inputs.adb-install-cert.url = "github:sysraccoon/adb-install-cert";
     # ...
 
-    outputs = { self, nixpkgs, ... } @ inputs {
+    outputs = { self, nixpkgs, adb-install-cert, ... } {
         nixosConfigurations.HOSTNAME = nixpkgs.lib.nixosSystem rec {
             system = "x86_64-linux";
             specialArgs = { inherit self system; };
             modules = [
                 {
                     environment.systemPackages = [
-                        self.inputs.adb-install-cert.packages.${system}.adb-install-cert;
+                        adb-install-cert.packages.${system}.adb-install-cert;
                     ];
                 }
             ];
         };
     };
 }
 ```
 
 ## Home-Manager flake installation
 
-```
+```nix
 # flake.nix
 {   
     nixpkgs.url = "github:nixos/nixpkgs?ref=nixos-unstable";
     home-manager = {
       url = "github:nix-community/home-manager";
       inputs.nixpkgs.follows = "nixpkgs";
     };
     inputs.adb-install-cert.url = "github:sysraccoon/adb-install-cert";
     # ...
 
-    outputs = { self, nixpkgs, ... } @ inputs {
+    outputs = { self, nixpkgs, adb-install-cert, ... } {
         homeConfigurations.USERNAME = home-manager.lib.homeManagerConfiguration rec {
             system = "x86_64-linux";
             specialArgs = { inherit self system; };
             modules = [
                 {
                     home.packages = [
-                        self.inputs.adb-install-cert.packages.${system}.adb-install-cert;
+                        adb-install-cert.packages.${system}.adb-install-cert;
                     ];
                 }
             ];
         };
     };
 }
 
 ```
 
 ## Usage
 
 After installation, you can plug your device and run:
 
+```sh
+$ adb-install-cert --cert ~/path/to/cert.pem
+```
+
+If certificate format detect incorrectly, pass it directly (only `der` and `pem` support):
+```sh
+$ adb-install-cert --cert ~/path/to/cert.crt --cert-format der
+```
+
+By default `adb-install-cert` automatically select installation mode, based on android version.
+If you want override it, pass `--mode` option (see `--help` or read technical description below for more information):
 ```
-$ adb-install-cert --pem-cert ~/path/to/cert.pem
+$ adb-install-cert --cert ~/path/to/cert.pem --mode temporary
 ```
 
 If multiple devices present, you can specify one by serial:
 
 ```
-$ adb-install-cert --pem-cert ~/path/to/cert.pem --device-serial some-serial
+$ adb-install-cert --cert ~/path/to/cert.pem --device-serial some-serial
 ```
 
 As alternative, you can use environment variables, as described [here](https://github.com/openatx/adbutils?tab=readme-ov-file#environment):
 
 ```
-$ ANDROID_SERIAL=emulator-5556 adb-install-cert --pem-cert ~/path/to/cert.pem
+$ ANDROID_SERIAL=emulator-5556 adb-install-cert --cert ~/path/to/cert.pem
 ```
 
 ## Technical Description
 
 **Before Android 10**, **permanent installation** of a certificate is possible by remounting the root directory in read-write mode. These changes may require a device reboot.
 
 **Starting with Android 10**, the root system is available in read-only mode. To install a certificate, the utility uses remounting `/system/etc/security/cacerts` directory in `tmpfs` with a preliminary copy of all existing certificates. **After a reboot, the changes will be reset and the utility will need to be reused**.
```

