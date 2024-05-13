# Comparing `tmp/tempit-0.1.3.tar.gz` & `tmp/tempit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempit-0.1.3.tar", last modified: Sun May 12 18:33:39 2024, max compression
+gzip compressed data, was "tempit-0.1.4.tar", last modified: Mon May 13 08:54:15 2024, max compression
```

## Comparing `tempit-0.1.3.tar` & `tempit-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:33:39.152836 tempit-0.1.3/
--rw-r--r--   0 mcrespo    (501) staff       (20)     1068 2024-05-11 14:15:52.000000 tempit-0.1.3/LICENSE.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)     3748 2024-05-12 18:33:39.152625 tempit-0.1.3/PKG-INFO
--rw-r--r--   0 mcrespo    (501) staff       (20)     3128 2024-05-12 10:42:15.000000 tempit-0.1.3/README.md
--rw-r--r--   0 mcrespo    (501) staff       (20)       38 2024-05-12 18:33:39.152878 tempit-0.1.3/setup.cfg
--rw-r--r--   0 mcrespo    (501) staff       (20)      839 2024-05-12 18:31:57.000000 tempit-0.1.3/setup.py
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:33:39.151474 tempit-0.1.3/tempit/
--rw-r--r--   0 mcrespo    (501) staff       (20)       47 2024-05-11 14:15:52.000000 tempit-0.1.3/tempit/__init__.py
--rw-r--r--   0 mcrespo    (501) staff       (20)     9442 2024-05-12 18:10:08.000000 tempit-0.1.3/tempit/core.py
--rw-r--r--   0 mcrespo    (501) staff       (20)     5353 2024-05-12 10:36:44.000000 tempit-0.1.3/tempit/utils.py
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:33:39.152413 tempit-0.1.3/tempit.egg-info/
--rw-r--r--   0 mcrespo    (501) staff       (20)     3748 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/PKG-INFO
--rw-r--r--   0 mcrespo    (501) staff       (20)      250 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/SOURCES.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)        1 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/dependency_links.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/requires.txt
--rw-r--r--   0 mcrespo    (501) staff       (20)        7 2024-05-12 18:33:39.000000 tempit-0.1.3/tempit.egg-info/top_level.txt
-drwxr-xr-x   0 mcrespo    (501) staff       (20)        0 2024-05-12 18:33:39.152224 tempit-0.1.3/tests/
--rw-r--r--   0 mcrespo    (501) staff       (20)    12230 2024-05-12 18:04:54.000000 tempit-0.1.3/tests/test_tempit.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:54:15.596791 tempit-0.1.4/
+-rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     5000 2024-05-13 08:54:15.595785 tempit-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4341 2024-05-13 07:52:51.000000 tempit-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:54:15.597785 tempit-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-13 07:54:34.000000 tempit-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:54:15.571436 tempit-0.1.4/tempit/
+-rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.4/tempit/__init__.py
+-rw-rw-rw-   0        0        0     9656 2024-05-13 06:36:00.000000 tempit-0.1.4/tempit/core.py
+-rw-rw-rw-   0        0        0     5498 2024-05-10 06:26:45.000000 tempit-0.1.4/tempit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:54:15.592773 tempit-0.1.4/tempit.egg-info/
+-rw-rw-rw-   0        0        0     5000 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 08:54:15.000000 tempit-0.1.4/tempit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:54:15.591153 tempit-0.1.4/tests/
+-rw-rw-rw-   0        0        0    12577 2024-05-13 08:25:53.000000 tempit-0.1.4/tests/test_tempit.py
```

### Comparing `tempit-0.1.3/LICENSE.txt` & `tempit-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tempit-0.1.3/PKG-INFO` & `tempit-0.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,123 +1,150 @@
-Metadata-Version: 2.1
-Name: tempit
-Version: 0.1.3
-Summary: A dead simple time decorator
-Home-page: https://github.com/mcrespoae/tempit
-Author: mcrespoae
-Author-email: info@mariocrespo.es
-Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: joblib
-
-# Tempit
-
-Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
-
-## Installation
-
-You can install Tempit using pip:
-
-```bash
-pip install tempit
-```
-
-## Usage
-
-Below are some examples demonstrating Tempit's usage:
-
-### Basic Usage
-
-```python
-from tempit import tempit
-
-@tempit
-def my_function():
-    # Normal code of your function
-    pass
-
-my_function()
-```
-
-This will output something like:
-
-```text
-Function my_function took 10.5908ms.
-```
-
-### Advanced Usage
-
-```python
-from tempit import tempit
-@tempit(run_times=20, concurrent_execution=True, verbose=True)
-def my_function_with_args(a:int = 1, b:int = 2):
-    return a + b
-
-result = my_function_with_args(1, b=2)
-```
-
-This will provide detailed output:
-
-```text
-***** tempit data for function my_function_with_args: *****
-Function name: my_function_with_args
-        Funcion object: <function my_function_with_args at 0x0000000000000000>
-        Args: (1,)
-        Kwargs: {'b': 2}
-        Run times: 20
-        Mean: 0.7000µs
-        Median: 0.8000µs
-        Min: 0.4000µs
-        Max: 1.0000µs
-        Standard deviation: 0.2828µs
-        Sum time: 3.5000µs
-        Real time: 965.1000µs
-***** End of tempit data. *****
-```
-
-More examples can be found in the [examples.py](examples/examples.py) script.
-
-## Features
-
-- Simplified usage.
-- Accurate measurement of function execution time.
-- Support for `classmethod` and `staticmethods`.
-- Parallel execution mode for performance measurement.
-- Human-readable time formatting.
-- Optional verbose mode for detailed information.
-
-## Parameters
-
-Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
-
-- `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
-- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
-- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
-
-## Contributing
-
-Contributions are welcome! Please follow these guidelines when contributing:
-
-1. Fork the repository.
-2. Create a new branch for your changes.
-3. Implement your changes and commit them.
-4. Push your changes to your forked repository.
-5. Submit a pull request.
-
-## Testing
-
-The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](tests) and can be executed using `make test`.
-
-## License
-
-This project is licensed under the [MIT License](LICENSE.txt).
-
-## Contributors
-
-- [Mario Crespo](https://github.com/mcrespoae)
+Metadata-Version: 2.1
+Name: tempit
+Version: 0.1.4
+Summary: A dead simple time decorator
+Home-page: https://github.com/mcrespoae/tempit
+Author: mcrespoae
+Author-email: info@mariocrespo.es
+Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: joblib==1.4.2
+
+# Tempit
+
+Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
+
+## Installation
+
+You can install Tempit using pip:
+
+```bash
+pip install tempit
+```
+
+## Usage
+
+Below are some examples demonstrating Tempit's usage:
+
+### Basic Usage
+
+```python
+from tempit import tempit
+
+@tempit
+def my_function():
+    # Normal code of your function
+    pass
+
+my_function()
+```
+
+This will output something like:
+
+```text
+Function my_function took 10.5908ms.
+```
+
+### Advanced Usage
+
+```python
+from tempit import tempit
+@tempit(run_times=20, concurrent_execution=True, verbose=True)
+def my_function_with_args(a:int = 1, b:int = 2):
+    return a + b
+
+result = my_function_with_args(1, b=2)
+```
+
+This will provide detailed output:
+
+```text
+***** tempit data for function my_function_with_args: *****
+Function name: my_function_with_args
+        Funcion object: <function my_function_with_args at 0x0000000000000000>
+        Args: (1,)
+        Kwargs: {'b': 2}
+        Run times: 20
+        Mean: 0.7000Âµs
+        Median: 0.8000Âµs
+        Min: 0.4000Âµs
+        Max: 1.0000Âµs
+        Standard deviation: 0.2828Âµs
+        Sum time: 3.5000Âµs
+        Real time: 965.1000Âµs
+***** End of tempit data. *****
+```
+
+More examples can be found in the [examples.py](examples/examples.py) script.
+
+## Features
+
+- Simplified usage.
+- Accurate measurement of function execution time.
+- Support for `classmethod` and `staticmethods`.
+- Parallel execution mode for performance measurement.
+- Human-readable time formatting.
+- Optional verbose mode for detailed information.
+
+## Parameters
+
+Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
+
+- `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
+- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
+- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
+
+## Note with recursive functions
+
+This package doesn't work well with recursive functions. The specific reason and limitation are that using recursive functions with this package may result in very verbose output, making it difficult to read, especially for larger values.
+
+To avoid this issue, you can encapsulate the recursive function within another function and call it without printing messages. Here's an example:
+
+```python
+@tempit
+def encapsulated_recursive_function(n):
+    """A non-verbose wrapper for the recursive function."""
+    def recursive_func(n):
+        if n == 0:
+            return 0
+        else:
+            return n + recursive_func(n - 1)
+
+    return recursive_func(n)
+
+# Using the encapsulated recursive function
+result = encapsulated_recursive_function(3)
+```
+
+This approach makes the output cleaner and easier to read, especially when dealing with recursive functions with many calls.
+
+## Contributing
+
+Contributions are welcome! Please follow these guidelines when contributing:
+
+1. Fork the repository.
+2. Use `make install` to install all depedencies.
+3. Create a new branch for your changes.
+4. Implement your changes and commit them.
+5. Push your changes to your forked repository.
+6. Submit a pull request.
+
+You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](Makefile) to know more about commands.
+
+## Testing
+
+The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](tests).
+
+## License
+
+This project is licensed under the [MIT License](LICENSE.txt).
+
+## Contributors
+
+- [Mario Crespo](https://github.com/mcrespoae)
```

### Comparing `tempit-0.1.3/tempit/core.py` & `tempit-0.1.4/tempit/core.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-import time
-from functools import partial, wraps
-from typing import Any, Callable, Dict, List, Tuple
-
-from .utils import print_tempit_values
-
-
-def tempit(*args: Any, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False) -> Callable:
-    """
-    Decorator function that measures the execution time of a given function. It can be called like @tempit or using arguments @tempit(...)
-
-    Args:
-        args: contains the function to be decorated if no arguments are provided when calling the decorator
-        run_times (int, optional): The number of times the function should be executed. Defaults to 1.
-        concurrent_execution (bool, optional): This parameter will allow for the concurrent execution of the function using joblib.
-                                               The default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading.
-                                               If the execution of the concurrency fails, it will try to execute the func run_times non concurrently in the main process.
-                                               Defaults to True.
-        verbose (bool, optional): Whether to print detailed information after execution. Defaults to False.
-
-    Returns:
-        Callable: The decorated function if arguments are provided, otherwise a partial function.
-
-    Raises:
-        RuntimeError: If the concurrency mode fails, the function is executed in the main process.
-
-    Notes:
-        - If `run_times` is less than 1, it will be set to 1.
-        - If the function is a method, the first argument will be removed from `args_to_print`.
-        - If the function is a class method, the first argument will be replaced with the class itself.
-        - If the function is a static method, the first argument will be removed.
-
-    Example:
-        @tempit(run_times=5, concurrent_execution=True, verbose=True)
-        def my_function(arg1, arg2):
-            # function body
-
-        @tempit
-        def my_function(arg1, arg2):
-            # function body
-
-        # The decorated function can be used as usual
-        result = my_function(arg1_value, arg2_value)
-    """
-
-    def decorator(
-        func: Callable, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False
-    ) -> Callable:
-        @wraps(func)
-        def tempit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
-            callable_func, args, args_to_print = extract_callable_and_args_if_method(func, *args)
-            result, total_times, real_time = function_execution(
-                callable_func,
-                run_times,
-                concurrent_execution,
-                *args,
-                **kwargs,
-            )
-
-            print_tempit_values(run_times, verbose, callable_func, total_times, real_time, *args_to_print, **kwargs)
-
-            return result
-
-        return tempit_wrapper
-
-    if args:  # If arguments are not provided, return a decorator
-        return decorator(*args, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
-
-    else:  # Otherwise, return a partial function
-        return partial(decorator, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
-
-
-def extract_callable_and_args_if_method(func, *args) -> Tuple[Callable, Tuple, Tuple]:
-    """
-    Extracts the callable function and arguments from a given function, if it is a method.
-    Args:
-        func (Callable): The function to extract the callable from.
-        args: Variable length argument list.
-    Returns:
-        Tuple[Callable, Tuple, Tuple]: A tuple containing the extracted callable function, the modified arguments,
-        and the arguments to be printed.
-    Raises:
-        None
-    """
-    callable_func = func
-    args_to_print = args
-
-    is_method = hasattr(args[0], func.__name__) if args else False
-    if is_method:
-        args_to_print = args[1:]
-        if isinstance(func, classmethod):
-            args = (args[0].__class__,) + args[1:]  # type: ignore
-            callable_func = func.__func__
-        elif isinstance(func, staticmethod):
-            args = args[1:]
-
-    return callable_func, args, args_to_print
-
-
-def function_execution(
-    callable_func: Callable, run_times: int, concurrent_execution: bool, *args: Tuple, **kwargs: Dict
-) -> Tuple[Any, List[float], float]:
-    """
-    Run and measure the execution time of a function. It also returns the value of the function return and the execution times.
-    Args:
-        callable_func (Callable): The function to be executed.
-        run_times (int): The number of times the function should be executed.
-        concurrency_mode (str): The concurrency mode for executing the function.
-        *args (Tuple): The positional arguments to be passed to the function.
-        **kwargs (Dict): The keyword arguments to be passed to the function.
-    Returns:
-        Tuple[Any, List[float], float]: A tuple containing the result of the function,
-        a list of execution times for each run, and the total real time taken.
-    """
-    if run_times < 1:
-        run_times = 1
-    start_time = time.perf_counter()
-    if run_times > 1 and concurrent_execution:
-        try:
-            result, total_times = tempit_with_concurrency(callable_func, run_times, *args, **kwargs)
-        except RuntimeError as e:
-            print(e)
-            result, total_times = tempit_main_process(callable_func, run_times, *args, **kwargs)
-    else:
-        result, total_times = tempit_main_process(callable_func, run_times, *args, **kwargs)
-    end_time = time.perf_counter()
-    real_time = end_time - start_time
-
-    return result, total_times, real_time
-
-
-def tempit_main_process(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
-    """
-    Run and measure the execution time of a function in the main process. It also returns the value of the function return and the execution times.
-    Args:
-        func (Callable): The function to be executed.
-        run_times (int): The number of times the function should be executed.
-        *args (Tuple): The positional arguments to be passed to the function.
-        **kwargs (Dict): The keyword arguments to be passed to the function.
-    Returns:
-        Tuple[Any, List[float]]: A tuple containing the result of the function and a list of execution times for each run.
-    """
-
-    total_times: List[float] = []
-    for _ in range(run_times):
-        start_time: float = time.perf_counter()
-        try:
-            result: Any = func(*args, **kwargs)
-        except Exception as e:
-            print(e)
-        end_time: float = time.perf_counter()
-        total_times.append(end_time - start_time)
-    return result, total_times
-
-
-def tempit_with_concurrency(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
-    """
-    Executes a given function concurrently a specified number of times using joblib.
-
-    Args:
-        func (Callable): The function to be executed.
-        run_times (int): The number of times the function should be executed.
-        *args (Tuple): The positional arguments to be passed to the function.
-        **kwargs (Dict): The keyword arguments to be passed to the function.
-
-    Returns:
-        Tuple[Any, List[float]]: A tuple containing the result of the function and a list of execution times for each run.
-        If an exception was raised in one of the concurrent tasks, the function will raise a RuntimeError and returns control
-        to the main process, then the function will be executed in the main process non-concurrently.
-    """
-
-    from multiprocessing import current_process
-    from os import cpu_count
-    from threading import current_thread
-
-    from joblib import Parallel, delayed
-
-    def run_func(
-        func: Callable,
-        *args: Tuple,
-        **kwargs: Dict,
-    ) -> Tuple[Any, float, bool]:
-
-        has_crashed: bool = False
-        start_time = time.perf_counter()
-        try:
-            result: Any = func(*args, **kwargs)
-        except Exception:
-            has_crashed = True
-            result = None
-        finally:
-            end_time = time.perf_counter()
-            return result, end_time - start_time, has_crashed
-
-    joblib_backend = None  # Default backend for joblib
-    # Rule of thumb, use at least 2 workers or at least the number of cores minus 1.
-    # It is not ideal for multithreading, but it will make good balance
-    workers: int = max(2, cpu_count() - 1) if cpu_count() is not None else 2  # type: ignore
-
-    if current_process().name != "MainProcess" or current_thread().name != "MainThread":
-        joblib_backend = "threading"  # If we are running in other than the main process or main thread, use threading instead of multiprocessing
-
-    results: List[Tuple[Any, float, bool]] = Parallel(n_jobs=workers, backend=joblib_backend)(
-        delayed(run_func)(func, *args, **kwargs) for _ in range(run_times)
-    )  # type: ignore
-
-    if any(has_crashed for _, _, has_crashed in results):
-        raise RuntimeError(
-            "An exception was raised in one of the concurrent jobs. Trying to execute in the main process non-concurrently."
-        )
-
-    total_times = [total_time for _, total_time, has_crashed in results if not has_crashed]
-    result = results[0][0]
-    return result, total_times
+import time
+from functools import partial, wraps
+from typing import Any, Callable, Dict, List, Tuple
+
+from .utils import print_tempit_values
+
+
+def tempit(*args: Any, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False) -> Callable:
+    """
+    Decorator function that measures the execution time of a given function. It can be called like @tempit or using arguments @tempit(...)
+
+    Args:
+        args: contains the function to be decorated if no arguments are provided when calling the decorator
+        run_times (int, optional): The number of times the function should be executed. Defaults to 1.
+        concurrent_execution (bool, optional): This parameter will allow for the concurrent execution of the function using joblib.
+                                               The default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading.
+                                               If the execution of the concurrency fails, it will try to execute the func run_times non concurrently in the main process.
+                                               Defaults to True.
+        verbose (bool, optional): Whether to print detailed information after execution. Defaults to False.
+
+    Returns:
+        Callable: The decorated function if arguments are provided, otherwise a partial function.
+
+    Raises:
+        RuntimeError: If the concurrency mode fails, the function is executed in the main process.
+
+    Notes:
+        - If `run_times` is less than 1, it will be set to 1.
+        - If the function is a method, the first argument will be removed from `args_to_print`.
+        - If the function is a class method, the first argument will be replaced with the class itself.
+        - If the function is a static method, the first argument will be removed.
+
+    Example:
+        @tempit(run_times=5, concurrent_execution=True, verbose=True)
+        def my_function(arg1, arg2):
+            # function body
+
+        @tempit
+        def my_function(arg1, arg2):
+            # function body
+
+        # The decorated function can be used as usual
+        result = my_function(arg1_value, arg2_value)
+    """
+
+    def decorator(
+        func: Callable, run_times: int = 1, concurrent_execution: bool = True, verbose: bool = False
+    ) -> Callable:
+        @wraps(func)
+        def tempit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
+            callable_func, args, args_to_print = extract_callable_and_args_if_method(func, *args)
+            result, total_times, real_time = function_execution(
+                callable_func,
+                run_times,
+                concurrent_execution,
+                *args,
+                **kwargs,
+            )
+
+            print_tempit_values(run_times, verbose, callable_func, total_times, real_time, *args_to_print, **kwargs)
+
+            return result
+
+        return tempit_wrapper
+
+    if args:  # If arguments are not provided, return a decorator
+        return decorator(*args, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
+
+    else:  # Otherwise, return a partial function
+        return partial(decorator, run_times=run_times, concurrent_execution=concurrent_execution, verbose=verbose)
+
+
+def extract_callable_and_args_if_method(func, *args) -> Tuple[Callable, Tuple, Tuple]:
+    """
+    Extracts the callable function and arguments from a given function, if it is a method.
+    Args:
+        func (Callable): The function to extract the callable from.
+        args: Variable length argument list.
+    Returns:
+        Tuple[Callable, Tuple, Tuple]: A tuple containing the extracted callable function, the modified arguments,
+        and the arguments to be printed.
+    Raises:
+        None
+    """
+    callable_func = func
+    args_to_print = args
+
+    is_method = hasattr(args[0], func.__name__) if args else False
+    if is_method:
+        args_to_print = args[1:]
+        if isinstance(func, classmethod):
+            args = (args[0].__class__,) + args[1:]  # type: ignore
+            callable_func = func.__func__
+        elif isinstance(func, staticmethod):
+            args = args[1:]
+
+    return callable_func, args, args_to_print
+
+
+def function_execution(
+    callable_func: Callable, run_times: int, concurrent_execution: bool, *args: Tuple, **kwargs: Dict
+) -> Tuple[Any, List[float], float]:
+    """
+    Run and measure the execution time of a function. It also returns the value of the function return and the execution times.
+    Args:
+        callable_func (Callable): The function to be executed.
+        run_times (int): The number of times the function should be executed.
+        concurrency_mode (str): The concurrency mode for executing the function.
+        *args (Tuple): The positional arguments to be passed to the function.
+        **kwargs (Dict): The keyword arguments to be passed to the function.
+    Returns:
+        Tuple[Any, List[float], float]: A tuple containing the result of the function,
+        a list of execution times for each run, and the total real time taken.
+    """
+    if run_times < 1:
+        run_times = 1
+    start_time = time.perf_counter()
+    if run_times > 1 and concurrent_execution:
+        try:
+            result, total_times = tempit_with_concurrency(callable_func, run_times, *args, **kwargs)
+        except RuntimeError as e:
+            print(e)
+            result, total_times = tempit_main_process(callable_func, run_times, *args, **kwargs)
+    else:
+        result, total_times = tempit_main_process(callable_func, run_times, *args, **kwargs)
+    end_time = time.perf_counter()
+    real_time = end_time - start_time
+
+    return result, total_times, real_time
+
+
+def tempit_main_process(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
+    """
+    Run and measure the execution time of a function in the main process. It also returns the value of the function return and the execution times.
+    Args:
+        func (Callable): The function to be executed.
+        run_times (int): The number of times the function should be executed.
+        *args (Tuple): The positional arguments to be passed to the function.
+        **kwargs (Dict): The keyword arguments to be passed to the function.
+    Returns:
+        Tuple[Any, List[float]]: A tuple containing the result of the function and a list of execution times for each run.
+    """
+
+    total_times: List[float] = []
+    for _ in range(run_times):
+        start_time: float = time.perf_counter()
+        try:
+            result: Any = func(*args, **kwargs)
+        except Exception as e:
+            print(e)
+        end_time: float = time.perf_counter()
+        total_times.append(end_time - start_time)
+    return result, total_times
+
+
+def tempit_with_concurrency(func: Callable, run_times: int, *args: Tuple, **kwargs: Dict) -> Tuple[Any, List[float]]:
+    """
+    Executes a given function concurrently a specified number of times using joblib.
+
+    Args:
+        func (Callable): The function to be executed.
+        run_times (int): The number of times the function should be executed.
+        *args (Tuple): The positional arguments to be passed to the function.
+        **kwargs (Dict): The keyword arguments to be passed to the function.
+
+    Returns:
+        Tuple[Any, List[float]]: A tuple containing the result of the function and a list of execution times for each run.
+        If an exception was raised in one of the concurrent tasks, the function will raise a RuntimeError and returns control
+        to the main process, then the function will be executed in the main process non-concurrently.
+    """
+
+    from multiprocessing import current_process
+    from os import cpu_count
+    from threading import current_thread
+
+    from joblib import Parallel, delayed
+
+    def run_func(
+        func: Callable,
+        *args: Tuple,
+        **kwargs: Dict,
+    ) -> Tuple[Any, float, bool]:
+
+        has_crashed: bool = False
+        start_time = time.perf_counter()
+        try:
+            result: Any = func(*args, **kwargs)
+        except Exception:
+            has_crashed = True
+            result = None
+        finally:
+            end_time = time.perf_counter()
+            return result, end_time - start_time, has_crashed
+
+    joblib_backend = None  # Default backend for joblib
+    # Rule of thumb, use at least 2 workers or at least the number of cores minus 1.
+    # It is not ideal for multithreading, but it will make good balance
+    workers: int = max(2, cpu_count() - 1) if cpu_count() is not None else 2  # type: ignore
+
+    if current_process().name != "MainProcess" or current_thread().name != "MainThread":
+        joblib_backend = "threading"  # If we are running in other than the main process or main thread, use threading instead of multiprocessing
+
+    results: List[Tuple[Any, float, bool]] = Parallel(n_jobs=workers, backend=joblib_backend)(
+        delayed(run_func)(func, *args, **kwargs) for _ in range(run_times)
+    )  # type: ignore
+
+    if any(has_crashed for _, _, has_crashed in results):
+        raise RuntimeError(
+            "An exception was raised in one of the concurrent jobs. Trying to execute in the main process non-concurrently."
+        )
+
+    total_times = [total_time for _, total_time, has_crashed in results if not has_crashed]
+    result = results[0][0]
+    return result, total_times
```

### Comparing `tempit-0.1.3/tempit/utils.py` & `tempit-0.1.4/tempit/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,145 +1,145 @@
-from statistics import mean, median, stdev
-from typing import Callable, Dict, List, Tuple
-
-
-def print_tempit_values(
-    run_times: int,
-    verbose: bool,
-    func: Callable,
-    total_times: List[float],
-    real_time: float,
-    *args: Tuple,
-    **kwargs: Dict,
-) -> None:
-    """
-    Print the tempit values for a given function.
-    Args:
-        run_times (int): The number of times the function was executed.
-        verbose (bool): Whether to print verbose information.
-        func (Callable): The function to print the values for.
-        total_times (List[float]): The total execution times for each run of the function.
-        real_time (float): The real time taken to execute the function.
-        *args (Tuple): Additional positional arguments to pass to the function.
-        **kwargs (Dict): Additional keyword arguments to pass to the function.
-    Returns:
-        None
-    """
-    if verbose:
-        print("*" * 5, f"tempit data for function {func.__name__}:", "*" * 5)
-    if run_times == 1:
-        print_single_value(verbose, func, total_times[0], *args, **kwargs)
-    else:
-        print_several_values(verbose, func, total_times, real_time, *args, **kwargs)
-    if verbose:
-        print("*" * 5, "End of tempit data.", "*" * 5)
-
-
-def print_verbose_common_parts(func: Callable, *args: Tuple, **kwargs: Dict) -> None:
-    """
-    Print the tempti verbose common parts of a function.
-    Args:
-        func (Callable): The function to print the common parts for.
-        *args (Tuple): Additional positional arguments.
-        **kwargs (Dict): Additional keyword arguments.
-    Returns:
-        None
-    """
-    print(f"Function name: {func.__name__}")
-    print(f"\tFuncion object: {func}")
-    print(f"\tArgs: {args}")
-    print(f"\tKwargs: {kwargs}")
-
-
-def print_single_value(verbose: bool, func: Callable, total_time: float, *args: Tuple, **kwargs: Dict) -> None:
-    """
-    Print a single value based on the given parameters.
-    Args:
-        verbose (bool): Whether to print verbose information.
-        func (Callable): The function to print the value for.
-        total_time (float): The total execution time of the function.
-        *args (Tuple): Additional positional arguments.
-        **kwargs (Dict): Additional keyword arguments.
-    Returns:
-        None
-    """
-    if verbose:
-        print_verbose_common_parts(func, *args, **kwargs)
-        print(f"\tTime: {format_time(total_time)}.")
-    else:
-        print(f"Function {func.__name__} took {format_time(total_time)}.")
-
-
-def print_several_values(
-    verbose: bool, func: Callable, total_times: List[float], real_time: float, *args: Tuple, **kwargs: Dict
-) -> None:
-    """
-    Print several values based on the given parameters.
-    Args:
-        verbose (bool): Whether to print verbose information.
-        func (Callable): The function to print the values for.
-        total_times (List[float]): The total execution times for each run of the function.
-        real_time (float): The real time taken to execute the function.
-        *args (Tuple): Additional positional arguments.
-        **kwargs (Dict): Additional keyword arguments.
-    Returns:
-        None
-    """
-    avg_time = mean(total_times)
-
-    if verbose:
-        med_time = median(total_times)
-        min_time = min(total_times)
-        max_time = max(total_times)
-        std_dev = stdev(total_times)
-        total_time = sum(total_times)
-        print_verbose_common_parts(func, *args, **kwargs)
-        print(f"\tRun times: {len(total_times)}")
-        print(f"\tMean: {format_time(avg_time)}")
-        print(f"\tMedian: {format_time(med_time)}")
-        print(f"\tMin: {format_time(min_time)}")
-        print(f"\tMax: {format_time(max_time)}")
-        print(f"\tStandard deviation: {format_time(std_dev)}")
-        print(f"\tSum time: {format_time(total_time)}")
-        print(f"\tReal time: {format_time(real_time)}")
-    else:
-        print(f"Function {func.__name__} took and avg of {format_time(avg_time)}.")
-
-
-def format_time(total_time: float) -> str:
-    """
-    Formats the given total time into a human-readable string representation.
-    Args:
-        total_time (float): The total time to be formatted.
-    Returns:
-        str: The formatted time string.
-    """
-    if total_time < 0.001:
-        microseconds = total_time * 1_000_000
-        return f"{microseconds:.4f}µs"
-    elif total_time < 0.1:
-        return f"{(total_time * 1000):.4f}ms"
-    elif total_time < 1:
-        return f"{total_time:.3f}s"
-    elif total_time < 60:
-        return f"{total_time:.2f}s"
-    elif total_time < 3600:
-        minutes = int(total_time // 60)
-        seconds = total_time % 60
-        ms = seconds % 1 * 1000
-        return f"{minutes:02}m:{seconds:02.0f}s.{ms:.0f}ms"
-    if total_time < 86400:
-        hours = int(total_time // 3600)
-        total_time %= 3600
-        minutes = int(total_time // 60)
-        seconds = total_time % 60
-        ms = seconds % 1 * 1000
-        return f"{hours:02}h:{minutes:02}m:{seconds:02.0f}s.{ms:.0f}ms"
-    else:
-        days = int(total_time // 86400)
-        total_time %= 86400
-        hours = int(total_time // 3600)
-        total_time %= 3600
-        minutes = int(total_time // 60)
-        seconds = total_time % 60
-        ms = seconds % 1 * 1000
-        return f"{days}d:{hours:02}h:{minutes:02}m:{seconds:02.0f}s.{ms:.0f}ms"
+from statistics import mean, median, stdev
+from typing import Callable, Dict, List, Tuple
+
+
+def print_tempit_values(
+    run_times: int,
+    verbose: bool,
+    func: Callable,
+    total_times: List[float],
+    real_time: float,
+    *args: Tuple,
+    **kwargs: Dict,
+) -> None:
+    """
+    Print the tempit values for a given function.
+    Args:
+        run_times (int): The number of times the function was executed.
+        verbose (bool): Whether to print verbose information.
+        func (Callable): The function to print the values for.
+        total_times (List[float]): The total execution times for each run of the function.
+        real_time (float): The real time taken to execute the function.
+        *args (Tuple): Additional positional arguments to pass to the function.
+        **kwargs (Dict): Additional keyword arguments to pass to the function.
+    Returns:
+        None
+    """
+    if verbose:
+        print("*" * 5, f"tempit data for function {func.__name__}:", "*" * 5)
+    if run_times == 1:
+        print_single_value(verbose, func, total_times[0], *args, **kwargs)
+    else:
+        print_several_values(verbose, func, total_times, real_time, *args, **kwargs)
+    if verbose:
+        print("*" * 5, "End of tempit data.", "*" * 5)
+
+
+def print_verbose_common_parts(func: Callable, *args: Tuple, **kwargs: Dict) -> None:
+    """
+    Print the tempti verbose common parts of a function.
+    Args:
+        func (Callable): The function to print the common parts for.
+        *args (Tuple): Additional positional arguments.
+        **kwargs (Dict): Additional keyword arguments.
+    Returns:
+        None
+    """
+    print(f"Function name: {func.__name__}")
+    print(f"\tFuncion object: {func}")
+    print(f"\tArgs: {args}")
+    print(f"\tKwargs: {kwargs}")
+
+
+def print_single_value(verbose: bool, func: Callable, total_time: float, *args: Tuple, **kwargs: Dict) -> None:
+    """
+    Print a single value based on the given parameters.
+    Args:
+        verbose (bool): Whether to print verbose information.
+        func (Callable): The function to print the value for.
+        total_time (float): The total execution time of the function.
+        *args (Tuple): Additional positional arguments.
+        **kwargs (Dict): Additional keyword arguments.
+    Returns:
+        None
+    """
+    if verbose:
+        print_verbose_common_parts(func, *args, **kwargs)
+        print(f"\tTime: {format_time(total_time)}.")
+    else:
+        print(f"Function {func.__name__} took {format_time(total_time)}.")
+
+
+def print_several_values(
+    verbose: bool, func: Callable, total_times: List[float], real_time: float, *args: Tuple, **kwargs: Dict
+) -> None:
+    """
+    Print several values based on the given parameters.
+    Args:
+        verbose (bool): Whether to print verbose information.
+        func (Callable): The function to print the values for.
+        total_times (List[float]): The total execution times for each run of the function.
+        real_time (float): The real time taken to execute the function.
+        *args (Tuple): Additional positional arguments.
+        **kwargs (Dict): Additional keyword arguments.
+    Returns:
+        None
+    """
+    avg_time = mean(total_times)
+
+    if verbose:
+        med_time = median(total_times)
+        min_time = min(total_times)
+        max_time = max(total_times)
+        std_dev = stdev(total_times)
+        total_time = sum(total_times)
+        print_verbose_common_parts(func, *args, **kwargs)
+        print(f"\tRun times: {len(total_times)}")
+        print(f"\tMean: {format_time(avg_time)}")
+        print(f"\tMedian: {format_time(med_time)}")
+        print(f"\tMin: {format_time(min_time)}")
+        print(f"\tMax: {format_time(max_time)}")
+        print(f"\tStandard deviation: {format_time(std_dev)}")
+        print(f"\tSum time: {format_time(total_time)}")
+        print(f"\tReal time: {format_time(real_time)}")
+    else:
+        print(f"Function {func.__name__} took and avg of {format_time(avg_time)}.")
+
+
+def format_time(total_time: float) -> str:
+    """
+    Formats the given total time into a human-readable string representation.
+    Args:
+        total_time (float): The total time to be formatted.
+    Returns:
+        str: The formatted time string.
+    """
+    if total_time < 0.001:
+        microseconds = total_time * 1_000_000
+        return f"{microseconds:.4f}µs"
+    elif total_time < 0.1:
+        return f"{(total_time * 1000):.4f}ms"
+    elif total_time < 1:
+        return f"{total_time:.3f}s"
+    elif total_time < 60:
+        return f"{total_time:.2f}s"
+    elif total_time < 3600:
+        minutes = int(total_time // 60)
+        seconds = total_time % 60
+        ms = seconds % 1 * 1000
+        return f"{minutes:02}m:{seconds:02.0f}s.{ms:.0f}ms"
+    if total_time < 86400:
+        hours = int(total_time // 3600)
+        total_time %= 3600
+        minutes = int(total_time // 60)
+        seconds = total_time % 60
+        ms = seconds % 1 * 1000
+        return f"{hours:02}h:{minutes:02}m:{seconds:02.0f}s.{ms:.0f}ms"
+    else:
+        days = int(total_time // 86400)
+        total_time %= 86400
+        hours = int(total_time // 3600)
+        total_time %= 3600
+        minutes = int(total_time // 60)
+        seconds = total_time % 60
+        ms = seconds % 1 * 1000
+        return f"{days}d:{hours:02}h:{minutes:02}m:{seconds:02.0f}s.{ms:.0f}ms"
```

### Comparing `tempit-0.1.3/tempit.egg-info/PKG-INFO` & `tempit-0.1.4/tempit.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,123 +1,150 @@
-Metadata-Version: 2.1
-Name: tempit
-Version: 0.1.3
-Summary: A dead simple time decorator
-Home-page: https://github.com/mcrespoae/tempit
-Author: mcrespoae
-Author-email: info@mariocrespo.es
-Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: joblib
-
-# Tempit
-
-Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
-
-## Installation
-
-You can install Tempit using pip:
-
-```bash
-pip install tempit
-```
-
-## Usage
-
-Below are some examples demonstrating Tempit's usage:
-
-### Basic Usage
-
-```python
-from tempit import tempit
-
-@tempit
-def my_function():
-    # Normal code of your function
-    pass
-
-my_function()
-```
-
-This will output something like:
-
-```text
-Function my_function took 10.5908ms.
-```
-
-### Advanced Usage
-
-```python
-from tempit import tempit
-@tempit(run_times=20, concurrent_execution=True, verbose=True)
-def my_function_with_args(a:int = 1, b:int = 2):
-    return a + b
-
-result = my_function_with_args(1, b=2)
-```
-
-This will provide detailed output:
-
-```text
-***** tempit data for function my_function_with_args: *****
-Function name: my_function_with_args
-        Funcion object: <function my_function_with_args at 0x0000000000000000>
-        Args: (1,)
-        Kwargs: {'b': 2}
-        Run times: 20
-        Mean: 0.7000µs
-        Median: 0.8000µs
-        Min: 0.4000µs
-        Max: 1.0000µs
-        Standard deviation: 0.2828µs
-        Sum time: 3.5000µs
-        Real time: 965.1000µs
-***** End of tempit data. *****
-```
-
-More examples can be found in the [examples.py](examples/examples.py) script.
-
-## Features
-
-- Simplified usage.
-- Accurate measurement of function execution time.
-- Support for `classmethod` and `staticmethods`.
-- Parallel execution mode for performance measurement.
-- Human-readable time formatting.
-- Optional verbose mode for detailed information.
-
-## Parameters
-
-Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
-
-- `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
-- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
-- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
-
-## Contributing
-
-Contributions are welcome! Please follow these guidelines when contributing:
-
-1. Fork the repository.
-2. Create a new branch for your changes.
-3. Implement your changes and commit them.
-4. Push your changes to your forked repository.
-5. Submit a pull request.
-
-## Testing
-
-The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](tests) and can be executed using `make test`.
-
-## License
-
-This project is licensed under the [MIT License](LICENSE.txt).
-
-## Contributors
-
-- [Mario Crespo](https://github.com/mcrespoae)
+Metadata-Version: 2.1
+Name: tempit
+Version: 0.1.4
+Summary: A dead simple time decorator
+Home-page: https://github.com/mcrespoae/tempit
+Author: mcrespoae
+Author-email: info@mariocrespo.es
+Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: joblib==1.4.2
+
+# Tempit
+
+Tempit is a Python package designed to simplify the process of measuring the execution time of your functions through a straightforward decorator.
+
+## Installation
+
+You can install Tempit using pip:
+
+```bash
+pip install tempit
+```
+
+## Usage
+
+Below are some examples demonstrating Tempit's usage:
+
+### Basic Usage
+
+```python
+from tempit import tempit
+
+@tempit
+def my_function():
+    # Normal code of your function
+    pass
+
+my_function()
+```
+
+This will output something like:
+
+```text
+Function my_function took 10.5908ms.
+```
+
+### Advanced Usage
+
+```python
+from tempit import tempit
+@tempit(run_times=20, concurrent_execution=True, verbose=True)
+def my_function_with_args(a:int = 1, b:int = 2):
+    return a + b
+
+result = my_function_with_args(1, b=2)
+```
+
+This will provide detailed output:
+
+```text
+***** tempit data for function my_function_with_args: *****
+Function name: my_function_with_args
+        Funcion object: <function my_function_with_args at 0x0000000000000000>
+        Args: (1,)
+        Kwargs: {'b': 2}
+        Run times: 20
+        Mean: 0.7000Âµs
+        Median: 0.8000Âµs
+        Min: 0.4000Âµs
+        Max: 1.0000Âµs
+        Standard deviation: 0.2828Âµs
+        Sum time: 3.5000Âµs
+        Real time: 965.1000Âµs
+***** End of tempit data. *****
+```
+
+More examples can be found in the [examples.py](examples/examples.py) script.
+
+## Features
+
+- Simplified usage.
+- Accurate measurement of function execution time.
+- Support for `classmethod` and `staticmethods`.
+- Parallel execution mode for performance measurement.
+- Human-readable time formatting.
+- Optional verbose mode for detailed information.
+
+## Parameters
+
+Using the decorator @tempit without any parameters executes the function once and displays the execution time. However, you can enhance the experience using the following arguments:
+
+- `run_times` (int, optional): Specifies the number of function executions. Defaults to 1.
+- `concurrency_mode` (bool, optional): Determines the concurrency mode for the function execution. It uses [joblib](https://pypi.org/project/joblib/) for parallel computing. The  default execution backend is "loky" but if the function is being triggered other than the main thread or main process, the backend will be changed to multithreading to aovid pickle errors. If, for any other reason, fails, the program will try to execute the func run_times non concurrently in the main process. Defaults to True.
+- `verbose` (bool, optional): Controls whether detailed information is printed after execution. Defaults to False.
+
+## Note with recursive functions
+
+This package doesn't work well with recursive functions. The specific reason and limitation are that using recursive functions with this package may result in very verbose output, making it difficult to read, especially for larger values.
+
+To avoid this issue, you can encapsulate the recursive function within another function and call it without printing messages. Here's an example:
+
+```python
+@tempit
+def encapsulated_recursive_function(n):
+    """A non-verbose wrapper for the recursive function."""
+    def recursive_func(n):
+        if n == 0:
+            return 0
+        else:
+            return n + recursive_func(n - 1)
+
+    return recursive_func(n)
+
+# Using the encapsulated recursive function
+result = encapsulated_recursive_function(3)
+```
+
+This approach makes the output cleaner and easier to read, especially when dealing with recursive functions with many calls.
+
+## Contributing
+
+Contributions are welcome! Please follow these guidelines when contributing:
+
+1. Fork the repository.
+2. Use `make install` to install all depedencies.
+3. Create a new branch for your changes.
+4. Implement your changes and commit them.
+5. Push your changes to your forked repository.
+6. Submit a pull request.
+
+You can test your code using `make test` and `make example` to trigger the examples. Please, check the [Makefile](Makefile) to know more about commands.
+
+## Testing
+
+The package has been thoroughly tested using unittesting. Test cases can be found in the [tests folder](tests).
+
+## License
+
+This project is licensed under the [MIT License](LICENSE.txt).
+
+## Contributors
+
+- [Mario Crespo](https://github.com/mcrespoae)
```

### Comparing `tempit-0.1.3/tests/test_tempit.py` & `tempit-0.1.4/tests/test_tempit.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,357 +1,357 @@
-import os
-import threading
-import time
-import unittest
-from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
-from multiprocessing import current_process
-
-from tempit.core import tempit
-from tempit.utils import format_time
-
-IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
-
-
-class TempitTestClass:
-    @tempit()
-    def tempit_basic(self):
-        time.sleep(0.01)
-
-    @tempit
-    def tempit_basic_no_parenthesis(self):
-        time.sleep(0.01)
-
-    @tempit(run_times=5)
-    def test_tempit_with_concurrency(self):
-        time.sleep(0.01)
-
-    @tempit(run_times=5, concurrent_execution=False, verbose=False)
-    def test_tempit_no_concurrency(self):
-        time.sleep(0.01)
-
-    @tempit(run_times=5, concurrent_execution=True, verbose=True)
-    def test_tempit_concurrency_verbose(self):
-        time.sleep(0.01)
-
-    @tempit(run_times=10, concurrent_execution=True, verbose=True)
-    def test_tempit_thread_crash(self, a: int = 1, b: int = 2, thread_name: str = "ThreadPoolExecutor-"):
-        current_thread_name = threading.current_thread().name
-        if not current_thread_name.startswith(thread_name):
-            raise RuntimeError("Crashing intentionally for testing other process inside a class")
-        return a + b
-
-    def sum(self, a: int = 1, b: int = 2):
-        return a + b
-
-    @tempit(run_times=10)
-    def test_tempit_args(self, a: int = 1, b: int = 2):
-        return self.sum(a, b)
-
-    @tempit(run_times=2)
-    @staticmethod
-    def static_method(a: int = 1, b: int = 2):
-        return a + b
-
-    @tempit(run_times=2, verbose=True)
-    @classmethod
-    def class_method(cls, a: int = 1, b: int = 2):
-        return cls.__name__, a + b
-
-
-class TestTempitDecoratorClass(unittest.TestCase):
-    def setUp(self):
-        self.test_class = TempitTestClass()
-
-    def test_tempit_basic(self):
-
-        start_time = time.perf_counter()
-        self.test_class.tempit_basic()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
-
-    def test_tempit_basic_no_parenthesis(self):
-
-        start_time = time.perf_counter()
-        self.test_class.tempit_basic_no_parenthesis()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
-
-    def test_tempit_with_concurrency(self):
-
-        start_time = time.perf_counter()
-        self.test_class.test_tempit_with_concurrency()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
-
-    def test_tempit_no_concurrency(self):
-        start_time = time.perf_counter()
-        self.test_class.test_tempit_no_concurrency()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
-
-    def test_tempit_concurrency_verbose(self):
-        # Just check it doesn't crash
-        start_time = time.perf_counter()
-        self.test_class.test_tempit_concurrency_verbose()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
-
-    def test_tempit_other_thread_crash(self):
-        # Just check if it the parallel execution doesn't work, it should be executed in the main thread
-        start_time = time.perf_counter()
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.test_tempit_thread_crash, 1, b=2)
-            result = future.result()
-        end_time = time.perf_counter()
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
-        self.assertEqual(result, 3)
-
-    def test_tempit_args(self):
-        result = self.test_class.test_tempit_args(1, b=2)
-        self.assertEqual(result, 3)
-
-    def test_tempit_static_method(self):
-        result = self.test_class.static_method(1, b=2)
-        self.assertEqual(result, 3)
-
-    def test_tempit_class_method(self):
-        class_name, result = self.test_class.class_method(1, b=2)
-        self.assertEqual(class_name, "TempitTestClass")
-        self.assertEqual(result, 3)
-
-    def test_tempit_run_from_other_thread(self):
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.test_tempit_args, 1, b=2)
-            result = future.result()
-
-        self.assertEqual(result, 3)
-
-    def test_tempit_run_from_other_process(self):
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.test_tempit_args, 1, b=2)
-            result = future.result()
-
-        self.assertEqual(result, 3)
-
-    def test_tempit_class_method_from_other_thread(self):
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.class_method, 1, b=2)
-            class_name, result = future.result()
-
-        self.assertEqual(class_name, "TempitTestClass")
-        self.assertEqual(result, 3)
-
-    def test_tempit_class_method_run_from_other_process(self):
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.class_method, 2, b=6)
-            class_name, result = future.result()
-
-        self.assertEqual(class_name, "TempitTestClass")
-        self.assertEqual(result, 8)
-
-    def test_tempit_static_method_from_other_thread(self):
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.static_method, 4, b=5)
-            result = future.result()
-
-        self.assertEqual(result, 9)
-
-    def test_tempit_static_method_run_from_other_process(self):
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(self.test_class.static_method, 1, b=2)
-            result = future.result()
-
-        self.assertEqual(result, 3)
-
-
-class TestTempitDecoratorFunction(unittest.TestCase):
-
-    def test_tempit_basic(self):
-        @tempit()
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.perf_counter()
-        my_function()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
-
-    def test_tempit_basic_no_parenthesis(self):
-        @tempit
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.perf_counter()
-        my_function()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
-
-    def test_tempit_with_concurrency(self):
-        @tempit(run_times=5, concurrent_execution=True)
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.perf_counter()
-        my_function()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)  # Check if execution time is close to 0.1 seconds
-
-    def test_tempit_no_concurrency(self):
-        @tempit(run_times=5, concurrent_execution=False)
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.perf_counter()
-        my_function()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
-
-    def test_tempit_multithreading_verbose(self):
-        # Just check it doesn't crash
-        @tempit(run_times=5, concurrent_execution=True, verbose=True)
-        def my_function():
-            time.sleep(0.01)
-
-        start_time = time.perf_counter()
-        my_function()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
-
-    def test_tempit_multithreading_crash(self):
-        # Just check if it the multihreading doesn't work, it should be executed in the main thread
-        @tempit(run_times=5, concurrent_execution=True)
-        def my_function():
-            current_thread_name = threading.current_thread().name
-            process_name = current_process().name
-            if current_thread_name != "MainThread" or process_name != "MainProcess":
-                raise RuntimeError("Crashing intentionally for testing multithreading outside class")
-            time.sleep(0.01)
-
-        start_time = time.perf_counter()
-        my_function()
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertLess(execution_time, 0.5)
-
-    def test_tempit_args(self):
-        @tempit(run_times=2, concurrent_execution=True, verbose=True)
-        def my_function(a: int = 1, b: int = 2):
-            return a + b
-
-        start_time = time.perf_counter()
-        result = my_function(1, b=2)
-        end_time = time.perf_counter()
-
-        execution_time = end_time - start_time
-        self.assertLess(execution_time, 0.05)
-        self.assertEqual(result, 3)
-
-    def test_run_from_other_thread(self):
-        @tempit(run_times=2, concurrent_execution=True, verbose=True)
-        def my_function(a: int = 1, b: int = 2):
-            return a + b
-
-        with ThreadPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(my_function, 2, b=4)
-            result = future.result()
-
-        self.assertEqual(result, 6)
-
-    def test_run_from_other_process(self):
-        with ProcessPoolExecutor(max_workers=1) as executor:
-            future = executor.submit(my_process_function, 1, b=2)
-            result = future.result()
-
-        self.assertEqual(result, 3)
-
-    @unittest.skipUnless(not IN_GITHUB_ACTIONS, "Skip if running in GitHub Actions: too expensive.")
-    def test_tempit_long_running_function(self):
-        @tempit(run_times=4, concurrent_execution=True)
-        def my_concurrent_function(a=2_000_000, n=16):
-            for _ in range(a):
-                pass  #
-            return fib(n=n)
-
-        @tempit(run_times=4, concurrent_execution=False)
-        def my_sequential_function(a=2_000_000, n=16):
-            for _ in range(a):
-                pass  #
-            return fib(n=n)
-
-        start_time = time.perf_counter()
-        result_concurrent = my_concurrent_function(200_000_000, n=32)
-        end_time = time.perf_counter()
-        execution_time_concurrent = end_time - start_time
-
-        start_time = time.perf_counter()
-        result_sequential = my_sequential_function(200_000_000, n=32)
-        end_time = time.perf_counter()
-        execution_time_sequential = end_time - start_time
-
-        # self.assertGreaterEqual(execution_time_sequential, lower_bound)
-        self.assertLessEqual(
-            execution_time_concurrent, (execution_time_sequential / 4) + (execution_time_sequential * 0.1)
-        )
-
-        self.assertEqual(result_concurrent, 2178309)
-        self.assertEqual(result_sequential, 2178309)
-
-
-def fib(n):
-    if n < 2:
-        return n
-    return fib(n - 2) + fib(n - 1)
-
-
-# Added here since calling a function from another process inside a test method doesn't work
-@tempit(run_times=2, concurrent_execution=True, verbose=True)
-def my_process_function(a: int = 1, b: int = 2):
-    return a + b
-
-
-class TestFormatTime(unittest.TestCase):
-    def test_format_time_microseconds(self):
-        self.assertEqual(format_time(0.0005), "500.0000µs")
-
-    def test_format_time_milliseconds(self):
-        self.assertEqual(format_time(0.08256741), "82.5674ms")
-
-    def test_format_time_deconds1(self):
-        self.assertEqual(format_time(0.25), "0.250s")
-
-    def test_format_time_seconds2(self):
-        self.assertEqual(format_time(3.14159), "3.14s")
-
-    def test_format_time_minutes(self):
-        self.assertEqual(format_time(65.4321), "01m:05s.432ms")
-
-    def test_format_time_hours(self):
-        self.assertEqual(format_time(3665.4321), "01h:01m:05s.432ms")
-
-    def test_format_time_days(self):
-        self.assertEqual(format_time(86465.4321), "1d:00h:01m:05s.432ms")
-
-
-if __name__ == "__main__":
-    unittest.main()
+import os
+import threading
+import time
+import unittest
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
+from multiprocessing import current_process
+
+from tempit.core import tempit
+from tempit.utils import format_time
+
+IN_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
+
+
+class TempitTestClass:
+    @tempit()
+    def tempit_basic(self):
+        time.sleep(0.01)
+
+    @tempit
+    def tempit_basic_no_parenthesis(self):
+        time.sleep(0.01)
+
+    @tempit(run_times=5)
+    def test_tempit_with_concurrency(self):
+        time.sleep(0.01)
+
+    @tempit(run_times=5, concurrent_execution=False, verbose=False)
+    def test_tempit_no_concurrency(self):
+        time.sleep(0.01)
+
+    @tempit(run_times=5, concurrent_execution=True, verbose=True)
+    def test_tempit_concurrency_verbose(self):
+        time.sleep(0.01)
+
+    @tempit(run_times=10, concurrent_execution=True, verbose=True)
+    def test_tempit_thread_crash(self, a: int = 1, b: int = 2, thread_name: str = "ThreadPoolExecutor-"):
+        current_thread_name = threading.current_thread().name
+        if not current_thread_name.startswith(thread_name):
+            raise RuntimeError("Crashing intentionally for testing other process inside a class")
+        return a + b
+
+    def sum(self, a: int = 1, b: int = 2):
+        return a + b
+
+    @tempit(run_times=10)
+    def test_tempit_args(self, a: int = 1, b: int = 2):
+        return self.sum(a, b)
+
+    @tempit(run_times=2)
+    @staticmethod
+    def static_method(a: int = 1, b: int = 2):
+        return a + b
+
+    @tempit(run_times=2, verbose=True)
+    @classmethod
+    def class_method(cls, a: int = 1, b: int = 2):
+        return cls.__name__, a + b
+
+
+class TestTempitDecoratorClass(unittest.TestCase):
+    def setUp(self):
+        self.test_class = TempitTestClass()
+
+    def test_tempit_basic(self):
+
+        start_time = time.perf_counter()
+        self.test_class.tempit_basic()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
+
+    def test_tempit_basic_no_parenthesis(self):
+
+        start_time = time.perf_counter()
+        self.test_class.tempit_basic_no_parenthesis()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
+
+    def test_tempit_with_concurrency(self):
+
+        start_time = time.perf_counter()
+        self.test_class.test_tempit_with_concurrency()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
+
+    def test_tempit_no_concurrency(self):
+        start_time = time.perf_counter()
+        self.test_class.test_tempit_no_concurrency()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
+
+    def test_tempit_concurrency_verbose(self):
+        # Just check it doesn't crash
+        start_time = time.perf_counter()
+        self.test_class.test_tempit_concurrency_verbose()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
+
+    def test_tempit_other_thread_crash(self):
+        # Just check if it the parallel execution doesn't work, it should be executed in the main thread
+        start_time = time.perf_counter()
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.test_tempit_thread_crash, 1, b=2)
+            result = future.result()
+        end_time = time.perf_counter()
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
+        self.assertEqual(result, 3)
+
+    def test_tempit_args(self):
+        result = self.test_class.test_tempit_args(1, b=2)
+        self.assertEqual(result, 3)
+
+    def test_tempit_static_method(self):
+        result = self.test_class.static_method(1, b=2)
+        self.assertEqual(result, 3)
+
+    def test_tempit_class_method(self):
+        class_name, result = self.test_class.class_method(1, b=2)
+        self.assertEqual(class_name, "TempitTestClass")
+        self.assertEqual(result, 3)
+
+    def test_tempit_run_from_other_thread(self):
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.test_tempit_args, 1, b=2)
+            result = future.result()
+
+        self.assertEqual(result, 3)
+
+    def test_tempit_run_from_other_process(self):
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.test_tempit_args, 1, b=2)
+            result = future.result()
+
+        self.assertEqual(result, 3)
+
+    def test_tempit_class_method_from_other_thread(self):
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.class_method, 1, b=2)
+            class_name, result = future.result()
+
+        self.assertEqual(class_name, "TempitTestClass")
+        self.assertEqual(result, 3)
+
+    def test_tempit_class_method_run_from_other_process(self):
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.class_method, 2, b=6)
+            class_name, result = future.result()
+
+        self.assertEqual(class_name, "TempitTestClass")
+        self.assertEqual(result, 8)
+
+    def test_tempit_static_method_from_other_thread(self):
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.static_method, 4, b=5)
+            result = future.result()
+
+        self.assertEqual(result, 9)
+
+    def test_tempit_static_method_run_from_other_process(self):
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(self.test_class.static_method, 1, b=2)
+            result = future.result()
+
+        self.assertEqual(result, 3)
+
+
+class TestTempitDecoratorFunction(unittest.TestCase):
+
+    def test_tempit_basic(self):
+        @tempit()
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
+
+    def test_tempit_basic_no_parenthesis(self):
+        @tempit
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.01)
+
+    def test_tempit_with_concurrency(self):
+        @tempit(run_times=5, concurrent_execution=True)
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)  # Check if execution time is close to 0.1 seconds
+
+    def test_tempit_no_concurrency(self):
+        @tempit(run_times=5, concurrent_execution=False)
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.05, delta=0.1)
+
+    def test_tempit_multithreading_verbose(self):
+        # Just check it doesn't crash
+        @tempit(run_times=5, concurrent_execution=True, verbose=True)
+        def my_function():
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertAlmostEqual(execution_time, 0.01, delta=0.1)
+
+    def test_tempit_multithreading_crash(self):
+        # Just check if it the multihreading doesn't work, it should be executed in the main thread
+        @tempit(run_times=5, concurrent_execution=True)
+        def my_function():
+            current_thread_name = threading.current_thread().name
+            process_name = current_process().name
+            if current_thread_name != "MainThread" or process_name != "MainProcess":
+                raise RuntimeError("Crashing intentionally for testing multithreading outside class")
+            time.sleep(0.01)
+
+        start_time = time.perf_counter()
+        my_function()
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertLess(execution_time, 0.5)
+
+    def test_tempit_args(self):
+        @tempit(run_times=2, concurrent_execution=True, verbose=True)
+        def my_function(a: int = 1, b: int = 2):
+            return a + b
+
+        start_time = time.perf_counter()
+        result = my_function(1, b=2)
+        end_time = time.perf_counter()
+
+        execution_time = end_time - start_time
+        self.assertLess(execution_time, 0.05)
+        self.assertEqual(result, 3)
+
+    def test_run_from_other_thread(self):
+        @tempit(run_times=2, concurrent_execution=True, verbose=True)
+        def my_function(a: int = 1, b: int = 2):
+            return a + b
+
+        with ThreadPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(my_function, 2, b=4)
+            result = future.result()
+
+        self.assertEqual(result, 6)
+
+    def test_run_from_other_process(self):
+        with ProcessPoolExecutor(max_workers=1) as executor:
+            future = executor.submit(my_process_function, 1, b=2)
+            result = future.result()
+
+        self.assertEqual(result, 3)
+
+    @unittest.skipUnless(not IN_GITHUB_ACTIONS, "Skip if running in GitHub Actions: too expensive.")
+    def test_tempit_long_running_function(self):
+        @tempit(run_times=4, concurrent_execution=True)
+        def my_concurrent_function(a=2_000_000, n=16):
+            for _ in range(a):
+                pass  #
+            return fib(n=n)
+
+        @tempit(run_times=4, concurrent_execution=False)
+        def my_sequential_function(a=2_000_000, n=16):
+            for _ in range(a):
+                pass  #
+            return fib(n=n)
+
+        start_time = time.perf_counter()
+        result_concurrent = my_concurrent_function(20_000_000, n=16)
+        end_time = time.perf_counter()
+        execution_time_concurrent = end_time - start_time
+
+        start_time = time.perf_counter()
+        result_sequential = my_sequential_function(20_000_000, n=16)
+        end_time = time.perf_counter()
+        execution_time_sequential = end_time - start_time
+
+        # self.assertGreaterEqual(execution_time_sequential, lower_bound)
+        self.assertLessEqual(
+            execution_time_concurrent, (execution_time_sequential / 3) + (execution_time_sequential * 0.2)
+        )
+
+        self.assertEqual(result_concurrent, 987)
+        self.assertEqual(result_sequential, 987)
+
+
+def fib(n):
+    if n < 2:
+        return n
+    return fib(n - 2) + fib(n - 1)
+
+
+# Added here since calling a function from another process inside a test method doesn't work
+@tempit(run_times=2, concurrent_execution=True, verbose=True)
+def my_process_function(a: int = 1, b: int = 2):
+    return a + b
+
+
+class TestFormatTime(unittest.TestCase):
+    def test_format_time_microseconds(self):
+        self.assertEqual(format_time(0.0005), "500.0000µs")
+
+    def test_format_time_milliseconds(self):
+        self.assertEqual(format_time(0.08256741), "82.5674ms")
+
+    def test_format_time_deconds1(self):
+        self.assertEqual(format_time(0.25), "0.250s")
+
+    def test_format_time_seconds2(self):
+        self.assertEqual(format_time(3.14159), "3.14s")
+
+    def test_format_time_minutes(self):
+        self.assertEqual(format_time(65.4321), "01m:05s.432ms")
+
+    def test_format_time_hours(self):
+        self.assertEqual(format_time(3665.4321), "01h:01m:05s.432ms")
+
+    def test_format_time_days(self):
+        self.assertEqual(format_time(86465.4321), "1d:00h:01m:05s.432ms")
+
+
+if __name__ == "__main__":
+    unittest.main()
```

