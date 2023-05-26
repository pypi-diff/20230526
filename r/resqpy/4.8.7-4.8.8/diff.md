# Comparing `tmp/resqpy-4.8.7.tar.gz` & `tmp/resqpy-4.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resqpy-4.8.7.tar", max compression
+gzip compressed data, was "resqpy-4.8.8.tar", max compression
```

## Comparing `resqpy-4.8.7.tar` & `resqpy-4.8.8.tar`

### file list

```diff
@@ -1,198 +1,198 @@
--rw-r--r--   0        0        0     1059 2023-05-18 20:33:38.671707 resqpy-4.8.7/LICENSE
--rw-r--r--   0        0        0     2893 2023-05-18 20:33:38.671707 resqpy-4.8.7/README.md
--rw-r--r--   0        0        0     3227 2023-05-18 20:33:54.331737 resqpy-4.8.7/pyproject.toml
--rw-r--r--   0        0        0      555 2023-05-18 20:33:54.331737 resqpy-4.8.7/resqpy/__init__.py
--rw-r--r--   0        0        0    24782 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/crs.py
--rw-r--r--   0        0        0     1982 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/__init__.py
--rw-r--r--   0        0        0     6410 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/_add_edges_per_column_property_array.py
--rw-r--r--   0        0        0    21022 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/_add_faults.py
--rw-r--r--   0        0        0     6417 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/_add_one_blocked_well_property.py
--rw-r--r--   0        0        0     8657 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/_add_one_grid_property_array.py
--rw-r--r--   0        0        0     2431 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/_add_single_cell_grid.py
--rw-r--r--   0        0        0     5495 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/_add_wells_from_ascii_file.py
--rw-r--r--   0        0        0     6037 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/_add_zone_by_layer_property.py
--rw-r--r--   0        0        0    11586 2023-05-18 20:33:38.683707 resqpy-4.8.7/resqpy/derived_model/_coarsened_grid.py
--rw-r--r--   0        0        0    10520 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_common.py
--rw-r--r--   0        0        0     3730 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_copy_grid.py
--rw-r--r--   0        0        0    11731 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_drape_to_surface.py
--rw-r--r--   0        0        0    16391 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_extract_box.py
--rw-r--r--   0        0        0    22969 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_extract_box_for_well.py
--rw-r--r--   0        0        0    20325 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_fault_throw_scaling.py
--rw-r--r--   0        0        0     7157 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_gather_ensemble.py
--rw-r--r--   0        0        0    17929 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_interpolated_grid.py
--rw-r--r--   0        0        0     9876 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_local_depth_adjustment.py
--rw-r--r--   0        0        0    20513 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_refined_grid.py
--rw-r--r--   0        0        0     5166 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_tilted_grid.py
--rw-r--r--   0        0        0     4792 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_unsplit_grid.py
--rw-r--r--   0        0        0    18825 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_zonal_grid.py
--rw-r--r--   0        0        0     4358 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/derived_model/_zone_layer_ranges_from_array.py
--rw-r--r--   0        0        0      996 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/fault/__init__.py
--rw-r--r--   0        0        0    29402 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/fault/_gcs_functions.py
--rw-r--r--   0        0        0   109110 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/fault/_grid_connection_set.py
--rw-r--r--   0        0        0      692 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/__init__.py
--rw-r--r--   0        0        0    20689 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/_cell_properties.py
--rw-r--r--   0        0        0    10120 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/_connection_sets.py
--rw-r--r--   0        0        0    19936 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/_create_grid_xml.py
--rw-r--r--   0        0        0    32064 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/_defined_geometry.py
--rw-r--r--   0        0        0    28203 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/_extract_functions.py
--rw-r--r--   0        0        0    16516 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/_face_functions.py
--rw-r--r--   0        0        0    12236 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/_faults.py
--rw-r--r--   0        0        0   127766 2023-05-18 20:33:38.687707 resqpy-4.8.7/resqpy/grid/_grid.py
--rw-r--r--   0        0        0     3544 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_grid_types.py
--rw-r--r--   0        0        0      338 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_intervals_info.py
--rw-r--r--   0        0        0      604 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_moved_functions.py
--rw-r--r--   0        0        0     7243 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_pillars.py
--rw-r--r--   0        0        0     5386 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_pixel_maps.py
--rw-r--r--   0        0        0    65440 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_points_functions.py
--rw-r--r--   0        0        0    45761 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_regular_grid.py
--rw-r--r--   0        0        0    19413 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_transmissibility.py
--rw-r--r--   0        0        0     7944 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_write_hdf5_from_caches.py
--rw-r--r--   0        0        0     6147 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_write_nexus_corp.py
--rw-r--r--   0        0        0    13087 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid/_xyz.py
--rw-r--r--   0        0        0     2593 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid_surface/__init__.py
--rw-r--r--   0        0        0    35739 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid_surface/_blocked_well_populate.py
--rw-r--r--   0        0        0    64016 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid_surface/_find_faces.py
--rw-r--r--   0        0        0    26056 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid_surface/_grid_skin.py
--rw-r--r--   0        0        0    14379 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid_surface/_grid_surface.py
--rw-r--r--   0        0        0    22498 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid_surface/_trajectory_intersects.py
--rw-r--r--   0        0        0    39760 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/grid_surface/grid_surface_cuda.py
--rw-r--r--   0        0        0      539 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/lines/__init__.py
--rw-r--r--   0        0        0    11960 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/lines/_common.py
--rw-r--r--   0        0        0    41425 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/lines/_polyline.py
--rw-r--r--   0        0        0    26366 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/lines/_polyline_set.py
--rw-r--r--   0        0        0      378 2023-05-18 20:33:38.691707 resqpy-4.8.7/resqpy/model/__init__.py
--rw-r--r--   0        0        0    30205 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/model/_catalogue.py
--rw-r--r--   0        0        0     2840 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/model/_context.py
--rw-r--r--   0        0        0    34552 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/model/_forestry.py
--rw-r--r--   0        0        0     3371 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/model/_grids.py
--rw-r--r--   0        0        0    14238 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/model/_hdf5.py
--rw-r--r--   0        0        0   103055 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/model/_model.py
--rw-r--r--   0        0        0    23589 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/model/_xml.py
--rw-r--r--   0        0        0      909 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/multi_processing/__init__.py
--rw-r--r--   0        0        0     7301 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/multi_processing/_multiprocessing.py
--rw-r--r--   0        0        0       72 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/multi_processing/wrappers/__init__.py
--rw-r--r--   0        0        0     5952 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/multi_processing/wrappers/blocked_well_mp.py
--rw-r--r--   0        0        0    21156 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/multi_processing/wrappers/grid_surface_mp.py
--rw-r--r--   0        0        0     5793 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/multi_processing/wrappers/mesh_mp.py
--rw-r--r--   0        0        0       84 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/__init__.py
--rw-r--r--   0        0        0     2147 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/ab_toolbox.py
--rw-r--r--   0        0        0     7521 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/base.py
--rw-r--r--   0        0        0    20925 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/box_utilities.py
--rw-r--r--   0        0        0     5935 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/class_dict.py
--rw-r--r--   0        0        0     9489 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/consolidation.py
--rw-r--r--   0        0        0     5177 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/data/build.py
--rw-r--r--   0        0        0   498136 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/data/properties.json
--rw-r--r--   0        0        0    19836 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/dataframe.py
--rw-r--r--   0        0        0      307 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/exceptions.py
--rw-r--r--   0        0        0     1313 2023-05-18 20:33:38.695707 resqpy-4.8.7/resqpy/olio/factors.py
--rw-r--r--   0        0        0    24541 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/fine_coarse.py
--rw-r--r--   0        0        0    27669 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/grid_functions.py
--rw-r--r--   0        0        0    20158 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/intersection.py
--rw-r--r--   0        0        0     8408 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/keyword_files.py
--rw-r--r--   0        0        0    19210 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/load_data.py
--rw-r--r--   0        0        0     6628 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/point_inclusion.py
--rw-r--r--   0        0        0     1103 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/random_seed.py
--rw-r--r--   0        0        0     5441 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/read_nexus_fault.py
--rw-r--r--   0        0        0    17083 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/relperm.py
--rw-r--r--   0        0        0    12189 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/simple_lines.py
--rw-r--r--   0        0        0      760 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/time.py
--rw-r--r--   0        0        0      822 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/trademark.py
--rw-r--r--   0        0        0    61869 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/transmission.py
--rw-r--r--   0        0        0    44768 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/triangulation.py
--rw-r--r--   0        0        0     7324 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/uuid.py
--rw-r--r--   0        0        0    45231 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/vdb.py
--rw-r--r--   0        0        0    46253 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/vector_utilities.py
--rw-r--r--   0        0        0     6185 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/volume.py
--rw-r--r--   0        0        0    26220 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/wellspec_keywords.py
--rw-r--r--   0        0        0     5142 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/write_data.py
--rw-r--r--   0        0        0    19055 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/write_hdf5.py
--rw-r--r--   0        0        0    24925 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/xml_et.py
--rw-r--r--   0        0        0     1824 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/xml_namespaces.py
--rw-r--r--   0        0        0     5709 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/olio/zmap_reader.py
--rw-r--r--   0        0        0     2206 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/__init__.py
--rw-r--r--   0        0        0     2937 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/_utils.py
--rw-r--r--   0        0        0     1685 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/boundary_feature.py
--rw-r--r--   0        0        0     5190 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/boundary_feature_interpretation.py
--rw-r--r--   0        0        0     6186 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/earth_model_interpretation.py
--rw-r--r--   0        0        0    12457 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/fault_interpretation.py
--rw-r--r--   0        0        0     2757 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/fluid_boundary_feature.py
--rw-r--r--   0        0        0     1702 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/frontier_feature.py
--rw-r--r--   0        0        0     4498 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/generic_interpretation.py
--rw-r--r--   0        0        0     3771 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/genetic_boundary_feature.py
--rw-r--r--   0        0        0     8605 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/geobody_boundary_interpretation.py
--rw-r--r--   0        0        0     1836 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/geobody_feature.py
--rw-r--r--   0        0        0     8052 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/geobody_interpretation.py
--rw-r--r--   0        0        0     1739 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/geologic_unit_feature.py
--rw-r--r--   0        0        0     8346 2023-05-18 20:33:38.699707 resqpy-4.8.7/resqpy/organize/horizon_interpretation.py
--rw-r--r--   0        0        0     2697 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/organize/organization_feature.py
--rw-r--r--   0        0        0     5565 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/organize/rock_fluid_unit_feature.py
--rw-r--r--   0        0        0     1802 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/organize/structural_organization_interpretation.py
--rw-r--r--   0        0        0     2675 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/organize/tectonic_boundary_feature.py
--rw-r--r--   0        0        0     1843 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/organize/wellbore_feature.py
--rw-r--r--   0        0        0     6973 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/organize/wellbore_interpretation.py
--rw-r--r--   0        0        0     2155 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/__init__.py
--rw-r--r--   0        0        0    16697 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/_collection_add_part.py
--rw-r--r--   0        0        0    12926 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/_collection_create_xml.py
--rw-r--r--   0        0        0    30090 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/_collection_get_attributes.py
--rw-r--r--   0        0        0     5368 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/_collection_support.py
--rw-r--r--   0        0        0    24426 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/_property.py
--rw-r--r--   0        0        0    66946 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/grid_property_collection.py
--rw-r--r--   0        0        0   143306 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/property_collection.py
--rw-r--r--   0        0        0    36127 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/property_common.py
--rw-r--r--   0        0        0     5557 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/property_kind.py
--rw-r--r--   0        0        0     7737 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/string_lookup.py
--rw-r--r--   0        0        0     1077 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/well_interval_property.py
--rw-r--r--   0        0        0     1577 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/well_interval_property_collection.py
--rw-r--r--   0        0        0     1205 2023-05-18 20:33:38.703707 resqpy-4.8.7/resqpy/property/well_log.py
--rw-r--r--   0        0        0     7633 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/property/well_log_collection.py
--rw-r--r--   0        0        0      713 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/rq_import/__init__.py
--rw-r--r--   0        0        0     4493 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/rq_import/_add_ab_properties.py
--rw-r--r--   0        0        0     6067 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/rq_import/_add_surfaces.py
--rw-r--r--   0        0        0    32019 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/rq_import/_grid_from_cp.py
--rw-r--r--   0        0        0    34317 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/rq_import/_import_nexus.py
--rw-r--r--   0        0        0     6306 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/rq_import/_import_vdb_all_grids.py
--rw-r--r--   0        0        0    21372 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/rq_import/_import_vdb_ensemble.py
--rw-r--r--   0        0        0     1311 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/strata/__init__.py
--rw-r--r--   0        0        0     8861 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/strata/_binary_contact_interpretation.py
--rw-r--r--   0        0        0    10381 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/strata/_geologic_unit_interpretation.py
--rw-r--r--   0        0        0     1772 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/strata/_strata_common.py
--rw-r--r--   0        0        0     6797 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/strata/_stratigraphic_column.py
--rw-r--r--   0        0        0    13322 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/strata/_stratigraphic_column_rank.py
--rw-r--r--   0        0        0     7432 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/strata/_stratigraphic_unit_feature.py
--rw-r--r--   0        0        0    10167 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/strata/_stratigraphic_unit_interpretation.py
--rw-r--r--   0        0        0      696 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/surface/__init__.py
--rw-r--r--   0        0        0     2331 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/surface/_base_surface.py
--rw-r--r--   0        0        0     3082 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/surface/_combined_surface.py
--rw-r--r--   0        0        0    42192 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/surface/_mesh.py
--rw-r--r--   0        0        0    26120 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/surface/_pointset.py
--rw-r--r--   0        0        0    56386 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/surface/_surface.py
--rw-r--r--   0        0        0    24315 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/surface/_tri_mesh.py
--rw-r--r--   0        0        0    25907 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/surface/_triangulated_patch.py
--rw-r--r--   0        0        0     1074 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/time_series/__init__.py
--rw-r--r--   0        0        0     8595 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/time_series/_any_time_series.py
--rw-r--r--   0        0        0     6617 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/time_series/_from_nexus_summary.py
--rw-r--r--   0        0        0     6366 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/time_series/_functions.py
--rw-r--r--   0        0        0     3311 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/time_series/_geologic_time_series.py
--rw-r--r--   0        0        0     2759 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/time_series/_time_duration.py
--rw-r--r--   0        0        0    10818 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/time_series/_time_series.py
--rw-r--r--   0        0        0      603 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/unstructured/__init__.py
--rw-r--r--   0        0        0    15328 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/unstructured/_hexa_grid.py
--rw-r--r--   0        0        0    35856 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/unstructured/_prism_grid.py
--rw-r--r--   0        0        0     7862 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/unstructured/_pyramid_grid.py
--rw-r--r--   0        0        0    10208 2023-05-18 20:33:38.707707 resqpy-4.8.7/resqpy/unstructured/_tetra_grid.py
--rw-r--r--   0        0        0    51550 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/unstructured/_unstructured_grid.py
--rw-r--r--   0        0        0     1135 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/weights_and_measures/__init__.py
--rw-r--r--   0        0        0     5434 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/weights_and_measures/nexus_units.py
--rw-r--r--   0        0        0    16186 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/weights_and_measures/weights_and_measures.py
--rw-r--r--   0        0        0      990 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/__init__.py
--rw-r--r--   0        0        0   187787 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/_blocked_well.py
--rw-r--r--   0        0        0    22138 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/_deviation_survey.py
--rw-r--r--   0        0        0     7154 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/_md_datum.py
--rw-r--r--   0        0        0    48693 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/_trajectory.py
--rw-r--r--   0        0        0    15192 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/_wellbore_frame.py
--rw-r--r--   0        0        0     8403 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/_wellbore_marker.py
--rw-r--r--   0        0        0    20933 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/_wellbore_marker_frame.py
--rw-r--r--   0        0        0    22555 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/blocked_well_frame.py
--rw-r--r--   0        0        0    24703 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/well_object_funcs.py
--rw-r--r--   0        0        0     5969 2023-05-18 20:33:38.711707 resqpy-4.8.7/resqpy/well/well_utils.py
--rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 resqpy-4.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-26 11:30:20.997823 resqpy-4.8.8/LICENSE
+-rw-r--r--   0        0        0     2893 2023-05-26 11:30:20.997823 resqpy-4.8.8/README.md
+-rw-r--r--   0        0        0     3354 2023-05-26 11:30:39.059405 resqpy-4.8.8/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-05-26 11:30:39.059405 resqpy-4.8.8/resqpy/__init__.py
+-rw-r--r--   0        0        0    24782 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/crs.py
+-rw-r--r--   0        0        0     1982 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/__init__.py
+-rw-r--r--   0        0        0     6410 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_add_edges_per_column_property_array.py
+-rw-r--r--   0        0        0    21022 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_add_faults.py
+-rw-r--r--   0        0        0     6417 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_add_one_blocked_well_property.py
+-rw-r--r--   0        0        0     8657 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_add_one_grid_property_array.py
+-rw-r--r--   0        0        0     2431 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_add_single_cell_grid.py
+-rw-r--r--   0        0        0     5495 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_add_wells_from_ascii_file.py
+-rw-r--r--   0        0        0     6037 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_add_zone_by_layer_property.py
+-rw-r--r--   0        0        0    11586 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_coarsened_grid.py
+-rw-r--r--   0        0        0    10520 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_common.py
+-rw-r--r--   0        0        0     3730 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_copy_grid.py
+-rw-r--r--   0        0        0    11731 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_drape_to_surface.py
+-rw-r--r--   0        0        0    16391 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_extract_box.py
+-rw-r--r--   0        0        0    22969 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_extract_box_for_well.py
+-rw-r--r--   0        0        0    20325 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_fault_throw_scaling.py
+-rw-r--r--   0        0        0     7157 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_gather_ensemble.py
+-rw-r--r--   0        0        0    17929 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_interpolated_grid.py
+-rw-r--r--   0        0        0     9876 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_local_depth_adjustment.py
+-rw-r--r--   0        0        0    20513 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_refined_grid.py
+-rw-r--r--   0        0        0     5166 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_tilted_grid.py
+-rw-r--r--   0        0        0     4792 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_unsplit_grid.py
+-rw-r--r--   0        0        0    18825 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_zonal_grid.py
+-rw-r--r--   0        0        0     4358 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/derived_model/_zone_layer_ranges_from_array.py
+-rw-r--r--   0        0        0      996 2023-05-26 11:30:21.013824 resqpy-4.8.8/resqpy/fault/__init__.py
+-rw-r--r--   0        0        0    29402 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/fault/_gcs_functions.py
+-rw-r--r--   0        0        0   109110 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/fault/_grid_connection_set.py
+-rw-r--r--   0        0        0      692 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/__init__.py
+-rw-r--r--   0        0        0    20689 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_cell_properties.py
+-rw-r--r--   0        0        0    10120 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_connection_sets.py
+-rw-r--r--   0        0        0    19936 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_create_grid_xml.py
+-rw-r--r--   0        0        0    32064 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_defined_geometry.py
+-rw-r--r--   0        0        0    28203 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_extract_functions.py
+-rw-r--r--   0        0        0    16516 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_face_functions.py
+-rw-r--r--   0        0        0    12236 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_faults.py
+-rw-r--r--   0        0        0   127766 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_grid.py
+-rw-r--r--   0        0        0     3544 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_grid_types.py
+-rw-r--r--   0        0        0      338 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_intervals_info.py
+-rw-r--r--   0        0        0      604 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_moved_functions.py
+-rw-r--r--   0        0        0     7243 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_pillars.py
+-rw-r--r--   0        0        0     5386 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_pixel_maps.py
+-rw-r--r--   0        0        0    65440 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_points_functions.py
+-rw-r--r--   0        0        0    45761 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_regular_grid.py
+-rw-r--r--   0        0        0    19413 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_transmissibility.py
+-rw-r--r--   0        0        0     7944 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_write_hdf5_from_caches.py
+-rw-r--r--   0        0        0     6147 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_write_nexus_corp.py
+-rw-r--r--   0        0        0    13087 2023-05-26 11:30:21.017825 resqpy-4.8.8/resqpy/grid/_xyz.py
+-rw-r--r--   0        0        0     2593 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/grid_surface/__init__.py
+-rw-r--r--   0        0        0    35739 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/grid_surface/_blocked_well_populate.py
+-rw-r--r--   0        0        0    64016 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/grid_surface/_find_faces.py
+-rw-r--r--   0        0        0    26056 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/grid_surface/_grid_skin.py
+-rw-r--r--   0        0        0    14379 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/grid_surface/_grid_surface.py
+-rw-r--r--   0        0        0    22498 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/grid_surface/_trajectory_intersects.py
+-rw-r--r--   0        0        0    39760 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/grid_surface/grid_surface_cuda.py
+-rw-r--r--   0        0        0      539 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/lines/__init__.py
+-rw-r--r--   0        0        0    11960 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/lines/_common.py
+-rw-r--r--   0        0        0    41425 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/lines/_polyline.py
+-rw-r--r--   0        0        0    26366 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/lines/_polyline_set.py
+-rw-r--r--   0        0        0      378 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/model/__init__.py
+-rw-r--r--   0        0        0    30205 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/model/_catalogue.py
+-rw-r--r--   0        0        0     2840 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/model/_context.py
+-rw-r--r--   0        0        0    34552 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/model/_forestry.py
+-rw-r--r--   0        0        0     3371 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/model/_grids.py
+-rw-r--r--   0        0        0    14238 2023-05-26 11:30:21.021825 resqpy-4.8.8/resqpy/model/_hdf5.py
+-rw-r--r--   0        0        0   103055 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/model/_model.py
+-rw-r--r--   0        0        0    23589 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/model/_xml.py
+-rw-r--r--   0        0        0      909 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/multi_processing/__init__.py
+-rw-r--r--   0        0        0     7301 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/multi_processing/_multiprocessing.py
+-rw-r--r--   0        0        0       72 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/multi_processing/wrappers/__init__.py
+-rw-r--r--   0        0        0     5952 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/multi_processing/wrappers/blocked_well_mp.py
+-rw-r--r--   0        0        0    21156 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/multi_processing/wrappers/grid_surface_mp.py
+-rw-r--r--   0        0        0     5793 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/multi_processing/wrappers/mesh_mp.py
+-rw-r--r--   0        0        0       84 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/olio/__init__.py
+-rw-r--r--   0        0        0     2147 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/olio/ab_toolbox.py
+-rw-r--r--   0        0        0     7521 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/olio/base.py
+-rw-r--r--   0        0        0    20925 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/olio/box_utilities.py
+-rw-r--r--   0        0        0     5935 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/olio/class_dict.py
+-rw-r--r--   0        0        0     9489 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/olio/consolidation.py
+-rw-r--r--   0        0        0     5177 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/olio/data/build.py
+-rw-r--r--   0        0        0   498136 2023-05-26 11:30:21.025825 resqpy-4.8.8/resqpy/olio/data/properties.json
+-rw-r--r--   0        0        0    19836 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/dataframe.py
+-rw-r--r--   0        0        0      307 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/exceptions.py
+-rw-r--r--   0        0        0     1313 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/factors.py
+-rw-r--r--   0        0        0    24541 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/fine_coarse.py
+-rw-r--r--   0        0        0    27669 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/grid_functions.py
+-rw-r--r--   0        0        0    20158 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/intersection.py
+-rw-r--r--   0        0        0     8408 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/keyword_files.py
+-rw-r--r--   0        0        0    19210 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/load_data.py
+-rw-r--r--   0        0        0     6628 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/point_inclusion.py
+-rw-r--r--   0        0        0     1103 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/random_seed.py
+-rw-r--r--   0        0        0     5441 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/read_nexus_fault.py
+-rw-r--r--   0        0        0    17083 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/relperm.py
+-rw-r--r--   0        0        0    12189 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/simple_lines.py
+-rw-r--r--   0        0        0      760 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/time.py
+-rw-r--r--   0        0        0      822 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/trademark.py
+-rw-r--r--   0        0        0    61869 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/transmission.py
+-rw-r--r--   0        0        0    44768 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/triangulation.py
+-rw-r--r--   0        0        0     7324 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/uuid.py
+-rw-r--r--   0        0        0    45231 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/vdb.py
+-rw-r--r--   0        0        0    46253 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/vector_utilities.py
+-rw-r--r--   0        0        0     6185 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/volume.py
+-rw-r--r--   0        0        0    26220 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/wellspec_keywords.py
+-rw-r--r--   0        0        0     5142 2023-05-26 11:30:21.029826 resqpy-4.8.8/resqpy/olio/write_data.py
+-rw-r--r--   0        0        0    19055 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/olio/write_hdf5.py
+-rw-r--r--   0        0        0    24925 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/olio/xml_et.py
+-rw-r--r--   0        0        0     1824 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/olio/xml_namespaces.py
+-rw-r--r--   0        0        0     5709 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/olio/zmap_reader.py
+-rw-r--r--   0        0        0     2206 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/__init__.py
+-rw-r--r--   0        0        0     2937 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/_utils.py
+-rw-r--r--   0        0        0     1685 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/boundary_feature.py
+-rw-r--r--   0        0        0     5190 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/boundary_feature_interpretation.py
+-rw-r--r--   0        0        0     6186 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/earth_model_interpretation.py
+-rw-r--r--   0        0        0    12457 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/fault_interpretation.py
+-rw-r--r--   0        0        0     2757 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/fluid_boundary_feature.py
+-rw-r--r--   0        0        0     1702 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/frontier_feature.py
+-rw-r--r--   0        0        0     4498 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/generic_interpretation.py
+-rw-r--r--   0        0        0     3771 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/genetic_boundary_feature.py
+-rw-r--r--   0        0        0     8605 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/geobody_boundary_interpretation.py
+-rw-r--r--   0        0        0     1836 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/geobody_feature.py
+-rw-r--r--   0        0        0     8052 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/geobody_interpretation.py
+-rw-r--r--   0        0        0     1739 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/geologic_unit_feature.py
+-rw-r--r--   0        0        0     8346 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/horizon_interpretation.py
+-rw-r--r--   0        0        0     2697 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/organization_feature.py
+-rw-r--r--   0        0        0     5565 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/rock_fluid_unit_feature.py
+-rw-r--r--   0        0        0     1802 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/structural_organization_interpretation.py
+-rw-r--r--   0        0        0     2675 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/tectonic_boundary_feature.py
+-rw-r--r--   0        0        0     1843 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/wellbore_feature.py
+-rw-r--r--   0        0        0     6973 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/organize/wellbore_interpretation.py
+-rw-r--r--   0        0        0     2155 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/property/__init__.py
+-rw-r--r--   0        0        0    16697 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/property/_collection_add_part.py
+-rw-r--r--   0        0        0    12926 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/property/_collection_create_xml.py
+-rw-r--r--   0        0        0    30090 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/property/_collection_get_attributes.py
+-rw-r--r--   0        0        0     5368 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/property/_collection_support.py
+-rw-r--r--   0        0        0    24426 2023-05-26 11:30:21.033826 resqpy-4.8.8/resqpy/property/_property.py
+-rw-r--r--   0        0        0    66946 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/grid_property_collection.py
+-rw-r--r--   0        0        0   143306 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/property_collection.py
+-rw-r--r--   0        0        0    36127 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/property_common.py
+-rw-r--r--   0        0        0     5557 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/property_kind.py
+-rw-r--r--   0        0        0     7737 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/string_lookup.py
+-rw-r--r--   0        0        0     1077 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/well_interval_property.py
+-rw-r--r--   0        0        0     1577 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/well_interval_property_collection.py
+-rw-r--r--   0        0        0     1205 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/well_log.py
+-rw-r--r--   0        0        0     7633 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/property/well_log_collection.py
+-rw-r--r--   0        0        0      713 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/rq_import/__init__.py
+-rw-r--r--   0        0        0     4493 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/rq_import/_add_ab_properties.py
+-rw-r--r--   0        0        0     6067 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/rq_import/_add_surfaces.py
+-rw-r--r--   0        0        0    32019 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/rq_import/_grid_from_cp.py
+-rw-r--r--   0        0        0    34317 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/rq_import/_import_nexus.py
+-rw-r--r--   0        0        0     6306 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/rq_import/_import_vdb_all_grids.py
+-rw-r--r--   0        0        0    21372 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/rq_import/_import_vdb_ensemble.py
+-rw-r--r--   0        0        0     1311 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/strata/__init__.py
+-rw-r--r--   0        0        0     8861 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/strata/_binary_contact_interpretation.py
+-rw-r--r--   0        0        0    10381 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/strata/_geologic_unit_interpretation.py
+-rw-r--r--   0        0        0     1772 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/strata/_strata_common.py
+-rw-r--r--   0        0        0     6797 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/strata/_stratigraphic_column.py
+-rw-r--r--   0        0        0    13322 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/strata/_stratigraphic_column_rank.py
+-rw-r--r--   0        0        0     7432 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/strata/_stratigraphic_unit_feature.py
+-rw-r--r--   0        0        0    10167 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/strata/_stratigraphic_unit_interpretation.py
+-rw-r--r--   0        0        0      696 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/surface/__init__.py
+-rw-r--r--   0        0        0     2331 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/surface/_base_surface.py
+-rw-r--r--   0        0        0     3082 2023-05-26 11:30:21.037826 resqpy-4.8.8/resqpy/surface/_combined_surface.py
+-rw-r--r--   0        0        0    42192 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/surface/_mesh.py
+-rw-r--r--   0        0        0    26120 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/surface/_pointset.py
+-rw-r--r--   0        0        0    56386 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/surface/_surface.py
+-rw-r--r--   0        0        0    24315 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/surface/_tri_mesh.py
+-rw-r--r--   0        0        0    25907 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/surface/_triangulated_patch.py
+-rw-r--r--   0        0        0     1074 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/time_series/__init__.py
+-rw-r--r--   0        0        0     8595 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/time_series/_any_time_series.py
+-rw-r--r--   0        0        0     6617 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/time_series/_from_nexus_summary.py
+-rw-r--r--   0        0        0     6366 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/time_series/_functions.py
+-rw-r--r--   0        0        0     3311 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/time_series/_geologic_time_series.py
+-rw-r--r--   0        0        0     2759 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/time_series/_time_duration.py
+-rw-r--r--   0        0        0    10818 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/time_series/_time_series.py
+-rw-r--r--   0        0        0      603 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/unstructured/__init__.py
+-rw-r--r--   0        0        0    15328 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/unstructured/_hexa_grid.py
+-rw-r--r--   0        0        0    35856 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/unstructured/_prism_grid.py
+-rw-r--r--   0        0        0     7862 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/unstructured/_pyramid_grid.py
+-rw-r--r--   0        0        0    10208 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/unstructured/_tetra_grid.py
+-rw-r--r--   0        0        0    51550 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/unstructured/_unstructured_grid.py
+-rw-r--r--   0        0        0     1135 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/weights_and_measures/__init__.py
+-rw-r--r--   0        0        0     5434 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/weights_and_measures/nexus_units.py
+-rw-r--r--   0        0        0    16186 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/weights_and_measures/weights_and_measures.py
+-rw-r--r--   0        0        0      990 2023-05-26 11:30:21.041827 resqpy-4.8.8/resqpy/well/__init__.py
+-rw-r--r--   0        0        0   187787 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/_blocked_well.py
+-rw-r--r--   0        0        0    22138 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/_deviation_survey.py
+-rw-r--r--   0        0        0     7154 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/_md_datum.py
+-rw-r--r--   0        0        0    50015 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/_trajectory.py
+-rw-r--r--   0        0        0    15192 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/_wellbore_frame.py
+-rw-r--r--   0        0        0     8403 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/_wellbore_marker.py
+-rw-r--r--   0        0        0    20933 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/_wellbore_marker_frame.py
+-rw-r--r--   0        0        0    22555 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/blocked_well_frame.py
+-rw-r--r--   0        0        0    24703 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/well_object_funcs.py
+-rw-r--r--   0        0        0     5969 2023-05-26 11:30:21.045827 resqpy-4.8.8/resqpy/well/well_utils.py
+-rw-r--r--   0        0        0     4106 1970-01-01 00:00:00.000000 resqpy-4.8.8/PKG-INFO
```

### Comparing `resqpy-4.8.7/LICENSE` & `resqpy-4.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/README.md` & `resqpy-4.8.8/README.md`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/pyproject.toml` & `resqpy-4.8.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 
 [build-system]
 requires = ["poetry>=1.0.2", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "resqpy"
-version = "4.8.7" # Set at build time
+version = "4.8.8" # Set at build time
 description = "Python API for working with RESQML models"
 authors = ["BP"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bp/resqpy"
 documentation = "https://resqpy.readthedocs.io/en/latest/"
 keywords = ["RESQML"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering",
     "Topic :: System :: Filesystems",
     "Topic :: Scientific/Engineering :: Information Analysis"
 ]
 include = ["data/*.json"]
 
@@ -35,20 +36,20 @@
 #   - Support all minor versions of Python released in the prior 42 months
 #   - Support all minor versions of NumPy/Pandas released in the prior 24 months
 #   - https://numpy.org/neps/nep-0029-deprecation_policy.html
 # See here for meaning of Semantic Version numbers:
 #   - https://semver.org/
 # See here for "caret" style dependency specifications:
 #   - https://python-poetry.org/docs/dependency-specification/
-python = ">= 3.8.1, < 3.11"
+python = ">= 3.8.1, < 3.12"
 numpy = "^1.23"
 pandas = "^1.4"
 h5py = "^3.7"
 lxml = "^4.9"
-lasio = "^0.30"
+lasio = "^0.31"
 scipy = "^1.9"
 numba = ">=0.56, < 1.0"
 joblib = "^1.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 pytest-cov = "^4.0"
@@ -110,9 +111,10 @@
 junit_family = "xunit2"
 testpaths = "tests/"
 filterwarnings = [
     # Error on internal deprecation warnings
     "error::DeprecationWarning:.*resqpy.*",
     # Ignore warnings that are entirely from 3rd party libs outside our control
     "ignore:.*importing the ABCs from 'collections'.*:DeprecationWarning:.*pyreadline.*",
-    "ignore:.*the imp module is deprecated in favour of importlib.*:DeprecationWarning:.*pywintypes.*"
+    "ignore:.*the imp module is deprecated in favour of importlib.*:DeprecationWarning:.*pywintypes.*",
+    "ignore:.*distutils package is deprecated.*:DeprecationWarning:.*joblib.*",
     ]
```

### Comparing `resqpy-4.8.7/resqpy/__init__.py` & `resqpy-4.8.8/resqpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,10 @@
     weights_and_measures
     well
     olio
 """
 
 import logging
 
-__version__ = "4.8.7"  # Set at build time
+__version__ = "4.8.8"  # Set at build time
 log = logging.getLogger(__name__)
 log.info(f"Imported resqpy version {__version__}")
```

### Comparing `resqpy-4.8.7/resqpy/crs.py` & `resqpy-4.8.8/resqpy/crs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/__init__.py` & `resqpy-4.8.8/resqpy/derived_model/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_add_edges_per_column_property_array.py` & `resqpy-4.8.8/resqpy/derived_model/_add_edges_per_column_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_add_faults.py` & `resqpy-4.8.8/resqpy/derived_model/_add_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_add_one_blocked_well_property.py` & `resqpy-4.8.8/resqpy/derived_model/_add_one_blocked_well_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_add_one_grid_property_array.py` & `resqpy-4.8.8/resqpy/derived_model/_add_one_grid_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_add_single_cell_grid.py` & `resqpy-4.8.8/resqpy/derived_model/_add_single_cell_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_add_wells_from_ascii_file.py` & `resqpy-4.8.8/resqpy/derived_model/_add_wells_from_ascii_file.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_add_zone_by_layer_property.py` & `resqpy-4.8.8/resqpy/derived_model/_add_zone_by_layer_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_coarsened_grid.py` & `resqpy-4.8.8/resqpy/derived_model/_coarsened_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_common.py` & `resqpy-4.8.8/resqpy/derived_model/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_copy_grid.py` & `resqpy-4.8.8/resqpy/derived_model/_copy_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_drape_to_surface.py` & `resqpy-4.8.8/resqpy/derived_model/_drape_to_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_extract_box.py` & `resqpy-4.8.8/resqpy/derived_model/_extract_box.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_extract_box_for_well.py` & `resqpy-4.8.8/resqpy/derived_model/_extract_box_for_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_fault_throw_scaling.py` & `resqpy-4.8.8/resqpy/derived_model/_fault_throw_scaling.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_gather_ensemble.py` & `resqpy-4.8.8/resqpy/derived_model/_gather_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_interpolated_grid.py` & `resqpy-4.8.8/resqpy/derived_model/_interpolated_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_local_depth_adjustment.py` & `resqpy-4.8.8/resqpy/derived_model/_local_depth_adjustment.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_refined_grid.py` & `resqpy-4.8.8/resqpy/derived_model/_refined_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_tilted_grid.py` & `resqpy-4.8.8/resqpy/derived_model/_tilted_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_unsplit_grid.py` & `resqpy-4.8.8/resqpy/derived_model/_unsplit_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_zonal_grid.py` & `resqpy-4.8.8/resqpy/derived_model/_zonal_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/derived_model/_zone_layer_ranges_from_array.py` & `resqpy-4.8.8/resqpy/derived_model/_zone_layer_ranges_from_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/fault/__init__.py` & `resqpy-4.8.8/resqpy/fault/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/fault/_gcs_functions.py` & `resqpy-4.8.8/resqpy/fault/_gcs_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/fault/_grid_connection_set.py` & `resqpy-4.8.8/resqpy/fault/_grid_connection_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/__init__.py` & `resqpy-4.8.8/resqpy/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_cell_properties.py` & `resqpy-4.8.8/resqpy/grid/_cell_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_connection_sets.py` & `resqpy-4.8.8/resqpy/grid/_connection_sets.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_create_grid_xml.py` & `resqpy-4.8.8/resqpy/grid/_create_grid_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_defined_geometry.py` & `resqpy-4.8.8/resqpy/grid/_defined_geometry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_extract_functions.py` & `resqpy-4.8.8/resqpy/grid/_extract_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_face_functions.py` & `resqpy-4.8.8/resqpy/grid/_face_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_faults.py` & `resqpy-4.8.8/resqpy/grid/_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_grid.py` & `resqpy-4.8.8/resqpy/grid/_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_grid_types.py` & `resqpy-4.8.8/resqpy/grid/_grid_types.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_moved_functions.py` & `resqpy-4.8.8/resqpy/grid/_moved_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_pillars.py` & `resqpy-4.8.8/resqpy/grid/_pillars.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_pixel_maps.py` & `resqpy-4.8.8/resqpy/grid/_pixel_maps.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_points_functions.py` & `resqpy-4.8.8/resqpy/grid/_points_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_regular_grid.py` & `resqpy-4.8.8/resqpy/grid/_regular_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_transmissibility.py` & `resqpy-4.8.8/resqpy/grid/_transmissibility.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_write_hdf5_from_caches.py` & `resqpy-4.8.8/resqpy/grid/_write_hdf5_from_caches.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_write_nexus_corp.py` & `resqpy-4.8.8/resqpy/grid/_write_nexus_corp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid/_xyz.py` & `resqpy-4.8.8/resqpy/grid/_xyz.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid_surface/__init__.py` & `resqpy-4.8.8/resqpy/grid_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid_surface/_blocked_well_populate.py` & `resqpy-4.8.8/resqpy/grid_surface/_blocked_well_populate.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid_surface/_find_faces.py` & `resqpy-4.8.8/resqpy/grid_surface/_find_faces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid_surface/_grid_skin.py` & `resqpy-4.8.8/resqpy/grid_surface/_grid_skin.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid_surface/_grid_surface.py` & `resqpy-4.8.8/resqpy/grid_surface/_grid_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid_surface/_trajectory_intersects.py` & `resqpy-4.8.8/resqpy/grid_surface/_trajectory_intersects.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/grid_surface/grid_surface_cuda.py` & `resqpy-4.8.8/resqpy/grid_surface/grid_surface_cuda.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/lines/__init__.py` & `resqpy-4.8.8/resqpy/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/lines/_common.py` & `resqpy-4.8.8/resqpy/lines/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/lines/_polyline.py` & `resqpy-4.8.8/resqpy/lines/_polyline.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/lines/_polyline_set.py` & `resqpy-4.8.8/resqpy/lines/_polyline_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/model/_catalogue.py` & `resqpy-4.8.8/resqpy/model/_catalogue.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/model/_context.py` & `resqpy-4.8.8/resqpy/model/_context.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/model/_forestry.py` & `resqpy-4.8.8/resqpy/model/_forestry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/model/_grids.py` & `resqpy-4.8.8/resqpy/model/_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/model/_hdf5.py` & `resqpy-4.8.8/resqpy/model/_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/model/_model.py` & `resqpy-4.8.8/resqpy/model/_model.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/model/_xml.py` & `resqpy-4.8.8/resqpy/model/_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/multi_processing/__init__.py` & `resqpy-4.8.8/resqpy/multi_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/multi_processing/_multiprocessing.py` & `resqpy-4.8.8/resqpy/multi_processing/_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/multi_processing/wrappers/blocked_well_mp.py` & `resqpy-4.8.8/resqpy/multi_processing/wrappers/blocked_well_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/multi_processing/wrappers/grid_surface_mp.py` & `resqpy-4.8.8/resqpy/multi_processing/wrappers/grid_surface_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/multi_processing/wrappers/mesh_mp.py` & `resqpy-4.8.8/resqpy/multi_processing/wrappers/mesh_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/ab_toolbox.py` & `resqpy-4.8.8/resqpy/olio/ab_toolbox.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/base.py` & `resqpy-4.8.8/resqpy/olio/base.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/box_utilities.py` & `resqpy-4.8.8/resqpy/olio/box_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/class_dict.py` & `resqpy-4.8.8/resqpy/olio/class_dict.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/consolidation.py` & `resqpy-4.8.8/resqpy/olio/consolidation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/data/build.py` & `resqpy-4.8.8/resqpy/olio/data/build.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/data/properties.json` & `resqpy-4.8.8/resqpy/olio/data/properties.json`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/dataframe.py` & `resqpy-4.8.8/resqpy/olio/dataframe.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/factors.py` & `resqpy-4.8.8/resqpy/olio/factors.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/fine_coarse.py` & `resqpy-4.8.8/resqpy/olio/fine_coarse.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/grid_functions.py` & `resqpy-4.8.8/resqpy/olio/grid_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/intersection.py` & `resqpy-4.8.8/resqpy/olio/intersection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/keyword_files.py` & `resqpy-4.8.8/resqpy/olio/keyword_files.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/load_data.py` & `resqpy-4.8.8/resqpy/olio/load_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/point_inclusion.py` & `resqpy-4.8.8/resqpy/olio/point_inclusion.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/random_seed.py` & `resqpy-4.8.8/resqpy/olio/random_seed.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/read_nexus_fault.py` & `resqpy-4.8.8/resqpy/olio/read_nexus_fault.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/relperm.py` & `resqpy-4.8.8/resqpy/olio/relperm.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/simple_lines.py` & `resqpy-4.8.8/resqpy/olio/simple_lines.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/time.py` & `resqpy-4.8.8/resqpy/olio/time.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/trademark.py` & `resqpy-4.8.8/resqpy/olio/trademark.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/transmission.py` & `resqpy-4.8.8/resqpy/olio/transmission.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/triangulation.py` & `resqpy-4.8.8/resqpy/olio/triangulation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/uuid.py` & `resqpy-4.8.8/resqpy/olio/uuid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/vdb.py` & `resqpy-4.8.8/resqpy/olio/vdb.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/vector_utilities.py` & `resqpy-4.8.8/resqpy/olio/vector_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/volume.py` & `resqpy-4.8.8/resqpy/olio/volume.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/wellspec_keywords.py` & `resqpy-4.8.8/resqpy/olio/wellspec_keywords.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/write_data.py` & `resqpy-4.8.8/resqpy/olio/write_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/write_hdf5.py` & `resqpy-4.8.8/resqpy/olio/write_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/xml_et.py` & `resqpy-4.8.8/resqpy/olio/xml_et.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/xml_namespaces.py` & `resqpy-4.8.8/resqpy/olio/xml_namespaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/olio/zmap_reader.py` & `resqpy-4.8.8/resqpy/olio/zmap_reader.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/__init__.py` & `resqpy-4.8.8/resqpy/organize/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/_utils.py` & `resqpy-4.8.8/resqpy/organize/_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/boundary_feature.py` & `resqpy-4.8.8/resqpy/organize/boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/boundary_feature_interpretation.py` & `resqpy-4.8.8/resqpy/organize/boundary_feature_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/earth_model_interpretation.py` & `resqpy-4.8.8/resqpy/organize/earth_model_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/fault_interpretation.py` & `resqpy-4.8.8/resqpy/organize/fault_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/fluid_boundary_feature.py` & `resqpy-4.8.8/resqpy/organize/fluid_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/frontier_feature.py` & `resqpy-4.8.8/resqpy/organize/frontier_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/generic_interpretation.py` & `resqpy-4.8.8/resqpy/organize/generic_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/genetic_boundary_feature.py` & `resqpy-4.8.8/resqpy/organize/genetic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/geobody_boundary_interpretation.py` & `resqpy-4.8.8/resqpy/organize/geobody_boundary_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/geobody_feature.py` & `resqpy-4.8.8/resqpy/organize/geobody_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/geobody_interpretation.py` & `resqpy-4.8.8/resqpy/organize/geobody_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/geologic_unit_feature.py` & `resqpy-4.8.8/resqpy/organize/geologic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/horizon_interpretation.py` & `resqpy-4.8.8/resqpy/organize/horizon_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/organization_feature.py` & `resqpy-4.8.8/resqpy/organize/organization_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/rock_fluid_unit_feature.py` & `resqpy-4.8.8/resqpy/organize/rock_fluid_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/structural_organization_interpretation.py` & `resqpy-4.8.8/resqpy/organize/structural_organization_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/tectonic_boundary_feature.py` & `resqpy-4.8.8/resqpy/organize/tectonic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/wellbore_feature.py` & `resqpy-4.8.8/resqpy/organize/wellbore_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/organize/wellbore_interpretation.py` & `resqpy-4.8.8/resqpy/organize/wellbore_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/__init__.py` & `resqpy-4.8.8/resqpy/property/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/_collection_add_part.py` & `resqpy-4.8.8/resqpy/property/_collection_add_part.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/_collection_create_xml.py` & `resqpy-4.8.8/resqpy/property/_collection_create_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/_collection_get_attributes.py` & `resqpy-4.8.8/resqpy/property/_collection_get_attributes.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/_collection_support.py` & `resqpy-4.8.8/resqpy/property/_collection_support.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/_property.py` & `resqpy-4.8.8/resqpy/property/_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/grid_property_collection.py` & `resqpy-4.8.8/resqpy/property/grid_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/property_collection.py` & `resqpy-4.8.8/resqpy/property/property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/property_common.py` & `resqpy-4.8.8/resqpy/property/property_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/property_kind.py` & `resqpy-4.8.8/resqpy/property/property_kind.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/string_lookup.py` & `resqpy-4.8.8/resqpy/property/string_lookup.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/well_interval_property.py` & `resqpy-4.8.8/resqpy/property/well_interval_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/well_interval_property_collection.py` & `resqpy-4.8.8/resqpy/property/well_interval_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/well_log.py` & `resqpy-4.8.8/resqpy/property/well_log.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/property/well_log_collection.py` & `resqpy-4.8.8/resqpy/property/well_log_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/rq_import/__init__.py` & `resqpy-4.8.8/resqpy/rq_import/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/rq_import/_add_ab_properties.py` & `resqpy-4.8.8/resqpy/rq_import/_add_ab_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/rq_import/_add_surfaces.py` & `resqpy-4.8.8/resqpy/rq_import/_add_surfaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/rq_import/_grid_from_cp.py` & `resqpy-4.8.8/resqpy/rq_import/_grid_from_cp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/rq_import/_import_nexus.py` & `resqpy-4.8.8/resqpy/rq_import/_import_nexus.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/rq_import/_import_vdb_all_grids.py` & `resqpy-4.8.8/resqpy/rq_import/_import_vdb_all_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/rq_import/_import_vdb_ensemble.py` & `resqpy-4.8.8/resqpy/rq_import/_import_vdb_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/strata/__init__.py` & `resqpy-4.8.8/resqpy/strata/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/strata/_binary_contact_interpretation.py` & `resqpy-4.8.8/resqpy/strata/_binary_contact_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/strata/_geologic_unit_interpretation.py` & `resqpy-4.8.8/resqpy/strata/_geologic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/strata/_strata_common.py` & `resqpy-4.8.8/resqpy/strata/_strata_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/strata/_stratigraphic_column.py` & `resqpy-4.8.8/resqpy/strata/_stratigraphic_column.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/strata/_stratigraphic_column_rank.py` & `resqpy-4.8.8/resqpy/strata/_stratigraphic_column_rank.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/strata/_stratigraphic_unit_feature.py` & `resqpy-4.8.8/resqpy/strata/_stratigraphic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/strata/_stratigraphic_unit_interpretation.py` & `resqpy-4.8.8/resqpy/strata/_stratigraphic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/surface/__init__.py` & `resqpy-4.8.8/resqpy/surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/surface/_base_surface.py` & `resqpy-4.8.8/resqpy/surface/_base_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/surface/_combined_surface.py` & `resqpy-4.8.8/resqpy/surface/_combined_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/surface/_mesh.py` & `resqpy-4.8.8/resqpy/surface/_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/surface/_pointset.py` & `resqpy-4.8.8/resqpy/surface/_pointset.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/surface/_surface.py` & `resqpy-4.8.8/resqpy/surface/_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/surface/_tri_mesh.py` & `resqpy-4.8.8/resqpy/surface/_tri_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/surface/_triangulated_patch.py` & `resqpy-4.8.8/resqpy/surface/_triangulated_patch.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/time_series/__init__.py` & `resqpy-4.8.8/resqpy/time_series/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/time_series/_any_time_series.py` & `resqpy-4.8.8/resqpy/time_series/_any_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/time_series/_from_nexus_summary.py` & `resqpy-4.8.8/resqpy/time_series/_from_nexus_summary.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/time_series/_functions.py` & `resqpy-4.8.8/resqpy/time_series/_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/time_series/_geologic_time_series.py` & `resqpy-4.8.8/resqpy/time_series/_geologic_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/time_series/_time_duration.py` & `resqpy-4.8.8/resqpy/time_series/_time_duration.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/time_series/_time_series.py` & `resqpy-4.8.8/resqpy/time_series/_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/unstructured/__init__.py` & `resqpy-4.8.8/resqpy/unstructured/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/unstructured/_hexa_grid.py` & `resqpy-4.8.8/resqpy/unstructured/_hexa_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/unstructured/_prism_grid.py` & `resqpy-4.8.8/resqpy/unstructured/_prism_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/unstructured/_pyramid_grid.py` & `resqpy-4.8.8/resqpy/unstructured/_pyramid_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/unstructured/_tetra_grid.py` & `resqpy-4.8.8/resqpy/unstructured/_tetra_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/unstructured/_unstructured_grid.py` & `resqpy-4.8.8/resqpy/unstructured/_unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/weights_and_measures/__init__.py` & `resqpy-4.8.8/resqpy/weights_and_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/weights_and_measures/nexus_units.py` & `resqpy-4.8.8/resqpy/weights_and_measures/nexus_units.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/weights_and_measures/weights_and_measures.py` & `resqpy-4.8.8/resqpy/weights_and_measures/weights_and_measures.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/__init__.py` & `resqpy-4.8.8/resqpy/well/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/_blocked_well.py` & `resqpy-4.8.8/resqpy/well/_blocked_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/_deviation_survey.py` & `resqpy-4.8.8/resqpy/well/_deviation_survey.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/_md_datum.py` & `resqpy-4.8.8/resqpy/well/_md_datum.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/_trajectory.py` & `resqpy-4.8.8/resqpy/well/_trajectory.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 log = logging.getLogger(__name__)
 
 import math as maths
 import numpy as np
 import pandas as pd
 from functools import partial
 
+import resqpy.crs as rqc
 import resqpy.lines as rql
 import resqpy.olio.uuid as bu
 import resqpy.olio.vector_utilities as vec
 import resqpy.olio.wellspec_keywords as wsk
 import resqpy.olio.write_hdf5 as rwh5
 import resqpy.olio.xml_et as rqet
 import resqpy.organize as rqo
-import resqpy.weights_and_measures as bwam
+import resqpy.weights_and_measures as wam
 import resqpy.well
 import resqpy.well._md_datum as rqmdd
 import resqpy.well._wellbore_frame as rqwbf
 import resqpy.well._deviation_survey as rqds
 import resqpy.well.well_utils as rqwu
 from resqpy.olio.base import BaseResqpy
 from resqpy.olio.xml_namespaces import curly_namespace as ns
@@ -362,16 +363,15 @@
 
         try:
             for col in [md_col, x_col, y_col, z_col]:
                 assert col in data_frame.columns
             self.knot_count = len(data_frame)
             assert self.knot_count >= 2  # vertical well could be hamdled by allowing a single station in survey?
             self.line_kind_index = 5  # assume minimum curvature spline
-            #         self.md_uom = bwam.p_length_unit(md_uom)
-            self.md_uom = bwam.rq_length_unit(md_uom)
+            self.md_uom = wam.rq_length_unit(md_uom)
             start = data_frame.iloc[0]
             finish = data_frame.iloc[-1]
             if title:
                 self.title = title
             self.start_md = start[md_col]
             self.finish_md = finish[md_col]
             if md_domain is not None:
@@ -397,15 +397,15 @@
         assert cell_kji0_list.ndim == 2 and cell_kji0_list.shape[1] == 3
         assert spline_mode in ['none', 'linear', 'square', 'cube']
 
         cell_centres = grid.centre_point_list(cell_kji0_list)
 
         knot_count = len(cell_kji0_list) + 2
         self.line_kind_index = 5  # 5 means minimum curvature spline; todo: set to cubic spline value?
-        self.md_uom = bwam.rq_length_unit(md_uom)
+        self.md_uom = wam.rq_length_unit(md_uom)
         self.start_md = 0.0
         points = np.empty((knot_count, 3))
         points[1:-1] = cell_centres
         points[0] = points[1]
         points[0, 2] = 0.0
         points[-1] = points[-2]
         points[-1, 2] *= 1.05
@@ -617,14 +617,37 @@
             return None
         if md <= self.start_md:
             if self.start_md == 0.0:
                 return self.md_datum.location
             return interpolate(np.array(self.md_datum.location), self.control_points[0], md / self.start_md)
         return search(md, 0, self.knot_count - 1)
 
+    def inclinations(self):
+        """Returns a numpy array of inclinations in degrees, zero being vertical, with a value per interval.
+
+        note:
+           this method returns inclinations of piecewise linear line segments between control points;
+           calling code can alternatively use the tangent vectors at knots to derive similar information
+        """
+        assert self.knot_count >= 2 and self.control_points.shape == (self.knot_count, 3)
+        crs = rqc.Crs(self.model, uuid = self.crs_uuid)
+        interval_vectors = self.control_points[1:] - self.control_points[:-1]
+        if crs.xy_units != crs.z_units:
+            wam.convert_lengths(interval_vectors[:, 2], crs.z_units, crs.xy_units)
+        if not crs.z_inc_down:
+            interval_vectors[:, 2] = -interval_vectors[:, 2]
+        interval_h = np.sqrt((interval_vectors[:, 0] * interval_vectors[:, 0]) +
+                             (interval_vectors[:, 1] * interval_vectors[:, 1]))
+        restore = np.seterr(all = 'ignore')
+        incl_radians = np.arctan(interval_h / interval_vectors[:, 2])  # horizontal / vertical
+        np.seterr(**restore)
+        incl_radians = np.where(interval_vectors[:, 2] == 0.0, maths.pi / 2.0, incl_radians)
+        incl_radians = np.where(incl_radians < 0.0, incl_radians + maths.pi, incl_radians)
+        return np.degrees(incl_radians)
+
     def splined_trajectory(self,
                            well_name,
                            min_subdivisions = 1,
                            max_segment_length = None,
                            max_degrees_per_knot = 5.0,
                            use_tangents_if_present = True,
                            store_tangents_if_calculated = True):
@@ -834,15 +857,15 @@
 
         finish_node = rqet.SubElement(wbt_node, ns['resqml2'] + 'FinishMd')
         finish_node.set(ns['xsi'] + 'type', ns['xsd'] + 'double')
         finish_node.text = str(self.finish_md)
 
         md_uom = rqet.SubElement(wbt_node, ns['resqml2'] + 'MdUom')
         md_uom.set(ns['xsi'] + 'type', ns['eml'] + 'LengthUom')
-        md_uom.text = bwam.rq_length_unit(self.md_uom)
+        md_uom.text = wam.rq_length_unit(self.md_uom)
 
         if self.md_domain:
             domain_node = rqet.SubElement(wbt_node, ns['resqml2'] + 'MdDomain')
             domain_node.set(ns['xsi'] + 'type', ns['resqml2'] + 'MdDomain')
             domain_node.text = self.md_domain
 
     def __create_wbt_node_geometry_sub_elements(self, wbt_node):
```

### Comparing `resqpy-4.8.7/resqpy/well/_wellbore_frame.py` & `resqpy-4.8.8/resqpy/well/_wellbore_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/_wellbore_marker.py` & `resqpy-4.8.8/resqpy/well/_wellbore_marker.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/_wellbore_marker_frame.py` & `resqpy-4.8.8/resqpy/well/_wellbore_marker_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/blocked_well_frame.py` & `resqpy-4.8.8/resqpy/well/blocked_well_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/well_object_funcs.py` & `resqpy-4.8.8/resqpy/well/well_object_funcs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/resqpy/well/well_utils.py` & `resqpy-4.8.8/resqpy/well/well_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.8.7/PKG-INFO` & `resqpy-4.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: resqpy
-Version: 4.8.7
+Version: 4.8.8
 Summary: Python API for working with RESQML models
 Home-page: https://github.com/bp/resqpy
 License: MIT
 Keywords: RESQML
 Author: BP
-Requires-Python: >=3.8.1,<3.11
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: System :: Filesystems
 Requires-Dist: h5py (>=3.7,<4.0)
 Requires-Dist: joblib (>=1.2,<2.0)
-Requires-Dist: lasio (>=0.30,<0.31)
+Requires-Dist: lasio (>=0.31,<0.32)
 Requires-Dist: lxml (>=4.9,<5.0)
 Requires-Dist: numba (>=0.56,<1.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: pandas (>=1.4,<2.0)
 Requires-Dist: scipy (>=1.9,<2.0)
 Project-URL: Documentation, https://resqpy.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/bp/resqpy
```

