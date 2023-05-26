# Comparing `tmp/pyaedt-0.6.76.tar.gz` & `tmp/pyaedt-0.6.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.76.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.77.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.76.tar` & `pyaedt-0.6.77.tar`

### file list

```diff
@@ -1,252 +1,252 @@
--rw-r--r--   0        0        0     1111 2023-05-18 13:27:42.185924 pyaedt-0.6.76/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-18 13:27:42.185924 pyaedt-0.6.76/README.md
--rw-r--r--   0        0        0     2634 2023-05-19 13:13:55.389500 pyaedt-0.6.76/pyaedt/__init__.py
--rw-r--r--   0        0        0    26596 2023-05-18 14:05:55.328452 pyaedt-0.6.76/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    86515 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41260 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17009 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19795 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4374 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4539 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   128111 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75493 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12433 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    37014 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62746 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/circuit.py
--rw-r--r--   0        0        0    10034 2023-05-18 13:27:43.889057 pyaedt-0.6.76/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    61908 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-18 13:27:43.904685 pyaedt-0.6.76/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-18 13:27:43.920373 pyaedt-0.6.76/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-18 13:27:43.920373 pyaedt-0.6.76/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-18 13:27:43.920373 pyaedt-0.6.76/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-18 13:27:43.935986 pyaedt-0.6.76/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-18 13:27:43.935986 pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-18 13:27:43.935986 pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-18 13:27:43.951639 pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-18 13:27:43.967239 pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-18 13:27:43.967239 pyaedt-0.6.76/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23386 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/downloads.py
--rw-r--r--   0        0        0   142256 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    92731 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32856 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40043 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      324 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/edb_builder.py
--rw-r--r--   0        0        0     1166 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12141 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65580 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20305 2023-05-18 13:27:43.982863 pyaedt-0.6.76/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4724 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61111 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32298 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    99826 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36282 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    33728 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     4147 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2425 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    64993 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2844 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-18 13:27:43.998437 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7706 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4646 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11333 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21750 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    49064 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33242 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    43680 2023-05-18 13:27:44.014060 pyaedt-0.6.76/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    46611 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57133 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   108971 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11275 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3291 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0     1074 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-05-19 05:07:06.470308 pyaedt-0.6.76/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    12191 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83387 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3395 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    68697 2023-05-19 12:41:50.180833 pyaedt-0.6.76/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62296 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-05-18 13:27:44.029696 pyaedt-0.6.76/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60355 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   252855 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   166996 2023-05-19 06:55:34.512608 pyaedt-0.6.76/pyaedt/icepak.py
--rw-r--r--   0        0        0   118454 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24259 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-18 13:27:44.045311 pyaedt-0.6.76/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3818 2023-05-19 06:53:58.810568 pyaedt-0.6.76/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-18 13:27:44.060935 pyaedt-0.6.76/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14076 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    19994 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16809 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120831 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194513 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   115362 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11332 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   127894 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    31549 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49002 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59516 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53100 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12588 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42270 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32723 2023-05-18 13:27:44.076561 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8157 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63043 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15094 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31982 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6897 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    52442 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31270 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49837 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65608 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    21640 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   114658 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51910 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40297 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82846 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28306 2023-05-18 13:27:44.092187 pyaedt-0.6.76/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53168 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11919 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26048 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   172950 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   119149 2023-05-19 05:07:06.470308 pyaedt-0.6.76/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33226 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28652 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103276 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   125048 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95851 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/q3d.py
--rw-r--r--   0        0        0    10556 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-18 13:27:44.107810 pyaedt-0.6.76/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7601 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10373 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-05-18 13:27:44.123438 pyaedt-0.6.76/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4134 2023-05-19 13:13:55.389500 pyaedt-0.6.76/pyproject.toml
--rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 pyaedt-0.6.76/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-18 13:27:42.185924 pyaedt-0.6.77/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-18 13:27:42.185924 pyaedt-0.6.77/README.md
+-rw-r--r--   0        0        0     2687 2023-05-26 13:07:30.590320 pyaedt-0.6.77/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26683 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88296 2023-05-26 11:47:35.471641 pyaedt-0.6.77/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41313 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17062 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19848 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4427 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4592 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   128774 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75522 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12462 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36747 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62954 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10034 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    64532 2023-05-26 11:47:35.471641 pyaedt-0.6.77/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-18 13:27:43.920373 pyaedt-0.6.77/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-18 13:27:43.920373 pyaedt-0.6.77/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-18 13:27:43.920373 pyaedt-0.6.77/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-18 13:27:43.935986 pyaedt-0.6.77/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-18 13:27:43.935986 pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-18 13:27:43.935986 pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-18 13:27:43.951639 pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-18 13:27:43.967239 pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-18 13:27:43.967239 pyaedt-0.6.77/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23386 2023-05-25 14:36:21.414077 pyaedt-0.6.77/pyaedt/downloads.py
+-rw-r--r--   0        0        0   143745 2023-05-26 11:30:35.579837 pyaedt-0.6.77/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    92784 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    32909 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40096 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      324 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/edb_core/edb_data/edb_builder.py
+-rw-r--r--   0        0        0      867 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12194 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65633 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20334 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     4777 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61164 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32351 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    99879 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36335 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    33757 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     4147 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2425 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    66636 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2844 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7759 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4699 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11386 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21750 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    49117 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33295 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    43733 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    46664 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57186 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   109024 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11359 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3291 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0     1091 2023-05-19 17:43:56.955082 pyaedt-0.6.77/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-05-19 05:07:06.470308 pyaedt-0.6.77/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    12244 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-26 11:30:35.579837 pyaedt-0.6.77/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83440 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3395 2023-05-19 12:41:50.180833 pyaedt-0.6.77/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    70263 2023-05-26 11:30:35.579837 pyaedt-0.6.77/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62325 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60408 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   252844 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   168413 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118475 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24312 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3818 2023-05-19 06:53:58.810568 pyaedt-0.6.77/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.77/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14105 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20047 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-18 13:27:44.076561 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16838 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120884 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   194589 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116603 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11385 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   127894 2023-05-24 13:32:35.806883 pyaedt-0.6.77/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.77/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    31587 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49055 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59074 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53129 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12641 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42625 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32776 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8210 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63096 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15147 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    32011 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6950 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    52598 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31323 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49890 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65637 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23685 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   114711 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51963 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40461 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82899 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28359 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53222 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11972 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26101 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   173003 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   119428 2023-05-26 11:30:35.579837 pyaedt-0.6.77/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33255 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28705 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103329 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   125077 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95904 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10577 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7630 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10426 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4134 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyproject.toml
+-rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 pyaedt-0.6.77/PKG-INFO
```

### Comparing `pyaedt-0.6.76/LICENSE` & `pyaedt-0.6.77/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/README.md` & `pyaedt-0.6.77/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/__init__.py` & `pyaedt-0.6.77/pyaedt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.76"
+__version__ = "0.6.77"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
 from pyaedt.generic.general_methods import _pythonver
@@ -25,14 +25,15 @@
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import generate_unique_project_name
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import is_windows
 from pyaedt.generic.general_methods import online_help
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 
 from pyaedt.aedt_logger import pyaedt_logger  # isort:skip
 
 try:
     from pyaedt.generic.design_types import Hfss3dLayout
```

### Comparing `pyaedt-0.6.76/pyaedt/aedt_logger.py` & `pyaedt-0.6.77/pyaedt/aedt_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 import logging
 from logging.handlers import RotatingFileHandler
 import os
+import shutil
 import sys
 import tempfile
 import time
 
 from pyaedt import settings
 
 message_levels = {"Global": 0, "Project": 1, "Design": 2}
@@ -158,22 +159,23 @@
         )
         my_handler.setFormatter(self.formatter)
         my_handler.setLevel(self.level)
         if not global_handler and settings.global_log_file_name:
             self._global.addHandler(my_handler)
         self._files_handlers.append(my_handler)
         if self.filename and os.path.exists(self.filename):
-            os.remove(self.filename)
+            shutil.rmtree(self.filename, ignore_errors=True)
         if self.filename and settings.enable_local_log_file:
             self.add_file_logger(self.filename, "Global", level)
 
         if to_stdout:
+            settings.enable_screen_logs = True
             self._std_out_handler = logging.StreamHandler(sys.stdout)
             self._std_out_handler.setLevel(level)
-            _logger_stdout_formatter = logging.Formatter("pyaedt %(levelname)s: %(message)s")
+            _logger_stdout_formatter = logging.Formatter("PyAEDT %(levelname)s: %(message)s")
 
             self._std_out_handler.setFormatter(_logger_stdout_formatter)
             self._global.addHandler(self._std_out_handler)
         self._timer = time.time()
 
     def add_file_logger(self, filename, project_name, level=None):
         """Add a new file to the logger handlers list."""
@@ -462,15 +464,15 @@
             if not des_name and message_levels[level] > 1:
                 des_name = self._design_name
             if des_name and ";" in des_name:
                 des_name = des_name[des_name.find(";") + 1 :]
             try:
                 self._desktop.AddMessage(proj_name, des_name, message_type, message_text)
             except:
-                print("pyaedt INFO: Failed in Adding Desktop Message")
+                print("PyAEDT INFO: Failed in Adding Desktop Message")
 
     def _log_on_handler(self, message_type, message_text, *args, **kwargs):
         if not (self._log_on_file or self._log_on_screen) or not self._global:
             return
         if len(message_text) > 250:
             message_text = message_text[:250] + "..."
         if message_type == 0:
```

### Comparing `pyaedt-0.6.76/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.77/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/application/Analysis.py` & `pyaedt-0.6.77/pyaedt/application/Analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from pyaedt.generic.constants import PLANE
 from pyaedt.generic.constants import SETUPS
 from pyaedt.generic.constants import SOLUTIONS
 from pyaedt.generic.constants import VIEW
 from pyaedt.generic.general_methods import filter_tuple
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Boundary import MaxwellParameters
 from pyaedt.modules.Boundary import NativeComponentObject
 from pyaedt.modules.DesignXPloration import OptimizationSetups
 from pyaedt.modules.DesignXPloration import ParametricSetups
 from pyaedt.modules.SolveSetup import Setup
 from pyaedt.modules.SolveSetup import SetupHFSS
@@ -1254,15 +1255,15 @@
         Create a setup and then delete it.
 
         >>> import pyaedt
         >>> hfss = pyaedt.Hfss()
         >>> setup1 = hfss.create_setup(setupname='Setup1')
         >>> hfss.delete_setup(setupname='Setup1')
         ...
-        pyaedt INFO: Sweep was deleted correctly.
+        PyAEDT INFO: Sweep was deleted correctly.
         """
         if setupname in self.existing_analysis_setups:
             self.oanalysis.DeleteSetups([setupname])
             for s in self.setups:
                 if s.name == setupname:
                     self.setups.remove(s)
             return True
@@ -1518,14 +1519,15 @@
         num_gpu=1,
         acf_file=None,
         use_auto_settings=True,
         solve_in_batch=False,
         machine="localhost",
         run_in_thread=False,
         revert_to_initial_mesh=False,
+        blocking=True,
     ):
         """Solve the active design.
 
         Parameters
         ----------
         setup_name : str, optional
             Setup to analyze. Default is ``None`` which solves all the setups.
@@ -1547,14 +1549,17 @@
         machine : str, optional
             Name of the machine if remote.  The default is ``"localhost"``.
         run_in_thread : bool, optional
             Whether to submit the batch command as a thread. The default is
             ``False``.
         revert_to_initial_mesh : bool, optional
             Whether to revert to initial mesh before solving or not. Default is ``False``.
+        blocking : bool, optional
+            Whether to block script while analysis is completed or not. It works from AEDT 2023 R2.
+            Default is ``True``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
@@ -1576,28 +1581,30 @@
                 setup_name,
                 num_cores,
                 num_tasks,
                 num_gpu,
                 acf_file,
                 use_auto_settings,
                 revert_to_initial_mesh=revert_to_initial_mesh,
+                blocking=blocking,
             )
 
     @pyaedt_function_handler()
     def analyze_setup(
         self,
         name,
         num_cores=1,
         num_tasks=1,
         num_gpu=0,
         acf_file=None,
         use_auto_settings=True,
         num_variations_to_distribute=None,
         allowed_distribution_types=None,
         revert_to_initial_mesh=False,
+        blocking=True,
     ):
         """Analyze a design setup.
 
         Parameters
         ----------
         name : str
             Name of the setup, which can be an optimetric setup or a simple setup.
@@ -1615,14 +1622,17 @@
         num_variations_to_distribute : int, optional
             Number of variations to distribute. For this to take effect ``use_auto_settings`` must be set to ``True``.
         allowed_distribution_types : list, optional
             List of strings. Each string represents a distribution type. The default value ``None`` does nothing.
             An empty list ``[]`` disables all types.
         revert_to_initial_mesh : bool, optional
             Whether to revert to initial mesh before solving or not. Default is ``False``.
+        blocking : bool, optional
+            Whether to block script while analysis is completed or not. It works from AEDT 2023 R2.
+            Default is ``True``.
 
         Returns
         -------
         bool
            ``True`` when successful, ``False`` when failed.
 
         References
@@ -1705,26 +1715,32 @@
                 self.set_registry_key(r"Desktop/ActiveDSOConfigurations/" + self.design_type, config_name)
                 set_custom_dso = True
             except:
                 pass
         if not name:
             try:
                 self.logger.info("Solving all design setups")
-                self.odesign.AnalyzeAll()
+                if self.desktop_class.aedt_version_id > "2023.1":
+                    self.odesign.AnalyzeAll(blocking)
+                else:
+                    self.odesign.AnalyzeAll()
             except:
                 if set_custom_dso:
                     self.set_registry_key(r"Desktop/ActiveDSOConfigurations/" + self.design_type, active_config)
                 self.logger.error("Error in Solving Setup %s", name)
                 return False
         elif name in self.existing_analysis_setups:
             try:
                 if revert_to_initial_mesh:
                     self.oanalysis.RevertSetupToInitial(name)
                 self.logger.info("Solving design setup %s", name)
-                self.odesign.Analyze(name)
+                if self.desktop_class.aedt_version_id > "2023.1":
+                    self.odesign.Analyze(name, blocking)
+                else:
+                    self.odesign.Analyze(name)
             except:
                 if set_custom_dso:
                     self.set_registry_key(r"Desktop/ActiveDSOConfigurations/" + self.design_type, active_config)
                 self.logger.error("Error in Solving Setup %s", name)
                 return False
         else:
             try:
@@ -1740,14 +1756,56 @@
         m, s = divmod(time.time() - start, 60)
         h, m = divmod(m, 60)
         self.logger.info(
             "Design setup {} solved correctly in {}h {}m {}s".format(name, round(h, 0), round(m, 0), round(s, 0))
         )
         return True
 
+    @property
+    def are_there_simulations_running(self):
+        """Check if there are simulation running.
+
+        .. note::
+           It works only for AEDT >= ``"2023.2"``.
+
+        Returns
+        -------
+        float
+
+        """
+        return self.desktop_class.are_there_simulations_running
+
+    @pyaedt_function_handler()
+    def get_monitor_data(self):
+        """Check and get monitor data of an existing analysis.
+
+        .. note::
+           It works only for AEDT >= ``"2023.2"``.
+
+        Returns
+        -------
+        dict
+
+        """
+        return self.desktop_class.get_monitor_data()
+
+    @pyaedt_function_handler()
+    def stop_simulations(self, clean_stop=True):
+        """Check if there are simulation running and stops them.
+
+        .. note::
+           It works only for AEDT >= ``"2023.2"``.
+
+        Returns
+        -------
+        str
+
+        """
+        return self.desktop_class.stop_simulations(clean_stop=clean_stop)
+
     @pyaedt_function_handler()
     def solve_in_batch(
         self,
         filename=None,
         machine="localhost",
         run_in_thread=False,
         num_cores=4,
```

### Comparing `pyaedt-0.6.76/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.77/pyaedt/application/Analysis3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pyaedt import settings
 from pyaedt.application.Analysis import Analysis
 from pyaedt.generic.configurations import Configurations
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class FieldAnalysis3D(Analysis, object):
     """Manages 3D field analysis setup in HFSS, Maxwell 3D, and Q3D.
 
     This class is automatically initialized by an application call from one of
```

### Comparing `pyaedt-0.6.76/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.77/pyaedt/application/Analysis3DLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 from pyaedt.application.Analysis import Analysis
 from pyaedt.generic.general_methods import is_ironpython
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSetup import Setup3DLayout
 
 
 class FieldAnalysis3DLayout(Analysis):
     """Manages 3D field analysis setup in HFSS 3D Layout.
@@ -491,15 +492,15 @@
         Create a setup and then delete it.
 
         >>> import pyaedt
         >>> hfss3dlayout = pyaedt.Hfss3dLayout()
         >>> setup1 = hfss3dlayout.create_setup(setupname='Setup1')
         >>> hfss3dlayout.delete_setup(setupname='Setup1')
         ...
-        pyaedt INFO: Sweep was deleted correctly.
+        PyAEDT INFO: Sweep was deleted correctly.
         """
         if setupname in self.existing_analysis_setups:
             self.osolution.Delete(setupname)
             for s in self.setups:
                 if s.name == setupname:
                     self.setups.remove(s)
             return True
```

### Comparing `pyaedt-0.6.76/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.77/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.77/pyaedt/application/AnalysisNexxim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pyaedt.application.Analysis import Analysis
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.circuits.object3dcircuit import CircuitComponent
 from pyaedt.modules.Boundary import CurrentSinSource
 from pyaedt.modules.Boundary import Excitations
 from pyaedt.modules.Boundary import PowerIQSource
 from pyaedt.modules.Boundary import PowerSinSource
 from pyaedt.modules.Boundary import Sources
```

### Comparing `pyaedt-0.6.76/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.77/pyaedt/application/AnalysisRMxprt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pyaedt.application.Analysis import Analysis
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class FieldAnalysisRMxprt(Analysis):
     """Manages RMXprt field analysis setup. (To be implemented.)
 
     This class is automatically initialized by an application call (like HFSS,
```

### Comparing `pyaedt-0.6.76/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.77/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pyaedt.application.Analysis import Analysis
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSetup import SetupCircuit
 
 
 class AnalysisTwinBuilder(Analysis):
     """Provides the Twin Builder Analysis Setup (TwinBuilder).
```

### Comparing `pyaedt-0.6.76/pyaedt/application/Design.py` & `pyaedt-0.6.77/pyaedt/application/Design.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import check_and_download_file
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_project_locked
 from pyaedt.generic.general_methods import is_windows
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import read_csv
 from pyaedt.generic.general_methods import read_tab
 from pyaedt.generic.general_methods import read_xlsx
 from pyaedt.generic.general_methods import settings
 from pyaedt.generic.general_methods import write_csv
 from pyaedt.modules.Boundary import BoundaryObject
@@ -102,19 +103,20 @@
         Only used when ``new_desktop_session = False``, specifies by process ID which instance
         of Electronics Desktop to point PyAEDT at.
 
     """
 
     def __str__(self):
         pyaedt_details = "      pyaedt API\n"
-        pyaedt_details += "pyaedt running AEDT Version {} \n".format(self._aedt_version)
+        pyaedt_details += "pyaedt running AEDT Version {} \n".format(settings.aedt_version)
         pyaedt_details += "Running {} tool in AEDT\n".format(self.design_type)
         pyaedt_details += "Solution Type: {} \n".format(self.solution_type)
         pyaedt_details += "Project Name: {} Design Name {} \n".format(self.project_name, self.design_name)
-        pyaedt_details += 'Project Path: "{}" \n'.format(self.project_path)
+        if self._oproject:
+            pyaedt_details += 'Project Path: "{}" \n'.format(self.project_path)
         return pyaedt_details
 
     def __exit__(self, ex_type, ex_value, ex_traceback):
         if ex_type:
             exception_to_desktop(ex_value, ex_traceback)
         if self.release_on_exit:
             self.release_desktop(self.close_on_exit, self.close_on_exit)
@@ -173,14 +175,15 @@
             and project_name
             and os.path.exists(project_name)
             and os.path.splitext(project_name)[1] == ".aedt"
         ):
             t = threading.Thread(target=load_aedt_thread, args=(project_name,))
             t.start()
         self._init_variables()
+        self._design_type = design_type
         self.last_run_log = ""
         self.last_run_job = ""
         self._design_dictionary = None
         # Get Desktop from global Desktop Environment
         self._project_dictionary = OrderedDict()
         self._boundaries = []
         self._project_datasets = {}
@@ -215,21 +218,19 @@
             )
             self.release_on_exit = False
 
         self.student_version = main_module.student_version
         if self.student_version:
             settings.disable_bounding_box_sat = True
         self._mttime = None
-        self._design_type = design_type
         self._desktop = main_module.oDesktop
 
         self._desktop_install_dir = main_module.sDesktopinstallDirectory
         self._odesign = None
         self._oproject = None
-        self._design_type = design_type
         if design_type == "HFSS":
             self.design_solutions = HFSSDesignSolution(None, design_type, self._aedt_version)
         elif design_type == "Icepak":
             self.design_solutions = IcepakDesignSolution(None, design_type, self._aedt_version)
         elif design_type == "Maxwell 2D":
             self.design_solutions = Maxwell2DDesignSolution(None, design_type, self._aedt_version)
         elif design_type == "RMxprtSolution" or design_type == "ModelCreation":
@@ -414,17 +415,18 @@
         >>> oDesktop.GetVersion()
         """
         version = self.odesktop.GetVersion()
         return get_version_env_variable(version)
 
     @property
     def _aedt_version(self):
-        v = self.odesktop.GetVersion()
-        if v:
-            return v[0:6]
+        if self.odesktop:
+            v = self.odesktop.GetVersion()
+            if v:
+                return v[0:6]
         return ""
 
     @property
     def design_name(self):
         """Design name.
 
         Returns
@@ -451,15 +453,14 @@
         name = self.odesign.GetName()
         if ";" in name:
             return name.split(";")[1]
         else:
             return name
 
     @design_name.setter
-    @pyaedt_function_handler()
     def design_name(self, new_name):
         if ";" in new_name:
             new_name = new_name.split(";")[1]
 
         self.odesign.RenameDesignInstance(self.design_name, new_name)
         timeout = 5.0
         timestep = 0.1
@@ -520,17 +521,17 @@
             Name of the project.
 
         References
         ----------
 
         >>> oProject.GetName
         """
-        if self._oproject:
+        if self.oproject:
             try:
-                return self._oproject.GetName()
+                return self.oproject.GetName()
             except:
                 return None
         else:
             return None
 
     @property
     def project_list(self):
@@ -558,15 +559,17 @@
             Path to the project.
 
         References
         ----------
 
         >>> oProject.GetPath
         """
-        return self.oproject.GetPath()
+        if self.oproject:
+            return self.oproject.GetPath()
+        return None
 
     @property
     def project_time_stamp(self):
         """Return Project time stamp."""
         if os.path.exists(self.project_file):
             settings._project_time_stamp = os.path.getmtime(self.project_file)
         else:
@@ -585,39 +588,42 @@
 
         Returns
         -------
         str
             Full absolute name and path for the project.
 
         """
-        return os.path.join(self.project_path, self.project_name + ".aedt")
+        if self.project_path:
+            return os.path.join(self.project_path, self.project_name + ".aedt")
 
     @property
     def lock_file(self):
         """Lock file.
 
         Returns
         -------
         str
             Full absolute name and path for the project's lock file.
 
         """
-        return os.path.join(self.project_path, self.project_name + ".aedt.lock")
+        if self.project_path:
+            return os.path.join(self.project_path, self.project_name + ".aedt.lock")
 
     @property
     def results_directory(self):
         """Results directory.
 
         Returns
         -------
         str
             Full absolute path for the ``aedtresults`` directory.
 
         """
-        return os.path.join(self.project_path, self.project_name + ".aedtresults")
+        if self.project_path:
+            return os.path.join(self.project_path, self.project_name + ".aedtresults")
 
     @property
     def solution_type(self):
         """Solution type.
 
         Returns
         -------
@@ -626,20 +632,22 @@
 
         References
         ----------
 
         >>> oDesign.GetSolutionType
         >>> oDesign.SetSolutionType
         """
-        return self.design_solutions.solution_type
+        if self.design_solutions:
+            return self.design_solutions.solution_type
+        return None
 
     @solution_type.setter
-    @pyaedt_function_handler()
     def solution_type(self, soltype):
-        self.design_solutions.solution_type = soltype
+        if self.design_solutions:
+            self.design_solutions.solution_type = soltype
 
     @property
     def valid_design(self):
         """Valid design.
 
         Returns
         -------
@@ -880,15 +888,14 @@
 
         >>> oProject.SetActiveDesign
         >>> oProject.InsertDesign
         """
         return self._odesign
 
     @odesign.setter
-    @pyaedt_function_handler()
     def odesign(self, des_name):
         if des_name:
             if self._assert_consistent_design_type(des_name) == des_name:
                 self._insert_design(self._design_type, design_name=des_name)
             self.design_solutions._odesign = self.odesign
             if self._temp_solution_type:
                 self.design_solutions.solution_type = self._temp_solution_type
@@ -920,15 +927,14 @@
         >>> oDesktop.GetActiveProject
         >>> oDesktop.SetActiveProject
         >>> oDesktop.NewProject
         """
         return self._oproject
 
     @oproject.setter
-    @pyaedt_function_handler()
     def oproject(self, proj_name=None):
         if not proj_name:
             self._oproject = self.odesktop.GetActiveProject()
             if self._oproject:
                 self.logger.info(
                     "No project is defined. Project {} exists and has been read.".format(self._oproject.GetName())
                 )
@@ -3052,15 +3058,15 @@
             if design_type == "HFSS" and self._aedt_version < "2021.2":
                 new_design = self._oproject.InsertDesign(design_type, unique_design_name, "DrivenModal", "")
             else:
                 new_design = self._oproject.InsertDesign(
                     design_type, unique_design_name, self.default_solution_type, ""
                 )
         self.logger.info("Added design '%s' of type %s.", unique_design_name, design_type)
-        name = _retry_ntimes(5, new_design.GetName)
+        name = _retry_ntimes(10, new_design.GetName)
         self._odesign = new_design
         return name
 
     @pyaedt_function_handler()
     def _generate_unique_design_name(self, design_name):
         """Generate an unique design name.
 
@@ -3570,30 +3576,39 @@
         float
             Evaluated value for the string expression.
 
         """
         # Set the value of an internal reserved design variable to the specified string
         if expression_string in self._variable_manager.variables:
             return self._variable_manager.variables[expression_string].value
-        else:
-            try:
-                self._variable_manager.set_variable(
-                    "pyaedt_evaluator",
-                    expression=expression_string,
-                    readonly=True,
-                    hidden=True,
-                    description="Internal_Evaluator",
-                )
-            except:
-                raise ("Invalid string expression {}".expression_string)
-
+        elif "pwl" in str(expression_string):
+            for ds in self.project_datasets:
+                if ds in expression_string:
+                    return expression_string
+            for ds in self.design_datasets:
+                if ds in expression_string:
+                    return expression_string
+        try:
+            variable_name = "pyaedt_evaluator"
+            if "$" in expression_string:
+                variable_name = "$pyaedt_evaluator"
+            self._variable_manager.set_variable(
+                variable_name,
+                expression=expression_string,
+                readonly=True,
+                hidden=True,
+                description="Internal_Evaluator",
+            )
+            eval_value = self._variable_manager.variables[variable_name].value
             # Extract the numeric value of the expression (in SI units!)
-            eval_value = self._variable_manager.variables["pyaedt_evaluator"].value
-            self._variable_manager.delete_variable("pyaedt_evaluator")
+            self._variable_manager.delete_variable(variable_name)
             return eval_value
+        except:
+            self.logger.warning("Invalid string expression {}".format(expression_string))
+            return expression_string
 
     @pyaedt_function_handler()
     def design_variation(self, variation_string=None):
         """Generate a string to specify a desired variation.
 
         This method converts an input string defining a desired solution variation into a valid
         string taking into account all existing design properties and project variables, including
```

### Comparing `pyaedt-0.6.76/pyaedt/application/JobManager.py` & `pyaedt-0.6.77/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/application/Variables.py` & `pyaedt-0.6.77/pyaedt/application/Variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from __future__ import absolute_import  # noreorder
 from __future__ import division
 
 import os
 import re
 import types
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import SI_UNITS
 from pyaedt.generic.constants import _resolve_unit_system
 from pyaedt.generic.constants import unit_system
 from pyaedt.generic.general_methods import is_array
 from pyaedt.generic.general_methods import is_number
```

### Comparing `pyaedt-0.6.76/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.77/pyaedt/application/aedt_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import sys
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 
 
 class AedtObjects(object):
     def __init__(self, project=None, design=None, is_inherithed=False):
         self._odesktop = sys.modules["__main__"].oDesktop
         if not is_inherithed:
```

### Comparing `pyaedt-0.6.76/pyaedt/application/design_solutions.py` & `pyaedt-0.6.77/pyaedt/application/design_solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import copy
 
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 solutions_defaults = {
     "Maxwell 2D": "Magnetostatic",
     "Maxwell 3D": "Magnetostatic",
     "Twin Builder": "TR",
     "Circuit Design": "NexximLNA",
@@ -524,15 +525,14 @@
             except:
                 self._solution_type = solutions_defaults[self._design_type]
         elif self._solution_type is None:
             self._solution_type = solutions_defaults[self._design_type]
         return self._solution_type
 
     @solution_type.setter
-    @pyaedt_function_handler()
     def solution_type(self, value):
         if value is None:
             if self._design_type in [
                 "Circuit Design",
                 "Twin Builder",
                 "HFSS 3D Layout Design",
                 "EMIT",
@@ -611,15 +611,14 @@
             except:
                 self._solution_type = solutions_defaults[self._design_type]
         elif self._solution_type is None:
             self._solution_type = solutions_defaults[self._design_type]
         return self._solution_type
 
     @solution_type.setter
-    @pyaedt_function_handler()
     def solution_type(self, value):
         if self._aedt_version < "2021.2":
             if not value:
                 self._solution_type = "DrivenModal"
                 self._odesign.SetSolutionType(self._solution_type)
             elif "Modal" in value:
                 self._solution_type = "DrivenModal"
@@ -672,15 +671,14 @@
         if self._aedt_version < "2021.2":
             return False
         if self.solution_type is not None:
             self._hybrid = "Hybrid" in self._odesign.GetSolutionType()
         return self._hybrid
 
     @hybrid.setter
-    @pyaedt_function_handler()
     def hybrid(self, value):
         if self._aedt_version < "2021.2":
             return
         if value and "Hybrid" not in self._solution_options[self.solution_type]["name"]:
             self._solution_options[self.solution_type]["name"] = self._solution_options[self.solution_type][
                 "name"
             ].replace("HFSS", "HFSS Hybrid")
@@ -697,15 +695,14 @@
         if self._aedt_version < "2021.2":
             return False
         if self._composite is None and self.solution_type is not None:
             self._composite = "Composite" in self._odesign.GetSolutionType()
         return self._composite
 
     @composite.setter
-    @pyaedt_function_handler()
     def composite(self, val):
         if self._aedt_version < "2021.2":
             return
         if val:
             self._solution_options[self.solution_type]["name"] = self._solution_options[self.solution_type][
                 "name"
             ].replace("Network", "Composite")
@@ -749,15 +746,14 @@
 
     @property
     def xy_plane(self):
         """Get/Set Maxwell 2d plane between `"XY"` and `"about Z"`."""
         return self._geometry_mode == "XY"
 
     @xy_plane.setter
-    @pyaedt_function_handler()
     def xy_plane(self, value=True):
         if value:
             self._geometry_mode = "XY"
         else:
             self._geometry_mode = "about Z"
         self._solution_options[self.solution_type]["options"] = self._geometry_mode
         self.solution_type = self.solution_type
@@ -769,15 +765,14 @@
             try:
                 self._solution_type = self._odesign.GetSolutionType()
             except:
                 self._solution_type = solutions_defaults[self._design_type]
         return self._solution_type
 
     @solution_type.setter
-    @pyaedt_function_handler()
     def solution_type(self, value):
         if value is None:
             if self._odesign and "GetSolutionType" in dir(self._odesign):
                 self._solution_type = self._odesign.GetSolutionType()
                 if "Modal" in self._solution_type:
                     self._solution_type = "Modal"
                 elif "Terminal" in self._solution_type:
@@ -815,15 +810,14 @@
         It can be any of`"TemperatureAndFlow"`, `"TemperatureOnly"`,`"FlowOnly"`.
         """
         if self._odesign:
             self._problem_type = self._odesign.GetProblemType()
         return self._problem_type
 
     @problem_type.setter
-    @pyaedt_function_handler()
     def problem_type(self, value="TemperatureAndFlow"):
         if value == "TemperatureAndFlow":
             self._problem_type = value
             self._solution_options[self.solution_type]["options"] = self._problem_type
             if self.solution_type == "SteadyState":
                 self._solution_options[self.solution_type]["default_setup"] = 11
             else:
@@ -853,15 +847,14 @@
             try:
                 self._solution_type = self._odesign.GetSolutionType()
             except:
                 self._solution_type = solutions_defaults[self._design_type]
         return self._solution_type
 
     @solution_type.setter
-    @pyaedt_function_handler()
     def solution_type(self, solution_type):
         if solution_type:
             if "SteadyState" in solution_type:
                 self._solution_type = "SteadyState"
             else:
                 self._solution_type = "Transient"
             if "TemperatureAndFlow" in solution_type:
@@ -892,27 +885,25 @@
     def solution_type(self):
         """Get/Set the Machine Type of the active Design."""
         if self._solution_type is None and "GetMachineType" in dir(self._odesign):
             self._solution_type = self._odesign.GetMachineType()
         return self._solution_type
 
     @solution_type.setter
-    @pyaedt_function_handler()
     def solution_type(self, solution_type):
         if solution_type:
             try:
                 self._odesign.SetDesignFlow(self._design_type, solution_type)
                 self._solution_type = solution_type
             except:
                 pass
 
     @property
     def design_type(self):
         """Get/Set the Machine Design Type."""
         return self._design_type
 
     @design_type.setter
-    @pyaedt_function_handler()
     def design_type(self, value):
         if value:
             self._design_type = value
             self.solution_type = self._solution_type
```

### Comparing `pyaedt-0.6.76/pyaedt/circuit.py` & `pyaedt-0.6.77/pyaedt/circuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1647,19 +1647,24 @@
             Path of the EDB file to copy.
 
         Returns
         -------
             ``Hfss3DLayout`` component instance.
         """
         hfss = Hfss3dLayout(edb_path)
-        hfss.edit_cosim_options(
-            simulate_missing_solution=True,
-            setup_override_name=hfss.setup_names[0],
-            sweep_override_name=hfss.existing_analysis_sweeps[0].split(":")[1].strip(" "),
-        )
+        try:
+            hfss.edit_cosim_options(
+                simulate_missing_solution=True,
+                setup_override_name=hfss.setup_names[0],
+                sweep_override_name=hfss.existing_analysis_sweeps[0].split(":")[1].strip(" "),
+            )
+        except:
+            self.logger.error(
+                "Failed to setup co-simulation settings, make sure the simulation setup is properly defined"
+            )
         active_project = hfss.odesktop.SetActiveProject(hfss.project_name)
         active_project.CopyDesign(hfss.design_name)
         active_project = self.odesktop.SetActiveProject(self.project_name)
         active_project.Paste()
         hfss_3d_layout_model = self.modeler.schematic.add_subcircuit_3dlayout(hfss.design_name)
         hfss.close_project(save_project=False)
         return hfss_3d_layout_model
```

### Comparing `pyaedt-0.6.76/pyaedt/common_rpc.py` & `pyaedt-0.6.77/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/desktop.py` & `pyaedt-0.6.77/pyaedt/desktop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """
 This module contains the ``Desktop`` class.
-
 This module is used to initialize AEDT and the message manager for managing AEDT.
-
 You can initialize this module before launching an app or
 have the app automatically initialize it to the latest installed AEDT version.
 """
 
 from __future__ import absolute_import  # noreorder
 
 import datetime
@@ -34,14 +32,15 @@
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
     import subprocess
 
 from pyaedt import __version__
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt import settings
 from pyaedt.generic.general_methods import _pythonver
 from pyaedt.generic.general_methods import active_sessions
 from pyaedt.generic.general_methods import com_active_sessions
 from pyaedt.generic.general_methods import grpc_active_sessions
 from pyaedt.generic.general_methods import inside_desktop
@@ -72,17 +71,21 @@
         command = [full_path, "-grpcsrv", str(port)]
         if non_graphical:
             command.append("-ng")
         my_env = os.environ.copy()
         for env, val in settings.aedt_environment_variables.items():
             my_env[env] = val
         if is_linux:  # pragma: no cover
-            subprocess.Popen(command, env=my_env, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
+            with subprocess.Popen(command, env=my_env, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL) as p:
+                p.wait()
         else:
-            subprocess.Popen(" ".join(command), env=my_env, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
+            with subprocess.Popen(
+                " ".join(command), env=my_env, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL
+            ) as p:
+                p.wait()
 
     _aedt_process_thread = threading.Thread(target=launch_desktop_on_port)
     _aedt_process_thread.daemon = True
     _aedt_process_thread.start()
     timeout = settings.desktop_launch_timeout
     k = 0
     while not _check_grpc_port(port):
@@ -122,15 +125,15 @@
             settings.lsf_aedt_command,
             "-grpcsrv",
             str(port),
         ]
     if non_graphical:
         command.append("-ng")
     print(command)
-    p = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
+    p = subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
     timeout = settings.lsf_timeout
     i = 0
     while i < timeout:
         err = p.stderr.readline().strip().decode("utf-8", "replace")
         m = re.search(r"<<Starting on (.+?)>>", err)
         if m:
             aedt_startup_timeout = 120
@@ -149,18 +152,20 @@
 def _check_grpc_port(port, machine_name=""):
     s = socket.socket()
     try:
         if not machine_name:
             machine_name = "127.0.0.1"
         s.connect((machine_name, port))
     except socket.error:
-        return False
+        success = False
     else:
+        success = True
+    finally:
         s.close()
-        return True
+    return success
 
 
 def _find_free_port():
     with socket.socket() as s:
         s.bind(("", 0))  # Bind to a free port provided by the host.
         return s.getsockname()[1]  # Return the port number assigned.
 
@@ -442,27 +447,27 @@
 
     Examples
     --------
     Launch AEDT 2021 R1 in non-graphical mode and initialize HFSS.
 
     >>> import pyaedt
     >>> desktop = pyaedt.Desktop("2021.2", non_graphical=True)
-    pyaedt INFO: pyaedt v...
-    pyaedt INFO: Python version ...
+    PyAEDT INFO: pyaedt v...
+    PyAEDT INFO: Python version ...
     >>> hfss = pyaedt.Hfss(designname="HFSSDesign1")
-    pyaedt INFO: Project...
-    pyaedt INFO: Added design 'HFSSDesign1' of type HFSS.
+    PyAEDT INFO: Project...
+    PyAEDT INFO: Added design 'HFSSDesign1' of type HFSS.
 
     Launch AEDT 2021 R1 in graphical mode and initialize HFSS.
 
     >>> desktop = Desktop("2021.2")
-    pyaedt INFO: pyaedt v...
-    pyaedt INFO: Python version ...
+    PyAEDT INFO: pyaedt v...
+    PyAEDT INFO: Python version ...
     >>> hfss = pyaedt.Hfss(designname="HFSSDesign1")
-    pyaedt INFO: No project is defined. Project...
+    PyAEDT INFO: No project is defined. Project...
     """
 
     def __init__(
         self,
         specified_version=None,
         non_graphical=False,
         new_desktop_session=True,
@@ -490,14 +495,18 @@
             self._main.isoutsideDesktop = False
         else:
             self._main.isoutsideDesktop = True
         self.release_on_exit = True
         self.logfile = None
 
         self._logger = pyaedt_logger
+        if settings.enable_screen_logs:
+            self._logger.enable_stdout_log()
+        else:
+            self._logger.disable_stdout_log()
         self._logger.info("using existing logger.")
 
         if "oDesktop" in dir():  # pragma: no cover
             self.release_on_exit = False
             self._main.oDesktop = oDesktop
             try:
                 settings.non_graphical = oDesktop.GetIsNonGraphical()
@@ -1304,16 +1313,16 @@
         bool
             ``True`` when successful, ``False`` when failed.
 
         Examples
         --------
         >>> import pyaedt
         >>> desktop = pyaedt.Desktop("2021.2")
-        pyaedt INFO: pyaedt v...
-        pyaedt INFO: Python version ...
+        PyAEDT INFO: pyaedt v...
+        PyAEDT INFO: Python version ...
         >>> desktop.release_desktop(close_projects=False, close_on_exit=False) # doctest: +SKIP
 
         """
         result = release_desktop(close_projects, close_on_exit)
         self.odesktop = None
         return result
 
@@ -1325,44 +1334,44 @@
         bool
             ``True`` when successful, ``False`` when failed.
 
         Examples
         --------
         >>> import pyaedt
         >>> desktop = pyaedt.Desktop("2021.2")
-        pyaedt INFO: pyaedt v...
-        pyaedt INFO: Python version ...
+        PyAEDT INFO: pyaedt v...
+        PyAEDT INFO: Python version ...
         >>> desktop.close_desktop() # doctest: +SKIP
 
         """
         return self.release_desktop(close_projects=True, close_on_exit=True)
 
     def enable_autosave(self):
         """Enable the autosave option.
 
         Examples
         --------
         >>> import pyaedt
         >>> desktop = pyaedt.Desktop("2021.2")
-        pyaedt INFO: pyaedt v...
-        pyaedt INFO: Python version ...
+        PyAEDT INFO: pyaedt v...
+        PyAEDT INFO: Python version ...
         >>> desktop.enable_autosave()
 
         """
         self._main.oDesktop.EnableAutoSave(True)
 
     def disable_autosave(self):
         """Disable the autosave option.
 
         Examples
         --------
         >>> import pyaedt
         >>> desktop = pyaedt.Desktop("2021.2")
-        pyaedt INFO: pyaedt v...
-        pyaedt INFO: Python version ...
+        PyAEDT INFO: pyaedt v...
+        PyAEDT INFO: Python version ...
         >>> desktop.disable_autosave()
 
         """
         self._main.oDesktop.EnableAutoSave(False)
 
     def change_license_type(self, license_type="Pool"):
         """Change the license type.
@@ -1674,7 +1683,76 @@
                 elif "WaitForLicense" in line:
                     lin = "\\	\\	WaitForLicense={}\\\n".format(str(wait_for_license).lower())
                     f1.write(lin)
                 else:
                     f1.write(line)
         f1.close()
         return self.odesktop.SubmitJob(os.path.join(project_path, "Job_settings.areg"), project_file)
+
+    @property
+    def are_there_simulations_running(self):
+        """Check if there are simulation running.
+
+        .. note::
+           It works only for AEDT >= ``"2023.2"``.
+
+        Returns
+        -------
+        float
+
+        """
+        if self.aedt_version_id > "2023.1":
+            return self.odesktop.AreThereSimulationsRunning()
+        else:
+            self.logger.error("It works only for AEDT >= `2023.2`.")
+        return False
+
+    @pyaedt_function_handler()
+    def get_monitor_data(self):
+        """Check and get monitor data of an existing analysis.
+
+        .. note::
+           It works only for AEDT >= ``"2023.2"``.
+
+        Returns
+        -------
+        dict
+
+        """
+        counts = {"profile": 0, "convergence": 0, "sweptvar": 0, "progress": 0, "variations": 0, "displaytype": 0}
+        if self.are_there_simulations_running:
+            reqstr = " ".join(["%s %d 0" % (t, counts[t]) for t in counts])
+            data = self.odesktop.GetMonitorData(reqstr)
+            all_lines = (line.strip() for line in data.split("\n"))
+            for line in all_lines:
+                if line.startswith("$begin"):
+                    btype = line.split()[1].strip("'")
+                    if btype == "MonitoringProfileMsg":
+                        counts["profile"] += 1
+                    elif btype == "MonConvData":
+                        counts["convergence"] += 1
+                    elif btype == "MonGenericVariations":
+                        pass
+                    elif btype == "MapMonGraphicalProgMsg":
+                        pass
+                    elif btype == "MonitoringSweptVariableMsg":
+                        counts["sweptvar"] += 1
+            return counts
+        return counts
+
+    @pyaedt_function_handler()
+    def stop_simulations(self, clean_stop=True):
+        """Check if there are simulation running and stops them.
+
+        .. note::
+           It works only for AEDT >= ``"2023.2"``.
+
+        Returns
+        -------
+        str
+
+        """
+        if self.aedt_version_id > "2023.1":
+            return self.odesktop.StopSimulations(clean_stop)
+        else:
+            self.logger.error("It works only for AEDT >= `2023.2`.")
+        return False
```

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.77/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/downloads.py` & `pyaedt-0.6.77/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb.py` & `pyaedt-0.6.77/pyaedt/edb.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from pyaedt.generic.general_methods import env_path_student
 from pyaedt.generic.general_methods import env_value
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import is_windows
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.process import SiwaveSolve
 from pyaedt.misc.misc import list_installed_ansysem
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
@@ -153,14 +154,18 @@
         self.standalone = True
         if edb_initialized:
             self.oproject = oproject
             self._main = sys.modules["__main__"]
             self._global_logger = pyaedt_logger
             self._logger = pyaedt_logger
             self.student_version = student_version
+            if settings.enable_screen_logs:
+                self.logger.enable_stdout_log()
+            else:
+                self.logger.disable_stdout_log()
             self.logger.info("Logger is initialized in EDB.")
             self.logger.info("pyaedt v%s", __version__)
             self.logger.info("Python version %s", sys.version)
             if not edbversion:
                 try:
                     edbversion = "20{}.{}".format(list_installed_ansysem()[0][-3:-1], list_installed_ansysem()[0][-1:])
                     self._logger.info("Edb version " + edbversion)
@@ -3370,38 +3375,51 @@
         Parameters
         ----------
         working_directory : str
             Directory path where all EDB project are copied, if empty will use the current EDB project.
 
         Returns
         -------
-           dict[str](EDB PolygonData)
-           Return a dictionary with edb path as key and EDB polygon Data defining the region.
+           dict[str](int, EDB PolygonData)
+           Return a dictionary with edb path as key and tuple Zone Id as first item and EDB polygon Data defining
+           the region as second item.
 
         """
         if working_directory:
             if not os.path.isdir(working_directory):
                 os.mkdir(working_directory)
             else:
                 shutil.rmtree(working_directory)
                 os.mkdir(working_directory)
         else:
             working_directory = os.path.dirname(self.edbpath)
         zone_primitives = list(self.active_layout.GetZonePrimitives())
+        zone_ids = list(self.stackup._layer_collection.GetZoneIds())
         edb_zones = {}
         if not self.setups:
             self.siwave.add_siwave_syz_analysis()
             self.save_edb()
-        for zone in zone_primitives:
-            edb_zone_path = os.path.join(
-                working_directory, "{}_{}".format(zone.GetId(), os.path.basename(self.edbpath))
-            )
-            shutil.copytree(self.edbpath, edb_zone_path)
-            poly_data = zone.GetPolygonData()
-            edb_zones[edb_zone_path] = poly_data
+        if not len(zone_primitives) == len(zone_ids):
+            self.logger.info("Number of zone primitives not equal to zone number, zone information will be lost")
+            for zone_primitive in zone_primitives:
+                edb_zone_path = os.path.join(
+                    working_directory, "{}_{}".format(zone_primitive.GetId(), os.path.basename(self.edbpath))
+                )
+                shutil.copytree(self.edbpath, edb_zone_path)
+                poly_data = zone_primitive.GetPolygonData()
+                edb_zones[edb_zone_path] = (-1, poly_data)
+        else:
+            for zone_index in range(len(zone_primitives)):
+                edb_zone_path = os.path.join(
+                    working_directory,
+                    "{}_{}".format(zone_primitives[zone_index].GetId(), os.path.basename(self.edbpath)),
+                )
+                shutil.copytree(self.edbpath, edb_zone_path)
+                poly_data = zone_primitives[zone_index].GetPolygonData()
+                edb_zones[edb_zone_path] = (zone_ids[0], poly_data)
         return edb_zones
 
     @pyaedt_function_handler()
     def cutout_multizone_layout(self, zone_dict, common_reference_net):
         """Create multizone project cutout.
 
         Parameters
@@ -3421,23 +3439,30 @@
         first dictionary defined_ports with edb name as key and existing port name list as value. Those ports are the
         ones defined before processing the multizone clipping.
         second is the list of connected port.
 
         """
         terminals = {}
         defined_ports = {}
-        for edb_path, zone_polygon in zone_dict.items():
+        for edb_path, zone_info in zone_dict.items():
             edb = Edb(edbversion=self.edbversion, edbpath=edb_path)
+            edb.cutout(use_pyaedt_cutout=True, custom_extent=zone_info[1], open_cutout_at_end=True)
+            if not zone_info == -1:
+                layers_to_remove = [
+                    lay.name for lay in list(edb.stackup.layers.values()) if not lay._edb_layer.IsInZone(zone_info[0])
+                ]
+                for layer in layers_to_remove:
+                    edb.stackup.remove_layer(layer)
             edb.stackup.stackup_mode = "Laminate"
-            signal_nets = list(self.nets.signal.keys())
-            edb.cutout(use_pyaedt_cutout=True, custom_extent=zone_polygon, open_cutout_at_end=True)
+            edb.cutout(use_pyaedt_cutout=True, custom_extent=zone_info[1], open_cutout_at_end=True)
             edb.active_cell.SetName(os.path.splitext(os.path.basename(edb_path))[0])
+            signal_nets = list(self.nets.signal.keys())
             defined_ports[os.path.splitext(os.path.basename(edb_path))[0]] = list(edb.excitations.keys())
             edb_terminals_info = edb.hfss.create_vertical_circuit_port_on_clipped_traces(
-                nets=signal_nets, reference_net=common_reference_net, user_defined_extent=zone_polygon
+                nets=signal_nets, reference_net=common_reference_net, user_defined_extent=zone_info[1]
             )
             if edb_terminals_info:
                 terminals[os.path.splitext(os.path.basename(edb_path))[0]] = edb_terminals_info
             edb.save_edb()
             edb.close_edb()
         project_connexions = self._get_connected_ports_from_multizone_cutout(terminals)
         return defined_ports, project_connexions
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/components.py` & `pyaedt-0.6.77/pyaedt/edb_core/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pyaedt.edb_core.edb_data.sources import SourceType
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.edb_core.padstack import EdbPadstacks
 from pyaedt.generic.clr_module import String
 from pyaedt.generic.clr_module import _clr
 from pyaedt.generic.general_methods import get_filename_without_extension
 from pyaedt.generic.general_methods import is_ironpython
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 def resistor_value_parser(RValue):
     """Convert a resistor value.
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/components_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
         import numpy as np
     except ImportError:
         warnings.warn(
             "The NumPy module is required to run some functionalities of EDB.\n"
             "Install with \n\npip install numpy\n\nRequires CPython."
         )
 from pyaedt.generic.general_methods import get_filename_without_extension
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EDBComponentDef(object):
     """Manages EDB functionalities for component definitions.
 
     Parameters
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/control_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from pyaedt import pyaedt_logger
 from pyaedt.generic.general_methods import ET
 from pyaedt.generic.general_methods import env_path
 from pyaedt.generic.general_methods import env_value
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.misc import list_installed_ansysem
 from pyaedt.misc.aedtlib_personalib_install import write_pretty_xml
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/variables.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,91 @@
-class EdbValue:
-    """Class defining Edb Value properties."""
+class Variable:
+    """Manages EDB methods for variable accessible from `Edb.Utility.VariableServer` property."""
 
-    def __init__(self, edb_obj):
-        self._edb_obj = edb_obj
+    def __init__(self, pedb, name):
+        self._pedb = pedb
+        self._name = name
 
     @property
-    def value(self):
-        """Variable Value Object.
+    def _is_design_varible(self):
+        """Determines whether this variable is a design variable."""
+        if self.name.startswith("$"):
+            return False
+        else:
+            return True
+
+    @property
+    def _var_server(self):
+        if self._is_design_varible:
+            return self._pedb.active_cell.GetVariableServer()
+        else:
+            return self._pedb.db.GetVariableServer()
+
+    @property
+    def name(self):
+        """Get the name of this variable."""
+        return self._name
+
+    @property
+    def value_string(self):
+        """Get/Set the value of this variable.
 
         Returns
         -------
-        Edb Object
+        str
+
         """
-        return self._edb_obj
+        return self._pedb.get_variable(self.name).tostring
 
     @property
-    def name(self):
-        """Variable name.
+    def value_object(self):
+        """Get/Set the value of this variable.
 
         Returns
         -------
-        str
+        :class:`pyaedt.edb_core.edb_data.edbvalue.EdbValue`
         """
-        return self._edb_obj.GetName()
+        return self._pedb.get_variable(self.name)
 
     @property
-    def tofloat(self):
-        """Returns the float number of the variable.
+    def value(self):
+        """Get the value of this variable.
 
         Returns
         -------
         float
         """
-        return self._edb_obj.ToDouble()
+        return self._pedb.get_variable(self.name).tofloat
+
+    @value.setter
+    def value(self, value):
+        self._pedb.change_design_variable_value(self.name, value)
+
+    @property
+    def description(self):
+        """Get the description of this variable."""
+        return self._var_server.GetVariableDescription(self.name)
+
+    @description.setter
+    def description(self, value):
+        self._var_server.SetVariableDescription(self.name, value)
 
     @property
-    def tostring(self):
-        """Returns the string of the variable.
+    def is_parameter(self):
+        """Determine whether this variable is a parameter."""
+        return self._var_server.IsVariableParameter(self.name)
+
+    def delete(self):
+        """Delete this variable.
 
         Returns
         -------
-        str
-        """
-        return self._edb_obj.ToString()
+        bool
+            ``True`` when successful, ``False`` when failed.
 
-    def __str__(self):
-        """Another way to return the string for the value."""
-        return self.tostring
-
-    def __repr__(self):
-        """Another way to return the string for the value."""
-        return "<Instance of pyaedt.edb_core.edb_data.EdbValue = " + self.tostring + ">"
+        Examples
+        --------
+        >>> from pyaedt import Edb
+        >>> edb = Edb()
+        >>> edb.design_variables["new_variable"].delete()
+        """
+        return self._var_server.DeleteVariable(self.name)
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pyaedt.edb_core.edb_data.edbvalue import EdbValue
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.edb_core.general import convert_pytuple_to_nettuple
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class HfssExtentInfo:
     """Manages EDB functionalities for HFSS extent information.
 
     Parameters
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import Tuple
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EdbFrequencySweep(object):
     """Manages EDB methods for frequency sweep."""
 
     def __init__(self, sim_setup, frequency_sweep=None, name=None, edb_sweep_data=None):
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import absolute_import
 
 import re
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 
 
 class LayerEdbClass(object):
     """Manages Edb Layers. Replaces EDBLayer."""
 
     def __init__(self, pclass, name):
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EDBNetsData(object):
     """Manages EDB functionalities for a primitives.
     It Inherits EDB Object properties.
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pyaedt import is_ironpython
 from pyaedt.edb_core.edb_data.edbvalue import EdbValue
 from pyaedt.edb_core.general import PadGeometryTpe
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import String
 from pyaedt.generic.clr_module import _clr
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EDBPadProperties(object):
     """Manages EDB functionalities for pad properties.
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 
 from pyaedt.edb_core.general import convert_py_list_to_net_list
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EDBPrimitives(object):
     """Manages EDB functionalities for a primitives.
     It Inherits EDB Object properties.
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pyaedt.generic.clr_module import Dictionary
 from pyaedt.generic.constants import BasisOrder
 from pyaedt.generic.constants import CutoutSubdesignType
 from pyaedt.generic.constants import RadiationBoxType
 from pyaedt.generic.constants import SolverType
 from pyaedt.generic.constants import SweepType
 from pyaedt.generic.constants import validate_enum_class_value
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class SimulationConfigurationBatch(object):
     """Contains all Cutout and Batch analysis settings.
     The class is part of `SimulationConfiguration` class as a property.
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pyaedt.edb_core.edb_data.hfss_simulation_setup_data import EdbFrequencySweep
 from pyaedt.edb_core.general import convert_netdict_to_pydict
 from pyaedt.edb_core.general import convert_pydict_to_netdict
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_linux
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class SiwaveAdvancedSettings(object):
     def __init__(self, parent):
         self._parent = parent
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.edb_core.edb_data.nets_data import EDBNetsData
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.generic.constants import NodeType
 from pyaedt.generic.constants import SourceType
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.77/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/general.py` & `pyaedt-0.6.77/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.77/pyaedt/edb_core/hfss.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pyaedt.edb_core.edb_data.sources import ExcitationDifferential
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.edb_core.general import convert_pytuple_to_nettuple
 from pyaedt.generic.constants import RadiationBoxType
 from pyaedt.generic.constants import SweepType
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EdbHfss(object):
     """Manages EDB method to configure Hfss setup accessible from `Edb.hfss` property.
 
@@ -1090,16 +1091,36 @@
                                 )
                                 ref_prim = [
                                     prim
                                     for prim in reference_net.primitives
                                     if prim.polygon_data.PointInPolygon(mid_pt_data)
                                 ]
                                 if not ref_prim:
-                                    self._logger.warning("No reference primitive found in port vicinity")
-                                else:
+                                    self._logger.warning("no reference primitive found, trying to extend scanning area")
+                                    scanning_zone = [
+                                        (mid_point[0] - mid_point[0] * 1e-3, mid_point[1] - mid_point[1] * 1e-3),
+                                        (mid_point[0] - mid_point[0] * 1e-3, mid_point[1] + mid_point[1] * 1e-3),
+                                        (mid_point[0] + mid_point[0] * 1e-3, mid_point[1] + mid_point[1] * 1e-3),
+                                        (mid_point[0] + mid_point[0] * 1e-3, mid_point[1] - mid_point[1] * 1e-3),
+                                    ]
+                                    for new_point in scanning_zone:
+                                        mid_pt_data = self._edb.Geometry.PointData(
+                                            self._edb.Utility.Value(new_point[0]), self._edb.Utility.Value(new_point[1])
+                                        )
+                                        ref_prim = [
+                                            prim
+                                            for prim in reference_net.primitives
+                                            if prim.polygon_data.PointInPolygon(mid_pt_data)
+                                        ]
+                                        if ref_prim:
+                                            self._logger.info("Reference primitive found")
+                                            break
+                                    if not ref_prim:
+                                        self._logger.error("Failed to collect valid reference primitives for terminal")
+                                if ref_prim:
                                     reference_layer = ref_prim[0].layer
                                     if term.SetReferenceLayer(reference_layer):  # pragma no cover
                                         self._logger.info("Port {} created".format(port_name))
             return terminal_info
         return False
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 
 from pyaedt.edb_core.ipc2581.ecad.cad_data.feature import Feature
 from pyaedt.edb_core.ipc2581.ecad.cad_data.feature import FeatureType
 from pyaedt.generic.general_methods import ET
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class LayerFeature(object):
     """Class describing IPC2581 layer feature."""
 
     def __init__(self, ipc):
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pyaedt.edb_core.ipc2581.content.entry_line import EntryLine
 from pyaedt.edb_core.ipc2581.ecad.cad_data.assembly_drawing import AssemblyDrawing
 from pyaedt.edb_core.ipc2581.ecad.cad_data.outline import Outline
 from pyaedt.edb_core.ipc2581.ecad.cad_data.pin import Pin
 from pyaedt.edb_core.ipc2581.ecad.cad_data.polygon import PolyStep
 from pyaedt.generic.general_methods import ET
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Package(object):
     """Class describing an IPC2581 package definition."""
 
     def __init__(self, ipc):
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pyaedt.edb_core.ipc2581.ecad.cad_data.layer_feature import LayerFeature
 from pyaedt.edb_core.ipc2581.ecad.cad_data.logical_net import LogicalNet
 from pyaedt.edb_core.ipc2581.ecad.cad_data.package import Package
 from pyaedt.edb_core.ipc2581.ecad.cad_data.padstack_def import PadstackDef
 from pyaedt.edb_core.ipc2581.ecad.cad_data.phy_net import PhyNet
 from pyaedt.edb_core.ipc2581.ecad.cad_data.profile import Profile
 from pyaedt.generic.general_methods import ET
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Step(object):
     def __init__(self, caddata, edb, units, ipc):
         self.design_name = caddata.design_name
         self._pedb = edb
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/layout.py` & `pyaedt-0.6.77/pyaedt/edb_core/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import math
 import warnings
 
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.edb_core.edb_data.utilities import EDBStatistics
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import Tuple
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EdbLayout(object):
     """Manages EDB methods for primitives management accessible from `Edb.modeler` property.
 
     Examples
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/materials.py` & `pyaedt-0.6.77/pyaedt/edb_core/materials.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import difflib
 import logging
 import warnings
 
 from pyaedt import is_ironpython
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import _clr
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 logger = logging.getLogger(__name__)
 
 
 class Material(object):
     """Manages EDB methods for material property management."""
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/nets.py` & `pyaedt-0.6.77/pyaedt/edb_core/nets.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pyaedt.edb_core.edb_data.nets_data import EDBNetsData
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.constants import CSS4_COLORS
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EdbNets(object):
     """Manages EDB methods for nets management accessible from `Edb.nets` property.
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.77/pyaedt/edb_core/padstack.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import warnings
 
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstack
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import Array
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EdbPadstacks(object):
     """Manages EDB methods for nets management accessible from `Edb.padstacks` property.
 
     Examples
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.77/pyaedt/edb_core/siwave.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from pyaedt.edb_core.edb_data.sources import ResistorSource
 from pyaedt.edb_core.edb_data.sources import VoltageSource
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.constants import SolverType
 from pyaedt.generic.constants import SweepType
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EdbSiwave(object):
     """Manages EDB methods related to Siwave Setup accessible from `Edb.siwave` property.
```

### Comparing `pyaedt-0.6.76/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.77/pyaedt/edb_core/stackup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import warnings
 
 from pyaedt import generate_unique_name
 from pyaedt.edb_core.edb_data.layer_data import LayerEdbClass
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.general_methods import ET
 from pyaedt.generic.general_methods import is_ironpython
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.misc.aedtlib_personalib_install import write_pretty_xml
 
 pd = None
 np = None
 if not is_ironpython:
     try:
```

### Comparing `pyaedt-0.6.76/pyaedt/emit.py` & `pyaedt-0.6.77/pyaedt/emit.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from pyaedt import emit_core
 from pyaedt import generate_unique_project_name
 from pyaedt.application.Design import Design
 from pyaedt.emit_core import EmitConstants
 from pyaedt.emit_core.Couplings import CouplingsEmit
 from pyaedt.emit_core.results.results import Results
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.schematic import ModelerEmit
 
 
 class Emit(Design, object):
     """Provides the Emit application interface.
 
@@ -49,14 +50,15 @@
         Whether to release AEDT on exit. The default is ``False``.
     student_version : bool, optional
         Whether to start the AEDT student version. The default is ``False``.
     port : int, optional
         Port number on which to start the oDesktop communication on an already existing server.
         This parameter is ignored when creating a server. This parameter works only in 2022 R2 or later.
         The remote server must be up and running with the command `"ansysedt.exe -grpcsrv portnum"`.
+        The default is ``0``.
     machine : str, optional
         Machine name that the Desktop session is to connect to. This
         parameter works only in 2022 R2 and later. The remote server must be
         up and running with the command `"ansysedt.exe -grpcsrv portnum"`.
         If the machine is `"localhost"`, the server starts if it is not present.
     aedt_process_id : int, optional
         Process ID for the instance of AEDT to point PyAEDT at. The default is
```

### Comparing `pyaedt-0.6.76/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.77/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.77/pyaedt/emit_core/EmitConstants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.77/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.77/pyaedt/emit_core/results/revision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import warnings
 
 import pyaedt.emit_core.EmitConstants as emitConsts
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Revision:
     """
     Provides the ``Revision`` object.
```

### Comparing `pyaedt-0.6.76/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.77/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.77/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/clr_module.py` & `pyaedt-0.6.77/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/configurations.py` & `pyaedt-0.6.77/pyaedt/generic/configurations.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pyaedt import generate_unique_folder_name
 from pyaedt import get_pyaedt_app
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.DataHandlers import _arg2dict
 from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 from pyaedt.generic.general_methods import _create_json_file
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import CoordinateSystem
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import BoundaryProps
 from pyaedt.modules.Boundary import NativeComponentObject
```

### Comparing `pyaedt-0.6.76/pyaedt/generic/constants.py` & `pyaedt-0.6.77/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/design_types.py` & `pyaedt-0.6.77/pyaedt/generic/design_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,27 +600,27 @@
 
     Examples
     --------
     Launch AEDT 2021 R1 in non-graphical mode and initialize HFSS.
 
     >>> import pyaedt
     >>> desktop = pyaedt.launch_desktop("2022.2", non_graphical=True)
-    pyaedt INFO: pyaedt v...
-    pyaedt INFO: Python version ...
+    PyAEDT INFO: pyaedt v...
+    PyAEDT INFO: Python version ...
     >>> hfss = pyaedt.Hfss(designname="HFSSDesign1")
-    pyaedt INFO: Project...
-    pyaedt INFO: Added design 'HFSSDesign1' of type HFSS.
+    PyAEDT INFO: Project...
+    PyAEDT INFO: Added design 'HFSSDesign1' of type HFSS.
 
     Launch AEDT 2021 R1 in graphical mode and initialize HFSS.
 
     >>> desktop = Desktop("2021.2")
-    pyaedt INFO: pyaedt v...
-    pyaedt INFO: Python version ...
+    PyAEDT INFO: pyaedt v...
+    PyAEDT INFO: Python version ...
     >>> hfss = pyaedt.Hfss(designname="HFSSDesign1")
-    pyaedt INFO: No project is defined. Project...
+    PyAEDT INFO: No project is defined. Project...
     """
     d = Desktop(
         specified_version=specified_version,
         non_graphical=non_graphical,
         new_desktop_session=new_desktop_session,
         close_on_exit=close_on_exit,
         student_version=student_version,
```

### Comparing `pyaedt-0.6.76/pyaedt/generic/filesystem.py` & `pyaedt-0.6.77/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/general_methods.py` & `pyaedt-0.6.77/pyaedt/generic/general_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,44 +85,48 @@
     message_to_print = ""
     try:
         messages = list(sys.modules["__main__"].oDesktop.GetMessages("", "", 2))
     except AttributeError:
         messages = []
     except TypeError:
         messages = []
-    if messages:
+    if messages and "error" in messages[-1].lower():
         message_to_print = messages[-1]
-    for el in tblist:
-        if func.__name__ in el:
-            _write_mes("Error in : " + el)
-    _write_mes("{} - {} -  {}.".format(ex_info[1], func.__name__, message.upper()))
+    # _write_mes("{} - {} -  {}.".format(ex_info[1], func.__name__, message.upper()))
 
     if message_to_print:
-        _write_mes(message_to_print)
-    _write_mes("Arguments with values: ")
+        _write_mes("API Message - " + message_to_print)
+    for el in tblist:
+        if func.__name__ in el:
+            _write_mes("{}, {}".format(el, message.upper()))
     args_name = []
     try:
         if int(sys.version[0]) > 2:
             args_name = list(OrderedDict.fromkeys(inspect.getfullargspec(func)[0] + list(kwargs.keys())))
             args_dict = OrderedDict(list(itertools.zip_longest(args_name, args)) + list(kwargs.items()))
         else:
             args_name = list(OrderedDict.fromkeys(inspect.getargspec(func)[0] + list(kwargs.keys())))
             args_dict = OrderedDict(list(itertools.izip(args_name, args)) + list(kwargs.iteritems()))
+        first_time_log = True
 
         for el in args_dict:
-            if el != "self":
+            if el != "self" and args_dict[el]:
+                if first_time_log:
+                    _write_mes("Method arguments: ")
+                    first_time_log = False
                 _write_mes("    {} = {} ".format(el, args_dict[el]))
     except:
         pass
     args = [func.__name__] + [i for i in args_name if i not in ["self"]]
-    _write_mes(
-        "Check Online documentation on: https://aedt.docs.pyansys.com/version/stable/search.html?q={}".format(
-            "+".join(args)
+    if not func.__name__.startswith("_"):
+        _write_mes(
+            "Check Online documentation on: https://aedt.docs.pyansys.com/version/stable/search.html?q={}".format(
+                "+".join(args)
+            )
         )
-    )
 
 
 def normalize_path(path_in, sep=None):
     """Normalize path separators.
 
     Parameters
     ----------
@@ -652,15 +656,15 @@
     while retry < n:
         try:
             ret_val = function(*args, **kwargs)
             if not ret_val and type(ret_val) is not float and type(ret_val) is not int:
                 ret_val = True
         except:
             retry += 1
-            time.sleep(0.1)
+            time.sleep(0.5)
         else:
             break
     if retry == n:
         if "__name__" in dir(function):
             raise AttributeError("Error in Executing Method {}.".format(function.__name__))
         else:
             raise AttributeError("Error in Executing Method.")
@@ -1710,14 +1714,54 @@
 
     def developer_forum(self):
         """Open the Discussions page on the Ansys Developer site."""
         url = "https://developer.ansys.com/"
         self._launch_ur(url)
 
 
+class Property(property):
+    @pyaedt_function_handler()
+    def __get__(self, obj, *args, **kwargs):
+        """Get value."""
+        # if obj is None:
+        #     return self
+        if self.fget is None:
+            raise AttributeError("unreadable attribute")
+        return self.fget(obj)
+
+    @pyaedt_function_handler()
+    def __set__(self, obj, value):
+        """Set value."""
+        if self.fset is None:
+            raise AttributeError("can't set attribute")
+        self.fset(obj, value)
+
+    @pyaedt_function_handler()
+    def __delete__(self, obj):
+        """Delete value."""
+        if self.fdel is None:
+            raise AttributeError("can't delete attribute")
+        self.fdel(obj)
+
+    @pyaedt_function_handler()
+    def getter(self, fget):
+        """Property getter."""
+        return self.__class__.__base__(fget, self.fset, self.fdel, self.__doc__)
+
+    @pyaedt_function_handler()
+    def setter(self, fset):
+        """Property setter."""
+        return self.__class__.__base__(self.fget, fset, self.fdel, self.__doc__)
+
+    @pyaedt_function_handler()
+    def deleter(self, fdel):
+        """Property deleter."""
+        return self.__class__.__base__(self.fget, self.fset, fdel, self.__doc__)
+
+
 class Settings(object):
     """Manages all PyAEDT environment variables and global settings."""
 
     def __init__(self):
         self._enable_logger = True
         self._enable_desktop_logs = True
         self._enable_screen_logs = True
@@ -2188,9 +2232,10 @@
         return self._enable_debug_logger
 
     @enable_debug_logger.setter
     def enable_debug_logger(self, val):
         self._enable_debug_logger = val
 
 
+property = Property
 settings = Settings()
 online_help = Help()
```

### Comparing `pyaedt-0.6.76/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.77/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.77/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/pdf.py` & `pyaedt-0.6.77/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/plot.py` & `pyaedt-0.6.77/pyaedt/generic/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import datetime
 import math
 import os
 import tempfile
 import time
 import warnings
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import CSS4_COLORS
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import open_file
 
 if not is_ironpython:
```

### Comparing `pyaedt-0.6.76/pyaedt/generic/process.py` & `pyaedt-0.6.77/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.77/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.77/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/generic/toolkit.py` & `pyaedt-0.6.77/pyaedt/generic/toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 
 from pyaedt import is_ironpython
 from pyaedt import is_linux
 from pyaedt import is_windows
 from pyaedt.desktop import Desktop
 import pyaedt.edb_core.edb_data.simulation_configuration
 from pyaedt.generic.clr_module import _clr
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
     import subprocess
```

### Comparing `pyaedt-0.6.76/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.77/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/hfss.py` & `pyaedt-0.6.77/pyaedt/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.generic.constants import INFINITE_SPHERE_TYPE
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import parse_excitation_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import FarFieldSetup
 from pyaedt.modules.Boundary import NativeComponentObject
 from pyaedt.modules.Boundary import NearFieldSetup
@@ -87,60 +88,60 @@
     Examples
     --------
     Create an instance of HFSS and connect to an existing HFSS
     design or create a new HFSS design if one does not exist.
 
     >>> from pyaedt import Hfss
     >>> hfss = Hfss()
-    pyaedt INFO: No project is defined...
-    pyaedt INFO: Active design is set to...
+    PyAEDT INFO: No project is defined...
+    PyAEDT INFO: Active design is set to...
 
 
     Create an instance of HFSS and link to a project named
     ``HfssProject``. If this project does not exist, create one with
     this name.
 
     >>> hfss = Hfss("HfssProject")
-    pyaedt INFO: Project HfssProject has been created.
-    pyaedt INFO: No design is present. Inserting a new design.
-    pyaedt INFO: Added design ...
+    PyAEDT INFO: Project HfssProject has been created.
+    PyAEDT INFO: No design is present. Inserting a new design.
+    PyAEDT INFO: Added design ...
 
 
     Create an instance of HFSS and link to a design named
     ``HfssDesign1`` in a project named ``HfssProject``.
 
     >>> hfss = Hfss("HfssProject","HfssDesign1")
-    pyaedt INFO: Added design 'HfssDesign1' of type HFSS.
+    PyAEDT INFO: Added design 'HfssDesign1' of type HFSS.
 
 
     Create an instance of HFSS and open the specified project,
     which is named ``"myfile.aedt"``.
 
     >>> hfss = Hfss("myfile.aedt")
-    pyaedt INFO: Project myfile has been created.
-    pyaedt INFO: No design is present. Inserting a new design.
-    pyaedt INFO: Added design...
+    PyAEDT INFO: Project myfile has been created.
+    PyAEDT INFO: No design is present. Inserting a new design.
+    PyAEDT INFO: Added design...
 
 
     Create an instance of HFSS using the 2021 R1 release and open
     the specified project, which is named ``"myfile2.aedt"``.
 
     >>> hfss = Hfss(specified_version="2021.2", projectname="myfile2.aedt")
-    pyaedt INFO: Project myfile2 has been created.
-    pyaedt INFO: No design is present. Inserting a new design.
-    pyaedt INFO: Added design...
+    PyAEDT INFO: Project myfile2 has been created.
+    PyAEDT INFO: No design is present. Inserting a new design.
+    PyAEDT INFO: Added design...
 
 
     Create an instance of HFSS using the 2021 R2 student version and open
     the specified project, which is named ``"myfile3.aedt"``.
 
     >>> hfss = Hfss(specified_version="2021.2", projectname="myfile3.aedt", student_version=True)
-    pyaedt INFO: Project myfile3 has been created.
-    pyaedt INFO: No design is present. Inserting a new design.
-    pyaedt INFO: Added design...
+    PyAEDT INFO: Project myfile3 has been created.
+    PyAEDT INFO: No design is present. Inserting a new design.
+    PyAEDT INFO: Added design...
 
     """
 
     # def __repr__(self):
     #     try:
     #         return "HFSS {} {}. ProjectName:{} DesignName:{} ".format(
     #             self._aedt_version, self.solution_type, self.project_name, self.design_name
@@ -213,25 +214,23 @@
 
     @property
     def hybrid(self):
         """HFSS hybrid mode for the active solution."""
         return self.design_solutions.hybrid
 
     @hybrid.setter
-    @pyaedt_function_handler()
     def hybrid(self, value):
         self.design_solutions.hybrid = value
 
     @property
     def composite(self):
         """HFSS composite mode for the active solution."""
         return self.design_solutions.composite
 
     @composite.setter
-    @pyaedt_function_handler()
     def composite(self, value):
         self.design_solutions.composite = value
 
     @pyaedt_function_handler()
     def set_auto_open(self, enable=True, boundary_type="Radiation"):
         """Set the HFSS auto open type.
 
@@ -1393,15 +1392,15 @@
 
         >>> oEditor.InsertNativeComponent
 
         Examples
         --------
         >>> from pyaedt import Hfss
         >>> hfss = Hfss(solution_type="SBR+")  # doctest: +SKIP
-        pyaedt INFO: Added design 'HFSS_IPO' of type HFSS.
+        PyAEDT INFO: Added design 'HFSS_IPO' of type HFSS.
         >>> parm = {"polarization": "Vertical"}  # doctest: +SKIP
         >>> par_beam = hfss.create_sbr_antenna(hfss.SbrAntennas.ShortDipole,
         ...                                    parameters_dict=parm,
         ...                                    antenna_name="TX1")  # doctest: +SKIP
 
         """
         if self.solution_type != "SBR+":
@@ -1679,15 +1678,15 @@
         >>> box1 = hfss.modeler.create_box([0, 0, 50], [10, 10, 5],
         ...                                "BoxLumped1","copper")
         >>> box2 = hfss.modeler.create_box([0, 0, 60], [10, 10, 5],
         ...                                "BoxLumped2", "copper")
         >>> hfss.create_lumped_port_between_objects("BoxLumped1", "BoxLumped2",
         ...                                         hfss.AxisDir.XNeg, 50,
         ...                                         "LumpedPort", True, False)
-        pyaedt INFO: Connection Correctly created
+        PyAEDT INFO: Connection Correctly created
         'LumpedPort'
 
         """
         warnings.warn("Use :func:`lumped_port` method instead.", DeprecationWarning)
         return self.lumped_port(
             signal=startobj,
             reference=endobject,
@@ -1921,15 +1920,15 @@
         >>> box1 = hfss.modeler.create_box([30, 0, 0], [40, 10, 5],
         ...                                "BoxVolt1", "copper")
         >>> box2 = hfss.modeler.create_box([30, 0, 10], [40, 10, 5],
         ...                                "BoxVolt2", "copper")
         >>> v1 = hfss.create_voltage_source_from_objects("BoxVolt1", "BoxVolt2",
         ...                                         hfss.AxisDir.XNeg,
         ...                                         "VoltageSource")
-        pyaedt INFO: Connection Correctly created
+        PyAEDT INFO: Connection Correctly created
 
         """
 
         if not self.modeler.does_object_exists(startobj) or not self.modeler.does_object_exists(endobject):
             self.logger.error("One or both objects doesn't exists. Check and retry")
             return False
         if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
@@ -1977,15 +1976,15 @@
         >>> box1 = hfss.modeler.create_box([30, 0, 20], [40, 10, 5],
         ...                                "BoxCurrent1", "copper")
         >>> box2 = hfss.modeler.create_box([30, 0, 30], [40, 10, 5],
         ...                                "BoxCurrent2", "copper")
         >>> i1 = hfss.create_current_source_from_objects("BoxCurrent1", "BoxCurrent2",
         ...                                         hfss.AxisDir.XPos,
         ...                                         "CurrentSource")
-        pyaedt INFO: Connection created 'CurrentSource' correctly.
+        PyAEDT INFO: Connection created 'CurrentSource' correctly.
 
         """
 
         if not self.modeler.does_object_exists(startobj) or not self.modeler.does_object_exists(endobject):
             self.logger.error("One or both objects do not exist. Check and retry.")
             return False
         if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
@@ -2093,15 +2092,15 @@
         >>> box1 = hfss.modeler.create_box([0,0,0], [10,10,5],
         ...                                           "BoxWave1", "copper")
         >>> box2 = hfss.modeler.create_box([0, 0, 10], [10, 10, 5],
         ...                                           "BoxWave2", "copper")
         >>> wave_port = hfss.create_wave_port_between_objects("BoxWave1", "BoxWave2",
         ...                                                   hfss.AxisDir.XNeg, 50, 1,
         ...                                                   "Wave Port", False)
-        pyaedt INFO: Connection Correctly created
+        PyAEDT INFO: Connection Correctly created
 
         """
         warnings.warn(
             "`create_wave_port_between_objects` is deprecated. Use `wave_port` property instead.", DeprecationWarning
         )
         return self.wave_port(
             signal=startobj,
@@ -2541,15 +2540,15 @@
         >>> sub = hfss.modeler.create_box([0, 5, -2], [20, 100, 2],
         ...                               name="SUB1", matname="FR4_epoxy")
         >>> gnd = hfss.modeler.create_box([0, 5, -2.2], [20, 100, 0.2],
         ...                               name="GND1", matname="FR4_epoxy")
         >>> port = hfss.create_wave_port_microstrip_between_objects("GND1", "MS1",
         ...                                                         portname="MS1",
         ...                                                         axisdir=1)
-        pyaedt INFO: Connection correctly created.
+        PyAEDT INFO: Connection correctly created.
 
         """
         warnings.warn(
             "`create_wave_port_microstrip_between_objects` is deprecated. Use `wave_port` property instead.",
             DeprecationWarning,
         )
         return self.wave_port(
@@ -2609,15 +2608,15 @@
 
         >>> box1 = hfss.modeler.create_box([0,0,0], [10,10,5],
         ...                                "perfect1", "Copper")
         >>> box2 = hfss.modeler.create_box([0, 0, 10], [10, 10, 5],
         ...                                "perfect2", "copper")
         >>> perfect_e = hfss.create_perfecte_from_objects("perfect1", "perfect2",
         ...                                               hfss.AxisDir.ZNeg, "PerfectE")
-        pyaedt INFO: Connection Correctly created
+        PyAEDT INFO: Connection Correctly created
         >>> type(perfect_e)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
         if not self.modeler.does_object_exists(startobj) or not self.modeler.does_object_exists(endobject):
             self.logger.error("One or both objects do not exist. Check and retry.")
@@ -2670,15 +2669,15 @@
 
         >>> box1 = hfss.modeler.create_box([0,0,20], [10,10,5],
         ...                                "perfect1", "Copper")
         >>> box2 = hfss.modeler.create_box([0, 0, 30], [10, 10, 5],
         ...                                "perfect2", "copper")
         >>> perfect_h = hfss.create_perfecth_from_objects("perfect1", "perfect2",
         ...                                               hfss.AxisDir.ZNeg, "Perfect H")
-        pyaedt INFO: Connection Correctly created
+        PyAEDT INFO: Connection Correctly created
         >>> type(perfect_h)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
         if not self.modeler.does_object_exists(startobj) or not self.modeler.does_object_exists(endobject):
             self.logger.error("One or both objects do not exist. Check and retry.")
@@ -2821,15 +2820,15 @@
         >>> box1 = hfss.modeler.create_box([0, 0, 50], [10, 10, 5],
         ...                                           "rlc1", "copper")
         >>> box2 = hfss.modeler.create_box([0, 0, 60], [10, 10, 5],
         ...                                           "rlc2", "copper")
         >>> rlc = hfss.create_lumped_rlc_between_objects("rlc1", "rlc2", hfss.AxisDir.XPos,
         ...                                              "Lumped RLC", Rvalue=50,
         ...                                              Lvalue=1e-9, Cvalue = 1e-6)
-        pyaedt INFO: Connection Correctly created
+        PyAEDT INFO: Connection Correctly created
 
         """
 
         if not self.modeler.does_object_exists(startobj) or not self.modeler.does_object_exists(endobject):
             self.logger.error("One or both objects do not exist. Check and retry.")
             return False
         if self.solution_type in ["Modal", "Terminal", "Transient Network"] and (Rvalue or Lvalue or Cvalue):
@@ -2916,15 +2915,15 @@
 
         >>> box1 = hfss.modeler.create_box([0, 0, 70], [10, 10, 5],
         ...                                           "box1", "copper")
         >>> box2 = hfss.modeler.create_box([0, 0, 80], [10, 10, 5],
         ...                                           "box2", "copper")
         >>> impedance = hfss.create_impedance_between_objects("box1", "box2", hfss.AxisDir.XPos,
         ...                                                   "ImpedanceExample", 100, 50)
-        pyaedt INFO: Connection Correctly created
+        PyAEDT INFO: Connection Correctly created
 
         """
 
         if not self.modeler.does_object_exists(startobj) or not self.modeler.does_object_exists(endobject):
             self.logger.error("One or both objects do not exist. Check and retry.")
             return False
         if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
@@ -3802,15 +3801,15 @@
         >>> sheet = hfss.modeler.create_circle(hfss.PLANE.YZ,
         ...                                    [-20, 0, 0], 10,
         ...                                    name="sheet_for_source")
         >>> hfss.solution_type = "Modal"
         >>> wave_port = hfss.create_wave_port_from_sheet(sheet, 5, hfss.AxisDir.XNeg, 40,
         ...                                              2, "SheetWavePort", True)
         >>> hfss.edit_source("SheetWavePort" + ":1", "10W")
-        pyaedt INFO: Setting up power to "SheetWavePort:1" = 10W
+        PyAEDT INFO: Setting up power to "SheetWavePort:1" = 10W
         True
 
         """
 
         if self.solution_type != "Eigenmode":
             if portandmode is None:
                 self.logger.error("Port and mode must be defined for solution type {}".format(self.solution_type))
@@ -3952,15 +3951,15 @@
 
         >>> sheet_for_thickness = hfss.modeler.create_circle(hfss.PLANE.YZ,
         ...                                                  [60, 60, 60], 10,
         ...                                                  name="SheetForThickness")
         >>> port_for_thickness = hfss.create_wave_port_from_sheet(sheet_for_thickness, 5, hfss.AxisDir.XNeg,
         ...                                                       40, 2, "WavePortForThickness", True)
         >>> hfss.thicken_port_sheets(["SheetForThickness"], 2)
-        pyaedt INFO: done
+        PyAEDT INFO: done
         {}
 
         """
 
         tol = 1e-6
         ports_ID = {}
         aedt_bounding_box = self.modeler.get_model_bounding_box()
@@ -4101,15 +4100,15 @@
 
         Examples
         --------
 
         Validate the current design and save the log file in the current project directory.
 
         >>> validation = hfss.validate_full_design()
-        pyaedt INFO: Design Validation Checks
+        PyAEDT INFO: Design Validation Checks
         >>> validation[1]
         False
 
         """
 
         self.logger.info("Design validation checks.")
         validation_ok = True
@@ -6003,15 +6002,15 @@
         >>> box1 = hfss.modeler.create_box([0, 0, 50], [10, 10, 5],
         ...                                "BoxLumped1","copper")
         >>> box2 = hfss.modeler.create_box([0, 0, 60], [10, 10, 5],
         ...                                "BoxLumped2", "copper")
         >>> hfss.lumped_port("BoxLumped1", "BoxLumped2",
         ...                  hfss.AxisDir.XNeg, 50,
         ...                  "LumpedPort", True, False)
-        pyaedt INFO: Connection Correctly created
+        PyAEDT INFO: Connection Correctly created
         'LumpedPort'
 
         """
         if create_port_sheet:
             signal = self.modeler.convert_to_selections(signal)
             reference = self.modeler.convert_to_selections(reference)
             if not self.modeler.does_object_exists(signal) or not self.modeler.does_object_exists(reference):
@@ -6144,15 +6143,15 @@
         >>> sub = hfss.modeler.create_box([0, 5, -2], [20, 100, 2],
         ...                               name="SUB1", matname="FR4_epoxy")
         >>> gnd = hfss.modeler.create_box([0, 5, -2.2], [20, 100, 0.2],
         ...                               name="GND1", matname="FR4_epoxy")
         >>> port = hfss.wave_port("GND1", "MS1",
         ...                       name="MS1",
         ...                        integration_line=1)
-        pyaedt INFO: Connection correctly created.
+        PyAEDT INFO: Connection correctly created.
 
         """
         oname = ""
 
         if create_port_sheet:
             if not self.modeler.does_object_exists(signal) or not self.modeler.does_object_exists(reference):
                 self.logger.error("One or both objects do not exist. Check and retry.")
```

### Comparing `pyaedt-0.6.76/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.77/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/icepak.py` & `pyaedt-0.6.77/pyaedt/icepak.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.generic.DataHandlers import _arg2dict
 from pyaedt.generic.DataHandlers import random_string
 from pyaedt.generic.configurations import ConfigurationsIcepak
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import NativeComponentObject
 from pyaedt.modules.monitor_icepak import Monitor
 
@@ -90,46 +91,46 @@
     --------
 
     Create an instance of Icepak and connect to an existing Icepak
     design or create a new Icepak design if one does not exist.
 
     >>> from pyaedt import Icepak
     >>> icepak = Icepak()
-    pyaedt INFO: No project is defined. Project ...
-    pyaedt INFO: Active design is set to ...
+    PyAEDT INFO: No project is defined. Project ...
+    PyAEDT INFO: Active design is set to ...
 
     Create an instance of Icepak and link to a project named
     ``IcepakProject``. If this project does not exist, create one with
     this name.
 
     >>> icepak = Icepak("IcepakProject")
-    pyaedt INFO: Project ...
-    pyaedt INFO: Added design ...
+    PyAEDT INFO: Project ...
+    PyAEDT INFO: Added design ...
 
     Create an instance of Icepak and link to a design named
     ``IcepakDesign1`` in a project named ``IcepakProject``.
 
     >>> icepak = Icepak("IcepakProject", "IcepakDesign1")
-    pyaedt INFO: Added design 'IcepakDesign1' of type Icepak.
+    PyAEDT INFO: Added design 'IcepakDesign1' of type Icepak.
 
     Create an instance of Icepak and open the specified project,
     which is ``myipk.aedt``.
 
     >>> icepak = Icepak("myipk.aedt")
-    pyaedt INFO: Project myipk has been created.
-    pyaedt INFO: No design is present. Inserting a new design.
-    pyaedt INFO: Added design ...
+    PyAEDT INFO: Project myipk has been created.
+    PyAEDT INFO: No design is present. Inserting a new design.
+    PyAEDT INFO: Added design ...
 
     Create an instance of Icepak using the 2021 R1 release and
     open the specified project, which is ``myipk2.aedt``.
 
     >>> icepak = Icepak(specified_version="2021.2", projectname="myipk2.aedt")
-    pyaedt INFO: Project...
-    pyaedt INFO: No design is present. Inserting a new design.
-    pyaedt INFO: Added design...
+    PyAEDT INFO: Project...
+    PyAEDT INFO: No design is present. Inserting a new design.
+    PyAEDT INFO: Added design...
     """
 
     def __init__(
         self,
         projectname=None,
         designname=None,
         solution_type=None,
@@ -169,15 +170,14 @@
     def problem_type(self):
         """Problem type of the Icepak design. Options are ``"TemperatureAndFlow"``, ``"TemperatureOnly"``,
         and ``"FlowOnly"``.
         """
         return self.design_solutions.problem_type
 
     @problem_type.setter
-    @pyaedt_function_handler()
     def problem_type(self, value="TemperatureAndFlow"):
         self.design_solutions.problem_type = value
 
     @property
     def existing_analysis_sweeps(self):
         """Existing analysis setups.
 
@@ -305,16 +305,16 @@
         --------
 
         Create an opening boundary for the faces of the ``"USB_GND"`` object.
 
         >>> faces = icepak.modeler["USB_GND"].faces
         >>> face_names = [face.id for face in faces]
         >>> boundary = icepak.assign_openings(face_names)
-        pyaedt INFO: Face List boundary_faces created
-        pyaedt INFO: Opening Assigned
+        PyAEDT INFO: Face List boundary_faces created
+        PyAEDT INFO: Opening Assigned
         """
         boundary_name = generate_unique_name("Opening")
         self.modeler.create_face_list(air_faces, "boundary_faces" + boundary_name)
         props = {}
         air_faces = self.modeler.convert_to_selections(air_faces, True)
 
         props["Faces"] = air_faces
@@ -415,15 +415,15 @@
         --------
 
         Create block boundaries from each box in the list.
 
         >>> box1 = icepak.modeler.create_box([1, 1, 1], [3, 3, 3], "BlockBox1", "copper")
         >>> box2 = icepak.modeler.create_box([2, 2, 2], [4, 4, 4], "BlockBox2", "copper")
         >>> blocks = icepak.create_source_blocks_from_list([["BlockBox1", 2], ["BlockBox2", 4]])
-        pyaedt INFO: Block on ...
+        PyAEDT INFO: Block on ...
         >>> blocks[1].props
         {'Objects': ['BlockBox1'], 'Block Type': 'Solid', 'Use External Conditions': False, 'Total Power': '2W'}
         >>> blocks[3].props
         {'Objects': ['BlockBox2'], 'Block Type': 'Solid', 'Use External Conditions': False, 'Total Power': '4W'}
         """
         oObjects = self.modeler.solid_names
         listmcad = []
@@ -478,15 +478,15 @@
         >>> oModule.AssignBlockBoundary
 
         Examples
         --------
 
         >>> box = icepak.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox3", "copper")
         >>> block = icepak.create_source_block("BlockBox3", "1W", False)
-        pyaedt INFO: Block on ...
+        PyAEDT INFO: Block on ...
         >>> block.props
         {'Objects': ['BlockBox3'], 'Block Type': 'Solid', 'Use External Conditions': False, 'Total Power': '1W'}
 
         """
         if assign_material:
             if isinstance(object_name, list):
                 for el in object_name:
@@ -680,15 +680,15 @@
         >>> source2.props["Temperature"]
         '28cel'
 
         """
         if input_power == 0:
             input_power = "0W"
         if not bool(input_power) ^ bool(thermal_dependent_dataset):
-            self.logger.error("Please assigned one input between ``thermal_dependent_dataset`` and  ``input_power``")
+            self.logger.error("Assign one input between ``thermal_dependent_dataset`` and  ``input_power``.")
         if not source_name:
             source_name = generate_unique_name("Source")
         props = {}
         if isinstance(face_id, int):
             props["Faces"] = [face_id]
         elif isinstance(face_id, str):
             props["Objects"] = [face_id]
@@ -765,15 +765,16 @@
 
         >>> box = icepak.modeler.create_box([4, 5, 6], [5, 5, 5], "NetworkBox1", "copper")
         >>> block = icepak.create_network_block("NetworkBox1", "2W", 20, 10, icepak.GravityDirection.ZNeg, 1.05918)
         >>> block.props["Nodes"]["Internal"][0]
         '2W'
         """
         warnings.warn(
-            "This method is deprecated in 0.6.27. Please use create_two_resistor_network_block", DeprecationWarning
+            "This method is deprecated in 0.6.27. Use the create_two_resistor_network_block() method.",
+            DeprecationWarning,
         )
         if object_name in self.modeler.object_names:
             if gravity_dir > 2:
                 gravity_dir = gravity_dir - 3
             faces_dict = self.modeler[object_name].faces
             faceCenter = {}
             for f in faces_dict:
@@ -3785,36 +3786,50 @@
         Assign block boundary for solid objects.
 
         Parameters
         ----------
         object_name : str
             Name of the object.
         power_assignment : str or dict
-            String with value and units of the power assignment or with ``"Joule Heating"``.
-            Also, a dictionary can be used for temperature dependent or transient assignment.
-            The dictionary should contain three keys: ``"Type"``, ``"Function"`` and
-            ``"Values"``. Accepted ``"Type"`` values are: ``"Temp Dep"`` and ``"Transient"``.
-            Accepted ``"Function"`` are: ``"Linear"``, ``"Power Law"``, ``"Exponential"``,
-            ``"Sinusoidal"``, ``"Square Wave"`` and ``"Piecewise Linear"``. ``"Temp Dep"`` only
-            support the latter. ``"Values"`` contains a list of strings containing the parameters
-            required by the ``"Function"`` selection (e.g. ``"Linear"`` requires two parameters:
-            the value of the variable at t=0 and the slope of the line). The parameters required by
-            each ``Function`` option is in Icepak documentation. The parameters must contain the
-            units where needed.
+            String with the value and units of the power assignment or with
+            ``"Joule Heating"``. For a temperature-dependent or transient
+            assignment, a dictionary can be used. The dictionary should contain three keys:
+            ``"Type"``, ``"Function"``, and ``"Values"``.
+
+            - For the ``"Type"`` key, accepted values are ``"Temp Dep"`` and ``"Transient"``.
+            - For the ``"Function"`` key, acceptable values depend on the ``"Type"`` key
+              selection. When the ``"Type"`` key is set to ``"Temp Dep"``, the only
+              accepted value is ````"Piecewise Linear"`` . When the ``"Type"`` key is
+              set to ``"Transient"``, acceptable values are `"Exponential"``, `"Linear"``,
+              ```"Piecewise Linear"``, ``"Power Law"``, ``"Sinusoidal"``, and ``"Square
+               Wave"``.
+            - For the ``"Values"`` key, a list of strings contain the parameters required by
+              the ``"Function"`` key selection. For example, whn``"Linear"`` is set as the
+              ``"Function"`` key, two parameters are required: the value of the variable
+              at t=0 and the slope of the line. For the parameters required by each
+              ``"Function"`` key selection, see the Icepack documentation (). The parameters
+              must contain the units where needed.
+
         boundary_name : str, optional
-            Name of the source boundary. The default is ``None`` and the boundary name will be
-            generated automatically.
-        htc : float, str or dict, optional
-            String with value and units of heat transfer coefficient for the external conditions.
-            Also, a dictionary can be used for temperature dependent or transient assignment as
-            described in ``power_assignment``. The default is ``None``
+            Name of the source boundary. The default is ``None``, in which case the
+            boundary name is automatically generated.
+        htc : float, str, or dict, optional
+            String with the value and units of the heat transfer coefficient for the
+            external conditions. If a float is provided, ``"w_per_m2kel"`` unit will be used.
+            For a temperature-dependent or transient
+            assignment, a dictionary can be used. For more information, see the
+            description for the preceding ``power_assignment`` parameter. The
+            default is ``None``, in which case no external condition will be applied.
         ext_temperature : float, str or dict, optional
-            String with value and units of temperature for the external conditions.
-            Also, a dictionary can be used for transient assignment as described in ``power_assignment``.
-            The default is ``"AmbientTemp"`` and will have effect if ``htc`` is not ``None``
+            String with the value and units of temperature for the external conditions.
+            If a float is provided, ``"cel"`` unit will be used.
+            For a transient assignment, a dictionary can be used. For more information,
+            see the description for the preceding ``power_assignment`` parameter. The
+            default is ``"AmbientTemp"``, which is used if the ``htc`` parameter is not
+            set to ``None``.
 
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object when successful or ``None`` when failed.
 
@@ -3830,19 +3845,19 @@
         >>> ipk.solution_type = "Transient"
         >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox3", "copper")
         >>> power_dict = {"Type": "Transient", "Function": "Sinusoidal", "Values": ["0W", 1, 1, "1s"]}
         >>> block = ipk.assign_solid_block("BlockBox3", power_dict)
         """
         if not self.modeler.get_object_from_name(object_name).solve_inside:
             self.logger.add_error_message(
-                "Please use ``assign_hollow_block`` function with this object as" "``solve_inside`` is ``False``."
+                "Use the ``assign_hollow_block()`` method with this object as ``solve_inside`` is ``False``."
             )
             return None
         if ext_temperature != "AmbientTemp" and ext_temperature is not None and not htc:
-            self.logger.add_error_message("Please set an argument for ``htc`` or remove ``ext_temperature`` argument.")
+            self.logger.add_error_message("Set an argument for ``htc`` or remove the ``ext_temperature`` argument.")
             return None
         if isinstance(ext_temperature, dict) and ext_temperature["Type"] == "Temp Dep":
             self.logger.add_error_message(
                 'It is not possible to use a "Temp Dep" assignment for ' "temperature assignment."
             )
             return None
         props = {"Block Type": "Solid", "Objects": [object_name]}
@@ -3898,35 +3913,47 @@
         Assign block boundary for hollow objects.
 
         Parameters
         ----------
         object_name : str
             Name of the object.
         assignment_type : str
-            Type of the boundary assignment. The accepted types are: "Total Power", "Heat Flux",
-            "Temperature" or "Heat Transfer Coefficient".
+            Type of the boundary assignment. Options are ``"Heat Transfer Coefficient"``,
+            ``"Heat Flux"``, ``"Temperature"``, and ``"Total Power"``.
         assignment_value : str or dict
-            String with value and units of the assignment. If ``"Total Power"`` is assignment_type,
-            ``"Joule Heating"`` can be used.
-            Also, a dictionary can be used for temperature dependent or transient assignment.
-            The dictionary should contain three keys: ``"Type"``, ``"Function"`` and
-            ``"Values"``. Accepted ``"Type"`` values are: ``"Temp Dep"`` and ``"Transient"``.
-            Accepted ``"Function"`` are: ``"Linear"``, ``"Power Law"``, ``"Exponential"``,
-            ``"Sinusoidal"``, ``"Square Wave"`` and ``"Piecewise Linear"``. ``"Temp Dep"`` only
-            support the latter. ``"Values"`` contains a list of strings containing the parameters
-            required by the ``"Function"`` selection (e.g. ``"Linear"`` requires two parameters:
-            the value of the variable at t=0 and the slope of the line). The parameters required by
-            each ``Function`` option is in Icepak documentation. The parameters must contain the
-            units where needed.
+            String with value and units of the assignment. If ``"Total Power"`` is
+            assignment_type, ``"Joule Heating"`` can be used.
+            For a temperature-dependent or transient assignment, a dictionary can be used.
+            The dictionary should contain three keys:
+            ``"Type"``, ``"Function"``, and ``"Values"``.
+
+            - For the ``"Type"`` key, accepted values are ``"Temp Dep"`` and ``"Transient"``.
+            - For the ``"Function"`` key, acceptable values depend on the ``"Type"`` key
+              selection. When the ``"Type"`` key is set to ``"Temp Dep"``, the only
+              accepted value is ````"Piecewise Linear"`` . When the ``"Type"`` key is
+              set to ``"Transient"``, acceptable values are `"Exponential"``, `"Linear"``,
+              ```"Piecewise Linear"``, ``"Power Law"``, ``"Sinusoidal"``, and ``"Square
+               Wave"``.
+            - For the ``"Values"`` key, a list of strings contain the parameters required by
+              the ``"Function"`` key selection. For example, whn``"Linear"`` is set as the
+              ``"Function"`` key, two parameters are required: the value of the variable
+              at t=0 and the slope of the line. For the parameters required by each
+              ``"Function"`` key selection, see the Icepack documentation (). The parameters
+              must contain the units where needed.
+
         boundary_name : str, optional
-            Name of the source boundary. The default is ``None`` and the boundary name will be
-            generated automatically.
+            Name of the source boundary. The default is ``None``, in which case the
+            boundary is automatically generated.
         external_temperature : str, dict or float, optional
-            String with value and unit of temperature for the Heat Transfer Coefficient. If float,
-            ``"cel"`` unit will be added automatically. The default is ``"AmbientTemp"``.
+            String with the value and unit of the temperature for the heat transfer
+            coefficient. If a float value is specified, the ``"cel"`` unit is automatically
+            added.
+            For a transient assignment, a dictionary can be used as described for the
+            assignment_value argument. Temperature dependent assignment is not supported.
+            The default is ``"AmbientTemp"``.
 
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Boundary object when successful or ``None`` when failed.
 
@@ -3943,15 +3970,15 @@
         >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox5", "copper")
         >>> box.solve_inside = False
         >>> temp_dict = {"Type": "Transient", "Function": "Square Wave", "Values": ["1cel", "0s", "1s", "0.5s", "0cel"]}
         >>> block = ipk.assign_hollow_block("BlockBox5", "Heat Transfer Coefficient", "1w_per_m2kel", "Test", temp_dict)
         """
         if self.modeler.get_object_from_name(object_name).solve_inside:
             self.logger.add_error_message(
-                "Please use ``assign_solid_block`` function with this object as" "``solve_inside`` is ``True``."
+                "Use ``assign_solid_block`` function with this object as" "``solve_inside`` is ``True``."
             )
             return None
         if assignment_value == "Joule Heating" and assignment_type != "Total Power":
             self.logger.add_error_message(
                 '``"Joule Heating"`` assignment is supported only if ``assignment_type``' 'is ``"Total Power"``.'
             )
             return None
@@ -3989,15 +4016,15 @@
             props.update(assignment_value_dict)
         else:
             props[thermal_condition[1]] = assignment_value
         if thermal_condition[0] == "Internal Conditions":
             if isinstance(external_temperature, dict):
                 if external_temperature["Type"] == "Temp Dep":
                     self.logger.add_error_message(
-                        'It is not possible to use a "Temp Dep" assignment for a' "temperature assignment."
+                        'It is not possible to use a "Temp Dep" assignment for a temperature assignment.'
                     )
                     return None
                 assignment_value_dict = self._parse_variation_data(
                     "Temperature",
                     external_temperature["Type"],
                     variation_value=external_temperature["Values"],
                     function=external_temperature["Function"],
```

### Comparing `pyaedt-0.6.76/pyaedt/maxwell.py` & `pyaedt-0.6.77/pyaedt/maxwell.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import re
 
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.generic.DataHandlers import float_units
 from pyaedt.generic.constants import SOLUTIONS
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import MaxwellParameters
 from pyaedt.modules.SetupTemplates import SetupKeys
 
 
@@ -2096,21 +2097,21 @@
     Examples
     --------
     Create an instance of Maxwell 3D and open the specified
     project, which is named ``mymaxwell.aedt``.
 
     >>> from pyaedt import Maxwell3d
     >>> aedtapp = Maxwell3d("mymaxwell.aedt")
-    pyaedt INFO: Added design ...
+    PyAEDT INFO: Added design ...
 
     Create an instance of Maxwell 3D using the 2021 R1 release and open
     the specified project, which is named ``mymaxwell2.aedt``.
 
     >>> aedtapp = Maxwell3d(specified_version="2021.2", projectname="mymaxwell2.aedt")
-    pyaedt INFO: Added design ...
+    PyAEDT INFO: Added design ...
 
     """
 
     @property  # for legacy purposes
     def dim(self):
         """Dimensions."""
         return "3D"
@@ -2642,15 +2643,14 @@
 
     @property
     def xy_plane(self):
         """Maxwell 2D plane between ``True`` and ``False``."""
         return self.design_solutions.xy_plane
 
     @xy_plane.setter
-    @pyaedt_function_handler()
     def xy_plane(self, value=True):
         self.design_solutions.xy_plane = value
 
     @property
     def model_depth(self):
         """Model depth."""
```

### Comparing `pyaedt-0.6.76/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.77/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/mechanical.py` & `pyaedt-0.6.77/pyaedt/mechanical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module contains the ``Mechanical`` class."""
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.SetupTemplates import SetupKeys
 
 
 class Mechanical(FieldAnalysis3D, object):
     """Provides the Mechanical application interface.
```

### Comparing `pyaedt-0.6.76/pyaedt/misc/Console.py_build` & `pyaedt-0.6.77/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.77/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.77/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.77/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.77/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.77/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/amat.xml` & `pyaedt-0.6.77/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/console_setup.py` & `pyaedt-0.6.77/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.77/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.77/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.77/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.77/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/misc.py` & `pyaedt-0.6.77/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.77/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.77/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.77/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.77/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.77/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.77/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/misc/template.acf` & `pyaedt-0.6.77/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/actors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.modeler.advanced_cad.multiparts import Actor
 from pyaedt.modeler.advanced_cad.multiparts import MultiPartComponent
 
 
 def read_actors(fn, actor_lib):
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 import os
 
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.generic.filesystem import get_json_files
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.advanced_cad.parts import Antenna
 from pyaedt.modeler.advanced_cad.parts import Part
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class MultiPartComponent(object):
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/parts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class Part(object):
     """Manages 3D component placement and definition.
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     except ImportError:
         pass
 
 from pyaedt import constants
 from pyaedt import pyaedt_path
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.MaterialLib import Material
 
 LAYERS = {"s": "signal", "g": "ground", "d": "dielectric"}
 
 
 def _replace_by_underscore(character, string):
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.77/pyaedt/modeler/cad/Modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import warnings
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
 from pyaedt.modeler.cad.object3d import Object3d
 from pyaedt.modeler.geometry_operators import GeometryOperators
@@ -184,15 +185,15 @@
         Returns
         -------
         list
             List of changed properties of the coordinate system.
 
         """
         arguments = ["NAME:AllTabs", ["NAME:Geometry3DCSTab", ["NAME:PropServers", name], arg]]
-        _retry_ntimes(5, self._modeler.oeditor.ChangeProperty, arguments)
+        _retry_ntimes(10, self._modeler.oeditor.ChangeProperty, arguments)
 
     @pyaedt_function_handler()
     def rename(self, newname):
         """Rename the coordinate system.
 
         Parameters
         ----------
@@ -2829,15 +2830,15 @@
         vArg2 = ["NAME:DuplicateToAlongLineParameters"]
         vArg2.append("CreateNewObjects:="), vArg2.append(not attachObject)
         vArg2.append("XComponent:="), vArg2.append(Xpos)
         vArg2.append("YComponent:="), vArg2.append(Ypos)
         vArg2.append("ZComponent:="), vArg2.append(Zpos)
         vArg2.append("Numclones:="), vArg2.append(str(nclones))
         vArg3 = ["NAME:Options", "DuplicateAssignments:=", duplicate_assignment]
-        _retry_ntimes(5, self.oeditor.DuplicateAlongLine, vArg1, vArg2, vArg3)
+        _retry_ntimes(10, self.oeditor.DuplicateAlongLine, vArg1, vArg2, vArg3)
         if is_3d_comp:
             return self._duplicate_added_components_tuple()
         if attachObject:
             return True, []
         return self._duplicate_added_objects_tuple()
 
     @pyaedt_function_handler()
@@ -3184,15 +3185,15 @@
 
     @pyaedt_function_handler()
     def subtract(self, blank_list, tool_list, keep_originals=True, **kwargs):
         """Subtract objects.
 
         Parameters
         ----------
-        blank_list : list of Object3d or list of int
+        blank_list : str, Object3d, int or List of str, int and Object3d.
             List of objects to subtract from. The list can be of
             either :class:`pyaedt.modeler.Object3d.Object3d` objects or object IDs.
         tool_list : list
             List of objects to subtract. The list can be of
             either Object3d objects or object IDs.
         keep_originals : bool, optional
             Whether to keep the original objects. The default is ``True``.
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.77/pyaedt/modeler/cad/Primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from pyaedt.application.Variables import Variable
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import is_number
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import Plane
 from pyaedt.modeler.cad.elements3d import Point
 from pyaedt.modeler.cad.object3d import Object3d
 from pyaedt.modeler.cad.polylines import Polyline
@@ -120,35 +121,35 @@
 
         Returns
         -------
         list of :class:`pyaedt.modeler.object3d.Object3d`
             3D object.
         """
         self._refresh_unclassified()
-        return [self[name] for name in self._unclassified]
+        return [self[name] for name in self._unclassified if name is not None]
 
     @property
     def object_list(self):
         """List of all objects.
 
         Returns
         -------
         list of :class:`pyaedt.modeler.object3d.Object3d`
             3D object.
         """
         self._refresh_object_types()
-        return [self[name] for name in self._all_object_names]
+        return [self[name] for name in self._all_object_names if name is not None]
 
     @property
     def solid_names(self):
         """List of the names of all solid objects.
 
         Returns
         -------
-        str
+        List
         """
         self._refresh_solids()
         return self._solids
 
     @property
     def sheet_names(self):
         """List of the names of all sheet objects.
@@ -1501,33 +1502,42 @@
         Parameters
         ----------
         materialname : str
             Name of the material. The default is ``None``.
 
         Returns
         -------
-        list
+        list of class:`pyaedt.modeler.cad.object3d.Object3d`
             If a material name is not provided, the method returns
-            a list of dictionaries where keys are the material names
-            and values are objects assigned to this material.
+            a list of dictionaries where keys are material names
+            of conductors, dielectrics, gases and liquids respectively
+            in the design and values are objects assigned to these materials.
             If a material name is provided, the method returns a list
-            of objects assigned to this material.
+            of objects assigned to the material.
 
         References
         ----------
 
         >>> oEditor.GetObjectsByMaterial
 
         """
+        obj_lst = []
         if materialname is not None:
-            obj_lst = [
-                x
-                for x in self.object_list
-                if x.material_name == materialname or x.material_name == materialname.lower()
-            ]
+            for obj in self.object_list:
+                if obj and ("[" in obj.material_name or "(" in obj.material_name):
+                    material = (
+                        self._app.odesign.GetChildObject("3D Modeler")
+                        .GetChildObject(obj.name)
+                        .GetPropEvaluatedValue("Material")
+                        .lower()
+                    )
+                    if materialname.lower() == material:
+                        obj_lst.append(obj)
+                elif obj and (obj.material_name == materialname or obj.material_name == materialname.lower()):
+                    obj_lst.append(obj)
         else:
             obj_lst = [
                 self._get_object_dict_by_material(self.materials.conductors),
                 self._get_object_dict_by_material(self.materials.dielectrics),
                 self._get_object_dict_by_material(self.materials.gases),
                 self._get_object_dict_by_material(self.materials.liquids),
             ]
@@ -3161,19 +3171,31 @@
                             break
             except:
                 self.logger.info("Native component properties were not retrieved from the AEDT file.")
 
         return native_comp_properties
 
     @pyaedt_function_handler
-    def _get_object_dict_by_material(self, material_type):
+    def _get_object_dict_by_material(self, material):
         obj_dict = {}
-        for cond in material_type:
-            obj = [x for x in self.object_list if x.material_name == cond]
-            obj_dict[cond] = obj
+        for mat in material:
+            objs = []
+            for obj in self.object_list:
+                if obj and ("[" in obj.material_name or "(" in obj.material_name):
+                    if (
+                        mat
+                        == self._app.odesign.GetChildObject("3D Modeler")
+                        .GetChildObject(obj.name)
+                        .GetPropEvaluatedValue("Material")
+                        .lower()
+                    ):
+                        objs.append(obj)
+                elif obj and (obj.material_name == mat or obj.material_name == mat.lower()):
+                    objs.append(obj)
+            obj_dict[mat] = objs
         return obj_dict
 
     @pyaedt_function_handler()
     def __getitem__(self, partId):
         """Get the object ``Object3D`` for a given object ID or object name.
 
         Parameters
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.77/pyaedt/modeler/cad/Primitives2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Primitives import Primitives
 
 
 class Primitives2D(Primitives, object):
     """Manages primitives in 2D tools.
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.77/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.77/pyaedt/modeler/cad/components_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import absolute_import
 
 from collections import OrderedDict
 import random
 import re
 import warnings
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.general_methods import _uname
 from pyaedt.modeler.cad.elements3d import BinaryTreeNode
 from pyaedt.modeler.cad.elements3d import _dict2arg
 
 
 class UserDefinedComponentParameters(dict):
@@ -825,21 +826,21 @@
          name: {}
          group_name: {}
          mesh_assembly: {}
          parameters: {}
          target_coordinate_system: {}
          """.format(
             type(self),
-            self.is3dcomponent,
-            self.parts,
-            self.name,
-            self.group_name,
-            self.mesh_assembly,
-            self.parameters,
-            self.target_coordinate_system,
+            self._is3dcomponent,
+            self._parts,
+            self._m_name,
+            self._group_name,
+            self._mesh_assembly,
+            self._parameters,
+            self._target_coordinate_system,
         )
 
     @pyaedt_function_handler()
     def edit_definition(self, password=""):
         """Edit 3d Definition. Open AEDT Project and return Pyaedt Object.
 
         Parameters
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.77/pyaedt/modeler/cad/elements3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import absolute_import
 
 from collections import OrderedDict
 
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import clamp
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import rgb_color_codes
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 @pyaedt_function_handler()
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.77/pyaedt/modeler/cad/object3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _to_boolean
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import clamp
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import rgb_color_codes
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import BinaryTreeNode
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
@@ -1872,30 +1873,13 @@
 
     @pyaedt_function_handler()
     def _change_property(self, vPropChange):
         return self._primitives._change_geometry_property(vPropChange, self._m_name)
 
     def __str__(self):
         return """
-         {}
          name: {}    id: {}    object_type: {}
-         --- read/write properties  ----
-         solve_inside: {}
-         model: {}
-         material_name: {}
-         color: {}
-         transparency: {}
-         display_wireframe {}
-         part_coordinate_system: {}
          """.format(
-            type(self),
             self.name,
             self.id,
-            self.object_type,
-            self.solve_inside,
-            self.model,
-            self.material_name,
-            self.color,
-            self.transparency,
-            self.display_wireframe,
-            self.part_coordinate_system,
+            self._object_type,
         )
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.77/pyaedt/modeler/cad/polylines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import absolute_import
 
 import math
 import warnings
 
 from pyaedt import _retry_ntimes
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import PLANE
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.cad.object3d import Object3d
 from pyaedt.modeler.geometry_operators import GeometryOperators
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/calculators.py` & `pyaedt-0.6.77/pyaedt/modeler/calculators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 
 from pyaedt import constants
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import SpeedOfLight
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class TransmissionLine(object):
     """Provides base methods common to transmission line calculation.
 
     Parameters
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import filter_string
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import recursive_glob
 from pyaedt.modeler.circuits.object3dcircuit import CircuitComponent
 from pyaedt.modeler.circuits.object3dcircuit import Wire
 
 
 class CircuitComponents(object):
@@ -363,44 +364,49 @@
         References
         ----------
 
         >>> oModelManager.Add
         >>> oComponentManager.Add
         """
 
-        def _parse_ports_name(file):
+        def _parse_ports_name(file, num_terminal):
             """Parse and interpret the option line in the touchstone file.
 
             Parameters
             ----------
             file : str
                 Path of the Touchstone file.
+            num_terminal : int
+                Number of terminals.
 
             Returns
             -------
             List of str
                 Names of the ports in the touchstone file.
 
             """
             portnames = []
             line = file.readline()
-            while not line.startswith("! Port"):
-                line = file.readline()
-            while line.startswith("! Port"):
-                portnames.append(line.split(" = ")[1].strip())
+            while not line.startswith("! Port") and line.find("S11") == -1:
                 line = file.readline()
+            if line.startswith("! Port"):
+                while line.startswith("! Port"):
+                    portnames.append(line.split(" = ")[1].strip())
+                    line = file.readline()
+            else:  # pragma: no cover
+                portnames = ["Port" + str(n) for n in range(1, num_terminal + 1)]
             return portnames
 
         if not model_name:
             model_name = os.path.splitext(os.path.basename(touchstone_full_path))[0]
         if model_name in list(self.o_model_manager.GetNames()):
             model_name = generate_unique_name(model_name, n=2)
         num_terminal = int(os.path.splitext(touchstone_full_path)[1].lower().strip(".sp"))
         with open_file(touchstone_full_path, "r") as f:
-            port_names = _parse_ports_name(f)
+            port_names = _parse_ports_name(f, num_terminal)
         image_subcircuit_path = os.path.join(self._modeler._app.desktop_install_dir, "syslib", "Bitmaps", "nport.bmp")
 
         if not port_names:
             port_names = ["Port" + str(i + 1) for i in range(num_terminal)]
         arg = [
             "NAME:" + model_name,
             "Name:=",
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import defaultdict
 
 from pyaedt.emit_core import EmitConstants as emit_consts
 import pyaedt.generic.constants as consts
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EmitComponents(object):
     """EmitComponents class.
 
     This is the class for managing all EMIT components.
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.circuits.PrimitivesCircuit import CircuitComponents
 
 
 class MaxwellCircuitComponents(CircuitComponents):
     """MaxwellCircuitComponents class.
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.circuits.PrimitivesCircuit import CircuitComponents
 from pyaedt.modeler.circuits.PrimitivesCircuit import ComponentCatalog
 from pyaedt.modeler.circuits.object3dcircuit import CircuitComponent
 from pyaedt.modules.Boundary import Excitations
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.circuits.PrimitivesCircuit import CircuitComponents
 from pyaedt.modeler.circuits.PrimitivesCircuit import ComponentCatalog
 
 
 class TwinBuilderComponents(CircuitComponents):
     """TwinBuilderComponents class.
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.77/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 
 from collections import OrderedDict
 import math
 
 from pyaedt import _retry_ntimes
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt import settings
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _arg2dict
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.cad.elements3d import _dict2arg
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.77/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.77/pyaedt/modeler/modeler2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 from warnings import warn
 
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import GeometryModeler
 from pyaedt.modeler.cad.Modeler import Modeler
 from pyaedt.modeler.cad.Primitives2D import Primitives2D
 
 
 class ModelerRMxprt(Modeler):
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.77/pyaedt/modeler/modeler3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import datetime
 import json
 import os.path
 import warnings
 
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import GeometryModeler
 from pyaedt.modeler.cad.Primitives3D import Primitives3D
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class Modeler3D(GeometryModeler, Primitives3D, object):
@@ -359,15 +360,15 @@
                                 cs_set.add(cs)
                 out_dict["coordinatesystems"] = copy.deepcopy(config_dict["coordinatesystems"])
                 for cs in list(out_dict["coordinatesystems"]):
                     if cs not in cs_set:
                         del out_dict["coordinatesystems"][cs]
             with open(auxiliary_dict, "w") as outfile:
                 json.dump(out_dict, outfile)
-        return _retry_ntimes(3, self.oeditor.Create3DComponent, arg, arg2, component_file, arg3)
+        return _retry_ntimes(10, self.oeditor.Create3DComponent, arg, arg2, component_file, arg3)
 
     @pyaedt_function_handler()
     def replace_3dcomponent(
         self,
         component_name=None,
         variables_to_include=None,
         object_list=None,
@@ -528,15 +529,15 @@
                 if all(included_obj in objs for included_obj in mesh_comp):
                     used_mesh_ops.append(self._app.mesh.meshoperations[mesh].name)
             arg2.append("MeshOperations:="), arg2.append(used_mesh_ops)
         else:
             arg2.append("MeshOperations:="), arg2.append(meshops)
         arg3 = ["NAME:ImageFile", "ImageFile:=", ""]
         old_components = self.user_defined_component_names
-        _retry_ntimes(3, self.oeditor.ReplaceWith3DComponent, arg, arg2, arg3)
+        _retry_ntimes(10, self.oeditor.ReplaceWith3DComponent, arg, arg2, arg3)
         self.refresh_all_ids()
         new_name = list(set(self.user_defined_component_names) - set(old_components))
         return self.user_defined_components[new_name[0]]
 
     @pyaedt_function_handler()
     def create_coaxial(
         self,
@@ -1127,14 +1128,16 @@
             plt.add_axes(line_width=2, xlabel="X", ylabel="Y", zlabel="Z")
             plt.add_axes_at_origin(x_color=None, y_color=None, z_color=None, line_width=2, labels_off=True)
             plt.show(interactive=True)
 
         if import_in_aedt:
             self.model_units = "meter"
             for part in parts_dict:
+                if not os.path.exists(parts_dict[part]["file_name"]):
+                    continue
                 obj_names = [i for i in self.object_names]
                 self.import_3d_cad(
                     parts_dict[part]["file_name"],
                     create_lightweigth_part=create_lightweigth_part,
                 )
                 added_objs = [i for i in self.object_names if i not in obj_names]
                 if part == "terrain":
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.77/pyaedt/modeler/modelerpcb.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pyaedt.edb import Edb
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import get_filename_without_extension
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import Modeler
 from pyaedt.modeler.pcb.Primitives3DLayout import Primitives3DLayout
 from pyaedt.modeler.pcb.object3dlayout import ComponentsSubCircuit3DLayout
 from pyaedt.modules.LayerStackup import Layers
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.77/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 import warnings
 
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Primitives import default_materials
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modeler.pcb.object3dlayout import Circle3dLayout
 from pyaedt.modeler.pcb.object3dlayout import Components3DLayout
 from pyaedt.modeler.pcb.object3dlayout import ComponentsSubCircuit3DLayout
 from pyaedt.modeler.pcb.object3dlayout import Line3dLayout
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.77/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 from __future__ import absolute_import  # noreorder
 
 import math
 import re
 
 from pyaedt import _retry_ntimes
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class Objec3DLayout(object):
```

### Comparing `pyaedt-0.6.76/pyaedt/modeler/schematic.py` & `pyaedt-0.6.77/pyaedt/modeler/schematic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import random
 import re
 
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _retry_ntimes
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import Modeler
 from pyaedt.modeler.circuits.PrimitivesEmit import EmitComponent
 from pyaedt.modeler.circuits.PrimitivesEmit import EmitComponents
 from pyaedt.modeler.circuits.PrimitivesMaxwellCircuit import MaxwellCircuitComponents
 from pyaedt.modeler.circuits.PrimitivesNexxim import NexximComponents
 from pyaedt.modeler.circuits.PrimitivesTwinBuilder import TwinBuilderComponents
@@ -236,59 +237,102 @@
 
         References
         ----------
 
         >>> oEditor.CreateText
 
         """
+        fill = {
+            0: "Hollow",
+            1: "Solid",
+            2: "NE Diagonal",
+            3: "Orthogonal Cross",
+            4: "Diagonal Cross",
+            5: "NW Diagonal",
+            6: "Horizontal",
+            7: "Vertical",
+        }
+        x_origin, y_origin = self.schematic._convert_point_to_meter([x_origin, y_origin])
+        x1, y1 = self.schematic._convert_point_to_meter([x1, y1])
+        x2, y2 = self.schematic._convert_point_to_meter([x2, y2])
+
         element_ids = []
         for el in self.oeditor.GetAllGraphics():
             element_ids.append(int(el.split("@")[1]))
         system_random = random.SystemRandom()
         text_id = system_random.randint(20000, 23000)
         while text_id in element_ids:
             text_id = system_random.randint(20000, 23000)
         args = [
             "NAME:TextData",
             "X:=",
             x_origin,
             "Y:=",
             y_origin,
             "Size:=",
-            text_size,
+            12,
             "Angle:=",
-            text_angle,
+            0,
             "Text:=",
             text,
             "Color:=",
-            text_color,
+            0,
             "Id:=",
             text_id,
             "ShowRect:=",
             show_rect,
             "X1:=",
             x1,
             "Y1:=",
             y1,
             "X2:=",
             x2,
             "Y2:=",
             y2,
             "RectLineWidth:=",
-            rect_line_width,
+            0,
             "RectBorderColor:=",
-            rect_border_color,
+            0,
             "RectFill:=",
-            rect_fill,
+            0,
             "RectColor:=",
-            rect_color,
+            0,
         ]
         a = ["NAME:Attributes", "Page:=", 1]
         try:
-            return self.oeditor.CreateText(args, a)
+            text_out = self.oeditor.CreateText(args, a)
+            if isinstance(text_color, (tuple, list)):
+                r, g, b = text_color
+            else:
+                r = (text_color >> 16) & 0xFF
+                g = (text_color >> 8) & 0xFF
+                b = (text_color >> 0) & 0xFF
+            if isinstance(rect_color, (tuple, list)):
+                r2, g2, b2 = rect_color
+            else:
+                r2 = (rect_color >> 16) & 0xFF
+                g2 = (rect_color >> 8) & 0xFF
+                b2 = (rect_color >> 0) & 0xFF
+            if isinstance(rect_border_color, (tuple, list)):
+                r3, g3, b3 = rect_border_color
+            else:
+                r3 = (rect_border_color >> 16) & 0xFF
+                g3 = (rect_border_color >> 8) & 0xFF
+                b3 = (rect_border_color >> 0) & 0xFF
+            self.change_text_property(str(text_id), "Color", [r, g, b])
+            self.change_text_property(str(text_id), "Angle", self._arg_with_dim(text_angle, "deg"))
+            self.change_text_property(str(text_id), "DisplayRectangle", show_rect)
+            if show_rect:
+                self.change_text_property(str(text_id), "Rectangle Color", [r2, g2, b2])
+                self.change_text_property(
+                    str(text_id), "Rectangle BorderWidth", self._arg_with_dim(rect_line_width, "mil")
+                )
+                self.change_text_property(str(text_id), "Rectangle BorderColor", [r3, g3, b3])
+                self.change_text_property(str(text_id), "Rectangle FillStyle", fill[rect_fill])
+            return text_out
         except:
             return False
 
     @pyaedt_function_handler
     def change_text_property(self, property_id, property_name, property_value):  # pragma: no cover
         """Change an oeditor property.
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.77/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modules/Boundary.py` & `pyaedt-0.6.77/pyaedt/modules/Boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.DataHandlers import random_string
 from pyaedt.generic.constants import CATEGORIESQ3D
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.generic.general_methods import filter_tuple
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
 from pyaedt.modules.CircuitTemplates import SourceKeys
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.77/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.77/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.77/pyaedt/modules/DesignXPloration.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import copy
 import csv
 
 from pyaedt.generic.DataHandlers import _arg2dict
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.OptimetricsTemplates import defaultdoeSetup
 from pyaedt.modules.OptimetricsTemplates import defaultdxSetup
 from pyaedt.modules.OptimetricsTemplates import defaultoptiSetup
 from pyaedt.modules.OptimetricsTemplates import defaultparametricSetup
 from pyaedt.modules.OptimetricsTemplates import defaultsensitivitySetup
 from pyaedt.modules.OptimetricsTemplates import defaultstatisticalSetup
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.77/pyaedt/modules/LayerStackup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import unit_converter
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 @pyaedt_function_handler()
 def _str2bool(str0):
     """Convert a string to a Boolean value.
 
@@ -965,17 +966,17 @@
                         "Roughness:=",
                         self._arg_with_dim(self.roughness, self.LengthUnitRough),
                         "BotRoughness:=",
                         self._arg_with_dim(self.bottom_roughness, self.LengthUnitRough),
                         "SideRoughness:=",
                         self._arg_with_dim(self.top_roughness, self.LengthUnitRough),
                         "Material:=",
-                        self.material.lower(),
+                        self._layers._app.materials[self.material].name if self.material != "" else "",
                         "FillMaterial:=",
-                        self.fill_material.lower(),
+                        self._layers._app.materials[self.fill_material].name if self.fill_material != "" else "",
                     ],
                     "Neg:=",
                     self._is_negative,
                     "Usp:=",
                     self.usp,
                     [
                         "NAME:Sp",
@@ -1057,15 +1058,15 @@
                         "Roughness:=",
                         0,
                         "BotRoughness:=",
                         0,
                         "SideRoughness:=",
                         0,
                         "Material:=",
-                        self.material.lower(),
+                        self.material,
                     ],
                 ]
             )
         else:
             args.extend(
                 [
                     "Type:=",
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/Material.py` & `pyaedt-0.6.77/pyaedt/modules/Material.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 * `SufaceMaterial`
 
 """
 from collections import OrderedDict
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import CSS4_COLORS
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class MatProperties(object):
     """Contains a list of constant names for all materials with
     mappings to their internal XML names.
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.77/pyaedt/modules/MaterialLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pyaedt import is_ironpython
 from pyaedt import settings
 from pyaedt.generic.DataHandlers import _arg2dict
 from pyaedt.generic.general_methods import _create_json_file
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Material import MatProperties
 from pyaedt.modules.Material import Material
 from pyaedt.modules.Material import OrderedDict
 from pyaedt.modules.Material import SurfaceMaterial
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/Mesh.py` & `pyaedt-0.6.77/pyaedt/modules/Mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from pyaedt.application.design_solutions import model_names
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
 from pyaedt.generic.general_methods import MethodNotSupportedError
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
 
 meshers = {
@@ -280,15 +281,15 @@
         Returns
         -------
         list
             List of changed properties of the mesh operation.
 
         """
         arguments = ["NAME:AllTabs", ["NAME:MeshSetupTab", ["NAME:PropServers", "MeshSetup:{}".format(name)], arg]]
-        _retry_ntimes(5, self._mesh._app.odesign.ChangeProperty, arguments)
+        _retry_ntimes(10, self._mesh._app.odesign.ChangeProperty, arguments)
 
     @pyaedt_function_handler()
     def delete(self):
         """Delete the mesh.
 
         Returns
         -------
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.77/pyaedt/modules/Mesh3DLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Mesh import MeshProps
 
 
 class Mesh3DOperation(PropsManager, object):
     """Mesh3DOperation class.
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.77/pyaedt/modules/MeshIcepak.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from collections import OrderedDict
 
 from pyaedt import settings
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Mesh import MeshOperation
 from pyaedt.modules.Mesh import meshers
 
 
 class IcepakMesh(object):
     """Manages Icepak meshes.
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.77/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.77/pyaedt/modules/PostProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import check_and_download_file
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 import pyaedt.modules.report_templates as rt
 from pyaedt.modules.solutions import FieldPlot
 from pyaedt.modules.solutions import SolutionData
 from pyaedt.modules.solutions import VRTFieldPlot
 
 if not is_ironpython:
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.77/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.77/pyaedt/modules/SolveSetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import time
 import warnings
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSweeps import SetupProps
 from pyaedt.modules.SolveSweeps import SweepHFSS
 from pyaedt.modules.SolveSweeps import SweepHFSS3DLayout
 from pyaedt.modules.SolveSweeps import SweepMatrix
 from pyaedt.modules.SolveSweeps import identify_setup
@@ -75,14 +76,15 @@
         num_gpu=0,
         acf_file=None,
         use_auto_settings=True,
         solve_in_batch=False,
         machine="localhost",
         run_in_thread=False,
         revert_to_initial_mesh=False,
+        blocking=True,
     ):
         """Solve the active design.
 
         Parameters
         ----------
         num_cores : int, optional
             Number of simulation cores. Default is ``1``.
@@ -101,14 +103,17 @@
         machine : str, optional
             Name of the machine if remote.  The default is ``"localhost"``.
         run_in_thread : bool, optional
             Whether to submit the batch command as a thread. The default is
             ``False``.
         revert_to_initial_mesh : bool, optional
             Whether to revert to initial mesh before solving or not. Default is ``False``.
+        blocking : bool, optional
+            Whether to block script while analysis is completed or not. It works from AEDT 2023 R2.
+            Default is ``True``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
@@ -123,14 +128,15 @@
             num_gpu=num_gpu,
             acf_file=acf_file,
             use_auto_settings=use_auto_settings,
             solve_in_batch=solve_in_batch,
             machine=machine,
             run_in_thread=run_in_thread,
             revert_to_initial_mesh=revert_to_initial_mesh,
+            blocking=blocking,
         )
 
     @pyaedt_function_handler()
     def _init_props(self, isnewsetup=False):
         if isnewsetup:
             setup_template = SetupKeys.get_setup_templates()[self.setuptype]
             self.props = SetupProps(self, setup_template)
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.77/pyaedt/modules/SolveSweeps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import copy
 from difflib import SequenceMatcher
 import json
 import os
 import sys
 import warnings
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
 from pyaedt.modules.SetupTemplates import Sweep3DLayout
 from pyaedt.modules.SetupTemplates import SweepHfss3D
 from pyaedt.modules.SetupTemplates import SweepSiwave
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.77/pyaedt/modules/monitor_icepak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import SI_UNITS
 from pyaedt.generic.constants import unit_system
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Monitor:
     """Provides Icepak monitor methods."""
 
     def __init__(self, p_app):
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/report_templates.py` & `pyaedt-0.6.77/pyaedt/modules/report_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import re
 
 from pyaedt.generic.constants import LineStyle
 from pyaedt.generic.constants import SymbolStyle
 from pyaedt.generic.constants import TraceType
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 def _props_with_default(dict_in, key, default_value=None):
     return dict_in[key] if dict_in.get(key, None) is not None else default_value
```

### Comparing `pyaedt-0.6.76/pyaedt/modules/solutions.py` & `pyaedt-0.6.77/pyaedt/modules/solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import math
 import os
 import sys
 import time
 
 from pyaedt import get_pyaedt_app
 from pyaedt import is_ironpython
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt import settings
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import db10
 from pyaedt.generic.constants import db20
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import check_and_download_folder
```

### Comparing `pyaedt-0.6.76/pyaedt/q3d.py` & `pyaedt-0.6.77/pyaedt/q3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pyaedt import is_ironpython
 from pyaedt import settings
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import MATRIXOPERATIONSQ2D
 from pyaedt.generic.constants import MATRIXOPERATIONSQ3D
 from pyaedt.generic.general_methods import generate_unique_name
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators as go
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import Matrix
 from pyaedt.modules.SetupTemplates import SetupKeys
 
 if not is_ironpython:
```

### Comparing `pyaedt-0.6.76/pyaedt/rmxprt.py` & `pyaedt-0.6.77/pyaedt/rmxprt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module contains these classes: ``RMXprtModule`` and ``Rmxprt``."""
 from __future__ import absolute_import  # noreorder
 
 from pyaedt.application.AnalysisRMxprt import FieldAnalysisRMxprt
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class RMXprtModule(object):
     """Provides RMxprt module properties."""
 
     component = None
@@ -240,15 +241,14 @@
 
     @property
     def design_type(self):
         """Machine design type."""
         return self.design_solutions.design_type
 
     @design_type.setter
-    @pyaedt_function_handler()
     def design_type(self, value):
         self.design_solutions.design_type = value
 
     @pyaedt_function_handler()
     def create_setup(self, setupname="MySetupAuto", setuptype=None, **kwargs):
         """Create an analysis setup for RmXport.
```

### Comparing `pyaedt-0.6.76/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.77/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.77/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.77/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.77/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.77/pyaedt/sbrplus/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import math
 import os
 import warnings
 
 import numpy as np
 import pyvista as pv
 
+from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.plot import CommonPlotter
 from pyaedt.generic.plot import ObjClass
 
 
 class HDMPlotter(CommonPlotter):
```

### Comparing `pyaedt-0.6.76/pyaedt/siwave.py` & `pyaedt-0.6.77/pyaedt/siwave.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import sys
 import time
 
 from pyaedt.generic.clr_module import _clr
 from pyaedt.generic.general_methods import _pythonver
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_windows
+from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.misc import list_installed_ansysem
 
 
 class Siwave(object):
     """Initializes SIwave based on the inputs provided and manages SIwave release and closing.
```

### Comparing `pyaedt-0.6.76/pyaedt/twinbuilder.py` & `pyaedt-0.6.77/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.76/pyproject.toml` & `pyaedt-0.6.77/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,45 +32,45 @@
     "psutil",
     "dotnetcore2 ==3.1.23;platform_system=='Linux'",
 ]
 
 [project.optional-dependencies]
 tests = [
     "ipython==8.13.0",
-    "imageio==2.28.0",
+    "imageio==2.29.0",
     "joblib==1.2.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
-    "pytest-xdist==3.3.0",
+    "pytest-xdist==3.3.1",
     "pyvista==0.39.1",
     "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
     "ansys-sphinx-theme==0.9.9",
-    "imageio==2.28.0",
+    "imageio==2.29.0",
     "imageio-ffmpeg==0.4.8",
     "ipython==8.13.0",
     "ipywidgets==8.0.6",
     "joblib==1.2.0",
     "jupyterlab==4.0.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
-    "nbsphinx==0.9.1",
+    "nbsphinx==0.9.2",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
     "pyvista==0.39.1",
     "recommonmark==0.7.1",
     "scikit-learn==1.2.2",
@@ -83,30 +83,30 @@
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 full = [
-    "imageio==2.28.0",
+    "imageio==2.29.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
     "pyvista==0.39.1",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
-    "imageio==2.28.0",
+    "imageio==2.29.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
```

### Comparing `pyaedt-0.6.76/PKG-INFO` & `pyaedt-0.6.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.76
+Version: 0.6.77
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -17,37 +17,37 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cffi == 1.15.1;platform_system=='Linux'
 Requires-Dist: pywin32 >= 303;platform_system=='Windows'
 Requires-Dist: pythonnet == 3.0.1
 Requires-Dist: rpyc==5.3.1
 Requires-Dist: psutil
 Requires-Dist: dotnetcore2 ==3.1.23;platform_system=='Linux'
-Requires-Dist: imageio==2.28.0 ; extra == "all"
+Requires-Dist: imageio==2.29.0 ; extra == "all"
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
 Requires-Dist: pyvista==0.39.1 ; extra == "all"
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
-Requires-Dist: imageio==2.28.0 ; extra == "doc"
+Requires-Dist: imageio==2.29.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
 Requires-Dist: ipython==8.13.0 ; extra == "doc"
 Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
 Requires-Dist: joblib==1.2.0 ; extra == "doc"
 Requires-Dist: jupyterlab==4.0.0 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
-Requires-Dist: nbsphinx==0.9.1 ; extra == "doc"
+Requires-Dist: nbsphinx==0.9.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
 Requires-Dist: pyvista==0.39.1 ; extra == "doc"
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
 Requires-Dist: scikit-learn==1.2.2 ; extra == "doc"
@@ -58,41 +58,41 @@
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
 Requires-Dist: openpyxl==3.1.2 ; extra == "doc"
-Requires-Dist: imageio==2.28.0 ; extra == "full"
+Requires-Dist: imageio==2.29.0 ; extra == "full"
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
 Requires-Dist: pyvista==0.39.1 ; extra == "full"
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
 Requires-Dist: ipython==8.13.0 ; extra == "tests"
-Requires-Dist: imageio==2.28.0 ; extra == "tests"
+Requires-Dist: imageio==2.29.0 ; extra == "tests"
 Requires-Dist: joblib==1.2.0 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
-Requires-Dist: pytest-xdist==3.3.0 ; extra == "tests"
+Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
 Requires-Dist: pyvista==0.39.1 ; extra == "tests"
 Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
 Project-URL: Bug Tracker, https://github.com/pyansys/pyaedt/issues
 Project-URL: Documentation, https://aedt.docs.pyansys.com
```

