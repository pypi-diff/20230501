# Comparing `tmp/akinator.py-0.2.3.tar.gz` & `tmp/akinator.py-0.2.4.tar.gz`

## Comparing `akinator.py-0.2.3.tar` & `akinator.py-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 akinator.py-0.2.3/Cargo.toml
--rw-r--r--   0     1001      123     4639 2023-04-15 22:17:44.000000 akinator.py-0.2.3/.github/workflows/ci.yml
--rw-r--r--   0     1001      123       88 2023-04-15 22:17:44.000000 akinator.py-0.2.3/.gitignore
--rw-r--r--   0     1001      123      213 2023-04-15 22:17:44.000000 akinator.py-0.2.3/.readthedocs.yml
--rw-r--r--   0     1001      123      190 2023-04-15 22:17:44.000000 akinator.py-0.2.3/.vscode/settings.json
--rw-r--r--   0     1001      123     1076 2023-04-15 22:17:44.000000 akinator.py-0.2.3/LICENSE
--rw-r--r--   0     1001      123      695 2023-04-15 22:17:44.000000 akinator.py-0.2.3/README.md
--rw-r--r--   0     1001      123     4220 2023-04-15 22:17:44.000000 akinator.py-0.2.3/akinator.pyi
--rw-r--r--   0     1001      123      146 2023-04-15 22:17:44.000000 akinator.py-0.2.3/docs/akinator.rst
--rw-r--r--   0     1001      123     2498 2023-04-15 22:17:44.000000 akinator.py-0.2.3/docs/conf.py
--rw-r--r--   0     1001      123     4170 2023-04-15 22:17:44.000000 akinator.py-0.2.3/docs/examples.rst
--rw-r--r--   0     1001      123      475 2023-04-15 22:17:44.000000 akinator.py-0.2.3/docs/index.rst
--rw-r--r--   0     1001      123      591 2023-04-15 22:17:44.000000 akinator.py-0.2.3/pyproject.toml
--rw-r--r--   0     1001      123    10034 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/async_akinator.rs
--rw-r--r--   0     1001      123     8646 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/blocking_akinator.rs
--rw-r--r--   0     1001      123     6575 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/enums.rs
--rw-r--r--   0     1001      123     3947 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/error.rs
--rw-r--r--   0     1001      123     1044 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/lib.rs
--rw-r--r--   0     1001      123     1996 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/models.rs
--rw-r--r--   0     1001      123     1612 2023-04-15 22:17:44.000000 akinator.py-0.2.3/tests/test_async.py
--rw-r--r--   0     1001      123     1543 2023-04-15 22:17:44.000000 akinator.py-0.2.3/tests/test_sync.py
--rw-r--r--   0     1001      123       10 2023-04-15 22:18:07.000000 akinator.py-0.2.3/wheelhouse/akinator.py-0.2.3.tar.gz
--rw-r--r--   0     1001      123    29149 2023-04-15 22:18:05.000000 akinator.py-0.2.3/Cargo.lock
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 akinator.py-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 akinator.py-0.2.4/Cargo.toml
+-rw-r--r--   0     1001      123     4639 2023-05-01 02:15:08.000000 akinator.py-0.2.4/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123       88 2023-05-01 02:15:08.000000 akinator.py-0.2.4/.gitignore
+-rw-r--r--   0     1001      123      213 2023-05-01 02:15:08.000000 akinator.py-0.2.4/.readthedocs.yml
+-rw-r--r--   0     1001      123      190 2023-05-01 02:15:08.000000 akinator.py-0.2.4/.vscode/settings.json
+-rw-r--r--   0     1001      123     1076 2023-05-01 02:15:08.000000 akinator.py-0.2.4/LICENSE
+-rw-r--r--   0     1001      123      695 2023-05-01 02:15:08.000000 akinator.py-0.2.4/README.md
+-rw-r--r--   0     1001      123     4220 2023-05-01 02:15:08.000000 akinator.py-0.2.4/akinator.pyi
+-rw-r--r--   0     1001      123      146 2023-05-01 02:15:08.000000 akinator.py-0.2.4/docs/akinator.rst
+-rw-r--r--   0     1001      123     2498 2023-05-01 02:15:08.000000 akinator.py-0.2.4/docs/conf.py
+-rw-r--r--   0     1001      123     4170 2023-05-01 02:15:08.000000 akinator.py-0.2.4/docs/examples.rst
+-rw-r--r--   0     1001      123      475 2023-05-01 02:15:08.000000 akinator.py-0.2.4/docs/index.rst
+-rw-r--r--   0     1001      123      591 2023-05-01 02:15:08.000000 akinator.py-0.2.4/pyproject.toml
+-rw-r--r--   0     1001      123    10090 2023-05-01 02:15:08.000000 akinator.py-0.2.4/src/async_akinator.rs
+-rw-r--r--   0     1001      123     8702 2023-05-01 02:15:08.000000 akinator.py-0.2.4/src/blocking_akinator.rs
+-rw-r--r--   0     1001      123     6575 2023-05-01 02:15:08.000000 akinator.py-0.2.4/src/enums.rs
+-rw-r--r--   0     1001      123     3947 2023-05-01 02:15:08.000000 akinator.py-0.2.4/src/error.rs
+-rw-r--r--   0     1001      123     1044 2023-05-01 02:15:08.000000 akinator.py-0.2.4/src/lib.rs
+-rw-r--r--   0     1001      123     1996 2023-05-01 02:15:08.000000 akinator.py-0.2.4/src/models.rs
+-rw-r--r--   0     1001      123     1612 2023-05-01 02:15:08.000000 akinator.py-0.2.4/tests/test_async.py
+-rw-r--r--   0     1001      123     1543 2023-05-01 02:15:08.000000 akinator.py-0.2.4/tests/test_sync.py
+-rw-r--r--   0     1001      123       10 2023-05-01 02:15:36.000000 akinator.py-0.2.4/wheelhouse/akinator.py-0.2.4.tar.gz
+-rw-r--r--   0     1001      123    31334 2023-05-01 02:15:34.000000 akinator.py-0.2.4/Cargo.lock
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 akinator.py-0.2.4/PKG-INFO
```

### Comparing `akinator.py-0.2.3/Cargo.toml` & `akinator.py-0.2.4/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "akinator-py"
 authors = ["Tom-the-Bomb"]
-version = "0.2.3"
+version = "0.2.4"
 edition = "2021"
 license = "MIT"
 readme = "README.md"
 description = "Python bindings for akinator-rs"
 documentation = "https://akinatorpy.readthedocs.io/en/latest/"
 repository = "https://github.com/Tom-the-Bomb/akinator.py"
 homepage = "https://github.com/Tom-the-Bomb/akinator.py"
```

### Comparing `akinator.py-0.2.3/.github/workflows/ci.yml` & `akinator.py-0.2.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/LICENSE` & `akinator.py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/README.md` & `akinator.py-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/akinator.pyi` & `akinator.py-0.2.4/akinator.pyi`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/docs/conf.py` & `akinator.py-0.2.4/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'akinator.py'
 copyright = '2022, Tom-the-Bomb'
 author = 'Tom-the-Bomb'
 
 # The full version, including alpha/beta/rc tags
-release = '0.2.3'
+release = '0.2.4'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `akinator.py-0.2.3/docs/examples.rst` & `akinator.py-0.2.4/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/pyproject.toml` & `akinator.py-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "akinator.py"
 author = "Tom-the-Bomb"
-version = "0.2.3"
+version = "0.2.4"
 license = { file = "LICENSE" }
 description = "Python bindings for akinator-rs"
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.urls]
 documentation = "https://akinatorpy.readthedocs.io/en/latest/"
```

### Comparing `akinator.py-0.2.3/src/async_akinator.rs` & `akinator.py-0.2.4/src/async_akinator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -50,33 +50,34 @@
 impl AsyncAkinator {
     #[new]
     #[args("*", theme, language, child_mode)]
     fn constructor(
         theme: Option<Theme>,
         language: Option<Language>,
         child_mode: Option<bool>,
-    ) -> Self {
+    ) -> PyResult<Self> {
         let mut akinator =
-            AkinatorStruct::new();
+            AkinatorStruct::new()
+            .map_err(|e| Error::from(e))?;
 
         if let Some(theme) = theme {
             akinator = akinator.with_theme(theme.into());
         }
 
         if let Some(language) = language {
             akinator = akinator.with_language(language.into());
         }
 
         if child_mode.unwrap_or(false) {
             akinator = akinator.with_child_mode();
         }
 
-        Self(
+        Ok(Self(
             Arc::new(RwLock::new(akinator))
-        )
+        ))
     }
 
     fn __repr__(&self) -> String {
         format!(
             "<AsyncAkinator theme=\"{:?}\" language=\"{:?}\" child_mode={}>",
             self.theme(),
             self.language(),
```

### Comparing `akinator.py-0.2.3/src/blocking_akinator.rs` & `akinator.py-0.2.4/src/blocking_akinator.rs`

 * *Files 0% similar despite different names*

```diff
@@ -45,31 +45,32 @@
 impl Akinator {
     #[new]
     #[args("*", theme, language, child_mode)]
     fn constructor(
         theme: Option<Theme>,
         language: Option<Language>,
         child_mode: Option<bool>,
-    ) -> Self {
+    ) -> PyResult<Self> {
         let mut akinator =
-            AkinatorStruct::new();
+            AkinatorStruct::new()
+            .map_err(|e| Error::from(e))?;
 
         if let Some(theme) = theme {
             akinator = akinator.with_theme(theme.into());
         }
 
         if let Some(language) = language {
             akinator = akinator.with_language(language.into());
         }
 
         if child_mode.unwrap_or(false) {
             akinator = akinator.with_child_mode();
         }
 
-        Self(akinator)
+        Ok(Self(akinator))
     }
 
     fn __repr__(&self) -> String {
         format!(
             "<Akinator theme=\"{:?}\" language=\"{:?}\" child_mode={}>",
             self.theme(),
             self.language(),
```

### Comparing `akinator.py-0.2.3/src/enums.rs` & `akinator.py-0.2.4/src/enums.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/src/error.rs` & `akinator.py-0.2.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/src/lib.rs` & `akinator.py-0.2.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/src/models.rs` & `akinator.py-0.2.4/src/models.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/tests/test_async.py` & `akinator.py-0.2.4/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/tests/test_sync.py` & `akinator.py-0.2.4/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.3/Cargo.lock` & `akinator.py-0.2.4/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "akinator-py"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "akinator-rs",
  "lazy_static",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
 ]
 
 [[package]]
 name = "akinator-rs"
-version = "0.1.10"
-source = "git+https://github.com/Tom-the-Bomb/akinator-rs#254f546eef15c0b593725496ff51c5a15ab8ecaf"
+version = "0.1.11"
+source = "git+https://github.com/Tom-the-Bomb/akinator-rs#89d53cc7f0add8d8710e58dd8d8c0a5482f3a0ed"
 dependencies = [
  "lazy_static",
  "regex",
  "reqwest",
  "serde",
  "serde_json",
  "thiserror",
@@ -51,17 +51,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "bytes"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89b2fd2a0dcf38d7971e2194b6b6eebab45ae01067456a7fd93d5547a61b70be"
 
@@ -188,17 +188,17 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.17"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "66b91535aa35fea1523ad1b86cb6b53c28e0ae566ba4a460f4457e936cad7c6f"
+checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -346,17 +346,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -390,15 +390,15 @@
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
 dependencies = [
  "libc",
  "log",
  "wasi",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
@@ -429,15 +429,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
@@ -551,34 +551,34 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
 
 [[package]]
 name = "reqwest"
-version = "0.11.16"
+version = "0.11.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "27b71749df584b7f4cac2c426c127a7c785a5106cc98f7a8feb044115f0fa254"
+checksum = "13293b639a097af28fc8a90f22add145a9c954e49d77da06263d58cf44d5fb91"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -770,17 +770,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
@@ -811,36 +811,36 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.27.0"
+version = "1.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
+checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
@@ -852,17 +852,17 @@
  "rustls",
  "tokio",
  "webpki",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -1079,75 +1079,141 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winreg"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
 dependencies = [
  "winapi",
 ]
```

### Comparing `akinator.py-0.2.3/PKG-INFO` & `akinator.py-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: akinator.py
-Version: 0.2.3
+Version: 0.2.4
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: sphinxext-opengraph; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Provides-Extra: docs
 License-File: LICENSE
 Summary: Python bindings for akinator-rs
 Keywords: akinator,python,async,game,pyo3
 Home-Page: https://github.com/Tom-the-Bomb/akinator.py
 Author: Tom-the-Bomb
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/Tom-the-Bomb/akinator.py
 Project-URL: documentation, https://akinatorpy.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/Tom-the-Bomb/akinator.py
+Project-URL: repository, https://github.com/Tom-the-Bomb/akinator.py
 
 # Akinator-py
 Python bindings for ``akinator-rs``, a wrapper around the undocumented akinator API, made using [pyo3](https://pyo3.rs)
 
 designed for easy implementation of an akinator game in code, providing a simple and easy to use API.
 
 ### Installation
```

