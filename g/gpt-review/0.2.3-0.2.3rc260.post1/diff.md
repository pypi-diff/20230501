# Comparing `tmp/gpt-review-0.2.3.tar.gz` & `tmp/gpt-review-0.2.3rc260.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.2.3.tar", last modified: Mon May  1 21:42:12 2023, max compression
+gzip compressed data, was "gpt-review-0.2.3rc260.post1.tar", last modified: Mon May  1 21:55:08 2023, max compression
```

## Comparing `gpt-review-0.2.3.tar` & `gpt-review-0.2.3rc260.post1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      336 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1464 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     4520 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      898 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.gitignore
--rw-r--r--   0        0        0      158 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-01 21:42:05.100027 gpt-review-0.2.3/LICENSE
--rw-r--r--   0        0        0     1615 2023-05-01 21:42:05.100027 gpt-review-0.2.3/README.md
--rw-r--r--   0        0        0     5206 2023-05-01 21:42:05.100027 gpt-review-0.2.3/action.yml
--rw-r--r--   0        0        0     8232 2023-05-01 21:42:05.100027 gpt-review-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-05-01 21:42:05.100027 gpt-review-0.2.3/review.py
--rw-r--r--   0        0        0      352 2023-05-01 21:42:11.916126 gpt-review-0.2.3/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11461 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      464 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/constants.py
--rw-r--r--   0        0        0      413 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/main.py
--rw-r--r--   0        0        0     1281 2023-05-01 21:42:05.100027 gpt-review-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     5449 2023-05-01 21:42:05.100027 gpt-review-0.2.3/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     3602 1970-01-01 00:00:00.000000 gpt-review-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1464 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2146 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4577 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      898 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/LICENSE
+-rw-r--r--   0        0        0     1615 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/README.md
+-rw-r--r--   0        0        0     5206 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/action.yml
+-rw-r--r--   0        0        0     8232 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/review.py
+-rw-r--r--   0        0        0      364 2023-05-01 21:55:07.710770 gpt-review-0.2.3rc260.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11461 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      464 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      413 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     1281 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/tests/conftest.py
+-rw-r--r--   0        0        0     5449 2023-05-01 21:55:00.014441 gpt-review-0.2.3rc260.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 gpt-review-0.2.3rc260.post1/PKG-INFO
```

### Comparing `gpt-review-0.2.3/.devcontainer/devcontainer.json` & `gpt-review-0.2.3rc260.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.2.3rc260.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/.github/dependabot.yml` & `gpt-review-0.2.3rc260.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/.github/pull_request_template.md` & `gpt-review-0.2.3rc260.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/.github/workflows/codeql.yml` & `gpt-review-0.2.3rc260.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/.github/workflows/dependency-review.yml` & `gpt-review-0.2.3rc260.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/.github/workflows/python.yml` & `gpt-review-0.2.3rc260.post1/.github/workflows/python.yml`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,19 @@
           pypi_password: ${{ secrets.PYPI_PASSWORD }}
           workdir: '.'
           python_version: '3.11.3'
 
       - uses: EndBug/add-and-commit@v9
         if: ${{ github.event_name == 'release' }}
         with:
-          message: Update Version to ${{ steps.tag_version.outputs.new_version }} [no ci]
+          message: Update Version to ${{ steps.tag_version.outputs.previous_version }} [no ci]
           committer_name: GitHub Actions
           committer_email: actions@github.com
           add: src/gpt_review/__init__.py
+          push: origin HEAD:main --force-with-lease
 
   coverage-unit:
     runs-on: ubuntu-latest
     env:
       OS: 'ubuntu-latest'
       PYTHON: '3.11'
     steps:
```

### Comparing `gpt-review-0.2.3/.github/workflows/test-action.yml` & `gpt-review-0.2.3rc260.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/.gitignore` & `gpt-review-0.2.3rc260.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/.vscode/settings.json` & `gpt-review-0.2.3rc260.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/LICENSE` & `gpt-review-0.2.3rc260.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/README.md` & `gpt-review-0.2.3rc260.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/action.yml` & `gpt-review-0.2.3rc260.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/pyproject.toml` & `gpt-review-0.2.3rc260.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/review.py` & `gpt-review-0.2.3rc260.post1/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/src/gpt_review/_ask.py` & `gpt-review-0.2.3rc260.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/src/gpt_review/_gpt_cli.py` & `gpt-review-0.2.3rc260.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/tests/conftest.py` & `gpt-review-0.2.3rc260.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/tests/test_gpt_cli.py` & `gpt-review-0.2.3rc260.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.2.3/PKG-INFO` & `gpt-review-0.2.3rc260.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.2.3
+Version: 0.2.3rc260.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3 Summary: Python Project
-for reviewing GitHub PRs with Open AI and Chat-GPT. Author-email: Daniel
-Ciborowski
+Metadata-Version: 2.1 Name: gpt-review Version: 0.2.3rc260.post1 Summary:
+Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
+email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Requires-Dist: azure-identity Requires-Dist: azure-keyvault-
```

