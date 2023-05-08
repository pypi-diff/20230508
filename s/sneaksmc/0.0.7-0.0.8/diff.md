# Comparing `tmp/sneaksmc-0.0.7.tar.gz` & `tmp/sneaksmc-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneaksmc-0.0.7.tar", last modified: Sat Apr 29 14:48:22 2023, max compression
+gzip compressed data, was "sneaksmc-0.0.8.tar", last modified: Mon May  8 13:20:13 2023, max compression
```

## Comparing `sneaksmc-0.0.7.tar` & `sneaksmc-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       79 2023-04-11 13:58:02.000000 sneaksmc-0.0.7/README.rst
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/setup.cfg
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-29 14:46:26.000000 sneaksmc-0.0.7/setup.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/sneaksmc/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.7/sneaksmc/__init__.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     3665 2023-04-29 12:46:43.000000 sneaksmc-0.0.7/sneaksmc/client.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.7/sneaksmc/crypt.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)    25039 2023-04-29 14:15:29.000000 sneaksmc-0.0.7/sneaksmc/server.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/sneaksmc.egg-info/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/SOURCES.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/dependency_links.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/requires.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/top_level.txt
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-05-08 13:20:13.475215 sneaksmc-0.0.8/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-05-08 13:20:13.475215 sneaksmc-0.0.8/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       79 2023-04-11 13:58:02.000000 sneaksmc-0.0.8/README.rst
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-05-08 13:20:13.475215 sneaksmc-0.0.8/setup.cfg
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-05-08 13:19:30.000000 sneaksmc-0.0.8/setup.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-05-08 13:20:13.475215 sneaksmc-0.0.8/sneaksmc/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.8/sneaksmc/__init__.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     4170 2023-05-08 11:55:43.000000 sneaksmc-0.0.8/sneaksmc/client.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.8/sneaksmc/crypt.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)    24906 2023-05-08 13:16:23.000000 sneaksmc-0.0.8/sneaksmc/server.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-05-08 13:20:13.475215 sneaksmc-0.0.8/sneaksmc.egg-info/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-05-08 13:20:13.000000 sneaksmc-0.0.8/sneaksmc.egg-info/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-05-08 13:20:13.000000 sneaksmc-0.0.8/sneaksmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-05-08 13:20:13.000000 sneaksmc-0.0.8/sneaksmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-05-08 13:20:13.000000 sneaksmc-0.0.8/sneaksmc.egg-info/requires.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-05-08 13:20:13.000000 sneaksmc-0.0.8/sneaksmc.egg-info/top_level.txt
```

### Comparing `sneaksmc-0.0.7/sneaksmc/client.py` & `sneaksmc-0.0.8/sneaksmc/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 
 class Client():
     """ Client class to request and communicate with a sneaksmc coordinator. """
     def __init__(self) -> None:
         self.ck = Crypt()
         self.coordinator_node = None
     
-    def request_analysis(self, coordinator_node):
+    def request_analysis(self, coordinator_node, data=""):
         """ Sends a request to start an analysis operation to the given coordinator address node.
             Returns (response-code, response-msg) tuple from coordinator node. Raises exception on error. """
         self.coordinator_node = coordinator_node
-        pub_key = Crypt.key2string(self.ck.get_public_key())
+        #pub_key = Crypt.key2string(self.ck.get_public_key())
 
         # Send start analysis request to the coordinator node.
         # If the node is not coordinator then the request is dropped.
         # Sends its public key as the result will be encrypted
-        r = send_client_request(type="GET", url="/start_analysis", body=pub_key, 
+        r = send_client_request(type="GET", url="/start_analysis", body=data, 
                                     receiver=self.coordinator_node, timeout=3.0)
         return r
         
     
     def get_result(self, id, tries=100, ms=50):
         """ Sends http request to coordinator node for the result of a requested analysis operation.
             Returns the result (if received) (response-code, response-msg) tuple, otherwise if not received, 
@@ -79,10 +79,16 @@
                 # Server done processing request
                 break
             
             time.sleep(0.001*ms)
         
         return (response_code, response_msg)
     
-    def shutdown(self):
-        # TODO: ask to shutdown all smc servers
-        pass
+    def shutdown(self, node=None):
+        """ Shutdown given node (or entire SMC network if coordinator node is given).
+            If node=None then tries to shut down coordinator from last analysis request sent."""
+        if node == None:
+            # Try shut down last (request_analysis) request sent
+            if self.coordinator_node == None:
+                raise Exception("No SMC request has been initialized, or no node was given (ip:port format)")
+            node = self.coordinator_node
+        return send_client_request(type="GET", url="/shutdown",receiver=node)
```

### Comparing `sneaksmc-0.0.7/sneaksmc/crypt.py` & `sneaksmc-0.0.8/sneaksmc/crypt.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.7/sneaksmc/server.py` & `sneaksmc-0.0.8/sneaksmc/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _request_timeout_sec = 3
 
 # Offset that the coordinator sets on result to make sure no other nodes can read it.
 _operations = None
 
 
 def get_scramble():
+    """ Returns a random scramble value. """
     return random.randint(-1000000, 1000000)
 
 def get_machine_info():
     """ Returns machine host name and public ip. If no public ip is found 
         then returns ip as localhost (127.0.0.1)"""
 
     import socket
@@ -55,14 +56,17 @@
     finally:
         s.close()
     
     return socket.gethostname(), ip
 
 
 class Operation():
+    """ Operation class that stores operations done in an SMC network (on coordinator only).
+        Stores all unique scrambles (by every node) for every unique operation.
+        Stores the result when the operation has completed (and coordinator has received the result). """
     def __init__(self):
         self.operations = {}
         self.id = 0
     def _get_id(self):
         # Returns a new valid operation id > 0
         self.id += 1
         return self.id
@@ -76,32 +80,33 @@
         # Removes id from dictionary if remove=True
         return self.operations.pop(int(id), None) if remove == True else self.operations.get(int(id), None)
     def set_result(self, id, result):
         # Sets the result for given operation id
         x = self.get(int(id), False)
         x[1] = result
     def get_result(self, id):
-        # Returns result or None if result has not been set yet
+        # Returns result or None if result has not been set yet for given operation id.
         x = self.get(int(id), False)
         scramble_list = x[0]
         result = x[1]
         if result == None:
             return None
         for scramble in scramble_list:
             result -= scramble
         
-        # Remove result from dict
+        # Remove this result from container of all stored operations.
         self.operations.pop(int(id))
         return result
 
 
 
-def analysis(sum_data):
-    """ Function to be overridden by user. Param @sum_data gives previous sum data and this function must return the new sum data after the analysis is complete.
-        @sum_data will be None if it has not been previously set (first time).
+def analysis(sum_data, input_data):
+    """ Function to be overridden by user. Param @sum_data gives previous sum data and 
+        this function must return the new sum data after the analysis is complete.
+        @input_data contains input given by the user who requested this analysis.
     """
     return 1 if sum_data is None else sum_data + 10
 
 
 
 def run_server(coordinator=None, analysis_function=None, nodefile=None, ip=None, 
                 port=None, timeout=None, request_timout=None, min_nodes=1):
@@ -226,19 +231,19 @@
         print("Request invalid..")
         # Set path to invalid url to handle specific invalid certificate case
         self.path = "/invalid-certificate"
         return certificate, decrypted_msg
         
 
     def validate_certificate(self, certificate):
-        # TODO:
         print("Validating ceritificate")
         return True
     
     def handle_invalid_certificate(self, certificate=None, decrypted_msg=None):
+        # Handle an invalid certificate.
         pass
 
     def get_node_ips(own_ip, own_port):
         """ Reads nodefile which contains all node information in the system and returns a list of their ips ["ip:port", public-key].
             Public-key is null on instantiation. Ignores its own ip:port. 
 
             Only coordinator will have the nodefile and is able to know about other nodes in the network on initialization.
@@ -384,15 +389,14 @@
         encrypted_msg = data[cert_size:]
 
         return ck.decrypt(certificate), ck.decrypt(encrypted_msg)
 
 
     def do_PUT(self):
         msg = self.validate_request()
-        # TODO: request from coordinator -> nodes to save all node data of other nodes.
 
         if self.path.startswith("/invalid-certificate"):
             certificate, decrypted_msg = msg
             self.handle_invalid_certificate(certificate, decrypted_msg)
 
         
         self.send_whole_response(200, "ok")
@@ -442,19 +446,19 @@
             if not self.validate_certificate(certificate):
                 self.handle_invalid_certificate(certificate)
                 return
 
             print("msg received: " + sendto_ip)
 
             # Perform the analysis function on this nodes data and update the analysis value 'data' in the dictionary.
-            dict['data'] = _analysis_function(dict['data']) + scramble
+            dict['data'] = _analysis_function(dict['data'], dict['input']) + scramble
 
             # Dump the dictionary back to string in order to send it over the internet to the next node.
             s = json.dumps(dict)
-            print(s)
+            #print(s)
 
             # Further the result
             # send /analysis_done url if next node is the coordinator, otherwise send /analysis
             url = "/analysis_done" if sendto_ip == _server_coordinator_addr else "/analysis"
             self.send_encrypted_msg(s, url=url, ip=sendto_ip)
 
 
@@ -473,22 +477,14 @@
         if self.path.startswith("/invalid-certificate"):
             self.handle_invalid_certificate()
 
         elif self.path.startswith("/get_public_key"):
             s = Crypt.key2string(ck.get_public_key())
             self.send_whole_response(200, s)
         
-        elif self.path.startswith("/send_test"):
-            #content_len = int(self.headers.get('Content-Length'))
-            print(_server_connected_ips)
-            self.send_encrypted_msg("0")
-            self.send_whole_response(200, "ok")
-        
-
-        # Shutdown
         elif self.path.startswith("/shutdown"):
             self.send_whole_response(200, "ok")
             self.server.shutdown()
             exit(0)
         
         elif self.path.startswith("/get_result"):
             """ Client request the result from coordinator. """
@@ -510,40 +506,36 @@
 
         
         elif self.path.startswith("/certificate"):
             # Only non coordinator node should get this request
             # If this node is the coordinator then raise an exception
             if _server_iscoordinator:
                 raise Exception("Coordinator node should not receive a certificate request from other nodes.")
-            
-            # receive_ip = self.client_address[0]
-            # if not ip_whitelisted(receive_ip):
-            #     raise Exception("Connected node %s is not whitelisted within nodefile for coordinator" % str(self.client_address))
 
             self.send_whole_response(200, self.get_certificate())
            
         
         elif self.path.startswith("/start_analysis"):
             """ Start analysis request. Only coordinator will receive this request from a client. """
 
             if not _server_iscoordinator:
                 self.send_whole_response(404, "Only coordinator should get a start_analysis request")
                 return
 
 
             content_length = int(self.headers.get('content-length', 0))
-            value = self.rfile.read(content_length).decode()
+            input_data = self.rfile.read(content_length).decode()
 
             # Send a dictionary containing encrypted list of receivers (send_list)
             # and some analysis data sum (data) which is initialized with a given offset such that no node can know the current data sum.
             enc = []
             scramble_list = []
             operation_id = _operations.add(scramble_list)
 
-            enc_dict = {'send_list': enc, 'data': 0, 'id': operation_id}
+            enc_dict = {'send_list': enc, 'data': 0, 'id': operation_id, 'input': input_data}
 
             # Create sequence list of nodes to perform analysis of its data
             # This is such that the nodes know which node to forward the data to.
 
             # Add all nodes from certificate-file into a list with address and their public key
             node_list = []
             with open(certificate_file, "r") as f:
```

