# Comparing `tmp/pyppin-1.0.6-py3.10.egg` & `tmp/pyppin-1.0.7-py3.10.egg`

## zipinfo {}

```diff
@@ -1,169 +1,181 @@
-Zip file size: 260250 bytes, number of entries: 167
--rw-r--r--  2.0 unx     1667 b- defN 22-Nov-17 14:11 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx     2292 b- defN 22-Nov-17 14:11 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Nov-17 14:11 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Nov-17 14:11 EGG-INFO/not-zip-safe
--rw-r--r--  2.0 unx       13 b- defN 22-Nov-17 14:11 EGG-INFO/top_level.txt
+Zip file size: 287313 bytes, number of entries: 179
+-rw-r--r--  2.0 unx     1667 b- defN 23-Apr-30 15:07 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx     2537 b- defN 23-Apr-30 15:07 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-30 15:07 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-30 15:07 EGG-INFO/not-zip-safe
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-30 15:07 EGG-INFO/top_level.txt
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 pyppin/__init__.py
--rw-r--r--  2.0 unx      146 b- defN 22-Nov-17 14:11 pyppin/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx      146 b- defN 23-Apr-30 15:07 pyppin/__pycache__/__init__.cpython-310.pyc
 -rw-r--r--  2.0 unx      524 b- defN 22-Jun-20 15:59 pyppin/base/__init__.py
--rw-r--r--  2.0 unx    18266 b- defN 22-Sep-30 14:49 pyppin/base/cache.py
--rw-r--r--  2.0 unx     6563 b- defN 22-Nov-17 14:11 pyppin/base/flex_decorator.py
--rw-r--r--  2.0 unx     2106 b- defN 22-Sep-28 11:43 pyppin/base/import_file.py
--rw-r--r--  2.0 unx     2595 b- defN 22-Jul-15 13:03 pyppin/base/lazyinit.py
+-rw-r--r--  2.0 unx    18266 b- defN 22-Nov-17 14:52 pyppin/base/cache.py
+-rw-r--r--  2.0 unx     6563 b- defN 22-Nov-17 14:52 pyppin/base/flex_decorator.py
+-rw-r--r--  2.0 unx     2106 b- defN 22-Nov-17 14:52 pyppin/base/import_file.py
+-rw-r--r--  2.0 unx     2595 b- defN 22-Nov-17 14:52 pyppin/base/lazyinit.py
 -rw-r--r--  2.0 unx     6200 b- defN 22-Jun-20 15:59 pyppin/base/registered_class.py
--rw-r--r--  2.0 unx      760 b- defN 22-Nov-17 14:11 pyppin/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx    15265 b- defN 22-Nov-17 14:11 pyppin/base/__pycache__/cache.cpython-310.pyc
--rw-r--r--  2.0 unx     4462 b- defN 22-Nov-17 14:11 pyppin/base/__pycache__/flex_decorator.cpython-310.pyc
--rw-r--r--  2.0 unx     1945 b- defN 22-Nov-17 14:11 pyppin/base/__pycache__/import_file.cpython-310.pyc
--rw-r--r--  2.0 unx     3095 b- defN 22-Nov-17 14:11 pyppin/base/__pycache__/lazyinit.cpython-310.pyc
--rw-r--r--  2.0 unx     5302 b- defN 22-Nov-17 14:11 pyppin/base/__pycache__/registered_class.cpython-310.pyc
--rw-r--r--  2.0 unx       31 b- defN 22-Jun-20 15:59 pyppin/containers/__init__.py
+-rw-r--r--  2.0 unx      760 b- defN 23-Apr-30 15:07 pyppin/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx    15265 b- defN 23-Apr-30 15:07 pyppin/base/__pycache__/cache.cpython-310.pyc
+-rw-r--r--  2.0 unx     4462 b- defN 23-Apr-30 15:07 pyppin/base/__pycache__/flex_decorator.cpython-310.pyc
+-rw-r--r--  2.0 unx     1945 b- defN 23-Apr-30 15:07 pyppin/base/__pycache__/import_file.cpython-310.pyc
+-rw-r--r--  2.0 unx     3095 b- defN 23-Apr-30 15:07 pyppin/base/__pycache__/lazyinit.cpython-310.pyc
+-rw-r--r--  2.0 unx     5302 b- defN 23-Apr-30 15:07 pyppin/base/__pycache__/registered_class.cpython-310.pyc
+-rw-r--r--  2.0 unx       32 b- defN 22-Nov-17 19:54 pyppin/containers/__init__.py
 -rw-r--r--  2.0 unx     1774 b- defN 22-Sep-28 16:17 pyppin/containers/iterators.py
+-rw-r--r--  2.0 unx    14626 b- defN 22-Nov-17 19:54 pyppin/containers/ring_buffer.py
 -rw-r--r--  2.0 unx    10897 b- defN 22-Jun-20 15:59 pyppin/containers/zip_by_key.py
--rw-r--r--  2.0 unx      193 b- defN 22-Nov-17 14:11 pyppin/containers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     1813 b- defN 22-Nov-17 14:11 pyppin/containers/__pycache__/iterators.cpython-310.pyc
--rw-r--r--  2.0 unx     9017 b- defN 22-Nov-17 14:11 pyppin/containers/__pycache__/zip_by_key.cpython-310.pyc
+-rw-r--r--  2.0 unx      194 b- defN 23-Apr-30 15:07 pyppin/containers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     1813 b- defN 23-Apr-30 15:07 pyppin/containers/__pycache__/iterators.cpython-310.pyc
+-rw-r--r--  2.0 unx    10013 b- defN 23-Apr-30 15:07 pyppin/containers/__pycache__/ring_buffer.cpython-310.pyc
+-rw-r--r--  2.0 unx     9017 b- defN 23-Apr-30 15:07 pyppin/containers/__pycache__/zip_by_key.cpython-310.pyc
 -rw-r--r--  2.0 unx       55 b- defN 22-Jun-20 15:59 pyppin/file/__init__.py
--rw-r--r--  2.0 unx     2271 b- defN 22-Sep-28 11:42 pyppin/file/dev_null.py
--rw-r--r--  2.0 unx     3792 b- defN 22-Sep-29 17:22 pyppin/file/memfile.py
--rw-r--r--  2.0 unx     4286 b- defN 22-Nov-17 14:11 pyppin/file/tee.py
--rw-r--r--  2.0 unx    15729 b- defN 22-Nov-17 14:11 pyppin/file/types.py
--rw-r--r--  2.0 unx      211 b- defN 22-Nov-17 14:11 pyppin/file/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     4592 b- defN 22-Nov-17 14:11 pyppin/file/__pycache__/dev_null.cpython-310.pyc
--rw-r--r--  2.0 unx     4177 b- defN 22-Nov-17 14:11 pyppin/file/__pycache__/memfile.cpython-310.pyc
--rw-r--r--  2.0 unx     5812 b- defN 22-Nov-17 14:11 pyppin/file/__pycache__/tee.cpython-310.pyc
--rw-r--r--  2.0 unx    13966 b- defN 22-Nov-17 14:11 pyppin/file/__pycache__/types.cpython-310.pyc
--rw-r--r--  2.0 unx     1847 b- defN 22-Sep-30 14:48 pyppin/iterators/__init__.py
--rw-r--r--  2.0 unx    10897 b- defN 22-Jun-20 15:59 pyppin/iterators/zip_by_key.py
--rw-r--r--  2.0 unx     1893 b- defN 22-Nov-17 14:11 pyppin/iterators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     9016 b- defN 22-Nov-17 14:11 pyppin/iterators/__pycache__/zip_by_key.cpython-310.pyc
--rw-r--r--  2.0 unx      922 b- defN 22-Sep-29 14:44 pyppin/math/__init__.py
--rw-r--r--  2.0 unx     2988 b- defN 22-Sep-29 17:22 pyppin/math/functions.py
--rw-r--r--  2.0 unx    13300 b- defN 22-Nov-17 14:11 pyppin/math/histogram.py
--rw-r--r--  2.0 unx    19340 b- defN 22-Nov-17 14:11 pyppin/math/plot_ascii.py
--rw-r--r--  2.0 unx     1172 b- defN 22-Nov-17 14:11 pyppin/math/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     3353 b- defN 22-Nov-17 14:11 pyppin/math/__pycache__/functions.cpython-310.pyc
--rw-r--r--  2.0 unx    12487 b- defN 22-Nov-17 14:11 pyppin/math/__pycache__/histogram.cpython-310.pyc
--rw-r--r--  2.0 unx    15356 b- defN 22-Nov-17 14:11 pyppin/math/__pycache__/plot_ascii.cpython-310.pyc
+-rw-r--r--  2.0 unx     2271 b- defN 22-Nov-17 14:52 pyppin/file/dev_null.py
+-rw-r--r--  2.0 unx     3792 b- defN 22-Nov-17 14:52 pyppin/file/memfile.py
+-rw-r--r--  2.0 unx     4286 b- defN 22-Nov-17 14:52 pyppin/file/tee.py
+-rw-r--r--  2.0 unx    15729 b- defN 22-Nov-17 14:52 pyppin/file/types.py
+-rw-r--r--  2.0 unx      211 b- defN 23-Apr-30 15:07 pyppin/file/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     4592 b- defN 23-Apr-30 15:07 pyppin/file/__pycache__/dev_null.cpython-310.pyc
+-rw-r--r--  2.0 unx     4177 b- defN 23-Apr-30 15:07 pyppin/file/__pycache__/memfile.cpython-310.pyc
+-rw-r--r--  2.0 unx     5812 b- defN 23-Apr-30 15:07 pyppin/file/__pycache__/tee.cpython-310.pyc
+-rw-r--r--  2.0 unx    13966 b- defN 23-Apr-30 15:07 pyppin/file/__pycache__/types.cpython-310.pyc
+-rw-r--r--  2.0 unx     1847 b- defN 22-Nov-17 14:52 pyppin/iterators/__init__.py
+-rw-r--r--  2.0 unx    10897 b- defN 22-Nov-17 14:52 pyppin/iterators/zip_by_key.py
+-rw-r--r--  2.0 unx     1893 b- defN 23-Apr-30 15:07 pyppin/iterators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     9016 b- defN 23-Apr-30 15:07 pyppin/iterators/__pycache__/zip_by_key.cpython-310.pyc
+-rw-r--r--  2.0 unx      922 b- defN 22-Nov-17 14:52 pyppin/math/__init__.py
+-rw-r--r--  2.0 unx     2988 b- defN 22-Nov-17 14:52 pyppin/math/functions.py
+-rw-r--r--  2.0 unx    13300 b- defN 22-Nov-17 14:52 pyppin/math/histogram.py
+-rw-r--r--  2.0 unx    19340 b- defN 22-Nov-17 14:52 pyppin/math/plot_ascii.py
+-rw-r--r--  2.0 unx     1172 b- defN 23-Apr-30 15:07 pyppin/math/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     3353 b- defN 23-Apr-30 15:07 pyppin/math/__pycache__/functions.cpython-310.pyc
+-rw-r--r--  2.0 unx    12487 b- defN 23-Apr-30 15:07 pyppin/math/__pycache__/histogram.cpython-310.pyc
+-rw-r--r--  2.0 unx    15356 b- defN 23-Apr-30 15:07 pyppin/math/__pycache__/plot_ascii.cpython-310.pyc
 -rw-r--r--  2.0 unx       34 b- defN 22-Jun-20 15:59 pyppin/os/__init__.py
--rw-r--r--  2.0 unx     3621 b- defN 22-Jul-15 13:04 pyppin/os/bulk_import.py
--rw-r--r--  2.0 unx     2857 b- defN 22-Sep-29 14:58 pyppin/os/list_files.py
--rw-r--r--  2.0 unx      188 b- defN 22-Nov-17 14:11 pyppin/os/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     3656 b- defN 22-Nov-17 14:11 pyppin/os/__pycache__/bulk_import.cpython-310.pyc
--rw-r--r--  2.0 unx     2568 b- defN 22-Nov-17 14:11 pyppin/os/__pycache__/list_files.cpython-310.pyc
+-rw-r--r--  2.0 unx     3621 b- defN 22-Nov-17 14:52 pyppin/os/bulk_import.py
+-rw-r--r--  2.0 unx     2857 b- defN 22-Nov-17 14:52 pyppin/os/list_files.py
+-rw-r--r--  2.0 unx      188 b- defN 23-Apr-30 15:07 pyppin/os/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     3656 b- defN 23-Apr-30 15:07 pyppin/os/__pycache__/bulk_import.cpython-310.pyc
+-rw-r--r--  2.0 unx     2568 b- defN 23-Apr-30 15:07 pyppin/os/__pycache__/list_files.cpython-310.pyc
 -rw-r--r--  2.0 unx       39 b- defN 22-Jun-20 15:59 pyppin/testing/__init__.py
--rw-r--r--  2.0 unx     3633 b- defN 22-Sep-29 14:59 pyppin/testing/interact.py
--rw-r--r--  2.0 unx     1154 b- defN 22-Sep-29 17:22 pyppin/testing/pprint_object.py
--rw-r--r--  2.0 unx     3246 b- defN 22-Sep-28 11:58 pyppin/testing/trace_on_failure.py
--rw-r--r--  2.0 unx    13508 b- defN 22-Sep-29 17:22 pyppin/testing/turn_taker.py
--rw-r--r--  2.0 unx      198 b- defN 22-Nov-17 14:11 pyppin/testing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     2866 b- defN 22-Nov-17 14:11 pyppin/testing/__pycache__/interact.cpython-310.pyc
--rw-r--r--  2.0 unx     1470 b- defN 22-Nov-17 14:11 pyppin/testing/__pycache__/pprint_object.cpython-310.pyc
--rw-r--r--  2.0 unx     3010 b- defN 22-Nov-17 14:11 pyppin/testing/__pycache__/trace_on_failure.cpython-310.pyc
--rw-r--r--  2.0 unx    12341 b- defN 22-Nov-17 14:11 pyppin/testing/__pycache__/turn_taker.cpython-310.pyc
--rw-r--r--  2.0 unx       38 b- defN 22-Sep-28 13:01 pyppin/text/__init__.py
--rw-r--r--  2.0 unx     8703 b- defN 22-Sep-30 14:49 pyppin/text/formatter.py
--rw-r--r--  2.0 unx     4929 b- defN 22-Sep-29 17:22 pyppin/text/now_and_then.py
--rw-r--r--  2.0 unx     5785 b- defN 22-Sep-30 14:49 pyppin/text/print_counter.py
--rw-r--r--  2.0 unx     8999 b- defN 22-Sep-30 14:49 pyppin/text/si_prefix.py
--rw-r--r--  2.0 unx     1852 b- defN 22-Sep-29 15:12 pyppin/text/sign.py
--rw-r--r--  2.0 unx      194 b- defN 22-Nov-17 14:11 pyppin/text/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     7746 b- defN 22-Nov-17 14:11 pyppin/text/__pycache__/formatter.cpython-310.pyc
--rw-r--r--  2.0 unx     4469 b- defN 22-Nov-17 14:11 pyppin/text/__pycache__/now_and_then.cpython-310.pyc
--rw-r--r--  2.0 unx     5802 b- defN 22-Nov-17 14:11 pyppin/text/__pycache__/print_counter.cpython-310.pyc
--rw-r--r--  2.0 unx     7407 b- defN 22-Nov-17 14:11 pyppin/text/__pycache__/si_prefix.cpython-310.pyc
--rw-r--r--  2.0 unx     1820 b- defN 22-Nov-17 14:11 pyppin/text/__pycache__/sign.cpython-310.pyc
+-rw-r--r--  2.0 unx     3633 b- defN 22-Nov-17 14:52 pyppin/testing/interact.py
+-rw-r--r--  2.0 unx     1154 b- defN 22-Nov-17 14:52 pyppin/testing/pprint_object.py
+-rw-r--r--  2.0 unx     3246 b- defN 22-Nov-17 14:52 pyppin/testing/trace_on_failure.py
+-rw-r--r--  2.0 unx    13508 b- defN 22-Nov-17 14:52 pyppin/testing/turn_taker.py
+-rw-r--r--  2.0 unx      198 b- defN 23-Apr-30 15:07 pyppin/testing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     2866 b- defN 23-Apr-30 15:07 pyppin/testing/__pycache__/interact.cpython-310.pyc
+-rw-r--r--  2.0 unx     1470 b- defN 23-Apr-30 15:07 pyppin/testing/__pycache__/pprint_object.cpython-310.pyc
+-rw-r--r--  2.0 unx     3010 b- defN 23-Apr-30 15:07 pyppin/testing/__pycache__/trace_on_failure.cpython-310.pyc
+-rw-r--r--  2.0 unx    12341 b- defN 23-Apr-30 15:07 pyppin/testing/__pycache__/turn_taker.cpython-310.pyc
+-rw-r--r--  2.0 unx       38 b- defN 22-Nov-17 14:52 pyppin/text/__init__.py
+-rw-r--r--  2.0 unx     8703 b- defN 22-Nov-17 14:52 pyppin/text/formatter.py
+-rw-r--r--  2.0 unx     4929 b- defN 22-Nov-17 14:52 pyppin/text/now_and_then.py
+-rw-r--r--  2.0 unx     5785 b- defN 22-Nov-17 14:52 pyppin/text/print_counter.py
+-rw-r--r--  2.0 unx     9104 b- defN 23-Apr-30 11:48 pyppin/text/si_prefix.py
+-rw-r--r--  2.0 unx     1852 b- defN 22-Nov-17 14:52 pyppin/text/sign.py
+-rw-r--r--  2.0 unx     2257 b- defN 23-Apr-30 15:04 pyppin/text/tty.py
+-rw-r--r--  2.0 unx      194 b- defN 23-Apr-30 15:07 pyppin/text/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     7746 b- defN 23-Apr-30 15:07 pyppin/text/__pycache__/formatter.cpython-310.pyc
+-rw-r--r--  2.0 unx     4469 b- defN 23-Apr-30 15:07 pyppin/text/__pycache__/now_and_then.cpython-310.pyc
+-rw-r--r--  2.0 unx     5802 b- defN 23-Apr-30 15:07 pyppin/text/__pycache__/print_counter.cpython-310.pyc
+-rw-r--r--  2.0 unx     7472 b- defN 23-Apr-30 15:07 pyppin/text/__pycache__/si_prefix.cpython-310.pyc
+-rw-r--r--  2.0 unx     1820 b- defN 23-Apr-30 15:07 pyppin/text/__pycache__/sign.cpython-310.pyc
+-rw-r--r--  2.0 unx     2653 b- defN 23-Apr-30 15:07 pyppin/text/__pycache__/tty.cpython-310.pyc
 -rw-r--r--  2.0 unx       36 b- defN 22-Jun-20 15:59 pyppin/threading/__init__.py
 -rw-r--r--  2.0 unx     5584 b- defN 22-Jun-20 15:59 pyppin/threading/periodic_task.py
--rw-r--r--  2.0 unx    15617 b- defN 22-Jul-22 17:15 pyppin/threading/semaphore.py
--rw-r--r--  2.0 unx     3214 b- defN 22-Sep-30 13:56 pyppin/threading/stack_trace.py
--rw-r--r--  2.0 unx    17491 b- defN 22-Nov-17 14:11 pyppin/threading/stack_trace_internals.py
--rw-r--r--  2.0 unx      197 b- defN 22-Nov-17 14:11 pyppin/threading/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     5253 b- defN 22-Nov-17 14:11 pyppin/threading/__pycache__/periodic_task.cpython-310.pyc
--rw-r--r--  2.0 unx    15303 b- defN 22-Nov-17 14:11 pyppin/threading/__pycache__/semaphore.cpython-310.pyc
--rw-r--r--  2.0 unx     3607 b- defN 22-Nov-17 14:11 pyppin/threading/__pycache__/stack_trace.cpython-310.pyc
--rw-r--r--  2.0 unx    16795 b- defN 22-Nov-17 14:11 pyppin/threading/__pycache__/stack_trace_internals.cpython-310.pyc
--rw-r--r--  2.0 unx       31 b- defN 22-Nov-17 14:11 pyppin/util/__init__.py
--rw-r--r--  2.0 unx    18687 b- defN 22-Nov-17 14:11 pyppin/util/expression.py
--rw-r--r--  2.0 unx      187 b- defN 22-Nov-17 14:11 pyppin/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx    15495 b- defN 22-Nov-17 14:11 pyppin/util/__pycache__/expression.cpython-310.pyc
+-rw-r--r--  2.0 unx    15617 b- defN 22-Nov-17 14:52 pyppin/threading/semaphore.py
+-rw-r--r--  2.0 unx     3214 b- defN 22-Nov-17 14:52 pyppin/threading/stack_trace.py
+-rw-r--r--  2.0 unx    17491 b- defN 22-Nov-17 14:52 pyppin/threading/stack_trace_internals.py
+-rw-r--r--  2.0 unx      197 b- defN 23-Apr-30 15:07 pyppin/threading/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     5253 b- defN 23-Apr-30 15:07 pyppin/threading/__pycache__/periodic_task.cpython-310.pyc
+-rw-r--r--  2.0 unx    15303 b- defN 23-Apr-30 15:07 pyppin/threading/__pycache__/semaphore.cpython-310.pyc
+-rw-r--r--  2.0 unx     3607 b- defN 23-Apr-30 15:07 pyppin/threading/__pycache__/stack_trace.cpython-310.pyc
+-rw-r--r--  2.0 unx    16795 b- defN 23-Apr-30 15:07 pyppin/threading/__pycache__/stack_trace_internals.cpython-310.pyc
+-rw-r--r--  2.0 unx       31 b- defN 22-Nov-17 14:52 pyppin/util/__init__.py
+-rw-r--r--  2.0 unx     6451 b- defN 23-Apr-30 15:05 pyppin/util/exponential_backoff.py
+-rw-r--r--  2.0 unx    18634 b- defN 22-Nov-17 19:54 pyppin/util/expression.py
+-rw-r--r--  2.0 unx      187 b- defN 23-Apr-30 15:07 pyppin/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     6098 b- defN 23-Apr-30 15:07 pyppin/util/__pycache__/exponential_backoff.cpython-310.pyc
+-rw-r--r--  2.0 unx    15465 b- defN 23-Apr-30 15:07 pyppin/util/__pycache__/expression.cpython-310.pyc
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 tests/base/__init__.py
--rw-r--r--  2.0 unx     4979 b- defN 22-Sep-07 11:15 tests/base/cache_test.py
--rw-r--r--  2.0 unx     1851 b- defN 22-Sep-07 11:14 tests/base/flex_decorator_test.py
+-rw-r--r--  2.0 unx     4979 b- defN 22-Nov-17 14:52 tests/base/cache_test.py
+-rw-r--r--  2.0 unx     1851 b- defN 22-Nov-17 14:52 tests/base/flex_decorator_test.py
 -rw-r--r--  2.0 unx     2179 b- defN 22-Jun-20 15:59 tests/base/lazyinit_test.py
 -rw-r--r--  2.0 unx     3100 b- defN 22-Jun-20 15:59 tests/base/registered_class_test.py
--rw-r--r--  2.0 unx      150 b- defN 22-Nov-17 14:11 tests/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     4526 b- defN 22-Nov-17 14:11 tests/base/__pycache__/cache_test.cpython-310.pyc
--rw-r--r--  2.0 unx     2758 b- defN 22-Nov-17 14:11 tests/base/__pycache__/flex_decorator_test.cpython-310.pyc
--rw-r--r--  2.0 unx     2628 b- defN 22-Nov-17 14:11 tests/base/__pycache__/lazyinit_test.cpython-310.pyc
--rw-r--r--  2.0 unx     3002 b- defN 22-Nov-17 14:11 tests/base/__pycache__/registered_class_test.cpython-310.pyc
--rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 tests/containers/__init__.py
+-rw-r--r--  2.0 unx      150 b- defN 23-Apr-30 15:07 tests/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     4526 b- defN 23-Apr-30 15:07 tests/base/__pycache__/cache_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     2758 b- defN 23-Apr-30 15:07 tests/base/__pycache__/flex_decorator_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     2628 b- defN 23-Apr-30 15:07 tests/base/__pycache__/lazyinit_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     3002 b- defN 23-Apr-30 15:07 tests/base/__pycache__/registered_class_test.cpython-310.pyc
+-rw-r--r--  2.0 unx        0 b- defN 22-Nov-17 19:54 tests/containers/__init__.py
 -rw-r--r--  2.0 unx     1788 b- defN 22-Sep-28 16:38 tests/containers/iterators_test.py
+-rw-r--r--  2.0 unx     7465 b- defN 22-Nov-17 19:54 tests/containers/ring_buffer_test.py
 -rw-r--r--  2.0 unx     6294 b- defN 22-Jun-20 15:59 tests/containers/zip_by_key_test.py
--rw-r--r--  2.0 unx      156 b- defN 22-Nov-17 14:11 tests/containers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     1904 b- defN 22-Nov-17 14:11 tests/containers/__pycache__/iterators_test.cpython-310.pyc
--rw-r--r--  2.0 unx     6915 b- defN 22-Nov-17 14:11 tests/containers/__pycache__/zip_by_key_test.cpython-310.pyc
+-rw-r--r--  2.0 unx      156 b- defN 23-Apr-30 15:07 tests/containers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     1904 b- defN 23-Apr-30 15:07 tests/containers/__pycache__/iterators_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     5587 b- defN 23-Apr-30 15:07 tests/containers/__pycache__/ring_buffer_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     6915 b- defN 23-Apr-30 15:07 tests/containers/__pycache__/zip_by_key_test.cpython-310.pyc
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 tests/file/__init__.py
--rw-r--r--  2.0 unx      424 b- defN 22-Sep-11 17:17 tests/file/dev_null_test.py
+-rw-r--r--  2.0 unx      424 b- defN 22-Nov-17 14:52 tests/file/dev_null_test.py
 -rw-r--r--  2.0 unx     6738 b- defN 22-Jun-20 15:59 tests/file/memfile_test.py
--rw-r--r--  2.0 unx      394 b- defN 22-Sep-11 17:16 tests/file/tee_test.py
--rw-r--r--  2.0 unx      150 b- defN 22-Nov-17 14:11 tests/file/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx      899 b- defN 22-Nov-17 14:11 tests/file/__pycache__/dev_null_test.cpython-310.pyc
--rw-r--r--  2.0 unx     4208 b- defN 22-Nov-17 14:11 tests/file/__pycache__/memfile_test.cpython-310.pyc
--rw-r--r--  2.0 unx      744 b- defN 22-Nov-17 14:11 tests/file/__pycache__/tee_test.cpython-310.pyc
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-28 16:47 tests/iterators/__init__.py
--rw-r--r--  2.0 unx     1777 b- defN 22-Sep-30 14:53 tests/iterators/iterators_test.py
--rw-r--r--  2.0 unx     6293 b- defN 22-Sep-29 12:54 tests/iterators/zip_by_key_test.py
--rw-r--r--  2.0 unx      155 b- defN 22-Nov-17 14:11 tests/iterators/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     1892 b- defN 22-Nov-17 14:11 tests/iterators/__pycache__/iterators_test.cpython-310.pyc
--rw-r--r--  2.0 unx     6913 b- defN 22-Nov-17 14:11 tests/iterators/__pycache__/zip_by_key_test.cpython-310.pyc
+-rw-r--r--  2.0 unx      394 b- defN 22-Nov-17 14:52 tests/file/tee_test.py
+-rw-r--r--  2.0 unx      150 b- defN 23-Apr-30 15:07 tests/file/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx      899 b- defN 23-Apr-30 15:07 tests/file/__pycache__/dev_null_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     4208 b- defN 23-Apr-30 15:07 tests/file/__pycache__/memfile_test.cpython-310.pyc
+-rw-r--r--  2.0 unx      744 b- defN 23-Apr-30 15:07 tests/file/__pycache__/tee_test.cpython-310.pyc
+-rw-r--r--  2.0 unx        0 b- defN 22-Nov-17 14:52 tests/iterators/__init__.py
+-rw-r--r--  2.0 unx     1777 b- defN 22-Nov-17 14:52 tests/iterators/iterators_test.py
+-rw-r--r--  2.0 unx     6293 b- defN 22-Nov-17 14:52 tests/iterators/zip_by_key_test.py
+-rw-r--r--  2.0 unx      155 b- defN 23-Apr-30 15:07 tests/iterators/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     1892 b- defN 23-Apr-30 15:07 tests/iterators/__pycache__/iterators_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     6913 b- defN 23-Apr-30 15:07 tests/iterators/__pycache__/zip_by_key_test.cpython-310.pyc
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 tests/math/__init__.py
 -rw-r--r--  2.0 unx      237 b- defN 22-Jun-20 15:59 tests/math/base_test.py
 -rw-r--r--  2.0 unx     3372 b- defN 22-Jun-20 15:59 tests/math/plot_ascii_test.py
--rw-r--r--  2.0 unx      150 b- defN 22-Nov-17 14:11 tests/math/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx      623 b- defN 22-Nov-17 14:11 tests/math/__pycache__/base_test.cpython-310.pyc
--rw-r--r--  2.0 unx     2620 b- defN 22-Nov-17 14:11 tests/math/__pycache__/plot_ascii_test.cpython-310.pyc
+-rw-r--r--  2.0 unx      150 b- defN 23-Apr-30 15:07 tests/math/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx      623 b- defN 23-Apr-30 15:07 tests/math/__pycache__/base_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     2620 b- defN 23-Apr-30 15:07 tests/math/__pycache__/plot_ascii_test.cpython-310.pyc
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 tests/os/__init__.py
 -rw-r--r--  2.0 unx      597 b- defN 22-Jun-20 15:59 tests/os/bulk_import_test.py
--rw-r--r--  2.0 unx     2166 b- defN 22-Jul-22 17:15 tests/os/list_files_test.py
--rw-r--r--  2.0 unx      148 b- defN 22-Nov-17 14:11 tests/os/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx      937 b- defN 22-Nov-17 14:11 tests/os/__pycache__/bulk_import_test.cpython-310.pyc
--rw-r--r--  2.0 unx     1632 b- defN 22-Nov-17 14:11 tests/os/__pycache__/list_files_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     2166 b- defN 22-Nov-17 14:52 tests/os/list_files_test.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Apr-30 15:07 tests/os/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx      937 b- defN 23-Apr-30 15:07 tests/os/__pycache__/bulk_import_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     1632 b- defN 23-Apr-30 15:07 tests/os/__pycache__/list_files_test.cpython-310.pyc
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 tests/os/bulk_import_test_data/__init__.py
 -rw-r--r--  2.0 unx      118 b- defN 22-Jun-20 15:59 tests/os/bulk_import_test_data/_def.py
 -rw-r--r--  2.0 unx      106 b- defN 22-Jun-20 15:59 tests/os/bulk_import_test_data/class1.py
 -rw-r--r--  2.0 unx      106 b- defN 22-Jun-20 15:59 tests/os/bulk_import_test_data/class2.py
--rw-r--r--  2.0 unx      170 b- defN 22-Nov-17 14:11 tests/os/bulk_import_test_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx      415 b- defN 22-Nov-17 14:11 tests/os/bulk_import_test_data/__pycache__/_def.cpython-310.pyc
--rw-r--r--  2.0 unx      400 b- defN 22-Nov-17 14:11 tests/os/bulk_import_test_data/__pycache__/class1.cpython-310.pyc
--rw-r--r--  2.0 unx      400 b- defN 22-Nov-17 14:11 tests/os/bulk_import_test_data/__pycache__/class2.cpython-310.pyc
+-rw-r--r--  2.0 unx      170 b- defN 23-Apr-30 15:07 tests/os/bulk_import_test_data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx      415 b- defN 23-Apr-30 15:07 tests/os/bulk_import_test_data/__pycache__/_def.cpython-310.pyc
+-rw-r--r--  2.0 unx      400 b- defN 23-Apr-30 15:07 tests/os/bulk_import_test_data/__pycache__/class1.cpython-310.pyc
+-rw-r--r--  2.0 unx      400 b- defN 23-Apr-30 15:07 tests/os/bulk_import_test_data/__pycache__/class2.cpython-310.pyc
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 tests/testing/__init__.py
 -rw-r--r--  2.0 unx     1094 b- defN 22-Jun-20 15:59 tests/testing/interact_test.py
--rw-r--r--  2.0 unx     2998 b- defN 22-Sep-07 11:18 tests/testing/trace_on_failure_test.py
+-rw-r--r--  2.0 unx     2998 b- defN 22-Nov-17 14:52 tests/testing/trace_on_failure_test.py
 -rw-r--r--  2.0 unx     2260 b- defN 22-Jun-20 15:59 tests/testing/turn_taker_test.py
--rw-r--r--  2.0 unx      153 b- defN 22-Nov-17 14:11 tests/testing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     1726 b- defN 22-Nov-17 14:11 tests/testing/__pycache__/interact_test.cpython-310.pyc
--rw-r--r--  2.0 unx     3660 b- defN 22-Nov-17 14:11 tests/testing/__pycache__/trace_on_failure_test.cpython-310.pyc
--rw-r--r--  2.0 unx     3176 b- defN 22-Nov-17 14:11 tests/testing/__pycache__/turn_taker_test.cpython-310.pyc
--rw-r--r--  2.0 unx        0 b- defN 22-Jul-18 14:13 tests/text/__init__.py
--rw-r--r--  2.0 unx      815 b- defN 22-Jul-22 17:15 tests/text/formatter_test.py
--rw-r--r--  2.0 unx     1801 b- defN 22-Sep-29 17:22 tests/text/now_and_then_test.py
--rw-r--r--  2.0 unx      930 b- defN 22-Jul-22 17:15 tests/text/print_counter_test.py
--rw-r--r--  2.0 unx     3655 b- defN 22-Jul-22 17:15 tests/text/si_prefix_test.py
--rw-r--r--  2.0 unx      150 b- defN 22-Nov-17 14:11 tests/text/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     1012 b- defN 22-Nov-17 14:11 tests/text/__pycache__/formatter_test.cpython-310.pyc
--rw-r--r--  2.0 unx     1601 b- defN 22-Nov-17 14:11 tests/text/__pycache__/now_and_then_test.cpython-310.pyc
--rw-r--r--  2.0 unx     1254 b- defN 22-Nov-17 14:11 tests/text/__pycache__/print_counter_test.cpython-310.pyc
--rw-r--r--  2.0 unx     3698 b- defN 22-Nov-17 14:11 tests/text/__pycache__/si_prefix_test.cpython-310.pyc
+-rw-r--r--  2.0 unx      153 b- defN 23-Apr-30 15:07 tests/testing/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     1726 b- defN 23-Apr-30 15:07 tests/testing/__pycache__/interact_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     3660 b- defN 23-Apr-30 15:07 tests/testing/__pycache__/trace_on_failure_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     3176 b- defN 23-Apr-30 15:07 tests/testing/__pycache__/turn_taker_test.cpython-310.pyc
+-rw-r--r--  2.0 unx        0 b- defN 22-Nov-17 14:52 tests/text/__init__.py
+-rw-r--r--  2.0 unx      815 b- defN 22-Nov-17 14:52 tests/text/formatter_test.py
+-rw-r--r--  2.0 unx     1801 b- defN 22-Nov-17 14:52 tests/text/now_and_then_test.py
+-rw-r--r--  2.0 unx      930 b- defN 22-Nov-17 14:52 tests/text/print_counter_test.py
+-rw-r--r--  2.0 unx     3683 b- defN 23-Apr-30 11:48 tests/text/si_prefix_test.py
+-rw-r--r--  2.0 unx      827 b- defN 23-Apr-30 15:04 tests/text/tty_test.py
+-rw-r--r--  2.0 unx      150 b- defN 23-Apr-30 15:07 tests/text/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     1012 b- defN 23-Apr-30 15:07 tests/text/__pycache__/formatter_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     1601 b- defN 23-Apr-30 15:07 tests/text/__pycache__/now_and_then_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     1254 b- defN 23-Apr-30 15:07 tests/text/__pycache__/print_counter_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     3704 b- defN 23-Apr-30 15:07 tests/text/__pycache__/si_prefix_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     1474 b- defN 23-Apr-30 15:07 tests/text/__pycache__/tty_test.cpython-310.pyc
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-20 15:59 tests/threading/__init__.py
 -rw-r--r--  2.0 unx     3125 b- defN 22-Jun-20 15:59 tests/threading/periodic_task_test.py
 -rw-r--r--  2.0 unx     6854 b- defN 22-Jun-20 15:59 tests/threading/semaphore_test.py
--rw-r--r--  2.0 unx      155 b- defN 22-Nov-17 14:11 tests/threading/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     3676 b- defN 22-Nov-17 14:11 tests/threading/__pycache__/periodic_task_test.cpython-310.pyc
--rw-r--r--  2.0 unx     6113 b- defN 22-Nov-17 14:11 tests/threading/__pycache__/semaphore_test.cpython-310.pyc
--rw-r--r--  2.0 unx        0 b- defN 22-Nov-17 14:11 tests/util/__init__.py
--rw-r--r--  2.0 unx     3281 b- defN 22-Nov-17 14:11 tests/util/expression_test.py
--rw-r--r--  2.0 unx      150 b- defN 22-Nov-17 14:11 tests/util/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     4652 b- defN 22-Nov-17 14:11 tests/util/__pycache__/expression_test.cpython-310.pyc
-167 files, 617023 bytes uncompressed, 234308 bytes compressed:  62.0%
+-rw-r--r--  2.0 unx      155 b- defN 23-Apr-30 15:07 tests/threading/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     3676 b- defN 23-Apr-30 15:07 tests/threading/__pycache__/periodic_task_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     6113 b- defN 23-Apr-30 15:07 tests/threading/__pycache__/semaphore_test.cpython-310.pyc
+-rw-r--r--  2.0 unx        0 b- defN 22-Nov-17 14:52 tests/util/__init__.py
+-rw-r--r--  2.0 unx     1789 b- defN 23-Apr-30 15:04 tests/util/exponential_backoff_test.py
+-rw-r--r--  2.0 unx     3281 b- defN 22-Nov-17 14:52 tests/util/expression_test.py
+-rw-r--r--  2.0 unx      150 b- defN 23-Apr-30 15:07 tests/util/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     2715 b- defN 23-Apr-30 15:07 tests/util/__pycache__/exponential_backoff_test.cpython-310.pyc
+-rw-r--r--  2.0 unx     4652 b- defN 23-Apr-30 15:07 tests/util/__pycache__/expression_test.cpython-310.pyc
+179 files, 679346 bytes uncompressed, 259439 bytes compressed:  61.8%
```

## zipnote «TEMP»/diffoscope__rjfn0jl_/tmppqaa_6fz_.zip

```diff
@@ -57,23 +57,29 @@
 
 Filename: pyppin/containers/__init__.py
 Comment: 
 
 Filename: pyppin/containers/iterators.py
 Comment: 
 
+Filename: pyppin/containers/ring_buffer.py
+Comment: 
+
 Filename: pyppin/containers/zip_by_key.py
 Comment: 
 
 Filename: pyppin/containers/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
 Filename: pyppin/containers/__pycache__/iterators.cpython-310.pyc
 Comment: 
 
+Filename: pyppin/containers/__pycache__/ring_buffer.cpython-310.pyc
+Comment: 
+
 Filename: pyppin/containers/__pycache__/zip_by_key.cpython-310.pyc
 Comment: 
 
 Filename: pyppin/file/__init__.py
 Comment: 
 
 Filename: pyppin/file/dev_null.py
@@ -201,14 +207,17 @@
 
 Filename: pyppin/text/si_prefix.py
 Comment: 
 
 Filename: pyppin/text/sign.py
 Comment: 
 
+Filename: pyppin/text/tty.py
+Comment: 
+
 Filename: pyppin/text/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
 Filename: pyppin/text/__pycache__/formatter.cpython-310.pyc
 Comment: 
 
 Filename: pyppin/text/__pycache__/now_and_then.cpython-310.pyc
@@ -219,14 +228,17 @@
 
 Filename: pyppin/text/__pycache__/si_prefix.cpython-310.pyc
 Comment: 
 
 Filename: pyppin/text/__pycache__/sign.cpython-310.pyc
 Comment: 
 
+Filename: pyppin/text/__pycache__/tty.cpython-310.pyc
+Comment: 
+
 Filename: pyppin/threading/__init__.py
 Comment: 
 
 Filename: pyppin/threading/periodic_task.py
 Comment: 
 
 Filename: pyppin/threading/semaphore.py
@@ -252,20 +264,26 @@
 
 Filename: pyppin/threading/__pycache__/stack_trace_internals.cpython-310.pyc
 Comment: 
 
 Filename: pyppin/util/__init__.py
 Comment: 
 
+Filename: pyppin/util/exponential_backoff.py
+Comment: 
+
 Filename: pyppin/util/expression.py
 Comment: 
 
 Filename: pyppin/util/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
+Filename: pyppin/util/__pycache__/exponential_backoff.cpython-310.pyc
+Comment: 
+
 Filename: pyppin/util/__pycache__/expression.cpython-310.pyc
 Comment: 
 
 Filename: tests/base/__init__.py
 Comment: 
 
 Filename: tests/base/cache_test.py
@@ -297,23 +315,29 @@
 
 Filename: tests/containers/__init__.py
 Comment: 
 
 Filename: tests/containers/iterators_test.py
 Comment: 
 
+Filename: tests/containers/ring_buffer_test.py
+Comment: 
+
 Filename: tests/containers/zip_by_key_test.py
 Comment: 
 
 Filename: tests/containers/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
 Filename: tests/containers/__pycache__/iterators_test.cpython-310.pyc
 Comment: 
 
+Filename: tests/containers/__pycache__/ring_buffer_test.cpython-310.pyc
+Comment: 
+
 Filename: tests/containers/__pycache__/zip_by_key_test.cpython-310.pyc
 Comment: 
 
 Filename: tests/file/__init__.py
 Comment: 
 
 Filename: tests/file/dev_null_test.py
@@ -450,14 +474,17 @@
 
 Filename: tests/text/print_counter_test.py
 Comment: 
 
 Filename: tests/text/si_prefix_test.py
 Comment: 
 
+Filename: tests/text/tty_test.py
+Comment: 
+
 Filename: tests/text/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
 Filename: tests/text/__pycache__/formatter_test.cpython-310.pyc
 Comment: 
 
 Filename: tests/text/__pycache__/now_and_then_test.cpython-310.pyc
@@ -465,14 +492,17 @@
 
 Filename: tests/text/__pycache__/print_counter_test.cpython-310.pyc
 Comment: 
 
 Filename: tests/text/__pycache__/si_prefix_test.cpython-310.pyc
 Comment: 
 
+Filename: tests/text/__pycache__/tty_test.cpython-310.pyc
+Comment: 
+
 Filename: tests/threading/__init__.py
 Comment: 
 
 Filename: tests/threading/periodic_task_test.py
 Comment: 
 
 Filename: tests/threading/semaphore_test.py
@@ -486,17 +516,23 @@
 
 Filename: tests/threading/__pycache__/semaphore_test.cpython-310.pyc
 Comment: 
 
 Filename: tests/util/__init__.py
 Comment: 
 
+Filename: tests/util/exponential_backoff_test.py
+Comment: 
+
 Filename: tests/util/expression_test.py
 Comment: 
 
 Filename: tests/util/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
+Filename: tests/util/__pycache__/exponential_backoff_test.cpython-310.pyc
+Comment: 
+
 Filename: tests/util/__pycache__/expression_test.cpython-310.pyc
 Comment: 
 
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyppin
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python tools collection
 Author: Yonatan Zunger
 Author-email: zunger@gmail.com
 License: Apache
 Project-URL: Source, https://github.com/yonatanzunger/pyppin
 Project-URL: Tracker, https://github.com/yonatanzunger/pyppin/issues
 Project-URL: Documentation, https://yonatanzunger.github.io/pyppin/
```

## EGG-INFO/SOURCES.txt

```diff
@@ -9,14 +9,16 @@
 pyppin.egg-info/top_level.txt
 pyppin/base/__init__.py
 pyppin/base/cache.py
 pyppin/base/flex_decorator.py
 pyppin/base/import_file.py
 pyppin/base/lazyinit.py
 pyppin/base/registered_class.py
+pyppin/containers/__init__.py
+pyppin/containers/ring_buffer.py
 pyppin/file/__init__.py
 pyppin/file/dev_null.py
 pyppin/file/memfile.py
 pyppin/file/tee.py
 pyppin/file/types.py
 pyppin/iterators/__init__.py
 pyppin/iterators/zip_by_key.py
@@ -34,26 +36,30 @@
 pyppin/testing/turn_taker.py
 pyppin/text/__init__.py
 pyppin/text/formatter.py
 pyppin/text/now_and_then.py
 pyppin/text/print_counter.py
 pyppin/text/si_prefix.py
 pyppin/text/sign.py
+pyppin/text/tty.py
 pyppin/threading/__init__.py
 pyppin/threading/periodic_task.py
 pyppin/threading/semaphore.py
 pyppin/threading/stack_trace.py
 pyppin/threading/stack_trace_internals.py
 pyppin/util/__init__.py
+pyppin/util/exponential_backoff.py
 pyppin/util/expression.py
 tests/base/__init__.py
 tests/base/cache_test.py
 tests/base/flex_decorator_test.py
 tests/base/lazyinit_test.py
 tests/base/registered_class_test.py
+tests/containers/__init__.py
+tests/containers/ring_buffer_test.py
 tests/file/__init__.py
 tests/file/dev_null_test.py
 tests/file/memfile_test.py
 tests/file/tee_test.py
 tests/iterators/__init__.py
 tests/iterators/iterators_test.py
 tests/iterators/zip_by_key_test.py
@@ -72,12 +78,14 @@
 tests/testing/trace_on_failure_test.py
 tests/testing/turn_taker_test.py
 tests/text/__init__.py
 tests/text/formatter_test.py
 tests/text/now_and_then_test.py
 tests/text/print_counter_test.py
 tests/text/si_prefix_test.py
+tests/text/tty_test.py
 tests/threading/__init__.py
 tests/threading/periodic_task_test.py
 tests/threading/semaphore_test.py
 tests/util/__init__.py
+tests/util/exponential_backoff_test.py
 tests/util/expression_test.py
```

## pyppin/base/__pycache__/cache.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 21:49:12 2022 UTC, .py size: 18266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5864 3763 5a47 0000  o.......Xd7cZG..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 5a47 0000  o.......!.vcZG..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0010 0000 0040 0000 0073 6402 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6401 6404 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 6d10 5a10  m.Z.m.Z.m.Z.m.Z.
```

## pyppin/base/__pycache__/flex_decorator.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 6563 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 a319 0000  o.......y.vc....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 a319 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 6d0a 5a0a 0100 6508 6405 6506 6406 6505  m.Z...e.d.e.d.e.
 00000070: 6602 1900 6407 8d02 5a0b 6408 6506 6409  f...d...Z.d.e.d.
```

## pyppin/base/__pycache__/import_file.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Sep 28 18:43:15 2022 UTC, .py size: 2106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c395 3463 3a08 0000  o.........4c:...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 3a08 0000  o.......!.vc:...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6403 6c04 6d05 5a05 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 0907 640e 6408 650a 650d  m.Z.....d.d.e.e.
```

## pyppin/base/__pycache__/lazyinit.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 15 20:03:25 2022 UTC, .py size: 2595 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0dc8 d162 230a 0000  o..........b#...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 230a 0000  o.......!.vc#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 0100 6506  m.Z.m.Z.m.Z...e.
 00000050: 6403 8301 5a07 6404 5a08 4700 6405 6406  d...Z.d.Z.G.d.d.
 00000060: 8400 6406 6504 6507 1900 8303 5a09 6407  ..d.e.e.....Z.d.
 00000070: 6503 6502 6701 6507 6602 1900 6408 6509  e.e.g.e.f...d.e.
```

## pyppin/containers/__init__.py

```diff
@@ -1 +1 @@
-"""Containers and iterators"""
+"""Useful container classes."""
```

## pyppin/containers/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 20 22:59:42 2022 UTC, .py size: 31 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,13 +1,13 @@
-00000000: 6f0d 0d0a 0000 0000 defb b062 1f00 0000  o..........b....
+00000000: 6f0d 0d0a 0000 0000 d901 7763 2000 0000  o.........wc ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0800 0000 6400  .....@...s....d.
-00000030: 5a00 6401 5300 2902 7a18 436f 6e74 6169  Z.d.S.).z.Contai
-00000040: 6e65 7273 2061 6e64 2069 7465 7261 746f  ners and iterato
-00000050: 7273 4e29 01da 075f 5f64 6f63 5f5f a900  rsN)...__doc__..
-00000060: 7202 0000 0072 0200 0000 fa40 6275 696c  r....r.....@buil
-00000070: 642f 6264 6973 742e 6d61 636f 7378 2d31  d/bdist.macosx-1
-00000080: 322e 342d 7838 365f 3634 2f65 6767 2f70  2.4-x86_64/egg/p
-00000090: 7970 7069 6e2f 636f 6e74 6169 6e65 7273  yppin/containers
-000000a0: 2f5f 5f69 6e69 745f 5f2e 7079 da08 3c6d  /__init__.py..<m
-000000b0: 6f64 756c 653e 0100 0000 7302 0000 0008  odule>....s.....
-000000c0: 00                                       .
+00000030: 5a00 6401 5300 2902 7a19 5573 6566 756c  Z.d.S.).z.Useful
+00000040: 2063 6f6e 7461 696e 6572 2063 6c61 7373   container class
+00000050: 6573 2e4e 2901 da07 5f5f 646f 635f 5fa9  es.N)...__doc__.
+00000060: 0072 0200 0000 7202 0000 00fa 4062 7569  .r....r.....@bui
+00000070: 6c64 2f62 6469 7374 2e6d 6163 6f73 782d  ld/bdist.macosx-
+00000080: 3132 2e34 2d78 3836 5f36 342f 6567 672f  12.4-x86_64/egg/
+00000090: 7079 7070 696e 2f63 6f6e 7461 696e 6572  pyppin/container
+000000a0: 732f 5f5f 696e 6974 5f5f 2e70 79da 083c  s/__init__.py..<
+000000b0: 6d6f 6475 6c65 3e01 0000 0073 0200 0000  module>....s....
+000000c0: 0800                                     ..
```

## pyppin/file/__pycache__/dev_null.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Sep 28 18:42:13 2022 UTC, .py size: 2271 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8595 3463 df08 0000  o.........4c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 df08 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 6d09 5a09 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c0a 6d0b 5a0b 6d0c 5a0c 0100 4700  d.l.m.Z.m.Z...G.
 00000070: 6405 6406 8400 6406 6501 6a0d 8303 5a0e  d.d...d.e.j...Z.
```

## pyppin/file/__pycache__/memfile.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 00:22:00 2022 UTC, .py size: 3792 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a836 3663 d00e 0000  o........66c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 d00e 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6506 8303 5a09 6406 5300 2907  ..d.e...Z.d.S.).
 00000070: 7a45 416c 6c6f 7720 6163 6365 7373 2074  zEAllow access t
```

## pyppin/file/__pycache__/tee.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 4286 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 be10 0000  o.......y.vc....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 be10 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6401  m.Z.m.Z.m.Z...d.
 00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6406 6701 5a0b  m.Z.m.Z...d.g.Z.
 00000070: 6407 650a 6408 650a 6604 6409 6406 8404  d.e.d.e.f.d.d...
```

## pyppin/file/__pycache__/types.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 15729 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 713d 0000  o.......y.vcq=..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 713d 0000  o.......!.vcq=..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 3001 0000 6400  .....@...s0...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 6401 6404 6c09  m.Z.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6401 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
```

## pyppin/iterators/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 21:48:26 2022 UTC, .py size: 1847 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2a64 3763 3707 0000  o.......*d7c7...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 3707 0000  o.......!.vc7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 650a 6405 8301  m.Z.m.Z...e.d...
 00000070: 5a0b 650a 6406 8301 5a0c 6407 6508 650b  Z.e.d...Z.d.e.e.
```

## pyppin/iterators/__pycache__/zip_by_key.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 20 22:59:42 2022 UTC, .py size: 10897 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 defb b062 912a 0000  o..........b.*..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 912a 0000  o.......!.vc.*..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000c 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 6d04 5a04 6d05 5a05 6d06 5a06 6d07 5a07  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6509  m.Z.m.Z.m.Z...e.
 00000060: 6403 8301 5a0b 6509 6404 8301 5a0c 6509  d...Z.e.d...Z.e.
 00000070: 6405 8301 5a0d 4700 6406 6407 8400 6407  d...Z.G.d.d...d.
```

## pyppin/math/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 21:44:15 2022 UTC, .py size: 922 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 af11 3663 9a03 0000  o.........6c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 9a03 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 6d03 5a03  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6403 6504 6404 6504 6405 6504 6606  ..d.e.d.e.d.e.f.
 00000050: 6406 6407 8404 5a05 6403 6504 6408 6504  d.d...Z.d.e.d.e.
 00000060: 6409 6504 6405 6504 6608 640a 640b 8404  d.e.d.e.f.d.d...
 00000070: 5a06 6403 6504 6408 6504 6409 6504 6405  Z.d.e.d.e.d.e.d.
```

## pyppin/math/__pycache__/functions.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 00:22:00 2022 UTC, .py size: 2988 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a836 3663 ac0b 0000  o........66c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 ac0b 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6400 0000 6400  .....@...sd...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 4700  m.Z.m.Z.m.Z...G.
 00000060: 6405 6406 8400 6406 6503 8303 5a09 4700  d.d...d.e...Z.G.
 00000070: 6407 6408 8400 6408 6509 8303 5a0a 4700  d.d...d.e...Z.G.
```

## pyppin/math/__pycache__/histogram.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 13300 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 f433 0000  o.......y.vc.3..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 f433 0000  o.......!.vc.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6401  m.Z.m.Z.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 0100 6401 6406 6c0b  d.l.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6401 6407 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
```

## pyppin/math/__pycache__/plot_ascii.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 19340 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 8c4b 0000  o.......y.vc.K..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 8c4b 0000  o.......!.vc.K..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0011 0000 0040 0000 0073 4201 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6401 6404 6c0a 6d0b 5a0b 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6405 6c0c 6d0d 5a0d 0100 6401 6406 6c0e  d.l.m.Z...d.d.l.
```

## pyppin/os/__pycache__/bulk_import.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 15 20:04:43 2022 UTC, .py size: 3621 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5bc8 d162 250e 0000  o.......[..b%...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 250e 0000  o.......!.vc%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6402 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 5a03 6401 6402 6c04 5a04 6401 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6401 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6406 6c0e  m.Z.m.Z...d.d.l.
```

## pyppin/os/__pycache__/list_files.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 21:58:33 2022 UTC, .py size: 2857 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0915 3663 290b 0000  o.........6c)...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 290b 0000  o.......!.vc)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 0905 0902 640f  m.Z.m.Z.......d.
 00000070: 6406 650a 650b 6504 6602 1900 6407 650c  d.e.e.e.f...d.e.
```

## pyppin/testing/__pycache__/interact.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 21:59:17 2022 UTC, .py size: 3633 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3515 3663 310e 0000  o.......5.6c1...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 310e 0000  o.......!.vc1...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 6d05 5a05  Z.d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 0902 0902 6409 6404 6506  m.Z.......d.d.e.
 00000060: 6507 1900 6405 6506 6505 6507 1900 1900  e...d.e.e.e.....
 00000070: 6406 6402 6606 6407 6408 8405 5a08 6402  d.d.f.d.d...Z.d.
```

## pyppin/testing/__pycache__/pprint_object.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 00:22:00 2022 UTC, .py size: 1154 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a836 3663 8204 0000  o........66c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 8204 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 6d05 5a05  d.l.m.Z.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 0904  m.Z.m.Z.m.Z.....
 00000060: 0904 640e 6405 6504 6406 6507 6503 6509  ..d.d.e.d.e.e.e.
 00000070: 1900 1900 6407 6507 6506 6509 1900 1900  ....d.e.e.e.....
```

## pyppin/testing/__pycache__/trace_on_failure.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Sep 28 18:58:32 2022 UTC, .py size: 3246 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5899 3463 ae0c 0000  o.......X.4c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 ae0c 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0010 0000 0040 0000 0073 2c01 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6401  m.Z.m.Z.m.Z...d.
 00000070: 6404 6c0b 6d0c 5a0c 0100 6401 6405 6c0d  d.l.m.Z...d.d.l.
@@ -133,17 +133,17 @@
 00000840: 2e77 7261 7070 6564 2903 da09 6675 6e63  .wrapped)...func
 00000850: 746f 6f6c 73da 0577 7261 7073 7202 0000  tools..wrapsr...
 00000860: 0029 0772 1b00 0000 720a 0000 0072 0b00  .).r....r....r..
 00000870: 0000 720c 0000 0072 0d00 0000 721c 0000  ..r....r....r...
 00000880: 0072 2500 0000 7218 0000 0072 2400 0000  .r%...r....r$...
 00000890: 7219 0000 0072 1700 0000 3100 0000 7306  r....r....1...s.
 000008a0: 0000 0008 0826 0104 0b72 1700 0000 3e04  .....&...r....>.
-000008b0: 0000 005a 0573 6574 5570 5a08 7465 6172  ...Z.setUpZ.tear
-000008c0: 446f 776e 5a0d 7465 6172 446f 776e 436c  DownZ.tearDownCl
-000008d0: 6173 735a 0a73 6574 5570 436c 6173 73da  assZ.setUpClass.
+000008b0: 0000 005a 0874 6561 7244 6f77 6e5a 0a73  ...Z.tearDownZ.s
+000008c0: 6574 5570 436c 6173 735a 0573 6574 5570  etUpClassZ.setUp
+000008d0: 5a0d 7465 6172 446f 776e 436c 6173 73da  Z.tearDownClass.
 000008e0: 0474 6573 7463 0600 0000 0000 0000 0000  .testc..........
 000008f0: 0000 0800 0000 0c00 0000 4300 0000 735a  ..........C...sZ
 00000900: 0000 007c 0572 057c 006a 006e 0164 007d  ...|.r.|.j.n.d.}
 00000910: 0674 01a0 0274 0374 04a0 05a1 00a0 067c  .t...t.t.......|
 00000920: 00a1 01a1 0244 005d 187d 0774 077c 007c  .....D.].}.t.|.|
 00000930: 0783 0272 2a74 087c 007c 0774 0974 0a7c  ...r*t.|.|.t.t.|
 00000940: 007c 0783 027c 067c 017c 027c 037c 0464  .|...|.|.|.|.|.d
```

## pyppin/testing/__pycache__/turn_taker.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 00:22:00 2022 UTC, .py size: 13508 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a836 3663 c434 0000  o........66c.4..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 c434 0000  o.......!.vc.4..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6507 8303  ..G.d.d...d.e...
 00000060: 5a08 4700 6406 6407 8400 6407 6509 8303  Z.G.d.d...d.e...
 00000070: 5a0a 4700 6408 6409 8400 6409 6507 8303  Z.G.d.d...d.e...
```

## pyppin/text/si_prefix.py

```diff
@@ -196,46 +196,52 @@
         return _NEGATIVE_LONG_IEC
     elif ascii_only:
         return _NEGATIVE_IEC_ASCII
     else:
         return _NEGATIVE_IEC_UNICODE
 
 
-_POSITIVE_SI = "kMGTPEZY"
-_NEGATIVE_SI_ASCII = "munpfazy"
-_NEGATIVE_SI_UNICODE = "mμnpfazy"
+_POSITIVE_SI = "kMGTPEZYRQ"
+_NEGATIVE_SI_ASCII = "munpfazyrq"
+_NEGATIVE_SI_UNICODE = "mμnpfazyrq"
 # Note the spaces before long forms!
 _POSITIVE_LONG_SI = [
     " kilo",
     " mega",
     " giga",
     " tera",
     " peta",
     " exa",
     " zetta",
     " yotta",
+    " ronna",
+    " quetta",
 ]
 _NEGATIVE_LONG_SI = [
     " milli",
     " micro",
     " nano",
     " pico",
     " femto",
     " atto",
     " zepto",
     " yocto",
+    " ronto",
+    " quecto",
 ]
 
-_POSITIVE_IEC = ["Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi", "Yi"]
+_POSITIVE_IEC = ["Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi", "Yi", "Ri", "Qi"]
 _NEGATIVE_IEC_ASCII = [x + "i" for x in _NEGATIVE_SI_ASCII]
 _NEGATIVE_IEC_UNICODE = [x + "i" for x in _NEGATIVE_SI_UNICODE]
 _POSITIVE_LONG_IEC = [
     " kibi",
     " mebi",
     " gibi",
     " tebi",
     " pebi",
     " exbi",
     " zebi",
     " yobi",
+    " ronni",
+    " quetti",
 ]
 _NEGATIVE_LONG_IEC: List[str] = []  # See comment on the full_names arg to si_prefix
```

## pyppin/text/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Sep 28 20:01:57 2022 UTC, .py size: 38 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 35a8 3463 2600 0000  o.......5.4c&...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 2600 0000  o.......!.vc&...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5300 2902 7a1f 5468 696e 6773  Z.d.S.).z.Things
 00000040: 2074 6f20 666f 726d 6174 2074 6578 7420   to format text 
 00000050: 7072 6574 7469 6c79 2e4e 2901 da07 5f5f  prettily.N)...__
 00000060: 646f 635f 5fa9 0072 0200 0000 7202 0000  doc__..r....r...
 00000070: 00fa 3a62 7569 6c64 2f62 6469 7374 2e6d  ..:build/bdist.m
```

## pyppin/text/__pycache__/formatter.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 21:49:12 2022 UTC, .py size: 8703 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5864 3763 ff21 0000  o.......Xd7c.!..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 ff21 0000  o.......!.vc.!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 2801 0000 6400  .....@...s(...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6401 6406 6c0b  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 6d0d 5a0d 0100 6401 6407 6c0e  m.Z.m.Z...d.d.l.
```

## pyppin/text/__pycache__/now_and_then.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 00:22:00 2022 UTC, .py size: 4929 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a836 3663 4113 0000  o........66cA...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 4113 0000  o.......!.vcA...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 0001 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 6d02 5a02  Z.d.d.l.m.Z.m.Z.
 00000040: 0100 6401 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6401 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 0100 0906 0907 6420 6408 6505 6501 1900  ......d d.e.e...
```

## pyppin/text/__pycache__/print_counter.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 21:49:12 2022 UTC, .py size: 5785 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5864 3763 9916 0000  o.......Xd7c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 9916 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d05 5a05 6d06 5a06 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6401 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

## pyppin/text/__pycache__/si_prefix.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 21:49:12 2022 UTC, .py size: 8999 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5864 3763 2723 0000  o.......Xd7c'#..
+00000000: 6f0d 0d0a 0000 0000 0eb8 4e64 9023 0000  o.........Nd.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0011 0000 0040 0000 0073 2a01 0000 5500  .....@...s*...U.
 00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6403  d.Z.d.d.l.Z.d.d.
 00000040: 6c02 6d03 5a03 0100 6401 6404 6c04 6d05  l.m.Z...d.d.l.m.
 00000050: 5a05 6d06 5a06 6d07 5a07 0100 6401 6405  Z.m.Z.m.Z...d.d.
 00000060: 6c08 6d09 5a09 6d0a 5a0a 0100 4700 6406  l.m.Z.m.Z...G.d.
 00000070: 6407 8400 6407 6503 8303 5a0b 650b 6a0c  d...d.e...Z.e.j.
@@ -407,57 +407,61 @@
 00001960: 4741 5449 5645 5f49 4543 5f41 5343 4949  GATIVE_IEC_ASCII
 00001970: da15 5f4e 4547 4154 4956 455f 4945 435f  .._NEGATIVE_IEC_
 00001980: 554e 4943 4f44 4529 0472 1400 0000 7234  UNICODE).r....r4
 00001990: 0000 0072 1700 0000 7218 0000 0072 1100  ...r....r....r..
 000019a0: 0000 7211 0000 0072 1200 0000 7226 0000  ..r....r....r&..
 000019b0: 00b3 0000 0073 1e00 0000 1004 0401 0c01  .....s..........
 000019c0: 0401 0401 0401 0401 0402 0402 0c01 0401  ................
-000019d0: 0401 0401 0401 0402 7226 0000 005a 086b  ........r&...Z.k
-000019e0: 4d47 5450 455a 595a 086d 756e 7066 617a  MGTPEZYZ.munpfaz
-000019f0: 7975 0900 0000 6dce bc6e 7066 617a 7929  yu....m..npfazy)
-00001a00: 087a 0520 6b69 6c6f 7a05 206d 6567 617a  .z. kiloz. megaz
-00001a10: 0520 6769 6761 7a05 2074 6572 617a 0520  . gigaz. teraz. 
-00001a20: 7065 7461 7a04 2065 7861 7a06 207a 6574  petaz. exaz. zet
-00001a30: 7461 7a06 2079 6f74 7461 2908 7a06 206d  taz. yotta).z. m
-00001a40: 696c 6c69 7a06 206d 6963 726f 7a05 206e  illiz. microz. n
-00001a50: 616e 6f7a 0520 7069 636f 7a06 2066 656d  anoz. picoz. fem
-00001a60: 746f 7a05 2061 7474 6f7a 0620 7a65 7074  toz. attoz. zept
-00001a70: 6f7a 0620 796f 6374 6f29 085a 024b 695a  oz. yocto).Z.KiZ
-00001a80: 024d 695a 0247 695a 0254 69da 0250 695a  .MiZ.GiZ.Ti..PiZ
-00001a90: 0245 695a 025a 695a 0259 6963 0100 0000  .EiZ.ZiZ.Yic....
-00001aa0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001ab0: 4300 0000 f314 0000 0067 007c 005d 067d  C........g.|.].}
-00001ac0: 017c 0164 0017 0091 0271 0253 00a9 01da  .|.d.....q.S....
-00001ad0: 0169 7211 0000 00a9 02da 022e 30da 0178  .ir.........0..x
-00001ae0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00001af0: 0a3c 6c69 7374 636f 6d70 3ee5 0000 00f3  .<listcomp>.....
-00001b00: 0200 0000 1400 7246 0000 0063 0100 0000  ......rF...c....
-00001b10: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001b20: 4300 0000 7240 0000 0072 4100 0000 7211  C...r@...rA...r.
-00001b30: 0000 0072 4300 0000 7211 0000 0072 1100  ...rC...r....r..
-00001b40: 0000 7212 0000 0072 4600 0000 e600 0000  ..r....rF.......
-00001b50: 7247 0000 0029 087a 0520 6b69 6269 7a05  rG...).z. kibiz.
-00001b60: 206d 6562 697a 0520 6769 6269 7a05 2074   mebiz. gibiz. t
-00001b70: 6562 697a 0520 7065 6269 7a05 2065 7862  ebiz. pebiz. exb
-00001b80: 697a 0520 7a65 6269 7a05 2079 6f62 6972  iz. zebiz. yobir
-00001b90: 3c00 0000 2920 720e 0000 0072 1e00 0000  <...) r....r....
-00001ba0: da04 656e 756d 7202 0000 00da 0674 7970  ..enumr......typ
-00001bb0: 696e 6772 0300 0000 7204 0000 0072 0500  ingr....r....r..
-00001bc0: 0000 5a10 7079 7070 696e 2e74 6578 742e  ..Z.pyppin.text.
-00001bd0: 7369 676e 7206 0000 0072 0700 0000 7208  signr....r....r.
-00001be0: 0000 0072 0f00 0000 5a0d 4e45 4741 5449  ...r....Z.NEGATI
-00001bf0: 5645 5f4f 4e4c 59da 0566 6c6f 6174 7225  VE_ONLY..floatr%
-00001c00: 0000 00da 0462 6f6f 6c72 2000 0000 7231  .....boolr ...r1
-00001c10: 0000 0072 2800 0000 7226 0000 0072 3600  ...r(...r&...r6.
-00001c20: 0000 7238 0000 0072 3900 0000 7235 0000  ..r8...r9...r5..
-00001c30: 0072 3700 0000 723b 0000 0072 3d00 0000  .r7...r;...r=...
-00001c40: 723e 0000 0072 3a00 0000 723c 0000 00da  r>...r:...r<....
-00001c50: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
-00001c60: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00001c70: 1200 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-00001c80: 0000 7368 0000 0006 0008 020c 0114 0110  ..sh............
-00001c90: 0210 0304 0f02 0102 0102 0102 0104 0104  ................
-00001ca0: f90a 0102 ff02 0202 fe02 0302 fd02 0402  ................
-00001cb0: fc02 0502 fb02 0602 fa02 0702 f902 080a  ................
-00001cc0: f800 7f1a 1102 0c02 0102 ff02 0102 ff02  ................
-00001cd0: 0102 ff02 0102 ff06 020a fe04 1804 0104  ................
-00001ce0: 0108 0208 0a08 0b0e 010e 0108 0114 0a    ...............
+000019d0: 0401 0401 0401 0402 7226 0000 005a 0a6b  ........r&...Z.k
+000019e0: 4d47 5450 455a 5952 515a 0a6d 756e 7066  MGTPEZYRQZ.munpf
+000019f0: 617a 7972 7175 0b00 0000 6dce bc6e 7066  azyrqu....m..npf
+00001a00: 617a 7972 7129 0a7a 0520 6b69 6c6f 7a05  azyrq).z. kiloz.
+00001a10: 206d 6567 617a 0520 6769 6761 7a05 2074   megaz. gigaz. t
+00001a20: 6572 617a 0520 7065 7461 7a04 2065 7861  eraz. petaz. exa
+00001a30: 7a06 207a 6574 7461 7a06 2079 6f74 7461  z. zettaz. yotta
+00001a40: 7a06 2072 6f6e 6e61 7a07 2071 7565 7474  z. ronnaz. quett
+00001a50: 6129 0a7a 0620 6d69 6c6c 697a 0620 6d69  a).z. milliz. mi
+00001a60: 6372 6f7a 0520 6e61 6e6f 7a05 2070 6963  croz. nanoz. pic
+00001a70: 6f7a 0620 6665 6d74 6f7a 0520 6174 746f  oz. femtoz. atto
+00001a80: 7a06 207a 6570 746f 7a06 2079 6f63 746f  z. zeptoz. yocto
+00001a90: 7a06 2072 6f6e 746f 7a07 2071 7565 6374  z. rontoz. quect
+00001aa0: 6f29 0a5a 024b 695a 024d 695a 0247 695a  o).Z.KiZ.MiZ.GiZ
+00001ab0: 0254 69da 0250 695a 0245 695a 025a 695a  .Ti..PiZ.EiZ.ZiZ
+00001ac0: 0259 695a 0252 695a 0251 6963 0100 0000  .YiZ.RiZ.Qic....
+00001ad0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001ae0: 4300 0000 f314 0000 0067 007c 005d 067d  C........g.|.].}
+00001af0: 017c 0164 0017 0091 0271 0253 00a9 01da  .|.d.....q.S....
+00001b00: 0169 7211 0000 00a9 02da 022e 30da 0178  .ir.........0..x
+00001b10: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00001b20: 0a3c 6c69 7374 636f 6d70 3ee9 0000 00f3  .<listcomp>.....
+00001b30: 0200 0000 1400 7246 0000 0063 0100 0000  ......rF...c....
+00001b40: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001b50: 4300 0000 7240 0000 0072 4100 0000 7211  C...r@...rA...r.
+00001b60: 0000 0072 4300 0000 7211 0000 0072 1100  ...rC...r....r..
+00001b70: 0000 7212 0000 0072 4600 0000 ea00 0000  ..r....rF.......
+00001b80: 7247 0000 0029 0a7a 0520 6b69 6269 7a05  rG...).z. kibiz.
+00001b90: 206d 6562 697a 0520 6769 6269 7a05 2074   mebiz. gibiz. t
+00001ba0: 6562 697a 0520 7065 6269 7a05 2065 7862  ebiz. pebiz. exb
+00001bb0: 697a 0520 7a65 6269 7a05 2079 6f62 697a  iz. zebiz. yobiz
+00001bc0: 0620 726f 6e6e 697a 0720 7175 6574 7469  . ronniz. quetti
+00001bd0: 723c 0000 0029 2072 0e00 0000 721e 0000  r<...) r....r...
+00001be0: 00da 0465 6e75 6d72 0200 0000 da06 7479  ...enumr......ty
+00001bf0: 7069 6e67 7203 0000 0072 0400 0000 7205  pingr....r....r.
+00001c00: 0000 005a 1070 7970 7069 6e2e 7465 7874  ...Z.pyppin.text
+00001c10: 2e73 6967 6e72 0600 0000 7207 0000 0072  .signr....r....r
+00001c20: 0800 0000 720f 0000 005a 0d4e 4547 4154  ....r....Z.NEGAT
+00001c30: 4956 455f 4f4e 4c59 da05 666c 6f61 7472  IVE_ONLY..floatr
+00001c40: 2500 0000 da04 626f 6f6c 7220 0000 0072  %.....boolr ...r
+00001c50: 3100 0000 7228 0000 0072 2600 0000 7236  1...r(...r&...r6
+00001c60: 0000 0072 3800 0000 7239 0000 0072 3500  ...r8...r9...r5.
+00001c70: 0000 7237 0000 0072 3b00 0000 723d 0000  ..r7...r;...r=..
+00001c80: 0072 3e00 0000 723a 0000 0072 3c00 0000  .r>...r:...r<...
+00001c90: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+00001ca0: 5f72 1100 0000 7211 0000 0072 1100 0000  _r....r....r....
+00001cb0: 7212 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001cc0: 0000 0073 6800 0000 0600 0802 0c01 1401  ...sh...........
+00001cd0: 1002 1003 040f 0201 0201 0201 0201 0401  ................
+00001ce0: 04f9 0a01 02ff 0202 02fe 0203 02fd 0204  ................
+00001cf0: 02fc 0205 02fb 0206 02fa 0207 02f9 0208  ................
+00001d00: 0af8 007f 1a11 020c 0201 02ff 0201 02ff  ................
+00001d10: 0201 02ff 0201 02ff 0602 0afe 0418 0401  ................
+00001d20: 0401 0802 080c 080d 0e01 0e01 0801 140c  ................
```

## pyppin/text/__pycache__/sign.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 22:12:15 2022 UTC, .py size: 1852 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3f18 3663 3c07 0000  o.......?.6c<...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 3c07 0000  o.......!.vc<...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000050: 8400 6405 6502 8303 5a05 6406 6506 6407  ..d.e...Z.d.e.d.
 00000060: 6505 6408 6507 6409 6506 6608 640a 640b  e.d.e.d.e.f.d.d.
 00000070: 8404 5a08 6505 6a09 6505 6a0a 6505 6a0b  ..Z.e.j.e.j.e.j.
```

## pyppin/threading/__pycache__/semaphore.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jul 23 00:15:23 2022 UTC, .py size: 15617 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9b3d db62 013d 0000  o........=.b.=..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 013d 0000  o.......!.vc.=..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6401 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6401 6407 6c0c 6d0d 5a0d 6d0e 5a0e  ..d.d.l.m.Z.m.Z.
```

## pyppin/threading/__pycache__/stack_trace.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 20:56:37 2022 UTC, .py size: 3214 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0558 3763 8e0c 0000  o........X7c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 8e0c 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000b 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d04 5a04 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6401  d.l.m.Z.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 6d0a 5a0a 0100 0902  d.l.m.Z.m.Z.....
 00000070: 0902 0906 0906 6410 6407 6506 6501 6a0b  ......d.d.e.e.j.
```

## pyppin/threading/__pycache__/stack_trace_internals.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 17491 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 5344 0000  o.......y.vcSD..
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 5344 0000  o.......!.vcSD..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 a202 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000060: 0100 6401 6404 6c08 6d09 5a09 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6401 6406 6c0c  d.l.m.Z...d.d.l.
```

## pyppin/util/expression.py

```diff
@@ -1,7 +1,9 @@
+"""Safe evaluation of Python expressions."""
+
 import ast
 import builtins
 import sys
 from typing import (
     Any,
     Callable,
     Dict,
@@ -13,50 +15,51 @@
     Tuple,
     Type,
     Union,
 )
 
 
 class Expression(object):
+    """Expression implements "safe" evaluation of user-entered Python expressions.
+
+    This is safe in that it tries to ensure that the given expression cannot mutate the state of
+    the system (e.g. modifying attributes), execute I/O, or change the broader control flow.
+    However, it is not perfectly safe: Sufficiently complex expressions can crash the entire
+    interpreter! See compile() for details. Length-limiting the input may help.
+
+    Args:
+        expression: A Python expression to be turned into this object.
+        functions: A list of functions which may be used in expressions. By default, only the
+            "safe" builtin functions (see SAFE_BUILTINS, below) are permitted; any others
+            must be explicitly specified.
+        allow_attribute_functions: By default, while all attributes of variables passed in to
+            the expression may be referenced, if the variable contains a function (e.g.,
+            x.foo()) then that function may *not* be called. If this is set to true, such
+            functions are permitted. This default makes it safe to pass objects which have
+            potentially dangerous methods for their data alone. Note that variable *properties*
+            are always accessible.
+        variables: If given, a list of variable names which may be referenced by the expression.
+            In this case, any reference to variables not in this list will raise a SyntaxError
+            at construction time. If not given, all variable names are permitted, and the actual
+            set of variables used can be checked with the ``variables`` property of this object.
+
+    Raises:
+        SyntaxError: If the expression cannot be parsed, or if the expression attempted to
+            do something forbidden, like reference an unknown variable.
+        ValueError: If the expression string contains NUL bytes for some reason.
+    """
+
     def __init__(
         self,
         expression: str,
         *,
         functions: List[Callable] = [],
         allow_attribute_functions: bool = False,
         variables: Optional[List[str]] = None,
     ) -> None:
-        """Expression implements "safe" evaluation of user-entered Python expressions.
-
-        This is safe in that it tries to ensure that the given expression cannot mutate the state of
-        the system (e.g. modifying attributes), execute I/O, or change the broader control flow.
-        However, it is not perfectly safe: Sufficiently complex expressions can crash the entire
-        interpreter! See compile() for details. Length-limiting the input may help.
-
-        Args:
-            expression: A Python expression to be turned into this object.
-            functions: A list of functions which may be used in expressions. By default, only the
-                "safe" builtin functions (see SAFE_BUILTINS, below) are permitted; any others
-                must be explicitly specified.
-            allow_attribute_functions: By default, while all attributes of variables passed in to
-                the expression may be referenced, if the variable contains a function (e.g.,
-                x.foo()) then that function may *not* be called. If this is set to true, such
-                functions are permitted. This default makes it safe to pass objects which have
-                potentially dangerous methods for their data alone. Note that variable *properties*
-                are always accessible.
-            variables: If given, a list of variable names which may be referenced by the expression.
-                In this case, any reference to variables not in this list will raise a SyntaxError
-                at construction time. If not given, all variable names are permitted, and the actual
-                set of variables used can be checked with the ``variables`` property of this object.
-
-        Raises:
-            SyntaxError: If the expression cannot be parsed, or if the expression attempted to
-                do something forbidden, like reference an unknown variable.
-            ValueError: If the expression string contains NUL bytes for some reason.
-        """
         self._fns: Dict[str, Callable] = _dict_sum(
             SAFE_BUILTINS, {fn.__name__: fn for fn in functions}
         )
 
         self._ast = ast.parse(expression, mode="eval")
         context = _ValidationContext(
             expression,
```

## pyppin/util/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 31 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 1f00 0000  o.......y.vc....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 1f00 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0800 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5300 2902 7a18 4d69 7363 656c  Z.d.S.).z.Miscel
 00000040: 6c61 6e65 6f75 7320 7574 696c 6974 6965  laneous utilitie
 00000050: 732e 4e29 01da 075f 5f64 6f63 5f5f a900  s.N)...__doc__..
 00000060: 7202 0000 0072 0200 0000 fa3a 6275 696c  r....r.....:buil
 00000070: 642f 6264 6973 742e 6d61 636f 7378 2d31  d/bdist.macosx-1
```

## pyppin/util/__pycache__/expression.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 18687 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,969 +1,967 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 ff48 0000  o.......y.vc.H..
+00000000: 6f0d 0d0a 0000 0000 d901 7763 ca48 0000  o.........wc.H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 8605 0000 5500  .....@...s....U.
-00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
-00000040: 6400 6401 6c02 5a02 6400 6402 6c03 6d04  d.d.l.Z.d.d.l.m.
-00000050: 5a04 6d05 5a05 6d06 5a06 6d07 5a07 6d08  Z.m.Z.m.Z.m.Z.m.
+00000020: 0006 0000 0040 0000 0073 8a05 0000 5500  .....@...s....U.
+00000030: 6400 5a00 6401 6402 6c01 5a01 6401 6402  d.Z.d.d.l.Z.d.d.
+00000040: 6c02 5a02 6401 6402 6c03 5a03 6401 6403  l.Z.d.d.l.Z.d.d.
+00000050: 6c04 6d05 5a05 6d06 5a06 6d07 5a07 6d08  l.m.Z.m.Z.m.Z.m.
 00000060: 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c  Z.m.Z.m.Z.m.Z.m.
-00000070: 5a0c 6d0d 5a0d 6d0e 5a0e 0100 4700 6403  Z.m.Z.m.Z...G.d.
-00000080: 6404 8400 6404 650f 8303 5a10 6405 6511  d...d.e...Z.d.e.
-00000090: 6406 6511 6604 6407 6408 8404 5a12 6409  d.e.f.d.d...Z.d.
-000000a0: 640a 8400 640b 4400 8301 5a13 6506 6514  d...d.D...Z.e.e.
-000000b0: 6505 6602 1900 6515 640c 3c00 4700 640d  e.f...e.d.<.G.d.
-000000c0: 640e 8400 640e 6508 8303 5a16 640f 6500  d...d.e...Z.d.e.
-000000d0: 6a17 6410 6516 6406 6518 6606 6411 6412  j.d.e.d.e.f.d.d.
-000000e0: 8404 5a19 640f 6500 6a17 6410 6516 6406  ..Z.d.e.j.d.e.d.
-000000f0: 6518 6606 6413 6414 8404 5a1a 640f 6500  e.f.d.d...Z.d.e.
-00000100: 6a17 6410 6516 6406 6518 6606 6415 6416  j.d.e.d.e.f.d.d.
-00000110: 8404 5a1b 640f 6500 6a17 6410 6516 6406  ..Z.d.e.j.d.e.d.
-00000120: 6518 6606 6417 6418 8404 5a1c 650e 6401  e.f.d.d...Z.e.d.
-00000130: 6514 6505 6500 6a17 6516 6702 6518 6602  e.e.e.j.e.g.e.f.
-00000140: 1900 6603 1900 5a1d 6900 5a1e 6506 650d  ..f...Z.i.Z.e.e.
-00000150: 6500 6a17 1900 651d 6602 1900 6515 6419  e.j...e.f...e.d.
-00000160: 3c00 641a 6514 641b 651d 6406 6401 6606  <.d.e.d.e.d.d.f.
-00000170: 641c 641d 8404 5a1f 641e 5a20 641f 5a21  d.d...Z.d.Z d.Z!
-00000180: 6420 5a22 6421 5a23 6422 5a24 651f 6404  d Z"d!Z#d"Z$e.d.
-00000190: 6401 8302 0100 651f 6423 6401 8302 0100  d.....e.d#d.....
-000001a0: 651f 6424 6401 8302 0100 651f 6425 6524  e.d$d.....e.d%e$
-000001b0: 8302 0100 651f 6426 6401 8302 0100 651f  ....e.d&d.....e.
-000001c0: 6427 6401 8302 0100 651f 6428 6401 8302  d'd.....e.d(d...
-000001d0: 0100 651f 6429 6401 8302 0100 651f 642a  ..e.d)d.....e.d*
-000001e0: 6401 8302 0100 651f 642b 6401 8302 0100  d.....e.d+d.....
-000001f0: 651f 642c 6401 8302 0100 651f 642d 6519  e.d,d.....e.d-e.
-00000200: 8302 0100 651f 642e 6401 8302 0100 651f  ....e.d.d.....e.
-00000210: 642f 6520 8302 0100 651f 6430 6521 8302  d/e ....e.d0e!..
-00000220: 0100 651f 6431 6401 8302 0100 651f 6432  ..e.d1d.....e.d2
-00000230: 6401 8302 0100 651f 6433 6401 8302 0100  d.....e.d3d.....
-00000240: 651f 6434 6401 8302 0100 651f 6435 6401  e.d4d.....e.d5d.
-00000250: 8302 0100 651f 6436 6401 8302 0100 651f  ....e.d6d.....e.
-00000260: 6437 6401 8302 0100 651f 6438 6401 8302  d7d.....e.d8d...
-00000270: 0100 651f 6439 6401 8302 0100 651f 643a  ..e.d9d.....e.d:
-00000280: 6401 8302 0100 651f 643b 6401 8302 0100  d.....e.d;d.....
-00000290: 651f 643c 6401 8302 0100 651f 643d 6401  e.d<d.....e.d=d.
-000002a0: 8302 0100 651f 643e 6401 8302 0100 651f  ....e.d>d.....e.
-000002b0: 643f 6401 8302 0100 651f 6440 6401 8302  d?d.....e.d@d...
-000002c0: 0100 651f 6441 6401 8302 0100 651f 6442  ..e.dAd.....e.dB
-000002d0: 6401 8302 0100 651f 6443 6401 8302 0100  d.....e.dCd.....
-000002e0: 651f 6444 6401 8302 0100 651f 6445 6401  e.dDd.....e.dEd.
-000002f0: 8302 0100 651f 6446 6401 8302 0100 651f  ....e.dFd.....e.
-00000300: 6447 6401 8302 0100 651f 6448 6401 8302  dGd.....e.dHd...
-00000310: 0100 651f 6449 6401 8302 0100 651f 644a  ..e.dId.....e.dJ
-00000320: 6401 8302 0100 651f 644b 6401 8302 0100  d.....e.dKd.....
-00000330: 651f 644c 6401 8302 0100 651f 644d 6401  e.dLd.....e.dMd.
-00000340: 8302 0100 651f 644e 6401 8302 0100 651f  ....e.dNd.....e.
-00000350: 644f 6401 8302 0100 651f 6450 6401 8302  dOd.....e.dPd...
-00000360: 0100 651f 6451 6401 8302 0100 651f 6452  ..e.dQd.....e.dR
-00000370: 6401 8302 0100 651f 6453 6401 8302 0100  d.....e.dSd.....
-00000380: 651f 6454 651a 8302 0100 651f 6455 6401  e.dTe.....e.dUd.
-00000390: 8302 0100 651f 6456 6401 8302 0100 651f  ....e.dVd.....e.
-000003a0: 6457 6401 8302 0100 651f 6458 6520 8302  dWd.....e.dXe ..
-000003b0: 0100 651f 6459 6401 8302 0100 651f 645a  ..e.dYd.....e.dZ
-000003c0: 6401 8302 0100 651f 645b 651b 8302 0100  d.....e.d[e.....
-000003d0: 651f 645c 651b 8302 0100 651f 645d 651b  e.d\e.....e.d]e.
-000003e0: 8302 0100 651f 645e 651b 8302 0100 651f  ....e.d^e.....e.
-000003f0: 645f 6401 8302 0100 651f 6460 6520 8302  d_d.....e.d`e ..
-00000400: 0100 651f 6461 6520 8302 0100 651f 6462  ..e.dae ....e.db
-00000410: 6520 8302 0100 651f 6463 6524 8302 0100  e ....e.dce$....
-00000420: 651f 6464 6524 8302 0100 651f 6465 6521  e.dde$....e.dee!
-00000430: 8302 0100 651f 6466 6401 8302 0100 651f  ....e.dfd.....e.
-00000440: 6467 6523 8302 0100 651f 6468 6523 8302  dge#....e.dhe#..
-00000450: 0100 651f 6469 6401 8302 0100 651f 646a  ..e.did.....e.dj
-00000460: 6401 8302 0100 651f 646b 6401 8302 0100  d.....e.dkd.....
-00000470: 651f 646c 6401 8302 0100 651f 646d 6401  e.dld.....e.dmd.
-00000480: 8302 0100 651f 646e 6401 8302 0100 651f  ....e.dnd.....e.
-00000490: 646f 6401 8302 0100 651f 6470 6401 8302  dod.....e.dpd...
-000004a0: 0100 651f 6471 6401 8302 0100 651f 6472  ..e.dqd.....e.dr
-000004b0: 6401 8302 0100 651f 6473 6401 8302 0100  d.....e.dsd.....
-000004c0: 651f 6474 6401 8302 0100 651f 6475 6401  e.dtd.....e.dud.
-000004d0: 8302 0100 651f 6476 6401 8302 0100 651f  ....e.dvd.....e.
-000004e0: 6477 6401 8302 0100 651f 6478 6401 8302  dwd.....e.dxd...
-000004f0: 0100 651f 6479 6401 8302 0100 651f 647a  ..e.dyd.....e.dz
-00000500: 6401 8302 0100 651f 647b 6401 8302 0100  d.....e.d{d.....
-00000510: 651f 647c 6401 8302 0100 651f 647d 6401  e.d|d.....e.d}d.
-00000520: 8302 0100 651f 647e 6522 8302 0100 651f  ....e.d~e"....e.
-00000530: 647f 6401 8302 0100 651f 6480 6401 8302  d.d.....e.d.d...
-00000540: 0100 651f 6481 6401 8302 0100 651f 6482  ..e.d.d.....e.d.
-00000550: 6524 8302 0100 651f 6483 6524 8302 0100  e$....e.d.e$....
-00000560: 651f 6484 6524 8302 0100 651f 6485 6486  e.d.e$....e.d.d.
-00000570: 8302 0100 651f 6487 6488 8302 0100 651f  ....e.d.d.....e.
-00000580: 6489 6522 8302 0100 651f 648a 6522 8302  d.e"....e.d.e"..
-00000590: 0100 651f 648b 6401 8302 0100 651f 648c  ..e.d.d.....e.d.
-000005a0: 6401 8302 0100 651f 648d 6401 8302 0100  d.....e.d.d.....
-000005b0: 6401 5300 298e e900 0000 004e 290b da03  d.S.)......N)...
-000005c0: 416e 79da 0843 616c 6c61 626c 65da 0444  Any..Callable..D
-000005d0: 6963 74da 044c 6973 74da 0a4e 616d 6564  ict..List..Named
-000005e0: 5475 706c 65da 084e 6f52 6574 7572 6eda  Tuple..NoReturn.
-000005f0: 084f 7074 696f 6e61 6cda 0353 6574 da05  .Optional..Set..
-00000600: 5475 706c 65da 0454 7970 65da 0555 6e69  Tuple..Type..Uni
-00000610: 6f6e 6300 0000 0000 0000 0000 0000 0000  onc.............
-00000620: 0000 000b 0000 0040 0000 0073 d000 0000  .......@...s....
-00000630: 6500 5a01 6400 5a02 6700 6401 6402 6403  e.Z.d.Z.g.d.d.d.
-00000640: 9c03 6404 6503 6405 6504 6505 1900 6406  ..d.e.d.e.e...d.
-00000650: 6506 6407 6507 6504 6503 1900 1900 6408  e.d.e.e.e.....d.
-00000660: 6402 660a 6409 640a 8406 5a08 640b 6509  d.f.d.d...Z.d.e.
-00000670: 6408 6509 6604 640c 640d 8404 5a0a 650b  d.e.f.d.d...Z.e.
-00000680: 6408 650c 6503 640e 6602 1900 6602 640f  d.e.e.d.f...f.d.
-00000690: 6410 8404 8301 5a0d 650b 6408 650c 6503  d.....Z.e.d.e.e.
-000006a0: 640e 6602 1900 6602 6411 6412 8404 8301  d.f...f.d.d.....
-000006b0: 5a0e 650b 6408 650f 6a10 6602 6413 6414  Z.e.d.e.j.f.d.d.
-000006c0: 8404 8301 5a0f 6408 6511 6503 6505 6602  ....Z.d.e.e.e.f.
-000006d0: 1900 6602 6415 6416 8404 5a12 6408 6503  ..f.d.d...Z.d.e.
-000006e0: 6602 6417 6418 8404 5a13 6419 6503 6408  f.d.d...Z.d.e.d.
-000006f0: 6506 6604 641a 641b 8404 5a14 6402 5300  e.f.d.d...Z.d.S.
-00000700: 291c da0a 4578 7072 6573 7369 6f6e 464e  )...ExpressionFN
-00000710: 2903 da09 6675 6e63 7469 6f6e 73da 1961  )...functions..a
-00000720: 6c6c 6f77 5f61 7474 7269 6275 7465 5f66  llow_attribute_f
-00000730: 756e 6374 696f 6e73 da09 7661 7269 6162  unctions..variab
-00000740: 6c65 73da 0a65 7870 7265 7373 696f 6e72  les..expressionr
-00000750: 0e00 0000 720f 0000 0072 1000 0000 da06  ....r....r......
-00000760: 7265 7475 726e 6302 0000 0000 0000 0003  returnc.........
-00000770: 0000 0006 0000 0005 0000 0043 0000 0073  ...........C...s
-00000780: 7800 0000 7400 7401 6401 6402 8400 7c02  x...t.t.d.d...|.
-00000790: 4400 8301 8302 7c00 5f02 7403 6a04 7c01  D.....|._.t.j.|.
-000007a0: 6403 6404 8d02 7c00 5f05 7406 7c01 7c04  d.d...|._.t.|.|.
-000007b0: 6405 7501 721d 7407 7c04 8301 6e01 6405  d.u.r.t.|...n.d.
-000007c0: 7c00 6a02 7c03 8304 7d05 7c05 a008 7c00  |.j.|...}.|...|.
-000007d0: 6a05 a101 0100 7409 7c00 6a05 6406 6403  j.....t.|.j.d.d.
-000007e0: 6407 8d03 7c00 5f0a 7c00 6a0a 6a0b 6408  d...|._.|.j.j.d.
-000007f0: 6b02 733a 4a00 8201 6405 5300 2909 61c2  k.s:J...d.S.).a.
-00000800: 0700 0045 7870 7265 7373 696f 6e20 696d  ...Expression im
-00000810: 706c 656d 656e 7473 2022 7361 6665 2220  plements "safe" 
-00000820: 6576 616c 7561 7469 6f6e 206f 6620 7573  evaluation of us
-00000830: 6572 2d65 6e74 6572 6564 2050 7974 686f  er-entered Pytho
-00000840: 6e20 6578 7072 6573 7369 6f6e 732e 0a0a  n expressions...
-00000850: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
-00000860: 7361 6665 2069 6e20 7468 6174 2069 7420  safe in that it 
-00000870: 7472 6965 7320 746f 2065 6e73 7572 6520  tries to ensure 
-00000880: 7468 6174 2074 6865 2067 6976 656e 2065  that the given e
-00000890: 7870 7265 7373 696f 6e20 6361 6e6e 6f74  xpression cannot
-000008a0: 206d 7574 6174 6520 7468 6520 7374 6174   mutate the stat
-000008b0: 6520 6f66 0a20 2020 2020 2020 2074 6865  e of.        the
-000008c0: 2073 7973 7465 6d20 2865 2e67 2e20 6d6f   system (e.g. mo
-000008d0: 6469 6679 696e 6720 6174 7472 6962 7574  difying attribut
-000008e0: 6573 292c 2065 7865 6375 7465 2049 2f4f  es), execute I/O
-000008f0: 2c20 6f72 2063 6861 6e67 6520 7468 6520  , or change the 
-00000900: 6272 6f61 6465 7220 636f 6e74 726f 6c20  broader control 
-00000910: 666c 6f77 2e0a 2020 2020 2020 2020 486f  flow..        Ho
-00000920: 7765 7665 722c 2069 7420 6973 206e 6f74  wever, it is not
-00000930: 2070 6572 6665 6374 6c79 2073 6166 653a   perfectly safe:
-00000940: 2053 7566 6669 6369 656e 746c 7920 636f   Sufficiently co
-00000950: 6d70 6c65 7820 6578 7072 6573 7369 6f6e  mplex expression
-00000960: 7320 6361 6e20 6372 6173 6820 7468 6520  s can crash the 
-00000970: 656e 7469 7265 0a20 2020 2020 2020 2069  entire.        i
-00000980: 6e74 6572 7072 6574 6572 2120 5365 6520  nterpreter! See 
-00000990: 636f 6d70 696c 6528 2920 666f 7220 6465  compile() for de
-000009a0: 7461 696c 732e 204c 656e 6774 682d 6c69  tails. Length-li
-000009b0: 6d69 7469 6e67 2074 6865 2069 6e70 7574  miting the input
-000009c0: 206d 6179 2068 656c 702e 0a0a 2020 2020   may help...    
-000009d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000009e0: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
-000009f0: 3a20 4120 5079 7468 6f6e 2065 7870 7265  : A Python expre
-00000a00: 7373 696f 6e20 746f 2062 6520 7475 726e  ssion to be turn
-00000a10: 6564 2069 6e74 6f20 7468 6973 206f 626a  ed into this obj
-00000a20: 6563 742e 0a20 2020 2020 2020 2020 2020  ect..           
-00000a30: 2066 756e 6374 696f 6e73 3a20 4120 6c69   functions: A li
-00000a40: 7374 206f 6620 6675 6e63 7469 6f6e 7320  st of functions 
-00000a50: 7768 6963 6820 6d61 7920 6265 2075 7365  which may be use
-00000a60: 6420 696e 2065 7870 7265 7373 696f 6e73  d in expressions
-00000a70: 2e20 4279 2064 6566 6175 6c74 2c20 6f6e  . By default, on
-00000a80: 6c79 2074 6865 0a20 2020 2020 2020 2020  ly the.         
-00000a90: 2020 2020 2020 2022 7361 6665 2220 6275         "safe" bu
-00000aa0: 696c 7469 6e20 6675 6e63 7469 6f6e 7320  iltin functions 
-00000ab0: 2873 6565 2053 4146 455f 4255 494c 5449  (see SAFE_BUILTI
-00000ac0: 4e53 2c20 6265 6c6f 7729 2061 7265 2070  NS, below) are p
-00000ad0: 6572 6d69 7474 6564 3b20 616e 7920 6f74  ermitted; any ot
-00000ae0: 6865 7273 0a20 2020 2020 2020 2020 2020  hers.           
-00000af0: 2020 2020 206d 7573 7420 6265 2065 7870       must be exp
-00000b00: 6c69 6369 746c 7920 7370 6563 6966 6965  licitly specifie
-00000b10: 642e 0a20 2020 2020 2020 2020 2020 2061  d..            a
-00000b20: 6c6c 6f77 5f61 7474 7269 6275 7465 5f66  llow_attribute_f
-00000b30: 756e 6374 696f 6e73 3a20 4279 2064 6566  unctions: By def
-00000b40: 6175 6c74 2c20 7768 696c 6520 616c 6c20  ault, while all 
-00000b50: 6174 7472 6962 7574 6573 206f 6620 7661  attributes of va
-00000b60: 7269 6162 6c65 7320 7061 7373 6564 2069  riables passed i
-00000b70: 6e20 746f 0a20 2020 2020 2020 2020 2020  n to.           
-00000b80: 2020 2020 2074 6865 2065 7870 7265 7373       the express
-00000b90: 696f 6e20 6d61 7920 6265 2072 6566 6572  ion may be refer
-00000ba0: 656e 6365 642c 2069 6620 7468 6520 7661  enced, if the va
-00000bb0: 7269 6162 6c65 2063 6f6e 7461 696e 7320  riable contains 
-00000bc0: 6120 6675 6e63 7469 6f6e 2028 652e 672e  a function (e.g.
-00000bd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000be0: 2020 782e 666f 6f28 2929 2074 6865 6e20    x.foo()) then 
-00000bf0: 7468 6174 2066 756e 6374 696f 6e20 6d61  that function ma
-00000c00: 7920 2a6e 6f74 2a20 6265 2063 616c 6c65  y *not* be calle
-00000c10: 642e 2049 6620 7468 6973 2069 7320 7365  d. If this is se
-00000c20: 7420 746f 2074 7275 652c 2073 7563 680a  t to true, such.
-00000c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c40: 6675 6e63 7469 6f6e 7320 6172 6520 7065  functions are pe
-00000c50: 726d 6974 7465 642e 2054 6869 7320 6465  rmitted. This de
-00000c60: 6661 756c 7420 6d61 6b65 7320 6974 2073  fault makes it s
-00000c70: 6166 6520 746f 2070 6173 7320 6f62 6a65  afe to pass obje
-00000c80: 6374 7320 7768 6963 6820 6861 7665 0a20  cts which have. 
-00000c90: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00000ca0: 6f74 656e 7469 616c 6c79 2064 616e 6765  otentially dange
-00000cb0: 726f 7573 206d 6574 686f 6473 2066 6f72  rous methods for
-00000cc0: 2074 6865 6972 2064 6174 6120 616c 6f6e   their data alon
-00000cd0: 652e 204e 6f74 6520 7468 6174 2076 6172  e. Note that var
-00000ce0: 6961 626c 6520 2a70 726f 7065 7274 6965  iable *propertie
-00000cf0: 732a 0a20 2020 2020 2020 2020 2020 2020  s*.             
-00000d00: 2020 2061 7265 2061 6c77 6179 7320 6163     are always ac
-00000d10: 6365 7373 6962 6c65 2e0a 2020 2020 2020  cessible..      
-00000d20: 2020 2020 2020 7661 7269 6162 6c65 733a        variables:
-00000d30: 2049 6620 6769 7665 6e2c 2061 206c 6973   If given, a lis
-00000d40: 7420 6f66 2076 6172 6961 626c 6520 6e61  t of variable na
-00000d50: 6d65 7320 7768 6963 6820 6d61 7920 6265  mes which may be
-00000d60: 2072 6566 6572 656e 6365 6420 6279 2074   referenced by t
-00000d70: 6865 2065 7870 7265 7373 696f 6e2e 0a20  he expression.. 
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2049                 I
-00000d90: 6e20 7468 6973 2063 6173 652c 2061 6e79  n this case, any
-00000da0: 2072 6566 6572 656e 6365 2074 6f20 7661   reference to va
-00000db0: 7269 6162 6c65 7320 6e6f 7420 696e 2074  riables not in t
-00000dc0: 6869 7320 6c69 7374 2077 696c 6c20 7261  his list will ra
-00000dd0: 6973 6520 6120 5379 6e74 6178 4572 726f  ise a SyntaxErro
-00000de0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00000df0: 2020 6174 2063 6f6e 7374 7275 6374 696f    at constructio
-00000e00: 6e20 7469 6d65 2e20 4966 206e 6f74 2067  n time. If not g
-00000e10: 6976 656e 2c20 616c 6c20 7661 7269 6162  iven, all variab
-00000e20: 6c65 206e 616d 6573 2061 7265 2070 6572  le names are per
-00000e30: 6d69 7474 6564 2c20 616e 6420 7468 6520  mitted, and the 
-00000e40: 6163 7475 616c 0a20 2020 2020 2020 2020  actual.         
-00000e50: 2020 2020 2020 2073 6574 206f 6620 7661         set of va
-00000e60: 7269 6162 6c65 7320 7573 6564 2063 616e  riables used can
-00000e70: 2062 6520 6368 6563 6b65 6420 7769 7468   be checked with
-00000e80: 2074 6865 2060 6076 6172 6961 626c 6573   the ``variables
-00000e90: 6060 2070 726f 7065 7274 7920 6f66 2074  `` property of t
-00000ea0: 6869 7320 6f62 6a65 6374 2e0a 0a20 2020  his object...   
-00000eb0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-00000ec0: 2020 2020 2020 2020 2053 796e 7461 7845           SyntaxE
-00000ed0: 7272 6f72 3a20 4966 2074 6865 2065 7870  rror: If the exp
-00000ee0: 7265 7373 696f 6e20 6361 6e6e 6f74 2062  ression cannot b
-00000ef0: 6520 7061 7273 6564 2c20 6f72 2069 6620  e parsed, or if 
-00000f00: 7468 6520 6578 7072 6573 7369 6f6e 2061  the expression a
-00000f10: 7474 656d 7074 6564 2074 6f0a 2020 2020  ttempted to.    
-00000f20: 2020 2020 2020 2020 2020 2020 646f 2073              do s
-00000f30: 6f6d 6574 6869 6e67 2066 6f72 6269 6464  omething forbidd
-00000f40: 656e 2c20 6c69 6b65 2072 6566 6572 656e  en, like referen
-00000f50: 6365 2061 6e20 756e 6b6e 6f77 6e20 7661  ce an unknown va
-00000f60: 7269 6162 6c65 2e0a 2020 2020 2020 2020  riable..        
-00000f70: 2020 2020 5661 6c75 6545 7272 6f72 3a20      ValueError: 
-00000f80: 4966 2074 6865 2065 7870 7265 7373 696f  If the expressio
-00000f90: 6e20 7374 7269 6e67 2063 6f6e 7461 696e  n string contain
-00000fa0: 7320 4e55 4c20 6279 7465 7320 666f 7220  s NUL bytes for 
-00000fb0: 736f 6d65 2072 6561 736f 6e2e 0a20 2020  some reason..   
-00000fc0: 2020 2020 2063 0100 0000 0000 0000 0000       c..........
-00000fd0: 0000 0200 0000 0400 0000 5300 0000 7314  ..........S...s.
-00000fe0: 0000 0069 007c 005d 067d 017c 016a 007c  ...i.|.].}.|.j.|
-00000ff0: 0193 0271 0253 00a9 0029 01da 085f 5f6e  ...q.S...)...__n
-00001000: 616d 655f 5f29 02da 022e 30da 0266 6e72  ame__)....0..fnr
-00001010: 1300 0000 7213 0000 00fa 3c62 7569 6c64  ....r.....<build
-00001020: 2f62 6469 7374 2e6d 6163 6f73 782d 3132  /bdist.macosx-12
-00001030: 2e34 2d78 3836 5f36 342f 6567 672f 7079  .4-x86_64/egg/py
-00001040: 7070 696e 2f75 7469 6c2f 6578 7072 6573  ppin/util/expres
-00001050: 7369 6f6e 2e70 79da 0a3c 6469 6374 636f  sion.py..<dictco
-00001060: 6d70 3e39 0000 0073 0200 0000 1400 7a27  mp>9...s......z'
-00001070: 4578 7072 6573 7369 6f6e 2e5f 5f69 6e69  Expression.__ini
-00001080: 745f 5f2e 3c6c 6f63 616c 733e 2e3c 6469  t__.<locals>.<di
-00001090: 6374 636f 6d70 3eda 0465 7661 6c29 01da  ctcomp>..eval)..
-000010a0: 046d 6f64 654e fa0c 3c65 7870 7265 7373  .modeN..<express
-000010b0: 696f 6e3e 2902 da08 6669 6c65 6e61 6d65  ion>)...filename
-000010c0: 721a 0000 0072 0100 0000 290c da09 5f64  r....r....)..._d
-000010d0: 6963 745f 7375 6dda 0d53 4146 455f 4255  ict_sum..SAFE_BU
-000010e0: 494c 5449 4e53 da04 5f66 6e73 da03 6173  ILTINS.._fns..as
-000010f0: 74da 0570 6172 7365 da04 5f61 7374 da12  t..parse.._ast..
-00001100: 5f56 616c 6964 6174 696f 6e43 6f6e 7465  _ValidationConte
-00001110: 7874 da03 7365 74da 0876 616c 6964 6174  xt..set..validat
-00001120: 65da 0763 6f6d 7069 6c65 da03 5f66 6eda  e..compile.._fn.
-00001130: 0b63 6f5f 6172 6763 6f75 6e74 2906 da04  .co_argcount)...
-00001140: 7365 6c66 7211 0000 0072 0e00 0000 720f  selfr....r....r.
-00001150: 0000 0072 1000 0000 da07 636f 6e74 6578  ...r......contex
-00001160: 7472 1300 0000 7213 0000 0072 1700 0000  tr....r....r....
-00001170: da08 5f5f 696e 6974 5f5f 1400 0000 731a  ..__init__....s.
-00001180: 0000 0002 240e 0106 ff10 0402 0102 0112  ....$...........
-00001190: 0104 0102 0104 fc0c 0612 0114 017a 1345  .............z.E
-000011a0: 7870 7265 7373 696f 6e2e 5f5f 696e 6974  xpression.__init
-000011b0: 5f5f da06 6b77 6172 6773 6301 0000 0000  __..kwargsc.....
-000011c0: 0000 0000 0000 0002 0000 0006 0000 004b  ...............K
-000011d0: 0000 0073 1600 0000 7400 7c00 6a01 6900  ...s....t.|.j.i.
-000011e0: 7402 7c00 6a03 7c01 8302 8303 5300 2902  t.|.j.|.....S.).
-000011f0: 615f 0200 0045 7661 6c75 6174 6520 7468  a_...Evaluate th
-00001200: 6520 6578 7072 6573 7369 6f6e 2c20 6769  e expression, gi
-00001210: 7669 6e67 2069 7420 6163 6365 7373 2074  ving it access t
-00001220: 6f20 616e 7920 696e 6469 6361 7465 6420  o any indicated 
-00001230: 7661 7269 6162 6c65 732e 0a0a 2020 2020  variables...    
-00001240: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00001250: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
-00001260: 416c 6c20 7468 6520 7661 7269 6162 6c65  All the variable
-00001270: 7320 7768 6963 6820 6172 6520 746f 2062  s which are to b
-00001280: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
-00001290: 6578 7072 6573 7369 6f6e 2e20 4e6f 7465  expression. Note
-000012a0: 2074 6861 7420 6966 2061 6e79 0a20 2020   that if any.   
-000012b0: 2020 2020 2020 2020 2020 2020 206d 656d               mem
-000012c0: 6265 7220 6f66 2073 656c 662e 6672 6565  ber of self.free
-000012d0: 5f76 6172 6961 626c 6573 2069 7320 6e6f  _variables is no
-000012e0: 7420 6769 7665 6e20 6865 7265 2c20 796f  t given here, yo
-000012f0: 7520 6172 6520 7665 7279 206c 696b 656c  u are very likel
-00001300: 7920 746f 2067 6574 2061 0a20 2020 2020  y to get a.     
-00001310: 2020 2020 2020 2020 2020 204e 616d 6545             NameE
-00001320: 7272 6f72 2e20 596f 7520 6d61 7920 616c  rror. You may al
-00001330: 736f 2072 6570 6c61 6365 2066 756e 6374  so replace funct
-00001340: 696f 6e73 2062 7920 7061 7373 696e 6720  ions by passing 
-00001350: 7661 6c75 6573 2066 6f72 2074 6865 6d20  values for them 
-00001360: 6865 7265 210a 0a20 2020 2020 2020 2052  here!..        R
-00001370: 6574 7572 6e73 3a20 5468 6520 6576 616c  eturns: The eval
-00001380: 7561 7465 6420 7661 6c75 6520 6f66 2074  uated value of t
-00001390: 6865 2065 7870 7265 7373 696f 6e2e 0a0a  he expression...
-000013a0: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
-000013b0: 2020 2020 2020 2020 2020 2020 416e 7920              Any 
-000013c0: 6578 6365 7074 696f 6e20 7261 6973 6564  exception raised
-000013d0: 2062 7920 7468 6520 6578 7072 6573 7369   by the expressi
-000013e0: 6f6e 2069 7473 656c 662e 0a20 2020 2020  on itself..     
-000013f0: 2020 2020 2020 204e 616d 6545 7272 6f72         NameError
-00001400: 3a20 4966 2073 6f6d 6520 7661 7269 6162  : If some variab
-00001410: 6c65 2072 6566 6572 656e 6365 6420 6279  le referenced by
-00001420: 2074 6865 2065 7870 7265 7373 696f 6e20   the expression 
-00001430: 7761 7320 6e6f 7420 6769 7665 6e20 696e  was not given in
-00001440: 2076 6172 6961 626c 6573 2e0a 2020 2020   variables..    
-00001450: 2020 2020 4e29 0472 1900 0000 7227 0000      N).r....r'..
-00001460: 0072 1d00 0000 721f 0000 0029 0272 2900  .r....r....).r).
-00001470: 0000 722c 0000 0072 1300 0000 7213 0000  ..r,...r....r...
-00001480: 0072 1700 0000 da08 5f5f 6361 6c6c 5f5f  .r......__call__
-00001490: 4700 0000 7302 0000 0016 0e7a 1345 7870  G...s......z.Exp
-000014a0: 7265 7373 696f 6e2e 5f5f 6361 6c6c 5f5f  ression.__call__
-000014b0: 2e63 0100 0000 0000 0000 0000 0000 0100  .c..............
-000014c0: 0000 0100 0000 4300 0000 7308 0000 007c  ......C...s....|
-000014d0: 006a 006a 0153 0029 027a 3f4c 6973 7420  .j.j.S.).z?List 
-000014e0: 616c 6c20 7661 7269 6162 6c65 7320 616e  all variables an
-000014f0: 6420 6675 6e63 7469 6f6e 7320 7265 6665  d functions refe
-00001500: 7265 6e63 6564 2062 7920 7468 6973 2065  renced by this e
-00001510: 7870 7265 7373 696f 6e2e 4e29 0272 2700  xpression.N).r'.
-00001520: 0000 da08 636f 5f6e 616d 6573 a901 7229  ....co_names..r)
-00001530: 0000 0072 1300 0000 7213 0000 0072 1700  ...r....r....r..
-00001540: 0000 7210 0000 0057 0000 0073 0200 0000  ..r....W...s....
-00001550: 0803 7a14 4578 7072 6573 7369 6f6e 2e76  ..z.Expression.v
-00001560: 6172 6961 626c 6573 6301 0000 0000 0000  ariablesc.......
-00001570: 0000 0000 0001 0000 0004 0000 0003 0000  ................
-00001580: 0073 1800 0000 7400 8700 6601 6401 6402  .s....t...f.d.d.
-00001590: 8408 8800 6a01 4400 8301 8301 5300 2904  ....j.D.....S.).
-000015a0: 7a7c 4c69 7374 2061 6c6c 2074 6865 2022  z|List all the "
-000015b0: 6672 6565 2220 7661 7269 6162 6c65 732c  free" variables,
-000015c0: 2069 2e65 2e20 7468 6520 6f6e 6573 2074   i.e. the ones t
-000015d0: 6861 7420 6d75 7374 2062 6520 7370 6563  hat must be spec
-000015e0: 6966 6965 6420 6279 2061 7267 756d 656e  ified by argumen
-000015f0: 7473 2077 6865 6e0a 2020 2020 2020 2020  ts when.        
-00001600: 6361 6c6c 696e 6720 7468 6520 6675 6e63  calling the func
-00001610: 7469 6f6e 2e0a 2020 2020 2020 2020 6301  tion..        c.
-00001620: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00001630: 0000 0033 0000 0073 1e00 0000 8100 7c00  ...3...s......|.
-00001640: 5d0a 7d01 8800 a000 7c01 a101 7302 7c01  ].}.....|...s.|.
-00001650: 5600 0100 7102 6400 5300 a901 4e29 01da  V...q.d.S...N)..
-00001660: 1169 735f 7661 6c69 645f 6675 6e63 7469  .is_valid_functi
-00001670: 6f6e a902 7215 0000 00da 046e 616d 6572  on..r......namer
-00001680: 2f00 0000 7213 0000 0072 1700 0000 da09  /...r....r......
-00001690: 3c67 656e 6578 7072 3e61 0000 0073 0c00  <genexpr>a...s..
-000016a0: 0000 0280 0400 0a01 02ff 0201 0aff 7a2c  ..............z,
-000016b0: 4578 7072 6573 7369 6f6e 2e66 7265 655f  Expression.free_
-000016c0: 7661 7269 6162 6c65 732e 3c6c 6f63 616c  variables.<local
-000016d0: 733e 2e3c 6765 6e65 7870 723e 4e29 02da  s>.<genexpr>N)..
-000016e0: 0574 7570 6c65 7210 0000 0072 2f00 0000  .tupler....r/...
-000016f0: 7213 0000 0072 2f00 0000 7217 0000 00da  r....r/...r.....
-00001700: 0e66 7265 655f 7661 7269 6162 6c65 735c  .free_variables\
-00001710: 0000 0073 0600 0000 0c05 0401 08ff 7a19  ...s..........z.
-00001720: 4578 7072 6573 7369 6f6e 2e66 7265 655f  Expression.free_
-00001730: 7661 7269 6162 6c65 7363 0100 0000 0000  variablesc......
-00001740: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
-00001750: 0000 f306 0000 007c 006a 0053 0029 027a  .......|.j.S.).z
-00001760: 2854 6865 2041 5354 2072 6570 7265 7365  (The AST represe
-00001770: 6e74 6174 696f 6e20 6f66 2074 6869 7320  ntation of this 
-00001780: 6675 6e63 7469 6f6e 2e4e 2901 7222 0000  function.N).r"..
-00001790: 0072 2f00 0000 7213 0000 0072 1300 0000  .r/...r....r....
-000017a0: 7217 0000 0072 2000 0000 6500 0000 7302  r....r ...e...s.
-000017b0: 0000 0006 037a 0e45 7870 7265 7373 696f  .....z.Expressio
-000017c0: 6e2e 6173 7463 0100 0000 0000 0000 0000  n.astc..........
-000017d0: 0000 0100 0000 0100 0000 4300 0000 7237  ..........C...r7
-000017e0: 0000 0029 027a 4054 6865 2064 6963 7469  ...).z@The dicti
-000017f0: 6f6e 6172 7920 6f66 2061 7661 696c 6162  onary of availab
-00001800: 6c65 2066 756e 6374 696f 6e73 2063 616c  le functions cal
-00001810: 6c61 626c 6520 6279 2074 6869 7320 6675  lable by this fu
-00001820: 6e63 7469 6f6e 2e4e a901 721f 0000 0072  nction.N..r....r
-00001830: 2f00 0000 7213 0000 0072 1300 0000 7217  /...r....r....r.
-00001840: 0000 0072 0e00 0000 6a00 0000 7302 0000  ...r....j...s...
-00001850: 0006 027a 1445 7870 7265 7373 696f 6e2e  ...z.Expression.
-00001860: 6675 6e63 7469 6f6e 7363 0100 0000 0000  functionsc......
-00001870: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001880: 0000 730c 0000 0074 00a0 017c 006a 02a1  ..s....t...|.j..
-00001890: 0153 0029 027a 5541 2073 7472 696e 6720  .S.).zUA string 
-000018a0: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-000018b0: 6620 7468 6520 6578 7072 6573 7369 6f6e  f the expression
-000018c0: 2e20 5468 6973 206d 6179 206e 6f74 2062  . This may not b
-000018d0: 6520 6964 656e 7469 6361 6c20 746f 2074  e identical to t
-000018e0: 6865 206f 7269 6769 6e61 6c2e 4e29 0372  he original.N).r
-000018f0: 2000 0000 da07 756e 7061 7273 6572 2200   .....unparser".
-00001900: 0000 722f 0000 0072 1300 0000 7213 0000  ..r/...r....r...
-00001910: 0072 1700 0000 da07 5f5f 7374 725f 5f6e  .r......__str__n
-00001920: 0000 0073 0200 0000 0c02 7a12 4578 7072  ...s......z.Expr
-00001930: 6573 7369 6f6e 2e5f 5f73 7472 5f5f 7233  ession.__str__r3
-00001940: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00001950: 0200 0000 0200 0000 4300 0000 f30a 0000  ........C.......
-00001960: 007c 017c 006a 0076 0053 0029 027a 9554  .|.|.j.v.S.).z.T
-00001970: 6573 7420 6966 2074 6865 2067 6976 656e  est if the given
-00001980: 206e 616d 6520 6973 2061 2076 616c 6964   name is a valid
-00001990: 2066 756e 6374 696f 6e20 666f 7220 7573   function for us
-000019a0: 6520 696e 2074 6869 7320 6578 7072 6573  e in this expres
-000019b0: 7369 6f6e 2e0a 0a20 2020 2020 2020 2054  sion...        T
-000019c0: 6869 7320 6973 2066 6173 7465 7220 7468  his is faster th
-000019d0: 616e 2063 6865 636b 696e 6720 6966 206e  an checking if n
-000019e0: 616d 6520 6973 2069 6e20 7365 6c66 2e66  ame is in self.f
-000019f0: 756e 6374 696f 6e73 2829 2e0a 2020 2020  unctions()..    
-00001a00: 2020 2020 4e72 3800 0000 a902 7229 0000      Nr8.....r)..
-00001a10: 0072 3300 0000 7213 0000 0072 1300 0000  .r3...r....r....
-00001a20: 7217 0000 0072 3100 0000 7200 0000 7302  r....r1...r...s.
-00001a30: 0000 000a 057a 1c45 7870 7265 7373 696f  .....z.Expressio
-00001a40: 6e2e 6973 5f76 616c 6964 5f66 756e 6374  n.is_valid_funct
-00001a50: 696f 6e29 1572 1400 0000 da0a 5f5f 6d6f  ion).r......__mo
-00001a60: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00001a70: 6d65 5f5f da03 7374 7272 0500 0000 7203  me__..strr....r.
-00001a80: 0000 00da 0462 6f6f 6c72 0800 0000 722b  .....boolr....r+
-00001a90: 0000 0072 0200 0000 722d 0000 00da 0870  ...r....r-.....p
-00001aa0: 726f 7065 7274 7972 0a00 0000 7210 0000  ropertyr....r...
-00001ab0: 0072 3600 0000 7220 0000 00da 0341 5354  .r6...r .....AST
-00001ac0: 7204 0000 0072 0e00 0000 723a 0000 0072  r....r....r:...r
-00001ad0: 3100 0000 7213 0000 0072 1300 0000 7213  1...r....r....r.
-00001ae0: 0000 0072 1700 0000 720d 0000 0013 0000  ...r....r.......
-00001af0: 0073 3200 0000 0800 0205 0201 0201 06fa  .s2.............
-00001b00: 0202 02fe 0604 02fc 0205 02fb 0a06 02fa  ................
-00001b10: 0207 0af9 1233 0210 1801 0204 1801 0208  .....3..........
-00001b20: 1201 1604 0e04 1604 720d 0000 00da 0564  ........r......d
-00001b30: 6963 7473 7212 0000 0063 0000 0000 0000  ictsr....c......
-00001b40: 0000 0000 0000 0500 0000 0400 0000 4700  ..............G.
-00001b50: 0000 735e 0000 0064 017d 0164 027d 027c  ..s^...d.}.d.}.|
-00001b60: 0044 005d 0a7d 037c 0372 107c 0264 0337  .D.].}.|.r.|.d.7
-00001b70: 007d 027c 037d 0171 067c 0273 1569 0053  .}.|.}.q.|.s.i.S
-00001b80: 007c 0264 036b 0272 217c 0164 0175 0173  .|.d.k.r!|.d.u.s
-00001b90: 1f4a 0082 017c 0153 0069 007d 047c 0044  .J...|.S.i.}.|.D
-00001ba0: 005d 077d 037c 04a0 007c 03a1 0101 0071  .].}.|...|.....q
-00001bb0: 257c 0453 0029 047a c852 6574 7572 6e20  %|.S.).z.Return 
-00001bc0: 7468 6520 756e 696f 6e20 6f66 2074 6865  the union of the
-00001bd0: 2067 6976 656e 2064 6963 7473 2c20 6d69   given dicts, mi
-00001be0: 6e69 6d69 7a69 6e67 2063 6f70 6965 732e  nimizing copies.
-00001bf0: 2049 7465 6d73 206c 6174 6572 2069 6e20   Items later in 
-00001c00: 6469 6374 7320 7461 6b65 2070 7269 6f72  dicts take prior
-00001c10: 6974 790a 2020 2020 6f76 6572 2069 7465  ity.    over ite
-00001c20: 6d73 2065 6172 6c69 6572 2069 6e20 6469  ms earlier in di
-00001c30: 6374 732e 0a0a 2020 2020 5468 6973 206d  cts...    This m
-00001c40: 6561 6e73 2074 6861 7420 7468 6520 7265  eans that the re
-00001c50: 7475 726e 2076 616c 7565 206d 6179 2062  turn value may b
-00001c60: 6520 6f6e 6520 6f66 2074 6865 206f 7269  e one of the ori
-00001c70: 6769 6e61 6c20 6469 6374 732e 0a20 2020  ginal dicts..   
-00001c80: 204e 7201 0000 00e9 0100 0000 2901 da06   Nr.........)...
-00001c90: 7570 6461 7465 2905 7243 0000 005a 096e  update).rC...Z.n
-00001ca0: 6f6e 5f65 6d70 7479 5a0f 636f 756e 745f  on_emptyZ.count_
-00001cb0: 6e6f 6e5f 656d 7074 795a 056c 6179 6572  non_emptyZ.layer
-00001cc0: da06 7265 7375 6c74 7213 0000 0072 1300  ..resultr....r..
-00001cd0: 0000 7217 0000 0072 1d00 0000 8000 0000  ..r....r........
-00001ce0: 7320 0000 0004 0604 0108 0104 0108 0104  s ..............
-00001cf0: 0102 8004 0204 0108 010c 0104 0104 0308  ................
-00001d00: 010c 0104 0172 1d00 0000 6301 0000 0000  .....r....c.....
-00001d10: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
-00001d20: 0000 0073 2200 0000 6900 7c00 5d0d 7d01  ...s"...i.|.].}.
-00001d30: 7400 7401 7c01 8302 7202 7c01 7402 7401  t.t.|...r.|.t.t.
-00001d40: 7c01 8302 9302 7102 5300 7213 0000 0029  |.....q.S.r....)
-00001d50: 03da 0768 6173 6174 7472 da08 6275 696c  ...hasattr..buil
-00001d60: 7469 6e73 da07 6765 7461 7474 7272 3200  tins..getattrr2.
-00001d70: 0000 7213 0000 0072 1300 0000 7217 0000  ..r....r....r...
-00001d80: 0072 1800 0000 a400 0000 7310 0000 0006  .r........s.....
-00001d90: 0002 0200 7f08 0500 8102 f90a 0106 ff72  ...............r
-00001da0: 1800 0000 2980 da03 6162 73da 0561 6974  ....)...abs..ait
-00001db0: 6572 da03 616c 6cda 0561 6e65 7874 da03  er..all..anext..
-00001dc0: 616e 79da 0561 7363 6969 da03 6269 6e72  any..ascii..binr
-00001dd0: 4000 0000 da09 6279 7465 6172 7261 79da  @.....bytearray.
-00001de0: 0562 7974 6573 da08 6361 6c6c 6162 6c65  .bytes..callable
-00001df0: da03 6368 72da 0763 6f6d 706c 6578 da04  ..chr..complex..
-00001e00: 6469 6374 da03 6469 72da 0664 6976 6d6f  dict..dir..divmo
-00001e10: 64da 0965 6e75 6d65 7261 7465 da06 6669  d..enumerate..fi
-00001e20: 6c74 6572 da05 666c 6f61 74da 0666 6f72  lter..float..for
-00001e30: 6d61 74da 0966 726f 7a65 6e73 6574 7249  mat..frozensetrI
-00001e40: 0000 0072 4700 0000 da04 6861 7368 da03  ...rG.....hash..
-00001e50: 6865 78da 0269 64da 0369 6e74 da0a 6973  hex..id..int..is
-00001e60: 696e 7374 616e 6365 da0a 6973 7375 6263  instance..issubc
-00001e70: 6c61 7373 da04 6974 6572 da03 6c65 6eda  lass..iter..len.
-00001e80: 046c 6973 74da 066c 6f63 616c 73da 036d  .list..locals..m
-00001e90: 6170 da03 6d61 78da 0a6d 656d 6f72 7976  ap..max..memoryv
-00001ea0: 6965 77da 036d 696e da04 6e65 7874 da06  iew..min..next..
-00001eb0: 6f62 6a65 6374 da03 6f63 74da 036f 7264  object..oct..ord
-00001ec0: da03 706f 77da 0572 616e 6765 da04 7265  ..pow..range..re
-00001ed0: 7072 da08 7265 7665 7273 6564 da05 726f  pr..reversed..ro
-00001ee0: 756e 6472 2400 0000 da05 736c 6963 65da  undr$.....slice.
-00001ef0: 0673 6f72 7465 6472 3f00 0000 da03 7375  .sortedr?.....su
-00001f00: 6dda 0573 7570 6572 7235 0000 00da 0474  m..superr5.....t
-00001f10: 7970 65da 0476 6172 73da 037a 6970 da05  ype..vars..zip..
-00001f20: 4661 6c73 65da 0454 7275 65da 0845 6c6c  False..True..Ell
-00001f30: 6970 7369 73da 044e 6f6e 65da 0f41 7269  ipsis..None..Ari
-00001f40: 7468 6d65 7469 6345 7272 6f72 da0e 4173  thmeticError..As
-00001f50: 7365 7274 696f 6e45 7272 6f72 da0e 4174  sertionError..At
-00001f60: 7472 6962 7574 6545 7272 6f72 da0d 4261  tributeError..Ba
-00001f70: 7365 4578 6365 7074 696f 6eda 0f42 6c6f  seException..Blo
-00001f80: 636b 696e 6749 4f45 7272 6f72 da0f 4272  ckingIOError..Br
-00001f90: 6f6b 656e 5069 7065 4572 726f 72da 0b42  okenPipeError..B
-00001fa0: 7566 6665 7245 7272 6f72 da0c 4279 7465  ufferError..Byte
-00001fb0: 7357 6172 6e69 6e67 da11 4368 696c 6450  sWarning..ChildP
-00001fc0: 726f 6365 7373 4572 726f 72da 1643 6f6e  rocessError..Con
-00001fd0: 6e65 6374 696f 6e41 626f 7274 6564 4572  nectionAbortedEr
-00001fe0: 726f 72da 0f43 6f6e 6e65 6374 696f 6e45  ror..ConnectionE
-00001ff0: 7272 6f72 da16 436f 6e6e 6563 7469 6f6e  rror..Connection
-00002000: 5265 6675 7365 6445 7272 6f72 da14 436f  RefusedError..Co
-00002010: 6e6e 6563 7469 6f6e 5265 7365 7445 7272  nnectionResetErr
-00002020: 6f72 da12 4465 7072 6563 6174 696f 6e57  or..DeprecationW
-00002030: 6172 6e69 6e67 da08 454f 4645 7272 6f72  arning..EOFError
-00002040: da0f 456e 636f 6469 6e67 5761 726e 696e  ..EncodingWarnin
-00002050: 67da 1045 6e76 6972 6f6e 6d65 6e74 4572  g..EnvironmentEr
-00002060: 726f 72da 0945 7863 6570 7469 6f6e da0f  ror..Exception..
-00002070: 4669 6c65 4578 6973 7473 4572 726f 72da  FileExistsError.
-00002080: 1146 696c 654e 6f74 466f 756e 6445 7272  .FileNotFoundErr
-00002090: 6f72 da12 466c 6f61 7469 6e67 506f 696e  or..FloatingPoin
-000020a0: 7445 7272 6f72 da0d 4675 7475 7265 5761  tError..FutureWa
-000020b0: 726e 696e 67da 0d47 656e 6572 6174 6f72  rning..Generator
-000020c0: 4578 6974 da07 494f 4572 726f 72da 0b49  Exit..IOError..I
-000020d0: 6d70 6f72 7445 7272 6f72 da0d 496d 706f  mportError..Impo
-000020e0: 7274 5761 726e 696e 67da 1049 6e64 656e  rtWarning..Inden
-000020f0: 7461 7469 6f6e 4572 726f 72da 0a49 6e64  tationError..Ind
-00002100: 6578 4572 726f 72da 1049 6e74 6572 7275  exError..Interru
-00002110: 7074 6564 4572 726f 72da 1149 7341 4469  ptedError..IsADi
-00002120: 7265 6374 6f72 7945 7272 6f72 da08 4b65  rectoryError..Ke
-00002130: 7945 7272 6f72 da11 4b65 7962 6f61 7264  yError..Keyboard
-00002140: 496e 7465 7272 7570 74da 0b4c 6f6f 6b75  Interrupt..Looku
-00002150: 7045 7272 6f72 da0b 4d65 6d6f 7279 4572  pError..MemoryEr
-00002160: 726f 72da 134d 6f64 756c 654e 6f74 466f  ror..ModuleNotFo
-00002170: 756e 6445 7272 6f72 da09 4e61 6d65 4572  undError..NameEr
-00002180: 726f 72da 124e 6f74 4144 6972 6563 746f  ror..NotADirecto
-00002190: 7279 4572 726f 72da 0e4e 6f74 496d 706c  ryError..NotImpl
-000021a0: 656d 656e 7465 64da 134e 6f74 496d 706c  emented..NotImpl
-000021b0: 656d 656e 7465 6445 7272 6f72 da07 4f53  ementedError..OS
-000021c0: 4572 726f 72da 0d4f 7665 7266 6c6f 7745  Error..OverflowE
-000021d0: 7272 6f72 da19 5065 6e64 696e 6744 6570  rror..PendingDep
-000021e0: 7265 6361 7469 6f6e 5761 726e 696e 67da  recationWarning.
-000021f0: 0f50 6572 6d69 7373 696f 6e45 7272 6f72  .PermissionError
-00002200: da12 5072 6f63 6573 734c 6f6f 6b75 7045  ..ProcessLookupE
-00002210: 7272 6f72 da0e 5265 6375 7273 696f 6e45  rror..RecursionE
-00002220: 7272 6f72 da0e 5265 6665 7265 6e63 6545  rror..ReferenceE
-00002230: 7272 6f72 da0f 5265 736f 7572 6365 5761  rror..ResourceWa
-00002240: 726e 696e 67da 0c52 756e 7469 6d65 4572  rning..RuntimeEr
-00002250: 726f 72da 0e52 756e 7469 6d65 5761 726e  ror..RuntimeWarn
-00002260: 696e 67da 1253 746f 7041 7379 6e63 4974  ing..StopAsyncIt
-00002270: 6572 6174 696f 6eda 0d53 746f 7049 7465  eration..StopIte
-00002280: 7261 7469 6f6e da0b 5379 6e74 6178 4572  ration..SyntaxEr
-00002290: 726f 72da 0d53 796e 7461 7857 6172 6e69  ror..SyntaxWarni
-000022a0: 6e67 da0b 5379 7374 656d 4572 726f 72da  ng..SystemError.
-000022b0: 0a53 7973 7465 6d45 7869 74da 0854 6162  .SystemExit..Tab
-000022c0: 4572 726f 72da 0c54 696d 656f 7574 4572  Error..TimeoutEr
-000022d0: 726f 72da 0954 7970 6545 7272 6f72 da11  ror..TypeError..
-000022e0: 556e 626f 756e 644c 6f63 616c 4572 726f  UnboundLocalErro
-000022f0: 72da 1255 6e69 636f 6465 4465 636f 6465  r..UnicodeDecode
-00002300: 4572 726f 72da 1255 6e69 636f 6465 456e  Error..UnicodeEn
-00002310: 636f 6465 4572 726f 72da 0c55 6e69 636f  codeError..Unico
-00002320: 6465 4572 726f 72da 1555 6e69 636f 6465  deError..Unicode
-00002330: 5472 616e 736c 6174 6545 7272 6f72 da0e  TranslateError..
-00002340: 556e 6963 6f64 6557 6172 6e69 6e67 da0b  UnicodeWarning..
-00002350: 5573 6572 5761 726e 696e 67da 0a56 616c  UserWarning..Val
-00002360: 7565 4572 726f 72da 0757 6172 6e69 6e67  ueError..Warning
-00002370: da11 5a65 726f 4469 7669 7369 6f6e 4572  ..ZeroDivisionEr
-00002380: 726f 7272 1e00 0000 6300 0000 0000 0000  rorr....c.......
-00002390: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
-000023a0: 0073 9800 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-000023b0: 6503 6504 6401 3c00 6505 6506 6503 1900  e.e.d.<.e.e.e...
-000023c0: 1900 6504 6402 3c00 6507 6503 6508 6602  ..e.d.<.e.e.e.f.
-000023d0: 1900 6504 6403 3c00 6509 6504 6404 3c00  ..e.d.<.e.e.d.<.
-000023e0: 6405 650a 6a0b 6406 6503 6407 650c 6606  d.e.j.d.e.d.e.f.
-000023f0: 6408 6409 8404 5a0d 640a 650e 6503 650a  d.d...Z.d.e.e.e.
-00002400: 6a0f 6602 1900 6407 6509 6604 640b 640c  j.f...d.e.f.d.d.
-00002410: 8404 5a10 640a 6503 6407 6509 6604 640d  ..Z.d.e.d.e.f.d.
-00002420: 640e 8404 5a11 6405 650a 6a0b 6407 640f  d...Z.d.e.j.d.d.
-00002430: 6604 6410 6411 8404 5a12 640f 5300 2912  f.d.d...Z.d.S.).
-00002440: 7223 0000 0072 1100 0000 7210 0000 0072  r#...r....r....r
-00002450: 0e00 0000 720f 0000 00da 046e 6f64 65da  ....r......node.
-00002460: 0565 7272 6f72 7212 0000 0063 0300 0000  .errorr....c....
-00002470: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00002480: 4300 0000 7340 0000 0074 006a 0164 016b  C...s@...t.j.d.k
-00002490: 0572 1264 027c 016a 027c 016a 037c 006a  .r.d.|.j.|.j.|.j
-000024a0: 047c 016a 057c 016a 0666 066e 0864 027c  .|.j.|.j.f.n.d.|
-000024b0: 016a 027c 016a 037c 006a 0466 047d 0374  .j.|.j.|.j.f.}.t
-000024c0: 077c 027c 0383 0282 0129 034e 6900 000a  .|.|.....).Ni...
-000024d0: 0372 1b00 0000 2908 da03 7379 73da 0a68  .r....)...sys..h
-000024e0: 6578 7665 7273 696f 6eda 066c 696e 656e  exversion..linen
-000024f0: 6fda 0a63 6f6c 5f6f 6666 7365 7472 1100  o..col_offsetr..
-00002500: 0000 da0a 656e 645f 6c69 6e65 6e6f da0e  ....end_lineno..
-00002510: 656e 645f 636f 6c5f 6f66 6673 6574 72b3  end_col_offsetr.
-00002520: 0000 0029 0472 2900 0000 72c4 0000 0072  ...).r)...r....r
-00002530: c500 0000 da07 7061 796c 6f61 6472 1300  ......payloadr..
-00002540: 0000 7213 0000 0072 1700 0000 da04 6661  ..r....r......fa
-00002550: 696c 3401 0000 7318 0000 0008 0a02 f802  il4...s.........
-00002560: 0104 0104 0104 0104 0104 0104 fa10 0902  ................
-00002570: f60a 0c7a 175f 5661 6c69 6461 7469 6f6e  ...z._Validation
-00002580: 436f 6e74 6578 742e 6661 696c 7233 0000  Context.failr3..
-00002590: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-000025a0: 0000 0300 0000 4300 0000 7330 0000 0074  ......C...s0...t
-000025b0: 007c 0174 016a 0283 0272 097c 016a 037d  .|.t.j...r.|.j.}
-000025c0: 017c 006a 0464 0075 0070 177c 017c 006a  .|.j.d.u.p.|.|.j
-000025d0: 0476 0070 177c 017c 006a 0576 0053 0072  .v.p.|.|.j.v.S.r
-000025e0: 3000 0000 2906 7262 0000 0072 2000 0000  0...).rb...r ...
-000025f0: da04 4e61 6d65 7260 0000 0072 1000 0000  ..Namer`...r....
-00002600: 720e 0000 0072 3c00 0000 7213 0000 0072  r....r<...r....r
-00002610: 1300 0000 7217 0000 00da 0d69 735f 7661  ....r......is_va
-00002620: 6c69 645f 6e61 6d65 4301 0000 7308 0000  lid_nameC...s...
-00002630: 000c 0106 011c 0202 ff7a 205f 5661 6c69  .........z _Vali
-00002640: 6461 7469 6f6e 436f 6e74 6578 742e 6973  dationContext.is
-00002650: 5f76 616c 6964 5f6e 616d 6563 0200 0000  _valid_namec....
-00002660: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00002670: 4300 0000 723b 0000 0072 3000 0000 2901  C...r;...r0...).
-00002680: 720e 0000 0072 3c00 0000 7213 0000 0072  r....r<...r....r
-00002690: 1300 0000 7217 0000 0072 3100 0000 4a01  ....r....r1...J.
-000026a0: 0000 7302 0000 000a 017a 245f 5661 6c69  ..s......z$_Vali
-000026b0: 6461 7469 6f6e 436f 6e74 6578 742e 6973  dationContext.is
-000026c0: 5f76 616c 6964 5f66 756e 6374 696f 6e4e  _valid_functionN
-000026d0: 6302 0000 0000 0000 0000 0000 0007 0000  c...............
-000026e0: 0005 0000 0043 0000 0073 9e00 0000 7400  .....C...s....t.
-000026f0: a001 7402 7c01 8301 7403 a102 7d02 6401  ..t.|...t...}.d.
-00002700: 7d03 7404 7c02 7405 8302 7216 7c00 a006  }.t.|.t...r.|...
-00002710: 7c01 7c02 a102 0100 6e09 7407 7c02 8301  |.|.....n.t.|...
-00002720: 721f 7c02 7c01 7c00 8302 7d03 7c03 734b  r.|.|.|...}.|.sK
-00002730: 7408 a009 7c01 a101 4400 5d26 5c02 7d04  t...|...D.]&\.}.
-00002740: 7d05 7404 7c05 740a 8302 723f 7c05 4400  }.t.|.t...r?|.D.
-00002750: 5d18 7d06 7404 7c06 7408 6a0b 8302 723e  ].}.t.|.t.j...r>
-00002760: 7c00 a00c 7c06 a101 0100 7131 7404 7c05  |...|.....q1t.|.
-00002770: 7408 6a0b 8302 724a 7c00 a00c 7c05 a101  t.j...rJ|...|...
-00002780: 0100 7126 6402 5300 6402 5300 2903 7ab6  ..q&d.S.d.S.).z.
-00002790: 5661 6c69 6461 7465 2074 6865 2073 6166  Validate the saf
-000027a0: 6574 7920 6f66 2061 6e20 4153 542e 0a0a  ety of an AST...
-000027b0: 2020 2020 2020 2020 5765 2064 6f6e 2774          We don't
-000027c0: 2075 7365 2061 7374 2e4e 6f64 6556 6973   use ast.NodeVis
-000027d0: 6974 6f72 2062 6563 6175 7365 2069 7473  itor because its
-000027e0: 2072 6563 7572 7369 6f6e 2069 736e 2774   recursion isn't
-000027f0: 2071 7569 7465 2066 6c65 7869 626c 6520   quite flexible 
-00002800: 656e 6f75 6768 2066 6f72 2075 732c 0a20  enough for us,. 
-00002810: 2020 2020 2020 2062 7574 2069 7427 7320         but it's 
-00002820: 6120 7265 616c 6c79 2073 696d 706c 6520  a really simple 
-00002830: 636c 6173 7320 616e 7977 6179 2e0a 2020  class anyway..  
-00002840: 2020 2020 2020 464e 290d da08 4841 4e44        FN)...HAND
-00002850: 4c45 5253 da03 6765 7472 7900 0000 da0d  LERS..getry.....
-00002860: 5f75 6e6b 6e6f 776e 5f6e 6f64 6572 6200  _unknown_noderb.
-00002870: 0000 723f 0000 0072 cd00 0000 7253 0000  ..r?...r....rS..
-00002880: 0072 2000 0000 da0b 6974 6572 5f66 6965  .r .....iter_fie
-00002890: 6c64 7372 6600 0000 7242 0000 0072 2500  ldsrf...rB...r%.
-000028a0: 0000 2907 7229 0000 0072 c400 0000 da02  ..).r)...r......
-000028b0: 6f70 5a10 616c 7265 6164 795f 7265 6375  opZ.already_recu
-000028c0: 7273 6564 da05 6669 656c 64da 0576 616c  rsed..field..val
-000028d0: 7565 da04 6974 656d 7213 0000 0072 1300  ue..itemr....r..
-000028e0: 0000 7217 0000 0072 2500 0000 4d01 0000  ..r....r%...M...
-000028f0: 7324 0000 0010 0604 010a 010e 0108 010a  s$..............
-00002900: 0104 0212 010a 0108 010c 010a 0102 800c  ................
-00002910: 010a 0102 8004 f904 017a 1b5f 5661 6c69  .........z._Vali
-00002920: 6461 7469 6f6e 436f 6e74 6578 742e 7661  dationContext.va
-00002930: 6c69 6461 7465 2913 7214 0000 0072 3d00  lidate).r....r=.
-00002940: 0000 723e 0000 0072 3f00 0000 da0f 5f5f  ..r>...r?.....__
-00002950: 616e 6e6f 7461 7469 6f6e 735f 5f72 0800  annotations__r..
-00002960: 0000 7209 0000 0072 0400 0000 7203 0000  ..r....r....r...
-00002970: 0072 4000 0000 7220 0000 0072 4200 0000  .r@...r ...rB...
-00002980: 7207 0000 0072 cd00 0000 720c 0000 0072  r....r....r....r
-00002990: ce00 0000 72cf 0000 0072 3100 0000 7225  ....r....r1...r%
-000029a0: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
-000029b0: 0000 7217 0000 0072 2300 0000 2e01 0000  ..r....r#.......
-000029c0: 7312 0000 000a 0008 0110 0110 0108 0118  s...............
-000029d0: 021c 0f12 0718 0372 2300 0000 72c4 0000  .......r#...r...
-000029e0: 0072 2a00 0000 6302 0000 0000 0000 0000  .r*...c.........
-000029f0: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-00002a00: 5800 0000 7400 7c00 7401 6a02 8302 7308  X...t.|.t.j...s.
-00002a10: 4a00 8201 7c01 a003 7c00 a101 7318 7c01  J...|...|...s.|.
-00002a20: a004 7c00 6401 7c00 6a05 9b00 6402 9d03  ..|.d.|.j...d...
-00002a30: a102 0100 7400 7c00 6a06 7401 6a07 8302  ....t.|.j.t.j...
-00002a40: 732a 7c01 a004 7c00 6403 7c00 6a05 9b00  s*|...|.d.|.j...
-00002a50: 6402 9d03 a102 0100 6404 5300 2905 4e7a  d.......d.S.).Nz
-00002a60: 1f52 6566 6572 656e 6365 2074 6f20 756e  .Reference to un
-00002a70: 6b6e 6f77 6e20 7661 7269 6162 6c65 2022  known variable "
-00002a80: fa01 227a 2041 7474 656d 7074 2074 6f20  .."z Attempt to 
-00002a90: 6d75 7461 7465 2074 6865 2076 6172 6961  mutate the varia
-00002aa0: 626c 6520 2246 2908 7262 0000 0072 2000  ble "F).rb...r .
-00002ab0: 0000 72ce 0000 0072 cf00 0000 72cd 0000  ..r....r....r...
-00002ac0: 0072 6000 0000 da03 6374 78da 044c 6f61  .r`.....ctx..Loa
-00002ad0: 64a9 0272 c400 0000 722a 0000 0072 1300  d..r....r*...r..
-00002ae0: 0000 7213 0000 0072 1700 0000 da0e 5f76  ..r....r......_v
-00002af0: 616c 6964 6174 655f 6e61 6d65 6401 0000  alidate_named...
-00002b00: 730c 0000 0010 010a 0116 010e 0116 0104  s...............
-00002b10: 0172 dd00 0000 6302 0000 0000 0000 0000  .r....c.........
-00002b20: 0000 0002 0000 0006 0000 0043 0000 0073  ...........C...s
-00002b30: ce00 0000 7400 7c00 7401 6a02 8302 7308  ....t.|.t.j...s.
-00002b40: 4a00 8201 7400 7c00 6a03 7401 6a04 8302  J...t.|.j.t.j...
-00002b50: 7224 7c01 a005 7c00 6a03 6a06 a101 7322  r$|...|.j.j...s"
-00002b60: 7c01 a007 7c00 6401 7c00 6a03 6a06 9b00  |...|.d.|.j.j...
-00002b70: 6402 9d03 a102 0100 6408 5300 7400 7c00  d.......d.S.t.|.
-00002b80: 6a03 7401 6a08 8302 725f 7400 7c00 6a03  j.t.j...r_t.|.j.
-00002b90: 6a09 7401 6a04 8302 7339 7c01 a007 7c00  j.t.j...s9|...|.
-00002ba0: 6403 a102 0100 7c01 a00a 7c00 6a03 6a09  d.....|...|.j.j.
-00002bb0: a101 734d 7c01 a007 7c00 6404 7c00 6a03  ..sM|...|.d.|.j.
-00002bc0: 6a09 6a06 9b00 6402 9d03 a102 0100 7c01  j.j...d.......|.
-00002bd0: 6a0b 735d 7c01 a007 7c00 6405 7c00 6a03  j.s]|...|.d.|.j.
-00002be0: 6a09 6a06 9b00 6406 9d03 a102 0100 6408  j.j...d.......d.
-00002bf0: 5300 7c01 a007 7c00 6407 a102 0100 6408  S.|...|.d.....d.
-00002c00: 5300 2909 4e7a 2241 7474 656d 7074 2074  S.).Nz"Attempt t
-00002c10: 6f20 6361 6c6c 2075 6e6b 6e6f 776e 2066  o call unknown f
-00002c20: 756e 6374 696f 6e20 2272 d900 0000 7a32  unction "r....z2
-00002c30: 5374 7261 6e67 6520 6174 7472 6962 7574  Strange attribut
-00002c40: 653b 2077 6861 7427 7320 6974 7320 6e61  e; what's its na
-00002c50: 6d65 3f20 4e65 7665 7220 6861 7070 656e  me? Never happen
-00002c60: 732e 7a2e 4174 7465 6d70 7420 746f 2063  s.z.Attempt to c
-00002c70: 616c 6c20 6675 6e63 7469 6f6e 2069 6e20  all function in 
-00002c80: 756e 6b6e 6f77 6e20 7661 7269 6162 6c65  unknown variable
-00002c90: 2022 7a1b 4174 7465 6d70 7420 746f 2063   "z.Attempt to c
-00002ca0: 616c 6c20 6d65 7468 6f64 206f 6620 227a  all method of "z
-00002cb0: 4122 2062 7574 2063 616c 6c69 6e67 206d  A" but calling m
-00002cc0: 6574 686f 6473 206f 6620 7661 7269 6162  ethods of variab
-00002cd0: 6c65 7320 6861 7320 6265 656e 2065 7870  les has been exp
-00002ce0: 6c69 6369 746c 7920 666f 7262 6964 6465  licitly forbidde
-00002cf0: 6e2e 7a44 4174 7465 6d70 7465 6420 746f  n.zDAttempted to
-00002d00: 2063 616c 6c20 736f 6d65 7468 696e 6720   call something 
-00002d10: 7468 6174 2069 7320 6e65 6974 6865 7220  that is neither 
-00002d20: 6120 6e61 6d65 206e 6f72 2061 6e20 6174  a name nor an at
-00002d30: 7472 6962 7574 652e 4629 0c72 6200 0000  tribute.F).rb...
-00002d40: 7220 0000 00da 0443 616c 6cda 0466 756e  r .....Call..fun
-00002d50: 6372 ce00 0000 7231 0000 0072 6000 0000  cr....r1...r`...
-00002d60: 72cd 0000 00da 0941 7474 7269 6275 7465  r......Attribute
-00002d70: 72d6 0000 0072 cf00 0000 720f 0000 0072  r....r....r....r
-00002d80: dc00 0000 7213 0000 0072 1300 0000 7217  ....r....r....r.
-00002d90: 0000 00da 0e5f 7661 6c69 6461 7465 5f63  ....._validate_c
-00002da0: 616c 6c6d 0100 0073 2e00 0000 1001 0e01  allm...s........
-00002db0: 0e01 1801 0414 0eed 1001 0c01 0e01 0401  ................
-00002dc0: 0201 1001 04fe 0604 0401 0201 1001 04fe  ................
-00002dd0: 040a 04fc 0401 04ff 0404 72e1 0000 0063  ..........r....c
-00002de0: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00002df0: 0a00 0000 4300 0000 736c 0100 0074 007c  ....C...sl...t.|
-00002e00: 0064 0183 0273 117c 01a0 017c 0064 0274  .d...s.|...|.d.t
-00002e10: 027c 0083 019b 0064 039d 03a1 0201 0067  .|.....d.......g
-00002e20: 007d 027c 006a 0344 005d 367d 0374 047c  .}.|.j.D.]6}.t.|
-00002e30: 036a 0574 066a 0783 0272 2774 047c 036a  .j.t.j...r't.|.j
-00002e40: 056a 0874 066a 0983 0273 2d7c 01a0 017c  .j.t.j...s-|...|
-00002e50: 0064 04a1 0201 007c 016a 0a64 0075 0172  .d.....|.j.d.u.r
-00002e60: 457c 036a 056a 0b7c 016a 0a76 0072 457c  E|.j.j.|.j.v.rE|
-00002e70: 01a0 017c 0064 057c 036a 056a 0b9b 0064  ...|.d.|.j.j...d
-00002e80: 069d 03a1 0201 007c 02a0 0c7c 036a 056a  .......|...|.j.j
-00002e90: 0ba1 0101 0071 167a 567c 016a 0a64 0075  .....q.zV|.j.d.u
-00002ea0: 0172 597c 016a 0aa0 0d7c 02a1 0101 007c  .rY|.j...|.....|
-00002eb0: 006a 0344 005d 137d 037c 01a0 0e7c 036a  .j.D.].}.|...|.j
-00002ec0: 0fa1 0101 007c 036a 1044 005d 077d 047c  .....|.j.D.].}.|
-00002ed0: 01a0 0e7c 04a1 0101 0071 6771 5c74 007c  ...|.....qgq\t.|
-00002ee0: 0064 0783 0272 7b7c 01a0 0e7c 006a 11a1  .d...r{|...|.j..
-00002ef0: 0101 0074 007c 0064 0883 0272 867c 01a0  ...t.|.d...r.|..
-00002f00: 0e7c 006a 12a1 0101 0074 007c 0064 0983  .|.j.....t.|.d..
-00002f10: 0272 917c 01a0 0e7c 006a 13a1 0101 0057  .r.|...|.j.....W
-00002f20: 007c 016a 0a64 0075 0172 a27c 0244 005d  .|.j.d.u.r.|.D.]
-00002f30: 087d 057c 016a 0aa0 147c 05a1 0101 0071  .}.|.j...|.....q
-00002f40: 9964 0a53 007c 016a 0a64 0075 0172 b47c  .d.S.|.j.d.u.r.|
-00002f50: 0244 005d 097d 057c 016a 0aa0 147c 05a1  .D.].}.|.j...|..
-00002f60: 0101 0071 ab77 0077 0029 0b4e da0a 6765  ...q.w.w.).N..ge
-00002f70: 6e65 7261 746f 7273 7a0e 456e 636f 756e  neratorsz.Encoun
-00002f80: 7465 7265 6420 6120 7a15 2077 6974 6820  tered a z. with 
-00002f90: 6e6f 2067 656e 6572 6174 6f72 733f 3f7a  no generators??z
-00002fa0: 1c49 6e76 616c 6964 2067 656e 6572 6174  .Invalid generat
-00002fb0: 6f72 2065 7870 7265 7373 696f 6e7a 1c54  or expressionz.T
-00002fc0: 6865 2063 6f6d 7072 6568 656e 7369 6f6e  he comprehension
-00002fd0: 2076 6172 6961 626c 6520 227a 1722 206d   variable "z." m
-00002fe0: 6173 6b73 2061 2076 6172 6961 626c 6520  asks a variable 
-00002ff0: 6e61 6d65 da03 656c 74da 036b 6579 72d6  name..elt..keyr.
-00003000: 0000 0054 2915 7247 0000 0072 cd00 0000  ...T).rG...r....
-00003010: 7279 0000 0072 e200 0000 7262 0000 00da  ry...r....rb....
-00003020: 0674 6172 6765 7472 2000 0000 72ce 0000  .targetr ...r...
-00003030: 0072 da00 0000 da05 5374 6f72 6572 1000  .r......Storer..
-00003040: 0000 7260 0000 00da 0661 7070 656e 6472  ..r`.....appendr
-00003050: 4500 0000 7225 0000 0072 6400 0000 da03  E...r%...rd.....
-00003060: 6966 7372 e300 0000 72e4 0000 0072 d600  ifsr....r....r..
-00003070: 0000 da07 6469 7363 6172 6429 0672 c400  ....discard).r..
-00003080: 0000 722a 0000 005a 0b63 6869 6c64 5f6e  ..r*...Z.child_n
-00003090: 616d 6573 da09 6765 6e65 7261 746f 72da  ames..generator.
-000030a0: 0963 6f6e 6469 7469 6f6e 5a0a 6368 696c  .conditionZ.chil
-000030b0: 645f 6e61 6d65 7213 0000 0072 1300 0000  d_namer....r....
-000030c0: 7217 0000 00da 175f 7661 6c69 6461 7465  r......_validate
-000030d0: 5f63 6f6d 7072 6568 656e 7369 6f6e 8801  _comprehension..
-000030e0: 0000 734c 0000 000a 0118 0104 030a 0110  ..sL............
-000030f0: 010a 0104 ff0c 0318 0104 0102 010e 0104  ................
-00003100: fe10 0402 030a 010c 010a 020c 010a 010c  ................
-00003110: 0102 ff0a 020c 010a 010c 010a 010c 0102  ................
-00003120: 800a 0308 010e 0104 020a fc08 010e 0102  ................
-00003130: fe02 0172 ec00 0000 6302 0000 0000 0000  ...r....c.......
-00003140: 0000 0000 0002 0000 0006 0000 0043 0000  .............C..
-00003150: 0073 1c00 0000 7c01 a000 7c00 6401 7401  .s....|...|.d.t.
-00003160: 7c00 8301 9b00 6402 9d03 a102 0100 6403  |.....d.......d.
-00003170: 5300 2904 4e7a 134f 7065 7261 7469 6f6e  S.).Nz.Operation
-00003180: 7320 6f66 2074 7970 6520 7a22 2061 7265  s of type z" are
-00003190: 206e 6f74 2073 7570 706f 7274 6564 2069   not supported i
-000031a0: 6e20 4578 7072 6573 7369 6f6e 732e 4629  n Expressions.F)
-000031b0: 0272 cd00 0000 7279 0000 0072 dc00 0000  .r....ry...r....
-000031c0: 7213 0000 0072 1300 0000 7217 0000 0072  r....r....r....r
-000031d0: d200 0000 b201 0000 7308 0000 0004 0110  ........s.......
-000031e0: 0104 ff04 0372 d200 0000 72d0 0000 0072  .....r....r....r
-000031f0: 3300 0000 da06 6163 7469 6f6e 6302 0000  3.....actionc...
-00003200: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00003210: 0043 0000 0073 2000 0000 7400 7401 7c00  .C...s ...t.t.|.
-00003220: 8302 720e 7c01 7402 7403 7401 7c00 8302  ..r.|.t.t.t.|...
-00003230: 3c00 6401 5300 6401 5300 2902 61f6 0200  <.d.S.d.S.).a...
-00003240: 0044 6566 696e 6520 7768 6174 2077 6520  .Define what we 
-00003250: 646f 2077 6865 6e20 7765 2073 6565 2061  do when we see a
-00003260: 206e 6f64 6520 6f66 2061 2067 6976 656e   node of a given
-00003270: 2074 7970 652e 2054 6869 7320 6675 6e63   type. This func
-00003280: 7469 6f6e 2069 7320 6865 7265 2073 6f20  tion is here so 
-00003290: 7468 6174 2077 650a 2020 2020 6361 6e20  that we.    can 
-000032a0: 6861 6e64 6c65 2064 6966 6665 7265 6e74  handle different
-000032b0: 2050 7974 686f 6e20 7665 7273 696f 6e73   Python versions
-000032c0: 2077 6869 6368 2068 6176 6520 6469 6666   which have diff
-000032d0: 6572 656e 7420 4153 5420 7479 7065 732e  erent AST types.
-000032e0: 204e 6f74 6520 7468 6174 2074 6869 7320   Note that this 
-000032f0: 6973 2062 6f74 680a 2020 2020 6120 706f  is both.    a po
-00003300: 7369 7469 7665 2061 6e64 206e 6567 6174  sitive and negat
-00003310: 6976 6520 6c69 7374 2066 6f72 2073 6563  ive list for sec
-00003320: 7572 6974 7920 7265 6173 6f6e 7321 2055  urity reasons! U
-00003330: 6e6b 6e6f 776e 206e 6f64 6520 7479 7065  nknown node type
-00003340: 7320 6172 6520 2a65 7272 6f72 732a 2062  s are *errors* b
-00003350: 790a 2020 2020 6465 6661 756c 7420 756e  y.    default un
-00003360: 7469 6c20 7765 2063 616e 206d 616e 7561  til we can manua
-00003370: 6c6c 7920 7361 7920 7468 6174 2074 6865  lly say that the
-00003380: 7927 7265 206b 6f73 6865 722e 0a0a 2020  y're kosher...  
-00003390: 2020 5468 6520 6163 7469 6f6e 7320 6172    The actions ar
-000033a0: 653a 0a20 2020 2020 2020 204e 6f6e 6520  e:.        None 
-000033b0: 2d2d 2074 6869 7320 6e6f 6465 2069 7320  -- this node is 
-000033c0: 6669 6e65 0a20 2020 2020 2020 2073 7472  fine.        str
-000033d0: 202d 2d20 7468 6973 206e 6f64 6520 6973   -- this node is
-000033e0: 2061 6c77 6179 7320 616e 2065 7272 6f72   always an error
-000033f0: 0a20 2020 2020 2020 2066 756e 6374 696f  .        functio
-00003400: 6e20 2d2d 2063 616c 6c20 7468 6973 2077  n -- call this w
-00003410: 6865 6e20 796f 7520 6669 6e64 2073 7563  hen you find suc
-00003420: 6820 6120 6e6f 6465 2e20 5468 6520 6172  h a node. The ar
-00003430: 6775 6d65 6e74 7320 6172 6520 7468 6520  guments are the 
-00003440: 4153 5420 6e6f 6465 2061 6e64 2074 6865  AST node and the
-00003450: 0a20 2020 2020 2020 2020 2020 205f 5661  .            _Va
-00003460: 6c69 6461 7469 6f6e 436f 6e74 6578 743b  lidationContext;
-00003470: 2074 6865 2072 6574 7572 6e20 7661 6c75   the return valu
-00003480: 6520 7368 6f75 6c64 2062 6520 6661 6c73  e should be fals
-00003490: 6520 746f 2061 6c6c 6f77 2074 6865 2073  e to allow the s
-000034a0: 6361 6e6e 6572 2074 6f20 7265 6375 7273  canner to recurs
-000034b0: 650a 2020 2020 2020 2020 2020 2020 7468  e.            th
-000034c0: 726f 7567 6820 616c 6c20 7468 6520 6e6f  rough all the no
-000034d0: 6465 2773 2063 6869 6c64 7265 6e20 6173  de's children as
-000034e0: 2075 7375 616c 2c20 6f72 2074 7275 6520   usual, or true 
-000034f0: 6966 2074 6865 2066 756e 6374 696f 6e20  if the function 
-00003500: 6861 7320 616c 7265 6164 7920 7461 6b65  has already take
-00003510: 6e0a 2020 2020 2020 2020 2020 2020 6361  n.            ca
-00003520: 7265 206f 6620 7468 6174 2069 7473 656c  re of that itsel
-00003530: 662e 0a20 2020 204e 2904 7247 0000 0072  f..    N).rG...r
-00003540: 2000 0000 72d0 0000 0072 4900 0000 2902   ...r....rI...).
-00003550: 7233 0000 0072 ed00 0000 7213 0000 0072  r3...r....r....r
-00003560: 1300 0000 7217 0000 00da 035f 6f6e c001  ....r......_on..
-00003570: 0000 7306 0000 000a 0e12 0104 ff72 ee00  ..s..........r..
-00003580: 0000 7a33 5661 7269 6162 6c65 2061 7373  ..z3Variable ass
-00003590: 6967 6e6d 656e 7420 6973 206e 6f74 2070  ignment is not p
-000035a0: 6572 6d69 7474 6564 2069 6e20 6578 7072  ermitted in expr
-000035b0: 6573 7369 6f6e 737a 3156 6172 6961 626c  essionsz1Variabl
-000035c0: 6520 6465 6c65 7469 6f6e 2069 7320 6e6f  e deletion is no
-000035d0: 7420 7065 726d 6974 7465 6420 696e 2065  t permitted in e
-000035e0: 7870 7265 7373 696f 6e73 7a49 4465 636c  xpressionszIDecl
-000035f0: 6172 6975 6e67 206f 626a 6563 7473 2c20  ariung objects, 
-00003600: 636c 6173 7365 732c 206f 7220 6675 6e63  classes, or func
-00003610: 7469 6f6e 7320 6973 206e 6f74 2070 6572  tions is not per
-00003620: 6d69 7474 6564 2069 6e20 6578 7072 6573  mitted in expres
-00003630: 7369 6f6e 737a 3149 6d70 6f72 7469 6e67  sionsz1Importing
-00003640: 206f 626a 6563 7473 2069 7320 6e6f 7420   objects is not 
-00003650: 7065 726d 6974 7465 6420 696e 2065 7870  permitted in exp
-00003660: 7265 7373 696f 6e73 7a38 436f 6e74 726f  ressionsz8Contro
-00003670: 6c20 666c 6f77 206f 7065 7261 7469 6f6e  l flow operation
-00003680: 7320 6172 6520 6e6f 7420 7065 726d 6974  s are not permit
-00003690: 7465 6420 696e 2065 7870 7265 7373 696f  ted in expressio
-000036a0: 6e73 da06 4d6f 6475 6c65 da0c 4675 6e63  ns..Module..Func
-000036b0: 7469 6f6e 5479 7065 da0b 496e 7465 7261  tionType..Intera
-000036c0: 6374 6976 65da 0843 6f6e 7374 616e 74da  ctive..Constant.
-000036d0: 0e46 6f72 6d61 7474 6564 5661 6c75 65da  .FormattedValue.
-000036e0: 094a 6f69 6e65 6453 7472 7205 0000 0072  .JoinedStrr....r
-000036f0: 0a00 0000 7209 0000 0072 0400 0000 72ce  ....r....r....r.
-00003700: 0000 0072 db00 0000 72e6 0000 00da 0344  ...r....r......D
-00003710: 656c da07 5374 6172 7265 64da 0445 7870  el..Starred..Exp
-00003720: 72da 0755 6e61 7279 4f70 da04 5541 6464  r..UnaryOp..UAdd
-00003730: da04 5553 7562 da03 4e6f 74da 0649 6e76  ..USub..Not..Inv
-00003740: 6572 74da 0542 696e 4f70 da03 4164 64da  ert..BinOp..Add.
-00003750: 0353 7562 da04 4d75 6c74 da03 4469 76da  .Sub..Mult..Div.
-00003760: 0846 6c6f 6f72 4469 76da 034d 6f64 da03  .FloorDiv..Mod..
-00003770: 506f 77da 064c 5368 6966 74da 0652 5368  Pow..LShift..RSh
-00003780: 6966 74da 0542 6974 4f72 da06 4269 7458  ift..BitOr..BitX
-00003790: 6f72 da06 4269 7441 6e64 da07 4d61 744d  or..BitAnd..MatM
-000037a0: 756c 74da 0642 6f6f 6c4f 70da 0341 6e64  ult..BoolOp..And
-000037b0: da02 4f72 da07 436f 6d70 6172 65da 0245  ..Or..Compare..E
-000037c0: 71da 054e 6f74 4571 da02 4c74 da03 4c74  q..NotEq..Lt..Lt
-000037d0: 45da 0247 74da 0347 7445 da02 4973 da05  E..Gt..GtE..Is..
-000037e0: 4973 4e6f 74da 016e da05 4e6f 7449 6e72  IsNot..n..NotInr
-000037f0: de00 0000 da07 6b65 7977 6f72 64da 0549  ......keyword..I
-00003800: 6645 7870 72e0 0000 00da 094e 616d 6564  fExpr......Named
-00003810: 4578 7072 da09 5375 6273 6372 6970 74da  Expr..Subscript.
-00003820: 0553 6c69 6365 da08 4c69 7374 436f 6d70  .Slice..ListComp
-00003830: da07 5365 7443 6f6d 70da 0c47 656e 6572  ..SetComp..Gener
-00003840: 6174 6f72 4578 70da 0844 6963 7443 6f6d  atorExp..DictCom
-00003850: 70da 0d63 6f6d 7072 6568 656e 7369 6f6e  p..comprehension
-00003860: da06 4173 7369 676e da09 416e 6e41 7373  ..Assign..AnnAss
-00003870: 6967 6eda 0941 7567 4173 7369 676e da05  ign..AugAssign..
-00003880: 5261 6973 65da 0641 7373 6572 74da 0644  Raise..Assert..D
-00003890: 656c 6574 65da 0450 6173 73da 0649 6d70  elete..Pass..Imp
-000038a0: 6f72 74da 0a49 6d70 6f72 7446 726f 6dda  ort..ImportFrom.
-000038b0: 0561 6c69 6173 da02 4966 da03 466f 72da  .alias..If..For.
-000038c0: 0557 6869 6c65 da05 4272 6561 6bda 0843  .While..Break..C
-000038d0: 6f6e 7469 6e75 65da 0354 7279 5a07 5472  ontinue..TryZ.Tr
-000038e0: 7953 7461 72da 0d45 7863 6570 7448 616e  yStar..ExceptHan
-000038f0: 646c 6572 da04 5769 7468 da08 7769 7468  dler..With..with
-00003900: 6974 656d da05 4d61 7463 68da 0a6d 6174  item..Match..mat
-00003910: 6368 5f63 6173 65da 0a4d 6174 6368 5661  ch_case..MatchVa
-00003920: 6c75 65da 0e4d 6174 6368 5369 6e67 6c65  lue..MatchSingle
-00003930: 746f 6eda 0d4d 6174 6368 5365 7175 656e  ton..MatchSequen
-00003940: 6365 da09 4d61 7463 6853 7461 72da 0c4d  ce..MatchStar..M
-00003950: 6174 6368 4d61 7070 696e 67da 0a4d 6174  atchMapping..Mat
-00003960: 6368 436c 6173 73da 074d 6174 6368 4173  chClass..MatchAs
-00003970: da07 4d61 7463 684f 72da 0b46 756e 6374  ..MatchOr..Funct
-00003980: 696f 6e44 6566 da06 4c61 6d62 6461 da09  ionDef..Lambda..
-00003990: 6172 6775 6d65 6e74 73da 0361 7267 da06  arguments..arg..
-000039a0: 5265 7475 726e da05 5969 656c 64da 0959  Return..Yield..Y
-000039b0: 6965 6c64 4672 6f6d da06 476c 6f62 616c  ieldFrom..Global
-000039c0: 7a3a 4d6f 6469 6679 696e 6720 676c 6f62  z:Modifying glob
-000039d0: 616c 2076 6172 6961 626c 6573 2069 7320  al variables is 
-000039e0: 6e6f 7420 7065 726d 6974 7465 6420 696e  not permitted in
-000039f0: 2065 7870 7265 7373 696f 6e73 da08 4e6f   expressions..No
-00003a00: 6e6c 6f63 616c 7a3c 4d6f 6469 6679 696e  nlocalz<Modifyin
-00003a10: 6720 6e6f 6e6c 6f63 616c 2076 6172 6961  g nonlocal varia
-00003a20: 626c 6573 2069 7320 6e6f 7420 7065 726d  bles is not perm
-00003a30: 6974 7465 6420 696e 2065 7870 7265 7373  itted in express
-00003a40: 696f 6e73 da08 436c 6173 7344 6566 da10  ions..ClassDef..
-00003a50: 4173 796e 6346 756e 6374 696f 6e44 6566  AsyncFunctionDef
-00003a60: da05 4177 6169 74da 0841 7379 6e63 466f  ..Await..AsyncFo
-00003a70: 72da 0941 7379 6e63 5769 7468 2925 7220  r..AsyncWith)%r 
-00003a80: 0000 0072 4800 0000 72c6 0000 00da 0674  ...rH...r......t
-00003a90: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
-00003aa0: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00003ab0: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00003ac0: 0000 720b 0000 0072 0c00 0000 726d 0000  ..r....r....rm..
-00003ad0: 0072 0d00 0000 7256 0000 0072 1d00 0000  .r....rV...r....
-00003ae0: 721e 0000 0072 3f00 0000 72d8 0000 0072  r....r?...r....r
-00003af0: 2300 0000 7242 0000 0072 4000 0000 72dd  #...rB...r@...r.
-00003b00: 0000 0072 e100 0000 72ec 0000 0072 d200  ...r....r....r..
-00003b10: 0000 5a07 5f41 4354 494f 4e72 d000 0000  ..Z._ACTIONr....
-00003b20: 72ee 0000 005a 094e 4f5f 4153 5349 474e  r....Z.NO_ASSIGN
-00003b30: 5a09 4e4f 5f44 454c 4554 455a 0a4e 4f5f  Z.NO_DELETEZ.NO_
-00003b40: 4445 434c 4152 455a 094e 4f5f 494d 504f  DECLAREZ.NO_IMPO
-00003b50: 5254 5a0a 4e4f 5f43 4f4e 5452 4f4c 7213  RTZ.NO_CONTROLr.
-00003b60: 0000 0072 1300 0000 7213 0000 0072 1700  ...r....r....r..
-00003b70: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00003b80: 7302 0100 000a 0008 0108 0134 0110 0f12  s..........4....
-00003b90: 6d06 2402 0216 fe00 7f10 0b18 3618 0918  m.$.........6...
-00003ba0: 1b18 2a1c 0a1a 0116 0304 1204 0104 0104  ..*.............
-00003bb0: 0104 010a 020a 010a 010a 010a 010a 010a  ................
-00003bc0: 010a 010a 010a 010a 010a 010a 020a 010a  ................
+00000070: 5a0c 6d0d 5a0d 6d0e 5a0e 6d0f 5a0f 0100  Z.m.Z.m.Z.m.Z...
+00000080: 4700 6404 6405 8400 6405 6510 8303 5a11  G.d.d...d.e...Z.
+00000090: 6406 6512 6407 6512 6604 6408 6409 8404  d.e.d.e.f.d.d...
+000000a0: 5a13 640a 640b 8400 640c 4400 8301 5a14  Z.d.d...d.D...Z.
+000000b0: 6507 6515 6506 6602 1900 6516 640d 3c00  e.e.e.f...e.d.<.
+000000c0: 4700 640e 640f 8400 640f 6509 8303 5a17  G.d.d...d.e...Z.
+000000d0: 6410 6501 6a18 6411 6517 6407 6519 6606  d.e.j.d.e.d.e.f.
+000000e0: 6412 6413 8404 5a1a 6410 6501 6a18 6411  d.d...Z.d.e.j.d.
+000000f0: 6517 6407 6519 6606 6414 6415 8404 5a1b  e.d.e.f.d.d...Z.
+00000100: 6410 6501 6a18 6411 6517 6407 6519 6606  d.e.j.d.e.d.e.f.
+00000110: 6416 6417 8404 5a1c 6410 6501 6a18 6411  d.d...Z.d.e.j.d.
+00000120: 6517 6407 6519 6606 6418 6419 8404 5a1d  e.d.e.f.d.d...Z.
+00000130: 650f 6402 6515 6506 6501 6a18 6517 6702  e.d.e.e.e.j.e.g.
+00000140: 6519 6602 1900 6603 1900 5a1e 6900 5a1f  e.f...f...Z.i.Z.
+00000150: 6507 650e 6501 6a18 1900 651e 6602 1900  e.e.e.j...e.f...
+00000160: 6516 641a 3c00 641b 6515 641c 651e 6407  e.d.<.d.e.d.e.d.
+00000170: 6402 6606 641d 641e 8404 5a20 641f 5a21  d.f.d.d...Z d.Z!
+00000180: 6420 5a22 6421 5a23 6422 5a24 6423 5a25  d Z"d!Z#d"Z$d#Z%
+00000190: 6520 6405 6402 8302 0100 6520 6424 6402  e d.d.....e d$d.
+000001a0: 8302 0100 6520 6425 6402 8302 0100 6520  ....e d%d.....e 
+000001b0: 6426 6525 8302 0100 6520 6427 6402 8302  d&e%....e d'd...
+000001c0: 0100 6520 6428 6402 8302 0100 6520 6429  ..e d(d.....e d)
+000001d0: 6402 8302 0100 6520 642a 6402 8302 0100  d.....e d*d.....
+000001e0: 6520 642b 6402 8302 0100 6520 642c 6402  e d+d.....e d,d.
+000001f0: 8302 0100 6520 642d 6402 8302 0100 6520  ....e d-d.....e 
+00000200: 642e 651a 8302 0100 6520 642f 6402 8302  d.e.....e d/d...
+00000210: 0100 6520 6430 6521 8302 0100 6520 6431  ..e d0e!....e d1
+00000220: 6522 8302 0100 6520 6432 6402 8302 0100  e"....e d2d.....
+00000230: 6520 6433 6402 8302 0100 6520 6434 6402  e d3d.....e d4d.
+00000240: 8302 0100 6520 6435 6402 8302 0100 6520  ....e d5d.....e 
+00000250: 6436 6402 8302 0100 6520 6437 6402 8302  d6d.....e d7d...
+00000260: 0100 6520 6438 6402 8302 0100 6520 6439  ..e d8d.....e d9
+00000270: 6402 8302 0100 6520 643a 6402 8302 0100  d.....e d:d.....
+00000280: 6520 643b 6402 8302 0100 6520 643c 6402  e d;d.....e d<d.
+00000290: 8302 0100 6520 643d 6402 8302 0100 6520  ....e d=d.....e 
+000002a0: 643e 6402 8302 0100 6520 643f 6402 8302  d>d.....e d?d...
+000002b0: 0100 6520 6440 6402 8302 0100 6520 6441  ..e d@d.....e dA
+000002c0: 6402 8302 0100 6520 6442 6402 8302 0100  d.....e dBd.....
+000002d0: 6520 6443 6402 8302 0100 6520 6444 6402  e dCd.....e dDd.
+000002e0: 8302 0100 6520 6445 6402 8302 0100 6520  ....e dEd.....e 
+000002f0: 6446 6402 8302 0100 6520 6447 6402 8302  dFd.....e dGd...
+00000300: 0100 6520 6448 6402 8302 0100 6520 6449  ..e dHd.....e dI
+00000310: 6402 8302 0100 6520 644a 6402 8302 0100  d.....e dJd.....
+00000320: 6520 644b 6402 8302 0100 6520 644c 6402  e dKd.....e dLd.
+00000330: 8302 0100 6520 644d 6402 8302 0100 6520  ....e dMd.....e 
+00000340: 644e 6402 8302 0100 6520 644f 6402 8302  dNd.....e dOd...
+00000350: 0100 6520 6450 6402 8302 0100 6520 6451  ..e dPd.....e dQ
+00000360: 6402 8302 0100 6520 6452 6402 8302 0100  d.....e dRd.....
+00000370: 6520 6453 6402 8302 0100 6520 6454 6402  e dSd.....e dTd.
+00000380: 8302 0100 6520 6455 651b 8302 0100 6520  ....e dUe.....e 
+00000390: 6456 6402 8302 0100 6520 6457 6402 8302  dVd.....e dWd...
+000003a0: 0100 6520 6458 6402 8302 0100 6520 6459  ..e dXd.....e dY
+000003b0: 6521 8302 0100 6520 645a 6402 8302 0100  e!....e dZd.....
+000003c0: 6520 645b 6402 8302 0100 6520 645c 651c  e d[d.....e d\e.
+000003d0: 8302 0100 6520 645d 651c 8302 0100 6520  ....e d]e.....e 
+000003e0: 645e 651c 8302 0100 6520 645f 651c 8302  d^e.....e d_e...
+000003f0: 0100 6520 6460 6402 8302 0100 6520 6461  ..e d`d.....e da
+00000400: 6521 8302 0100 6520 6462 6521 8302 0100  e!....e dbe!....
+00000410: 6520 6463 6521 8302 0100 6520 6464 6525  e dce!....e dde%
+00000420: 8302 0100 6520 6465 6525 8302 0100 6520  ....e dee%....e 
+00000430: 6466 6522 8302 0100 6520 6467 6402 8302  dfe"....e dgd...
+00000440: 0100 6520 6468 6524 8302 0100 6520 6469  ..e dhe$....e di
+00000450: 6524 8302 0100 6520 646a 6402 8302 0100  e$....e djd.....
+00000460: 6520 646b 6402 8302 0100 6520 646c 6402  e dkd.....e dld.
+00000470: 8302 0100 6520 646d 6402 8302 0100 6520  ....e dmd.....e 
+00000480: 646e 6402 8302 0100 6520 646f 6402 8302  dnd.....e dod...
+00000490: 0100 6520 6470 6402 8302 0100 6520 6471  ..e dpd.....e dq
+000004a0: 6402 8302 0100 6520 6472 6402 8302 0100  d.....e drd.....
+000004b0: 6520 6473 6402 8302 0100 6520 6474 6402  e dsd.....e dtd.
+000004c0: 8302 0100 6520 6475 6402 8302 0100 6520  ....e dud.....e 
+000004d0: 6476 6402 8302 0100 6520 6477 6402 8302  dvd.....e dwd...
+000004e0: 0100 6520 6478 6402 8302 0100 6520 6479  ..e dxd.....e dy
+000004f0: 6402 8302 0100 6520 647a 6402 8302 0100  d.....e dzd.....
+00000500: 6520 647b 6402 8302 0100 6520 647c 6402  e d{d.....e d|d.
+00000510: 8302 0100 6520 647d 6402 8302 0100 6520  ....e d}d.....e 
+00000520: 647e 6402 8302 0100 6520 647f 6523 8302  d~d.....e d.e#..
+00000530: 0100 6520 6480 6402 8302 0100 6520 6481  ..e d.d.....e d.
+00000540: 6402 8302 0100 6520 6482 6402 8302 0100  d.....e d.d.....
+00000550: 6520 6483 6525 8302 0100 6520 6484 6525  e d.e%....e d.e%
+00000560: 8302 0100 6520 6485 6525 8302 0100 6520  ....e d.e%....e 
+00000570: 6486 6487 8302 0100 6520 6488 6489 8302  d.d.....e d.d...
+00000580: 0100 6520 648a 6523 8302 0100 6520 648b  ..e d.e#....e d.
+00000590: 6523 8302 0100 6520 648c 6402 8302 0100  e#....e d.d.....
+000005a0: 6520 648d 6402 8302 0100 6520 648e 6402  e d.d.....e d.d.
+000005b0: 8302 0100 6402 5300 298f 7a26 5361 6665  ....d.S.).z&Safe
+000005c0: 2065 7661 6c75 6174 696f 6e20 6f66 2050   evaluation of P
+000005d0: 7974 686f 6e20 6578 7072 6573 7369 6f6e  ython expression
+000005e0: 732e e900 0000 004e 290b da03 416e 79da  s......N)...Any.
+000005f0: 0843 616c 6c61 626c 65da 0444 6963 74da  .Callable..Dict.
+00000600: 044c 6973 74da 0a4e 616d 6564 5475 706c  .List..NamedTupl
+00000610: 65da 084e 6f52 6574 7572 6eda 084f 7074  e..NoReturn..Opt
+00000620: 696f 6e61 6cda 0353 6574 da05 5475 706c  ional..Set..Tupl
+00000630: 65da 0454 7970 65da 0555 6e69 6f6e 6300  e..Type..Unionc.
+00000640: 0000 0000 0000 0000 0000 0000 0000 000b  ................
+00000650: 0000 0040 0000 0073 d400 0000 6500 5a01  ...@...s....e.Z.
+00000660: 6400 5a02 6401 5a03 6700 6402 6403 6404  d.Z.d.Z.g.d.d.d.
+00000670: 9c03 6405 6504 6406 6505 6506 1900 6407  ..d.e.d.e.e...d.
+00000680: 6507 6408 6508 6505 6504 1900 1900 6409  e.d.e.e.e.....d.
+00000690: 6403 660a 640a 640b 8406 5a09 640c 650a  d.f.d.d...Z.d.e.
+000006a0: 6409 650a 6604 640d 640e 8404 5a0b 650c  d.e.f.d.d...Z.e.
+000006b0: 6409 650d 6504 640f 6602 1900 6602 6410  d.e.e.d.f...f.d.
+000006c0: 6411 8404 8301 5a0e 650c 6409 650d 6504  d.....Z.e.d.e.e.
+000006d0: 640f 6602 1900 6602 6412 6413 8404 8301  d.f...f.d.d.....
+000006e0: 5a0f 650c 6409 6510 6a11 6602 6414 6415  Z.e.d.e.j.f.d.d.
+000006f0: 8404 8301 5a10 6409 6512 6504 6506 6602  ....Z.d.e.e.e.f.
+00000700: 1900 6602 6416 6417 8404 5a13 6409 6504  ..f.d.d...Z.d.e.
+00000710: 6602 6418 6419 8404 5a14 641a 6504 6409  f.d.d...Z.d.e.d.
+00000720: 6507 6604 641b 641c 8404 5a15 6403 5300  e.f.d.d...Z.d.S.
+00000730: 291d da0a 4578 7072 6573 7369 6f6e 6162  )...Expressionab
+00000740: 0700 0045 7870 7265 7373 696f 6e20 696d  ...Expression im
+00000750: 706c 656d 656e 7473 2022 7361 6665 2220  plements "safe" 
+00000760: 6576 616c 7561 7469 6f6e 206f 6620 7573  evaluation of us
+00000770: 6572 2d65 6e74 6572 6564 2050 7974 686f  er-entered Pytho
+00000780: 6e20 6578 7072 6573 7369 6f6e 732e 0a0a  n expressions...
+00000790: 2020 2020 5468 6973 2069 7320 7361 6665      This is safe
+000007a0: 2069 6e20 7468 6174 2069 7420 7472 6965   in that it trie
+000007b0: 7320 746f 2065 6e73 7572 6520 7468 6174  s to ensure that
+000007c0: 2074 6865 2067 6976 656e 2065 7870 7265   the given expre
+000007d0: 7373 696f 6e20 6361 6e6e 6f74 206d 7574  ssion cannot mut
+000007e0: 6174 6520 7468 6520 7374 6174 6520 6f66  ate the state of
+000007f0: 0a20 2020 2074 6865 2073 7973 7465 6d20  .    the system 
+00000800: 2865 2e67 2e20 6d6f 6469 6679 696e 6720  (e.g. modifying 
+00000810: 6174 7472 6962 7574 6573 292c 2065 7865  attributes), exe
+00000820: 6375 7465 2049 2f4f 2c20 6f72 2063 6861  cute I/O, or cha
+00000830: 6e67 6520 7468 6520 6272 6f61 6465 7220  nge the broader 
+00000840: 636f 6e74 726f 6c20 666c 6f77 2e0a 2020  control flow..  
+00000850: 2020 486f 7765 7665 722c 2069 7420 6973    However, it is
+00000860: 206e 6f74 2070 6572 6665 6374 6c79 2073   not perfectly s
+00000870: 6166 653a 2053 7566 6669 6369 656e 746c  afe: Sufficientl
+00000880: 7920 636f 6d70 6c65 7820 6578 7072 6573  y complex expres
+00000890: 7369 6f6e 7320 6361 6e20 6372 6173 6820  sions can crash 
+000008a0: 7468 6520 656e 7469 7265 0a20 2020 2069  the entire.    i
+000008b0: 6e74 6572 7072 6574 6572 2120 5365 6520  nterpreter! See 
+000008c0: 636f 6d70 696c 6528 2920 666f 7220 6465  compile() for de
+000008d0: 7461 696c 732e 204c 656e 6774 682d 6c69  tails. Length-li
+000008e0: 6d69 7469 6e67 2074 6865 2069 6e70 7574  miting the input
+000008f0: 206d 6179 2068 656c 702e 0a0a 2020 2020   may help...    
+00000900: 4172 6773 3a0a 2020 2020 2020 2020 6578  Args:.        ex
+00000910: 7072 6573 7369 6f6e 3a20 4120 5079 7468  pression: A Pyth
+00000920: 6f6e 2065 7870 7265 7373 696f 6e20 746f  on expression to
+00000930: 2062 6520 7475 726e 6564 2069 6e74 6f20   be turned into 
+00000940: 7468 6973 206f 626a 6563 742e 0a20 2020  this object..   
+00000950: 2020 2020 2066 756e 6374 696f 6e73 3a20       functions: 
+00000960: 4120 6c69 7374 206f 6620 6675 6e63 7469  A list of functi
+00000970: 6f6e 7320 7768 6963 6820 6d61 7920 6265  ons which may be
+00000980: 2075 7365 6420 696e 2065 7870 7265 7373   used in express
+00000990: 696f 6e73 2e20 4279 2064 6566 6175 6c74  ions. By default
+000009a0: 2c20 6f6e 6c79 2074 6865 0a20 2020 2020  , only the.     
+000009b0: 2020 2020 2020 2022 7361 6665 2220 6275         "safe" bu
+000009c0: 696c 7469 6e20 6675 6e63 7469 6f6e 7320  iltin functions 
+000009d0: 2873 6565 2053 4146 455f 4255 494c 5449  (see SAFE_BUILTI
+000009e0: 4e53 2c20 6265 6c6f 7729 2061 7265 2070  NS, below) are p
+000009f0: 6572 6d69 7474 6564 3b20 616e 7920 6f74  ermitted; any ot
+00000a00: 6865 7273 0a20 2020 2020 2020 2020 2020  hers.           
+00000a10: 206d 7573 7420 6265 2065 7870 6c69 6369   must be explici
+00000a20: 746c 7920 7370 6563 6966 6965 642e 0a20  tly specified.. 
+00000a30: 2020 2020 2020 2061 6c6c 6f77 5f61 7474         allow_att
+00000a40: 7269 6275 7465 5f66 756e 6374 696f 6e73  ribute_functions
+00000a50: 3a20 4279 2064 6566 6175 6c74 2c20 7768  : By default, wh
+00000a60: 696c 6520 616c 6c20 6174 7472 6962 7574  ile all attribut
+00000a70: 6573 206f 6620 7661 7269 6162 6c65 7320  es of variables 
+00000a80: 7061 7373 6564 2069 6e20 746f 0a20 2020  passed in to.   
+00000a90: 2020 2020 2020 2020 2074 6865 2065 7870           the exp
+00000aa0: 7265 7373 696f 6e20 6d61 7920 6265 2072  ression may be r
+00000ab0: 6566 6572 656e 6365 642c 2069 6620 7468  eferenced, if th
+00000ac0: 6520 7661 7269 6162 6c65 2063 6f6e 7461  e variable conta
+00000ad0: 696e 7320 6120 6675 6e63 7469 6f6e 2028  ins a function (
+00000ae0: 652e 672e 2c0a 2020 2020 2020 2020 2020  e.g.,.          
+00000af0: 2020 782e 666f 6f28 2929 2074 6865 6e20    x.foo()) then 
+00000b00: 7468 6174 2066 756e 6374 696f 6e20 6d61  that function ma
+00000b10: 7920 2a6e 6f74 2a20 6265 2063 616c 6c65  y *not* be calle
+00000b20: 642e 2049 6620 7468 6973 2069 7320 7365  d. If this is se
+00000b30: 7420 746f 2074 7275 652c 2073 7563 680a  t to true, such.
+00000b40: 2020 2020 2020 2020 2020 2020 6675 6e63              func
+00000b50: 7469 6f6e 7320 6172 6520 7065 726d 6974  tions are permit
+00000b60: 7465 642e 2054 6869 7320 6465 6661 756c  ted. This defaul
+00000b70: 7420 6d61 6b65 7320 6974 2073 6166 6520  t makes it safe 
+00000b80: 746f 2070 6173 7320 6f62 6a65 6374 7320  to pass objects 
+00000b90: 7768 6963 6820 6861 7665 0a20 2020 2020  which have.     
+00000ba0: 2020 2020 2020 2070 6f74 656e 7469 616c         potential
+00000bb0: 6c79 2064 616e 6765 726f 7573 206d 6574  ly dangerous met
+00000bc0: 686f 6473 2066 6f72 2074 6865 6972 2064  hods for their d
+00000bd0: 6174 6120 616c 6f6e 652e 204e 6f74 6520  ata alone. Note 
+00000be0: 7468 6174 2076 6172 6961 626c 6520 2a70  that variable *p
+00000bf0: 726f 7065 7274 6965 732a 0a20 2020 2020  roperties*.     
+00000c00: 2020 2020 2020 2061 7265 2061 6c77 6179         are alway
+00000c10: 7320 6163 6365 7373 6962 6c65 2e0a 2020  s accessible..  
+00000c20: 2020 2020 2020 7661 7269 6162 6c65 733a        variables:
+00000c30: 2049 6620 6769 7665 6e2c 2061 206c 6973   If given, a lis
+00000c40: 7420 6f66 2076 6172 6961 626c 6520 6e61  t of variable na
+00000c50: 6d65 7320 7768 6963 6820 6d61 7920 6265  mes which may be
+00000c60: 2072 6566 6572 656e 6365 6420 6279 2074   referenced by t
+00000c70: 6865 2065 7870 7265 7373 696f 6e2e 0a20  he expression.. 
+00000c80: 2020 2020 2020 2020 2020 2049 6e20 7468             In th
+00000c90: 6973 2063 6173 652c 2061 6e79 2072 6566  is case, any ref
+00000ca0: 6572 656e 6365 2074 6f20 7661 7269 6162  erence to variab
+00000cb0: 6c65 7320 6e6f 7420 696e 2074 6869 7320  les not in this 
+00000cc0: 6c69 7374 2077 696c 6c20 7261 6973 6520  list will raise 
+00000cd0: 6120 5379 6e74 6178 4572 726f 720a 2020  a SyntaxError.  
+00000ce0: 2020 2020 2020 2020 2020 6174 2063 6f6e            at con
+00000cf0: 7374 7275 6374 696f 6e20 7469 6d65 2e20  struction time. 
+00000d00: 4966 206e 6f74 2067 6976 656e 2c20 616c  If not given, al
+00000d10: 6c20 7661 7269 6162 6c65 206e 616d 6573  l variable names
+00000d20: 2061 7265 2070 6572 6d69 7474 6564 2c20   are permitted, 
+00000d30: 616e 6420 7468 6520 6163 7475 616c 0a20  and the actual. 
+00000d40: 2020 2020 2020 2020 2020 2073 6574 206f             set o
+00000d50: 6620 7661 7269 6162 6c65 7320 7573 6564  f variables used
+00000d60: 2063 616e 2062 6520 6368 6563 6b65 6420   can be checked 
+00000d70: 7769 7468 2074 6865 2060 6076 6172 6961  with the ``varia
+00000d80: 626c 6573 6060 2070 726f 7065 7274 7920  bles`` property 
+00000d90: 6f66 2074 6869 7320 6f62 6a65 6374 2e0a  of this object..
+00000da0: 0a20 2020 2052 6169 7365 733a 0a20 2020  .    Raises:.   
+00000db0: 2020 2020 2053 796e 7461 7845 7272 6f72       SyntaxError
+00000dc0: 3a20 4966 2074 6865 2065 7870 7265 7373  : If the express
+00000dd0: 696f 6e20 6361 6e6e 6f74 2062 6520 7061  ion cannot be pa
+00000de0: 7273 6564 2c20 6f72 2069 6620 7468 6520  rsed, or if the 
+00000df0: 6578 7072 6573 7369 6f6e 2061 7474 656d  expression attem
+00000e00: 7074 6564 2074 6f0a 2020 2020 2020 2020  pted to.        
+00000e10: 2020 2020 646f 2073 6f6d 6574 6869 6e67      do something
+00000e20: 2066 6f72 6269 6464 656e 2c20 6c69 6b65   forbidden, like
+00000e30: 2072 6566 6572 656e 6365 2061 6e20 756e   reference an un
+00000e40: 6b6e 6f77 6e20 7661 7269 6162 6c65 2e0a  known variable..
+00000e50: 2020 2020 2020 2020 5661 6c75 6545 7272          ValueErr
+00000e60: 6f72 3a20 4966 2074 6865 2065 7870 7265  or: If the expre
+00000e70: 7373 696f 6e20 7374 7269 6e67 2063 6f6e  ssion string con
+00000e80: 7461 696e 7320 4e55 4c20 6279 7465 7320  tains NUL bytes 
+00000e90: 666f 7220 736f 6d65 2072 6561 736f 6e2e  for some reason.
+00000ea0: 0a20 2020 2046 4e29 03da 0966 756e 6374  .    FN)...funct
+00000eb0: 696f 6e73 da19 616c 6c6f 775f 6174 7472  ions..allow_attr
+00000ec0: 6962 7574 655f 6675 6e63 7469 6f6e 73da  ibute_functions.
+00000ed0: 0976 6172 6961 626c 6573 da0a 6578 7072  .variables..expr
+00000ee0: 6573 7369 6f6e 720e 0000 0072 0f00 0000  essionr....r....
+00000ef0: 7210 0000 00da 0672 6574 7572 6e63 0200  r......returnc..
+00000f00: 0000 0000 0000 0300 0000 0600 0000 0500  ................
+00000f10: 0000 4300 0000 7378 0000 0074 0074 0164  ..C...sx...t.t.d
+00000f20: 0164 0284 007c 0244 0083 0183 027c 005f  .d...|.D.....|._
+00000f30: 0274 036a 047c 0164 0364 048d 027c 005f  .t.j.|.d.d...|._
+00000f40: 0574 067c 017c 0464 0075 0172 1d74 077c  .t.|.|.d.u.r.t.|
+00000f50: 0483 016e 0164 007c 006a 027c 0383 047d  ...n.d.|.j.|...}
+00000f60: 057c 05a0 087c 006a 05a1 0101 0074 097c  .|...|.j.....t.|
+00000f70: 006a 0564 0564 0364 068d 037c 005f 0a7c  .j.d.d.d...|._.|
+00000f80: 006a 0a6a 0b64 076b 0273 3a4a 0082 0164  .j.j.d.k.s:J...d
+00000f90: 0053 0029 084e 6301 0000 0000 0000 0000  .S.).Nc.........
+00000fa0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00000fb0: 1400 0000 6900 7c00 5d06 7d01 7c01 6a00  ....i.|.].}.|.j.
+00000fc0: 7c01 9302 7102 5300 a900 2901 da08 5f5f  |...q.S...)...__
+00000fd0: 6e61 6d65 5f5f 2902 da02 2e30 da02 666e  name__)....0..fn
+00000fe0: 7213 0000 0072 1300 0000 fa3c 6275 696c  r....r.....<buil
+00000ff0: 642f 6264 6973 742e 6d61 636f 7378 2d31  d/bdist.macosx-1
+00001000: 322e 342d 7838 365f 3634 2f65 6767 2f70  2.4-x86_64/egg/p
+00001010: 7970 7069 6e2f 7574 696c 2f65 7870 7265  yppin/util/expre
+00001020: 7373 696f 6e2e 7079 da0a 3c64 6963 7463  ssion.py..<dictc
+00001030: 6f6d 703e 3c00 0000 7302 0000 0014 007a  omp><...s......z
+00001040: 2745 7870 7265 7373 696f 6e2e 5f5f 696e  'Expression.__in
+00001050: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64  it__.<locals>.<d
+00001060: 6963 7463 6f6d 703e da04 6576 616c 2901  ictcomp>..eval).
+00001070: da04 6d6f 6465 fa0c 3c65 7870 7265 7373  ..mode..<express
+00001080: 696f 6e3e 2902 da08 6669 6c65 6e61 6d65  ion>)...filename
+00001090: 721a 0000 0072 0100 0000 290c da09 5f64  r....r....)..._d
+000010a0: 6963 745f 7375 6dda 0d53 4146 455f 4255  ict_sum..SAFE_BU
+000010b0: 494c 5449 4e53 da04 5f66 6e73 da03 6173  ILTINS.._fns..as
+000010c0: 74da 0570 6172 7365 da04 5f61 7374 da12  t..parse.._ast..
+000010d0: 5f56 616c 6964 6174 696f 6e43 6f6e 7465  _ValidationConte
+000010e0: 7874 da03 7365 74da 0876 616c 6964 6174  xt..set..validat
+000010f0: 65da 0763 6f6d 7069 6c65 da03 5f66 6eda  e..compile.._fn.
+00001100: 0b63 6f5f 6172 6763 6f75 6e74 2906 da04  .co_argcount)...
+00001110: 7365 6c66 7211 0000 0072 0e00 0000 720f  selfr....r....r.
+00001120: 0000 0072 1000 0000 da07 636f 6e74 6578  ...r......contex
+00001130: 7472 1300 0000 7213 0000 0072 1700 0000  tr....r....r....
+00001140: da08 5f5f 696e 6974 5f5f 3300 0000 731a  ..__init__3...s.
+00001150: 0000 0002 080e 0106 ff10 0402 0102 0112  ................
+00001160: 0104 0102 0104 fc0c 0612 0114 017a 1345  .............z.E
+00001170: 7870 7265 7373 696f 6e2e 5f5f 696e 6974  xpression.__init
+00001180: 5f5f da06 6b77 6172 6773 6301 0000 0000  __..kwargsc.....
+00001190: 0000 0000 0000 0002 0000 0006 0000 004b  ...............K
+000011a0: 0000 0073 1600 0000 7400 7c00 6a01 6900  ...s....t.|.j.i.
+000011b0: 7402 7c00 6a03 7c01 8302 8303 5300 2902  t.|.j.|.....S.).
+000011c0: 615f 0200 0045 7661 6c75 6174 6520 7468  a_...Evaluate th
+000011d0: 6520 6578 7072 6573 7369 6f6e 2c20 6769  e expression, gi
+000011e0: 7669 6e67 2069 7420 6163 6365 7373 2074  ving it access t
+000011f0: 6f20 616e 7920 696e 6469 6361 7465 6420  o any indicated 
+00001200: 7661 7269 6162 6c65 732e 0a0a 2020 2020  variables...    
+00001210: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00001220: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
+00001230: 416c 6c20 7468 6520 7661 7269 6162 6c65  All the variable
+00001240: 7320 7768 6963 6820 6172 6520 746f 2062  s which are to b
+00001250: 6520 7061 7373 6564 2074 6f20 7468 6520  e passed to the 
+00001260: 6578 7072 6573 7369 6f6e 2e20 4e6f 7465  expression. Note
+00001270: 2074 6861 7420 6966 2061 6e79 0a20 2020   that if any.   
+00001280: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+00001290: 6265 7220 6f66 2073 656c 662e 6672 6565  ber of self.free
+000012a0: 5f76 6172 6961 626c 6573 2069 7320 6e6f  _variables is no
+000012b0: 7420 6769 7665 6e20 6865 7265 2c20 796f  t given here, yo
+000012c0: 7520 6172 6520 7665 7279 206c 696b 656c  u are very likel
+000012d0: 7920 746f 2067 6574 2061 0a20 2020 2020  y to get a.     
+000012e0: 2020 2020 2020 2020 2020 204e 616d 6545             NameE
+000012f0: 7272 6f72 2e20 596f 7520 6d61 7920 616c  rror. You may al
+00001300: 736f 2072 6570 6c61 6365 2066 756e 6374  so replace funct
+00001310: 696f 6e73 2062 7920 7061 7373 696e 6720  ions by passing 
+00001320: 7661 6c75 6573 2066 6f72 2074 6865 6d20  values for them 
+00001330: 6865 7265 210a 0a20 2020 2020 2020 2052  here!..        R
+00001340: 6574 7572 6e73 3a20 5468 6520 6576 616c  eturns: The eval
+00001350: 7561 7465 6420 7661 6c75 6520 6f66 2074  uated value of t
+00001360: 6865 2065 7870 7265 7373 696f 6e2e 0a0a  he expression...
+00001370: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+00001380: 2020 2020 2020 2020 2020 2020 416e 7920              Any 
+00001390: 6578 6365 7074 696f 6e20 7261 6973 6564  exception raised
+000013a0: 2062 7920 7468 6520 6578 7072 6573 7369   by the expressi
+000013b0: 6f6e 2069 7473 656c 662e 0a20 2020 2020  on itself..     
+000013c0: 2020 2020 2020 204e 616d 6545 7272 6f72         NameError
+000013d0: 3a20 4966 2073 6f6d 6520 7661 7269 6162  : If some variab
+000013e0: 6c65 2072 6566 6572 656e 6365 6420 6279  le referenced by
+000013f0: 2074 6865 2065 7870 7265 7373 696f 6e20   the expression 
+00001400: 7761 7320 6e6f 7420 6769 7665 6e20 696e  was not given in
+00001410: 2076 6172 6961 626c 6573 2e0a 2020 2020   variables..    
+00001420: 2020 2020 4e29 0472 1900 0000 7227 0000      N).r....r'..
+00001430: 0072 1d00 0000 721f 0000 0029 0272 2900  .r....r....).r).
+00001440: 0000 722c 0000 0072 1300 0000 7213 0000  ..r,...r....r...
+00001450: 0072 1700 0000 da08 5f5f 6361 6c6c 5f5f  .r......__call__
+00001460: 4a00 0000 7302 0000 0016 0e7a 1345 7870  J...s......z.Exp
+00001470: 7265 7373 696f 6e2e 5f5f 6361 6c6c 5f5f  ression.__call__
+00001480: 2e63 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001490: 0000 0100 0000 4300 0000 7308 0000 007c  ......C...s....|
+000014a0: 006a 006a 0153 0029 027a 3f4c 6973 7420  .j.j.S.).z?List 
+000014b0: 616c 6c20 7661 7269 6162 6c65 7320 616e  all variables an
+000014c0: 6420 6675 6e63 7469 6f6e 7320 7265 6665  d functions refe
+000014d0: 7265 6e63 6564 2062 7920 7468 6973 2065  renced by this e
+000014e0: 7870 7265 7373 696f 6e2e 4e29 0272 2700  xpression.N).r'.
+000014f0: 0000 da08 636f 5f6e 616d 6573 a901 7229  ....co_names..r)
+00001500: 0000 0072 1300 0000 7213 0000 0072 1700  ...r....r....r..
+00001510: 0000 7210 0000 005a 0000 0073 0200 0000  ..r....Z...s....
+00001520: 0803 7a14 4578 7072 6573 7369 6f6e 2e76  ..z.Expression.v
+00001530: 6172 6961 626c 6573 6301 0000 0000 0000  ariablesc.......
+00001540: 0000 0000 0001 0000 0004 0000 0003 0000  ................
+00001550: 0073 1800 0000 7400 8700 6601 6401 6402  .s....t...f.d.d.
+00001560: 8408 8800 6a01 4400 8301 8301 5300 2904  ....j.D.....S.).
+00001570: 7a7c 4c69 7374 2061 6c6c 2074 6865 2022  z|List all the "
+00001580: 6672 6565 2220 7661 7269 6162 6c65 732c  free" variables,
+00001590: 2069 2e65 2e20 7468 6520 6f6e 6573 2074   i.e. the ones t
+000015a0: 6861 7420 6d75 7374 2062 6520 7370 6563  hat must be spec
+000015b0: 6966 6965 6420 6279 2061 7267 756d 656e  ified by argumen
+000015c0: 7473 2077 6865 6e0a 2020 2020 2020 2020  ts when.        
+000015d0: 6361 6c6c 696e 6720 7468 6520 6675 6e63  calling the func
+000015e0: 7469 6f6e 2e0a 2020 2020 2020 2020 6301  tion..        c.
+000015f0: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00001600: 0000 0033 0000 0073 1e00 0000 8100 7c00  ...3...s......|.
+00001610: 5d0a 7d01 8800 a000 7c01 a101 7302 7c01  ].}.....|...s.|.
+00001620: 5600 0100 7102 6400 5300 a901 4e29 01da  V...q.d.S...N)..
+00001630: 1169 735f 7661 6c69 645f 6675 6e63 7469  .is_valid_functi
+00001640: 6f6e a902 7215 0000 00da 046e 616d 6572  on..r......namer
+00001650: 2f00 0000 7213 0000 0072 1700 0000 da09  /...r....r......
+00001660: 3c67 656e 6578 7072 3e64 0000 0073 0c00  <genexpr>d...s..
+00001670: 0000 0280 0400 0a01 02ff 0201 0aff 7a2c  ..............z,
+00001680: 4578 7072 6573 7369 6f6e 2e66 7265 655f  Expression.free_
+00001690: 7661 7269 6162 6c65 732e 3c6c 6f63 616c  variables.<local
+000016a0: 733e 2e3c 6765 6e65 7870 723e 4e29 02da  s>.<genexpr>N)..
+000016b0: 0574 7570 6c65 7210 0000 0072 2f00 0000  .tupler....r/...
+000016c0: 7213 0000 0072 2f00 0000 7217 0000 00da  r....r/...r.....
+000016d0: 0e66 7265 655f 7661 7269 6162 6c65 735f  .free_variables_
+000016e0: 0000 0073 0600 0000 0c05 0401 08ff 7a19  ...s..........z.
+000016f0: 4578 7072 6573 7369 6f6e 2e66 7265 655f  Expression.free_
+00001700: 7661 7269 6162 6c65 7363 0100 0000 0000  variablesc......
+00001710: 0000 0000 0000 0100 0000 0100 0000 4300  ..............C.
+00001720: 0000 f306 0000 007c 006a 0053 0029 027a  .......|.j.S.).z
+00001730: 2854 6865 2041 5354 2072 6570 7265 7365  (The AST represe
+00001740: 6e74 6174 696f 6e20 6f66 2074 6869 7320  ntation of this 
+00001750: 6675 6e63 7469 6f6e 2e4e 2901 7222 0000  function.N).r"..
+00001760: 0072 2f00 0000 7213 0000 0072 1300 0000  .r/...r....r....
+00001770: 7217 0000 0072 2000 0000 6800 0000 7302  r....r ...h...s.
+00001780: 0000 0006 037a 0e45 7870 7265 7373 696f  .....z.Expressio
+00001790: 6e2e 6173 7463 0100 0000 0000 0000 0000  n.astc..........
+000017a0: 0000 0100 0000 0100 0000 4300 0000 7237  ..........C...r7
+000017b0: 0000 0029 027a 4054 6865 2064 6963 7469  ...).z@The dicti
+000017c0: 6f6e 6172 7920 6f66 2061 7661 696c 6162  onary of availab
+000017d0: 6c65 2066 756e 6374 696f 6e73 2063 616c  le functions cal
+000017e0: 6c61 626c 6520 6279 2074 6869 7320 6675  lable by this fu
+000017f0: 6e63 7469 6f6e 2e4e a901 721f 0000 0072  nction.N..r....r
+00001800: 2f00 0000 7213 0000 0072 1300 0000 7217  /...r....r....r.
+00001810: 0000 0072 0e00 0000 6d00 0000 7302 0000  ...r....m...s...
+00001820: 0006 027a 1445 7870 7265 7373 696f 6e2e  ...z.Expression.
+00001830: 6675 6e63 7469 6f6e 7363 0100 0000 0000  functionsc......
+00001840: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001850: 0000 730c 0000 0074 00a0 017c 006a 02a1  ..s....t...|.j..
+00001860: 0153 0029 027a 5541 2073 7472 696e 6720  .S.).zUA string 
+00001870: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
+00001880: 6620 7468 6520 6578 7072 6573 7369 6f6e  f the expression
+00001890: 2e20 5468 6973 206d 6179 206e 6f74 2062  . This may not b
+000018a0: 6520 6964 656e 7469 6361 6c20 746f 2074  e identical to t
+000018b0: 6865 206f 7269 6769 6e61 6c2e 4e29 0372  he original.N).r
+000018c0: 2000 0000 da07 756e 7061 7273 6572 2200   .....unparser".
+000018d0: 0000 722f 0000 0072 1300 0000 7213 0000  ..r/...r....r...
+000018e0: 0072 1700 0000 da07 5f5f 7374 725f 5f71  .r......__str__q
+000018f0: 0000 0073 0200 0000 0c02 7a12 4578 7072  ...s......z.Expr
+00001900: 6573 7369 6f6e 2e5f 5f73 7472 5f5f 7233  ession.__str__r3
+00001910: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00001920: 0200 0000 0200 0000 4300 0000 f30a 0000  ........C.......
+00001930: 007c 017c 006a 0076 0053 0029 027a 9554  .|.|.j.v.S.).z.T
+00001940: 6573 7420 6966 2074 6865 2067 6976 656e  est if the given
+00001950: 206e 616d 6520 6973 2061 2076 616c 6964   name is a valid
+00001960: 2066 756e 6374 696f 6e20 666f 7220 7573   function for us
+00001970: 6520 696e 2074 6869 7320 6578 7072 6573  e in this expres
+00001980: 7369 6f6e 2e0a 0a20 2020 2020 2020 2054  sion...        T
+00001990: 6869 7320 6973 2066 6173 7465 7220 7468  his is faster th
+000019a0: 616e 2063 6865 636b 696e 6720 6966 206e  an checking if n
+000019b0: 616d 6520 6973 2069 6e20 7365 6c66 2e66  ame is in self.f
+000019c0: 756e 6374 696f 6e73 2829 2e0a 2020 2020  unctions()..    
+000019d0: 2020 2020 4e72 3800 0000 a902 7229 0000      Nr8.....r)..
+000019e0: 0072 3300 0000 7213 0000 0072 1300 0000  .r3...r....r....
+000019f0: 7217 0000 0072 3100 0000 7500 0000 7302  r....r1...u...s.
+00001a00: 0000 000a 057a 1c45 7870 7265 7373 696f  .....z.Expressio
+00001a10: 6e2e 6973 5f76 616c 6964 5f66 756e 6374  n.is_valid_funct
+00001a20: 696f 6e29 1672 1400 0000 da0a 5f5f 6d6f  ion).r......__mo
+00001a30: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00001a40: 6d65 5f5f da07 5f5f 646f 635f 5fda 0373  me__..__doc__..s
+00001a50: 7472 7205 0000 0072 0300 0000 da04 626f  trr....r......bo
+00001a60: 6f6c 7208 0000 0072 2b00 0000 7202 0000  olr....r+...r...
+00001a70: 0072 2d00 0000 da08 7072 6f70 6572 7479  .r-.....property
+00001a80: 720a 0000 0072 1000 0000 7236 0000 0072  r....r....r6...r
+00001a90: 2000 0000 da03 4153 5472 0400 0000 720e   .....ASTr....r.
+00001aa0: 0000 0072 3a00 0000 7231 0000 0072 1300  ...r:...r1...r..
+00001ab0: 0000 7213 0000 0072 1300 0000 7217 0000  ..r....r....r...
+00001ac0: 0072 0d00 0000 1500 0000 7334 0000 0008  .r........s4....
+00001ad0: 0004 0102 2102 0102 0106 fa02 0202 fe06  ....!...........
+00001ae0: 0402 fc02 0502 fb0a 0602 fa02 070a f912  ................
+00001af0: 1702 1018 0102 0418 0102 0812 0116 040e  ................
+00001b00: 0416 0472 0d00 0000 da05 6469 6374 7372  ...r......dictsr
+00001b10: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
+00001b20: 0005 0000 0004 0000 0047 0000 0073 5e00  .........G...s^.
+00001b30: 0000 6401 7d01 6402 7d02 7c00 4400 5d0a  ..d.}.d.}.|.D.].
+00001b40: 7d03 7c03 7210 7c02 6403 3700 7d02 7c03  }.|.r.|.d.7.}.|.
+00001b50: 7d01 7106 7c02 7315 6900 5300 7c02 6403  }.q.|.s.i.S.|.d.
+00001b60: 6b02 7221 7c01 6401 7501 731f 4a00 8201  k.r!|.d.u.s.J...
+00001b70: 7c01 5300 6900 7d04 7c00 4400 5d07 7d03  |.S.i.}.|.D.].}.
+00001b80: 7c04 a000 7c03 a101 0100 7125 7c04 5300  |...|.....q%|.S.
+00001b90: 2904 7ac8 5265 7475 726e 2074 6865 2075  ).z.Return the u
+00001ba0: 6e69 6f6e 206f 6620 7468 6520 6769 7665  nion of the give
+00001bb0: 6e20 6469 6374 732c 206d 696e 696d 697a  n dicts, minimiz
+00001bc0: 696e 6720 636f 7069 6573 2e20 4974 656d  ing copies. Item
+00001bd0: 7320 6c61 7465 7220 696e 2064 6963 7473  s later in dicts
+00001be0: 2074 616b 6520 7072 696f 7269 7479 0a20   take priority. 
+00001bf0: 2020 206f 7665 7220 6974 656d 7320 6561     over items ea
+00001c00: 726c 6965 7220 696e 2064 6963 7473 2e0a  rlier in dicts..
+00001c10: 0a20 2020 2054 6869 7320 6d65 616e 7320  .    This means 
+00001c20: 7468 6174 2074 6865 2072 6574 7572 6e20  that the return 
+00001c30: 7661 6c75 6520 6d61 7920 6265 206f 6e65  value may be one
+00001c40: 206f 6620 7468 6520 6f72 6967 696e 616c   of the original
+00001c50: 2064 6963 7473 2e0a 2020 2020 4e72 0100   dicts..    Nr..
+00001c60: 0000 e901 0000 0029 01da 0675 7064 6174  .......)...updat
+00001c70: 6529 0572 4400 0000 5a09 6e6f 6e5f 656d  e).rD...Z.non_em
+00001c80: 7074 795a 0f63 6f75 6e74 5f6e 6f6e 5f65  ptyZ.count_non_e
+00001c90: 6d70 7479 5a05 6c61 7965 72da 0672 6573  mptyZ.layer..res
+00001ca0: 756c 7472 1300 0000 7213 0000 0072 1700  ultr....r....r..
+00001cb0: 0000 721d 0000 0083 0000 0073 2000 0000  ..r........s ...
+00001cc0: 0406 0401 0801 0401 0801 0401 0280 0402  ................
+00001cd0: 0401 0801 0c01 0401 0403 0801 0c01 0401  ................
+00001ce0: 721d 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001cf0: 0000 0200 0000 0600 0000 4300 0000 7322  ..........C...s"
+00001d00: 0000 0069 007c 005d 0d7d 0174 0074 017c  ...i.|.].}.t.t.|
+00001d10: 0183 0272 027c 0174 0274 017c 0183 0293  ...r.|.t.t.|....
+00001d20: 0271 0253 0072 1300 0000 2903 da07 6861  .q.S.r....)...ha
+00001d30: 7361 7474 72da 0862 7569 6c74 696e 73da  sattr..builtins.
+00001d40: 0767 6574 6174 7472 7232 0000 0072 1300  .getattrr2...r..
+00001d50: 0000 7213 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00001d60: 00a7 0000 0073 1000 0000 0600 0202 007f  .....s..........
+00001d70: 0805 0081 02f9 0a01 06ff 7218 0000 0029  ..........r....)
+00001d80: 80da 0361 6273 da05 6169 7465 72da 0361  ...abs..aiter..a
+00001d90: 6c6c da05 616e 6578 74da 0361 6e79 da05  ll..anext..any..
+00001da0: 6173 6369 69da 0362 696e 7241 0000 00da  ascii..binrA....
+00001db0: 0962 7974 6561 7272 6179 da05 6279 7465  .bytearray..byte
+00001dc0: 73da 0863 616c 6c61 626c 65da 0363 6872  s..callable..chr
+00001dd0: da07 636f 6d70 6c65 78da 0464 6963 74da  ..complex..dict.
+00001de0: 0364 6972 da06 6469 766d 6f64 da09 656e  .dir..divmod..en
+00001df0: 756d 6572 6174 65da 0666 696c 7465 72da  umerate..filter.
+00001e00: 0566 6c6f 6174 da06 666f 726d 6174 da09  .float..format..
+00001e10: 6672 6f7a 656e 7365 7472 4a00 0000 7248  frozensetrJ...rH
+00001e20: 0000 00da 0468 6173 68da 0368 6578 da02  .....hash..hex..
+00001e30: 6964 da03 696e 74da 0a69 7369 6e73 7461  id..int..isinsta
+00001e40: 6e63 65da 0a69 7373 7562 636c 6173 73da  nce..issubclass.
+00001e50: 0469 7465 72da 036c 656e da04 6c69 7374  .iter..len..list
+00001e60: da06 6c6f 6361 6c73 da03 6d61 70da 036d  ..locals..map..m
+00001e70: 6178 da0a 6d65 6d6f 7279 7669 6577 da03  ax..memoryview..
+00001e80: 6d69 6eda 046e 6578 74da 066f 626a 6563  min..next..objec
+00001e90: 74da 036f 6374 da03 6f72 64da 0370 6f77  t..oct..ord..pow
+00001ea0: da05 7261 6e67 65da 0472 6570 72da 0872  ..range..repr..r
+00001eb0: 6576 6572 7365 64da 0572 6f75 6e64 7224  eversed..roundr$
+00001ec0: 0000 00da 0573 6c69 6365 da06 736f 7274  .....slice..sort
+00001ed0: 6564 7240 0000 00da 0373 756d da05 7375  edr@.....sum..su
+00001ee0: 7065 7272 3500 0000 da04 7479 7065 da04  perr5.....type..
+00001ef0: 7661 7273 da03 7a69 70da 0546 616c 7365  vars..zip..False
+00001f00: da04 5472 7565 da08 456c 6c69 7073 6973  ..True..Ellipsis
+00001f10: da04 4e6f 6e65 da0f 4172 6974 686d 6574  ..None..Arithmet
+00001f20: 6963 4572 726f 72da 0e41 7373 6572 7469  icError..Asserti
+00001f30: 6f6e 4572 726f 72da 0e41 7474 7269 6275  onError..Attribu
+00001f40: 7465 4572 726f 72da 0d42 6173 6545 7863  teError..BaseExc
+00001f50: 6570 7469 6f6e da0f 426c 6f63 6b69 6e67  eption..Blocking
+00001f60: 494f 4572 726f 72da 0f42 726f 6b65 6e50  IOError..BrokenP
+00001f70: 6970 6545 7272 6f72 da0b 4275 6666 6572  ipeError..Buffer
+00001f80: 4572 726f 72da 0c42 7974 6573 5761 726e  Error..BytesWarn
+00001f90: 696e 67da 1143 6869 6c64 5072 6f63 6573  ing..ChildProces
+00001fa0: 7345 7272 6f72 da16 436f 6e6e 6563 7469  sError..Connecti
+00001fb0: 6f6e 4162 6f72 7465 6445 7272 6f72 da0f  onAbortedError..
+00001fc0: 436f 6e6e 6563 7469 6f6e 4572 726f 72da  ConnectionError.
+00001fd0: 1643 6f6e 6e65 6374 696f 6e52 6566 7573  .ConnectionRefus
+00001fe0: 6564 4572 726f 72da 1443 6f6e 6e65 6374  edError..Connect
+00001ff0: 696f 6e52 6573 6574 4572 726f 72da 1244  ionResetError..D
+00002000: 6570 7265 6361 7469 6f6e 5761 726e 696e  eprecationWarnin
+00002010: 67da 0845 4f46 4572 726f 72da 0f45 6e63  g..EOFError..Enc
+00002020: 6f64 696e 6757 6172 6e69 6e67 da10 456e  odingWarning..En
+00002030: 7669 726f 6e6d 656e 7445 7272 6f72 da09  vironmentError..
+00002040: 4578 6365 7074 696f 6eda 0f46 696c 6545  Exception..FileE
+00002050: 7869 7374 7345 7272 6f72 da11 4669 6c65  xistsError..File
+00002060: 4e6f 7446 6f75 6e64 4572 726f 72da 1246  NotFoundError..F
+00002070: 6c6f 6174 696e 6750 6f69 6e74 4572 726f  loatingPointErro
+00002080: 72da 0d46 7574 7572 6557 6172 6e69 6e67  r..FutureWarning
+00002090: da0d 4765 6e65 7261 746f 7245 7869 74da  ..GeneratorExit.
+000020a0: 0749 4f45 7272 6f72 da0b 496d 706f 7274  .IOError..Import
+000020b0: 4572 726f 72da 0d49 6d70 6f72 7457 6172  Error..ImportWar
+000020c0: 6e69 6e67 da10 496e 6465 6e74 6174 696f  ning..Indentatio
+000020d0: 6e45 7272 6f72 da0a 496e 6465 7845 7272  nError..IndexErr
+000020e0: 6f72 da10 496e 7465 7272 7570 7465 6445  or..InterruptedE
+000020f0: 7272 6f72 da11 4973 4144 6972 6563 746f  rror..IsADirecto
+00002100: 7279 4572 726f 72da 084b 6579 4572 726f  ryError..KeyErro
+00002110: 72da 114b 6579 626f 6172 6449 6e74 6572  r..KeyboardInter
+00002120: 7275 7074 da0b 4c6f 6f6b 7570 4572 726f  rupt..LookupErro
+00002130: 72da 0b4d 656d 6f72 7945 7272 6f72 da13  r..MemoryError..
+00002140: 4d6f 6475 6c65 4e6f 7446 6f75 6e64 4572  ModuleNotFoundEr
+00002150: 726f 72da 094e 616d 6545 7272 6f72 da12  ror..NameError..
+00002160: 4e6f 7441 4469 7265 6374 6f72 7945 7272  NotADirectoryErr
+00002170: 6f72 da0e 4e6f 7449 6d70 6c65 6d65 6e74  or..NotImplement
+00002180: 6564 da13 4e6f 7449 6d70 6c65 6d65 6e74  ed..NotImplement
+00002190: 6564 4572 726f 72da 074f 5345 7272 6f72  edError..OSError
+000021a0: da0d 4f76 6572 666c 6f77 4572 726f 72da  ..OverflowError.
+000021b0: 1950 656e 6469 6e67 4465 7072 6563 6174  .PendingDeprecat
+000021c0: 696f 6e57 6172 6e69 6e67 da0f 5065 726d  ionWarning..Perm
+000021d0: 6973 7369 6f6e 4572 726f 72da 1250 726f  issionError..Pro
+000021e0: 6365 7373 4c6f 6f6b 7570 4572 726f 72da  cessLookupError.
+000021f0: 0e52 6563 7572 7369 6f6e 4572 726f 72da  .RecursionError.
+00002200: 0e52 6566 6572 656e 6365 4572 726f 72da  .ReferenceError.
+00002210: 0f52 6573 6f75 7263 6557 6172 6e69 6e67  .ResourceWarning
+00002220: da0c 5275 6e74 696d 6545 7272 6f72 da0e  ..RuntimeError..
+00002230: 5275 6e74 696d 6557 6172 6e69 6e67 da12  RuntimeWarning..
+00002240: 5374 6f70 4173 796e 6349 7465 7261 7469  StopAsyncIterati
+00002250: 6f6e da0d 5374 6f70 4974 6572 6174 696f  on..StopIteratio
+00002260: 6eda 0b53 796e 7461 7845 7272 6f72 da0d  n..SyntaxError..
+00002270: 5379 6e74 6178 5761 726e 696e 67da 0b53  SyntaxWarning..S
+00002280: 7973 7465 6d45 7272 6f72 da0a 5379 7374  ystemError..Syst
+00002290: 656d 4578 6974 da08 5461 6245 7272 6f72  emExit..TabError
+000022a0: da0c 5469 6d65 6f75 7445 7272 6f72 da09  ..TimeoutError..
+000022b0: 5479 7065 4572 726f 72da 1155 6e62 6f75  TypeError..Unbou
+000022c0: 6e64 4c6f 6361 6c45 7272 6f72 da12 556e  ndLocalError..Un
+000022d0: 6963 6f64 6544 6563 6f64 6545 7272 6f72  icodeDecodeError
+000022e0: da12 556e 6963 6f64 6545 6e63 6f64 6545  ..UnicodeEncodeE
+000022f0: 7272 6f72 da0c 556e 6963 6f64 6545 7272  rror..UnicodeErr
+00002300: 6f72 da15 556e 6963 6f64 6554 7261 6e73  or..UnicodeTrans
+00002310: 6c61 7465 4572 726f 72da 0e55 6e69 636f  lateError..Unico
+00002320: 6465 5761 726e 696e 67da 0b55 7365 7257  deWarning..UserW
+00002330: 6172 6e69 6e67 da0a 5661 6c75 6545 7272  arning..ValueErr
+00002340: 6f72 da07 5761 726e 696e 67da 115a 6572  or..Warning..Zer
+00002350: 6f44 6976 6973 696f 6e45 7272 6f72 721e  oDivisionErrorr.
+00002360: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00002370: 0000 0000 0600 0000 4000 0000 7398 0000  ........@...s...
+00002380: 0065 005a 0164 005a 0255 0065 0365 0464  .e.Z.d.Z.U.e.e.d
+00002390: 013c 0065 0565 0665 0319 0019 0065 0464  .<.e.e.e.....e.d
+000023a0: 023c 0065 0765 0365 0866 0219 0065 0464  .<.e.e.e.f...e.d
+000023b0: 033c 0065 0965 0464 043c 0064 0565 0a6a  .<.e.e.d.<.d.e.j
+000023c0: 0b64 0665 0364 0765 0c66 0664 0864 0984  .d.e.d.e.f.d.d..
+000023d0: 045a 0d64 0a65 0e65 0365 0a6a 0f66 0219  .Z.d.e.e.e.j.f..
+000023e0: 0064 0765 0966 0464 0b64 0c84 045a 1064  .d.e.f.d.d...Z.d
+000023f0: 0a65 0364 0765 0966 0464 0d64 0e84 045a  .e.d.e.f.d.d...Z
+00002400: 1164 0565 0a6a 0b64 0764 0f66 0464 1064  .d.e.j.d.d.f.d.d
+00002410: 1184 045a 1264 0f53 0029 1272 2300 0000  ...Z.d.S.).r#...
+00002420: 7211 0000 0072 1000 0000 720e 0000 0072  r....r....r....r
+00002430: 0f00 0000 da04 6e6f 6465 da05 6572 726f  ......node..erro
+00002440: 7272 1200 0000 6303 0000 0000 0000 0000  rr....c.........
+00002450: 0000 0004 0000 0006 0000 0043 0000 0073  ...........C...s
+00002460: 4000 0000 7400 6a01 6401 6b05 7212 6402  @...t.j.d.k.r.d.
+00002470: 7c01 6a02 7c01 6a03 7c00 6a04 7c01 6a05  |.j.|.j.|.j.|.j.
+00002480: 7c01 6a06 6606 6e08 6402 7c01 6a02 7c01  |.j.f.n.d.|.j.|.
+00002490: 6a03 7c00 6a04 6604 7d03 7407 7c02 7c03  j.|.j.f.}.t.|.|.
+000024a0: 8302 8201 2903 4e69 0000 0a03 721b 0000  ....).Ni....r...
+000024b0: 0029 08da 0373 7973 da0a 6865 7876 6572  .)...sys..hexver
+000024c0: 7369 6f6e da06 6c69 6e65 6e6f da0a 636f  sion..lineno..co
+000024d0: 6c5f 6f66 6673 6574 7211 0000 00da 0a65  l_offsetr......e
+000024e0: 6e64 5f6c 696e 656e 6fda 0e65 6e64 5f63  nd_lineno..end_c
+000024f0: 6f6c 5f6f 6666 7365 7472 b400 0000 2904  ol_offsetr....).
+00002500: 7229 0000 0072 c500 0000 72c6 0000 00da  r)...r....r.....
+00002510: 0770 6179 6c6f 6164 7213 0000 0072 1300  .payloadr....r..
+00002520: 0000 7217 0000 00da 0466 6169 6c37 0100  ..r......fail7..
+00002530: 0073 1800 0000 080a 02f8 0201 0401 0401  .s..............
+00002540: 0401 0401 0401 04fa 1009 02f6 0a0c 7a17  ..............z.
+00002550: 5f56 616c 6964 6174 696f 6e43 6f6e 7465  _ValidationConte
+00002560: 7874 2e66 6169 6c72 3300 0000 6302 0000  xt.failr3...c...
+00002570: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00002580: 0043 0000 0073 3000 0000 7400 7c01 7401  .C...s0...t.|.t.
+00002590: 6a02 8302 7209 7c01 6a03 7d01 7c00 6a04  j...r.|.j.}.|.j.
+000025a0: 6400 7500 7017 7c01 7c00 6a04 7600 7017  d.u.p.|.|.j.v.p.
+000025b0: 7c01 7c00 6a05 7600 5300 7230 0000 0029  |.|.j.v.S.r0...)
+000025c0: 0672 6300 0000 7220 0000 00da 044e 616d  .rc...r .....Nam
+000025d0: 6572 6100 0000 7210 0000 0072 0e00 0000  era...r....r....
+000025e0: 723c 0000 0072 1300 0000 7213 0000 0072  r<...r....r....r
+000025f0: 1700 0000 da0d 6973 5f76 616c 6964 5f6e  ......is_valid_n
+00002600: 616d 6546 0100 0073 0800 0000 0c01 0601  ameF...s........
+00002610: 1c02 02ff 7a20 5f56 616c 6964 6174 696f  ....z _Validatio
+00002620: 6e43 6f6e 7465 7874 2e69 735f 7661 6c69  nContext.is_vali
+00002630: 645f 6e61 6d65 6302 0000 0000 0000 0000  d_namec.........
+00002640: 0000 0002 0000 0002 0000 0043 0000 0072  ...........C...r
+00002650: 3b00 0000 7230 0000 0029 0172 0e00 0000  ;...r0...).r....
+00002660: 723c 0000 0072 1300 0000 7213 0000 0072  r<...r....r....r
+00002670: 1700 0000 7231 0000 004d 0100 0073 0200  ....r1...M...s..
+00002680: 0000 0a01 7a24 5f56 616c 6964 6174 696f  ....z$_Validatio
+00002690: 6e43 6f6e 7465 7874 2e69 735f 7661 6c69  nContext.is_vali
+000026a0: 645f 6675 6e63 7469 6f6e 4e63 0200 0000  d_functionNc....
+000026b0: 0000 0000 0000 0000 0700 0000 0500 0000  ................
+000026c0: 4300 0000 739e 0000 0074 00a0 0174 027c  C...s....t...t.|
+000026d0: 0183 0174 03a1 027d 0264 017d 0374 047c  ...t...}.d.}.t.|
+000026e0: 0274 0583 0272 167c 00a0 067c 017c 02a1  .t...r.|...|.|..
+000026f0: 0201 006e 0974 077c 0283 0172 1f7c 027c  ...n.t.|...r.|.|
+00002700: 017c 0083 027d 037c 0373 4b74 08a0 097c  .|...}.|.sKt...|
+00002710: 01a1 0144 005d 265c 027d 047d 0574 047c  ...D.]&\.}.}.t.|
+00002720: 0574 0a83 0272 3f7c 0544 005d 187d 0674  .t...r?|.D.].}.t
+00002730: 047c 0674 086a 0b83 0272 3e7c 00a0 0c7c  .|.t.j...r>|...|
+00002740: 06a1 0101 0071 3174 047c 0574 086a 0b83  .....q1t.|.t.j..
+00002750: 0272 4a7c 00a0 0c7c 05a1 0101 0071 2664  .rJ|...|.....q&d
+00002760: 0253 0064 0253 0029 037a b656 616c 6964  .S.d.S.).z.Valid
+00002770: 6174 6520 7468 6520 7361 6665 7479 206f  ate the safety o
+00002780: 6620 616e 2041 5354 2e0a 0a20 2020 2020  f an AST...     
+00002790: 2020 2057 6520 646f 6e27 7420 7573 6520     We don't use 
+000027a0: 6173 742e 4e6f 6465 5669 7369 746f 7220  ast.NodeVisitor 
+000027b0: 6265 6361 7573 6520 6974 7320 7265 6375  because its recu
+000027c0: 7273 696f 6e20 6973 6e27 7420 7175 6974  rsion isn't quit
+000027d0: 6520 666c 6578 6962 6c65 2065 6e6f 7567  e flexible enoug
+000027e0: 6820 666f 7220 7573 2c0a 2020 2020 2020  h for us,.      
+000027f0: 2020 6275 7420 6974 2773 2061 2072 6561    but it's a rea
+00002800: 6c6c 7920 7369 6d70 6c65 2063 6c61 7373  lly simple class
+00002810: 2061 6e79 7761 792e 0a20 2020 2020 2020   anyway..       
+00002820: 2046 4e29 0dda 0848 414e 444c 4552 53da   FN)...HANDLERS.
+00002830: 0367 6574 727a 0000 00da 0d5f 756e 6b6e  .getrz....._unkn
+00002840: 6f77 6e5f 6e6f 6465 7263 0000 0072 4000  own_noderc...r@.
+00002850: 0000 72ce 0000 0072 5400 0000 7220 0000  ..r....rT...r ..
+00002860: 00da 0b69 7465 725f 6669 656c 6473 7267  ...iter_fieldsrg
+00002870: 0000 0072 4300 0000 7225 0000 0029 0772  ...rC...r%...).r
+00002880: 2900 0000 72c5 0000 00da 026f 705a 1061  )...r......opZ.a
+00002890: 6c72 6561 6479 5f72 6563 7572 7365 64da  lready_recursed.
+000028a0: 0566 6965 6c64 da05 7661 6c75 65da 0469  .field..value..i
+000028b0: 7465 6d72 1300 0000 7213 0000 0072 1700  temr....r....r..
+000028c0: 0000 7225 0000 0050 0100 0073 2400 0000  ..r%...P...s$...
+000028d0: 1006 0401 0a01 0e01 0801 0a01 0402 1201  ................
+000028e0: 0a01 0801 0c01 0a01 0280 0c01 0a01 0280  ................
+000028f0: 04f9 0401 7a1b 5f56 616c 6964 6174 696f  ....z._Validatio
+00002900: 6e43 6f6e 7465 7874 2e76 616c 6964 6174  nContext.validat
+00002910: 6529 1372 1400 0000 723d 0000 0072 3e00  e).r....r=...r>.
+00002920: 0000 7240 0000 00da 0f5f 5f61 6e6e 6f74  ..r@.....__annot
+00002930: 6174 696f 6e73 5f5f 7208 0000 0072 0900  ations__r....r..
+00002940: 0000 7204 0000 0072 0300 0000 7241 0000  ..r....r....rA..
+00002950: 0072 2000 0000 7243 0000 0072 0700 0000  .r ...rC...r....
+00002960: 72ce 0000 0072 0c00 0000 72cf 0000 0072  r....r....r....r
+00002970: d000 0000 7231 0000 0072 2500 0000 7213  ....r1...r%...r.
+00002980: 0000 0072 1300 0000 7213 0000 0072 1700  ...r....r....r..
+00002990: 0000 7223 0000 0031 0100 0073 1200 0000  ..r#...1...s....
+000029a0: 0a00 0801 1001 1001 0801 1802 1c0f 1207  ................
+000029b0: 1803 7223 0000 0072 c500 0000 722a 0000  ..r#...r....r*..
+000029c0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+000029d0: 0000 0600 0000 4300 0000 7358 0000 0074  ......C...sX...t
+000029e0: 007c 0074 016a 0283 0273 084a 0082 017c  .|.t.j...s.J...|
+000029f0: 01a0 037c 00a1 0173 187c 01a0 047c 0064  ...|...s.|...|.d
+00002a00: 017c 006a 059b 0064 029d 03a1 0201 0074  .|.j...d.......t
+00002a10: 007c 006a 0674 016a 0783 0273 2a7c 01a0  .|.j.t.j...s*|..
+00002a20: 047c 0064 037c 006a 059b 0064 029d 03a1  .|.d.|.j...d....
+00002a30: 0201 0064 0453 0029 054e 7a1f 5265 6665  ...d.S.).Nz.Refe
+00002a40: 7265 6e63 6520 746f 2075 6e6b 6e6f 776e  rence to unknown
+00002a50: 2076 6172 6961 626c 6520 22fa 0122 7a20   variable ".."z 
+00002a60: 4174 7465 6d70 7420 746f 206d 7574 6174  Attempt to mutat
+00002a70: 6520 7468 6520 7661 7269 6162 6c65 2022  e the variable "
+00002a80: 4629 0872 6300 0000 7220 0000 0072 cf00  F).rc...r ...r..
+00002a90: 0000 72d0 0000 0072 ce00 0000 7261 0000  ..r....r....ra..
+00002aa0: 00da 0363 7478 da04 4c6f 6164 a902 72c5  ...ctx..Load..r.
+00002ab0: 0000 0072 2a00 0000 7213 0000 0072 1300  ...r*...r....r..
+00002ac0: 0000 7217 0000 00da 0e5f 7661 6c69 6461  ..r......_valida
+00002ad0: 7465 5f6e 616d 6567 0100 0073 0c00 0000  te_nameg...s....
+00002ae0: 1001 0a01 1601 0e01 1601 0401 72de 0000  ............r...
+00002af0: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00002b00: 0000 0600 0000 4300 0000 73ce 0000 0074  ......C...s....t
+00002b10: 007c 0074 016a 0283 0273 084a 0082 0174  .|.t.j...s.J...t
+00002b20: 007c 006a 0374 016a 0483 0272 247c 01a0  .|.j.t.j...r$|..
+00002b30: 057c 006a 036a 06a1 0173 227c 01a0 077c  .|.j.j...s"|...|
+00002b40: 0064 017c 006a 036a 069b 0064 029d 03a1  .d.|.j.j...d....
+00002b50: 0201 0064 0853 0074 007c 006a 0374 016a  ...d.S.t.|.j.t.j
+00002b60: 0883 0272 5f74 007c 006a 036a 0974 016a  ...r_t.|.j.j.t.j
+00002b70: 0483 0273 397c 01a0 077c 0064 03a1 0201  ...s9|...|.d....
+00002b80: 007c 01a0 0a7c 006a 036a 09a1 0173 4d7c  .|...|.j.j...sM|
+00002b90: 01a0 077c 0064 047c 006a 036a 096a 069b  ...|.d.|.j.j.j..
+00002ba0: 0064 029d 03a1 0201 007c 016a 0b73 5d7c  .d.......|.j.s]|
+00002bb0: 01a0 077c 0064 057c 006a 036a 096a 069b  ...|.d.|.j.j.j..
+00002bc0: 0064 069d 03a1 0201 0064 0853 007c 01a0  .d.......d.S.|..
+00002bd0: 077c 0064 07a1 0201 0064 0853 0029 094e  .|.d.....d.S.).N
+00002be0: 7a22 4174 7465 6d70 7420 746f 2063 616c  z"Attempt to cal
+00002bf0: 6c20 756e 6b6e 6f77 6e20 6675 6e63 7469  l unknown functi
+00002c00: 6f6e 2022 72da 0000 007a 3253 7472 616e  on "r....z2Stran
+00002c10: 6765 2061 7474 7269 6275 7465 3b20 7768  ge attribute; wh
+00002c20: 6174 2773 2069 7473 206e 616d 653f 204e  at's its name? N
+00002c30: 6576 6572 2068 6170 7065 6e73 2e7a 2e41  ever happens.z.A
+00002c40: 7474 656d 7074 2074 6f20 6361 6c6c 2066  ttempt to call f
+00002c50: 756e 6374 696f 6e20 696e 2075 6e6b 6e6f  unction in unkno
+00002c60: 776e 2076 6172 6961 626c 6520 227a 1b41  wn variable "z.A
+00002c70: 7474 656d 7074 2074 6f20 6361 6c6c 206d  ttempt to call m
+00002c80: 6574 686f 6420 6f66 2022 7a41 2220 6275  ethod of "zA" bu
+00002c90: 7420 6361 6c6c 696e 6720 6d65 7468 6f64  t calling method
+00002ca0: 7320 6f66 2076 6172 6961 626c 6573 2068  s of variables h
+00002cb0: 6173 2062 6565 6e20 6578 706c 6963 6974  as been explicit
+00002cc0: 6c79 2066 6f72 6269 6464 656e 2e7a 4441  ly forbidden.zDA
+00002cd0: 7474 656d 7074 6564 2074 6f20 6361 6c6c  ttempted to call
+00002ce0: 2073 6f6d 6574 6869 6e67 2074 6861 7420   something that 
+00002cf0: 6973 206e 6569 7468 6572 2061 206e 616d  is neither a nam
+00002d00: 6520 6e6f 7220 616e 2061 7474 7269 6275  e nor an attribu
+00002d10: 7465 2e46 290c 7263 0000 0072 2000 0000  te.F).rc...r ...
+00002d20: da04 4361 6c6c da04 6675 6e63 72cf 0000  ..Call..funcr...
+00002d30: 0072 3100 0000 7261 0000 0072 ce00 0000  .r1...ra...r....
+00002d40: da09 4174 7472 6962 7574 6572 d700 0000  ..Attributer....
+00002d50: 72d0 0000 0072 0f00 0000 72dd 0000 0072  r....r....r....r
+00002d60: 1300 0000 7213 0000 0072 1700 0000 da0e  ....r....r......
+00002d70: 5f76 616c 6964 6174 655f 6361 6c6c 7001  _validate_callp.
+00002d80: 0000 732e 0000 0010 010e 010e 0118 0104  ..s.............
+00002d90: 140e ed10 010c 010e 0104 0102 0110 0104  ................
+00002da0: fe06 0404 0102 0110 0104 fe04 0a04 fc04  ................
+00002db0: 0104 ff04 0472 e200 0000 6302 0000 0000  .....r....c.....
+00002dc0: 0000 0000 0000 0006 0000 000a 0000 0043  ...............C
+00002dd0: 0000 0073 6c01 0000 7400 7c00 6401 8302  ...sl...t.|.d...
+00002de0: 7311 7c01 a001 7c00 6402 7402 7c00 8301  s.|...|.d.t.|...
+00002df0: 9b00 6403 9d03 a102 0100 6700 7d02 7c00  ..d.......g.}.|.
+00002e00: 6a03 4400 5d36 7d03 7404 7c03 6a05 7406  j.D.]6}.t.|.j.t.
+00002e10: 6a07 8302 7227 7404 7c03 6a05 6a08 7406  j...r't.|.j.j.t.
+00002e20: 6a09 8302 732d 7c01 a001 7c00 6404 a102  j...s-|...|.d...
+00002e30: 0100 7c01 6a0a 6400 7501 7245 7c03 6a05  ..|.j.d.u.rE|.j.
+00002e40: 6a0b 7c01 6a0a 7600 7245 7c01 a001 7c00  j.|.j.v.rE|...|.
+00002e50: 6405 7c03 6a05 6a0b 9b00 6406 9d03 a102  d.|.j.j...d.....
+00002e60: 0100 7c02 a00c 7c03 6a05 6a0b a101 0100  ..|...|.j.j.....
+00002e70: 7116 7a56 7c01 6a0a 6400 7501 7259 7c01  q.zV|.j.d.u.rY|.
+00002e80: 6a0a a00d 7c02 a101 0100 7c00 6a03 4400  j...|.....|.j.D.
+00002e90: 5d13 7d03 7c01 a00e 7c03 6a0f a101 0100  ].}.|...|.j.....
+00002ea0: 7c03 6a10 4400 5d07 7d04 7c01 a00e 7c04  |.j.D.].}.|...|.
+00002eb0: a101 0100 7167 715c 7400 7c00 6407 8302  ....qgq\t.|.d...
+00002ec0: 727b 7c01 a00e 7c00 6a11 a101 0100 7400  r{|...|.j.....t.
+00002ed0: 7c00 6408 8302 7286 7c01 a00e 7c00 6a12  |.d...r.|...|.j.
+00002ee0: a101 0100 7400 7c00 6409 8302 7291 7c01  ....t.|.d...r.|.
+00002ef0: a00e 7c00 6a13 a101 0100 5700 7c01 6a0a  ..|.j.....W.|.j.
+00002f00: 6400 7501 72a2 7c02 4400 5d08 7d05 7c01  d.u.r.|.D.].}.|.
+00002f10: 6a0a a014 7c05 a101 0100 7199 640a 5300  j...|.....q.d.S.
+00002f20: 7c01 6a0a 6400 7501 72b4 7c02 4400 5d09  |.j.d.u.r.|.D.].
+00002f30: 7d05 7c01 6a0a a014 7c05 a101 0100 71ab  }.|.j...|.....q.
+00002f40: 7700 7700 290b 4eda 0a67 656e 6572 6174  w.w.).N..generat
+00002f50: 6f72 737a 0e45 6e63 6f75 6e74 6572 6564  orsz.Encountered
+00002f60: 2061 207a 1520 7769 7468 206e 6f20 6765   a z. with no ge
+00002f70: 6e65 7261 746f 7273 3f3f 7a1c 496e 7661  nerators??z.Inva
+00002f80: 6c69 6420 6765 6e65 7261 746f 7220 6578  lid generator ex
+00002f90: 7072 6573 7369 6f6e 7a1c 5468 6520 636f  pressionz.The co
+00002fa0: 6d70 7265 6865 6e73 696f 6e20 7661 7269  mprehension vari
+00002fb0: 6162 6c65 2022 7a17 2220 6d61 736b 7320  able "z." masks 
+00002fc0: 6120 7661 7269 6162 6c65 206e 616d 65da  a variable name.
+00002fd0: 0365 6c74 da03 6b65 7972 d700 0000 5429  .elt..keyr....T)
+00002fe0: 1572 4800 0000 72ce 0000 0072 7a00 0000  .rH...r....rz...
+00002ff0: 72e3 0000 0072 6300 0000 da06 7461 7267  r....rc.....targ
+00003000: 6574 7220 0000 0072 cf00 0000 72db 0000  etr ...r....r...
+00003010: 00da 0553 746f 7265 7210 0000 0072 6100  ...Storer....ra.
+00003020: 0000 da06 6170 7065 6e64 7246 0000 0072  ....appendrF...r
+00003030: 2500 0000 7265 0000 00da 0369 6673 72e4  %...re.....ifsr.
+00003040: 0000 0072 e500 0000 72d7 0000 00da 0764  ...r....r......d
+00003050: 6973 6361 7264 2906 72c5 0000 0072 2a00  iscard).r....r*.
+00003060: 0000 5a0b 6368 696c 645f 6e61 6d65 73da  ..Z.child_names.
+00003070: 0967 656e 6572 6174 6f72 da09 636f 6e64  .generator..cond
+00003080: 6974 696f 6e5a 0a63 6869 6c64 5f6e 616d  itionZ.child_nam
+00003090: 6572 1300 0000 7213 0000 0072 1700 0000  er....r....r....
+000030a0: da17 5f76 616c 6964 6174 655f 636f 6d70  .._validate_comp
+000030b0: 7265 6865 6e73 696f 6e8b 0100 0073 4c00  rehension....sL.
+000030c0: 0000 0a01 1801 0403 0a01 1001 0a01 04ff  ................
+000030d0: 0c03 1801 0401 0201 0e01 04fe 1004 0203  ................
+000030e0: 0a01 0c01 0a02 0c01 0a01 0c01 02ff 0a02  ................
+000030f0: 0c01 0a01 0c01 0a01 0c01 0280 0a03 0801  ................
+00003100: 0e01 0402 0afc 0801 0e01 02fe 0201 72ed  ..............r.
+00003110: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+00003120: 0200 0000 0600 0000 4300 0000 731c 0000  ........C...s...
+00003130: 007c 01a0 007c 0064 0174 017c 0083 019b  .|...|.d.t.|....
+00003140: 0064 029d 03a1 0201 0064 0353 0029 044e  .d.......d.S.).N
+00003150: 7a13 4f70 6572 6174 696f 6e73 206f 6620  z.Operations of 
+00003160: 7479 7065 207a 2220 6172 6520 6e6f 7420  type z" are not 
+00003170: 7375 7070 6f72 7465 6420 696e 2045 7870  supported in Exp
+00003180: 7265 7373 696f 6e73 2e46 2902 72ce 0000  ressions.F).r...
+00003190: 0072 7a00 0000 72dd 0000 0072 1300 0000  .rz...r....r....
+000031a0: 7213 0000 0072 1700 0000 72d3 0000 00b5  r....r....r.....
+000031b0: 0100 0073 0800 0000 0401 1001 04ff 0403  ...s............
+000031c0: 72d3 0000 0072 d100 0000 7233 0000 00da  r....r....r3....
+000031d0: 0661 6374 696f 6e63 0200 0000 0000 0000  .actionc........
+000031e0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
+000031f0: 7320 0000 0074 0074 017c 0083 0272 0e7c  s ...t.t.|...r.|
+00003200: 0174 0274 0374 017c 0083 023c 0064 0153  .t.t.t.|...<.d.S
+00003210: 0064 0153 0029 0261 f602 0000 4465 6669  .d.S.).a....Defi
+00003220: 6e65 2077 6861 7420 7765 2064 6f20 7768  ne what we do wh
+00003230: 656e 2077 6520 7365 6520 6120 6e6f 6465  en we see a node
+00003240: 206f 6620 6120 6769 7665 6e20 7479 7065   of a given type
+00003250: 2e20 5468 6973 2066 756e 6374 696f 6e20  . This function 
+00003260: 6973 2068 6572 6520 736f 2074 6861 7420  is here so that 
+00003270: 7765 0a20 2020 2063 616e 2068 616e 646c  we.    can handl
+00003280: 6520 6469 6666 6572 656e 7420 5079 7468  e different Pyth
+00003290: 6f6e 2076 6572 7369 6f6e 7320 7768 6963  on versions whic
+000032a0: 6820 6861 7665 2064 6966 6665 7265 6e74  h have different
+000032b0: 2041 5354 2074 7970 6573 2e20 4e6f 7465   AST types. Note
+000032c0: 2074 6861 7420 7468 6973 2069 7320 626f   that this is bo
+000032d0: 7468 0a20 2020 2061 2070 6f73 6974 6976  th.    a positiv
+000032e0: 6520 616e 6420 6e65 6761 7469 7665 206c  e and negative l
+000032f0: 6973 7420 666f 7220 7365 6375 7269 7479  ist for security
+00003300: 2072 6561 736f 6e73 2120 556e 6b6e 6f77   reasons! Unknow
+00003310: 6e20 6e6f 6465 2074 7970 6573 2061 7265  n node types are
+00003320: 202a 6572 726f 7273 2a20 6279 0a20 2020   *errors* by.   
+00003330: 2064 6566 6175 6c74 2075 6e74 696c 2077   default until w
+00003340: 6520 6361 6e20 6d61 6e75 616c 6c79 2073  e can manually s
+00003350: 6179 2074 6861 7420 7468 6579 2772 6520  ay that they're 
+00003360: 6b6f 7368 6572 2e0a 0a20 2020 2054 6865  kosher...    The
+00003370: 2061 6374 696f 6e73 2061 7265 3a0a 2020   actions are:.  
+00003380: 2020 2020 2020 4e6f 6e65 202d 2d20 7468        None -- th
+00003390: 6973 206e 6f64 6520 6973 2066 696e 650a  is node is fine.
+000033a0: 2020 2020 2020 2020 7374 7220 2d2d 2074          str -- t
+000033b0: 6869 7320 6e6f 6465 2069 7320 616c 7761  his node is alwa
+000033c0: 7973 2061 6e20 6572 726f 720a 2020 2020  ys an error.    
+000033d0: 2020 2020 6675 6e63 7469 6f6e 202d 2d20      function -- 
+000033e0: 6361 6c6c 2074 6869 7320 7768 656e 2079  call this when y
+000033f0: 6f75 2066 696e 6420 7375 6368 2061 206e  ou find such a n
+00003400: 6f64 652e 2054 6865 2061 7267 756d 656e  ode. The argumen
+00003410: 7473 2061 7265 2074 6865 2041 5354 206e  ts are the AST n
+00003420: 6f64 6520 616e 6420 7468 650a 2020 2020  ode and the.    
+00003430: 2020 2020 2020 2020 5f56 616c 6964 6174          _Validat
+00003440: 696f 6e43 6f6e 7465 7874 3b20 7468 6520  ionContext; the 
+00003450: 7265 7475 726e 2076 616c 7565 2073 686f  return value sho
+00003460: 756c 6420 6265 2066 616c 7365 2074 6f20  uld be false to 
+00003470: 616c 6c6f 7720 7468 6520 7363 616e 6e65  allow the scanne
+00003480: 7220 746f 2072 6563 7572 7365 0a20 2020  r to recurse.   
+00003490: 2020 2020 2020 2020 2074 6872 6f75 6768           through
+000034a0: 2061 6c6c 2074 6865 206e 6f64 6527 7320   all the node's 
+000034b0: 6368 696c 6472 656e 2061 7320 7573 7561  children as usua
+000034c0: 6c2c 206f 7220 7472 7565 2069 6620 7468  l, or true if th
+000034d0: 6520 6675 6e63 7469 6f6e 2068 6173 2061  e function has a
+000034e0: 6c72 6561 6479 2074 616b 656e 0a20 2020  lready taken.   
+000034f0: 2020 2020 2020 2020 2063 6172 6520 6f66           care of
+00003500: 2074 6861 7420 6974 7365 6c66 2e0a 2020   that itself..  
+00003510: 2020 4e29 0472 4800 0000 7220 0000 0072    N).rH...r ...r
+00003520: d100 0000 724a 0000 0029 0272 3300 0000  ....rJ...).r3...
+00003530: 72ee 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00003540: 1700 0000 da03 5f6f 6ec3 0100 0073 0600  ......_on....s..
+00003550: 0000 0a0e 1201 04ff 72ef 0000 007a 3356  ........r....z3V
+00003560: 6172 6961 626c 6520 6173 7369 676e 6d65  ariable assignme
+00003570: 6e74 2069 7320 6e6f 7420 7065 726d 6974  nt is not permit
+00003580: 7465 6420 696e 2065 7870 7265 7373 696f  ted in expressio
+00003590: 6e73 7a31 5661 7269 6162 6c65 2064 656c  nsz1Variable del
+000035a0: 6574 696f 6e20 6973 206e 6f74 2070 6572  etion is not per
+000035b0: 6d69 7474 6564 2069 6e20 6578 7072 6573  mitted in expres
+000035c0: 7369 6f6e 737a 4944 6563 6c61 7269 756e  sionszIDeclariun
+000035d0: 6720 6f62 6a65 6374 732c 2063 6c61 7373  g objects, class
+000035e0: 6573 2c20 6f72 2066 756e 6374 696f 6e73  es, or functions
+000035f0: 2069 7320 6e6f 7420 7065 726d 6974 7465   is not permitte
+00003600: 6420 696e 2065 7870 7265 7373 696f 6e73  d in expressions
+00003610: 7a31 496d 706f 7274 696e 6720 6f62 6a65  z1Importing obje
+00003620: 6374 7320 6973 206e 6f74 2070 6572 6d69  cts is not permi
+00003630: 7474 6564 2069 6e20 6578 7072 6573 7369  tted in expressi
+00003640: 6f6e 737a 3843 6f6e 7472 6f6c 2066 6c6f  onsz8Control flo
+00003650: 7720 6f70 6572 6174 696f 6e73 2061 7265  w operations are
+00003660: 206e 6f74 2070 6572 6d69 7474 6564 2069   not permitted i
+00003670: 6e20 6578 7072 6573 7369 6f6e 73da 064d  n expressions..M
+00003680: 6f64 756c 65da 0c46 756e 6374 696f 6e54  odule..FunctionT
+00003690: 7970 65da 0b49 6e74 6572 6163 7469 7665  ype..Interactive
+000036a0: da08 436f 6e73 7461 6e74 da0e 466f 726d  ..Constant..Form
+000036b0: 6174 7465 6456 616c 7565 da09 4a6f 696e  attedValue..Join
+000036c0: 6564 5374 7272 0500 0000 720a 0000 0072  edStrr....r....r
+000036d0: 0900 0000 7204 0000 0072 cf00 0000 72dc  ....r....r....r.
+000036e0: 0000 0072 e700 0000 da03 4465 6cda 0753  ...r......Del..S
+000036f0: 7461 7272 6564 da04 4578 7072 da07 556e  tarred..Expr..Un
+00003700: 6172 794f 70da 0455 4164 64da 0455 5375  aryOp..UAdd..USu
+00003710: 62da 034e 6f74 da06 496e 7665 7274 da05  b..Not..Invert..
+00003720: 4269 6e4f 70da 0341 6464 da03 5375 62da  BinOp..Add..Sub.
+00003730: 044d 756c 74da 0344 6976 da08 466c 6f6f  .Mult..Div..Floo
+00003740: 7244 6976 da03 4d6f 64da 0350 6f77 da06  rDiv..Mod..Pow..
+00003750: 4c53 6869 6674 da06 5253 6869 6674 da05  LShift..RShift..
+00003760: 4269 744f 72da 0642 6974 586f 72da 0642  BitOr..BitXor..B
+00003770: 6974 416e 64da 074d 6174 4d75 6c74 da06  itAnd..MatMult..
+00003780: 426f 6f6c 4f70 da03 416e 64da 024f 72da  BoolOp..And..Or.
+00003790: 0743 6f6d 7061 7265 da02 4571 da05 4e6f  .Compare..Eq..No
+000037a0: 7445 71da 024c 74da 034c 7445 da02 4774  tEq..Lt..LtE..Gt
+000037b0: da03 4774 45da 0249 73da 0549 734e 6f74  ..GtE..Is..IsNot
+000037c0: da01 6eda 054e 6f74 496e 72df 0000 00da  ..n..NotInr.....
+000037d0: 076b 6579 776f 7264 da05 4966 4578 7072  .keyword..IfExpr
+000037e0: e100 0000 da09 4e61 6d65 6445 7870 72da  ......NamedExpr.
+000037f0: 0953 7562 7363 7269 7074 da05 536c 6963  .Subscript..Slic
+00003800: 65da 084c 6973 7443 6f6d 70da 0753 6574  e..ListComp..Set
+00003810: 436f 6d70 da0c 4765 6e65 7261 746f 7245  Comp..GeneratorE
+00003820: 7870 da08 4469 6374 436f 6d70 da0d 636f  xp..DictComp..co
+00003830: 6d70 7265 6865 6e73 696f 6eda 0641 7373  mprehension..Ass
+00003840: 6967 6eda 0941 6e6e 4173 7369 676e da09  ign..AnnAssign..
+00003850: 4175 6741 7373 6967 6eda 0552 6169 7365  AugAssign..Raise
+00003860: da06 4173 7365 7274 da06 4465 6c65 7465  ..Assert..Delete
+00003870: da04 5061 7373 da06 496d 706f 7274 da0a  ..Pass..Import..
+00003880: 496d 706f 7274 4672 6f6d da05 616c 6961  ImportFrom..alia
+00003890: 73da 0249 66da 0346 6f72 da05 5768 696c  s..If..For..Whil
+000038a0: 65da 0542 7265 616b da08 436f 6e74 696e  e..Break..Contin
+000038b0: 7565 da03 5472 795a 0754 7279 5374 6172  ue..TryZ.TryStar
+000038c0: da0d 4578 6365 7074 4861 6e64 6c65 72da  ..ExceptHandler.
+000038d0: 0457 6974 68da 0877 6974 6869 7465 6dda  .With..withitem.
+000038e0: 054d 6174 6368 da0a 6d61 7463 685f 6361  .Match..match_ca
+000038f0: 7365 da0a 4d61 7463 6856 616c 7565 da0e  se..MatchValue..
+00003900: 4d61 7463 6853 696e 676c 6574 6f6e da0d  MatchSingleton..
+00003910: 4d61 7463 6853 6571 7565 6e63 65da 094d  MatchSequence..M
+00003920: 6174 6368 5374 6172 da0c 4d61 7463 684d  atchStar..MatchM
+00003930: 6170 7069 6e67 da0a 4d61 7463 6843 6c61  apping..MatchCla
+00003940: 7373 da07 4d61 7463 6841 73da 074d 6174  ss..MatchAs..Mat
+00003950: 6368 4f72 da0b 4675 6e63 7469 6f6e 4465  chOr..FunctionDe
+00003960: 66da 064c 616d 6264 61da 0961 7267 756d  f..Lambda..argum
+00003970: 656e 7473 da03 6172 67da 0652 6574 7572  ents..arg..Retur
+00003980: 6eda 0559 6965 6c64 da09 5969 656c 6446  n..Yield..YieldF
+00003990: 726f 6dda 0647 6c6f 6261 6c7a 3a4d 6f64  rom..Globalz:Mod
+000039a0: 6966 7969 6e67 2067 6c6f 6261 6c20 7661  ifying global va
+000039b0: 7269 6162 6c65 7320 6973 206e 6f74 2070  riables is not p
+000039c0: 6572 6d69 7474 6564 2069 6e20 6578 7072  ermitted in expr
+000039d0: 6573 7369 6f6e 73da 084e 6f6e 6c6f 6361  essions..Nonloca
+000039e0: 6c7a 3c4d 6f64 6966 7969 6e67 206e 6f6e  lz<Modifying non
+000039f0: 6c6f 6361 6c20 7661 7269 6162 6c65 7320  local variables 
+00003a00: 6973 206e 6f74 2070 6572 6d69 7474 6564  is not permitted
+00003a10: 2069 6e20 6578 7072 6573 7369 6f6e 73da   in expressions.
+00003a20: 0843 6c61 7373 4465 66da 1041 7379 6e63  .ClassDef..Async
+00003a30: 4675 6e63 7469 6f6e 4465 66da 0541 7761  FunctionDef..Awa
+00003a40: 6974 da08 4173 796e 6346 6f72 da09 4173  it..AsyncFor..As
+00003a50: 796e 6357 6974 6829 2672 3f00 0000 7220  yncWith)&r?...r 
+00003a60: 0000 0072 4900 0000 72c7 0000 00da 0674  ...rI...r......t
+00003a70: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
+00003a80: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
+00003a90: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00003aa0: 0000 720b 0000 0072 0c00 0000 726e 0000  ..r....r....rn..
+00003ab0: 0072 0d00 0000 7257 0000 0072 1d00 0000  .r....rW...r....
+00003ac0: 721e 0000 0072 4000 0000 72d9 0000 0072  r....r@...r....r
+00003ad0: 2300 0000 7243 0000 0072 4100 0000 72de  #...rC...rA...r.
+00003ae0: 0000 0072 e200 0000 72ed 0000 0072 d300  ...r....r....r..
+00003af0: 0000 5a07 5f41 4354 494f 4e72 d100 0000  ..Z._ACTIONr....
+00003b00: 72ef 0000 005a 094e 4f5f 4153 5349 474e  r....Z.NO_ASSIGN
+00003b10: 5a09 4e4f 5f44 454c 4554 455a 0a4e 4f5f  Z.NO_DELETEZ.NO_
+00003b20: 4445 434c 4152 455a 094e 4f5f 494d 504f  DECLAREZ.NO_IMPO
+00003b30: 5254 5a0a 4e4f 5f43 4f4e 5452 4f4c 7213  RTZ.NO_CONTROLr.
+00003b40: 0000 0072 1300 0000 7213 0000 0072 1700  ...r....r....r..
+00003b50: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00003b60: 7304 0100 0006 0008 0208 0108 0134 0110  s............4..
+00003b70: 0f12 6e06 2402 0216 fe00 7f10 0b18 3618  ..n.$.........6.
+00003b80: 0918 1b18 2a1c 0a1a 0116 0304 1204 0104  ....*...........
+00003b90: 0104 0104 010a 020a 010a 010a 010a 010a  ................
+00003ba0: 010a 010a 010a 010a 010a 010a 010a 020a  ................
+00003bb0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
+00003bc0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003bd0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003be0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003bf0: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003c00: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003c10: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003c20: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003c30: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003c40: 010a 010a 010a 010a 010a 010a 010a 010a  ................
 00003c50: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00003c60: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00003c70: 010a 010a 010a 010a 010a 010a 010a 010a  ................
-00003c80: 010a 010a 010e 01                        .......
+00003c60: 010a 010a 010a 010e 01                   .........
```

## tests/base/__pycache__/cache_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Sep  7 18:15:49 2022 UTC, .py size: 4979 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d5df 1863 7313 0000  o..........cs...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 7313 0000  o.......!.vcs...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 a200 0000 5500  .....@...s....U.
 00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
 00000040: 6400 6402 6c02 6d03 5a03 6d04 5a04 0100  d.d.l.m.Z.m.Z...
 00000050: 6400 6403 6c05 6d06 5a06 6d07 5a07 0100  d.d.l.m.Z.m.Z...
 00000060: 6500 a008 a100 5a09 6900 5a0a 6504 650b  e.....Z.i.Z.e.e.
 00000070: 6503 6602 1900 650c 6404 3c00 4700 6405  e.f...e.d.<.G.d.
```

## tests/base/__pycache__/flex_decorator_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Sep  7 18:14:42 2022 UTC, .py size: 1851 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 92df 1863 3b07 0000  o..........c;...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 3b07 0000  o.......!.vc;...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6500 6a07 8303 5a08 6401 5300 2906 e900  e.j...Z.d.S.)...
 00000070: 0000 004e 2903 da03 416e 79da 0843 616c  ...N)...Any..Cal
```

## tests/containers/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 20 22:59:42 2022 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 defb b062 0000 0000  o..........b....
+00000000: 6f0d 0d0a 0000 0000 d901 7763 0000 0000  o.........wc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa3f 6275 696c 642f 6264  .r.....?build/bd
 00000050: 6973 742e 6d61 636f 7378 2d31 322e 342d  ist.macosx-12.4-
 00000060: 7838 365f 3634 2f65 6767 2f74 6573 7473  x86_64/egg/tests
 00000070: 2f63 6f6e 7461 696e 6572 732f 5f5f 696e  /containers/__in
```

## tests/file/__pycache__/dev_null_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Sep 12 00:17:28 2022 UTC, .py size: 424 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 987a 1e63 a801 0000  o........z.c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 a801 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6500 6a04 8303 5a05 6401 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 004e 2902 da0a 5261 7744 6576 4e75  ...N)...RawDevNu
 00000070: 6c6c da0b 5465 7874 4465 764e 756c 6c63  ll..TextDevNullc
```

## tests/file/__pycache__/tee_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Sep 12 00:16:52 2022 UTC, .py size: 394 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 747a 1e63 8a01 0000  o.......tz.c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 8a01 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 4700 6403 6404  d.l.m.Z...G.d.d.
 00000050: 8400 6404 6501 6a04 8303 5a05 6401 5300  ..d.e.j...Z.d.S.
 00000060: 2905 e900 0000 004e 2901 da03 7465 6563  )......N)...teec
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

## tests/iterators/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Sep 28 23:47:16 2022 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 04dd 3463 0000 0000  o.........4c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 0000 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa3e 6275 696c 642f 6264  .r.....>build/bd
 00000050: 6973 742e 6d61 636f 7378 2d31 322e 342d  ist.macosx-12.4-
 00000060: 7838 365f 3634 2f65 6767 2f74 6573 7473  x86_64/egg/tests
 00000070: 2f69 7465 7261 746f 7273 2f5f 5f69 6e69  /iterators/__ini
```

## tests/iterators/__pycache__/iterators_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 21:53:26 2022 UTC, .py size: 1777 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5665 3763 f106 0000  o.......Ve7c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 f106 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6405 6c08 6d09 5a09 0100 6400 6406 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
```

## tests/iterators/__pycache__/zip_by_key_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Sep 29 19:54:28 2022 UTC, .py size: 6293 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f4f7 3563 9518 0000  o.........5c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 9518 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6500 6a04 8303 5a05 6506 6405 6b02 721f  e.j...Z.e.d.k.r.
 00000060: 6500 a007 a100 0100 6401 5300 6401 5300  e.......d.S.d.S.
 00000070: 2906 e900 0000 004e 2902 da09 5a69 7053  )......N)...ZipS
```

## tests/os/__pycache__/list_files_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jul 23 00:15:23 2022 UTC, .py size: 2166 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9b3d db62 7608 0000  o........=.bv...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 7608 0000  o.......!.vcv...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6501 6a06 8303 5a07 6508 6406 6b02 7227  e.j...Z.e.d.k.r'
 00000070: 6501 a009 a100 0100 6401 5300 6401 5300  e.......d.S.d.S.
```

## tests/testing/__pycache__/trace_on_failure_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Sep  7 18:18:12 2022 UTC, .py size: 2998 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 64e0 1863 b60b 0000  o.......d..c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 b60b 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000a 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 0904 0904 0904 6411 6405  m.Z.........d.d.
 00000060: 6506 6406 6506 6407 6506 6408 6503 6501  e.d.e.d.e.d.e.e.
 00000070: 6a07 1900 6608 6409 640a 8405 5a08 0904  j...f.d.d...Z...
```

## tests/text/si_prefix_test.py

```diff
@@ -10,35 +10,35 @@
         self.assertEqual("0", si_prefix(0))
         self.assertEqual("100", si_prefix(100))
         self.assertEqual("100.0", si_prefix(100.0))
         self.assertEqual("1050", si_prefix(1050))
         self.assertEqual("1.2k", si_prefix(1210, precision=1))
         self.assertEqual("1100k", si_prefix(1.1e6, threshold=1.15, precision=0))
         self.assertEqual("1.1M", si_prefix(1.1e6, threshold=1.05, precision=1))
-        self.assertEqual("1.2E+29", si_prefix(1.23e29))
+        self.assertEqual("1.2E+49", si_prefix(1.23e49))
         self.assertEqual("1.2 giga", si_prefix(1.2e9, full_names=True))
 
     def test_negative_prefix_decimal(self) -> None:
         self.assertEqual("100.0m", si_prefix(0.1))
         self.assertEqual("1.1m", si_prefix(1.1e-3, threshold=1.05))
         self.assertEqual("1100μ", si_prefix(1.1e-3, threshold=1.2, precision=0))
         self.assertEqual(
             "1100u", si_prefix(1.1e-3, threshold=1.2, precision=0, ascii_only=True)
         )
-        self.assertEqual("1.2E-29", si_prefix(1.23e-29))
+        self.assertEqual("1.2E-49", si_prefix(1.23e-49))
         self.assertEqual("1.2 atto", si_prefix(1.2e-18, full_names=True))
 
     def test_signed_value_decimal(self) -> None:
         self.assertEqual("-100", si_prefix(-100))
         self.assertEqual("-100.0", si_prefix(-100.0))
         self.assertEqual("-1050", si_prefix(-1050))
         self.assertEqual("-1.2k", si_prefix(-1210, precision=1))
         self.assertEqual("-1100k", si_prefix(-1.1e6, threshold=1.15, precision=0))
         self.assertEqual("-1.1M", si_prefix(-1.1e6, threshold=1.05, precision=1))
-        self.assertEqual("-1.2E+29", si_prefix(-1.23e29))
+        self.assertEqual("-1.2E+49", si_prefix(-1.23e49))
 
         self.assertEqual(
             "+1.2k", si_prefix(1210, precision=1, sign=Sign.POSITIVE_AND_NEGATIVE)
         )
         self.assertEqual(
             " 1.2k", si_prefix(1210, precision=1, sign=Sign.SPACE_FOR_POSITIVE)
         )
@@ -47,32 +47,34 @@
         self.assertEqual("0", si_prefix(0, mode=Mode.BINARY))
         self.assertEqual("100", si_prefix(100, mode=Mode.BINARY))
         # NB that this is 1.1 * 1024, not 1.1 * 1000!
         self.assertEqual("1120", si_prefix(1120, mode=Mode.BINARY, threshold=1.1))
         self.assertEqual(
             "1.09k", si_prefix(1120, mode=Mode.BINARY, threshold=1.05, precision=2)
         )
-        self.assertEqual("1.2*2^90", si_prefix(1.2 * math.pow(2, 90), mode=Mode.BINARY))
+        self.assertEqual(
+            "1.2*2^120", si_prefix(1.2 * math.pow(2, 120), mode=Mode.BINARY)
+        )
 
     def test_positive_prefix_iec(self) -> None:
         self.assertEqual("0", si_prefix(0, mode=Mode.IEC))
         self.assertEqual("100", si_prefix(100, mode=Mode.IEC))
         self.assertEqual(
             "1.09Ki", si_prefix(1120, mode=Mode.IEC, threshold=1.05, precision=2)
         )
-        self.assertEqual("1.2*2^90", si_prefix(1.2 * math.pow(2, 90), mode=Mode.IEC))
+        self.assertEqual("1.2*2^120", si_prefix(1.2 * math.pow(2, 120), mode=Mode.IEC))
 
     def test_negative_prefix_iec(self) -> None:
         self.assertEqual("1.3μi", si_prefix(1.2e-6, mode=Mode.IEC))
         self.assertEqual("1.3*2^-20", si_prefix(1.2e-6, mode=Mode.IEC, full_names=True))
 
     def test_negative_prefix_binary(self) -> None:
         # Each ten powers of two is an index position, so this is 5*2^7*2^-20 = 640 * 2^-20
         self.assertEqual("640.0μ", si_prefix(5 * math.pow(2, -13), mode=Mode.BINARY))
         self.assertEqual(
-            "1.2*2^-90", si_prefix(1.2 * math.pow(2, -90), mode=Mode.BINARY)
+            "1.2*2^-120", si_prefix(1.2 * math.pow(2, -120), mode=Mode.BINARY)
         )
 
     def test_corner_cases(self) -> None:
         self.assertEqual("nan", si_prefix(math.nan))
         self.assertEqual("nan", si_prefix(math.nan, mode=Mode.IEC))
         self.assertEqual("inf", si_prefix(math.inf))
```

## tests/text/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 21:13:05 2022 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e1cc d562 0000 0000  o..........b....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 0000 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa39 6275 696c 642f 6264  .r.....9build/bd
 00000050: 6973 742e 6d61 636f 7378 2d31 322e 342d  ist.macosx-12.4-
 00000060: 7838 365f 3634 2f65 6767 2f74 6573 7473  x86_64/egg/tests
 00000070: 2f74 6578 742f 5f5f 696e 6974 5f5f 2e70  /text/__init__.p
```

## tests/text/__pycache__/formatter_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jul 23 00:15:23 2022 UTC, .py size: 815 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9b3d db62 2f03 0000  o........=.b/...
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 2f03 0000  o.......!.vc/...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6500 6a03  ..G.d.d...d.e.j.
 00000050: 8303 5a04 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000060: 2901 da09 466f 726d 6174 7465 7263 0000  )...Formatterc..
 00000070: 0000 0000 0000 0000 0000 0000 0000 0300  ................
```

## tests/text/__pycache__/now_and_then_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Sep 30 00:22:39 2022 UTC, .py size: 1801 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cf36 3663 0907 0000  o........66c....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 0907 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 0100 4700 6404 6405  m.Z.m.Z...G.d.d.
 00000060: 8400 6405 6500 6a07 8303 5a08 6401 5300  ..d.e.j...Z.d.S.
 00000070: 2906 e900 0000 004e 2902 da08 6461 7465  )......N)...date
```

## tests/text/__pycache__/print_counter_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jul 23 00:15:23 2022 UTC, .py size: 930 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9b3d db62 a203 0000  o........=.b....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 a203 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 4700 6403 6404 8400 6404 6502 6a05  ..G.d.d...d.e.j.
 00000060: 8303 5a06 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da0c 5072 696e 7443 6f75 6e74 6572  )...PrintCounter
```

## tests/text/__pycache__/si_prefix_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jul 23 00:15:23 2022 UTC, .py size: 3655 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9b3d db62 470e 0000  o........=.bG...
+00000000: 6f0d 0d0a 0000 0000 0eb8 4e64 630e 0000  o.........Ndc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 0100 4700 6404 6405  d.l.m.Z...G.d.d.
 00000060: 8400 6405 6501 6a07 8303 5a08 6401 5300  ..d.e.j...Z.d.S.
 00000070: 2906 e900 0000 004e 2902 da04 4d6f 6465  )......N)...Mode
@@ -33,16 +33,16 @@
 00000200: 007a 0531 3030 2e30 6700 0000 0000 0059  .z.100.0g......Y
 00000210: 405a 0431 3035 3069 1a04 0000 7a04 312e  @Z.1050i....z.1.
 00000220: 326b e9ba 0400 00e9 0100 0000 a901 da09  2k..............
 00000230: 7072 6563 6973 696f 6e5a 0531 3130 306b  precisionZ.1100k
 00000240: 6700 0000 00e0 c830 41e7 6666 6666 6666  g......0A.ffffff
 00000250: f23f a902 da09 7468 7265 7368 6f6c 6472  .?....thresholdr
 00000260: 0d00 0000 7a04 312e 314d e7cd cccc cccc  ....z.1.1M......
-00000270: ccf0 3f7a 0731 2e32 452b 3239 67da 920c  ..?z.1.2E+29g...
-00000280: 72f3 d6f8 457a 0831 2e32 2067 6967 6167  r...Ez.1.2 gigag
+00000270: ccf0 3f7a 0731 2e32 452b 3439 6718 92af  ..?z.1.2E+49g...
+00000280: 26fe d420 4a7a 0831 2e32 2067 6967 6167  &.. Jz.1.2 gigag
 00000290: 0000 0000 a3e1 d141 54a9 01da 0a66 756c  .......AT....ful
 000002a0: 6c5f 6e61 6d65 73a9 02da 0b61 7373 6572  l_names....asser
 000002b0: 7445 7175 616c 7203 0000 00a9 01da 0473  tEqualr........s
 000002c0: 656c 66a9 0072 1800 0000 fa3f 6275 696c  elf..r.....?buil
 000002d0: 642f 6264 6973 742e 6d61 636f 7378 2d31  d/bdist.macosx-1
 000002e0: 322e 342d 7838 365f 3634 2f65 6767 2f74  2.4-x86_64/egg/t
 000002f0: 6573 7473 2f74 6578 742f 7369 5f70 7265  ests/text/si_pre
@@ -65,16 +65,16 @@
 00000400: 0201 0064 0053 0029 134e 7a06 3130 302e  ...d.S.).Nz.100.
 00000410: 306d 679a 9999 9999 99b9 3f7a 0431 2e31  0mg.......?z.1.1
 00000420: 6d67 2f6e a301 bc05 523f 7211 0000 0029  mg/n....R?r....)
 00000430: 0172 1000 0000 7506 0000 0031 3130 30ce  .r....u....1100.
 00000440: bce7 3333 3333 3333 f33f 7201 0000 0072  ..333333.?r....r
 00000450: 0f00 0000 5a05 3131 3030 7554 2903 7210  ....Z.1100uT).r.
 00000460: 0000 0072 0d00 0000 5a0a 6173 6369 695f  ...r....Z.ascii_
-00000470: 6f6e 6c79 7a07 312e 3245 2d32 3967 d514  onlyz.1.2E-29g..
-00000480: 240b 282f ef39 7a08 312e 3220 6174 746f  $.(/.9z.1.2 atto
+00000470: 6f6e 6c79 7a07 312e 3245 2d34 3967 8bed  onlyz.1.2E-49g..
+00000480: b99c 8702 c735 7a08 312e 3220 6174 746f  .....5z.1.2 atto
 00000490: 6701 1ec9 fbd6 2236 3c72 1200 0000 7214  g....."6<r....r.
 000004a0: 0000 0072 1600 0000 7218 0000 0072 1800  ...r....r....r..
 000004b0: 0000 7219 0000 00da 1c74 6573 745f 6e65  ..r......test_ne
 000004c0: 6761 7469 7665 5f70 7265 6669 785f 6465  gative_prefix_de
 000004d0: 6369 6d61 6c14 0000 0073 1000 0000 1001  cimal....s......
 000004e0: 1401 1601 0401 1001 04ff 1003 1801 7a29  ..............z)
 000004f0: 5349 5072 6566 6978 5465 7374 2e74 6573  SIPrefixTest.tes
@@ -96,15 +96,15 @@
 000005f0: 2d31 3030 699c ffff ff7a 062d 3130 302e  -100i....z.-100.
 00000600: 3067 0000 0000 0000 59c0 7a05 2d31 3035  0g......Y.z.-105
 00000610: 3069 e6fb ffff 7a05 2d31 2e32 6b69 46fb  0i....z.-1.2kiF.
 00000620: ffff 720b 0000 0072 0c00 0000 7a06 2d31  ..r....r....z.-1
 00000630: 3130 306b 6700 0000 00e0 c830 c172 0e00  100kg......0.r..
 00000640: 0000 7201 0000 0072 0f00 0000 7a05 2d31  ..r....r....z.-1
 00000650: 2e31 4d72 1100 0000 7a08 2d31 2e32 452b  .1Mr....z.-1.2E+
-00000660: 3239 67da 920c 72f3 d6f8 c57a 052b 312e  29g...r....z.+1.
+00000660: 3439 6718 92af 26fe d420 ca7a 052b 312e  49g...&.. .z.+1.
 00000670: 326b 720a 0000 0029 0272 0d00 0000 da04  2kr....).r......
 00000680: 7369 676e 7a05 2031 2e32 6b29 0572 1500  signz. 1.2k).r..
 00000690: 0000 7203 0000 0072 0400 0000 5a15 504f  ..r....r....Z.PO
 000006a0: 5349 5449 5645 5f41 4e44 5f4e 4547 4154  SITIVE_AND_NEGAT
 000006b0: 4956 455a 1253 5041 4345 5f46 4f52 5f50  IVEZ.SPACE_FOR_P
 000006c0: 4f53 4954 4956 4572 1600 0000 7218 0000  OSITIVEr....r...
 000006d0: 0072 1800 0000 7219 0000 00da 1974 6573  .r....r......tes
@@ -126,107 +126,107 @@
 000007d0: 0214 0074 026a 0364 038d 02a1 0201 0064  ...t.j.d.......d
 000007e0: 0053 0029 114e 7207 0000 0072 0100 0000  .S.).Nr....r....
 000007f0: a901 da04 6d6f 6465 7208 0000 0072 0900  ....moder....r..
 00000800: 0000 5a04 3131 3230 e960 0400 0067 9a99  ..Z.1120.`...g..
 00000810: 9999 9999 f13f 2902 7220 0000 0072 1000  .....?).r ...r..
 00000820: 0000 7a05 312e 3039 6b72 1100 0000 e902  ..z.1.09kr......
 00000830: 0000 00a9 0372 2000 0000 7210 0000 0072  .....r ...r....r
-00000840: 0d00 0000 fa08 312e 322a 325e 3930 721b  ......1.2*2^90r.
-00000850: 0000 00e9 5a00 0000 2906 7215 0000 0072  ....Z...).r....r
-00000860: 0300 0000 7202 0000 00da 0642 494e 4152  ....r......BINAR
-00000870: 59da 046d 6174 68da 0370 6f77 7216 0000  Y..math..powr...
-00000880: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000890: da1b 7465 7374 5f70 6f73 6974 6976 655f  ..test_positive_
-000008a0: 7072 6566 6978 5f62 696e 6172 792e 0000  prefix_binary...
-000008b0: 0073 0e00 0000 1601 1601 1802 0401 1201  .s..............
-000008c0: 04ff 2603 7a28 5349 5072 6566 6978 5465  ..&.z(SIPrefixTe
-000008d0: 7374 2e74 6573 745f 706f 7369 7469 7665  st.test_positive
-000008e0: 5f70 7265 6669 785f 6269 6e61 7279 6301  _prefix_binaryc.
-000008f0: 0000 0000 0000 0000 0000 0001 0000 0009  ................
-00000900: 0000 0043 0000 0073 6c00 0000 7c00 a000  ...C...sl...|...
-00000910: 6401 7401 6402 7402 6a03 6403 8d02 a102  d.t.d.t.j.d.....
-00000920: 0100 7c00 a000 6404 7401 6405 7402 6a03  ..|...d.t.d.t.j.
-00000930: 6403 8d02 a102 0100 7c00 a000 6406 7401  d.......|...d.t.
-00000940: 6407 7402 6a03 6408 6409 640a 8d04 a102  d.t.j.d.d.d.....
-00000950: 0100 7c00 a000 640b 7401 640c 7404 a005  ..|...d.t.d.t...
-00000960: 6409 640d a102 1400 7402 6a03 6403 8d02  d.d.....t.j.d...
-00000970: a102 0100 6400 5300 290e 4e72 0700 0000  ....d.S.).Nr....
-00000980: 7201 0000 0072 1f00 0000 7208 0000 0072  r....r....r....r
-00000990: 0900 0000 7a06 312e 3039 4b69 7221 0000  ....z.1.09Kir!..
-000009a0: 0072 1100 0000 7222 0000 0072 2300 0000  .r....r"...r#...
-000009b0: 7224 0000 0072 1b00 0000 7225 0000 0029  r$...r....r%...)
-000009c0: 0672 1500 0000 7203 0000 0072 0200 0000  .r....r....r....
-000009d0: da03 4945 4372 2700 0000 7228 0000 0072  ..IECr'...r(...r
-000009e0: 1600 0000 7218 0000 0072 1800 0000 7219  ....r....r....r.
-000009f0: 0000 00da 1874 6573 745f 706f 7369 7469  .....test_positi
-00000a00: 7665 5f70 7265 6669 785f 6965 6338 0000  ve_prefix_iec8..
-00000a10: 0073 0c00 0000 1601 1601 0401 1201 04ff  .s..............
-00000a20: 2603 7a25 5349 5072 6566 6978 5465 7374  &.z%SIPrefixTest
-00000a30: 2e74 6573 745f 706f 7369 7469 7665 5f70  .test_positive_p
-00000a40: 7265 6669 785f 6965 6363 0100 0000 0000  refix_iecc......
-00000a50: 0000 0000 0000 0100 0000 0800 0000 4300  ..............C.
-00000a60: 0000 7332 0000 007c 00a0 0064 0174 0164  ..s2...|...d.t.d
-00000a70: 0274 026a 0364 038d 02a1 0201 007c 00a0  .t.j.d.......|..
-00000a80: 0064 0474 0164 0274 026a 0364 0564 068d  .d.t.d.t.j.d.d..
-00000a90: 03a1 0201 0064 0053 0029 074e 7506 0000  .....d.S.).Nu...
-00000aa0: 0031 2e33 cebc 6967 7683 0df4 f521 b43e  .1.3..igv....!.>
-00000ab0: 721f 0000 007a 0931 2e33 2a32 5e2d 3230  r....z.1.3*2^-20
-00000ac0: 5429 0272 2000 0000 7213 0000 0029 0472  T).r ...r....).r
-00000ad0: 1500 0000 7203 0000 0072 0200 0000 722a  ....r....r....r*
-00000ae0: 0000 0072 1600 0000 7218 0000 0072 1800  ...r....r....r..
-00000af0: 0000 7219 0000 00da 1874 6573 745f 6e65  ..r......test_ne
-00000b00: 6761 7469 7665 5f70 7265 6669 785f 6965  gative_prefix_ie
-00000b10: 6340 0000 0073 0400 0000 1601 1c01 7a25  c@...s........z%
-00000b20: 5349 5072 6566 6978 5465 7374 2e74 6573  SIPrefixTest.tes
-00000b30: 745f 6e65 6761 7469 7665 5f70 7265 6669  t_negative_prefi
-00000b40: 785f 6965 6363 0100 0000 0000 0000 0000  x_iecc..........
-00000b50: 0000 0100 0000 0900 0000 4300 0000 7348  ..........C...sH
-00000b60: 0000 007c 00a0 0064 0174 0164 0274 02a0  ...|...d.t.d.t..
-00000b70: 0364 0364 04a1 0214 0074 046a 0564 058d  .d.d.....t.j.d..
-00000b80: 02a1 0201 007c 00a0 0064 0674 0164 0774  .....|...d.t.d.t
-00000b90: 02a0 0364 0364 08a1 0214 0074 046a 0564  ...d.d.....t.j.d
-00000ba0: 058d 02a1 0201 0064 0053 0029 094e 7507  .......d.S.).Nu.
-00000bb0: 0000 0036 3430 2e30 cebc e905 0000 0072  ...640.0.......r
-00000bc0: 2200 0000 69f3 ffff ff72 1f00 0000 7a09  "...i....r....z.
-00000bd0: 312e 322a 325e 2d39 3072 1b00 0000 69a6  1.2*2^-90r....i.
-00000be0: ffff ff29 0672 1500 0000 7203 0000 0072  ...).r....r....r
-00000bf0: 2700 0000 7228 0000 0072 0200 0000 7226  '...r(...r....r&
-00000c00: 0000 0072 1600 0000 7218 0000 0072 1800  ...r....r....r..
-00000c10: 0000 7219 0000 00da 1b74 6573 745f 6e65  ..r......test_ne
-00000c20: 6761 7469 7665 5f70 7265 6669 785f 6269  gative_prefix_bi
-00000c30: 6e61 7279 4400 0000 7308 0000 0022 0204  naryD...s...."..
-00000c40: 011a 0108 ff7a 2853 4950 7265 6669 7854  .....z(SIPrefixT
-00000c50: 6573 742e 7465 7374 5f6e 6567 6174 6976  est.test_negativ
-00000c60: 655f 7072 6566 6978 5f62 696e 6172 7963  e_prefix_binaryc
-00000c70: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000c80: 0700 0000 4300 0000 7340 0000 007c 00a0  ....C...s@...|..
-00000c90: 0064 0174 0174 026a 0383 01a1 0201 007c  .d.t.t.j.......|
-00000ca0: 00a0 0064 0174 0174 026a 0374 046a 0564  ...d.t.t.j.t.j.d
-00000cb0: 028d 02a1 0201 007c 00a0 0064 0374 0174  .......|...d.t.t
-00000cc0: 026a 0683 01a1 0201 0064 0053 0029 044e  .j.......d.S.).N
-00000cd0: da03 6e61 6e72 1f00 0000 da03 696e 6629  ..nanr......inf)
-00000ce0: 0772 1500 0000 7203 0000 0072 2700 0000  .r....r....r'...
-00000cf0: 722f 0000 0072 0200 0000 722a 0000 0072  r/...r....r*...r
-00000d00: 3000 0000 7216 0000 0072 1800 0000 7218  0...r....r....r.
-00000d10: 0000 0072 1900 0000 da11 7465 7374 5f63  ...r......test_c
-00000d20: 6f72 6e65 725f 6361 7365 734b 0000 0073  orner_casesK...s
-00000d30: 0600 0000 1201 1801 1601 7a1e 5349 5072  ..........z.SIPr
-00000d40: 6566 6978 5465 7374 2e74 6573 745f 636f  efixTest.test_co
-00000d50: 726e 6572 5f63 6173 6573 2902 7206 0000  rner_cases).r...
-00000d60: 004e 290b da08 5f5f 6e61 6d65 5f5f da0a  .N)...__name__..
-00000d70: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
-00000d80: 616c 6e61 6d65 5f5f 721a 0000 0072 1c00  alname__r....r..
-00000d90: 0000 721e 0000 0072 2900 0000 722b 0000  ..r....r)...r+..
-00000da0: 0072 2c00 0000 722e 0000 0072 3100 0000  .r,...r....r1...
-00000db0: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-00000dc0: 1900 0000 7205 0000 0008 0000 0073 1200  ....r........s..
-00000dd0: 0000 0800 0a01 0a0b 0a0a 0a10 0a0a 0a08  ................
-00000de0: 0a04 0e07 7205 0000 0029 0972 2700 0000  ....r....).r'...
-00000df0: 5a08 756e 6974 7465 7374 5a15 7079 7070  Z.unittestZ.pypp
-00000e00: 696e 2e74 6578 742e 7369 5f70 7265 6669  in.text.si_prefi
-00000e10: 7872 0200 0000 7203 0000 005a 1070 7970  xr....r....Z.pyp
-00000e20: 7069 6e2e 7465 7874 2e73 6967 6e72 0400  pin.text.signr..
-00000e30: 0000 5a08 5465 7374 4361 7365 7205 0000  ..Z.TestCaser...
-00000e40: 0072 1800 0000 7218 0000 0072 1800 0000  .r....r....r....
-00000e50: 7219 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000e60: 0000 0073 0a00 0000 0800 0801 1002 0c01  ...s............
-00000e70: 1603                                     ..
+00000840: 0d00 0000 fa09 312e 322a 325e 3132 3072  ......1.2*2^120r
+00000850: 1b00 0000 e978 0000 0029 0672 1500 0000  .....x...).r....
+00000860: 7203 0000 0072 0200 0000 da06 4249 4e41  r....r......BINA
+00000870: 5259 da04 6d61 7468 da03 706f 7772 1600  RY..math..powr..
+00000880: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000890: 00da 1b74 6573 745f 706f 7369 7469 7665  ...test_positive
+000008a0: 5f70 7265 6669 785f 6269 6e61 7279 2e00  _prefix_binary..
+000008b0: 0000 7312 0000 0016 0116 0118 0204 0112  ..s.............
+000008c0: 0104 ff04 031a 0108 ff7a 2853 4950 7265  .........z(SIPre
+000008d0: 6669 7854 6573 742e 7465 7374 5f70 6f73  fixTest.test_pos
+000008e0: 6974 6976 655f 7072 6566 6978 5f62 696e  itive_prefix_bin
+000008f0: 6172 7963 0100 0000 0000 0000 0000 0000  aryc............
+00000900: 0100 0000 0900 0000 4300 0000 736c 0000  ........C...sl..
+00000910: 007c 00a0 0064 0174 0164 0274 026a 0364  .|...d.t.d.t.j.d
+00000920: 038d 02a1 0201 007c 00a0 0064 0474 0164  .......|...d.t.d
+00000930: 0574 026a 0364 038d 02a1 0201 007c 00a0  .t.j.d.......|..
+00000940: 0064 0674 0164 0774 026a 0364 0864 0964  .d.t.d.t.j.d.d.d
+00000950: 0a8d 04a1 0201 007c 00a0 0064 0b74 0164  .......|...d.t.d
+00000960: 0c74 04a0 0564 0964 0da1 0214 0074 026a  .t...d.d.....t.j
+00000970: 0364 038d 02a1 0201 0064 0053 0029 0e4e  .d.......d.S.).N
+00000980: 7207 0000 0072 0100 0000 721f 0000 0072  r....r....r....r
+00000990: 0800 0000 7209 0000 007a 0631 2e30 394b  ....r....z.1.09K
+000009a0: 6972 2100 0000 7211 0000 0072 2200 0000  ir!...r....r"...
+000009b0: 7223 0000 0072 2400 0000 721b 0000 0072  r#...r$...r....r
+000009c0: 2500 0000 2906 7215 0000 0072 0300 0000  %...).r....r....
+000009d0: 7202 0000 00da 0349 4543 7227 0000 0072  r......IECr'...r
+000009e0: 2800 0000 7216 0000 0072 1800 0000 7218  (...r....r....r.
+000009f0: 0000 0072 1900 0000 da18 7465 7374 5f70  ...r......test_p
+00000a00: 6f73 6974 6976 655f 7072 6566 6978 5f69  ositive_prefix_i
+00000a10: 6563 3a00 0000 730c 0000 0016 0116 0104  ec:...s.........
+00000a20: 0112 0104 ff26 037a 2553 4950 7265 6669  .....&.z%SIPrefi
+00000a30: 7854 6573 742e 7465 7374 5f70 6f73 6974  xTest.test_posit
+00000a40: 6976 655f 7072 6566 6978 5f69 6563 6301  ive_prefix_iecc.
+00000a50: 0000 0000 0000 0000 0000 0001 0000 0008  ................
+00000a60: 0000 0043 0000 0073 3200 0000 7c00 a000  ...C...s2...|...
+00000a70: 6401 7401 6402 7402 6a03 6403 8d02 a102  d.t.d.t.j.d.....
+00000a80: 0100 7c00 a000 6404 7401 6402 7402 6a03  ..|...d.t.d.t.j.
+00000a90: 6405 6406 8d03 a102 0100 6400 5300 2907  d.d.......d.S.).
+00000aa0: 4e75 0600 0000 312e 33ce bc69 6776 830d  Nu....1.3..igv..
+00000ab0: f4f5 21b4 3e72 1f00 0000 7a09 312e 332a  ..!.>r....z.1.3*
+00000ac0: 325e 2d32 3054 2902 7220 0000 0072 1300  2^-20T).r ...r..
+00000ad0: 0000 2904 7215 0000 0072 0300 0000 7202  ..).r....r....r.
+00000ae0: 0000 0072 2a00 0000 7216 0000 0072 1800  ...r*...r....r..
+00000af0: 0000 7218 0000 0072 1900 0000 da18 7465  ..r....r......te
+00000b00: 7374 5f6e 6567 6174 6976 655f 7072 6566  st_negative_pref
+00000b10: 6978 5f69 6563 4200 0000 7304 0000 0016  ix_iecB...s.....
+00000b20: 011c 017a 2553 4950 7265 6669 7854 6573  ...z%SIPrefixTes
+00000b30: 742e 7465 7374 5f6e 6567 6174 6976 655f  t.test_negative_
+00000b40: 7072 6566 6978 5f69 6563 6301 0000 0000  prefix_iecc.....
+00000b50: 0000 0000 0000 0001 0000 0009 0000 0043  ...............C
+00000b60: 0000 0073 4800 0000 7c00 a000 6401 7401  ...sH...|...d.t.
+00000b70: 6402 7402 a003 6403 6404 a102 1400 7404  d.t...d.d.....t.
+00000b80: 6a05 6405 8d02 a102 0100 7c00 a000 6406  j.d.......|...d.
+00000b90: 7401 6407 7402 a003 6403 6408 a102 1400  t.d.t...d.d.....
+00000ba0: 7404 6a05 6405 8d02 a102 0100 6400 5300  t.j.d.......d.S.
+00000bb0: 2909 4e75 0700 0000 3634 302e 30ce bce9  ).Nu....640.0...
+00000bc0: 0500 0000 7222 0000 0069 f3ff ffff 721f  ....r"...i....r.
+00000bd0: 0000 007a 0a31 2e32 2a32 5e2d 3132 3072  ...z.1.2*2^-120r
+00000be0: 1b00 0000 6988 ffff ff29 0672 1500 0000  ....i....).r....
+00000bf0: 7203 0000 0072 2700 0000 7228 0000 0072  r....r'...r(...r
+00000c00: 0200 0000 7226 0000 0072 1600 0000 7218  ....r&...r....r.
+00000c10: 0000 0072 1800 0000 7219 0000 00da 1b74  ...r....r......t
+00000c20: 6573 745f 6e65 6761 7469 7665 5f70 7265  est_negative_pre
+00000c30: 6669 785f 6269 6e61 7279 4600 0000 7308  fix_binaryF...s.
+00000c40: 0000 0022 0204 011a 0108 ff7a 2853 4950  ...".......z(SIP
+00000c50: 7265 6669 7854 6573 742e 7465 7374 5f6e  refixTest.test_n
+00000c60: 6567 6174 6976 655f 7072 6566 6978 5f62  egative_prefix_b
+00000c70: 696e 6172 7963 0100 0000 0000 0000 0000  inaryc..........
+00000c80: 0000 0100 0000 0700 0000 4300 0000 7340  ..........C...s@
+00000c90: 0000 007c 00a0 0064 0174 0174 026a 0383  ...|...d.t.t.j..
+00000ca0: 01a1 0201 007c 00a0 0064 0174 0174 026a  .....|...d.t.t.j
+00000cb0: 0374 046a 0564 028d 02a1 0201 007c 00a0  .t.j.d.......|..
+00000cc0: 0064 0374 0174 026a 0683 01a1 0201 0064  .d.t.t.j.......d
+00000cd0: 0053 0029 044e da03 6e61 6e72 1f00 0000  .S.).N..nanr....
+00000ce0: da03 696e 6629 0772 1500 0000 7203 0000  ..inf).r....r...
+00000cf0: 0072 2700 0000 722f 0000 0072 0200 0000  .r'...r/...r....
+00000d00: 722a 0000 0072 3000 0000 7216 0000 0072  r*...r0...r....r
+00000d10: 1800 0000 7218 0000 0072 1900 0000 da11  ....r....r......
+00000d20: 7465 7374 5f63 6f72 6e65 725f 6361 7365  test_corner_case
+00000d30: 734d 0000 0073 0600 0000 1201 1801 1601  sM...s..........
+00000d40: 7a1e 5349 5072 6566 6978 5465 7374 2e74  z.SIPrefixTest.t
+00000d50: 6573 745f 636f 726e 6572 5f63 6173 6573  est_corner_cases
+00000d60: 2902 7206 0000 004e 290b da08 5f5f 6e61  ).r....N)...__na
+00000d70: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000d80: da0c 5f5f 7175 616c 6e61 6d65 5f5f 721a  ..__qualname__r.
+00000d90: 0000 0072 1c00 0000 721e 0000 0072 2900  ...r....r....r).
+00000da0: 0000 722b 0000 0072 2c00 0000 722e 0000  ..r+...r,...r...
+00000db0: 0072 3100 0000 7218 0000 0072 1800 0000  .r1...r....r....
+00000dc0: 7218 0000 0072 1900 0000 7205 0000 0008  r....r....r.....
+00000dd0: 0000 0073 1200 0000 0800 0a01 0a0b 0a0a  ...s............
+00000de0: 0a10 0a0c 0a08 0a04 0e07 7205 0000 0029  ..........r....)
+00000df0: 0972 2700 0000 5a08 756e 6974 7465 7374  .r'...Z.unittest
+00000e00: 5a15 7079 7070 696e 2e74 6578 742e 7369  Z.pyppin.text.si
+00000e10: 5f70 7265 6669 7872 0200 0000 7203 0000  _prefixr....r...
+00000e20: 005a 1070 7970 7069 6e2e 7465 7874 2e73  .Z.pyppin.text.s
+00000e30: 6967 6e72 0400 0000 5a08 5465 7374 4361  ignr....Z.TestCa
+00000e40: 7365 7205 0000 0072 1800 0000 7218 0000  ser....r....r...
+00000e50: 0072 1800 0000 7219 0000 00da 083c 6d6f  .r....r......<mo
+00000e60: 6475 6c65 3e01 0000 0073 0a00 0000 0800  dule>....s......
+00000e70: 0801 1002 0c01 1603                      ........
```

## tests/util/__pycache__/__init__.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 0 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 0000 0000  o.......y.vc....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 0000 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0400 0000 6400  .....@...s....d.
 00000030: 5300 2901 4ea9 0072 0100 0000 7201 0000  S.).N..r....r...
 00000040: 0072 0100 0000 fa39 6275 696c 642f 6264  .r.....9build/bd
 00000050: 6973 742e 6d61 636f 7378 2d31 322e 342d  ist.macosx-12.4-
 00000060: 7838 365f 3634 2f65 6767 2f74 6573 7473  x86_64/egg/tests
 00000070: 2f75 7469 6c2f 5f5f 696e 6974 5f5f 2e70  /util/__init__.p
```

## tests/util/__pycache__/expression_test.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Nov 17 22:11:05 2022 UTC, .py size: 3281 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 79b1 7663 d10c 0000  o.......y.vc....
+00000000: 6f0d 0d0a 0000 0000 21bb 7663 d10c 0000  o.......!.vc....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6500 6a04 8303 5a05 6401 5300 2905 e900  e.j...Z.d.S.)...
 00000060: 0000 004e 2902 da0d 5341 4645 5f42 5549  ...N)...SAFE_BUI
 00000070: 4c54 494e 53da 0a45 7870 7265 7373 696f  LTINS..Expressio
@@ -145,16 +145,16 @@
 00000900: 0100 6400 5300 290a 4e7a 0f6c 6973 7428  ..d.S.).Nz.list(
 00000910: 7a69 7028 782c 2079 2929 7207 0000 00da  zip(x, y))r.....
 00000920: 0179 7208 0000 0029 0329 0272 2400 0000  .yr....).).r$...
 00000930: da01 6129 0272 0b00 0000 da01 6229 0272  ..a).r......b).r
 00000940: 2500 0000 da01 6372 2300 0000 2904 7228  %.....cr#...).r(
 00000950: 0000 0072 2900 0000 722a 0000 00da 0164  ...r)...r*.....d
 00000960: 2902 7207 0000 0072 2700 0000 3e04 0000  ).r....r'...>...
-00000970: 0072 0700 0000 7227 0000 00da 046c 6973  .r....r'.....lis
-00000980: 74da 037a 6970 2904 7203 0000 0072 0e00  t..zip).r....r..
+00000970: 0072 0700 0000 da04 6c69 7374 da03 7a69  .r......list..zi
+00000980: 7072 2700 0000 2904 7203 0000 0072 0e00  pr'...).r....r..
 00000990: 0000 da03 7365 7472 0900 0000 7212 0000  ....setr....r...
 000009a0: 0072 1500 0000 7215 0000 0072 1600 0000  .r....r....r....
 000009b0: da16 7465 7374 5f62 7569 6c74 696e 5f66  ..test_builtin_f
 000009c0: 756e 6374 696f 6e73 3700 0000 730a 0000  unctions7...s...
 000009d0: 0010 0104 0118 0104 ff1a 037a 2545 7870  ...........z%Exp
 000009e0: 7265 7373 696f 6e54 6573 742e 7465 7374  ressionTest.test
 000009f0: 5f62 7569 6c74 696e 5f66 756e 6374 696f  _builtin_functio
```

