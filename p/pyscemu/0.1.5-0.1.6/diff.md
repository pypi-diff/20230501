# Comparing `tmp/pyscemu-0.1.5.tar.gz` & `tmp/pyscemu-0.1.6.tar.gz`

## Comparing `pyscemu-0.1.5.tar` & `pyscemu-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.5/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.5/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.5/.gitignore
--rw-r--r--   0     1000     1000     9899 2023-04-30 10:55:32.000000 pyscemu-0.1.5/README.md
--rw-r--r--   0     1000     1000       72 2023-04-30 15:01:19.000000 pyscemu-0.1.5/examples/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0     1000     1000     6632 2023-04-30 13:18:53.000000 pyscemu-0.1.5/examples/.ipynb_checkpoints/raccoon_strings-checkpoint.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.1.5/examples/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000     1598 2023-04-30 14:32:44.000000 pyscemu-0.1.5/examples/.ipynb_checkpoints/xloader_keygen-checkpoint.ipynb
--rw-r--r--   0     1000     1000     2157 2023-04-30 16:11:36.000000 pyscemu-0.1.5/examples/Untitled.ipynb
--rw-r--r--   0     1000     1000     6790 2023-04-30 15:03:12.000000 pyscemu-0.1.5/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.1.5/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.5/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.5/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000      755 2023-04-30 17:09:34.000000 pyscemu-0.1.5/examples/test.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.1.5/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.5/pyproject.toml
--rw-r--r--   0     1000     1000    26293 2023-04-30 22:08:47.000000 pyscemu-0.1.5/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-04-30 22:05:57.000000 pyscemu-0.1.5/Cargo.lock
--rw-r--r--   0        0        0    10225 1970-01-01 00:00:00.000000 pyscemu-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.6/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.6/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.6/.gitignore
+-rw-r--r--   0     1000     1000     9969 2023-04-30 22:56:14.000000 pyscemu-0.1.6/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.1.6/examples/.ipynb_checkpoints/danabot_rsa-checkpoint.ipynb
+-rw-r--r--   0     1000     1000     6632 2023-04-30 13:18:53.000000 pyscemu-0.1.6/examples/.ipynb_checkpoints/raccoon_strings-checkpoint.ipynb
+-rw-r--r--   0     1000     1000     1598 2023-04-30 14:32:44.000000 pyscemu-0.1.6/examples/.ipynb_checkpoints/xloader_keygen-checkpoint.ipynb
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.1.6/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.1.6/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.1.6/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.1.6/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      755 2023-04-30 17:09:34.000000 pyscemu-0.1.6/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.6/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.6/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.1.6/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.6/pyproject.toml
+-rw-r--r--   0     1000     1000    26540 2023-04-30 22:58:27.000000 pyscemu-0.1.6/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-04-30 22:58:19.000000 pyscemu-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0    10295 1970-01-01 00:00:00.000000 pyscemu-0.1.6/PKG-INFO
```

### Comparing `pyscemu-0.1.5/.github/workflows/CI.yml` & `pyscemu-0.1.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.5/.gitignore` & `pyscemu-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.5/README.md` & `pyscemu-0.1.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 https://github.com/sha0coder/scemu
 
 releases:
 
 https://github.com/sha0coder/scemu/releases/download/maps/maps32.zip
 https://github.com/sha0coder/scemu/releases/download/maps/maps64.zip
 
+## Examples
+
+https://github.com/sha0coder/pyscemu/tree/main/examples
+
 ## Usage
 
 ### Fully emulation of a shellcode
 
 ```python
 ~ ❯❯❯ python3
 Python 3.9.2 (default, Feb 28 2021, 17:03:44)
```

### Comparing `pyscemu-0.1.5/examples/.ipynb_checkpoints/raccoon_strings-checkpoint.ipynb` & `pyscemu-0.1.6/examples/.ipynb_checkpoints/raccoon_strings-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.5/examples/.ipynb_checkpoints/xloader_keygen-checkpoint.ipynb` & `pyscemu-0.1.6/examples/.ipynb_checkpoints/xloader_keygen-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.5/examples/Untitled.ipynb` & `pyscemu-0.1.6/examples/.ipynb_checkpoints/danabot_rsa-checkpoint.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991815476190476%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(8, 'rsa_keygen = 0x022EBBC0 \\n'), (25, "*

 * *            "'emu.call(rsa_keygen,[priv_ptr, pub_ptr])\\n')], delete: [30, 29, 28, 27, 26, 25, 24, "*

 * *            '11, 8]}}}'}*

```diff
@@ -21,39 +21,32 @@
                 "\n",
                 "emu = pyscemu.init32()\n",
                 "emu.load_maps('/home/sha0/src/scemu/maps32/')\n",
                 "emu.load_binary('/home/sha0/samples/danabot/2023-04-03-MainModule/unpacked2/dbmm_unpacked.dll')\n",
                 "emu.set_verbose(3)\n",
                 "emu.set_base_address(0x1E70000)\n",
                 "emu.enable_banzai_mode()\n",
-                "danabot_init = 0x022EBBC0 \n",
+                "rsa_keygen = 0x022EBBC0 \n",
                 "\n",
                 "\n",
-                "'''\n",
                 "public_key_ptr = emu.alloc(\"pubkey\", 1024)\n",
                 "private_key_ptr = emu.alloc(\"privkey\", 1024)\n",
                 "pub_ptr = emu.alloc(\"pub_ptr\", 4)\n",
                 "priv_ptr = emu.alloc(\"priv_ptr\", 4)\n",
                 "\n",
                 "emu.write_dword(pub_ptr, public_key_ptr)\n",
                 "emu.write_dword(priv_ptr, private_key_ptr)\n",
                 "\n",
                 "emu.enable_trace_reg(['eax'])\n",
                 "\n",
                 "emu.set_reg('eax', pub_ptr)\n",
                 "emu.set_reg('edx', priv_ptr)\n",
-                "'''\n",
                 "\n",
-                "emu.set_reg('eax', 1)\n",
-                "emu.set_reg('esi', 1)\n",
-                "ret_addr = emu.set_reg('eip', danabot_init)\n",
-                "emu.run(ret_addr)\n",
                 "\n",
-                "\n",
-                "\n"
+                "emu.call(rsa_keygen,[priv_ptr, pub_ptr])\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "77cfab8c-f385-4d95-a3e5-c2a0455a0ea8",
             "metadata": {},
```

### Comparing `pyscemu-0.1.5/examples/raccoon_strings.ipynb` & `pyscemu-0.1.6/examples/raccoon_strings.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998015873015873%*

 * *Differences: {"'cells'": '{1: {\'source\': {insert: [(25, "    if opcode == 0x6a:  # '*

 * *            'emu.get_prev_mnemonic().startswith(\'ret\')\\n")], delete: [25]}}}'}*

```diff
@@ -205,15 +205,15 @@
                 "while True:\n",
                 "    emu.step()\n",
                 "\n",
                 "    if emu.get_reg('eip') >= 0x040b488:\n",
                 "        break\n",
                 "\n",
                 "    opcode = emu.read_byte(emu.get_reg('eip'))\n",
-                "    if opcode == 0x6a:    \n",
+                "    if opcode == 0x6a:  # emu.get_prev_mnemonic().startswith('ret')\n",
                 "        decrypted_ptr = emu.get_reg('eax')\n",
                 "        decrypted = emu.read_string(decrypted_ptr)\n",
                 "        strings.append(f'{hex(decrypted_ptr)}: {decrypted}')\n",
                 "\n",
                 "\n",
                 "for s in list(set(strings)):\n",
                 "    if s:\n",
```

### Comparing `pyscemu-0.1.5/examples/scripts/raccoon_strings.py` & `pyscemu-0.1.6/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.5/examples/scripts/xloader_dexor.py` & `pyscemu-0.1.6/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.5/examples/test.py` & `pyscemu-0.1.6/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.5/examples/xloader_keygen.ipynb` & `pyscemu-0.1.6/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.5/src/lib.rs` & `pyscemu-0.1.6/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 impl Emu {
 
     /// get pyscemu version
     fn version(&self) -> String {
         return env!("CARGO_PKG_VERSION").to_string();
     }
 
+    fn get_prev_mnemonic(&self) -> PyResult<String> {
+        return Ok(self.emu.out.clone());
+    }
+
     /// reset the instruction counter to zero.
     fn reset_pos(&mut self) {
         self.emu.pos = 0;
     }
    
     /// check if the emulator is in 64bits mode
     fn is_64bits(&self) -> PyResult<bool> {
@@ -759,22 +763,26 @@
     /// get the memory breakpoint on write
     pub fn bp_get_mem_write(&self) -> PyResult<u64> {
         return Ok(self.emu.bp.get_mem_write());
     }
 
     // hooks
 
+    /// use a synchronous loop with step() instead of using the run_hook(hook) 
+    /// this method is experimental.
     pub fn run_hook(&mut self, callback: PyObject) {
         loop {
             self.emu.step();
 
             let gil = Python::acquire_gil();
             let py = gil.python();
 
-            match callback.call1(py, (self.emu.regs.rip, &self.emu.out,)) {
+
+            let args = (self.emu.regs.rip, &self.emu.out,);
+            match callback.call1(py, args) {
                 Ok(r) => {
                     match r.extract::<bool>(py) {
                         Ok(b) => {
                             if b {
                                 continue;
                             } else {
                                 break;
@@ -783,16 +791,14 @@
                         Err(_) => break,
                     }
                 },
                 Err(_) => break,
             }
         }
     }
-
-
 }
 
 
 
 
 
 #[pyfunction]
```

### Comparing `pyscemu-0.1.5/Cargo.lock` & `pyscemu-0.1.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.1.5/PKG-INFO` & `pyscemu-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
@@ -28,14 +28,18 @@
 https://github.com/sha0coder/scemu
 
 releases:
 
 https://github.com/sha0coder/scemu/releases/download/maps/maps32.zip
 https://github.com/sha0coder/scemu/releases/download/maps/maps64.zip
 
+## Examples
+
+https://github.com/sha0coder/pyscemu/tree/main/examples
+
 ## Usage
 
 ### Fully emulation of a shellcode
 
 ```python
 ~ ❯❯❯ python3
 Python 3.9.2 (default, Feb 28 2021, 17:03:44)
```

