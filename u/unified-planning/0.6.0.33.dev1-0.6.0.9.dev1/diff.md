# Comparing `tmp/unified_planning-0.6.0.33.dev1.tar.gz` & `tmp/unified_planning-0.6.0.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified_planning-0.6.0.33.dev1.tar", last modified: Mon May 15 09:59:16 2023, max compression
+gzip compressed data, was "unified_planning-0.6.0.9.dev1.tar", last modified: Thu May  4 15:32:36 2023, max compression
```

## Comparing `unified_planning-0.6.0.33.dev1.tar` & `unified_planning-0.6.0.9.dev1.tar`

### file list

```diff
@@ -1,358 +1,360 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:59:16.557261 unified_planning-0.6.0.33.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.505260 unified_planning-0.6.0.33.dev1/unified_planning/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.509260 unified_planning-0.6.0.33.dev1/unified_planning/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.509260 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14506 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    18556 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    16331 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    29153 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/credits.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    46187 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/meta_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.509260 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/anytime_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/oneshot_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/plan_repairer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/oversubscription_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/engines/sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.513260 unified_planning-0.6.0.33.dev1/unified_planning/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/grpc/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.513260 unified_planning-0.6.0.33.dev1/unified_planning/grpc/generated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/grpc/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35525 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/grpc/proto_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    33351 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/grpc/proto_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.513260 unified_planning-0.6.0.33.dev1/unified_planning/interop/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/interop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/interop/from_tarski.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/interop/to_tarski.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.513260 unified_planning-0.6.0.33.dev1/unified_planning/io/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/io/anml_grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)    41213 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/io/anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/io/anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    37842 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/io/ma_pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    74227 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/io/pddl_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    37139 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/io/pddl_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.517260 unified_planning-0.6.0.33.dev1/unified_planning/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/abstract_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    28405 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/contingent_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/delta_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/fluent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/fnode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.517260 unified_planning-0.6.0.33.dev1/unified_planning/model/htn/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/htn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/htn/hierarchical_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/htn/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/htn/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/htn/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/htn/task_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.521260 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/actions_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/agents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/fluents_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/initial_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/objects_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/time_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/timed_conds_effs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/user_types_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.521260 unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/ma_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/ma_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    10393 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/problem_kind.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.521260 unified_planning-0.6.0.33.dev1/unified_planning/model/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/scheduling/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/scheduling/chronicle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/scheduling/scheduling_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.525260 unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/type_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.525260 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/any.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/fluents_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/free_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/identitydag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/linear_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/names_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/operators_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/quantifier_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/state_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/type_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.529260 unified_planning-0.6.0.33.dev1/unified_planning/plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/plans/contingent_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/plans/hierarchical_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/plans/partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/plans/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/plans/sequential_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/plans/stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/plans/time_triggered_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    29644 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.537260 unified_planning-0.6.0.33.dev1/unified_planning/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/basic.anml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/basic_conditional.anml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/connected_locations.anml
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/constants.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/durative_goals.anml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/forall.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/hydrone.anml
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/match.anml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/match_int_id.anml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/match_test_parser.anml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/simple_mais.anml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/anml/tils.anml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.497260 unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/colorballs/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/logistic_conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/examples/hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/examples/minimals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/examples/multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    39048 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/examples/realistic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/examples/tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30699 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/examples/testing_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.501260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-PCP/
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Rover/
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.541261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Satellite/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Childsnack/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Depots/
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Hiking/
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.545261 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
--rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Robot/
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
--rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Snake/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Towers/
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Transport/
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Woodworking/
--rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.549260 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/citycar/
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/citycar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/citycar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/counters/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/counters/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/counters/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/counters/problem2.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/depot/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/depot/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/depot/problem.pddl
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/enhsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/htn-transport/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/matchcellar/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/miconic/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/miconic/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/miconic/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/robot_fastener/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/safe_road/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/safe_road/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/safe_road/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/sailing/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/sailing/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/sailing/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/visit_precedence/
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.553261 unified_planning-0.6.0.33.dev1/unified_planning/test/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/scheduling/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/scheduling/jobshop.py
--rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_anml_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_anml_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_anytime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_bounded_types_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_compilers_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_compilers_quality_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_conditional_effects_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_contingent_pddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_credits.py
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_dnf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_expression_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_htn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_infix_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_negative_conditions_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_partial_order_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    32900 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_pddl_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_pddl_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_plan_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_planner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_protobuf_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_pyperplan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_quantifier_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_replanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_sequential_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_simplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_simulated_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_stn_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_substituter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_tamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_tarski_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_tarski_grounder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_temporal.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_trajectory_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_trajectory_constraints_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_usertype_fluents_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/test/test_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-15 09:59:13.000000 unified_planning-0.6.0.33.dev1/unified_planning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:59:16.505260 unified_planning-0.6.0.33.dev1/unified_planning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-15 09:59:16.000000 unified_planning-0.6.0.33.dev1/unified_planning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13959 2023-05-15 09:59:16.000000 unified_planning-0.6.0.33.dev1/unified_planning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:59:16.000000 unified_planning-0.6.0.33.dev1/unified_planning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-15 09:59:16.000000 unified_planning-0.6.0.33.dev1/unified_planning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 09:59:16.000000 unified_planning-0.6.0.33.dev1/unified_planning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.579271 unified_planning-0.6.0.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 15:32:36.579271 unified_planning-0.6.0.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:32:36.579271 unified_planning-0.6.0.9.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.543269 unified_planning-0.6.0.9.dev1/unified_planning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.547269 unified_planning-0.6.0.9.dev1/unified_planning/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.547269 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14454 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17677 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18492 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29101 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41064 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/meta_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.547269 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/anytime_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/oneshot_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/plan_repairer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/oversubscription_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8025 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19370 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27821 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/engines/sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.551269 unified_planning-0.6.0.9.dev1/unified_planning/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.551269 unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35468 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32998 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/proto_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33343 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/grpc/proto_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.551269 unified_planning-0.6.0.9.dev1/unified_planning/interop/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/interop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/interop/from_tarski.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/interop/to_tarski.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.551269 unified_planning-0.6.0.9.dev1/unified_planning/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/anml_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41213 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37842 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/ma_pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74227 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/pddl_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37139 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/pddl_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26929 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/python_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/abstract_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28405 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/contingent_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/delta_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15093 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/fluent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/fnode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/hierarchical_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8838 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/htn/task_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/actions_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/agents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/fluents_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/initial_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/objects_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/time_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14921 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/timed_conds_effs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/user_types_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/ma_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/ma_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38729 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/problem_kind.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/chronicle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/scheduling_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.555270 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8415 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/type_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.559270 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/fluents_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/free_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/identitydag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/linear_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/names_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/operators_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/quantifier_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/state_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24747 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/usertype_fluents_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.559270 unified_planning-0.6.0.9.dev1/unified_planning/plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/contingent_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/hierarchical_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/sequential_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/plans/time_triggered_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27425 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.563270 unified_planning-0.6.0.9.dev1/unified_planning/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/basic.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/basic_conditional.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/connected_locations.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/constants.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/constants_no_variable_duration.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/durative_goals.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/forall.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/hydrone.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match_int_id.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match_test_parser.anml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/simple_mais.anml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/anml/tils.anml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.539269 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14614 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/minimals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38724 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/realistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14293 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30699 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/examples/testing_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.543269 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    34291 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33635 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.567270 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)   189505 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    33123 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    13014 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.571271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/
+-rw-r--r--   0 runner    (1001) docker     (123)    34612 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/problem2.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/problem.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/enhsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/domain.hddl
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/problem.hddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/matchcellar/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/matchcellar/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/matchcellar/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/miconic/
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/miconic/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/miconic/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/robot_fastener/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/robot_fastener/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/safe_road/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/safe_road/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/safe_road/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/sailing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/sailing/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/sailing/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/visit_precedence/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/visit_precedence/problem.pddl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.575271 unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/jobshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_anml_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_anml_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_anytime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10336 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_bounded_types_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_compilers_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_compilers_quality_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_conditional_effects_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_contingent_pddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_credits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_disjunctive_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_dnf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_expression_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_htn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_infix_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_negative_conditions_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_partial_order_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32858 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_pddl_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_pddl_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_plan_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14049 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24949 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17866 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_protobuf_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_pyperplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_python_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_quantifier_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_replanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9570 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_sequential_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_simulated_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_stn_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_substituter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_tamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_tarski_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_tarski_grounder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_temporal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_trajectory_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_trajectory_constraints_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_usertype_fluents_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/test/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-04 15:32:31.000000 unified_planning-0.6.0.9.dev1/unified_planning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:36.543269 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 15:32:36.000000 unified_planning-0.6.0.9.dev1/unified_planning.egg-info/top_level.txt
```

### Comparing `unified_planning-0.6.0.33.dev1/LICENSE` & `unified_planning-0.6.0.9.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/PKG-INFO` & `unified_planning-0.6.0.9.dev1/unified_planning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unified_planning
-Version: 0.6.0.33.dev1
+Name: unified-planning
+Version: 0.6.0.9.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: UNKNOWN
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-0.6.0.33.dev1/README.md` & `unified_planning-0.6.0.9.dev1/README.md`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/setup.py` & `unified_planning-0.6.0.9.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/bounded_types_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/bounded_types_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/compilers_pipeline.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/conditional_effects_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/conditional_effects_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,14 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/disjunctive_conditions_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/grounder.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/grounder.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,17 +146,17 @@
         """
         Returns an iterator over all the possible grounded actions of the problem given at construction time.
         Every resulting tuple is made of 3 elements: ``original_action``, ``parameters``, ``grounded_action`` where:
 
         * The ``original_action`` is the `Action` of the ``Problem`` that is grounded.
         * The ``parameters`` is the `Tuple of expressions` used to ground the ``original_action``.
         * The ``grounded_action`` is the `Action` created by grounding the ``original_action`` with the given ``parameters``;
-            the ``grounded_action`` can be ``None`` if the grounding of the ``original_action`` with the given parameters
-            creates an invalid or meaningless `Action` (invalid if it has conflicting `Effects`,
-            meaningless if it has no `effects` or contradicting `conditions`).
+        the ``grounded_action`` can be ``None`` if the grounding of the ``original_action`` with the given parameters
+        creates an invalid or meaningless `Action` (invalid if it has conflicting `Effects`,
+        meaningless if it has no `effects` or contradicting `conditions`).
         """
         for old_action in self._problem.actions:
             for grounded_params in self.get_possible_parameters(old_action):
                 assert isinstance(grounded_params, tuple)
                 new_action = self.ground_action(old_action, grounded_params)
                 yield (old_action, grounded_params, new_action)
 
@@ -265,15 +265,14 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
         supported_kind.set_expression_duration("FLUENTS_IN_DURATIONS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_constraints_kind("TRAJECTORY_CONSTRAINTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/negative_conditions_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/negative_conditions_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("MAKESPAN")
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/quantifiers_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/quantifiers_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/tarski_grounder.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/usertype_fluents_remover.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_quality_metrics("ACTIONS_COST")
         supported_kind.set_actions_cost_kind("STATIC_FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_actions_cost_kind("FLUENTS_IN_ACTIONS_COST")
         supported_kind.set_quality_metrics("FINAL_VALUE")
         supported_kind.set_quality_metrics("MAKESPAN")
         supported_kind.set_quality_metrics("PLAN_LENGTH")
         supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/compilers/utils.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/compilers/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/credits.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/engine.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/factory.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from unified_planning.engines.mixins.portfolio import PortfolioSelectorMixin
 from unified_planning.engines.mixins.replanner import ReplannerMixin
 from unified_planning.engines.mixins.plan_repairer import PlanRepairerMixin
 from unified_planning.engines.mixins.sequential_simulator import (
     SequentialSimulatorMixin,
 )
 from unified_planning.engines.engine import OperationMode
-from typing import IO, Any, Dict, Tuple, Optional, List, Union, Type, Sequence, cast
+from typing import IO, Any, Dict, Tuple, Optional, List, Union, Type, Sequence
 from pathlib import PurePath
 
 
 DEFAULT_ENGINES = {
     "fast-downward": ("up_fast_downward", "FastDownwardPDDLPlanner"),
     "fast-downward-opt": ("up_fast_downward", "FastDownwardOptimalPDDLPlanner"),
     "pyperplan": ("up_pyperplan.engine", "EngineImpl"),
@@ -393,85 +393,14 @@
             module = importlib.import_module(module_name)
             EngineImpl = getattr(module, class_name)
             self._meta_engines[name] = EngineImpl
             self._meta_engines_info.append((name, module_name, class_name))
         if EngineImpl.is_compatible_engine(engine):
             self._engines[f"{name}[{engine_name}]"] = EngineImpl[engine]
 
-    def _engine_satisfies_conditions(
-        self,
-        EngineClass: Type["up.engines.engine.Engine"],
-        operation_mode: "OperationMode",
-        problem_kind: ProblemKind,
-        optimality_guarantee: Optional["OptimalityGuarantee"],
-        compilation_kind: Optional["CompilationKind"],
-        plan_kind: Optional["PlanKind"],
-        anytime_guarantee: Optional["AnytimeGuarantee"],
-    ) -> bool:
-        if not getattr(EngineClass, "is_" + operation_mode.value)():
-            return False
-        if (
-            operation_mode == OperationMode.ONESHOT_PLANNER
-            or operation_mode == OperationMode.REPLANNER
-            or operation_mode == OperationMode.PORTFOLIO_SELECTOR
-        ):
-            assert (
-                issubclass(EngineClass, OneshotPlannerMixin)
-                or issubclass(EngineClass, ReplannerMixin)
-                or issubclass(EngineClass, PortfolioSelectorMixin)
-            )
-            assert anytime_guarantee is None
-            assert compilation_kind is None
-            assert plan_kind is None
-            if optimality_guarantee is not None and not EngineClass.satisfies(
-                optimality_guarantee
-            ):
-                return False
-        elif operation_mode == OperationMode.PLAN_VALIDATOR:
-            assert issubclass(EngineClass, PlanValidatorMixin)
-            assert optimality_guarantee is None
-            assert anytime_guarantee is None
-            assert compilation_kind is None
-            if plan_kind is not None and not EngineClass.supports_plan(plan_kind):
-                return False
-        elif operation_mode == OperationMode.COMPILER:
-            assert issubclass(EngineClass, CompilerMixin)
-            assert optimality_guarantee is None
-            assert anytime_guarantee is None
-            assert plan_kind is None
-            if compilation_kind is not None and not EngineClass.supports_compilation(
-                compilation_kind
-            ):
-                return False
-        elif operation_mode == OperationMode.ANYTIME_PLANNER:
-            assert issubclass(EngineClass, AnytimePlannerMixin)
-            assert optimality_guarantee is None
-            assert compilation_kind is None
-            assert plan_kind is None
-            if anytime_guarantee is not None and not EngineClass.ensures(
-                anytime_guarantee
-            ):
-                return False
-        elif operation_mode == OperationMode.PLAN_REPAIRER:
-            assert issubclass(EngineClass, PlanRepairerMixin)
-            assert anytime_guarantee is None
-            assert compilation_kind is None
-            if plan_kind is not None and not EngineClass.supports_plan(plan_kind):
-                return False
-            if optimality_guarantee is not None and not EngineClass.satisfies(
-                optimality_guarantee
-            ):
-                return False
-        else:
-            assert optimality_guarantee is None
-            assert anytime_guarantee is None
-            assert compilation_kind is None
-            assert plan_kind is None
-        return EngineClass.supports(problem_kind)
-
     def _get_engine_class(
         self,
         operation_mode: "OperationMode",
         name: Optional[str] = None,
         problem_kind: ProblemKind = ProblemKind(),
         optimality_guarantee: Optional["OptimalityGuarantee"] = None,
         compilation_kind: Optional["CompilationKind"] = None,
@@ -485,33 +414,85 @@
                 raise up.exceptions.UPNoRequestedEngineAvailableException
         problem_features = list(problem_kind.features)
         planners_features = []
         # Make sure that optimality guarantees and compilation kind are mutually exclusive
         assert optimality_guarantee is None or compilation_kind is None
         for name in self._preference_list:
             EngineClass = self._engines[name]
-            if self._engine_satisfies_conditions(
-                EngineClass,
-                operation_mode,
-                problem_kind,
-                optimality_guarantee,
-                compilation_kind,
-                plan_kind,
-                anytime_guarantee,
-            ):
-                return EngineClass
-            elif getattr(EngineClass, "is_" + operation_mode.value)():
-                # The EngineClass satisfies the given OperationMode but does not
-                # satisfy some other features; add it to the error report features if
-                # no NoSuitableEngineAvailable are found.
-                x = [name] + [
-                    str(EngineClass.supports(ProblemKind({f})))
-                    for f in problem_features
-                ]
-                planners_features.append(x)
+            if getattr(EngineClass, "is_" + operation_mode.value)():
+                if (
+                    operation_mode == OperationMode.ONESHOT_PLANNER
+                    or operation_mode == OperationMode.REPLANNER
+                    or operation_mode == OperationMode.PORTFOLIO_SELECTOR
+                ):
+                    assert (
+                        issubclass(EngineClass, OneshotPlannerMixin)
+                        or issubclass(EngineClass, ReplannerMixin)
+                        or issubclass(EngineClass, PortfolioSelectorMixin)
+                    )
+                    assert anytime_guarantee is None
+                    assert compilation_kind is None
+                    assert plan_kind is None
+                    if optimality_guarantee is not None and not EngineClass.satisfies(
+                        optimality_guarantee
+                    ):
+                        continue
+                elif operation_mode == OperationMode.PLAN_VALIDATOR:
+                    assert issubclass(EngineClass, PlanValidatorMixin)
+                    assert optimality_guarantee is None
+                    assert anytime_guarantee is None
+                    assert compilation_kind is None
+                    if plan_kind is not None and not EngineClass.supports_plan(
+                        plan_kind
+                    ):
+                        continue
+                elif operation_mode == OperationMode.COMPILER:
+                    assert issubclass(EngineClass, CompilerMixin)
+                    assert optimality_guarantee is None
+                    assert anytime_guarantee is None
+                    assert plan_kind is None
+                    if (
+                        compilation_kind is not None
+                        and not EngineClass.supports_compilation(compilation_kind)
+                    ):
+                        continue
+                elif operation_mode == OperationMode.ANYTIME_PLANNER:
+                    assert issubclass(EngineClass, AnytimePlannerMixin)
+                    assert optimality_guarantee is None
+                    assert compilation_kind is None
+                    assert plan_kind is None
+                    if anytime_guarantee is not None and not EngineClass.ensures(
+                        anytime_guarantee
+                    ):
+                        continue
+                elif operation_mode == OperationMode.PLAN_REPAIRER:
+                    assert issubclass(EngineClass, PlanRepairerMixin)
+                    assert anytime_guarantee is None
+                    assert compilation_kind is None
+                    if plan_kind is not None and not EngineClass.supports_plan(
+                        plan_kind
+                    ):
+                        continue
+                    if optimality_guarantee is not None and not EngineClass.satisfies(
+                        optimality_guarantee
+                    ):
+                        continue
+                else:
+                    assert optimality_guarantee is None
+                    assert anytime_guarantee is None
+                    assert compilation_kind is None
+                    assert plan_kind is None
+                if EngineClass.supports(problem_kind):
+                    return EngineClass
+                else:
+                    x = [name] + [
+                        str(EngineClass.supports(ProblemKind({f})))
+                        for f in problem_features
+                    ]
+                    planners_features.append(x)
         if len(planners_features) > 0:
             header = ["Engine"] + problem_features
             msg = f"No available engine supports all the problem features:\n{format_table(header, planners_features)}"
         elif compilation_kind is not None:
             msg = f"No available engine supports {compilation_kind}"
         elif plan_kind is not None:
             msg = f"No available engine supports {plan_kind}"
@@ -756,20 +737,15 @@
         * optimal (``OPTIMAL_PLANS``);
         * just a different plan, with no specific guarantee (``None``).
 
         It raises an exception if the problem has no optimality metrics and anytime_guarantee
         is equal to ``INCREASING_QUALITY`` or ``OPTIMAL_PLAN``.
         """
         if isinstance(anytime_guarantee, str):
-            try:
-                anytime_guarantee = AnytimeGuarantee[anytime_guarantee]
-            except KeyError:
-                raise UPUsageError(
-                    f"{anytime_guarantee} is not a valid AnytimeGuarantee."
-                )
+            anytime_guarantee = AnytimeGuarantee[anytime_guarantee]
         return self._get_engine(
             OperationMode.ANYTIME_PLANNER,
             name,
             None,
             params,
             problem_kind,
             anytime_guarantee=anytime_guarantee,
@@ -829,32 +805,26 @@
 
         *   | using ``names`` (the names of the specific compilers), ``params`` (compilers dependent options) and ``compilation_kinds``.
             | e.g. ``Compiler(names=['up_quantifiers_remover', 'up_grounder'], params=[{'opt1': 'val1'}, {'opt2': 'val2'}], compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])``
         *   | using ``problem_kind`` and ``compilation_kinds`` parameters.
             | e.g. ``Compiler(problem_kind=problem.kind, compilation_kinds=[QUANTIFIERS_REMOVING, GROUNDING])``
         """
         if isinstance(compilation_kind, str):
-            try:
-                compilation_kind = CompilationKind[compilation_kind]
-            except KeyError:
-                raise UPUsageError(
-                    f"{compilation_kind} is not a valid CompilationKind."
-                )
+            compilation_kind = CompilationKind[compilation_kind]
+
         kinds: Optional[List[CompilationKind]] = None
         if compilation_kinds is not None:
             kinds = []
             for kind in compilation_kinds:
                 if isinstance(kind, str):
-                    try:
-                        kinds.append(CompilationKind[kind])
-                    except KeyError:
-                        raise UPUsageError(f"{kind} is not a valid CompilationKind.")
+                    kinds.append(CompilationKind[kind])
                 else:
-                    assert isinstance(kind, CompilationKind), "Typing not respected"
+                    assert isinstance(kind, CompilationKind)
                     kinds.append(kind)
+
         return self._get_engine(
             OperationMode.COMPILER,
             name,
             names,
             params,
             problem_kind,
             compilation_kind=compilation_kind,
@@ -932,18 +902,15 @@
 
         *   | using ``name`` (the name of a plan repairer) and eventually ``params``.
             | e.g. ``PlanRepairer(name='xxx')``
         *   | using ``problem_kind``, ``plan_kind`` and ``optimality_guarantee``.
             | e.g. ``PlanRepairer(problem_kind=problem.kind, plan_kind=plan.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
         """
         if isinstance(plan_kind, str):
-            try:
-                plan_kind = PlanKind[plan_kind]
-            except KeyError:
-                raise UPUsageError(f"{plan_kind} is not a valid PlanKind.")
+            plan_kind = PlanKind[plan_kind]
         if isinstance(optimality_guarantee, str):
             try:
                 optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
             except KeyError:
                 raise UPUsageError(
                     f"{optimality_guarantee} is not a valid OptimalityGuarantee."
                 )
@@ -966,15 +933,15 @@
     ) -> "up.engines.engine.Engine":
         """
         Returns a portfolio selector. There are two ways to call this method:
 
         *   | using ``name`` (the name of a specific portfolio) and eventually ``params`` (portfolio dependent options).
             | e.g. ``PortfolioSelector(name='ibacop')``
         *   | using ``problem_kind`` and ``optimality_guarantee``.
-            | e.g. ``PortfolioSelector(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
+            | e.g. ``OneshotPlanner(problem_kind=problem.kind, optimality_guarantee=SOLVED_OPTIMALLY)``
         """
         if isinstance(optimality_guarantee, str):
             try:
                 optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
             except KeyError:
                 raise UPUsageError(
                     f"{optimality_guarantee} is not a valid OptimalityGuarantee."
@@ -986,95 +953,16 @@
             problem_kind=problem_kind,
             optimality_guarantee=optimality_guarantee,
         )
 
     def print_engines_info(
         self, stream: IO[str] = sys.stdout, full_credits: bool = True
     ):
-        """
-        Writes the info of all the installed engines in the given stream.
-
-        :param stream: The ``IO[str]`` where all the engine's info are written;
-            defaults to sys.stdout.
-        :param full_credits: If ``False`` a shorter version of the info is written;
-            defaults to ``True``.
-        """
         stream.write("These are the engines currently available:\n")
         for Engine in self._engines.values():
             credits = Engine.get_credits()
             if credits is not None:
                 stream.write("---------------------------------------\n")
                 credits.write_credits(stream, full_credits)
                 stream.write(
                     f"This engine supports the following features:\n{str(Engine.supported_kind())}\n\n"
                 )
-
-    def get_all_applicable_engines(
-        self,
-        problem_kind: ProblemKind,
-        operation_mode: OperationMode = OperationMode.ONESHOT_PLANNER,
-        *,
-        optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
-        anytime_guarantee: Optional[Union["AnytimeGuarantee", str]] = None,
-        plan_kind: Optional[Union["PlanKind", str]] = None,
-        compilation_kind: Optional[Union["CompilationKind", str]] = None,
-    ) -> List[str]:
-        """
-        | Returns all the engine names installed that are able to handle all the given
-          requirements.
-
-        | Since the semantic of the parameters given to this function depends on the chosen ``OperationMode``,
-          an user must have clear their meaning in the Operation Mode context.
-
-        :param problem_kind: An engine is returned only if it supports this ``problem_kind``.
-        :param operation_mode: An engine is returned only if it implements this ``operation_mode``; defaults to ``ONESHOT_PLANNER``.
-        :param optimality_guarantee: An engine is returned only if it satisfies this ``optimality_guarantee``. This parameter
-            can be specified only if the ``operation_mode`` is ``ONESHOT_PLANNER``, ``REPLANNER``, ``PLAN_REPAIRER``
-            or ``PORTFOLIO_SELECTOR``.
-        :param anytime_guarantee: An engine is returned only if it satisfies this ``anytime_guarantee``. This parameter
-            can be specified only if the ``operation_mode`` is ``ANYTIME_PLANNER``.
-        :param plan_kind: An engine is returned only if it is able to handle this ``plan_kind``. This parameter
-            can be specified only if the ``operation_mode`` is ``PLAN_VALIDATOR`` or ``PLAN_REPAIRER``.
-        :param compilation_kind: An engine is returned only if it is able to handle this ``compilation_kind``. This
-            parameter can be specified only if the ``operation_mode`` is ``COMPILER``.
-        :return: The list of engines names that satisfy all the given requirements.
-        """
-        if isinstance(optimality_guarantee, str):
-            try:
-                optimality_guarantee = OptimalityGuarantee[optimality_guarantee]
-            except KeyError:
-                raise UPUsageError(
-                    f"{optimality_guarantee} is not a valid OptimalityGuarantee."
-                )
-        if isinstance(anytime_guarantee, str):
-            try:
-                anytime_guarantee = AnytimeGuarantee[anytime_guarantee]
-            except KeyError:
-                raise UPUsageError(
-                    f"{anytime_guarantee} is not a valid AnytimeGuarantee."
-                )
-        if isinstance(compilation_kind, str):
-            try:
-                compilation_kind = CompilationKind[compilation_kind]
-            except KeyError:
-                raise UPUsageError(
-                    f"{compilation_kind} is not a valid CompilationKind."
-                )
-        if isinstance(plan_kind, str):
-            try:
-                plan_kind = PlanKind[plan_kind]
-            except KeyError:
-                raise UPUsageError(f"{plan_kind} is not a valid PlanKind.")
-        names: List[str] = []
-        for name in self._preference_list:
-            EngineClass = self._engines[name]
-            if self._engine_satisfies_conditions(
-                EngineClass,
-                operation_mode,
-                problem_kind,
-                cast(Optional[OptimalityGuarantee], optimality_guarantee),
-                cast(Optional[CompilationKind], compilation_kind),
-                plan_kind,
-                cast(Optional[AnytimeGuarantee], anytime_guarantee),
-            ):
-                names.append(name)
-        return names
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/meta_engine.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/meta_engine.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/anytime_planner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/anytime_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         return True
 
     @staticmethod
     def ensures(anytime_guarantee: AnytimeGuarantee) -> bool:
         """
         :param anytime_guarantee: The `anytime_guarantee` that must be satisfied.
         :return: `True` if the `AnytimePlannerMixin` implementation ensures the given
-            `anytime_guarantee`, `False` otherwise.
+        `anytime_guarantee`, `False` otherwise.
         """
         return False
 
     def get_solutions(
         self,
         problem: "up.model.AbstractProblem",
         timeout: Optional[float] = None,
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/compiler.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/compiler.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/oneshot_planner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/oneshot_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,17 @@
     @staticmethod
     def is_oneshot_planner() -> bool:
         return True
 
     @staticmethod
     def satisfies(optimality_guarantee: OptimalityGuarantee) -> bool:
         """
-        :param optimality_guarantee: The ``optimality_guarantee`` that must be satisfied.
-        :return: ``True`` if the ``OneshotPlannerMixin`` implementation satisfies the given
-            ``optimality_guarantee``, ``False`` otherwise.
+        :param optimality_guarantee: The `optimality_guarantee` that must be satisfied.
+        :return: `True` if the `OneshotPlannerMixin` implementation satisfies the given
+        `optimality_guarantee`, `False` otherwise.
         """
         return False
 
     def solve(
         self,
         problem: "up.model.AbstractProblem",
         heuristic: Optional[Callable[["up.model.state.State"], Optional[float]]] = None,
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/plan_repairer.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/plan_repairer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/plan_validator.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/portfolio.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     @staticmethod
     def satisfies(
         optimality_guarantee: "up.engines.mixins.oneshot_planner.OptimalityGuarantee",
     ) -> bool:
         """
         :param optimality_guarantee: The `optimality_guarantee` that must be satisfied.
         :return: `True` if the `PortfolioSelectorMixin` implementation satisfies the given
-            `optimality_guarantee`, `False` otherwise.
+        `optimality_guarantee`, `False` otherwise.
         """
         return False
 
     def get_best_oneshot_planners(
         self,
         problem: "up.model.AbstractProblem",
         max_planners: Optional[int] = None,
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/replanner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/mixins/sequential_simulator.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/mixins/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/oversubscription_planner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/oversubscription_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         supported_kind.set_time("CONTINUOUS_TIME")
         supported_kind.set_time("DISCRETE_TIME")
         supported_kind.set_time("INTERMEDIATE_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("EXTERNAL_CONDITIONS_AND_EFFECTS")
         supported_kind.set_time("TIMED_EFFECTS")
         supported_kind.set_time("TIMED_GOALS")
         supported_kind.set_time("DURATION_INEQUALITIES")
-        supported_kind.set_time("SELF_OVERLAPPING")
         supported_kind.set_expression_duration("STATIC_FLUENTS_IN_DURATIONS")
         supported_kind.set_expression_duration("FLUENTS_IN_DURATIONS")
         supported_kind.set_simulated_entities("SIMULATED_EFFECTS")
         final_supported_kind = supported_kind.intersection(engine.supported_kind())
         final_supported_kind.set_quality_metrics("OVERSUBSCRIPTION")
         final_supported_kind.set_quality_metrics("TEMPORAL_OVERSUBSCRIPTION")
         return final_supported_kind
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/parallel.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/parallel.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/pddl_planner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/plan_validator.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/replanner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/results.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/results.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/engines/sequential_simulator.py` & `unified_planning-0.6.0.9.dev1/unified_planning/engines/sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/environment.py` & `unified_planning-0.6.0.9.dev1/unified_planning/environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/exceptions.py` & `unified_planning-0.6.0.9.dev1/unified_planning/exceptions.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/grpc/converter.py` & `unified_planning-0.6.0.9.dev1/unified_planning/grpc/converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/grpc/generated/unified_planning_pb2.py` & `unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16unified_planning.proto\"i\n\nExpression\x12\x13\n\x04\x61tom\x18\x01 \x01(\x0b\x32\x05.Atom\x12\x19\n\x04list\x18\x02 \x03(\x0b\x32\x0b.Expression\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x1d\n\x04kind\x18\x04 \x01(\x0e\x32\x0f.ExpressionKind\"\\\n\x04\x41tom\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x15\n\x04real\x18\x03 \x01(\x0b\x32\x05.RealH\x00\x12\x11\n\x07\x62oolean\x18\x04 \x01(\x08H\x00\x42\t\n\x07\x63ontent\".\n\x04Real\x12\x11\n\tnumerator\x18\x01 \x01(\x03\x12\x13\n\x0b\x64\x65nominator\x18\x02 \x01(\x03\"9\n\x0fTypeDeclaration\x12\x11\n\ttype_name\x18\x01 \x01(\t\x12\x13\n\x0bparent_type\x18\x02 \x01(\t\"\'\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"n\n\x06\x46luent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nvalue_type\x18\x02 \x01(\t\x12\x1e\n\nparameters\x18\x03 \x03(\x0b\x32\n.Parameter\x12\"\n\rdefault_value\x18\x04 \x01(\x0b\x32\x0b.Expression\"/\n\x11ObjectDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\xcd\x01\n\x10\x45\x66\x66\x65\x63tExpression\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x1c.EffectExpression.EffectKind\x12\x1b\n\x06\x66luent\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x03 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\tcondition\x18\x04 \x01(\x0b\x32\x0b.Expression\"4\n\nEffectKind\x12\n\n\x06\x41SSIGN\x10\x00\x12\x0c\n\x08INCREASE\x10\x01\x12\x0c\n\x08\x44\x45\x43REASE\x10\x02\"M\n\x06\x45\x66\x66\x65\x63t\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"C\n\tCondition\x12\x19\n\x04\x63ond\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1b\n\x04span\x18\x02 \x01(\x0b\x32\r.TimeInterval\"\x8d\x01\n\x06\x41\x63tion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.Duration\x12\x1e\n\nconditions\x18\x04 \x03(\x0b\x32\n.Condition\x12\x18\n\x07\x65\x66\x66\x65\x63ts\x18\x05 \x03(\x0b\x32\x07.Effect\"\x90\x01\n\tTimepoint\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.Timepoint.TimepointKind\x12\x14\n\x0c\x63ontainer_id\x18\x02 \x01(\t\"E\n\rTimepointKind\x12\x10\n\x0cGLOBAL_START\x10\x00\x12\x0e\n\nGLOBAL_END\x10\x01\x12\t\n\x05START\x10\x02\x12\x07\n\x03\x45ND\x10\x03\"=\n\x06Timing\x12\x1d\n\ttimepoint\x18\x01 \x01(\x0b\x32\n.Timepoint\x12\x14\n\x05\x64\x65lay\x18\x02 \x01(\x0b\x32\x05.Real\"o\n\x08Interval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x1a\n\x05lower\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x1a\n\x05upper\x18\x04 \x01(\x0b\x32\x0b.Expression\"k\n\x0cTimeInterval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x16\n\x05lower\x18\x02 \x01(\x0b\x32\x07.Timing\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x16\n\x05upper\x18\x04 \x01(\x0b\x32\x07.Timing\"5\n\x08\x44uration\x12)\n\x16\x63ontrollable_in_bounds\x18\x01 \x01(\x0b\x32\t.Interval\"G\n\x17\x41\x62stractTaskDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\"F\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\ttask_name\x18\x02 \x01(\t\x12\x1f\n\nparameters\x18\x03 \x03(\x0b\x32\x0b.Expression\"\xaf\x01\n\x06Method\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1c\n\rachieved_task\x18\x03 \x01(\x0b\x32\x05.Task\x12\x17\n\x08subtasks\x18\x04 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x05 \x03(\x0b\x32\x0b.Expression\x12\x1e\n\nconditions\x18\x06 \x03(\x0b\x32\n.Condition\"g\n\x0bTaskNetwork\x12\x1d\n\tvariables\x18\x01 \x03(\x0b\x32\n.Parameter\x12\x17\n\x08subtasks\x18\x02 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x03 \x03(\x0b\x32\x0b.Expression\"\x83\x01\n\tHierarchy\x12\x30\n\x0e\x61\x62stract_tasks\x18\x01 \x03(\x0b\x32\x18.AbstractTaskDeclaration\x12\x18\n\x07methods\x18\x02 \x03(\x0b\x32\x07.Method\x12*\n\x14initial_task_network\x18\x03 \x01(\x0b\x32\x0c.TaskNetwork\"@\n\x04Goal\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\"R\n\x0bTimedEffect\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"E\n\nAssignment\x12\x1b\n\x06\x66luent\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression\"B\n\x0eGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x15\n\x06weight\x18\x02 \x01(\x0b\x32\x05.Real\"f\n\x13TimedGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\x12\x15\n\x06weight\x18\x03 \x01(\x0b\x32\x05.Real\"\x9c\x04\n\x06Metric\x12 \n\x04kind\x18\x01 \x01(\x0e\x32\x12.Metric.MetricKind\x12\x1f\n\nexpression\x18\x02 \x01(\x0b\x32\x0b.Expression\x12.\n\x0c\x61\x63tion_costs\x18\x03 \x03(\x0b\x32\x18.Metric.ActionCostsEntry\x12(\n\x13\x64\x65\x66\x61ult_action_cost\x18\x04 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\x05goals\x18\x05 \x03(\x0b\x32\x0f.GoalWithWeight\x12)\n\x0btimed_goals\x18\x06 \x03(\x0b\x32\x14.TimedGoalWithWeight\x1a?\n\x10\x41\x63tionCostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression:\x02\x38\x01\"\xe8\x01\n\nMetricKind\x12\x19\n\x15MINIMIZE_ACTION_COSTS\x10\x00\x12#\n\x1fMINIMIZE_SEQUENTIAL_PLAN_LENGTH\x10\x01\x12\x15\n\x11MINIMIZE_MAKESPAN\x10\x02\x12&\n\"MINIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x03\x12&\n\"MAXIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x04\x12\x14\n\x10OVERSUBSCRIPTION\x10\x05\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10\x06\"\xe2\x02\n\x07Problem\x12\x13\n\x0b\x64omain_name\x18\x01 \x01(\t\x12\x14\n\x0cproblem_name\x18\x02 \x01(\t\x12\x1f\n\x05types\x18\x03 \x03(\x0b\x32\x10.TypeDeclaration\x12\x18\n\x07\x66luents\x18\x04 \x03(\x0b\x32\x07.Fluent\x12#\n\x07objects\x18\x05 \x03(\x0b\x32\x12.ObjectDeclaration\x12\x18\n\x07\x61\x63tions\x18\x06 \x03(\x0b\x32\x07.Action\x12\"\n\rinitial_state\x18\x07 \x03(\x0b\x32\x0b.Assignment\x12#\n\rtimed_effects\x18\x08 \x03(\x0b\x32\x0c.TimedEffect\x12\x14\n\x05goals\x18\t \x03(\x0b\x32\x05.Goal\x12\x1a\n\x08\x66\x65\x61tures\x18\n \x03(\x0e\x32\x08.Feature\x12\x18\n\x07metrics\x18\x0b \x03(\x0b\x32\x07.Metric\x12\x1d\n\thierarchy\x18\x0c \x01(\x0b\x32\n.Hierarchy\"\x80\x01\n\x0e\x41\x63tionInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63tion_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12\x19\n\nstart_time\x18\x04 \x01(\x0b\x32\x05.Real\x12\x17\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x05.Real\"\xae\x01\n\x0eMethodInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12/\n\x08subtasks\x18\x06 \x03(\x0b\x32\x1d.MethodInstance.SubtasksEntry\x1a/\n\rSubtasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x96\x01\n\rPlanHierarchy\x12\x31\n\nroot_tasks\x18\x01 \x03(\x0b\x32\x1d.PlanHierarchy.RootTasksEntry\x12 \n\x07methods\x18\x02 \x03(\x0b\x32\x0f.MethodInstance\x1a\x30\n\x0eRootTasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"K\n\x04Plan\x12 \n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x0f.ActionInstance\x12!\n\thierarchy\x18\x02 \x01(\x0b\x32\x0e.PlanHierarchy\"\x83\x02\n\x0bPlanRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12*\n\x0fresolution_mode\x18\x02 \x01(\x0e\x32\x11.PlanRequest.Mode\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x37\n\x0e\x65ngine_options\x18\x04 \x03(\x0b\x32\x1f.PlanRequest.EngineOptionsEntry\x1a\x34\n\x12\x45ngineOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x04Mode\x12\x0f\n\x0bSATISFIABLE\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\"C\n\x11ValidationRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\"{\n\nLogMessage\x12#\n\x05level\x18\x01 \x01(\x0e\x32\x14.LogMessage.LogLevel\x12\x0f\n\x07message\x18\x02 \x01(\t\"7\n\x08LogLevel\x12\t\n\x05\x44\x45\x42UG\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\t\n\x05\x45RROR\x10\x03\"\xbf\x03\n\x14PlanGenerationResult\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.PlanGenerationResult.Status\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\x12\x33\n\x07metrics\x18\x03 \x03(\x0b\x32\".PlanGenerationResult.MetricsEntry\x12!\n\x0clog_messages\x18\x04 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x05 \x01(\x0b\x32\x07.Engine\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x01\n\x06Status\x12\x16\n\x12SOLVED_SATISFICING\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\x12\x15\n\x11UNSOLVABLE_PROVEN\x10\x02\x12\x1b\n\x17UNSOLVABLE_INCOMPLETELY\x10\x03\x12\x0b\n\x07TIMEOUT\x10\r\x12\n\n\x06MEMOUT\x10\x0e\x12\x12\n\x0eINTERNAL_ERROR\x10\x0f\x12\x17\n\x13UNSUPPORTED_PROBLEM\x10\x10\x12\x10\n\x0cINTERMEDIATE\x10\x11\"\x16\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xba\x01\n\x10ValidationResult\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.ValidationResult.ValidationResultStatus\x12!\n\x0clog_messages\x18\x02 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x03 \x01(\x0b\x32\x07.Engine\"0\n\x16ValidationResultStatus\x12\t\n\x05VALID\x10\x00\x12\x0b\n\x07INVALID\x10\x01\"\xe5\x01\n\x0e\x43ompilerResult\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x37\n\rmap_back_plan\x18\x02 \x03(\x0b\x32 .CompilerResult.MapBackPlanEntry\x12!\n\x0clog_messages\x18\x03 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x04 \x01(\x0b\x32\x07.Engine\x1a\x43\n\x10MapBackPlanEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.ActionInstance:\x02\x38\x01*\xb0\x01\n\x0e\x45xpressionKind\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x43ONSTANT\x10\x01\x12\r\n\tPARAMETER\x10\x02\x12\x0c\n\x08VARIABLE\x10\x07\x12\x11\n\rFLUENT_SYMBOL\x10\x03\x12\x13\n\x0f\x46UNCTION_SYMBOL\x10\x04\x12\x12\n\x0eSTATE_VARIABLE\x10\x05\x12\x18\n\x14\x46UNCTION_APPLICATION\x10\x06\x12\x10\n\x0c\x43ONTAINER_ID\x10\x08*\xd2\t\n\x07\x46\x65\x61ture\x12\x10\n\x0c\x41\x43TION_BASED\x10\x00\x12\x10\n\x0cHIERARCHICAL\x10\x1a\x12\x1b\n\x17SIMPLE_NUMERIC_PLANNING\x10\x1e\x12\x1c\n\x18GENERAL_NUMERIC_PLANNING\x10\x1f\x12\x13\n\x0f\x43ONTINUOUS_TIME\x10\x01\x12\x11\n\rDISCRETE_TIME\x10\x02\x12\'\n#INTERMEDIATE_CONDITIONS_AND_EFFECTS\x10\x03\x12#\n\x1f\x45XTERNAL_CONDITIONS_AND_EFFECTS\x10\'\x12\x11\n\rTIMED_EFFECTS\x10\x04\x12\x0f\n\x0bTIMED_GOALS\x10\x05\x12\x19\n\x15\x44URATION_INEQUALITIES\x10\x06\x12\x14\n\x10SELF_OVERLAPPING\x10/\x12\x1f\n\x1bSTATIC_FLUENTS_IN_DURATIONS\x10\x1b\x12\x18\n\x14\x46LUENTS_IN_DURATIONS\x10\x1c\x12\x16\n\x12\x43ONTINUOUS_NUMBERS\x10\x07\x12\x14\n\x10\x44ISCRETE_NUMBERS\x10\x08\x12\x11\n\rBOUNDED_TYPES\x10&\x12\x17\n\x13NEGATIVE_CONDITIONS\x10\t\x12\x1a\n\x16\x44ISJUNCTIVE_CONDITIONS\x10\n\x12\x0e\n\nEQUALITIES\x10\x0b\x12\x1a\n\x16\x45XISTENTIAL_CONDITIONS\x10\x0c\x12\x18\n\x14UNIVERSAL_CONDITIONS\x10\r\x12\x17\n\x13\x43ONDITIONAL_EFFECTS\x10\x0e\x12\x14\n\x10INCREASE_EFFECTS\x10\x0f\x12\x14\n\x10\x44\x45\x43REASE_EFFECTS\x10\x10\x12)\n%STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS\x10)\x12)\n%STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS\x10*\x12\"\n\x1e\x46LUENTS_IN_BOOLEAN_ASSIGNMENTS\x10+\x12\"\n\x1e\x46LUENTS_IN_NUMERIC_ASSIGNMENTS\x10,\x12\x0f\n\x0b\x46LAT_TYPING\x10\x11\x12\x17\n\x13HIERARCHICAL_TYPING\x10\x12\x12\x13\n\x0fNUMERIC_FLUENTS\x10\x13\x12\x12\n\x0eOBJECT_FLUENTS\x10\x14\x12\x10\n\x0c\x41\x43TIONS_COST\x10\x15\x12\x0f\n\x0b\x46INAL_VALUE\x10\x16\x12\x0c\n\x08MAKESPAN\x10\x17\x12\x0f\n\x0bPLAN_LENGTH\x10\x18\x12\x14\n\x10OVERSUBSCRIPTION\x10\x1d\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10(\x12\"\n\x1eSTATIC_FLUENTS_IN_ACTIONS_COST\x10-\x12\x1b\n\x17\x46LUENTS_IN_ACTIONS_COST\x10.\x12\x15\n\x11SIMULATED_EFFECTS\x10\x19\x12\x18\n\x14METHOD_PRECONDITIONS\x10 \x12\x1c\n\x18TASK_NETWORK_CONSTRAINTS\x10!\x12\"\n\x1eINITIAL_TASK_NETWORK_VARIABLES\x10\"\x12\x14\n\x10TASK_ORDER_TOTAL\x10#\x12\x16\n\x12TASK_ORDER_PARTIAL\x10$\x12\x17\n\x13TASK_ORDER_TEMPORAL\x10%2\xd8\x01\n\x0fUnifiedPlanning\x12\x34\n\x0bplanAnytime\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult0\x01\x12\x32\n\x0bplanOneShot\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult\x12\x35\n\x0cvalidatePlan\x12\x12.ValidationRequest\x1a\x11.ValidationResult\x12$\n\x07\x63ompile\x12\x08.Problem\x1a\x0f.CompilerResultb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16unified_planning.proto\"i\n\nExpression\x12\x13\n\x04\x61tom\x18\x01 \x01(\x0b\x32\x05.Atom\x12\x19\n\x04list\x18\x02 \x03(\x0b\x32\x0b.Expression\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x1d\n\x04kind\x18\x04 \x01(\x0e\x32\x0f.ExpressionKind\"\\\n\x04\x41tom\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12\r\n\x03int\x18\x02 \x01(\x03H\x00\x12\x15\n\x04real\x18\x03 \x01(\x0b\x32\x05.RealH\x00\x12\x11\n\x07\x62oolean\x18\x04 \x01(\x08H\x00\x42\t\n\x07\x63ontent\".\n\x04Real\x12\x11\n\tnumerator\x18\x01 \x01(\x03\x12\x13\n\x0b\x64\x65nominator\x18\x02 \x01(\x03\"9\n\x0fTypeDeclaration\x12\x11\n\ttype_name\x18\x01 \x01(\t\x12\x13\n\x0bparent_type\x18\x02 \x01(\t\"\'\n\tParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"n\n\x06\x46luent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\nvalue_type\x18\x02 \x01(\t\x12\x1e\n\nparameters\x18\x03 \x03(\x0b\x32\n.Parameter\x12\"\n\rdefault_value\x18\x04 \x01(\x0b\x32\x0b.Expression\"/\n\x11ObjectDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\xcd\x01\n\x10\x45\x66\x66\x65\x63tExpression\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x1c.EffectExpression.EffectKind\x12\x1b\n\x06\x66luent\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x03 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\tcondition\x18\x04 \x01(\x0b\x32\x0b.Expression\"4\n\nEffectKind\x12\n\n\x06\x41SSIGN\x10\x00\x12\x0c\n\x08INCREASE\x10\x01\x12\x0c\n\x08\x44\x45\x43REASE\x10\x02\"M\n\x06\x45\x66\x66\x65\x63t\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"C\n\tCondition\x12\x19\n\x04\x63ond\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1b\n\x04span\x18\x02 \x01(\x0b\x32\r.TimeInterval\"\x8d\x01\n\x06\x41\x63tion\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1b\n\x08\x64uration\x18\x03 \x01(\x0b\x32\t.Duration\x12\x1e\n\nconditions\x18\x04 \x03(\x0b\x32\n.Condition\x12\x18\n\x07\x65\x66\x66\x65\x63ts\x18\x05 \x03(\x0b\x32\x07.Effect\"\x90\x01\n\tTimepoint\x12&\n\x04kind\x18\x01 \x01(\x0e\x32\x18.Timepoint.TimepointKind\x12\x14\n\x0c\x63ontainer_id\x18\x02 \x01(\t\"E\n\rTimepointKind\x12\x10\n\x0cGLOBAL_START\x10\x00\x12\x0e\n\nGLOBAL_END\x10\x01\x12\t\n\x05START\x10\x02\x12\x07\n\x03\x45ND\x10\x03\"=\n\x06Timing\x12\x1d\n\ttimepoint\x18\x01 \x01(\x0b\x32\n.Timepoint\x12\x14\n\x05\x64\x65lay\x18\x02 \x01(\x0b\x32\x05.Real\"o\n\x08Interval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x1a\n\x05lower\x18\x02 \x01(\x0b\x32\x0b.Expression\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x1a\n\x05upper\x18\x04 \x01(\x0b\x32\x0b.Expression\"k\n\x0cTimeInterval\x12\x14\n\x0cis_left_open\x18\x01 \x01(\x08\x12\x16\n\x05lower\x18\x02 \x01(\x0b\x32\x07.Timing\x12\x15\n\ris_right_open\x18\x03 \x01(\x08\x12\x16\n\x05upper\x18\x04 \x01(\x0b\x32\x07.Timing\"5\n\x08\x44uration\x12)\n\x16\x63ontrollable_in_bounds\x18\x01 \x01(\x0b\x32\t.Interval\"G\n\x17\x41\x62stractTaskDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\"F\n\x04Task\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\ttask_name\x18\x02 \x01(\t\x12\x1f\n\nparameters\x18\x03 \x03(\x0b\x32\x0b.Expression\"\xaf\x01\n\x06Method\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1e\n\nparameters\x18\x02 \x03(\x0b\x32\n.Parameter\x12\x1c\n\rachieved_task\x18\x03 \x01(\x0b\x32\x05.Task\x12\x17\n\x08subtasks\x18\x04 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x05 \x03(\x0b\x32\x0b.Expression\x12\x1e\n\nconditions\x18\x06 \x03(\x0b\x32\n.Condition\"g\n\x0bTaskNetwork\x12\x1d\n\tvariables\x18\x01 \x03(\x0b\x32\n.Parameter\x12\x17\n\x08subtasks\x18\x02 \x03(\x0b\x32\x05.Task\x12 \n\x0b\x63onstraints\x18\x03 \x03(\x0b\x32\x0b.Expression\"\x83\x01\n\tHierarchy\x12\x30\n\x0e\x61\x62stract_tasks\x18\x01 \x03(\x0b\x32\x18.AbstractTaskDeclaration\x12\x18\n\x07methods\x18\x02 \x03(\x0b\x32\x07.Method\x12*\n\x14initial_task_network\x18\x03 \x01(\x0b\x32\x0c.TaskNetwork\"@\n\x04Goal\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\"R\n\x0bTimedEffect\x12!\n\x06\x65\x66\x66\x65\x63t\x18\x01 \x01(\x0b\x32\x11.EffectExpression\x12 \n\x0foccurrence_time\x18\x02 \x01(\x0b\x32\x07.Timing\"E\n\nAssignment\x12\x1b\n\x06\x66luent\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression\"B\n\x0eGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x15\n\x06weight\x18\x02 \x01(\x0b\x32\x05.Real\"f\n\x13TimedGoalWithWeight\x12\x19\n\x04goal\x18\x01 \x01(\x0b\x32\x0b.Expression\x12\x1d\n\x06timing\x18\x02 \x01(\x0b\x32\r.TimeInterval\x12\x15\n\x06weight\x18\x03 \x01(\x0b\x32\x05.Real\"\x9c\x04\n\x06Metric\x12 \n\x04kind\x18\x01 \x01(\x0e\x32\x12.Metric.MetricKind\x12\x1f\n\nexpression\x18\x02 \x01(\x0b\x32\x0b.Expression\x12.\n\x0c\x61\x63tion_costs\x18\x03 \x03(\x0b\x32\x18.Metric.ActionCostsEntry\x12(\n\x13\x64\x65\x66\x61ult_action_cost\x18\x04 \x01(\x0b\x32\x0b.Expression\x12\x1e\n\x05goals\x18\x05 \x03(\x0b\x32\x0f.GoalWithWeight\x12)\n\x0btimed_goals\x18\x06 \x03(\x0b\x32\x14.TimedGoalWithWeight\x1a?\n\x10\x41\x63tionCostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1a\n\x05value\x18\x02 \x01(\x0b\x32\x0b.Expression:\x02\x38\x01\"\xe8\x01\n\nMetricKind\x12\x19\n\x15MINIMIZE_ACTION_COSTS\x10\x00\x12#\n\x1fMINIMIZE_SEQUENTIAL_PLAN_LENGTH\x10\x01\x12\x15\n\x11MINIMIZE_MAKESPAN\x10\x02\x12&\n\"MINIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x03\x12&\n\"MAXIMIZE_EXPRESSION_ON_FINAL_STATE\x10\x04\x12\x14\n\x10OVERSUBSCRIPTION\x10\x05\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10\x06\"\xe2\x02\n\x07Problem\x12\x13\n\x0b\x64omain_name\x18\x01 \x01(\t\x12\x14\n\x0cproblem_name\x18\x02 \x01(\t\x12\x1f\n\x05types\x18\x03 \x03(\x0b\x32\x10.TypeDeclaration\x12\x18\n\x07\x66luents\x18\x04 \x03(\x0b\x32\x07.Fluent\x12#\n\x07objects\x18\x05 \x03(\x0b\x32\x12.ObjectDeclaration\x12\x18\n\x07\x61\x63tions\x18\x06 \x03(\x0b\x32\x07.Action\x12\"\n\rinitial_state\x18\x07 \x03(\x0b\x32\x0b.Assignment\x12#\n\rtimed_effects\x18\x08 \x03(\x0b\x32\x0c.TimedEffect\x12\x14\n\x05goals\x18\t \x03(\x0b\x32\x05.Goal\x12\x1a\n\x08\x66\x65\x61tures\x18\n \x03(\x0e\x32\x08.Feature\x12\x18\n\x07metrics\x18\x0b \x03(\x0b\x32\x07.Metric\x12\x1d\n\thierarchy\x18\x0c \x01(\x0b\x32\n.Hierarchy\"\x80\x01\n\x0e\x41\x63tionInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63tion_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12\x19\n\nstart_time\x18\x04 \x01(\x0b\x32\x05.Real\x12\x17\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x05.Real\"\xae\x01\n\x0eMethodInstance\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x19\n\nparameters\x18\x03 \x03(\x0b\x32\x05.Atom\x12/\n\x08subtasks\x18\x06 \x03(\x0b\x32\x1d.MethodInstance.SubtasksEntry\x1a/\n\rSubtasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x96\x01\n\rPlanHierarchy\x12\x31\n\nroot_tasks\x18\x01 \x03(\x0b\x32\x1d.PlanHierarchy.RootTasksEntry\x12 \n\x07methods\x18\x02 \x03(\x0b\x32\x0f.MethodInstance\x1a\x30\n\x0eRootTasksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"K\n\x04Plan\x12 \n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x0f.ActionInstance\x12!\n\thierarchy\x18\x02 \x01(\x0b\x32\x0e.PlanHierarchy\"\x83\x02\n\x0bPlanRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12*\n\x0fresolution_mode\x18\x02 \x01(\x0e\x32\x11.PlanRequest.Mode\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x37\n\x0e\x65ngine_options\x18\x04 \x03(\x0b\x32\x1f.PlanRequest.EngineOptionsEntry\x1a\x34\n\x12\x45ngineOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\x04Mode\x12\x0f\n\x0bSATISFIABLE\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\"C\n\x11ValidationRequest\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\"{\n\nLogMessage\x12#\n\x05level\x18\x01 \x01(\x0e\x32\x14.LogMessage.LogLevel\x12\x0f\n\x07message\x18\x02 \x01(\t\"7\n\x08LogLevel\x12\t\n\x05\x44\x45\x42UG\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\x0b\n\x07WARNING\x10\x02\x12\t\n\x05\x45RROR\x10\x03\"\xbf\x03\n\x14PlanGenerationResult\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.PlanGenerationResult.Status\x12\x13\n\x04plan\x18\x02 \x01(\x0b\x32\x05.Plan\x12\x33\n\x07metrics\x18\x03 \x03(\x0b\x32\".PlanGenerationResult.MetricsEntry\x12!\n\x0clog_messages\x18\x04 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x05 \x01(\x0b\x32\x07.Engine\x1a.\n\x0cMetricsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xc2\x01\n\x06Status\x12\x16\n\x12SOLVED_SATISFICING\x10\x00\x12\x14\n\x10SOLVED_OPTIMALLY\x10\x01\x12\x15\n\x11UNSOLVABLE_PROVEN\x10\x02\x12\x1b\n\x17UNSOLVABLE_INCOMPLETELY\x10\x03\x12\x0b\n\x07TIMEOUT\x10\r\x12\n\n\x06MEMOUT\x10\x0e\x12\x12\n\x0eINTERNAL_ERROR\x10\x0f\x12\x17\n\x13UNSUPPORTED_PROBLEM\x10\x10\x12\x10\n\x0cINTERMEDIATE\x10\x11\"\x16\n\x06\x45ngine\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xba\x01\n\x10ValidationResult\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.ValidationResult.ValidationResultStatus\x12!\n\x0clog_messages\x18\x02 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x03 \x01(\x0b\x32\x07.Engine\"0\n\x16ValidationResultStatus\x12\t\n\x05VALID\x10\x00\x12\x0b\n\x07INVALID\x10\x01\"\xe5\x01\n\x0e\x43ompilerResult\x12\x19\n\x07problem\x18\x01 \x01(\x0b\x32\x08.Problem\x12\x37\n\rmap_back_plan\x18\x02 \x03(\x0b\x32 .CompilerResult.MapBackPlanEntry\x12!\n\x0clog_messages\x18\x03 \x03(\x0b\x32\x0b.LogMessage\x12\x17\n\x06\x65ngine\x18\x04 \x01(\x0b\x32\x07.Engine\x1a\x43\n\x10MapBackPlanEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1e\n\x05value\x18\x02 \x01(\x0b\x32\x0f.ActionInstance:\x02\x38\x01*\xb0\x01\n\x0e\x45xpressionKind\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08\x43ONSTANT\x10\x01\x12\r\n\tPARAMETER\x10\x02\x12\x0c\n\x08VARIABLE\x10\x07\x12\x11\n\rFLUENT_SYMBOL\x10\x03\x12\x13\n\x0f\x46UNCTION_SYMBOL\x10\x04\x12\x12\n\x0eSTATE_VARIABLE\x10\x05\x12\x18\n\x14\x46UNCTION_APPLICATION\x10\x06\x12\x10\n\x0c\x43ONTAINER_ID\x10\x08*\xbc\t\n\x07\x46\x65\x61ture\x12\x10\n\x0c\x41\x43TION_BASED\x10\x00\x12\x10\n\x0cHIERARCHICAL\x10\x1a\x12\x1b\n\x17SIMPLE_NUMERIC_PLANNING\x10\x1e\x12\x1c\n\x18GENERAL_NUMERIC_PLANNING\x10\x1f\x12\x13\n\x0f\x43ONTINUOUS_TIME\x10\x01\x12\x11\n\rDISCRETE_TIME\x10\x02\x12\'\n#INTERMEDIATE_CONDITIONS_AND_EFFECTS\x10\x03\x12#\n\x1f\x45XTERNAL_CONDITIONS_AND_EFFECTS\x10\'\x12\x11\n\rTIMED_EFFECTS\x10\x04\x12\x0f\n\x0bTIMED_GOALS\x10\x05\x12\x19\n\x15\x44URATION_INEQUALITIES\x10\x06\x12\x1f\n\x1bSTATIC_FLUENTS_IN_DURATIONS\x10\x1b\x12\x18\n\x14\x46LUENTS_IN_DURATIONS\x10\x1c\x12\x16\n\x12\x43ONTINUOUS_NUMBERS\x10\x07\x12\x14\n\x10\x44ISCRETE_NUMBERS\x10\x08\x12\x11\n\rBOUNDED_TYPES\x10&\x12\x17\n\x13NEGATIVE_CONDITIONS\x10\t\x12\x1a\n\x16\x44ISJUNCTIVE_CONDITIONS\x10\n\x12\x0e\n\nEQUALITIES\x10\x0b\x12\x1a\n\x16\x45XISTENTIAL_CONDITIONS\x10\x0c\x12\x18\n\x14UNIVERSAL_CONDITIONS\x10\r\x12\x17\n\x13\x43ONDITIONAL_EFFECTS\x10\x0e\x12\x14\n\x10INCREASE_EFFECTS\x10\x0f\x12\x14\n\x10\x44\x45\x43REASE_EFFECTS\x10\x10\x12)\n%STATIC_FLUENTS_IN_BOOLEAN_ASSIGNMENTS\x10)\x12)\n%STATIC_FLUENTS_IN_NUMERIC_ASSIGNMENTS\x10*\x12\"\n\x1e\x46LUENTS_IN_BOOLEAN_ASSIGNMENTS\x10+\x12\"\n\x1e\x46LUENTS_IN_NUMERIC_ASSIGNMENTS\x10,\x12\x0f\n\x0b\x46LAT_TYPING\x10\x11\x12\x17\n\x13HIERARCHICAL_TYPING\x10\x12\x12\x13\n\x0fNUMERIC_FLUENTS\x10\x13\x12\x12\n\x0eOBJECT_FLUENTS\x10\x14\x12\x10\n\x0c\x41\x43TIONS_COST\x10\x15\x12\x0f\n\x0b\x46INAL_VALUE\x10\x16\x12\x0c\n\x08MAKESPAN\x10\x17\x12\x0f\n\x0bPLAN_LENGTH\x10\x18\x12\x14\n\x10OVERSUBSCRIPTION\x10\x1d\x12\x1d\n\x19TEMPORAL_OVERSUBSCRIPTION\x10(\x12\"\n\x1eSTATIC_FLUENTS_IN_ACTIONS_COST\x10-\x12\x1b\n\x17\x46LUENTS_IN_ACTIONS_COST\x10.\x12\x15\n\x11SIMULATED_EFFECTS\x10\x19\x12\x18\n\x14METHOD_PRECONDITIONS\x10 \x12\x1c\n\x18TASK_NETWORK_CONSTRAINTS\x10!\x12\"\n\x1eINITIAL_TASK_NETWORK_VARIABLES\x10\"\x12\x14\n\x10TASK_ORDER_TOTAL\x10#\x12\x16\n\x12TASK_ORDER_PARTIAL\x10$\x12\x17\n\x13TASK_ORDER_TEMPORAL\x10%2\xd8\x01\n\x0fUnifiedPlanning\x12\x34\n\x0bplanAnytime\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult0\x01\x12\x32\n\x0bplanOneShot\x12\x0c.PlanRequest\x1a\x15.PlanGenerationResult\x12\x35\n\x0cvalidatePlan\x12\x12.ValidationRequest\x1a\x11.ValidationResult\x12$\n\x07\x63ompile\x12\x08.Problem\x1a\x0f.CompilerResultb\x06proto3')
 
 _EXPRESSIONKIND = DESCRIPTOR.enum_types_by_name['ExpressionKind']
 ExpressionKind = enum_type_wrapper.EnumTypeWrapper(_EXPRESSIONKIND)
 _FEATURE = DESCRIPTOR.enum_types_by_name['Feature']
 Feature = enum_type_wrapper.EnumTypeWrapper(_FEATURE)
 UNKNOWN = 0
 CONSTANT = 1
@@ -37,15 +37,14 @@
 CONTINUOUS_TIME = 1
 DISCRETE_TIME = 2
 INTERMEDIATE_CONDITIONS_AND_EFFECTS = 3
 EXTERNAL_CONDITIONS_AND_EFFECTS = 39
 TIMED_EFFECTS = 4
 TIMED_GOALS = 5
 DURATION_INEQUALITIES = 6
-SELF_OVERLAPPING = 47
 STATIC_FLUENTS_IN_DURATIONS = 27
 FLUENTS_IN_DURATIONS = 28
 CONTINUOUS_NUMBERS = 7
 DISCRETE_NUMBERS = 8
 BOUNDED_TYPES = 38
 NEGATIVE_CONDITIONS = 9
 DISJUNCTIVE_CONDITIONS = 10
@@ -468,15 +467,15 @@
   _PLANGENERATIONRESULT_METRICSENTRY._options = None
   _PLANGENERATIONRESULT_METRICSENTRY._serialized_options = b'8\001'
   _COMPILERRESULT_MAPBACKPLANENTRY._options = None
   _COMPILERRESULT_MAPBACKPLANENTRY._serialized_options = b'8\001'
   _EXPRESSIONKIND._serialized_start=5268
   _EXPRESSIONKIND._serialized_end=5444
   _FEATURE._serialized_start=5447
-  _FEATURE._serialized_end=6681
+  _FEATURE._serialized_end=6659
   _EXPRESSION._serialized_start=26
   _EXPRESSION._serialized_end=131
   _ATOM._serialized_start=133
   _ATOM._serialized_end=225
   _REAL._serialized_start=227
   _REAL._serialized_end=273
   _TYPEDECLARATION._serialized_start=275
@@ -573,10 +572,10 @@
   _VALIDATIONRESULT._serialized_end=5033
   _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_start=4985
   _VALIDATIONRESULT_VALIDATIONRESULTSTATUS._serialized_end=5033
   _COMPILERRESULT._serialized_start=5036
   _COMPILERRESULT._serialized_end=5265
   _COMPILERRESULT_MAPBACKPLANENTRY._serialized_start=5198
   _COMPILERRESULT_MAPBACKPLANENTRY._serialized_end=5265
-  _UNIFIEDPLANNING._serialized_start=6684
-  _UNIFIEDPLANNING._serialized_end=6900
+  _UNIFIEDPLANNING._serialized_start=6662
+  _UNIFIEDPLANNING._serialized_end=6878
 # @@protoc_insertion_point(module_scope)
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py` & `unified_planning-0.6.0.9.dev1/unified_planning/grpc/generated/unified_planning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/grpc/proto_reader.py` & `unified_planning-0.6.0.9.dev1/unified_planning/grpc/proto_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/grpc/proto_writer.py` & `unified_planning-0.6.0.9.dev1/unified_planning/grpc/proto_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,15 +524,15 @@
             abstract_tasks=[self.convert(t) for t in problem.tasks],
             methods=[self.convert(m) for m in problem.methods],
         )
 
     @handles(model.Problem, model.htn.HierarchicalProblem)
     def _convert_problem(self, problem: model.Problem) -> proto.Problem:
         goals = [proto.Goal(goal=self.convert(g)) for g in problem.goals]
-        for t, gs in problem.timed_goals.items():
+        for t, gs in problem.timed_goals:
             goals += [
                 proto.Goal(goal=self.convert(g), timing=self.convert(t)) for g in gs
             ]
 
         problem_name = str(problem.name) if problem.name is not None else ""
         hierarchy = None
         if isinstance(problem, model.htn.HierarchicalProblem):
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/interop/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/interop/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/interop/from_tarski.py` & `unified_planning-0.6.0.9.dev1/unified_planning/interop/from_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/interop/to_tarski.py` & `unified_planning-0.6.0.9.dev1/unified_planning/interop/to_tarski.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/io/anml_grammar.py` & `unified_planning-0.6.0.9.dev1/unified_planning/io/anml_grammar.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/io/anml_reader.py` & `unified_planning-0.6.0.9.dev1/unified_planning/io/anml_reader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 
     #. statements containing the duration of an action are **not** mixed with other statements ( ``duration == 3 and at(l_from);`` ).
     #. the action duration can be set with:
 
         * ``duration == expression;``
         * ``duration := expression;``
         * ``duration CT expression and duration CT expression``, where ``CT`` are Compare Tokens, so ``>``, ``>=``, ``<`` and ``<=``.
-
         All the other ways to define the duration of an Action are not supported.
+
     #. Statements containing both conditions and effects are **not** supported ( ``(at(l_from) == true) := false);`` or ``(at(l_from) == true) and (at(l_from) := false);`` ).
     #. Quantifier body does not support intervals, they can only be defined outside.
     #. Conditional effects are not supported inside an expression block.
     """
 
     def __init__(self, env: Optional[Environment] = None):
         self._env = get_environment(env)
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/io/anml_writer.py` & `unified_planning-0.6.0.9.dev1/unified_planning/io/anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/io/ma_pddl_writer.py` & `unified_planning-0.6.0.9.dev1/unified_planning/io/ma_pddl_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/io/pddl_reader.py` & `unified_planning-0.6.0.9.dev1/unified_planning/io/pddl_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/io/pddl_writer.py` & `unified_planning-0.6.0.9.dev1/unified_planning/io/pddl_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/io/utils.py` & `unified_planning-0.6.0.9.dev1/unified_planning/io/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/abstract_problem.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/abstract_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/action.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/contingent_problem.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/contingent_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/delta_stn.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/delta_stn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/effect.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/effect.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/expression.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/expression.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/fluent.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/fluent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/fnode.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/fnode.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/htn/hierarchical_problem.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/hierarchical_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/htn/method.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/method.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/htn/ordering.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/ordering.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/htn/task.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/task.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/htn/task_network.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/htn/task_network.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/metrics.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/actions_set.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/actions_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/agents_set.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/agents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/fluents_set.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/fluents_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/initial_state.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/initial_state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/metrics.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/objects_set.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/objects_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/time_model.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/time_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,19 +29,17 @@
     request.
     """
 
     def __init__(
         self,
         epsilon_default: Optional[Fraction],
         discrete_time: bool,
-        self_overlapping: bool,
     ):
         self._epsilon = epsilon_default
         self._discrete_time = discrete_time
-        self._self_overlapping = self_overlapping
 
     @property
     def epsilon(self) -> Optional[Fraction]:
         """
         This parameter has meaning only in temporal problems: it defines the minimum
         amount of time that can elapse between 2 temporal events. A temporal event can
         be, for example, the start of an action, the end of an action, an intermediate
@@ -71,23 +69,10 @@
         """Returns True if the problem time is discrete, False if it is continuous."""
         return self._discrete_time
 
     @discrete_time.setter
     def discrete_time(self, new_value: bool):
         self._discrete_time = new_value
 
-    @property
-    def self_overlapping(self) -> bool:
-        """
-        The ``self_overlapping`` flag determines if 2 (or more) different instances of the same
-        action grounded with the same parameters can be running at the same time.
-        """
-        return self._self_overlapping
-
-    @self_overlapping.setter
-    def self_overlapping(self, new_value: bool):
-        self._self_overlapping = new_value
-
     def _clone_to(self, other: "TimeModelMixin"):
         other.epsilon = self._epsilon
         other.discrete_time = self._discrete_time
-        other.self_overlapping = self._self_overlapping
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/timed_conds_effs.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/timed_conds_effs.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/mixins/user_types_set.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/mixins/user_types_set.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/agent.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/ma_environment.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/ma_environment.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/multi_agent/ma_problem.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/multi_agent/ma_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/object.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/object.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/operators.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/operators.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/parameter.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/parameter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/problem.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,17 +60,15 @@
         name: Optional[str] = None,
         environment: Optional["up.environment.Environment"] = None,
         *,
         initial_defaults: Dict["up.model.types.Type", "ConstantExpression"] = {},
     ):
         AbstractProblem.__init__(self, name, environment)
         UserTypesSetMixin.__init__(self, self.environment, self.has_name)
-        TimeModelMixin.__init__(
-            self, epsilon_default=None, discrete_time=False, self_overlapping=False
-        )
+        TimeModelMixin.__init__(self, epsilon_default=None, discrete_time=False)
         FluentsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name, initial_defaults
         )
         ActionsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name
         )
         ObjectsSetMixin.__init__(
@@ -673,18 +671,14 @@
             self._kind.unset_problem_type("SIMPLE_NUMERIC_PLANNING")
         else:
             if not self._kind.has_simple_numeric_planning():
                 self._kind.set_problem_type("GENERAL_NUMERIC_PLANNING")
         if self._kind.has_continuous_time() and self.discrete_time:
             self._kind.set_time("DISCRETE_TIME")
             self._kind.unset_time("CONTINUOUS_TIME")
-        if self._self_overlapping and (
-            self._kind.has_continuous_time() or self._kind.has_discrete_time()
-        ):
-            self._kind.set_time("SELF_OVERLAPPING")
         return self._kind
 
     def _update_problem_kind_effect(
         self,
         e: "up.model.effect.Effect",
         fluents_to_only_increase: Set["up.model.fluent.Fluent"],
         fluents_to_only_decrease: Set["up.model.fluent.Fluent"],
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/problem_kind.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/problem_kind.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
         "CONTINUOUS_TIME",
         "DISCRETE_TIME",
         "INTERMEDIATE_CONDITIONS_AND_EFFECTS",
         "EXTERNAL_CONDITIONS_AND_EFFECTS",
         "TIMED_EFFECTS",
         "TIMED_GOALS",
         "DURATION_INEQUALITIES",
-        "SELF_OVERLAPPING",
     ],
     "EXPRESSION_DURATION": ["STATIC_FLUENTS_IN_DURATIONS", "FLUENTS_IN_DURATIONS"],
     "NUMBERS": ["CONTINUOUS_NUMBERS", "DISCRETE_NUMBERS", "BOUNDED_TYPES"],
     "CONDITIONS_KIND": [
         "NEGATIVE_CONDITIONS",
         "DISJUNCTIVE_CONDITIONS",
         "EQUALITIES",
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/scheduling/activity.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/activity.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/scheduling/chronicle.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/chronicle.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/scheduling/scheduling_problem.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/scheduling/scheduling_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,32 +41,27 @@
     - it provides some shortcuts to deal with typical scheduling constructs (activities, resources, ...)
     """
 
     @property
     def kind(self) -> "up.model.problem_kind.ProblemKind":
         self._kind = up.model.problem_kind.ProblemKind()
         self._kind.set_problem_class("SCHEDULING")
-        # TODO: complete with more precise kinds
+        # TODO: complete with ore precise kinds
         return self._kind
 
     def __init__(
         self,
         name: Optional[str] = None,
         environment: Optional["up.environment.Environment"] = None,
         *,
         initial_defaults: Dict["up.model.types.Type", "ConstantExpression"] = {},
     ):
         AbstractProblem.__init__(self, name, environment)
         UserTypesSetMixin.__init__(self, self.environment, self.has_name)
-        TimeModelMixin.__init__(
-            self,
-            epsilon_default=Fraction(1),
-            discrete_time=True,
-            self_overlapping=False,
-        )
+        TimeModelMixin.__init__(self, epsilon_default=Fraction(1), discrete_time=True)
         FluentsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name, initial_defaults
         )
         ObjectsSetMixin.__init__(
             self, self.environment, self._add_user_type, self.has_name
         )
         InitialStateMixin.__init__(self, self, self, self.environment)
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/state.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/state.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/action.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/action.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/objects.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/objects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/path.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/path.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/tamp/types.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/tamp/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/timing.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/timing.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/type_manager.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/type_manager.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/types.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/types.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/variable.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/variable.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/any.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/any.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/dag.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/dag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/dnf.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/expression_quantifiers_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/fluents_substituter.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/fluents_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/free_vars.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/free_vars.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/generic.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,21 @@
 # NodeType to Function Name
 def nt_to_fun(o: OperatorKind) -> str:
     """Returns the name of the walk function for the given nodetype."""
     return "walk_%s" % (str(o).replace("OperatorKind.", "")).lower()
 
 
 class handles(object):
-    """
-    Decorator for walker functions.
+    """Decorator for walker functions.
     Use it by specifying the nodetypes that need to be handled by the
-    given function. It is possible to use grouped (e.g., OperatorKind.RELATIONS)
+    given function. It is possible to use groupd (e.g., OperatorKind.RELATIONS)
     directly. ::
-
-        `@handles(OperatorKind.NODE, ...)
-        def walk_special(...):
-            ...`
+    `@handles(OperatorKind.NODE, ...)
+    def walk_special(...):
+        ...`
 
     """
 
     def __init__(self, *nodetypes):
         if len(nodetypes) == 1 and isinstance(nodetypes[0], Iterable):
             nodetypes = nodetypes[0]  # type: ignore
         self.nodetypes = list(nodetypes)
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/identitydag.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/identitydag.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/linear_checker.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/linear_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/names_extractor.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/names_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/operators_extractor.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/operators_extractor.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/quantifier_simplifier.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/quantifier_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/simplifier.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/state_evaluator.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/state_evaluator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/substituter.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/type_checker.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/type_checker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/model/walkers/usertype_fluents_walker.py` & `unified_planning-0.6.0.9.dev1/unified_planning/model/walkers/usertype_fluents_walker.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/plans/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/plans/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/plans/contingent_plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/plans/contingent_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/plans/hierarchical_plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/plans/hierarchical_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/plans/partial_order_plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/plans/partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/plans/plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/plans/plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/plans/sequential_plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/plans/sequential_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             ["plans.plan.ActionInstance"], Optional["plans.plan.ActionInstance"]
         ],
     ) -> "up.plans.plan.Plan":
         """
         Returns a new `SequentialPlan` where every `ActionInstance` of the current `Plan` is replaced using the given function.
 
         :param replace_function: The function that applied to an `ActionInstance A` returns the `ActionInstance B`; `B`
-            replaces `A` in the resulting `SequentialPlan`.
+        replaces `A` in the resulting `SequentialPlan`.
         :return: The `SequentialPlan` where every `ActionInstance` is replaced using the given `replace_function`.
         """
         new_ai = []
         for ai in self._actions:
             replaced_ai = replace_function(ai)
             if replaced_ai is not None:
                 new_ai.append(replaced_ai)
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/plans/stn_plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/plans/stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/plans/time_triggered_plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/plans/time_triggered_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/shortcuts.py` & `unified_planning-0.6.0.9.dev1/unified_planning/shortcuts.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,17 @@
 from unified_planning.model import *
 from unified_planning.model.tamp import *
 from unified_planning.engines import (
     Engine,
     CompilationKind,
     OptimalityGuarantee,
     OperationMode,
-    AnytimeGuarantee,
 )
 from unified_planning.plans import PlanKind
-from typing import IO, Any, Iterable, Union, Dict, Optional, Sequence, List
+from typing import IO, Any, Iterable, Union, Dict, Optional, Sequence
 from fractions import Fraction
 
 
 def And(*args: Union[BoolExpression, Iterable[BoolExpression]]) -> FNode:
     """
     | Returns a conjunction of terms.
     | This function has polymorphic n-arguments:
@@ -739,52 +738,13 @@
         name=name,
         params=params,
         problem_kind=problem_kind,
         optimality_guarantee=optimality_guarantee,
     )
 
 
-def get_all_applicable_engines(
-    problem_kind: ProblemKind,
-    operation_mode: OperationMode = OperationMode.ONESHOT_PLANNER,
-    *,
-    optimality_guarantee: Optional[Union["OptimalityGuarantee", str]] = None,
-    anytime_guarantee: Optional[Union["AnytimeGuarantee", str]] = None,
-    plan_kind: Optional[Union["PlanKind", str]] = None,
-    compilation_kind: Optional[Union["CompilationKind", str]] = None,
-) -> List[str]:
-    """
-    | Returns all the engine names installed that are able to handle all the given
-        requirements.
-
-    | Since the semantic of the parameters given to this function depends on the chosen ``OperationMode``,
-        an user must have clear their meaning in the Operation Mode context.
-
-    :param problem_kind: An engine is returned only if it supports this ``problem_kind``.
-    :param operation_mode: An engine is returned only if it implements this ``operation_mode``; defaults to ``ONESHOT_PLANNER``.
-    :param optimality_guarantee: An engine is returned only if it satisfies this ``optimality_guarantee``. This parameter
-        can be specified only if the ``operation_mode`` is ``ONESHOT_PLANNER``, ``REPLANNER``, ``PLAN_REPAIRER``
-        or ``PORTFOLIO_SELECTOR``.
-    :param anytime_guarantee: An engine is returned only if it satisfies this ``anytime_guarantee``. This parameter
-        can be specified only if the ``operation_mode`` is ``ANYTIME_PLANNER``.
-    :param plan_kind: An engine is returned only if it is able to handle this ``plan_kind``. This parameter
-        can be specified only if the ``operation_mode`` is ``PLAN_VALIDATOR`` or ``PLAN_REPAIRER``.
-    :param compilation_kind: An engine is returned only if it is able to handle this ``compilation_kind``. This
-        parameter can be specified only if the ``operation_mode`` is ``COMPILER``.
-    :return: The list of engines names that satisfy all the given requirements.
-    """
-    return get_environment().factory.get_all_applicable_engines(
-        problem_kind,
-        operation_mode,
-        optimality_guarantee=optimality_guarantee,
-        anytime_guarantee=anytime_guarantee,
-        plan_kind=plan_kind,
-        compilation_kind=compilation_kind,
-    )
-
-
 def print_engines_info(stream: IO[str] = sys.stdout, full_credits: bool = False):
     get_environment().factory.print_engines_info(stream, full_credits)
 
 
 def set_credits_stream(stream: Optional[IO[str]]):
     get_environment().credits_stream = stream
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/connected_locations.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/connected_locations.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/constants.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/constants.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/constants_no_variable_duration.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/constants_no_variable_duration.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/forall.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/forall.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/hierarchical_blocks_world.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/hydrone.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/hydrone.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/match.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/match_int_id.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match_int_id.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/match_test_parser.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/match_test_parser.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/anml/simple_mais.anml` & `unified_planning-0.6.0.9.dev1/unified_planning/test/anml/simple_mais.anml`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/colorballs/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/contingent_pddl/logistic_conf/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/examples/__init__.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/examples/hierarchical.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/hierarchical.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/examples/minimals.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/minimals.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/examples/multi_agent.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/examples/realistic.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/realistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -882,21 +882,14 @@
                 Fraction(10, 1),
             ),
         ]
     )
     robot_static_fluents_duration = Example(problem=problem, plan=t_plan)
     problems["robot_with_static_fluents_duration"] = robot_static_fluents_duration
 
-    # Robot with timed_goals (extension of the previous problem with timed goals)
-    problem = problem.clone()
-    name = "robot_with_static_fluents_duration_timed_goals"
-    problem.name = name
-    problem.add_timed_goal(GlobalStartTiming() + 50, is_at(l5, r1))
-    problems[name] = Example(problem=problem, plan=t_plan)
-
     # travel
     problem = Problem("travel")
 
     Location = UserType("Location")
 
     is_at = Fluent("is_at", BoolType(), position=Location)
     is_connected = Fluent("is_connected", BoolType(), l_from=Location, l_to=Location)
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/examples/tamp.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/examples/testing_variants.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/examples/testing_variants.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-PCP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Rover/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Satellite/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-po-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-AssemblyHierarchical/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Blocksworld-HPDDL/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Childsnack/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Depots/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Elevator-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Entertainment/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Factories-simple/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Hiking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Logistics-Learned-ECAI-16/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Player/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Minecraft-Regular/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Fully-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Monroe-Partially-Observable/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Multiarm-Blocksworld/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Robot/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Rover-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Satellite-GTOHP/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Snake/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Towers/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Transport/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/hddl/2020-to-Woodworking/instance.1.pb.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/citycar/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/citycar/problem.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/citycar/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/counters/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/counters/problem2.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/counters/problem2.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/depot/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/depot/problem.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/depot/problem.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/enhsp.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/enhsp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/htn-transport/domain.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/domain.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/htn-transport/problem.hddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/htn-transport/problem.hddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/matchcellar/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/matchcellar/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/miconic/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/miconic/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/robot_fastener/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/safe_road/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/safe_road/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/sailing/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/sailing/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl` & `unified_planning-0.6.0.9.dev1/unified_planning/test/pddl/visit_precedence/domain.pddl`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/scheduling/examples.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/examples.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/scheduling/jobshop.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/scheduling/jobshop.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_anml_reader.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_anml_reader.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_anml_writer.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_anml_writer.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_anytime.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_anytime.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_bounded_types_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_bounded_types_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_compilers_pipeline.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_compilers_pipeline.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_compilers_quality_metrics.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_compilers_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_conditional_effects_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_conditional_effects_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_contingent_pddl.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_contingent_pddl.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_credits.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_credits.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_disjunctive_conditions_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_disjunctive_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_dnf.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_dnf.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_expression_analysis.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_expression_analysis.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_factory.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,50 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import inspect
 import tempfile
 import unified_planning
-from unified_planning.test.examples import get_example_problems
 from unified_planning.shortcuts import *
 from unified_planning.test import TestCase, skipIfEngineNotAvailable
 
 
 class TestFactory(TestCase):
-    def setUp(self):
-        TestCase.setUp(self)
-        self.problems = get_example_problems()
-
     @skipIfEngineNotAvailable("pyperplan")
     @skipIfEngineNotAvailable("tamer")
     def test_config_file(self):
         self.assertTrue("pyperplan" in get_environment().factory.preference_list)
         with tempfile.TemporaryDirectory() as tempdir:
             config_filename = os.path.join(tempdir, "up.ini")
             with open(config_filename, "w") as config:
                 config.write("[global]\n")
                 config.write("engine_preference_list: tamer\n")
             environment = unified_planning.environment.Environment()
             environment.factory.configure_from_file(config_filename)
             self.assertTrue("pyperplan" not in environment.factory.preference_list)
             self.assertEqual(environment.factory.preference_list, ["tamer"])
-
-    @skipIfEngineNotAvailable("pyperplan")
-    @skipIfEngineNotAvailable("tamer")
-    @skipIfEngineNotAvailable("opt-pddl-planner")
-    def test_get_all_applicable_engines(self):
-        problem = self.problems["basic"].problem
-        factory = problem.environment.factory
-        names = factory.get_all_applicable_engines(problem.kind)
-        expected_names = ["tamer", "opt-pddl-planner"]
-        for name in expected_names:
-            self.assertIn(name, names)
-
-        problem = self.problems["basic_without_negative_preconditions"].problem
-        names = factory.get_all_applicable_engines(problem.kind)
-        expected_names = ["tamer", "opt-pddl-planner", "pyperplan"]
-        for name in expected_names:
-            self.assertIn(name, names)
-
-        global_env_names = get_all_applicable_engines(problem.kind)
-        self.assertEqual(global_env_names, names)
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_grounder.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_htn.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_htn.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_infix_notation.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_infix_notation.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_model.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_model.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_multi_agent.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_multi_agent.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_negative_conditions_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_negative_conditions_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_partial_order_plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_partial_order_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_pddl_io.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_pddl_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,14 @@
         for example in self.problems.values():
             problem = example.problem
             kind = problem.kind
             if (
                 kind.has_intermediate_conditions_and_effects()
                 or kind.has_object_fluents()
                 or kind.has_oversubscription()
-                or kind.has_timed_goals()
             ):
                 continue
             with tempfile.TemporaryDirectory() as tempdir:
                 domain_filename = os.path.join(tempdir, "domain.pddl")
                 problem_filename = os.path.join(tempdir, "problem.pddl")
 
                 w = PDDLWriter(problem)
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_pddl_planner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_pddl_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_plan_validator.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_plan_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_planner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_planner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_problem.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_problem.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_protobuf_io.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_protobuf_io.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_pyperplan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_pyperplan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_quantifier_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_quantifier_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_replanner.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_replanner.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_scheduling.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_sequential_simulator.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_sequential_simulator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_simplifier.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_simplifier.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_simulated_effects.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_simulated_effects.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_stn_plan.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_stn_plan.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_substituter.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_substituter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_tamp.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_tamp.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_tarski_converter.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_tarski_converter.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_tarski_grounder.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_tarski_grounder.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_temporal.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_temporal.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_trajectory_constraint.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_trajectory_constraint.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_trajectory_constraints_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_trajectory_constraints_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_usertype_fluents_remover.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_usertype_fluents_remover.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/test/test_validator.py` & `unified_planning-0.6.0.9.dev1/unified_planning/test/test_validator.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning/utils.py` & `unified_planning-0.6.0.9.dev1/unified_planning/utils.py`

 * *Files identical despite different names*

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning.egg-info/PKG-INFO` & `unified_planning-0.6.0.9.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unified-planning
-Version: 0.6.0.33.dev1
+Name: unified_planning
+Version: 0.6.0.9.dev1
 Summary: Unified Planning Framework
 Home-page: https://www.aiplan4eu-project.eu
 Author: AIPlan4EU Project
 Author-email: aiplan4eu@fbk.eu
 License: APACHE
 Description: UNKNOWN
 Keywords: planning logic STRIPS RDDL
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning.egg-info/SOURCES.txt` & `unified_planning-0.6.0.9.dev1/unified_planning.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 unified_planning/io/__init__.py
 unified_planning/io/anml_grammar.py
 unified_planning/io/anml_reader.py
 unified_planning/io/anml_writer.py
 unified_planning/io/ma_pddl_writer.py
 unified_planning/io/pddl_reader.py
 unified_planning/io/pddl_writer.py
+unified_planning/io/python_writer.py
 unified_planning/io/utils.py
 unified_planning/model/__init__.py
 unified_planning/model/abstract_problem.py
 unified_planning/model/action.py
 unified_planning/model/contingent_problem.py
 unified_planning/model/delta_stn.py
 unified_planning/model/effect.py
@@ -162,14 +163,15 @@
 unified_planning/test/test_pddl_io.py
 unified_planning/test/test_pddl_planner.py
 unified_planning/test/test_plan_validator.py
 unified_planning/test/test_planner.py
 unified_planning/test/test_problem.py
 unified_planning/test/test_protobuf_io.py
 unified_planning/test/test_pyperplan.py
+unified_planning/test/test_python_writer.py
 unified_planning/test/test_quantifier_remover.py
 unified_planning/test/test_replanner.py
 unified_planning/test/test_scheduling.py
 unified_planning/test/test_sequential_simulator.py
 unified_planning/test/test_simplifier.py
 unified_planning/test/test_simulated_effects.py
 unified_planning/test/test_stn_plan.py
```

### Comparing `unified_planning-0.6.0.33.dev1/unified_planning.egg-info/requires.txt` & `unified_planning-0.6.0.9.dev1/unified_planning.egg-info/requires.txt`

 * *Files identical despite different names*

