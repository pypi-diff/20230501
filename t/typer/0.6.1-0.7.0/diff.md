# Comparing `tmp/typer-0.6.1.tar.gz` & `tmp/typer-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer-0.6.1.tar", last modified: Tue Jul 12 20:30:38 2022, max compression
+gzip compressed data, was "typer-0.7.0.tar", last modified: Sat Nov  5 19:43:52 2022, max compression
```

## Comparing `typer-0.6.1.tar` & `typer-0.7.0.tar`

### file list

```diff
@@ -1,485 +1,486 @@
--rw-r--r--   0        0        0       66 2022-07-12 20:30:16.582644 typer-0.6.1/.coveragerc
--rw-r--r--   0        0        0       19 2022-07-12 20:30:16.582644 typer-0.6.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      145 2022-07-12 20:30:16.582644 typer-0.6.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     6218 2022-07-12 20:30:16.582644 typer-0.6.1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     5288 2022-07-12 20:30:16.582644 typer-0.6.1/.github/ISSUE_TEMPLATE/question.yml
--rw-r--r--   0        0        0      115 2022-07-12 20:30:16.586644 typer-0.6.1/.github/actions/comment-docs-preview-in-pr/Dockerfile
--rw-r--r--   0        0        0      394 2022-07-12 20:30:16.586644 typer-0.6.1/.github/actions/comment-docs-preview-in-pr/action.yml
--rw-r--r--   0        0        0     2074 2022-07-12 20:30:16.586644 typer-0.6.1/.github/actions/comment-docs-preview-in-pr/app/main.py
--rw-r--r--   0        0        0      106 2022-07-12 20:30:16.586644 typer-0.6.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2778 2022-07-12 20:30:16.586644 typer-0.6.1/.github/workflows/build-docs.yml
--rw-r--r--   0        0        0      576 2022-07-12 20:30:16.586644 typer-0.6.1/.github/workflows/issue-manager.yml
--rw-r--r--   0        0        0     1130 2022-07-12 20:30:16.586644 typer-0.6.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1195 2022-07-12 20:30:16.586644 typer-0.6.1/.github/workflows/preview-docs.yml
--rw-r--r--   0        0        0      567 2022-07-12 20:30:16.586644 typer-0.6.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      944 2022-07-12 20:30:16.586644 typer-0.6.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      117 2022-07-12 20:30:16.586644 typer-0.6.1/.gitignore
--rw-r--r--   0        0        0     1473 2022-07-12 20:30:16.586644 typer-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      125 2022-07-12 20:30:16.586644 typer-0.6.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1086 2022-07-12 20:30:16.586644 typer-0.6.1/LICENSE
--rw-r--r--   0        0        0    15225 2022-07-12 20:30:16.586644 typer-0.6.1/README.md
--rw-r--r--   0        0        0     1160 2022-07-12 20:30:16.586644 typer-0.6.1/SECURITY.md
--rw-r--r--   0        0        0     4870 2022-07-12 20:30:16.586644 typer-0.6.1/docs/alternatives.md
--rw-r--r--   0        0        0     5980 2022-07-12 20:30:16.586644 typer-0.6.1/docs/contributing.md
--rw-r--r--   0        0        0      451 2022-07-12 20:30:16.586644 typer-0.6.1/docs/css/custom.css
--rw-r--r--   0        0        0     2214 2022-07-12 20:30:16.586644 typer-0.6.1/docs/css/termynal.css
--rw-r--r--   0        0        0     4434 2022-07-12 20:30:16.586644 typer-0.6.1/docs/features.md
--rw-r--r--   0        0        0     4884 2022-07-12 20:30:16.586644 typer-0.6.1/docs/help-typer.md
--rwxr-xr-x   0        0        0      439 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/favicon.png
--rw-r--r--   0        0        0    48377 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/github-social-preview.png
--rw-r--r--   0        0        0     3936 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/github-social-preview.svg
--rw-r--r--   0        0        0      284 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/icon-black.svg
--rw-r--r--   0        0        0     1743 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/icon-white.svg
--rw-r--r--   0        0        0     6768 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/logo-margin/logo-margin-vector.svg
--rw-r--r--   0        0        0     3010 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/logo-margin/logo-margin.svg
--rw-r--r--   0        0        0    13924 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/pycharm-completion.png
--rw-r--r--   0        0        0    22753 2022-07-12 20:30:16.586644 typer-0.6.1/docs/img/vscode-completion.png
--rw-r--r--   0        0        0    15225 2022-07-12 20:30:16.586644 typer-0.6.1/docs/index.md
--rw-r--r--   0        0        0     3897 2022-07-12 20:30:16.586644 typer-0.6.1/docs/js/custom.js
--rw-r--r--   0        0        0     9540 2022-07-12 20:30:16.586644 typer-0.6.1/docs/js/termynal.js
--rw-r--r--   0        0        0      912 2022-07-12 20:30:16.586644 typer-0.6.1/docs/overrides/main.html
--rw-r--r--   0        0        0    23333 2022-07-12 20:30:16.586644 typer-0.6.1/docs/release-notes.md
--rw-r--r--   0        0        0     1445 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/app-dir.md
--rw-r--r--   0        0        0     2437 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/arguments/default.md
--rw-r--r--   0        0        0     3107 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/arguments/envvar.md
--rw-r--r--   0        0        0    11924 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/arguments/help.md
--rw-r--r--   0        0        0      173 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/arguments/index.md
--rw-r--r--   0        0        0     4815 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/arguments/optional.md
--rw-r--r--   0        0        0      163 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/arguments/other-uses.md
--rw-r--r--   0        0        0     1084 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/commands/arguments.md
--rw-r--r--   0        0        0     4837 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/commands/callback.md
--rw-r--r--   0        0        0     3549 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/commands/context.md
--rw-r--r--   0        0        0    33028 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/commands/help.md
--rw-r--r--   0        0        0     6462 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/commands/index.md
--rw-r--r--   0        0        0     1162 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/commands/name.md
--rw-r--r--   0        0        0     3454 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/commands/one-or-multiple.md
--rw-r--r--   0        0        0     2044 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/commands/options.md
--rw-r--r--   0        0        0    24660 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/exceptions.md
--rw-r--r--   0        0        0    25408 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/first-steps.md
--rw-r--r--   0        0        0     2367 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/index.md
--rw-r--r--   0        0        0      974 2022-07-12 20:30:16.586644 typer-0.6.1/docs/tutorial/launch.md
--rw-r--r--   0        0        0     1876 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/multiple-values/arguments-with-multiple-values.md
--rw-r--r--   0        0        0      133 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/multiple-values/index.md
--rw-r--r--   0        0        0     1231 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/multiple-values/multiple-options.md
--rw-r--r--   0        0        0     2315 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/multiple-values/options-with-multiple-values.md
--rw-r--r--   0        0        0    12673 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/autocompletion.md
--rw-r--r--   0        0        0     7112 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/callback-and-context.md
--rw-r--r--   0        0        0     7202 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/help.md
--rw-r--r--   0        0        0      202 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/index.md
--rw-r--r--   0        0        0     8907 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/name.md
--rw-r--r--   0        0        0     1294 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/password.md
--rw-r--r--   0        0        0     1892 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/prompt.md
--rw-r--r--   0        0        0     1604 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/required.md
--rw-r--r--   0        0        0     3437 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/options/version.md
--rw-r--r--   0        0        0    20773 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/package.md
--rw-r--r--   0        0        0     4048 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/parameter-types/bool.md
--rw-r--r--   0        0        0     2416 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/parameter-types/datetime.md
--rw-r--r--   0        0        0     1791 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/parameter-types/enum.md
--rw-r--r--   0        0        0     7467 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/parameter-types/file.md
--rw-r--r--   0        0        0     2191 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/parameter-types/index.md
--rw-r--r--   0        0        0     3242 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/parameter-types/number.md
--rw-r--r--   0        0        0     3396 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/parameter-types/path.md
--rw-r--r--   0        0        0     1739 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/parameter-types/uuid.md
--rw-r--r--   0        0        0    10363 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/printing.md
--rw-r--r--   0        0        0     6259 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/progressbar.md
--rw-r--r--   0        0        0     1909 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/prompt.md
--rw-r--r--   0        0        0     3795 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/subcommands/add-typer.md
--rw-r--r--   0        0        0     2984 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/subcommands/callback-override.md
--rw-r--r--   0        0        0     1201 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/subcommands/index.md
--rw-r--r--   0        0        0    12517 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/subcommands/name-and-help.md
--rw-r--r--   0        0        0     6077 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/subcommands/nested-subcommands.md
--rw-r--r--   0        0        0     2729 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/subcommands/single-file.md
--rw-r--r--   0        0        0     3013 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/terminating.md
--rw-r--r--   0        0        0     6146 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/testing.md
--rw-r--r--   0        0        0     6229 2022-07-12 20:30:16.590644 typer-0.6.1/docs/tutorial/using-click.md
--rw-r--r--   0        0        0     9703 2022-07-12 20:30:16.590644 typer-0.6.1/docs/typer-cli.md
--rw-r--r--   0        0        0      310 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/app_dir/tutorial001.py
--rw-r--r--   0        0        0      144 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/default/tutorial001.py
--rw-r--r--   0        0        0      236 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/default/tutorial002.py
--rw-r--r--   0        0        0      165 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/envvar/tutorial001.py
--rw-r--r--   0        0        0      179 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/envvar/tutorial002.py
--rw-r--r--   0        0        0      184 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/envvar/tutorial003.py
--rw-r--r--   0        0        0      172 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/help/tutorial001.py
--rw-r--r--   0        0        0      231 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/help/tutorial002.py
--rw-r--r--   0        0        0      218 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/help/tutorial003.py
--rw-r--r--   0        0        0      238 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/help/tutorial004.py
--rw-r--r--   0        0        0      231 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/help/tutorial005.py
--rw-r--r--   0        0        0      164 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/help/tutorial006.py
--rw-r--r--   0        0        0      447 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/help/tutorial007.py
--rw-r--r--   0        0        0      210 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/help/tutorial008.py
--rw-r--r--   0        0        0      134 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/optional/tutorial001.py
--rw-r--r--   0        0        0      239 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/arguments/optional/tutorial002.py
--rw-r--r--   0        0        0      241 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/arguments/tutorial001.py
--rw-r--r--   0        0        0      721 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/callback/tutorial001.py
--rw-r--r--   0        0        0      216 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/callback/tutorial002.py
--rw-r--r--   0        0        0      304 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/callback/tutorial003.py
--rw-r--r--   0        0        0      315 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/callback/tutorial004.py
--rw-r--r--   0        0        0      411 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/context/tutorial001.py
--rw-r--r--   0        0        0      390 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/context/tutorial002.py
--rw-r--r--   0        0        0      451 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/context/tutorial003.py
--rw-r--r--   0        0        0      277 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/context/tutorial004.py
--rw-r--r--   0        0        0     1196 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/help/tutorial001.py
--rw-r--r--   0        0        0      439 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/help/tutorial002.py
--rw-r--r--   0        0        0      386 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/help/tutorial003.py
--rw-r--r--   0        0        0      827 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/help/tutorial004.py
--rw-r--r--   0        0        0      787 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/help/tutorial005.py
--rw-r--r--   0        0        0     1143 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/help/tutorial006.py
--rw-r--r--   0        0        0     1044 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/help/tutorial007.py
--rw-r--r--   0        0        0      293 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/help/tutorial008.py
--rw-r--r--   0        0        0      138 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/index/tutorial001.py
--rw-r--r--   0        0        0      215 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/index/tutorial002.py
--rw-r--r--   0        0        0      275 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/name/tutorial001.py
--rw-r--r--   0        0        0      187 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/one_or_multiple/tutorial001.py
--rw-r--r--   0        0        0      287 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/one_or_multiple/tutorial002.py
--rw-r--r--   0        0        0      693 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/commands/options/tutorial001.py
--rw-r--r--   0        0        0      115 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/exceptions/tutorial001.py
--rw-r--r--   0        0        0      174 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/exceptions/tutorial002.py
--rw-r--r--   0        0        0      170 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/exceptions/tutorial003.py
--rw-r--r--   0        0        0      171 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/exceptions/tutorial004.py
--rw-r--r--   0        0        0      101 2022-07-12 20:30:16.590644 typer-0.6.1/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      112 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      138 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      239 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/first_steps/tutorial004.py
--rw-r--r--   0        0        0      244 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/first_steps/tutorial005.py
--rw-r--r--   0        0        0      358 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/first_steps/tutorial006.py
--rw-r--r--   0        0        0      157 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/launch/tutorial001.py
--rw-r--r--   0        0        0      527 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/launch/tutorial002.py
--rw-r--r--   0        0        0      294 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/multiple_values/arguments_with_multiple_values/tutorial001.py
--rw-r--r--   0        0        0      291 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/multiple_values/arguments_with_multiple_values/tutorial002.py
--rw-r--r--   0        0        0      295 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/multiple_values/multiple_options/tutorial001.py
--rw-r--r--   0        0        0      178 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/multiple_values/multiple_options/tutorial002.py
--rw-r--r--   0        0        0      403 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/multiple_values/options_with_multiple_values/tutorial001.py
--rw-r--r--   0        0        0      167 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial001.py
--rw-r--r--   0        0        0      285 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial002.py
--rw-r--r--   0        0        0      451 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial003.py
--rw-r--r--   0        0        0      637 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial004.py
--rw-r--r--   0        0        0      536 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial005.py
--rw-r--r--   0        0        0      236 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial006.py
--rw-r--r--   0        0        0      672 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial007.py
--rw-r--r--   0        0        0      708 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial008.py
--rw-r--r--   0        0        0      791 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/autocompletion/tutorial009.py
--rw-r--r--   0        0        0      291 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/callback/tutorial001.py
--rw-r--r--   0        0        0      320 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/callback/tutorial002.py
--rw-r--r--   0        0        0      385 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/callback/tutorial003.py
--rw-r--r--   0        0        0      429 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/callback/tutorial004.py
--rw-r--r--   0        0        0      464 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/help/tutorial001.py
--rw-r--r--   0        0        0      643 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/help/tutorial002.py
--rw-r--r--   0        0        0      170 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/help/tutorial003.py
--rw-r--r--   0        0        0      152 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/name/tutorial001.py
--rw-r--r--   0        0        0      158 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/name/tutorial002.py
--rw-r--r--   0        0        0      148 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/name/tutorial003.py
--rw-r--r--   0        0        0      163 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/name/tutorial004.py
--rw-r--r--   0        0        0      281 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/name/tutorial005.py
--rw-r--r--   0        0        0      212 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/password/tutorial001.py
--rw-r--r--   0        0        0      341 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/password/tutorial002.py
--rw-r--r--   0        0        0      171 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/prompt/tutorial001.py
--rw-r--r--   0        0        0      204 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/prompt/tutorial002.py
--rw-r--r--   0        0        0      198 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/prompt/tutorial003.py
--rw-r--r--   0        0        0      158 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/required/tutorial001.py
--rw-r--r--   0        0        0      430 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/version/tutorial001.py
--rw-r--r--   0        0        0      566 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/version/tutorial002.py
--rw-r--r--   0        0        0      597 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/options/version/tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/bool/__init__.py
--rw-r--r--   0        0        0      208 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/bool/tutorial001.py
--rw-r--r--   0        0        0      323 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/bool/tutorial002.py
--rw-r--r--   0        0        0      228 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/bool/tutorial003.py
--rw-r--r--   0        0        0      225 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/bool/tutorial004.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/datetime/__init__.py
--rw-r--r--   0        0        0      211 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/datetime/tutorial001.py
--rw-r--r--   0        0        0      293 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/datetime/tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/enum/__init__.py
--rw-r--r--   0        0        0      299 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/enum/tutorial001.py
--rw-r--r--   0        0        0      341 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/enum/tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/file/__init__.py
--rw-r--r--   0        0        0      180 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/file/tutorial001.py
--rw-r--r--   0        0        0      202 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/file/tutorial002.py
--rw-r--r--   0        0        0      321 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/file/tutorial003.py
--rw-r--r--   0        0        0      547 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/file/tutorial004.py
--rw-r--r--   0        0        0      205 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/file/tutorial005.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/index/__init__.py
--rw-r--r--   0        0        0      394 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/index/tutorial001.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/number/__init__.py
--rw-r--r--   0        0        0      302 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/number/tutorial001.py
--rw-r--r--   0        0        0      335 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/number/tutorial002.py
--rw-r--r--   0        0        0      178 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/number/tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/path/__init__.py
--rw-r--r--   0        0        0      530 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/path/tutorial001.py
--rw-r--r--   0        0        0      371 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/path/tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/uuid/__init__.py
--rw-r--r--   0        0        0      196 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/parameter_types/uuid/tutorial001.py
--rw-r--r--   0        0        0      296 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/printing/tutorial001.py
--rw-r--r--   0        0        0      183 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/printing/tutorial002.py
--rw-r--r--   0        0        0      296 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/printing/tutorial003.py
--rw-r--r--   0        0        0      214 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/printing/tutorial004.py
--rw-r--r--   0        0        0      365 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/printing/tutorial005.py
--rw-r--r--   0        0        0      150 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/printing/tutorial006.py
--rw-r--r--   0        0        0      315 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/progressbar/tutorial001.py
--rw-r--r--   0        0        0      476 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/progressbar/tutorial002.py
--rw-r--r--   0        0        0      313 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/progressbar/tutorial003.py
--rw-r--r--   0        0        0      455 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/progressbar/tutorial004.py
--rw-r--r--   0        0        0      333 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/progressbar/tutorial005.py
--rw-r--r--   0        0        0      336 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/progressbar/tutorial006.py
--rw-r--r--   0        0        0      162 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/prompt/tutorial001.py
--rw-r--r--   0        0        0      245 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/prompt/tutorial002.py
--rw-r--r--   0        0        0      180 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/prompt/tutorial003.py
--rw-r--r--   0        0        0      193 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/prompt/tutorial004.py
--rw-r--r--   0        0        0      304 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/callback_override/tutorial001.py
--rw-r--r--   0        0        0      306 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/callback_override/tutorial002.py
--rw-r--r--   0        0        0      409 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/callback_override/tutorial003.py
--rw-r--r--   0        0        0      533 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/callback_override/tutorial004.py
--rw-r--r--   0        0        0      254 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/name_help/tutorial001.py
--rw-r--r--   0        0        0      289 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/name_help/tutorial002.py
--rw-r--r--   0        0        0      282 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/name_help/tutorial003.py
--rw-r--r--   0        0        0      372 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/name_help/tutorial004.py
--rw-r--r--   0        0        0      473 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/name_help/tutorial005.py
--rw-r--r--   0        0        0      514 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/name_help/tutorial006.py
--rw-r--r--   0        0        0      564 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/name_help/tutorial007.py
--rw-r--r--   0        0        0      644 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/name_help/tutorial008.py
--rw-r--r--   0        0        0      298 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial001/items.py
--rw-r--r--   0        0        0      177 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial001/main.py
--rw-r--r--   0        0        0      245 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial001/users.py
--rw-r--r--   0        0        0      698 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial002/main.py
--rw-r--r--   0        0        0      298 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial003/items.py
--rw-r--r--   0        0        0      180 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial003/lands.py
--rw-r--r--   0        0        0      229 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial003/main.py
--rw-r--r--   0        0        0      233 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial003/reigns.py
--rw-r--r--   0        0        0      221 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial003/towns.py
--rw-r--r--   0        0        0      245 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/subcommands/tutorial003/users.py
--rw-r--r--   0        0        0      598 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/terminating/tutorial001.py
--rw-r--r--   0        0        0      235 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/terminating/tutorial002.py
--rw-r--r--   0        0        0      230 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/terminating/tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/testing/app01/__init__.py
--rw-r--r--   0        0        0      256 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/testing/app01/main.py
--rw-r--r--   0        0        0      299 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/testing/app01/test_main.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/testing/app02/__init__.py
--rw-r--r--   0        0        0      207 2022-07-12 20:30:16.594645 typer-0.6.1/docs_src/testing/app02/main.py
--rw-r--r--   0        0        0      284 2022-07-12 20:30:16.598645 typer-0.6.1/docs_src/testing/app02/test_main.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/docs_src/testing/app03/__init__.py
--rw-r--r--   0        0        0      122 2022-07-12 20:30:16.598645 typer-0.6.1/docs_src/testing/app03/main.py
--rw-r--r--   0        0        0      284 2022-07-12 20:30:16.598645 typer-0.6.1/docs_src/testing/app03/test_main.py
--rw-r--r--   0        0        0      371 2022-07-12 20:30:16.598645 typer-0.6.1/docs_src/using_click/tutorial001.py
--rw-r--r--   0        0        0      287 2022-07-12 20:30:16.598645 typer-0.6.1/docs_src/using_click/tutorial002.py
--rw-r--r--   0        0        0      626 2022-07-12 20:30:16.598645 typer-0.6.1/docs_src/using_click/tutorial003.py
--rw-r--r--   0        0        0      511 2022-07-12 20:30:16.598645 typer-0.6.1/docs_src/using_click/tutorial004.py
--rw-r--r--   0        0        0       51 2022-07-12 20:30:16.598645 typer-0.6.1/mkdocs.insiders.yml
--rw-r--r--   0        0        0     5363 2022-07-12 20:30:16.598645 typer-0.6.1/mkdocs.yml
--rw-r--r--   0        0        0       96 2022-07-12 20:30:16.598645 typer-0.6.1/mypy.ini
--rw-r--r--   0        0        0     2129 2022-07-12 20:30:16.598645 typer-0.6.1/pyproject.toml
--rwxr-xr-x   0        0        0       76 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       98 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/clean.sh
--rwxr-xr-x   0        0        0       68 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/docs-live.sh
--rwxr-xr-x   0        0        0      167 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/format-imports.sh
--rwxr-xr-x   0        0        0      205 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/format.sh
--rw-r--r--   0        0        0      112 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/get-pwsh-activate.sh
--rwxr-xr-x   0        0        0      122 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/lint.sh
--rwxr-xr-x   0        0        0      339 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/netlify-docs.sh
--rwxr-xr-x   0        0        0       42 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/publish.sh
--rwxr-xr-x   0        0        0       80 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      350 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/test-files.sh
--rwxr-xr-x   0        0        0      530 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/test.sh
--rw-r--r--   0        0        0      108 2022-07-12 20:30:16.598645 typer-0.6.1/scripts/zip-docs.sh
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/assets/__init__.py
--rw-r--r--   0        0        0      675 2022-07-12 20:30:16.598645 typer-0.6.1/tests/assets/compat_click7_8.py
--rw-r--r--   0        0        0      542 2022-07-12 20:30:16.598645 typer-0.6.1/tests/assets/completion_no_types.py
--rw-r--r--   0        0        0      542 2022-07-12 20:30:16.598645 typer-0.6.1/tests/assets/completion_no_types_order.py
--rw-r--r--   0        0        0      160 2022-07-12 20:30:16.598645 typer-0.6.1/tests/assets/prog_name.py
--rw-r--r--   0        0        0      157 2022-07-12 20:30:16.598645 typer-0.6.1/tests/assets/type_error_no_rich.py
--rw-r--r--   0        0        0      213 2022-07-12 20:30:16.598645 typer-0.6.1/tests/assets/type_error_no_rich_short_disable.py
--rw-r--r--   0        0        0      306 2022-07-12 20:30:16.598645 typer-0.6.1/tests/assets/type_error_normal_traceback.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_compat/__init__.py
--rw-r--r--   0        0        0     1585 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_compat/test_option_get_help.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_completion/__init__.py
--rw-r--r--   0        0        0     5149 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_completion/test_completion.py
--rw-r--r--   0        0        0     5551 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_completion/test_completion_complete.py
--rw-r--r--   0        0        0     2110 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_completion/test_completion_complete_no_help.py
--rw-r--r--   0        0        0     5556 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_completion/test_completion_install.py
--rw-r--r--   0        0        0     3270 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_completion/test_completion_show.py
--rw-r--r--   0        0        0      797 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_exit_errors.py
--rw-r--r--   0        0        0     6720 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_others.py
--rw-r--r--   0        0        0      377 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_prog_name.py
--rw-r--r--   0        0        0      849 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_rich_utils.py
--rw-r--r--   0        0        0     2479 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tracebacks.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_default/__init__.py
--rw-r--r--   0        0        0      947 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py
--rw-r--r--   0        0        0     1072 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_envvar/__init__.py
--rw-r--r--   0        0        0     1621 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py
--rw-r--r--   0        0        0     1217 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py
--rw-r--r--   0        0        0     1238 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/__init__.py
--rw-r--r--   0        0        0     1310 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py
--rw-r--r--   0        0        0      955 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py
--rw-r--r--   0        0        0      946 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py
--rw-r--r--   0        0        0      950 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py
--rw-r--r--   0        0        0      868 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py
--rw-r--r--   0        0        0      852 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py
--rw-r--r--   0        0        0      842 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py
--rw-r--r--   0        0        0     1290 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_optional/__init__.py
--rw-r--r--   0        0        0     1155 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py
--rw-r--r--   0        0        0      850 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_arguments/__init__.py
--rw-r--r--   0        0        0     1045 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_callback/__init__.py
--rw-r--r--   0        0        0     2300 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py
--rw-r--r--   0        0        0      591 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py
--rw-r--r--   0        0        0      708 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py
--rw-r--r--   0        0        0      831 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_context/__init__.py
--rw-r--r--   0        0        0      831 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_context/test_tutorial001.py
--rw-r--r--   0        0        0      949 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_context/test_tutorial002.py
--rw-r--r--   0        0        0      957 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_context/test_tutorial003.py
--rw-r--r--   0        0        0      716 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_context/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/__init__.py
--rw-r--r--   0        0        0     4190 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     1646 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial002.py
--rw-r--r--   0        0        0     1105 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial003.py
--rw-r--r--   0        0        0     1808 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial004.py
--rw-r--r--   0        0        0     1875 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial005.py
--rw-r--r--   0        0        0     1577 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial006.py
--rw-r--r--   0        0        0     1674 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial007.py
--rw-r--r--   0        0        0      710 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial008.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_index/__init__.py
--rw-r--r--   0        0        0      662 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_index/test_tutorial001.py
--rw-r--r--   0        0        0      960 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_index/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_name/__init__.py
--rw-r--r--   0        0        0      911 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_name/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.598645 typer-0.6.1/tests/test_tutorial/test_commands/test_one_or_multiple/__init__.py
--rw-r--r--   0        0        0      721 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py
--rw-r--r--   0        0        0      865 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_commands/test_options/__init__.py
--rw-r--r--   0        0        0     3019 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_commands/test_options/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_exceptions/__init__.py
--rw-r--r--   0        0        0     1886 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_exceptions/test_tutorial001.py
--rw-r--r--   0        0        0     1898 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_exceptions/test_tutorial002.py
--rw-r--r--   0        0        0     1145 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_exceptions/test_tutorial003.py
--rw-r--r--   0        0        0     1090 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_exceptions/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0      528 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0      698 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial002.py
--rw-r--r--   0        0        0      735 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial003.py
--rw-r--r--   0        0        0     1521 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial004.py
--rw-r--r--   0        0        0     1510 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial005.py
--rw-r--r--   0        0        0     1386 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial006.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/__init__.py
--rw-r--r--   0        0        0      724 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py
--rw-r--r--   0        0        0     1479 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/test_multiple_options/__init__.py
--rw-r--r--   0        0        0     1093 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py
--rw-r--r--   0        0        0      910 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/__init__.py
--rw-r--r--   0        0        0     1433 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_callback/__init__.py
--rw-r--r--   0        0        0      756 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_callback/test_tutorial001.py
--rw-r--r--   0        0        0     1280 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_callback/test_tutorial003.py
--rw-r--r--   0        0        0     1287 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_callback/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_completion/__init__.py
--rw-r--r--   0        0        0     1118 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial002.py
--rw-r--r--   0        0        0     1129 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial003.py
--rw-r--r--   0        0        0     1194 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial004.py
--rw-r--r--   0        0        0     1284 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial007.py
--rw-r--r--   0        0        0     1388 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial008.py
--rw-r--r--   0        0        0     1432 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial009.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_help/__init__.py
--rw-r--r--   0        0        0     1301 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     1070 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_help/test_tutorial002.py
--rw-r--r--   0        0        0      785 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_help/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_name/__init__.py
--rw-r--r--   0        0        0      794 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial001.py
--rw-r--r--   0        0        0      977 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial002.py
--rw-r--r--   0        0        0      827 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial003.py
--rw-r--r--   0        0        0      982 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial004.py
--rw-r--r--   0        0        0     1311 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial005.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_prompt/__init__.py
--rw-r--r--   0        0        0     1057 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py
--rw-r--r--   0        0        0     1078 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py
--rw-r--r--   0        0        0     1504 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_required/__init__.py
--rw-r--r--   0        0        0     1302 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_required/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_version/__init__.py
--rw-r--r--   0        0        0     1420 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_options/test_version/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/__init__.py
--rw-r--r--   0        0        0     1189 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py
--rw-r--r--   0        0        0     1712 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py
--rw-r--r--   0        0        0      952 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py
--rw-r--r--   0        0        0     1014 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_datetime/__init__.py
--rw-r--r--   0        0        0     1438 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py
--rw-r--r--   0        0        0      791 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_enum/__init__.py
--rw-r--r--   0        0        0     1280 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py
--rw-r--r--   0        0        0      782 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/__init__.py
--rw-r--r--   0        0        0      833 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py
--rw-r--r--   0        0        0      859 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py
--rw-r--r--   0        0        0      778 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py
--rw-r--r--   0        0        0      893 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py
--rw-r--r--   0        0        0     1047 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_index/__init__.py
--rw-r--r--   0        0        0     1501 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_number/__init__.py
--rw-r--r--   0        0        0     2783 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py
--rw-r--r--   0        0        0     1058 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py
--rw-r--r--   0        0        0     1379 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_path/__init__.py
--rw-r--r--   0        0        0     1462 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py
--rw-r--r--   0        0        0     1312 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_uuid/__init__.py
--rw-r--r--   0        0        0     1106 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_prompt/__init__.py
--rw-r--r--   0        0        0      611 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_prompt/test_tutorial001.py
--rw-r--r--   0        0        0      887 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_prompt/test_tutorial002.py
--rw-r--r--   0        0        0      844 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_prompt/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/__init__.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/__init__.py
--rw-r--r--   0        0        0      618 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py
--rw-r--r--   0        0        0      618 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py
--rw-r--r--   0        0        0      747 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py
--rw-r--r--   0        0        0      849 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/__init__.py
--rw-r--r--   0        0        0      954 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py
--rw-r--r--   0        0        0      954 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py
--rw-r--r--   0        0        0      954 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py
--rw-r--r--   0        0        0      954 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py
--rw-r--r--   0        0        0      996 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py
--rw-r--r--   0        0        0      946 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py
--rw-r--r--   0        0        0      979 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py
--rw-r--r--   0        0        0      992 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py
--rw-r--r--   0        0        0     2572 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_tutorial001.py
--rw-r--r--   0        0        0     2145 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_tutorial002.py
--rw-r--r--   0        0        0     4351 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_subcommands/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_terminating/__init__.py
--rw-r--r--   0        0        0     1135 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_terminating/test_tutorial001.py
--rw-r--r--   0        0        0      723 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_terminating/test_tutorial002.py
--rw-r--r--   0        0        0     1240 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_terminating/test_tutorial003.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      390 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_testing/test_app01.py
--rw-r--r--   0        0        0      390 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_testing/test_app02.py
--rw-r--r--   0        0        0      390 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_testing/test_app03.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_using_click/__init__.py
--rw-r--r--   0        0        0      861 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_using_click/test_tutorial003.py
--rw-r--r--   0        0        0      938 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_tutorial/test_using_click/test_tutorial004.py
--rw-r--r--   0        0        0     2433 2022-07-12 20:30:16.602645 typer-0.6.1/tests/test_type_conversion.py
--rw-r--r--   0        0        0     1602 2022-07-12 20:30:16.602645 typer-0.6.1/typer/__init__.py
--rw-r--r--   0        0        0       94 2022-07-12 20:30:16.602645 typer-0.6.1/typer/_compat_utils.py
--rw-r--r--   0        0        0     4957 2022-07-12 20:30:16.602645 typer-0.6.1/typer/_completion_click7.py
--rw-r--r--   0        0        0     6688 2022-07-12 20:30:16.602645 typer-0.6.1/typer/_completion_click8.py
--rw-r--r--   0        0        0     8541 2022-07-12 20:30:16.602645 typer-0.6.1/typer/_completion_shared.py
--rw-r--r--   0        0        0      430 2022-07-12 20:30:16.606645 typer-0.6.1/typer/colors.py
--rw-r--r--   0        0        0     4979 2022-07-12 20:30:16.606645 typer-0.6.1/typer/completion.py
--rw-r--r--   0        0        0    26545 2022-07-12 20:30:16.606645 typer-0.6.1/typer/core.py
--rw-r--r--   0        0        0    39081 2022-07-12 20:30:16.606645 typer-0.6.1/typer/main.py
--rw-r--r--   0        0        0    14736 2022-07-12 20:30:16.606645 typer-0.6.1/typer/models.py
--rw-r--r--   0        0        0     5949 2022-07-12 20:30:16.606645 typer-0.6.1/typer/params.py
--rw-r--r--   0        0        0        0 2022-07-12 20:30:16.606645 typer-0.6.1/typer/py.typed
--rw-r--r--   0        0        0    23656 2022-07-12 20:30:16.606645 typer-0.6.1/typer/rich_utils.py
--rw-r--r--   0        0        0      874 2022-07-12 20:30:16.606645 typer-0.6.1/typer/testing.py
--rw-r--r--   0        0        0      590 2022-07-12 20:30:16.606645 typer-0.6.1/typer/utils.py
--rw-r--r--   0        0        0    17648 1970-01-01 00:00:00.000000 typer-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0       89 2022-11-05 19:43:29.205783 typer-0.7.0/.coveragerc
+-rw-r--r--   0        0        0       19 2022-11-05 19:43:29.205783 typer-0.7.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      145 2022-11-05 19:43:29.205783 typer-0.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     6218 2022-11-05 19:43:29.205783 typer-0.7.0/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     5288 2022-11-05 19:43:29.205783 typer-0.7.0/.github/ISSUE_TEMPLATE/question.yml
+-rw-r--r--   0        0        0      115 2022-11-05 19:43:29.205783 typer-0.7.0/.github/actions/comment-docs-preview-in-pr/Dockerfile
+-rw-r--r--   0        0        0      394 2022-11-05 19:43:29.205783 typer-0.7.0/.github/actions/comment-docs-preview-in-pr/action.yml
+-rw-r--r--   0        0        0     2074 2022-11-05 19:43:29.205783 typer-0.7.0/.github/actions/comment-docs-preview-in-pr/app/main.py
+-rw-r--r--   0        0        0      309 2022-11-05 19:43:29.205783 typer-0.7.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2778 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/build-docs.yml
+-rw-r--r--   0        0        0      576 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/issue-manager.yml
+-rw-r--r--   0        0        0     1130 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1195 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/preview-docs.yml
+-rw-r--r--   0        0        0      567 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      952 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/smokeshow.yml
+-rw-r--r--   0        0        0     2267 2022-11-05 19:43:29.205783 typer-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      117 2022-11-05 19:43:29.205783 typer-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1475 2022-11-05 19:43:29.205783 typer-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      125 2022-11-05 19:43:29.205783 typer-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1086 2022-11-05 19:43:29.205783 typer-0.7.0/LICENSE
+-rw-r--r--   0        0        0    15251 2022-11-05 19:43:29.205783 typer-0.7.0/README.md
+-rw-r--r--   0        0        0     1160 2022-11-05 19:43:29.205783 typer-0.7.0/SECURITY.md
+-rw-r--r--   0        0        0     4876 2022-11-05 19:43:29.205783 typer-0.7.0/docs/alternatives.md
+-rw-r--r--   0        0        0     5980 2022-11-05 19:43:29.205783 typer-0.7.0/docs/contributing.md
+-rw-r--r--   0        0        0      451 2022-11-05 19:43:29.205783 typer-0.7.0/docs/css/custom.css
+-rw-r--r--   0        0        0     2214 2022-11-05 19:43:29.205783 typer-0.7.0/docs/css/termynal.css
+-rw-r--r--   0        0        0     4434 2022-11-05 19:43:29.205783 typer-0.7.0/docs/features.md
+-rw-r--r--   0        0        0     4884 2022-11-05 19:43:29.205783 typer-0.7.0/docs/help-typer.md
+-rwxr-xr-x   0        0        0      439 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/favicon.png
+-rw-r--r--   0        0        0    48377 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/github-social-preview.png
+-rw-r--r--   0        0        0     3936 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/github-social-preview.svg
+-rw-r--r--   0        0        0      284 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/icon-black.svg
+-rw-r--r--   0        0        0     1743 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/icon-white.svg
+-rw-r--r--   0        0        0     6768 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/logo-margin/logo-margin-vector.svg
+-rw-r--r--   0        0        0     3010 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/logo-margin/logo-margin.svg
+-rw-r--r--   0        0        0    13924 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/pycharm-completion.png
+-rw-r--r--   0        0        0    22753 2022-11-05 19:43:29.205783 typer-0.7.0/docs/img/vscode-completion.png
+-rw-r--r--   0        0        0    15251 2022-11-05 19:43:29.205783 typer-0.7.0/docs/index.md
+-rw-r--r--   0        0        0     3897 2022-11-05 19:43:29.205783 typer-0.7.0/docs/js/custom.js
+-rw-r--r--   0        0        0     9540 2022-11-05 19:43:29.205783 typer-0.7.0/docs/js/termynal.js
+-rw-r--r--   0        0        0      912 2022-11-05 19:43:29.205783 typer-0.7.0/docs/overrides/main.html
+-rw-r--r--   0        0        0    26874 2022-11-05 19:43:29.205783 typer-0.7.0/docs/release-notes.md
+-rw-r--r--   0        0        0     1445 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/app-dir.md
+-rw-r--r--   0        0        0     2437 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/default.md
+-rw-r--r--   0        0        0     3107 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/envvar.md
+-rw-r--r--   0        0        0    11924 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/help.md
+-rw-r--r--   0        0        0      173 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/index.md
+-rw-r--r--   0        0        0     4815 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/optional.md
+-rw-r--r--   0        0        0      163 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/arguments/other-uses.md
+-rw-r--r--   0        0        0     1084 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/arguments.md
+-rw-r--r--   0        0        0     4837 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/callback.md
+-rw-r--r--   0        0        0     3549 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/context.md
+-rw-r--r--   0        0        0    33029 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/help.md
+-rw-r--r--   0        0        0     7323 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/index.md
+-rw-r--r--   0        0        0     1380 2022-11-05 19:43:29.205783 typer-0.7.0/docs/tutorial/commands/name.md
+-rw-r--r--   0        0        0     3454 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/commands/one-or-multiple.md
+-rw-r--r--   0        0        0     2044 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/commands/options.md
+-rw-r--r--   0        0        0    24660 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/exceptions.md
+-rw-r--r--   0        0        0    25417 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/first-steps.md
+-rw-r--r--   0        0        0     2367 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/index.md
+-rw-r--r--   0        0        0      974 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/launch.md
+-rw-r--r--   0        0        0     1876 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/multiple-values/arguments-with-multiple-values.md
+-rw-r--r--   0        0        0      133 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/multiple-values/index.md
+-rw-r--r--   0        0        0     1231 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/multiple-values/multiple-options.md
+-rw-r--r--   0        0        0     2315 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/multiple-values/options-with-multiple-values.md
+-rw-r--r--   0        0        0    12664 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options-autocompletion.md
+-rw-r--r--   0        0        0     7112 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/callback-and-context.md
+-rw-r--r--   0        0        0     7202 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/help.md
+-rw-r--r--   0        0        0      202 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/index.md
+-rw-r--r--   0        0        0     8907 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/name.md
+-rw-r--r--   0        0        0     1294 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/password.md
+-rw-r--r--   0        0        0     1892 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/prompt.md
+-rw-r--r--   0        0        0     1604 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/required.md
+-rw-r--r--   0        0        0     3437 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/options/version.md
+-rw-r--r--   0        0        0    20773 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/package.md
+-rw-r--r--   0        0        0     4048 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/bool.md
+-rw-r--r--   0        0        0     2420 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/datetime.md
+-rw-r--r--   0        0        0     1791 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/enum.md
+-rw-r--r--   0        0        0     7467 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/file.md
+-rw-r--r--   0        0        0     2191 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/index.md
+-rw-r--r--   0        0        0     3242 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/number.md
+-rw-r--r--   0        0        0     3396 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/path.md
+-rw-r--r--   0        0        0     1739 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/parameter-types/uuid.md
+-rw-r--r--   0        0        0    10363 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/printing.md
+-rw-r--r--   0        0        0     6259 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/progressbar.md
+-rw-r--r--   0        0        0     1909 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/prompt.md
+-rw-r--r--   0        0        0     3795 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/add-typer.md
+-rw-r--r--   0        0        0     2984 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/callback-override.md
+-rw-r--r--   0        0        0     1201 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/index.md
+-rw-r--r--   0        0        0    12517 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/name-and-help.md
+-rw-r--r--   0        0        0     6077 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/nested-subcommands.md
+-rw-r--r--   0        0        0     2729 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/subcommands/single-file.md
+-rw-r--r--   0        0        0     3013 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/terminating.md
+-rw-r--r--   0        0        0     6146 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     6229 2022-11-05 19:43:29.209783 typer-0.7.0/docs/tutorial/using-click.md
+-rw-r--r--   0        0        0     9703 2022-11-05 19:43:29.209783 typer-0.7.0/docs/typer-cli.md
+-rw-r--r--   0        0        0      310 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/app_dir/tutorial001.py
+-rw-r--r--   0        0        0      144 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/default/tutorial001.py
+-rw-r--r--   0        0        0      236 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/default/tutorial002.py
+-rw-r--r--   0        0        0      165 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/envvar/tutorial001.py
+-rw-r--r--   0        0        0      179 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/envvar/tutorial002.py
+-rw-r--r--   0        0        0      184 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/envvar/tutorial003.py
+-rw-r--r--   0        0        0      172 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial001.py
+-rw-r--r--   0        0        0      231 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial002.py
+-rw-r--r--   0        0        0      218 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial003.py
+-rw-r--r--   0        0        0      238 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial004.py
+-rw-r--r--   0        0        0      231 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial005.py
+-rw-r--r--   0        0        0      164 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial006.py
+-rw-r--r--   0        0        0      447 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial007.py
+-rw-r--r--   0        0        0      210 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/help/tutorial008.py
+-rw-r--r--   0        0        0      134 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/optional/tutorial001.py
+-rw-r--r--   0        0        0      239 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/arguments/optional/tutorial002.py
+-rw-r--r--   0        0        0      241 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/arguments/tutorial001.py
+-rw-r--r--   0        0        0      721 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/callback/tutorial001.py
+-rw-r--r--   0        0        0      216 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/callback/tutorial002.py
+-rw-r--r--   0        0        0      304 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/callback/tutorial003.py
+-rw-r--r--   0        0        0      315 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/callback/tutorial004.py
+-rw-r--r--   0        0        0      411 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/context/tutorial001.py
+-rw-r--r--   0        0        0      390 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/context/tutorial002.py
+-rw-r--r--   0        0        0      451 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/context/tutorial003.py
+-rw-r--r--   0        0        0      277 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/context/tutorial004.py
+-rw-r--r--   0        0        0     1196 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial001.py
+-rw-r--r--   0        0        0      439 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial002.py
+-rw-r--r--   0        0        0      386 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial003.py
+-rw-r--r--   0        0        0      827 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial004.py
+-rw-r--r--   0        0        0      787 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial005.py
+-rw-r--r--   0        0        0     1143 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial006.py
+-rw-r--r--   0        0        0     1044 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial007.py
+-rw-r--r--   0        0        0      293 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/help/tutorial008.py
+-rw-r--r--   0        0        0      138 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/index/tutorial001.py
+-rw-r--r--   0        0        0      215 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/index/tutorial002.py
+-rw-r--r--   0        0        0      275 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/name/tutorial001.py
+-rw-r--r--   0        0        0      187 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/one_or_multiple/tutorial001.py
+-rw-r--r--   0        0        0      287 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/one_or_multiple/tutorial002.py
+-rw-r--r--   0        0        0      693 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/commands/options/tutorial001.py
+-rw-r--r--   0        0        0      115 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/exceptions/tutorial001.py
+-rw-r--r--   0        0        0      174 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/exceptions/tutorial002.py
+-rw-r--r--   0        0        0      170 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/exceptions/tutorial003.py
+-rw-r--r--   0        0        0      171 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/exceptions/tutorial004.py
+-rw-r--r--   0        0        0      101 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      112 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      138 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      239 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial004.py
+-rw-r--r--   0        0        0      244 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial005.py
+-rw-r--r--   0        0        0      358 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/first_steps/tutorial006.py
+-rw-r--r--   0        0        0      157 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/launch/tutorial001.py
+-rw-r--r--   0        0        0      527 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/launch/tutorial002.py
+-rw-r--r--   0        0        0      294 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/arguments_with_multiple_values/tutorial001.py
+-rw-r--r--   0        0        0      291 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/arguments_with_multiple_values/tutorial002.py
+-rw-r--r--   0        0        0      295 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/multiple_options/tutorial001.py
+-rw-r--r--   0        0        0      178 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/multiple_options/tutorial002.py
+-rw-r--r--   0        0        0      403 2022-11-05 19:43:29.209783 typer-0.7.0/docs_src/multiple_values/options_with_multiple_values/tutorial001.py
+-rw-r--r--   0        0        0      291 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/callback/tutorial001.py
+-rw-r--r--   0        0        0      320 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/callback/tutorial002.py
+-rw-r--r--   0        0        0      385 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/callback/tutorial003.py
+-rw-r--r--   0        0        0      429 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/callback/tutorial004.py
+-rw-r--r--   0        0        0      464 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/help/tutorial001.py
+-rw-r--r--   0        0        0      643 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/help/tutorial002.py
+-rw-r--r--   0        0        0      170 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/help/tutorial003.py
+-rw-r--r--   0        0        0      152 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial001.py
+-rw-r--r--   0        0        0      158 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial002.py
+-rw-r--r--   0        0        0      148 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial003.py
+-rw-r--r--   0        0        0      163 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial004.py
+-rw-r--r--   0        0        0      281 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/name/tutorial005.py
+-rw-r--r--   0        0        0      212 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/password/tutorial001.py
+-rw-r--r--   0        0        0      341 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/password/tutorial002.py
+-rw-r--r--   0        0        0      171 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/prompt/tutorial001.py
+-rw-r--r--   0        0        0      204 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/prompt/tutorial002.py
+-rw-r--r--   0        0        0      198 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/prompt/tutorial003.py
+-rw-r--r--   0        0        0      158 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/required/tutorial001.py
+-rw-r--r--   0        0        0      430 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/version/tutorial001.py
+-rw-r--r--   0        0        0      566 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/version/tutorial002.py
+-rw-r--r--   0        0        0      597 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options/version/tutorial003.py
+-rw-r--r--   0        0        0      193 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial001.py
+-rw-r--r--   0        0        0      312 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial002.py
+-rw-r--r--   0        0        0      478 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial003.py
+-rw-r--r--   0        0        0      664 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial004.py
+-rw-r--r--   0        0        0      563 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial005.py
+-rw-r--r--   0        0        0      262 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial006.py
+-rw-r--r--   0        0        0      699 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial007.py
+-rw-r--r--   0        0        0      735 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial008.py
+-rw-r--r--   0        0        0      818 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/options_autocompletion/tutorial009.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/__init__.py
+-rw-r--r--   0        0        0      208 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/tutorial001.py
+-rw-r--r--   0        0        0      323 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/tutorial002.py
+-rw-r--r--   0        0        0      228 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/tutorial003.py
+-rw-r--r--   0        0        0      225 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/bool/tutorial004.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/datetime/__init__.py
+-rw-r--r--   0        0        0      211 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/datetime/tutorial001.py
+-rw-r--r--   0        0        0      293 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/datetime/tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/enum/__init__.py
+-rw-r--r--   0        0        0      299 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/enum/tutorial001.py
+-rw-r--r--   0        0        0      341 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/enum/tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/__init__.py
+-rw-r--r--   0        0        0      180 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial001.py
+-rw-r--r--   0        0        0      202 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial002.py
+-rw-r--r--   0        0        0      321 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial003.py
+-rw-r--r--   0        0        0      547 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial004.py
+-rw-r--r--   0        0        0      205 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/file/tutorial005.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/index/__init__.py
+-rw-r--r--   0        0        0      394 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/index/tutorial001.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/number/__init__.py
+-rw-r--r--   0        0        0      302 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/number/tutorial001.py
+-rw-r--r--   0        0        0      335 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/number/tutorial002.py
+-rw-r--r--   0        0        0      178 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/number/tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/path/__init__.py
+-rw-r--r--   0        0        0      530 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/path/tutorial001.py
+-rw-r--r--   0        0        0      371 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/path/tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/uuid/__init__.py
+-rw-r--r--   0        0        0      196 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/parameter_types/uuid/tutorial001.py
+-rw-r--r--   0        0        0      296 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial001.py
+-rw-r--r--   0        0        0      183 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial002.py
+-rw-r--r--   0        0        0      296 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial003.py
+-rw-r--r--   0        0        0      214 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial004.py
+-rw-r--r--   0        0        0      365 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial005.py
+-rw-r--r--   0        0        0      150 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/printing/tutorial006.py
+-rw-r--r--   0        0        0      315 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial001.py
+-rw-r--r--   0        0        0      476 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial002.py
+-rw-r--r--   0        0        0      313 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial003.py
+-rw-r--r--   0        0        0      455 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial004.py
+-rw-r--r--   0        0        0      333 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial005.py
+-rw-r--r--   0        0        0      336 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/progressbar/tutorial006.py
+-rw-r--r--   0        0        0      162 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/prompt/tutorial001.py
+-rw-r--r--   0        0        0      245 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/prompt/tutorial002.py
+-rw-r--r--   0        0        0      180 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/prompt/tutorial003.py
+-rw-r--r--   0        0        0      193 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/prompt/tutorial004.py
+-rw-r--r--   0        0        0      304 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/callback_override/tutorial001.py
+-rw-r--r--   0        0        0      306 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/callback_override/tutorial002.py
+-rw-r--r--   0        0        0      409 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/callback_override/tutorial003.py
+-rw-r--r--   0        0        0      533 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/callback_override/tutorial004.py
+-rw-r--r--   0        0        0      254 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial001.py
+-rw-r--r--   0        0        0      289 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial002.py
+-rw-r--r--   0        0        0      282 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial003.py
+-rw-r--r--   0        0        0      372 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial004.py
+-rw-r--r--   0        0        0      473 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial005.py
+-rw-r--r--   0        0        0      514 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial006.py
+-rw-r--r--   0        0        0      564 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial007.py
+-rw-r--r--   0        0        0      644 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/name_help/tutorial008.py
+-rw-r--r--   0        0        0      298 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial001/items.py
+-rw-r--r--   0        0        0      177 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial001/main.py
+-rw-r--r--   0        0        0      245 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial001/users.py
+-rw-r--r--   0        0        0      698 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial002/main.py
+-rw-r--r--   0        0        0      298 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/items.py
+-rw-r--r--   0        0        0      180 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/lands.py
+-rw-r--r--   0        0        0      229 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/main.py
+-rw-r--r--   0        0        0      233 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/reigns.py
+-rw-r--r--   0        0        0      221 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/towns.py
+-rw-r--r--   0        0        0      245 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/subcommands/tutorial003/users.py
+-rw-r--r--   0        0        0      598 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/terminating/tutorial001.py
+-rw-r--r--   0        0        0      235 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/terminating/tutorial002.py
+-rw-r--r--   0        0        0      230 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/terminating/tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app01/__init__.py
+-rw-r--r--   0        0        0      256 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app01/main.py
+-rw-r--r--   0        0        0      299 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app01/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app02/__init__.py
+-rw-r--r--   0        0        0      207 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app02/main.py
+-rw-r--r--   0        0        0      284 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app02/test_main.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app03/__init__.py
+-rw-r--r--   0        0        0      122 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app03/main.py
+-rw-r--r--   0        0        0      284 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/testing/app03/test_main.py
+-rw-r--r--   0        0        0      371 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/using_click/tutorial001.py
+-rw-r--r--   0        0        0      287 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/using_click/tutorial002.py
+-rw-r--r--   0        0        0      626 2022-11-05 19:43:29.213783 typer-0.7.0/docs_src/using_click/tutorial003.py
+-rw-r--r--   0        0        0      511 2022-11-05 19:43:29.217783 typer-0.7.0/docs_src/using_click/tutorial004.py
+-rw-r--r--   0        0        0       51 2022-11-05 19:43:29.217783 typer-0.7.0/mkdocs.insiders.yml
+-rw-r--r--   0        0        0     5359 2022-11-05 19:43:29.217783 typer-0.7.0/mkdocs.yml
+-rw-r--r--   0        0        0       96 2022-11-05 19:43:29.217783 typer-0.7.0/mypy.ini
+-rw-r--r--   0        0        0     2965 2022-11-05 19:43:29.217783 typer-0.7.0/pyproject.toml
+-rwxr-xr-x   0        0        0       76 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       98 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/clean.sh
+-rwxr-xr-x   0        0        0       68 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/docs-live.sh
+-rwxr-xr-x   0        0        0      167 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/format-imports.sh
+-rwxr-xr-x   0        0        0      205 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/format.sh
+-rw-r--r--   0        0        0      112 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/get-pwsh-activate.sh
+-rwxr-xr-x   0        0        0      122 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/lint.sh
+-rwxr-xr-x   0        0        0      339 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/netlify-docs.sh
+-rwxr-xr-x   0        0        0       42 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/publish.sh
+-rwxr-xr-x   0        0        0       80 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      350 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/test-files.sh
+-rwxr-xr-x   0        0        0      490 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/test.sh
+-rw-r--r--   0        0        0      108 2022-11-05 19:43:29.217783 typer-0.7.0/scripts/zip-docs.sh
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/__init__.py
+-rw-r--r--   0        0        0      675 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/compat_click7_8.py
+-rw-r--r--   0        0        0      542 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/completion_no_types.py
+-rw-r--r--   0        0        0      542 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/completion_no_types_order.py
+-rw-r--r--   0        0        0      160 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/prog_name.py
+-rw-r--r--   0        0        0      157 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/type_error_no_rich.py
+-rw-r--r--   0        0        0      213 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/type_error_no_rich_short_disable.py
+-rw-r--r--   0        0        0      306 2022-11-05 19:43:29.217783 typer-0.7.0/tests/assets/type_error_normal_traceback.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_compat/__init__.py
+-rw-r--r--   0        0        0     1585 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_compat/test_option_get_help.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/__init__.py
+-rw-r--r--   0        0        0     5152 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion.py
+-rw-r--r--   0        0        0     5551 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion_complete.py
+-rw-r--r--   0        0        0     2110 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion_complete_no_help.py
+-rw-r--r--   0        0        0     5559 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion_install.py
+-rw-r--r--   0        0        0     3273 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_completion/test_completion_show.py
+-rw-r--r--   0        0        0      797 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_exit_errors.py
+-rw-r--r--   0        0        0     6720 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_others.py
+-rw-r--r--   0        0        0      377 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_prog_name.py
+-rw-r--r--   0        0        0      849 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_rich_utils.py
+-rw-r--r--   0        0        0     2479 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tracebacks.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_default/__init__.py
+-rw-r--r--   0        0        0      947 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py
+-rw-r--r--   0        0        0     1072 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/__init__.py
+-rw-r--r--   0        0        0     1621 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py
+-rw-r--r--   0        0        0     1217 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py
+-rw-r--r--   0        0        0     1238 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/__init__.py
+-rw-r--r--   0        0        0     1310 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0      955 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0      946 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0      950 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py
+-rw-r--r--   0        0        0      868 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py
+-rw-r--r--   0        0        0      852 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py
+-rw-r--r--   0        0        0      842 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py
+-rw-r--r--   0        0        0     1290 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/__init__.py
+-rw-r--r--   0        0        0     1155 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py
+-rw-r--r--   0        0        0      850 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_arguments/__init__.py
+-rw-r--r--   0        0        0     1045 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/__init__.py
+-rw-r--r--   0        0        0     2300 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py
+-rw-r--r--   0        0        0      591 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py
+-rw-r--r--   0        0        0      708 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py
+-rw-r--r--   0        0        0      831 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/__init__.py
+-rw-r--r--   0        0        0      831 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial001.py
+-rw-r--r--   0        0        0      949 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial002.py
+-rw-r--r--   0        0        0      957 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial003.py
+-rw-r--r--   0        0        0      716 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/__init__.py
+-rw-r--r--   0        0        0     4190 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     1646 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0     1105 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0     1808 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial004.py
+-rw-r--r--   0        0        0     1875 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial005.py
+-rw-r--r--   0        0        0     1577 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial006.py
+-rw-r--r--   0        0        0     1674 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial007.py
+-rw-r--r--   0        0        0      710 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial008.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_index/__init__.py
+-rw-r--r--   0        0        0      662 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_index/test_tutorial001.py
+-rw-r--r--   0        0        0      960 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_index/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_name/__init__.py
+-rw-r--r--   0        0        0      911 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_name/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/__init__.py
+-rw-r--r--   0        0        0      721 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py
+-rw-r--r--   0        0        0      865 2022-11-05 19:43:29.217783 typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_commands/test_options/__init__.py
+-rw-r--r--   0        0        0     3019 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_commands/test_options/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/__init__.py
+-rw-r--r--   0        0        0     1886 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial001.py
+-rw-r--r--   0        0        0     1898 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial002.py
+-rw-r--r--   0        0        0     1145 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial003.py
+-rw-r--r--   0        0        0     1090 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0      528 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0      698 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial002.py
+-rw-r--r--   0        0        0      735 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial003.py
+-rw-r--r--   0        0        0     1521 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial004.py
+-rw-r--r--   0        0        0     1510 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial005.py
+-rw-r--r--   0        0        0     1386 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/__init__.py
+-rw-r--r--   0        0        0      724 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py
+-rw-r--r--   0        0        0     1479 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/__init__.py
+-rw-r--r--   0        0        0     1093 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py
+-rw-r--r--   0        0        0      910 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/__init__.py
+-rw-r--r--   0        0        0     1433 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_callback/__init__.py
+-rw-r--r--   0        0        0      756 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial001.py
+-rw-r--r--   0        0        0     1280 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial003.py
+-rw-r--r--   0        0        0     1287 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_help/__init__.py
+-rw-r--r--   0        0        0     1301 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     1070 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0      785 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/__init__.py
+-rw-r--r--   0        0        0      794 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial001.py
+-rw-r--r--   0        0        0      977 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial002.py
+-rw-r--r--   0        0        0      827 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial003.py
+-rw-r--r--   0        0        0      982 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial004.py
+-rw-r--r--   0        0        0     1311 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_prompt/__init__.py
+-rw-r--r--   0        0        0     1057 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py
+-rw-r--r--   0        0        0     1078 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py
+-rw-r--r--   0        0        0     1504 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_required/__init__.py
+-rw-r--r--   0        0        0     1302 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_required/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_version/__init__.py
+-rw-r--r--   0        0        0     1420 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options/test_version/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/__init__.py
+-rw-r--r--   0        0        0     1064 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py
+-rw-r--r--   0        0        0     1075 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py
+-rw-r--r--   0        0        0     1144 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py
+-rw-r--r--   0        0        0     1230 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py
+-rw-r--r--   0        0        0     1334 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py
+-rw-r--r--   0        0        0     1378 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/__init__.py
+-rw-r--r--   0        0        0     1189 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py
+-rw-r--r--   0        0        0     1712 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py
+-rw-r--r--   0        0        0      952 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py
+-rw-r--r--   0        0        0     1014 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/__init__.py
+-rw-r--r--   0        0        0     1438 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py
+-rw-r--r--   0        0        0      791 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/__init__.py
+-rw-r--r--   0        0        0     1280 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py
+-rw-r--r--   0        0        0      782 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/__init__.py
+-rw-r--r--   0        0        0      833 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py
+-rw-r--r--   0        0        0      859 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py
+-rw-r--r--   0        0        0      778 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py
+-rw-r--r--   0        0        0      893 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py
+-rw-r--r--   0        0        0     1047 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_index/__init__.py
+-rw-r--r--   0        0        0     1501 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/__init__.py
+-rw-r--r--   0        0        0     2783 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py
+-rw-r--r--   0        0        0     1058 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py
+-rw-r--r--   0        0        0     1379 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/__init__.py
+-rw-r--r--   0        0        0     1462 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py
+-rw-r--r--   0        0        0     1312 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_uuid/__init__.py
+-rw-r--r--   0        0        0     1106 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_prompt/__init__.py
+-rw-r--r--   0        0        0      611 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial001.py
+-rw-r--r--   0        0        0      887 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial002.py
+-rw-r--r--   0        0        0      844 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/__init__.py
+-rw-r--r--   0        0        0      618 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py
+-rw-r--r--   0        0        0      618 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py
+-rw-r--r--   0        0        0      747 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py
+-rw-r--r--   0        0        0      849 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/__init__.py
+-rw-r--r--   0        0        0      954 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py
+-rw-r--r--   0        0        0      954 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py
+-rw-r--r--   0        0        0      954 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py
+-rw-r--r--   0        0        0      954 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py
+-rw-r--r--   0        0        0      996 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py
+-rw-r--r--   0        0        0      946 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py
+-rw-r--r--   0        0        0      979 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py
+-rw-r--r--   0        0        0      992 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py
+-rw-r--r--   0        0        0     2572 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial001.py
+-rw-r--r--   0        0        0     2145 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial002.py
+-rw-r--r--   0        0        0     5514 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_terminating/__init__.py
+-rw-r--r--   0        0        0     1135 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial001.py
+-rw-r--r--   0        0        0      723 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial002.py
+-rw-r--r--   0        0        0     1240 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      390 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_testing/test_app01.py
+-rw-r--r--   0        0        0      390 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_testing/test_app02.py
+-rw-r--r--   0        0        0      390 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_testing/test_app03.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_using_click/__init__.py
+-rw-r--r--   0        0        0      861 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_using_click/test_tutorial003.py
+-rw-r--r--   0        0        0      938 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_tutorial/test_using_click/test_tutorial004.py
+-rw-r--r--   0        0        0     2433 2022-11-05 19:43:29.221783 typer-0.7.0/tests/test_type_conversion.py
+-rw-r--r--   0        0        0     1602 2022-11-05 19:43:29.221783 typer-0.7.0/typer/__init__.py
+-rw-r--r--   0        0        0       94 2022-11-05 19:43:29.221783 typer-0.7.0/typer/_compat_utils.py
+-rw-r--r--   0        0        0     4957 2022-11-05 19:43:29.221783 typer-0.7.0/typer/_completion_click7.py
+-rw-r--r--   0        0        0     6688 2022-11-05 19:43:29.221783 typer-0.7.0/typer/_completion_click8.py
+-rw-r--r--   0        0        0     8541 2022-11-05 19:43:29.221783 typer-0.7.0/typer/_completion_shared.py
+-rw-r--r--   0        0        0      430 2022-11-05 19:43:29.221783 typer-0.7.0/typer/colors.py
+-rw-r--r--   0        0        0     4979 2022-11-05 19:43:29.221783 typer-0.7.0/typer/completion.py
+-rw-r--r--   0        0        0    26545 2022-11-05 19:43:29.221783 typer-0.7.0/typer/core.py
+-rw-r--r--   0        0        0    39111 2022-11-05 19:43:29.221783 typer-0.7.0/typer/main.py
+-rw-r--r--   0        0        0    14736 2022-11-05 19:43:29.221783 typer-0.7.0/typer/models.py
+-rw-r--r--   0        0        0     5949 2022-11-05 19:43:29.221783 typer-0.7.0/typer/params.py
+-rw-r--r--   0        0        0        0 2022-11-05 19:43:29.221783 typer-0.7.0/typer/py.typed
+-rw-r--r--   0        0        0    23656 2022-11-05 19:43:29.225783 typer-0.7.0/typer/rich_utils.py
+-rw-r--r--   0        0        0      874 2022-11-05 19:43:29.225783 typer-0.7.0/typer/testing.py
+-rw-r--r--   0        0        0      590 2022-11-05 19:43:29.225783 typer-0.7.0/typer/utils.py
+-rw-r--r--   0        0        0    17937 1970-01-01 00:00:00.000000 typer-0.7.0/PKG-INFO
```

### Comparing `typer-0.6.1/.github/ISSUE_TEMPLATE/feature-request.yml` & `typer-0.7.0/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/.github/ISSUE_TEMPLATE/question.yml` & `typer-0.7.0/.github/ISSUE_TEMPLATE/question.yml`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/.github/actions/comment-docs-preview-in-pr/app/main.py` & `typer-0.7.0/.github/actions/comment-docs-preview-in-pr/app/main.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/.github/workflows/build-docs.yml` & `typer-0.7.0/.github/workflows/build-docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   build-docs:
     runs-on: ubuntu-20.04
     steps:
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.7"
       # Allow debugging with tmate
       - name: Setup tmate session
         uses: mxschmitt/action-tmate@v3
@@ -52,20 +52,20 @@
         if: github.event_name == 'pull_request' && github.event.pull_request.head.repo.fork == true
         run: python3.7 -m mkdocs build
       - name: Build Docs with Insiders
         if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.fork == false
         run: python3.7 -m mkdocs build --config-file mkdocs.insiders.yml
       - name: Zip docs
         run: bash ./scripts/zip-docs.sh
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           name: docs-zip
           path: ./docs.zip
       - name: Deploy to Netlify
-        uses: nwtgck/actions-netlify@v1.1.5
+        uses: nwtgck/actions-netlify@v1.2.4
         with:
           publish-dir: './site'
           production-branch: master
           github-token: ${{ secrets.GITHUB_TOKEN }}
           enable-commit-comment: false
         env:
           NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
```

### Comparing `typer-0.6.1/.github/workflows/issue-manager.yml` & `typer-0.7.0/.github/workflows/issue-manager.yml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     types:
       - labeled
 
 jobs:
   issue-manager:
     runs-on: ubuntu-latest
     steps:
-      - uses: tiangolo/issue-manager@0.2.0
+      - uses: tiangolo/issue-manager@0.4.0
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           config: >
             {
               "answered": {
                 "message": "Assuming the original issue was solved, it will be automatically closed now. But feel free to add more comments or create new issues."
               }
```

### Comparing `typer-0.6.1/.github/workflows/latest-changes.yml` & `typer-0.7.0/.github/workflows/latest-changes.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         required: false
         default: false
 
 jobs:
   latest-changes:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           # To allow latest-changes to commit to the main branch
           token: ${{ secrets.ACTIONS_TOKEN }}
       # Allow debugging with tmate
       - name: Setup tmate session
         uses: mxschmitt/action-tmate@v3
         if: ${{ github.event_name == 'workflow_dispatch' && github.event.inputs.debug_enabled }}
```

### Comparing `typer-0.6.1/.github/workflows/preview-docs.yml` & `typer-0.7.0/.github/workflows/preview-docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,30 @@
     types:
       - completed
 
 jobs:
   preview-docs:
     runs-on: ubuntu-20.04
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Download Artifact Docs
         uses: dawidd6/action-download-artifact@v2.9.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           workflow: build-docs.yml
           run_id: ${{ github.event.workflow_run.id }}
           name: docs-zip
       - name: Unzip docs
         run: |
           rm -rf ./site
           unzip docs.zip
           rm -f docs.zip
       - name: Deploy to Netlify
         id: netlify
-        uses: nwtgck/actions-netlify@v1.1.5
+        uses: nwtgck/actions-netlify@v1.2.4
         with:
           publish-dir: './site'
           production-deploy: false
           github-token: ${{ secrets.GITHUB_TOKEN }}
           enable-commit-comment: false
         env:
           NETLIFY_AUTH_TOKEN: ${{ secrets.NETLIFY_AUTH_TOKEN }}
```

### Comparing `typer-0.6.1/.github/workflows/publish.yml` & `typer-0.7.0/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     types:
       - created
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: "3.7"
       - name: Install Flit
         run: pip install flit
       - name: Install Dependencies
```

### Comparing `typer-0.6.1/.pre-commit-config.yaml` & `typer-0.7.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,24 @@
     -   id: check-toml
     -   id: check-yaml
         args:
         -   --unsafe
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v2.34.0
+    rev: v3.2.0
     hooks:
     -   id: pyupgrade
         args:
         - --py3-plus
         - --keep-runtime-typing
         # This file is more readable without yield from
         exclude: ^docs_src/progressbar/tutorial004\.py
--   repo: https://github.com/myint/autoflake
-    rev: v1.4
+-   repo: https://github.com/PyCQA/autoflake
+    rev: v1.7.7
     hooks:
     -   id: autoflake
         args:
         - --recursive
         - --in-place
         - --remove-all-unused-imports
         - --remove-unused-variables
@@ -41,13 +41,13 @@
     -   id: isort
         name: isort (cython)
         types: [cython]
     -   id: isort
         name: isort (pyi)
         types: [pyi]
 -   repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 22.10.0
     hooks:
     -   id: black
 ci:
     autofix_commit_msg: 🎨 [pre-commit.ci] Auto format from pre-commit.com hooks
     autoupdate_commit_msg: ⬆ [pre-commit.ci] pre-commit autoupdate
```

### Comparing `typer-0.6.1/LICENSE` & `typer-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/README.md` & `typer-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 <p align="center">
 <a href="https://github.com/tiangolo/typer/actions?query=workflow%3ATest" target="_blank">
     <img src="https://github.com/tiangolo/typer/workflows/Test/badge.svg" alt="Test">
 </a>
 <a href="https://github.com/tiangolo/typer/actions?query=workflow%3APublish" target="_blank">
     <img src="https://github.com/tiangolo/typer/workflows/Publish/badge.svg" alt="Publish">
 </a>
-<a href="https://codecov.io/gh/tiangolo/typer" target="_blank">
-    <img src="https://img.shields.io/codecov/c/github/tiangolo/typer?color=%2334D058" alt="Coverage">
-</a>
+<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/typer" target="_blank">
+    <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/typer.svg" alt="Coverage">
 <a href="https://pypi.org/project/typer" target="_blank">
     <img src="https://img.shields.io/pypi/v/typer?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 </p>
 
 ---
```

### Comparing `typer-0.6.1/SECURITY.md` & `typer-0.7.0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/alternatives.md` & `typer-0.7.0/docs/alternatives.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Hug is a library to create APIs and CLIs, it uses parameters in functions to declare the required data.
 
 It inspired a lot of the ideas in **FastAPI** and **Typer**.
 
 !!! check "Inspired **Typer** to"
     Use function parameters to declare *CLI arguments* and *CLI options* as it simplifies a lot the development experience.
 
-### <a href="https://micheles.github.io/plac/" class="external-link" target="_blank">Plac</a>
+### <a href="https://plac.readthedocs.io/en/latest/" class="external-link" target="_blank">Plac</a>
 
 Plac is another library to create CLIs using parameters in functions, similar to Hug.
 
 !!! check "Inspired **Typer** to"
     Provide a simple way to use a function as a command line app, without having to create a complete app, with `typer.run(some_function)`.
 
 ### <a href="https://pydantic-docs.helpmanual.io/" class="external-link" target="_blank">Pydantic</a>
```

### Comparing `typer-0.6.1/docs/contributing.md` & `typer-0.7.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/css/termynal.css` & `typer-0.7.0/docs/css/termynal.css`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/features.md` & `typer-0.7.0/docs/features.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/help-typer.md` & `typer-0.7.0/docs/help-typer.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/img/github-social-preview.png` & `typer-0.7.0/docs/img/github-social-preview.png`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/img/github-social-preview.svg` & `typer-0.7.0/docs/img/github-social-preview.svg`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/img/icon-white.svg` & `typer-0.7.0/docs/img/icon-white.svg`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/img/logo-margin/logo-margin-vector.svg` & `typer-0.7.0/docs/img/logo-margin/logo-margin-vector.svg`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/img/logo-margin/logo-margin.svg` & `typer-0.7.0/docs/img/logo-margin/logo-margin.svg`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/img/pycharm-completion.png` & `typer-0.7.0/docs/img/pycharm-completion.png`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/img/vscode-completion.png` & `typer-0.7.0/docs/img/vscode-completion.png`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/index.md` & `typer-0.7.0/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 <p align="center">
 <a href="https://github.com/tiangolo/typer/actions?query=workflow%3ATest" target="_blank">
     <img src="https://github.com/tiangolo/typer/workflows/Test/badge.svg" alt="Test">
 </a>
 <a href="https://github.com/tiangolo/typer/actions?query=workflow%3APublish" target="_blank">
     <img src="https://github.com/tiangolo/typer/workflows/Publish/badge.svg" alt="Publish">
 </a>
-<a href="https://codecov.io/gh/tiangolo/typer" target="_blank">
-    <img src="https://img.shields.io/codecov/c/github/tiangolo/typer?color=%2334D058" alt="Coverage">
-</a>
+<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/typer" target="_blank">
+    <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/typer.svg" alt="Coverage">
 <a href="https://pypi.org/project/typer" target="_blank">
     <img src="https://img.shields.io/pypi/v/typer?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 </p>
 
 ---
```

### Comparing `typer-0.6.1/docs/js/custom.js` & `typer-0.7.0/docs/js/custom.js`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/js/termynal.js` & `typer-0.7.0/docs/js/termynal.js`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/overrides/main.html` & `typer-0.7.0/docs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/release-notes.md` & `typer-0.7.0/docs/release-notes.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,45 @@
 ## Latest Changes
 
 
+## 0.7.0
+
+### Features
+
+* ✨ Make `typer.run()` not add completion scripts by default, it only makes sense in installed apps. Also update docs for handling [autocompletion in CLI options](https://typer.tiangolo.com/tutorial/options-autocompletion/). PR [#488](https://github.com/tiangolo/typer/pull/488) by [@tiangolo](https://github.com/tiangolo).
+* ✨ Add support for Python 3.11, tests in CI and official marker. PR [#487](https://github.com/tiangolo/typer/pull/487) by [@tiangolo](https://github.com/tiangolo).
+* 👷 Add CI for Python 3.10. PR [#384](https://github.com/tiangolo/typer/pull/384) by [@tiangolo](https://github.com/tiangolo).
+
+### Fixes
+
+* 🎨 Fix type annotation of `typer.run()`. PR [#284](https://github.com/tiangolo/typer/pull/284) by [@yassu](https://github.com/yassu).
+* 🎨 Fix type annotations for `get_group`. PR [#430](https://github.com/tiangolo/typer/pull/430) by [@tiangolo](https://github.com/tiangolo).
+
+### Docs
+
+* 📝 Add note about how subcommands with function names using underscores are converted to dashes. PR [#403](https://github.com/tiangolo/typer/pull/403) by [@targhs](https://github.com/targhs).
+* 📝 Fix typo in docs at `docs/tutorial/commands/help.md`. PR [#466](https://github.com/tiangolo/typer/pull/466) by [@fepegar](https://github.com/fepegar).
+* ✏ Fix link in docs to `datetime.strptime()`. PR [#464](https://github.com/tiangolo/typer/pull/464) by [@Kobu](https://github.com/Kobu).
+* ✏ Update `first-steps.md`, clarify distinction between parameter and argument. PR [#176](https://github.com/tiangolo/typer/pull/176) by [@mccarthysean](https://github.com/mccarthysean).
+* ✏ Fix broken plac link. PR [#275](https://github.com/tiangolo/typer/pull/275) by [@mgielda](https://github.com/mgielda).
+
+### Internal
+
+* ✅ Add extra tests just for coverage because monkeypatching with strange imports confuses coverage. PR [#490](https://github.com/tiangolo/typer/pull/490) by [@tiangolo](https://github.com/tiangolo).
+* 🔧 Tweak pytest coverage. PR [#485](https://github.com/tiangolo/typer/pull/485) by [@tiangolo](https://github.com/tiangolo).
+* ➕ Bring back pytest-cov because coverage can't detect pytest-xdist. PR [#484](https://github.com/tiangolo/typer/pull/484) by [@tiangolo](https://github.com/tiangolo).
+* ⬆ Bump actions/upload-artifact from 2 to 3. PR [#477](https://github.com/tiangolo/typer/pull/477) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump actions/checkout from 2 to 3. PR [#478](https://github.com/tiangolo/typer/pull/478) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ [pre-commit.ci] pre-commit autoupdate. PR [#411](https://github.com/tiangolo/typer/pull/411) by [@pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci).
+* ⬆ Bump nwtgck/actions-netlify from 1.1.5 to 1.2.4. PR [#479](https://github.com/tiangolo/typer/pull/479) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* ⬆ Bump tiangolo/issue-manager from 0.2.0 to 0.4.0. PR [#481](https://github.com/tiangolo/typer/pull/481) by [@dependabot[bot]](https://github.com/apps/dependabot).
+* 👷 Move from pytest-cov to coverage and Codecov to Smokeshow. PR [#483](https://github.com/tiangolo/typer/pull/483) by [@tiangolo](https://github.com/tiangolo).
+* ➕ Add extra Material for MkDocs deps for docs. PR [#482](https://github.com/tiangolo/typer/pull/482) by [@tiangolo](https://github.com/tiangolo).
+* 🔧 Update Dependabot config. PR [#476](https://github.com/tiangolo/typer/pull/476) by [@tiangolo](https://github.com/tiangolo).
+
 ## 0.6.1
 
 ### Fixes
 
 * 🐛 Fix setting `FORCE_TERMINAL` with colors 2. PR [#424](https://github.com/tiangolo/typer/pull/424) by [@tiangolo](https://github.com/tiangolo).
 * 🐛 Fix setting `FORCE_TERMINAL` with colors. PR [#423](https://github.com/tiangolo/typer/pull/423) by [@tiangolo](https://github.com/tiangolo).
```

### Comparing `typer-0.6.1/docs/tutorial/app-dir.md` & `typer-0.7.0/docs/tutorial/app-dir.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/arguments/default.md` & `typer-0.7.0/docs/tutorial/arguments/default.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/arguments/envvar.md` & `typer-0.7.0/docs/tutorial/arguments/envvar.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/arguments/help.md` & `typer-0.7.0/docs/tutorial/arguments/help.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/arguments/optional.md` & `typer-0.7.0/docs/tutorial/arguments/optional.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/commands/arguments.md` & `typer-0.7.0/docs/tutorial/commands/arguments.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/commands/callback.md` & `typer-0.7.0/docs/tutorial/commands/callback.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/commands/context.md` & `typer-0.7.0/docs/tutorial/commands/context.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/commands/help.md` & `typer-0.7.0/docs/tutorial/commands/help.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
 <font color="#A5A5A1">│                            [default: no-force]                    │</font>
 <font color="#A5A5A1">│ </font><font color="#A1EFE4"><b>--help</b></font>                     Show this message and exit.            │
 <font color="#A5A5A1">╰───────────────────────────────────────────────────────────────────╯</font>
 ```
 
 </div>
 
-### Rich Markown
+### Rich Markdown
 
 If you set `rich_markup_mode="markdown"` when creating the `typer.Typer()` app, you will be able to use Markdown in the docstring:
 
 ```Python hl_lines="3  7  9-17  22  24-25"
 {!../docs_src/commands/help/tutorial005.py!}
 ```
```

### Comparing `typer-0.6.1/docs/tutorial/commands/index.md` & `typer-0.7.0/docs/tutorial/commands/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
     You put it on top of a function. Like a pretty decorative hat (I guess that's where the term came from).
 
     A "decorator" takes the function below and does something with it.
 
     In our case, this decorator tells **Typer** that the function below is a "`command`".
 
-Both ways, with `typer.run()` and creating the explicit application, achieve the same.
+Both ways, with `typer.run()` and creating the explicit application, achieve almost the same.
 
 !!! tip
     If your use case is solved with just `typer.run()`, that's fine, you don't have to create the explicit `app` and use `@app.command()`, etc.
 
     You might want to do that later when your app needs the extra features, but if it doesn't need them yet, that's fine.
 
 If you run the second example, with the explicit `app`, it works exactly the same:
@@ -110,14 +110,52 @@
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
 ```
 
 </div>
 
+## CLI application completion
+
+There's a little detail that is worth noting here.
+
+To get shell/tab completion, it's necessary to build a package that you and your users can install and **call directly**.
+
+So instead of running a Python script like:
+
+<div class="termy">
+
+```console
+$ python main.py
+
+✨ Some magic here ✨
+```
+
+</div>
+
+...It would be called like:
+
+<div class="termy">
+
+```console
+$ magic-app
+
+✨ Some magic here ✨
+```
+
+</div>
+
+Having a standalone program like that allows setting up shell/tab completion.
+
+The first step to be able to create an installable package like that is to use an explicit `typer.Typer()` app.
+
+Later you can learn all the process to create a standalone CLI application and [Build a Package](../package.md){.internal-link target=_blank}.
+
+But for now, it's just good to know that you are on that path. 😎
+
 ## A CLI application with multiple commands
 
 Coming back to the CLI applications with multiple commands/subcommands, **Typer** allows creating CLI applications with multiple of them.
 
 Now that you know how to create an explicit `typer.Typer()` application and add one command, let's see how to add multiple commands.
 
 Let's say that we have a CLI application to manage users.
```

### Comparing `typer-0.6.1/docs/tutorial/commands/name.md` & `typer-0.7.0/docs/tutorial/commands/name.md`

 * *Files 6% similar despite different names*

```diff
@@ -40,7 +40,17 @@
 // Test it
 $ python main.py create Camila
 
 Creating user: Camila
 ```
 
 </div>
+
+Note that any underscores in the function name will be replaced with dashes.
+
+So if your function is something like:
+
+```Python
+def create_user(username: str):
+    ...
+```
+Then the command name will be `create-user`.
```

### Comparing `typer-0.6.1/docs/tutorial/commands/one-or-multiple.md` & `typer-0.7.0/docs/tutorial/commands/one-or-multiple.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/commands/options.md` & `typer-0.7.0/docs/tutorial/commands/options.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/exceptions.md` & `typer-0.7.0/docs/tutorial/exceptions.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/first-steps.md` & `typer-0.7.0/docs/tutorial/first-steps.md`

 * *Files 1% similar despite different names*

```diff
@@ -428,22 +428,22 @@
 are called "Python function parameters" or "Python function arguments".
 
 !!! note "Technical Details"
     There's actually a very small distinction in Python between "parameter" and "argument".
 
     It's quite technical... and somewhat pedantic.
 
-    One refers to the variable name in a function *declaration*. Like:
+    *Parameter* refers to the variable name in a function *declaration*. Like:
 
     ```
     def bring_person(name: str, lastname: str = ""):
         pass
     ```
 
-    The other refers to the value passed when *calling* a function. Like:
+    *Argument* refers to the value passed when *calling* a function. Like:
 
     ```
     person = bring_person("Camila", lastname="Gutiérrez")
     ```
 
     ...but you will probably see them used interchangeably in most of the places (including here).
```

### Comparing `typer-0.6.1/docs/tutorial/index.md` & `typer-0.7.0/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/launch.md` & `typer-0.7.0/docs/tutorial/launch.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/multiple-values/arguments-with-multiple-values.md` & `typer-0.7.0/docs/tutorial/multiple-values/arguments-with-multiple-values.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/multiple-values/multiple-options.md` & `typer-0.7.0/docs/tutorial/multiple-values/multiple-options.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/multiple-values/options-with-multiple-values.md` & `typer-0.7.0/docs/tutorial/multiple-values/options-with-multiple-values.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/options/autocompletion.md` & `typer-0.7.0/docs/tutorial/options-autocompletion.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 Before checking how to provide custom completions, let's check again how it works.
 
 After installing completion (for your own Python package or for **Typer CLI**), when you use your CLI program and start adding a *CLI option* with `--` an then hit <kbd>TAB</kbd>, your shell will show you the available *CLI options* (the same for *CLI arguments*, etc).
 
 To check it quickly without creating a new Python package, install [Typer CLI](../../typer-cli.md){.internal-link target=_blank}.
 
-Then let's create small example script:
+Then let's create small example program:
 
 ```Python
-{!../docs_src/options/autocompletion/tutorial001.py!}
+{!../docs_src/options_autocompletion/tutorial001.py!}
 ```
 
 And let's try it with **Typer CLI** to get completion:
 
 <div class="termy">
 
 ```console
@@ -46,16 +46,16 @@
 
 ## Custom completion for values
 
 Right now we get completion for the *CLI option* names, but not for the values.
 
 We can provide completion for the values creating an `autocompletion` function, similar to the `callback` functions from [CLI Option Callback and Context](./callback-and-context.md){.internal-link target=_blank}:
 
-```Python hl_lines="4 5  10"
-{!../docs_src/options/autocompletion/tutorial002.py!}
+```Python hl_lines="4-5  14"
+{!../docs_src/options_autocompletion/tutorial002.py!}
 ```
 
 We return a `list` of strings from the `complete_name()` function.
 
 And then we get those values when using completion:
 
 <div class="termy">
@@ -77,16 +77,16 @@
 
 But we can fix that so that it always works correctly.
 
 Modify the `complete_name()` function to receive a parameter of type `str`, it will contain the incomplete value.
 
 Then we can check and return only the values that start with the incomplete value from the command line:
 
-```Python hl_lines="6 7 8 9 10 11"
-{!../docs_src/options/autocompletion/tutorial003.py!}
+```Python hl_lines="6-11"
+{!../docs_src/options_autocompletion/tutorial003.py!}
 ```
 
 Now let's try it:
 
 <div class="termy">
 
 ```console
@@ -116,15 +116,15 @@
 We can provide that extra help text so that those shells can show it.
 
 In the `complete_name()` function, instead of providing one `str` per completion element, we provide a `tuple` with 2 items. The first item is the actual completion string, and the second item is the help text.
 
 So, in the end, we return a `list` of `tuples` of `str`:
 
 ```Python hl_lines="3 4 5 6 7  10 11 12 13 14 15 16"
-{!../docs_src/options/autocompletion/tutorial004.py!}
+{!../docs_src/options_autocompletion/tutorial004.py!}
 ```
 
 !!! tip
     If you want to have help text for each item, make sure each item in the list is a `tuple`. Not a `list`.
 
     Click checks specifically for a `tuple` when extracting the help text.
 
@@ -153,15 +153,15 @@
 ## Simplify with `yield`
 
 Instead of creating and returning a list with values (`str` or `tuple`), we can use `yield` with each value that we want in the completion.
 
 That way our function will be a <a href="https://docs.python.org/3.8/glossary.html#index-19" class="external-link" target="_blank">generator</a> that **Typer** (actually Click) can iterate:
 
 ```Python hl_lines="10 11 12 13"
-{!../docs_src/options/autocompletion/tutorial005.py!}
+{!../docs_src/options_autocompletion/tutorial005.py!}
 ```
 
 That simplifies our code a bit and works the same.
 
 !!! tip
     If all the `yield` part seems complex for you, don't worry, you can just use the version with the `list` above.
 
@@ -181,16 +181,16 @@
 !!! tip
     You will learn more about *CLI parameters* with multiple values later in the tutorial.
 
     So, for now, take this as a sneak peek 😉.
 
 For this we use a `List` of `str`:
 
-```Python hl_lines="6 7 8"
-{!../docs_src/options/autocompletion/tutorial006.py!}
+```Python hl_lines="8-11"
+{!../docs_src/options_autocompletion/tutorial006.py!}
 ```
 
 And then we can use it like:
 
 <div class="termy">
 
 ```console
@@ -209,15 +209,15 @@
 For that, we will access and use the "Context". When you create a **Typer** application it uses Click underneath. And every Click application has a special object called a <a href="https://click.palletsprojects.com/en/7.x/commands/#nested-handling-and-contexts" class="external-link" target="_blank">"Context"</a> that is normally hidden.
 
 But you can access the context by declaring a function parameter of type `typer.Context`.
 
 And from that context you can get the current values for each parameter.
 
 ```Python hl_lines="12 13  15"
-{!../docs_src/options/autocompletion/tutorial007.py!}
+{!../docs_src/options_autocompletion/tutorial007.py!}
 ```
 
 We are getting the `names` already provided with `--name` in the command line before this completion was triggered.
 
 If there's no `--name` in the command line, it will be `None`, so we use `or []` to make sure we have a `list` (even if empty) to check its contents later.
 
 Then, when we have a completion candidate, we check if each `name` was already provided with `--name` by checking if it's in that list of `names` with `name not in names`.
@@ -278,15 +278,15 @@
 The completion system only reads from "standard output", so, printing to "standard error" won't break completion. 🚀
 
 You can print to "standard error" with a **Rich** `Console(stderr=True)`.
 
 Using `stderr=True` tells **Rich** that the output should be shown in "standard error".
 
 ```Python hl_lines="12  15-16"
-{!../docs_src/options/autocompletion/tutorial008.py!}
+{!../docs_src/options_autocompletion/tutorial008.py!}
 ```
 
 !!! info
     If you can't install and use Rich, you can also use `print(lastname, file=sys.stderr)` or `typer.echo("some text", err=True)` instead.
 
 We get all the *CLI parameters* as a raw `list` of `str` by declaring a parameter with type `List[str]`, here it's named `args`.
 
@@ -319,15 +319,15 @@
     But it's probably useful only in very advanced use cases.
 
 ## Getting the Context and the raw *CLI parameters*
 
 Of course, you can declare everything if you need it, the context, the raw *CLI parameters*, and the incomplete `str`:
 
 ```Python hl_lines="15"
-{!../docs_src/options/autocompletion/tutorial009.py!}
+{!../docs_src/options_autocompletion/tutorial009.py!}
 ```
 
 Check it:
 
 <div class="termy">
 
 ```console
```

### Comparing `typer-0.6.1/docs/tutorial/options/callback-and-context.md` & `typer-0.7.0/docs/tutorial/options/callback-and-context.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/options/help.md` & `typer-0.7.0/docs/tutorial/options/help.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/options/name.md` & `typer-0.7.0/docs/tutorial/options/name.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/options/password.md` & `typer-0.7.0/docs/tutorial/options/password.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/options/prompt.md` & `typer-0.7.0/docs/tutorial/options/prompt.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/options/required.md` & `typer-0.7.0/docs/tutorial/options/required.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/options/version.md` & `typer-0.7.0/docs/tutorial/options/version.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/package.md` & `typer-0.7.0/docs/tutorial/package.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/parameter-types/bool.md` & `typer-0.7.0/docs/tutorial/parameter-types/bool.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/parameter-types/datetime.md` & `typer-0.7.0/docs/tutorial/parameter-types/datetime.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 </div>
 
 ## Custom date format
 
 You can also customize the formats received for the `datetime` with the `formats` parameter.
 
-`formats` receives a list of strings with the date formats that would be passed to <a href="https://docs.python.org/3/library/datetime.html#datetime.date.strftime" class="external-link" target="_blank">datetime.strptime()</a>.
+`formats` receives a list of strings with the date formats that would be passed to <a href="https://docs.python.org/3/library/datetime.html#datetime.datetime.strptime" class="external-link" target="_blank">datetime.strptime()</a>.
 
 For example, let's imagine that you want to accept an ISO formatted datetime, but for some strange reason, you also want to accept a format with:
 
 * first the month
 * then the day
 * then the year
 * separated with "`/`"
```

### Comparing `typer-0.6.1/docs/tutorial/parameter-types/enum.md` & `typer-0.7.0/docs/tutorial/parameter-types/enum.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/parameter-types/file.md` & `typer-0.7.0/docs/tutorial/parameter-types/file.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/parameter-types/index.md` & `typer-0.7.0/docs/tutorial/parameter-types/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/parameter-types/number.md` & `typer-0.7.0/docs/tutorial/parameter-types/number.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/parameter-types/path.md` & `typer-0.7.0/docs/tutorial/parameter-types/path.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/parameter-types/uuid.md` & `typer-0.7.0/docs/tutorial/parameter-types/uuid.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/printing.md` & `typer-0.7.0/docs/tutorial/printing.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/progressbar.md` & `typer-0.7.0/docs/tutorial/progressbar.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/prompt.md` & `typer-0.7.0/docs/tutorial/prompt.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/subcommands/add-typer.md` & `typer-0.7.0/docs/tutorial/subcommands/add-typer.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/subcommands/callback-override.md` & `typer-0.7.0/docs/tutorial/subcommands/callback-override.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/subcommands/index.md` & `typer-0.7.0/docs/tutorial/subcommands/index.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/subcommands/name-and-help.md` & `typer-0.7.0/docs/tutorial/subcommands/name-and-help.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/subcommands/nested-subcommands.md` & `typer-0.7.0/docs/tutorial/subcommands/nested-subcommands.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/subcommands/single-file.md` & `typer-0.7.0/docs/tutorial/subcommands/single-file.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/terminating.md` & `typer-0.7.0/docs/tutorial/terminating.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/testing.md` & `typer-0.7.0/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/tutorial/using-click.md` & `typer-0.7.0/docs/tutorial/using-click.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs/typer-cli.md` & `typer-0.7.0/docs/typer-cli.md`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/commands/callback/tutorial001.py` & `typer-0.7.0/docs_src/commands/callback/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/commands/help/tutorial001.py` & `typer-0.7.0/docs_src/commands/help/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/commands/help/tutorial004.py` & `typer-0.7.0/docs_src/commands/help/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/commands/help/tutorial005.py` & `typer-0.7.0/docs_src/commands/help/tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/commands/help/tutorial006.py` & `typer-0.7.0/docs_src/commands/help/tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/commands/help/tutorial007.py` & `typer-0.7.0/docs_src/commands/help/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/commands/options/tutorial001.py` & `typer-0.7.0/docs_src/commands/options/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/launch/tutorial002.py` & `typer-0.7.0/docs_src/launch/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/options/autocompletion/tutorial004.py` & `typer-0.7.0/docs_src/options_autocompletion/tutorial004.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,17 +12,21 @@
     for name, help_text in valid_completion_items:
         if name.startswith(incomplete):
             completion_item = (name, help_text)
             completion.append(completion_item)
     return completion
 
 
+app = typer.Typer()
+
+
+@app.command()
 def main(
     name: str = typer.Option(
         "World", help="The name to say hi to.", autocompletion=complete_name
     )
 ):
     print(f"Hello {name}")
 
 
 if __name__ == "__main__":
-    typer.run(main)
+    app()
```

### Comparing `typer-0.6.1/docs_src/options/autocompletion/tutorial005.py` & `typer-0.7.0/docs_src/options_autocompletion/tutorial009.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,37 @@
+from typing import List
+
 import typer
+from rich.console import Console
 
 valid_completion_items = [
     ("Camila", "The reader of books."),
     ("Carlos", "The writer of scripts."),
     ("Sebastian", "The type hints guy."),
 ]
 
+err_console = Console(stderr=True)
+
 
-def complete_name(incomplete: str):
+def complete_name(ctx: typer.Context, args: List[str], incomplete: str):
+    err_console.print(f"{args}")
+    names = ctx.params.get("name") or []
     for name, help_text in valid_completion_items:
-        if name.startswith(incomplete):
+        if name.startswith(incomplete) and name not in names:
             yield (name, help_text)
 
 
+app = typer.Typer()
+
+
+@app.command()
 def main(
-    name: str = typer.Option(
-        "World", help="The name to say hi to.", autocompletion=complete_name
+    name: List[str] = typer.Option(
+        ["World"], help="The name to say hi to.", autocompletion=complete_name
     )
 ):
-    print(f"Hello {name}")
+    for n in name:
+        print(f"Hello {n}")
 
 
 if __name__ == "__main__":
-    typer.run(main)
+    app()
```

### Comparing `typer-0.6.1/docs_src/options/autocompletion/tutorial007.py` & `typer-0.7.0/docs_src/options_autocompletion/tutorial007.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 def complete_name(ctx: typer.Context, incomplete: str):
     names = ctx.params.get("name") or []
     for name, help_text in valid_completion_items:
         if name.startswith(incomplete) and name not in names:
             yield (name, help_text)
 
 
+app = typer.Typer()
+
+
+@app.command()
 def main(
     name: List[str] = typer.Option(
         ["World"], help="The name to say hi to.", autocompletion=complete_name
     )
 ):
     for n in name:
         print(f"Hello {n}")
 
 
 if __name__ == "__main__":
-    typer.run(main)
+    app()
```

### Comparing `typer-0.6.1/docs_src/options/autocompletion/tutorial008.py` & `typer-0.7.0/docs_src/options_autocompletion/tutorial008.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,18 +15,22 @@
 def complete_name(args: List[str], incomplete: str):
     err_console.print(f"{args}")
     for name, help_text in valid_completion_items:
         if name.startswith(incomplete):
             yield (name, help_text)
 
 
+app = typer.Typer()
+
+
+@app.command()
 def main(
     name: List[str] = typer.Option(
         ["World"], help="The name to say hi to.", autocompletion=complete_name
     )
 ):
     for n in name:
         print(f"Hello {n}")
 
 
 if __name__ == "__main__":
-    typer.run(main)
+    app()
```

### Comparing `typer-0.6.1/docs_src/options/help/tutorial002.py` & `typer-0.7.0/docs_src/options/help/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/options/version/tutorial002.py` & `typer-0.7.0/docs_src/options/version/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/options/version/tutorial003.py` & `typer-0.7.0/docs_src/options/version/tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/parameter_types/file/tutorial004.py` & `typer-0.7.0/docs_src/parameter_types/file/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/parameter_types/path/tutorial001.py` & `typer-0.7.0/docs_src/parameter_types/path/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/subcommands/callback_override/tutorial004.py` & `typer-0.7.0/docs_src/subcommands/callback_override/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/subcommands/name_help/tutorial006.py` & `typer-0.7.0/docs_src/subcommands/name_help/tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/subcommands/name_help/tutorial007.py` & `typer-0.7.0/docs_src/subcommands/name_help/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/subcommands/name_help/tutorial008.py` & `typer-0.7.0/docs_src/subcommands/name_help/tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/subcommands/tutorial002/main.py` & `typer-0.7.0/docs_src/subcommands/tutorial002/main.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/terminating/tutorial001.py` & `typer-0.7.0/docs_src/terminating/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/docs_src/using_click/tutorial003.py` & `typer-0.7.0/docs_src/using_click/tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/mkdocs.yml` & `typer-0.7.0/mkdocs.yml`

 * *Files 0% similar despite different names*

```diff
@@ -37,24 +37,24 @@
           - CLI Options with Help: tutorial/options/help.md
           - Required CLI Options: tutorial/options/required.md
           - CLI Option Prompt: tutorial/options/prompt.md
           - Password CLI Option and Confirmation Prompt: tutorial/options/password.md
           - CLI Option Name: tutorial/options/name.md
           - CLI Option Callback and Context: tutorial/options/callback-and-context.md
           - Version CLI Option, is_eager: tutorial/options/version.md
-          - CLI Option autocompletion: tutorial/options/autocompletion.md
       - Commands:
           - Commands Intro: tutorial/commands/index.md
           - Command CLI Arguments: tutorial/commands/arguments.md
           - Command CLI Options: tutorial/commands/options.md
           - Command Help: tutorial/commands/help.md
           - Custom Command Name: tutorial/commands/name.md
           - Typer Callback: tutorial/commands/callback.md
           - One or Multiple Commands: tutorial/commands/one-or-multiple.md
           - Using the Context: tutorial/commands/context.md
+      - CLI Option autocompletion: tutorial/options-autocompletion.md
       - CLI Parameter Types:
           - CLI Parameter Types Intro: tutorial/parameter-types/index.md
           - Number: tutorial/parameter-types/number.md
           - Boolean CLI Options: tutorial/parameter-types/bool.md
           - UUID: tutorial/parameter-types/uuid.md
           - DateTime: tutorial/parameter-types/datetime.md
           - Enum - Choices: tutorial/parameter-types/enum.md
```

### Comparing `typer-0.6.1/pyproject.toml` & `typer-0.7.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -20,42 +20,47 @@
     "Typing :: Typed",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License"
     ]
 requires = [
     "click >= 7.1.1, <9.0.0"
 ]
 description-file = "README.md"
 requires-python = ">=3.6"
 
 [tool.flit.metadata.urls]
 Documentation = "https://typer.tiangolo.com/"
 
 [tool.flit.metadata.requires-extra]
 test = [
     "shellingham >=1.3.0,<2.0.0",
-    "pytest >=4.4.0,<5.4.0",
-    "pytest-cov >=2.10.0,<3.0.0",
-    "coverage >=5.2,<6.0",
-    "pytest-xdist >=1.32.0,<2.0.0",
+    "pytest >=4.4.0,<8.0.0",
+    "pytest-cov >=2.10.0,<5.0.0",
+    "coverage >=6.2,<7.0",
+    "pytest-xdist >=1.32.0,<4.0.0",
     "pytest-sugar >=0.9.4,<0.10.0",
     "mypy ==0.910",
     "black >=22.3.0,<23.0.0",
     "isort >=5.0.6,<6.0.0",
     "rich >=10.11.0,<13.0.0",
 ]
 doc = [
     "mkdocs >=1.1.2,<2.0.0",
     "mkdocs-material >=8.1.4,<9.0.0",
     "mdx-include >=1.4.1,<2.0.0",
+    "pillow >=9.3.0,<10.0.0",
+    "cairosvg >=2.5.2,<3.0.0",
 ]
 dev = [
     "autoflake >=1.3.1,<2.0.0",
     "flake8 >=3.8.3,<4.0.0",
     "pre-commit >=2.17.0,<3.0.0",
 ]
 all = [
@@ -68,7 +73,23 @@
 profile = "black"
 known_third_party = ["typer", "click"]
 skip_glob = [
     "docs_src/subcommands/tutorial001/main.py",
     "docs_src/subcommands/tutorial003/lands.py",
     "docs_src/subcommands/tutorial003/main.py",
     ]
+
+[tool.pytest.ini_options]
+addopts = [
+  "--strict-config",
+  "--strict-markers",
+]
+xfail_strict = true
+junit_family = "xunit2"
+filterwarnings = [
+    "error",
+    # TODO: until I refactor completion to use the new shell_complete
+    "ignore:'autocompletion' is renamed to 'shell_complete'. The old name is deprecated and will be removed in Click 8.1. See the docs about 'Parameter' for information about new behavior.:DeprecationWarning:typer",
+    'ignore:starlette.middleware.wsgi is deprecated and will be removed in a future release\..*:DeprecationWarning:starlette',
+    # For pytest-xdist
+    'ignore::DeprecationWarning:xdist',
+]
```

### Comparing `typer-0.6.1/tests/assets/compat_click7_8.py` & `typer-0.7.0/tests/assets/compat_click7_8.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/assets/completion_no_types.py` & `typer-0.7.0/tests/assets/completion_no_types.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/assets/completion_no_types_order.py` & `typer-0.7.0/tests/assets/completion_no_types_order.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_compat/test_option_get_help.py` & `typer-0.7.0/tests/test_compat/test_option_get_help.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_completion/test_completion.py` & `typer-0.7.0/tests/test_completion/test_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import subprocess
 import sys
 from pathlib import Path
 
-from docs_src.first_steps import tutorial001 as mod
+from docs_src.commands.index import tutorial001 as mod
 
 
 def test_show_completion():
     result = subprocess.run(
         [
             "bash",
             "-c",
```

### Comparing `typer-0.6.1/tests/test_completion/test_completion_complete.py` & `typer-0.7.0/tests/test_completion/test_completion_complete.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_completion/test_completion_complete_no_help.py` & `typer-0.7.0/tests/test_completion/test_completion_complete_no_help.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_completion/test_completion_install.py` & `typer-0.7.0/tests/test_completion/test_completion_install.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from unittest import mock
 
 import shellingham
 import typer
 from typer.testing import CliRunner
 
-from docs_src.first_steps import tutorial001 as mod
+from docs_src.commands.index import tutorial001 as mod
 
 runner = CliRunner()
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_completion_install_no_shell():
```

### Comparing `typer-0.6.1/tests/test_completion/test_completion_show.py` & `typer-0.7.0/tests/test_completion/test_completion_show.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import subprocess
 
-from docs_src.first_steps import tutorial001 as mod
+from docs_src.commands.index import tutorial001 as mod
 
 
 def test_completion_show_no_shell():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, "--show-completion"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
```

### Comparing `typer-0.6.1/tests/test_exit_errors.py` & `typer-0.7.0/tests/test_exit_errors.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_others.py` & `typer-0.7.0/tests/test_others.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_rich_utils.py` & `typer-0.7.0/tests/test_rich_utils.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tracebacks.py` & `typer-0.7.0/tests/test_tracebacks.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_context/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_context/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_context/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_context/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_context/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial005.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial006.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial007.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_help/test_tutorial008.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_index/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_index/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_index/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_index/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_name/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_name/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_commands/test_options/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_commands/test_options/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_exceptions/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_exceptions/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_exceptions/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_exceptions/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_exceptions/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial005.py` & `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_first_steps/test_tutorial006.py` & `typer-0.7.0/tests/test_tutorial/test_first_steps/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_callback/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_callback/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_callback/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_callback/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import os
 import subprocess
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.options.autocompletion import tutorial002 as mod
+from docs_src.options_autocompletion import tutorial002 as mod
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
-
 
 def test_completion():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
@@ -27,15 +23,15 @@
     )
     assert "Camila" in result.stdout
     assert "Carlos" in result.stdout
     assert "Sebastian" in result.stdout
 
 
 def test_1():
-    result = runner.invoke(app, ["--name", "Camila"])
+    result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, "--help"],
```

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 import os
 import subprocess
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.options.autocompletion import tutorial003 as mod
+from docs_src.options_autocompletion import tutorial004 as mod
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
-
 
 def test_completion():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL003.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial003.py --name Seb",
+            "_TUTORIAL004.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial004_aux.py --name ",
             "_TYPER_COMPLETE_TESTING": "True",
         },
     )
-    assert "Camila" not in result.stdout
-    assert "Carlos" not in result.stdout
-    assert "Sebastian" in result.stdout
+    assert '"Camila":"The reader of books."' in result.stdout
+    assert '"Carlos":"The writer of scripts."' in result.stdout
+    assert '"Sebastian":"The type hints guy."' in result.stdout
 
 
 def test_1():
-    result = runner.invoke(app, ["--name", "Camila"])
+    result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, "--help"],
```

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_version/test_tutorial003.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 import os
 import subprocess
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.options.autocompletion import tutorial004 as mod
+from docs_src.options.version import tutorial003 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
-def test_completion():
-    result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        encoding="utf-8",
-        env={
-            **os.environ,
-            "_TUTORIAL004.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial004.py --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
-        },
-    )
-    assert '"Camila":"The reader of books."' in result.stdout
-    assert '"Carlos":"The writer of scripts."' in result.stdout
-    assert '"Sebastian":"The type hints guy."' in result.stdout
+def test_1():
+    result = runner.invoke(app, ["--name", "Rick", "--version"])
+    assert result.exit_code == 0
+    assert "Awesome CLI Version: 0.1.0" in result.output
 
 
-def test_1():
+def test_2():
+    result = runner.invoke(app, ["--name", "rick"])
+    assert result.exit_code != 0
+    assert "Invalid value for '--name': Only Camila is allowed" in result.output
+
+
+def test_3():
     result = runner.invoke(app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
+
+
+def test_completion():
+    result = subprocess.run(
+        ["coverage", "run", mod.__file__, " "],
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        encoding="utf-8",
+        env={
+            **os.environ,
+            "_TUTORIAL003.PY_COMPLETE": "complete_bash",
+            "COMP_WORDS": "tutorial003.py --name Rick --v",
+            "COMP_CWORD": "3",
+            "_TYPER_COMPLETE_TESTING": "True",
+        },
+    )
+    assert "--version" in result.stdout
```

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial007.py` & `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import os
 import subprocess
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.options.autocompletion import tutorial007 as mod
+from docs_src.options_autocompletion import tutorial007 as mod
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
-
 
 def test_completion():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
@@ -27,15 +23,15 @@
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' not in result.stdout
 
 
 def test_1():
-    result = runner.invoke(app, ["--name", "Camila", "--name", "Sebastian"])
+    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
     assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
```

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial008.py` & `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import os
 import subprocess
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.options.autocompletion import tutorial008 as mod
+from docs_src.options_autocompletion import tutorial008 as mod
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
-
 
 def test_completion():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
@@ -29,15 +25,15 @@
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' in result.stdout
     # TODO: when deprecating Click 7, remove second option
     assert "[]" in result.stderr or "['--name']" in result.stderr
 
 
 def test_1():
-    result = runner.invoke(app, ["--name", "Camila", "--name", "Sebastian"])
+    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
     assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
```

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_completion/test_tutorial009.py` & `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import os
 import subprocess
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.options.autocompletion import tutorial009 as mod
+from docs_src.options_autocompletion import tutorial009 as mod
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
-
 
 def test_completion():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, " "],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
@@ -29,15 +25,15 @@
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' not in result.stdout
     # TODO: when deprecating Click 7, remove second option
     assert "[]" in result.stderr or "['--name', 'Sebastian', '--name']" in result.stderr
 
 
 def test_1():
-    result = runner.invoke(app, ["--name", "Camila", "--name", "Sebastian"])
+    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
     assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
```

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_help/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_help/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_help/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_name/test_tutorial005.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_name/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_required/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_options/test_required/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_options/test_version/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,42 @@
 import os
 import subprocess
 
-import typer
 from typer.testing import CliRunner
 
-from docs_src.options.version import tutorial003 as mod
+from docs_src.options_autocompletion import tutorial003 as mod
 
 runner = CliRunner()
 
-app = typer.Typer()
-app.command()(mod.main)
 
-
-def test_1():
-    result = runner.invoke(app, ["--name", "Rick", "--version"])
-    assert result.exit_code == 0
-    assert "Awesome CLI Version: 0.1.0" in result.output
-
-
-def test_2():
-    result = runner.invoke(app, ["--name", "rick"])
-    assert result.exit_code != 0
-    assert "Invalid value for '--name': Only Camila is allowed" in result.output
+def test_completion():
+    result = subprocess.run(
+        ["coverage", "run", mod.__file__, " "],
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        encoding="utf-8",
+        env={
+            **os.environ,
+            "_TUTORIAL003.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial003.py --name Seb",
+            "_TYPER_COMPLETE_TESTING": "True",
+        },
+    )
+    assert "Camila" not in result.stdout
+    assert "Carlos" not in result.stdout
+    assert "Sebastian" in result.stdout
 
 
-def test_3():
-    result = runner.invoke(app, ["--name", "Camila"])
+def test_1():
+    result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
 
 
 def test_script():
     result = subprocess.run(
         ["coverage", "run", mod.__file__, "--help"],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         encoding="utf-8",
     )
     assert "Usage" in result.stdout
-
-
-def test_completion():
-    result = subprocess.run(
-        ["coverage", "run", mod.__file__, " "],
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        encoding="utf-8",
-        env={
-            **os.environ,
-            "_TUTORIAL003.PY_COMPLETE": "complete_bash",
-            "COMP_WORDS": "tutorial003.py --name Rick --v",
-            "COMP_CWORD": "3",
-            "_TYPER_COMPLETE_TESTING": "True",
-        },
-    )
-    assert "--version" in result.stdout
```

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_prompt/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_prompt/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_prompt/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_prompt/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_subcommands/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_subcommands/test_tutorial003.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import subprocess
 
 import pytest
 from typer.testing import CliRunner
 
 from docs_src.subcommands import tutorial003
+from docs_src.subcommands.tutorial003 import items, users
 
 runner = CliRunner()
 
 
 @pytest.fixture()
 def mod(monkeypatch):
     with monkeypatch.context() as m:
@@ -42,26 +43,38 @@
     assert "sell" in result.output
 
 
 def test_items_create(app):
     result = runner.invoke(app, ["items", "create", "Wand"])
     assert result.exit_code == 0
     assert "Creating item: Wand" in result.output
+    # For coverage, becauses the monkeypatch above sometimes confuses coverage
+    result = runner.invoke(items.app, ["create", "Wand"])
+    assert result.exit_code == 0
+    assert "Creating item: Wand" in result.output
 
 
 def test_items_sell(app):
     result = runner.invoke(app, ["items", "sell", "Vase"])
     assert result.exit_code == 0
     assert "Selling item: Vase" in result.output
+    # For coverage, becauses the monkeypatch above sometimes confuses coverage
+    result = runner.invoke(items.app, ["sell", "Vase"])
+    assert result.exit_code == 0
+    assert "Selling item: Vase" in result.output
 
 
 def test_items_delete(app):
     result = runner.invoke(app, ["items", "delete", "Vase"])
     assert result.exit_code == 0
     assert "Deleting item: Vase" in result.output
+    # For coverage, becauses the monkeypatch above sometimes confuses coverage
+    result = runner.invoke(items.app, ["delete", "Vase"])
+    assert result.exit_code == 0
+    assert "Deleting item: Vase" in result.output
 
 
 def test_help_users(app):
     result = runner.invoke(app, ["users", "--help"])
     assert result.exit_code == 0
     assert "[OPTIONS] COMMAND [ARGS]..." in result.output
     assert "Commands" in result.output
@@ -70,20 +83,28 @@
     assert "sell" not in result.output
 
 
 def test_users_create(app):
     result = runner.invoke(app, ["users", "create", "Camila"])
     assert result.exit_code == 0
     assert "Creating user: Camila" in result.output
+    # For coverage, becauses the monkeypatch above sometimes confuses coverage
+    result = runner.invoke(users.app, ["create", "Camila"])
+    assert result.exit_code == 0
+    assert "Creating user: Camila" in result.output
 
 
 def test_users_delete(app):
     result = runner.invoke(app, ["users", "delete", "Camila"])
     assert result.exit_code == 0
     assert "Deleting user: Camila" in result.output
+    # For coverage, becauses the monkeypatch above sometimes confuses coverage
+    result = runner.invoke(users.app, ["delete", "Camila"])
+    assert result.exit_code == 0
+    assert "Deleting user: Camila" in result.output
 
 
 def test_help_lands(app):
     result = runner.invoke(app, ["lands", "--help"])
     assert result.exit_code == 0
     assert "lands [OPTIONS] COMMAND [ARGS]..." in result.output
     assert "Commands" in result.output
```

### Comparing `typer-0.6.1/tests/test_tutorial/test_terminating/test_tutorial001.py` & `typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_terminating/test_tutorial002.py` & `typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_terminating/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_terminating/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_using_click/test_tutorial003.py` & `typer-0.7.0/tests/test_tutorial/test_using_click/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_tutorial/test_using_click/test_tutorial004.py` & `typer-0.7.0/tests/test_tutorial/test_using_click/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/tests/test_type_conversion.py` & `typer-0.7.0/tests/test_type_conversion.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/__init__.py` & `typer-0.7.0/typer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Typer, build great CLIs. Easy to code. Based on Python type hints."""
 
-__version__ = "0.6.1"
+__version__ = "0.7.0"
 
 from shutil import get_terminal_size as get_terminal_size
 
 from click.exceptions import Abort as Abort
 from click.exceptions import BadParameter as BadParameter
 from click.exceptions import Exit as Exit
 from click.termui import clear as clear
```

### Comparing `typer-0.6.1/typer/_completion_click7.py` & `typer-0.7.0/typer/_completion_click7.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/_completion_click8.py` & `typer-0.7.0/typer/_completion_click8.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/_completion_shared.py` & `typer-0.7.0/typer/_completion_shared.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/completion.py` & `typer-0.7.0/typer/completion.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/core.py` & `typer-0.7.0/typer/core.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/main.py` & `typer-0.7.0/typer/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
                     pretty_exceptions_show_locals=self.pretty_exceptions_show_locals,
                     pretty_exceptions_short=self.pretty_exceptions_short,
                 ),
             )
             raise e
 
 
-def get_group(typer_instance: Typer) -> click.Command:
+def get_group(typer_instance: Typer) -> TyperGroup:
     group = get_group_from_info(
         TyperInfo(typer_instance),
         pretty_exceptions_short=typer_instance.pretty_exceptions_short,
         rich_markup_mode=typer_instance.rich_markup_mode,
     )
     return group
 
@@ -343,15 +343,15 @@
     if (
         typer_instance.registered_callback
         or typer_instance.info.callback
         or typer_instance.registered_groups
         or len(typer_instance.registered_commands) > 1
     ):
         # Create a Group
-        click_command = get_group(typer_instance)
+        click_command: click.Command = get_group(typer_instance)
         if typer_instance._add_completion:
             click_command.params.append(click_install_param)
             click_command.params.append(click_show_param)
         return click_command
     elif len(typer_instance.registered_commands) == 1:
         # Create a single Command
         single_command = typer_instance.registered_commands[0]
@@ -470,15 +470,15 @@
 
 
 def get_group_from_info(
     group_info: TyperInfo,
     *,
     pretty_exceptions_short: bool,
     rich_markup_mode: MarkupMode,
-) -> click.Command:
+) -> TyperGroup:
     assert (
         group_info.typer_instance
     ), "A Typer instance is needed to generate a Click Group"
     commands: Dict[str, click.Command] = {}
     for command_info in group_info.typer_instance.registered_commands:
         command = get_command_from_info(
             command_info=command_info,
@@ -1040,11 +1040,11 @@
             use_params[incomplete_name] = incomplete
         return callback(**use_params)  # type: ignore
 
     update_wrapper(wrapper, callback)
     return wrapper
 
 
-def run(function: Callable[..., Any]) -> Any:
-    app = Typer()
+def run(function: Callable[..., Any]) -> None:
+    app = Typer(add_completion=False)
     app.command()(function)
     app()
```

### Comparing `typer-0.6.1/typer/models.py` & `typer-0.7.0/typer/models.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/params.py` & `typer-0.7.0/typer/params.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/rich_utils.py` & `typer-0.7.0/typer/rich_utils.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/testing.py` & `typer-0.7.0/typer/testing.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/typer/utils.py` & `typer-0.7.0/typer/utils.py`

 * *Files identical despite different names*

### Comparing `typer-0.6.1/PKG-INFO` & `typer-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer
-Version: 0.6.1
+Version: 0.7.0
 Summary: Typer, build great CLIs. Easy to code. Based on Python type hints.
 Home-page: https://github.com/tiangolo/typer
 Author: Sebastián Ramírez
 Author-email: tiangolo@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -19,30 +19,35 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click >= 7.1.1, <9.0.0
 Requires-Dist: colorama >=0.4.3,<0.5.0 ; extra == "all"
 Requires-Dist: shellingham >=1.3.0,<2.0.0 ; extra == "all"
 Requires-Dist: rich >=10.11.0,<13.0.0 ; extra == "all"
 Requires-Dist: autoflake >=1.3.1,<2.0.0 ; extra == "dev"
 Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "dev"
 Requires-Dist: pre-commit >=2.17.0,<3.0.0 ; extra == "dev"
 Requires-Dist: mkdocs >=1.1.2,<2.0.0 ; extra == "doc"
 Requires-Dist: mkdocs-material >=8.1.4,<9.0.0 ; extra == "doc"
 Requires-Dist: mdx-include >=1.4.1,<2.0.0 ; extra == "doc"
+Requires-Dist: pillow >=9.3.0,<10.0.0 ; extra == "doc"
+Requires-Dist: cairosvg >=2.5.2,<3.0.0 ; extra == "doc"
 Requires-Dist: shellingham >=1.3.0,<2.0.0 ; extra == "test"
-Requires-Dist: pytest >=4.4.0,<5.4.0 ; extra == "test"
-Requires-Dist: pytest-cov >=2.10.0,<3.0.0 ; extra == "test"
-Requires-Dist: coverage >=5.2,<6.0 ; extra == "test"
-Requires-Dist: pytest-xdist >=1.32.0,<2.0.0 ; extra == "test"
+Requires-Dist: pytest >=4.4.0,<8.0.0 ; extra == "test"
+Requires-Dist: pytest-cov >=2.10.0,<5.0.0 ; extra == "test"
+Requires-Dist: coverage >=6.2,<7.0 ; extra == "test"
+Requires-Dist: pytest-xdist >=1.32.0,<4.0.0 ; extra == "test"
 Requires-Dist: pytest-sugar >=0.9.4,<0.10.0 ; extra == "test"
 Requires-Dist: mypy ==0.910 ; extra == "test"
 Requires-Dist: black >=22.3.0,<23.0.0 ; extra == "test"
 Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
 Requires-Dist: rich >=10.11.0,<13.0.0 ; extra == "test"
 Project-URL: Documentation, https://typer.tiangolo.com/
 Provides-Extra: all
@@ -59,17 +64,16 @@
 <p align="center">
 <a href="https://github.com/tiangolo/typer/actions?query=workflow%3ATest" target="_blank">
     <img src="https://github.com/tiangolo/typer/workflows/Test/badge.svg" alt="Test">
 </a>
 <a href="https://github.com/tiangolo/typer/actions?query=workflow%3APublish" target="_blank">
     <img src="https://github.com/tiangolo/typer/workflows/Publish/badge.svg" alt="Publish">
 </a>
-<a href="https://codecov.io/gh/tiangolo/typer" target="_blank">
-    <img src="https://img.shields.io/codecov/c/github/tiangolo/typer?color=%2334D058" alt="Coverage">
-</a>
+<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/tiangolo/typer" target="_blank">
+    <img src="https://coverage-badge.samuelcolvin.workers.dev/tiangolo/typer.svg" alt="Coverage">
 <a href="https://pypi.org/project/typer" target="_blank">
     <img src="https://img.shields.io/pypi/v/typer?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 </p>
 
 ---
```

#### html2text {}

```diff
@@ -1,43 +1,46 @@
-Metadata-Version: 2.1 Name: typer Version: 0.6.1 Summary: Typer, build great
+Metadata-Version: 2.1 Name: typer Version: 0.7.0 Summary: Typer, build great
 CLIs. Easy to code. Based on Python type hints. Home-page: https://github.com/
 tiangolo/typer Author: SebastiÃ¡n RamÃ­rez Author-email: tiangolo@gmail.com
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries ::
 Application Frameworks Classifier: Topic :: Software Development :: Libraries
 :: Python Modules Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 License :: OSI Approved :: MIT License Requires-Dist: click >= 7.1.1, <9.0.0
 Requires-Dist: colorama >=0.4.3,<0.5.0 ; extra == "all" Requires-Dist:
 shellingham >=1.3.0,<2.0.0 ; extra == "all" Requires-Dist: rich
 >=10.11.0,<13.0.0 ; extra == "all" Requires-Dist: autoflake >=1.3.1,<2.0.0 ;
 extra == "dev" Requires-Dist: flake8 >=3.8.3,<4.0.0 ; extra == "dev" Requires-
 Dist: pre-commit >=2.17.0,<3.0.0 ; extra == "dev" Requires-Dist: mkdocs
 >=1.1.2,<2.0.0 ; extra == "doc" Requires-Dist: mkdocs-material >=8.1.4,<9.0.0 ;
 extra == "doc" Requires-Dist: mdx-include >=1.4.1,<2.0.0 ; extra == "doc"
-Requires-Dist: shellingham >=1.3.0,<2.0.0 ; extra == "test" Requires-Dist:
-pytest >=4.4.0,<5.4.0 ; extra == "test" Requires-Dist: pytest-cov
->=2.10.0,<3.0.0 ; extra == "test" Requires-Dist: coverage >=5.2,<6.0 ; extra ==
-"test" Requires-Dist: pytest-xdist >=1.32.0,<2.0.0 ; extra == "test" Requires-
-Dist: pytest-sugar >=0.9.4,<0.10.0 ; extra == "test" Requires-Dist: mypy
-==0.910 ; extra == "test" Requires-Dist: black >=22.3.0,<23.0.0 ; extra ==
-"test" Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test" Requires-Dist:
-rich >=10.11.0,<13.0.0 ; extra == "test" Project-URL: Documentation, https://
-typer.tiangolo.com/ Provides-Extra: all Provides-Extra: dev Provides-Extra: doc
-Provides-Extra: test
+Requires-Dist: pillow >=9.3.0,<10.0.0 ; extra == "doc" Requires-Dist: cairosvg
+>=2.5.2,<3.0.0 ; extra == "doc" Requires-Dist: shellingham >=1.3.0,<2.0.0 ;
+extra == "test" Requires-Dist: pytest >=4.4.0,<8.0.0 ; extra == "test"
+Requires-Dist: pytest-cov >=2.10.0,<5.0.0 ; extra == "test" Requires-Dist:
+coverage >=6.2,<7.0 ; extra == "test" Requires-Dist: pytest-xdist
+>=1.32.0,<4.0.0 ; extra == "test" Requires-Dist: pytest-sugar >=0.9.4,<0.10.0 ;
+extra == "test" Requires-Dist: mypy ==0.910 ; extra == "test" Requires-Dist:
+black >=22.3.0,<23.0.0 ; extra == "test" Requires-Dist: isort >=5.0.6,<6.0.0 ;
+extra == "test" Requires-Dist: rich >=10.11.0,<13.0.0 ; extra == "test"
+Project-URL: Documentation, https://typer.tiangolo.com/ Provides-Extra: all
+Provides-Extra: dev Provides-Extra: doc Provides-Extra: test
                                     [Typer]
       Typer, build great CLIs. Easy to code. Based on Python type hints.
-                 [Test] [Publish] [Coverage] [Package_version]
+                 [Test] [Publish] [Coverage]_[Package_version]
 --- **Documentation**: https://typer.tiangolo.com **Source Code**: https://
 github.com/tiangolo/typer --- Typer is a library for building CLI applications
 that users will **love using** and developers will **love creating**. Based on
 Python 3.6+ type hints. The key features are: * **Intuitive to write**: Great
 editor support. Completion everywhere. Less time debugging. Designed to be easy
 to use and learn. Less time reading docs. * **Easy to use**: It's easy to use
 for the final users. Automatic help, and automatic completion for all shells. *
```

