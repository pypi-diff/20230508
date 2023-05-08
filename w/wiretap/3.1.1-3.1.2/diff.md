# Comparing `tmp/wiretap-3.1.1-py3-none-any.whl.zip` & `tmp/wiretap-3.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4654 bytes, number of entries: 7
+Zip file size: 4686 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      199 b- defN 23-May-08 08:36 wiretap/__init__.py
 -rw-rw-rw-  2.0 fat      620 b- defN 23-Feb-08 09:16 wiretap/layers.py
--rw-rw-rw-  2.0 fat    10750 b- defN 23-May-08 09:05 wiretap/wiretap.py
--rw-rw-rw-  2.0 fat      244 b- defN 23-May-08 09:06 wiretap-3.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-08 09:06 wiretap-3.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-08 09:06 wiretap-3.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      520 b- defN 23-May-08 09:06 wiretap-3.1.1.dist-info/RECORD
-7 files, 12433 bytes uncompressed, 3736 bytes compressed:  70.0%
+-rw-rw-rw-  2.0 fat    10833 b- defN 23-May-08 09:53 wiretap/wiretap.py
+-rw-rw-rw-  2.0 fat      244 b- defN 23-May-08 09:55 wiretap-3.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-08 09:55 wiretap-3.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-08 09:55 wiretap-3.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      520 b- defN 23-May-08 09:55 wiretap-3.1.2.dist-info/RECORD
+7 files, 12516 bytes uncompressed, 3768 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: wiretap/layers.py
 Comment: 
 
 Filename: wiretap/wiretap.py
 Comment: 
 
-Filename: wiretap-3.1.1.dist-info/METADATA
+Filename: wiretap-3.1.2.dist-info/METADATA
 Comment: 
 
-Filename: wiretap-3.1.1.dist-info/WHEEL
+Filename: wiretap-3.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: wiretap-3.1.1.dist-info/top_level.txt
+Filename: wiretap-3.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: wiretap-3.1.1.dist-info/RECORD
+Filename: wiretap-3.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wiretap/wiretap.py

```diff
@@ -182,15 +182,15 @@
         status = inspect.stack()[1][3]
         with _use_custom_log_record_factory(
                 _set_exc_text,
                 functools.partial(_set_module_name, name=self.module),
                 functools.partial(_set_func_name, name=self.scope),
                 functools.partial(_set_attachment, value=kwargs.pop("attachment", None)),
         ):
-            exc_info = all(sys.exc_info())
+            exc_info = all(sys.exc_info()) and status in [self.faulted.__name__]  # Dump the exception or in case of a fault.
             self._logger.log(level=self._logger.level, msg=None, exc_info=exc_info, extra={
                 "parent": self.parent.id if self.parent else None,
                 "node": self.id,
                 "status": status,
                 "elapsed": self.elapsed,
                 "details": kwargs | {"depth": self.depth}
             })
```

