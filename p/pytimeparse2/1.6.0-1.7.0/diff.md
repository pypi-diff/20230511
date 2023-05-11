# Comparing `tmp/pytimeparse2-1.6.0.tar.gz` & `tmp/pytimeparse2-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytimeparse2-1.6.0.tar", last modified: Thu Jan 26 09:46:00 2023, max compression
+gzip compressed data, was "dist/pytimeparse2-1.7.0.tar", last modified: Thu May 11 21:21:40 2023, max compression
```

## Comparing `pytimeparse2-1.6.0.tar` & `pytimeparse2-1.7.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-01-26 09:46:00.000000 pytimeparse2-1.6.0/
--rw-rw-r--   0 grey      (1000) grey      (1000)     1082 2022-09-27 06:01:24.000000 pytimeparse2-1.6.0/LICENSE.rst
--rw-rw-r--   0 grey      (1000) grey      (1000)    14448 2023-01-26 09:26:40.000000 pytimeparse2-1.6.0/setup.py
--rw-rw-r--   0 grey      (1000) grey      (1000)     1232 2023-01-26 09:46:00.000000 pytimeparse2-1.6.0/setup.cfg
--rw-rw-r--   0 grey      (1000) grey      (1000)     4121 2023-01-26 09:46:00.000000 pytimeparse2-1.6.0/PKG-INFO
--rw-rw-r--   0 grey      (1000) grey      (1000)     2650 2022-09-27 06:01:24.000000 pytimeparse2-1.6.0/README.rst
-drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-01-26 09:46:00.000000 pytimeparse2-1.6.0/pytimeparse2.egg-info/
--rw-rw-r--   0 grey      (1000) grey      (1000)        1 2023-01-26 09:46:00.000000 pytimeparse2-1.6.0/pytimeparse2.egg-info/dependency_links.txt
--rw-rw-r--   0 grey      (1000) grey      (1000)     4121 2023-01-26 09:46:00.000000 pytimeparse2-1.6.0/pytimeparse2.egg-info/PKG-INFO
--rw-rw-r--   0 grey      (1000) grey      (1000)       13 2023-01-26 09:46:00.000000 pytimeparse2-1.6.0/pytimeparse2.egg-info/top_level.txt
--rw-rw-r--   0 grey      (1000) grey      (1000)        1 2023-01-26 09:45:58.000000 pytimeparse2-1.6.0/pytimeparse2.egg-info/not-zip-safe
--rw-rw-r--   0 grey      (1000) grey      (1000)      248 2023-01-26 09:46:00.000000 pytimeparse2-1.6.0/pytimeparse2.egg-info/SOURCES.txt
--rw-rw-r--   0 grey      (1000) grey      (1000)       57 2022-09-27 06:01:24.000000 pytimeparse2-1.6.0/MANIFEST.in
--rw-rw-r--   0 grey      (1000) grey      (1000)     7001 2023-01-26 09:35:12.000000 pytimeparse2-1.6.0/pytimeparse2.py
+drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/
+-rw-rw-r--   0 grey      (1000) grey      (1000)     1082 2022-09-27 06:01:24.000000 pytimeparse2-1.7.0/LICENSE.rst
+-rw-rw-r--   0 grey      (1000) grey      (1000)    14448 2023-05-04 20:38:21.000000 pytimeparse2-1.7.0/setup.py
+-rw-rw-r--   0 grey      (1000) grey      (1000)     1294 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/setup.cfg
+-rw-rw-r--   0 grey      (1000) grey      (1000)     4599 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/PKG-INFO
+-rw-rw-r--   0 grey      (1000) grey      (1000)     3103 2023-05-11 21:04:01.000000 pytimeparse2-1.7.0/README.rst
+drwxrwxr-x   0 grey      (1000) grey      (1000)        0 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/pytimeparse2.egg-info/
+-rw-rw-r--   0 grey      (1000) grey      (1000)        1 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/pytimeparse2.egg-info/dependency_links.txt
+-rw-rw-r--   0 grey      (1000) grey      (1000)       35 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/pytimeparse2.egg-info/requires.txt
+-rw-rw-r--   0 grey      (1000) grey      (1000)     4599 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/pytimeparse2.egg-info/PKG-INFO
+-rw-rw-r--   0 grey      (1000) grey      (1000)       13 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/pytimeparse2.egg-info/top_level.txt
+-rw-rw-r--   0 grey      (1000) grey      (1000)        1 2023-05-11 21:21:39.000000 pytimeparse2-1.7.0/pytimeparse2.egg-info/not-zip-safe
+-rw-rw-r--   0 grey      (1000) grey      (1000)      283 2023-05-11 21:21:40.000000 pytimeparse2-1.7.0/pytimeparse2.egg-info/SOURCES.txt
+-rw-rw-r--   0 grey      (1000) grey      (1000)       57 2022-09-27 06:01:24.000000 pytimeparse2-1.7.0/MANIFEST.in
+-rw-rw-r--   0 grey      (1000) grey      (1000)     9017 2023-05-11 21:16:40.000000 pytimeparse2-1.7.0/pytimeparse2.py
```

### Comparing `pytimeparse2-1.6.0/LICENSE.rst` & `pytimeparse2-1.7.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pytimeparse2-1.6.0/setup.py` & `pytimeparse2-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytimeparse2-1.6.0/setup.cfg` & `pytimeparse2-1.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,18 @@
 	Topic :: Utilities
 
 [options]
 zip_safe = False
 include_package_data = True
 python_requires = >=3.6
 
+[options.extras_require]
+dateutil = 
+	python-dateutil~=2.8.2
+
 [build_sphinx]
 project = 'pytimeparse2'
 
 [aliases]
 
 [egg_info]
 tag_build =
```

### Comparing `pytimeparse2-1.6.0/PKG-INFO` & `pytimeparse2-1.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytimeparse2
-Version: 1.6.0
+Version: 1.7.0
 Summary: Time expression parser.
 Home-page: https://github.com/onegreyonewhite/pytimeparse2
 Author: Sergey Klyuykov
 Author-email: onegreyonewhite@mail.ru
 License: MIT
 Project-URL: Issue Tracker, https://github.com/onegreyonewhite/pytimeparse2/-/issues
 Project-URL: Source Code, https://github.com/onegreyonewhite/pytimeparse2.git
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+Provides-Extra: dateutil
 License-File: LICENSE.rst
 
 pytimeparse2: time expression parser
 =====================================
 
 .. image:: https://github.com/onegreyonewhite/pytimeparse2/actions/workflows/check.yml/badge.svg?branch=master
     :target: https://github.com/onegreyonewhite/pytimeparse2/actions
@@ -104,14 +105,24 @@
 
 - ``2 mo``
 - ``2 months``
 - ``3y``
 - ``3 years``
 - ``1y2mo3w4d5h6m7s8ms``
 
+For better capability with dates, use keyword ``as_timedelta=True`` which mark for function returns
+value as ``datetime.timedelta`` or ``dateutil.relitivedelta.relativedelta`` (if installed)::
+
+    >>> from pytimeparse import parse
+    >>> parse('24h', as_timedelta=True)
+    relativedelta(days=+1)
+
+You can also forced disable dateutil support by calling ``disable_dateutil()`` before ``parse(...)``.
+For returning support call ``enable_dateutil()``.
+
 Notes
 -----
 
 A number of seconds can be converted back into a string using the
 ``datetime`` module in the standard library, as noted in
 `this other StackOverflow question <http://stackoverflow.com/questions/538666/python-format-timedelta-to-string>`_::
```

### Comparing `pytimeparse2-1.6.0/README.rst` & `pytimeparse2-1.7.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -70,14 +70,24 @@
 
 - ``2 mo``
 - ``2 months``
 - ``3y``
 - ``3 years``
 - ``1y2mo3w4d5h6m7s8ms``
 
+For better capability with dates, use keyword ``as_timedelta=True`` which mark for function returns
+value as ``datetime.timedelta`` or ``dateutil.relitivedelta.relativedelta`` (if installed)::
+
+    >>> from pytimeparse import parse
+    >>> parse('24h', as_timedelta=True)
+    relativedelta(days=+1)
+
+You can also forced disable dateutil support by calling ``disable_dateutil()`` before ``parse(...)``.
+For returning support call ``enable_dateutil()``.
+
 Notes
 -----
 
 A number of seconds can be converted back into a string using the
 ``datetime`` module in the standard library, as noted in
 `this other StackOverflow question <http://stackoverflow.com/questions/538666/python-format-timedelta-to-string>`_::
```

### Comparing `pytimeparse2-1.6.0/pytimeparse2.egg-info/PKG-INFO` & `pytimeparse2-1.7.0/pytimeparse2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytimeparse2
-Version: 1.6.0
+Version: 1.7.0
 Summary: Time expression parser.
 Home-page: https://github.com/onegreyonewhite/pytimeparse2
 Author: Sergey Klyuykov
 Author-email: onegreyonewhite@mail.ru
 License: MIT
 Project-URL: Issue Tracker, https://github.com/onegreyonewhite/pytimeparse2/-/issues
 Project-URL: Source Code, https://github.com/onegreyonewhite/pytimeparse2.git
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+Provides-Extra: dateutil
 License-File: LICENSE.rst
 
 pytimeparse2: time expression parser
 =====================================
 
 .. image:: https://github.com/onegreyonewhite/pytimeparse2/actions/workflows/check.yml/badge.svg?branch=master
     :target: https://github.com/onegreyonewhite/pytimeparse2/actions
@@ -104,14 +105,24 @@
 
 - ``2 mo``
 - ``2 months``
 - ``3y``
 - ``3 years``
 - ``1y2mo3w4d5h6m7s8ms``
 
+For better capability with dates, use keyword ``as_timedelta=True`` which mark for function returns
+value as ``datetime.timedelta`` or ``dateutil.relitivedelta.relativedelta`` (if installed)::
+
+    >>> from pytimeparse import parse
+    >>> parse('24h', as_timedelta=True)
+    relativedelta(days=+1)
+
+You can also forced disable dateutil support by calling ``disable_dateutil()`` before ``parse(...)``.
+For returning support call ``enable_dateutil()``.
+
 Notes
 -----
 
 A number of seconds can be converted back into a string using the
 ``datetime`` module in the standard library, as noted in
 `this other StackOverflow question <http://stackoverflow.com/questions/538666/python-format-timedelta-to-string>`_::
```

### Comparing `pytimeparse2-1.6.0/pytimeparse2.py` & `pytimeparse2-1.7.0/pytimeparse2.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,45 +26,53 @@
 # MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = '1.6.0'
+__version__ = '1.7.0'
 
 import typing
 import re
+from datetime import timedelta
+
+try:
+    from dateutil.relativedelta import relativedelta
+    HAS_RELITIVE_TIMEDELTA = True
+except ImportError:  # pragma: no cover
+    HAS_RELITIVE_TIMEDELTA = False
+    relativedelta = None  # type: ignore
 
 
 SIGN = r'(?P<sign>[+|-]|\+)?'
 YEARS = r'(?P<years>[\d.]+)\s*(?:ys?|yrs?.?|years?)'
 MONTHS = r'(?P<months>[\d.]+)\s*(?:mos?.?|mths?.?|months?)'
 WEEKS = r'(?P<weeks>[\d.]+)\s*(?:w|wks?|weeks?)'
 DAYS = r'(?P<days>[\d.]+)\s*(?:d|dys?|days?)'
 HOURS = r'(?P<hours>[\d.]+)\s*(?:h|hrs?|hours?)'
-MINS = r'(?P<mins>[\d.]+)\s*(?:m|(mins?)|(minutes?))'
-SECS = r'(?P<secs>[\d.]+)\s*(?:s|secs?|seconds?)'
-MILLIS = r'(?P<millis>[\d.]+)\s*(?:ms|msecs?|millis|milliseconds?)'
+MINS = r'(?P<minutes>[\d.]+)\s*(?:m|(mins?)|(minutes?))'
+SECS = r'(?P<seconds>[\d.]+)\s*(?:s|secs?|seconds?)'
+MILLIS = r'(?P<milliseconds>[\d.]+)\s*(?:ms|msecs?|millis|milliseconds?)'
 SEPARATORS = r'[,/]'
-SECCLOCK = r':(?P<secs>\d{2}(?:\.\d+)?)'
-MINCLOCK = r'(?P<mins>\d{1,2}):(?P<secs>\d{2}(?:\.\d+)?)'
-HOURCLOCK = r'(?P<hours>\d+):(?P<mins>\d{2}):(?P<secs>\d{2}(?:\.\d+)?)'
+SECCLOCK = r':(?P<seconds>\d{2}(?:\.\d+)?)'
+MINCLOCK = r'(?P<minutes>\d{1,2}):(?P<seconds>\d{2}(?:\.\d+)?)'
+HOURCLOCK = r'(?P<hours>\d+):(?P<minutes>\d{2}):(?P<seconds>\d{2}(?:\.\d+)?)'
 DAYCLOCK = (r'(?P<days>\d+):(?P<hours>\d{2}):'
-            r'(?P<mins>\d{2}):(?P<secs>\d{2}(?:\.\d+)?)')
+            r'(?P<minutes>\d{2}):(?P<seconds>\d{2}(?:\.\d+)?)')
 
 MULTIPLIERS = {
     'years': 60 * 60 * 24 * 365,
     'months': 60 * 60 * 24 * 30,
     'weeks': 60 * 60 * 24 * 7,
     'days': 60 * 60 * 24,
     'hours': 60 * 60,
-    'mins': 60,
-    'secs': 1,
-    'millis': 1e-3,
+    'minutes': 60,
+    'seconds': 1,
+    'milliseconds': 1e-3,
 }
 
 
 def OPT(x):
     return r'(?:{x})?'.format(x=x)
 
 
@@ -93,61 +101,72 @@
 COMPILED_SIGN = re.compile(r'\s*' + SIGN + r'\s*(?P<unsigned>.*)$')
 COMPILED_TIMEFORMATS = [
     re.compile(r'\s*' + timefmt + r'\s*$', re.I)
     for timefmt in TIMEFORMATS
 ]
 
 
-def _all_digits(mdict):
-    digits_sum = 0
-    should_int = True
+def _all_digits(mdict, delta_class):
+    if HAS_RELITIVE_TIMEDELTA and issubclass(delta_class, relativedelta):
+        if 'milliseconds' in mdict:
+            mdict['microseconds'] = float(mdict.pop('milliseconds') or 0) * 1000
+        return delta_class(**{k: float(v) for k, v in mdict.items() if v}).normalized()
+
+    delta = delta_class(**{
+        key: float(mdict.pop(key) or 0)
+        for key in mdict.copy()
+        if key in ('hours', 'minutes', 'days', 'milliseconds')
+    })
 
     for time_type, value in mdict.items():
         if not value:
             continue
         if value.isdigit():
-            digits_sum += MULTIPLIERS[time_type] * int(value, 10)
-            if time_type == 'millis':
-                should_int = False
+            delta += delta_class(seconds=MULTIPLIERS[time_type] * int(value, 10))
         elif value.replace('.', '', 1).isdigit():
-            digits_sum += MULTIPLIERS[time_type] * float(value)
-            if time_type == 'secs':
-                should_int = False
-
-    if should_int:
-        return int(digits_sum)
-    return digits_sum
+            delta += delta_class(seconds=MULTIPLIERS[time_type] * float(value))
+
+    return delta
 
 
 def _interpret_as_minutes(sval, mdict):
     """
     Times like "1:22" are ambiguous; do they represent minutes and seconds
     or hours and minutes?  By default, parse assumes the latter.  Call
     this function after parsing out a dictionary to change that assumption.
 
     >>> import pprint
-    >>> pprint.pprint(_interpret_as_minutes('1:24', {'secs': '24', 'mins': '1'}))
-    {'hours': '1', 'mins': '24'}
+    >>> pprint.pprint(_interpret_as_minutes('1:24', {'seconds': '24', 'minutes': '1'}))
+    {'hours': '1', 'minutes': '24'}
     """
     if sval.count(':') == 1 and '.' not in sval and (('hours' not in mdict) or (mdict['hours'] is None)) and (
             ('days' not in mdict) or (mdict['days'] is None)) and (('weeks' not in mdict) or (mdict['weeks'] is None)) \
             and (('months' not in mdict) or (mdict['months'] is None)) \
             and (('years' not in mdict) or (mdict['years'] is None)):
-        mdict['hours'] = mdict['mins']
-        mdict['mins'] = mdict['secs']
-        mdict.pop('secs')
+        mdict['hours'] = mdict['minutes']
+        mdict['minutes'] = mdict['seconds']
+        mdict.pop('seconds')
     return mdict
 
 
+def _normilized_relativedelta(value: typing.Optional[timedelta]) -> typing.Optional[timedelta]:
+    if isinstance(value, relativedelta):
+        return value.normalized()
+    return value
+
+
 def _parse(
         sval: typing.Union[str, int, float],
-        granularity: str = 'seconds'
-) -> typing.Optional[typing.Union[int, float]]:
+        granularity: str = 'seconds',
+        delta_class: typing.Type[timedelta] = timedelta
+) -> typing.Optional[timedelta]:
     if isinstance(sval, (int, float)):
-        return int(sval)
+        return _normilized_relativedelta(delta_class(seconds=float(sval)))
+    if sval.replace('.', '', 1).replace('-', '', 1).replace('+', '', 1).isdigit():
+        return _normilized_relativedelta(delta_class(seconds=float(sval)))
 
     match = COMPILED_SIGN.match(sval)
     sign = -1 if match.groupdict()['sign'] == '-' else 1  # type: ignore
     sval = match.groupdict()['unsigned']  # type: ignore
 
     for timefmt in COMPILED_TIMEFORMATS:
         match = timefmt.match(sval)
@@ -155,34 +174,47 @@
         if not (match and match.group(0).strip()):
             continue
 
         mdict = match.groupdict()
         if granularity == 'minutes':
             mdict = _interpret_as_minutes(sval, mdict)
 
-        return sign * _all_digits(mdict)
+        return sign * _all_digits(mdict, delta_class)
+
+    return timedelta(seconds=float(sval)) * sign
 
-    return int(float(sval)) * sign
+
+def enable_dateutil():
+    global HAS_RELITIVE_TIMEDELTA
+    assert relativedelta is not None, 'Module python-dateutil should be installed before.'
+    HAS_RELITIVE_TIMEDELTA = True
+
+
+def disable_dateutil():
+    global HAS_RELITIVE_TIMEDELTA
+    HAS_RELITIVE_TIMEDELTA = False
 
 
 def parse(
         sval: typing.Union[str, int, float],
         granularity: str = 'seconds',
         raise_exception: bool = False,
-) -> typing.Optional[typing.Union[int, float, typing.NoReturn]]:
+        as_timedelta: bool = False,
+) -> typing.Optional[typing.Union[int, float, timedelta, typing.NoReturn]]:
     """
     Parse a time expression, returning it as a number of seconds.  If
     possible, the return value will be an `int`; if this is not
     possible, the return will be a `float`.  Returns `None` if a time
     expression cannot be parsed from the given string.
 
     Arguments:
     - `sval`: the string value to parse
     - `granularity`: minimal type of digits after last colon (default is ``seconds``)
     - `raise_exception`: raise exception on parsing errors (default is ``False``)
+    - `as_timedelta`: return ``datetime.timedelta`` object instead of ``int`` (default is ``False``)
 
     >>> parse('1:24')
     84
     >>> parse(':22')
     22
     >>> parse('1 minute, 24 secs')
     84
@@ -204,21 +236,35 @@
     a colon will be interpreted as minutes; otherwise they are considered seconds.
 
     >>> parse('1:30')
     90
     >>> parse('1:30', granularity='minutes')
     5400
 
+    If ``as_timedelta`` is specified as ``True``, then return timedelta object.
+
+    >>> parse('24h', as_timedelta=True)
+    relativedelta(days=+1)
+    >>> parse('48:00', as_timedelta=True, granularity='minutes')
+    relativedelta(days=+2)
+
     If ``raise_exception`` is specified as ``True``, then exception will raised
     on failed parsing.
 
     >>> parse(':1.1.1', raise_exception=True)
     Traceback (most recent call last):
         ...
     ValueError: could not convert string to float: ':1.1.1'
     """
     try:
-        return _parse(sval, granularity)
+        value = _parse(sval, granularity, relativedelta if HAS_RELITIVE_TIMEDELTA and as_timedelta else timedelta)
+        if not as_timedelta and value is not None:
+            new_value = value.total_seconds()
+            if new_value.is_integer():
+                return int(new_value)
+            else:
+                return new_value
+        return value
     except Exception:
         if raise_exception:
             raise
         return None
```

