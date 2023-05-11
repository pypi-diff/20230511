# Comparing `tmp/easycheck-0.6.0.tar.gz` & `tmp/easycheck-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck-0.6.0.tar", last modified: Tue May  9 09:39:43 2023, max compression
+gzip compressed data, was "easycheck-0.7.0.tar", last modified: Thu May 11 05:11:12 2023, max compression
```

## Comparing `easycheck-0.6.0.tar` & `easycheck-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-09 09:39:43.001563 easycheck-0.6.0/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1073 2023-05-05 06:17:51.000000 easycheck-0.6.0/LICENSE
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    13312 2023-05-09 09:39:43.000566 easycheck-0.6.0/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    12543 2023-05-09 02:28:08.000000 easycheck-0.6.0/README.rst
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-09 09:39:42.961958 easycheck-0.6.0/easycheck/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      633 2023-05-05 06:17:51.000000 easycheck-0.6.0/easycheck/__init__.py
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    41348 2023-05-09 02:28:08.000000 easycheck-0.6.0/easycheck/easycheck.py
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-09 09:39:42.993566 easycheck-0.6.0/easycheck.egg-info/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    13312 2023-05-09 09:39:42.000000 easycheck-0.6.0/easycheck.egg-info/PKG-INFO
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      260 2023-05-09 09:39:42.000000 easycheck-0.6.0/easycheck.egg-info/SOURCES.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-05-09 09:39:42.000000 easycheck-0.6.0/easycheck.egg-info/dependency_links.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       26 2023-05-09 09:39:42.000000 easycheck-0.6.0/easycheck.egg-info/requires.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       10 2023-05-09 09:39:42.000000 easycheck-0.6.0/easycheck.egg-info/top_level.txt
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-05-09 09:39:43.001563 easycheck-0.6.0/setup.cfg
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1088 2023-05-09 02:28:08.000000 easycheck-0.6.0/setup.py
-drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-09 09:39:42.996568 easycheck-0.6.0/tests/
--rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    53348 2023-05-09 09:35:35.000000 easycheck-0.6.0/tests/test_easycheck.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-11 05:11:12.181404 easycheck-0.7.0/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1073 2021-01-27 07:58:06.000000 easycheck-0.7.0/LICENSE
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    18030 2023-05-11 05:11:12.179970 easycheck-0.7.0/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    15058 2023-05-11 05:10:55.000000 easycheck-0.7.0/README.rst
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-11 05:11:12.160752 easycheck-0.7.0/easycheck/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      614 2023-05-11 05:10:55.000000 easycheck-0.7.0/easycheck/__init__.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    37062 2023-05-11 05:10:55.000000 easycheck-0.7.0/easycheck/easycheck.py
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      865 2023-03-01 16:15:06.000000 easycheck-0.7.0/easycheck/tmp.py
+drwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        0 2023-05-11 05:11:12.175970 easycheck-0.7.0/easycheck.egg-info/
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)    18030 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/PKG-INFO
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)      253 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)        1 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       26 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/requires.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       10 2023-05-11 05:11:06.000000 easycheck-0.7.0/easycheck.egg-info/top_level.txt
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)       38 2023-05-11 05:11:12.181596 easycheck-0.7.0/setup.cfg
+-rwxrwxrwx   0 kozakm5   (1000) kozakm5   (1000)     1126 2023-05-11 05:10:55.000000 easycheck-0.7.0/setup.py
```

### Comparing `easycheck-0.6.0/LICENSE` & `easycheck-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easycheck-0.6.0/PKG-INFO` & `easycheck-0.7.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,16 @@
-Metadata-Version: 2.1
-Name: easycheck
-Version: 0.6.0
-Summary: A tool for simple functionalized assertions in Python
-Home-page: https://github.com/nyggus/easycheck
-Author: Nyggus & Ke Boan
-Author-email: nyggus@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 easycheck
 =========
 
-The :code:`easycheck` package offers a lightweight tool for running functionized assertion-like checks within Python code; it also offers functions to be used in testing - particularly in doctests, but also in pytests, for which purpose some of the functions have dedicated aliases. The idea is to use the :code:`easycheck` functions in a similar way as assertions, but with more functionality and with a slightly different aim: When a condition you define is met, nothing happens (in fact, the function returns :code:`None`); if the condition is violated, an exception is raised or a warning is issued. The main differences between :code:`easycheck` functions and assertions are as follows:
+The :code:`easycheck` package offers a lightweight tool for running functionized checks within Python code; it also offers functions to be used in testing - particularly in doctests, but also in pytests, for which purpose some of the functions have dedicated aliases (starting off with :code:`assert_` instead of :code:`check_`).
+
+The idea is to use the :code:`easycheck` functions to check conditions that are _not_ assertions. The checks work in the following general way: When a condition is met, nothing happens (in fact, the function returns :code:`None`); if it is violated, an exception is raised or a warning is issued. The main differences between :code:`easycheck` functions and assertions are as follows:
 
-* While you should not use assertions in your Python code, you can do so with the :code:`easycheck` functions.
+* Assertions are meant to be used conditions that _must_ be true (when only the code is correct). So, if an assertion is incorrect, it means something is wrong with the code. You should never use assertions to handle regular exceptions, like those related to data or arguments.
+* Unlike assertions, :code:`easycheck` functions are to be used to check conditions related to things like data and argument values, and to handle regular exceptions.
 * While assertions only raise :code:`AssertionError`, you can choose any exception to be raised by easycheck functions.
 * When using :code:`easycheck`, instead of raising an exception, you can issue a warning.
 
 The main :code:`easycheck` functions (with names starting off with :code:`check_`) are designed in such a way that they can be used as easy-to-understand code that checks whether one or more conditions are met. They can be used instead of :code:`if`-blocks, which are normally used to check conditions and raise exceptions (or issue warnings) if they are not met. So, you can do the following:
 
 .. code-block:: python
 
@@ -50,26 +31,35 @@
 * It saves a little space; not much, since most often you'll end up with one line of code instead of two, but not always, particularly when you provide an exception type to be raised and a long message. 
 * Mainly, it increases code simplicity and readability, since both the names of easycheck functions and their arguments are designed in such a way that the reader immediately understands what is being checked.
 
 You can also issue a warning:
 
 .. code-block:: python
 
-    check_if(x <= 10, Warning, 'For stable functioning of the function, x should not be greater than 10.')
+    check_if(x <= 10,
+             Warning,
+             'For stable functioning of the function, '
+             'x should not be greater than 10.')
 
 The package also offers functions dedicated to testing, e.g.,
 
 .. code-block:: python
 
     assert_type(x, (float, int))
     assert_if(x <= 10)
 
 The :code:`message` argument has the default value of :code:`None`, which does the following. If the exception class provided in :code:`handle_with` is built-in (that is, can be found in :code:`dir(builtins)`), no message is provided. But if it is not a built-in exception (or warning) class, then the exception/warning class's docstring is taken as the message. This is a convenient way of providing a  typical message. If you want to customize the message (e.g., depending on the value of a variable), you should use a customized string (e.g., through an f-string). But if you do not want to use any message with a custom exception/warning, simply provide an empty string (:code:`message=''`).
 
 
+Read about :code:`easycheck`
+----------------------------
+
+You will find more about assertions in `this article <https://medium.com/towards-data-science/python-assertions-or-checking-if-a-cat-is-a-dog-ce11c55d143>`_, entitled "Python Assertions, or Checking If a Cat Is a Dog" and published in *Towards Data Science*. It mentions :code:`easycheck`! You will read about :code:`easycheck` also in `the article "Comparing floating-point numbers with easycheck" <https://medium.com/towards-data-science/comparing-floating-point-numbers-with-easycheck-dcbae480f75f>`_  (also from *Towards Data Science*). The *Better Programming* article entitiled `"How to Overwrite AssertionError in Python and Use Custom Exceptions" <https://medium.com/better-programming/how-to-overwrite-asserterror-in-python-and-use-custom-exceptions-c0b252989977>`_, mentions the package, too.
+
+
 Installing
 ----------
 
 Install and update using pip:
 
 .. code-block:: text
 
@@ -273,7 +263,11 @@
 
 Other examples
 --------------
 
 You will find a number of examples in `doctest files <https://github.com/nyggus/easycheck/tree/master/docs/>`_, which also serve as doctests.
 
 
+Changelog
+---------
+
+* Version 0.6.0 came with significant optimization of performance. Before, :code:`easycheck` functions performed internal checks of the argument values provided to the function call. Most of these checks are not performed anymore, at least not for the most significant :code:`easycheck` functions, such as :code:`check_if()` or :code:`check_type()`. Some checks, however, are still done. These are mainly checks without which the behavior of the function would be either unwanted or unexpected. We decided to remove all checks that do not change much; for instance, they raise an error due to an incorrect type of an argument value — even though it would be raised anyway, but by the internal Python process, not by the :code:`easycheck` function itself. The point is to remove such unnecessary checks and that way remove the unnecessary :code:`if` blocks, which certainly add some cost to execution time. While one such check costs almost nothing, many of them (e.g., in a long loop) can mean a significant cost. As of version 0.6.0, we will try to optimize the performance of :code:`easycheck` by getting rid of such overhead costs, unless they are important for the behavior of the corresponding :code:`easycheck` function.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `easycheck-0.6.0/easycheck/__init__.py` & `easycheck-0.7.0/easycheck/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     check_argument,
     check_comparison,
     catch_check,
     # Exception classes
     ComparisonError,
     ArgumentValueError,
     LengthError,
-    OperatorError,
     NotCloseEnoughError,
     # Testing aliases
     assert_if,
     assert_if_not,
     assert_length,
     assert_if_isclose,
     assert_type,
```

### Comparing `easycheck-0.6.0/easycheck/easycheck.py` & `easycheck-0.7.0/easycheck/easycheck.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 """A module for simple checks to be used within code and testing.
 
 The easycheck module offers simple functions to check conditions and either raise
 an exception or issue a warning if the condition is violated; otherwise,
 nothing happens (the function returns None). You can either choose default
-exceptions and messages (or no message) or customize them. Unlike the assertion
-expression, you can use easycheck functions within code.
+exceptions and messages (or no message) or customize them. Unlike the assert
+statement, you can use easycheck functions within code.
 
 The module also offers aliases to be used in testing, all of which have the
 word "assert" in their names (assert_if(), assert_if_not(),
 assert_type(), assert_length(), and assert_path()).
 """
 import builtins
 import warnings
 
 from collections.abc import Iterable, Callable
 from math import isclose
+from numbers import Number
 from operator import eq, le, lt, gt, ge, ne, is_, is_not
 from pathlib import Path
 
 class LimitError(Exception):
     """Number out of limit."""
 
 
 class LengthError(Exception):
     """Violated length check."""
 
 
-class OperatorError(Exception):
-    """Invalid operator."""
-
-
 class ComparisonError(Exception):
     """The comparison is not true."""
 
 
 class NotCloseEnoughError(Exception):
     """The two float numbers are not close enough."""
 
 class ArgumentValueError(Exception):
     """Argument's value is incorrect."""
 
 
-class IncorrectMessageType(Exception):
-    """Argument message must be either None or string."""
-
-
 def check_if(condition, handle_with=AssertionError, message=None):
     """Check if a condition is true.
 
     Args:
         condition (bool): condition to check.
         handle_with (type): the type of exception to be raised or warning to
             be issued
@@ -94,25 +87,26 @@
     or
     >>> check_args = a < 50 and b > 100 and isinstance(c, str)
     >>> check_if(check_args)
 
     In such combined comparisons, you can easily use any logical operator:
     >>> check_if((a < 50 and b > 100) or isinstance(c, str))
 
-    To issue a warning, use the Warning class or its subclass:
-    >>> check_if(2 < 1, handle_with=Warning, message='2 is not smaller than 1')
+    To issue a warning, use the Warning class or its subclass
+    (we'll catch the warning here):
+    >>> with warnings.catch_warnings(record=True) as w:
+    ...     check_if(2 < 1, handle_with=Warning, message='2 is not smaller than 1')
+    ...     assert_if("2 is not smaller than 1" in str(w[-1].message))
 
     or shorter
-    >>> check_if(2 < 1, Warning, '2 is not smaller than 1')
-
+    >>> with warnings.catch_warnings(record=True) as w:
+    ...     check_if(2 < 1, Warning, '2 is not smaller than 1')
+    ...     assert_if("2 is not smaller than 1" in str(w[-1].message))
     """
     __tracebackhide__ = True
-    _check_easycheck_arguments(
-        handle_with=handle_with, message=message, condition=condition
-    )
     if not condition:
         _raise(handle_with, message)
 
 
 def check_if_not(condition, handle_with=AssertionError, message=None):
     """Check if a condition is not true.
 
@@ -167,24 +161,24 @@
     >>> BMI = 50
     >>> disaster = True if BMI > 30 else False
     >>> check_if_not(disaster, message='BMI disaster! Watch out for candies!')
     Traceback (most recent call last):
         ...
     AssertionError: BMI disaster! Watch out for candies!
 
-    To issue a warning, use the Warning class or one of its subclasses:
-    >>> check_if_not(2 > 1, Warning, '2 is not bigger than 1')
+    To issue a warning, use the Warning class or one of its subclasses
+    (we'll catch the warning):
+    >>> with warnings.catch_warnings(record=True) as w:
+    ...     check_if_not(2 > 1, Warning, '2 is bigger than 1')
+    ...     assert_if("2 is bigger than 1" in str(w[-1].message))
     """
     __tracebackhide__ = True
-    _check_easycheck_arguments(
-        handle_with=handle_with, message=message, condition=condition
-    )
-
-    check_if(not condition, handle_with=handle_with, message=message)
-
+    if condition:
+        _raise(handle_with, message)
+    
 
 def check_if_in_limits(
     x, 
     lower_limit = float('-inf'), 
     upper_limit = float('inf'), 
     handle_with=LimitError, 
     message=None,
@@ -226,25 +220,22 @@
     >>> check_if_in_limits(5, 1, 3)
     Traceback (most recent call last):
         ...
     LimitError: Number out of limit.
     >>> check_if_in_limits(5, 1, 3, Warning)
     """
     __tracebackhide__ = True
-    _check_easycheck_arguments(
-        handle_with=handle_with, 
-        message=message
-    )
     x = float(x)
     if include_equal:
         condition = lower_limit <= x <= upper_limit
     else:
         condition = lower_limit < x < upper_limit
 
-    check_if(condition, handle_with=handle_with, message=message)
+    if not condition:
+        _raise(handle_with, message)
 
 def check_length(
     item,
     expected_length,
     handle_with=LengthError,
     message=None,
     operator=eq,
@@ -284,28 +275,21 @@
     >>> check_length(2, 0, operator=gt, assign_length_to_others=True)
     >>> check_length(True, 1, assign_length_to_others=True)
 
     To issue a warning, use the Warning class or its subclass:
     >>> check_length('string', 6, Warning)
     """
     __tracebackhide__ = True
-    _check_easycheck_arguments(
-        handle_with=handle_with,
-        message=message,
-        operator=operator,
-        expected_length=expected_length,
-        assign_length_to_others=assign_length_to_others,
-    )
-
     if assign_length_to_others:
-        if isinstance(item, (int, float, complex, bool)):
+        if isinstance(item, (Number, bool)):
             item = [item]
 
-    condition_to_check = operator(len(item), expected_length)
-    check_if(condition_to_check, handle_with=handle_with, message=message)
+    condition = operator(len(item), expected_length)
+    if not condition:
+        _raise(handle_with, message)
 
 
 def check_type(item, expected_type, handle_with=TypeError, message=None):
     """Check if item has the type of expected_type.
 
     Args:
         item: the object whose type we want to validate
@@ -359,33 +343,26 @@
     >>> check_type('a', (str, None))
     >>> check_type(None, expected_type=(str, None))
 
     To issue a warning, do the following:
     >>> check_type('a', (str, None), Warning, 'Undesired instance')
     """
     __tracebackhide__ = True
-    _check_easycheck_arguments(
-        handle_with=handle_with, message=message, expected_type=expected_type
-    )
-
     if expected_type is None:
-        check_if(item is None, handle_with=handle_with, message=message)
+        if item is not None:
+            _raise(handle_with, message)
         return None
 
     if isinstance(expected_type, Iterable):
         if item is None and any(t is None for t in expected_type):
             return None
         expected_type = tuple(t for t in expected_type if t is not None)
 
-    check_if(
-        isinstance(item, expected_type),
-        handle_with=handle_with,
-        message=message,
-    )
-
+    if not isinstance(item, expected_type):
+        _raise(handle_with, message)
 
 
 def check_if_isclose(x, y, /,
                      handle_with=NotCloseEnoughError,
                      message=None,
                      rel_tol=1e-09, abs_tol=0.0):
     """Check if two floats are close in value.
@@ -448,23 +425,19 @@
 
     >>> check_if_isclose(1.12, 2.12, ValueError, rel_tol=1e-09)
     Traceback (most recent call last):
         ...
     ValueError
     """
     __tracebackhide__ = True
-    _check_easycheck_arguments(handle_with=handle_with, message=message)
     x = float(x)
     y = float(y)
 
-    check_if(
-        isclose(x, y, rel_tol=rel_tol, abs_tol=abs_tol),
-        handle_with,
-        message
-    )
+    if not isclose(x, y, rel_tol=rel_tol, abs_tol=abs_tol):
+        _raise(handle_with, message)
 
 
 def check_if_paths_exist(
     paths, handle_with=FileNotFoundError, message=None, execution_mode="raise"
 ):
     """Check if a path or paths exist.
 
@@ -506,41 +479,43 @@
     >>> check_if_paths_exist('Q:/Op/Oop', execution_mode='return')
     (FileNotFoundError(), ['Q:/Op/Oop'])
     >>> check_if_paths_exist(os.listdir()[0], execution_mode='return')
     (None, [])
     >>> check_if_paths_exist(os.listdir(), execution_mode='return')
     (None, [])
 
-    To issue a warning, do the following:
-    >>> check_if_paths_exist('Q:/Op/Oop', handle_with=Warning)
+    To issue a warning, do the following (we'll catch the warning):
+    >>> with warnings.catch_warnings(record=True) as w:
+    ...     check_if_paths_exist('Q:/Op/Oop', handle_with=Warning)
     >>> check_if_paths_exist('Q:/Op/Oop',
     ...    execution_mode='return',
     ...    handle_with=Warning)
     (Warning(), ['Q:/Op/Oop'])
     >>> check_if_paths_exist('Q:/Op/Oop',
     ...    execution_mode='return',
     ...    handle_with=Warning,
     ...    message='Attempt to use a non-existing path')
     (Warning('Attempt to use a non-existing path'), ['Q:/Op/Oop'])
     """
     __tracebackhide__ = True
-    _check_easycheck_arguments(
-        handle_with=handle_with, message=message, execution_mode=execution_mode
-    )
+    if not execution_mode in ("raise", "return"):
+        _raise(ValueError,
+               "execution_mode must be either 'raise' or 'return'")
 
     is_allowed_type = isinstance(paths, (str, Path)) or (
         isinstance(paths, Iterable)
         and all(isinstance(path, (str, Path)) for path in paths)
     )
 
-    check_if(
-        is_allowed_type,
-        TypeError,
-        "Argument paths must be string or pathlib.Path or iterable thereof",
-    )
+    if not is_allowed_type:
+        _raise(
+            TypeError,
+            "Argument paths must be string"
+            " or pathlib.Path or iterable thereof",
+        )
 
     error = None
 
     if isinstance(paths, (str, Path)):
         paths = (paths,)
 
     non_existing_paths = [
@@ -600,26 +575,23 @@
     ...                  handle_with=ComparisonError,
     ...                  message='Not less!')
     Traceback (most recent call last):
         ...
     ComparisonError: Not less!
 
     To issue a warning, do the following:
-    >>> check_comparison('one text', lt, 'another text',
-    ...                  handle_with=Warning,
-    ...                  message='Not less!')
+    >>> with warnings.catch_warnings(record=True) as w:
+    ...     check_comparison('one text', lt, 'another text',
+    ...         handle_with=Warning,
+    ...         message='Not less!')
+    ...     assert_if("Not less" in str(w[-1].message))
     """
     __tracebackhide__ = True
-    _check_easycheck_arguments(
-        handle_with=handle_with, message=message, operator=operator
-    )
-
-    check_if(
-        operator(item_1, item_2), handle_with=handle_with, message=message
-    )
+    if not operator(item_1, item_2):
+        _raise(handle_with, message)
 
 
 def check_all_ifs(*args):
     """Check all multiple conditions and return all checks.
 
     Args:
         args: tuples of the form (check_function, arguments), where:
@@ -775,19 +747,21 @@
     ArgumentValueError: Incorrect type of x; valid ... <class 'int'>
 
     This is how you can check exceptions and errors provided as arguments:
     >>> check_argument(TypeError, 'error_arg', expected_type=type)
     >>> check_argument(TypeError(), 'error_arg', expected_type=Exception)
 
     You can also issue a warning instead of raising an exception:
-    >>> check_argument(
-    ...    x, 'x',
-    ...    expected_type=int,
-    ...    handle_with=Warning,
-    ...    message="Incorrect argument's value")
+    >>> with warnings.catch_warnings(record=True) as w:
+    ...     check_argument(
+    ...         x, 'x',
+    ...         expected_type=int,
+    ...         handle_with=Warning,
+    ...         message="Incorrect argument's value")
+    ...     assert_if("Incorrect argument's value" in str(w[-1].message))
     """
     __tracebackhide__ = True
     if all(
         item is None
         for item in (expected_type, expected_choices, expected_length)
     ):
         raise ValueError(
@@ -800,78 +774,48 @@
         argument_name,
         str,
         handle_with=handle_with,
         message="argument_name must be string",
     )
 
     if expected_type is not None:
-        instance_message = _make_message(
-            message,
-            (
-                f"Incorrect type of {argument_name}; valid type(s):"
-                f" {expected_type}"
-            ),
-        )
+        instance_message = (
+            message
+            or f"Incorrect type of {argument_name}; valid type(s):"
+               f" {expected_type}"
+            )
         check_type(
             item=argument,
             expected_type=expected_type,
             handle_with=handle_with,
             message=instance_message,
         )
     if expected_choices is not None:
-        choices_message = _make_message(
-            message,
-            (
-                f"{argument_name}'s value, {argument}, "
-                f"is not among valid values: {expected_choices}."
-            ),
-        )
-        check_if(
-            argument in expected_choices,
-            handle_with=handle_with,
-            message=choices_message,
-        )
+        choices_message = (
+            message
+            or f"{argument_name}'s value, {argument}, "
+               f"is not among valid values: {expected_choices}."
+            )
+        if argument not in expected_choices:
+            _raise(handle_with, choices_message)
     if expected_length is not None:
-        length_message = _make_message(
-            message,
-            (
-                f"Unexpected length of {argument_name}"
-                f" (should be {expected_length})"
-            ),
-        )
+        length_message = (
+            message
+            or f"Unexpected length of {argument_name}"
+               f" (should be {expected_length})"
+            )
         check_length(
             item=argument,
             expected_length=expected_length,
             handle_with=handle_with,
             message=length_message,
             **kwargs,
         )
 
 
-def _make_message(message_provided, message_otherwise):
-    """If message was provided, use it; otherwise, use the alternative one.
-
-    Args:
-        message_provided: message to use if provided
-        message_otherwise: message to use if the first one was not provided
-
-    Returns:
-        First message that evaluates to True
-
-    This function is used by the check_argument() function.
-
-    >>> _make_message(None, 'Otherwise')
-    'Otherwise'
-    >>> _make_message('Provided', 'Otherwise')
-    'Provided'
-    """
-    __tracebackhide__ = True
-    return message_provided or message_otherwise
-
-
 def catch_check(check_function, *args, **kwargs):
     """Catch an exception or warning raised/issued by a easycheck function.
 
     Args:
         check_function: function to call (one of the public easycheck functions)
         args: positional arguments to pass on to check_function
         kwargs: keyword arguments to pass on to check_function
@@ -1048,121 +992,28 @@
         if not message:
             # Instead of passing an empty string,
             # better to pass None as message.
             message = None
         else:
             message = message
     else:
-        raise IncorrectMessageType(IncorrectMessageType.__doc__)
+        raise TypeError("Argument message must be either None or string")
 
     if issubclass(error, Warning):
         if message:
             warnings.warn(message, error)
         else:
             warnings.warn(error)
     elif issubclass(error, Exception):
         if message:
             raise error(message)
         else:
             raise error
 
 
-def _check_easycheck_arguments(
-    handle_with=None,
-    message=None,
-    condition=None,
-    operator=None,
-    assign_length_to_others=None,
-    execution_mode=None,
-    expected_length=None,
-    expected_type=None,
-):
-    """Validate the most common arguments used in easycheck functions.
-
-    This is a generic function that works for most easycheck functions, and can
-    be customized by providing selected arguments from a given function.
-    Other arguments, not included in this function, need to be checked using
-    other ways.
-
-    >>> _check_easycheck_arguments(handle_with=LengthError)
-    >>> _check_easycheck_arguments(handle_with=ValueError)
-
-    You must provide an exception (or warning) class, not its instance:
-    >>> _check_easycheck_arguments(handle_with=ValueError())
-    Traceback (most recent call last):
-        ...
-    TypeError: handle_with must be an exception
-
-    >>> _check_easycheck_arguments(handle_with=LengthError, message=False)
-    Traceback (most recent call last):
-        ...
-    TypeError: message must be either None or string
-    >>> _check_easycheck_arguments(handle_with=ValueError, condition=2<1)
-    """
-    __tracebackhide__ = True
-    if all(
-        argument is None
-        for argument in (
-            handle_with,
-            message,
-            condition,
-            operator,
-            assign_length_to_others,
-            execution_mode,
-            expected_length,
-            expected_type,
-        )
-    ):
-        raise ValueError("Provide at least one argument")
-
-    if handle_with is not None:
-        try:
-            is_subclass = issubclass(handle_with, Exception)
-        except TypeError:
-            is_subclass = False
-        if not is_subclass:
-            raise TypeError("handle_with must be an exception")
-    if message is not None:
-        if not isinstance(message, str):
-            raise TypeError("message must be either None or string")
-    if condition is not None:
-        if not isinstance(condition, bool):
-            raise ValueError("The condition does not return a boolean value")
-    if operator is not None:
-        if operator not in get_possible_operators():
-            raise OperatorError(
-                "Incorrect operator. Check get_possible_operators()"
-            )
-    if expected_length is not None:
-        if not isinstance(expected_length, (int, float)):
-            raise TypeError(
-                "expected_length should be an integer (or a float)"
-            )
-    if assign_length_to_others is not None:
-        if not isinstance(assign_length_to_others, bool):
-            raise TypeError(
-                "assign_length_to_others should be" " a boolean value"
-            )
-    if execution_mode is not None:
-        if execution_mode not in ("raise", "return"):
-            raise ValueError(
-                'execution_mode should be either "raise" or "return"'
-            )
-    if expected_type is not None:
-        if isinstance(expected_type, Iterable):
-            if any(
-                not isinstance(t, type) for t in expected_type if t is not None
-            ):
-                raise TypeError(
-                    "all items in expected_type must be valid types"
-                )
-        elif not isinstance(expected_type, type):
-            raise TypeError("expected_type must be a valid type")
-
-
 def get_possible_operators():
     """Provide a list of possible operators to be used in easycheck functions.
 
     All of these operators come from the operator module, but not all operators
     from this module are allowed.
 
     >>> operators = get_possible_operators()
@@ -1189,8 +1040,9 @@
 check_instance = check_type
 assert_instance = assert_type
 
 
 if __name__ == "__main__":
     import doctest
     
-    doctest.testmod()
+    flags = doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE
+    doctest.testmod(optionflags=flags)
```

### Comparing `easycheck-0.6.0/easycheck.egg-info/PKG-INFO` & `easycheck-0.7.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,279 +1,294 @@
 Metadata-Version: 2.1
 Name: easycheck
-Version: 0.6.0
-Summary: A tool for simple functionalized assertions in Python
+Version: 0.7.0
+Summary: A tool for checking conditions in Python
 Home-page: https://github.com/nyggus/easycheck
 Author: Nyggus & Ke Boan
 Author-email: nyggus@gmail.com
 License: MIT
+Description: easycheck
+        =========
+        
+        The :code:`easycheck` package offers a lightweight tool for running functionized checks within Python code; it also offers functions to be used in testing - particularly in doctests, but also in pytests, for which purpose some of the functions have dedicated aliases (starting off with :code:`assert_` instead of :code:`check_`).
+        
+        The idea is to use the :code:`easycheck` functions to check conditions that are _not_ assertions. The checks work in the following general way: When a condition is met, nothing happens (in fact, the function returns :code:`None`); if it is violated, an exception is raised or a warning is issued. The main differences between :code:`easycheck` functions and assertions are as follows:
+        
+        * Assertions are meant to be used conditions that _must_ be true (when only the code is correct). So, if an assertion is incorrect, it means something is wrong with the code. You should never use assertions to handle regular exceptions, like those related to data or arguments.
+        * Unlike assertions, :code:`easycheck` functions are to be used to check conditions related to things like data and argument values, and to handle regular exceptions.
+        * While assertions only raise :code:`AssertionError`, you can choose any exception to be raised by easycheck functions.
+        * When using :code:`easycheck`, instead of raising an exception, you can issue a warning.
+        
+        The main :code:`easycheck` functions (with names starting off with :code:`check_`) are designed in such a way that they can be used as easy-to-understand code that checks whether one or more conditions are met. They can be used instead of :code:`if`-blocks, which are normally used to check conditions and raise exceptions (or issue warnings) if they are not met. So, you can do the following:
+        
+        .. code-block:: python
+        
+            if not isinstance(x, (float, int)):
+                raise TypeError('x must be a number')
+            if x > 10:
+                raise ValueError('Too high value of x')
+        
+        or you can use :code:`easycheck` for this:
+        
+        .. code-block:: python
+        
+            check_type(x, (float, int), message='x must be a number')
+            check_if(x <= 10, ValueError, 'Too high value of x')
+        
+        The :code:`easycheck` approach has two main advantages over this classical approach:
+        
+        * It saves a little space; not much, since most often you'll end up with one line of code instead of two, but not always, particularly when you provide an exception type to be raised and a long message. 
+        * Mainly, it increases code simplicity and readability, since both the names of easycheck functions and their arguments are designed in such a way that the reader immediately understands what is being checked.
+        
+        You can also issue a warning:
+        
+        .. code-block:: python
+        
+            check_if(x <= 10,
+                     Warning,
+                     'For stable functioning of the function, '
+                     'x should not be greater than 10.')
+        
+        The package also offers functions dedicated to testing, e.g.,
+        
+        .. code-block:: python
+        
+            assert_type(x, (float, int))
+            assert_if(x <= 10)
+        
+        The :code:`message` argument has the default value of :code:`None`, which does the following. If the exception class provided in :code:`handle_with` is built-in (that is, can be found in :code:`dir(builtins)`), no message is provided. But if it is not a built-in exception (or warning) class, then the exception/warning class's docstring is taken as the message. This is a convenient way of providing a  typical message. If you want to customize the message (e.g., depending on the value of a variable), you should use a customized string (e.g., through an f-string). But if you do not want to use any message with a custom exception/warning, simply provide an empty string (:code:`message=''`).
+        
+        
+        Read about :code:`easycheck`
+        ----------------------------
+        
+        You will find more about assertions in `this article <https://medium.com/towards-data-science/python-assertions-or-checking-if-a-cat-is-a-dog-ce11c55d143>`_, entitled "Python Assertions, or Checking If a Cat Is a Dog" and published in *Towards Data Science*. It mentions :code:`easycheck`! You will read about :code:`easycheck` also in `the article "Comparing floating-point numbers with easycheck" <https://medium.com/towards-data-science/comparing-floating-point-numbers-with-easycheck-dcbae480f75f>`_  (also from *Towards Data Science*). The *Better Programming* article entitiled `"How to Overwrite AssertionError in Python and Use Custom Exceptions" <https://medium.com/better-programming/how-to-overwrite-asserterror-in-python-and-use-custom-exceptions-c0b252989977>`_, mentions the package, too.
+        
+        
+        Installing
+        ----------
+        
+        Install and update using pip:
+        
+        .. code-block:: text
+        
+            pip install easycheck
+        
+        Testing
+        -------
+        
+        The package is covered with both pytests and doctests. The latter are included in both docstrings of all the functions, but also in `documentation files <https://github.com/nyggus/easycheck/tree/master/docs>`_.
+        
+        Use in code to raise exceptions
+        -------------------------------
+        
+        Here are several examples of a simple use of basic :code:`easycheck` functions. The most basic usage resembles the following:
+        
+        .. code-block:: python
+        
+            check_if(a < 10)
+        	
+        This simply checks if :code:`a` is smaller than 10; if it is, nothing happens (in fact, :code:`check_if(a < 10)` returns :code:`None`). But if the condition is violated, the function raises :code:`AssertionError`. :code:`AssertionError` is the default exception returned by :code:`check_if()`, but you can change this:
+        
+        .. code-block:: python
+        
+            check_if(a < 10, handle_with=ValueError)
+            # or shorter and equally readable:
+            check_if(a < 10, ValueError)
+        
+        For built-in exceptions, like :code:`ValueError`, the default behaviour is to not print any message. For custom exceptions, however, the exception's docstring (`.__doc__`) serves as a message. You can use this when you create custom exceptions:
+        
+        .. code-block:: python
+        
+            class IncorrectNameTypeError(Exception):
+                """Argument name must be a string."""
+            
+            name = 40
+            check_type(name, IncorrectNameTypeError)
+            Traceback (most recent call last):
+              ...
+            IncorrectNameTypeError: Argument name must be a string.
+        
+        If you want to ensure that no message is printed, even for a custom exception, override the default behaviour by passing an empty string :code:`message=''`. You can also add a custom message:
+        
+        .. code-block:: python
+        
+            check_if(a < 10, handle_with=ValueError, message='Too high a')
+            # or shorter and equally readable:
+            check_if(a < 10, ValueError, 'Too high a')
+        
+        Some other functions have different default errors; for instance, this call
+        
+        .. code-block:: python
+        
+            check_type(a, expected_type=str)
+            # or shorter:
+            check_type(a, str)
+        
+        will raise :code:`TypeError` while this
+        
+        .. code-block:: python
+        
+            check_length([1, 2, 3], 1)
+        	
+        will raise :code:`LengthError` (an exception class defined in the :code:`easycheck` module).
+        
+        Here is a list of :code:`easycheck` functions the module offers, along with their aliases to be used for testing:
+        
+        * :code:`check_if()`, with the alias of :code:`assert_if()`; it's the most basic :code:`easycheck` function, similar to what you would get using :code:`if`;
+        * :code:`check_if_not()`, with the alias of :code:`assert_if_not()`; the opposite of :code:`check_if()`, helpful when you need to assure that a condition is _not_ met;
+        * :code:`check_if_isclose()`, with the alias of :code:`assert_if_isclose()`; to compare two floating-point numbers, based on :code:`match.isclose()` (see `this file <https://github.com/nyggus/easycheck/blob/master/docs/compare_floats_doctest.rst>`_);
+        * :code:`check_if_in_limits()`, with the alias of :code:`assert_if_in_limits()`;
+        * :code:`check_length()`, with the alias of :code:`assert_length()`; to compare length (equal to, smaller than, greater than, and the like);
+        * :code:`check_type()`, with the alias of :code:`assert_type()`; to check expected type, similar to :code:`isinstance()`;
+        * :code:`check_if_paths_exist()`, with the alias of :code:`assert_paths()`; to compare paths (or just one path) exist;
+        * :code:`check_comparison()` (used to compare two items); to compare to objectsm just like you would do using :code:`if obj1 != obj2: raise`
+        * :code:`check_all_ifs()`; used to check multiple conditions and return all the checks;
+        * :code:`check_argument()`; used to make one or more checks of a function's argument.
+        
+        You can also use a :code:`catch_check()` function, if you want to catch an exception or a warning the :code:`easycheck` function you use would raise (see examples `here <https://github.com/nyggus/easycheck/blob/master/docs/catch_exceptions_doctest.rst>`_). Sometimes, however, you will do better using a :code:`try-except` block to catch exceptions (`see examples <https://github.com/nyggus/easycheck/blob/master/docs/use_with_try_doctest.rst>`_).
+        
+        > Note that some :code:`easycheck` functions are simple wrappers around built-in functions, but their behavior is different, as they have the typical behavior of an :code:`easycheck` function: if a condition is not met, an exception is raised or an issue is raised.
+        
+        
+        Use in code to issue warnings
+        -----------------------------
+        
+        In order to issue a warning if a condition is violated, simply use a warning class (in the :code:`handle_with` argument) instead of an exception class:
+        
+        .. code-block:: python
+        
+            check_if(2 > 1, Warning, 'Too high a value')
+            check_length([1, 2, 3], 10, Warning, 'Too short list with data')
+        
+        Remember to always use a message with warnings, in order to make them meaningful. (See more in `use_with_warnings_doctest.rst <https://github.com/nyggus/easycheck/blob/master/docs/use_with_warnings_doctest.rst>`_).
+        
+        
+        Of course, you can use a custom warning:
+        
+        .. code-block:: python
+        
+            class TooSmallSampleSize(Warning):
+                """Results for samples size below 100 can be unstable."""
+            
+            n = 50
+            check_if(n >= 100, TooSmallSampleSize)
+            ... TooSmallSampleSize: Results for samples size below 100 can be unstable.
+              warnings.warn(message, error)
+        
+        
+        Use in code, an example
+        -----------------------
+        
+        Imagine you want to connect to a database; if the connection fails for any reason, you want to read an archived flat file. (We will use some undefined functions whose names will clearly convey what the functions do.)
+        
+        .. code-block:: python
+        
+            from easycheck import check_if, check_if_paths_exist
+            
+            class DataBaseConnectionError(Exception):
+                pass
+            
+            def get_data_from_db(db_details, db_credentials):
+                try:
+                    connect_to_db(db_details, db_credentials)
+                except:
+                    return False
+                data = get_records_from_db()
+                return data
+        
+        The :code:`easycheck` code could look like the following:
+        
+        .. code-block:: python
+        
+            def get_data(db_details, db_credentials):
+                data = get_data_from_db(db_details, db_credentials)
+                check_if(
+                    data,
+                    handle_with=DataBaseConnectionError,
+                    message='Cannot communicate with the database'
+                    )
+                return data
+                      
+        You can of course handle this exception, for example like here:
+        
+        .. code-block:: python
+        
+            def get_data(db_details, db_credentials, archived_data_file):
+                data = get_data_from_db(db_details, db_credentials)
+                try:
+                    check_if(
+                        data,
+                        handle_with=DataBaseConnectionError,
+                        message='Cannot communicate with the database'
+                    )
+                except DataBaseConnectionError:
+                    check_if_paths_exist(archived_data_file)
+                    with open(archived_data_file) as f:
+                        data = f.readlines()
+                return data
+            
+        Of course, you might use here a dedicated context manager. Sure, you can write it in a shorter way, without :code:`easycheck`, but the flow of information will not be as smooth, resulting in less readability:
+        
+        .. code-block:: python
+        
+            def get_data(db_details, db_credentials, archived_data_file):
+                data = get_data_from_db(db_details, db_credentials)
+                if not data:
+                    with open(archived_data_file) as f:
+                        data = f.readlines()
+                return data
+        
+        Of course, the :code:`open()` context manager will itself throw an error, but when you use the :code:`check_if()` function and explicitly define an exception class, you clearly show the reader that you're checking if this file exists and raise a particular exception if it doesn't.
+                
+        Use in testing
+        --------------
+        
+        As mentioned above, most :code:`easycheck` functions have aliases to be used in testing. Of course, you can use :code:`check_if()`, but to align with the common use of assertions, the :code:`easycheck` module offers those aliases so that the reader will immediately see that you're using these functions to test. Consider these examples:
+        
+        .. code-block:: python
+        
+            # Using assertions
+            def test_something():
+                a, b = my_function_1(), my_function_2()
+        
+                assert a == 2; 
+                assert isinstance(a, int)
+                assert isinstance(b, tuple)
+                assert len(b) == 5
+        		
+            # Using easycheck assert-like functions:
+            def test_something():
+                a, b = my_function_1(), my_function_2()
+                
+                assert_if(a == 2)
+                assert_type(a, int)
+                assert_type(b, tuple)
+                assert_length(b, 5)
+        
+        Note that only the first one will raise :code:`AssertionError` while the others will raise more meaningful errors (:code:`TypeError` and :code:`LengthError`), which may better explain the reasons that the tests did not pass.
+        
+        You will find more about using :code:`easycheck` in `use_in_testing_doctest.rst <https://github.com/nyggus/easycheck/blob/master/docs/use_in_testing_doctest.rst>`_.
+        
+        Other examples
+        --------------
+        
+        You will find a number of examples in `doctest files <https://github.com/nyggus/easycheck/tree/master/docs/>`_, which also serve as doctests.
+        
+        
+        Changelog
+        ---------
+        
+        * Version 0.6.0 came with significant optimization of performance. Before, :code:`easycheck` functions performed internal checks of the argument values provided to the function call. Most of these checks are not performed anymore, at least not for the most significant :code:`easycheck` functions, such as :code:`check_if()` or :code:`check_type()`. Some checks, however, are still done. These are mainly checks without which the behavior of the function would be either unwanted or unexpected. We decided to remove all checks that do not change much; for instance, they raise an error due to an incorrect type of an argument value — even though it would be raised anyway, but by the internal Python process, not by the :code:`easycheck` function itself. The point is to remove such unnecessary checks and that way remove the unnecessary :code:`if` blocks, which certainly add some cost to execution time. While one such check costs almost nothing, many of them (e.g., in a long loop) can mean a significant cost. As of version 0.6.0, we will try to optimize the performance of :code:`easycheck` by getting rid of such overhead costs, unless they are important for the behavior of the corresponding :code:`easycheck` function.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
-License-File: LICENSE
-
-easycheck
-=========
-
-The :code:`easycheck` package offers a lightweight tool for running functionized assertion-like checks within Python code; it also offers functions to be used in testing - particularly in doctests, but also in pytests, for which purpose some of the functions have dedicated aliases. The idea is to use the :code:`easycheck` functions in a similar way as assertions, but with more functionality and with a slightly different aim: When a condition you define is met, nothing happens (in fact, the function returns :code:`None`); if the condition is violated, an exception is raised or a warning is issued. The main differences between :code:`easycheck` functions and assertions are as follows:
-
-* While you should not use assertions in your Python code, you can do so with the :code:`easycheck` functions.
-* While assertions only raise :code:`AssertionError`, you can choose any exception to be raised by easycheck functions.
-* When using :code:`easycheck`, instead of raising an exception, you can issue a warning.
-
-The main :code:`easycheck` functions (with names starting off with :code:`check_`) are designed in such a way that they can be used as easy-to-understand code that checks whether one or more conditions are met. They can be used instead of :code:`if`-blocks, which are normally used to check conditions and raise exceptions (or issue warnings) if they are not met. So, you can do the following:
-
-.. code-block:: python
-
-    if not isinstance(x, (float, int)):
-        raise TypeError('x must be a number')
-    if x > 10:
-        raise ValueError('Too high value of x')
-
-or you can use :code:`easycheck` for this:
-
-.. code-block:: python
-
-    check_type(x, (float, int), message='x must be a number')
-    check_if(x <= 10, ValueError, 'Too high value of x')
-
-The :code:`easycheck` approach has two main advantages over this classical approach:
-
-* It saves a little space; not much, since most often you'll end up with one line of code instead of two, but not always, particularly when you provide an exception type to be raised and a long message. 
-* Mainly, it increases code simplicity and readability, since both the names of easycheck functions and their arguments are designed in such a way that the reader immediately understands what is being checked.
-
-You can also issue a warning:
-
-.. code-block:: python
-
-    check_if(x <= 10, Warning, 'For stable functioning of the function, x should not be greater than 10.')
-
-The package also offers functions dedicated to testing, e.g.,
-
-.. code-block:: python
-
-    assert_type(x, (float, int))
-    assert_if(x <= 10)
-
-The :code:`message` argument has the default value of :code:`None`, which does the following. If the exception class provided in :code:`handle_with` is built-in (that is, can be found in :code:`dir(builtins)`), no message is provided. But if it is not a built-in exception (or warning) class, then the exception/warning class's docstring is taken as the message. This is a convenient way of providing a  typical message. If you want to customize the message (e.g., depending on the value of a variable), you should use a customized string (e.g., through an f-string). But if you do not want to use any message with a custom exception/warning, simply provide an empty string (:code:`message=''`).
-
-
-Installing
-----------
-
-Install and update using pip:
-
-.. code-block:: text
-
-    pip install easycheck
-
-Testing
--------
-
-The package is covered with both pytests and doctests. The latter are included in both docstrings of all the functions, but also in `documentation files <https://github.com/nyggus/easycheck/tree/master/docs>`_.
-
-Use in code to raise exceptions
--------------------------------
-
-Here are several examples of a simple use of basic :code:`easycheck` functions. The most basic usage resembles the following:
-
-.. code-block:: python
-
-    check_if(a < 10)
-	
-This simply checks if :code:`a` is smaller than 10; if it is, nothing happens (in fact, :code:`check_if(a < 10)` returns :code:`None`). But if the condition is violated, the function raises :code:`AssertionError`. :code:`AssertionError` is the default exception returned by :code:`check_if()`, but you can change this:
-
-.. code-block:: python
-
-    check_if(a < 10, handle_with=ValueError)
-    # or shorter and equally readable:
-    check_if(a < 10, ValueError)
-
-For built-in exceptions, like :code:`ValueError`, the default behaviour is to not print any message. For custom exceptions, however, the exception's docstring (`.__doc__`) serves as a message. You can use this when you create custom exceptions:
-
-.. code-block:: python
-
-    class IncorrectNameTypeError(Exception):
-        """Argument name must be a string."""
-    
-    name = 40
-    check_type(name, IncorrectNameTypeError)
-    Traceback (most recent call last):
-      ...
-    IncorrectNameTypeError: Argument name must be a string.
-
-If you want to ensure that no message is printed, even for a custom exception, override the default behaviour by passing an empty string :code:`message=''`. You can also add a custom message:
-
-.. code-block:: python
-
-    check_if(a < 10, handle_with=ValueError, message='Too high a')
-    # or shorter and equally readable:
-    check_if(a < 10, ValueError, 'Too high a')
-
-Some other functions have different default errors; for instance, this call
-
-.. code-block:: python
-
-    check_type(a, expected_type=str)
-    # or shorter:
-    check_type(a, str)
-
-will raise :code:`TypeError` while this
-
-.. code-block:: python
-
-    check_length([1, 2, 3], 1)
-	
-will raise :code:`LengthError` (an exception class defined in the :code:`easycheck` module).
-
-Here is a list of :code:`easycheck` functions the module offers, along with their aliases to be used for testing:
-
-* :code:`check_if()`, with the alias of :code:`assert_if()`; it's the most basic :code:`easycheck` function, similar to what you would get using :code:`if`;
-* :code:`check_if_not()`, with the alias of :code:`assert_if_not()`; the opposite of :code:`check_if()`, helpful when you need to assure that a condition is _not_ met;
-* :code:`check_if_isclose()`, with the alias of :code:`assert_if_isclose()`; to compare two floating-point numbers, based on :code:`match.isclose()` (see `this file <https://github.com/nyggus/easycheck/blob/master/docs/compare_floats_doctest.rst>`_);
-* :code:`check_if_in_limits()`, with the alias of :code:`assert_if_in_limits()`;
-* :code:`check_length()`, with the alias of :code:`assert_length()`; to compare length (equal to, smaller than, greater than, and the like);
-* :code:`check_type()`, with the alias of :code:`assert_type()`; to check expected type, similar to :code:`isinstance()`;
-* :code:`check_if_paths_exist()`, with the alias of :code:`assert_paths()`; to compare paths (or just one path) exist;
-* :code:`check_comparison()` (used to compare two items); to compare to objectsm just like you would do using :code:`if obj1 != obj2: raise`
-* :code:`check_all_ifs()`; used to check multiple conditions and return all the checks;
-* :code:`check_argument()`; used to make one or more checks of a function's argument.
-
-You can also use a :code:`catch_check()` function, if you want to catch an exception or a warning the :code:`easycheck` function you use would raise (see examples `here <https://github.com/nyggus/easycheck/blob/master/docs/catch_exceptions_doctest.rst>`_). Sometimes, however, you will do better using a :code:`try-except` block to catch exceptions (`see examples <https://github.com/nyggus/easycheck/blob/master/docs/use_with_try_doctest.rst>`_).
-
-> Note that some :code:`easycheck` functions are simple wrappers around built-in functions, but their behavior is different, as they have the typical behavior of an :code:`easycheck` function: if a condition is not met, an exception is raised or an issue is raised.
-
-
-Use in code to issue warnings
------------------------------
-
-In order to issue a warning if a condition is violated, simply use a warning class (in the :code:`handle_with` argument) instead of an exception class:
-
-.. code-block:: python
-
-    check_if(2 > 1, Warning, 'Too high a value')
-    check_length([1, 2, 3], 10, Warning, 'Too short list with data')
-
-Remember to always use a message with warnings, in order to make them meaningful. (See more in `use_with_warnings_doctest.rst <https://github.com/nyggus/easycheck/blob/master/docs/use_with_warnings_doctest.rst>`_).
-
-
-Of course, you can use a custom warning:
-
-.. code-block:: python
-
-    class TooSmallSampleSize(Warning):
-        """Results for samples size below 100 can be unstable."""
-    
-    n = 50
-    check_if(n >= 100, TooSmallSampleSize)
-    ... TooSmallSampleSize: Results for samples size below 100 can be unstable.
-      warnings.warn(message, error)
-
-
-Use in code, an example
------------------------
-
-Imagine you want to connect to a database; if the connection fails for any reason, you want to read an archived flat file. (We will use some undefined functions whose names will clearly convey what the functions do.)
-
-.. code-block:: python
-
-    from easycheck import check_if, check_if_paths_exist
-    
-    class DataBaseConnectionError(Exception):
-        pass
-    
-    def get_data_from_db(db_details, db_credentials):
-        try:
-            connect_to_db(db_details, db_credentials)
-        except:
-            return False
-        data = get_records_from_db()
-        return data
-
-The :code:`easycheck` code could look like the following:
-
-.. code-block:: python
-
-    def get_data(db_details, db_credentials):
-        data = get_data_from_db(db_details, db_credentials)
-        check_if(
-            data,
-            handle_with=DataBaseConnectionError,
-            message='Cannot communicate with the database'
-            )
-        return data
-              
-You can of course handle this exception, for example like here:
-
-.. code-block:: python
-
-    def get_data(db_details, db_credentials, archived_data_file):
-        data = get_data_from_db(db_details, db_credentials)
-        try:
-            check_if(
-                data,
-                handle_with=DataBaseConnectionError,
-                message='Cannot communicate with the database'
-            )
-        except DataBaseConnectionError:
-            check_if_paths_exist(archived_data_file)
-            with open(archived_data_file) as f:
-                data = f.readlines()
-        return data
-    
-Of course, you might use here a dedicated context manager. Sure, you can write it in a shorter way, without :code:`easycheck`, but the flow of information will not be as smooth, resulting in less readability:
-
-.. code-block:: python
-
-    def get_data(db_details, db_credentials, archived_data_file):
-        data = get_data_from_db(db_details, db_credentials)
-        if not data:
-            with open(archived_data_file) as f:
-                data = f.readlines()
-        return data
-
-Of course, the :code:`open()` context manager will itself throw an error, but when you use the :code:`check_if()` function and explicitly define an exception class, you clearly show the reader that you're checking if this file exists and raise a particular exception if it doesn't.
-        
-Use in testing
---------------
-
-As mentioned above, most :code:`easycheck` functions have aliases to be used in testing. Of course, you can use :code:`check_if()`, but to align with the common use of assertions, the :code:`easycheck` module offers those aliases so that the reader will immediately see that you're using these functions to test. Consider these examples:
-
-.. code-block:: python
-
-    # Using assertions
-    def test_something():
-        a, b = my_function_1(), my_function_2()
-
-        assert a == 2; 
-        assert isinstance(a, int)
-        assert isinstance(b, tuple)
-        assert len(b) == 5
-		
-    # Using easycheck assert-like functions:
-    def test_something():
-        a, b = my_function_1(), my_function_2()
-        
-        assert_if(a == 2)
-        assert_type(a, int)
-        assert_type(b, tuple)
-        assert_length(b, 5)
-
-Note that only the first one will raise :code:`AssertionError` while the others will raise more meaningful errors (:code:`TypeError` and :code:`LengthError`), which may better explain the reasons that the tests did not pass.
-
-You will find more about using :code:`easycheck` in `use_in_testing_doctest.rst <https://github.com/nyggus/easycheck/blob/master/docs/use_in_testing_doctest.rst>`_.
-
-Other examples
---------------
-
-You will find a number of examples in `doctest files <https://github.com/nyggus/easycheck/tree/master/docs/>`_, which also serve as doctests.
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `easycheck-0.6.0/setup.py` & `easycheck-0.7.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 
 extras_requirements = {
     "dev": ["pytest", "wheel", "black"],
 }
 
 setuptools.setup(
     name="easycheck",
-    version="0.6.0",
+    version="0.7.0",
     author="Nyggus & Ke Boan",
     author_email="nyggus@gmail.com",
     license="MIT",
-    description="A tool for simple functionalized assertions in Python",
+    description="A tool for checking conditions in Python",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/nyggus/easycheck",
     packages=setuptools.find_packages(),
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.8",
     extras_require=extras_requirements,
 )
```

