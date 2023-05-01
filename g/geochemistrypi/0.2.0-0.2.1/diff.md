# Comparing `tmp/geochemistrypi-0.2.0.tar.gz` & `tmp/geochemistrypi-0.2.1.tar.gz`

## Comparing `geochemistrypi-0.2.0.tar` & `geochemistrypi-0.2.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/requirements.txt
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/.github/workflows/geochemistrypy.yml
--rw-r--r--   0        0        0   285992 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/docs/Geochemistry π.png
--rw-r--r--   0        0        0   255925 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/docs/Geochemistryπ-Activity Diagram_v1.png
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/__init__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/cli.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/main.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/UI.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/__init__.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/global_variable.py
--rw-r--r--   0        0        0    15242 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/pipeline.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/__init__.py
--rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/data_readiness.py
--rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/feature_engineering.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/imputation.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/preprocessing.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/statistic.py
--rw-r--r--   0        0        0   225291 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx
--rw-r--r--   0        0        0   225363 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx
--rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx
--rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/__init__.py
--rw-r--r--   0        0        0    10732 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/_base.py
--rw-r--r--   0        0        0   106659 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/classification.py
--rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/clustering.py
--rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/decomposition.py
--rw-r--r--   0        0        0    94512 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/regression.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/__init__.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_deep_neural_network.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_rf.py
--rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_svm.py
--rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_common.py
--rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py
--rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_decomposition/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_decomposition/_common.py
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/__init__.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_deep_neural_network.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_rf.py
--rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_svr.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/__init__.py
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/geochemistry_plot.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/map_plot.py
--rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/statistic_plot.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/__init__.py
--rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/classify.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/cluster.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/decompose.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/process/regress.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/tests/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/tests/test_data/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/utils/__init__.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/utils/base.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/geochemistrypi/data_mining/utils/exceptions.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/LICENSE
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/README.md
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 geochemistrypi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/requirements.txt
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/.github/workflows/geochemistrypy.yml
+-rw-r--r--   0        0        0   285992 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/docs/Geochemistry π.png
+-rw-r--r--   0        0        0   255925 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/docs/Geochemistryπ-Activity Diagram_v1.png
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/__init__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/cli.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/main.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/UI.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/__init__.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/global_variable.py
+-rw-r--r--   0        0        0    15241 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/pipeline.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/__init__.py
+-rw-r--r--   0        0        0    12027 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/data_readiness.py
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/feature_engineering.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/imputation.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/preprocessing.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/statistic.py
+-rw-r--r--   0        0        0   225291 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx
+-rw-r--r--   0        0        0   225363 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx
+-rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx
+-rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/__init__.py
+-rw-r--r--   0        0        0    10732 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/_base.py
+-rw-r--r--   0        0        0   106659 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/classification.py
+-rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/clustering.py
+-rw-r--r--   0        0        0    11942 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/decomposition.py
+-rw-r--r--   0        0        0    94512 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/regression.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/__init__.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_common.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_deep_neural_network.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_rf.py
+-rw-r--r--   0        0        0     6967 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_svm.py
+-rw-r--r--   0        0        0     8499 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_clustering/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_clustering/_common.py
+-rw-r--r--   0        0        0     5818 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py
+-rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_decomposition/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_decomposition/_common.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/__init__.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_common.py
+-rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_deep_neural_network.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_rf.py
+-rw-r--r--   0        0        0     6807 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_svr.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/plot/__init__.py
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/plot/geochemistry_plot.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/plot/map_plot.py
+-rw-r--r--   0        0        0     4354 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/plot/statistic_plot.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/process/__init__.py
+-rw-r--r--   0        0        0     8069 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/process/classify.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/process/cluster.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/process/decompose.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/process/regress.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/tests/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/utils/__init__.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/utils/base.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/geochemistrypi/data_mining/utils/exceptions.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/LICENSE
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/README.md
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12548 2020-02-02 00:00:00.000000 geochemistrypi-0.2.1/PKG-INFO
```

### Comparing `geochemistrypi-0.2.0/.github/workflows/geochemistrypy.yml` & `geochemistrypi-0.2.1/.github/workflows/geochemistrypy.yml`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/docs/Geochemistry π.png` & `geochemistrypi-0.2.1/docs/Geochemistry π.png`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/docs/Geochemistryπ-Activity Diagram_v1.png` & `geochemistrypi-0.2.1/docs/Geochemistryπ-Activity Diagram_v1.png`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/cli.py` & `geochemistrypi-0.2.1/geochemistrypi/cli.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/UI.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/UI.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tkinter import Label, Text, Button, Tk, INSERT
+from tkinter import *
 from tkinter import filedialog
 
 class Geochemistrypi_GUI():
     def __init__(self,root):
         self.root = root
         self.name = None
 
@@ -46,11 +46,8 @@
     # Instantiate a parent window
     init_window = Tk()
     data_gui = Geochemistrypi_GUI(init_window)
     # Set the default properties of the root window
     data_gui.set_init_window()
     # Keep window running
     init_window.mainloop()
-    return data_gui.name
-
-if __name__ == '__main__':
-    file_path = gui_data_input()
+    return data_gui.name
```

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/global_variable.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/global_variable.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/pipeline.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 os.makedirs(DATASET_OUTPUT_PATH, exist_ok=True)
 os.makedirs(MAP_IMAGE_PATH, exist_ok=True)
 os.makedirs(GEO_IMAGE_PATH, exist_ok=True)
 os.makedirs(MODEL_PATH, exist_ok=True)
 
 
 def pipeline(file_name: str) -> None:
-    print("Geochemistry Py v.1.0.0 - Beta Version")
+    print("Geochemistry Py v0.2.1 - Beta Version")
     print("....... Initializing .......")
     logger = log(OUTPUT_PATH, "inner_test.log")
     logger.info("Geochemistry Py v.1.0.0 - beta version")
 
     # If the argument is False, hide all Python level warnings.
     show_warning(False)
```

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/data_readiness.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/data_readiness.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/feature_engineering.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/imputation.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/imputation.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/preprocessing.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/statistic.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/statistic.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/_base.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/_base.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/classification.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/classification.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/clustering.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/clustering.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/decomposition.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/decomposition.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/regression.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_common.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_deep_neural_network.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_deep_neural_network.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_rf.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_rf.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_svm.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_svm.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_common.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_deep_neural_network.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_deep_neural_network.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_rf.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_rf.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_svr.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_svr.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/geochemistry_plot.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/plot/geochemistry_plot.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/plot/statistic_plot.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/plot/statistic_plot.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/process/classify.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/process/classify.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/process/cluster.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/process/cluster.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/process/decompose.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/process/decompose.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/process/regress.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/process/regress.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/geochemistrypi/data_mining/utils/base.py` & `geochemistrypi-0.2.1/geochemistrypi/data_mining/utils/base.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/LICENSE` & `geochemistrypi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.2.0/README.md` & `geochemistrypi-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 
 One instruction to download on command line, such as Terminal on macOS, CMD on Windows.  
 ```
 pip install geochemistrypi
 ```
 **Note**: The beta version runs on MacOS, Windows or Linux.
 
+## Quick Update
+One instruction to update the software to the latest version on command line, such as Terminal on macOS, CMD on Windows. 
+```
+pip install --upgrade geochemistrypi
+```
+
 ## Example
 
 **How to run:** After successfully downloading, run this instruction on command line whatever directory it is.
 
 ### Case 1: Run with built-in data set for testing
 ```
 geochemistrypi data-mining
```

### Comparing `geochemistrypi-0.2.0/pyproject.toml` & `geochemistrypi-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geochemistrypi"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Can He", email="sanyhew1097618435@163.com" },
 ]
 maintainers = [] 
 description = "A Python framework for data-driven geochemistry discovery"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -29,19 +29,17 @@
     "multipledispatch==0.6.0",
     "statsmodels==0.13.2",
     "scipy",
     "openpyxl==3.0.10",
     "pandas==1.5.2",
     "joblib==1.2.0",
     "flaml==1.0.14",         # required to run Xgboost + FLMAL
-    "numpy==1.21.6",         # required to run Xgboost + FLMAL
+    "numpy==1.23.5",         # required to run Xgboost + FLMAL
     "xgboost==1.6.2",        # required to run Xgboost + FLAML and be compatible with M2 chip on Mac
-    "pyogrio==0.4.2",        # required to draw world map
-    "geopandas==0.10.2",     # required to draw world map
-    "Fiona==1.8.19",         # required to draw world map
+    "basemap==1.3.6",        # required to draw world map
     "threadpoolctl==3.1.0",  # required to draw 3d plot for KMeans
     "matplotlib==3.5.2"      # required to draw 3d plot for KMeans
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest"
```

### Comparing `geochemistrypi-0.2.0/PKG-INFO` & `geochemistrypi-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geochemistrypi
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python framework for data-driven geochemistry discovery
 Project-URL: Homepage, https://github.com/ZJUEarthData/geochemistrypi
 Project-URL: Bug Tracker, https://github.com/ZJUEarthData/geochemistrypi/issues
 Author-email: Can He <sanyhew1097618435@163.com>
 License: MIT License
         
         Copyright (c) 2021 ZJUEarthData
@@ -27,25 +27,23 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: ~=3.9
-Requires-Dist: fiona==1.8.19
+Requires-Dist: basemap==1.3.6
 Requires-Dist: flaml==1.0.14
-Requires-Dist: geopandas==0.10.2
 Requires-Dist: joblib==1.2.0
 Requires-Dist: matplotlib==3.5.2
 Requires-Dist: multipledispatch==0.6.0
-Requires-Dist: numpy==1.21.6
+Requires-Dist: numpy==1.23.5
 Requires-Dist: openpyxl==3.0.10
 Requires-Dist: optuna
 Requires-Dist: pandas==1.5.2
-Requires-Dist: pyogrio==0.4.2
 Requires-Dist: ray==2.2.0
 Requires-Dist: ray[tune]
 Requires-Dist: scikit-learn==1.1.3
 Requires-Dist: scipy
 Requires-Dist: seaborn==0.11.0
 Requires-Dist: statsmodels==0.13.2
 Requires-Dist: threadpoolctl==3.1.0
@@ -82,14 +80,20 @@
 
 One instruction to download on command line, such as Terminal on macOS, CMD on Windows.  
 ```
 pip install geochemistrypi
 ```
 **Note**: The beta version runs on MacOS, Windows or Linux.
 
+## Quick Update
+One instruction to update the software to the latest version on command line, such as Terminal on macOS, CMD on Windows. 
+```
+pip install --upgrade geochemistrypi
+```
+
 ## Example
 
 **How to run:** After successfully downloading, run this instruction on command line whatever directory it is.
 
 ### Case 1: Run with built-in data set for testing
 ```
 geochemistrypi data-mining
```

