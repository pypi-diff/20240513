# Comparing `tmp/brax-0.9.3.tar.gz` & `tmp/brax-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brax-0.9.3.tar", last modified: Thu Oct 19 22:08:12 2023, max compression
+gzip compressed data, was "brax-0.9.4.tar", last modified: Thu Jan  4 01:03:11 2024, max compression
```

## Comparing `brax-0.9.3.tar` & `brax-0.9.4.tar`

### file list

```diff
@@ -1,457 +1,463 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.572638 brax-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-10-19 22:08:00.000000 brax-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-19 22:08:00.000000 brax-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2023-10-19 22:08:12.572638 brax-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2023-10-19 22:08:00.000000 brax-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.508637 brax-0.9.3/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-19 22:08:00.000000 brax-0.9.3/bin/learn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.512637 brax-0.9.3/brax/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-19 22:08:00.000000 brax-0.9.3/brax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2023-10-19 22:08:00.000000 brax-0.9.3/brax/actuator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2023-10-19 22:08:00.000000 brax-0.9.3/brax/actuator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23466 2023-10-19 22:08:00.000000 brax-0.9.3/brax/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2023-10-19 22:08:00.000000 brax-0.9.3/brax/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2023-10-19 22:08:00.000000 brax-0.9.3/brax/com.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-10-19 22:08:00.000000 brax-0.9.3/brax/com_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.512637 brax-0.9.3/brax/envs/
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14342 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/ant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.520638 brax-0.9.3/brax/envs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/ant.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/half_cheetah.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/hopper.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/humanoid.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/humanoidstandup.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/inverted_double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/inverted_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/pusher.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/reacher.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/swimmer.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/assets/walker2d.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/env_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     9979 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/half_cheetah.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/hopper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23136 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/humanoid.py
--rw-r--r--   0 runner    (1001) docker     (127)    21219 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/humanoidstandup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/inverted_double_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/inverted_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    12192 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/pusher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/reacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/swimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12033 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/walker2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.520638 brax-0.9.3/brax/envs/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/wrappers/dm_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/wrappers/dm_env_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/wrappers/gym.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/wrappers/gym_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/wrappers/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/wrappers/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2023-10-19 22:08:00.000000 brax-0.9.3/brax/envs/wrappers/training_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.520638 brax-0.9.3/brax/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.520638 brax-0.9.3/brax/experimental/barkour_v0/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.528638 brax-0.9.3/brax/experimental/barkour_v0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   429334 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/abduction.stl
--rw-r--r--   0 runner    (1001) docker     (127)    14867 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/barkour_v0_brax.xml
--rw-r--r--   0 runner    (1001) docker     (127)  1169584 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/body.stl
--rw-r--r--   0 runner    (1001) docker     (127)    23384 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/foot.stl
--rw-r--r--   0 runner    (1001) docker     (127)   739084 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/handle.stl
--rw-r--r--   0 runner    (1001) docker     (127)   267584 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/head.stl
--rw-r--r--   0 runner    (1001) docker     (127)   163984 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/head_mount.stl
--rw-r--r--   0 runner    (1001) docker     (127)   523084 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/lower_leg_1to1.stl
--rw-r--r--   0 runner    (1001) docker     (127)  1199984 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/powercable.stl
--rw-r--r--   0 runner    (1001) docker     (127)   530834 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/upper_left_1.stl
--rw-r--r--   0 runner    (1001) docker     (127)   628484 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/upper_left_2.stl
--rw-r--r--   0 runner    (1001) docker     (127)  1500284 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/upper_left_3.stl
--rw-r--r--   0 runner    (1001) docker     (127)  1106034 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/upper_right_1.stl
--rw-r--r--   0 runner    (1001) docker     (127)   670284 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/upper_right_2.stl
--rw-r--r--   0 runner    (1001) docker     (127)  1521284 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/assets/upper_right_3.stl
--rw-r--r--   0 runner    (1001) docker     (127)    18410 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/barkour_joystick.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/barkour_joystick_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.532638 brax-0.9.3/brax/experimental/barkour_v0/data/
--rw-r--r--   0 runner    (1001) docker     (127)   443805 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/data/barkour_run_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   437193 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/data/barkour_run_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)   304497 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/data/barkour_run_2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    11046 2023-10-19 22:08:00.000000 brax-0.9.3/brax/experimental/barkour_v0/score_barkour.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2023-10-19 22:08:00.000000 brax-0.9.3/brax/fluid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2023-10-19 22:08:00.000000 brax-0.9.3/brax/fluid_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.532638 brax-0.9.3/brax/generalized/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/constraint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8125 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/dynamics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/integrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/mass_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/perf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-10-19 22:08:00.000000 brax-0.9.3/brax/generalized/pipeline_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.536638 brax-0.9.3/brax/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-10-19 22:08:00.000000 brax-0.9.3/brax/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21245 2023-10-19 22:08:00.000000 brax-0.9.3/brax/geometry/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)    18639 2023-10-19 22:08:00.000000 brax-0.9.3/brax/geometry/contact_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2023-10-19 22:08:00.000000 brax-0.9.3/brax/geometry/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    15084 2023-10-19 22:08:00.000000 brax-0.9.3/brax/geometry/math_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2023-10-19 22:08:00.000000 brax-0.9.3/brax/geometry/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-10-19 22:08:00.000000 brax-0.9.3/brax/geometry/mesh_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.536638 brax-0.9.3/brax/io/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/json_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    20445 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/mjcf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/mjcf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2023-10-19 22:08:00.000000 brax-0.9.3/brax/io/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12946 2023-10-19 22:08:00.000000 brax-0.9.3/brax/kinematics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2023-10-19 22:08:00.000000 brax-0.9.3/brax/kinematics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11915 2023-10-19 22:08:00.000000 brax-0.9.3/brax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-10-19 22:08:00.000000 brax-0.9.3/brax/math_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.536638 brax-0.9.3/brax/positional/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/collisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/integrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/joints_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/perf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2023-10-19 22:08:00.000000 brax-0.9.3/brax/positional/pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2023-10-19 22:08:00.000000 brax-0.9.3/brax/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2023-10-19 22:08:00.000000 brax-0.9.3/brax/scan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.540638 brax-0.9.3/brax/spring/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/collisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/integrator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/joints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/joints_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/perf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    10700 2023-10-19 22:08:00.000000 brax-0.9.3/brax/spring/pipeline_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.544638 brax-0.9.3/brax/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/capsule.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/colour_objects.xml
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/convex_convex.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/double_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/double_prismatic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/fat_cylinder.xml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/flat_cylinder.xml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/fluid_box.xml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/fluid_box_offset_com.xml
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/fluid_ellipsoid.xml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/fluid_sphere.xml
--rw-r--r--   0 runner    (1001) docker     (127)      859 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/fluid_two_spheres.xml
--rw-r--r--   0 runner    (1001) docker     (127)      519 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/fluid_wind.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.544638 brax-0.9.3/brax/test_data/laikago/
--rw-r--r--   0 runner    (1001) docker     (127)    16099 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/laikago_toes_zup.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    14646 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/laikago_viz.urdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.552638 brax-0.9.3/brax/test_data/laikago/meshes/
--rw-r--r--   0 runner    (1001) docker     (127)   711948 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/chassis.obj
--rw-r--r--   0 runner    (1001) docker     (127)   311084 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/chassis.stl
--rw-r--r--   0 runner    (1001) docker     (127)   169189 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/chassis_mod.obj
--rw-r--r--   0 runner    (1001) docker     (127)    23708 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/chassis_vhacd.obj
--rw-r--r--   0 runner    (1001) docker     (127)    32143 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/chassis_vhacd_mod.obj
--rw-r--r--   0 runner    (1001) docker     (127)    66809 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj
--rw-r--r--   0 runner    (1001) docker     (127)   746953 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/chassis_zup.obj
--rw-r--r--   0 runner    (1001) docker     (127)    72588 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/chassis_zup_lores.obj
--rw-r--r--   0 runner    (1001) docker     (127)    59569 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/hip_motor.obj
--rw-r--r--   0 runner    (1001) docker     (127)    40484 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/hip_motor.stl
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/hip_motor_lores.obj
--rw-r--r--   0 runner    (1001) docker     (127)    59686 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/hip_motor_mirror.obj
--rw-r--r--   0 runner    (1001) docker     (127)    40484 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/hip_motor_mirror.stl
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj
--rw-r--r--   0 runner    (1001) docker     (127)    12904 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_no_toes.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    15792 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    16088 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_limits.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    15992 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    18044 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    20646 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision_xyz_spherical.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    16183 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_joint_order.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    16070 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_lores.urdf
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_xyz_xyzrot.urdf
--rw-r--r--   0 runner    (1001) docker     (127)   330874 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/lower_leg3.obj
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/lower_leg3_lores.obj
--rw-r--r--   0 runner    (1001) docker     (127)   188884 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/lower_leg_3.stl
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/lower_leg_3_collision.stl
--rw-r--r--   0 runner    (1001) docker     (127)   112984 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg.stl
--rw-r--r--   0 runner    (1001) docker     (127)   210097 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left.obj
--rw-r--r--   0 runner    (1001) docker     (127)   210149 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left2.obj
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left2_lores.obj
--rw-r--r--   0 runner    (1001) docker     (127)    16386 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left_lores.obj
--rw-r--r--   0 runner    (1001) docker     (127)    17380 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left_vhacd.obj
--rw-r--r--   0 runner    (1001) docker     (127)   180144 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror.obj
--rw-r--r--   0 runner    (1001) docker     (127)   112984 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror.stl
--rw-r--r--   0 runner    (1001) docker     (127)   180145 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror2.obj
--rw-r--r--   0 runner    (1001) docker     (127)    14652 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror2_lores.obj
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror_lores.obj
--rw-r--r--   0 runner    (1001) docker     (127)   199652 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_right.obj
--rw-r--r--   0 runner    (1001) docker     (127)    17337 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_right_vhacd.obj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.552638 brax-0.9.3/brax/test_data/meshes/
--rw-r--r--   0 runner    (1001) docker     (127)    20884 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/meshes/cylinder.stl
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/meshes/dodecahedron.stl
--rw-r--r--   0 runner    (1001) docker     (127)      384 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/meshes/pyramid.stl
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/meshes/tetrahedron.stl
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/nonzero_joint_ref.xml
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/prismaversal_2dof_joint.xml
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/prismaversal_3dof_joint.xml
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_pendulum_motor.xml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_pendulum_position.xml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_pendulum_position_frclimit.xml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_pendulum_velocity.xml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_prismatic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      543 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_spherical_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_spherical_pendulum_motor.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_spherical_pendulum_position.xml
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/single_universal_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)      409 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/solver_params_v2.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/triple_pendulum.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/triple_pendulum_motor.xml
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/triple_prismatic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      842 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/world_body_transform.xml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/world_fromto.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_data/world_self_collision.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2023-10-19 22:08:00.000000 brax-0.9.3/brax/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.552638 brax-0.9.3/brax/training/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.552638 brax-0.9.3/brax/training/acme/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/acme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9571 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/acme/running_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/acme/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/acme/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/acting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.552638 brax-0.9.3/brax/training/agents/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.556638 brax-0.9.3/brax/training/agents/apg/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/apg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/apg/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/apg/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/apg/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.556638 brax-0.9.3/brax/training/agents/ars/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ars/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11563 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ars/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ars/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.556638 brax-0.9.3/brax/training/agents/es/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/es/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/es/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/es/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.556638 brax-0.9.3/brax/training/agents/ppo/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ppo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ppo/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ppo/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14691 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ppo/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/ppo/train_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.556638 brax-0.9.3/brax/training/agents/sac/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/sac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/sac/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/sac/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)    19191 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/sac/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/agents/sac/train_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5170 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/gradients.py
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/learner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6904 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/pmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    16797 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/replay_buffers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22646 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/replay_buffers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/spectral_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-10-19 22:08:00.000000 brax-0.9.3/brax/training/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.556638 brax-0.9.3/brax/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/envs/
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/acrobot.py
--rw-r--r--   0 runner    (1001) docker     (127)    26290 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/ant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)    17282 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    27963 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/grasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    24287 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/half_cheetah.py
--rw-r--r--   0 runner    (1001) docker     (127)    16976 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/hopper.py
--rw-r--r--   0 runner    (1001) docker     (127)    43652 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/humanoid.py
--rw-r--r--   0 runner    (1001) docker     (127)    45541 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/humanoid_standup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/inverted_double_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/inverted_pendulum.py
--rw-r--r--   0 runner    (1001) docker     (127)    20254 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/pusher.py
--rw-r--r--   0 runner    (1001) docker     (127)    14084 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/reacher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/reacherangle.py
--rw-r--r--   0 runner    (1001) docker     (127)    16065 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/swimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/to_torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14733 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/ur5e.py
--rw-r--r--   0 runner    (1001) docker     (127)    22667 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/walker2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/envs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/
--rw-r--r--   0 runner    (1001) docker     (127)    10567 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/registry/
--rw-r--r--   0 runner    (1001) docker     (127)      914 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/registry/ant/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/ant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/registry/ant/components/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/ant/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/ant/components/ant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/registry/jump/
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/jump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/registry/jump/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/jump/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/jump/envs/cheetah.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/registry/proant/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/proant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/registry/proant/components/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/proant/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/proant/components/ant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/biggym/registry/proant/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/proant/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/registry/proant/envs/ant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/biggym/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.560638 brax-0.9.3/brax/v1/experimental/braxlines/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.564638 brax-0.9.3/brax/v1/experimental/braxlines/common/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/common/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/common/dist_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/common/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     9959 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/common/logger_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/common/sim_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.564638 brax-0.9.3/brax/v1/experimental/braxlines/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/envs/obs_indices.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/envs/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.564638 brax-0.9.3/brax/v1/experimental/braxlines/experiments/
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/experiments/chase_ma_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/experiments/composer_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/experiments/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/experiments/dmin_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/experiments/mimax_sweep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/experiments/sumo_ma_sweep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.564638 brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6920 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    13557 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.564638 brax-0.9.3/brax/v1/experimental/braxlines/training/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/training/env.py
--rw-r--r--   0 runner    (1001) docker     (127)    20552 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/training/ppo.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/training/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.564638 brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11166 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/train.py
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.564638 brax-0.9.3/brax/v1/experimental/composer/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/agent_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/component_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.568638 brax-0.9.3/brax/v1/experimental/composer/components/
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/ant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/ground.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/halfcheetah.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/humanoid.py
--rw-r--r--   0 runner    (1001) docker     (127)    22588 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/octopus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/pro_ant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/components/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)    20635 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/composer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.568638 brax-0.9.3/brax/v1/experimental/composer/envs/
--rw-r--r--   0 runner    (1001) docker     (127)     3712 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/envs/ma_descs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/envs/sa_descs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/observers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/reward_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.568638 brax-0.9.3/brax/v1/experimental/composer/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/tests/composer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.568638 brax-0.9.3/brax/v1/experimental/composer/training/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23341 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/composer/training/mappo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.568638 brax-0.9.3/brax/v1/experimental/tracing/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/tracing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/tracing/customize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/tracing/randomizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/tracing/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/experimental/tracing/wrappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.568638 brax-0.9.3/brax/v1/io/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/npy_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/io/torch.py
--rw-r--r--   0 runner    (1001) docker     (127)    18655 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/jumpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6403 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.572638 brax-0.9.3/brax/v1/physics/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/actuators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/bodies.py
--rw-r--r--   0 runner    (1001) docker     (127)    40679 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/colliders.py
--rw-r--r--   0 runner    (1001) docker     (127)    17184 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/forces.py
--rw-r--r--   0 runner    (1001) docker     (127)    37491 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17079 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/joints.py
--rw-r--r--   0 runner    (1001) docker     (127)    13484 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/spring_joints.py
--rw-r--r--   0 runner    (1001) docker     (127)    15157 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/physics/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/pytree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.572638 brax-0.9.3/brax/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9982 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/colliders_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/env_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/geometry_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/grasp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/jumpy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/math_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23529 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/physics_legacy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29993 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/physics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/running_statistics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tests/urdf_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.572638 brax-0.9.3/brax/v1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20203 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tools/mujoco.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tools/mujoco_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tools/print_mesh_com.py
--rw-r--r--   0 runner    (1001) docker     (127)    10947 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tools/urdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2023-10-19 22:08:00.000000 brax-0.9.3/brax/v1/tools/urdf_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.572638 brax-0.9.3/brax/visualizer/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2023-10-19 22:08:00.000000 brax-0.9.3/brax/visualizer/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-10-19 22:08:00.000000 brax-0.9.3/brax/visualizer/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.572638 brax-0.9.3/brax/visualizer/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2023-10-19 22:08:00.000000 brax-0.9.3/brax/visualizer/js/animator.js
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2023-10-19 22:08:00.000000 brax-0.9.3/brax/visualizer/js/selector.js
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2023-10-19 22:08:00.000000 brax-0.9.3/brax/visualizer/js/system.js
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2023-10-19 22:08:00.000000 brax-0.9.3/brax/visualizer/js/viewer.js
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2023-10-19 22:08:00.000000 brax-0.9.3/brax/visualizer/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 22:08:12.512637 brax-0.9.3/brax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2023-10-19 22:08:12.000000 brax-0.9.3/brax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14333 2023-10-19 22:08:12.000000 brax-0.9.3/brax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 22:08:12.000000 brax-0.9.3/brax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-10-19 22:08:12.000000 brax-0.9.3/brax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-19 22:08:12.000000 brax-0.9.3/brax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-19 22:08:12.572638 brax-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2023-10-19 22:08:00.000000 brax-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.938777 brax-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-01-04 01:02:53.000000 brax-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-04 01:02:53.000000 brax-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-01-04 01:03:11.938777 brax-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-01-04 01:02:53.000000 brax-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.842777 brax-0.9.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-04 01:02:53.000000 brax-0.9.4/bin/learn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.846777 brax-0.9.4/brax/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-01-04 01:02:53.000000 brax-0.9.4/brax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-01-04 01:02:53.000000 brax-0.9.4/brax/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-01-04 01:02:53.000000 brax-0.9.4/brax/actuator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23978 2024-01-04 01:02:53.000000 brax-0.9.4/brax/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-01-04 01:02:53.000000 brax-0.9.4/brax/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-01-04 01:02:53.000000 brax-0.9.4/brax/com.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-01-04 01:02:53.000000 brax-0.9.4/brax/com_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.850777 brax-0.9.4/brax/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/ant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.854777 brax-0.9.4/brax/envs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/ant.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/half_cheetah.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/hopper.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/humanoid.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9495 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/humanoidstandup.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/inverted_double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/inverted_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/pusher.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/reacher.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/swimmer.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/assets/walker2d.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/env_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/half_cheetah.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/hopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/humanoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21219 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/humanoidstandup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/inverted_double_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/inverted_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12192 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/pusher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/reacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/swimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/walker2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.854777 brax-0.9.4/brax/envs/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/wrappers/dm_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/wrappers/dm_env_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/wrappers/gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/wrappers/gym_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/wrappers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/wrappers/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-01-04 01:02:53.000000 brax-0.9.4/brax/envs/wrappers/training_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.854777 brax-0.9.4/brax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.854777 brax-0.9.4/brax/experimental/barkour_v0/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.870777 brax-0.9.4/brax/experimental/barkour_v0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   429334 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/abduction.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    14867 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/barkour_v0_brax.xml
+-rw-r--r--   0 runner    (1001) docker     (127)  1169584 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/body.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    23384 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/foot.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   739084 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/handle.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   267584 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/head.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   163984 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/head_mount.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   523084 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/lower_leg_1to1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)  1199984 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/powercable.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   530834 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/upper_left_1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   628484 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/upper_left_2.stl
+-rw-r--r--   0 runner    (1001) docker     (127)  1500284 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/upper_left_3.stl
+-rw-r--r--   0 runner    (1001) docker     (127)  1106034 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/upper_right_1.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   670284 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/upper_right_2.stl
+-rw-r--r--   0 runner    (1001) docker     (127)  1521284 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/assets/upper_right_3.stl
+-rw-r--r--   0 runner    (1001) docker     (127)    18410 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/barkour_joystick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-01-04 01:02:53.000000 brax-0.9.4/brax/experimental/barkour_v0/barkour_joystick_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.874777 brax-0.9.4/brax/experimental/barkour_v0/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   443805 2024-01-04 01:02:54.000000 brax-0.9.4/brax/experimental/barkour_v0/data/barkour_run_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   437193 2024-01-04 01:02:54.000000 brax-0.9.4/brax/experimental/barkour_v0/data/barkour_run_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   304497 2024-01-04 01:02:54.000000 brax-0.9.4/brax/experimental/barkour_v0/data/barkour_run_2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11046 2024-01-04 01:02:54.000000 brax-0.9.4/brax/experimental/barkour_v0/score_barkour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-01-04 01:02:54.000000 brax-0.9.4/brax/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-01-04 01:02:54.000000 brax-0.9.4/brax/fluid_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.874777 brax-0.9.4/brax/generalized/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/constraint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/dynamics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/mass_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/perf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-01-04 01:02:54.000000 brax-0.9.4/brax/generalized/pipeline_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.878777 brax-0.9.4/brax/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-04 01:02:54.000000 brax-0.9.4/brax/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21245 2024-01-04 01:02:54.000000 brax-0.9.4/brax/geometry/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18639 2024-01-04 01:02:54.000000 brax-0.9.4/brax/geometry/contact_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-01-04 01:02:54.000000 brax-0.9.4/brax/geometry/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-01-04 01:02:54.000000 brax-0.9.4/brax/geometry/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-01-04 01:02:54.000000 brax-0.9.4/brax/geometry/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2024-01-04 01:02:54.000000 brax-0.9.4/brax/geometry/mesh_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.878777 brax-0.9.4/brax/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/json_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20465 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/mjcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/mjcf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-01-04 01:02:54.000000 brax-0.9.4/brax/io/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-01-04 01:02:54.000000 brax-0.9.4/brax/kinematics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-01-04 01:02:54.000000 brax-0.9.4/brax/kinematics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-01-04 01:02:54.000000 brax-0.9.4/brax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-01-04 01:02:54.000000 brax-0.9.4/brax/math_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.878777 brax-0.9.4/brax/mjx/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/mjx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-04 01:02:54.000000 brax-0.9.4/brax/mjx/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-01-04 01:02:54.000000 brax-0.9.4/brax/mjx/perf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-01-04 01:02:54.000000 brax-0.9.4/brax/mjx/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-01-04 01:02:54.000000 brax-0.9.4/brax/mjx/pipeline_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.882777 brax-0.9.4/brax/positional/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/joints_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/perf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-01-04 01:02:54.000000 brax-0.9.4/brax/positional/pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-01-04 01:02:54.000000 brax-0.9.4/brax/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-01-04 01:02:54.000000 brax-0.9.4/brax/scan_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.882777 brax-0.9.4/brax/spring/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/joints_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/perf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10700 2024-01-04 01:02:54.000000 brax-0.9.4/brax/spring/pipeline_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.886777 brax-0.9.4/brax/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/capsule.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/colour_objects.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/convex_convex.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/double_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/double_prismatic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/fat_cylinder.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/flat_cylinder.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/fluid_box.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/fluid_box_offset_com.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/fluid_ellipsoid.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/fluid_sphere.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/fluid_two_spheres.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/fluid_wind.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.890777 brax-0.9.4/brax/test_data/laikago/
+-rw-r--r--   0 runner    (1001) docker     (127)    16099 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/laikago_toes_zup.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    14646 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/laikago_viz.urdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.902777 brax-0.9.4/brax/test_data/laikago/meshes/
+-rw-r--r--   0 runner    (1001) docker     (127)   711948 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/chassis.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   311084 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/chassis.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   169189 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/chassis_mod.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    23708 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/chassis_vhacd.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/chassis_vhacd_mod.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    66809 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   746953 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/chassis_zup.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    72588 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/chassis_zup_lores.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    59569 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/hip_motor.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    40484 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/hip_motor.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/hip_motor_lores.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    59686 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/hip_motor_mirror.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    40484 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/hip_motor_mirror.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_no_toes.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15792 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    16088 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_limits.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    15992 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    18044 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    20646 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision_xyz_spherical.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    16183 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_joint_order.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    16070 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_lores.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_xyz_xyzrot.urdf
+-rw-r--r--   0 runner    (1001) docker     (127)   330874 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/lower_leg3.obj
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/lower_leg3_lores.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   188884 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/lower_leg_3.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/lower_leg_3_collision.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   112984 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   210097 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   210149 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left2.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left2_lores.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    16386 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left_lores.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    17380 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left_vhacd.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   180144 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   112984 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror.stl
+-rw-r--r--   0 runner    (1001) docker     (127)   180145 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror2.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror2_lores.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror_lores.obj
+-rw-r--r--   0 runner    (1001) docker     (127)   199652 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_right.obj
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_right_vhacd.obj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.902777 brax-0.9.4/brax/test_data/meshes/
+-rw-r--r--   0 runner    (1001) docker     (127)    20884 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/meshes/cylinder.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/meshes/dodecahedron.stl
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/meshes/pyramid.stl
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/meshes/tetrahedron.stl
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/nonzero_joint_ref.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/prismaversal_2dof_joint.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/prismaversal_3dof_joint.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_pendulum_motor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_pendulum_position.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_pendulum_position_frclimit.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_pendulum_velocity.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_prismatic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_spherical_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_spherical_pendulum_motor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_spherical_pendulum_position.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/single_universal_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/solver_params_v2.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/triple_pendulum.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/triple_pendulum_motor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/triple_prismatic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/world_body_transform.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/world_fromto.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_data/world_self_collision.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-01-04 01:02:54.000000 brax-0.9.4/brax/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.906777 brax-0.9.4/brax/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.906777 brax-0.9.4/brax/training/acme/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/acme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/acme/running_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/acme/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/acme/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/acting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.906777 brax-0.9.4/brax/training/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.906777 brax-0.9.4/brax/training/agents/apg/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/apg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/apg/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/apg/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/apg/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.906777 brax-0.9.4/brax/training/agents/ars/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ars/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11563 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ars/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ars/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.910777 brax-0.9.4/brax/training/agents/es/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/es/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/es/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/es/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.910777 brax-0.9.4/brax/training/agents/ppo/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ppo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ppo/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ppo/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17477 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ppo/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/ppo/train_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.910777 brax-0.9.4/brax/training/agents/sac/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/sac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/sac/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/sac/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19191 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/sac/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/agents/sac/train_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/gradients.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/learner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6904 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/pmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16797 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/replay_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22646 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/replay_buffers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/spectral_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-01-04 01:02:54.000000 brax-0.9.4/brax/training/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.910777 brax-0.9.4/brax/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.914777 brax-0.9.4/brax/v1/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/acrobot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26290 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/ant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17282 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27963 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/grasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24287 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/half_cheetah.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16976 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/hopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43652 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/humanoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45541 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/humanoid_standup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/inverted_double_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/inverted_pendulum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20254 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/pusher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/reacher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/reacherangle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16065 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/swimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/to_torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14733 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/ur5e.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22667 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/walker2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/envs/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.914777 brax-0.9.4/brax/v1/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.914777 brax-0.9.4/brax/v1/experimental/biggym/
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.914777 brax-0.9.4/brax/v1/experimental/biggym/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/biggym/registry/ant/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/ant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/biggym/registry/ant/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/ant/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/ant/components/ant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/biggym/registry/jump/
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/jump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/biggym/registry/jump/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/jump/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/jump/envs/cheetah.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/biggym/registry/proant/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/proant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/biggym/registry/proant/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/proant/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/proant/components/ant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/biggym/registry/proant/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/proant/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/registry/proant/envs/ant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/biggym/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/braxlines/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/braxlines/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/common/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/common/dist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/common/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9959 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/common/logger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/common/sim_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.918777 brax-0.9.4/brax/v1/experimental/braxlines/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/envs/obs_indices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/envs/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.922777 brax-0.9.4/brax/v1/experimental/braxlines/experiments/
+-rw-r--r--   0 runner    (1001) docker     (127)    14122 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/experiments/chase_ma_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/experiments/composer_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/experiments/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/experiments/dmin_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/experiments/mimax_sweep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/experiments/sumo_ma_sweep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.922777 brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6920 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13557 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.922777 brax-0.9.4/brax/v1/experimental/braxlines/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/training/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20552 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/training/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/training/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.922777 brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.922777 brax-0.9.4/brax/v1/experimental/composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/agent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/component_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.926777 brax-0.9.4/brax/v1/experimental/composer/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/ant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/ground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/halfcheetah.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/humanoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22588 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/octopus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/pro_ant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/components/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20635 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/composer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.926777 brax-0.9.4/brax/v1/experimental/composer/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/envs/ma_descs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/envs/sa_descs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/observers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/reward_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.926777 brax-0.9.4/brax/v1/experimental/composer/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/tests/composer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.926777 brax-0.9.4/brax/v1/experimental/composer/training/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23341 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/composer/training/mappo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.926777 brax-0.9.4/brax/v1/experimental/tracing/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/tracing/customize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/tracing/randomizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/tracing/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/experimental/tracing/wrappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.930777 brax-0.9.4/brax/v1/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/npy_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/io/torch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18655 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/jumpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.930777 brax-0.9.4/brax/v1/physics/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/actuators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/bodies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40679 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/colliders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17184 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37491 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17079 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13484 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/spring_joints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/physics/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/pytree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.934777 brax-0.9.4/brax/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9982 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/colliders_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/env_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/geometry_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/grasp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/jumpy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23529 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/physics_legacy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29993 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/physics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/running_statistics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tests/urdf_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.934777 brax-0.9.4/brax/v1/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20203 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tools/mujoco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tools/mujoco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tools/print_mesh_com.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10947 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tools/urdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-01-04 01:02:54.000000 brax-0.9.4/brax/v1/tools/urdf_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.934777 brax-0.9.4/brax/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-01-04 01:02:54.000000 brax-0.9.4/brax/visualizer/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-04 01:02:54.000000 brax-0.9.4/brax/visualizer/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.934777 brax-0.9.4/brax/visualizer/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-01-04 01:02:54.000000 brax-0.9.4/brax/visualizer/js/animator.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-01-04 01:02:54.000000 brax-0.9.4/brax/visualizer/js/selector.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-01-04 01:02:54.000000 brax-0.9.4/brax/visualizer/js/system.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-01-04 01:02:54.000000 brax-0.9.4/brax/visualizer/js/viewer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-01-04 01:02:54.000000 brax-0.9.4/brax/visualizer/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 01:03:11.934777 brax-0.9.4/brax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-01-04 01:03:11.000000 brax-0.9.4/brax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14440 2024-01-04 01:03:11.000000 brax-0.9.4/brax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 01:03:11.000000 brax-0.9.4/brax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-04 01:03:11.000000 brax-0.9.4/brax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-04 01:03:11.000000 brax-0.9.4/brax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-04 01:03:11.938777 brax-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-01-04 01:02:54.000000 brax-0.9.4/setup.py
```

### Comparing `brax-0.9.3/LICENSE` & `brax-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/PKG-INFO` & `brax-0.9.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: brax
-Version: 0.9.3
-Summary: A differentiable physics engine written in JAX.
-Home-page: http://github.com/google/brax
-Author: Brax Authors
-Author-email: no-reply@google.com
-License: Apache 2.0
-Keywords: JAX reinforcement learning rigidbody physics
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-Provides-Extra: develop
-License-File: LICENSE
-
 <img src="https://github.com/google/brax/raw/main/docs/img/brax_logo.gif" width="336" height="80" alt="BRAX"/>
 
 Brax is a fast and fully differentiable physics engine used for research and
 development of robotics, human perception, materials science, reinforcement
 learning, and other simulation-heavy applications.
 
 Brax is written in [JAX](https://github.com/google/jax) and is designed for use
@@ -36,21 +17,23 @@
 *   Baseline learning algorithms such as
     [PPO](https://github.com/google/brax/blob/main/brax/training/agents/ppo),
     [SAC](https://github.com/google/brax/blob/main/brax/training/agents/sac),
     [ARS](https://github.com/google/brax/blob/main/brax/training/agents/ars), and
     [evolutionary strategies](https://github.com/google/brax/blob/main/brax/training/agents/es).
 *   Learning algorithms that leverage the differentiability of the simulator, such as [analytic policy gradients](https://github.com/google/brax/blob/main/brax/training/agents/apg).
 
-## One API, Three Pipelines
+## One API, Four Pipelines
 
-Brax offers three distinct physics pipelines that are easy to swap:
+Brax offers four distinct physics pipelines that are easy to swap:
 
+* [MuJoCo XLA - MJX](https://mujoco.readthedocs.io/en/stable/mjx.html) - a JAX
+reimplementation of the MuJoCo physics engine.
 * [Generalized](https://github.com/google/brax/blob/main/brax/v2/generalized/)
-calculates motion in [generalized coordinates](https://en.wikipedia.org/wiki/Generalized_coordinates) using the same accurate robot
-dynamics algorithms as [MuJoCo](https://mujoco.org/) and [TDS](https://github.com/erwincoumans/tiny-differentiable-simulator).
+calculates motion in [generalized coordinates](https://en.wikipedia.org/wiki/Generalized_coordinates)
+using dynamics algorithms similar to [MuJoCo](https://mujoco.org/) and [TDS](https://github.com/erwincoumans/tiny-differentiable-simulator).
 * [Positional](https://github.com/google/brax/blob/main/brax/v2/positional/)
 uses [Position Based Dynamics](https://matthias-research.github.io/pages/publications/posBasedDyn.pdf),
 a fast but stable method of resolving joint and collision constraints.
 * [Spring](https://github.com/google/brax/blob/main/brax/v2/spring/) provides
 fast and cheap simulation for rapid experimentation, using simple impulse-based
 methods often found in video games.
 
@@ -60,14 +43,15 @@
 
 ## Quickstart: Colab in the Cloud
 
 Explore Brax easily and quickly through a series of colab notebooks:
 
 * [Brax Basics](https://colab.research.google.com/github/google/brax/blob/main/notebooks/basics.ipynb) introduces the Brax API, and shows how to simulate basic physics primitives.
 * [Brax Training](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training.ipynb) introduces Brax's training algorithms, and lets you train your own policies directly within the colab. It also demonstrates loading and saving policies.
+* [Brax Training with MuJoCo XLA - MJX](https://colab.sandbox.google.com/github/google-deepmind/mujoco/blob/main/mjx/tutorial.ipynb) demonstrates training in Brax using the `MJX` physics simulator.
 * [Brax Training with PyTorch on GPU](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training_torch.ipynb) demonstrates how Brax can be used in other ML frameworks for fast training, in this case PyTorch.
 
 ## Using Brax Locally
 
 To install Brax from pypi, install it with:
 
 ```
@@ -112,15 +96,15 @@
 If you would like to reference Brax in a publication, please use:
 
 ```
 @software{brax2021github,
   author = {C. Daniel Freeman and Erik Frey and Anton Raichuk and Sertan Girgin and Igor Mordatch and Olivier Bachem},
   title = {Brax - A Differentiable Physics Engine for Large Scale Rigid Body Simulation},
   url = {http://github.com/google/brax},
-  version = {0.9.3},
+  version = {0.9.4},
   year = {2021},
 }
 ```
 
 ## Acknowledgements
 
 Brax has come a long way since its original publication.  We offer gratitude and
```

### Comparing `brax-0.9.3/brax/__init__.py` & `brax-0.9.4/brax/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Import top-level classes and functions here for encapsulation/clarity."""
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
 
 from brax.base import Motion
 from brax.base import State
 from brax.base import System
 from brax.base import Transform
```

### Comparing `brax-0.9.3/brax/actuator.py` & `brax-0.9.4/brax/actuator.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/actuator_test.py` & `brax-0.9.4/brax/actuator_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/base.py` & `brax-0.9.4/brax/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 # limitations under the License.
 
 # pylint:disable=g-multiple-import, g-importing-member
 """Base brax primitives and simple manipulations of them."""
 
 import copy
 import functools
-from typing import Any, Dict, List, Optional, Sequence, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 
 from brax import math
 from flax import struct
 import jax
 from jax import numpy as jp
 from jax import vmap
 from jax.tree_util import tree_map
-
+import mujoco
+from mujoco import mjx
 
 # f: free, 1: 1-dof, 2: 2-dof, 3: 3-dof
 Q_WIDTHS = {'f': 7, '1': 1, '2': 2, '3': 3}
 QD_WIDTHS = {'f': 6, '1': 1, '2': 2, '3': 3}
 
 
 @struct.dataclass
@@ -613,14 +614,15 @@
   link_names: List[str] = struct.field(pytree_node=False)
   link_types: str = struct.field(pytree_node=False)
   link_parents: Tuple[int, ...] = struct.field(pytree_node=False)
   # only used in `brax.physics.generalized`:
   matrix_inv_iterations: int = struct.field(pytree_node=False)
   solver_iterations: int = struct.field(pytree_node=False)
   solver_maxls: int = struct.field(pytree_node=False)
+  _model: mujoco.MjModel = struct.field(pytree_node=False, default=None)
 
   def num_links(self) -> int:
     """Returns the number of links in the system."""
     return len(self.link_types)
 
   def dof_link(self, depth=False) -> jax.Array:
     """Returns the link index corresponding to each system dof."""
@@ -674,14 +676,26 @@
     """Returns the size of the qd vector (joint velocity) for this system."""
     return sum([QD_WIDTHS[t] for t in self.link_types])
 
   def act_size(self) -> int:
     """Returns the act dimension for the system."""
     return self.actuator.q_id.shape[0]
 
+  def set_model(self, model: mujoco.MjModel):
+    """Sets the source MuJoCo model of this System."""
+    object.__setattr__(self, '_model', model)
+
+  def get_model(self) -> mujoco.MjModel:
+    """Returns the source MuJoCo model of this System."""
+    return self._model
+
+  def get_mjx_model(self) -> mjx.Model:
+    """Returns an MJX model of this System."""
+    return mjx.put_model(getattr(self, '_model'))
+
 
 # below are some operation dispatch derivations
 
 
 @functools.singledispatch
 def _transform_do(other, self: Transform):
   del other, self
```

### Comparing `brax-0.9.3/brax/base_test.py` & `brax-0.9.4/brax/base_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/com.py` & `brax-0.9.4/brax/com.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/com_test.py` & `brax-0.9.4/brax/com_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/__init__.py` & `brax-0.9.4/brax/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/ant.py` & `brax-0.9.4/brax/envs/ant.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from brax import base
 from brax import math
 from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
+import mujoco
 
 
 class Ant(PipelineEnv):
 
 
 
   # pyformat: disable
@@ -162,14 +163,20 @@
 
     n_frames = 5
 
     if backend in ['spring', 'positional']:
       sys = sys.replace(dt=0.005)
       n_frames = 10
 
+    if backend == 'mjx':
+      sys._model.opt.solver = mujoco.mjtSolver.mjSOL_NEWTON
+      sys._model.opt.disableflags = mujoco.mjtDisableBit.mjDSBL_EULERDAMP
+      sys._model.opt.iterations = 1
+      sys._model.opt.ls_iterations = 4
+
     if backend == 'positional':
       # TODO: does the same actuator strength work as in spring
       sys = sys.replace(
           actuator=sys.actuator.replace(
               gear=200 * jp.ones_like(sys.actuator.gear)
           )
       )
@@ -226,18 +233,16 @@
     pipeline_state0 = state.pipeline_state
     pipeline_state = self.pipeline_step(pipeline_state0, action)
 
     velocity = (pipeline_state.x.pos[0] - pipeline_state0.x.pos[0]) / self.dt
     forward_reward = velocity[0]
 
     min_z, max_z = self._healthy_z_range
-    is_healthy = jp.where(pipeline_state.x.pos[0, 2] < min_z, x=0.0, y=1.0)
-    is_healthy = jp.where(
-        pipeline_state.x.pos[0, 2] > max_z, x=0.0, y=is_healthy
-    )
+    is_healthy = jp.where(pipeline_state.x.pos[0, 2] < min_z, 0.0, 1.0)
+    is_healthy = jp.where(pipeline_state.x.pos[0, 2] > max_z, 0.0, is_healthy)
     if self._terminate_when_unhealthy:
       healthy_reward = self._healthy_reward
     else:
       healthy_reward = self._healthy_reward * is_healthy
     ctrl_cost = self._ctrl_cost_weight * jp.sum(jp.square(action))
     contact_cost = 0.0
```

### Comparing `brax-0.9.3/brax/envs/assets/ant.xml` & `brax-0.9.4/brax/envs/assets/ant.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/half_cheetah.xml` & `brax-0.9.4/brax/envs/assets/half_cheetah.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/hopper.xml` & `brax-0.9.4/brax/envs/assets/hopper.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/humanoid.xml` & `brax-0.9.4/brax/envs/assets/humanoid.xml`

 * *Files 0% similar despite different names*

#### Comparing `brax-0.9.3/brax/envs/assets/humanoid.xml` & `brax-0.9.4/brax/envs/assets/humanoid.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <mujoco model="humanoid">
   <compiler angle="degree" inertiafromgeom="true"/>
   <default>
     <joint armature="1" damping="1" limited="true"/>
-    <geom conaffinity="0" condim="1" contype="0" material="geom"/>
+    <geom conaffinity="0" condim="3" contype="0" material="geom"/>
     <motor ctrllimited="true" ctrlrange="-.4 .4"/>
   </default>
   <!-- Removed RK4 integrator for brax. -->
   <option iterations="8" timestep="0.003"/>
   <custom>
     <!-- brax custom params -->
     <numeric data="2500" name="constraint_limit_stiffness"/>
```

### Comparing `brax-0.9.3/brax/envs/assets/humanoidstandup.xml` & `brax-0.9.4/brax/envs/assets/humanoidstandup.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/inverted_double_pendulum.xml` & `brax-0.9.4/brax/envs/assets/inverted_double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/inverted_pendulum.xml` & `brax-0.9.4/brax/envs/assets/inverted_pendulum.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/pusher.xml` & `brax-0.9.4/brax/envs/assets/pusher.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/reacher.xml` & `brax-0.9.4/brax/envs/assets/reacher.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/swimmer.xml` & `brax-0.9.4/brax/envs/assets/swimmer.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/assets/walker2d.xml` & `brax-0.9.4/brax/envs/assets/walker2d.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/base.py` & `brax-0.9.4/brax/envs/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,23 +12,26 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # pylint:disable=g-multiple-import
 """A brax environment for training and inference."""
 
 import abc
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional, Sequence, Union
 
 from brax import base
 from brax.generalized import pipeline as g_pipeline
+from brax.mjx import pipeline as m_pipeline
 from brax.positional import pipeline as p_pipeline
 from brax.spring import pipeline as s_pipeline
 from flax import struct
 import jax
-from jax import numpy as jp
+import mujoco
+from mujoco import mjx
+import numpy as np
 
 
 @struct.dataclass
 class State(base.Base):
   """Environment state for training and inference."""
 
   pipeline_state: Optional[base.State]
@@ -140,14 +143,84 @@
     return self.sys.act_size()
 
   @property
   def backend(self) -> str:
     return self._backend
 
 
+class MjxEnv(Env):
+  """API for driving a MuJoCo model for training and inference."""
+
+  def __init__(
+      self,
+      model: mujoco.MjModel,
+      n_frames: int = 1,
+      debug: bool = False,
+  ):
+    """Initializes PipelineEnv.
+
+    Args:
+      model: an mjx.Model
+      n_frames: the number of times to step the physics pipeline for each
+        environment step
+      debug: whether to get debug info from the pipeline init/step (ignored)
+    """
+    # HACK: sys here is improperly typed, some code expects sys to be a System
+    self._model = model
+    self.sys = mjx.put_model(model)
+    self._n_frames = n_frames
+    self._debug = debug
+
+  def pipeline_init(self, q: jax.Array, qd: jax.Array) -> base.State:
+    """Initializes the pipeline state."""
+    return m_pipeline.init(self.sys, q, qd, self._debug)
+
+  def pipeline_step(self, pipeline_state: Any, action: jax.Array) -> base.State:
+    """Takes a physics step using the physics pipeline."""
+
+    def f(state, _):
+      return m_pipeline.step(self.sys, state, action, self._debug), None
+
+    return jax.lax.scan(f, pipeline_state, (), self._n_frames)[0]
+
+  @property
+  def dt(self) -> jax.Array:
+    """The timestep used for each env step."""
+    return self.sys.opt.timestep * self._n_frames
+
+  @property
+  def observation_size(self) -> int:
+    rng = jax.random.PRNGKey(0)
+    reset_state = self.unwrapped.reset(rng)
+    return reset_state.obs.shape[-1]
+
+  @property
+  def action_size(self) -> int:
+    return self.sys.nu
+
+  @property
+  def backend(self) -> str:
+    return 'mjx'
+
+  def render(
+      self, trajectory: List[base.State], camera: Union[str, None] = None
+  ) -> Sequence[np.ndarray]:
+    """Renders a trajectory using the MuJoCo renderer."""
+    renderer = mujoco.Renderer(self._model)
+    camera = camera or -1
+
+    def get_image(state: mjx.Data):
+      d = mjx.get_data(self._model, state)
+      mujoco.mj_forward(self._model, d)
+      renderer.update_scene(d, camera=camera)
+      return renderer.render()
+
+    return [get_image(s.data) for s in trajectory]  # pytype: disable=attribute-error
+
+
 class Wrapper(Env):
   """Wraps an environment to allow modular transformations."""
 
   def __init__(self, env: Env):
     self.env = env
 
   def reset(self, rng: jax.Array) -> State:
```

### Comparing `brax-0.9.3/brax/envs/env_test.py` & `brax-0.9.4/brax/envs/env_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/fast.py` & `brax-0.9.4/brax/envs/fast.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/half_cheetah.py` & `brax-0.9.4/brax/envs/half_cheetah.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/hopper.py` & `brax-0.9.4/brax/envs/hopper.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/humanoid.py` & `brax-0.9.4/brax/envs/humanoid.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from brax import actuator
 from brax import base
 from brax.envs.base import PipelineEnv, State
 from brax.io import mjcf
 from etils import epath
 import jax
 from jax import numpy as jp
+import mujoco
 
 
 class Humanoid(PipelineEnv):
 
 
 
   # pyformat: disable
@@ -197,14 +198,20 @@
       sys = sys.replace(dt=0.0015)
       n_frames = 10
       gear = jp.array([
           350.0, 350.0, 350.0, 350.0, 350.0, 350.0, 350.0, 350.0, 350.0, 350.0,
           350.0, 100.0, 100.0, 100.0, 100.0, 100.0, 100.0])  # pyformat: disable
       sys = sys.replace(actuator=sys.actuator.replace(gear=gear))
 
+    if backend == 'mjx':
+      sys._model.opt.solver = mujoco.mjtSolver.mjSOL_NEWTON
+      sys._model.opt.disableflags = mujoco.mjtDisableBit.mjDSBL_EULERDAMP
+      sys._model.opt.iterations = 1
+      sys._model.opt.ls_iterations = 4
+
     kwargs['n_frames'] = kwargs.get('n_frames', n_frames)
 
     super().__init__(sys=sys, backend=backend, **kwargs)
 
     self._forward_reward_weight = forward_reward_weight
     self._ctrl_cost_weight = ctrl_cost_weight
     self._healthy_reward = healthy_reward
@@ -251,18 +258,16 @@
 
     com_before, *_ = self._com(pipeline_state0)
     com_after, *_ = self._com(pipeline_state)
     velocity = (com_after - com_before) / self.dt
     forward_reward = self._forward_reward_weight * velocity[0]
 
     min_z, max_z = self._healthy_z_range
-    is_healthy = jp.where(pipeline_state.x.pos[0, 2] < min_z, x=0.0, y=1.0)
-    is_healthy = jp.where(
-        pipeline_state.x.pos[0, 2] > max_z, x=0.0, y=is_healthy
-    )
+    is_healthy = jp.where(pipeline_state.x.pos[0, 2] < min_z, 0.0, 1.0)
+    is_healthy = jp.where(pipeline_state.x.pos[0, 2] > max_z, 0.0, is_healthy)
     if self._terminate_when_unhealthy:
       healthy_reward = self._healthy_reward
     else:
       healthy_reward = self._healthy_reward * is_healthy
 
     ctrl_cost = self._ctrl_cost_weight * jp.sum(jp.square(action))
```

### Comparing `brax-0.9.3/brax/envs/humanoidstandup.py` & `brax-0.9.4/brax/envs/humanoidstandup.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/inverted_double_pendulum.py` & `brax-0.9.4/brax/envs/inverted_double_pendulum.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/inverted_pendulum.py` & `brax-0.9.4/brax/envs/inverted_pendulum.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/pusher.py` & `brax-0.9.4/brax/envs/pusher.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/reacher.py` & `brax-0.9.4/brax/envs/reacher.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/swimmer.py` & `brax-0.9.4/brax/envs/swimmer.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/walker2d.py` & `brax-0.9.4/brax/envs/walker2d.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/wrappers/__init__.py` & `brax-0.9.4/brax/envs/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/wrappers/dm_env.py` & `brax-0.9.4/brax/envs/wrappers/dm_env.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/wrappers/dm_env_test.py` & `brax-0.9.4/brax/envs/wrappers/dm_env_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/wrappers/gym.py` & `brax-0.9.4/brax/envs/wrappers/gym.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/wrappers/gym_test.py` & `brax-0.9.4/brax/envs/wrappers/gym_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/wrappers/torch.py` & `brax-0.9.4/brax/envs/wrappers/torch.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/wrappers/training.py` & `brax-0.9.4/brax/envs/wrappers/training.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/envs/wrappers/training_test.py` & `brax-0.9.4/brax/envs/wrappers/training_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/__init__.py` & `brax-0.9.4/brax/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/__init__.py` & `brax-0.9.4/brax/experimental/barkour_v0/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/abduction.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/abduction.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/barkour_v0_brax.xml` & `brax-0.9.4/brax/experimental/barkour_v0/assets/barkour_v0_brax.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/body.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/body.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/foot.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/foot.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/handle.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/handle.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/head.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/head.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/head_mount.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/head_mount.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/lower_leg_1to1.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/lower_leg_1to1.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/powercable.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/powercable.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/upper_left_1.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/upper_left_1.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/upper_left_2.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/upper_left_2.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/upper_left_3.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/upper_left_3.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/upper_right_1.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/upper_right_1.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/upper_right_2.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/upper_right_2.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/assets/upper_right_3.stl` & `brax-0.9.4/brax/experimental/barkour_v0/assets/upper_right_3.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/barkour_joystick.py` & `brax-0.9.4/brax/experimental/barkour_v0/barkour_joystick.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/barkour_joystick_test.py` & `brax-0.9.4/brax/experimental/barkour_v0/barkour_joystick_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/data/barkour_run_0.csv` & `brax-0.9.4/brax/experimental/barkour_v0/data/barkour_run_0.csv`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/data/barkour_run_1.csv` & `brax-0.9.4/brax/experimental/barkour_v0/data/barkour_run_1.csv`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/data/barkour_run_2.csv` & `brax-0.9.4/brax/experimental/barkour_v0/data/barkour_run_2.csv`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/experimental/barkour_v0/score_barkour.py` & `brax-0.9.4/brax/experimental/barkour_v0/score_barkour.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/fluid.py` & `brax-0.9.4/brax/fluid.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/fluid_test.py` & `brax-0.9.4/brax/fluid_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/__init__.py` & `brax-0.9.4/brax/generalized/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/base.py` & `brax-0.9.4/brax/generalized/base.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/constraint.py` & `brax-0.9.4/brax/generalized/constraint.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/constraint_test.py` & `brax-0.9.4/brax/generalized/constraint_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/dynamics.py` & `brax-0.9.4/brax/generalized/dynamics.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/dynamics_test.py` & `brax-0.9.4/brax/generalized/dynamics_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/integrator.py` & `brax-0.9.4/brax/generalized/integrator.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/mass.py` & `brax-0.9.4/brax/generalized/mass.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/mass_test.py` & `brax-0.9.4/brax/generalized/mass_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/perf_test.py` & `brax-0.9.4/brax/generalized/perf_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/pipeline.py` & `brax-0.9.4/brax/generalized/pipeline.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/generalized/pipeline_test.py` & `brax-0.9.4/brax/generalized/pipeline_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # pylint:disable=g-multiple-import
 """Tests for generalized pipeline."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from brax import test_utils
 from brax.generalized import pipeline
+from brax.io import mjcf
 import jax
 from jax import numpy as jp
 import numpy as np
 
 
 class PipelineTest(parameterized.TestCase):
 
@@ -42,9 +43,41 @@
       state = jax.jit(pipeline.init)(sys, mj_prev.qpos, mj_prev.qvel)
       state = jax.jit(pipeline.step)(sys, state, jp.zeros(sys.act_size()))
 
       np.testing.assert_allclose(state.q, mj_next.qpos, atol=0.002)
       np.testing.assert_allclose(state.qd, mj_next.qvel, atol=0.5)
 
 
+class GradientTest(absltest.TestCase):
+  """Tests that gradients are not NaN."""
+
+  def test_grad(self):
+    """Tests that gradients are not NaN."""
+    xml = """
+    <mujoco>
+      <worldbody>
+        <body>
+          <joint type="slide" axis="1 0 0" damping="1"/>
+          <joint type="slide" axis="0 1 0" damping="1"/>
+          <geom size="0.1" mass="1"/>
+        </body>
+      </worldbody>
+    </mujoco>
+    """
+    sys = mjcf.loads(xml)
+    init_state = jax.jit(pipeline.init)(
+        sys, sys.init_q, jp.zeros(sys.qd_size())
+    )
+
+    def fn(xd):
+      qd = jp.zeros(sys.qd_size()).at[0].set(xd)
+      state = init_state.replace(qd=qd)
+      for _ in range(10):
+        state = jax.jit(pipeline.step)(sys, state, None)
+      return state.qd[0]
+
+    grad = jax.grad(fn)(-1.0)
+    self.assertFalse(np.isnan(grad))
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `brax-0.9.3/brax/geometry/__init__.py` & `brax-0.9.4/brax/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/geometry/contact.py` & `brax-0.9.4/brax/geometry/contact.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/geometry/contact_test.py` & `brax-0.9.4/brax/geometry/contact_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/geometry/math.py` & `brax-0.9.4/brax/geometry/math.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/geometry/math_test.py` & `brax-0.9.4/brax/geometry/math_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/geometry/mesh.py` & `brax-0.9.4/brax/geometry/mesh.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/geometry/mesh_test.py` & `brax-0.9.4/brax/geometry/mesh_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/__init__.py` & `brax-0.9.4/brax/io/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/html.py` & `brax-0.9.4/brax/io/html.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/image.py` & `brax-0.9.4/brax/io/image.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/image_test.py` & `brax-0.9.4/brax/io/image_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/json.py` & `brax-0.9.4/brax/io/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 import jax
 import jax.numpy as jp
 import numpy as np
 
 # State attributes needed for the visualizer.
 _STATE_ATTR = ['x', 'contact']
 
+_IGNORE_FIELDS = ['_model', '_mjx_model']
+
 
 def _to_dict(obj):
   """Converts python object to a json encodeable object."""
   if isinstance(obj, list) or isinstance(obj, tuple):
     return [_to_dict(s) for s in obj]
   if isinstance(obj, dict):
-    return {k: _to_dict(v) for k, v in obj.items()}
+    return {k: _to_dict(v) for k, v in obj.items() if k not in _IGNORE_FIELDS}
   if isinstance(obj, jax.Array):
     return _to_dict(obj.tolist())
   if hasattr(obj, '__dict__'):
     d = dict(obj.__dict__)
     d['name'] = obj.__class__.__name__
     return _to_dict(d)
   if isinstance(obj, np.ndarray):
```

### Comparing `brax-0.9.3/brax/io/json_test.py` & `brax-0.9.4/brax/io/json_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/metrics.py` & `brax-0.9.4/brax/io/metrics.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/mjcf.py` & `brax-0.9.4/brax/io/mjcf.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,14 +493,15 @@
       link_parents=link_parents,
       matrix_inv_iterations=int(custom['matrix_inv_iterations']),
       solver_iterations=mj.opt.iterations,
       solver_maxls=int(custom['solver_maxls']),
   )
 
   sys = jax.tree_map(jp.array, sys)
+  sys.set_model(mj)
 
   return sys
 
 
 def fuse_bodies(xml: str):
   """Fuses together parent child bodies that have no joint."""
   xml = ElementTree.fromstring(xml)
```

### Comparing `brax-0.9.3/brax/io/mjcf_test.py` & `brax-0.9.4/brax/io/mjcf_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/model.py` & `brax-0.9.4/brax/io/model.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/io/torch.py` & `brax-0.9.4/brax/io/torch.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/kinematics.py` & `brax-0.9.4/brax/kinematics.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/kinematics_test.py` & `brax-0.9.4/brax/kinematics_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/math.py` & `brax-0.9.4/brax/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,21 +299,21 @@
     A^-1 inverted matrix
   """
 
   def body_fn(carry, _):
     a_inv, r, err = carry
     a_inv_next = a_inv @ (np.eye(a.shape[0]) + r)
     r_next = np.eye(a.shape[0]) - a @ a_inv_next
-    err_next = jp.linalg.norm(r_next)
+    err_next = safe_norm(r_next)
     a_inv_next = jp.where(err_next < err, a_inv_next, a_inv)
     return (a_inv_next, r_next, err_next), None
 
   # ensure ||I - X0 @ A|| < 1, in order to guarantee convergence
   r0 = jp.eye(a.shape[0]) - a @ a_inv
-  a_inv = jp.where(jp.linalg.norm(r0) > 1, 0.5 * a.T / jp.trace(a @ a.T), a_inv)
+  a_inv = jp.where(safe_norm(r0) > 1, 0.5 * a.T / jp.trace(a @ a.T), a_inv)
   (a_inv, _, _), _ = jax.lax.scan(body_fn, (a_inv, r0, 1.0), None, num_iter)
 
   return a_inv
 
 
 def safe_norm(
     x: jax.Array, axis: Optional[Union[Tuple[int, ...], int]] = None
@@ -328,17 +328,17 @@
 
   Returns:
     Norm of the array x.
   """
 
   is_zero = jp.allclose(x, 0.0)
   # temporarily swap x with ones if is_zero, then swap back
-  x = jp.where(is_zero, jp.ones_like(x), x)
-  n = jp.linalg.norm(x, axis=axis)
-  n = jp.where(is_zero, 0.0, n)
+  x = x + is_zero * 1.0
+  n = jp.linalg.norm(x) * (1.0 - is_zero)
+
   return n
 
 
 def normalize(
     x: jax.Array, axis: Optional[Union[Tuple[int, ...], int]] = None
 ) -> Tuple[jax.Array, jax.Array]:
   """Normalizes an array.
```

### Comparing `brax-0.9.3/brax/math_test.py` & `brax-0.9.4/brax/math_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/__init__.py` & `brax-0.9.4/brax/mjx/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/base.py` & `brax-0.9.4/brax/positional/base.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/collisions.py` & `brax-0.9.4/brax/positional/collisions.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/integrator.py` & `brax-0.9.4/brax/positional/integrator.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/joints.py` & `brax-0.9.4/brax/positional/joints.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/joints_test.py` & `brax-0.9.4/brax/positional/joints_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/perf_test.py` & `brax-0.9.4/brax/positional/perf_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/pipeline.py` & `brax-0.9.4/brax/positional/pipeline.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/positional/pipeline_test.py` & `brax-0.9.4/brax/positional/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/scan.py` & `brax-0.9.4/brax/scan.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/scan_test.py` & `brax-0.9.4/brax/scan_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/__init__.py` & `brax-0.9.4/brax/positional/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/base.py` & `brax-0.9.4/brax/spring/base.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/collisions.py` & `brax-0.9.4/brax/spring/collisions.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/integrator.py` & `brax-0.9.4/brax/spring/integrator.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/joints.py` & `brax-0.9.4/brax/spring/joints.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/joints_test.py` & `brax-0.9.4/brax/spring/joints_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/perf_test.py` & `brax-0.9.4/brax/spring/perf_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/pipeline.py` & `brax-0.9.4/brax/spring/pipeline.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/spring/pipeline_test.py` & `brax-0.9.4/brax/spring/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/capsule.xml` & `brax-0.9.4/brax/test_data/capsule.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/colour_objects.xml` & `brax-0.9.4/brax/test_data/colour_objects.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/convex_convex.xml` & `brax-0.9.4/brax/test_data/convex_convex.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/double_pendulum.xml` & `brax-0.9.4/brax/test_data/double_pendulum.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/double_prismatic.xml` & `brax-0.9.4/brax/test_data/double_prismatic.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/fluid_box_offset_com.xml` & `brax-0.9.4/brax/test_data/fluid_box_offset_com.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/fluid_ellipsoid.xml` & `brax-0.9.4/brax/test_data/fluid_ellipsoid.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/fluid_sphere.xml` & `brax-0.9.4/brax/test_data/fluid_sphere.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/fluid_two_spheres.xml` & `brax-0.9.4/brax/test_data/fluid_two_spheres.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/fluid_wind.xml` & `brax-0.9.4/brax/test_data/fluid_wind.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/laikago_toes_zup.urdf` & `brax-0.9.4/brax/test_data/laikago/laikago_toes_zup.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/laikago_viz.urdf` & `brax-0.9.4/brax/test_data/laikago/laikago_viz.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/chassis.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/chassis.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/chassis.stl` & `brax-0.9.4/brax/test_data/laikago/meshes/chassis.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/chassis_mod.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/chassis_mod.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/chassis_vhacd.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/chassis_vhacd.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/chassis_vhacd_mod.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/chassis_vhacd_mod.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/chassis_vhacd_mod_zup.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/chassis_zup.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/chassis_zup.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/chassis_zup_lores.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/chassis_zup_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/hip_motor.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/hip_motor.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/hip_motor.stl` & `brax-0.9.4/brax/test_data/laikago/meshes/hip_motor.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/hip_motor_lores.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/hip_motor_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/hip_motor_mirror.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/hip_motor_mirror.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/hip_motor_mirror.stl` & `brax-0.9.4/brax/test_data/laikago/meshes/hip_motor_mirror.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/hip_motor_mirror_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_no_toes.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_no_toes.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_limits.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_limits.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision_xyz_spherical.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_chassis_collision_xyz_spherical.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_joint_order.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_joint_order.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_lores.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_lores.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/laikago_toes_zup_xyz_xyzrot.urdf` & `brax-0.9.4/brax/test_data/laikago/meshes/laikago_toes_zup_xyz_xyzrot.urdf`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/lower_leg3.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/lower_leg3.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/lower_leg3_lores.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/lower_leg3_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/lower_leg_3.stl` & `brax-0.9.4/brax/test_data/laikago/meshes/lower_leg_3.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/lower_leg_3_collision.stl` & `brax-0.9.4/brax/test_data/laikago/meshes/lower_leg_3_collision.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg.stl` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left2.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left2.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left2_lores.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left2_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left_lores.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_left_vhacd.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_left_vhacd.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror.stl` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror2.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror2.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror2_lores.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror2_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_mirror_lores.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_mirror_lores.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_right.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_right.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/laikago/meshes/upper_leg_right_vhacd.obj` & `brax-0.9.4/brax/test_data/laikago/meshes/upper_leg_right_vhacd.obj`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/meshes/cylinder.stl` & `brax-0.9.4/brax/test_data/meshes/cylinder.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/meshes/dodecahedron.stl` & `brax-0.9.4/brax/test_data/meshes/dodecahedron.stl`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/nonzero_joint_ref.xml` & `brax-0.9.4/brax/test_data/nonzero_joint_ref.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/prismaversal_2dof_joint.xml` & `brax-0.9.4/brax/test_data/prismaversal_2dof_joint.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/prismaversal_3dof_joint.xml` & `brax-0.9.4/brax/test_data/prismaversal_3dof_joint.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/single_pendulum_motor.xml` & `brax-0.9.4/brax/test_data/single_pendulum_motor.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/single_pendulum_position.xml` & `brax-0.9.4/brax/test_data/single_pendulum_position.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/single_pendulum_position_frclimit.xml` & `brax-0.9.4/brax/test_data/single_pendulum_position_frclimit.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/single_pendulum_velocity.xml` & `brax-0.9.4/brax/test_data/single_pendulum_velocity.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/single_spherical_pendulum.xml` & `brax-0.9.4/brax/test_data/single_spherical_pendulum.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/single_spherical_pendulum_motor.xml` & `brax-0.9.4/brax/test_data/single_spherical_pendulum_motor.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/single_spherical_pendulum_position.xml` & `brax-0.9.4/brax/test_data/single_spherical_pendulum_position.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/triple_pendulum.xml` & `brax-0.9.4/brax/test_data/triple_pendulum.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/triple_pendulum_motor.xml` & `brax-0.9.4/brax/test_data/triple_pendulum_motor.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/triple_prismatic.xml` & `brax-0.9.4/brax/test_data/triple_prismatic.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/world_body_transform.xml` & `brax-0.9.4/brax/test_data/world_body_transform.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/world_fromto.xml` & `brax-0.9.4/brax/test_data/world_fromto.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_data/world_self_collision.xml` & `brax-0.9.4/brax/test_data/world_self_collision.xml`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/test_utils.py` & `brax-0.9.4/brax/test_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/__init__.py` & `brax-0.9.4/brax/spring/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/acme/__init__.py` & `brax-0.9.4/brax/training/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/acme/running_statistics.py` & `brax-0.9.4/brax/training/acme/running_statistics.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/acme/specs.py` & `brax-0.9.4/brax/training/acme/specs.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/acme/types.py` & `brax-0.9.4/brax/training/acme/types.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/acting.py` & `brax-0.9.4/brax/training/acting.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/__init__.py` & `brax-0.9.4/brax/training/acme/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/apg/__init__.py` & `brax-0.9.4/brax/training/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/apg/networks.py` & `brax-0.9.4/brax/training/agents/apg/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/apg/train.py` & `brax-0.9.4/brax/training/agents/apg/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/apg/train_test.py` & `brax-0.9.4/brax/training/agents/apg/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/ars/__init__.py` & `brax-0.9.4/brax/training/agents/apg/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/ars/networks.py` & `brax-0.9.4/brax/training/agents/ars/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/ars/train.py` & `brax-0.9.4/brax/training/agents/ars/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/ars/train_test.py` & `brax-0.9.4/brax/training/agents/ars/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/es/__init__.py` & `brax-0.9.4/brax/training/agents/ars/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/es/networks.py` & `brax-0.9.4/brax/training/agents/es/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/es/train.py` & `brax-0.9.4/brax/training/agents/es/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/es/train_test.py` & `brax-0.9.4/brax/training/agents/es/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/ppo/__init__.py` & `brax-0.9.4/brax/training/agents/es/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/ppo/losses.py` & `brax-0.9.4/brax/training/agents/ppo/losses.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/ppo/networks.py` & `brax-0.9.4/brax/training/agents/ppo/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/ppo/train.py` & `brax-0.9.4/brax/training/agents/ppo/train.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Proximal policy optimization training.
 
 See: https://arxiv.org/pdf/1707.06347.pdf
 """
 
 import functools
 import time
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from typing import Callable, Optional, Tuple, Union
 
 from absl import logging
 from brax import base
 from brax import envs
 from brax.training import acting
 from brax.training import gradients
 from brax.training import pmap
@@ -100,15 +100,65 @@
     normalize_advantage: bool = True,
     eval_env: Optional[envs.Env] = None,
     policy_params_fn: Callable[..., None] = lambda *args: None,
     randomization_fn: Optional[
         Callable[[base.System, jnp.ndarray], Tuple[base.System, base.System]]
     ] = None,
 ):
-  """PPO training."""
+  """PPO training.
+
+  Args:
+    environment: the environment to train
+    num_timesteps: the total number of environment steps to use during training
+    episode_length: the length of an environment episode
+    action_repeat: the number of timesteps to repeat an action
+    num_envs: the number of parallel environments to use for rollouts
+      NOTE: `num_envs` must be divisible by the total number of chips since each
+        chip gets `num_envs // total_number_of_chips` environments to roll out
+      NOTE: `batch_size * num_minibatches` must be divisible by `num_envs` since
+        data generated by `num_envs` parallel envs gets used for gradient
+        updates over `num_minibatches` of data, where each minibatch has a
+        leading dimension of `batch_size`
+    max_devices_per_host: maximum number of chips to use per host process
+    num_eval_envs: the number of envs to use for evluation. Each env will run 1
+      episode, and all envs run in parallel during eval.
+    learning_rate: learning rate for ppo loss
+    entropy_cost: entropy reward for ppo loss, higher values increase entropy
+      of the policy
+    discounting: discounting rate
+    seed: random seed
+    unroll_length: the number of timesteps to unroll in each environment. The
+      PPO loss is computed over `unroll_length` timesteps
+    batch_size: the batch size for each minibatch SGD step
+    num_minibatches: the number of times to run the SGD step, each with a
+      different minibatch with leading dimension of `batch_size`
+    num_updates_per_batch: the number of times to run the gradient update over
+      all minibatches before doing a new environment rollout
+    num_evals: the number of evals to run during the entire training run.
+      Increasing the number of evals increases total training time
+    num_resets_per_eval: the number of environment resets to run between each
+      eval. The environment resets occur on the host
+    normalize_observations: whether to normalize observations
+    reward_scaling: float scaling for reward
+    clipping_epsilon: clipping epsilon for PPO loss
+    gae_lambda: General advantage estimation lambda
+    deterministic_eval: whether to run the eval with a deterministic policy
+    network_factory: function that generates networks for policy and value
+      functions
+    progress_fn: a user-defined callback function for reporting/plotting metrics
+    normalize_advantage: whether to normalize advantage estimate
+    eval_env: an optional environment for eval only, defaults to `environment`
+    policy_params_fn: a user-defined callback function that can be used for
+      saving policy checkpoints
+    randomization_fn: a user-defined callback function that generates randomized
+      environments
+
+  Returns:
+    Tuple of (make_policy function, network params, metrics)
+  """
   assert batch_size * num_minibatches % num_envs == 0
   xt = time.time()
 
   process_count = jax.process_count()
   process_id = jax.process_index()
   local_device_count = jax.local_device_count()
   local_devices_to_use = local_device_count
```

### Comparing `brax-0.9.3/brax/training/agents/ppo/train_test.py` & `brax-0.9.4/brax/training/agents/ppo/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/sac/__init__.py` & `brax-0.9.4/brax/training/agents/ppo/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/sac/losses.py` & `brax-0.9.4/brax/training/agents/sac/losses.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/sac/networks.py` & `brax-0.9.4/brax/training/agents/sac/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/sac/train.py` & `brax-0.9.4/brax/training/agents/sac/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/agents/sac/train_test.py` & `brax-0.9.4/brax/training/agents/sac/train_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/distribution.py` & `brax-0.9.4/brax/training/distribution.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/gradients.py` & `brax-0.9.4/brax/training/gradients.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/learner.py` & `brax-0.9.4/brax/training/learner.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/networks.py` & `brax-0.9.4/brax/training/networks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/pmap.py` & `brax-0.9.4/brax/training/pmap.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/replay_buffers.py` & `brax-0.9.4/brax/training/replay_buffers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/replay_buffers_test.py` & `brax-0.9.4/brax/training/replay_buffers_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/spectral_norm.py` & `brax-0.9.4/brax/training/spectral_norm.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/training/types.py` & `brax-0.9.4/brax/training/types.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/__init__.py` & `brax-0.9.4/brax/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/__init__.py` & `brax-0.9.4/brax/v1/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/acrobot.py` & `brax-0.9.4/brax/v1/envs/acrobot.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/ant.py` & `brax-0.9.4/brax/v1/envs/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/env.py` & `brax-0.9.4/brax/v1/envs/env.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/fast.py` & `brax-0.9.4/brax/v1/envs/fast.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/fetch.py` & `brax-0.9.4/brax/v1/envs/fetch.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/grasp.py` & `brax-0.9.4/brax/v1/envs/grasp.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/half_cheetah.py` & `brax-0.9.4/brax/v1/envs/half_cheetah.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/hopper.py` & `brax-0.9.4/brax/v1/envs/hopper.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/humanoid.py` & `brax-0.9.4/brax/v1/envs/humanoid.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/humanoid_standup.py` & `brax-0.9.4/brax/v1/envs/humanoid_standup.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/inverted_double_pendulum.py` & `brax-0.9.4/brax/v1/envs/inverted_double_pendulum.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/inverted_pendulum.py` & `brax-0.9.4/brax/v1/envs/inverted_pendulum.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/pusher.py` & `brax-0.9.4/brax/v1/envs/pusher.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/reacher.py` & `brax-0.9.4/brax/v1/envs/reacher.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/reacherangle.py` & `brax-0.9.4/brax/v1/envs/reacherangle.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/swimmer.py` & `brax-0.9.4/brax/v1/envs/swimmer.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/to_torch.py` & `brax-0.9.4/brax/v1/envs/to_torch.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/ur5e.py` & `brax-0.9.4/brax/v1/envs/ur5e.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/walker2d.py` & `brax-0.9.4/brax/v1/envs/walker2d.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/envs/wrappers.py` & `brax-0.9.4/brax/v1/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/__init__.py` & `brax-0.9.4/brax/training/agents/sac/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/ant/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/ant/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/ant/components/__init__.py` & `brax-0.9.4/brax/v1/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/ant/components/ant.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/ant/components/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/jump/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/jump/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/jump/envs/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/ant/components/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/jump/envs/cheetah.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/jump/envs/cheetah.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/proant/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/proant/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/proant/components/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/jump/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/proant/components/ant.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/proant/components/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/proant/envs/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/proant/components/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/registry/proant/envs/ant.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/proant/envs/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/biggym/tasks.py` & `brax-0.9.4/brax/v1/experimental/biggym/tasks.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/__init__.py` & `brax-0.9.4/brax/v1/experimental/biggym/registry/proant/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/common/__init__.py` & `brax-0.9.4/brax/v1/experimental/braxlines/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/common/config_utils.py` & `brax-0.9.4/brax/v1/experimental/braxlines/common/config_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/common/dist_utils.py` & `brax-0.9.4/brax/v1/experimental/braxlines/common/dist_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/common/evaluators.py` & `brax-0.9.4/brax/v1/experimental/braxlines/common/evaluators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/common/logger_utils.py` & `brax-0.9.4/brax/v1/experimental/braxlines/common/logger_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/common/sim_utils.py` & `brax-0.9.4/brax/v1/experimental/braxlines/common/sim_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/envs/__init__.py` & `brax-0.9.4/brax/v1/experimental/braxlines/common/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/envs/obs_indices.py` & `brax-0.9.4/brax/v1/experimental/braxlines/envs/obs_indices.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/envs/wrappers.py` & `brax-0.9.4/brax/v1/experimental/braxlines/envs/wrappers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/experiments/__init__.py` & `brax-0.9.4/brax/v1/experimental/braxlines/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/experiments/chase_ma_sweep.py` & `brax-0.9.4/brax/v1/experimental/braxlines/experiments/chase_ma_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/experiments/composer_sweep.py` & `brax-0.9.4/brax/v1/experimental/braxlines/experiments/composer_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/experiments/defaults.py` & `brax-0.9.4/brax/v1/experimental/braxlines/experiments/defaults.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/experiments/dmin_sweep.py` & `brax-0.9.4/brax/v1/experimental/braxlines/experiments/dmin_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/experiments/mimax_sweep.py` & `brax-0.9.4/brax/v1/experimental/braxlines/experiments/mimax_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/experiments/sumo_ma_sweep.py` & `brax-0.9.4/brax/v1/experimental/braxlines/experiments/sumo_ma_sweep.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/__init__.py` & `brax-0.9.4/brax/v1/experimental/braxlines/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/evaluators.py` & `brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/evaluators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/train.py` & `brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/irl_smm/utils.py` & `brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/training/__init__.py` & `brax-0.9.4/brax/v1/experimental/braxlines/irl_smm/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/training/env.py` & `brax-0.9.4/brax/v1/experimental/braxlines/training/env.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/training/ppo.py` & `brax-0.9.4/brax/v1/experimental/braxlines/training/ppo.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/training/utils.py` & `brax-0.9.4/brax/v1/experimental/braxlines/training/utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/__init__.py` & `brax-0.9.4/brax/v1/experimental/braxlines/training/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/evaluators.py` & `brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/evaluators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/train.py` & `brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/braxlines/vgcrl/utils.py` & `brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/__init__.py` & `brax-0.9.4/brax/v1/experimental/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/agent_utils.py` & `brax-0.9.4/brax/v1/experimental/composer/agent_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/component_editor.py` & `brax-0.9.4/brax/v1/experimental/composer/component_editor.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/__init__.py` & `brax-0.9.4/brax/v1/experimental/composer/components/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/ant.py` & `brax-0.9.4/brax/v1/experimental/composer/components/ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/common.py` & `brax-0.9.4/brax/v1/experimental/composer/components/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   del info
   # upright termination
   index = sim_utils.names2indices(sys.config, component['root'], 'body')[0][0]
   rot = qp.rot[index]
   up = jnp.array([0., 0., 1.])
   torso_up = math.rotate(up, rot)
   torso_is_up = jnp.dot(torso_up, up)
-  done = jnp.where(torso_is_up < 0.0, x=1.0, y=done)
+  done = jnp.where(torso_is_up < 0.0, 1.0, done)
   return done
 
 
 def height_term_fn(done,
                    sys,
                    qp: brax.QP,
                    info: brax.Info,
@@ -41,10 +41,10 @@
                    min_height: float = 0.2):
   """Terminate when it flips or jumps too high."""
   del info
   # height termination
   z_offset = component.get('term_params', {}).get('z_offset', 0.0)
   index = sim_utils.names2indices(sys.config, component['root'], 'body')[0][0]
   z = qp.pos[index][2]
-  done = jnp.where(z < min_height + z_offset, x=1.0, y=done)
-  done = jnp.where(z > max_height + z_offset, x=1.0, y=done)
+  done = jnp.where(z < min_height + z_offset, 1.0, done)
+  done = jnp.where(z > max_height + z_offset, 1.0, done)
   return done
```

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/ground.py` & `brax-0.9.4/brax/v1/experimental/composer/components/ground.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/halfcheetah.py` & `brax-0.9.4/brax/v1/experimental/composer/components/halfcheetah.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/humanoid.py` & `brax-0.9.4/brax/v1/experimental/composer/components/humanoid.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/octopus.py` & `brax-0.9.4/brax/v1/experimental/composer/components/octopus.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/pro_ant.py` & `brax-0.9.4/brax/v1/experimental/composer/components/pro_ant.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/components/singleton.py` & `brax-0.9.4/brax/v1/experimental/composer/components/singleton.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/composer.py` & `brax-0.9.4/brax/v1/experimental/composer/composer.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/composer_utils.py` & `brax-0.9.4/brax/v1/experimental/composer/composer_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/data_utils.py` & `brax-0.9.4/brax/v1/experimental/composer/data_utils.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/envs/__init__.py` & `brax-0.9.4/brax/v1/experimental/composer/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/envs/ma_descs.py` & `brax-0.9.4/brax/v1/experimental/composer/envs/ma_descs.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/envs/sa_descs.py` & `brax-0.9.4/brax/v1/experimental/composer/envs/sa_descs.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/observers.py` & `brax-0.9.4/brax/v1/experimental/composer/observers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/reward_functions.py` & `brax-0.9.4/brax/v1/experimental/composer/reward_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     reward, done = reward_fn(*args, **kwargs)
     if exclude_from_score:
       score = jnp.zeros_like(reward)
     else:
       score = reward
     reward = (reward + offset) * scale
     score *= jnp.sign(scale)
-    reward = jnp.where(done, x=reward + done_bonus, y=reward)
-    score = jnp.where(done, x=score + done_bonus, y=score)
+    reward = jnp.where(done, reward + done_bonus, reward)
+    score = jnp.where(done, score + done_bonus, score)
     return reward, score, done
 
   return fn
 
 
 def index_obs_dict(obs_dict: Dict[str, jnp.ndarray], obs: Union[Observer,
                                                                 jnp.ndarray]):
@@ -164,16 +164,16 @@
   obs1 = obs1.reshape((1,) * (ndim - obs1.ndim) + obs1.shape)
   obs2 = obs2.reshape((1,) * (ndim - obs2.ndim) + obs2.shape)
   delta = obs1 - obs2
   dist = jnp.linalg.norm(delta, axis=-1, **norm_kwargs)
   # instead of clipping, terminate
   # dist = jnp.clip(dist, a_min=min_dist, a_max=max_dist)
   done = jnp.zeros_like(dist)
-  done = jnp.where(dist < min_dist, x=jnp.ones_like(done), y=done)
-  done = jnp.where(dist > max_dist, x=jnp.ones_like(done), y=done)
+  done = jnp.where(dist < min_dist, jnp.ones_like(done), done)
+  done = jnp.where(dist > max_dist, jnp.ones_like(done), done)
   return -dist, done
 
 
 def get_reward_fns(*components: Dict[str, Any],
                    reward_type: str = 'root_goal',
                    **reward_kwargs):
   """Get components-based reward functions.
```

### Comparing `brax-0.9.3/brax/v1/experimental/composer/tests/__init__.py` & `brax-0.9.4/brax/v1/experimental/braxlines/vgcrl/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/tests/composer_test.py` & `brax-0.9.4/brax/v1/experimental/composer/tests/composer_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/train.py` & `brax-0.9.4/brax/v1/experimental/composer/train.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/training/__init__.py` & `brax-0.9.4/brax/v1/experimental/composer/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/composer/training/mappo.py` & `brax-0.9.4/brax/v1/experimental/composer/training/mappo.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/normalization.py` & `brax-0.9.4/brax/v1/experimental/normalization.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/tracing/__init__.py` & `brax-0.9.4/brax/v1/experimental/composer/training/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/tracing/customize.py` & `brax-0.9.4/brax/v1/experimental/tracing/customize.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/tracing/randomizers.py` & `brax-0.9.4/brax/v1/experimental/tracing/randomizers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/tracing/wrappers.py` & `brax-0.9.4/brax/v1/experimental/tracing/wrappers.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/experimental/tracing/wrappers_test.py` & `brax-0.9.4/brax/v1/experimental/tracing/wrappers_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/__init__.py` & `brax-0.9.4/brax/v1/experimental/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/export.py` & `brax-0.9.4/brax/v1/io/export.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/file.py` & `brax-0.9.4/brax/v1/io/file.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/html.py` & `brax-0.9.4/brax/v1/io/html.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/image.py` & `brax-0.9.4/brax/v1/io/image.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/json.py` & `brax-0.9.4/brax/v1/io/json.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/mesh.py` & `brax-0.9.4/brax/v1/io/mesh.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/metrics.py` & `brax-0.9.4/brax/v1/io/metrics.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/model.py` & `brax-0.9.4/brax/v1/io/model.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/npy_file.py` & `brax-0.9.4/brax/v1/io/npy_file.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/io/torch.py` & `brax-0.9.4/brax/v1/io/torch.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/jumpy.py` & `brax-0.9.4/brax/v1/jumpy.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/math.py` & `brax-0.9.4/brax/v1/math.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/__init__.py` & `brax-0.9.4/brax/v1/io/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/actuators.py` & `brax-0.9.4/brax/v1/physics/actuators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/base.py` & `brax-0.9.4/brax/v1/physics/base.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/bodies.py` & `brax-0.9.4/brax/v1/physics/bodies.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/colliders.py` & `brax-0.9.4/brax/v1/physics/colliders.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/config_pb2.py` & `brax-0.9.4/brax/v1/physics/config_pb2.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/forces.py` & `brax-0.9.4/brax/v1/physics/forces.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/geometry.py` & `brax-0.9.4/brax/v1/physics/geometry.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/integrators.py` & `brax-0.9.4/brax/v1/physics/integrators.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/joints.py` & `brax-0.9.4/brax/v1/physics/joints.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/spring_joints.py` & `brax-0.9.4/brax/v1/physics/spring_joints.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/physics/system.py` & `brax-0.9.4/brax/v1/physics/system.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/pytree.py` & `brax-0.9.4/brax/v1/pytree.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/__init__.py` & `brax-0.9.4/brax/v1/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/colliders_test.py` & `brax-0.9.4/brax/v1/tests/colliders_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/env_test.py` & `brax-0.9.4/brax/v1/tests/env_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/geometry_test.py` & `brax-0.9.4/brax/v1/tests/geometry_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/grasp_test.py` & `brax-0.9.4/brax/v1/tests/grasp_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/jumpy_test.py` & `brax-0.9.4/brax/v1/tests/jumpy_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/math_test.py` & `brax-0.9.4/brax/v1/tests/math_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/physics_legacy_test.py` & `brax-0.9.4/brax/v1/tests/physics_legacy_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/physics_test.py` & `brax-0.9.4/brax/v1/tests/physics_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/running_statistics_test.py` & `brax-0.9.4/brax/v1/tests/running_statistics_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tests/urdf_test.py` & `brax-0.9.4/brax/v1/tests/urdf_test.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tools/__init__.py` & `brax-0.9.4/brax/v1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tools/mujoco.py` & `brax-0.9.4/brax/v1/tools/mujoco.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tools/mujoco_converter.py` & `brax-0.9.4/brax/v1/tools/mujoco_converter.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tools/print_mesh_com.py` & `brax-0.9.4/brax/v1/tools/print_mesh_com.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tools/urdf.py` & `brax-0.9.4/brax/v1/tools/urdf.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/v1/tools/urdf_converter.py` & `brax-0.9.4/brax/v1/tools/urdf_converter.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/visualizer/favicon.ico` & `brax-0.9.4/brax/visualizer/favicon.ico`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/visualizer/index.html` & `brax-0.9.4/brax/visualizer/index.html`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/visualizer/js/animator.js` & `brax-0.9.4/brax/visualizer/js/animator.js`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/visualizer/js/selector.js` & `brax-0.9.4/brax/visualizer/js/selector.js`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/visualizer/js/system.js` & `brax-0.9.4/brax/visualizer/js/system.js`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/visualizer/js/viewer.js` & `brax-0.9.4/brax/visualizer/js/viewer.js`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax/visualizer/visualizer.py` & `brax-0.9.4/brax/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `brax-0.9.3/brax.egg-info/PKG-INFO` & `brax-0.9.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,51 @@
 Metadata-Version: 2.1
 Name: brax
-Version: 0.9.3
+Version: 0.9.4
 Summary: A differentiable physics engine written in JAX.
 Home-page: http://github.com/google/brax
 Author: Brax Authors
 Author-email: no-reply@google.com
 License: Apache 2.0
 Keywords: JAX reinforcement learning rigidbody physics
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
-Provides-Extra: develop
 License-File: LICENSE
+Requires-Dist: absl-py
+Requires-Dist: dataclasses; python_version < "3.7"
+Requires-Dist: dm_env
+Requires-Dist: etils
+Requires-Dist: flask
+Requires-Dist: flask_cors
+Requires-Dist: flax
+Requires-Dist: grpcio
+Requires-Dist: gym
+Requires-Dist: jax>=0.4.6
+Requires-Dist: jaxlib>=0.4.6
+Requires-Dist: jaxopt
+Requires-Dist: jinja2
+Requires-Dist: ml_collections
+Requires-Dist: mujoco
+Requires-Dist: mujoco-mjx
+Requires-Dist: numpy
+Requires-Dist: optax
+Requires-Dist: Pillow
+Requires-Dist: pytinyrenderer
+Requires-Dist: scipy
+Requires-Dist: tensorboardX
+Requires-Dist: trimesh
+Requires-Dist: typing-extensions
+Provides-Extra: develop
+Requires-Dist: pytest; extra == "develop"
+Requires-Dist: transforms3d; extra == "develop"
 
 <img src="https://github.com/google/brax/raw/main/docs/img/brax_logo.gif" width="336" height="80" alt="BRAX"/>
 
 Brax is a fast and fully differentiable physics engine used for research and
 development of robotics, human perception, materials science, reinforcement
 learning, and other simulation-heavy applications.
 
@@ -36,21 +62,23 @@
 *   Baseline learning algorithms such as
     [PPO](https://github.com/google/brax/blob/main/brax/training/agents/ppo),
     [SAC](https://github.com/google/brax/blob/main/brax/training/agents/sac),
     [ARS](https://github.com/google/brax/blob/main/brax/training/agents/ars), and
     [evolutionary strategies](https://github.com/google/brax/blob/main/brax/training/agents/es).
 *   Learning algorithms that leverage the differentiability of the simulator, such as [analytic policy gradients](https://github.com/google/brax/blob/main/brax/training/agents/apg).
 
-## One API, Three Pipelines
+## One API, Four Pipelines
 
-Brax offers three distinct physics pipelines that are easy to swap:
+Brax offers four distinct physics pipelines that are easy to swap:
 
+* [MuJoCo XLA - MJX](https://mujoco.readthedocs.io/en/stable/mjx.html) - a JAX
+reimplementation of the MuJoCo physics engine.
 * [Generalized](https://github.com/google/brax/blob/main/brax/v2/generalized/)
-calculates motion in [generalized coordinates](https://en.wikipedia.org/wiki/Generalized_coordinates) using the same accurate robot
-dynamics algorithms as [MuJoCo](https://mujoco.org/) and [TDS](https://github.com/erwincoumans/tiny-differentiable-simulator).
+calculates motion in [generalized coordinates](https://en.wikipedia.org/wiki/Generalized_coordinates)
+using dynamics algorithms similar to [MuJoCo](https://mujoco.org/) and [TDS](https://github.com/erwincoumans/tiny-differentiable-simulator).
 * [Positional](https://github.com/google/brax/blob/main/brax/v2/positional/)
 uses [Position Based Dynamics](https://matthias-research.github.io/pages/publications/posBasedDyn.pdf),
 a fast but stable method of resolving joint and collision constraints.
 * [Spring](https://github.com/google/brax/blob/main/brax/v2/spring/) provides
 fast and cheap simulation for rapid experimentation, using simple impulse-based
 methods often found in video games.
 
@@ -60,14 +88,15 @@
 
 ## Quickstart: Colab in the Cloud
 
 Explore Brax easily and quickly through a series of colab notebooks:
 
 * [Brax Basics](https://colab.research.google.com/github/google/brax/blob/main/notebooks/basics.ipynb) introduces the Brax API, and shows how to simulate basic physics primitives.
 * [Brax Training](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training.ipynb) introduces Brax's training algorithms, and lets you train your own policies directly within the colab. It also demonstrates loading and saving policies.
+* [Brax Training with MuJoCo XLA - MJX](https://colab.sandbox.google.com/github/google-deepmind/mujoco/blob/main/mjx/tutorial.ipynb) demonstrates training in Brax using the `MJX` physics simulator.
 * [Brax Training with PyTorch on GPU](https://colab.research.google.com/github/google/brax/blob/main/notebooks/training_torch.ipynb) demonstrates how Brax can be used in other ML frameworks for fast training, in this case PyTorch.
 
 ## Using Brax Locally
 
 To install Brax from pypi, install it with:
 
 ```
@@ -112,15 +141,15 @@
 If you would like to reference Brax in a publication, please use:
 
 ```
 @software{brax2021github,
   author = {C. Daniel Freeman and Erik Frey and Anton Raichuk and Sertan Girgin and Igor Mordatch and Olivier Bachem},
   title = {Brax - A Differentiable Physics Engine for Large Scale Rigid Body Simulation},
   url = {http://github.com/google/brax},
-  version = {0.9.3},
+  version = {0.9.4},
   year = {2021},
 }
 ```
 
 ## Acknowledgements
 
 Brax has come a long way since its original publication.  We offer gratitude and
```

### Comparing `brax-0.9.3/brax.egg-info/SOURCES.txt` & `brax-0.9.4/brax.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,19 @@
 brax/io/json.py
 brax/io/json_test.py
 brax/io/metrics.py
 brax/io/mjcf.py
 brax/io/mjcf_test.py
 brax/io/model.py
 brax/io/torch.py
+brax/mjx/__init__.py
+brax/mjx/base.py
+brax/mjx/perf_test.py
+brax/mjx/pipeline.py
+brax/mjx/pipeline_test.py
 brax/positional/__init__.py
 brax/positional/base.py
 brax/positional/collisions.py
 brax/positional/integrator.py
 brax/positional/joints.py
 brax/positional/joints_test.py
 brax/positional/perf_test.py
```

### Comparing `brax-0.9.3/setup.py` & `brax-0.9.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 """
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="brax",
-    version="0.9.3",
+    version="0.9.4",
     description=("A differentiable physics engine written in JAX."),
     author="Brax Authors",
     author_email="no-reply@google.com",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/google/brax",
     license="Apache 2.0",
@@ -49,14 +49,15 @@
         "gym",
         "jax>=0.4.6",
         "jaxlib>=0.4.6",
         "jaxopt",
         "jinja2",
         "ml_collections",
         "mujoco",
+        "mujoco-mjx",
         "numpy",
         "optax",
         "Pillow",
         "pytinyrenderer",
         "scipy",
         "tensorboardX",
         "trimesh",
```

