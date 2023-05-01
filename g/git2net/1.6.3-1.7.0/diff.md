# Comparing `tmp/git2net-1.6.3.tar.gz` & `tmp/git2net-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2net-1.6.3.tar", last modified: Wed Feb 22 08:42:29 2023, max compression
+gzip compressed data, was "git2net-1.7.0.tar", last modified: Mon May  1 20:22:51 2023, max compression
```

## Comparing `git2net-1.6.3.tar` & `git2net-1.7.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:42:29.757987 git2net-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-22 08:42:16.000000 git2net-1.6.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-02-22 08:42:29.757987 git2net-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-02-22 08:42:16.000000 git2net-1.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:42:29.753987 git2net-1.6.3/git2net/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-22 08:42:16.000000 git2net-1.6.3/git2net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-02-22 08:42:16.000000 git2net-1.6.3/git2net/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-02-22 08:42:16.000000 git2net-1.6.3/git2net/complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-02-22 08:42:16.000000 git2net-1.6.3/git2net/disambiguation.py
--rw-r--r--   0 runner    (1001) docker     (123)    76453 2023-02-22 08:42:16.000000 git2net-1.6.3/git2net/extraction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:42:29.749987 git2net-1.6.3/git2net/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:42:29.753987 git2net-1.6.3/git2net/helpers/binary-extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-02-22 08:42:16.000000 git2net-1.6.3/git2net/helpers/binary-extensions/binary-extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)    25851 2023-02-22 08:42:16.000000 git2net-1.6.3/git2net/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:42:29.753987 git2net-1.6.3/git2net.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-02-22 08:42:29.000000 git2net-1.6.3/git2net.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-22 08:42:29.000000 git2net-1.6.3/git2net.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 08:42:29.000000 git2net-1.6.3/git2net.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-22 08:42:29.000000 git2net-1.6.3/git2net.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-22 08:42:29.000000 git2net-1.6.3/git2net.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-22 08:42:29.000000 git2net-1.6.3/git2net.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-22 08:42:16.000000 git2net-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-22 08:42:29.757987 git2net-1.6.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 08:42:29.757987 git2net-1.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-22 08:42:16.000000 git2net-1.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-02-22 08:42:16.000000 git2net-1.6.3/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.075456 git2net-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-01 20:22:40.000000 git2net-1.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-01 20:22:51.075456 git2net-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-01 20:22:40.000000 git2net-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.071455 git2net-1.7.0/git2net/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/disambiguation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81636 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/extraction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.071455 git2net-1.7.0/git2net/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.075456 git2net-1.7.0/git2net/helpers/binary-extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/helpers/binary-extensions/binary-extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-05-01 20:22:40.000000 git2net-1.7.0/git2net/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.075456 git2net-1.7.0/git2net.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-01 20:22:51.000000 git2net-1.7.0/git2net.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-01 20:22:40.000000 git2net-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-01 20:22:51.075456 git2net-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:51.075456 git2net-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 20:22:40.000000 git2net-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-05-01 20:22:40.000000 git2net-1.7.0/tests/test_functions.py
```

### Comparing `git2net-1.6.3/LICENSE.txt` & `git2net-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `git2net-1.6.3/PKG-INFO` & `git2net-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2net
-Version: 1.6.3
+Version: 1.7.0
 Summary: An OpenSource Python package for the extraction of fine-grained and time-stamped co-editing networks from git repositories.
 Home-page: https://gotec.github.io/git2net/
 Author: Christoph Gote
 Author-email: cgote@ethz.ch
 License: AGPL-3.0+
 Keywords: co-editing,networks,repository,mining,network,analysis
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2net-1.6.3/README.md` & `git2net-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `git2net-1.6.3/git2net/__init__.py` & `git2net-1.7.0/git2net/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,7 +20,13 @@
 from .disambiguation import disambiguate_aliases_db
 from .visualisation import get_line_editing_paths
 from .visualisation import get_commit_editing_dag
 from .visualisation import get_coediting_network
 from .visualisation import get_coauthorship_network
 from .visualisation import get_bipartite_network
 from .complexity import compute_complexity
+
+import logging
+
+logging.basicConfig(level=logging.INFO,
+                    format='[%(asctime)s]  %(name)s:%(levelname)-10s %(message)s',
+                    datefmt='%Y-%m-%d %H:%M:%S')
```

### Comparing `git2net-1.6.3/git2net/command_line.py` & `git2net-1.7.0/git2net/command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,15 +256,14 @@
                                              time_to=args.time_to)
             d.write_file(args.csvfile)
         elif args.projection == 'line_editing':
             if args.filename:
                 args.filename = [args.filename]
             _, d, _, _ = get_line_editing_paths(args.database,
                                                 file_paths=args.filename)
-            print(d)
             d.write_file(args.csvfile)
         elif args.projection == 'coedit':
             t, _, _ = get_coediting_network(args.database,
                                             time_from=args.time_from,
                                             time_to=args.time_to)
             t.write_file(args.csvfile)
         elif args.projection == 'coauthor':
```

### Comparing `git2net-1.6.3/git2net/complexity.py` & `git2net-1.7.0/git2net/complexity.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
     
     result_df = pd.DataFrame(result, index=[0])
         
     return result_df
 
 
 def compute_complexity(git_repo_dir, sqlite_db_file, no_of_processes=os.cpu_count(), read_chunksize = 1e6,
-                         write_chunksize = 100):
+                       write_chunksize = 100):
     """
     Computes complexity measures for all mined commit/file combinations in a given database. Computing
     complexities for merge commits is currently not supported.
     
     :param str git_repo_dir: path to the git repository that is analysed
     :param str sqlite_db_file: path to the SQLite database containing the mined commits
     :param str no_of_processes: number of parallel processes that are spawned
@@ -284,22 +284,23 @@
                   'new_path': row.new_path, 'events': row.events, 'levenshtein_distance': row.levenshtein_distance}
                      for idx, row in total_compute.iterrows()
                      if not (row.commit_hash, row.old_path, row.new_path) in already_done]
     
     def _init(git_repo_dir, git_init_lock_):
         global git_init_lock
         git_init_lock = git_init_lock_
-        
+      
+    
     with multiprocessing.Pool(no_of_processes, initializer=_init,
                               initargs=(git_repo_dir,git_init_lock)) as p:
         results = []
         with tqdm(total=len(args_pool), desc='complexity computation') as pbar:
             for result in p.imap_unordered(_compute_complexity_measures, args_pool, chunksize=1):
                 results.append(result)
-
+                
                 # We write the results to the database. If results are already present, we append
                 # the new results to them.
                 if len(results) >= write_chunksize:
                     results = pd.concat(results, axis=0, copy=False)
                     
                     results = results[['commit_hash', 'old_path', 'new_path',
                                        'events', 'levenshtein_distance',
@@ -310,14 +311,15 @@
                                        'FUN_pre', 'FUN_post', 'FUN_delta']]
                     
                     with sqlite3.connect(sqlite_db_file) as con:
                         results.to_sql('complexity', con, if_exists='append', index=False)
                     results=[]
 
                 pbar.update(1)
-
+                
+    
     # As we write the results in chunks, some might remain unwritten in the loop above. We write
     # them now.
     if len(results) != 0:
         results = pd.concat(results, axis=0, copy=False)
         with sqlite3.connect(sqlite_db_file) as con:
             results.to_sql('complexity', con, if_exists='append', index=False)
```

### Comparing `git2net-1.6.3/git2net/disambiguation.py` & `git2net-1.7.0/git2net/disambiguation.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,17 +33,24 @@
         cur = con.cursor()
 
         cols = [i[1] for i in cur.execute('PRAGMA table_info(commits)')]
 
         if 'author_id' not in cols:
             cur.execute("""ALTER TABLE commits
                            ADD COLUMN author_id""")
+
+        cur.execute('''
+            CREATE INDEX IF NOT EXISTS author_info_index ON commits(author_name,author_email);
+            ''')
+
         con.commit()
+
         for idx, row in aliases.iterrows():
             cur.execute("""UPDATE commits
                            SET author_id = :author_id
                            WHERE author_name IS :author_name
                            AND author_email IS :author_email""",
                         {'author_id': row.author_id,
                          'author_name': row.alias_name,
                          'author_email': row.alias_email})
-            con.commit()
+
+        con.commit()
```

### Comparing `git2net-1.6.3/git2net/extraction.py` & `git2net-1.7.0/git2net/extraction.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import os
 from subprocess import check_output
 
 import multiprocessing
 
 import pandas as pd
 from tqdm import tqdm
+from tqdm.contrib.logging import logging_redirect_tqdm
 import numpy as np
 from scipy.stats import entropy
 
 import pydriller as pydriller
 from Levenshtein import distance as lev_dist
 import datetime
 
@@ -25,47 +26,73 @@
 import collections
 import git
 from git.exc import GitCommandError
 
 from git2net import __version__
 
 import time
-import threading
+import sys
 
 import json
 
-git_init_lock = multiprocessing.Lock()
-
-try:
-    import thread
-except ImportError:
-    import _thread as thread
-
-
-class TimeoutException(Exception):   # Custom exception class
-    pass
+import contextlib
+import io
 
+import threading
+import ctypes
 
-class Alarm(threading.Thread):
-    def __init__(self, timeout):
-        threading.Thread.__init__(self)
-        self.timeout = timeout
-        self.daemon = True
+import logging
 
-    def run(self):
-        if self.timeout > 0:
-            time.sleep(self.timeout)
-            thread.interrupt_main()
+git_init_lock = multiprocessing.Lock()
 
 
 abs_path = os.path.dirname(__file__)
 rel_path = 'helpers/binary-extensions/binary-extensions.json'
 with open(os.path.join(abs_path, rel_path)) as json_file:
     binary_extensions = json.load(json_file)
 
+    
+class TimeoutException(Exception):
+    pass
+
+            
+class Timeout():
+    """
+    Context manager that raises TimeoutException after wait of length timeout.
+    If timeout is <= 0, no timer is started.
+    
+    """
+    def __init__(self, timeout):
+        self.timeout = timeout
+        self.timed_out = False
+        self.active = False
+        self.target_tid = threading.current_thread().ident
+        self.timer = None
+        
+    def __enter__(self):
+        if self.timeout > 0:
+            self.timer = threading.Timer(self.timeout, self.stop)
+            self.timer.start()
+            self.active = True
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        if self.active:
+            self.timer.cancel()
+            self.active = False
+        if exc_type == TimeoutException:
+            return True
+        return False
+        
+    def stop(self):
+        self.timed_out = True
+        # raise TimeoutException in main thread. Inspired by implementation in 'stopit'
+        ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(self.target_tid),
+                                                     ctypes.py_object(TimeoutException))
+    
 
 def _get_block_length(lines, k):
     """
     Calculates the length (in number of lines) of a edit of added/deleted
     lines starting in a given line k.
 
     :param dict lines: dictionary of added or deleted lines
@@ -569,15 +596,16 @@
         # Levenshtein edit distance set to 0 to distinguish from deletion
         if extraction_settings['extract_text']:
             e['pre_text'] = None
             e['post_text'] = None
         e['levenshtein_dist'] = 0
 
     else:
-        print(edit.type)
+        LOG = logging.getLogger('git2net')
+        LOG.error(edit.type)
         raise Exception("Unexpected error in '_get_edit_details'.")
 
     return e
 
 
 def is_binary_file(filename, file_content):
     """
@@ -1057,15 +1085,15 @@
     'param str email: git email
     'param pydriller.Git git_repo: PyDriller Git object
 
     :return:
         - *str* – corresponding username from mailmap
         - *str* – corresponding email from mailmap
     """
-    if name.strip().startswith('--'):
+    if name.strip().startswith('-'):
         test_str = '<{}>'.format(email)
     else:
         test_str = '{} <{}>'.format(name, email)
     out_str = git.Git(str(git_repo.path)).check_mailmap(test_str)
 
     matches = re.findall("^(.*) <(.*)>$", out_str)
     if len(matches) > 1:
@@ -1076,200 +1104,252 @@
     # else name and email remain the same as the ones passed
 
     return name, email
 
 
 def _process_commit(args):
     """
-    Extracts information on commit and all edits made with the commit.
+    Extracts information on commit and all edits made with the commit. As this function is run in
+    parallel workers, any outputs are returned and output in a serial manner.
 
     :param dict args: dictionary with arguments. For multiprocessing, function can only
                       take single input.
                       Dictionary must contain:
                           git_repo_dir: path to the git repository that is mined
                           commit_hash: hash of the commit that is processed
                           extraction_settings: settings for the extraction
 
     :return:
         *dict* – dict containing two dataframes with information of commit and edits
+        *tuple* – tuple of logging type and logging message if any were created, otherwise None
+        *str* – text of exception if any was raised, otherwise None
     """
-    with git_init_lock:
-        git_repo = pydriller.Git(args['git_repo_dir'])
-        commit = git_repo.get_commit(args['commit_hash'])
+    try:
+        log = None
+        exception = None
 
-    alarm = Alarm(args['extraction_settings']['timeout'])
-    alarm.start()
+        with contextlib.redirect_stderr(io.StringIO()) as redirected_stderr_ctx_mgr:
+            with git_init_lock:
+                git_repo = pydriller.Git(args['git_repo_dir'])
+                commit = git_repo.get_commit(args['commit_hash'])
 
-    try:
-        author_name, author_email = _check_mailmap(commit.author.name,
+            with Timeout(args['extraction_settings']['timeout']) as timeout:
+                author_name, author_email = _check_mailmap(commit.author.name,
                                                    commit.author.email,
                                                    git_repo)
 
-        committer_name, committer_email = _check_mailmap(commit.committer.name,
-                                                         commit.committer.email,
-                                                         git_repo)
-
-        # parse commit
-        c = {}
-        c['hash'] = commit.hash
-        c['author_email'] = author_email
-        c['author_name'] = author_name
-        c['committer_email'] = committer_email
-        c['committer_name'] = committer_name
-        c['author_date'] = commit.author_date.strftime('%Y-%m-%d %H:%M:%S')
-        c['committer_date'] = commit.committer_date \
-                                    .strftime('%Y-%m-%d %H:%M:%S')
-        c['author_timezone'] = commit.author_timezone
-        c['committer_timezone'] = commit.committer_timezone
-        c['no_of_modifications'] = len(commit.modified_files)
-        c['commit_message_len'] = len(commit.msg)
-        if args['extraction_settings']['extract_text']:
-            c['commit_message'] = commit.msg \
-                                        .encode('utf8', 'surrogateescape') \
-                                        .decode('utf8', 'replace')
-        c['project_name'] = commit.project_name
-        c['parents'] = ','.join(commit.parents)
-        c['merge'] = commit.merge
-        c['in_main_branch'] = commit.in_main_branch
-        c['branches'] = ','.join(commit.branches)
-
-        # parse modification
-        df_edits = pd.DataFrame()
-        if commit.merge and args['extraction_settings']['extract_merges']:
-            # Git does not create a modification if own changes are accpeted
-            # during a merge. Therefore, the edited files are extracted
-            # manually.
-            edited_file_paths = {f for p in commit.parents for f in
-                                 git.Git(str(git_repo.path))
-                                    .diff(commit.hash, p, '--name-only')
-                                    .split('\n')}
-
-            if (args['extraction_settings']['max_modifications'] > 0) and \
-               (len(edited_file_paths) >
-                    args['extraction_settings']['max_modifications']):
-                print('Commit exceeding max_modifications: ', commit.hash)
-                extracted_result = {'commit': pd.DataFrame(),
-                                    'edits': pd.DataFrame()}
-                return extracted_result
-
-            for edited_file_path in edited_file_paths:
-                exclude_file = False
-                for x in args['extraction_settings']['exclude']:
-                    if edited_file_path.startswith(x + os.sep) or \
-                       (edited_file_path == x):
-                        exclude_file = True
-                if not exclude_file:
-                    modification_info = {}
-                    try:
-                        file_content = git.Git(str(git_repo.path)) \
-                                          .show('{}:{}'
-                                                .format(commit.hash,
-                                                        edited_file_path))
-
-                        modification_info['filename'] = edited_file_path.split(os.sep)[-1]
-                        modification_info['new_path'] = edited_file_path
-                        modification_info['old_path'] = edited_file_path
-                        modification_info['modification_type'] = 'merge_self_accept'
-
-                        df_edits = pd.concat(
-                            [df_edits,
-                             _extract_edits_merge(
-                                 git_repo, commit, modification_info,
-                                 args['extraction_settings'])],
-                            axis=0, ignore_index=True, sort=True)
-                    except GitCommandError:
-                        # A GitCommandError occurs if the file was deleted. In
-                        # this case it currently has no content.
-
-                        # Get filenames from all modifications in merge commit.
-                        paths = [m.old_path for m in commit.modified_files]
-
-                        # Analyse changes if modification was recorded. Else,
-                        # the deletions were made before the merge.
-                        if edited_file_path in paths:
-                            modification_info['filename'] = edited_file_path.split(os.sep)[-1]
-                            # File was deleted.
-                            modification_info['new_path'] = None
-                            modification_info['old_path'] = edited_file_path
-                            modification_info['modification_type'] = 'merge_self_accept'
 
+                committer_name, committer_email = _check_mailmap(commit.committer.name,
+                                                                 commit.committer.email,
+                                                                 git_repo)
+                                
+                # parse commit
+                c = {}
+                c['hash'] = commit.hash
+                c['author_email'] = author_email
+                c['author_name'] = author_name
+                c['committer_email'] = committer_email
+                c['committer_name'] = committer_name
+                c['author_date'] = commit.author_date.strftime('%Y-%m-%d %H:%M:%S')
+                c['committer_date'] = commit.committer_date \
+                                            .strftime('%Y-%m-%d %H:%M:%S')
+                c['author_timezone'] = commit.author_timezone
+                c['committer_timezone'] = commit.committer_timezone
+                c['no_of_modifications'] = len(commit.modified_files)
+                c['commit_message_len'] = len(commit.msg)
+                if args['extraction_settings']['extract_text']:
+                    c['commit_message'] = commit.msg \
+                                                .encode('utf8', 'surrogateescape') \
+                                                .decode('utf8', 'replace')
+                c['project_name'] = commit.project_name
+                c['parents'] = ','.join(commit.parents)
+                c['merge'] = commit.merge
+                c['in_main_branch'] = commit.in_main_branch
+                c['branches'] = ','.join(commit.branches)
+
+                # parse modification
+                df_edits = pd.DataFrame()
+                if commit.merge and args['extraction_settings']['extract_merges']:
+                    # Git does not create a modification if own changes are accpeted
+                    # during a merge. Therefore, the edited files are extracted
+                    # manually.
+                    edited_file_paths = {f for p in commit.parents for f in
+                                         git.Git(str(git_repo.path))
+                                            .diff(commit.hash, p, '--name-only')
+                                            .split('\n')}
+
+                    if (args['extraction_settings']['max_modifications'] > 0) and \
+                       (len(edited_file_paths) >
+                            args['extraction_settings']['max_modifications']):
+                        log = ('warning', 'max_modifications exceeded: ' + commit.hash)
+                        extracted_result = {'commit': pd.DataFrame(),
+                                            'edits': pd.DataFrame()}
+                        return extracted_result, log, exception
+
+
+                    for edited_file_path in edited_file_paths:
+                        exclude_file = False
+                        for x in args['extraction_settings']['exclude']:
+                            if edited_file_path.startswith(x + os.sep) or \
+                               (edited_file_path == x):
+                                exclude_file = True
+                        if not exclude_file:
+                            modification_info = {}
+                            try:
+                                file_content = git.Git(str(git_repo.path)) \
+                                                  .show('{}:{}'
+                                                        .format(commit.hash,
+                                                                edited_file_path)) 
+
+                                modification_info['filename'] = edited_file_path.split(os.sep)[-1]
+                                modification_info['new_path'] = edited_file_path
+                                modification_info['old_path'] = edited_file_path
+                                modification_info['modification_type'] = 'merge_self_accept'
+
+                                df_edits = pd.concat(
+                                    [df_edits,
+                                     _extract_edits_merge(
+                                         git_repo, commit, modification_info,
+                                         args['extraction_settings'])],
+                                    axis=0, ignore_index=True, sort=True)
+                            except GitCommandError:
+                                # A GitCommandError occurs if the file was deleted. In
+                                # this case it currently has no content.
+
+                                # Get filenames from all modifications in merge commit.
+                                paths = [m.old_path for m in commit.modified_files]
+
+                                # Analyse changes if modification was recorded. Else,
+                                # the deletions were made before the merge.
+                                if edited_file_path in paths:
+                                    modification_info['filename'] = edited_file_path.split(os.sep)[-1]
+                                    # File was deleted.
+                                    modification_info['new_path'] = None
+                                    modification_info['old_path'] = edited_file_path
+                                    modification_info['modification_type'] = 'merge_self_accept'
+
+                                    df_edits = pd.concat(
+                                        [df_edits,
+                                         _extract_edits_merge(
+                                             git_repo, commit, modification_info,
+                                             args['extraction_settings'])],
+                                        axis=0, ignore_index=True, sort=True)
+
+                else:
+                    if (args['extraction_settings']['max_modifications'] > 0) and \
+                       (len(commit.modified_files) >
+                           args['extraction_settings']['max_modifications']):
+                        log = ('warning', 'max_modifications exceeded: ' + commit.hash)
+                        extracted_result = {'commit': pd.DataFrame(),
+                                            'edits': pd.DataFrame()}
+                        return extracted_result, log, exception
+
+                    for modification in commit.modified_files:
+                        exclude_file = False
+                        for x in args['extraction_settings']['exclude']:
+                            if modification.new_path:
+                                if modification.new_path.startswith(x + os.sep) or \
+                                   (modification.new_path == x):
+                                    exclude_file = True
+                            if not exclude_file and modification.old_path:
+                                if modification.old_path.startswith(x + os.sep):
+                                    exclude_file = True
+                        if not exclude_file:
                             df_edits = pd.concat(
                                 [df_edits,
-                                 _extract_edits_merge(
-                                     git_repo, commit, modification_info,
-                                     args['extraction_settings'])],
+                                 _extract_edits(git_repo, commit,
+                                                modification,
+                                                args['extraction_settings'])],
                                 axis=0, ignore_index=True, sort=True)
 
-        else:
-            if (args['extraction_settings']['max_modifications'] > 0) and \
-               (len(commit.modified_files) >
-                   args['extraction_settings']['max_modifications']):
-                print('Commit exceeding max_modifications: ', commit.hash)
-                extracted_result = {'commit': pd.DataFrame(),
-                                    'edits': pd.DataFrame()}
-                return extracted_result
-
-            for modification in commit.modified_files:
-                exclude_file = False
-                for x in args['extraction_settings']['exclude']:
-                    if modification.new_path:
-                        if modification.new_path.startswith(x + os.sep) or \
-                           (modification.new_path == x):
-                            exclude_file = True
-                    if not exclude_file and modification.old_path:
-                        if modification.old_path.startswith(x + os.sep):
-                            exclude_file = True
-                if not exclude_file:
-                    df_edits = pd.concat(
-                        [df_edits,
-                         _extract_edits(git_repo, commit,
-                                        modification,
-                                        args['extraction_settings'])],
-                        axis=0, ignore_index=True, sort=True)
-
-        df_commit = pd.DataFrame(c, index=[0])
-
-        extracted_result = {'commit': df_commit, 'edits': df_edits}
-    except KeyboardInterrupt:
-        print('Timeout processing commit: ', commit.hash)
-        extracted_result = {'commit': pd.DataFrame(), 'edits': pd.DataFrame()}
+                df_commit = pd.DataFrame(c, index=[0])
+
+                extracted_result = {'commit': df_commit, 'edits': df_edits}
 
-    del alarm
 
-    return extracted_result
+        redirected_stderr = redirected_stderr_ctx_mgr.getvalue().strip()
 
+        if redirected_stderr:
+            # Something was written to stderr. This could be a real error, however, often 
+            # it is just a notification that an exception was ignored while deleting an object
+            # after the threading timeout triggered. In this case, we ignore the message.
+            if not (redirected_stderr.startswith('Exception ignored in:') and \
+                    redirected_stderr.endswith('git2net.extraction.TimeoutException:')):
+                extracted_result = {'commit': pd.DataFrame(), 'edits': pd.DataFrame()}
+                log = ('error', 'processing error: ' + commit.hash)
+                exception = redirected_stderr
 
+        if pd.isnull(exception) and timeout.timed_out:
+            log = ('warning', 'processing timeout: ' + commit.hash)
+            extracted_result = {'commit': pd.DataFrame(), 'edits': pd.DataFrame()}
+
+        return extracted_result, log, exception
+
+    except Exception as e:
+        return e
+
+def _log_commit_results(log, exception):
+    """
+    Processes log and exception returned from _process_commit and creates corresponding entries.
+    
+    :param tuple log: tuple of logging type and logging message if any were created, otherwise None
+    :param str exception: text of exception if any was raised, otherwise None
+    
+    :return:
+        log message will be written and exception raised if one occurred
+    """
+    
+    LOG = logging.getLogger('git2net')
+
+    if pd.notnull(log):
+        if log[0] == 'warning':
+            LOG.warning(log[1])
+        elif log[0] == 'error':
+            LOG.error(log[1])
+            raise Exception(exception)
+        else:
+            Exception(("Not implemented logging type. Please report on "
+                       "https://github.com/gotec/git2net."))
+
+            
 def _process_repo_serial(git_repo_dir, sqlite_db_file, commits,
                          extraction_settings):
     """
     Processes all commits in a given git repository in a serial manner.
 
     :param str git_repo_dir: path to the git repository that is mined
     :param str sqlite_db_file: path (including database name) where the sqlite database will be created
     :param List[str] commits: list of commits that have to be processed
     :param dict extraction_settings: settings for the extraction
 
     :return:
         SQLite database will be written at specified location
     """
 
-    # git_repo = pydriller.Git(git_repo_dir)
-
+    LOG = logging.getLogger('git2net')
+    
     for commit in tqdm(commits, desc='Serial'):
-        args = {'git_repo_dir': git_repo_dir, 'commit_hash': commit.hash,
-                'extraction_settings': extraction_settings}
-        result = _process_commit(args)
+        with logging_redirect_tqdm(tqdm_class=tqdm):            
+            args = {'git_repo_dir': git_repo_dir, 'commit_hash': commit.hash,
+                    'extraction_settings': extraction_settings}
+            res = _process_commit(args)
 
-        with sqlite3.connect(sqlite_db_file) as con:
-            if not result['edits'].empty:
-                result['edits'].to_sql('edits', con, if_exists='append',
-                                       index=False)
-            if not result['commit'].empty:
-                result['commit'].to_sql('commits', con, if_exists='append',
-                                        index=False)
+            if isinstance(res, Exception):
+                raise res
+            else:
+                extracted_result, log, exception = res
+                _log_commit_results(log, exception)
+
+                with sqlite3.connect(sqlite_db_file) as con:
+                    if not extracted_result['edits'].empty:
+                        extracted_result['edits'].to_sql('edits', con, if_exists='append',
+                                                         index=False)
+                    if not extracted_result['commit'].empty:
+                        extracted_result['commit'].to_sql('commits', con, if_exists='append',
+                                                          index=False)
 
 
 # suggestion by marco-c (github.com/ishepard/pydriller/issues/110)
 def _init(git_repo_dir, git_init_lock_):
     global git_init_lock
     git_init_lock = git_init_lock_
 
@@ -1284,35 +1364,44 @@
     :param List[str] commits: list of commits that are already in the database
     :param dict extraction_settings: settings for the extraction
 
     :return:
         SQLite database will be written at specified location
     """
 
+    LOG = logging.getLogger('git2net')
+    
     args = [{'git_repo_dir': git_repo_dir, 'commit_hash': commit.hash,
              'extraction_settings': extraction_settings}
             for commit in commits]
 
     with multiprocessing.Pool(extraction_settings['no_of_processes'],
                               initializer=_init,
                               initargs=(git_repo_dir, git_init_lock)) as p:
         with tqdm(total=len(args), desc='Parallel ({0} processes)'
                   .format(extraction_settings['no_of_processes'])) as pbar:
-            for result in p.imap_unordered(
-                _process_commit, args,
-                    chunksize=extraction_settings['chunksize']):
-                with sqlite3.connect(sqlite_db_file) as con:
-                    if not result['edits'].empty:
-                        result['edits'].to_sql('edits', con,
-                                               if_exists='append', index=False)
-                    if not result['commit'].empty:
-                        result['commit'].to_sql('commits', con,
-                                                if_exists='append',
-                                                index=False)
-                pbar.update(1)
+            with logging_redirect_tqdm(tqdm_class=tqdm):
+                for res in p.imap_unordered(_process_commit, args, chunksize=extraction_settings['chunksize']):
+                    
+                    if isinstance(res, Exception):
+                        raise res
+                    else:
+                        extracted_result, log, exception = res
+
+                        _log_commit_results(log, exception)
+
+                        with sqlite3.connect(sqlite_db_file) as con:
+                            if not extracted_result['edits'].empty:
+                                extracted_result['edits'].to_sql('edits', con,
+                                                                 if_exists='append', index=False)
+                            if not extracted_result['commit'].empty:
+                                extracted_result['commit'].to_sql('commits', con,
+                                                                  if_exists='append',
+                                                                  index=False)
+                        pbar.update(1)
 
 
 def identify_file_renaming(git_repo_dir):
     """
     Identifies all names and locations different files in a repository have had.
 
     :param str git_repo_dir: path to the git repository that is mined
@@ -1435,25 +1524,28 @@
     :param str git_repo_dir: path to the git repository that is mined
     :param str sqlite_db_file: path (including database name) where with sqlite database
     :param List[str] commits: only consider specific set of commits, considers all if empty
 
     :return:
         *bool* – True if all commits are included in the database, otherwise False
     """
+    LOG = logging.getLogger('git2net')
+    
     git_repo = pydriller.Git(git_repo_dir)
     if os.path.exists(sqlite_db_file):
         try:
             with sqlite3.connect(sqlite_db_file) as con:
                 try:
                     p_commits = set(x[0] for x in
                                     con.execute("SELECT hash FROM commits")
                                     .fetchall())
                 except sqlite3.OperationalError:
+                    LOG.warning("Found a database on provided path that did not contain a 'commits' table.")
                     p_commits = set()
-        except sqlite3.OperationalError:
+        except (sqlite3.OperationalError, sqlite3.DatabaseError):
             raise Exception("The provided file is not a compatible database.")
     else:
         raise Exception("Found no database at provided path.")
 
     if not commits:
         commits = [c.hash for c in git_repo.get_list_commits(all=all_branches)]
     if set(commits).issubset(p_commits):
@@ -1475,79 +1567,83 @@
 
     :param str git_repo_dir: path to the git repository that is mined
     :param str sqlite_db_file: path (including database name) where with sqlite database
 
     :return:
         *pandas.DataFrame* – dataframe with details on missing commits
     """
+    LOG = logging.getLogger('git2net')
+    
     git_repo = pydriller.Git(git_repo_dir)
     if os.path.exists(sqlite_db_file):
         try:
             with sqlite3.connect(sqlite_db_file) as con:
                 try:
                     p_commits = set(x[0] for x in
                                     con.execute("SELECT hash FROM commits")
                                     .fetchall())
                 except sqlite3.OperationalError:
+                    LOG.warning("Found a database on provided path that did not contain a 'commits' table.")
                     p_commits = set()
         except sqlite3.OperationalError:
             raise Exception("The provided file is not a compatible database.")
     else:
         raise Exception("Found no database at provided path.")
 
     commits = [c for c in git_repo.get_list_commits(all=all_branches)]
     if not p_commits.issubset({c.hash for c in commits}):
         raise Exception("The database does not match the provided repository.")
 
     no_of_commits = len({c.hash for c in commits})
-    print('{} / {} ({:.2f}%) of commits were successfully mined.'.format(
-            len(p_commits), no_of_commits,
-            len(p_commits) / no_of_commits * 100))
+    LOG = logging.getLogger('git2net')
+    LOG.info('{} / {} ({:.2f}%) of commits were successfully mined.'.format(
+        len(p_commits), no_of_commits,
+        len(p_commits) / no_of_commits * 100))
 
     u_commits = [c for c in commits if c.hash not in p_commits]
 
     u_commit_info = {'hash': [],
                      'is_merge': [],
                      'modifications': [],
                      'author_name': [],
                      'author_email': [],
                      'author_date': []}
     for c in tqdm(u_commits):
         u_commit_info['hash'].append(c.hash)
         try:
             u_commit_info['is_merge'].append(c.merge)
         except:
-            print('Error reading "merge" for', c.hash)
+            LOG.error('Error reading "merge" for', c.hash)
             u_commit_info['is_merge'].append(None)
 
         if c.merge:
             u_commit_info['modifications'].append(
                 len({f for p in c.parents for f in
                      git.Git(str(git_repo.path))
                         .diff(c.hash, p, '--name-only').split('\n')}))
         else:
             u_commit_info['modifications'].append(len(c.modified_files))
 
         try:
             u_commit_info['author_name'].append(c.author.name)
         except:
-            print('Error reading "author.name" for', c.hash)
+            LOG.error('Error reading "author.name" for', c.hash)
             u_commit_info['author_name'].append(None)
 
         try:
             u_commit_info['author_email'].append(c.author.email)
         except:
-            print('Error reading "author.email" for', c.hash)
+            LOG.error('Error reading "author.email" for', c.hash)
             u_commit_info['author_email'].append(None)
 
         try:
             u_commit_info['author_date'].append(
                 c.author_date.strftime('%Y-%m-%d %H:%M:%S'))
         except:
-            print('Error reading "author_date" for', c.hash)
+            LOG.error('Error reading "author_date" for', c.hash)
             u_commit_info['author_date'].append(None)
 
     u_commits_info = pd.DataFrame(u_commit_info)
 
     return u_commits_info
 
 
@@ -1575,14 +1671,16 @@
     :param bool extract_text: extract the commit message and line texts
     :param bool extract_merges: process merges
     :param bool extract_merge_deletions: extract lines that are not accepted during a merge as 'deletions'
 
     :return:
         SQLite database will be written at specified location
     """
+    LOG = logging.getLogger('git2net')
+    
     git_version = check_output(['git', '--version']).strip().decode("utf-8")
 
     parsed_git_version = re.search(r'(\d+)\.(\d+)\.(\d+)', git_version) \
                            .groups()
 
     if int(parsed_git_version[0]) < 2 or \
        (
@@ -1632,20 +1730,18 @@
                         p_commits = set(x[0] for x in
                                         con.execute("SELECT hash FROM commits")
                                         .fetchall())
                     except sqlite3.OperationalError:
                         p_commits = set()
                     if all_branches:
                         c_commits = set(c.hash for c in
-                                        pydriller.Git(git_repo_dir)
-                                                 .get_list_commits(all=True))
+                                        git_repo.get_list_commits(all=True))
                     else:
                         c_commits = set(c.hash for c in
-                                        pydriller.Git(git_repo_dir)
-                                                 .get_list_commits())
+                                        git_repo.get_list_commits())
                     if not p_commits.issubset(c_commits):
                         if prev_repository != git_repo.repo.remotes.origin.url:
                             raise Exception(("Found a database that was "
                                              "created with identical settings. "
                                              "However, some commits in the "
                                              "database are not in the provided "
                                              "git repository and the url of "
@@ -1653,38 +1749,38 @@
                                              "to the one listed in the "
                                              "database. Please provide a clean "
                                              "database or update the origin in "
                                              "the current database if you want "
                                              "to proceed."))
                     else:
                         if p_commits == c_commits:
-                            print("All commits have already been mined!")
+                            LOG.info("All commits have already been mined!")
                         else:
-                            print(("Found a matching database on provided "
-                                   "path. Skipping {} ({:.2f}%) of {} commits. "
-                                   "{} commits remaining.")
-                                  .format(len(p_commits),
-                                          len(p_commits)/len(c_commits)*100,
-                                          len(c_commits),
-                                          len(c_commits)-len(p_commits)))
+                            LOG.info('Found a matching database on provided path.')
+                            LOG.info('\t Skipping {} ({:.2f}%) of {} commits.'
+                                     .format(len(p_commits),
+                                             len(p_commits)/len(c_commits)*100,
+                                             len(c_commits)))
+                            LOG.info('\t {} commits remaining.'
+                                     .format(len(c_commits)-len(p_commits)))
                 else:
                     raise Exception(("Found a database on provided path that "
                                      "was created with settings not matching "
                                      "the ones selected for the current run. A "
                                      "path to either no database or a database "
                                      "from a previously paused run with "
                                      "identical settings is required."))
         except sqlite3.OperationalError:
             raise Exception(("Found a database on provided path that was "
                              "likely not created with git2net. A path to "
                              "either no database or a database from a "
                              "previously paused run with identical settings "
                              "is required."))
     else:
-        print("Found no database on provided path. Starting from scratch.")
+        LOG.info("Found no database on provided path. Starting from scratch.")
         try:
             repo_url = git_repo.repo.remotes.origin.url
         except:
             repo_url = git_repo_dir
 
         with sqlite3.connect(sqlite_db_file) as con:
             con.execute("""CREATE TABLE _metadata ('created with',
@@ -1710,60 +1806,59 @@
                          'extract_text': str(extract_text)})
             con.commit()
             p_commits = set()
 
     # commits in the currently mined repository
     if all_branches:
         c_commits = set(c.hash for c in
-                        pydriller.Git(git_repo_dir).get_list_commits(all=True))
+                        git_repo.get_list_commits(all=True))
     else:
         c_commits = set(c.hash for c in
-                        pydriller.Git(git_repo_dir).get_list_commits())
+                        git_repo.get_list_commits())
 
     if not commits:
         # unprocessed commits
         if all_branches:
             u_commits = [c for c in git_repo.get_list_commits(all=True) if
                          c.hash not in p_commits]
         else:
             u_commits = [c for c in git_repo.get_list_commits() if c.hash not
                          in p_commits]
     else:
         if not set(commits).issubset(c_commits):
-            raise Exception(("At least one provided commit does not exist in "
-                             "the repository."))
+            raise Exception(("At least one provided commit does not exist in the repository."))
         commits = [git_repo.get_commit(h) for h in commits]
         u_commits = [c for c in commits if c.hash not in p_commits]
 
     # Add information on commit being present in currently active branch
     current_branch = git_repo.repo.active_branch.name
     c_intersect = p_commits.intersection(c_commits)
     if len(c_intersect) > 0:
-        print(("Updated branch information for already mined commits that are "
-               "in the active branch."))
+        LOG.info(("Updated branch information for mined commits in the active branch."))
         for c in p_commits.intersection(c_commits):
             b = con.execute("""SELECT branches
                                FROM commits
                                WHERE hash = (:hash)""",
                             {'hash': c}).fetchall()[0][0]
             b = set(b.split(','))
             if current_branch not in b:
                 b.add(current_branch)
                 con.execute("""UPDATE commits
                                SET branches = (:branches)
                                WHERE hash = (:hash)""",
                             {'branches': ','.join(b), 'hash': c})
         con.commit()
-
-    if extraction_settings['no_of_processes'] > 1:
-        _process_repo_parallel(git_repo_dir, sqlite_db_file, u_commits,
-                               extraction_settings)
-    else:
-        _process_repo_serial(git_repo_dir, sqlite_db_file, u_commits,
-                             extraction_settings)
+     
+    if len(u_commits) > 0:
+        if extraction_settings['no_of_processes'] > 1:
+            _process_repo_parallel(git_repo_dir, sqlite_db_file, u_commits,
+                                   extraction_settings)
+        else:
+            _process_repo_serial(git_repo_dir, sqlite_db_file, u_commits,
+                                 extraction_settings)
 
 
 def mine_github(github_url, git_repo_dir, sqlite_db_file, branch=None,
                 **kwargs):
     """
     Clones a repository from github and starts the mining process.
 
@@ -1773,17 +1868,19 @@
     :param str branch: The branch of the github project that will be checked out and mined. If no branch is provided the default branch of the repository is used.
     :param \**kwargs: arguments that will be passed on to mine_git_repo
 
     :return:
         - git repository will be cloned to specified location
         - SQLite database will be written at specified location
     """
+    LOG = logging.getLogger('git2net')    
+    
     # github_url can either be provided as full url or as in form <USER>/<REPO>
     user_repo_pattern = r'^([^\/]*)\/([^\/]*)$'
-    full_url_pattern = r'^https:\/\/github\.com\/([^\/]*)\/([^\/i]*)(\.git)?$'
+    full_url_pattern = r'^https:\/\/github\.com\/([^\/]*)\/([^\/.]*)(\.git)?$'
 
     match = re.match(user_repo_pattern, github_url)
     if match:
         git_owner = match.groups()[0]
         git_repo = match.groups()[1]
         github_url = 'https://github.com/{}/{}'.format(git_owner, git_repo)
     else:
@@ -1802,16 +1899,16 @@
         local_directory = '.'
     if git_repo_folder == '':
         git_repo_folder = git_owner + '__' + git_repo
 
     # check if the folder is empty if it exists
     if os.path.exists(git_repo_dir) and \
        (len(os.listdir(os.path.join(local_directory, git_repo_folder))) > 0):
-        print(("Provided folder is not empty. Skipping the cloning and trying "
-               "to resume."))
+        LOG.info('Provided folder is not empty.')
+        LOG.info('\t Skipping the cloning and trying to resume.')
     else:
         if branch:
             git.Git(local_directory).clone(github_url, git_repo_folder,
                                            branch=branch)
         else:
             git.Git(local_directory).clone(github_url, git_repo_folder)
```

### Comparing `git2net-1.6.3/git2net/helpers/binary-extensions/binary-extensions.json` & `git2net-1.7.0/git2net/helpers/binary-extensions/binary-extensions.json`

 * *Files identical despite different names*

### Comparing `git2net-1.6.3/git2net/visualisation.py` & `git2net-1.7.0/git2net/visualisation.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 import pathpy as pp
 import sqlite3
 import datetime
 from tqdm import tqdm
 import math
 import numpy as np
 import calendar
+import networkx as nx
 
+import logging
 
 def _ensure_author_id_exists(sqlite_db_file):
     with sqlite3.connect(sqlite_db_file) as con:
         cur = con.cursor()
         cols = [i[1] for i in cur.execute('PRAGMA table_info(commits)')]
         if 'author_id' not in cols:
             raise Exception("The author_id is not yet computed. To use author_id as identifier, please " + 
                             "run git2net.disambiguate_aliases_db on the database before visualisation.")
         elif pd.isnull(pd.read_sql('''SELECT author_id FROM commits''', con).author_id).sum() > 0:
             raise Exception("The author_id is missing entries. To use author_id as identifier, please " + 
                             "rerun git2net.disambiguate_aliases_db on the database before visualisation.")
-                
+    return True
                 
 def get_line_editing_paths(sqlite_db_file, git_repo_dir, author_identifier='author_id', commit_hashes=None,
                            file_paths=None, with_start=False, merge_renaming=False):
     """
     Returns line editing DAG as well as line editing paths.
 
     :param str sqlite_db_file: path to SQLite database mined with git2net line method
@@ -43,14 +45,16 @@
     :return:
         - *pathpy.Paths* – line editing paths
         - *pathpy.DAG* – line editing directed acyclic graph
         - *dict* – info on node charactaristics
         - *dict* – info on edge characteristics
     """
 
+    LOG = logging.getLogger('git2net')
+    
     if author_identifier == 'author_id':
         _ensure_author_id_exists(sqlite_db_file)
     
     # Connect to provided database.
     con = sqlite3.connect(sqlite_db_file)
 
     # Check if database is valid.
@@ -64,30 +68,30 @@
         raise Exception("You either provided no database or a database not created with git2net. " +
                         "Please provide a valid datatabase mined with 'use_blocks=False'.")
 
     if file_paths is not None:
         assert type(file_paths) is list
 
     if merge_renaming:
-        print('Searching for aliases')
+        LOG.info('Searching for aliases')
         # Identify files that have been renamed.
         _, aliases = identify_file_renaming(git_repo_dir)
 
     dag = pp.DAG()
     node_info = {}
     node_info['colors'] = {}
     node_info['time'] = {}
     # node_info['file_paths'] = {}
     # node_info['edit_distance'] = {}
     edge_info = {}
     edge_info['colors'] = {}
     edge_info['weights'] = {}
 
     # Extract required data from the provided database.
-    print('Querying commits')
+    LOG.info('Querying commits')
     if author_identifier == 'author_id':
         commits = pd.read_sql("""SELECT hash,
                                         author_id as author_identifier,
                                         author_date
                                  FROM commits""", con)
     elif author_identifier == 'author_name':
         commits = pd.read_sql("""SELECT hash,
@@ -98,15 +102,15 @@
         commits = pd.read_sql("""SELECT hash,
                                         author_email as author_identifier,
                                         author_date
                                  FROM commits""", con)
     else:
         raise Exception("author_identifier must be from {'author_id', 'author_name', 'author_email'}.")
     
-    print('Querying edits')
+    LOG.info('Querying edits')
     edits = pd.DataFrame()
     no_of_edits = pd.read_sql("""SELECT count(*) FROM edits""", con).iloc[0, 0]
     chunksize = 1000
     for edits in tqdm(pd.read_sql("""SELECT levenshtein_dist,
                                             old_path,
                                             new_path,
                                             commit_hash,
@@ -149,18 +153,14 @@
 
         # Get current author and date
         edits = pd.merge(edits, commits, how='left', left_on='commit_hash',
                                 right_on='hash').drop(['hash'], axis=1)
 
         file_paths_dag = set()
 
-        # Sort edits by author date.
-        #print('Sorting edits')
-        #edits.sort_values('author_date', ascending=True, inplace=True)
-
         for _, edit in edits.iterrows():
             if edit.edit_type == 'replacement':
                 # Generate name of target node.
                 target = 'L' + str(int(float(edit.post_starting_line_no))) + ' ' + \
                         edit.new_path + ' ' + \
                         edit.commit_hash
 
@@ -224,16 +224,17 @@
                     edge_info['colors'][(source_addition, target)] = '#FBB13C'
                     edge_info['weights'][(source_addition, target)] = edit.levenshtein_dist
                     node_info['time'][target] = edit.author_date
                     node_info['time'][source_addition] = edit.author_date_addition
             elif edit.edit_type == 'file_renaming' or edit.edit_type == 'binary_file_change':
                 pass
             else:
-                raise Exception("Unexpected error in 'extract_editing_paths'. ({})"
-                                    .format(edit.edit_type))
+                raise Exception("Unexpected error in 'extract_editing_paths' ({})."
+                                    .format(edit.edit_type) + " Please report on " +
+                                "https://github.com/gotec/git2net.")
 
     for node in tqdm(dag.nodes):
         if node in file_paths_dag:
             node_info['colors'][node] = 'gray'
         else:
             if '#FBB13C' in [edge_info['colors'][n] for n in [(x, node)
                                                     for x in dag.predecessors[node]]]:
@@ -316,15 +317,15 @@
     dag.topsort()
 
     assert dag.is_acyclic is True
 
     return dag, node_info, edge_info
 
 
-def get_coediting_network(sqlite_db_file, author_identifier='author_id', time_from=None, time_to=None):
+def get_coediting_network(sqlite_db_file, author_identifier='author_id', time_from=None, time_to=None, engine='pathpy'):
     """
     Returns coediting network containing links between authors who coedited at least one line of
     code within a given time window.
 
     :param str sqlite_db_file: path to SQLite database
     :param datetime.datetime time_from: start time of time window filter
     :param datetime.datetime time_to: end time of time window filter
@@ -387,27 +388,49 @@
         time_to = max(data.time)
     else:
         time_to = int(calendar.timegm(time_to.timetuple()))
 
     node_info = {}
     edge_info = {}
     
-    t = pp.TemporalNetwork()
-    for row in data.itertuples():
-        if (row.time >= time_from) and (row.time <= time_to) and not \
-           (row.post_author == row.pre_author):
-            if not (pd.isnull(row.post_author) or pd.isnull(row.pre_author)):
-                t.add_edge(row.post_author,
-                           row.pre_author,
-                           row.time,
-                           directed=True)
-
-    return t, node_info, edge_info
-
-
+    if engine=='pathpy':
+        t = pp.TemporalNetwork()
+        for row in data.itertuples():
+            if (row.time >= time_from) and (row.time <= time_to) and not \
+               (row.post_author == row.pre_author):
+                if not (pd.isnull(row.post_author) or pd.isnull(row.pre_author)):
+                    t.add_edge(row.post_author,
+                               row.pre_author,
+                               row.time,
+                               directed=True)
+
+        return t, node_info, edge_info
+    elif engine=='networkx':
+        n = nx.DiGraph()
+        for row in data.itertuples():
+            if (row.time >= time_from) and (row.time <= time_to) and not \
+               (row.post_author == row.pre_author):
+                if not (pd.isnull(row.post_author) or pd.isnull(row.pre_author)):
+                    n.add_node(row.post_author)
+                    n.add_node(row.pre_author)
+                    n.add_edge(row.post_author,
+                               row.pre_author)
+                    if author_identifier=='author_id':
+                        edge = (int(row.post_author), int(row.pre_author))
+                    else:
+                        edge = (row.post_author, row.pre_author)
+                    
+                    if edge in edge_info:
+                        edge_info[edge]['times'].append(row.time)
+                    else:
+                        edge_info[edge] = {'times': [row.time]}
+        return n, node_info, edge_info
+    else:
+        raise Exception('Not implemented network engine.')
+    
 def get_coauthorship_network(sqlite_db_file, author_identifier='author_id', time_from=None, time_to=None):
     """
     Returns coauthorship network containing links between authors who coedited at least one code
     file within a given time window.
 
     :param str sqlite_db_file: path to SQLite database
     :param datetime.datetime time_from: start time of time window filter
```

### Comparing `git2net-1.6.3/git2net.egg-info/PKG-INFO` & `git2net-1.7.0/git2net.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2net
-Version: 1.6.3
+Version: 1.7.0
 Summary: An OpenSource Python package for the extraction of fine-grained and time-stamped co-editing networks from git repositories.
 Home-page: https://gotec.github.io/git2net/
 Author: Christoph Gote
 Author-email: cgote@ethz.ch
 License: AGPL-3.0+
 Keywords: co-editing,networks,repository,mining,network,analysis
 Classifier: Programming Language :: Python :: 3
```

### Comparing `git2net-1.6.3/setup.cfg` & `git2net-1.7.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = git2net
-version = 1.6.3
+version = 1.7.0
 author = Christoph Gote
 author_email = cgote@ethz.ch
 license = AGPL-3.0+
 description = An OpenSource Python package for the extraction of fine-grained and time-stamped co-editing networks from git repositories.
 keywords = 
 	co-editing
 	networks
@@ -26,15 +26,15 @@
 	pandas
 	tqdm>=4.27.0
 	numpy
 	scipy
 	python-levenshtein
 	pathpy2>=2.2.0
 	lizard
-	pydriller>=2.0.0
+	pydriller>=2.0.0,<2.2.0
 	gambit-disambig
 	setuptools
 	pygments
 
 [options.entry_points]
 console_scripts = git2net = git2net.command_line:main
```

