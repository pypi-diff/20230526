# Comparing `tmp/polyglot_piranha-0.3.3.tar.gz` & `tmp/polyglot_piranha-0.3.4.tar.gz`

## Comparing `polyglot_piranha-0.3.3.tar` & `polyglot_piranha-0.3.4.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.3/Cargo.toml
--rw-r--r--   0     1001      123    35472 2023-04-24 21:40:36.000000 polyglot_piranha-0.3.3/Cargo.lock
--rw-r--r--   0     1001      123    11359 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/LICENSE
--rw-r--r--   0     1001      123     3091 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/README.md
--rw-r--r--   0     1001      123     1373 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
--rw-r--r--   0     1001      123      994 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
--rw-r--r--   0     1001      123     5517 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
--rw-r--r--   0     1001      123     5621 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
--rw-r--r--   0     1001      123    66915 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
--rw-r--r--   0     1001      123    21518 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
--rw-r--r--   0     1001      123     5106 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
--rw-r--r--   0     1001      123      377 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
--rw-r--r--   0     1001      123     3615 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
--rw-r--r--   0     1001      123     5039 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
--rw-r--r--   0     1001      123     2584 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
--rw-r--r--   0     1001      123     2605 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
--rw-r--r--   0     1001      123      550 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
--rw-r--r--   0     1001      123     2456 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
--rw-r--r--   0     1001      123    13106 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
--rw-r--r--   0     1001      123     5875 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
--rw-r--r--   0     1001      123    85120 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
--rw-r--r--   0     1001      123    55188 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
--rw-r--r--   0     1001      123    48474 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
--rw-r--r--   0     1001      123     2304 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
--rw-r--r--   0     1001      123    33367 2023-04-24 21:33:44.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
--rw-r--r--   0     1001      123     6780 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
--rw-r--r--   0     1001      123     3480 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
--rw-r--r--   0     1001      123     8540 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
--rw-r--r--   0     1001      123     4153 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
--rw-r--r--   0     1001      123     4326 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
--rw-r--r--   0     1001      123     2555 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
--rw-r--r--   0     1001      123     1490 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
--rw-r--r--   0     1001      123     2091 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
--rw-r--r--   0     1001      123     2194 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
--rw-r--r--   0     1001      123     1550 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
--rw-r--r--   0     1001      123     1618 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
--rw-r--r--   0     1001      123     1573 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
--rw-r--r--   0     1001      123       75 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
--rw-r--r--   0     1001      123      109 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
--rw-r--r--   0     1001      123      175 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
--rw-r--r--   0     1001      123      103 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
--rw-r--r--   0     1001      123      154 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
--rw-r--r--   0     1001      123      155 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
--rw-r--r--   0     1001      123      160 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
--rw-r--r--   0     1001      123      122 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
--rw-r--r--   0     1001      123      229 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
--rw-r--r--   0     1001      123       97 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
--rw-r--r--   0     1001      123      202 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
--rw-r--r--   0     1001      123      213 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
--rw-r--r--   0     1001      123      216 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
--rw-r--r--   0     1001      123      361 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
--rw-r--r--   0     1001      123      525 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
--rw-r--r--   0     1001      123      526 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
--rw-r--r--   0     1001      123      488 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
--rw-r--r--   0     1001      123      489 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
--rw-r--r--   0     1001      123      526 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
--rw-r--r--   0     1001      123      704 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
--rw-r--r--   0     1001      123     1332 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
--rw-r--r--   0     1001      123      192 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
--rw-r--r--   0     1001      123      739 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
--rw-r--r--   0     1001      123      652 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
--rw-r--r--   0     1001      123     1896 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
--rw-r--r--   0     1001      123      844 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return.json
--rw-r--r--   0     1001      123     1776 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
--rw-r--r--   0     1001      123     1932 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
--rw-r--r--   0     1001      123     4525 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
--rw-r--r--   0     1001      123      251 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
--rw-r--r--   0     1001      123      246 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
--rw-r--r--   0     1001      123      142 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
--rw-r--r--   0     1001      123     1637 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
--rw-r--r--   0     1001      123     1304 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
--rw-r--r--   0     1001      123     1304 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
--rw-r--r--   0     1001      123     1107 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
--rw-r--r--   0     1001      123     2565 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/javascript/src/config_checker.js
--rw-r--r--   0     1001      123     4304 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/javascript/src/piranha.js
--rw-r--r--   0     1001      123    27988 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/javascript/src/refactor.js
--rw-r--r--   0     1001      123     1445 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/javascript/src/source_checker.js
--rw-r--r--   0     1001      123      646 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
--rw-r--r--   0     1001      123     1064 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/README.txt
--rw-r--r--   0     1001      123    26229 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
--rw-r--r--   0     1001      123        0 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
--rw-r--r--   0     1001      123      793 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/pyproject.toml
--rw-r--r--   0     1001      123     2043 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/go/edges.toml
--rw-r--r--   0     1001      123    11027 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/go/rules.toml
--rw-r--r--   0     1001      123     1460 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/go/scope_config.toml
--rwxr-xr-x   0     1001      123     2241 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/java/edges.toml
--rwxr-xr-x   0     1001      123    17618 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/java/rules.toml
--rwxr-xr-x   0     1001      123     3582 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/java/scope_config.toml
--rwxr-xr-x   0     1001      123     2251 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/kt/edges.toml
--rwxr-xr-x   0     1001      123    19122 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/kt/rules.toml
--rwxr-xr-x   0     1001      123     2139 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/kt/scope_config.toml
--rw-r--r--   0     1001      123     1133 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/swift/edges.toml
--rw-r--r--   0     1001      123    10134 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/swift/rules.toml
--rw-r--r--   0     1001      123     1369 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/cleanup_rules/swift/scope_config.toml
--rw-r--r--   0     1001      123     7317 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/lib.rs
--rw-r--r--   0     1001      123     1679 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/main.rs
--rw-r--r--   0     1001      123     5799 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/constraint.rs
--rw-r--r--   0     1001      123     3178 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/default_configs.rs
--rw-r--r--   0     1001      123     4915 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/edit.rs
--rw-r--r--   0     1001      123     7047 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/language.rs
--rw-r--r--   0     1001      123    11140 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/matches.rs
--rw-r--r--   0     1001      123      928 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/mod.rs
--rw-r--r--   0     1001      123     1987 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/outgoing_edges.rs
--rw-r--r--   0     1001      123    14202 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/piranha_arguments.rs
--rw-r--r--   0     1001      123     2091 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/piranha_output.rs
--rw-r--r--   0     1001      123     7916 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/rule.rs
--rw-r--r--   0     1001      123     6286 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/rule_graph.rs
--rw-r--r--   0     1001      123     5931 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/rule_store.rs
--rw-r--r--   0     1001      123     3329 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/scopes.rs
--rw-r--r--   0     1001      123    14473 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/source_code_unit.rs
--rw-r--r--   0     1001      123     1586 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/unit_tests/piranha_arguments_test.rs
--rw-r--r--   0     1001      123     8340 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/unit_tests/rule_test.rs
--rw-r--r--   0     1001      123     6061 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/unit_tests/scopes_test.rs
--rw-r--r--   0     1001      123     6996 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/models/unit_tests/source_code_unit_test.rs
--rw-r--r--   0     1001      123     8222 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/mod.rs
--rw-r--r--   0     1001      123     1647 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_go.rs
--rw-r--r--   0     1001      123    12255 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_java.rs
--rw-r--r--   0     1001      123     1862 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_kt.rs
--rw-r--r--   0     1001      123     2423 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_python.rs
--rw-r--r--   0     1001      123     1833 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_swift.rs
--rw-r--r--   0     1001      123      770 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_thrift.rs
--rw-r--r--   0     1001      123     1138 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_ts.rs
--rw-r--r--   0     1001      123     1281 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/tests/test_piranha_tsx.rs
--rw-r--r--   0     1001      123     5476 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/utilities/mod.rs
--rw-r--r--   0     1001      123    12743 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/utilities/tree_sitter_utilities.rs
--rw-r--r--   0     1001      123     3681 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/utilities/unit_tests/tree_sitter_utilities_test.rs
--rw-r--r--   0     1001      123     2237 2023-04-24 21:33:45.000000 polyglot_piranha-0.3.3/src/utilities/unit_tests/utilities_test.rs
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.4/Cargo.toml
+-rw-r--r--   0     1001      123    35670 2023-05-26 12:53:30.000000 polyglot_piranha-0.3.4/Cargo.lock
+-rw-r--r--   0     1001      123    11359 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/LICENSE
+-rw-r--r--   0     1001      123     3091 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/README.md
+-rw-r--r--   0     1001      123     1373 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java
+-rw-r--r--   0     1001      123      994 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java
+-rw-r--r--   0     1001      123     5517 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java
+-rw-r--r--   0     1001      123     5621 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java
+-rw-r--r--   0     1001      123    66915 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java
+-rw-r--r--   0     1001      123    21518 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java
+-rw-r--r--   0     1001      123     5106 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java
+-rw-r--r--   0     1001      123      377 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaConfigurationException.java
+-rw-r--r--   0     1001      123     3615 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java
+-rw-r--r--   0     1001      123     5039 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java
+-rw-r--r--   0     1001      123     2584 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java
+-rw-r--r--   0     1001      123     2605 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java
+-rw-r--r--   0     1001      123      550 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java
+-rw-r--r--   0     1001      123     2456 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java
+-rw-r--r--   0     1001      123    13106 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java
+-rw-r--r--   0     1001      123     5875 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java
+-rw-r--r--   0     1001      123    85120 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java
+-rw-r--r--   0     1001      123    55188 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java
+-rw-r--r--   0     1001      123    48474 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java
+-rw-r--r--   0     1001      123     2304 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java
+-rw-r--r--   0     1001      123    33367 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java
+-rw-r--r--   0     1001      123     6780 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java
+-rw-r--r--   0     1001      123     3480 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java
+-rw-r--r--   0     1001      123     8540 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java
+-rw-r--r--   0     1001      123     4153 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java
+-rw-r--r--   0     1001      123     4326 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java
+-rw-r--r--   0     1001      123     2555 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java
+-rw-r--r--   0     1001      123     1490 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java
+-rw-r--r--   0     1001      123     2091 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java
+-rw-r--r--   0     1001      123     2194 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java
+-rw-r--r--   0     1001      123     1550 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java
+-rw-r--r--   0     1001      123     1618 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java
+-rw-r--r--   0     1001      123     1573 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java
+-rw-r--r--   0     1001      123       75 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParam.java
+-rw-r--r--   0     1001      123      109 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/BoolParameter.java
+-rw-r--r--   0     1001      123      175 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/OverlappingNameInterface.java
+-rw-r--r--   0     1001      123      103 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/PVal.java
+-rw-r--r--   0     1001      123      154 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/Parameter.java
+-rw-r--r--   0     1001      123      155 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeOtherInterface.java
+-rw-r--r--   0     1001      123      160 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/SomeParamRev.java
+-rw-r--r--   0     1001      123      122 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/mock/StaticMthds.java
+-rw-r--r--   0     1001      123      229 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/piranha.properties
+-rw-r--r--   0     1001      123       97 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid.json
+-rw-r--r--   0     1001      123      202 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_2.json
+-rw-r--r--   0     1001      123      213 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_3.json
+-rw-r--r--   0     1001      123      216 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/invalid/properties_test_invalid_4.json
+-rw-r--r--   0     1001      123      361 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_enum_no_arg.json
+-rw-r--r--   0     1001      123      525 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json
+-rw-r--r--   0     1001      123      526 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json
+-rw-r--r--   0     1001      123      488 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name.json
+-rw-r--r--   0     1001      123      489 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_no_flag_method_name_no_method_chain.json
+-rw-r--r--   0     1001      123      526 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json
+-rw-r--r--   0     1001      123      704 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_argument.json
+-rw-r--r--   0     1001      123     1332 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json
+-rw-r--r--   0     1001      123      192 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_noFlag.json
+-rw-r--r--   0     1001      123      739 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json
+-rw-r--r--   0     1001      123      652 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_receive.json
+-rw-r--r--   0     1001      123     1896 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json
+-rw-r--r--   0     1001      123      844 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return.json
+-rw-r--r--   0     1001      123     1776 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json
+-rw-r--r--   0     1001      123     1932 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json
+-rw-r--r--   0     1001      123     4525 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json
+-rw-r--r--   0     1001      123      251 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_no_match.json
+-rw-r--r--   0     1001      123      246 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_with_enum_wrong_arg.json
+-rw-r--r--   0     1001      123      142 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_without_enum.json
+-rw-r--r--   0     1001      123     1637 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json
+-rw-r--r--   0     1001      123     1304 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java
+-rw-r--r--   0     1001      123     1304 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak
+-rw-r--r--   0     1001      123     1107 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect
+-rw-r--r--   0     1001      123     2565 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/javascript/src/config_checker.js
+-rw-r--r--   0     1001      123     4304 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/javascript/src/piranha.js
+-rw-r--r--   0     1001      123    27988 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/javascript/src/refactor.js
+-rw-r--r--   0     1001      123     1445 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/javascript/src/source_checker.js
+-rw-r--r--   0     1001      123      646 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt
+-rw-r--r--   0     1001      123     1064 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/README.txt
+-rw-r--r--   0     1001      123    26229 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp
+-rw-r--r--   0     1001      123        0 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.exports
+-rw-r--r--   0     1001      123      793 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/pyproject.toml
+-rw-r--r--   0     1001      123     2043 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/go/edges.toml
+-rw-r--r--   0     1001      123    11039 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/go/rules.toml
+-rw-r--r--   0     1001      123     1466 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/go/scope_config.toml
+-rwxr-xr-x   0     1001      123     2241 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/java/edges.toml
+-rwxr-xr-x   0     1001      123    17674 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/java/rules.toml
+-rwxr-xr-x   0     1001      123     3580 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/java/scope_config.toml
+-rwxr-xr-x   0     1001      123     2251 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/kt/edges.toml
+-rwxr-xr-x   0     1001      123    19368 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/kt/rules.toml
+-rwxr-xr-x   0     1001      123     2142 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/kt/scope_config.toml
+-rw-r--r--   0     1001      123     2316 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/swift/edges.toml
+-rw-r--r--   0     1001      123    27137 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/swift/rules.toml
+-rw-r--r--   0     1001      123     1684 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/cleanup_rules/swift/scope_config.toml
+-rw-r--r--   0     1001      123     7391 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/lib.rs
+-rw-r--r--   0     1001      123     1679 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/main.rs
+-rw-r--r--   0     1001      123     3583 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/default_configs.rs
+-rw-r--r--   0     1001      123     4915 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/edit.rs
+-rw-r--r--   0     1001      123    10594 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/filter.rs
+-rw-r--r--   0     1001      123     7097 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/language.rs
+-rw-r--r--   0     1001      123    11128 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/matches.rs
+-rw-r--r--   0     1001      123      924 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/mod.rs
+-rw-r--r--   0     1001      123     1987 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/outgoing_edges.rs
+-rw-r--r--   0     1001      123    14245 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/piranha_arguments.rs
+-rw-r--r--   0     1001      123     2091 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/piranha_output.rs
+-rw-r--r--   0     1001      123     7801 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/rule.rs
+-rw-r--r--   0     1001      123     6286 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/rule_graph.rs
+-rw-r--r--   0     1001      123     6288 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/rule_store.rs
+-rw-r--r--   0     1001      123     3402 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/scopes.rs
+-rw-r--r--   0     1001      123    14473 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/source_code_unit.rs
+-rw-r--r--   0     1001      123     1661 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/unit_tests/piranha_arguments_test.rs
+-rw-r--r--   0     1001      123     8344 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/unit_tests/rule_test.rs
+-rw-r--r--   0     1001      123     6067 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/unit_tests/scopes_test.rs
+-rw-r--r--   0     1001      123    11082 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/models/unit_tests/source_code_unit_test.rs
+-rw-r--r--   0     1001      123     8260 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/mod.rs
+-rw-r--r--   0     1001      123     1647 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_go.rs
+-rw-r--r--   0     1001      123    12953 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_java.rs
+-rw-r--r--   0     1001      123     1862 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_kt.rs
+-rw-r--r--   0     1001      123     2423 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_python.rs
+-rw-r--r--   0     1001      123     3532 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_swift.rs
+-rw-r--r--   0     1001      123      770 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_thrift.rs
+-rw-r--r--   0     1001      123     1138 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_ts.rs
+-rw-r--r--   0     1001      123     1281 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/tests/test_piranha_tsx.rs
+-rw-r--r--   0     1001      123     5629 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/utilities/mod.rs
+-rw-r--r--   0     1001      123    12743 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/utilities/tree_sitter_utilities.rs
+-rw-r--r--   0     1001      123     3681 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/utilities/unit_tests/tree_sitter_utilities_test.rs
+-rw-r--r--   0     1001      123     2237 2023-05-26 12:50:38.000000 polyglot_piranha-0.3.4/src/utilities/unit_tests/utilities_test.rs
+-rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 polyglot_piranha-0.3.4/PKG-INFO
```

### Comparing `polyglot_piranha-0.3.3/Cargo.toml` & `polyglot_piranha-0.3.4/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "Ameya Ketkar <ketkara@uber.com>",
   "Lazaro Clapp <lazaro@uber.com>",
   "Murali Krishna Ramanathan",
   "Uber Technologies Inc.",
 ]
 name = "piranha"
 description = "Polyglot Piranha is a library for performing structural find and replace with deep cleanup."
-version = "0.3.3"
+version = "0.3.4"
 edition = "2021"
 include = ["pyproject.toml", "src/"]
 exclude = ["legacy"]
 license-file = "LICENSE"
 categories = [
   "structural find-replace",
   "find-replace",
@@ -24,14 +24,15 @@
 name = "polyglot_piranha"
 path = "src/main.rs"
 
 [lib]
 name = "polyglot_piranha"
 path = "src/lib.rs"
 crate-type = ["cdylib", "rlib"]
+doctest = false
 
 [build-dependencies]
 cc = "1.0.73"
 
 [dependencies]
 tree-sitter = "0.20.6"
 tree-sitter-traversal = "0.1.2"
@@ -49,24 +50,25 @@
 tempdir = "0.3"
 serde_json = "1.0.82"
 # TODO: Update after https://github.com/fwcd/tree-sitter-kotlin/pull/71 lands
 tree-sitter-kotlin = { git = "https://github.com/ketkarameya/tree-sitter-kotlin.git", rev = "a87ddd003368e068563f1cc478a1b2a3f9d73b60" }
 # TODO: Update after next version is released (https://github.com/tree-sitter/tree-sitter-java/issues/146)
 tree-sitter-java = { git = "https://github.com/tree-sitter/tree-sitter-java.git", rev = "c194ee5e6ede5f26cf4799feead4a8f165dcf14d" }
 # TODO: Update after: https://github.com/alex-pinkus/tree-sitter-swift/issues/278 resolves
-tree-sitter-swift = { git = "https://github.com/satyam1749/tree-sitter-swift.git", rev = "c92496b5273e4d3b094148fee51de371c94729bf" }
+tree-sitter-swift = { git = "https://github.com/satyam1749/tree-sitter-swift.git", rev = "895cd7814488cb32cf73f68a75458b4bc6d50a85" }
 tree-sitter-python = "0.20.2"
 tree-sitter-typescript = "0.20.1"
 # TODO: Update after https://github.com/tree-sitter/tree-sitter-go/pull/103 lands
 tree-sitter-go = { git = "https://github.com/uber/tree-sitter-go.git", rev = "8f807196afab4a1a1256dbf62a011020c6fe7745" }
 tree-sitter-thrift = "0.5.0"
 derive_builder = "0.12.0"
 getset = "0.1.2"
 pyo3 = "0.18.2"
 pyo3-log = "0.8.1"
+glob = "0.3.1"
 
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
 
 
 [dev-dependencies]
```

### Comparing `polyglot_piranha-0.3.3/Cargo.lock` & `polyglot_piranha-0.3.4/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -102,17 +102,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bstr"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d4260bcc2e8fc9df1eac4919a720effeb63a3f0952f5bf4944adfa18897f09"
+checksum = "a246e68bb43f6cd9db24bea052a53e40405417c5fb372e3d1a8a7f770a564ef5"
 dependencies = [
  "memchr",
  "once_cell",
  "regex-automata",
  "serde",
 ]
 
@@ -126,53 +126,53 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.2.4"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "956ac1f6381d8d82ab4684768f89c0ea3afe66925ceadb4eeb3fc452ffc55d62"
+checksum = "93aae7a4192245f70fe75dd9157fc7b4a5bf53e88d30bd4396f7d8f9284d5acc"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.4"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84080e799e54cff944f4b4a4b0e71630b0e0443b25b985175c7dddc1a859b749"
+checksum = "4f423e341edefb78c9caba2d9c7f7687d0e72e89df3ce3394554754393ac3990"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.2.0"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f9644cd56d6b87dbe899ef8b053e331c0637664e9e21a33dfcdc36093f5c5c4"
+checksum = "191d9573962933b4027f932c600cd252ce27a8ad5979418fe78e43c07996f27b"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.17",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
@@ -402,14 +402,20 @@
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "heck"
@@ -467,17 +473,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
@@ -527,23 +533,23 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.4"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -627,23 +633,24 @@
  "redox_syscall",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "piranha"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "assert_cmd",
  "cc",
  "clap",
  "colored",
  "derive_builder",
  "env_logger",
  "getset",
+ "glob",
  "itertools",
  "json",
  "jwalk",
  "log",
  "predicates",
  "pyo3",
  "pyo3-log",
@@ -717,17 +724,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -797,17 +804,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.4.6"
@@ -874,49 +881,49 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.14"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b864d3c18a5785a05953adeed93e2dca37ed30f18e69bba9f30079d51f363f"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -932,27 +939,27 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.160"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 
 [[package]]
 name = "serde_derive"
-version = "1.0.160"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.17",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -960,17 +967,17 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0efd8caf556a6cebd3b285caf480045fcc1ac04f6bd786b09a6f11af30c4fcf4"
+checksum = "93107647184f6027e3b7dcb2e11034cf95ffa1e3a682c67951963ac69c1c007d"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
@@ -992,28 +999,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "45b6ddbb36c5b969c182aec3c4a0bce7df3fbad4b77114706a49aacc80567388"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempdir"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15f2b5fb00ccdf689e0149d1b1b3c03fead81c2b37735d812fa8bddbbf41b6d8"
 dependencies = [
@@ -1034,38 +1041,38 @@
 name = "termtree"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3369f5ac52d5eb6ab48c6b4ffdc8efbcad6b89c765749064ba298f2c68a16a76"
 
 [[package]]
 name = "toml"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b403acf6f2bb0859c93c7f0d967cb4a75a7ac552100f9322faf64dc047669b21"
+checksum = "d6135d499e69981f9ff0ef2167955a5333c35e36f6937d382974566b3d5b94ec"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.8"
+version = "0.19.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
+checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
@@ -1116,15 +1123,15 @@
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-swift"
 version = "0.3.6"
-source = "git+https://github.com/satyam1749/tree-sitter-swift.git?rev=c92496b5273e4d3b094148fee51de371c94729bf#c92496b5273e4d3b094148fee51de371c94729bf"
+source = "git+https://github.com/satyam1749/tree-sitter-swift.git?rev=895cd7814488cb32cf73f68a75458b4bc6d50a85#895cd7814488cb32cf73f68a75458b4bc6d50a85"
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "tree-sitter-thrift"
@@ -1153,17 +1160,17 @@
 dependencies = [
  "cc",
  "tree-sitter",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -1349,13 +1356,13 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.4.1"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
+checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
```

### Comparing `polyglot_piranha-0.3.3/LICENSE` & `polyglot_piranha-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/README.md` & `polyglot_piranha-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/EnumWithClassSymbol.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaRuntimeException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/PiranhaUtils.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/UsageCounter.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/XPFlagCleaner.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/Config.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/MethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaEnumRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaMethodRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/config/PiranhaRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationArgument.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/AnnotationResolutionException.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/ResolvedTestAnnotation.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationResolver.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/main/java/com/uber/piranha/testannotations/TestAnnotationSpecRecord.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/ConfigurationTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/CorePiranhaTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/EnumConstantTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/PiranhaTestingHelpers.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/TestCaseCleanUpTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/java/com/uber/piranha/TreatmentGroupsTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerNegativeCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPFlagCleanerPositiveCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCases.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesControl.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotAllowMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesDoNotallowArgMatchingAndMethodChain.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatment.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPMethodChainCasesTreatmentDoNotAllowMatchingArgMethodInvc.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/com/uber/piranha/XPTest.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_method_chain_control.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_method_chain_treated.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_no_method_chain.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_argument.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_clean_by_setters_ignore_others.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_noTreatmentGroup.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_receive.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_receive.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_test_return_receive_argument.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json` & `polyglot_piranha-0.3.4/legacy/java/piranha/src/test/resources/config/properties_unnecessary_instance_method.json`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java` & `polyglot_piranha-0.3.4/legacy/java/sample/src/main/java/com/uber/mylib/MyClass.java`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak` & `polyglot_piranha-0.3.4/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.bak`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect` & `polyglot_piranha-0.3.4/legacy/java/sample/src/main/resources/com/uber/mylib/MyClass.expect`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/javascript/src/config_checker.js` & `polyglot_piranha-0.3.4/legacy/javascript/src/config_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/javascript/src/piranha.js` & `polyglot_piranha-0.3.4/legacy/javascript/src/piranha.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/javascript/src/refactor.js` & `polyglot_piranha-0.3.4/legacy/javascript/src/refactor.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/javascript/src/source_checker.js` & `polyglot_piranha-0.3.4/legacy/javascript/src/source_checker.js`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt` & `polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/README.txt` & `polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/README.txt`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp` & `polyglot_piranha-0.3.4/legacy/objc/src/XPFlagRefactoring/XPFlagRefactoring.cpp`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/pyproject.toml` & `polyglot_piranha-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/go/edges.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/go/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/go/rules.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/go/rules.toml`

 * *Files 3% similar despite different names*

```diff
@@ -448,18 +448,18 @@
 )
 """
 replace = ""
 replace_node = "short_v_decl"
 is_seed_rule = false
 # Check if there is an assignment to @variable_name with a value other than @value
 # Note that the query is against a short_var_declaration while
-# the constraint is against an assigment_statement
-[[rules.constraints]]
-matcher = "(block) @block"
-queries = ["""
+# the filter is against an assigment_statement
+[[rules.filters]]
+enclosing_node = "(block) @block"
+not_contains = ["""
 (
     (assignment_statement
         left: (expression_list
             (identifier) @a.lhs
         )
         right: (expression_list
             (_) @a.rhs
@@ -478,17 +478,17 @@
     (#eq? @identifier "@variable_name")
 )
 """
 replace = "@value"
 replace_node = "identifier"
 holes = ["variable_name", "value"]
 is_seed_rule = false
-[[rules.constraints]]
-matcher = "(block) @block"
-queries = ["""
+[[rules.filters]]
+enclosing_node = "(block) @block"
+not_contains = ["""
 (
     [
         (short_var_declaration
             left: (expression_list
                 (identifier) @vn
             )
         ) @assignment
```

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/go/scope_config.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/go/scope_config.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 [[scopes]]
 name = "File"
 [[scopes.rules]]
-matcher = """
+enclosing_node = """
 (source_file) @source_file
 """
-generator = """(source_file) @sf"""
+scope = """(source_file) @sf"""
 
 [[scopes]]
 name = "Function-Method"
 [[scopes.rules]]
-matcher = """
+enclosing_node = """
 (
     (
         [
             (function_declaration
                 name: (_) @n
                 parameters: (parameter_list) @pl
             )
@@ -32,15 +32,15 @@
                 name: (_) @n
                 parameters: (parameter_list) @pl
             )
         ]
     ) @f_decl1
 )
 """
-generator = """
+scope = """
 (
     (
         [
             (function_declaration
                 name: (_) @fn
                 parameters: (parameter_list) @paramlist
             )
```

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/java/edges.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/java/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/java/rules.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/java/rules.toml`

 * *Files 5% similar despite different names*

```diff
@@ -482,34 +482,34 @@
 [[rules]]
 name = "delete_empty_enum_declaration"
 query = """
 (enum_declaration) @enum_declaration"""
 replace = ""
 replace_node = "enum_declaration"
 is_seed_rule = false
-[[rules.constraints]]
-matcher = "(enum_declaration) @ed"
-queries = ["(enum_constant) @ec"]
+[[rules.filters]]
+enclosing_node = "(enum_declaration) @ed"
+not_contains = ["(enum_constant) @ec"]
 
 
 # This rule deltes all the content of the file if it contains 
 # no type declaration, enum declaration and annotation type declaration. 
 #
 # It optionally captures the @package_name for the deleted file. 
 [[rules]]
 name = "delete_file_with_no_type_declarations"
 query = """(
 (program 
   (package_declaration (_) @package_name)?) @program)"""
 replace = ""
 replace_node = "program"
 is_seed_rule = false
-[[rules.constraints]]
-matcher = "(program) @c_program"
-queries = [
+[[rules.filters]]
+enclosing_node = "(program) @c_program"
+not_contains = [
   "(enum_declaration) @c_enum_declaration",
   "(class_declaration) @c_class_declaration",
   "(interface_declaration) @c_interface_declaration",
   "(annotation_type_declaration) @c_annotation_type_declaration",
   "(module_declaration) @c_module_declaration",
   "(record_declaration) @c_arecord_declaration",
 ]
@@ -551,19 +551,19 @@
 """
 replace = ""
 replace_node = "variable_declaration"
 is_seed_rule = false
 
 # Check if there is no assignment where the variable @variable_name is 
 # assigned to a value other than @init, within the method body
-# Please note that the tree-sitter queries in the constraint uses holes (i.e. `@variable_name` and `@init`).
+# Please note that the tree-sitter queries in the filter uses holes (i.e. `@variable_name` and `@init`).
 # These holes will be filled contextually based on the code snippet matched to `rule.query
-[[rules.constraints]]
-matcher = "[(method_declaration) (constructor_declaration)] @md"
-queries = ["""
+[[rules.filters]]
+enclosing_node = "[(method_declaration) (constructor_declaration)] @md"
+not_contains = ["""
 (
 ((assignment_expression
                     left: (_) @a.lhs
                     right: (_) @a.rhs) @assignment)
 (#eq? @a.lhs "@variable_name")
 (#not-eq? @a.rhs "@init")
 )"""]
@@ -582,17 +582,17 @@
 """
 replace = ""
 replace_node = "field_declaration"
 is_seed_rule = false
 
 # Check if there is no assignment where the variable @variable_name is 
 # assigned to a value other than @init, within the method body
-[[rules.constraints]]
-matcher = "(class_declaration) @cd"
-queries = ["""(
+[[rules.filters]]
+enclosing_node = "(class_declaration) @cd"
+not_contains = ["""(
 ((assignment_expression
                     left: (_) @a.lhs
                     right: (_) @a.rhs) @assignment)
 (#eq? @a.lhs "@variable_name")
 (#not-eq? @a.rhs "@init")
 )"""]
 
@@ -613,17 +613,17 @@
 """
 replace = ""
 replace_node = "expression_statement"
 is_seed_rule = false
 holes = ["variable_name", "init"]
 # The enclosing methode declaration should not contain a local variable decalration named "@variable_name"
 # which is initialized to "@init".
-[[rules.constraints]]
-matcher = "[(method_declaration) (constructor_declaration)] @md"
-queries = ["""(
+[[rules.filters]]
+enclosing_node = "[(method_declaration) (constructor_declaration)] @md"
+not_contains = ["""(
 ((local_variable_declaration 
                 declarator: (variable_declarator 
                                     name: (_) @vdcl.lhs
                                     value: (_) @vdcl.init)) @field_declaration)
 (#eq? @vdcl.lhs "@l")
 )"""]
 
@@ -641,30 +641,30 @@
                     right: (_) @init)) @expression_statement
 ) 
 """
 replace = ""
 replace_node = "expression_statement"
 is_seed_rule = false
 # The enclosing methode declaration should not contain a local variable decalration named "@variable_name"
-[[rules.constraints]]
-matcher = "(method_declaration) @md"
-queries = [
+[[rules.filters]]
+enclosing_node = "(method_declaration) @md"
+not_contains = [
   """(
 ((local_variable_declaration
                 declarator: (variable_declarator 
                                     name: (_) @vdcl.lhs
                                     value: (_)? @vdcl.init)) @variable_declaration)
 (#eq? @vdcl.lhs "@variable_name")
 )""",
 ]
-[[rules.constraints]]
+[[rules.filters]]
 # There should exist no field declaration named `@variable_name` and
 # there should be no assignments to @variable_name that are not same as `@init`.
-matcher = "(class_declaration) @cd"
-queries = ["""(
+enclosing_node = "(class_declaration) @cd"
+not_contains = ["""(
 ((assignment_expression
                     left: (_) @a.lhs
                     right: (_) @a.rhs) @a)
 (#eq? @a.lhs "@variable_name")
 (#not-eq? @a.rhs "@init")
 )""", """(
 ((field_declaration 
@@ -673,31 +673,31 @@
                                     value: (_) @fdcl.init)) @field_declaration)
 (#eq? @fdcl.lhs "@variable_name")
 (#not-eq? @fdcl.init "@init")
 )"""]
 
 # Replace identifier with value if :
 # (i) There is no local variable declaration in the enclosing method with the name as the identifier 
-# TODO: Add field constraint
+# TODO: Add field filter
 [[rules]]
 name = "replace_identifier_with_value"
 query = """
 (
 (identifier) @identifier
 (#eq? @identifier "@variable_name")
 )
 """
 replace = "@init"
 replace_node = "identifier"
 holes = ["variable_name", "init"]
 is_seed_rule = false
-[[rules.constraints]]
+[[rules.filters]]
 # There should exist no local variable declaration named `@identifer`
-matcher = "[(method_declaration) (constructor_declaration)] @md"
-queries = ["""(
+enclosing_node = "[(method_declaration) (constructor_declaration)] @md"
+not_contains = ["""(
 ((local_variable_declaration 
                 declarator: (variable_declarator 
                                     name: (_) @vdcl.lhs
                                     value: (_) @vdcl.init)) @field_declaration)
 (#eq? @vdcl.lhs "@identifier")
 )"""]
```

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/java/scope_config.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/java/scope_config.toml`

 * *Files 15% similar despite different names*

```diff
@@ -13,54 +13,54 @@
 # In `edges.toml`, we specify how the rules should be chained by constructing an edge labelled graph with rules as nodes. 
 # These edges are labelled as - Parent, Global, Method and Class. These edges determine "scope" where the next rule will be applied with respect
 # to the previously applied rule. 
 # Unlike Parent and Global scopes, capturing Method and Class scopes for Java is unique to Java's syntax. 
 # Each language has a syntax to define methods, classes, functions, therefore capturing such scopees is language dependent. 
 # This file allows users to define these language dependent scopes. 
 # Each scope consists of a scope name and a list of scope rules. 
-# Each scope rule consists of a `matcher` and a `generator`. 
+# Each scope rule consists of a `enclosing_node` and a `scope`.
 
 # When Piranha encounters a "Method" or "Class" scope, it looks up these configurations to obtain the list of scope rules. 
 # It then applies each `scope.rules.matcher` to the ancestors of changed node in the previous edit.
-# Upon finding the match (it short-circuits), Piranha substitutes the tags in `scope.rules.generator` based on the tag matches obtained from 
+# Upon finding the match (it short-circuits), Piranha substitutes the tags in `scope.rulesscope` based on the tag matches obtained from
 # matching `scope.rules.matcher` to create a context specific rule for the changed node.
 
 [[scopes]]
 name = "Method"
 [[scopes.rules]]
 # Example : 
 #
 # pub void foo(int a, int b, int c, int d, int e){
 #   // Let's assume that some rule was previously applied within this method body.
 # }  
 #
 # To capture the signature of the enclosing method, Piranha will match the below rule against the method.
 # This will result in matches - { n: "foo", fp: "int a, int b, int c, int d, int e"} 
-# Substituting these matches in the `scopes.rules.generator` will result in : 
+# Substituting these matches in the `scopes.rulesscope` will result in :
 #
 #(((method_declaration 
 #           name : (_) @z
 #           parameters : (formal_parameters)@fp) @xdn)
 
 # (#eq? @z "@foo")
 # (#eq? @tp "int a, int b, int c, int d, int e")
 # )
 #
-matcher = """
+enclosing_node = """
 (
   [(method_declaration 
             name : (_) @n
             parameters : (formal_parameters)@fp)
    (constructor_declaration 
             name: (_) @n
             parameters : (formal_parameters)@fp)
             
   ]          
             @xdn)"""
-generator = """
+scope = """
 (
   [(((method_declaration 
             name : (_) @z
             parameters : (formal_parameters)@tp))
     (#eq? @z "@n")
     (#eq? @tp "@fp")                  
     )
@@ -69,34 +69,34 @@
             parameters : (formal_parameters)@tp))
     (#eq? @tp "@fp")
     (#eq? @z "@n")
     )
   ]
 )@qdn"""
 
-# Scope generators for Java Class.
+# Scope generator for Java Class.
 [[scopes]]
 name = "Class"
 [[scopes.rules]]
-matcher = """(
+enclosing_node = """(
   [
     (class_declaration name:(_) @n) @c
     (enum_declaration name:(_) @n) @c
   ]
 )"""
-generator = """(
+scope = """(
   [
     ((class_declaration name:(_) @z) @qc)
     ((enum_declaration name:(_) @z) @qc)
   ]
 (#eq? @z "@n")
 )
 """
 
 # Scope generator for java compilation unit
 [[scopes]]
 name = "File"
 [[scopes.rules]]
-matcher = """
+enclosing_node = """
 (program) @c_u
 """
-generator = "(program) @compilation_unit"
+scope = "(program) @compilation_unit"
```

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/kt/edges.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/kt/edges.toml`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/kt/rules.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/kt/rules.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,27 +7,38 @@
 # <p>Unless required by applicable law or agreed to in writing, software distributed under the
 # License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
 # express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 # The language specific rules in this file are applied after the API specific change has been performed.
 
+# (true) -> true
+# (false) -> false
+[[rules]]
+name = "simplify_parenthesized_expression"
+query = """(
+  (parenthesized_expression (boolean_literal) @literal) @pe
+)"""
+replace = "@literal"
+replace_node = "pe"
+groups = ["boolean_expression_simplify"]
+is_seed_rule = false
 # Before : 
 # else if (true) { doSomething() }
 # After :
 # { doSomething(); } 
 # abc()
 # 
 [[rules]]
 groups = ["if_cleanup", "boolean_expression_simplify"]
 name = "simplify_ladder_if_true"
 query = """
 (
 (if_expression (_) (_) 
-               (control_structure_body ((if_expression [((boolean_literal) @condition) (parenthesized_expression (boolean_literal) @condition)] 
+               (control_structure_body ((if_expression ((boolean_literal) @condition) 
                (control_structure_body (_) ) @consequence) @if_expression) )) @outer_if
 (#eq? @condition "true")
 )
 """
 replace = "@consequence"
 replace_node = "if_expression"
 is_seed_rule = false
@@ -40,15 +51,15 @@
 # { doSomething(); } 
 [[rules]]
 groups = ["if_cleanup", "boolean_expression_simplify"]
 name = "simplify_ladder_if_true_with_alternative"
 query = """
 (
 (if_expression (_) @x (_) @y
-               (control_structure_body ((if_expression [((boolean_literal) @condition) (parenthesized_expression (boolean_literal) @condition)] 
+               (control_structure_body ((if_expression ((boolean_literal) @condition) 
                (control_structure_body (_))  @consequence 
                (control_structure_body (_) ) @alternative) @if_expression ) )) @outer_if
 (#eq? @condition "true")
 )
 """
 replace = "@consequence"
 replace_node = "if_expression"
@@ -61,15 +72,15 @@
 #
 [[rules]]
 groups = ["if_cleanup", "boolean_expression_simplify"]
 name = "simplify_ladder_if_false_with_alternative"
 query = """
 (
 (if_expression (_) (_) 
-               (control_structure_body ((if_expression [((boolean_literal) @condition) (parenthesized_expression (boolean_literal) @condition)] 
+               (control_structure_body ((if_expression ((boolean_literal) @condition)
                (control_structure_body) @consquent
                (_) @alternative) @if_expression) )) @outer_if
 (#eq? @condition "false")
 )
 """
 replace = "@alternative"
 replace_node = "if_expression"
@@ -81,15 +92,15 @@
 #  
 [[rules]]
 groups = ["if_cleanup", "boolean_expression_simplify"]
 name = "simplify_ladder_if_false"
 query = """
 (
 (if_expression (_) (_) 
-               (control_structure_body ((if_expression [((boolean_literal) @condition) (parenthesized_expression (boolean_literal) @condition)] 
+               (control_structure_body ((if_expression ((boolean_literal) @condition) 
                (control_structure_body) @consquent)) ) @alternative) @if_expression
 (#eq? @condition "false")
 )
 """
 replace = ""
 replace_node = "if_expression"
 is_seed_rule = false
@@ -100,15 +111,15 @@
 # { doSomething(); } 
 # 
 [[rules]]
 groups = ["if_cleanup", "boolean_expression_simplify"]
 name = "simplify_if_true"
 query = """
 (
-(if_expression [((boolean_literal) @condition) (parenthesized_expression (boolean_literal) @condition)] 
+(if_expression ((boolean_literal) @condition) 
                (control_structure_body (_)* @consequence ) ) @if_expression
 (#eq? @condition "true")
 )
 """
 replace = "@consequence"
 replace_node = "if_expression"
 is_seed_rule = false
@@ -120,15 +131,15 @@
 # { doSomething(); } 
 # abc()
 [[rules]]
 groups = ["if_cleanup", "boolean_expression_simplify"]
 name = "simplify_if_true_with_alternative"
 query = """
 (
-(if_expression [((boolean_literal) @condition) (parenthesized_expression (boolean_literal) @condition)] 
+(if_expression ((boolean_literal) @condition) 
                (control_structure_body (_)* @consequence ) 
                (control_structure_body) @alternative) @if_expression
 (#eq? @condition "true")
 )
 """
 replace = "@consequence"
 replace_node = "if_expression"
@@ -144,15 +155,15 @@
 # After :
 #  
 [[rules]]
 groups = ["if_cleanup", "boolean_expression_simplify"]
 name = "simplify_if_false_with_alternative"
 query = """
 (
-(if_expression [((boolean_literal) @condition) (parenthesized_expression (boolean_literal) @condition)] 
+(if_expression ((boolean_literal) @condition) 
                (control_structure_body) @consquent
                (control_structure_body (_)* @alternative) ) @if_expression
 (#eq? @condition "false")
 )"""
 replace = "@alternative"
 replace_node = "if_expression"
 is_seed_rule = false
@@ -162,15 +173,15 @@
 # After :
 #  
 [[rules]]
 groups = ["if_cleanup", "boolean_expression_simplify"]
 name = "simplify_if_false"
 query = """
 (
-(if_expression [((boolean_literal) @condition) (parenthesized_expression (boolean_literal) @condition)] 
+(if_expression ((boolean_literal) @condition) 
                (control_structure_body) @consquent) @if_expression
 (#eq? @condition "false")
 )"""
 replace = ""
 replace_node = "if_expression"
 is_seed_rule = false
 
@@ -180,15 +191,15 @@
 #  true 
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_not_false"
 query = """
 (
-(prefix_expression [((boolean_literal) @exp) (parenthesized_expression (boolean_literal) @exp)]) @prefix_expression
+(prefix_expression (boolean_literal) @exp) @prefix_expression
 (#eq? @exp "false")
 (#match @prefix_expression "!.*")  
 )
 """
 replace = "true"
 replace_node = "prefix_expression"
 is_seed_rule = false
@@ -199,15 +210,15 @@
 #  false
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_not_true"
 query = """
 (
-(prefix_expression [((boolean_literal) @exp) (parenthesized_expression (boolean_literal) @exp)]) @prefix_expression
+(prefix_expression (boolean_literal) @exp) @prefix_expression
 (#eq? @exp "true")
 (#match @prefix_expression "!.*")  
 )
 """
 replace = "false"
 replace_node = "prefix_expression"
 is_seed_rule = false
@@ -219,15 +230,15 @@
 #
 
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_true_and_something"
 query = """
 (
-(conjunction_expression [((boolean_literal) @lhs) (parenthesized_expression (boolean_literal) @lhs)]
+(conjunction_expression ((boolean_literal) @lhs)
                         (_) @rhs ) @conjunction_expression
 (#eq? @lhs "true")  
 )
 """
 replace = "@rhs"
 replace_node = "conjunction_expression"
 is_seed_rule = false
@@ -238,16 +249,15 @@
 #  abc()
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_something_and_true"
 query = """
 (
-(conjunction_expression (_) @lhs 
-                    [((boolean_literal) @rhs) (parenthesized_expression (boolean_literal) @rhs)] ) @conjunction_expression
+(conjunction_expression (_) @lhs (boolean_literal) @rhs) @conjunction_expression
 (#eq? @rhs "true")  
 )"""
 replace = "@lhs"
 replace_node = "conjunction_expression"
 is_seed_rule = false
 
 # Before :
@@ -256,15 +266,15 @@
 #  false
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_false_and_something"
 query = """
 (
-(conjunction_expression [((boolean_literal) @lhs) (parenthesized_expression (boolean_literal) @lhs)]
+(conjunction_expression ((boolean_literal) @lhs)
                          (_) @rhs ) @conjunction_expression
 (#eq? @lhs "false")  
 )"""
 replace = "false"
 replace_node = "conjunction_expression"
 is_seed_rule = false
 
@@ -275,19 +285,17 @@
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_something_and_false"
 query = """
 (
 (conjunction_expression [(simple_identifier)
-                          (parenthesized_expression (simple_identifier))
                           (boolean_literal)
-                          (parenthesized_expression (boolean_literal))
                         ] @lhs 
-                        [((boolean_literal) @rhs) (parenthesized_expression (boolean_literal) @rhs)] ) @conjunction_expression
+                        ((boolean_literal) @rhs) ) @conjunction_expression
 (#eq? @rhs "false")  
 )
 """
 replace = "false"
 replace_node = "conjunction_expression"
 is_seed_rule = false
 
@@ -298,19 +306,17 @@
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_something_or_true"
 query = """
 (
 (disjunction_expression [(simple_identifier)
-                          (parenthesized_expression (simple_identifier))
                           (boolean_literal)
-                          (parenthesized_expression (boolean_literal))
                         ] @lhs 
-                        [((boolean_literal) @rhs) (parenthesized_expression (boolean_literal) @rhs)] ) @disjunction_expression
+                        ((boolean_literal) @rhs)  ) @disjunction_expression
 (#eq? @rhs "true")  
 )"""
 replace = "true"
 replace_node = "disjunction_expression"
 is_seed_rule = false
 
 # Before :
@@ -319,15 +325,15 @@
 #  true
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_true_or_something"
 query = """
 (
-(disjunction_expression [((boolean_literal) @lhs) (parenthesized_expression (boolean_literal) @lhs)]
+(disjunction_expression ((boolean_literal) @lhs)
                          (_) @rhs ) @disjunction_expression
 (#eq? @lhs "true")  
 )
 """
 replace = "true"
 replace_node = "disjunction_expression"
 is_seed_rule = false
@@ -339,15 +345,15 @@
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_something_or_false"
 query = """
 (
 (disjunction_expression (_) @lhs 
-                        [((boolean_literal) @rhs) (parenthesized_expression (boolean_literal) @rhs)] ) @disjunction_expression
+                        ((boolean_literal) @rhs)  ) @disjunction_expression
 (#eq? @rhs "false")  
 )"""
 replace = "@lhs"
 replace_node = "disjunction_expression"
 is_seed_rule = false
 
 # Before: 
@@ -356,22 +362,89 @@
 #  abc()
 #
 [[rules]]
 groups = ["boolean_expression_simplify"]
 name = "simplify_false_or_something"
 query = """
 (
-(disjunction_expression [((boolean_literal) @lhs) (parenthesized_expression (boolean_literal) @lhs)]
+(disjunction_expression ((boolean_literal) @lhs)
                          (_) @rhs ) @disjunction_expression
 (#eq? @lhs "false")  
 )"""
 replace = "@rhs"
 replace_node = "disjunction_expression"
 is_seed_rule = false
 
+
+# Before
+# (true) == true
+# x == (x)
+# x == x
+# After
+# true 
+# true
+# true
+[[rules]]
+groups = ["boolean_expression_simplify"]
+name = "simplify_equality_true"
+query = """(
+(equality_expression (_)@l1 "==" (_)@l2) @equality
+(#eq? @l1 @l2)
+)"""
+replace = "true"
+replace_node = "equality"
+is_seed_rule = false
+
+# Before
+# true == false
+# After
+# false
+[[rules]]
+groups = ["boolean_expression_simplify"]
+name = "simplify_equality_false"
+query = """(
+(equality_expression [(boolean_literal) (integer_literal) (real_literal)]@l1 "==" [(boolean_literal) (integer_literal) (real_literal)]@l2) @equality
+(#not-eq? @l1 @l2)
+)"""
+replace = "false"
+replace_node = "equality"
+is_seed_rule = false
+
+# Before
+# true != true
+# After
+# false
+[[rules]]
+groups = ["boolean_expression_simplify"]
+name = "simplify_inequality_false"
+query = """(
+(equality_expression [(boolean_literal) (integer_literal) (real_literal)]@l1 "!=" [(boolean_literal) (integer_literal) (real_literal)] @l2) @inequality
+(#eq? @l1 @l2)
+)"""
+replace = "false"
+replace_node = "inequality"
+is_seed_rule = false
+
+
+# Before
+# true != false
+# After
+# true
+[[rules]]
+groups = ["boolean_expression_simplify"]
+name = "simplify_inequality_true"
+query = """(
+(equality_expression [(boolean_literal) (integer_literal) (real_literal)]@l1 "!=" [(boolean_literal) (integer_literal) (real_literal)] @l2) @inequality
+(#not-eq? @l1 @l2)
+)"""
+replace = "true"
+replace_node = "inequality"
+is_seed_rule = false
+
+
 # Before :
 #  {
 #    something();
 #    return 10;
 #    somethingMore();  
 #    return 100;
 #  } 
@@ -400,30 +473,30 @@
 name = "delete_empty_enum_declaration"
 query = """
 (class_declaration (_) @name 
     (enum_class_body)) @enum_declaration"""
 replace = ""
 replace_node = "enum_declaration"
 is_seed_rule = false
-[[rules.constraints]]
-matcher = """(class_declaration (_) @nm
+[[rules.filters]]
+enclosing_node = """(class_declaration (_) @nm
     (enum_class_body)) @ed"""
-queries = ["(enum_entry) @ee"]
+not_contains = ["(enum_entry) @ee"]
 
 # Delete all file contents if 
 [[rules]]
 name = "delete_file_with_no_declarations"
 query = """
 (source_file) @source_file"""
 replace = ""
 replace_node = "program"
 is_seed_rule = false
-[[rules.constraints]]
-matcher = "(source_file) @sf"
-queries = [
+[[rules.filters]]
+enclosing_node = "(source_file) @sf"
+not_contains = [
   "(class_declaration) @cd",
   "(object_declaration) @od",
   "(function_declaration) @fd",
   "(property_declaration) @pd",
 ]
 
 
@@ -463,54 +536,53 @@
 replace_node = "property_declaration"
 holes = ["variable_name"]
 is_seed_rule = false
 
 [[rules]]
 name = "delete_local_var_property_declaration"
 query = """
-(property_declaration (variable_declaration (simple_identifier)@variable_name ) 
-                                 [(boolean_literal) @init ( parenthesized_expression (boolean_literal) @init)]) @property_declaration
+(property_declaration (variable_declaration (simple_identifier)@variable_name) (boolean_literal) @init) @property_declaration
 """
 replace = ""
 replace_node = "property_declaration"
 is_seed_rule = false
 
 # Check if there is no assignment where the variable @variable_name is 
 # assigned to a value other than @init, within the method body
-# Please note that the tree-sitter queries in the constraint uses holes (i.e. `@variable_name` and `@init`).
+# Please note that the tree-sitter queries in the filter uses holes (i.e. `@variable_name` and `@init`).
 # These holes will be filled contextually based on the code snippet matched to `rule.query
-# [[rules.constraints]]
-# matcher = "(function_declaration) @md"
-# queries = [] 
-[[rules.constraints]]
-matcher = "(function_declaration) @md"
-queries = [
+# [[rules.filters]]
+# enclosing_node =  "(function_declaration) @md"
+# not_contains = []
+[[rules.filters]]
+enclosing_node = "(function_declaration) @md"
+not_contains = [
   """(
 (assignment (directly_assignable_expression (simple_identifier)@a.lhs) (_)@a.rhs)    @assignment
 (#eq? @a.lhs "@variable_name")
 (#not-eq? @a.rhs "@init")
 )""",
 ]
 
 # This rule is part (and entry point) of the inline field declaration cleanup.
 # Same as the rule `delete_variable_declaration`, but applicable to fields.
 [[rules]]
 name = "delete_field_property_declaration"
 query = """
-(property_declaration (variable_declaration (simple_identifier)@variable_name ) 
-                                 [(boolean_literal)  @init ( parenthesized_expression (boolean_literal) @init)]) @property_declaration
+(property_declaration (variable_declaration (simple_identifier)@variable_name) 
+                                 (boolean_literal)  @init) @property_declaration
 """
 replace = ""
 replace_node = "property_declaration"
 is_seed_rule = false
 # Check if there is no assignment where the variable @variable_name is 
 # assigned to a value other than @init, within the method body
-[[rules.constraints]]
-matcher = "(class_declaration) @cd"
-queries = [
+[[rules.filters]]
+enclosing_node = "(class_declaration) @cd"
+not_contains = [
   """(
 (assignment (directly_assignable_expression (simple_identifier)@a.lhs) (_)@a.rhs)    @assignment
 (#eq? @a.lhs "@variable_name")
 (#not-eq? @a.rhs "@init")
 )""",
 ]
 
@@ -529,20 +601,20 @@
 """
 replace = ""
 replace_node = "assignment"
 holes = ["variable_name", "init"]
 is_seed_rule = false
 # The enclosing methode declaration should not contain a local variable decalration named "@variable_name"
 # which is initialized to "@init".
-[[rules.constraints]]
-matcher = "(function_declaration) @md"
-queries = [
+[[rules.filters]]
+enclosing_node = "(function_declaration) @md"
+not_contains = [
   """(
 (property_declaration (variable_declaration (simple_identifier)@vdcl.lhs ) 
-                                 [(boolean_literal)  @vdcl.init ( parenthesized_expression (boolean_literal) @vdcl.init)]) @property_declaration
+                                 (boolean_literal)  @vdcl.init) @property_declaration
 (#eq? @vdcl.lhs "@l")
 )""",
 ]
 
 [[rules]]
 name = "delete_boolean_assignments_for_field"
 query = """
@@ -554,20 +626,20 @@
 """
 replace = ""
 replace_node = "assignment"
 holes = ["variable_name", "init"]
 is_seed_rule = false
 # The enclosing methode declaration should not contain a local variable decalration named "@variable_name"
 # which is initialized to "@init".
-[[rules.constraints]]
-matcher = "(class_declaration) @md"
-queries = [
+[[rules.filters]]
+enclosing_node = "(class_declaration) @md"
+not_contains = [
   """(
 (property_declaration (variable_declaration (simple_identifier)@vdcl.lhs ) 
-                                 [(boolean_literal)  @vdcl.init ( parenthesized_expression (boolean_literal) @vdcl.init)]) @property_declaration
+                                 (boolean_literal)  @vdcl.init) @property_declaration
 (#eq? @vdcl.lhs "@l")
 )""",
 ]
 
 # This rule is part (and entry point) of the inline variable / field declaration. 
 # delete assignment if 
 # (i) if it is the only assignment in the entire class in the enclosing class
@@ -578,72 +650,72 @@
 query = """
 (assignment (directly_assignable_expression (simple_identifier)@variable_name) (boolean_literal) @init)    @assignment
 """
 replace = ""
 replace_node = "assignment"
 is_seed_rule = false
 # The enclosing methode declaration should not contain a local variable decalration named "@variable_name"\
-[[rules.constraints]]
-matcher = "(function_declaration) @md"
-queries = ["""(
+[[rules.filters]]
+enclosing_node = "(function_declaration) @md"
+not_contains = ["""(
 (property_declaration (variable_declaration (simple_identifier)@f_vdcl.lhs ) 
                                  (_)@f_vdcl.init) @property_declaration
   (#eq? @f_vdcl.lhs "@variable_name")
   (#not-eq? @f_vdcl.init "@init")
 )"""]
 
-[[rules.constraints]]
-matcher = "(function_declaration) @md"
-queries = [
+[[rules.filters]]
+enclosing_node = "(function_declaration) @md"
+not_contains = [
   """(
 (assignment (directly_assignable_expression (simple_identifier)@a.lhs) (_)@a.rhs)    @f_assignment
   (#eq? @a.lhs "@variable_name")
   (#not-eq? @a.rhs "@init")
 )""",
 ]
 
-[[rules.constraints]]
-matcher = "(class_declaration) @md"
-queries = ["""(
+[[rules.filters]]
+enclosing_node = "(class_declaration) @md"
+not_contains = ["""(
 (property_declaration (variable_declaration (simple_identifier)@vdcl.lhs ) 
                                  (_)@vdcl.init ) @property_declaration
 (#eq? @vdcl.lhs "@variable_name")
 (#not-eq? @vdcl.init "@init")
 )"""]
 
-[[rules.constraints]]
-matcher = "(class_declaration) @md"
-queries = [
+[[rules.filters]]
+enclosing_node = "(class_declaration) @md"
+not_contains = [
   """(
 (assignment (directly_assignable_expression (simple_identifier)@a.lhs) (_)@a.rhs)    @c_assignment
   (#eq? @a.lhs "@variable_name")
   (#not-eq? @a.rhs "@init")
 )""",
 ]
 
 
 # Replace identifier with value if :
 # (i) There is no local variable declaration in the enclosing method with the name as the identifier 
-# TODO: Add field constraint
+# TODO: Add field filter
 [[rules]]
 holes = ["variable_name", "init"]
 name = "replace_identifier_with_value"
 query = """
 (
 (simple_identifier) @identifier
 (#eq? @identifier "@variable_name")
 )
 """
 replace = "@init"
 replace_node = "identifier"
 is_seed_rule = false
-# [[rules.constraints]]
+# [[rules.filters]]
 # There should exist no local variable declaration named `@identifer`
-# matcher = "(function_declaration) @md"
-# queries = [
+# enclosing_node =  "(function_declaration) @md"
+# not_contains = [
 #   """(
 # (property_declaration (variable_declaration (simple_identifier)@vdcl.lhs ) 
 #                                  [(boolean_literal)  @vdcl.init ( parenthesized_expression (boolean_literal) @vdcl.init)]) @property_declaration
 # (#eq? @vdcl.lhs "@identifier")
 # )""",
 # ]
```

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/kt/scope_config.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/kt/scope_config.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,50 +15,50 @@
 
 # fun add(int a, int b, int c, int d, int e): Int{
 #   // Let's assume that some rule was previously applied within this method body.
 # }  
 #
 # To capture the signature of the enclosing method, Piranha will match the below rule against the method.
 # This will result in matches - { n: "add", fp: "(int a, int b, int c, int d, int e): Int"} 
-# Substituting these matches in the `scopes.rules.generator` will result in : 
+# Substituting these matches in the `scopes.rulesscope` will result in :
 #
 #(((method_declaration 
 #           name : (_) @z
 #           parameters : (formal_parameters)@fp) @xdn)
 
 # (#eq? @z "add")
 # (#eq? @tp "(int a, int b, int c, int d, int e): Int")
 # )
 #
 [[scopes]]
 name = "Function"
 [[scopes.rules]]
-matcher = """
+enclosing_node = """
 ((function_declaration (simple_identifier) @n  (function_value_parameters) @sign (function_body) @fb) @qd5)
 """
-generator = """(
+scope = """(
 ((function_declaration (simple_identifier) @z  (function_value_parameters) @g_sign (function_body) @g_fb) @g_qd5)
 (#eq? @z "@n")
 (#eq? @g_sign "@sign")                
 )"""
 
 # Scope generator for Kotlin class.
 [[scopes]]
 name = "Class"
 [[scopes.rules]]
-matcher = "(class_declaration (type_identifier) @n) @c"
-generator = """
+enclosing_node = "(class_declaration (type_identifier) @n) @c"
+scope = """
 (
 ((class_declaration (type_identifier) @z) @qc)
 (#eq? @z "@n")
 )
 """
 
 
 # Scope generator for kt compilation unit
 [[scopes]]
 name = "File"
 [[scopes.rules]]
-matcher = """
+enclosing_node = """
 (source_file) @s_f
 """
-generator = "(source_file) @source_file"
+scope = "(source_file) @source_file"
```

### Comparing `polyglot_piranha-0.3.3/src/cleanup_rules/swift/scope_config.toml` & `polyglot_piranha-0.3.4/src/cleanup_rules/swift/scope_config.toml`

 * *Files 24% similar despite different names*

```diff
@@ -9,43 +9,59 @@
 # express or implied. See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 [[scopes]]
 name = "Class"
 [[scopes.rules]]
-matcher = """
+enclosing_node = """
 (class_declaration name: (_) @cls_name) @class
 """
-generator = """(
+scope = """(
 (class_declaration name: (_) @name) @cs
 (#eq? @name "@cls_name")              
 )"""
 
 [[scopes]]
 name = "Function"
 [[scopes.rules]]
-matcher = """(
+enclosing_node = """(
     (function_declaration
         name: (simple_identifier)? @name
         (parameter)? @params
         body: (function_body)
     ) @function
 )"""
-generator = """(
+scope = """(
     (function_declaration
         name: (simple_identifier)? @func_name
         (parameter)? @parameters
         body: (function_body)
     ) @func
     (#eq? @func_name "@name")
     (#eq? @parameters "@params")
 )"""
 
+[[scopes]]
+name = "Constructor"
+[[scopes.rules]]
+enclosing_node = """(
+    (init_declaration
+        (parameter)? @params
+        body: (function_body)
+    )
+)"""
+scope = """(
+    (init_declaration)
+        (parameter)? @parameters
+        body: (function_body)
+    )
+    (#eq? @parameters "@params")
+)"""
 
 [[scopes]]
 name = "File"
 [[scopes.rules]]
-matcher = """
+enclosing_node = """
 (source_file) @source_file
 """
-generator = """(source_file) @sf"""
+scope = """(source_file) @sf"""
```

### Comparing `polyglot_piranha-0.3.3/src/lib.rs` & `polyglot_piranha-0.3.4/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 
 #![allow(deprecated)] // This prevents cargo clippy throwing warning for deprecated use.
 use models::{
-  constraint::Constraint, edit::Edit, matches::Match, outgoing_edges::OutgoingEdges,
+  edit::Edit, filter::Filter, matches::Match, outgoing_edges::OutgoingEdges,
   piranha_arguments::PiranhaArguments, piranha_output::PiranhaOutputSummary, rule::Rule,
   rule_graph::RuleGraph, source_code_unit::SourceCodeUnit,
 };
 
 pub mod models;
 #[cfg(test)]
 mod tests;
@@ -41,15 +41,15 @@
   m.add_class::<PiranhaArguments>()?;
   m.add_class::<PiranhaOutputSummary>()?;
   m.add_class::<Edit>()?;
   m.add_class::<Match>()?;
   m.add_class::<RuleGraph>()?;
   m.add_class::<Rule>()?;
   m.add_class::<OutgoingEdges>()?;
-  m.add_class::<Constraint>()?;
+  m.add_class::<Filter>()?;
   Ok(())
 }
 
 /// Executes piranha for the given `piranha_arguments`.
 ///
 /// # Arguments:
 /// * piranha_arguments: Piranha Arguments
@@ -137,15 +137,19 @@
     // Keep looping until new `global` rules are added.
     loop {
       let current_rules = self.rule_store.global_rules().clone();
 
       debug!("\n # Global rules {}", current_rules.len());
       // Iterate over each file containing the usage of the feature flag API
 
-      for (path, content) in self.rule_store.get_relevant_files(&path_to_codebase) {
+      for (path, content) in self.rule_store.get_relevant_files(
+        &path_to_codebase,
+        piranha_args.include(),
+        piranha_args.exclude(),
+      ) {
         // Get the `SourceCodeUnit` for the file `path` from the cache `relevant_files`.
         // In case of miss, lazily insert a new `SourceCodeUnit`.
         let source_code_unit = self
           .relevant_files
           .entry(path.to_path_buf())
           .or_insert_with(|| {
             SourceCodeUnit::new(
@@ -194,15 +198,15 @@
   /// Returns: A temporary directory containing the created input code snippet as a file
   /// This function panics if it finds that neither `code_snippet` nor `path_to_configuration` are provided  
   fn write_code_snippet_to_temp(&self) -> TempDir {
     let temp_dir = TempDir::new_in(".", "tmp").unwrap();
     let temp_dir_path = temp_dir.path();
     let sample_file = temp_dir_path.join(format!(
       "sample.{}",
-      self.piranha_arguments.language().name()
+      self.piranha_arguments.language().extension()
     ));
     let mut file = File::create(sample_file).unwrap();
     file
       .write_all(self.piranha_arguments.code_snippet().as_bytes())
       .unwrap();
     temp_dir
   }
```

### Comparing `polyglot_piranha-0.3.3/src/main.rs` & `polyglot_piranha-0.3.4/src/main.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/models/default_configs.rs` & `polyglot_piranha-0.3.4/src/models/default_configs.rs`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,18 @@
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 
 use std::collections::{HashMap, HashSet};
 
+use glob::Pattern;
+
 use super::{
-  constraint::Constraint, language::PiranhaLanguage, outgoing_edges::OutgoingEdges, rule::Rule,
+  filter::Filter, language::PiranhaLanguage, outgoing_edges::OutgoingEdges, rule::Rule,
   rule_graph::RuleGraph,
 };
 use crate::utilities::tree_sitter_utilities::TSQuery;
 
 pub const JAVA: &str = "java";
 pub const KOTLIN: &str = "kt";
 pub const GO: &str = "go";
@@ -27,14 +29,15 @@
 pub const TYPESCRIPT: &str = "ts";
 pub const TSX: &str = "tsx";
 pub const THRIFT: &str = "thrift";
 
 #[cfg(test)]
 //FIXME: Remove this  hack by not passing PiranhaArguments to SourceCodeUnit
 pub(crate) const UNUSED_CODE_PATH: &str = "/dev/null";
+pub(crate) const DEFAULT_ENCLOSING_QUERY: &str = "";
 
 pub fn default_number_of_ancestors_in_parent_scope() -> u8 {
   4
 }
 
 pub fn default_language() -> String {
   JAVA.to_string()
@@ -68,14 +71,22 @@
   String::new()
 }
 
 pub fn default_code_snippet() -> String {
   String::new()
 }
 
+pub fn default_include() -> Vec<Pattern> {
+  Vec::new()
+}
+
+pub fn default_exclude() -> Vec<Pattern> {
+  Vec::new()
+}
+
 pub fn default_path_to_configurations() -> String {
   String::new()
 }
 
 pub fn default_path_to_output_summaries() -> Option<String> {
   None
 }
@@ -108,31 +119,43 @@
   HashSet::new()
 }
 
 pub(crate) fn default_groups() -> HashSet<String> {
   HashSet::new()
 }
 
-pub(crate) fn default_constraints() -> HashSet<Constraint> {
+pub(crate) fn default_filters() -> HashSet<Filter> {
   HashSet::new()
 }
 
 pub(crate) fn default_rules() -> Vec<Rule> {
   Vec::new()
 }
 
 pub(crate) fn default_edges() -> Vec<OutgoingEdges> {
   vec![]
 }
 
-pub(crate) fn default_queries() -> Vec<TSQuery> {
+pub(crate) fn default_not_contains_queries() -> Vec<TSQuery> {
   Vec::new()
 }
 
-pub(crate) fn default_matcher() -> TSQuery {
+pub(crate) fn default_contains_query() -> TSQuery {
+  TSQuery::new(String::from(""))
+}
+
+pub(crate) fn default_contains_at_least() -> u32 {
+  1
+}
+
+pub(crate) fn default_contains_at_most() -> u32 {
+  u32::MAX
+}
+
+pub(crate) fn default_enclosing_node() -> TSQuery {
   TSQuery::new(String::new())
 }
 
 pub(crate) fn default_rule_name() -> String {
   String::new()
 }
```

### Comparing `polyglot_piranha-0.3.3/src/models/edit.rs` & `polyglot_piranha-0.3.4/src/models/edit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/models/language.rs` & `polyglot_piranha-0.3.4/src/models/language.rs`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   scopes::{ScopeConfig, ScopeGenerator},
 };
 
 #[derive(Debug, Clone, Getters, PartialEq)]
 pub struct PiranhaLanguage {
   /// The extension of the language FIXME: - https://github.com/uber/piranha/issues/365
   #[get = "pub"]
-  name: String,
+  extension: String,
   /// the language (enum)
   #[get = "pub"]
   supported_language: SupportedLanguage,
   /// the language (As tree sitter model)
   #[get = "pub"]
   language: tree_sitter::Language,
   /// Built-in rules for the language
@@ -84,15 +84,15 @@
       .expect("Could not set the language for the parser.");
     parser
   }
 
   pub(crate) fn can_parse(&self, de: &jwalk::DirEntry<((), ())>) -> bool {
     de.path()
       .extension()
-      .and_then(|e| e.to_str().filter(|x| x.eq(&self.name())))
+      .and_then(|e| e.to_str().filter(|x| x.eq(&self.extension())))
       .is_some()
   }
 
   #[cfg(test)]
   pub(crate) fn set_scopes(&mut self, scopes: Vec<ScopeGenerator>) {
     self.scopes = scopes;
   }
@@ -116,15 +116,15 @@
   /// argument into PiranhaLanguage
   fn from_str(language: &str) -> Result<Self, Self::Err> {
     match language {
       JAVA => {
         let rules: Rules = parse_toml(include_str!("../cleanup_rules/java/rules.toml"));
         let edges: Edges = parse_toml(include_str!("../cleanup_rules/java/edges.toml"));
         Ok(Self {
-          name: language.to_string(),
+          extension: language.to_string(),
           supported_language: SupportedLanguage::Java,
           language: tree_sitter_java::language(),
           rules: Some(rules),
           edges: Some(edges),
           scopes: parse_toml::<ScopeConfig>(include_str!(
             "../cleanup_rules/java/scope_config.toml"
           ))
@@ -133,86 +133,86 @@
           comment_nodes: vec!["line_comment".to_string(), "block_comment".to_string()],
         })
       }
       GO => {
         let rules: Rules = parse_toml(include_str!("../cleanup_rules/go/rules.toml"));
         let edges: Edges = parse_toml(include_str!("../cleanup_rules/go/edges.toml"));
         Ok(PiranhaLanguage {
-          name: language.to_string(),
+          extension: language.to_string(),
           supported_language: SupportedLanguage::Go,
           language: tree_sitter_go::language(),
           rules: Some(rules),
           edges: Some(edges),
           scopes: parse_toml::<ScopeConfig>(include_str!("../cleanup_rules/go/scope_config.toml"))
             .scopes()
             .to_vec(),
           comment_nodes: vec!["comment".to_string()],
         })
       }
       KOTLIN => {
         let rules: Rules = parse_toml(include_str!("../cleanup_rules/kt/rules.toml"));
         let edges: Edges = parse_toml(include_str!("../cleanup_rules/kt/edges.toml"));
         Ok(PiranhaLanguage {
-          name: language.to_string(),
+          extension: language.to_string(),
           supported_language: SupportedLanguage::Kotlin,
           language: tree_sitter_kotlin::language(),
           rules: Some(rules),
           edges: Some(edges),
           scopes: parse_toml::<ScopeConfig>(include_str!("../cleanup_rules/kt/scope_config.toml"))
             .scopes()
             .to_vec(),
           comment_nodes: vec!["comment".to_string()],
         })
       }
       PYTHON => Ok(PiranhaLanguage {
-        name: language.to_string(),
+        extension: language.to_string(),
         supported_language: SupportedLanguage::Python,
         language: tree_sitter_python::language(),
         rules: None,
         edges: None,
         scopes: vec![],
         comment_nodes: vec![],
       }),
       SWIFT => {
         let rules: Rules = parse_toml(include_str!("../cleanup_rules/swift/rules.toml"));
         let edges: Edges = parse_toml(include_str!("../cleanup_rules/swift/edges.toml"));
         Ok(PiranhaLanguage {
-          name: language.to_string(),
+          extension: language.to_string(),
           supported_language: SupportedLanguage::Swift,
           language: tree_sitter_swift::language(),
           scopes: parse_toml::<ScopeConfig>(include_str!(
             "../cleanup_rules/swift/scope_config.toml"
           ))
           .scopes()
           .to_vec(),
           comment_nodes: vec!["comment".to_string(), "multiline_comment".to_string()],
           rules: Some(rules),
           edges: Some(edges),
         })
       }
       TYPESCRIPT => Ok(PiranhaLanguage {
-        name: language.to_string(),
+        extension: language.to_string(),
         supported_language: SupportedLanguage::Ts,
         language: tree_sitter_typescript::language_typescript(),
         rules: None,
         edges: None,
         scopes: vec![],
         comment_nodes: vec![],
       }),
       TSX => Ok(PiranhaLanguage {
-        name: language.to_string(),
+        extension: language.to_string(),
         supported_language: SupportedLanguage::Tsx,
         language: tree_sitter_typescript::language_tsx(),
         rules: None,
         edges: None,
         scopes: vec![],
         comment_nodes: vec![],
       }),
       THRIFT => Ok(PiranhaLanguage {
-        name: language.to_string(),
+        extension: language.to_string(),
         supported_language: SupportedLanguage::Thrift,
         language: tree_sitter_thrift::language(),
         rules: None,
         edges: None,
         scopes: vec![],
         comment_nodes: vec![],
       }),
```

### Comparing `polyglot_piranha-0.3.3/src/models/matches.rs` & `polyglot_piranha-0.3.4/src/models/matches.rs`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
       &node,
       self.code().to_string(),
       rule_store.query(&rule.query()),
       recursive,
       replace_node_tag,
     );
 
-    // Return the first match that satisfies constraint of the rule
+    // Applies the filter and returns the first element
     for p_match in all_query_matches.iter_mut() {
       let matched_node = get_node_for_range(
         self.root_node(),
         p_match.range().start_byte,
         p_match.range().end_byte,
       );
       if self.is_satisfied(matched_node, rule, p_match.matches(), rule_store) {
```

### Comparing `polyglot_piranha-0.3.3/src/models/mod.rs` & `polyglot_piranha-0.3.4/src/models/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
  <p>Unless required by applicable law or agreed to in writing, software distributed under the
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 
-pub(crate) mod constraint;
 pub(crate) mod default_configs;
 pub(crate) mod edit;
+pub(crate) mod filter;
 pub(crate) mod language;
 pub(crate) mod matches;
 pub(crate) mod outgoing_edges;
 pub mod piranha_arguments;
 pub mod piranha_output;
 pub(crate) mod rule;
 pub(crate) mod rule_graph;
```

### Comparing `polyglot_piranha-0.3.3/src/models/outgoing_edges.rs` & `polyglot_piranha-0.3.4/src/models/outgoing_edges.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/models/piranha_arguments.rs` & `polyglot_piranha-0.3.4/src/models/piranha_arguments.rs`

 * *Files 16% similar despite different names*

```diff
@@ -11,28 +11,29 @@
  limitations under the License.
 */
 
 use super::{
   default_configs::{
     default_allow_dirty_ast, default_cleanup_comments, default_cleanup_comments_buffer,
     default_code_snippet, default_delete_consecutive_new_lines, default_delete_file_if_empty,
-    default_dry_run, default_global_tag_prefix, default_number_of_ancestors_in_parent_scope,
-    default_path_to_codebase, default_path_to_configurations, default_path_to_output_summaries,
-    default_piranha_language, default_rule_graph, default_substitutions, GO, JAVA, KOTLIN, PYTHON,
-    SWIFT, TSX, TYPESCRIPT,
+    default_dry_run, default_exclude, default_global_tag_prefix, default_include,
+    default_number_of_ancestors_in_parent_scope, default_path_to_codebase,
+    default_path_to_configurations, default_path_to_output_summaries, default_piranha_language,
+    default_rule_graph, default_substitutions, GO, JAVA, KOTLIN, PYTHON, SWIFT, TSX, TYPESCRIPT,
   },
   language::PiranhaLanguage,
   rule_graph::{read_user_config_files, RuleGraph, RuleGraphBuilder},
   source_code_unit::SourceCodeUnit,
 };
-use crate::utilities::parse_key_val;
+use crate::utilities::{parse_glob_pattern, parse_key_val};
 use clap::builder::TypedValueParser;
 use clap::Parser;
 use derive_builder::Builder;
 use getset::{CopyGetters, Getters};
+use glob::Pattern;
 use itertools::Itertools;
 use log::{info, warn};
 use pyo3::{
   prelude::{pyclass, pymethods},
   types::PyDict,
 };
 use regex::Regex;
@@ -44,27 +45,39 @@
 #[clap(name = "Piranha")]
 #[pyclass]
 #[builder(build_fn(name = "create"))]
 pub struct PiranhaArguments {
   /// Path to source code folder or file
   #[get = "pub"]
   #[builder(default = "default_path_to_codebase()")]
-  #[clap(short = 'c', long, default_value_t = default_path_to_codebase())]
+  #[clap(short = 'c', long, required = true)]
   path_to_codebase: String,
 
+  /// Paths to include (as glob patterns)
+  #[get = "pub"]
+  #[builder(default = "default_include()")]
+  #[clap(long, value_parser = parse_glob_pattern, num_args = 0.., required=false)]
+  include: Vec<Pattern>,
+
+  /// Paths to exclude (as glob patterns)
+  #[get = "pub"]
+  #[builder(default = "default_exclude()")]
+  #[clap(long, value_parser = parse_glob_pattern, num_args = 0.., required=false)]
+  exclude: Vec<Pattern>,
+
   /// Code snippet to transform
   #[get = "pub"]
   #[builder(default = "default_code_snippet()")]
   #[clap(short = 't', long, default_value_t = default_code_snippet())]
   code_snippet: String,
 
   /// These substitutions instantiate the initial set of rules.
   /// Usage : -s stale_flag_name=SOME_FLAG -s namespace=SOME_NS1
   #[builder(default = "default_substitutions()")]
-  #[clap(short = 's',value_parser = parse_key_val)]
+  #[clap(short = 's', value_parser = parse_key_val)]
   substitutions: Vec<(String, String)>,
 
   /// Directory containing the configuration files -  `rules.toml` and  `edges.toml` (optional)
   #[get = "pub"]
   #[builder(default = "default_path_to_configurations()")]
   #[clap(short = 'f', long)]
   path_to_configurations: String,
@@ -160,73 +173,96 @@
   /// * global_tag_prefix (string): the prefix for global tags
   /// * delete_file_if_empty (bool): User option that determines whether an empty file will be deleted
   /// * path_to_output_summary : Path to the file where the Piranha output summary should be persisted
   /// * allow_dirty_ast : Allows syntax errors in the input source code
   /// Returns PiranhaArgument.
   #[new]
   fn py_new(
-    language: String, substitutions: Option<&PyDict>, path_to_configurations: Option<String>,
-    rule_graph: Option<RuleGraph>, path_to_codebase: Option<String>, code_snippet: Option<String>,
-    dry_run: Option<bool>, cleanup_comments: Option<bool>, cleanup_comments_buffer: Option<i32>,
-    number_of_ancestors_in_parent_scope: Option<u8>, delete_consecutive_new_lines: Option<bool>,
-    global_tag_prefix: Option<String>, delete_file_if_empty: Option<bool>,
-    path_to_output_summary: Option<String>, allow_dirty_ast: Option<bool>,
+    language: String, path_to_codebase: Option<String>, include: Option<Vec<String>>,
+    exclude: Option<Vec<String>>, substitutions: Option<&PyDict>,
+    path_to_configurations: Option<String>, rule_graph: Option<RuleGraph>,
+    code_snippet: Option<String>, dry_run: Option<bool>, cleanup_comments: Option<bool>,
+    cleanup_comments_buffer: Option<i32>, number_of_ancestors_in_parent_scope: Option<u8>,
+    delete_consecutive_new_lines: Option<bool>, global_tag_prefix: Option<String>,
+    delete_file_if_empty: Option<bool>, path_to_output_summary: Option<String>,
+    allow_dirty_ast: Option<bool>,
   ) -> Self {
     let subs = if substitutions.is_some() {
       substitutions
         .unwrap()
         .iter()
         .map(|(k, v)| (k.to_string(), v.to_string()))
         .collect_vec()
     } else {
       vec![]
     };
 
     let rg = rule_graph.unwrap_or_else(|| RuleGraphBuilder::default().build());
-    piranha_arguments! {
-      path_to_codebase = path_to_codebase.unwrap_or_else(default_path_to_codebase),
-      path_to_configurations = path_to_configurations.unwrap_or_else(default_path_to_configurations),
-      rule_graph = rg,
-      code_snippet = code_snippet.unwrap_or_else(default_code_snippet),
-      language = PiranhaLanguage::from(language.as_str()),
-      substitutions = subs,
-      dry_run = dry_run.unwrap_or_else(default_dry_run),
-      cleanup_comments = cleanup_comments.unwrap_or_else(default_cleanup_comments),
-      cleanup_comments_buffer = cleanup_comments_buffer.unwrap_or_else(default_cleanup_comments_buffer),
-      number_of_ancestors_in_parent_scope = number_of_ancestors_in_parent_scope.unwrap_or_else(default_number_of_ancestors_in_parent_scope),
-      delete_consecutive_new_lines = delete_consecutive_new_lines.unwrap_or_else(default_delete_consecutive_new_lines),
-      global_tag_prefix = global_tag_prefix.unwrap_or_else(default_global_tag_prefix),
-      delete_file_if_empty = delete_file_if_empty.unwrap_or_else(default_delete_file_if_empty),
-      path_to_output_summary = path_to_output_summary,
-      allow_dirty_ast = allow_dirty_ast.unwrap_or_else(default_allow_dirty_ast),
-    }
+    PiranhaArgumentsBuilder::default()
+      .path_to_codebase(path_to_codebase.unwrap_or_else(default_path_to_codebase))
+      .include(
+        include
+          .unwrap_or_default()
+          .iter()
+          .map(|x| Pattern::new(x).unwrap())
+          .collect_vec(),
+      )
+      .exclude(
+        exclude
+          .unwrap_or_default()
+          .iter()
+          .map(|x| Pattern::new(x).unwrap())
+          .collect_vec(),
+      )
+      .path_to_configurations(path_to_configurations.unwrap_or_else(default_path_to_configurations))
+      .rule_graph(rg)
+      .code_snippet(code_snippet.unwrap_or_else(default_code_snippet))
+      .language(PiranhaLanguage::from(language.as_str()))
+      .substitutions(subs)
+      .dry_run(dry_run.unwrap_or_else(default_dry_run))
+      .cleanup_comments(cleanup_comments.unwrap_or_else(default_cleanup_comments))
+      .cleanup_comments_buffer(
+        cleanup_comments_buffer.unwrap_or_else(default_cleanup_comments_buffer),
+      )
+      .number_of_ancestors_in_parent_scope(
+        number_of_ancestors_in_parent_scope
+          .unwrap_or_else(default_number_of_ancestors_in_parent_scope),
+      )
+      .delete_consecutive_new_lines(
+        delete_consecutive_new_lines.unwrap_or_else(default_delete_consecutive_new_lines),
+      )
+      .global_tag_prefix(global_tag_prefix.unwrap_or_else(default_global_tag_prefix))
+      .delete_file_if_empty(delete_file_if_empty.unwrap_or_else(default_delete_file_if_empty))
+      .path_to_output_summary(path_to_output_summary)
+      .allow_dirty_ast(allow_dirty_ast.unwrap_or_else(default_allow_dirty_ast))
+      .build()
   }
 }
 
 impl PiranhaArguments {
   pub fn get_language(&self) -> String {
-    self.language.name().to_string()
+    self.language.extension().to_string()
   }
 
   pub fn from_cli() -> Self {
     let p = PiranhaArguments::parse();
-    piranha_arguments! {
-      path_to_codebase = p.path_to_codebase().to_string(),
-      substitutions = p.substitutions.clone(),
-      language = p.language().clone(),
-      path_to_configurations = p.path_to_configurations().to_string(),
-      path_to_output_summary = p.path_to_output_summary().clone(),
-      delete_file_if_empty = *p.delete_file_if_empty(),
-      delete_consecutive_new_lines = *p.delete_consecutive_new_lines(),
-      global_tag_prefix = p.global_tag_prefix().to_string(),
-      number_of_ancestors_in_parent_scope = *p.number_of_ancestors_in_parent_scope(),
-      cleanup_comments_buffer = *p.cleanup_comments_buffer(),
-      cleanup_comments = *p.cleanup_comments(),
-      dry_run = *p.dry_run(),
-    }
+    PiranhaArgumentsBuilder::default()
+      .path_to_codebase(p.path_to_codebase().to_string())
+      .substitutions(p.substitutions.clone())
+      .language(p.language().clone())
+      .path_to_configurations(p.path_to_configurations().to_string())
+      .path_to_output_summary(p.path_to_output_summary().clone())
+      .delete_file_if_empty(*p.delete_file_if_empty())
+      .delete_consecutive_new_lines(*p.delete_consecutive_new_lines())
+      .global_tag_prefix(p.global_tag_prefix().to_string())
+      .number_of_ancestors_in_parent_scope(*p.number_of_ancestors_in_parent_scope())
+      .cleanup_comments_buffer(*p.cleanup_comments_buffer())
+      .cleanup_comments(*p.cleanup_comments())
+      .dry_run(*p.dry_run())
+      .build()
   }
 
   pub(crate) fn input_substitutions(&self) -> HashMap<String, String> {
     self.substitutions.iter().cloned().collect()
   }
 }
 
@@ -294,49 +330,14 @@
   if user_defined_rules.graph().is_empty() {
     warn!("NO RULES PROVIDED. Please provide rules via the RuleGraph API or as toml files");
   }
 
   built_in_rules.merge(&user_defined_rules)
 }
 
-#[macro_export]
-/// This macro can be used to construct a PiranhaArgument (via the builder).'
-/// Allows to use builder pattern more "dynamically"
-///
-/// Usage:
-///
-/// ```ignore
-/// piranha_arguments! {
-///   path_to_codebase = "path/to/code/base".to_string(),
-///   language = "Java".to_string(),
-///   path_to_configurations = "path/to/configurations".to_string(),
-/// }
-/// ```
-///
-/// expands to
-///
-/// ```ignore
-/// PiranhaArgumentsBuilder::default()
-///      .path_to_codebase("path/to/code/base".to_string())
-///      .language("Java".to_string())
-///      .path_to_configurations("path/to/configurations".to_string())
-///      .build()
-/// ```
-///
-macro_rules! piranha_arguments {
-    ($($kw: ident = $value: expr,)*) => {
-      $crate::models::piranha_arguments::PiranhaArgumentsBuilder::default()
-      $(
-        .$kw($value)
-       )*
-      .build()
-    };
-}
-pub use piranha_arguments;
-
 #[cfg(test)]
 #[path = "unit_tests/piranha_arguments_test.rs"]
 mod piranha_arguments_test;
 
 // Implements instance methods related to applying the user options provided in  piranha arguments
 impl SourceCodeUnit {
   /// Replaces three consecutive newline characters with two
```

### Comparing `polyglot_piranha-0.3.3/src/models/piranha_output.rs` & `polyglot_piranha-0.3.4/src/models/piranha_output.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/models/rule.rs` & `polyglot_piranha-0.3.4/src/models/rule.rs`

 * *Files 16% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 use getset::Getters;
 use pyo3::prelude::{pyclass, pymethods};
 use serde_derive::Deserialize;
 
 use crate::utilities::{gen_py_str_methods, tree_sitter_utilities::TSQuery, Instantiate};
 
 use super::{
-  constraint::Constraint,
   default_configs::{
-    default_constraints, default_groups, default_holes, default_is_seed_rule, default_query,
+    default_filters, default_groups, default_holes, default_is_seed_rule, default_query,
     default_replace, default_replace_node, default_rule_name,
   },
+  filter::Filter,
 };
 
 #[derive(Deserialize, Debug, Clone, Default, PartialEq)]
 // Represents the `rules.toml` file
 pub(crate) struct Rules {
   pub(crate) rules: Vec<Rule>,
 }
@@ -69,22 +69,22 @@
   groups: HashSet<String>,
   /// Holes that need to be filled, in order to instantiate a rule
   #[builder(default = "default_holes()")]
   #[serde(default = "default_holes")]
   #[get = "pub"]
   #[pyo3(get)]
   holes: HashSet<String>,
-  /// Additional constraints for matching the rule
-  #[builder(default = "default_constraints()")]
-  #[serde(default = "default_constraints")]
+  /// Filters to test before applying a rule
+  #[builder(default = "default_filters()")]
+  #[serde(default = "default_filters")]
   #[get = "pub"]
   #[pyo3(get)]
-  constraints: HashSet<Constraint>,
+  filters: HashSet<Filter>,
 
-  /// Additional constraints for matching the rule
+  /// Marks a rule as a seed rule
   #[builder(default = "default_is_seed_rule()")]
   #[serde(default = "default_is_seed_rule")]
   #[get = "pub"]
   #[pyo3(get)]
   is_seed_rule: bool,
 }
 
@@ -102,59 +102,59 @@
 
 #[macro_export]
 /// This macro can be used to construct a Rule (via the builder).'
 /// Allows to use builder pattern more "dynamically"
 ///
 /// Usage:
 ///
-/// ```ignore
+/// ```
 /// piranha_rule! {
 ///   name = "Some Rule".to_string(),
 ///   query= "(method_invocation name: (_) @name) @mi".to_string()
 /// }
 /// ```
 ///
 /// expands to
 ///
-/// ```ignore
+/// ```
 /// RuleBuilder::default()
 ///      .name("Some Rule".to_string())
 ///      .query("(method_invocation name: (_) @name) @mi".to_string)
 ///      .build()
 /// ```
 ///
 macro_rules! piranha_rule {
   (name = $name:expr
                 $(, query =$query: expr)?
                 $(, replace_node = $replace_node:expr)?
                 $(, replace = $replace:expr)?
                 $(, holes = [$($hole: expr)*])?
                 $(, is_seed_rule = $is_seed_rule:expr)?
                 $(, groups = [$($group_name: expr)*])?
-                $(, constraints = [$($constraint:tt)*])?
+                $(, filters = [$($filter:tt)*])?
               ) => {
     $crate::models::rule::RuleBuilder::default()
     .name($name.to_string())
     $(.query($crate::utilities::tree_sitter_utilities::TSQuery::new($query.to_string())))?
     $(.replace_node($replace_node.to_string()))?
     $(.replace($replace.to_string()))?
     $(.holes(std::collections::HashSet::from([$($hole.to_string(),)*])))?
     $(.groups(std::collections::HashSet::from([$($group_name.to_string(),)*])))?
-    $(.constraints(std::collections::HashSet::from([$($constraint)*])))?
+    $(.filters(std::collections::HashSet::from([$($filter)*])))?
     .build().unwrap()
   };
 }
 
 #[pymethods]
 impl Rule {
   #[new]
   fn py_new(
     name: String, query: String, replace: Option<String>, replace_node: Option<String>,
     holes: Option<HashSet<String>>, groups: Option<HashSet<String>>,
-    constraints: Option<HashSet<Constraint>>, is_seed_rule: Option<bool>,
+    filters: Option<HashSet<Filter>>, is_seed_rule: Option<bool>,
   ) -> Self {
     let mut rule_builder = RuleBuilder::default();
     rule_builder.name(name).query(TSQuery::new(query));
     if let Some(replace) = replace {
       rule_builder.replace(replace);
     }
 
@@ -166,16 +166,16 @@
       rule_builder.holes(holes);
     }
 
     if let Some(groups) = groups {
       rule_builder.groups(groups);
     }
 
-    if let Some(constraints) = constraints {
-      rule_builder.constraints(constraints);
+    if let Some(filters) = filters {
+      rule_builder.filters(filters);
     }
 
     if let Some(is_seed_rule) = is_seed_rule {
       rule_builder.is_seed_rule(is_seed_rule);
     }
 
     rule_builder.build().unwrap()
@@ -229,16 +229,16 @@
     self.rule().replace_node().to_string()
   }
 
   pub fn holes(&self) -> &HashSet<String> {
     self.rule().holes()
   }
 
-  pub fn constraints(&self) -> &HashSet<Constraint> {
-    self.rule().constraints()
+  pub fn filters(&self) -> &HashSet<Filter> {
+    self.rule().filters()
   }
 }
 
 impl Instantiate for Rule {
   /// Create a new query from `self` by updating the `query` and `replace` based on the substitutions.
   /// This functions assumes that each hole in the rule can be substituted.
   /// i.e. It assumes that `substitutions_for_holes` is exaustive and complete
```

### Comparing `polyglot_piranha-0.3.3/src/models/rule_graph.rs` & `polyglot_piranha-0.3.4/src/models/rule_graph.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/models/rule_store.rs` & `polyglot_piranha-0.3.4/src/models/rule_store.rs`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 use crate::{
   models::piranha_arguments::PiranhaArguments,
   models::scopes::ScopeQueryGenerator,
   utilities::{read_file, tree_sitter_utilities::TSQuery},
 };
 
 use super::{language::PiranhaLanguage, rule::InstantiatedRule};
+use glob::Pattern;
 
 /// This maintains the state for Piranha.
 #[derive(Debug, Getters, Default)]
 pub(crate) struct RuleStore {
   // Caches the compiled tree-sitter queries.
   rule_query_cache: HashMap<String, Query>,
   // Current global rules to be applied.
@@ -122,32 +123,39 @@
   pub(crate) fn any_global_rules_has_holes(&self) -> bool {
     self.global_rules().iter().any(|x| !x.holes().is_empty())
   }
 
   /// Gets all the files from the code base that (i) have the language appropriate file extension, and (ii) contains the grep pattern.
   /// Note that `WalkDir` traverses the directory with parallelism.
   /// If all the global rules have no holes (i.e. we will have no grep patterns), we will try to find a match for each global rule in every file in the target.
-  pub(crate) fn get_relevant_files(&self, path_to_codebase: &str) -> HashMap<PathBuf, String> {
+  pub(crate) fn get_relevant_files(
+    &self, path_to_codebase: &str, include: &Vec<Pattern>, exclude: &Vec<Pattern>,
+  ) -> HashMap<PathBuf, String> {
     let _path_to_codebase = Path::new(path_to_codebase).to_path_buf();
 
     //If the path_to_codebase is a file, then execute piranha on it
     if _path_to_codebase.is_file() {
       return HashMap::from_iter([(
         _path_to_codebase.clone(),
         read_file(&_path_to_codebase).unwrap(),
       )]);
     }
+
     let mut files: HashMap<PathBuf, String> = WalkDir::new(path_to_codebase)
-      // Walk over the entire code base
+      // walk over the entire code base
       .into_iter()
-      // Ignore errors
+      // ignore errors
       .filter_map(|e| e.ok())
-      // Filter files with the desired extension
+      // only retain the included paths (if any)
+      .filter(|f| include.is_empty() || include.iter().any(|p| p.matches_path(&f.path())))
+      // filter out all excluded paths (if any)
+      .filter(|f| exclude.is_empty() || exclude.iter().all(|p| !p.matches_path(&f.path())))
+      // filter files with the desired extension
       .filter(|de| self.language().can_parse(de))
-      // Read the file
+      // read the file
       .map(|f| (f.path(), read_file(&f.path()).unwrap()))
       .collect();
 
     if self.any_global_rules_has_holes() {
       let pattern = self.get_grep_heuristics();
       files = files
         .iter()
```

### Comparing `polyglot_piranha-0.3.3/src/models/scopes.rs` & `polyglot_piranha-0.3.4/src/models/scopes.rs`

 * *Files 11% similar despite different names*

```diff
@@ -36,48 +36,48 @@
   #[get = "pub"]
   rules: Vec<ScopeQueryGenerator>,
 }
 
 #[derive(Deserialize, Debug, Clone, Hash, PartialEq, Eq, Default, Getters, Builder)]
 pub(crate) struct ScopeQueryGenerator {
   #[get = "pub"]
-  matcher: TSQuery, // a tree-sitter query matching some enclosing AST pattern (like method or class)
+  enclosing_node: TSQuery, // a tree-sitter query matching some enclosing AST pattern (like method or class)
   #[get = "pub"]
-  generator: TSQuery, // a tree-sitter query matching the exact AST node
+  scope: TSQuery, // a tree-sitter query that will match the same node that matched `enclosing_node`
 }
 
 // Implements instance methods related to getting the scope
 impl SourceCodeUnit {
   /// Generate a tree-sitter based query representing the scope of the previous edit.
   /// We generate these scope queries by matching the rules provided in `<lang>_scopes.toml`.
   pub(crate) fn get_scope_query(
     &self, scope_level: &str, start_byte: usize, end_byte: usize, rules_store: &mut RuleStore,
   ) -> TSQuery {
     let root_node = self.root_node();
     let mut changed_node = get_node_for_range(root_node, start_byte, end_byte);
-    // Get the scope matchers for `scope_level` from the `scope_config.toml`.
-    let scope_matchers = rules_store.get_scope_query_generators(scope_level);
+    // Get the scope enclosing_nodes for `scope_level` from the `scope_config.toml`.
+    let scope_enclosing_nodes = rules_store.get_scope_query_generators(scope_level);
 
-    // Match the `scope_matcher.matcher` to the parent
+    // Match the `scope_enclosing_node.enclosing_node` to the parent
     loop {
       trace!(
         "Getting scope {} for node kind {}",
         scope_level,
         changed_node.kind()
       );
-      for m in &scope_matchers {
+      for m in &scope_enclosing_nodes {
         if let Some(p_match) = get_match_for_query(
           &changed_node,
           self.code(),
-          rules_store.query(m.matcher()),
+          rules_store.query(m.enclosing_node()),
           false,
         ) {
           // Generate the scope query for the specific context by substituting the
           // the tags with code snippets appropriately in the `generator` query.
-          return m.generator().instantiate(p_match.matches());
+          return m.scope().instantiate(p_match.matches());
         }
       }
       if let Some(parent) = changed_node.parent() {
         changed_node = parent;
       } else {
         break;
       }
```

### Comparing `polyglot_piranha-0.3.3/src/models/source_code_unit.rs` & `polyglot_piranha-0.3.4/src/models/source_code_unit.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/models/unit_tests/piranha_arguments_test.rs` & `polyglot_piranha-0.3.4/src/models/unit_tests/piranha_arguments_test.rs`

 * *Files 21% similar despite different names*

```diff
@@ -12,30 +12,32 @@
 */
 
 use crate::{
   models::{default_configs::JAVA, language::PiranhaLanguage},
   tests::substitutions,
 };
 
+use super::PiranhaArgumentsBuilder;
+
 #[test]
 #[should_panic(expected = "Invalid Piranha Argument. Missing `path_to_codebase` or `code_snippet`")]
 fn piranha_argument_invalid_no_codebase_and_snippet() {
-  let _ = piranha_arguments! {
-    path_to_configurations = "some/path".to_string(),
-    language = PiranhaLanguage::from(JAVA),
-    substitutions = substitutions! {"super_interface_name" => "SomeInterface"},
-  };
+  let _ = PiranhaArgumentsBuilder::default()
+    .path_to_configurations("some/path".to_string())
+    .language(PiranhaLanguage::from(JAVA))
+    .substitutions(substitutions! {"super_interface_name" => "SomeInterface"})
+    .build();
 }
 
 #[test]
 #[should_panic(
   expected = "Invalid Piranha arguments. Please either specify the `path_to_codebase` or the `code_snippet`. Not Both."
 )]
 fn piranha_argument_invalid_both_codebase_and_snippet() {
-  let _ = piranha_arguments! {
-    path_to_configurations = "some/path".to_string(),
-    path_to_codebase = "dev/null".to_string(),
-    code_snippet = "class A { }".to_string(),
-    language = PiranhaLanguage::from(JAVA),
-    substitutions = substitutions! {"super_interface_name" => "SomeInterface"},
-  };
+  let _ = PiranhaArgumentsBuilder::default()
+    .path_to_configurations("some/path".to_string())
+    .path_to_codebase("dev/null".to_string())
+    .code_snippet("class A { }".to_string())
+    .language(PiranhaLanguage::from(JAVA))
+    .substitutions(substitutions! {"super_interface_name" => "SomeInterface"})
+    .build();
 }
```

### Comparing `polyglot_piranha-0.3.3/src/models/unit_tests/rule_test.rs` & `polyglot_piranha-0.3.4/src/models/unit_tests/rule_test.rs`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
  <p>Unless required by applicable law or agreed to in writing, software distributed under the
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 use crate::{
-  constraint,
+  filter,
   models::{default_configs::UNUSED_CODE_PATH, piranha_arguments::PiranhaArgumentsBuilder},
   utilities::eq_without_whitespace,
 };
 
 use super::InstantiatedRule;
 use {
   crate::models::{rule_store::RuleStore, source_code_unit::SourceCodeUnit},
@@ -74,18 +74,18 @@
     ((local_variable_declaration
       declarator: (variable_declarator
           name: (_) @variable_name
           value: [(true) (false)] @init)) @variable_declaration)
      )",
     replace_node = "variable_declaration",
     replace = "",
-    constraints =[
-        constraint! {
-          matcher= "(method_declaration) @md",
-          queries = [
+    filters =[
+        filter! {
+          enclosing_node= "(method_declaration) @md",
+          not_contains = [
             "(
               ((assignment_expression
                 left: (_) @a.lhs
                 right: (_) @a.rhs) @assignment)
               (#eq? @a.lhs \"@variable_name\")
               (#not-eq? @a.rhs \"@init\")
             )",
@@ -135,17 +135,17 @@
       ((local_variable_declaration
         declarator: (variable_declarator
           name: (_) @variable_name
           value: [(true) (false)] @init)) @variable_declaration)
       )",
     replace_node = "variable_declaration",
     replace = "",
-    constraints =  [constraint! {
-          matcher= "(method_declaration) @md",
-          queries = [
+    filters =  [filter! {
+          enclosing_node= "(method_declaration) @md",
+          not_contains = [
             "(
               ((assignment_expression
                 left: (_) @a.lhs
                 right: (_) @a.rhs) @assignment)
               (#eq? @a.lhs \"@variable_name\")
               (#not-eq? @a.rhs \"@init\")
             )",
```

### Comparing `polyglot_piranha-0.3.3/src/models/unit_tests/scopes_test.rs` & `polyglot_piranha-0.3.4/src/models/unit_tests/scopes_test.rs`

 * *Files 3% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     utilities::eq_without_whitespace,
   },
   std::{collections::HashMap, path::PathBuf},
 };
 
 fn _get_class_scope() -> ScopeGenerator {
   let scope_query_generator_class: ScopeQueryGenerator = ScopeQueryGeneratorBuilder::default()
-    .matcher(TSQuery::new(
+    .enclosing_node(TSQuery::new(
       "(class_declaration name:(_) @n) @c".to_string(),
     ))
-    .generator(TSQuery::new(
+    .scope(TSQuery::new(
       "(
       ((class_declaration name:(_) @z) @qc)
       (#eq? @z \"@n\")
     )"
       .to_string(),
     ))
     .build()
@@ -60,26 +60,26 @@
     .rules(vec![scope_query_generator_class])
     .build()
     .unwrap()
 }
 
 fn _get_method_scope() -> ScopeGenerator {
   let scope_query_generator_method: ScopeQueryGenerator = ScopeQueryGeneratorBuilder::default()
-    .matcher(TSQuery::new(
+    .enclosing_node(TSQuery::new(
       "(
     [(method_declaration 
               name : (_) @n
               parameters : (formal_parameters)@fp)
      (constructor_declaration 
               name: (_) @n
               parameters : (formal_parameters)@fp)
     ]@xdn)"
         .to_string(),
     ))
-    .generator(TSQuery::new(
+    .scope(TSQuery::new(
       "(
       [(((method_declaration 
                 name : (_) @z
                 parameters : (formal_parameters)@tp))
         (#eq? @z \"@n\")
         (#eq? @tp \"@fp\")                  
         )
```

### Comparing `polyglot_piranha-0.3.3/src/tests/mod.rs` & `polyglot_piranha-0.3.4/src/tests/mod.rs`

 * *Files 7% similar despite different names*

```diff
@@ -172,22 +172,22 @@
     $(
     #[test]
     fn $test_name() {
       super::initialize();
       let _path= std::path::PathBuf::from("test-resources").join($language).join($path_to_test);
       let path_to_codebase = _path.join("input").to_str().unwrap().to_string();
       let path_to_configurations = _path.join("configurations").to_str().unwrap().to_string();
-      let piranha_arguments =  $crate::models::piranha_arguments::piranha_arguments!{
-        path_to_codebase = path_to_codebase,
-        path_to_configurations = path_to_configurations,
-        language= $crate::models::language::PiranhaLanguage::from($language),
+      let piranha_arguments =  $crate::models::piranha_arguments::PiranhaArgumentsBuilder::default()
+        .path_to_codebase(path_to_codebase)
+        .path_to_configurations(path_to_configurations)
+        .language($crate::models::language::PiranhaLanguage::from($language))
         $(
-          $kw = $value,
+          .$kw($value)
         )*
-      };
+      .build();
       let output_summaries = $crate::execute_piranha(&piranha_arguments);
       super::assert_frequency_for_matches(&output_summaries, &$matches_frequency);
     }
   )*
   };
 }
 
@@ -215,22 +215,22 @@
     $(
     #[test]
     fn $test_name() {
       super::initialize();
       let _path= std::path::PathBuf::from("test-resources").join($language).join($path_to_test);
       let temp_dir= super::copy_folder_to_temp_dir(&_path.join("input"));
 
-      let piranha_arguments =  $crate::models::piranha_arguments::piranha_arguments!{
-        path_to_codebase = temp_dir.path().to_str().unwrap().to_string(),
-        path_to_configurations = _path.join("configurations").to_str().unwrap().to_string(),
-        language= $crate::models::language::PiranhaLanguage::from($language),
+      let piranha_arguments =  $crate::models::piranha_arguments::PiranhaArgumentsBuilder::default()
+        .path_to_codebase(temp_dir.path().to_str().unwrap().to_string())
+        .path_to_configurations(_path.join("configurations").to_str().unwrap().to_string())
+        .language($crate::models::language::PiranhaLanguage::from($language))
         $(
-          $kw = $value,
+          .$kw($value)
         )*
-      };
+      .build();
 
       super::execute_piranha_and_check_result(&piranha_arguments, &_path.join("expected"), $files_changed, true);
       // Delete temp_dir
       _ = temp_dir.close().unwrap();
     }
   )*
   };
```

### Comparing `polyglot_piranha-0.3.3/src/tests/test_piranha_go.rs` & `polyglot_piranha-0.3.4/src/tests/test_piranha_go.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/tests/test_piranha_java.rs` & `polyglot_piranha-0.3.4/src/tests/test_piranha_java.rs`

 * *Files 24% similar despite different names*

```diff
@@ -7,22 +7,24 @@
 
  <p>Unless required by applicable law or agreed to in writing, software distributed under the
  License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either
  express or implied. See the License for the specific language governing permissions and
  limitations under the License.
 */
 
+use glob::Pattern;
+
 use super::{
   copy_folder_to_temp_dir, create_match_tests, create_rewrite_tests,
   execute_piranha_and_check_result, initialize, substitutions,
 };
 use crate::{
-  constraint, edges, execute_piranha,
+  edges, execute_piranha, filter,
   models::{
-    default_configs::JAVA, language::PiranhaLanguage, piranha_arguments::piranha_arguments,
+    default_configs::JAVA, language::PiranhaLanguage, piranha_arguments::PiranhaArgumentsBuilder,
     rule_graph::RuleGraphBuilder,
   },
   piranha_rule,
   utilities::eq_without_whitespace,
 };
 use std::{collections::HashMap, path::PathBuf};
 
@@ -62,52 +64,65 @@
   test_user_option_delete_if_empty: "user_option_delete_if_empty", 1;
   test_user_option_do_not_delete_if_empty : "user_option_do_not_delete_if_empty", 1, delete_file_if_empty =false;
   test_new_line_character_used_in_string_literal:  "new_line_character_used_in_string_literal",   1;
 }
 
 create_match_tests! {
   JAVA,
-  test_java_match_only: "structural_find", HashMap::from([("find_enum_constant", 1), ("find_method", 1), ("replace_isToggleEnabled_with_boolean_literal", 20)]);
+  test_java_match_only: "structural_find",
+              HashMap::from([
+                  ("find_enum_constant", 1),
+                  ("find_method", 1),
+                  ("replace_isToggleEnabled_with_boolean_literal", 20)
+                  ]);
+  test_java_match_only_with_include_exclude: "structural_find_with_include_exclude",
+              HashMap::from([
+                  ("find_enum_constant", 1),
+                  ("find_method", 1),
+                  ("replace_isToggleEnabled_with_boolean_literal", 20)
+                  ]),
+              include = vec![Pattern::new("*/folder_2/**/*").unwrap()],
+              exclude = vec![Pattern::new("*/folder_2_1/**/*").unwrap()];
 }
 
 #[test]
 #[should_panic(
   expected = "Could not instantiate the rule Rule { name: \"find_interface_extension\""
 )]
 fn test_scenarios_find_and_propagate_panic() {
   initialize();
   let _path = PathBuf::from("test-resources")
     .join(JAVA)
     .join("find_and_propagate");
   let path_to_codebase = _path.join("input").to_str().unwrap().to_string();
   let path_to_configurations = _path.join("configurations").to_str().unwrap().to_string();
-  let piranha_arguments = piranha_arguments! {
-    path_to_codebase = path_to_codebase,
-    path_to_configurations = path_to_configurations,
-    language = PiranhaLanguage::from(JAVA),
-  };
+  let piranha_arguments = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(path_to_codebase)
+    .path_to_configurations(path_to_configurations)
+    .language(PiranhaLanguage::from(JAVA))
+    .build();
 
   let _ = execute_piranha(&piranha_arguments);
 }
 
 #[test]
 #[should_panic(expected = "Could not instantiate the rule Rule { name: \"delete_class\"")]
 fn test_scenarios_find_and_propagate_invalid_substitutions_panic() {
   initialize();
   let _path = PathBuf::from("test-resources")
     .join(JAVA)
     .join("find_and_propagate_invalid_substitutions");
   let path_to_codebase = _path.join("input").to_str().unwrap().to_string();
   let path_to_configurations = _path.join("configurations").to_str().unwrap().to_string();
-  let piranha_arguments = piranha_arguments! {
-    path_to_codebase = path_to_codebase,
-    path_to_configurations = path_to_configurations,
-    language = PiranhaLanguage::from(JAVA),
-    substitutions = substitutions! {"super_interface_name" => "SomeInterface"},
-  };
+  let piranha_arguments = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(path_to_codebase)
+    .path_to_configurations(path_to_configurations)
+    .language(PiranhaLanguage::from(JAVA))
+    .substitutions(substitutions! {"super_interface_name" => "SomeInterface"})
+    .build();
 
   let _ = execute_piranha(&piranha_arguments);
 }
 
 #[test]
 fn test_user_option_delete_consecutive_lines() {
   let _path = PathBuf::from("test-resources")
@@ -124,20 +139,26 @@
     .join("new_line_character_used_in_string_literal");
   let code_snippet = "package com.uber.piranha;
   class SomeClass {
     void someMethod(String s) {
       assert (s.equals(\"Hello \\n World\"));
     }
   }";
-  let piranha_arguments = piranha_arguments! {
-    path_to_configurations = path_to_scenario.join("configurations").to_str().unwrap().to_string(),
-    language = PiranhaLanguage::from(JAVA),
-    dry_run = true,
-    code_snippet = code_snippet.to_string(),
-  };
+  let piranha_arguments = PiranhaArgumentsBuilder::default()
+    .path_to_configurations(
+      path_to_scenario
+        .join("configurations")
+        .to_str()
+        .unwrap()
+        .to_string(),
+    )
+    .language(PiranhaLanguage::from(JAVA))
+    .dry_run(true)
+    .code_snippet(code_snippet.to_string())
+    .build();
 
   let expected = "package com.uber.piranha;
   class SomeClass {
     void someMethod(String s) {
       assert (\"Hello \\n World\".equals(s));
     }
   }";
@@ -161,20 +182,26 @@
 fn _helper_user_option_delete_consecutive_lines(
   path_to_scenario: PathBuf, delete_consecutive_new_lines: bool,
 ) {
   initialize();
 
   let temp_dir = copy_folder_to_temp_dir(&path_to_scenario.join("input"));
 
-  let piranha_arguments = piranha_arguments! {
-    path_to_codebase = temp_dir.path().to_str().unwrap().to_string(),
-    path_to_configurations = path_to_scenario.join("configurations").to_str().unwrap().to_string(),
-    language = PiranhaLanguage::from(JAVA),
-    delete_consecutive_new_lines = delete_consecutive_new_lines,
-  };
+  let piranha_arguments = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(temp_dir.path().to_str().unwrap().to_string())
+    .path_to_configurations(
+      path_to_scenario
+        .join("configurations")
+        .to_str()
+        .unwrap()
+        .to_string(),
+    )
+    .language(PiranhaLanguage::from(JAVA))
+    .delete_consecutive_new_lines(delete_consecutive_new_lines)
+    .build();
 
   execute_piranha_and_check_result(
     &piranha_arguments,
     &path_to_scenario.join("expected"),
     1,
     false,
   );
@@ -202,18 +229,18 @@
       replace_node = "class_body",
       replace = "{
         @class_members
         public class InnerFooBar {  
             private String name;
         }  
         }",
-      constraints = [
-        constraint! {
-          matcher = "(class_declaration ) @c_cd",
-          queries = ["(
+      filters = [
+        filter! {
+          enclosing_node =  "(class_declaration ) @c_cd",
+          not_contains = ["(
             (class_declaration name:(_) @name ) @cd
             (#eq? @name \"InnerFooBar\")
             )",]
         }
       ]
     },
     piranha_rule! {
@@ -222,40 +249,42 @@
         (class_declaration name: (_)@class_name
             body : (class_body ((_)*) @class_members)  @class_body
          ) @class_declaration
         )",
       replace_node = "class_body",
       replace = "{\n private String address;\n @class_members \n}",
       is_seed_rule= false,
-      constraints = [
-        constraint! {
-          matcher = "(class_declaration ) @c_cd",
-          queries = ["(
+      filters = [
+        filter! {
+          enclosing_node =  "(class_declaration ) @c_cd",
+          not_contains = ["(
           (field_declaration (variable_declarator name:(_) @name )) @field
           (#eq? @name \"address\")
           )",]
         }
       ]
     },
   ];
 
   let edges = vec![edges! {
     from = "add_inner_class",
     to = ["add_field_declaration"],
     scope = "Class"
   }];
 
-  let args = piranha_arguments! {
-    path_to_codebase = temp_dir.path().to_str().unwrap().to_string(),
-    language = PiranhaLanguage::from(JAVA),
-    rule_graph = RuleGraphBuilder::default()
-                .rules(rules)
-                .edges(edges)
-                .build(),
-  };
+  let args = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(temp_dir.path().to_str().unwrap().to_string())
+    .language(PiranhaLanguage::from(JAVA))
+    .rule_graph(
+      RuleGraphBuilder::default()
+        .rules(rules)
+        .edges(edges)
+        .build(),
+    )
+    .build();
 
   execute_piranha_and_check_result(&args, _path.join("expected").as_path(), 1, true)
 }
 
 /// This test is to check if Piranha is able to handle a syntactically incorrect tree.
 #[test]
 fn test_handle_syntactically_incorrect_tree() {
@@ -270,22 +299,20 @@
   (variable_declarator value: (decimal_integer_literal) @value)
   (#not-match? @value \"l|L\")
   )",
     replace_node = "value",
     replace = "@valuel"
   };
 
-  let piranha_arguments = piranha_arguments! {
-    path_to_codebase = temp_dir.path().to_str().unwrap().to_string(),
-    language = PiranhaLanguage::from(JAVA),
-    rule_graph = RuleGraphBuilder::default()
-                .rules(vec![rule])
-                .build(),
-    allow_dirty_ast = true,
-  };
+  let piranha_arguments = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(temp_dir.path().to_str().unwrap().to_string())
+    .language(PiranhaLanguage::from(JAVA))
+    .rule_graph(RuleGraphBuilder::default().rules(vec![rule]).build())
+    .allow_dirty_ast(true)
+    .build();
 
   execute_piranha_and_check_result(&piranha_arguments, &_path.join("expected"), 1, true);
   // Delete temp_dir
   temp_dir.close().unwrap();
 }
 
 /// This test is to check if Piranha panics when it encounters a syntactically incorrect tree and
@@ -304,21 +331,19 @@
   (variable_declarator value: (decimal_integer_literal) @value)
   (#not-match? @value \"l|L\")
   )",
     replace_node = "value",
     replace = "@valuel"
   };
 
-  let piranha_arguments = piranha_arguments! {
-    path_to_codebase = temp_dir.path().to_str().unwrap().to_string(),
-    language = PiranhaLanguage::from(JAVA),
-    rule_graph = RuleGraphBuilder::default()
-                .rules(vec![rule])
-                .build(),
-  };
+  let piranha_arguments = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(temp_dir.path().to_str().unwrap().to_string())
+    .language(PiranhaLanguage::from(JAVA))
+    .rule_graph(RuleGraphBuilder::default().rules(vec![rule]).build())
+    .build();
 
   execute_piranha_and_check_result(&piranha_arguments, &_path.join("expected"), 1, true);
   // Delete temp_dir
   temp_dir.close().unwrap();
 }
 
 /// This test is to check if Piranha is able to handle a syntactically incorrect tree.
@@ -338,19 +363,17 @@
   (#not-match? @value \"X|x\")
   )",
     replace_node = "value",
     // Purposefully appending `x` so that it results in a incorrect syntax tree.
     replace = "@valuex"
   };
 
-  let piranha_arguments = piranha_arguments! {
-    path_to_codebase = temp_dir.path().to_str().unwrap().to_string(),
-    language = PiranhaLanguage::from(JAVA),
-    rule_graph = RuleGraphBuilder::default()
-                .rules(vec![rule])
-                .build(),
-  };
+  let piranha_arguments = PiranhaArgumentsBuilder::default()
+    .path_to_codebase(temp_dir.path().to_str().unwrap().to_string())
+    .language(PiranhaLanguage::from(JAVA))
+    .rule_graph(RuleGraphBuilder::default().rules(vec![rule]).build())
+    .build();
 
   execute_piranha_and_check_result(&piranha_arguments, &_path.join("expected"), 1, true);
   // Delete temp_dir
   temp_dir.close().unwrap();
 }
```

### Comparing `polyglot_piranha-0.3.3/src/tests/test_piranha_kt.rs` & `polyglot_piranha-0.3.4/src/tests/test_piranha_kt.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/tests/test_piranha_python.rs` & `polyglot_piranha-0.3.4/src/tests/test_piranha_python.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/tests/test_piranha_thrift.rs` & `polyglot_piranha-0.3.4/src/tests/test_piranha_thrift.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/tests/test_piranha_ts.rs` & `polyglot_piranha-0.3.4/src/tests/test_piranha_ts.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/tests/test_piranha_tsx.rs` & `polyglot_piranha-0.3.4/src/tests/test_piranha_tsx.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/utilities/mod.rs` & `polyglot_piranha-0.3.4/src/utilities/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,20 @@
 ) -> Result<(String, String), Box<dyn Error + Send + Sync + 'static>> {
   let pos = s
     .find('=')
     .ok_or_else(|| format!("invalid KEY=value: no `=` found in `{s}`"))?;
   Ok((s[..pos].parse()?, s[pos + 1..].parse()?))
 }
 
+pub(crate) fn parse_glob_pattern(
+  s: &str,
+) -> Result<Pattern, Box<dyn Error + Send + Sync + 'static>> {
+  Ok(Pattern::new(s)?)
+}
+
 /// Returns the file with the given name within the given directory.
 #[cfg(test)] // Rust analyzer FP
 pub(crate) fn find_file(input_dir: &PathBuf, name: &str) -> PathBuf {
   fs::read_dir(input_dir)
     .unwrap()
     .filter_map(|d| d.ok())
     .find(|de| has_name(de, name))
@@ -135,14 +141,15 @@
     fn __str__(&self) -> String {
       self.__repr__()
     }
   };
 }
 
 pub(crate) use gen_py_str_methods;
+use glob::Pattern;
 
 use self::tree_sitter_utilities::TSQuery;
 
 pub(crate) trait Instantiate {
   /// Replaces the all the occurrences of a tree-sitter specific tag with the corresponding string values
   /// specified in `substitutions`
   ///
```

### Comparing `polyglot_piranha-0.3.3/src/utilities/tree_sitter_utilities.rs` & `polyglot_piranha-0.3.4/src/utilities/tree_sitter_utilities.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/utilities/unit_tests/tree_sitter_utilities_test.rs` & `polyglot_piranha-0.3.4/src/utilities/unit_tests/tree_sitter_utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/src/utilities/unit_tests/utilities_test.rs` & `polyglot_piranha-0.3.4/src/utilities/unit_tests/utilities_test.rs`

 * *Files identical despite different names*

### Comparing `polyglot_piranha-0.3.3/PKG-INFO` & `polyglot_piranha-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: polyglot_piranha
-Version: 0.3.3
+Version: 0.3.4
 License-File: LICENSE
 License-File: LICENSE
 License-File: NOTICE
 Summary: Polyglot Piranha is a library for performing structural find and replace with deep cleanup.
 Keywords: refactoring,code update,structural find-replace,structural search and replace,structural search
 Author: Uber Technologies Inc.
 Author-email: Ameya Ketkar <ketkara@uber.com>, Lazaro Clapp <lazaro@uber.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/uber/piranha
 Project-URL: homepage, https://github.com/uber/piranha
 Project-URL: documentation, https://github.com/uber/piranha
+Project-URL: repository, https://github.com/uber/piranha
 
 # Piranha
 
 [![Join the chat at https://gitter.im/uber/piranha](https://badges.gitter.im/uber/piranha.svg)](https://gitter.im/uber/piranha?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 
 Feature flags are commonly used to enable gradual rollout or experiment with new features. In a few cases, even after the purpose of the flag is accomplished, the code pertaining to the feature flag is not removed. We refer to such flags as stale flags. The presence of code pertaining to stale flags can have the following drawbacks: 
 - Unnecessary code clutter increases the overall complexity w.r.t maintenance resulting in reduced developer productivity
```

