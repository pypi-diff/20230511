# Comparing `tmp/aiokit-1.1.3-py3-none-any.whl.zip` & `tmp/aiokit-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3836 bytes, number of entries: 7
--rw-r--r--  2.0 unx      176 b- defN 22-Sep-13 12:14 aiokit/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 22-Aug-15 06:28 aiokit/aiothing.py
--rw-r--r--  2.0 unx     3817 b- defN 22-Sep-13 12:14 aiokit/executors.py
--rw-r--r--  2.0 unx     1226 b- defN 22-Sep-13 12:14 aiokit/utils.py
-?rw-------  2.0 unx       91 b- defN 22-Sep-22 10:17 aiokit-1.1.3.dist-info/WHEEL
-?rw-------  2.0 unx      326 b- defN 22-Sep-22 10:17 aiokit-1.1.3.dist-info/METADATA
-?rw-------  2.0 unx      499 b- defN 22-Sep-22 10:17 aiokit-1.1.3.dist-info/RECORD
-7 files, 8881 bytes uncompressed, 2966 bytes compressed:  66.6%
+Zip file size: 3919 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      176 b- defN 22-Oct-25 09:23 aiokit/__init__.py
+-rw-r--r--  2.0 unx     3085 b- defN 22-Nov-29 23:24 aiokit/aiothing.py
+-rw-r--r--  2.0 unx     4046 b- defN 22-Oct-25 09:23 aiokit/executors.py
+-rw-r--r--  2.0 unx     1226 b- defN 22-Oct-25 09:23 aiokit/utils.py
+?rw-------  2.0 unx       91 b- defN 22-Dec-03 22:52 aiokit-1.2.0.dist-info/WHEEL
+?rw-------  2.0 unx      326 b- defN 22-Dec-03 22:52 aiokit-1.2.0.dist-info/METADATA
+?rw-------  2.0 unx      499 b- defN 22-Dec-03 22:52 aiokit-1.2.0.dist-info/RECORD
+7 files, 9449 bytes uncompressed, 3049 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -6,17 +6,17 @@
 
 Filename: aiokit/executors.py
 Comment: 
 
 Filename: aiokit/utils.py
 Comment: 
 
-Filename: aiokit-1.1.3.dist-info/WHEEL
+Filename: aiokit-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: aiokit-1.1.3.dist-info/METADATA
+Filename: aiokit-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: aiokit-1.1.3.dist-info/RECORD
+Filename: aiokit-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiokit/aiothing.py

```diff
@@ -22,15 +22,24 @@
             self.setup_hooks()
             for aw in self.starts:
                 logging.getLogger('debug').debug({
                     'action': 'start',
                     'mode': 'aiothing',
                     'class': str(aw),
                 })
-                await aw.start()
+                try:
+                    await aw.start()
+                except Exception as e:
+                    logging.getLogger('error').error({
+                        'action': 'start',
+                        'mode': 'aiothing',
+                        'class': str(aw),
+                        'error': str(e)
+                    })
+                    raise e
             r = await fn(*args, **kwargs)
             self._started_event.set()
             return r
         return guarded_fn
 
     def _guard_stop(self, fn):
         async def guarded_fn(*args, **kwargs):
```

## aiokit/executors.py

```diff
@@ -84,18 +84,23 @@
                         'pid': process.pid
                     })
                     self.stop_children(signal.SIGTERM)
                     for process_to_join in self.processes:
                         logger.debug({
                             'action': 'join',
                             'mode': 'join',
-                            'exitcode': process.exitcode,
-                            'pid': process.pid
+                            'pid': process_to_join.pid
                         })
                         process_to_join.join()
+                        logger.debug({
+                            'action': 'joined',
+                            'mode': 'join',
+                            'exitcode': process_to_join.exitcode,
+                            'pid': process_to_join.pid
+                        })
                     logger.debug({
                         'action': 'all_processes_exited',
                         'mode': 'join',
                     })
                     return
             time.sleep(1.0)
```

