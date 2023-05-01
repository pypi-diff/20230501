# Comparing `tmp/tartanair-1.0.1.tar.gz` & `tmp/tartanair-1.0.2.tar.gz`

## Comparing `tartanair-1.0.1.tar` & `tartanair-1.0.2.tar`

### file list

```diff
@@ -1,146 +1,125 @@
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 tartanair-1.0.1/.gitmodules
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tartanair-1.0.1/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tartanair-1.0.1/.github/workflows/documentation.yaml
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 tartanair-1.0.1/docs/conf.py
--rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 tartanair-1.0.1/docs/examples.rst
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tartanair-1.0.1/docs/index.rst
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 tartanair-1.0.1/docs/installation.rst
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 tartanair-1.0.1/docs/usage.rst
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/customization_example.py
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/dataloader_example.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/dataset_example.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/download_config.yaml
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/download_example.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/evaluator_example.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/get_traj_example.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/iterator_example.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/list_example.py
--rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/sanity_test.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/slowloader_example.py
--rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/trippy_video.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 tartanair-1.0.1/examples/visualization_example.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/__init__.py
--rw-r--r--   0        0        0    25971 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/customizer.py
--rw-r--r--   0        0        0    14773 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/dataloader.py
--rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/dataset.py
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/downloader.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/evaluator.py
--rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/iterator.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/lister.py
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/reader.py
--rw-r--r--   0        0        0    23789 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/tartanair.py
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/tartanair_module.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/visualizer.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/.git
--rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/CacherDataset.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/ConfigParser.py
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/DataCacher.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/DataSplitter.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/LICENSE
--rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/MultiDatasets.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/RAMBuffer.py
--rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/RAMDataset.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/README.md
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/TrajBuffer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/__init__.py
--rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/data_roots.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/input_parser.py
--rw-r--r--   0        0        0    43545 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/utils.py
--rw-r--r--   0        0        0  9454241 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/data/data_tartanairv2.txt
--rw-r--r--   0        0        0   260281 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/data/tartan_test.txt
--rw-r--r--   0        0        0  2838077 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/data/tartan_train.txt
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/modality_type/ModBase.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/modality_type/__init__.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/modality_type/ply_io.py
--rw-r--r--   0        0        0    22699 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/modality_type/tartanair_types.py
--rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/modality_type/tartanairv1_types.py
--rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/modality_type/tartandrive_types.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/data_cacher/modality_type/test_register.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/eval_utils/trajectory_evaluator_ate.py
--rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/eval_utils/trajectory_evaluator_base.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/eval_utils/trajectory_evaluator_rpe.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/.git
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/LICENSE
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/__init__.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/blend_function.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/camera_model_sampler.py
--rw-r--r--   0        0        0    11078 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/full_view_rotation.py
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/numba_support_check.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/ocv_torch.py
--rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/planar_as_base.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/register.py
--rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images_common.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images_cupy.cu
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images_numba.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images_py_numba.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/examples/README.md
--rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py
--rw-r--r--   0        0        0   445601 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt
--rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/.git
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/.gitmodules
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/LICENSE
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/README.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/__init__.py
--rw-r--r--   0        0        0    50658 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/camera_models.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/compatible_torch.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/debug.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/file_sys.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/frame_io.py
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/kalibr_parser.py
--rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/metadata_reader.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/point_cloud_helper.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/pose.py
--rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/pretty_dict.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/shape_struct.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/test_frame_io.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/test_inheritance.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/examples/README.md
--rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/.git
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/LICENSE
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/README.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/__init__.py
--rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/compatible_pytree.py
--rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py
--rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py
--rw-r--r--   0        0        0    18694 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/image_io/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/image_io/float_type.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/image_io/image_read.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/image_io/image_write.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 tartanair-1.0.1/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/ta_data_spec.txt
--rw-r--r--   0        0        0     6433 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/tartanairpy_test.py
--rw-r--r--   0        0        0    11843 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/pose_lcam_front.txt
--rw-r--r--   0        0        0    11592 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure.txt
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_easy_P000.txt
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_easy_P001.txt
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_easy_P002.txt
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_easy_P003.txt
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_easy_P004.txt
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_easy_P005.txt
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_easy_P006.txt
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_easy_P007.txt
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_hard_P000.txt
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_hard_P001.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_hard_P002.txt
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_hard_P003.txt
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_hard_P004.txt
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_hard_P005.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_hard_P006.txt
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_Data_hard_P007.txt
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_bad_frames.txt
--rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 tartanair-1.0.1/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/analyze/data_ArchVizTinyHouseDayExposure_good_frames.txt
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tartanair-1.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tartanair-1.0.1/LICENSE
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tartanair-1.0.1/README.md
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tartanair-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 tartanair-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 tartanair-1.0.2/.gitmodules
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tartanair-1.0.2/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tartanair-1.0.2/.github/workflows/documentation.yaml
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/examples.rst
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/installation.rst
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 tartanair-1.0.2/docs/usage.rst
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/customization_example.py
+-rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/dataloader_example.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/dataset_example.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/download_config.yaml
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/download_example.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/evaluator_example.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/get_traj_example.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/iterator_example.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/list_example.py
+-rw-r--r--   0        0        0     6754 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/sanity_test.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/slowloader_example.py
+-rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/trippy_video.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 tartanair-1.0.2/examples/visualization_example.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/__init__.py
+-rw-r--r--   0        0        0    25971 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/customizer.py
+-rw-r--r--   0        0        0    14773 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/dataloader.py
+-rw-r--r--   0        0        0    40499 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/dataset.py
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/downloader.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/evaluator.py
+-rw-r--r--   0        0        0    16084 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/iterator.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/lister.py
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/reader.py
+-rw-r--r--   0        0        0    23789 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/tartanair.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/tartanair_module.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/visualizer.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/.git
+-rw-r--r--   0        0        0     4962 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/CacherDataset.py
+-rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/ConfigParser.py
+-rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/DataCacher.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/DataSplitter.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/LICENSE
+-rw-r--r--   0        0        0     9715 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/MultiDatasets.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/RAMBuffer.py
+-rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/RAMDataset.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/README.md
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/TrajBuffer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/__init__.py
+-rw-r--r--   0        0        0     9001 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/data_roots.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/input_parser.py
+-rw-r--r--   0        0        0    43545 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/utils.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/ModBase.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/__init__.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/ply_io.py
+-rw-r--r--   0        0        0    22699 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/tartanair_types.py
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/tartanairv1_types.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/tartandrive_types.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/data_cacher/modality_type/test_register.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_ate.py
+-rw-r--r--   0        0        0     9795 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_base.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_rpe.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/.git
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/LICENSE
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/__init__.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/blend_function.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/camera_model_sampler.py
+-rw-r--r--   0        0        0    11078 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/full_view_rotation.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/numba_support_check.py
+-rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/ocv_torch.py
+-rw-r--r--   0        0        0     9941 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/planar_as_base.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/register.py
+-rw-r--r--   0        0        0     9238 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_common.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_cupy.cu
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_numba.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_py_numba.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/README.md
+-rw-r--r--   0        0        0     8745 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py
+-rw-r--r--   0        0        0   445601 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt
+-rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/.git
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/.gitmodules
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/LICENSE
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/README.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/__init__.py
+-rw-r--r--   0        0        0    50658 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/camera_models.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/compatible_torch.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/debug.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/file_sys.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/frame_io.py
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/kalibr_parser.py
+-rw-r--r--   0        0        0     7146 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/metadata_reader.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/point_cloud_helper.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/pose.py
+-rw-r--r--   0        0        0    14499 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/pretty_dict.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/shape_struct.py
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_frame_io.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_inheritance.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/examples/README.md
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/.git
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/LICENSE
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/README.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/__init__.py
+-rw-r--r--   0        0        0     8218 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/compatible_pytree.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py
+-rw-r--r--   0        0        0    18394 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py
+-rw-r--r--   0        0        0    18694 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/float_type.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/image_read.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/image_write.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 tartanair-1.0.2/tests/README.md
+-rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 tartanair-1.0.2/tests/tartanairpy_test.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 tartanair-1.0.2/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_doublesphere/camera_model_params_lcam_image_custom0_doublesphere.json
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tartanair-1.0.2/tests/sample_tartanair_v2_data_root/ArchVizTinyHouseDayExposure/Data_hard/P000/image_lcam_custom0_pinhole/camera_model_params_lcam_image_custom0_pinhole.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 tartanair-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tartanair-1.0.2/LICENSE
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tartanair-1.0.2/README.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 tartanair-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 tartanair-1.0.2/PKG-INFO
```

### Comparing `tartanair-1.0.1/.gitmodules` & `tartanair-1.0.2/.gitmodules`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/.github/workflows/documentation.yaml` & `tartanair-1.0.2/.github/workflows/documentation.yaml`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/docs/conf.py` & `tartanair-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/docs/examples.rst` & `tartanair-1.0.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/docs/index.rst` & `tartanair-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/docs/installation.rst` & `tartanair-1.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/docs/usage.rst` & `tartanair-1.0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/customization_example.py` & `tartanair-1.0.2/examples/customization_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/dataloader_example.py` & `tartanair-1.0.2/examples/dataloader_example.py`

 * *Files 20% similar despite different names*

```diff
@@ -80,14 +80,36 @@
     # Get the next batch.
     batch = dataloader.load_sample()
     # Check if the batch is None.
     if batch is None:
         break
     # Visualize some images.
     # The shape of an image batch is (B, S, H, W, C), where B is the batch size, S is the sequence length, H is the height, W is the width, and C is the number of channels.
+
+    # Create image cross.
+    left = batch['rgb_lcam_left'][0][0]
+    front = batch['rgb_lcam_front'][0][0]
+    right = batch['rgb_lcam_right'][0][0]
+    back = batch['rgb_lcam_back'][0][0]
+    top = batch['rgb_lcam_top'][0][0]
+    bottom = batch['rgb_lcam_bottom'][0][0]
+    cross_mid = np.concatenate([left, front, right, back], axis=1)
+    cross_top = np.concatenate([np.zeros_like(top), top, np.zeros_like(top), np.zeros_like(top)], axis=1)
+    cross_bottom = np.concatenate([np.zeros_like(bottom), bottom, np.zeros_like(bottom), np.zeros_like(bottom)], axis=1)
+    cross = np.concatenate([cross_top, cross_mid, cross_bottom], axis=0)
+
+    # Resize.
+    cross = cv2.resize(cross, (cross.shape[1]//4, cross.shape[0]//4))
+
+    # Show the image cross.
+    cv2.imshow('cross', cross)
+    cv2.imwrite('cross.png', cross)
+    cv2.waitKey(0)
+
+
     images = []
     for b in range(batch['rgb_lcam_front'].shape[0]):
         images.append(batch['rgb_lcam_front'][b][0])
     # Visualize the images.
     outimg = np.concatenate(images, axis=1)
     outimg = cv2.resize(outimg, (outimg.shape[1]//4, outimg.shape[0]//4))
     cv2.imshow('outimg', outimg)
```

### Comparing `tartanair-1.0.1/examples/dataset_example.py` & `tartanair-1.0.2/examples/dataset_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/download_example.py` & `tartanair-1.0.2/examples/download_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/evaluator_example.py` & `tartanair-1.0.2/examples/evaluator_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/get_traj_example.py` & `tartanair-1.0.2/examples/get_traj_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/iterator_example.py` & `tartanair-1.0.2/examples/iterator_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/list_example.py` & `tartanair-1.0.2/examples/list_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/sanity_test.py` & `tartanair-1.0.2/examples/sanity_test.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/slowloader_example.py` & `tartanair-1.0.2/examples/slowloader_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/trippy_video.py` & `tartanair-1.0.2/examples/trippy_video.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/examples/visualization_example.py` & `tartanair-1.0.2/examples/visualization_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/customizer.py` & `tartanair-1.0.2/tartanair/customizer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/dataloader.py` & `tartanair-1.0.2/tartanair/dataloader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/dataset.py` & `tartanair-1.0.2/tartanair/dataset.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/downloader.py` & `tartanair-1.0.2/tartanair/downloader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/evaluator.py` & `tartanair-1.0.2/tartanair/evaluator.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/iterator.py` & `tartanair-1.0.2/tartanair/iterator.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/lister.py` & `tartanair-1.0.2/tartanair/lister.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/reader.py` & `tartanair-1.0.2/tartanair/reader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/tartanair.py` & `tartanair-1.0.2/tartanair/tartanair.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/visualizer.py` & `tartanair-1.0.2/tartanair/visualizer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/CacherDataset.py` & `tartanair-1.0.2/tartanair/data_cacher/CacherDataset.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/ConfigParser.py` & `tartanair-1.0.2/tartanair/data_cacher/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/DataCacher.py` & `tartanair-1.0.2/tartanair/data_cacher/DataCacher.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/DataSplitter.py` & `tartanair-1.0.2/tartanair/data_cacher/DataSplitter.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/LICENSE` & `tartanair-1.0.2/tartanair/data_cacher/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/MultiDatasets.py` & `tartanair-1.0.2/tartanair/data_cacher/MultiDatasets.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/RAMBuffer.py` & `tartanair-1.0.2/tartanair/data_cacher/RAMBuffer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/RAMDataset.py` & `tartanair-1.0.2/tartanair/data_cacher/RAMDataset.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/TrajBuffer.py` & `tartanair-1.0.2/tartanair/data_cacher/TrajBuffer.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/data_roots.py` & `tartanair-1.0.2/tartanair/data_cacher/data_roots.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/input_parser.py` & `tartanair-1.0.2/tartanair/data_cacher/input_parser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/utils.py` & `tartanair-1.0.2/tartanair/data_cacher/utils.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml` & `tartanair-1.0.2/tartanair/data_cacher/dataspec/flowvo_train_local_v1.yaml`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml` & `tartanair-1.0.2/tartanair/data_cacher/dataspec/flowvo_train_local_v2.yaml`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/modality_type/ModBase.py` & `tartanair-1.0.2/tartanair/data_cacher/modality_type/ModBase.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/modality_type/ply_io.py` & `tartanair-1.0.2/tartanair/data_cacher/modality_type/ply_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/modality_type/tartanair_types.py` & `tartanair-1.0.2/tartanair/data_cacher/modality_type/tartanair_types.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/modality_type/tartanairv1_types.py` & `tartanair-1.0.2/tartanair/data_cacher/modality_type/tartanairv1_types.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/modality_type/tartandrive_types.py` & `tartanair-1.0.2/tartanair/data_cacher/modality_type/tartandrive_types.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/data_cacher/modality_type/test_register.py` & `tartanair-1.0.2/tartanair/data_cacher/modality_type/test_register.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/eval_utils/trajectory_evaluator_ate.py` & `tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_ate.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/eval_utils/trajectory_evaluator_base.py` & `tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_base.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/eval_utils/trajectory_evaluator_rpe.py` & `tartanair-1.0.2/tartanair/eval_utils/trajectory_evaluator_rpe.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/LICENSE` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/__init__.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/blend_function.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/blend_function.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/camera_model_sampler.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/camera_model_sampler.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/full_view_rotation.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/full_view_rotation.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/generic_camera_model_sampler.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/numba_support_check.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/numba_support_check.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/ocv_torch.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/ocv_torch.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/planar_as_base.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/planar_as_base.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/register.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/register.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images_common.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_common.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images_cupy.cu` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_cupy.cu`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images_numba.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_numba.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/six_images_py_numba.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/six_images_py_numba.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/examples/README.md` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/generic_sampler_optical_flow_sampling_example.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/data/flow_img.pt`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py` & `tartanair-1.0.2/tartanair/image_resampling/image_sampler/examples/examples_utils/visualization_utils.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/LICENSE` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/camera_models.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/camera_models.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/compatible_torch.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/compatible_torch.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/debug.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/debug.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/frame_io.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/frame_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/kalibr_parser.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/kalibr_parser.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/metadata_reader.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/metadata_reader.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/point_cloud_helper.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/point_cloud_helper.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/pose.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/pose.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/pretty_dict.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/pretty_dict.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/shape_struct.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/shape_struct.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/simulated_lidar_pre_def_models.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/test_frame_io.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_frame_io.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/test_inheritance.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/examples/README.md` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/examples/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/examples/linear_fisheye_camera_model.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/LICENSE` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/README.md` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/README.md`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/_pytree.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/frame_graph.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/ftensor.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/test_frame_graph.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/ftensor/test_ftensor.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/image_io/float_type.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/float_type.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/image_io/image_read.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/image_read.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/image_io/image_write.py` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/image_io/image_write.py`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json` & `tartanair-1.0.2/tartanair/image_resampling/mvs_utils/test_data/frame_graph.json`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/.gitignore` & `tartanair-1.0.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -142,7 +142,8 @@
 azcopy
 requirements.txt
 .vscode/settings.json
 docs/make.bat
 .gitignore
 docs/Makefile
 examples/ta_data_spec.txt
+*.txt
```

### Comparing `tartanair-1.0.1/LICENSE` & `tartanair-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tartanair-1.0.1/pyproject.toml` & `tartanair-1.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tartanair"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Yorai Shaoul", email="yorai@cmu.edu" },
   { name="Wenshan Wang", email="wenshanw@cs.cmu.edu " } 
 ]
 description = "TartanAir"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -30,11 +30,12 @@
     "plyfile",
     "pyquaternion",
     "pytransform3d",
     "PyYAML",
     "scipy",
     "torchvision",
     "pyyaml",
+    "pandas"
     ]
 
 [project.urls]
 "Homepage" = "http://theairlab.org/tartanair-dataset/"
```

### Comparing `tartanair-1.0.1/PKG-INFO` & `tartanair-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tartanair
-Version: 1.0.1
+Version: 1.0.2
 Summary: TartanAir
 Project-URL: Homepage, http://theairlab.org/tartanair-dataset/
 Author-email: Yorai Shaoul <yorai@cmu.edu>, Wenshan Wang <wenshanw@cs.cmu.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Requires-Dist: colorama>=0.4.0
 Requires-Dist: kornia
 Requires-Dist: matplotlib>=3.1.2
 Requires-Dist: networkx>=2.4
 Requires-Dist: numba>=0.56
 Requires-Dist: numpy
 Requires-Dist: opencv-contrib-python
+Requires-Dist: pandas
 Requires-Dist: pillow
 Requires-Dist: plyfile
 Requires-Dist: pyquaternion
 Requires-Dist: pytransform3d
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: torchvision
```

