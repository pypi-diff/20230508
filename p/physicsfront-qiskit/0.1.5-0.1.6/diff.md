# Comparing `tmp/physicsfront-qiskit-0.1.5.tar.gz` & `tmp/physicsfront-qiskit-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicsfront-qiskit-0.1.5.tar", last modified: Mon Feb  6 01:05:18 2023, max compression
+gzip compressed data, was "physicsfront-qiskit-0.1.6.tar", last modified: Mon May  8 19:27:11 2023, max compression
```

## Comparing `physicsfront-qiskit-0.1.5.tar` & `physicsfront-qiskit-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-02-06 01:05:18.440329 physicsfront-qiskit-0.1.5/
--rw-rw-r--   0 gweon     (1000) gweon     (1000)    11357 2023-01-14 17:25:03.000000 physicsfront-qiskit-0.1.5/LICENSE
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     1287 2023-02-06 01:05:18.440329 physicsfront-qiskit-0.1.5/PKG-INFO
--rw-rw-r--   0 gweon     (1000) gweon     (1000)      452 2023-01-30 19:55:11.000000 physicsfront-qiskit-0.1.5/README.md
-drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-02-06 01:05:18.440329 physicsfront-qiskit-0.1.5/physicsfront/
-drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-02-06 01:05:18.440329 physicsfront-qiskit-0.1.5/physicsfront/qiskit/
--rw-rw-r--   0 gweon     (1000) gweon     (1000)    30609 2023-02-05 18:51:54.000000 physicsfront-qiskit-0.1.5/physicsfront/qiskit/__init__.py
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     7705 2023-01-27 19:09:37.000000 physicsfront-qiskit-0.1.5/physicsfront/qiskit/colab.py
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     5774 2023-01-30 01:36:22.000000 physicsfront-qiskit-0.1.5/physicsfront/qiskit/patch.py
-drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-02-06 01:05:18.440329 physicsfront-qiskit-0.1.5/physicsfront_qiskit.egg-info/
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     1287 2023-02-06 01:05:18.000000 physicsfront-qiskit-0.1.5/physicsfront_qiskit.egg-info/PKG-INFO
--rw-rw-r--   0 gweon     (1000) gweon     (1000)      382 2023-02-06 01:05:18.000000 physicsfront-qiskit-0.1.5/physicsfront_qiskit.egg-info/SOURCES.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)        1 2023-02-06 01:05:18.000000 physicsfront-qiskit-0.1.5/physicsfront_qiskit.egg-info/dependency_links.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)       13 2023-02-06 01:05:18.000000 physicsfront-qiskit-0.1.5/physicsfront_qiskit.egg-info/namespace_packages.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)      100 2023-02-06 01:05:18.000000 physicsfront-qiskit-0.1.5/physicsfront_qiskit.egg-info/requires.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)       13 2023-02-06 01:05:18.000000 physicsfront-qiskit-0.1.5/physicsfront_qiskit.egg-info/top_level.txt
--rw-rw-r--   0 gweon     (1000) gweon     (1000)       38 2023-02-06 01:05:18.440329 physicsfront-qiskit-0.1.5/setup.cfg
--rw-rw-r--   0 gweon     (1000) gweon     (1000)     4124 2023-02-06 01:04:08.000000 physicsfront-qiskit-0.1.5/setup.py
+drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-08 19:27:11.825553 physicsfront-qiskit-0.1.6/
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)    11357 2023-01-14 17:25:03.000000 physicsfront-qiskit-0.1.6/LICENSE
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     1257 2023-05-08 19:27:11.825553 physicsfront-qiskit-0.1.6/PKG-INFO
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)      452 2023-01-30 19:55:11.000000 physicsfront-qiskit-0.1.6/README.md
+drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-08 19:27:11.821553 physicsfront-qiskit-0.1.6/physicsfront/
+drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-08 19:27:11.825553 physicsfront-qiskit-0.1.6/physicsfront/qiskit/
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)    36178 2023-05-08 18:47:42.000000 physicsfront-qiskit-0.1.6/physicsfront/qiskit/__init__.py
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)      975 2023-05-06 19:09:30.000000 physicsfront-qiskit-0.1.6/physicsfront/qiskit/_requires.py
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     8876 2023-05-08 01:17:14.000000 physicsfront-qiskit-0.1.6/physicsfront/qiskit/colab.py
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     5774 2023-01-30 01:36:22.000000 physicsfront-qiskit-0.1.6/physicsfront/qiskit/patch.py
+drwxrwxr-x   0 gweon     (1000) gweon     (1000)        0 2023-05-08 19:27:11.825553 physicsfront-qiskit-0.1.6/physicsfront_qiskit.egg-info/
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     1257 2023-05-08 19:27:11.000000 physicsfront-qiskit-0.1.6/physicsfront_qiskit.egg-info/PKG-INFO
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)      363 2023-05-08 19:27:11.000000 physicsfront-qiskit-0.1.6/physicsfront_qiskit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)        1 2023-05-08 19:27:11.000000 physicsfront-qiskit-0.1.6/physicsfront_qiskit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)       84 2023-05-08 19:27:11.000000 physicsfront-qiskit-0.1.6/physicsfront_qiskit.egg-info/requires.txt
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)       13 2023-05-08 19:27:11.000000 physicsfront-qiskit-0.1.6/physicsfront_qiskit.egg-info/top_level.txt
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)       38 2023-05-08 19:27:11.825553 physicsfront-qiskit-0.1.6/setup.cfg
+-rw-rw-r--   0 gweon     (1000) gweon     (1000)     4283 2023-05-08 19:25:33.000000 physicsfront-qiskit-0.1.6/setup.py
```

### Comparing `physicsfront-qiskit-0.1.5/LICENSE` & `physicsfront-qiskit-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `physicsfront-qiskit-0.1.5/PKG-INFO` & `physicsfront-qiskit-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsfront-qiskit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Utility package for qiskit
 Home-page: https://github.com/sam-pf/pf-qiskit
 Author: Physics Front LLC
 Author-email: info@physicsfront.com
 License: Apache 2.0
 Project-URL: GitHub, https://github.com/sam-pf/pf-qiskit
 Platform: Posix; MacOS X; Windows
@@ -19,13 +19,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
-Provides-Extra: ibm-provider
 Provides-Extra: mpl
 License-File: LICENSE
 
 This package provides modules such as physicsfront.qiskit and physicsfront.qiskit.colab.  These modules can be used to aid the usage of qiskit in various environments, e.g., in the Google Colab environment.
-
```

### Comparing `physicsfront-qiskit-0.1.5/physicsfront/qiskit/__init__.py` & `physicsfront-qiskit-0.1.6/physicsfront/qiskit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,20 @@
 # limitations under the License.
 ##
 
 from . import colab
 try:
     from . import patch
 except ModuleNotFoundError:
-    # e.g., if qiskit is not available yet (in colab)
+    ##
+    # If IBM qiskit is not available yet, then the patching won't work.  In
+    # such a case, the patching must be done manually by importing patch
+    # again after qiskit is installed.  For example, colab.init includes
+    # importing patch.
+    ##
     pass
 
 class WiringInstruction (object): # <<<
 
     """
     A helper class to ease composing quantum circuits.
 
@@ -255,59 +260,72 @@
         for r in qc1.cregs:
             qc0.add_register (r)
         return {'qubits': qubits_arg, 'clbits': clbits_arg}
     # >>>
 
 # >>>
 
-def backends (provider = None, hub = 'ibm-q', backend = None, ** kwargs): # <<<
+def backends (backend = None, provider = None, instance = None, # <<<
+              ** kwargs):
     """
-    Yields backends.
+    Yields backend instances given the information in the arguments.
 
-    Any :class:`~qiskit.providers.backend.Backend` instance, as specified as
-    the value of ``backend`` or any part of iterated values of ``backend``
-    will be left untouched and be yielded as is.  None of the arguments are
-    used in this case.
+    Any backend instance (of type
+    :class:`~qiskit_ibm_provider.ibm_backend.IBMBackend` or
+    :class:`~qiskit.providers.backend.Backend` instance), specified as the
+    value of ``backend`` or as an iterated value of an iterable ``backend``,
+    would be left untouched: such a backend instance would be yielded as is.
+
+    The rest of arguments are used only if there are any backends left to be
+    found.
 
     If ``backend`` is left unspecified, is a string, or an iterable that
-    yields a string among others, then the provider is necessasry to identify
-    and it will be obtained using ``provider`` and ``hub``.  Then, its
-    ``backends`` method is called with ``kwargs`` passed to it.  For example,
-    kwargs can specify a ``filters`` function.
-
-    :param backend:  A string (backend name),
-        a :class:`~qiskit.providers.backend.Backend` instance, an iterable of
-        them, or ``None``.
+    yields string, then arguments ``provider`` and ``instance`` are used
+    together to identify the provider (see :func:`get_provider`).  Then the
+    backends method of this provider is called with ``** kwargs`` to find
+    backends.  For example, ``kwargs`` can specify a ``filters`` function.
+
+
+    :param backend:  A string (backend name), a backend instance, an iterable
+        of strings or backend instances, or ``None``.
 
         The default value ``None`` means all backends for the provider,
-        specified by ``provider`` and ``hub`` (see :func:`~get_provider`).
+        specified by ``provider`` and ``instance``.
     """
-    from qiskit.providers.backend import Backend # pylint: disable=E0401,E0611
+    from qiskit_ibm_provider.ibm_backend import IBMBackend # new
+    from qiskit.providers.backend import Backend # old (deprecated) # pylint: disable=E0611,E0401
+    classes = (IBMBackend, Backend)
     it_backends = None
     if isinstance (backend, str):
         it_backends = [backend]
-    elif isinstance (backend, Backend):
+    elif isinstance (backend, classes):
         it_backends = [backend]
     elif backend is not None:
         it_backends = backend
     if it_backends is None:
-        for b in get_provider (provider = provider, hub = hub).backends (** kwargs):
+        for b in (get_provider (provider = provider, instance = instance)
+                  .backends (** kwargs)):
             yield b
     else:
         name2backend = None
         for b in it_backends:
             if isinstance (b, str):
                 if name2backend is None:
-                    # name is method in BackendV1 and property in BackendV2
-                    name2backend = dict (((s (), o) if callable (s) else (s, o))
+                    ##
+                    # name is a property/attribute for IBMBackend/BackendV2
+                    # and is a method in BackendV1
+                    ##
+                    name2backend = dict (((s (), o) if callable (s) else
+                                          (s, o))
                         for (s, o) in ((o.name, o) for o in get_provider
-                        (provider = provider, hub = hub).backends (** kwargs)))
+                        (provider = provider, instance = instance)
+                        .backends (** kwargs)))
                 yield name2backend [b]
             else:
-                assert isinstance (b, Backend)
+                assert isinstance (b, classes)
                 yield b
 # >>>
 def clbit_label_to_mii (r): # <<<
     """
     Given the job result ``r``, computes the mapping from the classical bit
     label to the memory item index.
 
@@ -596,68 +614,190 @@
     ans = Counter (it)
     if keys:
         if not isinstance (keys, Mapping):
             keys = dict ((k, 0) for k in keys)
         ans.update (keys)
     return ans
 # >>>
-def get_provider (provider = None, hub = 'ibm-q'): # <<<
-    """
-    If ``provider`` is not ``None``, then this function just returns it.
-    Otherwise, it will provision the provider based on ``hub``.
-    """
-    if provider is None:
-        from qiskit import IBMQ # pylint: disable=W0406,E0611
-        provider = IBMQ.get_provider (hub = hub)
-    return provider
-# >>>>>
-def jobs (provider = None, hub = 'ibm-q', backend = None, age = '1d', # <<<
-          ** kwargs):
+def get_provider (): # <<<
+    _cached = None
+    def _get_provider (provider = None, token = None, instance = None):
+        """
+        Returns a provider instance based on the information given.
+
+        1. If ``provider`` is given a provider instance (of type IBMProvider
+           or AccountProvider, the latter of which is deprecated), then it is
+           returned as is.
+
+           In this case, no cache mechanism is used.
+
+        2. If ``provider`` is any other value, it must be one of the
+           following values.
+
+                ``None``, ``"cached"``, ``"renew"``
+
+           In this case, a cache mechanism will kick into action.
+
+           First, even if the cache value exists, it is accepted only it is
+           valid.  The cached value is valid if the values for ``token`` and
+           ``instance`` of its active account are equal to the passed values,
+           if any, of ``token`` and ``instance`` arguments.
+
+           If ``provider`` is passed ``"cached"``, then any valid cached
+           provider value or ``None`` will be returned immediately.  This is
+           simply a check on the cached value.  The return value would be
+           either ``None`` or an IBMProvider instance.
+
+           If ``provider`` is passed ``"renew"``, then any cached value will
+           be expunged first.
+
+           If ``provider`` is ``None``, then any valid cached value will be
+           kept.
+
+           In the latter two cases, a new cache value will be provisioned if
+           a valid cached value is not found or has just been expunged.  Then
+           the new cached value, of type IBMProvider, will be returned.
+        """
+        ##
+        # These import statements can't be put outside this function, since
+        # colab.init must be loaded first to install these modules in the
+        # first place!
+        ##
+        from qiskit_ibm_provider.ibm_provider import IBMProvider
+        from qiskit.providers.ibmq.accountprovider import AccountProvider # pylint: disable=E0611,E0401
+        classes = (IBMProvider, AccountProvider)
+        from qiskit_ibm_provider import IBMProvider # pylint: disable=W0404
+        if isinstance (provider, classes):
+            return provider
+        nonlocal _cached
+        if provider == 'renew':
+            provider = _cached = None
+        has_cache_value = _cached is not None
+        if has_cache_value:
+            assert isinstance (_cached, classes [0])
+        has_valid_cache_value = (has_cache_value and
+            (token is None or
+             _cached.active_account () ['token'] == token) and
+            (instance is None or
+             _cached.active_account () ['instance'] == instance))
+        if provider == 'cached':
+            return _cached if has_valid_cache_value else None
+        if provider is not None:
+            raise ValueError ("** Invalid value passed for provider "
+                              f"argument: {provider}")
+        if not has_valid_cache_value:
+            _cached = IBMProvider (token = token, instance = instance)
+        assert isinstance (_cached, classes [0])
+        return _cached
+    return _get_provider
+get_provider = get_provider ()
+# >>>
+def jobs (provider = None, instance = None, age = '1d', ** kwargs): # <<<
     """
-    Yields jobs.
+    Yields jobs meeting the given descriptions at selected backends.
 
-    The arguments ``provider``, ``hub``, and ``backend`` are used to get
-    backends (see :func:`~backends`).  Then, for each backend, jobs are
-    yielded with ``kwargs``.
+    The arguments ``provider``, ``instance`` are used to get the provider
+    (:func:`get_provider`).
 
-    For details of what ``kwargs`` can be,
-    `see here <https://qiskit.org/documentation/stubs/qiskit.providers.ibmq.IBMQBackend.jobs.html>`_.
+    Then, ``provider.backend.jobs`` is invoked with ``kwargs`` passed to it
+    to collect jobs.
 
-    Note that by default ``limit = 10`` is, implicitly, part of ``kwargs``,
-    which means, in this function, 10 jobs maximum yielded per backend.
+    For possible keys for ``kwargs``, see the documentation for
+    :func:`~qiskit_ibm_provider.ibm_backend_service.IBMBackendService.jobs`.
+    The keys include ``"backend_name"`` (to filter for specific backend),
+    ``"start_datetime"``, and ``"end_datetime"``. 
 
-    If none of ``kwargs`` is given, then by default
+    Note that by default ``limit = 10`` is implied, meaning the maximum of 10
+    jobs yielded.
 
     :param age:  By default, the ``start_datetime`` argument in ``kwargs`` is
         automatically generated so that only jobs created within one day are
         yielded.
 
         To change this behavior, the value of this argument may be changed to
         any other string that ends with 'd' or 'h', or any false value (in
         which case, there will be no consideration of this argument).
 
-        If ``start_datetime`` is specified in ``kwargs``, then this argument
-        will not be considered at all.
+        If ``start_datetime`` is already specified in ``kwargs``, then that
+        takes precedence and this argument will have no effect at all.
     """
     if 'start_datetime' not in kwargs and age:
         import datetime, dateutil
         timedelta_o = None
         if isinstance (age, str):
             if age.endswith ('d'):
                 timedelta_o = datetime.timedelta (days = float (age [:-1]))
             elif age.endswith ('h'):
                 timedelta_o = datetime.timedelta (hours = float (age [:-1]))
         if timedelta_o is None:
             raise ValueError ("age must be a string that ends with 'd' or 'h'")
         kwargs ['start_datetime'] = (
                 datetime.datetime.now (dateutil.tz.tzlocal ()) -
                 timedelta_o)
-    for b in backends (provider = provider, hub = hub, backend = backend):
-        for j in b.jobs (** kwargs):
-            yield j
+    p = get_provider (provider = provider, instance = instance)
+    for j in p.backend.jobs (** kwargs):
+        yield j
+# >>>
+def jobs_monitor (jobs, interval = None, # <<< # pylint: disable=W0621
+                  quiet = False, job_id_minlen = 6,
+                  line_discipline = "\r", output = None):
+    """
+    A bit like of qiskit.tools.monitor.job_monitor, but for an iterable of
+    jobs, instead of a single job.
+    """
+    import sys, time
+    if interval is None:
+        interval = 5
+    assert type (interval) is int and interval >= 1
+    assert type (job_id_minlen) is int and job_id_minlen >= 4
+    assert type (line_discipline) is str
+    if output is None:
+        output = sys.stderr
+    #print (type (jobs), jobs)
+    jobs = tuple (jobs)
+    n_jobs = len (jobs)
+    ended = frozenset (('DONE', 'CANCELLED', 'ERROR'))
+    states = [None] * n_jobs
+    job_ids = list (job.job_id () for job in jobs)
+    while True:
+        job_ids_short = list (j [:job_id_minlen] for j in job_ids)
+        if len (set (job_ids_short)) == n_jobs:
+            break
+        job_id_minlen += 2
+    all_ended = False
+    msg_len = 0
+    while True:
+        all_ended = True
+        for i, job in enumerate (jobs):
+            if states [i] in ended:
+                continue
+            status = job.status ()
+            state = status.name
+            if state == 'QUEUED':
+                queue_position = job.queue_position ()
+                if queue_position is not None:
+                    state += f'({queue_position})'
+            states [i] = state
+            all_ended = False
+        msg = (f'Status for {n_jobs} job{"s" if n_jobs > 1 else ""}: ' +
+            ', '.join (':'.join ([job_id_short, state])
+                for job_id_short, state in zip (job_ids_short, states)))
+        lendiff = msg_len - len (msg)
+        if lendiff > 0:
+            msg += " " * lendiff
+        msg_len = len (msg)
+        if not quiet:
+            print (line_discipline + msg, end = '', file = output)
+        if all_ended:
+            break
+        if 'QUEUED' not in states:
+            interval = 2
+        time.sleep (interval)
+    if not quiet:
+        print ('', file = output)
 # >>>
 def memory_item_index (r, * clbitspec): # <<<
     """
     Given a job result ``r`` and classical bit spec(s) ``clbitspec``, returns
     the corresponding memory item index/indices.
 
     If only one ``clbitspec`` is given, then an index will be returned.  If
@@ -691,68 +831,64 @@
                 raise ValueError (f'Name {name!r} does not complete a '
                                   'classical bit register name (uniquely).')
             regname = cands [0]
         ans.append (clabel2index [(regname, index) if key_is_tuple
                                   else regname])
     return ans [0] if len (ans) == 1 else tuple (ans)
 # >>>
-def run_quantum_computer (qc, hub = 'ibm-q', shots = 2000, memory = True, # <<<
-                          qasm3 = False, backend = None, quiet = False):
+def run_quantum_computer (qc, instance = None, shots = 2000, # <<<
+                          memory = True, qasm3 = False, backend = None,
+                          quiet = False):
     """
-    Runs a real quantum computer on quantum circuit ``qc``.
+    Runs quantum circuit ``qc`` on a real quantum computer.
 
     :param qasm3:  WIP.  Does not seem to work if this option is turned on,
         as of 01-25-2023.  Nor do the dynamic code examples in the IBM qiskit
         tutorial, when they are run in IBM Quantum Jupyter lab.
 
         When this argument is turned on, passing ``backend`` as a backend
         instance might be preferred.  And, ``memory`` might not work (I get a
         warning).
 
     :param backend:  If given, then it can be a backend instance or a backend
         name.
     """
     n = qc.num_qubits
-    if qasm3:
-        from qiskit_ibm_provider import IBMProvider
-        provider = IBMProvider ()
-    else:
-        provider = None
-    bs = list (backends (provider = provider, hub = hub, backend = backend,
+    bs = list (backends (instance = instance, backend = backend,
                          filters = lambda x:
                             x.configuration ().n_qubits >= n and
                             not x.configuration ().simulator and
                             x.status ().operational == True))
     if not len (bs):
-        raise ValueError ("No operational backends found.")
+        raise ValueError ("No suitable backends found.")
     if len (bs) > 1:
-        from qiskit.providers.ibmq import least_busy # pylint: disable=W0406,E0401,E0611
+        from qiskit_ibm_provider import least_busy
         b = least_busy (bs)
         if not quiet:
             print ("backend auto-determined as the least busy:", b)
     else:
         b = bs [0]
     from qiskit import transpile # pylint: disable=W0406,E0611
     kwargs = {}
-    if qasm3:
+    if qasm3: # WIP
         #from qiskit import qasm3 as q3 # pylint: disable=W0406,E0611
         qc_t = transpile (qc, b)
         #runnable = q3.Exporter (basis_gates =
         #        b.configuration ().basis_gates).dumps (qc_t)
         runnable = qc_t
         kwargs ['dynamic'] = True
     else:
         runnable = transpile (qc, b, optimization_level = 3)
     return b.run (runnable, shots = shots, memory = memory, ** kwargs)
 # >>>
 def run_quantum_simulator (qc, shots = 2000, memory = True, seed = 100): # <<<
     """
     Runs an Aer quantum simulator on the quantum circuit ``qc``.
 
-    See :func:`run_quantum` for how to process the run result.
+    See :func:`run_quantum_computer` for how to process the run result.
 
     In a simulator run, it is also possible to do
 
         `r.get_statevector ()`
 
     assuming that the statevector was saved in the qc.
```

### Comparing `physicsfront-qiskit-0.1.5/physicsfront/qiskit/colab.py` & `physicsfront-qiskit-0.1.6/physicsfront/qiskit/colab.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,60 +10,87 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ##
 
-PIP_PKGS_TO_INSTALL = ('qiskit', 'qiskit_ibm_provider', 'matplotlib', 'pylatexenc')
+import os, io
+
+##
+# PIP_PKGS_TO_INSTALL: collect all packages from _requires.py (including
+#   extras; as colab needs all) into a tuple.
+##
+with io.open (os.path.join (os.path.split (__file__) [0], '_requires.py'),
+              'r', encoding = 'utf-8') as _:
+    PIP_PKGS_TO_INSTALL = {}
+    exec (_.read (), PIP_PKGS_TO_INSTALL)
+    PIP_PKGS_TO_INSTALL = (list (PIP_PKGS_TO_INSTALL ['dependencies']) +
+        sum ((list (l) for l
+              in PIP_PKGS_TO_INSTALL.get ('extras', {}).values ()), []))
+    PIP_PKGS_TO_INSTALL = tuple (w.replace (' ', '')
+                                for w in PIP_PKGS_TO_INSTALL)
 
 def _check_setup_file (kind, fallback_filename = None): # <<<
     """
-    Checks the qiskitrc or settings file and returns that file name.
+    Checks, or creates, a qiskit setup file of the given kind.
+
+    If the file does not exist and if ``fallback_filename`` has been given,
+    then the file is created by copying ``fallback_filename``.
 
     :returns:  ``(setup_filename, status)``
 
-        ``setup_filename`` is the setup file name that will be read by
-        qiskit.
+        ``setup_filename`` is the name of the setup file that qiskit will
+        read.
+
+        ``status`` would be false if checking or creating the setup file
+        failed.
 
-        ``status`` is false if ``setup_filename`` does not exist.
+        If ``status`` is true, it will be either ``setup_filename`` (if it
+        existed already) or ``fallback_filename`` (it it was copied from
+        fallback).
 
-        If ``status`` is true, it will be either ``setup_filename`` or
-        ``fallback_filename``.
+    :param kind:  'json', 'conf', or 'rc'
 
-    :param kind:  'rc', 'conf', or 'json'
+        The corresponding file name is respectively  'qiskit-ibm.json',
+        'settings.conf', and 'qiskitrc'.
 
-        The corresponding file names are respectively 'qiskitrc',
-        'settings.conf', and 'qiskit-ibm.json'.
+        Consider the 'rc' kind as deprecated since the 'rc' setup file is
+        read by qiskit.providers or qiskit.IBMQ, both of which are deprecated
+        modules.  The new module to use is qiskit_ibm_provider, which uses
+        the 'json' kind for account information.
 
     :param fallback_filename:  If the file does not exist and this
-        filename is given, then this file will be copied to the setup file,
-        before fallback_filename is returned.
+        filename is given, then this file will be copied to the setup file.
 
-        If this name is given, then it will be replaced by the value returned
-        by :func:`_correct_filename`.
+        The name may be subject to a correction by :func:`_correct_filename`
+        (for internal technical reasons related to file system matters,
+        basically).
+
+        When this name was utilized, then the ``status`` value in the return
+        tuple will be this name (possibly corrected).
     """
-    import os.path, shutil
+    import shutil
     setup_dir = os.path.join (os.path.expandvars ('$HOME'), '.qiskit')
     if kind == 'rc':
         filename = 'qiskitrc'
     elif kind == 'conf':
         filename = 'settings.conf'
     else:
         assert kind == 'json'
         filename = 'qiskit-ibm.json'
     setup_file = os.path.join (setup_dir, filename)
     if os.path.exists (setup_file):
         return (setup_file, setup_file)
+    if not os.path.exists (setup_dir):
+        os.mkdir (setup_dir)
     if fallback_filename:
         #print (fallback_filename, '...', end = ' ')
         fallback_filename = _correct_filename (fallback_filename)
         #print (fallback_filename)
-        if not os.path.exists (setup_dir):
-            os.mkdir (setup_dir)
         if shutil.copy2 (fallback_filename, setup_file):
             return (setup_file, fallback_filename)
     return (setup_file, False)
 # >>>
 def _correct_filename (filename): # <<<
     """
     Corrects ``filename`` in an edge case of a Google Drive access within
@@ -85,99 +112,93 @@
     #. There is no file (or folder) with ``filename``.
 
     #. There is no extension in ``filename``.
 
     #. There is one unique file found with its name = ``filename`` +
        extension (which cannot have another '.').
     """
-    import os.path
     if os.path.exists (filename):
         return filename
     dname, fname = os.path.split (filename)
     if '.' in fname:
         return filename
     cands = list (name for name in os.listdir (dname)
                   if name.split ('.') [0] == fname)
     if len (cands) != 1 or len (cands [0].split ('.')) != 2:
         return filename
     return os.path.join (dname, cands [0])
 # >>>
-def _install_pip_packages (reload = False, quiet = False): # <<<
+def _install_pip_packages (reload = False, quiet = False): # <<< # pylint: disable=W0613
     import subprocess, sys
-    if 'qiskit' in sys.modules and not reload:
-        if not quiet:
-            print ("== Installing/checking needed pip packages: aborted since "
-                   "qiskit has already been imported and reload was not "
-                   "requested.\n"
-                   "   Restart runtime if you wish to restart everything anew.")
-        return
     pkgs = list (PIP_PKGS_TO_INSTALL)
     if not quiet:
         print ("== Installing/checking needed pip packages:", pkgs,
                '...', end = ' ', flush = True)
     r = subprocess.run ([sys.executable, "-m", "pip", "install"] + pkgs, # pylint: disable=W1510
                         capture_output = True)
     rv = r.returncode
     if not rv:
         if not quiet: print ("OK!")
         return
     if not quiet:
         print ("\r", end = '')
     print ("** Error while installing required pip packages:", pkgs)
     print (r.stderr.decode ('utf-8'))
-    raise Exception ("pip returned error %d" % (rv,))
+    raise SystemError ("pip returned error %d" % (rv,))
 # >>>
-def _setup_account (reload = False, quiet = False, filename = None): # <<<
-    from qiskit import IBMQ # pylint: disable=E0611
+def _setup_account (reload = False, instance = None, quiet = False, # <<<
+                    filename = None):
+    """
+    :param filename:  Used as ``fallback_filename`` when checking the account
+        setup file.
+    """
+    ##
+    # The method that involves
+    # qiskit.IBMQ.{active_account,disable_account,load_account} has been
+    # deprecated.  As of 2023-05-07, it has been noted that the jobs executed
+    # in the last couple of days do not show up, if the job query is made
+    # from the deprecated provider.  They do show up if the job query is made
+    # from a provider of new type, which is recommended for use.  So, it is
+    # time to move on to the new style.
+    ##
     if not quiet:
         print ("== Account setup (you might be prompted for an API TOKEN) ...",
                end = ' ', flush = True)
-    d = IBMQ.active_account ()
-    if d and not reload:
+    from . import get_provider
+    provider = get_provider (provider = 'cached', instance = instance)
+    if provider and not reload:
         if not quiet:
             print ("OK! (account already active; reload not requested)\n"
-                   "   Restart runtime if you wish to restart everything anew.")
+                "   Restart runtime if you wish to restart everything anew.")
         return
-    _, rv = _check_setup_file ('rc', fallback_filename = filename)
-    if reload: IBMQ.disable_account ()
+    _, rv = _check_setup_file ('json', fallback_filename = filename)
     if rv:
-        IBMQ.load_account ()
+        provider = get_provider (provider = 'renew' if reload else None,
+                                 instance = instance)
     else:
-        old_token = d ['token'] if d else ''
-        import IPython
+        old_token = '' # d ['token'] if d else ''
+        import IPython # pylint: disable=E0401
         display = IPython.display.display
         from google.colab import output # pylint: disable=E0401,E0611
         display (IPython.display.Javascript (f'window._key = "{old_token}"'))
         display (IPython.display.Javascript ('''
-window._key = prompt ("Please enter your IBMQ API TOKEN:", window._key)
+window._key = prompt ("Please enter your IBM Quantum API TOKEN:", window._key)
         '''))
         token = output.eval_js ('_key')
         # for safety; even if javascript is sandboxed per cell
         output.eval_js ('delete window._key')
-        IBMQ.enable_account (token)
-    d = IBMQ.active_account ()
-    if not d:
-        raise Exception ("Failed to set up an IBMQ account.")
-    jsonfilename, rv = _check_setup_file ('json')
+        provider = get_provider (token = token, instance = instance)
+    if not provider:
+        raise Exception ("Failed to set up an IBM Quantum provider.") # pylint: disable=W0719
     if not rv:
-        jsonobj = {
-            'default-ibm-quantum': {
-                'channel': 'ibm_quantum',
-                'token': d ['token'],
-                'url': d.get ('url',
-                              'https://auth.quantum-computing.ibm.com/api'),
-            },
-        }
-        import json
-        json.dump (jsonobj, open (jsonfilename, 'w', encoding = 'utf-8'))
+        provider.save_account ()
     if not quiet:
         print ("OK!")
 # >>>
 def _setup_settings (reload = False, quiet = False, filename = None): # <<<
-    import io
     if not quiet:
         print ("== Qiskit settings file check ...", end = ' ', flush = True)
     setupfname, rv = _check_setup_file ('conf', fallback_filename = filename)
     msg = ''
     if rv:
         if rv == setupfname:
             msg = 'file exists'
@@ -192,15 +213,15 @@
 ''')
         msg = 'created with default content'
     assert msg
     if not quiet:
         print ("OK! (" + msg + ")")
 # >>>
 
-def init (reload = False, quiet = False, qiskitrc_filename = None,
-          settings_filename = None):
+def init (reload = False, quiet = False, json_filename = None,
+          conf_filename = None):
     _install_pip_packages (reload = reload, quiet = quiet)
     _setup_settings (reload = reload, quiet = quiet,
-                     filename = settings_filename)
+                     filename = conf_filename)
     _setup_account (reload = reload, quiet = quiet,
-                    filename = qiskitrc_filename)
+                    filename = json_filename)
     from . import patch as _
```

### Comparing `physicsfront-qiskit-0.1.5/physicsfront/qiskit/patch.py` & `physicsfront-qiskit-0.1.6/physicsfront/qiskit/patch.py`

 * *Files identical despite different names*

### Comparing `physicsfront-qiskit-0.1.5/physicsfront_qiskit.egg-info/PKG-INFO` & `physicsfront-qiskit-0.1.6/physicsfront_qiskit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicsfront-qiskit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Utility package for qiskit
 Home-page: https://github.com/sam-pf/pf-qiskit
 Author: Physics Front LLC
 Author-email: info@physicsfront.com
 License: Apache 2.0
 Project-URL: GitHub, https://github.com/sam-pf/pf-qiskit
 Platform: Posix; MacOS X; Windows
@@ -19,13 +19,11 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
-Provides-Extra: ibm-provider
 Provides-Extra: mpl
 License-File: LICENSE
 
 This package provides modules such as physicsfront.qiskit and physicsfront.qiskit.colab.  These modules can be used to aid the usage of qiskit in various environments, e.g., in the Google Colab environment.
-
```

### Comparing `physicsfront-qiskit-0.1.5/setup.py` & `physicsfront-qiskit-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,44 +18,32 @@
 author = "Physics Front LLC"
 author_email = "info@physicsfront.com"
 url = "https://github.com/sam-pf/pf-qiskit"
 project_urls = {
     'GitHub': url,
     # potential useful keys: 'Documentation', 'ChangeLog', 'Issues', ...
 }
-version = "0.1.5"
+version = "0.1.6"
 license_ = "Apache 2.0"
 description = "Utility package for qiskit"
 long_description = "This package provides modules such as physicsfront.qiskit and physicsfront.qiskit.colab.  These modules can be used to aid the usage of qiskit in various environments, e.g., in the Google Colab environment."
 
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = 'Development Status :: 3 - Alpha'
 
-##
-# These requirements are rough values determined from limited test runs in
-# google colab as well as terminal based ipython.
-##
-dependencies = [
-    "qiskit >= 0.39.2",
-]
-extras = {
-    "mpl": [
-        "matplotlib >= 3.2.2",
-        "pylatexenc >= 2.10",
-    ],
-    "ibm-provider": [
-        "qiskit_ibm_provider >= 0.1.0",
-    ],
-}
-python_requires = ">=3.8"
+import io, os, setuptools, sys
 
-import os, setuptools, sys
+# dependencies, extras, python_requires
+exec (io.open (os.path.join (os.path.split (__file__)[0],
+                             'physicsfront', 'qiskit', '_requires.py'),
+               mode = 'r', encoding = 'utf-8').read (),
+      globals ())
 
 packages = setuptools.find_namespace_packages (include = ['physicsfront.*'])
 
 namespaces = ["physicsfront"]
 # any additional namespace as necessary (none so far)
 #if "physicsfront.cloud" in packages:
 #    namespaces.append("physicsfront.cloud")
@@ -69,54 +57,56 @@
 # with a false value _before_ running the content of this file.
 #
 # Example: python3 -c '_do_setup = False; exec (open ("setup.py", "r").read ()); print (version)'
 ##
 try:
     _do_setup # pylint: disable=E0601
 except:
-    _do_setup = True
+    _do_setup = __name__ == '__main__'
 
 if _do_setup and __name__ == '__main__' and os.environ.get ('PYARUNNING'):
     # 'PYARUNNING' set with any non-empty value? take it as 'pdf dev cycle'.
     if sys.argv [-1] == 'setup.py' or sys.argv [-1].endswith ('/setup.py'):
         ##
         # Some (auto) pf dev cylce command may invoke this file with no
         # argument following this file name.  We allow such type of
         # invocation by falling back to 'check'.
         ##
         sys.argv.append ('check')
-
 # >>>
 
-if _do_setup: setuptools.setup (
-    name = name,
-    version = version,
-    description = description,
-    long_description = long_description,
-    author = author,
-    author_email = author_email,
-    license = license_,
-    url = url,
-    project_urls = project_urls,
-    classifiers = [
-        release_status,
-        "Intended Audience :: Developers",
-        "Intended Audience :: Education",
-        "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Operating System :: OS Independent",
-        "Topic :: Internet",
-        "Topic :: Scientific/Engineering :: Physics",
-        "Topic :: Security :: Cryptography",
-    ],
-    platforms = "Posix; MacOS X; Windows",
-    packages = packages,
-    namespace_packages = namespaces,
-    install_requires = dependencies,
-    extras_require = extras,
-    python_requires = python_requires,
-)
+if _do_setup:
+    import pkg_resources
+    for _ in namespaces:
+        pkg_resources.declare_namespace (_)
+    setuptools.setup (
+        name = name,
+        version = version,
+        description = description,
+        long_description = long_description,
+        author = author,
+        author_email = author_email,
+        license = license_,
+        url = url,
+        project_urls = project_urls,
+        classifiers = [
+            release_status,
+            "Intended Audience :: Developers",
+            "Intended Audience :: Education",
+            "License :: OSI Approved :: Apache Software License",
+            "Programming Language :: Python",
+            "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
+            "Operating System :: OS Independent",
+            "Topic :: Internet",
+            "Topic :: Scientific/Engineering :: Physics",
+            "Topic :: Security :: Cryptography",
+        ],
+        platforms = "Posix; MacOS X; Windows",
+        packages = packages,
+        install_requires = dependencies, # pylint: disable=E0602
+        extras_require = extras, # pylint: disable=E0602
+        python_requires = python_requires, # pylint: disable=E0602
+    )
```

