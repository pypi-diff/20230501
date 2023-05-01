# Comparing `tmp/NlpToolkit-Classification-1.0.8.tar.gz` & `tmp/NlpToolkit-Classification-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NlpToolkit-Classification-1.0.8.tar", last modified: Sun Apr 25 14:50:08 2021, max compression
+gzip compressed data, was "dist/NlpToolkit-Classification-1.0.9.tar", last modified: Sun Apr 25 15:05:43 2021, max compression
```

## Comparing `NlpToolkit-Classification-1.0.8.tar` & `NlpToolkit-Classification-1.0.9.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Attribute/
--rw-r--r--   0 olcay      (501) staff       (20)      274 2020-02-07 20:20:40.000000 NlpToolkit-Classification-1.0.8/Classification/Attribute/Attribute.py
--rw-r--r--   0 olcay      (501) staff       (20)      348 2020-02-07 20:20:40.000000 NlpToolkit-Classification-1.0.8/Classification/Attribute/AttributeType.py
--rw-r--r--   0 olcay      (501) staff       (20)      449 2020-02-17 19:08:09.000000 NlpToolkit-Classification-1.0.8/Classification/Attribute/BinaryAttribute.py
--rw-r--r--   0 olcay      (501) staff       (20)     1143 2020-02-17 19:08:08.000000 NlpToolkit-Classification-1.0.8/Classification/Attribute/ContinuousAttribute.py
--rw-r--r--   0 olcay      (501) staff       (20)      918 2020-02-17 19:08:09.000000 NlpToolkit-Classification-1.0.8/Classification/Attribute/DiscreteAttribute.py
--rw-r--r--   0 olcay      (501) staff       (20)     1318 2020-02-17 19:08:08.000000 NlpToolkit-Classification-1.0.8/Classification/Attribute/DiscreteIndexedAttribute.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-09-28 15:01:19.000000 NlpToolkit-Classification-1.0.8/Classification/Attribute/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/
--rw-r--r--   0 olcay      (501) staff       (20)     1543 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/AutoEncoder.py
--rw-r--r--   0 olcay      (501) staff       (20)     1682 2020-06-28 11:00:00.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/Bagging.py
--rw-r--r--   0 olcay      (501) staff       (20)     1245 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/C45.py
--rw-r--r--   0 olcay      (501) staff       (20)      805 2020-02-17 19:08:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/C45Stump.py
--rw-r--r--   0 olcay      (501) staff       (20)     3258 2020-06-26 06:32:49.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/Classifier.py
--rw-r--r--   0 olcay      (501) staff       (20)      988 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/DeepNetwork.py
--rw-r--r--   0 olcay      (501) staff       (20)      763 2020-02-17 19:08:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/Dummy.py
--rw-r--r--   0 olcay      (501) staff       (20)      744 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/KMeans.py
--rw-r--r--   0 olcay      (501) staff       (20)      714 2020-02-17 19:08:09.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/Knn.py
--rw-r--r--   0 olcay      (501) staff       (20)     1924 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/Lda.py
--rw-r--r--   0 olcay      (501) staff       (20)     1179 2020-06-28 09:58:04.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/LinearPerceptron.py
--rw-r--r--   0 olcay      (501) staff       (20)     1223 2020-06-27 07:14:22.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/MultiLayerPerceptron.py
--rw-r--r--   0 olcay      (501) staff       (20)     3178 2020-06-27 07:14:48.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/NaiveBayes.py
--rw-r--r--   0 olcay      (501) staff       (20)     1733 2020-06-27 07:16:38.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/Qda.py
--rw-r--r--   0 olcay      (501) staff       (20)      640 2020-06-26 05:44:41.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/RandomClassifier.py
--rw-r--r--   0 olcay      (501) staff       (20)     1357 2020-06-26 06:04:47.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/RandomForest.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-13 14:20:08.000000 NlpToolkit-Classification-1.0.8/Classification/Classifier/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/DataSet/
--rw-r--r--   0 olcay      (501) staff       (20)     3601 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/DataSet/DataDefinition.py
--rw-r--r--   0 olcay      (501) staff       (20)    11818 2020-06-28 06:29:49.000000 NlpToolkit-Classification-1.0.8/Classification/DataSet/DataSet.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-09 11:07:38.000000 NlpToolkit-Classification-1.0.8/Classification/DataSet/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/DistanceMetric/
--rw-r--r--   0 olcay      (501) staff       (20)      227 2020-02-07 20:32:13.000000 NlpToolkit-Classification-1.0.8/Classification/DistanceMetric/DistanceMetric.py
--rw-r--r--   0 olcay      (501) staff       (20)     1168 2020-02-07 20:32:13.000000 NlpToolkit-Classification-1.0.8/Classification/DistanceMetric/EuclidianDistance.py
--rw-r--r--   0 olcay      (501) staff       (20)     1243 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/DistanceMetric/MahalanobisDistance.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-15 11:26:35.000000 NlpToolkit-Classification-1.0.8/Classification/DistanceMetric/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/
--rw-r--r--   0 olcay      (501) staff       (20)     1611 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/BootstrapRun.py
--rw-r--r--   0 olcay      (501) staff       (20)     2150 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/Experiment.py
--rw-r--r--   0 olcay      (501) staff       (20)     2062 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/KFoldRun.py
--rw-r--r--   0 olcay      (501) staff       (20)     2317 2020-06-27 07:10:01.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/KFoldRunSeparateTest.py
--rw-r--r--   0 olcay      (501) staff       (20)      309 2019-10-14 06:35:36.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/MultipleRun.py
--rw-r--r--   0 olcay      (501) staff       (20)     1532 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/MxKFoldRun.py
--rw-r--r--   0 olcay      (501) staff       (20)     1882 2020-06-27 07:10:01.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/MxKFoldRunSeparateTest.py
--rw-r--r--   0 olcay      (501) staff       (20)      277 2019-10-14 06:34:35.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/SingleRun.py
--rw-r--r--   0 olcay      (501) staff       (20)     1812 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/SingleRunWithK.py
--rw-r--r--   0 olcay      (501) staff       (20)     1427 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedKFoldRun.py
--rw-r--r--   0 olcay      (501) staff       (20)     1755 2020-06-27 07:10:01.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedKFoldRunSeparateTest.py
--rw-r--r--   0 olcay      (501) staff       (20)     1608 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedMxKFoldRun.py
--rw-r--r--   0 olcay      (501) staff       (20)     1610 2020-06-27 07:10:01.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedMxKFoldRunSeparateTest.py
--rw-r--r--   0 olcay      (501) staff       (20)     1470 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedSingleRunWithK.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-14 06:25:46.000000 NlpToolkit-Classification-1.0.8/Classification/Experiment/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/
--rw-r--r--   0 olcay      (501) staff       (20)     1206 2020-06-29 11:22:20.000000 NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/BackwardSelection.py
--rw-r--r--   0 olcay      (501) staff       (20)     2179 2020-06-29 11:28:55.000000 NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/FeatureSubSet.py
--rw-r--r--   0 olcay      (501) staff       (20)      914 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/FloatingSelection.py
--rw-r--r--   0 olcay      (501) staff       (20)     1048 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/ForwardSelection.py
--rw-r--r--   0 olcay      (501) staff       (20)     3759 2020-06-29 11:11:17.000000 NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/SubSetSelection.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-14 12:39:08.000000 NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/
--rw-r--r--   0 olcay      (501) staff       (20)     2477 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/DiscreteToContinuous.py
--rw-r--r--   0 olcay      (501) staff       (20)     1373 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/DiscreteToIndexed.py
--rw-r--r--   0 olcay      (501) staff       (20)      958 2020-10-15 08:47:08.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/FeatureFilter.py
--rw-r--r--   0 olcay      (501) staff       (20)     1813 2020-10-15 08:47:08.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/LaryFilter.py
--rw-r--r--   0 olcay      (501) staff       (20)     2370 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/LaryToBinary.py
--rw-r--r--   0 olcay      (501) staff       (20)     1687 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/Normalize.py
--rw-r--r--   0 olcay      (501) staff       (20)     4147 2020-06-29 10:53:23.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/Pca.py
--rw-r--r--   0 olcay      (501) staff       (20)      493 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/TrainedFeatureFilter.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-15 11:50:54.000000 NlpToolkit-Classification-1.0.8/Classification/Filter/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Instance/
--rw-r--r--   0 olcay      (501) staff       (20)     1875 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Instance/CompositeInstance.py
--rw-r--r--   0 olcay      (501) staff       (20)     6162 2020-06-28 09:21:59.000000 NlpToolkit-Classification-1.0.8/Classification/Instance/Instance.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-05 11:13:05.000000 NlpToolkit-Classification-1.0.8/Classification/Instance/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/InstanceList/
--rw-r--r--   0 olcay      (501) staff       (20)    20477 2020-06-29 10:40:36.000000 NlpToolkit-Classification-1.0.8/Classification/InstanceList/InstanceList.py
--rw-r--r--   0 olcay      (501) staff       (20)      658 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/InstanceList/InstanceListOfSameClass.py
--rw-r--r--   0 olcay      (501) staff       (20)     5595 2020-06-28 07:19:06.000000 NlpToolkit-Classification-1.0.8/Classification/InstanceList/Partition.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-09 11:07:49.000000 NlpToolkit-Classification-1.0.8/Classification/InstanceList/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Model/
--rw-r--r--   0 olcay      (501) staff       (20)     5467 2020-06-26 05:58:28.000000 NlpToolkit-Classification-1.0.8/Classification/Model/AutoEncoderModel.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Model/DecisionTree/
--rw-r--r--   0 olcay      (501) staff       (20)     2780 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Model/DecisionTree/DecisionCondition.py
--rw-r--r--   0 olcay      (501) staff       (20)    13496 2021-04-25 14:40:46.000000 NlpToolkit-Classification-1.0.8/Classification/Model/DecisionTree/DecisionNode.py
--rw-r--r--   0 olcay      (501) staff       (20)     2767 2021-04-25 14:42:08.000000 NlpToolkit-Classification-1.0.8/Classification/Model/DecisionTree/DecisionTree.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-19 05:25:07.000000 NlpToolkit-Classification-1.0.8/Classification/Model/DecisionTree/__init__.py
--rw-r--r--   0 olcay      (501) staff       (20)     6560 2020-06-26 05:59:57.000000 NlpToolkit-Classification-1.0.8/Classification/Model/DeepNetworkModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     1533 2021-04-25 14:43:24.000000 NlpToolkit-Classification-1.0.8/Classification/Model/DummyModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     1855 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Model/GaussianModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     2049 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Model/KMeansModel.py
--rw-r--r--   0 olcay      (501) staff       (20)      864 2020-10-15 07:52:20.000000 NlpToolkit-Classification-1.0.8/Classification/Model/KnnInstance.py
--rw-r--r--   0 olcay      (501) staff       (20)     3951 2021-04-25 14:45:05.000000 NlpToolkit-Classification-1.0.8/Classification/Model/KnnModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     1378 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Model/LdaModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     2720 2020-06-26 06:01:52.000000 NlpToolkit-Classification-1.0.8/Classification/Model/LinearPerceptronModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     1190 2021-04-25 14:45:05.000000 NlpToolkit-Classification-1.0.8/Classification/Model/Model.py
--rw-r--r--   0 olcay      (501) staff       (20)     3787 2020-06-28 10:30:21.000000 NlpToolkit-Classification-1.0.8/Classification/Model/MultiLayerPerceptronModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     4614 2020-06-28 09:48:43.000000 NlpToolkit-Classification-1.0.8/Classification/Model/NaiveBayesModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     7527 2021-04-25 14:46:41.000000 NlpToolkit-Classification-1.0.8/Classification/Model/NeuralNetworkModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     1747 2020-10-15 08:05:07.000000 NlpToolkit-Classification-1.0.8/Classification/Model/QdaModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     1709 2021-04-25 14:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Model/RandomModel.py
--rw-r--r--   0 olcay      (501) staff       (20)     1407 2021-04-25 14:50:02.000000 NlpToolkit-Classification-1.0.8/Classification/Model/TreeEnsembleModel.py
--rw-r--r--   0 olcay      (501) staff       (20)      944 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.8/Classification/Model/ValidatedModel.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-13 14:20:16.000000 NlpToolkit-Classification-1.0.8/Classification/Model/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/
--rw-r--r--   0 olcay      (501) staff       (20)      725 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/BaggingParameter.py
--rw-r--r--   0 olcay      (501) staff       (20)     1128 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/C45Parameter.py
--rw-r--r--   0 olcay      (501) staff       (20)     1833 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/DeepNetworkParameter.py
--rw-r--r--   0 olcay      (501) staff       (20)      972 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/KMeansParameter.py
--rw-r--r--   0 olcay      (501) staff       (20)      900 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/KnnParameter.py
--rw-r--r--   0 olcay      (501) staff       (20)     1933 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/LinearPerceptronParameter.py
--rw-r--r--   0 olcay      (501) staff       (20)     1318 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/MultiLayerPerceptronParameter.py
--rw-r--r--   0 olcay      (501) staff       (20)      495 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/Parameter.py
--rw-r--r--   0 olcay      (501) staff       (20)      939 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/RandomForestParameter.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-09-28 16:37:42.000000 NlpToolkit-Classification-1.0.8/Classification/Parameter/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/Performance/
--rw-r--r--   0 olcay      (501) staff       (20)      813 2020-06-28 07:26:13.000000 NlpToolkit-Classification-1.0.8/Classification/Performance/ClassificationPerformance.py
--rw-r--r--   0 olcay      (501) staff       (20)     6571 2020-06-28 07:29:01.000000 NlpToolkit-Classification-1.0.8/Classification/Performance/ConfusionMatrix.py
--rw-r--r--   0 olcay      (501) staff       (20)      965 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Performance/DetailedClassificationPerformance.py
--rw-r--r--   0 olcay      (501) staff       (20)     7888 2020-06-29 13:55:41.000000 NlpToolkit-Classification-1.0.8/Classification/Performance/ExperimentPerformance.py
--rw-r--r--   0 olcay      (501) staff       (20)      494 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.8/Classification/Performance/Performance.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-09-30 18:15:40.000000 NlpToolkit-Classification-1.0.8/Classification/Performance/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/
--rw-r--r--   0 olcay      (501) staff       (20)     2167 2020-02-18 04:52:52.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Combined5x2F.py
--rw-r--r--   0 olcay      (501) staff       (20)     2123 2020-02-18 04:53:50.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Combined5x2t.py
--rw-r--r--   0 olcay      (501) staff       (20)     2048 2020-02-18 04:53:24.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Paired5x2t.py
--rw-r--r--   0 olcay      (501) staff       (20)     1086 2020-02-07 20:37:43.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/PairedTest.py
--rw-r--r--   0 olcay      (501) staff       (20)     1862 2020-06-29 13:55:58.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Pairedt.py
--rw-r--r--   0 olcay      (501) staff       (20)     1602 2020-02-18 04:54:27.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Sign.py
--rw-r--r--   0 olcay      (501) staff       (20)      119 2019-10-05 10:26:00.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/StatisticalTestNotApplicable.py
--rw-r--r--   0 olcay      (501) staff       (20)     1367 2020-02-07 20:37:43.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/StatisticalTestResult.py
--rw-r--r--   0 olcay      (501) staff       (20)      177 2019-10-05 07:12:24.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/StatisticalTestResultType.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-05 07:10:00.000000 NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/__init__.py
--rw-r--r--   0 olcay      (501) staff       (20)        0 2019-09-28 15:01:05.000000 NlpToolkit-Classification-1.0.8/Classification/__init__.py
-drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/NlpToolkit_Classification.egg-info/
--rw-r--r--   0 olcay      (501) staff       (20)      283 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/NlpToolkit_Classification.egg-info/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)     5335 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/NlpToolkit_Classification.egg-info/SOURCES.txt
--rw-r--r--   0 olcay      (501) staff       (20)        1 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/NlpToolkit_Classification.egg-info/dependency_links.txt
--rw-r--r--   0 olcay      (501) staff       (20)       61 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/NlpToolkit_Classification.egg-info/requires.txt
--rw-r--r--   0 olcay      (501) staff       (20)       15 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/NlpToolkit_Classification.egg-info/top_level.txt
--rw-r--r--   0 olcay      (501) staff       (20)      283 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/PKG-INFO
--rw-r--r--   0 olcay      (501) staff       (20)     8555 2021-04-24 15:49:39.000000 NlpToolkit-Classification-1.0.8/README.md
--rw-r--r--   0 olcay      (501) staff       (20)       38 2021-04-25 14:50:08.000000 NlpToolkit-Classification-1.0.8/setup.cfg
--rw-r--r--   0 olcay      (501) staff       (20)      891 2021-04-25 14:50:02.000000 NlpToolkit-Classification-1.0.8/setup.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Attribute/
+-rw-r--r--   0 olcay      (501) staff       (20)      274 2020-02-07 20:20:40.000000 NlpToolkit-Classification-1.0.9/Classification/Attribute/Attribute.py
+-rw-r--r--   0 olcay      (501) staff       (20)      348 2020-02-07 20:20:40.000000 NlpToolkit-Classification-1.0.9/Classification/Attribute/AttributeType.py
+-rw-r--r--   0 olcay      (501) staff       (20)      449 2020-02-17 19:08:09.000000 NlpToolkit-Classification-1.0.9/Classification/Attribute/BinaryAttribute.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1143 2020-02-17 19:08:08.000000 NlpToolkit-Classification-1.0.9/Classification/Attribute/ContinuousAttribute.py
+-rw-r--r--   0 olcay      (501) staff       (20)      918 2020-02-17 19:08:09.000000 NlpToolkit-Classification-1.0.9/Classification/Attribute/DiscreteAttribute.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1318 2020-02-17 19:08:08.000000 NlpToolkit-Classification-1.0.9/Classification/Attribute/DiscreteIndexedAttribute.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-09-28 15:01:19.000000 NlpToolkit-Classification-1.0.9/Classification/Attribute/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/
+-rw-r--r--   0 olcay      (501) staff       (20)     1543 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/AutoEncoder.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1682 2020-06-28 11:00:00.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/Bagging.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1245 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/C45.py
+-rw-r--r--   0 olcay      (501) staff       (20)      805 2020-02-17 19:08:08.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/C45Stump.py
+-rw-r--r--   0 olcay      (501) staff       (20)     3258 2020-06-26 06:32:49.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/Classifier.py
+-rw-r--r--   0 olcay      (501) staff       (20)      988 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/DeepNetwork.py
+-rw-r--r--   0 olcay      (501) staff       (20)      763 2020-02-17 19:08:08.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/Dummy.py
+-rw-r--r--   0 olcay      (501) staff       (20)      744 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/KMeans.py
+-rw-r--r--   0 olcay      (501) staff       (20)      714 2020-02-17 19:08:09.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/Knn.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1924 2020-06-27 07:13:08.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/Lda.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1179 2020-06-28 09:58:04.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/LinearPerceptron.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1223 2020-06-27 07:14:22.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/MultiLayerPerceptron.py
+-rw-r--r--   0 olcay      (501) staff       (20)     3178 2020-06-27 07:14:48.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/NaiveBayes.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1733 2020-06-27 07:16:38.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/Qda.py
+-rw-r--r--   0 olcay      (501) staff       (20)      640 2020-06-26 05:44:41.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/RandomClassifier.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1357 2020-06-26 06:04:47.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/RandomForest.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-13 14:20:08.000000 NlpToolkit-Classification-1.0.9/Classification/Classifier/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/DataSet/
+-rw-r--r--   0 olcay      (501) staff       (20)     3601 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/DataSet/DataDefinition.py
+-rw-r--r--   0 olcay      (501) staff       (20)    11818 2020-06-28 06:29:49.000000 NlpToolkit-Classification-1.0.9/Classification/DataSet/DataSet.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-09 11:07:38.000000 NlpToolkit-Classification-1.0.9/Classification/DataSet/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/DistanceMetric/
+-rw-r--r--   0 olcay      (501) staff       (20)      227 2020-02-07 20:32:13.000000 NlpToolkit-Classification-1.0.9/Classification/DistanceMetric/DistanceMetric.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1168 2020-02-07 20:32:13.000000 NlpToolkit-Classification-1.0.9/Classification/DistanceMetric/EuclidianDistance.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1243 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/DistanceMetric/MahalanobisDistance.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-15 11:26:35.000000 NlpToolkit-Classification-1.0.9/Classification/DistanceMetric/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/
+-rw-r--r--   0 olcay      (501) staff       (20)     1611 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/BootstrapRun.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2150 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/Experiment.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2062 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/KFoldRun.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2317 2020-06-27 07:10:01.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/KFoldRunSeparateTest.py
+-rw-r--r--   0 olcay      (501) staff       (20)      309 2019-10-14 06:35:36.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/MultipleRun.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1532 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/MxKFoldRun.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1882 2020-06-27 07:10:01.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/MxKFoldRunSeparateTest.py
+-rw-r--r--   0 olcay      (501) staff       (20)      277 2019-10-14 06:34:35.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/SingleRun.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1812 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/SingleRunWithK.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1427 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedKFoldRun.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1755 2020-06-27 07:10:01.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedKFoldRunSeparateTest.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1608 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedMxKFoldRun.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1610 2020-06-27 07:10:01.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedMxKFoldRunSeparateTest.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1470 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedSingleRunWithK.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-14 06:25:46.000000 NlpToolkit-Classification-1.0.9/Classification/Experiment/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/
+-rw-r--r--   0 olcay      (501) staff       (20)     1206 2020-06-29 11:22:20.000000 NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/BackwardSelection.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2179 2020-06-29 11:28:55.000000 NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/FeatureSubSet.py
+-rw-r--r--   0 olcay      (501) staff       (20)      914 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/FloatingSelection.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1048 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/ForwardSelection.py
+-rw-r--r--   0 olcay      (501) staff       (20)     3759 2020-06-29 11:11:17.000000 NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/SubSetSelection.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-14 12:39:08.000000 NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/
+-rw-r--r--   0 olcay      (501) staff       (20)     2477 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/DiscreteToContinuous.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1373 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/DiscreteToIndexed.py
+-rw-r--r--   0 olcay      (501) staff       (20)      958 2020-10-15 08:47:08.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/FeatureFilter.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1813 2020-10-15 08:47:08.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/LaryFilter.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2370 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/LaryToBinary.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1687 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/Normalize.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4147 2020-06-29 10:53:23.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/Pca.py
+-rw-r--r--   0 olcay      (501) staff       (20)      493 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/TrainedFeatureFilter.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-15 11:50:54.000000 NlpToolkit-Classification-1.0.9/Classification/Filter/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Instance/
+-rw-r--r--   0 olcay      (501) staff       (20)     1875 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Instance/CompositeInstance.py
+-rw-r--r--   0 olcay      (501) staff       (20)     6162 2020-06-28 09:21:59.000000 NlpToolkit-Classification-1.0.9/Classification/Instance/Instance.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-05 11:13:05.000000 NlpToolkit-Classification-1.0.9/Classification/Instance/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/InstanceList/
+-rw-r--r--   0 olcay      (501) staff       (20)    20477 2020-06-29 10:40:36.000000 NlpToolkit-Classification-1.0.9/Classification/InstanceList/InstanceList.py
+-rw-r--r--   0 olcay      (501) staff       (20)      658 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/InstanceList/InstanceListOfSameClass.py
+-rw-r--r--   0 olcay      (501) staff       (20)     5595 2020-06-28 07:19:06.000000 NlpToolkit-Classification-1.0.9/Classification/InstanceList/Partition.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-09 11:07:49.000000 NlpToolkit-Classification-1.0.9/Classification/InstanceList/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Model/
+-rw-r--r--   0 olcay      (501) staff       (20)     5467 2020-06-26 05:58:28.000000 NlpToolkit-Classification-1.0.9/Classification/Model/AutoEncoderModel.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Model/DecisionTree/
+-rw-r--r--   0 olcay      (501) staff       (20)     2780 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Model/DecisionTree/DecisionCondition.py
+-rw-r--r--   0 olcay      (501) staff       (20)    13496 2021-04-25 14:40:46.000000 NlpToolkit-Classification-1.0.9/Classification/Model/DecisionTree/DecisionNode.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2767 2021-04-25 14:42:08.000000 NlpToolkit-Classification-1.0.9/Classification/Model/DecisionTree/DecisionTree.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-19 05:25:07.000000 NlpToolkit-Classification-1.0.9/Classification/Model/DecisionTree/__init__.py
+-rw-r--r--   0 olcay      (501) staff       (20)     6560 2020-06-26 05:59:57.000000 NlpToolkit-Classification-1.0.9/Classification/Model/DeepNetworkModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1533 2021-04-25 14:43:24.000000 NlpToolkit-Classification-1.0.9/Classification/Model/DummyModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1855 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Model/GaussianModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2049 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Model/KMeansModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)      864 2020-10-15 07:52:20.000000 NlpToolkit-Classification-1.0.9/Classification/Model/KnnInstance.py
+-rw-r--r--   0 olcay      (501) staff       (20)     3951 2021-04-25 14:45:05.000000 NlpToolkit-Classification-1.0.9/Classification/Model/KnnModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1378 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Model/LdaModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2720 2020-06-26 06:01:52.000000 NlpToolkit-Classification-1.0.9/Classification/Model/LinearPerceptronModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1190 2021-04-25 14:45:05.000000 NlpToolkit-Classification-1.0.9/Classification/Model/Model.py
+-rw-r--r--   0 olcay      (501) staff       (20)     3787 2020-06-28 10:30:21.000000 NlpToolkit-Classification-1.0.9/Classification/Model/MultiLayerPerceptronModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     4614 2020-06-28 09:48:43.000000 NlpToolkit-Classification-1.0.9/Classification/Model/NaiveBayesModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     7599 2021-04-25 15:04:47.000000 NlpToolkit-Classification-1.0.9/Classification/Model/NeuralNetworkModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1747 2020-10-15 08:05:07.000000 NlpToolkit-Classification-1.0.9/Classification/Model/QdaModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1709 2021-04-25 14:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Model/RandomModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1407 2021-04-25 14:50:02.000000 NlpToolkit-Classification-1.0.9/Classification/Model/TreeEnsembleModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)      944 2020-02-17 19:48:49.000000 NlpToolkit-Classification-1.0.9/Classification/Model/ValidatedModel.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-13 14:20:16.000000 NlpToolkit-Classification-1.0.9/Classification/Model/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/
+-rw-r--r--   0 olcay      (501) staff       (20)      725 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/BaggingParameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1128 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/C45Parameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1833 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/DeepNetworkParameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)      972 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/KMeansParameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)      900 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/KnnParameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1933 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/LinearPerceptronParameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1318 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/MultiLayerPerceptronParameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)      495 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/Parameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)      939 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/RandomForestParameter.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-09-28 16:37:42.000000 NlpToolkit-Classification-1.0.9/Classification/Parameter/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/Performance/
+-rw-r--r--   0 olcay      (501) staff       (20)      813 2020-06-28 07:26:13.000000 NlpToolkit-Classification-1.0.9/Classification/Performance/ClassificationPerformance.py
+-rw-r--r--   0 olcay      (501) staff       (20)     6571 2020-06-28 07:29:01.000000 NlpToolkit-Classification-1.0.9/Classification/Performance/ConfusionMatrix.py
+-rw-r--r--   0 olcay      (501) staff       (20)      965 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Performance/DetailedClassificationPerformance.py
+-rw-r--r--   0 olcay      (501) staff       (20)     7888 2020-06-29 13:55:41.000000 NlpToolkit-Classification-1.0.9/Classification/Performance/ExperimentPerformance.py
+-rw-r--r--   0 olcay      (501) staff       (20)      494 2020-02-18 04:45:49.000000 NlpToolkit-Classification-1.0.9/Classification/Performance/Performance.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-09-30 18:15:40.000000 NlpToolkit-Classification-1.0.9/Classification/Performance/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/
+-rw-r--r--   0 olcay      (501) staff       (20)     2167 2020-02-18 04:52:52.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Combined5x2F.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2123 2020-02-18 04:53:50.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Combined5x2t.py
+-rw-r--r--   0 olcay      (501) staff       (20)     2048 2020-02-18 04:53:24.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Paired5x2t.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1086 2020-02-07 20:37:43.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/PairedTest.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1862 2020-06-29 13:55:58.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Pairedt.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1602 2020-02-18 04:54:27.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Sign.py
+-rw-r--r--   0 olcay      (501) staff       (20)      119 2019-10-05 10:26:00.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/StatisticalTestNotApplicable.py
+-rw-r--r--   0 olcay      (501) staff       (20)     1367 2020-02-07 20:37:43.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/StatisticalTestResult.py
+-rw-r--r--   0 olcay      (501) staff       (20)      177 2019-10-05 07:12:24.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/StatisticalTestResultType.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-10-05 07:10:00.000000 NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/__init__.py
+-rw-r--r--   0 olcay      (501) staff       (20)        0 2019-09-28 15:01:05.000000 NlpToolkit-Classification-1.0.9/Classification/__init__.py
+drwxr-xr-x   0 olcay      (501) staff       (20)        0 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/NlpToolkit_Classification.egg-info/
+-rw-r--r--   0 olcay      (501) staff       (20)      283 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/NlpToolkit_Classification.egg-info/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     5335 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/NlpToolkit_Classification.egg-info/SOURCES.txt
+-rw-r--r--   0 olcay      (501) staff       (20)        1 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/NlpToolkit_Classification.egg-info/dependency_links.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       61 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/NlpToolkit_Classification.egg-info/requires.txt
+-rw-r--r--   0 olcay      (501) staff       (20)       15 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/NlpToolkit_Classification.egg-info/top_level.txt
+-rw-r--r--   0 olcay      (501) staff       (20)      283 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/PKG-INFO
+-rw-r--r--   0 olcay      (501) staff       (20)     8555 2021-04-24 15:49:39.000000 NlpToolkit-Classification-1.0.9/README.md
+-rw-r--r--   0 olcay      (501) staff       (20)       38 2021-04-25 15:05:43.000000 NlpToolkit-Classification-1.0.9/setup.cfg
+-rw-r--r--   0 olcay      (501) staff       (20)      891 2021-04-25 15:05:36.000000 NlpToolkit-Classification-1.0.9/setup.py
```

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Attribute/ContinuousAttribute.py` & `NlpToolkit-Classification-1.0.9/Classification/Attribute/ContinuousAttribute.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Attribute/DiscreteAttribute.py` & `NlpToolkit-Classification-1.0.9/Classification/Attribute/DiscreteAttribute.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Attribute/DiscreteIndexedAttribute.py` & `NlpToolkit-Classification-1.0.9/Classification/Attribute/DiscreteIndexedAttribute.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/AutoEncoder.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/AutoEncoder.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/Bagging.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/Bagging.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/C45.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/C45.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/C45Stump.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/C45Stump.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/Classifier.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/Classifier.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/DeepNetwork.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/DeepNetwork.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/Dummy.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/Dummy.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/KMeans.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/KMeans.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/Knn.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/Knn.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/Lda.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/Lda.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/LinearPerceptron.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/LinearPerceptron.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/MultiLayerPerceptron.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/MultiLayerPerceptron.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/NaiveBayes.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/NaiveBayes.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/Qda.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/Qda.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/RandomClassifier.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/RandomClassifier.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Classifier/RandomForest.py` & `NlpToolkit-Classification-1.0.9/Classification/Classifier/RandomForest.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/DataSet/DataDefinition.py` & `NlpToolkit-Classification-1.0.9/Classification/DataSet/DataDefinition.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/DataSet/DataSet.py` & `NlpToolkit-Classification-1.0.9/Classification/DataSet/DataSet.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/DistanceMetric/EuclidianDistance.py` & `NlpToolkit-Classification-1.0.9/Classification/DistanceMetric/EuclidianDistance.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/DistanceMetric/MahalanobisDistance.py` & `NlpToolkit-Classification-1.0.9/Classification/DistanceMetric/MahalanobisDistance.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/BootstrapRun.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/BootstrapRun.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/Experiment.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/Experiment.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/KFoldRun.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/KFoldRun.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/KFoldRunSeparateTest.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/KFoldRunSeparateTest.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/MxKFoldRun.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/MxKFoldRun.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/MxKFoldRunSeparateTest.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/MxKFoldRunSeparateTest.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/SingleRunWithK.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/SingleRunWithK.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedKFoldRun.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedKFoldRun.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedKFoldRunSeparateTest.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedKFoldRunSeparateTest.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedMxKFoldRun.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedMxKFoldRun.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedMxKFoldRunSeparateTest.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedMxKFoldRunSeparateTest.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Experiment/StratifiedSingleRunWithK.py` & `NlpToolkit-Classification-1.0.9/Classification/Experiment/StratifiedSingleRunWithK.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/BackwardSelection.py` & `NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/BackwardSelection.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/FeatureSubSet.py` & `NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/FeatureSubSet.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/FloatingSelection.py` & `NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/FloatingSelection.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/ForwardSelection.py` & `NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/ForwardSelection.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/FeatureSelection/SubSetSelection.py` & `NlpToolkit-Classification-1.0.9/Classification/FeatureSelection/SubSetSelection.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Filter/DiscreteToContinuous.py` & `NlpToolkit-Classification-1.0.9/Classification/Filter/DiscreteToContinuous.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Filter/DiscreteToIndexed.py` & `NlpToolkit-Classification-1.0.9/Classification/Filter/DiscreteToIndexed.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Filter/FeatureFilter.py` & `NlpToolkit-Classification-1.0.9/Classification/Filter/FeatureFilter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Filter/LaryFilter.py` & `NlpToolkit-Classification-1.0.9/Classification/Filter/LaryFilter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Filter/LaryToBinary.py` & `NlpToolkit-Classification-1.0.9/Classification/Filter/LaryToBinary.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Filter/Normalize.py` & `NlpToolkit-Classification-1.0.9/Classification/Filter/Normalize.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Filter/Pca.py` & `NlpToolkit-Classification-1.0.9/Classification/Filter/Pca.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Instance/CompositeInstance.py` & `NlpToolkit-Classification-1.0.9/Classification/Instance/CompositeInstance.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Instance/Instance.py` & `NlpToolkit-Classification-1.0.9/Classification/Instance/Instance.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/InstanceList/InstanceList.py` & `NlpToolkit-Classification-1.0.9/Classification/InstanceList/InstanceList.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/InstanceList/InstanceListOfSameClass.py` & `NlpToolkit-Classification-1.0.9/Classification/InstanceList/InstanceListOfSameClass.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/InstanceList/Partition.py` & `NlpToolkit-Classification-1.0.9/Classification/InstanceList/Partition.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/AutoEncoderModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/AutoEncoderModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/DecisionTree/DecisionCondition.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/DecisionTree/DecisionCondition.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/DecisionTree/DecisionNode.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/DecisionTree/DecisionNode.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/DecisionTree/DecisionTree.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/DecisionTree/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/DeepNetworkModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/DeepNetworkModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/DummyModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/DummyModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/GaussianModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/GaussianModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/KMeansModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/KMeansModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/KnnInstance.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/KnnInstance.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/KnnModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/KnnModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/LdaModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/LdaModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/LinearPerceptronModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/LinearPerceptronModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/Model.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/Model.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/MultiLayerPerceptronModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/MultiLayerPerceptronModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/NaiveBayesModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/NaiveBayesModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/NeuralNetworkModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/NeuralNetworkModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,11 +223,13 @@
         self.calculateOutput()
         if isinstance(instance, CompositeInstance):
             return self.predictWithCompositeInstance(instance.getPossibleClassLabels())
         else:
             return self.classLabels[self.y.maxIndex()]
 
     def predictProbability(self, instance: Instance) -> dict:
+        self.createInputVector(instance)
+        self.calculateOutput()
         result = {}
         for i in range(len(self.classLabels)):
             result[self.classLabels[i]] = self.y.getValue(i)
         return result
```

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/QdaModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/QdaModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/RandomModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/RandomModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/TreeEnsembleModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/TreeEnsembleModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Model/ValidatedModel.py` & `NlpToolkit-Classification-1.0.9/Classification/Model/ValidatedModel.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Parameter/BaggingParameter.py` & `NlpToolkit-Classification-1.0.9/Classification/Parameter/BaggingParameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Parameter/C45Parameter.py` & `NlpToolkit-Classification-1.0.9/Classification/Parameter/C45Parameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Parameter/DeepNetworkParameter.py` & `NlpToolkit-Classification-1.0.9/Classification/Parameter/DeepNetworkParameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Parameter/KMeansParameter.py` & `NlpToolkit-Classification-1.0.9/Classification/Parameter/KMeansParameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Parameter/KnnParameter.py` & `NlpToolkit-Classification-1.0.9/Classification/Parameter/KnnParameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Parameter/LinearPerceptronParameter.py` & `NlpToolkit-Classification-1.0.9/Classification/Parameter/LinearPerceptronParameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Parameter/MultiLayerPerceptronParameter.py` & `NlpToolkit-Classification-1.0.9/Classification/Parameter/MultiLayerPerceptronParameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Parameter/RandomForestParameter.py` & `NlpToolkit-Classification-1.0.9/Classification/Parameter/RandomForestParameter.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Performance/ClassificationPerformance.py` & `NlpToolkit-Classification-1.0.9/Classification/Performance/ClassificationPerformance.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Performance/ConfusionMatrix.py` & `NlpToolkit-Classification-1.0.9/Classification/Performance/ConfusionMatrix.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Performance/DetailedClassificationPerformance.py` & `NlpToolkit-Classification-1.0.9/Classification/Performance/DetailedClassificationPerformance.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/Performance/ExperimentPerformance.py` & `NlpToolkit-Classification-1.0.9/Classification/Performance/ExperimentPerformance.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Combined5x2F.py` & `NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Combined5x2F.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Combined5x2t.py` & `NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Combined5x2t.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Paired5x2t.py` & `NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Paired5x2t.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/PairedTest.py` & `NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/PairedTest.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Pairedt.py` & `NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Pairedt.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/Sign.py` & `NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/Sign.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/Classification/StatisticalTest/StatisticalTestResult.py` & `NlpToolkit-Classification-1.0.9/Classification/StatisticalTest/StatisticalTestResult.py`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/NlpToolkit_Classification.egg-info/SOURCES.txt` & `NlpToolkit-Classification-1.0.9/NlpToolkit_Classification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/README.md` & `NlpToolkit-Classification-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `NlpToolkit-Classification-1.0.8/setup.py` & `NlpToolkit-Classification-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='NlpToolkit-Classification',
-    version='1.0.8',
+    version='1.0.9',
     packages=['Classification', 'Classification.Model', 'Classification.Model.DecisionTree', 'Classification.Filter',
               'Classification.DataSet', 'Classification.Instance', 'Classification.Attribute',
               'Classification.Parameter', 'Classification.Classifier', 'Classification.Experiment',
               'Classification.Performance', 'Classification.InstanceList', 'Classification.DistanceMetric',
               'Classification.StatisticalTest', 'Classification.FeatureSelection'],
     url='https://github.com/StarlangSoftware/Classification-Py',
     license='',
```

