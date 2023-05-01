# Comparing `tmp/gpt-review-0.0.1rc95.post1.tar.gz` & `tmp/gpt-review-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.0.1rc95.post1.tar", last modified: Thu Apr 27 03:51:20 2023, max compression
+gzip compressed data, was "gpt-review-0.2.3.tar", last modified: Mon May  1 21:42:12 2023, max compression
```

## Comparing `gpt-review-0.0.1rc95.post1.tar` & `gpt-review-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0      336 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1333 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      697 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0      747 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      866 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.pypirc
--rw-r--r--   0        0        0      816 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/LICENSE
--rw-r--r--   0        0        0      733 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/README.md
--rw-r--r--   0        0        0     5116 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/action.yml
--rw-r--r--   0        0        0     6847 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/review.py
--rw-r--r--   0        0        0      363 2023-04-27 03:51:19.712891 gpt-review-0.0.1rc95.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0     5796 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      413 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0      792 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/tests/conftest.py
--rw-r--r--   0        0        0     1193 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 gpt-review-0.0.1rc95.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1464 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     4520 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      898 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-01 21:42:05.100027 gpt-review-0.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-01 21:42:05.100027 gpt-review-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1615 2023-05-01 21:42:05.100027 gpt-review-0.2.3/README.md
+-rw-r--r--   0        0        0     5206 2023-05-01 21:42:05.100027 gpt-review-0.2.3/action.yml
+-rw-r--r--   0        0        0     8232 2023-05-01 21:42:05.100027 gpt-review-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-05-01 21:42:05.100027 gpt-review-0.2.3/review.py
+-rw-r--r--   0        0        0      352 2023-05-01 21:42:11.916126 gpt-review-0.2.3/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11461 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      464 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      413 2023-05-01 21:42:05.100027 gpt-review-0.2.3/src/gpt_review/main.py
+-rw-r--r--   0        0        0     1281 2023-05-01 21:42:05.100027 gpt-review-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0     5449 2023-05-01 21:42:05.100027 gpt-review-0.2.3/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     3602 1970-01-01 00:00:00.000000 gpt-review-0.2.3/PKG-INFO
```

### Comparing `gpt-review-0.0.1rc95.post1/.devcontainer/devcontainer.json` & `gpt-review-0.2.3/.devcontainer/devcontainer.json`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,20 @@
 		"ms-python.black-formatter",
 		"ms-vsliveshare.vsliveshare",
 		"ryanluker.vscode-coverage-gutters",
 		"bungcip.better-toml",
 		"GitHub.copilot",
 		"GitHub.vscode-github-actions",
 		"ms-vscode.azurecli",
-		"ms-vscode.azure-account"
+		"ms-vscode.azure-account",
+		"zokugun.explicit-folding",
+		"MaxKless.git-squash-all",
+		"GitHub.copilot-labs",
+		"GitHub.codespaces",
+		"charliermarsh.ruff"
 	],
       "settings": {
         "python.defaultInterpreterPath": "/usr/local/bin/python",
         "black-formatter.path": [
           "/usr/local/py-utils/bin/black"
         ],
         "pylint.path": [
```

### Comparing `gpt-review-0.0.1rc95.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.2.3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc95.post1/.github/pull_request_template.md` & `gpt-review-0.2.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc95.post1/.github/workflows/test-action.yml` & `gpt-review-0.2.3/.github/workflows/test-action.yml`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     name: OpenAI PR Comment
     steps:
       - uses: actions/checkout@v3
         with:
           ref: ${{ github.event.pull_request.head.sha }}
           fetch-depth: 2
       - uses: ./ # dciborow/action-gpt@0.0.3
+        continue-on-error: true
         with:
           GIT_COMMIT_HASH: ${{ github.event.pull_request.head.sha }}
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
           OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
           OPENAI_ORG_KEY: ${{ secrets.OPENAI_ORG_KEY }}
           PR_NUMBER: ${{ github.event.pull_request.number }}
           PR_TITLE: ${{ github.event.pull_request.title }}
```

### Comparing `gpt-review-0.0.1rc95.post1/.gitignore` & `gpt-review-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc95.post1/.vscode/settings.json` & `gpt-review-0.2.3/.vscode/settings.json`

 * *Files 24% similar despite different names*

```diff
@@ -44,8 +44,28 @@
 000002b0: 616b 6538 2e61 7267 7322 3a20 5b0a 2020  ake8.args": [.  
 000002c0: 2020 2020 2020 222d 2d74 6f6d 6c2d 636f        "--toml-co
 000002d0: 6e66 6967 3d70 7970 726f 6a65 6374 2e74  nfig=pyproject.t
 000002e0: 6f6d 6c22 0a20 2020 205d 2c0a 2020 2020  oml".    ],.    
 000002f0: 2269 736f 7274 2e61 7267 7322 3a20 5b0a  "isort.args": [.
 00000300: 2020 2020 2020 2020 222d 2d73 6574 7469          "--setti
 00000310: 6e67 732d 7061 7468 3d70 7970 726f 6a65  ngs-path=pyproje
-00000320: 6374 2e74 6f6d 6c22 0a20 2020 205d 0a7d  ct.toml".    ].}
+00000320: 6374 2e74 6f6d 6c22 0a20 2020 205d 2c0a  ct.toml".    ],.
+00000330: 2020 2020 2270 7974 686f 6e2e 6c69 6e74      "python.lint
+00000340: 696e 672e 6261 6e64 6974 456e 6162 6c65  ing.banditEnable
+00000350: 6422 3a20 7472 7565 2c0a 2020 2020 2270  d": true,.    "p
+00000360: 7974 686f 6e2e 6c69 6e74 696e 672e 6261  ython.linting.ba
+00000370: 6e64 6974 4172 6773 223a 205b 0a20 2020  nditArgs": [.   
+00000380: 2020 2020 2022 2d63 222c 0a20 2020 2020       "-c",.     
+00000390: 2020 2022 7079 7072 6f6a 6563 742e 746f     "pyproject.to
+000003a0: 6d6c 220a 2020 2020 5d2c 0a20 2020 2022  ml".    ],.    "
+000003b0: 7079 7468 6f6e 2e61 6e61 6c79 7369 732e  python.analysis.
+000003c0: 696e 6c61 7948 696e 7473 2e66 756e 6374  inlayHints.funct
+000003d0: 696f 6e52 6574 7572 6e54 7970 6573 223a  ionReturnTypes":
+000003e0: 2074 7275 652c 0a20 2020 2022 7079 7468   true,.    "pyth
+000003f0: 6f6e 2e61 6e61 6c79 7369 732e 6469 6167  on.analysis.diag
+00000400: 6e6f 7374 6963 5365 7665 7269 7479 4f76  nosticSeverityOv
+00000410: 6572 7269 6465 7322 3a20 7b0a 2020 2020  errides": {.    
+00000420: 2020 2020 2272 6570 6f72 7455 6e64 6566      "reportUndef
+00000430: 696e 6564 5661 7269 6162 6c65 223a 2022  inedVariable": "
+00000440: 6e6f 6e65 2220 2f2f 2043 6f76 6572 6564  none" // Covered
+00000450: 2062 7920 5275 6666 2046 3832 310a 2020   by Ruff F821.  
+00000460: 2020 7d0a 7d                               }.}
```

### Comparing `gpt-review-0.0.1rc95.post1/LICENSE` & `gpt-review-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc95.post1/action.yml` & `gpt-review-0.2.3/action.yml`

 * *Files 3% similar despite different names*

```diff
@@ -126,26 +126,28 @@
         if: ${{ github.action_ref == '' }}
         run: echo "BRANCH=$(echo ${GITHUB_HEAD_REF:-${GITHUB_REF##*/}})" >> $GITHUB_ENV
 
       - name: Review PR and make comment
         shell: bash
         run: |
           source .env/bin/activate
-
-          curl --request GET --url https://raw.githubusercontent.com/microsoft/ask-gpt/$ACTION_REF/review.py > review.py
+          
+          ORG_NAME=$(echo ${BRANCH%/*})
+          curl --request GET --url https://raw.githubusercontent.com/$ORG_NAME/gpt-review/$ACTION_REF/review.py > review.py
 
           python review.py
         env:
           ACTION_REF: ${{ github.action_ref || env.BRANCH }}
           GIT_COMMIT_HASH: ${{ inputs.GIT_COMMIT_HASH }}
           GITHUB_TOKEN: ${{ inputs.GITHUB_TOKEN }}
           LINK: "https://github.com/${{ inputs.REPOSITORY_NAME }}/pull/${{ inputs.PR_NUMBER }}"
           OPENAI_API_KEY: ${{ inputs.OPENAI_API_KEY }}
           OPENAI_ORG_KEY: ${{ inputs.OPENAI_ORG_KEY }}
           PR_TITLE: ${{ inputs.PR_TITLE }}
+          BRANCH:  ${{ env.BRANCH }}
           AZURE_OPENAI_API_KEY: ${{ inputs.AZURE_OPENAI_API_KEY || '' }}
           AZURE_OPENAI_API: ${{ inputs.AZURE_OPENAI_API || '' }}
           PATCH_PR: ${{ github.event.pull_request.number }}
           PATCH_REPO: ${{ github.repository }}
           FULL_SUMMARY: ${{ inputs.FULL_SUMMARY }}
           FILE_SUMMARY: ${{ inputs.FILE_SUMMARY }}
           TEST_SUMMARY: ${{ inputs.TEST_SUMMARY }}
```

### Comparing `gpt-review-0.0.1rc95.post1/pyproject.toml` & `gpt-review-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -31,24 +31,24 @@
   'openai',
   'requests',
   "pyyaml",
 ]
 
 [project.optional-dependencies]
 test = [
-    "bandit[toml]==1.7.4",
-    "black==23.1.0",
-    "check-manifest==0.48",
-    "flake8-bugbear==23.3.12",
+    "bandit[toml]==1.7.5",
+    "black==23.3.0",
+    "check-manifest==0.49",
+    "flake8-bugbear==23.3.23",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8",
     "flake8-pyproject",
-    "pre-commit==2.17.0",
-    "pylint==2.17.0",
+    "pre-commit==3.2.2",
+    "pylint==2.17.3",
     "pylint_junit",
     "pytest-cov>=3.0.0",
     "pytest-mock",
     "pytest-runner",
     "pytest>=7.2.2",
     "pytest-github-actions-annotate-failures",
     "shellcheck-py==0.9.0.2"
@@ -96,15 +96,20 @@
     "tests",
     "swagger_client"
 ]
 ignore = [
     "E722",
     "B001",
     "W503",
-    "E203"
+    "E203",
+    # Covered by Ruff
+    "F401",
+    "F501",
+    "F821",
+    "W391", # Covered by Pylint trailing-newlines
 ]
 
 [tool.pyright]
 include = ["src"]
 exclude = [
     "**/node_modules",
     "**/__pycache__",
@@ -186,15 +191,19 @@
 limit-inference-results=100
 persistent="yes"
 suggestion-mode="yes"
 unsafe-load-any-extension="no"
 
 [tool.pylint.'MESSAGES CONTROL']
 enable="c-extension-no-member"
-
+disable = [
+    "unused-import", # Covered by Ruff F401
+    "undefined-variable", # Covered by Ruff F821
+    "line-too-long", # Covered by Ruff E501
+]
 [tool.pylint.'REPORTS']
 evaluation="10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10)"
 output-format="text"
 reports="no"
 score="yes"
 
 [tool.pylint.'REFACTORING']
@@ -321,7 +330,53 @@
 deprecated-modules="optparse,tkinter.tix"
 
 [tool.pylint.'EXCEPTIONS']
 overgeneral-exceptions= [
     "BaseException",
     "Exception"
 ]
+
+[tool.ruff]
+# Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
+select = ["E", "F"]
+ignore = []
+
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F", "G", "I", "N", "Q", "S", "T", "W", "ANN", "ARG", "BLE", "COM", "DJ", "DTZ", "EM", "ERA", "EXE", "FBT", "ICN", "INP", "ISC", "NPY", "PD", "PGH", "PIE", "PL", "PT", "PTH", "PYI", "RET", "RSE", "RUF", "SIM", "SLF", "TCH", "TID", "TRY", "UP", "YTT"]
+unfixable = []
+
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".bzr",
+    ".direnv",
+    ".eggs",
+    ".git",
+    ".hg",
+    ".mypy_cache",
+    ".nox",
+    ".pants.d",
+    ".pytype",
+    ".ruff_cache",
+    ".svn",
+    ".tox",
+    ".venv",
+    "__pypackages__",
+    "_build",
+    "buck-out",
+    "build",
+    "dist",
+    "node_modules",
+    "venv",
+]
+
+# Same as Black.
+line-length = 120
+
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+
+# Assume Python 3.10.
+target-version = "py311"
+
+[tool.ruff.mccabe]
+# Unlike Flake8, default to a complexity level of 10.
+max-complexity = 10
```

### Comparing `gpt-review-0.0.1rc95.post1/review.py` & `gpt-review-0.2.3/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc95.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.2.3/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

