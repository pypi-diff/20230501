# Comparing `tmp/github-policies-0.1.0.tar.gz` & `tmp/github-policies-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github-policies-0.1.0.tar", last modified: Fri Apr 21 10:07:14 2023, max compression
+gzip compressed data, was "github-policies-0.2.0.tar", last modified: Mon May  1 07:47:07 2023, max compression
```

## Comparing `github-policies-0.1.0.tar` & `github-policies-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:07:14.034899 github-policies-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-21 10:07:14.034899 github-policies-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-21 10:07:03.000000 github-policies-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-21 10:07:03.000000 github-policies-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:07:14.034899 github-policies-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:07:14.034899 github-policies-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:07:14.034899 github-policies-0.1.0/src/ghpolicy/
--rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-04-21 10:07:03.000000 github-policies-0.1.0/src/ghpolicy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-04-21 10:07:03.000000 github-policies-0.1.0/src/ghpolicy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:07:14.034899 github-policies-0.1.0/src/ghpolicy/policies/
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-21 10:07:03.000000 github-policies-0.1.0/src/ghpolicy/policies/default_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-21 10:07:03.000000 github-policies-0.1.0/src/ghpolicy/policies/team_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-21 10:07:03.000000 github-policies-0.1.0/src/ghpolicy/policies/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-21 10:07:03.000000 github-policies-0.1.0/src/ghpolicy/policies/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-21 10:07:03.000000 github-policies-0.1.0/src/ghpolicy/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:07:14.034899 github-policies-0.1.0/src/github_policies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-21 10:07:14.000000 github-policies-0.1.0/src/github_policies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 10:07:14.000000 github-policies-0.1.0/src/github_policies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:07:14.000000 github-policies-0.1.0/src/github_policies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 10:07:14.000000 github-policies-0.1.0/src/github_policies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 10:07:14.000000 github-policies-0.1.0/src/github_policies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 10:07:14.000000 github-policies-0.1.0/src/github_policies.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:47:07.004837 github-policies-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 07:47:07.004837 github-policies-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-01 07:46:58.000000 github-policies-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-01 07:46:58.000000 github-policies-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 07:47:07.004837 github-policies-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:47:07.000837 github-policies-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:47:07.000837 github-policies-0.2.0/src/ghpolicy/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      319 2023-05-01 07:46:58.000000 github-policies-0.2.0/src/ghpolicy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-01 07:46:58.000000 github-policies-0.2.0/src/ghpolicy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:47:07.000837 github-policies-0.2.0/src/ghpolicy/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-01 07:46:58.000000 github-policies-0.2.0/src/ghpolicy/policies/default_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-01 07:46:58.000000 github-policies-0.2.0/src/ghpolicy/policies/repository_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-01 07:46:58.000000 github-policies-0.2.0/src/ghpolicy/policies/team_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-01 07:46:58.000000 github-policies-0.2.0/src/ghpolicy/policies/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-01 07:46:58.000000 github-policies-0.2.0/src/ghpolicy/policies/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-01 07:46:58.000000 github-policies-0.2.0/src/ghpolicy/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 07:47:07.004837 github-policies-0.2.0/src/github_policies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-01 07:47:06.000000 github-policies-0.2.0/src/github_policies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-01 07:47:07.000000 github-policies-0.2.0/src/github_policies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 07:47:06.000000 github-policies-0.2.0/src/github_policies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-01 07:47:06.000000 github-policies-0.2.0/src/github_policies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-01 07:47:06.000000 github-policies-0.2.0/src/github_policies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-01 07:47:06.000000 github-policies-0.2.0/src/github_policies.egg-info/top_level.txt
```

### Comparing `github-policies-0.1.0/pyproject.toml` & `github-policies-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Same as Black.
 line-length = 88
 
 [project]
 name = "github-policies"
 description = "Automate GitHub repository settings."
 readme = "README.md"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     {name = "Lab Digital", email = "opensource@labdigital.nl"},
 ]
 dependencies = [
     "PyGithub>=1.58.1",
     "click>=8.1.3",
     "PyYAML>=6.0",
```

### Comparing `github-policies-0.1.0/src/ghpolicy/main.py` & `github-policies-0.2.0/src/ghpolicy/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import functools
 import os
 import re
 
 import github
-from github.Organization import Organization
-from github.Repository import Repository
-
+from ghpolicy.policies.repository_settings import RepositorySettingsPolicy
 from ghpolicy.policies.team_permission import TeamPermissionsPolicy
 from ghpolicy.policies.topics import TopicsContainsPolicy
 from ghpolicy.policies.visibility import VisibilityInternalPolicy
 from ghpolicy.policy import PolicyApplicator
+from github.Organization import Organization
+from github.Repository import Repository
 
 PolicyApplicator.register("visibility-internal", VisibilityInternalPolicy)
+PolicyApplicator.register("repository-settings", RepositorySettingsPolicy)
 PolicyApplicator.register("topics-contains", TopicsContainsPolicy)
 PolicyApplicator.register("team-permissions", TeamPermissionsPolicy)
 
 
 class Rule:
     def __init__(self, name: str, applicator: PolicyApplicator):
         self.name = name
@@ -51,18 +52,17 @@
     token = os.environ.get("GITHUB_TOKEN")
     if not token:
         raise Exception("GITHUB_TOKEN environment variable not set")
 
     gh = github.Github(token)
     org = gh.get_organization(data["organization"])
     for repo in org.get_repos():
+        print("Processing %s" % repo.name)
         matching = [rule for rule in rules if rule.match(repo.name)]
         if not matching:
             continue
 
         if len(matching) > 1:
-            print("Multiple rules matched", repo.name, matching)
             rule = functools.reduce(Rule.merge, matching)
             rule.apply(org, repo, dry_run=dry_run)
         else:
-            print("Matched", repo.name, matching[0])
             matching[0].apply(org, repo, dry_run=dry_run)
```

### Comparing `github-policies-0.1.0/src/ghpolicy/policies/default_branch.py` & `github-policies-0.2.0/src/ghpolicy/policies/default_branch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from ghpolicy.policy import BasePolicy
 from github.Organization import Organization
 from github.Repository import Repository
 
-from ghpolicy.policy import BasePolicy
-
 
 class DefaultBranch(BasePolicy):
     def apply(self, org: Organization, repo: Repository, dry_run: bool = False):
         """Make sure the default branch is called main and that the master
         branch is deleted.
 
         """
```

### Comparing `github-policies-0.1.0/src/ghpolicy/policies/team_permission.py` & `github-policies-0.2.0/src/ghpolicy/policies/team_permission.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import copy
 
+from ghpolicy.policy import BasePolicy
 from github.GithubException import UnknownObjectException
 from github.Organization import Organization
 from github.Repository import Repository
 from github.Team import Team
 
-from ghpolicy.policy import BasePolicy
-
 
 class TeamPermissionsPolicy(BasePolicy):
     def __init__(self, options: list[dict[str, str]]):
         self.options = options
 
     def merge(self, other: "TeamPermissionsPolicy") -> "TeamPermissionsPolicy":
         data = copy.deepcopy(self.options)
@@ -56,17 +55,15 @@
                 continue
 
             if dry_run:
                 print(
                     f"Would add {team.name} to {repo.name} with {permission} permission"
                 )
             else:
-                print(
-                    f"Adding {team.name} to {repo.name} with {permission} permission"
-                )
+                print(f"Adding {team.name} to {repo.name} with {permission} permission")
                 team.set_repo_permission(repo, self.map_permission(permission))
 
     def map_permission(self, permission: str) -> str:
         map_permissions = {
             "read": "pull",
             "write": "push",
         }
```

### Comparing `github-policies-0.1.0/src/ghpolicy/policies/topics.py` & `github-policies-0.2.0/src/ghpolicy/policies/topics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import copy
 
+from ghpolicy.policy import BasePolicy
 from github.Organization import Organization
 from github.Repository import Repository
 
-from ghpolicy.policy import BasePolicy
-
 
 class TopicsContainsPolicy(BasePolicy):
     def __init__(self, options: list[str]):
         self.options = options
 
     def apply(self, org: Organization, repo: Repository, dry_run: bool = False):
         pass
```

### Comparing `github-policies-0.1.0/src/ghpolicy/policies/visibility.py` & `github-policies-0.2.0/src/ghpolicy/policies/visibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from ghpolicy.policy import BasePolicy
 from github.Organization import Organization
 from github.Repository import Repository
 
-from ghpolicy.policy import BasePolicy
-
 
 class VisibilityInternalPolicy(BasePolicy):
     def merge(self, other: "VisibilityInternalPolicy") -> "VisibilityInternalPolicy":
         return VisibilityInternalPolicy(None)
 
     def apply(self, org: Organization, repo: Repository, dry_run: bool = False):
         """Make sure the repository is correctly set to private or internal.
```

### Comparing `github-policies-0.1.0/src/ghpolicy/policy.py` & `github-policies-0.2.0/src/ghpolicy/policy.py`

 * *Files identical despite different names*

