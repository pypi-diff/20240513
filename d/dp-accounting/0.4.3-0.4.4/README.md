# Comparing `tmp/dp-accounting-0.4.3.tar.gz` & `tmp/dp_accounting-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp-accounting-0.4.3.tar", last modified: Tue Sep 19 20:39:05 2023, max compression
+gzip compressed data, was "dp_accounting-0.4.4.tar", last modified: Mon May 13 18:08:44 2024, max compression
```

## Comparing `dp-accounting-0.4.3.tar` & `dp_accounting-0.4.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-09-19 20:39:05.290081 dp-accounting-0.4.3/
--rw-r--r--   0 pritishk (568285) primarygroup (89939)     1752 2023-09-19 20:39:05.290081 dp-accounting-0.4.3/PKG-INFO
--rw-r-----   0 pritishk (568285) primarygroup (89939)     1806 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/README.md
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-09-19 20:39:05.282081 dp-accounting-0.4.3/dp_accounting/
--rw-r-----   0 pritishk (568285) primarygroup (89939)     1800 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/__init__.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    13808 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/dp_event.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     2833 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/dp_event_builder.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     3054 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/dp_event_builder_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     3688 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/dp_event_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     8640 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/mechanism_calibration.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     8663 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/mechanism_calibration_test.py
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-09-19 20:39:05.290081 dp-accounting-0.4.3/dp_accounting/pld/
--rw-r-----   0 pritishk (568285) primarygroup (89939)      675 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/__init__.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    13306 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/accountant.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     8424 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/accountant_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    12372 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/common.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     8948 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/common_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    32711 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/pld_pmf.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    28136 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/pld_pmf_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     5662 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/pld_privacy_accountant.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     6085 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/pld_privacy_accountant_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    63971 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_distribution.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     2548 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_distribution_basic_example.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    52970 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_distribution_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    73592 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_mechanism.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    64627 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_mechanism_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     3054 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/test_util.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     3647 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/pld/test_util_test.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     5579 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/privacy_accountant.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)     4351 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/privacy_accountant_test.py
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-09-19 20:39:05.290081 dp-accounting-0.4.3/dp_accounting/rdp/
--rw-r-----   0 pritishk (568285) primarygroup (89939)      744 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/rdp/__init__.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    34719 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/rdp/rdp_privacy_accountant.py
--rw-r-----   0 pritishk (568285) primarygroup (89939)    28704 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/dp_accounting/rdp/rdp_privacy_accountant_test.py
-drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2023-09-19 20:39:05.282081 dp-accounting-0.4.3/dp_accounting.egg-info/
--rw-r--r--   0 pritishk (568285) primarygroup (89939)     1752 2023-09-19 20:39:04.000000 dp-accounting-0.4.3/dp_accounting.egg-info/PKG-INFO
--rw-r-----   0 pritishk (568285) primarygroup (89939)     1277 2023-09-19 20:39:04.000000 dp-accounting-0.4.3/dp_accounting.egg-info/SOURCES.txt
--rw-r-----   0 pritishk (568285) primarygroup (89939)        1 2023-09-19 20:39:04.000000 dp-accounting-0.4.3/dp_accounting.egg-info/dependency_links.txt
--rw-r-----   0 pritishk (568285) primarygroup (89939)       73 2023-09-19 20:39:04.000000 dp-accounting-0.4.3/dp_accounting.egg-info/requires.txt
--rw-r-----   0 pritishk (568285) primarygroup (89939)       14 2023-09-19 20:39:04.000000 dp-accounting-0.4.3/dp_accounting.egg-info/top_level.txt
--rw-r-----   0 pritishk (568285) primarygroup (89939)       38 2023-09-19 20:39:05.290081 dp-accounting-0.4.3/setup.cfg
--rw-r-----   0 pritishk (568285) primarygroup (89939)     2576 2023-09-19 20:37:33.000000 dp-accounting-0.4.3/setup.py
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2024-05-13 18:08:44.187655 dp_accounting-0.4.4/
+-rw-r--r--   0 pritishk (568285) primarygroup (89939)     1752 2024-05-13 18:08:44.187655 dp_accounting-0.4.4/PKG-INFO
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     1806 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/README.md
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2024-05-13 18:08:44.179654 dp_accounting-0.4.4/dp_accounting/
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     1967 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/__init__.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    14600 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/dp_event.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     2833 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/dp_event_builder.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     3054 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/dp_event_builder_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     3816 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/dp_event_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    10331 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/mechanism_calibration.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    11661 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/mechanism_calibration_test.py
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2024-05-13 18:08:44.187655 dp_accounting-0.4.4/dp_accounting/pld/
+-rw-r-----   0 pritishk (568285) primarygroup (89939)      953 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/__init__.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    13307 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/accountant.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     8425 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/accountant_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    12372 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/common.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     8949 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/common_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    32712 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/pld_pmf.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    28137 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/pld_pmf_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     6337 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/pld_privacy_accountant.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     7048 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/pld_privacy_accountant_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    66862 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_distribution.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     2565 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_distribution_basic_example.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    67894 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_distribution_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)   100241 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_mechanism.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    89447 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_mechanism_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     3054 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/test_util.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     3648 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/pld/test_util_test.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     5579 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/privacy_accountant.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     4351 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/privacy_accountant_test.py
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2024-05-13 18:08:44.187655 dp_accounting-0.4.4/dp_accounting/rdp/
+-rw-r-----   0 pritishk (568285) primarygroup (89939)      797 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/rdp/__init__.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    35741 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/rdp/rdp_privacy_accountant.py
+-rw-r-----   0 pritishk (568285) primarygroup (89939)    29256 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/dp_accounting/rdp/rdp_privacy_accountant_test.py
+drwxr-x---   0 pritishk (568285) primarygroup (89939)        0 2024-05-13 18:08:44.187655 dp_accounting-0.4.4/dp_accounting.egg-info/
+-rw-r--r--   0 pritishk (568285) primarygroup (89939)     1752 2024-05-13 18:08:44.000000 dp_accounting-0.4.4/dp_accounting.egg-info/PKG-INFO
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     1277 2024-05-13 18:08:44.000000 dp_accounting-0.4.4/dp_accounting.egg-info/SOURCES.txt
+-rw-r-----   0 pritishk (568285) primarygroup (89939)        1 2024-05-13 18:08:44.000000 dp_accounting-0.4.4/dp_accounting.egg-info/dependency_links.txt
+-rw-r-----   0 pritishk (568285) primarygroup (89939)       73 2024-05-13 18:08:44.000000 dp_accounting-0.4.4/dp_accounting.egg-info/requires.txt
+-rw-r-----   0 pritishk (568285) primarygroup (89939)       14 2024-05-13 18:08:44.000000 dp_accounting-0.4.4/dp_accounting.egg-info/top_level.txt
+-rw-r-----   0 pritishk (568285) primarygroup (89939)       38 2024-05-13 18:08:44.187655 dp_accounting-0.4.4/setup.cfg
+-rw-r-----   0 pritishk (568285) primarygroup (89939)     2576 2024-05-13 17:59:42.000000 dp_accounting-0.4.4/setup.py
```

### Comparing `dp-accounting-0.4.3/PKG-INFO` & `dp_accounting-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-accounting
-Version: 0.4.3
+Version: 0.4.4
 Summary: Tools for tracking differential privacy budgets
 Home-page: https://github.com/google/differential-privacy/
 Author: Google Differential Privacy Team
 Author-email: dp-open-source@google.com
 License: Apache 2.0
 Keywords: differential-privacy accounting
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dp-accounting-0.4.3/README.md` & `dp_accounting-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.3/dp_accounting/__init__.py` & `dp_accounting-0.4.4/dp_accounting/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,32 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """DP Accounting package."""
 
+from dp_accounting import dp_event
+from dp_accounting import dp_event_builder
+from dp_accounting import mechanism_calibration
 from dp_accounting import pld
+from dp_accounting import privacy_accountant
 from dp_accounting import rdp
-
 from dp_accounting.dp_event import ComposedDpEvent
 from dp_accounting.dp_event import DpEvent
 from dp_accounting.dp_event import GaussianDpEvent
 from dp_accounting.dp_event import LaplaceDpEvent
 from dp_accounting.dp_event import NonPrivateDpEvent
 from dp_accounting.dp_event import NoOpDpEvent
 from dp_accounting.dp_event import PoissonSampledDpEvent
 from dp_accounting.dp_event import SampledWithoutReplacementDpEvent
 from dp_accounting.dp_event import SampledWithReplacementDpEvent
 from dp_accounting.dp_event import SelfComposedDpEvent
 from dp_accounting.dp_event import SingleEpochTreeAggregationDpEvent
 from dp_accounting.dp_event import UnsupportedDpEvent
-
 from dp_accounting.dp_event_builder import DpEventBuilder
-
 from dp_accounting.mechanism_calibration import calibrate_dp_mechanism
 from dp_accounting.mechanism_calibration import ExplicitBracketInterval
 from dp_accounting.mechanism_calibration import LowerEndpointAndGuess
-
 from dp_accounting.privacy_accountant import NeighboringRelation
 from dp_accounting.privacy_accountant import PrivacyAccountant
 from dp_accounting.privacy_accountant import UnsupportedEventError
```

### Comparing `dp-accounting-0.4.3/dp_accounting/dp_event.py` & `dp_accounting-0.4.4/dp_accounting/dp_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -366,7 +366,29 @@
     event: The DpEvent that is being repeated.
     mean: The mean number of repetitions.
     shape: The shape of the distribution of the number of repetitions.
   """
   event: DpEvent
   mean: float
   shape: float
+
+
+@attr.s(frozen=True, slots=True, auto_attribs=True)
+class MixtureOfGaussiansDpEvent(DpEvent):
+  """Represents an application of the Mixture of Gaussians mechanism.
+
+  For sigma, sensitivities c_i and probabilities p_i, given D this mechanism
+  outputs a sample from N(0, sigma^2) and given D' this mechanism outputs a
+  sample from sum_i p_i N(c_i, sigma^2).
+
+  See https://arxiv.org/abs/2310.15526 for details.
+
+  Attributes:
+    standard_deviation: The standard deviation of the Gaussian noise.
+    sensitivities: The support of the sensitivity random variable. Should be the
+      same length as sampling_probs.
+    sampling_probs: The probabilities associated with the sensitivities.
+  """
+
+  standard_deviation: float
+  sensitivities: Sequence[float]
+  sampling_probs: Sequence[float]
```

### Comparing `dp-accounting-0.4.3/dp_accounting/dp_event_builder.py` & `dp_accounting-0.4.4/dp_accounting/dp_event_builder.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.3/dp_accounting/dp_event_builder_test.py` & `dp_accounting-0.4.4/dp_accounting/dp_event_builder_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.3/dp_accounting/dp_event_test.py` & `dp_accounting-0.4.4/dp_accounting/dp_event_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,18 @@
                   dp_event.SampledWithReplacementDpEvent(
                       1000, 10, dp_event.GaussianDpEvent(1.0)
                   ),
                   50,
               ),
           ]),
       ),
+      (
+          'mixture_gaussian',
+          dp_event.MixtureOfGaussiansDpEvent(1.0, [0, 1, 2], [0.25, 0.5, 0.25]),
+      ),
   )
   def test_to_from_named_tuple(self, event):
     named_tuple = event.to_named_tuple()
     self.assertIsInstance(named_tuple, tuple)
     self.assertIsInstance(named_tuple, dp_event.DpEventNamedTuple)
     assert_not_contains_attrs(named_tuple)
```

### Comparing `dp-accounting-0.4.3/dp_accounting/mechanism_calibration.py` & `dp_accounting-0.4.4/dp_accounting/mechanism_calibration.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,18 +42,14 @@
   initial_guess: float
 
 
 class NoBracketIntervalFoundError(Exception):
   """Error raised when explicit bracket interval cannot be found."""
 
 
-class NoOptimumFoundError(Exception):
-  """Error raised when root finding algorithm fails."""
-
-
 class NonEmptyAccountantError(Exception):
   """Error raised when result of make_fresh_accountant has nonempty ledger."""
 
 
 def _search_for_explicit_bracket_interval(
     bracket_interval: LowerEndpointAndGuess,
     epsilon_gap: Callable[[float], float]) -> ExplicitBracketInterval:
@@ -96,14 +92,67 @@
     gap *= 2  # Loop invariant: gap = initial_gap * (2 ** num_tries).
     lower, upper = upper, upper + gap
     lower_value, upper_value = upper_value, epsilon_gap(upper)
 
   return ExplicitBracketInterval(lower, upper)
 
 
+def _bisect(
+    function: Callable[[float], float],
+    lower: float,
+    upper: float,
+    tol: float,
+    lower_value: Optional[float] = None,
+    upper_value: Optional[float] = None,
+) -> float:
+  """Bisection search to find approximate root with non-positive value.
+
+  Args:
+    function: Function to find approximate root of. Conceptually, the function
+      should be continuous, although really the only requirement is that it has
+      opposite signs at the endpoints.
+    lower: Lower endpoint.
+    upper: Upper endpoint.
+    tol: Terminate when endpoints are within tol of each other.
+    lower_value: Value at lower endpoint.
+    upper_value: Value at upper endpoint.
+
+  Returns:
+    A point with non-positive value within tol of root.
+
+  Raises:
+    ValueError: If values at lower and upper do not have opposite signs.
+  """
+  if lower_value is None:
+    lower_value = function(lower)
+  if upper_value is None:
+    upper_value = function(upper)
+
+  if lower_value == 0:
+    return lower
+  if upper_value == 0:
+    return upper
+
+  if lower_value * upper_value > 0:
+    raise ValueError('Values must have opposite signs.')
+
+  if upper - lower <= tol:
+    return lower if lower_value < 0 else upper
+
+  middle = (lower + upper) / 2
+  middle_value = function(middle)
+
+  if middle_value == 0:
+    return middle
+  elif lower_value * middle_value < 0:
+    return _bisect(function, lower, middle, tol, lower_value, middle_value)
+  else:
+    return _bisect(function, middle, upper, tol, middle_value, upper_value)
+
+
 def calibrate_dp_mechanism(
     make_fresh_accountant: Callable[[], privacy_accountant.PrivacyAccountant],
     make_event_from_param: Union[Callable[[float], dp_event.DpEvent],
                                  Callable[[int], dp_event.DpEvent]],
     target_epsilon: float,
     target_delta: float,
     bracket_interval: Optional[BracketInterval] = None,
@@ -148,15 +197,14 @@
     constraint. If discrete=True, the returned value will be an integer.
     Otherwise it will be a float.
 
   Raises:
     NoBracketIntervalFoundError: if bracket_interval is LowerEndpointAndGuess
       and no upper bound can be found within a factor of 2**30 of the original
       guess.
-    NoOptimumFoundError: if scipy.optimize.brentq fails to find an optimum.
     NonEmptyAccountantError: if make_fresh_accountant returns an accountant with
       nonempty ledger.
   """
 
   if not callable(make_fresh_accountant):
     raise TypeError(f'make_fresh_accountant must be callable. '
                     f'found {type(make_fresh_accountant)}.')
@@ -173,17 +221,17 @@
     raise ValueError(f'target_delta must be in range [0, 1]. Found '
                      f'{target_delta}.')
 
   if bracket_interval is None:
     bracket_interval = LowerEndpointAndGuess(0, 1)
 
   if tol is None:
-    tol = 0.5 if discrete else 1e-6
+    tol = 1.0 if discrete else 1e-6
   elif discrete:
-    tol = max(tol, 0.5)
+    tol = max(tol, 1.0)
   elif tol <= 0:
     raise ValueError(f'tol must be positive. Found {tol}.')
 
   def epsilon_gap(x: float) -> float:
     if discrete:
       x = round(x)
     event = make_event_from_param(x)
@@ -208,25 +256,35 @@
         full_output=True)
   except ValueError as err:
     raise ValueError(
         '`brentq` raised ValueError. This often means the supplied bracket '
         f'interval {bracket_interval} did not bracket a solution.') from err
 
   if not result.converged:
-    raise NoOptimumFoundError(
-        'Unable to find root with scipy.optimize.brentq.')
-
-  if epsilon_gap(root) > 0:
-    # Ensure that gap is not positive, guaranteeing returned parameter gives no
-    # less privacy than was requested.
-    if epsilon_gap(root + tol) < 0:
-      root += tol
-    elif epsilon_gap(root - tol) < 0:
-      root -= tol
-    else:
-      raise NoOptimumFoundError(
-          f'Unable to find valid value near root {root} returned by brentq.')
+    root = None
+  else:
+    # We need to ensure that gap is not positive, guaranteeing the returned
+    # parameter gives no less privacy than was requested. Since epsilon_gap can
+    # be expensive to compute, we first try values near the returned root.
+    # Considering brentq's contract that there exists a root within tol of the
+    # returned value, in most cases adding +/- tol will suffice.
+    if epsilon_gap(root) > 0:
+      if epsilon_gap(root + tol) < 0:
+        root += tol
+      elif epsilon_gap(root - tol) < 0:
+        root -= tol
+      else:
+        root = None
+
+  if root is None:
+    # Fallback to custom bisection that guarantees root with non-positive value.
+    root = _bisect(
+        epsilon_gap,
+        bracket_interval.endpoint_1,
+        bracket_interval.endpoint_2,
+        tol,
+    )
 
   if discrete:
     root = round(root)
 
   return root
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/__init__.py` & `dp_accounting-0.4.4/dp_accounting/rdp/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,10 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""PLD Accounting package."""
+"""RDP Accounting package."""
 
-from dp_accounting.pld.pld_privacy_accountant import PLDAccountant
+from dp_accounting.rdp import rdp_privacy_accountant
+from dp_accounting.rdp.rdp_privacy_accountant import compute_epsilon
+from dp_accounting.rdp.rdp_privacy_accountant import RdpAccountant
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/accountant.py` & `dp_accounting-0.4.4/dp_accounting/pld/accountant.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Helper functions for privacy accounting across queries."""
 
 import math
 from typing import Callable, Optional
+
 from scipy import special
 
 from dp_accounting.pld import common
 from dp_accounting.pld import privacy_loss_distribution
 from dp_accounting.pld import privacy_loss_mechanism
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/accountant_test.py` & `dp_accounting-0.4.4/dp_accounting/pld/accountant_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for accountant."""
 
 import unittest
+
 from absl.testing import parameterized
 
 from dp_accounting.pld import accountant
 from dp_accounting.pld import common
 
 
 class AccountantTest(parameterized.TestCase):
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/common.py` & `dp_accounting-0.4.4/dp_accounting/pld/common.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/common_test.py` & `dp_accounting-0.4.4/dp_accounting/pld/common_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for common."""
 
 import math
 import unittest
 from unittest import mock
+
 from absl.testing import parameterized
 
 from dp_accounting.pld import common
 from dp_accounting.pld import test_util
 
 
 class DifferentialPrivacyParametersTest(parameterized.TestCase):
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/pld_pmf.py` & `dp_accounting-0.4.4/dp_accounting/pld/pld_pmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 """
 
 import abc
 import itertools
 import math
 import numbers
 from typing import Iterable, List, Mapping, Sequence, Tuple, Union
+
 import numpy as np
 import numpy.typing
 from scipy import signal
 
 from dp_accounting.pld import common
 
 ArrayLike = Union[np.ndarray, List[float]]
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/pld_pmf_test.py` & `dp_accounting-0.4.4/dp_accounting/pld/pld_pmf_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for PLDPmf."""
 
 import unittest
+
 from absl.testing import parameterized
 import numpy as np
 
 from dp_accounting.pld import common
 from dp_accounting.pld import pld_pmf
 from dp_accounting.pld import test_util
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/pld_privacy_accountant.py` & `dp_accounting-0.4.4/dp_accounting/pld/pld_privacy_accountant.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,14 +72,29 @@
         else:
           laplace_pld = PLD.from_laplace_mechanism(
               parameter=event.noise_multiplier,
               value_discretization_interval=self._value_discretization_interval
           ).self_compose(count)
           self._pld = self._pld.compose(laplace_pld)
       return None
+    elif isinstance(event, dp_event.MixtureOfGaussiansDpEvent):
+      if do_compose:
+        if len(event.sensitivities) == 1 and event.sensitivities[0] == 0.0:
+          pass
+        elif event.standard_deviation == 0:
+          self._contains_non_dp_event = True
+        else:
+          mog_pld = PLD.from_mixture_gaussian_mechanism(
+              standard_deviation=event.standard_deviation,
+              sensitivities=event.sensitivities,
+              sampling_probs=event.sampling_probs,
+              value_discretization_interval=self._value_discretization_interval,
+          ).self_compose(count)
+          self._pld = self._pld.compose(mog_pld)
+      return None
     elif isinstance(event, dp_event.PoissonSampledDpEvent):
       if self.neighboring_relation != NeighborRel.ADD_OR_REMOVE_ONE:
         error_msg = (
             'neighboring_relation must be `ADD_OR_REMOVE_ONE` for '
             f'`PoissonSampledDpEvent`. Found {self._neighboring_relation}.')
         return CompositionErrorDetails(
             invalid_event=event, error_message=error_msg)
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/pld_privacy_accountant_test.py` & `dp_accounting-0.4.4/dp_accounting/pld/pld_privacy_accountant_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,26 +51,31 @@
     with self.assertRaises(ValueError):
       accountant.compose(event, count)
 
   @parameterized.parameters(
       dp_event.GaussianDpEvent(0),
       dp_event.LaplaceDpEvent(0),
       dp_event.PoissonSampledDpEvent(0.1, dp_event.GaussianDpEvent(0)),
-      dp_event.PoissonSampledDpEvent(0.1, dp_event.LaplaceDpEvent(0)))
+      dp_event.PoissonSampledDpEvent(0.1, dp_event.LaplaceDpEvent(0)),
+      dp_event.MixtureOfGaussiansDpEvent(0, [1, 2], [0.5, 0.5]),
+  )
   def test_additive_noise_mechanisms_with_zero_noise_multiplier(self, event):
     accountant = pld_privacy_accountant.PLDAccountant()
     accountant.compose(event)
     self.assertEqual(accountant.get_delta(1.0), 1)
     self.assertEqual(accountant.get_epsilon(0.01), math.inf)
 
   @parameterized.parameters(
       dp_event.PoissonSampledDpEvent(0, dp_event.GaussianDpEvent(1)),
       dp_event.PoissonSampledDpEvent(0, dp_event.LaplaceDpEvent(1)),
       dp_event.PoissonSampledDpEvent(0, dp_event.GaussianDpEvent(0)),
-      dp_event.PoissonSampledDpEvent(0, dp_event.LaplaceDpEvent(0)))
+      dp_event.PoissonSampledDpEvent(0, dp_event.LaplaceDpEvent(0)),
+      dp_event.MixtureOfGaussiansDpEvent(1, [0], [1.0]),
+      dp_event.MixtureOfGaussiansDpEvent(0, [0], [1.0]),
+  )
   def test_poisson_subsampling_with_zero_probability(self, event):
     accountant = pld_privacy_accountant.PLDAccountant()
     accountant.compose(event)
     self.assertEqual(accountant.get_delta(0), 0)
     self.assertEqual(accountant.get_epsilon(0), 0)
 
   def test_gaussian_basic(self):
@@ -118,31 +123,55 @@
     second_laplace_event = dp_event.LaplaceDpEvent(noise_multiplier=2)
     accountant = pld_privacy_accountant.PLDAccountant()
     accountant.compose(first_laplace_event, 3)
     accountant.compose(second_laplace_event, 2)
 
     expected_epsilon = 4
     expected_delta = 1e-14  # expected delta is not 0 due to truncation in
-                            # self composition
+    # self composition
     self.assertAlmostEqual(
         accountant.get_delta(expected_epsilon), expected_delta, delta=1e-6)
     self.assertAlmostEqual(
         accountant.get_epsilon(expected_delta), expected_epsilon, delta=1e-6)
 
   def test_poisson_subsampled_laplace(self):
     subsampled_laplace_event = dp_event.PoissonSampledDpEvent(
         0.2, dp_event.LaplaceDpEvent(noise_multiplier=0.5))
     accountant = pld_privacy_accountant.PLDAccountant()
     accountant.compose(subsampled_laplace_event, 1)
     accountant.compose(subsampled_laplace_event, 2)
 
     exact_epsilon = 2.46964
     expected_delta = 1e-14  # expected delta is not 0 due to truncation in
-                            # self composition
+    # self composition
     self.assertAlmostEqual(
         accountant.get_delta(exact_epsilon), expected_delta, delta=1e-6)
     self.assertAlmostEqual(
         accountant.get_epsilon(expected_delta), exact_epsilon, delta=1e-3)
 
+  def test_mixture_of_gaussians_basic(self):
+    first_mog_event = dp_event.MixtureOfGaussiansDpEvent(
+        standard_deviation=1.0,
+        sensitivities=[0.0, 1.0, 2.0],
+        sampling_probs=[0.2, 0.6, 0.2],
+    )
+    second_mog_event = dp_event.MixtureOfGaussiansDpEvent(
+        standard_deviation=2.0,
+        sensitivities=[0.0, 2.0, 3.0],
+        sampling_probs=[0.33, 0.34, 0.33],
+    )
+    accountant = pld_privacy_accountant.PLDAccountant()
+    accountant.compose(first_mog_event, 3)
+    accountant.compose(second_mog_event, 2)
+
+    expected_epsilon = 17.193115
+    expected_delta = 1e-6
+    self.assertAlmostEqual(
+        accountant.get_delta(expected_epsilon), expected_delta, delta=1e-12
+    )
+    self.assertAlmostEqual(
+        accountant.get_epsilon(expected_delta), expected_epsilon, delta=1e-6
+    )
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_distribution.py` & `dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 ../../common_docs/Privacy_Loss_Distributions.pdf
 """
 
 import collections
 import logging
 import math
 from typing import Any, Callable, Mapping, Optional, Sequence, Tuple, Union
+
 import numpy as np
 
 from dp_accounting.pld import common
 from dp_accounting.pld import pld_pmf
 from dp_accounting.pld import privacy_loss_mechanism
 
 
@@ -1323,14 +1324,77 @@
         value_discretization_interval=value_discretization_interval,
         use_connect_dots=use_connect_dots)
 
   return _pld_for_subsampled_mechanism(single_discrete_gaussian_pld,
                                        sampling_prob)
 
 
+def from_mixture_gaussian_mechanism(
+    standard_deviation: float,
+    sensitivities: Sequence[float],
+    sampling_probs: Sequence[float],
+    pessimistic_estimate: bool = True,
+    value_discretization_interval: float = 1e-4,
+    log_mass_truncation_bound: float = -50,
+    use_connect_dots: bool = True,
+) -> PrivacyLossDistribution:
+  """Creates the privacy loss distribution of a Mixture of Gaussians mechanism.
+
+  This method supports two algorithms for constructing the privacy loss
+  distribution. One given by the "Privacy Buckets" algorithm and other given by
+  "Connect the Dots" algorithm. See Sections 2.1 and 2.2 of supplementary
+  material for more details.
+
+  Args:
+    standard_deviation: the standard_deviation of the Gaussian distribution.
+    sensitivities: the support of the sensitivity distribution. Must be the same
+      length as sampling_probs, and both should be 1D.
+    sampling_probs: the probabilities associated with the sensitivities.
+    pessimistic_estimate: a value indicating whether the rounding is done in
+      such a way that the resulting epsilon-hockey stick divergence computation
+      gives an upper estimate to the real value.
+    value_discretization_interval: the length of the dicretization interval for
+      the privacy loss distribution. The values will be rounded up/down to be
+      integer multiples of this number. Smaller value results in more accurate
+      estimates of the privacy loss, at the cost of increased run-time / memory
+      usage.
+    log_mass_truncation_bound: the ln of the probability mass that might be
+      discarded from the noise distribution. The larger this number, the more
+      error it may introduce in divergence calculations.
+    use_connect_dots: When True (default), the connect-the-dots algorithm will
+      be used to construct the privacy loss distribution. When False, the
+      privacy buckets algorithm will be used.
+
+  Returns:
+    The privacy loss distribution corresponding to the Mixture of Gaussians
+    mechanism with given parameters.
+  """
+
+  def single_pld_pmf(
+      adjacency_type: privacy_loss_mechanism.AdjacencyType,
+  ) -> pld_pmf.PLDPmf:
+    return _create_pld_pmf_from_additive_noise(
+        privacy_loss_mechanism.MixtureGaussianPrivacyLoss(
+            standard_deviation,
+            sensitivities,
+            sampling_probs,
+            pessimistic_estimate=pessimistic_estimate,
+            log_mass_truncation_bound=log_mass_truncation_bound,
+            adjacency_type=adjacency_type,
+        ),
+        pessimistic_estimate=pessimistic_estimate,
+        value_discretization_interval=value_discretization_interval,
+        use_connect_dots=use_connect_dots,
+    )
+
+  pmf_remove = single_pld_pmf(privacy_loss_mechanism.AdjacencyType.REMOVE)
+  pmf_add = single_pld_pmf(privacy_loss_mechanism.AdjacencyType.ADD)
+  return PrivacyLossDistribution(pmf_remove, pmf_add)
+
+
 def from_privacy_parameters(
     privacy_parameters: common.DifferentialPrivacyParameters,
     value_discretization_interval: float = 1e-4) -> PrivacyLossDistribution:
   """Constructs pessimistic PLD from epsilon and delta parameters.
 
   When the mechanism is (epsilon, delta)-differentially private, the following
   is a pessimistic estimate of its privacy loss distribution (see Section 3.5
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_distribution_basic_example.py` & `dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_distribution_basic_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,59 +8,65 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Basic Example for Using Privacy Loss Distributions.
-"""
+"""Basic Example for Using Privacy Loss Distributions."""
 
 from absl import app
 
-from dp_accounting import privacy_loss_distribution
+from dp_accounting.pld import privacy_loss_distribution
 
 
 def main(argv):
   if len(argv) > 1:
     raise app.UsageError('Too many command-line arguments.')
 
   # The parameter of Laplace Noise added
   parameter_laplace = 3
   # PLD for one execution of the Laplace Mechanism. (Throughout we assume that
   # sensitivity = 1.)
   laplace_pld = privacy_loss_distribution.from_laplace_mechanism(
-      parameter_laplace, value_discretization_interval=1e-3)
+      parameter_laplace, value_discretization_interval=1e-3
+  )
 
   # Number of times Laplace Mechanism is run
   num_laplace = 40
   # PLD for num_laplace executions of the Laplace Mechanism.
   composed_laplace_pld = laplace_pld.self_compose(num_laplace)
 
   epsilon = 10
   delta = composed_laplace_pld.get_delta_for_epsilon(epsilon)
-  print(f'An algorithm that executes the Laplace Mechanism with parameter '
-        f'{parameter_laplace} for a total of {num_laplace} times is '
-        f'({epsilon}, {delta})-DP.')
+  print(
+      'An algorithm that executes the Laplace Mechanism with parameter '
+      f'{parameter_laplace} for a total of {num_laplace} times is '
+      f'({epsilon}, {delta})-DP.'
+  )
 
   # PLDs for different mechanisms can also be composed. Below is an example in
   # which we compose PLDs for Laplace Mechanism and Gaussian Mechanism.
 
   # STD of the Gaussian Noise
   standard_deviation = 5
   # PLD for an execution of the Gaussian Mechanism.
   gaussian_pld = privacy_loss_distribution.from_gaussian_mechanism(
-      standard_deviation, value_discretization_interval=1e-3)
+      standard_deviation, value_discretization_interval=1e-3
+  )
 
   # PLD for num_laplace executions of the Laplace Mechanism and one execution of
   # the Gaussian Mechanism.
   composed_laplace_and_gaussian_pld = composed_laplace_pld.compose(gaussian_pld)
 
   epsilon = 10
   delta = composed_laplace_and_gaussian_pld.get_delta_for_epsilon(epsilon)
-  print(f'An algorithm that executes the Laplace Mechanism with parameter '
-        f'{parameter_laplace} for a total of {num_laplace} times and in '
-        f'addition executes once the Gaussian Mechanism with STD '
-        f'{standard_deviation} is ({epsilon}, {delta})-DP.')
+  print(
+      'An algorithm that executes the Laplace Mechanism with parameter '
+      f'{parameter_laplace} for a total of {num_laplace} times and in '
+      'addition executes once the Gaussian Mechanism with STD '
+      f'{standard_deviation} is ({epsilon}, {delta})-DP.'
+  )
+
 
 if __name__ == '__main__':
   app.run(main)
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_distribution_test.py` & `dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_distribution_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for privacy_loss_distribution.py."""
 import math
 from typing import Any, Mapping, Optional
 import unittest
+
 from absl.testing import parameterized
 from scipy import stats
 
 from dp_accounting.pld import common
 from dp_accounting.pld import pld_pmf
 from dp_accounting.pld import privacy_loss_distribution
 from dp_accounting.pld import test_util
@@ -1471,14 +1472,498 @@
 
     _assert_pld_pmf_equal(
         self, pld,
         expected_rounded_pmf_add, expected_infinity_mass_add,
         expected_rounded_pmf_remove, expected_infinity_mass_remove)
 
 
+class MixtureGaussianPrivacyLossDistributionTest(parameterized.TestCase):
+  """Tests for from_mixture_gaussian_mechanism.
+
+  We reuse some test cases from GaussianPrivacyLoss since
+  MixtureGaussianPrivacyLoss generalizes that class. However, since
+  MixtureGaussianPrivacyLoss uses tighter cutoffs on the PLD than
+  GaussianPrivacyLoss, their expected values are different for the same test
+  case.
+  """
+
+  @parameterized.named_parameters(
+      # Gaussian mechanisms
+      {
+          'testcase_name': 'gaussian_1',
+          'standard_deviation': 1.0,
+          'sensitivities': [1.0],
+          'sampling_probs': [1.0],
+          'expected_rounded_pmf_add': {
+              2: 0.12447741,
+              1: 0.38292492,
+              0: 0.30853754,
+          },
+          'expected_rounded_pmf_remove': {
+              2: 0.12447741,
+              1: 0.38292492,
+              0: 0.24173034,
+              -1: 0.0668072
+          },
+      },
+      {
+          'testcase_name': 'gaussian_2',
+          'standard_deviation': 1.0,
+          'sensitivities': [2.0],
+          'sampling_probs': [1.0],
+          'expected_rounded_pmf_add': {
+              1: 0.30853754,
+              2: 0.19146246,
+              3: 0.19146246,
+              4: 0.12447741
+          },
+          'expected_rounded_pmf_remove': {
+              -3: 0.00620967,
+              -2: 0.01654047,
+              -1: 0.04405707,
+              0: 0.09184805,
+              1: 0.14988228,
+              2: 0.19146246,
+              3: 0.19146246,
+              4: 0.12447741,
+          },
+      },
+      # Subsampled Gaussian mechanisms
+      {
+          'testcase_name': 'subsampled_gaussian_1',
+          'standard_deviation': 1.0,
+          'sensitivities': [0.0, 1.0],
+          'sampling_probs': [0.2, 0.8],
+          'expected_rounded_pmf_add': {
+              1: 0.50740234,
+              0: 0.30853754,
+          },
+          'expected_rounded_pmf_remove': {
+              2: 0.03303238,
+              1: 0.39779076,
+              0: 0.38512252
+          },
+      },
+      {
+          'testcase_name': 'subsampled_gaussian_2',
+          'standard_deviation': 5.0,
+          'sensitivities': [0.0, 5.0],
+          'sampling_probs': [0.4, 0.6],
+          'expected_rounded_pmf_add': {
+              1: 0.50740234,
+              0: 0.30853754,
+          },
+          'expected_rounded_pmf_remove': {
+              1: 0.35423381,
+              0: 0.46170751
+          },
+      },
+      # Mixture Gaussian mechanisms
+      {
+          'testcase_name': 'mixture_gaussian_1',
+          'standard_deviation': 1.0,
+          'sensitivities': [0.0, 1.0, 2.0],
+          'sampling_probs': [0.2, 0.6, 0.2],
+          'expected_rounded_pmf_add': {
+              2: 0.315939874,
+              1: 0.0,
+              0: 0.5
+          },
+          'expected_rounded_pmf_remove': {
+              2: 0.315949035,
+              1: 0.300256821,
+              0: 0.0,
+              -1: 0.199743179
+          },
+      },
+  )
+  def test_mixture_gaussian_varying_standard_deviation_and_sensitivity(
+      self,
+      standard_deviation,
+      sensitivities,
+      sampling_probs,
+      expected_rounded_pmf_add,
+      expected_rounded_pmf_remove,
+  ):
+    """Verifies correctness of pessimistic PLD for various parameter values."""
+    pld = privacy_loss_distribution.from_mixture_gaussian_mechanism(
+        standard_deviation,
+        sensitivities=sensitivities,
+        sampling_probs=sampling_probs,
+        log_mass_truncation_bound=math.log(2) + stats.norm.logcdf(-0.9),
+        value_discretization_interval=1,
+        use_connect_dots=False,
+    )
+
+    test_util.assert_dictionary_almost_equal(
+        self, expected_rounded_pmf_add, pld._pmf_add._loss_probs  # pytype: disable=attribute-error
+    )
+    test_util.assert_almost_greater_equal(
+        self, stats.norm.cdf(-0.9), pld._pmf_add._infinity_mass
+    )
+    test_util.assert_dictionary_almost_equal(
+        self, expected_rounded_pmf_remove, pld._pmf_remove._loss_probs  # pytype: disable=attribute-error
+    )
+    test_util.assert_almost_greater_equal(
+        self, stats.norm.cdf(-0.9), pld._pmf_remove._infinity_mass
+    )
+    self.assertFalse(pld._symmetric)
+
+  @parameterized.named_parameters(
+      # Gaussian mechanisms
+      {
+          'testcase_name': 'gaussian_1',
+          'standard_deviation': 1.0,
+          'sensitivities': [1.0],
+          'sampling_probs': [1.0],
+          'expected_rounded_pmf_add': {
+              -1: 0.158655254,
+              0: 0.341344746,
+              1: 0.391270256,
+              2: 0.108729744
+          },
+          'expected_rounded_pmf_remove': {
+              -2: 0.016737493,
+              -1: 0.141917761,
+              0: 0.341344746,
+              1: 0.391270256,
+              2: 0.108729744,
+          },
+      },
+      {
+          'testcase_name': 'gaussian_2',
+          'standard_deviation': 1.0,
+          'sensitivities': [2.0],
+          'sampling_probs': [1.0],
+          'expected_rounded_pmf_add': {
+              0: 0.1749993,
+              1: 0.3250007,
+              2: 0.02438595,
+              3: 0.390660732,
+              4: 0.0,
+          },
+          'expected_rounded_pmf_remove': {
+              -4: 0.0,
+              -3: 0.023964237,
+              -2: 0.0,
+              -1: 0.119561076,
+              0: 0.016344046,
+              1: 0.38577247,
+              2: 0.0,
+              3: 0.390660732,
+              4: 0.0,
+          },
+      },
+      # Subsampled Gaussian mechanisms
+      {
+          'testcase_name': 'subsampled_gaussian_1',
+          'standard_deviation': 1.0,
+          'sensitivities': [0.0, 1.0],
+          'sampling_probs': [0.2, 0.8],
+          'expected_rounded_pmf_add': {
+              -1: 0.158655254,
+              0: 0.422688932,
+              1: 0.395727515
+          },
+          'expected_rounded_pmf_remove': {
+              -1: 0.145580017,
+              0: 0.422688932,
+              1: 0.431001195,
+              2: 0.000729856
+          },
+      },
+      {
+          'testcase_name': 'subsampled_gaussian_2',
+          'standard_deviation': 5.0,
+          'sensitivities': [0.0, 5.0],
+          'sampling_probs': [0.4, 0.6],
+          'expected_rounded_pmf_add': {
+              -1: 0.107598496,
+              0: 0.530601573,
+              1: 0.361799931
+          },
+          'expected_rounded_pmf_remove': {
+              -1: 0.133098756,
+              0: 0.530601573,
+              1: 0.292483037
+          },
+      },
+      # Mixture Gaussian mechanisms
+      {
+          'testcase_name': 'mixture_gaussian_1',
+          'standard_deviation': 1.0,
+          'sensitivities': [0.0, 1.0, 2.0],
+          'sampling_probs': [0.2, 0.6, 0.2],
+          'expected_rounded_pmf_add': {
+              -1: 0.134743039,
+              0: 0.390257664,
+              1: 0.474999297,
+              2: 0.0,
+          },
+          'expected_rounded_pmf_remove': {
+              -2: 0.0,
+              -1: 0.208940423,
+              0: 0.365256961,
+              1: 0.344684545,
+              2: 0.058674138,
+          },
+      },
+  )
+  def test_mixture_gaussian_varying_standard_deviation_and_sensitivity_connect_dots(
+      self,
+      standard_deviation,
+      sensitivities,
+      sampling_probs,
+      expected_rounded_pmf_add,
+      expected_rounded_pmf_remove,
+  ):
+    """Verifies correctness of pessimistic PLD for various parameter values."""
+    pld = privacy_loss_distribution.from_mixture_gaussian_mechanism(
+        standard_deviation,
+        sensitivities=sensitivities,
+        sampling_probs=sampling_probs,
+        log_mass_truncation_bound=math.log(2) + stats.norm.logcdf(-0.9),
+        value_discretization_interval=1,
+        use_connect_dots=True,
+    )
+
+    test_util.assert_dictionary_almost_equal(
+        self, expected_rounded_pmf_add, pld._pmf_add._loss_probs  # pytype: disable=attribute-error
+    )
+    test_util.assert_almost_greater_equal(
+        self, stats.norm.cdf(-0.9), pld._pmf_add._infinity_mass
+    )
+    test_util.assert_dictionary_almost_equal(
+        self, expected_rounded_pmf_remove, pld._pmf_remove._loss_probs  # pytype: disable=attribute-error
+    )
+    test_util.assert_almost_greater_equal(
+        self, stats.norm.cdf(-0.9), pld._pmf_remove._infinity_mass
+    )
+    self.assertFalse(pld._symmetric)
+
+  @parameterized.named_parameters(
+      {
+          'testcase_name': 'discretization_0.5',
+          'value_discretization_interval': 0.5,
+          'expected_add_pmf': {
+              3: 0.02595983,
+              2: 0.3045079,
+              1: 0.22891269,
+              0: 0.25655945
+          },
+          'expected_remove_pmf': {
+              4: 0.01100095,
+              3: 0.10672757,
+              2: 0.1421942,
+              1: 0.17070797,
+              0: 0.17687728,
+              -1: 0.144677,
+              -2: 0.06376406,
+          },
+      },
+      {
+          'testcase_name': 'discretization_0.3',
+          'value_discretization_interval': 0.3,
+          'expected_add_pmf': {
+              4: 0.08817633,
+              3: 0.18512511,
+              2: 0.16071804,
+              1: 0.12536095,
+              0: 0.25655945,
+          },
+          'expected_remove_pmf': {
+              6: 0.01100095,
+              5: 0.05979597,
+              4: 0.07257058,
+              3: 0.08541692,
+              2: 0.09686874,
+              1: 0.10497753,
+              0: 0.10751992,
+              -1: 0.10233776,
+              -2: 0.08761942,
+              -3: 0.08784134,
+          },
+      },
+  )
+  def test_mixture_gaussian_discretization(
+      self,
+      value_discretization_interval,
+      expected_add_pmf,
+      expected_remove_pmf,
+  ):
+    """Verifies correctness of pessimistic PLD for varying discretization."""
+    pld = privacy_loss_distribution.from_mixture_gaussian_mechanism(
+        standard_deviation=1,
+        sensitivities=[0.0, 1.0, 2.0],
+        sampling_probs=[0.2, 0.6, 0.2],
+        log_mass_truncation_bound=math.log(2) + stats.norm.logcdf(-0.9),
+        value_discretization_interval=value_discretization_interval,
+        use_connect_dots=False,
+    )
+    test_util.assert_almost_greater_equal(
+        self, stats.norm.cdf(-0.9), pld._pmf_add._infinity_mass
+    )
+    test_util.assert_almost_greater_equal(
+        self, stats.norm.cdf(-0.9), pld._pmf_remove._infinity_mass
+    )
+    test_util.assert_dictionary_almost_equal(
+        self, expected_add_pmf, pld._pmf_add._loss_probs  # pytype: disable=attribute-error
+    )
+    test_util.assert_dictionary_almost_equal(
+        self, expected_remove_pmf, pld._pmf_remove._loss_probs  # pytype: disable=attribute-error
+    )
+
+  @parameterized.named_parameters(
+      {
+          'testcase_name': 'discretization_0.5',
+          'value_discretization_interval': 0.5,
+          'expected_add_infinity_mass': 7.02736093e-05,
+          'expected_remove_infinity_mass': 0.058450414,
+          'expected_add_pmf': {
+              -1: 0.1766054,
+              0: 0.17661904,
+              1: 0.26907836,
+              2: 0.2845549,
+              3: 0.09307203,
+          },
+          'expected_remove_pmf': {
+              -3: 0.02076718,
+              -2: 0.1046819,
+              -1: 0.16320427,
+              0: 0.17661904,
+              1: 0.15880237,
+              2: 0.12600393,
+              3: 0.09134778,
+              4: 0.10012311,
+          },
+      },
+      {
+          'testcase_name': 'discretization_0.3',
+          'value_discretization_interval': 0.3,
+          'expected_add_infinity_mass': 0.010838515,
+          'expected_remove_infinity_mass': 0.072142753,
+          'expected_add_pmf': {
+              -1: 0.20621578,
+              0: 0.10686974,
+              1: 0.14244404,
+              2: 0.17395599,
+              3: 0.18472755,
+              4: 0.17494839,
+          },
+          'expected_remove_pmf': {
+              -4: 0.05269344,
+              -3: 0.07510462,
+              -2: 0.09546907,
+              -1: 0.10552514,
+              0: 0.10686974,
+              1: 0.10149509,
+              2: 0.09162041,
+              3: 0.07936186,
+              4: 0.06644975,
+              5: 0.05409823,
+              6: 0.09916991,
+          },
+      },
+  )
+  def test_mixture_gaussian_discretization_connect_dots(
+      self,
+      value_discretization_interval,
+      expected_add_infinity_mass,
+      expected_remove_infinity_mass,
+      expected_add_pmf,
+      expected_remove_pmf,
+  ):
+    """Verifies correctness of pessimistic PLD for varying discretization."""
+    pld = privacy_loss_distribution.from_mixture_gaussian_mechanism(
+        standard_deviation=1,
+        sensitivities=[0.0, 1.0, 2.0],
+        sampling_probs=[0.2, 0.6, 0.2],
+        log_mass_truncation_bound=math.log(2) + stats.norm.logcdf(-0.9),
+        value_discretization_interval=value_discretization_interval,
+        use_connect_dots=True,
+    )
+    self.assertAlmostEqual(
+        expected_add_infinity_mass, pld._pmf_add._infinity_mass
+    )
+    self.assertAlmostEqual(
+        expected_remove_infinity_mass, pld._pmf_remove._infinity_mass
+    )
+    test_util.assert_dictionary_almost_equal(
+        self, expected_add_pmf, pld._pmf_add._loss_probs  # pytype: disable=attribute-error
+    )
+    test_util.assert_dictionary_almost_equal(
+        self, expected_remove_pmf, pld._pmf_remove._loss_probs  # pytype: disable=attribute-error
+    )
+
+  @parameterized.named_parameters(
+      (
+          'negative_stdev',
+          -1.0,
+          [1.0],
+          [1.0],
+      ),
+      (
+          'negative_sensitivity',
+          1.0,
+          [-1.0, 1.0],
+          [0.5, 0.5],
+      ),
+      (
+          'negative_probability',
+          1.0,
+          [0.0, 1.0, 2.0],
+          [0.75, 0.75, -0.5],
+      ),
+      (
+          'probability_greater_than_one',
+          1.0,
+          [0.0, 1.0, 2.0],
+          [1.5, 0.5, 0.5],
+      ),
+      (
+          'probabilities_dont_add_up_to_one',
+          1.0,
+          [0.0, 1.0, 2.0],
+          [0.2, 0.2, 0.2],
+      ),
+      (
+          'list_lengths_differ_1',
+          1.0,
+          [1.0],
+          [0.5, 0.5],
+      ),
+      (
+          'list_lengths_differ_2',
+          1.0,
+          [1.0, 2.0, 3.0],
+          [0.5, 0.5],
+      ),
+  )
+  def test_mixture_gaussian_value_errors(
+      self, standard_deviation, sensitivities, sampling_probs
+  ):
+    with self.assertRaises(ValueError):
+      privacy_loss_distribution.from_mixture_gaussian_mechanism(
+          standard_deviation,
+          sensitivities=sensitivities,
+          sampling_probs=sampling_probs,
+          value_discretization_interval=1,
+      )
+
+  def test_mixture_gaussian_does_not_overflow(self):
+    """Verifies that mixture Gaussian PLD does not result in overflow."""
+    privacy_loss_distribution.from_mixture_gaussian_mechanism(
+        standard_deviation=1,
+        sensitivities=[0.0, 1.0, 10.0],
+        sampling_probs=[0.98, 0.01, 0.01],
+        value_discretization_interval=1,
+        use_connect_dots=False,
+    )
+
+
 class RandomizedResponsePrivacyLossDistributionTest(parameterized.TestCase):
 
   @parameterized.parameters((0.5, 2, {
       2: 0.75,
       -1: 0.25
   }), (0.2, 4, {
       3: 0.85,
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/privacy_loss_mechanism.py` & `dp_accounting-0.4.4/dp_accounting/pld/privacy_loss_mechanism.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 Please refer to the supplementary material below for more details:
 ../docs/Privacy_Loss_Distributions.pdf
 """
 
 import abc
 import dataclasses
 import enum
+import functools
 import math
 import numbers
-from typing import Iterable, List, Mapping, Optional, Union
+from typing import Iterable, List, Mapping, Optional, Sequence, Union
+
 import numpy as np
+import scipy
 from scipy import stats
 
 from dp_accounting.pld import common
 
 
 class AdjacencyType(enum.Enum):
   """Designates the type of adjacency for computing privacy loss distributions.
@@ -271,15 +274,15 @@
         self.inverse_privacy_loss(eps) for eps in epsilons[inverse_indices]
     ])
     deltas[inverse_indices] = (
         self.mu_upper_cdf(x_cutoffs) -
         np.exp(epsilons[inverse_indices] + self.mu_lower_log_cdf(x_cutoffs)))
     # Clip delta values to lie in [0,1] (to avoid numerical errors)
     deltas = np.clip(deltas, 0, 1)
-    return float(deltas) if is_scalar else deltas
+    return float(deltas[0]) if is_scalar else deltas
 
   @abc.abstractmethod
   def privacy_loss_tail(self) -> TailPrivacyLossDistribution:
     """Computes the privacy loss at the tail of the distribution.
 
     Returns:
       A TailPrivacyLossDistribution instance representing the tail of the
@@ -1671,7 +1674,648 @@
         adjacency_type=adjacency_type)
 
   def standard_deviation(self) -> float:
     """The standard deviation of the corresponding discrete Gaussian noise."""
     return math.sqrt(
         sum(((i + self._offset)**2) * probability_mass
             for i, probability_mass in enumerate(self._pmf_array)))
+
+
+@np.vectorize
+def _pl_without_sampling_add(pl, sampling_prob):
+  return -common.log_a_times_exp_b_plus_c(
+      1 / (sampling_prob), -pl, 1 - 1 / (sampling_prob)
+  )
+
+
+@np.vectorize
+def _pl_without_sampling_remove(pl, sampling_prob):
+  return -_pl_without_sampling_add(-pl, sampling_prob)
+
+
+class MixtureGaussianPrivacyLoss(AdditiveNoisePrivacyLoss):
+  """Privacy loss of the Mixture of Gaussians mechanism.
+
+  This class gives the privacy loss for a scalar Gaussian mechanism where the
+  sensitivity is a random variable equal to sensitivities[i] with probability
+  sampling_probs[i].
+
+  The privacy loss distribution of the Mixture of Gaussians mechanism is
+  equivalent to the privacy loss distribution between the Gaussian distribution
+  and the same distribution convolved with the discrete distribution specified
+  by sensitivities and sampling_probs. That is, let mu be the Gaussian noise PDF
+  with sigma = standard_deviation. The privacy loss distribution is generated as
+  follows:
+  For ADD adjacency type:
+  - Let mu_lower(x) := sum over i of sampling_probs[i] *
+    mu(x - sensitivities[i])
+  - Sample x ~ mu_upper = mu and let the privacy loss be
+    ln(mu_upper(x) / mu_lower(x)).
+  For REMOVE adjacency type:
+  - Let mu_upper(x) := sum over i of sampling_probs[i] *
+    mu(x + sensitivities[i])
+  - Sample x ~ mu_lower = mu and let the privacy loss be
+    ln(mu_upper(x) / mu_lower(x)).
+
+  For example:
+    sensitivities = [1.0], sampling_probs = [1.0] captures the sensitivity-1
+      Gaussian mechanism.
+    sensitivities = [0.0, 1.0], sampling_probs = [0.9, 0.1] captures the
+      sensitivity-1 subsampled Gaussian mechanism with sampling probability
+      0.1.
+    sensitivities = [0.0, 1.0, 2.0], sampling_probs = [0.81, 0.18, 0.01]
+      captures a generalization of the subsampled Gaussian mechanism where
+      we can potentially sample the sensitive example twice, each time
+      with sampling probability 0.1.
+
+  This class can be used for vector-valued mechanisms via Corollary 4.7 from the
+  following paper:
+    Title: Privacy Amplification for Matrix Mechanisms
+    Authors: C. A. Choquette-Choo, A. Ganesh, T. Steinke, A. Thakurta
+    Link: https://arxiv.org/abs/2310.15526
+  In particular, this corollary shows the vector-valued mixture of Gaussians
+  mechanism is dominated by the scalar-valued mechanism given by replacing each
+  sensitivity vector with its norm.
+
+  For almost all methods (the exception is inverse_privacy_losses, for reasons
+  discussed in the docstring for that method), we reimplement the corresponding
+  method in GaussianPrivacyLoss, but with some minor changes to account for the
+  fact that this class is more general.
+
+  Attributes:
+    sensitivities: the support of the sensitivity distribution.
+    sampling_probs: the probabilities associated with the sensitivities.
+  """
+
+  def __init__(  # pylint: disable=super-init-not-called
+      self,
+      standard_deviation: float,
+      sensitivities: Sequence[float],
+      sampling_probs: Sequence[float],
+      pessimistic_estimate: bool = True,
+      log_mass_truncation_bound: float = -50,
+      adjacency_type: AdjacencyType = AdjacencyType.REMOVE,
+  ) -> None:
+    """Initializes the privacy loss of the MoG mechanism.
+
+    Args:
+      standard_deviation: The standard_deviation of the Gaussian distribution.
+      sensitivities: The support of the sensitivity distribution. Must be the
+        same length as sampling_probs, and both should be 1D.
+      sampling_probs: The probabilities associated with the sensitivities.
+      pessimistic_estimate: A value indicating whether the rounding is done in
+        such a way that the resulting epsilon-hockey stick divergence
+        computation gives an upper estimate to the real value.
+      log_mass_truncation_bound: The ln of the probability mass that might be
+        discarded from the noise distribution. The larger this number, the more
+        error it may introduce in divergence calculations.
+      adjacency_type: Type of adjacency relation to be used for defining the
+        privacy loss distribution.
+
+    Raises:
+      ValueError: If args are invalid, e.g. standard_deviation is negative or
+      sensitivities and sampling_probs are different lengths.
+    """
+    if standard_deviation <= 0:
+      raise ValueError(
+          'Standard deviation is not a positive real number: '
+          f'{standard_deviation}'
+      )
+    if log_mass_truncation_bound > 0:
+      raise ValueError(
+          'Log mass truncation bound is not a non-positive real '
+          f'number: {log_mass_truncation_bound}'
+      )
+    if len(sampling_probs) != len(sensitivities):
+      raise ValueError(
+          'sensitivities and sampling_probs must have the same '
+          f'length. Got {sampling_probs=} of length {len(sampling_probs)}, '
+          f'{sensitivities=} of length {len(sensitivities)}.'
+      )
+
+    non_zero_indices = np.asarray(sampling_probs) != 0.0
+    sensitivities = np.asarray(sensitivities)[non_zero_indices]
+    sampling_probs = np.asarray(sampling_probs)[non_zero_indices]
+    if np.any(sensitivities < 0):
+      raise ValueError(
+          f'Sensitivities contains a negative number: {sensitivities}.'
+      )
+    if sensitivities.max() == 0.0:
+      raise ValueError('Must have at least one positive sensitivity.')
+    if not math.isclose(sum(sampling_probs), 1):
+      raise ValueError(
+          f'Probabilities do not add up to 1: {sum(sampling_probs)}'
+      )
+    for sampling_prob in sampling_probs:
+      if sampling_prob <= 0 or sampling_prob > 1:
+        raise ValueError(
+            f'Sampling probability is not in (0,1] : {sampling_prob}'
+        )
+    self.discrete_noise = False
+    self.adjacency_type = adjacency_type
+    self.sampling_probs = sampling_probs
+    self.sensitivities = sensitivities
+    self._standard_deviation = standard_deviation
+    self._variance = standard_deviation**2
+    self._pessimistic_estimate = pessimistic_estimate
+    self._log_mass_truncation_bound = log_mass_truncation_bound
+
+    # Constant properties.
+    self._log_sampling_probs = np.log(self.sampling_probs)
+    self._pos_sampling_probs = self.sampling_probs[self.sensitivities > 0.0]
+    self._sampling_prob = np.clip(self._pos_sampling_probs.sum(), 0, 1)
+    nonzero_sens = self.sensitivities[self.sensitivities > 0.0]
+    self._min_sens = np.min(nonzero_sens)
+    self._max_sens = np.max(nonzero_sens)
+    self._gaussian_random_variable = stats.norm(scale=standard_deviation)
+
+  def mu_upper_cdf(
+      self, x: Union[float, Iterable[float]]
+  ) -> Union[float, np.ndarray]:
+    """Computes the cumulative density function of the mu_upper distribution.
+
+    For ADD adjacency type:
+      mu_upper(x) := mu
+    For REMOVE adjacency type:
+      mu_upper(x) := sum of sampling_probs[i] * mu(x + sensitivities[i])
+
+    Args:
+      x: the point or points at which the cumulative density function is to be
+        calculated.
+
+    Returns:
+      The cumulative density function of the mu_upper distribution at x, i.e.,
+      the probability that mu_upper is less than or equal to x.
+    """
+    if self.adjacency_type == AdjacencyType.ADD:
+      return self.noise_cdf(x)
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      points_per_sens = np.add.outer(np.atleast_1d(x), self.sensitivities)
+      output = (self.noise_cdf(points_per_sens) * self.sampling_probs).sum(
+          axis=1
+      )
+      if isinstance(x, numbers.Number):
+        return output[0]
+      else:
+        return output
+
+  def mu_lower_log_cdf(
+      self, x: Union[float, Iterable[float]]
+  ) -> Union[float, np.ndarray]:
+    """Computes log cumulative density function of the mu_lower distribution.
+
+    For ADD adjacency type:
+      mu_lower(x) := sum of sampling_probs[i] * mu(x - sensitivities[i])
+    For REMOVE adjacency type:
+      mu_lower(x) := mu
+
+    Args:
+      x: the point or points at which the log of the cumulative density function
+        is to be calculated.
+
+    Returns:
+      The log of the cumulative density function of the mu_lower distribution at
+      x, i.e., the log of the probability that mu_lower is less than or equal to
+      x.
+    """
+    if self.adjacency_type == AdjacencyType.ADD:
+      points_per_sens = np.add.outer(np.atleast_1d(x), -self.sensitivities)
+      logcdf_per_sens = self.noise_log_cdf(points_per_sens)
+      output = scipy.special.logsumexp(
+          logcdf_per_sens, axis=1, b=self.sampling_probs
+      )
+      if isinstance(x, numbers.Number):
+        return output[0]
+      else:
+        return output
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      return self.noise_log_cdf(x)
+
+  def get_delta_for_epsilon(
+      self, epsilon: Union[float, Sequence[float]]
+  ) -> Union[float, list[float]]:
+    """Computes the epsilon-hockey stick divergence of the mechanism.
+
+    Args:
+      epsilon: the epsilon, or list-like object of epsilon values, in
+        epsilon-hockey stick divergence. Should be non-decreasing if list-like.
+
+    Returns:
+      A non-negative real number which is the epsilon-hockey stick divergence of
+      the mechanism, or a numpy array if epsilon is list-like.
+    """
+    epsilons = np.atleast_1d(epsilon)
+    if not np.all(epsilons[1:] >= epsilons[:-1]):
+      raise ValueError(f'Epsilon values must be non-decreasing: {epsilons}')
+    deltas = np.zeros_like(epsilons, dtype=float)
+    if self._sampling_prob == 1.0:
+      inverse_indices = np.full_like(epsilons, True, dtype=bool)
+    elif self.adjacency_type == AdjacencyType.ADD:
+      inverse_indices = epsilons < -np.log1p(-self._sampling_prob)
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      inverse_indices = epsilons > np.log1p(-self._sampling_prob)
+      other_indices = np.logical_not(inverse_indices)
+      deltas[other_indices] = -np.expm1(epsilons[other_indices])
+    x_cutoffs = self.inverse_privacy_losses(epsilons[inverse_indices])
+    deltas[inverse_indices] = self.mu_upper_cdf(x_cutoffs) - np.exp(
+        epsilons[inverse_indices] + self.mu_lower_log_cdf(x_cutoffs)
+    )
+    # Clip delta values to lie in [0,1] (to avoid numerical errors)
+    deltas = np.clip(deltas, 0, 1)
+    if isinstance(epsilon, numbers.Number):
+      return float(deltas)
+    else:
+      # For numerical stability reasons, deltas may not be non-increasing. This
+      # is fixed post-hoc at small cost in accuracy.
+      for i in reversed(range(deltas.shape[0] - 1)):
+        deltas[i] = max(deltas[i], deltas[i + 1])
+      return deltas
+
+  def privacy_loss_tail(
+      self, precision: float = 1e-4
+  ) -> TailPrivacyLossDistribution:
+    """Computes the privacy loss at the tail of the random-sensitivity Gaussian.
+
+    For ADD adjacency type: The upper distribution is a single Gaussian and we
+      can exactly compute the tails easily.
+
+    For REMOVE adjacency type:  We set upper_x_truncation such that
+      CDF(upper_x_truncation) = 1 - 0.5 * exp(log_mass_truncation_bound). It is
+      worthwhile to spend some up-front computation getting a more precise value
+      for lower_x_truncation to save computation later on. So we binary search
+      over the interval [-upper_x_truncation - max(sensitivities),
+      -upper_x_truncation] for the point where the cdf of mu_upper is
+      0.5 * exp(log_mass_truncation_bound). Since we're binary searching over a
+      continuous domain, we proceed until the width of the binary search
+      interval is at most some small precision, and then set lower_x_truncation
+      to be the left endpoint of this interval.
+
+    Args:
+      precision: The additive error we will compute the truncation values
+        within. That is, when we binary search for log_mass_truncation_bound in
+        the REMOVE case, we terminate the binary search when the interval has
+        length at most precision, and then use the more conservative endpoint
+        of the interval as our truncation value.
+
+    Returns:
+      A TailPrivacyLossDistribution instance representing the tail of the
+      privacy loss distribution.
+    """
+    tail_mass = 0.5 * np.exp(self._log_mass_truncation_bound)
+    z_value = self._gaussian_random_variable.ppf(tail_mass)
+    upper_x_truncation = -z_value
+    if self.adjacency_type == AdjacencyType.ADD:
+      lower_x_truncation = z_value
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      lower_x_truncation = common.inverse_monotone_function(
+          self.mu_upper_cdf,
+          tail_mass,
+          common.BinarySearchParameters(
+              z_value - self._max_sens,
+              z_value,
+              tolerance=precision
+          ),
+          increasing=True,
+      )
+    if self._pessimistic_estimate:
+      tail_probability_mass_function = {
+          math.inf: self.mu_upper_cdf(lower_x_truncation),
+          self.privacy_loss(upper_x_truncation): 1 - self.mu_upper_cdf(
+              upper_x_truncation
+          ),
+      }
+    else:
+      tail_probability_mass_function = {
+          self.privacy_loss(lower_x_truncation): self.mu_upper_cdf(
+              lower_x_truncation
+          ),
+      }
+    return TailPrivacyLossDistribution(
+        lower_x_truncation, upper_x_truncation, tail_probability_mass_function
+    )
+
+  def connect_dots_bounds(self) -> ConnectDotsBounds:
+    """Computes the bounds on epsilon values to use in connect-the-dots algorithm.
+
+    Returns:
+      A ConnectDotsBounds instance containing upper and lower values of
+      epsilon to use in connect-the-dots algorithm.
+    """
+    tail_pld = self.privacy_loss_tail()
+
+    return ConnectDotsBounds(
+        epsilon_upper=self.privacy_loss(tail_pld.lower_x_truncation),
+        epsilon_lower=self.privacy_loss(tail_pld.upper_x_truncation),
+    )
+
+  @functools.cached_property
+  def _precompute_privacy_loss_constants(self) -> np.ndarray:
+    """(Pre-)computes the constants in the expression for the privacy loss."""
+    sens_loss = self.privacy_loss_for_single_gaussian(
+        np.repeat(0, len(self.sensitivities)), self.sensitivities
+    )
+    if self.adjacency_type == AdjacencyType.ADD:
+      return self._log_sampling_probs - sens_loss
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      return self._log_sampling_probs + sens_loss
+
+  def privacy_loss(self, x: float) -> float:
+    """Computes the privacy loss at a given point `x`."""
+    # Because this method is called many times, we opt to precompute as much
+    # as possible. It can be see that the computation below is equivalent to:
+    #
+    # x_rep = np.repeat(x, len(self.sensitivities))
+    # privacy_losses_without_subsampling = (
+    #     self.privacy_loss_for_single_gaussian(x_rep, self.sensitivities)
+    # )
+    # if self.adjacency_type == AdjacencyType.ADD:
+    #   summands = self._log_sampling_probs - privacy_losses_without_subsampling
+    #   return -np.logaddexp.reduce(summands)
+    #
+    # and similarly for .REMOVE.
+    x_loss = self.sensitivities * x / (self._variance)
+    if self.adjacency_type == AdjacencyType.ADD:
+      summands = self._precompute_privacy_loss_constants + x_loss
+      return -np.logaddexp.reduce(summands)
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      summands = self._precompute_privacy_loss_constants - x_loss
+      return np.logaddexp.reduce(summands)
+
+  def privacy_loss_without_subsampling(self, x: float) -> float:
+    raise NotImplementedError(
+        'MixtureGaussianPrivacyLoss uses multiple sensitivities, so '
+        'privacy loss without subsampling is ill-defined. Use '
+        'privacy_loss_for_single_gaussian instead.'
+    )
+
+  def privacy_loss_for_single_gaussian(
+      self,
+      x: Union[float, np.ndarray],
+      sensitivity: Union[float, np.ndarray] = 1.0
+  ) -> np.ndarray:
+    """Computes the privacy loss of the Gaussian mechanism.
+
+    Args:
+      x: the point(s) at which the privacy loss is computed.
+      sensitivity: The sensitivity/sensitivities of interest.
+
+    Returns:
+      The privacy loss of the Gaussian mechanism without sub-sampling at
+      point(s) x with the given sensitivity, which is given as
+      For ADD adjacency type:
+        sensitivity * (0.5 * sensitivity - x) / standard_deviation^2.
+      For REMOVE adjacency type:
+        sensitivity * (- 0.5 * sensitivity - x) / standard_deviation^2.
+    """
+    x = np.atleast_1d(x)
+    if self.adjacency_type == AdjacencyType.ADD:
+      scale = 0.5
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      scale = -0.5
+    return sensitivity * (scale * sensitivity - x) / (self._variance)
+
+  def inverse_privacy_loss_without_subsampling(
+      self, privacy_loss: float
+  ) -> float:
+    raise NotImplementedError(
+        'MixtureGaussianPrivacyLoss uses multiple sensitivities, so '
+        'inverse_privacy_loss_without_subsampling is ill-defined. Use '
+        'inverse_privacy_loss_for_single_gaussian instead.'
+    )
+
+  def inverse_privacy_loss_for_single_gaussian(
+      self,
+      privacy_loss: Union[float, np.ndarray],
+      sensitivity: Union[float, np.ndarray] = 1.0,
+  ) -> Union[float, np.ndarray]:
+    """Computes the inverse privacy loss for the Gaussian mechanism.
+
+    Args:
+      privacy_loss: the privacy loss value(s).
+      sensitivity: sensitivity/sensitivies of the Gaussian.
+
+    Returns:
+      The largest float(s) x such that the privacy loss at x is at least
+      privacy_loss. REMOVE is the same as ADD, minus sensitivity.
+    """
+    add_inverse_loss = (
+        0.5 * sensitivity - privacy_loss * (self._variance) / sensitivity
+    )
+    if self.adjacency_type == AdjacencyType.ADD:
+      return add_inverse_loss
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      return add_inverse_loss - sensitivity
+
+  def inverse_privacy_loss(
+      self, privacy_loss: float, precision: float = 1e-6
+  ) -> float:
+    """(Approximately) computes the inverse of a given privacy loss.
+
+    Technically, this method can be sped up by rewriting the logic in
+    inverse_privacy_losses to take advantage of the fact that we have a
+    single privacy loss rather than a list. However, this method is only written
+    to complete the abstract class, and the process of generating a PLD from
+    this class won't ever call this method. So, we have chosen the simple but
+    inefficient implementation of calling inverse_privacy_losses.
+
+    Args:
+      privacy_loss: the privacy loss value.
+      precision: Precision of the output.
+
+    Returns:
+      The largest float x such that the privacy loss at x is at least
+      privacy_loss, rounded down to the nearest multiple of precision if
+      we are using pessimistic estimates, and otherwise rounded up.
+    """
+    return float(
+        self.inverse_privacy_losses(np.atleast_1d(privacy_loss), precision)[0]
+    )
+
+  def inverse_privacy_losses(
+      self,
+      privacy_losses: np.ndarray,
+      precision: float = 1e-6,
+  ) -> np.ndarray:
+    """(Approximately) computes the inverse of a list of privacy losses.
+
+    Unlike subsampled Gaussians, for mixture Gaussians the privacy loss does
+    not have a closed-form inverse, to the best of our knowledge. So, we use
+    binary search. This is the main bottleneck in this library, so we optimize
+    it by doing one binary search for all values in privacy losses rather than a
+    separate binary search for each. This way, we avoid recomputing the privacy
+    loss at the same point across different binary searches.
+
+    Args:
+      privacy_losses: the privacy losses we wish to invert, in increasing order.
+      precision: Precision of the output. In particular, for each entry l in
+        privacy_losses, we output the smallest multiple of precision, x, such
+        that the privacy loss at x is at most l. This ensures (i) given a
+        monotonic privacy_losses, we return a monotonic list of xs, and (ii) the
+        approximation results in an overestimate of epsilon, i.e. the final
+        epsilon reported is valid.
+
+    Returns:
+      For each l in privacy_losses, the smallest multiple of precision, x, such
+      that the privacy loss at x is at most l.
+    """
+    if not (np.diff(privacy_losses) >= 0).all():
+      raise ValueError(
+          f'Expected non-decreasing privacy_losses, got: {privacy_losses}.'
+      )
+    if len(privacy_losses) == 0:  # pylint: disable=g-explicit-length-test
+      return np.ndarray([])
+
+    # If we have a non-zero probability of choosing sensitivity = 0, then the
+    # privacy loss does not take on all values in [-inf, inf], and so we need to
+    # make sure all values in privacy_losses are in the proper range for the
+    # given adjacency type.
+
+    # Some privacy losses might be close to the privacy loss at x = +/-inf, in
+    # which case we report the corresponding infinity for them.
+    min_pl = privacy_losses[0]
+    max_pl = privacy_losses[-1]
+    log_1m_prob = (
+        math.log1p(-self._sampling_prob) if self._sampling_prob < 1 else -np.inf
+    )
+    if self.adjacency_type == AdjacencyType.ADD:
+      if max_pl > -log_1m_prob:
+        raise ValueError(
+            f'max of privacy_losses ({max_pl}) is larger than '
+            f'-log(1 - sampling_prob)={-log_1m_prob}.'
+        )
+      finite_indices = np.logical_not(np.isclose(privacy_losses, -log_1m_prob))
+      max_pl = np.max(privacy_losses[finite_indices])
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      if min_pl <= log_1m_prob:
+        raise ValueError(
+            f'min of privacy_losses ({min_pl}) is smaller than '
+            f'log(1 - sampling_prob)={log_1m_prob}'
+        )
+      finite_indices = np.logical_not(np.isclose(privacy_losses, log_1m_prob))
+      min_pl = np.min(privacy_losses[finite_indices])
+
+    # Now, we need to determine a suitable range to binary search over. To do
+    # this, we consider the subsampled Gaussian mechanisms given by moving
+    # all the probability mass on non-zero sensitivities to either the
+    # smallest or largest sensitivity. We can show the privacy loss of the
+    # mixture is contained between these two mechanisms' privacy losses, and
+    # the subsampled Gaussian privacy loss is easy to invert. Then, we can
+    # compute the inverse privacy loss at min_pl and max_pl to get four
+    # candidate bounds, and take the min/max of these bounds.
+    loss_bounds = np.array([min_pl, min_pl, max_pl, max_pl])
+    sens_bounds = np.array([
+        self._min_sens,
+        self._max_sens,
+        self._min_sens,
+        self._max_sens,
+    ])
+    if self.adjacency_type == AdjacencyType.ADD:
+      pl_without_sampling = _pl_without_sampling_add
+    else:  # Case: self.adjacency_type == AdjacencyType.REMOVE
+      pl_without_sampling = _pl_without_sampling_remove
+
+    possible_bounds = self.inverse_privacy_loss_for_single_gaussian(
+        pl_without_sampling(loss_bounds, self._sampling_prob), sens_bounds
+    )
+    bounds = (
+        np.floor(np.min(possible_bounds) / precision) * precision,
+        np.ceil(np.max(possible_bounds) / precision) * precision,
+    )
+    if self.adjacency_type == AdjacencyType.ADD:
+      output = self.privacy_loss_for_single_gaussian(
+          np.full_like(privacy_losses, np.inf)
+      )
+    else:
+      output = self.privacy_loss_for_single_gaussian(
+          np.full_like(privacy_losses, -np.inf)
+      )
+    output[finite_indices] = self._inverse_privacy_losses_with_range(
+        privacy_losses[finite_indices], bounds, precision
+    )
+    return output
+
+  def _inverse_privacy_losses_with_range(
+      self,
+      privacy_losses: np.ndarray,
+      bounds: tuple[float, float],
+      precision: float = 1e-6,
+  ) -> Iterable[float]:
+    """Helper method for performing binary search in inverse_privacy_losses.
+
+    Args:
+      privacy_losses: the privacy losses we wish to invert.
+      bounds: Range to search over, i.e. the inverses are in the range
+        [bounds[0], bounds[1]].
+      precision: Precision of the output; in particular, for each entry l in
+        privacy_losses, we output the smallest multiple of precision, x, such
+        that the privacy loss at x is at most l. This ensures (i) given a
+        monotonic privacy_losses, we return a monotonic list of xs, and (ii) the
+        approximation results in an overestimate of epsilon, i.e. the final
+        epsilon we report is a valid epsilon.
+
+    Returns:
+      For each l in privacy_losses, the smallest multiple of precision, x, such
+      that the privacy loss at x is at most l.
+    """
+    if len(privacy_losses) == 0:  # pylint: disable=g-explicit-length-test
+      return []
+    if bounds[1] - bounds[0] <= precision:
+      return np.repeat(
+          np.floor(bounds[1] / precision) * precision, len(privacy_losses)
+      )
+
+    mid = (bounds[0] + bounds[1]) / 2
+    pl_split = self.privacy_loss(mid)
+    lower_indices = privacy_losses < pl_split
+    higher_indices = privacy_losses >= pl_split
+    output = np.zeros_like(privacy_losses)
+    output[lower_indices] = self._inverse_privacy_losses_with_range(
+        privacy_losses[lower_indices], (mid, bounds[1]), precision
+    )
+    output[higher_indices] = self._inverse_privacy_losses_with_range(
+        privacy_losses[higher_indices], (bounds[0], mid), precision
+    )
+    return output
+
+  def noise_cdf(
+      self, x: Union[float, Iterable[float]]
+  ) -> Union[float, np.ndarray]:
+    """Computes the cumulative density function of the Gaussian distribution.
+
+    Args:
+     x: the point or points at which the cumulative density function is to be
+       calculated.
+
+    Returns:
+      The cumulative density function of the Gaussian noise at x, i.e., the
+      probability that the Gaussian noise is less than or equal to x.
+    """
+    return self._gaussian_random_variable.cdf(x)
+
+  def noise_log_cdf(
+      self, x: Union[float, Iterable[float]]
+  ) -> Union[float, np.ndarray]:
+    """Computes log of cumulative density function of the Gaussian distribution.
+
+    Args:
+      x: the point or points at which the log cumulative density function is to
+        be calculated.
+
+    Returns:
+      The log cumulative density function of the Gaussian noise at x, i.e., the
+      log of the probability that the Gaussian noise is less than or equal to x.
+    """
+    return self._gaussian_random_variable.logcdf(x)
+
+  @classmethod
+  def from_privacy_guarantee(
+      cls,
+      privacy_parameters: common.DifferentialPrivacyParameters,
+      sensitivity: float = 1,
+      pessimistic_estimate: bool = True,
+      sampling_prob: float = 1.0,
+      adjacency_type: AdjacencyType = AdjacencyType.REMOVE,
+  ) -> 'MixtureGaussianPrivacyLoss':
+    raise NotImplementedError(
+        'MixtureGaussianPrivacy loss cannot be uniquely '
+        'instantiated from privacy parameters.'
+    )
```

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/test_util.py` & `dp_accounting-0.4.4/dp_accounting/pld/test_util.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.3/dp_accounting/pld/test_util_test.py` & `dp_accounting-0.4.4/dp_accounting/pld/test_util_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for test_util."""
 
 import unittest
+
 from absl.testing import parameterized
 
 from dp_accounting.pld import test_util
 
 
 class TestUtilTest(parameterized.TestCase):
```

### Comparing `dp-accounting-0.4.3/dp_accounting/privacy_accountant.py` & `dp_accounting-0.4.4/dp_accounting/privacy_accountant.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.3/dp_accounting/privacy_accountant_test.py` & `dp_accounting-0.4.4/dp_accounting/privacy_accountant_test.py`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.3/dp_accounting/rdp/__init__.py` & `dp_accounting-0.4.4/dp_accounting/pld/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,11 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""RDP Accounting package."""
+"""PLD Accounting package."""
 
-from dp_accounting.rdp.rdp_privacy_accountant import compute_epsilon
-from dp_accounting.rdp.rdp_privacy_accountant import RdpAccountant
+from dp_accounting.pld import accountant
+from dp_accounting.pld import common
+from dp_accounting.pld import pld_pmf
+from dp_accounting.pld import pld_privacy_accountant
+from dp_accounting.pld import privacy_loss_distribution
+from dp_accounting.pld import privacy_loss_mechanism
+from dp_accounting.pld.pld_privacy_accountant import PLDAccountant
```

### Comparing `dp-accounting-0.4.3/dp_accounting/rdp/rdp_privacy_accountant.py` & `dp_accounting-0.4.4/dp_accounting/rdp/rdp_privacy_accountant.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Privacy accountant that uses Renyi differential privacy."""
 
 import math
 from typing import Callable, Optional, Sequence, Tuple, Union
 
+from absl import logging
 import numpy as np
 from scipy import special
 
 from dp_accounting import dp_event
 from dp_accounting import privacy_accountant
 
 NeighborRel = privacy_accountant.NeighboringRelation
@@ -34,96 +35,74 @@
   a, b = min(logx, logy), max(logx, logy)
   if a == -np.inf:  # adding 0
     return b
   # Use exp(a) + exp(b) = (exp(a - b) + 1) * exp(b)
   return math.log1p(math.exp(a - b)) + b  # log1p(x) = log(x + 1)
 
 
-def _log_sub(logx: float, logy: float) -> float:
-  """Subtracts two numbers in the log space. Answer must be non-negative."""
-  if logx < logy:
-    raise ValueError('The result of subtraction must be non-negative.')
-  if logy == -np.inf:  # subtracting 0
-    return logx
-  if logx == logy:
-    return -np.inf  # 0 is represented as -np.inf in the log space.
-
-  try:
-    # Use exp(x) - exp(y) = (exp(x - y) - 1) * exp(y).
-    return math.log(math.expm1(logx - logy)) + logy  # expm1(x) = exp(x) - 1
-  except OverflowError:
-    return logx
-
-
 def _log_sub_sign(logx: float, logy: float) -> Tuple[bool, float]:
   """Returns log(exp(logx)-exp(logy)) and its sign."""
   if logx > logy:
     s = True
-    mag = logx + np.log(1 - np.exp(logy - logx))
+    mag = logx + math.log1p(-np.exp(logy - logx))
   elif logx < logy:
     s = False
-    mag = logy + np.log(1 - np.exp(logx - logy))
+    mag = logy + np.log1p(-np.exp(logx - logy))
   else:
     s = True
     mag = -np.inf
 
   return s, mag
 
 
-def _log_comb(n: int, k: int) -> float:
+def _log_comb(n: float, k: float) -> float:
   """Computes log of binomial coefficient."""
   return (special.gammaln(n + 1) - special.gammaln(k + 1) -
           special.gammaln(n - k + 1))
 
 
 def _compute_log_a_int(q: float, sigma: float, alpha: int) -> float:
   """Computes log(A_alpha) for integer alpha, 0 < q < 1."""
 
   # Initialize with 0 in the log space.
   log_a = -np.inf
+  log1mq = math.log1p(-q)
 
   for i in range(alpha + 1):
-    log_coef_i = (
-        _log_comb(alpha, i) + i * math.log(q) + (alpha - i) * math.log(1 - q))
-
+    log_coef_i = _log_comb(alpha, i) + i * math.log(q) + (alpha - i) * log1mq
     s = log_coef_i + (i * i - i) / (2 * (sigma**2))
     log_a = _log_add(log_a, s)
 
-  return float(log_a)
+  return log_a
 
 
 def _compute_log_a_frac(q: float, sigma: float, alpha: float) -> float:
   """Computes log(A_alpha) for fractional alpha, 0 < q < 1."""
   # The two parts of A_alpha, integrals over (-inf,z0] and [z0, +inf), are
   # initialized to 0 in the log space:
   log_a0, log_a1 = -np.inf, -np.inf
-  i = 0
-
   z0 = sigma**2 * math.log(1 / q - 1) + .5
+  log1mq = math.log1p(-q)
 
+  i = 0
   while True:  # do ... until loop
-    coef = special.binom(alpha, i)
-    log_coef = math.log(abs(coef))
+    log_coef = _log_comb(alpha, i)
     j = alpha - i
 
-    log_t0 = log_coef + i * math.log(q) + j * math.log(1 - q)
-    log_t1 = log_coef + j * math.log(q) + i * math.log(1 - q)
+    log_t0 = log_coef + i * math.log(q) + j * log1mq
+    log_t1 = log_coef + j * math.log(q) + i * log1mq
 
     log_e0 = math.log(.5) + _log_erfc((i - z0) / (math.sqrt(2) * sigma))
     log_e1 = math.log(.5) + _log_erfc((z0 - j) / (math.sqrt(2) * sigma))
 
     log_s0 = log_t0 + (i * i - i) / (2 * (sigma**2)) + log_e0
     log_s1 = log_t1 + (j * j - j) / (2 * (sigma**2)) + log_e1
 
-    if coef > 0:
-      log_a0 = _log_add(log_a0, log_s0)
-      log_a1 = _log_add(log_a1, log_s1)
-    else:
-      log_a0 = _log_sub(log_a0, log_s0)
-      log_a1 = _log_sub(log_a1, log_s1)
+    log_a0 = _log_add(log_a0, log_s0)
+    log_a1 = _log_add(log_a1, log_s1)
 
     i += 1
     if max(log_s0, log_s1) < -30:
       break
 
   return _log_add(log_a0, log_a1)
 
@@ -173,19 +152,24 @@
 
   # Improved bound from https://arxiv.org/abs/2004.00010 Proposition 12 (in v4):
   logdeltas = []  # work in log space to avoid overflows
   for (a, r) in zip(orders, rdp):
     if a < 1:
       raise ValueError(f'Renyi divergence order must be at least 1. Found {a}.')
     if r < 0:
-      raise ValueError(f'Renyi divergence cannot be negative. Found {r}.')
+      logging.warning(
+          'Negative Renyi divergence of %s, probably caused by numerical '
+          'instability from extreme DpEvents. Returning a delta of zero.',
+          r,
+      )
+      logdelta = -np.inf
     # For small alpha, we are better of with bound via KL divergence:
     # delta <= sqrt(1-exp(-KL)).
     # Take a min of the two bounds.
-    if r == 0:
+    elif r == 0:
       logdelta = -np.inf
     else:
       logdelta = 0.5 * math.log1p(-math.exp(-r))
     if a > 1.01:
       # This bound is not numerically stable as alpha->1.
       # Thus we have a min value for alpha.
       # The bound is also not useful for small alpha, so doesn't matter.
@@ -233,17 +217,21 @@
   # Improved bound from https://arxiv.org/abs/2004.00010 Proposition 12 (in v4).
   # Also appears in https://arxiv.org/abs/2001.05990 Equation 20 (in v1).
   eps = []
   for (a, r) in zip(orders, rdp):
     if a < 1:
       raise ValueError(f'Renyi divergence order must be at least 1. Found {a}.')
     if r < 0:
-      raise ValueError(f'Renyi divergence cannot be negative. Found {r}.')
-
-    if delta**2 + math.expm1(-r) > 0:
+      logging.warning(
+          'Negative Renyi divergence of %s, probably caused by numerical '
+          'instability from extreme DpEvents. Returning an epsilon of zero.',
+          r,
+      )
+      epsilon = 0.0
+    elif delta**2 + math.expm1(-r) > 0:
       # In this case, we can simply bound via KL divergence:
       # delta <= sqrt(1-exp(-KL)).
       epsilon = 0  # No need to try further computation if we have epsilon = 0.
     elif a > 1.01:
       # This bound is not numerically stable as alpha->1.
       # Thus we have a min value of alpha.
       # The bound is also not useful for small alpha, so doesn't matter.
@@ -464,28 +452,27 @@
   def func(x):
     # Return the rdp of Gaussian mechanism
     return 1.0 * x / (2.0 * sigma**2)
 
   # Initialize with 1 in the log space.
   log_a = 0
   # Calculates the log term when alpha = 2
-  log_f2m1 = func(2.0) + np.log(1 - np.exp(-func(2.0)))
+  log_f2m1 = func(2.0) + math.log1p(-np.exp(-func(2.0)))
   if alpha <= max_alpha:
     # We need forward differences of exp(cgf)
     # The following line is the numerically stable way of implementing it.
     # The output is in polar form with logarithmic magnitude
     deltas, _ = _get_forward_diffs(cgf, alpha)
     # Compute the bound exactly requires book keeping of O(alpha**2)
-
     for i in range(2, alpha + 1):
       if i == 2:
         s = 2 * np.log(q) + _log_comb(alpha, 2) + np.minimum(
             np.log(4) + log_f2m1,
             func(2.0) + np.log(2))
-      elif i > 2:
+      else:  # i > 2
         delta_lo = deltas[int(2 * np.floor(i / 2.0)) - 1]
         delta_hi = deltas[int(2 * np.ceil(i / 2.0)) - 1]
         s = np.log(4) + 0.5 * (delta_lo + delta_hi)
         s = np.minimum(s, np.log(2) + cgf(i - 1))
         s += i * np.log(q) + _log_comb(alpha, i)
       log_a = _log_add(log_a, s)
     return float(log_a)
@@ -772,14 +759,53 @@
     # We can use this to bound rdp for low orders.
     for i in range(len(orders)):
       rdp_out[i] = min(
           rdp_out[j] for j in range(len(orders)) if orders[i] <= orders[j])
   return rdp_out
 
 
+def _laplace_rdp(eps: float, order: float) -> float:
+  """Computes RDP of Laplace noise addition.
+
+  See Proposition 6 of Mironov (2017): https://arxiv.org/abs/1702.07476
+  RDP = eps + log[ 1 + (a-1) * [exp( (1-2*a) * eps) - 1] / (2*a-1) ] / (a-1).
+  In contrast, the naive bound is RDP <= eps, which is tight as order->infinity.
+  For small order & eps, we can do better: In general, RDP <= order * eps^2 / 2.
+  The above formula is exactly tight for the Laplace mechanism.
+
+  Args:
+    eps: The pure DP guarantee corresponding to the limit order->infinity.
+    order: The Renyi divergence order (a.k.a. alpha).
+
+  Returns:
+    The RDP of Laplace noise addition
+  """
+  a = float(order)
+  eps = float(eps)
+  if not math.isfinite(eps) or eps < 0:
+    raise ValueError(f'eps must be > 0. Got {eps}')
+  if not math.isfinite(a) or a < 1:
+    raise ValueError(f'order must be >= 1. Got {a}')
+
+  if a == 1:  # KL divergence
+    # Taking the limit as order->1 gives the following expression.
+    return eps + math.expm1(-eps)
+  elif a < 1.1:  # 1 < order <= 1.1
+    # For numerical stability in this case, we use a Taylor series.
+    # log(1+x) = sum_{k>=1} -(-x)^k/k
+    # Thus log(1+c*x)/x = c * sum_{k>=1} (-c*x)^{k-1}/k
+    # Since 0 <= -c*x <= 0.1, this Taylor series converges rapidly.
+    c = math.expm1(eps * (1 - 2 * a)) / (2 * a - 1)
+    v = -c * (a - 1)
+    return eps + c * math.fsum(v**(k - 1) / k for k in range(1, 100))
+  else:  # order > 1.1
+    return eps + math.log1p(
+        (a - 1) * math.expm1(eps * (1 - 2 * a)) / (2 * a - 1)
+    ) / (a - 1)
+
 # Default orders chosen to give good coverage for Gaussian mechanism in
 # the privacy regime of interest.
 DEFAULT_RDP_ORDERS = ([1 + x / 10. for x in range(1, 100)] +
                       list(range(11, 64)) + [128, 256, 512, 1024])
 
 
 class RdpAccountant(privacy_accountant.PrivacyAccountant):
@@ -876,28 +902,25 @@
             invalid_event=event, error_message=error_msg)
       if do_compose:
         self._rdp += count * _compute_rdp_single_epoch_tree_aggregation(
             event.noise_multiplier, event.step_counts, self._orders)
       return None
     elif isinstance(event, dp_event.LaplaceDpEvent):
       if do_compose:
-        # Laplace satisfies eps-DP with eps = 1 / event.noise_multiplier
-        # eps-DP implies (alpha, min(eps,alpha*eps^2/2))-RDP for all alpha.
         eps = 1 / event.noise_multiplier
-        rho = 0.5 * eps * eps
         self._rdp += count * np.array(
-            [min(eps, rho * order) for order in self._orders])
+            [_laplace_rdp(eps, order) for order in self._orders])
       return None
     elif isinstance(event, dp_event.RepeatAndSelectDpEvent):
+      save_rdp = self._rdp
       if do_compose:
         # Save the RDP values from already composed DPEvents. These will
         # be added back after we process this RepeatAndSelectDpEvent.
         # Zero out self._rdp before computing the RDP of the underlying
         # DP event.
-        save_rdp = self._rdp
         self._rdp = np.zeros_like(self._orders, dtype=np.float64)
       composition_error = self._maybe_compose(event.event, 1, do_compose)
       if composition_error is None and do_compose:
         self._rdp = count * _compute_rdp_repeat_and_select(
             self._orders, self._rdp, event.mean, event.shape) + save_rdp
       return composition_error
     else:
```

### Comparing `dp-accounting-0.4.3/dp_accounting/rdp/rdp_privacy_accountant_test.py` & `dp_accounting-0.4.4/dp_accounting/rdp/rdp_privacy_accountant_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,38 +259,49 @@
   def test_compute_rdp_poisson_sampled_gaussian(self):
     orders = [1.5, 2.5, 5, 50, 100, np.inf]
     noise_multiplier = 2.5
     sampling_probability = 0.01
     count = 50
     event = dp_event.SelfComposedDpEvent(
         dp_event.PoissonSampledDpEvent(
-            sampling_probability, dp_event.GaussianDpEvent(noise_multiplier)),
-        count)
+            sampling_probability, dp_event.GaussianDpEvent(noise_multiplier)
+        ),
+        count,
+    )
     accountant = rdp_privacy_accountant.RdpAccountant(orders=orders)
     accountant.compose(event)
     self.assertTrue(
         np.allclose(
-            accountant._rdp, [
-                6.5007e-04, 1.0854e-03, 2.1808e-03, 2.3846e-02, 1.6742e+02,
-                np.inf
+            accountant._rdp,
+            [
+                6.70579741e-04,
+                1.08548710e-03,
+                2.18075656e-03,
+                2.38460375e-02,
+                1.67416308e02,
+                np.inf,
             ],
-            rtol=1e-4))
+            rtol=1e-4,
+        )
+    )
 
   def test_compute_epsilon_delta_pure_dp(self):
     orders = range(2, 33)
-    rdp = [1.1 for o in orders]  # Constant corresponds to pure DP.
+    rdp = [1.1 for _ in orders]  # Constant corresponds to pure DP.
 
     epsilon, optimal_order = rdp_privacy_accountant.compute_epsilon(
-        orders, rdp, delta=1e-5)
+        orders, rdp, delta=1e-5
+    )
     # Compare with epsilon computed by hand.
     self.assertAlmostEqual(epsilon, 1.32783806176)
     self.assertEqual(optimal_order, 32)
 
     delta, optimal_order = rdp_privacy_accountant.compute_delta(
-        orders, rdp, epsilon=1.32783806176)
+        orders, rdp, epsilon=1.32783806176
+    )
     self.assertAlmostEqual(delta, 1e-5)
     self.assertEqual(optimal_order, 32)
 
   def test_compute_epsilon_delta_gaussian(self):
     orders = [0.001 * i for i in range(1000, 100000)]
 
     # noise multiplier is chosen to obtain exactly (1,1e-6)-DP.
@@ -348,15 +359,15 @@
   # pylint:disable=undefined-variable
   @parameterized.parameters(p for p in params)
   def test_compute_log_a_equals_mp(self, q, sigma, order):
     # Compare the cheap computation of log(A) with an expensive, multi-precision
     # computation.
     log_a = rdp_privacy_accountant._compute_log_a(q, sigma, order)
     log_a_mp = _log_float_mp(_compute_a_mp(sigma, q, order))
-    np.testing.assert_allclose(log_a, log_a_mp, rtol=1e-4)
+    np.testing.assert_allclose(log_a, log_a_mp, rtol=1e-4, atol=1e-8)
 
   def test_delta_bounds_gaussian(self):
     # Compare the optimal bound for Gaussian with the one derived from RDP.
     # Also compare the RDP upper bound with the "standard" upper bound.
     orders = [0.1 * x for x in range(10, 505)]
     eps_vec = [0.1 * x for x in range(500)]
     rdp = rdp_privacy_accountant._compute_rdp_poisson_subsampled_gaussian(
@@ -483,27 +494,32 @@
     base_rdp = accountant._rdp
     self.assertTrue(np.allclose(tree_rdp, base_rdp, rtol=1e-12))
 
   @parameterized.named_parameters(
       ('small_eps', 0.01, 1),
       ('medium_eps', 1.0, 1),
       ('large_eps', 100.0, 1),
-      ('repetition', 1.0, 100)
+      ('repetition', 1.0, 100),
   )
   def test_laplace(self, eps, count):
-    event = dp_event.LaplaceDpEvent(1/eps)
+    event = dp_event.LaplaceDpEvent(1 / eps)
     if count != 1:
       event = dp_event.SelfComposedDpEvent(event, count)
     # Simulate Pure DP by using a large Renyi order.
-    accountant = rdp_privacy_accountant.RdpAccountant(orders=[1.0, 1e10])
+    accountant = rdp_privacy_accountant.RdpAccountant(
+        orders=[1.0, 1 + 1e-6, 1.1 - 1e-6, 1.1 + 1e-6, 1e10]
+    )
     accountant.compose(event)
     # Check basic composition by having small delta.
     self.assertAlmostEqual(accountant.get_epsilon(1e-10), eps * count)
     # Check KL divergence, a.k.a. expected privacy loss, a.k.a. order=1.
-    self.assertAlmostEqual(accountant._rdp[0], min(eps, eps*eps/2) * count)
+    self.assertLessEqual(accountant._rdp[0], min(eps, eps * eps / 2) * count)
+    # Check consistency between the three formulas.
+    self.assertAlmostEqual(accountant._rdp[0], accountant._rdp[1], places=3)
+    self.assertAlmostEqual(accountant._rdp[2], accountant._rdp[3], places=3)
 
   # The function _truncated_negative_binomial_mean computes the mean in
   # multiple ways to ensure numerical stability.
   # This test checks that those different ways of computing are consistent.
   @parameterized.named_parameters(
       ('gamma_shape0', 0.9, 0, 0.9 - 1e-9, 0),
       ('gamma_shape2', 0.9, 2, 0.9 - 1e-9, 2),
@@ -646,26 +662,33 @@
 
   @parameterized.named_parameters(
       ('mean1', 1, 1),
       ('mean2', 0.1, 2),
       ('mean10', 10, 10),
       ('mean100', 0.001, 100),
       ('mean10^4', 2, 1000),
-      ('mean10^10', 1, 1e10)
+      ('mean10^10', 1, 1e10),
   )
   def test_repeat_and_select_pure_poisson(self, eps, mean):
-    event = dp_event.LaplaceDpEvent(1/eps)
+    event = dp_event.LaplaceDpEvent(1 / eps)
     event = dp_event.RepeatAndSelectDpEvent(event, mean, np.inf)
-    alpha = 1 + 1/math.expm1(eps)
-    orders = [alpha, 1e10, 1e100, 1e1000]
+    alpha = 1 + 1 / math.expm1(eps)
+    orders = [alpha, 1e10, 1e100]
     accountant = rdp_privacy_accountant.RdpAccountant(orders=orders)
     accountant.compose(event)
-    ans = min(eps, alpha*eps**2/2) + math.log(mean) * math.expm1(eps)
+    ans = (
+        eps
+        + math.log1p(
+            math.expm1((1 - 2 * alpha) * eps) * (alpha - 1) / (2 * alpha - 1)
+        )
+        / (alpha - 1)
+        + math.log(mean) * math.expm1(eps)
+    )
     self.assertAlmostEqual(accountant._orders[0], alpha)
-    self.assertAlmostEqual(accountant._rdp[0], ans)
+    self.assertAlmostEqual(accountant._rdp[0] / ans, 1, places=3)
 
 
 @parameterized.named_parameters(
     ('small_small', 0.001, 1),
     ('small_med', 0.001, 1000),
     ('small_large', 0.001, 1e9),
     ('med_small', 1, 1),
```

### Comparing `dp-accounting-0.4.3/dp_accounting.egg-info/PKG-INFO` & `dp_accounting-0.4.4/dp_accounting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dp-accounting
-Version: 0.4.3
+Version: 0.4.4
 Summary: Tools for tracking differential privacy budgets
 Home-page: https://github.com/google/differential-privacy/
 Author: Google Differential Privacy Team
 Author-email: dp-open-source@google.com
 License: Apache 2.0
 Keywords: differential-privacy accounting
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `dp-accounting-0.4.3/dp_accounting.egg-info/SOURCES.txt` & `dp_accounting-0.4.4/dp_accounting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dp-accounting-0.4.3/setup.py` & `dp_accounting-0.4.4/setup.py`

 * *Files identical despite different names*

