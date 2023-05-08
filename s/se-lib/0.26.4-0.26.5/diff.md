# Comparing `tmp/se_lib-0.26.4.tar.gz` & `tmp/se_lib-0.26.5.tar.gz`

## Comparing `se_lib-0.26.4.tar` & `se_lib-0.26.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.4/.DS_Store
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.4/.gitattributes
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.4/selib/.DS_Store
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 se_lib-0.26.4/selib/__init__.py
--rw-r--r--   0        0        0    74890 2020-02-02 00:00:00.000000 se_lib-0.26.4/selib/selib.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.26.4/LICENSE
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.4/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 se_lib-0.26.4/pyproject.toml
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 se_lib-0.26.4/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.26.5/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.26.5/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.26.5/selib/.DS_Store
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 se_lib-0.26.5/selib/__init__.py
+-rw-r--r--   0        0        0    77332 2020-02-02 00:00:00.000000 se_lib-0.26.5/selib/selib.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 se_lib-0.26.5/LICENSE
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 se_lib-0.26.5/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 se_lib-0.26.5/pyproject.toml
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 se_lib-0.26.5/PKG-INFO
```

### Comparing `se_lib-0.26.4/.DS_Store` & `se_lib-0.26.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.4/selib/.DS_Store` & `se_lib-0.26.5/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.26.4/selib/selib.py` & `se_lib-0.26.5/selib/selib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-se-lib Version .26.4
+se-lib Version .26.5
 
 Copyright (c) 2022-2023 Ray Madachy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
@@ -13,20 +13,26 @@
 import graphviz
 import textwrap
 import os
 import sys
 from os.path import exists
 import pandas as pd
 import matplotlib.pyplot as plt
+import matplotlib as mpl
+mpl.rcParams['axes.spines.top'] = False
+mpl.rcParams['axes.spines.right'] = False
+
 from copy import deepcopy
 
 import simpy
 import random
 import numpy as np
 
+online = False
+
 # text for SVG included files
 
 actor_svg = """<?xml version="1.0" encoding="UTF-8" standalone="no"?>
 <svg
    xmlns:dc="http://purl.org/dc/elements/1.1/"
    xmlns:cc="http://creativecommons.org/ns#"
    xmlns:rdf="http://www.w3.org/1999/02/22-rdf-syntax-ns#"
@@ -119,22 +125,33 @@
     def wrap(text): return textwrap.fill(
         text, width=wrap_width, break_long_words=False)
     node_attr = {'color': 'black', 'fontsize': '11', 'fontname': 'arial',
                  'shape': 'box'}  # 'fontname': 'arial',
     c = graphviz.Graph('G', node_attr=node_attr,
                        filename=filename, format=format, engine=engine)
 
-    human_actor_keywords = ["User", "user", "Customer", "customer", "Operator", "Patient", "Doctor", "operator"]
+    human_actor_keywords = ["user", "student", "instructor", "customer", "patient", "doctor", "operator", 'citizen', 'criminal', 'enforcer', 'legislator']
 
     for external_system in external_systems:
-        if (external_system in human_actor_keywords): c.node(wrap(external_system), labelloc="b", image='actor.svg', shape='none')
-        c.edge(wrap(system), wrap(external_system), len="1.2") # len="1.2"
+        if (type(external_system) is not tuple and external_system.casefold() in human_actor_keywords):
+            c.node(wrap(external_system), label=f'''<<font point-size="30">🧍</font>{'<br/>' if online == False else '&lt;br/&gt;'}<font point-size="11">{external_system}</font>>''', labelloc="b", shape='plain')
+            c.edge(wrap(system), wrap(external_system), len="1.2") # len="1.2"
+        elif (type(external_system) is tuple):
+            c.node(wrap(external_system[0]), label=f'''<<font point-size="30">{external_system[1]}</font>{'<br/>' if online == False else '&lt;br/&gt;'}<font point-size="11">{external_system[0]}   </font>>''', labelloc="b", shape='plain')
+            c.edge(wrap(system), wrap(external_system[0]), len="1.2") # len="1.2"
+        else:
+            c.edge(wrap(system), wrap(external_system), len="1.2") # len="1.2"
+            
     if filename is not None:
         c.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
-    return c
+    if online:
+        svg = return_svg_from_dot(str(c), engine)
+        print(svg)
+    else:
+        return c
 
 
 def activity_diagram(element_dependencies, filename=None, format='svg'):
     node_attr = {'color': 'black', 'fontsize': '11',
                  'style': "rounded", 'shape': 'box'}  # 'fontname': 'arial',
     edge_attr = {'arrowsize': '.5', 'fontname': 'arial', 'fontsize': '11', }
     activity = graphviz.Digraph('G', filename=filename, node_attr=node_attr,
@@ -192,28 +209,29 @@
         a.write(actor_svg)
         a.close()
 
     column = -2
     for number, actor in enumerate(actors):
         division = system_height / (len(actors) + 1)
         #print (division)
-        u.node(wrap(actor), pos=f'{column}, {system_height - division*(number+1) + .25}!',
-               width='.1', shape='none', image='actor.svg', labelloc='b')
+        u.node(wrap(actor), label=f'''<<font point-size="30">🧍</font><br/><font point-size="11">{actor}</font>>''', pos=f'{column}, {system_height - division*(number+1) + .25}!',
+               width='.1', shape='none', labelloc='b')
 
     column = 0
     for number, use_case in enumerate(use_cases):
         u.node(
             wrap(use_case), pos=f'{column}, {len(use_cases)-number}!', width='1.25', height=".7")
 
     for edge in (interactions):
         u.edge(wrap(edge[0]), wrap(edge[1]))  # lhead='clusterx' not used
 
     if filename != None:
         u.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
         #os.remove(filename) also doesn't work on windows "permission denied"
+    # print(str(u)) # for dot text
     return u
 
 
 def sequence_diagram(system_name, actors, objects, actions, filename=None, format='svg'):
     """ Returns a sequence diagram.
 
     Parameters
@@ -1532,20 +1550,27 @@
 
   Parameters
   ----------
   variables: variable name or list of variable names to plot on graph
   filename: file name with format extension
   """
   for var in outputs:
-    #print(var)
-    fig, axis = plt.subplots()
-    axis.set(xlabel='Time', ylabel=var)
-    axis.plot(output.index, output[var].values, label=var)
-    axis.legend(loc="best", )
-    #plot.show()
+    label_string=str(var)
+    if type(var) == list:
+        label_string=str(var[0])
+        for count, element in enumerate(var):
+            if count > 0: label_string += ", "+element
+    fig, axis = plt.subplots(figsize=(6, 4))
+    label_string = textwrap.fill(label_string, width=40)
+    axis.set(xlabel='Time', ylabel=label_string)
+    if type(var) == list:
+        axis.plot(output.index, output[var].values, label=var)
+        axis.legend(loc="best", )
+    else: 
+        axis.plot(output.index, output[var].values)
     plt.savefig(filename)
             
 def run_model(verbose=True):
 	"""
 	Executes the current model
     
 	Returns
@@ -1672,14 +1697,15 @@
     if model_type == "continuous": return(draw_sd_model(filename, format))
     if model_type == "discrete": return(draw_discrete_model_diagram(filename, format, engine='dot'))	
 	
 # Discrete Event Modeling 
 
 # define network dictionary of dictionaries
 network = {}
+
 run_specs = {}
 entity_num = 0
 entity_data = {}
 
 verbose = True
 
 
@@ -1710,16 +1736,20 @@
     capacity: integer
     	The number of resource usage slots in the server
     """
     network[name] = {
         'type': 'server',
         'resource': simpy.Resource(env, capacity=capacity),
         'connections': connections,
-        'service_time': str(service_time),
-        'waiting_times': []
+        'service_time': service_time,
+        'waiting_times': [],
+        'service_times': [],
+        'capacity': capacity,
+        'resource_busy_time': 0,
+        'resource_utilization': 0
     }
 
 
 def add_delay(name, connections, delay_time):
     """
     Add a delay to a discrete event model. 
 
@@ -1735,113 +1765,111 @@
     network[name] = {
         'type': 'delay',
         'connections': connections,
         'delay_time': delay_time,
     }
 
 
-def add_source(name, connections, num_entities, interarrival_time):
+def add_source(name, entity_name, num_entities, connections, interarrival_time):
     """
     Add a source node to a discrete event model to generate entities. 
 
     Parameters
     ----------
     name: string
-    	A name for the the source.
+    	A name for the source.
+    entity_name: string
+    	A name for the type of entity being generated.
+    num_entities: integer
+    	Number of entities to generated.
     connections: dictionary
     	A dictionary of the node connections after the source.  The node names are the keys and the values are the relative probabilities of traversing the connections.
-    num_entities: integer
-    	Number of entities to be generated.
-    interarrival_time: float
-    	The time between entity arrrivals into the system.  May be a constant or random function.
+    interarrival_time: string
+    	The time between entity arrrivals into the system.  The string may enclose a constant, random function or logical expression to be evaluated.
     """
 
     network[name] = {
         'type': 'source',
+        'entity_name': entity_name,
+        'num_entities': num_entities,
         'connections': connections,
         'interarrival_time': interarrival_time,
+        'arrivals': []
     }
     run_specs['interarrival_time'] = interarrival_time
     run_specs['num_entities'] = num_entities
+    run_specs['entity_name'] = entity_name
     run_specs['source'] = name
 
 
 def add_terminate(name):
     """
     Add a terminate node to a discrete event model for entities leaving the system. 
 
     Parameters
     ----------
     name: string
     	A name for the terminate.
     """
-    network[name] = {'type': 'terminate', 'connections': {}}
+    network[name] = {
+        'type': 'terminate', 
+        'connections': {}}
 
 
 # define processes for each entity
-def process_initial_arrival(env, arrival_time, node_name, entity_num):
+def process_initial_arrival(env, arrival_time, node_name, entity_num, entity_name):
     yield env.timeout(arrival_time)
-    if verbose: print(f"{env.now}: entity {entity_num} entered from {run_specs['source']}")
-    env.process(process_node(
-        env,
-        node_name,
-        entity_num,
-    ))
-
+    print(f"{env.now}: {entity_name} {entity_num} entered from {run_specs['source']}")
+    env.process(process_node(env, node_name, entity_num, entity_name))
 
     # define processes for each node
-def process_node(
-    env,
-    node_name,
-    entity_num,
-):
+def process_node(env, node_name, entity_num, entity_name):
     # process resource usage
 
     if network[node_name]['type'] == 'delay':
-        if verbose: print(f"{env.now}: *** delay entity {entity_num} delay_time")
-        yield env.timeout(network[node_name]['delay_time'])
+        delay_time = eval(network[node_name]['delay_time'])
+        yield env.timeout(delay_time)
+        print(f"{env.now}: {entity_name} {entity_num} delayed {delay_time} at {node_name}")
         entity_data[entity_num]['nodes'].append((node_name, env.now))
 
+
     if network[node_name]['type'] == 'server':
         with network[node_name]['resource'].request() as req:
-            #if verbose: print(network[node_name]['service_time'])
-            if verbose: print(
-                f"{env.now}: entity {entity_num} requesting {node_name} resource "
-            )
+            print(f"{env.now}: {entity_name} {entity_num} requesting {node_name} resource ")
             this_arrival_time = env.now
             #entity_data[entity_num]['nodes'].append((node_name, env.now))
             yield req
 
             waiting_time = env.now - this_arrival_time
             # collect waiting times
             network[node_name]['waiting_times'].append(waiting_time)
-            if verbose: print(
-                f"{env.now}: entity {entity_num} granted {node_name} resource waiting time {waiting_time}"
-            )
+            print(f"{env.now}: {entity_name} {entity_num} granted {node_name} resource waiting time {waiting_time}")
             service_time = eval(network[node_name]['service_time'])
             yield env.timeout(service_time)
+
+            # collect service times
+            network[node_name]['service_times'].append(service_time)
             entity_data[entity_num]['nodes'].append((node_name, env.now))
-            if verbose: print(
-                f"{env.now}: entity {entity_num} completed using {node_name} resource with service time {service_time}"
-            )
+            network[node_name]['resource_busy_time'] += service_time
+            network[node_name]['resource_utilization'] = network[node_name]['resource_busy_time']/env.now/network[node_name]['capacity'] 
+            print(f"{env.now}: {entity_name} {entity_num} completed using {node_name} resource with service time {service_time}")
 
-    # process arrivals and connections
+    if network[node_name]['type'] == 'terminate':
+        print(f"{env.now}: {entity_name} {entity_num} leaving system at {node_name} ")
+        entity_data[entity_num]['nodes'].append((node_name, env.now))
+
+
+            # process arrivals and connections
     if len(network[node_name]['connections']) > 0:
         weights = tuple(network[node_name]['connections'].values())
-        #if verbose: print(weights)
-        connection, probability = random.choice(
-            list(network[node_name]['connections'].items()))
-        connection = random.choices(list(
-            network[node_name]['connections'].keys()),
-                                    weights,
-                                    k=1)[0]
-        if verbose: print(
-            f"{env.now}: entity {entity_num} {node_name} -> {connection} (probability={probability})"
-        )
-        env.process(process_node(env, connection, entity_num))
+        #print(weights)
+        connection, probability = random.choice(list(network[node_name]['connections'].items()))
+        connection = random.choices(list(network[node_name]['connections'].keys()), weights, k=1)[0]
+        print(f"{env.now}: {entity_name} {entity_num} {node_name} -> {connection}")
+        env.process(process_node(env, connection, entity_num, entity_name))
 
 
 def run_de_model(verbose=True):
     """
     Executes the current model
     
     Returns:
@@ -1852,21 +1880,22 @@
     verbose = verbose
     for key, value in network.items():
         if value.get('type') == 'source':
             source_name = key
     arrival_time = 0
     for entity_num in range(run_specs['num_entities']):
         #yield env.timeout(1)
-        arrival_time += run_specs['interarrival_time']
+        arrival_time += eval(run_specs['interarrival_time'])
+        network[source_name]['arrivals'].append(arrival_time)
         entity_num += 1
 
         entity_data[entity_num] = {'arrival': arrival_time, 'nodes': []}
         env.process(
             process_initial_arrival(env, arrival_time, source_name,
-                                    entity_num))  #+str(entity)
+                                    entity_num, run_specs['entity_name']))  #+str(entity)
 
     # start simulation at first node
     #env.process(process_node(env, 'node1'))
     env.run()
     return network, entity_data
 
 
@@ -1897,8 +1926,18 @@
             graph.edge(
                 node_name,
                 connection,
             )
     if filename is not None:
         graph.render(
         )  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
-    return graph
+    return graph
+    
+def plot_histogram(data, xlabel= "Data"):
+    kwargs = {'color': 'blue', 'rwidth': 0.9}
+    fig, ax = plt.subplots(figsize=(5, 3))
+    ax.hist(data, **kwargs)
+    ax.set(xlabel=xlabel, ylabel='Frequency')
+    ax.xaxis.labelmargin = -50
+    ax.yaxis.labelmargin = 30
+    plt.subplots_adjust(bottom=0.15,)
+    return fig
```

### Comparing `se_lib-0.26.4/LICENSE` & `se_lib-0.26.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-se-lib Version .2
+se-lib Version .26.5
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.26.4/README.md` & `se_lib-0.26.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Systems Engineering Library (se-lib)
-Version .26.4
+Version .26.5
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.26.4/pyproject.toml` & `se_lib-0.26.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "se-lib"
-version = "0.26.4"
+version = "0.26.5"
 authors = [
   { name="se-lib Development Team", email="info@se-lib.org" },
 ]
 description = "Systems Engineering Library (se-lib)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `se_lib-0.26.4/PKG-INFO` & `se_lib-0.26.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.26.4
+Version: 0.26.5
 Summary: Systems Engineering Library (se-lib)
 Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: netcdf4
 Requires-Dist: pandas
 Requires-Dist: pysd
 Description-Content-Type: text/markdown
 
 # Systems Engineering Library (se-lib)
-Version .26.4
+Version .26.5
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

