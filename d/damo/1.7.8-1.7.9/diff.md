# Comparing `tmp/damo-1.7.8.tar.gz` & `tmp/damo-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.7.8.tar", last modified: Mon Apr 24 21:50:35 2023, max compression
+gzip compressed data, was "damo-1.7.9.tar", last modified: Mon May  1 19:59:59 2023, max compression
```

## Comparing `damo-1.7.8.tar` & `damo-1.7.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:35.804108 damo-1.7.8/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6881 2023-04-24 21:50:35.804108 damo-1.7.8/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6360 2023-04-24 21:50:31.000000 damo-1.7.8/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-04-24 21:50:31.000000 damo-1.7.8/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-04-24 21:50:35.804108 damo-1.7.8/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-04-24 21:50:31.000000 damo-1.7.8/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:35.788109 damo-1.7.8/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:35.800108 damo-1.7.8/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      916 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    33096 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9985 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8485 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_args_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17917 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17878 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    18889 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3643 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      768 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13288 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2900 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1611 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1545 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3289 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      677 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      650 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3958 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5568 2023-04-24 21:50:31.000000 damo-1.7.8/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-04-24 21:50:35.800108 damo-1.7.8/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6881 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-04-24 21:50:35.000000 damo-1.7.8/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:59.216548 damo-1.7.9/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7226 2023-05-01 19:59:59.216548 damo-1.7.9/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6705 2023-05-01 19:59:55.000000 damo-1.7.9/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-01 19:59:55.000000 damo-1.7.9/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-01 19:59:59.216548 damo-1.7.9/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-05-01 19:59:55.000000 damo-1.7.9/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:59.200549 damo-1.7.9/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:59.212548 damo-1.7.9/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      923 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_python2_support.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34053 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9985 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8485 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_args_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17961 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17960 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19344 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3644 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      768 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13296 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2970 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1611 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1545 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3079 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      677 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      650 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3966 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5576 2023-05-01 19:59:55.000000 damo-1.7.9/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-01 19:59:59.216548 damo-1.7.9/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7226 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-01 19:59:59.000000 damo-1.7.9/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.7.8/PKG-INFO` & `damo-1.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.7.8
+Version: 1.7.9
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.9/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -110,14 +110,22 @@
 ----------------------------------------------------------------------------------------
 
 Because the single line DAMOS scheme format is no more supported.  Please
 report your usecase to sj@kernel.org, damon@lists.linux.dev and
 linux-mm@kvack.org if you depend on those.
 
 
+damo suddenly prints `Python2 support of damo is deprecated` message. Why?
+--------------------------------------------------------------------------
+
+Because Python2 is no more supported.  Please report your usecase to
+sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
+those.
+
+
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
 
     $ git clone https://github.com/sjp38/masim
@@ -166,14 +174,15 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 Note: Previously, one-line scheme specification format like below was used.  It
-is now deprecated, and the support will be removed by 2023 Q2.  Please report
+is now DEPRECATED, and the support will be removed by 2023 Q2.  Please report
 your usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if
 you depend on those.
 
+    $ # !!! BELOW IS NO MORE SUPPORTED
     $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
     $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
     $ sudo damo schemes -c my_scheme <pid of your workload>
```

### Comparing `damo-1.7.8/README.md` & `damo-1.7.9/src/damo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: damo
+Version: 1.7.9
+Summary: DAMON user-space tool
+Home-page: https://github.com/awslabs/damo
+Author: SeongJae Park
+Author-email: sj@kernel.org
+Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
+Project-URL: DAMON, https://damonitor.github.io
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -27,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.9/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -95,14 +110,22 @@
 ----------------------------------------------------------------------------------------
 
 Because the single line DAMOS scheme format is no more supported.  Please
 report your usecase to sj@kernel.org, damon@lists.linux.dev and
 linux-mm@kvack.org if you depend on those.
 
 
+damo suddenly prints `Python2 support of damo is deprecated` message. Why?
+--------------------------------------------------------------------------
+
+Because Python2 is no more supported.  Please report your usecase to
+sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
+those.
+
+
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
 
     $ git clone https://github.com/sjp38/masim
@@ -151,14 +174,15 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 Note: Previously, one-line scheme specification format like below was used.  It
-is now deprecated, and the support will be removed by 2023 Q2.  Please report
+is now DEPRECATED, and the support will be removed by 2023 Q2.  Please report
 your usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if
 you depend on those.
 
+    $ # !!! BELOW IS NO MORE SUPPORTED
     $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
     $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
     $ sudo damo schemes -c my_scheme <pid of your workload>
```

### Comparing `damo-1.7.8/setup.py` & `damo-1.7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="damo",
-    version="1.7.8",
+    version="1.7.9",
     author="SeongJae Park",
     author_email="sj@kernel.org",
     description="DAMON user-space tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/awslabs/damo",
     project_urls={
```

### Comparing `damo-1.7.8/src/damo/_damo_dist.py` & `damo-1.7.9/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/_damo_fmt_str.py` & `damo-1.7.9/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/_damo_fs.py` & `damo-1.7.9/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/_damo_paddr_layout.py` & `damo-1.7.9/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/_damo_python2_support.py` & `damo-1.7.9/src/damo/_damo_python2_support.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 
 import os
 import subprocess
 import sys
 
 if sys.version.startswith('2.'):
     sys.stderr.write('''
-WARNING: damo will remove python2 support by 2023-Q2.  Please report your
-    usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if
-    you depend on those.
+Python2 support of damo is deprecated.  This will not work suddenly.
+
+Please report your usecase to sj@kernel.org, damon@lists.linux.dev and
+linux-mm@kvack.org if you depend on those.
 
 ''')
 
 # For supporting python 2.6
 try:
     subprocess.DEVNULL = subprocess.DEVNULL
 except AttributeError:
```

### Comparing `damo-1.7.8/src/damo/_damo_subcmds.py` & `damo-1.7.9/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/_damon.py` & `damo-1.7.9/src/damo/_damon.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,31 +75,130 @@
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict([
             ('min', _damo_fmt_str.format_nr(self.minimum, raw)),
             ('max', _damo_fmt_str.format_nr(self.maximum, raw)),
             ])
 
+unit_percent = 'percent'
+unit_samples = 'samples'
+unit_usec = 'usec'
+unit_aggr_intervals = 'aggr_intervals'
+
+class DamonNrAccesses:
+    samples = None
+    percent = None
+
+    def __init__(self, val, unit):
+        if unit == unit_samples:
+            self.samples = val
+        elif unit == unit_percent:
+            self.percent = val
+
+    def __eq__(self, other):
+        return (type(self) == type(other) and
+                (self.samples == other.samples or
+                    self.percent == other.percent))
+
+    def add_unset_unit(self, intervals):
+        if self.samples != None and self.percent != None:
+            return
+        max_val = intervals.aggr / intervals.sample
+        if self.samples == None:
+            self.samples = int(self.percent * max_val / 100)
+        elif self.percent == None:
+            self.percent = int(self.samples * 100.0 / max_val)
+
+    def to_str(self, unit, raw):
+        if unit == unit_percent:
+            return '%s %%' % (_damo_fmt_str.format_nr(self.percent, raw))
+        elif unit == unit_samples:
+            return '%s %s' % (_damo_fmt_str.format_nr(self.samples, raw),
+                    unit_samples)
+        raise Exception('unsupported unit for NrAccesses (%s)' % unit)
+
+class DamonAge:
+    usec = None
+    aggr_intervals = None
+
+    def __init__(self, val, unit):
+        if unit == unit_usec:
+            self.usec = val
+        elif unit == unit_aggr_intervals:
+            self.aggr_intervals = val
+        else:
+            raise Exception('DamonAge unsupported unit (%s)' % unit)
+
+    def __eq__(self, other):
+        return (type(self) == type(other) and
+                (self.usec == other.usec or
+                    self.aggr_intervals == other.aggr_intervals))
+
+    def add_unset_unit(self, intervals):
+        if self.usec != None and self.aggr_intervals != None:
+            return
+        if self.usec == None:
+            self.usec = self.aggr_intervals * intervals.aggr
+        elif self.aggr_intervals == None:
+            self.aggr_intervals = int(self.usec / intervals.aggr)
+
+    def to_str(self, unit, raw):
+        if unit == unit_usec:
+            return _damo_fmt_str.format_time_us_exact(self.usec, raw)
+        return '%s %s' % (_damo_fmt_str.format_nr(self.aggr_intervals, raw),
+                unit_aggr_intervals)
+
 class DamonRegion:
-    # [star, end)
+    # [start, end)
     start = None
     end = None
+    # nr_accesses and age could be None
+    nr_accesses = None
+    age = None
 
-    def __init__(self, start, end):
+    def __init__(self, start, end, nr_accesses=None, nr_accesses_unit=None,
+            age=None, age_unit=None):
         self.start = _damo_fmt_str.text_to_bytes(start)
         self.end = _damo_fmt_str.text_to_bytes(end)
 
-    def to_str(self, raw):
-        return _damo_fmt_str.format_addr_range(self.start, self.end, raw)
+        if nr_accesses == None:
+            return
+        self.nr_accesses = DamonNrAccesses(nr_accesses, nr_accesses_unit)
+        self.age = DamonAge(age, age_unit)
+
+    def to_str(self, raw, intervals=None):
+        if self.nr_accesses == None:
+            return _damo_fmt_str.format_addr_range(self.start, self.end, raw)
+
+        if intervals != None:
+            self.nr_accesses.add_unset_unit(intervals)
+            self.age.add_unset_unit(intervals)
+
+        if raw == False and intervals != None:
+            nr_accesses_unit = unit_percent
+            age_unit = unit_usec
+        else:
+            nr_accesses_unit = unit_samples
+            age_unit = unit_aggr_intervals
+        return '%s: nr_accesses: %s, age: %s' % (
+                _damo_fmt_str.format_addr_range(self.start, self.end, raw),
+                self.nr_accesses.to_str(nr_accesses_unit, raw),
+                self.age.to_str(age_unit, raw))
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
-        return type(self) == type(other) and '%s' % self == '%s' % other
+        if self.nr_accesses == None:
+            return type(self) == type(other) and '%s' % self == '%s' % other
+
+    # For aggregate_snapshots() support
+    def __hash__(self):
+        identification = '%s-%s' % (self.start, self.end)
+        return hash(identification)
 
     @classmethod
     def from_kvpairs(cls, kvpairs):
         return DamonRegion(kvpairs['start'], kvpairs['end'])
 
     def to_kvpairs(self, raw=False):
         return collections.OrderedDict([
@@ -133,73 +232,20 @@
 
     def to_kvpairs(self, raw=False):
         kvp = collections.OrderedDict()
         kvp['pid'] = self.pid
         kvp['regions'] = [r.to_kvpairs(raw) for r in self.regions]
         return kvp
 
-unit_percent = 'percent'
-unit_samples = 'samples'
-unit_usec = 'usec'
-unit_aggr_intervals = 'aggr_intervals'
-
-class DamonIntervalsBasedValUnit:
-    value = None
-    unit = None # percent, samples, usec, aggr_intervals
-
-    def __init__(self, value, unit):
-        self.value = value
-        self.unit = unit
-
-    def eq(self, other, intervals=None):
-        if intervals == None:
-            return self.value == other.value and self.unit == other.unit
-
-        return self.value == other.value_for(self.unit, intervals)
-
-    def __eq__(self, other):
-        return self.eq(other, None)
-
-    def value_for(self, new_unit, intervals):
-        if self.unit == new_unit:
-            return self.value
-        if self.unit == unit_samples and new_unit == unit_percent:
-            max_val = intervals.aggr / intervals.sample
-            return int(self.value * 100.0 / max_val)
-        elif self.unit == unit_percent and new_unit == unit_samples:
-            max_val = intervals.aggr / intervals.sample
-            return int(self.value * max_val / 100)
-        elif self.unit == unit_aggr_intervals and new_unit == unit_usec:
-            return self.value * intervals.aggr
-        elif self.unit == unit_usec and new_unit == unit_aggr_intervals:
-            return int(self.value / intervals.aggr)
-        raise Exception('unsupported unit change')
-
-    def convert_unit(self, new_unit, intervals):
-        self.value = self.value_for(new_unit, intervals)
-        self.unit = new_unit
-
-    def converted_for_unit(self, new_unit, intervals):
-        return DamonIntervalsBasedValUnit(
-                self.value_for(new_unit, intervals), new_unit)
-
-    def to_str(self, raw):
-        unit = self.unit
-
-        if unit == unit_usec:
-            return _damo_fmt_str.format_time_us_exact(self.value, raw)
-
-        if unit == unit_percent:
-            unit = '%'
-        return '%s %s' % (_damo_fmt_str.format_nr(self.value, raw), unit)
-
 class DamosAccessPattern:
     sz_bytes = None
-    nr_accesses = None # [min/max DamonIntervalsBasedValUnit]
-    age = None  # [min/max DamonIntervalsBasedValUnit]
+    nr_acc_min_max = None # [min/max DamonNrAccesses]
+    nr_accesses_unit = None
+    age_min_max = None # [min/max DamonAge]
+    age_unit = None
 
     # every region by default, so that it can be used for monitoring
     def __init__(self, sz_bytes=['min', 'max'],
             nr_accesses=['min', 'max'], nr_accesses_unit=unit_percent,
             age=['min', 'max'], age_unit=unit_usec):
         self.sz_bytes = [_damo_fmt_str.text_to_bytes(sz_bytes[0]),
                 _damo_fmt_str.text_to_bytes(sz_bytes[1])]
@@ -213,44 +259,46 @@
         if not nr_accesses_unit in parsers_for_unit:
             raise Exception('invalid access pattern nr_accesses_unit \'%s\'' %
                     nr_accesses_unit)
         if not age_unit in parsers_for_unit:
             raise Exception('invalid access pattern age_unit \'%s\'' %
                     age_unit)
 
-        unit = nr_accesses_unit
-        fn = parsers_for_unit[unit]
-        self.nr_accesses = [
-                DamonIntervalsBasedValUnit(fn(nr_accesses[0]), unit),
-                DamonIntervalsBasedValUnit(fn(nr_accesses[1]), unit)]
-
+        fn = parsers_for_unit[nr_accesses_unit]
+        self.nr_acc_min_max = [
+                DamonNrAccesses(fn(nr_accesses[0]), nr_accesses_unit),
+                DamonNrAccesses(fn(nr_accesses[1]), nr_accesses_unit)]
+        self.nr_accesses_unit = nr_accesses_unit
         fn = parsers_for_unit[age_unit]
-        self.age = [
-                DamonIntervalsBasedValUnit(fn(age[0]), age_unit),
-                DamonIntervalsBasedValUnit(fn(age[1]), age_unit)]
+        self.age_min_max = [
+                DamonAge(fn(age[0]), age_unit),
+                DamonAge(fn(age[1]), age_unit)]
+        self.age_unit = age_unit
 
     def to_str(self, raw):
         lines = [
             'sz: [%s, %s]' % (_damo_fmt_str.format_sz(self.sz_bytes[0], raw),
                 _damo_fmt_str.format_sz(self.sz_bytes[1], raw)),
             ]
         lines.append('nr_accesses: [%s, %s]' % (
-            self.nr_accesses[0].to_str(raw), self.nr_accesses[1].to_str(raw)))
-        lines.append('age: [%s, %s]' %
-                (self.age[0].to_str(raw), self.age[1].to_str(raw)))
+            self.nr_acc_min_max[0].to_str(self.nr_accesses_unit, raw),
+            self.nr_acc_min_max[1].to_str(self.nr_accesses_unit, raw)))
+        lines.append('age: [%s, %s]' % (
+            self.age_min_max[0].to_str(self.age_unit, raw),
+            self.age_min_max[1].to_str(self.age_unit, raw)))
         return '\n'.join(lines)
 
     def __str__(self):
         return self.to_str(False)
 
     def __eq__(self, other):
         return (type(self) == type(other) and
                 self.sz_bytes == other.sz_bytes and
-                self.nr_accesses == other.nr_accesses and
-                self.age == other.age)
+                self.nr_acc_min_max == other.nr_acc_min_max and
+                self.age_min_max == other.age_min_max)
 
     @classmethod
     def from_kvpairs(cls, kv):
         sz_bytes = [_damo_fmt_str.text_to_bytes(kv['sz_bytes']['min']),
                 _damo_fmt_str.text_to_bytes(kv['sz_bytes']['max'])]
 
         kv_ = kv['nr_accesses']
@@ -277,34 +325,38 @@
                 raise Exception('age units should be same')
             age = [min_age, max_age]
 
         return DamosAccessPattern(sz_bytes, nr_accesses, nr_accesses_unit, age,
                 age_unit)
 
     def to_kvpairs(self, raw=False):
-        min_nr_accesses = self.nr_accesses[0].to_str(raw)
-        max_nr_accesses = self.nr_accesses[1].to_str(raw)
-        min_age = self.age[0].to_str(raw)
-        max_age = self.age[1].to_str(raw)
+        min_nr_accesses = self.nr_acc_min_max[0].to_str(
+                self.nr_accesses_unit, raw)
+        max_nr_accesses = self.nr_acc_min_max[1].to_str(
+                self.nr_accesses_unit, raw)
+        min_age = self.age_min_max[0].to_str(self.age_unit, raw)
+        max_age = self.age_min_max[1].to_str(self.age_unit, raw)
 
         return collections.OrderedDict([
             ('sz_bytes', (collections.OrderedDict([
                 ('min', _damo_fmt_str.format_sz(self.sz_bytes[0], raw)),
                 ('max', _damo_fmt_str.format_sz(self.sz_bytes[1], raw))]))),
             ('nr_accesses', (collections.OrderedDict([
                 ('min', min_nr_accesses), ('max', max_nr_accesses)]))),
             ('age', (collections.OrderedDict([
                 ('min', min_age), ('max', max_age)]))),
             ])
 
     def convert_for_units(self, nr_accesses_unit, age_unit, intervals):
-        self.nr_accesses[0].convert_unit(nr_accesses_unit, intervals)
-        self.nr_accesses[1].convert_unit(nr_accesses_unit, intervals)
-        self.age[0].convert_unit(age_unit, intervals)
-        self.age[1].convert_unit(age_unit, intervals)
+        self.nr_acc_min_max[0].add_unset_unit(intervals)
+        self.nr_acc_min_max[1].add_unset_unit(intervals)
+        self.age_min_max[0].add_unset_unit(intervals)
+        self.age_min_max[1].add_unset_unit(intervals)
+        self.nr_accesses_unit = nr_accesses_unit
+        self.age_unit = age_unit
 
     def converted_for_units(self, nr_accesses_unit, age_unit, intervals):
         copied = copy.deepcopy(self)
         copied.convert_for_units(nr_accesses_unit, age_unit, intervals)
         return copied
 
     def effectively_equal(self, other, intervals):
@@ -494,43 +546,14 @@
             _damo_fmt_str.format_sz(self.sz_applied, raw)),
             'quota exceeded %d times' % self.qt_exceeds,
             ])
 
     def __str__(self):
         return self.to_str(False)
 
-class DamosTriedRegion:
-    start = None
-    end = None
-    nr_accesses = None
-    age = None
-
-    def __init__(self, start, end, nr_accesses, nr_accesses_unit,
-            age, age_unit):
-        self.start = start
-        self.end = end
-        self.nr_accesses = DamonIntervalsBasedValUnit(nr_accesses,
-                nr_accesses_unit)
-        self.age = DamonIntervalsBasedValUnit(age, age_unit)
-
-    def to_str(self, raw, intervals=None):
-        if raw == False and intervals != None:
-            nr_accesses = self.nr_accesses.converted_for_unit(unit_percent,
-                    intervals)
-            age = self.age.converted_for_unit(unit_usec, intervals)
-        else:
-            nr_accesses = self.nr_accesses
-            age = self.age
-        return '%s: nr_accesses: %s, age: %s' % (
-                _damo_fmt_str.format_addr_range(self.start, self.end, raw),
-                nr_accesses.to_str(raw), age.to_str(raw))
-
-    def __str__(self):
-        return self.to_str(False)
-
 # TODO: check support of pageout and lru_(de)prio
 damos_actions = [
         'willneed',
         'cold',
         'pageout',
         'hugepage',
         'nohugepage',
```

### Comparing `damo-1.7.8/src/damo/_damon_args.py` & `damo-1.7.9/src/damo/_damon_args.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/_damon_args_schemes.py` & `damo-1.7.9/src/damo/_damon_args_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/_damon_dbgfs.py` & `damo-1.7.9/src/damo/_damon_dbgfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,16 +95,16 @@
             intervals)
     quotas = damos.quotas
     watermarks = damos.watermarks
 
     max_nr_accesses = intervals.aggr / intervals.sample
     v0_scheme = '%d\t%d\t%d\t%d\t%d\t%d\t%s' % (
             pattern.sz_bytes[0], pattern.sz_bytes[1],
-            pattern.nr_accesses[0].value, pattern.nr_accesses[1].value,
-            pattern.age[0].value, pattern.age[1].value,
+            pattern.nr_acc_min_max[0].samples, pattern.nr_acc_min_max[1].samples,
+            pattern.age_min_max[0].aggr_intervals, pattern.age_min_max[1].aggr_intervals,
             damos_action_to_file_input(damos.action))
     if scheme_version == 0:
         return v0_scheme
 
     v1_scheme = '%s\t%d\t%d' % (v0_scheme,
             quotas.sz_bytes, quotas.reset_interval_ms)
     if scheme_version == 1:
```

### Comparing `damo-1.7.8/src/damo/_damon_result.py` & `damo-1.7.9/src/damo/_damon_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,14 @@
 import time
 
 import _damon
 
 PERF = 'perf'
 PERF_EVENT = 'damon:damon_aggregated'
 
-class DAMONRegion:
-    start = None
-    end = None
-    nr_accesses = None
-    age = None
-    age_unit = None # _damon.unit_aggr_intervals or _damon.unit_usec
-
-    def __init__(self, start, end, nr_accesses, age, age_unit):
-        self.start = start
-        self.end = end
-        self.nr_accesses = nr_accesses
-        self.age = age
-        self.age_unit = age_unit
-
 class DAMONSnapshot:
     start_time = None
     end_time = None
     regions = None
 
     def __init__(self, start_time, end_time):
         self.start_time = start_time
@@ -79,26 +65,28 @@
 def read_snapshot_from_record_file(f, start_time, end_time):
     snapshot = DAMONSnapshot(start_time, end_time)
     nr_regions = struct.unpack('I', f.read(4))[0]
     for r in range(nr_regions):
         start_addr = struct.unpack('L', f.read(8))[0]
         end_addr = struct.unpack('L', f.read(8))[0]
         nr_accesses = struct.unpack('I', f.read(4))[0]
-        region = DAMONRegion(start_addr, end_addr, nr_accesses, None,
-                _damon.unit_aggr_intervals)
+        region = _damon.DamonRegion(start_addr, end_addr,
+                nr_accesses, _damon.unit_samples,
+                None, _damon.unit_aggr_intervals)
         snapshot.regions.append(region)
     return snapshot
 
 # if number of snapshots is one, write_damon_record() adds a fake snapshot for
 # snapshot start time deduction.
 def is_fake_snapshot(snapshot):
     if len(snapshot.regions) != 1:
         return False
     r = snapshot.regions[0]
-    return r.start == 0 and r.end == 0 and r.nr_accesses == -1 and r.age == -1
+    return (r.start == 0 and r.end == 0 and
+            r.nr_accesses.samples == -1 and r.age.aggr_intervals == -1)
 
 def set_first_snapshot_start_time(result):
     for record in result.records:
         snapshots = record.snapshots
         if len(snapshots) < 2:
             break
         end_time = snapshots[-1].end_time
@@ -164,16 +152,17 @@
 
         start_addr, end_addr = [int(x) for x in fields[7][:-1].split('-')]
         nr_accesses = int(fields[8])
         if len(fields) == 10:
             age = int(fields[9])
         else:
             age = None
-        region = DAMONRegion(start_addr, end_addr, nr_accesses, age,
-                _damon.unit_aggr_intervals)
+        region = _damon.DamonRegion(start_addr, end_addr,
+                nr_accesses, _damon.unit_samples,
+                age, _damon.unit_aggr_intervals)
 
         return region, end_time, target_id, nr_regions
 
 def perf_script_to_damon_result(script_output):
     result = DAMONResult()
     snapshot = None
 
@@ -259,15 +248,15 @@
                 else:
                     f.write(struct.pack('L', record.target_id))
 
                 f.write(struct.pack('I', len(snapshot.regions)))
                 for region in snapshot.regions:
                     f.write(struct.pack('L', region.start))
                     f.write(struct.pack('L', region.end))
-                    f.write(struct.pack('I', region.nr_accesses))
+                    f.write(struct.pack('I', region.nr_accesses.samples))
 
 def write_damon_perf_script(result, file_path):
     '''
     Example of the normal perf script output:
 
     kdamond.0  4452 [000] 82877.315633: damon:damon_aggregated: \
             target_id=18446623435582458880 nr_regions=17 \
@@ -281,15 +270,16 @@
                 for region in snapshot.regions:
                     f.write(' '.join(['kdamond.x', 'xxxx', 'xxxx',
                         '%f:' % (snapshot.end_time / 1000000000.0),
                         'damon:damon_aggregated:',
                         'target_id=%s' % record.target_id,
                         'nr_regions=%d' % len(snapshot.regions),
                         '%d-%d: %d %s' % (region.start, region.end,
-                            region.nr_accesses, region.age)]) + '\n')
+                            region.nr_accesses.samples,
+                            region.age.aggr_intervals)]) + '\n')
 
 def parse_file_permission_str(file_permission_str):
     try:
         file_permission = int(file_permission_str, 8)
     except Exception as e:
         return None, 'parsing failed (%s)' % e
     if file_permission < 0o0 or file_permission > 0o777:
@@ -305,17 +295,17 @@
         if len(snapshots) == 1:
             # we cannot know start/end time of single snapshot from the file
             # to allow it with later read, write a fake snapshot
             snapshot = snapshots[0]
             snap_duration = snapshot.end_time - snapshot.start_time
             fake_snapshot = DAMONSnapshot(snapshot.end_time,
                     snapshot.end_time + snap_duration)
-            # -1 nr_accesses/ -1 age means fake
-            fake_snapshot.regions = [DAMONRegion(0, 0, -1, -1,
-                _damon.unit_aggr_intervals)]
+            # -1 nr_accesses.samples / -1 age.aggr_intervals means fake
+            fake_snapshot.regions = [_damon.DamonRegion(0, 0,
+                -1, _damon.unit_samples, -1, _damon.unit_aggr_intervals)]
             snapshots.append(fake_snapshot)
     if file_type == file_type_record:
         write_damon_record(result, file_path, 2)
     elif file_type == file_type_perf_script:
         write_damon_perf_script(result, file_path)
     else:
         print('write unsupported file type: %s' % file_type)
@@ -333,24 +323,28 @@
     return not (r1.end <= r2.start or r2.end <= r1.start)
 
 def add_region(regions, region, nr_acc_to_add):
     for r in regions:
         if regions_intersect(r, region):
             if not r in nr_acc_to_add:
                 nr_acc_to_add[r] = 0
-            nr_acc_to_add[r] = max(nr_acc_to_add[r], region.nr_accesses)
+            nr_acc_to_add[r] = max(nr_acc_to_add[r],
+                    region.nr_accesses.samples)
 
             new_regions = []
             if region.start < r.start:
-                new_regions.append(DAMONRegion(
-                    region.start, r.start, region.nr_accesses, region.age,
-                    _damon.unit_aggr_intervals))
+                new_regions.append(_damon.DamonRegion(
+                    region.start, r.start,
+                    region.nr_accesses.samples, _damon.unit_samepls,
+                    region.age.aggr_intervals, _damon.unit_aggr_intervals))
             if r.end < region.end:
-                new_regions.append(DAMONRegion(
-                        r.end, region.end, region.nr_accesses, region.age,
+                new_regions.append(_damon.DamonRegion(
+                        r.end, region.end,
+                        region.nr_accesses.samples, _damon.unit_samples,
+                        region.age.aggr_intervals,
                         _damon.unit_aggr_intervals))
 
             for new_r in new_regions:
                 add_region(regions, new_r, nr_acc_to_add)
             return
     regions.append(region)
 
@@ -361,15 +355,17 @@
         # snapshot has two regions, 1-5:2, 5-10: 4.  Aggregated snapshot should
         # be 1-10:9.  That is, we should add maximum nr_accesses of
         # intersecting regions.  nr_acc_to_add contains the information.
         nr_acc_to_add = {}
         for region in snapshot.regions:
             add_region(new_regions, region, nr_acc_to_add)
         for region in nr_acc_to_add:
-            region.nr_accesses += nr_acc_to_add[region]
+            region.nr_accesses.samples += nr_acc_to_add[region]
+            region.nr_accesses.val = region.nr_accesses.samples
+            region.nr_accesses.unit = _damon.unit_samples
 
     new_snapshot = DAMONSnapshot(snapshots[0].start_time,
             snapshots[-1].end_time)
     new_snapshot.regions = new_regions
     return new_snapshot
 
 def adjusted_snapshots(snapshots, aggregate_interval_us):
@@ -444,35 +440,31 @@
 
 def tried_regions_to_snapshot(tried_regions, intervals):
     snapshot_end_time_ns = time.time() * 1000000000
     snapshot_start_time_ns = snapshot_end_time_ns - intervals.aggr * 1000
     snapshot = DAMONSnapshot(snapshot_start_time_ns, snapshot_end_time_ns)
 
     for tried_region in tried_regions:
-        snapshot.regions.append(DAMONRegion(tried_region.start,
-            tried_region.end,
-            tried_region.nr_accesses.value_for(_damon.unit_samples,
-                intervals),
-            tried_region.age.value_for(_damon.unit_usec, intervals),
-            _damon.unit_usec))
+        snapshot.regions.append(tried_region)
     return snapshot
 
 def tried_regions_to_snapshots(monitor_scheme):
-    snapshots = {} # {kdamond idx: {ctx: Snapshot}}
+    snapshots = {} # {kdamond idx: {ctx idx: [Snapshot, intervals]}}
     for kdamond_idx, kdamond in enumerate(_damon.current_kdamonds()):
         if kdamond.state != 'on':
             continue
         # TODO: Make a cleaner way for passing the index
-        kdamond.idx = kdamond_idx
-        for ctx in kdamond.contexts:
+        for ctx_idx, ctx in enumerate(kdamond.contexts):
             for scheme in ctx.schemes:
                 if scheme.effectively_equal(monitor_scheme, ctx.intervals):
                     snapshot = tried_regions_to_snapshot(scheme.tried_regions,
                             ctx.intervals)
-                    snapshots[kdamond] = {ctx: snapshot}
+                    if not kdamond_idx in snapshots:
+                        snapshots[kdamond_idx] = {}
+                    snapshots[kdamond_idx][ctx_idx] = [snapshot, ctx.intervals]
                     break
     return snapshots
 
 def get_snapshots(access_pattern):
     'return DAMONSnapshots and an error'
     running_kdamond_idxs = _damon.running_kdamond_idxs()
     if len(running_kdamond_idxs) == 0:
```

### Comparing `damo-1.7.8/src/damo/_damon_sysfs.py` & `damo-1.7.9/src/damo/_damon_sysfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,20 +136,20 @@
 
     return {
         'sz': {
             'min': '%d' % pattern.sz_bytes[0],
             'max': '%d' % pattern.sz_bytes[1],
         },
         'nr_accesses': {
-            'min': '%d' % pattern.nr_accesses[0].value,
-            'max': '%d' % pattern.nr_accesses[1].value,
+            'min': '%d' % pattern.nr_acc_min_max[0].samples,
+            'max': '%d' % pattern.nr_acc_min_max[1].samples,
         },
         'age': {
-            'min': '%d' % pattern.age[0].value,
-            'max': '%d' % pattern.age[1].value,
+            'min': '%d' % pattern.age_min_max[0].aggr_intervals,
+            'max': '%d' % pattern.age_min_max[1].aggr_intervals,
         },
     }
 
 def wops_for_schemes(ctx):
     schemes = ctx.schemes
 
     schemes_wops = {}
@@ -297,14 +297,21 @@
         return 'currently only <=one target is supported'
     ensure_dirs_populated_for(kdamonds)
 
     return _damo_fs.write_files({kdamonds_dir: wops_for_kdamonds(kdamonds)})
 
 # for current_kdamonds()
 
+def numbered_dirs_content(files_content, nr_filename):
+    nr_dirs = int(files_content[nr_filename])
+    number_dirs = []
+    for i in range(nr_dirs):
+        number_dirs.append(files_content['%d' % i])
+    return number_dirs
+
 def number_sorted_dirs(files_content):
     number_dirs = {}
     for filename, content in files_content.items():
         try:
             nr = int(filename)
         except:
             continue
@@ -341,26 +348,27 @@
             int(files_content['high']),
             int(files_content['mid']),
             int(files_content['low']))
 
 def files_content_to_damos_filters(files_content):
     return [_damon.DamosFilter(filter_kv['type'].strip(),
             filter_kv['memcg_path'].strip(), filter_kv['matching'].strip())
-            for filter_kv in number_sorted_dirs(files_content)]
+            for filter_kv in numbered_dirs_content(
+                files_content, 'nr_filters')]
 
 def files_content_to_damos_stats(files_content):
     return _damon.DamosStats(
             int(files_content['nr_tried']),
             int(files_content['sz_tried']),
             int(files_content['nr_applied']),
             int(files_content['sz_applied']),
             int(files_content['qt_exceeds']))
 
 def files_content_to_damos_tried_regions(files_content):
-    return [_damon.DamosTriedRegion(
+    return [_damon.DamonRegion(
             int(kv['start']), int(kv['end']),
             int(kv['nr_accesses']), _damon.unit_samples,
             int(kv['age']), _damon.unit_aggr_intervals)
             for kv in number_sorted_dirs(files_content)]
 
 def files_content_to_scheme(files_content):
     return _damon.Damos(
@@ -374,15 +382,15 @@
             files_content_to_damos_tried_regions(
                 files_content['tried_regions'])
                 if 'tried_regions' in files_content else [])
 
 def files_content_to_regions(files_content):
     return [_damon.DamonRegion(
             int(kv['start']), int(kv['end']))
-            for kv in number_sorted_dirs(files_content)]
+            for kv in numbered_dirs_content(files_content, 'nr_regions')]
 
 def files_content_to_target(files_content):
     try:
         pid = int(files_content['pid_target'])
     except:
         pid = None
     regions = files_content_to_regions(files_content['regions'])
@@ -399,33 +407,37 @@
     nr_regions = _damon.DamonNrRegionsRange(
             int(nr_regions_content['min']),
             int(nr_regions_content['max']))
     ops = files_content['operations'].strip()
 
     targets_content = files_content['targets']
     targets = [files_content_to_target(content)
-            for content in number_sorted_dirs(targets_content)]
+            for content in numbered_dirs_content(
+                targets_content, 'nr_targets')]
 
     schemes_content = files_content['schemes']
     schemes = [files_content_to_scheme(content)
-            for content in number_sorted_dirs(schemes_content)]
+            for content in numbered_dirs_content(
+                schemes_content, 'nr_schemes')]
 
     return _damon.DamonCtx(intervals, nr_regions, ops, targets, schemes)
 
 def files_content_to_kdamond(files_content):
     contexts_content = files_content['contexts']
     contexts = [files_content_to_context(content)
-            for content in number_sorted_dirs(contexts_content)]
+            for content in numbered_dirs_content(
+                contexts_content, 'nr_contexts')]
     state = files_content['state'].strip()
     pid = files_content['pid'].strip()
     return _damon.Kdamond(state, pid, contexts)
 
 def files_content_to_kdamonds(files_contents):
     return [files_content_to_kdamond(content)
-            for content in number_sorted_dirs(files_contents)]
+            for content in numbered_dirs_content(
+                files_contents, 'nr_kdamonds')]
 
 def current_kdamonds():
     return files_content_to_kdamonds(
             _damo_fs.read_files(kdamonds_dir))
 
 def nr_current_kdamonds():
     nr_kdamonds, err = _damo_fs.read_file(nr_kdamonds_file)
```

### Comparing `damo-1.7.8/src/damo/damo.py` & `damo-1.7.9/src/damo/damo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 import os
 os.sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 import sys
```

### Comparing `damo-1.7.8/src/damo/damo_adjust.py` & `damo-1.7.9/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_features.py` & `damo-1.7.9/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_fmt_json.py` & `damo-1.7.9/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_heats.py` & `damo-1.7.9/src/damo/damo_heats.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             continue
 
         fraction_start = start
         addr_idx = int(float(fraction_start - addr_range[0]) / space_unit)
         while fraction_start < end:
             fraction_end = min((addr_idx + 1) * space_unit + addr_range[0],
                     end)
-            heat = region.nr_accesses * duration * (
+            heat = region.nr_accesses.samples * duration * (
                     fraction_end - fraction_start)
 
             pixel = pixels[addr_idx]
             heat += pixel.heat * pixel_sz
             pixel.heat = float(heat) / pixel_sz
 
             fraction_start = fraction_end
```

### Comparing `damo-1.7.8/src/damo/damo_lru_sort.py` & `damo-1.7.9/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_monitor.py` & `damo-1.7.9/src/damo/damo_monitor.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_nr_regions.py` & `damo-1.7.9/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_reclaim.py` & `damo-1.7.9/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_record.py` & `damo-1.7.9/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_report.py` & `damo-1.7.9/src/damo/damo_report.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_report_raw.py` & `damo-1.7.9/src/damo/damo_report_raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,13 +68,14 @@
             print('nr_regions: %s' % len(snapshot.regions))
             print('# %10s %12s  %12s  %11s %5s' %
                     ('start_addr', 'end_addr', 'length', 'nr_accesses', 'age'))
             for r in snapshot.regions:
                 print("%012x-%012x (%12s) %11d %5d" %
                         (r.start, r.end,
                             _damo_fmt_str.format_sz(r.end - r.start,
-                                args.raw_number), r.nr_accesses,
-                                r.age if r.age != None else -1))
+                                args.raw_number), r.nr_accesses.samples,
+                                r.age.aggr_intervals
+                                if r.age.aggr_intervals != None else -1))
             print('')
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.7.8/src/damo/damo_schemes.py` & `damo-1.7.9/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_start.py` & `damo-1.7.9/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_stat.py` & `damo-1.7.9/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_stat_kdamonds.py` & `damo-1.7.9/src/damo/damo_stat_kdamonds.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_stat_regions.py` & `damo-1.7.9/src/damo/damo_stat_regions.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,50 +7,47 @@
 
 import _damo_fmt_str
 import _damo_subcmds
 import _damon
 import _damon_result
 
 def priority(region, weights):
-    if region.nr_accesses > 0:
-        return region.nr_accesses * weights[0] + region.age * weights[1]
+    if region.nr_accesses.samples > 0:
+        return (region.nr_accesses.samples * weights[0] +
+                region.age * weights[1])
     return region.age * weights[1] * -1
 
 def __pr_schemes_tried_regions(regions, intervals, size_only, sortby,
         prio_weights, raw_nr):
 
     if sortby == 'priority':
         regions.sort(key=lambda region: priority(region, prio_weights))
 
     total_sz = 0
     for region in regions:
-        # region is DamonRegion.  Convert to DamosTriedRegion
-        region = _damon.DamosTriedRegion(region.start, region.end,
-                region.nr_accesses, _damon.unit_samples,
-                region.age / intervals.aggr, _damon.unit_aggr_intervals)
         if not size_only:
             print(region.to_str(raw_nr, intervals))
         else:
             total_sz += (region.end - region.start)
     if size_only:
         print('%s' % _damo_fmt_str.format_sz(total_sz, raw_nr))
 
 def update_pr_schemes_tried_regions(access_pattern, size_only, sortby,
         prio_weights, raw_nr):
     snapshots, err = _damon_result.get_snapshots(access_pattern)
     if snapshots == None:
         print(err)
         return
 
-    for kdamond, ctx_snapshots in snapshots.items():
-        for ctx, snapshot in ctx_snapshots.items():
-            ctx_idx = kdamond.contexts.index(ctx)
-            print('kdamond %s ctx %s' % (kdamond.idx, ctx_idx))
-            __pr_schemes_tried_regions(snapshot.regions, ctx.intervals,
-                    size_only, sortby, prio_weights, raw_nr)
+    for kdamond_idx, ctx_snapshot in snapshots.items():
+        for ctx_idx, snapshot_intervals in ctx_snapshot.items():
+            snapshot, intervals = snapshot_intervals
+            print('kdamond %s ctx %s' % (kdamond_idx, ctx_idx))
+            __pr_schemes_tried_regions(snapshot.regions, intervals, size_only,
+                    sortby, prio_weights, raw_nr)
 
 def set_argparser(parser):
     damo_stat.set_common_argparser(parser)
     parser.add_argument('--sz_region', metavar=('<min>', '<max>'), nargs=2,
             default=['min', 'max'],
             help='min/max size of regions (bytes)')
     parser.add_argument('--access_rate', metavar=('<min>', '<max>'), nargs=2,
```

### Comparing `damo-1.7.8/src/damo/damo_stat_schemes.py` & `damo-1.7.9/src/damo/damo_stat_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_stop.py` & `damo-1.7.9/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_translate_damos.py` & `damo-1.7.9/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_tune.py` & `damo-1.7.9/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.7.8/src/damo/damo_validate.py` & `damo-1.7.9/src/damo/damo_validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,12 +98,12 @@
                 if region.start >= region.end:
                     print('wrong regiosn [%d, %d)' % (saddr, eaddr))
                     exit(1)
 
                 if regions_boundary:
                     check_boundary(region, regions_boundary)
 
-                assert_value_in_range(region.nr_accesses, args.nr_accesses,
-                        'nr_accesses', False)
+                assert_value_in_range(region.nr_accesses.samples,
+                        args.nr_accesses, 'nr_accesses', False)
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.7.8/src/damo/damo_wss.py` & `damo-1.7.9/src/damo/damo_wss.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     wss_dists = {}
     for record in result.records:
         wss_dist = []
         for snapshot in record.snapshots:
             wss = 0
             for r in snapshot.regions:
                 # Ignore regions not fulfill working set conditions
-                if r.nr_accesses < acc_thres:
+                if r.nr_accesses.samples < acc_thres:
                     continue
                 if r.end - r.start < sz_thres:
                     continue
                 wss += r.end - r.start
             wss_dist.append(wss)
         if do_sort:
             wss_dist.sort(reverse=False)
```

### Comparing `damo-1.7.8/src/damo.egg-info/PKG-INFO` & `damo-1.7.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: damo
-Version: 1.7.8
-Summary: DAMON user-space tool
-Home-page: https://github.com/awslabs/damo
-Author: SeongJae Park
-Author-email: sj@kernel.org
-Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
-Project-URL: DAMON, https://damonitor.github.io
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 DAMO: Data Access Monitoring Operator
 =====================================
 
 `damo` is a user space tool for [DAMON](https://damonitor.github.io).  Using
 this, you can monitor the data access patterns of your system or workloads and
 make data access-aware memory management optimizations.
 
@@ -42,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.8/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.7.9/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.8/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.7.9/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -110,14 +95,22 @@
 ----------------------------------------------------------------------------------------
 
 Because the single line DAMOS scheme format is no more supported.  Please
 report your usecase to sj@kernel.org, damon@lists.linux.dev and
 linux-mm@kvack.org if you depend on those.
 
 
+damo suddenly prints `Python2 support of damo is deprecated` message. Why?
+--------------------------------------------------------------------------
+
+Because Python2 is no more supported.  Please report your usecase to
+sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if you depend on
+those.
+
+
 Recording Data Access Patterns
 ==============================
 
 Below commands record memory access patterns of a program and save the
 monitoring results in `damon.data` file.
 
     $ git clone https://github.com/sjp38/masim
@@ -166,14 +159,15 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 Note: Previously, one-line scheme specification format like below was used.  It
-is now deprecated, and the support will be removed by 2023 Q2.  Please report
+is now DEPRECATED, and the support will be removed by 2023 Q2.  Please report
 your usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if
 you depend on those.
 
+    $ # !!! BELOW IS NO MORE SUPPORTED
     $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
     $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
     $ sudo damo schemes -c my_scheme <pid of your workload>
```

### Comparing `damo-1.7.8/src/damo.egg-info/SOURCES.txt` & `damo-1.7.9/src/damo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

