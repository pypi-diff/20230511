# Comparing `tmp/laboneq-2.5.0-py3-none-any.whl.zip` & `tmp/laboneq-2.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,90 +1,86 @@
-Zip file size: 955846 bytes, number of entries: 248
--rw-rw-rw-  2.0 unx        5 b- defN 23-Apr-27 08:13 laboneq/VERSION.txt
+Zip file size: 932038 bytes, number of entries: 246
+-rw-rw-rw-  2.0 unx        5 b- defN 23-May-11 13:50 laboneq/VERSION.txt
 -rw-r--r--  2.0 unx      306 b- defN 23-Feb-02 07:13 laboneq/__init__.py
 -rw-r--r--  2.0 unx     2829 b- defN 23-Feb-02 07:13 laboneq/_token.py
+-rw-r--r--  2.0 unx      928 b- defN 23-May-10 12:50 laboneq/_utils.py
 -rw-r--r--  2.0 unx      238 b- defN 23-Feb-02 07:13 laboneq/_version.py
--rw-r--r--  2.0 unx     1411 b- defN 23-Apr-27 08:13 laboneq/simple.py
+-rw-r--r--  2.0 unx     1525 b- defN 23-May-11 13:51 laboneq/simple.py
 -rw-r--r--  2.0 unx      184 b- defN 23-Feb-02 07:13 laboneq/_observability/__init__.py
 -rw-r--r--  2.0 unx      538 b- defN 23-Feb-02 07:13 laboneq/_observability/tracing/__init__.py
 -rw-r--r--  2.0 unx      893 b- defN 23-Feb-16 12:45 laboneq/_observability/tracing/_noop_tracer.py
 -rw-r--r--  2.0 unx     2309 b- defN 23-Feb-16 12:45 laboneq/_observability/tracing/_tracer.py
 -rw-r--r--  2.0 unx      444 b- defN 23-Feb-02 07:13 laboneq/compiler/__init__.py
 -rw-r--r--  2.0 unx      204 b- defN 23-Feb-02 07:13 laboneq/compiler/fastlogging.py
--rw-rw-rw-  2.0 unx    22524 b- defN 23-Apr-25 11:23 laboneq/compiler/qccs-schema_2_5_0.json
+-rw-rw-rw-  2.0 unx    22524 b- defN 23-Apr-28 11:39 laboneq/compiler/qccs-schema_2_5_0.json
 -rw-r--r--  2.0 unx      666 b- defN 23-Feb-02 07:13 laboneq/compiler/remote.py
 -rw-r--r--  2.0 unx      654 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/__init__.py
 -rw-r--r--  2.0 unx    18645 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/analyze_events.py
--rw-r--r--  2.0 unx    28581 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/analyze_playback.py
--rw-r--r--  2.0 unx    64112 b- defN 23-Apr-25 11:23 laboneq/compiler/code_generator/code_generator.py
+-rw-r--r--  2.0 unx    26665 b- defN 23-May-10 12:50 laboneq/compiler/code_generator/analyze_playback.py
+-rw-r--r--  2.0 unx    71375 b- defN 23-May-11 07:18 laboneq/compiler/code_generator/code_generator.py
 -rw-r--r--  2.0 unx     4026 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/command_table_tracker.py
--rw-r--r--  2.0 unx     2880 b- defN 23-Apr-25 11:23 laboneq/compiler/code_generator/compressor.py
+-rw-r--r--  2.0 unx     2880 b- defN 23-Apr-28 11:39 laboneq/compiler/code_generator/compressor.py
 -rw-r--r--  2.0 unx     1414 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/feedback_register_allocator.py
 -rw-r--r--  2.0 unx    10355 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/interval_calculator.py
--rw-r--r--  2.0 unx    18617 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/measurement_calculator.py
--rw-r--r--  2.0 unx    29598 b- defN 23-Apr-25 11:23 laboneq/compiler/code_generator/sampled_event_handler.py
--rw-r--r--  2.0 unx    18188 b- defN 23-Apr-25 11:23 laboneq/compiler/code_generator/seq_c_generator.py
--rw-r--r--  2.0 unx     6129 b- defN 23-Apr-25 11:23 laboneq/compiler/code_generator/seqc_tracker.py
+-rw-r--r--  2.0 unx    17825 b- defN 23-May-09 12:30 laboneq/compiler/code_generator/measurement_calculator.py
+-rw-r--r--  2.0 unx    30333 b- defN 23-May-10 12:50 laboneq/compiler/code_generator/sampled_event_handler.py
+-rw-r--r--  2.0 unx    19239 b- defN 23-May-10 12:50 laboneq/compiler/code_generator/seq_c_generator.py
+-rw-r--r--  2.0 unx     6333 b- defN 23-May-10 12:50 laboneq/compiler/code_generator/seqc_tracker.py
 -rw-r--r--  2.0 unx     7741 b- defN 23-Apr-06 14:15 laboneq/compiler/code_generator/signatures.py
 -rw-r--r--  2.0 unx     3500 b- defN 23-Feb-28 13:10 laboneq/compiler/code_generator/utils.py
+-rw-r--r--  2.0 unx     3737 b- defN 23-May-10 12:50 laboneq/compiler/code_generator/wave_compressor.py
 -rw-r--r--  2.0 unx     1476 b- defN 23-Feb-28 13:10 laboneq/compiler/code_generator/wave_index_tracker.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/compiler/common/__init__.py
 -rw-r--r--  2.0 unx     1093 b- defN 23-Apr-06 14:15 laboneq/compiler/common/awg_info.py
--rw-r--r--  2.0 unx     1903 b- defN 23-Apr-06 14:15 laboneq/compiler/common/awg_sampled_event.py
+-rw-r--r--  2.0 unx     1926 b- defN 23-May-10 12:50 laboneq/compiler/common/awg_sampled_event.py
 -rw-r--r--  2.0 unx      480 b- defN 23-Feb-02 07:13 laboneq/compiler/common/awg_signal_type.py
--rw-r--r--  2.0 unx     3983 b- defN 23-Apr-06 14:15 laboneq/compiler/common/compiler_settings.py
--rw-r--r--  2.0 unx     4708 b- defN 23-Apr-25 11:23 laboneq/compiler/common/device_type.py
--rw-r--r--  2.0 unx     1532 b- defN 23-Feb-15 13:56 laboneq/compiler/common/event_type.py
+-rw-r--r--  2.0 unx     4015 b- defN 23-May-10 12:50 laboneq/compiler/common/compiler_settings.py
+-rw-r--r--  2.0 unx     6058 b- defN 23-May-05 14:53 laboneq/compiler/common/device_type.py
+-rw-r--r--  2.0 unx     1532 b- defN 23-May-11 07:18 laboneq/compiler/common/event_type.py
 -rw-r--r--  2.0 unx      229 b- defN 23-Mar-07 13:19 laboneq/compiler/common/play_wave_type.py
 -rw-r--r--  2.0 unx      580 b- defN 23-Apr-06 14:15 laboneq/compiler/common/pulse_parameters.py
--rw-r--r--  2.0 unx     2594 b- defN 23-Apr-25 11:23 laboneq/compiler/common/signal_obj.py
+-rw-r--r--  2.0 unx     2594 b- defN 23-Apr-28 11:39 laboneq/compiler/common/signal_obj.py
 -rw-r--r--  2.0 unx      400 b- defN 23-Feb-02 07:13 laboneq/compiler/common/trigger_mode.py
 -rw-r--r--  2.0 unx      154 b- defN 23-Feb-02 07:13 laboneq/compiler/experiment_access/__init__.py
 -rw-r--r--  2.0 unx      222 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/acquire_info.py
--rw-r--r--  2.0 unx      602 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/cache.py
--rw-r--r--  2.0 unx      349 b- defN 23-Apr-25 11:23 laboneq/compiler/experiment_access/device_info.py
--rw-r--r--  2.0 unx    44686 b- defN 23-Apr-25 11:23 laboneq/compiler/experiment_access/dsl_loader.py
--rw-r--r--  2.0 unx    16529 b- defN 23-Apr-25 11:23 laboneq/compiler/experiment_access/experiment_dao.py
--rw-r--r--  2.0 unx    14106 b- defN 23-Apr-25 11:23 laboneq/compiler/experiment_access/json_dumper.py
--rw-r--r--  2.0 unx    21004 b- defN 23-Apr-25 11:23 laboneq/compiler/experiment_access/json_loader.py
--rw-r--r--  2.0 unx     6182 b- defN 23-Apr-25 11:23 laboneq/compiler/experiment_access/loader_base.py
+-rw-r--r--  2.0 unx      349 b- defN 23-Apr-28 11:39 laboneq/compiler/experiment_access/device_info.py
+-rw-r--r--  2.0 unx    44928 b- defN 23-May-11 07:18 laboneq/compiler/experiment_access/dsl_loader.py
+-rw-r--r--  2.0 unx    16509 b- defN 23-May-11 07:18 laboneq/compiler/experiment_access/experiment_dao.py
+-rw-r--r--  2.0 unx    14106 b- defN 23-May-11 07:18 laboneq/compiler/experiment_access/json_dumper.py
+-rw-r--r--  2.0 unx    21004 b- defN 23-May-11 07:18 laboneq/compiler/experiment_access/json_loader.py
+-rw-r--r--  2.0 unx     6182 b- defN 23-Apr-28 11:39 laboneq/compiler/experiment_access/loader_base.py
 -rw-r--r--  2.0 unx      270 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/marker.py
--rw-r--r--  2.0 unx      286 b- defN 23-Apr-25 11:23 laboneq/compiler/experiment_access/oscillator_info.py
+-rw-r--r--  2.0 unx      286 b- defN 23-Apr-28 11:39 laboneq/compiler/experiment_access/oscillator_info.py
 -rw-r--r--  2.0 unx      197 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/param_ref.py
--rw-r--r--  2.0 unx     1263 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/pulse_def.py
--rw-r--r--  2.0 unx    21550 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/section_graph.py
+-rw-r--r--  2.0 unx     1311 b- defN 23-May-10 12:50 laboneq/compiler/experiment_access/pulse_def.py
 -rw-r--r--  2.0 unx      851 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/section_info.py
 -rw-r--r--  2.0 unx     1069 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/section_signal_pulse.py
 -rw-r--r--  2.0 unx      387 b- defN 23-Apr-06 14:15 laboneq/compiler/experiment_access/signal_info.py
--rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 14:57 laboneq/compiler/new_scheduler/__init__.py
--rw-r--r--  2.0 unx     3269 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/case_schedule.py
--rw-r--r--  2.0 unx     7443 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/interval_schedule.py
--rw-r--r--  2.0 unx     3331 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/loop_iteration_schedule.py
--rw-r--r--  2.0 unx     8588 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/loop_schedule.py
--rw-r--r--  2.0 unx     8075 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/match_schedule.py
--rw-r--r--  2.0 unx     2252 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/oscillator_schedule.py
--rw-r--r--  2.0 unx     1765 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/phase_reset_schedule.py
--rw-r--r--  2.0 unx     1820 b- defN 23-Apr-06 14:15 laboneq/compiler/new_scheduler/preorder_map.py
--rw-r--r--  2.0 unx     3821 b- defN 23-Apr-06 14:15 laboneq/compiler/new_scheduler/pulse_phase.py
--rw-r--r--  2.0 unx     6962 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/pulse_schedule.py
--rw-r--r--  2.0 unx      625 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/reserve_schedule.py
--rw-r--r--  2.0 unx     1375 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/root_schedule.py
--rw-r--r--  2.0 unx     1016 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/schedule_data.py
--rw-r--r--  2.0 unx    40991 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/scheduler.py
--rw-r--r--  2.0 unx    13207 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/section_schedule.py
--rw-r--r--  2.0 unx      757 b- defN 23-Apr-25 11:23 laboneq/compiler/new_scheduler/utils.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/compiler/scheduler/__init__.py
--rw-r--r--  2.0 unx    12943 b- defN 23-Apr-06 14:15 laboneq/compiler/scheduler/event_graph.py
--rw-r--r--  2.0 unx    24682 b- defN 23-Feb-02 07:13 laboneq/compiler/scheduler/event_graph_builder.py
+-rw-r--r--  2.0 unx     3265 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/case_schedule.py
+-rw-r--r--  2.0 unx     7439 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/interval_schedule.py
+-rw-r--r--  2.0 unx     3327 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/loop_iteration_schedule.py
+-rw-r--r--  2.0 unx     8576 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/loop_schedule.py
+-rw-r--r--  2.0 unx     9267 b- defN 23-May-11 07:18 laboneq/compiler/scheduler/match_schedule.py
+-rw-r--r--  2.0 unx     2248 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/oscillator_schedule.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/phase_reset_schedule.py
+-rw-r--r--  2.0 unx     1808 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/preorder_map.py
+-rw-r--r--  2.0 unx     3821 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/pulse_phase.py
+-rw-r--r--  2.0 unx     6958 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/pulse_schedule.py
+-rw-r--r--  2.0 unx      621 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/reserve_schedule.py
+-rw-r--r--  2.0 unx     1367 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/root_schedule.py
 -rw-r--r--  2.0 unx     1949 b- defN 23-Feb-09 09:31 laboneq/compiler/scheduler/sampling_rate_tracker.py
--rw-r--r--  2.0 unx   115572 b- defN 23-Apr-25 11:23 laboneq/compiler/scheduler/scheduler.py
+-rw-r--r--  2.0 unx     1012 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/schedule_data.py
+-rw-r--r--  2.0 unx    40949 b- defN 23-May-10 12:50 laboneq/compiler/scheduler/scheduler.py
+-rw-r--r--  2.0 unx    13191 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/section_schedule.py
+-rw-r--r--  2.0 unx      757 b- defN 23-May-04 12:22 laboneq/compiler/scheduler/utils.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/compiler/workflow/__init__.py
--rw-r--r--  2.0 unx    49793 b- defN 23-Apr-25 11:23 laboneq/compiler/workflow/compiler.py
+-rw-r--r--  2.0 unx    50498 b- defN 23-May-11 07:18 laboneq/compiler/workflow/compiler.py
 -rw-r--r--  2.0 unx    12424 b- defN 23-Feb-28 13:10 laboneq/compiler/workflow/precompensation_helpers.py
--rw-r--r--  2.0 unx    12229 b- defN 23-Apr-25 11:23 laboneq/compiler/workflow/recipe_generator.py
+-rw-r--r--  2.0 unx    12420 b- defN 23-May-09 12:30 laboneq/compiler/workflow/recipe_generator.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/__init__.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/__init__.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/inspector/__init__.py
 -rw-r--r--  2.0 unx     4511 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/inspector/update_inspect.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/plotter/__init__.py
 -rw-r--r--  2.0 unx     3379 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/plotter/plot_funs.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/bloch_simulator_pulse_plotter/pulse_simulator/__init__.py
@@ -95,156 +91,158 @@
 -rw-r--r--  2.0 unx     3581 b- defN 23-Apr-06 14:15 laboneq/contrib/example_helpers/qubit_helper.py
 -rw-r--r--  2.0 unx     8830 b- defN 23-Apr-06 14:15 laboneq/contrib/example_helpers/randomized_benchmarking_helper.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/example_helpers/data_analysis/__init__.py
 -rw-r--r--  2.0 unx     6670 b- defN 23-Apr-06 14:15 laboneq/contrib/example_helpers/data_analysis/data_analysis.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/example_helpers/descriptors/__init__.py
 -rw-r--r--  2.0 unx      502 b- defN 23-Apr-06 14:15 laboneq/contrib/example_helpers/descriptors/hdawg.py
 -rw-r--r--  2.0 unx      956 b- defN 23-Apr-06 14:15 laboneq/contrib/example_helpers/descriptors/hdawg_uhfqa_pqsc.py
--rw-r--r--  2.0 unx     1345 b- defN 23-Apr-26 08:59 laboneq/contrib/example_helpers/descriptors/shfqc.py
--rw-r--r--  2.0 unx     1377 b- defN 23-Apr-26 08:59 laboneq/contrib/example_helpers/descriptors/shfsg.py
--rw-r--r--  2.0 unx     1930 b- defN 23-Apr-26 08:59 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_hdawg_pqsc.py
--rw-r--r--  2.0 unx     1618 b- defN 23-Apr-26 08:59 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_pqsc.py
--rw-r--r--  2.0 unx     2383 b- defN 23-Apr-26 08:59 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_shfqc_hdawg_pqsc.py
+-rw-r--r--  2.0 unx     1887 b- defN 23-May-04 12:22 laboneq/contrib/example_helpers/descriptors/shfqc.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-May-04 12:22 laboneq/contrib/example_helpers/descriptors/shfsg.py
+-rw-r--r--  2.0 unx     2472 b- defN 23-May-04 12:22 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_hdawg_pqsc.py
+-rw-r--r--  2.0 unx     2160 b- defN 23-May-04 12:22 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_pqsc.py
+-rw-r--r--  2.0 unx     2708 b- defN 23-May-04 12:22 laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_shfqc_hdawg_pqsc.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Apr-06 14:15 laboneq/contrib/example_helpers/plotting/__init__.py
--rw-r--r--  2.0 unx     6620 b- defN 23-Apr-27 08:13 laboneq/contrib/example_helpers/plotting/plot_helpers.py
+-rw-r--r--  2.0 unx    10340 b- defN 23-May-10 12:50 laboneq/contrib/example_helpers/plotting/plot_helpers.py
 -rw-r--r--  2.0 unx      308 b- defN 23-Feb-13 10:57 laboneq/controller/__init__.py
 -rw-r--r--  2.0 unx     1479 b- defN 23-Feb-02 07:13 laboneq/controller/cache.py
--rw-r--r--  2.0 unx    13536 b- defN 23-Apr-25 11:23 laboneq/controller/communication.py
--rw-r--r--  2.0 unx    32890 b- defN 23-Apr-25 11:23 laboneq/controller/controller.py
--rw-r--r--  2.0 unx     4504 b- defN 23-Apr-06 14:15 laboneq/controller/laboneq_logging.py
+-rw-r--r--  2.0 unx    13604 b- defN 23-May-10 12:50 laboneq/controller/communication.py
+-rw-r--r--  2.0 unx    34132 b- defN 23-May-11 07:18 laboneq/controller/controller.py
+-rw-r--r--  2.0 unx     4600 b- defN 23-May-05 14:53 laboneq/controller/laboneq_logging.py
 -rw-r--r--  2.0 unx      337 b- defN 23-Feb-02 07:13 laboneq/controller/protected_session.py
--rw-r--r--  2.0 unx    15011 b- defN 23-Apr-25 11:23 laboneq/controller/recipe_1_4_0.py
+-rw-r--r--  2.0 unx    15088 b- defN 23-May-11 07:18 laboneq/controller/recipe_1_4_0.py
 -rw-r--r--  2.0 unx      638 b- defN 23-Feb-02 07:13 laboneq/controller/recipe_enums.py
--rw-r--r--  2.0 unx    19876 b- defN 23-Apr-25 11:23 laboneq/controller/recipe_processor.py
+-rw-r--r--  2.0 unx    19876 b- defN 23-May-11 07:18 laboneq/controller/recipe_processor.py
 -rw-r--r--  2.0 unx     1917 b- defN 23-Feb-02 07:13 laboneq/controller/results.py
 -rw-r--r--  2.0 unx     1594 b- defN 23-Feb-13 10:57 laboneq/controller/toolkit_adapter.py
--rw-r--r--  2.0 unx      624 b- defN 23-Apr-06 14:15 laboneq/controller/util.py
+-rw-r--r--  2.0 unx     1178 b- defN 23-May-09 12:30 laboneq/controller/util.py
 -rw-r--r--  2.0 unx      281 b- defN 23-Mar-07 07:28 laboneq/controller/versioning.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/controller/devices/__init__.py
--rw-r--r--  2.0 unx    15400 b- defN 23-Apr-26 08:59 laboneq/controller/devices/device_collection.py
--rw-r--r--  2.0 unx     1275 b- defN 23-Apr-25 11:23 laboneq/controller/devices/device_factory.py
--rw-r--r--  2.0 unx    23542 b- defN 23-Apr-26 08:59 laboneq/controller/devices/device_hdawg.py
--rw-r--r--  2.0 unx      491 b- defN 23-Apr-25 11:23 laboneq/controller/devices/device_nonqc.py
--rw-r--r--  2.0 unx     8115 b- defN 23-Apr-26 08:59 laboneq/controller/devices/device_pqsc.py
--rw-r--r--  2.0 unx     4137 b- defN 23-Apr-26 08:59 laboneq/controller/devices/device_setup_dao.py
--rw-r--r--  2.0 unx     3758 b- defN 23-Apr-25 11:23 laboneq/controller/devices/device_shfppc.py
--rw-r--r--  2.0 unx    40101 b- defN 23-Apr-26 08:59 laboneq/controller/devices/device_shfqa.py
--rw-r--r--  2.0 unx    20509 b- defN 23-Apr-26 08:59 laboneq/controller/devices/device_shfsg.py
--rw-r--r--  2.0 unx    28521 b- defN 23-Apr-26 08:59 laboneq/controller/devices/device_uhfqa.py
--rw-r--r--  2.0 unx    36707 b- defN 23-Apr-26 08:59 laboneq/controller/devices/device_zi.py
--rw-r--r--  2.0 unx    29590 b- defN 23-Apr-25 11:23 laboneq/controller/devices/zi_emulator.py
--rw-r--r--  2.0 unx    10358 b- defN 23-Apr-26 08:59 laboneq/controller/devices/zi_node_monitor.py
+-rw-r--r--  2.0 unx    15400 b- defN 23-Apr-28 11:39 laboneq/controller/devices/device_collection.py
+-rw-r--r--  2.0 unx     1275 b- defN 23-Apr-28 11:39 laboneq/controller/devices/device_factory.py
+-rw-r--r--  2.0 unx    23794 b- defN 23-May-11 07:18 laboneq/controller/devices/device_hdawg.py
+-rw-r--r--  2.0 unx      491 b- defN 23-Apr-28 11:39 laboneq/controller/devices/device_nonqc.py
+-rw-r--r--  2.0 unx     8115 b- defN 23-Apr-28 11:39 laboneq/controller/devices/device_pqsc.py
+-rw-r--r--  2.0 unx     4137 b- defN 23-Apr-28 11:39 laboneq/controller/devices/device_setup_dao.py
+-rw-r--r--  2.0 unx     4013 b- defN 23-May-11 07:18 laboneq/controller/devices/device_shfppc.py
+-rw-r--r--  2.0 unx    40727 b- defN 23-May-11 07:18 laboneq/controller/devices/device_shfqa.py
+-rw-r--r--  2.0 unx    20509 b- defN 23-May-11 07:18 laboneq/controller/devices/device_shfsg.py
+-rw-r--r--  2.0 unx    28857 b- defN 23-May-11 07:18 laboneq/controller/devices/device_uhfqa.py
+-rw-r--r--  2.0 unx    36238 b- defN 23-May-11 07:18 laboneq/controller/devices/device_zi.py
+-rw-r--r--  2.0 unx    29590 b- defN 23-Apr-28 11:39 laboneq/controller/devices/zi_emulator.py
+-rw-r--r--  2.0 unx    10358 b- defN 23-Apr-28 11:39 laboneq/controller/devices/zi_node_monitor.py
 -rw-r--r--  2.0 unx       97 b- defN 23-Feb-02 07:13 laboneq/core/__init__.py
--rw-r--r--  2.0 unx     2015 b- defN 23-Apr-26 08:59 laboneq/core/path.py
+-rw-r--r--  2.0 unx     2015 b- defN 23-Apr-28 11:39 laboneq/core/path.py
 -rw-r--r--  2.0 unx     1338 b- defN 23-Feb-02 07:13 laboneq/core/validators.py
 -rw-r--r--  2.0 unx      126 b- defN 23-Feb-02 07:13 laboneq/core/exceptions/__init__.py
 -rw-r--r--  2.0 unx      123 b- defN 23-Feb-02 07:13 laboneq/core/exceptions/laboneq_exception.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/core/serialization/__init__.py
--rw-r--r--  2.0 unx    19090 b- defN 23-Apr-06 14:15 laboneq/core/serialization/simple_serialization.py
+-rw-r--r--  2.0 unx    19090 b- defN 23-May-09 12:50 laboneq/core/serialization/simple_serialization.py
 -rw-r--r--  2.0 unx      161 b- defN 23-Feb-02 07:13 laboneq/core/types/__init__.py
--rw-r--r--  2.0 unx     5138 b- defN 23-Feb-28 13:10 laboneq/core/types/compiled_experiment.py
+-rw-r--r--  2.0 unx     5169 b- defN 23-May-10 12:50 laboneq/core/types/compiled_experiment.py
 -rw-r--r--  2.0 unx     1473 b- defN 23-Feb-02 07:13 laboneq/core/types/uid.py
 -rw-r--r--  2.0 unx      660 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/__init__.py
 -rw-r--r--  2.0 unx      934 b- defN 23-Feb-07 16:25 laboneq/core/types/enums/acquisition_type.py
 -rw-r--r--  2.0 unx      213 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/averaging_mode.py
 -rw-r--r--  2.0 unx      188 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/carrier_type.py
 -rw-r--r--  2.0 unx      227 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/dsl_version.py
 -rw-r--r--  2.0 unx      185 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/execution_type.py
 -rw-r--r--  2.0 unx      223 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/high_pass_compensation_clearing.py
 -rw-r--r--  2.0 unx      157 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/io_direction.py
--rw-r--r--  2.0 unx      268 b- defN 23-Apr-25 11:23 laboneq/core/types/enums/io_signal_type.py
+-rw-r--r--  2.0 unx      268 b- defN 23-Apr-28 11:39 laboneq/core/types/enums/io_signal_type.py
 -rw-r--r--  2.0 unx      316 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/mixer_type.py
 -rw-r--r--  2.0 unx      200 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/modulation_type.py
 -rw-r--r--  2.0 unx      152 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/port_mode.py
 -rw-r--r--  2.0 unx      188 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/reference_clock_source.py
 -rw-r--r--  2.0 unx      198 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/repetition_mode.py
 -rw-r--r--  2.0 unx      170 b- defN 23-Feb-02 07:13 laboneq/core/types/enums/section_alignment.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/core/utilities/__init__.py
 -rw-r--r--  2.0 unx     8039 b- defN 23-Apr-06 14:15 laboneq/core/utilities/pulse_sampler.py
 -rw-r--r--  2.0 unx     9808 b- defN 23-Apr-06 14:15 laboneq/core/utilities/replace_pulse.py
--rw-r--r--  2.0 unx      178 b- defN 23-Feb-02 07:13 laboneq/dsl/__init__.py
--rw-r--r--  2.0 unx     2929 b- defN 23-Apr-25 11:23 laboneq/dsl/laboneq_facade.py
+-rw-r--r--  2.0 unx      178 b- defN 23-May-03 09:34 laboneq/dsl/__init__.py
+-rw-r--r--  2.0 unx     2929 b- defN 23-Apr-28 11:39 laboneq/dsl/laboneq_facade.py
 -rw-r--r--  2.0 unx     2552 b- defN 23-Feb-15 13:56 laboneq/dsl/parameter.py
--rw-r--r--  2.0 unx    25670 b- defN 23-Apr-25 11:23 laboneq/dsl/session.py
+-rw-r--r--  2.0 unx    25670 b- defN 23-Apr-28 11:39 laboneq/dsl/session.py
 -rw-r--r--  2.0 unx     2296 b- defN 23-Feb-02 07:13 laboneq/dsl/utils.py
--rw-r--r--  2.0 unx      529 b- defN 23-Apr-25 11:23 laboneq/dsl/calibration/__init__.py
--rw-r--r--  2.0 unx     1017 b- defN 23-Apr-25 11:23 laboneq/dsl/calibration/amplifier_pump.py
+-rw-r--r--  2.0 unx      529 b- defN 23-Apr-28 11:39 laboneq/dsl/calibration/__init__.py
+-rw-r--r--  2.0 unx     1017 b- defN 23-May-11 07:18 laboneq/dsl/calibration/amplifier_pump.py
 -rw-r--r--  2.0 unx      545 b- defN 23-Feb-02 07:13 laboneq/dsl/calibration/calibratable.py
--rw-r--r--  2.0 unx     1886 b- defN 23-Apr-25 16:53 laboneq/dsl/calibration/calibration.py
+-rw-r--r--  2.0 unx     2313 b- defN 23-May-04 12:22 laboneq/dsl/calibration/calibration.py
 -rw-r--r--  2.0 unx      111 b- defN 23-Feb-02 07:13 laboneq/dsl/calibration/calibration_item.py
 -rw-r--r--  2.0 unx      992 b- defN 23-Feb-27 16:33 laboneq/dsl/calibration/mixer_calibration.py
 -rw-r--r--  2.0 unx     3403 b- defN 23-Feb-02 07:13 laboneq/dsl/calibration/observable.py
--rw-r--r--  2.0 unx     1716 b- defN 23-Feb-27 16:33 laboneq/dsl/calibration/oscillator.py
+-rw-r--r--  2.0 unx     1716 b- defN 23-May-11 07:18 laboneq/dsl/calibration/oscillator.py
 -rw-r--r--  2.0 unx     2650 b- defN 23-Feb-27 16:33 laboneq/dsl/calibration/precompensation.py
--rw-r--r--  2.0 unx     5607 b- defN 23-Apr-25 11:23 laboneq/dsl/calibration/signal_calibration.py
+-rw-r--r--  2.0 unx     5607 b- defN 23-May-11 07:18 laboneq/dsl/calibration/signal_calibration.py
 -rw-r--r--  2.0 unx      553 b- defN 23-Feb-02 07:13 laboneq/dsl/calibration/units.py
 -rw-r--r--  2.0 unx      363 b- defN 23-Feb-02 07:13 laboneq/dsl/device/__init__.py
--rw-r--r--  2.0 unx    45826 b- defN 23-Apr-25 11:23 laboneq/dsl/device/_device_setup_generator.py
+-rw-r--r--  2.0 unx    45826 b- defN 23-Apr-28 11:39 laboneq/dsl/device/_device_setup_generator.py
 -rw-r--r--  2.0 unx      601 b- defN 23-Feb-02 07:13 laboneq/dsl/device/connection.py
--rw-r--r--  2.0 unx    13663 b- defN 23-Apr-26 08:59 laboneq/dsl/device/device_setup.py
+-rw-r--r--  2.0 unx    13663 b- defN 23-May-09 12:50 laboneq/dsl/device/device_setup.py
 -rw-r--r--  2.0 unx     2551 b- defN 23-Apr-06 14:15 laboneq/dsl/device/device_setup_helper.py
--rw-r--r--  2.0 unx     1362 b- defN 23-Apr-26 08:59 laboneq/dsl/device/instrument.py
+-rw-r--r--  2.0 unx     1362 b- defN 23-Apr-28 11:39 laboneq/dsl/device/instrument.py
 -rw-r--r--  2.0 unx     1893 b- defN 23-Feb-02 07:13 laboneq/dsl/device/logical_signal_group.py
 -rw-r--r--  2.0 unx     1729 b- defN 23-Feb-02 07:13 laboneq/dsl/device/physical_channel_group.py
 -rw-r--r--  2.0 unx      538 b- defN 23-Feb-02 07:13 laboneq/dsl/device/ports.py
--rw-r--r--  2.0 unx     4453 b- defN 23-Apr-27 08:13 laboneq/dsl/device/qubits.py
+-rw-r--r--  2.0 unx     4557 b- defN 23-May-10 12:50 laboneq/dsl/device/qubits.py
+-rw-r--r--  2.0 unx     3104 b- defN 23-May-11 13:51 laboneq/dsl/device/quops.py
 -rw-r--r--  2.0 unx      215 b- defN 23-Feb-02 07:13 laboneq/dsl/device/server.py
--rw-r--r--  2.0 unx      328 b- defN 23-Apr-25 11:23 laboneq/dsl/device/instruments/__init__.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Apr-28 11:39 laboneq/dsl/device/instruments/__init__.py
 -rw-r--r--  2.0 unx     1778 b- defN 23-Feb-02 07:13 laboneq/dsl/device/instruments/hdawg.py
 -rw-r--r--  2.0 unx      466 b- defN 23-Feb-13 10:57 laboneq/dsl/device/instruments/nonqc.py
 -rw-r--r--  2.0 unx      948 b- defN 23-Feb-02 07:13 laboneq/dsl/device/instruments/pqsc.py
--rw-r--r--  2.0 unx      927 b- defN 23-Apr-25 11:23 laboneq/dsl/device/instruments/shfppc.py
+-rw-r--r--  2.0 unx      927 b- defN 23-Apr-28 11:39 laboneq/dsl/device/instruments/shfppc.py
 -rw-r--r--  2.0 unx     2248 b- defN 23-Feb-06 17:42 laboneq/dsl/device/instruments/shfqa.py
 -rw-r--r--  2.0 unx     1659 b- defN 23-Feb-06 17:42 laboneq/dsl/device/instruments/shfsg.py
 -rw-r--r--  2.0 unx     2312 b- defN 23-Feb-16 12:45 laboneq/dsl/device/instruments/uhfqa.py
 -rw-r--r--  2.0 unx      888 b- defN 23-Feb-13 10:57 laboneq/dsl/device/instruments/zi_standard_instrument.py
 -rw-r--r--  2.0 unx      187 b- defN 23-Feb-02 07:13 laboneq/dsl/device/io_units/__init__.py
--rw-r--r--  2.0 unx    12750 b- defN 23-Apr-25 11:23 laboneq/dsl/device/io_units/logical_signal.py
--rw-r--r--  2.0 unx     3811 b- defN 23-Apr-26 08:59 laboneq/dsl/device/io_units/physical_channel.py
+-rw-r--r--  2.0 unx    12750 b- defN 23-May-03 09:34 laboneq/dsl/device/io_units/logical_signal.py
+-rw-r--r--  2.0 unx     3811 b- defN 23-May-03 09:34 laboneq/dsl/device/io_units/physical_channel.py
 -rw-r--r--  2.0 unx      114 b- defN 23-Feb-02 07:13 laboneq/dsl/device/servers/__init__.py
 -rw-r--r--  2.0 unx      704 b- defN 23-Feb-02 07:13 laboneq/dsl/device/servers/data_server.py
 -rw-r--r--  2.0 unx      718 b- defN 23-Feb-02 07:13 laboneq/dsl/enums/__init__.py
 -rw-r--r--  2.0 unx      508 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/__init__.py
 -rw-r--r--  2.0 unx      972 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/acquire.py
 -rw-r--r--  2.0 unx      814 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/call.py
 -rw-r--r--  2.0 unx      780 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/delay.py
--rw-r--r--  2.0 unx    39779 b- defN 23-Apr-25 11:23 laboneq/dsl/experiment/experiment.py
--rw-r--r--  2.0 unx     8216 b- defN 23-Apr-25 11:23 laboneq/dsl/experiment/experiment_signal.py
+-rw-r--r--  2.0 unx    39779 b- defN 23-May-11 07:18 laboneq/dsl/experiment/experiment.py
+-rw-r--r--  2.0 unx     8216 b- defN 23-Apr-28 11:39 laboneq/dsl/experiment/experiment_signal.py
 -rw-r--r--  2.0 unx      401 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/operation.py
 -rw-r--r--  2.0 unx     1647 b- defN 23-Feb-28 13:10 laboneq/dsl/experiment/play_pulse.py
--rw-r--r--  2.0 unx     3568 b- defN 23-Apr-03 11:23 laboneq/dsl/experiment/pulse.py
--rw-r--r--  2.0 unx     7932 b- defN 23-Mar-13 15:23 laboneq/dsl/experiment/pulse_library.py
+-rw-r--r--  2.0 unx     3953 b- defN 23-May-10 12:50 laboneq/dsl/experiment/pulse.py
+-rw-r--r--  2.0 unx     8194 b- defN 23-May-10 12:50 laboneq/dsl/experiment/pulse_library.py
 -rw-r--r--  2.0 unx      890 b- defN 23-Feb-16 12:45 laboneq/dsl/experiment/reserve.py
--rw-r--r--  2.0 unx    11431 b- defN 23-Apr-25 11:23 laboneq/dsl/experiment/section.py
+-rw-r--r--  2.0 unx    11431 b- defN 23-Apr-28 11:39 laboneq/dsl/experiment/section.py
 -rw-r--r--  2.0 unx      640 b- defN 23-Feb-02 07:13 laboneq/dsl/experiment/set.py
--rw-r--r--  2.0 unx      323 b- defN 23-Apr-25 11:23 laboneq/dsl/experiment/utils.py
+-rw-r--r--  2.0 unx      323 b- defN 23-Apr-28 11:39 laboneq/dsl/experiment/utils.py
 -rw-r--r--  2.0 unx      151 b- defN 23-Feb-14 15:16 laboneq/dsl/result/__init__.py
 -rw-r--r--  2.0 unx     1766 b- defN 23-Feb-02 07:13 laboneq/dsl/result/acquired_result.py
 -rw-r--r--  2.0 unx     7240 b- defN 23-Feb-02 07:13 laboneq/dsl/result/results.py
 -rw-r--r--  2.0 unx      113 b- defN 23-Feb-02 07:13 laboneq/dsl/serialization/__init__.py
--rw-r--r--  2.0 unx     5339 b- defN 23-Apr-27 08:13 laboneq/dsl/serialization/serializer.py
+-rw-r--r--  2.0 unx     5379 b- defN 23-May-11 13:51 laboneq/dsl/serialization/serializer.py
 -rw-r--r--  2.0 unx       77 b- defN 23-Feb-02 07:13 laboneq/executor/__init__.py
 -rw-r--r--  2.0 unx     3819 b- defN 23-Feb-16 12:45 laboneq/executor/execution_from_experiment.py
 -rw-r--r--  2.0 unx     8152 b- defN 23-Apr-06 14:15 laboneq/executor/executor.py
 -rw-r--r--  2.0 unx      145 b- defN 23-Feb-14 15:16 laboneq/openqasm3/__init__.py
--rw-r--r--  2.0 unx     2488 b- defN 23-Apr-27 08:13 laboneq/openqasm3/expression.py
--rw-r--r--  2.0 unx     1929 b- defN 23-Apr-27 08:13 laboneq/openqasm3/gate_store.py
--rw-r--r--  2.0 unx    10789 b- defN 23-Apr-27 08:13 laboneq/openqasm3/openqasm3_importer.py
--rw-r--r--  2.0 unx     1732 b- defN 23-Apr-25 11:23 laboneq/openqasm3/openqasm_error.py
--rw-r--r--  2.0 unx     5136 b- defN 23-Apr-27 08:13 laboneq/openqasm3/reset_gate_factory.py
--rw-r--r--  2.0 unx     3069 b- defN 23-Apr-27 08:13 laboneq/openqasm3/variable_store.py
+-rw-r--r--  2.0 unx     8730 b- defN 23-May-11 13:51 laboneq/openqasm3/expression.py
+-rw-r--r--  2.0 unx     1604 b- defN 23-May-11 13:51 laboneq/openqasm3/gate_store.py
+-rw-r--r--  2.0 unx     2060 b- defN 23-May-11 13:21 laboneq/openqasm3/namespace.py
+-rw-r--r--  2.0 unx    13702 b- defN 23-May-11 13:51 laboneq/openqasm3/openqasm3_importer.py
+-rw-r--r--  2.0 unx     1732 b- defN 23-Apr-28 11:39 laboneq/openqasm3/openqasm_error.py
+-rw-r--r--  2.0 unx     4850 b- defN 23-May-04 12:22 laboneq/openqasm3/reset_gate_factory.py
+-rw-r--r--  2.0 unx     1492 b- defN 23-May-11 13:21 laboneq/openqasm3/signal_store.py
 -rw-r--r--  2.0 unx      127 b- defN 23-Feb-02 07:13 laboneq/pulse_sheet_viewer/__init__.py
 -rw-r--r--  2.0 unx     2059 b- defN 23-Feb-16 12:45 laboneq/pulse_sheet_viewer/event_graph_viewer.py
 -rw-r--r--  2.0 unx     2692 b- defN 23-Feb-02 14:48 laboneq/pulse_sheet_viewer/interactive_psv.py
 -rw-r--r--  2.0 unx     3288 b- defN 23-Feb-02 14:48 laboneq/pulse_sheet_viewer/pulse_sheet_viewer.py
 -rw-rw-rw-  2.0 unx  1443040 b- defN 23-Apr-06 14:15 laboneq/pulse_sheet_viewer/pulse_sheet_viewer_template.html
 -rw-r--r--  2.0 unx      152 b- defN 23-Feb-14 15:16 laboneq/simulator/__init__.py
 -rw-r--r--  2.0 unx     5904 b- defN 23-Feb-02 14:48 laboneq/simulator/output_simulator.py
--rw-r--r--  2.0 unx    39230 b- defN 23-Apr-25 11:23 laboneq/simulator/seqc_parser.py
--rw-r--r--  2.0 unx    12081 b- defN 23-Apr-06 14:15 laboneq/simulator/wave_scroller.py
--rw-rw-rw-  2.0 unx       22 b- defN 23-Apr-27 08:14 laboneq-2.5.0.dist-info/AUTHORS
--rw-rw-rw-  2.0 unx    11358 b- defN 23-Apr-27 08:14 laboneq-2.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3188 b- defN 23-Apr-27 08:14 laboneq-2.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 08:14 laboneq-2.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-27 08:14 laboneq-2.5.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    24287 b- defN 23-Apr-27 08:14 laboneq-2.5.0.dist-info/RECORD
-248 files, 2988946 bytes uncompressed, 916406 bytes compressed:  69.4%
+-rw-r--r--  2.0 unx    40863 b- defN 23-May-10 12:50 laboneq/simulator/seqc_parser.py
+-rw-r--r--  2.0 unx    12500 b- defN 23-May-10 12:50 laboneq/simulator/wave_scroller.py
+-rw-rw-rw-  2.0 unx       22 b- defN 23-May-11 13:51 laboneq-2.6.0.dist-info/AUTHORS
+-rw-rw-rw-  2.0 unx    11358 b- defN 23-May-11 13:51 laboneq-2.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3188 b- defN 23-May-11 13:51 laboneq-2.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-11 13:51 laboneq-2.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-11 13:51 laboneq-2.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    23965 b- defN 23-May-11 13:51 laboneq-2.6.0.dist-info/RECORD
+246 files, 2852565 bytes uncompressed, 893164 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: laboneq/__init__.py
 Comment: 
 
 Filename: laboneq/_token.py
 Comment: 
 
+Filename: laboneq/_utils.py
+Comment: 
+
 Filename: laboneq/_version.py
 Comment: 
 
 Filename: laboneq/simple.py
 Comment: 
 
 Filename: laboneq/_observability/__init__.py
@@ -75,14 +78,17 @@
 
 Filename: laboneq/compiler/code_generator/signatures.py
 Comment: 
 
 Filename: laboneq/compiler/code_generator/utils.py
 Comment: 
 
+Filename: laboneq/compiler/code_generator/wave_compressor.py
+Comment: 
+
 Filename: laboneq/compiler/code_generator/wave_index_tracker.py
 Comment: 
 
 Filename: laboneq/compiler/common/__init__.py
 Comment: 
 
 Filename: laboneq/compiler/common/awg_info.py
@@ -117,17 +123,14 @@
 
 Filename: laboneq/compiler/experiment_access/__init__.py
 Comment: 
 
 Filename: laboneq/compiler/experiment_access/acquire_info.py
 Comment: 
 
-Filename: laboneq/compiler/experiment_access/cache.py
-Comment: 
-
 Filename: laboneq/compiler/experiment_access/device_info.py
 Comment: 
 
 Filename: laboneq/compiler/experiment_access/dsl_loader.py
 Comment: 
 
 Filename: laboneq/compiler/experiment_access/experiment_dao.py
@@ -150,90 +153,75 @@
 
 Filename: laboneq/compiler/experiment_access/param_ref.py
 Comment: 
 
 Filename: laboneq/compiler/experiment_access/pulse_def.py
 Comment: 
 
-Filename: laboneq/compiler/experiment_access/section_graph.py
-Comment: 
-
 Filename: laboneq/compiler/experiment_access/section_info.py
 Comment: 
 
 Filename: laboneq/compiler/experiment_access/section_signal_pulse.py
 Comment: 
 
 Filename: laboneq/compiler/experiment_access/signal_info.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/__init__.py
-Comment: 
-
-Filename: laboneq/compiler/new_scheduler/case_schedule.py
-Comment: 
-
-Filename: laboneq/compiler/new_scheduler/interval_schedule.py
-Comment: 
-
-Filename: laboneq/compiler/new_scheduler/loop_iteration_schedule.py
+Filename: laboneq/compiler/scheduler/__init__.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/loop_schedule.py
+Filename: laboneq/compiler/scheduler/case_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/match_schedule.py
+Filename: laboneq/compiler/scheduler/interval_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/oscillator_schedule.py
+Filename: laboneq/compiler/scheduler/loop_iteration_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/phase_reset_schedule.py
+Filename: laboneq/compiler/scheduler/loop_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/preorder_map.py
+Filename: laboneq/compiler/scheduler/match_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/pulse_phase.py
+Filename: laboneq/compiler/scheduler/oscillator_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/pulse_schedule.py
+Filename: laboneq/compiler/scheduler/phase_reset_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/reserve_schedule.py
+Filename: laboneq/compiler/scheduler/preorder_map.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/root_schedule.py
+Filename: laboneq/compiler/scheduler/pulse_phase.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/schedule_data.py
+Filename: laboneq/compiler/scheduler/pulse_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/scheduler.py
+Filename: laboneq/compiler/scheduler/reserve_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/section_schedule.py
+Filename: laboneq/compiler/scheduler/root_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/new_scheduler/utils.py
+Filename: laboneq/compiler/scheduler/sampling_rate_tracker.py
 Comment: 
 
-Filename: laboneq/compiler/scheduler/__init__.py
+Filename: laboneq/compiler/scheduler/schedule_data.py
 Comment: 
 
-Filename: laboneq/compiler/scheduler/event_graph.py
+Filename: laboneq/compiler/scheduler/scheduler.py
 Comment: 
 
-Filename: laboneq/compiler/scheduler/event_graph_builder.py
+Filename: laboneq/compiler/scheduler/section_schedule.py
 Comment: 
 
-Filename: laboneq/compiler/scheduler/sampling_rate_tracker.py
-Comment: 
-
-Filename: laboneq/compiler/scheduler/scheduler.py
+Filename: laboneq/compiler/scheduler/utils.py
 Comment: 
 
 Filename: laboneq/compiler/workflow/__init__.py
 Comment: 
 
 Filename: laboneq/compiler/workflow/compiler.py
 Comment: 
@@ -558,14 +546,17 @@
 
 Filename: laboneq/dsl/device/ports.py
 Comment: 
 
 Filename: laboneq/dsl/device/qubits.py
 Comment: 
 
+Filename: laboneq/dsl/device/quops.py
+Comment: 
+
 Filename: laboneq/dsl/device/server.py
 Comment: 
 
 Filename: laboneq/dsl/device/instruments/__init__.py
 Comment: 
 
 Filename: laboneq/dsl/device/instruments/hdawg.py
@@ -681,24 +672,27 @@
 
 Filename: laboneq/openqasm3/expression.py
 Comment: 
 
 Filename: laboneq/openqasm3/gate_store.py
 Comment: 
 
+Filename: laboneq/openqasm3/namespace.py
+Comment: 
+
 Filename: laboneq/openqasm3/openqasm3_importer.py
 Comment: 
 
 Filename: laboneq/openqasm3/openqasm_error.py
 Comment: 
 
 Filename: laboneq/openqasm3/reset_gate_factory.py
 Comment: 
 
-Filename: laboneq/openqasm3/variable_store.py
+Filename: laboneq/openqasm3/signal_store.py
 Comment: 
 
 Filename: laboneq/pulse_sheet_viewer/__init__.py
 Comment: 
 
 Filename: laboneq/pulse_sheet_viewer/event_graph_viewer.py
 Comment: 
@@ -720,26 +714,26 @@
 
 Filename: laboneq/simulator/seqc_parser.py
 Comment: 
 
 Filename: laboneq/simulator/wave_scroller.py
 Comment: 
 
-Filename: laboneq-2.5.0.dist-info/AUTHORS
+Filename: laboneq-2.6.0.dist-info/AUTHORS
 Comment: 
 
-Filename: laboneq-2.5.0.dist-info/LICENSE
+Filename: laboneq-2.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: laboneq-2.5.0.dist-info/METADATA
+Filename: laboneq-2.6.0.dist-info/METADATA
 Comment: 
 
-Filename: laboneq-2.5.0.dist-info/WHEEL
+Filename: laboneq-2.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: laboneq-2.5.0.dist-info/top_level.txt
+Filename: laboneq-2.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: laboneq-2.5.0.dist-info/RECORD
+Filename: laboneq-2.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## laboneq/VERSION.txt

```diff
@@ -1 +1 @@
-2.5.0
+2.6.0
```

## laboneq/simple.py

```diff
@@ -21,14 +21,16 @@
     Oscillator,
     Precompensation,
     SignalCalibration,
     units,
 )
 from laboneq.dsl.device import DeviceSetup
 from laboneq.dsl.device.device_setup_helper import DeviceSetupHelper
+from laboneq.dsl.device.qubits import QuantumElement, Qubit
+from laboneq.dsl.device.quops import QuantumOperation
 from laboneq.dsl.enums import (
     AcquisitionType,
     AveragingMode,
     CarrierType,
     ExecutionType,
     HighPassCompensationClearing,
     ModulationType,
```

## laboneq/compiler/code_generator/analyze_playback.py

```diff
@@ -29,15 +29,14 @@
 from laboneq.compiler.common.awg_sampled_event import (
     AWGEvent,
     AWGEventType,
     AWGSampledEventSequence,
 )
 from laboneq.compiler.common.awg_signal_type import AWGSignalType
 from laboneq.compiler.common.device_type import DeviceType
-from laboneq.compiler.common.event_type import EventType
 from laboneq.compiler.common.play_wave_type import PlayWaveType
 from laboneq.compiler.common.signal_obj import SignalObj
 from laboneq.core.exceptions import LabOneQException
 from laboneq.core.utilities.pulse_sampler import (
     combine_pulse_parameters,
     interval_to_samples_with_errors,
     length_to_samples,
@@ -45,14 +44,15 @@
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass
 class _IntervalStartEvent:
     event_type: str
+    signal_id: str
     time: float
     play_wave_id: str
     amplitude: float
     index: int
     oscillator_phase: Optional[float]
     oscillator_frequency: Optional[float]
     phase: Optional[float]
@@ -72,111 +72,29 @@
     index: int
 
 
 @dataclass
 class _PlayIntervalData:
     pulse: str
     index: int
+    signal_id: str
     amplitude: float
     channel: int
     oscillator_phase: float
     oscillator_frequency: float
     baseband_phase: float
     phase: float
     sub_channel: int
     play_pulse_parameters: Optional[Dict[str, Any]]
     pulse_pulse_parameters: Optional[Dict[str, Any]]
     state: int
     start_rounding_error: float
     markers: Any
 
 
-def _analyze_oscillator_switch_events(
-    signals: Dict[str, SignalObj],
-    events: List[Dict],
-    sampling_rate: float,
-    granularity: int,
-    delay: float,
-) -> AWGSampledEventSequence:
-    osc_switch_events = AWGSampledEventSequence()
-    hw_oscillators = {
-        signal_id: signals[signal_id].hw_oscillator for signal_id in signals
-    }
-    hw_oscs_values = set(hw_oscillators.values())
-    awg = next(iter(signals.values())).awg
-    device_type = awg.device_type
-    if device_type == DeviceType.HDAWG:
-        if awg.signal_type == AWGSignalType.DOUBLE:
-            # Skip for now. In double mode, 2 oscillators may (?) be active.
-            # todo (PW): Do we support dual HW modulated RF signals?
-            return osc_switch_events
-    if not device_type.supports_oscillator_switching:
-        if len(hw_oscs_values) > 1:
-            raise LabOneQException(
-                f"Attempting to multiplex several HW-modulated signals "
-                f"({', '.join(signals)}) on {device_type.value}, which does not "
-                f"support oscillator switching."
-            )
-    if len(hw_oscs_values) <= 1:
-        return osc_switch_events
-
-    if None in hw_oscs_values:
-        missing_oscillator_signal = next(
-            signal_id for signal_id, osc in hw_oscillators.items() if osc is None
-        )
-        del hw_oscillators[missing_oscillator_signal]
-        other_signals = set(hw_oscillators.keys())
-        raise LabOneQException(
-            f"Attempting to multiplex HW-modulated signal(s) "
-            f"({', '.join(other_signals)}) "
-            f"with signal that is not HW modulated ({missing_oscillator_signal})."
-        )
-
-    active_osc = None
-    active_play_segments = set()
-    current_osc = None
-
-    for event in events:
-        if event.get("signal") not in signals:
-            continue
-        signal_id = event["signal"]
-        event_time_in_samples = length_to_samples(event["time"] + delay, sampling_rate)
-        if event["event_type"] == EventType.PLAY_START:
-            if active_osc is not None:
-                raise LabOneQException(
-                    f"Conflicting HW oscillators on signals {', '.join(signals)}"
-                )
-            active_osc = hw_oscillators.get(signal_id)
-            active_play_segments.add(event["chain_element_id"])
-
-            if active_osc != current_osc:
-                current_osc = active_osc
-
-                # Round down to sequencer grid. Collisions with other playback will be
-                # detected downstream when calculating waveform intervals.
-                osc_switch_time = event_time_in_samples // granularity * granularity
-
-                osc_switch_event = AWGEvent(
-                    type=AWGEventType.SWITCH_OSCILLATOR,
-                    start=osc_switch_time,
-                    params={
-                        "oscillator": active_osc,
-                        "signal": signal_id,
-                        "section_name": event["section_name"],
-                        "play_wave_id": event["play_wave_id"],
-                    },
-                )
-                osc_switch_events.add(osc_switch_time, osc_switch_event)
-        elif event["event_type"] == EventType.PLAY_END:
-            active_play_segments.remove(event["chain_element_id"])
-            if len(active_play_segments) == 0:
-                active_osc = None
-    return osc_switch_events
-
-
 def _analyze_branches(events, delay, sampling_rate, playwave_max_hint):
     """For feedback, the pulses in the branches create a single waveform which spans
     the whole duration of the section; also keep the state to be able to split
     later.
     """
     cut_points = set()
     branching_intervals: Dict[str, List[MutableInterval]] = {}
@@ -222,14 +140,15 @@
     for state in itertools.chain(set(states.values()), (None,)):
         for index, cur_signal_id in enumerate(signal_ids):
             interval_zip.extend(
                 zip(
                     [
                         _IntervalStartEvent(
                             event_type=event["event_type"],
+                            signal_id=cur_signal_id,
                             time=event["time"] + delay,
                             play_wave_id=event["play_wave_id"],
                             amplitude=event["amplitude"],
                             index=index,
                             oscillator_phase=event.get("oscillator_phase"),
                             oscillator_frequency=event.get("oscillator_frequency"),
                             phase=event.get("phase"),
@@ -260,14 +179,15 @@
                 )
             )
             interval_zip.extend(
                 zip(
                     [
                         _IntervalStartEvent(
                             event_type="DELAY_START",
+                            signal_id=cur_signal_id,
                             time=event["time"] + delay,
                             play_wave_id=None,
                             amplitude=None,
                             index=index,
                             oscillator_phase=None,
                             oscillator_frequency=None,
                             phase=None,
@@ -321,14 +241,15 @@
 
 def _make_interval_tree(
     events, states, signal_ids, delay, sub_channel, sampling_rate
 ) -> IntervalTree:
     interval_zip = _interval_list(events, states, signal_ids, delay, sub_channel)
 
     interval_tree = IntervalTree()
+
     for index, (interval_start, interval_end) in enumerate(interval_zip):
         oscillator_phase = interval_start.oscillator_phase
 
         baseband_phase: Optional[float] = None
         if interval_start.baseband_phase is not None:
             baseband_phase = interval_start.baseband_phase
         (start_samples, end_samples), (
@@ -340,26 +261,27 @@
 
         if start_samples != end_samples:
             interval_tree.addi(
                 start_samples,
                 end_samples,
                 _PlayIntervalData(
                     pulse=interval_start.play_wave_id,
+                    signal_id=interval_start.signal_id,
                     index=index,
                     amplitude=interval_start.amplitude,
                     channel=interval_start.index,
                     oscillator_phase=oscillator_phase,
+                    oscillator_frequency=interval_start.oscillator_frequency,
                     baseband_phase=baseband_phase,
                     phase=interval_start.phase,
                     sub_channel=interval_start.sub_channel,
                     play_pulse_parameters=interval_start.play_pulse_parameters,
                     pulse_pulse_parameters=interval_start.pulse_pulse_parameters,
                     state=interval_start.state,
                     start_rounding_error=start_rounding_error,
-                    oscillator_frequency=interval_start.oscillator_frequency,
                     markers=interval_start.markers,
                 ),
             )
 
         else:
             _logger.debug(
                 "Skipping interval %s because it is zero length (from %s samples to %s samples) ",
@@ -373,56 +295,88 @@
 
     return interval_tree
 
 
 def _oscillator_switch_cut_points(
     interval_tree: IntervalTree,
     signals: Dict[str, SignalObj],
-    events,
-    sampling_rate,
     sample_multiple,
-    delay,
-    other_events: AWGSampledEventSequence,
-) -> AWGSampledEventSequence:
+) -> Tuple[AWGSampledEventSequence, Set]:
     cut_points = set()
-    oscillator_switch_events = _analyze_oscillator_switch_events(
-        signals, events, sampling_rate, sample_multiple, delay
-    )
 
-    other_events.merge(oscillator_switch_events)
+    osc_switch_events = AWGSampledEventSequence()
+    hw_oscillators = {
+        signal_id: signals[signal_id].hw_oscillator for signal_id in signals
+    }
+    hw_oscs_values = set(hw_oscillators.values())
+    awg = next(iter(signals.values())).awg
+    device_type = awg.device_type
+    if device_type == DeviceType.HDAWG:
+        if awg.signal_type == AWGSignalType.DOUBLE:
+            # Skip for now. In double mode, 2 oscillators may (?) be active.
+            # todo (PW): Do we support dual HW modulated RF signals?
+            return osc_switch_events, cut_points
+    if not device_type.supports_oscillator_switching:
+        if len(hw_oscs_values) > 1:
+            raise LabOneQException(
+                f"Attempting to multiplex several HW-modulated signals "
+                f"({', '.join(signals)}) on {device_type.value}, which does not "
+                f"support oscillator switching."
+            )
+    if len(hw_oscs_values) <= 1:
+        return osc_switch_events, cut_points
 
-    for event_time, other_event_list in other_events.sequence.items():
-        intervals: List[Interval] = [
-            interval
-            for interval in interval_tree.at(event_time)
-            if interval.begin < event_time
-        ]
+    if None in hw_oscs_values:
+        missing_oscillator_signal = next(
+            signal_id for signal_id, osc in hw_oscillators.items() if osc is None
+        )
+        del hw_oscillators[missing_oscillator_signal]
+        other_signals = set(hw_oscillators.keys())
+        raise LabOneQException(
+            f"Attempting to multiplex HW-modulated signal(s) "
+            f"({', '.join(other_signals)}) "
+            f"with signal that is not HW modulated ({missing_oscillator_signal})."
+        )
 
-        if len(intervals) > 0:
-            try:
-                other_event = next(
-                    e
-                    for e in other_event_list
-                    if e.type == AWGEventType.SWITCH_OSCILLATOR
-                )
-                section = other_event.params["section_name"]
-                pulse = other_event.params["play_wave_id"]
-                signal_name = other_event.params["signal"]
-                raise LabOneQException(
-                    f"In section {section}, pulse {pulse}, on signal {signal_name}: "
-                    f"cannot switch oscillator because the event intersects with "
-                    f"other playback."
-                )
-            except StopIteration:
-                pass
-            raise RuntimeError(
-                f"Events {other_event_list} intersect playWave intervals {intervals}"
+    osc_intervals = IntervalTree()
+    for pulse_iv in interval_tree:
+        oscillator = signals[pulse_iv.data.signal_id].hw_oscillator
+        # if there were any pulses w/o HW modulator, we should have returned already
+        assert oscillator is not None
+
+        osc_intervals.addi(
+            # Round down to sequencer grid
+            pulse_iv.begin // sample_multiple * sample_multiple,
+            pulse_iv.end,
+            {
+                "oscillator": oscillator,
+                "signal": pulse_iv.data.signal_id,
+            },
+        )
+
+    def reducer(a, b):
+        if a["oscillator"] != b["oscillator"]:
+            raise LabOneQException(
+                f"Overlapping HW oscillators: "
+                f"'{a['oscillator']}' on signal '{a['signal']}' and "
+                f"'{b['oscillator']}' on signal '{b['signal']}'"
             )
-        else:
-            cut_points.add(event_time)
+        return a
+
+    osc_intervals.merge_overlaps(reducer)
+
+    oscillator_switch_events = AWGSampledEventSequence()
+    for iv in osc_intervals:
+        osc_switch_event = AWGEvent(
+            type=AWGEventType.SWITCH_OSCILLATOR,
+            start=iv.begin,
+            params={"oscillator": iv.data["oscillator"], "signal": iv.data["signal"]},
+        )
+        oscillator_switch_events.add(iv.begin, osc_switch_event)
+        cut_points.add(iv.begin)
 
     return oscillator_switch_events, cut_points
 
 
 def _sequence_end(events, sampling_rate, sample_multiple, delay, waveform_size_hint):
     sequence_end = length_to_samples(
         max(event["time"] for event in events) + delay, sampling_rate
@@ -567,27 +521,21 @@
 
     use_ct_phase = use_command_table and all(s.hw_oscillator for s in signals.values())
 
     sequence_end = _sequence_end(
         events, sampling_rate, sample_multiple, delay, waveform_size_hints
     )
     cut_points.add(sequence_end)
+    cut_points.update(other_events.sequence)
 
     (
         oscillator_switch_events,
         oscillator_switch_cut_points,
-    ) = _oscillator_switch_cut_points(
-        interval_tree,
-        signals,
-        events,
-        sampling_rate,
-        sample_multiple,
-        delay,
-        other_events,
-    )
+    ) = _oscillator_switch_cut_points(interval_tree, signals, sample_multiple)
+
     cut_points.update(oscillator_switch_cut_points)
     oscillator_intervals = _oscillator_intervals(
         signals.values(), oscillator_switch_events, sequence_end
     )
     used_oscillators = {osc_iv.data["oscillator"] for osc_iv in oscillator_intervals}
     if len(used_oscillators) > 1 and not use_command_table:
         raise LabOneQException(
```

## laboneq/compiler/code_generator/code_generator.py

```diff
@@ -45,14 +45,19 @@
 )
 from laboneq.compiler.code_generator.seqc_tracker import SeqCTracker
 from laboneq.compiler.code_generator.signatures import (
     PlaybackSignature,
     WaveformSignature,
 )
 from laboneq.compiler.code_generator.utils import normalize_phase
+from laboneq.compiler.code_generator.wave_compressor import (
+    PlayHold,
+    PlaySamples,
+    WaveCompressor,
+)
 from laboneq.compiler.code_generator.wave_index_tracker import WaveIndexTracker
 from laboneq.compiler.common.awg_info import AWGInfo, AwgKey
 from laboneq.compiler.common.awg_sampled_event import (
     AWGEvent,
     AWGEventType,
     AWGSampledEventSequence,
 )
@@ -274,14 +279,15 @@
         self._signal_delays: SignalDelays = None
         self._integration_weights = None
         self._simultaneous_acquires: Dict[float, Dict[str, str]] = None
         self._command_table_match_offsets: Dict[AwgKey, int] = {}
         self._feedback_connections: Dict[str, FeedbackConnection] = {}
         self._feedback_register_allocator: FeedbackRegisterAllocator = None
         self._total_execution_time = None
+        self._wave_compressor = WaveCompressor()
 
         self.EMIT_TIMING_COMMENTS = self._settings.EMIT_TIMING_COMMENTS
         self.PHASE_RESOLUTION_BITS = self._settings.PHASE_RESOLUTION_BITS
 
     def integration_weights(self):
         return self._integration_weights
 
@@ -685,14 +691,151 @@
             awg.awg_number,
             EngNumber(global_delay or 0),
             [(s, EngNumber(d)) for s, d in all_relevant_delays.items()],
         )
 
         return global_sampling_rate, global_delay
 
+    def _emit_new_awg_events(self, old_event, new_events):
+        new_awg_events = []
+        time = old_event.start
+        for new_event in new_events:
+            if isinstance(new_event, PlayHold):
+                new_awg_events.append(
+                    AWGEvent(
+                        type=AWGEventType.PLAY_HOLD,
+                        start=time,
+                        end=time + new_event.num_samples,
+                    )
+                )
+                time += new_event.num_samples
+            if isinstance(new_event, PlaySamples):
+                new_params = copy.deepcopy(old_event.params)
+                new_length = len(next(iter(new_event.samples.values())))
+
+                new_params["playback_signature"].waveform.length = new_length
+
+                assert len(new_params["playback_signature"].waveform.pulses) == 1
+                new_params["playback_signature"].waveform.pulses[0].length = new_length
+                new_params["playback_signature"].waveform.pulses[
+                    0
+                ].pulse += f"_compr_{new_event.label}"
+
+                new_awg_events.append(
+                    AWGEvent(
+                        type=AWGEventType.PLAY_WAVE,
+                        start=time,
+                        end=time + new_length,
+                        params=new_params,
+                    )
+                )
+
+                time += new_length
+        return new_awg_events
+
+    def _compress_waves(
+        self, sampled_events, sampled_signatures, signal_obj, pulse_defs
+    ):
+        compressed_waveform_signatures = set()
+        for event_group in sampled_events.sequence.values():
+            event_replacement = {}
+            for i, event in enumerate(event_group):
+                if event.type == AWGEventType.PLAY_WAVE:
+                    wave_form = event.params["playback_signature"].waveform
+                    if wave_form.pulses[0].pulse not in pulse_defs:
+                        assert (
+                            wave_form.pulses[0].pulse is None
+                            or wave_form.pulses[0].pulse == "dummy_precomp_reset"
+                        )
+                        continue
+                    if not pulse_defs[wave_form.pulses[0].pulse].can_compress:
+                        continue
+                    if len(wave_form.pulses) > 1:
+                        _logger.info(
+                            "Requested to compress wave which features more than one pulse. Skipping compression."
+                        )
+                        continue
+                    sampled_signature = sampled_signatures[wave_form]
+                    sample_dict = {
+                        k: sampled_signature[k]
+                        for k in (
+                            "samples_i",
+                            "samples_q",
+                            "samples_marker1",
+                            "samples_marker2",
+                        )
+                        if k in sampled_signature
+                    }
+                    new_events = self._wave_compressor.compress_wave(
+                        sample_dict, signal_obj.device_type.min_play_wave
+                    )
+                    if new_events is None:
+                        _logger.info(
+                            "Requested to compress pulse %s which has either no, or too short, constant sections. Skipping compression",
+                            wave_form.pulses[0].pulse,
+                        )
+                        continue
+                    event_replacement[i] = new_events
+                    _logger.info(
+                        "Compressing pulse %s using %d PlayWave and %d PlayHold events",
+                        wave_form.pulses[0].pulse,
+                        sum(
+                            1 for event in new_events if isinstance(event, PlaySamples)
+                        ),
+                        sum(1 for event in new_events if isinstance(event, PlayHold)),
+                    )
+            for idx, new_events in event_replacement.items():
+                new_awg_events = self._emit_new_awg_events(event_group[idx], new_events)
+
+                old_event = event_group[idx]
+                event_group[idx : idx + 1] = new_awg_events
+
+                old_waveform = old_event.params["playback_signature"].waveform
+                for new_event, new_awg_event in zip(new_events, new_awg_events):
+                    if new_awg_event.type == AWGEventType.PLAY_WAVE:
+                        new_waveform = new_awg_event.params[
+                            "playback_signature"
+                        ].waveform
+                        new_length = len(next(iter(new_event.samples.values())))
+
+                        old_sampled_signature = self._sampled_signatures[signal_obj.id][
+                            old_waveform
+                        ]
+                        compressed_waveform_signatures.add(old_waveform)
+                        new_sampled_signature = copy.deepcopy(old_sampled_signature)
+
+                        new_sampled_signature = (
+                            new_sampled_signature | new_event.samples
+                        )
+                        new_signature_pulse_map = new_sampled_signature[
+                            "signature_pulse_map"
+                        ]
+
+                        old_pulse_name = old_waveform.pulses[0].pulse
+                        new_pulse_name = new_waveform.pulses[0].pulse
+
+                        new_signature_pulse_map[
+                            new_pulse_name
+                        ] = new_signature_pulse_map.pop(old_pulse_name)
+                        new_signature_pulse_map[
+                            new_pulse_name
+                        ].length_samples = new_length
+
+                        new_signature_pulse_map[new_pulse_name].instances[
+                            0
+                        ].length = new_length
+
+                        self._sampled_signatures[signal_obj.id][
+                            new_waveform
+                        ] = new_sampled_signature
+
+        # evict waveforms that have been compressed, and thus replaced with one or more, shorter, waves
+        for waveform_signature in compressed_waveform_signatures:
+            self._sampled_signatures[signal_obj.id].pop(waveform_signature)
+
     def _gen_seq_c_per_awg(
         self,
         awg: AWGInfo,
         events: List[Any],
         pulse_defs: Dict[str, PulseDef],
     ):
         function_defs_generator = SeqCGenerator()
@@ -872,14 +1015,22 @@
                 device_type=device_type,
                 multi_iq_signal=True,
                 mixer_type=mixer_type,
             )
 
             self._sampled_signatures[virtual_signal_id] = sampled_signatures
             sampled_events.merge(interval_events)
+
+            self._compress_waves(
+                sampled_events=sampled_events,
+                sampled_signatures=sampled_signatures,
+                signal_obj=signal_obj,
+                pulse_defs=pulse_defs,
+            )
+
             if virtual_signal_id in self._sampled_signatures:
                 for sig, sampled in self._sampled_signatures[virtual_signal_id].items():
                     if not sampled:
                         continue
                     sig_string = sig.signature_string()
 
                     length = sig.length
@@ -923,14 +1074,21 @@
                     device_type=signal_obj.device_type,
                     mixer_type=signal_obj.mixer_type,
                 )
 
                 self._sampled_signatures[signal_obj.id] = sampled_signatures
                 sampled_events.merge(interval_events)
 
+                self._compress_waves(
+                    sampled_events=sampled_events,
+                    sampled_signatures=sampled_signatures,
+                    signal_obj=signal_obj,
+                    pulse_defs=pulse_defs,
+                )
+
                 if signal_obj.id in self._sampled_signatures:
                     signature_infos = []
                     for sig, sampled in self._sampled_signatures[signal_obj.id].items():
                         has_marker1 = False
                         has_marker2 = False
                         if sampled:
                             if "samples_marker1" in sampled:
@@ -977,14 +1135,22 @@
                 signal_type=signal_a.signal_type,
                 device_type=signal_a.device_type,
                 mixer_type=signal_a.mixer_type,
             )
 
             self._sampled_signatures[virtual_signal_id] = sampled_signatures
             sampled_events.merge(interval_events)
+
+            self._compress_waves(
+                sampled_events=sampled_events,
+                sampled_signatures=sampled_signatures,
+                signal_obj=signal_obj,
+                pulse_defs=pulse_defs,
+            )
+
             if virtual_signal_id in self._sampled_signatures:
                 for sig, sampled in self._sampled_signatures[virtual_signal_id].items():
                     if not sampled:
                         continue
                     sig_string = sig.signature_string()
                     length = sig.length
                     declarations_generator.add_wave_declaration(
@@ -1366,14 +1532,15 @@
                         if play_pulse_parameters is None
                         else {k: v for k, v in play_pulse_parameters},
                         pulse_pulse_parameters=None
                         if pulse_pulse_parameters is None
                         else {k: v for k, v in pulse_pulse_parameters},
                         has_marker1=has_marker1,
                         has_marker2=has_marker2,
+                        can_compress=pulse_def.can_compress,
                     )
                 )
 
             sampled_pulse_obj = {
                 "signature_pulse_map": signature_pulse_map,
                 "samples_i": samples_i,
             }
```

## laboneq/compiler/code_generator/measurement_calculator.py

```diff
@@ -30,15 +30,14 @@
     num_plays: Any = field(default=0)
     awg: Any = field(default=None)
     device_id: Any = field(default=None)
     length: Any = field(default=None)
     device_type: Any = field(default=None)
     delay_signal: Any = field(default=None)
     length_in_samples: int = None
-    delay_in_samples: int = None
 
 
 @dataclass(init=True, repr=True, order=True)
 class SectionIntegrationInfo:
     signals: Dict[str, SignalIntegrationInfo] = field(default_factory=dict)
     section_start: float = field(default=0.0)
 
@@ -202,34 +201,29 @@
                 )
 
                 signal_integration_info.length_in_samples = round(
                     signal_integration_info.length * sampling_rate
                 )
                 _dlogger.debug("signal_integration_info=%s", signal_integration_info)
                 _dlogger.debug("section_info=%s", section_info)
-                delay_time = signal_integration_info.start - section_info.section_start
 
-                signal_integration_info.delay = delay_time
-                delay_in_samples = round(signal_integration_info.delay * sampling_rate)
-                signal_integration_info.delay_in_samples = delay_in_samples
+                delay_time = signal_integration_info.start - section_info.section_start
 
                 awg_key = (
                     signal_info["device_id"],
                     signal_integration_info.awg,
                     "PLAY" if signal_integration_info.is_play else "ACQUIRE",
                 )
                 if awg_key not in delays_per_awg:
                     delays_per_awg[awg_key] = {
                         "delays": set(),
                         "signals": [],
                         "sections": [],
                     }
-                delays_per_awg[awg_key]["delays"].add(
-                    signal_integration_info.delay_in_samples
-                )
+                delays_per_awg[awg_key]["delays"].add(round(delay_time * sampling_rate))
                 delays_per_awg[awg_key]["signals"].append(signal)
                 delays_per_awg[awg_key]["sections"].append(section_name)
                 delays_per_awg[awg_key]["device_type"] = DeviceType(
                     signal_info["device_type"]
                 )
 
         _dlogger.debug("Delays per awg: %s", delays_per_awg)
@@ -369,23 +363,14 @@
                             on_device=acquire_delay_in_s + rounding_error_acquire,
                         )
 
             except StopIteration:
                 pass
 
         for k, v in integration_times.items():
-            for signal, section_signal_info in v.items():
-                if signal in signal_delays and section_signal_info.delay is not None:
-                    section_signal_info.delay = signal_delays[signal].on_device
-                    sampling_rate = signal_info["sampling_rate"]
-                    section_signal_info.delay_in_samples = round(
-                        section_signal_info.delay * sampling_rate
-                    )
-
-        for k, v in integration_times.items():
             _dlogger.debug("%s:", k)
             for x, y in v.items():
                 _dlogger.debug("  %s:%s", x, y)
 
         for signal_id, signal_delay in signal_delays.items():
             _dlogger.debug("Signal delay for %s:", signal_id)
             signal_info = signal_info_map[signal_id]
```

## laboneq/compiler/code_generator/sampled_event_handler.py

```diff
@@ -14,14 +14,15 @@
 )
 from laboneq.compiler.code_generator.signatures import PlaybackSignature
 from laboneq.compiler.common.awg_sampled_event import (
     AWGEvent,
     AWGEventType,
     AWGSampledEventSequence,
 )
+from laboneq.compiler.common.compiler_settings import EXECUTETABLEENTRY_LATENCY
 from laboneq.compiler.common.device_type import DeviceType
 from laboneq.core.exceptions import LabOneQException
 
 if TYPE_CHECKING:
     from laboneq.compiler.code_generator.command_table_tracker import (
         CommandTableTracker,
     )
@@ -242,14 +243,24 @@
                     sampled_event.start - self.match_parent_event.start,
                 )
             self.feedback_connections.setdefault(
                 self.match_parent_event.params["handle"], FeedbackConnection(None)
             ).drive.add(signal_id)
         return True
 
+    def handle_playhold(
+        self,
+        sampled_event: AWGEvent,
+    ):
+        assert self.seqc_tracker.current_time == sampled_event.start
+        self.seqc_tracker.add_play_hold_statement(
+            sampled_event.end - sampled_event.start
+        )
+        self.seqc_tracker.current_time = sampled_event.end
+
     def handle_acquire(self, sampled_event: AWGEvent):
         _logger.debug("  Processing ACQUIRE EVENT %s", sampled_event)
 
         args = [
             "QA_INT_ALL",
             "1" if "RAW" in sampled_event.params["acquisition_type"] else "0",
         ]
@@ -614,32 +625,40 @@
                     assert self.command_table_match_offset + idx == id2
 
             ev = self.match_parent_event
             start = ev.start
             assert start >= self.seqc_tracker.current_time
             assert start % self.sequencer_step == 0
             self.seqc_tracker.add_required_playzeros(ev)
-            latency = start // self.sequencer_step - self.current_sequencer_step
+            # Subtract the 3 cycles that we added (see match_schedule.py for details)
+            latency = (
+                start // self.sequencer_step
+                - self.current_sequencer_step
+                - EXECUTETABLEENTRY_LATENCY
+            )
             self.seqc_tracker.add_command_table_execution(
                 "QA_DATA_PROCESSED"
                 if ev.params["local"]
                 else "ZSYNC_DATA_PQSC_REGISTER",
-                latency=f"current_seq_step + {latency}",
+                latency="current_seq_step "
+                + (f"+ {latency}" if latency >= 0 else f"- {-latency}"),
                 comment="Match handle " + handle,
             )
             self.seqc_tracker.add_timing_comment(ev.end)
             self.seqc_tracker.flush_deferred_function_calls()
             self.seqc_tracker.current_time = self.match_parent_event.end
             self.match_parent_event = None
 
     def handle_sampled_event(self, sampled_event: AWGEvent):
         signature = sampled_event.type
         if signature == AWGEventType.PLAY_WAVE:
             if not self.handle_playwave(sampled_event):
                 return
+        if signature == AWGEventType.PLAY_HOLD:
+            self.handle_playhold(sampled_event)
         elif signature == AWGEventType.ACQUIRE:
             self.handle_acquire(sampled_event)
         elif signature == AWGEventType.QA_EVENT:
             self.handle_qa_event(sampled_event)
         elif signature == AWGEventType.RESET_PRECOMPENSATION_FILTERS:
             self.handle_reset_precompensation_filters(sampled_event)
         elif signature in (
```

## laboneq/compiler/code_generator/seq_c_generator.py

```diff
@@ -14,18 +14,18 @@
 from laboneq.compiler.code_generator.compressor import Run, compressor_core
 from laboneq.compiler.common.device_type import DeviceType
 from laboneq.core.exceptions import LabOneQException
 
 _logger = logging.getLogger(__name__)
 
 
-MAX_PLAY_ZERO_UHFQA = 131056
-MAX_PLAY_ZERO_HDAWG = 1048560
+MAX_PLAY_ZERO_HOLD_UHFQA = 131056
+MAX_PLAY_ZERO_HOLD_HDAWG = 1048560
 
-MIN_PLAY_ZERO = 512 + 128
+MIN_PLAY_ZERO_HOLD = 512 + 128
 
 
 @functools.lru_cache()
 def string_sanitize(input):
     """Sanitize the input string, so it can be safely used as (part of) an identifier
     in seqC."""
 
@@ -197,102 +197,131 @@
                 "type": "executeTableEntry",
                 "table_index": ct_index,
                 "latency": latency,
                 "comment": comment,
             }
         )
 
-    def add_play_zero_statement(
+    def _add_play_zero_or_hold(
         self,
         num_samples,
         device_type,
+        fname: str,
         deferred_calls: Optional[SeqCGenerator] = None,
     ):
-        """Add a playZero command
-
-        If the requested number of samples exceeds the allowed number of samples for
-        a single playZero, a tight loop of playZeros will be emitted.
-
-        If deferred_calls is passed, the deferred function calls are cleared in the
-        context of the added playZero(s). The passed list will be drained.
-        """
         if deferred_calls is None:
             deferred_calls = SeqCGenerator()
 
         if isinstance(device_type, str):
             device_type = DeviceType(device_type)
 
         sample_multiple = device_type.sample_multiple
         if num_samples % sample_multiple != 0:
             raise Exception(
-                f"Emitting playZero({num_samples}), which is not divisible by {sample_multiple}, which it should be for {device_type}"
+                f"Emitting {fname}({num_samples}), which is not divisible by {sample_multiple}, which it should be for {device_type}"
             )
         if num_samples < device_type.min_play_wave:
             raise LabOneQException(
-                f"Attempting to emit playZero({num_samples}), which is below the "
+                f"Attempting to emit {fname}({num_samples}), which is below the "
                 f"minimum waveform length {device_type.min_play_wave} of device "
                 f"'{device_type.value}' (sample multiple is {device_type.sample_multiple})"
             )
-        max_play_zero = (
-            MAX_PLAY_ZERO_HDAWG
+        max_play_fun = (
+            MAX_PLAY_ZERO_HOLD_HDAWG
             if device_type == DeviceType.HDAWG
-            else MAX_PLAY_ZERO_UHFQA
+            else MAX_PLAY_ZERO_HOLD_UHFQA
         )
 
         def statement_factory(samples):
             self.add_statement(
                 {
-                    "type": "playZero",
+                    "type": f"{fname}",
                     "device_type": device_type,
                     "num_samples": samples,
                 }
             )
 
         def flush_deferred_calls():
             self.append_statements_from(deferred_calls)
             deferred_calls.clear()
 
-        if num_samples <= max_play_zero:
+        if num_samples <= max_play_fun:
             statement_factory(num_samples)
             flush_deferred_calls()
-        elif num_samples <= 2 * max_play_zero:
+        elif num_samples <= 2 * max_play_fun:
             # split in the middle
             half_samples = (num_samples // 2 // 16) * 16
             statement_factory(half_samples)
             flush_deferred_calls()
             statement_factory(num_samples - half_samples)
         else:  # non-unrolled loop
-            num_segments, rest = divmod(num_samples, max_play_zero)
-            if 0 < rest < MIN_PLAY_ZERO:
-                chunk = (max_play_zero // 2 // 16) * 16
+            num_segments, rest = divmod(num_samples, max_play_fun)
+            if 0 < rest < MIN_PLAY_ZERO_HOLD:
+                chunk = (max_play_fun // 2 // 16) * 16
                 statement_factory(chunk)
                 flush_deferred_calls()
                 num_samples -= chunk
-                num_segments, rest = divmod(num_samples, max_play_zero)
+                num_segments, rest = divmod(num_samples, max_play_fun)
             if rest > 0:
                 statement_factory(rest)
                 flush_deferred_calls()
             if deferred_calls.num_statements() > 0:
-                statement_factory(max_play_zero)
+                statement_factory(max_play_fun)
                 flush_deferred_calls()
                 num_segments -= 1
             if num_segments == 1:
-                statement_factory(max_play_zero)
+                statement_factory(max_play_fun)
                 return
 
             loop_body = SeqCGenerator()
             loop_body.add_statement(
                 {
-                    "type": "playZero",
+                    "type": f"{fname}",
                     "device_type": device_type,
-                    "num_samples": max_play_zero,
+                    "num_samples": max_play_fun,
                 }
             )
             self.add_repeat(num_segments, loop_body)
 
+    def add_play_zero_statement(
+        self,
+        num_samples,
+        device_type,
+        deferred_calls: Optional[SeqCGenerator] = None,
+    ):
+        """Add a playZero command
+
+        If the requested number of samples exceeds the allowed number of samples for
+        a single playZero, a tight loop of playZeros will be emitted.
+
+        If deferred_calls is passed, the deferred function calls are cleared in the
+        context of the added playZero(s). The passed list will be drained.
+        """
+        self._add_play_zero_or_hold(
+            num_samples, device_type, "playZero", deferred_calls
+        )
+
+    def add_play_hold_statement(
+        self,
+        num_samples,
+        device_type,
+        deferred_calls: Optional[SeqCGenerator] = None,
+    ):
+        """Add a playHold command
+
+        If the requested number of samples exceeds the allowed number of samples for
+        a single playHold, a tight loop of playZeros will be emitted.
+
+        If deferred_calls is passed, the deferred function calls are cleared in the
+        context of the added playHold(s). The passed list will be drained.
+        """
+        self._add_play_zero_or_hold(
+            num_samples, device_type, "playHold", deferred_calls
+        )
+
     def generate_seq_c(self):
         self._seq_c_text = ""
         for statement in self._statements:
             _logger.debug("processing statement %s", statement)
             self.emit_statement(statement)
         return self._seq_c_text
 
@@ -360,14 +389,16 @@
             if statement["comment"] != "":
                 self._seq_c_text += f"  // {statement['comment']}"
             self._seq_c_text += "\n"
         elif statement["type"] == "comment":
             self._seq_c_text += "/* " + statement["text"] + " */\n"
         elif statement["type"] == "playZero":
             self._seq_c_text += f"playZero({statement['num_samples']});\n"
+        elif statement["type"] == "playHold":
+            self._seq_c_text += f"playHold({statement['num_samples']});\n"
 
     def _gen_wave_declaration_placeholder(self, statement: SeqCStatement) -> str:
         dual_channel = statement["signal_type"] in ["iq", "double", "multi"]
         sig_string = statement["wave_id"]
         length = statement["length"]
         device_type = statement["device_type"]
         assert length >= device_type.min_play_wave
```

## laboneq/compiler/code_generator/seqc_tracker.py

```diff
@@ -111,14 +111,19 @@
             )
 
     def add_play_zero_statement(self, num_samples):
         self.current_loop_stack_generator().add_play_zero_statement(
             num_samples, self.device_type, self.deferred_function_calls
         )
 
+    def add_play_hold_statement(self, num_samples):
+        self.current_loop_stack_generator().add_play_hold_statement(
+            num_samples, self.device_type, self.deferred_function_calls
+        )
+
     def add_play_wave_statement(
         self, device_type: DeviceType, signal_type, wave_id, channel
     ):
         self.current_loop_stack_generator().add_play_wave_statement(
             device_type, signal_type, wave_id, channel
         )
```

## laboneq/compiler/common/awg_sampled_event.py

```diff
@@ -22,14 +22,15 @@
     SET_OSCILLATOR_FREQUENCY = auto()
     ACQUIRE = auto()
     QA_EVENT = auto()
     TRIGGER_OUTPUT = auto()
     SWITCH_OSCILLATOR = auto()
     MATCH = auto()
     PLAY_WAVE = auto()
+    PLAY_HOLD = auto()
 
 
 @dataclass
 class AWGEvent:
     type: AWGEventType
     start: int = None
     end: int = None
```

## laboneq/compiler/common/compiler_settings.py

```diff
@@ -124,7 +124,10 @@
 
     compiler_settings = CompilerSettings(**compiler_settings_dict)
 
     for k, v in asdict(compiler_settings).items():
         _logger.debug("Setting %s=%s", k, v)
 
     return compiler_settings
+
+
+EXECUTETABLEENTRY_LATENCY = 3
```

## laboneq/compiler/common/device_type.py

```diff
@@ -21,14 +21,16 @@
     channels_per_awg: int
     sampling_rate_2GHz: float = None
     num_integration_units_per_acquire_signal: int = None
     oscillator_set_latency: float = 0.0
     reset_osc_duration: float = 0.0
     supports_oscillator_switching: bool = False
     lo_frequency_granularity: Optional[float] = None
+    min_lo_frequency: Optional[float] = None
+    max_lo_frequency: Optional[float] = None
 
 
 class DeviceType(DeviceTraits, Enum):
     def __new__(cls, value: DeviceTraits):
         # This is needed to ensure DeviceType(<str_value>) resolves to the corresponding enum
         obj = object.__new__(cls)
         obj._value_ = value.str_value
@@ -96,14 +98,16 @@
         channels_per_awg=1,
         num_integration_units_per_acquire_signal=1,
         oscillator_set_latency=88e-9,
         # Verified by PW (2022-10-13) on dev12093, rev 68689. Observed ~50 ns.
         reset_osc_duration=56e-9,
         lo_frequency_granularity=100e6,
         supports_oscillator_switching=False,
+        min_lo_frequency=1e9,
+        max_lo_frequency=8.5e9,
     )
     SHFSG = DeviceTraits(
         str_value="shfsg",
         sampling_rate=2.0e9,
         min_play_wave=32,
         sample_multiple=16,
         supports_zsync=True,
@@ -115,12 +119,42 @@
         channels_per_awg=1,
         oscillator_set_latency=88e-9,
         # todo (PW): exact worst-case runtime unknown.
         # Verified by PW (2022-10-13) on dev12117, rev 68689. Observed ~35 ns.
         reset_osc_duration=56e-9,
         lo_frequency_granularity=100e6,
         supports_oscillator_switching=True,
+        min_lo_frequency=1e9,
+        max_lo_frequency=8.5e9,
     )
 
     def __repr__(self):
         cls_name = self.__class__.__name__
         return f"{cls_name}.{self.name}"
+
+
+def validate_local_oscillator_frequency(value: float, device_type: DeviceType):
+    """Validate correct local oscillator frequencies.
+
+    Raises:
+        ValueError: The value is invalid for given device type.
+    """
+    if device_type.min_lo_frequency is not None:
+        if value < device_type.min_lo_frequency:
+            raise ValueError(
+                f"({device_type}) Local oscillator frequency {value} Hz is smaller than minimum "
+                f"{device_type.min_lo_frequency} Hz."
+            )
+
+    if device_type.max_lo_frequency:
+        if value > device_type.max_lo_frequency:
+            raise ValueError(
+                f"({device_type}) Local oscillator frequency {value} Hz is larger than maximum "
+                f"{device_type.max_lo_frequency} Hz."
+            )
+
+    if device_type.lo_frequency_granularity is not None:
+        if value % device_type.lo_frequency_granularity != 0:
+            raise ValueError(
+                f"({device_type}) Local oscillator frequency {value} "
+                f"(device {device_type}) is not multiple of {device_type.lo_frequency_granularity} Hz."
+            )
```

## laboneq/compiler/experiment_access/dsl_loader.py

```diff
@@ -814,23 +814,28 @@
                             if hasattr(pulse, "samples"):
                                 samples = pulse.samples
 
                             amplitude, amplitude_param = find_value_or_parameter_attr(
                                 pulse, "amplitude", (float, int, complex)
                             )
 
+                            can_compress = False
+                            if hasattr(pulse, "can_compress"):
+                                can_compress = pulse.can_compress
+
                             self.add_pulse(
                                 pulse.uid,
                                 PulseDef(
                                     id=pulse.uid,
                                     function=function,
                                     length=length,
                                     amplitude=amplitude,
                                     amplitude_param=amplitude_param,
                                     play_mode=None,
+                                    can_compress=can_compress,
                                     samples=samples,
                                 ),
                             )
                         (
                             pulse_amplitude,
                             pulse_amplitude_param,
                         ) = find_value_or_parameter_attr(
```

## laboneq/compiler/experiment_access/experiment_dao.py

```diff
@@ -6,16 +6,16 @@
 import copy
 import logging
 from collections import deque
 from typing import List, Optional
 
 from jsonschema import ValidationError
 
+from laboneq._utils import cached_method
 from laboneq.compiler.experiment_access import json_dumper
-from laboneq.compiler.experiment_access.cache import memoize_method
 from laboneq.compiler.experiment_access.device_info import DeviceInfo
 from laboneq.compiler.experiment_access.dsl_loader import DSLLoader
 from laboneq.compiler.experiment_access.json_loader import JsonLoader
 from laboneq.compiler.experiment_access.oscillator_info import OscillatorInfo
 from laboneq.compiler.experiment_access.section_info import SectionInfo
 from laboneq.compiler.experiment_access.signal_info import SignalInfo
 from laboneq.core.exceptions import LabOneQException
@@ -180,15 +180,15 @@
             "connection_type",
             "channels",
             "delay_signal",
             "modulation",
             "offset",
         ]
 
-    @memoize_method
+    @cached_method()
     def signal_info(self, signal_id):
         signal_info = self._data["signals"].get(signal_id)
         if signal_info is not None:
             signal_info_copy = copy.deepcopy(signal_info)
             signal_connection = self._data["signal_connections"][signal_id]
 
             for k in ["device_id", "connection_type", "channels", "delay_signal"]:
@@ -213,27 +213,27 @@
         if retval.count is not None:
             retval.count = int(retval.count)
         return retval
 
     def root_sections(self):
         return self._data["root_sections"]
 
-    @memoize_method
+    @cached_method()
     def _has_near_time_child(self, section_id) -> Optional[str]:
         children = self.direct_section_children(section_id)
         for child in children:
             child_info = self.section_info(child)
             if child_info.execution_type == "controller":
                 return child
             child_contains_nt = self._has_near_time_child(child)
             if child_contains_nt:
                 return child_contains_nt
         return None
 
-    @memoize_method
+    @cached_method()
     def root_rt_sections(self):
         retval = []
         queue = deque(self.root_sections())
         while len(queue):
             candidate = queue.popleft()
             info = self.section_info(candidate)
             nt_subsection = self._has_near_time_child(candidate)
@@ -244,30 +244,30 @@
                         f"{nt_subsection}."
                     )
                 retval.append(candidate)
             else:
                 queue.extend(self.direct_section_children(candidate))
         return tuple(retval)  # tuple is immutable, so no one can break memoization
 
-    @memoize_method
+    @cached_method()
     def direct_section_children(self, section_id) -> List[str]:
         return self._data["section_tree"].get(section_id, [])
 
-    @memoize_method
+    @cached_method()
     def all_section_children(self, section_id):
         retval = []
 
         direct_children = self.direct_section_children(section_id)
         retval = retval + direct_children
         for child in direct_children:
             retval = retval + list(self.all_section_children(child))
 
         return set(retval)
 
-    @memoize_method
+    @cached_method()
     def section_parent(self, section_id):
         try:
             return next(
                 parent
                 for parent, children in self._data["section_tree"].items()
                 if section_id in children
             )
@@ -301,15 +301,15 @@
 
     def is_dio_leader(self, device_id):
         return bool({d[1] for d in self._data["dios"] if d[0] == device_id})
 
     def section_signals(self, section_id):
         return self._data["section_signals"].get(section_id, set())
 
-    @memoize_method
+    @cached_method()
     def section_signals_with_children(self, section_id):
         retval = set()
         section_with_children = self.all_section_children(section_id)
         section_with_children.add(section_id)
         for child in section_with_children:
             retval = retval.union(self.section_signals(child))
         return retval
```

## laboneq/compiler/experiment_access/pulse_def.py

```diff
@@ -14,15 +14,16 @@
 class PulseDef:
     id: str
     function: str
     length: float
     amplitude: float
     amplitude_param: str
     play_mode: str
-    samples: Optional[ArrayLike]
+    can_compress: Optional[bool] = False
+    samples: Optional[ArrayLike] = None
 
     @property
     def effective_amplitude(self) -> float:
         return 1.0 if self.amplitude is None else self.amplitude
 
     @staticmethod
     def effective_length(pulse_def: PulseDef, sampling_rate: float) -> float:
```

## laboneq/compiler/scheduler/scheduler.py

```diff
@@ -1,2650 +1,1049 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import copy
+import dataclasses
+import itertools
 import logging
-import math
-from collections import OrderedDict
-from dataclasses import dataclass, field
-from fractions import Fraction
-from itertools import groupby
-from operator import itemgetter
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Union
+from dataclasses import replace
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    FrozenSet,
+    Iterable,
+    List,
+    Optional,
+    Set,
+    Tuple,
+)
 
 import numpy as np
-from box import Box
-from engineering_notation import EngNumber
-from sortedcollections import ValueSortedDict
-from sortedcontainers import SortedDict
 
 from laboneq._observability.tracing import trace
+from laboneq._utils import cached_method
 from laboneq.compiler.common.compiler_settings import CompilerSettings
 from laboneq.compiler.common.device_type import DeviceType
 from laboneq.compiler.common.event_type import EventType
-from laboneq.compiler.common.play_wave_type import PlayWaveType
-from laboneq.compiler.common.pulse_parameters import encode_pulse_parameters
-from laboneq.compiler.common.signal_obj import SignalObj
 from laboneq.compiler.experiment_access.experiment_dao import ExperimentDAO
 from laboneq.compiler.experiment_access.param_ref import ParamRef
-from laboneq.compiler.experiment_access.pulse_def import PulseDef
-from laboneq.compiler.experiment_access.section_graph import SectionGraph
-from laboneq.compiler.scheduler.event_graph import EventGraph, EventRelation, node_info
-from laboneq.compiler.scheduler.event_graph_builder import (
-    ChainElement,
-    EventGraphBuilder,
+from laboneq.compiler.experiment_access.section_info import SectionInfo
+from laboneq.compiler.experiment_access.section_signal_pulse import SectionSignalPulse
+from laboneq.compiler.scheduler.case_schedule import CaseSchedule, EmptyBranch
+from laboneq.compiler.scheduler.interval_schedule import IntervalSchedule
+from laboneq.compiler.scheduler.loop_iteration_schedule import LoopIterationSchedule
+from laboneq.compiler.scheduler.loop_schedule import LoopSchedule
+from laboneq.compiler.scheduler.match_schedule import MatchSchedule
+from laboneq.compiler.scheduler.oscillator_schedule import (
+    OscillatorFrequencyStepSchedule,
+    SweptHardwareOscillator,
+)
+from laboneq.compiler.scheduler.phase_reset_schedule import PhaseResetSchedule
+from laboneq.compiler.scheduler.preorder_map import calculate_preorder_map
+from laboneq.compiler.scheduler.pulse_phase import calculate_osc_phase
+from laboneq.compiler.scheduler.pulse_schedule import (
+    PrecompClearSchedule,
+    PulseSchedule,
 )
+from laboneq.compiler.scheduler.reserve_schedule import ReserveSchedule
+from laboneq.compiler.scheduler.root_schedule import RootSchedule
 from laboneq.compiler.scheduler.sampling_rate_tracker import SamplingRateTracker
+from laboneq.compiler.scheduler.schedule_data import ScheduleData
+from laboneq.compiler.scheduler.section_schedule import SectionSchedule
+from laboneq.compiler.scheduler.utils import (
+    assert_valid,
+    ceil_to_grid,
+    lcm,
+    round_to_grid,
+    to_tinysample,
+)
 from laboneq.core.exceptions import LabOneQException
+from laboneq.core.types.enums import RepetitionMode, SectionAlignment
+
+if TYPE_CHECKING:
+    from laboneq.compiler.common.signal_obj import SignalObj
 
 _logger = logging.getLogger(__name__)
 
 
-@dataclass
-class _PlayWave:
-    id: str
-    signal: str
-    length: float = None
-    offset: Any = None
-    amplitude: Any = None
-    parameterized_with: list = field(default_factory=list)
-    acquire_handle: str = None
-    acquisition_type: list = field(default_factory=list)
-    phase: float = None
-    increment_oscillator_phase: float = None
-    set_oscillator_phase: float = None
-    oscillator_frequency: float = None
-    play_wave_type: PlayWaveType = PlayWaveType.PLAY
-    play_pulse_parameters: Dict[str, Any] = field(default_factory=dict)
-    pulse_pulse_parameters: Dict[str, Any] = field(default_factory=dict)
-    precompensation_clear: bool = field(default=False)
-    markers: Any = None
-
-
-@dataclass
-class _PreambleInserter:
-    event_graph: EventGraph
-    before_loops_id: int
-    loop_step_start_id: int
-    previous_loop_step_end_id: Optional[int]
+@dataclasses.dataclass
+class RepetitionInfo:
+    section: str
+    mode: RepetitionMode
+    time: Optional[float]
 
-    def insert(
-        self,
-        node_ids: Union[int, List[int]],
-        add_before_first_loop_start: bool,
-    ):
-        if not isinstance(node_ids, list):
-            node_ids = [node_ids]
-        for n in node_ids:
-            if self.previous_loop_step_end_id is None:
-                # First loop step: Schedule before/after start of outer looping section
-                if add_before_first_loop_start:
-                    self.event_graph.after_or_at(self.before_loops_id, n)
-                else:
-                    self.event_graph.after_or_at(n, self.before_loops_id)
-            else:
-                # After first loop: Schedule after beginning of new loop step
-                self.event_graph.after_or_at(n, self.previous_loop_step_end_id)
-            self.event_graph.after_or_at(self.loop_step_start_id, n)
-
-
-def _set_playwave_resolved_param(section_pulse, play_wave: _PlayWave, name, value=None):
-    if getattr(section_pulse, name) is not None:
-        setattr(play_wave, name, getattr(section_pulse, name))
-    elif value is not None:
-        setattr(play_wave, name, value)
-    if getattr(section_pulse, name + "_param") is not None:
-        param_ref = ParamRef(getattr(section_pulse, name + "_param"))
-        setattr(play_wave, name, param_ref)
-        play_wave.parameterized_with.append(param_ref)
-
-
-def _assign_playwave_parameters(play_wave, section_pulse, oscillator, length):
-    play_wave.parameterized_with = []
-    _set_playwave_resolved_param(section_pulse, play_wave, "offset")
-    _set_playwave_resolved_param(section_pulse, play_wave, "amplitude")
-    _set_playwave_resolved_param(section_pulse, play_wave, "length", length)
-    _set_playwave_resolved_param(section_pulse, play_wave, "phase")
-    _set_playwave_resolved_param(section_pulse, play_wave, "increment_oscillator_phase")
-    _set_playwave_resolved_param(section_pulse, play_wave, "set_oscillator_phase")
-    if oscillator is None or oscillator.hardware:
-        pass
-    elif oscillator.frequency is not None:
-        play_wave.oscillator_frequency = oscillator.frequency
-    elif oscillator.frequency_param is not None:
-        param_ref = ParamRef(oscillator.frequency_param)
-        play_wave.oscillator_frequency = param_ref
-        play_wave.parameterized_with.append(param_ref)
-
-    play_wave.precompensation_clear = section_pulse.precompensation_clear
-    play_pulse_parameters = section_pulse.play_pulse_parameters
-    pulse_pulse_parameters = section_pulse.pulse_pulse_parameters
-    if play_pulse_parameters is not None:
-        for param, val in play_pulse_parameters.items():
-            if isinstance(val, ParamRef):
-                play_wave.parameterized_with.append(val)
-        play_wave.play_pulse_parameters = play_pulse_parameters
-    if pulse_pulse_parameters is not None:
-        for param, val in pulse_pulse_parameters.items():
-            if isinstance(val, ParamRef):
-                play_wave.parameterized_with.append(val)
-        play_wave.pulse_pulse_parameters = pulse_pulse_parameters
-
-    if section_pulse.acquire_params is not None:
-        play_wave.acquire_handle = section_pulse.acquire_params.handle
-        play_wave.acquisition_type.append(section_pulse.acquire_params.acquisition_type)
+
+# from more_itertools
+def pairwise(iterator):
+    a, b = itertools.tee(iterator)
+    next(b, None)
+    yield from zip(a, b)
 
 
 class Scheduler:
     def __init__(
         self,
         experiment_dao: ExperimentDAO,
         sampling_rate_tracker: SamplingRateTracker,
         signal_objects: Dict[str, SignalObj],
-        clock_settings: Optional[Dict] = None,
+        # For compatibility with old scheduler, remove once we remove that
+        _clock_settings: Optional[Dict] = None,
         settings: Optional[CompilerSettings] = None,
     ):
+        self._schedule_data = ScheduleData(
+            experiment_dao=experiment_dao,
+            settings=settings or CompilerSettings(),
+            sampling_rate_tracker=sampling_rate_tracker,
+            signal_objects=signal_objects,
+        )
         self._experiment_dao = experiment_dao
         self._sampling_rate_tracker = sampling_rate_tracker
-        self._clock_settings = clock_settings or {}
-        self._settings = settings or CompilerSettings()
-        self._event_graph = EventGraph()
-        self._section_grids = {}
-        self._section_events = {}
-
-        self._loop_step_events: Dict[str, Dict[int, Tuple[int, int, int]]] = {}
-
-        self._section_graph_object = SectionGraph.from_dao(self._experiment_dao)
-
-    @trace("scheduler.run()", {"version": "v1"})
-    def run(self):
-        root_sections = self._section_graph_object.root_sections()
-        start_events = self._add_start_events()
-
-        EventGraphBuilder.build_section_structure(
-            self._event_graph, self._section_graph_object, start_events
-        )
-
-        match_case_signals = {}
-        empty_match_case_sections = {}
-        clear_bit_events_of_section = {}
-        for section_node in self._section_graph_object.topologically_sorted_sections():
-
-            parent = self._section_graph_object.parent(section_node)
-            assert parent is not None or section_node in root_sections
-            section_info = self._section_graph_object.section_info(section_node)
-            section_name = section_info.section_id
-
-            section_span = self._event_graph.find_section_start_end(section_name)
-
-            section_start_node = section_span.start
-
-            signals = self._experiment_dao.section_signals(
-                section_info.section_display_name
-            )
-
-            clear_bit_events = []
-            parent_section_trigger_states = set()
-            parent_section_id = section_name
-            while True:
-                parent_section_id = self._experiment_dao.section_parent(
-                    parent_section_id
-                )
-                if parent_section_id is None:
-                    break
-                parent_section_info = self._experiment_dao.section_info(
-                    parent_section_id
-                )
-                for trigger_info in parent_section_info.trigger_output:
-                    state = int(trigger_info["state"])
-                    if state:
-                        parent_section_trigger_states.add(state)
-
-            for trigger_info in section_info.trigger_output:
-                state = int(trigger_info["state"])
-                if state:
-                    for bit in range(2):
-                        bit_mask = 2**bit
-                        if bit_mask & state > 0:
-                            # check if the current bit is controlled by any parent section
-                            # if so, leave it alone
-                            if not any(
-                                [
-                                    parent_statee & bit_mask > 0
-                                    for parent_statee in parent_section_trigger_states
-                                ]
-                            ):
-                                set_bit_event = self._event_graph.add_node(
-                                    event_type=EventType.DIGITAL_SIGNAL_STATE_CHANGE,
-                                    section_name=section_node,
-                                    bit=bit,
-                                    change="SET",
-                                    signal=trigger_info["signal_id"],
-                                )
-                                self._event_graph.after_or_at(
-                                    set_bit_event, section_span.start
-                                )
-                                self._event_graph.after_or_at(
-                                    section_span.end, set_bit_event
-                                )
-                                clear_bit_event = self._event_graph.add_node(
-                                    event_type=EventType.DIGITAL_SIGNAL_STATE_CHANGE,
-                                    section_name=section_node,
-                                    bit=bit,
-                                    change="CLEAR",
-                                    signal=trigger_info["signal_id"],
-                                )
-                                self._event_graph.after_or_at(
-                                    clear_bit_event, section_span.start
-                                )
-                                self._event_graph.after_or_at(
-                                    section_span.end, clear_bit_event
-                                )
-                                clear_bit_events.append(clear_bit_event)
-
-            if section_info.state is not None:
-                if signals:
-                    match_case_signals.setdefault(parent, set()).update(signals)
-                else:
-                    empty_match_case_sections[section_name] = (
-                        parent,
-                        section_start_node,
-                    )
-
-            for signal_id in signals:
-                _logger.debug(
-                    "Considering signal %s in section %s", signal_id, section_name
-                )
-
-                signal_info_main = self._experiment_dao.signal_info(signal_id)
-
-                _logger.debug("signal_info_main =  %s", signal_info_main)
-                play_wave_chain: List[_PlayWave] = []
-
-                is_integration = signal_info_main.signal_type == "integration"
-
-                device_id = signal_info_main.device_id
-
-                sampling_rate = self._sampling_rate_tracker.sampling_rate_for_device(
-                    device_id
-                )
-
-                for section_pulse in self._experiment_dao.section_pulses(
-                    section_info.section_display_name, signal_id
-                ):
-                    pulse_name = section_pulse.pulse_id
-                    pulse_def = None
-                    if pulse_name is not None:
-                        pulse_def = self._experiment_dao.pulse(pulse_name)
-                        play_wave = _PlayWave(
-                            id=pulse_name,
-                            signal=signal_id,
-                            play_wave_type=PlayWaveType.INTEGRATION
-                            if is_integration
-                            else PlayWaveType.PLAY,
-                            markers=section_pulse.markers,
-                        )
-                    else:
-                        play_wave = _PlayWave(
-                            id="DELAY",
-                            signal=signal_id,
-                            play_wave_type=PlayWaveType.DELAY,
-                        )
-
-                    assert signal_id == signal_info_main.signal_id
-
-                    length = PulseDef.effective_length(pulse_def, sampling_rate)
-                    oscillator = self._experiment_dao.signal_oscillator(signal_id)
-                    _assign_playwave_parameters(
-                        play_wave, section_pulse, oscillator, length
-                    )
-
-                    play_wave_chain.append(play_wave)
-                self.add_play_wave_chain(
-                    play_wave_chain,
-                    section_info.section_id,
-                    right_aligned=(section_info.align == "right"),
-                    section_start_node=section_start_node,
-                )
-
-            clear_bit_events_of_section[section_name] = clear_bit_events
-
-        for section_name, clear_bit_events in clear_bit_events_of_section.items():
-            section_span = self._event_graph.find_section_start_end(section_name)
-            for edge in self._event_graph.out_edges(section_span.end):
-                # make sure that the clearing of the trigger event happens after everything else in the section
-                # while also making sure there is a path in the graph from section end -> bit clear node -> section start
-                # so that the event gets properly copied in loops
-                for clear_bit_event in clear_bit_events:
-                    other_node = edge[1]
-                    if other_node != clear_bit_event:
-                        if edge[2]["relation"] == EventRelation.AFTER_OR_AT:
-                            self._event_graph.after_or_at(clear_bit_event, other_node)
-
-        for empty_section, parent in empty_match_case_sections.items():
-            for signal in match_case_signals[parent[0]]:
-                # This is an empty branch of a feedback, but we still want to create
-                # events such that we can play zeros during the duration of that event
-                # via the command table - it needs an entry even when nothing is played.
-
-                signal_info_main = self._experiment_dao.signal_info(signal)
-                sampling_rate = self._sampling_rate_tracker.sampling_rate_for_device(
-                    signal_info_main.device_id
-                )
-                play_zeros = _PlayWave(
-                    id="EMPTY_MATCH_CASE_DELAY",
-                    play_wave_type=PlayWaveType.EMPTY_CASE,
-                    signal=signal,
-                    length=1e-9,
-                )
-                self.add_play_wave_chain(
-                    [play_zeros],
-                    parent_section_name=empty_section,
-                    right_aligned=False,
-                    section_start_node=parent[1],
-                )
-
-        repeat_sections: Dict[str, Scheduler.RepeatSectionsEntry] = {}
-        for section_node in list(
-            reversed(list(self._section_graph_object.topologically_sorted_sections()))
-        ):
-            _logger.debug("Processing section %s", section_node)
-            section_info_1 = self._section_graph_object.section_info(section_node)
-
-            if section_info_1.has_repeat:
-                section_name = section_info_1.section_id
-                _logger.debug("Adding repeat for section %s", section_name)
-                parameters_list = [
-                    {
-                        "id": param["id"],
-                        "start": param["start"],
-                        "step": param["step"],
-                        "values": param["values"],
-                    }
-                    for param in self._experiment_dao.section_parameters(
-                        section_info_1.section_display_name
-                    )
-                ]
-                num_repeats = section_info_1.count
-
-                reset_phase_hw = section_info_1.reset_oscillator_phase
-                reset_phase_sw = (
-                    reset_phase_hw or section_info_1.averaging_type == "hardware"
-                )
-                repeat_sections[section_name] = self.add_repeat(
-                    section_name,
-                    num_repeats,
-                    parameters_list,
-                    reset_phase_sw,
-                    reset_phase_hw,
-                )
-
-        EventGraphBuilder.complete_section_structure(
-            self._event_graph, self._section_graph_object
-        )
-
-        self.generate_loop_events(repeat_sections)
-        self._add_repetition_time_edges()
-        self._sorted_events = self._event_graph.sorted_events()
-        self._add_feedback_time_edges()
-        self.calculate_timing()
-        self.verify_timing()
-        _logger.debug("Calculating play wave parameters")
-        self._calculate_play_wave_parameters()
-
-    def _calculate_play_wave_parameters(self):
-        amplitude_resolution = pow(2, self._settings.AMPLITUDE_RESOLUTION_BITS)
-        parameter_values = {}
-        oscillator_phase_cumulative = {}
-        oscillator_phase_sets = {}
-
-        phase_reset_time = 0.0
-        sorted_events = SortedDict()
-        priority_map = {
-            EventType.SET_OSCILLATOR_PHASE: -5,
-            EventType.PLAY_START: 0,
-            EventType.ACQUIRE_START: 0,
-            EventType.PARAMETER_SET: -15,
-            EventType.INCREMENT_OSCILLATOR_PHASE: -9,
-            EventType.RESET_SW_OSCILLATOR_PHASE: -15,
-        }
-
-        for local_event_id in self._event_timing.keys():
-            event = self._event_graph.node(local_event_id)
-
-            if event["event_type"] in priority_map:
-                key = (event["time"], priority_map[event["event_type"]], event["id"])
-                sorted_events[key] = event
-
-        def make_error_nt_param(param: ParamRef, event):
-            return LabOneQException(
-                f"Parameter {param.param_name} in section {event['section_name']} "
-                f"could not be resolved. "
-                f"Note that only RT sweep parameters are currently supported here."
-            )
-
-        for event in sorted_events.values():
-            if event["event_type"] == EventType.PARAMETER_SET:
-                param_obj = event["parameter"]
-                parameter_values[param_obj["id"]] = self._event_graph.node(event["id"])[
-                    "value"
-                ]
-            if event["event_type"] == EventType.RESET_SW_OSCILLATOR_PHASE:
-                phase_reset_time = event["time"]
-                for signal_id in oscillator_phase_cumulative.keys():
-                    oscillator_phase_cumulative[signal_id] = 0.0
-
-            if event["event_type"] == EventType.INCREMENT_OSCILLATOR_PHASE:
-                signal_id = event["signal"]
-                if signal_id not in oscillator_phase_cumulative:
-                    oscillator_phase_cumulative[signal_id] = 0.0
-                phase_incr = event["increment_oscillator_phase"]
-                if isinstance(phase_incr, ParamRef):
-                    try:
-                        phase_incr = parameter_values[phase_incr.param_name]
-                        event["increment_oscillator_phase"] = phase_incr
-                    except KeyError as e:
-                        raise make_error_nt_param(phase_incr, event) from e
-                oscillator_phase_cumulative[signal_id] += phase_incr
-            if event["event_type"] == EventType.SET_OSCILLATOR_PHASE:
-                signal_id = event["signal"]
-                osc_phase = event["set_oscillator_phase"]
-                if isinstance(osc_phase, ParamRef):
-                    try:
-                        osc_phase = parameter_values[osc_phase.param_name]
-                        event["set_oscillator_phase"] = osc_phase
-                    except KeyError as e:
-                        raise make_error_nt_param(osc_phase, event) from e
-                oscillator_phase_cumulative[signal_id] = osc_phase
-                oscillator_phase_sets[signal_id] = event["time"]
-
-            if event["event_type"] in [EventType.PLAY_START, EventType.ACQUIRE_START]:
-                amplitude = event["amplitude"]
-                if isinstance(amplitude, ParamRef):
-                    _logger.debug(
-                        "Resolving param name %s, parameter_values=%s",
-                        amplitude.param_name,
-                        parameter_values,
-                    )
-                    try:
-                        amplitude = parameter_values[amplitude.param_name]
-                        event["amplitude"] = amplitude
-                    except KeyError as e:
-                        raise make_error_nt_param(amplitude, event) from e
-                    amplitude = (
-                        round(amplitude * amplitude_resolution) / amplitude_resolution
-                    )
+        self._TINYSAMPLE = self._schedule_data.TINYSAMPLE
 
-                    self._event_graph.set_node_attributes(
-                        event["id"], {"amplitude": amplitude}
-                    )
-                if amplitude is not None and abs(amplitude) > 1.0:
-                    raise LabOneQException(
-                        f"Magnitude of amplitude {amplitude} exceeding unity for event {event}"
-                    )
+        self._system_grid = self.grid(*self._experiment_dao.signals())[1]
+        self._root_schedule: Optional[IntervalSchedule] = None
+        self._scheduled_sections = {}
 
-                phase = event["phase"]
-                if isinstance(phase, ParamRef):
-                    try:
-                        phase = parameter_values[phase.param_name]
-                        event["phase"] = phase
-                    except KeyError as e:
-                        raise make_error_nt_param(phase, event) from e
-                    self._event_graph.set_node_attributes(event["id"], {"phase": phase})
+    @trace("scheduler.run()", {"version": "v2"})
+    def run(self, nt_parameters=None):
+        if nt_parameters is None:
+            nt_parameters = {}
+        self._root_schedule = self._schedule_root(nt_parameters)
+        _logger.info("Schedule completed")
 
-                oscillator_frequency = event["oscillator_frequency"]
-                if isinstance(oscillator_frequency, ParamRef):
-                    oscillator_frequency = parameter_values[
-                        oscillator_frequency.param_name
-                    ]
-                    self._event_graph.set_node_attributes(
-                        event["id"], {"oscillator_frequency": oscillator_frequency}
-                    )
+    def generate_event_list(self, expand_loops: bool, max_events: int):
+        event_list = self._start_events()
 
-                play_pulse_parameters = event.get("play_pulse_parameters", {})
-                pulse_pulse_parameters = event.get("pulse_pulse_parameters", {})
-                for k, v in play_pulse_parameters.items():
-                    if isinstance(v, ParamRef):
-                        try:
-                            play_pulse_parameters[k] = parameter_values[v.param_name]
-                        except KeyError as e:
-                            raise make_error_nt_param(v, event) from e
-                for k, v in pulse_pulse_parameters.items():
-                    if isinstance(v, ParamRef):
-                        try:
-                            pulse_pulse_parameters[k] = parameter_values[v.param_name]
-                        except KeyError as e:
-                            raise make_error_nt_param(v, event) from e
-                self._event_graph.set_node_attributes(
-                    event["id"],
-                    {
-                        "play_pulse_parameters": encode_pulse_parameters(
-                            play_pulse_parameters
-                        ),
-                        "pulse_pulse_parameters": encode_pulse_parameters(
-                            pulse_pulse_parameters
-                        ),
-                    },
+        if self._root_schedule is not None:
+            id_tracker = itertools.count()
+            event_list.extend(
+                self._root_schedule.generate_event_list(
+                    start=0,
+                    max_events=max_events,
+                    id_tracker=id_tracker,
+                    expand_loops=expand_loops,
+                    settings=self._schedule_data.settings,
                 )
+            )
 
-                oscillator_phase = None
-                baseband_phase = None
-                signal_id = event["signal"]
-                signal_info = self._experiment_dao.signal_info(signal_id)
-                oscillator_info = self._experiment_dao.signal_oscillator(signal_id)
-                if oscillator_info is not None:
-                    if signal_info.modulation and signal_info.device_type in [
-                        "hdawg",
-                        "shfsg",
-                    ]:
-                        if oscillator_info.frequency_param is not None:
-                            try:
-                                frequency = parameter_values[
-                                    oscillator_info.frequency_param
-                                ]
-                            except KeyError as e:
-                                # HW oscillator sweeps with a NT parameter is fine - the
-                                # controller will take care of it.
-                                if not oscillator_info.hardware:
-                                    raise make_error_nt_param(
-                                        oscillator_info.frequency_param, event
-                                    ) from e
-                        else:
-                            frequency = oscillator_info.frequency
-
-                        incremented_phase = 0.0
-                        if signal_id in oscillator_phase_cumulative:
-                            incremented_phase = oscillator_phase_cumulative[signal_id]
-
-                        if oscillator_info.hardware:
-                            if signal_id in oscillator_phase_sets:
-                                raise Exception(
-                                    f"There are set_oscillator_phase entries for signal '{signal_id}', but oscillator '{oscillator_info.id}' is a hardware oscillator. Setting absolute phase is not supported for hardware oscillators."
-                                )
-                            baseband_phase = incremented_phase
-                        else:
-                            phase_reference_time = phase_reset_time
-                            if signal_id in oscillator_phase_sets:
-                                phase_reference_time = max(
-                                    phase_reset_time, oscillator_phase_sets[signal_id]
-                                )
-                            oscillator_phase = (
-                                event["time"] - phase_reference_time
-                            ) * 2.0 * math.pi * frequency + incremented_phase
-                event_node = self._event_graph.node(event["id"])
-                event_node["oscillator_phase"] = oscillator_phase
-                event_node["baseband_phase"] = baseband_phase
-
-    def _add_repetition_time_edges_for(self, section_name, repetition_time):
-        if repetition_time is None:
-            return
-
-        section_info = self._section_graph_object.section_info(section_name)
+            # assign every event an id
+            for event in event_list:
+                if "id" not in event:
+                    event["id"] = next(id_tracker)
 
-        loop_step_start_events = self._event_graph.find_section_events_by_type(
-            section_name, event_type=EventType.LOOP_STEP_START
-        )
+        # convert time from units of tiny samples to seconds
+        for event in event_list:
+            event["time"] = event["time"] * self._TINYSAMPLE
 
-        loop_step_end_events = {
-            (e["iteration"], e.get("loop_iteration")): e
-            for e in self._event_graph.find_section_events_by_type(
-                section_name, event_type=EventType.LOOP_STEP_END
-            )
-        }
-        right_aligned_collector_events = {}
-        if section_info.align == "right":
-            right_aligned_collector_events = {}
-            for iteration, e in loop_step_end_events.items():
-                for edge in self._event_graph.out_edges(e["id"]):
-                    other_node = self._event_graph.node(edge[1])
-                    if (
-                        other_node["event_type"] == EventType.RIGHT_ALIGNED_COLLECTOR
-                        and other_node["section_name"] == section_name
-                    ):
-                        right_aligned_collector_events[iteration] = other_node
-
-        for iteration_start_event in loop_step_start_events:
-            key = (
-                iteration_start_event["iteration"],
-                iteration_start_event.get("loop_iteration"),
-            )
-            iteration_end_event = loop_step_end_events[key]
-            if key in right_aligned_collector_events:
-                iteration_end_event = right_aligned_collector_events[key]
-
-            self._event_graph.after_exactly(
-                iteration_end_event["id"], iteration_start_event["id"], repetition_time
-            )
-
-        section_span = self._event_graph.find_section_start_end(section_name)
-        loop_iteration_end_event = next(
-            e
-            for e in self._event_graph.find_section_events_by_type(
-                section_name, event_type=EventType.LOOP_ITERATION_END
-            )
-            if not e.get("shadow")
-        )
+        calculate_osc_phase(event_list, self._experiment_dao)
 
-        if section_info.align == "right":
-            right_aligned_collector_of_iteration_end = None
-            for edge in self._event_graph.out_edges(loop_iteration_end_event["id"]):
-                other_node = self._event_graph.node(edge[1])
-                if (
-                    other_node["event_type"] == EventType.RIGHT_ALIGNED_COLLECTOR
-                    and other_node["section_name"] == section_name
-                ):
-                    right_aligned_collector_of_iteration_end = other_node
-            self._event_graph.after_at_least(
-                right_aligned_collector_of_iteration_end["id"],
-                section_span.start,
-                repetition_time,
-            )
-        else:
+        return event_list
 
-            self._event_graph.after_at_least(
-                loop_iteration_end_event["id"], section_span.start, repetition_time
-            )
+    def _start_events(self):
+        retval = []
 
-    def _find_repetition_mode_info(self, section):
-        section_info = self._section_graph_object.section_info(section)
-        if section_info.averaging_mode == "sequential" and (
-            section_info.repetition_mode == "constant"
-            or section_info.repetition_mode == "auto"
-        ):
-            return Box(
+        # Add initial events to reset the NCOs.
+        # Todo (PW): Drop once system tests have been migrated from legacy behaviour.
+        for device_info in self._experiment_dao.device_infos():
+            try:
+                device_type = DeviceType(device_info.device_type)
+            except ValueError:
+                # Not every device has a corresponding DeviceType (e.g. PQSC)
+                continue
+            if not device_type.supports_reset_osc_phase:
+                continue
+            retval.append(
                 {
-                    k: getattr(section_info, k)
-                    for k in [
-                        "repetition_mode",
-                        "repetition_time",
-                        "averaging_mode",
-                        "section_id",
-                    ]
+                    "event_type": EventType.INITIAL_RESET_HW_OSCILLATOR_PHASE,
+                    "device_id": device_info.id,
+                    "duration": device_type.reset_osc_duration,
+                    "time": 0,
                 }
             )
+        return retval
 
-        has_repeating_child = False
-        for child in self._section_graph_object.section_children(section):
-            child_section_info = self._section_graph_object.section_info(child)
-            if child_section_info.has_repeat:
-                has_repeating_child = True
-
-        if not has_repeating_child and (
-            section_info.repetition_mode == "constant"
-            or section_info.repetition_mode == "auto"
-        ):
-            return {
-                k: getattr(section_info, k)
-                for k in [
-                    "repetition_mode",
-                    "repetition_time",
-                    "averaging_mode",
-                    "section_id",
-                ]
-            }
-
-        if not section_info.has_repeat:
+    def event_timing(self, expand_loops=False, max_events: Optional[int] = None):
+        if max_events is None:
+            # inf is not an int, but a good enough substitute!
+            max_events = float("inf")
+        return self.generate_event_list(expand_loops, max_events)
+
+    def _schedule_root(self, nt_parameters: Dict[str, float]) -> Optional[RootSchedule]:
+        root_sections = self._experiment_dao.root_rt_sections()
+        if len(root_sections) == 0:
             return None
 
-        last_parent_section = None
-        while True:
-            parent_section = self._section_graph_object.parent(section)
-            if parent_section is None or parent_section == last_parent_section:
-                return None
-            parent_section_info = self._section_graph_object.section_info(
-                parent_section
-            )
-            if (
-                parent_section_info.repetition_mode == "constant"
-                or parent_section_info.repetition_mode == "auto"
-            ) and parent_section_info.averaging_mode == "cyclic":
-
-                return {
-                    k: getattr(parent_section_info, k)
-                    for k in [
-                        "repetition_mode",
-                        "repetition_time",
-                        "averaging_mode",
-                        "section_id",
-                    ]
-                }
+        self._repetition_info = self._resolve_repetition_time(root_sections)
 
-            last_parent_section = parent_section
+        # todo: we do currently not actually support multiple root sections in the DSL.
+        #  Some of our tests do however do this. For now, we always run all root
+        #  sections *in parallel*.
+        schedules = [self._schedule_section(s, nt_parameters) for s in root_sections]
 
-    def _add_repetition_time_edges(self):
-        for section in self._section_graph_object.sections():
-            repetition_mode_info = self._find_repetition_mode_info(section)
-            if repetition_mode_info is not None:
-                repetition_time = repetition_mode_info.get("repetition_time")
-                if repetition_time is not None:
-                    self._add_repetition_time_edges_for(section, repetition_time)
-
-    def _add_feedback_time_edges(self):
-        @dataclass
-        class AcquiresMatches:
-            acquire_node_id: Optional[int] = None
-            match_node_ids: List[int] = field(default_factory=list)
-            local: bool = False
-
-        event_graph_modified = False
-        acquires = OrderedDict()
-        signals_to_handles = {}
-        for event_id in self._sorted_events:
-            event_data = self._event_graph.node(event_id)
-            event_type = event_data["event_type"]
-            if event_type == "ACQUIRE_START":
-                handle = event_data["acquire_handle"]
-                signal = event_data["signal"]
-                signals_to_handles[signal] = handle
-                acquires.setdefault(handle, []).append(AcquiresMatches())
-            elif event_type == "ACQUIRE_END":
-                try:
-                    handle = signals_to_handles[event_data["signal"]]
-                    last_acquire = acquires[handle][-1]
-                    assert last_acquire.acquire_node_id is None
-                    last_acquire.acquire_node_id = event_id
-                except KeyError:
-                    # Right aligned section - cannot schedule feedback. Error is handled
-                    # later
-                    pass
-            elif event_type == "SECTION_START":
-                handle = event_data.get("handle")
-                if handle is not None:
-                    try:
-                        last_acquire = acquires[handle][-1]
-                        last_acquire.match_node_ids.append(event_id)
-                        last_acquire.local = event_data["local"]
-                        if last_acquire.acquire_node_id is None:
-                            # Right aligned section - cannot schedule feedback.
-                            # Consider passing worst-case timing along for that case
-                            raise LabOneQException(
-                                "Could not compute match section timing "
-                                "- end of acquire came before start. Did you use "
-                                "right-alignment?"
-                            )
+        signals = set()
+        for c in schedules:
+            signals.update(c.signals)
 
-                    except KeyError:
-                        raise LabOneQException(
-                            "No matching acquire found for handle %s; this "
-                            "can also happen if a match section is responding to a "
-                            "right-aligned acquire. "
-                        )
-
-        for acquires_per_handle in acquires.values():
-            for acquire in acquires_per_handle:
-                if acquire.match_node_ids:
-                    event_graph_modified = True
-                    for m in acquire.match_node_ids:
-                        # N.B.: Careful with very short delays, they are difficult to
-                        # represent with playZero/executeTableEntry; thus this delay
-                        # will be at least be 32 samples long
-                        #
-                        if acquire.local:
-                            # todo(JL): Proper timing model; but does it work for right alignment?
-                            # timing = lambda _: 50e-9
-                            timing = lambda _: 0
-                        else:
-                            # todo(JL): Proper timing model; but does it work for right alignment?
-                            timing = lambda _: 500e-9
-                        self._event_graph.after_at_least(
-                            m, acquire.acquire_node_id, timing
-                        )
-        if event_graph_modified:
-            self._sorted_events = self._event_graph.sorted_events()
-
-    @dataclass
-    class RepeatSectionsEntry:
-        section_name: str
-        num_repeats: int
-        nesting_level: int
-        loop_iteration_end_id: int
-        loop_end_id: int
-        parameter_list: List
-        section_span: Any
-        reset_phase_sw: bool
-        reset_phase_hw: bool
-
-    def add_repeat(
-        self,
-        section_name,
-        num_repeats,
-        parameter_list=None,
-        reset_phase_sw=False,
-        reset_phase_hw=False,
-    ) -> RepeatSectionsEntry:
-        if parameter_list is None:
-            parameter_list = []
-        _logger.debug("Adding repeat of %s", section_name)
-        section_span = self._event_graph.find_section_start_end(section_name)
-        nesting_level = len(self._path_to_root(section_name))
-
-        loop_iteration_end_id = self._event_graph.add_node(
-            section_name=section_name,
-            event_type=EventType.LOOP_ITERATION_END,
-            num_repeats=num_repeats,
-            parameter_list=parameter_list,
-            loop_start_node=section_span.start,
-            nesting_level=nesting_level,
-        )
+        root_schedule = RootSchedule(grid=1, signals=signals, children=schedules)  # type: ignore
+        root_schedule.calculate_timing(self._schedule_data, 0, False)
 
-        for edge in self._event_graph.out_edges(section_span.end):
-            if edge[2]["relation"] == EventRelation.AFTER_OR_AT:
-                self._event_graph.after_or_at(loop_iteration_end_id, edge[1])
-
-        loop_end_id = self._event_graph.add_node(
-            section_name=section_name,
-            event_type=EventType.LOOP_END,
-            num_repeats=num_repeats,
-            nesting_level=nesting_level,
-        )
-        self._event_graph.add_edge(
-            loop_end_id, loop_iteration_end_id, relation=EventRelation.AFTER_LOOP
-        )
-
-        self._event_graph.after_or_at(section_span.end, loop_end_id)
-
-        return self.RepeatSectionsEntry(
-            section_name,
-            num_repeats,
-            nesting_level,
-            loop_iteration_end_id,
-            loop_end_id,
-            parameter_list,
-            section_span,
-            reset_phase_sw,
-            reset_phase_hw,
-        )
-
-    def _nodes_which_reference_parameters(self):
-
-        zero_getter = itemgetter(0)
-        param_referencing_nodes = [
-            (e[2].get("delta").param_name, e[0])
-            for e in self._event_graph.edge_list()
-            if isinstance(e[2].get("delta"), ParamRef)
-        ]
-        nodes_of_param_dict = {
-            k: [node[1] for node in g]
-            for k, g in groupby(
-                sorted(param_referencing_nodes, key=zero_getter), zero_getter
-            )
-        }
-        return nodes_of_param_dict
-
-    def add_iteration_control_events(
-        self, repeat_section_entry: RepeatSectionsEntry, first_only=False
-    ):
-        section_name = repeat_section_entry.section_name
-        num_repeats = repeat_section_entry.num_repeats
-        nesting_level = repeat_section_entry.nesting_level
-        loop_iteration_end_id = repeat_section_entry.loop_iteration_end_id
-        loop_end_id = repeat_section_entry.loop_end_id
-        parameter_list = repeat_section_entry.parameter_list
-        section_span = repeat_section_entry.section_span
-        reset_phase_sw = repeat_section_entry.reset_phase_sw
-        reset_phase_hw = repeat_section_entry.reset_phase_hw
-        previous_loop_step_end_id = None
-
-        repeats = num_repeats
-        if first_only and num_repeats > 1:
-            repeats = 1
-
-        nodes_which_reference_params = self._nodes_which_reference_parameters()
-        _logger.debug("Adding iteration events for %s", section_name)
-
-        right_aligned = False
-        if self._section_graph_object.section_info(section_name).align == "right":
-            right_aligned = True
-
-        for iteration in range(repeats):
-            _logger.debug(
-                "Processing iteration %d of num repeats= %d in section %s",
-                iteration,
-                num_repeats,
-                section_name,
-            )
-
-            # Every step of the loop is delimited by 3 events: LOOP_STEP_START (LSS),
-            # LOOP_STEP_BODY_START (LSBS) and LOOP_STEP_END (LSE).
-            # LOOP_STEP_BODY_START marks the end of the loop preamble (P), and the start
-            # of the actual body (B) of the loop. The preamble is used for setting
-            # parameters like the oscillator frequency. Setting these may consume time,
-            # so by having a dedicated time slot, we avoid them bleeding into
-            # neighbouring sections.
-            # The loop is enclosed between section_span.begin (SSB) and section_span.end
-            # (SSE) and ended by LOOP_END (LE), and SUBSECTION_END (SSNE).
-            # LOOP_ITERATION_END (LIE) marks the end of the first loop iteration
-            # The body ends by loop_iteration_end_id; between this and the actual
-            # LOOP_STEP_END, the preamble for the next step can be run
-            #
-            # SSB | LSS -P- LSBS -B- LSE LIE |: LSS -P- LSBS -B- LSE :| SSNE LE SSE
-
-            loop_step_start_id = self._event_graph.add_node(
-                section_name=section_name,
-                event_type=EventType.LOOP_STEP_START,
-                iteration=iteration,
-                nesting_level=nesting_level,
-            )
-
-            loop_step_body_start_id = self._event_graph.add_node(
-                section_name=section_name,
-                event_type=EventType.LOOP_STEP_BODY_START,
-                iteration=iteration,
-                nesting_level=nesting_level,
-            )
-
-            loop_step_end_id = self._event_graph.add_node(
-                section_name=section_name,
-                event_type=EventType.LOOP_STEP_END,
-                iteration=iteration,
-                nesting_level=nesting_level,
-            )
-
-            if section_name not in self._loop_step_events:
-                self._loop_step_events[section_name] = {}
-            self._loop_step_events[section_name][iteration] = (
-                loop_step_start_id,
-                loop_step_body_start_id,
-                loop_step_end_id,
-            )
-
-            preamble_inserter = _PreambleInserter(
-                self._event_graph,
-                previous_loop_step_end_id=previous_loop_step_end_id,
-                before_loops_id=section_span.start,
-                loop_step_start_id=loop_step_start_id,
-            )
-
-            if iteration == 0:
-                # make sure the loop step end at least depends on the same nodes
-                # as the loop iteration end
-                for edge in self._event_graph.out_edges(loop_iteration_end_id):
-                    if edge[2]["relation"] == EventRelation.AFTER_OR_AT:
-                        self._event_graph.after_or_at(loop_step_end_id, edge[1])
-
-                self._event_graph.after_or_at(loop_iteration_end_id, loop_step_end_id)
-
-                subsection_events = [
-                    event
-                    for sublist in [
-                        self._event_graph.find_section_events_by_type(
-                            section_name, event_type
-                        )
-                        for event_type in (
-                            EventType.SUBSECTION_START,
-                            EventType.SUBSECTION_END,
-                            EventType.PLAY_START,
-                            EventType.PLAY_END,
-                            EventType.DELAY_START,
-                            EventType.DELAY_END,
-                        )
-                    ]
-                    for event in sublist
-                ]
-
-                if right_aligned:
-                    right_aligned_collector = next(
-                        e
-                        for e in self._event_graph.find_section_events_by_type(
-                            section_name, EventType.RIGHT_ALIGNED_COLLECTOR
-                        )
-                    )["id"]
-                    self._event_graph.after_or_at(
-                        loop_step_end_id, right_aligned_collector
+        for handle, acquire_pulses in self._schedule_data.acquire_pulses.items():
+            for a, b in pairwise(acquire_pulses):
+                if assert_valid(a.absolute_start) > assert_valid(b.absolute_start):
+                    _logger.warn(
+                        "Topological order of the acquires for handle"
+                        f" {handle} does not match time order."
                     )
 
-                nodes_linked_to_end = [
-                    e[1] for e in self._event_graph.out_edges(section_span.end)
-                ]
+        return root_schedule
 
-                nodes_linked_to_start = [
-                    e[0] for e in self._event_graph.in_edges(section_span.start)
+    def _schedule_section(
+        self,
+        section_id: str,
+        current_parameters: Dict[str, float],
+    ) -> SectionSchedule:
+        """Schedule the given section as the top level.
+
+        ``current_parameters`` represents the parameter context from the parent.
+        """
+
+        try:
+            # todo: do not hash the entire current_parameters dict, but just the param values
+            # todo: reduce key to those parameters actually required by the section
+            return copy.deepcopy(
+                self._scheduled_sections[
+                    (section_id, frozenset(current_parameters.items()))
                 ]
-
-                for subsection_event in subsection_events:
-
-                    subsection_event_id = subsection_event["id"]
-                    if subsection_event_id in nodes_linked_to_end:
-                        _logger.debug(
-                            "Linking subsection event %s to loop_step_end_id=%s",
-                            subsection_event,
-                            loop_step_end_id,
-                        )
-                        self._event_graph.after_or_at(
-                            loop_step_end_id, subsection_event["id"]
-                        )
-                    if subsection_event_id in nodes_linked_to_start:
-                        self._event_graph.after_or_at(
-                            subsection_event["id"], loop_step_start_id
-                        )
-
-            if iteration == 1:
-                self._event_graph.after_or_at(loop_step_start_id, loop_iteration_end_id)
-
-            if iteration == repeats - 1:
-                self._event_graph.after_or_at(loop_end_id, loop_step_end_id)
-
-            self._event_graph.after_or_at(loop_step_body_start_id, loop_step_start_id)
-            self._event_graph.after_or_at(loop_step_end_id, loop_step_body_start_id)
-
-            if previous_loop_step_end_id is not None:
-                self._event_graph.after_or_at(
-                    loop_step_start_id, previous_loop_step_end_id
-                )
-            else:
-                self._event_graph.after_or_at(loop_step_start_id, section_span.start)
-
-            if reset_phase_sw:
-                reset_phase_sw_id = self._event_graph.add_node(
-                    section_name=section_name,
-                    event_type=EventType.RESET_SW_OSCILLATOR_PHASE,
-                    iteration=iteration,
-                )
-                preamble_inserter.insert(
-                    reset_phase_sw_id, add_before_first_loop_start=True
-                )
-
-            if reset_phase_hw:
-                devices = {
-                    self._experiment_dao.device_from_signal(s)
-                    for s in self._experiment_dao.section_signals_with_children(
-                        section_name
-                    )
-                }
-                for device in devices:
-                    device_info = self._experiment_dao.device_info(device)
-                    try:
-                        device_type = DeviceType(device_info.device_type)
-                    except ValueError:
-                        # Not every device has a corresponding DeviceType (e.g. PQSC)
-                        continue
-                    if not device_type.supports_reset_osc_phase:
-                        continue
-                    reset_phase_hw_id = self._event_graph.add_node(
-                        section_name=section_name,
-                        event_type=EventType.RESET_HW_OSCILLATOR_PHASE,
-                        iteration=iteration,
-                        duration=device_type.reset_osc_duration,
-                        device_id=device_info.id,
-                    )
-                    preamble_inserter.insert(
-                        reset_phase_hw_id, add_before_first_loop_start=False
-                    )
-                    self._event_graph.after_at_least(
-                        loop_step_body_start_id,
-                        reset_phase_hw_id,
-                        device_type.reset_osc_duration,
-                    )
-
-            # Find oscillators driven by parameters
-            # TODO(PW): for performance, consider moving out of loop over iterations
-            oscillator_param_lookup = dict()
-            for oscillator in self._experiment_dao.hardware_oscillators():
-                oscillator_id = oscillator.id
-                device_id = oscillator.device_id
-                frequency_param = oscillator.frequency_param
-                if frequency_param is None:
-                    continue
-
-                for signal_id in self._experiment_dao.signals():
-                    oscillator = self._experiment_dao.signal_oscillator(signal_id)
-                    # Not every signal has an oscillator (e.g. flux lines), so check for None
-                    if oscillator is None:
-                        continue
-                    if (
-                        frequency_param in oscillator_param_lookup
-                        and oscillator_param_lookup[frequency_param]["id"]
-                        != oscillator_id
-                    ):
-                        raise LabOneQException(
-                            "Hardware frequency sweep may drive only a single oscillator"
-                        )
-                    if oscillator.id == oscillator_id:
-                        oscillator_param_lookup[frequency_param] = {
-                            "id": oscillator_id,
-                            "device_id": device_id,
-                            "signal_id": signal_id,
-                        }
-
-            for param in parameter_list:
-
-                if param.get("values") is not None:
-                    current_param_value = param["values"][iteration]
-                else:
-                    current_param_value = param["start"] + iteration * param["step"]
-
-                param_set_id = self._event_graph.add_node(
-                    section_name=section_name,
-                    event_type=EventType.PARAMETER_SET,
-                    parameter=param,
-                    iteration=iteration,
-                    value=current_param_value,
-                )
-
-                preamble_inserter.insert(param_set_id, add_before_first_loop_start=True)
-                if iteration == 0:
-
-                    param_referencing_nodes = nodes_which_reference_params.get(
-                        param["id"], []
-                    )
-                    # Make sure that nodes which reference the parameter through parameterized edges
-                    # are scheduled after the parameter setting node
-                    for n in param_referencing_nodes:
-                        self._event_graph.after_or_at(n, param_set_id)
-
-                param_oscillator = oscillator_param_lookup.get(param["id"])
-                if param_oscillator is not None:
-                    osc_freq_start_id = self._event_graph.add_node(
-                        section_name=section_name,
-                        event_type=EventType.SET_OSCILLATOR_FREQUENCY_START,
-                        parameter=param,
-                        iteration=iteration,
-                        value=current_param_value,
-                        device_id=param_oscillator["device_id"],
-                        signal=param_oscillator["signal_id"],
-                    )
-
-                    preamble_inserter.insert(
-                        osc_freq_start_id, add_before_first_loop_start=True
-                    )
-                    device_id = param_oscillator["device_id"]
-                    osc_freq_end_id = self._event_graph.add_node(
-                        section_name=section_name,
-                        event_type=EventType.SET_OSCILLATOR_FREQUENCY_END,
-                        parameter=param,
-                        iteration=iteration,
-                        value=current_param_value,
-                        device_id=device_id,
-                        signal=param_oscillator["signal_id"],
-                    )
-                    device_type = DeviceType(
-                        self._experiment_dao.device_info(device_id).device_type
-                    )
-                    oscillator_set_latency = max(
-                        device_type.oscillator_set_latency,
-                        device_type.min_play_wave / device_type.sampling_rate,
-                    )
-                    self._event_graph.after_at_least(
-                        osc_freq_end_id, osc_freq_start_id, oscillator_set_latency
-                    )
-                    self._event_graph.after_or_at(
-                        loop_step_body_start_id, osc_freq_end_id
-                    )
-
-            previous_loop_step_end_id = loop_step_end_id
-
-        if previous_loop_step_end_id is not None:
-            self._event_graph.after_or_at(section_span.end, previous_loop_step_end_id)
-            self._event_graph.after_or_at(loop_end_id, previous_loop_step_end_id)
-
-    def generate_loop_events(self, repeat_sections: Dict[str, RepeatSectionsEntry]):
-        defined_parameters_of_children = set()
-        for section_name in reversed(
-            list(self._section_graph_object.topologically_sorted_sections())
-        ):
-            section_info = self._section_graph_object.section_info(section_name)
-            if not section_info.has_repeat:
-                _logger.debug("Section %s is not repeated", section_name)
-                continue
-
-            _logger.debug("Adding loop events for section %s", section_name)
-            _logger.debug(section_info)
-
-            iteration_events = self._event_graph.find_section_events_by_type(
-                section_name, event_type=EventType.LOOP_ITERATION_END
-            )
-            _logger.debug("Iteration events:  %s", iteration_events)
-            if len(iteration_events) > 1:
-                _logger.warning("Mulitple iteration events found: %s", iteration_events)
-            iteration_event = iteration_events[0]
-            parameter_list = [
-                param["id"] for param in iteration_event["parameter_list"]
-            ]
-
-            descendants = self._event_graph.descendants(iteration_event["id"])
-            for descendant in descendants:
-                event_data = self._event_graph.node(descendant)
-
-                _logger.debug("Descendant:  %s", node_info(event_data))
-
-            section_span = self._event_graph.find_section_start_end(section_name)
-            section_start_descendants = self._event_graph.descendants(
-                section_span.start
             )
-            section_start_descendants.add(section_span.start)
-
-            for descendant in section_start_descendants:
-                event_data = self._event_graph.node(descendant)
-                _logger.debug("Section start descendant:  %s", node_info(event_data))
+        except KeyError:
+            pass
 
-            between_event_ids = set(descendants).difference(
-                set(section_start_descendants)
-            )
+        section_info = self._experiment_dao.section_info(section_id)
+        sweep_parameters = self._experiment_dao.section_parameters(section_id)
+        for param in sweep_parameters:
+            if "values" not in param or param["values"] is None:
+                param["values"] = (
+                    param["start"] + np.arange(section_info.count) * param["step"]
+                )
+
+        is_loop = section_info.has_repeat
+        if is_loop:
+            schedule = self._schedule_loop(
+                section_id, section_info, current_parameters, sweep_parameters
+            )
+        elif section_info.handle is not None:
+            schedule = self._schedule_match(
+                section_id, section_info, current_parameters
+            )
+        else:  # regular section
+            children_schedules = self._collect_children_schedules(
+                section_id, current_parameters
+            )
+            schedule = self._schedule_children(
+                section_id, section_info, children_schedules
+            )
+
+        if schedule.cacheable:
+            self._scheduled_sections[
+                (section_id, frozenset(current_parameters.items()))
+            ] = schedule
+
+        return schedule
+
+    def _swept_hw_oscillators(
+        self, sweep_parameters: Set[str], signals: Set[str]
+    ) -> Dict[str, SweptHardwareOscillator]:
+        """Collect all hardware oscillators with a frequency swept by one of the
+        given parameters, and that modulate one of the given signals. The keys of the
+        returned dict are the parameter names."""
+        oscillator_param_lookup = dict()
+        for signal in signals:
+            signal_info = self._experiment_dao.signal_info(signal)
+            oscillator = self._experiment_dao.signal_oscillator(signal)
 
-            filtered_between_event_ids = []
-            for between_id in between_event_ids:
-                event_data = self._event_graph.node(between_id)
+            # Not every signal has an oscillator (e.g. flux lines), so check for None
+            if oscillator is None:
+                continue
+            param = oscillator.frequency_param
+            if param in sweep_parameters and oscillator.hardware:
                 if (
-                    event_data["event_type"] in ["LOOP_STEP_START", "LOOP_STEP_END"]
-                    and event_data["section_name"] == section_name
+                    param in oscillator_param_lookup
+                    and oscillator_param_lookup[param].id != oscillator.id
                 ):
-                    _logger.debug("Filtering loop node:  %s", node_info(event_data))
-                else:
-                    filtered_between_event_ids.append(between_id)
-
-            between_event_ids = filtered_between_event_ids
-
-            self._event_graph.set_node_attributes(
-                iteration_event["id"], {"events_in_iteration": list(between_event_ids)}
-            )
-
-            between_events = [
-                self._event_graph.node(between_event_id)
-                for between_event_id in between_event_ids
-            ]
-
-            has_parameterized_events = False
-            referenced_parameters = set()
-            defined_parameters = set()
-            for event_data in between_events:
-                _logger.debug("Between:  %s", node_info(event_data))
-                if event_data["event_type"] == "PARAMETER_SET":
-                    _logger.debug(
-                        "There is a PARAMETER_SET event in between: %s", event_data
+                    raise LabOneQException(
+                        "Hardware frequency sweep may drive only a single oscillator"
                     )
-                    if event_data["section_name"] == section_name:
-                        _logger.debug("And it is in this section %s", event_data)
-                        has_parameterized_events = True
-                    else:
-                        _logger.debug("BUT it is not in this section %s", event_data)
-                    param_obj = event_data["parameter"]
-                    defined_parameters.add(param_obj["id"])
-                if "parameterized_with" in event_data:
-                    parameterized_with = event_data["parameterized_with"]
-                    if parameterized_with is not None:
-                        referenced_parameters.update(parameterized_with)
-
-            missing_parameters = referenced_parameters.difference(set(parameter_list))
-            missing_parameters = missing_parameters.difference(
-                defined_parameters_of_children
-            )
-            _logger.debug(
-                "Section %s has parameter_list %s and refers to parameters %s ,"
-                + " missing parameters %s and defines parameters %s, children defined parameters %s",
-                section_name,
-                parameter_list,
-                referenced_parameters,
-                missing_parameters,
-                defined_parameters,
-                defined_parameters_of_children,
-            )
-
-            # todo (Pol): this is wrong. The previously visited node may have been a
-            # sibling, not a child.
-            defined_parameters_of_children = defined_parameters_of_children.union(
-                set(parameter_list)
-            )
-
-            if (
-                parameter_list == []
-                and not has_parameterized_events
-                and repeat_sections[section_name].num_repeats > 1
-            ):
-                _logger.debug("Compressing events of section %s", section_name)
-                repeat_section = repeat_sections[section_name]
-                self.add_iteration_control_events(repeat_section, first_only=True)
-                _logger.debug(
-                    "Setting compressed to true on node %s",
-                    repeat_section.loop_iteration_end_id,
+                oscillator_param_lookup[param] = SweptHardwareOscillator(
+                    id=oscillator.id, device=signal_info.device_id, signal=signal
                 )
-                self._event_graph.set_node_attributes(
-                    repeat_section.loop_iteration_end_id, {"compressed": True}
-                )
-                compressed = True
-            else:
-                _logger.debug("Not compressing events of section %s", section_name)
 
-                self.add_iteration_control_events(repeat_sections[section_name])
+        return oscillator_param_lookup
 
-                step_start_events = self._event_graph.find_section_events_by_type(
-                    section_name, event_type=EventType.LOOP_STEP_START
-                )
-                _logger.debug(
-                    "Found %d step start events for section %s",
-                    len(step_start_events),
-                    section_name,
-                )
+    def _schedule_loop(
+        self,
+        section_id,
+        section_info: SectionInfo,
+        current_parameters: Dict[str, float],
+        sweep_parameters: List[Dict],
+    ) -> LoopSchedule:
+        """Schedule the individual iterations of the loop ``section_id``.
+
+        Args:
+          section_id: The ID of the loop
+          section_info: Section info of the loop
+          current_parameters: The parameter context from the parent. Does *not* include
+            the sweep parameters of the current loop.
+          sweep_parameters: The sweep parameters of the loop.
+        """
+        repetition_mode, repetition_time = (
+            (self._repetition_info.mode, self._repetition_info.time)
+            if self._repetition_info is not None
+            and self._repetition_info.section == section_id
+            else (None, None)
+        )
 
-                self._event_graph.set_node_attributes(
-                    iteration_event["id"], {"compressed": False}
-                )
-                compressed = False
+        children_schedules = []
+        for param in sweep_parameters:
+            if param["values"] is not None:
+                assert len(param["values"]) >= section_info.count
+        # todo: unroll loops that are too short
+        if len(sweep_parameters) == 0:
+            compressed = section_info.count > 1
+            prototype = self._schedule_loop_iteration(
+                section_id,
+                iteration=0,
+                num_repeats=section_info.count,
+                all_parameters=current_parameters,
+                sweep_parameters=[],
+                swept_hw_oscillators={},
+            )
+            children_schedules.append(prototype)
+        else:
+            compressed = False
+            signals = self._experiment_dao.section_signals_with_children(section_id)
+            swept_hw_oscillators = self._swept_hw_oscillators(
+                {p["id"] for p in sweep_parameters}, signals
+            )
 
-            for (iteration, (_, step_body_id, step_end_id)) in self._loop_step_events[
-                section_name
-            ].items():
-
-                if iteration == 0:
-                    for event in between_events:
-                        self._event_graph.after_or_at(event["id"], step_body_id)
-                elif not compressed:
-                    _logger.debug(
-                        "Copying %d events for iteration %d",
-                        len(between_events),
-                        iteration,
+            for iteration in range(section_info.count):
+                new_parameters = {
+                    param["id"]: (
+                        param["values"][iteration]
+                        if param["values"] is not None
+                        else param["start"] + param["step"] * iteration
                     )
-                    self.copy_iteration_events(
-                        between_events,
-                        section_name,
+                    for param in sweep_parameters
+                }
+                all_parameters = {**current_parameters, **new_parameters}
+
+                children_schedules.append(
+                    self._schedule_loop_iteration(
+                        section_id,
                         iteration,
-                        step_body_id,
-                        step_end_id,
+                        section_info.count,
+                        all_parameters,
+                        sweep_parameters,
+                        swept_hw_oscillators,
                     )
-
-    def copy_iteration_events(
-        self, events, section_name, iteration, step_body, step_end
-    ):
-
-        event_map = {}
-        for event in events:
-            if "section_name" not in event:
-                raise Exception(f"No section name in {event}")
-            new_id = self._event_graph.add_node(
-                section_name=event["section_name"],
-                event_type=event["event_type"],
-                orig_event=event["id"],
-                shadow=True,
-                loop_iteration=section_name + "_" + str(iteration),
-            )
-            _logger.debug("Copying event %s to %s", event, new_id)
-
-            attributes = {}
-            for k, v in event.items():
-                if k != "id":
-                    attributes[k] = copy.deepcopy(v)
-            self._event_graph.set_node_attributes(new_id, attributes)
-            event_map[event["id"]] = new_id
-            self._event_graph.after_or_at(new_id, step_body)
-            self._event_graph.after_or_at(step_end, new_id)
-
-        for event in events:
-            new_node_id = event_map[event["id"]]
-            new_event = self._event_graph.node(new_node_id)
-            start_node_id = new_event.get("loop_start_node")
-            if start_node_id in event_map:
-                mapped_start_id = event_map[start_node_id]
-                self._event_graph.set_node_attributes(
-                    new_node_id, {"loop_start_node": mapped_start_id}
-                )
-
-            events_in_iteration = new_event.get("events_in_iteration")
-            if events_in_iteration is not None:
-                new_events_in_iteration = []
-                for iteration_event_id in events_in_iteration:
-                    if iteration_event_id in event_map:
-                        new_events_in_iteration.append(event_map[iteration_event_id])
-                    else:
-                        new_events_in_iteration.append(iteration_event_id)
-                self._event_graph.set_node_attributes(
-                    new_node_id, {"events_in_iteration": new_events_in_iteration}
                 )
 
-            for edge in self._event_graph.out_edges(event["id"]):
-                other_event = self._event_graph.node(edge[1])
-                new_other_event = None
-                if other_event["id"] in event_map:
-                    new_other_event = event_map[other_event["id"]]
-                if new_other_event is not None:
-                    self._event_graph.add_edge(
-                        new_node_id, new_other_event, relation=edge[2]["relation"]
-                    )
-                    for k, v in edge[2].items():
-                        self._event_graph.set_edge_attribute(
-                            new_node_id, new_other_event, k, v
-                        )
+        schedule = self._schedule_children(section_id, section_info, children_schedules)
+
+        return LoopSchedule.from_section_schedule(
+            schedule,
+            compressed=compressed,
+            sweep_parameters=sweep_parameters,
+            iterations=section_info.count,
+            repetition_mode=repetition_mode,
+            repetition_time=to_tinysample(repetition_time, self._TINYSAMPLE),
+        )
 
-    def add_play_wave_chain(
+    def _schedule_oscillator_frequency_step(
         self,
-        play_wave_list: List[_PlayWave],
-        parent_section_name,
-        right_aligned=False,
-        section_start_node=None,
-    ):
-        section_span = self._event_graph.find_section_start_end(parent_section_name)
-        if section_start_node is None:
-            section_start_node = section_span.start
-
-        chain = []
-        signal = None
-        for i, play_wave in enumerate(play_wave_list):
-
-            chain_element_id = parent_section_name + (play_wave.id or "") + str(i)
-            default_attributes = {
-                "section_name": parent_section_name,
-                "signal": play_wave.signal,
-            }
-            if signal is None:
-                signal = play_wave.signal
-            else:
-                if signal != play_wave.signal:
-                    raise Exception(
-                        f"Getting mixed signals: {signal} and {play_wave.signal}"
-                    )
-
-            if play_wave.precompensation_clear:
-                if right_aligned:
-                    # In principle, there is nothing that would stop us from
-                    # implementing this. But the logic of the event graph is already
-                    # quite complex, and PW doesn't want to strain it any more unless we
-                    # actually need to.
-                    raise LabOneQException(
-                        "Precompensation clear not supported in right aligned sections"
-                    )
-                precompensation_clear_element = ChainElement(
-                    id=chain_element_id + "RESET_PRECOMPENSATION_FILTERS_UNALIGNED",
-                    start_type=EventType.RESET_PRECOMPENSATION_FILTERS_UNALIGNED,
-                    end_type=None,
-                    attributes={
-                        **default_attributes,
-                    },
-                )
-                chain.append(precompensation_clear_element)
+        swept_hw_oscillators: Dict[str, SweptHardwareOscillator],
+        iteration: int,
+        sweep_parameters: List[Dict],
+        signals: Set[str],
+        grid: int,
+        section_id: str,
+    ) -> OscillatorFrequencyStepSchedule:
+        length = 0
+
+        # Include the signals from the loop body proper, so that the oscillator set
+        # is not scheduled in parallel to the loop body (in the unlikely event that
+        # the loop body does not depend on the oscillator's signal)
+        signals = signals.copy()
+
+        swept_oscs_list = []
+        values = []
+        params = []
+        for param in sweep_parameters:
+            osc = swept_hw_oscillators.get(param["id"])
+            if osc is None:
+                continue
+            values.append(param["values"][iteration])
+            swept_oscs_list.append(osc)
+            params.append(param["id"])
+            device_id = osc.device
+            device_info = self._experiment_dao.device_info(device_id)
+            device_type = DeviceType(device_info.device_type)
+            length = max(
+                length,
+                int(device_type.oscillator_set_latency / self._TINYSAMPLE),
+            )
+            signals.add(osc.signal)
+
+        return OscillatorFrequencyStepSchedule(
+            length=length,
+            signals=signals,
+            grid=grid,
+            section=section_id,
+            oscillators=swept_oscs_list,
+            params=params,
+            values=values,
+            iteration=iteration,
+        )
 
-            if play_wave.offset is not None:
-                delay_element = ChainElement(
-                    chain_element_id + "DELAY",
-                    start_type=EventType.DELAY_START,
-                    end_type=EventType.DELAY_END,
-                    length=play_wave.offset,
-                    attributes={**default_attributes, **{"play_wave_id": play_wave.id}},
-                )
-                chain.append(delay_element)
+    @cached_method(8)
+    def _schedule_phase_reset(
+        self,
+        section_id: str,
+        grid: int,
+        signals: FrozenSet[str],
+        hw_signals: FrozenSet[str],
+    ) -> List[PhaseResetSchedule]:
+        reset_sw_oscillators = (
+            len(hw_signals) > 0
+            or self._experiment_dao.section_info(section_id).averaging_type
+            == "hardware"
+        )
 
-            if play_wave.increment_oscillator_phase is not None:
+        if not reset_sw_oscillators and len(hw_signals) == 0:
+            return []
 
-                increment_oscillator_phase_element = ChainElement(
-                    id=chain_element_id + "INCREMENT_OSCILLATOR_PHASE",
-                    start_type=EventType.INCREMENT_OSCILLATOR_PHASE,
-                    end_type=None,
-                    attributes={
-                        **default_attributes,
-                        **{
-                            "increment_oscillator_phase": play_wave.increment_oscillator_phase
-                        },
-                    },
+        length = 0
+        hw_osc_devices = {}
+        for signal in hw_signals:
+            device = self._experiment_dao.device_from_signal(signal)
+            device_type = DeviceType(
+                self._experiment_dao.device_info(device).device_type
+            )
+            if not device_type.supports_reset_osc_phase:
+                continue
+            duration = device_type.reset_osc_duration / self._TINYSAMPLE
+            hw_osc_devices[device] = duration
+            length = max(length, duration)
+            if device_type.lo_frequency_granularity is not None:
+                # The frequency of Grimsel's LO in RF mode is a multiple of 100 MHz.
+                # By aligning the grid with this (10 ns) we make sure the LO's phase is
+                # consistent after the reset of the NCO.
+                df = device_type.lo_frequency_granularity
+                lo_granularity_tinysamples = round(1 / df / self._TINYSAMPLE)
+                grid = lcm(grid, lo_granularity_tinysamples)
+                _logger.info(
+                    f"Phase reset in section '{section_id}' has extended the section's "
+                    f"timing grid to {grid*self._TINYSAMPLE*1e9:.2f} ns, so to be "
+                    f"commensurate with the local oscillator."
                 )
-                chain.append(increment_oscillator_phase_element)
 
-            if play_wave.set_oscillator_phase is not None:
+        hw_osc_devices = [(k, v) for k, v in hw_osc_devices.items()]
+        length = ceil_to_grid(length, grid)
 
-                set_oscillator_phase_element = ChainElement(
-                    id=chain_element_id + "SET_OSCILLATOR_PHASE",
-                    start_type=EventType.SET_OSCILLATOR_PHASE,
-                    end_type=None,
-                    attributes={
-                        **default_attributes,
-                        **{"set_oscillator_phase": play_wave.set_oscillator_phase},
-                    },
-                )
-                chain.append(set_oscillator_phase_element)
+        if reset_sw_oscillators:
+            sw_signals = signals
+        else:
+            sw_signals = ()
 
-            chain_element = ChainElement(
-                chain_element_id,
-                attributes={**default_attributes, **{"play_wave_id": play_wave.id}},
-                start_attributes={},
-                end_attributes={},
+        return [
+            PhaseResetSchedule(
+                grid=grid,
+                length=length,
+                signals={*hw_signals, *sw_signals},
+                section=section_id,
+                hw_osc_devices=hw_osc_devices,
+                reset_sw_oscillators=reset_sw_oscillators,
             )
+        ]
 
-            is_match_case_empty_section = (
-                play_wave.play_wave_type == PlayWaveType.EMPTY_CASE
-            )
-            is_integration = play_wave.play_wave_type == PlayWaveType.INTEGRATION
-            if (
-                play_wave.length is not None
-                or is_integration
-                or is_match_case_empty_section
-            ):
-                chain_element.start_type = EventType.PLAY_START
-                chain_element.end_type = EventType.PLAY_END
-                if is_integration:
-                    chain_element.start_type = EventType.ACQUIRE_START
-                    chain_element.end_type = EventType.ACQUIRE_END
-                elif play_wave.play_wave_type != PlayWaveType.PLAY:
-                    chain_element.start_type = EventType.DELAY_START
-                    chain_element.end_type = EventType.DELAY_END
-
-                chain_element.length = play_wave.length
-                chain_element.start_attributes["parameterized_with"] = [
-                    p.param_name for p in play_wave.parameterized_with
-                ]
-                chain_element.start_attributes["phase"] = play_wave.phase
-                chain_element.start_attributes["amplitude"] = play_wave.amplitude
-                chain_element.start_attributes[
-                    "oscillator_frequency"
-                ] = play_wave.oscillator_frequency
-                chain_element.start_attributes[
-                    "acquire_handle"
-                ] = play_wave.acquire_handle
-                chain_element.start_attributes[
-                    "acquisition_type"
-                ] = play_wave.acquisition_type
-                chain_element.start_attributes[
-                    "play_wave_type"
-                ] = play_wave.play_wave_type.name
-                chain_element.end_attributes[
-                    "play_wave_type"
-                ] = play_wave.play_wave_type.name
-                chain_element.start_attributes[
-                    "play_pulse_parameters"
-                ] = play_wave.play_pulse_parameters
-                chain_element.start_attributes[
-                    "pulse_pulse_parameters"
-                ] = play_wave.pulse_pulse_parameters
-
-                if play_wave.markers is not None:
-                    chain_element.start_attributes["markers"] = [
-                        copy.deepcopy(vars(m)) for m in play_wave.markers
-                    ]
+    def _schedule_loop_iteration(
+        self,
+        section_id: str,
+        iteration: int,
+        num_repeats: int,
+        all_parameters: Dict[str, float],
+        sweep_parameters: List[Dict],
+        swept_hw_oscillators: Dict[str, SweptHardwareOscillator],
+    ) -> LoopIterationSchedule:
+        """Schedule a single iteration of a loop.
+
+        Args:
+            section_id: The loop section.
+            iteration: The iteration to be scheduled
+            num_repeats: The total number of iterations
+            all_parameters: The parameter context. Includes the parameter swept in the loop.
+            sweep_parameters: The parameters swept in this loop.
+            swept_hw_oscillators: The hardware oscillators driven by the sweep parameters.
+        """
+
+        # add child sections
+        signals = set()
+        children_schedules = self._collect_children_schedules(
+            section_id, all_parameters
+        )
 
-                if (
-                    play_wave.play_wave_type != PlayWaveType.DELAY
-                    or play_wave.length is not None
-                    or is_match_case_empty_section
-                ):
-                    chain.append(chain_element)
+        for c in children_schedules:
+            signals.update(c.signals)
 
-        if right_aligned:
-            right_aligned_collector_id = EventGraphBuilder.find_right_aligned_collector(
-                self._event_graph, parent_section_name
-            )
-            if right_aligned_collector_id is None:
-                raise Exception(
-                    f"Found no RIGHT_ALIGNED_COLLECTOR in section {parent_section_name}"
-                )
-            EventGraphBuilder.add_right_aligned_chain(
-                self._event_graph,
-                section_start_node,
-                right_aligned_collector_id,
-                terminal_node_id=section_span.end,
-                chain=chain,
+        section_info = self._experiment_dao.section_info(section_id)
+        hw_osc_reset_signals = set()
+        if section_info.reset_oscillator_phase:
+            # todo: This behaves differently than the legacy scheduler.
+            #  The old scheduler would reset ALL devices in the setup.
+            #  Unfortunately, the section grid of the loop (and hence of the phase
+            #  reset) was still defined by the *section signals*. This would potentially
+            #  lead to problems when resetting an otherwise unused device that cannot
+            #  align with the loop grid.
+            #  The new scheduler does not reset devices with unused signals.
+            for signal in self._experiment_dao.section_signals_with_children(
+                section_id
+            ):
+                osc_info = self._experiment_dao.signal_oscillator(signal)
+                if osc_info is not None and osc_info.hardware:
+                    hw_osc_reset_signals.add(signal)
+
+        for _, osc in swept_hw_oscillators.items():
+            signals.add(osc.signal)
+
+        # escalate the grid to sequencer grid
+        # todo: Currently we do this unconditionally. This is something we might want to
+        #  relax in the future
+        _, grid = self.grid(*signals)
+
+        # Deepcopy here because of caching
+        osc_phase_reset = copy.deepcopy(
+            self._schedule_phase_reset(
+                section_id, grid, frozenset(signals), frozenset(hw_osc_reset_signals)
             )
+        )
 
+        if len(swept_hw_oscillators):
+            osc_sweep = [
+                self._schedule_oscillator_frequency_step(
+                    swept_hw_oscillators,
+                    iteration,
+                    sweep_parameters,
+                    signals,
+                    grid,
+                    section_id,
+                ),
+            ]
         else:
-            terminal_id = section_span.end
-            pull_out_node_id = None
-            added_nodes = EventGraphBuilder.add_chain(
-                self._event_graph,
-                section_start_node,
-                terminal_id,
-                chain,
-                reversed=False,
-                link_last=True,
-            )
-            if pull_out_node_id is not None and len(chain) > 0:
-                last_node_id = added_nodes[len(chain) - 1]["end_node_id"]
-                self._event_graph.after_or_at(last_node_id, pull_out_node_id)
-
-            for added_node in added_nodes.values():
-                node_id = added_node["start_node_id"]
-                node_data = self._event_graph.node(node_id)
-                if (
-                    node_data["event_type"]
-                    == EventType.RESET_PRECOMPENSATION_FILTERS_UNALIGNED
-                ):
-                    aligned_node_id = self._event_graph.add_node(
-                        event_type=EventType.RESET_PRECOMPENSATION_FILTERS,
-                        section_name=node_data["section_name"],
-                        signal_id=node_data["signal"],
-                    )
-                    EventGraphBuilder.add_time_link(
-                        self._event_graph, aligned_node_id, node_id, None, False, False
-                    )
+            osc_sweep = []
 
-    def process_events(self):
-        _logger.debug("**** Event Timing")
-        index = 0
-        for event_id in self._event_timing.keys():
-            event = self._event_graph.node(event_id)
-            if event["event_type"] in [EventType.PLAY_START, EventType.PLAY_END]:
-                event_time = event["time"]
-                event_type = event["event_type"]
-                signal = event["signal"]
-                play_wave_id = event["play_wave_id"]
-                time_beautified = EngNumber(float(event_time))
-                if index < 500:
-                    _logger.debug(
-                        "%s %s %s %s", time_beautified, event_type, signal, play_wave_id
-                    )
-                else:
-                    if index == 501:
-                        _logger.debug("**Event log truncated")
-                    _logger.debug(
-                        "%s %s %s %s", time_beautified, event_type, signal, play_wave_id
-                    )
-            else:
-                event_time = event["time"]
-                event_type = event["event_type"]
-                time_beautified = EngNumber(float(event_time))
-                _logger.debug("%s %s", time_beautified, event_type)
-            index += 1
-
-    @staticmethod
-    def _expand_loop_iterations(
-        event_objects,
-        loop_iteration_ends,
-        loop_iteration_event,
-        start_time,
-        loop_iteration_lengths,
-        offset,
-        event_graph,
-        max_events,
-        events_added_ref,
-        level=0,
-    ):
-        logheader = ""
-        for i in range(level):
-            logheader += "  "
-        section_name = loop_iteration_event["section_name"]
-        _logger.debug(
-            "%sExpanding LOOP_ITERATION_END %s %s, at time %s, offset=%s",
-            logheader,
-            section_name,
-            loop_iteration_event["id"],
-            EngNumber(float(loop_iteration_event["time"])),
-            EngNumber(float(offset)),
+        if osc_phase_reset and osc_phase_reset[0].grid != grid:
+            # On SHFxx, we align the phase reset with the LO granularity (100 MHz)
+            grid = osc_phase_reset[0].grid
+
+        children_schedules = [*osc_phase_reset, *osc_sweep, *children_schedules]
+        schedule = self._schedule_children(
+            section_id, section_info, children_schedules, grid
         )
-        iteration_length = loop_iteration_lengths[section_name]
-        iteration_start_time = loop_iteration_event["time"] - iteration_length
-
-        _logger.debug(
-            "%siteration_length=%s iteration_start_time=%s",
-            logheader,
-            EngNumber(float(iteration_length)),
-            EngNumber(float(iteration_start_time)),
+        return LoopIterationSchedule.from_section_schedule(
+            schedule,
+            iteration=iteration,
+            shadow=iteration > 0,
+            num_repeats=num_repeats,
+            sweep_parameters=sweep_parameters,
         )
-        inner_logheader = logheader + " "
-        expanded = 0
-        for iteration in range(1, loop_iteration_event["num_repeats"]):
-
-            _logger.debug(
-                "%sExpanding iteration %d of iteration event %s at %s  section %s events_in_iteration=%s",
-                logheader,
-                iteration,
-                loop_iteration_event["id"],
-                EngNumber(float(loop_iteration_event["time"])),
-                section_name,
-                loop_iteration_event["events_in_iteration"],
-            )
-
-            for orig_event_id in loop_iteration_event["events_in_iteration"]:
-
-                orig_event = event_graph.node(orig_event_id)
-                shadow_event = copy.deepcopy(orig_event)
-                shadow_event["shadow"] = True
-                shadow_event["orig_event"] = orig_event_id
-                shadow_event["iteration"] = iteration
-                shadow_event["exp_iteration"] = iteration
-                shadow_event["id"] = orig_event_id + 10000
-                shadow_event["iterating_section_name"] = section_name
-                shadow_event["iterating_event_id"] = loop_iteration_event["id"]
-
-                relative_time = orig_event["time"] - iteration_start_time
-                shadow_event["shadow_sequence"] = events_added_ref[0]
-
-                new_time = (
-                    iteration_length * iteration
-                    + relative_time
-                    + iteration_start_time
-                    + offset
-                )
-
-                _logger.debug(
-                    "%sCopying %s %s has time of %s and relative time of %s, start time is %s; offset is %f moving to %s",
-                    inner_logheader,
-                    orig_event["id"],
-                    orig_event["event_type"],
-                    EngNumber(float(orig_event["time"])),
-                    EngNumber(float(relative_time)),
-                    EngNumber(float(start_time)),
-                    offset,
-                    EngNumber(float(new_time)),
-                )
-                shadow_event["time"] = new_time
-                event_objects.append(shadow_event)
-                expanded += 1
-                events_added_ref[0] += 1
-                if max_events is not None and events_added_ref[0] >= max_events:
-                    _logger.debug(
-                        "%sTruncating events at %d", inner_logheader, max_events
-                    )
-                    break
-                if (
-                    orig_event["event_type"] == "LOOP_ITERATION_END"
-                    and orig_event["section_name"] != section_name
-                    and orig_event.get("compressed")
-                ):
 
-                    inner_offset = loop_iteration_event[
-                        "time"
-                    ] + loop_iteration_lengths[section_name] * (iteration - 1)
-                    _logger.debug(
-                        "%sDescending a level for iteration %d of iteration event %s  section %s",
-                        inner_logheader,
-                        iteration,
-                        loop_iteration_event["id"],
-                        section_name,
-                    )
-                    Scheduler._expand_loop_iterations(
-                        event_objects,
-                        loop_iteration_ends,
-                        orig_event,
-                        start_time=orig_event["time"]
-                        - loop_iteration_lengths[orig_event["section_name"]],
-                        loop_iteration_lengths=loop_iteration_lengths,
-                        offset=inner_offset,
-                        event_graph=event_graph,
-                        max_events=max_events,
-                        events_added_ref=events_added_ref,
-                        level=level + 1,
-                    )
-                    if max_events is not None and events_added_ref[0] >= max_events:
-                        _logger.debug(
-                            "%sTruncating events at %d", inner_logheader, max_events
-                        )
-                        break
-            if max_events is not None and events_added_ref[0] >= max_events:
-                _logger.debug("%sTruncating events at %d", inner_logheader, max_events)
-                break
+    def _schedule_children(
+        self, section_id, section_info, children: List[IntervalSchedule], grid=1
+    ) -> SectionSchedule:
+        """Schedule the given children of a section, arranging them in the required
+        order.
+
+        The final grid of the section is chosen to be commensurate (via LCM) with all
+        the children's grids. By passing a value for the `grid`argument, the caller can
+        additionally enforce a grid. The default value (`grid=1`) does not add any
+        restrictions beyond those imposed by the children. In addition, escalation to
+        the system grid can be enforced via the DSL.
+        """
+        right_align = section_info.align == SectionAlignment.RIGHT.value
+        signals = set()
+        for c in children:
+            signals.update(c.signals)
+
+        signals.update(self._experiment_dao.section_signals(section_id))
+        play_after = section_info.play_after or []
+        if isinstance(play_after, str):
+            play_after = [play_after]
+
+        signal_grid, sequencer_grid = self.grid(*signals)
+
+        signal_grids = {self.grid(s)[0] for s in signals}
+        if section_info.on_system_grid:
+            grid = lcm(grid, self._system_grid)
+        if len(signal_grids) > 1:
+            # two different sample rates -> escalate to sequencer grid
+            grid = lcm(grid, sequencer_grid)
+        else:
+            grid = lcm(grid, signal_grid)
 
-        _logger.debug(
-            "%sExpanded %d events for  LOOP_ITERATION_END %s",
-            logheader,
-            expanded,
-            loop_iteration_event["id"],
+        trigger_output = self._compute_trigger_output(section_info)
+        if len(trigger_output):
+            grid = lcm(grid, sequencer_grid)
+
+        schedule = SectionSchedule(
+            grid=grid,
+            sequencer_grid=sequencer_grid,
+            length=to_tinysample(section_info.length, self._TINYSAMPLE),
+            signals=signals,
+            children=children,
+            play_after=play_after,
+            right_aligned=right_align,
+            section=section_id,
+            trigger_output=trigger_output,
         )
 
-    def _events_ordered(self) -> Iterator[Any]:
-        for event_id in self._event_timing.keys():
-            event = self._event_graph.node(event_id)
-            yield event
-
-    @staticmethod
-    def _calc_loop_iteration_info(events_ordered):
-        loop_iteration_ends = {}
-        loop_iteration_lengths = {}
-        loop_starts = {}
-        for event in events_ordered:
-            section_name = event.get("section_name")
-            if event["event_type"] == "LOOP_ITERATION_END":
-                if section_name not in loop_iteration_ends:
-                    loop_iteration_ends[section_name] = event
-                    loop_iteration_lengths[section_name] = (
-                        event["time"] - loop_starts[section_name]
-                    )
+        return schedule
 
-            if event["event_type"] == "SECTION_START":
-                existing_start = None
-                if section_name in loop_starts:
-                    existing_start = loop_starts[section_name]
-                if existing_start is None or event["time"] < existing_start:
-                    loop_starts[section_name] = event["time"]
-        return loop_iteration_ends, loop_iteration_lengths, loop_starts
-
-    def event_timing(self, expand_loops=True, max_events=None) -> List[Any]:
-
-        events_added_ref = [0]
-        (
-            loop_iteration_ends,
-            loop_iteration_lengths,
-            loop_starts,
-        ) = self._calc_loop_iteration_info(self._events_ordered())
-        _logger.debug("Iteration lengths: %s", loop_iteration_lengths)
-        too_short = set()
-        for section, event in loop_iteration_ends.items():
-            start_time = loop_starts[section]
-            section_length = event["time"] - start_time
-            section_devices = set()
-            for signal in self._experiment_dao.section_signals_with_children(section):
-                section_devices.add(
-                    DeviceType(self._experiment_dao.signal_info(signal).device_type)
-                )
-            for device in section_devices:
-                sampling_rate = device.sampling_rate
-                if device == DeviceType.HDAWG:
-                    sampling_rate = (
-                        DeviceType.HDAWG.sampling_rate_2GHz
-                        if self._clock_settings["use_2GHz_for_HDAWG"]
-                        else DeviceType.HDAWG.sampling_rate
+    def _schedule_pulse(
+        self,
+        pulse: SectionSignalPulse,
+        section: str,
+        current_parameters: Dict[str, float],
+    ) -> PulseSchedule:
+
+        # todo: add memoization
+
+        grid, _ = self.grid(pulse.signal_id)
+
+        def resolve_value_or_parameter(name, default):
+            value = default
+            param_name = name + "_param"
+            if getattr(pulse, name) is not None:
+                value = getattr(pulse, name)
+            elif getattr(pulse, param_name) is not None:
+                try:
+                    value = current_parameters[getattr(pulse, param_name)]
+                except KeyError as e:
+                    raise LabOneQException(
+                        f"Parameter '{name}' requested outside of sweep. "
+                        "Note that only RT sweep parameters are currently supported here."
+                    ) from e
+            return value
+
+        offset = resolve_value_or_parameter("offset", 0.0)
+        length = resolve_value_or_parameter("length", None)
+        if length is None:
+            pulse_def = self._experiment_dao.pulse(pulse.pulse_id)
+            if pulse_def is not None:
+                assert pulse_def.length is None
+                if pulse_def.samples is None:
+                    raise LabOneQException(
+                        f"Cannot determine length of pulse '{pulse.pulse_id}' in section "
+                        f"'{section}'. Either specify the length at the pulse definition, "
+                        f"when playing the pulse, or by specifying the samples."
                     )
-                section_length_samples = section_length * sampling_rate
-                if section_length_samples < device.min_play_wave:
-                    too_short.add(section)
-        if not expand_loops:
-            _logger.debug(
-                "Sections %s are too short, will expand even though expand_loops is false",
-                list(too_short),
-            )
-
-        event_objects: List[Any] = []
-
-        for event in self._events_ordered():
-            _logger.debug("event: %s", event)
-            if (
-                event["event_type"] == EventType.LOOP_ITERATION_END
-                and "compressed" in event
-                and event["compressed"]
-                and (expand_loops or event["section_name"] in too_short)
-            ):
-                event_copy = copy.deepcopy(event)
-                event_copy["compressed"] = False
-                event_copy["expanded"] = True
-
-                event_objects.append(event_copy)
-                events_added_ref[0] += 1
-                if max_events is not None and events_added_ref[0] >= max_events:
-                    _logger.debug("Truncating events at %d", max_events)
-                    break
-                Scheduler._expand_loop_iterations(
-                    event_objects,
-                    loop_iteration_ends,
-                    event,
-                    loop_starts[event["section_name"]],
-                    loop_iteration_lengths,
-                    0,
-                    self._event_graph,
-                    max_events,
-                    events_added_ref,
-                )
+                length = len(pulse_def.samples) * grid * self._TINYSAMPLE
             else:
-                event_objects.append(copy.copy(event))
-        for event_object in event_objects:
-            event_object["accurate_time"] = repr(event_object["time"])
-            event_object["time"] = float(event_object["time"])
-            if "parameter" in event_object:
-                event_object["parameter"] = {"id": event_object["parameter"].get("id")}
-            if "parameter_list" in event_object:
-                event_object["parameter_list"] = [
-                    {"id": p.get("id")} for p in event_object["parameter_list"]
-                ]
+                assert offset is not None
+                length = 0.0
 
-        event_objects = list(
-            sorted(
-                event_objects,
-                key=lambda x: (
-                    round(x.get("time") * 100e9),
-                    x.get("exp_iteration") or 0,
-                ),
+        amplitude = resolve_value_or_parameter("amplitude", 1.0)
+        if abs(amplitude) > 1.0 + 1e-9:
+            raise LabOneQException(
+                f"Magnitude of amplitude {amplitude} exceeding unity for pulse "
+                f"'{pulse.pulse_id}' on signal '{pulse.signal_id}' in section '{section}'"
             )
+        phase = resolve_value_or_parameter("phase", 0.0)
+        set_oscillator_phase = resolve_value_or_parameter("set_oscillator_phase", None)
+        increment_oscillator_phase = resolve_value_or_parameter(
+            "increment_oscillator_phase", None
         )
 
-        return event_objects
-
-    def calculate_timing(self):
-        (
-            event_times,
-            event_times_tiny_samples,
-        ) = self._calculate_timing_for_graph(self._event_graph)
-
-        repetition_mode_auto_sections = []
-        if self._section_graph_object is not None:
-            for section in self._section_graph_object.sections():
-                repetition_mode_info = self._find_repetition_mode_info(section)
-                if (
-                    repetition_mode_info is not None
-                    and repetition_mode_info.get("repetition_mode") == "auto"
-                ):
-                    repetition_mode_auto_sections.append(section)
+        def resolve_pulse_params(params: Dict[str, Any]):
+            for param, value in params.items():
+                if isinstance(value, ParamRef):
+                    try:
+                        resolved = current_parameters[value.param_name]
+                    except KeyError as e:
+                        raise LabOneQException(
+                            f"Pulse '{pulse.pulse_id}' in section '{section}' requires "
+                            f"parameter '{param}' which is not available. "
+                            f"Note that only RT sweep parameters are currently supported here."
+                        ) from e
+                    params[param] = resolved
+
+        pulse_pulse_params = None
+        if pulse.pulse_pulse_parameters is not None:
+            pulse_pulse_params = pulse.pulse_pulse_parameters.copy()
+            resolve_pulse_params(pulse_pulse_params)
+
+        play_pulse_params = None
+        if pulse.play_pulse_parameters is not None:
+            play_pulse_params = pulse.play_pulse_parameters.copy()
+            resolve_pulse_params(play_pulse_params)
+
+        scheduled_length = length + offset
+
+        length_int = round_to_grid(scheduled_length / self._TINYSAMPLE, grid)
+        offset_int = round_to_grid(offset / self._TINYSAMPLE, grid)
+
+        osc = self._experiment_dao.signal_oscillator(pulse.signal_id)
+        if osc is None:
+            freq = None
+        elif not osc.hardware and osc.frequency_param is not None:
+            try:
+                freq = current_parameters[osc.frequency_param]
+            except KeyError as e:
+                raise LabOneQException(
+                    f"Playback of pulse '{pulse.pulse_id}' in section '{section} "
+                    f"requires the parameter '{osc.frequency_param}' to set the frequency."
+                ) from e
+        elif osc is None or osc.hardware:
+            freq = None
+        else:
+            freq = osc.frequency if osc is not None else None
 
-            if len(repetition_mode_auto_sections) > 0:
-                for repetition_mode_auto_section in repetition_mode_auto_sections:
-                    loop_step_start_events = (
-                        self._event_graph.find_section_events_by_type(
-                            repetition_mode_auto_section,
-                            event_type=EventType.LOOP_STEP_START,
-                        )
-                    )
-                    loop_step_end_events = {
-                        (e["iteration"], e.get("loop_iteration")): e
-                        for e in self._event_graph.find_section_events_by_type(
-                            repetition_mode_auto_section,
-                            event_type=EventType.LOOP_STEP_END,
-                        )
-                    }
-                    max_time = 0
-                    max_iteration = None
-                    for iteration_start_event in loop_step_start_events:
-                        iteration_end_event = loop_step_end_events[
-                            (
-                                iteration_start_event["iteration"],
-                                iteration_start_event.get("loop_iteration"),
-                            )
-                        ]
-                        current_time = (
-                            event_times_tiny_samples[iteration_end_event["id"]]
-                            - event_times_tiny_samples[iteration_start_event["id"]]
-                        )
-                        if current_time > max_time:
-                            max_time = current_time
-                            max_iteration = iteration_end_event["id"]
+        signal_info = self._experiment_dao.signal_info(pulse.signal_id)
+        is_acquire = signal_info.signal_type == "integration"
+        markers = pulse.markers
+
+        return PulseSchedule(
+            grid=grid,
+            length=length_int,
+            signals={pulse.signal_id},
+            pulse=pulse,
+            section=section,
+            amplitude=amplitude,
+            phase=phase,
+            offset=offset_int,
+            set_oscillator_phase=set_oscillator_phase,
+            increment_oscillator_phase=increment_oscillator_phase,
+            oscillator_frequency=freq,
+            play_pulse_params=play_pulse_params,
+            pulse_pulse_params=pulse_pulse_params,
+            is_acquire=is_acquire,
+            markers=markers,
+        )
 
-                    section_span = self._event_graph.find_section_start_end(
-                        repetition_mode_auto_section
-                    )
-                    loop_iteration_end_event = next(
-                        e
-                        for e in self._event_graph.find_section_events_by_type(
-                            repetition_mode_auto_section,
-                            event_type=EventType.LOOP_ITERATION_END,
-                        )
-                        if not e.get("shadow")
-                    )
-                    current_time = (
-                        event_times_tiny_samples[loop_iteration_end_event["id"]]
-                        - event_times_tiny_samples[section_span.start]
-                    )
-                    if current_time > max_time:
-                        max_time = current_time
-                        max_iteration = loop_iteration_end_event["id"]
-
-                    max_time = max_time * self._settings.TINYSAMPLE
-                    section_grid = self.section_grid(repetition_mode_auto_section)
-                    max_time_raw = max_time
-                    max_time = math.ceil(max_time / section_grid) * section_grid
-
-                    _logger.debug(
-                        "Max iteration time for section %s: %f, max_time_raw=%f max_iteration=%d",
-                        repetition_mode_auto_section,
-                        max_time,
-                        max_time_raw,
-                        max_iteration,
-                    )
-                    self._add_repetition_time_edges_for(
-                        repetition_mode_auto_section, max_time
-                    )
-                _logger.debug(
-                    "Performing second scheduling pass because of sections %s with repetition_mode auto",
-                    repetition_mode_auto_sections,
+    def _schedule_match(
+        self,
+        section_id: str,
+        section_info: SectionInfo,
+        current_parameters: Dict[str, float],
+    ) -> MatchSchedule:
+
+        dao = self._schedule_data.experiment_dao
+        children_schedules = []
+        section_children = dao.direct_section_children(section_id)
+        if len(section_children) == 0:
+            raise LabOneQException("Must provide at least one branch option")
+        for case_section in section_children:
+            children_schedules.append(
+                self._schedule_case(case_section, current_parameters)
+            )
+
+        signals = set()
+        for c in children_schedules:
+            signals.update(c.signals)
+        _, grid = self.grid(*signals)
+
+        for i, cs in enumerate(children_schedules):
+            if not cs.children:  # empty branch
+                children_schedules[i] = EmptyBranch(
+                    grid=grid,
+                    sequencer_grid=grid,
+                    signals=signals,
+                    right_aligned=False,
+                    section=cs.section,
+                    state=cs.state,
                 )
-                (
-                    event_times,
-                    event_times_tiny_samples,
-                ) = self._calculate_timing_for_graph(self._event_graph)
-
-        for event_id, time in event_times.items():
-            self._event_graph.node(event_id)["time"] = time
-
-        self._event_timing = ValueSortedDict()
-        sequence_nr = 0
-        for event_id in self._sorted_events:
-            event_data = self._event_graph.node(event_id)
-            event_data["sequence_nr"] = sequence_nr
-            event_time = float(event_data["time"])
-            event_data["time"] = event_time
-            self._event_timing[event_id] = (event_time, sequence_nr)
-            sequence_nr += 1
-
-        _logger.debug("Event times calculated")
-
-    def _calculate_timing_for_graph(self, event_graph: EventGraph):
-        event_times = {}
-        parameter_change_times = SortedDict()
-
-        def parameter_value(param_id, at_time):
-            latest_value = None
-            latest_time = None
-            for k, v in parameter_change_times.items():
-                if k[0] == param_id and at_time >= k[1]:
-                    if latest_value is None or (
-                        latest_time is None or k[1] >= latest_time
-                    ):
-                        latest_value = v
-                        latest_time = k[1]
-            return latest_value
 
-        TINYSAMPLE = self._settings.TINYSAMPLE
+        assert section_info.handle is not None
+        handle: str = section_info.handle
+        local: bool = section_info.local
+        try:
+            acquire_signal = dao.acquisition_signal(handle)
+        except KeyError as e:
+            raise LabOneQException(f"No acquisition with handle '{handle}'") from e
+        acquire_device = dao.device_from_signal(acquire_signal)
+        match_devices = {dao.device_from_signal(s) for s in signals}
+
+        # todo: this is a brittle check for SHFQC
+        local_feedback_allowed = match_devices == {f"{acquire_device}_sg"}
+
+        if local is None:
+            local = local_feedback_allowed
+        elif local and not local_feedback_allowed:
+            raise LabOneQException(
+                f"Local feedback not possible across devices {acquire_device} and {', '.join(match_devices)}"
+            )
 
-        iteration_ends = {}
+        play_after = section_info.play_after or []
+        if isinstance(play_after, str):
+            play_after = [play_after]
+
+        compressed_loop_grid = round(
+            (
+                (8 if local else 200)
+                / self._sampling_rate_tracker.sampling_rate_for_device(acquire_device)
+                / self._TINYSAMPLE
+            )
+        )
 
-        for event_id in self._sorted_events:
-            has_exactly_constraint = False
+        return MatchSchedule(
+            grid=grid,
+            length=to_tinysample(section_info.length, self._schedule_data.TINYSAMPLE),
+            sequencer_grid=grid,
+            signals=signals,
+            children=children_schedules,
+            right_aligned=False,
+            section=section_id,
+            play_after=play_after,
+            handle=handle,
+            local=local,
+            compressed_loop_grid=compressed_loop_grid,
+        )
 
-            event_data = event_graph.node(event_id)
+    def _schedule_case(self, section_id, current_parameters) -> CaseSchedule:
+        try:
+            # todo: do not hash the entire current_parameters dict, but just the param values
+            # todo: reduce key to those parameters actually required by the section
+            return copy.deepcopy(
+                self._scheduled_sections[
+                    (section_id, frozenset(current_parameters.items()))
+                ]
+            )
+        except KeyError:
+            pass
 
-            if (
-                event_data["event_type"] == "LOOP_ITERATION_END"
-                and "compressed" in event_data
-                and event_data["compressed"]
-            ):
-                iteration_ends[event_data["section_name"]] = event_data
+        section_info = self._schedule_data.experiment_dao.section_info(section_id)
 
-            event_time = 0
-            earliest_event_time = 0
-            latest_event_time = None
-
-            if event_data["event_type"] in ["LOOP_END", "LOOP_STEP_END"]:
-                if event_data["section_name"] in iteration_ends:
-                    iteration_end = iteration_ends[event_data["section_name"]]
-                    start_time = event_times[iteration_end["loop_start_node"]]
-
-                    end_time = event_times[iteration_end["id"]]
-                    iteration_length = end_time - start_time
-                    if event_data["event_type"] == "LOOP_STEP_END":
-                        loop_length = (event_data["iteration"] + 1) * iteration_length
-                    else:
-                        loop_length = iteration_end["num_repeats"] * iteration_length
-                    loop_end_time = start_time + loop_length
-                    earliest_event_time = max(earliest_event_time, loop_end_time)
-
-            early_reference = None
-            late_reference = None
-            before_reference_time = None
-
-            for _, other_event_id, edge in event_graph.out_edges(event_id):
-                other_event = event_graph.node(other_event_id)
-                other_time = event_times[other_event["id"]]
-                if edge["relation"] == EventRelation.USES_EARLY_REFERENCE:
-                    early_reference = other_time
-
-                elif edge["relation"] == EventRelation.USES_LATE_REFERENCE:
-                    late_reference = other_time
-
-                elif edge["relation"] == EventRelation.AFTER_OR_AT:
-                    event_time = max(other_time, event_time)
-                    earliest_event_time = max(earliest_event_time, event_time)
-
-                elif edge["relation"] == EventRelation.AFTER_AT_LEAST:
-                    delay_time = edge["delta"]
-                    if isinstance(delay_time, ParamRef):
-                        delay_time = parameter_value(delay_time.param_name, other_time)
-                    elif callable(delay_time):
-                        delay_time = delay_time(other_time * TINYSAMPLE)
-
-                    # todo (Pol): this causes off-by-one errors!
-                    delay_time_tinysamples = math.floor(delay_time / TINYSAMPLE)
-                    delayed_event_time = other_time + delay_time_tinysamples
-                    earliest_event_time = max(earliest_event_time, delayed_event_time)
-                    if delayed_event_time > event_time:
-                        event_time = delayed_event_time
-
-                elif edge["relation"] == EventRelation.AFTER_EXACTLY:
-                    has_exactly_constraint = True
-                    delay_time = edge["delta"]
-                    if isinstance(delay_time, ParamRef):
-                        delay_time = parameter_value(delay_time.param_name, other_time)
-                    elif callable(delay_time):
-                        delay_time = delay_time(other_time * TINYSAMPLE)
-                    # todo (Pol): is this intended behavior?
-                    delay_time_tinysamples = math.floor(delay_time / TINYSAMPLE)
-
-                    delayed_event_time = other_time + delay_time_tinysamples
-                    earliest_event_time = max(earliest_event_time, delayed_event_time)
-                    if latest_event_time is None:
-                        latest_event_time = delayed_event_time
-                    else:
-                        latest_event_time = min(delayed_event_time, latest_event_time)
-
-                elif edge["relation"] == EventRelation.BEFORE_AT_LEAST:
-                    delay_time = edge["delta"]
-                    if isinstance(delay_time, ParamRef):
-                        delay_time = parameter_value(delay_time.param_name, other_time)
-                    elif callable(delay_time):
-                        delay_time = delay_time(other_time * TINYSAMPLE)
-                    # todo (Pol): is this intended behavior?
-                    delayed_event_time = other_time - math.floor(
-                        delay_time / TINYSAMPLE
-                    )
-                    if latest_event_time is None:
-                        latest_event_time = delayed_event_time
-                    else:
-                        latest_event_time = min(delayed_event_time, latest_event_time)
-
-                elif edge["relation"] == EventRelation.BEFORE_OR_AT:
-                    if latest_event_time is not None:
-                        latest_event_time = min(latest_event_time, other_time)
-                    else:
-                        latest_event_time = other_time
+        assert not section_info.has_repeat  # case must not be a loop
+        assert section_info.handle is None
+        state = section_info.state
+        assert state is not None
 
-                elif edge["relation"] == EventRelation.RELATIVE_BEFORE:
-                    before_reference_time = other_time
+        children_schedules = self._collect_children_schedules(
+            section_id, current_parameters
+        )
+        for cs in children_schedules:
+            if not isinstance(cs, PulseSchedule):
+                raise LabOneQException(
+                    "Only pulses, not sections, are allowed inside a case"
+                )
+        # We don't want any branches that are empty, but we don't know yet what signals
+        # the placeholder should cover. So we defer the creation of placeholders to
+        # `_schedule_match()`.
+        schedule = self._schedule_children(section_id, section_info, children_schedules)
+        schedule = CaseSchedule.from_section_schedule(schedule, state)
+        if schedule.cacheable:
+            self._scheduled_sections[
+                (section_id, frozenset(current_parameters.items()))
+            ] = schedule
+
+        return schedule
+
+    def _schedule_precomp_clear(self, pulse: PulseSchedule):
+        signal = pulse.pulse.signal_id
+        _, grid = self.grid(signal)
+        # The precompensation clearing overlaps with a 'pulse' on the same signal,
+        # whereas regular scheduling rules disallow this. For this reason we do not
+        # assign a signal to the precomp schedule, and pass `frozenset()` instead.
+        return PrecompClearSchedule(
+            grid=grid,
+            length=0,
+            pulse=pulse,
+        )
 
-            if (
-                early_reference is not None
-                and late_reference is not None
-                and before_reference_time is not None
-            ):
-                if latest_event_time is None:
-                    latest_event_time = before_reference_time - (
-                        late_reference - early_reference
-                    )
-                else:
-                    latest_event_time = min(
-                        latest_event_time,
-                        before_reference_time - (late_reference - early_reference),
-                    )
+    def _collect_children_schedules(
+        self, section_id: str, parameters: Dict[str, float]
+    ):
+        """Return a list of the schedules of the children"""
+        subsection_schedules = []
+        section_children = self._schedule_data.experiment_dao.direct_section_children(
+            section_id
+        )
+        for child_section in section_children:
+            subsection_schedules.append(
+                self._schedule_section(child_section, parameters)
+            )
 
-            event_type = event_data["event_type"]
-            if event_type == EventType.SKELETON:
-                event_type = event_data["skeleton_of"]
-
-            if event_type in [
-                EventType.SECTION_END,
-                EventType.SECTION_START,
-                EventType.RIGHT_ALIGNED_COLLECTOR,
-                EventType.SPECTROSCOPY_END,
-                EventType.LOOP_ITERATION_END,
-                EventType.LOOP_STEP_BODY_START,
-                EventType.LOOP_STEP_END,
-                EventType.SUBSECTION_START,
-                EventType.SUBSECTION_END,
-                EventType.SECTION_SKELETON,
-                EventType.RESET_PRECOMPENSATION_FILTERS,
-                EventType.DIGITAL_SIGNAL_STATE_CHANGE,
-            ]:
-                if (
-                    event_type
-                    in [
-                        EventType.SUBSECTION_START,
-                        EventType.SUBSECTION_END,
-                        EventType.SECTION_SKELETON,
-                    ]
-                    and "subsection_name" in event_data
-                ):
-                    # subsection determines the relevant grid for subsection start events
-                    event_section = event_data["subsection_name"]
-                else:
-                    event_section = event_data["section_name"]
-
-                section_grid = self.section_grid(event_section)
-                section_grid_in_tinysamples = round(section_grid / TINYSAMPLE)
-
-                corrected__earliest_event_time = (
-                    (earliest_event_time + section_grid_in_tinysamples - 1)
-                    // section_grid_in_tinysamples
-                    * section_grid_in_tinysamples
+        pulse_schedules = []
+        section_signals = self._schedule_data.experiment_dao.section_signals(section_id)
+        for signal_id in section_signals:
+            pulses = self._schedule_data.experiment_dao.section_pulses(
+                section_id, signal_id
+            )
+            for pulse in pulses:
+                pulse_schedules.append(
+                    self._schedule_pulse(pulse, section_id, parameters)
                 )
-
-                if latest_event_time is not None:
-                    corrected__latest_event_time = (
-                        (latest_event_time + section_grid_in_tinysamples - 1)
-                        // section_grid_in_tinysamples
-                        * section_grid_in_tinysamples
+                if pulse.precompensation_clear:
+                    pulse_schedules.append(
+                        self._schedule_precomp_clear(pulse_schedules[-1])
                     )
-                    if (
-                        not has_exactly_constraint
-                        and corrected__latest_event_time > latest_event_time
-                    ):
-                        corrected__latest_event_time -= section_grid_in_tinysamples
-                else:
-                    corrected__latest_event_time = latest_event_time
 
-            else:
-                corrected__earliest_event_time = earliest_event_time
-                corrected__latest_event_time = latest_event_time
+            signal_grid, _ = self.grid(signal_id)
+            if len(pulses) == 0:
+                # the section occupies the signal via a reserve, so add a placeholder
+                # to include this signal in the grid calculation
+                pulse_schedules.append(ReserveSchedule.create(signal_id, signal_grid))
 
-            if (
-                corrected__latest_event_time is not None
-                and corrected__earliest_event_time - corrected__latest_event_time
-                > self._settings.CONSTRAINT_TOLERANCE / TINYSAMPLE
-            ):
-                exactly_constraint = None
-                _logger.warning("Event %s %s", event_data["event_type"], event_data)
-                for edge in event_graph.out_edges(event_id):
-                    node1 = event_graph.node(edge[0])
-                    node2 = event_graph.node(edge[1])
-                    deltatext = ""
-                    if edge[2].get("delta") is not None:
-                        deltatext = f" delta={edge[2].get('delta')}"
-                    _logger.warning(
-                        "  Edge  %s %s %s -> %s at time %s",
-                        edge[2]["relation"].name,
-                        deltatext,
-                        node_info(node1),
-                        node_info(node2),
-                        event_times[edge[1]],
-                    )
-                    if edge[2]["relation"] == EventRelation.AFTER_EXACTLY:
-                        exactly_constraint = {
-                            "other_node": edge[0],
-                            "edge": edge,
-                            "delta": edge[2].get("delta"),
-                        }
-                _logger.warning(
-                    "corrected__earliest_event_time %f > corrected__latest_event_time %f",
-                    corrected__earliest_event_time,
-                    corrected__latest_event_time,
+        if len(pulse_schedules) and len(subsection_schedules):
+            if any(not isinstance(ps, ReserveSchedule) for ps in pulse_schedules):
+                raise LabOneQException(
+                    f"sections and pulses cannot be mixed in section '{section_id}'"
                 )
 
-                if (
-                    event_type
-                    in [EventType.SECTION_END, EventType.RIGHT_ALIGNED_COLLECTOR]
-                    or (
-                        event_type == EventType.SKELETON
-                        and event_data.get("skeleton_of") == EventType.SECTION_END
-                    )
-                ) and exactly_constraint is not None:
-                    raise LabOneQException(
-                        f"Section end of section {event_data['section_name'] } must "
-                        f"happen exactly {exactly_constraint['delta']} s after its "
-                        f"start, but it contains operations which take longer."
-                    )
-                if (
-                    event_type in [EventType.LOOP_STEP_END]
-                ) and exactly_constraint is not None:
-                    iteration = event_data.get("iteration")
-                    raise LabOneQException(
-                        f"Sweep step end of iteration {iteration} in section "
-                        f"{event_data['section_name'] }  must happen exactly "
-                        f"{exactly_constraint['delta']} s after its start, but it "
-                        f"contains operations which take longer."
-                    )
+        return subsection_schedules + pulse_schedules
 
-                raise Exception(
-                    f"Inconsistent constraints for event {node_info(node1)}"
-                )
-            else:
-                if corrected__latest_event_time is not None:
-                    event_time = corrected__latest_event_time
-                else:
-                    event_time = corrected__earliest_event_time
-
-            _logger.debug(
-                "Calculated event time for event %s to be %f tinysamples",
-                event_id,
-                event_time,
-            )
-            event_times[event_id] = event_time
-
-            if event_data["event_type"] == EventType.PARAMETER_SET:
-                param_obj = event_data["parameter"]
-                parameter_change_times[(param_obj["id"], event_time)] = event_data[
-                    "value"
-                ]
+    def grid(self, *signal_ids: Iterable[str]) -> Tuple[int, int]:
+        """Compute signal and sequencer grid for the given signals. If multiple signals
+        are given, return the LCM of the individual grids."""
 
-        event_times_tiny_samples = copy.deepcopy(event_times)
+        # todo: add memoization; use frozenset?
 
-        for k in event_times.keys():
-            event_times[k] = event_times[k] * TINYSAMPLE
+        signal_grid = 1
+        sequencer_grid = 1
 
-        return event_times, event_times_tiny_samples
+        for signal_id in signal_ids:
+            signal = self._schedule_data.experiment_dao.signal_info(signal_id)
+            device = self._schedule_data.experiment_dao.device_info(signal.device_id)
+            assert device is not None
 
-    def verify_timing(self):
-        TOLERANCE = 1e-11
-        # find nodes which are the reference for another node
-        # through a parameterized edge indicating an "after" relation
-        # this results in the earlier node of the relation being in the list, they are the
-        # second item (b) in the edge (a,b), "a AFTER b"
-        # we need the earlier nodes here so that a new parameter setting
-        # has not yet overridden the current parameter value
-        raw_param_referencing_nodes = [
-            (e[1], e[2].get("delta").param_name)
-            for e in self._event_graph.edge_list()
-            if isinstance(e[2].get("delta"), ParamRef)
-            and e[2].get("relation")
-            in {EventRelation.AFTER_AT_LEAST, EventRelation.AFTER_EXACTLY}
-        ]
-        # add the nodes which are the reference for another node
-        # through a parameterized edge indicating a "before" relation
-        # this also results in the earlier node ending up in the list, they are the
-        # first item (a) in the edge (a,b), "a BEFORE b"
-        raw_param_referencing_nodes.extend(
-            [
-                (e[0], e[2].get("delta").param_name)
-                for e in self._event_graph.edge_list()
-                if isinstance(e[2].get("delta"), ParamRef)
-                and e[2].get("relation") in {EventRelation.BEFORE_AT_LEAST}
-            ]
-        )
-
-        zerogetter = itemgetter(0)
-        # a dict with a node id as a key, mapping to a list of parameters
-        # that are referenced through a parameterized edge by the key node
-        parameter_referencing_nodes = {
-            k: set([node[1] for node in g])
-            for k, g in groupby(
-                sorted(raw_param_referencing_nodes, key=zerogetter), zerogetter
-            )
-        }
-
-        def add_issue(
-            relation, event_time, other_time, delta, event, other_event, edge_data
-        ):
-            issues.append(
-                {
-                    "relation": relation,
-                    "event_time": event_time,
-                    "other_time": other_time,
-                    "delta": delta,
-                    "event": event,
-                    "other_event": other_event,
-                    "edge_data": edge_data,
-                }
+            sample_rate = self._sampling_rate_tracker.sampling_rate_for_device(
+                device.id
             )
-
-        parameter_values = {}
-        parameter_values_at_node = {}
-        sorted_events = sorted(
-            [
-                self._event_graph.node(event_id)
-                for event_id in self._event_graph.node_ids()
-            ],
-            # PARAMETER_SET must be visited early in case of tie
-            key=lambda node: (node["time"], node["event_type"] != "PARAMETER_SET"),
-        )
-        issues = []
-
-        for event in sorted_events:
-            if event["event_type"] == EventType.PARAMETER_SET:
-                parameter_values[event["parameter"]["id"]] = event["value"]
-
-            if event["id"] in parameter_referencing_nodes:
-                parameter_values_at_node[event["id"]] = {
-                    k: parameter_values[k]
-                    for k in parameter_referencing_nodes[event["id"]]
-                }
-
-            for _, other_node_id, edge_data in self._event_graph.out_edges(event["id"]):
-
-                other_event = self._event_graph.node(other_node_id)
-                relation = edge_data["relation"]
-
-                if "delta" in edge_data:
-                    if isinstance(edge_data["delta"], ParamRef):
-                        param_name = edge_data["delta"].param_name
-                        # get the value of the parameter as it was at the node at the other end of the edge
-                        # because if a parameter change happens at the same time as the end of the interval
-                        # the new value would be used - which is wrong because that value applies only to the
-                        # next interval
-                        param_values_at_other_node = parameter_values_at_node.get(
-                            other_node_id
-                        )
-                        if param_values_at_other_node is not None:
-                            delta = param_values_at_other_node[param_name]
-                        else:
-                            delta = parameter_values[param_name]
-
-                    elif callable(edge_data["delta"]):
-                        delta = edge_data["delta"](other_event["time"])
-                    else:
-                        delta = edge_data["delta"]
-                else:
-                    delta = None
-
-                if (
-                    "SKELETON" in event["event_type"]
-                    or "SKELETON" in other_event["event_type"]
-                ):
-                    # SKELETON events have a difficult parameter-dependent timing -> ignore
-                    continue
-
-                if relation == EventRelation.AFTER_OR_AT:
-                    if not event["time"] >= other_event["time"]:
-                        add_issue(
-                            relation,
-                            event["time"],
-                            other_event["time"],
-                            delta,
-                            event,
-                            other_event,
-                            edge_data,
-                        )
-
-                elif relation == EventRelation.AFTER_AT_LEAST:
-                    if callable(delta):
-                        delta = delta(other_event["time"])
-                    if not event["time"] >= other_event["time"] + delta - TOLERANCE:
-                        add_issue(
-                            relation,
-                            event["time"],
-                            other_event["time"],
-                            delta,
-                            event,
-                            other_event,
-                            edge_data,
-                        )
-                elif relation == EventRelation.AFTER:
-                    if not event["time"] > other_event["time"]:
-                        add_issue(
-                            relation,
-                            event["time"],
-                            other_event["time"],
-                            delta,
-                            event,
-                            other_event,
-                            edge_data,
-                        )
-
-                elif relation in (
-                    EventRelation.USES_EARLY_REFERENCE,
-                    EventRelation.USES_LATE_REFERENCE,
-                ):
-                    pass
-                elif relation == EventRelation.AFTER_EXACTLY and delta is not None:
-                    if not event["time"] - other_event["time"] - delta >= -TOLERANCE:
-                        add_issue(
-                            relation,
-                            event["time"],
-                            other_event["time"],
-                            delta,
-                            event,
-                            other_event,
-                            edge_data,
-                        )
-
-                elif relation == EventRelation.AFTER_LOOP:
-                    pass
-                    # assert event["time"] == other_event["time"]
-                elif relation == EventRelation.BEFORE:
-                    if not event["time"] < other_event["time"]:
-                        add_issue(
-                            relation,
-                            event["time"],
-                            other_event["time"],
-                            delta,
-                            event,
-                            other_event,
-                            edge_data,
-                        )
-
-                elif relation == EventRelation.BEFORE_OR_AT:
-                    if not event["time"] <= other_event["time"]:
-                        add_issue(
-                            relation,
-                            event["time"],
-                            other_event["time"],
-                            delta,
-                            event,
-                            other_event,
-                            edge_data,
-                        )
-
-                elif relation == EventRelation.BEFORE_AT_LEAST:
-                    if not event["time"] + delta <= other_event["time"] + TOLERANCE:
-                        add_issue(
-                            relation,
-                            event["time"],
-                            other_event["time"],
-                            delta,
-                            event,
-                            other_event,
-                            edge_data,
-                        )
-
-                elif relation == EventRelation.RELATIVE_BEFORE:
-                    if not event["time"] <= other_event["time"]:
-                        add_issue(
-                            relation,
-                            event["time"],
-                            other_event["time"],
-                            delta,
-                            event,
-                            other_event,
-                            edge_data,
-                        )
-                else:
-                    raise ValueError("invalid relation")
-
-        for issue in issues:
-            issue_text = ", ".join(f"{key}: {value}" for key, value in issue.items())
-            _logger.warning(
-                f"Issue: Not fulfilled timing relation {issue['event']['id']}  ->  {issue['other_event']['id']} : {issue_text}"
-            )
-        if len(issues) > 0 and not self._settings.IGNORE_GRAPH_VERIFY_RESULTS:
-            raise LabOneQException(
-                f"Scheduler issues: Constraints not satisfied: {issue_text}"
+            sequencer_rate = self._sampling_rate_tracker.sequencer_rate_for_device(
+                device.id
             )
 
-    def _has_control_elements(self, section_display_name):
-        section_info = self._experiment_dao.section_info(section_display_name)
-
-        if (
-            section_info.has_repeat
-            or section_info.acquisition_types is not None
-            and len(section_info.acquisition_types) > 0
-            or section_info.handle is not None
-            or section_info.state is not None
-        ):
-            return True
-        for trigger_info in section_info.trigger_output:
-            if trigger_info["state"]:
-                return True
-
-        for signal in self._experiment_dao.section_signals(section_display_name):
-            if any(
-                pulse.precompensation_clear
-                for pulse in self._experiment_dao.section_pulses(
-                    section_display_name, signal
+            signal_grid = int(
+                lcm(
+                    signal_grid,
+                    round(1 / (self._schedule_data.TINYSAMPLE * sample_rate)),
                 )
-            ):
-                return True
-
-        return False
-
-    def section_grid(self, section):
-
-        if section in self._section_grids:
-            _logger.debug("Section cache hit for section %s", section)
-            return self._section_grids[section]
-
-        if self._settings.FIXED_SLOW_SECTION_GRID:
-            section_grid = Fraction(8, int(600e6))
-            _logger.warning(
-                "Fixed section grid because setting 'fixed_slow_section_grid' is set"
             )
-            self._section_grids[section] = section_grid
-            return section_grid
-
-        if self._section_graph_object is not None:
-            section_info = self._section_graph_object.section_info(section)
-            section_display_name = section_info.section_display_name
-        else:
-            section_info = self._experiment_dao.section_info(section)
-            section_display_name = section
-
-        device_types = [
-            DeviceType(device_type)
-            for device_type in self._experiment_dao.device_types_in_section(
-                section_display_name
+            sequencer_grid = int(
+                lcm(
+                    sequencer_grid,
+                    round(1 / (self._schedule_data.TINYSAMPLE * sequencer_rate)),
+                )
             )
-        ]
-        has_control_elements = self._has_control_elements(section_display_name)
-
-        _logger.debug("Device types for section %s are %s", section, device_types)
-        self._section_grids[section] = self._calculate_section_grid(
-            section,
-            device_types,
-            self._clock_settings["use_2GHz_for_HDAWG"],
-            has_control_elements,
-            section_info.on_system_grid,
-        )
-        return self._section_grids[section]
+        return signal_grid, sequencer_grid
 
-    @staticmethod
-    def _calculate_section_grid(
-        section,
-        device_types,
-        use_2GHz_for_HDAWG,
-        has_control_elements,
-        on_system_grid=False,
-    ):
+    def _compute_trigger_output(
+        self, section_info: SectionInfo
+    ) -> Set[Tuple[str, int]]:
+        """Compute the effective trigger signals for the given section.
 
-        if len(device_types) == 0:
-            _logger.debug(
-                "Section %s : using default section grid, device_types=%s",
-                section,
-                device_types,
-            )
-            return Fraction(8, 600 * 1000 * 1000)
-
-        sequencer_frequencies = []
-        signal_frequencies = set()
-        for d in device_types:
-            if d == DeviceType.HDAWG and use_2GHz_for_HDAWG:
-                sequencer_frequencies.append(
-                    int(d.sampling_rate_2GHz / d.sample_multiple)
+        The return value is a set of `(signal_id, bit_index)` tuples.
+        """
+        if len(section_info.trigger_output) == 0:
+            return set()
+        section_name = section_info.section_display_name or section_info.section_id
+        parent_section_trigger_states = {}  # signal -> state
+        parent_section_id = section_name
+        while True:
+            parent_section_id = self._schedule_data.experiment_dao.section_parent(
+                parent_section_id
+            )
+            if parent_section_id is None:
+                break
+            parent_section_info = self._schedule_data.experiment_dao.section_info(
+                parent_section_id
+            )
+            for trigger_info in parent_section_info.trigger_output:
+                state = trigger_info["state"]
+                signal = trigger_info["signal_id"]
+                parent_section_trigger_states[signal] = (
+                    parent_section_trigger_states.get(signal, 0) | state
                 )
-                signal_frequencies.add(d.sampling_rate_2GHz)
-            else:
-                sequencer_frequencies.append(int(d.sampling_rate / d.sample_multiple))
-                signal_frequencies.add(d.sampling_rate)
-
-        signal_frequencies = list(signal_frequencies)
-        if (
-            len(signal_frequencies) == 1
-            and not has_control_elements
-            and not on_system_grid
-        ):
-            _logger.debug(
-                "signal frequencies are %s - returning signal frequency grid",
-                [str(EngNumber(f)) for f in signal_frequencies],
-            )
-            return 1 / signal_frequencies[0]
-
-        # Actually, we should return the total system grid when on_system_grid is True
-        # and not only the sequencer frequencies here, but since this scheduler will
-        # be replaced soon and the two grids anyway match for the relevant case, this is
-        # fine.
-        _logger.debug(
-            "Sequencer frequencies are %s",
-            [str(EngNumber(f)) for f in sequencer_frequencies],
-        )
-        sequencer_frequency = np.gcd.reduce(sequencer_frequencies)
-        return 1 / Fraction(int(sequencer_frequency))
 
-    def _add_start_events(self):
-        retval = []
-
-        # Add initial events to reset the NCOs.
-        # Todo (PW): Drop once system tests have been migrated from legacy behaviour.
-        for device_info in self._experiment_dao.device_infos():
-            try:
-                device_type = DeviceType(device_info.device_type)
-            except ValueError:
-                # Not every device has a corresponding DeviceType (e.g. PQSC)
-                continue
-            if not device_type.supports_reset_osc_phase:
+        section_trigger_signals = set()
+        for trigger_info in section_info.trigger_output:
+            signal = trigger_info["signal_id"]
+            state = trigger_info["state"]
+            parent_state = parent_section_trigger_states.get(signal, 0)
+            if not state:
                 continue
-            retval.append(
-                self._event_graph.add_node(
-                    event_type=EventType.INITIAL_RESET_HW_OSCILLATOR_PHASE,
-                    device_id=device_info.id,
-                    duration=device_type.reset_osc_duration,
+            for bit, bit_mask in enumerate([0b01, 0b10]):
+                # skip the current bit if it is controlled by any parent section
+                if parent_state & bit_mask != state & bit_mask and state & bit_mask > 0:
+                    section_trigger_signals.add((signal, bit))
+        return section_trigger_signals
+
+    def _resolve_repetition_time(
+        self, root_sections: Tuple[str]
+    ) -> Optional[RepetitionInfo]:
+        """Locate the loop section which corresponds to the shot boundary.
+
+        This section will be padded to the repetition length."""
+
+        repetition_info: Optional[RepetitionInfo] = None
+        for section in self._schedule_data.experiment_dao.sections():
+            section_info = self._schedule_data.experiment_dao.section_info(section)
+            if (
+                section_info.repetition_mode is not None
+                or section_info.repetition_time is not None
+            ):
+                if repetition_info is not None:
+                    raise LabOneQException(
+                        f"Both sections '{repetition_info.section}' and '{section} define"
+                        f"a repetition mode."
+                    )
+                repetition_info = RepetitionInfo(
+                    section,
+                    RepetitionMode(section_info.repetition_mode),
+                    section_info.repetition_time,
                 )
-            )
-        return retval
 
-    def _path_to_root(self, section_id):
-        current_section = section_id
-        path_to_root = [current_section]
-        while True:
-            parent = self._experiment_dao.section_parent(current_section)
-            if parent is not None:
-                path_to_root.append(parent)
-                current_section = parent
-            else:
-                break
-        _logger.debug("Path to root from %s : %s", section_id, path_to_root)
-        return path_to_root
+        if repetition_info is None or repetition_info.mode == RepetitionMode.FASTEST:
+            return None
+
+        # Multi-root experiment not allowed in DSL anyway. For non-trivial repetition
+        # mode, scheduling of these is not possible.
+        assert len(root_sections) == 1
+        root_section = root_sections[0]
+
+        def search_lowest_level_loop(section):
+            loop: Optional[str] = None
+            section_info = self._schedule_data.experiment_dao.section_info(section)
+            if section_info.has_repeat:
+                loop = section
+
+            children = self._schedule_data.experiment_dao.direct_section_children(
+                section
+            )
+            if len(children) == 0:
+                return loop
+            if len(children) == 1:
+                return search_lowest_level_loop(children[0]) or loop
+
+            # Two or more children - no loops allowed!
+            for child in children:
+                nested_loop = search_lowest_level_loop(child)
+                if nested_loop:
+                    raise LabOneQException(
+                        f"Section '{section}' contains multiple children, including "
+                        f"other loops (e.g. '{nested_loop}'). This is not permitted in "
+                        f"repetition mode '{repetition_info.mode}'."
+                    )
+            return loop
+
+        shot_loop = search_lowest_level_loop(root_section)
+        if shot_loop is None:
+            return None
+        return replace(repetition_info, section=shot_loop)
 
     def preorder_map(self):
-        return self._section_graph_object.preorder_map()
+        preorder_map = {}
+        assert self._root_schedule is not None
+        for s in self._root_schedule.children:
+            calculate_preorder_map(s, preorder_map)
+        return preorder_map
```

## laboneq/compiler/workflow/compiler.py

```diff
@@ -15,29 +15,32 @@
 from laboneq.compiler.code_generator.measurement_calculator import (
     IntegrationTimes,
     SignalDelays,
 )
 from laboneq.compiler.common import compiler_settings
 from laboneq.compiler.common.awg_info import AWGInfo, AwgKey
 from laboneq.compiler.common.awg_signal_type import AWGSignalType
-from laboneq.compiler.common.device_type import DeviceType
+from laboneq.compiler.common.device_type import (
+    DeviceType,
+    validate_local_oscillator_frequency,
+)
 from laboneq.compiler.common.signal_obj import SignalObj
 from laboneq.compiler.common.trigger_mode import TriggerMode
 from laboneq.compiler.experiment_access.device_info import DeviceInfo
 from laboneq.compiler.experiment_access.experiment_dao import ExperimentDAO
-from laboneq.compiler.new_scheduler.scheduler import Scheduler as NewScheduler
 from laboneq.compiler.scheduler.sampling_rate_tracker import SamplingRateTracker
 from laboneq.compiler.scheduler.scheduler import Scheduler
 from laboneq.compiler.workflow.precompensation_helpers import (
     compute_precompensation_delays_on_grid,
     compute_precompensations_and_delays,
     precompensation_is_nonzero,
     verify_precompensation_parameters,
 )
 from laboneq.compiler.workflow.recipe_generator import RecipeGenerator
+from laboneq.core.exceptions import LabOneQException
 from laboneq.core.types.compiled_experiment import CompiledExperiment
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 from laboneq.core.types.enums.mixer_type import MixerType
 
 _logger = logging.getLogger(__name__)
 
 
@@ -48,26 +51,21 @@
     internal_followers: List[str] = field(default_factory=list)
 
 
 _AWGMapping = Dict[str, Dict[int, AWGInfo]]
 
 
 class Compiler:
-    Scheduler = Scheduler
-
     def __init__(self, settings: Optional[Dict] = None):
         self._osc_numbering = None
         self._section_grids = {}
         self._experiment_dao: ExperimentDAO = None
         self._settings = compiler_settings.from_dict(settings)
         self._sampling_rate_tracker: SamplingRateTracker = None
-        self.Scheduler = Scheduler
-        if self._settings.USE_EXPERIMENTAL_SCHEDULER:
-            self.Scheduler = NewScheduler
-        self._scheduler: Compiler.Scheduler = None
+        self._scheduler: Scheduler = None
 
         self._leader_properties = LeaderProperties()
         self._clock_settings: Dict[str, Any] = {}
         self._integration_unit_allocation = None
         self._awgs: _AWGMapping = {}
         self._precompensations: Dict[
             str, Dict[str, Union[Dict[str, Any], float]]
@@ -222,15 +220,21 @@
             self._experiment_dao, self._clock_settings
         )
         self._calc_integration_unit_allocation()
         self._precompensations = self._calc_precompensations()
         self._signal_objects = self._generate_signal_objects()
         _logger.debug("Processing Sections:::::::")
 
-        self._scheduler = self.Scheduler(
+        if not self._settings.USE_EXPERIMENTAL_SCHEDULER:
+            _logger.warning(
+                "The legacy scheduler has been removed; "
+                "the 'USE_EXPERIMENTAL_SCHEDULER' compiler flag is ignored."
+            )
+
+        self._scheduler = Scheduler(
             self._experiment_dao,
             self._sampling_rate_tracker,
             self._signal_objects,
             self._clock_settings,
             self._settings,
         )
         self._scheduler.run()
@@ -637,38 +641,46 @@
             lo_frequency = self._experiment_dao.lo_frequency(signal_id)
             port_mode = self._experiment_dao.port_mode(signal_id)
             signal_range, signal_range_unit = self._experiment_dao.signal_range(
                 signal_id
             )
             device_type = DeviceType(signal_info.device_type)
             port_delay = self._experiment_dao.port_delay(signal_id)
+
+            scheduler_port_delay: float = 0.0
             if signal_id in signal_delays:
-                port_delay = (port_delay or 0) + signal_delays[signal_id].on_device
-                if abs(port_delay) < 1e-12:
-                    port_delay = None
+                scheduler_port_delay += signal_delays[signal_id].on_device
             precompensation = self._precompensations[signal_id]
             pc_port_delay = precompensation["computed_port_delay"]
             if pc_port_delay:
-                port_delay = (port_delay or 0) + pc_port_delay
+                scheduler_port_delay += pc_port_delay
 
             base_channel = min(signal_info.channels)
 
             markers = self._experiment_dao.markers_on_signal(signal_id)
 
             triggers = self._experiment_dao.triggers_on_signal(signal_id)
+            if lo_frequency is not None:
+                try:
+                    validate_local_oscillator_frequency(lo_frequency, device_type)
+                except ValueError as error:
+                    raise LabOneQException(
+                        f"Error on signal line '{signal_id}': {error}"
+                    ) from error
 
             for channel in signal_info.channels:
                 output = {
                     "device_id": signal_info.device_id,
                     "channel": channel,
                     "lo_frequency": lo_frequency,
                     "port_mode": port_mode,
                     "range": signal_range,
                     "range_unit": signal_range_unit,
                     "port_delay": port_delay,
+                    "scheduler_port_delay": scheduler_port_delay,
                 }
                 signal_is_modulated = signal_info.modulation
                 output_modulation_logic = {
                     (True, True): True,
                     (False, False): False,
                     (True, False): False,
                     (False, True): False,
@@ -773,34 +785,41 @@
                 all_channels[channel_key] = output
         retval = sorted(
             all_channels.values(),
             key=lambda output: output["device_id"] + str(output["channel"]),
         )
         return retval
 
-    def calc_inputs(self):
+    def calc_inputs(self, signal_delays: SignalDelays):
         all_channels = {}
         for signal_id in self._experiment_dao.signals():
             signal_info = self._experiment_dao.signal_info(signal_id)
             if signal_info.signal_type != "integration":
                 continue
 
             lo_frequency = self._experiment_dao.lo_frequency(signal_id)
             signal_range, signal_range_unit = self._experiment_dao.signal_range(
                 signal_id
             )
+
             port_delay = self._experiment_dao.port_delay(signal_id)
+
+            scheduler_port_delay: float = 0.0
+            if signal_id in signal_delays:
+                scheduler_port_delay += signal_delays[signal_id].on_device
+
             for channel in signal_info.channels:
                 input = {
                     "device_id": signal_info.device_id,
                     "channel": channel,
                     "lo_frequency": lo_frequency,
                     "range": signal_range,
                     "range_unit": signal_range_unit,
                     "port_delay": port_delay,
+                    "scheduler_port_delay": scheduler_port_delay,
                 }
                 channel_key = (signal_info.device_id, channel)
                 # TODO(2K): check for conflicts if 'channel_key' already present in 'all_channels'
                 all_channels[channel_key] = input
         retval = sorted(
             all_channels.values(),
             key=lambda input: input["device_id"] + str(input["channel"]),
@@ -869,15 +888,15 @@
                         "Expanding existing measurement record for device %s awg %d (when looking at section %s )",
                         device_id,
                         awg_nr,
                         info["section_name"],
                     )
                     measurement = measurements[(device_id, awg_nr)]
                 else:
-                    measurement = {"length": None, "delay": 0}
+                    measurement = {"length": None}
 
                     integration_time_info = integration_times.section_info(
                         info["section_name"]
                     )
                     if integration_time_info is not None:
 
                         _logger.debug(
@@ -888,17 +907,14 @@
                             i
                             for i in integration_time_info.values()
                             if i.awg == awg_nr and i.device_id == device_id
                         )
                         measurement[
                             "length"
                         ] = signal_info_for_section_and_device_awg.length_in_samples
-                        measurement[
-                            "delay"
-                        ] = signal_info_for_section_and_device_awg.delay_in_samples
                     else:
                         del measurement["length"]
                     _logger.debug(
                         "Added measurement %s\n  for %s", measurement, device_awg_nr
                     )
 
                 measurements[(device_id, awg_nr)] = measurement
@@ -935,26 +951,28 @@
                 oscillator=output["oscillator"],
                 oscillator_frequency=output["oscillator_frequency"],
                 lo_frequency=output["lo_frequency"],
                 port_mode=output["port_mode"],
                 output_range=output["range"],
                 output_range_unit=output["range_unit"],
                 port_delay=output["port_delay"],
+                scheduler_port_delay=output["scheduler_port_delay"],
                 marker_mode=output.get("marker_mode"),
             )
 
-        for input in self.calc_inputs():
+        for input in self.calc_inputs(self._code_generator.signal_delays()):
             _logger.debug("Adding input %s", input)
             recipe_generator.add_input(
                 input["device_id"],
                 input["channel"],
                 lo_frequency=input["lo_frequency"],
                 input_range=input["range"],
                 input_range_unit=input["range_unit"],
                 port_delay=input["port_delay"],
+                scheduler_port_delay=input["scheduler_port_delay"],
             )
 
         for device_id, awgs in self._awgs.items():
             for awg in awgs.values():
                 signal_type = awg.signal_type
                 if signal_type == AWGSignalType.DOUBLE:
                     awg_signals = {
```

## laboneq/compiler/workflow/recipe_generator.py

```diff
@@ -194,14 +194,15 @@
         oscillator=None,
         oscillator_frequency=None,
         lo_frequency=None,
         port_mode=None,
         output_range=None,
         output_range_unit=None,
         port_delay=None,
+        scheduler_port_delay=0.0,
         marker_mode=None,
     ):
         output = {"channel": channel, "enable": True}
         if offset is not None:
             output.update({"offset": offset})
         if diagonal is not None and off_diagonal is not None:
             output.update(
@@ -220,14 +221,15 @@
         if oscillator is not None:
             output["oscillator"] = oscillator
         output["modulation"] = modulation
         if oscillator_frequency is not None:
             output["oscillator_frequency"] = oscillator_frequency
         if port_delay is not None:
             output["port_delay"] = port_delay
+        output["scheduler_port_delay"] = scheduler_port_delay
         if marker_mode is not None:
             output["marker_mode"] = marker_mode
 
         initialization: dict = self._find_initialization(device_id)
         outputs: list = initialization.setdefault("outputs", [])
         outputs.append(output)
 
@@ -235,24 +237,26 @@
         self,
         device_id,
         channel,
         lo_frequency=None,
         input_range=None,
         input_range_unit=None,
         port_delay=None,
+        scheduler_port_delay=0.0,
     ):
         input = {"channel": channel, "enable": True}
         if lo_frequency is not None:
             input["lo_frequency"] = lo_frequency
         if input_range is not None:
             input["range"] = input_range
         if input_range_unit is not None:
             input["range_unit"] = input_range_unit
         if port_delay is not None:
             input["port_delay"] = port_delay
+        input["scheduler_port_delay"] = scheduler_port_delay
 
         initialization: dict = self._find_initialization(device_id)
         inputs: list = initialization.setdefault("inputs", [])
         inputs.append(input)
 
     def add_awg(
         self,
```

## laboneq/contrib/example_helpers/descriptors/shfqc.py

```diff
@@ -24,14 +24,22 @@
       ports: SGCHANNELS/2/OUTPUT
     - iq_signal: q2/drive_line_ef
       ports: SGCHANNELS/2/OUTPUT
     - iq_signal: q3/drive_line
       ports: SGCHANNELS/3/OUTPUT
     - iq_signal: q3/drive_line_ef
       ports: SGCHANNELS/3/OUTPUT
+    - iq_signal: q4/drive_line
+      ports: SGCHANNELS/4/OUTPUT
+    - iq_signal: q4/drive_line_ef
+      ports: SGCHANNELS/4/OUTPUT
+    - iq_signal: q5/drive_line
+      ports: SGCHANNELS/5/OUTPUT
+    - iq_signal: q5/drive_line_ef
+      ports: SGCHANNELS/5/OUTPUT
 
     - iq_signal: q0/measure_line
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q0/acquire_line
       ports: [QACHANNELS/0/INPUT]
     - iq_signal: q1/measure_line
       ports: [QACHANNELS/0/OUTPUT]
@@ -41,8 +49,16 @@
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q2/acquire_line
       ports: [QACHANNELS/0/INPUT]
     - iq_signal: q3/measure_line
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q3/acquire_line
       ports: [QACHANNELS/0/INPUT]
+    - iq_signal: q4/measure_line
+      ports: [QACHANNELS/0/OUTPUT]
+    - acquire_signal: q4/acquire_line
+      ports: [QACHANNELS/0/INPUT]
+    - iq_signal: q5/measure_line
+      ports: [QACHANNELS/0/OUTPUT]
+    - acquire_signal: q5/acquire_line
+      ports: [QACHANNELS/0/INPUT]
 """
```

## laboneq/contrib/example_helpers/descriptors/shfsg.py

```diff
@@ -24,14 +24,22 @@
       ports: SGCHANNELS/2/OUTPUT
     - iq_signal: q2/drive_line_ef
       ports: SGCHANNELS/2/OUTPUT
     - iq_signal: q3/drive_line
       ports: SGCHANNELS/3/OUTPUT
     - iq_signal: q3/drive_line_ef
       ports: SGCHANNELS/3/OUTPUT
+    - iq_signal: q4/drive_line
+      ports: SGCHANNELS/4/OUTPUT
+    - iq_signal: q4/drive_line_ef
+      ports: SGCHANNELS/4/OUTPUT
+    - iq_signal: q5/drive_line
+      ports: SGCHANNELS/5/OUTPUT
+    - iq_signal: q5/drive_line_ef
+      ports: SGCHANNELS/5/OUTPUT
 
     # - iq_signal: q0/measure_line
     #   ports: [QACHANNELS/0/OUTPUT]
     # - acquire_signal: q0/acquire_line
     #   ports: [QACHANNELS/0/INPUT]
     # - iq_signal: q1/measure_line
     #   ports: [QACHANNELS/0/OUTPUT]
```

## laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_hdawg_pqsc.py

```diff
@@ -43,14 +43,22 @@
       ports: SGCHANNELS/2/OUTPUT
     - iq_signal: q2/drive_line_ef
       ports: SGCHANNELS/2/OUTPUT
     - iq_signal: q3/drive_line
       ports: SGCHANNELS/3/OUTPUT
     - iq_signal: q3/drive_line_ef
       ports: SGCHANNELS/3/OUTPUT
+    - iq_signal: q4/drive_line
+      ports: SGCHANNELS/4/OUTPUT
+    - iq_signal: q4/drive_line_ef
+      ports: SGCHANNELS/4/OUTPUT
+    - iq_signal: q5/drive_line
+      ports: SGCHANNELS/5/OUTPUT
+    - iq_signal: q5/drive_line_ef
+      ports: SGCHANNELS/5/OUTPUT
 
   device_shfqa:
     - iq_signal: q0/measure_line
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q0/acquire_line
       ports: [QACHANNELS/0/INPUT]
     - iq_signal: q1/measure_line
@@ -61,14 +69,22 @@
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q2/acquire_line
       ports: [QACHANNELS/0/INPUT]
     - iq_signal: q3/measure_line
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q3/acquire_line
       ports: [QACHANNELS/0/INPUT]
+    - iq_signal: q4/measure_line
+      ports: [QACHANNELS/0/OUTPUT]
+    - acquire_signal: q4/acquire_line
+      ports: [QACHANNELS/0/INPUT]
+    - iq_signal: q5/measure_line
+      ports: [QACHANNELS/0/OUTPUT]
+    - acquire_signal: q5/acquire_line
+      ports: [QACHANNELS/0/INPUT]
 
   device_pqsc:
     - to: device_hdawg
       port: ZSYNCS/0
     - to: device_shfsg
       port: ZSYNCS/1
     - to: device_shfqa
```

## laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_pqsc.py

```diff
@@ -30,14 +30,22 @@
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q2/acquire_line
       ports: [QACHANNELS/0/INPUT]
     - iq_signal: q3/measure_line
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q3/acquire_line
       ports: [QACHANNELS/0/INPUT]
+    - iq_signal: q4/measure_line
+      ports: [QACHANNELS/0/OUTPUT]
+    - acquire_signal: q4/acquire_line
+      ports: [QACHANNELS/0/INPUT]
+    - iq_signal: q5/measure_line
+      ports: [QACHANNELS/0/OUTPUT]
+    - acquire_signal: q5/acquire_line
+      ports: [QACHANNELS/0/INPUT]
 
   device_shfsg:
     - iq_signal: q0/drive_line
       ports: SGCHANNELS/0/OUTPUT
     - iq_signal: q0/drive_line_ef
       ports: SGCHANNELS/0/OUTPUT
     - iq_signal: q1/drive_line
@@ -48,14 +56,22 @@
       ports: SGCHANNELS/2/OUTPUT
     - iq_signal: q2/drive_line_ef
       ports: SGCHANNELS/2/OUTPUT
     - iq_signal: q3/drive_line
       ports: SGCHANNELS/3/OUTPUT
     - iq_signal: q3/drive_line_ef
       ports: SGCHANNELS/3/OUTPUT
+    - iq_signal: q4/drive_line
+      ports: SGCHANNELS/4/OUTPUT
+    - iq_signal: q4/drive_line_ef
+      ports: SGCHANNELS/4/OUTPUT
+    - iq_signal: q5/drive_line
+      ports: SGCHANNELS/5/OUTPUT
+    - iq_signal: q5/drive_line_ef
+      ports: SGCHANNELS/5/OUTPUT
 
   device_pqsc:
     # - internal_clock_signal
     - to: device_shfqa
       port: ZSYNCS/0
     - to: device_shfsg
       port: ZSYNCS/1
```

## laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_shfqc_hdawg_pqsc.py

```diff
@@ -30,14 +30,16 @@
       ports: SIGOUTS/1
     - rf_signal: q2/flux_line
       ports: SIGOUTS/2
     - rf_signal: q3/flux_line
       ports: SIGOUTS/3
     - rf_signal: q4/flux_line
       ports: SIGOUTS/4
+    - rf_signal: q5/flux_line
+      ports: SIGOUTS/5
 
   device_shfsg:
     - iq_signal: q0/drive_line
       ports: SGCHANNELS/0/OUTPUT
     - iq_signal: q0/drive_line_ef
       ports: SGCHANNELS/0/OUTPUT
     - iq_signal: q1/drive_line
@@ -72,18 +74,27 @@
       ports: [QACHANNELS/0/INPUT]
 
   device_shfqc:
     - iq_signal: q4/drive_line
       ports: SGCHANNELS/0/OUTPUT
     - iq_signal: q4/drive_line_ef
       ports: SGCHANNELS/0/OUTPUT
+    - iq_signal: q5/drive_line
+      ports: SGCHANNELS/1/OUTPUT
+    - iq_signal: q5/drive_line_ef
+      ports: SGCHANNELS/1/OUTPUT
+
     - iq_signal: q4/measure_line
       ports: [QACHANNELS/0/OUTPUT]
     - acquire_signal: q4/acquire_line
       ports: [QACHANNELS/0/INPUT]
+    - iq_signal: q5/measure_line
+      ports: [QACHANNELS/0/OUTPUT]
+    - acquire_signal: q5/acquire_line
+      ports: [QACHANNELS/0/INPUT]
 
   device_pqsc:
     - to: device_hdawg
       port: ZSYNCS/0
     - to: device_shfsg
       port: ZSYNCS/1
     - to: device_shfqa
```

## laboneq/contrib/example_helpers/plotting/plot_helpers.py

```diff
@@ -164,14 +164,114 @@
             axes.grid(True)
 
     fig.tight_layout()
     # fig.legend(loc="upper left")
     plt.show()
 
 
+# general result plotting
+def plot_results(
+    results,
+    phase=False,
+    plot_width=6,
+    plot_height=2,
+):
+    handles = results.acquired_results.keys()
+
+    for handle in handles:
+        axis_name_list = [k for k in results.get_axis_name(handle)]
+        acquired_data = results.get_data(handle)
+        if len(axis_name_list) == 1 and phase is False:
+            axis_grid = results.get_axis(handle)[0]
+            axis_name = results.get_axis_name(handle)[0]
+            plt.figure(figsize=(plot_width, plot_height))
+            plt.plot(axis_grid, np.absolute(acquired_data))
+            plt.xlabel(axis_name)
+            plt.ylabel("Amplitude (a.u.)")
+            plt.title(f"Handle: {handle}")
+            plt.show()
+
+        elif len(axis_name_list) == 1 and phase is True:
+            axis_grid = results.get_axis(handle)[0]
+            axis_name = results.get_axis_name(handle)[0]
+
+            fig, [ax1, ax2] = plt.subplots(2, 1, figsize=(plot_width, plot_height))
+
+            ax1.set_title(f"Handle: {handle}")
+            ax1.plot(axis_grid, abs(acquired_data), ".k")
+            ax2.plot(axis_grid, np.unwrap(np.angle(acquired_data)))
+            ax1.set_ylabel("Amplitude (a.u)")
+            ax2.set_ylabel("$\\phi$ (rad)")
+            ax2.set_xlabel(axis_name)
+            fig.tight_layout()
+            plt.show()
+
+        elif len(axis_name_list) == 2 and phase is False:
+            axis_1 = results.get_axis(handle)[1]
+            axis_1_name = results.get_axis_name(handle)[1]
+            axis_0 = results.get_axis(handle)[0]
+            axis_0_name = results.get_axis_name(handle)[0]
+            data = results.get_data(handle)
+
+            X, Y = np.meshgrid(axis_1, axis_0)
+            fig, ax = plt.subplots(nrows=1, ncols=1, constrained_layout=True)
+
+            CS = ax.contourf(X, Y, np.abs(data), levels=100, cmap="magma")
+            ax.set_title(f"{handle}")
+            ax.set_xlabel(axis_1_name)
+            ax.set_ylabel(axis_0_name)
+            cbar = fig.colorbar(CS)
+            cbar.set_label("Amplitude (a.u.)")
+
+        elif len(axis_name_list) == 2 and phase is True:
+            axis_1 = results.get_axis(handle)[1]
+            axis_1_name = results.get_axis_name(handle)[1]
+            axis_0 = results.get_axis(handle)[0]
+            axis_0_name = results.get_axis_name(handle)[0]
+            data = results.get_data(handle)
+
+            X, Y = np.meshgrid(axis_1, axis_0)
+            fig, ax = plt.subplots(nrows=1, ncols=2, constrained_layout=True)
+
+            CS = ax[0].contourf(X, Y, np.abs(data), levels=100, cmap="magma")
+            plt.suptitle(f"Handle: {handle}")
+            ax[0].set_xlabel(axis_1_name)
+            ax[0].set_ylabel(axis_0_name)
+            cbar = fig.colorbar(CS)
+            cbar.set_label("Amplitude (a.u.)")
+
+            cs2_max_value = (
+                max(
+                    int(np.abs(np.min(np.unwrap(np.angle(data, deg=True))))),
+                    int(np.abs(np.max(np.unwrap(np.angle(data, deg=True))))),
+                )
+                + 1
+            )
+
+            cs2_levels = np.linspace(
+                -cs2_max_value, cs2_max_value, 2 * (cs2_max_value) + 1
+            )
+
+            CS2 = ax[1].contourf(
+                X,
+                Y,
+                np.unwrap(np.angle(data, deg=True)),
+                levels=cs2_levels,
+                cmap="twilight_shifted",
+            )
+            # ax[1].set_title("Phase")
+            ax[1].set_xlabel(axis_1_name)
+            ax[1].set_ylabel(axis_0_name)
+            cbar2 = fig.colorbar(CS2)
+            cbar2.set_label("$\\phi$ (deg)")
+
+        elif len(axis_name_list) > 2:
+            print("Too many dimensions. I don't know how to plot your data!")
+
+
 # 2D plot
 def plot_result_2d(results, handle, mult_axis=None):
     plt.figure()
     acquired_data = results.get_data(handle)
     if mult_axis is None:
         axis_grid = results.get_axis(handle)[0]
         axis_name = results.get_axis_name(handle)[0]
```

## laboneq/controller/communication.py

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
-from functools import lru_cache
+from functools import cached_property
 from typing import TYPE_CHECKING, Any, Dict, List
 
 import zhinst.core as zi
 from zhinst.toolkit import Session as TKSession
 
 from laboneq.controller.devices.zi_emulator import ziDAQServerEmulator
 from laboneq.controller.devices.zi_node_monitor import NodeMonitor
@@ -124,18 +124,20 @@
             self._log_get(method_name, daq_action.path)
 
     def get(self, daq_action):
         self._log_get("get", daq_action.path)
         daq_reply = self._api_wrapper("get", daq_action.path, flat=True)
         return self._api_reply_to_val_history_dict(daq_reply)[daq_action.path][-1]
 
-    def _actions_to_set_api_input(self, daq_actions):
+    def _actions_to_set_api_input(
+        self, daq_actions: list[DaqNodeSetAction]
+    ) -> list[list[Any]]:
         return [[action.path, action.value] for action in daq_actions]
 
-    def batch_set(self, daq_actions: List[DaqNodeAction]):
+    def batch_set(self, daq_actions: list[DaqNodeAction]):
         """Set the list of nodes in one call to API
 
         Parameters:
             daq_actions: a list of DaqNodeSetAction objects
 
         Returns:
             when all nodes are set
@@ -144,15 +146,15 @@
         if not isinstance(daq_actions, list):
             raise LabOneQControllerException("List expected")
 
         node_list = [daq_action.path for daq_action in daq_actions]
         _logger.debug("Batch set node list: %s", node_list)
 
         api_input = []
-        daq_actions_to_execute = []
+        daq_actions_to_execute: list[DaqNodeSetAction] = []
 
         for action in daq_actions:
             if not isinstance(action, DaqNodeSetAction):
                 raise LabOneQControllerException(
                     "List elements must be of type DaqNodeSetAction"
                 )
             if action.caching_strategy == CachingStrategy.CACHE:
@@ -259,16 +261,15 @@
             retval = api_method(*args, **kwargs)
             return retval
         except Exception as ex:
             raise LabOneQControllerException(
                 f"Exception {ex} when calling method {method_name} with {args} and {kwargs}"
             )
 
-    @property
-    @lru_cache(maxsize=1)
+    @cached_property
     def toolkit_session(self) -> TKSession:
         """Toolkit session from the initialized DAQ session."""
         return TKSession(
             server_host=self.server_qualifier.host,
             server_port=self.server_qualifier.port,
             connection=self._zi_api_object,
         )
```

## laboneq/controller/controller.py

```diff
@@ -39,15 +39,15 @@
     pre_process_compiled,
 )
 from laboneq.controller.results import (
     build_partial_result,
     make_acquired_result,
     make_empty_results,
 )
-from laboneq.controller.util import LabOneQControllerException
+from laboneq.controller.util import LabOneQControllerException, SweepParamsTracker
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 from laboneq.core.types.enums.averaging_mode import AveragingMode
 from laboneq.core.utilities.replace_pulse import ReplacementType, calc_wave_replacements
 from laboneq.executor.executor import ExecutorBase, LoopingMode, LoopType
 
 if TYPE_CHECKING:
     from laboneq.core.types import CompiledExperiment
@@ -513,14 +513,32 @@
         near-time loop without experiment recompilation.
 
         Args:
             pulse_uid: pulse to replace, can be Pulse object or uid of the pulse
             pulse_or_array: replacement pulse, can be Pulse object or value array
             (see sampled_pulse_* from the pulse library)
         """
+        if isinstance(pulse_uid, str):
+            for waveform in self._recipe_data.compiled.pulse_map[
+                pulse_uid
+            ].waveforms.values():
+                if any([instance.can_compress for instance in waveform.instances]):
+                    _logger.error(
+                        "Pulse replacement on pulses that allow compression not allowed. Pulse %s",
+                        pulse_uid,
+                    )
+                    return
+
+        if hasattr(pulse_uid, "can_compress") and pulse_uid.can_compress:
+            _logger.error(
+                "Pulse replacement on pulses that allow compression not allowed. Pulse %s",
+                pulse_uid.uid,
+            )
+            return
+
         acquisition_type = RtExecutionInfo.get_acquisition_type(
             self._recipe_data.rt_execution_infos
         )
         wave_replacements = calc_wave_replacements(
             self._recipe_data.compiled, pulse_uid, pulse_or_array, self._current_waves
         )
         for repl in wave_replacements:
@@ -556,17 +574,15 @@
                         waveform=repl.samples,
                         awg_index=awg[1],
                         wave_index=target_wave[0],
                         acquisition_type=acquisition_type,
                     )
                 )
 
-    def _prepare_rt_execution(
-        self, rt_section_uid: str
-    ) -> Tuple[List[DaqNodeAction], AcquisitionType]:
+    def _prepare_rt_execution(self, rt_section_uid: str) -> list[DaqNodeAction]:
         if rt_section_uid is None:
             return [], []  # Old recipe-based execution - skip RT preparation
         rt_execution_info = self._recipe_data.rt_execution_infos[rt_section_uid]
         self._nodes_from_user_functions.sort(key=lambda v: v.path)
         nodes_to_prepare_rt = [*self._nodes_from_user_functions]
         self._nodes_from_user_functions.clear()
         for _, device in self._devices.leaders:
@@ -592,20 +608,21 @@
             )
         return nodes_to_prepare_rt
 
     class NearTimeExecutor(ExecutorBase):
         def __init__(self, controller: Controller):
             super().__init__(looping_mode=LoopingMode.EXECUTE)
             self.controller = controller
-            self.step_param_nodes = []
-            self.nt_loop_indices: List[int] = []
+            self.user_set_nodes = []
+            self.nt_loop_indices: list[int] = []
+            self.sweep_params_tracker = SweepParamsTracker()
 
         def set_handler(self, path: str, value):
             dev = self.controller._devices.find_by_node_path(path)
-            self.step_param_nodes.append(
+            self.user_set_nodes.append(
                 DaqNodeSetAction(
                     dev._daq, path, value, caching_strategy=CachingStrategy.NO_CACHE
                 )
             )
 
         def user_func_handler(self, func_name: str, args: Dict[str, Any]):
             func = self.controller._user_functions.get(func_name)
@@ -623,20 +640,15 @@
             self,
             name: str,
             index: int,
             value: float,
             axis_name: str,
             values: npt.ArrayLike,
         ):
-            device_ids = self.controller._recipe_data.param_to_device_map.get(name, [])
-            for device_id in device_ids:
-                device = self.controller._devices.find_by_uid(device_id)
-                self.step_param_nodes.extend(
-                    device.collect_prepare_sweep_step_nodes_for_param(name, value)
-                )
+            self.sweep_params_tracker.set_param(name, value)
 
         def for_loop_handler(
             self, count: int, index: int, loop_type: LoopType, enter: bool
         ):
             if enter:
                 self.nt_loop_indices.append(index)
             else:
@@ -647,19 +659,36 @@
             count: int,
             uid: str,
             averaging_mode: AveragingMode,
             acquisition_type: AcquisitionType,
             enter: bool,
         ):
             if enter:
+                affected_devices: set[str] = set()
+                for param in self.sweep_params_tracker.updated_params():
+                    affected_devices.update(
+                        self.controller._recipe_data.param_to_device_map.get(param, [])
+                    )
+                nt_sweep_nodes: list[DaqNodeAction] = []
+                for device_id in affected_devices:
+                    device = self.controller._devices.find_by_uid(device_id)
+                    nt_sweep_nodes.extend(
+                        device.collect_prepare_sweep_step_nodes_for_param(
+                            self.sweep_params_tracker
+                        )
+                    )
+                self.sweep_params_tracker.clear_for_next_step()
+
                 step_prepare_nodes = self.controller._prepare_rt_execution(
                     rt_section_uid=uid
                 )
-                batch_set([*self.step_param_nodes, *step_prepare_nodes])
-                self.step_param_nodes.clear()
+
+                batch_set([*self.user_set_nodes, *nt_sweep_nodes, *step_prepare_nodes])
+                self.user_set_nodes.clear()
+
                 for retry in range(3):  # Up to 3 retries
                     if retry > 0:
                         _logger.info("Step retry %s of 3...", retry + 1)
                         batch_set(step_prepare_nodes)
                     try:
                         self.controller._execute_one_step(acquisition_type)
                         self.controller._read_one_step_results(
```

## laboneq/controller/laboneq_logging.py

```diff
@@ -53,20 +53,22 @@
             stream: ext://sys.stderr
 
         file_handler:
             class: logging.FileHandler
             level: NOTSET
             formatter: file_formatter
             filename: \"controller.log\"
+            encoding: utf-8
 
         node_log_handler:
             class: logging.FileHandler
             level: NOTSET
             formatter: node_log_formatter
             filename: \"node.log\"
+            encoding: utf-8
 
     root:
         level: NOTSET
         handlers: [error_handler]
 
     loggers:
         laboneq:
@@ -117,15 +119,17 @@
     logging.config.dictConfig(config)
 
     performance_log_file = None
     if performance_log:
         performance_log_file = os.path.abspath(
             os.path.join(get_log_dir(), "controller_perf.log")
         )
-        performance_handler = logging.FileHandler(performance_log_file, mode="a")
+        performance_handler = logging.FileHandler(
+            performance_log_file, mode="a", encoding="utf-8"
+        )
         performance_handler.setLevel(logging.DEBUG)
         formatter = logging.Formatter(
             fmt="%(asctime)s.%(msecs)03d\t%(levelname)s\t%(name)-30s\t%(message)s",
             datefmt="%Y-%m-%d %H:%M:%S",
         )
         performance_handler.setFormatter(formatter)
         root_logger = logging.getLogger()
```

## laboneq/controller/recipe_1_4_0.py

```diff
@@ -119,14 +119,15 @@
             "gains",
             "range",
             "range_unit",
             "precompensation",
             "lo_frequency",
             "port_mode",
             "port_delay",
+            "scheduler_port_delay",
             "delay_signal",
             "marker_mode",
         )
         ordered = True
 
     @dataclass
     class Data:
@@ -139,14 +140,15 @@
         gains: Optional[Gains] = None
         range: Optional[float] = None
         range_unit: Optional[str] = None
         precompensation: Optional[Dict[str, Dict]] = None
         lo_frequency: Optional[float] = None
         port_mode: Optional[str] = None
         port_delay: Optional[float] = None
+        scheduler_port_delay: float = 0.0
         delay_signal: Optional[float] = None
         marker_mode: Optional[str] = None
 
     channel = fields.Integer()
     enable = fields.Boolean(required=False)
     modulation = fields.Boolean(required=False)
     oscillator = fields.Integer(required=False)
@@ -155,14 +157,15 @@
     gains = fields.Nested(Gains, required=False)
     range = fields.Float(required=False)
     range_unit = fields.Str(required=False)
     precompensation = fields.Dict(required=False)
     lo_frequency = fields.Float(required=False)
     port_mode = fields.Str(required=False)
     port_delay = fields.Float(required=False)
+    scheduler_port_delay = fields.Float(required=False)
     delay_signal = fields.Float(required=False)
     marker_mode = fields.Str(required=False)
 
 
 class SignalTypeField(fields.Field):
     def _serialize(self, value, attr, obj, **kwargs):
         return value.name
@@ -321,24 +324,22 @@
     count = fields.Integer(required=False)
     parameters = fields.List(fields.Nested(Parameter), required=False)
     children = fields.List(fields.Nested(lambda: Execution()), required=False)
 
 
 class Measurement(QCCSSchema):
     class Meta:
-        fields = ("length", "delay", "channel")
+        fields = ("length", "channel")
 
     @dataclass
     class Data:
         length: int
-        delay: int
         channel: int = 0
 
     length = fields.Integer()
-    delay = fields.Integer()
     channel = fields.Integer()
 
 
 class RefClkTypeField(fields.Field):
     def _serialize(self, value, attr, obj, **kwargs):
         return value.name
```

## laboneq/controller/util.py

```diff
@@ -18,7 +18,26 @@
     def __init__(self, wrapped_object):
         self._wrapped_object = wrapped_object
 
     def __getattr__(self, attr):
         if attr in self.__dict__:
             return getattr(self, attr)
         return getattr(self._wrapped_object, attr)
+
+
+class SweepParamsTracker:
+    def __init__(self):
+        self.sweep_param_values: dict[str, float] = {}
+        self.sweep_param_updates: set[str] = set()
+
+    def set_param(self, param: str, value: float):
+        self.sweep_param_values[param] = value
+        self.sweep_param_updates.add(param)
+
+    def updated_params(self) -> set[str]:
+        return self.sweep_param_updates
+
+    def clear_for_next_step(self):
+        self.sweep_param_updates.clear()
+
+    def get_param(self, param: str) -> float:
+        return self.sweep_param_values[param]
```

## laboneq/controller/devices/device_hdawg.py

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 
 from laboneq.controller.communication import (
     CachingStrategy,
     DaqNodeAction,
     DaqNodeSetAction,
 )
-from laboneq.controller.devices.device_zi import DeviceZI
+from laboneq.controller.devices.device_zi import DeviceZI, delay_to_rounded_samples
 from laboneq.controller.devices.zi_node_monitor import (
     Command,
     Condition,
     FloatWithTolerance,
     NodeControlBase,
     Prepare,
     Response,
@@ -262,26 +262,30 @@
                         f"sigouts/{output.channel}/range",
                         output.range,
                     )
                 )
             nodes.append((f"sigouts/{output.channel}/offset", output.offset))
             nodes.append((f"awgs/{awg_idx}/single", 1))
 
-            measurement_delay_rounded = (
-                self._get_total_rounded_delay_samples(
-                    output,
-                    self._sampling_rate,
-                    DELAY_NODE_GRANULARITY_SAMPLES,
-                    DELAY_NODE_MAX_SAMPLES,
-                    0,
+            output_delay = output.scheduler_port_delay
+            output_delay += output.port_delay or 0.0
+
+            output_delay_rounded = (
+                delay_to_rounded_samples(
+                    channel=output.channel,
+                    dev_repr=self.dev_repr,
+                    delay=output_delay,
+                    sample_frequency_hz=self._sampling_rate,
+                    granularity_samples=DELAY_NODE_GRANULARITY_SAMPLES,
+                    max_node_delay_samples=DELAY_NODE_MAX_SAMPLES,
                 )
                 / self._sampling_rate
             )
 
-            nodes.append((f"sigouts/{output.channel}/delay", measurement_delay_rounded))
+            nodes.append((f"sigouts/{output.channel}/delay", output_delay_rounded))
 
             awg_ch = output.channel % 2
             iq_idx = output.channel // 2
             iq_gains_mx = device_recipe_data.iq_settings.get(iq_idx, None)
 
             if iq_gains_mx is None:
                 # Fall back to old behavior (suitable for single channel output)
```

## laboneq/controller/devices/device_shfppc.py

```diff
@@ -5,14 +5,15 @@
 
 from collections import defaultdict
 
 from laboneq.controller.communication import DaqNodeAction, DaqNodeSetAction
 from laboneq.controller.devices.device_zi import DeviceZI
 from laboneq.controller.recipe_1_4_0 import Initialization
 from laboneq.controller.recipe_processor import DeviceRecipeData
+from laboneq.controller.util import SweepParamsTracker
 
 
 class DeviceSHFPPC(DeviceZI):
     param_keys = ["pump_freq", "pump_power", "probe_frequency", "probe_power"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -81,13 +82,18 @@
                     DaqNodeSetAction(
                         self._daq, self._key_to_path(key, ch), _convert(value)
                     )
                 )
         return nodes_to_set
 
     def collect_prepare_sweep_step_nodes_for_param(
-        self, param: str, value: float
+        self, sweep_params_tracker: SweepParamsTracker
     ) -> list[DaqNodeAction]:
         nodes_to_set: list[DaqNodeAction] = []
-        for path in self._param_to_paths.get(param, []):
-            nodes_to_set.append(DaqNodeSetAction(self._daq, path, value))
+        for param in sweep_params_tracker.updated_params():
+            for path in self._param_to_paths.get(param, []):
+                nodes_to_set.append(
+                    DaqNodeSetAction(
+                        self._daq, path, sweep_params_tracker.get_param(param)
+                    )
+                )
         return nodes_to_set
```

## laboneq/controller/devices/device_shfqa.py

```diff
@@ -12,15 +12,15 @@
 
 from laboneq.controller.communication import (
     CachingStrategy,
     DaqNodeAction,
     DaqNodeGetAction,
     DaqNodeSetAction,
 )
-from laboneq.controller.devices.device_zi import DeviceZI
+from laboneq.controller.devices.device_zi import DeviceZI, delay_to_rounded_samples
 from laboneq.controller.recipe_1_4_0 import (
     IO,
     Initialization,
     IntegratorAllocation,
     Measurement,
 )
 from laboneq.controller.recipe_enums import DIOConfigType
@@ -485,21 +485,25 @@
                 DaqNodeSetAction(
                     self._daq,
                     f"/{self.serial}/qachannels/{output.channel}/generator/single",
                     1,
                 )
             )
 
+            measurement_delay = output.scheduler_port_delay
+            measurement_delay += output.port_delay or 0.0
+
             measurement_delay_rounded = (
-                self._get_total_rounded_delay_samples(
-                    output,
-                    SAMPLE_FREQUENCY_HZ,
-                    DELAY_NODE_GRANULARITY_SAMPLES,
-                    DELAY_NODE_MAX_SAMPLES,
-                    0,
+                delay_to_rounded_samples(
+                    channel=output.channel,
+                    dev_repr=self.dev_repr,
+                    delay=measurement_delay,
+                    sample_frequency_hz=SAMPLE_FREQUENCY_HZ,
+                    granularity_samples=DELAY_NODE_GRANULARITY_SAMPLES,
+                    max_node_delay_samples=DELAY_NODE_MAX_SAMPLES,
                 )
                 / SAMPLE_FREQUENCY_HZ
             )
 
             nodes_to_initialize_output.append(
                 DaqNodeSetAction(
                     self._daq,
@@ -607,26 +611,27 @@
         dev_output: IO.Data,
         measurement: Measurement.Data | None,
         device_uid: str,
         recipe_data: RecipeData,
     ):
         _logger.debug("%s: Setting measurement mode to 'Readout'.", self.dev_repr)
 
-        measurement_delay_output = 0
-        if dev_output is not None:
-            if dev_output.port_delay is not None:
-                measurement_delay_output += dev_output.port_delay * SAMPLE_FREQUENCY_HZ
+        measurement_delay = dev_output.scheduler_port_delay
+        measurement_delay += dev_output.port_delay or 0.0
+        measurement_delay += dev_input.scheduler_port_delay
+        measurement_delay += dev_input.port_delay or 0.0
 
         measurement_delay_rounded = (
-            self._get_total_rounded_delay_samples(
-                dev_input,
-                SAMPLE_FREQUENCY_HZ,
-                DELAY_NODE_GRANULARITY_SAMPLES,
-                DELAY_NODE_MAX_SAMPLES,
-                measurement.delay + measurement_delay_output,
+            delay_to_rounded_samples(
+                channel=dev_output.channel,
+                dev_repr=self.dev_repr,
+                delay=measurement_delay,
+                sample_frequency_hz=SAMPLE_FREQUENCY_HZ,
+                granularity_samples=DELAY_NODE_GRANULARITY_SAMPLES,
+                max_node_delay_samples=DELAY_NODE_MAX_SAMPLES,
             )
             / SAMPLE_FREQUENCY_HZ
         )
 
         nodes_to_set_for_readout_mode = [
             DaqNodeSetAction(
                 self._daq,
@@ -686,25 +691,29 @@
                     filename=wave_name,
                     caching_strategy=CachingStrategy.CACHE,
                 )
             )
         return nodes_to_set_for_readout_mode
 
     def _configure_spectroscopy_mode_nodes(
-        self, dev_input, measurement: Measurement.Data | None
+        self, dev_input: IO.Data, measurement: Measurement.Data | None
     ):
         _logger.debug("%s: Setting measurement mode to 'Spectroscopy'.", self.dev_repr)
 
+        measurement_delay = dev_input.scheduler_port_delay
+        measurement_delay += dev_input.port_delay or 0.0
+
         measurement_delay_rounded = (
-            self._get_total_rounded_delay_samples(
-                dev_input,
-                SAMPLE_FREQUENCY_HZ,
-                DELAY_NODE_GRANULARITY_SAMPLES,
-                DELAY_NODE_MAX_SAMPLES,
-                measurement.delay,
+            delay_to_rounded_samples(
+                channel=dev_input.channel,
+                dev_repr=self.dev_repr,
+                delay=measurement_delay,
+                sample_frequency_hz=SAMPLE_FREQUENCY_HZ,
+                granularity_samples=DELAY_NODE_GRANULARITY_SAMPLES,
+                max_node_delay_samples=DELAY_NODE_MAX_SAMPLES,
             )
             / SAMPLE_FREQUENCY_HZ
         )
 
         nodes_to_set_for_spectroscopy_mode = [
             DaqNodeSetAction(
                 self._daq,
```

## laboneq/controller/devices/device_uhfqa.py

```diff
@@ -10,15 +10,15 @@
 
 from laboneq.controller.communication import (
     CachingStrategy,
     DaqNodeAction,
     DaqNodeGetAction,
     DaqNodeSetAction,
 )
-from laboneq.controller.devices.device_zi import DeviceZI
+from laboneq.controller.devices.device_zi import DeviceZI, delay_to_rounded_samples
 from laboneq.controller.devices.zi_node_monitor import Command, NodeControlBase
 from laboneq.controller.recipe_1_4_0 import IO, Initialization, IntegratorAllocation
 from laboneq.controller.recipe_enums import DIOConfigType
 from laboneq.controller.recipe_processor import (
     AwgConfig,
     AwgKey,
     DeviceRecipeData,
@@ -532,21 +532,28 @@
                 DaqNodeSetAction(
                     self._daq,
                     f"/{self.serial}/qas/0/integration/length",
                     measurement.length,
                 )
             )
 
-            dev_input = None if inputs is None or len(inputs) == 0 else inputs[0]
-            measurement_delay_rounded = self._get_total_rounded_delay_samples(
-                dev_input,
-                SAMPLE_FREQUENCY_HZ,
-                DELAY_NODE_GRANULARITY_SAMPLES,
-                DELAY_NODE_MAX_SAMPLES,
-                measurement.delay,
+            if inputs is None or len(inputs) == 0:
+                measurement_delay = 0.0
+            else:
+                dev_input = inputs[0]
+                measurement_delay = dev_input.scheduler_port_delay
+                measurement_delay += dev_input.port_delay or 0.0
+
+            measurement_delay_rounded = delay_to_rounded_samples(
+                channel=dev_input.channel,
+                dev_repr=self.dev_repr,
+                delay=measurement_delay,
+                sample_frequency_hz=SAMPLE_FREQUENCY_HZ,
+                granularity_samples=DELAY_NODE_GRANULARITY_SAMPLES,
+                max_node_delay_samples=DELAY_NODE_MAX_SAMPLES,
             )
 
             nodes_to_initialize_measurement.append(
                 DaqNodeSetAction(
                     self._daq, f"/{self.serial}/qas/0/delay", measurement_delay_rounded
                 )
             )
```

## laboneq/controller/devices/device_zi.py

```diff
@@ -39,15 +39,15 @@
 )
 from laboneq.controller.recipe_processor import (
     AwgConfig,
     AwgKey,
     DeviceRecipeData,
     RecipeData,
 )
-from laboneq.controller.util import LabOneQControllerException
+from laboneq.controller.util import LabOneQControllerException, SweepParamsTracker
 from laboneq.core.types.enums.acquisition_type import AcquisitionType
 from laboneq.core.types.enums.averaging_mode import AveragingMode
 
 if TYPE_CHECKING:
     from laboneq.core.types import CompiledExperiment
 
 
@@ -88,14 +88,53 @@
 class DeviceQualifier:
     dry_run: bool = True
     driver: str = None
     server: DaqWrapper = None
     options: DeviceOptions = None
 
 
+def delay_to_rounded_samples(
+    channel: int,
+    dev_repr: str,
+    delay: float,
+    sample_frequency_hz,
+    granularity_samples,
+    max_node_delay_samples,
+) -> int:
+    if delay < 0:
+        raise LabOneQControllerException(
+            f"Negative node delay for device {dev_repr} and channel {channel} specified."
+        )
+
+    delay_samples = delay * sample_frequency_hz
+    # Quantize to granularity and round ties towards zero
+    delay_rounded = (
+        math.ceil(delay_samples / granularity_samples + 0.5) - 1
+    ) * granularity_samples
+
+    if delay_rounded > max_node_delay_samples:
+        raise LabOneQControllerException(
+            f"Maximum delay via {dev_repr}'s node is "
+            + f"{max_node_delay_samples / sample_frequency_hz * 1e9:.2f} ns - for larger "
+            + "values, use the delay_signal property."
+        )
+    if abs(delay_samples - delay_rounded) > 1:
+        _logger.debug(
+            "Node delay %.2f ns of %s, channel %d will be rounded to "
+            "%.2f ns, a multiple of %.0f samples.",
+            delay_samples / sample_frequency_hz * 1e9,
+            dev_repr,
+            channel,
+            delay_rounded / sample_frequency_hz * 1e9,
+            granularity_samples,
+        )
+
+    return delay_rounded
+
+
 class DeviceZI(ABC):
     def __init__(self, device_qualifier: DeviceQualifier):
         self._device_qualifier: DeviceQualifier = device_qualifier
         self._downlinks: dict[str, tuple[str, ReferenceType[DeviceZI]]] = {}
         self._uplinks: dict[str, ReferenceType[DeviceZI]] = {}
         self._rf_offsets: dict[int, float] = []
 
@@ -573,20 +612,22 @@
                     f"expected frequency: {expected_freqs}, actual: {freq}"
                 )
 
     def _adjust_frequency(self, freq):
         return freq
 
     def collect_prepare_sweep_step_nodes_for_param(
-        self, param: str, value: float
+        self, sweep_params_tracker: SweepParamsTracker
     ) -> list[DaqNodeAction]:
         nodes_to_set: list[DaqNodeAction] = []
         for osc in self._allocated_oscs:
-            if osc.param == param:
-                freq_value = self._adjust_frequency(value)
+            if osc.param in sweep_params_tracker.updated_params():
+                freq_value = self._adjust_frequency(
+                    sweep_params_tracker.get_param(osc.param)
+                )
                 nodes_to_set.append(
                     DaqNodeSetAction(
                         self._daq,
                         self._make_osc_path(next(iter(osc.channels)), osc.index),
                         freq_value,
                     )
                 )
@@ -973,59 +1014,14 @@
             # for proper testing of the logic we have to mock the data server better.
             # Currently is returns 0 for all nodes...
             check_errors(all_errors[error_node], self.dev_repr)
 
     def collect_reset_nodes(self) -> list[DaqNodeAction]:
         return [DaqNodeSetAction(self._daq, f"/{self.serial}/raw/error/clear", 1)]
 
-    def _get_total_rounded_delay_samples(
-        self,
-        port,
-        sample_frequency_hz,
-        granularity_samples,
-        max_node_delay_samples,
-        measurement_delay_samples=0,
-    ):
-        channel = 0
-        if port is not None:
-            if port.port_delay is not None:
-                measurement_delay_samples += port.port_delay * sample_frequency_hz
-                channel = port.channel
-        else:
-            _logger.debug(
-                "Port argument of %s is None, please check whether port delays are as specified.",
-                self.dev_repr,
-            )
-
-        if measurement_delay_samples < 0:
-            raise LabOneQControllerException(
-                f"Negative node delay for device {self.dev_repr} and channel {channel} specified."
-            )
-        # Quantize to granularity and round ties towards zero
-        measurement_delay_rounded = (
-            math.ceil(measurement_delay_samples / granularity_samples + 0.5) - 1
-        ) * granularity_samples
-        if measurement_delay_rounded > max_node_delay_samples:
-            raise LabOneQControllerException(
-                f"Maximum delay via {self.dev_repr}'s node is "
-                + f"{max_node_delay_samples / sample_frequency_hz * 1e9:.2f} ns - for larger "
-                + "values, use the delay_signal property."
-            )
-        if abs(measurement_delay_samples - measurement_delay_rounded) > 1:
-            _logger.debug(
-                "Node delay %.2f ns of %s, channel %d will be rounded to "
-                "%.2f ns, a multiple of %.0f samples.",
-                measurement_delay_samples / sample_frequency_hz * 1e9,
-                self.dev_repr,
-                channel,
-                measurement_delay_rounded / sample_frequency_hz * 1e9,
-                granularity_samples,
-            )
-        return measurement_delay_rounded
-
 
 class ErrorLevels(Enum):
     info = 0
     warning = 1
     error = 2
```

## laboneq/core/types/compiled_experiment.py

```diff
@@ -30,14 +30,15 @@
     play_pulse_parameters: Optional[Dict[str, Any]] = field(default_factory=dict)
     pulse_pulse_parameters: Optional[Dict[str, Any]] = field(default_factory=dict)
 
     # uid of pulses that this instance overlaps with
     overlaps: List[str] = None
     has_marker1: bool = False
     has_marker2: bool = False
+    can_compress: bool = False
 
 
 @dataclass
 class PulseWaveformMap:
     """Data structure to store mappings between the given pulse and an AWG waveform."""
 
     sampling_rate: float
```

## laboneq/dsl/calibration/calibration.py

```diff
@@ -1,34 +1,48 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from dataclasses import dataclass, field
-from typing import Dict
+from typing import Any, Dict
 
 from laboneq.dsl.calibration.calibration_item import CalibrationItem
 
 
+def _sanitize_key(key: Any) -> str:
+    try:
+        return key.path
+    except AttributeError as error:
+        if not isinstance(key, str):
+            raise TypeError("Key must be a string.") from error
+        return key
+
+
 @dataclass(init=True, repr=True, order=True)
 class Calibration:
     """Calibration object containing a dict of :class:`~.CalibrationItem`.
 
     The dictionary has the path i.e. UID to the :py:class:`~.Calibratable` object as
     key and the actual :py:class:`~.CalibrationItem` object as value.
     """
 
     calibration_items: Dict[str, CalibrationItem] = field(default_factory=dict)
 
+    def __post_init__(self):
+        self.calibration_items = {
+            _sanitize_key(k): v for k, v in self.calibration_items.items()
+        }
+
     def __getitem__(self, key):
-        return self.calibration_items[key]
+        return self.calibration_items[_sanitize_key(key)]
 
     def __setitem__(self, key, value):
-        self.calibration_items[key] = value
+        self.calibration_items[_sanitize_key(key)] = value
 
     def __delitem__(self, key):
-        del self.calibration_items[key]
+        del self.calibration_items[_sanitize_key(key)]
 
     def __iter__(self):
         return iter(self.calibration_items)
 
     def __len__(self):
         return len(self.calibration_items)
```

## laboneq/dsl/device/qubits.py

```diff
@@ -30,26 +30,28 @@
         parameters: Dict[str, Any] = None,
     ):
         """
         Initializes a new QuantumElement object.
 
         Args:
             uid: A unique identifier for the quantum element.
-            logical_signals: A dictionary of logical signals associated with the quantum element.
+            signals: A dictionary of logical signals associated with the quantum element.
             logical_signal_group: A logical signal group associated with the quantum element.
             parameters: A dictionary of parameters associated with the quantum element.
         """
-        if uid is None:
-            self.uid = uuid.uuid4().hex
-        else:
-            self.uid = uid
-        self.signals = {} if signals is None else signals
-
+        self.uid = uuid.uuid4().hex if uid is None else uid
+        self.signals = (
+            {
+                k: (v.uid if isinstance(v, LogicalSignal) else v)
+                for k, v in signals.items()
+            }
+            if signals
+            else {}
+        )
         self._parameters = {} if parameters is None else parameters
-
         if logical_signal_group is not None:
             if signals:
                 raise ValueError("Cannot have both signals and logical signal_group")
             else:
                 self.signals = self._parse_signals(logical_signal_group)
 
     def __hash__(self):
@@ -95,15 +97,15 @@
     def set_signal_group(self, logical_signal_group: LogicalSignalGroup):
         """
         Sets the logical signal group for the quantum element.
 
         Args:
             logical_signal_group: The logical signal group to set for the quantum element.
         """
-        self.signals.update(self._parse_signal(logical_signal_group))
+        self.signals.update(self._parse_signals(logical_signal_group))
 
     def set_parameters(self, parameters: Dict[str, Any]):
         """
         Sets the parameters for the quantum element.
         Allowed datatypes for the parameters are the following: Integer, Boolean, Float, Complex numbers,
         Numpy arrays of the above, Strings, Dictionaries of the above, LabOne Q types and None.
```

## laboneq/dsl/experiment/pulse.py

```diff
@@ -41,14 +41,16 @@
 class PulseSampledReal(Pulse):
     """Pulse based on a list of real-valued samples."""
 
     #: List of real values.
     samples: ArrayLike
     #: Unique identifier of the pulse.
     uid: str = field(default_factory=pulse_id_generator)
+    #: Flag indicating whether the compiler should attempt to compress this pulse
+    can_compress: bool = field(default=False)
 
     def __post_init__(self):
         if not isinstance(self.uid, str):
             raise LabOneQException("PulseSampledReal must have a string uid")
         self.samples = np.array(self.samples)
         shape = np.shape(self.samples)
         if not len(shape) == 1:
@@ -67,14 +69,16 @@
 class PulseSampledComplex(Pulse):
     """Pulse base on a list of complex-valued samples."""
 
     #: Complex-valued data.
     samples: ArrayLike
     #: Unique identifier of the pulse.
     uid: str = field(default_factory=pulse_id_generator)
+    #: Flag indicating whether the compiler should attempt to compress this pulse
+    can_compress: bool = field(default=False)
 
     def __post_init__(self):
         if not isinstance(self.uid, str):
             raise LabOneQException("PulseSampledComplex must have a string uid")
 
         if not np.iscomplexobj(self.samples):
             shape = np.shape(self.samples)
@@ -103,13 +107,16 @@
 
     #: Amplitude of the pulse.
     amplitude: float = field(default=None)
 
     #: Length of the pulse in seconds.
     length: float = field(default=None)
 
+    #: Flag indicating whether the compiler should attempt to compress this pulse
+    can_compress: bool = field(default=False)
+
     #: Optional (re)binding of user pulse parameters
     pulse_parameters: Optional[Dict[str, Any]] = field(default=None)
 
     def __post_init__(self):
         if not isinstance(self.uid, str):
             raise LabOneQException(f"{PulseFunctional.__name__} must have a string uid")
```

## laboneq/dsl/experiment/pulse_library.py

```diff
@@ -65,32 +65,35 @@
     else:
         function_name = name
 
     def factory(
         uid: str = None,
         length: float = 100e-9,
         amplitude: float = 1.0,
+        can_compress=False,
         **pulse_parameters: Dict[str, Any],
     ):
         if pulse_parameters == {}:
             pulse_parameters = None
         if uid is None:
             return PulseFunctional(
                 function=function_name,
                 length=length,
                 amplitude=amplitude,
                 pulse_parameters=pulse_parameters,
+                can_compress=can_compress,
             )
         else:
             return PulseFunctional(
                 function=function_name,
                 uid=uid,
                 length=length,
                 amplitude=amplitude,
                 pulse_parameters=pulse_parameters,
+                can_compress=can_compress,
             )
 
     factory.__name__ = function_name
     factory.__doc__ = sampler.__doc__
     # we do not wrap __qualname__, it throws off the documentation generator
 
     pulse_function_library[function_name] = sampler
@@ -240,37 +243,37 @@
 
     Returns:
         Raised cosine pulse.
     """
     return np.cos(x * np.pi / 2) ** 2
 
 
-def sampled_pulse_real(samples, uid=None):
+def sampled_pulse_real(samples, uid=None, can_compress=False):
     """Create a pulse based on a array of real values.
 
     Args:
         samples: Real valued data.
         uid: Unique identifier of the created pulse.
 
     Returns:
         Pulse based on the provided sample values.
     """
     if uid is None:
-        return PulseSampledReal(samples=samples)
+        return PulseSampledReal(samples=samples, can_compress=can_compress)
     else:
-        return PulseSampledReal(uid=uid, samples=samples)
+        return PulseSampledReal(uid=uid, samples=samples, can_compress=can_compress)
 
 
-def sampled_pulse_complex(samples, uid=None):
+def sampled_pulse_complex(samples, uid=None, can_compress=False):
     """Create a pulse based on a array of complex values.
 
     Args:
         samples: Complex valued data.
         uid: Unique identifier of the created pulse.
 
     Returns:
         Pulse based on the provided sample values.
     """
     if uid is None:
-        return PulseSampledComplex(samples=samples)
+        return PulseSampledComplex(samples=samples, can_compress=can_compress)
     else:
-        return PulseSampledComplex(uid=uid, samples=samples)
+        return PulseSampledComplex(uid=uid, samples=samples, can_compress=can_compress)
```

## laboneq/dsl/serialization/serializer.py

```diff
@@ -99,14 +99,15 @@
             "laboneq.dsl.calibration.oscillator",
             "laboneq.dsl.calibration.signal_calibration",
             "laboneq.dsl.result.results",
             "laboneq.dsl.parameter",
             "laboneq.dsl.calibration",
             "laboneq.dsl.device",
             "laboneq.dsl.device.qubits",
+            "laboneq.dsl.device.quops",
             "laboneq.dsl.device.server",
             "laboneq.dsl.device.servers.data_server",
             "laboneq.core.types.enums",
             "laboneq.core.types.compiled_experiment",
             "laboneq.dsl.device.io_units.logical_signal",
             "laboneq.dsl.device.io_units.physical_channel",
             "laboneq.dsl.device.instruments",
```

## laboneq/openqasm3/expression.py

```diff
@@ -1,15 +1,19 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
+from __future__ import annotations
+
 import math
 import operator
+from typing import Iterable, Optional, Type
 
 from openqasm3 import ast
 
+from .namespace import ClassicalRef, Namespace, QubitRef
 from .openqasm_error import OpenQasmException
 
 binary_ops = {
     "+": operator.add,
     "-": operator.sub,
     "*": operator.mul,
     "/": operator.truediv,
@@ -41,15 +45,19 @@
     }
 
     if duration.unit == ast.TimeUnit.dt:
         raise OpenQasmException("Backend-dependent duration not supported")
     return val * scale[duration.unit]
 
 
-def eval_expression(expression: ast.Expression):
+def _eval_expression(
+    expression: ast.Expression | ast.DiscreteSet | None, namespace: Namespace
+):
+    if expression is None:
+        return None
     if isinstance(
         expression,
         (
             ast.IntegerLiteral,
             ast.FloatLiteral,
             ast.BooleanLiteral,
             ast.BitstringLiteral,
@@ -63,28 +71,167 @@
     if isinstance(expression, ast.BinaryExpression):
         try:
             op = binary_ops[expression.op.name]
         except KeyError as e:
             raise OpenQasmException(
                 f"Unsupported operator '{expression.op.name}'", expression.span
             ) from e
-        lhs = eval_expression(expression.lhs)
-        rhs = eval_expression(expression.rhs)
+        lhs = _eval_expression(expression.lhs, namespace)
+        rhs = _eval_expression(expression.rhs, namespace)
         return op(lhs, rhs)
     if isinstance(expression, ast.UnaryExpression):
         try:
             op = unary_ops[expression.op.name]
         except KeyError as e:
             raise OpenQasmException(
                 f"Unsupported operator '{expression.op}'", expression.span
             ) from e
-        return op(eval_expression(expression.expression))
+        return op(_eval_expression(expression.expression, namespace))
 
     if isinstance(expression, ast.Identifier):
         try:
             return constants[expression.name]
+        except KeyError:
+            pass
+        value = eval_lvalue(expression, namespace)
+        if isinstance(value, QubitRef):
+            return value
+        if isinstance(value, ClassicalRef):
+            # in an expression (rvalue), we can safely dereference classical values
+            return value.value
+        else:  # value is a list; dereference classical references
+            return [v.value if isinstance(v, ClassicalRef) else v for v in value]
+    if isinstance(expression, ast.RangeDefinition):
+        start = _eval_expression(expression.start, namespace)
+        end = _eval_expression(expression.end, namespace)
+        end += 1 if end >= start else -1
+        step = _eval_expression(expression.step, namespace) or 1
+        return range(start, end, step)
+    if isinstance(expression, ast.DiscreteSet):
+        return [_eval_expression(x, namespace) for x in expression.values]
+
+    if isinstance(expression, ast.IndexExpression):
+        collection = _eval_expression(expression.collection, namespace)
+        if not isinstance(collection, list):
+            raise OpenQasmException("Collection expected", mark=expression.span)
+        if isinstance(expression.index, list):
+            indices = [_eval_expression(i, namespace) for i in expression.index]
+        elif isinstance(expression.index, ast.DiscreteSet):
+            indices = _eval_expression(expression.index, namespace)
+        retval = []
+        for index in indices:
+            try:
+                if isinstance(index, Iterable):
+                    retval.extend([collection[i] for i in index])
+                else:
+                    retval.append(collection[index])
+            except IndexError as e:
+                raise OpenQasmException(str(e), mark=expression.span)
+        if len(retval) == 1:
+            retval = retval[0]
+        return retval
+
+    if isinstance(expression, ast.IndexedIdentifier):
+        # IndexedIdentifier as an r-value
+        collection = _eval_expression(expression.name, namespace)
+        for index_element in expression.indices:
+            if not isinstance(index_element, list) and not len(index_element) == 1:
+                raise OpenQasmException("Unsupported index")
+            index = _eval_expression(index_element[0], namespace)
+            collection = collection[index]
+        if isinstance(collection, list) and len(collection) == 1:
+            return collection[0]
+        return collection
+
+    if isinstance(expression, ast.Concatenation):
+        lhs = _eval_expression(expression.lhs, namespace)
+        rhs = _eval_expression(expression.rhs, namespace)
+        return [*lhs, *rhs]
+
+    raise OpenQasmException(
+        "Failed to evaluate expression", getattr(expression, "span", None)
+    )
+
+
+def eval_expression(
+    expression: Optional[ast.Expression],
+    *,
+    namespace: Namespace = None,
+    type: Type = None,
+):
+    if namespace is None:
+        namespace = Namespace()
+    retval = _eval_expression(expression, namespace)
+
+    if type is not None and not isinstance(retval, type):
+        raise OpenQasmException(
+            f"Expected expression of type {type}, got {type(retval)}", expression.span
+        )
+    return retval
+
+
+def eval_lvalue(
+    node, namespace: Namespace
+) -> ClassicalRef | QubitRef | list[ClassicalRef] | list[QubitRef]:
+    if isinstance(node, ast.Identifier):
+        if node.name in constants:
+            raise OpenQasmException("Cannot alias a constant", node.span)
+        try:
+            return namespace.lookup(node.name)
         except KeyError as e:
             raise OpenQasmException(
-                f"Unknown identifier '{expression.name}'", expression.span
+                f"Unknown identifier '{node.name}'", node.span
             ) from e
-
-    raise OpenQasmException("Failed to evaluate expression", expression.span)
+    if isinstance(node, ast.IndexedIdentifier):
+        identifier = node.name
+        if identifier.name in constants:
+            raise OpenQasmException("Cannot alias a constant", node.span)
+        collection = namespace.lookup(identifier.name)
+        if isinstance(collection, QubitRef):
+            raise OpenQasmException("Cannot index a single qubit", node.span)
+        for index_element in node.indices:
+            if isinstance(index_element, ast.DiscreteSet):
+                index = _eval_expression(index_element, namespace)
+            elif isinstance(index_element, list) and len(index_element) == 1:
+                index_element = index_element[0]
+                if isinstance(index_element, ast.RangeDefinition):
+                    index = _eval_expression(index_element, namespace)
+                else:
+                    index = [_eval_expression(index_element, namespace)]
+            else:
+                raise OpenQasmException("Unsupported index")
+
+            try:
+                collection = [collection[i] for i in index]
+            except Exception as e:
+                raise OpenQasmException(f"Indexing failed: {str(e)}", node.span) from e
+
+        if isinstance(collection, list) and len(collection) == 1:
+            return collection[0]
+        return collection
+
+    if isinstance(node, ast.IndexExpression):
+        # When aliasing an indexed identifier, e.g.:
+        #    let foo = bar[1];
+        # the RHS is currently parsed as an IndexExpression.
+        # We'll be storing it as an lvalue so it is not really an expression...
+        # We'll work around this by casting the syntax tree node to an IndexIdentifier
+        # and go from there.
+        if not isinstance(node.collection, ast.Identifier):
+            raise OpenQasmException("Identifier expected", node.collection.span)
+        new_node = ast.IndexedIdentifier(
+            name=node.collection,
+            indices=[node.index],
+        )
+        new_node.span = node.span
+        return eval_lvalue(new_node, namespace)
+
+    if isinstance(node, ast.Concatenation):
+        lhs = eval_lvalue(node.lhs, namespace=namespace)
+        rhs = eval_lvalue(node.rhs, namespace=namespace)
+        for node, lval in ((node.lhs, lhs), (node.rhs, rhs)):
+            if not isinstance(lval, list):
+                raise OpenQasmException(
+                    f"Array view expected, got {type(lval.__name__)}", node.span
+                )
+        return [*lhs, *rhs]
+    raise OpenQasmException("lvalue expected", node.span)
```

## laboneq/openqasm3/gate_store.py

```diff
@@ -6,19 +6,18 @@
 from laboneq.dsl.experiment import Section
 from laboneq.dsl.experiment.pulse import Pulse
 from laboneq.dsl.experiment.utils import id_generator
 
 
 class GateStore:
     def __init__(self):
-        self.gates: Dict[Tuple[str, Tuple[int, ...]], Callable[..., Section]] = {}
+        self.gates: Dict[Tuple[str, Tuple[str, ...]], Callable[..., Section]] = {}
         self.gate_map: Dict[str, str] = {}
-        self.qubit_lsg_map: Dict[int, str] = {}
 
-    def lookup_gate(self, name: str, qubits: Tuple[int, ...], args=()) -> Section:
+    def lookup_gate(self, name: str, qubits: Tuple[str, ...], args=()) -> Section:
         return self.gates[(self.gate_map.get(name, name), qubits)](*args)
 
     def map_gate(self, qasm_name: str, l1q_name: str):
         """Define mapping from qasm gate name to L1Q gate name."""
         self.gate_map[qasm_name] = l1q_name
 
     def register_gate_section(self, name, qubits, section_factory):
@@ -34,23 +33,14 @@
                 pulse=pulse,
                 increment_oscillator_phase=phase,
             )
             return gate
 
         return impl
 
-    def map_qubits(self, map: Dict[int, str]):
-        """Define mapping from qasm qubit names to LabOne Q logical signal groups.
-
-        Required by `GateStore.register_gate()`.
-        """
-        self.qubit_lsg_map.update(map)
-
     def register_gate(
-        self, name: str, qubit: int, pulse: Optional[Pulse], phase=None, id=None
+        self, name: str, qubit: str, pulse: Optional[Pulse], phase=None, id=None
     ):
         """Register a pulse as a single-qubit gate."""
         self.register_gate_section(
-            name,
-            (qubit,),
-            self._gate_pulse(self.qubit_lsg_map[qubit], pulse, phase, id),
+            name, (qubit,), self._gate_pulse(qubit, pulse, phase, id)
         )
```

## laboneq/openqasm3/openqasm3_importer.py

```diff
@@ -1,101 +1,90 @@
 # Copyright 2023 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
+import operator
 from collections import deque
+from contextlib import contextmanager
 from typing import Optional, TextIO, Union
 
 import openpulse
 import openpulse.ast as ast
 
 import openqasm3.visitor
 from laboneq.dsl.experiment import Section
 from laboneq.dsl.experiment.utils import id_generator
-from laboneq.openqasm3.expression import eval_expression
+from laboneq.openqasm3.expression import eval_expression, eval_lvalue
 from laboneq.openqasm3.gate_store import GateStore
+from laboneq.openqasm3.namespace import Namespace, QubitRef
 from laboneq.openqasm3.openqasm_error import OpenQasmException
-from laboneq.openqasm3.variable_store import VariableStore
+from laboneq.openqasm3.signal_store import SignalStore
 
 ALLOWED_NODE_TYPES = {
-    ast.Program,
-    ast.QuantumGate,
+    # quantum logic
     ast.Box,
-    ast.Identifier,
-    ast.IntegerLiteral,
-    ast.FloatLiteral,
-    ast.DurationLiteral,
-    ast.BitstringLiteral,
-    ast.BooleanLiteral,
-    ast.ImaginaryLiteral,
-    ast.BinaryExpression,
-    ast.BinaryOperator,
-    ast.UnaryExpression,
-    ast.UnaryOperator,
-    ast.Span,
+    ast.DelayInstruction,
+    ast.QuantumBarrier,
+    ast.QuantumGate,
+    ast.QuantumReset,
     ast.QubitDeclaration,
+    # auxiliary
     ast.AliasStatement,
-    ast.IndexExpression,
+    ast.ClassicalDeclaration,
+    ast.Concatenation,
+    ast.DiscreteSet,
+    ast.Identifier,
     ast.Include,
+    ast.Program,
     ast.RangeDefinition,
+    ast.Span,
+    ast.ClassicalAssignment,
+    # expressions
+    ast.BinaryExpression,
+    ast.BinaryOperator,
     ast.IndexedIdentifier,
-    ast.QuantumReset,
+    ast.IndexExpression,
+    ast.UnaryExpression,
+    ast.UnaryOperator,
+    ast.AssignmentOperator,
+    # literals
+    ast.BitstringLiteral,
+    ast.BooleanLiteral,
+    ast.DurationLiteral,
+    ast.FloatLiteral,
+    ast.ImaginaryLiteral,
+    ast.IntegerLiteral,
+    # types
+    ast.IntType,
+    ast.FloatType,
+    ast.BoolType,
+    ast.DurationType,
+    ast.BitType,
 }
 
 
 class AllowedNodeTypesVisitor(openqasm3.visitor.QASMVisitor):
     def generic_visit(self, node: ast.QASMNode, context=None):
         if type(node) not in ALLOWED_NODE_TYPES:
             raise OpenQasmException(
                 f"Node type {type(node)} not yet supported", mark=node.span
             )
         super().generic_visit(node, context)
 
 
-def get_collection_and_single_index(
-    expression: Union[ast.IndexExpression, ast.IndexedIdentifier]
-):
-    # todo: DiscreteSet as index
-    if isinstance(expression, ast.IndexExpression):
-        name_identifier = expression.collection
-        if len(expression.index) != 1:
-            return "invalid", None
-        ex0 = expression.index[0]
-    else:
-        assert isinstance(expression, ast.IndexedIdentifier)
-        name_identifier = expression.name
-        if len(expression.indices) != 1 or len(expression.indices[0]) != 1:
-            return "invalid", None
-        ex0 = expression.indices[0][0]
-
-    if not isinstance(name_identifier, ast.Identifier):
-        return None, None
-    collection = name_identifier.name
-    if isinstance(ex0, ast.RangeDefinition):
-        if not (
-            isinstance(ex0.start, ast.IntegerLiteral)
-            and isinstance(ex0.end, ast.IntegerLiteral)
-            and ex0.start.value == ex0.end.value
-        ):
-            return collection, None
-        return collection, ex0.start.value
-    elif isinstance(ex0, ast.IntegerLiteral):
-        return collection, ex0.value
-    else:
-        return collection, None
-
-
 class OpenQasm3Importer:
     def __init__(
-        self,
-        gate_store: GateStore,
+        self, gate_store: GateStore, signal_store: Optional[SignalStore] = None
     ):
         self.gate_store = gate_store
-        self.scoped_variables = deque([VariableStore({})])
+        self.signal_store = (
+            signal_store if signal_store is not None else SignalStore({})
+        )
+        self.scoped_variables = deque([Namespace()])
 
     def __call__(
         self,
         text: Optional[str] = None,
         file: Optional[TextIO] = None,
         filename: Optional[str] = None,
         stream: Optional[TextIO] = None,
@@ -110,173 +99,264 @@
         elif file:
             return self._import_text(file.read())
         elif stream:
             return self._import_text(stream.read())
         else:
             return self._import_text(text)
 
-    def _merge_scoped_variables(self):
-        result = VariableStore()
-        for vars in self.scoped_variables:
-            result.variables.update(vars.variables)
-            result.current_index += vars.current_index
-        return result
-
     def _import_text(self, text) -> Section:
         tree = openpulse.parse(text)
         assert isinstance(tree, ast.Program)
         AllowedNodeTypesVisitor().visit(tree, None)
         try:
-            return self.transpile(tree, uid_hint="root")
+            root = self.transpile(tree, uid_hint="root")
         except OpenQasmException as e:
             e.source = text
             raise
+        self.signal_store.leftover_raise()
+        return root
+
+    @contextmanager
+    def _new_scope(self):
+        parent_namespace = self.scoped_variables[-1]
+        self.scoped_variables.append(Namespace(parent=parent_namespace))
+        yield
+        self.scoped_variables.pop()
 
     def transpile(self, parent: Union[ast.Program, ast.Box], uid_hint="") -> Section:
         sect = Section(uid=id_generator(uid_hint))
-        self.scoped_variables.append(VariableStore({}))
 
         try:
             body = parent.statements
         except AttributeError:
             body = parent.body
 
         for child in body:
+            subsect = None
             try:
                 if isinstance(child, ast.QubitDeclaration):
                     self._handle_qubit_declaration(child)
+                elif isinstance(child, ast.ClassicalDeclaration):
+                    self._handle_classical_declaration(child)
                 elif isinstance(child, ast.AliasStatement):
                     self._handle_alias_statement(child)
                 elif isinstance(child, ast.Include):
                     self._handle_include(child)
                 elif isinstance(child, ast.QuantumGate):
-                    self._handle_quantum_gate(child, sect)
+                    subsect = self._handle_quantum_gate(child)
                 elif isinstance(child, ast.Box):
-                    self._handle_box(child, sect)
+                    subsect = self._handle_box(child)
+                elif isinstance(child, ast.QuantumBarrier):
+                    subsect = self._handle_barrier(child)
                 elif isinstance(child, ast.QuantumReset):
-                    self._handle_quantum_reset(child, sect)
+                    subsect = self._handle_quantum_reset(child)
+                elif isinstance(child, ast.DelayInstruction):
+                    subsect = self._handle_delay_instruction(child)
+                elif isinstance(child, ast.ClassicalAssignment):
+                    self._handle_assignment(child)
                 else:
                     raise OpenQasmException(
                         f"Statement type {type(child)} not supported",
                         mark=child.span,
                     )
+                if subsect is not None:
+                    sect.add(subsect)
             except OpenQasmException:
                 raise
             except Exception as e:
                 mark = child.span
                 raise OpenQasmException("Failed to process statement", mark) from e
+
         return sect
 
     def _handle_qubit_declaration(self, statement: ast.QubitDeclaration):
         name = statement.qubit.name
         try:
             if statement.size is not None:
-                if not isinstance(statement.size, ast.IntegerLiteral):
+                try:
+                    size = eval_expression(
+                        statement.size, namespace=self.scoped_variables[-1], type=int
+                    )
+                except Exception:
                     raise OpenQasmException(
-                        "Qubit declaration size must be an integer.",
+                        "Qubit declaration size must evaluate to an integer.",
                         mark=statement.span,
                     )
-                self.scoped_variables[-1].add_array_variable(name, statement.size.value)
+
+                # declare the individual qubits...
+                qubits = [
+                    self.scoped_variables[-1].declare_qubit(f"{name}[{i}]")
+                    for i in range(size)
+                ]
+                # ... as well as a list aliasing them
+                self.scoped_variables[-1].declare_reference(name, qubits)
             else:
-                self.scoped_variables[-1].add_variable(name)
+                self.scoped_variables[-1].declare_qubit(name)
         except ValueError as e:
             raise OpenQasmException(str(e), mark=statement.span) from e
+        except OpenQasmException as e:
+            e.mark = statement.span
+            raise
+
+    def _handle_classical_declaration(self, statement: ast.ClassicalDeclaration):
+        name = statement.identifier.name
+        if isinstance(statement.type, ast.BitType):
+            value = eval_expression(
+                statement.init_expression, namespace=self.scoped_variables[-1], type=int
+            )
+            size = statement.type.size
+            if size is not None:
+                size = eval_expression(
+                    size, namespace=self.scoped_variables[-1], type=int
+                )
+
+                # declare the individual bits...
+                bits = [
+                    self.scoped_variables[-1].declare_classical_value(
+                        f"{name}[{i}]", value=bool((value >> i) & 1)
+                    )
+                    for i in range(size)
+                ]
+                # ... as well as a list aliasing them
+                self.scoped_variables[-1].declare_reference(name, bits)
+            else:
+                self.scoped_variables[-1].declare_classical_value(name, value)
+        else:
+            value = eval_expression(
+                statement.init_expression, namespace=self.scoped_variables[-1]
+            )
+            self.scoped_variables[-1].declare_classical_value(name, value)
 
     def _handle_alias_statement(self, statement: ast.AliasStatement):
         if not isinstance(statement.target, ast.Identifier):
             raise OpenQasmException(
                 "Alias target must be an identifier.", mark=statement.span
             )
         name = statement.target.name
-        if isinstance(statement.value, ast.IndexExpression):
-            collection, idx = get_collection_and_single_index(statement.value)
-            if collection is None:
-                raise OpenQasmException(
-                    "Array name must be an identifier.", statement.span
-                )
-            if idx is None:
-                raise OpenQasmException(
-                    "Alias index must be a single integer.", mark=statement.span
-                )
-            try:
-                self.scoped_variables[-1].add_alias(name, collection, idx)
-            except ValueError as e:
-                raise OpenQasmException(str(e), mark=statement.span) from e
-        elif isinstance(statement.value, ast.Identifier):
-            try:
-                self.scoped_variables[-1].add_alias(name, statement.value.name)
-            except ValueError as e:
-                raise OpenQasmException(str(e), mark=statement.span) from e
-        else:
+
+        try:
+            value = eval_lvalue(statement.value, namespace=self.scoped_variables[-1])
+        except OpenQasmException:
+            raise
+        except Exception as e:
             raise OpenQasmException(
-                "Alias value must be an identifier or index expression.",
-                mark=statement.span,
-            )
+                "Invalid alias value", mark=statement.value.span
+            ) from e
+        try:
+            self.scoped_variables[-1].declare_reference(name, value)
+        except OpenQasmException as e:
+            e.mark = statement.span
+            raise
 
-    def _handle_quantum_gate(self, statement: ast.QuantumGate, parent: Section):
+    def _handle_quantum_gate(self, statement: ast.QuantumGate):
         args = tuple(eval_expression(arg) for arg in statement.arguments)
         if statement.modifiers or statement.duration:
             raise OpenQasmException(
                 "Gate modifiers and duration not yet supported.",
                 mark=statement.span,
             )
         if not isinstance(statement.name, ast.Identifier):
             raise OpenQasmException(
                 "Gate name must be an identifier.", mark=statement.span
             )
         name = statement.name.name
-        qubit_indices = tuple(self._get_qubit_index(q) for q in statement.qubits)
+        qubit_names = []
+        for q in statement.qubits:
+            qubit = eval_expression(q, namespace=self.scoped_variables[-1])
+            try:
+                qubit_names.append(qubit.canonical_name)
+            except AttributeError as e:
+                raise OpenQasmException(
+                    f"Qubit expected, got '{type(qubit).__name__}'", mark=q.span
+                ) from e
+        qubit_names = tuple(qubit_names)
         try:
-            parent.add(self.gate_store.lookup_gate(name, qubit_indices, args=args))
+            return self.gate_store.lookup_gate(name, qubit_names, args=args)
         except KeyError as e:
             raise OpenQasmException(
-                f"Gate '{name}' for qubit indices {qubit_indices} not found.",
+                f"Gate '{name}' for qubit(s) {qubit_names} not found.",
                 mark=statement.span,
             ) from e
 
-    def _handle_box(self, statement: ast.Box, parent: Section):
+    def _handle_box(self, statement: ast.Box):
         if statement.duration:
             raise ValueError("Box duration not yet supported.")
-        try:
-            parent.add(self.transpile(statement, uid_hint="box"))
-        except KeyError:
-            raise ValueError(f"Unable to add box for {parent}.")
+        with self._new_scope():
+            return self.transpile(statement, uid_hint="box")
+
+    def _handle_barrier(self, statement: ast.QuantumBarrier):
+        sect = Section(uid=id_generator("barrier"), length=0)
+        reserved_qubits = [
+            eval_expression(qubit, namespace=self.scoped_variables[-1]).canonical_name
+            for qubit in statement.qubits
+        ]
+        reserved_signals = set()
+        if not reserved_qubits:  # get all signals
+            for each_qubit_signals in self.signal_store.user_map.values():
+                for signal in each_qubit_signals:
+                    reserved_signals.add(signal.exp_signal)
+        for qubit in reserved_qubits:  # get only selected signals
+            for signal in self.signal_store.user_map[qubit]:
+                reserved_signals.add(signal.exp_signal)
+        for exp_signal in reserved_signals:
+            sect.reserve(exp_signal)
+        return sect
 
     def _handle_include(self, statement: ast.Include):
         if statement.filename != "stdgates.inc":
             raise OpenQasmException(
                 f"Only 'stdgates.inc' is supported for include, found '{statement.filename}'.",
                 mark=statement.span,
             )
 
-    def _handle_quantum_reset(self, statement: ast.QuantumReset, parent: Section):
+    def _handle_quantum_reset(self, statement: ast.QuantumReset):
         # Although ``qubits`` is plural, only a single qubit is allowed.
-        qubit_index = self._get_qubit_index(statement.qubits)
+        qubit_name = eval_expression(
+            statement.qubits, namespace=self.scoped_variables[-1]
+        ).canonical_name
         try:
-            parent.add(self.gate_store.lookup_gate("reset", (qubit_index,)))
+            return self.gate_store.lookup_gate("reset", (qubit_name,))
         except KeyError as e:
             raise OpenQasmException(
-                f"Reset gate for qubit index {qubit_index} not found.",
+                f"Reset gate for qubit '{qubit_name}' not found.",
                 mark=statement.span,
             ) from e
 
-    def _get_qubit_index(self, q: Union[ast.IndexedIdentifier, ast.Identifier]):
-        if isinstance(q, ast.Identifier):
-            try:
-                return self._merge_scoped_variables().get_qubit_number(q.name)
-            except (KeyError, ValueError) as e:
-                raise OpenQasmException(str(e), mark=q.span) from e
-        elif isinstance(q, ast.IndexedIdentifier):
-            collection, idx = get_collection_and_single_index(q)
-            if collection is None:
-                raise OpenQasmException(
-                    "Qubit name must be an identifier.", mark=q.span
-                )
-            if idx is None:
-                raise OpenQasmException(
-                    "Qubit index must be a single integer.", mark=q.span
-                )
-            return self._merge_scoped_variables().get_qubit_number(collection, idx)
-        else:
+    def _handle_delay_instruction(self, statement: ast.DelayInstruction):
+        qubits = statement.qubits
+        duration = eval_expression(
+            statement.duration, namespace=self.scoped_variables[-1], type=float
+        )
+        qubit_names = [
+            eval_expression(qubit, namespace=self.scoped_variables[-1]).canonical_name
+            for qubit in qubits
+        ]
+        qubits_str = "_".join(qubit_names)
+        delay_section = Section(
+            uid=id_generator(f"{qubits_str}_delay_{duration * 1e9:.0f}ns")
+        )
+        for qubit in qubit_names:
+            # todo: TBD only delaying drive signal?
+            delay_section.delay(signal=f"{qubit}_drive", time=duration)
+        return delay_section
+
+    def _handle_assignment(self, statement: ast.ClassicalAssignment):
+        lvalue = eval_lvalue(statement.lvalue, self.scoped_variables[-1])
+        if isinstance(lvalue, QubitRef):
+            raise OpenQasmException(f"Cannot assign to qubit '{lvalue.canonical_name}'")
+        if isinstance(lvalue, list):
+            raise OpenQasmException("Cannot assign to arrays")
+        ops = {
+            "=": lambda a, b: b,
+            "*=": operator.mul,
+            "/=": operator.truediv,
+            "+=": operator.add,
+            "-=": operator.sub,
+        }
+        try:
+            op = ops[statement.op.name]
+        except KeyError as e:
             raise OpenQasmException(
-                "Qubit names must be identifiers or index expressions.", mark=q.span
-            )
+                "Unsupported assignment operator", mark=statement.span
+            ) from e
+        rvalue = eval_expression(statement.rvalue, namespace=self.scoped_variables[-1])
+        lvalue.value = op(lvalue.value, rvalue)
```

## laboneq/openqasm3/reset_gate_factory.py

```diff
@@ -1,162 +1,150 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
-from enum import Enum
 from typing import TYPE_CHECKING, Callable, Optional
 
 from laboneq.dsl.experiment.acquire import Acquire
 from laboneq.dsl.experiment.play_pulse import PlayPulse
 from laboneq.dsl.experiment.pulse import Pulse
 from laboneq.dsl.experiment.section import Case, Match, Section
 from laboneq.dsl.experiment.utils import id_generator
+from laboneq.openqasm3.signal_store import SignalLineType
 
 if TYPE_CHECKING:
     from laboneq.openqasm3.openqasm3_importer import GateStore
 
 # todo: The following four blocks shall be moved once the corresponding task is to be
 #  implemented.
 
 
-class SignalLineType(Enum):
-    """An enum for the different signal line types."""
-
-    MEASURE = "measure"
-    ACQUIRE = "acquire"
-    DRIVE = "drive"
-
-
-def default_signal_mapper(signal_line_type: SignalLineType, qubit_index: int) -> str:
+def default_signal_mapper(signal_line_type: SignalLineType, qubit: str) -> str:
     """Default signal mapper.
 
     Args:
         signal_line_type: The signal line type to map.
-        qubit_index: The index of the qubit to map the signal for.
+        qubit: The name of the qubit to map the signal for.
 
     Returns:
         The mapped signal.
     """
-    return f"q{qubit_index}_{signal_line_type.value}"
+    return f"{qubit}_{signal_line_type.value}"
 
 
 def create_measure_gate(
-    qubit_index: int,
+    qubit: str,
     measure_pulse: Pulse,
     acquire_kernel: Pulse,
     handle: Optional[str] = None,
-    signal_mapper: Callable[[SignalLineType, int], str] = default_signal_mapper,
+    signal_mapper: Callable[[SignalLineType, str], str] = default_signal_mapper,
 ) -> Callable[[], Section]:
     """Creates a measure gate factory.
 
     Args:
-        qubit_index: The index of the qubit to measure.
+        qubit: The name of the qubit to measure.
         measure_pulse: The pulse to use for measure pulse.
         acquire_kernel: The pulse to use as integration kernel.
         handle: The handle to use for the acquire, auto-generated if not provided.
         signal_mapper: A callable to general a signal id from the line type and qubit
             index
 
     Returns:
         A section modelling the measure gate.
     """
 
     def impl():
-        uid = id_generator(f"measure_q{qubit_index}")
+        uid = id_generator(f"measure_{qubit}")
         nonlocal handle
         if handle is None:
             handle = uid
 
         measure_section = Section(uid=uid)
         measure_section.play(
-            signal=signal_mapper(SignalLineType.MEASURE, qubit_index),
+            signal=signal_mapper(SignalLineType.MEASURE, qubit),
             pulse=measure_pulse,
         )
         measure_section.acquire(
-            signal=signal_mapper(SignalLineType.ACQUIRE, qubit_index),
+            signal=signal_mapper(SignalLineType.ACQUIRE, qubit),
             kernel=acquire_kernel,
             handle=handle if handle is not None else uid,
         )
         return measure_section
 
     return impl
 
 
 def create_x_gate(
-    qubit_index: int,
+    qubit: str,
     x_pulse: Pulse,
     angle_deg: float,
-    signal_mapper: Callable[[SignalLineType, int], str] = default_signal_mapper,
+    signal_mapper: Callable[[SignalLineType, str], str] = default_signal_mapper,
 ) -> Callable[[], Section]:
     """Creates an x gate.
 
     Args:
-        qubit_index: The index of the qubit to apply the x gate to.
+        qubit: The name of the qubit to apply the x gate to.
         x_pulse: The pulse to use for the x gate.
 
     Returns:
         A section modelling the x gate.
     """
 
     def impl():
-        uid = id_generator(f"x{angle_deg}_q{qubit_index}")
+        uid = id_generator(f"x{angle_deg}_{qubit}")
 
         x_section = Section(uid=uid)
-        x_section.play(
-            signal=signal_mapper(SignalLineType.DRIVE, qubit_index), pulse=x_pulse
-        )
+        x_section.play(signal=signal_mapper(SignalLineType.DRIVE, qubit), pulse=x_pulse)
 
         return x_section
 
     return impl
 
 
 def create_reset_gate(
-    qubit_index: int,
+    qubit: str,
     local: bool,
     reuse_measurement_handle: bool,
     gate_store: GateStore,
 ) -> Callable[[], Section]:
     """Creates a reset gate.
 
     Args:
-        qubit_index: The index of the qubit to apply the reset gate to.
+        qubit: The name of the qubit to apply the reset gate to.
         local: Whether to use local feedback (SHFQC only) or go via the PQSC.
         reuse_measurement_handle: Whether to reuse the handle used for other
           measurements of this qubit or create a new handle
         gate_store: A dictionary of sections to use for the measure and flip pulse.
 
     Returns:
         A section modelling the reset gate.
     """
 
     def impl():
-        uid = id_generator(f"reset_q{qubit_index}_l{local}_r{reuse_measurement_handle}")
+        uid = id_generator(f"reset_{qubit}_l{local}_r{reuse_measurement_handle}")
         handle = None
 
-        acquire_section = gate_store.lookup_gate("measure", (qubit_index,))
+        acquire_section = gate_store.lookup_gate("measure", (qubit,))
         acquire_section.uid = uid + "_acquire"
         for c in acquire_section.children:
             if isinstance(c, Acquire):
                 if reuse_measurement_handle:
                     handle = c.handle
                 else:
-                    handle = id_generator(f"reset_q{qubit_index}")
+                    handle = id_generator(f"reset_{qubit}")
                     c.handle = handle
 
         if handle is None:
             raise RuntimeError(
-                f"No valid acquire operation in measurement gate for q{qubit_index}."
+                f"No valid acquire operation in measurement gate for {qubit}."
             )
 
         case0 = Case(uid=id_generator("NOOP"), state=0)
-        case1 = Case.from_section(
-            gate_store.lookup_gate("x180", (qubit_index,)), state=1
-        )
+        case1 = Case.from_section(gate_store.lookup_gate("x180", (qubit,)), state=1)
         signals = {p.signal for p in case1.children if isinstance(p, PlayPulse)}
         for s in signals:
             acquire_section.reserve(signal=s)
 
         match_section = Match(uid=uid + "_match", handle=handle, local=local)
         match_section.add(case0)
         match_section.add(case1)
```

## laboneq/simulator/seqc_parser.py

```diff
@@ -27,14 +27,16 @@
     FuncDef,
     If,
     Node,
     UnaryOp,
 )
 from pycparser.c_parser import CParser
 
+from laboneq.compiler.common.compiler_settings import EXECUTETABLEENTRY_LATENCY
+
 if TYPE_CHECKING:
     from laboneq.core.types.compiled_experiment import CompiledExperiment
 
 
 def precompensation_is_nonzero(precompensation):
     """Check whether the precompensation has any effect"""
     return precompensation is not None and (
@@ -49,18 +51,17 @@
 
 
 def precompensation_delay_samples(precompensation):
     """Compute the additional delay (in samples) caused by the precompensation"""
     if not precompensation_is_nonzero(precompensation):
         return 0
     delay = 72
-    try:
-        delay += 88 * len(precompensation["exponential"])
-    except KeyError:
-        pass
+    exponential = precompensation.get("exponential")
+    if exponential is not None:
+        delay += 88 * len(exponential)
     if precompensation.get("high_pass") is not None:
         delay += 96
     if precompensation.get("bounce") is not None:
         delay += 32
     if precompensation.get("FIR") is not None:
         delay += 136
     return delay
@@ -302,14 +303,15 @@
     PLAY_ZERO = auto()
     PLAY_WAVE = auto()
     START_QA = auto()
     SET_OSC_FREQ = auto()
     SET_TRIGGER = auto()
     SET_PRECOMP_CLEAR = auto()
     WAIT_WAVE = auto()
+    PLAY_HOLD = auto()
 
 
 @dataclass
 class SeqCEvent:
     start_samples: int
     length_samples: int
     operation: Operation
@@ -436,19 +438,23 @@
             "QA_INT_ALL": 0b1111111111111111,
             "QA_INT_NONE": 0,
             "QA_GEN_ALL": 0b1111111111111111,
             "QA_GEN_NONE": 0,
             "QA_DATA_PROCESSED": 0b1000000000100
             if descriptor.device_type == "SHFSG"
             else 0b10000000100,
+            "ZSYNC_DATA_PQSC_REGISTER": 0b1000000000001
+            if descriptor.device_type == "SHFSG"
+            else 0b10000000001,
         }
         self.exposedFunctions = {
             "assignWaveIndex": self.assignWaveIndex,
             "playWave": self.playWave,
             "playZero": self.playZero,
+            "playHold": self.playHold,
             "executeTableEntry": self.executeTableEntry,
             "startQA": self.startQA,
             "startQAResult": self.startQAResult,
             "configFreqSweep": self.configFreqSweep,
             "setSweepStep": self.setSweepStep,
             "setOscFreq": self.setOscFreq,
             "setTrigger": self.setTrigger,
@@ -482,14 +488,15 @@
         # of the preceding time-span event (like playWave).
         ev = self.seqc_simulation.events
         if len(ev) == 0:
             return 0, 0
         if ev[-1].operation in [
             Operation.PLAY_WAVE,
             Operation.PLAY_ZERO,
+            Operation.PLAY_HOLD,  # ?
             Operation.WAIT_WAVE,
         ]:
             return ev[-1].start_samples, -1
         return ev[-1].start_samples + ev[-1].length_samples, len(ev)
 
     def program_finished(self):
         self.seqc_simulation.device_type = self.descriptor.device_type
@@ -635,20 +642,38 @@
                     start_samples=time_samples,
                     length_samples=length,
                     operation=Operation.PLAY_ZERO,
                     args=[],
                 )
             )
 
+    def playHold(self, length):
+        if length > 0:
+            time_samples = self._last_played_sample()
+            self.seqc_simulation.events.append(
+                SeqCEvent(
+                    start_samples=time_samples,
+                    length_samples=length,
+                    operation=Operation.PLAY_HOLD,
+                    args=[],
+                )
+            )
+
     def executeTableEntry(self, ct_index, latency=None):
         QA_DATA_PROCESSED_SG = 0b1000000000100
-        if ct_index == QA_DATA_PROCESSED_SG:
+        ZSYNC_DATA_PQSC_REGISTER_SG = 0b1000000000001
+        ZSYNC_DATA_PQSC_REGISTER_HD = 0b10000000001
+        if ct_index == QA_DATA_PROCESSED_SG or ct_index == ZSYNC_DATA_PQSC_REGISTER_SG:
             assert self.descriptor.device_type == "SHFSG"
             # todo(JL): Find a better index via the command table offset; take last for now
             ct_index = self.descriptor.command_table[-1]["index"]
+        elif ct_index == ZSYNC_DATA_PQSC_REGISTER_HD:
+            assert self.descriptor.device_type == "HDAWG"
+            # todo(JL): Find a better index via the command table offset; take last for now
+            ct_index = self.descriptor.command_table[-1]["index"]
 
         ct_entry = next(
             iter(i for i in self.descriptor.command_table if i["index"] == ct_index)
         )
         if "waveform" not in ct_entry:
             return  # todo: simulator does not yet support playZero via command table
 
@@ -669,19 +694,20 @@
         else:
             assert False, f"Unknown signal type: {wave['type']}"
 
         ct_info = CommandTableEntryInfo.from_ct_entry(ct_entry)
 
         if latency is not None:
             time_samples = self._last_played_sample()
-            if latency * 8 < time_samples:
+            corrected_latency = latency + EXECUTETABLEENTRY_LATENCY
+            if corrected_latency * 8 < time_samples:
                 raise RuntimeError(
                     f"ExecuteTableEntry scheduled with latency {latency} before current time {time_samples}"
                 )
-            elif latency * 8 > time_samples:
+            elif corrected_latency * 8 > time_samples:
                 raise RuntimeError(
                     f"Play queue starved at current time {time_samples} for ExecuteTableEntry scheduled with latency {latency}"
                 )
 
         if ct_entry["waveform"].get("precompClear", False):
             self.setPrecompClear(1)
             self._append_wave_event(wave_names, known_wave, ct_info)
@@ -889,19 +915,14 @@
 
 def analyze_recipe(
     recipe, sources, wave_indices, command_tables
 ) -> List[SeqCDescriptor]:
     outputs: Dict[str, List[int]] = {}
     seqc_descriptors_from_recipe: Dict[str, SeqCDescriptor] = {}
     for init in recipe["experiment"]["initializations"]:
-        delay = 0
-        if "measurements" in init and len(init["measurements"]) > 0:
-            if "delay" in init["measurements"][0]:
-                delay = init["measurements"][0]["delay"]
-
         device_uid = init["device_uid"]
         device = find_device(recipe, device_uid)
         device_type = device["driver"]
         sample_multiple = get_sample_multiple(device_type)
         try:
             sampling_rate = init["config"]["sampling_rate"]
         except KeyError:
@@ -914,38 +935,50 @@
                 dio_mode = init["config"]["dio_mode"]
                 if dio_mode == "hdawg_leader":
                     if sampling_rate == 2e9:
                         startup_delay = -24e-9
                     else:
                         startup_delay = -20e-9
 
+        # TODO(2K): input port_delay previously was not taken into account by the simulator
+        # - keeping it as is for not breaking the tests. To be cleaned up.
+        input_channel_delays: Dict[int, float] = {
+            i["channel"]: i["scheduler_port_delay"]  # + i.get("port_delay", 0.0)
+            for i in init.get("inputs", [])
+        }
+
         output_channel_delays: Dict[int, float] = {
-            o["channel"]: o.get("port_delay", 0.0) for o in init.get("outputs", [])
+            o["channel"]: o["scheduler_port_delay"] + o.get("port_delay", 0.0)
+            for o in init.get("outputs", [])
         }
 
         output_channel_precompensation = {
             o["channel"]: o.get("precompensation", {}) for o in init.get("outputs", [])
         }
 
         awg_index = 0
         if "awgs" in init:
             for awg in init["awgs"]:
                 seqc = awg["seqc"]
                 awg_nr = awg["awg"]
                 if device_type == "SHFSG" or device_type == "SHFQA":
+                    input_channel = awg_nr
                     output_channels = [awg_nr]
                 else:
+                    input_channel = 2 * awg_nr
                     output_channels = [2 * awg_nr, 2 * awg_nr + 1]
 
                 seqc_descriptors_from_recipe[seqc] = SeqCDescriptor(
                     name=seqc,
                     device_uid=device_uid,
                     device_type=device_type,
                     awg_index=awg_index,
-                    measurement_delay_samples=delay,
+                    measurement_delay_samples=round(
+                        input_channel_delays.get(input_channel, 0.0) * sampling_rate
+                    ),
                     startup_delay=startup_delay,
                     sample_multiple=sample_multiple,
                     sampling_rate=sampling_rate,
                     output_port_delay=output_channel_delays.get(
                         output_channels[0], 0.0
                     ),
                 )
```

## laboneq/simulator/wave_scroller.py

```diff
@@ -50,14 +50,15 @@
         self.last_trig = 0
         self.last_freq_set_samples = 0
         self.last_freq = np.nan
         self.oscillator_phase: Optional[float] = None
 
         self.processors = {
             Operation.PLAY_WAVE: self._process_play_wave,
+            Operation.PLAY_HOLD: self._process_play_hold,
             Operation.START_QA: self._process_start_qa,
             Operation.SET_TRIGGER: self._process_set_trigger,
             Operation.SET_OSC_FREQ: self._process_set_osc_freq,
         }
 
     def is_output(self) -> bool:
         return any(
@@ -85,14 +86,15 @@
             or SimTarget.TRIGGER in self.sim_targets
             or SimTarget.PLAY in self.sim_targets
             and self.is_shfqa
         ):
             target_events.add(Operation.START_QA)
         if SimTarget.PLAY in self.sim_targets and not self.is_shfqa:
             target_events.add(Operation.PLAY_WAVE)
+            target_events.add(Operation.PLAY_HOLD)
         if SimTarget.TRIGGER in self.sim_targets:
             target_events.add(Operation.SET_TRIGGER)
         if SimTarget.FREQUENCY in self.sim_targets:
             target_events.add(Operation.SET_OSC_FREQ)
         return target_events
 
     def _process_play_wave(self, event: SeqCEvent, snippet_start_samples: int):
@@ -118,14 +120,20 @@
             # Note: CT phase not implemented on RF signals
         ct_abs_amplitude = ct_info.abs_amplitude if ct_info is not None else None
         if ct_abs_amplitude is not None:
             wave = wave * ct_abs_amplitude
         wave_start_samples = event.start_samples - snippet_start_samples
         self.wave_snippet[wave_start_samples : wave_start_samples + len(wave)] = wave
 
+    def _process_play_hold(self, event: SeqCEvent, snippet_start_samples: int):
+        wave_start_samples = event.start_samples - snippet_start_samples
+        self.wave_snippet[
+            wave_start_samples : wave_start_samples + event.length_samples
+        ] = self.wave_snippet[wave_start_samples - 1]
+
     def _process_start_qa(self, event: SeqCEvent, snippet_start_samples: int):
         if SimTarget.PLAY in self.sim_targets and self.is_shfqa:
             self._process_shfqa_gen(event, snippet_start_samples)
         if (
             SimTarget.ACQUIRE in self.sim_targets
             or SimTarget.TRIGGER in self.sim_targets
         ):
```

## Comparing `laboneq/compiler/new_scheduler/case_schedule.py` & `laboneq/compiler/scheduler/case_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict, Iterator, List
 
 from attrs import asdict, define
 
 from laboneq.compiler import CompilerSettings
 from laboneq.compiler.common.event_type import EventType
 from laboneq.compiler.common.play_wave_type import PlayWaveType
-from laboneq.compiler.new_scheduler.section_schedule import SectionSchedule
+from laboneq.compiler.scheduler.section_schedule import SectionSchedule
 
 
 @define(kw_only=True, slots=True)
 class CaseSchedule(SectionSchedule):
     state: int
 
     def generate_event_list(
```

## Comparing `laboneq/compiler/new_scheduler/interval_schedule.py` & `laboneq/compiler/scheduler/interval_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from __future__ import annotations
 
 from typing import Dict, Iterator, List, Optional, Set
 
 from attrs import define, field
 
 from laboneq.compiler.common.compiler_settings import CompilerSettings
-from laboneq.compiler.new_scheduler.utils import lcm
+from laboneq.compiler.scheduler.utils import lcm
 
 # A deferred value is not really optional, but will initialized later; using this alias,
 # we can still use None as sentinel, but express that this property shall not be seen
 # as optional after (possibly external) initialization.
 Deferred = Optional
```

## Comparing `laboneq/compiler/new_scheduler/loop_iteration_schedule.py` & `laboneq/compiler/scheduler/loop_iteration_schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from typing import Dict, Iterator, List
 
 from attrs import asdict, define, evolve
 
 from laboneq.compiler.common.compiler_settings import CompilerSettings
 from laboneq.compiler.common.event_type import EventType
-from laboneq.compiler.new_scheduler.section_schedule import SectionSchedule
+from laboneq.compiler.scheduler.section_schedule import SectionSchedule
 
 
 @define(kw_only=True, slots=True)
 class LoopIterationSchedule(SectionSchedule):
     """Schedule of a single iteration of a loop (sweep or average)"""
 
     iteration: int
```

## Comparing `laboneq/compiler/new_scheduler/loop_schedule.py` & `laboneq/compiler/scheduler/loop_schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from typing import Dict, Iterator, List, Optional
 
 from attrs import asdict, define
 
 from laboneq.compiler.common.compiler_settings import CompilerSettings
 from laboneq.compiler.common.event_type import EventType
-from laboneq.compiler.new_scheduler.loop_iteration_schedule import LoopIterationSchedule
-from laboneq.compiler.new_scheduler.section_schedule import SectionSchedule
-from laboneq.compiler.new_scheduler.utils import ceil_to_grid, lcm
+from laboneq.compiler.scheduler.loop_iteration_schedule import LoopIterationSchedule
+from laboneq.compiler.scheduler.section_schedule import SectionSchedule
+from laboneq.compiler.scheduler.utils import ceil_to_grid, lcm
 from laboneq.core.exceptions.laboneq_exception import LabOneQException
 from laboneq.core.types.enums.repetition_mode import RepetitionMode
 
 
 @define(kw_only=True, slots=True)
 class LoopSchedule(SectionSchedule):
     compressed: bool
```

## Comparing `laboneq/compiler/new_scheduler/match_schedule.py` & `laboneq/compiler/scheduler/match_schedule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import math
+from dataclasses import dataclass
 from typing import TYPE_CHECKING, Dict, Iterable, Iterator, List
 
 from attrs import define
 from zhinst.utils.feedback_model import (
     FeedbackPath,
     PQSCMode,
     QAType,
     QCCSFeedbackModel,
     SGType,
     get_feedback_system_description,
 )
 
 from laboneq.compiler import CompilerSettings
+from laboneq.compiler.common.compiler_settings import EXECUTETABLEENTRY_LATENCY
 from laboneq.compiler.common.event_type import EventType
-from laboneq.compiler.new_scheduler.case_schedule import CaseSchedule
-from laboneq.compiler.new_scheduler.section_schedule import SectionSchedule
-from laboneq.compiler.new_scheduler.utils import ceil_to_grid
+from laboneq.compiler.scheduler.case_schedule import CaseSchedule
+from laboneq.compiler.scheduler.section_schedule import SectionSchedule
+from laboneq.compiler.scheduler.utils import ceil_to_grid
 from laboneq.core.exceptions.laboneq_exception import LabOneQException
 
 if TYPE_CHECKING:
-    from laboneq.compiler.new_scheduler.schedule_data import ScheduleData
+    from laboneq.compiler.scheduler.schedule_data import ScheduleData
+
+# Temporary corrected timing model
+@dataclass
+class QCCSFeedbackModelPlus(QCCSFeedbackModel):
+    additional_latency: int = 6
+
+    def get_latency(self, length: int) -> int:
+        return super().get_latency(length) + self.additional_latency
+
+
+FeedbackTimingModel = lambda *args, **kwargs: QCCSFeedbackModelPlus(
+    kwargs["description"]
+)
 
 # Copy from device_zi.py (without checks)
 def _get_total_rounded_delay_samples(
     port_delays, sample_frequency_hz, granularity_samples
 ):
     delay = sum(round((d or 0) * sample_frequency_hz) for d in port_delays)
     return (math.ceil(delay / granularity_samples + 0.5) - 1) * granularity_samples
@@ -120,30 +135,42 @@
         else:
             toolkit_sgtype = {
                 "hdawg": SGType.HDAWG,
                 "shfsg": SGType.SHFSG,
                 "shfqc": SGType.SHFQC,
             }[sg_device_type.str_value]
 
-        time_of_arrival_at_register = QCCSFeedbackModel(
+        model = FeedbackTimingModel if not local else QCCSFeedbackModel
+        time_of_arrival_at_register = model(
             description=get_feedback_system_description(
                 generator_type=toolkit_sgtype,
                 analyzer_type=toolkit_qatype,
                 pqsc_mode=None if local else PQSCMode.REGISTER_FORWARD,
                 feedback_path=FeedbackPath.INTERNAL if local else FeedbackPath.ZSYNC,
             )
         ).get_latency(acquire_end_in_samples)
 
+        # We also add three latency cycles here, which then, in the code generator, will
+        # be subtracted again for the latency argument of executeTableEntry. The reason
+        # is that there is an additional latency of three cycles from the execution
+        # of the command in the sequencer until the arrival of the chosen waveform in
+        # the wave player queue. For now, we look at the time the pulse is played
+        # (arrival time of data in register + 3), which also simplifies phase
+        # calculation for software modulated signals, and take care of subtracting it
+        # later
+
+        time_of_pulse_played = time_of_arrival_at_register + EXECUTETABLEENTRY_LATENCY
+
         sg_seq_rate = schedule_data.sampling_rate_tracker.sequencer_rate_for_device(
             sg_signal_obj.device_id
         )
         sg_seq_dt_for_latency_in_ts = round(
             1 / (2 * sg_seq_rate * schedule_data.TINYSAMPLE)
         )
-        latency_in_ts = time_of_arrival_at_register * sg_seq_dt_for_latency_in_ts
+        latency_in_ts = time_of_pulse_played * sg_seq_dt_for_latency_in_ts
 
         # Calculate the shift of compiler zero time for the SG; we may subtract this
         # from the time of arrival (which is measured since the trigger) to get the
         # start point in compiler time. The following elements need to be considered:
         # - The lead time of the acquisition AWG
         # - The setting of the delay_signal parameter for the acquisition AWG
         # - The time of arrival computed above
```

## Comparing `laboneq/compiler/new_scheduler/oscillator_schedule.py` & `laboneq/compiler/scheduler/oscillator_schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import Dict, Iterator, List
 
 from attrs import define
 
 from laboneq.compiler import CompilerSettings
 from laboneq.compiler.common.event_type import EventType
-from laboneq.compiler.new_scheduler.interval_schedule import IntervalSchedule
+from laboneq.compiler.scheduler.interval_schedule import IntervalSchedule
 
 
 @define
 class SweptHardwareOscillator:
     id: str
     signal: str
     device: str
```

## Comparing `laboneq/compiler/new_scheduler/phase_reset_schedule.py` & `laboneq/compiler/scheduler/phase_reset_schedule.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import Dict, Iterator, List, Tuple
 
 from attrs import define
 
 from laboneq.compiler import CompilerSettings
 from laboneq.compiler.common.event_type import EventType
-from laboneq.compiler.new_scheduler.interval_schedule import IntervalSchedule
+from laboneq.compiler.scheduler.interval_schedule import IntervalSchedule
 
 
 @define(kw_only=True, slots=True)
 class PhaseResetSchedule(IntervalSchedule):
     section: str
     hw_osc_devices: List[Tuple[str, float]]
     reset_sw_oscillators: bool
```

## Comparing `laboneq/compiler/new_scheduler/preorder_map.py` & `laboneq/compiler/scheduler/preorder_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import Dict
 
 import intervaltree
 
-from laboneq.compiler.new_scheduler.interval_schedule import IntervalSchedule
-from laboneq.compiler.new_scheduler.loop_schedule import LoopSchedule
-from laboneq.compiler.new_scheduler.section_schedule import SectionSchedule
+from laboneq.compiler.scheduler.interval_schedule import IntervalSchedule
+from laboneq.compiler.scheduler.loop_schedule import LoopSchedule
+from laboneq.compiler.scheduler.section_schedule import SectionSchedule
 
 
 def calculate_preorder_map(
     schedule: IntervalSchedule, preorder_map: Dict, current_depth=0
 ) -> int:
     max_depth = current_depth
     intervals = intervaltree.IntervalTree()
```

## Comparing `laboneq/compiler/new_scheduler/pulse_phase.py` & `laboneq/compiler/scheduler/pulse_phase.py`

 * *Files identical despite different names*

## Comparing `laboneq/compiler/new_scheduler/pulse_schedule.py` & `laboneq/compiler/scheduler/pulse_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from attrs import define
 
 from laboneq.compiler.common.compiler_settings import CompilerSettings
 from laboneq.compiler.common.event_type import EventType
 from laboneq.compiler.common.play_wave_type import PlayWaveType
 from laboneq.compiler.common.pulse_parameters import encode_pulse_parameters
 from laboneq.compiler.experiment_access.section_signal_pulse import SectionSignalPulse
-from laboneq.compiler.new_scheduler.interval_schedule import IntervalSchedule
+from laboneq.compiler.scheduler.interval_schedule import IntervalSchedule
 
 
 @define(kw_only=True, slots=True)
 class PulseSchedule(IntervalSchedule):
     pulse: SectionSignalPulse
     amplitude: float
     phase: float
```

## Comparing `laboneq/compiler/new_scheduler/reserve_schedule.py` & `laboneq/compiler/scheduler/reserve_schedule.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import Dict, List
 
-from laboneq.compiler.new_scheduler.interval_schedule import IntervalSchedule
+from laboneq.compiler.scheduler.interval_schedule import IntervalSchedule
 
 
 class ReserveSchedule(IntervalSchedule):
     @classmethod
     def create(cls, signal, grid):
         return cls(grid=grid, signals={signal})
```

## Comparing `laboneq/compiler/new_scheduler/root_schedule.py` & `laboneq/compiler/scheduler/root_schedule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2022 Zurich Instruments AG
 # SPDX-License-Identifier: Apache-2.0
 
 from typing import Dict, Iterator, List
 
 from laboneq.compiler import CompilerSettings
-from laboneq.compiler.new_scheduler.interval_schedule import IntervalSchedule
-from laboneq.compiler.new_scheduler.utils import ceil_to_grid
+from laboneq.compiler.scheduler.interval_schedule import IntervalSchedule
+from laboneq.compiler.scheduler.utils import ceil_to_grid
 
 
 class RootSchedule(IntervalSchedule):
     def generate_event_list(
         self,
         start: int,
         max_events: int,
```

## Comparing `laboneq/compiler/new_scheduler/schedule_data.py` & `laboneq/compiler/scheduler/schedule_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Dict, List
 
 if TYPE_CHECKING:
     from laboneq.compiler.common.compiler_settings import CompilerSettings
     from laboneq.compiler.common.signal_obj import SignalObj
     from laboneq.compiler.experiment_access.experiment_dao import ExperimentDAO
-    from laboneq.compiler.new_scheduler.pulse_schedule import PulseSchedule
+    from laboneq.compiler.scheduler.pulse_schedule import PulseSchedule
     from laboneq.compiler.scheduler.sampling_rate_tracker import SamplingRateTracker
 
 
 @dataclass
 class ScheduleData:
     experiment_dao: ExperimentDAO
     sampling_rate_tracker: SamplingRateTracker
```

## Comparing `laboneq/compiler/new_scheduler/section_schedule.py` & `laboneq/compiler/scheduler/section_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 from typing import TYPE_CHECKING, Dict, Iterator, List, Set, Tuple
 
 from attrs import define, field
 
 from laboneq.compiler.common.compiler_settings import CompilerSettings
 from laboneq.compiler.common.event_type import EventType
-from laboneq.compiler.new_scheduler.interval_schedule import IntervalSchedule
-from laboneq.compiler.new_scheduler.pulse_schedule import PrecompClearSchedule
-from laboneq.compiler.new_scheduler.utils import ceil_to_grid, floor_to_grid
+from laboneq.compiler.scheduler.interval_schedule import IntervalSchedule
+from laboneq.compiler.scheduler.pulse_schedule import PrecompClearSchedule
+from laboneq.compiler.scheduler.utils import ceil_to_grid, floor_to_grid
 from laboneq.core.exceptions.laboneq_exception import LabOneQException
 
 if TYPE_CHECKING:
-    from laboneq.compiler.new_scheduler.schedule_data import ScheduleData
+    from laboneq.compiler.scheduler.schedule_data import ScheduleData
 
 
 @define(kw_only=True, slots=True)
 class SectionSchedule(IntervalSchedule):
     right_aligned: bool
 
     #: The id of the section
```

## Comparing `laboneq/compiler/new_scheduler/utils.py` & `laboneq/compiler/scheduler/utils.py`

 * *Files identical despite different names*

## Comparing `laboneq-2.5.0.dist-info/LICENSE` & `laboneq-2.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `laboneq-2.5.0.dist-info/METADATA` & `laboneq-2.6.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: laboneq
-Version: 2.5.0
+Version: 2.6.0
 Summary: Zurich Instruments LabOne Q software framework for quantum computing control
 Author-email: Zurich Instruments Development Team <info@zhinst.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/zhinst/laboneq
 Keywords: quantum,sdk,zhinst
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

## Comparing `laboneq-2.5.0.dist-info/RECORD` & `laboneq-2.6.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,89 +1,85 @@
-laboneq/VERSION.txt,sha256=8OovyZ87edMyuqkbiNTk5GnLa58slmabO07I8Nb1uGM,5
+laboneq/VERSION.txt,sha256=4zzPZSfduHstyJSxfdhGIGxdGDNHENJT9_Nm8sRAP-A,5
 laboneq/__init__.py,sha256=xb0bbmhv6-zquNTknTRURgHIU1VG11TJVgz5svWkvzI,306
 laboneq/_token.py,sha256=D2wS1TbZ6-CzF73l5kd6Wilcm18IPyymygB6VakHyRc,2829
+laboneq/_utils.py,sha256=4TRw9Hv192vqcPwcPDBsqXcdAGhIOvH_D24mZdyfZok,928
 laboneq/_version.py,sha256=zaxeCShR641vx5bH27_dVdirv71bA2i9ciFcH4A2krE,238
-laboneq/simple.py,sha256=vSMPWUdUX4e9b8P8fifLMlXHtKCde280kf4kh3HMPhk,1411
+laboneq/simple.py,sha256=LfAlXPh-d8Z3n5LwwzhQCYlvAObkj1RIkqjR9V9MOcE,1525
 laboneq/_observability/__init__.py,sha256=rcsPn8d52W6G9ZGkI8TPrEtwSJ2WbQN_Urc2DiIaUDg,184
 laboneq/_observability/tracing/__init__.py,sha256=rEFK2BFplAYa8ZHwQpiaVKv9EaSDrUWKHBplg-AmzGE,538
 laboneq/_observability/tracing/_noop_tracer.py,sha256=z7yhOOaTwCbWTQVQJ3i0SPCYsvd2wdbngf7ygoPJVCE,893
 laboneq/_observability/tracing/_tracer.py,sha256=vqgWJiy17tpzSMIOFXgkXHg9oQotbM8Jd-cWjNyVvk0,2309
 laboneq/compiler/__init__.py,sha256=PQOZ0TyWFSH0U7NJZnaYtO62iQW7DGgEV5KQD0lyKVw,444
 laboneq/compiler/fastlogging.py,sha256=SCJykQ5V_qvRPvWkkDZOqFexmazzhW-fbP2jkglOUkA,204
 laboneq/compiler/qccs-schema_2_5_0.json,sha256=YauxP1Z39AGXi5lUB7eKRLsRxsllayxNlzeyHQBGOSY,22524
 laboneq/compiler/remote.py,sha256=Fyb1RaWU-JBudPSv3LN56yQhYndduOchiai2brTE1WA,666
 laboneq/compiler/code_generator/__init__.py,sha256=s8ihwbuWxGpCAMjnsBXQ0kdoXGqT-B8doSsk850gQA0,654
 laboneq/compiler/code_generator/analyze_events.py,sha256=xA7nDePKXzxQHeR4m95cOmN0CBTR6KY5T3mccT7bBM8,18645
-laboneq/compiler/code_generator/analyze_playback.py,sha256=x4GitPjYDZuSsDWxAeQgFD-2fCltVFiYWTPDnsCdaJw,28581
-laboneq/compiler/code_generator/code_generator.py,sha256=Y16IhjEpk4Xo6d1wTsoLXtz18XVBoCIG6Rmd3bt2isM,64112
+laboneq/compiler/code_generator/analyze_playback.py,sha256=dcRfLFAltlXyGbQIGtb_YAl-8sdkx4GLAYf37a837pE,26665
+laboneq/compiler/code_generator/code_generator.py,sha256=Gtok3LuvDbwTiXI_FL56tewR55ld7mFu31JfPi_VsaI,71375
 laboneq/compiler/code_generator/command_table_tracker.py,sha256=jXD4Ep8SMIgS_DNqgdfnGujma-oRhRZcvFcIa-AkAXc,4026
 laboneq/compiler/code_generator/compressor.py,sha256=sIbtla_ju0NM1FL1oWGV7SMyxpZoNKwMzHKvbyb3Ut8,2880
 laboneq/compiler/code_generator/feedback_register_allocator.py,sha256=iXuwHFa9g5YQriNqLHXoHIzkBanyR8XnD9C0mw6sPQU,1414
 laboneq/compiler/code_generator/interval_calculator.py,sha256=7dyk02iUdPHyzS4DU6JvkTKn36yWpUE2lhvUynY0aYQ,10355
-laboneq/compiler/code_generator/measurement_calculator.py,sha256=LkgLsVU-majR3ogXvGyuCItb7iNW6Q9QrssJS1gX-Rk,18617
-laboneq/compiler/code_generator/sampled_event_handler.py,sha256=c9JocBLk6H_kdQpeVbpGfdQW87FjkMfPh-odBvh1Wvg,29598
-laboneq/compiler/code_generator/seq_c_generator.py,sha256=-5EXgBoH89KbEIYp5hsZ1wkDSm1HkVZ2QOATaEC81B0,18188
-laboneq/compiler/code_generator/seqc_tracker.py,sha256=a2Jmd7ZZmG3eYleoaqDKEq1H4ntydacdpU59PBTbjVg,6129
+laboneq/compiler/code_generator/measurement_calculator.py,sha256=w15OoQt0yXR4k3V2nvJT2CoNGtrPDeCiPoQazk5TZFc,17825
+laboneq/compiler/code_generator/sampled_event_handler.py,sha256=yBaaIp7PH6vTVTkDAFqnt65iO_d9hSnI00_XJMl6JTU,30333
+laboneq/compiler/code_generator/seq_c_generator.py,sha256=oZ4-TzXQmrfYToNnRe-GPQa0A9ctlE4y2JsWj2yf918,19239
+laboneq/compiler/code_generator/seqc_tracker.py,sha256=bZPvLecbCXYH02TlTL7KkhOv6NXoMHOmS_kLZE9WzO8,6333
 laboneq/compiler/code_generator/signatures.py,sha256=2Ez4Tw_IbmQ2pwkpVMoWKsAuyy6h0mpRIWVUNVMb6-E,7741
 laboneq/compiler/code_generator/utils.py,sha256=KJtRJg6wE8FPALrG4B8H7GRZa_7WqOrXroWW8kgSdBA,3500
+laboneq/compiler/code_generator/wave_compressor.py,sha256=AUIDhuBIh-h6VahdjnWehAlEvQjVPvik4-punkWxjSo,3737
 laboneq/compiler/code_generator/wave_index_tracker.py,sha256=700LQq60nX9Btcn9bj2SDn674qRmsxy_Nz6yy0qx1Y0,1476
 laboneq/compiler/common/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/compiler/common/awg_info.py,sha256=djhjq5t8JruHRi9hKk4rtBVH4KfMWRkuamcypmhP6WA,1093
-laboneq/compiler/common/awg_sampled_event.py,sha256=IWSNsuACjHMJIvQpwSOY4-yMfQEyAyB9rY1myA1xcJc,1903
+laboneq/compiler/common/awg_sampled_event.py,sha256=Sz21qx__YTdkpeBAhpfyVgT4ED1zUR4OiIn6GTnNVvw,1926
 laboneq/compiler/common/awg_signal_type.py,sha256=aXiZ_K-yaG1pPPUMh5IpOXn2rQJngQnTzwqP1LExtT8,480
-laboneq/compiler/common/compiler_settings.py,sha256=KKBWEH8ZQ10AGaniDKZvpE9sv2eicYNlnYweORJ6EYs,3983
-laboneq/compiler/common/device_type.py,sha256=Mp6_bsBycpaT2gCeHjl6NRbcqy8ZKaqz_PK6a88cxEk,4708
+laboneq/compiler/common/compiler_settings.py,sha256=1Rr42CsHTmKtykUgOQuu0H56jCV4cGHAgoMb0nVuPFM,4015
+laboneq/compiler/common/device_type.py,sha256=QK48fFIH9-bcO25j6l4d-WrG1kpyapoTEZvHLzzsffI,6058
 laboneq/compiler/common/event_type.py,sha256=VJiiMUTbZHTetjnBPEPyoSVREczPAjTTxA7d7GbjN9M,1532
 laboneq/compiler/common/play_wave_type.py,sha256=9olrAuZqSSq-3fDpUCwbH2IC2F1mYaZ64H_NG0J6eXM,229
 laboneq/compiler/common/pulse_parameters.py,sha256=zhIljy4MHaBGSFYR-28ksDetM39C5p006e8flU21ZWE,580
 laboneq/compiler/common/signal_obj.py,sha256=UBrf78oTS_MyH3YaPZudNqDvFJzoY5_Fw-MJIUcOXVA,2594
 laboneq/compiler/common/trigger_mode.py,sha256=PfV_HskFUlk99bsngdjYz-b137e2qA6e1TNqA0Bjvbs,400
 laboneq/compiler/experiment_access/__init__.py,sha256=mb9ULouZiKIforKo2d458L6pvf0LmV4PXhmKhPBUj7g,154
 laboneq/compiler/experiment_access/acquire_info.py,sha256=bQrMObuyxABUpGTc0ubuUvOs15KzKJzos1dPw4B_PYs,222
-laboneq/compiler/experiment_access/cache.py,sha256=aCJLqqHMPPNk7k-ngo3GaeWQWMYq8THvSv-UL8gUVHs,602
 laboneq/compiler/experiment_access/device_info.py,sha256=HQBj1WpSt8TwHX5G_kE-1m5ulJ06-j_hdIIVamxHQDI,349
-laboneq/compiler/experiment_access/dsl_loader.py,sha256=0wH-Q6LPuX9wjWPlUb97ISl-8UZNMmj50Jot67jl5hw,44686
-laboneq/compiler/experiment_access/experiment_dao.py,sha256=NW5Kc-2TOPVCFWLffHCCF4iFvA1FSMm51ETYPpnZMyA,16529
+laboneq/compiler/experiment_access/dsl_loader.py,sha256=Hl6QwehHkBDHPCxhscpsMlFoWk7gvXvjIhsfyHmH6rI,44928
+laboneq/compiler/experiment_access/experiment_dao.py,sha256=ejzxEOBua2ztVe35tlZXe7SGcX2k-wVy0xKP-Tj2Bmc,16509
 laboneq/compiler/experiment_access/json_dumper.py,sha256=Yds37AhZV8nre6u_a50bVmkYrJCQF6WIqIs2MzB2m48,14106
 laboneq/compiler/experiment_access/json_loader.py,sha256=iyPOMYATaqjSxSCabHqsKGBbtEf5ttclYAH0Ajpfvqc,21004
 laboneq/compiler/experiment_access/loader_base.py,sha256=FEFxOs-_tS8ZMbLRAeaY7jDkFV6EmJvgxoKirI7kFo8,6182
 laboneq/compiler/experiment_access/marker.py,sha256=2Okj9Q_Ukk02B-Z7_WDM6nHN-nuXw3qFjUNaw8LUMsI,270
 laboneq/compiler/experiment_access/oscillator_info.py,sha256=VvEyOttSTDd7-oxpbim4xmPJUwYEzjrsDXup9xLwI0k,286
 laboneq/compiler/experiment_access/param_ref.py,sha256=wqyyzAiSIEu2GVeNdZc-MtvdhdSDp1Quch8qBVIPppw,197
-laboneq/compiler/experiment_access/pulse_def.py,sha256=HgUWmq0wyU1HWjBz2pADa8WhrQSnTsQN62zbkzbK_vA,1263
-laboneq/compiler/experiment_access/section_graph.py,sha256=0bIQle4g1adY8Ke7DjBG143Y4eWbTakO6YXdHzS3Tw8,21550
+laboneq/compiler/experiment_access/pulse_def.py,sha256=wC192cXc_oxtxj-xJS2tY2dHkDr_CAYrtIkcp45gj6E,1311
 laboneq/compiler/experiment_access/section_info.py,sha256=vRIw7KvrlNhXjh8ynUjGUer_DVJPxdo9FGBdDMWVuUY,851
 laboneq/compiler/experiment_access/section_signal_pulse.py,sha256=ZGgbvNW3v-qIgyvcW34Lk31hyhFeNb_UjE6uIUXd8os,1069
 laboneq/compiler/experiment_access/signal_info.py,sha256=HLkN-Kq2vZrh5tg92RA3ZSSYaiRXXQecw01-NtXGR_Q,387
-laboneq/compiler/new_scheduler/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
-laboneq/compiler/new_scheduler/case_schedule.py,sha256=hx2y33Cwjm484ZW3fYzheuQEjgg1dvJHMxfRzWIITR8,3269
-laboneq/compiler/new_scheduler/interval_schedule.py,sha256=x9ZbMhVZxoDjLHs5SbbgTpvf7YhDsIFJCr75ATr-_Io,7443
-laboneq/compiler/new_scheduler/loop_iteration_schedule.py,sha256=oWQaNGxixdxnkSDbdxfNMboMxTwD0GWf3V80kaeKcpg,3331
-laboneq/compiler/new_scheduler/loop_schedule.py,sha256=kUzQ3v-2Ca-w5f0nqxM1yIUjeYWKL5o6HPe7LNe9qyA,8588
-laboneq/compiler/new_scheduler/match_schedule.py,sha256=D0Qs7K8HwOKhnrlXPSmmXO5g_SQ5LnzdTDSuAkRy_mw,8075
-laboneq/compiler/new_scheduler/oscillator_schedule.py,sha256=80LLDWtu12iseHHvKoysfzDRCYnK8EkJjK2sgZFdcqA,2252
-laboneq/compiler/new_scheduler/phase_reset_schedule.py,sha256=lVXrMB-CFdC4_QLeFiqsp2C0iX2BIpRavuJj1tp-lsI,1765
-laboneq/compiler/new_scheduler/preorder_map.py,sha256=0e1zQEuUs6sc9PWRzl0cTHhvKAwx549njQtGQ8BFhLM,1820
-laboneq/compiler/new_scheduler/pulse_phase.py,sha256=poXl-PKFIO7X_xN3Qjqo-NWC-svaom3dWjetfKEsw8c,3821
-laboneq/compiler/new_scheduler/pulse_schedule.py,sha256=kw_8NWNRTNcSqGCdHxyhjwwTfAMlhsJ3KrtKcyzPRRY,6962
-laboneq/compiler/new_scheduler/reserve_schedule.py,sha256=ML-aqZlwj8_TpUV8lVdZuvdEtr3JahjYGIu6EvUXM38,625
-laboneq/compiler/new_scheduler/root_schedule.py,sha256=ni57ni5v4d5sBTYolt364x0mM_BIKA_dcifP2w8lnp8,1375
-laboneq/compiler/new_scheduler/schedule_data.py,sha256=qt6GHxcfsYPiCgM9doBV48XFTkcje-w1D7B8A2KyNXU,1016
-laboneq/compiler/new_scheduler/scheduler.py,sha256=ni0eNCApwJLGG9RuzBxgWGwmJEoFuHgRpwyT5BI7VYM,40991
-laboneq/compiler/new_scheduler/section_schedule.py,sha256=6x2PPJykhWnIBaclojjpkp54eY8XPN3rpXTxB1KkblE,13207
-laboneq/compiler/new_scheduler/utils.py,sha256=buFGd2oxNFr3hfGc8fx_dyMCbxTwimiSOuxCqeqSDRk,757
 laboneq/compiler/scheduler/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
-laboneq/compiler/scheduler/event_graph.py,sha256=N3jMW3wW_aX4123B3WxKMIcDr-CmZvZqshc-mTE0Vh0,12943
-laboneq/compiler/scheduler/event_graph_builder.py,sha256=aoT1FIXGZ601gGL-d4awtztWmEtdglOcZyXYEJC4EcE,24682
+laboneq/compiler/scheduler/case_schedule.py,sha256=HwzkOLBBYQip5bDBxNApQnGITb5cgyLVsYezwhxCdCQ,3265
+laboneq/compiler/scheduler/interval_schedule.py,sha256=tp4CauVPr-hOXxtzvUQYZrmXcqJBY7UqQDPlDDo1S_0,7439
+laboneq/compiler/scheduler/loop_iteration_schedule.py,sha256=5RKVr5tmtYqcGx8DY_kichm2rjeHtXbMrthFzwzFE9U,3327
+laboneq/compiler/scheduler/loop_schedule.py,sha256=RUFiK0sMisFwB1NVL1fAphcxKGMjB1f0ZpMPAf5-_fk,8576
+laboneq/compiler/scheduler/match_schedule.py,sha256=-laj65-4ozlLSc4AqTOXCaUA5hRhOZ06YMwAA4MRueM,9267
+laboneq/compiler/scheduler/oscillator_schedule.py,sha256=Iykf3E3wT7xXuH-hVk9_MwTHM7eWQFmhR3JzzQTd1eM,2248
+laboneq/compiler/scheduler/phase_reset_schedule.py,sha256=yLyoKe5S57LGcPMcgFxsBDyKjPROgCUdASTSPU-fQog,1761
+laboneq/compiler/scheduler/preorder_map.py,sha256=luqooLzAEbK2b0j8TIDcHsE3riHA_GFyhcSRerHUFUk,1808
+laboneq/compiler/scheduler/pulse_phase.py,sha256=poXl-PKFIO7X_xN3Qjqo-NWC-svaom3dWjetfKEsw8c,3821
+laboneq/compiler/scheduler/pulse_schedule.py,sha256=im2DdPgi2Q4pQq4Q-YnApyZyi04888iSOq03BRrzNds,6958
+laboneq/compiler/scheduler/reserve_schedule.py,sha256=WM-fLfdDnViVwB5U0TrrkiDKB0s3DSw3yUFLC5vyvQU,621
+laboneq/compiler/scheduler/root_schedule.py,sha256=2ErHbKUaD8f6xp42UdoCSaQ5AeZc5n4PNHaluspKRcE,1367
 laboneq/compiler/scheduler/sampling_rate_tracker.py,sha256=taR4AdTTaYNXfaEgM5hZNhL2VbcGnJCkx9gt4xAJg9E,1949
-laboneq/compiler/scheduler/scheduler.py,sha256=W0rMofmnGEeG9pbFQMcfPDd5BUZCQ4O3zBqzT_boZRI,115572
+laboneq/compiler/scheduler/schedule_data.py,sha256=FmMZQ2U_rsJyr3KQ2vYxAAexhS5crQp2kQBnHCpc2jg,1012
+laboneq/compiler/scheduler/scheduler.py,sha256=0Og-Ihgy1d5h17md12yBznP52MRIjPaIZXcug8hN5Ak,40949
+laboneq/compiler/scheduler/section_schedule.py,sha256=UruX04LNrMUUAUoJ3RooT3zSquPW5Atfa18ds6n8sWw,13191
+laboneq/compiler/scheduler/utils.py,sha256=buFGd2oxNFr3hfGc8fx_dyMCbxTwimiSOuxCqeqSDRk,757
 laboneq/compiler/workflow/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
-laboneq/compiler/workflow/compiler.py,sha256=grSiCLvvP6t_zzDhK7C8njwWfjHlw50a_CNy3X7YBm8,49793
+laboneq/compiler/workflow/compiler.py,sha256=JC-DzUfEzGCB-XD7_yMpk4uGJ5Ay-G7pwj-MctSpiJU,50498
 laboneq/compiler/workflow/precompensation_helpers.py,sha256=dpRw6dGJcsDAv0uI48cfzso75IYHNVfP1NUkRhD-giI,12424
-laboneq/compiler/workflow/recipe_generator.py,sha256=MEUGD0x8aGQaUZYDTcGeaIbfOykbvaz1bBa7xiV8GTI,12229
+laboneq/compiler/workflow/recipe_generator.py,sha256=ysiYXRS4JuKOnOsPldw1PClEasvG9oY-ieGet3M2qDQ,12420
 laboneq/contrib/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/bloch_simulator_pulse_plotter/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/bloch_simulator_pulse_plotter/inspector/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/bloch_simulator_pulse_plotter/inspector/update_inspect.py,sha256=dII-ZVAa3HumwKfHYGiARVBDCjaqJhGFy55XAjOPiaM,4511
 laboneq/contrib/bloch_simulator_pulse_plotter/plotter/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/bloch_simulator_pulse_plotter/plotter/plot_funs.py,sha256=3RjtFb3sxYokBP92COK53gCmBrCk9ubs8_xOb75fem4,3379
 laboneq/contrib/bloch_simulator_pulse_plotter/pulse_simulator/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
@@ -94,57 +90,57 @@
 laboneq/contrib/example_helpers/qubit_helper.py,sha256=Eh2UVnSrGlBy7nmxRcCWpQL2GG2fCrA1A6582UbYWqg,3581
 laboneq/contrib/example_helpers/randomized_benchmarking_helper.py,sha256=JKYF-5BXJJ3aBc4fEOOGnbheh9LPX4wir-xZCMrrzTs,8830
 laboneq/contrib/example_helpers/data_analysis/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/example_helpers/data_analysis/data_analysis.py,sha256=8eNR-b89_rs0odyNcWmH0DlTZ9zZHYI1wjIRCy8buSs,6670
 laboneq/contrib/example_helpers/descriptors/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
 laboneq/contrib/example_helpers/descriptors/hdawg.py,sha256=Q8Asxnt3x1Jl84nrTahjOgx-Ao_TWYdbIFf4WZdAkCU,502
 laboneq/contrib/example_helpers/descriptors/hdawg_uhfqa_pqsc.py,sha256=CzjRnXjw4v_WMtSvY5xZbmLztyEHfAQlzMbgvZ8cAmE,956
-laboneq/contrib/example_helpers/descriptors/shfqc.py,sha256=J3yEwcXPHlwylmhXmjztNwxr3idEkRrt7v9eTZPMp2k,1345
-laboneq/contrib/example_helpers/descriptors/shfsg.py,sha256=hFcFls-QkY7tQdvQ9y5K25UHsuWcV-nIxwOwyn_42JM,1377
-laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_hdawg_pqsc.py,sha256=mDvjBkffwNTOI0ZZggySTmVdjFejzZx3nGdwQctLTZY,1930
-laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_pqsc.py,sha256=N6W7sxG0HnjqS4xbfxqeUK60b4eYdrnN-57qk7Xkkiw,1618
-laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_shfqc_hdawg_pqsc.py,sha256=kZcUW_hQ_yUziYa7aPNi0iRZ5wWwTcYxqD8DDQYQnNg,2383
+laboneq/contrib/example_helpers/descriptors/shfqc.py,sha256=Vu_W7gf5XigJBTq3QZV8u-mAVXt560OFbuIiNCX_G10,1887
+laboneq/contrib/example_helpers/descriptors/shfsg.py,sha256=aWkqMMBq90JCPAj0-uZadDEMziln_OsqxZSFBJpsf-E,1639
+laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_hdawg_pqsc.py,sha256=ztHPSen0jfWqWzifanf-TmyXZ7P_R5-ssKXfOD_ASzo,2472
+laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_pqsc.py,sha256=cH9gx4th7Gh_oC72Fs0U3XQL1DUW3ownAv3BYsJ4PnA,2160
+laboneq/contrib/example_helpers/descriptors/shfsg_shfqa_shfqc_hdawg_pqsc.py,sha256=PIPiyvyyMv9wwcKBf81xFhF1Pflol2WrS5fkfb21EKU,2708
 laboneq/contrib/example_helpers/plotting/__init__.py,sha256=7Yt1BeCJ-am29jPA5s55Otv83hbYF3ZZum1MZabcNMk,77
-laboneq/contrib/example_helpers/plotting/plot_helpers.py,sha256=YH0AJlCXvV7ixAu9y61tXIiDWLcnZG2loQSAcigpePs,6620
+laboneq/contrib/example_helpers/plotting/plot_helpers.py,sha256=wACi_GadX6ldAALY6PK5isFE9FWsGDVAJYPa6B7BCJY,10340
 laboneq/controller/__init__.py,sha256=gPuU9BwcRA-VFMRLtIzd9Y-KvLQhYv0czaGuo-uimjc,308
 laboneq/controller/cache.py,sha256=sI4qtTQurYPWzMp7iW1oKwQp_GVftQX9isDkTNZ-bDE,1479
-laboneq/controller/communication.py,sha256=CxB46hJHKIVMtA55mSjGCOyjScFOpl5EFBwZYee5K1M,13536
-laboneq/controller/controller.py,sha256=rUZz3QllUDpKGbPBfivDJnlTyRkvKdeih6G5OucSRXw,32890
-laboneq/controller/laboneq_logging.py,sha256=esE9zHGFnANO-cBb2Im6s1UtyL2loZU-VMdpBUchPvk,4504
+laboneq/controller/communication.py,sha256=K-9sn7UABcGb9hGLM_8tLYtKWbNeSvUqcoubnBUTcvk,13604
+laboneq/controller/controller.py,sha256=oLZJaQQ1wHFfk8jMmoxIVRjEclqKgFvz_vLsYZRtN3k,34132
+laboneq/controller/laboneq_logging.py,sha256=XB51Z2RYeiozXPlRdeuWVFQGe8eXDbCOIp_nuOT3DTI,4600
 laboneq/controller/protected_session.py,sha256=v4T5NsQxE57E22hJltIumOnLAoBms0D7ZTtUYjGHGGM,337
-laboneq/controller/recipe_1_4_0.py,sha256=lD4WDlE9_iZJeHpI21Dy6u88LdF-AHCc61yaSrochnw,15011
+laboneq/controller/recipe_1_4_0.py,sha256=3UueBUAD5Eyij0T2Q4F0-_gvr-8OD7wgWmTAL7xjHV0,15088
 laboneq/controller/recipe_enums.py,sha256=uNjZPJci2KCleSh2zNYTOkUEfBpBK0spOU16GvaWj6Y,638
 laboneq/controller/recipe_processor.py,sha256=L2MBGJoaYFLLFqI53vuETuuzP6FHOfHMb6nJI7CatTA,19876
 laboneq/controller/results.py,sha256=b9Oy_F0GqSzHulNSWqt6ltUzXpYZ4JmC0BVIE176Qzc,1917
 laboneq/controller/toolkit_adapter.py,sha256=moZzwjnRUUbyT-7JL31EBtBh39VD3USx1SRolFS8v-g,1594
-laboneq/controller/util.py,sha256=UuAnPes0F2VXm_3nw0NCAVRNRhsOSUorkTN0gjHMcsw,624
+laboneq/controller/util.py,sha256=fi5_nCRrmORASGaFlge4TN6gXAWZIiS0pinr9-DVjnA,1178
 laboneq/controller/versioning.py,sha256=IcmXytxA6OtbudyM2aK8gCgWLcuLbweru5wIafolpnU,281
 laboneq/controller/devices/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/controller/devices/device_collection.py,sha256=OFIBllNQnuWNz31EelrkkOvGL6v4l47ZZsXM6V0uR1U,15400
 laboneq/controller/devices/device_factory.py,sha256=CQmdrldqyhI7wCFw2aObszp9g3XhPaJZv9Y8U_VAdMY,1275
-laboneq/controller/devices/device_hdawg.py,sha256=YgFUX9SjFp7Eer4_6sD4aCdeF6PZffRV8i5UyumTJPA,23542
+laboneq/controller/devices/device_hdawg.py,sha256=L6pV-wtfYWoxnyPzMa1jW_KszUIWiDqyU6rNIWMRn5M,23794
 laboneq/controller/devices/device_nonqc.py,sha256=m1rpD0XgwgNChmIkzdOBFiyg4bbPWY-1b0ysrMLqLNs,491
 laboneq/controller/devices/device_pqsc.py,sha256=FkH6ZaKqQDoX_WmROL1czc_dTU5DP0nU6IkqShA30fo,8115
 laboneq/controller/devices/device_setup_dao.py,sha256=daW-WJHaqCuxxNF3Wtnzr0_ebL2X9cYo-WHTv_U0Bas,4137
-laboneq/controller/devices/device_shfppc.py,sha256=ARsbwvxvTDFcvTdRZi463l-fvNDWVlsFZbM7qiU4Dzo,3758
-laboneq/controller/devices/device_shfqa.py,sha256=fq7WrGNIaYvStoojzqr0-YuSWpYEd1qT-hYihXpvN1c,40101
+laboneq/controller/devices/device_shfppc.py,sha256=NeGDmCxney0boI-7QHblA3VQCUpULFdkUIqt2l9oJqM,4013
+laboneq/controller/devices/device_shfqa.py,sha256=y0xFpvK_cszqje3uoNYzY7lLDxlJ4NnGVQwg6iT-hus,40727
 laboneq/controller/devices/device_shfsg.py,sha256=KTOAkTEslNQ4GanZI9Frh-bFcSwkQPckus-zejKk230,20509
-laboneq/controller/devices/device_uhfqa.py,sha256=SxKhhfaTQ2QUKYB2uJAGQ-3HRRO-XY83nxa4Rb85pVk,28521
-laboneq/controller/devices/device_zi.py,sha256=RNYRX1ljsLtyHYj4A04BlLK5eJ5djJM_7KffvtxA2ig,36707
+laboneq/controller/devices/device_uhfqa.py,sha256=vhoEyLZnOZVcyx5kSkYA3hYfeCSdpB7n35uctAVDdWc,28857
+laboneq/controller/devices/device_zi.py,sha256=ump_Phk0NOtJ8RpbDXAi32shSgiI04h7b7UnJp4x_NY,36238
 laboneq/controller/devices/zi_emulator.py,sha256=Y2uZuFe020_fmG8fG_dyFk6HlUpK36fxwG6hrBMr4Lk,29590
 laboneq/controller/devices/zi_node_monitor.py,sha256=2N2Q79sP-USY9-ovk5DHOXiO6Sov9QSzBGqdsyAPnuA,10358
 laboneq/core/__init__.py,sha256=nx0-aqsC4hdoO7jIj0Ut7yNTQbe5dme7jodU9wkd4N4,97
 laboneq/core/path.py,sha256=ZDMafOg44r5I3T-sW-iY6j7xrjYMbx12UsLoqbhg3Vw,2015
 laboneq/core/validators.py,sha256=pmtl8RdlBr-49CkxJseW1VrDtJU2gqLVBWSZdLrRpWc,1338
 laboneq/core/exceptions/__init__.py,sha256=8ZaME3lWkRJ7BZw1qVWGbt91jaklPd67iyIZ-zXoBpE,126
 laboneq/core/exceptions/laboneq_exception.py,sha256=bWRVbnLJiBszdNeEglRFp-z1Q3bb-irTIzf2vgTaBK0,123
 laboneq/core/serialization/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/core/serialization/simple_serialization.py,sha256=03qj5sZYadGGsqmd7qyCGmDizeRr8d91edo2Er6FT1Y,19090
 laboneq/core/types/__init__.py,sha256=fvF9SQu_JVfxc3et0G1RWE-FZvliRnYc_m6Ym6oavto,161
-laboneq/core/types/compiled_experiment.py,sha256=zeLm821a4hn5hbDzEAT-NnhPbQP-aP6OVP4vQoybz3E,5138
+laboneq/core/types/compiled_experiment.py,sha256=UNEhjGizBsy8pKOxCyKdeFLX4G3t-Y9oFjuaMR7vezI,5169
 laboneq/core/types/uid.py,sha256=bly72s6lGrQLYLJ3sk-vjJgzGhbLLYuQ87HMR9BOG9I,1473
 laboneq/core/types/enums/__init__.py,sha256=RfmSFJUHNxbqCeYHZWeg9Vl5wAA9u8k-_LDMTOTBbmM,660
 laboneq/core/types/enums/acquisition_type.py,sha256=PpK4El9Gvmt7ojw6tCcTSkfrDkJxmpvZyE2wbkPooLg,934
 laboneq/core/types/enums/averaging_mode.py,sha256=skosaedPnNxrW_UGRpksM1uiT7tCRLNx-9I3SuvdlMY,213
 laboneq/core/types/enums/carrier_type.py,sha256=PEbKKDkeBlQuUJCF-TFytQHjZf_enLJUDOvImdwVBH8,188
 laboneq/core/types/enums/dsl_version.py,sha256=Ba_d-Bw4wPQOb7Nv6Uy1S5XFCvDBXkNWzOoiPokiVxs,227
 laboneq/core/types/enums/execution_type.py,sha256=5AndgsShuhqkXr64g3IOuXal_TvhCrVMl7PkblOrZ1U,185
@@ -164,15 +160,15 @@
 laboneq/dsl/laboneq_facade.py,sha256=xfeHLO9ywCpClZ1Jl_I_Z_IC5wDpr2tckFsJhPuy8PY,2929
 laboneq/dsl/parameter.py,sha256=AbR78048B3-jyYvq_A5rmBqaeg4v0C601f9EGFJzRN0,2552
 laboneq/dsl/session.py,sha256=P-mOhpv3-u5stl3oeRSjTn97b4Nm4M42gxw24HYzsT4,25670
 laboneq/dsl/utils.py,sha256=v0qlt2XA2CXiGK3Rpi_PC45YZGeQriRz-ShovaTXMBE,2296
 laboneq/dsl/calibration/__init__.py,sha256=3becZcLdza9jTczHmfBgbbaH238UfP9uPakbhe5kwto,529
 laboneq/dsl/calibration/amplifier_pump.py,sha256=A4QI8YE-lRGaUv_yE6q7Osn3JfFSEuO-PzHyeowtaD0,1017
 laboneq/dsl/calibration/calibratable.py,sha256=DEx55rhplLTxoaf8-bGnmZqyO4eZdIyMptiLAGKEp7M,545
-laboneq/dsl/calibration/calibration.py,sha256=2js2bMMwX6pYrRFlWv3NRyeJOE5pwxDRqg3qVff6X5c,1886
+laboneq/dsl/calibration/calibration.py,sha256=3t6v9XjyhsT8ZtZM5kIRIgfUy99OWk85JvcMFtDc-Ok,2313
 laboneq/dsl/calibration/calibration_item.py,sha256=JlPu54zS2NfivokgD4ICOhrw5e3Rhs5DO7pB0iDazpY,111
 laboneq/dsl/calibration/mixer_calibration.py,sha256=_ivXcsDgELxaC8zZ7E5caMhE-HZYSuuDyR5odaVImKw,992
 laboneq/dsl/calibration/observable.py,sha256=5zf7HE7e4MnrnHcgwAWMKkejOiVTZs4UCtlRiVn8OVw,3403
 laboneq/dsl/calibration/oscillator.py,sha256=H2_32nckXQLraVZzq15Y-NLMB9U3BJp3lQW1QI3QxLs,1716
 laboneq/dsl/calibration/precompensation.py,sha256=N-GduIP4AVdKfxDH2rQ3zbYEarKx1rYrxO2Egb70Q9A,2650
 laboneq/dsl/calibration/signal_calibration.py,sha256=_SpbINwf-0i8vr_-r0smIL5v0cmN1cyLNZAw5n3E0GA,5607
 laboneq/dsl/calibration/units.py,sha256=9W7YXV75G2VgNGSNserL_rsnEdjQugCuzg1gQmkvutU,553
@@ -181,15 +177,16 @@
 laboneq/dsl/device/connection.py,sha256=e_uMDO-7YrMKJkZEbizlTQZITsXU1--ceOYOZ0m40Xc,601
 laboneq/dsl/device/device_setup.py,sha256=hDYGDooO-rFxHsC7i1HD5kyzPvXzNSjrXBWkCTg0dMk,13663
 laboneq/dsl/device/device_setup_helper.py,sha256=KRaya8xtzjqzdn1SZ_NMCU7p_V-76Aj_S0evSzuey7c,2551
 laboneq/dsl/device/instrument.py,sha256=XjaPAcpKdPQx1z-QpAFwHLFERoK65-Rgb7SjIyW_zy8,1362
 laboneq/dsl/device/logical_signal_group.py,sha256=i12USV4K1ij8y_3SOYStnZE_z3Bo6G0-f03RtuBjO-w,1893
 laboneq/dsl/device/physical_channel_group.py,sha256=1u4c9TyfC5WZWkgQGTpDcbIc6hXcgKuNdE8AJcxbaRk,1729
 laboneq/dsl/device/ports.py,sha256=-jVPCUfRq1e2PHpPBrcHuUQcrrfv7kylzDUF9rZWTnQ,538
-laboneq/dsl/device/qubits.py,sha256=OZ7LO7MaX_9-Qm2um-jC1EQwmBh3mqBQM4vxhCiBGlc,4453
+laboneq/dsl/device/qubits.py,sha256=zjEg3HIPvRU8giDSqI9i1vOISPtQSEPEKLez-CyoauA,4557
+laboneq/dsl/device/quops.py,sha256=V7XsyXTUqHH5s5Q2QeqF2GKko2roQxSm89cdZ4k2FCc,3104
 laboneq/dsl/device/server.py,sha256=JOM2xKKWMwFWYPcAjoCoFIuF_4ZC73_fMiZXUhNSZPk,215
 laboneq/dsl/device/instruments/__init__.py,sha256=sl302P7-HQO6Y8NXCcN2-r5mfbGastN7Ugs6PfRA1wg,328
 laboneq/dsl/device/instruments/hdawg.py,sha256=xLmo7LJhGC61PDkv_ZYn37VD0bnRxC1Ag54ET_KRLE4,1778
 laboneq/dsl/device/instruments/nonqc.py,sha256=j6jLNrFifaKe1QDcQJcTVWMdQR7eBI345V7S-iWqhts,466
 laboneq/dsl/device/instruments/pqsc.py,sha256=JQrg31Gj6HRjUOYjDyG5m2A9ngrQOFcX0mHw_2BwsGk,948
 laboneq/dsl/device/instruments/shfppc.py,sha256=E_-2fesNBJ0E-qrrwSA5MK1TdL0Daht9OX2U0BeBtkg,927
 laboneq/dsl/device/instruments/shfqa.py,sha256=C6yaZvxr1xZwUegOILTNC8_B7a28O_GqsIYag-dCvYo,2248
@@ -206,43 +203,44 @@
 laboneq/dsl/experiment/acquire.py,sha256=g4Pvm6T0qu8tH8LRTHhCZ1wb2K4Drc1rawNeNTRkS_E,972
 laboneq/dsl/experiment/call.py,sha256=eATarAz81C0QC5Ih-Uuh9PrS0g4rEF_vbQsrav_-I6Q,814
 laboneq/dsl/experiment/delay.py,sha256=98P3AePai3fqH1csDnWSxUN3EGJchuysX_2qnkCF2-Y,780
 laboneq/dsl/experiment/experiment.py,sha256=pr5g9l1DEHEWSrqVCwqiIoENt-hbwQXcChywV9e4ppg,39779
 laboneq/dsl/experiment/experiment_signal.py,sha256=eHDHAu7Hv9xTSF-f9-YsJ1suZmZfaevS9anyLaBiOPY,8216
 laboneq/dsl/experiment/operation.py,sha256=kJPLIjNTFf_lJkVsOmASPi7GZVJ9CCZySdA2YDCmswU,401
 laboneq/dsl/experiment/play_pulse.py,sha256=yGd_-jzkuOK_i4A65mfoPfeG1IRKK8ZaDQE-E627Idw,1647
-laboneq/dsl/experiment/pulse.py,sha256=WH8cUpm40dv-xUTi-B4s542QU3c3BF4Dpwm-QtYTwOw,3568
-laboneq/dsl/experiment/pulse_library.py,sha256=cvLbQXr4lUPeXDY-09iNuWyqhdAvtTAROTcJbiPZD8I,7932
+laboneq/dsl/experiment/pulse.py,sha256=cdmMmMo1yGygx_5EkyemW6xO-8-FuIErugjN1PHiKrE,3953
+laboneq/dsl/experiment/pulse_library.py,sha256=kmvFKXNGXIVCnjFMsFqAdiUM5bk8u-grY4ZeuKWHJ8M,8194
 laboneq/dsl/experiment/reserve.py,sha256=tn1YEkW6E7BbBuG4SKveCmiAXrsYm2IeMUI2iDnwazs,890
 laboneq/dsl/experiment/section.py,sha256=0gg3PscVUPEoTEhYaE4bsX8qsTvxgXQ4RyKb_gop5q8,11431
 laboneq/dsl/experiment/set.py,sha256=4hEgxT9iYWNgDEEAFDS4D1GlgTsInRK3regArR4cnaU,640
 laboneq/dsl/experiment/utils.py,sha256=TiO1tKG5F8Zqx1lUz1rUPc3lNVE6UMPnniuLNoyMql8,323
 laboneq/dsl/result/__init__.py,sha256=XAUfjo82SDzPK0s8ZZSJPTVRIF8b4smFBWhI5rwqBAQ,151
 laboneq/dsl/result/acquired_result.py,sha256=yNCpd1C8BnKeWbMCJHSVFOQzcYoy00-eLdLwjAEcFQk,1766
 laboneq/dsl/result/results.py,sha256=79EozB9G1ExCYAY8dFjEQdpDL82G5tJGKTdMH1XWRn8,7240
 laboneq/dsl/serialization/__init__.py,sha256=XVKLzoqNC9_psuftSgRNbbNmrcvTeJmWW5bIa-bmwRU,113
-laboneq/dsl/serialization/serializer.py,sha256=f-eflHyxkv4dvli2WctR-dAP-ykUR-1PcEiyLtyeF9E,5339
+laboneq/dsl/serialization/serializer.py,sha256=vInxTlXMw-K_RavNnJckdmbpJxppEnVJ2cwgJCKFuzc,5379
 laboneq/executor/__init__.py,sha256=FVNdflrImH-vSDDkoz05G5rNUUDB7mf4sgoOZHttkBQ,77
 laboneq/executor/execution_from_experiment.py,sha256=eE1lzSHYQqZZqlM2TAyjm0ibP3ifeeNTIOazin9z96M,3819
 laboneq/executor/executor.py,sha256=xvJwDB-9hlPjD4dTPqfxN2uNVB_2o8ZoKLNWPQBgpQc,8152
 laboneq/openqasm3/__init__.py,sha256=zIfFQa39Ko4nUcnnLBmRilnUVJ9eeg022QoLpodiv2o,145
-laboneq/openqasm3/expression.py,sha256=2X5JNUQKnVL0aST5QcrTuwvn3UTRRp36Do1dSxBP6UI,2488
-laboneq/openqasm3/gate_store.py,sha256=9OSAaIZhUUYCCl-I8vq5aSoTWpIZwYy_eOOUkbMX6oY,1929
-laboneq/openqasm3/openqasm3_importer.py,sha256=Z3Vp_SeHG0RLVeaogO7CQkWJw884VHztxzwRamk-XIQ,10789
+laboneq/openqasm3/expression.py,sha256=j22P0GOjizCvOZ-G87xX4qIYxnZiJxRUF9_UytCnuS0,8730
+laboneq/openqasm3/gate_store.py,sha256=33P_tN8UVV9VpHzcpP2HVbYFuWXlYs_BEe9VyWUEsxg,1604
+laboneq/openqasm3/namespace.py,sha256=xpMmnQZ-ap-y7wECmdPAd3u9waHV6eYaGFYmwwENJtY,2060
+laboneq/openqasm3/openqasm3_importer.py,sha256=AmITRhrw1PpVYLAImbTWCY_ruA2PkrA7TOlm9oaGsnI,13702
 laboneq/openqasm3/openqasm_error.py,sha256=rgkp6fT1tNrhVX8eCV-q1PLJUfGxkmT4gXEErJcSB-8,1732
-laboneq/openqasm3/reset_gate_factory.py,sha256=zmIZK4huifimAN-SSj4ww6UJ_2Ix1-7n-K99JaWWQZU,5136
-laboneq/openqasm3/variable_store.py,sha256=lj4duVPjDjalsdwzt3cm6HKGcyiM8UJx36CwGA3ClTY,3069
+laboneq/openqasm3/reset_gate_factory.py,sha256=WnWPrS0E0NXXy1pbSryMw8KgswOoGm7IW71vhynXhKA,4850
+laboneq/openqasm3/signal_store.py,sha256=mR5qYGiTtOGNGfTevQyLCW5Pwy2rgHiL1oLen1zXgLo,1492
 laboneq/pulse_sheet_viewer/__init__.py,sha256=F_gdqvR3iTbFH2-iGtGWPp2v2XpMu0c4SXEPEIJyQb0,127
 laboneq/pulse_sheet_viewer/event_graph_viewer.py,sha256=hKBUzFzimfz9YAFUYNYwrhwMscXHa-4M3BNa6id6SHE,2059
 laboneq/pulse_sheet_viewer/interactive_psv.py,sha256=D7pEX9C8mP9EZofE5L3aAAkX3lNFaEoHwBc_l2AHyec,2692
 laboneq/pulse_sheet_viewer/pulse_sheet_viewer.py,sha256=_O53T2cm8KWDhbUKoONuRb_9JOKyKvOqEMtQgrwlQPI,3288
 laboneq/pulse_sheet_viewer/pulse_sheet_viewer_template.html,sha256=TsX3r0W8qf_PKAw1pYreXQEcexRfzgL_FmbvOAFh06s,1443040
 laboneq/simulator/__init__.py,sha256=BuPOsR4Dwi6tSLAsG0lBeHzpOZFnCsNn93ohr-v9mZ8,152
 laboneq/simulator/output_simulator.py,sha256=OjbHVNNkrYITwZaJ58HaqAeM-ETeLP4y_ifA0aQXrGE,5904
-laboneq/simulator/seqc_parser.py,sha256=Ru8TnmLX49vX9jhY_o8hbZ6iy3FgL5EuB1XHgmAjFgg,39230
-laboneq/simulator/wave_scroller.py,sha256=j3lQLcCuqv8b2UTbViAtXIDvEa2mXADApPmhj570fdU,12081
-laboneq-2.5.0.dist-info/AUTHORS,sha256=Uu7pMg_oQJSHTrzjG8G3ApfutLIKqdOdjmtf5VZQILs,22
-laboneq-2.5.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-laboneq-2.5.0.dist-info/METADATA,sha256=nUWf4JIKgsC1hS2kCVv8aIAHvCjOGu1g6dgPLLM7yAo,3188
-laboneq-2.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-laboneq-2.5.0.dist-info/top_level.txt,sha256=oZ0o6Elw6GJcR44azoSi8l6opKF-v5Ks1MLYbqpXJGA,8
-laboneq-2.5.0.dist-info/RECORD,,
+laboneq/simulator/seqc_parser.py,sha256=gVR7AEtmuJH2QDGnzA4LRkZPgr3iBorwWMk-CJ3cPGQ,40863
+laboneq/simulator/wave_scroller.py,sha256=P9YjG9w_td2SrZfQohIVcRe4Gf9MBI_-RgA615de99g,12500
+laboneq-2.6.0.dist-info/AUTHORS,sha256=Uu7pMg_oQJSHTrzjG8G3ApfutLIKqdOdjmtf5VZQILs,22
+laboneq-2.6.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+laboneq-2.6.0.dist-info/METADATA,sha256=zyGQqVdAX3KFnJtDUEU2QogqYqCPWvOHfGZUJt5hOk8,3188
+laboneq-2.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+laboneq-2.6.0.dist-info/top_level.txt,sha256=oZ0o6Elw6GJcR44azoSi8l6opKF-v5Ks1MLYbqpXJGA,8
+laboneq-2.6.0.dist-info/RECORD,,
```

