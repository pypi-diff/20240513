# Comparing `tmp/grasp_planning-0.4.2.tar.gz` & `tmp/grasp_planning-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.4.2.tar", last modified: Wed May  8 08:46:34 2024, max compression
+gzip compressed data, was "grasp_planning-0.5.0.tar", max compression
```

## Comparing `grasp_planning-0.4.2.tar` & `grasp_planning-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      267 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/PKG-INFO
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      123 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/__init__.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning/constraints/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2024-05-03 09:25:11.000000 grasp_planning-0.4.2/grasp_planning/constraints/collision_constraint.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      271 2024-05-07 16:07:10.000000 grasp_planning-0.4.2/grasp_planning/constraints/constraint_template.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      252 2024-05-08 08:42:32.000000 grasp_planning-0.4.2/grasp_planning/constraints/constraints.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1434 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/constraints/grasp_pos_constraint.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     3156 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/constraints/grasp_rot_constraint.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1037 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/constraints/manipulation_constraint.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning/cost/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       65 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/cost/costs.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        0 2024-05-02 12:00:02.000000 grasp_planning-0.4.2/grasp_planning/cost/dist_to_home.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1439 2024-04-18 15:29:48.000000 grasp_planning-0.4.2/grasp_planning/cost/squared_acc_cost.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning/solver/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     5714 2024-05-07 16:34:01.000000 grasp_planning-0.4.2/grasp_planning/solver/gomp_planner.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1736 2024-05-08 08:42:59.000000 grasp_planning-0.4.2/grasp_planning/solver/robot_model.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/grasp_planning.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      267 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      718 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      100 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2024-05-08 08:46:34.000000 grasp_planning-0.4.2/grasp_planning.egg-info/top_level.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      428 2024-05-08 08:41:47.000000 grasp_planning-0.4.2/pyproject.toml
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2024-05-08 08:46:34.181957 grasp_planning-0.4.2/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      714 2024-05-08 08:46:09.000000 grasp_planning-0.4.2/setup.py
+-rw-r--r--   0        0        0     1676 2024-05-13 14:58:14.750519 grasp_planning-0.5.0/README.md
+-rw-r--r--   0        0        0      123 2024-05-07 16:34:01.834623 grasp_planning-0.5.0/grasp_planning/__init__.py
+-rw-r--r--   0        0        0     1335 2024-05-13 14:27:59.161140 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0      799 2024-05-13 12:55:10.134092 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc
+-rw-r--r--   0        0        0      411 2024-05-08 08:43:17.328729 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/constraints.cpython-38.pyc
+-rw-r--r--   0        0        0     1331 2024-05-13 12:55:10.134092 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0     1528 2024-05-13 13:10:01.879282 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0     1557 2024-05-09 15:57:33.554280 grasp_planning-0.5.0/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc
+-rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884832 grasp_planning-0.5.0/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.0/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      252 2024-05-08 08:42:32.500427 grasp_planning-0.5.0/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452309 grasp_planning-0.5.0/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.0/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.0/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0      219 2024-05-07 16:34:48.974947 grasp_planning-0.5.0/grasp_planning/cost/__pycache__/costs.cpython-38.pyc
+-rw-r--r--   0        0        0     1344 2024-05-13 08:32:20.007123 grasp_planning-0.5.0/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc
+-rw-r--r--   0        0        0       65 2024-05-07 16:34:01.834623 grasp_planning-0.5.0/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0        0 2024-05-02 12:00:02.772313 grasp_planning-0.5.0/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.0/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     5689 2024-05-13 14:30:35.090364 grasp_planning-0.5.0/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc
+-rw-r--r--   0        0        0     2203 2024-05-13 13:26:57.783698 grasp_planning-0.5.0/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc
+-rw-r--r--   0        0        0     7077 2024-05-13 14:30:31.766338 grasp_planning-0.5.0/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     1875 2024-05-13 13:26:55.591679 grasp_planning-0.5.0/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      450 2024-05-13 14:54:58.605033 grasp_planning-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 grasp_planning-0.5.0/PKG-INFO
```

### Comparing `grasp_planning-0.4.2/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.0/grasp_planning/constraints/manipulation_constraint.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 import numpy as np
 import casadi as ca
 import spatial_casadi as sc
 from grasp_planning.constraints.constraint_template import Constraint
 
-class GraspPosConstraint(Constraint):
-    def __init__(self, robot, q_ca, waypoint_ID, n_dofs, tolerance=0.0) -> None:
+
+class ManipulationConstraint(Constraint):
+    def __init__(self, robot, q_ca, waypoint_ID, n_dofs) -> None:
         super().__init__() 
         # q = q_ca[:n_dof, waypoint_ID] -> joint space of the robot (decision variable)
         # manip_frame = q_ca[n_dof:, waypoint_ID] -> manipulation frame (decision variable)
-        # manip frame_pos - T_W_Grasp_pos = 0
+        # FK(q)_rpy - manip frame = 0
         self._robot = robot
-        self.g = q_ca[n_dofs:(n_dofs+3), waypoint_ID]
-        self.g_eval = ca.Function('g_grasp_pos', [q_ca], [self.g])
-        self.tolerance = tolerance
-        # self.update_limits(T_W_Grasp)
-      
-    def get_constraint(self):
-        return self.g
+        
+        self.g = self._robot.compute_fk_rpy_ca(q_ca[:n_dofs, waypoint_ID]) - q_ca[n_dofs:, waypoint_ID] 
+        self.g_lb = np.zeros(6)
+        self.g_ub = np.zeros(6)
+        self.g_eval = ca.Function('g_manip', [q_ca], [self.g])
 
-    def do_eval(self, q):
-        return self.g_eval(q)
+        
+    def get_constraint(self):
+        return self.g, self.g_lb, self.g_ub
+    
+    def get_limits(self):
+        return self.g_lb, self.g_ub
     
     def set_limits(self, lb, ub):
         self.g_lb = lb
         self.g_ub = ub
-
-    def get_limits(self):
-        return self.g_lb, self.g_ub
     
-    def update_limits(self, T_W_Grasp):
-        R_W_Grasp_rpy = sc.Rotation.from_matrix(T_W_Grasp[:3,:3]).as_euler("xyz") #convert rotation part of FK into rpy 
-        self._T_W_Grasp_rpy = np.vstack((T_W_Grasp[:3,3][:,None], R_W_Grasp_rpy))
-        g_lb = (np.zeros((3,1)) + self._T_W_Grasp_rpy[:3]) - self.tolerance
-        g_ub = (np.zeros((3,1)) + self._T_W_Grasp_rpy[:3]) + self.tolerance
-        self.set_limits(g_lb, g_ub)
+    def do_eval(self, q):
+        return self.g_eval(q)
```

### Comparing `grasp_planning-0.4.2/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.0/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 import numpy as np
 import casadi as ca
 import spatial_casadi as sc
 from grasp_planning.constraints.constraint_template import Constraint
 
-
-class ManipulationConstraint(Constraint):
-    def __init__(self, robot, q_ca, waypoint_ID, n_dofs) -> None:
+class GraspPosConstraint(Constraint):
+    def __init__(self, robot, q_ca, waypoint_ID, param_grasp_ca, tolerance=0.0) -> None:
         super().__init__() 
         # q = q_ca[:n_dof, waypoint_ID] -> joint space of the robot (decision variable)
         # manip_frame = q_ca[n_dof:, waypoint_ID] -> manipulation frame (decision variable)
-        # FK(q)_rpy - manip frame = 0
+        # manip frame_pos - T_W_Grasp_pos = 0
         self._robot = robot
+        self.tolerance = tolerance
+        Rpy_W_EEF = self._robot.compute_fk_rpy_ca(q_ca[:,waypoint_ID])
         
-        self.g = self._robot.compute_fk_rpy_ca(q_ca[:n_dofs, waypoint_ID]) - q_ca[n_dofs:, waypoint_ID] 
-        self.g_lb = np.zeros(6)
-        self.g_ub = np.zeros(6)
-        self.g_eval = ca.Function('g_manip', [q_ca], [self.g])
-
-        
+        self.g = Rpy_W_EEF[:3] - param_grasp_ca[:3,3]
+        self.g_lb = np.zeros(3) - self.tolerance
+        self.g_ub = np.zeros(3) + self.tolerance
+        self.g_eval = ca.Function('g_grasp_pos', [q_ca, param_grasp_ca], [self.g])
+      
     def get_constraint(self):
-        return self.g
-    
-    def get_limits(self):
-        return self.g_lb, self.g_ub
-    
-    def set_limits(self, lb, ub):
-        self.g_lb = lb
-        self.g_ub = ub
-    
-    def do_eval(self, q):
-        return self.g_eval(q)
+        return self.g, self.g_lb, self.g_ub
+
+    def do_eval(self, q, T_W_Grasp):
+        return self.g_eval(q, T_W_Grasp)
```

### Comparing `grasp_planning-0.4.2/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.0/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.4.2/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.5.0/grasp_planning/solver/gomp_planner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 import numpy as np
 import casadi as ca
 import spatial_casadi as sc
 from scipy.spatial.transform import Rotation as R
 from grasp_planning.solver.robot_model import RobotKinematicModel
 from grasp_planning.cost.costs import SquaredAccCost
-from grasp_planning.constraints.constraints import GraspPosConstraint, GraspRotConstraint, ManipulationConstraint
+from grasp_planning.constraints.constraints import *
 
 class GOMP():
     def __init__(self, n_waypoints, urdf, theta=np.pi/4, root_link='world', end_link='tool_frame') -> None:
         # Init variables
         self.T_W_Grasp = None
         self.T_W_Obj = None
         self.T_Obj_Grasp = np.eye(4, dtype=float)
         
         # Kinematics
         self._robot_model = RobotKinematicModel(urdf, root_link, end_link)
         self.n_dofs = self._robot_model.n_dofs
         self.manipulation_frame_dim = 6
-        self.x_dim = self.n_dofs + self.manipulation_frame_dim
+        self.x_dim = self.n_dofs
         self.n_waypoints = n_waypoints
         self.theta = theta
         
         # Optimization
         self.x = ca.SX.sym("x", self.x_dim, self.n_waypoints)
         self.x_init = None
         
         self._objective = None
         self.l_joint_limits, self.u_joint_limits = None, None
         self.g_list = []
 
+        self.param_grasp_ca = ca.SX.sym("param_grasp", 4, 4)
+        self.param_obst_ca = ca.SX.sym("param_obst", 4, 4)
 
 
 
     def update_grasp_DOF(self, theta: float, degrees=True) -> None:
         """
         Object has to have z-axis aligned with the world frame
         """
+        self.T_Obj_Grasp = np.eye(4, dtype=float)
         if degrees:
             R_Obj_Grasp = R.from_euler('xyz', [180, 0, theta], degrees=True).as_matrix()
-            self.theta = np.deg2rad(theta)
+            self.theta = np.round(np.deg2rad(theta), 2)
         else:
             R_Obj_Grasp = R.from_euler('xyz', [np.pi, 0, theta], degrees=False).as_matrix()
-            self.theta = theta
+            self.theta = np.round(theta, 2)
         self.T_Obj_Grasp[:3,:3] = R_Obj_Grasp
         self.T_W_Grasp = self.T_W_Obj @ self.T_Obj_Grasp
 
     def update_object_pose(self, T_W_Obj: np.array) -> None:
         """
         Update object and grasp poses
         """
@@ -80,68 +83,88 @@
         
         # init boundary
         self.l_joint_limits[:,0] = q_start
         self.u_joint_limits[:,0] = q_start
 
         if q_end != None:
             print("Final boundary condition is not implemented.")
-      
+    
+    
 
-    def setup_problem(self):
+    def setup_problem(self, verbose=False):
         # assert self.T_Obj_Grasp != None, "Grasp DOF is not set. Set additional degree of freedom around object."
         # assert self.T_W_Obj != None, "Object pose is not set."
         # 1. create decision variable
         x_ca_flatten = self.x.reshape((-1,1))
         
         # assert self.x_init != None, "Initial guess is missing. Set up one using `set_init_guess(q)`."
 
         # Define objective function
         cost = SquaredAccCost(self.n_waypoints, self.x_dim, manip_frame=True)
         objective = cost.eval_cost(x_ca_flatten)
 
-        # Define constraints
-        g = ca.vertcat()
+        g, self.g_lb, self.g_ub = ca.vertcat(), ca.vertcat(), ca.vertcat()
         for g_term in self.g_list:
-            gt = g_term.get_constraint()
+            gt, g_lb, g_ub = g_term.get_constraint()
             g = ca.vertcat(g, gt)
+            self.g_lb = ca.vertcat(self.g_lb, g_lb)
+            self.g_ub = ca.vertcat(self.g_ub, g_ub)
+
+
 
         options = {}
         options["ipopt.acceptable_tol"] = 1e-3
-        self.solver = ca.nlpsol('solver', 'ipopt', {'x': x_ca_flatten, 'f': objective, 'g': g}, options)
-  
+        if not verbose:
+            options["ipopt.print_level"] = 0
+            options["print_time"] = 0
+
+        params_optim_ca = ca.vertcat(self.param_grasp_ca, self.param_obst_ca)
+        self.solver = ca.nlpsol('solver', 'ipopt', {'x': x_ca_flatten, 'f': objective, 'g': g, 'p': params_optim_ca}, options)
+    
+
         
     def solve(self):
         result = self.solver(x0=self.x_init,
                              lbg=self.g_lb,
                              ubg=self.g_ub,
                              lbx=self.l_joint_limits.reshape((-1,1), order='F'),
-                             ubx=self.u_joint_limits.reshape((-1,1), order='F'))
-        return result['x']
+                             ubx=self.u_joint_limits.reshape((-1,1), order='F'),
+                             p=self.params_optim_num)
+        success_flag = self.solver.stats()["success"]
+        success_msg = self.solver.stats()["return_status"]
+        return result['x'], success_flag
 
     def _add_grasp_pos_constraint(self, waypoint_ID, tolerance=0.0):
-        self.g_list.append(ManipulationConstraint(self._robot_model, self.x, waypoint_ID, self.n_dofs))
-        self.g_list.append(GraspPosConstraint(self._robot_model, self.x, waypoint_ID, self.n_dofs, tolerance))
+        self.g_list.append(GraspPosConstraint(self._robot_model, 
+                                              self.x, 
+                                              waypoint_ID, 
+                                              self.param_grasp_ca, 
+                                              tolerance))
 
     def _add_grasp_rot_constraint(self, waypoint_ID, tolerance=0.1):
-        self.g_list.append(GraspRotConstraint(self._robot_model, self.x, waypoint_ID, self.n_dofs, self.theta, tolerance))
-
+        self.g_list.append(GraspRotConstraint(self._robot_model, 
+                                              self.x, 
+                                              waypoint_ID, 
+                                              self.param_grasp_ca, 
+                                              self.theta, 
+                                              tolerance))
 
     def add_grasp_constraint(self, waypoint_ID, tolerance=0.0):
         self._add_grasp_pos_constraint(waypoint_ID, tolerance)
-        self._add_grasp_rot_constraint(waypoint_ID)
+        self._add_grasp_rot_constraint(waypoint_ID, tolerance)
 
-    def add_collision_constraint(self, waypoint_ID):
-        pass
+    def add_collision_constraint(self, waypoint_ID, child_link, r_link=0.5, r_obst=0.2, tolerance=0.01):
+        self.g_list.append(CollisionConstraint(robot=self._robot_model,
+                                                q_ca=self.x,
+                                                waypoint_ID=waypoint_ID,
+                                                param_obst_ca=self.param_obst_ca,
+                                                link_name=child_link,
+                                                r_link= r_link,
+                                                r_obst= r_obst,
+                                                tolerance=tolerance))
 
-    def update_constraints_boundaries(self, T_W_Obj):
+    def update_constraints_params(self, T_W_Obj, T_W_Obst):
         self.update_object_pose(T_W_Obj)
         self.update_grasp_DOF(theta=self.theta, degrees=False)
-   
-        self.g_lb, self.g_ub = ca.vertcat(), ca.vertcat()
-
-        for g_term in self.g_list:
-            g_term.update_limits(self.T_W_Grasp)
-            g_lb, g_ub = g_term.get_limits()
-            self.g_lb = ca.vertcat(self.g_lb, g_lb)
-            self.g_ub = ca.vertcat(self.g_ub, g_ub)
-        
 
+      
+        self.params_optim_num = ca.vertcat(T_W_Obj, T_W_Obst)
```

### Comparing `grasp_planning-0.4.2/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.0/grasp_planning/solver/robot_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,21 @@
                         )
         self.end_link = end_link
         self.n_dofs = self.robot_fk.n()
         self.joint_names = []
         self.joint_pos_limits = np.zeros((self.n_dofs, 2))
         self._read_joint_pos_limits()
 
-    def compute_fk_ca(self, q_ca):
-        return self.robot_fk.casadi(q_ca, self.end_link, position_only=False)
-            
+    def compute_fk_ca(self, q_ca, end_link=None):
+        if end_link == None:
+            return self.robot_fk.casadi(q_ca, self.end_link, position_only=False)
+        else:
+            return self.robot_fk.casadi(q_ca, child_link=end_link, position_only=False)
+
+
     def compute_fk_rpy_ca(self, q_ca):
         fk_ca = self.compute_fk_ca(q_ca)
         R_ca_rpy = sc.Rotation.from_matrix(fk_ca[:3,:3]).as_euler("xyz") #convert rotation part of FK into rpy
         return ca.vertcat(fk_ca[:3,3], R_ca_rpy)
 
     def eval_fk(self, q):
         return self.robot_fk.numpy(q, self.end_link, position_only=False)
```

