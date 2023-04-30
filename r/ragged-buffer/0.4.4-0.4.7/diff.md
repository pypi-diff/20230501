# Comparing `tmp/ragged_buffer-0.4.4.tar.gz` & `tmp/ragged_buffer-0.4.7.tar.gz`

## Comparing `ragged_buffer-0.4.4.tar` & `ragged_buffer-0.4.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 ragged_buffer-0.4.4/Cargo.toml
--rw-r--r--   0        0        0     1675 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/.github/workflows/publish-wheel.yaml
--rw-r--r--   0        0        0      668 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/.github/workflows/test.yaml
--rw-r--r--   0        0        0       55 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/.gitignore
--rw-r--r--   0        0        0     9867 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/LICENSE-APACHE
--rw-r--r--   0        0        0     1091 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/LICENSE-MIT
--rw-r--r--   0        0        0     6663 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/README.md
--rw-r--r--   0        0        0      386 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/monomorphize.sh
--rw-r--r--   0        0        0      406 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2358 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/ragged_buffer/__init__.py
--rw-r--r--   0        0        0     2769 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/ragged_buffer/__init__.pyi
--rw-r--r--   0        0        0        0 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/ragged_buffer/py.typed
--rw-r--r--   0        0        0      945 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/src/lib.rs
--rw-r--r--   0        0        0     6449 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/src/monomorphs/bool.rs
--rw-r--r--   0        0        0     6403 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/src/monomorphs/f32.rs
--rw-r--r--   0        0        0     6362 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/src/monomorphs/i64.rs
--rw-r--r--   0        0        0     1490 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/src/monomorphs.rs
--rw-r--r--   0        0        0    22561 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/src/ragged_buffer.rs
--rw-r--r--   0        0        0    22562 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/src/ragged_buffer_view.rs
--rw-r--r--   0        0        0    13190 2022-08-26 03:43:32.000000 ragged_buffer-0.4.4/tests/test.py
--rw-r--r--   0        0        0     7315 1970-01-01 00:00:00.000000 ragged_buffer-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      647 1970-01-01 00:00:00.000000 ragged_buffer-0.4.7/Cargo.toml
+-rw-r--r--   0      501       20     1613 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/.github/workflows/publish-wheel.yaml
+-rw-r--r--   0      501       20      637 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/.github/workflows/test.yaml
+-rw-r--r--   0      501       20       50 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/.gitignore
+-rw-r--r--   0      501       20     9694 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/LICENSE-APACHE
+-rw-r--r--   0      501       20     1071 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/LICENSE-MIT
+-rw-r--r--   0      501       20     6476 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/README.md
+-rwxr-xr-x   0      501       20      376 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/monomorphize.sh
+-rw-r--r--   0      501       20      391 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/pyproject.toml
+-rw-r--r--   0      501       20     2295 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/ragged_buffer/__init__.py
+-rw-r--r--   0      501       20     2698 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/ragged_buffer/__init__.pyi
+-rw-r--r--   0      501       20        0 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/ragged_buffer/py.typed
+-rw-r--r--   0      501       20      913 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/src/lib.rs
+-rw-r--r--   0      501       20     6257 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/src/monomorphs/bool.rs
+-rw-r--r--   0      501       20     6198 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/src/monomorphs/f32.rs
+-rw-r--r--   0      501       20     6171 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/src/monomorphs/i64.rs
+-rw-r--r--   0      501       20     1440 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/src/monomorphs.rs
+-rw-r--r--   0      501       20    22141 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/src/ragged_buffer.rs
+-rw-r--r--   0      501       20    22095 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/src/ragged_buffer_view.rs
+-rw-r--r--   0      501       20    12701 2023-04-30 23:47:22.000000 ragged_buffer-0.4.7/tests/test.py
+-rw-r--r--   0      501       20     9138 2023-04-30 23:48:31.000000 ragged_buffer-0.4.7/Cargo.lock
+-rw-r--r--   0        0        0     7209 1970-01-01 00:00:00.000000 ragged_buffer-0.4.7/PKG-INFO
```

### Comparing `ragged_buffer-0.4.4/Cargo.toml` & `ragged_buffer-0.4.7/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-[package]
-name = "ragged-buffer"
-version = "0.4.4"
-edition = "2021"
-authors = ["Clemens Winter <clemenswinter1@gmail.com>"]
-readme = "README.md"
-license = "MIT OR Apache-2.0"
-description = "Efficient RaggedBuffer datatype that implements 3D arrays with variable-length 2nd dimension."
-
-[lib]
-name = "ragged_buffer"
-crate-type = ["cdylib", "rlib"]
-
-[dependencies]
-numpy = { version = "0.16.2", optional = true }
-pyo3 = { version = "0.16.5", features = ["extension-module"], optional = true }
-ndarray = "0.15.4"
-
-[profile.release]
-debug = true
-
-[features]
-python = ["pyo3", "numpy"]
+[package]
+authors = ["Clemens Winter <clemenswinter1@gmail.com>"]
+description = "Efficient RaggedBuffer datatype that implements 3D arrays with variable-length 2nd dimension."
+edition = "2021"
+license = "MIT OR Apache-2.0"
+name = "ragged-buffer"
+readme = "README.md"
+repository = "https://github.com/entity-neural-network/ragged-buffer"
+version = "0.4.7"
+
+[lib]
+crate-type = ["cdylib", "rlib"]
+name = "ragged_buffer"
+
+[dependencies]
+ndarray = "0.15.4"
+numpy = {version = "0.16.2", optional = true}
+pyo3 = {version = "0.16.5", features = ["extension-module"], optional = true}
+
+[profile.release]
+debug = true
+
+[features]
+python = ["pyo3", "numpy"]
```

### Comparing `ragged_buffer-0.4.4/LICENSE-APACHE` & `ragged_buffer-0.4.7/LICENSE-APACHE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-                              Apache License
-                        Version 2.0, January 2004
-                     http://www.apache.org/licenses/
-
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-1. Definitions.
-
-   "License" shall mean the terms and conditions for use, reproduction,
-   and distribution as defined by Sections 1 through 9 of this document.
-
-   "Licensor" shall mean the copyright owner or entity authorized by
-   the copyright owner that is granting the License.
-
-   "Legal Entity" shall mean the union of the acting entity and all
-   other entities that control, are controlled by, or are under common
-   control with that entity. For the purposes of this definition,
-   "control" means (i) the power, direct or indirect, to cause the
-   direction or management of such entity, whether by contract or
-   otherwise, or (ii) ownership of fifty percent (50%) or more of the
-   outstanding shares, or (iii) beneficial ownership of such entity.
-
-   "You" (or "Your") shall mean an individual or Legal Entity
-   exercising permissions granted by this License.
-
-   "Source" form shall mean the preferred form for making modifications,
-   including but not limited to software source code, documentation
-   source, and configuration files.
-
-   "Object" form shall mean any form resulting from mechanical
-   transformation or translation of a Source form, including but
-   not limited to compiled object code, generated documentation,
-   and conversions to other media types.
-
-   "Work" shall mean the work of authorship, whether in Source or
-   Object form, made available under the License, as indicated by a
-   copyright notice that is included in or attached to the work
-   (an example is provided in the Appendix below).
-
-   "Derivative Works" shall mean any work, whether in Source or Object
-   form, that is based on (or derived from) the Work and for which the
-   editorial revisions, annotations, elaborations, or other modifications
-   represent, as a whole, an original work of authorship. For the purposes
-   of this License, Derivative Works shall not include works that remain
-   separable from, or merely link (or bind by name) to the interfaces of,
-   the Work and Derivative Works thereof.
-
-   "Contribution" shall mean any work of authorship, including
-   the original version of the Work and any modifications or additions
-   to that Work or Derivative Works thereof, that is intentionally
-   submitted to Licensor for inclusion in the Work by the copyright owner
-   or by an individual or Legal Entity authorized to submit on behalf of
-   the copyright owner. For the purposes of this definition, "submitted"
-   means any form of electronic, verbal, or written communication sent
-   to the Licensor or its representatives, including but not limited to
-   communication on electronic mailing lists, source code control systems,
-   and issue tracking systems that are managed by, or on behalf of, the
-   Licensor for the purpose of discussing and improving the Work, but
-   excluding communication that is conspicuously marked or otherwise
-   designated in writing by the copyright owner as "Not a Contribution."
-
-   "Contributor" shall mean Licensor and any individual or Legal Entity
-   on behalf of whom a Contribution has been received by Licensor and
-   subsequently incorporated within the Work.
-
-2. Grant of Copyright License. Subject to the terms and conditions of
-   this License, each Contributor hereby grants to You a perpetual,
-   worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-   copyright license to reproduce, prepare Derivative Works of,
-   publicly display, publicly perform, sublicense, and distribute the
-   Work and such Derivative Works in Source or Object form.
-
-3. Grant of Patent License. Subject to the terms and conditions of
-   this License, each Contributor hereby grants to You a perpetual,
-   worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-   (except as stated in this section) patent license to make, have made,
-   use, offer to sell, sell, import, and otherwise transfer the Work,
-   where such license applies only to those patent claims licensable
-   by such Contributor that are necessarily infringed by their
-   Contribution(s) alone or by combination of their Contribution(s)
-   with the Work to which such Contribution(s) was submitted. If You
-   institute patent litigation against any entity (including a
-   cross-claim or counterclaim in a lawsuit) alleging that the Work
-   or a Contribution incorporated within the Work constitutes direct
-   or contributory patent infringement, then any patent licenses
-   granted to You under this License for that Work shall terminate
-   as of the date such litigation is filed.
-
-4. Redistribution. You may reproduce and distribute copies of the
-   Work or Derivative Works thereof in any medium, with or without
-   modifications, and in Source or Object form, provided that You
-   meet the following conditions:
-
-   (a) You must give any other recipients of the Work or
-       Derivative Works a copy of this License; and
-
-   (b) You must cause any modified files to carry prominent notices
-       stating that You changed the files; and
-
-   (c) You must retain, in the Source form of any Derivative Works
-       that You distribute, all copyright, patent, trademark, and
-       attribution notices from the Source form of the Work,
-       excluding those notices that do not pertain to any part of
-       the Derivative Works; and
-
-   (d) If the Work includes a "NOTICE" text file as part of its
-       distribution, then any Derivative Works that You distribute must
-       include a readable copy of the attribution notices contained
-       within such NOTICE file, excluding those notices that do not
-       pertain to any part of the Derivative Works, in at least one
-       of the following places: within a NOTICE text file distributed
-       as part of the Derivative Works; within the Source form or
-       documentation, if provided along with the Derivative Works; or,
-       within a display generated by the Derivative Works, if and
-       wherever such third-party notices normally appear. The contents
-       of the NOTICE file are for informational purposes only and
-       do not modify the License. You may add Your own attribution
-       notices within Derivative Works that You distribute, alongside
-       or as an addendum to the NOTICE text from the Work, provided
-       that such additional attribution notices cannot be construed
-       as modifying the License.
-
-   You may add Your own copyright statement to Your modifications and
-   may provide additional or different license terms and conditions
-   for use, reproduction, or distribution of Your modifications, or
-   for any such Derivative Works as a whole, provided Your use,
-   reproduction, and distribution of the Work otherwise complies with
-   the conditions stated in this License.
-
-5. Submission of Contributions. Unless You explicitly state otherwise,
-   any Contribution intentionally submitted for inclusion in the Work
-   by You to the Licensor shall be under the terms and conditions of
-   this License, without any additional terms or conditions.
-   Notwithstanding the above, nothing herein shall supersede or modify
-   the terms of any separate license agreement you may have executed
-   with Licensor regarding such Contributions.
-
-6. Trademarks. This License does not grant permission to use the trade
-   names, trademarks, service marks, or product names of the Licensor,
-   except as required for reasonable and customary use in describing the
-   origin of the Work and reproducing the content of the NOTICE file.
-
-7. Disclaimer of Warranty. Unless required by applicable law or
-   agreed to in writing, Licensor provides the Work (and each
-   Contributor provides its Contributions) on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-   implied, including, without limitation, any warranties or conditions
-   of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-   PARTICULAR PURPOSE. You are solely responsible for determining the
-   appropriateness of using or redistributing the Work and assume any
-   risks associated with Your exercise of permissions under this License.
-
-8. Limitation of Liability. In no event and under no legal theory,
-   whether in tort (including negligence), contract, or otherwise,
-   unless required by applicable law (such as deliberate and grossly
-   negligent acts) or agreed to in writing, shall any Contributor be
-   liable to You for damages, including any direct, indirect, special,
-   incidental, or consequential damages of any character arising as a
-   result of this License or out of the use or inability to use the
-   Work (including but not limited to damages for loss of goodwill,
-   work stoppage, computer failure or malfunction, or any and all
-   other commercial damages or losses), even if such Contributor
-   has been advised of the possibility of such damages.
-
-9. Accepting Warranty or Additional Liability. While redistributing
-   the Work or Derivative Works thereof, You may choose to offer,
-   and charge a fee for, acceptance of support, warranty, indemnity,
-   or other liability obligations and/or rights consistent with this
-   License. However, in accepting such obligations, You may act only
-   on Your own behalf and on Your sole responsibility, not on behalf
-   of any other Contributor, and only if You agree to indemnify,
-   defend, and hold each Contributor harmless for any liability
-   incurred by, or claims asserted against, such Contributor by reason
+                              Apache License
+                        Version 2.0, January 2004
+                     http://www.apache.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+   "License" shall mean the terms and conditions for use, reproduction,
+   and distribution as defined by Sections 1 through 9 of this document.
+
+   "Licensor" shall mean the copyright owner or entity authorized by
+   the copyright owner that is granting the License.
+
+   "Legal Entity" shall mean the union of the acting entity and all
+   other entities that control, are controlled by, or are under common
+   control with that entity. For the purposes of this definition,
+   "control" means (i) the power, direct or indirect, to cause the
+   direction or management of such entity, whether by contract or
+   otherwise, or (ii) ownership of fifty percent (50%) or more of the
+   outstanding shares, or (iii) beneficial ownership of such entity.
+
+   "You" (or "Your") shall mean an individual or Legal Entity
+   exercising permissions granted by this License.
+
+   "Source" form shall mean the preferred form for making modifications,
+   including but not limited to software source code, documentation
+   source, and configuration files.
+
+   "Object" form shall mean any form resulting from mechanical
+   transformation or translation of a Source form, including but
+   not limited to compiled object code, generated documentation,
+   and conversions to other media types.
+
+   "Work" shall mean the work of authorship, whether in Source or
+   Object form, made available under the License, as indicated by a
+   copyright notice that is included in or attached to the work
+   (an example is provided in the Appendix below).
+
+   "Derivative Works" shall mean any work, whether in Source or Object
+   form, that is based on (or derived from) the Work and for which the
+   editorial revisions, annotations, elaborations, or other modifications
+   represent, as a whole, an original work of authorship. For the purposes
+   of this License, Derivative Works shall not include works that remain
+   separable from, or merely link (or bind by name) to the interfaces of,
+   the Work and Derivative Works thereof.
+
+   "Contribution" shall mean any work of authorship, including
+   the original version of the Work and any modifications or additions
+   to that Work or Derivative Works thereof, that is intentionally
+   submitted to Licensor for inclusion in the Work by the copyright owner
+   or by an individual or Legal Entity authorized to submit on behalf of
+   the copyright owner. For the purposes of this definition, "submitted"
+   means any form of electronic, verbal, or written communication sent
+   to the Licensor or its representatives, including but not limited to
+   communication on electronic mailing lists, source code control systems,
+   and issue tracking systems that are managed by, or on behalf of, the
+   Licensor for the purpose of discussing and improving the Work, but
+   excluding communication that is conspicuously marked or otherwise
+   designated in writing by the copyright owner as "Not a Contribution."
+
+   "Contributor" shall mean Licensor and any individual or Legal Entity
+   on behalf of whom a Contribution has been received by Licensor and
+   subsequently incorporated within the Work.
+
+2. Grant of Copyright License. Subject to the terms and conditions of
+   this License, each Contributor hereby grants to You a perpetual,
+   worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+   copyright license to reproduce, prepare Derivative Works of,
+   publicly display, publicly perform, sublicense, and distribute the
+   Work and such Derivative Works in Source or Object form.
+
+3. Grant of Patent License. Subject to the terms and conditions of
+   this License, each Contributor hereby grants to You a perpetual,
+   worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+   (except as stated in this section) patent license to make, have made,
+   use, offer to sell, sell, import, and otherwise transfer the Work,
+   where such license applies only to those patent claims licensable
+   by such Contributor that are necessarily infringed by their
+   Contribution(s) alone or by combination of their Contribution(s)
+   with the Work to which such Contribution(s) was submitted. If You
+   institute patent litigation against any entity (including a
+   cross-claim or counterclaim in a lawsuit) alleging that the Work
+   or a Contribution incorporated within the Work constitutes direct
+   or contributory patent infringement, then any patent licenses
+   granted to You under this License for that Work shall terminate
+   as of the date such litigation is filed.
+
+4. Redistribution. You may reproduce and distribute copies of the
+   Work or Derivative Works thereof in any medium, with or without
+   modifications, and in Source or Object form, provided that You
+   meet the following conditions:
+
+   (a) You must give any other recipients of the Work or
+       Derivative Works a copy of this License; and
+
+   (b) You must cause any modified files to carry prominent notices
+       stating that You changed the files; and
+
+   (c) You must retain, in the Source form of any Derivative Works
+       that You distribute, all copyright, patent, trademark, and
+       attribution notices from the Source form of the Work,
+       excluding those notices that do not pertain to any part of
+       the Derivative Works; and
+
+   (d) If the Work includes a "NOTICE" text file as part of its
+       distribution, then any Derivative Works that You distribute must
+       include a readable copy of the attribution notices contained
+       within such NOTICE file, excluding those notices that do not
+       pertain to any part of the Derivative Works, in at least one
+       of the following places: within a NOTICE text file distributed
+       as part of the Derivative Works; within the Source form or
+       documentation, if provided along with the Derivative Works; or,
+       within a display generated by the Derivative Works, if and
+       wherever such third-party notices normally appear. The contents
+       of the NOTICE file are for informational purposes only and
+       do not modify the License. You may add Your own attribution
+       notices within Derivative Works that You distribute, alongside
+       or as an addendum to the NOTICE text from the Work, provided
+       that such additional attribution notices cannot be construed
+       as modifying the License.
+
+   You may add Your own copyright statement to Your modifications and
+   may provide additional or different license terms and conditions
+   for use, reproduction, or distribution of Your modifications, or
+   for any such Derivative Works as a whole, provided Your use,
+   reproduction, and distribution of the Work otherwise complies with
+   the conditions stated in this License.
+
+5. Submission of Contributions. Unless You explicitly state otherwise,
+   any Contribution intentionally submitted for inclusion in the Work
+   by You to the Licensor shall be under the terms and conditions of
+   this License, without any additional terms or conditions.
+   Notwithstanding the above, nothing herein shall supersede or modify
+   the terms of any separate license agreement you may have executed
+   with Licensor regarding such Contributions.
+
+6. Trademarks. This License does not grant permission to use the trade
+   names, trademarks, service marks, or product names of the Licensor,
+   except as required for reasonable and customary use in describing the
+   origin of the Work and reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty. Unless required by applicable law or
+   agreed to in writing, Licensor provides the Work (and each
+   Contributor provides its Contributions) on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+   implied, including, without limitation, any warranties or conditions
+   of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+   PARTICULAR PURPOSE. You are solely responsible for determining the
+   appropriateness of using or redistributing the Work and assume any
+   risks associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability. In no event and under no legal theory,
+   whether in tort (including negligence), contract, or otherwise,
+   unless required by applicable law (such as deliberate and grossly
+   negligent acts) or agreed to in writing, shall any Contributor be
+   liable to You for damages, including any direct, indirect, special,
+   incidental, or consequential damages of any character arising as a
+   result of this License or out of the use or inability to use the
+   Work (including but not limited to damages for loss of goodwill,
+   work stoppage, computer failure or malfunction, or any and all
+   other commercial damages or losses), even if such Contributor
+   has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability. While redistributing
+   the Work or Derivative Works thereof, You may choose to offer,
+   and charge a fee for, acceptance of support, warranty, indemnity,
+   or other liability obligations and/or rights consistent with this
+   License. However, in accepting such obligations, You may act only
+   on Your own behalf and on Your sole responsibility, not on behalf
+   of any other Contributor, and only if You agree to indemnify,
+   defend, and hold each Contributor harmless for any liability
+   incurred by, or claims asserted against, such Contributor by reason
    of your accepting any such warranty or additional liability.
```

### Comparing `ragged_buffer-0.4.4/LICENSE-MIT` & `ragged_buffer-0.4.7/LICENSE-MIT`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Clemens Winter
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2021 Clemens Winter
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `ragged_buffer-0.4.4/README.md` & `ragged_buffer-0.4.7/README.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-# ENN Ragged Buffer
-
-[![Actions Status](https://github.com/entity-neural-network/ragged-buffer/workflows/Test/badge.svg)](https://github.com/entity-neural-network/ragged-buffer/actions)
-[![PyPI](https://img.shields.io/pypi/v/ragged-buffer.svg?style=flat-square)](https://pypi.org/project/ragged-buffer/)
-[![Discord](https://img.shields.io/discord/913497968701747270?style=flat-square)](https://discord.gg/SjVqhSW4Qf)
-
-This Python package implements an efficient `RaggedBuffer` datatype that is similar to
-a 3D numpy array, but which allows for variable sequence length in the second
-dimension. It was created primarily for use in [enn-trainer](https://github.com/entity-neural-network/enn-trainer) 
-and currently only supports a small selection of the numpy array methods.
-
-![Ragged Buffer](https://user-images.githubusercontent.com/12845088/143787823-c6a585de-aeda-429c-9824-f4b4a98e6cea.png)
-
-## User Guide
-
-Install the package with `pip install ragged-buffer`.
-The package currently supports three `RaggedBuffer` variants, `RaggedBufferF32`, `RaggedBufferI64`, and `RaggedBufferBool`.
-
-<!-- no toc -->
-- [Creating a RaggedBuffer](#creating-a-raggedbuffer)
-- [Get size](#get-size)
-- [Convert to numpy array](#convert-to-numpy-array)
-- [Indexing](#indexing)
-- [Addition](#addition)
-- [Concatenation](#concatentation)
-- [Clear](#clear)
-
-### Creating a RaggedBuffer
-
-There are three ways to create a `RaggedBuffer`:
-- `RaggedBufferF32(features: int)` creates an empty `RaggedBuffer` with the specified number of features.
-- `RaggedBufferF32.from_flattened(flattened: np.ndarray, lenghts: np.ndarray)` creates a `RaggedBuffer` from a flattened 2D numpy array and a 1D numpy array of lengths.
-- `RaggedBufferF32.from_array` creates a `RaggedBuffer` (with equal sequence lenghts) from a 3D numpy array.
-
-Creating an empty buffer and pushing each row:
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-# Create an empty RaggedBuffer with a feature size of 3
-buffer = RaggedBufferF32(3)
-# Push sequences with 3, 5, 0, and 1 elements
-buffer.push(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]], dtype=np.float32))
-buffer.push(np.array([[10, 11, 12], [13, 14, 15], [16, 17, 18], [19, 20, 21], [22, 23, 24]], dtype=np.float32))
-buffer.push(np.array([], dtype=np.float32))  # Alternative: `buffer.push_empty()`
-buffer.push(np.array([[25, 25, 27]], dtype=np.float32))
-```
-
-Creating a RaggedBuffer from a flat 2D numpy array which combines the first and second dimension,
-and an array of sequence lengths:
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-buffer = RaggedBufferF32.from_flattened(
-    np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12], [13, 14, 15], [16, 17, 18], [19, 20, 21], [22, 23, 24], [25, 25, 27]], dtype=np.float32),
-    np.array([3, 5, 0, 1], dtype=np.int64))
-)
-```
-
-Creating a RaggedBuffer from a 3D numpy array (all sequences have the same length):
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-buffer = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
-```
-
-### Get size
-
-The `size0`, `size1`, and `size2` methods return the number of sequences, the number of elements in a sequence, and the number of features respectively.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-buffer = RaggedBufferF32.from_flattened(
-    np.zeros((9, 64), dtype=np.float32),
-    np.array([3, 5, 0, 1], dtype=np.int64))
-)
-
-# Get size of the first/batch dimension.
-assert buffer.size0() == 10
-# Get size of individual sequences.
-assert buffer.size1(1) == 5
-assert buffer.size1(2) == 0
-# Get size of the last/feature dimension.
-assert buffer.size2() == 64
-```
-
-### Convert to numpy array
-
-`as_aray` converts a `RaggedBuffer` to a flat 2D numpy array that combines the first and second dimension.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferI64
-
-buffer = RaggedBufferI64(1)
-buffer.push(np.array([[1], [1], [1]], dtype=np.int64))
-buffer.push(np.array([[2], [2]], dtype=np.int64))
-assert np.all(buffer.as_array(), np.array([[1], [1], [1], [2], [2]], dtype=np.int64))
-```
-
-### Indexing
-
-You can index a `RaggedBuffer` with a single integer (returning a `RaggedBuffer` with a single sequence), or with a numpy array of integers selecting/permuting multiple sequences.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-# Create a new `RaggedBufferF32`
-buffer = RaggedBufferF32.from_flattened(
-    np.arange(0, 40, dtype=np.float32).reshape(10, 4),
-    np.array([3, 5, 0, 1], dtype=np.int64)
-)
-
-# Retrieve the first sequence.
-assert np.all(
-    buffer[0].as_array() ==
-    np.array([[0, 1, 2, 3], [4, 5, 6, 7], [8, 9, 10, 11]], dtype=np.float32)
-)
-
-# Get a RaggedBatch with 2 randomly selected sequences.
-buffer[np.random.permutation(4)[:2]]
-```
-
-### Addition
-
-You can add two `RaggedBuffer`s with the `+` operator if they have the same number of sequences, sequence lengths, and features. You can also add a `RaggedBuffer` where all sequences have a length of 1 to a `RaggedBuffer` with variable length sequences, broadcasting along each sequence.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-# Create ragged buffer with dimensions (3, [1, 3, 2], 1)
-rb3 = RaggedBufferI64(1)
-rb3.push(np.array([[0]], dtype=np.int64))
-rb3.push(np.array([[0], [1], [2]], dtype=np.int64))
-rb3.push(np.array([[0], [5]], dtype=np.int64))
-
-# Create ragged buffer with dimensions (3, [1, 1, 1], 1)
-rb4 = RaggedBufferI64.from_array(np.array([0, 3, 10], dtype=np.int64).reshape(3, 1, 1))
-
-# Add rb3 and rb4, broadcasting along the sequence dimension.
-rb5 = rb3 + rb4
-assert np.all(
-    rb5.as_array() == np.array([[0], [3], [4], [5], [10], [15]], dtype=np.int64)
-)
-```
-
-### Concatenation
-
-The `extend` method can be used to mutate a `RaggedBuffer` by appending another `RaggedBuffer` to it.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-
-rb1 = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
-rb2 = RaggedBufferF32.from_array(np.zeros((2, 5, 3), dtype=np.float32))
-rb1.extend(r2)
-assert rb1.size0() == 6
-```
-
-### Clear
-
-The `clear` method removes all elements from a `RaggedBuffer` without deallocating the underlying memory.
-
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-rb = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
-rb.clear()
-assert rb.size0() == 0
-```
-
-## License
-
-ENN Ragged Buffer dual-licensed under Apache-2.0 and MIT.
+# ENN Ragged Buffer
+
+[![Actions Status](https://github.com/entity-neural-network/ragged-buffer/workflows/Test/badge.svg)](https://github.com/entity-neural-network/ragged-buffer/actions)
+[![PyPI](https://img.shields.io/pypi/v/ragged-buffer.svg?style=flat-square)](https://pypi.org/project/ragged-buffer/)
+[![Discord](https://img.shields.io/discord/913497968701747270?style=flat-square)](https://discord.gg/SjVqhSW4Qf)
+
+This Python package implements an efficient `RaggedBuffer` datatype that is similar to
+a 3D numpy array, but which allows for variable sequence length in the second
+dimension. It was created primarily for use in [enn-trainer](https://github.com/entity-neural-network/enn-trainer) 
+and currently only supports a small selection of the numpy array methods.
+
+![Ragged Buffer](https://user-images.githubusercontent.com/12845088/143787823-c6a585de-aeda-429c-9824-f4b4a98e6cea.png)
+
+## User Guide
+
+Install the package with `pip install ragged-buffer`.
+The package currently supports three `RaggedBuffer` variants, `RaggedBufferF32`, `RaggedBufferI64`, and `RaggedBufferBool`.
+
+<!-- no toc -->
+- [Creating a RaggedBuffer](#creating-a-raggedbuffer)
+- [Get size](#get-size)
+- [Convert to numpy array](#convert-to-numpy-array)
+- [Indexing](#indexing)
+- [Addition](#addition)
+- [Concatenation](#concatentation)
+- [Clear](#clear)
+
+### Creating a RaggedBuffer
+
+There are three ways to create a `RaggedBuffer`:
+- `RaggedBufferF32(features: int)` creates an empty `RaggedBuffer` with the specified number of features.
+- `RaggedBufferF32.from_flattened(flattened: np.ndarray, lenghts: np.ndarray)` creates a `RaggedBuffer` from a flattened 2D numpy array and a 1D numpy array of lengths.
+- `RaggedBufferF32.from_array` creates a `RaggedBuffer` (with equal sequence lenghts) from a 3D numpy array.
+
+Creating an empty buffer and pushing each row:
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+# Create an empty RaggedBuffer with a feature size of 3
+buffer = RaggedBufferF32(3)
+# Push sequences with 3, 5, 0, and 1 elements
+buffer.push(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]], dtype=np.float32))
+buffer.push(np.array([[10, 11, 12], [13, 14, 15], [16, 17, 18], [19, 20, 21], [22, 23, 24]], dtype=np.float32))
+buffer.push(np.array([], dtype=np.float32))  # Alternative: `buffer.push_empty()`
+buffer.push(np.array([[25, 25, 27]], dtype=np.float32))
+```
+
+Creating a RaggedBuffer from a flat 2D numpy array which combines the first and second dimension,
+and an array of sequence lengths:
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+buffer = RaggedBufferF32.from_flattened(
+    np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12], [13, 14, 15], [16, 17, 18], [19, 20, 21], [22, 23, 24], [25, 25, 27]], dtype=np.float32),
+    np.array([3, 5, 0, 1], dtype=np.int64))
+)
+```
+
+Creating a RaggedBuffer from a 3D numpy array (all sequences have the same length):
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+buffer = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
+```
+
+### Get size
+
+The `size0`, `size1`, and `size2` methods return the number of sequences, the number of elements in a sequence, and the number of features respectively.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+buffer = RaggedBufferF32.from_flattened(
+    np.zeros((9, 64), dtype=np.float32),
+    np.array([3, 5, 0, 1], dtype=np.int64))
+)
+
+# Get size of the first/batch dimension.
+assert buffer.size0() == 10
+# Get size of individual sequences.
+assert buffer.size1(1) == 5
+assert buffer.size1(2) == 0
+# Get size of the last/feature dimension.
+assert buffer.size2() == 64
+```
+
+### Convert to numpy array
+
+`as_aray` converts a `RaggedBuffer` to a flat 2D numpy array that combines the first and second dimension.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferI64
+
+buffer = RaggedBufferI64(1)
+buffer.push(np.array([[1], [1], [1]], dtype=np.int64))
+buffer.push(np.array([[2], [2]], dtype=np.int64))
+assert np.all(buffer.as_array(), np.array([[1], [1], [1], [2], [2]], dtype=np.int64))
+```
+
+### Indexing
+
+You can index a `RaggedBuffer` with a single integer (returning a `RaggedBuffer` with a single sequence), or with a numpy array of integers selecting/permuting multiple sequences.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+# Create a new `RaggedBufferF32`
+buffer = RaggedBufferF32.from_flattened(
+    np.arange(0, 40, dtype=np.float32).reshape(10, 4),
+    np.array([3, 5, 0, 1], dtype=np.int64)
+)
+
+# Retrieve the first sequence.
+assert np.all(
+    buffer[0].as_array() ==
+    np.array([[0, 1, 2, 3], [4, 5, 6, 7], [8, 9, 10, 11]], dtype=np.float32)
+)
+
+# Get a RaggedBatch with 2 randomly selected sequences.
+buffer[np.random.permutation(4)[:2]]
+```
+
+### Addition
+
+You can add two `RaggedBuffer`s with the `+` operator if they have the same number of sequences, sequence lengths, and features. You can also add a `RaggedBuffer` where all sequences have a length of 1 to a `RaggedBuffer` with variable length sequences, broadcasting along each sequence.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+# Create ragged buffer with dimensions (3, [1, 3, 2], 1)
+rb3 = RaggedBufferI64(1)
+rb3.push(np.array([[0]], dtype=np.int64))
+rb3.push(np.array([[0], [1], [2]], dtype=np.int64))
+rb3.push(np.array([[0], [5]], dtype=np.int64))
+
+# Create ragged buffer with dimensions (3, [1, 1, 1], 1)
+rb4 = RaggedBufferI64.from_array(np.array([0, 3, 10], dtype=np.int64).reshape(3, 1, 1))
+
+# Add rb3 and rb4, broadcasting along the sequence dimension.
+rb5 = rb3 + rb4
+assert np.all(
+    rb5.as_array() == np.array([[0], [3], [4], [5], [10], [15]], dtype=np.int64)
+)
+```
+
+### Concatenation
+
+The `extend` method can be used to mutate a `RaggedBuffer` by appending another `RaggedBuffer` to it.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+
+rb1 = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
+rb2 = RaggedBufferF32.from_array(np.zeros((2, 5, 3), dtype=np.float32))
+rb1.extend(r2)
+assert rb1.size0() == 6
+```
+
+### Clear
+
+The `clear` method removes all elements from a `RaggedBuffer` without deallocating the underlying memory.
+
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+rb = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
+rb.clear()
+assert rb.size0() == 0
+```
+
+## License
+
+ENN Ragged Buffer dual-licensed under Apache-2.0 and MIT.
```

### Comparing `ragged_buffer-0.4.4/ragged_buffer/__init__.py` & `ragged_buffer-0.4.7/ragged_buffer/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import Any, Generic, List, Protocol, Type, TypeVar, Union, cast, overload
-from numpy.typing import NDArray
-import numpy as np
-
-from .ragged_buffer import (
-    RaggedBufferF32,
-    RaggedBufferI64,
-    RaggedBufferBool,
-    translate_rotate,
-)
-
-ScalarType = TypeVar("ScalarType", bound=np.generic)
-
-
-class RaggedBuffer(Generic[ScalarType]):
-    def __init__(self, features: int) -> None:
-        raise ValueError(
-            "RaggedBuffer is an abstract class, use RaggedBufferF32 or RaggedBufferI64"
-        )
-
-    @classmethod
-    def from_array(cls, x: NDArray[ScalarType]) -> "RaggedBuffer[ScalarType]":
-        if x.dtype == np.float32:
-            return RaggedBufferF32.from_array(x)
-        elif x.dtype == np.int64:
-            return RaggedBufferI64.from_array(x)
-        elif x.dtype == np.bool_:
-            return RaggedBufferBool.from_array(x)
-        else:
-            raise ValueError(
-                f"Unsupported dtype {x.dtype}. Only float32 and int64 are currently supported."
-            )
-
-    @classmethod
-    def from_flattened(
-        cls, flattened: NDArray[ScalarType], lengths: NDArray[np.int64]
-    ) -> "RaggedBuffer[ScalarType]":
-        if flattened.dtype == np.float32:
-            return RaggedBufferF32.from_flattened(flattened, lengths)
-        elif flattened.dtype == np.int64:
-            return RaggedBufferI64.from_flattened(flattened, lengths)
-        elif flattened.dtype == np.bool_:
-            return RaggedBufferBool.from_flattened(flattened, lengths)
-        else:
-            raise ValueError(
-                f"Unsupported dtype {flattened.dtype}. Only float32 and int64 are currently supported."
-            )
-
-
-def cat(
-    buffers: List[RaggedBuffer[ScalarType]], dim: int = 0
-) -> RaggedBuffer[ScalarType]:
-    if len(buffers) == 0:
-        raise ValueError("Can't concatenate an empty list of buffers")
-    else:
-        if isinstance(buffers[0], RaggedBufferF32):
-            return RaggedBufferF32.cat(buffers, dim)
-        elif isinstance(buffers[0], RaggedBufferI64):
-            return RaggedBufferI64.cat(buffers, dim)
-        elif isinstance(buffers[0], RaggedBufferBool):
-            return RaggedBufferBool.cat(buffers, dim)
-        else:
-            raise TypeError(f"Type {type(buffers[0])} is not a RaggedBuffer")
+from typing import Any, Generic, List, Protocol, Type, TypeVar, Union, cast, overload
+from numpy.typing import NDArray
+import numpy as np
+
+from .ragged_buffer import (
+    RaggedBufferF32,
+    RaggedBufferI64,
+    RaggedBufferBool,
+    translate_rotate,
+)
+
+ScalarType = TypeVar("ScalarType", bound=np.generic)
+
+
+class RaggedBuffer(Generic[ScalarType]):
+    def __init__(self, features: int) -> None:
+        raise ValueError(
+            "RaggedBuffer is an abstract class, use RaggedBufferF32 or RaggedBufferI64"
+        )
+
+    @classmethod
+    def from_array(cls, x: NDArray[ScalarType]) -> "RaggedBuffer[ScalarType]":
+        if x.dtype == np.float32:
+            return RaggedBufferF32.from_array(x)
+        elif x.dtype == np.int64:
+            return RaggedBufferI64.from_array(x)
+        elif x.dtype == np.bool_:
+            return RaggedBufferBool.from_array(x)
+        else:
+            raise ValueError(
+                f"Unsupported dtype {x.dtype}. Only float32 and int64 are currently supported."
+            )
+
+    @classmethod
+    def from_flattened(
+        cls, flattened: NDArray[ScalarType], lengths: NDArray[np.int64]
+    ) -> "RaggedBuffer[ScalarType]":
+        if flattened.dtype == np.float32:
+            return RaggedBufferF32.from_flattened(flattened, lengths)
+        elif flattened.dtype == np.int64:
+            return RaggedBufferI64.from_flattened(flattened, lengths)
+        elif flattened.dtype == np.bool_:
+            return RaggedBufferBool.from_flattened(flattened, lengths)
+        else:
+            raise ValueError(
+                f"Unsupported dtype {flattened.dtype}. Only float32 and int64 are currently supported."
+            )
+
+
+def cat(
+    buffers: List[RaggedBuffer[ScalarType]], dim: int = 0
+) -> RaggedBuffer[ScalarType]:
+    if len(buffers) == 0:
+        raise ValueError("Can't concatenate an empty list of buffers")
+    else:
+        if isinstance(buffers[0], RaggedBufferF32):
+            return RaggedBufferF32.cat(buffers, dim)
+        elif isinstance(buffers[0], RaggedBufferI64):
+            return RaggedBufferI64.cat(buffers, dim)
+        elif isinstance(buffers[0], RaggedBufferBool):
+            return RaggedBufferBool.cat(buffers, dim)
+        else:
+            raise TypeError(f"Type {type(buffers[0])} is not a RaggedBuffer")
```

### Comparing `ragged_buffer-0.4.4/ragged_buffer/__init__.pyi` & `ragged_buffer-0.4.7/ragged_buffer/__init__.pyi`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import numpy as np
-from typing import Any, Generic, Tuple, TypeVar, Union, overload, List, Optional
-from numpy.typing import NDArray
-import numpy as np
-
-ScalarType = TypeVar("ScalarType", bound=np.generic)
-
-class RaggedBuffer(Generic[ScalarType]):
-    def __init__(self, features: int) -> None: ...
-    @classmethod
-    def from_array(cls, x: NDArray[ScalarType]) -> RaggedBuffer[ScalarType]: ...
-    @classmethod
-    def from_flattened(
-        cls, flattened: NDArray[ScalarType], lengths: NDArray[np.int64]
-    ) -> RaggedBuffer[ScalarType]: ...
-    def push(self, x: NDArray[ScalarType]) -> None: ...
-    def push_empty(self) -> None: ...
-    def extend(self, x: RaggedBuffer[ScalarType]) -> None: ...
-    def as_array(self) -> NDArray[ScalarType]: ...
-    def size0(self) -> int: ...
-    @overload
-    def size1(self) -> NDArray[np.int64]: ...
-    @overload
-    def size1(self, i: int) -> int: ...
-    def size2(self) -> int: ...
-    @overload
-    def __add__(self, other: RaggedBuffer[ScalarType]) -> RaggedBuffer[ScalarType]: ...
-    @overload
-    def __add__(self, other: int) -> RaggedBuffer[ScalarType]: ...
-    @overload
-    def __add__(self, other: float) -> RaggedBuffer[np.float32]: ...
-    @overload
-    def __mul__(self, other: RaggedBuffer[ScalarType]) -> RaggedBuffer[ScalarType]: ...
-    @overload
-    def __mul__(self, other: int) -> RaggedBuffer[ScalarType]: ...
-    @overload
-    def __mul__(self, other: float) -> RaggedBuffer[np.float32]: ...
-    def __getitem__(
-        self,
-        i: Union[
-            int,
-            NDArray[np.int64],
-            Tuple[Union[int, List[int], slice, NDArray[np.int64]], ...],
-        ],
-    ) -> RaggedBuffer[ScalarType]: ...
-    def __eq__(self, other: Any) -> bool: ...
-    def __ne__(self, other: Any) -> bool: ...
-    def clear(self) -> None: ...
-    def indices(self, dim: int) -> RaggedBufferI64: ...
-    def flat_indices(self) -> RaggedBufferI64: ...
-    def padpack(
-        self,
-    ) -> Optional[Tuple[NDArray[np.int64], NDArray[np.float32], NDArray[np.int64]]]: ...
-    def __isub__(self, other: RaggedBuffer[ScalarType]) -> RaggedBuffer[ScalarType]: ...
-    def __len__(self) -> int: ...
-    def items(self) -> int: ...
-    def clone(self) -> RaggedBuffer[ScalarType]: ...
-    def materialize(self) -> RaggedBuffer[ScalarType]: ...
-
-RaggedBufferF32 = RaggedBuffer[np.float32]
-RaggedBufferI64 = RaggedBuffer[np.int64]
-RaggedBufferBool = RaggedBuffer[np.bool_]
-
-def cat(
-    buffers: List[RaggedBuffer[ScalarType]], dim: int = 0
-) -> RaggedBuffer[ScalarType]: ...
-def translate_rotate(
-    source: RaggedBuffer[np.float32],
-    translation: RaggedBuffer[np.float32],
-    rotation: RaggedBuffer[np.float32],
-) -> None: ...
+import numpy as np
+from typing import Any, Generic, Tuple, TypeVar, Union, overload, List, Optional
+from numpy.typing import NDArray
+import numpy as np
+
+ScalarType = TypeVar("ScalarType", bound=np.generic)
+
+class RaggedBuffer(Generic[ScalarType]):
+    def __init__(self, features: int) -> None: ...
+    @classmethod
+    def from_array(cls, x: NDArray[ScalarType]) -> RaggedBuffer[ScalarType]: ...
+    @classmethod
+    def from_flattened(
+        cls, flattened: NDArray[ScalarType], lengths: NDArray[np.int64]
+    ) -> RaggedBuffer[ScalarType]: ...
+    def push(self, x: NDArray[ScalarType]) -> None: ...
+    def push_empty(self) -> None: ...
+    def extend(self, x: RaggedBuffer[ScalarType]) -> None: ...
+    def as_array(self) -> NDArray[ScalarType]: ...
+    def size0(self) -> int: ...
+    @overload
+    def size1(self) -> NDArray[np.int64]: ...
+    @overload
+    def size1(self, i: int) -> int: ...
+    def size2(self) -> int: ...
+    @overload
+    def __add__(self, other: RaggedBuffer[ScalarType]) -> RaggedBuffer[ScalarType]: ...
+    @overload
+    def __add__(self, other: int) -> RaggedBuffer[ScalarType]: ...
+    @overload
+    def __add__(self, other: float) -> RaggedBuffer[np.float32]: ...
+    @overload
+    def __mul__(self, other: RaggedBuffer[ScalarType]) -> RaggedBuffer[ScalarType]: ...
+    @overload
+    def __mul__(self, other: int) -> RaggedBuffer[ScalarType]: ...
+    @overload
+    def __mul__(self, other: float) -> RaggedBuffer[np.float32]: ...
+    def __getitem__(
+        self,
+        i: Union[
+            int,
+            NDArray[np.int64],
+            Tuple[Union[int, List[int], slice, NDArray[np.int64]], ...],
+        ],
+    ) -> RaggedBuffer[ScalarType]: ...
+    def __eq__(self, other: Any) -> bool: ...
+    def __ne__(self, other: Any) -> bool: ...
+    def clear(self) -> None: ...
+    def indices(self, dim: int) -> RaggedBufferI64: ...
+    def flat_indices(self) -> RaggedBufferI64: ...
+    def padpack(
+        self,
+    ) -> Optional[Tuple[NDArray[np.int64], NDArray[np.float32], NDArray[np.int64]]]: ...
+    def __isub__(self, other: RaggedBuffer[ScalarType]) -> RaggedBuffer[ScalarType]: ...
+    def __len__(self) -> int: ...
+    def items(self) -> int: ...
+    def clone(self) -> RaggedBuffer[ScalarType]: ...
+    def materialize(self) -> RaggedBuffer[ScalarType]: ...
+
+RaggedBufferF32 = RaggedBuffer[np.float32]
+RaggedBufferI64 = RaggedBuffer[np.int64]
+RaggedBufferBool = RaggedBuffer[np.bool_]
+
+def cat(
+    buffers: List[RaggedBuffer[ScalarType]], dim: int = 0
+) -> RaggedBuffer[ScalarType]: ...
+def translate_rotate(
+    source: RaggedBuffer[np.float32],
+    translation: RaggedBuffer[np.float32],
+    rotation: RaggedBuffer[np.float32],
+) -> None: ...
```

### Comparing `ragged_buffer-0.4.4/src/lib.rs` & `ragged_buffer-0.4.7/src/lib.rs`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#[cfg(feature = "python")]
-use pyo3::prelude::*;
-#[cfg(feature = "python")]
-use pyo3::wrap_pyfunction;
-#[cfg(feature = "python")]
-pub mod monomorphs;
-
-pub mod ragged_buffer;
-
-#[cfg(feature = "python")]
-pub mod ragged_buffer_view;
-
-#[cfg(feature = "python")]
-#[pymodule]
-fn ragged_buffer(_py: Python, m: &PyModule) -> PyResult<()> {
-    // New exports also have to be added to __init__.py
-    m.add_class::<monomorphs::RaggedBufferF32>()?;
-    m.add_class::<monomorphs::RaggedBufferI64>()?;
-    m.add_class::<monomorphs::RaggedBufferBool>()?;
-    m.add_function(wrap_pyfunction!(translate_rotate, m)?)?;
-    Ok(())
-}
-
-#[cfg(feature = "python")]
-#[pyfunction]
-fn translate_rotate(
-    source: &monomorphs::RaggedBufferF32,
-    translation: monomorphs::RaggedBufferF32,
-    rotation: monomorphs::RaggedBufferF32,
-) -> PyResult<()> {
-    ragged_buffer_view::translate_rotate(&source.0, &translation.0, &rotation.0)
-}
+#[cfg(feature = "python")]
+use pyo3::prelude::*;
+#[cfg(feature = "python")]
+use pyo3::wrap_pyfunction;
+#[cfg(feature = "python")]
+pub mod monomorphs;
+
+pub mod ragged_buffer;
+
+#[cfg(feature = "python")]
+pub mod ragged_buffer_view;
+
+#[cfg(feature = "python")]
+#[pymodule]
+fn ragged_buffer(_py: Python, m: &PyModule) -> PyResult<()> {
+    // New exports also have to be added to __init__.py
+    m.add_class::<monomorphs::RaggedBufferF32>()?;
+    m.add_class::<monomorphs::RaggedBufferI64>()?;
+    m.add_class::<monomorphs::RaggedBufferBool>()?;
+    m.add_function(wrap_pyfunction!(translate_rotate, m)?)?;
+    Ok(())
+}
+
+#[cfg(feature = "python")]
+#[pyfunction]
+fn translate_rotate(
+    source: &monomorphs::RaggedBufferF32,
+    translation: monomorphs::RaggedBufferF32,
+    rotation: monomorphs::RaggedBufferF32,
+) -> PyResult<()> {
+    ragged_buffer_view::translate_rotate(&source.0, &translation.0, &rotation.0)
+}
```

### Comparing `ragged_buffer-0.4.4/src/monomorphs/bool.rs` & `ragged_buffer-0.4.7/src/monomorphs/f32.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-use numpy::{PyReadonlyArray1, PyReadonlyArray2, PyReadonlyArray3, PyReadonlyArrayDyn, ToPyArray};
-use pyo3::basic::CompareOp;
-use pyo3::prelude::*;
-use pyo3::types::PyType;
-
-use crate::monomorphs::RaggedBufferI64;
-use crate::ragged_buffer_view::RaggedBufferView;
-
-use super::{Index, MultiIndex, PadpackResult};
-
-#[pyclass]
-#[derive(Clone)]
-pub struct RaggedBufferBool(pub RaggedBufferView<bool>);
-
-#[pymethods]
-impl RaggedBufferBool {
-    #[new]
-    pub fn new(features: usize) -> Self {
-        RaggedBufferBool(RaggedBufferView::new(features))
-    }
-    #[classmethod]
-    fn from_array(_cls: &PyType, array: PyReadonlyArray3<bool>) -> Self {
-        RaggedBufferBool(RaggedBufferView::from_array(array))
-    }
-    #[classmethod]
-    fn from_flattened(
-        _cls: &PyType,
-        flattened: PyReadonlyArray2<bool>,
-        lengths: PyReadonlyArray1<i64>,
-    ) -> PyResult<Self> {
-        Ok(RaggedBufferBool(RaggedBufferView::from_flattened(
-            flattened, lengths,
-        )?))
-    }
-    fn push(&mut self, items: PyReadonlyArrayDyn<bool>) -> PyResult<()> {
-        if items.ndim() == 1 && items.len() == 0 {
-            self.0.push_empty()
-        } else if items.ndim() == 2 {
-            self.0.push(
-                &items
-                    .reshape((items.shape()[0], items.shape()[1]))?
-                    .readonly(),
-            )
-        } else {
-            Err(pyo3::exceptions::PyValueError::new_err(
-                "Expected 2 dimensional array",
-            ))
-        }
-    }
-    fn push_empty(&mut self) -> PyResult<()> {
-        self.0.push_empty()
-    }
-
-    fn clear(&mut self) -> PyResult<()> {
-        self.0.clear()
-    }
-
-    fn as_array<'a>(
-        &self,
-        py: Python<'a>,
-    ) -> PyResult<&'a numpy::PyArray<bool, numpy::ndarray::Dim<[usize; 2]>>> {
-        self.0.as_array(py)
-    }
-
-    fn extend(&mut self, other: &RaggedBufferBool) -> PyResult<()> {
-        self.0.extend(&other.0)
-    }
-    fn size0(&self) -> usize {
-        self.0.size0()
-    }
-    fn size1(&mut self, py: Python, i: Option<usize>) -> PyResult<PyObject> {
-        match i {
-            Some(i) => self.0.size1(i).map(|s| s.into_py(py)),
-            None => self.0.lengths(py).map(|ok| ok.into_py(py)),
-        }
-    }
-    fn size2(&self) -> usize {
-        self.0.size2()
-    }
-    fn indices(&mut self, dim: usize) -> PyResult<RaggedBufferI64> {
-        Ok(RaggedBufferI64(self.0.indices(dim)?))
-    }
-    fn flat_indices(&mut self) -> PyResult<RaggedBufferI64> {
-        Ok(RaggedBufferI64(self.0.flat_indices()?))
-    }
-    #[classmethod]
-    fn cat(_cls: &PyType, buffers: Vec<PyRef<RaggedBufferBool>>, dim: usize) -> PyResult<Self> {
-        Ok(RaggedBufferBool(RaggedBufferView::cat(
-            &buffers.iter().map(|b| &b.0).collect::<Vec<_>>(),
-            dim,
-        )?))
-    }
-    #[allow(clippy::type_complexity)]
-    fn padpack<'a>(&mut self, py: Python<'a>) -> PadpackResult<'a> {
-        match self.0.padpack()? {
-            Some((padbpack_index, padpack_batch, padpack_inverse_index, dims)) => Ok(Some((
-                padbpack_index.to_pyarray(py).reshape(dims)?,
-                padpack_batch.to_pyarray(py).reshape(dims)?,
-                padpack_inverse_index
-                    .to_pyarray(py)
-                    .reshape(self.0.len()?)?,
-            ))),
-            _ => Ok(None),
-        }
-    }
-    fn items(&mut self) -> PyResult<usize> {
-        self.0.items()
-    }
-    fn clone(&self) -> Self {
-        RaggedBufferBool(self.0.deepclone())
-    }
-    fn materialize(&self) -> Self {
-        RaggedBufferBool(self.0.materialize())
-    }
-    fn __str__(&self) -> PyResult<String> {
-        self.0.__str__()
-    }
-
-    fn __repr__(&self) -> PyResult<String> {
-        self.0.__str__()
-    }
-
-    fn __richcmp__(&self, other: RaggedBufferBool, op: CompareOp) -> PyResult<bool> {
-        match op {
-            CompareOp::Eq => Ok(self.0 == other.0),
-            CompareOp::Ne => Ok(self.0 != other.0),
-            _ => Err(pyo3::exceptions::PyTypeError::new_err(
-                "Only == and != are supported",
-            )),
-        }
-    }
-
-    // Is substituted for #[cfg(any())] for bool.rs to omit method
-    #[cfg(any())]
-    fn __add__(
-        lhs: PyRef<RaggedBufferBool>,
-        rhs: RaggedBufferBoolOrBool,
-    ) -> PyResult<RaggedBufferBool> {
-        match rhs {
-            RaggedBufferBoolOrBool::RB(rhs) => Ok(RaggedBufferBool(
-                lhs.0.binop::<crate::ragged_buffer::BinOpAdd>(&rhs.0)?,
-            )),
-            RaggedBufferBoolOrBool::Scalar(rhs) => Ok(RaggedBufferBool(
-                lhs.0.op_scalar::<crate::ragged_buffer::BinOpAdd>(rhs)?,
-            )),
-        }
-    }
-
-    #[cfg(any())]
-    fn __mul__(
-        lhs: PyRef<RaggedBufferBool>,
-        rhs: RaggedBufferBoolOrBool,
-    ) -> PyResult<RaggedBufferBool> {
-        match rhs {
-            RaggedBufferBoolOrBool::RB(rhs) => Ok(RaggedBufferBool(
-                lhs.0.binop::<crate::ragged_buffer::BinOpMul>(&rhs.0)?,
-            )),
-            RaggedBufferBoolOrBool::Scalar(rhs) => Ok(RaggedBufferBool(
-                lhs.0.op_scalar::<crate::ragged_buffer::BinOpMul>(rhs)?,
-            )),
-        }
-    }
-
-    #[cfg(any())]
-    fn __isub__(&mut self, rhs: RaggedBufferBool) -> PyResult<()> {
-        self.0.binop_mut::<crate::ragged_buffer::BinOpSub>(&rhs.0)
-    }
-
-    fn __getitem__(&self, index: MultiIndex) -> PyResult<RaggedBufferBool> {
-        match index {
-            MultiIndex::Index1(index) => match index {
-                Index::PermutationNP(indices) => Ok(RaggedBufferBool(self.0.swizzle(indices)?)),
-                Index::Permutation(_indices) => panic!("oh no"), //Ok(RaggedBufferBool(self.0.swizzle(indices)?)),
-                Index::Int(i) => Ok(RaggedBufferBool(self.0.get_sequence(i)?)),
-                Index::Slice(slice) => panic!("{:?}", slice),
-            },
-            MultiIndex::Index3((i0, i1, i2)) => Ok(RaggedBufferBool(Python::with_gil(|py| {
-                self.0.get_slice(py, i0, i1, i2)
-            })?)),
-            x => panic!("{:?}", x),
-        }
-    }
-    fn __len__(&self) -> PyResult<usize> {
-        self.0.len()
-    }
-}
-
-#[derive(FromPyObject)]
-pub enum RaggedBufferBoolOrBool<'p> {
-    RB(PyRef<'p, RaggedBufferBool>),
-    Scalar(bool),
-}
+use numpy::{PyReadonlyArray1, PyReadonlyArray2, PyReadonlyArray3, PyReadonlyArrayDyn, ToPyArray};
+use pyo3::basic::CompareOp;
+use pyo3::prelude::*;
+use pyo3::types::PyType;
+
+use crate::monomorphs::RaggedBufferI64;
+use crate::ragged_buffer_view::RaggedBufferView;
+
+use super::{Index, MultiIndex, PadpackResult};
+
+#[pyclass]
+#[derive(Clone)]
+pub struct RaggedBufferF32(pub RaggedBufferView<f32>);
+
+#[pymethods]
+impl RaggedBufferF32 {
+    #[new]
+    pub fn new(features: usize) -> Self {
+        RaggedBufferF32(RaggedBufferView::new(features))
+    }
+    #[classmethod]
+    fn from_array(_cls: &PyType, array: PyReadonlyArray3<f32>) -> Self {
+        RaggedBufferF32(RaggedBufferView::from_array(array))
+    }
+    #[classmethod]
+    fn from_flattened(
+        _cls: &PyType,
+        flattened: PyReadonlyArray2<f32>,
+        lengths: PyReadonlyArray1<i64>,
+    ) -> PyResult<Self> {
+        Ok(RaggedBufferF32(RaggedBufferView::from_flattened(
+            flattened, lengths,
+        )?))
+    }
+    fn push(&mut self, items: PyReadonlyArrayDyn<f32>) -> PyResult<()> {
+        if items.ndim() == 1 && items.len() == 0 {
+            self.0.push_empty()
+        } else if items.ndim() == 2 {
+            self.0.push(
+                &items
+                    .reshape((items.shape()[0], items.shape()[1]))?
+                    .readonly(),
+            )
+        } else {
+            Err(pyo3::exceptions::PyValueError::new_err(
+                "Expected 2 dimensional array",
+            ))
+        }
+    }
+    fn push_empty(&mut self) -> PyResult<()> {
+        self.0.push_empty()
+    }
+
+    fn clear(&mut self) -> PyResult<()> {
+        self.0.clear()
+    }
+
+    fn as_array<'a>(
+        &self,
+        py: Python<'a>,
+    ) -> PyResult<&'a numpy::PyArray<f32, numpy::ndarray::Dim<[usize; 2]>>> {
+        self.0.as_array(py)
+    }
+
+    fn extend(&mut self, other: &RaggedBufferF32) -> PyResult<()> {
+        self.0.extend(&other.0)
+    }
+    fn size0(&self) -> usize {
+        self.0.size0()
+    }
+    fn size1(&mut self, py: Python, i: Option<usize>) -> PyResult<PyObject> {
+        match i {
+            Some(i) => self.0.size1(i).map(|s| s.into_py(py)),
+            None => self.0.lengths(py).map(|ok| ok.into_py(py)),
+        }
+    }
+    fn size2(&self) -> usize {
+        self.0.size2()
+    }
+    fn indices(&mut self, dim: usize) -> PyResult<RaggedBufferI64> {
+        Ok(RaggedBufferI64(self.0.indices(dim)?))
+    }
+    fn flat_indices(&mut self) -> PyResult<RaggedBufferI64> {
+        Ok(RaggedBufferI64(self.0.flat_indices()?))
+    }
+    #[classmethod]
+    fn cat(_cls: &PyType, buffers: Vec<PyRef<RaggedBufferF32>>, dim: usize) -> PyResult<Self> {
+        Ok(RaggedBufferF32(RaggedBufferView::cat(
+            &buffers.iter().map(|b| &b.0).collect::<Vec<_>>(),
+            dim,
+        )?))
+    }
+    #[allow(clippy::type_complexity)]
+    fn padpack<'a>(&mut self, py: Python<'a>) -> PadpackResult<'a> {
+        match self.0.padpack()? {
+            Some((padbpack_index, padpack_batch, padpack_inverse_index, dims)) => Ok(Some((
+                padbpack_index.to_pyarray(py).reshape(dims)?,
+                padpack_batch.to_pyarray(py).reshape(dims)?,
+                padpack_inverse_index
+                    .to_pyarray(py)
+                    .reshape(self.0.len()?)?,
+            ))),
+            _ => Ok(None),
+        }
+    }
+    fn items(&mut self) -> PyResult<usize> {
+        self.0.items()
+    }
+    fn clone(&self) -> Self {
+        RaggedBufferF32(self.0.deepclone())
+    }
+    fn materialize(&self) -> Self {
+        RaggedBufferF32(self.0.materialize())
+    }
+    fn __str__(&self) -> PyResult<String> {
+        self.0.__str__()
+    }
+
+    fn __repr__(&self) -> PyResult<String> {
+        self.0.__str__()
+    }
+
+    fn __richcmp__(&self, other: RaggedBufferF32, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Eq => Ok(self.0 == other.0),
+            CompareOp::Ne => Ok(self.0 != other.0),
+            _ => Err(pyo3::exceptions::PyTypeError::new_err(
+                "Only == and != are supported",
+            )),
+        }
+    }
+
+    // Is substituted for #[cfg(any())] for bool.rs to omit method
+    #[cfg(all())]
+    fn __add__(
+        lhs: PyRef<RaggedBufferF32>,
+        rhs: RaggedBufferF32OrF32,
+    ) -> PyResult<RaggedBufferF32> {
+        match rhs {
+            RaggedBufferF32OrF32::RB(rhs) => Ok(RaggedBufferF32(
+                lhs.0.binop::<crate::ragged_buffer::BinOpAdd>(&rhs.0)?,
+            )),
+            RaggedBufferF32OrF32::Scalar(rhs) => Ok(RaggedBufferF32(
+                lhs.0.op_scalar::<crate::ragged_buffer::BinOpAdd>(rhs)?,
+            )),
+        }
+    }
+
+    #[cfg(all())]
+    fn __mul__(
+        lhs: PyRef<RaggedBufferF32>,
+        rhs: RaggedBufferF32OrF32,
+    ) -> PyResult<RaggedBufferF32> {
+        match rhs {
+            RaggedBufferF32OrF32::RB(rhs) => Ok(RaggedBufferF32(
+                lhs.0.binop::<crate::ragged_buffer::BinOpMul>(&rhs.0)?,
+            )),
+            RaggedBufferF32OrF32::Scalar(rhs) => Ok(RaggedBufferF32(
+                lhs.0.op_scalar::<crate::ragged_buffer::BinOpMul>(rhs)?,
+            )),
+        }
+    }
+
+    #[cfg(all())]
+    fn __isub__(&mut self, rhs: RaggedBufferF32) -> PyResult<()> {
+        self.0.binop_mut::<crate::ragged_buffer::BinOpSub>(&rhs.0)
+    }
+
+    fn __getitem__(&self, index: MultiIndex) -> PyResult<RaggedBufferF32> {
+        match index {
+            MultiIndex::Index1(index) => match index {
+                Index::PermutationNP(indices) => Ok(RaggedBufferF32(self.0.swizzle(indices)?)),
+                Index::Permutation(indices) => Ok(RaggedBufferF32(self.0.swizzle_usize(&indices)?)),
+                Index::Int(i) => Ok(RaggedBufferF32(self.0.get_sequence(i)?)),
+                Index::Slice(slice) => panic!("{:?}", slice),
+            },
+            MultiIndex::Index3((i0, i1, i2)) => Ok(RaggedBufferF32(Python::with_gil(|py| {
+                self.0.get_slice(py, i0, i1, i2)
+            })?)),
+            x => panic!("{:?}", x),
+        }
+    }
+    fn __len__(&self) -> PyResult<usize> {
+        self.0.len()
+    }
+}
+
+#[derive(FromPyObject)]
+pub enum RaggedBufferF32OrF32<'p> {
+    RB(PyRef<'p, RaggedBufferF32>),
+    Scalar(f32),
+}
```

### Comparing `ragged_buffer-0.4.4/src/monomorphs/i64.rs` & `ragged_buffer-0.4.7/src/monomorphs/i64.rs`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-use numpy::{PyReadonlyArray1, PyReadonlyArray2, PyReadonlyArray3, PyReadonlyArrayDyn, ToPyArray};
-use pyo3::basic::CompareOp;
-use pyo3::prelude::*;
-use pyo3::types::PyType;
-
-use crate::ragged_buffer_view::RaggedBufferView;
-
-use super::{Index, MultiIndex, PadpackResult};
-
-#[pyclass]
-#[derive(Clone)]
-pub struct RaggedBufferI64(pub RaggedBufferView<i64>);
-
-#[pymethods]
-impl RaggedBufferI64 {
-    #[new]
-    pub fn new(features: usize) -> Self {
-        RaggedBufferI64(RaggedBufferView::new(features))
-    }
-    #[classmethod]
-    fn from_array(_cls: &PyType, array: PyReadonlyArray3<i64>) -> Self {
-        RaggedBufferI64(RaggedBufferView::from_array(array))
-    }
-    #[classmethod]
-    fn from_flattened(
-        _cls: &PyType,
-        flattened: PyReadonlyArray2<i64>,
-        lengths: PyReadonlyArray1<i64>,
-    ) -> PyResult<Self> {
-        Ok(RaggedBufferI64(RaggedBufferView::from_flattened(
-            flattened, lengths,
-        )?))
-    }
-    fn push(&mut self, items: PyReadonlyArrayDyn<i64>) -> PyResult<()> {
-        if items.ndim() == 1 && items.len() == 0 {
-            self.0.push_empty()
-        } else if items.ndim() == 2 {
-            self.0.push(
-                &items
-                    .reshape((items.shape()[0], items.shape()[1]))?
-                    .readonly(),
-            )
-        } else {
-            Err(pyo3::exceptions::PyValueError::new_err(
-                "Expected 2 dimensional array",
-            ))
-        }
-    }
-    fn push_empty(&mut self) -> PyResult<()> {
-        self.0.push_empty()
-    }
-
-    fn clear(&mut self) -> PyResult<()> {
-        self.0.clear()
-    }
-
-    fn as_array<'a>(
-        &self,
-        py: Python<'a>,
-    ) -> PyResult<&'a numpy::PyArray<i64, numpy::ndarray::Dim<[usize; 2]>>> {
-        self.0.as_array(py)
-    }
-
-    fn extend(&mut self, other: &RaggedBufferI64) -> PyResult<()> {
-        self.0.extend(&other.0)
-    }
-    fn size0(&self) -> usize {
-        self.0.size0()
-    }
-    fn size1(&mut self, py: Python, i: Option<usize>) -> PyResult<PyObject> {
-        match i {
-            Some(i) => self.0.size1(i).map(|s| s.into_py(py)),
-            None => self.0.lengths(py).map(|ok| ok.into_py(py)),
-        }
-    }
-    fn size2(&self) -> usize {
-        self.0.size2()
-    }
-    fn indices(&mut self, dim: usize) -> PyResult<RaggedBufferI64> {
-        Ok(RaggedBufferI64(self.0.indices(dim)?))
-    }
-    fn flat_indices(&mut self) -> PyResult<RaggedBufferI64> {
-        Ok(RaggedBufferI64(self.0.flat_indices()?))
-    }
-    #[classmethod]
-    fn cat(_cls: &PyType, buffers: Vec<PyRef<RaggedBufferI64>>, dim: usize) -> PyResult<Self> {
-        Ok(RaggedBufferI64(RaggedBufferView::cat(
-            &buffers.iter().map(|b| &b.0).collect::<Vec<_>>(),
-            dim,
-        )?))
-    }
-    #[allow(clippy::type_complexity)]
-    fn padpack<'a>(&mut self, py: Python<'a>) -> PadpackResult<'a> {
-        match self.0.padpack()? {
-            Some((padbpack_index, padpack_batch, padpack_inverse_index, dims)) => Ok(Some((
-                padbpack_index.to_pyarray(py).reshape(dims)?,
-                padpack_batch.to_pyarray(py).reshape(dims)?,
-                padpack_inverse_index
-                    .to_pyarray(py)
-                    .reshape(self.0.len()?)?,
-            ))),
-            _ => Ok(None),
-        }
-    }
-    fn items(&mut self) -> PyResult<usize> {
-        self.0.items()
-    }
-    fn clone(&self) -> Self {
-        RaggedBufferI64(self.0.deepclone())
-    }
-    fn materialize(&self) -> Self {
-        RaggedBufferI64(self.0.materialize())
-    }
-    fn __str__(&self) -> PyResult<String> {
-        self.0.__str__()
-    }
-
-    fn __repr__(&self) -> PyResult<String> {
-        self.0.__str__()
-    }
-
-    fn __richcmp__(&self, other: RaggedBufferI64, op: CompareOp) -> PyResult<bool> {
-        match op {
-            CompareOp::Eq => Ok(self.0 == other.0),
-            CompareOp::Ne => Ok(self.0 != other.0),
-            _ => Err(pyo3::exceptions::PyTypeError::new_err(
-                "Only == and != are supported",
-            )),
-        }
-    }
-
-    // Is substituted for #[cfg(any())] for bool.rs to omit method
-    #[cfg(all())]
-    fn __add__(
-        lhs: PyRef<RaggedBufferI64>,
-        rhs: RaggedBufferI64OrI64,
-    ) -> PyResult<RaggedBufferI64> {
-        match rhs {
-            RaggedBufferI64OrI64::RB(rhs) => Ok(RaggedBufferI64(
-                lhs.0.binop::<crate::ragged_buffer::BinOpAdd>(&rhs.0)?,
-            )),
-            RaggedBufferI64OrI64::Scalar(rhs) => Ok(RaggedBufferI64(
-                lhs.0.op_scalar::<crate::ragged_buffer::BinOpAdd>(rhs)?,
-            )),
-        }
-    }
-
-    #[cfg(all())]
-    fn __mul__(
-        lhs: PyRef<RaggedBufferI64>,
-        rhs: RaggedBufferI64OrI64,
-    ) -> PyResult<RaggedBufferI64> {
-        match rhs {
-            RaggedBufferI64OrI64::RB(rhs) => Ok(RaggedBufferI64(
-                lhs.0.binop::<crate::ragged_buffer::BinOpMul>(&rhs.0)?,
-            )),
-            RaggedBufferI64OrI64::Scalar(rhs) => Ok(RaggedBufferI64(
-                lhs.0.op_scalar::<crate::ragged_buffer::BinOpMul>(rhs)?,
-            )),
-        }
-    }
-
-    #[cfg(all())]
-    fn __isub__(&mut self, rhs: RaggedBufferI64) -> PyResult<()> {
-        self.0.binop_mut::<crate::ragged_buffer::BinOpSub>(&rhs.0)
-    }
-
-    fn __getitem__(&self, index: MultiIndex) -> PyResult<RaggedBufferI64> {
-        match index {
-            MultiIndex::Index1(index) => match index {
-                Index::PermutationNP(indices) => Ok(RaggedBufferI64(self.0.swizzle(indices)?)),
-                Index::Permutation(_indices) => panic!("oh no"), //Ok(RaggedBufferI64(self.0.swizzle(indices)?)),
-                Index::Int(i) => Ok(RaggedBufferI64(self.0.get_sequence(i)?)),
-                Index::Slice(slice) => panic!("{:?}", slice),
-            },
-            MultiIndex::Index3((i0, i1, i2)) => Ok(RaggedBufferI64(Python::with_gil(|py| {
-                self.0.get_slice(py, i0, i1, i2)
-            })?)),
-            x => panic!("{:?}", x),
-        }
-    }
-    fn __len__(&self) -> PyResult<usize> {
-        self.0.len()
-    }
-}
-
-#[derive(FromPyObject)]
-pub enum RaggedBufferI64OrI64<'p> {
-    RB(PyRef<'p, RaggedBufferI64>),
-    Scalar(i64),
-}
+use numpy::{PyReadonlyArray1, PyReadonlyArray2, PyReadonlyArray3, PyReadonlyArrayDyn, ToPyArray};
+use pyo3::basic::CompareOp;
+use pyo3::prelude::*;
+use pyo3::types::PyType;
+
+use crate::ragged_buffer_view::RaggedBufferView;
+
+use super::{Index, MultiIndex, PadpackResult};
+
+#[pyclass]
+#[derive(Clone)]
+pub struct RaggedBufferI64(pub RaggedBufferView<i64>);
+
+#[pymethods]
+impl RaggedBufferI64 {
+    #[new]
+    pub fn new(features: usize) -> Self {
+        RaggedBufferI64(RaggedBufferView::new(features))
+    }
+    #[classmethod]
+    fn from_array(_cls: &PyType, array: PyReadonlyArray3<i64>) -> Self {
+        RaggedBufferI64(RaggedBufferView::from_array(array))
+    }
+    #[classmethod]
+    fn from_flattened(
+        _cls: &PyType,
+        flattened: PyReadonlyArray2<i64>,
+        lengths: PyReadonlyArray1<i64>,
+    ) -> PyResult<Self> {
+        Ok(RaggedBufferI64(RaggedBufferView::from_flattened(
+            flattened, lengths,
+        )?))
+    }
+    fn push(&mut self, items: PyReadonlyArrayDyn<i64>) -> PyResult<()> {
+        if items.ndim() == 1 && items.len() == 0 {
+            self.0.push_empty()
+        } else if items.ndim() == 2 {
+            self.0.push(
+                &items
+                    .reshape((items.shape()[0], items.shape()[1]))?
+                    .readonly(),
+            )
+        } else {
+            Err(pyo3::exceptions::PyValueError::new_err(
+                "Expected 2 dimensional array",
+            ))
+        }
+    }
+    fn push_empty(&mut self) -> PyResult<()> {
+        self.0.push_empty()
+    }
+
+    fn clear(&mut self) -> PyResult<()> {
+        self.0.clear()
+    }
+
+    fn as_array<'a>(
+        &self,
+        py: Python<'a>,
+    ) -> PyResult<&'a numpy::PyArray<i64, numpy::ndarray::Dim<[usize; 2]>>> {
+        self.0.as_array(py)
+    }
+
+    fn extend(&mut self, other: &RaggedBufferI64) -> PyResult<()> {
+        self.0.extend(&other.0)
+    }
+    fn size0(&self) -> usize {
+        self.0.size0()
+    }
+    fn size1(&mut self, py: Python, i: Option<usize>) -> PyResult<PyObject> {
+        match i {
+            Some(i) => self.0.size1(i).map(|s| s.into_py(py)),
+            None => self.0.lengths(py).map(|ok| ok.into_py(py)),
+        }
+    }
+    fn size2(&self) -> usize {
+        self.0.size2()
+    }
+    fn indices(&mut self, dim: usize) -> PyResult<RaggedBufferI64> {
+        Ok(RaggedBufferI64(self.0.indices(dim)?))
+    }
+    fn flat_indices(&mut self) -> PyResult<RaggedBufferI64> {
+        Ok(RaggedBufferI64(self.0.flat_indices()?))
+    }
+    #[classmethod]
+    fn cat(_cls: &PyType, buffers: Vec<PyRef<RaggedBufferI64>>, dim: usize) -> PyResult<Self> {
+        Ok(RaggedBufferI64(RaggedBufferView::cat(
+            &buffers.iter().map(|b| &b.0).collect::<Vec<_>>(),
+            dim,
+        )?))
+    }
+    #[allow(clippy::type_complexity)]
+    fn padpack<'a>(&mut self, py: Python<'a>) -> PadpackResult<'a> {
+        match self.0.padpack()? {
+            Some((padbpack_index, padpack_batch, padpack_inverse_index, dims)) => Ok(Some((
+                padbpack_index.to_pyarray(py).reshape(dims)?,
+                padpack_batch.to_pyarray(py).reshape(dims)?,
+                padpack_inverse_index
+                    .to_pyarray(py)
+                    .reshape(self.0.len()?)?,
+            ))),
+            _ => Ok(None),
+        }
+    }
+    fn items(&mut self) -> PyResult<usize> {
+        self.0.items()
+    }
+    fn clone(&self) -> Self {
+        RaggedBufferI64(self.0.deepclone())
+    }
+    fn materialize(&self) -> Self {
+        RaggedBufferI64(self.0.materialize())
+    }
+    fn __str__(&self) -> PyResult<String> {
+        self.0.__str__()
+    }
+
+    fn __repr__(&self) -> PyResult<String> {
+        self.0.__str__()
+    }
+
+    fn __richcmp__(&self, other: RaggedBufferI64, op: CompareOp) -> PyResult<bool> {
+        match op {
+            CompareOp::Eq => Ok(self.0 == other.0),
+            CompareOp::Ne => Ok(self.0 != other.0),
+            _ => Err(pyo3::exceptions::PyTypeError::new_err(
+                "Only == and != are supported",
+            )),
+        }
+    }
+
+    // Is substituted for #[cfg(any())] for bool.rs to omit method
+    #[cfg(all())]
+    fn __add__(
+        lhs: PyRef<RaggedBufferI64>,
+        rhs: RaggedBufferI64OrI64,
+    ) -> PyResult<RaggedBufferI64> {
+        match rhs {
+            RaggedBufferI64OrI64::RB(rhs) => Ok(RaggedBufferI64(
+                lhs.0.binop::<crate::ragged_buffer::BinOpAdd>(&rhs.0)?,
+            )),
+            RaggedBufferI64OrI64::Scalar(rhs) => Ok(RaggedBufferI64(
+                lhs.0.op_scalar::<crate::ragged_buffer::BinOpAdd>(rhs)?,
+            )),
+        }
+    }
+
+    #[cfg(all())]
+    fn __mul__(
+        lhs: PyRef<RaggedBufferI64>,
+        rhs: RaggedBufferI64OrI64,
+    ) -> PyResult<RaggedBufferI64> {
+        match rhs {
+            RaggedBufferI64OrI64::RB(rhs) => Ok(RaggedBufferI64(
+                lhs.0.binop::<crate::ragged_buffer::BinOpMul>(&rhs.0)?,
+            )),
+            RaggedBufferI64OrI64::Scalar(rhs) => Ok(RaggedBufferI64(
+                lhs.0.op_scalar::<crate::ragged_buffer::BinOpMul>(rhs)?,
+            )),
+        }
+    }
+
+    #[cfg(all())]
+    fn __isub__(&mut self, rhs: RaggedBufferI64) -> PyResult<()> {
+        self.0.binop_mut::<crate::ragged_buffer::BinOpSub>(&rhs.0)
+    }
+
+    fn __getitem__(&self, index: MultiIndex) -> PyResult<RaggedBufferI64> {
+        match index {
+            MultiIndex::Index1(index) => match index {
+                Index::PermutationNP(indices) => Ok(RaggedBufferI64(self.0.swizzle(indices)?)),
+                Index::Permutation(_indices) => panic!("oh no"), //Ok(RaggedBufferI64(self.0.swizzle(indices)?)),
+                Index::Int(i) => Ok(RaggedBufferI64(self.0.get_sequence(i)?)),
+                Index::Slice(slice) => panic!("{:?}", slice),
+            },
+            MultiIndex::Index3((i0, i1, i2)) => Ok(RaggedBufferI64(Python::with_gil(|py| {
+                self.0.get_slice(py, i0, i1, i2)
+            })?)),
+            x => panic!("{:?}", x),
+        }
+    }
+    fn __len__(&self) -> PyResult<usize> {
+        self.0.len()
+    }
+}
+
+#[derive(FromPyObject)]
+pub enum RaggedBufferI64OrI64<'p> {
+    RB(PyRef<'p, RaggedBufferI64>),
+    Scalar(i64),
+}
```

### Comparing `ragged_buffer-0.4.4/src/ragged_buffer.rs` & `ragged_buffer-0.4.7/src/ragged_buffer.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,626 +1,629 @@
-use std::cmp::Ordering;
-use std::collections::{binary_heap, BinaryHeap};
-use std::fmt::{Display, Write};
-use std::ops::{Add, Mul, Range, Sub};
-
-use ndarray::{ArrayView1, ArrayView2, ArrayView3};
-
-#[derive(Debug)]
-pub enum Error {
-    Generic(String),
-}
-
-impl Error {
-    fn generic<S: Into<String>>(s: S) -> Self {
-        Self::Generic(s.into())
-    }
-}
-
-pub type Result<T> = std::result::Result<T, Error>;
-
-#[derive(Clone, PartialEq, Eq, Hash, Debug)]
-pub struct RaggedBuffer<T> {
-    pub data: Vec<T>,
-    // Each element of `subarrays` gives the start/end index of the items within that subarray (step size 1).
-    // The start index of the data of an item is obtained by multiplying its index by `features`.
-    pub subarrays: Vec<Range<usize>>,
-    pub features: usize,
-    // equal to data.len() / features
-    pub items: usize,
-}
-
-pub trait BinOp<T> {
-    fn op(lhs: T, rhs: T) -> T;
-}
-
-pub struct BinOpAdd;
-
-impl<T: Add<T, Output = T>> BinOp<T> for BinOpAdd {
-    #[inline]
-    fn op(lhs: T, rhs: T) -> T {
-        lhs + rhs
-    }
-}
-
-pub struct BinOpSub;
-
-impl<T: Sub<T, Output = T>> BinOp<T> for BinOpSub {
-    #[inline]
-    fn op(lhs: T, rhs: T) -> T {
-        lhs - rhs
-    }
-}
-
-pub struct BinOpMul;
-
-impl<T: Mul<T, Output = T>> BinOp<T> for BinOpMul {
-    #[inline]
-    fn op(lhs: T, rhs: T) -> T {
-        lhs * rhs
-    }
-}
-
-impl<T: Copy + Display + std::fmt::Debug> RaggedBuffer<T> {
-    pub fn new(features: usize) -> Self {
-        RaggedBuffer {
-            data: Vec::new(),
-            subarrays: Vec::new(),
-            features,
-            items: 0,
-        }
-    }
-
-    pub fn from_array(data: ArrayView3<T>) -> Self {
-        let features = data.shape()[2];
-        RaggedBuffer {
-            data: data.iter().cloned().collect(),
-            subarrays: (0..data.shape()[0])
-                .map(|i| i * data.shape()[1]..(i + 1) * data.shape()[1])
-                .collect(),
-            features,
-            items: data.shape()[0] * data.shape()[1],
-        }
-    }
-
-    pub fn from_flattened(data: ArrayView2<T>, lengths: ArrayView1<i64>) -> Result<Self> {
-        let features = data.shape()[1];
-        let mut subarrays = Vec::new();
-        let mut item = 0;
-        for len in lengths.iter().cloned() {
-            subarrays.push(item..(item + len as usize));
-            item += len as usize;
-        }
-        if item != data.shape()[0] {
-            Err(Error::generic(format!(
-                "Lengths array specifies {} items, but data array has {} items",
-                item,
-                data.shape()[0]
-            )))
-        } else {
-            Ok(RaggedBuffer {
-                data: data.iter().cloned().collect(),
-                subarrays,
-                features,
-                items: item,
-            })
-        }
-    }
-
-    pub fn extend(&mut self, other: &RaggedBuffer<T>) -> Result<()> {
-        if self.features != other.features {
-            return Err(Error::generic(format!(
-                "Features mismatch: {} != {}",
-                self.features, other.features
-            )));
-        }
-        let item = self.items;
-        self.data.extend(other.data.iter());
-        self.subarrays
-            .extend(other.subarrays.iter().map(|r| r.start + item..r.end + item));
-        self.items += other.items;
-        Ok(())
-    }
-
-    pub fn clear(&mut self) {
-        self.data.clear();
-        self.subarrays.clear();
-        self.items = 0;
-    }
-
-    // pub fn as_array<'a>(
-    //     &self,
-    //     py: Python<'a>,
-    // ) -> PyResult<&'a numpy::PyArray<T, numpy::ndarray::Dim<[usize; 2]>>> {
-    //     self.data
-    //         .to_pyarray(py)
-    //         .reshape((self.items, self.features))
-    // }
-
-    pub fn push(&mut self, data: &ArrayView2<T>) -> Result<()> {
-        if data.dim().1 != self.features {
-            return Err(Error::generic(format!(
-                "Features mismatch: {} != {}",
-                self.features,
-                data.dim().1
-            )));
-        }
-        self.subarrays.push(self.items..(self.items + data.dim().0));
-        match data.as_slice() {
-            Some(slice) => self.data.extend_from_slice(slice),
-            None => {
-                for x in data.iter() {
-                    self.data.push(*x);
-                }
-            }
-        }
-        self.items += data.dim().0;
-        Ok(())
-    }
-
-    pub fn push_empty(&mut self) {
-        self.subarrays.push(self.items..self.items);
-    }
-
-    pub fn swizzle(&self, indices: ArrayView1<i64>) -> Result<RaggedBuffer<T>> {
-        let indices = indices
-            .as_slice()
-            .ok_or_else(|| Error::generic("Indices must be a **contiguous** 1D array"))?;
-        let mut subarrays = Vec::with_capacity(indices.len());
-        let mut item = 0usize;
-        for i in indices {
-            let sublen = self.subarrays[*i as usize].end - self.subarrays[*i as usize].start;
-            subarrays.push(item..(item + sublen));
-            item += sublen;
-        }
-        let mut data = Vec::with_capacity(item * self.features);
-        for i in indices {
-            let Range { start, end } = self.subarrays[*i as usize];
-            data.extend_from_slice(&self.data[start * self.features..end * self.features]);
-        }
-        Ok(RaggedBuffer {
-            data,
-            subarrays,
-            features: self.features,
-            items: item,
-        })
-    }
-
-    pub fn get(&self, i: usize) -> RaggedBuffer<T> {
-        let subarray = self.subarrays[i].clone();
-        let Range { start, end } = subarray;
-        RaggedBuffer {
-            subarrays: vec![0..subarray.len()],
-            data: self.data[start * self.features..end * self.features].to_vec(),
-            features: self.features,
-            items: subarray.len(),
-        }
-    }
-
-    pub fn size0(&self) -> usize {
-        self.subarrays.len()
-    }
-
-    pub fn lengths(&self) -> Vec<i64> {
-        self.subarrays
-            .iter()
-            .map(|r| (r.end - r.start) as i64)
-            .collect::<Vec<_>>()
-    }
-
-    pub fn size1(&self, i: usize) -> Result<usize> {
-        if i >= self.subarrays.len() {
-            Err(Error::generic(format!("Index {} out of range", i)))
-        } else {
-            Ok(self.subarrays[i].end - self.subarrays[i].start)
-        }
-    }
-
-    pub fn size2(&self) -> usize {
-        self.features
-    }
-
-    pub fn __str__(&self) -> Result<String> {
-        let mut array = String::new();
-        array.push_str("RaggedBuffer([");
-        array.push('\n');
-        for range in &self.subarrays {
-            let slice = range.start * self.features..range.end * self.features;
-            if range.start == range.end {
-                writeln!(array, "    [],").unwrap();
-            } else if range.start + 1 == range.end {
-                writeln!(array, "    [{:?}],", &self.data[slice]).unwrap();
-            } else {
-                writeln!(array, "    [").unwrap();
-                for i in slice.clone() {
-                    if i % self.features == 0 {
-                        if i != slice.start {
-                            writeln!(array, "],").unwrap();
-                        }
-                        write!(array, "        [").unwrap();
-                    }
-                    write!(array, "{}", self.data[i]).unwrap();
-                    if i % self.features != self.features - 1 {
-                        write!(array, ", ").unwrap();
-                    }
-                }
-                writeln!(array, "],").unwrap();
-                writeln!(array, "    ],").unwrap();
-            }
-        }
-        write!(
-            array,
-            "], '{} * var * {} * {})",
-            self.subarrays.len(),
-            self.features,
-            std::any::type_name::<T>(),
-        )
-        .unwrap();
-
-        Ok(array)
-    }
-
-    pub fn binop<Op: BinOp<T>>(&self, rhs: &RaggedBuffer<T>) -> Result<RaggedBuffer<T>> {
-        if self.features == rhs.features && self.subarrays == rhs.subarrays {
-            let mut data = Vec::with_capacity(self.data.len());
-            for i in 0..self.data.len() {
-                data.push(Op::op(self.data[i], rhs.data[i]));
-            }
-            Ok(RaggedBuffer {
-                data,
-                subarrays: self.subarrays.clone(),
-                features: self.features,
-                items: self.items,
-            })
-        } else if self.features == rhs.features
-            && self.subarrays.len() == rhs.subarrays.len()
-            && rhs.subarrays.iter().all(|r| r.end - r.start == 1)
-        {
-            let mut data = Vec::with_capacity(self.data.len());
-            for (subarray, rhs_subarray) in self.subarrays.iter().zip(rhs.subarrays.iter()) {
-                for item in subarray.clone() {
-                    let lhs_offset = item * self.features;
-                    let rhs_offset = rhs_subarray.start * self.features;
-                    for i in 0..self.features {
-                        data.push(Op::op(self.data[lhs_offset + i], rhs.data[rhs_offset + i]));
-                    }
-                }
-            }
-            Ok(RaggedBuffer {
-                data,
-                subarrays: self.subarrays.clone(),
-                features: self.features,
-                items: self.items,
-            })
-        } else if self.features == rhs.features
-            && self.subarrays.len() == rhs.subarrays.len()
-            && self.subarrays.iter().all(|r| r.end - r.start == 1)
-        {
-            rhs.binop::<Op>(self)
-        } else {
-            Err(Error::generic(format!(
-                "Dimensions mismatch: ({}, {:?}, {}) != ({}, {:?}, {})",
-                self.size0(),
-                self.subarrays
-                    .iter()
-                    .map(|r| r.end - r.start)
-                    .collect::<Vec<_>>(),
-                self.size2(),
-                rhs.size0(),
-                rhs.subarrays
-                    .iter()
-                    .map(|r| r.end - r.start)
-                    .collect::<Vec<_>>(),
-                rhs.size2(),
-            )))
-        }
-    }
-
-    pub fn op_scalar<Op: BinOp<T>>(&self, scalar: T) -> RaggedBuffer<T> {
-        RaggedBuffer {
-            data: self.data.iter().map(|x| Op::op(*x, scalar)).collect(),
-            subarrays: self.subarrays.clone(),
-            features: self.features,
-            items: self.items,
-        }
-    }
-
-    pub fn indices(&self, dim: usize) -> Result<RaggedBuffer<i64>> {
-        match dim {
-            0 => {
-                let mut indices = Vec::with_capacity(self.items);
-                for (index, subarray) in self.subarrays.iter().enumerate() {
-                    for _ in subarray.clone() {
-                        indices.push(index as i64);
-                    }
-                }
-                Ok(RaggedBuffer {
-                    subarrays: self.subarrays.clone(),
-                    data: indices,
-                    features: 1,
-                    items: self.items,
-                })
-            }
-            1 => {
-                let mut indices = Vec::with_capacity(self.items);
-                for subarray in &self.subarrays {
-                    for (i, _) in subarray.clone().enumerate() {
-                        indices.push(i as i64);
-                    }
-                }
-                Ok(RaggedBuffer {
-                    subarrays: self.subarrays.clone(),
-                    data: indices,
-                    features: 1,
-                    items: self.items,
-                })
-            }
-            _ => Err(Error::generic(format!("Invalid dimension {}", dim))),
-        }
-    }
-
-    pub fn flat_indices(&self) -> Result<RaggedBuffer<i64>> {
-        Ok(RaggedBuffer {
-            subarrays: self.subarrays.clone(),
-            data: (0..self.items).map(|i| i as i64).collect(),
-            features: 1,
-            items: self.items,
-        })
-    }
-
-    pub fn cat(buffers: &[&RaggedBuffer<T>], dim: usize) -> Result<RaggedBuffer<T>> {
-        match dim {
-            0 => {
-                if buffers.iter().any(|b| b.features != buffers[0].features) {
-                    return Err(Error::generic(format!(
-                        "All buffers must have the same number of features, but found {}",
-                        buffers
-                            .iter()
-                            .map(|b| b.features.to_string())
-                            .collect::<Vec<_>>()
-                            .join(", ")
-                    )));
-                }
-                let mut data = Vec::with_capacity(buffers.iter().map(|b| b.data.len()).sum());
-                for buffer in buffers {
-                    data.extend_from_slice(&buffer.data);
-                }
-                let mut subarrays =
-                    Vec::with_capacity(buffers.iter().map(|b| b.subarrays.len()).sum());
-                let mut item = 0;
-                for buffer in buffers {
-                    subarrays.extend_from_slice(
-                        &buffer
-                            .subarrays
-                            .iter()
-                            .map(|r| {
-                                let start = r.start + item;
-                                let end = r.end + item;
-                                start..end
-                            })
-                            .collect::<Vec<_>>(),
-                    );
-                    item += buffer.items;
-                }
-                Ok(RaggedBuffer {
-                    data,
-                    subarrays,
-                    features: buffers[0].features,
-                    items: item,
-                })
-            }
-            1 => {
-                if buffers
-                    .iter()
-                    .any(|b| b.subarrays.len() != buffers[0].subarrays.len())
-                {
-                    return Err(Error::generic(format!(
-                        "All buffers must have the same number of subarrays, but found {}",
-                        buffers
-                            .iter()
-                            .map(|b| b.subarrays.len().to_string())
-                            .collect::<Vec<_>>()
-                            .join(", ")
-                    )));
-                }
-                if buffers.iter().any(|b| b.features != buffers[0].features) {
-                    return Err(Error::generic(format!(
-                        "All buffers must have the same number of features, but found {}",
-                        buffers
-                            .iter()
-                            .map(|b| b.features.to_string())
-                            .collect::<Vec<_>>()
-                            .join(", ")
-                    )));
-                }
-                let mut data = Vec::with_capacity(buffers.iter().map(|b| b.data.len()).sum());
-                let mut subarrays =
-                    Vec::with_capacity(buffers.iter().map(|b| b.subarrays.len()).sum());
-                let mut item = 0;
-                let mut last_item = 0;
-                for i in 0..buffers[0].subarrays.len() {
-                    for buffer in buffers {
-                        let Range { start, end } = &buffer.subarrays[i];
-                        data.extend_from_slice(
-                            &buffer.data[start * buffer.features..end * buffer.features],
-                        );
-                        item += end - start;
-                    }
-                    subarrays.push(Range {
-                        start: last_item,
-                        end: item,
-                    });
-                    last_item = item;
-                }
-                Ok(RaggedBuffer {
-                    data,
-                    subarrays,
-                    features: buffers[0].features,
-                    items: item,
-                })
-            }
-            2 => {
-                // TODO: disallow broadcasting on some sequences but not other?
-                // TODO: think more about empty sequences
-                let sequences = buffers[0].size0();
-                if buffers.iter().any(|b| b.size0() != sequences) {
-                    return Err(Error::generic(format!(
-                        "All buffers must have the same number of sequences, but found {}",
-                        buffers
-                            .iter()
-                            .map(|b| b.size0().to_string())
-                            .collect::<Vec<_>>()
-                            .join(", ")
-                    )));
-                }
-
-                let features = buffers.iter().map(|b| b.features).sum();
-                let mut subarrays = Vec::with_capacity(sequences);
-                let mut data = Vec::with_capacity(sequences * features);
-                let mut items = 0;
-                for iseq in 0..sequences {
-                    let seqlen = if buffers.iter().any(|b| {
-                        b.size1(iseq)
-                            .expect("All sequences should be the same length.")
-                            == 0
-                    }) {
-                        0
-                    } else {
-                        buffers
-                            .iter()
-                            .map(|b| {
-                                b.size1(iseq)
-                                    .expect("All sequences should be the same length.")
-                            })
-                            .max()
-                            .expect("There should be at least one buffer.")
-                    };
-                    subarrays.push(items..items + seqlen);
-                    items += seqlen;
-                    for iitem in 0..seqlen {
-                        for (ibuf, buffer) in buffers.iter().enumerate() {
-                            let _items = buffer.subarrays[iseq].len();
-                            if _items == 1 {
-                                data.extend_from_slice(
-                                    &buffer.data[buffer.subarrays[iseq].start * buffer.features
-                                        ..buffer.subarrays[iseq].end * buffer.features],
-                                );
-                            } else {
-                                if _items != seqlen {
-                                    return Err(Error::generic(format!(
-                                        "Buffer {} has {} items for sequence {}, but expected {}",
-                                        ibuf, _items, iseq, seqlen
-                                    )));
-                                }
-                                let start_item = buffer.subarrays[iseq].start + iitem;
-                                data.extend_from_slice(
-                                    &buffer.data[start_item * buffer.features
-                                        ..(start_item + 1) * buffer.features],
-                                );
-                            }
-                        }
-                    }
-                }
-
-                Ok(RaggedBuffer {
-                    items: data.len() / features,
-                    data,
-                    subarrays,
-                    features,
-                })
-            }
-            _ => Err(Error::generic(format!(
-                "Invalid dimension {}, RaggedBuffer only has 3 dimensions",
-                dim
-            ))),
-        }
-    }
-
-    #[allow(clippy::type_complexity)]
-    pub fn padpack(&self) -> Option<(Vec<i64>, Vec<f32>, Vec<i64>, (usize, usize))> {
-        if self.subarrays.is_empty()
-            || self
-                .subarrays
-                .iter()
-                .all(|r| r.end - r.start == self.subarrays[0].end - self.subarrays[0].start)
-        {
-            return None;
-        }
-
-        let mut padbpack_index = vec![];
-        let mut padpack_batch = vec![];
-        let mut padpack_inverse_index = vec![];
-        let max_seq_len = self
-            .subarrays
-            .iter()
-            .map(|r| r.end - r.start)
-            .max()
-            .unwrap();
-        let mut sequences: BinaryHeap<Sequence> = binary_heap::BinaryHeap::new();
-
-        for (batch_index, subarray) in self.subarrays.iter().enumerate() {
-            let (free, packed_batch_index) = match sequences.peek().cloned() {
-                Some(seq) if seq.free >= subarray.end - subarray.start => {
-                    sequences.pop();
-                    (seq.free, seq.batch_index)
-                }
-                _ => {
-                    for _ in 0..max_seq_len {
-                        padbpack_index.push(0);
-                        padpack_batch.push(f32::NAN);
-                    }
-                    (max_seq_len, sequences.len())
-                }
-            };
-
-            for (i, item) in subarray.clone().enumerate() {
-                let packed_index = packed_batch_index * max_seq_len + max_seq_len - free + i;
-                padbpack_index[packed_index] = item as i64;
-                padpack_batch[packed_index] = batch_index as f32;
-                padpack_inverse_index.push(packed_index as i64);
-            }
-            sequences.push(Sequence {
-                batch_index: packed_batch_index,
-                free: free - (subarray.end - subarray.start),
-            });
-        }
-
-        Some((
-            padbpack_index,
-            padpack_batch,
-            padpack_inverse_index,
-            (sequences.len(), max_seq_len),
-        ))
-    }
-
-    pub fn items(&self) -> usize {
-        self.items
-    }
-
-    pub fn len(&self) -> usize {
-        self.data.len()
-    }
-
-    pub fn is_empty(&self) -> bool {
-        self.data.is_empty()
-    }
-}
-
-#[derive(Copy, Clone, Eq, PartialEq, Debug)]
-struct Sequence {
-    free: usize,
-    batch_index: usize,
-}
-
-impl Ord for Sequence {
-    fn cmp(&self, other: &Self) -> Ordering {
-        self.free
-            .cmp(&other.free)
-            .then_with(|| other.batch_index.cmp(&self.batch_index))
-    }
-}
-
-impl PartialOrd for Sequence {
-    fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
-        Some(self.cmp(other))
-    }
-}
+use std::cmp::Ordering;
+use std::collections::{binary_heap, BinaryHeap};
+use std::fmt::{Display, Write};
+use std::ops::{Add, Mul, Range, Sub};
+
+use ndarray::{ArrayView1, ArrayView2, ArrayView3};
+
+#[derive(Debug)]
+pub enum Error {
+    Generic(String),
+}
+
+impl Error {
+    fn generic<S: Into<String>>(s: S) -> Self {
+        Self::Generic(s.into())
+    }
+}
+
+pub type Result<T> = std::result::Result<T, Error>;
+
+#[derive(Clone, PartialEq, Eq, Hash, Debug)]
+pub struct RaggedBuffer<T> {
+    pub data: Vec<T>,
+    // Each element of `subarrays` gives the start/end index of the items within that subarray (step size 1).
+    // The start index of the data of an item is obtained by multiplying its index by `features`.
+    pub subarrays: Vec<Range<usize>>,
+    pub features: usize,
+}
+
+pub trait BinOp<T> {
+    fn op(lhs: T, rhs: T) -> T;
+}
+
+pub struct BinOpAdd;
+
+impl<T: Add<T, Output = T>> BinOp<T> for BinOpAdd {
+    #[inline]
+    fn op(lhs: T, rhs: T) -> T {
+        lhs + rhs
+    }
+}
+
+pub struct BinOpSub;
+
+impl<T: Sub<T, Output = T>> BinOp<T> for BinOpSub {
+    #[inline]
+    fn op(lhs: T, rhs: T) -> T {
+        lhs - rhs
+    }
+}
+
+pub struct BinOpMul;
+
+impl<T: Mul<T, Output = T>> BinOp<T> for BinOpMul {
+    #[inline]
+    fn op(lhs: T, rhs: T) -> T {
+        lhs * rhs
+    }
+}
+
+impl<T: Copy + Display + std::fmt::Debug> RaggedBuffer<T> {
+    pub fn new(features: usize) -> Self {
+        RaggedBuffer {
+            data: Vec::new(),
+            subarrays: Vec::new(),
+            features,
+        }
+    }
+
+    pub fn from_array(data: ArrayView3<T>) -> Self {
+        let features = data.shape()[2];
+        RaggedBuffer {
+            data: data.iter().cloned().collect(),
+            subarrays: (0..data.shape()[0])
+                .map(|i| i * data.shape()[1]..(i + 1) * data.shape()[1])
+                .collect(),
+            features,
+        }
+    }
+
+    pub fn from_flattened(data: ArrayView2<T>, lengths: ArrayView1<i64>) -> Result<Self> {
+        let features = data.shape()[1];
+        let mut subarrays = Vec::new();
+        let mut item = 0;
+        for len in lengths.iter().cloned() {
+            subarrays.push(item..(item + len as usize));
+            item += len as usize;
+        }
+        if item != data.shape()[0] {
+            Err(Error::generic(format!(
+                "Lengths array specifies {} items, but data array has {} items",
+                item,
+                data.shape()[0]
+            )))
+        } else {
+            Ok(RaggedBuffer {
+                data: data.iter().cloned().collect(),
+                subarrays,
+                features,
+            })
+        }
+    }
+
+    pub fn extend(&mut self, other: &RaggedBuffer<T>) -> Result<()> {
+        if self.features != other.features {
+            return Err(Error::generic(format!(
+                "Features mismatch: {} != {}",
+                self.features, other.features
+            )));
+        }
+        let item = self.items();
+        self.data.extend(other.data.iter());
+        self.subarrays
+            .extend(other.subarrays.iter().map(|r| r.start + item..r.end + item));
+        Ok(())
+    }
+
+    pub fn clear(&mut self) {
+        self.data.clear();
+        self.subarrays.clear();
+    }
+
+    // pub fn as_array<'a>(
+    //     &self,
+    //     py: Python<'a>,
+    // ) -> PyResult<&'a numpy::PyArray<T, numpy::ndarray::Dim<[usize; 2]>>> {
+    //     self.data
+    //         .to_pyarray(py)
+    //         .reshape((self.items, self.features))
+    // }
+
+    pub fn push(&mut self, data: &ArrayView2<T>) -> Result<()> {
+        if data.dim().1 != self.features {
+            return Err(Error::generic(format!(
+                "Features mismatch: {} != {}",
+                self.features,
+                data.dim().1
+            )));
+        }
+        self.subarrays
+            .push(self.items()..(self.items() + data.dim().0));
+        match data.as_slice() {
+            Some(slice) => self.data.extend_from_slice(slice),
+            None => {
+                for x in data.iter() {
+                    self.data.push(*x);
+                }
+            }
+        }
+        Ok(())
+    }
+
+    pub fn push_empty(&mut self) {
+        self.subarrays.push(self.items()..self.items());
+    }
+
+    pub fn swizzle(&self, indices: ArrayView1<i64>) -> Result<RaggedBuffer<T>> {
+        let indices = indices
+            .as_slice()
+            .ok_or_else(|| Error::generic("Indices must be a **contiguous** 1D array"))?;
+        let mut subarrays = Vec::with_capacity(indices.len());
+        let mut item = 0usize;
+        for i in indices {
+            let sublen = self.subarrays[*i as usize].end - self.subarrays[*i as usize].start;
+            subarrays.push(item..(item + sublen));
+            item += sublen;
+        }
+        let mut data = Vec::with_capacity(item * self.features);
+        for i in indices {
+            let Range { start, end } = self.subarrays[*i as usize];
+            data.extend_from_slice(&self.data[start * self.features..end * self.features]);
+        }
+        Ok(RaggedBuffer {
+            data,
+            subarrays,
+            features: self.features,
+        })
+    }
+
+    // TODO: dedupe with swizzle
+    pub fn swizzle_usize(&self, indices: &[usize]) -> Result<RaggedBuffer<T>> {
+        let mut subarrays = Vec::with_capacity(indices.len());
+        let mut item = 0usize;
+        for &i in indices {
+            let sublen = self.subarrays[i].end - self.subarrays[i].start;
+            subarrays.push(item..(item + sublen));
+            item += sublen;
+        }
+        let mut data = Vec::with_capacity(item * self.features);
+        for i in indices {
+            let Range { start, end } = self.subarrays[*i as usize];
+            data.extend_from_slice(&self.data[start * self.features..end * self.features]);
+        }
+        Ok(RaggedBuffer {
+            data,
+            subarrays,
+            features: self.features,
+        })
+    }
+
+    pub fn get(&self, i: usize) -> RaggedBuffer<T> {
+        let subarray = self.subarrays[i].clone();
+        let Range { start, end } = subarray;
+        RaggedBuffer {
+            subarrays: vec![0..subarray.len()],
+            data: self.data[start * self.features..end * self.features].to_vec(),
+            features: self.features,
+        }
+    }
+
+    pub fn size0(&self) -> usize {
+        self.subarrays.len()
+    }
+
+    pub fn lengths(&self) -> Vec<i64> {
+        self.subarrays
+            .iter()
+            .map(|r| (r.end - r.start) as i64)
+            .collect::<Vec<_>>()
+    }
+
+    pub fn size1(&self, i: usize) -> Result<usize> {
+        if i >= self.subarrays.len() {
+            Err(Error::generic(format!("Index {} out of range", i)))
+        } else {
+            Ok(self.subarrays[i].end - self.subarrays[i].start)
+        }
+    }
+
+    pub fn size2(&self) -> usize {
+        self.features
+    }
+
+    pub fn __str__(&self) -> Result<String> {
+        let mut array = String::new();
+        array.push_str("RaggedBuffer([");
+        array.push('\n');
+        for range in &self.subarrays {
+            let slice = range.start * self.features..range.end * self.features;
+            if range.start == range.end {
+                writeln!(array, "    [],").unwrap();
+            } else if range.start + 1 == range.end {
+                writeln!(array, "    [{:?}],", &self.data[slice]).unwrap();
+            } else {
+                writeln!(array, "    [").unwrap();
+                for i in slice.clone() {
+                    if i % self.features == 0 {
+                        if i != slice.start {
+                            writeln!(array, "],").unwrap();
+                        }
+                        write!(array, "        [").unwrap();
+                    }
+                    write!(array, "{}", self.data[i]).unwrap();
+                    if i % self.features != self.features - 1 {
+                        write!(array, ", ").unwrap();
+                    }
+                }
+                writeln!(array, "],").unwrap();
+                writeln!(array, "    ],").unwrap();
+            }
+        }
+        write!(
+            array,
+            "], '{} * var * {} * {})",
+            self.subarrays.len(),
+            self.features,
+            std::any::type_name::<T>(),
+        )
+        .unwrap();
+
+        Ok(array)
+    }
+
+    pub fn binop<Op: BinOp<T>>(&self, rhs: &RaggedBuffer<T>) -> Result<RaggedBuffer<T>> {
+        if self.features == rhs.features && self.subarrays == rhs.subarrays {
+            let mut data = Vec::with_capacity(self.data.len());
+            for i in 0..self.data.len() {
+                data.push(Op::op(self.data[i], rhs.data[i]));
+            }
+            Ok(RaggedBuffer {
+                data,
+                subarrays: self.subarrays.clone(),
+                features: self.features,
+            })
+        } else if self.features == rhs.features
+            && self.subarrays.len() == rhs.subarrays.len()
+            && rhs.subarrays.iter().all(|r| r.end - r.start == 1)
+        {
+            let mut data = Vec::with_capacity(self.data.len());
+            for (subarray, rhs_subarray) in self.subarrays.iter().zip(rhs.subarrays.iter()) {
+                for item in subarray.clone() {
+                    let lhs_offset = item * self.features;
+                    let rhs_offset = rhs_subarray.start * self.features;
+                    for i in 0..self.features {
+                        data.push(Op::op(self.data[lhs_offset + i], rhs.data[rhs_offset + i]));
+                    }
+                }
+            }
+            Ok(RaggedBuffer {
+                data,
+                subarrays: self.subarrays.clone(),
+                features: self.features,
+            })
+        } else if self.features == rhs.features
+            && self.subarrays.len() == rhs.subarrays.len()
+            && self.subarrays.iter().all(|r| r.end - r.start == 1)
+        {
+            rhs.binop::<Op>(self)
+        } else {
+            Err(Error::generic(format!(
+                "Dimensions mismatch: ({}, {:?}, {}) != ({}, {:?}, {})",
+                self.size0(),
+                self.subarrays
+                    .iter()
+                    .map(|r| r.end - r.start)
+                    .collect::<Vec<_>>(),
+                self.size2(),
+                rhs.size0(),
+                rhs.subarrays
+                    .iter()
+                    .map(|r| r.end - r.start)
+                    .collect::<Vec<_>>(),
+                rhs.size2(),
+            )))
+        }
+    }
+
+    pub fn op_scalar<Op: BinOp<T>>(&self, scalar: T) -> RaggedBuffer<T> {
+        RaggedBuffer {
+            data: self.data.iter().map(|x| Op::op(*x, scalar)).collect(),
+            subarrays: self.subarrays.clone(),
+            features: self.features,
+        }
+    }
+
+    pub fn indices(&self, dim: usize) -> Result<RaggedBuffer<i64>> {
+        match dim {
+            0 => {
+                let mut indices = Vec::with_capacity(self.items());
+                for (index, subarray) in self.subarrays.iter().enumerate() {
+                    for _ in subarray.clone() {
+                        indices.push(index as i64);
+                    }
+                }
+                Ok(RaggedBuffer {
+                    subarrays: self.subarrays.clone(),
+                    data: indices,
+                    features: 1,
+                })
+            }
+            1 => {
+                let mut indices = Vec::with_capacity(self.items());
+                for subarray in &self.subarrays {
+                    for (i, _) in subarray.clone().enumerate() {
+                        indices.push(i as i64);
+                    }
+                }
+                Ok(RaggedBuffer {
+                    subarrays: self.subarrays.clone(),
+                    data: indices,
+                    features: 1,
+                })
+            }
+            _ => Err(Error::generic(format!("Invalid dimension {}", dim))),
+        }
+    }
+
+    pub fn flat_indices(&self) -> Result<RaggedBuffer<i64>> {
+        Ok(RaggedBuffer {
+            subarrays: self.subarrays.clone(),
+            data: (0..self.items()).map(|i| i as i64).collect(),
+            features: 1,
+        })
+    }
+
+    pub fn cat(buffers: &[&RaggedBuffer<T>], dim: usize) -> Result<RaggedBuffer<T>> {
+        match dim {
+            0 => {
+                if buffers.iter().any(|b| b.features != buffers[0].features) {
+                    return Err(Error::generic(format!(
+                        "All buffers must have the same number of features, but found {}",
+                        buffers
+                            .iter()
+                            .map(|b| b.features.to_string())
+                            .collect::<Vec<_>>()
+                            .join(", ")
+                    )));
+                }
+                let mut data = Vec::with_capacity(buffers.iter().map(|b| b.data.len()).sum());
+                for buffer in buffers {
+                    data.extend_from_slice(&buffer.data);
+                }
+                let mut subarrays =
+                    Vec::with_capacity(buffers.iter().map(|b| b.subarrays.len()).sum());
+                let mut item = 0;
+                for buffer in buffers {
+                    subarrays.extend_from_slice(
+                        &buffer
+                            .subarrays
+                            .iter()
+                            .map(|r| {
+                                let start = r.start + item;
+                                let end = r.end + item;
+                                start..end
+                            })
+                            .collect::<Vec<_>>(),
+                    );
+                    item += buffer.items();
+                }
+                Ok(RaggedBuffer {
+                    data,
+                    subarrays,
+                    features: buffers[0].features,
+                })
+            }
+            1 => {
+                if buffers
+                    .iter()
+                    .any(|b| b.subarrays.len() != buffers[0].subarrays.len())
+                {
+                    return Err(Error::generic(format!(
+                        "All buffers must have the same number of subarrays, but found {}",
+                        buffers
+                            .iter()
+                            .map(|b| b.subarrays.len().to_string())
+                            .collect::<Vec<_>>()
+                            .join(", ")
+                    )));
+                }
+                if buffers.iter().any(|b| b.features != buffers[0].features) {
+                    return Err(Error::generic(format!(
+                        "All buffers must have the same number of features, but found {}",
+                        buffers
+                            .iter()
+                            .map(|b| b.features.to_string())
+                            .collect::<Vec<_>>()
+                            .join(", ")
+                    )));
+                }
+                let mut data = Vec::with_capacity(buffers.iter().map(|b| b.data.len()).sum());
+                let mut subarrays =
+                    Vec::with_capacity(buffers.iter().map(|b| b.subarrays.len()).sum());
+                let mut item = 0;
+                let mut last_item = 0;
+                for i in 0..buffers[0].subarrays.len() {
+                    for buffer in buffers {
+                        let Range { start, end } = &buffer.subarrays[i];
+                        data.extend_from_slice(
+                            &buffer.data[start * buffer.features..end * buffer.features],
+                        );
+                        item += end - start;
+                    }
+                    subarrays.push(Range {
+                        start: last_item,
+                        end: item,
+                    });
+                    last_item = item;
+                }
+                Ok(RaggedBuffer {
+                    data,
+                    subarrays,
+                    features: buffers[0].features,
+                })
+            }
+            2 => {
+                // TODO: disallow broadcasting on some sequences but not other?
+                // TODO: think more about empty sequences
+                let sequences = buffers[0].size0();
+                if buffers.iter().any(|b| b.size0() != sequences) {
+                    return Err(Error::generic(format!(
+                        "All buffers must have the same number of sequences, but found {}",
+                        buffers
+                            .iter()
+                            .map(|b| b.size0().to_string())
+                            .collect::<Vec<_>>()
+                            .join(", ")
+                    )));
+                }
+
+                let features = buffers.iter().map(|b| b.features).sum();
+                let mut subarrays = Vec::with_capacity(sequences);
+                let mut data = Vec::with_capacity(sequences * features);
+                let mut items = 0;
+                for iseq in 0..sequences {
+                    let seqlen = if buffers.iter().any(|b| {
+                        b.size1(iseq)
+                            .expect("All sequences should be the same length.")
+                            == 0
+                    }) {
+                        0
+                    } else {
+                        buffers
+                            .iter()
+                            .map(|b| {
+                                b.size1(iseq)
+                                    .expect("All sequences should be the same length.")
+                            })
+                            .max()
+                            .expect("There should be at least one buffer.")
+                    };
+                    subarrays.push(items..items + seqlen);
+                    items += seqlen;
+                    for iitem in 0..seqlen {
+                        for (ibuf, buffer) in buffers.iter().enumerate() {
+                            let _items = buffer.subarrays[iseq].len();
+                            if _items == 1 {
+                                data.extend_from_slice(
+                                    &buffer.data[buffer.subarrays[iseq].start * buffer.features
+                                        ..buffer.subarrays[iseq].end * buffer.features],
+                                );
+                            } else {
+                                if _items != seqlen {
+                                    return Err(Error::generic(format!(
+                                        "Buffer {} has {} items for sequence {}, but expected {}",
+                                        ibuf, _items, iseq, seqlen
+                                    )));
+                                }
+                                let start_item = buffer.subarrays[iseq].start + iitem;
+                                data.extend_from_slice(
+                                    &buffer.data[start_item * buffer.features
+                                        ..(start_item + 1) * buffer.features],
+                                );
+                            }
+                        }
+                    }
+                }
+
+                Ok(RaggedBuffer {
+                    data,
+                    subarrays,
+                    features,
+                })
+            }
+            _ => Err(Error::generic(format!(
+                "Invalid dimension {}, RaggedBuffer only has 3 dimensions",
+                dim
+            ))),
+        }
+    }
+
+    #[allow(clippy::type_complexity)]
+    pub fn padpack(&self) -> Option<(Vec<i64>, Vec<f32>, Vec<i64>, (usize, usize))> {
+        if self.subarrays.is_empty()
+            || self
+                .subarrays
+                .iter()
+                .all(|r| r.end - r.start == self.subarrays[0].end - self.subarrays[0].start)
+        {
+            return None;
+        }
+
+        let mut padbpack_index = vec![];
+        let mut padpack_batch = vec![];
+        let mut padpack_inverse_index = vec![];
+        let max_seq_len = self
+            .subarrays
+            .iter()
+            .map(|r| r.end - r.start)
+            .max()
+            .unwrap();
+        let mut sequences: BinaryHeap<Sequence> = binary_heap::BinaryHeap::new();
+
+        for (batch_index, subarray) in self.subarrays.iter().enumerate() {
+            let (free, packed_batch_index) = match sequences.peek().cloned() {
+                Some(seq) if seq.free >= subarray.end - subarray.start => {
+                    sequences.pop();
+                    (seq.free, seq.batch_index)
+                }
+                _ => {
+                    for _ in 0..max_seq_len {
+                        padbpack_index.push(0);
+                        padpack_batch.push(f32::NAN);
+                    }
+                    (max_seq_len, sequences.len())
+                }
+            };
+
+            for (i, item) in subarray.clone().enumerate() {
+                let packed_index = packed_batch_index * max_seq_len + max_seq_len - free + i;
+                padbpack_index[packed_index] = item as i64;
+                padpack_batch[packed_index] = batch_index as f32;
+                padpack_inverse_index.push(packed_index as i64);
+            }
+            sequences.push(Sequence {
+                batch_index: packed_batch_index,
+                free: free - (subarray.end - subarray.start),
+            });
+        }
+
+        Some((
+            padbpack_index,
+            padpack_batch,
+            padpack_inverse_index,
+            (sequences.len(), max_seq_len),
+        ))
+    }
+
+    pub fn items(&self) -> usize {
+        self.subarrays.last().map(|r| r.end).unwrap_or(0)
+    }
+
+    pub fn len(&self) -> usize {
+        self.data.len()
+    }
+
+    pub fn is_empty(&self) -> bool {
+        self.data.is_empty()
+    }
+}
+
+#[derive(Copy, Clone, Eq, PartialEq, Debug)]
+struct Sequence {
+    free: usize,
+    batch_index: usize,
+}
+
+impl Ord for Sequence {
+    fn cmp(&self, other: &Self) -> Ordering {
+        self.free
+            .cmp(&other.free)
+            .then_with(|| other.batch_index.cmp(&self.batch_index))
+    }
+}
+
+impl PartialOrd for Sequence {
+    fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
+        Some(self.cmp(other))
+    }
+}
```

### Comparing `ragged_buffer-0.4.4/src/ragged_buffer_view.rs` & `ragged_buffer-0.4.7/src/ragged_buffer_view.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,645 +1,650 @@
-use std::fmt::Display;
-use std::sync::{Arc, RwLock, RwLockReadGuard, RwLockWriteGuard};
-
-use numpy::{PyReadonlyArray1, PyReadonlyArray2, PyReadonlyArray3, ToPyArray};
-use pyo3::{exceptions, PyErr, PyResult, Python};
-
-use crate::monomorphs::Index;
-use crate::ragged_buffer::{BinOp, Error, RaggedBuffer};
-
-#[derive(Clone, PartialEq, Eq, Hash, Debug)]
-enum Slice {
-    Range {
-        start: usize,
-        end: usize,
-        step: usize,
-    },
-    Permutation(Vec<usize>),
-}
-
-impl Slice {
-    fn into_iter(self) -> Box<dyn Iterator<Item = usize>> {
-        match self {
-            Slice::Range { start, end, step } => Box::new((start..end).step_by(step)),
-            Slice::Permutation(permutation) => Box::new(permutation.into_iter()),
-        }
-    }
-
-    fn len(&self) -> usize {
-        match self {
-            Slice::Range { start, end, step } => (end - start + step - 1) / step,
-            Slice::Permutation(permutation) => permutation.len(),
-        }
-    }
-}
-
-// TODO: Eq/PartialEq/Hash
-#[derive(Clone, Debug)]
-pub struct RaggedBufferView<T> {
-    pub inner: Arc<RwLock<RaggedBuffer<T>>>,
-    view: Option<(Slice, Slice, Slice)>,
-}
-
-impl<T: numpy::Element + Copy + Display + std::fmt::Debug> RaggedBufferView<T> {
-    pub fn new(features: usize) -> Self {
-        RaggedBufferView {
-            inner: Arc::new(RwLock::new(RaggedBuffer::new(features))),
-            view: None,
-        }
-    }
-
-    pub fn get_slice<'a>(
-        &self,
-        py: Python<'a>,
-        i0: Index,
-        i1: Index,
-        i2: Index,
-    ) -> PyResult<RaggedBufferView<T>> {
-        // TODO: Check that i0, i1, i2 are valid indices
-        let materialized = self.materialize();
-        let v0 = match i0 {
-            Index::PermutationNP(np) => {
-                Slice::Permutation(np.to_vec()?.into_iter().map(|x| x as usize).collect())
-            }
-            Index::Permutation(p) => Slice::Permutation(p),
-            Index::Int(i) => Slice::Range {
-                start: i,
-                end: i + 1,
-                step: 1,
-            },
-            Index::Slice(slice) => {
-                let indices = slice
-                    .as_ref(py)
-                    .indices(materialized.size0().try_into().unwrap())?;
-                Slice::Range {
-                    start: indices.start as usize,
-                    end: indices.stop as usize,
-                    step: indices.step as usize,
-                }
-            }
-        };
-        let v1 = match i1 {
-            Index::PermutationNP(np) => {
-                Slice::Permutation(np.to_vec()?.into_iter().map(|x| x as usize).collect())
-            }
-            Index::Permutation(p) => Slice::Permutation(p),
-            Index::Int(i) => Slice::Range {
-                start: i,
-                end: i + 1,
-                step: 1,
-            },
-            Index::Slice(slice) => {
-                let indices = slice
-                    .as_ref(py)
-                    .indices(materialized.len()?.try_into().unwrap())?;
-                Slice::Range {
-                    start: indices.start as usize,
-                    end: indices.stop as usize,
-                    step: indices.step as usize,
-                }
-            }
-        };
-        let v2 = match i2 {
-            Index::PermutationNP(np) => {
-                Slice::Permutation(np.to_vec()?.into_iter().map(|x| x as usize).collect())
-            }
-            Index::Permutation(p) => Slice::Permutation(p),
-            Index::Int(i) => Slice::Range {
-                start: i,
-                end: i + 1,
-                step: 1,
-            },
-            Index::Slice(slice) => {
-                let indices = slice
-                    .as_ref(py)
-                    .indices(materialized.size2().try_into().unwrap())?;
-                Slice::Range {
-                    start: indices.start as usize,
-                    end: indices.stop as usize,
-                    step: indices.step as usize,
-                }
-            }
-        };
-
-        Ok(RaggedBufferView {
-            inner: materialized.inner,
-            view: Some((v0, v1, v2)),
-        })
-    }
-
-    fn get(&self) -> RwLockReadGuard<RaggedBuffer<T>> {
-        self.inner.read().unwrap()
-    }
-
-    fn get_mut(&self) -> RwLockWriteGuard<RaggedBuffer<T>> {
-        self.inner.write().unwrap()
-    }
-
-    fn make_contiguous(&mut self) {
-        let materialized = self.materialize();
-        self.inner = materialized.inner;
-        self.view = None;
-    }
-    fn require_contiguous(&self, method_name: &str) -> PyResult<()> {
-        match self.view {
-            Some(_) => Err(pyo3::exceptions::PyValueError::new_err(format!(
-                "Cannot call method {} on a view. Call .materialize() first to get a materialized copy of the view.",
-                method_name
-            ))),
-            None => Ok(()),
-        }
-    }
-
-    pub fn from_array(data: PyReadonlyArray3<T>) -> Self {
-        RaggedBufferView {
-            inner: Arc::new(RwLock::new(RaggedBuffer::from_array(data.as_array()))),
-            view: None,
-        }
-    }
-
-    pub fn from_flattened(
-        data: PyReadonlyArray2<T>,
-        lengths: PyReadonlyArray1<i64>,
-    ) -> PyResult<Self> {
-        Ok(RaggedBufferView {
-            inner: Arc::new(RwLock::new(RaggedBuffer::from_flattened(
-                data.as_array(),
-                lengths.as_array(),
-            )?)),
-            view: None,
-        })
-    }
-
-    pub fn extend(&mut self, other: &RaggedBufferView<T>) -> PyResult<()> {
-        self.make_contiguous();
-        let other = other.materialize();
-        let other = other.get();
-        self.get_mut().extend(&*other).map_err(Into::into)
-    }
-
-    pub fn clear(&mut self) -> PyResult<()> {
-        self.make_contiguous();
-        self.get_mut().clear();
-        Ok(())
-    }
-
-    pub fn as_array<'a>(
-        &self,
-        py: Python<'a>,
-    ) -> PyResult<&'a numpy::PyArray<T, numpy::ndarray::Dim<[usize; 2]>>> {
-        match self.view {
-            None => {
-                let inner = self.get();
-                inner
-                    .data
-                    .to_pyarray(py)
-                    .reshape((inner.items, inner.features))
-                    .map_err(Into::into)
-            }
-            _ => self.materialize().as_array(py),
-        }
-    }
-
-    pub fn materialize(&self) -> RaggedBufferView<T> {
-        match self.view.clone() {
-            Some((
-                Slice::Range {
-                    start: start0,
-                    end: end0,
-                    step: step0,
-                },
-                Slice::Range {
-                    start: start1,
-                    end: end1,
-                    step: step1,
-                },
-                Slice::Range {
-                    start: start2,
-                    end: end2,
-                    step: step2,
-                },
-            )) => {
-                let mut data = Vec::new();
-                let mut subarrays = Vec::new();
-                let mut item = 0;
-                let inner = self.get();
-                for i0 in (start0..end0).step_by(step0) {
-                    let mut items = 0;
-                    for i1 in inner.subarrays[i0]
-                        .clone()
-                        .skip(start1)
-                        .take(end1 - start1)
-                        .step_by(step1)
-                    {
-                        for i2 in (start2..end2).step_by(step2) {
-                            data.push(inner.data[i1 * inner.features + i2]);
-                        }
-                        items += 1;
-                    }
-                    subarrays.push(item..item + items);
-                    item += items;
-                }
-                let features = (end2 - start2 + step2 - 1) / step2;
-                let materialized = RaggedBuffer {
-                    data,
-                    subarrays,
-                    features,
-                    items: item,
-                };
-                RaggedBufferView {
-                    inner: Arc::new(RwLock::new(materialized)),
-                    view: None,
-                }
-            }
-            Some((v0, v1, v2)) => {
-                let mut data = Vec::new();
-                let mut items = 0;
-                let mut subarrays = Vec::new();
-                let inner = self.get();
-                for i0 in v0.into_iter() {
-                    let item_start = items;
-                    let subarray = inner.subarrays[i0].clone();
-                    for i1 in v1.clone().into_iter() {
-                        if i1 >= subarray.len() {
-                            break;
-                        }
-                        let offset = (subarray.start + i1) * inner.features;
-                        for i2 in v2.clone().into_iter() {
-                            data.push(inner.data[offset + i2]);
-                        }
-                        items += 1;
-                    }
-                    subarrays.push(item_start..items);
-                }
-                let features = v2.len();
-                let materialized = RaggedBuffer {
-                    data,
-                    subarrays,
-                    features,
-                    items,
-                };
-                RaggedBufferView {
-                    inner: Arc::new(RwLock::new(materialized)),
-                    view: None,
-                }
-            }
-            None => self.clone(),
-        }
-    }
-
-    pub fn push(&mut self, x: &PyReadonlyArray2<T>) -> PyResult<()> {
-        self.make_contiguous();
-        self.get_mut().push(&x.as_array()).map_err(Into::into)
-    }
-
-    pub fn push_empty(&mut self) -> PyResult<()> {
-        self.make_contiguous();
-        self.get_mut().push_empty();
-        Ok(())
-    }
-
-    pub fn swizzle(&self, indices: PyReadonlyArray1<i64>) -> PyResult<RaggedBufferView<T>> {
-        match self.view {
-            Some((_, _, _)) => todo!(),
-            None => Ok(self.get().swizzle(indices.as_array())?.view()),
-        }
-    }
-
-    pub fn get_sequence(&self, i: usize) -> PyResult<RaggedBufferView<T>> {
-        self.require_contiguous("get_sequence")?;
-        Ok(self.get().get(i).view())
-    }
-
-    pub fn size0(&self) -> usize {
-        match &self.view {
-            Some((s0, _, _)) => s0.len(),
-            None => self.get().size0(),
-        }
-    }
-
-    pub fn size2(&self) -> usize {
-        match &self.view {
-            Some((_, _, s2)) => s2.len(),
-            None => self.get().size2(),
-        }
-    }
-
-    pub fn lengths<'a>(
-        &self,
-        py: Python<'a>,
-    ) -> PyResult<&'a numpy::PyArray<i64, numpy::ndarray::Dim<[usize; 1]>>> {
-        match self.view {
-            None => Ok(self.get().lengths().to_pyarray(py)),
-            Some((
-                Slice::Range {
-                    start: start0,
-                    end: end0,
-                    step: step0,
-                },
-                Slice::Range {
-                    start: start1,
-                    end: end1,
-                    step: step1,
-                },
-                _,
-            )) => {
-                let mut lengths = Vec::with_capacity((end0 - start0) / step0);
-                let inner = self.get();
-                for i0 in (start0..end0).step_by(step0) {
-                    let end1 = std::cmp::min(end1, inner.subarrays[i0].len());
-                    if end1 > start1 {
-                        let stepsf = (end1 - start1) / step1;
-                        lengths.push(
-                            stepsf as i64 + if stepsf * step1 < end1 - start1 { 1 } else { 0 },
-                        );
-                    } else {
-                        lengths.push(0);
-                    }
-                }
-                Ok(lengths.to_pyarray(py))
-            }
-            _ => {
-                self.require_contiguous("lengths")?;
-                Ok(self.get().lengths().to_pyarray(py))
-            }
-        }
-    }
-
-    pub fn size1(&mut self, i: usize) -> PyResult<usize> {
-        self.make_contiguous();
-        self.get().size1(i).map_err(Into::into)
-    }
-
-    pub fn __str__(&self) -> PyResult<String> {
-        self.materialize().get().__str__().map_err(Into::into)
-    }
-
-    pub fn binop<Op: BinOp<T>>(&self, rhs: &RaggedBufferView<T>) -> PyResult<RaggedBufferView<T>> {
-        self.require_contiguous("binop")?;
-        Ok(self.get().binop::<Op>(&*rhs.get())?.view())
-    }
-
-    pub fn op_scalar<Op: BinOp<T>>(&self, scalar: T) -> PyResult<RaggedBufferView<T>> {
-        self.require_contiguous("op_scalar")?;
-        Ok(self.get().op_scalar::<Op>(scalar).view())
-    }
-
-    pub fn indices(&mut self, dim: usize) -> PyResult<RaggedBufferView<i64>> {
-        self.make_contiguous();
-        Ok(self.get().indices(dim)?.view())
-    }
-
-    pub fn flat_indices(&mut self) -> PyResult<RaggedBufferView<i64>> {
-        self.make_contiguous();
-        Ok(self.get().flat_indices()?.view())
-    }
-
-    pub fn cat(buffers: &[&RaggedBufferView<T>], dim: usize) -> PyResult<RaggedBufferView<T>> {
-        if buffers.is_empty() {
-            return Err(pyo3::exceptions::PyValueError::new_err(
-                "cat requires at least one ragged buffer",
-            ));
-        }
-        let mut rbs = Vec::new();
-        for b in buffers {
-            b.require_contiguous("cat")?;
-            rbs.push(b.get());
-        }
-        let rb = RaggedBuffer::cat(&rbs.iter().map(|r| &**r).collect::<Vec<_>>(), dim)?;
-        Ok(RaggedBufferView {
-            inner: Arc::new(RwLock::new(rb)),
-            view: None,
-        })
-    }
-
-    #[allow(clippy::type_complexity)]
-    pub fn padpack(&mut self) -> PyResult<Option<(Vec<i64>, Vec<f32>, Vec<i64>, (usize, usize))>> {
-        self.make_contiguous();
-        Ok(self.get().padpack())
-    }
-
-    #[allow(clippy::len_without_is_empty)]
-    pub fn len(&self) -> PyResult<usize> {
-        self.require_contiguous("len")?;
-        Ok(self.get().len())
-    }
-
-    pub fn is_empty(&mut self) -> PyResult<bool> {
-        self.make_contiguous();
-        Ok(self.get().is_empty())
-    }
-
-    pub fn items(&mut self) -> PyResult<usize> {
-        self.make_contiguous();
-        Ok(self.get().items())
-    }
-
-    pub fn binop_mut<Op: BinOp<T>>(&self, rhs: &RaggedBufferView<T>) -> PyResult<()> {
-        let (lhs_i0, lhs_i1, lhs_i2) = self.view.clone().unwrap();
-        let (rhs_i0, rhs_i1, rhs_i2) = rhs.view.clone().unwrap();
-
-        let (lhs_iter_0, rhs_iter_0) = if self.size0() == rhs.size0() {
-            (lhs_i0.into_iter(), rhs_i0.into_iter())
-        } else {
-            return Err(exceptions::PyValueError::new_err(format!(
-                "size mismatch in first dimension: {} != {}",
-                self.size0(),
-                rhs.size0(),
-            )));
-        };
-        assert!(matches!(lhs_i1, Slice::Range { .. }));
-        assert!(matches!(rhs_i1, Slice::Range { .. }));
-        if self.size2() != rhs.size2() {
-            return Err(exceptions::PyValueError::new_err(format!(
-                "size mismatch in third dimension: {} != {}",
-                self.size2(),
-                rhs.size2(),
-            )));
-        };
-
-        let stride2l = self.get().size2();
-        let stride2r = rhs.get().size2();
-
-        let mut lhs = self.get_mut();
-        let rhs = rhs.get();
-        for (l0, r0) in lhs_iter_0.zip(rhs_iter_0) {
-            let (lhs_iter_1, rhs_iter_1): (
-                Box<dyn Iterator<Item = usize>>,
-                Box<dyn Iterator<Item = usize>>,
-            ) = if lhs.subarrays[l0].len() != rhs.subarrays[r0].len() {
-                if lhs.subarrays[l0].len() == 1 {
-                    (
-                        Box::new(
-                            vec![lhs.subarrays[l0].start; rhs.subarrays[r0].len()].into_iter(),
-                        ),
-                        Box::new(rhs.subarrays[r0].clone()),
-                    )
-                } else if rhs.subarrays[r0].len() == 1 {
-                    (
-                        Box::new(lhs.subarrays[l0].clone()),
-                        Box::new(
-                            vec![rhs.subarrays[r0].start; lhs.subarrays[l0].len()].into_iter(),
-                        ),
-                    )
-                } else {
-                    return Err(exceptions::PyValueError::new_err(format!(
-                        "size mismatch between {}th and {}th sequence: {} != {}",
-                        l0,
-                        r0,
-                        lhs.subarrays[l0].len(),
-                        rhs.subarrays[r0].len(),
-                    )));
-                }
-            } else {
-                (
-                    Box::new(lhs.subarrays[l0].clone()),
-                    Box::new(rhs.subarrays[r0].clone()),
-                )
-            };
-            for (l1, r1) in lhs_iter_1.zip(rhs_iter_1) {
-                for (l2, r2) in lhs_i2.clone().into_iter().zip(rhs_i2.clone().into_iter()) {
-                    lhs.data[l1 * stride2l + l2] =
-                        Op::op(lhs.data[l1 * stride2l + l2], rhs.data[r1 * stride2r + r2]);
-                }
-            }
-        }
-
-        Ok(())
-    }
-
-    pub fn deepclone(&self) -> RaggedBufferView<T> {
-        let inner = self.get().clone();
-        RaggedBufferView {
-            inner: Arc::new(RwLock::new(inner)),
-            view: self.view.clone(),
-        }
-    }
-}
-
-pub fn translate_rotate(
-    source: &RaggedBufferView<f32>,
-    translation: &RaggedBufferView<f32>,
-    rotation: &RaggedBufferView<f32>,
-) -> PyResult<()> {
-    if source.size0() != translation.size0() {
-        return Err(exceptions::PyValueError::new_err(format!(
-            "size mismatch in first dimension: {} != {}",
-            source.size0(),
-            translation.size0(),
-        )));
-    }
-    if source.size2() != 2 {
-        return Err(exceptions::PyValueError::new_err(format!(
-            "expected 2D source, got {}D",
-            source.size2(),
-        )));
-    }
-    if translation.size2() != 2 {
-        return Err(exceptions::PyValueError::new_err(format!(
-            "expected 2D translation, got {}D",
-            translation.size2(),
-        )));
-    }
-    if rotation.size2() != 2 {
-        return Err(exceptions::PyValueError::new_err(format!(
-            "expected rotation to be a 2D direction, got {}D",
-            rotation.size2(),
-        )));
-    }
-    let (s0, _, s2) = source.view.clone().unwrap();
-    let (t0, _, t2) = translation.view.clone().unwrap();
-    let (r0, _, r2) = rotation.view.clone().unwrap();
-    let mut source = source.get_mut();
-    let translation = translation.get();
-    let rotation = rotation.get();
-
-    let ss0 = source.size0();
-    let ts0 = translation.size0();
-    let rs0 = rotation.size0();
-    match s0 {
-        Slice::Range { start, end, step } if start == 0 && end == ss0 && step == 1 => {}
-        _ => {
-            return Err(exceptions::PyValueError::new_err(
-                "view on first dimension of source not supported".to_string(),
-            ))
-        }
-    }
-    match t0 {
-        Slice::Range { start, end, step } if start == 0 && end == ts0 && step == 1 => {}
-        _ => {
-            return Err(exceptions::PyValueError::new_err(
-                "view on first dimension of translation not supported".to_string(),
-            ))
-        }
-    }
-    match r0 {
-        Slice::Range { start, end, step } if start == 0 && end == rs0 && step == 1 => {}
-        _ => {
-            return Err(exceptions::PyValueError::new_err(
-                "view on first dimension of rotation not supported".to_string(),
-            ))
-        }
-    }
-    let (sxi, syi) = match s2 {
-        Slice::Range { start, step, .. } => (start, start + step),
-        Slice::Permutation(indices) => (indices[0], indices[1]),
-    };
-    let (txi, tyi) = match t2 {
-        Slice::Range { start, step, .. } => (start, start + step),
-        Slice::Permutation(indices) => (indices[0], indices[1]),
-    };
-    let (rxi, ryi) = match r2 {
-        Slice::Range { start, step, .. } => (start, start + step),
-        Slice::Permutation(indices) => (indices[0], indices[1]),
-    };
-    let sstride = source.features;
-    for i0 in 0..source.size0() {
-        if translation.size1(i0)? != 1 || rotation.size1(i0)? != 1 {
-            return Err(exceptions::PyValueError::new_err(format!(
-                "must have single item in translation and rotation for each sequence, but got {} and {} items for sequence {}",
-                translation.size1(i0)?, rotation.size1(i0)?, i0,
-            )));
-        }
-        // TODO: check no view on dim 1
-        for i1 in source.subarrays[i0].clone() {
-            let sstart = i1 * sstride;
-            source.data[sstart + sxi] -= translation.data[i0 * translation.features + txi];
-            source.data[sstart + syi] -= translation.data[i0 * translation.features + tyi];
-            let rx = rotation.data[i0 * rotation.features + rxi];
-            let ry = rotation.data[i0 * rotation.features + ryi];
-            let sx = source.data[sstart + sxi];
-            let sy = source.data[sstart + syi];
-            source.data[sstart + sxi] = rx * sx + ry * sy;
-            source.data[sstart + syi] = -ry * sx + rx * sy;
-        }
-    }
-    Ok(())
-}
-
-impl<T: numpy::Element + Copy + Display + std::fmt::Debug + PartialEq> PartialEq
-    for RaggedBufferView<T>
-{
-    fn eq(&self, other: &RaggedBufferView<T>) -> bool {
-        // TODO: implement for views
-        self.require_contiguous("eq").unwrap();
-        other.require_contiguous("eq").unwrap();
-        *self.get() == *other.get()
-    }
-}
-
-impl<T: numpy::Element + Copy + Display + std::fmt::Debug + Eq> Eq for RaggedBufferView<T> {}
-
-impl<T> RaggedBuffer<T> {
-    pub fn view(self) -> RaggedBufferView<T> {
-        RaggedBufferView {
-            inner: Arc::new(RwLock::new(self)),
-            view: None,
-        }
-    }
-}
-
-impl From<Error> for PyErr {
-    fn from(Error::Generic(msg): Error) -> PyErr {
-        exceptions::PyValueError::new_err(msg)
-    }
-}
+use std::fmt::Display;
+use std::sync::{Arc, RwLock, RwLockReadGuard, RwLockWriteGuard};
+
+use numpy::{PyReadonlyArray1, PyReadonlyArray2, PyReadonlyArray3, ToPyArray};
+use pyo3::{exceptions, PyErr, PyResult, Python};
+
+use crate::monomorphs::Index;
+use crate::ragged_buffer::{BinOp, Error, RaggedBuffer};
+
+#[derive(Clone, PartialEq, Eq, Hash, Debug)]
+enum Slice {
+    Range {
+        start: usize,
+        end: usize,
+        step: usize,
+    },
+    Permutation(Vec<usize>),
+}
+
+impl Slice {
+    fn into_iter(self) -> Box<dyn Iterator<Item = usize>> {
+        match self {
+            Slice::Range { start, end, step } => Box::new((start..end).step_by(step)),
+            Slice::Permutation(permutation) => Box::new(permutation.into_iter()),
+        }
+    }
+
+    fn len(&self) -> usize {
+        match self {
+            Slice::Range { start, end, step } => (end - start + step - 1) / step,
+            Slice::Permutation(permutation) => permutation.len(),
+        }
+    }
+}
+
+// TODO: Eq/PartialEq/Hash
+#[derive(Clone, Debug)]
+pub struct RaggedBufferView<T> {
+    pub inner: Arc<RwLock<RaggedBuffer<T>>>,
+    view: Option<(Slice, Slice, Slice)>,
+}
+
+impl<T: numpy::Element + Copy + Display + std::fmt::Debug> RaggedBufferView<T> {
+    pub fn new(features: usize) -> Self {
+        RaggedBufferView {
+            inner: Arc::new(RwLock::new(RaggedBuffer::new(features))),
+            view: None,
+        }
+    }
+
+    pub fn get_slice<'a>(
+        &self,
+        py: Python<'a>,
+        i0: Index,
+        i1: Index,
+        i2: Index,
+    ) -> PyResult<RaggedBufferView<T>> {
+        // TODO: Check that i0, i1, i2 are valid indices
+        let materialized = self.materialize();
+        let v0 = match i0 {
+            Index::PermutationNP(np) => {
+                Slice::Permutation(np.to_vec()?.into_iter().map(|x| x as usize).collect())
+            }
+            Index::Permutation(p) => Slice::Permutation(p),
+            Index::Int(i) => Slice::Range {
+                start: i,
+                end: i + 1,
+                step: 1,
+            },
+            Index::Slice(slice) => {
+                let indices = slice
+                    .as_ref(py)
+                    .indices(materialized.size0().try_into().unwrap())?;
+                Slice::Range {
+                    start: indices.start as usize,
+                    end: indices.stop as usize,
+                    step: indices.step as usize,
+                }
+            }
+        };
+        let v1 = match i1 {
+            Index::PermutationNP(np) => {
+                Slice::Permutation(np.to_vec()?.into_iter().map(|x| x as usize).collect())
+            }
+            Index::Permutation(p) => Slice::Permutation(p),
+            Index::Int(i) => Slice::Range {
+                start: i,
+                end: i + 1,
+                step: 1,
+            },
+            Index::Slice(slice) => {
+                let indices = slice
+                    .as_ref(py)
+                    .indices(materialized.len()?.try_into().unwrap())?;
+                Slice::Range {
+                    start: indices.start as usize,
+                    end: indices.stop as usize,
+                    step: indices.step as usize,
+                }
+            }
+        };
+        let v2 = match i2 {
+            Index::PermutationNP(np) => {
+                Slice::Permutation(np.to_vec()?.into_iter().map(|x| x as usize).collect())
+            }
+            Index::Permutation(p) => Slice::Permutation(p),
+            Index::Int(i) => Slice::Range {
+                start: i,
+                end: i + 1,
+                step: 1,
+            },
+            Index::Slice(slice) => {
+                let indices = slice
+                    .as_ref(py)
+                    .indices(materialized.size2().try_into().unwrap())?;
+                Slice::Range {
+                    start: indices.start as usize,
+                    end: indices.stop as usize,
+                    step: indices.step as usize,
+                }
+            }
+        };
+
+        Ok(RaggedBufferView {
+            inner: materialized.inner,
+            view: Some((v0, v1, v2)),
+        })
+    }
+
+    fn get(&self) -> RwLockReadGuard<RaggedBuffer<T>> {
+        self.inner.read().unwrap()
+    }
+
+    fn get_mut(&self) -> RwLockWriteGuard<RaggedBuffer<T>> {
+        self.inner.write().unwrap()
+    }
+
+    fn make_contiguous(&mut self) {
+        let materialized = self.materialize();
+        self.inner = materialized.inner;
+        self.view = None;
+    }
+    fn require_contiguous(&self, method_name: &str) -> PyResult<()> {
+        match self.view {
+            Some(_) => Err(pyo3::exceptions::PyValueError::new_err(format!(
+                "Cannot call method {} on a view. Call .materialize() first to get a materialized copy of the view.",
+                method_name
+            ))),
+            None => Ok(()),
+        }
+    }
+
+    pub fn from_array(data: PyReadonlyArray3<T>) -> Self {
+        RaggedBufferView {
+            inner: Arc::new(RwLock::new(RaggedBuffer::from_array(data.as_array()))),
+            view: None,
+        }
+    }
+
+    pub fn from_flattened(
+        data: PyReadonlyArray2<T>,
+        lengths: PyReadonlyArray1<i64>,
+    ) -> PyResult<Self> {
+        Ok(RaggedBufferView {
+            inner: Arc::new(RwLock::new(RaggedBuffer::from_flattened(
+                data.as_array(),
+                lengths.as_array(),
+            )?)),
+            view: None,
+        })
+    }
+
+    pub fn extend(&mut self, other: &RaggedBufferView<T>) -> PyResult<()> {
+        self.make_contiguous();
+        let other = other.materialize();
+        let other = other.get();
+        self.get_mut().extend(&*other).map_err(Into::into)
+    }
+
+    pub fn clear(&mut self) -> PyResult<()> {
+        self.make_contiguous();
+        self.get_mut().clear();
+        Ok(())
+    }
+
+    pub fn as_array<'a>(
+        &self,
+        py: Python<'a>,
+    ) -> PyResult<&'a numpy::PyArray<T, numpy::ndarray::Dim<[usize; 2]>>> {
+        match self.view {
+            None => {
+                let inner = self.get();
+                inner
+                    .data
+                    .to_pyarray(py)
+                    .reshape((inner.items(), inner.features))
+                    .map_err(Into::into)
+            }
+            _ => self.materialize().as_array(py),
+        }
+    }
+
+    pub fn materialize(&self) -> RaggedBufferView<T> {
+        match self.view.clone() {
+            Some((
+                Slice::Range {
+                    start: start0,
+                    end: end0,
+                    step: step0,
+                },
+                Slice::Range {
+                    start: start1,
+                    end: end1,
+                    step: step1,
+                },
+                Slice::Range {
+                    start: start2,
+                    end: end2,
+                    step: step2,
+                },
+            )) => {
+                let mut data = Vec::new();
+                let mut subarrays = Vec::new();
+                let mut item = 0;
+                let inner = self.get();
+                for i0 in (start0..end0).step_by(step0) {
+                    let mut items = 0;
+                    for i1 in inner.subarrays[i0]
+                        .clone()
+                        .skip(start1)
+                        .take(end1 - start1)
+                        .step_by(step1)
+                    {
+                        for i2 in (start2..end2).step_by(step2) {
+                            data.push(inner.data[i1 * inner.features + i2]);
+                        }
+                        items += 1;
+                    }
+                    subarrays.push(item..item + items);
+                    item += items;
+                }
+                let features = (end2 - start2 + step2 - 1) / step2;
+                let materialized = RaggedBuffer {
+                    data,
+                    subarrays,
+                    features,
+                };
+                RaggedBufferView {
+                    inner: Arc::new(RwLock::new(materialized)),
+                    view: None,
+                }
+            }
+            Some((v0, v1, v2)) => {
+                let mut data = Vec::new();
+                let mut items = 0;
+                let mut subarrays = Vec::new();
+                let inner = self.get();
+                for i0 in v0.into_iter() {
+                    let item_start = items;
+                    let subarray = inner.subarrays[i0].clone();
+                    for i1 in v1.clone().into_iter() {
+                        if i1 >= subarray.len() {
+                            break;
+                        }
+                        let offset = (subarray.start + i1) * inner.features;
+                        for i2 in v2.clone().into_iter() {
+                            data.push(inner.data[offset + i2]);
+                        }
+                        items += 1;
+                    }
+                    subarrays.push(item_start..items);
+                }
+                let features = v2.len();
+                let materialized = RaggedBuffer {
+                    data,
+                    subarrays,
+                    features,
+                };
+                RaggedBufferView {
+                    inner: Arc::new(RwLock::new(materialized)),
+                    view: None,
+                }
+            }
+            None => self.clone(),
+        }
+    }
+
+    pub fn push(&mut self, x: &PyReadonlyArray2<T>) -> PyResult<()> {
+        self.make_contiguous();
+        self.get_mut().push(&x.as_array()).map_err(Into::into)
+    }
+
+    pub fn push_empty(&mut self) -> PyResult<()> {
+        self.make_contiguous();
+        self.get_mut().push_empty();
+        Ok(())
+    }
+
+    pub fn swizzle(&self, indices: PyReadonlyArray1<i64>) -> PyResult<RaggedBufferView<T>> {
+        match self.view {
+            Some((_, _, _)) => todo!(),
+            None => Ok(self.get().swizzle(indices.as_array())?.view()),
+        }
+    }
+
+    pub fn swizzle_usize(&self, indices: &[usize]) -> PyResult<RaggedBufferView<T>> {
+        match self.view {
+            Some((_, _, _)) => todo!(),
+            None => Ok(self.get().swizzle_usize(indices)?.view()),
+        }
+    }
+
+    pub fn get_sequence(&self, i: usize) -> PyResult<RaggedBufferView<T>> {
+        self.require_contiguous("get_sequence")?;
+        Ok(self.get().get(i).view())
+    }
+
+    pub fn size0(&self) -> usize {
+        match &self.view {
+            Some((s0, _, _)) => s0.len(),
+            None => self.get().size0(),
+        }
+    }
+
+    pub fn size2(&self) -> usize {
+        match &self.view {
+            Some((_, _, s2)) => s2.len(),
+            None => self.get().size2(),
+        }
+    }
+
+    pub fn lengths<'a>(
+        &self,
+        py: Python<'a>,
+    ) -> PyResult<&'a numpy::PyArray<i64, numpy::ndarray::Dim<[usize; 1]>>> {
+        match self.view {
+            None => Ok(self.get().lengths().to_pyarray(py)),
+            Some((
+                Slice::Range {
+                    start: start0,
+                    end: end0,
+                    step: step0,
+                },
+                Slice::Range {
+                    start: start1,
+                    end: end1,
+                    step: step1,
+                },
+                _,
+            )) => {
+                let mut lengths = Vec::with_capacity((end0 - start0) / step0);
+                let inner = self.get();
+                for i0 in (start0..end0).step_by(step0) {
+                    let end1 = std::cmp::min(end1, inner.subarrays[i0].len());
+                    if end1 > start1 {
+                        let stepsf = (end1 - start1) / step1;
+                        lengths.push(
+                            stepsf as i64 + if stepsf * step1 < end1 - start1 { 1 } else { 0 },
+                        );
+                    } else {
+                        lengths.push(0);
+                    }
+                }
+                Ok(lengths.to_pyarray(py))
+            }
+            _ => {
+                self.require_contiguous("lengths")?;
+                Ok(self.get().lengths().to_pyarray(py))
+            }
+        }
+    }
+
+    pub fn size1(&mut self, i: usize) -> PyResult<usize> {
+        self.make_contiguous();
+        self.get().size1(i).map_err(Into::into)
+    }
+
+    pub fn __str__(&self) -> PyResult<String> {
+        self.materialize().get().__str__().map_err(Into::into)
+    }
+
+    pub fn binop<Op: BinOp<T>>(&self, rhs: &RaggedBufferView<T>) -> PyResult<RaggedBufferView<T>> {
+        self.require_contiguous("binop")?;
+        Ok(self.get().binop::<Op>(&*rhs.get())?.view())
+    }
+
+    pub fn op_scalar<Op: BinOp<T>>(&self, scalar: T) -> PyResult<RaggedBufferView<T>> {
+        self.require_contiguous("op_scalar")?;
+        Ok(self.get().op_scalar::<Op>(scalar).view())
+    }
+
+    pub fn indices(&mut self, dim: usize) -> PyResult<RaggedBufferView<i64>> {
+        self.make_contiguous();
+        Ok(self.get().indices(dim)?.view())
+    }
+
+    pub fn flat_indices(&mut self) -> PyResult<RaggedBufferView<i64>> {
+        self.make_contiguous();
+        Ok(self.get().flat_indices()?.view())
+    }
+
+    pub fn cat(buffers: &[&RaggedBufferView<T>], dim: usize) -> PyResult<RaggedBufferView<T>> {
+        if buffers.is_empty() {
+            return Err(pyo3::exceptions::PyValueError::new_err(
+                "cat requires at least one ragged buffer",
+            ));
+        }
+        let mut rbs = Vec::new();
+        for b in buffers {
+            b.require_contiguous("cat")?;
+            rbs.push(b.get());
+        }
+        let rb = RaggedBuffer::cat(&rbs.iter().map(|r| &**r).collect::<Vec<_>>(), dim)?;
+        Ok(RaggedBufferView {
+            inner: Arc::new(RwLock::new(rb)),
+            view: None,
+        })
+    }
+
+    #[allow(clippy::type_complexity)]
+    pub fn padpack(&mut self) -> PyResult<Option<(Vec<i64>, Vec<f32>, Vec<i64>, (usize, usize))>> {
+        self.make_contiguous();
+        Ok(self.get().padpack())
+    }
+
+    #[allow(clippy::len_without_is_empty)]
+    pub fn len(&self) -> PyResult<usize> {
+        self.require_contiguous("len")?;
+        Ok(self.get().len())
+    }
+
+    pub fn is_empty(&mut self) -> PyResult<bool> {
+        self.make_contiguous();
+        Ok(self.get().is_empty())
+    }
+
+    pub fn items(&mut self) -> PyResult<usize> {
+        self.make_contiguous();
+        Ok(self.get().items())
+    }
+
+    pub fn binop_mut<Op: BinOp<T>>(&self, rhs: &RaggedBufferView<T>) -> PyResult<()> {
+        let (lhs_i0, lhs_i1, lhs_i2) = self.view.clone().unwrap();
+        let (rhs_i0, rhs_i1, rhs_i2) = rhs.view.clone().unwrap();
+
+        let (lhs_iter_0, rhs_iter_0) = if self.size0() == rhs.size0() {
+            (lhs_i0.into_iter(), rhs_i0.into_iter())
+        } else {
+            return Err(exceptions::PyValueError::new_err(format!(
+                "size mismatch in first dimension: {} != {}",
+                self.size0(),
+                rhs.size0(),
+            )));
+        };
+        assert!(matches!(lhs_i1, Slice::Range { .. }));
+        assert!(matches!(rhs_i1, Slice::Range { .. }));
+        if self.size2() != rhs.size2() {
+            return Err(exceptions::PyValueError::new_err(format!(
+                "size mismatch in third dimension: {} != {}",
+                self.size2(),
+                rhs.size2(),
+            )));
+        };
+
+        let stride2l = self.get().size2();
+        let stride2r = rhs.get().size2();
+
+        let mut lhs = self.get_mut();
+        let rhs = rhs.get();
+        for (l0, r0) in lhs_iter_0.zip(rhs_iter_0) {
+            let (lhs_iter_1, rhs_iter_1): (
+                Box<dyn Iterator<Item = usize>>,
+                Box<dyn Iterator<Item = usize>>,
+            ) = if lhs.subarrays[l0].len() != rhs.subarrays[r0].len() {
+                if lhs.subarrays[l0].len() == 1 {
+                    (
+                        Box::new(
+                            vec![lhs.subarrays[l0].start; rhs.subarrays[r0].len()].into_iter(),
+                        ),
+                        Box::new(rhs.subarrays[r0].clone()),
+                    )
+                } else if rhs.subarrays[r0].len() == 1 {
+                    (
+                        Box::new(lhs.subarrays[l0].clone()),
+                        Box::new(
+                            vec![rhs.subarrays[r0].start; lhs.subarrays[l0].len()].into_iter(),
+                        ),
+                    )
+                } else {
+                    return Err(exceptions::PyValueError::new_err(format!(
+                        "size mismatch between {}th and {}th sequence: {} != {}",
+                        l0,
+                        r0,
+                        lhs.subarrays[l0].len(),
+                        rhs.subarrays[r0].len(),
+                    )));
+                }
+            } else {
+                (
+                    Box::new(lhs.subarrays[l0].clone()),
+                    Box::new(rhs.subarrays[r0].clone()),
+                )
+            };
+            for (l1, r1) in lhs_iter_1.zip(rhs_iter_1) {
+                for (l2, r2) in lhs_i2.clone().into_iter().zip(rhs_i2.clone().into_iter()) {
+                    lhs.data[l1 * stride2l + l2] =
+                        Op::op(lhs.data[l1 * stride2l + l2], rhs.data[r1 * stride2r + r2]);
+                }
+            }
+        }
+
+        Ok(())
+    }
+
+    pub fn deepclone(&self) -> RaggedBufferView<T> {
+        let inner = self.get().clone();
+        RaggedBufferView {
+            inner: Arc::new(RwLock::new(inner)),
+            view: self.view.clone(),
+        }
+    }
+}
+
+pub fn translate_rotate(
+    source: &RaggedBufferView<f32>,
+    translation: &RaggedBufferView<f32>,
+    rotation: &RaggedBufferView<f32>,
+) -> PyResult<()> {
+    if source.size0() != translation.size0() {
+        return Err(exceptions::PyValueError::new_err(format!(
+            "size mismatch in first dimension: {} != {}",
+            source.size0(),
+            translation.size0(),
+        )));
+    }
+    if source.size2() != 2 {
+        return Err(exceptions::PyValueError::new_err(format!(
+            "expected 2D source, got {}D",
+            source.size2(),
+        )));
+    }
+    if translation.size2() != 2 {
+        return Err(exceptions::PyValueError::new_err(format!(
+            "expected 2D translation, got {}D",
+            translation.size2(),
+        )));
+    }
+    if rotation.size2() != 2 {
+        return Err(exceptions::PyValueError::new_err(format!(
+            "expected rotation to be a 2D direction, got {}D",
+            rotation.size2(),
+        )));
+    }
+    let (s0, _, s2) = source.view.clone().unwrap();
+    let (t0, _, t2) = translation.view.clone().unwrap();
+    let (r0, _, r2) = rotation.view.clone().unwrap();
+    let mut source = source.get_mut();
+    let translation = translation.get();
+    let rotation = rotation.get();
+
+    let ss0 = source.size0();
+    let ts0 = translation.size0();
+    let rs0 = rotation.size0();
+    match s0 {
+        Slice::Range { start, end, step } if start == 0 && end == ss0 && step == 1 => {}
+        _ => {
+            return Err(exceptions::PyValueError::new_err(
+                "view on first dimension of source not supported".to_string(),
+            ))
+        }
+    }
+    match t0 {
+        Slice::Range { start, end, step } if start == 0 && end == ts0 && step == 1 => {}
+        _ => {
+            return Err(exceptions::PyValueError::new_err(
+                "view on first dimension of translation not supported".to_string(),
+            ))
+        }
+    }
+    match r0 {
+        Slice::Range { start, end, step } if start == 0 && end == rs0 && step == 1 => {}
+        _ => {
+            return Err(exceptions::PyValueError::new_err(
+                "view on first dimension of rotation not supported".to_string(),
+            ))
+        }
+    }
+    let (sxi, syi) = match s2 {
+        Slice::Range { start, step, .. } => (start, start + step),
+        Slice::Permutation(indices) => (indices[0], indices[1]),
+    };
+    let (txi, tyi) = match t2 {
+        Slice::Range { start, step, .. } => (start, start + step),
+        Slice::Permutation(indices) => (indices[0], indices[1]),
+    };
+    let (rxi, ryi) = match r2 {
+        Slice::Range { start, step, .. } => (start, start + step),
+        Slice::Permutation(indices) => (indices[0], indices[1]),
+    };
+    let sstride = source.features;
+    for i0 in 0..source.size0() {
+        if translation.size1(i0)? != 1 || rotation.size1(i0)? != 1 {
+            return Err(exceptions::PyValueError::new_err(format!(
+                "must have single item in translation and rotation for each sequence, but got {} and {} items for sequence {}",
+                translation.size1(i0)?, rotation.size1(i0)?, i0,
+            )));
+        }
+        // TODO: check no view on dim 1
+        for i1 in source.subarrays[i0].clone() {
+            let sstart = i1 * sstride;
+            source.data[sstart + sxi] -= translation.data[i0 * translation.features + txi];
+            source.data[sstart + syi] -= translation.data[i0 * translation.features + tyi];
+            let rx = rotation.data[i0 * rotation.features + rxi];
+            let ry = rotation.data[i0 * rotation.features + ryi];
+            let sx = source.data[sstart + sxi];
+            let sy = source.data[sstart + syi];
+            source.data[sstart + sxi] = rx * sx + ry * sy;
+            source.data[sstart + syi] = -ry * sx + rx * sy;
+        }
+    }
+    Ok(())
+}
+
+impl<T: numpy::Element + Copy + Display + std::fmt::Debug + PartialEq> PartialEq
+    for RaggedBufferView<T>
+{
+    fn eq(&self, other: &RaggedBufferView<T>) -> bool {
+        // TODO: implement for views
+        self.require_contiguous("eq").unwrap();
+        other.require_contiguous("eq").unwrap();
+        *self.get() == *other.get()
+    }
+}
+
+impl<T: numpy::Element + Copy + Display + std::fmt::Debug + Eq> Eq for RaggedBufferView<T> {}
+
+impl<T> RaggedBuffer<T> {
+    pub fn view(self) -> RaggedBufferView<T> {
+        RaggedBufferView {
+            inner: Arc::new(RwLock::new(self)),
+            view: None,
+        }
+    }
+}
+
+impl From<Error> for PyErr {
+    fn from(Error::Generic(msg): Error) -> PyErr {
+        exceptions::PyValueError::new_err(msg)
+    }
+}
```

### Comparing `ragged_buffer-0.4.4/tests/test.py` & `ragged_buffer-0.4.7/tests/test.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,489 +1,489 @@
-from typing import TypeVar
-import math
-import numpy as np
-from ragged_buffer import (
-    RaggedBufferF32,
-    RaggedBufferI64,
-    RaggedBufferBool,
-    RaggedBuffer,
-)
-import ragged_buffer
-
-rba = RaggedBufferF32(3)
-
-ScalarType = TypeVar("ScalarType", bound=np.generic)
-
-
-def generic_len(r: RaggedBuffer[ScalarType]) -> int:
-    return sum([r.size1(s) for s in range(r.size0())]) * r.size2()
-
-
-expected = """RaggedBuffer([
-], '0 * var * 3 * f32)"""
-assert str(rba) == expected
-
-rba.push(np.array([[2.0, 3.0, 1.0], [1.0, 2.0, 3.0]], dtype=np.float32))
-rba.push(
-    np.array([[2.0, 3.0, 1.0], [1.0, 2.0, 3.0], [1.4, 2.4, 3.4]], dtype=np.float32)
-)
-rba.push(
-    np.array(
-        [[2.0, 3.0, 1.0], [1.0, 2.0, 3.0], [1.4, 2.4, 3.4], [1.4, 2.4, 3.4]],
-        dtype=np.float32,
-    )
-)
-rba.push(np.array([], dtype=np.float32))
-rba.push_empty()
-
-assert generic_len(rba) == 27, f"Expected 27 elements, got {generic_len(rba)}"
-
-expected = """RaggedBuffer([
-    [
-        [2, 3, 1],
-        [1, 2, 3],
-    ],
-    [
-        [2, 3, 1],
-        [1, 2, 3],
-        [1.4, 2.4, 3.4],
-    ],
-    [
-        [2, 3, 1],
-        [1, 2, 3],
-        [1.4, 2.4, 3.4],
-        [1.4, 2.4, 3.4],
-    ],
-    [],
-    [],
-], '5 * var * 3 * f32)"""
-
-
-assert str(rba) == expected, str(rba)
-flattened = np.array(
-    [
-        [2.0, 3.0, 1.0],
-        [1.0, 2.0, 3.0],
-        [2.0, 3.0, 1.0],
-        [1.0, 2.0, 3.0],
-        [1.4, 2.4, 3.4],
-        [2.0, 3.0, 1.0],
-        [1.0, 2.0, 3.0],
-        [1.4, 2.4, 3.4],
-        [1.4, 2.4, 3.4],
-    ],
-    dtype=np.float32,
-)
-assert np.all(rba.as_array() == flattened)
-assert rba == RaggedBufferF32.from_flattened(
-    flattened=flattened,
-    lengths=np.array([2, 3, 4, 0, 0], dtype=np.int64),
-)
-assert RaggedBufferF32(3) == RaggedBufferF32(3)
-
-
-rba2 = RaggedBufferF32(3)
-rba2.push(np.array([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0]], dtype=np.float32))
-rba2.push(
-    np.array([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]], dtype=np.float32)
-)
-rba.extend(rba2)
-assert rba == RaggedBufferF32.from_flattened(
-    flattened=np.concatenate([flattened, np.zeros((5, 3), dtype=np.float32)]),
-    lengths=np.array([2, 3, 4, 0, 0, 2, 3], dtype=np.int64),
-)
-rba[np.random.permutation(rba.size0())]
-
-assert rba.size0() == 7
-assert rba.size1(0) == 2
-assert rba.size1(1) == 3
-assert rba.size1(2) == 4
-assert rba.size1(3) == 0
-assert rba.size1(4) == 0
-assert rba.size1(5) == 2
-assert rba.size1(6) == 3
-assert np.all(rba.size1() == np.array([2, 3, 4, 0, 0, 2, 3], dtype=np.int64))
-assert rba.size2() == 3
-
-rba.clear()
-assert rba == RaggedBufferF32(3)
-
-rb3 = RaggedBufferI64(1)
-rb3.push(np.array([[0]], dtype=np.int64))
-rb3.push(np.array([[0], [1], [2]], dtype=np.int64))
-rb3.push(np.array([[0], [5]], dtype=np.int64))
-assert rb3 == RaggedBufferI64.from_flattened(
-    flattened=np.array([[0], [0], [1], [2], [0], [5]], dtype=np.int64),
-    lengths=np.array([1, 3, 2], dtype=np.int64),
-)
-# Shuffle
-rb3[np.random.permutation(rb3.size0())]
-
-rb4 = RaggedBufferI64.from_array(np.array([0, 3, 10], dtype=np.int64).reshape(3, 1, 1))
-assert rb4 == RaggedBufferI64.from_flattened(
-    flattened=np.array([[0], [3], [10]], dtype=np.int64),
-    lengths=np.array([1, 1, 1], dtype=np.int64),
-)
-rb5 = rb3 + rb4
-assert np.all(
-    rb5.as_array() == np.array([[0], [3], [4], [5], [10], [15]], dtype=np.int64)
-), f"{rb5.as_array()}"
-assert rb3 + rb4 == rb4 + rb3
-assert rb5 * 10 == RaggedBufferI64.from_flattened(
-    flattened=np.array([[0], [30], [40], [50], [100], [150]], dtype=np.int64),
-    lengths=np.array([1, 3, 2], dtype=np.int64),
-)
-assert rb5.indices(1) == RaggedBufferI64.from_flattened(
-    flattened=np.array([[0], [0], [1], [2], [0], [1]], dtype=np.int64),
-    lengths=np.array([1, 3, 2], dtype=np.int64),
-)
-
-
-rb6 = RaggedBufferF32.from_flattened(
-    np.array(
-        [
-            [0.0, 0.0, 0.0],
-            [1.0, 2.0, 3.0],
-            [4.0, 5.0, 6.0],
-            [7.0, 8.0, 9.0],
-            [10.0, 11.0, 12.0],
-            [13.0, 14.0, 15.0],
-        ],
-        dtype=np.float32,
-    ),
-    np.array([3, 0, 2, 1], dtype=np.int64),
-)
-assert rb6[np.array([1, 3, 0], dtype=np.int64)] == RaggedBufferF32.from_flattened(
-    np.array(
-        [
-            [13.0, 14.0, 15.0],
-            [0, 0, 0],
-            [1, 2, 3],
-            [4, 5, 6],
-        ],
-        dtype=np.float32,
-    ),
-    np.array([0, 1, 3], dtype=np.int64),
-)
-
-assert np.all(
-    rb6[2].as_array()
-    == np.array([[7.0, 8.0, 9.0], [10.0, 11.0, 12.0]], dtype=np.float32)
-), f"{rb6[2]}"
-
-
-entities1 = RaggedBufferF32.from_flattened(
-    np.zeros((6, 64), dtype=np.float32), np.array([3, 1, 2], dtype=np.int64)
-)
-entities2 = RaggedBufferF32.from_flattened(
-    np.zeros((3, 64), dtype=np.float32), np.array([1, 2, 0], dtype=np.int64)
-)
-assert np.all(entities1.size1() == np.array([3, 1, 2], dtype=np.int64))
-assert np.all(entities2.size1() == np.array([1, 2, 0], dtype=np.int64))
-print("TEST 1 PASSED")
-
-bi1 = entities1.indices(0).as_array().flatten()
-bi2 = entities2.indices(0).as_array().flatten()
-assert np.all(bi1 == np.array([0, 0, 0, 1, 2, 2], dtype=np.int64)), f"{bi1}"
-assert np.all(bi2 == np.array([0, 1, 1], dtype=np.int64)), f"{bi2}"
-print("TEST 2 PASSED")
-
-flati1 = entities1.flat_indices()
-print("TEST 3 PASSED")
-flati2 = entities2.flat_indices() + 6
-print("TEST 4 PASSED")
-flat = ragged_buffer.cat([flati1, flati2, flati1, flati2], dim=1).as_array().flatten()
-assert np.all(
-    flat
-    == np.array([0, 1, 2, 6, 0, 1, 2, 6, 3, 7, 8, 3, 7, 8, 4, 5, 4, 5], dtype=np.int64),
-), f"{flat} {ragged_buffer.cat([flati1, flati2, flati1, flati2], dim=1)}"
-print("TEST 5 PASSED")
-
-
-mask = RaggedBufferI64.from_array(np.zeros((4, 1, 1), dtype=np.int64))
-offset = RaggedBufferI64.from_flattened(
-    np.array([0, 1, 2, 3, 13, 22, 32, 41, 42, 43, 44, 45,], dtype=np.int64).reshape(
-        -1,
-        1,
-    ),
-    np.ones(12, dtype=np.int64),
-)
-try:
-    mask = mask + offset
-except ValueError as e:
-    pass
-else:
-    assert False, "Did not raise ValueError"
-
-
-zerofeats = RaggedBufferF32(features=0)
-zerofeats.push(np.zeros((1, 0), dtype=np.float32))
-zerofeats.push(np.zeros((0, 0), dtype=np.float32))
-assert zerofeats.as_array().shape == (1, 0), f"{zerofeats.as_array().shape}"
-
-
-boolrb = RaggedBufferBool.from_flattened(
-    np.array([[True, False, True], [False, True, False]], dtype=np.bool_),
-    np.array([2, 0], dtype=np.int64),
-)
-assert boolrb.as_array().shape == (2, 3), f"{boolrb.as_array().shape}"
-assert np.all(
-    boolrb.as_array()
-    == np.array([[True, False, True], [False, True, False]], dtype=np.bool_)
-), f"{boolrb.as_array()}"
-
-batch_index = RaggedBufferI64.from_flattened(
-    np.array(
-        [[0], [0], [0], [0], [0], [0], [1], [1], [1], [2], [2], [2], [2], [4]],
-        dtype=np.int64,
-    ),
-    np.array([6, 3, 4, 0, 1], dtype=np.int64),
-)
-
-padpack = batch_index.padpack()
-assert padpack is not None
-padpack_index, padpack_batch, padpack_inverse_index = padpack
-
-assert np.all(
-    padpack_index
-    == np.array(
-        [[0, 1, 2, 3, 4, 5], [6, 7, 8, 13, 0, 0], [9, 10, 11, 12, 0, 0]], dtype=np.int64
-    ),
-), f"{padpack_index}"
-
-
-np.testing.assert_equal(
-    padpack_batch,
-    np.array(
-        [
-            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
-            [1.0, 1.0, 1.0, 4.0, np.NaN, np.NaN],
-            [2.0, 2.0, 2.0, 2.0, np.NaN, np.NaN],
-        ],
-        dtype=np.float32,
-    ),
-)
-
-np.testing.assert_equal(
-    padpack_inverse_index,
-    np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 12, 13, 14, 15, 9], dtype=np.int64),
-)
-
-
-origin = RaggedBufferF32.from_array(
-    np.array(
-        [
-            [[0.0, 0.0, 100.0, -23.0]],
-            [[1.0, -1.0, 200.0, -23.0]],
-            [[2.0, -2.0, 300.0, -23.0]],
-            [[-10.0, -10.0, 400.0, -23.0]],
-        ],
-        dtype=np.float32,
-    )
-)
-entities = RaggedBufferF32.from_flattened(
-    np.array(
-        [
-            [10, 3.0, 10, 1.0],
-            [11, 4.0, 11, 2.0],
-            [12, 5.0, 12, 3.0],
-            [13, 6.0, 13, 4.0],
-            [14, 7.0, 14, 5.0],
-            [15, 8.0, 15, 6.0],
-        ],
-        dtype=np.float32,
-    ),
-    np.array([3, 0, 2, 1], dtype=np.int64),
-)
-
-
-entities_slice = entities[:, :, [1, 3]]
-entities_clone = entities.clone()
-entities_slice -= origin[:, :, [0, 1]]
-assert entities == RaggedBufferF32.from_flattened(
-    np.array(
-        [
-            [10, 3.0, 10, 1.0],
-            [11, 4.0, 11, 2.0],
-            [12, 5.0, 12, 3.0],
-            [13, 4.0, 13, 6.0],
-            [14, 5.0, 14, 7.0],
-            [15, 18.0, 15, 16.0],
-        ],
-        dtype=np.float32,
-    ),
-    np.array([3, 0, 2, 1], dtype=np.int64),
-), f"{entities}"
-
-assert len(entities) == 24, f"{len(entities)}"
-assert entities.items() == 6
-assert entities_clone != entities
-
-
-origin = RaggedBufferF32.from_array(
-    np.array(
-        [
-            [[0.0, 0.0, 100.0, -23.0, 1.0, 0.0]],
-            [[1.0, -1.0, 200.0, -23.0, 1.0, 0.0]],
-            [[2.0, -2.0, 300.0, -23.0, math.sqrt(2) / 2, -math.sqrt(2) / 2]],
-            [[-10.0, -10.0, 400.0, -23.0, -1.0, 0.0]],
-        ],
-        dtype=np.float32,
-    )
-)
-entities = RaggedBufferF32.from_flattened(
-    np.array(
-        [
-            [10, 3.0, 10, 1.0],
-            [11, 4.0, 11, 2.0],
-            [12, 5.0, 12, 3.0],
-            [13, 6.0, 13, 4.0],
-            [14, 7.0, 14, 5.0],
-            [15, 8.0, 15, 6.0],
-        ],
-        dtype=np.float32,
-    ),
-    np.array([3, 0, 2, 1], dtype=np.int64),
-)
-
-
-ragged_buffer.translate_rotate(
-    entities[:, :, [1, 3]], origin[:, :, [0, 1]], origin[:, :, [4, 5]]
-)
-assert np.allclose(
-    entities.as_array(),
-    np.array(
-        [
-            [10, 3.0, 10, 1.0],
-            [11, 4.0, 11, 2.0],
-            [12, 5.0, 12, 3.0],
-            [13, -1.4142134, 13, 7.071068],
-            [14, -1.4142137, 14, 8.485281],
-            [15, -18.0, 15, -16.0],
-        ],
-        dtype=np.float32,
-    ),
-    1e-6,
-), f"{entities}"
-
-
-feats = RaggedBufferF32.from_flattened(
-    np.array(
-        [
-            [0.0, 3.0, 1.0, 1.0],
-            [1.0, 4.0, 0, 2.0],
-            [2.0, 5.0, 1.0, 3.0],
-            [3.0, 6.0, 0.0, 4.0],
-            [4.0, 7.0, 0.0, 5.0],
-            [5.0, 8.0, 0.0, 6.0],
-        ],
-        dtype=np.float32,
-    ),
-    np.array([3, 2, 1], dtype=np.int64),
-)
-assert np.array_equal(
-    feats[1:2, :, :].as_array(),
-    np.array(
-        [
-            [3.0, 6.0, 0.0, 4.0],
-            [4.0, 7.0, 0.0, 5.0],
-        ],
-        dtype=np.float32,
-    ),
-), f"{feats[1:2, :, :].as_array()}"
-assert np.array_equal(
-    feats[:, :, 1:3].as_array(),
-    np.array(
-        [
-            [3.0, 1.0],
-            [4.0, 0.0],
-            [5.0, 1.0],
-            [6.0, 0.0],
-            [7.0, 0.0],
-            [8.0, 0.0],
-        ],
-        dtype=np.float32,
-    ),
-), f"{feats[:, :, 1:3].as_array()}"
-assert np.array_equal(
-    feats[:, 0, :].as_array(),
-    np.array(
-        [
-            [0.0, 3.0, 1.0, 1.0],
-            [3.0, 6.0, 0.0, 4.0],
-            [5.0, 8.0, 0.0, 6.0],
-        ],
-        dtype=np.float32,
-    ),
-), f"{feats[:, :, 0].as_array()}"
-assert np.array_equal(
-    feats[:, 0:2:3, :].size1(),
-    np.array([1, 1, 1], dtype=np.int64),
-), f"{feats[:, 0:2:3, :].size1()}"
-assert np.array_equal(
-    feats[:, 1:3, 0].size1(),
-    np.array([2, 1, 0], dtype=np.int64),
-), f"{feats[:, 1:3, 0].size1()}"
-assert np.array_equal(
-    feats[1:, 1:10, 0].size1(),
-    np.array([1, 0], dtype=np.int64),
-), f"{feats[1:, 1:10, 0].size1()}"
-
-
-# Test broadcasting concatenation along dim 2
-entities = RaggedBufferF32.from_flattened(
-    np.array(
-        [
-            [10, 3.0, 10, 1.0],
-            [11, 4.0, 11, 2.0],
-            [12, 5.0, 12, 3.0],
-            [13, 4.0, 13, 6.0],
-            [14, 5.0, 14, 7.0],
-            [15, 18.0, 15, 16.0],
-        ],
-        dtype=np.float32,
-    ),
-    np.array([3, 0, 2, 1], dtype=np.int64),
-)
-global_feats = RaggedBufferF32.from_array(
-    np.array(
-        [
-            [[0.0]],
-            [[1.0]],
-            [[2.0]],
-            [[3.0]],
-        ],
-        dtype=np.float32,
-    )
-)
-result = ragged_buffer.cat([entities, global_feats], dim=2)
-assert np.array_equal(
-    result.as_array(),
-    np.array(
-        [
-            [10, 3.0, 10, 1.0, 0.0],
-            [11, 4.0, 11, 2.0, 0.0],
-            [12, 5.0, 12, 3.0, 0.0],
-            [13, 4.0, 13, 6.0, 2.0],
-            [14, 5.0, 14, 7.0, 2.0],
-            [15, 18.0, 15, 16.0, 3.0],
-        ]
-    ),
-), f"{result}"
-
-# Test complex indexing
-sliced = entities[[1, 0], 0:3:2, [0, 3, 2]]
-assert np.array_equal(
-    sliced.as_array(),
-    np.array(
-        [
-            [10, 1.0, 10],
-            [12, 3.0, 12],
-        ]
-    ),
-), f"{sliced}"
-assert np.array_equal(
-    sliced.materialize().size1(),
-    np.array([0, 2], dtype=np.int64),
-), f"{sliced.size1()}"
-
-print("ALL TESTS PASSED")
+from typing import TypeVar
+import math
+import numpy as np
+from ragged_buffer import (
+    RaggedBufferF32,
+    RaggedBufferI64,
+    RaggedBufferBool,
+    RaggedBuffer,
+)
+import ragged_buffer
+
+rba = RaggedBufferF32(3)
+
+ScalarType = TypeVar("ScalarType", bound=np.generic)
+
+
+def generic_len(r: RaggedBuffer[ScalarType]) -> int:
+    return sum([r.size1(s) for s in range(r.size0())]) * r.size2()
+
+
+expected = """RaggedBuffer([
+], '0 * var * 3 * f32)"""
+assert str(rba) == expected
+
+rba.push(np.array([[2.0, 3.0, 1.0], [1.0, 2.0, 3.0]], dtype=np.float32))
+rba.push(
+    np.array([[2.0, 3.0, 1.0], [1.0, 2.0, 3.0], [1.4, 2.4, 3.4]], dtype=np.float32)
+)
+rba.push(
+    np.array(
+        [[2.0, 3.0, 1.0], [1.0, 2.0, 3.0], [1.4, 2.4, 3.4], [1.4, 2.4, 3.4]],
+        dtype=np.float32,
+    )
+)
+rba.push(np.array([], dtype=np.float32))
+rba.push_empty()
+
+assert generic_len(rba) == 27, f"Expected 27 elements, got {generic_len(rba)}"
+
+expected = """RaggedBuffer([
+    [
+        [2, 3, 1],
+        [1, 2, 3],
+    ],
+    [
+        [2, 3, 1],
+        [1, 2, 3],
+        [1.4, 2.4, 3.4],
+    ],
+    [
+        [2, 3, 1],
+        [1, 2, 3],
+        [1.4, 2.4, 3.4],
+        [1.4, 2.4, 3.4],
+    ],
+    [],
+    [],
+], '5 * var * 3 * f32)"""
+
+
+assert str(rba) == expected, str(rba)
+flattened = np.array(
+    [
+        [2.0, 3.0, 1.0],
+        [1.0, 2.0, 3.0],
+        [2.0, 3.0, 1.0],
+        [1.0, 2.0, 3.0],
+        [1.4, 2.4, 3.4],
+        [2.0, 3.0, 1.0],
+        [1.0, 2.0, 3.0],
+        [1.4, 2.4, 3.4],
+        [1.4, 2.4, 3.4],
+    ],
+    dtype=np.float32,
+)
+assert np.all(rba.as_array() == flattened)
+assert rba == RaggedBufferF32.from_flattened(
+    flattened=flattened,
+    lengths=np.array([2, 3, 4, 0, 0], dtype=np.int64),
+)
+assert RaggedBufferF32(3) == RaggedBufferF32(3)
+
+
+rba2 = RaggedBufferF32(3)
+rba2.push(np.array([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0]], dtype=np.float32))
+rba2.push(
+    np.array([[0.0, 0.0, 0.0], [0.0, 0.0, 0.0], [0.0, 0.0, 0.0]], dtype=np.float32)
+)
+rba.extend(rba2)
+assert rba == RaggedBufferF32.from_flattened(
+    flattened=np.concatenate([flattened, np.zeros((5, 3), dtype=np.float32)]),
+    lengths=np.array([2, 3, 4, 0, 0, 2, 3], dtype=np.int64),
+)
+rba[np.random.permutation(rba.size0())]
+
+assert rba.size0() == 7
+assert rba.size1(0) == 2
+assert rba.size1(1) == 3
+assert rba.size1(2) == 4
+assert rba.size1(3) == 0
+assert rba.size1(4) == 0
+assert rba.size1(5) == 2
+assert rba.size1(6) == 3
+assert np.all(rba.size1() == np.array([2, 3, 4, 0, 0, 2, 3], dtype=np.int64))
+assert rba.size2() == 3
+
+rba.clear()
+assert rba == RaggedBufferF32(3)
+
+rb3 = RaggedBufferI64(1)
+rb3.push(np.array([[0]], dtype=np.int64))
+rb3.push(np.array([[0], [1], [2]], dtype=np.int64))
+rb3.push(np.array([[0], [5]], dtype=np.int64))
+assert rb3 == RaggedBufferI64.from_flattened(
+    flattened=np.array([[0], [0], [1], [2], [0], [5]], dtype=np.int64),
+    lengths=np.array([1, 3, 2], dtype=np.int64),
+)
+# Shuffle
+rb3[np.random.permutation(rb3.size0())]
+
+rb4 = RaggedBufferI64.from_array(np.array([0, 3, 10], dtype=np.int64).reshape(3, 1, 1))
+assert rb4 == RaggedBufferI64.from_flattened(
+    flattened=np.array([[0], [3], [10]], dtype=np.int64),
+    lengths=np.array([1, 1, 1], dtype=np.int64),
+)
+rb5 = rb3 + rb4
+assert np.all(
+    rb5.as_array() == np.array([[0], [3], [4], [5], [10], [15]], dtype=np.int64)
+), f"{rb5.as_array()}"
+assert rb3 + rb4 == rb4 + rb3
+assert rb5 * 10 == RaggedBufferI64.from_flattened(
+    flattened=np.array([[0], [30], [40], [50], [100], [150]], dtype=np.int64),
+    lengths=np.array([1, 3, 2], dtype=np.int64),
+)
+assert rb5.indices(1) == RaggedBufferI64.from_flattened(
+    flattened=np.array([[0], [0], [1], [2], [0], [1]], dtype=np.int64),
+    lengths=np.array([1, 3, 2], dtype=np.int64),
+)
+
+
+rb6 = RaggedBufferF32.from_flattened(
+    np.array(
+        [
+            [0.0, 0.0, 0.0],
+            [1.0, 2.0, 3.0],
+            [4.0, 5.0, 6.0],
+            [7.0, 8.0, 9.0],
+            [10.0, 11.0, 12.0],
+            [13.0, 14.0, 15.0],
+        ],
+        dtype=np.float32,
+    ),
+    np.array([3, 0, 2, 1], dtype=np.int64),
+)
+assert rb6[np.array([1, 3, 0], dtype=np.int64)] == RaggedBufferF32.from_flattened(
+    np.array(
+        [
+            [13.0, 14.0, 15.0],
+            [0, 0, 0],
+            [1, 2, 3],
+            [4, 5, 6],
+        ],
+        dtype=np.float32,
+    ),
+    np.array([0, 1, 3], dtype=np.int64),
+)
+
+assert np.all(
+    rb6[2].as_array()
+    == np.array([[7.0, 8.0, 9.0], [10.0, 11.0, 12.0]], dtype=np.float32)
+), f"{rb6[2]}"
+
+
+entities1 = RaggedBufferF32.from_flattened(
+    np.zeros((6, 64), dtype=np.float32), np.array([3, 1, 2], dtype=np.int64)
+)
+entities2 = RaggedBufferF32.from_flattened(
+    np.zeros((3, 64), dtype=np.float32), np.array([1, 2, 0], dtype=np.int64)
+)
+assert np.all(entities1.size1() == np.array([3, 1, 2], dtype=np.int64))
+assert np.all(entities2.size1() == np.array([1, 2, 0], dtype=np.int64))
+print("TEST 1 PASSED")
+
+bi1 = entities1.indices(0).as_array().flatten()
+bi2 = entities2.indices(0).as_array().flatten()
+assert np.all(bi1 == np.array([0, 0, 0, 1, 2, 2], dtype=np.int64)), f"{bi1}"
+assert np.all(bi2 == np.array([0, 1, 1], dtype=np.int64)), f"{bi2}"
+print("TEST 2 PASSED")
+
+flati1 = entities1.flat_indices()
+print("TEST 3 PASSED")
+flati2 = entities2.flat_indices() + 6
+print("TEST 4 PASSED")
+flat = ragged_buffer.cat([flati1, flati2, flati1, flati2], dim=1).as_array().flatten()
+assert np.all(
+    flat
+    == np.array([0, 1, 2, 6, 0, 1, 2, 6, 3, 7, 8, 3, 7, 8, 4, 5, 4, 5], dtype=np.int64),
+), f"{flat} {ragged_buffer.cat([flati1, flati2, flati1, flati2], dim=1)}"
+print("TEST 5 PASSED")
+
+
+mask = RaggedBufferI64.from_array(np.zeros((4, 1, 1), dtype=np.int64))
+offset = RaggedBufferI64.from_flattened(
+    np.array([0, 1, 2, 3, 13, 22, 32, 41, 42, 43, 44, 45,], dtype=np.int64).reshape(
+        -1,
+        1,
+    ),
+    np.ones(12, dtype=np.int64),
+)
+try:
+    mask = mask + offset
+except ValueError as e:
+    pass
+else:
+    assert False, "Did not raise ValueError"
+
+
+zerofeats = RaggedBufferF32(features=0)
+zerofeats.push(np.zeros((1, 0), dtype=np.float32))
+zerofeats.push(np.zeros((0, 0), dtype=np.float32))
+assert zerofeats.as_array().shape == (1, 0), f"{zerofeats.as_array().shape}"
+
+
+boolrb = RaggedBufferBool.from_flattened(
+    np.array([[True, False, True], [False, True, False]], dtype=np.bool_),
+    np.array([2, 0], dtype=np.int64),
+)
+assert boolrb.as_array().shape == (2, 3), f"{boolrb.as_array().shape}"
+assert np.all(
+    boolrb.as_array()
+    == np.array([[True, False, True], [False, True, False]], dtype=np.bool_)
+), f"{boolrb.as_array()}"
+
+batch_index = RaggedBufferI64.from_flattened(
+    np.array(
+        [[0], [0], [0], [0], [0], [0], [1], [1], [1], [2], [2], [2], [2], [4]],
+        dtype=np.int64,
+    ),
+    np.array([6, 3, 4, 0, 1], dtype=np.int64),
+)
+
+padpack = batch_index.padpack()
+assert padpack is not None
+padpack_index, padpack_batch, padpack_inverse_index = padpack
+
+assert np.all(
+    padpack_index
+    == np.array(
+        [[0, 1, 2, 3, 4, 5], [6, 7, 8, 13, 0, 0], [9, 10, 11, 12, 0, 0]], dtype=np.int64
+    ),
+), f"{padpack_index}"
+
+
+np.testing.assert_equal(
+    padpack_batch,
+    np.array(
+        [
+            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+            [1.0, 1.0, 1.0, 4.0, np.NaN, np.NaN],
+            [2.0, 2.0, 2.0, 2.0, np.NaN, np.NaN],
+        ],
+        dtype=np.float32,
+    ),
+)
+
+np.testing.assert_equal(
+    padpack_inverse_index,
+    np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 12, 13, 14, 15, 9], dtype=np.int64),
+)
+
+
+origin = RaggedBufferF32.from_array(
+    np.array(
+        [
+            [[0.0, 0.0, 100.0, -23.0]],
+            [[1.0, -1.0, 200.0, -23.0]],
+            [[2.0, -2.0, 300.0, -23.0]],
+            [[-10.0, -10.0, 400.0, -23.0]],
+        ],
+        dtype=np.float32,
+    )
+)
+entities = RaggedBufferF32.from_flattened(
+    np.array(
+        [
+            [10, 3.0, 10, 1.0],
+            [11, 4.0, 11, 2.0],
+            [12, 5.0, 12, 3.0],
+            [13, 6.0, 13, 4.0],
+            [14, 7.0, 14, 5.0],
+            [15, 8.0, 15, 6.0],
+        ],
+        dtype=np.float32,
+    ),
+    np.array([3, 0, 2, 1], dtype=np.int64),
+)
+
+
+entities_slice = entities[:, :, [1, 3]]
+entities_clone = entities.clone()
+entities_slice -= origin[:, :, [0, 1]]
+assert entities == RaggedBufferF32.from_flattened(
+    np.array(
+        [
+            [10, 3.0, 10, 1.0],
+            [11, 4.0, 11, 2.0],
+            [12, 5.0, 12, 3.0],
+            [13, 4.0, 13, 6.0],
+            [14, 5.0, 14, 7.0],
+            [15, 18.0, 15, 16.0],
+        ],
+        dtype=np.float32,
+    ),
+    np.array([3, 0, 2, 1], dtype=np.int64),
+), f"{entities}"
+
+assert len(entities) == 24, f"{len(entities)}"
+assert entities.items() == 6
+assert entities_clone != entities
+
+
+origin = RaggedBufferF32.from_array(
+    np.array(
+        [
+            [[0.0, 0.0, 100.0, -23.0, 1.0, 0.0]],
+            [[1.0, -1.0, 200.0, -23.0, 1.0, 0.0]],
+            [[2.0, -2.0, 300.0, -23.0, math.sqrt(2) / 2, -math.sqrt(2) / 2]],
+            [[-10.0, -10.0, 400.0, -23.0, -1.0, 0.0]],
+        ],
+        dtype=np.float32,
+    )
+)
+entities = RaggedBufferF32.from_flattened(
+    np.array(
+        [
+            [10, 3.0, 10, 1.0],
+            [11, 4.0, 11, 2.0],
+            [12, 5.0, 12, 3.0],
+            [13, 6.0, 13, 4.0],
+            [14, 7.0, 14, 5.0],
+            [15, 8.0, 15, 6.0],
+        ],
+        dtype=np.float32,
+    ),
+    np.array([3, 0, 2, 1], dtype=np.int64),
+)
+
+
+ragged_buffer.translate_rotate(
+    entities[:, :, [1, 3]], origin[:, :, [0, 1]], origin[:, :, [4, 5]]
+)
+assert np.allclose(
+    entities.as_array(),
+    np.array(
+        [
+            [10, 3.0, 10, 1.0],
+            [11, 4.0, 11, 2.0],
+            [12, 5.0, 12, 3.0],
+            [13, -1.4142134, 13, 7.071068],
+            [14, -1.4142137, 14, 8.485281],
+            [15, -18.0, 15, -16.0],
+        ],
+        dtype=np.float32,
+    ),
+    1e-6,
+), f"{entities}"
+
+
+feats = RaggedBufferF32.from_flattened(
+    np.array(
+        [
+            [0.0, 3.0, 1.0, 1.0],
+            [1.0, 4.0, 0, 2.0],
+            [2.0, 5.0, 1.0, 3.0],
+            [3.0, 6.0, 0.0, 4.0],
+            [4.0, 7.0, 0.0, 5.0],
+            [5.0, 8.0, 0.0, 6.0],
+        ],
+        dtype=np.float32,
+    ),
+    np.array([3, 2, 1], dtype=np.int64),
+)
+assert np.array_equal(
+    feats[1:2, :, :].as_array(),
+    np.array(
+        [
+            [3.0, 6.0, 0.0, 4.0],
+            [4.0, 7.0, 0.0, 5.0],
+        ],
+        dtype=np.float32,
+    ),
+), f"{feats[1:2, :, :].as_array()}"
+assert np.array_equal(
+    feats[:, :, 1:3].as_array(),
+    np.array(
+        [
+            [3.0, 1.0],
+            [4.0, 0.0],
+            [5.0, 1.0],
+            [6.0, 0.0],
+            [7.0, 0.0],
+            [8.0, 0.0],
+        ],
+        dtype=np.float32,
+    ),
+), f"{feats[:, :, 1:3].as_array()}"
+assert np.array_equal(
+    feats[:, 0, :].as_array(),
+    np.array(
+        [
+            [0.0, 3.0, 1.0, 1.0],
+            [3.0, 6.0, 0.0, 4.0],
+            [5.0, 8.0, 0.0, 6.0],
+        ],
+        dtype=np.float32,
+    ),
+), f"{feats[:, :, 0].as_array()}"
+assert np.array_equal(
+    feats[:, 0:2:3, :].size1(),
+    np.array([1, 1, 1], dtype=np.int64),
+), f"{feats[:, 0:2:3, :].size1()}"
+assert np.array_equal(
+    feats[:, 1:3, 0].size1(),
+    np.array([2, 1, 0], dtype=np.int64),
+), f"{feats[:, 1:3, 0].size1()}"
+assert np.array_equal(
+    feats[1:, 1:10, 0].size1(),
+    np.array([1, 0], dtype=np.int64),
+), f"{feats[1:, 1:10, 0].size1()}"
+
+
+# Test broadcasting concatenation along dim 2
+entities = RaggedBufferF32.from_flattened(
+    np.array(
+        [
+            [10, 3.0, 10, 1.0],
+            [11, 4.0, 11, 2.0],
+            [12, 5.0, 12, 3.0],
+            [13, 4.0, 13, 6.0],
+            [14, 5.0, 14, 7.0],
+            [15, 18.0, 15, 16.0],
+        ],
+        dtype=np.float32,
+    ),
+    np.array([3, 0, 2, 1], dtype=np.int64),
+)
+global_feats = RaggedBufferF32.from_array(
+    np.array(
+        [
+            [[0.0]],
+            [[1.0]],
+            [[2.0]],
+            [[3.0]],
+        ],
+        dtype=np.float32,
+    )
+)
+result = ragged_buffer.cat([entities, global_feats], dim=2)
+assert np.array_equal(
+    result.as_array(),
+    np.array(
+        [
+            [10, 3.0, 10, 1.0, 0.0],
+            [11, 4.0, 11, 2.0, 0.0],
+            [12, 5.0, 12, 3.0, 0.0],
+            [13, 4.0, 13, 6.0, 2.0],
+            [14, 5.0, 14, 7.0, 2.0],
+            [15, 18.0, 15, 16.0, 3.0],
+        ]
+    ),
+), f"{result}"
+
+# Test complex indexing
+sliced = entities[[1, 0], 0:3:2, [0, 3, 2]]
+assert np.array_equal(
+    sliced.as_array(),
+    np.array(
+        [
+            [10, 1.0, 10],
+            [12, 3.0, 12],
+        ]
+    ),
+), f"{sliced}"
+assert np.array_equal(
+    sliced.materialize().size1(),
+    np.array([0, 2], dtype=np.int64),
+), f"{sliced.size1()}"
+
+print("ALL TESTS PASSED")
```

### Comparing `ragged_buffer-0.4.4/PKG-INFO` & `ragged_buffer-0.4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,204 +1,205 @@
 Metadata-Version: 2.1
 Name: ragged-buffer
-Version: 0.4.4
+Version: 0.4.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: numpy~=1.21
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: Efficient RaggedBuffer datatype that implements 3D arrays with variable-length 2nd dimension.
 Author: Clemens Winter <clemenswinter1@gmail.com>
 Author-email: Clemens Winter <clemenswinter1@gmail.com>
 License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/entity-neural-network/ragged-buffer
 
-# ENN Ragged Buffer
-
-[![Actions Status](https://github.com/entity-neural-network/ragged-buffer/workflows/Test/badge.svg)](https://github.com/entity-neural-network/ragged-buffer/actions)
-[![PyPI](https://img.shields.io/pypi/v/ragged-buffer.svg?style=flat-square)](https://pypi.org/project/ragged-buffer/)
-[![Discord](https://img.shields.io/discord/913497968701747270?style=flat-square)](https://discord.gg/SjVqhSW4Qf)
-
-This Python package implements an efficient `RaggedBuffer` datatype that is similar to
-a 3D numpy array, but which allows for variable sequence length in the second
-dimension. It was created primarily for use in [enn-trainer](https://github.com/entity-neural-network/enn-trainer) 
-and currently only supports a small selection of the numpy array methods.
-
-![Ragged Buffer](https://user-images.githubusercontent.com/12845088/143787823-c6a585de-aeda-429c-9824-f4b4a98e6cea.png)
-
-## User Guide
-
-Install the package with `pip install ragged-buffer`.
-The package currently supports three `RaggedBuffer` variants, `RaggedBufferF32`, `RaggedBufferI64`, and `RaggedBufferBool`.
-
-<!-- no toc -->
-- [Creating a RaggedBuffer](#creating-a-raggedbuffer)
-- [Get size](#get-size)
-- [Convert to numpy array](#convert-to-numpy-array)
-- [Indexing](#indexing)
-- [Addition](#addition)
-- [Concatenation](#concatentation)
-- [Clear](#clear)
-
-### Creating a RaggedBuffer
-
-There are three ways to create a `RaggedBuffer`:
-- `RaggedBufferF32(features: int)` creates an empty `RaggedBuffer` with the specified number of features.
-- `RaggedBufferF32.from_flattened(flattened: np.ndarray, lenghts: np.ndarray)` creates a `RaggedBuffer` from a flattened 2D numpy array and a 1D numpy array of lengths.
-- `RaggedBufferF32.from_array` creates a `RaggedBuffer` (with equal sequence lenghts) from a 3D numpy array.
-
-Creating an empty buffer and pushing each row:
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-# Create an empty RaggedBuffer with a feature size of 3
-buffer = RaggedBufferF32(3)
-# Push sequences with 3, 5, 0, and 1 elements
-buffer.push(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]], dtype=np.float32))
-buffer.push(np.array([[10, 11, 12], [13, 14, 15], [16, 17, 18], [19, 20, 21], [22, 23, 24]], dtype=np.float32))
-buffer.push(np.array([], dtype=np.float32))  # Alternative: `buffer.push_empty()`
-buffer.push(np.array([[25, 25, 27]], dtype=np.float32))
-```
-
-Creating a RaggedBuffer from a flat 2D numpy array which combines the first and second dimension,
-and an array of sequence lengths:
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-buffer = RaggedBufferF32.from_flattened(
-    np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12], [13, 14, 15], [16, 17, 18], [19, 20, 21], [22, 23, 24], [25, 25, 27]], dtype=np.float32),
-    np.array([3, 5, 0, 1], dtype=np.int64))
-)
-```
-
-Creating a RaggedBuffer from a 3D numpy array (all sequences have the same length):
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-buffer = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
-```
-
-### Get size
-
-The `size0`, `size1`, and `size2` methods return the number of sequences, the number of elements in a sequence, and the number of features respectively.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-buffer = RaggedBufferF32.from_flattened(
-    np.zeros((9, 64), dtype=np.float32),
-    np.array([3, 5, 0, 1], dtype=np.int64))
-)
-
-# Get size of the first/batch dimension.
-assert buffer.size0() == 10
-# Get size of individual sequences.
-assert buffer.size1(1) == 5
-assert buffer.size1(2) == 0
-# Get size of the last/feature dimension.
-assert buffer.size2() == 64
-```
-
-### Convert to numpy array
-
-`as_aray` converts a `RaggedBuffer` to a flat 2D numpy array that combines the first and second dimension.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferI64
-
-buffer = RaggedBufferI64(1)
-buffer.push(np.array([[1], [1], [1]], dtype=np.int64))
-buffer.push(np.array([[2], [2]], dtype=np.int64))
-assert np.all(buffer.as_array(), np.array([[1], [1], [1], [2], [2]], dtype=np.int64))
-```
-
-### Indexing
-
-You can index a `RaggedBuffer` with a single integer (returning a `RaggedBuffer` with a single sequence), or with a numpy array of integers selecting/permuting multiple sequences.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-# Create a new `RaggedBufferF32`
-buffer = RaggedBufferF32.from_flattened(
-    np.arange(0, 40, dtype=np.float32).reshape(10, 4),
-    np.array([3, 5, 0, 1], dtype=np.int64)
-)
-
-# Retrieve the first sequence.
-assert np.all(
-    buffer[0].as_array() ==
-    np.array([[0, 1, 2, 3], [4, 5, 6, 7], [8, 9, 10, 11]], dtype=np.float32)
-)
-
-# Get a RaggedBatch with 2 randomly selected sequences.
-buffer[np.random.permutation(4)[:2]]
-```
-
-### Addition
-
-You can add two `RaggedBuffer`s with the `+` operator if they have the same number of sequences, sequence lengths, and features. You can also add a `RaggedBuffer` where all sequences have a length of 1 to a `RaggedBuffer` with variable length sequences, broadcasting along each sequence.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-# Create ragged buffer with dimensions (3, [1, 3, 2], 1)
-rb3 = RaggedBufferI64(1)
-rb3.push(np.array([[0]], dtype=np.int64))
-rb3.push(np.array([[0], [1], [2]], dtype=np.int64))
-rb3.push(np.array([[0], [5]], dtype=np.int64))
-
-# Create ragged buffer with dimensions (3, [1, 1, 1], 1)
-rb4 = RaggedBufferI64.from_array(np.array([0, 3, 10], dtype=np.int64).reshape(3, 1, 1))
-
-# Add rb3 and rb4, broadcasting along the sequence dimension.
-rb5 = rb3 + rb4
-assert np.all(
-    rb5.as_array() == np.array([[0], [3], [4], [5], [10], [15]], dtype=np.int64)
-)
-```
-
-### Concatenation
-
-The `extend` method can be used to mutate a `RaggedBuffer` by appending another `RaggedBuffer` to it.
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-
-rb1 = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
-rb2 = RaggedBufferF32.from_array(np.zeros((2, 5, 3), dtype=np.float32))
-rb1.extend(r2)
-assert rb1.size0() == 6
-```
-
-### Clear
-
-The `clear` method removes all elements from a `RaggedBuffer` without deallocating the underlying memory.
-
-
-```python
-import numpy as np
-from ragged_buffer import RaggedBufferF32
-
-rb = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
-rb.clear()
-assert rb.size0() == 0
-```
-
-## License
-
-ENN Ragged Buffer dual-licensed under Apache-2.0 and MIT.
+# ENN Ragged Buffer
+
+[![Actions Status](https://github.com/entity-neural-network/ragged-buffer/workflows/Test/badge.svg)](https://github.com/entity-neural-network/ragged-buffer/actions)
+[![PyPI](https://img.shields.io/pypi/v/ragged-buffer.svg?style=flat-square)](https://pypi.org/project/ragged-buffer/)
+[![Discord](https://img.shields.io/discord/913497968701747270?style=flat-square)](https://discord.gg/SjVqhSW4Qf)
+
+This Python package implements an efficient `RaggedBuffer` datatype that is similar to
+a 3D numpy array, but which allows for variable sequence length in the second
+dimension. It was created primarily for use in [enn-trainer](https://github.com/entity-neural-network/enn-trainer) 
+and currently only supports a small selection of the numpy array methods.
+
+![Ragged Buffer](https://user-images.githubusercontent.com/12845088/143787823-c6a585de-aeda-429c-9824-f4b4a98e6cea.png)
+
+## User Guide
+
+Install the package with `pip install ragged-buffer`.
+The package currently supports three `RaggedBuffer` variants, `RaggedBufferF32`, `RaggedBufferI64`, and `RaggedBufferBool`.
+
+<!-- no toc -->
+- [Creating a RaggedBuffer](#creating-a-raggedbuffer)
+- [Get size](#get-size)
+- [Convert to numpy array](#convert-to-numpy-array)
+- [Indexing](#indexing)
+- [Addition](#addition)
+- [Concatenation](#concatentation)
+- [Clear](#clear)
+
+### Creating a RaggedBuffer
+
+There are three ways to create a `RaggedBuffer`:
+- `RaggedBufferF32(features: int)` creates an empty `RaggedBuffer` with the specified number of features.
+- `RaggedBufferF32.from_flattened(flattened: np.ndarray, lenghts: np.ndarray)` creates a `RaggedBuffer` from a flattened 2D numpy array and a 1D numpy array of lengths.
+- `RaggedBufferF32.from_array` creates a `RaggedBuffer` (with equal sequence lenghts) from a 3D numpy array.
+
+Creating an empty buffer and pushing each row:
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+# Create an empty RaggedBuffer with a feature size of 3
+buffer = RaggedBufferF32(3)
+# Push sequences with 3, 5, 0, and 1 elements
+buffer.push(np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]], dtype=np.float32))
+buffer.push(np.array([[10, 11, 12], [13, 14, 15], [16, 17, 18], [19, 20, 21], [22, 23, 24]], dtype=np.float32))
+buffer.push(np.array([], dtype=np.float32))  # Alternative: `buffer.push_empty()`
+buffer.push(np.array([[25, 25, 27]], dtype=np.float32))
+```
+
+Creating a RaggedBuffer from a flat 2D numpy array which combines the first and second dimension,
+and an array of sequence lengths:
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+buffer = RaggedBufferF32.from_flattened(
+    np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12], [13, 14, 15], [16, 17, 18], [19, 20, 21], [22, 23, 24], [25, 25, 27]], dtype=np.float32),
+    np.array([3, 5, 0, 1], dtype=np.int64))
+)
+```
+
+Creating a RaggedBuffer from a 3D numpy array (all sequences have the same length):
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+buffer = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
+```
+
+### Get size
+
+The `size0`, `size1`, and `size2` methods return the number of sequences, the number of elements in a sequence, and the number of features respectively.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+buffer = RaggedBufferF32.from_flattened(
+    np.zeros((9, 64), dtype=np.float32),
+    np.array([3, 5, 0, 1], dtype=np.int64))
+)
+
+# Get size of the first/batch dimension.
+assert buffer.size0() == 10
+# Get size of individual sequences.
+assert buffer.size1(1) == 5
+assert buffer.size1(2) == 0
+# Get size of the last/feature dimension.
+assert buffer.size2() == 64
+```
+
+### Convert to numpy array
+
+`as_aray` converts a `RaggedBuffer` to a flat 2D numpy array that combines the first and second dimension.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferI64
+
+buffer = RaggedBufferI64(1)
+buffer.push(np.array([[1], [1], [1]], dtype=np.int64))
+buffer.push(np.array([[2], [2]], dtype=np.int64))
+assert np.all(buffer.as_array(), np.array([[1], [1], [1], [2], [2]], dtype=np.int64))
+```
+
+### Indexing
+
+You can index a `RaggedBuffer` with a single integer (returning a `RaggedBuffer` with a single sequence), or with a numpy array of integers selecting/permuting multiple sequences.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+# Create a new `RaggedBufferF32`
+buffer = RaggedBufferF32.from_flattened(
+    np.arange(0, 40, dtype=np.float32).reshape(10, 4),
+    np.array([3, 5, 0, 1], dtype=np.int64)
+)
+
+# Retrieve the first sequence.
+assert np.all(
+    buffer[0].as_array() ==
+    np.array([[0, 1, 2, 3], [4, 5, 6, 7], [8, 9, 10, 11]], dtype=np.float32)
+)
+
+# Get a RaggedBatch with 2 randomly selected sequences.
+buffer[np.random.permutation(4)[:2]]
+```
+
+### Addition
+
+You can add two `RaggedBuffer`s with the `+` operator if they have the same number of sequences, sequence lengths, and features. You can also add a `RaggedBuffer` where all sequences have a length of 1 to a `RaggedBuffer` with variable length sequences, broadcasting along each sequence.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+# Create ragged buffer with dimensions (3, [1, 3, 2], 1)
+rb3 = RaggedBufferI64(1)
+rb3.push(np.array([[0]], dtype=np.int64))
+rb3.push(np.array([[0], [1], [2]], dtype=np.int64))
+rb3.push(np.array([[0], [5]], dtype=np.int64))
+
+# Create ragged buffer with dimensions (3, [1, 1, 1], 1)
+rb4 = RaggedBufferI64.from_array(np.array([0, 3, 10], dtype=np.int64).reshape(3, 1, 1))
+
+# Add rb3 and rb4, broadcasting along the sequence dimension.
+rb5 = rb3 + rb4
+assert np.all(
+    rb5.as_array() == np.array([[0], [3], [4], [5], [10], [15]], dtype=np.int64)
+)
+```
+
+### Concatenation
+
+The `extend` method can be used to mutate a `RaggedBuffer` by appending another `RaggedBuffer` to it.
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+
+rb1 = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
+rb2 = RaggedBufferF32.from_array(np.zeros((2, 5, 3), dtype=np.float32))
+rb1.extend(r2)
+assert rb1.size0() == 6
+```
+
+### Clear
+
+The `clear` method removes all elements from a `RaggedBuffer` without deallocating the underlying memory.
+
+
+```python
+import numpy as np
+from ragged_buffer import RaggedBufferF32
+
+rb = RaggedBufferF32.from_array(np.zeros((4, 5, 3), dtype=np.float32))
+rb.clear()
+assert rb.size0() == 0
+```
+
+## License
+
+ENN Ragged Buffer dual-licensed under Apache-2.0 and MIT.
```

