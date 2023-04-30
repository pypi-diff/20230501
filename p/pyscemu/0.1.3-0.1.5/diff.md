# Comparing `tmp/pyscemu-0.1.3.tar.gz` & `tmp/pyscemu-0.1.5.tar.gz`

## Comparing `pyscemu-0.1.3.tar` & `pyscemu-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,19 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.3/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.3/.gitignore
--rw-r--r--   0     1000     1000     9899 2023-04-30 10:55:32.000000 pyscemu-0.1.3/README.md
--rw-r--r--   0     1000     1000      723 2023-04-30 12:20:49.000000 pyscemu-0.1.3/examples/raccoon_strings.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.3/examples/xloader_dexor.py
--rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.3/examples/xloader_keygen.py
--rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.3/pyproject.toml
--rw-r--r--   0     1000     1000    24019 2023-04-30 12:21:37.000000 pyscemu-0.1.3/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-04-30 12:23:14.000000 pyscemu-0.1.3/Cargo.lock
--rw-r--r--   0        0        0    10225 1970-01-01 00:00:00.000000 pyscemu-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.5/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.5/.gitignore
+-rw-r--r--   0     1000     1000     9899 2023-04-30 10:55:32.000000 pyscemu-0.1.5/README.md
+-rw-r--r--   0     1000     1000       72 2023-04-30 15:01:19.000000 pyscemu-0.1.5/examples/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0     1000     1000     6632 2023-04-30 13:18:53.000000 pyscemu-0.1.5/examples/.ipynb_checkpoints/raccoon_strings-checkpoint.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.1.5/examples/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000     1598 2023-04-30 14:32:44.000000 pyscemu-0.1.5/examples/.ipynb_checkpoints/xloader_keygen-checkpoint.ipynb
+-rw-r--r--   0     1000     1000     2157 2023-04-30 16:11:36.000000 pyscemu-0.1.5/examples/Untitled.ipynb
+-rw-r--r--   0     1000     1000     6790 2023-04-30 15:03:12.000000 pyscemu-0.1.5/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.1.5/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.5/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.5/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000      755 2023-04-30 17:09:34.000000 pyscemu-0.1.5/examples/test.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.1.5/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.5/pyproject.toml
+-rw-r--r--   0     1000     1000    26293 2023-04-30 22:08:47.000000 pyscemu-0.1.5/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-04-30 22:05:57.000000 pyscemu-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0    10225 1970-01-01 00:00:00.000000 pyscemu-0.1.5/PKG-INFO
```

### Comparing `pyscemu-0.1.3/.github/workflows/CI.yml` & `pyscemu-0.1.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.3/.gitignore` & `pyscemu-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.3/README.md` & `pyscemu-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.3/examples/raccoon_strings.py` & `pyscemu-0.1.5/examples/scripts/raccoon_strings.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,19 +19,18 @@
 while True:
     emu.step()
 
     if emu.get_reg('eip') >= 0x040b488:
         break
 
     opcode = emu.read_byte(emu.get_reg('eip'))
-    print(hex(opcode))
-    if opcode == 0x59:    
-        decrypted_ptr = emu.get_reg('ecx')
+    if opcode == 0x6a:    
+        decrypted_ptr = emu.get_reg('eax')
         decrypted = emu.read_string(decrypted_ptr)
-        strings.append(decrypted)
+        strings.append(f'{hex(decrypted_ptr)}: {decrypted}')
 
 
 for s in list(set(strings)):
     if s:
         print(s)
 
 #emu.show_allocs()
```

### Comparing `pyscemu-0.1.3/examples/xloader_dexor.py` & `pyscemu-0.1.5/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.3/src/lib.rs` & `pyscemu-0.1.5/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 use libscemu::emu32;
 use libscemu::emu64;
 
 use pyo3::prelude::*;
 use pyo3::exceptions::PyValueError;
 
 
-
 #[pyclass]
-struct Emu {
+pub struct Emu {
     emu: libscemu::emu::Emu,
 }
 
 #[pymethods]
+#[allow(deprecated)]
 impl Emu {
 
+    /// get pyscemu version
+    fn version(&self) -> String {
+        return env!("CARGO_PKG_VERSION").to_string();
+    }
+
     /// reset the instruction counter to zero.
     fn reset_pos(&mut self) {
         self.emu.pos = 0;
     }
    
     /// check if the emulator is in 64bits mode
     fn is_64bits(&self) -> PyResult<bool> {
@@ -700,35 +705,119 @@
     }
 
     /// perform a memory test to see overlapps or other possible problems.
     pub fn mem_test(&self) -> PyResult<bool> {
         return Ok(self.emu.maps.mem_test());
     }
 
+    /// breakpoints
+
+    /// show breakpoints
+    pub fn bp_show(&self) {
+        self.emu.bp.show();
+    }
+
+    /// clear all the breakpoints
+    pub fn bp_clear_all(&mut self) {
+        self.emu.bp.clear_bp();
+    }
+
+    /// set breakpoint on an address
+    pub fn bp_set_addr(&mut self, addr:u64) {
+        self.emu.bp.set_bp(addr);
+    }
+
+    /// get the current address breakpoint
+    pub fn bp_get_addr(&self) -> PyResult<u64> {
+        return Ok(self.emu.bp.get_bp());
+    }
+
+    /// set breakpoint on a instruction counter
+    pub fn bp_set_inst(&mut self, ins:u64) {
+        self.emu.bp.set_instruction(ins);
+    }
+
+    /// get breakpoint on a instrunction counter
+    pub fn bp_get_inst(&self) -> PyResult<u64> {
+        return Ok(self.emu.bp.get_instruction());
+    }
+
+    /// set a memory breakpoint on read
+    pub fn bp_set_mem_read(&mut self, addr:u64) {
+        self.emu.bp.set_mem_read(addr);
+    }
+
+    /// get the memory breakpoint on read
+    pub fn bp_get_mem_read(&self) -> PyResult<u64> {
+        return Ok(self.emu.bp.get_mem_read());
+    }
+
+    /// set a memory breakpoint on write
+    pub fn bp_set_mem_write(&mut self, addr:u64) {
+        self.emu.bp.set_mem_write(addr);
+    }
+
+    /// get the memory breakpoint on write
+    pub fn bp_get_mem_write(&self) -> PyResult<u64> {
+        return Ok(self.emu.bp.get_mem_write());
+    }
+
+    // hooks
+
+    pub fn run_hook(&mut self, callback: PyObject) {
+        loop {
+            self.emu.step();
+
+            let gil = Python::acquire_gil();
+            let py = gil.python();
+
+            match callback.call1(py, (self.emu.regs.rip, &self.emu.out,)) {
+                Ok(r) => {
+                    match r.extract::<bool>(py) {
+                        Ok(b) => {
+                            if b {
+                                continue;
+                            } else {
+                                break;
+                            }
+                        }
+                        Err(_) => break,
+                    }
+                },
+                Err(_) => break,
+            }
+        }
+    }
+
+
 }
 
 
 
 
 
 #[pyfunction]
 fn init32() -> PyResult<Emu> {
-    let mut emu = Emu{emu: emu32()};
+    let mut emu = Emu{
+        emu: emu32(), 
+    };
     emu.emu.cfg.is_64bits = false;
     emu.emu.cfg.console_enabled = false;
     emu.emu.cfg.verbose = 0;
 
 
     Ok(emu)
 }
 
 
 #[pyfunction]
 fn init64() -> PyResult<Emu> {
-    let mut emu = Emu{emu: emu64()};
+    let mut emu = Emu{
+        emu: emu64(), 
+    };
     emu.emu.cfg.is_64bits = true;
     emu.emu.cfg.console_enabled = false;
     emu.emu.cfg.verbose = 0;
 
     Ok(emu)
 }
```

### Comparing `pyscemu-0.1.3/Cargo.lock` & `pyscemu-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.11.6"
+version = "0.11.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea355172c86c50676adbf3c9753a409ff4ad0149b60ee5bef3eafcfc9727ce48"
+checksum = "2cffdb15b120776d2eed7a3cb432cc77fb271ea56da588f41a45c82606678845"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.1.3"
+version = "0.1.5"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.1.3/PKG-INFO` & `pyscemu-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.1.3
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
```

