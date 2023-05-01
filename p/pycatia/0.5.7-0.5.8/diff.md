# Comparing `tmp/pycatia-0.5.7.tar.gz` & `tmp/pycatia-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatia-0.5.7.tar", last modified: Fri Dec  2 10:55:47 2022, max compression
+gzip compressed data, was "pycatia-0.5.8.tar", last modified: Mon May  1 09:47:34 2023, max compression
```

## Comparing `pycatia-0.5.7.tar` & `pycatia-0.5.8.tar`

### file list

```diff
@@ -1,573 +1,573 @@
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.139387 pycatia-0.5.7/
--rw-rw-rw-   0        0        0     1087 2022-04-12 12:15:17.000000 pycatia-0.5.7/LICENSE.txt
--rw-rw-rw-   0        0        0     4853 2022-12-02 10:55:47.138388 pycatia-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     4331 2022-11-30 12:09:59.000000 pycatia-0.5.7/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.434243 pycatia-0.5.7/pycatia/
--rw-rw-rw-   0        0        0      936 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.459988 pycatia-0.5.7/pycatia/base_interfaces/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/base_interfaces/__init__.py
--rw-rw-rw-   0        0        0      224 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/base_interfaces/base_application.py
--rw-rw-rw-   0        0        0     2683 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/base_interfaces/context.py
--rw-rw-rw-   0        0        0      447 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/base_interfaces/pycatia.py
--rw-rw-rw-   0        0        0     1443 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/cat_logger.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.469680 pycatia-0.5.7/pycatia/cat_mat_interfaces/
--rw-rw-rw-   0        0        0        0 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/__init__.py
--rw-rw-rw-   0        0        0     2917 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/analysis_material.py
--rw-rw-rw-   0        0        0     6342 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/material.py
--rw-rw-rw-   0        0        0     2054 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/material_document.py
--rw-rw-rw-   0        0        0     5438 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/material_families.py
--rw-rw-rw-   0        0        0     1829 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/material_family.py
--rw-rw-rw-   0        0        0    13566 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/material_manager.py
--rw-rw-rw-   0        0        0     4988 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/materials.py
--rw-rw-rw-   0        0        0     3560 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_mat_interfaces/positioned_material.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.471681 pycatia-0.5.7/pycatia/cat_rma_interfaces/
--rw-rw-rw-   0        0        0        0 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_rma_interfaces/__init__.py
--rw-rw-rw-   0        0        0    70055 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/cat_rma_interfaces/rendering_material.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.514539 pycatia-0.5.7/pycatia/drafting_interfaces/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/drafting_interfaces/__init__.py
--rw-rw-rw-   0        0        0    59467 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drafting_setting_att.py
--rw-rw-rw-   0        0        0    15708 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_arrow.py
--rw-rw-rw-   0        0        0     7046 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_arrows.py
--rw-rw-rw-   0        0        0    19792 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_component.py
--rw-rw-rw-   0        0        0     8685 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_components.py
--rw-rw-rw-   0        0        0    19975 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dim_ext_line.py
--rw-rw-rw-   0        0        0    16325 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dim_line.py
--rw-rw-rw-   0        0        0    27211 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dim_value.py
--rw-rw-rw-   0        0        0    33622 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dimension.py
--rw-rw-rw-   0        0        0    13765 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dimensions.py
--rw-rw-rw-   0        0        0     7948 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_document.py
--rw-rw-rw-   0        0        0    16754 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_leader.py
--rw-rw-rw-   0        0        0     6833 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_leaders.py
--rw-rw-rw-   0        0        0     4575 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_page_setup.py
--rw-rw-rw-   0        0        0    13585 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_picture.py
--rw-rw-rw-   0        0        0     8304 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_pictures.py
--rw-rw-rw-   0        0        0     4097 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_root.py
--rw-rw-rw-   0        0        0    25567 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_sheet.py
--rw-rw-rw-   0        0        0    10536 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_sheets.py
--rw-rw-rw-   0        0        0    42625 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_table.py
--rw-rw-rw-   0        0        0     7567 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_tables.py
--rw-rw-rw-   0        0        0    25630 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_text.py
--rw-rw-rw-   0        0        0    19009 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_text_properties.py
--rw-rw-rw-   0        0        0     9947 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_text_range.py
--rw-rw-rw-   0        0        0     6990 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_texts.py
--rw-rw-rw-   0        0        0     3908 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_thread.py
--rw-rw-rw-   0        0        0     6682 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_threads.py
--rw-rw-rw-   0        0        0    42565 2022-08-18 11:15:13.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_view.py
--rw-rw-rw-   0        0        0    79150 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_view_generative_behavior.py
--rw-rw-rw-   0        0        0     6824 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_view_generative_links.py
--rw-rw-rw-   0        0        0     9579 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_views.py
--rw-rw-rw-   0        0        0    17535 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_welding.py
--rw-rw-rw-   0        0        0     7174 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/drawing_weldings.py
--rw-rw-rw-   0        0        0    10187 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/drafting_interfaces/print_area.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.518541 pycatia-0.5.7/pycatia/enumeration/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/enumeration/__init__.py
--rw-rw-rw-   0        0        0    52251 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/enumeration/enumeration_types.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.521539 pycatia-0.5.7/pycatia/exception_handling/
--rw-rw-rw-   0        0        0       76 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/exception_handling/__init__.py
--rw-rw-rw-   0        0        0      331 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/exception_handling/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.555108 pycatia-0.5.7/pycatia/funct_system_interfaces/
--rw-rw-rw-   0        0        0        0 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/__init__.py
--rw-rw-rw-   0        0        0     9424 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_actions_group.py
--rw-rw-rw-   0        0        0     5678 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_actions_groups.py
--rw-rw-rw-   0        0        0     3917 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_association.py
--rw-rw-rw-   0        0        0     5635 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_associations.py
--rw-rw-rw-   0        0        0     3368 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_facet_managers.py
--rw-rw-rw-   0        0        0     2511 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_gen_script_mgr.py
--rw-rw-rw-   0        0        0     2514 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_multi_rep_mgr.py
--rw-rw-rw-   0        0        0     2999 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_node_graph_layout.py
--rw-rw-rw-   0        0        0     1915 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_script.py
--rw-rw-rw-   0        0        0     5380 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/funct_scripts.py
--rw-rw-rw-   0        0        0     7313 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_action.py
--rw-rw-rw-   0        0        0     5384 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_actions.py
--rw-rw-rw-   0        0        0     7699 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_description.py
--rw-rw-rw-   0        0        0     3098 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_document.py
--rw-rw-rw-   0        0        0     2377 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_element.py
--rw-rw-rw-   0        0        0     2598 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_facet.py
--rw-rw-rw-   0        0        0     1337 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_facet_mgr.py
--rw-rw-rw-   0        0        0     4004 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_object.py
--rw-rw-rw-   0        0        0     3601 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_object_proxy.py
--rw-rw-rw-   0        0        0     5986 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_objects.py
--rw-rw-rw-   0        0        0     2867 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_position.py
--rw-rw-rw-   0        0        0    43072 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_system_setting_att.py
--rw-rw-rw-   0        0        0     2063 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_variant.py
--rw-rw-rw-   0        0        0     5103 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/funct_system_interfaces/functional_variants.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.708747 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/__init__.py
--rw-rw-rw-   0        0        0     6033 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_3d_curve_offset.py
--rw-rw-rw-   0        0        0    12648 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_affinity.py
--rw-rw-rw-   0        0        0    34360 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_assemble.py
--rw-rw-rw-   0        0        0     6050 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_line.py
--rw-rw-rw-   0        0        0     7657 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_to_axis.py
--rw-rw-rw-   0        0        0    56457 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_blend.py
--rw-rw-rw-   0        0        0     7818 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_boundary.py
--rw-rw-rw-   0        0        0     8366 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_bump.py
--rw-rw-rw-   0        0        0    14004 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle.py
--rw-rw-rw-   0        0        0    11999 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle2_points_rad.py
--rw-rw-rw-   0        0        0     7097 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle3_points.py
--rw-rw-rw-   0        0        0    16781 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_point.py
--rw-rw-rw-   0        0        0    18063 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_radius.py
--rw-rw-rw-   0        0        0     8701 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_axis.py
--rw-rw-rw-   0        0        0    16425 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_tangent.py
--rw-rw-rw-   0        0        0     7157 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_pt.py
--rw-rw-rw-   0        0        0    12704 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_rad.py
--rw-rw-rw-   0        0        0     1870 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_explicit.py
--rw-rw-rw-   0        0        0    19541 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_tritangent.py
--rw-rw-rw-   0        0        0    10145 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_combine.py
--rw-rw-rw-   0        0        0    53392 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_conic.py
--rw-rw-rw-   0        0        0    12219 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_connect.py
--rw-rw-rw-   0        0        0    22559 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_corner.py
--rw-rw-rw-   0        0        0     1522 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_explicit.py
--rw-rw-rw-   0        0        0    23764 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_par.py
--rw-rw-rw-   0        0        0    38621 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_smooth.py
--rw-rw-rw-   0        0        0    10225 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_cylinder.py
--rw-rw-rw-   0        0        0    16154 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_develop.py
--rw-rw-rw-   0        0        0    10718 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_direction.py
--rw-rw-rw-   0        0        0    11548 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extract.py
--rw-rw-rw-   0        0        0    48581 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extract_multi.py
--rw-rw-rw-   0        0        0    28384 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extrapol.py
--rw-rw-rw-   0        0        0     7303 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum.py
--rw-rw-rw-   0        0        0     6366 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum_polar.py
--rw-rw-rw-   0        0        0    15226 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extrude.py
--rw-rw-rw-   0        0        0   242671 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_factory.py
--rw-rw-rw-   0        0        0    37813 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_fill.py
--rw-rw-rw-   0        0        0    20556 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_bi_tangent.py
--rw-rw-rw-   0        0        0    10660 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_tri_tangent.py
--rw-rw-rw-   0        0        0    34043 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_healing.py
--rw-rw-rw-   0        0        0    15704 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_helix.py
--rw-rw-rw-   0        0        0    18164 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_integrated_law.py
--rw-rw-rw-   0        0        0     9958 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_intersection.py
--rw-rw-rw-   0        0        0     3469 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_inverse.py
--rw-rw-rw-   0        0        0    13234 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_law_dist_proj.py
--rw-rw-rw-   0        0        0    11962 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_angle.py
--rw-rw-rw-   0        0        0    15338 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bi_tangent.py
--rw-rw-rw-   0        0        0    12411 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bisecting.py
--rw-rw-rw-   0        0        0     1563 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_explicit.py
--rw-rw-rw-   0        0        0    11364 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_normal.py
--rw-rw-rw-   0        0        0    12928 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_dir.py
--rw-rw-rw-   0        0        0    11748 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_pt.py
--rw-rw-rw-   0        0        0    12920 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_tangency.py
--rw-rw-rw-   0        0        0    66589 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_loft.py
--rw-rw-rw-   0        0        0     4829 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_mid_surface.py
--rw-rw-rw-   0        0        0     4022 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_near.py
--rw-rw-rw-   0        0        0     7862 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_offset.py
--rw-rw-rw-   0        0        0     2655 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_curve.py
--rw-rw-rw-   0        0        0     3520 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_line1_pt.py
--rw-rw-rw-   0        0        0     4635 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane2_lines.py
--rw-rw-rw-   0        0        0     5168 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane3_points.py
--rw-rw-rw-   0        0        0     6035 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_angle.py
--rw-rw-rw-   0        0        0     9331 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_equation.py
--rw-rw-rw-   0        0        0     1574 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_explicit.py
--rw-rw-rw-   0        0        0     9251 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_mean.py
--rw-rw-rw-   0        0        0     3836 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_normal.py
--rw-rw-rw-   0        0        0     3657 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset.py
--rw-rw-rw-   0        0        0     3884 2022-04-13 12:01:46.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset_pt.py
--rw-rw-rw-   0        0        0     3876 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_tangent.py
--rw-rw-rw-   0        0        0     7468 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_between.py
--rw-rw-rw-   0        0        0     2938 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_center.py
--rw-rw-rw-   0        0        0     6992 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_coord.py
--rw-rw-rw-   0        0        0     1574 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_explicit.py
--rw-rw-rw-   0        0        0    13963 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_curve.py
--rw-rw-rw-   0        0        0    10422 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_plane.py
--rw-rw-rw-   0        0        0     6533 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_surface.py
--rw-rw-rw-   0        0        0     4324 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_tangent.py
--rw-rw-rw-   0        0        0    13205 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_polyline.py
--rw-rw-rw-   0        0        0    21183 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_position_transfo.py
--rw-rw-rw-   0        0        0    12833 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_project.py
--rw-rw-rw-   0        0        0    12451 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_reflect_line.py
--rw-rw-rw-   0        0        0    13549 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_revol.py
--rw-rw-rw-   0        0        0     9479 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_rolling_offset.py
--rw-rw-rw-   0        0        0    15733 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_rotate.py
--rw-rw-rw-   0        0        0     8169 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_scaling.py
--rw-rw-rw-   0        0        0     2780 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_section.py
--rw-rw-rw-   0        0        0    12946 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sphere.py
--rw-rw-rw-   0        0        0    19098 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_spine.py
--rw-rw-rw-   0        0        0    11743 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_spiral.py
--rw-rw-rw-   0        0        0    42981 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_spline.py
--rw-rw-rw-   0        0        0    30442 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_split.py
--rw-rw-rw-   0        0        0     1536 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_surface_explicit.py
--rw-rw-rw-   0        0        0     9038 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep.py
--rw-rw-rw-   0        0        0    49278 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_circle.py
--rw-rw-rw-   0        0        0    37464 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_conic.py
--rw-rw-rw-   0        0        0    62780 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_explicit.py
--rw-rw-rw-   0        0        0    85334 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_line.py
--rw-rw-rw-   0        0        0     6713 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_symmetry.py
--rw-rw-rw-   0        0        0     6359 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_thickness.py
--rw-rw-rw-   0        0        0     5792 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_transfer.py
--rw-rw-rw-   0        0        0    15615 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_translate.py
--rw-rw-rw-   0        0        0    42597 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_trim.py
--rw-rw-rw-   0        0        0    18591 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_unfold.py
--rw-rw-rw-   0        0        0     1529 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_volume_explicit.py
--rw-rw-rw-   0        0        0    25430 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_curve.py
--rw-rw-rw-   0        0        0     6258 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_surface.py
--rw-rw-rw-   0        0        0     9561 2022-11-30 11:49:21.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/line.py
--rw-rw-rw-   0        0        0    15950 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/plane.py
--rw-rw-rw-   0        0        0     4513 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/hybrid_shape_interfaces/point.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.794048 pycatia-0.5.7/pycatia/in_interfaces/
--rw-rw-rw-   0        0        0       21 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/__init__.py
--rw-rw-rw-   0        0        0    43835 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/in_interfaces/application.py
--rw-rw-rw-   0        0        0     2502 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/camera.py
--rw-rw-rw-   0        0        0     2780 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/camera_2d.py
--rw-rw-rw-   0        0        0     2818 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/camera_3d.py
--rw-rw-rw-   0        0        0     6566 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/cameras.py
--rw-rw-rw-   0        0        0    15684 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/cgr_adhesion_setting_att.py
--rw-rw-rw-   0        0        0    34709 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/in_interfaces/document.py
--rw-rw-rw-   0        0        0    19007 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/documentation_setting_att.py
--rw-rw-rw-   0        0        0    13266 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/in_interfaces/documents.py
--rw-rw-rw-   0        0        0     4565 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/drafting_page_setup.py
--rw-rw-rw-   0        0        0     4102 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/file.py
--rw-rw-rw-   0        0        0     3285 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/file_component.py
--rw-rw-rw-   0        0        0    18697 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/file_system.py
--rw-rw-rw-   0        0        0     3376 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/files.py
--rw-rw-rw-   0        0        0     3120 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/folder.py
--rw-rw-rw-   0        0        0     3481 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/folders.py
--rw-rw-rw-   0        0        0    23192 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/general_session_setting_att.py
--rw-rw-rw-   0        0        0     5010 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/light_source.py
--rw-rw-rw-   0        0        0     5285 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/light_sources.py
--rw-rw-rw-   0        0        0    17244 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/macros_setting_att.py
--rw-rw-rw-   0        0        0     5235 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/move.py
--rw-rw-rw-   0        0        0     1524 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/page_setup.py
--rw-rw-rw-   0        0        0     6714 2022-11-18 09:48:20.000000 pycatia-0.5.7/pycatia/in_interfaces/position.py
--rw-rw-rw-   0        0        0     5065 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/printer.py
--rw-rw-rw-   0        0        0     3434 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/printers.py
--rw-rw-rw-   0        0        0    33375 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/printers_setting_att.py
--rw-rw-rw-   0        0        0     3905 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/reference.py
--rw-rw-rw-   0        0        0     3419 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/references.py
--rw-rw-rw-   0        0        0    21779 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/search_setting_att.py
--rw-rw-rw-   0        0        0    15063 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/selected_element.py
--rw-rw-rw-   0        0        0   120144 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/in_interfaces/selection.py
--rw-rw-rw-   0        0        0     8533 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/selection_sets.py
--rw-rw-rw-   0        0        0    16375 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/send_to_service.py
--rw-rw-rw-   0        0        0     2906 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/setting_controllers.py
--rw-rw-rw-   0        0        0     3803 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/specs_and_geom_window.py
--rw-rw-rw-   0        0        0     2579 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/specs_viewer.py
--rw-rw-rw-   0        0        0     8076 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/system_configuration.py
--rw-rw-rw-   0        0        0     6602 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/text_stream.py
--rw-rw-rw-   0        0        0    38256 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/tree_viz_manip_setting_att.py
--rw-rw-rw-   0        0        0    13060 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/viewer.py
--rw-rw-rw-   0        0        0     2358 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/viewer_2d.py
--rw-rw-rw-   0        0        0    15709 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/viewer_3d.py
--rw-rw-rw-   0        0        0     3425 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/viewers.py
--rw-rw-rw-   0        0        0     5840 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/viewpoint_2d.py
--rw-rw-rw-   0        0        0    15252 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/viewpoint_3d.py
--rw-rw-rw-   0        0        0    45630 2022-11-27 12:50:10.000000 pycatia-0.5.7/pycatia/in_interfaces/vis_property_set.py
--rw-rw-rw-   0        0        0   241606 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/visualization_setting_att.py
--rw-rw-rw-   0        0        0    32340 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/vrml_setting_att.py
--rw-rw-rw-   0        0        0    15214 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/window.py
--rw-rw-rw-   0        0        0     4438 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/windows.py
--rw-rw-rw-   0        0        0     1411 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/in_interfaces/workbench.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.846806 pycatia-0.5.7/pycatia/knowledge_interfaces/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1927 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/angle.py
--rw-rw-rw-   0        0        0     2713 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/bool_param.py
--rw-rw-rw-   0        0        0     3466 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/check.py
--rw-rw-rw-   0        0        0     1976 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/constraint_satisfaction.py
--rw-rw-rw-   0        0        0     9798 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/design_table.py
--rw-rw-rw-   0        0        0     3543 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/dimension.py
--rw-rw-rw-   0        0        0     2365 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/enum_param.py
--rw-rw-rw-   0        0        0     4657 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/feature_generator.py
--rw-rw-rw-   0        0        0     2958 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/formula.py
--rw-rw-rw-   0        0        0     4100 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/free_parameter.py
--rw-rw-rw-   0        0        0     4702 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/free_parameters.py
--rw-rw-rw-   0        0        0    10853 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/int_param.py
--rw-rw-rw-   0        0        0     3836 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/knowledge_activate_object.py
--rw-rw-rw-   0        0        0     2443 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/knowledge_object.py
--rw-rw-rw-   0        0        0    39797 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/knowledge_sheet_setting_att.py
--rw-rw-rw-   0        0        0    14688 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/language_sheet_setting_att.py
--rw-rw-rw-   0        0        0     2899 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/law.py
--rw-rw-rw-   0        0        0     2040 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/length.py
--rw-rw-rw-   0        0        0     7009 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/list.py
--rw-rw-rw-   0        0        0     1766 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/list_parameter.py
--rw-rw-rw-   0        0        0     1479 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/loop.py
--rw-rw-rw-   0        0        0    11754 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/optimization.py
--rw-rw-rw-   0        0        0     3579 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/optimization_constraint.py
--rw-rw-rw-   0        0        0     5315 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/optimization_constraints.py
--rw-rw-rw-   0        0        0     5566 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/optimizations.py
--rw-rw-rw-   0        0        0    13131 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/parameter.py
--rw-rw-rw-   0        0        0     3176 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/parameter_set.py
--rw-rw-rw-   0        0        0     4949 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/parameter_sets.py
--rw-rw-rw-   0        0        0    20891 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/parameters.py
--rw-rw-rw-   0        0        0    14915 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/real_param.py
--rw-rw-rw-   0        0        0     9812 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/relation.py
--rw-rw-rw-   0        0        0    26769 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/relations.py
--rw-rw-rw-   0        0        0    51472 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/report_generation_sheet_setting_att.py
--rw-rw-rw-   0        0        0     2647 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/rule.py
--rw-rw-rw-   0        0        0    11105 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/set_of_equation.py
--rw-rw-rw-   0        0        0     6933 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/str_param.py
--rw-rw-rw-   0        0        0    25620 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/tolerance_sheet_setting_att.py
--rw-rw-rw-   0        0        0     5665 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/unit.py
--rw-rw-rw-   0        0        0     3216 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/units.py
--rw-rw-rw-   0        0        0    33338 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/knowledge_interfaces/units_sheet_setting_att.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.897264 pycatia-0.5.7/pycatia/mec_mod_interfaces/
--rw-rw-rw-   0        0        0       21 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/__init__.py
--rw-rw-rw-   0        0        0    41235 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/axis_system.py
--rw-rw-rw-   0        0        0     4627 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/axis_systems.py
--rw-rw-rw-   0        0        0     3400 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/bi_dim_feat_edge.py
--rw-rw-rw-   0        0        0     4373 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/bodies.py
--rw-rw-rw-   0        0        0     9422 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/body.py
--rw-rw-rw-   0        0        0     5009 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/boundary.py
--rw-rw-rw-   0        0        0    25287 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/constraint.py
--rw-rw-rw-   0        0        0    12680 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/constraints.py
--rw-rw-rw-   0        0        0     6097 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/cylindrical_face.py
--rw-rw-rw-   0        0        0     3567 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/edge.py
--rw-rw-rw-   0        0        0     3144 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/face.py
--rw-rw-rw-   0        0        0     1206 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/factory.py
--rw-rw-rw-   0        0        0    13037 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/fix_together.py
--rw-rw-rw-   0        0        0     5963 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/fix_togethers.py
--rw-rw-rw-   0        0        0     3918 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/geometric_elements.py
--rw-rw-rw-   0        0        0     4926 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_bodies.py
--rw-rw-rw-   0        0        0     8987 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_body.py
--rw-rw-rw-   0        0        0     4549 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_shape.py
--rw-rw-rw-   0        0        0    16133 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_shape_instance.py
--rw-rw-rw-   0        0        0     4553 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_shapes.py
--rw-rw-rw-   0        0        0    16636 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/instance_factory.py
--rw-rw-rw-   0        0        0     2060 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/mono_dim_feat_edge.py
--rw-rw-rw-   0        0        0     2249 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/not_wire_boundary_mono_dim_feat_vertex.py
--rw-rw-rw-   0        0        0     8132 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/ordered_geometrical_set.py
--rw-rw-rw-   0        0        0     5329 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/ordered_geometrical_sets.py
--rw-rw-rw-   0        0        0     3919 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/origin_elements.py
--rw-rw-rw-   0        0        0    35575 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/part.py
--rw-rw-rw-   0        0        0     3399 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/part_document.py
--rw-rw-rw-   0        0        0   230621 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/part_infrastructure_setting_att.py
--rw-rw-rw-   0        0        0     9175 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/planar_face.py
--rw-rw-rw-   0        0        0     5848 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/rectilinear_bi_dim_feat_edge.py
--rw-rw-rw-   0        0        0     5926 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/rectilinear_mono_dim_feat_edge.py
--rw-rw-rw-   0        0        0     7623 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/rectilinear_tri_dim_feat_edge.py
--rw-rw-rw-   0        0        0     1455 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/shape.py
--rw-rw-rw-   0        0        0    15849 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/shape_instance.py
--rw-rw-rw-   0        0        0     4256 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/shapes.py
--rw-rw-rw-   0        0        0     5597 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/sketches.py
--rw-rw-rw-   0        0        0     4694 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/solid.py
--rw-rw-rw-   0        0        0     2895 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/tri_dim_feat_edge.py
--rw-rw-rw-   0        0        0     2121 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/tri_dim_feat_vertex_or_bi_dim_feat_vertex.py
--rw-rw-rw-   0        0        0     3661 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/vertex.py
--rw-rw-rw-   0        0        0     2201 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/mec_mod_interfaces/zero_dim_feat_vertex_or_wire_boundary_mono_dim_feat_vertex.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.920675 pycatia-0.5.7/pycatia/navigator_interfaces/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/__init__.py
--rw-rw-rw-   0        0        0    16882 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/annotated_view.py
--rw-rw-rw-   0        0        0     8082 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/annotated_views.py
--rw-rw-rw-   0        0        0     5975 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/dmu_data_flow.py
--rw-rw-rw-   0        0        0     3443 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/dmu_review.py
--rw-rw-rw-   0        0        0     8361 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/dmu_reviews.py
--rw-rw-rw-   0        0        0    15722 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/group.py
--rw-rw-rw-   0        0        0     7821 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/groups.py
--rw-rw-rw-   0        0        0     5487 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/hyperlink.py
--rw-rw-rw-   0        0        0     7787 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/hyperlinks.py
--rw-rw-rw-   0        0        0    17112 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/marker_2D.py
--rw-rw-rw-   0        0        0    18792 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/marker_2Ds.py
--rw-rw-rw-   0        0        0    21466 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/marker_3D.py
--rw-rw-rw-   0        0        0     9076 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/marker_3Ds.py
--rw-rw-rw-   0        0        0    71610 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/marker_setting_att.py
--rw-rw-rw-   0        0        0   196711 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/n_4D_navigator_setting_att.py
--rw-rw-rw-   0        0        0    15489 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/navigator_interfaces/navigator_workbench.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.003027 pycatia-0.5.7/pycatia/part_interfaces/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1380 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/add.py
--rw-rw-rw-   0        0        0     3086 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/affinity.py
--rw-rw-rw-   0        0        0     3477 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/angular_repartition.py
--rw-rw-rw-   0        0        0     1542 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/assemble.py
--rw-rw-rw-   0        0        0     7140 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/auto_draft.py
--rw-rw-rw-   0        0        0    11415 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/auto_fillet.py
--rw-rw-rw-   0        0        0     3130 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/axis_to_axis.py
--rw-rw-rw-   0        0        0     5010 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/boolean_shape.py
--rw-rw-rw-   0        0        0    12638 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/chamfer.py
--rw-rw-rw-   0        0        0    21249 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/circ_pattern.py
--rw-rw-rw-   0        0        0    20731 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/close_surface.py
--rw-rw-rw-   0        0        0     7827 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/const_rad_edge_fillet.py
--rw-rw-rw-   0        0        0     2913 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/defeaturing.py
--rw-rw-rw-   0        0        0     1450 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/defeaturing_fillet_filter.py
--rw-rw-rw-   0        0        0     1220 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/defeaturing_filter.py
--rw-rw-rw-   0        0        0    16497 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/defeaturing_filter_with_range.py
--rw-rw-rw-   0        0        0     5942 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/defeaturing_filters.py
--rw-rw-rw-   0        0        0     1440 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/defeaturing_hole_filter.py
--rw-rw-rw-   0        0        0     4452 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/draft.py
--rw-rw-rw-   0        0        0    17507 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/draft_domain.py
--rw-rw-rw-   0        0        0     3348 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/draft_domains.py
--rw-rw-rw-   0        0        0     1559 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/dress_up_shape.py
--rw-rw-rw-   0        0        0     8029 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/edge_fillet.py
--rw-rw-rw-   0        0        0     4637 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/face_fillet.py
--rw-rw-rw-   0        0        0     4170 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/fillet.py
--rw-rw-rw-   0        0        0     1679 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/groove.py
--rw-rw-rw-   0        0        0    29934 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/hole.py
--rw-rw-rw-   0        0        0     2066 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/intersect.py
--rw-rw-rw-   0        0        0     3446 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/limit.py
--rw-rw-rw-   0        0        0     2624 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/linear_repartition.py
--rw-rw-rw-   0        0        0     2457 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/loft.py
--rw-rw-rw-   0        0        0     3395 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/mirror.py
--rw-rw-rw-   0        0        0     1565 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/pad.py
--rw-rw-rw-   0        0        0     5497 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/pattern.py
--rw-rw-rw-   0        0        0     1658 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/pocket.py
--rw-rw-rw-   0        0        0    16072 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/prism.py
--rw-rw-rw-   0        0        0    22765 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/rect_pattern.py
--rw-rw-rw-   0        0        0     1399 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/remove.py
--rw-rw-rw-   0        0        0     7954 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/remove_face.py
--rw-rw-rw-   0        0        0     2273 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/repartition.py
--rw-rw-rw-   0        0        0     6941 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/replace_face.py
--rw-rw-rw-   0        0        0     8638 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/revolution.py
--rw-rw-rw-   0        0        0     1588 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/rib.py
--rw-rw-rw-   0        0        0     5240 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/rotate.py
--rw-rw-rw-   0        0        0     3629 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/scaling.py
--rw-rw-rw-   0        0        0     4474 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/scaling2.py
--rw-rw-rw-   0        0        0    10146 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/sew_surface.py
--rw-rw-rw-   0        0        0     1671 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/shaft.py
--rw-rw-rw-   0        0        0   160771 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/part_interfaces/shape_factory.py
--rw-rw-rw-   0        0        0    13741 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/shell.py
--rw-rw-rw-   0        0        0     3738 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/sketch_based_shape.py
--rw-rw-rw-   0        0        0     1677 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/slot.py
--rw-rw-rw-   0        0        0     6529 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/solid_combine.py
--rw-rw-rw-   0        0        0     2669 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/split.py
--rw-rw-rw-   0        0        0     7359 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/stiffener.py
--rw-rw-rw-   0        0        0     2183 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/surface_based_shape.py
--rw-rw-rw-   0        0        0    12593 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/sweep.py
--rw-rw-rw-   0        0        0     2776 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/symmetry.py
--rw-rw-rw-   0        0        0     4871 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/thick_surface.py
--rw-rw-rw-   0        0        0    12606 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/thickness.py
--rw-rw-rw-   0        0        0    12918 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/thread.py
--rw-rw-rw-   0        0        0     1609 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/transformation_shape.py
--rw-rw-rw-   0        0        0     2847 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/translate.py
--rw-rw-rw-   0        0        0    19000 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/trim.py
--rw-rw-rw-   0        0        0     5338 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/tritangent_fillet.py
--rw-rw-rw-   0        0        0     4454 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/user_pattern.py
--rw-rw-rw-   0        0        0     3581 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/user_repartition.py
--rw-rw-rw-   0        0        0    16156 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/part_interfaces/var_rad_edge_fillet.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.012029 pycatia-0.5.7/pycatia/product_structure_interfaces/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/product_structure_interfaces/__init__.py
--rw-rw-rw-   0        0        0     8690 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/product_structure_interfaces/analyze.py
--rw-rw-rw-   0        0        0     4920 2022-04-13 12:01:46.000000 pycatia-0.5.7/pycatia/product_structure_interfaces/assembly_convertor.py
--rw-rw-rw-   0        0        0    56658 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/product_structure_interfaces/product.py
--rw-rw-rw-   0        0        0     2752 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/product_structure_interfaces/product_document.py
--rw-rw-rw-   0        0        0    17282 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/product_structure_interfaces/products.py
--rw-rw-rw-   0        0        0     3594 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/product_structure_interfaces/publication.py
--rw-rw-rw-   0        0        0    10017 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/product_structure_interfaces/publications.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.016770 pycatia-0.5.7/pycatia/scripts/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/scripts/__init__.py
--rw-rw-rw-   0        0        0      388 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/scripts/checking.py
--rw-rw-rw-   0        0        0     2916 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/scripts/csv_tools.py
--rw-rw-rw-   0        0        0      914 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/scripts/document_types.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.032242 pycatia-0.5.7/pycatia/sketcher_interfaces/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/__init__.py
--rw-rw-rw-   0        0        0     2854 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/axis_2D.py
--rw-rw-rw-   0        0        0     5295 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/circle_2D.py
--rw-rw-rw-   0        0        0     5482 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/control_point_2D.py
--rw-rw-rw-   0        0        0    17525 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/curve_2D.py
--rw-rw-rw-   0        0        0     8859 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/ellipse_2D.py
--rw-rw-rw-   0        0        0    20999 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/factory_2D.py
--rw-rw-rw-   0        0        0     1863 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/geometric_element.py
--rw-rw-rw-   0        0        0     2659 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/geometry_2D.py
--rw-rw-rw-   0        0        0     6788 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/hyperbola_2D.py
--rw-rw-rw-   0        0        0     5201 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/line_2D.py
--rw-rw-rw-   0        0        0     5926 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/parabola_2D.py
--rw-rw-rw-   0        0        0     3233 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/point_2D.py
--rw-rw-rw-   0        0        0    13726 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/sketch.py
--rw-rw-rw-   0        0        0     5391 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/sketcher_interfaces/spline_2D.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.052253 pycatia-0.5.7/pycatia/space_analyses_interfaces/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/__init__.py
--rw-rw-rw-   0        0        0    13227 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/clash.py
--rw-rw-rw-   0        0        0     3448 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/clash_result.py
--rw-rw-rw-   0        0        0     7191 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/clash_results.py
--rw-rw-rw-   0        0        0     6989 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/clashes.py
--rw-rw-rw-   0        0        0    12155 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/conflict.py
--rw-rw-rw-   0        0        0     3179 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/conflicts.py
--rw-rw-rw-   0        0        0    21840 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/distance.py
--rw-rw-rw-   0        0        0     7294 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/distances.py
--rw-rw-rw-   0        0        0      227 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/general_functions.py
--rw-rw-rw-   0        0        0    15124 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/inertia.py
--rw-rw-rw-   0        0        0     6662 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/inertias.py
--rw-rw-rw-   0        0        0    25608 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/measurable.py
--rw-rw-rw-   0        0        0    28720 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/measure_setting_att.py
--rw-rw-rw-   0        0        0    21497 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/section.py
--rw-rw-rw-   0        0        0    81518 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/sectioning_setting_att.py
--rw-rw-rw-   0        0        0     7207 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/sections.py
--rw-rw-rw-   0        0        0     8178 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/space_analyses_interfaces/spa_workbench.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.081676 pycatia-0.5.7/pycatia/system_interfaces/
--rw-rw-rw-   0        0        0       23 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/system_interfaces/__init__.py
--rw-rw-rw-   0        0        0     1915 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/accesslog_statistics_setting_att.py
--rw-rw-rw-   0        0        0     7750 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/any_object.py
--rw-rw-rw-   0        0        0    28964 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/cache_setting_att.py
--rw-rw-rw-   0        0        0     1666 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/cat_base_dispatch.py
--rw-rw-rw-   0        0        0     1530 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/cat_base_unknown.py
--rw-rw-rw-   0        0        0     8904 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/collection.py
--rw-rw-rw-   0        0        0     1901 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/command_statistics_setting_att.py
--rw-rw-rw-   0        0        0     7521 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/disconnection_setting_att.py
--rw-rw-rw-   0        0        0    23652 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/dl_name_setting_att.py
--rw-rw-rw-   0        0        0    12275 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/dyn_license_setting_att.py
--rw-rw-rw-   0        0        0     9646 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/errorlog_statistics_setting_att.py
--rw-rw-rw-   0        0        0     1920 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/file_access_statistics_setting_att.py
--rw-rw-rw-   0        0        0    21080 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/general_statistics_setting_att.py
--rw-rw-rw-   0        0        0     7896 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/global_statistics_setting_att.py
--rw-rw-rw-   0        0        0     1257 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/i_dispatch.py
--rw-rw-rw-   0        0        0     1147 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/i_unknown.py
--rw-rw-rw-   0        0        0    29377 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/license_setting_att.py
--rw-rw-rw-   0        0        0    10573 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/memory_warning_setting_att.py
--rw-rw-rw-   0        0        0     2732 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/pcs_statistics_setting_att.py
--rw-rw-rw-   0        0        0     1895 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/server_statistics_setting_att.py
--rw-rw-rw-   0        0        0     1901 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/session_statistics_setting_att.py
--rw-rw-rw-   0        0        0    12823 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/setting_controller.py
--rw-rw-rw-   0        0        0    13614 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/setting_repository.py
--rw-rw-rw-   0        0        0    12706 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/system_service.py
--rw-rw-rw-   0        0        0     1914 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/system_interfaces/workbench_statistics_setting_att.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.134387 pycatia-0.5.7/pycatia/tps_interfaces/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/__init__.py
--rw-rw-rw-   0        0        0    32496 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/annotation.py
--rw-rw-rw-   0        0        0    20353 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/annotation_2.py
--rw-rw-rw-   0        0        0    20429 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/annotation_factory.py
--rw-rw-rw-   0        0        0    22390 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/annotation_factory_2.py
--rw-rw-rw-   0        0        0    15049 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/annotation_set.py
--rw-rw-rw-   0        0        0     2576 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/annotation_set_transform_into_assembly_set.py
--rw-rw-rw-   0        0        0     3708 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/annotation_sets.py
--rw-rw-rw-   0        0        0     4109 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/annotations.py
--rw-rw-rw-   0        0        0     3005 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/assembly_annotation_sets.py
--rw-rw-rw-   0        0        0     2717 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/associated_ref_frame.py
--rw-rw-rw-   0        0        0    11972 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/capture.py
--rw-rw-rw-   0        0        0     2067 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/capture_factory.py
--rw-rw-rw-   0        0        0     2163 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/captures.py
--rw-rw-rw-   0        0        0     2309 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/composite_tolerance.py
--rw-rw-rw-   0        0        0     1772 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/controlled_radius.py
--rw-rw-rw-   0        0        0     2553 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/datum_simple.py
--rw-rw-rw-   0        0        0    11766 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/datum_target.py
--rw-rw-rw-   0        0        0     3526 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/default_annotation.py
--rw-rw-rw-   0        0        0    10599 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/dimension_3d.py
--rw-rw-rw-   0        0        0     6363 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/dimension_limit.py
--rw-rw-rw-   0        0        0     1642 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/dimension_pattern.py
--rw-rw-rw-   0        0        0    20046 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/dmu_tol_setting_att.py
--rw-rw-rw-   0        0        0     1663 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/envelope_condition.py
--rw-rw-rw-   0        0        0     9455 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/flag_note.py
--rw-rw-rw-   0        0        0     1761 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/free_state.py
--rw-rw-rw-   0        0        0    70472 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/fta_infra_setting_att.py
--rw-rw-rw-   0        0        0   241089 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/fta_setting_att.py
--rw-rw-rw-   0        0        0     1671 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/material_condition.py
--rw-rw-rw-   0        0        0    11475 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/noa.py
--rw-rw-rw-   0        0        0     1767 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/non_semantic_datum.py
--rw-rw-rw-   0        0        0     3225 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/non_semantic_datum_target.py
--rw-rw-rw-   0        0        0     3380 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/non_semantic_dimension.py
--rw-rw-rw-   0        0        0     1736 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/non_semantic_gdt.py
--rw-rw-rw-   0        0        0     1941 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/particular_tol_elem.py
--rw-rw-rw-   0        0        0     5589 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/projected_tolerance_zone.py
--rw-rw-rw-   0        0        0    14665 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/reference_frame.py
--rw-rw-rw-   0        0        0     6101 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/roughness.py
--rw-rw-rw-   0        0        0    18486 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/semantic_gdt.py
--rw-rw-rw-   0        0        0     6901 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/shifted_profile_tolerance.py
--rw-rw-rw-   0        0        0     1785 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/tangent_plane.py
--rw-rw-rw-   0        0        0     2788 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/text.py
--rw-rw-rw-   0        0        0     2203 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/tolerance_per_unit_basis_restrictive_value.py
--rw-rw-rw-   0        0        0     3066 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/tolerance_unit_basis_value.py
--rw-rw-rw-   0        0        0     2349 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/tolerance_zone.py
--rw-rw-rw-   0        0        0     2553 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/tps_parallel_on_screen.py
--rw-rw-rw-   0        0        0     1221 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/tps_view.py
--rw-rw-rw-   0        0        0     2659 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/tps_view_factory.py
--rw-rw-rw-   0        0        0     2208 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/tps_views.py
--rw-rw-rw-   0        0        0     6298 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/user_surface.py
--rw-rw-rw-   0        0        0     7897 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/user_surfaces.py
--rw-rw-rw-   0        0        0     2204 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/tps_interfaces/weld.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:47.137389 pycatia-0.5.7/pycatia/types/
--rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/types/__init__.py
--rw-rw-rw-   0        0        0      584 2022-11-18 10:48:10.000000 pycatia-0.5.7/pycatia/types/document_types.py
--rw-rw-rw-   0        0        0      560 2022-04-12 12:15:17.000000 pycatia-0.5.7/pycatia/types/general.py
--rw-rw-rw-   0        0        0       19 2022-11-30 12:09:59.000000 pycatia-0.5.7/pycatia/version.py
-drwxrwxrwx   0        0        0        0 2022-12-02 10:55:46.455017 pycatia-0.5.7/pycatia.egg-info/
--rw-rw-rw-   0        0        0     4853 2022-12-02 10:55:46.000000 pycatia-0.5.7/pycatia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    25596 2022-12-02 10:55:46.000000 pycatia-0.5.7/pycatia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-02 10:55:46.000000 pycatia-0.5.7/pycatia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-12-02 10:55:46.000000 pycatia-0.5.7/pycatia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-02 10:55:46.000000 pycatia-0.5.7/pycatia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-02 10:55:47.139387 pycatia-0.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1049 2022-11-30 12:09:59.000000 pycatia-0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:34.022381 pycatia-0.5.8/
+-rw-rw-rw-   0        0        0     1087 2022-04-12 12:15:17.000000 pycatia-0.5.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     4853 2023-05-01 09:47:34.022381 pycatia-0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4331 2023-05-01 08:31:08.000000 pycatia-0.5.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.415332 pycatia-0.5.8/pycatia/
+-rw-rw-rw-   0        0        0      936 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.441159 pycatia-0.5.8/pycatia/base_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/base_interfaces/__init__.py
+-rw-rw-rw-   0        0        0      224 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/base_interfaces/base_application.py
+-rw-rw-rw-   0        0        0     2683 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/base_interfaces/context.py
+-rw-rw-rw-   0        0        0      447 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/base_interfaces/pycatia.py
+-rw-rw-rw-   0        0        0     1443 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/cat_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.450001 pycatia-0.5.8/pycatia/cat_mat_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-08-18 11:15:13.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/analysis_material.py
+-rw-rw-rw-   0        0        0     6342 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/material.py
+-rw-rw-rw-   0        0        0     2054 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/material_document.py
+-rw-rw-rw-   0        0        0     5438 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/material_families.py
+-rw-rw-rw-   0        0        0     1829 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/material_family.py
+-rw-rw-rw-   0        0        0    13566 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/material_manager.py
+-rw-rw-rw-   0        0        0     4988 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/materials.py
+-rw-rw-rw-   0        0        0     3560 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_mat_interfaces/positioned_material.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.451002 pycatia-0.5.8/pycatia/cat_rma_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-08-18 11:15:13.000000 pycatia-0.5.8/pycatia/cat_rma_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    70055 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/cat_rma_interfaces/rendering_material.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.489218 pycatia-0.5.8/pycatia/drafting_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/drafting_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    59467 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drafting_setting_att.py
+-rw-rw-rw-   0        0        0    15708 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_arrow.py
+-rw-rw-rw-   0        0        0     7046 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_arrows.py
+-rw-rw-rw-   0        0        0    19792 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_component.py
+-rw-rw-rw-   0        0        0     8685 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_components.py
+-rw-rw-rw-   0        0        0    19975 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dim_ext_line.py
+-rw-rw-rw-   0        0        0    16325 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dim_line.py
+-rw-rw-rw-   0        0        0    27211 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dim_value.py
+-rw-rw-rw-   0        0        0    33622 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dimension.py
+-rw-rw-rw-   0        0        0    13765 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dimensions.py
+-rw-rw-rw-   0        0        0     7948 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_document.py
+-rw-rw-rw-   0        0        0    16754 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_leader.py
+-rw-rw-rw-   0        0        0     6833 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_leaders.py
+-rw-rw-rw-   0        0        0     4575 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_page_setup.py
+-rw-rw-rw-   0        0        0    13585 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_picture.py
+-rw-rw-rw-   0        0        0     8304 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_pictures.py
+-rw-rw-rw-   0        0        0     4097 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_root.py
+-rw-rw-rw-   0        0        0    25567 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_sheet.py
+-rw-rw-rw-   0        0        0    10536 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_sheets.py
+-rw-rw-rw-   0        0        0    42625 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_table.py
+-rw-rw-rw-   0        0        0     7567 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_tables.py
+-rw-rw-rw-   0        0        0    25630 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_text.py
+-rw-rw-rw-   0        0        0    19009 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_text_properties.py
+-rw-rw-rw-   0        0        0     9947 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_text_range.py
+-rw-rw-rw-   0        0        0     6990 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_texts.py
+-rw-rw-rw-   0        0        0     3908 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_thread.py
+-rw-rw-rw-   0        0        0     6682 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_threads.py
+-rw-rw-rw-   0        0        0    42565 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_view.py
+-rw-rw-rw-   0        0        0    79150 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_view_generative_behavior.py
+-rw-rw-rw-   0        0        0     6824 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_view_generative_links.py
+-rw-rw-rw-   0        0        0     9579 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_views.py
+-rw-rw-rw-   0        0        0    17535 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_welding.py
+-rw-rw-rw-   0        0        0     7174 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/drawing_weldings.py
+-rw-rw-rw-   0        0        0    10187 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/drafting_interfaces/print_area.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.491219 pycatia-0.5.8/pycatia/enumeration/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/enumeration/__init__.py
+-rw-rw-rw-   0        0        0    52251 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/enumeration/enumeration_types.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.493734 pycatia-0.5.8/pycatia/exception_handling/
+-rw-rw-rw-   0        0        0       76 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/exception_handling/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/exception_handling/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.518703 pycatia-0.5.8/pycatia/funct_system_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-11-18 10:48:10.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     9424 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_actions_group.py
+-rw-rw-rw-   0        0        0     5678 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_actions_groups.py
+-rw-rw-rw-   0        0        0     3917 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_association.py
+-rw-rw-rw-   0        0        0     5635 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_associations.py
+-rw-rw-rw-   0        0        0     3368 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_facet_managers.py
+-rw-rw-rw-   0        0        0     2511 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_gen_script_mgr.py
+-rw-rw-rw-   0        0        0     2514 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_multi_rep_mgr.py
+-rw-rw-rw-   0        0        0     2999 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_node_graph_layout.py
+-rw-rw-rw-   0        0        0     1915 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_script.py
+-rw-rw-rw-   0        0        0     5380 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/funct_scripts.py
+-rw-rw-rw-   0        0        0     7313 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_action.py
+-rw-rw-rw-   0        0        0     5384 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_actions.py
+-rw-rw-rw-   0        0        0     7699 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_description.py
+-rw-rw-rw-   0        0        0     3098 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_document.py
+-rw-rw-rw-   0        0        0     2377 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_element.py
+-rw-rw-rw-   0        0        0     2598 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_facet.py
+-rw-rw-rw-   0        0        0     1337 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_facet_mgr.py
+-rw-rw-rw-   0        0        0     4004 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_object.py
+-rw-rw-rw-   0        0        0     3601 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_object_proxy.py
+-rw-rw-rw-   0        0        0     5986 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_objects.py
+-rw-rw-rw-   0        0        0     2867 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_position.py
+-rw-rw-rw-   0        0        0    43072 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_system_setting_att.py
+-rw-rw-rw-   0        0        0     2063 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_variant.py
+-rw-rw-rw-   0        0        0     5103 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/funct_system_interfaces/functional_variants.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.638318 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     6033 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_3d_curve_offset.py
+-rw-rw-rw-   0        0        0    12648 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_affinity.py
+-rw-rw-rw-   0        0        0    34360 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_assemble.py
+-rw-rw-rw-   0        0        0     6050 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_line.py
+-rw-rw-rw-   0        0        0     7657 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_to_axis.py
+-rw-rw-rw-   0        0        0    56457 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_blend.py
+-rw-rw-rw-   0        0        0     7818 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_boundary.py
+-rw-rw-rw-   0        0        0     8366 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_bump.py
+-rw-rw-rw-   0        0        0    14004 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle.py
+-rw-rw-rw-   0        0        0    11999 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle2_points_rad.py
+-rw-rw-rw-   0        0        0     7097 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle3_points.py
+-rw-rw-rw-   0        0        0    16781 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_point.py
+-rw-rw-rw-   0        0        0    18063 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_radius.py
+-rw-rw-rw-   0        0        0     8701 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_axis.py
+-rw-rw-rw-   0        0        0    16425 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_tangent.py
+-rw-rw-rw-   0        0        0     7157 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_pt.py
+-rw-rw-rw-   0        0        0    12704 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_rad.py
+-rw-rw-rw-   0        0        0     1870 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_explicit.py
+-rw-rw-rw-   0        0        0    19541 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_tritangent.py
+-rw-rw-rw-   0        0        0    10145 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_combine.py
+-rw-rw-rw-   0        0        0    53392 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_conic.py
+-rw-rw-rw-   0        0        0    12219 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_connect.py
+-rw-rw-rw-   0        0        0    22559 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_corner.py
+-rw-rw-rw-   0        0        0     1522 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_explicit.py
+-rw-rw-rw-   0        0        0    23764 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_par.py
+-rw-rw-rw-   0        0        0    38621 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_smooth.py
+-rw-rw-rw-   0        0        0    10225 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_cylinder.py
+-rw-rw-rw-   0        0        0    16154 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_develop.py
+-rw-rw-rw-   0        0        0    10718 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_direction.py
+-rw-rw-rw-   0        0        0    11548 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extract.py
+-rw-rw-rw-   0        0        0    48581 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extract_multi.py
+-rw-rw-rw-   0        0        0    28384 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extrapol.py
+-rw-rw-rw-   0        0        0     7303 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum.py
+-rw-rw-rw-   0        0        0     6366 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum_polar.py
+-rw-rw-rw-   0        0        0    15237 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extrude.py
+-rw-rw-rw-   0        0        0   241156 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_factory.py
+-rw-rw-rw-   0        0        0    37813 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fill.py
+-rw-rw-rw-   0        0        0    20556 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_bi_tangent.py
+-rw-rw-rw-   0        0        0    10660 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_tri_tangent.py
+-rw-rw-rw-   0        0        0    34043 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_healing.py
+-rw-rw-rw-   0        0        0    15704 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_helix.py
+-rw-rw-rw-   0        0        0    18164 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_integrated_law.py
+-rw-rw-rw-   0        0        0     9958 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_intersection.py
+-rw-rw-rw-   0        0        0     3469 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_inverse.py
+-rw-rw-rw-   0        0        0    13234 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_law_dist_proj.py
+-rw-rw-rw-   0        0        0    11962 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_angle.py
+-rw-rw-rw-   0        0        0    15338 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bi_tangent.py
+-rw-rw-rw-   0        0        0    12411 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bisecting.py
+-rw-rw-rw-   0        0        0     1563 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_explicit.py
+-rw-rw-rw-   0        0        0    11364 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_normal.py
+-rw-rw-rw-   0        0        0    12928 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_dir.py
+-rw-rw-rw-   0        0        0    11748 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_pt.py
+-rw-rw-rw-   0        0        0    12920 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_tangency.py
+-rw-rw-rw-   0        0        0    66589 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_loft.py
+-rw-rw-rw-   0        0        0     4829 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_mid_surface.py
+-rw-rw-rw-   0        0        0     4022 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_near.py
+-rw-rw-rw-   0        0        0     7862 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_offset.py
+-rw-rw-rw-   0        0        0     2655 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_curve.py
+-rw-rw-rw-   0        0        0     3520 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_line1_pt.py
+-rw-rw-rw-   0        0        0     4635 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane2_lines.py
+-rw-rw-rw-   0        0        0     5168 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane3_points.py
+-rw-rw-rw-   0        0        0     6035 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_angle.py
+-rw-rw-rw-   0        0        0     9331 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_equation.py
+-rw-rw-rw-   0        0        0     1574 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_explicit.py
+-rw-rw-rw-   0        0        0     9251 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_mean.py
+-rw-rw-rw-   0        0        0     3836 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_normal.py
+-rw-rw-rw-   0        0        0     3657 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset.py
+-rw-rw-rw-   0        0        0     3884 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset_pt.py
+-rw-rw-rw-   0        0        0     3876 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_tangent.py
+-rw-rw-rw-   0        0        0     7468 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_between.py
+-rw-rw-rw-   0        0        0     2938 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_center.py
+-rw-rw-rw-   0        0        0     6992 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_coord.py
+-rw-rw-rw-   0        0        0     1574 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_explicit.py
+-rw-rw-rw-   0        0        0    13963 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_curve.py
+-rw-rw-rw-   0        0        0    10422 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_plane.py
+-rw-rw-rw-   0        0        0     6533 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_surface.py
+-rw-rw-rw-   0        0        0     4324 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_tangent.py
+-rw-rw-rw-   0        0        0    13205 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_polyline.py
+-rw-rw-rw-   0        0        0    21183 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_position_transfo.py
+-rw-rw-rw-   0        0        0    12833 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_project.py
+-rw-rw-rw-   0        0        0    12451 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_reflect_line.py
+-rw-rw-rw-   0        0        0    13549 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_revol.py
+-rw-rw-rw-   0        0        0     9479 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_rolling_offset.py
+-rw-rw-rw-   0        0        0    15733 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_rotate.py
+-rw-rw-rw-   0        0        0     8169 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_scaling.py
+-rw-rw-rw-   0        0        0     2780 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_section.py
+-rw-rw-rw-   0        0        0    12946 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sphere.py
+-rw-rw-rw-   0        0        0    19098 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spine.py
+-rw-rw-rw-   0        0        0    11743 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spiral.py
+-rw-rw-rw-   0        0        0    42981 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spline.py
+-rw-rw-rw-   0        0        0    30442 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_split.py
+-rw-rw-rw-   0        0        0     1536 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_surface_explicit.py
+-rw-rw-rw-   0        0        0     9038 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep.py
+-rw-rw-rw-   0        0        0    49278 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_circle.py
+-rw-rw-rw-   0        0        0    37464 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_conic.py
+-rw-rw-rw-   0        0        0    62780 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_explicit.py
+-rw-rw-rw-   0        0        0    85334 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_line.py
+-rw-rw-rw-   0        0        0     6713 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_symmetry.py
+-rw-rw-rw-   0        0        0     6359 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_thickness.py
+-rw-rw-rw-   0        0        0     5792 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_transfer.py
+-rw-rw-rw-   0        0        0    15615 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_translate.py
+-rw-rw-rw-   0        0        0    42597 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_trim.py
+-rw-rw-rw-   0        0        0    18591 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_unfold.py
+-rw-rw-rw-   0        0        0     1529 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_volume_explicit.py
+-rw-rw-rw-   0        0        0    25430 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_curve.py
+-rw-rw-rw-   0        0        0     6258 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_surface.py
+-rw-rw-rw-   0        0        0     9561 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/line.py
+-rw-rw-rw-   0        0        0    15950 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/plane.py
+-rw-rw-rw-   0        0        0     4513 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/hybrid_shape_interfaces/point.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.693472 pycatia-0.5.8/pycatia/in_interfaces/
+-rw-rw-rw-   0        0        0       21 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/in_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    43835 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/in_interfaces/application.py
+-rw-rw-rw-   0        0        0     2502 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/camera.py
+-rw-rw-rw-   0        0        0     2780 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/camera_2d.py
+-rw-rw-rw-   0        0        0     2818 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/camera_3d.py
+-rw-rw-rw-   0        0        0     6566 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/cameras.py
+-rw-rw-rw-   0        0        0    15684 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/cgr_adhesion_setting_att.py
+-rw-rw-rw-   0        0        0    34709 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/document.py
+-rw-rw-rw-   0        0        0    19007 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/documentation_setting_att.py
+-rw-rw-rw-   0        0        0    13197 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/documents.py
+-rw-rw-rw-   0        0        0     4565 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/drafting_page_setup.py
+-rw-rw-rw-   0        0        0     4102 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/file.py
+-rw-rw-rw-   0        0        0     3285 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/file_component.py
+-rw-rw-rw-   0        0        0    18697 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/file_system.py
+-rw-rw-rw-   0        0        0     3376 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/files.py
+-rw-rw-rw-   0        0        0     3120 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/folder.py
+-rw-rw-rw-   0        0        0     3481 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/folders.py
+-rw-rw-rw-   0        0        0    23192 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/general_session_setting_att.py
+-rw-rw-rw-   0        0        0     5010 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/light_source.py
+-rw-rw-rw-   0        0        0     5285 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/light_sources.py
+-rw-rw-rw-   0        0        0    17244 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/macros_setting_att.py
+-rw-rw-rw-   0        0        0     5235 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/move.py
+-rw-rw-rw-   0        0        0     1524 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/page_setup.py
+-rw-rw-rw-   0        0        0     6714 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/position.py
+-rw-rw-rw-   0        0        0     5065 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/printer.py
+-rw-rw-rw-   0        0        0     3434 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/printers.py
+-rw-rw-rw-   0        0        0    33375 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/printers_setting_att.py
+-rw-rw-rw-   0        0        0     3905 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/reference.py
+-rw-rw-rw-   0        0        0     3419 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/references.py
+-rw-rw-rw-   0        0        0    21779 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/search_setting_att.py
+-rw-rw-rw-   0        0        0    15063 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/selected_element.py
+-rw-rw-rw-   0        0        0   120144 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/selection.py
+-rw-rw-rw-   0        0        0     8533 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/selection_sets.py
+-rw-rw-rw-   0        0        0    16375 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/send_to_service.py
+-rw-rw-rw-   0        0        0     2906 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/setting_controllers.py
+-rw-rw-rw-   0        0        0     3803 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/specs_and_geom_window.py
+-rw-rw-rw-   0        0        0     2579 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/specs_viewer.py
+-rw-rw-rw-   0        0        0     8076 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/system_configuration.py
+-rw-rw-rw-   0        0        0     6602 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/text_stream.py
+-rw-rw-rw-   0        0        0    38256 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/tree_viz_manip_setting_att.py
+-rw-rw-rw-   0        0        0    13060 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/viewer.py
+-rw-rw-rw-   0        0        0     2358 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/viewer_2d.py
+-rw-rw-rw-   0        0        0    15709 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/viewer_3d.py
+-rw-rw-rw-   0        0        0     3425 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/viewers.py
+-rw-rw-rw-   0        0        0     5840 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/viewpoint_2d.py
+-rw-rw-rw-   0        0        0    15252 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/viewpoint_3d.py
+-rw-rw-rw-   0        0        0    45630 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/vis_property_set.py
+-rw-rw-rw-   0        0        0   241606 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/visualization_setting_att.py
+-rw-rw-rw-   0        0        0    32340 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/vrml_setting_att.py
+-rw-rw-rw-   0        0        0    15214 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/window.py
+-rw-rw-rw-   0        0        0     4438 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/windows.py
+-rw-rw-rw-   0        0        0     1411 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/in_interfaces/workbench.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.736412 pycatia-0.5.8/pycatia/knowledge_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1927 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/angle.py
+-rw-rw-rw-   0        0        0     2713 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/bool_param.py
+-rw-rw-rw-   0        0        0     3466 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/check.py
+-rw-rw-rw-   0        0        0     1976 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/constraint_satisfaction.py
+-rw-rw-rw-   0        0        0     9798 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/design_table.py
+-rw-rw-rw-   0        0        0     3543 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/dimension.py
+-rw-rw-rw-   0        0        0     2365 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/enum_param.py
+-rw-rw-rw-   0        0        0     4657 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/feature_generator.py
+-rw-rw-rw-   0        0        0     2958 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/formula.py
+-rw-rw-rw-   0        0        0     4100 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/free_parameter.py
+-rw-rw-rw-   0        0        0     4702 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/free_parameters.py
+-rw-rw-rw-   0        0        0    10853 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/int_param.py
+-rw-rw-rw-   0        0        0     3836 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/knowledge_activate_object.py
+-rw-rw-rw-   0        0        0     2443 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/knowledge_object.py
+-rw-rw-rw-   0        0        0    39797 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/knowledge_sheet_setting_att.py
+-rw-rw-rw-   0        0        0    14688 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/language_sheet_setting_att.py
+-rw-rw-rw-   0        0        0     2899 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/law.py
+-rw-rw-rw-   0        0        0     2040 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/length.py
+-rw-rw-rw-   0        0        0     7009 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/list.py
+-rw-rw-rw-   0        0        0     1766 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/list_parameter.py
+-rw-rw-rw-   0        0        0     1479 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/loop.py
+-rw-rw-rw-   0        0        0    11754 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/optimization.py
+-rw-rw-rw-   0        0        0     3579 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/optimization_constraint.py
+-rw-rw-rw-   0        0        0     5315 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/optimization_constraints.py
+-rw-rw-rw-   0        0        0     5566 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/optimizations.py
+-rw-rw-rw-   0        0        0    13131 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/parameter.py
+-rw-rw-rw-   0        0        0     3176 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/parameter_set.py
+-rw-rw-rw-   0        0        0     4949 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/parameter_sets.py
+-rw-rw-rw-   0        0        0    20891 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/parameters.py
+-rw-rw-rw-   0        0        0    14915 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/real_param.py
+-rw-rw-rw-   0        0        0     9812 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/relation.py
+-rw-rw-rw-   0        0        0    26769 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/relations.py
+-rw-rw-rw-   0        0        0    51472 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/report_generation_sheet_setting_att.py
+-rw-rw-rw-   0        0        0     2647 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/rule.py
+-rw-rw-rw-   0        0        0    11105 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/set_of_equation.py
+-rw-rw-rw-   0        0        0     6933 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/str_param.py
+-rw-rw-rw-   0        0        0    25620 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/tolerance_sheet_setting_att.py
+-rw-rw-rw-   0        0        0     5665 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/unit.py
+-rw-rw-rw-   0        0        0     3216 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/units.py
+-rw-rw-rw-   0        0        0    33338 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/knowledge_interfaces/units_sheet_setting_att.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.780085 pycatia-0.5.8/pycatia/mec_mod_interfaces/
+-rw-rw-rw-   0        0        0       21 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    41279 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/axis_system.py
+-rw-rw-rw-   0        0        0     4627 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/axis_systems.py
+-rw-rw-rw-   0        0        0     3400 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/bi_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     4373 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/bodies.py
+-rw-rw-rw-   0        0        0     9422 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/body.py
+-rw-rw-rw-   0        0        0     5009 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/boundary.py
+-rw-rw-rw-   0        0        0    25287 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/constraint.py
+-rw-rw-rw-   0        0        0    12680 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/constraints.py
+-rw-rw-rw-   0        0        0     6097 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/cylindrical_face.py
+-rw-rw-rw-   0        0        0     3567 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/edge.py
+-rw-rw-rw-   0        0        0     3144 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/face.py
+-rw-rw-rw-   0        0        0     1206 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/factory.py
+-rw-rw-rw-   0        0        0    13037 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/fix_together.py
+-rw-rw-rw-   0        0        0     5963 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/fix_togethers.py
+-rw-rw-rw-   0        0        0     3918 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/geometric_elements.py
+-rw-rw-rw-   0        0        0     4926 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_bodies.py
+-rw-rw-rw-   0        0        0     8987 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_body.py
+-rw-rw-rw-   0        0        0     4549 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_shape.py
+-rw-rw-rw-   0        0        0    16133 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_shape_instance.py
+-rw-rw-rw-   0        0        0     4553 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_shapes.py
+-rw-rw-rw-   0        0        0    16636 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/instance_factory.py
+-rw-rw-rw-   0        0        0     2060 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/mono_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     2249 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/not_wire_boundary_mono_dim_feat_vertex.py
+-rw-rw-rw-   0        0        0     8132 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/ordered_geometrical_set.py
+-rw-rw-rw-   0        0        0     5329 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/ordered_geometrical_sets.py
+-rw-rw-rw-   0        0        0     3919 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/origin_elements.py
+-rw-rw-rw-   0        0        0    35575 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/part.py
+-rw-rw-rw-   0        0        0     3399 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/part_document.py
+-rw-rw-rw-   0        0        0   230621 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/part_infrastructure_setting_att.py
+-rw-rw-rw-   0        0        0     9175 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/planar_face.py
+-rw-rw-rw-   0        0        0     5848 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/rectilinear_bi_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     5926 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/rectilinear_mono_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     7623 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/rectilinear_tri_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     1455 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/shape.py
+-rw-rw-rw-   0        0        0    15849 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/shape_instance.py
+-rw-rw-rw-   0        0        0     4256 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/shapes.py
+-rw-rw-rw-   0        0        0     5597 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/sketches.py
+-rw-rw-rw-   0        0        0     4694 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/solid.py
+-rw-rw-rw-   0        0        0     2895 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/tri_dim_feat_edge.py
+-rw-rw-rw-   0        0        0     2121 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/tri_dim_feat_vertex_or_bi_dim_feat_vertex.py
+-rw-rw-rw-   0        0        0     3661 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/vertex.py
+-rw-rw-rw-   0        0        0     2201 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/mec_mod_interfaces/zero_dim_feat_vertex_or_wire_boundary_mono_dim_feat_vertex.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.797750 pycatia-0.5.8/pycatia/navigator_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/navigator_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    16882 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/annotated_view.py
+-rw-rw-rw-   0        0        0     8082 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/annotated_views.py
+-rw-rw-rw-   0        0        0     5975 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/dmu_data_flow.py
+-rw-rw-rw-   0        0        0     3443 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/dmu_review.py
+-rw-rw-rw-   0        0        0     8361 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/dmu_reviews.py
+-rw-rw-rw-   0        0        0    15722 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/group.py
+-rw-rw-rw-   0        0        0     7821 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/groups.py
+-rw-rw-rw-   0        0        0     5487 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/hyperlink.py
+-rw-rw-rw-   0        0        0     7787 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/hyperlinks.py
+-rw-rw-rw-   0        0        0    17112 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/marker_2D.py
+-rw-rw-rw-   0        0        0    18792 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/marker_2Ds.py
+-rw-rw-rw-   0        0        0    21466 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/marker_3D.py
+-rw-rw-rw-   0        0        0     9076 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/marker_3Ds.py
+-rw-rw-rw-   0        0        0    71610 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/marker_setting_att.py
+-rw-rw-rw-   0        0        0   196711 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/n_4D_navigator_setting_att.py
+-rw-rw-rw-   0        0        0    15489 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/navigator_interfaces/navigator_workbench.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.873368 pycatia-0.5.8/pycatia/part_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/part_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/add.py
+-rw-rw-rw-   0        0        0     3086 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/affinity.py
+-rw-rw-rw-   0        0        0     3477 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/angular_repartition.py
+-rw-rw-rw-   0        0        0     1542 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/assemble.py
+-rw-rw-rw-   0        0        0     7140 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/auto_draft.py
+-rw-rw-rw-   0        0        0    11415 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/auto_fillet.py
+-rw-rw-rw-   0        0        0     3130 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/axis_to_axis.py
+-rw-rw-rw-   0        0        0     5010 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/boolean_shape.py
+-rw-rw-rw-   0        0        0    12638 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/chamfer.py
+-rw-rw-rw-   0        0        0    21249 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/circ_pattern.py
+-rw-rw-rw-   0        0        0    20731 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/close_surface.py
+-rw-rw-rw-   0        0        0     7827 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/const_rad_edge_fillet.py
+-rw-rw-rw-   0        0        0     2913 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/defeaturing.py
+-rw-rw-rw-   0        0        0     1450 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/defeaturing_fillet_filter.py
+-rw-rw-rw-   0        0        0     1220 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/defeaturing_filter.py
+-rw-rw-rw-   0        0        0    16497 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/defeaturing_filter_with_range.py
+-rw-rw-rw-   0        0        0     5942 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/defeaturing_filters.py
+-rw-rw-rw-   0        0        0     1440 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/defeaturing_hole_filter.py
+-rw-rw-rw-   0        0        0     4452 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/draft.py
+-rw-rw-rw-   0        0        0    17507 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/draft_domain.py
+-rw-rw-rw-   0        0        0     3348 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/draft_domains.py
+-rw-rw-rw-   0        0        0     1559 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/dress_up_shape.py
+-rw-rw-rw-   0        0        0     8029 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/edge_fillet.py
+-rw-rw-rw-   0        0        0     4637 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/face_fillet.py
+-rw-rw-rw-   0        0        0     4170 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/fillet.py
+-rw-rw-rw-   0        0        0     1679 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/groove.py
+-rw-rw-rw-   0        0        0    29934 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/hole.py
+-rw-rw-rw-   0        0        0     2066 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/intersect.py
+-rw-rw-rw-   0        0        0     3457 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/limit.py
+-rw-rw-rw-   0        0        0     2624 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/linear_repartition.py
+-rw-rw-rw-   0        0        0     2457 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/loft.py
+-rw-rw-rw-   0        0        0     3395 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/mirror.py
+-rw-rw-rw-   0        0        0     1565 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/pad.py
+-rw-rw-rw-   0        0        0     5497 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/pattern.py
+-rw-rw-rw-   0        0        0     1658 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/pocket.py
+-rw-rw-rw-   0        0        0    16072 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/prism.py
+-rw-rw-rw-   0        0        0    22765 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/rect_pattern.py
+-rw-rw-rw-   0        0        0     1399 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/remove.py
+-rw-rw-rw-   0        0        0     7954 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/remove_face.py
+-rw-rw-rw-   0        0        0     2273 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/repartition.py
+-rw-rw-rw-   0        0        0     6941 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/replace_face.py
+-rw-rw-rw-   0        0        0     8638 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/revolution.py
+-rw-rw-rw-   0        0        0     1588 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/rib.py
+-rw-rw-rw-   0        0        0     5240 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/rotate.py
+-rw-rw-rw-   0        0        0     3629 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/scaling.py
+-rw-rw-rw-   0        0        0     4474 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/scaling2.py
+-rw-rw-rw-   0        0        0    10146 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/sew_surface.py
+-rw-rw-rw-   0        0        0     1671 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/shaft.py
+-rw-rw-rw-   0        0        0   160771 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/shape_factory.py
+-rw-rw-rw-   0        0        0    13741 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/shell.py
+-rw-rw-rw-   0        0        0     3738 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/sketch_based_shape.py
+-rw-rw-rw-   0        0        0     1677 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/slot.py
+-rw-rw-rw-   0        0        0     6529 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/solid_combine.py
+-rw-rw-rw-   0        0        0     2669 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/split.py
+-rw-rw-rw-   0        0        0     7359 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/stiffener.py
+-rw-rw-rw-   0        0        0     2183 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/surface_based_shape.py
+-rw-rw-rw-   0        0        0    12593 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/sweep.py
+-rw-rw-rw-   0        0        0     2776 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/symmetry.py
+-rw-rw-rw-   0        0        0     4871 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/thick_surface.py
+-rw-rw-rw-   0        0        0    12606 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/thickness.py
+-rw-rw-rw-   0        0        0    12918 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/thread.py
+-rw-rw-rw-   0        0        0     1609 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/transformation_shape.py
+-rw-rw-rw-   0        0        0     2847 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/translate.py
+-rw-rw-rw-   0        0        0    19000 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/trim.py
+-rw-rw-rw-   0        0        0     5338 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/tritangent_fillet.py
+-rw-rw-rw-   0        0        0     4454 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/user_pattern.py
+-rw-rw-rw-   0        0        0     3581 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/user_repartition.py
+-rw-rw-rw-   0        0        0    16156 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/part_interfaces/var_rad_edge_fillet.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.881368 pycatia-0.5.8/pycatia/product_structure_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/product_structure_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     8690 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/product_structure_interfaces/analyze.py
+-rw-rw-rw-   0        0        0     4920 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/product_structure_interfaces/assembly_convertor.py
+-rw-rw-rw-   0        0        0    56658 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/product_structure_interfaces/product.py
+-rw-rw-rw-   0        0        0     2752 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/product_structure_interfaces/product_document.py
+-rw-rw-rw-   0        0        0    17282 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/product_structure_interfaces/products.py
+-rw-rw-rw-   0        0        0     3594 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/product_structure_interfaces/publication.py
+-rw-rw-rw-   0        0        0    10017 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/product_structure_interfaces/publications.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.885575 pycatia-0.5.8/pycatia/scripts/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/scripts/__init__.py
+-rw-rw-rw-   0        0        0      388 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/scripts/checking.py
+-rw-rw-rw-   0        0        0     2916 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/scripts/csv_tools.py
+-rw-rw-rw-   0        0        0      991 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/scripts/document_types.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.900087 pycatia-0.5.8/pycatia/sketcher_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     2854 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/axis_2D.py
+-rw-rw-rw-   0        0        0     5295 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/circle_2D.py
+-rw-rw-rw-   0        0        0     5482 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/control_point_2D.py
+-rw-rw-rw-   0        0        0    17525 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/curve_2D.py
+-rw-rw-rw-   0        0        0     8859 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/ellipse_2D.py
+-rw-rw-rw-   0        0        0    20999 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/factory_2D.py
+-rw-rw-rw-   0        0        0     1863 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/geometric_element.py
+-rw-rw-rw-   0        0        0     2659 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/geometry_2D.py
+-rw-rw-rw-   0        0        0     6788 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/hyperbola_2D.py
+-rw-rw-rw-   0        0        0     5201 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/line_2D.py
+-rw-rw-rw-   0        0        0     5926 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/parabola_2D.py
+-rw-rw-rw-   0        0        0     3233 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/point_2D.py
+-rw-rw-rw-   0        0        0    13726 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/sketch.py
+-rw-rw-rw-   0        0        0     5391 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/sketcher_interfaces/spline_2D.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.923194 pycatia-0.5.8/pycatia/space_analyses_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    13227 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/clash.py
+-rw-rw-rw-   0        0        0     3448 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/clash_result.py
+-rw-rw-rw-   0        0        0     7191 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/clash_results.py
+-rw-rw-rw-   0        0        0     6989 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/clashes.py
+-rw-rw-rw-   0        0        0    12155 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/conflict.py
+-rw-rw-rw-   0        0        0     3179 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/conflicts.py
+-rw-rw-rw-   0        0        0    21840 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/distance.py
+-rw-rw-rw-   0        0        0     7294 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/distances.py
+-rw-rw-rw-   0        0        0      227 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/general_functions.py
+-rw-rw-rw-   0        0        0    15124 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/inertia.py
+-rw-rw-rw-   0        0        0     6662 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/inertias.py
+-rw-rw-rw-   0        0        0    25608 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/measurable.py
+-rw-rw-rw-   0        0        0    28720 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/measure_setting_att.py
+-rw-rw-rw-   0        0        0    21497 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/section.py
+-rw-rw-rw-   0        0        0    81518 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/sectioning_setting_att.py
+-rw-rw-rw-   0        0        0     7207 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/sections.py
+-rw-rw-rw-   0        0        0     8178 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/space_analyses_interfaces/spa_workbench.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.949304 pycatia-0.5.8/pycatia/system_interfaces/
+-rw-rw-rw-   0        0        0       23 2023-05-01 08:31:08.000000 pycatia-0.5.8/pycatia/system_interfaces/__init__.py
+-rw-rw-rw-   0        0        0     1915 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/accesslog_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     7750 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/any_object.py
+-rw-rw-rw-   0        0        0    28964 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/cache_setting_att.py
+-rw-rw-rw-   0        0        0     1666 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/cat_base_dispatch.py
+-rw-rw-rw-   0        0        0     1530 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/cat_base_unknown.py
+-rw-rw-rw-   0        0        0     8904 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/collection.py
+-rw-rw-rw-   0        0        0     1901 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/command_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     7521 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/disconnection_setting_att.py
+-rw-rw-rw-   0        0        0    23652 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/dl_name_setting_att.py
+-rw-rw-rw-   0        0        0    12275 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/dyn_license_setting_att.py
+-rw-rw-rw-   0        0        0     9646 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/errorlog_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     1920 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/file_access_statistics_setting_att.py
+-rw-rw-rw-   0        0        0    21080 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/general_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     7896 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/global_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     1257 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/i_dispatch.py
+-rw-rw-rw-   0        0        0     1147 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/i_unknown.py
+-rw-rw-rw-   0        0        0    29377 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/license_setting_att.py
+-rw-rw-rw-   0        0        0    10573 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/memory_warning_setting_att.py
+-rw-rw-rw-   0        0        0     2732 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/pcs_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     1895 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/server_statistics_setting_att.py
+-rw-rw-rw-   0        0        0     1901 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/session_statistics_setting_att.py
+-rw-rw-rw-   0        0        0    12823 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/setting_controller.py
+-rw-rw-rw-   0        0        0    13614 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/setting_repository.py
+-rw-rw-rw-   0        0        0    12706 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/system_service.py
+-rw-rw-rw-   0        0        0     1914 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/system_interfaces/workbench_statistics_setting_att.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:34.018381 pycatia-0.5.8/pycatia/tps_interfaces/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/tps_interfaces/__init__.py
+-rw-rw-rw-   0        0        0    32496 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/annotation.py
+-rw-rw-rw-   0        0        0    20353 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/annotation_2.py
+-rw-rw-rw-   0        0        0    20429 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/annotation_factory.py
+-rw-rw-rw-   0        0        0    22390 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/annotation_factory_2.py
+-rw-rw-rw-   0        0        0    15049 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/annotation_set.py
+-rw-rw-rw-   0        0        0     2576 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/annotation_set_transform_into_assembly_set.py
+-rw-rw-rw-   0        0        0     3708 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/annotation_sets.py
+-rw-rw-rw-   0        0        0     4109 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/annotations.py
+-rw-rw-rw-   0        0        0     3005 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/assembly_annotation_sets.py
+-rw-rw-rw-   0        0        0     2717 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/associated_ref_frame.py
+-rw-rw-rw-   0        0        0    11972 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/capture.py
+-rw-rw-rw-   0        0        0     2067 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/capture_factory.py
+-rw-rw-rw-   0        0        0     2163 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/captures.py
+-rw-rw-rw-   0        0        0     2309 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/composite_tolerance.py
+-rw-rw-rw-   0        0        0     1772 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/controlled_radius.py
+-rw-rw-rw-   0        0        0     2553 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/datum_simple.py
+-rw-rw-rw-   0        0        0    11766 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/datum_target.py
+-rw-rw-rw-   0        0        0     3526 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/default_annotation.py
+-rw-rw-rw-   0        0        0    10599 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/dimension_3d.py
+-rw-rw-rw-   0        0        0     6363 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/dimension_limit.py
+-rw-rw-rw-   0        0        0     1642 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/dimension_pattern.py
+-rw-rw-rw-   0        0        0    20046 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/dmu_tol_setting_att.py
+-rw-rw-rw-   0        0        0     1663 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/envelope_condition.py
+-rw-rw-rw-   0        0        0     9455 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/flag_note.py
+-rw-rw-rw-   0        0        0     1761 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/free_state.py
+-rw-rw-rw-   0        0        0    70472 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/fta_infra_setting_att.py
+-rw-rw-rw-   0        0        0   241089 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/fta_setting_att.py
+-rw-rw-rw-   0        0        0     1671 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/material_condition.py
+-rw-rw-rw-   0        0        0    11475 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/noa.py
+-rw-rw-rw-   0        0        0     1767 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/non_semantic_datum.py
+-rw-rw-rw-   0        0        0     3225 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/non_semantic_datum_target.py
+-rw-rw-rw-   0        0        0     3380 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/non_semantic_dimension.py
+-rw-rw-rw-   0        0        0     1736 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/non_semantic_gdt.py
+-rw-rw-rw-   0        0        0     1941 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/particular_tol_elem.py
+-rw-rw-rw-   0        0        0     5589 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/projected_tolerance_zone.py
+-rw-rw-rw-   0        0        0    14665 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/reference_frame.py
+-rw-rw-rw-   0        0        0     6101 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/roughness.py
+-rw-rw-rw-   0        0        0    18486 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/semantic_gdt.py
+-rw-rw-rw-   0        0        0     6901 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/shifted_profile_tolerance.py
+-rw-rw-rw-   0        0        0     1785 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/tangent_plane.py
+-rw-rw-rw-   0        0        0     2788 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/text.py
+-rw-rw-rw-   0        0        0     2203 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/tolerance_per_unit_basis_restrictive_value.py
+-rw-rw-rw-   0        0        0     3066 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/tolerance_unit_basis_value.py
+-rw-rw-rw-   0        0        0     2349 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/tolerance_zone.py
+-rw-rw-rw-   0        0        0     2553 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/tps_parallel_on_screen.py
+-rw-rw-rw-   0        0        0     1221 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/tps_view.py
+-rw-rw-rw-   0        0        0     2659 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/tps_view_factory.py
+-rw-rw-rw-   0        0        0     2208 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/tps_views.py
+-rw-rw-rw-   0        0        0     6298 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/user_surface.py
+-rw-rw-rw-   0        0        0     7897 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/user_surfaces.py
+-rw-rw-rw-   0        0        0     2204 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/tps_interfaces/weld.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:34.021381 pycatia-0.5.8/pycatia/types/
+-rw-rw-rw-   0        0        0        0 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/types/__init__.py
+-rw-rw-rw-   0        0        0      584 2022-11-18 10:48:10.000000 pycatia-0.5.8/pycatia/types/document_types.py
+-rw-rw-rw-   0        0        0      560 2022-04-12 12:15:17.000000 pycatia-0.5.8/pycatia/types/general.py
+-rw-rw-rw-   0        0        0       19 2023-05-01 08:46:40.000000 pycatia-0.5.8/pycatia/version.py
+drwxrwxrwx   0        0        0        0 2023-05-01 09:47:33.437188 pycatia-0.5.8/pycatia.egg-info/
+-rw-rw-rw-   0        0        0     4853 2023-05-01 09:47:33.000000 pycatia-0.5.8/pycatia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    25596 2023-05-01 09:47:33.000000 pycatia-0.5.8/pycatia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-01 09:47:33.000000 pycatia-0.5.8/pycatia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-01 09:47:33.000000 pycatia-0.5.8/pycatia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-01 09:47:33.000000 pycatia-0.5.8/pycatia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-01 09:47:34.022381 pycatia-0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-05-01 08:31:08.000000 pycatia-0.5.8/setup.py
```

### Comparing `pycatia-0.5.7/LICENSE.txt` & `pycatia-0.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/PKG-INFO` & `pycatia-0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatia
-Version: 0.5.7
+Version: 0.5.8
 Summary: A python module to access the CATIA Measurable object.
 Home-page: https://github.com/evereux/pycatia
 Author: Paul Bourne
 Author-email: evereux@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycatia-0.5.7/README.rst` & `pycatia-0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/__init__.py` & `pycatia-0.5.8/pycatia/__init__.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/base_interfaces/context.py` & `pycatia-0.5.8/pycatia/base_interfaces/context.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/cat_logger.py` & `pycatia-0.5.8/pycatia/cat_logger.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/cat_mat_interfaces/analysis_material.py` & `pycatia-0.5.8/pycatia/cat_mat_interfaces/analysis_material.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/cat_mat_interfaces/material.py` & `pycatia-0.5.8/pycatia/cat_mat_interfaces/material.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/cat_mat_interfaces/material_document.py` & `pycatia-0.5.8/pycatia/cat_mat_interfaces/material_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/cat_mat_interfaces/material_families.py` & `pycatia-0.5.8/pycatia/cat_mat_interfaces/material_families.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/cat_mat_interfaces/material_family.py` & `pycatia-0.5.8/pycatia/cat_mat_interfaces/material_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/cat_mat_interfaces/material_manager.py` & `pycatia-0.5.8/pycatia/cat_mat_interfaces/material_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/cat_mat_interfaces/materials.py` & `pycatia-0.5.8/pycatia/cat_mat_interfaces/materials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/cat_mat_interfaces/positioned_material.py` & `pycatia-0.5.8/pycatia/cat_mat_interfaces/positioned_material.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/cat_rma_interfaces/rendering_material.py` & `pycatia-0.5.8/pycatia/cat_rma_interfaces/rendering_material.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drafting_setting_att.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drafting_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_arrow.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_arrow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_arrows.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_arrows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_component.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_components.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dim_ext_line.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dim_ext_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dim_line.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dim_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dim_value.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dim_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dimension.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_dimensions.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_dimensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_document.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_leader.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_leader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_leaders.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_leaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_page_setup.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_page_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_picture.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_picture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_pictures.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_pictures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_root.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_root.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_sheet.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_sheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_sheets.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_sheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_table.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_tables.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_text.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_text_properties.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_text_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_text_range.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_text_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_texts.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_texts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_thread.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_threads.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_threads.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_view.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_view_generative_behavior.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_view_generative_behavior.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_view_generative_links.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_view_generative_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_views.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_welding.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_welding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/drawing_weldings.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/drawing_weldings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/drafting_interfaces/print_area.py` & `pycatia-0.5.8/pycatia/drafting_interfaces/print_area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/enumeration/enumeration_types.py` & `pycatia-0.5.8/pycatia/enumeration/enumeration_types.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_actions_group.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_actions_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_actions_groups.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_actions_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_association.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_association.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_associations.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_associations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_facet_managers.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_facet_managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_gen_script_mgr.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_gen_script_mgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_multi_rep_mgr.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_multi_rep_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_node_graph_layout.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_node_graph_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_script.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/funct_scripts.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/funct_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_action.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_actions.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_description.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_document.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_element.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_facet.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_facet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_facet_mgr.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_facet_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_object.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_object_proxy.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_object_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_objects.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_position.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_system_setting_att.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_system_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_variant.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_variant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/funct_system_interfaces/functional_variants.py` & `pycatia-0.5.8/pycatia/funct_system_interfaces/functional_variants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_3d_curve_offset.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_3d_curve_offset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_affinity.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_affinity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_assemble.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_assemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_line.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_to_axis.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_axis_to_axis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_blend.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_blend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_boundary.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_bump.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_bump.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle2_points_rad.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle2_points_rad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle3_points.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle3_points.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_point.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_radius.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_bitangent_radius.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_axis.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_axis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_tangent.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_center_tangent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_pt.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_pt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_rad.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_ctr_rad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_explicit.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_explicit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_tritangent.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_circle_tritangent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_combine.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_combine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_conic.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_conic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_connect.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_corner.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_corner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_explicit.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_explicit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_par.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_par.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_smooth.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_curve_smooth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_cylinder.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_cylinder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_develop.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_develop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_direction.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_direction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extract.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extract_multi.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extract_multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extrapol.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extrapol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum_polar.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extremum_polar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_extrude.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_extrude.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
@@ -299,15 +299,15 @@
     
     @first_upto_element.setter
     def first_upto_element(self, reference_element: Reference):
         """
         :param Reference reference_element:
         """
 
-        self.hybrid_shape_extrude.FirstUptoElement = reference_element
+        self.hybrid_shape_extrude.FirstUptoElement = reference_element.com_object
 
     @property
     def orientation(self) -> bool:
         """
         .. note::
             :class: toggle
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_factory.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
-        
+
 """
 
 from pycatia.hybrid_shape_interfaces.hybrid_shape_3d_curve_offset import HybridShape3DCurveOffset
 from pycatia.hybrid_shape_interfaces.hybrid_shape_affinity import HybridShapeAffinity
 from pycatia.hybrid_shape_interfaces.hybrid_shape_assemble import HybridShapeAssemble
 from pycatia.hybrid_shape_interfaces.hybrid_shape_axis_line import HybridShapeAxisLine
 from pycatia.hybrid_shape_interfaces.hybrid_shape_axis_to_axis import HybridShapeAxisToAxis
@@ -124,32 +124,32 @@
                 | System.IUnknown
                 |     System.IDispatch
                 |         System.CATBaseUnknown
                 |             System.CATBaseDispatch
                 |                 System.AnyObject
                 |                     MecModInterfaces.Factory
                 |                         HybridShapeFactory
-                | 
+                |
                 | Interface to create all kinds of HybridShape objects that may be needed in
                 | wireframe and surface design.
-                | 
+                |
                 | Note:
                 | This interface concern GSD/GSO/DL1 feature creation via VB
                 | Use of the creation methods requires to have granted license configuration for
                 | feature creation
                 | i.e:
                 | - Bump, Develop,WrapCurve,WrapSurface require GSO license.
                 | - Unfold, Develop require DL1 license.
                 | - Other require GSD license.
                 | Note2:
                 | For all methods creating datums AddNew*Datum,
                 | the object passed as parameter to create the datum has to be in the current
                 | container.
                 | Otherwise, an error occurs.
-    
+
     """
 
     def __init__(self, com_object):
         super().__init__(com_object)
         self.hybrid_shape_factory = com_object
 
     def add_new3_d_corner(self, i_element1: Reference, i_element2: Reference, i_direction: HybridShapeDirection,
@@ -162,39 +162,39 @@
                 | o Func AddNew3DCorner(Reference iElement1,
                 | Reference iElement2,
                 | HybridShapeDirection iDirection,
                 | double iRadius,
                 | long iOrientation1,
                 | long iOrientation2,
                 | boolean iTrim) As HybridShapeCorner
-                | 
+                |
                 |     Creates a new 3D Corner within the current body.
                 |     Create a 3D corner curve between a point and a curve or 2 curves along a
                 |     direction.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement1
-                |             First reference curve. 
+                |             First reference curve.
                 |         iElement2
-                |             Second reference curve. 
+                |             Second reference curve.
                 |         iDirection
-                |             Direction. 
+                |             Direction.
                 |         iRadius
-                |             Radius of the corner. 
+                |             Radius of the corner.
                 |         iOrientation1
                 |             Manage the corner center position. Value can be 1 or -1
-                |             
+                |
                 |         iOrientation2
                 |             Manage the corner center position. Value can be 1 or -1
-                |             
+                |
                 |         iTrim
                 |             Value can be FALSE or TRUE
                 |             if TRUE the 2 curves are trimed and asembled with the corner.
-                |             
+                |
                 |         oCorner
                 |             Created corner.
 
         :param Reference i_element1:
         :param Reference i_element2:
         :param HybridShapeDirection i_direction:
         :param float i_radius:
@@ -216,30 +216,30 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNew3DCurveOffset(Reference iCurveToOffset,
                 | HybridShapeDirection iDirection,
                 | double iOffset,
                 | double iCornerRadius,
                 | double iCornerTension) As HybridShape3DCurveOffset
-                | 
+                |
                 |     Creates a 3D Curve Offset.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
-                |             The curve to offset 
+                |             The curve to offset
                 |         iDirection
-                |             Offset pulling direction. 
+                |             Offset pulling direction.
                 |         iOffsetValue
-                |             Offset Value. 
+                |             Offset Value.
                 |         iCornerRadius
-                |             Radius of the 3D corners. 
+                |             Radius of the 3D corners.
                 |         iCornerTension
-                |             Tension of the 3D corners. 
-                | 
+                |             Tension of the 3D corners.
+                |
                 |     Returns:
                 |         CATIGSM3DCurveOffset_var created 3DCurveOffset.
 
         :param Reference i_curve_to_offset:
         :param HybridShapeDirection i_direction:
         :param float i_offset:
         :param float i_corner_radius:
@@ -258,31 +258,31 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewAffinity(Reference iElement,
                 | double iXRatio,
                 | double iYRatio,
                 | double iZRatio) As HybridShapeAffinity
-                | 
+                |
                 |     Creates a new Affinity within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement
                 |             point, curve, surface or solid.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, TriDimFeatEdge, BiDimFeatEdge and Vertex.
-                |         
+                |
                 |     iXRatio
-                |         Ratio of affinity in iX direction. 
+                |         Ratio of affinity in iX direction.
                 |     iYRatio
-                |         Ratio of affinity in iY direction. 
+                |         Ratio of affinity in iY direction.
                 |     iZRatio
-                |         Ratio of affinity in iZ direction. 
+                |         Ratio of affinity in iZ direction.
                 |     oAffinity
                 |         Created affinity
 
         :param Reference i_element:
         :param float i_x_ratio:
         :param float i_y_ratio:
         :param float i_z_ratio:
@@ -296,22 +296,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewAxisLine(Reference iElement) As
                 | HybridShapeAxisLine
-                | 
+                |
                 |     Creates a new AxisLine within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement
                 |             Circle, Ellipse, Oblong, Sphere, Revolution surface. Axis is
-                |             computed for this element 
+                |             computed for this element
                 |         oAxisLine
                 |             Created axis line
 
         :param Reference i_element:
         :return: HybridShapeAxisLine
         :rtype: HybridShapeAxisLine
         """
@@ -323,26 +323,26 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewAxisToAxis(Reference iObject,
                 | Reference iReferenceAxis,
                 | Reference iTargetAxis) As HybridShapeAxisToAxis
-                | 
+                |
                 |     Creates a new axis to axis transformation within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
-                |             Point, curve, surface or solid to transform. 
+                |             Point, curve, surface or solid to transform.
                 |         iReferenceAxis
-                |             reference axis system 
+                |             reference axis system
                 |         iTargetAxis
-                |             target axis system 
+                |             target axis system
                 |         oAxisToAxis
                 |             Created axis to axis transformation.
 
         :param Reference i_object:
         :param Reference i_reference_axis:
         :param Reference i_target_axis:
         :return: HybridShapeAxisToAxis
@@ -355,19 +355,19 @@
     def add_new_blend(self) -> HybridShapeBlend:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewBlend() As HybridShapeBlend
-                | 
+                |
                 |     Creates a new blend surface within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oBlend
                 |             The Blend object if succeded
 
         :return: HybridShapeBlend
         :rtype: HybridShapeBlend
         """
         return HybridShapeBlend(self.hybrid_shape_factory.AddNewBlend())
@@ -378,36 +378,36 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewBoundary(Reference iInitialElement,
                 | Reference iSupport,
                 | long iTypedePropagation) As HybridShapeBoundary
-                | 
+                |
                 |     Creates a new Boundary within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iInitialElement
                 |             the element used to initialise the propagation around the
                 |             surface
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see BiDimFeatEdge. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see BiDimFeatEdge.
                 |     iSupport
                 |         the surface used to compute the boundary around it
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iTypedePropagation
                 |         Propagation type the values are: 0 for Boundary for all edges 1 for
                 |         Boundary propagation for edges on connexe point 2 for Boundary propagation for
                 |         edges tangent at point breaks 3 for Boundary not propagation from the current
-                |         edge 
+                |         edge
                 |     oBoundary
                 |         The computed element
 
         :param Reference i_initial_element:
         :param Reference i_support:
         :param int i_typede_propagation:
         :return: HybridShapeBoundary
@@ -421,22 +421,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewBoundaryOfSurface(Reference Surface) As
                 | HybridShapeBoundary
-                | 
+                |
                 |     Creates a Boundary within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSurface
                 |             the feature on which all the boundaries will be computed
-                |             
+                |
                 |         oBoundary
                 |             the whole boundary of the Surface given in first
                 |             parameter
 
         :param Reference surface:
         :return: HybridShapeBoundary
         :rtype: HybridShapeBoundary
@@ -446,22 +446,22 @@
     def add_new_bump(self, i_body_to_bump: Reference) -> HybridShapeBump:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewBump(Reference iBodyToBump) As HybridShapeBump
-                | 
+                |
                 |     Creates a new Bump within the current body.
                 |     Note: require GSO license.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         :
-                |             iBodyToBump Body to deform witn a Bump 
+                |             iBodyToBump Body to deform witn a Bump
                 |         :
                 |             oBump Bump result
 
         :param Reference i_body_to_bump:
         :return: HybridShapeBump
         :rtype: HybridShapeBump
         """
@@ -476,42 +476,42 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircle2PointsRad(Reference iPoint1,
                 | Reference iPoint2,
                 | Reference iSupport,
                 | boolean iGeodesic,
                 | double iRadius,
                 | long iOri) As HybridShapeCircle2PointsRad
-                | 
+                |
                 |     Creates a new Circle passing through 2 points with a radius within the
                 |     current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPoint1
                 |             first passing point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iPoint2
                 |         second passing point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iSupport
                 |         support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iGeodesic
-                |         Puts the circle on the surface. 
+                |         Puts the circle on the surface.
                 |     iRadius
                 |         Value specified is considered as radius. To use this value as diameter,
-                |         set DiameterMode using SetDiameterMode method 
+                |         set DiameterMode using SetDiameterMode method
                 |     iOri
                 |         circle orientation. Defines the side where circle is computed using the
                 |         normal direction of line between the 2 passing points.
-                |         
+                |
                 |     oCircle
                 |         The Circle object if succeeded
 
         :param Reference i_point1:
         :param Reference i_point2:
         :param Reference i_support:
         :param bool i_geodesic:
@@ -530,25 +530,25 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircle3Points(Reference iPoint1,
                 | Reference iPoint2,
                 | Reference iPoint3) As HybridShapeCircle3Points
-                | 
+                |
                 |     Creates a new circle passing through 3 points within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPoint1
                 |             first passing point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iPoint2
                 |         second passing point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iPoint3
                 |         third passing point.
                 |         Sub-element(s) supported (see Boundary object): see
@@ -576,42 +576,42 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleBitangentPoint(Reference iCurve1,
                 | Reference iCurve2,
                 | Reference iPoint,
                 | Reference iSupport,
                 | long iOri1,
                 | long iOri2) As HybridShapeCircleBitangentPoint
-                | 
+                |
                 |     Creates a new circle tangent to 2 curves and passing through one point
                 |     within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve1
                 |             first curve to which the circle will be tangent.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iCurve2
                 |         second curve to which the circle will be tangent.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge and
                 |         BiDimFeatEdge.
                 |     iPoint
                 |         passing point. This point must lie on second curve.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iSupport
                 |         support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iOri1
-                |         first curve orientation for circle computation. 
+                |         first curve orientation for circle computation.
                 |     iOri2
-                |         second curve orientation for circle computation. 
+                |         second curve orientation for circle computation.
                 |     oCircle
                 |         Created circle
 
         :param Reference i_curve1:
         :param Reference i_curve2:
         :param Reference i_point:
         :param Reference i_support:
@@ -634,41 +634,41 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleBitangentRadius(Reference iCurve1,
                 | Reference iCurve2,
                 | Reference iSupport,
                 | double iRadius,
                 | long iOri1,
                 | long iOri2) As HybridShapeCircleBitangentRadius
-                | 
+                |
                 |     Creates a new circle tangent to 2 curves and with a radius within the
                 |     current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve1
                 |             first curve to which the circle will be tangent.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iCurve2
                 |         second curve to which the circle will be tangent.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge and
                 |         BiDimFeatEdge.
                 |     iSupport
                 |         support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iRadius
                 |         Value specified is considered as radius. To use this value as diameter,
-                |         set DiameterMode using SetDiameterMode method 
+                |         set DiameterMode using SetDiameterMode method
                 |     iOri1
-                |         first curve orientation for circle computation. 
+                |         first curve orientation for circle computation.
                 |     iOri2
-                |         second curve orientation for circle computation. 
+                |         second curve orientation for circle computation.
                 |     oCircle
                 |         Created circle
 
         :param Reference i_curve1:
         :param Reference i_curve2:
         :param Reference i_support:
         :param float i_radius:
@@ -688,27 +688,27 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleCenterAxis(Reference iAxis,
                 | Reference iPoint,
                 | double iValue,
                 | boolean iProjection) As HybridShapeCircleCenterAxis
-                | 
+                |
                 |     Creates a circle from point and axis.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iAxis
-                |             Axis of plane in which circle is lying 
+                |             Axis of plane in which circle is lying
                 |         iPoint
                 |             Point used for center computation. It will be the center if ProjectionMode is False.
                 |             If ProjectionMode = True, this point will be projected on to axis/line
                 |         iValue
                 |             Value specified is considered as radius. To use this value as
-                |             diameter, set DiameterMode property 
+                |             diameter, set DiameterMode property
                 |         iProjection
                 |             Sets Projection Mode. ProjectionMode = TRUE implies point will be projected on to
                 |             axis/line, ProjectionMode = FALSE implies that point will be center of the circle.
                 |         oCircle
                 |             Created circle
 
         :param Reference i_axis:
@@ -732,38 +732,38 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleCenterAxisWithAngles(Reference iAxis,
                 | Reference iPoint,
                 | double iValue,
                 | boolean iProjection,
                 | double iStartAngle,
                 | double iEndAngle) As HybridShapeCircleCenterAxis
-                | 
+                |
                 |     Creates a circle from point and axis.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iAxis
                 |             Axis of plane in which circle is lying
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object):
                 |     iPoint
                 |         Point used for center computation. It will be the center if ProjectionMode is False.
                 |         If ProjectionMode = True, this point will be projected on to axis/line
                 |         Sub-element(s) supported (see Boundary object):
                 |     iValue
                 |         Value specified is considered as radius. To use this value as diameter,
-                |         set DiameterMode property 
+                |         set DiameterMode property
                 |     iProjection
                 |         Sets Projection Mode. ProjectionMode = TRUE implies point will be projected on to axis/line,
                 |         ProjectionMode = FALSE implies that point will be center of the circle.
                 |     iStartAngle
-                |         start angle 
+                |         start angle
                 |     iEndAngle
-                |         end angle 
+                |         end angle
                 |     oCircle
                 |         Created circle
 
         :param Reference i_axis:
         :param Reference i_point:
         :param float i_value:
         :param bool i_projection:
@@ -783,30 +783,30 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleCenterTangent(Reference iCenterElem,
                 | Reference iTangentCurve,
                 | Reference iSupport,
                 | double iRadius) As HybridShapeCircleCenterTangent
-                | 
+                |
                 |     Creates a new circle with given center element and tangent
                 |     curve.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCenterElem
-                |             Can be either curve or point. 
+                |             Can be either curve or point.
                 |         iTangentCurve
-                |             Curve to which the circle will be tangent. 
+                |             Curve to which the circle will be tangent.
                 |         iSupport
-                |             support surface or plane. 
+                |             support surface or plane.
                 |         iRadius
                 |             circle radius, valid only if center element is curve. Value
                 |             specified is considered as radius. To use this value as diameter, set
-                |             DiameterMode using SetDiameterMode method 
+                |             DiameterMode using SetDiameterMode method
                 |         oCircle
                 |             Created circle
 
         :param Reference i_center_elem:
         :param Reference i_tangent_curve:
         :param Reference i_support:
         :param float i_radius:
@@ -824,35 +824,35 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleCtrPt(Reference iCenter,
                 | Reference iCrossingPoint,
                 | Reference iSupport,
                 | boolean iGeodesic) As HybridShapeCircleCtrPt
-                | 
+                |
                 |     Creates a new whole circle defined by its center, a passing point within
                 |     the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCenter
                 |             circle center.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iCrossingPoint
                 |         passing point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iSupport
                 |         support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iGeodesic
-                |         Puts the circle on the surface. 
+                |         Puts the circle on the surface.
                 |     oCircle
                 |         CreatedCircle
 
         :param Reference i_center:
         :param Reference i_crossing_point:
         :param Reference i_support:
         :param bool i_geodesic:
@@ -873,39 +873,39 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleCtrPtWithAngles(Reference iCenter,
                 | Reference iCrossingPoint,
                 | Reference iSupport,
                 | boolean iGeodesic,
                 | double iStartAngle,
                 | double iEndAngle) As HybridShapeCircleCtrPt
-                | 
+                |
                 |     Creates a new circle defined by its center, a passing point and angles
                 |     within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCenter
                 |             circle center.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iCrossingPoint
                 |         passing point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iSupport
                 |         support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iGeodesic
-                |         Puts the circle on the surface. 
+                |         Puts the circle on the surface.
                 |     iStartAngle
-                |         start angle 
+                |         start angle
                 |     iEndAngle
-                |         end angle 
+                |         end angle
                 |     oCircle
                 |         Created circle
 
         :param Reference i_center:
         :param Reference i_crossing_point:
         :param Reference i_support:
         :param bool i_geodesic:
@@ -926,34 +926,34 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleCtrRad(Reference iCenter,
                 | Reference iSupport,
                 | boolean iGeodesic,
                 | double iRadius) As HybridShapeCircleCtrRad
-                | 
+                |
                 |     Creates a new whole circle defined by its center and a radius within the
                 |     current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCenter
                 |             circle center.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iSupport
                 |         support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iGeodesic
-                |         Puts the circle on the surface. 
+                |         Puts the circle on the surface.
                 |     iRadius
                 |         Value specified is considered as radius. To use this value as diameter,
-                |         set DiameterMode using SetDiameterMode method 
+                |         set DiameterMode using SetDiameterMode method
                 |     oCircle
                 |         Created circle
 
         :param Reference i_center:
         :param Reference i_support:
         :param bool i_geodesic:
         :param float i_radius:
@@ -974,38 +974,38 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleCtrRadWithAngles(Reference iCenter,
                 | Reference iSupport,
                 | boolean iGeodesic,
                 | double iRadius,
                 | double iStartAngle,
                 | double iEndAngle) As HybridShapeCircleCtrRad
-                | 
+                |
                 |     Creates a new circle defined by its center, a radius and angles within the
                 |     current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCenter
                 |             circle center.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iSupport
                 |         support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iGeodesic
-                |         Puts the circle on the surface. 
+                |         Puts the circle on the surface.
                 |     iRadius
                 |         Value specified is considered as radius. To use this value as diameter,
-                |         set DiameterMode using SetDiameterMode method 
+                |         set DiameterMode using SetDiameterMode method
                 |     iStartAngle
-                |         start angle 
+                |         start angle
                 |     iEndAngle
-                |         end angle 
+                |         end angle
                 |     oCircle
                 |         Created circle
 
         :param Reference i_center:
         :param Reference i_support:
         :param bool i_geodesic:
         :param float i_radius:
@@ -1022,22 +1022,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCircleDatum(Reference iObject) As
                 | HybridShapeCircleExplicit
-                | 
+                |
                 |     Creates a new datum of circle within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             The object whose topological body will be duplicated and put into
-                |             created datum 
+                |             created datum
                 |         oCircle
                 |             Created datum Note2: the object passed as parameter to create the
                 |             datum has to be in the current container. Otherwise, an error
                 |             occurs.
 
         :param Reference i_object:
         :return: HybridShapeCircleExplicit
@@ -1056,43 +1056,43 @@
                 | o Func AddNewCircleTritangent(Reference iCurve1,
                 | Reference iCurve2,
                 | Reference iCurve3,
                 | Reference iSupport,
                 | long iOri1,
                 | long iOri2,
                 | long iOri3) As HybridShapeCircleTritangent
-                | 
+                |
                 |     Creates a new tritangent circle within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve1
                 |             first curve to which the circle will be tangent.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iCurve2
                 |         second curve to which the circle will be tangent.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge and
                 |         BiDimFeatEdge.
                 |     iCurve3
                 |         third curve to which the circle will be tangent.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge and
                 |         BiDimFeatEdge.
                 |     iSupport
                 |         support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iOri1
-                |         first curve orientation for circle computation. 
+                |         first curve orientation for circle computation.
                 |     iOri2
-                |         second curve orientation for circle computation. 
+                |         second curve orientation for circle computation.
                 |     iOri3
-                |         third curve orientation for circle computation. 
+                |         third curve orientation for circle computation.
                 |     oCircle
                 |         Created circle
 
         :param Reference i_curve1:
         :param Reference i_curve2:
         :param Reference i_curve3:
         :param Reference i_support:
@@ -1113,36 +1113,36 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCombine(Reference iFirstCurve,
                 | Reference iSecondCurve,
                 | long iNearestSolutions) As HybridShapeCombine
-                | 
+                |
                 |     Creates a new Combine within the current body. By default, the combine
                 |     direction is the normal of each curve. If you want to change see
                 |     CATIAHybridShapeCombine interfaces.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iFirstCurve
                 |             First curve to combine
-                | 
-                |             Sub-element(s) supported (see 
-                | 
+                |
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iSecondCurve
                 |         Second curve to combine
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge and
                 |         BiDimFeatEdge.
                 |     iNearestSolution
                 |         If more than one solution, to choose the nearest solution of the first
-                |         curve 
+                |         curve
                 |     oCombine
                 |         The combine object if succeded
 
         :param Reference i_first_curve:
         :param Reference i_second_curve:
         :param int i_nearest_solutions:
         :return: HybridShapeCombine
@@ -1158,31 +1158,31 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewConic(Reference iSupport,
                 | Reference iStartingPoint,
                 | Reference iEndPoint) As HybridShapeConic
-                | 
+                |
                 |     Creates a new conic within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSupport
                 |             The conic support (always a plane).
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see PlanarFace. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see PlanarFace.
                 |     iStartingPoint
                 |         Starting Point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iEndPoint
                 |         End Point
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     oConic
                 |         The Conic object if succeded
 
         :param Reference i_support:
         :param Reference i_starting_point:
@@ -1201,41 +1201,41 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewConicalReflectLineWithType(Reference iSupport,
                 | Reference iOrigin,
                 | double iAngle,
                 | long iOrientationSupport,
                 | long iType) As HybridShapeReflectLine
-                | 
+                |
                 |     Creates a new conical ReflectLine within the current body.
                 |     Create a conical reflectline curve on a support surface from an origin
                 |     point with an angle.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSupport
-                |             Support surface. 
+                |             Support surface.
                 |         iOrigin
-                |             Origin point. 
+                |             Origin point.
                 |         iAngle
-                |             Angle of the reflectline. 
+                |             Angle of the reflectline.
                 |         iOrientationSupport
                 |             Manage the angle used to compute the reflectline. Value can be 1 or
-                |             -1 
+                |             -1
                 |         iType
                 |             Manage the type used to compute the reflectline. Value can be 0 or
                 |             1 Returns or sets whether the reflectline curve is or should be created with
                 |             the normal to the support or the tangent plane to the
                 |             support.
                 |             Role: The TypeSolution indicates whether the created reflectline
                 |             curve is compute with the angle between the normale to the support and the
                 |             direction or with the angle between the tangent plane to the support and the
                 |             direction..
                 |             Legal values: 0 for the normal and 1 for the tangent plane.
-                |             
+                |
                 |         oReflectLine
                 |             Created conical reflectline.
 
         :param Reference i_support:
         :param Reference i_origin:
         :param float i_angle:
         :param int i_orientation_support:
@@ -1262,53 +1262,53 @@
                 | double iTension1,
                 | Reference iCurve2,
                 | Reference iPoint2,
                 | long iOrient2,
                 | long iContinuity2,
                 | double iTension2,
                 | boolean Trim) As HybridShapeConnect
-                | 
+                |
                 |     Creates a new Connect within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve1
                 |             First curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iPoint1
                 |         First point (lying on the first curve)
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iOrient1
-                |         Orientation on the first curve 
+                |         Orientation on the first curve
                 |     iContinuity1
-                |         Continuity on first curve 
+                |         Continuity on first curve
                 |     iTension1
-                |         Tension on first curve 
+                |         Tension on first curve
                 |     iCurve2
                 |         Second curve.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge and
                 |         BiDimFeatEdge.
                 |     iPoint2
                 |         Second point (lying on the second curve)
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iOrient2
-                |         Orientation on the second curve 
+                |         Orientation on the second curve
                 |     iContinuity2
-                |         Continuity on second curve 
+                |         Continuity on second curve
                 |     iTension2
-                |         Tension on second curve 
+                |         Tension on second curve
                 |     iTrim
-                |         Trim the two curves with the connect 
+                |         Trim the two curves with the connect
                 |     oConnect
                 |         The connect object
 
         :param Reference i_curve1:
         :param Reference i_point1:
         :param int i_orient1:
         :param int i_continuity1:
@@ -1337,47 +1337,47 @@
                 | o Func AddNewCorner(Reference iElement1,
                 | Reference iElement2,
                 | Reference iSupport,
                 | double iRadius,
                 | long iOrientation1,
                 | long iOrientation2,
                 | boolean iTrim) As HybridShapeCorner
-                | 
+                |
                 |     Creates a new Corner within the current body.
                 |     Create a corner curve between a point and a curve or 2 curves on a support
                 |     surface.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement1
                 |             First reference curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge, BiDimFeatEdge and Vertex.
-                |         
+                |
                 |     iElement2
                 |         Second reference curve.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge,
                 |         BiDimFeatEdge and Vertex.
                 |     iSupport
                 |         Support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iRadius
-                |         Radius of the corner. 
+                |         Radius of the corner.
                 |     iOrientation1
                 |         Manage the corner center position. Value can be 1 or -1
-                |         
+                |
                 |     iOrientation2
                 |         Manage the corner center position. Value can be 1 or -1
-                |         
+                |
                 |     iTrim
                 |         Value can be FALSE or TRUE
                 |         if TRUE the 2 curves are trimed and asembled with the corner.
-                |         
+                |
                 |     oCorner
                 |         Created corner.
 
         :param Reference i_element1:
         :param Reference i_element2:
         :param Reference i_support:
         :param float i_radius:
@@ -1395,22 +1395,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCurveDatum(Reference iObject) As
                 | HybridShapeCurveExplicit
-                | 
+                |
                 |     Creates a new datum of curve within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             The object whose topological body will be duplicated and put into
-                |             created datum 
+                |             created datum
                 |         oCurve
                 |             Created curve Note2: the object passed as parameter to create the
                 |             datum has to be in the current container. Otherwise, an error
                 |             occurs.
 
         :param Reference i_object:
         :return: HybridShapeCurveExplicit
@@ -1426,36 +1426,36 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCurvePar(Reference Curve,
                 | Reference Support,
                 | double Distance,
                 | boolean InvertDirection,
                 | boolean Geodesic) As HybridShapeCurvePar
-                | 
+                |
                 |     Creates a new CurvePar within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
                 |             Reference curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iSupport
                 |         Support on which the curve is lying on
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iDistance
-                |         Distance value 
+                |         Distance value
                 |     iInvertDirection
-                |         Orientation 
+                |         Orientation
                 |     iGeodesic
-                |         Geodesic mode 
+                |         Geodesic mode
                 |     oCurvePar
                 |         Parallel curve
 
         :param Reference curve:
         :param Reference support:
         :param float distance:
         :param bool invert_direction:
@@ -1471,21 +1471,21 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCurveSmooth(Reference ipIACurve) As
                 | HybridShapeCurveSmooth
-                | 
+                |
                 |     Creates a new CurveSmooth within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
-                |             Reference curve to be smoothened 
+                |             Reference curve to be smoothened
                 |         oCurveSmooth
                 |             Smoothened curve
 
         :param Reference ip_ia_curve:
         :return: HybridShapeCurveSmooth
         :rtype: HybridShapeCurveSmooth
         """
@@ -1499,32 +1499,32 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewCylinder(Reference iCenter,
                 | double iRadius,
                 | double iFirstLength,
                 | double iSecondLength,
                 | HybridShapeDirection iDirection) As HybridShapeCylinder
-                | 
+                |
                 |     Creates a new Cylinder within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCenter
                 |             Center of the Cylinder - Can be Point or Vertex.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Vertex object): 
+                |             Sub-element(s) supported (see
+                |
+                |         Vertex object):
                 |     iRadius
-                |         Radius of Cylinder. 
+                |         Radius of Cylinder.
                 |     iFirstLength
-                |         Length of Cylinder in the given direction. 
+                |         Length of Cylinder in the given direction.
                 |     iSecondLength
-                |         Length of Cylinder in the opposite direction. 
+                |         Length of Cylinder in the opposite direction.
                 |     iDirection
-                |         Direction of extrusion for Cylinder. 
+                |         Direction of extrusion for Cylinder.
                 |     oCylinderObject
                 |         Created CylinderObjct.
 
         :param Reference i_center:
         :param float i_radius:
         :param float i_first_length:
         :param float i_second_length:
@@ -1539,46 +1539,46 @@
     def add_new_datums(self, i_elem: Reference) -> tuple:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewDatums(Reference iElem) As CATSafeArrayVariant
-                | 
+                |
                 |     Creates datums from a multi-domain result feature, one datum is created by
                 |     object domain.
                 |     Note; Available only for a shape design feature as input ( not for datum
                 |     feature ).
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElem
-                |             Reference element 
+                |             Reference element
                 |         oArrayOfDatum
                 |             List of datum objects , one datum is created per
                 |             omain
                 |             Level of availability = V5R14
-                | 
+                |
                 |             Example:
                 |                 This example converts a hybrid shape object in as much as
                 |                 datums that the original hybrid shape features contains of
                 |                 domain
-                | 
-                |                   Dim HShape 
+                |
+                |                   Dim HShape
                 |                   Set reference   = part.CreateReferenceFromObject(hybridShapeObject)
-                |                   ' Convert to Datums 
-                |                   HShape = hybridShapeFactory.AddNewDatums reference  
+                |                   ' Convert to Datums
+                |                   HShape = hybridShapeFactory.AddNewDatums reference
                 |                   Num =UBound(HShape)
-                |                   For i = 0 to Num  
+                |                   For i = 0 to Num
                 |                         hybridBody1.AppendHybridShape HShape (i)
-                |                         
-                |                   Next 
-                |                   part.InWorkObject = HShape(num) 
-                |                   part.Update 
-                |                   ' Delete original feature 
+                |
+                |                   Next
+                |                   part.InWorkObject = HShape(num)
+                |                   part.Update
+                |                   ' Delete original feature
                 |                   hybridShapeFactory.DeleteObjectForDatum
                 |                   reference
 
         :param Reference i_elem:
         :return: tuple
         :rtype: tuple
         """
@@ -1599,28 +1599,28 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewDevelop(long iMode,
                 | Reference iToDevelop,
                 | Reference iSupport) As HybridShapeDevelop
-                | 
+                |
                 |     Creates a new Develop within the current body.
                 |     Note: require either DL1 or GSO license.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iMode
-                |             Develop method. 
+                |             Develop method.
                 |         iToDevelop
                 |             Wire to be developed.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iSupport
                 |         Revolution support surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     oExt
                 |         Created developed wire.
 
@@ -1637,29 +1637,29 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewDirection(Reference iElement) As
                 | HybridShapeDirection
-                | 
+                |
                 |     Creates a new direction specified by an element within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement
                 |             Line or plane specifying the direction. In case of plane, the plane
                 |             normal vector is the direction
-                | 
-                |             Sub-element(s) supported (see 
-                | 
+                |
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge,
                 |         RectilinearBiDimFeatEdge and RectilinearMonoDimFeatEdge.
-                |         
+                |
                 |     oDirection
                 |         Created direction.
 
         :param Reference i_element:
         :return: HybridShapeDirection
         :rtype: HybridShapeDirection
         """
@@ -1670,26 +1670,26 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewDirectionByCoord(double iX,
                 | double iY,
                 | double iZ) As HybridShapeDirection
-                | 
+                |
                 |     Creates a new Direction specifed by coordinates within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iX
-                |             X component 
+                |             X component
                 |         iY
-                |             Y component 
+                |             Y component
                 |         iZ
-                |             Z component 
+                |             Z component
                 |         oDirection
                 |             Created direction
 
         :param float i_x:
         :param float i_y:
         :param float i_z:
         :return: HybridShapeDirection
@@ -1700,30 +1700,30 @@
     def add_new_empty_rotate(self) -> HybridShapeRotate:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewEmptyRotate() As HybridShapeRotate
-                | 
+                |
                 |     Creates a new empty Rotate within the current body.
 
         :return: HybridShapeRotate
         :rtype: HybridShapeRotate
         """
         return HybridShapeRotate(self.hybrid_shape_factory.AddNewEmptyRotate())
 
     def add_new_empty_translate(self) -> HybridShapeTranslate:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewEmptyTranslate() As HybridShapeTranslate
-                | 
+                |
                 |     Creates a new empty Translate within the current body.
 
         :return: HybridShapeTranslate
         :rtype: HybridShapeTranslate
         """
         return HybridShapeTranslate(self.hybrid_shape_factory.AddNewEmptyTranslate())
 
@@ -1731,25 +1731,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewExtract(Reference Element) As
                 | HybridShapeExtract
-                | 
+                |
                 |     Creates a new Extract within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement
                 |             Initial element used to start the extraction
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Boundary. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Boundary.
                 |     oExt
                 |         The extracted object
 
         :param Reference element:
         :return: HybridShapeExtract
         :rtype: HybridShapeExtract
         """
@@ -1759,25 +1759,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewExtractMulti(Reference Element) As
                 | HybridShapeExtractMulti
-                | 
+                |
                 |     Creates a new Multiple Extract within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement
                 |             Initial element used to start the extraction
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Boundary. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Boundary.
                 |     oExt
                 |         The extracted object
 
         :param Reference element:
         :return: HybridShapeExtractMulti
         :rtype: HybridShapeExtractMulti
         """
@@ -1789,33 +1789,33 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewExtrapolLength(Reference iBoundary,
                 | Reference iToExtrapol,
                 | double iLength) As HybridShapeExtrapol
-                | 
+                |
                 |     Creates a new Extrapol (specified by length) within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iBoundary
                 |             Boundary point of curve to extrapolate or boundary curve of surface
                 |             to extrapolate.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iToExtrapol
                 |         Curve or surface to extrapolate.
                 |         Sub-element(s) supported (see Boundary object): see Face,
                 |         TriDimFeatEdge and BiDimFeatEdge.
                 |     iLength
-                |         Extrapolation length. 
+                |         Extrapolation length.
                 |     oExtrapol
                 |         Created Extrapolation.
 
         :param Reference i_boundary:
         :param Reference i_to_extrapol:
         :param float i_length:
         :return: HybridShapeExtrapol
@@ -1830,33 +1830,33 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewExtrapolUntil(Reference iBoundary,
                 | Reference iToExtrapol,
                 | Reference iUntil) As HybridShapeExtrapol
-                | 
+                |
                 |     Creates a new Extrapol (until an element) within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iBoundary
                 |             Boundary point of curve to extrapolate or boundary curve of surface
                 |             to extrapolate.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iToExtrapol
                 |         Curve or surface to extrapolate.
                 |         Sub-element(s) supported (see Boundary object): see Face,
                 |         TriDimFeatEdge and BiDimFeatEdge.
                 |     iUntil
-                |         Extrapolation limit surface. 
+                |         Extrapolation limit surface.
                 |     oExtrapol
                 |         Created Extrapolation.
 
         :param Reference i_boundary:
         :param Reference i_to_extrapol:
         :param Reference i_until:
         :return: HybridShapeExtrapol
@@ -1871,30 +1871,30 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewExtremum(Reference iObjet,
                 | HybridShapeDirection iDir,
                 | long iMinMax) As HybridShapeExtremum
-                | 
+                |
                 |     Creates a new Extremum within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObjet
                 |             Element onto extremum is computed
-                | 
-                |             Sub-element(s) supported (see 
-                | 
+                |
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge, BiDimFeatEdge and Face.
-                |         
+                |
                 |     iDir
-                |         Extremum direction 
+                |         Extremum direction
                 |     iMinMax
-                |         Maximum (GSMMax) or Minimum (GSMMin) 
+                |         Maximum (GSMMax) or Minimum (GSMMin)
                 |     oExt
                 |         The extremum object if succeded
 
         :param Reference i_objet:
         :param HybridShapeDirection i_dir:
         :param int i_min_max:
         :return: HybridShapeExtremum
@@ -1907,24 +1907,24 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewExtremumPolar(short iType,
                 | Reference ipIAContour) As HybridShapeExtremumPolar
-                | 
+                |
                 |     Creates a new Extremum Polar within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iType
                 |             Type of extremum polar 0-Min Radius 1-Max Radius 2- Min Angle 3-
-                |             Maximum Angle 
+                |             Maximum Angle
                 |         ipIAContour
-                |             Extremum Polar Contour. It should be non convex 
+                |             Extremum Polar Contour. It should be non convex
                 |         opIAExtPolar
                 |             The extremum polar object if succeded
 
         :param int i_type:
         :param Reference ip_ia_contour:
         :return: HybridShapeExtremumPolar
         :rtype: HybridShapeExtremumPolar
@@ -1938,32 +1938,32 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewExtrude(Reference iObjectToExtrude,
                 | double iOffsetDebut,
                 | double iOffsetFin,
                 | HybridShapeDirection iDirection) As HybridShapeExtrude
-                | 
+                |
                 |     Creates a new extrude within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObjectToExtrude
                 |             Object to be extruded (point, line ,curve,or face)
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Boundary. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Boundary.
                 |     iOffsetDebut
-                |         Length value 
+                |         Length value
                 |     iOffsetFin
                 |         Length value ( iOffsetFin has to be larger than iOffsetDebut)
-                |         
+                |
                 |     iDirection
-                |         Extrusion direction 
+                |         Extrusion direction
                 |     oExtrudeObject
                 |         Extruded result
 
         :param Reference i_object_to_extrude:
         :param float i_offset_debut:
         :param float i_offset_fin:
         :param HybridShapeDirection i_direction:
@@ -1977,19 +1977,19 @@
     def add_new_fill(self) -> HybridShapeFill:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewFill() As HybridShapeFill
-                | 
+                |
                 |     Creates a new Fill within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oFill
                 |             Fill object
 
         :return: HybridShapeFill
         :rtype: HybridShapeFill
         """
         return HybridShapeFill(self.hybrid_shape_factory.AddNewFill())
@@ -2005,37 +2005,37 @@
                 | o Func AddNewFilletBiTangent(Reference iElement1,
                 | Reference iElement2,
                 | double iRadius,
                 | long iOrientation1,
                 | long iOrientation2,
                 | long iSupportsTrimMode,
                 | long iRibbonRelimitationMode) As HybridShapeFilletBiTangent
-                | 
+                |
                 |     Creates a new a sphere bitangent fillet between two skins.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement1
                 |             First support of fillet.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Face. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Face.
                 |     iElement2
                 |         Second support of fillet.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iRadius
-                |         Radius of the fillet. 
+                |         Radius of the fillet.
                 |     iOrientation1
-                |         Manage the fillet center position. 
+                |         Manage the fillet center position.
                 |     iOrientation2
-                |         Manage the fillet center position. 
+                |         Manage the fillet center position.
                 |     iSupportsTrimMode
                 |         The 2 supports can be trimmed and assembled with the fillet. Value can
-                |         be 0 (No trim ) or 1 (Trim) 
+                |         be 0 (No trim ) or 1 (Trim)
                 |     iRibbonRelimitationMode
                 |         Manage the relimition of fillet extremities.
                 |         Value can be : 0 (Smooth), 1 (Straight), 2 (Maximum) or 3 (Minimum)
                 |     oFillet
                 |         Created fillet.
 
         :param Reference i_element1:
@@ -2066,41 +2066,41 @@
                 | Reference iElement2,
                 | Reference iRemoveElem,
                 | long iOrientation1,
                 | long iOrientation2,
                 | long iRemoveOrientation,
                 | long iSupportsTrimMode,
                 | long iRibbonRelimitationMode) As HybridShapeFilletTriTangent
-                | 
+                |
                 |     Creates a new a tritangent fillet between three skins.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement1
                 |             First support of fillet.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Face. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Face.
                 |     iElement2
                 |         Second support of fillet.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iRemoveElem
                 |         Support to remove of fillet.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iOrientation1
-                |         Manage the fillet center position. 
+                |         Manage the fillet center position.
                 |     iOrientation2
-                |         Manage the fillet center position. 
+                |         Manage the fillet center position.
                 |     iRemoveOrientation
-                |         Manage the fillet center position. 
+                |         Manage the fillet center position.
                 |     iSupportsTrimMode
                 |         The 2 supports can be trimmed and assembled with the fillet. Value can
-                |         be 0 (No trim ) or 1 (Trim) 
+                |         be 0 (No trim ) or 1 (Trim)
                 |     iRibbonRelimitationMode
                 |         Manage the relimition of fillet extremities.
                 |         Value can be : 0 (Smooth), 1 (Straight), 2 (Maximum) or 3 (Minimum)
                 |     oFillet
                 |         Created fillet.
 
         :param Reference i_element1:
@@ -2124,21 +2124,21 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewHealing(Reference iBodyToheal) As
                 | HybridShapeHealing
-                | 
+                |
                 |     Creates a new healing within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iBodyToHeal
-                |             The body to heal 
+                |             The body to heal
                 |         oHealing
                 |             The created healing
 
         :param Reference i_body_toheal:
         :return: HybridShapeHealing
         :rtype: HybridShapeHealing
         """
@@ -2157,45 +2157,45 @@
                 | Reference iStartingPoint,
                 | double iPitch,
                 | double iHeight,
                 | boolean iClockwiseRevolution,
                 | double iStartingAngle,
                 | double iTaperAngle,
                 | boolean iTaperOutward) As HybridShapeHelix
-                | 
+                |
                 |     Creates a new Helix within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iAxis
                 |             The helix axis (always a line).
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge and
-                |         RectilinearBiDimFeatEdge. 
+                |         RectilinearBiDimFeatEdge.
                 |     iInvertAxis
                 |     iStartingPoint
                 |         Starting Point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iPitch
-                |         Pitch. 
+                |         Pitch.
                 |     iHeight
-                |         Helix height. 
+                |         Helix height.
                 |     iClockwiseRevolution
                 |         Revolutions are clockwise if TRUE, counterclockwise if FALSE.
-                |         
+                |
                 |     iStartingAngle
                 |         Starting angle from starting point measured on the helix itself. If no
-                |         starting angle is wanted, set it to 0.0. 
+                |         starting angle is wanted, set it to 0.0.
                 |     iTaperAngle
                 |         0 <= Taper Angle < Pi/2 If no taper angle is wanted, set it to 0.0
-                |         (constant helix radius). 
+                |         (constant helix radius).
                 |     iTaperOutward
-                |         Helix radius increases if TRUE, decreases if FALSE. 
+                |         Helix radius increases if TRUE, decreases if FALSE.
                 |     oHelix
                 |         The Helix object if succeded
 
         :param Reference i_axis:
         :param bool i_invert_axis:
         :param Reference i_starting_point:
         :param float i_pitch:
@@ -2218,31 +2218,31 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewHybridScaling(Reference iElemToScale,
                 | Reference iCenter,
                 | double iRatio) As HybridShapeScaling
-                | 
+                |
                 |     Creates a new scaling within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElemToScale
                 |             Point, curve, surface or solid to transform.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, TriDimFeatEdge, BiDimFeatEdge and Vertex.
-                |         
+                |
                 |     iCenter
                 |         Reference point or reference plane.
                 |         Sub-element(s) supported (see Boundary object): see PlanarFace and
                 |         Vertex.
                 |     iRatio
-                |         Scaling ratio. 
+                |         Scaling ratio.
                 |     oScaling
                 |         Created scaling.
 
         :param Reference i_elem_to_scale:
         :param Reference i_center:
         :param float i_ratio:
         :return: HybridShapeScaling
@@ -2257,32 +2257,32 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewHybridSplit(Reference iElement1,
                 | Reference iElement2,
                 | long iOrientation) As HybridShapeSplit
-                | 
+                |
                 |     Creates a new Split within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement1
                 |             The feature to cut (curve or surface).
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iElement2
                 |         The cutting feature (point, curve, surface).
                 |         Sub-element(s) supported (see Boundary object): see Face,
                 |         TriDimFeatEdge, BiDimFeatEdge and Vertex.
                 |     iOrientation
                 |         Manage the kept side of the feature to cut (value can be 1 or -1)
-                |         
+                |
                 |     oSplit
                 |         Created split
 
         :param Reference i_element1:
         :param Reference i_element2:
         :param int i_orientation:
         :return: HybridShapeSplit
@@ -2298,31 +2298,31 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewHybridTrim(Reference iElement1,
                 | long iOrientation1,
                 | Reference iElement2,
                 | long iOrientation2) As HybridShapeTrim
-                | 
+                |
                 |     Creates a new Trim within the current body by cutting and joining two
                 |     elements.
                 |     You can trim a surface by a surface or a curve by a curve.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement1
-                |             The feature to trim (curve or surface). 
+                |             The feature to trim (curve or surface).
                 |         iOrientation1
                 |             Manage the kept side of iElement1 (value can be 1 or -1).
-                |             
+                |
                 |         iElement2
-                |             The second feature to trim (curve or surface). 
+                |             The second feature to trim (curve or surface).
                 |         iOrientation2
                 |             Manage the kept side of iElement2 (value can be 1 or -1).
-                |             
+                |
                 |         oTrim
                 |             Created trim.
 
         :param Reference i_element1:
         :param int i_orientation1:
         :param Reference i_element2:
         :param int i_orientation2:
@@ -2337,19 +2337,19 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewIntegratedLaw(long iType) As
                 | HybridShapeIntegratedLaw
-                | 
+                |
                 |     Creates Integrated Law.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iType
                 |             Type of law =
                 |             0 : None | 1 : Constant | 2 : Linear | 3 : SType | 4 : Advanced | 5 : Implicit
 
         :param int i_type:
         :return: HybridShapeIntegratedLaw
         :rtype: HybridShapeIntegratedLaw
@@ -2360,25 +2360,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewIntersection(Reference iObject1,
                 | Reference iObject2) As HybridShapeIntersection
-                | 
+                |
                 |     Creates a new Intersection within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject1
                 |             First element ( line, curve, plane, surface.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, RectilinearTriDimFeatEdge and
-                |         RectilinearBiDimFeatEdge. 
+                |         RectilinearBiDimFeatEdge.
                 |     iObject2
                 |         Second element ( line , curve, plane, surface.
                 |         Sub-element(s) supported (see Boundary object): see Face,
                 |         RectilinearTriDimFeatEdge and
                 |         RectilinearBiDimFeatEdge.
                 |     oIntersection
                 |         Intersection
@@ -2395,24 +2395,24 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewInverse(Reference Element,
                 | long Inverse) As HybridShapeInverse
-                | 
+                |
                 |     Creates a new Inverse within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement
-                |             The objet to inverse 
+                |             The objet to inverse
                 |         iInverse
                 |             the type of inversion (see CATGSMOrientation.h) 1 for no inversion
-                |             -1 for inversion 
+                |             -1 for inversion
                 |         oInv
                 |             The inverted object
 
         :param Reference element:
         :param int inverse:
         :return: HybridShapeInverse
         :rtype: HybridShapeInverse
@@ -2423,29 +2423,29 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewJoin(Reference Element1,
                 | Reference Element2) As HybridShapeAssemble
-                | 
+                |
                 |     Creates a new Join within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement1
                 |             First element to join ( curve or surface.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iElement2
                 |         Second element to join ( same type of the first
                 |         element)
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see Face,
                 |         TriDimFeatEdge and BiDimFeatEdge.
                 |     oExt
                 |         Join result The default value used to join element is
                 |         0.001mm
 
         :param Reference element1:
@@ -2459,25 +2459,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLawDistProj(Reference iReference,
                 | Reference iDefinition) As HybridShapeLawDistProj
-                | 
+                |
                 |     Creates a new law within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iReference
                 |             Reference line of the law.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge and
-                |         RectilinearBiDimFeatEdge. 
+                |         RectilinearBiDimFeatEdge.
                 |     iDefinition
                 |         Definition curve of the law.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge and
                 |         BiDimFeatEdge.
                 |     oLaw
                 |         The Law object if succeded
 
@@ -2501,45 +2501,45 @@
                 | Reference iSurface,
                 | Reference iPoint,
                 | boolean iGeodesic,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | double iAngle,
                 | boolean iOrientation) As HybridShapeLineAngle
-                | 
+                |
                 |     Creates a new angle line within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
                 |             Reference curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iSurface
                 |         Reference surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iPoint
                 |         reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iGeodesic
-                |         Puts the line on the surface 
+                |         Puts the line on the surface
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iAngle
-                |         angle to reference curve 
+                |         angle to reference curve
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_curve:
         :param Reference i_surface:
         :param Reference i_point:
         :param bool i_geodesic:
@@ -2560,25 +2560,25 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLineBiTangent(Reference iCurve1,
                 | Reference iElement2,
                 | Reference iSupport) As HybridShapeLineBiTangent
-                | 
+                |
                 |     Creates a new bitangent line within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve1
                 |             First tangency curve lying on the support surface.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iCurve2
                 |         Second tangency element (point, curve) lying on the support
                 |         surface.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge,
                 |         BiDimFeatEdge and Vertex.
                 |     iSupport
                 |         The support surface of the two elements.
@@ -2606,38 +2606,38 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLineBisecting(Reference iLine1,
                 | Reference iLine2,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation,
                 | long SolutionNb) As HybridShapeLineBisecting
-                | 
+                |
                 |     Creates a new bisecting line within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iLine1
                 |             First line.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge and
-                |         RectilinearBiDimFeatEdge. 
+                |         RectilinearBiDimFeatEdge.
                 |     iLine2
                 |         Second line.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         RectilinearTriDimFeatEdge and
                 |         RectilinearBiDimFeatEdge.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_line1:
         :param Reference i_line2:
         :param float i_begin_offset:
         :param float i_end_offset:
@@ -2661,43 +2661,43 @@
                 | o Func AddNewLineBisectingOnSupport(Reference iLine1,
                 | Reference iLine2,
                 | Reference iSurface,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation,
                 | long SolutionNb) As HybridShapeLineBisecting
-                | 
+                |
                 |     Creates a new bisecting line on a support within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iLine1
                 |             First line.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge and
-                |         RectilinearBiDimFeatEdge. 
+                |         RectilinearBiDimFeatEdge.
                 |     iLine2
                 |         Second line.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         RectilinearTriDimFeatEdge and
                 |         RectilinearBiDimFeatEdge.
                 |     iSurface
                 |         Reference surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_line1:
         :param Reference i_line2:
         :param Reference i_surface:
         :param float i_begin_offset:
@@ -2726,47 +2726,47 @@
                 | Reference iLine2,
                 | Reference iRefPoint,
                 | Reference iSurface,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation,
                 | long SolutionNb) As HybridShapeLineBisecting
-                | 
+                |
                 |     Creates a new bisecting line on a support with a atarting point within the
                 |     current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iLine1
                 |             First line.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge and
-                |         RectilinearBiDimFeatEdge. 
+                |         RectilinearBiDimFeatEdge.
                 |     iLine2
                 |         Second line.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         RectilinearTriDimFeatEdge and
                 |         RectilinearBiDimFeatEdge.
                 |     iRefPoint
                 |         Starting point of the bisecting line.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iSurface
                 |         Reference surface.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_line1:
         :param Reference i_line2:
         :param Reference i_ref_point:
         :param Reference i_surface:
@@ -2794,43 +2794,43 @@
                 | o Func AddNewLineBisectingWithPoint(Reference iLine1,
                 | Reference iLine2,
                 | Reference iRefPoint,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation,
                 | long SolutionNb) As HybridShapeLineBisecting
-                | 
+                |
                 |     Creates a new bisecting line with a starting point within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iLine1
                 |             First line.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge and
-                |         RectilinearBiDimFeatEdge. 
+                |         RectilinearBiDimFeatEdge.
                 |     iLine2
                 |         Second line.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         RectilinearTriDimFeatEdge and
                 |         RectilinearBiDimFeatEdge.
                 |     iRefPoint
                 |         Starting point of the bisecting line.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_line1:
         :param Reference i_line2:
         :param Reference i_ref_point:
         :param float i_begin_offset:
@@ -2849,22 +2849,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLineDatum(Reference iObject) As
                 | HybridShapeLineExplicit
-                | 
+                |
                 |     Creates a new datum of line within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             The object whose topological body will be duplicated and put into
-                |             created datum 
+                |             created datum
                 |         oLine
                 |             Created datum Note2: the object passed as parameter to create the
                 |             datum has to be in the current container. Otherwise, an error
                 |             occurs.
 
         :param Reference i_object:
         :return: HybridShapeLineExplicit
@@ -2880,36 +2880,36 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLineNormal(Reference iSurface,
                 | Reference iPoint,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation) As HybridShapeLineNormal
-                | 
+                |
                 |     Creates a new normal line within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSurface
                 |             Reference surface.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Face. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Face.
                 |     iPoint
                 |         Reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_surface:
         :param Reference i_point:
         :param float i_begin_offset:
         :param float i_end_offset:
@@ -2929,35 +2929,35 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLinePtDir(Reference iPt,
                 | HybridShapeDirection iDirection,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation) As HybridShapeLinePtDir
-                | 
+                |
                 |     Creates a new point-direction line within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPt
                 |             reference point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iDirection
-                |         Direction 
+                |         Direction
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_pt:
         :param HybridShapeDirection i_direction:
         :param float i_begin_offset:
         :param float i_end_offset:
@@ -2979,40 +2979,40 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLinePtDirOnSupport(Reference iPt,
                 | HybridShapeDirection iDirection,
                 | Reference iSupport,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation) As HybridShapeLinePtDir
-                | 
+                |
                 |     Creates a new point-direction line within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPt
                 |             reference point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iDirection
-                |         Direction 
+                |         Direction
                 |     iSupport
                 |         Support element (surface or plane)
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_pt:
         :param HybridShapeDirection i_direction:
         :param Reference i_support:
         :param float i_begin_offset:
@@ -3030,24 +3030,24 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLinePtPt(Reference iPtOrigine,
                 | Reference iPtExtremite) As HybridShapeLinePtPt
-                | 
+                |
                 |     Creates a new point-point line within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPtOrigine
                 |             Origin point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iPtExtremite
                 |         Extremity point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     oLine
                 |         Created line
 
@@ -3066,33 +3066,33 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLinePtPtExtended(Reference iPtOrigine,
                 | Reference iPtExtremite,
                 | double iBeginOffset,
                 | double iEndOffset) As HybridShapeLinePtPt
-                | 
+                |
                 |     Creates a new point-point line with extensions within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPtOrigine
                 |             Origin point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iPtExtremite
                 |         Extremity point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     oLine
                 |         Created line
 
         :param Reference i_pt_origine:
         :param Reference i_pt_extremite:
         :param float i_begin_offset:
         :param float i_end_offset:
@@ -3109,32 +3109,32 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLinePtPtOnSupport(Reference iPtOrigine,
                 | Reference iPtExtremite,
                 | Reference iSupport) As HybridShapeLinePtPt
-                | 
+                |
                 |     Creates a new point-point line with support within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPtOrigine
                 |             Origin point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iPtExtremite
                 |         Extremity point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iSupport
                 |         Support element (surface or plane)
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     oLine
                 |         Created line
 
         :param Reference i_pt_origine:
         :param Reference i_pt_extremite:
@@ -3155,38 +3155,38 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLinePtPtOnSupportExtended(Reference iPtOrigine,
                 | Reference iPtExtremite,
                 | Reference iSupport,
                 | double iBeginOffset,
                 | double iEndOffset) As HybridShapeLinePtPt
-                | 
+                |
                 |     Creates a new point-point line with extensions and with support within the
                 |     current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPtOrigine
                 |             Origin point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iPtExtremite
                 |         Extremity point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iSupport
                 |         Support element (surface or plane)
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     oLine
                 |         Created line
 
         :param Reference i_pt_origine:
         :param Reference i_pt_extremite:
         :param Reference i_support:
         :param float i_begin_offset:
@@ -3208,37 +3208,37 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLineTangency(Reference iCurve,
                 | Reference iPoint,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation) As HybridShapeLineTangency
-                | 
+                |
                 |     Creates a new tangent line within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
                 |             Reference curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iPoint
                 |         Reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_curve:
         :param Reference i_point:
         :param float i_begin_offset:
         :param float i_end_offset:
@@ -3260,42 +3260,42 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLineTangencyOnSupport(Reference iCurve,
                 | Reference iPoint,
                 | Reference iSupport,
                 | double iBeginOffset,
                 | double iEndOffset,
                 | boolean iOrientation) As HybridShapeLineTangency
-                | 
+                |
                 |     Creates a new tangent line within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
                 |             Reference curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iPoint
                 |         Reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iSupport
                 |         Support element (surface or plane)
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Face.
                 |     iBeginOffset
-                |         start offset 
+                |         start offset
                 |     iEndOffset
-                |         end offset 
+                |         end offset
                 |     iOrientation
                 |         Orientation allows to reverse the line direction from the reference
                 |         point. For a line of L length, it is the same as creating this line with -L
-                |         length. 
+                |         length.
                 |     oLine
                 |         Created line
 
         :param Reference i_curve:
         :param Reference i_point:
         :param Reference i_support:
         :param float i_begin_offset:
@@ -3312,19 +3312,19 @@
     def add_new_loft(self) -> HybridShapeLoft:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewLoft() As HybridShapeLoft
-                | 
+                |
                 |     Creates a new Loft within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oExt
                 |             CATIAHybridShapeLoft created
 
         :return: HybridShapeLoft
         :rtype: HybridShapeLoft
         """
         return HybridShapeLoft(self.hybrid_shape_factory.AddNewLoft())
@@ -3335,26 +3335,26 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewMidSurface(Reference iSupport,
                 | long iCreationMode,
                 | double iThreshold) As HybridShapeMidSurface
-                | 
+                |
                 |     Creates a new MidSurface in Automatic Creation Mode Only.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSupport
-                |             support Body 
+                |             support Body
                 |         iCreationMode
-                |             Creation Mode (Only Automatic Accepted) 
+                |             Creation Mode (Only Automatic Accepted)
                 |         iThreshold
-                |             Threshold Thickness 
-                | 
+                |             Threshold Thickness
+                |
                 |     Returns:
                 |         oMidSurface Created MidSurface
 
         :param Reference i_support:
         :param int i_creation_mode:
         :param float i_threshold:
         :return: HybridShapeMidSurface
@@ -3370,28 +3370,28 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewMidSurfaceWithAutoThreshold(Reference iSupport,
                 | long iCreationMode,
                 | double iThreshold,
                 | long iAutoThicknessThreshold) As HybridShapeMidSurface
-                | 
+                |
                 |     Creates a new MidSurface in Automatic Creation Mode Only.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSupport
-                |             support Body 
+                |             support Body
                 |         iCreationMode
-                |             Creation Mode (Only Automatic Accepted) 
+                |             Creation Mode (Only Automatic Accepted)
                 |         iThreshold
-                |             Threshold Thickness 
+                |             Threshold Thickness
                 |         iAutoThicknessThreshold
-                |             Automatic Thickness Threshold 
-                | 
+                |             Automatic Thickness Threshold
+                |
                 |     Returns:
                 |         oMidSurface Created MidSurface
 
         :param Reference i_support:
         :param int i_creation_mode:
         :param float i_threshold:
         :param int i_auto_thickness_threshold:
@@ -3406,28 +3406,28 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewNear(Reference MultiElement,
                 | Reference ReferenceElement) As HybridShapeNear
-                | 
+                |
                 |     Creates a new Near within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iMultiElement
                 |             Non connex element (point,curve,surface.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, TriDimFeatEdge, BiDimFeatEdge and Vertex.
-                |         
+                |
                 |     iReferenceElement
                 |         Reference element
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see Face,
                 |         TriDimFeatEdge, BiDimFeatEdge and Vertex.
                 |     oNear
                 |         The result is the connex component that is the nearest from the
                 |         reference element
 
         :param Reference multi_element:
@@ -3445,31 +3445,31 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewOffset(Reference iObjectToOffset,
                 | double iOffset,
                 | boolean iOrientation,
                 | double iPrecision) As HybridShapeOffset
-                | 
+                |
                 |     Creates a new offset within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObjectToOffset
                 |             Surface to offset.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Face. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Face.
                 |     iOffset
-                |         Offset value 
+                |         Offset value
                 |     iOrientation
-                |         Offset orientation 
+                |         Offset orientation
                 |     iPrecision
                 |         This variable is no longer in use and any change in it's value does not
-                |         impact the output. 
+                |         impact the output.
                 |     oOffsetObject
                 |         Offset Surface
 
         :param Reference i_object_to_offset:
         :param float i_offset:
         :param bool i_orientation:
         :param float i_precision:
@@ -3483,26 +3483,26 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlane1Curve(Reference iPlanarCurve) As
                 | HybridShapePlane1Curve
-                | 
+                |
                 |     Creates a new plane passing through one planar curve within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPlanarCurve
                 |             passing curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     oPlane
                 |         Created plane
 
         :param Reference i_planar_curve:
         :return: HybridShapePlane1Curve
         :rtype: HybridShapePlane1Curve
         """
@@ -3512,27 +3512,27 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlane1Line1Pt(Reference iLn,
                 | Reference iPt) As HybridShapePlane1Line1Pt
-                | 
+                |
                 |     Creates a new plane passing through 1 line and 1 point within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iLn
                 |             passing line.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge,
                 |         RectilinearBiDimFeatEdge and RectilinearMonoDimFeatEdge.
-                |         
+                |
                 |     iPt
                 |         passing point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     oPlane
                 |         Created plane
 
@@ -3547,27 +3547,27 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlane2Lines(Reference iLn1,
                 | Reference iLn2) As HybridShapePlane2Lines
-                | 
+                |
                 |     Creates a new plane passing through 2 lines within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iLn1
                 |             first passing line.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see RectilinearTriDimFeatEdge,
                 |         RectilinearBiDimFeatEdge and RectilinearMonoDimFeatEdge.
-                |         
+                |
                 |     iLn2
                 |         second passing line.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         RectilinearTriDimFeatEdge, RectilinearBiDimFeatEdge and
                 |         RectilinearMonoDimFeatEdge.
                 |     oPlane
                 |         Created line
@@ -3584,25 +3584,25 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlane3Points(Reference iPt1,
                 | Reference iPt2,
                 | Reference iPt3) As HybridShapePlane3Points
-                | 
+                |
                 |     Creates a new plane passing through 3 points within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPt1
                 |             first passing point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iPt2
                 |         second passing point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iPt3
                 |         third passing point.
                 |         Sub-element(s) supported (see Boundary object): see
@@ -3626,36 +3626,36 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlaneAngle(Reference iPlane,
                 | Reference iRevolAxis,
                 | double iAngle,
                 | boolean iOrientation) As HybridShapePlaneAngle
-                | 
+                |
                 |     Creates a new angle plane within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPlane
                 |             reference plane
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see PlanarFace. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see PlanarFace.
                 |     iRevolAxis
                 |         rotation axis
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         RectilinearTriDimFeatEdge, RectilinearBiDimFeatEdge and
                 |         RectilinearMonoDimFeatEdge.
                 |     iAngle
-                |         angle 
+                |         angle
                 |     iOrientation
                 |         Orientation to reverse the plane from the reference plane.
-                |         
+                |
                 |     oPlane
                 |         Created plane
 
         :param Reference i_plane:
         :param Reference i_revol_axis:
         :param float i_angle:
         :param bool i_orientation:
@@ -3670,22 +3670,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlaneDatum(Reference iObject) As
                 | HybridShapePlaneExplicit
-                | 
+                |
                 |     Creates a new datum of plane within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             The object whose topological body will be duplicated and put into
-                |             created datum 
+                |             created datum
                 |         oPlane
                 |             Created datum Note2: the object passed as parameter to create the
                 |             datum has to be in the current container. Otherwise, an error
                 |             occurs.
 
         :param Reference i_object:
         :return: HybridShapePlaneExplicit
@@ -3700,27 +3700,27 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlaneEquation(double iA_Coeff,
                 | double iB_Coeff,
                 | double iC_Coeff,
                 | double iD_Coeff) As HybridShapePlaneEquation
-                | 
+                |
                 |     Creates a new equation plane within the current body. Plane equation is Ax+By+Cz = D.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iA_Coeff
-                |             A coefficient 
+                |             A coefficient
                 |         iB_Coeff
-                |             B coefficient 
+                |             B coefficient
                 |         iC_Coeff
-                |             C coefficient 
+                |             C coefficient
                 |         iD_Coeff
-                |             D coefficient 
+                |             D coefficient
                 |         oPlane
                 |             Created plane
 
         :param float i_a_coeff:
         :param float i_b_coeff:
         :param float i_c_coeff:
         :param float i_d_coeff:
@@ -3734,25 +3734,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlaneMean(CATSafeArrayVariant iListOfPoints,
                 | long NbPoint) As HybridShapePlaneMean
-                | 
+                |
                 |     Creates a new mean through points plane within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oIListOfPoints
                 |             list of passing points Warning : Input and Output parameter for CATScript applications,
                 |             procedural type
                 |         iNbPoint
-                |             Number of points 
+                |             Number of points
                 |         oPlane
                 |             Created plane
 
         :param tuple i_list_of_points:
         :param int nb_point:
         :return: HybridShapePlaneMean
         :rtype: HybridShapePlaneMean
@@ -3763,25 +3763,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlaneNormal(Reference iCurve,
                 | Reference iPt) As HybridShapePlaneNormal
-                | 
+                |
                 |     Creates a new normal plane within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
                 |             Reference curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iPt
                 |         Reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     oPlane
                 |         Created plane
 
@@ -3797,30 +3797,30 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlaneOffset(Reference iPlane,
                 | double iOffset,
                 | boolean iOrientation) As HybridShapePlaneOffset
-                | 
+                |
                 |     Creates a new offset plane within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPlane
                 |             reference plane
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see PlanarFace. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see PlanarFace.
                 |     iOffset
-                |         offset value 
+                |         offset value
                 |     iOrientation
                 |         Orientation to reverse the plane from the reference plane.
-                |         
+                |
                 |     oPlane
                 |         Created plane
 
         :param Reference i_plane:
         :param float i_offset:
         :param bool i_orientation:
         :return: HybridShapePlaneOffset
@@ -3833,26 +3833,26 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlaneOffsetPt(Reference iPlane,
                 | Reference iPt) As HybridShapePlaneOffsetPt
-                | 
+                |
                 |     Creates a new offset trough point plane within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPlane
                 |             reference plane
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see PlanarFace. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see PlanarFace.
                 |     iPt
                 |         Reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     oPlane
                 |         Created plane
 
@@ -3868,24 +3868,24 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPlaneTangent(Reference iSurface,
                 | Reference iPt) As HybridShapePlaneTangent
-                | 
+                |
                 |     Creates a new tangent plane within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSurface
                 |             reference surface.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Face. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Face.
                 |     iPt
                 |         reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     oPlane
                 |         Created plane
 
@@ -3904,32 +3904,32 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointBetween(Reference iPoint1,
                 | Reference iPoint2,
                 | double iRatio,
                 | long iOrientation) As HybridShapePointBetween
-                | 
+                |
                 |     Creates a new PointBetween within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPoint1
                 |             Reference point to compute the barycenter.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iPoint2
                 |         Second point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iRatio
-                |         barycenter parameter 
+                |         barycenter parameter
                 |     iOrientation
-                |         To compute the barycenter of the segment [Pt1 - Pt2] 
+                |         To compute the barycenter of the segment [Pt1 - Pt2]
                 |     oPoint
                 |         PointBetween if succeded
 
         :param Reference i_point1:
         :param Reference i_point2:
         :param float i_ratio:
         :param int i_orientation:
@@ -3944,25 +3944,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointCenter(Reference iCurve) As
                 | HybridShapePointCenter
-                | 
+                |
                 |     Creates a new circle center point within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
                 |             Reference circle
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Edge. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Edge.
                 |     oPoint
                 |         Created point
 
         :param Reference i_curve:
         :return: HybridShapePointCenter
         :rtype: HybridShapePointCenter
         """
@@ -3973,26 +3973,26 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointCoord(double iX,
                 | double iY,
                 | double iZ) As HybridShapePointCoord
-                | 
+                |
                 |     Creates a new point defined by its cartesian coordinates within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iX
-                |             X coordinate for the point 
+                |             X coordinate for the point
                 |         iY
-                |             Y coordinate for the point 
+                |             Y coordinate for the point
                 |         iZ
-                |             Z coordinate for the point 
+                |             Z coordinate for the point
                 |         oPoint
                 |             Created point
 
         :param float i_x:
         :param float i_y:
         :param float i_z:
         :return: HybridShapePointCoord
@@ -4022,31 +4022,31 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointCoordWithReference(double iX,
                 | double iY,
                 | double iZ,
                 | Reference iPt) As HybridShapePointCoord
-                | 
+                |
                 |     Creates a new point defined its the cartesian coordinates regarding a
                 |     reference point.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iX
-                |             X coordinate for the point 
+                |             X coordinate for the point
                 |         iY
-                |             Y coordinate for the point 
+                |             Y coordinate for the point
                 |         iZ
-                |             Z coordinate for the point 
+                |             Z coordinate for the point
                 |         iPt
                 |             Reference point.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     oPoint
                 |         Created point
 
         :param float i_x:
         :param float i_y:
         :param float i_z:
         :param Reference i_pt:
@@ -4060,22 +4060,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointDatum(Reference iObject) As
                 | HybridShapePointExplicit
-                | 
+                |
                 |     Creates a new datum of point within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             The object whose topological body will be duplicated and put into
-                |             created datum 
+                |             created datum
                 |         oPoint
                 |             Created datum Note2: the object passed as parameter to create the
                 |             datum has to be in the current container. Otherwise, an error
                 |             occurs.
 
         :param Reference i_object:
         :return: HybridShapePointExplicit
@@ -4090,33 +4090,33 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnCurveAlongDirection(Reference iCrv,
                 | double iLong,
                 | boolean iOrientation,
                 | HybridShapeDirection iDirection) As HybridShapePointOnCurve
-                | 
+                |
                 |     Creates a new point on a curve with a deafult origin point and from a
                 |     distance along direction.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCrv
                 |             support curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iLong
                 |         distance to default origin point.(origin of acurrent axis system)
-                |         
+                |
                 |     iOrientation
-                |         Orientation = TRUE means that distance is measured in the other orientation of the curve. 
+                |         Orientation = TRUE means that distance is measured in the other orientation of the curve.
                 |     iDirection
-                |         Direction = The distance at which point is created is measured in this direction. 
+                |         Direction = The distance at which point is created is measured in this direction.
                 |     oPoint
                 |         Created point
 
         :param Reference i_crv:
         :param float i_long:
         :param bool i_orientation:
         :param HybridShapeDirection i_direction:
@@ -4133,28 +4133,28 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnCurveFromDistance(Reference iCrv,
                 | double iLong,
                 | boolean iOrientation) As HybridShapePointOnCurve
-                | 
+                |
                 |     Creates a new point on a curve from a distance to an extremity within the
                 |     current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCrv
                 |             support curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iLong
-                |         distance to extremity 
+                |         distance to extremity
                 |     iOrientation
                 |         Orientation = TRUE means that distance is measured in the other orientation of the curve and
                 |         from the other extremity.
                 |     oPoint
                 |         Created point
 
         :param Reference i_crv:
@@ -4172,28 +4172,28 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnCurveFromPercent(Reference iCrv,
                 | double iLong,
                 | boolean iOrientation) As HybridShapePointOnCurve
-                | 
+                |
                 |     Creates a new point on a curve from a ratio of distance to an extremity
                 |     within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCrv
                 |             support curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iLong
-                |         Ratio of curve length 
+                |         Ratio of curve length
                 |     iOrientation
                 |         Orientation = TRUE means that ratio is measured in the other orientation of the curve and
                 |         from the other extremity.
                 |     oPoint
                 |         Created point
 
         :param Reference i_crv:
@@ -4217,36 +4217,36 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnCurveWithReferenceAlongDirection(Reference
                 | iCrv,
                 | Reference iPt,
                 | double iLong,
                 | boolean iOrientation,
                 | HybridShapeDirection iDirection) As HybridShapePointOnCurve
-                | 
+                |
                 |     Creates a new point on a curve with a reference point and from a distance
                 |     along direction.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCrv
                 |             support curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iPt
                 |         reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iLong
-                |         distance (length) to reference point 
+                |         distance (length) to reference point
                 |     iOrientation
-                |         Orientation = TRUE means that distance is measured in the other orientation of the curve 
+                |         Orientation = TRUE means that distance is measured in the other orientation of the curve
                 |     iDirection
-                |         Direction = The distance at which point is created is measured in this direction. 
+                |         Direction = The distance at which point is created is measured in this direction.
                 |     oPoint
                 |         Created point
 
         :param Reference i_crv:
         :param Reference i_pt:
         :param float i_long:
         :param bool i_orientation:
@@ -4267,34 +4267,34 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnCurveWithReferenceFromDistance(Reference
                 | iCrv,
                 | Reference iPt,
                 | double iLong,
                 | boolean iOrientation) As HybridShapePointOnCurve
-                | 
+                |
                 |     Creates a new point on a curve with a reference point and from a distance
                 |     within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCrv
                 |             support curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iPt
                 |         reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iLong
-                |         distance (length) to reference point 
+                |         distance (length) to reference point
                 |     iOrientation
-                |         Orientation = TRUE means that distance is measured in the other orientation of the curve 
+                |         Orientation = TRUE means that distance is measured in the other orientation of the curve
                 |     oPoint
                 |         Created point
 
         :param Reference i_crv:
         :param Reference i_pt:
         :param float i_long:
         :param bool i_orientation:
@@ -4313,34 +4313,34 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnCurveWithReferenceFromPercent(Reference
                 | iCrv,
                 | Reference iPt,
                 | double iLong,
                 | boolean iOrientation) As HybridShapePointOnCurve
-                | 
+                |
                 |     Creates a new point on a curve with a reference point and from a ratio of
                 |     distance within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCrv
                 |             Support curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iPt
                 |         reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iLong
-                |         Ratio of curve length 
+                |         Ratio of curve length
                 |     iOrientation
-                |         Orientation = TRUE means that ratio is measured in the other orientation of the curve 
+                |         Orientation = TRUE means that ratio is measured in the other orientation of the curve
                 |     oPoint
                 |         Created point
 
         :param Reference i_crv:
         :param Reference i_pt:
         :param float i_long:
         :param bool i_orientation:
@@ -4356,29 +4356,29 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnPlane(Reference iPlane,
                 | double iX,
                 | double iY) As HybridShapePointOnPlane
-                | 
+                |
                 |     Creates a new point on a plane within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPlane
                 |             Support plane
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see PlanarFace. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see PlanarFace.
                 |     iX
-                |         X cartesian coordinates in the plane. 
+                |         X cartesian coordinates in the plane.
                 |     iY
-                |         Y cartesian coordinates in the plane. 
+                |         Y cartesian coordinates in the plane.
                 |     oPoint
                 |         Created point
 
         :param Reference i_plane:
         :param float i_x:
         :param float i_y:
         :return: HybridShapePointOnPlane
@@ -4393,35 +4393,35 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnPlaneWithReference(Reference iPlane,
                 | Reference iPt,
                 | double iX,
                 | double iY) As HybridShapePointOnPlane
-                | 
+                |
                 |     Creates a new point on a plane with a reference point within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iPlane
                 |             Support plane
-                | 
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see PlanarFace. 
+                |
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see PlanarFace.
                 |     iPt
                 |         Reference plane
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iX
-                |         X cartesian coordinates in the plane. 
+                |         X cartesian coordinates in the plane.
                 |     iY
-                |         Y cartesian coordinates in the plane. 
+                |         Y cartesian coordinates in the plane.
                 |     oPoint
                 |         Created point
 
         :param Reference i_plane:
         :param Reference i_pt:
         :param float i_x:
         :param float i_y:
@@ -4437,29 +4437,29 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnSurface(Reference iSurface,
                 | HybridShapeDirection iDirection,
                 | double iX) As HybridShapePointOnSurface
-                | 
+                |
                 |     Creates a new point on a surface within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSurface
                 |             Support surface.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Face. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Face.
                 |     iDirection
                 |         Direction from the reference point in which the point is computed.
-                |         
+                |
                 |     iX
-                |         geodesic length to reference point 
+                |         geodesic length to reference point
                 |     oPoint
                 |         Created point
 
         :param Reference i_surface:
         :param HybridShapeDirection i_direction:
         :param float i_x:
         :return: HybridShapePointOnSurface
@@ -4476,34 +4476,34 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointOnSurfaceWithReference(Reference iSurface,
                 | Reference iPt,
                 | HybridShapeDirection iDirection,
                 | double iX) As HybridShapePointOnSurface
-                | 
+                |
                 |     Creates a new point on a surface with a reference point within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSurface
                 |             Support surface.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Face. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Face.
                 |     iPt
                 |         reference point.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Vertex.
                 |     iDirection
                 |         Direction from the reference point in which the point is computed.
-                |         
+                |
                 |     iX
-                |         geodesic length to reference point 
+                |         geodesic length to reference point
                 |     oPoint
                 |         Created point
 
         :param Reference i_surface:
         :param Reference i_pt:
         :param HybridShapeDirection i_direction:
         :param float i_x:
@@ -4518,27 +4518,27 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPointTangent(Reference iCurve,
                 | HybridShapeDirection iDirection) As HybridShapePointTangent
-                | 
+                |
                 |     Creates a new tangent to curve point within the current
                 |     body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCurve
                 |             Reference curve.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Edge. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Edge.
                 |     iDirection
-                |         Direction in which tangent points are computed 
+                |         Direction in which tangent points are computed
                 |     oPoint
                 |         Created point
 
         :param Reference i_curve:
         :param HybridShapeDirection i_direction:
         :return: HybridShapePointTangent
         :rtype: HybridShapePointTangent
@@ -4549,19 +4549,19 @@
     def add_new_polyline(self) -> HybridShapePolyline:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPolyline() As HybridShapePolyline
-                | 
+                |
                 |     Creates a new Polyline within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oPolyline
                 |             The Polyline object if succeded
 
         :return: HybridShapePolyline
         :rtype: HybridShapePolyline
         """
         return HybridShapePolyline(self.hybrid_shape_factory.AddNewPolyline())
@@ -4570,21 +4570,21 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewPositionTransfo(long iMode) As
                 | HybridShapePositionTransfo
-                | 
+                |
                 |     Creates a new PositionTransfo within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iMode
-                |             Positioning mode. 
+                |             Positioning mode.
                 |         oExt
                 |             Created positioning transformation (i.e. positioned wire /
                 |             profile).
 
         :param int i_mode:
         :return: HybridShapePositionTransfo
         :rtype: HybridShapePositionTransfo
@@ -4595,25 +4595,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewProject(Reference iElement,
                 | Reference iSupport) As HybridShapeProject
-                | 
+                |
                 |     Creates a new Project within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement
                 |             Element to project (point, curve).
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge, BiDimFeatEdge and Vertex.
-                |         
+                |
                 |     iSupport
                 |         Curve or surface support for projection.
                 |         Sub-element(s) supported (see Boundary object): see Face,
                 |         TriDimFeatEdge and BiDimFeatEdge.
                 |     oProjection
                 |         Created projection
 
@@ -4632,35 +4632,35 @@
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewReflectLine(Reference iSupport,
                 | HybridShapeDirection iDir,
                 | double iAngle,
                 | long iOrientationSupport,
                 | long iOrientationDirection) As HybridShapeReflectLine
-                | 
+                |
                 |     Deprecated:
                 |         V5R17 CATIAHybridShapeFactory#AddNewReflectLineWithType Creates a new
                 |         ReflectLine within the current body.
                 |         Create a reflectline curve on a support surface along a direction with
-                |         an angle. 
+                |         an angle.
                 |     Parameters:
-                | 
+                |
                 |         iSupport
                 |             Support surface.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Face. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Face.
                 |     iAngle
-                |         Angle of the reflectline. 
+                |         Angle of the reflectline.
                 |     iOrientationSupport
                 |         Manage the angle used to compute the reflectline. Value can be 1 or -1
-                |         
+                |
                 |     iOrientationDirection
                 |         Manage the angle used to compute the reflectline. Value can be 1 or -1
-                |         
+                |
                 |     oReflectLine
                 |         Created reflectline.
 
         :param Reference i_support:
         :param HybridShapeDirection i_dir:
         :param float i_angle:
         :param int i_orientation_support:
@@ -4682,42 +4682,42 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewReflectLineWithType(Reference iSupport,
                 | HybridShapeDirection iDir,
                 | double iAngle,
                 | long iOrientationSupport,
                 | long iOrientationDirection,
                 | long iType) As HybridShapeReflectLine
-                | 
+                |
                 |     Creates a new ReflectLine within the current body.
                 |     Create a reflectline curve on a support surface along a direction with an
                 |     angle.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iSupport
-                |             Support surface. 
+                |             Support surface.
                 |         iAngle
-                |             Angle of the reflectline. 
+                |             Angle of the reflectline.
                 |         iOrientationSupport
                 |             Manage the angle used to compute the reflectline. Value can be 1 or
-                |             -1 
+                |             -1
                 |         iOrientationDirection
                 |             Manage the angle used to compute the reflectline. Value can be 1 or
-                |             -1 
+                |             -1
                 |         iType
                 |             Manage the type used to compute the reflectline. Value can be 0 or
                 |             1 Returns or sets whether the reflectline curve is or should be created with
                 |             the normal to the support or the tangent plane to the
                 |             support.
                 |             Role: The TypeSolution indicates whether the created reflectline
                 |             curve is compute with the angle between the normale to the support and the
                 |             direction or with the angle between the tangent plane to the support and the
                 |             direction..
                 |             Legal values: 0 for the normal and 1 for the tangent plane.
-                |             
+                |
                 |         oReflectLine
                 |             Created reflectline.
 
         :param Reference i_support:
         :param HybridShapeDirection i_dir:
         :param float i_angle:
         :param int i_orientation_support:
@@ -4737,34 +4737,34 @@
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewRevol(Reference iObjectToExtrude,
                 | double iOffsetDebut,
                 | double iOffsetFin,
                 | Reference iAxis) As HybridShapeRevol
-                | 
+                |
                 |     Creates a new revolution within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObjectToExtrude
                 |             Profile to be revolved
-                | 
-                |             Sub-element(s) supported (see 
-                | 
+                |
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, TriDimFeatEdge, BiDimFeatEdge and Vertex.
-                |         
+                |
                 |     iOffsetDebut
-                |         Angle value 
+                |         Angle value
                 |     iOffsetFin
-                |         Angle value 
+                |         Angle value
                 |     iAxis
                 |         Revolution axis ( line that has to be in the profil
                 |         plane
-                | 
+                |
                 |         Sub-element(s) supported (see Boundary object): see
                 |         RectilinearTriDimFeatEdge, RectilinearBiDimFeatEdge and
                 |         RectilinearMonoDimFeatEdge.
                 |     oRevolObject
                 |         Revolved result
 
         :param Reference i_object_to_extrude:
@@ -4783,31 +4783,31 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewRotate(Reference iToRotate,
                 | Reference iAxis,
                 | double iAngle) As HybridShapeRotate
-                | 
+                |
                 |     Creates a new Rotate within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iToRotate
                 |             point, curve, surface or solid to transform.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, TriDimFeatEdge, BiDimFeatEdge and Vertex.
-                |         
+                |
                 |     iAxis
                 |         Rotation axis.
                 |         Sub-element(s) supported (see Boundary object): see
                 |         Edge.
                 |     iAngle
-                |         Rotation angle. 
+                |         Rotation angle.
                 |     oRotate
                 |         Created rotation.
 
         :param Reference i_to_rotate:
         :param Reference i_axis:
         :param float i_angle:
         :return: HybridShapeRotate
@@ -4819,19 +4819,19 @@
     def add_new_section(self) -> HybridShapeSection:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSection() As HybridShapeSection
-                | 
+                |
                 |     Creates a new section.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oSection
                 |             Created Section
 
         :return: HybridShapeSection
         :rtype: HybridShapeSection
         """
         return HybridShapeSection(self.hybrid_shape_factory.AddNewSection())
@@ -4847,36 +4847,36 @@
                 | o Func AddNewSphere(Reference iCenter,
                 | Reference iAxis,
                 | double iRadius,
                 | double iBeginParallelAngle,
                 | double iEndParallelAngle,
                 | double iBeginMeridianAngle,
                 | double iEndMeridianAngle) As HybridShapeSphere
-                | 
+                |
                 |     Creates a new Sphere within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iCenter
                 |             Sphere center.
-                |             Sub-element(s) supported (see 
-                | 
-                |         Boundary object): see Vertex. 
+                |             Sub-element(s) supported (see
+                |
+                |         Boundary object): see Vertex.
                 |     iAxis
-                |         Sphere axis 
+                |         Sphere axis
                 |     iRadius
-                |         Radius 
+                |         Radius
                 |     iBeginParallelAngle
-                |         Angle value 
+                |         Angle value
                 |     iEndParallelAngle
-                |         Angle value 
+                |         Angle value
                 |     iBeginMeridianAngle
-                |         Angle value 
+                |         Angle value
                 |     iEndMeridianAngle
-                |         Angle value 
+                |         Angle value
                 |     oSphereObject
                 |         Sphere result
 
         :param Reference i_center:
         :param Reference i_axis:
         :param float i_radius:
         :param float i_begin_parallel_angle:
@@ -4894,19 +4894,19 @@
     def add_new_spine(self) -> HybridShapeSpine:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSpine() As HybridShapeSpine
-                | 
+                |
                 |     Creates a new spine within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oExt
                 |             CATIAHybridShapeSpine created
 
         :return: HybridShapeSpine
         :rtype: HybridShapeSpine
         """
         return HybridShapeSpine(self.hybrid_shape_factory.AddNewSpine())
@@ -4920,34 +4920,34 @@
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSpiral(long iType,
                 | Reference iSupport,
                 | Reference iCenterPoint,
                 | HybridShapeDirection iAxis,
                 | double iStartingRadius,
                 | boolean iClockwiseRevolution) As HybridShapeSpiral
-                | 
+                |
                 |     Creates a new Spiral within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iType
                 |             Spiral is defined by AngleRadius, AnglePitch or PitchRadius.
-                |             
+                |
                 |         iSupport
-                |             Spiral planar support. 
+                |             Spiral planar support.
                 |         iCenterPoint
-                |             Center point. 
+                |             Center point.
                 |         iAxis
-                |             Axis. 
+                |             Axis.
                 |         iStartingRadius
                 |             Defines the starting point: distance from the center point on the
-                |             axis. 
+                |             axis.
                 |         iClockwiseRevolution
                 |             Revolutions are clockwise if TRUE, counterclockwise if FALSE.
-                |             
+                |
                 |         oSpiral
                 |             The Spiral object if succeded
 
         :param int i_type:
         :param Reference i_support:
         :param Reference i_center_point:
         :param HybridShapeDirection i_axis:
@@ -4963,19 +4963,19 @@
     def add_new_spline(self) -> HybridShapeSpline:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSpline() As HybridShapeSpline
-                | 
+                |
                 |     Creates a new Spline within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oSpline
                 |             Created spline.
 
         :return: HybridShapeSpline
         :rtype: HybridShapeSpline
         """
         return HybridShapeSpline(self.hybrid_shape_factory.AddNewSpline())
@@ -4984,22 +4984,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSurfaceDatum(Reference iObject) As
                 | HybridShapeSurfaceExplicit
-                | 
+                |
                 |     Creates a new datum of surface within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             The object whose topological body will be duplicated and put into
-                |             created datum 
+                |             created datum
                 |         oSurface
                 |             Created surface Note2: the object passed as parameter to create the
                 |             datum has to be in the current container. Otherwise, an error
                 |             occurs.
 
         :param Reference i_object:
         :return: HybridShapeSurfaceExplicit
@@ -5011,25 +5011,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSweepCircle(Reference iGuide1) As
                 | HybridShapeSweepCircle
-                | 
+                |
                 |     Creates a new SweepCircle within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iGuide1
                 |             First guide or center curve.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     oExt
                 |         Created swept surface.
 
         :param Reference i_guide1:
         :return: HybridShapeSweepCircle
         :rtype: HybridShapeSweepCircle
         """
@@ -5039,21 +5039,21 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSweepConic(Reference ipIAGuide1) As
                 | HybridShapeSweepConic
-                | 
+                |
                 |     Creates a new SweepConic within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iGuide1
-                |             First guide curve. 
+                |             First guide curve.
                 |         opIASweepConic
                 |             Created swept surface.
 
         :param Reference ip_ia_guide1:
         :return: HybridShapeSweepConic
         :rtype: HybridShapeSweepConic
         """
@@ -5063,25 +5063,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSweepExplicit(Reference iProfile,
                 | Reference iGuide) As HybridShapeSweepExplicit
-                | 
+                |
                 |     Creates a new SweepExplicit within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iProfile
                 |             Profile.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see TriDimFeatEdge and BiDimFeatEdge.
-                |         
+                |
                 |     iGuide
                 |         First guide curve.
                 |         Sub-element(s) supported (see Boundary object): see TriDimFeatEdge and
                 |         BiDimFeatEdge.
                 |     oExt
                 |         Created swept surface.
 
@@ -5097,21 +5097,21 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSweepLine(Reference iGuide1) As
                 | HybridShapeSweepLine
-                | 
+                |
                 |     Creates a new SweepLine within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iGuide1
-                |             First guide curve. 
+                |             First guide curve.
                 |         oExt
                 |             Created swept surface.
 
         :param Reference i_guide1:
         :return: HybridShapeSweepLine
         :rtype: HybridShapeSweepLine
         """
@@ -5121,25 +5121,25 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewSymmetry(Reference iObject,
                 | Reference iReference) As HybridShapeSymmetry
-                | 
+                |
                 |     Creates a new Symmetry within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             Point, curve, surface or solid to transform.
-                |             Sub-element(s) supported (see 
-                | 
+                |             Sub-element(s) supported (see
+                |
                 |         Boundary object): see Face, TriDimFeatEdge, BiDimFeatEdge and Vertex.
-                |         
+                |
                 |     iReference
                 |         Point, line or reference plane.
                 |         Sub-element(s) supported (see Boundary object): see PlanarFace, Edge
                 |         and Vertex.
                 |     oSymmetry
                 |         Created symmetry.
 
@@ -5155,24 +5155,24 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewTransfer(Reference iElementToTransfer,
                 | long iTypeOfTransfer) As HybridShapeTransfer
-                | 
+                |
                 |     Creates a new Transfer within the current body.
                 |     Note: require DL1 license.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElementToTransfer
-                |             The element to transfer 
+                |             The element to transfer
                 |         iTypeOfTransfer
-                |             The type of transfer 
+                |             The type of transfer
                 |         oExt
                 |             Created Transfer operation.
 
         :param Reference i_element_to_transfer:
         :param int i_type_of_transfer:
         :return: HybridShapeTransfer
         :rtype: HybridShapeTransfer
@@ -5186,32 +5186,32 @@
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewTranslate(Reference iElement,
                 | HybridShapeDirection iDirection,
                 | double iDistance) As HybridShapeTranslate
-                | 
+                |
                 |     Creates a new Translate within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElement
-                |             Point, curve, surface or solid to translate. 
+                |             Point, curve, surface or solid to translate.
                 |         iDirection
-                |             Translation direction. 
+                |             Translation direction.
                 |         iDistance
-                |             Translation Distance. 
+                |             Translation Distance.
                 |         oTranslate
-                |             Created translation 
+                |             Created translation
                 |         oTranslate
                 |             Created Translate (Empty feature)
                 |             Note: Then translate mode and inputs has to be initialized
-                |             
-                | 
+                |
+                |
                 |     See also:
                 |         HybridShapeTranslate
 
         :param Reference i_element:
         :param HybridShapeDirection i_direction:
         :param float i_distance:
         :return: HybridShapeTranslate
@@ -5223,20 +5223,20 @@
     def add_new_unfold(self) -> HybridShapeUnfold:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewUnfold() As HybridShapeUnfold
-                | 
+                |
                 |     Creates a new Unfold within the current body.
                 |     Note: require DL1 license.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oExt
                 |             Created unfold operation.
 
         :return: HybridShapeUnfold
         :rtype: HybridShapeUnfold
         """
         return HybridShapeUnfold(self.hybrid_shape_factory.AddNewUnfold())
@@ -5245,23 +5245,23 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewVolumeDatum(Reference iObject) As
                 | HybridShapeVolumeExplicit
-                | 
+                |
                 |     Creates a new datum of volume within the current body.
                 |     Note: requires GSO License
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             The object whose topological body will be duplicated and put into
-                |             created datum 
+                |             created datum
                 |         oVolume
                 |             Created Volume Note2: the object passed as parameter to create the
                 |             datum has to be in the current container. Otherwise, an error
                 |             occurs.
 
         :param Reference i_object:
         :return: HybridShapeVolumeExplicit
@@ -5272,20 +5272,20 @@
     def add_new_wrap_curve(self) -> HybridShapeWrapCurve:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewWrapCurve() As HybridShapeWrapCurve
-                | 
+                |
                 |     Creates a new Wrap Curve Surface within the current body.
                 |     Note: require GSO license.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         oWrapCurve
                 |             The Wrap Curve object if succeded
 
         :return: HybridShapeWrapCurve
         :rtype: HybridShapeWrapCurve
         """
         return HybridShapeWrapCurve(self.hybrid_shape_factory.AddNewWrapCurve())
@@ -5294,22 +5294,22 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func AddNewWrapSurface(Reference iBodyToDeform) As
                 | HybridShapeWrapSurface
-                | 
+                |
                 |     Creates a new Wrap Surface within the current body.
                 |     Note: require GSO license.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         :
-                |             iBodyToDeform Body to deform with a Wrap Surface 
+                |             iBodyToDeform Body to deform with a Wrap Surface
                 |         oWrapSurface
                 |             The Wrap Surface object if succeded
 
         :param Reference i_body_to_deform:
         :return: HybridShapeWrapSurface
         :rtype: HybridShapeWrapSurface
         """
@@ -5319,31 +5319,31 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Sub ChangeFeatureName(Reference iElem,
                 | CATBSTR Name)
-                | 
+                |
                 |     Set display name for Shape Design Features.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElem
-                |             Element to rename 
+                |             Element to rename
                 |         Name
                 |             User name
 
         :param Reference i_elem:
         :param str name:
         :return: None
         :rtype: None
         """
         return self.hybrid_shape_factory.ChangeFeatureName(i_elem.com_object, name)
-        # # # # Autogenerated comment: 
+        # # # # Autogenerated comment:
         # # some methods require a system service call as the methods expects a vb array object
         # # passed to it and there is no way to do this directly with python. In those cases the following code
         # # should be uncommented and edited accordingly. Otherwise completely remove all this.
         # # vba_function_name = 'change_feature_name'
         # # vba_code = """
         # # Public Function change_feature_name(hybrid_shape_factory)
         # #     Dim iElem (2)
@@ -5358,28 +5358,28 @@
     def delete_object_for_datum(self, i_object: Reference) -> None:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Sub DeleteObjectForDatum(Reference iObject)
-                | 
+                |
                 |     Deletes an object within the current body.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iObject
                 |             Object to delete
 
         :param Reference i_object:
         :return: None
         :rtype: None
         """
         return self.hybrid_shape_factory.DeleteObjectForDatum(i_object.com_object)
-        # # # # Autogenerated comment: 
+        # # # # Autogenerated comment:
         # # some methods require a system service call as the methods expects a vb array object
         # # passed to it and there is no way to do this directly with python. In those cases the following code
         # # should be uncommented and edited accordingly. Otherwise completely remove all this.
         # # vba_function_name = 'delete_object_for_datum'
         # # vba_code = """
         # # Public Function delete_object_for_datum(hybrid_shape_factory)
         # #     Dim iObject (2)
@@ -5395,31 +5395,31 @@
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Sub GSMVisibility(Reference iElem,
                 | long Show)
-                | 
+                |
                 |     Set Visibility attribut for Shape Design Features.
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElem
-                |             Element to show/NoShow 
+                |             Element to show/NoShow
                 |         Show
                 |             = 0 NoShow , 1= Show
 
         :param Reference i_elem:
         :param int show:
         :return: None
         :rtype: None
         """
         return self.hybrid_shape_factory.GSMVisibility(i_elem.com_object, show)
-        # # # # Autogenerated comment: 
+        # # # # Autogenerated comment:
         # # some methods require a system service call as the methods expects a vb array object
         # # passed to it and there is no way to do this directly with python. In those cases the following code
         # # should be uncommented and edited accordingly. Otherwise completely remove all this.
         # # vba_function_name = 'gsm_visibility'
         # # vba_code = """
         # # Public Function gsm_visibility(hybrid_shape_factory)
         # #     Dim iElem (2)
@@ -5434,21 +5434,21 @@
     def get_geometrical_feature_type(self, i_elem: Reference) -> int:
         """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-07-06 14:02:20.222384))
                 | o Func GetGeometricalFeatureType(Reference iElem) As short
-                | 
+                |
                 |     Returns type of "geometrical" shape Design feature .
-                | 
+                |
                 |     Parameters:
-                | 
+                |
                 |         iElem
-                |             Reference element 
+                |             Reference element
                 |         oType
                 |             Type of feature
                 |             0 = Unknown, 1 = Point,  2 = Curve, 3 = Line, 4 = Circle,
                 |             5 = Surface, 6 = Plane, 7 = Solid / Volume
                 |             Level of availability = V5R14
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_fill.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fill.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_bi_tangent.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_bi_tangent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_tri_tangent.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_fillet_tri_tangent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_healing.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_healing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_helix.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_helix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_integrated_law.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_integrated_law.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_intersection.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_intersection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_inverse.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_inverse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_law_dist_proj.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_law_dist_proj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_angle.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_angle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bi_tangent.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bi_tangent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bisecting.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_bisecting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_explicit.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_explicit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_normal.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_normal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_dir.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_dir.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_pt.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_pt_pt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_line_tangency.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_line_tangency.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_loft.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_loft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_mid_surface.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_mid_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_near.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_near.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_offset.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_offset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_curve.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_line1_pt.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane1_line1_pt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane2_lines.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane2_lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane3_points.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane3_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_angle.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_angle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_equation.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_equation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_explicit.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_explicit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_mean.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_mean.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_normal.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_normal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset_pt.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_offset_pt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_tangent.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_plane_tangent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_between.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_between.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_center.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_center.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_coord.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_coord.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_explicit.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_explicit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_curve.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_plane.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_surface.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_on_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_point_tangent.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_point_tangent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_polyline.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_polyline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_position_transfo.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_position_transfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_project.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_reflect_line.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_reflect_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_revol.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_revol.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_rolling_offset.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_rolling_offset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_rotate.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_rotate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_scaling.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_scaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_section.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_section.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sphere.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sphere.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_spine.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_spiral.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spiral.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_spline.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_spline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_split.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_split.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_surface_explicit.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_surface_explicit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_circle.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_circle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_conic.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_conic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_explicit.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_explicit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_line.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_sweep_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_symmetry.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_symmetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_thickness.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_thickness.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_transfer.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_translate.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_translate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_trim.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_trim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_unfold.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_unfold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_volume_explicit.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_volume_explicit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_curve.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_surface.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/hybrid_shape_wrap_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/line.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/plane.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/hybrid_shape_interfaces/point.py` & `pycatia-0.5.8/pycatia/hybrid_shape_interfaces/point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/application.py` & `pycatia-0.5.8/pycatia/in_interfaces/application.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/camera.py` & `pycatia-0.5.8/pycatia/in_interfaces/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/camera_2d.py` & `pycatia-0.5.8/pycatia/in_interfaces/camera_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/camera_3d.py` & `pycatia-0.5.8/pycatia/in_interfaces/camera_3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/cameras.py` & `pycatia-0.5.8/pycatia/in_interfaces/cameras.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/cgr_adhesion_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/cgr_adhesion_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/document.py` & `pycatia-0.5.8/pycatia/in_interfaces/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/documentation_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/documentation_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/documents.py` & `pycatia-0.5.8/pycatia/in_interfaces/documents.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,16 @@
                 |          Set PartDoc = Documents.Add("Part")
 
         :param str document_type:
         :return: Document
         :rtype: Document
         """
 
-        # document_types = ['Part', 'Product', 'Drawing', 'FunctionalSystem']
-        # if document_type not in document_types:
-        #     raise ValueError(f'Document type {document_type} must be in {document_types}')
+        # document_types string must be one of these types:
+        # 'Part', 'Product', 'Drawing', 'FunctionalSystem', 'CATMaterial', 'CatalogDocument'
 
         dt = get_document_type(document_type)
 
         self.logger.info(f'Creating a new "{dt}".')
 
         return Document(self.documents.Add(dt))
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/drafting_page_setup.py` & `pycatia-0.5.8/pycatia/in_interfaces/drafting_page_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/file.py` & `pycatia-0.5.8/pycatia/in_interfaces/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/file_component.py` & `pycatia-0.5.8/pycatia/in_interfaces/file_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/file_system.py` & `pycatia-0.5.8/pycatia/in_interfaces/file_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/files.py` & `pycatia-0.5.8/pycatia/in_interfaces/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/folder.py` & `pycatia-0.5.8/pycatia/in_interfaces/folder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/folders.py` & `pycatia-0.5.8/pycatia/in_interfaces/folders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/general_session_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/general_session_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/light_source.py` & `pycatia-0.5.8/pycatia/in_interfaces/light_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/light_sources.py` & `pycatia-0.5.8/pycatia/in_interfaces/light_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/macros_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/macros_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/move.py` & `pycatia-0.5.8/pycatia/in_interfaces/move.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/page_setup.py` & `pycatia-0.5.8/pycatia/in_interfaces/page_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/position.py` & `pycatia-0.5.8/pycatia/in_interfaces/position.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/printer.py` & `pycatia-0.5.8/pycatia/in_interfaces/printer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/printers.py` & `pycatia-0.5.8/pycatia/in_interfaces/printers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/printers_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/printers_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/reference.py` & `pycatia-0.5.8/pycatia/in_interfaces/reference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/references.py` & `pycatia-0.5.8/pycatia/in_interfaces/references.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/search_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/search_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/selected_element.py` & `pycatia-0.5.8/pycatia/in_interfaces/selected_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/selection.py` & `pycatia-0.5.8/pycatia/in_interfaces/selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-03 17:02:05.216737
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/selection_sets.py` & `pycatia-0.5.8/pycatia/in_interfaces/selection_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/send_to_service.py` & `pycatia-0.5.8/pycatia/in_interfaces/send_to_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/setting_controllers.py` & `pycatia-0.5.8/pycatia/in_interfaces/setting_controllers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/specs_and_geom_window.py` & `pycatia-0.5.8/pycatia/in_interfaces/specs_and_geom_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/specs_viewer.py` & `pycatia-0.5.8/pycatia/in_interfaces/specs_viewer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/system_configuration.py` & `pycatia-0.5.8/pycatia/in_interfaces/system_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/text_stream.py` & `pycatia-0.5.8/pycatia/in_interfaces/text_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/tree_viz_manip_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/tree_viz_manip_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/viewer.py` & `pycatia-0.5.8/pycatia/in_interfaces/viewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/viewer_2d.py` & `pycatia-0.5.8/pycatia/in_interfaces/viewer_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/viewer_3d.py` & `pycatia-0.5.8/pycatia/in_interfaces/viewer_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/viewers.py` & `pycatia-0.5.8/pycatia/in_interfaces/viewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/viewpoint_2d.py` & `pycatia-0.5.8/pycatia/in_interfaces/viewpoint_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/viewpoint_3d.py` & `pycatia-0.5.8/pycatia/in_interfaces/viewpoint_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/vis_property_set.py` & `pycatia-0.5.8/pycatia/in_interfaces/vis_property_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/visualization_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/visualization_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/vrml_setting_att.py` & `pycatia-0.5.8/pycatia/in_interfaces/vrml_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/window.py` & `pycatia-0.5.8/pycatia/in_interfaces/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/windows.py` & `pycatia-0.5.8/pycatia/in_interfaces/windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/in_interfaces/workbench.py` & `pycatia-0.5.8/pycatia/in_interfaces/workbench.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/angle.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/angle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/bool_param.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/bool_param.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/check.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/constraint_satisfaction.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/constraint_satisfaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/design_table.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/design_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/dimension.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/dimension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/enum_param.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/enum_param.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/feature_generator.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/feature_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/formula.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/formula.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/free_parameter.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/free_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/free_parameters.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/free_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/int_param.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/int_param.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/knowledge_activate_object.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/knowledge_activate_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/knowledge_object.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/knowledge_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/knowledge_sheet_setting_att.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/knowledge_sheet_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/language_sheet_setting_att.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/language_sheet_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/law.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/law.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/length.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/length.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/list.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/list_parameter.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/list_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/loop.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/optimization.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/optimization_constraint.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/optimization_constraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/optimization_constraints.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/optimization_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/optimizations.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/optimizations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/parameter.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/parameter_set.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/parameter_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/parameter_sets.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/parameter_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/parameters.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/real_param.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/real_param.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/relation.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/relations.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/relations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/report_generation_sheet_setting_att.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/report_generation_sheet_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/rule.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/set_of_equation.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/set_of_equation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/str_param.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/str_param.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/tolerance_sheet_setting_att.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/tolerance_sheet_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/unit.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/units.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/knowledge_interfaces/units_sheet_setting_att.py` & `pycatia-0.5.8/pycatia/knowledge_interfaces/units_sheet_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/axis_system.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/axis_system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
@@ -160,15 +160,15 @@
 
     @origin_point.setter
     def origin_point(self, value: Reference):
         """
         :param Reference value:
         """
 
-        self.axis_system.OriginPoint = value
+        self.axis_system.OriginPoint = value.com_object
 
     @property
     def origin_type(self) -> int:
         """
         .. note::
             :class: toggle
 
@@ -292,15 +292,15 @@
 
     @x_axis_direction.setter
     def x_axis_direction(self, value: Reference):
         """
         :param Reference value:
         """
 
-        self.axis_system.XAxisDirection = value
+        self.axis_system.XAxisDirection = value.com_object
 
     @property
     def x_axis_type(self) -> int:
         """
         .. note::
             :class: toggle
 
@@ -378,15 +378,15 @@
 
     @y_axis_direction.setter
     def y_axis_direction(self, value: Reference):
         """
         :param Reference value:
         """
 
-        self.axis_system.YAxisDirection = value
+        self.axis_system.YAxisDirection = value.com_object
 
     @property
     def y_axis_type(self) -> int:
         """
         .. note::
             :class: toggle
 
@@ -464,15 +464,15 @@
 
     @z_axis_direction.setter
     def z_axis_direction(self, value: Reference):
         """
         :param Reference value:
         """
 
-        self.axis_system.ZAxisDirection = value
+        self.axis_system.ZAxisDirection = value.com_object
 
     @property
     def z_axis_type(self) -> int:
         """
         .. note::
             :class: toggle
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/axis_systems.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/axis_systems.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/bi_dim_feat_edge.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/bi_dim_feat_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/bodies.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/bodies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/body.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/boundary.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/constraint.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/constraint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/constraints.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/cylindrical_face.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/cylindrical_face.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/edge.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/face.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/face.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/factory.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/fix_together.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/fix_together.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/fix_togethers.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/fix_togethers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/geometric_elements.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/geometric_elements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_bodies.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_bodies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_body.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_shape.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_shape_instance.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_shape_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/hybrid_shapes.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/hybrid_shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/instance_factory.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/instance_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/mono_dim_feat_edge.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/mono_dim_feat_edge.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/not_wire_boundary_mono_dim_feat_vertex.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/not_wire_boundary_mono_dim_feat_vertex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/ordered_geometrical_set.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/ordered_geometrical_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/ordered_geometrical_sets.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/ordered_geometrical_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/origin_elements.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/origin_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/part.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/part.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/part_document.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/part_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/part_infrastructure_setting_att.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/part_infrastructure_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/planar_face.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/planar_face.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/rectilinear_bi_dim_feat_edge.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/rectilinear_bi_dim_feat_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/rectilinear_mono_dim_feat_edge.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/rectilinear_mono_dim_feat_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/rectilinear_tri_dim_feat_edge.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/rectilinear_tri_dim_feat_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/shape.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/shape_instance.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/shape_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/shapes.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/sketches.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/sketches.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/solid.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/solid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/tri_dim_feat_edge.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/tri_dim_feat_edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/tri_dim_feat_vertex_or_bi_dim_feat_vertex.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/tri_dim_feat_vertex_or_bi_dim_feat_vertex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/vertex.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/vertex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/mec_mod_interfaces/zero_dim_feat_vertex_or_wire_boundary_mono_dim_feat_vertex.py` & `pycatia-0.5.8/pycatia/mec_mod_interfaces/zero_dim_feat_vertex_or_wire_boundary_mono_dim_feat_vertex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/annotated_view.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/annotated_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/annotated_views.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/annotated_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/dmu_data_flow.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/dmu_data_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/dmu_review.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/dmu_review.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/dmu_reviews.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/dmu_reviews.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/group.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/groups.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/hyperlink.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/hyperlink.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/hyperlinks.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/hyperlinks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/marker_2D.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/marker_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/marker_2Ds.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/marker_2Ds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/marker_3D.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/marker_3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/marker_3Ds.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/marker_3Ds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/marker_setting_att.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/marker_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/n_4D_navigator_setting_att.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/n_4D_navigator_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/navigator_interfaces/navigator_workbench.py` & `pycatia-0.5.8/pycatia/navigator_interfaces/navigator_workbench.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/add.py` & `pycatia-0.5.8/pycatia/part_interfaces/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/affinity.py` & `pycatia-0.5.8/pycatia/part_interfaces/affinity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/angular_repartition.py` & `pycatia-0.5.8/pycatia/part_interfaces/angular_repartition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/assemble.py` & `pycatia-0.5.8/pycatia/part_interfaces/assemble.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/auto_draft.py` & `pycatia-0.5.8/pycatia/part_interfaces/auto_draft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/auto_fillet.py` & `pycatia-0.5.8/pycatia/part_interfaces/auto_fillet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/axis_to_axis.py` & `pycatia-0.5.8/pycatia/part_interfaces/axis_to_axis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/boolean_shape.py` & `pycatia-0.5.8/pycatia/part_interfaces/boolean_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/chamfer.py` & `pycatia-0.5.8/pycatia/part_interfaces/chamfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/circ_pattern.py` & `pycatia-0.5.8/pycatia/part_interfaces/circ_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/close_surface.py` & `pycatia-0.5.8/pycatia/part_interfaces/close_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/const_rad_edge_fillet.py` & `pycatia-0.5.8/pycatia/part_interfaces/const_rad_edge_fillet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/defeaturing.py` & `pycatia-0.5.8/pycatia/part_interfaces/defeaturing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/defeaturing_fillet_filter.py` & `pycatia-0.5.8/pycatia/part_interfaces/defeaturing_hole_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
         
 """
 
 from pycatia.part_interfaces.defeaturing_filter_with_range import DefeaturingFilterWithRange
 
 
-class DefeaturingFilletFilter(DefeaturingFilterWithRange):
+class DefeaturingHoleFilter(DefeaturingFilterWithRange):
     """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-06-11 12:40:47.360445)
 
                 | System.IUnknown
                 |     System.IDispatch
                 |         System.CATBaseUnknown
                 |             System.CATBaseDispatch
                 |                 System.AnyObject
                 |                     PartInterfaces.DefeaturingFilter
                 |                        PartInterfaces.DefeaturingFilterWithRange
-                |                             DefeaturingFilletFilter
+                |                             DefeaturingHoleFilter
                 | 
-                | Represents the defeaturing fillet filter.
+                | Represents the defeaturing hole filter.
 
     """
 
     def __init__(self, com_object):
         super().__init__(com_object)
-        self.defeaturing_fillet_filter = com_object
+        self.defeaturing_hole_filter = com_object
 
     def __repr__(self):
-        return f'DefeaturingFilletFilter(name="{self.name}")'
+        return f'DefeaturingHoleFilter(name="{self.name}")'
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/defeaturing_filter.py` & `pycatia-0.5.8/pycatia/part_interfaces/defeaturing_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/defeaturing_filter_with_range.py` & `pycatia-0.5.8/pycatia/part_interfaces/defeaturing_filter_with_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/defeaturing_filters.py` & `pycatia-0.5.8/pycatia/part_interfaces/defeaturing_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/defeaturing_hole_filter.py` & `pycatia-0.5.8/pycatia/part_interfaces/defeaturing_fillet_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
         
 """
 
 from pycatia.part_interfaces.defeaturing_filter_with_range import DefeaturingFilterWithRange
 
 
-class DefeaturingHoleFilter(DefeaturingFilterWithRange):
+class DefeaturingFilletFilter(DefeaturingFilterWithRange):
     """
         .. note::
             :class: toggle
 
             CAA V5 Visual Basic Help (2020-06-11 12:40:47.360445)
 
                 | System.IUnknown
                 |     System.IDispatch
                 |         System.CATBaseUnknown
                 |             System.CATBaseDispatch
                 |                 System.AnyObject
                 |                     PartInterfaces.DefeaturingFilter
                 |                        PartInterfaces.DefeaturingFilterWithRange
-                |                             DefeaturingHoleFilter
+                |                             DefeaturingFilletFilter
                 | 
-                | Represents the defeaturing hole filter.
+                | Represents the defeaturing fillet filter.
 
     """
 
     def __init__(self, com_object):
         super().__init__(com_object)
-        self.defeaturing_hole_filter = com_object
+        self.defeaturing_fillet_filter = com_object
 
     def __repr__(self):
-        return f'DefeaturingHoleFilter(name="{self.name}")'
+        return f'DefeaturingFilletFilter(name="{self.name}")'
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/draft.py` & `pycatia-0.5.8/pycatia/part_interfaces/draft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/draft_domain.py` & `pycatia-0.5.8/pycatia/part_interfaces/draft_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/draft_domains.py` & `pycatia-0.5.8/pycatia/part_interfaces/draft_domains.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/dress_up_shape.py` & `pycatia-0.5.8/pycatia/part_interfaces/dress_up_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/edge_fillet.py` & `pycatia-0.5.8/pycatia/part_interfaces/edge_fillet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/face_fillet.py` & `pycatia-0.5.8/pycatia/part_interfaces/face_fillet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/fillet.py` & `pycatia-0.5.8/pycatia/part_interfaces/fillet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/groove.py` & `pycatia-0.5.8/pycatia/part_interfaces/groove.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/hole.py` & `pycatia-0.5.8/pycatia/part_interfaces/hole.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/intersect.py` & `pycatia-0.5.8/pycatia/part_interfaces/intersect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/limit.py` & `pycatia-0.5.8/pycatia/part_interfaces/limit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
@@ -105,11 +105,11 @@
 
     @limiting_element.setter
     def limiting_element(self, value: Reference):
         """
         :param Reference value:
         """
 
-        self.limit.LimitingElement = value
+        self.limit.LimitingElement = value.com_object
 
     def __repr__(self):
         return f'Limit(name="{ self.name }")'
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/linear_repartition.py` & `pycatia-0.5.8/pycatia/part_interfaces/linear_repartition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/loft.py` & `pycatia-0.5.8/pycatia/part_interfaces/loft.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/mirror.py` & `pycatia-0.5.8/pycatia/part_interfaces/mirror.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/pad.py` & `pycatia-0.5.8/pycatia/part_interfaces/pad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/pattern.py` & `pycatia-0.5.8/pycatia/part_interfaces/pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/pocket.py` & `pycatia-0.5.8/pycatia/part_interfaces/pocket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/prism.py` & `pycatia-0.5.8/pycatia/part_interfaces/prism.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/rect_pattern.py` & `pycatia-0.5.8/pycatia/part_interfaces/rect_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/remove.py` & `pycatia-0.5.8/pycatia/part_interfaces/remove.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/remove_face.py` & `pycatia-0.5.8/pycatia/part_interfaces/remove_face.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/repartition.py` & `pycatia-0.5.8/pycatia/part_interfaces/repartition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/replace_face.py` & `pycatia-0.5.8/pycatia/part_interfaces/replace_face.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/revolution.py` & `pycatia-0.5.8/pycatia/part_interfaces/revolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/rib.py` & `pycatia-0.5.8/pycatia/part_interfaces/rib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/rotate.py` & `pycatia-0.5.8/pycatia/part_interfaces/rotate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/scaling.py` & `pycatia-0.5.8/pycatia/part_interfaces/scaling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/scaling2.py` & `pycatia-0.5.8/pycatia/part_interfaces/scaling2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/sew_surface.py` & `pycatia-0.5.8/pycatia/part_interfaces/sew_surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/shaft.py` & `pycatia-0.5.8/pycatia/part_interfaces/shaft.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/shape_factory.py` & `pycatia-0.5.8/pycatia/part_interfaces/shape_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/shell.py` & `pycatia-0.5.8/pycatia/part_interfaces/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/sketch_based_shape.py` & `pycatia-0.5.8/pycatia/part_interfaces/sketch_based_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/slot.py` & `pycatia-0.5.8/pycatia/part_interfaces/slot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/solid_combine.py` & `pycatia-0.5.8/pycatia/part_interfaces/solid_combine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/split.py` & `pycatia-0.5.8/pycatia/part_interfaces/split.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/stiffener.py` & `pycatia-0.5.8/pycatia/part_interfaces/stiffener.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/surface_based_shape.py` & `pycatia-0.5.8/pycatia/part_interfaces/surface_based_shape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/sweep.py` & `pycatia-0.5.8/pycatia/part_interfaces/sweep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/symmetry.py` & `pycatia-0.5.8/pycatia/part_interfaces/symmetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/thick_surface.py` & `pycatia-0.5.8/pycatia/part_interfaces/thick_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/thickness.py` & `pycatia-0.5.8/pycatia/part_interfaces/thickness.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/thread.py` & `pycatia-0.5.8/pycatia/part_interfaces/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/transformation_shape.py` & `pycatia-0.5.8/pycatia/part_interfaces/transformation_shape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/translate.py` & `pycatia-0.5.8/pycatia/part_interfaces/translate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/trim.py` & `pycatia-0.5.8/pycatia/part_interfaces/trim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/tritangent_fillet.py` & `pycatia-0.5.8/pycatia/part_interfaces/tritangent_fillet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/user_pattern.py` & `pycatia-0.5.8/pycatia/part_interfaces/user_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/user_repartition.py` & `pycatia-0.5.8/pycatia/part_interfaces/user_repartition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/part_interfaces/var_rad_edge_fillet.py` & `pycatia-0.5.8/pycatia/part_interfaces/var_rad_edge_fillet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/product_structure_interfaces/analyze.py` & `pycatia-0.5.8/pycatia/product_structure_interfaces/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/product_structure_interfaces/assembly_convertor.py` & `pycatia-0.5.8/pycatia/product_structure_interfaces/assembly_convertor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/product_structure_interfaces/product.py` & `pycatia-0.5.8/pycatia/product_structure_interfaces/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/product_structure_interfaces/product_document.py` & `pycatia-0.5.8/pycatia/product_structure_interfaces/product_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/product_structure_interfaces/products.py` & `pycatia-0.5.8/pycatia/product_structure_interfaces/products.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/product_structure_interfaces/publication.py` & `pycatia-0.5.8/pycatia/product_structure_interfaces/publication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/product_structure_interfaces/publications.py` & `pycatia-0.5.8/pycatia/product_structure_interfaces/publications.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/scripts/csv_tools.py` & `pycatia-0.5.8/pycatia/scripts/csv_tools.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/scripts/document_types.py` & `pycatia-0.5.8/pycatia/scripts/document_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from pycatia.exception_handling import CATIAApplicationException
 
 allowed_document_types = {
     'part': 'Part',
     'product': 'Product',
     'drawing': 'Drawing',
     'functionalsystem': 'FunctionalSystem',
+    'catmaterial': 'CATMaterial',
+    'catalogdocument': 'CatalogDocument'
 }
 
 
 def get_document_type(dt: str) -> str:
     """
 
     This allows some flexibility regarding use of case.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/axis_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/axis_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/circle_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/circle_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/control_point_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/control_point_2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/curve_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/curve_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/ellipse_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/ellipse_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/factory_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/factory_2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/geometric_element.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/geometric_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/geometry_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/geometry_2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/hyperbola_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/hyperbola_2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/line_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/line_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/parabola_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/parabola_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/point_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/point_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/sketch.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/sketch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/sketcher_interfaces/spline_2D.py` & `pycatia-0.5.8/pycatia/sketcher_interfaces/spline_2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/clash.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/clash.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/clash_result.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/clash_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/clash_results.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/clash_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/clashes.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/clashes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/conflict.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/conflict.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/conflicts.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/conflicts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/distance.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/distances.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/distances.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/inertia.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/inertia.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/inertias.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/inertias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/measurable.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/measurable.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/measure_setting_att.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/measure_setting_att.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/section.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/section.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-07-06 14:02:20.222384
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/sectioning_setting_att.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/sectioning_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/sections.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/sections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/space_analyses_interfaces/spa_workbench.py` & `pycatia-0.5.8/pycatia/space_analyses_interfaces/spa_workbench.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-11 12:40:47.360445
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/accesslog_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/accesslog_statistics_setting_att.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/any_object.py` & `pycatia-0.5.8/pycatia/system_interfaces/any_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/cache_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/cache_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/cat_base_dispatch.py` & `pycatia-0.5.8/pycatia/system_interfaces/cat_base_dispatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/cat_base_unknown.py` & `pycatia-0.5.8/pycatia/system_interfaces/cat_base_unknown.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/collection.py` & `pycatia-0.5.8/pycatia/system_interfaces/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-10 10:58:07.270911
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/command_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/command_statistics_setting_att.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/disconnection_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/disconnection_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/dl_name_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/dl_name_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/dyn_license_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/dyn_license_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/errorlog_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/errorlog_statistics_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/file_access_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/file_access_statistics_setting_att.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/general_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/general_statistics_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/global_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/global_statistics_setting_att.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/i_dispatch.py` & `pycatia-0.5.8/pycatia/system_interfaces/i_dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/i_unknown.py` & `pycatia-0.5.8/pycatia/system_interfaces/i_unknown.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/license_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/license_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/memory_warning_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/memory_warning_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/pcs_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/pcs_statistics_setting_att.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/server_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/server_statistics_setting_att.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/session_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/session_statistics_setting_att.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/setting_controller.py` & `pycatia-0.5.8/pycatia/system_interfaces/setting_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/setting_repository.py` & `pycatia-0.5.8/pycatia/system_interfaces/setting_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/system_service.py` & `pycatia-0.5.8/pycatia/system_interfaces/system_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/system_interfaces/workbench_statistics_setting_att.py` & `pycatia-0.5.8/pycatia/system_interfaces/workbench_statistics_setting_att.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-06-09 09:53:18.676780
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/annotation.py` & `pycatia-0.5.8/pycatia/tps_interfaces/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/annotation_2.py` & `pycatia-0.5.8/pycatia/tps_interfaces/annotation_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/annotation_factory.py` & `pycatia-0.5.8/pycatia/tps_interfaces/annotation_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/annotation_factory_2.py` & `pycatia-0.5.8/pycatia/tps_interfaces/annotation_factory_2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/annotation_set.py` & `pycatia-0.5.8/pycatia/tps_interfaces/annotation_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/annotation_set_transform_into_assembly_set.py` & `pycatia-0.5.8/pycatia/tps_interfaces/annotation_set_transform_into_assembly_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/annotation_sets.py` & `pycatia-0.5.8/pycatia/tps_interfaces/annotation_sets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/annotations.py` & `pycatia-0.5.8/pycatia/tps_interfaces/annotations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/assembly_annotation_sets.py` & `pycatia-0.5.8/pycatia/tps_interfaces/assembly_annotation_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/associated_ref_frame.py` & `pycatia-0.5.8/pycatia/tps_interfaces/associated_ref_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/capture.py` & `pycatia-0.5.8/pycatia/tps_interfaces/capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/capture_factory.py` & `pycatia-0.5.8/pycatia/tps_interfaces/capture_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/captures.py` & `pycatia-0.5.8/pycatia/tps_interfaces/captures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/composite_tolerance.py` & `pycatia-0.5.8/pycatia/tps_interfaces/composite_tolerance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/controlled_radius.py` & `pycatia-0.5.8/pycatia/tps_interfaces/controlled_radius.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/datum_simple.py` & `pycatia-0.5.8/pycatia/tps_interfaces/datum_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/datum_target.py` & `pycatia-0.5.8/pycatia/tps_interfaces/datum_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/default_annotation.py` & `pycatia-0.5.8/pycatia/tps_interfaces/default_annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/dimension_3d.py` & `pycatia-0.5.8/pycatia/tps_interfaces/dimension_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/dimension_limit.py` & `pycatia-0.5.8/pycatia/tps_interfaces/dimension_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/dimension_pattern.py` & `pycatia-0.5.8/pycatia/tps_interfaces/dimension_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/dmu_tol_setting_att.py` & `pycatia-0.5.8/pycatia/tps_interfaces/dmu_tol_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/envelope_condition.py` & `pycatia-0.5.8/pycatia/tps_interfaces/envelope_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/flag_note.py` & `pycatia-0.5.8/pycatia/tps_interfaces/flag_note.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/free_state.py` & `pycatia-0.5.8/pycatia/tps_interfaces/free_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/fta_infra_setting_att.py` & `pycatia-0.5.8/pycatia/tps_interfaces/fta_infra_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/fta_setting_att.py` & `pycatia-0.5.8/pycatia/tps_interfaces/fta_setting_att.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/material_condition.py` & `pycatia-0.5.8/pycatia/tps_interfaces/material_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/noa.py` & `pycatia-0.5.8/pycatia/tps_interfaces/noa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/non_semantic_datum.py` & `pycatia-0.5.8/pycatia/tps_interfaces/non_semantic_datum.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/non_semantic_datum_target.py` & `pycatia-0.5.8/pycatia/tps_interfaces/non_semantic_datum_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/non_semantic_dimension.py` & `pycatia-0.5.8/pycatia/tps_interfaces/non_semantic_dimension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/non_semantic_gdt.py` & `pycatia-0.5.8/pycatia/tps_interfaces/non_semantic_gdt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/particular_tol_elem.py` & `pycatia-0.5.8/pycatia/tps_interfaces/particular_tol_elem.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/projected_tolerance_zone.py` & `pycatia-0.5.8/pycatia/tps_interfaces/projected_tolerance_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/reference_frame.py` & `pycatia-0.5.8/pycatia/tps_interfaces/reference_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/roughness.py` & `pycatia-0.5.8/pycatia/tps_interfaces/roughness.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/semantic_gdt.py` & `pycatia-0.5.8/pycatia/tps_interfaces/semantic_gdt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/shifted_profile_tolerance.py` & `pycatia-0.5.8/pycatia/tps_interfaces/shifted_profile_tolerance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/tangent_plane.py` & `pycatia-0.5.8/pycatia/tps_interfaces/tangent_plane.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/text.py` & `pycatia-0.5.8/pycatia/tps_interfaces/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/tolerance_per_unit_basis_restrictive_value.py` & `pycatia-0.5.8/pycatia/tps_interfaces/tolerance_per_unit_basis_restrictive_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/tolerance_unit_basis_value.py` & `pycatia-0.5.8/pycatia/tps_interfaces/tolerance_unit_basis_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/tolerance_zone.py` & `pycatia-0.5.8/pycatia/tps_interfaces/tolerance_zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/tps_parallel_on_screen.py` & `pycatia-0.5.8/pycatia/tps_interfaces/tps_parallel_on_screen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/tps_view.py` & `pycatia-0.5.8/pycatia/tps_interfaces/tps_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/tps_view_factory.py` & `pycatia-0.5.8/pycatia/tps_interfaces/tps_view_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/tps_views.py` & `pycatia-0.5.8/pycatia/tps_interfaces/tps_views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/user_surface.py` & `pycatia-0.5.8/pycatia/tps_interfaces/user_surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/user_surfaces.py` & `pycatia-0.5.8/pycatia/tps_interfaces/user_surfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/tps_interfaces/weld.py` & `pycatia-0.5.8/pycatia/tps_interfaces/weld.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! usr/bin/python3.6
+#! usr/bin/python3.9
 """
     Module initially auto generated using V5Automation files from CATIA V5 R28 on 2020-09-25 14:34:21.593357
 
     .. warning::
         The notes denoted "CAA V5 Visual Basic Help" are to be used as reference only.
         They are there as a guide as to how the visual basic / catscript functions work
         and thus help debugging in pycatia.
```

### Comparing `pycatia-0.5.7/pycatia/types/document_types.py` & `pycatia-0.5.8/pycatia/types/document_types.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia/types/general.py` & `pycatia-0.5.8/pycatia/types/general.py`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/pycatia.egg-info/PKG-INFO` & `pycatia-0.5.8/pycatia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycatia
-Version: 0.5.7
+Version: 0.5.8
 Summary: A python module to access the CATIA Measurable object.
 Home-page: https://github.com/evereux/pycatia
 Author: Paul Bourne
 Author-email: evereux@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pycatia-0.5.7/pycatia.egg-info/SOURCES.txt` & `pycatia-0.5.8/pycatia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycatia-0.5.7/setup.py` & `pycatia-0.5.8/setup.py`

 * *Files identical despite different names*

