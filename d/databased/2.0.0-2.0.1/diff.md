# Comparing `tmp/databased-2.0.0.tar.gz` & `tmp/databased-2.0.1.tar.gz`

## Comparing `databased-2.0.0.tar` & `databased-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 databased-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    34874 2020-02-02 00:00:00.000000 databased-2.0.0/docs/databased.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.0.0/docs/index.html
--rw-r--r--   0        0        0    65282 2020-02-02 00:00:00.000000 databased-2.0.0/docs/search.js
--rw-r--r--   0        0        0    44621 2020-02-02 00:00:00.000000 databased-2.0.0/docs/databased/customshell.html
--rw-r--r--   0        0        0   430465 2020-02-02 00:00:00.000000 databased-2.0.0/docs/databased/databased.html
--rw-r--r--   0        0        0   121748 2020-02-02 00:00:00.000000 databased-2.0.0/docs/databased/dbparsers.html
--rw-r--r--   0        0        0   304581 2020-02-02 00:00:00.000000 databased-2.0.0/docs/databased/dbshell.html
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 databased-2.0.0/src/databased/__init__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.0.0/src/databased/customshell.py
--rw-r--r--   0        0        0    22129 2020-02-02 00:00:00.000000 databased-2.0.0/src/databased/databased.py
--rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 databased-2.0.0/src/databased/dbparsers.py
--rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 databased-2.0.0/src/databased/dbshell.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.0.0/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 databased-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 databased-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5776 2020-02-02 00:00:00.000000 databased-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34874 2020-02-02 00:00:00.000000 databased-2.0.1/docs/databased.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.0.1/docs/index.html
+-rw-r--r--   0        0        0    65282 2020-02-02 00:00:00.000000 databased-2.0.1/docs/search.js
+-rw-r--r--   0        0        0    44621 2020-02-02 00:00:00.000000 databased-2.0.1/docs/databased/customshell.html
+-rw-r--r--   0        0        0   431224 2020-02-02 00:00:00.000000 databased-2.0.1/docs/databased/databased.html
+-rw-r--r--   0        0        0   121748 2020-02-02 00:00:00.000000 databased-2.0.1/docs/databased/dbparsers.html
+-rw-r--r--   0        0        0   304581 2020-02-02 00:00:00.000000 databased-2.0.1/docs/databased/dbshell.html
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 databased-2.0.1/src/databased/__init__.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.0.1/src/databased/customshell.py
+-rw-r--r--   0        0        0    22194 2020-02-02 00:00:00.000000 databased-2.0.1/src/databased/databased.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 databased-2.0.1/src/databased/dbparsers.py
+-rw-r--r--   0        0        0    13626 2020-02-02 00:00:00.000000 databased-2.0.1/src/databased/dbshell.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.0.1/README.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 databased-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 databased-2.0.1/PKG-INFO
```

### Comparing `databased-2.0.0/CHANGELOG.md` & `databased-2.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # Changelog
 
-## 1.7.0 (2023-05-04)
+## 2.0.0 (2023-05-04)
+
+#### Refactorings
+
+* change dbmanager names to dbshell (Breaking)
+
+
+## v1.7.0 (2023-05-04)
 
 #### New Features
 
 * add add_rows()
-* update() supports exact_match param
+* update supports exact_match param
 * do_update prints number of updated rows
 * do_query prints number of affected rows
 #### Performance improvements
 
 * make counting rows optional for do_info()
 * do_add_row() prints addition success status
 * add_row() returns whether the addition was successful
 * delete() returns number of deleted rows via cursor.rowcount
 #### Refactorings
 
 * update() returns number of affected rows
+#### Others
+
+* build v1.7.0
+* update changelog
 
 
 ## v1.6.0 (2023-05-03)
 
 #### New Features
 
 * add do_scan_dbs()
```

### Comparing `databased-2.0.0/docs/databased.html` & `databased-2.0.1/docs/databased.html`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/docs/search.js` & `databased-2.0.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/docs/databased/customshell.html` & `databased-2.0.1/docs/databased/customshell.html`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/docs/databased/databased.html` & `databased-2.0.1/docs/databased/databased.html`

 * *Files 1% similar despite different names*

```diff
@@ -279,44 +279,44 @@
 </span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
 </span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>
 </span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
 </span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
 </span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
 </span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
 </span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
 </span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
 </span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>    <span class="nd">@_connect</span>
 </span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
 </span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
 </span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
 </span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">        #### :params:</span>
 </span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
 </span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a><span class="sd">        `table`: Name of the table to create.</span>
 </span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
 </span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
 </span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
 </span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
 </span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
 </span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
 </span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
 </span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="nd">@_connect</span>
 </span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
 </span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
 </span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
 </span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="p">)</span>
 </span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
 </span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
 </span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>    <span class="nd">@_connect</span>
 </span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
 </span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
 </span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
 </span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="nd">@_connect</span>
 </span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
 </span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="bp">self</span><span class="p">,</span>
 </span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
 </span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
@@ -331,15 +331,15 @@
 </span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
 </span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
 </span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
 </span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
 </span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
 </span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
 </span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
 </span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
 </span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>                <span class="p">)</span>
 </span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>            <span class="k">else</span><span class="p">:</span>
 </span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
@@ -365,20 +365,20 @@
 </span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
 </span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
 </span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
 </span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
 </span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
 </span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
 </span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                    <span class="n">values</span><span class="p">,</span>
 </span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                <span class="p">)</span>
 </span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>            <span class="k">else</span><span class="p">:</span>
 </span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
 </span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>                <span class="p">)</span>
 </span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
 </span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>            <span class="k">return</span> <span class="kc">True</span>
 </span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
 </span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
 </span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
@@ -454,15 +454,15 @@
 </span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
 </span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a>
 </span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
 </span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a>
 </span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
 </span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
 </span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
 </span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
 </span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
@@ -524,15 +524,15 @@
 </span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
 </span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
 </span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a>
 </span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
 </span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
 </span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
 </span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
 </span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
 </span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
 </span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a>            <span class="p">)</span>
 </span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
 </span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
@@ -562,15 +562,15 @@
 </span><span id="L-446"><a href="#L-446"><span class="linenos">446</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
 </span><span id="L-447"><a href="#L-447"><span class="linenos">447</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
 </span><span id="L-448"><a href="#L-448"><span class="linenos">448</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
 </span><span id="L-449"><a href="#L-449"><span class="linenos">449</span></a>
 </span><span id="L-450"><a href="#L-450"><span class="linenos">450</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
 </span><span id="L-451"><a href="#L-451"><span class="linenos">451</span></a>
 </span><span id="L-452"><a href="#L-452"><span class="linenos">452</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
-</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="L-453"><a href="#L-453"><span class="linenos">453</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
 </span><span id="L-454"><a href="#L-454"><span class="linenos">454</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
 </span><span id="L-455"><a href="#L-455"><span class="linenos">455</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="L-456"><a href="#L-456"><span class="linenos">456</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
 </span><span id="L-457"><a href="#L-457"><span class="linenos">457</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="L-458"><a href="#L-458"><span class="linenos">458</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="L-459"><a href="#L-459"><span class="linenos">459</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
 </span><span id="L-460"><a href="#L-460"><span class="linenos">460</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
@@ -592,15 +592,15 @@
 </span><span id="L-476"><a href="#L-476"><span class="linenos">476</span></a>
 </span><span id="L-477"><a href="#L-477"><span class="linenos">477</span></a>    <span class="nd">@_connect</span>
 </span><span id="L-478"><a href="#L-478"><span class="linenos">478</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
 </span><span id="L-479"><a href="#L-479"><span class="linenos">479</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
 </span><span id="L-480"><a href="#L-480"><span class="linenos">480</span></a>
 </span><span id="L-481"><a href="#L-481"><span class="linenos">481</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
 </span><span id="L-482"><a href="#L-482"><span class="linenos">482</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="L-483"><a href="#L-483"><span class="linenos">483</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
 </span><span id="L-484"><a href="#L-484"><span class="linenos">484</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="L-485"><a href="#L-485"><span class="linenos">485</span></a>            <span class="k">return</span> <span class="kc">True</span>
 </span><span id="L-486"><a href="#L-486"><span class="linenos">486</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="L-487"><a href="#L-487"><span class="linenos">487</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
 </span><span id="L-488"><a href="#L-488"><span class="linenos">488</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="L-489"><a href="#L-489"><span class="linenos">489</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span><span id="L-490"><a href="#L-490"><span class="linenos">490</span></a>
@@ -616,107 +616,109 @@
 </span><span id="L-500"><a href="#L-500"><span class="linenos">500</span></a>
 </span><span id="L-501"><a href="#L-501"><span class="linenos">501</span></a><span class="sd">        `_type`: The data type of the new column.</span>
 </span><span id="L-502"><a href="#L-502"><span class="linenos">502</span></a>
 </span><span id="L-503"><a href="#L-503"><span class="linenos">503</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
 </span><span id="L-504"><a href="#L-504"><span class="linenos">504</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="L-505"><a href="#L-505"><span class="linenos">505</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
 </span><span id="L-506"><a href="#L-506"><span class="linenos">506</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-507"><a href="#L-507"><span class="linenos">507</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
 </span><span id="L-508"><a href="#L-508"><span class="linenos">508</span></a>                <span class="p">)</span>
 </span><span id="L-509"><a href="#L-509"><span class="linenos">509</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
 </span><span id="L-510"><a href="#L-510"><span class="linenos">510</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
-</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a>
-</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>
-</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-511"><a href="#L-511"><span class="linenos">511</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="L-512"><a href="#L-512"><span class="linenos">512</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="L-513"><a href="#L-513"><span class="linenos">513</span></a>                <span class="p">)</span>
+</span><span id="L-514"><a href="#L-514"><span class="linenos">514</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-515"><a href="#L-515"><span class="linenos">515</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-516"><a href="#L-516"><span class="linenos">516</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="L-517"><a href="#L-517"><span class="linenos">517</span></a>
+</span><span id="L-518"><a href="#L-518"><span class="linenos">518</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="L-519"><a href="#L-519"><span class="linenos">519</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="L-520"><a href="#L-520"><span class="linenos">520</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-521"><a href="#L-521"><span class="linenos">521</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-522"><a href="#L-522"><span class="linenos">522</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
 </span><span id="L-523"><a href="#L-523"><span class="linenos">523</span></a>
-</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a>
-</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="L-524"><a href="#L-524"><span class="linenos">524</span></a><span class="sd">        #### :params:</span>
+</span><span id="L-525"><a href="#L-525"><span class="linenos">525</span></a>
+</span><span id="L-526"><a href="#L-526"><span class="linenos">526</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="L-527"><a href="#L-527"><span class="linenos">527</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
 </span><span id="L-528"><a href="#L-528"><span class="linenos">528</span></a>
-</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
-</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a>
-</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>
-</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a>
-</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-529"><a href="#L-529"><span class="linenos">529</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="L-530"><a href="#L-530"><span class="linenos">530</span></a>
+</span><span id="L-531"><a href="#L-531"><span class="linenos">531</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="L-532"><a href="#L-532"><span class="linenos">532</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="L-533"><a href="#L-533"><span class="linenos">533</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="L-534"><a href="#L-534"><span class="linenos">534</span></a>
+</span><span id="L-535"><a href="#L-535"><span class="linenos">535</span></a>
+</span><span id="L-536"><a href="#L-536"><span class="linenos">536</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="L-537"><a href="#L-537"><span class="linenos">537</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-538"><a href="#L-538"><span class="linenos">538</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="L-539"><a href="#L-539"><span class="linenos">539</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
 </span><span id="L-540"><a href="#L-540"><span class="linenos">540</span></a>
-</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a>
-</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="L-541"><a href="#L-541"><span class="linenos">541</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-542"><a href="#L-542"><span class="linenos">542</span></a>
+</span><span id="L-543"><a href="#L-543"><span class="linenos">543</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="L-544"><a href="#L-544"><span class="linenos">544</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
 </span><span id="L-545"><a href="#L-545"><span class="linenos">545</span></a>
-</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
-</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
-</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
-</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
-</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
-</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
-</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a>
-</span><span id="L-556"><a href="#L-556"><span class="linenos">556</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-557"><a href="#L-557"><span class="linenos">557</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="L-558"><a href="#L-558"><span class="linenos">558</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
-</span><span id="L-559"><a href="#L-559"><span class="linenos">559</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
-</span><span id="L-560"><a href="#L-560"><span class="linenos">560</span></a>    <span class="c1"># to see if shrinking is necessary</span>
-</span><span id="L-561"><a href="#L-561"><span class="linenos">561</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="L-562"><a href="#L-562"><span class="linenos">562</span></a>        <span class="n">data</span><span class="p">,</span>
-</span><span id="L-563"><a href="#L-563"><span class="linenos">563</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="L-564"><a href="#L-564"><span class="linenos">564</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="L-565"><a href="#L-565"><span class="linenos">565</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="L-566"><a href="#L-566"><span class="linenos">566</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="L-567"><a href="#L-567"><span class="linenos">567</span></a>    <span class="p">)</span>
-</span><span id="L-568"><a href="#L-568"><span class="linenos">568</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-569"><a href="#L-569"><span class="linenos">569</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-570"><a href="#L-570"><span class="linenos">570</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-571"><a href="#L-571"><span class="linenos">571</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="L-572"><a href="#L-572"><span class="linenos">572</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-573"><a href="#L-573"><span class="linenos">573</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="L-574"><a href="#L-574"><span class="linenos">574</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
-</span><span id="L-575"><a href="#L-575"><span class="linenos">575</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-576"><a href="#L-576"><span class="linenos">576</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;=</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-577"><a href="#L-577"><span class="linenos">577</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="L-578"><a href="#L-578"><span class="linenos">578</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
-</span><span id="L-579"><a href="#L-579"><span class="linenos">579</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-580"><a href="#L-580"><span class="linenos">580</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
-</span><span id="L-581"><a href="#L-581"><span class="linenos">581</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-582"><a href="#L-582"><span class="linenos">582</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
-</span><span id="L-583"><a href="#L-583"><span class="linenos">583</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
-</span><span id="L-584"><a href="#L-584"><span class="linenos">584</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
-</span><span id="L-585"><a href="#L-585"><span class="linenos">585</span></a>                <span class="p">)</span>
-</span><span id="L-586"><a href="#L-586"><span class="linenos">586</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="L-587"><a href="#L-587"><span class="linenos">587</span></a>                <span class="n">data</span><span class="p">,</span>
-</span><span id="L-588"><a href="#L-588"><span class="linenos">588</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="L-589"><a href="#L-589"><span class="linenos">589</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="L-590"><a href="#L-590"><span class="linenos">590</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="L-591"><a href="#L-591"><span class="linenos">591</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="L-592"><a href="#L-592"><span class="linenos">592</span></a>            <span class="p">)</span>
-</span><span id="L-593"><a href="#L-593"><span class="linenos">593</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-594"><a href="#L-594"><span class="linenos">594</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="L-595"><a href="#L-595"><span class="linenos">595</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="L-596"><a href="#L-596"><span class="linenos">596</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="L-597"><a href="#L-597"><span class="linenos">597</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
-</span><span id="L-598"><a href="#L-598"><span class="linenos">598</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="L-599"><a href="#L-599"><span class="linenos">599</span></a>    <span class="k">return</span> <span class="n">output</span>
+</span><span id="L-546"><a href="#L-546"><span class="linenos">546</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="L-547"><a href="#L-547"><span class="linenos">547</span></a>
+</span><span id="L-548"><a href="#L-548"><span class="linenos">548</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="L-549"><a href="#L-549"><span class="linenos">549</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="L-550"><a href="#L-550"><span class="linenos">550</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-551"><a href="#L-551"><span class="linenos">551</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
+</span><span id="L-552"><a href="#L-552"><span class="linenos">552</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
+</span><span id="L-553"><a href="#L-553"><span class="linenos">553</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
+</span><span id="L-554"><a href="#L-554"><span class="linenos">554</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
+</span><span id="L-555"><a href="#L-555"><span class="linenos">555</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
+</span><span id="L-556"><a href="#L-556"><span class="linenos">556</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
+</span><span id="L-557"><a href="#L-557"><span class="linenos">557</span></a>
+</span><span id="L-558"><a href="#L-558"><span class="linenos">558</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-559"><a href="#L-559"><span class="linenos">559</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="L-560"><a href="#L-560"><span class="linenos">560</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
+</span><span id="L-561"><a href="#L-561"><span class="linenos">561</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
+</span><span id="L-562"><a href="#L-562"><span class="linenos">562</span></a>    <span class="c1"># to see if shrinking is necessary</span>
+</span><span id="L-563"><a href="#L-563"><span class="linenos">563</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="L-564"><a href="#L-564"><span class="linenos">564</span></a>        <span class="n">data</span><span class="p">,</span>
+</span><span id="L-565"><a href="#L-565"><span class="linenos">565</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="L-566"><a href="#L-566"><span class="linenos">566</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="L-567"><a href="#L-567"><span class="linenos">567</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="L-568"><a href="#L-568"><span class="linenos">568</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="L-569"><a href="#L-569"><span class="linenos">569</span></a>    <span class="p">)</span>
+</span><span id="L-570"><a href="#L-570"><span class="linenos">570</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-571"><a href="#L-571"><span class="linenos">571</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-572"><a href="#L-572"><span class="linenos">572</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-573"><a href="#L-573"><span class="linenos">573</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="L-574"><a href="#L-574"><span class="linenos">574</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-575"><a href="#L-575"><span class="linenos">575</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="L-576"><a href="#L-576"><span class="linenos">576</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
+</span><span id="L-577"><a href="#L-577"><span class="linenos">577</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-578"><a href="#L-578"><span class="linenos">578</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;=</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-579"><a href="#L-579"><span class="linenos">579</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="L-580"><a href="#L-580"><span class="linenos">580</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
+</span><span id="L-581"><a href="#L-581"><span class="linenos">581</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-582"><a href="#L-582"><span class="linenos">582</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
+</span><span id="L-583"><a href="#L-583"><span class="linenos">583</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-584"><a href="#L-584"><span class="linenos">584</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
+</span><span id="L-585"><a href="#L-585"><span class="linenos">585</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
+</span><span id="L-586"><a href="#L-586"><span class="linenos">586</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
+</span><span id="L-587"><a href="#L-587"><span class="linenos">587</span></a>                <span class="p">)</span>
+</span><span id="L-588"><a href="#L-588"><span class="linenos">588</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="L-589"><a href="#L-589"><span class="linenos">589</span></a>                <span class="n">data</span><span class="p">,</span>
+</span><span id="L-590"><a href="#L-590"><span class="linenos">590</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="L-591"><a href="#L-591"><span class="linenos">591</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="L-592"><a href="#L-592"><span class="linenos">592</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="L-593"><a href="#L-593"><span class="linenos">593</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="L-594"><a href="#L-594"><span class="linenos">594</span></a>            <span class="p">)</span>
+</span><span id="L-595"><a href="#L-595"><span class="linenos">595</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-596"><a href="#L-596"><span class="linenos">596</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="L-597"><a href="#L-597"><span class="linenos">597</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="L-598"><a href="#L-598"><span class="linenos">598</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="L-599"><a href="#L-599"><span class="linenos">599</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
+</span><span id="L-600"><a href="#L-600"><span class="linenos">600</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="L-601"><a href="#L-601"><span class="linenos">601</span></a>    <span class="k">return</span> <span class="n">output</span>
 </span></pre></div>
 
 
             </section>
                 <section id="DataBased">
                             <input id="DataBased-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -868,44 +870,44 @@
 </span><span id="DataBased-164"><a href="#DataBased-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
 </span><span id="DataBased-165"><a href="#DataBased-165"><span class="linenos">165</span></a>
 </span><span id="DataBased-166"><a href="#DataBased-166"><span class="linenos">166</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
 </span><span id="DataBased-167"><a href="#DataBased-167"><span class="linenos">167</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
 </span><span id="DataBased-168"><a href="#DataBased-168"><span class="linenos">168</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
 </span><span id="DataBased-169"><a href="#DataBased-169"><span class="linenos">169</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
 </span><span id="DataBased-170"><a href="#DataBased-170"><span class="linenos">170</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="DataBased-171"><a href="#DataBased-171"><span class="linenos">171</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-171"><a href="#DataBased-171"><span class="linenos">171</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
 </span><span id="DataBased-172"><a href="#DataBased-172"><span class="linenos">172</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span><span id="DataBased-173"><a href="#DataBased-173"><span class="linenos">173</span></a>
 </span><span id="DataBased-174"><a href="#DataBased-174"><span class="linenos">174</span></a>    <span class="nd">@_connect</span>
 </span><span id="DataBased-175"><a href="#DataBased-175"><span class="linenos">175</span></a>    <span class="k">def</span> <span class="nf">create_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">column_defs</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]):</span>
 </span><span id="DataBased-176"><a href="#DataBased-176"><span class="linenos">176</span></a>        <span class="sd">&quot;&quot;&quot;Create a table if it doesn&#39;t exist.</span>
 </span><span id="DataBased-177"><a href="#DataBased-177"><span class="linenos">177</span></a>
 </span><span id="DataBased-178"><a href="#DataBased-178"><span class="linenos">178</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased-179"><a href="#DataBased-179"><span class="linenos">179</span></a>
 </span><span id="DataBased-180"><a href="#DataBased-180"><span class="linenos">180</span></a><span class="sd">        `table`: Name of the table to create.</span>
 </span><span id="DataBased-181"><a href="#DataBased-181"><span class="linenos">181</span></a>
 </span><span id="DataBased-182"><a href="#DataBased-182"><span class="linenos">182</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
 </span><span id="DataBased-183"><a href="#DataBased-183"><span class="linenos">183</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
 </span><span id="DataBased-184"><a href="#DataBased-184"><span class="linenos">184</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="DataBased-185"><a href="#DataBased-185"><span class="linenos">185</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="DataBased-185"><a href="#DataBased-185"><span class="linenos">185</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
 </span><span id="DataBased-186"><a href="#DataBased-186"><span class="linenos">186</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
 </span><span id="DataBased-187"><a href="#DataBased-187"><span class="linenos">187</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
 </span><span id="DataBased-188"><a href="#DataBased-188"><span class="linenos">188</span></a>
 </span><span id="DataBased-189"><a href="#DataBased-189"><span class="linenos">189</span></a>    <span class="nd">@_connect</span>
 </span><span id="DataBased-190"><a href="#DataBased-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">get_table_names</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Returns a list of table names from the database.&quot;&quot;&quot;</span>
 </span><span id="DataBased-192"><a href="#DataBased-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
 </span><span id="DataBased-193"><a href="#DataBased-193"><span class="linenos">193</span></a>            <span class="s1">&#39;select name from sqlite_Schema where type = &quot;table&quot; and name not like &quot;sqlite_%&quot;;&#39;</span>
 </span><span id="DataBased-194"><a href="#DataBased-194"><span class="linenos">194</span></a>        <span class="p">)</span>
 </span><span id="DataBased-195"><a href="#DataBased-195"><span class="linenos">195</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">result</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">result</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()]</span>
 </span><span id="DataBased-196"><a href="#DataBased-196"><span class="linenos">196</span></a>
 </span><span id="DataBased-197"><a href="#DataBased-197"><span class="linenos">197</span></a>    <span class="nd">@_connect</span>
 </span><span id="DataBased-198"><a href="#DataBased-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="DataBased-199"><a href="#DataBased-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="DataBased-200"><a href="#DataBased-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="DataBased-200"><a href="#DataBased-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
 </span><span id="DataBased-201"><a href="#DataBased-201"><span class="linenos">201</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
 </span><span id="DataBased-202"><a href="#DataBased-202"><span class="linenos">202</span></a>
 </span><span id="DataBased-203"><a href="#DataBased-203"><span class="linenos">203</span></a>    <span class="nd">@_connect</span>
 </span><span id="DataBased-204"><a href="#DataBased-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">count</span><span class="p">(</span>
 </span><span id="DataBased-205"><a href="#DataBased-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="p">,</span>
 </span><span id="DataBased-206"><a href="#DataBased-206"><span class="linenos">206</span></a>        <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span>
 </span><span id="DataBased-207"><a href="#DataBased-207"><span class="linenos">207</span></a>        <span class="n">match_criteria</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">tuple</span><span class="p">]</span> <span class="o">|</span> <span class="nb">dict</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span>
@@ -920,15 +922,15 @@
 </span><span id="DataBased-216"><a href="#DataBased-216"><span class="linenos">216</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="DataBased-217"><a href="#DataBased-217"><span class="linenos">217</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
 </span><span id="DataBased-218"><a href="#DataBased-218"><span class="linenos">218</span></a>
 </span><span id="DataBased-219"><a href="#DataBased-219"><span class="linenos">219</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
 </span><span id="DataBased-220"><a href="#DataBased-220"><span class="linenos">220</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
 </span><span id="DataBased-221"><a href="#DataBased-221"><span class="linenos">221</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
 </span><span id="DataBased-222"><a href="#DataBased-222"><span class="linenos">222</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased-223"><a href="#DataBased-223"><span class="linenos">223</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-223"><a href="#DataBased-223"><span class="linenos">223</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
 </span><span id="DataBased-224"><a href="#DataBased-224"><span class="linenos">224</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="DataBased-225"><a href="#DataBased-225"><span class="linenos">225</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="DataBased-226"><a href="#DataBased-226"><span class="linenos">226</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
 </span><span id="DataBased-227"><a href="#DataBased-227"><span class="linenos">227</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
 </span><span id="DataBased-228"><a href="#DataBased-228"><span class="linenos">228</span></a>                <span class="p">)</span>
 </span><span id="DataBased-229"><a href="#DataBased-229"><span class="linenos">229</span></a>            <span class="k">else</span><span class="p">:</span>
 </span><span id="DataBased-230"><a href="#DataBased-230"><span class="linenos">230</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
@@ -954,20 +956,20 @@
 </span><span id="DataBased-250"><a href="#DataBased-250"><span class="linenos">250</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
 </span><span id="DataBased-251"><a href="#DataBased-251"><span class="linenos">251</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
 </span><span id="DataBased-252"><a href="#DataBased-252"><span class="linenos">252</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
 </span><span id="DataBased-253"><a href="#DataBased-253"><span class="linenos">253</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="DataBased-254"><a href="#DataBased-254"><span class="linenos">254</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
 </span><span id="DataBased-255"><a href="#DataBased-255"><span class="linenos">255</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
 </span><span id="DataBased-256"><a href="#DataBased-256"><span class="linenos">256</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-257"><a href="#DataBased-257"><span class="linenos">257</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="DataBased-257"><a href="#DataBased-257"><span class="linenos">257</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
 </span><span id="DataBased-258"><a href="#DataBased-258"><span class="linenos">258</span></a>                    <span class="n">values</span><span class="p">,</span>
 </span><span id="DataBased-259"><a href="#DataBased-259"><span class="linenos">259</span></a>                <span class="p">)</span>
 </span><span id="DataBased-260"><a href="#DataBased-260"><span class="linenos">260</span></a>            <span class="k">else</span><span class="p">:</span>
 </span><span id="DataBased-261"><a href="#DataBased-261"><span class="linenos">261</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-262"><a href="#DataBased-262"><span class="linenos">262</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased-262"><a href="#DataBased-262"><span class="linenos">262</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
 </span><span id="DataBased-263"><a href="#DataBased-263"><span class="linenos">263</span></a>                <span class="p">)</span>
 </span><span id="DataBased-264"><a href="#DataBased-264"><span class="linenos">264</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
 </span><span id="DataBased-265"><a href="#DataBased-265"><span class="linenos">265</span></a>            <span class="k">return</span> <span class="kc">True</span>
 </span><span id="DataBased-266"><a href="#DataBased-266"><span class="linenos">266</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="DataBased-267"><a href="#DataBased-267"><span class="linenos">267</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
 </span><span id="DataBased-268"><a href="#DataBased-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
 </span><span id="DataBased-269"><a href="#DataBased-269"><span class="linenos">269</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
@@ -1043,15 +1045,15 @@
 </span><span id="DataBased-339"><a href="#DataBased-339"><span class="linenos">339</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
 </span><span id="DataBased-340"><a href="#DataBased-340"><span class="linenos">340</span></a>
 </span><span id="DataBased-341"><a href="#DataBased-341"><span class="linenos">341</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
 </span><span id="DataBased-342"><a href="#DataBased-342"><span class="linenos">342</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="DataBased-343"><a href="#DataBased-343"><span class="linenos">343</span></a>
 </span><span id="DataBased-344"><a href="#DataBased-344"><span class="linenos">344</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
 </span><span id="DataBased-345"><a href="#DataBased-345"><span class="linenos">345</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="DataBased-346"><a href="#DataBased-346"><span class="linenos">346</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased-346"><a href="#DataBased-346"><span class="linenos">346</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
 </span><span id="DataBased-347"><a href="#DataBased-347"><span class="linenos">347</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="DataBased-348"><a href="#DataBased-348"><span class="linenos">348</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="DataBased-349"><a href="#DataBased-349"><span class="linenos">349</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="DataBased-350"><a href="#DataBased-350"><span class="linenos">350</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
 </span><span id="DataBased-351"><a href="#DataBased-351"><span class="linenos">351</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="DataBased-352"><a href="#DataBased-352"><span class="linenos">352</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
 </span><span id="DataBased-353"><a href="#DataBased-353"><span class="linenos">353</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
@@ -1113,15 +1115,15 @@
 </span><span id="DataBased-409"><a href="#DataBased-409"><span class="linenos">409</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
 </span><span id="DataBased-410"><a href="#DataBased-410"><span class="linenos">410</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
 </span><span id="DataBased-411"><a href="#DataBased-411"><span class="linenos">411</span></a>
 </span><span id="DataBased-412"><a href="#DataBased-412"><span class="linenos">412</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
 </span><span id="DataBased-413"><a href="#DataBased-413"><span class="linenos">413</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="DataBased-414"><a href="#DataBased-414"><span class="linenos">414</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
 </span><span id="DataBased-415"><a href="#DataBased-415"><span class="linenos">415</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-416"><a href="#DataBased-416"><span class="linenos">416</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-416"><a href="#DataBased-416"><span class="linenos">416</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
 </span><span id="DataBased-417"><a href="#DataBased-417"><span class="linenos">417</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
 </span><span id="DataBased-418"><a href="#DataBased-418"><span class="linenos">418</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
 </span><span id="DataBased-419"><a href="#DataBased-419"><span class="linenos">419</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
 </span><span id="DataBased-420"><a href="#DataBased-420"><span class="linenos">420</span></a>            <span class="p">)</span>
 </span><span id="DataBased-421"><a href="#DataBased-421"><span class="linenos">421</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
 </span><span id="DataBased-422"><a href="#DataBased-422"><span class="linenos">422</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="DataBased-423"><a href="#DataBased-423"><span class="linenos">423</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
@@ -1151,15 +1153,15 @@
 </span><span id="DataBased-447"><a href="#DataBased-447"><span class="linenos">447</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
 </span><span id="DataBased-448"><a href="#DataBased-448"><span class="linenos">448</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
 </span><span id="DataBased-449"><a href="#DataBased-449"><span class="linenos">449</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
 </span><span id="DataBased-450"><a href="#DataBased-450"><span class="linenos">450</span></a>
 </span><span id="DataBased-451"><a href="#DataBased-451"><span class="linenos">451</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
 </span><span id="DataBased-452"><a href="#DataBased-452"><span class="linenos">452</span></a>
 </span><span id="DataBased-453"><a href="#DataBased-453"><span class="linenos">453</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
-</span><span id="DataBased-454"><a href="#DataBased-454"><span class="linenos">454</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="DataBased-454"><a href="#DataBased-454"><span class="linenos">454</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
 </span><span id="DataBased-455"><a href="#DataBased-455"><span class="linenos">455</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
 </span><span id="DataBased-456"><a href="#DataBased-456"><span class="linenos">456</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="DataBased-457"><a href="#DataBased-457"><span class="linenos">457</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
 </span><span id="DataBased-458"><a href="#DataBased-458"><span class="linenos">458</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="DataBased-459"><a href="#DataBased-459"><span class="linenos">459</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="DataBased-460"><a href="#DataBased-460"><span class="linenos">460</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
 </span><span id="DataBased-461"><a href="#DataBased-461"><span class="linenos">461</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
@@ -1181,15 +1183,15 @@
 </span><span id="DataBased-477"><a href="#DataBased-477"><span class="linenos">477</span></a>
 </span><span id="DataBased-478"><a href="#DataBased-478"><span class="linenos">478</span></a>    <span class="nd">@_connect</span>
 </span><span id="DataBased-479"><a href="#DataBased-479"><span class="linenos">479</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
 </span><span id="DataBased-480"><a href="#DataBased-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
 </span><span id="DataBased-481"><a href="#DataBased-481"><span class="linenos">481</span></a>
 </span><span id="DataBased-482"><a href="#DataBased-482"><span class="linenos">482</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
 </span><span id="DataBased-483"><a href="#DataBased-483"><span class="linenos">483</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased-484"><a href="#DataBased-484"><span class="linenos">484</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased-484"><a href="#DataBased-484"><span class="linenos">484</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
 </span><span id="DataBased-485"><a href="#DataBased-485"><span class="linenos">485</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="DataBased-486"><a href="#DataBased-486"><span class="linenos">486</span></a>            <span class="k">return</span> <span class="kc">True</span>
 </span><span id="DataBased-487"><a href="#DataBased-487"><span class="linenos">487</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="DataBased-488"><a href="#DataBased-488"><span class="linenos">488</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
 </span><span id="DataBased-489"><a href="#DataBased-489"><span class="linenos">489</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="DataBased-490"><a href="#DataBased-490"><span class="linenos">490</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span><span id="DataBased-491"><a href="#DataBased-491"><span class="linenos">491</span></a>
@@ -1205,39 +1207,41 @@
 </span><span id="DataBased-501"><a href="#DataBased-501"><span class="linenos">501</span></a>
 </span><span id="DataBased-502"><a href="#DataBased-502"><span class="linenos">502</span></a><span class="sd">        `_type`: The data type of the new column.</span>
 </span><span id="DataBased-503"><a href="#DataBased-503"><span class="linenos">503</span></a>
 </span><span id="DataBased-504"><a href="#DataBased-504"><span class="linenos">504</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
 </span><span id="DataBased-505"><a href="#DataBased-505"><span class="linenos">505</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="DataBased-506"><a href="#DataBased-506"><span class="linenos">506</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
 </span><span id="DataBased-507"><a href="#DataBased-507"><span class="linenos">507</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased-508"><a href="#DataBased-508"><span class="linenos">508</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased-508"><a href="#DataBased-508"><span class="linenos">508</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
 </span><span id="DataBased-509"><a href="#DataBased-509"><span class="linenos">509</span></a>                <span class="p">)</span>
 </span><span id="DataBased-510"><a href="#DataBased-510"><span class="linenos">510</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
 </span><span id="DataBased-511"><a href="#DataBased-511"><span class="linenos">511</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased-512"><a href="#DataBased-512"><span class="linenos">512</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
-</span><span id="DataBased-513"><a href="#DataBased-513"><span class="linenos">513</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-514"><a href="#DataBased-514"><span class="linenos">514</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased-515"><a href="#DataBased-515"><span class="linenos">515</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased-516"><a href="#DataBased-516"><span class="linenos">516</span></a>
-</span><span id="DataBased-517"><a href="#DataBased-517"><span class="linenos">517</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="DataBased-518"><a href="#DataBased-518"><span class="linenos">518</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="DataBased-519"><a href="#DataBased-519"><span class="linenos">519</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased-520"><a href="#DataBased-520"><span class="linenos">520</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased-521"><a href="#DataBased-521"><span class="linenos">521</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="DataBased-522"><a href="#DataBased-522"><span class="linenos">522</span></a>
-</span><span id="DataBased-523"><a href="#DataBased-523"><span class="linenos">523</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-512"><a href="#DataBased-512"><span class="linenos">512</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased-513"><a href="#DataBased-513"><span class="linenos">513</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased-514"><a href="#DataBased-514"><span class="linenos">514</span></a>                <span class="p">)</span>
+</span><span id="DataBased-515"><a href="#DataBased-515"><span class="linenos">515</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-516"><a href="#DataBased-516"><span class="linenos">516</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased-517"><a href="#DataBased-517"><span class="linenos">517</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased-518"><a href="#DataBased-518"><span class="linenos">518</span></a>
+</span><span id="DataBased-519"><a href="#DataBased-519"><span class="linenos">519</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="DataBased-520"><a href="#DataBased-520"><span class="linenos">520</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="DataBased-521"><a href="#DataBased-521"><span class="linenos">521</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased-522"><a href="#DataBased-522"><span class="linenos">522</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased-523"><a href="#DataBased-523"><span class="linenos">523</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
 </span><span id="DataBased-524"><a href="#DataBased-524"><span class="linenos">524</span></a>
-</span><span id="DataBased-525"><a href="#DataBased-525"><span class="linenos">525</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="DataBased-526"><a href="#DataBased-526"><span class="linenos">526</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="DataBased-527"><a href="#DataBased-527"><span class="linenos">527</span></a>
-</span><span id="DataBased-528"><a href="#DataBased-528"><span class="linenos">528</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased-525"><a href="#DataBased-525"><span class="linenos">525</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased-526"><a href="#DataBased-526"><span class="linenos">526</span></a>
+</span><span id="DataBased-527"><a href="#DataBased-527"><span class="linenos">527</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="DataBased-528"><a href="#DataBased-528"><span class="linenos">528</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
 </span><span id="DataBased-529"><a href="#DataBased-529"><span class="linenos">529</span></a>
-</span><span id="DataBased-530"><a href="#DataBased-530"><span class="linenos">530</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="DataBased-531"><a href="#DataBased-531"><span class="linenos">531</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="DataBased-532"><a href="#DataBased-532"><span class="linenos">532</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="DataBased-530"><a href="#DataBased-530"><span class="linenos">530</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased-531"><a href="#DataBased-531"><span class="linenos">531</span></a>
+</span><span id="DataBased-532"><a href="#DataBased-532"><span class="linenos">532</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="DataBased-533"><a href="#DataBased-533"><span class="linenos">533</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="DataBased-534"><a href="#DataBased-534"><span class="linenos">534</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Sqli wrapper so queries don't need to be written except table definitions.</p>
 
 <p>Supports saving and reading dates as datetime objects.</p>
 
@@ -1392,15 +1396,15 @@
 </span><span id="DataBased.create_tables-164"><a href="#DataBased.create_tables-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Create tables if they don&#39;t exist.</span>
 </span><span id="DataBased.create_tables-165"><a href="#DataBased.create_tables-165"><span class="linenos">165</span></a>
 </span><span id="DataBased.create_tables-166"><a href="#DataBased.create_tables-166"><span class="linenos">166</span></a><span class="sd">        :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`&quot;&quot;&quot;</span>
 </span><span id="DataBased.create_tables-167"><a href="#DataBased.create_tables-167"><span class="linenos">167</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">table_defs</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
 </span><span id="DataBased.create_tables-168"><a href="#DataBased.create_tables-168"><span class="linenos">168</span></a>            <span class="n">table_names</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">()</span>
 </span><span id="DataBased.create_tables-169"><a href="#DataBased.create_tables-169"><span class="linenos">169</span></a>            <span class="k">for</span> <span class="n">table</span> <span class="ow">in</span> <span class="n">table_defs</span><span class="p">:</span>
 </span><span id="DataBased.create_tables-170"><a href="#DataBased.create_tables-170"><span class="linenos">170</span></a>                <span class="k">if</span> <span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">table_names</span><span class="p">:</span>
-</span><span id="DataBased.create_tables-171"><a href="#DataBased.create_tables-171"><span class="linenos">171</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.create_tables-171"><a href="#DataBased.create_tables-171"><span class="linenos">171</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
 </span><span id="DataBased.create_tables-172"><a href="#DataBased.create_tables-172"><span class="linenos">172</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;</span><span class="si">{</span><span class="n">table</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s2">&quot;(&quot;</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1"> table created.&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create tables if they don't exist.</p>
 
 <h6 id="parameters">Parameters</h6>
@@ -1430,15 +1434,15 @@
 </span><span id="DataBased.create_table-178"><a href="#DataBased.create_table-178"><span class="linenos">178</span></a><span class="sd">        #### :params:</span>
 </span><span id="DataBased.create_table-179"><a href="#DataBased.create_table-179"><span class="linenos">179</span></a>
 </span><span id="DataBased.create_table-180"><a href="#DataBased.create_table-180"><span class="linenos">180</span></a><span class="sd">        `table`: Name of the table to create.</span>
 </span><span id="DataBased.create_table-181"><a href="#DataBased.create_table-181"><span class="linenos">181</span></a>
 </span><span id="DataBased.create_table-182"><a href="#DataBased.create_table-182"><span class="linenos">182</span></a><span class="sd">        `column_defs`: List of column definitions in proper Sqlite3 sytax.</span>
 </span><span id="DataBased.create_table-183"><a href="#DataBased.create_table-183"><span class="linenos">183</span></a><span class="sd">        i.e. `&quot;column_name text unique&quot;` or `&quot;column_name int primary key&quot;` etc.&quot;&quot;&quot;</span>
 </span><span id="DataBased.create_table-184"><a href="#DataBased.create_table-184"><span class="linenos">184</span></a>        <span class="k">if</span> <span class="n">table</span> <span class="ow">not</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">get_table_names</span><span class="p">():</span>
-</span><span id="DataBased.create_table-185"><a href="#DataBased.create_table-185"><span class="linenos">185</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">(</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
+</span><span id="DataBased.create_table-185"><a href="#DataBased.create_table-185"><span class="linenos">185</span></a>            <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;create table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">](</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column_defs</span><span class="p">)</span><span class="si">}</span><span class="s2">);&quot;</span>
 </span><span id="DataBased.create_table-186"><a href="#DataBased.create_table-186"><span class="linenos">186</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query</span><span class="p">)</span>
 </span><span id="DataBased.create_table-187"><a href="#DataBased.create_table-187"><span class="linenos">187</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;&#39;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&#39; table created.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a table if it doesn't exist.</p>
 
@@ -1488,15 +1492,15 @@
                 <label class="view-source-button" for="DataBased.get_column_names-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.get_column_names"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.get_column_names-197"><a href="#DataBased.get_column_names-197"><span class="linenos">197</span></a>    <span class="nd">@_connect</span>
 </span><span id="DataBased.get_column_names-198"><a href="#DataBased.get_column_names-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">get_column_names</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
 </span><span id="DataBased.get_column_names-199"><a href="#DataBased.get_column_names-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Return a list of column names from a table.&quot;&quot;&quot;</span>
-</span><span id="DataBased.get_column_names-200"><a href="#DataBased.get_column_names-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where 1=0&quot;</span><span class="p">)</span>
+</span><span id="DataBased.get_column_names-200"><a href="#DataBased.get_column_names-200"><span class="linenos">200</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where 1=0;&quot;</span><span class="p">)</span>
 </span><span id="DataBased.get_column_names-201"><a href="#DataBased.get_column_names-201"><span class="linenos">201</span></a>        <span class="k">return</span> <span class="p">[</span><span class="n">description</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="k">for</span> <span class="n">description</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">description</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a list of column names from a table.</p>
 </div>
 
@@ -1529,15 +1533,15 @@
 </span><span id="DataBased.count-216"><a href="#DataBased.count-216"><span class="linenos">216</span></a><span class="sd">        keys are column names and values are row values.</span>
 </span><span id="DataBased.count-217"><a href="#DataBased.count-217"><span class="linenos">217</span></a><span class="sd">        If `None`, all rows from the table will be counted.</span>
 </span><span id="DataBased.count-218"><a href="#DataBased.count-218"><span class="linenos">218</span></a>
 </span><span id="DataBased.count-219"><a href="#DataBased.count-219"><span class="linenos">219</span></a><span class="sd">        `exact_match`: If `False`, the row value for a given column</span>
 </span><span id="DataBased.count-220"><a href="#DataBased.count-220"><span class="linenos">220</span></a><span class="sd">        in `match_criteria` will be matched as a substring.</span>
 </span><span id="DataBased.count-221"><a href="#DataBased.count-221"><span class="linenos">221</span></a><span class="sd">        Has no effect if `match_criteria` is `None`.</span>
 </span><span id="DataBased.count-222"><a href="#DataBased.count-222"><span class="linenos">222</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="DataBased.count-223"><a href="#DataBased.count-223"><span class="linenos">223</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.count-223"><a href="#DataBased.count-223"><span class="linenos">223</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select count(_rowid_) from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
 </span><span id="DataBased.count-224"><a href="#DataBased.count-224"><span class="linenos">224</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="DataBased.count-225"><a href="#DataBased.count-225"><span class="linenos">225</span></a>            <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="DataBased.count-226"><a href="#DataBased.count-226"><span class="linenos">226</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
 </span><span id="DataBased.count-227"><a href="#DataBased.count-227"><span class="linenos">227</span></a>                    <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">;&quot;</span>
 </span><span id="DataBased.count-228"><a href="#DataBased.count-228"><span class="linenos">228</span></a>                <span class="p">)</span>
 </span><span id="DataBased.count-229"><a href="#DataBased.count-229"><span class="linenos">229</span></a>            <span class="k">else</span><span class="p">:</span>
 </span><span id="DataBased.count-230"><a href="#DataBased.count-230"><span class="linenos">230</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">query</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
@@ -1592,20 +1596,20 @@
 </span><span id="DataBased.add_row-250"><a href="#DataBased.add_row-250"><span class="linenos">250</span></a><span class="sd">        If `columns` is provided, it should contain the same number of elements as `values`.&quot;&quot;&quot;</span>
 </span><span id="DataBased.add_row-251"><a href="#DataBased.add_row-251"><span class="linenos">251</span></a>        <span class="n">parameterizer</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s2">&quot;?&quot;</span> <span class="k">for</span> <span class="n">_</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
 </span><span id="DataBased.add_row-252"><a href="#DataBased.add_row-252"><span class="linenos">252</span></a>        <span class="n">logger_values</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">value</span><span class="p">)</span> <span class="k">for</span> <span class="n">value</span> <span class="ow">in</span> <span class="n">values</span><span class="p">)</span>
 </span><span id="DataBased.add_row-253"><a href="#DataBased.add_row-253"><span class="linenos">253</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="DataBased.add_row-254"><a href="#DataBased.add_row-254"><span class="linenos">254</span></a>            <span class="k">if</span> <span class="n">columns</span><span class="p">:</span>
 </span><span id="DataBased.add_row-255"><a href="#DataBased.add_row-255"><span class="linenos">255</span></a>                <span class="n">columns_query</span> <span class="o">=</span> <span class="s2">&quot;, &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">column</span> <span class="k">for</span> <span class="n">column</span> <span class="ow">in</span> <span class="n">columns</span><span class="p">)</span>
 </span><span id="DataBased.add_row-256"><a href="#DataBased.add_row-256"><span class="linenos">256</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_row-257"><a href="#DataBased.add_row-257"><span class="linenos">257</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
+</span><span id="DataBased.add_row-257"><a href="#DataBased.add_row-257"><span class="linenos">257</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] (</span><span class="si">{</span><span class="n">columns_query</span><span class="si">}</span><span class="s2">) values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span>
 </span><span id="DataBased.add_row-258"><a href="#DataBased.add_row-258"><span class="linenos">258</span></a>                    <span class="n">values</span><span class="p">,</span>
 </span><span id="DataBased.add_row-259"><a href="#DataBased.add_row-259"><span class="linenos">259</span></a>                <span class="p">)</span>
 </span><span id="DataBased.add_row-260"><a href="#DataBased.add_row-260"><span class="linenos">260</span></a>            <span class="k">else</span><span class="p">:</span>
 </span><span id="DataBased.add_row-261"><a href="#DataBased.add_row-261"><span class="linenos">261</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_row-262"><a href="#DataBased.add_row-262"><span class="linenos">262</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
+</span><span id="DataBased.add_row-262"><a href="#DataBased.add_row-262"><span class="linenos">262</span></a>                    <span class="sa">f</span><span class="s2">&quot;insert into [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] values(</span><span class="si">{</span><span class="n">parameterizer</span><span class="si">}</span><span class="s2">);&quot;</span><span class="p">,</span> <span class="n">values</span>
 </span><span id="DataBased.add_row-263"><a href="#DataBased.add_row-263"><span class="linenos">263</span></a>                <span class="p">)</span>
 </span><span id="DataBased.add_row-264"><a href="#DataBased.add_row-264"><span class="linenos">264</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span><span class="p">)</span>
 </span><span id="DataBased.add_row-265"><a href="#DataBased.add_row-265"><span class="linenos">265</span></a>            <span class="k">return</span> <span class="kc">True</span>
 </span><span id="DataBased.add_row-266"><a href="#DataBased.add_row-266"><span class="linenos">266</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="DataBased.add_row-267"><a href="#DataBased.add_row-267"><span class="linenos">267</span></a>            <span class="k">if</span> <span class="s2">&quot;constraint&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="nb">str</span><span class="p">(</span><span class="n">e</span><span class="p">)</span><span class="o">.</span><span class="n">lower</span><span class="p">():</span>
 </span><span id="DataBased.add_row-268"><a href="#DataBased.add_row-268"><span class="linenos">268</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">exception</span><span class="p">(</span>
 </span><span id="DataBased.add_row-269"><a href="#DataBased.add_row-269"><span class="linenos">269</span></a>                    <span class="sa">f</span><span class="s1">&#39;Error adding &quot;</span><span class="si">{</span><span class="n">logger_values</span><span class="si">}</span><span class="s1">&quot; to </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1"> table.&#39;</span>
@@ -1740,15 +1744,15 @@
 </span><span id="DataBased.get_rows-339"><a href="#DataBased.get_rows-339"><span class="linenos">339</span></a><span class="sd">        `order_by`: If given, a `order by {order_by}` clause will be added to the select query.</span>
 </span><span id="DataBased.get_rows-340"><a href="#DataBased.get_rows-340"><span class="linenos">340</span></a>
 </span><span id="DataBased.get_rows-341"><a href="#DataBased.get_rows-341"><span class="linenos">341</span></a><span class="sd">        `limit`: If given, a `limit {limit}` clause will be added to the select query.</span>
 </span><span id="DataBased.get_rows-342"><a href="#DataBased.get_rows-342"><span class="linenos">342</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="DataBased.get_rows-343"><a href="#DataBased.get_rows-343"><span class="linenos">343</span></a>
 </span><span id="DataBased.get_rows-344"><a href="#DataBased.get_rows-344"><span class="linenos">344</span></a>        <span class="k">if</span> <span class="nb">type</span><span class="p">(</span><span class="n">columns_to_return</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span><span class="p">:</span>
 </span><span id="DataBased.get_rows-345"><a href="#DataBased.get_rows-345"><span class="linenos">345</span></a>            <span class="n">columns_to_return</span> <span class="o">=</span> <span class="p">[</span><span class="n">columns_to_return</span><span class="p">]</span>
-</span><span id="DataBased.get_rows-346"><a href="#DataBased.get_rows-346"><span class="linenos">346</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DataBased.get_rows-346"><a href="#DataBased.get_rows-346"><span class="linenos">346</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;select * from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">]&quot;</span>
 </span><span id="DataBased.get_rows-347"><a href="#DataBased.get_rows-347"><span class="linenos">347</span></a>        <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="DataBased.get_rows-348"><a href="#DataBased.get_rows-348"><span class="linenos">348</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="DataBased.get_rows-349"><a href="#DataBased.get_rows-349"><span class="linenos">349</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="DataBased.get_rows-350"><a href="#DataBased.get_rows-350"><span class="linenos">350</span></a>        <span class="k">if</span> <span class="n">order_by</span><span class="p">:</span>
 </span><span id="DataBased.get_rows-351"><a href="#DataBased.get_rows-351"><span class="linenos">351</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; order by </span><span class="si">{</span><span class="n">order_by</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="DataBased.get_rows-352"><a href="#DataBased.get_rows-352"><span class="linenos">352</span></a>        <span class="k">if</span> <span class="n">limit</span><span class="p">:</span>
 </span><span id="DataBased.get_rows-353"><a href="#DataBased.get_rows-353"><span class="linenos">353</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; limit </span><span class="si">{</span><span class="n">limit</span><span class="si">}</span><span class="s2">&quot;</span>
@@ -1881,15 +1885,15 @@
 </span><span id="DataBased.delete-409"><a href="#DataBased.delete-409"><span class="linenos">409</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`</span>
 </span><span id="DataBased.delete-410"><a href="#DataBased.delete-410"><span class="linenos">410</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
 </span><span id="DataBased.delete-411"><a href="#DataBased.delete-411"><span class="linenos">411</span></a>
 </span><span id="DataBased.delete-412"><a href="#DataBased.delete-412"><span class="linenos">412</span></a><span class="sd">        `exact_match`: If `False`, the value for a given column will be matched as a substring.</span>
 </span><span id="DataBased.delete-413"><a href="#DataBased.delete-413"><span class="linenos">413</span></a><span class="sd">        &quot;&quot;&quot;</span>
 </span><span id="DataBased.delete-414"><a href="#DataBased.delete-414"><span class="linenos">414</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
 </span><span id="DataBased.delete-415"><a href="#DataBased.delete-415"><span class="linenos">415</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.delete-416"><a href="#DataBased.delete-416"><span class="linenos">416</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.delete-416"><a href="#DataBased.delete-416"><span class="linenos">416</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;delete from [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
 </span><span id="DataBased.delete-417"><a href="#DataBased.delete-417"><span class="linenos">417</span></a>            <span class="n">num_deletions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">rowcount</span>
 </span><span id="DataBased.delete-418"><a href="#DataBased.delete-418"><span class="linenos">418</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span>
 </span><span id="DataBased.delete-419"><a href="#DataBased.delete-419"><span class="linenos">419</span></a>                <span class="sa">f</span><span class="s1">&#39;Deleted </span><span class="si">{</span><span class="n">num_deletions</span><span class="si">}</span><span class="s1"> rows from &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s1">&quot;.&#39;</span>
 </span><span id="DataBased.delete-420"><a href="#DataBased.delete-420"><span class="linenos">420</span></a>            <span class="p">)</span>
 </span><span id="DataBased.delete-421"><a href="#DataBased.delete-421"><span class="linenos">421</span></a>            <span class="k">return</span> <span class="n">num_deletions</span>
 </span><span id="DataBased.delete-422"><a href="#DataBased.delete-422"><span class="linenos">422</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="DataBased.delete-423"><a href="#DataBased.delete-423"><span class="linenos">423</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span>
@@ -1946,15 +1950,15 @@
 </span><span id="DataBased.update-447"><a href="#DataBased.update-447"><span class="linenos">447</span></a><span class="sd">        `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`</span>
 </span><span id="DataBased.update-448"><a href="#DataBased.update-448"><span class="linenos">448</span></a><span class="sd">        or a dictionary where keys are column names and values are corresponding values.</span>
 </span><span id="DataBased.update-449"><a href="#DataBased.update-449"><span class="linenos">449</span></a><span class="sd">        If `None`, every row in `table` will be updated.</span>
 </span><span id="DataBased.update-450"><a href="#DataBased.update-450"><span class="linenos">450</span></a>
 </span><span id="DataBased.update-451"><a href="#DataBased.update-451"><span class="linenos">451</span></a><span class="sd">        `exact_match`: If `False`, `match_criteria` values will be treated as substrings.</span>
 </span><span id="DataBased.update-452"><a href="#DataBased.update-452"><span class="linenos">452</span></a>
 </span><span id="DataBased.update-453"><a href="#DataBased.update-453"><span class="linenos">453</span></a><span class="sd">        Returns the number of updated rows.&quot;&quot;&quot;</span>
-</span><span id="DataBased.update-454"><a href="#DataBased.update-454"><span class="linenos">454</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
+</span><span id="DataBased.update-454"><a href="#DataBased.update-454"><span class="linenos">454</span></a>        <span class="n">query</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;update [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] set </span><span class="si">{</span><span class="n">column_to_update</span><span class="si">}</span><span class="s2"> = ?&quot;</span>
 </span><span id="DataBased.update-455"><a href="#DataBased.update-455"><span class="linenos">455</span></a>        <span class="n">conditions</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span>
 </span><span id="DataBased.update-456"><a href="#DataBased.update-456"><span class="linenos">456</span></a>        <span class="k">if</span> <span class="n">match_criteria</span><span class="p">:</span>
 </span><span id="DataBased.update-457"><a href="#DataBased.update-457"><span class="linenos">457</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_get_conditions</span><span class="p">(</span><span class="n">match_criteria</span><span class="p">,</span> <span class="n">exact_match</span><span class="p">)</span>
 </span><span id="DataBased.update-458"><a href="#DataBased.update-458"><span class="linenos">458</span></a>            <span class="n">query</span> <span class="o">+=</span> <span class="sa">f</span><span class="s2">&quot; where </span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="DataBased.update-459"><a href="#DataBased.update-459"><span class="linenos">459</span></a>        <span class="k">else</span><span class="p">:</span>
 </span><span id="DataBased.update-460"><a href="#DataBased.update-460"><span class="linenos">460</span></a>            <span class="n">conditions</span> <span class="o">=</span> <span class="kc">None</span>
 </span><span id="DataBased.update-461"><a href="#DataBased.update-461"><span class="linenos">461</span></a>        <span class="n">query</span> <span class="o">+=</span> <span class="s2">&quot;;&quot;</span>
@@ -2010,15 +2014,15 @@
     <a class="headerlink" href="#DataBased.drop_table"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.drop_table-478"><a href="#DataBased.drop_table-478"><span class="linenos">478</span></a>    <span class="nd">@_connect</span>
 </span><span id="DataBased.drop_table-479"><a href="#DataBased.drop_table-479"><span class="linenos">479</span></a>    <span class="k">def</span> <span class="nf">drop_table</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">table</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
 </span><span id="DataBased.drop_table-480"><a href="#DataBased.drop_table-480"><span class="linenos">480</span></a>        <span class="sd">&quot;&quot;&quot;Drop `table` from the database.</span>
 </span><span id="DataBased.drop_table-481"><a href="#DataBased.drop_table-481"><span class="linenos">481</span></a>
 </span><span id="DataBased.drop_table-482"><a href="#DataBased.drop_table-482"><span class="linenos">482</span></a><span class="sd">        Returns `True` if successful, `False` if not.&quot;&quot;&quot;</span>
 </span><span id="DataBased.drop_table-483"><a href="#DataBased.drop_table-483"><span class="linenos">483</span></a>        <span class="k">try</span><span class="p">:</span>
-</span><span id="DataBased.drop_table-484"><a href="#DataBased.drop_table-484"><span class="linenos">484</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
+</span><span id="DataBased.drop_table-484"><a href="#DataBased.drop_table-484"><span class="linenos">484</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;drop Table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">];&quot;</span><span class="p">)</span>
 </span><span id="DataBased.drop_table-485"><a href="#DataBased.drop_table-485"><span class="linenos">485</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Dropped table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="DataBased.drop_table-486"><a href="#DataBased.drop_table-486"><span class="linenos">486</span></a>            <span class="k">return</span> <span class="kc">True</span>
 </span><span id="DataBased.drop_table-487"><a href="#DataBased.drop_table-487"><span class="linenos">487</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
 </span><span id="DataBased.drop_table-488"><a href="#DataBased.drop_table-488"><span class="linenos">488</span></a>            <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
 </span><span id="DataBased.drop_table-489"><a href="#DataBased.drop_table-489"><span class="linenos">489</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to drop table &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span><span id="DataBased.drop_table-490"><a href="#DataBased.drop_table-490"><span class="linenos">490</span></a>            <span class="k">return</span> <span class="kc">False</span>
 </span></pre></div>
@@ -2054,22 +2058,24 @@
 </span><span id="DataBased.add_column-501"><a href="#DataBased.add_column-501"><span class="linenos">501</span></a>
 </span><span id="DataBased.add_column-502"><a href="#DataBased.add_column-502"><span class="linenos">502</span></a><span class="sd">        `_type`: The data type of the new column.</span>
 </span><span id="DataBased.add_column-503"><a href="#DataBased.add_column-503"><span class="linenos">503</span></a>
 </span><span id="DataBased.add_column-504"><a href="#DataBased.add_column-504"><span class="linenos">504</span></a><span class="sd">        `default_value`: Optional default value for the column.&quot;&quot;&quot;</span>
 </span><span id="DataBased.add_column-505"><a href="#DataBased.add_column-505"><span class="linenos">505</span></a>        <span class="k">try</span><span class="p">:</span>
 </span><span id="DataBased.add_column-506"><a href="#DataBased.add_column-506"><span class="linenos">506</span></a>            <span class="k">if</span> <span class="n">default_value</span><span class="p">:</span>
 </span><span id="DataBased.add_column-507"><a href="#DataBased.add_column-507"><span class="linenos">507</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
-</span><span id="DataBased.add_column-508"><a href="#DataBased.add_column-508"><span class="linenos">508</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased.add_column-508"><a href="#DataBased.add_column-508"><span class="linenos">508</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2"> default </span><span class="si">{</span><span class="n">default_value</span><span class="si">}</span><span class="s2">;&quot;</span>
 </span><span id="DataBased.add_column-509"><a href="#DataBased.add_column-509"><span class="linenos">509</span></a>                <span class="p">)</span>
 </span><span id="DataBased.add_column-510"><a href="#DataBased.add_column-510"><span class="linenos">510</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="n">column</span><span class="p">,</span> <span class="n">default_value</span><span class="p">)</span>
 </span><span id="DataBased.add_column-511"><a href="#DataBased.add_column-511"><span class="linenos">511</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DataBased.add_column-512"><a href="#DataBased.add_column-512"><span class="linenos">512</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;alter table </span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2"> add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span><span class="p">)</span>
-</span><span id="DataBased.add_column-513"><a href="#DataBased.add_column-513"><span class="linenos">513</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
-</span><span id="DataBased.add_column-514"><a href="#DataBased.add_column-514"><span class="linenos">514</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DataBased.add_column-515"><a href="#DataBased.add_column-515"><span class="linenos">515</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_column-512"><a href="#DataBased.add_column-512"><span class="linenos">512</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
+</span><span id="DataBased.add_column-513"><a href="#DataBased.add_column-513"><span class="linenos">513</span></a>                    <span class="sa">f</span><span class="s2">&quot;alter table [</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s2">] add column </span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">_type</span><span class="si">}</span><span class="s2">;&quot;</span>
+</span><span id="DataBased.add_column-514"><a href="#DataBased.add_column-514"><span class="linenos">514</span></a>                <span class="p">)</span>
+</span><span id="DataBased.add_column-515"><a href="#DataBased.add_column-515"><span class="linenos">515</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">info</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Added column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
+</span><span id="DataBased.add_column-516"><a href="#DataBased.add_column-516"><span class="linenos">516</span></a>        <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DataBased.add_column-517"><a href="#DataBased.add_column-517"><span class="linenos">517</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">logger</span><span class="o">.</span><span class="n">error</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;Failed to add column &quot;</span><span class="si">{</span><span class="n">column</span><span class="si">}</span><span class="s1">&quot; to &quot;</span><span class="si">{</span><span class="n">table</span><span class="si">}</span><span class="s1">&quot; table.&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add a new column to <code>table</code>.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -2090,30 +2096,30 @@
         <span class="def">def</span>
         <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="DataBased.data_to_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.data_to_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.data_to_string-517"><a href="#DataBased.data_to_string-517"><span class="linenos">517</span></a>    <span class="nd">@staticmethod</span>
-</span><span id="DataBased.data_to_string-518"><a href="#DataBased.data_to_string-518"><span class="linenos">518</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="DataBased.data_to_string-519"><a href="#DataBased.data_to_string-519"><span class="linenos">519</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="DataBased.data_to_string-520"><a href="#DataBased.data_to_string-520"><span class="linenos">520</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="DataBased.data_to_string-521"><a href="#DataBased.data_to_string-521"><span class="linenos">521</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="DataBased.data_to_string-522"><a href="#DataBased.data_to_string-522"><span class="linenos">522</span></a>
-</span><span id="DataBased.data_to_string-523"><a href="#DataBased.data_to_string-523"><span class="linenos">523</span></a><span class="sd">        #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.data_to_string-519"><a href="#DataBased.data_to_string-519"><span class="linenos">519</span></a>    <span class="nd">@staticmethod</span>
+</span><span id="DataBased.data_to_string-520"><a href="#DataBased.data_to_string-520"><span class="linenos">520</span></a>    <span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="DataBased.data_to_string-521"><a href="#DataBased.data_to_string-521"><span class="linenos">521</span></a>        <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="DataBased.data_to_string-522"><a href="#DataBased.data_to_string-522"><span class="linenos">522</span></a>    <span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="DataBased.data_to_string-523"><a href="#DataBased.data_to_string-523"><span class="linenos">523</span></a>        <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
 </span><span id="DataBased.data_to_string-524"><a href="#DataBased.data_to_string-524"><span class="linenos">524</span></a>
-</span><span id="DataBased.data_to_string-525"><a href="#DataBased.data_to_string-525"><span class="linenos">525</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="DataBased.data_to_string-526"><a href="#DataBased.data_to_string-526"><span class="linenos">526</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="DataBased.data_to_string-527"><a href="#DataBased.data_to_string-527"><span class="linenos">527</span></a>
-</span><span id="DataBased.data_to_string-528"><a href="#DataBased.data_to_string-528"><span class="linenos">528</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased.data_to_string-525"><a href="#DataBased.data_to_string-525"><span class="linenos">525</span></a><span class="sd">        #### :params:</span>
+</span><span id="DataBased.data_to_string-526"><a href="#DataBased.data_to_string-526"><span class="linenos">526</span></a>
+</span><span id="DataBased.data_to_string-527"><a href="#DataBased.data_to_string-527"><span class="linenos">527</span></a><span class="sd">        `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="DataBased.data_to_string-528"><a href="#DataBased.data_to_string-528"><span class="linenos">528</span></a><span class="sd">        Assumes all dictionaries in list have the same set of keys.</span>
 </span><span id="DataBased.data_to_string-529"><a href="#DataBased.data_to_string-529"><span class="linenos">529</span></a>
-</span><span id="DataBased.data_to_string-530"><a href="#DataBased.data_to_string-530"><span class="linenos">530</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="DataBased.data_to_string-531"><a href="#DataBased.data_to_string-531"><span class="linenos">531</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="DataBased.data_to_string-532"><a href="#DataBased.data_to_string-532"><span class="linenos">532</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
+</span><span id="DataBased.data_to_string-530"><a href="#DataBased.data_to_string-530"><span class="linenos">530</span></a><span class="sd">        `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="DataBased.data_to_string-531"><a href="#DataBased.data_to_string-531"><span class="linenos">531</span></a>
+</span><span id="DataBased.data_to_string-532"><a href="#DataBased.data_to_string-532"><span class="linenos">532</span></a><span class="sd">        `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="DataBased.data_to_string-533"><a href="#DataBased.data_to_string-533"><span class="linenos">533</span></a><span class="sd">        Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="DataBased.data_to_string-534"><a href="#DataBased.data_to_string-534"><span class="linenos">534</span></a>        <span class="k">return</span> <span class="n">data_to_string</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">sort_key</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses tabulate to produce pretty string output from a list of dictionaries.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -2136,80 +2142,80 @@
         <span class="def">def</span>
         <span class="name">data_to_string</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">]</span>,</span><span class="param">	<span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">) -> <span class="nb">str</span>:</span></span>
 
                 <label class="view-source-button" for="data_to_string-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#data_to_string"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="data_to_string-535"><a href="#data_to_string-535"><span class="linenos">535</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
-</span><span id="data_to_string-536"><a href="#data_to_string-536"><span class="linenos">536</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="data_to_string-537"><a href="#data_to_string-537"><span class="linenos">537</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
-</span><span id="data_to_string-538"><a href="#data_to_string-538"><span class="linenos">538</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
-</span><span id="data_to_string-539"><a href="#data_to_string-539"><span class="linenos">539</span></a>
-</span><span id="data_to_string-540"><a href="#data_to_string-540"><span class="linenos">540</span></a><span class="sd">    #### :params:</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="data_to_string-537"><a href="#data_to_string-537"><span class="linenos">537</span></a><span class="k">def</span> <span class="nf">data_to_string</span><span class="p">(</span>
+</span><span id="data_to_string-538"><a href="#data_to_string-538"><span class="linenos">538</span></a>    <span class="n">data</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">dict</span><span class="p">],</span> <span class="n">sort_key</span><span class="p">:</span> <span class="nb">str</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">wrap_to_terminal</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="data_to_string-539"><a href="#data_to_string-539"><span class="linenos">539</span></a><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span><span class="p">:</span>
+</span><span id="data_to_string-540"><a href="#data_to_string-540"><span class="linenos">540</span></a>    <span class="sd">&quot;&quot;&quot;Uses tabulate to produce pretty string output from a list of dictionaries.</span>
 </span><span id="data_to_string-541"><a href="#data_to_string-541"><span class="linenos">541</span></a>
-</span><span id="data_to_string-542"><a href="#data_to_string-542"><span class="linenos">542</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
-</span><span id="data_to_string-543"><a href="#data_to_string-543"><span class="linenos">543</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
-</span><span id="data_to_string-544"><a href="#data_to_string-544"><span class="linenos">544</span></a>
-</span><span id="data_to_string-545"><a href="#data_to_string-545"><span class="linenos">545</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="data_to_string-542"><a href="#data_to_string-542"><span class="linenos">542</span></a><span class="sd">    #### :params:</span>
+</span><span id="data_to_string-543"><a href="#data_to_string-543"><span class="linenos">543</span></a>
+</span><span id="data_to_string-544"><a href="#data_to_string-544"><span class="linenos">544</span></a><span class="sd">    `data`: The list of dictionaries to create a grid from.</span>
+</span><span id="data_to_string-545"><a href="#data_to_string-545"><span class="linenos">545</span></a><span class="sd">    Assumes all dictionaries in list have the same set of keys.</span>
 </span><span id="data_to_string-546"><a href="#data_to_string-546"><span class="linenos">546</span></a>
-</span><span id="data_to_string-547"><a href="#data_to_string-547"><span class="linenos">547</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
-</span><span id="data_to_string-548"><a href="#data_to_string-548"><span class="linenos">548</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
-</span><span id="data_to_string-549"><a href="#data_to_string-549"><span class="linenos">549</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="data_to_string-550"><a href="#data_to_string-550"><span class="linenos">550</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
-</span><span id="data_to_string-551"><a href="#data_to_string-551"><span class="linenos">551</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
-</span><span id="data_to_string-552"><a href="#data_to_string-552"><span class="linenos">552</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
-</span><span id="data_to_string-553"><a href="#data_to_string-553"><span class="linenos">553</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
-</span><span id="data_to_string-554"><a href="#data_to_string-554"><span class="linenos">554</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
-</span><span id="data_to_string-555"><a href="#data_to_string-555"><span class="linenos">555</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
-</span><span id="data_to_string-556"><a href="#data_to_string-556"><span class="linenos">556</span></a>
-</span><span id="data_to_string-557"><a href="#data_to_string-557"><span class="linenos">557</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="data_to_string-558"><a href="#data_to_string-558"><span class="linenos">558</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
-</span><span id="data_to_string-559"><a href="#data_to_string-559"><span class="linenos">559</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
-</span><span id="data_to_string-560"><a href="#data_to_string-560"><span class="linenos">560</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
-</span><span id="data_to_string-561"><a href="#data_to_string-561"><span class="linenos">561</span></a>    <span class="c1"># to see if shrinking is necessary</span>
-</span><span id="data_to_string-562"><a href="#data_to_string-562"><span class="linenos">562</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="data_to_string-563"><a href="#data_to_string-563"><span class="linenos">563</span></a>        <span class="n">data</span><span class="p">,</span>
-</span><span id="data_to_string-564"><a href="#data_to_string-564"><span class="linenos">564</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-565"><a href="#data_to_string-565"><span class="linenos">565</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="data_to_string-566"><a href="#data_to_string-566"><span class="linenos">566</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-567"><a href="#data_to_string-567"><span class="linenos">567</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="data_to_string-568"><a href="#data_to_string-568"><span class="linenos">568</span></a>    <span class="p">)</span>
-</span><span id="data_to_string-569"><a href="#data_to_string-569"><span class="linenos">569</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-570"><a href="#data_to_string-570"><span class="linenos">570</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-571"><a href="#data_to_string-571"><span class="linenos">571</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="data_to_string-572"><a href="#data_to_string-572"><span class="linenos">572</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="data_to_string-573"><a href="#data_to_string-573"><span class="linenos">573</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-574"><a href="#data_to_string-574"><span class="linenos">574</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="data_to_string-575"><a href="#data_to_string-575"><span class="linenos">575</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
-</span><span id="data_to_string-576"><a href="#data_to_string-576"><span class="linenos">576</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="data_to_string-577"><a href="#data_to_string-577"><span class="linenos">577</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;=</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-578"><a href="#data_to_string-578"><span class="linenos">578</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
-</span><span id="data_to_string-579"><a href="#data_to_string-579"><span class="linenos">579</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
-</span><span id="data_to_string-580"><a href="#data_to_string-580"><span class="linenos">580</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-581"><a href="#data_to_string-581"><span class="linenos">581</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
-</span><span id="data_to_string-582"><a href="#data_to_string-582"><span class="linenos">582</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="data_to_string-583"><a href="#data_to_string-583"><span class="linenos">583</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
-</span><span id="data_to_string-584"><a href="#data_to_string-584"><span class="linenos">584</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
-</span><span id="data_to_string-585"><a href="#data_to_string-585"><span class="linenos">585</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
-</span><span id="data_to_string-586"><a href="#data_to_string-586"><span class="linenos">586</span></a>                <span class="p">)</span>
-</span><span id="data_to_string-587"><a href="#data_to_string-587"><span class="linenos">587</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
-</span><span id="data_to_string-588"><a href="#data_to_string-588"><span class="linenos">588</span></a>                <span class="n">data</span><span class="p">,</span>
-</span><span id="data_to_string-589"><a href="#data_to_string-589"><span class="linenos">589</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-590"><a href="#data_to_string-590"><span class="linenos">590</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
-</span><span id="data_to_string-591"><a href="#data_to_string-591"><span class="linenos">591</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
-</span><span id="data_to_string-592"><a href="#data_to_string-592"><span class="linenos">592</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
-</span><span id="data_to_string-593"><a href="#data_to_string-593"><span class="linenos">593</span></a>            <span class="p">)</span>
-</span><span id="data_to_string-594"><a href="#data_to_string-594"><span class="linenos">594</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-595"><a href="#data_to_string-595"><span class="linenos">595</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
-</span><span id="data_to_string-596"><a href="#data_to_string-596"><span class="linenos">596</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
-</span><span id="data_to_string-597"><a href="#data_to_string-597"><span class="linenos">597</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
-</span><span id="data_to_string-598"><a href="#data_to_string-598"><span class="linenos">598</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
-</span><span id="data_to_string-599"><a href="#data_to_string-599"><span class="linenos">599</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
-</span><span id="data_to_string-600"><a href="#data_to_string-600"><span class="linenos">600</span></a>    <span class="k">return</span> <span class="n">output</span>
+</span><span id="data_to_string-547"><a href="#data_to_string-547"><span class="linenos">547</span></a><span class="sd">    `sort_key`: Optional dictionary key to sort data with.</span>
+</span><span id="data_to_string-548"><a href="#data_to_string-548"><span class="linenos">548</span></a>
+</span><span id="data_to_string-549"><a href="#data_to_string-549"><span class="linenos">549</span></a><span class="sd">    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit within the current terminal window.</span>
+</span><span id="data_to_string-550"><a href="#data_to_string-550"><span class="linenos">550</span></a><span class="sd">    Pass as `False` if the output is going into something like a `.txt` file.&quot;&quot;&quot;</span>
+</span><span id="data_to_string-551"><a href="#data_to_string-551"><span class="linenos">551</span></a>    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">data</span><span class="p">)</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="data_to_string-552"><a href="#data_to_string-552"><span class="linenos">552</span></a>        <span class="k">return</span> <span class="s2">&quot;&quot;</span>
+</span><span id="data_to_string-553"><a href="#data_to_string-553"><span class="linenos">553</span></a>    <span class="k">if</span> <span class="n">sort_key</span><span class="p">:</span>
+</span><span id="data_to_string-554"><a href="#data_to_string-554"><span class="linenos">554</span></a>        <span class="n">data</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">d</span><span class="p">:</span> <span class="n">d</span><span class="p">[</span><span class="n">sort_key</span><span class="p">])</span>
+</span><span id="data_to_string-555"><a href="#data_to_string-555"><span class="linenos">555</span></a>    <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">d</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">data</span><span class="p">):</span>
+</span><span id="data_to_string-556"><a href="#data_to_string-556"><span class="linenos">556</span></a>        <span class="k">for</span> <span class="n">k</span> <span class="ow">in</span> <span class="n">d</span><span class="p">:</span>
+</span><span id="data_to_string-557"><a href="#data_to_string-557"><span class="linenos">557</span></a>            <span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">]</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">[</span><span class="n">i</span><span class="p">][</span><span class="n">k</span><span class="p">])</span>
+</span><span id="data_to_string-558"><a href="#data_to_string-558"><span class="linenos">558</span></a>
+</span><span id="data_to_string-559"><a href="#data_to_string-559"><span class="linenos">559</span></a>    <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="data_to_string-560"><a href="#data_to_string-560"><span class="linenos">560</span></a>    <span class="n">terminal_width</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">get_terminal_size</span><span class="p">()</span><span class="o">.</span><span class="n">columns</span>
+</span><span id="data_to_string-561"><a href="#data_to_string-561"><span class="linenos">561</span></a>    <span class="n">max_col_widths</span> <span class="o">=</span> <span class="n">terminal_width</span>
+</span><span id="data_to_string-562"><a href="#data_to_string-562"><span class="linenos">562</span></a>    <span class="c1"># Make an output with effectively unrestricted column widths</span>
+</span><span id="data_to_string-563"><a href="#data_to_string-563"><span class="linenos">563</span></a>    <span class="c1"># to see if shrinking is necessary</span>
+</span><span id="data_to_string-564"><a href="#data_to_string-564"><span class="linenos">564</span></a>    <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="data_to_string-565"><a href="#data_to_string-565"><span class="linenos">565</span></a>        <span class="n">data</span><span class="p">,</span>
+</span><span id="data_to_string-566"><a href="#data_to_string-566"><span class="linenos">566</span></a>        <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-567"><a href="#data_to_string-567"><span class="linenos">567</span></a>        <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="data_to_string-568"><a href="#data_to_string-568"><span class="linenos">568</span></a>        <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-569"><a href="#data_to_string-569"><span class="linenos">569</span></a>        <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="data_to_string-570"><a href="#data_to_string-570"><span class="linenos">570</span></a>    <span class="p">)</span>
+</span><span id="data_to_string-571"><a href="#data_to_string-571"><span class="linenos">571</span></a>    <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-572"><a href="#data_to_string-572"><span class="linenos">572</span></a>    <span class="k">if</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-573"><a href="#data_to_string-573"><span class="linenos">573</span></a>        <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="data_to_string-574"><a href="#data_to_string-574"><span class="linenos">574</span></a>    <span class="k">if</span> <span class="n">wrap_to_terminal</span> <span class="ow">and</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="data_to_string-575"><a href="#data_to_string-575"><span class="linenos">575</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Resizing grid to fit within the terminal...</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-576"><a href="#data_to_string-576"><span class="linenos">576</span></a>        <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="data_to_string-577"><a href="#data_to_string-577"><span class="linenos">577</span></a>        <span class="n">acceptable_width</span> <span class="o">=</span> <span class="n">terminal_width</span> <span class="o">-</span> <span class="mi">10</span>
+</span><span id="data_to_string-578"><a href="#data_to_string-578"><span class="linenos">578</span></a>        <span class="k">while</span> <span class="n">too_wide</span> <span class="ow">and</span> <span class="n">max_col_widths</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="data_to_string-579"><a href="#data_to_string-579"><span class="linenos">579</span></a>            <span class="k">if</span> <span class="n">current_width</span> <span class="o">&gt;=</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-580"><a href="#data_to_string-580"><span class="linenos">580</span></a>                <span class="n">previous_col_widths</span> <span class="o">=</span> <span class="n">max_col_widths</span>
+</span><span id="data_to_string-581"><a href="#data_to_string-581"><span class="linenos">581</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">max_col_widths</span> <span class="o">*</span> <span class="mf">0.5</span><span class="p">)</span>
+</span><span id="data_to_string-582"><a href="#data_to_string-582"><span class="linenos">582</span></a>            <span class="k">elif</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-583"><a href="#data_to_string-583"><span class="linenos">583</span></a>                <span class="c1"># Without lowering acceptable_width, this condition will cause infinite loop</span>
+</span><span id="data_to_string-584"><a href="#data_to_string-584"><span class="linenos">584</span></a>                <span class="k">if</span> <span class="n">max_col_widths</span> <span class="o">==</span> <span class="n">previous_col_widths</span> <span class="o">-</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="data_to_string-585"><a href="#data_to_string-585"><span class="linenos">585</span></a>                    <span class="n">acceptable_width</span> <span class="o">-=</span> <span class="mi">10</span>
+</span><span id="data_to_string-586"><a href="#data_to_string-586"><span class="linenos">586</span></a>                <span class="n">max_col_widths</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span>
+</span><span id="data_to_string-587"><a href="#data_to_string-587"><span class="linenos">587</span></a>                    <span class="n">max_col_widths</span> <span class="o">+</span> <span class="p">(</span><span class="mf">0.5</span> <span class="o">*</span> <span class="p">(</span><span class="n">previous_col_widths</span> <span class="o">-</span> <span class="n">max_col_widths</span><span class="p">))</span>
+</span><span id="data_to_string-588"><a href="#data_to_string-588"><span class="linenos">588</span></a>                <span class="p">)</span>
+</span><span id="data_to_string-589"><a href="#data_to_string-589"><span class="linenos">589</span></a>            <span class="n">output</span> <span class="o">=</span> <span class="n">tabulate</span><span class="p">(</span>
+</span><span id="data_to_string-590"><a href="#data_to_string-590"><span class="linenos">590</span></a>                <span class="n">data</span><span class="p">,</span>
+</span><span id="data_to_string-591"><a href="#data_to_string-591"><span class="linenos">591</span></a>                <span class="n">headers</span><span class="o">=</span><span class="s2">&quot;keys&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-592"><a href="#data_to_string-592"><span class="linenos">592</span></a>                <span class="n">disable_numparse</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
+</span><span id="data_to_string-593"><a href="#data_to_string-593"><span class="linenos">593</span></a>                <span class="n">tablefmt</span><span class="o">=</span><span class="s2">&quot;grid&quot;</span><span class="p">,</span>
+</span><span id="data_to_string-594"><a href="#data_to_string-594"><span class="linenos">594</span></a>                <span class="n">maxcolwidths</span><span class="o">=</span><span class="n">max_col_widths</span><span class="p">,</span>
+</span><span id="data_to_string-595"><a href="#data_to_string-595"><span class="linenos">595</span></a>            <span class="p">)</span>
+</span><span id="data_to_string-596"><a href="#data_to_string-596"><span class="linenos">596</span></a>            <span class="n">current_width</span> <span class="o">=</span> <span class="n">output</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-597"><a href="#data_to_string-597"><span class="linenos">597</span></a>            <span class="k">if</span> <span class="n">acceptable_width</span> <span class="o">&lt;</span> <span class="n">current_width</span> <span class="o">&lt;</span> <span class="n">terminal_width</span><span class="p">:</span>
+</span><span id="data_to_string-598"><a href="#data_to_string-598"><span class="linenos">598</span></a>                <span class="n">too_wide</span> <span class="o">=</span> <span class="kc">False</span>
+</span><span id="data_to_string-599"><a href="#data_to_string-599"><span class="linenos">599</span></a>        <span class="k">if</span> <span class="n">too_wide</span><span class="p">:</span>
+</span><span id="data_to_string-600"><a href="#data_to_string-600"><span class="linenos">600</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Couldn&#39;t resize grid to fit within the terminal.&quot;</span><span class="p">)</span>
+</span><span id="data_to_string-601"><a href="#data_to_string-601"><span class="linenos">601</span></a>            <span class="k">return</span> <span class="nb">str</span><span class="p">(</span><span class="n">data</span><span class="p">)</span>
+</span><span id="data_to_string-602"><a href="#data_to_string-602"><span class="linenos">602</span></a>    <span class="k">return</span> <span class="n">output</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses tabulate to produce pretty string output from a list of dictionaries.</p>
 
 <h4 id="params">:params:</h4>
```

#### html2text {}

```diff
@@ -202,15 +202,15 @@
 164
 165        :param `table_defs`: Each definition should be in the form
 `table_name(column_definitions)`"""
 166        if len(table_defs) > 0:
 167            table_names = self.get_table_names()
 168            for table in table_defs:
 169                if table.split("(")[0].strip() not in table_names:
-170                    self.cursor.execute(f"create table {table};")
+170                    self.cursor.execute(f"create table [{table}];")
 171                    self.logger.info(f'{table.split("(")[0]} table
 created.')
 172
 173    @_connect
 174    def create_table(self, table: str, column_defs: list[str]):
 175        """Create a table if it doesn't exist.
 176
@@ -218,15 +218,15 @@
 178
 179        `table`: Name of the table to create.
 180
 181        `column_defs`: List of column definitions in proper Sqlite3 sytax.
 182        i.e. `"column_name text unique"` or `"column_name int primary key"`
 etc."""
 183        if table not in self.get_table_names():
-184            query = f"create table {table}({', '.join(column_defs)});"
+184            query = f"create table [{table}]({', '.join(column_defs)});"
 185            self.cursor.execute(query)
 186            self.logger.info(f"'{table}' table created.")
 187
 188    @_connect
 189    def get_table_names(self) -> list[str]:
 190        """Returns a list of table names from the database."""
 191        self.cursor.execute(
@@ -234,15 +234,15 @@
 not like "sqlite_%";'
 193        )
 194        return [result[0] for result in self.cursor.fetchall()]
 195
 196    @_connect
 197    def get_column_names(self, table: str) -> list[str]:
 198        """Return a list of column names from a table."""
-199        self.cursor.execute(f"select * from {table} where 1=0")
+199        self.cursor.execute(f"select * from [{table}] where 1=0;")
 200        return [description[0] for description in self.cursor.description]
 201
 202    @_connect
 203    def count(
 204        self,
 205        table: str,
 206        match_criteria: list[tuple] | dict | None = None,
@@ -257,15 +257,15 @@
 215        keys are column names and values are row values.
 216        If `None`, all rows from the table will be counted.
 217
 218        `exact_match`: If `False`, the row value for a given column
 219        in `match_criteria` will be matched as a substring.
 220        Has no effect if `match_criteria` is `None`.
 221        """
-222        query = f"select count(_rowid_) from {table}"
+222        query = f"select count(_rowid_) from [{table}]"
 223        try:
 224            if match_criteria:
 225                self.cursor.execute(
 226                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)};"
 227                )
 228            else:
@@ -295,21 +295,22 @@
 elements as `values`."""
 250        parameterizer = ", ".join("?" for _ in values)
 251        logger_values = ", ".join(str(value) for value in values)
 252        try:
 253            if columns:
 254                columns_query = ", ".join(column for column in columns)
 255                self.cursor.execute(
-256                    f"insert into {table} ({columns_query}) values(
+256                    f"insert into [{table}] ({columns_query}) values(
 {parameterizer});",
 257                    values,
 258                )
 259            else:
 260                self.cursor.execute(
-261                    f"insert into {table} values({parameterizer});", values
+261                    f"insert into [{table}] values({parameterizer});",
+values
 262                )
 263            self.logger.info(f'Added "{logger_values}" to {table} table.')
 264            return True
 265        except Exception as e:
 266            if "constraint" not in str(e).lower():
 267                self.logger.exception(
 268                    f'Error adding "{logger_values}" to {table} table.'
@@ -395,15 +396,15 @@
 339
 340        `limit`: If given, a `limit {limit}` clause will be added to the
 select query.
 341        """
 342
 343        if type(columns_to_return) is str:
 344            columns_to_return = [columns_to_return]
-345        query = f"select * from {table}"
+345        query = f"select * from [{table}]"
 346        matches = []
 347        if match_criteria:
 348            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
 349        if order_by:
 350            query += f" order by {order_by}"
 351        if limit:
@@ -473,15 +474,16 @@
 corresponding values.
 410
 411        `exact_match`: If `False`, the value for a given column will be
 matched as a substring.
 412        """
 413        conditions = self._get_conditions(match_criteria, exact_match)
 414        try:
-415            self.cursor.execute(f"delete from {table} where {conditions};")
+415            self.cursor.execute(f"delete from [{table}] where
+{conditions};")
 416            num_deletions = self.cursor.rowcount
 417            self.logger.info(
 418                f'Deleted {num_deletions} rows from "{table}" where
 {conditions}".'
 419            )
 420            return num_deletions
 421        except Exception as e:
@@ -517,15 +519,15 @@
 corresponding values.
 448        If `None`, every row in `table` will be updated.
 449
 450        `exact_match`: If `False`, `match_criteria` values will be treated
 as substrings.
 451
 452        Returns the number of updated rows."""
-453        query = f"update {table} set {column_to_update} = ?"
+453        query = f"update [{table}] set {column_to_update} = ?"
 454        conditions = ""
 455        if match_criteria:
 456            conditions = self._get_conditions(match_criteria, exact_match)
 457            query += f" where {conditions}"
 458        else:
 459            conditions = None
 460        query += ";"
@@ -549,15 +551,15 @@
 476
 477    @_connect
 478    def drop_table(self, table: str) -> bool:
 479        """Drop `table` from the database.
 480
 481        Returns `True` if successful, `False` if not."""
 482        try:
-483            self.cursor.execute(f"drop Table {table};")
+483            self.cursor.execute(f"drop Table [{table}];")
 484            self.logger.info(f'Dropped table "{table}"')
 485            return True
 486        except Exception as e:
 487            print(e)
 488            self.logger.error(f'Failed to drop table "{table}"')
 489            return False
 490
@@ -574,120 +576,121 @@
 500
 501        `_type`: The data type of the new column.
 502
 503        `default_value`: Optional default value for the column."""
 504        try:
 505            if default_value:
 506                self.cursor.execute(
-507                    f"alter table {table} add column {column} {_type}
+507                    f"alter table [{table}] add column {column} {_type}
 default {default_value};"
 508                )
 509                self.update(table, column, default_value)
 510            else:
-511                self.cursor.execute(f"alter table {table} add column
-{column} {_type};")
-512            self.logger.info(f'Added column "{column}" to "{table}" table.')
-513        except Exception as e:
-514            self.logger.error(f'Failed to add column "{column}" to "{table}"
+511                self.cursor.execute(
+512                    f"alter table [{table}] add column {column} {_type};"
+513                )
+514            self.logger.info(f'Added column "{column}" to "{table}" table.')
+515        except Exception as e:
+516            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
-515
-516    @staticmethod
-517    def data_to_string(
-518        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+517
+518    @staticmethod
+519    def data_to_string(
+520        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
 bool = True
-519    ) -> str:
-520        """Uses tabulate to produce pretty string output from a list of
+521    ) -> str:
+522        """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-521
-522        #### :params:
 523
-524        `data`: The list of dictionaries to create a grid from.
-525        Assumes all dictionaries in list have the same set of keys.
-526
-527        `sort_key`: Optional dictionary key to sort data with.
+524        #### :params:
+525
+526        `data`: The list of dictionaries to create a grid from.
+527        Assumes all dictionaries in list have the same set of keys.
 528
-529        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+529        `sort_key`: Optional dictionary key to sort data with.
+530
+531        `wrap_to_terminal`: If `True`, the table width will be wrapped to
 fit within the current terminal window.
-530        Pass as `False` if the output is going into something like a `.txt`
+532        Pass as `False` if the output is going into something like a `.txt`
 file."""
-531        return data_to_string(data, sort_key, wrap_to_terminal)
-532
-533
-534def data_to_string(
-535    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
+533        return data_to_string(data, sort_key, wrap_to_terminal)
+534
+535
+536def data_to_string(
+537    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
 True
-536) -> str:
-537    """Uses tabulate to produce pretty string output from a list of
+538) -> str:
+539    """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-538
-539    #### :params:
 540
-541    `data`: The list of dictionaries to create a grid from.
-542    Assumes all dictionaries in list have the same set of keys.
-543
-544    `sort_key`: Optional dictionary key to sort data with.
+541    #### :params:
+542
+543    `data`: The list of dictionaries to create a grid from.
+544    Assumes all dictionaries in list have the same set of keys.
 545
-546    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
+546    `sort_key`: Optional dictionary key to sort data with.
+547
+548    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
 within the current terminal window.
-547    Pass as `False` if the output is going into something like a `.txt`
+549    Pass as `False` if the output is going into something like a `.txt`
 file."""
-548    if len(data) == 0:
-549        return ""
-550    if sort_key:
-551        data = sorted(data, key=lambda d: d[sort_key])
-552    for i, d in enumerate(data):
-553        for k in d:
-554            data[i][k] = str(data[i][k])
-555
-556    too_wide = True
-557    terminal_width = os.get_terminal_size().columns
-558    max_col_widths = terminal_width
-559    # Make an output with effectively unrestricted column widths
-560    # to see if shrinking is necessary
-561    output = tabulate(
-562        data,
-563        headers="keys",
-564        disable_numparse=True,
-565        tablefmt="grid",
-566        maxcolwidths=max_col_widths,
-567    )
-568    current_width = output.index("\n")
-569    if current_width < terminal_width:
-570        too_wide = False
-571    if wrap_to_terminal and too_wide:
-572        print("Resizing grid to fit within the terminal...\n")
-573        previous_col_widths = max_col_widths
-574        acceptable_width = terminal_width - 10
-575        while too_wide and max_col_widths > 1:
-576            if current_width >= terminal_width:
-577                previous_col_widths = max_col_widths
-578                max_col_widths = int(max_col_widths * 0.5)
-579            elif current_width < terminal_width:
-580                # Without lowering acceptable_width, this condition will
+550    if len(data) == 0:
+551        return ""
+552    if sort_key:
+553        data = sorted(data, key=lambda d: d[sort_key])
+554    for i, d in enumerate(data):
+555        for k in d:
+556            data[i][k] = str(data[i][k])
+557
+558    too_wide = True
+559    terminal_width = os.get_terminal_size().columns
+560    max_col_widths = terminal_width
+561    # Make an output with effectively unrestricted column widths
+562    # to see if shrinking is necessary
+563    output = tabulate(
+564        data,
+565        headers="keys",
+566        disable_numparse=True,
+567        tablefmt="grid",
+568        maxcolwidths=max_col_widths,
+569    )
+570    current_width = output.index("\n")
+571    if current_width < terminal_width:
+572        too_wide = False
+573    if wrap_to_terminal and too_wide:
+574        print("Resizing grid to fit within the terminal...\n")
+575        previous_col_widths = max_col_widths
+576        acceptable_width = terminal_width - 10
+577        while too_wide and max_col_widths > 1:
+578            if current_width >= terminal_width:
+579                previous_col_widths = max_col_widths
+580                max_col_widths = int(max_col_widths * 0.5)
+581            elif current_width < terminal_width:
+582                # Without lowering acceptable_width, this condition will
 cause infinite loop
-581                if max_col_widths == previous_col_widths - 1:
-582                    acceptable_width -= 10
-583                max_col_widths = int(
-584                    max_col_widths + (0.5 * (previous_col_widths -
+583                if max_col_widths == previous_col_widths - 1:
+584                    acceptable_width -= 10
+585                max_col_widths = int(
+586                    max_col_widths + (0.5 * (previous_col_widths -
 max_col_widths))
-585                )
-586            output = tabulate(
-587                data,
-588                headers="keys",
-589                disable_numparse=True,
-590                tablefmt="grid",
-591                maxcolwidths=max_col_widths,
-592            )
-593            current_width = output.index("\n")
-594            if acceptable_width < current_width < terminal_width:
-595                too_wide = False
-596        if too_wide:
-597            print("Couldn't resize grid to fit within the terminal.")
-598            return str(data)
-599    return output
+587                )
+588            output = tabulate(
+589                data,
+590                headers="keys",
+591                disable_numparse=True,
+592                tablefmt="grid",
+593                maxcolwidths=max_col_widths,
+594            )
+595            current_width = output.index("\n")
+596            if acceptable_width < current_width < terminal_width:
+597                too_wide = False
+598        if too_wide:
+599            print("Couldn't resize grid to fit within the terminal.")
+600            return str(data)
+601    return output
   ⁰
 class DataBased: View Source
 _27class DataBased:
 _28    """Sqli wrapper so queries don't need to be written except table
 definitions.
 _29
 _30    Supports saving and reading dates as datetime objects.
@@ -836,15 +839,15 @@
 165
 166        :param `table_defs`: Each definition should be in the form
 `table_name(column_definitions)`"""
 167        if len(table_defs) > 0:
 168            table_names = self.get_table_names()
 169            for table in table_defs:
 170                if table.split("(")[0].strip() not in table_names:
-171                    self.cursor.execute(f"create table {table};")
+171                    self.cursor.execute(f"create table [{table}];")
 172                    self.logger.info(f'{table.split("(")[0]} table
 created.')
 173
 174    @_connect
 175    def create_table(self, table: str, column_defs: list[str]):
 176        """Create a table if it doesn't exist.
 177
@@ -852,15 +855,15 @@
 179
 180        `table`: Name of the table to create.
 181
 182        `column_defs`: List of column definitions in proper Sqlite3 sytax.
 183        i.e. `"column_name text unique"` or `"column_name int primary key"`
 etc."""
 184        if table not in self.get_table_names():
-185            query = f"create table {table}({', '.join(column_defs)});"
+185            query = f"create table [{table}]({', '.join(column_defs)});"
 186            self.cursor.execute(query)
 187            self.logger.info(f"'{table}' table created.")
 188
 189    @_connect
 190    def get_table_names(self) -> list[str]:
 191        """Returns a list of table names from the database."""
 192        self.cursor.execute(
@@ -868,15 +871,15 @@
 not like "sqlite_%";'
 194        )
 195        return [result[0] for result in self.cursor.fetchall()]
 196
 197    @_connect
 198    def get_column_names(self, table: str) -> list[str]:
 199        """Return a list of column names from a table."""
-200        self.cursor.execute(f"select * from {table} where 1=0")
+200        self.cursor.execute(f"select * from [{table}] where 1=0;")
 201        return [description[0] for description in self.cursor.description]
 202
 203    @_connect
 204    def count(
 205        self,
 206        table: str,
 207        match_criteria: list[tuple] | dict | None = None,
@@ -891,15 +894,15 @@
 216        keys are column names and values are row values.
 217        If `None`, all rows from the table will be counted.
 218
 219        `exact_match`: If `False`, the row value for a given column
 220        in `match_criteria` will be matched as a substring.
 221        Has no effect if `match_criteria` is `None`.
 222        """
-223        query = f"select count(_rowid_) from {table}"
+223        query = f"select count(_rowid_) from [{table}]"
 224        try:
 225            if match_criteria:
 226                self.cursor.execute(
 227                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)};"
 228                )
 229            else:
@@ -929,21 +932,22 @@
 elements as `values`."""
 251        parameterizer = ", ".join("?" for _ in values)
 252        logger_values = ", ".join(str(value) for value in values)
 253        try:
 254            if columns:
 255                columns_query = ", ".join(column for column in columns)
 256                self.cursor.execute(
-257                    f"insert into {table} ({columns_query}) values(
+257                    f"insert into [{table}] ({columns_query}) values(
 {parameterizer});",
 258                    values,
 259                )
 260            else:
 261                self.cursor.execute(
-262                    f"insert into {table} values({parameterizer});", values
+262                    f"insert into [{table}] values({parameterizer});",
+values
 263                )
 264            self.logger.info(f'Added "{logger_values}" to {table} table.')
 265            return True
 266        except Exception as e:
 267            if "constraint" not in str(e).lower():
 268                self.logger.exception(
 269                    f'Error adding "{logger_values}" to {table} table.'
@@ -1029,15 +1033,15 @@
 340
 341        `limit`: If given, a `limit {limit}` clause will be added to the
 select query.
 342        """
 343
 344        if type(columns_to_return) is str:
 345            columns_to_return = [columns_to_return]
-346        query = f"select * from {table}"
+346        query = f"select * from [{table}]"
 347        matches = []
 348        if match_criteria:
 349            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
 350        if order_by:
 351            query += f" order by {order_by}"
 352        if limit:
@@ -1107,15 +1111,16 @@
 corresponding values.
 411
 412        `exact_match`: If `False`, the value for a given column will be
 matched as a substring.
 413        """
 414        conditions = self._get_conditions(match_criteria, exact_match)
 415        try:
-416            self.cursor.execute(f"delete from {table} where {conditions};")
+416            self.cursor.execute(f"delete from [{table}] where
+{conditions};")
 417            num_deletions = self.cursor.rowcount
 418            self.logger.info(
 419                f'Deleted {num_deletions} rows from "{table}" where
 {conditions}".'
 420            )
 421            return num_deletions
 422        except Exception as e:
@@ -1151,15 +1156,15 @@
 corresponding values.
 449        If `None`, every row in `table` will be updated.
 450
 451        `exact_match`: If `False`, `match_criteria` values will be treated
 as substrings.
 452
 453        Returns the number of updated rows."""
-454        query = f"update {table} set {column_to_update} = ?"
+454        query = f"update [{table}] set {column_to_update} = ?"
 455        conditions = ""
 456        if match_criteria:
 457            conditions = self._get_conditions(match_criteria, exact_match)
 458            query += f" where {conditions}"
 459        else:
 460            conditions = None
 461        query += ";"
@@ -1183,15 +1188,15 @@
 477
 478    @_connect
 479    def drop_table(self, table: str) -> bool:
 480        """Drop `table` from the database.
 481
 482        Returns `True` if successful, `False` if not."""
 483        try:
-484            self.cursor.execute(f"drop Table {table};")
+484            self.cursor.execute(f"drop Table [{table}];")
 485            self.logger.info(f'Dropped table "{table}"')
 486            return True
 487        except Exception as e:
 488            print(e)
 489            self.logger.error(f'Failed to drop table "{table}"')
 490            return False
 491
@@ -1208,46 +1213,47 @@
 501
 502        `_type`: The data type of the new column.
 503
 504        `default_value`: Optional default value for the column."""
 505        try:
 506            if default_value:
 507                self.cursor.execute(
-508                    f"alter table {table} add column {column} {_type}
+508                    f"alter table [{table}] add column {column} {_type}
 default {default_value};"
 509                )
 510                self.update(table, column, default_value)
 511            else:
-512                self.cursor.execute(f"alter table {table} add column
-{column} {_type};")
-513            self.logger.info(f'Added column "{column}" to "{table}" table.')
-514        except Exception as e:
-515            self.logger.error(f'Failed to add column "{column}" to "{table}"
+512                self.cursor.execute(
+513                    f"alter table [{table}] add column {column} {_type};"
+514                )
+515            self.logger.info(f'Added column "{column}" to "{table}" table.')
+516        except Exception as e:
+517            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
-516
-517    @staticmethod
-518    def data_to_string(
-519        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+518
+519    @staticmethod
+520    def data_to_string(
+521        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
 bool = True
-520    ) -> str:
-521        """Uses tabulate to produce pretty string output from a list of
+522    ) -> str:
+523        """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-522
-523        #### :params:
 524
-525        `data`: The list of dictionaries to create a grid from.
-526        Assumes all dictionaries in list have the same set of keys.
-527
-528        `sort_key`: Optional dictionary key to sort data with.
+525        #### :params:
+526
+527        `data`: The list of dictionaries to create a grid from.
+528        Assumes all dictionaries in list have the same set of keys.
 529
-530        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+530        `sort_key`: Optional dictionary key to sort data with.
+531
+532        `wrap_to_terminal`: If `True`, the table width will be wrapped to
 fit within the current terminal window.
-531        Pass as `False` if the output is going into something like a `.txt`
+533        Pass as `False` if the output is going into something like a `.txt`
 file."""
-532        return data_to_string(data, sort_key, wrap_to_terminal)
+534        return data_to_string(data, sort_key, wrap_to_terminal)
 Sqli wrapper so queries don't need to be written except table definitions.
 Supports saving and reading dates as datetime objects.
 Supports using a context manager.
 ⁰
 DataBased(
 dbpath: str | pathier.pathier.Pathier,
 logger_encoding: str = 'utf-8',
@@ -1323,15 +1329,15 @@
 165
 166        :param `table_defs`: Each definition should be in the form
 `table_name(column_definitions)`"""
 167        if len(table_defs) > 0:
 168            table_names = self.get_table_names()
 169            for table in table_defs:
 170                if table.split("(")[0].strip() not in table_names:
-171                    self.cursor.execute(f"create table {table};")
+171                    self.cursor.execute(f"create table [{table}];")
 172                    self.logger.info(f'{table.split("(")[0]} table
 created.')
 Create tables if they don't exist.
 * Parameters *
     * table_defs: Each definition should be in the form table_name
       (column_definitions)
 ⁰
@@ -1344,15 +1350,15 @@
 179
 180        `table`: Name of the table to create.
 181
 182        `column_defs`: List of column definitions in proper Sqlite3 sytax.
 183        i.e. `"column_name text unique"` or `"column_name int primary key"`
 etc."""
 184        if table not in self.get_table_names():
-185            query = f"create table {table}({', '.join(column_defs)});"
+185            query = f"create table [{table}]({', '.join(column_defs)});"
 186            self.cursor.execute(query)
 187            self.logger.info(f"'{table}' table created.")
 Create a table if it doesn't exist.
 *** :params: ***
 table: Name of the table to create.
 column_defs: List of column definitions in proper Sqlite3 sytax. i.e.
 "column_name text unique" or "column_name int primary key" etc.
@@ -1368,15 +1374,15 @@
 195        return [result[0] for result in self.cursor.fetchall()]
 Returns a list of table names from the database.
 ⁰
 def get_column_names(self, table: str) -> list[str]: View Source
 197    @_connect
 198    def get_column_names(self, table: str) -> list[str]:
 199        """Return a list of column names from a table."""
-200        self.cursor.execute(f"select * from {table} where 1=0")
+200        self.cursor.execute(f"select * from [{table}] where 1=0;")
 201        return [description[0] for description in self.cursor.description]
 Return a list of column names from a table.
 ⁰
 def count(
 self,
 table: str,
 match_criteria: list[tuple] | dict | None = None,
@@ -1397,15 +1403,15 @@
 216        keys are column names and values are row values.
 217        If `None`, all rows from the table will be counted.
 218
 219        `exact_match`: If `False`, the row value for a given column
 220        in `match_criteria` will be matched as a substring.
 221        Has no effect if `match_criteria` is `None`.
 222        """
-223        query = f"select count(_rowid_) from {table}"
+223        query = f"select count(_rowid_) from [{table}]"
 224        try:
 225            if match_criteria:
 226                self.cursor.execute(
 227                    f"{query} where {self._get_conditions(match_criteria,
 exact_match)};"
 228                )
 229            else:
@@ -1447,21 +1453,22 @@
 elements as `values`."""
 251        parameterizer = ", ".join("?" for _ in values)
 252        logger_values = ", ".join(str(value) for value in values)
 253        try:
 254            if columns:
 255                columns_query = ", ".join(column for column in columns)
 256                self.cursor.execute(
-257                    f"insert into {table} ({columns_query}) values(
+257                    f"insert into [{table}] ({columns_query}) values(
 {parameterizer});",
 258                    values,
 259                )
 260            else:
 261                self.cursor.execute(
-262                    f"insert into {table} values({parameterizer});", values
+262                    f"insert into [{table}] values({parameterizer});",
+values
 263                )
 264            self.logger.info(f'Added "{logger_values}" to {table} table.')
 265            return True
 266        except Exception as e:
 267            if "constraint" not in str(e).lower():
 268                self.logger.exception(
 269                    f'Error adding "{logger_values}" to {table} table.'
@@ -1582,15 +1589,15 @@
 340
 341        `limit`: If given, a `limit {limit}` clause will be added to the
 select query.
 342        """
 343
 344        if type(columns_to_return) is str:
 345            columns_to_return = [columns_to_return]
-346        query = f"select * from {table}"
+346        query = f"select * from [{table}]"
 347        matches = []
 348        if match_criteria:
 349            query += f" where {self._get_conditions(match_criteria,
 exact_match)}"
 350        if order_by:
 351            query += f" order by {order_by}"
 352        if limit:
@@ -1696,15 +1703,16 @@
 corresponding values.
 411
 412        `exact_match`: If `False`, the value for a given column will be
 matched as a substring.
 413        """
 414        conditions = self._get_conditions(match_criteria, exact_match)
 415        try:
-416            self.cursor.execute(f"delete from {table} where {conditions};")
+416            self.cursor.execute(f"delete from [{table}] where
+{conditions};")
 417            num_deletions = self.cursor.rowcount
 418            self.logger.info(
 419                f'Deleted {num_deletions} rows from "{table}" where
 {conditions}".'
 420            )
 421            return num_deletions
 422        except Exception as e:
@@ -1755,15 +1763,15 @@
 corresponding values.
 449        If `None`, every row in `table` will be updated.
 450
 451        `exact_match`: If `False`, `match_criteria` values will be treated
 as substrings.
 452
 453        Returns the number of updated rows."""
-454        query = f"update {table} set {column_to_update} = ?"
+454        query = f"update [{table}] set {column_to_update} = ?"
 455        conditions = ""
 456        if match_criteria:
 457            conditions = self._get_conditions(match_criteria, exact_match)
 458            query += f" where {conditions}"
 459        else:
 460            conditions = None
 461        query += ";"
@@ -1799,15 +1807,15 @@
 def drop_table(self, table: str) -> bool: View Source
 478    @_connect
 479    def drop_table(self, table: str) -> bool:
 480        """Drop `table` from the database.
 481
 482        Returns `True` if successful, `False` if not."""
 483        try:
-484            self.cursor.execute(f"drop Table {table};")
+484            self.cursor.execute(f"drop Table [{table}];")
 485            self.logger.info(f'Dropped table "{table}"')
 486            return True
 487        except Exception as e:
 488            print(e)
 489            self.logger.error(f'Failed to drop table "{table}"')
 490            return False
 Drop table from the database.
@@ -1832,141 +1840,142 @@
 501
 502        `_type`: The data type of the new column.
 503
 504        `default_value`: Optional default value for the column."""
 505        try:
 506            if default_value:
 507                self.cursor.execute(
-508                    f"alter table {table} add column {column} {_type}
+508                    f"alter table [{table}] add column {column} {_type}
 default {default_value};"
 509                )
 510                self.update(table, column, default_value)
 511            else:
-512                self.cursor.execute(f"alter table {table} add column
-{column} {_type};")
-513            self.logger.info(f'Added column "{column}" to "{table}" table.')
-514        except Exception as e:
-515            self.logger.error(f'Failed to add column "{column}" to "{table}"
+512                self.cursor.execute(
+513                    f"alter table [{table}] add column {column} {_type};"
+514                )
+515            self.logger.info(f'Added column "{column}" to "{table}" table.')
+516        except Exception as e:
+517            self.logger.error(f'Failed to add column "{column}" to "{table}"
 table.')
 Add a new column to table.
 *** :params: ***
 column: Name of the column to add.
 _type: The data type of the new column.
 default_value: Optional default value for the column.
 ⁰
 @staticmethod
 def data_to_string(
 data: list[dict],
 sort_key: str | None = None,
 wrap_to_terminal: bool = True) -> str: View Source
-517    @staticmethod
-518    def data_to_string(
-519        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
+519    @staticmethod
+520    def data_to_string(
+521        data: list[dict], sort_key: str | None = None, wrap_to_terminal:
 bool = True
-520    ) -> str:
-521        """Uses tabulate to produce pretty string output from a list of
+522    ) -> str:
+523        """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-522
-523        #### :params:
 524
-525        `data`: The list of dictionaries to create a grid from.
-526        Assumes all dictionaries in list have the same set of keys.
-527
-528        `sort_key`: Optional dictionary key to sort data with.
+525        #### :params:
+526
+527        `data`: The list of dictionaries to create a grid from.
+528        Assumes all dictionaries in list have the same set of keys.
 529
-530        `wrap_to_terminal`: If `True`, the table width will be wrapped to
+530        `sort_key`: Optional dictionary key to sort data with.
+531
+532        `wrap_to_terminal`: If `True`, the table width will be wrapped to
 fit within the current terminal window.
-531        Pass as `False` if the output is going into something like a `.txt`
+533        Pass as `False` if the output is going into something like a `.txt`
 file."""
-532        return data_to_string(data, sort_key, wrap_to_terminal)
+534        return data_to_string(data, sort_key, wrap_to_terminal)
 Uses tabulate to produce pretty string output from a list of dictionaries.
 *** :params: ***
 data: The list of dictionaries to create a grid from. Assumes all dictionaries
 in list have the same set of keys.
 sort_key: Optional dictionary key to sort data with.
 wrap_to_terminal: If True, the table width will be wrapped to fit within the
 current terminal window. Pass as False if the output is going into something
 like a .txt file.
   ⁰
 def data_to_string(
 data: list[dict],
 sort_key: str | None = None,
 wrap_to_terminal: bool = True) -> str: View Source
-535def data_to_string(
-536    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
+537def data_to_string(
+538    data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool =
 True
-537) -> str:
-538    """Uses tabulate to produce pretty string output from a list of
+539) -> str:
+540    """Uses tabulate to produce pretty string output from a list of
 dictionaries.
-539
-540    #### :params:
 541
-542    `data`: The list of dictionaries to create a grid from.
-543    Assumes all dictionaries in list have the same set of keys.
-544
-545    `sort_key`: Optional dictionary key to sort data with.
+542    #### :params:
+543
+544    `data`: The list of dictionaries to create a grid from.
+545    Assumes all dictionaries in list have the same set of keys.
 546
-547    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
+547    `sort_key`: Optional dictionary key to sort data with.
+548
+549    `wrap_to_terminal`: If `True`, the table width will be wrapped to fit
 within the current terminal window.
-548    Pass as `False` if the output is going into something like a `.txt`
+550    Pass as `False` if the output is going into something like a `.txt`
 file."""
-549    if len(data) == 0:
-550        return ""
-551    if sort_key:
-552        data = sorted(data, key=lambda d: d[sort_key])
-553    for i, d in enumerate(data):
-554        for k in d:
-555            data[i][k] = str(data[i][k])
-556
-557    too_wide = True
-558    terminal_width = os.get_terminal_size().columns
-559    max_col_widths = terminal_width
-560    # Make an output with effectively unrestricted column widths
-561    # to see if shrinking is necessary
-562    output = tabulate(
-563        data,
-564        headers="keys",
-565        disable_numparse=True,
-566        tablefmt="grid",
-567        maxcolwidths=max_col_widths,
-568    )
-569    current_width = output.index("\n")
-570    if current_width < terminal_width:
-571        too_wide = False
-572    if wrap_to_terminal and too_wide:
-573        print("Resizing grid to fit within the terminal...\n")
-574        previous_col_widths = max_col_widths
-575        acceptable_width = terminal_width - 10
-576        while too_wide and max_col_widths > 1:
-577            if current_width >= terminal_width:
-578                previous_col_widths = max_col_widths
-579                max_col_widths = int(max_col_widths * 0.5)
-580            elif current_width < terminal_width:
-581                # Without lowering acceptable_width, this condition will
+551    if len(data) == 0:
+552        return ""
+553    if sort_key:
+554        data = sorted(data, key=lambda d: d[sort_key])
+555    for i, d in enumerate(data):
+556        for k in d:
+557            data[i][k] = str(data[i][k])
+558
+559    too_wide = True
+560    terminal_width = os.get_terminal_size().columns
+561    max_col_widths = terminal_width
+562    # Make an output with effectively unrestricted column widths
+563    # to see if shrinking is necessary
+564    output = tabulate(
+565        data,
+566        headers="keys",
+567        disable_numparse=True,
+568        tablefmt="grid",
+569        maxcolwidths=max_col_widths,
+570    )
+571    current_width = output.index("\n")
+572    if current_width < terminal_width:
+573        too_wide = False
+574    if wrap_to_terminal and too_wide:
+575        print("Resizing grid to fit within the terminal...\n")
+576        previous_col_widths = max_col_widths
+577        acceptable_width = terminal_width - 10
+578        while too_wide and max_col_widths > 1:
+579            if current_width >= terminal_width:
+580                previous_col_widths = max_col_widths
+581                max_col_widths = int(max_col_widths * 0.5)
+582            elif current_width < terminal_width:
+583                # Without lowering acceptable_width, this condition will
 cause infinite loop
-582                if max_col_widths == previous_col_widths - 1:
-583                    acceptable_width -= 10
-584                max_col_widths = int(
-585                    max_col_widths + (0.5 * (previous_col_widths -
+584                if max_col_widths == previous_col_widths - 1:
+585                    acceptable_width -= 10
+586                max_col_widths = int(
+587                    max_col_widths + (0.5 * (previous_col_widths -
 max_col_widths))
-586                )
-587            output = tabulate(
-588                data,
-589                headers="keys",
-590                disable_numparse=True,
-591                tablefmt="grid",
-592                maxcolwidths=max_col_widths,
-593            )
-594            current_width = output.index("\n")
-595            if acceptable_width < current_width < terminal_width:
-596                too_wide = False
-597        if too_wide:
-598            print("Couldn't resize grid to fit within the terminal.")
-599            return str(data)
-600    return output
+588                )
+589            output = tabulate(
+590                data,
+591                headers="keys",
+592                disable_numparse=True,
+593                tablefmt="grid",
+594                maxcolwidths=max_col_widths,
+595            )
+596            current_width = output.index("\n")
+597            if acceptable_width < current_width < terminal_width:
+598                too_wide = False
+599        if too_wide:
+600            print("Couldn't resize grid to fit within the terminal.")
+601            return str(data)
+602    return output
 Uses tabulate to produce pretty string output from a list of dictionaries.
 *** :params: ***
 data: The list of dictionaries to create a grid from. Assumes all dictionaries
 in list have the same set of keys.
 sort_key: Optional dictionary key to sort data with.
 wrap_to_terminal: If True, the table width will be wrapped to fit within the
 current terminal window. Pass as False if the output is going into something
```

### Comparing `databased-2.0.0/docs/databased/dbparsers.html` & `databased-2.0.1/docs/databased/dbparsers.html`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/docs/databased/dbshell.html` & `databased-2.0.1/docs/databased/dbshell.html`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/src/databased/customshell.py` & `databased-2.0.1/src/databased/customshell.py`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/src/databased/databased.py` & `databased-2.0.1/src/databased/databased.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,44 +163,44 @@
         """Create tables if they don't exist.
 
         :param `table_defs`: Each definition should be in the form `table_name(column_definitions)`"""
         if len(table_defs) > 0:
             table_names = self.get_table_names()
             for table in table_defs:
                 if table.split("(")[0].strip() not in table_names:
-                    self.cursor.execute(f"create table {table};")
+                    self.cursor.execute(f"create table [{table}];")
                     self.logger.info(f'{table.split("(")[0]} table created.')
 
     @_connect
     def create_table(self, table: str, column_defs: list[str]):
         """Create a table if it doesn't exist.
 
         #### :params:
 
         `table`: Name of the table to create.
 
         `column_defs`: List of column definitions in proper Sqlite3 sytax.
         i.e. `"column_name text unique"` or `"column_name int primary key"` etc."""
         if table not in self.get_table_names():
-            query = f"create table {table}({', '.join(column_defs)});"
+            query = f"create table [{table}]({', '.join(column_defs)});"
             self.cursor.execute(query)
             self.logger.info(f"'{table}' table created.")
 
     @_connect
     def get_table_names(self) -> list[str]:
         """Returns a list of table names from the database."""
         self.cursor.execute(
             'select name from sqlite_Schema where type = "table" and name not like "sqlite_%";'
         )
         return [result[0] for result in self.cursor.fetchall()]
 
     @_connect
     def get_column_names(self, table: str) -> list[str]:
         """Return a list of column names from a table."""
-        self.cursor.execute(f"select * from {table} where 1=0")
+        self.cursor.execute(f"select * from [{table}] where 1=0;")
         return [description[0] for description in self.cursor.description]
 
     @_connect
     def count(
         self,
         table: str,
         match_criteria: list[tuple] | dict | None = None,
@@ -215,15 +215,15 @@
         keys are column names and values are row values.
         If `None`, all rows from the table will be counted.
 
         `exact_match`: If `False`, the row value for a given column
         in `match_criteria` will be matched as a substring.
         Has no effect if `match_criteria` is `None`.
         """
-        query = f"select count(_rowid_) from {table}"
+        query = f"select count(_rowid_) from [{table}]"
         try:
             if match_criteria:
                 self.cursor.execute(
                     f"{query} where {self._get_conditions(match_criteria, exact_match)};"
                 )
             else:
                 self.cursor.execute(f"{query}")
@@ -249,20 +249,20 @@
         If `columns` is provided, it should contain the same number of elements as `values`."""
         parameterizer = ", ".join("?" for _ in values)
         logger_values = ", ".join(str(value) for value in values)
         try:
             if columns:
                 columns_query = ", ".join(column for column in columns)
                 self.cursor.execute(
-                    f"insert into {table} ({columns_query}) values({parameterizer});",
+                    f"insert into [{table}] ({columns_query}) values({parameterizer});",
                     values,
                 )
             else:
                 self.cursor.execute(
-                    f"insert into {table} values({parameterizer});", values
+                    f"insert into [{table}] values({parameterizer});", values
                 )
             self.logger.info(f'Added "{logger_values}" to {table} table.')
             return True
         except Exception as e:
             if "constraint" not in str(e).lower():
                 self.logger.exception(
                     f'Error adding "{logger_values}" to {table} table.'
@@ -338,15 +338,15 @@
         `order_by`: If given, a `order by {order_by}` clause will be added to the select query.
 
         `limit`: If given, a `limit {limit}` clause will be added to the select query.
         """
 
         if type(columns_to_return) is str:
             columns_to_return = [columns_to_return]
-        query = f"select * from {table}"
+        query = f"select * from [{table}]"
         matches = []
         if match_criteria:
             query += f" where {self._get_conditions(match_criteria, exact_match)}"
         if order_by:
             query += f" order by {order_by}"
         if limit:
             query += f" limit {limit}"
@@ -408,15 +408,15 @@
         `match_criteria`: Can be a list of 2-tuples where each tuple is `(column_name, value)`
         or a dictionary where keys are column names and values are corresponding values.
 
         `exact_match`: If `False`, the value for a given column will be matched as a substring.
         """
         conditions = self._get_conditions(match_criteria, exact_match)
         try:
-            self.cursor.execute(f"delete from {table} where {conditions};")
+            self.cursor.execute(f"delete from [{table}] where {conditions};")
             num_deletions = self.cursor.rowcount
             self.logger.info(
                 f'Deleted {num_deletions} rows from "{table}" where {conditions}".'
             )
             return num_deletions
         except Exception as e:
             self.logger.debug(
@@ -446,15 +446,15 @@
         `match_criteria`: Can be a list of 2-tuples where each tuple is `(columnName, rowValue)`
         or a dictionary where keys are column names and values are corresponding values.
         If `None`, every row in `table` will be updated.
 
         `exact_match`: If `False`, `match_criteria` values will be treated as substrings.
 
         Returns the number of updated rows."""
-        query = f"update {table} set {column_to_update} = ?"
+        query = f"update [{table}] set {column_to_update} = ?"
         conditions = ""
         if match_criteria:
             conditions = self._get_conditions(match_criteria, exact_match)
             query += f" where {conditions}"
         else:
             conditions = None
         query += ";"
@@ -476,15 +476,15 @@
 
     @_connect
     def drop_table(self, table: str) -> bool:
         """Drop `table` from the database.
 
         Returns `True` if successful, `False` if not."""
         try:
-            self.cursor.execute(f"drop Table {table};")
+            self.cursor.execute(f"drop Table [{table}];")
             self.logger.info(f'Dropped table "{table}"')
             return True
         except Exception as e:
             print(e)
             self.logger.error(f'Failed to drop table "{table}"')
             return False
 
@@ -500,19 +500,21 @@
 
         `_type`: The data type of the new column.
 
         `default_value`: Optional default value for the column."""
         try:
             if default_value:
                 self.cursor.execute(
-                    f"alter table {table} add column {column} {_type} default {default_value};"
+                    f"alter table [{table}] add column {column} {_type} default {default_value};"
                 )
                 self.update(table, column, default_value)
             else:
-                self.cursor.execute(f"alter table {table} add column {column} {_type};")
+                self.cursor.execute(
+                    f"alter table [{table}] add column {column} {_type};"
+                )
             self.logger.info(f'Added column "{column}" to "{table}" table.')
         except Exception as e:
             self.logger.error(f'Failed to add column "{column}" to "{table}" table.')
 
     @staticmethod
     def data_to_string(
         data: list[dict], sort_key: str | None = None, wrap_to_terminal: bool = True
```

### Comparing `databased-2.0.0/src/databased/dbparsers.py` & `databased-2.0.1/src/databased/dbparsers.py`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/src/databased/dbshell.py` & `databased-2.0.1/src/databased/dbshell.py`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/LICENSE.txt` & `databased-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/README.md` & `databased-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `databased-2.0.0/pyproject.toml` & `databased-2.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "databased"
 authors = [{name="Matt Manes"}]
 description = "Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier."
-version = "2.0.0"
+version = "2.0.1"
 requires-python = ">=3.10"
 dependencies = ["pandas", "tabulate", "pytest", "argshell", "pathier"]
 readme = "README.md"
 keywords = [
     "database",
     "sqlite",
     "sqlite3"
```

### Comparing `databased-2.0.0/PKG-INFO` & `databased-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databased
-Version: 2.0.0
+Version: 2.0.1
 Summary: Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier.
 Project-URL: Homepage, https://github.com/matt-manes/databased
 Project-URL: Documentation, https://github.com/matt-manes/databased/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/databased/tree/main/src/databased
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: database,sqlite,sqlite3
```

