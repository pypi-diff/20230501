# Comparing `tmp/arelle-release-2.8.1.tar.gz` & `tmp/arelle-release-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arelle-release-2.8.1.tar", last modified: Wed Apr 26 14:32:29 2023, max compression
+gzip compressed data, was "arelle-release-2.9.0.tar", last modified: Mon May  1 19:54:03 2023, max compression
```

## Comparing `arelle-release-2.8.1.tar` & `arelle-release-2.9.0.tar`

### file list

```diff
@@ -1,747 +1,747 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.473324 arelle-release-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.377324 arelle-release-2.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.377324 arelle-release-2.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/ISSUE_TEMPLATE/change.yml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.377324 arelle-release-2.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/build-and-release-linux.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/build-and-release-mac.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/build-and-release-windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/build-windows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/conformance-suites.yml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/project.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/test-ui.yml
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-26 14:31:54.000000 arelle-release-2.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-26 14:31:54.000000 arelle-release-2.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-26 14:31:54.000000 arelle-release-2.8.1/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-26 14:31:54.000000 arelle-release-2.8.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-26 14:31:54.000000 arelle-release-2.8.1/EFM-only-test.ini
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-26 14:31:54.000000 arelle-release-2.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-26 14:32:29.473324 arelle-release-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-26 14:31:54.000000 arelle-release-2.8.1/QuickBooks.qwc
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-26 14:31:54.000000 arelle-release-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.377324 arelle-release-2.8.1/apidocs/
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-26 14:31:54.000000 arelle-release-2.8.1/apidocs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-04-26 14:31:54.000000 arelle-release-2.8.1/apidocs/arelle.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-04-26 14:31:54.000000 arelle-release-2.8.1/apidocs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-26 14:31:54.000000 arelle-release-2.8.1/apidocs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-04-26 14:31:54.000000 arelle-release-2.8.1/apidocs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 14:31:54.000000 arelle-release-2.8.1/apidocs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.393324 arelle-release-2.8.1/arelle/
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/Aspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    40266 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/Cntlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    76890 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/CntlrCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/CntlrComServer.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/CntlrProfiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31445 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/CntlrQuickBooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    48719 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/CntlrWebMain.py
--rw-r--r--   0 runner    (1001) docker     (123)    88802 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/CntlrWinMain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/CntlrWinTooltip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogAbout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogArcroleGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogFind.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogFormulaParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogLanguage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogNewFactItem.py
--rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogOpenArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogOpenTaxonomyPackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogPackageManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogPluginManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogRssWatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogURL.py
--rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DialogUserPassword.py
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/DisclosureSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    43656 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/FileSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/FunctionCustom.py
--rw-r--r--   0 runner    (1001) docker     (123)    36519 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/FunctionFn.py
--rw-r--r--   0 runner    (1001) docker     (123)    80279 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/FunctionIxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/FunctionUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    71334 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/FunctionXfi.py
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/FunctionXs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/HashUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/HtmlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/InstanceAspectsEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/LeiUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/LocalViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28242 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/Locale.py
--rw-r--r--   0 runner    (1001) docker     (123)   120056 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelDocument.py
--rw-r--r--   0 runner    (1001) docker     (123)    88883 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelDtsObject.py
--rw-r--r--   0 runner    (1001) docker     (123)   122124 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelFormulaObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    72084 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelInstanceObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelObjectFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    70336 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelRenderingObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelRssItem.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelRssObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelTestcaseObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    38714 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelValue.py
--rw-r--r--   0 runner    (1001) docker     (123)    26062 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelVersObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    73327 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)    69922 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ModelXbrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    31672 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/PackageManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    29039 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/PluginManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/PrototypeDtsObject.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/PrototypeInstanceObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/PythonUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/RenderingEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43733 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/RenderingResolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/SystemInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    29404 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/TableStructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    32276 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/TkTableWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    39250 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/UITkTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/UiUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/Updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    32121 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/UrlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49309 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/Validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    51377 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ValidateFilingText.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ValidateInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ValidateUtr.py
--rw-r--r--   0 runner    (1001) docker     (123)    43196 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ValidateVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)    75131 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ValidateXbrl.py
--rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ValidateXbrlCalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)   100180 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ValidateXbrlDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    38118 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ValidateXbrlDimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileConcepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileFactList.py
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileFactTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileRenderedGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileRoleTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileRssFeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewFileTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewUtilFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinConcepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinDiffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinFactGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinFactList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinFactTable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinFormulae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinList.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinPane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinRelationshipSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    78864 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinRenderedGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinRoleTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinRssFeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinTests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinTkTable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinTree.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinTupleGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinVersReport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/ViewWinXml.py
--rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/WatchRss.py
--rw-r--r--   0 runner    (1001) docker     (123)    36652 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/WebCache.py
--rw-r--r--   0 runner    (1001) docker     (123)    62211 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/XbrlConst.py
--rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/XbrlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/XhtmlValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)    56964 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/XmlUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)    44568 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/XmlValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/XmlValidateParticles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/XmlValidateSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 14:32:29.000000 arelle-release-2.8.1/arelle/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.393324 arelle-release-2.8.1/arelle/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/arelle_test.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/creationSoftwareNames.json
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/disclosuresystems.xml
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/disclosuresystems.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/edbody.dtd
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/empty-instance.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/erxl.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/mappings.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/mappings.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/xbrlschemafiles.xml
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/xhtml-lat1.ent
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/xhtml-special.ent
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/xhtml-symbol.ent
--rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/xhtml1-strict-ix.dtd
--rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/config/xhtml1_1-strict-ix.dtd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.397324 arelle-release-2.8.1/arelle/doc/
--rw-r--r--   0 runner    (1001) docker     (123)   458032 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/doc/messagesCatalog.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/doc/messagesCatalog.xsd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.397324 arelle-release-2.8.1/arelle/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/.pydevproject
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/CustomLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/LoadEFMvalidate.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/LoadSavePreLbCsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/LoadValidate.cs
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/LoadValidate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/LoadValidateCmdLine.java
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/LoadValidatePostedZip.java
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/LoadValidateWebService.java
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/SaveTableToExelle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/TR3toTR4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.401324 arelle-release-2.8.1/arelle/examples/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/bigInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/cmdWebServerExtension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/crashTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/formulaSuiteConverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/functionsCustom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/hello_dolly.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/hello_i18n.pot
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/hello_i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/importTestChild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/importTestChild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/importTestGrandchild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/importTestGrandchild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/importTestImported1.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/importTestImported11.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/importTestParent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.365324 arelle-release-2.8.1/arelle/examples/plugin/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.365324 arelle-release-2.8.1/arelle/examples/plugin/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.401324 arelle-release-2.8.1/arelle/examples/plugin/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.401324 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestChild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestChild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestImported1.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestImported11.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.401324 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.401324 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/sakaCalendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/saveInstanceInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/streamingExtensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/updateTableLB.py
--rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/validateSchemaLxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/plugin/validateTableInfoset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/us-gaap-dei-docType-extraction-frm.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/examples/us-gaap-dei-ratio-cash-frm.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.401324 arelle-release-2.8.1/arelle/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/formula/FactAspectsCache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/formula/FormulaConsisAsser.py
--rw-r--r--   0 runner    (1001) docker     (123)    83178 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/formula/FormulaEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    98324 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/formula/ValidateFormula.py
--rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/formula/XPathContext.py
--rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/formula/XPathParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/formula/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.409324 arelle-release-2.8.1/arelle/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle-full-word.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle-mac-icon-4.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle-word-only.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle.gif
--rw-r--r--   0 runner    (1001) docker     (123)   212911 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle.icns
--rw-r--r--   0 runner    (1001) docker     (123)   392859 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle.icns.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle.ico
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle.xbm
--rw-r--r--   0 runner    (1001) docker     (123)   269858 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle128.psd
--rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle16.psd
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle16x16and32x32.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/arelle32.gif
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/columnSortDown.gif
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/columnSortUp.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/dmg_background.png
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/octocat.png
--rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/python-clear.png
--rw-r--r--   0 runner    (1001) docker     (123)   696358 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/python-icon-pack-crystalxp.net-842.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarClose.gif
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarCompare.gif
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarDelete.gif
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarFindMenu.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarLogClear - 1-piece-top.gif
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarLogClear-orig.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarLogClear.gif
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarNewFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarOpenDatabase.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarOpenFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarOpenWeb.gif
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarProperties.gif
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarQuit.gif
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarReopen.gif
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarSaveFile.gif
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/toolbarValidate.gif
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/xbrl.gif
--rw-r--r--   0 runner    (1001) docker     (123)   201686 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/xbrl.psd
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/xbrl128-2.gif
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/xbrl128.gif
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/xbrl16.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/images/xbrl32.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.409324 arelle-release-2.8.1/arelle/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.365324 arelle-release-2.8.1/arelle/locale/ar_EG/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.409324 arelle-release-2.8.1/arelle/locale/ar_EG/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   341883 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po
--rw-r--r--   0 runner    (1001) docker     (123)   185904 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.365324 arelle-release-2.8.1/arelle/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.409324 arelle-release-2.8.1/arelle/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   149331 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/es/LC_MESSAGES/arelle.mo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.365324 arelle-release-2.8.1/arelle/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.409324 arelle-release-2.8.1/arelle/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   118897 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/fr/LC_MESSAGES/arelle.mo
--rw-r--r--   0 runner    (1001) docker     (123)   168077 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/fr/LC_MESSAGES/fr.po
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)   249762 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.365324 arelle-release-2.8.1/arelle/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.409324 arelle-release-2.8.1/arelle/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)   375378 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/ru/LC_MESSAGES/arelle.mo
--rw-r--r--   0 runner    (1001) docker     (123)   449579 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/locale/ru/LC_MESSAGES/ru.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.413324 arelle-release-2.8.1/arelle/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/EdgarRendererAllReports.py
--rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/SECCorrespondenceLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/TDnetLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/UKCompaniesHouseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)   101637 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/formulaLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)    31396 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/formulaSaver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/formulaXPathChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/functionsMath.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/functionsXmlCreation.py
--rw-r--r--   0 runner    (1001) docker     (123)    42075 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/inlineXbrlDocumentSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/instanceInfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.365324 arelle-release-2.8.1/arelle/plugin/internet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.413324 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/U32.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/des.py
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/des_c.py
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/des_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html
--rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/ntlm.py
--rw-r--r--   0 runner    (1001) docker     (123)   124382 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/loadFromExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    76473 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/loadFromOIM-2018.py
--rw-r--r--   0 runner    (1001) docker     (123)   195836 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/loadFromOIM.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.417324 arelle-release-2.8.1/arelle/plugin/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/logging/dpmSignature.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/logging/dqcParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/logging/saveMessages.py
--rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/objectmaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/profileCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/profileFormula.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/saveCHComponentFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/saveDTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/saveHtmlEBAtables.py
--rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/saveLoadableExcel.py
--rw-r--r--   0 runner    (1001) docker     (123)    32261 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/saveLoadableOIM.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/saveSKOS.py
--rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/saveSampleInstance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.417324 arelle-release-2.8.1/arelle/plugin/security/
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/security/cryptAES_CBC.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/security/cryptAES_EAX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.417324 arelle-release-2.8.1/arelle/plugin/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/sphinx/FormulaGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/sphinx/SphinxContext.py
--rw-r--r--   0 runner    (1001) docker     (123)    35742 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/sphinx/SphinxEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    49810 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/sphinx/SphinxMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/sphinx/SphinxParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/sphinx/SphinxValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47646 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/streamingExtensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.417324 arelle-release-2.8.1/arelle/plugin/transforms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.417324 arelle-release-2.8.1/arelle/plugin/transforms/SEC/
--rw-r--r--   0 runner    (1001) docker     (123)    41892 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.421324 arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/extractTestcase.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)  4737705 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/saxon9.jar
--rw-r--r--   0 runner    (1001) docker     (123)   225611 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/testcase.xml
--rw-r--r--   0 runner    (1001) docker     (123)    59680 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/tests.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/text2num.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.425324 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.425324 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/schema/
--rw-r--r--   0 runner    (1001) docker     (123)    55540 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/transforms/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/unpackSecEisFile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.425324 arelle-release-2.8.1/arelle/plugin/validate/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.425324 arelle-release-2.8.1/arelle/plugin/validate/CIPC/
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/CIPC/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/CIPC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/CIPC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.425324 arelle-release-2.8.1/arelle/plugin/validate/EBA/
--rw-r--r--   0 runner    (1001) docker     (123)    45950 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EBA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EBA/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.425324 arelle-release-2.8.1/arelle/plugin/validate/EFM/
--rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/Consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/Document.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   253045 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/Filing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/PreCalAlignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.437324 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/axiswarnings.json
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/cef-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/country-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/currency-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/dei-deprecated-concepts.json
--rwxr-xr-x   0 runner    (1001) docker     (123)   113832 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/dei-validations.json
--rw-r--r--   0 runner    (1001) docker     (123)    76859 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/dqc-us-rules.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/ecd-deprecated-concepts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/
--rw-r--r--   0 runner    (1001) docker     (123)    31435 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    76545 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    76785 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    73012 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    80115 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   150333 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   138364 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml
--rw-r--r--   0 runner    (1001) docker     (123)   135467 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml
--rw-r--r--   0 runner    (1001) docker     (123)   180977 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   125792 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)   119973 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)   134456 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   109498 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    99358 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)    28394 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml
--rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml
--rw-r--r--   0 runner    (1001) docker     (123)    29744 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml
--rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml
--rw-r--r--   0 runner    (1001) docker     (123)    31676 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml
--rw-r--r--   0 runner    (1001) docker     (123)   109944 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    35860 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml
--rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    58455 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml
--rw-r--r--   0 runner    (1001) docker     (123)    62455 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    49163 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    48412 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml
--rw-r--r--   0 runner    (1001) docker     (123)    57294 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml
--rw-r--r--   0 runner    (1001) docker     (123)    69072 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)    69638 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml
--rw-r--r--   0 runner    (1001) docker     (123)   368244 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)    93735 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/other-standard-taxonomies.json
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/sic-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/signwarnings.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/srt-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/stpr-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json
--rw-r--r--   0 runner    (1001) docker     (123)   205448 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json
--rw-r--r--   0 runner    (1001) docker     (123)  1583747 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json
--rw-r--r--   0 runner    (1001) docker     (123)  1624986 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json
--rw-r--r--   0 runner    (1001) docker     (123)  1593440 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json
--rw-r--r--   0 runner    (1001) docker     (123)  1613560 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/vip-deprecated-concepts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/EFM/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM/tools/CheckTxmyRefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.429324 arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.429324 arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/ESEF/
--rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    76372 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/ESEF/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF/resources/authority-validations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/
--rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/Const.py
--rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    85329 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/FERC/
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/FERC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/FERC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/FERC/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/FERC/resources/ferc-utr.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/GFM/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/GFM/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/GFM/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/HMRC/
--rw-r--r--   0 runner    (1001) docker     (123)    29346 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/HMRC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/HMRC/config.xml
--rw-r--r--   0 runner    (1001) docker     (123)    25247 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/HMRC/consistencyChecksByName.json
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.445324 arelle-release-2.8.1/arelle/plugin/validate/ROS/
--rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ROS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/ROS/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.449324 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/CustomLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/DTS.py
--rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/Dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    59358 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/Document.py
--rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/Filing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/config.xml
--rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml
--rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/USBestPractices.py
--rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/USCorpAction.py
--rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/USSecTagging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.449324 arelle-release-2.8.1/arelle/plugin/validate/XDC/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/XDC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/XDC/config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.449324 arelle-release-2.8.1/arelle/plugin/validate/XFsyntax/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/XFsyntax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66728 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/XFsyntax/xf.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validate/calc2.py
--rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/validateSBRnl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.449324 arelle-release-2.8.1/arelle/plugin/xbrlDB/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/DialogRssWatchExtender.py
--rw-r--r--   0 runner    (1001) docker     (123)    56450 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/SqlDb.py
--rw-r--r--   0 runner    (1001) docker     (123)    78257 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    78348 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    36203 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    64539 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    55073 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    67782 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/entityInformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.449324 arelle-release-2.8.1/arelle/plugin/xbrlDB/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/ext/china.py
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/ext/edgar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/ext/xdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/primaryDocumentFacts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.449324 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.453324 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/ext/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   714004 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.453324 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open2/
--rw-r--r--   0 runner    (1001) docker     (123)   728541 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.453324 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/public/
--rw-r--r--   0 runner    (1001) docker     (123)   963416 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.457324 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql
--rw-r--r--   0 runner    (1001) docker     (123)    21988 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   728214 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)   729124 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)  1056221 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)   727913 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)   726301 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xbrlDB/tableFacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/plugin/xuleSaver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.457324 arelle-release-2.8.1/arelle/scripts-macOS/
--rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-macOS/startWebServer.command
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.457324 arelle-release-2.8.1/arelle/scripts-unix/
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-unix/startWebServer.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/arelle/scripts-windows/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-windows/exportCsvFromXbrlInstance.bat
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-windows/runEFMTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-windows/runFormulaTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-windows/runFunctionTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-windows/runXBRL21Tests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-windows/runXDTTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-windows/startWebServer.bat
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/scripts-windows/validateAndRunFormulas.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/arelle/webserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   116069 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/webserver/bottle-no2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)   171083 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle/webserver/bottle.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle.pyw
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelleCmdLine.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelleGUI.pyw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/arelle_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-26 14:32:29.000000 arelle-release-2.8.1/arelle_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26653 2023-04-26 14:32:29.000000 arelle-release-2.8.1/arelle_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 14:32:29.000000 arelle-release-2.8.1/arelle_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 14:32:29.000000 arelle-release-2.8.1/arelle_release.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-26 14:32:29.000000 arelle-release-2.8.1/arelle_release.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 14:32:29.000000 arelle-release-2.8.1/arelle_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-04-26 14:31:54.000000 arelle-release-2.8.1/arelle_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/attic/
--rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-04-26 14:31:54.000000 arelle-release-2.8.1/attic/CntlrGenVersReports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-26 14:31:54.000000 arelle-release-2.8.1/buildVersion.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-26 14:31:54.000000 arelle-release-2.8.1/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 14:31:54.000000 arelle-release-2.8.1/debugCmdLineEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-26 14:31:54.000000 arelle-release-2.8.1/distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-04-26 14:31:54.000000 arelle-release-2.8.1/docker/ubuntu.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 14:31:54.000000 arelle-release-2.8.1/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-26 14:31:54.000000 arelle-release-2.8.1/encodeUtf8PySource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-04-26 14:31:54.000000 arelle-release-2.8.1/generateMessagesCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-26 14:31:54.000000 arelle-release-2.8.1/installWin64.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-26 14:31:54.000000 arelle-release-2.8.1/installWin86.nsi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/libs/linux/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/libs/linux/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/linux/Tktable2.11/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/libs/linux/Tktable2.11/html/
--rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/linux/Tktable2.11/html/tkTable.html
--rwxr-xr-x   0 runner    (1001) docker     (123)   161976 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/linux/Tktable2.11/libTktable2.11.so
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/linux/Tktable2.11/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/linux/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/linux/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/linux/Tktable2.11/tktable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/libs/macos/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/libs/macos/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/macos/Tktable2.11/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.461324 arelle-release-2.8.1/libs/macos/Tktable2.11/html/
--rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/macos/Tktable2.11/html/tkTable.html
--rw-r--r--   0 runner    (1001) docker     (123)   130952 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/macos/Tktable2.11/libTktable2.11.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/macos/Tktable2.11/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/macos/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/macos/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/macos/Tktable2.11/tktable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/libs/win64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.465324 arelle-release-2.8.1/libs/win64/Tktable2.11/
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/win64/Tktable2.11/Tktable.dll
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/win64/Tktable2.11/pkgIndex.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-04-26 14:31:54.000000 arelle-release-2.8.1/libs/win64/Tktable2.11/tkTable.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-26 14:31:54.000000 arelle-release-2.8.1/messages.pot
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-26 14:31:54.000000 arelle-release-2.8.1/msgfmt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.465324 arelle-release-2.8.1/plugins/xbrl-us/
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-26 14:31:54.000000 arelle-release-2.8.1/plugins/xbrl-us/us-gaap-consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-04-26 14:31:54.000000 arelle-release-2.8.1/pygettext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-26 14:31:54.000000 arelle-release-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 14:31:54.000000 arelle-release-2.8.1/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 14:31:54.000000 arelle-release-2.8.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-26 14:31:54.000000 arelle-release-2.8.1/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-04-26 14:31:54.000000 arelle-release-2.8.1/runMacGUI.sh
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-26 14:31:54.000000 arelle-release-2.8.1/runtime.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.465324 arelle-release-2.8.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/buildLinuxDist.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/buildMacDist.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/buildWinDist.bat
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/charlieTest.bat
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/exportCsvFormulae.bat
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/exportCsvFromXbrlInstance.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/generateTestcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/reportAllTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runAllTests.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runESMAtests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runGUI.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      266 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runGUI.sh
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runGenerateVersioningTestcases.bat
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runGeneratedTestcase.bat
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runLocaleGettext.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runPackageTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runProfilerXDTTest.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runPyTest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runTR2Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runTR3Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runTR4Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runTR5Tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runTRSECTests.sh
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runUS-GFMTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/runVersioningConsumptionTests.bat
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/startWebServer-27.bat
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-26 14:31:54.000000 arelle-release-2.8.1/scripts/startWebServer.bat
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-26 14:32:29.473324 arelle-release-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-26 14:31:54.000000 arelle-release-2.8.1/testParser.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-26 14:31:54.000000 arelle-release-2.8.1/testParser2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.465324 arelle-release-2.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/tests/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/tests/integration_tests/ui_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.465324 arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.465324 arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj
--rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Usings.cs
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.465324 arelle-release-2.8.1/tests/integration_tests/ui_tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   223544 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/ui_tests/resources/workiva.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.469324 arelle-release-2.8.1/tests/integration_tests/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.469324 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_assertion_severity_2_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_link_role_registry_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)    29081 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_taxonomy_packages_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_4.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/download_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/run_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/test_conformance_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/integration_tests/validation/validation_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.369324 arelle-release-2.8.1/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.473324 arelle-release-2.8.1/tests/unit_tests/arelle/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.473324 arelle-release-2.8.1/tests/unit_tests/arelle/formula/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.473324 arelle-release-2.8.1/tests/unit_tests/arelle/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/plugin/test_loadfromoim.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_cntlr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_modelmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_packagemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_pluginmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_qname.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_urlutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tests/unit_tests/arelle/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 14:31:54.000000 arelle-release-2.8.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.373324 arelle-release-2.8.1/vms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 14:32:29.473324 arelle-release-2.8.1/vms/mac/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-26 14:31:54.000000 arelle-release-2.8.1/vms/mac/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-04-26 14:31:54.000000 arelle-release-2.8.1/vms/mac/create-macos-bootable-for-virtualbox.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.860487 arelle-release-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.756484 arelle-release-2.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.756484 arelle-release-2.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/ISSUE_TEMPLATE/change.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.756484 arelle-release-2.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/build-and-release-linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/build-and-release-mac.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/build-and-release-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/build-windows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/conformance-suites.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/test-ui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-01 19:53:47.000000 arelle-release-2.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-05-01 19:53:47.000000 arelle-release-2.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-01 19:53:47.000000 arelle-release-2.9.0/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-01 19:53:47.000000 arelle-release-2.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-01 19:53:47.000000 arelle-release-2.9.0/EFM-only-test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-01 19:53:47.000000 arelle-release-2.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-01 19:54:03.860487 arelle-release-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-01 19:53:47.000000 arelle-release-2.9.0/QuickBooks.qwc
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-01 19:53:47.000000 arelle-release-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.756484 arelle-release-2.9.0/apidocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-01 19:53:47.000000 arelle-release-2.9.0/apidocs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-01 19:53:47.000000 arelle-release-2.9.0/apidocs/arelle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-05-01 19:53:47.000000 arelle-release-2.9.0/apidocs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-01 19:53:47.000000 arelle-release-2.9.0/apidocs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-05-01 19:53:47.000000 arelle-release-2.9.0/apidocs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-01 19:53:47.000000 arelle-release-2.9.0/apidocs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.776485 arelle-release-2.9.0/arelle/
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/Aspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40266 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/Cntlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76890 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/CntlrCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/CntlrComServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/CntlrProfiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31445 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/CntlrQuickBooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48719 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/CntlrWebMain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88802 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/CntlrWinMain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/CntlrWinTooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogAbout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogArcroleGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19419 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogFind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogFormulaParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogLanguage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogNewFactItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24340 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogOpenArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogOpenTaxonomyPackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogPackageManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32913 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogPluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogRssWatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogURL.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13768 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DialogUserPassword.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/DisclosureSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43656 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/FileSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/FunctionCustom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36519 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/FunctionFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80279 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/FunctionIxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/FunctionUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71334 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/FunctionXfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/FunctionXs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/HashUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/HtmlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/InstanceAspectsEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/LeiUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/LocalViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28242 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/Locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120056 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelDocument.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88883 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelDtsObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122124 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelFormulaObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72084 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelInstanceObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18470 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelObjectFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70336 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelRenderingObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelRssItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelRssObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21204 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelTestcaseObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38714 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26062 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelVersObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73327 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69922 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ModelXbrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31672 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/PackageManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29039 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/PluginManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/PrototypeDtsObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/PrototypeInstanceObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/PythonUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16693 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/RenderingEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43733 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/RenderingResolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/SystemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29404 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/TableStructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32276 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/TkTableWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39250 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/UITkTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34218 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/UiUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/Updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32121 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/UrlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49309 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/Validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51377 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ValidateFilingText.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ValidateInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ValidateUtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43196 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ValidateVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75131 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ValidateXbrl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30954 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ValidateXbrlCalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100180 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ValidateXbrlDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38118 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ValidateXbrlDimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileConcepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileFactList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileFactTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileRenderedGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileRoleTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileRssFeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewFileTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewUtilFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinConcepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinDiffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinFactGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinFactList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinFactTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinFormulae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinPane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinRelationshipSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78864 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinRenderedGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinRoleTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinRssFeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinTkTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinTupleGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinVersReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/ViewWinXml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13892 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/WatchRss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36652 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/WebCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62211 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/XbrlConst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/XbrlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/XhtmlValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56964 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/XmlUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44568 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/XmlValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/XmlValidateParticles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/XmlValidateSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-01 19:54:03.000000 arelle-release-2.9.0/arelle/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.776485 arelle-release-2.9.0/arelle/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/arelle_test.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/creationSoftwareNames.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/disclosuresystems.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/disclosuresystems.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    15557 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/edbody.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/empty-instance.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/erxl.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/mappings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/mappings.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/xbrlschemafiles.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/xhtml-lat1.ent
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/xhtml-special.ent
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/xhtml-symbol.ent
+-rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/xhtml1-strict-ix.dtd
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/config/xhtml1_1-strict-ix.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.776485 arelle-release-2.9.0/arelle/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)   458032 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/doc/messagesCatalog.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/doc/messagesCatalog.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.780485 arelle-release-2.9.0/arelle/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/.pydevproject
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/CustomLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/LoadEFMvalidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/LoadSavePreLbCsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/LoadValidate.cs
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/LoadValidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/LoadValidateCmdLine.java
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/LoadValidatePostedZip.java
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/LoadValidateWebService.java
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/SaveTableToExelle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/TR3toTR4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.780485 arelle-release-2.9.0/arelle/examples/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/bigInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/cmdWebServerExtension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/crashTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/formulaSuiteConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/functionsCustom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/hello_dolly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/hello_i18n.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/hello_i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/importTestChild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/importTestChild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/importTestGrandchild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/importTestGrandchild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/importTestImported1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/importTestImported11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/importTestParent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.744484 arelle-release-2.9.0/arelle/examples/plugin/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.744484 arelle-release-2.9.0/arelle/examples/plugin/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.780485 arelle-release-2.9.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.784485 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestChild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestChild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestImported1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestImported11.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.784485 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.784485 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/sakaCalendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/saveInstanceInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/streamingExtensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/updateTableLB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/validateSchemaLxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/plugin/validateTableInfoset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/us-gaap-dei-docType-extraction-frm.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/examples/us-gaap-dei-ratio-cash-frm.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.784485 arelle-release-2.9.0/arelle/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/formula/FactAspectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7567 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/formula/FormulaConsisAsser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83178 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/formula/FormulaEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98324 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/formula/ValidateFormula.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48615 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/formula/XPathContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49913 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/formula/XPathParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/formula/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.792485 arelle-release-2.9.0/arelle/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle-full-word.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle-mac-icon-4.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle-word-only.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   212911 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle.icns
+-rw-r--r--   0 runner    (1001) docker     (123)   392859 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle.icns.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle.xbm
+-rw-r--r--   0 runner    (1001) docker     (123)   269858 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle128.psd
+-rw-r--r--   0 runner    (1001) docker     (123)    24028 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle16.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle16x16and32x32.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/arelle32.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/columnSortDown.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/columnSortUp.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/dmg_background.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/octocat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23863 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/python-clear.png
+-rw-r--r--   0 runner    (1001) docker     (123)   696358 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/python-icon-pack-crystalxp.net-842.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarClose.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarCompare.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarDelete.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarFindMenu.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarLogClear - 1-piece-top.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarLogClear-orig.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarLogClear.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarNewFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarOpenDatabase.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarOpenFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarOpenWeb.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarProperties.gif
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarQuit.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarReopen.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarSaveFile.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/toolbarValidate.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/xbrl.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   201686 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/xbrl.psd
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/xbrl128-2.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/xbrl128.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/xbrl16.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/images/xbrl32.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.792485 arelle-release-2.9.0/arelle/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/arelle/locale/ar_EG/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.792485 arelle-release-2.9.0/arelle/locale/ar_EG/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   341883 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po
+-rw-r--r--   0 runner    (1001) docker     (123)   185904 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/arelle/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.792485 arelle-release-2.9.0/arelle/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   149331 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/es/LC_MESSAGES/arelle.mo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/arelle/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.792485 arelle-release-2.9.0/arelle/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   118897 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/fr/LC_MESSAGES/arelle.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   168077 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/fr/LC_MESSAGES/fr.po
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   249762 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/arelle/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.792485 arelle-release-2.9.0/arelle/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)   375378 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/ru/LC_MESSAGES/arelle.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   449579 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/locale/ru/LC_MESSAGES/ru.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.796485 arelle-release-2.9.0/arelle/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/EdgarRendererAllReports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/SECCorrespondenceLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/TDnetLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/UKCompaniesHouseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101637 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/formulaLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31396 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/formulaSaver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/formulaXPathChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/functionsMath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/functionsXmlCreation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42075 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/inlineXbrlDocumentSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/instanceInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/arelle/plugin/internet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.800485 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/U32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/des_c.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/des_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html
+-rw-r--r--   0 runner    (1001) docker     (123)    22226 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/ntlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124382 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/loadFromExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76473 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/loadFromOIM-2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199186 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/loadFromOIM.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.800485 arelle-release-2.9.0/arelle/plugin/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/logging/dpmSignature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/logging/dqcParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/logging/saveMessages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13883 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/objectmaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/profileCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/profileFormula.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/saveCHComponentFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/saveDTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/saveHtmlEBAtables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20476 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/saveLoadableExcel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32261 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/saveLoadableOIM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/saveSKOS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23823 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/saveSampleInstance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.800485 arelle-release-2.9.0/arelle/plugin/security/
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/security/cryptAES_CBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/security/cryptAES_EAX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.800485 arelle-release-2.9.0/arelle/plugin/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/sphinx/FormulaGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19516 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/sphinx/SphinxContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35742 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/sphinx/SphinxEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49810 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/sphinx/SphinxMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48614 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/sphinx/SphinxParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/sphinx/SphinxValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr
+-rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47646 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/streamingExtensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.800485 arelle-release-2.9.0/arelle/plugin/transforms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.800485 arelle-release-2.9.0/arelle/plugin/transforms/SEC/
+-rw-r--r--   0 runner    (1001) docker     (123)    41892 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.808486 arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/extractTestcase.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  4737705 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/saxon9.jar
+-rw-r--r--   0 runner    (1001) docker     (123)   225611 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/testcase.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    59680 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/tests.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/text2num.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.808486 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.808486 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    55540 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/transforms/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/unpackSecEisFile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.808486 arelle-release-2.9.0/arelle/plugin/validate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.812486 arelle-release-2.9.0/arelle/plugin/validate/CIPC/
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/CIPC/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/CIPC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/CIPC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.812486 arelle-release-2.9.0/arelle/plugin/validate/EBA/
+-rw-r--r--   0 runner    (1001) docker     (123)    45950 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EBA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EBA/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.812486 arelle-release-2.9.0/arelle/plugin/validate/EFM/
+-rw-r--r--   0 runner    (1001) docker     (123)    16365 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/Consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17393 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/Document.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   253045 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/Filing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/PreCalAlignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37995 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.824486 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/axiswarnings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/cef-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/country-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/currency-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/dei-deprecated-concepts.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113832 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/dei-validations.json
+-rw-r--r--   0 runner    (1001) docker     (123)    76859 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/dqc-us-rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/ecd-deprecated-concepts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.828486 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/
+-rw-r--r--   0 runner    (1001) docker     (123)    31435 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    76545 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    76785 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    73012 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    80115 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   150333 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   138364 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   135467 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   180977 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   125792 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   119973 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   134456 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   109498 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    99358 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    28394 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    29132 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    29744 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    31676 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   109944 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    39675 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    35860 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    58455 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    62455 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    49163 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    48412 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    57294 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    69072 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    69638 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   368244 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    93735 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/other-standard-taxonomies.json
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/sic-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/signwarnings.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/srt-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/stpr-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205448 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1583747 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1624986 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1593440 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1613560 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/vip-deprecated-concepts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.828486 arelle-release-2.9.0/arelle/plugin/validate/EFM/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM/tools/CheckTxmyRefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.812486 arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.812486 arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/ESEF/
+-rw-r--r--   0 runner    (1001) docker     (123)    21793 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26323 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76372 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/ESEF/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF/resources/authority-validations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/
+-rw-r--r--   0 runner    (1001) docker     (123)    22270 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/Const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85329 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    11317 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/FERC/
+-rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/FERC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/FERC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/FERC/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/FERC/resources/ferc-utr.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/GFM/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/GFM/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/GFM/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/HMRC/
+-rw-r--r--   0 runner    (1001) docker     (123)    29346 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/HMRC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/HMRC/config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    25247 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/HMRC/consistencyChecksByName.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.832486 arelle-release-2.9.0/arelle/plugin/validate/ROS/
+-rw-r--r--   0 runner    (1001) docker     (123)    19281 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ROS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/ROS/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.836486 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/CustomLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/DTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/Dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59358 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/Document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29571 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/Filing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/config.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/USBestPractices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31356 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/USCorpAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18558 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/USSecTagging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.836486 arelle-release-2.9.0/arelle/plugin/validate/XDC/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/XDC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/XDC/config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.836486 arelle-release-2.9.0/arelle/plugin/validate/XFsyntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/XFsyntax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66728 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/XFsyntax/xf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31565 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validate/calc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35332 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/validateSBRnl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.836486 arelle-release-2.9.0/arelle/plugin/xbrlDB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/DialogRssWatchExtender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56450 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/SqlDb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78257 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78348 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36203 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64539 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48567 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55073 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67782 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/entityInformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.836486 arelle-release-2.9.0/arelle/plugin/xbrlDB/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/ext/china.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/ext/edgar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/ext/xdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8208 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/primaryDocumentFacts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.836486 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.840486 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   714004 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)    15891 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.840486 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open2/
+-rw-r--r--   0 runner    (1001) docker     (123)   728541 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.840486 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/public/
+-rw-r--r--   0 runner    (1001) docker     (123)   963416 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.844487 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    21988 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   728214 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)   729124 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)  1056221 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)   727913 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)   726301 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xbrlDB/tableFacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/plugin/xuleSaver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.844487 arelle-release-2.9.0/arelle/scripts-macOS/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       91 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-macOS/startWebServer.command
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.844487 arelle-release-2.9.0/arelle/scripts-unix/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-unix/startWebServer.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.848487 arelle-release-2.9.0/arelle/scripts-windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-windows/exportCsvFromXbrlInstance.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-windows/runEFMTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-windows/runFormulaTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-windows/runFunctionTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-windows/runXBRL21Tests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-windows/runXDTTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-windows/startWebServer.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/scripts-windows/validateAndRunFormulas.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.848487 arelle-release-2.9.0/arelle/webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116069 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/webserver/bottle-no2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171083 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle/webserver/bottle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle.pyw
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelleCmdLine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelleGUI.pyw
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.848487 arelle-release-2.9.0/arelle_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-01 19:54:03.000000 arelle-release-2.9.0/arelle_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26653 2023-05-01 19:54:03.000000 arelle-release-2.9.0/arelle_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 19:54:03.000000 arelle-release-2.9.0/arelle_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 19:54:03.000000 arelle-release-2.9.0/arelle_release.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-01 19:54:03.000000 arelle-release-2.9.0/arelle_release.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 19:54:03.000000 arelle-release-2.9.0/arelle_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-05-01 19:53:47.000000 arelle-release-2.9.0/arelle_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.848487 arelle-release-2.9.0/attic/
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-05-01 19:53:47.000000 arelle-release-2.9.0/attic/CntlrGenVersReports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-01 19:53:47.000000 arelle-release-2.9.0/buildVersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-01 19:53:47.000000 arelle-release-2.9.0/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-01 19:53:47.000000 arelle-release-2.9.0/debugCmdLineEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-01 19:53:47.000000 arelle-release-2.9.0/distro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.848487 arelle-release-2.9.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-01 19:53:47.000000 arelle-release-2.9.0/docker/ubuntu.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-01 19:53:47.000000 arelle-release-2.9.0/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-01 19:53:47.000000 arelle-release-2.9.0/encodeUtf8PySource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-05-01 19:53:47.000000 arelle-release-2.9.0/generateMessagesCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-01 19:53:47.000000 arelle-release-2.9.0/installWin64.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-05-01 19:53:47.000000 arelle-release-2.9.0/installWin86.nsi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/libs/linux/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.848487 arelle-release-2.9.0/libs/linux/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/linux/Tktable2.11/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.848487 arelle-release-2.9.0/libs/linux/Tktable2.11/html/
+-rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/linux/Tktable2.11/html/tkTable.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)   161976 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/linux/Tktable2.11/libTktable2.11.so
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/linux/Tktable2.11/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/linux/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/linux/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/linux/Tktable2.11/tktable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.748484 arelle-release-2.9.0/libs/macos/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.852487 arelle-release-2.9.0/libs/macos/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/macos/Tktable2.11/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.852487 arelle-release-2.9.0/libs/macos/Tktable2.11/html/
+-rw-r--r--   0 runner    (1001) docker     (123)    66891 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/macos/Tktable2.11/html/tkTable.html
+-rw-r--r--   0 runner    (1001) docker     (123)   130952 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/macos/Tktable2.11/libTktable2.11.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/macos/Tktable2.11/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/macos/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/macos/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24896 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/macos/Tktable2.11/tktable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.752484 arelle-release-2.9.0/libs/win64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.852487 arelle-release-2.9.0/libs/win64/Tktable2.11/
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/win64/Tktable2.11/Tktable.dll
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/win64/Tktable2.11/pkgIndex.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-05-01 19:53:47.000000 arelle-release-2.9.0/libs/win64/Tktable2.11/tkTable.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-01 19:53:47.000000 arelle-release-2.9.0/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-01 19:53:47.000000 arelle-release-2.9.0/msgfmt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.752484 arelle-release-2.9.0/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.852487 arelle-release-2.9.0/plugins/xbrl-us/
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-01 19:53:47.000000 arelle-release-2.9.0/plugins/xbrl-us/us-gaap-consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22284 2023-05-01 19:53:47.000000 arelle-release-2.9.0/pygettext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-01 19:53:47.000000 arelle-release-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-01 19:53:47.000000 arelle-release-2.9.0/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-01 19:53:47.000000 arelle-release-2.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-01 19:53:47.000000 arelle-release-2.9.0/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      276 2023-05-01 19:53:47.000000 arelle-release-2.9.0/runMacGUI.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-01 19:53:47.000000 arelle-release-2.9.0/runtime.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.856487 arelle-release-2.9.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1517 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/buildLinuxDist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/buildMacDist.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/buildWinDist.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/charlieTest.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/exportCsvFormulae.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/exportCsvFromXbrlInstance.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/generateTestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/reportAllTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runAllTests.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2138 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runESMAtests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runGUI.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      266 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runGUI.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runGenerateVersioningTestcases.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runGeneratedTestcase.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runLocaleGettext.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runPackageTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runProfilerXDTTest.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      557 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runPyTest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runTR2Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runTR3Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runTR4Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runTR5Tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runTRSECTests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runUS-GFMTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/runVersioningConsumptionTests.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/startWebServer-27.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-01 19:53:47.000000 arelle-release-2.9.0/scripts/startWebServer.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-01 19:54:03.860487 arelle-release-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-01 19:53:47.000000 arelle-release-2.9.0/testParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-01 19:53:47.000000 arelle-release-2.9.0/testParser2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.856487 arelle-release-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.752484 arelle-release-2.9.0/tests/integration_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.752484 arelle-release-2.9.0/tests/integration_tests/ui_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.856487 arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.856487 arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj
+-rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Usings.cs
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.856487 arelle-release-2.9.0/tests/integration_tests/ui_tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   223544 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/ui_tests/resources/workiva.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.856487 arelle-release-2.9.0/tests/integration_tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.860487 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_assertion_severity_2_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_link_role_registry_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29081 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_taxonomy_packages_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_transformation_registry_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/download_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/run_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/test_conformance_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/integration_tests/validation/validation_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.752484 arelle-release-2.9.0/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.860487 arelle-release-2.9.0/tests/unit_tests/arelle/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.860487 arelle-release-2.9.0/tests/unit_tests/arelle/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.860487 arelle-release-2.9.0/tests/unit_tests/arelle/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/plugin/test_loadfromoim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_cntlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_modelmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_packagemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_pluginmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_qname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_urlutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tests/unit_tests/arelle/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-01 19:53:47.000000 arelle-release-2.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.752484 arelle-release-2.9.0/vms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 19:54:03.860487 arelle-release-2.9.0/vms/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-01 19:53:47.000000 arelle-release-2.9.0/vms/mac/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1478 2023-05-01 19:53:47.000000 arelle-release-2.9.0/vms/mac/create-macos-bootable-for-virtualbox.sh
```

### Comparing `arelle-release-2.8.1/.github/ISSUE_TEMPLATE/bug.yml` & `arelle-release-2.9.0/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/build-and-release-linux.yml` & `arelle-release-2.9.0/.github/workflows/build-and-release-linux.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/build-and-release-mac.yml` & `arelle-release-2.9.0/.github/workflows/build-and-release-mac.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/build-and-release-windows.yml` & `arelle-release-2.9.0/.github/workflows/build-and-release-windows.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/build-windows.yml` & `arelle-release-2.9.0/.github/workflows/build-windows.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/conformance-suites.yml` & `arelle-release-2.9.0/.github/workflows/conformance-suites.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/python-package.yml` & `arelle-release-2.9.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/release.yml` & `arelle-release-2.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/test-ui.yml` & `arelle-release-2.9.0/.github/workflows/test-ui.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.github/workflows/tests.yml` & `arelle-release-2.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/.gitignore` & `arelle-release-2.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/CONTRIBUTING.md` & `arelle-release-2.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/EFM-only-test.ini` & `arelle-release-2.9.0/EFM-only-test.ini`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/LICENSE.md` & `arelle-release-2.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/PKG-INFO` & `arelle-release-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arelle-release
-Version: 2.8.1
+Version: 2.9.0
 Summary: An open source XBRL platform.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `arelle-release-2.8.1/QuickBooks.qwc` & `arelle-release-2.9.0/QuickBooks.qwc`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/README.md` & `arelle-release-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/apidocs/Makefile` & `arelle-release-2.9.0/apidocs/Makefile`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/apidocs/arelle.rst` & `arelle-release-2.9.0/apidocs/arelle.rst`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/apidocs/conf.py` & `arelle-release-2.9.0/apidocs/conf.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/apidocs/make.bat` & `arelle-release-2.9.0/apidocs/make.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/Aspect.py` & `arelle-release-2.9.0/arelle/Aspect.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/Cntlr.py` & `arelle-release-2.9.0/arelle/Cntlr.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/CntlrCmdLine.py` & `arelle-release-2.9.0/arelle/CntlrCmdLine.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/CntlrComServer.py` & `arelle-release-2.9.0/arelle/CntlrComServer.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/CntlrProfiler.py` & `arelle-release-2.9.0/arelle/CntlrProfiler.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/CntlrQuickBooks.py` & `arelle-release-2.9.0/arelle/CntlrQuickBooks.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/CntlrWebMain.py` & `arelle-release-2.9.0/arelle/CntlrWebMain.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/CntlrWinMain.py` & `arelle-release-2.9.0/arelle/CntlrWinMain.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/CntlrWinTooltip.py` & `arelle-release-2.9.0/arelle/CntlrWinTooltip.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogAbout.py` & `arelle-release-2.9.0/arelle/DialogAbout.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogArcroleGroup.py` & `arelle-release-2.9.0/arelle/DialogArcroleGroup.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogFind.py` & `arelle-release-2.9.0/arelle/DialogFind.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogFormulaParameters.py` & `arelle-release-2.9.0/arelle/DialogFormulaParameters.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogLanguage.py` & `arelle-release-2.9.0/arelle/DialogLanguage.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogNewFactItem.py` & `arelle-release-2.9.0/arelle/DialogNewFactItem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogOpenArchive.py` & `arelle-release-2.9.0/arelle/DialogOpenArchive.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogPackageManager.py` & `arelle-release-2.9.0/arelle/DialogPackageManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogPluginManager.py` & `arelle-release-2.9.0/arelle/DialogPluginManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogRssWatch.py` & `arelle-release-2.9.0/arelle/DialogRssWatch.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogURL.py` & `arelle-release-2.9.0/arelle/DialogURL.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DialogUserPassword.py` & `arelle-release-2.9.0/arelle/DialogUserPassword.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/DisclosureSystem.py` & `arelle-release-2.9.0/arelle/DisclosureSystem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/FileSource.py` & `arelle-release-2.9.0/arelle/FileSource.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/FunctionCustom.py` & `arelle-release-2.9.0/arelle/FunctionCustom.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/FunctionFn.py` & `arelle-release-2.9.0/arelle/FunctionFn.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/FunctionIxt.py` & `arelle-release-2.9.0/arelle/FunctionIxt.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/FunctionUtil.py` & `arelle-release-2.9.0/arelle/FunctionUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/FunctionXfi.py` & `arelle-release-2.9.0/arelle/FunctionXfi.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/FunctionXs.py` & `arelle-release-2.9.0/arelle/FunctionXs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/HashUtil.py` & `arelle-release-2.9.0/arelle/HashUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/HtmlUtil.py` & `arelle-release-2.9.0/arelle/HtmlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/InstanceAspectsEvaluator.py` & `arelle-release-2.9.0/arelle/InstanceAspectsEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/LeiUtil.py` & `arelle-release-2.9.0/arelle/LeiUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/LocalViewer.py` & `arelle-release-2.9.0/arelle/LocalViewer.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/Locale.py` & `arelle-release-2.9.0/arelle/Locale.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelDocument.py` & `arelle-release-2.9.0/arelle/ModelDocument.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelDtsObject.py` & `arelle-release-2.9.0/arelle/ModelDtsObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelFormulaObject.py` & `arelle-release-2.9.0/arelle/ModelFormulaObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelInstanceObject.py` & `arelle-release-2.9.0/arelle/ModelInstanceObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelManager.py` & `arelle-release-2.9.0/arelle/ModelManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelObject.py` & `arelle-release-2.9.0/arelle/ModelObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelObjectFactory.py` & `arelle-release-2.9.0/arelle/ModelObjectFactory.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelRelationshipSet.py` & `arelle-release-2.9.0/arelle/ModelRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelRenderingObject.py` & `arelle-release-2.9.0/arelle/ModelRenderingObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelRssItem.py` & `arelle-release-2.9.0/arelle/ModelRssItem.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelRssObject.py` & `arelle-release-2.9.0/arelle/ModelRssObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelTestcaseObject.py` & `arelle-release-2.9.0/arelle/ModelTestcaseObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelValue.py` & `arelle-release-2.9.0/arelle/ModelValue.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelVersObject.py` & `arelle-release-2.9.0/arelle/ModelVersObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelVersReport.py` & `arelle-release-2.9.0/arelle/ModelVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ModelXbrl.py` & `arelle-release-2.9.0/arelle/ModelXbrl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/PackageManager.py` & `arelle-release-2.9.0/arelle/PackageManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/PluginManager.py` & `arelle-release-2.9.0/arelle/PluginManager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/PrototypeDtsObject.py` & `arelle-release-2.9.0/arelle/PrototypeDtsObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/PrototypeInstanceObject.py` & `arelle-release-2.9.0/arelle/PrototypeInstanceObject.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/PythonUtil.py` & `arelle-release-2.9.0/arelle/PythonUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/RenderingEvaluator.py` & `arelle-release-2.9.0/arelle/RenderingEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/RenderingResolver.py` & `arelle-release-2.9.0/arelle/RenderingResolver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/SystemInfo.py` & `arelle-release-2.9.0/arelle/SystemInfo.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/TableStructure.py` & `arelle-release-2.9.0/arelle/TableStructure.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/TkTableWrapper.py` & `arelle-release-2.9.0/arelle/TkTableWrapper.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/UITkTable.py` & `arelle-release-2.9.0/arelle/UITkTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/UiUtil.py` & `arelle-release-2.9.0/arelle/UiUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/Updater.py` & `arelle-release-2.9.0/arelle/Updater.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/UrlUtil.py` & `arelle-release-2.9.0/arelle/UrlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/Validate.py` & `arelle-release-2.9.0/arelle/Validate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ValidateFilingText.py` & `arelle-release-2.9.0/arelle/ValidateFilingText.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ValidateInfoset.py` & `arelle-release-2.9.0/arelle/ValidateInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ValidateUtr.py` & `arelle-release-2.9.0/arelle/ValidateUtr.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ValidateVersReport.py` & `arelle-release-2.9.0/arelle/ValidateVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ValidateXbrl.py` & `arelle-release-2.9.0/arelle/ValidateXbrl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ValidateXbrlCalcs.py` & `arelle-release-2.9.0/arelle/ValidateXbrlCalcs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ValidateXbrlDTS.py` & `arelle-release-2.9.0/arelle/ValidateXbrlDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ValidateXbrlDimensions.py` & `arelle-release-2.9.0/arelle/ValidateXbrlDimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/Version.py` & `arelle-release-2.9.0/arelle/Version.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFile.py` & `arelle-release-2.9.0/arelle/ViewFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileConcepts.py` & `arelle-release-2.9.0/arelle/ViewFileConcepts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileDTS.py` & `arelle-release-2.9.0/arelle/ViewFileDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileFactList.py` & `arelle-release-2.9.0/arelle/ViewFileFactList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileFactTable.py` & `arelle-release-2.9.0/arelle/ViewFileFactTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileFormulae.py` & `arelle-release-2.9.0/arelle/ViewFileFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileRelationshipSet.py` & `arelle-release-2.9.0/arelle/ViewFileRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileRenderedGrid.py` & `arelle-release-2.9.0/arelle/ViewFileRenderedGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileRoleTypes.py` & `arelle-release-2.9.0/arelle/ViewFileRoleTypes.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileRssFeed.py` & `arelle-release-2.9.0/arelle/ViewFileRssFeed.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewFileTests.py` & `arelle-release-2.9.0/arelle/ViewFileTests.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewUtil.py` & `arelle-release-2.9.0/arelle/ViewUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewUtilFormulae.py` & `arelle-release-2.9.0/arelle/ViewUtilFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinConcepts.py` & `arelle-release-2.9.0/arelle/ViewWinConcepts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinDTS.py` & `arelle-release-2.9.0/arelle/ViewWinDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinDiffs.py` & `arelle-release-2.9.0/arelle/ViewWinDiffs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinFactGrid.py` & `arelle-release-2.9.0/arelle/ViewWinFactGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinFactList.py` & `arelle-release-2.9.0/arelle/ViewWinFactList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinFactTable.py` & `arelle-release-2.9.0/arelle/ViewWinFactTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinFormulae.py` & `arelle-release-2.9.0/arelle/ViewWinFormulae.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinGrid.py` & `arelle-release-2.9.0/arelle/ViewWinGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinList.py` & `arelle-release-2.9.0/arelle/ViewWinList.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinPane.py` & `arelle-release-2.9.0/arelle/ViewWinPane.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinProperties.py` & `arelle-release-2.9.0/arelle/ViewWinProperties.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinRelationshipSet.py` & `arelle-release-2.9.0/arelle/ViewWinRelationshipSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinRenderedGrid.py` & `arelle-release-2.9.0/arelle/ViewWinRenderedGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinRoleTypes.py` & `arelle-release-2.9.0/arelle/ViewWinRoleTypes.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinRssFeed.py` & `arelle-release-2.9.0/arelle/ViewWinRssFeed.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinTests.py` & `arelle-release-2.9.0/arelle/ViewWinTests.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinTkTable.py` & `arelle-release-2.9.0/arelle/ViewWinTkTable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinTree.py` & `arelle-release-2.9.0/arelle/ViewWinTree.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinTupleGrid.py` & `arelle-release-2.9.0/arelle/ViewWinTupleGrid.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinVersReport.py` & `arelle-release-2.9.0/arelle/ViewWinVersReport.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/ViewWinXml.py` & `arelle-release-2.9.0/arelle/ViewWinXml.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/WatchRss.py` & `arelle-release-2.9.0/arelle/WatchRss.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/WebCache.py` & `arelle-release-2.9.0/arelle/WebCache.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/XbrlConst.py` & `arelle-release-2.9.0/arelle/XbrlConst.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/XbrlUtil.py` & `arelle-release-2.9.0/arelle/XbrlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/XhtmlValidate.py` & `arelle-release-2.9.0/arelle/XhtmlValidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/XmlUtil.py` & `arelle-release-2.9.0/arelle/XmlUtil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/XmlValidate.py` & `arelle-release-2.9.0/arelle/XmlValidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/XmlValidateParticles.py` & `arelle-release-2.9.0/arelle/XmlValidateParticles.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/XmlValidateSchema.py` & `arelle-release-2.9.0/arelle/XmlValidateSchema.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/arelle_test.ini` & `arelle-release-2.9.0/arelle/config/arelle_test.ini`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/creationSoftwareNames.json` & `arelle-release-2.9.0/arelle/config/creationSoftwareNames.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/disclosuresystems.xml` & `arelle-release-2.9.0/arelle/config/disclosuresystems.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/disclosuresystems.xsd` & `arelle-release-2.9.0/arelle/config/disclosuresystems.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/edbody.dtd` & `arelle-release-2.9.0/arelle/config/edbody.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/erxl.xsd` & `arelle-release-2.9.0/arelle/config/erxl.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/mappings.xml` & `arelle-release-2.9.0/arelle/config/mappings.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/mappings.xsd` & `arelle-release-2.9.0/arelle/config/mappings.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/xbrlschemafiles.xml` & `arelle-release-2.9.0/arelle/config/xbrlschemafiles.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/xhtml-lat1.ent` & `arelle-release-2.9.0/arelle/config/xhtml-lat1.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/xhtml-special.ent` & `arelle-release-2.9.0/arelle/config/xhtml-special.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/xhtml-symbol.ent` & `arelle-release-2.9.0/arelle/config/xhtml-symbol.ent`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/xhtml1-strict-ix.dtd` & `arelle-release-2.9.0/arelle/config/xhtml1-strict-ix.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/config/xhtml1_1-strict-ix.dtd` & `arelle-release-2.9.0/arelle/config/xhtml1_1-strict-ix.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/doc/messagesCatalog.xml` & `arelle-release-2.9.0/arelle/doc/messagesCatalog.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/doc/messagesCatalog.xsd` & `arelle-release-2.9.0/arelle/doc/messagesCatalog.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/CustomLogger.py` & `arelle-release-2.9.0/arelle/examples/CustomLogger.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/LoadEFMvalidate.py` & `arelle-release-2.9.0/arelle/examples/LoadEFMvalidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/LoadSavePreLbCsv.py` & `arelle-release-2.9.0/arelle/examples/LoadSavePreLbCsv.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/LoadValidate.cs` & `arelle-release-2.9.0/arelle/examples/LoadValidate.cs`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/LoadValidate.py` & `arelle-release-2.9.0/arelle/examples/LoadValidate.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/LoadValidateCmdLine.java` & `arelle-release-2.9.0/arelle/examples/LoadValidateCmdLine.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/LoadValidatePostedZip.java` & `arelle-release-2.9.0/arelle/examples/LoadValidatePostedZip.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/LoadValidateWebService.java` & `arelle-release-2.9.0/arelle/examples/LoadValidateWebService.java`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/SaveTableToExelle.py` & `arelle-release-2.9.0/arelle/examples/SaveTableToExelle.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/TR3toTR4.py` & `arelle-release-2.9.0/arelle/examples/TR3toTR4.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/bigInstance.py` & `arelle-release-2.9.0/arelle/examples/plugin/bigInstance.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/cmdWebServerExtension.py` & `arelle-release-2.9.0/arelle/examples/plugin/cmdWebServerExtension.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/crashTest.py` & `arelle-release-2.9.0/arelle/examples/plugin/crashTest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/formulaSuiteConverter.py` & `arelle-release-2.9.0/arelle/examples/plugin/formulaSuiteConverter.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/functionsCustom.py` & `arelle-release-2.9.0/arelle/examples/plugin/functionsCustom.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/hello_dolly.py` & `arelle-release-2.9.0/arelle/examples/plugin/hello_dolly.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/hello_i18n.pot` & `arelle-release-2.9.0/arelle/examples/plugin/hello_i18n.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/hello_i18n.py` & `arelle-release-2.9.0/arelle/examples/plugin/hello_i18n.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/importTestChild1.py` & `arelle-release-2.9.0/arelle/examples/plugin/importTestChild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/importTestChild2.py` & `arelle-release-2.9.0/arelle/examples/plugin/importTestChild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/importTestGrandchild1.py` & `arelle-release-2.9.0/arelle/examples/plugin/importTestGrandchild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/importTestGrandchild2.py` & `arelle-release-2.9.0/arelle/examples/plugin/importTestGrandchild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/importTestImported1.py` & `arelle-release-2.9.0/arelle/examples/plugin/importTestImported1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/importTestImported11.py` & `arelle-release-2.9.0/arelle/examples/plugin/importTestImported11.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/importTestParent.py` & `arelle-release-2.9.0/arelle/examples/plugin/importTestParent.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po` & `arelle-release-2.9.0/arelle/examples/plugin/locale/fr/LC_MESSAGES/hello_i18n.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/__init__.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestChild1.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestChild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestChild2.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestChild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestGrandchild2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestImported1.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestImported1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/importTestImported11.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/importTestImported11.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/subdir/importTestImported111.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py` & `arelle-release-2.9.0/arelle/examples/plugin/packagedImportTest/subdir/subsubdir/importTestImported1111.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/sakaCalendar.py` & `arelle-release-2.9.0/arelle/examples/plugin/sakaCalendar.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/saveInstanceInfoset.py` & `arelle-release-2.9.0/arelle/examples/plugin/saveInstanceInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/streamingExtensions.py` & `arelle-release-2.9.0/arelle/examples/plugin/streamingExtensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py` & `arelle-release-2.9.0/arelle/examples/plugin/testcaseIxExpectedHtmlFixup.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/updateTableLB.py` & `arelle-release-2.9.0/arelle/examples/plugin/updateTableLB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/validateSchemaLxml.py` & `arelle-release-2.9.0/arelle/examples/plugin/validateSchemaLxml.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/plugin/validateTableInfoset.py` & `arelle-release-2.9.0/arelle/examples/plugin/validateTableInfoset.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/us-gaap-dei-docType-extraction-frm.xml` & `arelle-release-2.9.0/arelle/examples/us-gaap-dei-docType-extraction-frm.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/examples/us-gaap-dei-ratio-cash-frm.xml` & `arelle-release-2.9.0/arelle/examples/us-gaap-dei-ratio-cash-frm.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/formula/FactAspectsCache.py` & `arelle-release-2.9.0/arelle/formula/FactAspectsCache.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/formula/FormulaConsisAsser.py` & `arelle-release-2.9.0/arelle/formula/FormulaConsisAsser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/formula/FormulaEvaluator.py` & `arelle-release-2.9.0/arelle/formula/FormulaEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/formula/ValidateFormula.py` & `arelle-release-2.9.0/arelle/formula/ValidateFormula.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/formula/XPathContext.py` & `arelle-release-2.9.0/arelle/formula/XPathContext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/formula/XPathParser.py` & `arelle-release-2.9.0/arelle/formula/XPathParser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle-full-word.ico` & `arelle-release-2.9.0/arelle/images/arelle-full-word.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle-mac-icon-4.gif` & `arelle-release-2.9.0/arelle/images/arelle-mac-icon-4.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle-word-only.ico` & `arelle-release-2.9.0/arelle/images/arelle-word-only.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle.gif` & `arelle-release-2.9.0/arelle/images/arelle.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle.icns` & `arelle-release-2.9.0/arelle/images/arelle.icns`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle.icns.zip` & `arelle-release-2.9.0/arelle/images/arelle.icns.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle.ico` & `arelle-release-2.9.0/arelle/images/arelle.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle128.psd` & `arelle-release-2.9.0/arelle/images/arelle128.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle16.psd` & `arelle-release-2.9.0/arelle/images/arelle16.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle16x16and32x32.ico` & `arelle-release-2.9.0/arelle/images/arelle16x16and32x32.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/arelle32.gif` & `arelle-release-2.9.0/arelle/images/arelle32.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/dmg_background.png` & `arelle-release-2.9.0/arelle/images/dmg_background.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/octocat.png` & `arelle-release-2.9.0/arelle/images/octocat.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/python-clear.png` & `arelle-release-2.9.0/arelle/images/python-clear.png`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/python-icon-pack-crystalxp.net-842.zip` & `arelle-release-2.9.0/arelle/images/python-icon-pack-crystalxp.net-842.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarClose.gif` & `arelle-release-2.9.0/arelle/images/toolbarClose.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarCompare.gif` & `arelle-release-2.9.0/arelle/images/toolbarCompare.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarFindMenu.gif` & `arelle-release-2.9.0/arelle/images/toolbarFindMenu.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarLogClear - 1-piece-top.gif` & `arelle-release-2.9.0/arelle/images/toolbarLogClear - 1-piece-top.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarLogClear-orig.gif` & `arelle-release-2.9.0/arelle/images/toolbarLogClear-orig.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarLogClear.gif` & `arelle-release-2.9.0/arelle/images/toolbarLogClear.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarNewFile.gif` & `arelle-release-2.9.0/arelle/images/toolbarNewFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarOpenFile.gif` & `arelle-release-2.9.0/arelle/images/toolbarOpenFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarOpenWeb.gif` & `arelle-release-2.9.0/arelle/images/toolbarOpenWeb.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarReopen.gif` & `arelle-release-2.9.0/arelle/images/toolbarReopen.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarSaveFile.gif` & `arelle-release-2.9.0/arelle/images/toolbarSaveFile.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/toolbarValidate.gif` & `arelle-release-2.9.0/arelle/images/toolbarValidate.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/xbrl.gif` & `arelle-release-2.9.0/arelle/images/xbrl.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/xbrl.psd` & `arelle-release-2.9.0/arelle/images/xbrl.psd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/xbrl128-2.gif` & `arelle-release-2.9.0/arelle/images/xbrl128-2.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/xbrl128.gif` & `arelle-release-2.9.0/arelle/images/xbrl128.gif`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/xbrl16.ico` & `arelle-release-2.9.0/arelle/images/xbrl16.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/images/xbrl32.ico` & `arelle-release-2.9.0/arelle/images/xbrl32.ico`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po` & `arelle-release-2.9.0/arelle/locale/ar_EG/LC_MESSAGES/ar_EG.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo` & `arelle-release-2.9.0/arelle/locale/ar_EG/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/locale/es/LC_MESSAGES/arelle.mo` & `arelle-release-2.9.0/arelle/locale/es/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/locale/fr/LC_MESSAGES/arelle.mo` & `arelle-release-2.9.0/arelle/locale/fr/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/locale/fr/LC_MESSAGES/fr.po` & `arelle-release-2.9.0/arelle/locale/fr/LC_MESSAGES/fr.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/locale/messages.pot` & `arelle-release-2.9.0/arelle/locale/messages.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/locale/ru/LC_MESSAGES/arelle.mo` & `arelle-release-2.9.0/arelle/locale/ru/LC_MESSAGES/arelle.mo`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/locale/ru/LC_MESSAGES/ru.po` & `arelle-release-2.9.0/arelle/locale/ru/LC_MESSAGES/ru.po`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/EdgarRendererAllReports.py` & `arelle-release-2.9.0/arelle/plugin/EdgarRendererAllReports.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/SECCorrespondenceLoader.py` & `arelle-release-2.9.0/arelle/plugin/SECCorrespondenceLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/TDnetLoader.py` & `arelle-release-2.9.0/arelle/plugin/TDnetLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/UKCompaniesHouseLoader.py` & `arelle-release-2.9.0/arelle/plugin/UKCompaniesHouseLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/formulaLoader.py` & `arelle-release-2.9.0/arelle/plugin/formulaLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/formulaSaver.py` & `arelle-release-2.9.0/arelle/plugin/formulaSaver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/formulaXPathChecker.py` & `arelle-release-2.9.0/arelle/plugin/formulaXPathChecker.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/functionsMath.py` & `arelle-release-2.9.0/arelle/plugin/functionsMath.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/functionsXmlCreation.py` & `arelle-release-2.9.0/arelle/plugin/functionsXmlCreation.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/inlineXbrlDocumentSet.py` & `arelle-release-2.9.0/arelle/plugin/inlineXbrlDocumentSet.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/instanceInfo.py` & `arelle-release-2.9.0/arelle/plugin/instanceInfo.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py` & `arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/HTTPNtlmAuthHandler.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/U32.py` & `arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/U32.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/__init__.py` & `arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/des.py` & `arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/des.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/des_c.py` & `arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/des_c.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/des_data.py` & `arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/des_data.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html` & `arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/lgpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/internet/proxyNTLM/ntlm.py` & `arelle-release-2.9.0/arelle/plugin/internet/proxyNTLM/ntlm.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/loadFromExcel.py` & `arelle-release-2.9.0/arelle/plugin/loadFromExcel.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/loadFromOIM-2018.py` & `arelle-release-2.9.0/arelle/plugin/loadFromOIM-2018.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/loadFromOIM.py` & `arelle-release-2.9.0/arelle/plugin/loadFromOIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -923,15 +923,15 @@
                         else:
                             _valueKeyDict[value] = key
             return _dict
 
         primaryOimFile = oimFile
         extensionProperties = OrderedDict() # key is property QName, value is property path
 
-        def loadOimObject(oimFile, extendingFile, visitedFiles, primaryReportParameters=None): # returns oimObject, oimWb
+        def loadOimObject(oimFile, extendingFile, visitedFiles, extensionChain, primaryReportParameters=None): # returns oimObject, oimWb
             # isXL means metadata loaded from Excel (but instance data can be in excel or CSV)
             isXL = oimFile.endswith(".xlsx") or oimFile.endswith(".xls")
             # same logic as modelDocument.load
             normalizedUrl = modelXbrl.modelManager.cntlr.webCache.normalizeUrl(oimFile, extendingFile)
             if modelXbrl.fileSource.isMappedUrl(normalizedUrl):
                 mappedUrl = modelXbrl.fileSource.mappedUrl(normalizedUrl)
             elif PackageManager.isMappedUrl(normalizedUrl):
@@ -945,17 +945,22 @@
                 if filepath:
                     url = modelXbrl.modelManager.cntlr.webCache.normalizeUrl(filepath)
             if filepath and filepath.endswith(".csv") or ("metadata" in filepath and filepath.endswith(".json")):
                 errPrefix = "xbrlce"
             else:
                 errPrefix = "xbrlje"
             # prevent recursion
-            if filepath in visitedFiles:
-                return None # block directed cycle looping
+            if filepath in extensionChain:
+                raise OIMException("{}:cycleInExtensionChain".format(errPrefix),
+                      _("File MUST NOT extend itself: %(file)s cycles to %(extendingFile)s"),
+                      file=filepath, extendingFile=extendingFile)
+            elif filepath in visitedFiles:
+                return None
             visitedFiles.add(filepath)
+            extensionChain.add(filepath)
             if not isXL:
                 try:
                     _file = modelXbrl.fileSource.file(filepath, encoding="utf-8-sig")[0]
                     with _file as f:
                         chars = f.read(16) # test encoding
                         m = UTF_7_16_Pattern.match(chars)
                         if m:
@@ -1108,14 +1113,15 @@
                         mbrNdx += 1
             checkMemberTypes(oimObject, "/", [])
             numErrorsBeforeJsonCheck = len(modelXbrl.errors)
             if not isJSON and not isCSV and not isXL:
                 error("oimce:unsupportedDocumentType",
                       _("Unrecognized /documentInfo/docType: %(documentType)s"),
                       documentType=documentType)
+                extensionChain.discard(filepath)
                 return {}
             if missingRequiredMembers or unexpectedMembers:
                 msg = []
                 if missingRequiredMembers:
                     msg.append(_("Required element(s) are missing from metadata: %(missing)s"))
                 if unexpectedMembers:
                     msg.append(_("Unexpected element(s) in metadata: %(unexpected)s"))
@@ -1184,15 +1190,21 @@
                 t = documentInfo.get("taxonomy",())
                 for i, tUrl in enumerate(t):
                     t[i] = modelXbrl.modelManager.cntlr.webCache.normalizeUrl(tUrl, normalizedUrl)
 
             if isCSVorXL and "extends" in documentInfo:
                 # process extension
                 for extendedFile in documentInfo["extends"]:
-                    extendedOimObject = loadOimObject(extendedFile, mappedUrl, visitedFiles)
+                    try:
+                        extendedOimObject = loadOimObject(extendedFile, mappedUrl, visitedFiles, extensionChain)
+                    except FileNotFoundError:
+                        error("{}:unresolvableBaseMetadataFile".format(errPrefix),
+                              _("Extending document file not found: %(extendingFile)s, referenced from %(extendedFile)s"),
+                              extendingFile=extendedFile, extendedFile=oimFile)
+                        raise OIMException()
                     if extendedOimObject is None:
                         continue # None returned when directed cycle blocks reloading same file
                     # extended must be CSV
                     extendedDocumentInfo = extendedOimObject.get("documentInfo", EMPTY_DICT)
                     extendedDocumentType = extendedDocumentInfo.get("documentType")
                     extendedFinal = extendedDocumentInfo.get("final", EMPTY_DICT)
                     if extendedDocumentType != documentType:
@@ -1222,15 +1234,15 @@
                                     if extendedFinal.get(objectName, False) and parProp not in extendedParent.get(objectName,EMPTY_DICT):
                                         error("xbrlce:illegalExtensionOfFinalProperty",
                                               _("Extended file %(extendedFile)s specifies final object %(objectName)s property %(property)s"),
                                               extendedFile=oimFile, objectName=objectName, property=parProp)
                                 for extProp, extPropValue in extendedParent.get(objectName,EMPTY_DICT).items():
                                     if extProp in parent.get(objectName,EMPTY_DICT):
                                         if json.dumps(extPropValue,sort_keys=True) != json.dumps(parent[objectName][extProp],sort_keys=True): # ordered dicts, especially nested are not comparable
-                                            error("xbrlce:illegalExtensionOfFinalProperty" if extendedFinal.get(objectName, False)
+                                            error("xbrlce:conflictingMetadataValue" if extendedFinal.get(objectName, False)
                                                   else "xbrlce:conflictingMetadataValue",
                                                   _("Extended file %(extendedFile)s redefines object %(objectName)s property %(property)s"),
                                                   extendedFile=extendedFile, objectName=objectName, property=extProp)
                                     else:
                                         if objectName not in parent:
                                             parent[objectName] = {}
                                         parent[objectName][extProp] = extPropValue
@@ -1251,18 +1263,19 @@
                     error("oime:noTaxonomy",
                           _("The list of taxonomies MUST NOT be empty."))
                 if  len(modelXbrl.errors) > numErrorsBeforeJsonCheck:
                     raise OIMException()
 
                 oimObject["=entryParameters"] = (isJSON, isCSV, isXL, isCSVorXL, oimWb, documentInfo, documentType, documentBase)
 
+            extensionChain.discard(filepath)
             return oimObject
 
         errorIndexBeforeLoadOim = len(modelXbrl.errors)
-        oimObject = loadOimObject(oimFile, None, set())
+        oimObject = loadOimObject(oimFile, None, set(), set())
         try:
             isJSON, isCSV, isXL, isCSVorXL, oimWb, oimDocumentInfo, documentType, documentBase = oimObject["=entryParameters"]
         except KeyError:
             raise OIMException() # no document
         del oimObject["=entryParameters"]
 
         currentAction = "identifying Metadata objects"
@@ -1412,17 +1425,16 @@
                                 tableParameterReferenceNames.add(paramName)
                         unitDims = set()
                         for factColName, colDims in factDimensions.items():
                             if colDims is not None:
                                 factDims = set()
                                 for inheritedDims in (colDims, tableDimensions, reportDimensions):
                                     for dimName, dimValue in inheritedDims.items():
-                                        if True: # dimName not in factDims:
-                                            checkParamRef(dimValue, factColName, dimName)
-                                            factDims.add(dimName)
+                                        checkParamRef(dimValue, factColName, dimName)
+                                        factDims.add(dimName)
                                 parseMetadataCellValues(colDims)
                                 for _factDecimals in (factDecimals.get(factColName), tableDecimals, reportDecimals):
                                     if "decimals" not in factDims:
                                         checkParamRef(_factDecimals, factColName, "decimals")
 
                         if hasHeaderError:
                             return
@@ -1556,29 +1568,38 @@
                                         if source:
                                             yield {"decimals": dec}, source
                                 for inheritedDims, dimSource in dimChecks():
                                     for dimName, dimValue in inheritedDims.items():
                                         if dimName not in checkedDims:
                                             dimValue = inheritedDims[dimName]
                                             # resolve column-relative dimensions
-                                            if isinstance(dimValue, str) and dimValue.startswith("$"):
-                                                dimValue = dimValue[1:]
-                                                if not dimValue.startswith("$"):
-                                                    dimValue, _sep, dimAttr = dimValue.partition("@")
-                                                    if _sep and dimAttr not in ("start", "end"):
-                                                        hasHeaderError = True
-                                                        error("xbrlce:invalidPeriodSpecifier",
-                                                              _("Table %(table)s %(source)s %(dimension)s period-specifier invalid: %(target)s, url: %(url)s"),
-                                                              table=tableId, source=dimSource, dimension=dimName, target=dimAttr, url=tableUrl)
-                                                    if dimValue not in checkedParams:
-                                                        checkedParams.add(dimValue)
-                                                        if dimValue in ("rowNumber", ) or (dimValue in header and dimValue not in commentColumns) or dimValue in tableParameters or dimValue in reportParameters:
-                                                            checkedDims.add(dimValue)
-                                                        else:
-                                                            potentialInvalidReferenceTargets[dimName] = dimValue
+                                            if isinstance(dimValue, str):
+                                                if dimValue.startswith("$"):
+                                                    dimValue = dimValue[1:]
+                                                    if not dimValue.startswith("$"):
+                                                        dimValue, _sep, dimAttr = dimValue.partition("@")
+                                                        if _sep and dimAttr not in ("start", "end"):
+                                                            hasHeaderError = True
+                                                            error("xbrlce:invalidPeriodSpecifier",
+                                                                  _("Table %(table)s %(source)s %(dimension)s period-specifier invalid: %(target)s, url: %(url)s"),
+                                                                  table=tableId, source=dimSource, dimension=dimName, target=dimAttr, url=tableUrl)
+                                                        if dimValue not in checkedParams:
+                                                            checkedParams.add(dimValue)
+                                                            if dimValue in ("rowNumber", ) or (dimValue in header and dimValue not in commentColumns) or dimValue in tableParameters or dimValue in reportParameters:
+                                                                checkedDims.add(dimValue)
+                                                            else:
+                                                                potentialInvalidReferenceTargets[dimName] = dimValue
+                                                elif ":" in dimName and ":" in dimValue:
+                                                    dimConcept = modelXbrl.qnameConcepts.get(qname(dimName, namespaces))
+                                                    if dimConcept is not None and dimConcept.isExplicitDimension:
+                                                        memConcept = modelXbrl.qnameConcepts.get(qname(dimValue, namespaces))
+                                                        if memConcept is not None and modelXbrl.dimensionDefaultConcepts.get(dimConcept) == memConcept:
+                                                            error("xbrlce:invalidDimensionValue",
+                                                                  _("Table %(table)s %(source)s %(dimension)s value must not be the default member %(member)s, url: %(url)s"),
+                                                                  table=tableId, source=dimSource, dimension=dimName, member=dimValue, url=tableUrl)
                                 for commentCol in commentColumns:
                                     colNameIndex.pop(commentCol,None) # remove comment columns from col name index
                                 unreportedFactDimensionColumns = factDimensions.keys() - set(header)
                                 reportedDimensionsColumns = dimensionsColumns & set(header)
                                 if hasHeaderError:
                                     break # stop processing table
                             else:
@@ -1838,14 +1859,15 @@
         # create the instance document
         currentAction = "creating instance document"
         # relativize taxonomyRefs to base where feasible
         txBase = os.path.dirname(documentBase or (modelXbrl.entryLoadingUrl if modelXbrl else ""))
         for i, tUrl in enumerate(taxonomyRefs or ()):
             if not isAbsoluteUri(tUrl) and os.path.isabs(tUrl) and not isAbsoluteUri(txBase) and os.path.isabs(txBase):
                 taxonomyRefs[i] = os.path.relpath(tUrl, txBase)
+        prevErrLen = len(modelXbrl.errors) # track any xbrl validation errors
         if modelXbrl: # pull loader implementation
             modelXbrl.blockDpmDBrecursion = True
             modelXbrl.modelDocument = _return = createModelDocument(
                   modelXbrl,
                   Type.INSTANCE,
                   instanceFileName,
                   schemaRefs=taxonomyRefs,
@@ -1860,14 +1882,22 @@
                 Type.INSTANCE,
                 instanceFileName,
                 schemaRefs=taxonomyRefs,
                 isEntry=True,
                 initialComment="extracted from OIM {}".format(mappedUri),
                 base=documentBase)
             _return = modelXbrl.modelDocument
+        if len(modelXbrl.errors) > prevErrLen:
+            error("oime:invalidTaxonomy",
+                  _("Unable to obtain a valid taxonomy from URLs provided"),
+                  modelObject=modelXbrl)
+
+        currentAction = "identifying default dimensions"
+        if modelXbrl is not None:
+            ValidateXbrlDimensions.loadDimensionDefaults(modelXbrl) # needs dimension defaults
 
         # validate statically defined templates
         if isCSVorXL:
             currentAction = "checking statically defined dimensions in CSV templates"
             prevErrLen = len(modelXbrl.errors) # track any xbrl validation errors
             reportParametersUsed = set()
 
@@ -2068,18 +2098,23 @@
                               _("PropertiesFrom references repeat dimensions from: %(propFroms)s, dimension: %(dimensions)s at %(path)s."),
                               propFroms=", ".join(sorted(set(c for d,cs in dimPGs.items() if len(cs) > 1 for c in cs))),
                               dimensions=", ".join(sorted(d for d,cs in dimPGs.items() if len(cs) > 1)),
                               path="/tableTemplates/{}/columns/{}/propertiesFrom".format(tblTmplId,columnId))
 
 
                 rowIdColName = tblTmpl.get("rowIdColumn")
-                if rowIdColName and rowIdColName not in columns:
-                    error("xbrlce:undefinedRowIdColumn",
-                          _("RowIdColumn is not defined in columns: %(rowIdColumn)s at %(path)s"),
-                          rowIdColumn=rowIdColName, path="/tableTemplates/{}".format(tblTmplId))
+                if rowIdColName:
+                    if rowIdColName not in columns:
+                        error("xbrlce:undefinedRowIdColumn",
+                              _("RowIdColumn is not defined in columns: %(rowIdColumn)s at %(path)s"),
+                              rowIdColumn=rowIdColName, path="/tableTemplates/{}".format(tblTmplId))
+                    elif columns[rowIdColName].get("comment") == True:
+                        error("xbrlce:invalidRowIdColumn",
+                              _("RowIdColumn must not be a comment column: %(rowIdColumn)s at %(path)s"),
+                              rowIdColumn=rowIdColName, path="/tableTemplates/{}".format(tblTmplId))
 
             # table static checks
             for tableId, table in tables.items():
                 checkIdentifier(tableId, "/tables")
                 tblTmplId = table.get("template", tableId)
                 if checkIdentifier(tblTmplId, "/tables/{}/template".format(tableId)) and tblTmplId not in tableTemplates:
                     error("xbrlce:unknownTableTemplate",
@@ -2353,14 +2388,20 @@
                             if dimConcept.isExplicitDimension:
                                 mem = qname(dimVal, namespaces)
                                 if mem is None:
                                     error("{}:invalidDimensionValue".format(valErrPrefix),
                                           _("Fact %(factId)s taxonomy-defined explicit dimension value is invalid: %(memberQName)s."),
                                           modelObject=modelXbrl, factId=id, memberQName=dimVal)
                                     continue
+                                memConcept = modelXbrl.qnameConcepts.get(mem)
+                                if memConcept is not None and modelXbrl.dimensionDefaultConcepts.get(dimConcept) == memConcept:
+                                    error("{}:invalidDimensionValue".format("oime" if valErrPrefix == "xbrlje" else valErrPrefix),
+                                          _("Fact %(factId)s taxonomy-defined explicit dimension value must not be the default member: %(memberQName)s."),
+                                          modelObject=modelXbrl, factId=id, memberQName=dimVal)
+                                    continue
                             elif dimConcept.isTypedDimension:
                                 # a modelObject xml element is needed for all of the instance functions to manage the typed dim
                                 if dimConcept.typedDomainElement.baseXsdType in ("ENTITY", "ENTITIES", "ID", "IDREF", "IDREFS", "NMTOKEN", "NMTOKENS", "NOTATION") or (
                                    dimConcept.typedDomainElement.instanceOfType(dtrPrefixedContentTypes) and not dimConcept.typedDomainElement.instanceOfType(dtrSQNameNamesTypes)) or (
                                     dimConcept.typedDomainElement.type is not None and
                                     dimConcept.typedDomainElement.type.qname != XbrlConst.qnXbrliDateUnion and
                                     (dimConcept.typedDomainElement.type.localName == "complexType" or
@@ -2910,15 +2951,15 @@
             _zip.close()
             responseZipStream.seek(0)
 
 def validateFinally(val, *args, **kwargs):
     modelXbrl = val.modelXbrl
     if getattr(modelXbrl, "loadedFromOIM", False):
         if modelXbrl.loadedFromOimErrorCount < len(modelXbrl.errors):
-            modelXbrl.error("oime:invalidXBRL",
+            modelXbrl.error("oime:invalidTaxonomy",
                                 _("XBRL validation errors were logged for this instance."),
                                 modelObject=modelXbrl)
     else:
         # validate xBRL-XML instances
         fractionFacts = []
         tupleFacts = []
         precisionZeroFacts = []
```

### Comparing `arelle-release-2.8.1/arelle/plugin/logging/dpmSignature.py` & `arelle-release-2.9.0/arelle/plugin/logging/dpmSignature.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/logging/dqcParameters.py` & `arelle-release-2.9.0/arelle/plugin/logging/dqcParameters.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/logging/saveMessages.py` & `arelle-release-2.9.0/arelle/plugin/logging/saveMessages.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/objectmaker.py` & `arelle-release-2.9.0/arelle/plugin/objectmaker.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/profileCmdLine.py` & `arelle-release-2.9.0/arelle/plugin/profileCmdLine.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/profileFormula.py` & `arelle-release-2.9.0/arelle/plugin/profileFormula.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/saveCHComponentFile.py` & `arelle-release-2.9.0/arelle/plugin/saveCHComponentFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/saveDTS.py` & `arelle-release-2.9.0/arelle/plugin/saveDTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/saveHtmlEBAtables.py` & `arelle-release-2.9.0/arelle/plugin/saveHtmlEBAtables.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/saveLoadableExcel.py` & `arelle-release-2.9.0/arelle/plugin/saveLoadableExcel.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/saveLoadableOIM.py` & `arelle-release-2.9.0/arelle/plugin/saveLoadableOIM.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/saveSKOS.py` & `arelle-release-2.9.0/arelle/plugin/saveSKOS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/saveSampleInstance.py` & `arelle-release-2.9.0/arelle/plugin/saveSampleInstance.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/security/cryptAES_CBC.py` & `arelle-release-2.9.0/arelle/plugin/security/cryptAES_CBC.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/security/cryptAES_EAX.py` & `arelle-release-2.9.0/arelle/plugin/security/cryptAES_EAX.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/sphinx/FormulaGenerator.py` & `arelle-release-2.9.0/arelle/plugin/sphinx/FormulaGenerator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/sphinx/SphinxContext.py` & `arelle-release-2.9.0/arelle/plugin/sphinx/SphinxContext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/sphinx/SphinxEvaluator.py` & `arelle-release-2.9.0/arelle/plugin/sphinx/SphinxEvaluator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/sphinx/SphinxMethods.py` & `arelle-release-2.9.0/arelle/plugin/sphinx/SphinxMethods.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/sphinx/SphinxParser.py` & `arelle-release-2.9.0/arelle/plugin/sphinx/SphinxParser.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/sphinx/SphinxValidator.py` & `arelle-release-2.9.0/arelle/plugin/sphinx/SphinxValidator.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr` & `arelle-release-2.9.0/arelle/plugin/sphinx/US-GAAP Ratios Example.xsr`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/sphinx/__init__.py` & `arelle-release-2.9.0/arelle/plugin/sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/streamingExtensions.py` & `arelle-release-2.9.0/arelle/plugin/streamingExtensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/__init__.py` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/README.md` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/extractTestcase.xsl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/runIxtSecTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/saxon9.jar` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/saxon9.jar`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/testcase.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/testcase.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/conf/tests.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/conf/tests.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/text2num.py` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/text2num.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-boolballotbox.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-countrynameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-datequarterend.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durday.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durhour.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durmonth.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durweek.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-durwordsen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-duryear.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-edgarprovcountryen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-entityfilercategoryen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-exchnameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-numwordsen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-stateprovnameen.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/ixt-sec-yesnoballotbox.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/registry/transform-registry.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd` & `arelle-release-2.9.0/arelle/plugin/transforms/SEC/transformationRegistry/schema/inlinexbrl-sec-transformation.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/transforms/tester.py` & `arelle-release-2.9.0/arelle/plugin/transforms/tester.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/unpackSecEisFile.py` & `arelle-release-2.9.0/arelle/plugin/unpackSecEisFile.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/CIPC/Const.py` & `arelle-release-2.9.0/arelle/plugin/validate/CIPC/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/CIPC/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/CIPC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/CIPC/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/CIPC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EBA/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/EBA/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EBA/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EBA/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/Consts.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/Consts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/DTS.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/Dimensions.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/Document.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/Document.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/Filing.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/Filing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/PreCalAlignment.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/PreCalAlignment.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/Util.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/Util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/README.md` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/axiswarnings.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/axiswarnings.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/dei-validations.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/dei-validations.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/dqc-us-rules.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/dqc-us-rules.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-16-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-0-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-17-3-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-18.3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-19-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-20-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2012.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2013.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2014.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2015.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-2016.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-3.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-21-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1-preview.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-2.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-22-4.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1-1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-23-1.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/edgartaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/erxl.xsd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/extendedtaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrs-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/edgartaxonomies/ifrstaxonomies-all-years.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/exch-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/ifrs-full-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/invest-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/ixbrl-transform-registries.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/naics-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/rr-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/signwarnings.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/signwarnings.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/taxonomy-compatibility.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-deprecated-concepts.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2020.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2021.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2022.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/resources/us-gaap-rels-2023.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM/tools/CheckTxmyRefs.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM/tools/CheckTxmyRefs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/Const.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd` & `arelle-release-2.9.0/arelle/plugin/validate/EFM-htm/resources/efm-htm.dtd`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF/Const.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF/DTS.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF/Dimensions.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF/Util.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF/Util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF/resources/authority-validations.json` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF/resources/authority-validations.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/Const.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/Const.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/DTS.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/Dimensions.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/Util.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/Util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json` & `arelle-release-2.9.0/arelle/plugin/validate/ESEF_2022/resources/authority-validations.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/FERC/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/FERC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/FERC/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/FERC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/FERC/resources/ferc-utr.xml` & `arelle-release-2.9.0/arelle/plugin/validate/FERC/resources/ferc-utr.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/GFM/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/GFM/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/GFM/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/GFM/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/HMRC/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/HMRC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/HMRC/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/HMRC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/HMRC/consistencyChecksByName.json` & `arelle-release-2.9.0/arelle/plugin/validate/HMRC/consistencyChecksByName.json`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml` & `arelle-release-2.9.0/arelle/plugin/validate/HMRC/hmrc-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ROS/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/ROS/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/ROS/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/ROS/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/SBRnl/CustomLoader.py` & `arelle-release-2.9.0/arelle/plugin/validate/SBRnl/CustomLoader.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/SBRnl/DTS.py` & `arelle-release-2.9.0/arelle/plugin/validate/SBRnl/DTS.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/SBRnl/Dimensions.py` & `arelle-release-2.9.0/arelle/plugin/validate/SBRnl/Dimensions.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/SBRnl/Document.py` & `arelle-release-2.9.0/arelle/plugin/validate/SBRnl/Document.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/SBRnl/Filing.py` & `arelle-release-2.9.0/arelle/plugin/validate/SBRnl/Filing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/SBRnl/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/SBRnl/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/SBRnl/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/SBRnl/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml` & `arelle-release-2.9.0/arelle/plugin/validate/SBRnl/sbr-nl-taxonomies.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/USBestPractices.py` & `arelle-release-2.9.0/arelle/plugin/validate/USBestPractices.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/USCorpAction.py` & `arelle-release-2.9.0/arelle/plugin/validate/USCorpAction.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/USSecTagging.py` & `arelle-release-2.9.0/arelle/plugin/validate/USSecTagging.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/XDC/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/XDC/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/XDC/config.xml` & `arelle-release-2.9.0/arelle/plugin/validate/XDC/config.xml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/XFsyntax/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/XFsyntax/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/XFsyntax/xf.py` & `arelle-release-2.9.0/arelle/plugin/validate/XFsyntax/xf.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/__init__.py` & `arelle-release-2.9.0/arelle/plugin/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validate/calc2.py` & `arelle-release-2.9.0/arelle/plugin/validate/calc2.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/validateSBRnl.py` & `arelle-release-2.9.0/arelle/plugin/validateSBRnl.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/DialogRssWatchExtender.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/DialogRssWatchExtender.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/SqlDb.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/SqlDb.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlDpmSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlOpenSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlPublicPostgresDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlSemanticGraphDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlSemanticJsonDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlSemanticRdfDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/XbrlSemanticSqlDB.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/__init__.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/__init__.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/entityInformation.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/entityInformation.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/ext/china.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/ext/china.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/ext/edgar.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/ext/edgar.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/ext/xdc.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/ext/xdc.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/primaryDocumentFacts.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/primaryDocumentFacts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/ext/chinaPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/ext/edgarPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/ext/xdcPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open/xbrlOpenPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/open2/xbrlOpen2PostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/public/xbrlPublicPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/secDatabaseModelViews.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticColumnComments.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMSSqlDB.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticMySqlDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticOracleDB.sql`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticPostgresDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/sql/semantic/xbrlSemanticSQLiteDB.ddl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xbrlDB/tableFacts.py` & `arelle-release-2.9.0/arelle/plugin/xbrlDB/tableFacts.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/plugin/xuleSaver.py` & `arelle-release-2.9.0/arelle/plugin/xuleSaver.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/scripts-windows/exportCsvFromXbrlInstance.bat` & `arelle-release-2.9.0/arelle/scripts-windows/exportCsvFromXbrlInstance.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/scripts-windows/runFormulaTests.bat` & `arelle-release-2.9.0/arelle/scripts-windows/runFormulaTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/scripts-windows/validateAndRunFormulas.bat` & `arelle-release-2.9.0/arelle/scripts-windows/validateAndRunFormulas.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/typing.py` & `arelle-release-2.9.0/arelle/typing.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/webserver/bottle-no2to3.py` & `arelle-release-2.9.0/arelle/webserver/bottle-no2to3.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle/webserver/bottle.py` & `arelle-release-2.9.0/arelle/webserver/bottle.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelleCmdLine.py` & `arelle-release-2.9.0/arelleCmdLine.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle_release.egg-info/PKG-INFO` & `arelle-release-2.9.0/arelle_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arelle-release
-Version: 2.8.1
+Version: 2.9.0
 Summary: An open source XBRL platform.
 Author-email: "arelle.org" <support@arelle.org>
 License: Apache-2.0
 Project-URL: Homepage, https://arelle.org/
 Project-URL: Downloads, https://arelle.org/arelle/pub/
 Project-URL: Documentation, https://arelle.org/arelle/documentation/
 Project-URL: Blog, https://arelle.org/arelle/blog/
```

### Comparing `arelle-release-2.8.1/arelle_release.egg-info/SOURCES.txt` & `arelle-release-2.9.0/arelle_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/arelle_test.py` & `arelle-release-2.9.0/arelle_test.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/attic/CntlrGenVersReports.py` & `arelle-release-2.9.0/attic/CntlrGenVersReports.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/buildVersion.py` & `arelle-release-2.9.0/buildVersion.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/conftest.py` & `arelle-release-2.9.0/conftest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/distro.py` & `arelle-release-2.9.0/distro.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/docker/ubuntu.Dockerfile` & `arelle-release-2.9.0/docker/ubuntu.Dockerfile`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/encodeUtf8PySource.py` & `arelle-release-2.9.0/encodeUtf8PySource.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/generateMessagesCatalog.py` & `arelle-release-2.9.0/generateMessagesCatalog.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/installWin64.nsi` & `arelle-release-2.9.0/installWin64.nsi`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/installWin86.nsi` & `arelle-release-2.9.0/installWin86.nsi`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/linux/Tktable2.11/README.txt` & `arelle-release-2.9.0/libs/linux/Tktable2.11/README.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/linux/Tktable2.11/html/tkTable.html` & `arelle-release-2.9.0/libs/linux/Tktable2.11/html/tkTable.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/linux/Tktable2.11/libTktable2.11.so` & `arelle-release-2.9.0/libs/linux/Tktable2.11/libTktable2.11.so`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/linux/Tktable2.11/license.txt` & `arelle-release-2.9.0/libs/linux/Tktable2.11/license.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/linux/Tktable2.11/tkTable.tcl` & `arelle-release-2.9.0/libs/linux/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/linux/Tktable2.11/tktable.py` & `arelle-release-2.9.0/libs/linux/Tktable2.11/tktable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/macos/Tktable2.11/README.txt` & `arelle-release-2.9.0/libs/macos/Tktable2.11/README.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/macos/Tktable2.11/html/tkTable.html` & `arelle-release-2.9.0/libs/macos/Tktable2.11/html/tkTable.html`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/macos/Tktable2.11/libTktable2.11.dylib` & `arelle-release-2.9.0/libs/macos/Tktable2.11/libTktable2.11.dylib`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/macos/Tktable2.11/license.txt` & `arelle-release-2.9.0/libs/macos/Tktable2.11/license.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/macos/Tktable2.11/tkTable.tcl` & `arelle-release-2.9.0/libs/macos/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/macos/Tktable2.11/tktable.py` & `arelle-release-2.9.0/libs/macos/Tktable2.11/tktable.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/win64/Tktable2.11/Tktable.dll` & `arelle-release-2.9.0/libs/win64/Tktable2.11/Tktable.dll`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/libs/win64/Tktable2.11/tkTable.tcl` & `arelle-release-2.9.0/libs/win64/Tktable2.11/tkTable.tcl`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/messages.pot` & `arelle-release-2.9.0/messages.pot`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/msgfmt.py` & `arelle-release-2.9.0/msgfmt.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/plugins/xbrl-us/us-gaap-consistency.py` & `arelle-release-2.9.0/plugins/xbrl-us/us-gaap-consistency.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/pygettext.py` & `arelle-release-2.9.0/pygettext.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/pyproject.toml` & `arelle-release-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/requirements.txt` & `arelle-release-2.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/buildLinuxDist.sh` & `arelle-release-2.9.0/scripts/buildLinuxDist.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/buildMacDist.sh` & `arelle-release-2.9.0/scripts/buildMacDist.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/buildWinDist.bat` & `arelle-release-2.9.0/scripts/buildWinDist.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/charlieTest.bat` & `arelle-release-2.9.0/scripts/charlieTest.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/exportCsvFormulae.bat` & `arelle-release-2.9.0/scripts/exportCsvFormulae.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/exportCsvFromXbrlInstance.bat` & `arelle-release-2.9.0/scripts/exportCsvFromXbrlInstance.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/generateTestcase.py` & `arelle-release-2.9.0/scripts/generateTestcase.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/reportAllTests.bat` & `arelle-release-2.9.0/scripts/reportAllTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runESMAtests.sh` & `arelle-release-2.9.0/scripts/runESMAtests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runGenerateVersioningTestcases.bat` & `arelle-release-2.9.0/scripts/runGenerateVersioningTestcases.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runPackageTests.sh` & `arelle-release-2.9.0/scripts/runPackageTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runPyTest.sh` & `arelle-release-2.9.0/scripts/runPyTest.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runTR2Tests.sh` & `arelle-release-2.9.0/scripts/runTR2Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runTR3Tests.sh` & `arelle-release-2.9.0/scripts/runTR3Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runTR4Tests.sh` & `arelle-release-2.9.0/scripts/runTR4Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runTR5Tests.sh` & `arelle-release-2.9.0/scripts/runTR5Tests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runTRSECTests.sh` & `arelle-release-2.9.0/scripts/runTRSECTests.sh`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/scripts/runVersioningConsumptionTests.bat` & `arelle-release-2.9.0/scripts/runVersioningConsumptionTests.bat`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/setup.cfg` & `arelle-release-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj` & `arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/ArelleGUITest.csproj`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs` & `arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest/Tests.cs`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln` & `arelle-release-2.9.0/tests/integration_tests/ui_tests/ArelleGUITest/ArelleGUITest.sln`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/ui_tests/resources/workiva.zip` & `arelle-release-2.9.0/tests/integration_tests/ui_tests/resources/workiva.zip`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/README.md` & `arelle-release-2.9.0/tests/integration_tests/validation/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_config.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_config.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configs.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configs.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/efm_current.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2021.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/esef_ixbrl_2022.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2021.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/esef_xhtml_2022.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_2_1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_dimensions_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_extensible_enumerations_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_formula_1_0_function_registry.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_ixbrl_1_1.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_oim_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_table_linkbase_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_malformed_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_registry_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conformance_suite_configurations/xbrl_utr_structure_1_0.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/conftest.py` & `arelle-release-2.9.0/tests/integration_tests/validation/conftest.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/download_conformance_suites.py` & `arelle-release-2.9.0/tests/integration_tests/validation/download_conformance_suites.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/run_conformance_suites.py` & `arelle-release-2.9.0/tests/integration_tests/validation/run_conformance_suites.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/test_conformance_suites.py` & `arelle-release-2.9.0/tests/integration_tests/validation/test_conformance_suites.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/integration_tests/validation/validation_util.py` & `arelle-release-2.9.0/tests/integration_tests/validation/validation_util.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/formula/test_fact_aspects_cache.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/plugin/test_loadfromoim.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/plugin/test_loadfromoim.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_cntlr.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_cntlr.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_import.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_import.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_locale.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_locale.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_packagemanager.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_packagemanager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_pluginmanager.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_pluginmanager.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_qname.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_qname.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_system_info.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_system_info.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_updater.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_updater.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_urlutil.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_urlutil.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/tests/unit_tests/arelle/test_version.py` & `arelle-release-2.9.0/tests/unit_tests/arelle/test_version.py`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/vms/mac/README.md` & `arelle-release-2.9.0/vms/mac/README.md`

 * *Files identical despite different names*

### Comparing `arelle-release-2.8.1/vms/mac/create-macos-bootable-for-virtualbox.sh` & `arelle-release-2.9.0/vms/mac/create-macos-bootable-for-virtualbox.sh`

 * *Files identical despite different names*

