# Comparing `tmp/qm_qua-1.1.1.tar.gz` & `tmp/qm_qua-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qm_qua-1.1.1.tar", max compression
+gzip compressed data, was "qm_qua-1.1.2.tar", max compression
```

## Comparing `qm_qua-1.1.1.tar` & `qm_qua-1.1.2.tar`

### file list

```diff
@@ -1,136 +1,135 @@
--rw-r--r--   0        0        0    11914 2023-03-20 18:30:05.640746 qm_qua-1.1.1/CHANGELOG.md
--rw-r--r--   0        0        0    14988 2023-03-20 18:30:05.640746 qm_qua-1.1.1/LICENSE
--rw-r--r--   0        0        0      453 2023-03-20 18:30:05.640746 qm_qua-1.1.1/README.md
--rw-r--r--   0        0        0     4883 2023-03-20 18:30:55.324612 qm_qua-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      209 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/QmJob.py
--rw-r--r--   0        0        0      246 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/QmPendingJob.py
--rw-r--r--   0        0        0      220 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/QmQueue.py
--rw-r--r--   0        0        0      313 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/QuaNodeVisitor.py
--rw-r--r--   0        0        0    33244 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/QuantumMachine.py
--rw-r--r--   0        0        0    11629 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/QuantumMachinesManager.py
--rw-r--r--   0        0        0     1592 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/StreamMetadata.py
--rw-r--r--   0        0        0     9023 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/_QmJobErrors.py
--rw-r--r--   0        0        0     1651 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/__init__.py
--rw-r--r--   0        0        0      246 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/_controller.py
--rw-r--r--   0        0        0      321 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/_loc.py
--rw-r--r--   0        0        0      716 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/_pretty_errors.py
--rw-r--r--   0        0        0      779 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/_python_to_pb.py
--rw-r--r--   0        0        0     2331 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/_report.py
--rw-r--r--   0        0        0      499 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/_results.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/__init__.py
--rw-r--r--   0        0        0     4582 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/base_api.py
--rw-r--r--   0        0        0    16894 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/frontend_api.py
--rw-r--r--   0        0        0      983 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/info_service_api.py
--rw-r--r--   0        0        0     8323 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/job_manager_api.py
--rw-r--r--   0        0        0     3522 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/job_result_api.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/__init__.py
--rw-r--r--   0        0        0     1875 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/capabilities.py
--rw-r--r--   0        0        0      553 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/compiler.py
--rw-r--r--   0        0        0      484 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/debug_data.py
--rw-r--r--   0        0        0      836 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/devices.py
--rw-r--r--   0        0        0      252 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/info.py
--rw-r--r--   0        0        0      272 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/jobs.py
--rw-r--r--   0        0        0      170 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/quantum_machine.py
--rw-r--r--   0        0        0     1163 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/models/server_details.py
--rw-r--r--   0        0        0     3329 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/server_detector.py
--rw-r--r--   0        0        0     6274 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/simulation_api.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/stubs/__init__.py
--rw-r--r--   0        0        0     2076 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/api/stubs/deprecated_job_manager_stub.py
--rw-r--r--   0        0        0      296 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/capabilities.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/containers/__init__.py
--rw-r--r--   0        0        0      866 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/containers/capabilities_container.py
--rw-r--r--   0        0        0     1809 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/datadog_api.py
--rw-r--r--   0        0        0     1281 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/devices.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/elements/__init__.py
--rw-r--r--   0        0        0     4336 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/elements/basic_element.py
--rw-r--r--   0        0        0     8351 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/elements/element_with_octave.py
--rw-r--r--   0        0        0     6467 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/elements/native_elements.py
--rw-r--r--   0        0        0     9300 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/elements_db.py
--rw-r--r--   0        0        0     2095 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/__init__.py
--rw-r--r--   0        0        0     2070 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/compiler/__init__.py
--rw-r--r--   0        0        0     1054 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/errors/__init__.py
--rw-r--r--   0        0        0    67465 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/frontend/__init__.py
--rw-r--r--   0        0        0      723 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/general_messages/__init__.py
--rw-r--r--   0        0        0     8255 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/job_manager/__init__.py
--rw-r--r--   0        0        0     3128 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/octave_models/__init__.py
--rw-r--r--   0        0        0     8463 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/qm_api/__init__.py
--rw-r--r--   0        0        0     3735 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/qm_manager/__init__.py
--rw-r--r--   0        0        0    31736 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/qua/__init__.py
--rw-r--r--   0        0        0    20175 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/qua_config/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:52.988619 qm_qua-1.1.1/qm/grpc/quantum_simulator/__init__.py
--rw-r--r--   0        0        0    11363 2023-03-20 18:30:52.988619 qm_qua-1.1.1/qm/grpc/quantum_simulator/v1/__init__.py
--rw-r--r--   0        0        0    22458 2023-03-20 18:30:51.348624 qm_qua-1.1.1/qm/grpc/results_analyser/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:54.432614 qm_qua-1.1.1/qm/io/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:54.432614 qm_qua-1.1.1/qm/io/qualang/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:54.432614 qm_qua-1.1.1/qm/io/qualang/api/__init__.py
--rw-r--r--   0        0        0     2363 2023-03-20 18:30:54.432614 qm_qua-1.1.1/qm/io/qualang/api/v1/__init__.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:05.912746 qm_qua-1.1.1/qm/jobs/__init__.py
--rw-r--r--   0        0        0     3617 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/jobs/base_job.py
--rw-r--r--   0        0        0     8871 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/jobs/job_queue.py
--rw-r--r--   0        0        0     3388 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/jobs/pending_job.py
--rw-r--r--   0        0        0       86 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/jobs/qm_job.py
--rw-r--r--   0        0        0     4411 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/jobs/running_qm_job.py
--rw-r--r--   0        0        0    10439 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/jobs/simulated_job.py
--rw-r--r--   0        0        0      395 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/logger.py
--rw-r--r--   0        0        0      772 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/logging_utils.py
--rw-r--r--   0        0        0      515 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/octave/__init__.py
--rw-r--r--   0        0        0     7763 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/octave/_calibration_config.py
--rw-r--r--   0        0        0    13378 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/octave/_calibration_program.py
--rw-r--r--   0        0        0     5618 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/octave/calibration_db.py
--rw-r--r--   0        0        0      675 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/octave/enums.py
--rw-r--r--   0        0        0    10312 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/octave/octave_config.py
--rw-r--r--   0        0        0    22126 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/octave/octave_manager.py
--rw-r--r--   0        0        0     9047 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/octave/qm_octave.py
--rw-r--r--   0        0        0     1859 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/persistence.py
--rw-r--r--   0        0        0    15334 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/ConfigBuilder.py
--rw-r--r--   0        0        0    17971 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/StatementsCollection.py
--rw-r--r--   0        0        0      235 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/_Program.py
--rw-r--r--   0        0        0     2915 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/_ResultAnalysis.py
--rw-r--r--   0        0        0      167 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/__init__.py
--rw-r--r--   0        0        0     1262 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/_execution_overrides_schema.py
--rw-r--r--   0        0        0    48008 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/_qua_config_schema.py
--rw-r--r--   0        0        0    23373 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/_qua_config_to_pb.py
--rw-r--r--   0        0        0     3371 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/_validate_config_schema.py
--rw-r--r--   0        0        0     4870 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/expressions.py
--rw-r--r--   0        0        0     3835 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/program/program.py
--rw-r--r--   0        0        0     3648 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/qua/AnalogMeasureProcess.py
--rw-r--r--   0        0        0      718 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/qua/DigitalMeasureProcess.py
--rw-r--r--   0        0        0       67 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/qua/__init__.py
--rw-r--r--   0        0        0   127476 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/qua/_dsl.py
--rw-r--r--   0        0        0     2753 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/qua/_type_hinting.py
--rw-r--r--   0        0        0    15149 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/qua/lib.py
--rw-r--r--   0        0        0      243 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/results/__init__.py
--rw-r--r--   0        0        0    12589 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/results/base_streaming_result_fetcher.py
--rw-r--r--   0        0        0     5903 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/results/multiple_streaming_result_fetcher.py
--rw-r--r--   0        0        0     1951 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/results/simulator_samples.py
--rw-r--r--   0        0        0     2725 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/results/single_streaming_result_fetcher.py
--rw-r--r--   0        0        0     8236 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/results/streaming_result_fetcher.py
--rw-r--r--   0        0        0        0 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/serialization/__init__.py
--rw-r--r--   0        0        0    14445 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/serialization/expression_serializing_visitor.py
--rw-r--r--   0        0        0     9577 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/serialization/generate_qua_script.py
--rw-r--r--   0        0        0     2068 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/serialization/qua_node_visitor.py
--rw-r--r--   0        0        0    25507 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/serialization/qua_serializing_visitor.py
--rw-r--r--   0        0        0      216 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/simulate/__init__.py
--rw-r--r--   0        0        0     1685 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/simulate/credentials.py
--rw-r--r--   0        0        0     3308 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/simulate/interface.py
--rw-r--r--   0        0        0     3667 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/simulate/loopback.py
--rw-r--r--   0        0        0      840 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/simulate/quantum.py
--rw-r--r--   0        0        0     2301 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/simulate/raw.py
--rw-r--r--   0        0        0      504 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/singleton.py
--rw-r--r--   0        0        0    14456 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/sources/logo_qm_square.png
--rw-r--r--   0        0        0      244 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/type_hinting/__init__.py
--rw-r--r--   0        0        0     4881 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/type_hinting/config_types.py
--rw-r--r--   0        0        0      240 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/type_hinting/exceution_overrides.py
--rw-r--r--   0        0        0      537 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/type_hinting/general.py
--rw-r--r--   0        0        0     1960 2023-03-20 18:30:05.916746 qm_qua-1.1.1/qm/type_hinting/simulator_types.py
--rw-r--r--   0        0        0     5045 2023-03-20 18:30:05.920745 qm_qua-1.1.1/qm/user_config.py
--rw-r--r--   0        0        0      846 2023-03-20 18:30:05.920745 qm_qua-1.1.1/qm/utils/__init__.py
--rw-r--r--   0        0        0      904 2023-03-20 18:30:05.920745 qm_qua-1.1.1/qm/utils/async_utils.py
--rw-r--r--   0        0        0     1559 2023-03-20 18:30:05.920745 qm_qua-1.1.1/qm/utils/deprecation_utils.py
--rw-r--r--   0        0        0     1388 2023-03-20 18:30:05.920745 qm_qua-1.1.1/qm/utils/general_utils.py
--rw-r--r--   0        0        0      945 2023-03-20 18:30:05.920745 qm_qua-1.1.1/qm/utils/protobuf_utils.py
--rw-r--r--   0        0        0     2156 2023-03-20 18:30:05.920745 qm_qua-1.1.1/qm/utils/types_utils.py
--rw-r--r--   0        0        0       22 2023-03-20 18:30:55.328611 qm_qua-1.1.1/qm/version.py
--rw-r--r--   0        0        0    33236 2023-03-20 18:30:05.920745 qm_qua-1.1.1/qm/waveform_report.py
--rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 qm_qua-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    13079 2023-05-11 10:31:12.068640 qm_qua-1.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0    14988 2023-05-11 10:31:12.068640 qm_qua-1.1.2/LICENSE
+-rw-r--r--   0        0        0      453 2023-05-11 10:31:12.068640 qm_qua-1.1.2/README.md
+-rw-r--r--   0        0        0     5346 2023-05-11 10:32:25.829000 qm_qua-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QmJob.py
+-rw-r--r--   0        0        0      247 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QmPendingJob.py
+-rw-r--r--   0        0        0      221 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QmQueue.py
+-rw-r--r--   0        0        0      307 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QuaNodeVisitor.py
+-rw-r--r--   0        0        0    34119 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QuantumMachine.py
+-rw-r--r--   0        0        0      295 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/QuantumMachinesManager.py
+-rw-r--r--   0        0        0     2043 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/StreamMetadata.py
+-rw-r--r--   0        0        0     9601 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_QmJobErrors.py
+-rw-r--r--   0        0        0     1629 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/__init__.py
+-rw-r--r--   0        0        0      246 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_controller.py
+-rw-r--r--   0        0        0      316 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_loc.py
+-rw-r--r--   0        0        0     2446 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_report.py
+-rw-r--r--   0        0        0      483 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/_results.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.352642 qm_qua-1.1.2/qm/api/__init__.py
+-rw-r--r--   0        0        0     4549 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/base_api.py
+-rw-r--r--   0        0        0    17062 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/frontend_api.py
+-rw-r--r--   0        0        0      983 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/info_service_api.py
+-rw-r--r--   0        0        0     8290 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/job_manager_api.py
+-rw-r--r--   0        0        0     3500 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/job_result_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/__init__.py
+-rw-r--r--   0        0        0     1875 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/capabilities.py
+-rw-r--r--   0        0        0      553 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/compiler.py
+-rw-r--r--   0        0        0      484 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/debug_data.py
+-rw-r--r--   0        0        0      749 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/devices.py
+-rw-r--r--   0        0        0      252 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/info.py
+-rw-r--r--   0        0        0      272 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/jobs.py
+-rw-r--r--   0        0        0      170 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/quantum_machine.py
+-rw-r--r--   0        0        0     1185 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/models/server_details.py
+-rw-r--r--   0        0        0     4641 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/server_detector.py
+-rw-r--r--   0        0        0     6424 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/simulation_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/stubs/__init__.py
+-rw-r--r--   0        0        0     2059 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/api/stubs/deprecated_job_manager_stub.py
+-rw-r--r--   0        0        0      296 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/capabilities.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/communication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/communication/http_redirection.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/containers/__init__.py
+-rw-r--r--   0        0        0      866 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/containers/capabilities_container.py
+-rw-r--r--   0        0        0     1980 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/datadog_api.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements/basic_element.py
+-rw-r--r--   0        0        0     9739 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements/element_with_octave.py
+-rw-r--r--   0        0        0     6528 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements/native_elements.py
+-rw-r--r--   0        0        0     9540 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/elements_db.py
+-rw-r--r--   0        0        0     2538 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/__init__.py
+-rw-r--r--   0        0        0     2070 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/compiler/__init__.py
+-rw-r--r--   0        0        0     1054 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/errors/__init__.py
+-rw-r--r--   0        0        0    67465 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/frontend/__init__.py
+-rw-r--r--   0        0        0      723 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/general_messages/__init__.py
+-rw-r--r--   0        0        0     8255 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/job_manager/__init__.py
+-rw-r--r--   0        0        0     3128 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/octave_models/__init__.py
+-rw-r--r--   0        0        0     8463 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/qm_api/__init__.py
+-rw-r--r--   0        0        0     3735 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/qm_manager/__init__.py
+-rw-r--r--   0        0        0    31736 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/qua/__init__.py
+-rw-r--r--   0        0        0    20057 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/qua_config/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:32:22.448980 qm_qua-1.1.2/qm/grpc/quantum_simulator/__init__.py
+-rw-r--r--   0        0        0    11363 2023-05-11 10:32:22.448980 qm_qua-1.1.2/qm/grpc/quantum_simulator/v1/__init__.py
+-rw-r--r--   0        0        0    22458 2023-05-11 10:32:20.052966 qm_qua-1.1.2/qm/grpc/results_analyser/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:32:24.572993 qm_qua-1.1.2/qm/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:32:24.572993 qm_qua-1.1.2/qm/io/qualang/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:32:24.572993 qm_qua-1.1.2/qm/io/qualang/api/__init__.py
+-rw-r--r--   0        0        0     2363 2023-05-11 10:32:24.572993 qm_qua-1.1.2/qm/io/qualang/api/v1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/__init__.py
+-rw-r--r--   0        0        0     3617 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/base_job.py
+-rw-r--r--   0        0        0     8871 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/job_queue.py
+-rw-r--r--   0        0        0     3284 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/pending_job.py
+-rw-r--r--   0        0        0       86 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/qm_job.py
+-rw-r--r--   0        0        0     4412 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/running_qm_job.py
+-rw-r--r--   0        0        0    10406 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/jobs/simulated_job.py
+-rw-r--r--   0        0        0      395 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/logger.py
+-rw-r--r--   0        0        0      781 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/logging_utils.py
+-rw-r--r--   0        0        0      516 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/__init__.py
+-rw-r--r--   0        0        0     7763 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/_calibration_config.py
+-rw-r--r--   0        0        0    13378 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/_calibration_program.py
+-rw-r--r--   0        0        0     5618 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/calibration_db.py
+-rw-r--r--   0        0        0      675 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/enums.py
+-rw-r--r--   0        0        0    10320 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/octave_config.py
+-rw-r--r--   0        0        0    22068 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/octave_manager.py
+-rw-r--r--   0        0        0     9018 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/octave/qm_octave.py
+-rw-r--r--   0        0        0     1905 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/persistence.py
+-rw-r--r--   0        0        0    15425 2023-05-11 10:31:12.356642 qm_qua-1.1.2/qm/program/ConfigBuilder.py
+-rw-r--r--   0        0        0    17971 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/StatementsCollection.py
+-rw-r--r--   0        0        0      235 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_Program.py
+-rw-r--r--   0        0        0     2915 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_ResultAnalysis.py
+-rw-r--r--   0        0        0      167 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/__init__.py
+-rw-r--r--   0        0        0     1261 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_execution_overrides_schema.py
+-rw-r--r--   0        0        0    47831 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_qua_config_schema.py
+-rw-r--r--   0        0        0    23256 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_qua_config_to_pb.py
+-rw-r--r--   0        0        0     3372 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/_validate_config_schema.py
+-rw-r--r--   0        0        0     4870 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/expressions.py
+-rw-r--r--   0        0        0     3835 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/program/program.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/py.typed
+-rw-r--r--   0        0        0     3648 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/AnalogMeasureProcess.py
+-rw-r--r--   0        0        0      718 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/DigitalMeasureProcess.py
+-rw-r--r--   0        0        0       67 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/__init__.py
+-rw-r--r--   0        0        0   127669 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/_dsl.py
+-rw-r--r--   0        0        0     2755 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/_type_hinting.py
+-rw-r--r--   0        0        0    15150 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/qua/lib.py
+-rw-r--r--   0        0        0    12834 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/quantum_machines_manager.py
+-rw-r--r--   0        0        0      347 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/__init__.py
+-rw-r--r--   0        0        0    13865 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/base_streaming_result_fetcher.py
+-rw-r--r--   0        0        0     6051 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/multiple_streaming_result_fetcher.py
+-rw-r--r--   0        0        0     2987 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/simulator_samples.py
+-rw-r--r--   0        0        0     3236 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/single_streaming_result_fetcher.py
+-rw-r--r--   0        0        0     8438 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/results/streaming_result_fetcher.py
+-rw-r--r--   0        0        0        0 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/__init__.py
+-rw-r--r--   0        0        0    14445 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/expression_serializing_visitor.py
+-rw-r--r--   0        0        0     9577 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/generate_qua_script.py
+-rw-r--r--   0        0        0     2068 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/qua_node_visitor.py
+-rw-r--r--   0        0        0    25507 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/serialization/qua_serializing_visitor.py
+-rw-r--r--   0        0        0      377 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/credentials.py
+-rw-r--r--   0        0        0     3225 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/interface.py
+-rw-r--r--   0        0        0     3549 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/loopback.py
+-rw-r--r--   0        0        0     2896 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/simulate/raw.py
+-rw-r--r--   0        0        0    14456 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/sources/logo_qm_square.png
+-rw-r--r--   0        0        0      243 2023-05-11 10:31:12.360642 qm_qua-1.1.2/qm/type_hinting/__init__.py
+-rw-r--r--   0        0        0     4860 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/type_hinting/config_types.py
+-rw-r--r--   0        0        0      239 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/type_hinting/exceution_overrides.py
+-rw-r--r--   0        0        0      566 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/type_hinting/general.py
+-rw-r--r--   0        0        0     1929 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/type_hinting/simulator_types.py
+-rw-r--r--   0        0        0     5916 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/user_config.py
+-rw-r--r--   0        0        0      789 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/__init__.py
+-rw-r--r--   0        0        0     1089 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/async_utils.py
+-rw-r--r--   0        0        0     1559 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/deprecation_utils.py
+-rw-r--r--   0        0        0     1906 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/general_utils.py
+-rw-r--r--   0        0        0      945 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/protobuf_utils.py
+-rw-r--r--   0        0        0     2614 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/utils/types_utils.py
+-rw-r--r--   0        0        0       22 2023-05-11 10:32:25.829000 qm_qua-1.1.2/qm/version.py
+-rw-r--r--   0        0        0    36595 2023-05-11 10:31:12.364642 qm_qua-1.1.2/qm/waveform_report.py
+-rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 qm_qua-1.1.2/PKG-INFO
```

### Comparing `qm_qua-1.1.1/CHANGELOG.md` & `qm_qua-1.1.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 ## Unreleased
+### Deprecation
+- Moved `qm.QuantumMachinesManager.QuantumMachinesManager` path to `qm.quantum_machines_manager.QuantumMachinesManager`. Old path will be removed in 1.2.0
+
+### Added
+- Added `qmm.validate_qua_config()` for config validation without opening a qm
+- :guardswoman: Added support for getting clusters by name in `QuantumMachinesManager` 
+- Added a `py.typed` file, that marks the package as supporting type-hints.
+- Added a default (minimal) duration for sticky elements
+- Added `qm.get_job(job_id)` to retreieve previously ran jobs
+
+### Fixed
+- Fixed creating credentials for authentication in gRPC
+- Removed redundant entry from element generated class (`up_converted`)
+- Float frequency support - fixed the creation of config classes so integer frequency will always exist
+- Fixed creating a mixer dict-config from protobuf class instance
+- Fixed error raised when fetching saved data in the backwards compatible
+- Fixed creating a digital port dict-config from protobuf class instance
+- Fixed event-loop Windows bug of creating multiple instances of QuantumMachine
+
 
 ## [1.1.1] - 2023-03-20
 ### Fixed
 - Fixed long delay while waiting for values
 
 ## [1.1.0] - 2023-03-16
 
@@ -39,14 +58,15 @@
 - :guardswoman: Extended the sticky capability to include the digital pulse (optional)
 - Added option to validate QUA config with protobuf instead of marshmallow. It is usually faster when working with large configs, to use this feature, set `validate_with_protobuf=True` while opening a quantum machine.
 - Added type hinting for all `qua` functions and programs
 - Added another way of getting results from job results: `job.result_handles["result_name"]`.`
 - Octave reset request command added to "Octave manager".
 - Added support for octave configuration inside the QUA-config dictionary, this will later deprecate the `OctaveConfig` object, which is still supported
 - Added objects that reflects the elements in the `QuantumMachine` instance.
+- :guardswoman: Added the waveform report for better displaying simulation results.
 
 ### Changed
 - Updated `play` docstrings to reflect that the changes to conditional digital pulse.
 - Changed octave's `set_clock` API.
 - Changed and improved internal grpc infrastructure
 - Changed and improved async infrastructure
```

### Comparing `qm_qua-1.1.1/LICENSE` & `qm_qua-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/pyproject.toml` & `qm_qua-1.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,90 @@
 [tool.poetry]
 name = "qm-qua"
-version = "1.1.1"
+version = "1.1.2"
 description = "QUA language SDK to control a Quantum Computer"
 readme = "README.md"
 authors = ["Quantum Machines <info@quantum-machines.co>"]
 
 packages = [
-    { include = "qm" }
+    { include = "qm" },
+    { include = "qm/py.typed" }
 ]
 include = [
     "CHANGELOG.md",
     "LICENSE",
     "qm/io/**/*",
     "qm/grpc/**/*.py",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.7, <3.11"
 grpcio = "^1.39.0"
 protobuf = "^3.17.3"
 betterproto = "2.0.0b5"
 marshmallow = "^3.0.0"
 marshmallow-polyfield = "^5.7"
 numpy = "^1.17.0"
 tinydb = "^4.6.1"
 certifi = { version = "*", optional = true }
-pretty_errors = "^1.2.25"
 datadog-api-client = "^2.6.0"
 deprecation = "^2.1.0"
 dependency_injector = "^4.41.0"
 qm-octave = "^1.1.0"
 
-grpclib = { version = "^0.4.3rc3", python = "^3.10", allow-prereleases = true}
+grpclib = { version = "^0.4.3rc3", python = "^3.10", allow-prereleases = true }
 plotly = "^5.13.0"
+httpx = { version = "^0.23.3", extras = ["http2"] }
 
 [tool.poetry.dev-dependencies]
 grpcio = "1.39.0"
 grpcio-tools = "1.39.0"
 betterproto = { extras = ["compiler"], version = "2.0.0b5" }
 coverage = "^7.0.1"
-pytest-asyncio="^0.20.3"
-pytest-benchmark = { extras = ["aspect"], version = "^4.0.0"}
+pytest-asyncio = "^0.20.3"
+pytest-benchmark = { extras = ["aspect"], version = "^4.0.0" }
 
 black = "^22.6.0"
 flake8 = "^3.9.2"
+importlib-metadata = { version = "^4.0.0", python = "~3.7" }
 pytest = "^7.0.0"
 flake8-bugbear = "^21.11.29"
 poethepoet = "^0.16.0"
 pytest-order = "^1.0.0"
 
 Sphinx = "^4.3.1"
 sphinx-rtd-theme = "^1.0.0"
 sphinxcontrib-redoc = "^1.6.0"
 apispec = "^5.1.1"
 sphinx-toolbox = "^2.15.2"
-poetry-dynamic-versioning = {extras = ["plugin"], version = "^0.21.2"}
+poetry-dynamic-versioning = { extras = ["plugin"], version = "^0.21.2" }
 
 mypy = "^1.1.1"
+isort = "*"
 
 [tool.poetry.extras]
 simulation = ["certifi"]
 
 [tool.black]
 line-length = 120
 target-version = ["py37"]
 extend-exclude = '''
 /(
   | qm/grpc/.*
   | qm/io/.*
 )/
 '''
 
+[tool.isort]
+profile = "black"
+line_length = 120
+length_sort = true
+skip_gitignore = true
+force_sort_within_sections = true
+extra_standard_library = ["typing_extensions"]
 
 
 [tool.poe.tasks]
 
 [tool.poe.tasks.build-docs]
 sequence = [
     { script = "shutil:rmtree('dist/docs', ignore_errors=True)" },
@@ -132,18 +142,25 @@
 script = "os:remove('__init__.py')"
 help = "Remove the root __init__.py file generated by generate-grpc-sim"
 
 [tool.poe.tasks.generate-grpc]
 sequence = ["clean-grpc", "generate-grpc-api", "generate-grpc-sim", "generate-grpc-qua", "generate-grpc-qua-clean", "remove-root-init"]
 help = "Generate gRPC python files"
 
-[tool.poe.tasks.format]
+[tool.poe.tasks.format-black]
 cmd = "black qm"
 help = "Format source files according to the style rules"
 
+[tool.poe.tasks.format-isort]
+cmd = "isort qm"
+help = "Fixes imports"
+
+[tool.poe.tasks.format]
+sequence = ["format-black", "format-isort"]
+
 [tool.poe.tasks.check-links]
 cmd = "sphinx-build -b linkcheck docs_sphinx dist/check-links"
 help = "Checks that the links are valid"
 
 [tool.poe.tasks.check-format]
 cmd = "black qm --check"
 help = "Check that all files are formatted according to the style rules"
```

### Comparing `qm_qua-1.1.1/qm/QuantumMachine.py` & `qm_qua-1.1.2/qm/QuantumMachine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 import json
 import logging
 import warnings
-from typing import Optional, Union, List, Tuple, Dict, Any, cast, Sequence
+from typing import Any, Dict, List, Tuple, Union, Optional, Sequence, cast
 
-from qm.elements.element_with_octave import ElementWithOctave
-from qm.elements.native_elements import (
-    static_set_mixer_correction,
-    SingleInputElement,
-    MixInputsElement,
-)
-from qm.elements_db import ElementsDB, init_elements
+from qm.program import Program
 from qm.jobs.qm_job import QmJob
+from qm.octave import QmOctaveConfig
+from qm.persistence import BaseStore
 from qm.jobs.job_queue import QmQueue
-from qm._QmJobErrors import InvalidDigitalInputPolarityError
+from qm.grpc.qua_config import QuaConfig
+from qm.octave.qm_octave import QmOctave
+from qm.utils import deprecation_message
+from qm.api.models.devices import Polarity
 from qm.api.frontend_api import FrontendApi
+from qm.jobs.pending_job import QmPendingJob
+from qm.jobs.simulated_job import SimulatedJob
+from qm.api.simulation_api import SimulationApi
+from qm.grpc.frontend import JobExecutionStatus
+from qm.jobs.running_qm_job import RunningQmJob
 from qm.api.job_manager_api import JobManagerApi
+from qm.octave.octave_manager import OctaveManager
+from qm.simulate.interface import SimulationConfig
+from qm.elements_db import ElementsDB, init_elements
+from qm.utils.types_utils import convert_object_type
 from qm.api.models.capabilities import ServerCapabilities
 from qm.api.models.compiler import CompilerOptionArguments
-from qm.api.models.devices import Polarity
-from qm.api.simulation_api import SimulationApi
+from qm.program.ConfigBuilder import convert_msg_to_config
+from qm._QmJobErrors import InvalidDigitalInputPolarityError
+from qm.elements.element_with_octave import ElementWithOctave
+from qm.type_hinting.config_types import DictQuaConfig, PortReferenceType, DigitalInputPortConfigType
+from qm.type_hinting.general import Value, Number, PathLike, NumpySupportedFloat, NumpySupportedValue
+from qm.elements.native_elements import MixInputsElement, SingleInputElement, static_set_mixer_correction
 from qm.exceptions import (
+    QmValueError,
     JobCancelledError,
+    ErrorJobStateError,
     InvalidConfigError,
     UnsupportedCapabilityError,
 )
-from qm.jobs.running_qm_job import RunningQmJob
-from qm.octave import QmOctaveConfig
-from qm.jobs.pending_job import QmPendingJob
-from qm.jobs.simulated_job import SimulatedJob
-from qm.octave.octave_manager import OctaveManager
-from qm.octave.qm_octave import QmOctave
-from qm.persistence import BaseStore
-from qm.program import Program
-from qm.program.ConfigBuilder import convert_msg_to_config
-from qm.simulate.interface import SimulationConfig
-from qm.grpc.qua_config import QuaConfig
-from qm.type_hinting.config_types import (
-    DigitalInputPortConfigType,
-    DictQuaConfig,
-    PortReferenceType,
-)
-from qm.type_hinting.general import PathLike, Number, Value, NumpySupportedValue, NumpySupportedFloat
-from qm.utils import deprecation_message, fix_object_data_type
 
 logger = logging.getLogger(__name__)
 
 
 class FunctionInputError(Exception):
     pass
 
@@ -147,17 +143,16 @@
             A simulated job does not support calling QuantumMachine API functions.
 
         The following example shows a simple execution of the simulator, where the
         associated config object is omitted for brevity.
 
         Example:
             ```python
-            from qm.QuantumMachinesManager import QuantumMachinesManager
             from qm.qua import *
-            from qm.simulate import SimulationConfig
+            from qm.simulate import SimulationConfig, QuantumMachinesManager
 
             qmManager = QuantumMachinesManager()
             qm1 = qmManager.open_qm(config)
 
             with program() as prog:
                 play('pulse1', 'element1')
 
@@ -695,25 +690,24 @@
             value_2 (Optional[Union[float, bool, int]]): the value to be
                 placed in ``IO2``
         """
 
         if value_1 is None and value_2 is None:
             return
 
-        if value_1 is not None:
-            logger.debug(f"Setting value '{value_1}' to IO1")
-        if value_2 is not None:
-            logger.debug(f"Setting value '{value_2}' to IO2")
-
-        value_1 = fix_object_data_type(value_1)
-        value_2 = fix_object_data_type(value_2)
-
-        for index, value in enumerate([value_1, value_2]):
-            if type(value) not in (int, float, bool) and value is not None:
-                raise Exception(f"Invalid value_{index + 1} type (The possible types are: int, bool or float)")
+        try:
+            if value_1 is not None:
+                logger.debug(f"Setting value '{value_1}' to IO1")
+                value_1 = convert_object_type(value_1)
+
+            if value_2 is not None:
+                logger.debug(f"Setting value '{value_2}' to IO2")
+                value_2 = convert_object_type(value_2)
+        except QmValueError as e:
+            raise QmValueError(f"Failed to set_io_values: {e.message}") from e
 
         self._frontend.set_io_values(self._id, [value_1, value_2])
 
     def get_io1_value(self) -> Dict[str, Value]:
         """Gets the data stored in ``IO1``
 
         No inference is made on type.
@@ -822,14 +816,39 @@
             )
             return pending_job.wait_for_execution(timeout=10.0)
         except JobCancelledError:
             # In case that the job has finished between the GetRunningJon and the
             # wait for execution
             return None
 
+    def get_job(self, job_id: str) -> Union[QmJob, QmPendingJob]:
+        status: JobExecutionStatus = self._job_manager.get_job_execution_status(job_id, self._id)
+        if status.running or status.completed:
+            return QmJob(
+                job_id=job_id,
+                machine_id=self._id,
+                frontend_api=self._frontend,
+                capabilities=self._capabilities,
+                store=self._store,
+            )
+
+        if status.pending or status.loading:
+            return QmPendingJob(
+                job_id=job_id,
+                machine_id=self._id,
+                frontend_api=self._frontend,
+                capabilities=self._capabilities,
+                store=self._store,
+            )
+
+        raise ErrorJobStateError(
+            f"job {self._id} encountered an error",
+            error_list=[value.string_value for value in status.error.error_messages.values],
+        )
+
     def set_digital_input_threshold(self, port: PortReferenceType, threshold: float) -> None:
         controller_name, port_number = port
         self._frontend.set_digital_input_threshold(self._id, controller_name, port_number, threshold)
 
     def _get_digital_input_port(self, port: PortReferenceType) -> DigitalInputPortConfigType:
         config = self.get_config()
         component = "Controller"
```

### Comparing `qm_qua-1.1.1/qm/QuantumMachinesManager.py` & `qm_qua-1.1.2/qm/quantum_machines_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,58 @@
+import ssl
 import json
 import logging
 import warnings
-
-from typing import Optional, List, Dict, Any
-
 from typing_extensions import TypedDict
+from typing import Any, Dict, List, Optional
 
-from qm.program import Program
-from qm.simulate.interface import SimulationConfig
-from qm.api.models.compiler import CompilerOptionArguments
-from qm.containers.capabilities_container import create_capabilities_container
-from qm.QuantumMachine import QuantumMachine
+import marshmallow
+
+from qm.octave import QmOctaveConfig
 from qm._controller import Controller
+from qm.user_config import UserConfig
+from qm.grpc.qua_config import QuaConfig
+from qm.utils import deprecation_message
 from qm.api.frontend_api import FrontendApi
+from qm.program import Program, load_config
+from qm.QuantumMachine import QuantumMachine
 from qm.api.models.debug_data import DebugData
-from qm.api.models.server_details import ServerDetails
-from qm.api.server_detector import detect_server
-from qm.api.simulation_api import SimulationApi
-from qm.exceptions import QmmException
 from qm.jobs.simulated_job import SimulatedJob
 from qm.logging_utils import set_logging_level
-from qm.octave import QmOctaveConfig
-from qm.octave.calibration_db import load_from_calibration_db
+from qm.api.simulation_api import SimulationApi
+from qm.api.server_detector import detect_server
 from qm.octave.octave_manager import OctaveManager
-from qm.persistence import SimpleFileStore, BaseStore
-from qm.program import load_config
-from qm.program._qua_config_schema import validate_config_capabilities
-from qm.program._qua_config_to_pb import load_config_pb
+from qm.simulate.interface import SimulationConfig
+from qm.persistence import BaseStore, SimpleFileStore
+from qm.api.models.server_details import ServerDetails
 from qm.type_hinting.config_types import DictQuaConfig
-from qm.user_config import UserConfig
-from qm.utils import deprecation_message
+from qm.program._qua_config_to_pb import load_config_pb
+from qm.api.models.compiler import CompilerOptionArguments
+from qm.octave.calibration_db import load_from_calibration_db
+from qm.exceptions import QmmException, ConfigValidationException
+from qm.program._qua_config_schema import validate_config_capabilities
+from qm.containers.capabilities_container import create_capabilities_container
 
 logger = logging.getLogger(__name__)
 
 Version = TypedDict("Version", {"client": str, "server": Optional[str]})
 
 
 class QuantumMachinesManager:
     def __init__(
         self,
         host: Optional[str] = None,
         port: Optional[int] = None,
         *,
+        cluster_name: Optional[str] = None,
         timeout: Optional[float] = None,
         log_level: int = logging.INFO,
         connection_headers: Optional[Dict[str, str]] = None,
         add_debug_data: bool = False,
-        credentials: Optional[str] = None,
+        credentials: Optional[ssl.SSLContext] = None,
         store: Optional[BaseStore] = None,
         file_store_root: str = ".",
         octave: Optional[QmOctaveConfig] = None,
     ):
         """
         Args:
             host (string): Host where to find the QM orchestrator. If
@@ -59,21 +61,22 @@
                 settings are used
         """
         set_logging_level(log_level)
 
         self._user_config = UserConfig.create_from_file()
 
         self._port = port
-        self._host = host or self._user_config.manager_host
+        self._host = host or self._user_config.manager_host or ""
         if self._host is None:
             message = "Failed to connect to QuantumMachines server. No host given."
             logger.error(message)
             raise QmmException(message)
 
         self._credentials = credentials
+        self._cluster_name = cluster_name
         self._store = store if store else SimpleFileStore(file_store_root)
 
         self._octave_config = octave
         self._octave_manager = OctaveManager(octave, self)
 
         self._server_details = self._initialize_connection(
             timeout=timeout,
@@ -94,16 +97,17 @@
     def _initialize_connection(
         self,
         timeout: Optional[float],
         add_debug_data: bool,
         connection_headers: Optional[Dict[str, str]],
     ) -> ServerDetails:
         server_details = detect_server(
+            cluster_name=self._cluster_name,
             user_token=self._user_config.user_token,
-            credentials=self._credentials,
+            ssl_context=self._credentials,
             host=self._host,
             port_from_user_config=self._user_config.manager_port,
             user_provided_port=self._port,
             add_debug_data=add_debug_data,
             timeout=timeout,
             extra_headers=connection_headers,
         )
@@ -115,14 +119,18 @@
         return self._store
 
     @property
     def octave_manager(self) -> OctaveManager:
         warnings.warn("Do not use OctaveManager, it will be removed in the next version", DeprecationWarning)
         return self._octave_manager
 
+    @property
+    def cluster_name(self) -> str:
+        return self._cluster_name or "any"
+
     def perform_healthcheck(self, strict: bool = True) -> None:
         """Perform a health check against the QM server.
 
         Args:
             strict: Will raise an exception if health check failed
         """
         self._frontend.healthcheck(strict)
@@ -176,32 +184,50 @@
         """
         if kwargs:
             logger.warning(f"unused kwargs: {list(kwargs)}, please remove them.")
 
         if use_calibration_data and self._octave_config is not None and self._octave_config.calibration_db is not None:
             load_from_calibration_db(config, self._octave_config.calibration_db)
 
-        if validate_with_protobuf:
-            loaded_config = load_config_pb(config)
-        else:
-            loaded_config = load_config(config)
-        validate_config_capabilities(loaded_config, self._caps)
+        qua_config = self._load_config(config, disable_marshmallow_validation=validate_with_protobuf)
 
-        machine_id = self._frontend.open_qm(loaded_config, close_other_machines)
+        machine_id = self._frontend.open_qm(qua_config, close_other_machines)
 
         return QuantumMachine(
             machine_id=machine_id,
-            pb_config=loaded_config,
+            pb_config=qua_config,
             frontend_api=self._frontend,
             capabilities=self._caps,
             store=self._store,
             octave_config=self._octave_config,
             octave_manager=self._octave_manager,
         )
 
+    def _load_config(self, qua_config: DictQuaConfig, *, disable_marshmallow_validation: bool = False) -> QuaConfig:
+        try:
+            if disable_marshmallow_validation:
+                loaded_config = load_config_pb(qua_config)
+            else:
+                loaded_config = load_config(qua_config)
+            validate_config_capabilities(loaded_config, self._caps)
+            return loaded_config
+        except KeyError as key_error:
+            raise ConfigValidationException(f"Missing key {key_error} in config") from key_error
+        except marshmallow.exceptions.ValidationError as validation_error:
+            raise ConfigValidationException(str(validation_error)) from validation_error
+
+    def validate_qua_config(self, qua_config: DictQuaConfig) -> None:
+        """
+        Validates a qua config based on the connected server's capabilities and returns True if the config is correct.
+
+        Args:
+            qua_config: A python dict containing the qua config to validate
+        """
+        self._load_config(qua_config)
+
     def open_qm_from_file(self, filename: str, close_other_machines: bool = True) -> QuantumMachine:
         """Opens a new quantum machine with config taken from a file on the local file system
 
         Args:
             filename: The path to the file that contains the config
             close_other_machines: Flag whether to close all other
                 running machines
@@ -228,17 +254,16 @@
         """Simulate the outputs of a deterministic QUA program.
 
         The following example shows a simple execution of the simulator, where the
         associated config object is omitted for brevity.
 
         Example:
             ```python
-            from qm.QuantumMachinesManager import QuantumMachinesManager
             from qm.qua import *
-            from qm import SimulationConfig
+            from qm import SimulationConfig, QuantumMachinesManager
 
             qmm = QuantumMachinesManager()
 
             with program() as prog:
                 play('pulse1', 'qe1')
 
             job = qmm.simulate(config, prog, SimulationConfig(duration=100))
```

### Comparing `qm_qua-1.1.1/qm/StreamMetadata.py` & `qm_qua-1.1.2/qm/StreamMetadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,28 @@
+from typing import Dict, List
 from dataclasses import dataclass
-from typing import List, Dict
 
 import betterproto
 import numpy as np
+import numpy.typing as nt
 
 from qm.grpc import results_analyser
-from qm.grpc.results_analyser import ProgramStreamMetadata
+from qm.grpc.results_analyser import (
+    ProgramStreamMetadata,
+    IterationDataForIntIterationValues,
+    IterationDataForDoubleIterationValues,
+    IterationDataForEachIntIterationValues,
+    IterationDataForEachDoubleIterationValues,
+)
 
 
 @dataclass
 class IterationData:
     iteration_variable_name: str
-    iteration_values: np.ndarray
+    iteration_values: nt.NDArray[np.generic]
 
 
 @dataclass
 class StreamMetadataError:
     error: str
     location: str
 
@@ -24,32 +31,34 @@
 class StreamMetadata:
     stream_name: str
     iteration_values: List[IterationData]
 
 
 def _get_numpy_array_from_proto_iteration_data(
     iteration_data: results_analyser.IterationData,
-) -> np.ndarray:
+) -> nt.NDArray[np.generic]:
     name, value = betterproto.which_one_of(iteration_data, "iterationValues")
     if name in ("for_each_int_iteration_values", "for_each_double_iteration_values"):
+        assert isinstance(value, (IterationDataForEachDoubleIterationValues, IterationDataForEachIntIterationValues))
         return np.array(value.values)
 
+    assert isinstance(value, (IterationDataForDoubleIterationValues, IterationDataForIntIterationValues))
     start = value.start_value
     step = value.step
     stop = start + step * value.number_of_iterations
 
     if name == "for_double_iteration_values":
         stop = round(stop, 9)
 
     return np.arange(start=start, step=step, stop=stop)
 
 
 def _get_stream_metadata_dict_from_proto_resp(
     program_metadata: ProgramStreamMetadata,
-) -> Dict[str, List[StreamMetadata]]:
+) -> Dict[str, StreamMetadata]:
     stream_metadata_dict = {
         x.stream_name: StreamMetadata(
             x.stream_name,
             [
                 IterationData(
                     y.iteration_variable_name,
                     _get_numpy_array_from_proto_iteration_data(y),
```

### Comparing `qm_qua-1.1.1/qm/__init__.py` & `qm_qua-1.1.2/qm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,31 @@
 import logging
 
+from qm.jobs.qm_job import QmJob  # noqa
+from qm.type_hinting import DictQuaConfig
 from qm.version import __version__  # noqa
-
-from qm.QuantumMachinesManager import QuantumMachinesManager  # noqa
-from qm.QuantumMachine import QuantumMachine  # noqa
-
+from qm.logging_utils import config_loggers
 from qm.jobs.job_queue import QmQueue  # noqa
+from qm.user_config import UserConfig  # noqa
+from qm.QuantumMachine import QuantumMachine  # noqa
 from qm.jobs.pending_job import QmPendingJob  # noqa
-from qm.jobs.qm_job import QmJob  # noqa
-
-from qm.results import (  # noqa
-    StreamingResultFetcher,
-    SingleStreamingResultFetcher,
-    MultipleStreamingResultFetcher,
-)
-
-from qm.program import Program, _ResultAnalysis, _Program  # noqa
-
+from qm.program import Program, _Program, _ResultAnalysis  # noqa
 from qm.api.models.compiler import CompilerOptionArguments  # noqa
+from qm.quantum_machines_manager import QuantumMachinesManager  # noqa
 from qm.serialization.generate_qua_script import generate_qua_script  # noqa
-from qm.logging_utils import config_loggers
-from qm.user_config import UserConfig  # noqa
-
+from qm.results import StreamingResultFetcher, SingleStreamingResultFetcher, MultipleStreamingResultFetcher  # noqa
 from qm.simulate import (  # noqa
-    SimulationConfig,
     InterOpxAddress,
     InterOpxChannel,
-    ControllerConnection,
     InterOpxPairing,
+    SimulationConfig,
     LoopbackInterface,
+    ControllerConnection,
 )
 
-from qm.type_hinting import DictQuaConfig
-
 __all__ = [
     "QuantumMachinesManager",
     "QuantumMachine",
     "QmQueue",
     "QmPendingJob",
     "QmJob",
     "StreamingResultFetcher",
```

### Comparing `qm_qua-1.1.1/qm/_report.py` & `qm_qua-1.1.2/qm/_report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from dataclasses import dataclass
 from enum import Enum
 from typing import List
+from dataclasses import dataclass
 
-from qm.grpc.results_analyser import GetJobErrorsResponseExecutionErrorSeverity
 from qm.api.job_result_api import JobResultServiceApi
+from qm.grpc.results_analyser import GetJobErrorsResponseExecutionErrorSeverity
 
 
 class ExecutionErrorSeverity(Enum):
     Warn = 0
     Error = 1
 
 
 @dataclass(frozen=True)
 class ExecutionError:
     error_code: int
     message: str
     severity: ExecutionErrorSeverity
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.error_code}\t\t{self.severity.name}\t\t{self.message}"
 
 
 class ExecutionReport:
     def __init__(self, job_id: str, service: JobResultServiceApi) -> None:
         self._job_id = job_id
         self._service = service
@@ -34,19 +34,20 @@
                 message=item.message,
                 severity=ExecutionReport._parse_error_severity(item.error_severity),
             )
             for item in self._service.get_job_errors(self._job_id)
         ]
 
     @staticmethod
-    def _parse_error_severity(error_severity) -> ExecutionErrorSeverity:
+    def _parse_error_severity(error_severity: GetJobErrorsResponseExecutionErrorSeverity) -> ExecutionErrorSeverity:
         if error_severity == GetJobErrorsResponseExecutionErrorSeverity.WARNING:
             return ExecutionErrorSeverity.Warn
         elif error_severity == GetJobErrorsResponseExecutionErrorSeverity.ERROR:
             return ExecutionErrorSeverity.Error
+        raise TypeError(f"No severity level: {error_severity}")
 
     def has_errors(self) -> bool:
         """Returns: True if encountered a runtime error while executing the job."""
         return len(self._errors) > 0
 
     def errors(self) -> List[ExecutionError]:
         """Returns: list of all execution errors for this job"""
```

### Comparing `qm_qua-1.1.1/qm/api/base_api.py` & `qm_qua-1.1.2/qm/api/base_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-import asyncio
-import functools
 import json
+import asyncio
 import logging
-from typing import Optional, Callable, Type, TypeVar
+import functools
 from typing_extensions import ParamSpec
+from typing import Type, TypeVar, Callable, Optional
 
 import grpclib.exceptions
 from grpclib.client import Channel
 from grpclib.config import Configuration
-from grpclib.events import (
-    RecvInitialMetadata,
-    listen,
-    SendRequest,
-    SendMessage,
-)
+from grpclib.events import SendMessage, SendRequest, RecvInitialMetadata, listen
 
-from qm.utils.async_utils import EventLoopThread, run_async
 from qm.api.models.server_details import ConnectionDetails
-from qm.exceptions import QMConnectionError, QMTimeoutError
+from qm.exceptions import QMTimeoutError, QMConnectionError
+from qm.utils.async_utils import EventLoopThread, run_async
 
 logger = logging.getLogger(__name__)
 
 Ret = TypeVar("Ret")
 P = ParamSpec("P")
 
 
@@ -55,15 +50,15 @@
     return decorate
 
 
 async def create_channel(connection_details: ConnectionDetails) -> Channel:
     return Channel(
         host=connection_details.host,
         port=connection_details.port,
-        ssl=connection_details.credentials is not None,
+        ssl=connection_details.ssl_context,
         config=Configuration(
             http2_connection_window_size=connection_details.max_message_size,
             http2_stream_window_size=connection_details.max_message_size,
         ),
     )
```

### Comparing `qm_qua-1.1.1/qm/api/frontend_api.py` & `qm_qua-1.1.2/qm/api/frontend_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,76 +1,74 @@
 import logging
-from typing import List, Tuple, Optional
+from typing import List, Tuple, Optional, cast
 
 from betterproto.lib.google.protobuf import Empty
 
+import qm.grpc.qm_api
 from qm.type_hinting import Value
+from qm.grpc.qua import QuaProgram
+from qm.grpc.compiler import QuaValues
+from qm.grpc.qua_config import QuaConfig
 from qm.utils.async_utils import run_async
-from qm.api.base_api import connection_error_handle, BaseApi
-from qm.api.models.compiler import (
-    CompilerOptionArguments,
-    _get_request_compiler_options,
-)
-from qm.api.models.devices import MixerInfo, AnalogOutputPortFilter, Polarity
+from qm.grpc.general_messages import Matrix
 from qm.api.models.jobs import InsertDirection
-from qm.api.models.quantum_machine import QuantumMachineData
+from qm.utils.protobuf_utils import LOG_LEVEL_MAP
 from qm.api.models.server_details import ConnectionDetails
-from qm.exceptions import (
-    OpenQmException,
-    FailedToAddJobToQueueException,
-    CompilationException,
-    QMHealthCheckError,
-    QMFailedToGetQuantumMachineError,
-    QmFailedToCloseQuantumMachineError,
-    QMFailedToCloseAllQuantumMachinesError,
-    QMRequestError,
-    QMConnectionError,
-    QMRequestDataError,
+from qm.api.base_api import BaseApi, connection_error_handle
+from qm.api.models.quantum_machine import QuantumMachineData
+from qm.api.models.devices import Polarity, MixerInfo, AnalogOutputPortFilter
+from qm.api.models.compiler import CompilerOptionArguments, _get_request_compiler_options
+from qm.grpc.qm_manager import (
+    Controller,
+    GetQuantumMachineRequest,
+    OpenQuantumMachineRequest,
+    CloseQuantumMachineRequest,
 )
-from qm.grpc.compiler import QuaValues
 from qm.grpc.frontend import (
     FrontendStub,
-    ResetDataProcessingRequest,
-    PerformHalDebugCommandRequest,
-    AddToQueueRequest,
+    QmDataRequest,
     QueuePosition,
-    ExecutionOverrides,
-    AddCompiledToQueueRequest,
     CompileRequest,
-    QmDataRequest,
     IoValueRequest,
+    AddToQueueRequest,
+    ExecutionOverrides,
+    AddCompiledToQueueRequest,
+    ResetDataProcessingRequest,
+    PerformHalDebugCommandRequest,
+)
+from qm.exceptions import (
+    QMRequestError,
+    OpenQmException,
+    QMConnectionError,
+    QMHealthCheckError,
+    QMRequestDataError,
+    CompilationException,
+    FailedToAddJobToQueueException,
+    QMFailedToGetQuantumMachineError,
+    QmFailedToCloseQuantumMachineError,
+    QMFailedToCloseAllQuantumMachinesError,
 )
 from qm.grpc.qm_api import (
+    DigitalInputPort,
     HighQmApiRequest,
-    HighQmApiRequestSetCorrection,
-    HighQmApiRequestSetCorrectionMixerInfo,
+    HighQmApiRequestQePort,
+    HighQmApiRequestSetIoValues,
     HighQmApiRequestSetFrequency,
+    HighQmApiRequestSetCorrection,
+    HighQmApiRequestIoValueSetData,
+    HighQmApiRequestSetDigitalRoute,
+    HighQmApiRequestSetInputDcOffset,
     HighQmApiRequestSetOutputDcOffset,
-    HighQmApiRequestQePort,
     HighQmApiRequestSetOutputFilterTaps,
     HighQmApiRequestAnalogOutputPortFilter,
-    HighQmApiRequestSetInputDcOffset,
-    HighQmApiRequestSetDigitalRoute,
-    HighQmApiRequestSetIoValues,
-    HighQmApiRequestIoValueSetData,
-    HighQmApiRequestSetDigitalInputThreshold,
-    DigitalInputPort,
-    HighQmApiRequestSetDigitalInputPolarity,
+    HighQmApiRequestSetCorrectionMixerInfo,
     HighQmApiRequestSetDigitalInputDeadtime,
-    Matrix,
-)
-from qm.grpc.qm_manager import (
-    OpenQuantumMachineRequest,
-    GetQuantumMachineRequest,
-    CloseQuantumMachineRequest,
-    Controller,
+    HighQmApiRequestSetDigitalInputPolarity,
+    HighQmApiRequestSetDigitalInputThreshold,
 )
-from qm.grpc.qua import QuaProgram
-from qm.grpc.qua_config import QuaConfig
-from qm.utils.protobuf_utils import LOG_LEVEL_MAP
 
 logger = logging.getLogger(__name__)
 
 
 @connection_error_handle()
 class FrontendApi(BaseApi):
     def __init__(self, connection_details: ConnectionDetails):
@@ -280,15 +278,16 @@
                 mixer=mixer.mixer,
                 frequency_negative=mixer.frequency_negative,
                 intermediate_frequency=mixer.intermediate_frequency,
                 intermediate_frequency_double=mixer.intermediate_frequency_double,
                 lo_frequency=mixer.lo_frequency,
                 lo_frequency_double=mixer.lo_frequency_double,
             ),
-            correction=correction,
+            correction=cast(qm.grpc.qm_api.Matrix, correction),  # For some reason we have two matrix messages,
+            # although they are the same...
         )
         request = HighQmApiRequest(quantum_machine_id=machine_id, set_correction=correction_request)
         self._perform_qm_request(request)
 
     def set_intermediate_frequency(self, machine_id: str, element: str, value: float) -> None:
         set_frequency_request = HighQmApiRequestSetFrequency(qe=element, value=value)
         request = HighQmApiRequest(quantum_machine_id=machine_id, set_frequency=set_frequency_request)
```

### Comparing `qm_qua-1.1.1/qm/api/info_service_api.py` & `qm_qua-1.1.2/qm/api/info_service_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from qm.utils.async_utils import run_async
-from qm.api.base_api import BaseApi, connection_error_handle
-from qm.api.models.info import ImplementationInfo, QuaMachineInfo
 from qm.api.models.server_details import ConnectionDetails
-from qm.io.qualang.api.v1 import InfoServiceStub, GetInfoRequest
+from qm.api.base_api import BaseApi, connection_error_handle
+from qm.io.qualang.api.v1 import GetInfoRequest, InfoServiceStub
+from qm.api.models.info import QuaMachineInfo, ImplementationInfo
 
 
 @connection_error_handle()
 class InfoServiceApi(BaseApi):
     def __init__(self, connection_details: ConnectionDetails):
         super().__init__(connection_details)
         self._stub = InfoServiceStub(self._channel)
```

### Comparing `qm_qua-1.1.1/qm/api/job_manager_api.py` & `qm_qua-1.1.2/qm/api/job_manager_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 import logging
-from typing import List, Optional, cast, Tuple
+from typing import List, Tuple, Optional, cast
 
 from dependency_injector.wiring import Provide
 
+from qm.type_hinting import Value
+from qm.exceptions import QmValueError
+from qm.utils.async_utils import run_async
+from qm.grpc.general_messages import Matrix
+from qm.api.models.jobs import PendingJobData
+from qm.grpc.qm_manager import GetRunningJobRequest
+from qm.api.models.capabilities import ServerCapabilities
+from qm.api.models.server_details import ConnectionDetails
+from qm.api.base_api import BaseApi, connection_error_handle
+from qm.containers.capabilities_container import CapabilitiesContainer
+from qm.grpc.job_manager import (
+    JobManagerServiceStub,
+    InsertInputStreamRequest,
+    GetElementCorrectionRequest,
+    SetElementCorrectionRequest,
+)
 from qm._QmJobErrors import (
+    MissingJobError,
     MissingElementError,
+    UnknownInputStreamError,
     ElementWithSingleInputError,
     InvalidElementCorrectionError,
+    InvalidJobExecutionStatusError,
     ElementWithoutIntermediateFrequencyError,
     _handle_job_manager_error,
-    MissingJobError,
-    InvalidJobExecutionStatusError,
-    UnknownInputStreamError,
 )
-from qm.type_hinting import Value
-from qm.utils.async_utils import run_async
-from qm.api.base_api import BaseApi, connection_error_handle
-from qm.api.models.capabilities import ServerCapabilities
-from qm.api.models.jobs import PendingJobData
-from qm.api.models.server_details import ConnectionDetails
-from qm.containers.capabilities_container import CapabilitiesContainer
-from qm.exceptions import QmValueError
 from qm.grpc.frontend import (
-    FrontendStub,
     HaltRequest,
+    FrontendStub,
     ResumeRequest,
-    PausedStatusRequest,
+    JobQueryParams,
+    QueryValueMatcher,
+    JobExecutionStatus,
     IsJobRunningRequest,
-    IsJobAcquiringDataResponseAcquiringStatus,
+    PausedStatusRequest,
     IsJobAcquiringDataRequest,
-    JobExecutionStatus,
     GetJobExecutionStatusRequest,
-    JobQueryParams,
-    QueryValueMatcher,
-)
-from qm.grpc.general_messages import Matrix
-from qm.grpc.job_manager import (
-    JobManagerServiceStub,
-    SetElementCorrectionRequest,
-    GetElementCorrectionRequest,
-    InsertInputStreamRequest,
+    IsJobAcquiringDataResponseAcquiringStatus,
 )
-from qm.grpc.qm_manager import GetRunningJobRequest
 
 logger = logging.getLogger(__name__)
 
 
 @connection_error_handle()
 class JobManagerApi(BaseApi):
     def __init__(
@@ -53,17 +53,15 @@
         connection_details: ConnectionDetails,
         capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities],
     ):
         super().__init__(connection_details)
         if capabilities.supports_new_grpc_structure:
             self._job_manager_stub = JobManagerServiceStub(self._channel)
         else:
-            from qm.api.stubs.deprecated_job_manager_stub import (
-                DeprecatedJobManagerServiceStub,
-            )
+            from qm.api.stubs.deprecated_job_manager_stub import DeprecatedJobManagerServiceStub
 
             # TODO: add deprecation warning
             self._job_manager_stub = DeprecatedJobManagerServiceStub(self._channel)
         self._frontend_stub = FrontendStub(self._channel)
 
     def set_element_correction(
         self, job_id: str, element_name: str, correction: Matrix
```

### Comparing `qm_qua-1.1.1/qm/api/job_result_api.py` & `qm_qua-1.1.2/qm/api/job_result_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-from typing import List, AsyncIterator, Tuple, Dict
 import logging
-from qm.StreamMetadata import (
-    StreamMetadataError,
-    _get_stream_metadata_dict_from_proto_resp,
-    StreamMetadata,
-)
+from typing import Dict, List, Tuple, AsyncIterator
+
 from qm.utils.async_utils import run_async
+from qm.api.models.server_details import ConnectionDetails
+from qm.api.base_api import BaseApi, connection_error_handle
+from qm.StreamMetadata import StreamMetadata, StreamMetadataError, _get_stream_metadata_dict_from_proto_resp
 from qm.grpc.results_analyser import (
-    JobResultsServiceStub,
+    GetJobStateRequest,
     GetJobErrorsRequest,
-    GetJobErrorsResponseError,
+    GetJobStateResponse,
+    JobResultsServiceStub,
+    GetJobDebugDataRequest,
+    GetJobDebugDataResponse,
     GetJobNamedResultRequest,
+    GetJobErrorsResponseError,
     GetJobNamedResultResponse,
-    GetJobStateRequest,
-    GetJobNamedResultHeaderRequest,
-    GetJobNamedResultHeaderResponse,
-    GetProgramMetadataRequest,
     GetJobResultSchemaRequest,
-    GetJobDebugDataRequest,
-    GetJobStateResponse,
-    GetJobDebugDataResponse,
+    GetProgramMetadataRequest,
     GetJobResultSchemaResponse,
+    GetJobNamedResultHeaderRequest,
+    GetJobNamedResultHeaderResponse,
 )
-from qm.api.base_api import BaseApi, connection_error_handle
-from qm.api.models.server_details import ConnectionDetails
 
 logger = logging.getLogger(__name__)
 
 
 @connection_error_handle()
 class JobResultServiceApi(BaseApi):
     def __init__(self, connection_details: ConnectionDetails):
@@ -51,15 +48,15 @@
         return response
 
     def get_named_header(self, job_id: str, output_name: str, flat_struct: bool) -> GetJobNamedResultHeaderResponse:
         request = GetJobNamedResultHeaderRequest(job_id=job_id, output_name=output_name, flat_format=flat_struct)
         response = run_async(self._stub.get_job_named_result_header(request, timeout=self._timeout))
         return response
 
-    def get_program_metadata(self, job_id: str) -> Tuple[List[StreamMetadataError], Dict[str, List[StreamMetadata]]]:
+    def get_program_metadata(self, job_id: str) -> Tuple[List[StreamMetadataError], Dict[str, StreamMetadata]]:
         request = GetProgramMetadataRequest(job_id=job_id)
 
         response = run_async(self._stub.get_program_metadata(request, timeout=self._timeout))
 
         if response.success:
             metadata_errors = [
                 StreamMetadataError(error.error, error.location)
```

### Comparing `qm_qua-1.1.1/qm/api/models/capabilities.py` & `qm_qua-1.1.2/qm/api/models/capabilities.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/api/models/compiler.py` & `qm_qua-1.1.2/qm/api/models/compiler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from dataclasses import dataclass, field
-from typing import Optional, List
+from typing import List, Optional
+from dataclasses import field, dataclass
 
 from qm.grpc.qua import QuaProgramCompilerOptions
 
 
 @dataclass
 class CompilerOptionArguments:
     strict: Optional[bool] = field(default=None)
```

### Comparing `qm_qua-1.1.1/qm/api/models/devices.py` & `qm_qua-1.1.2/qm/api/models/devices.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from dataclasses import dataclass, field, asdict
 from enum import Enum
-from typing import List, Dict, Union
+from typing import Dict, List, Union
+from dataclasses import asdict, dataclass
 
 from qm.grpc.qm_api import DigitalInputPortPolarity
 
 
 @dataclass(frozen=True)
 class MixerInfo:
     mixer: str
     frequency_negative: bool
-    intermediate_frequency: int = field(default=0)
-    intermediate_frequency_double: float = field(default=0.0)
-    lo_frequency: int = field(default=0)
-    lo_frequency_double: float = field(default=0.0)
+    intermediate_frequency: int
+    intermediate_frequency_double: float
+    lo_frequency: int
+    lo_frequency_double: float
 
     def as_dict(self) -> Dict[str, Union[str, bool, int, float]]:
         return {key: value for key, value in asdict(self).items() if value is not None}
 
 
 @dataclass(frozen=True)
 class AnalogOutputPortFilter:
```

### Comparing `qm_qua-1.1.1/qm/api/models/server_details.py` & `qm_qua-1.1.2/qm/api/models/server_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+import ssl
 import dataclasses
-from typing import Optional, Dict
+from typing import Dict, Optional
 
-from qm.api.models.capabilities import ServerCapabilities
 from qm.api.models.info import QuaMachineInfo
 from qm.api.models.debug_data import DebugData
+from qm.api.models.capabilities import ServerCapabilities
 
 MAX_MESSAGE_SIZE = 1024 * 1024 * 100  # 100 mb in bytes
 BASE_TIMEOUT = 60
 
 
 @dataclasses.dataclass
 class ConnectionDetails:
     host: str
     port: int
     user_token: Optional[str]
-    credentials: Optional[str]
+    ssl_context: Optional[ssl.SSLContext]
     max_message_size: int = dataclasses.field(default=MAX_MESSAGE_SIZE)
     headers: Dict[str, str] = dataclasses.field(default_factory=dict)
     timeout: float = dataclasses.field(default=BASE_TIMEOUT)
     debug_data: Optional[DebugData] = dataclasses.field(default=None)
 
 
 @dataclasses.dataclass
```

### Comparing `qm_qua-1.1.1/qm/api/simulation_api.py` & `qm_qua-1.1.2/qm/api/simulation_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 import logging
 from typing import Tuple, AsyncIterator
 
-from qm.type_hinting.config_types import DictQuaConfig
-from qm.utils.async_utils import run_async
 from qm.simulate import interface
-from qm.simulate.interface import SimulationConfig
-from qm.program import Program
 from qm.api.base_api import BaseApi
-from qm.api.models.compiler import (
-    CompilerOptionArguments,
-    _get_request_compiler_options,
-)
+from qm.utils.async_utils import run_async
+from qm.program import Program, load_config
+from qm.utils.protobuf_utils import LOG_LEVEL_MAP
+from qm.simulate.interface import SimulationConfig
+from qm.type_hinting.config_types import DictQuaConfig
 from qm.api.models.server_details import ConnectionDetails
 from qm.exceptions import QMSimulationError, FailedToExecuteJobException
+from qm.api.models.compiler import CompilerOptionArguments, _get_request_compiler_options
+from qm.grpc.results_analyser import SimulatorSamplesResponse, PullSimulatorSamplesRequest
 from qm.grpc.frontend import (
     FrontendStub,
-    SimulatedResponsePart,
-    SimulationRequest,
-    ExecutionRequestSimulate,
+    DensityMatrix,
     InterOpxAddress,
+    InterOpxChannel,
+    SimulationRequest,
     InterOpxConnection,
+    SimulatedResponsePart,
+    ExecutionRequestSimulate,
+    GetSimulatedQuantumStateRequest,
     InterOpxConnectionAddressToAddress,
-    InterOpxChannel,
     InterOpxConnectionChannelToChannel,
-    GetSimulatedQuantumStateRequest,
-    DensityMatrix,
 )
-from qm.grpc.results_analyser import (
-    PullSimulatorSamplesRequest,
-    SimulatorSamplesResponse,
-)
-from qm.program import load_config
-from qm.utils.protobuf_utils import LOG_LEVEL_MAP
 
 logger = logging.getLogger(__name__)
 
 
 class SimulationApi(BaseApi):
     def __init__(self, connection_details: ConnectionDetails):
         super().__init__(connection_details)
@@ -70,28 +63,32 @@
                 if not isinstance(connection.source, type(connection.target)):
                     raise Exception(
                         f"Unsupported InterOpx connection. Source is "
                         f"{type(connection.source).__name__} but target is "
                         f"{type(connection.target).__name__}"
                     )
 
-                if isinstance(connection.source, interface.InterOpxAddress):
+                if isinstance(connection.source, interface.InterOpxAddress) and isinstance(
+                    connection.target, interface.InterOpxAddress
+                ):
                     con = InterOpxConnection(
                         address_to_address=InterOpxConnectionAddressToAddress(
                             source=InterOpxAddress(
                                 controller=connection.source.controller,
                                 left=connection.source.is_left_connection,
                             ),
                             target=InterOpxAddress(
                                 controller=connection.target.controller,
                                 left=connection.target.is_left_connection,
                             ),
                         )
                     )
-                elif isinstance(connection.source, interface.InterOpxChannel):
+                elif isinstance(connection.source, interface.InterOpxChannel) and isinstance(
+                    connection.target, interface.InterOpxChannel
+                ):
                     con = InterOpxConnection(
                         channel_to_channel=InterOpxConnectionChannelToChannel(
                             source=InterOpxChannel(
                                 controller=connection.source.controller,
                                 channel_number=connection.source.channel_number,
                             ),
                             target=InterOpxChannel(
```

### Comparing `qm_qua-1.1.1/qm/api/stubs/deprecated_job_manager_stub.py` & `qm_qua-1.1.2/qm/api/stubs/deprecated_job_manager_stub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from typing import Optional
 
 import betterproto
 
-from qm.grpc.job_manager import (
-    GetElementCorrectionResponse,
-    SetElementCorrectionResponse,
-    InsertInputStreamResponse,
-)
+from qm.grpc.job_manager import InsertInputStreamResponse, GetElementCorrectionResponse, SetElementCorrectionResponse
 
 
 class DeprecatedJobManagerServiceStub(betterproto.ServiceStub):
     async def get_element_correction(
         self,
         get_element_correction_request: "GetElementCorrectionRequest",
         *,
```

### Comparing `qm_qua-1.1.1/qm/containers/capabilities_container.py` & `qm_qua-1.1.2/qm/containers/capabilities_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
-from dependency_injector import containers, providers
+from dependency_injector import providers, containers
 
-from qm.api.models.capabilities import ServerCapabilities
 from qm.api.models.info import QuaMachineInfo
+from qm.api.models.capabilities import ServerCapabilities
 
 
 class CapabilitiesContainer(containers.DeclarativeContainer):
     config = providers.Configuration()
 
     capabilities = providers.Singleton(ServerCapabilities.build, qua_implementation=config.qua_implementation)
```

### Comparing `qm_qua-1.1.1/qm/datadog_api.py` & `qm_qua-1.1.2/qm/datadog_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import sys
-from qm.version import __version__
-from datadog_api_client import ApiClient, Configuration
+from logging import LogRecord
+from logging.handlers import BufferingHandler
+
 from datadog_api_client.v2.api.logs_api import LogsApi
-from datadog_api_client.v2.model.content_encoding import ContentEncoding
 from datadog_api_client.v2.model.http_log import HTTPLog
 from datadog_api_client.v2.model.http_log_item import HTTPLogItem
+from datadog_api_client.v2.model.content_encoding import ContentEncoding
+from datadog_api_client import ApiClient, Configuration  # type: ignore[attr-defined]
 
-
-from logging import LogRecord
-from logging.handlers import BufferingHandler
+from qm.version import __version__
 
 
 class DatadogHandler(BufferingHandler):
     def __init__(self, user_id: str, organization: str, user_token: str, session_id: str):
         super().__init__(capacity=100)
         self._user_id = user_id
         self._organization = organization
         self._user_token = user_token
         self._session_id = session_id
 
-    def _prepare_record(self, record: LogRecord):
+    def _prepare_record(self, record: LogRecord) -> HTTPLogItem:
         return HTTPLogItem(
             ddsource="python",
             hostname=self._user_id,
             message=record.msg,
             service=record.name,
             status=record.levelname,
             session_id=str(self._session_id),
             python_version=sys.version,
             qua_version=__version__,
         )
 
     @property
-    def logs_as_http(self):
+    def logs_as_http(self) -> HTTPLog:
         _logs = []
         for record in self.buffer:
             _logs.append(self._prepare_record(record))
-        return HTTPLog(_logs)
+        return HTTPLog(_logs)  # type: ignore[no-untyped-call]
 
-    def send_logs(self):
-        configuration = Configuration(
+    def send_logs(self) -> None:
+        configuration = Configuration(  # type: ignore[no-untyped-call]
             api_key={"apiKeyAuth": self._user_token},
             server_variables={"site": "datadoghq.eu"},
         )
         with ApiClient(configuration) as api_client:
-            api_instance = LogsApi(api_client)
+            api_instance = LogsApi(api_client)  # type: ignore[no-untyped-call]
             response = api_instance.submit_log(content_encoding=ContentEncoding.GZIP, body=self.logs_as_http)
             print(response)
 
-    def flush(self):
+    def flush(self) -> None:
         self.send_logs()
         super().flush()
```

### Comparing `qm_qua-1.1.1/qm/elements/basic_element.py` & `qm_qua-1.1.2/qm/elements/basic_element.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
 
 import numpy
-from dependency_injector.wiring import inject, Provide
+from dependency_injector.wiring import Provide, inject
 
 from qm.api.frontend_api import FrontendApi
 from qm.api.models.capabilities import ServerCapabilities
 from qm.containers.capabilities_container import CapabilitiesContainer
 from qm.grpc.qua_config import QuaConfigElementDec, QuaConfigDacPortReference
-from qm.utils import fix_object_data_type
 
 logger = logging.getLogger(__name__)
 
 
 class BasicElement:
     def __init__(
         self,
@@ -21,25 +20,25 @@
         machine_id: str,
     ):
         self._config = config
         self._name = name
         self._frontend = frontend_api
         self._id = machine_id
 
-    def _output_dc_offset(self, port: QuaConfigDacPortReference) -> float:
+    def _output_dc_offset(self, port: QuaConfigDacPortReference) -> None:
         pass
 
     @inject
     def set_intermediate_frequency(
         self, freq: float, capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities]
-    ):
+    ) -> None:
         if not isinstance(freq, (numpy.floating, float)):
             raise TypeError("freq must be a float")
 
-        freq = fix_object_data_type(freq)
+        freq = float(freq)
         logger.debug(f"Setting element '{self._name}' intermediate frequency to '{freq}'.")
         self._frontend.set_intermediate_frequency(self._id, self._name, freq)
         if capabilities.supports_double_frequency:
             self._config.intermediate_frequency_double = float(freq)
             self._config.intermediate_frequency = 0
         else:
             self._config.intermediate_frequency = int(freq)
@@ -48,55 +47,55 @@
     @property
     @inject
     def intermediate_frequency(
         self, capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities]
     ) -> float:
         if capabilities.supports_double_frequency:
             return self._config.intermediate_frequency_double
-        return self._config.intermediate_frequency
+        return float(self._config.intermediate_frequency or 0)
 
     def get_digital_delay(self, digital_input_name: str) -> int:
         try:
             return self._config.digital_inputs[digital_input_name].delay
         except KeyError:
             raise Exception(f"Digital input for {digital_input_name} was not found.")
 
     def get_digital_buffer(self, digital_input_name: str) -> int:
         try:
             return self._config.digital_inputs[digital_input_name].buffer
         except KeyError:
             raise Exception(f"Digital buffer for {digital_input_name} was not found.")
 
-    def set_digital_delay(self, digital_input: str, delay: int):
+    def set_digital_delay(self, digital_input: str, delay: int) -> None:
         if not isinstance(digital_input, str):
             raise Exception("port must be a string")
         if not isinstance(delay, int):
             raise Exception("delay must be an int")
         logger.debug(f"Setting delay of digital port '{digital_input}' on element '{self._name}' to '{delay}'")
         self._frontend.set_digital_delay(self._id, self._name, digital_input, delay)
         self._config.digital_inputs[digital_input].delay = delay
 
-    def set_digital_buffer(self, digital_input: str, buffer: int):
+    def set_digital_buffer(self, digital_input: str, buffer: int) -> None:
         if not isinstance(digital_input, str):
             raise Exception("port must be a string")
         if not isinstance(buffer, int):
             raise Exception("buffer must be an int.")
         logger.debug(f"Setting buffer of digital port '{digital_input}' on element '{self._name}' to '{buffer}'")
         self._frontend.set_digital_buffer(self._id, self._name, digital_input, buffer)
         self._config.digital_inputs[digital_input].buffer = buffer
 
-    def set_input_dc_offset(self, output: str, offset: float):
+    def set_input_dc_offset(self, output: str, offset: float) -> None:
         logger.debug(f"Setting DC offset of output '{output}' on element '{self._name}' to '{offset}'.")
         if not isinstance(output, str):
             raise TypeError("output must be a string")
         if output not in self._config.outputs:
             raise ValueError(f"output {output} was not found in the element's outputs")
         if not isinstance(offset, (numpy.floating, float)):
             raise TypeError("offset must be a float")
-        offset = fix_object_data_type(offset)
+        offset = float(offset)
         self._frontend.set_input_dc_offset(self._id, self._name, output, offset)
 
     @property
     def time_of_flight(self) -> int:
         return self._config.time_of_flight or 0
 
     @property
```

### Comparing `qm_qua-1.1.1/qm/elements/element_with_octave.py` & `qm_qua-1.1.2/qm/elements/element_with_octave.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from typing import Optional
 
 import betterproto
-from octave_sdk import (
-    OctaveLOSource,
-    RFOutputMode,
-    RFInputLOSource,
+from octave_sdk.octave import Octave, ClockInfo  # type: ignore[import]
+from octave_sdk import (  # type: ignore[import]
     IFMode,
     ClockType,
+    RFOutputMode,
     ClockFrequency,
+    OctaveLOSource,
+    RFInputLOSource,
     RFInputRFSource,
 )
-from octave_sdk.octave import ClockInfo, Octave
 
 from qm.api.frontend_api import FrontendApi
+from qm.grpc.octave_models import OctaveLoSourceInput
 from qm.elements.native_elements import MixInputsElement
-from qm.grpc.qua_config import QuaConfigElementDec
+from qm.grpc.qua_config import QuaConfigElementDec, QuaConfigOutputSwitchState
+
+
+class NoOctaveSdkException(Exception):
+    pass
 
 
 class SetFrequencyException(Exception):
     pass
 
 
 class ElementWithOctave(MixInputsElement):
@@ -40,40 +45,59 @@
         self._octave_rf_input_port_number = octave_rf_input_port_number
 
     def set_client(self) -> None:
         """
         This function is intended to be used from outside, using the batch mode,
         to run it in parallel on all the quantum-elements, on all the octaves
         """
-        if self._config.mix_inputs.octave_params.lo_source:
-            self.set_lo_source(OctaveLOSource[self._config.config.mix_inputs.octave_params.lo_source.name])
+        octave_params = self._config.mix_inputs.octave_params
+        if octave_params.lo_source:
+            self.set_lo_source(OctaveLOSource[octave_params.lo_source.name])
         else:
             self.set_lo_source(OctaveLOSource.Internal)
 
         if self.lo_source == OctaveLOSource.Internal and self.lo_source in self._client._port_mapping:
             self.set_lo_frequency(self.lo_frequency, set_source=False)
 
-    def set_downconversion_port(self, downconversion_client: Octave, octave_rf_input_port_number: int):
+        if octave_params.output_switch_state != QuaConfigOutputSwitchState.unset:
+            output_mode = {
+                QuaConfigOutputSwitchState.always_on: RFOutputMode.on,
+                QuaConfigOutputSwitchState.always_off: RFOutputMode.off,
+                QuaConfigOutputSwitchState.triggered: RFOutputMode.trig_normal,
+                QuaConfigOutputSwitchState.triggered_reversed: RFOutputMode.trig_inverse,
+            }[octave_params.output_switch_state]
+            self.set_rf_output_mode(output_mode)
+
+        if octave_params.output_gain is not None:
+            self.set_rf_output_gain(octave_params.output_gain)
+
+        if octave_params.downconversion_lo_source not in {OctaveLoSourceInput.Off, 0}:
+            self._set_downconversion_lo(
+                lo_source=RFInputLOSource[octave_params.downconversion_lo_source.name],
+                lo_frequency=octave_params.downconversion_lo_frequency or None,
+            )
+
+    def set_downconversion_port(self, downconversion_client: Octave, octave_rf_input_port_number: int) -> None:
         self._downconversion_client = downconversion_client
         self._octave_rf_input_port_number = octave_rf_input_port_number
 
     @property
     def _octave_if_input_port_number(self) -> int:
-        if betterproto.serialized_on_wire(self._config.up_converted):
-            enum_number = self._config.up_converted.rf_output_port.output.value + 1
+        if betterproto.serialized_on_wire(self._config.mix_inputs.octave_params):
+            enum_number = self._config.mix_inputs.octave_params.rf_output_port.port_name.value + 1
             # The enums are 0-based and the ports are 1-based
         else:
             enum_number = self._octave_if_input_port_number_backup
         return enum_number
 
     @property
     def lo_source(self) -> OctaveLOSource:
         return self._client.rf_outputs[self._octave_if_input_port_number].get_lo_source()
 
-    def set_lo_frequency(self, lo_frequency: float, set_source: bool = True):
+    def set_lo_frequency(self, lo_frequency: float, set_source: bool = True) -> None:
         # TODO - validate that LO frequency can be casted to int, or it should be a float in the proto
         """
         Sets the LO frequency of the synthesizer associated to element
 
         :param lo_frequency:
         :param set_source:
         """
@@ -84,35 +108,35 @@
             self._client.rf_outputs[self._octave_if_input_port_number].set_lo_source(
                 self.lo_source, ignore_shared_errors=True
             )
 
         self._client.rf_outputs[self._octave_if_input_port_number].set_lo_frequency(self.lo_source, lo_frequency)
         self.lo_frequency = lo_frequency
 
-    def set_lo_source(self, lo_port: OctaveLOSource):
+    def set_lo_source(self, lo_port: OctaveLOSource) -> None:
         """
         Sets the source of LO going to the upconverter associated with element.
         :param lo_port:
         """
         self._client.rf_outputs[self._octave_if_input_port_number].set_lo_source(lo_port, ignore_shared_errors=True)
 
-    def set_rf_output_mode(self, switch_mode: RFOutputMode):
+    def set_rf_output_mode(self, switch_mode: RFOutputMode) -> None:
         """
         Configures the output switch of the upconverter associated to element.
         switch_mode can be either: 'always_on', 'always_off', 'normal' or 'inverted'
         When in 'normal' mode a high trigger will turn the switch on and a low trigger will turn it off
         When in 'inverted' mode a high trigger will turn the switch off and a low trigger will turn it on
         When in 'always_on' the switch will be permanently on. When in 'always_off' mode the switch will
         be permanently off.
 
         :param switch_mode:
         """
         self._client.rf_outputs[self._octave_if_input_port_number].set_output(switch_mode)
 
-    def set_rf_output_gain(self, gain_in_db: float):
+    def set_rf_output_gain(self, gain_in_db: float) -> None:
         """
         Sets the RF output gain for the up-converter associated with the element.
         RF_gain is in steps of 0.5dB from -20 to +24 and is referring
         to the maximum OPX output power of 4dBm (=0.5V pk-pk) So for a value of -24
         for example, an IF signal coming from the OPX at max power (4dBm) will be
         upconverted and come out of Octave at -20dBm
 
@@ -124,15 +148,15 @@
 
     def set_downconversion(
         self,
         lo_source: Optional[RFInputLOSource] = None,
         lo_frequency: Optional[float] = None,
         if_mode_i: IFMode = IFMode.direct,
         if_mode_q: IFMode = IFMode.direct,
-    ):
+    ) -> None:
         """
         Sets the LO source for the downconverters.
         The LO source will be the one associated with the upconversion of element
 
         :param lo_source:
         :param lo_frequency:
         :param if_mode_i:
@@ -141,15 +165,15 @@
         self._set_downconversion_lo(lo_source, lo_frequency)
         self._set_downconversion_if_mode(if_mode_i, if_mode_q)
 
     def _set_downconversion_lo(
         self,
         lo_source: Optional[RFInputLOSource] = None,
         lo_frequency: Optional[float] = None,
-    ):
+    ) -> None:
         """
         Sets the LO source for the downconverters.
         If no value is given the LO source will be the one associated with the
         upconversion of element
 
         :param lo_frequency:
         :param lo_source:
@@ -161,32 +185,36 @@
         # any settings applied will affect all elements”
         if self._octave_rf_input_port_number is None:
             raise AttributeError("This element has no connection ot octave RF-in, cannot set downconversion")
 
         if lo_source is None:
             lo_source = self.lo_source
 
-        self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_lo_source(
-            lo_source, ignore_shared_errors=True
-        )
-        self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_rf_source(RFInputRFSource.RF_in)
-        is_internal = lo_source in {RFInputLOSource.Internal, RFInputLOSource.Analyzer}
-
-        if lo_frequency is not None and is_internal:
-            self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_lo_frequency(
-                source_name=lo_source, frequency=lo_frequency
+        if self._downconversion_client:
+            self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_lo_source(
+                lo_source, ignore_shared_errors=True
+            )
+            self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_rf_source(
+                RFInputRFSource.RF_in
             )
+            is_internal = lo_source in {RFInputLOSource.Internal, RFInputLOSource.Analyzer}
+
+            if lo_frequency is not None and is_internal:
+                self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_lo_frequency(
+                    source_name=lo_source, frequency=lo_frequency
+                )
 
-    def _set_downconversion_if_mode(self, if_mode_i: IFMode = IFMode.direct, if_mode_q: IFMode = IFMode.direct):
+    def _set_downconversion_if_mode(self, if_mode_i: IFMode = IFMode.direct, if_mode_q: IFMode = IFMode.direct) -> None:
         if self._octave_rf_input_port_number is None:
             raise AttributeError("This element has no connection ot octave RF-in, cannot set downconversion")
-        self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_if_mode_i(if_mode_i)
-        self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_if_mode_q(if_mode_q)
+        if self._downconversion_client:
+            self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_if_mode_i(if_mode_i)
+            self._downconversion_client.rf_inputs[self._octave_rf_input_port_number].set_if_mode_q(if_mode_q)
 
-    def set_clock(self, clock_type: ClockType, frequency: Optional[ClockFrequency]):
+    def set_clock(self, clock_type: ClockType, frequency: Optional[ClockFrequency]) -> None:
         """
         This function will set the octave clock type - internal, external or buffered.
         It can also set the clock frequency - 10, 100 or 1000 MHz
 
         :param clock_type: ClockType
         :param frequency: ClockFrequency
         """
```

### Comparing `qm_qua-1.1.1/qm/elements/native_elements.py` & `qm_qua-1.1.2/qm/elements/native_elements.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,110 +1,97 @@
-from typing import Tuple, Union, List, Optional, Sequence
+from typing import List, Tuple, Union, Optional, Sequence, cast
 
-import betterproto
 import numpy
+import betterproto
 from dependency_injector.wiring import Provide, inject
 
 from qm.api.frontend_api import FrontendApi
+from qm.grpc.general_messages import Matrix
+from qm.grpc.qua_config import QuaConfigDacPortReference
 from qm.api.models.capabilities import ServerCapabilities
-from qm.api.models.devices import AnalogOutputPortFilter, MixerInfo
+from qm.elements.basic_element import BasicElement, logger
+from qm.api.models.devices import MixerInfo, AnalogOutputPortFilter
 from qm.containers.capabilities_container import CapabilitiesContainer
-from qm.elements.basic_element import logger, BasicElement
-from qm.grpc.qua_config import QuaConfigDacPortReference
-from qm.type_hinting.general import NumpySupportedFloat
-from qm.utils import fix_object_data_type
-from qm.grpc.general_messages import Matrix
-
-
-def _fix_offset(offset):
-    if offset == 0:
-        offset = float(offset)
-    if not isinstance(offset, (numpy.floating, float)):
-        raise TypeError("offset must be a float or a tuple of floats")
-
-    offset = fix_object_data_type(offset)
-    return offset
+from qm.type_hinting.general import NumpySupportedFloat, NumpySupportedNumber
 
 
 def _set_single_output_port_dc_offset(
     frontend_api: FrontendApi,
     machine_id: str,
     element_name: str,
     input_name: str,
-    offset,
-):
-    offset = _fix_offset(offset)
+    offset: NumpySupportedNumber,
+) -> None:
+    offset = float(offset)
     logger.debug(f"Setting DC offset of input '{input_name}' on element '{element_name}' to '{offset}'")
     frontend_api.set_output_dc_offset(machine_id, element_name, input_name, offset)
 
 
-def _create_taps_filter(feedforward, feedback):
+def _create_taps_filter(
+    feedforward: Union[Sequence[NumpySupportedFloat], None], feedback: Union[Sequence[NumpySupportedFloat], None]
+) -> AnalogOutputPortFilter:
     for name, instance in zip(["feedforward", "feedback"], [feedforward, feedback]):
         if instance is not None and not isinstance(instance, (numpy.ndarray, List)):
             raise TypeError(f"{name} must be None, a list, or a numpy array. Got {type(instance)}.")
     if isinstance(feedforward, numpy.ndarray):
         feedforward = feedforward.tolist()
     if isinstance(feedback, numpy.ndarray):
         feedback = feedback.tolist()
-    return AnalogOutputPortFilter(feedforward=feedforward, feedback=feedback)
+    return AnalogOutputPortFilter(feedforward=cast(List[float], feedforward), feedback=cast(List[float], feedback))
 
 
 @inject
 def static_set_mixer_correction(
     frontend_api: FrontendApi,
     machine_id: str,
     mixer: str,
     intermediate_frequency: Union[int, float],
     lo_frequency: Union[int, float],
     values: Tuple[float, float, float, float],
     capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities],
-):
+) -> None:
     # TODO - this function is here (and not under MixedInputsElement) to support backwards the direct calling to mixer
     #  Once it is changed, one can put this function under the element
 
     if not isinstance(values, (tuple, list)) or len(values) != 4:
         raise Exception("correction values must have 4 items")
 
-    correction_matrix = Matrix(*[fix_object_data_type(x) for x in values])
+    float_values = [float(x) for x in values]
+    correction_matrix = Matrix(*float_values)
 
+    mixer_lo_frequency_double = 0.0
+    mixer_intermediate_frequency_double = 0.0
     if capabilities.supports_double_frequency:
-        frequencies = {
-            "lo_frequency_double": float(lo_frequency),
-            "intermediate_frequency_double": abs(float(intermediate_frequency)),
-        }
-    else:
-        frequencies = {
-            "lo_frequency": int(lo_frequency),
-            "intermediate_frequency": abs(int(intermediate_frequency)),
-        }
+        mixer_lo_frequency_double = float(lo_frequency)
+        mixer_intermediate_frequency_double = abs(float(intermediate_frequency))
 
     mixer_info = MixerInfo(
         mixer=mixer,
         frequency_negative=intermediate_frequency < 0,
-        **frequencies,
+        lo_frequency=int(lo_frequency),
+        intermediate_frequency=abs(int(intermediate_frequency)),
+        lo_frequency_double=mixer_lo_frequency_double,
+        intermediate_frequency_double=mixer_intermediate_frequency_double,
     )
     frontend_api.set_correction(machine_id, mixer_info, correction_matrix)
 
 
 class SingleInputElement(BasicElement):
     @property
     def port(self) -> QuaConfigDacPortReference:
         return self._config.single_input.port
 
-    def get_output_dc_offset(self) -> float:
-        pass
-
-    def set_output_dc_offset(self, offset: float):
+    def set_output_dc_offset(self, offset: float) -> None:
         _set_single_output_port_dc_offset(self._frontend, self._id, self._name, "single", offset)
 
     def set_output_filter(
         self,
         feedforward: Union[Sequence[NumpySupportedFloat], None],
         feedback: Union[Sequence[NumpySupportedFloat], None],
-    ):
+    ) -> None:
         analog_filter = _create_taps_filter(feedforward, feedback)
         self._frontend.set_output_filter_taps(self._id, self._name, "single", analog_filter)
 
 
 class MultipleInputsElement(BasicElement):
     pass
 
@@ -119,68 +106,66 @@
         return self._config.mix_inputs.i
 
     @property
     def q_port(self) -> QuaConfigDacPortReference:
         return self._config.mix_inputs.q
 
     @property
-    def lo_frequency(self) -> int:
+    @inject
+    def lo_frequency(self, capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities]) -> float:
+        if capabilities.supports_double_frequency:
+            return self._config.mix_inputs.lo_frequency_double
         return self._config.mix_inputs.lo_frequency
 
     @lo_frequency.setter
     @inject
     def lo_frequency(
         self, value: float, capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities]
-    ):
-        freq = fix_object_data_type(value)
+    ) -> None:
+        freq = float(value)
         logger.debug(f"Setting element '{self._name}' intermediate frequency to '{freq}'.")
+        self._config.mix_inputs.lo_frequency = int(freq)
+        self._config.mix_inputs.lo_frequency_double = 0.0
         if capabilities.supports_double_frequency:
             self._config.mix_inputs.lo_frequency_double = float(freq)
-            self._config.mix_inputs.lo_frequency = 0
-        else:
-            self._config.mix_inputs.lo_frequency = int(freq)
-            self._config.mix_inputs.lo_frequency_double = 0.0
 
     @property
     def mixer(self) -> str:
         return self._config.mix_inputs.mixer
 
     @property
     def has_octave_params(self) -> bool:
         return betterproto.serialized_on_wire(self._config.mix_inputs.octave_params)
 
-    def get_output_dc_offset(self, port_name) -> float:
-        pass
-
-    def set_output_dc_offset(self, i_offset: Optional[float] = None, q_offset: Optional[float] = None):
+    def set_output_dc_offset(self, i_offset: Optional[float] = None, q_offset: Optional[float] = None) -> None:
         if i_offset is not None:
             _set_single_output_port_dc_offset(self._frontend, self._id, self._name, "I", i_offset)
         if q_offset is not None:
             _set_single_output_port_dc_offset(self._frontend, self._id, self._name, "Q", q_offset)
 
     def set_output_filter(
         self,
         input_name: str,
         feedforward: Union[Sequence[NumpySupportedFloat], None],
         feedback: Union[Sequence[NumpySupportedFloat], None],
-    ):
+    ) -> None:
         analog_filter = _create_taps_filter(feedforward, feedback)
         self._frontend.set_output_filter_taps(
             self._id,
             self._name,
             input_name,
             analog_filter,
         )
 
     def set_mixer_correction(
         self,
         intermediate_frequency: int,
         lo_frequency: int,
         values: Tuple[float, float, float, float],
-    ):
+    ) -> None:
         static_set_mixer_correction(
             self._frontend,
             self._id,
             mixer=self.mixer,
             intermediate_frequency=intermediate_frequency,
             lo_frequency=lo_frequency,
             values=values,
```

### Comparing `qm_qua-1.1.1/qm/elements_db.py` & `qm_qua-1.1.2/qm/elements_db.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from typing import Dict, Union, Optional
+from typing import Dict, Optional
 
 import betterproto
-from octave_sdk import OctaveLOSource, OctaveOutput, Octave
+from octave_sdk import Octave, OctaveOutput, OctaveLOSource  # type: ignore[import]
 
+from qm.octave import QmOctaveConfig
 from qm.api.frontend_api import FrontendApi
 from qm.elements.basic_element import BasicElement
+from qm.elements.element_with_octave import ElementWithOctave
+from qm.grpc.octave_models import OctaveIfInputPort, OctaveIfInputPortName
 from qm.elements.native_elements import (
-    SingleInputElement,
     MixInputsElement,
+    SingleInputElement,
     MultipleInputsElement,
     SingleInputCollectionElement,
 )
-from qm.elements.element_with_octave import ElementWithOctave
 from qm.grpc.qua_config import (
     QuaConfig,
-    QuaConfigMultipleInputs,
     QuaConfigMixInputs,
     QuaConfigSingleInput,
-    QuaConfigSingleInputCollection,
+    QuaConfigMultipleInputs,
     QuaConfigDacPortReference,
+    QuaConfigSingleInputCollection,
 )
-from qm.grpc.octave_models import OctaveIfInputPort, OctaveIfInputPortName
-from qm.octave import QmOctaveConfig
-
 
 MaybeOctaveInputPort = Optional[OctaveIfInputPort]
 
 
 class ElementNotFound(KeyError):
-    def __init__(self, key):
+    def __init__(self, key: str):
         self._key = key
 
     def __str__(self) -> str:
         return f"Element with the key {self._key} was not found."
 
 
 class UnknownElementType(ValueError):
@@ -48,46 +47,52 @@
         self._i = i_port
         self._q = q_port
 
 
 class OnlyOneConnectedPort(OctaveConnectionError):
     def __str__(self) -> str:
         connected_port = self._i or self._q
+        assert isinstance(connected_port, OctaveIfInputPort)
         return (
             f"Only {connected_port.port_name.name} is connected to octave, while the other isn't. "
             f"Either both of them should be connected, or none of them"
         )
 
 
 class DifferentOctavesForTheSameElement(OctaveConnectionError):
     def __str__(self) -> str:
+        assert isinstance(self._i, OctaveIfInputPort)
+        assert isinstance(self._q, OctaveIfInputPort)
         return (
             f"The I port is connected to {self._i.device_name} and Q is connected to {self._q.device_name}. "
             f"Both of them should be connected to the same Octave, with the same number (i.e. I1 & Q1 etc.)."
         )
 
 
 class DifferentOctaveInputsForTheSameElement(OctaveConnectionError):
     def __str__(self) -> str:
+        assert isinstance(self._i, OctaveIfInputPort)
+        assert isinstance(self._q, OctaveIfInputPort)
         return (
             f"The I port is connected to {self._i.port_name.name} and Q is connected to {self._q.port_name.name}. "
             f"Both of them should be connected to the same Octave, with the same number (i.e. I1 & Q1 etc.)."
         )
 
 
 class BothPortsConnectedToTheSameOctavePort(OctaveConnectionError):
     def __str__(self) -> str:
+        assert isinstance(self._i, OctaveIfInputPort)
         return (
             f"Both I and Q port are connected to {(self._i.device_name, self._i.port_name.name)}. "
             f"This is probably a configuration mistake."
         )
 
 
 class ElementsDB(Dict[str, BasicElement]):
-    def __missing__(self, key) -> None:
+    def __missing__(self, key: str) -> None:
         raise ElementNotFound(key)
 
 
 INPUTS_TO_ELEMENTS = {
     type(None): BasicElement,
     QuaConfigMixInputs: MixInputsElement,
     QuaConfigSingleInput: SingleInputElement,
@@ -150,36 +155,29 @@
             else:
                 return {}
         return self._octave_config.get_lo_loopbacks_by_octave(octave_name)
 
     @staticmethod
     def _validate_octave_is_connected_properly(
         i_octave_input_port: MaybeOctaveInputPort, q_octave_input_port: MaybeOctaveInputPort
-    ):
+    ) -> None:
         if i_octave_input_port is None and q_octave_input_port is None:
             return
         if (i_octave_input_port is None) != (q_octave_input_port is None):
             raise OnlyOneConnectedPort(i_octave_input_port, q_octave_input_port)
+        assert isinstance(i_octave_input_port, OctaveIfInputPort)
+        assert isinstance(q_octave_input_port, OctaveIfInputPort)
         if i_octave_input_port.device_name != q_octave_input_port.device_name:
             raise DifferentOctavesForTheSameElement(i_octave_input_port, q_octave_input_port)
         if i_octave_input_port.port_name.name[-1] != q_octave_input_port.port_name.name[-1]:
             raise DifferentOctaveInputsForTheSameElement(i_octave_input_port, q_octave_input_port)
         if i_octave_input_port == q_octave_input_port:
             raise BothPortsConnectedToTheSameOctavePort(i_octave_input_port, q_octave_input_port)
 
-    def add_octave(
-        self,
-        element: Union[MixInputsElement, SingleInputElement, MultipleInputsElement, SingleInputCollectionElement],
-    ) -> Union[
-        MixInputsElement,
-        SingleInputElement,
-        MultipleInputsElement,
-        SingleInputCollectionElement,
-        ElementWithOctave,
-    ]:
+    def add_octave(self, element: BasicElement) -> BasicElement:
         if not isinstance(element, MixInputsElement):
             return element
 
         i_octave_input_port = self._get_connections_to_octave(element.i_port)
         q_octave_input_port = self._get_connections_to_octave(element.q_port)
 
         self._validate_octave_is_connected_properly(i_octave_input_port, q_octave_input_port)
```

### Comparing `qm_qua-1.1.1/qm/grpc/compiler/__init__.py` & `qm_qua-1.1.2/qm/grpc/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/errors/__init__.py` & `qm_qua-1.1.2/qm/grpc/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/frontend/__init__.py` & `qm_qua-1.1.2/qm/grpc/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/general_messages/__init__.py` & `qm_qua-1.1.2/qm/grpc/general_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/job_manager/__init__.py` & `qm_qua-1.1.2/qm/grpc/job_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/octave_models/__init__.py` & `qm_qua-1.1.2/qm/grpc/octave_models/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/qm_api/__init__.py` & `qm_qua-1.1.2/qm/grpc/qm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/qm_manager/__init__.py` & `qm_qua-1.1.2/qm/grpc/qm_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/qua/__init__.py` & `qm_qua-1.1.2/qm/grpc/qua/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/qua_config/__init__.py` & `qm_qua-1.1.2/qm/grpc/qua_config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,17 +290,14 @@
     )
     single_input_collection: "QuaConfigSingleInputCollection" = (
         betterproto.message_field(50, group="element_inputs_one_of")
     )
     multiple_inputs: "QuaConfigMultipleInputs" = betterproto.message_field(
         51, group="element_inputs_one_of"
     )
-    up_converted: "QuaConfigUpConverted" = betterproto.message_field(
-        52, group="element_inputs_one_of"
-    )
     time_of_flight: Optional[int] = betterproto.message_field(
         7, wraps=betterproto.TYPE_UINT32
     )
     smearing: Optional[int] = betterproto.message_field(
         8, wraps=betterproto.TYPE_UINT32
     )
     intermediate_frequency: Optional[int] = betterproto.message_field(
```

### Comparing `qm_qua-1.1.1/qm/grpc/quantum_simulator/v1/__init__.py` & `qm_qua-1.1.2/qm/grpc/quantum_simulator/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/grpc/results_analyser/__init__.py` & `qm_qua-1.1.2/qm/grpc/results_analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/io/qualang/api/v1/__init__.py` & `qm_qua-1.1.2/qm/io/qualang/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/jobs/base_job.py` & `qm_qua-1.1.2/qm/jobs/base_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import datetime
-from typing import Optional, List
+from typing import List, Optional
 from typing_extensions import Protocol
 
 import betterproto
 
+from qm.type_hinting import Value
+from qm.persistence import BaseStore
+from qm.exceptions import QmQuaException
+from qm.utils import deprecate_to_property
 from qm.api.frontend_api import FrontendApi
+from qm.grpc.frontend import JobExecutionStatus
 from qm.api.job_manager_api import JobManagerApi
 from qm.api.models.capabilities import ServerCapabilities
-from qm.exceptions import QmQuaException
-from qm.grpc.frontend import JobExecutionStatus
-from qm.persistence import BaseStore
-from qm.type_hinting import Value
-from qm.utils import deprecate_to_property
 
 
 class JobStateProtocol(Protocol):
     added_by: Optional[str]
     time_added: Optional[datetime.datetime]
```

### Comparing `qm_qua-1.1.1/qm/jobs/job_queue.py` & `qm_qua-1.1.2/qm/jobs/job_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 from typing import List, Optional
 
-from qm.jobs.pending_job import QmPendingJob
+from qm.persistence import BaseStore
+from qm.program.program import Program
+from qm.grpc.qua_config import QuaConfig
 from qm.api.frontend_api import FrontendApi
+from qm.jobs.pending_job import QmPendingJob
 from qm.api.job_manager_api import JobManagerApi
 from qm.api.models.capabilities import ServerCapabilities
 from qm.api.models.compiler import CompilerOptionArguments
-from qm.api.models.jobs import InsertDirection, PendingJobData
-from qm.grpc.qua_config import QuaConfig
-from qm.persistence import BaseStore
-from qm.program.program import Program
-from qm.program._execution_overrides_schema import ExecutionOverridesSchema
+from qm.api.models.jobs import PendingJobData, InsertDirection
 from qm.type_hinting.exceution_overrides import ExecutionOverridesType
+from qm.program._execution_overrides_schema import ExecutionOverridesSchema
 
 logger = logging.getLogger(__name__)
 
 
 class JobNotFoundError(Exception):
     pass
```

### Comparing `qm_qua-1.1.1/qm/jobs/pending_job.py` & `qm_qua-1.1.2/qm/jobs/pending_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
-from typing import cast
 
 from qm.jobs.qm_job import QmJob
-from qm.exceptions import JobCancelledError, ErrorJobStateError, UnknownJobStateError
-from qm.grpc.frontend import JobExecutionStatus
 from qm.jobs.base_job import QmBaseJob
 from qm.utils import run_until_with_timeout
+from qm.grpc.frontend import JobExecutionStatus
+from qm.exceptions import JobCancelledError, ErrorJobStateError, UnknownJobStateError
 
 logger = logging.getLogger(__name__)
 
 INVALID_QUEUE_POSITION = -1
 
 
 class QmPendingJob(QmBaseJob):
@@ -72,25 +71,22 @@
                 job_id=self._id,
                 machine_id=self._machine_id,
                 frontend_api=self._frontend,
                 capabilities=self._capabilities,
                 store=self._store,
             )
 
-        return cast(
-            QmJob,
-            run_until_with_timeout(
-                on_iteration_callback=on_iteration,
-                on_complete_callback=on_complete,
-                timeout=timeout,
-                loop_interval=0.01,
-                timeout_message=f"job {self._id} was not started in time. "
-                f"Check the QMApp for errors and try reloading the version. "
-                f"Please also inform QM about this issue. ",
-            ),
+        return run_until_with_timeout(
+            on_iteration_callback=on_iteration,
+            on_complete_callback=on_complete,
+            timeout=timeout,
+            loop_interval=0.01,
+            timeout_message=f"job {self._id} was not started in time. "
+            f"Check the QMApp for errors and try reloading the version. "
+            f"Please also inform QM about this issue. ",
         )
 
     def cancel(self) -> bool:
         """Removes the job from the queue
 
         Returns:
             true if the operation was successful
```

### Comparing `qm_qua-1.1.1/qm/jobs/running_qm_job.py` & `qm_qua-1.1.2/qm/jobs/running_qm_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import warnings
 from enum import Enum
 from typing import Tuple
-from qm.results.streaming_result_fetcher import StreamingResultFetcher
+
 from qm._report import ExecutionReport
-from qm.api.job_result_api import JobResultServiceApi
-from qm.grpc.general_messages import Matrix
 from qm.jobs.base_job import QmBaseJob
 from qm.utils import deprecation_message
+from qm.grpc.general_messages import Matrix
+from qm.api.job_result_api import JobResultServiceApi
+from qm.results.streaming_result_fetcher import StreamingResultFetcher
 
 
 class AcquiringStatus(Enum):
     AcquireStopped = 0
     NoDataToAcquire = 1
     HasDataToAcquire = 2
```

### Comparing `qm_qua-1.1.1/qm/jobs/simulated_job.py` & `qm_qua-1.1.2/qm/jobs/simulated_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import json as _json
 import warnings
-from dataclasses import dataclass
+import json as _json
 from io import BytesIO
-from typing import Dict, BinaryIO, Any, Optional, Callable
+from dataclasses import dataclass
+from typing import Any, Dict, BinaryIO, Callable, Optional
 
-import betterproto
 import numpy
+import betterproto
 import numpy.typing
-from betterproto.lib.google.protobuf import Value, Struct
 from numpy.lib import format as _format
+from betterproto.lib.google.protobuf import Value, Struct
 
-from qm.grpc.results_analyser import SimulatorSamplesResponseHeader, SimulatorSamplesResponseData
-from qm.type_hinting.simulator_types import AnalogOutputsType, DigitalOutputsType, WaveformInPortsType
+from qm.persistence import BaseStore
 from qm.utils import deprecation_message
 from qm.utils.async_utils import run_async
 from qm.api.frontend_api import FrontendApi
-from qm.api.models.capabilities import ServerCapabilities
-from qm.api.simulation_api import SimulationApi
 from qm.exceptions import QMSimulationError
-from qm.grpc.frontend import SimulatedResponsePart
+from qm.waveform_report import WaveformReport
+from qm.api.simulation_api import SimulationApi
 from qm.jobs.running_qm_job import RunningQmJob
-from qm.persistence import BaseStore
+from qm.grpc.frontend import SimulatedResponsePart
+from qm.api.models.capabilities import ServerCapabilities
 from qm.results.simulator_samples import SimulatorSamples
-from qm.waveform_report import WaveformReport
+from qm.grpc.results_analyser import SimulatorSamplesResponseData, SimulatorSamplesResponseHeader
+from qm.type_hinting.simulator_types import AnalogOutputsType, DigitalOutputsType, WaveformInPortsType
 
 
 @dataclass
 class DensityMatrix:
     timestamp: int
     data: numpy.typing.NDArray[numpy.cdouble]
 
@@ -205,15 +205,15 @@
         run_async(self._pull_simulator_samples(include_analog, include_digital, writer, data_writer))
 
         data_writer.seek(0)
         for d in data_writer:
             writer.write(d)
 
         writer.seek(0)
-        ret: numpy.typing.NDArray[numpy.generic] = numpy.load(writer)  # type: ignore[no-untyped-call]
+        ret: numpy.typing.NDArray[numpy.generic] = numpy.load(writer)
         return ret
 
     def get_simulated_samples(self, include_analog: bool = True, include_digital: bool = True) -> SimulatorSamples:
         """
         Obtain the output samples of a QUA program simulation.
 
         Samples are returned in an object that holds the controllers in the current simulation,
```

### Comparing `qm_qua-1.1.1/qm/logging_utils.py` & `qm_qua-1.1.2/qm/logging_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from logging import config
+
 from qm.user_config import UserConfig
 
 
-def config_loggers(user_config: UserConfig):
+def config_loggers(user_config: UserConfig) -> None:
     config.dictConfig(user_config.logging_config_dict)
 
 
 def set_logging_level(level: int) -> None:
     """Sets the logging level of the qm-qua module ("qm")
     See `Messages control <https://qm-docs.qualang.io/guides/error#messages-control>`__ for more information.
```

### Comparing `qm_qua-1.1.1/qm/octave/__init__.py` & `qm_qua-1.1.2/qm/octave/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from octave_sdk import (
-    OctaveOutput,
+    IFMode,
     ClockType,
+    OctaveOutput,
+    RFOutputMode,
     ClockFrequency,
     OctaveLOSource,
-    IFMode,
     RFInputLOSource,
     RFInputRFSource,
-    RFOutputMode,
 )
+
 from qm.octave.octave_config import QmOctaveConfig
 from qm.octave.calibration_db import octave_output_mixer_name
 
 __all__ = [
     "OctaveOutput",
     "ClockType",
     "ClockFrequency",
```

### Comparing `qm_qua-1.1.1/qm/octave/_calibration_config.py` & `qm_qua-1.1.2/qm/octave/_calibration_config.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/octave/_calibration_program.py` & `qm_qua-1.1.2/qm/octave/_calibration_program.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from qm.octave._calibration_config import offset_amp
 from qm.qua import (
-    assign,
+    amp,
+    if_,
     for_,
-    reset_phase,
-    align,
     play,
-    measure,
-    dual_demod,
-    if_,
     save,
-    amp,
-    update_correction,
+    wait,
+    align,
     else_,
+    fixed,
+    assign,
     while_,
-    program,
     declare,
-    fixed,
+    measure,
+    program,
+    dual_demod,
+    reset_phase,
     declare_stream,
-    wait,
     stream_processing,
+    update_correction,
 )
 
 
 def _generate_program(calibration_parameters):
     n_average = calibration_parameters["average_iterations"]
     iterations = calibration_parameters["iterations"]
     keep_on = calibration_parameters["keep_on"]
```

### Comparing `qm_qua-1.1.1/qm/octave/calibration_db.py` & `qm_qua-1.1.2/qm/octave/calibration_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import logging
-from dataclasses import dataclass, asdict
 from pathlib import Path
-from typing import List, Dict, Union, Any, Optional
+from dataclasses import asdict, dataclass
+from typing import Any, Dict, List, Union, Optional
 
-from tinydb import TinyDB, Query
+from tinydb import Query, TinyDB
 
 from qm.type_hinting.config_types import DictQuaConfig
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
```

### Comparing `qm_qua-1.1.1/qm/octave/enums.py` & `qm_qua-1.1.2/qm/octave/enums.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import warnings
 
+from octave_sdk.octave import IFMode, ClockInfo
 from octave_sdk import (
-    RFInputRFSource,
+    ClockType,
+    OctaveOutput,
     RFOutputMode,
+    ClockFrequency,
     OctaveLOSource,
     RFInputLOSource,
-    ClockType,
-    ClockFrequency,
-    OctaveOutput,
+    RFInputRFSource,
 )
-from octave_sdk.octave import IFMode, ClockInfo
 
 __all__ = [
     "RFInputRFSource",
     "RFOutputMode",
     "OctaveLOSource",
     "RFInputLOSource",
     "ClockType",
```

### Comparing `qm_qua-1.1.1/qm/octave/octave_config.py` & `qm_qua-1.1.2/qm/octave/octave_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import dataclasses
-import logging
 import re
+import logging
 import warnings
-from typing import Dict, Optional, Tuple, TypeVar, Generic, List, Union
+import dataclasses
+from typing import Dict, List, Tuple, Union, Generic, TypeVar, Optional
+
 from deprecation import deprecated
 from octave_sdk import OctaveOutput, OctaveLOSource
 
 from qm.octave.calibration_db import CalibrationDB
 
-
 logger = logging.getLogger(__name__)
 
 ConnectionMapping = Dict[Tuple[str, int], Tuple[str, str]]
 
 DEFAULT_CONNECTIONS = {
     1: "I1",
     2: "Q1",
@@ -72,15 +72,15 @@
 
 
 def _convert_number_to_octave_port(name: str, port: int) -> List:
     return [(name, f"I{port}"), (name, f"Q{port}")]
 
 
 class QmOctaveConfig:
-    def __init__(self, fan=None):
+    def __init__(self, fan=None) -> None:
         self._devices: Dict[str, ConnectionInfo] = {}
         self._calibration_db_path: Optional[str] = None
         self._loopbacks: Optional[Dict[LoopbackInfo[OctaveLOSource], LoopbackInfo[OctaveOutput]]] = None
         self._opx_octave_port_mapping: Optional[ConnectionMapping] = None
         self._calibration_db: Optional[CalibrationDB] = None
         self._fan = fan
```

### Comparing `qm_qua-1.1.1/qm/octave/octave_manager.py` & `qm_qua-1.1.2/qm/octave/octave_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,42 +1,27 @@
-from time import perf_counter
-import contextlib
 import logging
 import warnings
-from collections import defaultdict
+import contextlib
 from enum import Enum
+from time import perf_counter
+from collections import defaultdict
+from typing import TYPE_CHECKING, Dict, List, Tuple, Optional
 
 from octave_sdk.octave import ClockInfo
+from octave_sdk import IFMode, ClockType, RFOutputMode, ClockFrequency, OctaveLOSource, RFInputLOSource, RFInputRFSource
 
 from qm import QuantumMachine
-from qm.api.models.capabilities import ServerCapabilities
 from qm.exceptions import OpenQmException
-from qm.octave._calibration_config import (
-    _prep_config,
-    _get_frequencies,
-)
-from qm.octave.calibration_db import (
-    CalibrationResult,
-    octave_output_mixer_name,
-)
-from octave_sdk import (
-    OctaveLOSource,
-    RFInputRFSource,
-    ClockType,
-    ClockFrequency,
-    RFOutputMode,
-    RFInputLOSource,
-    IFMode,
-)
-from qm.octave.octave_config import _convert_octave_port_to_number, QmOctaveConfig
-
-from typing import Dict, Tuple, Optional, List, TYPE_CHECKING
+from qm.api.models.capabilities import ServerCapabilities
+from qm.octave._calibration_config import _prep_config, _get_frequencies
+from qm.octave.calibration_db import CalibrationResult, octave_output_mixer_name
+from qm.octave.octave_config import QmOctaveConfig, _convert_octave_port_to_number
 
 if TYPE_CHECKING:
-    from qm.QuantumMachinesManager import QuantumMachinesManager
+    from qm.quantum_machines_manager import QuantumMachinesManager
 
 try:
     from octave_sdk import Octave
 
     OCTAVE_SDK_LOADED = True
 
 except ModuleNotFoundError:
```

### Comparing `qm_qua-1.1.1/qm/octave/qm_octave.py` & `qm_qua-1.1.2/qm/octave/qm_octave.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import warnings
-from typing import Dict, Tuple, Union, List, Optional, ContextManager
+from typing import Dict, List, Tuple, Union, Optional, ContextManager
 
 from octave_sdk.octave import ClockInfo
-from qm.elements.element_with_octave import ElementWithOctave
+from octave_sdk import IFMode, ClockType, RFOutputMode, ClockFrequency, OctaveLOSource, RFInputLOSource
 
 from qm.elements_db import ElementsDB
 from qm.octave.calibration_db import CalibrationResult
-from octave_sdk import (
-    OctaveLOSource,
-    RFOutputMode,
-    RFInputLOSource,
-    IFMode,
-    ClockType,
-    ClockFrequency,
-)
-from qm.octave.octave_manager import OctaveManager, ClockMode
+from qm.elements.element_with_octave import ElementWithOctave
+from qm.octave.octave_manager import ClockMode, OctaveManager
 
 
 class ElementHasNoOctaveError(Exception):
     pass
 
 
 class QmOctave:
```

### Comparing `qm_qua-1.1.1/qm/persistence.py` & `qm_qua-1.1.2/qm/persistence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 from pathlib import Path
-from typing import BinaryIO
+from typing import BinaryIO, Optional
 
 
 class BinaryAsset(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def for_writing(self) -> BinaryIO:
         raise NotImplementedError()
 
@@ -28,17 +28,17 @@
         raise NotImplementedError()
 
 
 class FileBinaryAsset(BinaryAsset):
     def __init__(self, path: Path) -> None:
         super().__init__()
         self._path = path
-        self._opened_fd = None
+        self._opened_fd: Optional[BinaryIO] = None
 
-    def close(self):
+    def close(self) -> None:
         if self._opened_fd:
             self._opened_fd.close()
 
     def for_writing(self) -> BinaryIO:
         self.close()
         self._opened_fd = self._path.open("wb")
         return self._opened_fd
@@ -50,15 +50,15 @@
 
 
 class SimpleFileStore(BaseStore):
     def __init__(self, root: str = ".") -> None:
         super().__init__()
         self._root = Path(root).absolute()
 
-    def _job_path(self, job_id: str):
+    def _job_path(self, job_id: str) -> Path:
         path = Path(f"{self._root}/{job_id}")
         path.mkdir(parents=True, exist_ok=True)
         return path
 
     def job_named_result(self, job_id: str, name: str) -> BinaryAsset:
         return FileBinaryAsset(self._job_path(job_id).joinpath(f"result_{name}.npy"))
```

### Comparing `qm_qua-1.1.1/qm/program/ConfigBuilder.py` & `qm_qua-1.1.2/qm/program/ConfigBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import cast
 
-from qm.grpc.qua_config import QuaConfig, QuaConfigPulseDecOperation, QuaConfigQuaConfigV1
 from qm.type_hinting.config_types import DictQuaConfig
+from qm.grpc.qua_config import QuaConfig, QuaConfigQuaConfigV1, QuaConfigPulseDecOperation
 
 
 def convert_msg_to_config(config: QuaConfig) -> DictQuaConfig:
     msg_dict = config.to_dict()
 
     if "v1Beta" in msg_dict:
         return _convert_v1_beta(msg_dict["v1Beta"])
@@ -17,22 +17,22 @@
     if mixers is None:
         return {}
 
     ret = {}
     for name, data in mixers.items():
         temp_list = []
         for correction in data["correction"]:
-            if "frequencyDouble" in correction:
+            if "frequencyDouble" in data:
                 frequency = float(correction["frequencyDouble"])
             elif "frequency" in correction:
                 frequency = float(correction["frequency"])
             else:
                 frequency = 0.0
 
-            if "frequencyNegative" in correction:
+            if "frequencyNegative" in data:
                 if bool(correction["frequencyNegative"]):
                     frequency = -frequency
 
             if "loFrequencyDouble" in correction:
                 lo_frequency = float(correction["loFrequencyDouble"])
             elif "loFrequency" in correction:
                 lo_frequency = float(correction["loFrequency"])
@@ -444,17 +444,19 @@
 
 def _convert_controller_digital_outputs(outputs):
     if outputs is None:
         return {}
 
     ret = {}
     for name, data in outputs.items():
-        port_info = {"shareable": False}
+        port_info = {"shareable": False, "inverted": False}
         if "shareable" in data:
             port_info["shareable"] = data["shareable"]
+        if "inverted" in data:
+            port_info["inverted"] = data["inverted"]
         ret[int(name)] = port_info
     return ret
 
 
 def _convert_controller_digital_inputs(inputs):
     if inputs is None:
         return {}
```

### Comparing `qm_qua-1.1.1/qm/program/StatementsCollection.py` & `qm_qua-1.1.2/qm/program/StatementsCollection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Union, Tuple, TYPE_CHECKING, Optional, List
+from typing import TYPE_CHECKING, List, Tuple, Union, Optional
 
 import betterproto
 from betterproto.lib.google.protobuf import Empty
 
 import qm.grpc.qua as _qua
 from qm._loc import _get_loc
 from qm.exceptions import QmQuaException
 
 if TYPE_CHECKING:
     from qm.qua._dsl import _ResultSource
     from qm.qua._type_hinting import (
-        MeasurePulseType,
         PlayPulseType,
-        MessageExpressionType,
-        MessageVariableOrExpression,
         MessageVarType,
+        MeasurePulseType,
         MessageVariableType,
+        MessageExpressionType,
+        MessageVariableOrExpression,
     )
 
 
 class StatementsCollection:
     def __init__(self, body: _qua.QuaProgramStatementsCollection):
         self._body = body
```

### Comparing `qm_qua-1.1.1/qm/program/_ResultAnalysis.py` & `qm_qua-1.1.2/qm/program/_ResultAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Union
 
-from betterproto.lib.google.protobuf import ListValue, Value
+from betterproto.lib.google.protobuf import Value, ListValue
 
 from qm.grpc.qua import QuaResultAnalysis
 
 _RESULT_SYMBOL = "@re"
 
 
 class _ResultAnalysis:
```

### Comparing `qm_qua-1.1.1/qm/program/_execution_overrides_schema.py` & `qm_qua-1.1.2/qm/program/_execution_overrides_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from marshmallow_polyfield import PolyField
+from marshmallow import Schema, ValidationError, fields, post_load
 
-from marshmallow import Schema, fields, post_load, ValidationError
-
-from qm.grpc.frontend import ExecutionOverrides, WaveformOverride
+from qm.grpc.frontend import WaveformOverride, ExecutionOverrides
 
 
 def load_overrides(overrides):
     return ExecutionOverridesSchema().load(overrides)
 
 
 def _non_empty(v):
```

### Comparing `qm_qua-1.1.1/qm/program/_qua_config_schema.py` & `qm_qua-1.1.2/qm/program/_qua_config_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-from typing import List, Any, Mapping, Dict
 import logging
+from typing import Any, Dict, List, Mapping
 
 import betterproto
 import numpy as np
-from betterproto.lib.google.protobuf import Empty
-from dependency_injector.wiring import inject, Provide
-from marshmallow import (
-    Schema,
-    fields,
-    post_load,
-    ValidationError,
-    validates_schema,
-    validate,
-)
 from marshmallow_polyfield import PolyField
+from betterproto.lib.google.protobuf import Empty
+from dependency_injector.wiring import Provide, inject
+from marshmallow import Schema, ValidationError, fields, validate, post_load, validates_schema
 
+from qm.grpc import qua_config, octave_models
+from qm.exceptions import ConfigValidationException
+from qm.type_hinting.config_types import DictQuaConfig
 from qm.api.models.capabilities import ServerCapabilities
 from qm.containers.capabilities_container import CapabilitiesContainer
-from qm.exceptions import ConfigValidationException
+from qm.grpc.qua_config import QuaConfig, QuaConfigAnalogOutputPortFilter
 from qm.program._qua_config_to_pb import (
-    octave_connection_to_pb,
-    get_octave_loopbacks,
     OctaveConnectionAmbiguity,
     octave_params_to_pb,
+    get_octave_loopbacks,
+    octave_connection_to_pb,
 )
-
 from qm.program._validate_config_schema import (
-    validate_output_smearing,
     validate_oscillator,
     validate_output_tof,
-    validate_arbitrary_waveform,
     validate_used_inputs,
+    validate_output_smearing,
+    validate_arbitrary_waveform,
     validate_timetagging_parameters,
 )
-from qm.grpc import qua_config, octave_models
-from qm.grpc.qua_config import QuaConfigAnalogOutputPortFilter, QuaConfig
-from qm.type_hinting.config_types import DictQuaConfig
 
 logger = logging.getLogger(__name__)
 
 
 def validate_config_capabilities(pb_config, server_capabilities: ServerCapabilities):
     if not server_capabilities.supports_inverted_digital_output:
         for con_name, con in pb_config.v1_beta.controllers.items():
@@ -673,24 +665,22 @@
         data,
         capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities],
         **kwargs,
     ):
         item = qua_config.QuaConfigCorrectionEntry(correction=qua_config.QuaConfigMatrix(*data["correction"]))
 
         if "lo_frequency" in data:
+            item.lo_frequency = int(data["lo_frequency"])  # backwards compatibility
             if capabilities.supports_double_frequency:
                 item.lo_frequency_double = float(data["lo_frequency"])
-            else:
-                item.lo_frequency = int(data["lo_frequency"])  # backwards compatibility
 
         if "intermediate_frequency" in data:
+            item.frequency = abs(int(data["intermediate_frequency"]))  # backwards compatibility
             if capabilities.supports_double_frequency:
                 item.frequency_double = abs(float(data["intermediate_frequency"]))
-            else:
-                item.frequency = abs(int(data["intermediate_frequency"]))  # backwards compatibility
 
             item.frequency_negative = data["intermediate_frequency"] < 0
 
         item.correction = qua_config.QuaConfigMatrix(
             data["correction"][0],
             data["correction"][1],
             data["correction"][2],
@@ -808,15 +798,15 @@
     class Meta:
         title = "Sticky"
         description = "When defined, makes the element sticky"
 
     @post_load(pass_many=False)
     def build(self, data, **kwargs):
         item = qua_config.QuaConfigSticky()
-        item.duration = data.get("duration")
+        item.duration = data.get("duration", 1)
         item.analog = data.get("analog")
         if "digital" in data:
             item.digital = data.get("digital")
         return item
 
 
 class MixInputSchema(Schema):
@@ -842,25 +832,23 @@
     def build(
         self,
         data,
         capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities],
         **kwargs,
     ):
         lo_frequency = data.get("lo_frequency", 0)
-        if capabilities.supports_double_frequency:
-            frequency = {"lo_frequency_double": float(lo_frequency)}
-        else:
-            frequency = {"lo_frequency": int(lo_frequency)}
 
         item = qua_config.QuaConfigMixInputs(
             i=qua_config.QuaConfigDacPortReference(controller=data["I"][0], number=data["I"][1]),
             q=qua_config.QuaConfigDacPortReference(controller=data["Q"][0], number=data["Q"][1]),
             mixer=data.get("mixer", ""),
-            **frequency,
+            lo_frequency=int(lo_frequency),
         )
+        if capabilities.supports_double_frequency:
+            item.lo_frequency_double = float(lo_frequency)
         if "octave_params" in data:
             item.octave_params = data["octave_params"]
         return item
 
 
 class SingleInputCollectionSchema(Schema):
     inputs = fields.Dict(
@@ -921,24 +909,23 @@
         self,
         data,
         capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities],
         **kwargs,
     ):
         osc = qua_config.QuaConfigOscillator()
         if "intermediate_frequency" in data and data["intermediate_frequency"] is not None:
+            osc.intermediate_frequency = int(data["intermediate_frequency"])
             if capabilities.supports_double_frequency:
-                osc.intermediate_frequency_double = data["intermediate_frequency"]
-            else:
-                osc.intermediate_frequency = int(data["intermediate_frequency"])
+                osc.intermediate_frequency_double = float(data["intermediate_frequency"])
+
         if "mixer" in data and data["mixer"] is not None:
             osc.mixer.mixer = data["mixer"]
+            osc.mixer.lo_frequency = int(data.get("lo_frequency", 0))
             if capabilities.supports_double_frequency:
-                osc.mixer.lo_frequency_double = data.get("lo_frequency", 0.0)
-            else:
-                osc.mixer.lo_frequency = int(data.get("lo_frequency", 0))
+                osc.mixer.lo_frequency_double = float(data.get("lo_frequency", 0.0))
 
         return osc
 
 
 class ElementSchema(Schema):
     intermediate_frequency = fields.Float(
         metadata={"description": "The frequency at which the controller modulates the output to this element [Hz]."},
@@ -1004,20 +991,19 @@
         self,
         data,
         capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities],
         **kwargs,
     ):
         el = qua_config.QuaConfigElementDec()
         if "intermediate_frequency" in data and data["intermediate_frequency"] is not None:
+            el.intermediate_frequency = abs(int(data["intermediate_frequency"]))
+            el.intermediate_frequency_oscillator = int(data["intermediate_frequency"])
             if capabilities.supports_double_frequency:
-                el.intermediate_frequency_double = abs(data["intermediate_frequency"])
-                el.intermediate_frequency_oscillator_double = data["intermediate_frequency"]
-            else:
-                el.intermediate_frequency = abs(int(data["intermediate_frequency"]))
-                el.intermediate_frequency_oscillator = int(data["intermediate_frequency"])
+                el.intermediate_frequency_double = float(abs(data["intermediate_frequency"]))
+                el.intermediate_frequency_oscillator_double = float(data["intermediate_frequency"])
 
             el.intermediate_frequency_negative = data["intermediate_frequency"] < 0
         elif "oscillator" in data and data["oscillator"] is not None:
             el.named_oscillator = data["oscillator"]
         else:
             el.no_oscillator = Empty()
```

### Comparing `qm_qua-1.1.1/qm/program/_qua_config_to_pb.py` & `qm_qua-1.1.2/qm/program/_qua_config_to_pb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import Dict, Any, Optional, List, Union
+from typing import Any, Dict, List, Union, Optional
+
 import numpy as np
 from betterproto.lib.google.protobuf import Empty
-from dependency_injector.wiring import inject, Provide
+from dependency_injector.wiring import Provide, inject
 
+from qm.grpc import qua_config, octave_models
+from qm.exceptions import ConfigValidationException
 from qm.api.models.capabilities import ServerCapabilities
 from qm.containers.capabilities_container import CapabilitiesContainer
-from qm.exceptions import ConfigValidationException
-from qm.grpc import qua_config, octave_models
 from qm.program._validate_config_schema import (
-    validate_output_smearing,
     validate_oscillator,
     validate_output_tof,
-    validate_arbitrary_waveform,
     validate_used_inputs,
+    validate_output_smearing,
+    validate_arbitrary_waveform,
     validate_timetagging_parameters,
 )
 
 
 class OctaveConnectionAmbiguity(Exception):
     def __str__(self):
         return (
@@ -49,15 +50,15 @@
         )
     elif connection_type == "digital_output":
         return_class, port_class = (
             octave_models.OctaveDigitalOutputPort,
             octave_models.OctaveDigitalOutputPortName,
         )
     else:
-        raise Exception("Unknown connection type")
+        raise ConfigValidationException("Unknown connection type")
 
     if device_name is not None:
         if isinstance(port_data, dict) and port_data.get("connectivity") is not None:
             raise OctaveConnectionAmbiguity
         port = port_class(port_num - 1)
         # The enum is 0-based and the port enumeration is 1-based, so we need to align them.
         return return_class(device_name=device_name, port_name=port)
@@ -211,39 +212,36 @@
 
 @inject
 def mixer_ref_to_pb(
     name: str,
     lo_frequency: int,
     capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities],
 ) -> qua_config.QuaConfigMixerRef:
+    item = qua_config.QuaConfigMixerRef(mixer=name, lo_frequency=int(lo_frequency))
     if capabilities.supports_double_frequency:
-        frequency = {"lo_frequency": int(lo_frequency)}
-    else:
-        frequency = {"lo_frequency_double": float(lo_frequency)}
-
-    return qua_config.QuaConfigMixerRef(mixer=name, **frequency)
+        item.lo_frequency_double = float(lo_frequency)
+    return item
 
 
 @inject
 def oscillator_to_pb(
     data, capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities]
 ) -> qua_config.QuaConfigOscillator:
     oscillator = qua_config.QuaConfigOscillator()
     if "intermediate_frequency" in data:
+        oscillator.intermediate_frequency = int(data["intermediate_frequency"])
         if capabilities.supports_double_frequency:
             oscillator.intermediate_frequency_double = float(data["intermediate_frequency"])
-        else:
-            oscillator.intermediate_frequency = int(data["intermediate_frequency"])
 
     if "mixer" in data:
         oscillator.mixer = qua_config.QuaConfigMixerRef(mixer=data["mixer"])
+        oscillator.mixer.lo_frequency = int(data.get("lo_frequency", 0))
         if capabilities.supports_double_frequency:
             oscillator.mixer.lo_frequency_double = float(data.get("lo_frequency", 0.0))
-        else:
-            oscillator.mixer.lo_frequency = int(data.get("lo_frequency", 0))
+
     return oscillator
 
 
 @inject
 def create_correction_entry(
     mixer_data,
     capabilities: ServerCapabilities = Provide[CapabilitiesContainer.capabilities],
@@ -253,20 +251,20 @@
         correction=qua_config.QuaConfigMatrix(
             v00=mixer_data["correction"][0],
             v01=mixer_data["correction"][1],
             v10=mixer_data["correction"][2],
             v11=mixer_data["correction"][3],
         ),
     )
+    correction.frequency = abs(int(mixer_data["intermediate_frequency"]))
+    correction.lo_frequency = int(mixer_data["lo_frequency"])
     if capabilities.supports_double_frequency:
         correction.frequency_double = abs(float(mixer_data["intermediate_frequency"]))
         correction.lo_frequency_double = float(mixer_data["lo_frequency"])
-    else:
-        correction.frequency = abs(int(mixer_data["intermediate_frequency"]))
-        correction.lo_frequency = int(mixer_data["lo_frequency"])
+
     return correction
 
 
 def mixer_to_pb(data) -> qua_config.QuaConfigMixerDec:
     return qua_config.QuaConfigMixerDec(correction=[create_correction_entry(mixer) for mixer in data])
 
 
@@ -347,20 +345,19 @@
     if "time_of_flight" in data:
         element.time_of_flight = int(data["time_of_flight"])
 
     if "smearing" in data:
         element.smearing = int(data["smearing"])
 
     if "intermediate_frequency" in data:
+        element.intermediate_frequency = abs(int(data["intermediate_frequency"]))
+        element.intermediate_frequency_oscillator = int(data["intermediate_frequency"])
         if capabilities.supports_double_frequency:
             element.intermediate_frequency_double = abs(float(data["intermediate_frequency"]))
             element.intermediate_frequency_oscillator_double = float(data["intermediate_frequency"])
-        else:
-            element.intermediate_frequency = abs(int(data["intermediate_frequency"]))
-            element.intermediate_frequency_oscillator = int(data["intermediate_frequency"])
 
         element.intermediate_frequency_negative = data["intermediate_frequency"] < 0
 
     if "thread" in data:
         element.thread = element_thread_to_pb(data["thread"])
 
     if "outputs" in data:
@@ -390,18 +387,17 @@
         element.mix_inputs = qua_config.QuaConfigMixInputs(
             i=dac_port_ref_to_pb(cont_I, port_id_I),
             q=dac_port_ref_to_pb(cont_Q, port_id_Q),
             mixer=mix_inputs.get("mixer", ""),
         )
 
         lo_frequency = mix_inputs.get("lo_frequency", 0)
+        element.mix_inputs.lo_frequency = int(lo_frequency)
         if capabilities.supports_double_frequency:
             element.mix_inputs.lo_frequency_double = float(lo_frequency)
-        else:
-            element.mix_inputs.lo_frequency = int(lo_frequency)
 
         if "octave_params" in mix_inputs:
             element.mix_inputs.octave_params = octave_params_to_pb(mix_inputs["octave_params"])
 
     if "singleInputCollection" in data:
         element.single_input_collection = qua_config.QuaConfigSingleInputCollection(
             inputs={k: dac_port_ref_to_pb(v[0], v[1]) for k, v in data["singleInputCollection"]["inputs"].items()}
```

### Comparing `qm_qua-1.1.1/qm/program/_validate_config_schema.py` & `qm_qua-1.1.2/qm/program/_validate_config_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from marshmallow import ValidationError
+
 from qm.exceptions import ConfigValidationException
 
 
 def validate_timetagging_parameters(data):
     if "outputPulseParameters" in data:
         pulseParameters = data["outputPulseParameters"]
         neededParameters = [
```

### Comparing `qm_qua-1.1.1/qm/program/expressions.py` & `qm_qua-1.1.2/qm/program/expressions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union, Optional
 
-from qm.exceptions import QmQuaException
 import qm.grpc.qua as _qua
 from qm._loc import _get_loc
+from qm.exceptions import QmQuaException
 
 _ScalarExpressionType = _qua.QuaProgramAnyScalarExpression
 _VariableRefType = _qua.QuaProgramVarRefExpression
 
 
 def var(name: str) -> _VariableRefType:
     """A reference to a variable
```

### Comparing `qm_qua-1.1.1/qm/program/program.py` & `qm_qua-1.1.2/qm/program/program.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import dataclasses
-from typing import Optional, List
+from typing import List, Optional
 
+from qm.grpc.qua_config import QuaConfig
+from qm.program._ResultAnalysis import _ResultAnalysis
+from qm.program.StatementsCollection import StatementsCollection
 from qm.grpc.qua import (
     QuaProgram,
     QuaProgramType,
-    QuaProgramLiteralExpression,
-    QuaProgramVarDeclaration,
     QuaProgramScript,
     QuaResultAnalysis,
+    QuaProgramVarDeclaration,
+    QuaProgramLiteralExpression,
     QuaProgramStatementsCollection,
 )
-from qm.grpc.qua_config import QuaConfig
-from qm.program.StatementsCollection import StatementsCollection
-from qm.program._ResultAnalysis import _ResultAnalysis
 
 
 @dataclasses.dataclass
 class ProgramMetadata:
     uses_command_timestamps: bool
     uses_fast_frame_rotation: bool
```

### Comparing `qm_qua-1.1.1/qm/qua/AnalogMeasureProcess.py` & `qm_qua-1.1.2/qm/qua/AnalogMeasureProcess.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/qua/DigitalMeasureProcess.py` & `qm_qua-1.1.2/qm/qua/DigitalMeasureProcess.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/qua/_dsl.py` & `qm_qua-1.1.2/qm/qua/_dsl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,62 +1,55 @@
-import dataclasses
 import logging
+import dataclasses
 import math as _math
-from collections.abc import Iterable
+from enum import Enum
+from enum import Enum as _Enum
 from dataclasses import dataclass
-from enum import Enum as _Enum, Enum
-from typing import Optional, Union, List, Tuple, Type, Set, Dict
+from collections.abc import Iterable
+from typing import Set, Dict, List, Type, Tuple, Union, Optional
 
 import betterproto
 import numpy as np
 from deprecation import deprecated
 
-import qm.grpc.qua as _qua
-import qm.program.expressions as _expressions
 from qm import Program
-from qm.serialization.expression_serializing_visitor import ExpressionSerializingVisitor
+import qm.grpc.qua as _qua
 from qm._loc import _get_loc
 from qm.exceptions import QmQuaException
-from qm.program.StatementsCollection import (
-    StatementsCollection as _StatementsCollection,
-)
-from qm.program._ResultAnalysis import _ResultAnalysis, _RESULT_SYMBOL
-from qm.qua import AnalogMeasureProcess
-from qm.qua import DigitalMeasureProcess
+from qm.utils import is_iter as _is_iter
+import qm.program.expressions as _expressions
+from qm.qua import AnalogMeasureProcess, DigitalMeasureProcess
+from qm.program._ResultAnalysis import _RESULT_SYMBOL, _ResultAnalysis
+from qm.serialization.expression_serializing_visitor import ExpressionSerializingVisitor
+from qm.program.StatementsCollection import StatementsCollection as _StatementsCollection
+from qm.utils import collection_has_type_int, collection_has_type_bool, collection_has_type_float
 from qm.qua._type_hinting import (
-    PlayPulseType,
-    QuaNumberType,
-    QuaExpressionType,
     ChirpType,
-    MeasurePulseType,
-    StreamType,
-    MeasureProcessType,
     OneOrMore,
-    QuaVariableType,
-    AllQuaTypes,
-    TypeOrExpression,
     AllPyTypes,
-    ForEachValuesType,
+    StreamType,
+    AllQuaTypes,
+    PyFloatType,
     PyNumberType,
-    MessageExpressionType,
-    VariableDeclarationType,
-    MessageVariableOrExpression,
     AmpValuesType,
+    PlayPulseType,
+    QuaNumberType,
     MessageVarType,
-    AnalogProcessTargetType,
+    QuaVariableType,
+    MeasurePulseType,
     TimeDivisionType,
+    TypeOrExpression,
+    ForEachValuesType,
     PyNumberArrayType,
-    PyFloatType,
-)
-from qm.utils import (
-    fix_object_data_type as _fix_object_data_type,
-    collection_has_type_bool,
-    collection_has_type_int,
-    collection_has_type_float,
-    is_iter as _is_iter,
+    QuaExpressionType,
+    MeasureProcessType,
+    MessageExpressionType,
+    AnalogProcessTargetType,
+    VariableDeclarationType,
+    MessageVariableOrExpression,
 )
 
 _TIMESTAMPS_LEGACY_SUFFIX = "_timestamps"
 
 _block_stack: List["_BaseScope"] = []
 
 logger = logging.getLogger(__name__)
@@ -434,15 +427,15 @@
 
             # measure by playing 'meas_pulse' to element 'resonator', save raw results to `adc_st`
             # demodulate data from 'out1' port of 'resonator' using 'optimized_weights' and store result in I
             measure('meas_pulse', 'resonator', adc_st, demod.full("optimized_weights", I, "out1"))
             with stream_processing():
                 adc_st.input1().save_all("raw_adc_stream")
 
-        from qm.QuantumMachinesManager import QuantumMachinesManager
+        from qm import QuantumMachinesManager
         qm = QuantumMachinesManager().open_qm(config)
         job = qm.execute(prog)
         # ... we wait for the results to be ready...
         job.result_handles.wait_for_all_values()
         # raw results can be retrieved as follows (here job is a QmJob object:
         raw_I_handle = job.result_handles.get("raw_adc_stream")
         ```
@@ -1485,14 +1478,25 @@
             is_adc_trace=is_adc_trace,
             input=-1,
             auto_reshape=False,
         )
     )
 
 
+def _fix_object_data_type(obj):
+    if isinstance(obj, (np.floating, np.integer, np.bool_)):
+        obj_item = obj.item()
+        if isinstance(obj_item, np.longdouble):
+            return float(obj_item)
+        else:
+            return obj_item
+    else:
+        return obj
+
+
 def _to_expression(other: AllQuaTypes, index_exp: Optional[QuaNumberType] = None) -> MessageVariableOrExpression:
     other = _fix_object_data_type(other)
     if index_exp is not None and type(index_exp) is not _qua.QuaProgramAnyScalarExpression:
         index_exp = _to_expression(index_exp, None)
 
     if index_exp is not None and type(other) is not _qua.QuaProgramArrayVarRefExpression:
         raise QmQuaException(f"{other} is not an array")
```

### Comparing `qm_qua-1.1.1/qm/qua/_type_hinting.py` & `qm_qua-1.1.2/qm/qua/_type_hinting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from typing import Tuple, List, Union, TypeVar, TYPE_CHECKING, Type
-from qm.grpc import qua
+from typing import TYPE_CHECKING, List, Type, Tuple, Union, TypeVar
+
 import numpy as np
 import numpy.typing as npt
 
+from qm.grpc import qua
+
 if TYPE_CHECKING:
-    from _dsl import _Expression, _Variable, fixed, _ResultSource  # noqa
+    from _dsl import fixed, _Variable, _Expression, _ResultSource  # noqa
 
 MessageExpressionType = qua.QuaProgramAnyScalarExpression
 MessageArrayVarType = qua.QuaProgramArrayVarRefExpression
 MessageVarType = qua.QuaProgramVarRefExpression
 MessageVariableType = Union[MessageArrayVarType, MessageVarType]
 MessageVariableOrExpression = Union[MessageExpressionType, MessageVariableType]
```

### Comparing `qm_qua-1.1.1/qm/qua/lib.py` & `qm_qua-1.1.2/qm/qua/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
-import qm.program.expressions as _exp
-from qm.qua._dsl import _Expression, _to_expression, declare, assign
 from functools import wraps
-from qm.utils import get_iterable_elements_datatype as _get_iterable_elements_datatype
 from collections.abc import Iterable
 
+import qm.program.expressions as _exp
+from qm.qua._dsl import assign, declare, _Expression, _to_expression
+from qm.utils import get_iterable_elements_datatype as _get_iterable_elements_datatype
+
 
 def _library_function(lib_name, func_name):
     def library_decorator(function):
         @wraps(function)
         def wrapper(*args, **kwargs):
             new_args = function(*args, **kwargs)
             return call_library_function(lib_name, func_name, new_args)
```

### Comparing `qm_qua-1.1.1/qm/results/base_streaming_result_fetcher.py` & `qm_qua-1.1.2/qm/results/base_streaming_result_fetcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 import abc
 import json
 import logging
 import warnings
+from io import BytesIO
 from dataclasses import dataclass
-from io import BufferedWriter, BytesIO
-from typing import List, Optional, Union, Tuple, Dict
+from typing_extensions import Protocol
+from typing import Any, Dict, List, Tuple, Union, BinaryIO, Optional, cast
 
 import numpy
+import numpy.typing
 from numpy.lib import format as _format
 
-from qm.StreamMetadata import StreamMetadataError, StreamMetadata
-from qm.utils.general_utils import run_until_with_timeout
+from qm.persistence import BaseStore
+from qm.utils import deprecation_message
 from qm.utils.async_utils import run_async
+from qm.type_hinting.general import PathLike
+from qm.exceptions import InvalidStreamMetadataError
 from qm.api.job_result_api import JobResultServiceApi
 from qm.api.models.capabilities import ServerCapabilities
-from qm.exceptions import InvalidStreamMetadataError
-from qm.persistence import BaseStore
+from qm.utils.general_utils import run_until_with_timeout
+from qm.StreamMetadata import StreamMetadata, StreamMetadataError
 
 logger = logging.getLogger(__name__)
 
+DtypeType = List[List[str]]
+
 
-def _parse_dtype(simple_dtype: str) -> dict:
-    def hinted_tuple_hook(obj):
+class JobStreamingStateProtocol(Protocol):
+    done: bool
+    closed: bool
+    has_dataloss: bool
+
+
+def _parse_dtype(simple_dtype: str) -> DtypeType:
+    def hinted_tuple_hook(obj: Any) -> Any:
         if "__tuple__" in obj:
             return tuple(obj["items"])
         else:
             return obj
 
     dtype = json.loads(simple_dtype, object_hook=hinted_tuple_hook)
-    return dtype
+    return cast(DtypeType, dtype)
 
 
 @dataclass
 class JobResultItemSchema:
     name: str
-    dtype: dict
-    shape: Tuple[int]
+    dtype: DtypeType
+    shape: Tuple[int, ...]
     is_single: bool
     expected_count: int
 
 
 @dataclass
 class JobResultSchema:
     items: Dict[str, JobResultItemSchema]
@@ -47,16 +59,16 @@
 
 @dataclass
 class NamedJobResultHeader:
     count_so_far: int
     is_single: bool
     output_name: str
     job_id: str
-    d_type: dict
-    shape: Tuple[int]
+    d_type: DtypeType
+    shape: Tuple[int, ...]
     has_dataloss: bool
 
 
 @dataclass
 class JobStreamingState:
     job_id: str
     done: bool
@@ -68,30 +80,30 @@
     def __init__(
         self,
         job_id: str,
         schema: JobResultItemSchema,
         service: JobResultServiceApi,
         store: BaseStore,
         stream_metadata_errors: List[StreamMetadataError],
-        stream_metadata: StreamMetadata,
+        stream_metadata: Optional[StreamMetadata],
         capabilities: ServerCapabilities,
     ) -> None:
         self._job_id = job_id
         self._schema = schema
         self._service = service
         self._store = store
         self._stream_metadata_errors = stream_metadata_errors
         self._stream_metadata = stream_metadata
         self._count_data_written = 0
         self._capabilities = capabilities
 
         self._validate_schema()
 
     @abc.abstractmethod
-    def _validate_schema(self):
+    def _validate_schema(self) -> None:
         pass
 
     @property
     def name(self) -> str:
         """The name of result this handle is connected to"""
         return self._schema.name
 
@@ -101,72 +113,87 @@
         return self._job_id
 
     @property
     def expected_count(self) -> int:
         return self._schema.expected_count
 
     @property
-    def numpy_dtype(self):
+    def numpy_dtype(self) -> DtypeType:
         return self._schema.dtype
 
     @property
-    def stream_metadata(self) -> StreamMetadata:
+    def stream_metadata(self) -> Optional[StreamMetadata]:
         """Provides the StreamMetadata of this stream.
 
         Metadata currently includes the values and shapes of the automatically identified loops
         in the program.
 
         """
         if len(self._stream_metadata_errors) > 0:
             logger.error("Error creating stream metadata:")
-            for x in self._stream_metadata_errors:
-                logger.error(f"{x.error} in {x.location}")
+            for e in self._stream_metadata_errors:
+                logger.error(f"{e.error} at: {e.location}")
             raise InvalidStreamMetadataError(self._stream_metadata_errors)
         return self._stream_metadata
 
     def save_to_store(
         self,
-        writer: Optional[Union[BufferedWriter, BytesIO, str]] = None,
+        writer: Optional[Union[BinaryIO, str]] = None,
         flat_struct: bool = False,
     ) -> int:
         """Saving to persistent store the NPY data of this result handle
 
         Args:
             writer: An optional writer to override the store defined in
-                [QuantumMachinesManager][qm.QuantumMachinesManager.QuantumMachinesManager]
+                [QuantumMachinesManager][qm.quantum_machines_manager.QuantumMachinesManager]
             flat_struct: results will have a flat structure - dimensions
                 will be part of the shape and not of the type
 
         Returns:
             The number of items saved
         """
-        own_writer = False
-        if writer is None:
-            own_writer = True
-            writer = self._store.job_named_result(self._job_id, self._schema.name).for_writing()
+        warnings.warn(
+            deprecation_message(
+                method="StreamingResultFetcher.save_to_store",
+                deprecated_in="1.1.1",
+                removed_in="1.2.0",
+                details="function no longer supported, will be removed.",
+            ),
+            DeprecationWarning,
+        )
+        writer_opened = False
+        if writer is None or isinstance(writer, str):
+            writer_opened = True
+            writer = self._open_bytes_writer(writer)
         try:
             header = self._get_named_header(flat_struct=flat_struct)
             return self._save_to_file(header, writer)
         finally:
-            if own_writer:
+            if writer_opened:
                 writer.close()
 
-    def wait_for_values(self, count: int = 1, timeout: Optional[float] = None):
+    def _open_bytes_writer(self, path: Optional[PathLike]) -> BinaryIO:
+        if path is not None:
+            return open(path, "wb+")
+        else:
+            return self._store.job_named_result(self._job_id, self._schema.name).for_writing()
+
+    def wait_for_values(self, count: int = 1, timeout: float = float("infinity")) -> None:
         """Wait until we know at least `count` values were processed for this named result
 
         Args:
             count: The number of items to wait for
             timeout: Timeout for waiting in seconds
 
         Returns:
 
         """
         run_until_with_timeout(
             lambda: self.count_so_far() >= count,
-            timeout=timeout if timeout else float("infinity"),
+            timeout=timeout,
             timeout_message=f"result {self.name} was not done in time",
         )
 
     def wait_for_all_values(self, timeout: float = float("infinity")) -> bool:
         """Wait until we know all values were processed for this named result
 
         Args:
@@ -219,44 +246,38 @@
         if there was data loss during job execution
         """
         state = self.get_job_state()
         return state.has_dataloss
 
     def _write_header(
         self,
-        writer: Union[BufferedWriter, BytesIO, str],
-        shape: Tuple[int],
+        writer: BinaryIO,
+        shape: Tuple[int, ...],
         d_type: object,
-    ):
-        _format.write_array_header_2_0(writer, {"descr": d_type, "fortran_order": False, "shape": shape})
+    ) -> None:
+        _format.write_array_header_2_0(
+            writer, {"descr": d_type, "fortran_order": False, "shape": shape}
+        )  # type: ignore[no-untyped-call]
 
-    async def _add_results_to_writer(self, data_writer, start, stop):
+    async def _add_results_to_writer(self, data_writer: BinaryIO, start: int, stop: int) -> None:
         async for result in self._service.get_job_named_result(self._job_id, self._schema.name, start, stop - start):
             self._count_data_written += result.count_of_items
             data_writer.write(result.data)
 
-    def _save_to_file(self, header: NamedJobResultHeader, writer: Union[BufferedWriter, BytesIO, str]) -> int:
+    def _save_to_file(self, header: NamedJobResultHeader, writer: BinaryIO) -> int:
         self._count_data_written = 0
-        owning_writer = False
-
-        if type(writer) is str:
-            writer = open(writer, "wb+")
-            owning_writer = True
 
-        try:
-            final_shape = self._get_final_shape(header.count_so_far, header.shape)
-            self._write_header(writer, final_shape, header.d_type)
+        final_shape = self._get_final_shape(header.count_so_far, header.shape)
+        self._write_header(writer, final_shape, header.d_type)
 
-            run_async(self._add_results_to_writer(writer, 0, header.count_so_far))
-        finally:
-            if owning_writer:
-                writer.close()
+        run_async(self._add_results_to_writer(writer, 0, header.count_so_far))
         return self._count_data_written
 
     def get_job_state(self) -> JobStreamingState:
+        response: JobStreamingStateProtocol
         if self._capabilities.has_job_streaming_state:
             response = self._service.get_job_state(self._job_id)
         else:
             response = self._service.get_named_header(self._job_id, self.name, False)
         return JobStreamingState(
             job_id=self._job_id,
             done=response.done,
@@ -280,15 +301,17 @@
             output_name=self.name,
             job_id=self.job_id,
             d_type=dtype,
             shape=tuple(response.shape),
             has_dataloss=response.has_dataloss,
         )
 
-    def fetch_all(self, *, check_for_errors: bool = False, flat_struct: bool = False):
+    def fetch_all(
+        self, *, check_for_errors: bool = False, flat_struct: bool = False
+    ) -> Optional[numpy.typing.NDArray[numpy.generic]]:
         """Fetch a result from the current result stream saved in server memory.
         The result stream is populated by the save() and save_all() statements.
         Note that if save_all() statements are used, calling this function twice
         may give different results.
 
         Args:
             flat_struct: results will have a flat structure - dimensions
@@ -305,15 +328,24 @@
 
     def fetch(
         self,
         item: Union[int, slice],
         *,
         check_for_errors: bool = False,
         flat_struct: bool = False,
-    ) -> numpy.array:
+    ) -> Optional[numpy.typing.NDArray[numpy.generic]]:
+        return self.strict_fetch(item, check_for_errors=check_for_errors, flat_struct=flat_struct)
+
+    def strict_fetch(
+        self,
+        item: Union[int, slice],
+        *,
+        check_for_errors: bool = False,
+        flat_struct: bool = False,
+    ) -> numpy.typing.NDArray[numpy.generic]:
         """Fetch a result from the current result stream saved in server memory.
         The result stream is populated by the save() and save_all() statements.
         Note that if save_all() statements are used, calling this function twice
         with the same item index may give different results.
 
         Args:
             item: The index of the result in the saved results stream.
@@ -353,17 +385,17 @@
             start = 0
 
         writer = self._fetch_all_job_results(header, start, stop)
 
         if header.has_dataloss:
             logger.warning(f"Possible data loss detected in data for job: {self._job_id}")
 
-        return numpy.load(writer)
+        return cast(numpy.typing.NDArray[numpy.generic], numpy.load(writer))
 
-    def _fetch_all_job_results(self, header, start, stop):
+    def _fetch_all_job_results(self, header: NamedJobResultHeader, start: int, stop: int) -> BinaryIO:
         self._count_data_written = 0
         writer = BytesIO()
         data_writer = BytesIO()
 
         run_async(self._add_results_to_writer(data_writer, start, stop))
 
         final_shape = self._get_final_shape(self._count_data_written, header.shape)
@@ -374,15 +406,15 @@
         for d in data_writer:
             writer.write(d)
 
         writer.seek(0)
         return writer
 
     @staticmethod
-    def _get_final_shape(count, shape):
+    def _get_final_shape(count: int, shape: Tuple[int, ...]) -> Tuple[int, ...]:
         if count == 1:
             final_shape = shape
         else:
             if len(shape) == 1 and shape[0] == 1:
                 final_shape = (count,)
             else:
                 final_shape = (count,) + shape
```

### Comparing `qm_qua-1.1.1/qm/results/multiple_streaming_result_fetcher.py` & `qm_qua-1.1.2/qm/results/multiple_streaming_result_fetcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,60 @@
-from io import BufferedWriter, BytesIO
-from typing import List, Union, Optional
+from typing import TYPE_CHECKING, List, Union, BinaryIO, Optional, cast
 
 import numpy
 
-from qm.StreamMetadata import StreamMetadataError, StreamMetadata
+from qm.persistence import BaseStore
 from qm.api.job_result_api import JobResultServiceApi
 from qm.api.models.capabilities import ServerCapabilities
-from qm.exceptions import QmInvalidSchemaError
-from qm.persistence import BaseStore
-from qm.results.base_streaming_result_fetcher import (
-    BaseStreamingResultFetcher,
-    JobResultItemSchema,
-)
+from qm.exceptions import QmNoResultsError, QmInvalidSchemaError
+from qm.StreamMetadata import StreamMetadata, StreamMetadataError
+from qm.results.base_streaming_result_fetcher import JobResultItemSchema, BaseStreamingResultFetcher
 
 TIMESTAMPS_LEGACY_EXT = "_timestamps"
 
+if TYPE_CHECKING:
+    from qm import StreamingResultFetcher
+
 
 class MultipleStreamingResultFetcher(BaseStreamingResultFetcher):
     """A handle to a result of a pipeline terminating with ``save_all``"""
 
     def __init__(
         self,
-        job_results,
+        job_results: "StreamingResultFetcher",
         job_id: str,
         schema: JobResultItemSchema,
         service: JobResultServiceApi,
         store: BaseStore,
         stream_metadata_errors: List[StreamMetadataError],
-        stream_metadata: StreamMetadata,
+        stream_metadata: Optional[StreamMetadata],
         capabilities: ServerCapabilities,
     ) -> None:
         self.job_results = job_results
         super().__init__(
             job_id=job_id,
             schema=schema,
             service=service,
             store=store,
             stream_metadata_errors=stream_metadata_errors,
             stream_metadata=stream_metadata,
             capabilities=capabilities,
         )
 
-    def _validate_schema(self):
+    def _validate_schema(self) -> None:
         if self._schema.is_single:
             raise QmInvalidSchemaError("expecting a multi-result schema")
 
     def fetch(
         self,
         item: Union[int, slice],
         *,
         check_for_errors: bool = False,
         flat_struct: bool = False,
-    ) -> numpy.array:
+    ) -> Optional[numpy.typing.NDArray[numpy.generic]]:
         """Fetch a result from the current result stream saved in server memory.
         The result stream is populated by the save() and save_all() statements.
         Note that if save_all() statements are used, calling this function twice
         with the same item index may give different results.
 
         Args:
             item: The index of the result in the saved results stream.
@@ -70,52 +69,55 @@
             res.fetch(0)         # return the item in the top position
             res.fetch(1)         # return the item in position number 2
             res.fetch(slice(1,6))# return items from position 1 to position 6 (exclusive)
                                  # same as res.fetch_all()[1:6]
             ```
         """
         if flat_struct:
-            return super().fetch(item, check_for_errors=check_for_errors, flat_struct=flat_struct)
+            return self.strict_fetch(item, check_for_errors=check_for_errors, flat_struct=flat_struct)
         else:
             # legacy support - reconstruct the old structure
             name = self._schema.name
             timestamps_name = name + TIMESTAMPS_LEGACY_EXT
             timestamps_result_handle = self.job_results.get(timestamps_name)
             if timestamps_result_handle is None:
-                return super().fetch(item, check_for_errors=check_for_errors)
+                return self.strict_fetch(item, check_for_errors=check_for_errors)
             else:
-                values_result = super().fetch(item, check_for_errors=check_for_errors, flat_struct=True)
+                values_result = self.strict_fetch(item, check_for_errors=check_for_errors, flat_struct=True)
 
                 fetched_length = len(values_result)
                 if isinstance(item, slice):
                     item = slice(item.start, item.start + fetched_length, item.step)
                 else:
                     item = slice(0, fetched_length)
 
                 timestamps_result = timestamps_result_handle.fetch(
                     item, flat_struct=True, check_for_errors=check_for_errors
                 )
 
+                if timestamps_result is None:
+                    raise QmNoResultsError("Failed to fetch timestamp results, please wait until results are ready")
+
                 dtype = [
                     ("value", values_result.dtype),
                     ("timestamp", timestamps_result.dtype),
                 ]  # timestamps_result.dtype.descr
                 combined = numpy.rec.fromarrays([values_result, timestamps_result], dtype=dtype)
-                return combined.view(numpy.ndarray).astype(dtype)
+                return cast(numpy.typing.NDArray[numpy.generic], combined.view(numpy.ndarray).astype(dtype))
 
     def save_to_store(
         self,
-        writer: Optional[Union[BufferedWriter, BytesIO, str]] = None,
+        writer: Optional[Union[BinaryIO, str]] = None,
         flat_struct: bool = False,
     ) -> int:
         """Saving to persistent store the NPY data of this result handle
 
         Args:
             writer: An optional writer to override the store defined in
-                [QuantumMachinesManager][qm.QuantumMachinesManager.QuantumMachinesManager]
+                [QuantumMachinesManager][qm.quantum_machines_manager.QuantumMachinesManager]
 
         Returns:
             The number of items saved
         """
         if flat_struct:
             return super().save_to_store(writer, flat_struct)
         else:
@@ -123,28 +125,23 @@
             name = self._schema.name
             timestamps_name = name + TIMESTAMPS_LEGACY_EXT
             timestamps_result_handle = self.job_results.get(timestamps_name)
             if timestamps_result_handle is None:
                 return super().save_to_store(writer, flat_struct)
             else:
                 final_result = self.fetch_all(flat_struct=flat_struct)
-                own_writer = False
-                if writer is None:
-                    own_writer = True
-                    writer = self._store.job_named_result(self._job_id, self._schema.name).for_writing()
+                if final_result is None:
+                    raise QmNoResultsError("Failed to fetch results, please wait until results are ready")
+
+                writer_opened = False
+                if writer is None or isinstance(writer, str):
+                    writer_opened = True
+                    writer = self._open_bytes_writer(writer)
+
                 try:
-                    owning_writer = False
-                    if type(writer) is str:
-                        writer = open(writer, "wb+")
-                        owning_writer = True
-
-                    try:
-                        self._write_header(writer, (len(final_result),), final_result.dtype.descr)
-                        writer.write(final_result.tobytes())
-
-                    finally:
-                        if owning_writer:
-                            writer.close()
-                    return len(final_result)
+                    self._write_header(writer, (len(final_result),), final_result.dtype.descr)
+                    writer.write(final_result.tobytes())
+
                 finally:
-                    if own_writer:
+                    if writer_opened:
                         writer.close()
+                return len(final_result)
```

### Comparing `qm_qua-1.1.1/qm/results/simulator_samples.py` & `qm_qua-1.1.2/qm/results/simulator_samples.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,73 @@
-import numpy as np
+from typing_extensions import Literal, TypedDict
+from typing import Dict, List, Union, Mapping, Optional, Sequence, cast
 
-
-class SimulatorSamples:
-    def __init__(self, controllers):
-        for k, v in controllers.items():
-            self.__setattr__(k, v)
-
-    @staticmethod
-    def from_np_array(arr: np.ndarray) -> "SimulatorSamples":
-        controllers = dict()
-        for col in arr.dtype.names:
-            parts = col.split(":")
-            controller = controllers.setdefault(parts[0], {"analog": dict(), "digital": dict()})
-            controller[parts[1]][parts[2]] = arr[col]
-        res = dict()
-        for item in controllers.items():
-            res[item[0]] = SimulatorControllerSamples(item[1]["analog"], item[1]["digital"])
-        return SimulatorSamples(res)
+import numpy.typing
 
 
-class SimulatorControllerSamples(object):
-    def __init__(self, analog, digital):
+class SimulatorControllerSamples:
+    def __init__(self, analog: Mapping[str, Sequence[float]], digital: Mapping[str, Sequence[bool]]):
         self.analog = self._add_keys_for_first_con(analog)
         self.digital = self._add_keys_for_first_con(digital)
         self._analog_conns = analog
         self._digital_conns = digital
 
     @staticmethod
-    def _add_keys_for_first_con(data):
-        first_con_data = {k[2:]: v for (k, v) in data.items() if k.startswith("1-")}
+    def _add_keys_for_first_con(
+        data: Mapping[str, Union[Sequence[float], Sequence[bool]]]
+    ) -> Mapping[str, Union[Sequence[float], Sequence[bool]]]:
+        # Note(jonatann): I have no idea what this function does and why it exists...
+        first_con_data = {
+            controller_name[2:]: samples
+            for controller_name, samples in data.items()
+            if controller_name.startswith("1-")
+        }
         return {**data, **first_con_data}
 
-    def plot(self, analog_ports=None, digital_ports=None):
+    def plot(
+        self,
+        analog_ports: Optional[Union[str, List[str]]] = None,
+        digital_ports: Optional[Union[str, List[str]]] = None,
+    ) -> None:
         """Plots the simulated output of the OPX in the given ports.
         If no ports are given, all active ports are plotted.
 
         Args:
             analog_ports: Union[None, str, list[str]]
             digital_ports: Union[None, str, list[str]]
         """
-        import matplotlib.pyplot as plt
+        import matplotlib.pyplot as plt  # type: ignore[import]
 
         for port, samples in self._analog_conns.items():
             if analog_ports is None or port in analog_ports:
                 plt.plot(samples, label=f"Analog {port}")
         for port, samples in self._digital_conns.items():
             if digital_ports is None or port in digital_ports:
                 plt.plot(samples, label=f"Digital {port}")
         plt.xlabel("Time [ns]")
         plt.ylabel("Output")
         plt.legend()
+
+
+class SimulatorSamplesDictType(TypedDict):
+    analog: Dict[str, Sequence[float]]
+    digital: Dict[str, Sequence[bool]]
+
+
+class SimulatorSamples:
+    def __init__(self, controllers: Dict[str, SimulatorControllerSamples]):
+        for k, v in controllers.items():
+            self.__setattr__(k, v)
+
+    @staticmethod
+    def from_np_array(arr: numpy.typing.NDArray[numpy.generic]) -> "SimulatorSamples":
+        controllers: Dict[str, SimulatorSamplesDictType] = {}
+        assert arr.dtype.names is not None
+        for col in arr.dtype.names:
+            controller_name, output, number = col.split(":")
+            output = cast(Union[Literal["analog"], Literal["digital"]], output)
+            controller = controllers.setdefault(controller_name, {"analog": {}, "digital": {}})
+            controller[output][number] = arr[col]  # type: ignore[call-overload]
+        res = {}
+        for controller_name, samples in controllers.items():
+            res[controller_name] = SimulatorControllerSamples(samples["analog"], samples["digital"])
+        return SimulatorSamples(res)
```

### Comparing `qm_qua-1.1.1/qm/results/single_streaming_result_fetcher.py` & `qm_qua-1.1.2/qm/results/single_streaming_result_fetcher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import logging
-from typing import Optional, Union
+from typing import Union, Optional, cast
+
+import numpy.typing
 
 from qm.exceptions import QmInvalidSchemaError
 from qm.results.base_streaming_result_fetcher import BaseStreamingResultFetcher
 
 logger = logging.getLogger(__name__)
 
 
 class SingleStreamingResultFetcher(BaseStreamingResultFetcher):
     """A handle to a result of a pipeline terminating with ``save``"""
 
-    def _validate_schema(self):
+    def _validate_schema(self) -> None:
         if not self._schema.is_single:
             raise QmInvalidSchemaError("expecting a single-result schema")
 
-    def wait_for_values(self, count: int = 1, timeout: Optional[float] = None):
+    def wait_for_values(self, count: int = 1, timeout: float = float("inf")) -> None:
         if count != 1:
             raise RuntimeError("single result can wait only for a single value")
-        return super().wait_for_values(1, timeout)
+        super().wait_for_values(1, timeout)
 
-    def fetch_all(self, *, check_for_errors: bool = False, flat_struct: bool = False):
+    def fetch_all(
+        self, *, check_for_errors: bool = False, flat_struct: bool = False
+    ) -> Optional[numpy.typing.NDArray[numpy.generic]]:
         """Fetch a result from the current result stream saved in server memory.
         The result stream is populated by the save() and save_all() statements.
         Note that if save_all() statements are used, calling this function twice
         may give different results.
 
         Args:
             flat_struct: results will have a flat structure - dimensions
@@ -36,15 +40,15 @@
 
     def fetch(
         self,
         item: Union[int, slice],
         *,
         check_for_errors: bool = False,
         flat_struct: bool = False,
-    ):
+    ) -> Optional[numpy.typing.NDArray[numpy.generic]]:
 
         """Fetch a single result from the current result stream saved in server memory.
         The result stream is populated by the save().
 
         Args:
             item: ignored
             flat_struct: results will have a flat structure - dimensions
@@ -56,22 +60,24 @@
         Example:
             ```python
             res.fetch() # return the item in the top position
             ```
         """
         if (isinstance(item, int) and item != 0) or isinstance(item, slice):
             logger.warning("Fetching single result will always return the single value")
-        value = super().fetch(0, check_for_errors=check_for_errors, flat_struct=flat_struct)
+        value = self.strict_fetch(0, check_for_errors=check_for_errors, flat_struct=flat_struct)
         if flat_struct:
             if len(value) == 0:
+                logger.warning("Nothing to fetch: no results were found. Please wait until the results are ready.")
                 return None
             elif len(value) == 1:
-                return value[0]
+                return cast(numpy.typing.NDArray[numpy.generic], value[0])
             else:
                 return value
         else:
             if len(value) == 0:
+                logger.warning("Nothing to fetch: no results were found. Please wait until the results are ready.")
                 return None
             elif len(value[0]) == 1:
-                return value[0][0]
+                return cast(numpy.typing.NDArray[numpy.generic], value[0][0])
             else:
-                return value[0]
+                return cast(numpy.typing.NDArray[numpy.generic], value[0])
```

### Comparing `qm_qua-1.1.1/qm/results/streaming_result_fetcher.py` & `qm_qua-1.1.2/qm/results/streaming_result_fetcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import logging
 import zipfile
-from io import BufferedWriter, BytesIO
-from typing import Optional, Union, Dict, Tuple, Generator, List
+from typing import Dict, List, Tuple, Union, BinaryIO, Optional, Generator, cast
 
-from qm.StreamMetadata import (
-    StreamMetadata,
-    StreamMetadataError,
-)
+from qm.persistence import BaseStore
 from qm.utils.async_utils import run_async
-from qm.utils.general_utils import run_until_with_timeout
 from qm.api.job_result_api import JobResultServiceApi
 from qm.api.models.capabilities import ServerCapabilities
-from qm.persistence import BaseStore
+from qm.utils.general_utils import run_until_with_timeout
+from qm.StreamMetadata import StreamMetadata, StreamMetadataError
+from qm.results.single_streaming_result_fetcher import SingleStreamingResultFetcher
+from qm.results.multiple_streaming_result_fetcher import MultipleStreamingResultFetcher
 from qm.results.base_streaming_result_fetcher import (
+    JobResultSchema,
+    JobResultItemSchema,
     BaseStreamingResultFetcher,
     _parse_dtype,
-    JobResultItemSchema,
-    JobResultSchema,
 )
-from qm.results.multiple_streaming_result_fetcher import MultipleStreamingResultFetcher
-from qm.results.single_streaming_result_fetcher import SingleStreamingResultFetcher
 
 logger = logging.getLogger(__name__)
 
 
 class StreamingResultFetcher:
     """Access to the results of a QmJob
 
@@ -55,25 +51,26 @@
         service: JobResultServiceApi,
         store: BaseStore,
         capabilities: ServerCapabilities,
     ) -> None:
         self._job_id = job_id
         self._service = service
         self._store = store
-        self._schema = None
+        self._schema: JobResultSchema = JobResultSchema({})
         self._capabilities = capabilities
 
         self._all_results: Dict[str, BaseStreamingResultFetcher] = {}
         self._add_job_results()
 
-    def _add_job_results(self):
+    def _add_job_results(self) -> None:
         self._schema = StreamingResultFetcher._load_schema(self._job_id, self._service)
         stream_metadata_errors, stream_metadata_dict = self._get_stream_metadata()
         for (name, item_schema) in self._schema.items.items():
             stream_metadata = stream_metadata_dict.get(name)
+            result: BaseStreamingResultFetcher
             if item_schema.is_single:
                 result = SingleStreamingResultFetcher(
                     job_id=self._job_id,
                     schema=item_schema,
                     service=self._service,
                     store=self._store,
                     stream_metadata_errors=stream_metadata_errors,
@@ -89,67 +86,68 @@
                     store=self._store,
                     stream_metadata_errors=stream_metadata_errors,
                     stream_metadata=stream_metadata,
                     capabilities=self._capabilities,
                 )
             self._all_results[name] = result
 
-    def __getitem__(self, item: str):
+    def __getitem__(self, item: str) -> Optional[BaseStreamingResultFetcher]:
         return self.get(item)
 
-    def __getattr__(self, item: str):
+    def __getattr__(self, item: str) -> Optional[BaseStreamingResultFetcher]:
         if item == "shape" or item == "__len__":
-            return  # this is here because of a bug in pycharm debugger: ver: 2022.3.2 build #PY-223.8617.48 (24/1/23)
+            return (
+                None  # this is here because of a bug in pycharm debugger: ver: 2022.3.2 build #PY-223.8617.48 (24/1/23)
+            )
         return self.get(item)
 
-    def _get_stream_metadata(
-        self,
-    ) -> Optional[Tuple[List[StreamMetadataError], Dict[str, StreamMetadata]]]:
+    def _get_stream_metadata(self) -> Tuple[List[StreamMetadataError], Dict[str, StreamMetadata]]:
         return self._service.get_program_metadata(job_id=self._job_id)
 
-    def __iter__(self) -> Generator[Tuple[str, BaseStreamingResultFetcher], None, None]:
+    def __iter__(self) -> Generator[Tuple[str, Optional[BaseStreamingResultFetcher]], None, None]:
         for item in self._schema.items.values():
             yield item.name, self.get(item.name)
 
     def is_processing(self) -> bool:
         """Check if the job is still processing results
 
         Returns:
             True if results are still being processed, False otherwise
         """
         key = list(self._all_results.keys())[0]
         return self._all_results[key].is_processing()
 
     def save_to_store(
         self,
-        writer: Optional[Union[BufferedWriter, BytesIO, str]] = None,
+        writer: Optional[BinaryIO] = None,
         flat_struct: bool = False,
-    ):
+    ) -> None:
         """Save all results to store (file system by default) in a single NPZ file
 
         Args:
             writer: An optional writer to be used instead of the pre-
-                populated store passed to [qm.QuantumMachinesManager.QuantumMachinesManager][]
+                populated store passed to [qm.quantum_machines_manager.QuantumMachinesManager][]
             flat_struct: results will have a flat structure - dimensions
                 will be part of the shape and not of the type
 
         """
         own_writer = False
         if writer is None:
             own_writer = True
             writer = self._store.all_job_results(self._job_id).for_writing()
         zipf = None
         try:
             zipf = zipfile.ZipFile(writer, allowZip64=True, mode="w", compression=zipfile.ZIP_DEFLATED)
             for (name, result) in self:
-                with zipf.open(f"{name}.npy", "w") as entry:
-                    result.save_to_store(entry, flat_struct)
-                pass
+                if result is not None:
+                    with zipf.open(f"{name}.npy", "w") as entry:
+                        result.save_to_store(cast(BinaryIO, entry), flat_struct)
         finally:
-            zipf.close()
+            if zipf is not None:
+                zipf.close()
             if own_writer:
                 writer.close()
 
     @staticmethod
     def _load_schema(job_id: str, service: JobResultServiceApi) -> JobResultSchema:
         response = service.get_job_result_schema(job_id)
         return JobResultSchema(
@@ -161,27 +159,27 @@
                     item.is_single,
                     item.expected_count,
                 )
                 for item in response.items
             }
         )
 
-    def get(self, name: str) -> Optional[Union[MultipleStreamingResultFetcher, SingleStreamingResultFetcher]]:
+    def get(self, name: str) -> Optional[BaseStreamingResultFetcher]:
         """Get a handle to a named result from [stream_processing][qm.qua._dsl.stream_processing]
 
         Args:
             name: The named result using in [stream_processing][qm.qua._dsl.stream_processing]
 
 
         Returns:
             A handle object to the results `MultipleNamedJobResult` or `SingleNamedJobResult` or None if the named results in unknown
         """
         return self._all_results[name] if name in self._all_results else None
 
-    def __contains__(self, name: str):
+    def __contains__(self, name: str) -> bool:
         return name in self._all_results
 
     def wait_for_all_values(self, timeout: Optional[float] = None) -> bool:
         """Wait until we know all values were processed for all named results
 
         Args:
             timeout: Timeout for waiting in seconds
@@ -202,30 +200,30 @@
         return run_until_with_timeout(
             on_iteration_callback=on_iteration,
             on_complete_callback=on_complete,
             timeout=timeout if timeout else float("infinity"),
             timeout_message="Job was not done in time",
         )
 
-    def get_debug_data(self, writer: Optional[Union[BufferedWriter, BytesIO, str]] = None):
+    def get_debug_data(self, writer: Optional[Union[BinaryIO, str]] = None) -> None:
         """
         Returns:
             debugging data to report to QM
         """
         if writer is None:
             writer = f"./{self._job_id}-DebugData.zip"
 
         owning_writer = False
-        if type(writer) is str:
+        if isinstance(writer, str):
             writer = open(writer, "wb+")
             owning_writer = True
 
         try:
             run_async(self._fetch_all_job_debug_data(writer))
 
         finally:
             if owning_writer:
                 writer.close()
 
-    async def _fetch_all_job_debug_data(self, writer):
+    async def _fetch_all_job_debug_data(self, writer: BinaryIO) -> None:
         async for result in self._service.get_job_debug_data(self._job_id):
-            writer.write(result)
+            writer.write(result.data)
```

### Comparing `qm_qua-1.1.1/qm/serialization/expression_serializing_visitor.py` & `qm_qua-1.1.2/qm/serialization/expression_serializing_visitor.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import betterproto
 
-from qm.serialization.qua_node_visitor import QuaNodeVisitor
-from qm.exceptions import QmQuaException
 from qm.grpc import qua
+from qm.exceptions import QmQuaException
+from qm.serialization.qua_node_visitor import QuaNodeVisitor
 
 
 class ExpressionSerializingVisitor(QuaNodeVisitor):
     def __init__(self) -> None:
         self._out = ""
         super().__init__()
```

### Comparing `qm_qua-1.1.1/qm/serialization/generate_qua_script.py` & `qm_qua-1.1.2/qm/serialization/generate_qua_script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import datetime
 import re
 import sys
-import traceback
 import types
-from typing import Optional, Dict, Any
+import datetime
+import traceback
+from typing import Any, Dict, Optional
 
 import betterproto
 import numpy as np
 
 from qm import Program, version
-from qm.serialization.qua_node_visitor import QuaNodeVisitor
-from qm.serialization.qua_serializing_visitor import QuaSerializingVisitor
-from qm.exceptions import ConfigSerializationException
-from qm.grpc.qua_config import QuaConfig
 from qm.program import load_config
+from qm.grpc.qua_config import QuaConfig
+from qm.exceptions import ConfigSerializationException
 from qm.program.ConfigBuilder import convert_msg_to_config
+from qm.serialization.qua_node_visitor import QuaNodeVisitor
+from qm.serialization.qua_serializing_visitor import QuaSerializingVisitor
 
 SERIALIZATION_VALIDATION_ERROR = "SERIALIZATION VALIDATION ERROR"
 
 LOADED_CONFIG_ERROR = "LOADED CONFIG SERIALIZATION ERROR"
 
 CONFIG_ERROR = "CONFIG SERIALIZATION ERROR"
```

### Comparing `qm_qua-1.1.1/qm/serialization/qua_node_visitor.py` & `qm_qua-1.1.2/qm/serialization/qua_node_visitor.py`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/serialization/qua_serializing_visitor.py` & `qm_qua-1.1.2/qm/serialization/qua_serializing_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional, Union, List
 import re
+from typing import List, Union, Optional
 
 import betterproto
-from betterproto.lib.google.protobuf import ListValue, Value
+from betterproto.lib.google.protobuf import Value, ListValue
 
-from qm.serialization.expression_serializing_visitor import ExpressionSerializingVisitor
-from qm.serialization.qua_node_visitor import QuaNodeVisitor
-from qm.exceptions import QmQuaException
 from qm.grpc import qua
+from qm.exceptions import QmQuaException
+from qm.serialization.qua_node_visitor import QuaNodeVisitor
+from qm.serialization.expression_serializing_visitor import ExpressionSerializingVisitor
 
 
 class QuaSerializingVisitor(QuaNodeVisitor):
     def __init__(self) -> None:
         super().__init__()
         self._indent = 0
         self._lines = []
```

### Comparing `qm_qua-1.1.1/qm/simulate/interface.py` & `qm_qua-1.1.2/qm/simulate/interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import abc
 from dataclasses import dataclass
-from typing import Union, TypeVar, Generic, NewType, List
+from typing import List, Union, Optional
 
-from qm.grpc.frontend import (
-    SimulationRequest,
-    ExecutionRequestSimulateSimulationInterfaceNone,
-)
+from qm.grpc.frontend import SimulationRequest, ExecutionRequestSimulateSimulationInterfaceNone
 
 
-class SimulationConfig(object):
+class SimulatorInterface(metaclass=abc.ABCMeta):
+    @abc.abstractmethod
+    def update_simulate_request(self, request: SimulationRequest) -> SimulationRequest:
+        pass
+
+
+class SimulationConfig:
     """Creates a configuration object to pass to
-    [qm.QuantumMachinesManager.QuantumMachinesManager.simulate][]
+    [qm.quantum_machines_manager.QuantumMachinesManager.simulate][]
 
     Args:
         duration (int): The duration to run the simulation for, in clock
             cycles
         include_analog_waveforms (bool): True to collect simulated
             analog waveform names
         include_digital_waveforms (bool): True to collect simulated
@@ -33,45 +36,39 @@
     """
 
     duration = 0
     simulate_analog_outputs = False
 
     def __init__(
         self,
-        duration=0,
-        include_analog_waveforms=False,
-        include_digital_waveforms=False,
-        simulation_interface=None,
-        controller_connections: List["ControllerConnection"] = None,
-        extraProcessingTimeoutInMs=-1,
+        duration: int = 0,
+        include_analog_waveforms: bool = False,
+        include_digital_waveforms: bool = False,
+        simulation_interface: Optional[SimulatorInterface] = None,
+        controller_connections: Optional[List["ControllerConnection"]] = None,
+        extraProcessingTimeoutInMs: int = -1,
     ):
         if controller_connections is None:
             controller_connections = []
         super(SimulationConfig, self).__init__()
         self.duration = duration
         self.include_analog_waveforms = include_analog_waveforms is True
         self.include_digital_waveforms = include_digital_waveforms is True
         self.simulation_interface = simulation_interface
         self.controller_connections = controller_connections
         self.extraProcessingTimeoutInMs = extraProcessingTimeoutInMs
 
-    def update_simulate_request(self, request: SimulationRequest):
+    def update_simulate_request(self, request: SimulationRequest) -> SimulationRequest:
         if self.simulation_interface is None:
             request.simulate.simulation_interface.none = ExecutionRequestSimulateSimulationInterfaceNone()
         else:
             request = self.simulation_interface.update_simulate_request(request)
         return request
 
 
-class SimulatorInterface(metaclass=abc.ABCMeta):
-    @abc.abstractmethod
-    def update_simulate_request(self, request: SimulationRequest) -> SimulationRequest:
-        pass
-
-
 @dataclass
 class InterOpxAddress:
     """Args:
     controller (str): The name of the controller
     is_left_connection (bool)
     """
 
@@ -86,17 +83,14 @@
     channel_number (int)
     """
 
     controller: str
     channel_number: int
 
 
-InterOpxPairing = NewType("InterOpxPairing", Union[InterOpxAddress, InterOpxChannel])
-T = TypeVar("T", InterOpxPairing, InterOpxPairing)
-
+InterOpxPairing = Union[InterOpxAddress, InterOpxChannel]
 
-class ControllerConnection(Generic[T]):
-    """"""
 
-    def __init__(self, source: T, target: T):
-        self.source = source
-        self.target = target
+@dataclass
+class ControllerConnection:
+    source: InterOpxPairing
+    target: InterOpxPairing
```

### Comparing `qm_qua-1.1.1/qm/simulate/loopback.py` & `qm_qua-1.1.2/qm/simulate/loopback.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,75 @@
+from typing import List, Tuple
+
+from qm.simulate.interface import SimulatorInterface
 from qm.grpc.frontend import (
     SimulationRequest,
     ExecutionRequestSimulateSimulationInterfaceLoopback,
     ExecutionRequestSimulateSimulationInterfaceLoopbackConnections,
 )
-from qm.simulate.interface import SimulatorInterface
 
 
 class LoopbackInterface(SimulatorInterface):
     """Creates a loopback interface for use in
     [qm.simulate.interface.SimulationConfig][].
     A loopback connects the output of the OPX into it's input. This can be defined
     directly using the ports or through the elements.
 
     Args:
         connections (list):
-            List of tuples with loopback connections. Each tuple can be
+            List of tuples with loopback connections. Each tuple should represent physical connection between ports:
 
-                1. Physical connection between ports:
+                    ``(from_controller: str, from_port: int, to_controller: str, to_port: int)``
 
-                    ``(fromController: str, fromPort: int, toController: str, toPort: int)``
-
-                2. Virtual connection between elements:
-
-                    ``(fromQE: str, toQE: str, toQEInput: int)``
         latency (int): The latency between the OPX outputs and its
             input.
         noisePower (float): How much noise to add to the input.
 
     Example:
         ```python
         job = qmm.simulate(config, prog, SimulationConfig(
                           duration=20000,
                           # loopback from output 1 to input 2 of controller 1:
                           simulation_interface=LoopbackInterface([("con1", 1, "con1", 2)])
         ```
     """
 
-    def __init__(self, connections, latency=24, noisePower=0.0):
-        if type(latency) is not int or latency < 0:
-            raise Exception("latency must be a positive integer")
+    def __init__(self, connections: List[Tuple[str, int, str, int]], latency: int = 24, noisePower: float = 0.0):
+        self._validate_inputs(connections, latency, noisePower)
 
         self.latency = latency
+        self.noisePower = float(noisePower)
+        self.connections = connections.copy()
 
-        if (type(noisePower) is not float and type(noisePower) is not int) or noisePower < 0:
+    @staticmethod
+    def _validate_inputs(connections: List[Tuple[str, int, str, int]], latency: int, noise_power: float) -> None:
+        if (not isinstance(latency, int)) or latency < 0:
+            raise Exception("latency must be a positive integer")
+        if (not isinstance(noise_power, (int, float))) or noise_power < 0:
             raise Exception("noisePower must be a positive number")
-
-        self.noisePower = noisePower
-
-        if type(connections) is not list:
+        if not isinstance(connections, list):
             raise Exception("connections argument must be of type list")
-
-        self.connections = list()
         for connection in connections:
-            if type(connection) is not tuple:
-                raise Exception("each connection must be of type tuple")
-            if len(connection) == 4:
-                if (
-                    type(connection[0]) is not str
-                    or type(connection[1]) is not int
-                    or type(connection[2]) is not str
-                    or type(connection[3]) is not int
-                ):
-                    raise Exception("connection should be (fromController, fromPort, toController, toPort)")
-                self.connections.append(connection)
-            elif len(connection) == 3:
-                if type(connection[0]) is not str or type(connection[1]) is not str or type(connection[2]) is not int:
-                    raise Exception("connection should be (fromQE, toQE, toQEInput)")
-                self.connections.append((connection[0], -1, connection[1], connection[2]))
-            else:
-                raise Exception("connection should be tuple of length 3 or 4")
+            LoopbackInterface._validate_connection(connection)
+
+    @staticmethod
+    def _validate_connection(connection: Tuple[str, int, str, int]) -> None:
+        if not isinstance(connection, tuple):
+            raise Exception("each connection must be a tuple")
+        if len(connection) != 4:
+            raise Exception("connection should be tuple of length 4.")
+        if not all(
+            [
+                isinstance(connection[0], str),
+                isinstance(connection[1], int),
+                isinstance(connection[2], str),
+                isinstance(connection[3], int),
+            ]
+        ):
+            raise Exception("connection should be (from_controller, from_port, to_controller, to_port)")
 
     def update_simulate_request(self, request: SimulationRequest) -> SimulationRequest:
         request.simulate.simulation_interface.loopback = ExecutionRequestSimulateSimulationInterfaceLoopback(
             latency=self.latency, noise_power=self.noisePower
         )
         for connection in self.connections:
             con = ExecutionRequestSimulateSimulationInterfaceLoopbackConnections(
```

### Comparing `qm_qua-1.1.1/qm/simulate/raw.py` & `qm_qua-1.1.2/qm/simulate/raw.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,15 @@
-from qm.grpc.frontend import SimulationRequest
+from typing import List, Tuple
+
 from qm.simulate.interface import SimulatorInterface
+from qm.grpc.frontend import (
+    SimulationRequest,
+    ExecutionRequestSimulateSimulationInterfaceRawInterface,
+    ExecutionRequestSimulateSimulationInterfaceRawInterfaceConnections,
+)
 
 
 class RawInterface(SimulatorInterface):
     """Creates a raw interface for use in [qm.simulate.interface.SimulationConfig][].
     A raw interface defines samples that will be inputted into the OPX inputs.
 
     Args:
@@ -19,36 +25,42 @@
         job = qmm.simulate(config, prog, SimulationConfig(
                           duration=20000,
                           # 500 ns of DC 0.2 V into con1 input 1
                           simulation_interface=RawInterface([("con1", 1, [0.2]*500)])
         ```
     """
 
-    def __init__(self, connections, noisePower=0.0):
-
-        if (type(noisePower) is not float and type(noisePower) is not int) or noisePower < 0:
-            raise Exception("noisePower must be a positive number")
+    def __init__(self, connections: List[Tuple[str, int, List[float]]], noisePower: float = 0.0):
+        self._validate_inputs(connections, noisePower)
 
-        self.noisePower = noisePower
+        self.noisePower = float(noisePower)
+        self.connections = connections.copy()
 
+    @staticmethod
+    def _validate_inputs(connections: List[Tuple[str, int, List[float]]], noise_power: float) -> None:
+        if not isinstance(noise_power, (int, float)) or noise_power < 0:
+            raise Exception("noisePower must be a positive number")
         if type(connections) is not list:
             raise Exception("connections argument must be of type list")
-
-        self.connections = list()
         for connection in connections:
-            if type(connection) is not tuple:
-                raise Exception("each connection must be of type tuple")
-            if len(connection) == 3:
-                if type(connection[0]) is not str or type(connection[1]) is not int or type(connection[2]) is not list:
-                    raise Exception("connection should be (fromController, fromPort, toSamples)")
-                self.connections.append(connection)
-            else:
-                raise Exception("connection should be tuple of length 3 or 4")
-
-    def update_simulate_request(self, request: SimulationRequest):
-        request.simulate.simulationInterface.raw.SetInParent()
-        request.simulate.simulationInterface.raw.noisePower = self.noisePower
+            RawInterface._validate_connection(connection)
+
+    @staticmethod
+    def _validate_connection(connection: Tuple[str, int, List[float]]) -> None:
+        if not isinstance(connection, tuple):
+            raise Exception("each connection must be of type tuple")
+        if len(connection) != 3:
+            raise Exception("connection should be tuple of length 3")
+        if not all([isinstance(connection[0], str), isinstance(connection[1], int), isinstance(connection[2], list)]):
+            raise Exception("connection should be (from_controller, from_port, to_samples)")
+
+    def update_simulate_request(self, request: SimulationRequest) -> SimulationRequest:
+        request.simulate.simulation_interface.raw = ExecutionRequestSimulateSimulationInterfaceRawInterface(
+            noise_power=self.noisePower
+        )
         for connection in self.connections:
-            con = request.simulate.simulationInterface.raw.connections.add()
-            con.fromController = connection[0]
-            con.fromPort = connection[1]
-            con.toSamples.extend(connection[2])
+            request.simulate.simulation_interface.raw.connections.append(
+                ExecutionRequestSimulateSimulationInterfaceRawInterfaceConnections(
+                    from_controller=connection[0], from_port=connection[1], to_samples=connection[2]
+                )
+            )
+        return request
```

### Comparing `qm_qua-1.1.1/qm/sources/logo_qm_square.png` & `qm_qua-1.1.2/qm/sources/logo_qm_square.png`

 * *Files identical despite different names*

### Comparing `qm_qua-1.1.1/qm/type_hinting/config_types.py` & `qm_qua-1.1.2/qm/type_hinting/config_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Dict, Union, Tuple, List
-from typing_extensions import TypedDict, Literal
+from typing_extensions import TypedDict
+from typing import Dict, List, Tuple, Union
 
 from qm.type_hinting.general import Number
 
 PortReferenceType = Tuple[str, int]
 
 
 # TODO: This is a placeholder while we still use dicts, once we move to pydantics we can simply change the
@@ -40,27 +40,27 @@
 class DigitalInputPortConfigType(TypedDict, total=False):
     deadtime: int
     polarity: str
     threshold: Number
     connectivity: Tuple[str, str]
 
 
-class OctaveConfigType(TypedDict, total=False):
-    loopbacks: List[Tuple[Tuple[str, str], str]]
-
-
 class ControllerConfigType(TypedDict, total=False):
-    type: Literal["opx1"]
+    type: str
     analog_outputs: Dict[int, AnalogOutputPortConfigType]
     analog_inputs: Dict[int, AnalogInputPortConfigType]
     digital_outputs: Dict[int, DigitalOutputPortConfigType]
     digital_inputs: Dict[int, DigitalInputPortConfigType]
     connectivity: str
 
 
+class OctaveConfigType(TypedDict, total=False):
+    loopbacks: List[Tuple[Tuple[str, str], str]]
+
+
 class DigitalInputConfigType(TypedDict, total=False):
     delay: int
     buffer: int
     port: PortReferenceType
 
 
 class IntegrationWeightConfigType(TypedDict, total=False):
```

### Comparing `qm_qua-1.1.1/qm/type_hinting/general.py` & `qm_qua-1.1.2/qm/type_hinting/general.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import os
 import pathlib
-import numpy
-from typing import TypeVar, Union, ClassVar
 from typing_extensions import Protocol
+from typing import Any, Dict, Union, ClassVar
+
+import numpy
 
-PathLike = TypeVar("PathLike", str, pathlib.Path)
+PathLike = Union[str, bytes, pathlib.Path, os.PathLike]
 Number = Union[int, float]
 Value = Union[Number, bool]
 
 NumpyNumber = Union[numpy.floating, numpy.integer]
 NumpyValue = Union[NumpyNumber, numpy.bool_]
 
 NumpySupportedNumber = Union[Number, NumpyNumber]
 NumpySupportedFloat = Union[float, numpy.floating]
 NumpySupportedValue = Union[Value, NumpyValue]
 
 
 class DataClassType(Protocol):
-    __dataclass_fields__: ClassVar[dict]
+    __dataclass_fields__: ClassVar[Dict[str, Any]]
```

### Comparing `qm_qua-1.1.1/qm/type_hinting/simulator_types.py` & `qm_qua-1.1.2/qm/type_hinting/simulator_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Set, List, Dict, Optional
-
 from typing_extensions import TypedDict
+from typing import Set, Dict, List, Optional
 
 
 class PulserLocationType(TypedDict, total=False):
     controllerName: str
     pulserIndex: int
 
 
@@ -33,15 +32,14 @@
     endsAt: int
     outputPorts: Set[int]
     quantumElements: str
 
 
 class PlayedAnalogWaveformType(PlayedWaveformType, total=False):
     currentFrame: List[float]
-    currentFrame: List[float]
     currentCorrectionElements: List[float]
     currentIntermediateFrequency: float
     currentGMatrixElements: List[float]
     currentDCOffsetByPort: Dict[int, float]
     currentPhase: float
     chirpInfo: ChirpInfoType
```

### Comparing `qm_qua-1.1.1/qm/utils/__init__.py` & `qm_qua-1.1.2/qm/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,22 @@
+from qm.utils.general_utils import run_until_with_timeout
+from qm.utils.protobuf_utils import LOG_LEVEL_MAP, list_fields
+from qm.utils.deprecation_utils import deprecation_message, deprecate_to_property
 from qm.utils.types_utils import (
-    fix_object_data_type,
-    get_all_iterable_data_types,
+    is_iter,
     collection_has_type,
-    collection_has_type_bool,
     collection_has_type_int,
+    collection_has_type_bool,
     collection_has_type_float,
-    is_iter,
+    get_all_iterable_data_types,
     get_iterable_elements_datatype,
 )
 
-from qm.utils.deprecation_utils import deprecate_to_property, deprecation_message
-
-from qm.utils.protobuf_utils import LOG_LEVEL_MAP, list_fields
-
-from qm.utils.general_utils import run_until_with_timeout
-
 __all__ = [
     "LOG_LEVEL_MAP",
-    "fix_object_data_type",
     "get_all_iterable_data_types",
     "collection_has_type",
     "collection_has_type_bool",
     "collection_has_type_int",
     "collection_has_type_float",
     "is_iter",
     "get_iterable_elements_datatype",
```

### Comparing `qm_qua-1.1.1/qm/utils/deprecation_utils.py` & `qm_qua-1.1.2/qm/utils/deprecation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import warnings
-from typing import TypeVar, Any
+from typing import Any, TypeVar
 
 
 def deprecation_message(method: str, deprecated_in: str, removed_in: str, details: str) -> str:
     """
     Generates a deprecation message for deprecation a function.
 
     This call:
```

### Comparing `qm_qua-1.1.1/qm/utils/general_utils.py` & `qm_qua-1.1.2/qm/utils/general_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import time
-from typing import TypeVar, Callable, Optional
+import logging
+from typing import Any, Dict, Generic, TypeVar, Callable
 
 T = TypeVar("T")
 
 
 def run_until_with_timeout(
     on_iteration_callback: Callable[[], bool],
-    on_complete_callback: Callable[[], Optional[T]] = lambda: None,
+    # The type ignore can be removed in 3.12 with `T = TypeVar("T", default=None)`
+    on_complete_callback: Callable[[], T] = lambda: None,  # type: ignore[assignment, return-value]
     timeout: float = float("infinity"),
     loop_interval: float = 0.1,
     timeout_message: str = "Timeout Exceeded",
-) -> Optional[T]:
+) -> T:
     """
 
     :param on_iteration_callback: A callback that returns bool that is called every loop iteration.
      If True is returned, the loop is complete and on_complete_callback is called.
 
     :param on_complete_callback: A callback that is called when the loop is completed.
     This function returns the return value of on_complete_callback
@@ -37,7 +39,23 @@
         if on_iteration_callback():
             return on_complete_callback()
 
         time.sleep(loop_interval)
 
         if time.time() >= end:
             raise TimeoutError(timeout_message)
+
+
+_T = TypeVar("_T")
+
+
+class Singleton(type, Generic[_T]):
+    _instances: Dict["Singleton[_T]", _T] = {}
+
+    def __call__(cls, *args: Any, **kwargs: Any) -> _T:
+        if cls not in cls._instances:
+            cls._instances[cls] = super().__call__(*args, **kwargs)
+        return cls._instances[cls]
+
+
+def is_debug() -> bool:
+    return logging.getLogger("qm").level <= logging.DEBUG
```

### Comparing `qm_qua-1.1.1/qm/utils/protobuf_utils.py` & `qm_qua-1.1.2/qm/utils/protobuf_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import dataclasses
 import logging
-from typing import Union, Dict, Iterable
+import dataclasses
+from typing import Dict, Union, Iterable
 
 import betterproto
 
 from qm.grpc.general_messages import MessageLevel
 from qm.type_hinting.general import DataClassType
 
 LOG_LEVEL_MAP = {
```

### Comparing `qm_qua-1.1.1/qm/utils/types_utils.py` & `qm_qua-1.1.2/qm/utils/types_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,45 @@
-from typing import TypeVar, Collection, Type, Iterable, Any, Set, Union, Optional, cast, Sequence
+from typing_extensions import SupportsIndex
+from typing import (
+    Any,
+    Set,
+    Type,
+    Union,
+    TypeVar,
+    Iterable,
+    Optional,
+    Sequence,
+    Collection,
+    SupportsInt,
+    SupportsFloat,
+    cast,
+)
 
 import numpy as np
 import numpy.typing
 
-from qm.type_hinting import Value, NumpySupportedValue
+from qm.type_hinting import Value
+from qm.exceptions import QmValueError
 
-
-def fix_object_data_type(obj: Optional[NumpySupportedValue]) -> Optional[Value]:
-    if isinstance(obj, (np.floating, np.integer, np.bool_)):
-        obj_item = obj.item()
-        if isinstance(obj_item, np.longdouble):
-            return float(obj_item)
-        else:
-            return obj_item
-    else:
-        return obj
+GeneralConversionType = Union[str, bytes, bytearray, memoryview]
+FloatConversionType = Union[SupportsFloat, SupportsIndex, GeneralConversionType]
+IntConversionType = Union[SupportsInt, SupportsIndex, GeneralConversionType]
+Bool = Union[bool, np.bool_]
+
+T = TypeVar("T", IntConversionType, FloatConversionType, Bool)
+
+
+def convert_object_type(obj: T) -> Value:
+    if isinstance(obj, (np.bool_, bool)):
+        return bool(obj)
+    if isinstance(obj, (np.integer, int)):
+        return int(obj)
+    if isinstance(obj, (np.floating, float)):
+        return float(obj)
+    raise QmValueError(f"cannot convert {type(obj)} to int | float | bool")
 
 
 def get_all_iterable_data_types(it: Iterable[Any]) -> Set[Type[Any]]:
     return {type(e) for e in it}
 
 
 C = TypeVar("C")
```

### Comparing `qm_qua-1.1.1/qm/waveform_report.py` & `qm_qua-1.1.2/qm/waveform_report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,99 @@
 import base64
-import dataclasses
-import datetime
-import functools
 import logging
 import os.path
-
-from typing import Dict, List, Optional, Any, Union, Tuple, Iterable
-from abc import abstractmethod
-from abc import ABCMeta
+import datetime
+import functools
+import dataclasses
+from copy import deepcopy
 from dataclasses import dataclass
+from typing_extensions import Protocol
+from abc import ABCMeta, abstractmethod
+from typing import (
+    Any,
+    Set,
+    Dict,
+    List,
+    Type,
+    Tuple,
+    Union,
+    Mapping,
+    TypeVar,
+    Callable,
+    Iterable,
+    Optional,
+    Sequence,
+    MutableMapping,
+    cast,
+)
 
 import numpy as np
-import plotly.colors
-import plotly.graph_objects as go
+import plotly.colors  # type: ignore[import]
+import plotly.graph_objects as go  # type: ignore[import]
+
+from qm.type_hinting.simulator_types import (
+    IqInfoType,
+    ChirpInfoType,
+    AdcAcquisitionType,
+    PlayedWaveformType,
+    PulserLocationType,
+    WaveformReportType,
+    PlayedAnalogWaveformType,
+)
+
+
+class HasPortsProtocol(Protocol):
+    controller: str
+
+    @property
+    def ports(self) -> List[int]:
+        return [1]
+
+
+T = TypeVar("T", bound="PlayedWaveform")
 
 
 @dataclass(frozen=True)
 class PlayedWaveform(metaclass=ABCMeta):
     waveform_name: str
     pulse_name: str
     length: int
     timestamp: int
-    iq_info: Dict[str, Any]
+    iq_info: IqInfoType
     element: str
     output_ports: List[int]
     controller: str
     pulser: Dict[str, Any]
 
-    @classmethod
-    def from_job_dict(cls, dict_description: Dict, formated_attribute_dict: Dict):
-        formated_attribute_dict.update(
+    @staticmethod
+    def _build_initialization_dict(
+        dict_description: PlayedWaveformType, formatted_attribute_dict: Optional[Dict[str, Any]] = None
+    ) -> Dict[str, Any]:
+        attribute_dict: Dict[str, Any]
+        if formatted_attribute_dict is None:
+            attribute_dict = {}
+        else:
+            attribute_dict = deepcopy(formatted_attribute_dict)
+
+        attribute_dict.update(
             pulse_name=dict_description["pulseName"],
             waveform_name=dict_description["waveformName"],
             timestamp=int(dict_description["timestamp"]),
             length=int(dict_description["length"]),
             iq_info=dict_description["iqInfo"],
             element=dict_description["quantumElements"],
             output_ports=[int(p) for p in dict_description["outputPorts"]],
             pulser=dict_description["pulser"],
             controller=dict_description["pulser"]["controllerName"],
         )
-        return cls(**formated_attribute_dict)
+        return attribute_dict
+
+    @classmethod
+    def from_job_dict(cls: Type[T], dict_description: PlayedWaveformType) -> T:
+        return cls(**cls._build_initialization_dict(dict_description))
 
     @property
     def ports(self) -> List[int]:
         return self.output_ports
 
     @property
     def is_iq(self) -> bool:
@@ -64,77 +113,85 @@
     def ends_at(self) -> int:
         return self.timestamp + self.length
 
     @abstractmethod
     def to_string(self) -> str:
         return ""
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.to_string()
 
-    def to_dict(self):
+    def to_dict(self) -> Dict[str, Any]:
         return dataclasses.asdict(self)
 
     def _common_attributes_to_printable_str_list(self) -> List[str]:
         waveform_type_string = "Type="
         if self.is_iq:
-            waveform_type_string += f"IQ Type ({'I' if self.iq_info['isI']  else 'Q'})"
+            waveform_type_string += f"IQ Type ({'I' if self.iq_info['isI'] else 'Q'})"
         else:
             waveform_type_string += "Single"
         return [
             f"Waveform Name={self.waveform_name}",
-            f"Pulse name={self.pulse_name.removeprefix('OriginPulseName=')}",
+            f"Pulse name={remove_prefix(self.pulse_name, 'OriginPulseName=')}",
             f"Start Time={self.timestamp} ns",
             f"Length={self.length} ns",
             f"Element={self.element}",
             f"Output Ports={self.output_ports}",
             waveform_type_string,
         ]
 
 
-def format_float(f) -> str:
+# str.removeprefix exists only for python 3.9+, this is here for backward compatibility
+def remove_prefix(text: str, prefix: str) -> str:
+    if text.startswith(prefix):
+        return text[len(prefix) :]
+    return text
+
+
+def format_float(f: float) -> str:
     return "{:.3f}".format(f)
 
 
-def pretty_string_freq(f) -> str:
+def pretty_string_freq(f: float) -> str:
     if f < 1000:
-        div, units = 1, "Hz"
+        div, units = 1.0, "Hz"
     elif 1000 <= f < 1_000_000:
-        div, units = 1000, "kHz"
+        div, units = 1000.0, "kHz"
     else:
         div, units = 10e6, "MHz"
-    return f"{format_float(f/div).rstrip('0').rstrip('.')}{units}"
+    return f"{format_float(f / div).rstrip('0').rstrip('.')}{units}"
 
 
 @dataclass(frozen=True)
 class PlayedAnalogWaveform(PlayedWaveform):
     current_amp_elements: List[float]
     current_dc_offset_by_port: Dict[str, float]
     current_intermediate_frequency: float
     current_frame: List[float]
     current_correction_elements: List[float]
-    chirp_info: Optional[Dict]
+    chirp_info: Optional[ChirpInfoType]
     current_phase: float
 
     @classmethod
-    def from_job_dict(cls, dict_description: Dict):
+    def from_job_dict(cls: Type[T], dict_description: PlayedWaveformType) -> T:
+        dict_description = cast(PlayedAnalogWaveformType, dict_description)
         pulse_chirp_info = dict_description["chirpInfo"]
         is_pulse_have_chirp = len(pulse_chirp_info["units"]) > 0 or len(pulse_chirp_info["rate"]) > 0
         formated_attribute_list = dict(
             current_amp_elements=dict_description["currentGMatrixElements"],
             current_dc_offset_by_port=dict_description["currentDCOffsetByPort"],
             current_intermediate_frequency=dict_description["currentIntermediateFrequency"],
             current_frame=dict_description["currentFrame"],
             current_correction_elements=dict_description["currentCorrectionElements"],
             chirp_info=pulse_chirp_info if is_pulse_have_chirp else None,
             current_phase=dict_description.get("currentPhase", 0),
         )
-        return super(cls, cls).from_job_dict(dict_description, formated_attribute_list)
+        return cls(**cls._build_initialization_dict(dict_description, formated_attribute_list))
 
-    def _to_custom_string(self, show_chirp=True) -> str:
+    def _to_custom_string(self, show_chirp: bool = True) -> str:
         _attributes = super()._common_attributes_to_printable_str_list()
         _attributes += (
             [
                 f"{k}={v if self.is_iq else v[0]}"
                 for k, v in [
                     (
                         "Amplitude Values",
@@ -163,16 +220,16 @@
     def to_string(self) -> str:
         return self._to_custom_string()
 
 
 @dataclass(frozen=True)
 class PlayedDigitalWaveform(PlayedWaveform):
     @classmethod
-    def from_job_dict(cls, dict_description: Dict):
-        return super(cls, cls).from_job_dict(dict_description, {})
+    def from_job_dict(cls: Type[T], dict_description: PlayedWaveformType) -> T:
+        return cls(**cls._build_initialization_dict(dict_description))
 
     def to_string(self) -> str:
         s = (
             "DigitalWaveform("
             + ("\n" + len("DigitalWaveform(") * " ").join(self._common_attributes_to_printable_str_list())
             + ")"
         )
@@ -180,33 +237,33 @@
 
 
 @dataclass(frozen=True)
 class AdcAcquisition:
     start_time: int
     end_time: int
     process: str
-    pulser: Dict[str, dict]
+    pulser: PulserLocationType
     quantum_element: str
     adc_ports: List[int]
     controller: str
 
     @classmethod
-    def from_job_dict(cls, dict_description: Dict):
+    def from_job_dict(cls, dict_description: AdcAcquisitionType) -> "AdcAcquisition":
         return cls(
             start_time=int(dict_description["startTime"]),
             end_time=int(dict_description["endTime"]),
             process=dict_description["process"],
             pulser=dict_description["pulser"],
             quantum_element=dict_description["quantumElement"],
             adc_ports=[int(p) + 1 for p in dict_description["adc"]],
             controller=dict_description["pulser"]["controllerName"],
         )
 
     @property
-    def ports(self):
+    def ports(self) -> List[int]:
         return self.adc_ports
 
     def to_string(self) -> str:
         return (
             "AdcAcquisition("
             + ("\n" + len("AdcAcquisition(") * " ").join(
                 [
@@ -216,144 +273,154 @@
                     f"element={self.quantum_element}",
                     f"input_ports={self.adc_ports}",
                 ]
             )
             + ")"
         )
 
-    def to_dict(self):
+    def to_dict(self) -> Dict[str, Any]:
         return dataclasses.asdict(self)
 
 
 class WaveformReport:
-    def __init__(self, descriptor_dict: Optional[Dict] = None, job_id=-1):
+    def __init__(self, descriptor_dict: Optional[WaveformReportType] = None, job_id: Union[int, str] = -1):
         self.analog_waveforms: List[PlayedAnalogWaveform] = []
         self.digital_waveforms: List[PlayedDigitalWaveform] = []
         self.adc_acquisitions: List[AdcAcquisition] = []
         self.job_id = job_id
         if descriptor_dict is not None:
-            for wf in descriptor_dict["analogWaveforms"]:
-                self.analog_waveforms.append(PlayedAnalogWaveform.from_job_dict(wf))
-            for wf in descriptor_dict["digitalWaveforms"]:
-                self.digital_waveforms.append(PlayedDigitalWaveform.from_job_dict(wf))
+            for awf in descriptor_dict["analogWaveforms"]:
+                self.analog_waveforms.append(PlayedAnalogWaveform.from_job_dict(awf))
+            for dwf in descriptor_dict["digitalWaveforms"]:
+                self.digital_waveforms.append(PlayedDigitalWaveform.from_job_dict(dwf))
             if "adcAcquisitions" in descriptor_dict:
                 for acq in descriptor_dict["adcAcquisitions"]:
                     self.adc_acquisitions.append(AdcAcquisition.from_job_dict(acq))
-        return
 
     @classmethod
-    def from_dict(cls, d: Dict, job_id=-1) -> "WaveformReport":
+    def from_dict(cls, d: WaveformReportType, job_id: Union[int, str] = -1) -> "WaveformReport":
         return cls(d, job_id)
 
     @property
-    def waveforms(self) -> List[PlayedWaveform]:
-        return self.analog_waveforms + self.digital_waveforms
+    def waveforms(self) -> Sequence[PlayedWaveform]:
+        return cast(List[PlayedWaveform], self.analog_waveforms) + cast(List[PlayedWaveform], self.digital_waveforms)
 
     @property
-    def controllers_in_use(self) -> List[str]:
-        return list(set([c.controller for c in (self.waveforms + self.adc_acquisitions)]))
+    def controllers_in_use(self) -> Sequence[str]:
+        waveform_controllers = [c.controller for c in self.waveforms]
+        adc_controller = [c.controller for c in self.adc_acquisitions]
+        return list(set(adc_controller + waveform_controllers))
 
     @property
     def num_controllers_in_use(self) -> int:
         return len(self.controllers_in_use)
 
-    def _sort_ports_dict(self, ports_in_use):
+    @staticmethod
+    def _sort_ports_dict(ports_in_use: Mapping[str, Iterable[int]]) -> Mapping[str, Sequence[int]]:
+        output: MutableMapping[str, Sequence[int]] = {}
         for k, v in ports_in_use.items():
-            ports_in_use[k] = sorted(v)
-        return ports_in_use
+            output[k] = sorted(v)
+        return output
 
-    def _get_output_ports_in_use(self, src: List, on_controller):
-        ports_in_use = {c: set() for c in self.controllers_in_use}
+    def _get_output_ports_in_use(
+        self, src: List[HasPortsProtocol], on_controller: Optional[str]
+    ) -> Union[Mapping[str, Sequence[int]], Sequence[int]]:
+        ports_in_use: MutableMapping[str, Set[int]] = {c: set() for c in self.controllers_in_use}
         for ap in src:
             ports_in_use[ap.controller].update(ap.ports)
-        self._sort_ports_dict(ports_in_use)
+        sorted_ports: Mapping[str, Sequence[int]] = self._sort_ports_dict(ports_in_use)
         if on_controller is None:
             if self.num_controllers_in_use == 1:
-                return ports_in_use[self.controllers_in_use[0]]
+                return sorted_ports[self.controllers_in_use[0]]
             else:
-                return ports_in_use
+                return sorted_ports
         else:
-            return ports_in_use[on_controller]
+            return sorted_ports[on_controller]
 
-    def analog_output_ports_in_use(self, on_controller: Optional[str] = None) -> Union[List[int], Dict[str, List[int]]]:
-        return self._get_output_ports_in_use(self.analog_waveforms, on_controller)
+    def analog_output_ports_in_use(
+        self, on_controller: Optional[str] = None
+    ) -> Union[Mapping[str, Sequence[int]], Sequence[int]]:
+        return self._get_output_ports_in_use(self.analog_waveforms, on_controller)  # type: ignore[arg-type]
 
     def digital_output_ports_in_use(
         self, on_controller: Optional[str] = None
-    ) -> Union[List[int], Dict[str, List[int]]]:
-        return self._get_output_ports_in_use(self.digital_waveforms, on_controller)
+    ) -> Union[Mapping[str, Sequence[int]], Sequence[int]]:
+        return self._get_output_ports_in_use(self.digital_waveforms, on_controller)  # type: ignore[arg-type]
 
-    def adcs_ports_in_use(self, on_controller: Optional[str] = None) -> Union[List[int], Dict[str, List[int]]]:
-        return self._get_output_ports_in_use(self.adc_acquisitions, on_controller)
+    def adcs_ports_in_use(
+        self, on_controller: Optional[str] = None
+    ) -> Union[Mapping[str, Sequence[int]], Sequence[int]]:
+        return self._get_output_ports_in_use(self.adc_acquisitions, on_controller)  # type: ignore[arg-type]
 
-    def to_string(self):
-        return "\n".join([wf.to_string() for wf in (self.waveforms + self.adc_acquisitions)])
+    def to_string(self) -> str:
+        waveforms_str = [wf.to_string() for wf in self.waveforms]
+        adc_string = [adc.to_string() for adc in self.adc_acquisitions]
+        return "\n".join(waveforms_str + adc_string)
 
-    def _transform_report_by_func(self, func) -> "WaveformReport":
+    def _transform_report_by_func(self, func: Callable[..., Any]) -> "WaveformReport":
         new_report = WaveformReport(job_id=self.job_id)
         new_report.analog_waveforms = list(filter(func, self.analog_waveforms))
         new_report.digital_waveforms = list(filter(func, self.digital_waveforms))
         new_report.adc_acquisitions = list(filter(func, self.adc_acquisitions))
         return new_report
 
-    def report_by_controllers(self) -> Dict[str, "WaveformReport"]:
-        by_controller_map = {k: None for k in self.controllers_in_use}
-
-        def _filter_func(r, conn):
+    def report_by_controllers(self) -> Mapping[str, "WaveformReport"]:
+        def _filter_func(r: HasPortsProtocol, conn: str) -> bool:
             return r.controller == conn
 
-        for con_name in by_controller_map.keys():
+        by_controller_map: Dict[str, "WaveformReport"] = {}
+        for con_name in self.controllers_in_use:
             con_filter = functools.partial(_filter_func, conn=con_name)
             by_controller_map[con_name] = self._transform_report_by_func(con_filter)
 
         return by_controller_map
 
-    def to_dict(self) -> Dict:
+    def to_dict(self) -> Dict[str, Any]:
         return {
             "analog_waveforms": [awf.to_dict() for awf in self.analog_waveforms],
             "digital_waveforms": [dwf.to_dict() for dwf in self.digital_waveforms],
             "adc_acquisitions": [acq.to_dict() for acq in self.adc_acquisitions],
         }
 
-    def get_report_by_output_ports(self, on_controller: Optional[str] = None):
+    def get_report_by_output_ports(self, on_controller: Optional[str] = None) -> Dict[str, Any]:
 
-        map_by_output_ports = {
+        map_by_output_ports: Dict[str, Dict[str, Any]] = {
             con_name: {
                 "analog_out": {k: [] for k in self.analog_output_ports_in_use(on_controller=con_name)},
                 "digital_out": {k: [] for k in self.digital_output_ports_in_use(on_controller=con_name)},
                 "analog_in": {k: [] for k in self.adcs_ports_in_use(on_controller=con_name)},
             }
             for con_name in self.controllers_in_use
         }
 
-        for wf in self.analog_waveforms:
-            for p in wf.output_ports:
-                map_by_output_ports[wf.controller]["analog_out"][p].append(wf)
-        for wf in self.digital_waveforms:
-            for p in wf.output_ports:
-                map_by_output_ports[wf.controller]["digital_out"][p].append(wf)
+        for awf in self.analog_waveforms:
+            for p in awf.output_ports:
+                map_by_output_ports[awf.controller]["analog_out"][p].append(awf)
+        for dwf in self.digital_waveforms:
+            for p in dwf.output_ports:
+                map_by_output_ports[dwf.controller]["digital_out"][p].append(dwf)
         for adc in self.adc_acquisitions:
             for p in adc.adc_ports:
                 map_by_output_ports[adc.controller]["analog_in"][p].append(adc)
 
         if on_controller is None:
             if self.num_controllers_in_use == 1:
                 return map_by_output_ports[self.controllers_in_use[0]]
             else:
                 return map_by_output_ports
         else:
             return map_by_output_ports[on_controller]
 
     def create_plot(
         self,
-        samples: Optional[Iterable] = None,
+        samples: Optional[Iterable[Any]] = None,  # TODO: for liran - fill type
         controllers: Optional[List[str]] = None,
         plot: bool = True,
         save_path: Optional[str] = None,
-    ):
+    ) -> None:
 
         if save_path is None:
             dirname, filename = "./", f"waveform_report_{self.job_id}"
         else:
             dirname, filename = os.path.split(save_path)
             if filename == "":
                 filename = f"waveform_report_{self.job_id}"
@@ -371,27 +438,27 @@
                 con_builder.save(dirname, filename)
             if plot:
                 con_builder.plot()
         return
 
 
 class _WaveformPlotBuilder:
-    def __init__(self, wf_report: WaveformReport, samples=None, job_id=-1):
+    def __init__(self, wf_report: WaveformReport, samples: Any = None, job_id: Union[int, str] = -1):
         self._report = wf_report
         if wf_report.num_controllers_in_use > 1:
             raise RuntimeError(
                 f"Plot Builder does not support plotting more than 1 controllers, yet. {os.linesep}"
                 "Please provide a report containing a single controller."
             )
         self._samples = samples
         self._job_id = job_id
-        self._figure: Union[go.Figure, None] = None
-        self._already_registered_qe = set()
-        self._colormap = {}
-        self._max_parallel_traces_per_row = {}
+        self._figure: Optional[go.Figure] = None
+        self._already_registered_qe: Set[str] = set()
+        self._colormap: Dict[str, Any] = {}
+        self._max_parallel_traces_per_row: Dict[str, Any] = {}  # TODO: for liran - fill type
         return
 
     @property
     def _num_rows(self) -> int:
         with_samples = self._samples is not None
         num_rows = (
             len(self._report.analog_output_ports_in_use()) + len(self._report.digital_output_ports_in_use())
@@ -407,61 +474,61 @@
     def _num_analog_rows(self) -> int:
         return len(self._report.analog_output_ports_in_use()) * (1 + (self._samples is not None))
 
     @property
     def _num_digital_rows(self) -> int:
         return len(self._report.digital_output_ports_in_use()) * (1 + (self._samples is not None))
 
-    def _is_row_analog(self, r) -> bool:
+    def _is_row_analog(self, r: int) -> bool:
         return 1 <= r <= self._num_analog_rows
 
-    def _is_row_digital(self, r) -> bool:
+    def _is_row_digital(self, r: int) -> bool:
         return self._num_analog_rows < r <= self._num_output_rows
 
-    def _is_row_analog_input(self, r) -> bool:
+    def _is_row_analog_input(self, r: int) -> bool:
         return self._num_output_rows < r <= self._num_rows
 
     @property
     def _xrange(self) -> int:
         return (
             len(self._samples.analog["1"])
             if self._samples is not None
             else max(self._report.waveforms, key=lambda x: x.ends_at).ends_at + 100
         )
 
-    def _pre_setup(self):
+    def _pre_setup(self) -> None:
         self._setup_qe_colorscale()
         self._calculate_max_parallel_traces_per_row()
         return
 
-    def _get_all_qe_used(self):
+    def _get_all_qe_used(self) -> Sequence[str]:
         return list(set([wf.element for wf in self._report.waveforms]))
 
-    def _setup_qe_colorscale(self):
+    def _setup_qe_colorscale(self) -> None:
         qe_in_use = self._get_all_qe_used()
         n_colors = len(qe_in_use)
         samples = plotly.colors.qualitative.Pastel + plotly.colors.qualitative.Safe
         if n_colors > len(samples):
             samples += plotly.colors.sample_colorscale(
                 "turbo",
                 [n / (n_colors - len(samples)) for n in range(n_colors - len(samples))],
             )
         self._colormap = dict(zip(qe_in_use, samples))
         return
 
-    def _calculate_max_parallel_traces_per_row(self):
+    def _calculate_max_parallel_traces_per_row(self) -> None:
         report_by_output_port = self._report.get_report_by_output_ports()
         self._max_parallel_traces_per_row["analog"] = {}
         self._max_parallel_traces_per_row["digital"] = {}
 
-        def calc_row(waveform_list):
+        def calc_row(waveform_list: List[Any]) -> int:  # TODO: for liran - fill type
             max_in_row = 0
             functional_ts = sorted(
                 [(r.timestamp, 1) for r in waveform_list] + [(r.ends_at, -1) for r in waveform_list],
-                key=lambda t: t[0],
+                key=lambda t: t[0],  # type: ignore[no-any-return]
             )
             for _, f in functional_ts:
                 max_in_row = max(max_in_row, max_in_row + f)
             return max_in_row
 
         for output_port, waveform_list in report_by_output_port["analog_out"].items():
             self._max_parallel_traces_per_row["analog"][output_port] = calc_row(waveform_list)
@@ -470,33 +537,35 @@
             self._max_parallel_traces_per_row["digital"][output_port] = calc_row(waveform_list)
 
         return
 
     def _is_intersect(self, r1: Tuple[int, int], r2: Tuple[int, int]) -> bool:
         return (r1[0] <= r2[0] <= r1[1]) or (r1[0] <= r2[1] <= r1[1]) or (r2[0] < r1[0] and r2[1] > r1[1])
 
-    def _get_hover_text(self, played_waveform):
+    def _get_hover_text(self, played_waveform: PlayedWaveform) -> str:
         waveform_desc = played_waveform.to_string()
         if isinstance(played_waveform, PlayedAnalogWaveform):
             if played_waveform.chirp_info is not None:
                 waveform_desc = played_waveform._to_custom_string(False)
                 s = (
                     f"rate={played_waveform.chirp_info['rate']},units={played_waveform.chirp_info['units']},"
                     f" times={played_waveform.chirp_info['times']}\n"
                     + f"start_freq={pretty_string_freq(played_waveform.chirp_info['startFrequency'])}, "
                     + f"end_freq={pretty_string_freq(played_waveform.chirp_info['endFrequency'])}"
                 )
 
                 waveform_desc = f"<b>Chirp Pulse</b>\n({s})\n" + waveform_desc
         return "%{x}ns<br>" + waveform_desc.replace("\n", "</br>") + "<extra></extra>"
 
-    def _get_output_port_waveform_plot_data(self, port_played_waveforms: List[PlayedWaveform], gui_args):
-        graph_data = []
-        annotations = []
-        levels = []
+    def _get_output_port_waveform_plot_data(
+        self, port_played_waveforms: List[PlayedWaveform], gui_args: Dict[str, Any]
+    ) -> Any:  # TODO: for liran - fill type
+        graph_data: List[Any] = []  # TODO: for liran - fill type
+        annotations: List[Any] = []  # TODO: for liran - fill type
+        levels: List[Any] = []  # TODO: for liran - fill type
         x_axis_name = gui_args["x_axis_name"]
         max_in_row = gui_args["max_in_row"]
         diff_between_traces, start_y = (0.2, 1.2) if max_in_row <= 7 else (1.4 / max_in_row, 1.45)
         y_level = [start_y] * 3
         for wf in port_played_waveforms:
             x_axis_points = (wf.timestamp, wf.ends_at)
             num_intersections = len([l for l in levels if self._is_intersect(l, x_axis_points)])
@@ -506,15 +575,15 @@
             graph_data.append(
                 go.Scatter(
                     x=[x_axis_points[0], sum(x_axis_points) // 2, x_axis_points[1]],
                     y=y_level,
                     mode="lines+markers+text",
                     text=[
                         "",
-                        f"{wf.pulse_name.removeprefix('OriginPulseName=')}"
+                        f"{remove_prefix(wf.pulse_name, 'OriginPulseName=')}"
                         + (f"({wf.get_iq_association})" if wf.is_iq else ""),
                         "",
                     ],
                     hovertemplate=self._get_hover_text(wf),
                     textfont=dict(size=10),
                     xaxis=x_axis_name,
                     name=wf.element,
@@ -528,29 +597,30 @@
                 )
             )
             self._already_registered_qe.add(wf.element)
 
         return graph_data, annotations
 
     def _add_plot_data_for_analog_output_port(
-        self, figure_row_number, output_port, port_waveforms: List[PlayedWaveform]
-    ):
+        self, figure_row_number: int, output_port: int, port_waveforms: List[PlayedWaveform]
+    ) -> None:
         if len(port_waveforms) == 0:
             return
         use_samples = self._samples is not None
 
         xaxis_name = f"x{figure_row_number}"
         port_wf_plot, annotations = self._get_output_port_waveform_plot_data(
             port_waveforms,
             {
                 "x_axis_name": xaxis_name,
                 "max_in_row": self._max_parallel_traces_per_row["analog"][output_port],
             },
         )
         row_number = figure_row_number * (1 + use_samples)
+        assert isinstance(self._figure, go.Figure)
         self._figure.add_traces(port_wf_plot, rows=row_number, cols=1)
         [self._figure.add_annotation(annot, row=row_number, col=1) for annot in annotations]
 
         if use_samples:
             port_samples = self._samples.analog[str(output_port)]
 
             self._figure.add_trace(
@@ -563,29 +633,30 @@
                 row=(figure_row_number * 2 - 1),
                 col=1,
             )
 
         return
 
     def _add_plot_data_for_digital_output_port(
-        self, figure_row_number, output_port, port_waveforms: List[PlayedWaveform]
-    ):
+        self, figure_row_number: int, output_port: int, port_waveforms: List[PlayedWaveform]
+    ) -> None:
         if len(port_waveforms) == 0:
             return
         use_samples = self._samples is not None
 
         xaxis_name = f"x{figure_row_number}"
         port_wf_plot, annotations = self._get_output_port_waveform_plot_data(
             port_waveforms,
             {
                 "x_axis_name": xaxis_name,
                 "max_in_row": self._max_parallel_traces_per_row["digital"][output_port],
             },
         )
         row_number = figure_row_number * (1 + use_samples)
+        assert isinstance(self._figure, go.Figure)
         self._figure.add_traces(port_wf_plot, rows=row_number, cols=1)
         [self._figure.add_annotation(annot, row=row_number, col=1) for annot in annotations]
 
         if use_samples:
             port_samples = self._samples.digital.get(str(output_port), np.zeros(shape=self._xrange))
             if port_samples is None:
                 logging.log(
@@ -606,20 +677,20 @@
                 col=1,
             )
 
         return
 
     def _add_plot_data_for_adc_port(
         self,
-        figure_row_number,
-        adc_port_number,
+        figure_row_number: int,
+        adc_port_number: int,
         adc_port_acquisitions: List[AdcAcquisition],
-    ):
-        graph_data = []
-        levels = []
+    ) -> None:
+        graph_data: List[Any] = []
+        levels: List[Any] = []
         y_level = [1.2] * 3
         for adc in adc_port_acquisitions:
             x_axis_points = (adc.start_time, adc.end_time)
             num_intersections = len([l for l in levels if self._is_intersect(l, x_axis_points)])
             levels.append(x_axis_points)
             prev_y = 1.2 if num_intersections == 0 else y_level[0]
             y_level = [prev_y - 0.2] * 3
@@ -643,19 +714,20 @@
                         symbol=["line-ns", "line-ew", "line-ns"],
                     ),
                     line=dict(color=self._colormap[adc.quantum_element], width=5),
                 )
             )
             self._already_registered_qe.add(adc.quantum_element)
 
+        assert isinstance(self._figure, go.Figure)
         self._figure.add_traces(graph_data, rows=figure_row_number, cols=1)
 
         return
 
-    def _add_data(self):
+    def _add_data(self) -> None:
         for (figure_row_number, (output_port, port_waveforms_list)) in enumerate(
             self._report.get_report_by_output_ports()["analog_out"].items()
         ):
             self._add_plot_data_for_analog_output_port(figure_row_number + 1, output_port, port_waveforms_list)
 
         for (figure_row_number, (output_port, port_waveforms_list)) in enumerate(
             self._report.get_report_by_output_ports()["digital_out"].items()
@@ -672,15 +744,16 @@
             self._add_plot_data_for_adc_port(
                 figure_row_number + self._num_output_rows + 1,
                 input_port,
                 adc_acquisition_list,
             )
         return
 
-    def _update_extra_features(self):
+    def _update_extra_features(self) -> None:
+        assert isinstance(self._figure, go.Figure)
         all_xaxis_names = sorted(
             [a for a in self._figure.layout.__dir__() if a.startswith("xaxis")],
             key=lambda s: int(s.removeprefix("xaxis")) if s.removeprefix("xaxis").isnumeric() else 0,
         )
         all_xaxis_names_short = {
             k: "x" + k.removeprefix("xaxis") if k.removeprefix("xaxis").isnumeric() else "" for k in all_xaxis_names
         }
@@ -749,24 +822,24 @@
             sizex=0.1,
             sizey=0.1,
             xanchor="center",
             yanchor="bottom",
         )
         return
 
-    def _setup_figure(self):
+    def _setup_figure(self) -> None:
         self._figure = go.Figure()
         with_samples = self._samples is not None
         num_rows = max(self._num_rows, 4)
         titles = [f"Analog-Out-{a}" for a in self._report.analog_output_ports_in_use()] + [
             f"Digital-Out-{d}" for d in self._report.digital_output_ports_in_use()
         ]
         if with_samples:
-            zipped = list(zip(titles, [[]] * self._num_output_rows))
-            titles = [item for z in zipped for item in z]
+            zipped: List[Any] = list(zip(titles, [[]] * self._num_output_rows))
+            titles: List[Any] = [item for z in zipped for item in z]  # type: ignore[no-redef]
         titles += [f"Analog-In-{a}" for a in self._report.adcs_ports_in_use()]
 
         if with_samples:
             specs = ([[{"t": 1.2 / (num_rows * 5)}]] + [[{"b": 1.2 / (num_rows * 5)}]]) * (
                 self._num_output_rows // 2
             ) + [[{"t": 1 / (num_rows * 4)}]] * len(self._report.adcs_ports_in_use())
         else:
@@ -828,15 +901,15 @@
                 self._figure.update_yaxes(
                     title=dict(text=title_text, standoff=5, font=dict(size=9)),
                     row=r,
                     col=1,
                 )
 
         for r in list(range(1 + with_samples, self._num_output_rows + 1, 1 + with_samples)) + [
-            p + self._num_output_rows for p in self._report.adcs_ports_in_use()
+            p + self._num_output_rows for p in self._report.adcs_ports_in_use()  # type: ignore[operator]
         ]:
             self._figure.update_yaxes(
                 range=[-0.5, 1.5],
                 showticklabels=False,
                 tickvals=[-0.5],
                 ticklen=50,
                 tickcolor="#000000",
@@ -846,28 +919,29 @@
                 col=1,
             )
             self._figure.update_xaxes(title=dict(text="Time(ns)", standoff=5, font=dict(size=9)), row=r, col=1)
             title_text = ""
 
         return
 
-    def build(self):
+    def build(self) -> None:
         self._pre_setup()
         self._setup_figure()
         self._add_data()
         self._update_extra_features()
         return
 
-    def plot(self):
+    def plot(self) -> None:
         if self._figure is None:
             raise RuntimeError("No graph has been built. Use 'build' on the instance to first build the figure.")
         self._figure.show()
         return
 
-    def save(self, basedir="", filename=""):
+    def save(self, basedir: str = "", filename: str = "") -> None:
+        assert isinstance(self._figure, go.Figure)
         if not os.path.exists(basedir):
             os.makedirs(basedir)
         if filename == "":
             filename = f"waveform_report_{self._job_id}"
         if not os.path.splitext(filename)[1] == "html":
             filename += ".html"
```

### Comparing `qm_qua-1.1.1/PKG-INFO` & `qm_qua-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: qm-qua
-Version: 1.1.1
+Version: 1.1.2
 Summary: QUA language SDK to control a Quantum Computer
 Author: Quantum Machines
 Author-email: info@quantum-machines.co
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: simulation
 Requires-Dist: betterproto (==2.0.0b5)
 Requires-Dist: certifi ; extra == "simulation"
 Requires-Dist: datadog-api-client (>=2.6.0,<3.0.0)
 Requires-Dist: dependency_injector (>=4.41.0,<5.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: grpcio (>=1.39.0,<2.0.0)
 Requires-Dist: grpclib (>=0.4.3rc3,<0.5.0) ; python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: httpx[http2] (>=0.23.3,<0.24.0)
 Requires-Dist: marshmallow (>=3.0.0,<4.0.0)
 Requires-Dist: marshmallow-polyfield (>=5.7,<6.0)
 Requires-Dist: numpy (>=1.17.0,<2.0.0)
 Requires-Dist: plotly (>=5.13.0,<6.0.0)
-Requires-Dist: pretty_errors (>=1.2.25,<2.0.0)
 Requires-Dist: protobuf (>=3.17.3,<4.0.0)
 Requires-Dist: qm-octave (>=1.1.0,<2.0.0)
 Requires-Dist: tinydb (>=4.6.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 
 # QM-QUA SDK
```

