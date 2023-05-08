# Comparing `tmp/magic_duckdb-0.1.8-py3-none-any.whl.zip` & `tmp/magic_duckdb-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,20 @@
-Zip file size: 13792 bytes, number of entries: 12
+Zip file size: 20839 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat       62 b- defN 23-Apr-01 22:19 magic_duckdb/__init__.py
 -rw-rw-rw-  2.0 fat     8742 b- defN 23-Apr-03 01:57 magic_duckdb/autocompletion.py
--rw-rw-rw-  2.0 fat     2669 b- defN 23-Apr-03 14:17 magic_duckdb/duckdb_mode.py
+-rw-rw-rw-  2.0 fat     2650 b- defN 23-Apr-04 02:22 magic_duckdb/duckdb_mode.py
 -rw-rw-rw-  2.0 fat     3282 b- defN 23-Apr-02 18:23 magic_duckdb/explain_analyze_graphviz.py
 -rw-rw-rw-  2.0 fat      417 b- defN 23-Apr-03 01:33 magic_duckdb/logging_init.py
--rw-rw-rw-  2.0 fat     6856 b- defN 23-Apr-03 14:44 magic_duckdb/magic.py
+-rw-rw-rw-  2.0 fat     6251 b- defN 23-Apr-04 02:23 magic_duckdb/magic.py
 -rw-rw-rw-  2.0 fat      991 b- defN 23-Apr-02 18:23 magic_duckdb/sqlformatter.py
--rw-rw-rw-  2.0 fat     1503 b- defN 23-Apr-03 14:44 magic_duckdb-0.1.8.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat     7218 b- defN 23-Apr-03 14:44 magic_duckdb-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-03 14:44 magic_duckdb-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-03 14:44 magic_duckdb-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1007 b- defN 23-Apr-03 14:44 magic_duckdb-0.1.8.dist-info/RECORD
-12 files, 32852 bytes uncompressed, 12088 bytes compressed:  63.2%
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 11:52 magic_duckdb/extras/__init__.py
+-rw-rw-rw-  2.0 fat     8582 b- defN 23-Apr-03 14:06 magic_duckdb/extras/autocompletion.py
+-rw-rw-rw-  2.0 fat     3282 b- defN 23-Apr-02 18:23 magic_duckdb/extras/explain_analyze_graphviz.py
+-rw-rw-rw-  2.0 fat      417 b- defN 23-Apr-03 01:33 magic_duckdb/extras/logging_init.py
+-rw-rw-rw-  2.0 fat     3590 b- defN 23-Apr-04 02:03 magic_duckdb/extras/sql_ai.py
+-rw-rw-rw-  2.0 fat      991 b- defN 23-Apr-02 18:23 magic_duckdb/extras/sqlformatter.py
+-rw-rw-rw-  2.0 fat     1503 b- defN 23-Apr-04 11:53 magic_duckdb-0.1.9.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     7247 b- defN 23-Apr-04 11:53 magic_duckdb-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-04 11:53 magic_duckdb-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Apr-04 11:53 magic_duckdb-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1558 b- defN 23-Apr-04 11:53 magic_duckdb-0.1.9.dist-info/RECORD
+18 files, 49670 bytes uncompressed, 18251 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -15,23 +15,41 @@
 
 Filename: magic_duckdb/magic.py
 Comment: 
 
 Filename: magic_duckdb/sqlformatter.py
 Comment: 
 
-Filename: magic_duckdb-0.1.8.dist-info/LICENSE.md
+Filename: magic_duckdb/extras/__init__.py
 Comment: 
 
-Filename: magic_duckdb-0.1.8.dist-info/METADATA
+Filename: magic_duckdb/extras/autocompletion.py
 Comment: 
 
-Filename: magic_duckdb-0.1.8.dist-info/WHEEL
+Filename: magic_duckdb/extras/explain_analyze_graphviz.py
 Comment: 
 
-Filename: magic_duckdb-0.1.8.dist-info/top_level.txt
+Filename: magic_duckdb/extras/logging_init.py
 Comment: 
 
-Filename: magic_duckdb-0.1.8.dist-info/RECORD
+Filename: magic_duckdb/extras/sql_ai.py
+Comment: 
+
+Filename: magic_duckdb/extras/sqlformatter.py
+Comment: 
+
+Filename: magic_duckdb-0.1.9.dist-info/LICENSE.md
+Comment: 
+
+Filename: magic_duckdb-0.1.9.dist-info/METADATA
+Comment: 
+
+Filename: magic_duckdb-0.1.9.dist-info/WHEEL
+Comment: 
+
+Filename: magic_duckdb-0.1.9.dist-info/top_level.txt
+Comment: 
+
+Filename: magic_duckdb-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## magic_duckdb/duckdb_mode.py

```diff
@@ -18,15 +18,14 @@
         "explain",
         "show",
         "relation",
         "explain_analyze_tree",
         "explain_analyze_json",
         "explain_analyze_draw",
         "analyze [alias for explain_analyze_draw]",
-        "format",
     ]
 
     def default_connection(self) -> duckdb.DuckDBPyConnection:
         return duckdb.default_connection
 
     def connect(self, conn_string: str) -> duckdb.DuckDBPyConnection:
         return duckdb.connect(conn_string)
```

## magic_duckdb/magic.py

```diff
@@ -1,23 +1,26 @@
-import re
+import logging
+import argparse
+from typing import Optional
+
 from traitlets.config.configurable import Configurable
-from IPython.core.magic_arguments import magic_arguments
+from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 from IPython.core.magic import (
     Magics,
     cell_magic,
     line_magic,
     magics_class,
     no_var_expand,
     needs_local_scope,
 )
 from IPython.core.getipython import get_ipython
 from duckdb import ConnectionException, DuckDBPyConnection
+
 from magic_duckdb.duckdb_mode import DuckDbMode
-from typing import Optional
-import logging
+
 
 logger = logging.getLogger("magic_duckdb")
 
 # dbwrapper: To override database logic, replace or monkeypatch this object
 dbwrapper: DuckDbMode = DuckDbMode()
 
 ENABLE_AUTOCOMPLETE = False
@@ -41,104 +44,117 @@
     def __init__(self, shell):
         Configurable.__init__(self, config=shell.config)
         Magics.__init__(self, shell=shell)
 
         # Add ourself to the list of module configurable via %config
         self.shell.configurables.append(self)  # type: ignore
 
-    pattern = re.compile(r"(?si)\s*(\-\S+)(\s+(\S+))?(\s+(.*))?\s*")
+    def connect_by_objectname(self, connection_object):
+        con: DuckDBPyConnection = _get_obj_from_name(connection_object)  # type: ignore
+        if not isinstance(con, DuckDBPyConnection):
+            raise ValueError(f"{connection_object} is not a DuckDBPyConnection")
+        if con is None:
+            raise ValueError(f"Couldn't find {connection_object}")
+        else:
+            logger.info(f"Using existing connection: {connection_object}")
+
+        global connection
+        connection = con
+
+    def format_wrapper(self, query):
+        try:
+            from magic_duckdb.extras.sqlformatter import formatsql
+
+            return formatsql(query)
+        except Exception as e:
+            logger.exception("Error processing")
+            raise e
+
+    def ai_wrapper(self, chat: bool, prompt, query):
+        try:
+            from magic_duckdb.extras import sql_ai
+
+            sql_ai.call_ai(connection, chat, prompt, query)
+            return None  # suppress for now, need to figure out formatting
+        except Exception as e:
+            logger.exception("Error with AI")
+            raise e
 
     @no_var_expand
     @needs_local_scope
     @line_magic("dql")
     @cell_magic("dql")
     @magic_arguments()
-    def execute(
-        self, line: Optional[str] = None, cell: Optional[str] = None, local_ns=None
-    ):
+    @argument("-l", "--listtype", help="List the available types", action="store_true")
+    @argument("-g", "--getcon", help="Return current connection", action="store_true")
+    @argument(
+        "-d", "--default_connection", help="Use default connection", action="store_true"
+    )
+    @argument("-f", "--format", help="Format (beautify) SQL input", action="store_true")
+    @argument("-ai", help="Format (beautify) SQL input", action="store_true")
+    @argument("-aichat", help="Format (beautify) SQL input", action="store_true")
+    @argument(
+        "-cn",
+        "--connection_string",
+        help="Connect to a database using the connection string, such as :memory: or file.db",
+        nargs=1,
+        type=str,
+        action="store",
+    )
+    @argument(
+        "-co",
+        "--connection_object",
+        help="Connect to a database using the connection object",
+        nargs=1,
+        type=str,
+        action="store",
+    )
+    @argument(
+        "-t",
+        "--type",
+        help="Set the default output type",
+        nargs=1,
+        type=str,
+        action="store",
+    )
+    @argument("rest", nargs=argparse.REMAINDER)
+    def execute(self, line: str = "", cell: str = "", local_ns=None):
         global connection
 
-        # Handle arguments via a regexp. Run any statement after the argument and/or option.
-        # TODO: Replace with argparser or cmdparser or equivalent.
-        if line is not None:
-            m = self.pattern.match(line)
-            if m is not None:  # a command was found
-                cmd = m.group(1)
-                everything_after_cmd = m.group(2)
-                cmd_option = m.group(3)
-                everything_after_cmd_option = (
-                    m.group(5) if len(m.groups()) >= 5 else None
+        args = parse_argstring(self.execute, line)
+        # Grab rest of line
+        rest = " ".join(args.rest)
+        query = f"{rest}\n{cell}".strip()
+
+        logger.debug(f"Query = {query}, {len(query)}")
+        if args.listtype:
+            return dbwrapper.export_functions
+        elif args.getcon:
+            return connection
+        elif args.format:
+            return self.format_wrapper(query)
+        elif args.ai:
+            return self.ai_wrapper(False, rest, query)
+        elif args.aichat:
+            return self.ai_wrapper(False, rest, query)
+
+        if args.default_connection:
+            connection = dbwrapper.default_connection()
+        if args.connection_object:
+            self.connect_by_objectname(args.connection_object[0])
+        if args.connection_string:
+            connection = dbwrapper.connect(args.connection_string[0])
+        if args.type:
+            export_function = args.type[0]
+            if export_function in dbwrapper.export_functions:
+                self.export_function = export_function
+            else:
+                raise ValueError(
+                    f"{export_function} not found in {dbwrapper.export_functions}"
                 )
-                if cmd == "--listtypes" or cmd == "-listtypes" or cmd == "-l":
-                    return dbwrapper.export_functions
-                elif cmd == "--getcon" or cmd == "-getcon" or cmd == "-g":
-                    return connection
-                elif cmd == "--format" or cmd == "-f" or cmd == "-format":
-                    try:
-                        from magic_duckdb.extras.sqlformatter import formatsql
-
-                        return formatsql(
-                            everything_after_cmd
-                            if cell is None or len(cell) == 0
-                            else cell
-                        )
-                    except Exception as e:
-                        logger.exception("Error processing")
-                        raise e
-                elif cmd == "-d":
-                    connection = dbwrapper.default_connection()
-                    line = everything_after_cmd
-                elif cmd == "-ai" or cmd == "-aichat":
-                    try:
-                        from magic_duckdb.extras import sql_ai
-
-                        sql_ai.call_ai(
-                            connection,
-                            cmd,
-                            cmd_option
-                            if cell is None or len(cell) == 0
-                            else everything_after_cmd,  # if this is a cell magic, the first line is the entire prompt, otherwise just the first word
-                            cell
-                            if cell is not None and len(cell) > 0
-                            else everything_after_cmd_option,
-                        )
-                        return None  # suppress for now, need to figure out formatting
-                    except Exception as e:
-                        logger.exception("Error with AI")
-                        raise e
-                elif cmd == "-co":
-                    connection_object = cmd_option
-                    con: DuckDBPyConnection = _get_obj_from_name(connection_object)  # type: ignore
-                    if not isinstance(con, DuckDBPyConnection):
-                        raise ValueError(
-                            f"{connection_object} is not a DuckDBPyConnection"
-                        )
-                    if con is None:
-                        raise ValueError(f"Couldn't find {connection_object}")
-                    else:
-                        logger.info(f"Using existing connection: {connection_object}")
-                    connection = con
-                    line = everything_after_cmd_option
-                elif cmd == "-cn":
-                    connection_string = cmd_option
-                    logger.info(f"Connecting to {connection_string}")
-                    con = dbwrapper.connect(connection_string)
-                    line = everything_after_cmd_option
-                elif cmd == "-t":
-                    export_function = cmd_option
-                    if export_function in dbwrapper.export_functions:
-                        self.export_function = export_function
-                    else:
-                        raise ValueError(
-                            f"{export_function} not found in {dbwrapper.export_functions}"
-                        )
-                    line = everything_after_cmd_option
-
-        # Arguments done, now run the query (either the remainder of the line, or the cell if a cell magic)
-        query = cell if (cell is not None and len(cell) > 0) else line
 
         if query is None or len(query) == 0:
             logger.debug("Nothing to execute")
             return
 
         if connection is None:
             logger.info("Setting connection to default_connection()")
```

## Comparing `magic_duckdb-0.1.8.dist-info/LICENSE.md` & `magic_duckdb-0.1.9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `magic_duckdb-0.1.8.dist-info/METADATA` & `magic_duckdb-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-duckdb
-Version: 0.1.8
+Version: 0.1.9
 Summary: Jupyter Cell and Line Magics for DuckDB
 Home-page: https://github.com/iqmo-org/magic_duckdb
 Author: iqmo
 Author-email: info@iqmo.com
 Keywords: Jupyter,Cell Magic,DuckDB,Line Magic,Magic
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -40,15 +40,15 @@
 
 ## Motivation
 
 magic_duckdb was created to:
 
 - Expose duckdb's functionality with minimal overhead and complexity
 - Make it easier to use duckdb in Jupyter notebooks
-- Bundle useful features, like sql formatting (beautifying) and explain analyze graphics
+- Bundle useful features, like using OpenAI to improve SQL, sql formatting (beautifying) and explain analyze graphics
 - Provide a starting point to add other useful features with minimal complexity
 
 ### Why not other projects like Jupysql or ipython-sql?
 
 The %sql magics are great, but are intended for breadth (supporting many types of databases), not depth (deep integration and optimizations for specific databases). As shown below (Performance Comparison), this breadth comes at a performance cost.
 
 ## Simplicity
```

