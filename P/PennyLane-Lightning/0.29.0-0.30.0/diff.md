# Comparing `tmp/PennyLane-Lightning-0.29.0.tar.gz` & `tmp/PennyLane-Lightning-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PennyLane-Lightning-0.29.0.tar", last modified: Tue Feb 28 15:40:32 2023, max compression
+gzip compressed data, was "PennyLane-Lightning-0.30.0.tar", last modified: Mon May  1 17:21:51 2023, max compression
```

## Comparing `PennyLane-Lightning-0.29.0.tar` & `PennyLane-Lightning-0.30.0.tar`

### file list

```diff
@@ -1,188 +1,190 @@
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.155624 PennyLane-Lightning-0.29.0/
--rw-rw-r--   0 lee       (1001) lee       (1001)    11720 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/LICENSE
--rw-rw-r--   0 lee       (1001) lee       (1001)       46 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/MANIFEST.in
--rw-rw-r--   0 lee       (1001) lee       (1001)    10009 2023-02-28 15:40:32.155624 PennyLane-Lightning-0.29.0/PKG-INFO
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.119624 PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/
--rw-rw-r--   0 lee       (1001) lee       (1001)    10009 2023-02-28 15:40:32.000000 PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/PKG-INFO
--rw-rw-r--   0 lee       (1001) lee       (1001)     9414 2023-02-28 15:40:32.000000 PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/SOURCES.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)        1 2023-02-28 15:40:32.000000 PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/dependency_links.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)       73 2023-02-28 15:40:32.000000 PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/entry_points.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)       47 2023-02-28 15:40:32.000000 PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/requires.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)       40 2023-02-28 15:40:32.000000 PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/top_level.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)     8829 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/README.rst
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.119624 PennyLane-Lightning-0.29.0/pennylane_lightning/
--rw-rw-r--   0 lee       (1001) lee       (1001)      716 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/__init__.py
--rw-rw-r--   0 lee       (1001) lee       (1001)     6021 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/_serialize.py
--rw-rw-r--   0 lee       (1001) lee       (1001)      692 2023-02-28 15:40:22.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/_version.py
--rw-rw-r--   0 lee       (1001) lee       (1001)    36067 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/lightning_qubit.py
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.119624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/
--rw-rw-r--   0 lee       (1001) lee       (1001)     1449 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/CMakeLists.txt
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.123624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/
--rw-rw-r--   0 lee       (1001) lee       (1001)     1034 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/AdjointDiff.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     6028 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/AdjointDiff.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     6450 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/AlgUtil.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      726 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/CMakeLists.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)      862 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/JacobianTape.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    10403 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/JacobianTape.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1093 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4893 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.hpp
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.123624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/
--rw-rw-r--   0 lee       (1001) lee       (1001)     6882 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/AllOperations.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    11137 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_ApplyOperations.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4589 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_BitUtil.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5702 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_Kernels.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    17914 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_LinearAlgebra.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3978 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_Utils.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4092 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/CMakeLists.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)    28627 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/README.md
--rwxrwxr-x   0 lee       (1001) lee       (1001)      108 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/benchmark_all.sh
--rwxrwxr-x   0 lee       (1001) lee       (1001)     3853 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/plot_gate_benchmark.py
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.123624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/bindings/
--rw-rw-r--   0 lee       (1001) lee       (1001)    19732 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/bindings/Bindings.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    11906 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/bindings/Bindings.hpp
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.127624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/
--rw-rw-r--   0 lee       (1001) lee       (1001)     2923 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/CMakeLists.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)    14641 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/Constant.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    19275 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/DynamicDispatcher.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2282 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/GateOperation.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1776 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/GateUtil.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3191 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/GateUtil.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    19656 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/Gates.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      950 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/KernelType.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    26198 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/OpToMemberFuncPtr.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     9620 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernel.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1068 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_AVX2.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1078 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_AVX512.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1308 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_Default.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1791 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_x64.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      843 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_x64.hpp
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.131624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/
--rw-rw-r--   0 lee       (1001) lee       (1001)     3438 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX2.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3889 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX512.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    26076 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVXCommon.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    27378 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    90687 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    25048 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    61514 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2239 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/PauliGenerator.hpp
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.139624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/
--rw-rw-r--   0 lee       (1001) lee       (1001)     4208 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX2Concept.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4013 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX512Concept.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1456 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXConceptType.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1433 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXGateKernels.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    11500 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXUtil.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     7384 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCNOT.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    12414 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRX.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    12550 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRY.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    12070 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRZ.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    11384 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCY.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4048 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCZ.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     8773 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyControlledPhaseShift.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5210 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingXX.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5690 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingYY.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4958 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingZZ.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2961 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorPhaseShift.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3408 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyHadamard.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     7069 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXX.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    10159 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXY.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     7776 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingYY.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     6778 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingZZ.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2678 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliX.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3323 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliY.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2450 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliZ.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5139 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPhaseShift.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3669 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRX.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3639 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRY.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3864 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRZ.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4122 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyS.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     6674 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySWAP.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     7335 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySingleQubitOp.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5009 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyT.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3238 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Blender.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    12798 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Permutation.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1628 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/README.md
--rw-rw-r--   0 lee       (1001) lee       (1001)     8315 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/SingleQubitGateHelper.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    22206 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/TwoQubitGateHelper.hpp
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.143624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/
--rw-rw-r--   0 lee       (1001) lee       (1001)     4794 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      894 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5090 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      899 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    12598 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      830 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1026 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/CMakeLists.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)     3100 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/CPUMemoryModel.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    13533 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/KernelMap.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1066 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/KernelMap_Default.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2570 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/KernelMap_X64.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      851 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Measures.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    17653 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Measures.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1103 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Observables.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    14331 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Observables.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    14520 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorBase.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5476 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorCPU.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      781 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5924 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      769 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorRawCPU.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4719 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorRawCPU.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1730 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Threading.hpp
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.151624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/
--rw-rw-r--   0 lee       (1001) lee       (1001)     4330 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/CMakeLists.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)      416 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/CompareVector.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1083 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/CreateAllWires.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2824 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/CreateAllWires.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      790 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/README.md
--rw-rw-r--   0 lee       (1001) lee       (1001)     4291 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/TestConstant.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    15268 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/TestHelpers.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      380 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/TestKernels.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    15564 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_AVXSingleQubitGateHelpers.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    42963 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_AVXTwoQubitGateHelpers.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    24194 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_AdjDiff.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2675 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_AlgUtil.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Bindings.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      947 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_CompilerSupport.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5897 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_DynamicDispatcher.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2051 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Error.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     7642 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_CompareKernels.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5714 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Generator.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2528 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Inverse.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    55833 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Matrix.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    24510 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Nonparam.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)   106877 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Param.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3127 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateUtil.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5904 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Internal.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     8032 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_KernelMap.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5507 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Kokkos_Sparse.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    39241 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_LinearAlgebra.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    11361 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Measures.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3273 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Measures_Sparse.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    15067 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Observables.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    12496 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_OpToMemberFuncPtr.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      487 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_RuntimeInfo.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    11147 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_StateVecAdjDiff.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     7625 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_StateVectorManagedCPU.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2867 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_StateVectorRawCPU.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1864 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_TypeTraits.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    12910 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Util.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    26684 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_VectorJacobianProduct.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      153 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/compile_time_tests.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)       54 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/runner_main.cpp
-drwxrwxr-x   0 lee       (1001) lee       (1001)        0 2023-02-28 15:40:32.155624 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/
--rw-rw-r--   0 lee       (1001) lee       (1001)     2764 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/BitUtil.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      446 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/CMakeLists.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)     7443 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/ConstantUtil.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5161 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Error.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)      276 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Generators.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     3318 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/IntegerInterval.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     8856 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Kokkos_Sparse.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    31572 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/LinearAlgebra.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     7129 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Macros.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     5723 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Memory.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     4061 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/RuntimeInfo.cpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2095 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/RuntimeInfo.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     2562 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/TypeList.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)     1874 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/TypeTraits.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)    13409 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Util.hpp
--rw-rw-r--   0 lee       (1001) lee       (1001)       67 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/requirements.txt
--rw-rw-r--   0 lee       (1001) lee       (1001)       38 2023-02-28 15:40:32.155624 PennyLane-Lightning-0.29.0/setup.cfg
--rw-rw-r--   0 lee       (1001) lee       (1001)     6699 2023-02-28 15:40:07.000000 PennyLane-Lightning-0.29.0/setup.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11720 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/LICENSE
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       46 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/MANIFEST.in
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10009 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/PKG-INFO
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10009 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/PKG-INFO
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     9526 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)        1 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       73 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/entry_points.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       47 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/requires.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       40 2023-05-01 17:21:51.000000 PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/top_level.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8829 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/README.rst
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      716 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/__init__.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6972 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/_serialize.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      693 2023-05-01 17:21:46.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/_version.py
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    38964 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/lightning_qubit.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/src/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1449 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/CMakeLists.txt
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1034 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AdjointDiff.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6028 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AdjointDiff.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6450 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AlgUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      726 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      862 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/JacobianTape.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10403 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/JacobianTape.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1093 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4893 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6882 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/AllOperations.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11137 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_ApplyOperations.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4589 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_BitUtil.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5702 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_Kernels.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    17914 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_LinearAlgebra.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3978 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_Utils.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4092 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    28627 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/README.md
+-rwxr-xr-x   0 mlxd      (1000) mlxd      (1000)      108 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/benchmark_all.sh
+-rwxr-xr-x   0 mlxd      (1000) mlxd      (1000)     3853 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/plot_gate_benchmark.py
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.527851 PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    20837 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/Bindings.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11906 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/Bindings.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.531184 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2923 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14641 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/Constant.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    19322 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/DynamicDispatcher.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2282 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateOperation.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1776 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateUtil.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3191 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    19656 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/Gates.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      950 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/KernelType.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26198 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/OpToMemberFuncPtr.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     9620 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernel.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1068 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_AVX2.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1078 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_AVX512.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1308 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_Default.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1791 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_x64.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      843 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_x64.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.531184 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3438 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX2.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3889 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX512.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26076 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVXCommon.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    27378 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    90687 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    25048 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    61514 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2239 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/PauliGenerator.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.534517 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4208 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX2Concept.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4013 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX512Concept.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1456 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXConceptType.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1433 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXGateKernels.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11500 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7384 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCNOT.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12414 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12550 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12070 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11384 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4048 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8773 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyControlledPhaseShift.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5210 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingXX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5690 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingYY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4958 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingZZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2961 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorPhaseShift.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3408 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyHadamard.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7069 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    10159 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7776 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingYY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6778 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingZZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2678 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3323 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2450 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5139 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPhaseShift.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3669 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRX.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3639 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRY.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3864 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRZ.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4122 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyS.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     6674 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySWAP.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7335 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySingleQubitOp.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5009 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyT.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3238 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Blender.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12798 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Permutation.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1628 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/README.md
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8315 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/SingleQubitGateHelper.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    22206 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/TwoQubitGateHelper.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.534517 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4794 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      894 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5090 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      899 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12598 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      830 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1048 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3100 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/CPUMemoryModel.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    13533 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1066 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap_Default.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2570 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap_X64.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      851 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Measures.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    21397 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Measures.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1103 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Observables.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14331 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Observables.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    14520 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorBase.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5476 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorCPU.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      781 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5924 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      769 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorRawCPU.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4719 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorRawCPU.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1730 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Threading.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      405 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/TransitionKernels.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4965 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/TransitionKernels.hpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4494 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      416 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CompareVector.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1083 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CreateAllWires.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2824 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CreateAllWires.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      790 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/README.md
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4291 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestConstant.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15278 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestHelpers.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      380 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestKernels.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15564 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AVXSingleQubitGateHelpers.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    42963 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AVXTwoQubitGateHelpers.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    24194 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AdjDiff.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2675 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AlgUtil.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Bindings.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      947 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_CompilerSupport.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5897 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_DynamicDispatcher.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2051 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Error.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7642 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_CompareKernels.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5714 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Generator.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2528 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Inverse.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    55833 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Matrix.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    24510 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Nonparam.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)   106877 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Param.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3127 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateUtil.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5904 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Internal.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8032 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_KernelMap.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5507 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Kokkos_Sparse.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    39241 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_LinearAlgebra.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15851 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Measures.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3273 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Measures_Sparse.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    15067 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Observables.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12496 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_OpToMemberFuncPtr.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      487 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_RuntimeInfo.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    11147 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVecAdjDiff.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7625 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVectorManagedCPU.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2867 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVectorRawCPU.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1864 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_TypeTraits.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    12910 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Util.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    26684 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_VectorJacobianProduct.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      153 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/compile_time_tests.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       54 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/runner_main.cpp
+drwxr-xr-x   0 mlxd      (1000) mlxd      (1000)        0 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2764 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/BitUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      446 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/CMakeLists.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7443 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/ConstantUtil.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5161 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Error.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)      276 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Generators.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     3318 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/IntegerInterval.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     8856 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Kokkos_Sparse.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    31572 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/LinearAlgebra.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7129 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Macros.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     5723 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Memory.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     4061 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/RuntimeInfo.cpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2095 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/RuntimeInfo.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     2562 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/TypeList.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     1874 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/TypeTraits.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)    13409 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Util.hpp
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       67 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/requirements.txt
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)       38 2023-05-01 17:21:51.541184 PennyLane-Lightning-0.30.0/setup.cfg
+-rw-r--r--   0 mlxd      (1000) mlxd      (1000)     7938 2023-05-01 17:21:41.000000 PennyLane-Lightning-0.30.0/setup.py
```

### Comparing `PennyLane-Lightning-0.29.0/LICENSE` & `PennyLane-Lightning-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/PKG-INFO` & `PennyLane-Lightning-0.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Lightning
-Version: 0.29.0
+Version: 0.30.0
 Summary: PennyLane-Lightning plugin
 Home-page: https://github.com/XanaduAI/pennylane-lightning
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/PKG-INFO` & `PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PennyLane-Lightning
-Version: 0.29.0
+Version: 0.30.0
 Summary: PennyLane-Lightning plugin
 Home-page: https://github.com/XanaduAI/pennylane-lightning
 Maintainer: Xanadu Inc.
 Maintainer-email: software@xanadu.ai
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `PennyLane-Lightning-0.29.0/PennyLane_Lightning.egg-info/SOURCES.txt` & `PennyLane-Lightning-0.30.0/PennyLane_Lightning.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,16 @@
 pennylane_lightning/src/simulator/StateVectorBase.hpp
 pennylane_lightning/src/simulator/StateVectorCPU.hpp
 pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp
 pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp
 pennylane_lightning/src/simulator/StateVectorRawCPU.cpp
 pennylane_lightning/src/simulator/StateVectorRawCPU.hpp
 pennylane_lightning/src/simulator/Threading.hpp
+pennylane_lightning/src/simulator/TransitionKernels.cpp
+pennylane_lightning/src/simulator/TransitionKernels.hpp
 pennylane_lightning/src/tests/CMakeLists.txt
 pennylane_lightning/src/tests/CompareVector.hpp
 pennylane_lightning/src/tests/CreateAllWires.cpp
 pennylane_lightning/src/tests/CreateAllWires.hpp
 pennylane_lightning/src/tests/README.md
 pennylane_lightning/src/tests/TestConstant.hpp
 pennylane_lightning/src/tests/TestHelpers.hpp
```

### Comparing `PennyLane-Lightning-0.29.0/README.rst` & `PennyLane-Lightning-0.30.0/README.rst`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/__init__.py` & `PennyLane-Lightning-0.30.0/pennylane_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/_serialize.py` & `PennyLane-Lightning-0.30.0/pennylane_lightning/_serialize.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,21 +16,22 @@
 """
 from typing import List, Tuple
 
 import numpy as np
 from pennylane import (
     BasisState,
     Hadamard,
-    Projector,
-    Hamiltonian,
+    PauliX,
+    PauliY,
+    PauliZ,
+    Identity,
     QubitStateVector,
     Rot,
 )
-from pennylane.grouping import is_pauli_word
-from pennylane.operation import Observable, Tensor
+from pennylane.operation import Tensor
 from pennylane.tape import QuantumTape
 from pennylane.math import unwrap
 
 # Remove after the next release of PL
 # Add from pennylane import matrix
 import pennylane as qml
 
@@ -50,53 +51,43 @@
         HamiltonianC128,
         OpsStructC64,
         OpsStructC128,
     )
 except ImportError:
     pass
 
+pauli_name_map = {
+    "I": "Identity",
+    "X": "PauliX",
+    "Y": "PauliY",
+    "Z": "PauliZ",
+}
+
+
+def _serialize_named_obs(ob, wires_map: dict, use_csingle: bool):
+    """Serializes a Named observable"""
+    named_obs = NamedObsC64 if use_csingle else NamedObsC128
+    wires = [wires_map[w] for w in ob.wires]
+    if ob.name == "Identity":
+        wires = wires[:1]
+    return named_obs(ob.name, wires)
 
-def _obs_has_kernel(ob: Observable) -> bool:
-    """Returns True if the input observable has a supported kernel in the C++ backend.
 
-    Args:
-        ob (Observable): the input observable
-
-    Returns:
-        bool: indicating whether ``obs`` has a dedicated kernel in the backend
-    """
-    if is_pauli_word(ob):
-        return True
-    if isinstance(ob, (Hadamard)):
-        return True
-    if isinstance(ob, Hamiltonian):
-        return all(_obs_has_kernel(o) for o in ob.ops)
-    if isinstance(ob, Tensor):
-        return all(_obs_has_kernel(o) for o in ob.obs)
-
-    return False
-
-
-def _serialize_named_hermitian_ob(o, wires_map: dict, use_csingle: bool):
-    """Serializes an observable (Named or Hermitian)"""
+def _serialize_hermitian_ob(o, wires_map: dict, use_csingle: bool):
+    """Serializes a Hermitian observable"""
     assert not isinstance(o, Tensor)
 
     if use_csingle:
         ctype = np.complex64
-        named_obs = NamedObsC64
         hermitian_obs = HermitianObsC64
     else:
         ctype = np.complex128
-        named_obs = NamedObsC128
         hermitian_obs = HermitianObsC128
 
-    wires_list = o.wires.tolist()
-    wires = [wires_map[w] for w in wires_list]
-    if _obs_has_kernel(o):
-        return named_obs(o.name, wires)
+    wires = [wires_map[w] for w in o.wires]
     return hermitian_obs(qml.matrix(o).ravel().astype(ctype), wires)
 
 
 def _serialize_tensor_ob(ob, wires_map: dict, use_csingle: bool):
     """Serialize a tensor observable"""
     assert isinstance(ob, Tensor)
 
@@ -117,21 +108,58 @@
         hamiltonian_obs = HamiltonianC128
 
     coeffs = np.array(unwrap(ob.coeffs)).astype(rtype)
     terms = [_serialize_ob(t, wires_map, use_csingle) for t in ob.ops]
     return hamiltonian_obs(coeffs, terms)
 
 
+def _serialize_pauli_word(ob, wires_map: dict, use_csingle: bool):
+    """Serialize a :class:`pennylane.pauli.PauliWord` into a Named or Tensor observable."""
+    if use_csingle:
+        named_obs = NamedObsC64
+        tensor_obs = TensorProdObsC64
+    else:
+        named_obs = NamedObsC128
+        tensor_obs = TensorProdObsC128
+
+    if len(ob) == 1:
+        wire, pauli = list(ob.items())[0]
+        return named_obs(pauli_name_map[pauli], [wires_map[wire]])
+
+    return tensor_obs(
+        [named_obs(pauli_name_map[pauli], [wires_map[wire]]) for wire, pauli in ob.items()]
+    )
+
+
+def _serialize_pauli_sentence(ob, wires_map: dict, use_csingle: bool):
+    """Serialize a :class:`pennylane.pauli.PauliSentence` into a Hamiltonian."""
+    if use_csingle:
+        rtype = np.float32
+        hamiltonian_obs = HamiltonianC64
+    else:
+        rtype = np.float64
+        hamiltonian_obs = HamiltonianC128
+
+    pwords, coeffs = zip(*ob.items())
+    terms = [_serialize_pauli_word(pw, wires_map, use_csingle) for pw in pwords]
+    coeffs = np.array(coeffs).astype(rtype)
+    return hamiltonian_obs(coeffs, terms)
+
+
 def _serialize_ob(ob, wires_map, use_csingle):
     if isinstance(ob, Tensor):
         return _serialize_tensor_ob(ob, wires_map, use_csingle)
     elif ob.name == "Hamiltonian":
         return _serialize_hamiltonian(ob, wires_map, use_csingle)
+    elif isinstance(ob, (PauliX, PauliY, PauliZ, Identity, Hadamard)):
+        return _serialize_named_obs(ob, wires_map, use_csingle)
+    elif ob._pauli_rep is not None:
+        return _serialize_pauli_sentence(ob._pauli_rep, wires_map, use_csingle)
     else:
-        return _serialize_named_hermitian_ob(ob, wires_map, use_csingle)
+        return _serialize_hermitian_ob(ob, wires_map, use_csingle)
 
 
 def _serialize_observables(tape: QuantumTape, wires_map: dict, use_csingle: bool = False) -> List:
     """Serializes the observables of an input tape.
 
     Args:
         tape (QuantumTape): the input quantum tape
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/_version.py` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorRawCPU.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Copyright 2020 Xanadu Quantum Technologies Inc.
+// Copyright 2021 Xanadu Quantum Technologies Inc.
 
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+// Licensed under the Apache License, Version 2.0 (the "License");
+// you may not use this file except in compliance with the License.
+// You may obtain a copy of the License at
 
-#     http://www.apache.org/licenses/LICENSE-2.0
+//     http://www.apache.org/licenses/LICENSE-2.0
 
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+// Unless required by applicable law or agreed to in writing, software
+// distributed under the License is distributed on an "AS IS" BASIS,
+// WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+// See the License for the specific language governing permissions and
+// limitations under the License.
 
-"""Version information.
-   Version number (major.minor.patch[-label])
-"""
+#include "StateVectorRawCPU.hpp"
 
-__version__ = "0.29.0"
+// explicit instantiation
+template class Pennylane::StateVectorRawCPU<float>;
+template class Pennylane::StateVectorRawCPU<double>;
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/lightning_qubit.py` & `PennyLane-Lightning-0.30.0/pennylane_lightning/lightning_qubit.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,28 +156,46 @@
     Args:
         wires (int): the number of wires to initialize the device with
         c_dtype: Datatypes for statevector representation. Must be one of ``np.complex64`` or ``np.complex128``.
         shots (int): How many times the circuit should be evaluated (or sampled) to estimate
             the expectation values. Defaults to ``None`` if not specified. Setting
             to ``None`` results in computing statistics like expectation values and
             variances analytically.
+        mcmc (bool): Determine whether to use the approximate Markov Chain Monte Carlo sampling method when generating samples.
+        kernel_name (str): name of transition kernel. The current version supports two kernels: ``"Local"`` and ``"NonZeroRandom"``.
+            The local kernel conducts a bit-flip local transition between states. The local kernel generates a
+            random qubit site and then generates a random number to determine the new bit at that qubit site. The ``"NonZeroRandom"`` kernel
+            randomly transits between states that have nonzero probability.
+        num_burnin (int): number of steps that will be dropped. Increasing this value will
+        result in a closer approximation but increased runtime.
         batch_obs (bool): Determine whether we process observables parallelly when computing the
             jacobian. This value is only relevant when the lightning qubit is built with OpenMP.
     """
 
     name = "Lightning Qubit PennyLane plugin"
     short_name = "lightning.qubit"
     pennylane_requires = ">=0.26"
     version = __version__
     author = "Xanadu Inc."
     _CPP_BINARY_AVAILABLE = True
     operations = allowed_operations
     observables = allowed_observables
 
-    def __init__(self, wires, *, c_dtype=np.complex128, shots=None, batch_obs=False, analytic=None):
+    def __init__(
+        self,
+        wires,
+        *,
+        c_dtype=np.complex128,
+        shots=None,
+        mcmc=False,
+        kernel_name="Local",
+        num_burnin=100,
+        batch_obs=False,
+        analytic=None,
+    ):
         if c_dtype is np.complex64:
             r_dtype = np.float32
             self.use_csingle = True
         elif c_dtype is np.complex128:
             r_dtype = np.float64
             self.use_csingle = False
         else:
@@ -186,14 +204,28 @@
         self._batch_obs = batch_obs
 
         # Create the initial state. Internally, we store the
         # state as an array of dimension [2]*wires.
         self._state = self._create_basis_state(0)
         self._pre_rotated_state = self._state
 
+        self._mcmc = mcmc
+        if self._mcmc:
+            if kernel_name not in [
+                "Local",
+                "NonZeroRandom",
+            ]:
+                raise NotImplementedError(
+                    f"The {kernel_name} is not supported and currently only 'Local' and 'NonZeroRandom' kernels are supported."
+                )
+            if num_burnin >= shots:
+                raise ValueError("Shots should be greater than num_burnin.")
+            self._kernel_name = kernel_name
+            self._num_burnin = num_burnin
+
     @property
     def stopping_condition(self):
         """.BooleanFn: Returns the stopping condition for the device. The returned
         function accepts a queuable object (including a PennyLane operation
         and observable) and returns ``True`` if supported by the device."""
 
         def accepts_obj(obj):
@@ -495,17 +527,16 @@
             return None
 
         tp_shift = []
         record_tp_rows = []
         all_params = 0
 
         for op_idx, tp in enumerate(trainable_params):
-            op, _ = tape.get_operation(
-                op_idx
-            )  # get op_idx-th operator among differentiable operators
+            # get op_idx-th operator among differentiable operators
+            op, _, _ = tape.get_operation(op_idx)
             if isinstance(op, Operation) and not isinstance(op, (BasisState, QubitStateVector)):
                 # We now just ignore non-op or state preps
                 tp_shift.append(tp)
                 record_tp_rows.append(all_params)
             all_params += 1
 
         if use_sp:
@@ -575,15 +606,32 @@
                 processed_data["ops_serialized"],
                 trainable_params,
             )
         jac = np.array(jac)
         jac = jac.reshape(-1, len(trainable_params))
         jac_r = np.zeros((jac.shape[0], processed_data["all_params"]))
         jac_r[:, processed_data["record_tp_rows"]] = jac
-        return jac_r
+        return self._adjoint_jacobian_processing(jac_r) if qml.active_return() else jac_r
+
+    @staticmethod
+    def _adjoint_jacobian_processing(jac):
+        """
+        Post-process the Jacobian matrix returned by ``adjoint_jacobian`` for
+        the new return type system.
+        """
+        jac = np.squeeze(jac)
+
+        if jac.ndim == 0:
+            return np.array(jac)
+
+        if jac.ndim == 1:
+            return tuple(np.array(j) for j in jac)
+
+        # must be 2-dimensional
+        return tuple(tuple(np.array(j_) for j_ in j) for j in jac)
 
     def vjp(self, measurements, dy, starting_state=None, use_device_state=False):
         """Generate the processing function required to compute the vector-Jacobian products of a tape.
 
         This function can be used with multiple expectation values or a quantum state. When a quantum state
         is given,
 
@@ -599,15 +647,15 @@
             w_k = \\langle v| \\frac{\\partial}{\\partial \\theta_k} | \\psi_{\\pmb{\\theta}} \\rangle.
 
         Here, :math:`m` is the total number of trainable parameters, :math:`\\pmb{\\theta}` is the vector of trainable parameters and :math:`\\psi_{\\pmb{\\theta}}`
         is the output quantum state.
 
         Args:
             measurements (list): List of measurement processes for vector-Jacobian product. Now it must be expectation values or a quantum state.
-            dy (tensor_like): Gradient-output vector. Must have shape matching the output shape of the corresponding tape, i.e. number of measrurements if the return type is expectation or :math:`2^N` if the return type is statevector
+            dy (tensor_like): Gradient-output vector. Must have shape matching the output shape of the corresponding tape, i.e. number of measurements if the return type is expectation or :math:`2^N` if the return type is statevector
             starting_state (tensor_like): post-forward pass state to start execution with. It should be
                 complex-valued. Takes precedence over ``use_device_state``.
             use_device_state (bool): use current device state to initialize. A forward pass of the same
                 circuit should be the last thing the device has executed. If a ``starting_state`` is
                 provided, that takes precedence.
 
         Returns:
@@ -644,15 +692,15 @@
 
                 if num_params == 0:
                     return np.array([], dtype=self._state.dtype)
 
                 new_tape = tape.copy()
                 new_tape._measurements = [qml.expval(ham)]
 
-                return self.adjoint_jacobian(new_tape, starting_state, use_device_state).reshape(-1)
+                return self.adjoint_jacobian(new_tape, starting_state, use_device_state)
 
             return processing_fn
 
         if tape_return_type is State:
             if len(dy) != 2 ** len(self.wires):
                 raise ValueError(
                     "Size of the provided vector dy must be the same as the size of the statevector"
@@ -713,14 +761,21 @@
             fns.append(fn)
 
         def processing_fns(tapes):
             vjps = []
             for t, f in zip(tapes, fns):
                 vjp = f(t)
 
+                # make sure vjp is iterable if using extend reduction
+                if (
+                    not isinstance(vjp, tuple)
+                    and getattr(reduction, "__name__", reduction) == "extend"
+                ):
+                    vjp = (vjp,)
+
                 if isinstance(reduction, str):
                     getattr(vjps, reduction)(vjp)
                 elif callable(reduction):
                     reduction(vjps, vjp)
 
             return vjps
 
@@ -772,22 +827,25 @@
 
     def generate_samples(self):
         """Generate samples
 
         Returns:
             array[int]: array of samples in binary representation with shape ``(dev.shots, dev.num_wires)``
         """
-
         # Initialization of state
         ket = np.ravel(self._state)
 
         state_vector = StateVectorC64(ket) if self.use_csingle else StateVectorC128(ket)
         M = MeasuresC64(state_vector) if self.use_csingle else MeasuresC128(state_vector)
-
-        return M.generate_samples(len(self.wires), self.shots).astype(int, copy=False)
+        if self._mcmc:
+            return M.generate_mcmc_samples(
+                len(self.wires), self._kernel_name, self._num_burnin, self.shots
+            ).astype(int, copy=False)
+        else:
+            return M.generate_samples(len(self.wires), self.shots).astype(int, copy=False)
 
     def expval(self, observable, shot_range=None, bin_size=None):
         """Expectation value of the supplied observable.
 
         Args:
             observable: A PennyLane observable.
             shot_range (tuple[int]): 2-tuple of integers specifying the range of samples
@@ -902,14 +960,23 @@
             return M.var(ob_serialized)
 
         # translate to wire labels used by device
         observable_wires = self.map_wires(observable.wires)
 
         return M.var(observable.name, observable_wires)
 
+    def _get_diagonalizing_gates(self, circuit: qml.tape.QuantumTape) -> List[Operation]:
+        skip_diagonalizing = lambda obs: isinstance(obs, qml.Hamiltonian) or (
+            isinstance(obs, qml.ops.Sum) and obs._pauli_rep is not None
+        )
+        meas_filtered = list(
+            filter(lambda m: m.obs is None or not skip_diagonalizing(m.obs), circuit.measurements)
+        )
+        return super()._get_diagonalizing_gates(qml.tape.QuantumScript(measurements=meas_filtered))
+
 
 if not CPP_BINARY_AVAILABLE:
 
     class LightningQubit(DefaultQubit):  # pragma: no cover
         name = "Lightning Qubit PennyLane plugin"
         short_name = "lightning.qubit"
         pennylane_requires = ">=0.26"
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/CMakeLists.txt` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/AdjointDiff.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AdjointDiff.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/AdjointDiff.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AdjointDiff.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/AlgUtil.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/AlgUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/CMakeLists.txt` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/JacobianTape.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/JacobianTape.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/JacobianTape.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/JacobianTape.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/algorithms/StateVecAdjDiff.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/AllOperations.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/AllOperations.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_ApplyOperations.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_ApplyOperations.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_BitUtil.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_BitUtil.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_Kernels.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_Kernels.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_LinearAlgebra.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_LinearAlgebra.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/Bench_Utils.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/Bench_Utils.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/CMakeLists.txt` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/README.md` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/benchmarks/plot_gate_benchmark.py` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/benchmarks/plot_gate_benchmark.py`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/bindings/Bindings.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/Bindings.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -131,14 +131,35 @@
                      sz,            /* size of one scalar        */
                      py::format_descriptor<size_t>::format(), /* data type */
                      ndim,   /* number of dimensions      */
                      shape,  /* shape of the matrix       */
                      strides /* strides for each axis     */
                      ));
              })
+        .def("generate_mcmc_samples",
+             [](Measures<PrecisionT> &M, size_t num_wires,
+                const std::string &kernelname, size_t num_burnin,
+                size_t num_shots) {
+                 std::vector<size_t> &&result = M.generate_samples_metropolis(
+                     kernelname, num_burnin, num_shots);
+
+                 const size_t ndim = 2;
+                 const std::vector<size_t> shape{num_shots, num_wires};
+                 constexpr auto sz = sizeof(size_t);
+                 const std::vector<size_t> strides{sz * num_wires, sz};
+                 // return 2-D NumPy array
+                 return py::array(py::buffer_info(
+                     result.data(), /* data as contiguous array  */
+                     sz,            /* size of one scalar        */
+                     py::format_descriptor<size_t>::format(), /* data type */
+                     ndim,   /* number of dimensions      */
+                     shape,  /* shape of the matrix       */
+                     strides /* strides for each axis     */
+                     ));
+             })
         .def("var",
              [](Measures<PrecisionT> &M, const std::string &operation,
                 const std::vector<size_t> &wires) {
                  return M.var(operation, wires);
              })
         .def("var",
              static_cast<PrecisionT (Measures<PrecisionT>::*)(
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/bindings/Bindings.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/bindings/Bindings.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/CMakeLists.txt` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/Constant.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/Constant.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/DynamicDispatcher.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/DynamicDispatcher.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     /**
      * @brief Get all registered kernels
      */
     [[nodiscard]] auto registeredKernels() const
         -> std::vector<Gates::KernelType> {
         std::vector<Gates::KernelType> kernels;
 
+        kernels.reserve(kernel_names_.size());
         for (const auto &[kernel, name] : kernel_names_) {
             kernels.emplace_back(kernel);
         }
         return kernels;
     }
 
     /**
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/GateOperation.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateOperation.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/GateUtil.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateUtil.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/GateUtil.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/GateUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/Gates.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/Gates.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/KernelType.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/KernelType.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/OpToMemberFuncPtr.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/OpToMemberFuncPtr.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernel.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernel.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_AVX2.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_AVX2.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_AVX512.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_AVX512.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_Default.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_Default.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_x64.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_x64.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/RegisterKernels_x64.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/RegisterKernels_x64.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX2.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX2.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX512.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVX512.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVXCommon.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsAVXCommon.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsLM.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/GateImplementationsPI.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/PauliGenerator.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/PauliGenerator.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX2Concept.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX2Concept.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX512Concept.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVX512Concept.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXConceptType.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXConceptType.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXGateKernels.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXGateKernels.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXUtil.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/AVXUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCNOT.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCNOT.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRX.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRY.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRZ.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCRZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCY.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCZ.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyCZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyControlledPhaseShift.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyControlledPhaseShift.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingXX.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingXX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingYY.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingYY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingZZ.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorIsingZZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorPhaseShift.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyGeneratorPhaseShift.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyHadamard.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyHadamard.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXX.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXY.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingXY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingYY.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingYY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingZZ.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyIsingZZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliX.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliY.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliZ.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPauliZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPhaseShift.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyPhaseShift.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRX.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRX.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRY.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRY.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRZ.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyRZ.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyS.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyS.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySWAP.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySWAP.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySingleQubitOp.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplySingleQubitOp.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyT.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/ApplyT.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Blender.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Blender.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Permutation.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/Permutation.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/README.md` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/README.md`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/SingleQubitGateHelper.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/SingleQubitGateHelper.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/TwoQubitGateHelper.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/gates/cpu_kernels/avx_common/TwoQubitGateHelper.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX2.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_AVX512.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/AssignKernelMap_Default.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/CMakeLists.txt` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/CMakeLists.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 project(lightning_simulator)
 
-set(SIMULATOR_FILES StateVectorRawCPU.cpp Observables.cpp StateVectorManagedCPU.cpp Measures.cpp CACHE INTERNAL "" FORCE)
+set(SIMULATOR_FILES StateVectorRawCPU.cpp Observables.cpp StateVectorManagedCPU.cpp TransitionKernels.cpp Measures.cpp CACHE INTERNAL "" FORCE)
 
 add_library(lightning_simulator STATIC ${SIMULATOR_FILES})
 
 if (ENABLE_GATE_DISPATCHER AND UNIX AND (${CMAKE_SYSTEM_PROCESSOR} MATCHES "(AMD64)|(X64)|(x64)|(x86_64)"))
     target_sources(lightning_simulator PRIVATE KernelMap_X64.cpp AssignKernelMap_AVX2.cpp AssignKernelMap_AVX512.cpp AssignKernelMap_Default.cpp)
 else()
     target_sources(lightning_simulator PRIVATE KernelMap_Default.cpp AssignKernelMap_Default.cpp)
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/CPUMemoryModel.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/CPUMemoryModel.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/KernelMap.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/KernelMap_Default.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap_Default.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/KernelMap_X64.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/KernelMap_X64.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Measures.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Measures.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Measures.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Measures.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 #include <vector>
 
 #include "Kokkos_Sparse.hpp"
 #include "LinearAlgebra.hpp"
 #include "Observables.hpp"
 #include "StateVectorManagedCPU.hpp"
 #include "StateVectorRawCPU.hpp"
+#include "TransitionKernels.hpp"
 
 namespace Pennylane::Simulators {
 
 /**
  * @brief Observable's Measurement Class.
  *
  * This class performs measurements in the state vector provided to its
@@ -328,14 +329,114 @@
                 var(operations_list[index], wires_list[index]));
         }
 
         return expected_value_list;
     };
 
     /**
+     * @brief Complete a single Metropolis-Hastings step.
+     *
+     * @param sv state vector
+     * @param tk User-defined functor for producing transitions
+     * between metropolis states.
+     * @param gen Random number generator.
+     * @param distrib Random number distribution.
+     * @param init_idx Init index of basis state.
+     */
+    size_t metropolis_step(const SVType &sv,
+                           const std::unique_ptr<TransitionKernel<fp_t>> &tk,
+                           std::mt19937 &gen,
+                           std::uniform_real_distribution<fp_t> &distrib,
+                           size_t init_idx) {
+        auto init_plog = std::log(
+            (sv.getData()[init_idx] * std::conj(sv.getData()[init_idx]))
+                .real());
+
+        auto init_qratio = tk->operator()(init_idx);
+
+        // transition kernel outputs these two
+        auto &trans_idx = init_qratio.first;
+        auto &trans_qratio = init_qratio.second;
+
+        auto trans_plog = std::log(
+            (sv.getData()[trans_idx] * std::conj(sv.getData()[trans_idx]))
+                .real());
+
+        auto alph =
+            std::min<fp_t>(1., trans_qratio * std::exp(trans_plog - init_plog));
+        auto ran = distrib(gen);
+
+        if (ran < alph) {
+            return trans_idx;
+        }
+        return init_idx;
+    }
+
+    /**
+     * @brief Generate samples using the Metropolis-Hastings method.
+     * Reference: Numerical Recipes, NetKet paper
+     *
+     * @param transition_kernel User-defined functor for producing transitions
+     * between metropolis states.
+     * @param num_burnin Number of Metropolis burn-in steps.
+     * @param num_samples The number of samples to generate.
+     * @return 1-D vector of samples in binary, each sample is
+     * separated by a stride equal to the number of qubits.
+     */
+    std::vector<size_t>
+    generate_samples_metropolis(const std::string &kernelname,
+                                size_t num_burnin, size_t num_samples) {
+        size_t num_qubits = original_statevector.getNumQubits();
+        std::random_device rd;
+        std::mt19937 gen(rd());
+        std::uniform_real_distribution<fp_t> distrib(0.0, 1.0);
+        std::vector<size_t> samples(num_samples * num_qubits, 0);
+        std::unordered_map<size_t, size_t> cache;
+
+        TransitionKernelType transition_kernel =
+            Pennylane::TransitionKernelType::Local;
+        if (kernelname == "NonZeroRandom") {
+            transition_kernel = Pennylane::TransitionKernelType::NonZeroRandom;
+        }
+
+        auto tk =
+            kernel_factory(transition_kernel, original_statevector.getData(),
+                           original_statevector.getNumQubits());
+        size_t idx = 0;
+
+        // Burn In
+        for (size_t i = 0; i < num_burnin; i++) {
+            idx = metropolis_step(original_statevector, tk, gen, distrib,
+                                  idx); // Burn-in.
+        }
+
+        // Sample
+        for (size_t i = 0; i < num_samples; i++) {
+            idx = metropolis_step(original_statevector, tk, gen, distrib, idx);
+
+            if (cache.contains(idx)) {
+                size_t cache_id = cache[idx];
+                auto it_temp = samples.begin() + cache_id * num_qubits;
+                std::copy(it_temp, it_temp + num_qubits,
+                          samples.begin() + i * num_qubits);
+            }
+
+            // If not cached, compute
+            else {
+                for (size_t j = 0; j < num_qubits; j++) {
+                    samples[i * num_qubits + (num_qubits - 1 - j)] =
+                        (idx >> j) & 1U;
+                }
+                cache[idx] = i;
+            }
+        }
+        return samples;
+    }
+
+    /**
      * @brief Variance of a Sparse Hamiltonian.
      *
      * @tparam index_type integer type used as indices of the sparse matrix.
      * @param row_map_ptr   row_map array pointer.
      *                      The j element encodes the number of non-zeros above
      * row j.
      * @param row_map_size  row_map array size.
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Observables.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Observables.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Observables.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Observables.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorBase.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorBase.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorCPU.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorCPU.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorManagedCPU.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/StateVectorRawCPU.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/StateVectorRawCPU.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/simulator/Threading.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/simulator/Threading.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/CMakeLists.txt` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,17 @@
   Catch2
   GIT_REPOSITORY https://github.com/catchorg/Catch2.git
   GIT_TAG        v2.13.9
 )
 
 FetchContent_MakeAvailable(Catch2)
 
+get_target_property(CATCH2_IID Catch2 INTERFACE_INCLUDE_DIRECTORIES)
+set_target_properties(Catch2 PROPERTIES INTERFACE_SYSTEM_INCLUDE_DIRECTORIES "${CATCH2_IID}")
+
 # Required for catch_discover_tests().
 list(APPEND CMAKE_MODULE_PATH ${catch2_SOURCE_DIR}/contrib)
 
 # Modify `ctest` to only run the supported subset of tests.
 include(CTest)
 include(Catch)
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/CreateAllWires.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CreateAllWires.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/CreateAllWires.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/CreateAllWires.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/README.md` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/README.md`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/TestConstant.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestConstant.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/TestHelpers.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/TestHelpers.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -365,16 +365,16 @@
  * @param num_qubits number of qubits
  * @return StateVectorManaged<T>
  */
 template <typename T = double>
 StateVectorManagedCPU<T> Initializing_StateVector(size_t num_qubits = 3) {
     size_t data_size = Util::exp2(num_qubits);
 
-    std::vector<std::complex<T>> arr(data_size, 0);
-    arr[0] = 1;
+    std::vector<std::complex<T>> arr(data_size, {0, 0});
+    arr[0] = {1, 0};
     StateVectorManagedCPU<T> Measured_StateVector(arr.data(), data_size);
 
     std::vector<std::string> gates;
     std::vector<std::vector<size_t>> wires;
     std::vector<bool> inv_op(num_qubits * 2, false);
     std::vector<std::vector<T>> phase;
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_AVXSingleQubitGateHelpers.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AVXSingleQubitGateHelpers.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_AVXTwoQubitGateHelpers.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AVXTwoQubitGateHelpers.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_AdjDiff.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AdjDiff.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_AlgUtil.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_AlgUtil.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_CompilerSupport.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_CompilerSupport.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_DynamicDispatcher.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_DynamicDispatcher.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Error.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Error.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_CompareKernels.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_CompareKernels.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Generator.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Generator.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Inverse.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Inverse.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Matrix.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Matrix.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Nonparam.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Nonparam.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateImplementations_Param.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateImplementations_Param.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_GateUtil.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_GateUtil.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Internal.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Internal.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_KernelMap.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_KernelMap.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Kokkos_Sparse.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Kokkos_Sparse.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_LinearAlgebra.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_LinearAlgebra.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Measures.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Measures.cpp`

 * *Files 26% similar despite different names*

```diff
@@ -192,14 +192,128 @@
     // compare estimated probabilities to real probabilities
     SECTION("No wires provided:") {
         REQUIRE_THAT(probabilities,
                      Catch::Approx(expected_probabilities).margin(.05));
     }
 }
 
+TEMPLATE_TEST_CASE("Sample with Metropolis (Local Kernel)", "[Measures]", float,
+                   double) {
+    constexpr uint32_t twos[] = {
+        1U << 0U,  1U << 1U,  1U << 2U,  1U << 3U,  1U << 4U,  1U << 5U,
+        1U << 6U,  1U << 7U,  1U << 8U,  1U << 9U,  1U << 10U, 1U << 11U,
+        1U << 12U, 1U << 13U, 1U << 14U, 1U << 15U, 1U << 16U, 1U << 17U,
+        1U << 18U, 1U << 19U, 1U << 20U, 1U << 21U, 1U << 22U, 1U << 23U,
+        1U << 24U, 1U << 25U, 1U << 26U, 1U << 27U, 1U << 28U, 1U << 29U,
+        1U << 30U, 1U << 31U};
+
+    // Defining the State Vector that will be measured.
+    StateVectorManagedCPU<TestType> Measured_StateVector =
+        Initializing_StateVector<TestType>();
+
+    // Initializing the measures class.
+    // This object attaches to the statevector allowing several measures.
+    Measures<TestType, StateVectorManagedCPU<TestType>> Measurer(
+        Measured_StateVector);
+    vector<TestType> expected_probabilities = {
+        0.67078706, 0.03062806, 0.0870997,  0.00397696,
+        0.17564072, 0.00801973, 0.02280642, 0.00104134};
+
+    size_t num_qubits = 3;
+    size_t N = std::pow(2, num_qubits);
+    size_t num_samples = 100000;
+    size_t num_burnin = 1000;
+
+    std::string kernel = "Local";
+    auto &&samples =
+        Measurer.generate_samples_metropolis(kernel, num_burnin, num_samples);
+
+    std::vector<size_t> counts(N, 0);
+    std::vector<size_t> samples_decimal(num_samples, 0);
+
+    // convert samples to decimal and then bin them in counts
+    for (size_t i = 0; i < num_samples; i++) {
+        for (size_t j = 0; j < num_qubits; j++) {
+            if (samples[i * num_qubits + j] != 0) {
+                samples_decimal[i] += twos[(num_qubits - 1 - j)];
+            }
+        }
+        counts[samples_decimal[i]] += 1;
+    }
+
+    // compute estimated probabilities from histogram
+    std::vector<TestType> probabilities(counts.size());
+    for (size_t i = 0; i < counts.size(); i++) {
+        probabilities[i] = counts[i] / (TestType)num_samples;
+    }
+
+    // compare estimated probabilities to real probabilities
+    SECTION("No wires provided:") {
+        REQUIRE_THAT(probabilities,
+                     Catch::Approx(expected_probabilities).margin(.05));
+    }
+}
+
+TEMPLATE_TEST_CASE("Sample with Metropolis (NonZeroRandom Kernel)",
+                   "[Measures]", float, double) {
+    constexpr uint32_t twos[] = {
+        1U << 0U,  1U << 1U,  1U << 2U,  1U << 3U,  1U << 4U,  1U << 5U,
+        1U << 6U,  1U << 7U,  1U << 8U,  1U << 9U,  1U << 10U, 1U << 11U,
+        1U << 12U, 1U << 13U, 1U << 14U, 1U << 15U, 1U << 16U, 1U << 17U,
+        1U << 18U, 1U << 19U, 1U << 20U, 1U << 21U, 1U << 22U, 1U << 23U,
+        1U << 24U, 1U << 25U, 1U << 26U, 1U << 27U, 1U << 28U, 1U << 29U,
+        1U << 30U, 1U << 31U};
+
+    // Defining the State Vector that will be measured.
+    StateVectorManagedCPU<TestType> Measured_StateVector =
+        Initializing_StateVector<TestType>();
+
+    // Initializing the measures class.
+    // This object attaches to the statevector allowing several measures.
+    Measures<TestType, StateVectorManagedCPU<TestType>> Measurer(
+        Measured_StateVector);
+    vector<TestType> expected_probabilities = {
+        0.67078706, 0.03062806, 0.0870997,  0.00397696,
+        0.17564072, 0.00801973, 0.02280642, 0.00104134};
+
+    size_t num_qubits = 3;
+    size_t N = std::pow(2, num_qubits);
+    size_t num_samples = 100000;
+    size_t num_burnin = 1000;
+
+    const std::string kernel = "NonZeroRandom";
+    auto &&samples =
+        Measurer.generate_samples_metropolis(kernel, num_burnin, num_samples);
+
+    std::vector<size_t> counts(N, 0);
+    std::vector<size_t> samples_decimal(num_samples, 0);
+
+    // convert samples to decimal and then bin them in counts
+    for (size_t i = 0; i < num_samples; i++) {
+        for (size_t j = 0; j < num_qubits; j++) {
+            if (samples[i * num_qubits + j] != 0) {
+                samples_decimal[i] += twos[(num_qubits - 1 - j)];
+            }
+        }
+        counts[samples_decimal[i]] += 1;
+    }
+
+    // compute estimated probabilities from histogram
+    std::vector<TestType> probabilities(counts.size());
+    for (size_t i = 0; i < counts.size(); i++) {
+        probabilities[i] = counts[i] / (TestType)num_samples;
+    }
+
+    // compare estimated probabilities to real probabilities
+    SECTION("No wires provided:") {
+        REQUIRE_THAT(probabilities,
+                     Catch::Approx(expected_probabilities).margin(.05));
+    }
+}
+
 TEMPLATE_TEST_CASE("Variances", "[Measures]", float, double) {
     // Defining the State Vector that will be measured.
     StateVectorManagedCPU<TestType> Measured_StateVector =
         Initializing_StateVector<TestType>();
 
     // Initializing the measures class.
     // This object attaches to the statevector allowing several measures.
```

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Measures_Sparse.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Measures_Sparse.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Observables.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Observables.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_OpToMemberFuncPtr.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_OpToMemberFuncPtr.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_StateVecAdjDiff.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVecAdjDiff.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_StateVectorManagedCPU.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVectorManagedCPU.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_StateVectorRawCPU.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_StateVectorRawCPU.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_TypeTraits.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_TypeTraits.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_Util.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_Util.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/tests/Test_VectorJacobianProduct.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/tests/Test_VectorJacobianProduct.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/BitUtil.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/BitUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/ConstantUtil.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/ConstantUtil.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Error.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Error.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/IntegerInterval.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/IntegerInterval.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Kokkos_Sparse.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Kokkos_Sparse.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/LinearAlgebra.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/LinearAlgebra.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Macros.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Macros.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Memory.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Memory.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/RuntimeInfo.cpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/RuntimeInfo.cpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/RuntimeInfo.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/RuntimeInfo.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/TypeList.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/TypeList.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/TypeTraits.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/TypeTraits.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/pennylane_lightning/src/util/Util.hpp` & `PennyLane-Lightning-0.30.0/pennylane_lightning/src/util/Util.hpp`

 * *Files identical despite different names*

### Comparing `PennyLane-Lightning-0.29.0/setup.py` & `PennyLane-Lightning-0.30.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -85,40 +85,70 @@
         if platform.system() == "Darwin":
             # To support ARM64
             if os.getenv("ARCHS") == "arm64":
                 configure_args += [
                     "-DCMAKE_CXX_COMPILER_TARGET=arm64-apple-macos11",
                     "-DCMAKE_SYSTEM_NAME=Darwin",
                     "-DCMAKE_SYSTEM_PROCESSOR=ARM64",
+                    "-DENABLE_OPENMP=OFF",
                 ]
             else:  # X64 arch
-                if shutil.which("brew"):
-                    llvmpath = (
-                        subprocess.check_output(["brew", "--prefix", "llvm"]).decode().strip()
-                    )
+                # If we explicitly request a brew LLVM version, use that
+                if os.getenv("BREW_LLVM_VERSION") and shutil.which("brew"):
+                    brew_llvm_version = os.getenv("BREW_LLVM_VERSION")
+                    llvmpath = subprocess.run(
+                        [
+                            "brew",
+                            "--prefix",
+                            "llvm" + f"@{brew_llvm_version}" if brew_llvm_version else "",
+                        ],
+                        check=True,
+                        capture_output=True,
+                        text=True,
+                    ).stdout.strip()
+                
                 else:
+                    # No brew, use the default clang++ install provided by MacOS
                     llvmpath = shutil.which("clang++")
                     llvmpath = Path(llvmpath).parent.parent
+
+                # Ensure the appropriate compiler and linker are chosen
                 configure_args += [
                     f"-DCMAKE_CXX_COMPILER={llvmpath}/bin/clang++",
                     f"-DCMAKE_LINKER={llvmpath}/bin/lld",
                 ]  # Use clang instead of appleclang
-            # Disable OpenMP in M1 Macs
-            configure_args += [] if os.environ.get("USE_OMP") else ["-DENABLE_OPENMP=OFF"]
+
+                # Try to support OpenMP through libomp if available
+                if os.environ.get("USE_OMP") and shutil.which("brew"):
+                    libomp_path = subprocess.run(
+                        [
+                            "brew",
+                            "--prefix",
+                            "libomp",
+                        ],
+                        check=False,
+                        capture_output=True,
+                        text=True,
+                    ).stdout.strip()
+                    configure_args += (
+                        [f"-DOpenMP_ROOT={libomp_path}/"] if libomp_path else ["-DENABLE_OPENMP=OFF"]
+                    )
         elif platform.system() == "Windows":
             configure_args += ["-DENABLE_OPENMP=OFF", "-DENABLE_BLAS=OFF"]
         elif platform.system() != "Linux":
             raise RuntimeError(f"Unsupported '{platform.system()}' platform")
 
         if not Path(self.build_temp).exists():
             os.makedirs(self.build_temp)
 
-        subprocess.check_call(["cmake", str(ext.sourcedir)] + configure_args, cwd=self.build_temp)
-        subprocess.check_call(
-            ["cmake", "--build", ".", "--verbose"] + build_args, cwd=self.build_temp
+        subprocess.run(
+            ["cmake", str(ext.sourcedir)] + configure_args, cwd=self.build_temp, check=True
+        )
+        subprocess.run(
+            ["cmake", "--build", ".", "--verbose"] + build_args, cwd=self.build_temp, check=True
         )
 
 
 with open(os.path.join("pennylane_lightning", "_version.py")) as f:
     version = f.readlines()[-1].split()[-1].strip("\"'")
 
 requirements = [
```

