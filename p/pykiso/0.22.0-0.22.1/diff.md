# Comparing `tmp/pykiso-0.22.0.tar.gz` & `tmp/pykiso-0.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykiso-0.22.0.tar", max compression
+gzip compressed data, was "pykiso-0.22.1.tar", max compression
```

## Comparing `pykiso-0.22.0.tar` & `pykiso-0.22.1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    14194 2023-04-17 14:37:25.523320 pykiso-0.22.0/LICENSE
--rw-r--r--   0        0        0     6028 2023-04-17 14:37:25.524320 pykiso-0.22.0/README.md
--rw-r--r--   0        0        0     4289 2023-04-17 14:37:25.725318 pykiso-0.22.0/pyproject.toml
--rw-r--r--   0        0        0     1972 2023-04-17 14:37:25.725318 pykiso-0.22.0/src/pykiso/__init__.py
--rw-r--r--   0        0        0      642 2023-04-17 14:37:25.725318 pykiso-0.22.0/src/pykiso/__main__.py
--rw-r--r--   0        0        0     9480 2023-04-17 14:37:25.725318 pykiso-0.22.0/src/pykiso/auxiliary.py
--rw-r--r--   0        0        0     7920 2023-04-17 14:37:25.725318 pykiso-0.22.0/src/pykiso/cli.py
--rw-r--r--   0        0        0    11837 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/config_parser.py
--rw-r--r--   0        0        0     5559 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/connector.py
--rw-r--r--   0        0        0     2436 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/exceptions.py
--rw-r--r--   0        0        0     4509 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/global_config.py
--rw-r--r--   0        0        0      410 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/interfaces/__init__.py
--rw-r--r--   0        0        0    13651 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/interfaces/dt_auxiliary.py
--rw-r--r--   0        0        0     8975 2023-04-17 14:37:25.726318 pykiso-0.22.0/src/pykiso/interfaces/mp_auxiliary.py
--rw-r--r--   0        0        0     4318 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/interfaces/simple_auxiliary.py
--rw-r--r--   0        0        0     8665 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/interfaces/thread_auxiliary.py
--rw-r--r--   0        0        0      516 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/lib/__init__.py
--rw-r--r--   0        0        0      552 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/__init__.py
--rw-r--r--   0        0        0     8415 2023-04-17 14:37:25.727318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/acroname_auxiliary.py
--rw-r--r--   0        0        0     7916 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/communication_auxiliary.py
--rw-r--r--   0        0        0    12655 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/dut_auxiliary.py
--rw-r--r--   0        0        0     2014 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py
--rw-r--r--   0        0        0    10145 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py
--rw-r--r--   0        0        0    19216 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py
--rw-r--r--   0        0        0     5029 2023-04-17 14:37:25.728318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py
--rw-r--r--   0        0        0    16676 2023-04-17 14:37:25.729318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py
--rw-r--r--   0        0        0    14219 2023-04-17 14:37:25.729318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py
--rw-r--r--   0        0        0    14149 2023-04-17 14:37:25.729318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/proxy_auxiliary.py
--rw-r--r--   0        0        0    17111 2023-04-17 14:37:25.729318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/record_auxiliary.py
--rw-r--r--   0        0        0     2645 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py
--rw-r--r--   0        0        0     6511 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py
--rw-r--r--   0        0        0    14146 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py
--rw-r--r--   0        0        0     3889 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py
--rw-r--r--   0        0        0     4288 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py
--rw-r--r--   0        0        0      718 2023-04-17 14:37:25.730318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/__init__.py
--rw-r--r--   0        0        0      599 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py
--rw-r--r--   0        0        0     3913 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py
--rw-r--r--   0        0        0     5284 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py
--rw-r--r--   0        0        0    12896 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py
--rw-r--r--   0        0        0     1517 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py
--rw-r--r--   0        0        0     1570 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py
--rw-r--r--   0        0        0     2664 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py
--rw-r--r--   0        0        0     1404 2023-04-17 14:37:25.731318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py
--rw-r--r--   0        0        0    12733 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py
--rw-r--r--   0        0        0    17074 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py
--rw-r--r--   0        0        0    13528 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/auxiliaries/ykush_auxiliary.py
--rw-r--r--   0        0        0      548 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/connectors/__init__.py
--rw-r--r--   0        0        0     3999 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_example.py
--rw-r--r--   0        0        0    13274 2023-04-17 14:37:25.732318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_fdx_lauterbach.py
--rw-r--r--   0        0        0     1446 2023-04-17 14:37:25.815317 pykiso-0.22.0/src/pykiso/lib/connectors/cc_flasher_example.py
--rw-r--r--   0        0        0     4966 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_mp_proxy.py
--rw-r--r--   0        0        0    19974 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_pcan_can.py
--rw-r--r--   0        0        0    11002 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_process.py
--rw-r--r--   0        0        0     5697 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_proxy.py
--rw-r--r--   0        0        0     2048 2023-04-17 14:37:25.816318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_raw_loopback.py
--rw-r--r--   0        0        0    14178 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_rtt_segger.py
--rw-r--r--   0        0        0     5713 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_serial.py
--rw-r--r--   0        0        0      538 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/__init__.py
--rw-r--r--   0        0        0     7361 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py
--rw-r--r--   0        0        0     8065 2023-04-17 14:37:25.817318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py
--rw-r--r--   0        0        0     3215 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_tcp_ip.py
--rw-r--r--   0        0        0     5893 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_uart.py
--rw-r--r--   0        0        0     2981 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_udp.py
--rw-r--r--   0        0        0     3425 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_udp_server.py
--rw-r--r--   0        0        0     2440 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_usb.py
--rw-r--r--   0        0        0     7302 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_vector_can.py
--rw-r--r--   0        0        0     7194 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/cc_visa.py
--rw-r--r--   0        0        0     4085 2023-04-17 14:37:25.818318 pykiso-0.22.0/src/pykiso/lib/connectors/flash_jlink.py
--rw-r--r--   0        0        0     8380 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/connectors/flash_lauterbach.py
--rw-r--r--   0        0        0      530 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/__init__.py
--rw-r--r--   0        0        0     4193 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/acroname_auxiliary.py
--rw-r--r--   0        0        0     2380 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/aux_interface.py
--rw-r--r--   0        0        0     3361 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/communication_auxiliary.py
--rw-r--r--   0        0        0     3639 2023-04-17 14:37:25.819317 pykiso-0.22.0/src/pykiso/lib/robot_framework/dut_auxiliary.py
--rw-r--r--   0        0        0    16126 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py
--rw-r--r--   0        0        0     3599 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/loader.py
--rw-r--r--   0        0        0     2321 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/proxy_auxiliary.py
--rw-r--r--   0        0        0     6606 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/record_auxiliary.py
--rw-r--r--   0        0        0     6840 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/lib/robot_framework/uds_auxiliary.py
--rw-r--r--   0        0        0     7770 2023-04-17 14:37:25.820318 pykiso-0.22.0/src/pykiso/logging_initializer.py
--rw-r--r--   0        0        0    11744 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/message.py
--rw-r--r--   0        0        0      410 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/test_coordinator/__init__.py
--rw-r--r--   0        0        0    12735 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/test_coordinator/test_case.py
--rw-r--r--   0        0        0    16086 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/test_coordinator/test_execution.py
--rw-r--r--   0        0        0     5480 2023-04-17 14:37:25.821318 pykiso-0.22.0/src/pykiso/test_coordinator/test_message_handler.py
--rw-r--r--   0        0        0    16859 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_coordinator/test_suite.py
--rw-r--r--   0        0        0      515 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_result/__init__.py
--rw-r--r--   0        0        0    16836 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_result/assert_step_report.py
--rw-r--r--   0        0        0     8391 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_result/multi_result.py
--rw-r--r--   0        0        0     1971 2023-04-17 14:37:25.822317 pykiso-0.22.0/src/pykiso/test_result/templates/report_template.css
--rw-r--r--   0        0        0     5461 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_result/templates/report_template.html.j2
--rw-r--r--   0        0        0     1624 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_result/templates/report_template_script.js
--rw-r--r--   0        0        0     9917 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_result/text_result.py
--rw-r--r--   0        0        0     5663 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_result/xml_result.py
--rw-r--r--   0        0        0      410 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_setup/__init__.py
--rw-r--r--   0        0        0     9772 2023-04-17 14:37:25.823317 pykiso-0.22.0/src/pykiso/test_setup/config_registry.py
--rw-r--r--   0        0        0    14160 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/test_setup/dynamic_loader.py
--rw-r--r--   0        0        0      410 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/__init__.py
--rw-r--r--   0        0        0      410 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/__init__.py
--rw-r--r--   0        0        0     5577 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/cli.py
--rw-r--r--   0        0        0     3114 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2
--rw-r--r--   0        0        0    11816 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/show_tag.py
--rw-r--r--   0        0        0      410 2023-04-17 14:37:25.824318 pykiso-0.22.0/src/pykiso/tool/testrail/__init__.py
--rw-r--r--   0        0        0    12414 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/api.py
--rw-r--r--   0        0        0     7584 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/cli.py
--rw-r--r--   0        0        0     5195 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/console.py
--rw-r--r--   0        0        0     8545 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/containers.py
--rw-r--r--   0        0        0     5075 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/extraction.py
--rw-r--r--   0        0        0    12851 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/tool/testrail/testrail.py
--rw-r--r--   0        0        0     1794 2023-04-17 14:37:25.825317 pykiso-0.22.0/src/pykiso/types.py
--rw-r--r--   0        0        0     9371 1970-01-01 00:00:00.000000 pykiso-0.22.0/setup.py
--rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 pykiso-0.22.0/PKG-INFO
+-rw-r--r--   0        0        0    14194 2023-05-26 11:45:04.349382 pykiso-0.22.1/LICENSE
+-rw-r--r--   0        0        0     6028 2023-05-26 11:45:04.349382 pykiso-0.22.1/README.md
+-rw-r--r--   0        0        0     4289 2023-05-26 11:45:04.542378 pykiso-0.22.1/pyproject.toml
+-rw-r--r--   0        0        0     1972 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/__main__.py
+-rw-r--r--   0        0        0     9480 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/auxiliary.py
+-rw-r--r--   0        0        0     7920 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/cli.py
+-rw-r--r--   0        0        0    11837 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/config_parser.py
+-rw-r--r--   0        0        0     5559 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/connector.py
+-rw-r--r--   0        0        0     2436 2023-05-26 11:45:04.543378 pykiso-0.22.1/src/pykiso/exceptions.py
+-rw-r--r--   0        0        0     4509 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/global_config.py
+-rw-r--r--   0        0        0      410 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/__init__.py
+-rw-r--r--   0        0        0    13651 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/dt_auxiliary.py
+-rw-r--r--   0        0        0     8975 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/mp_auxiliary.py
+-rw-r--r--   0        0        0     4318 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/simple_auxiliary.py
+-rw-r--r--   0        0        0     8665 2023-05-26 11:45:04.544378 pykiso-0.22.1/src/pykiso/interfaces/thread_auxiliary.py
+-rw-r--r--   0        0        0      516 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/__init__.py
+-rw-r--r--   0        0        0     8415 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/acroname_auxiliary.py
+-rw-r--r--   0        0        0     7916 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/communication_auxiliary.py
+-rw-r--r--   0        0        0    12655 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/dut_auxiliary.py
+-rw-r--r--   0        0        0     2014 2023-05-26 11:45:04.545378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py
+-rw-r--r--   0        0        0    10145 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py
+-rw-r--r--   0        0        0    19216 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py
+-rw-r--r--   0        0        0     5029 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py
+-rw-r--r--   0        0        0    16676 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py
+-rw-r--r--   0        0        0    14219 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py
+-rw-r--r--   0        0        0    14149 2023-05-26 11:45:04.546378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/proxy_auxiliary.py
+-rw-r--r--   0        0        0    17111 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/record_auxiliary.py
+-rw-r--r--   0        0        0     2645 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py
+-rw-r--r--   0        0        0     6511 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py
+-rw-r--r--   0        0        0    14146 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py
+-rw-r--r--   0        0        0     3889 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py
+-rw-r--r--   0        0        0     4288 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py
+-rw-r--r--   0        0        0      718 2023-05-26 11:45:04.547378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py
+-rw-r--r--   0        0        0     3913 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py
+-rw-r--r--   0        0        0     5299 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py
+-rw-r--r--   0        0        0    12896 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py
+-rw-r--r--   0        0        0     1517 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py
+-rw-r--r--   0        0        0     1570 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py
+-rw-r--r--   0        0        0     2664 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py
+-rw-r--r--   0        0        0     1404 2023-05-26 11:45:04.548378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py
+-rw-r--r--   0        0        0    12764 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py
+-rw-r--r--   0        0        0    17074 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py
+-rw-r--r--   0        0        0    13528 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/auxiliaries/ykush_auxiliary.py
+-rw-r--r--   0        0        0      548 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/connectors/__init__.py
+-rw-r--r--   0        0        0     3999 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_example.py
+-rw-r--r--   0        0        0    13274 2023-05-26 11:45:04.549378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_fdx_lauterbach.py
+-rw-r--r--   0        0        0     1446 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_flasher_example.py
+-rw-r--r--   0        0        0     4966 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_mp_proxy.py
+-rw-r--r--   0        0        0    19971 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_pcan_can.py
+-rw-r--r--   0        0        0    11002 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_process.py
+-rw-r--r--   0        0        0     5697 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_proxy.py
+-rw-r--r--   0        0        0     2048 2023-05-26 11:45:04.550378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_raw_loopback.py
+-rw-r--r--   0        0        0    14178 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_rtt_segger.py
+-rw-r--r--   0        0        0     5713 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_serial.py
+-rw-r--r--   0        0        0      538 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/__init__.py
+-rw-r--r--   0        0        0     7361 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py
+-rw-r--r--   0        0        0     8065 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py
+-rw-r--r--   0        0        0     3215 2023-05-26 11:45:04.551378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_tcp_ip.py
+-rw-r--r--   0        0        0     5893 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_uart.py
+-rw-r--r--   0        0        0     2981 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_udp.py
+-rw-r--r--   0        0        0     3425 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_udp_server.py
+-rw-r--r--   0        0        0     2440 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_usb.py
+-rw-r--r--   0        0        0     7302 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_vector_can.py
+-rw-r--r--   0        0        0     7194 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/cc_visa.py
+-rw-r--r--   0        0        0     4085 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/flash_jlink.py
+-rw-r--r--   0        0        0     8380 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/connectors/flash_lauterbach.py
+-rw-r--r--   0        0        0      530 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/robot_framework/__init__.py
+-rw-r--r--   0        0        0     4193 2023-05-26 11:45:04.552378 pykiso-0.22.1/src/pykiso/lib/robot_framework/acroname_auxiliary.py
+-rw-r--r--   0        0        0     2380 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/aux_interface.py
+-rw-r--r--   0        0        0     3361 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/communication_auxiliary.py
+-rw-r--r--   0        0        0     3639 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/dut_auxiliary.py
+-rw-r--r--   0        0        0    16126 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py
+-rw-r--r--   0        0        0     3599 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/loader.py
+-rw-r--r--   0        0        0     2321 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/proxy_auxiliary.py
+-rw-r--r--   0        0        0     6606 2023-05-26 11:45:04.553378 pykiso-0.22.1/src/pykiso/lib/robot_framework/record_auxiliary.py
+-rw-r--r--   0        0        0     6840 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/lib/robot_framework/uds_auxiliary.py
+-rw-r--r--   0        0        0     7770 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/logging_initializer.py
+-rw-r--r--   0        0        0    11744 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/message.py
+-rw-r--r--   0        0        0      410 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/test_coordinator/__init__.py
+-rw-r--r--   0        0        0    12735 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/test_coordinator/test_case.py
+-rw-r--r--   0        0        0    16086 2023-05-26 11:45:04.554378 pykiso-0.22.1/src/pykiso/test_coordinator/test_execution.py
+-rw-r--r--   0        0        0     5480 2023-05-26 11:45:04.555378 pykiso-0.22.1/src/pykiso/test_coordinator/test_message_handler.py
+-rw-r--r--   0        0        0    16859 2023-05-26 11:45:04.555378 pykiso-0.22.1/src/pykiso/test_coordinator/test_suite.py
+-rw-r--r--   0        0        0      515 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/__init__.py
+-rw-r--r--   0        0        0    17429 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/assert_step_report.py
+-rw-r--r--   0        0        0     8391 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/multi_result.py
+-rw-r--r--   0        0        0     1971 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/templates/report_template.css
+-rw-r--r--   0        0        0     5812 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/templates/report_template.html.j2
+-rw-r--r--   0        0        0     1624 2023-05-26 11:45:04.556378 pykiso-0.22.1/src/pykiso/test_result/templates/report_template_script.js
+-rw-r--r--   0        0        0     9917 2023-05-26 11:45:04.640376 pykiso-0.22.1/src/pykiso/test_result/text_result.py
+-rw-r--r--   0        0        0     5663 2023-05-26 11:45:04.640376 pykiso-0.22.1/src/pykiso/test_result/xml_result.py
+-rw-r--r--   0        0        0      410 2023-05-26 11:45:04.640376 pykiso-0.22.1/src/pykiso/test_setup/__init__.py
+-rw-r--r--   0        0        0     9772 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/test_setup/config_registry.py
+-rw-r--r--   0        0        0    14160 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/test_setup/dynamic_loader.py
+-rw-r--r--   0        0        0      410 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/__init__.py
+-rw-r--r--   0        0        0     5577 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/cli.py
+-rw-r--r--   0        0        0     3114 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2
+-rw-r--r--   0        0        0    11816 2023-05-26 11:45:04.641376 pykiso-0.22.1/src/pykiso/tool/show_tag.py
+-rw-r--r--   0        0        0      410 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/__init__.py
+-rw-r--r--   0        0        0    12414 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/api.py
+-rw-r--r--   0        0        0     7728 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/cli.py
+-rw-r--r--   0        0        0     5195 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/console.py
+-rw-r--r--   0        0        0     8545 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/containers.py
+-rw-r--r--   0        0        0     5075 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/extraction.py
+-rw-r--r--   0        0        0    12851 2023-05-26 11:45:04.642376 pykiso-0.22.1/src/pykiso/tool/testrail/testrail.py
+-rw-r--r--   0        0        0     1794 2023-05-26 11:45:04.643376 pykiso-0.22.1/src/pykiso/types.py
+-rw-r--r--   0        0        0     9371 1970-01-01 00:00:00.000000 pykiso-0.22.1/setup.py
+-rw-r--r--   0        0        0     9260 1970-01-01 00:00:00.000000 pykiso-0.22.1/PKG-INFO
```

### Comparing `pykiso-0.22.0/LICENSE` & `pykiso-0.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/README.md` & `pykiso-0.22.1/README.md`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/pyproject.toml` & `pykiso-0.22.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykiso"
-version = "0.22.0"
+version = "0.22.1"
 description = "Embedded integration testing framework."
 authors = ["Sebastian Fischer <sebastian.fischer@de.bosch.com>"]
 license = "Eclipse Public License - v 2.0"
 readme = "README.md"
 homepage = "https://pypi.org/project/pykiso/"
 repository = "https://github.com/eclipse/kiso-testing"
 documentation = "https://kiso-testing.readthedocs.io/en/latest/"
```

### Comparing `pykiso-0.22.0/src/pykiso/__init__.py` & `pykiso-0.22.1/src/pykiso/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/__main__.py` & `pykiso-0.22.1/src/pykiso/__main__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/auxiliary.py` & `pykiso-0.22.1/src/pykiso/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/cli.py` & `pykiso-0.22.1/src/pykiso/cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/config_parser.py` & `pykiso-0.22.1/src/pykiso/config_parser.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/connector.py` & `pykiso-0.22.1/src/pykiso/connector.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/exceptions.py` & `pykiso-0.22.1/src/pykiso/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/global_config.py` & `pykiso-0.22.1/src/pykiso/global_config.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/interfaces/dt_auxiliary.py` & `pykiso-0.22.1/src/pykiso/interfaces/dt_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/interfaces/mp_auxiliary.py` & `pykiso-0.22.1/src/pykiso/interfaces/mp_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/interfaces/simple_auxiliary.py` & `pykiso-0.22.1/src/pykiso/interfaces/simple_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/interfaces/thread_auxiliary.py` & `pykiso-0.22.1/src/pykiso/interfaces/thread_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/acroname_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/acroname_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/communication_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/communication_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/dut_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/dut_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/instrument_control_cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_instruments.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/instrument_control_auxiliary/lib_scpi_commands.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/mp_proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/proxy_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/record_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/record_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/response_templates.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/scenario.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulated_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/simulated_auxiliary/simulation.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/odx_parser.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_base_auxiliary.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         tp_layer: dict = None,
         uds_layer: dict = None,
         **kwargs,
     ):
         """Initialize attributes.
 
         :param com: communication channel connector.
-        :param config_ini_path: UDS parameter file.
+        :param config_ini_path: unused. Legacy UDS parameter file.
         :param odx_file_path: ecu diagnostic definition file.
         :param request_id: optional CAN ID used for sending messages.
         :param response_id: optional CAN ID used for receiving messages.
         """
         super().__init__(
             is_proxy_capable=True, tx_task_on=False, rx_task_on=True, **kwargs
         )
```

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_callback.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_exceptions.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_request.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_response.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/common/uds_utils.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/uds_auxiliary.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
         timeout_in_s: float = 6,
         response_required: bool = True,
     ) -> Union[UdsResponse, bool]:
         """Send a UDS diagnostic request to the target ECU and check response.
 
         :param msg_to_send: can uds raw bytes to be sent
         :param timeout_in_s: not used, actual timeout in seconds for the response can be
-            configured with the P2_CAN_Client parameter in the config.ini file
-            (default value is 5s)
+            configured with the uds_aux.config.uds_layer.p2_can_client parameter
+            inside the yaml config file. (default value is 5s)
         :param response_required: Wait for a response if True
 
         :raise ResponseNotReceivedError: raised when no answer has been received
         :raise Exception: raised when the raw message could not be send properly
 
         :return: the raw uds response's bytes, or True if a response is
             not expected and the command is properly sent otherwise
```

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/udsaux/uds_server_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/auxiliaries/ykush_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/auxiliaries/ykush_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_example.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_example.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_fdx_lauterbach.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_fdx_lauterbach.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_flasher_example.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_flasher_example.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_mp_proxy.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_mp_proxy.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_pcan_can.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_pcan_can.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,42 +400,42 @@
                 result_trace = Path(self.trace_path / self.trace_name)
                 list_of_traces[0] = list_of_traces[0].rename(result_trace)
 
             # End of the trace header
             first_message_line = 33
 
             # Get start time of the first trc file
-            with open(list_of_traces[0], "r") as trc:
+            with list_of_traces[0].open("r") as trc:
                 data = trc.read().splitlines(True)
 
                 first_trc_start_time = CCPCanCan._get_trace_start_time(
                     data, first_message_line
                 )
                 message_idx = len(data[first_message_line:])
 
             list_of_traces.pop(0)
 
             # Append all trace files
             for file in list_of_traces:
-                with open(file, "r") as trc:
+                with file.open("r") as trc:
                     data = trc.read().splitlines(True)
 
                     # Get offset between current and first trc file
                     trc_start_time = CCPCanCan._get_trace_start_time(
                         data, first_message_line
                     )
                     offset = trc_start_time - first_trc_start_time
 
                     # Fix message number and time offset inconstistancies
                     corrected_data = CCPCanCan._fix_merge_inconsistencies(
                         data[first_message_line:], offset, message_idx
                     )
                     message_idx += len(data[first_message_line:])
 
-                with open(result_trace, "a") as merged_trc:
+                with result_trace.open("a") as merged_trc:
                     merged_trc.writelines(corrected_data)
                 os.remove(file)
 
         except IndexError:
             log.internal_warning("No trace to merge")
 
     @staticmethod
```

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_process.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_process.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_proxy.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_proxy.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_raw_loopback.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_raw_loopback.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_rtt_segger.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_rtt_segger.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_serial.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_serial.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/cc_socket_can.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_socket_can/socketcan_to_trc.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_tcp_ip.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_tcp_ip.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_uart.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_uart.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_udp.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_udp.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_udp_server.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_udp_server.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_usb.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_usb.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_vector_can.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_vector_can.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/cc_visa.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/cc_visa.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/flash_jlink.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/flash_jlink.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/connectors/flash_lauterbach.py` & `pykiso-0.22.1/src/pykiso/lib/connectors/flash_lauterbach.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/__init__.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/acroname_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/acroname_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/aux_interface.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/aux_interface.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/communication_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/communication_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/dut_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/dut_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/instrument_control_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/loader.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/loader.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/proxy_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/proxy_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/record_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/record_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/lib/robot_framework/uds_auxiliary.py` & `pykiso-0.22.1/src/pykiso/lib/robot_framework/uds_auxiliary.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/logging_initializer.py` & `pykiso-0.22.1/src/pykiso/logging_initializer.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/message.py` & `pykiso-0.22.1/src/pykiso/message.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_coordinator/test_case.py` & `pykiso-0.22.1/src/pykiso/test_coordinator/test_case.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_coordinator/test_execution.py` & `pykiso-0.22.1/src/pykiso/test_coordinator/test_execution.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_coordinator/test_message_handler.py` & `pykiso-0.22.1/src/pykiso/test_coordinator/test_message_handler.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_coordinator/test_suite.py` & `pykiso-0.22.1/src/pykiso/test_coordinator/test_suite.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_result/__init__.py` & `pykiso-0.22.1/src/pykiso/test_result/__init__.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_result/assert_step_report.py` & `pykiso-0.22.1/src/pykiso/test_result/assert_step_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,15 @@
     # Create the current test step storage
     if not ALL_STEP_REPORT[test_class_name]["test_list"].get(test_name):
         test_method = getattr(test, test_name, None)
         test_description = test_method.__doc__ or ""
         ALL_STEP_REPORT[test_class_name]["test_list"][test_name] = {
             "description": test_description,
             "steps": [],
+            "unexpected_errors": [],
         }
 
 
 def _add_step(
     test_class_name: str,
     test_name: str,
     message: str,
@@ -384,21 +385,24 @@
 
     :return: the date string
     """
     dt = datetime.fromtimestamp(timestamp)
     return dt.strftime("%d/%m/%y %H:%M:%S")
 
 
-def is_test_success(test: List) -> bool:
+def is_test_success(test: dict) -> bool:
     """Check if test was successful.
 
     :param tests: test
-    :return: True if each step in a test was successful else False
+    :return: True if each step in a test was successful and no unexpected error
+        was raised else False
     """
-    return all([step["succeed"] for step in test])
+    return all([step["succeed"] for step in test["steps"]]) and not test.get(
+        "unexpected_errors"
+    )
 
 
 jinja_template_functions = {
     "is_test_success": is_test_success,
 }
 
 
@@ -414,15 +418,14 @@
     global ALL_STEP_REPORT, SCRIPT_PATH, REPORT_TEMPLATE
     test_result.stream.writeln("Generating HTML reports...")
 
     succeeded_tests = test_result.successes + test_result.expectedFailures
     failed_test = (
         test_result.failures + test_result.errors + test_result.unexpectedSuccesses
     )
-
     # Update info for each test
     for test_case in succeeded_tests + failed_test:
         if isinstance(test_case, (TestCase, TestInfo)):
             # Case of success
             test_info = test_case
         elif isinstance(test_case, tuple) and isinstance(
             test_case[0], (TestCase, TestInfo)
@@ -431,34 +434,41 @@
             test_info = test_case[0]
 
         if isinstance(test_info, _SubTest):
             class_name = test_info.test_case.__class__.__name__
             start_time = _parse_timestamp(test_info.test_case.start_time)
             stop_time = _parse_timestamp(test_info.test_case.stop_time)
             elapsed_time = test_info.test_case.elapsed_time
+            test_method_name = test_info.test_case._testMethodName
         elif isinstance(test_info, TestCase):
             class_name = test_info.__class__.__name__
             start_time = _parse_timestamp(test_info.start_time)
             stop_time = _parse_timestamp(test_info.stop_time)
             elapsed_time = test_info.elapsed_time
+            test_method_name = test_info._testMethodName
         elif isinstance(test_info, TestInfo):
             # test_info is TestInfo
             class_name = test_info.test_name.split(".")[-1]
             start_time = _parse_timestamp(test_info.test_result.start_time)
             stop_time = _parse_timestamp(test_info.test_result.stop_time)
             elapsed_time = test_info.elapsed_time
-
+            test_method_name = test_info.test_id.split(".")[-1]
         # Update test_case
         if class_name in ALL_STEP_REPORT:
             ALL_STEP_REPORT[class_name]["time_result"]["Start Time"] = start_time
             ALL_STEP_REPORT[class_name]["time_result"]["End Time"] = stop_time
             ALL_STEP_REPORT[class_name]["time_result"]["Elapsed Time"] = round(
                 elapsed_time, 2
             )
+            if test_case in test_result.errors:
+                ALL_STEP_REPORT[class_name]["test_list"][test_method_name][
+                    "unexpected_errors"
+                ].append(test_case[1])
 
+                ALL_STEP_REPORT[class_name]["succeed"] = False
     # Render the source template
     render_environment = jinja2.Environment(loader=jinja2.FileSystemLoader(SCRIPT_PATH))
     template = render_environment.get_template(REPORT_TEMPLATE)
     template.globals.update(jinja_template_functions)
     output_text = template.render({"ALL_STEP_REPORT": ALL_STEP_REPORT})
 
     output_file = Path(output_file).resolve()
```

### Comparing `pykiso-0.22.0/src/pykiso/test_result/multi_result.py` & `pykiso-0.22.1/src/pykiso/test_result/multi_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_result/templates/report_template.css` & `pykiso-0.22.1/src/pykiso/test_result/templates/report_template.css`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_result/templates/report_template.html.j2` & `pykiso-0.22.1/src/pykiso/test_result/templates/report_template.html.j2`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 {% for key, value in data.items() -%}
                     <u>{{key}}</u>: {{value}}</br>
                 {%- endfor %}
             {%- endfor %}
             </p>
             {#- For each test (setUp, run, tearDown) -#}
             {% for test_name, test_content in class_content["test_list"].items() %}
-                {% set test_success = is_test_success(test_content["steps"]) -%}
+                {% set test_success = is_test_success(test_content) -%}
                 <details {% if not test_success %}open{% endif %}><summary><h3>{{test_name}}
                 {% if test_success -%}<span style="color:green;">Success</span>
                 {% else %}<span style="color:red;">Fail</span>
                 {%- endif %}</h3></summary>
                 <p>{{test_content["description"] | replace("\n", "<br/>\n") }}</p>
                 <table>
                     <thead>
@@ -80,14 +80,21 @@
                                         {%- endif %}
                                     </td>
                                 {%- endfor %}
                             </tr>
                         {%- endfor %}
                     </tbody>
                 </table>
+                {% if test_content.get("unexpected_errors") -%}
+                    <b style='color:red;'><strong>Unexpected errors happened :</strong> <br></b>
+                        {% for error in test_content.get("unexpected_errors") -%}
+                            <pre>{{error}}</pre>
+                        {%- endfor %}
+
+                {%- endif %}
                 </details>
             {%- endfor %}
         </div>
     {%- endfor %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -10,18 +10,21 @@
 \n") }}
 **** Date, Time, Software versions: ****
 {# Add additional information from header key -#} {% for data in [class_content
 ["time_result"], class_content["header"]] -%} {% for key, value in data.items()
 -%} {{key}}: {{value}} {%- endfor %} {%- endfor %}
 {#- For each test (setUp, run, tearDown) -#} {% for test_name, test_content in
 class_content["test_list"].items() %} {% set test_success = is_test_success
-(test_content["steps"]) -%}
+(test_content) -%}
 % if not test_success %}open{% endif %}>
 **** {{test_name}} {% if test_success -%}Success {% else %}Fail {%- endif %}
 ****
 {{test_content["description"] | replace("\n", "
 \n") }}
 Step           {{column_name}}
 {{loop.index}}
- {%- endfor %}
+{% if test_content.get("unexpected_errors") -%} Unexpected errors happened :
+ {% for error in test_content.get("unexpected_errors") -%}
+{{error}}
+{%- endfor %} {%- endif %}  {%- endfor %}
 {%- endfor %}
```

### Comparing `pykiso-0.22.0/src/pykiso/test_result/templates/report_template_script.js` & `pykiso-0.22.1/src/pykiso/test_result/templates/report_template_script.js`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_result/text_result.py` & `pykiso-0.22.1/src/pykiso/test_result/text_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_result/xml_result.py` & `pykiso-0.22.1/src/pykiso/test_result/xml_result.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_setup/config_registry.py` & `pykiso-0.22.1/src/pykiso/test_setup/config_registry.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/test_setup/dynamic_loader.py` & `pykiso-0.22.1/src/pykiso/test_setup/dynamic_loader.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/cli.py` & `pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/cli.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2` & `pykiso-0.22.1/src/pykiso/tool/pykiso_to_pytest/templates/conftest_template.jinja2`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/tool/show_tag.py` & `pykiso-0.22.1/src/pykiso/tool/show_tag.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/tool/testrail/api.py` & `pykiso-0.22.1/src/pykiso/tool/testrail/api.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/tool/testrail/cli.py` & `pykiso-0.22.1/src/pykiso/tool/testrail/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 :synopsis: CLI entry-point for TestRail helper tool
 
 .. currentmodule:: cli
 
 """
 import getpass
+import sys
 
 import click
 
 from .console import (
     print_cases,
     print_milestones,
     print_projects,
@@ -241,19 +242,19 @@
 def cli_upload(
     ctx,
     run_name: str,
     project: str,
     suite: str,
     milestone: str,
     results: str,
-    attr: str,
+    tag: str,
     custom_field: str,
 ) -> None:
     """Upload all test case results on TestRail."""
-    JunitReport.set_id_tag(attr)
+    JunitReport.set_id_tag(tag)
 
     # get all available cases from the given project
     project_id, cases = enumerate_all_cases(
         base_url=ctx.obj["URL"],
         user=ctx.obj["USER"],
         password=ctx.obj["PASSWORD"],
         project_name=project,
@@ -273,16 +274,20 @@
         base_url=ctx.obj["URL"],
         user=ctx.obj["USER"],
         password=ctx.obj["PASSWORD"],
         project_name=project,
         suite_name=suite,
     )
     # extract the ids from each given JUNIT report and finally get the
-    # couple (TestRail id, req id, state)
+    # tuple (TestRail id, req id, state)
     case_results = extract_test_results(results=results, cases=cases)
+    if len(case_results) == 0:
+        print("Could not match any JUnit result to a Testrail test case, exiting.")
+        sys.exit(1)
+
     case_ids = [rail_id for rail_ids, _, _ in case_results for rail_id in rail_ids]
     # Create a brand new run on TestRail and associate the case ids
     run_id = create_new_run(
         base_url=ctx.obj["URL"],
         user=ctx.obj["USER"],
         password=ctx.obj["PASSWORD"],
         project_id=project_id,
```

### Comparing `pykiso-0.22.0/src/pykiso/tool/testrail/console.py` & `pykiso-0.22.1/src/pykiso/tool/testrail/console.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/tool/testrail/containers.py` & `pykiso-0.22.1/src/pykiso/tool/testrail/containers.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/tool/testrail/extraction.py` & `pykiso-0.22.1/src/pykiso/tool/testrail/extraction.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/tool/testrail/testrail.py` & `pykiso-0.22.1/src/pykiso/tool/testrail/testrail.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/src/pykiso/types.py` & `pykiso-0.22.1/src/pykiso/types.py`

 * *Files identical despite different names*

### Comparing `pykiso-0.22.0/setup.py` & `pykiso-0.22.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
                      'pykiso = pykiso.cli:main',
                      'pykiso-tags = pykiso.tool.show_tag:main',
                      'pykitest = pykiso.tool.pykiso_to_pytest.cli:main',
                      'testrail = pykiso.tool.testrail.cli:cli_testrail']}
 
 setup_kwargs = {
     'name': 'pykiso',
-    'version': '0.22.0',
+    'version': '0.22.1',
     'description': 'Embedded integration testing framework.',
     'long_description': '[![License](https://img.shields.io/badge/Licence-Eclipse%20Public%20License%202.0-lightgrey)](https://opensource.org/licenses/EPL-2.0)\n[![Platforms](https://img.shields.io/badge/Platforms-win64%20linux64%20osx64-lightgrey)]()\n[![Supported python version](https://img.shields.io/pypi/pyversions/pykiso)]()\n[![Build status](https://img.shields.io/jenkins/build?jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![Documentation Status](https://readthedocs.org/projects/kiso-testing/badge/?version=latest)](https://kiso-testing.readthedocs.io/en/latest/?badge=latest)\n[![Test results](https://img.shields.io/jenkins/tests?compact_message&failed_label=failed&jobUrl=https%3A%2F%2Fci.eclipse.org%2Fkiso-testing%2Fjob%2Fkiso-testing%2Fjob%2Fmaster%2F&passed_label=passed&skipped_label=skipped)](https://ci.eclipse.org/kiso-testing/job/kiso-testing/job/master/)\n[![codecov](https://codecov.io/gh/eclipse/kiso-testing/branch/master/graph/badge.svg?token=IBKQ700ABS)](https://codecov.io/gh/eclipse/kiso-testing)\n[![CodeFactor](https://www.codefactor.io/repository/github/eclipse/kiso-testing/badge)](https://www.codefactor.io/repository/github/eclipse/kiso-testing)\n[![Last commit](https://img.shields.io/github/last-commit/eclipse/kiso-testing)]()\n[![Commits since latest version](https://img.shields.io/github/commits-since/eclipse/kiso-testing/latest/master)]()\n\n# PyKiso\n\n![Optional Text](./docs/images/pykiso_logo.png)\n\n## Introduction ##\n\n**pykiso** is an integration test framework. With it, it is possible to write\n* Whitebox integration tests directly on my target device\n* Graybox integration tests to make sure the communication-link with my target device is working as expected\n* Blackbox integration tests to make sure my external device interfaces are working as expected\n\nThe project will contain:\n* The core python framework (this repository)\n* Framework plugins that are generic enough to be integrated as "native" (this repository)\n* Additional "testApps" for different targets platforms (e.g. stm32, ...) or languages (C, C++, ...) . It could be pure SW or also HW (other repositories)\n\n## Link to Eclipse Project\nhttps://projects.eclipse.org/projects/iot.kiso-testing\n\n## Requirements ##\n\n* Python 3.7+\n* pip/poetry (used to get the rest of the requirements)\n\n## Install ##\n\n```bash\npip install pykiso # Core framework\npip install pykiso[plugins] # For installing all plugins\npip install pykiso[all] # For installing all what we have to offer\n```\n\n[Poetry](https://python-poetry.org/) is more appropriate for developers as it automatically creates virtual environments.\n\n```bash\ncd kiso-testing\npoetry install --all-extras\npoetry shell\n```\n\n### Pre-Commit\n\nTo improve code-quality, a configuration of [pre-commit](https://pre-commit.com/) hooks are available.\nThe following pre-commit hooks are used:\n\n- black\n- flake8\n- isort\n- trailing-whitespace\n- end-of-file-fixer\n- check-docstring-first\n- check-json\n- check-added-large-files\n- check-yaml\n- debug-statements\n\nIf you don\'t have pre-commit installed, you can get it using pip:\n\n```bash\npip install pre-commit\n```\n\nStart using the hooks with\n\n```bash\npre-commit install\n```\n\n## Commit message convention\n\nCommits are sorted into multiple categories based on keywords that can occur at any position as part of the commit message.\n[Category] Keywords\n* [BREAKING CHANGES] BREAKING CHANGE\n* [Features] feat:\n* [Fixes] fix:\n* [Docs] docs:\n* [Styles] style:\n* [Refactors] refactor!:\n* [Performances] perf:\n* [Tests] test:\n* [Build] build:\n* [Ci] ci:\nEach commit is considered only once according to the order of the categories listed above. Merge commits are ignored.\n\nThe tool commitizen can help you to create commits which follows these standards.\n```bash\n# if not yet installed:\npip install -U commitizen==2.20.4\n# helps you to create a commit:\ncz commit\n# or use equivalent short variant:\ncz c\n```\n\n## Generate Changelog\n\nAfter you installed the dev dependencies from the pipfile you are able to\nautogenerate the Changelog.\n\n```bash\ninvoke changelog\n```\n\n## Usage ##\n\nOnce installed the application is bound to `pykiso`, it can be called with the following arguments:\n\n```bash\nUsage: pykiso [OPTIONS]\n\n  Embedded Integration Test Framework - CLI Entry Point.\n\n  TAG Filters: any additional option to be passed to the test as tag through\n  the pykiso call. Multiple values must be separated with a comma.\n\n  For example: pykiso -c your_config.yaml --branch-level dev,master --variant\n  delta\n\nOptions:\n  -c, --test-configuration-file FILE\n                                  path to the test configuration file (in YAML\n                                  format)  [required]\n  -l, --log-path PATH             path to log-file or folder. If not set will\n                                  log to STDOUT\n  --log-level [DEBUG|INFO|WARNING|ERROR]\n                                  set the verbosity of the logging\n  --junit                         enables the generation of a junit report\n  --text                          default, test results are only displayed in\n                                  the console\n  --step-report PATH              generate the step report at the specified\n                                  path\n  --failfast                      stop the test run on the first error or\n                                  failure\n  -v, --verbose                   activate the internal framework logs\n  -p, --pattern TEXT              test filter pattern, e.g. \'test_suite_1.py\'\n                                  or \'test_*.py\'. Or even more granularly\n                                  \'test_suite_1.py::test_class::test_name\'\n  --version                       Show the version and exit.\n  -h, --help                      Show this message and exit.\n```\n\nSuitable config files are available in the `examples` folder.\n\n### Demo using example config ##\n\n```bash\ninvoke run\n```\n\n### Running the Tests ##\n\n```bash\ninvoke test\n```\n\nor\n\n```bash\npytest\n```\n',
     'author': 'Sebastian Fischer',
     'author_email': 'sebastian.fischer@de.bosch.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/pykiso/',
```

### Comparing `pykiso-0.22.0/PKG-INFO` & `pykiso-0.22.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykiso
-Version: 0.22.0
+Version: 0.22.1
 Summary: Embedded integration testing framework.
 Home-page: https://pypi.org/project/pykiso/
 License: Eclipse Public License - v 2.0
 Keywords: testing,integration testing,framework,testing framework
 Author: Sebastian Fischer
 Author-email: sebastian.fischer@de.bosch.com
 Requires-Python: >=3.7,<4.0
```

