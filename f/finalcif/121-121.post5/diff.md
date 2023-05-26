# Comparing `tmp/finalcif-121.tar.gz` & `tmp/finalcif-121.post5.tar.gz`

## Comparing `finalcif-121.tar` & `finalcif-121.post5.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-121/finalcif/__init__.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 finalcif-121/finalcif/app_path.py
--rw-r--r--   0        0        0    92019 2020-02-02 00:00:00.000000 finalcif-121/finalcif/appwindow.py
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 finalcif-121/finalcif/finalcif_start.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/all_cif_dicts.py
--rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/atoms.py
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cif_dict_foo.py
--rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cif_file_io.py
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cif_order.py
--rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/core_dict.py
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/hkl.py
--rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/modulation_dict.py
--rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/powder_dict.py
--rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/reference.py
--rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/restraints_dict.py
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/text.py
--rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/twin_dict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/checkcif/__init__.py
--rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/checkcif/checkcif.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/__init__.py
--rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/deposit.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/deposit_check.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/deposition_list.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/doi.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/upload.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-121/finalcif/cif/cod/website_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/__init__.py
--rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/bruker_data.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/bruker_frame.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/ccdc_mail.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/data.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/p4p_reader.py
--rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/sadabs.py
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/saint.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/shelx_lst.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-121/finalcif/datafiles/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/displaymol/__init__.py
--rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 finalcif-121/finalcif/displaymol/molecule2D.py
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-121/finalcif/displaymol/sdm.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-121/finalcif/displaymol/vtk_molecule.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/__init__.py
--rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/author_loop_templates.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/equipment.py
--rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/properties.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 finalcif-121/finalcif/equip_property/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/__init__.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/combobox.py
--rw-r--r--   0        0        0    11048 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/custom_classes.py
--rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/dialogs.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/equipmenttable.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/file_editor.py
--rw-r--r--   0        0        0   162120 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/finalcif_gui_ui.py
--rw-r--r--   0        0        0   187031 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/finalcif_gui_ui.ui
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/loop_creator.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/loop_creator_ui.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/loop_creator_ui.ui
--rw-r--r--   0        0        0    11548 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/loops.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/mainstackwidget.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/mixins.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/new_key_dialog.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/new_key_dialog_ui.py
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/new_key_dialog_ui.ui
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/plaintextedit.py
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/playground.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/propertytable.py
--rw-r--r--   0        0        0    12927 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/spell_check_edit.py
--rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/text_templates_ui.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/text_templates_ui.ui
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/text_value_editor.py
--rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 finalcif-121/finalcif/gui/vrf_classes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/__init__.py
--rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/finalcif.png
--rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/finalcif2.ico
--rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/finalcif2.png
--rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/multitable.ico
--rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/multitable.png
--rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-121/finalcif/icon/multitable.xcf
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/__init__.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/archive_report.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/mtools.py
--rw-r--r--   0        0        0    19119 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/references.py
--rw-r--r--   0        0        0    24577 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/report_text.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/symm.py
--rw-r--r--   0        0        0    37156 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/tables.py
--rw-r--r--   0        0        0    26709 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/templated_report.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/gui/__init__.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/gui/mainwindow.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-121/finalcif/report/gui/mainwindow.ui
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/__init__.py
--rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/mathml2omml.xsl
--rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/template1.docx
--rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/template_text.docx
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/template_without_text.docx
--rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 finalcif-121/finalcif/template/templates.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/__init__.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/download.py
--rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/dsrmath.py
--rw-r--r--   0        0        0    32788 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/misc.py
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/options.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/platon.py
--rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/pupdate.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/settings.py
--rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/shred.py
--rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/space_groups.py
--rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/spgr_format.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/statusbar.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-121/finalcif/tools/sumformula.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 finalcif-121/.gitignore
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-121/LICENSE
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 finalcif-121/README.md
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 finalcif-121/pyproject.toml
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 finalcif-121/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/__init__.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/app_path.py
+-rw-r--r--   0        0        0    93493 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/appwindow.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/finalcif_start.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/all_cif_dicts.py
+-rw-r--r--   0        0        0    18681 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/atoms.py
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cif_dict_foo.py
+-rw-r--r--   0        0        0    38969 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cif_file_io.py
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cif_order.py
+-rw-r--r--   0        0        0   484078 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/core_dict.py
+-rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/hkl.py
+-rw-r--r--   0        0        0  1041931 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/modulation_dict.py
+-rw-r--r--   0        0        0   221592 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/powder_dict.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/reference.py
+-rw-r--r--   0        0        0   106774 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/restraints_dict.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/text.py
+-rw-r--r--   0        0        0    21412 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/twin_dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/checkcif/__init__.py
+-rw-r--r--   0        0        0    10770 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/checkcif/checkcif.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cod/__init__.py
+-rw-r--r--   0        0        0    18635 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cod/deposit.py
+-rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cod/deposit_check.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cod/deposition_list.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cod/doi.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cod/upload.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/cif/cod/website_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/__init__.py
+-rw-r--r--   0        0        0    12742 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/bruker_data.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/bruker_frame.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/ccdc_mail.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/data.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/p4p_reader.py
+-rw-r--r--   0        0        0     7148 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/sadabs.py
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/saint.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/shelx_lst.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/datafiles/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/displaymol/__init__.py
+-rw-r--r--   0        0        0    11614 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/displaymol/molecule2D.py
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/displaymol/sdm.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/displaymol/vtk_molecule.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/equip_property/__init__.py
+-rw-r--r--   0        0        0    21598 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/equip_property/author_loop_templates.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/equip_property/equipment.py
+-rw-r--r--   0        0        0    13453 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/equip_property/properties.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/equip_property/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/__init__.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/combobox.py
+-rw-r--r--   0        0        0    11048 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/custom_classes.py
+-rw-r--r--   0        0        0     7931 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/dialogs.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/equipmenttable.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/file_editor.py
+-rw-r--r--   0        0        0   162120 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/finalcif_gui_ui.py
+-rw-r--r--   0        0        0   187031 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/finalcif_gui_ui.ui
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/loop_creator.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/loop_creator_ui.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/loop_creator_ui.ui
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/loops.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/mainstackwidget.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/mixins.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/new_key_dialog.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/new_key_dialog_ui.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/new_key_dialog_ui.ui
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/plaintextedit.py
+-rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/playground.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/propertytable.py
+-rw-r--r--   0        0        0    12927 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/spell_check_edit.py
+-rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/text_templates_ui.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/text_templates_ui.ui
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/text_value_editor.py
+-rw-r--r--   0        0        0     6745 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/gui/vrf_classes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/icon/__init__.py
+-rw-r--r--   0        0        0    13567 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/icon/finalcif.png
+-rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/icon/finalcif2.ico
+-rw-r--r--   0        0        0    17091 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/icon/finalcif2.png
+-rw-r--r--   0        0        0   103782 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/icon/multitable.ico
+-rw-r--r--   0        0        0    17746 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/icon/multitable.png
+-rw-r--r--   0        0        0   124043 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/icon/multitable.xcf
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/archive_report.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/mtools.py
+-rw-r--r--   0        0        0    19119 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/references.py
+-rw-r--r--   0        0        0    24577 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/report_text.py
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/symm.py
+-rw-r--r--   0        0        0    37156 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/tables.py
+-rw-r--r--   0        0        0    26709 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/templated_report.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/gui/__init__.py
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/gui/mainwindow.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/report/gui/mainwindow.ui
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/template/__init__.py
+-rw-r--r--   0        0        0   151706 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/template/mathml2omml.xsl
+-rw-r--r--   0        0        0    14998 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/template/template1.docx
+-rw-r--r--   0        0        0    35411 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/template/template_text.docx
+-rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/template/template_without_text.docx
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/template/templates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/__init__.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/download.py
+-rw-r--r--   0        0        0    43454 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/dsrmath.py
+-rw-r--r--   0        0        0    32788 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/misc.py
+-rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/options.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/platon.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/pupdate.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/settings.py
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/shred.py
+-rw-r--r--   0        0        0     9596 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/space_groups.py
+-rw-r--r--   0        0        0   137178 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/spgr_format.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/statusbar.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 finalcif-121.post5/finalcif/tools/sumformula.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 finalcif-121.post5/.gitignore
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finalcif-121.post5/LICENSE
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 finalcif-121.post5/README.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 finalcif-121.post5/pyproject.toml
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 finalcif-121.post5/PKG-INFO
```

### Comparing `finalcif-121/finalcif/app_path.py` & `finalcif-121.post5/finalcif/app_path.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/appwindow.py` & `finalcif-121.post5/finalcif/appwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,16 @@
         self.templates = ReportTemplates(self, self.settings)
         if not self.running_inside_unit_test:
             self.check_for_update_version()
         self.textedit = MyTextTemplateEdit(parent=self)
         self.ui.page_textTemplate.layout().addWidget(self.textedit)
         #
         self.connect_signals_and_slots()
-        self.make_button_icons()
+        with suppress(Exception):
+            self.make_button_icons()
         self.format_report_button()
 
     def set_initial_button_states(self) -> None:
         self.ui.appendCifPushButton.setDisabled(True)
         self.ui.PictureWidthDoubleSpinBox.setRange(0.0, 25)
         self.ui.PictureWidthDoubleSpinBox.setSingleStep(0.5)
         # Just too slow for large structures:
@@ -194,59 +195,91 @@
 
     def make_button_icons(self) -> None:
         self.ui.CheckcifButton.setIcon(qta.icon('mdi.file-document-outline'))
         self.ui.CheckcifStartButton.setIcon(qta.icon('mdi.file-document-outline'))
         self.ui.LoopsPushButton.setIcon(qta.icon('mdi.table'))
         self.ui.CheckcifHTMLOnlineButton.setIcon(qta.icon('mdi.comment-check-outline'))
         self.ui.CheckcifPDFOnlineButton.setIcon(qta.icon('mdi.comment-check'))
-        self.ui.SaveFullReportButton.setIcon(qta.icon('mdi.file-table-outline'))
-        self.ui.ExploreDirButton.setIcon(qta.icon('ph.folder-open'))
-        self.ui.SaveCifButton.setIcon(qta.icon('ri.save-3-line'))
-        self.ui.SelectCif_PushButton.setIcon(qta.icon('ri.file-text-line', options=[{'color': 'darkgreen'}]))
-        self.ui.AuthorEditPushButton.setIcon(qta.icon('ph.users-three-bold'))
-        self.ui.SourcesPushButton.setIcon(qta.icon('ph.list-bullets-bold'))
-        self.ui.OptionsPushButton.setIcon(qta.icon('ri.settings-5-line'))
-        self.ui.ShredCifButton.setIcon(qta.icon('ph.files-bold'))
-        self.ui.DetailsPushButton.setIcon(qta.icon('ph.bird-bold'))
+        with suppress(Exception):
+            self.ui.SaveFullReportButton.setIcon(qta.icon('mdi.file-table-outline'))
+        try:
+            self.ui.ExploreDirButton.setIcon(qta.icon('ph.folder-open'))
+        except Exception:
+            self.ui.ExploreDirButton.setIcon(qta.icon('mdi.folder-open-outline'))
+        self.ui.SaveCifButton.setIcon(qta.icon('fa5.save'))
+        self.ui.SelectCif_PushButton.setIcon(qta.icon('fa.file-text-o', options=[{'color': 'darkgreen'}]))
+        try:
+            self.ui.AuthorEditPushButton.setIcon(qta.icon('ph.users-three-bold'))
+        except Exception:
+            self.ui.AuthorEditPushButton.setIcon(qta.icon('fa5s.users'))
+        try:
+            self.ui.SourcesPushButton.setIcon(qta.icon('ph.list-bullets-bold'))
+        except Exception:
+            self.ui.SourcesPushButton.setIcon(qta.icon('fa5s.list-ul'))
+        try:
+            self.ui.OptionsPushButton.setIcon(qta.icon('ph.gear'))
+        except Exception:
+            self.ui.OptionsPushButton.setIcon(qta.icon('fa.gear'))
+        try:
+            self.ui.ShredCifButton.setIcon(qta.icon('ph.files-bold'))
+        except Exception:
+            self.ui.ShredCifButton.setIcon(qta.icon('fa.files-o'))
+        try:
+            self.ui.DetailsPushButton.setIcon(qta.icon('ph.bird-bold'))
+        except Exception:
+            self.ui.DetailsPushButton.setIcon(qta.icon('fa5s.kiwi-bird'))
         self.ui.NewEquipmentTemplateButton.setIcon(qta.icon('mdi.playlist-plus'))
         self.ui.EditEquipmentTemplateButton.setIcon(qta.icon('mdi.playlist-edit'))
         self.ui.DeleteEquipmentButton.setIcon(qta.icon('mdi.playlist-minus'))
         self.ui.ImportEquipmentTemplateButton.setIcon(qta.icon('mdi.import'))
         self.ui.SaveEquipmentButton.setIcon(qta.icon('mdi.content-save-outline'))
         self.ui.CancelEquipmentButton.setIcon(qta.icon('mdi.cancel'))
         self.ui.ExportEquipmentButton.setIcon(qta.icon('mdi.export'))
         self.ui.NewPropertyTemplateButton.setIcon(qta.icon('mdi.playlist-plus'))
         self.ui.EditPropertyTemplateButton.setIcon(qta.icon('mdi.playlist-edit'))
         self.ui.ImportPropertyTemplateButton.setIcon(qta.icon('mdi.import'))
         self.ui.DeletePropertiesButton.setIcon(qta.icon('mdi.playlist-minus'))
         self.ui.SavePropertiesButton.setIcon(qta.icon('mdi.content-save-outline'))
         self.ui.CancelPropertiesButton.setIcon(qta.icon('mdi.cancel'))
         self.ui.ExportPropertyButton.setIcon(qta.icon('mdi.export'))
-        self.ui.CCDCpushButton.setIcon(qta.icon('ph.upload-simple-bold'))
+        try:
+            self.ui.CCDCpushButton.setIcon(qta.icon('ph.upload-simple-bold'))
+        except Exception:
+            self.ui.CCDCpushButton.setIcon(qta.icon('fa5s.cloud-upload-alt'))
         self.ui.CODpushButton.setIcon(qta.icon('mdi.upload'))
         self.ui.SavePushButton.setIcon(qta.icon('mdi.content-save'))
         self.ui.revertLoopsPushButton.setIcon(qta.icon('mdi.backup-restore'))
         # Backbuttons:
         self.ui.BackpushButtonDetails.setIcon(qta.icon('mdi.keyboard-backspace'))
         self.ui.BackFromDepositPushButton.setIcon(qta.icon('mdi.keyboard-backspace'))
         self.ui.BackPushButton.setIcon(qta.icon('mdi.keyboard-backspace'))
         self.ui.BackSourcesPushButton.setIcon(qta.icon('mdi.keyboard-backspace'))
         self.ui.BackFromOptionspPushButton.setIcon(qta.icon('mdi.keyboard-backspace'))
         self.ui.BackFromLoopsPushButton.setIcon(qta.icon('mdi.keyboard-backspace'))
         self.ui.BackFromPlatonPushButton.setIcon(qta.icon('mdi.keyboard-backspace'))
         self.textedit.ui.cancelTextPushButton.setIcon(qta.icon('mdi.keyboard-backspace'))
-        self.textedit.ui.applyTextPushButton.setIcon(qta.icon('ph.check-bold'))
+        try:
+            self.textedit.ui.applyTextPushButton.setIcon(qta.icon('ph.check-bold'))
+        except Exception:
+            self.textedit.ui.applyTextPushButton.setIcon(qta.icon('fa.check'))
         self.textedit.ui.exportTextPushButton.setIcon(qta.icon('mdi.export'))
         self.textedit.ui.savePushButton.setIcon(qta.icon('mdi.content-save'))
         self.textedit.ui.deletePushButton.setIcon(qta.icon('mdi.playlist-minus'))
         self.textedit.ui.importPushButton.setIcon(qta.icon('mdi.import'))
         #
-        self.ui.SaveAuthorLoopToTemplateButton.setIcon(qta.icon('mdi.badge-account-outline'))
-        self.ui.AddThisAuthorToLoopPushButton.setIcon(qta.icon('mdi.folder-table-outline'))
-        self.ui.DeleteLoopAuthorTemplateButton.setIcon(qta.icon('mdi.delete-forever-outline'))
+        try:
+            self.ui.SaveAuthorLoopToTemplateButton.setIcon(qta.icon('mdi.badge-account-outline'))
+        except Exception:
+            self.ui.SaveAuthorLoopToTemplateButton.setIcon(qta.icon('fa.id-badge'))
+        try:
+            self.ui.AddThisAuthorToLoopPushButton.setIcon(qta.icon('mdi.folder-table-outline'))
+        except Exception:
+            self.ui.AddThisAuthorToLoopPushButton.setIcon(qta.icon('mdi.file-table-outline'))
+        with suppress(Exception):
+            self.ui.DeleteLoopAuthorTemplateButton.setIcon(qta.icon('mdi.delete-forever-outline'))
 
     def connect_signals_and_slots(self) -> None:
         """
         this method connects all signals to slots. Only a few mighjt be defined elsewere.
         """
         self.ui.datanameComboBox.currentIndexChanged.connect(self._load_block)
         ## main
@@ -1059,16 +1092,22 @@
                                                       caption='Open a Report Picture')
             self.set_report_picture_path(filename)
 
     def set_report_picture_path(self, filename: str):
         with suppress(Exception):
             self.report_picture_path = Path(filename)
         if self.report_picture_path.exists() and self.report_picture_path.is_file():
+            with suppress(Exception):
+                self.set_picture_button_icon()
+
+    def set_picture_button_icon(self):
+        try:
             self.ui.ReportPicPushButton.setIcon(qta.icon('ph.image-bold'))
-            # self.ui.ReportPicPushButton.setText('')
+        except Exception:
+            self.ui.ReportPicPushButton.setIcon(qta.icon('fa.image'))
 
     def get_checked_templates_list_text(self) -> str:
         for index in range(self.ui.TemplatesListWidget.count()):
             item = self.ui.TemplatesListWidget.item(index)
             if item.checkState() == Qt.Checked:
                 return item.text()
```

### Comparing `finalcif-121/finalcif/finalcif_start.py` & `finalcif-121.post5/finalcif/finalcif_start.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/all_cif_dicts.py` & `finalcif-121.post5/finalcif/cif/all_cif_dicts.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/atoms.py` & `finalcif-121.post5/finalcif/cif/atoms.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cif_dict_foo.py` & `finalcif-121.post5/finalcif/cif/cif_dict_foo.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cif_file_io.py` & `finalcif-121.post5/finalcif/cif/cif_file_io.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cif_order.py` & `finalcif-121.post5/finalcif/cif/cif_order.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/core_dict.py` & `finalcif-121.post5/finalcif/cif/core_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/hkl.py` & `finalcif-121.post5/finalcif/cif/hkl.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/modulation_dict.py` & `finalcif-121.post5/finalcif/cif/modulation_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/powder_dict.py` & `finalcif-121.post5/finalcif/cif/powder_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/reference.py` & `finalcif-121.post5/finalcif/cif/reference.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/restraints_dict.py` & `finalcif-121.post5/finalcif/cif/restraints_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/text.py` & `finalcif-121.post5/finalcif/cif/text.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/twin_dict.py` & `finalcif-121.post5/finalcif/cif/twin_dict.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/checkcif/checkcif.py` & `finalcif-121.post5/finalcif/cif/checkcif/checkcif.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cod/deposit.py` & `finalcif-121.post5/finalcif/cif/cod/deposit.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cod/deposit_check.py` & `finalcif-121.post5/finalcif/cif/cod/deposit_check.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cod/deposition_list.py` & `finalcif-121.post5/finalcif/cif/cod/deposition_list.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cod/doi.py` & `finalcif-121.post5/finalcif/cif/cod/doi.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cod/upload.py` & `finalcif-121.post5/finalcif/cif/cod/upload.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/cif/cod/website_parser.py` & `finalcif-121.post5/finalcif/cif/cod/website_parser.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/bruker_data.py` & `finalcif-121.post5/finalcif/datafiles/bruker_data.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/bruker_frame.py` & `finalcif-121.post5/finalcif/datafiles/bruker_frame.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/ccdc_mail.py` & `finalcif-121.post5/finalcif/datafiles/ccdc_mail.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/data.py` & `finalcif-121.post5/finalcif/datafiles/data.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/p4p_reader.py` & `finalcif-121.post5/finalcif/datafiles/p4p_reader.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/sadabs.py` & `finalcif-121.post5/finalcif/datafiles/sadabs.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/saint.py` & `finalcif-121.post5/finalcif/datafiles/saint.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/shelx_lst.py` & `finalcif-121.post5/finalcif/datafiles/shelx_lst.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/datafiles/utils.py` & `finalcif-121.post5/finalcif/datafiles/utils.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/displaymol/molecule2D.py` & `finalcif-121.post5/finalcif/displaymol/molecule2D.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/displaymol/sdm.py` & `finalcif-121.post5/finalcif/displaymol/sdm.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/displaymol/vtk_molecule.py` & `finalcif-121.post5/finalcif/displaymol/vtk_molecule.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/equip_property/author_loop_templates.py` & `finalcif-121.post5/finalcif/equip_property/author_loop_templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/equip_property/equipment.py` & `finalcif-121.post5/finalcif/equip_property/equipment.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/equip_property/properties.py` & `finalcif-121.post5/finalcif/equip_property/properties.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/equip_property/tools.py` & `finalcif-121.post5/finalcif/equip_property/tools.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/combobox.py` & `finalcif-121.post5/finalcif/gui/combobox.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/custom_classes.py` & `finalcif-121.post5/finalcif/gui/custom_classes.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/dialogs.py` & `finalcif-121.post5/finalcif/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/equipmenttable.py` & `finalcif-121.post5/finalcif/gui/equipmenttable.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/file_editor.py` & `finalcif-121.post5/finalcif/gui/file_editor.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/finalcif_gui_ui.py` & `finalcif-121.post5/finalcif/gui/finalcif_gui_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/finalcif_gui_ui.ui` & `finalcif-121.post5/finalcif/gui/finalcif_gui_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/loop_creator.py` & `finalcif-121.post5/finalcif/gui/loop_creator.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/loop_creator_ui.py` & `finalcif-121.post5/finalcif/gui/loop_creator_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/loop_creator_ui.ui` & `finalcif-121.post5/finalcif/gui/loop_creator_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/loops.py` & `finalcif-121.post5/finalcif/gui/loops.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,18 +133,19 @@
         del_action = QAction('Delete Row', self)
         down_action = QAction('Move row down', self)
         up_action = QAction('Move row up', self)
         add_action.triggered.connect(lambda: self._add_row(event))
         del_action.triggered.connect(lambda: self._delete_row(event))
         up_action.triggered.connect(lambda: self._row_up(event))
         down_action.triggered.connect(lambda: self._row_down(event))
-        up_action.setIcon(qtawesome.icon('mdi.arrow-up'))
-        down_action.setIcon(qtawesome.icon('mdi.arrow-down'))
-        del_action.setIcon(qtawesome.icon('mdi.trash-can-outline'))
-        add_action.setIcon(qtawesome.icon('mdi.table-row-plus-after'))
+        with suppress(Exception):
+            up_action.setIcon(qtawesome.icon('mdi.arrow-up'))
+            down_action.setIcon(qtawesome.icon('mdi.arrow-down'))
+            del_action.setIcon(qtawesome.icon('mdi.trash-can-outline'))
+            add_action.setIcon(qtawesome.icon('mdi.table-row-plus-after'))
         self.menu.addAction(add_action)
         self.menu.addAction(del_action)
         self.menu.addSeparator()
         self.menu.addAction(up_action)
         self.menu.addAction(down_action)
         # add other required actions
         self.menu.popup(QCursor.pos())
```

### Comparing `finalcif-121/finalcif/gui/mainstackwidget.py` & `finalcif-121.post5/finalcif/gui/mainstackwidget.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/mixins.py` & `finalcif-121.post5/finalcif/gui/mixins.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/new_key_dialog.py` & `finalcif-121.post5/finalcif/gui/new_key_dialog.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/new_key_dialog_ui.py` & `finalcif-121.post5/finalcif/gui/new_key_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/new_key_dialog_ui.ui` & `finalcif-121.post5/finalcif/gui/new_key_dialog_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/plaintextedit.py` & `finalcif-121.post5/finalcif/gui/plaintextedit.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/playground.py` & `finalcif-121.post5/finalcif/gui/playground.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/propertytable.py` & `finalcif-121.post5/finalcif/gui/propertytable.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/spell_check_edit.py` & `finalcif-121.post5/finalcif/gui/spell_check_edit.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/text_templates_ui.py` & `finalcif-121.post5/finalcif/gui/text_templates_ui.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/text_templates_ui.ui` & `finalcif-121.post5/finalcif/gui/text_templates_ui.ui`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/text_value_editor.py` & `finalcif-121.post5/finalcif/gui/text_value_editor.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/gui/vrf_classes.py` & `finalcif-121.post5/finalcif/gui/vrf_classes.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/icon/finalcif.png` & `finalcif-121.post5/finalcif/icon/finalcif.png`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/icon/finalcif2.ico` & `finalcif-121.post5/finalcif/icon/finalcif2.ico`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/icon/finalcif2.png` & `finalcif-121.post5/finalcif/icon/finalcif2.png`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/icon/multitable.ico` & `finalcif-121.post5/finalcif/icon/multitable.ico`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/icon/multitable.png` & `finalcif-121.post5/finalcif/icon/multitable.png`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/icon/multitable.xcf` & `finalcif-121.post5/finalcif/icon/multitable.xcf`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/archive_report.py` & `finalcif-121.post5/finalcif/report/archive_report.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/mtools.py` & `finalcif-121.post5/finalcif/report/mtools.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/references.py` & `finalcif-121.post5/finalcif/report/references.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/report_text.py` & `finalcif-121.post5/finalcif/report/report_text.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/symm.py` & `finalcif-121.post5/finalcif/report/symm.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/tables.py` & `finalcif-121.post5/finalcif/report/tables.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/templated_report.py` & `finalcif-121.post5/finalcif/report/templated_report.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/gui/mainwindow.py` & `finalcif-121.post5/finalcif/report/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/report/gui/mainwindow.ui` & `finalcif-121.post5/finalcif/report/gui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/template/mathml2omml.xsl` & `finalcif-121.post5/finalcif/template/mathml2omml.xsl`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/template/template1.docx` & `finalcif-121.post5/finalcif/template/template1.docx`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/template/template_text.docx` & `finalcif-121.post5/finalcif/template/template_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/template/template_without_text.docx` & `finalcif-121.post5/finalcif/template/template_without_text.docx`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/template/templates.py` & `finalcif-121.post5/finalcif/template/templates.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/download.py` & `finalcif-121.post5/finalcif/tools/download.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/dsrmath.py` & `finalcif-121.post5/finalcif/tools/dsrmath.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/misc.py` & `finalcif-121.post5/finalcif/tools/misc.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/options.py` & `finalcif-121.post5/finalcif/tools/options.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/platon.py` & `finalcif-121.post5/finalcif/tools/platon.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/pupdate.py` & `finalcif-121.post5/finalcif/tools/pupdate.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/settings.py` & `finalcif-121.post5/finalcif/tools/settings.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/shred.py` & `finalcif-121.post5/finalcif/tools/shred.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/space_groups.py` & `finalcif-121.post5/finalcif/tools/space_groups.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/spgr_format.py` & `finalcif-121.post5/finalcif/tools/spgr_format.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/statusbar.py` & `finalcif-121.post5/finalcif/tools/statusbar.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/finalcif/tools/sumformula.py` & `finalcif-121.post5/finalcif/tools/sumformula.py`

 * *Files identical despite different names*

### Comparing `finalcif-121/.gitignore` & `finalcif-121.post5/.gitignore`

 * *Files identical despite different names*

### Comparing `finalcif-121/README.md` & `finalcif-121.post5/README.md`

 * *Files identical despite different names*

### Comparing `finalcif-121/pyproject.toml` & `finalcif-121.post5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "finalcif"
-version = "121"
+version = "121.post5"
 authors = [
     { name = "Daniel Kratzert", email = "dkratzert@gmx.de" },
 ]
 description = "CIF file editor"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `finalcif-121/PKG-INFO` & `finalcif-121.post5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finalcif
-Version: 121
+Version: 121.post5
 Summary: CIF file editor
 Project-URL: Homepage, https://dkratzert.de/finalcif.html
 Project-URL: Bug Tracker, https://github.com/dkratzert/FinalCif/issues
 Author-email: Daniel Kratzert <dkratzert@gmx.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: finalcif Version: 121 Summary: CIF file editor
-Project-URL: Homepage, https://dkratzert.de/finalcif.html Project-URL: Bug
-Tracker, https://github.com/dkratzert/FinalCif/issues Author-email: Daniel
+Metadata-Version: 2.1 Name: finalcif Version: 121.post5 Summary: CIF file
+editor Project-URL: Homepage, https://dkratzert.de/finalcif.html Project-URL:
+Bug Tracker, https://github.com/dkratzert/FinalCif/issues Author-email: Daniel
 Kratzert
 gmx.de> License-File: LICENSE Classifier: Development Status :: 5 - Production/
 Stable Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry Requires-Python: >=3.9
 Requires-Dist: altgraph Requires-Dist: certifi Requires-Dist: chardet Requires-
 Dist: crossrefapi Requires-Dist: docxtpl Requires-Dist: future Requires-Dist:
```

