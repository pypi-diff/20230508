# Comparing `tmp/pqinput-0.0.2.tar.gz` & `tmp/pqinput-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.2.tar", last modified: Mon Feb 20 12:22:17 2023, max compression
+gzip compressed data, was "pqinput-0.0.3.tar", last modified: Mon May  8 09:03:02 2023, max compression
```

## Comparing `pqinput-0.0.2.tar` & `pqinput-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-20 12:22:17.728445 pqinput-0.0.2/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.2/LICENSE.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1573 2023-02-20 12:22:17.724445 pqinput-0.0.2/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1002 2023-02-20 12:21:44.000000 pqinput-0.0.2/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-20 12:22:17.724445 pqinput-0.0.2/pqinput/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      107 2023-02-09 09:26:09.000000 pqinput-0.0.2/pqinput/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11237 2023-02-14 10:36:27.000000 pqinput-0.0.2/pqinput/inpxml.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-02-20 12:22:17.724445 pqinput-0.0.2/pqinput.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1573 2023-02-20 12:22:17.000000 pqinput-0.0.2/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      207 2023-02-20 12:22:17.000000 pqinput-0.0.2/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-02-20 12:22:17.000000 pqinput-0.0.2/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-02-20 12:22:17.000000 pqinput-0.0.2/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      539 2023-02-20 12:14:18.000000 pqinput-0.0.2/pyproject.toml
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-02-20 12:22:17.728445 pqinput-0.0.2/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      657 2023-02-20 12:14:09.000000 pqinput-0.0.2/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:03:02.726419 pqinput-0.0.3/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.3/LICENSE.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1934 2023-05-08 09:03:02.726419 pqinput-0.0.3/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1363 2023-02-20 12:29:30.000000 pqinput-0.0.3/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:03:02.726419 pqinput-0.0.3/pqinput/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      119 2023-05-04 15:25:36.000000 pqinput-0.0.3/pqinput/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8411 2023-05-08 08:52:27.000000 pqinput-0.0.3/pqinput/drawPES.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    13687 2023-05-04 15:14:28.000000 pqinput-0.0.3/pqinput/inpxml.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-08 09:03:02.726419 pqinput-0.0.3/pqinput.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1934 2023-05-08 09:03:02.000000 pqinput-0.0.3/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-08 09:03:02.000000 pqinput-0.0.3/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-08 09:03:02.000000 pqinput-0.0.3/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-08 09:03:02.000000 pqinput-0.0.3/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      540 2023-05-08 09:01:24.000000 pqinput-0.0.3/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-08 09:03:02.726419 pqinput-0.0.3/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      651 2023-05-08 09:01:57.000000 pqinput-0.0.3/setup.py
```

### Comparing `pqinput-0.0.2/LICENSE.txt` & `pqinput-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.2/README.md` & `pqinput-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 # Python package for making QDng calculations inputs
 
 ### Module:
 - `inpxml.py`: **InpXML** class with methods designed for the creation of *xml* structures intended as input files for quantum chemistry calculations with QDng package. Requires *lxml*.
 ### Example: 
+In:
+    mCO = 1240 
+    T = {'head':'T', 'name':"GridNablaSq", 'mass':mCO}
+    Vg = {'head':'V', 'name':"GridPotential", 'file':'pot_Vg'}
+    Ve = {'head':'V', 'name':"GridPotential", 'file':'pot_Ve'}
+    mel = {'head':'m0.0', 'name':'Sum', 'Opes':[T, Vg]}
 
+    Hparams = {'type':'Sum', 'Mels':mel} 
+    WFpar = {'type':'file', 'states':1, 'file':'wfguess', 'normalize':False}
     propapar = {'dt': 0.165697, 'steps': 500, 'wcycle': 100, 'dir': 'propa_files', 'nfile': 'norm'}
+    
     prop = InpXML()
     prop.program('propa', propapar, WFpar)
     prop.propagation('Cheby', Hparams)
     prop.addfilter('filterpost', {'expeconly':{'name':'Flux', 'int':'True'}})
     prop.show()
 
-> Output:
-`<qdng>`
-`  <propa dt="0.165697" steps="500" wcycle="100" dir="propa_files" nfile="norm">`
-`    <propagator name="Cheby">`
-`      <hamiltonian name="Sum">`
-`        <T name="GridNablaSq" mass="1240"/>`
-`        <V name="GridPotential" file="pot_Vg"/>`
-`      </hamiltonian>`
-`    </propagator>`
-`    <wf file="wfguess"/>`
-`    <filterpost>`
-`      <expeconly name="Flux" int="True"/>`
-`    </filterpost>`
-`  </propa>`
-`</qdng>`
+Out:
+```xml
+<qdng>
+  <propa dt="0.165697" steps="500" wcycle="100" dir="propa_files" nfile="norm">
+   <propagator name="Cheby">
+      <hamiltonian name="Sum">
+        <T name="GridNablaSq" mass="1240"/>
+        <V name="GridPotential" file="pot_Vg"/>
+      </hamiltonian>
+    </propagator>
+    <wf file="wfguess"/>
+    <filterpost>
+      <expeconly name="Flux" int="True"/>
+    </filterpost>
+  </propa>
+</qdng>
+```
+
+
+
```

### Comparing `pqinput-0.0.2/pqinput/inpxml.py` & `pqinput-0.0.3/pqinput/inpxml.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,18 +4,30 @@
 Created on Mon Jan  9 15:02:59 2023
 
 @author: lucas
 
 New INPUTMAKER with a "dictionary to XML" structure 
 
 """
+
+'''TO IMPLEMENT
+make laser part functional
+'''
 # %% Imports
 from lxml import etree as et
 
 # %% General functions
+def dict2attr(element, params, tag=None):
+    """ set the attributes for the xml element using a dict
+        ignores keys as head, Opes and extras    """
+    for key, value in params.items(): 
+        if key not in ('head', 'Opes', 'extra'):
+            element.set(str(key), str(value))
+    if tag: element.tag = tag
+    
 def dict2elem(d, head=None, text_mode=False):
     """ transform a dictionary to a etree.element
     
     Args:
         d (dict) dictionary with attributes in key:value format
         _format: {'head':str, attr1:value1, ..., 'Opes':[dicts, ]}   
         head (string) node for the etree.Element
@@ -24,97 +36,75 @@
     Return: 
         string format of the etree.Element if text_mode else the etree._Element
         
         E.g.
         
         _In: dict2elem({'head':'node', 'attr1':'value1', 'Opes':[{'Op_element':'op'}]}, text_mode=True)
         
-        _Out: b'<node attr1="value1"/>' 
+        _Out: b'<node attr1="value1"/>'
         
         # missing the operators part...
     """
     if not isinstance(d, dict):
         raise SyntaxError('Provide a dictionary to transform in a lxml element.')
     xml = et.Element(d['head']) if head==None else et.Element(head)
     # set the attributes of the lxml element removing the head and Operators part
-    [xml.set(str(key), str(value)) for key, value in d.items() if key not in ('head', 'Opes')]
-
+    # [xml.set(str(key), str(value)) for key, value in d.items() if key not in ('head', 'Opes')]
+    dict2attr(xml, d)
     return et.tostring(xml) if text_mode else xml
 
-def printx(xmlelem):
-    print(et.tostring(xmlelem, pretty_print=True).decode())
-
-# %% Class functions
-def hamilt_elem(propag, Hp):    
-    # Create a lxml element to be appended to the self.propag 
-    Hel = et.SubElement(propag, 'hamiltonian')
-    # upper element of self.qdng
-    if Hp['type'] == 'Sum':
-        Hel.set('name', Hp['type'])
-        # (Hel.append(dict2elem(melOpe) ) for melOpe in Hp['Mels']['Opes'] )
-        for opes in Hp['Mels']['Opes']:
-            Operator = et.SubElement(Hel, opes['head'])
-            [Operator.set(str(key), str(value)) for key, value in opes.items() if key not in ('head','Opes')]
-            # Hel.append( dict2elem(opes)) 
-
-    elif Hp['type'] == 'Multistate':
-        Hel.set('name', Hp['type'])
-        if None == Hp['Mels']:
-            raise SyntaxError('Include states for the Multistate hamiltonian!')
-        else:
-            for mel in Hp['Mels'][:]:
-                if not mel:
-                    pass
-                else:
-                    branch = et.SubElement(Hel, mel['head'])
-                    [branch.set(str(key), str(value)) for key, value in mel.items() if key not in ('head','Opes')]
-
-                    if 'Opes' in  mel.keys():
-                        for ind in range(len(mel['Opes'])):
-                            branch.append( dict2elem(mel['Opes'][ind])) 
-    return Hel
+def subelem(supelem, params, head=None):
+    """ create subelement for a lxml supelement using params dict
+    Input:
+        params; string - tail of subelement
+                dict - tail with parameters
+    Return: 
+        lxml element; not mandatory
+    """
+    if not head:
+        try: 
+            params['head']
+        except:
+            raise SyntaxError('element head not provided')
+    else: params['head'] = head
+    sub = et.SubElement(supelem, params['head'])
+    dict2attr(sub, params) 
+    return sub
 
-def filterpost(filter_list):
-    Filt = et.Element('filterpost')
+def printx(xmlelem): # works for any kind of lxml element, show is just for class
+    print(et.tostring(xmlelem, pretty_print=True).decode())
     
-    for dic in filter_list:
-        [et.SubElement(Filt, str(opes), values) for opes, values in dic.items() 
-         if not opes.startswith('m')]
-        [et.SubElement(Filt.getchildren()[-1], str(opes), values) for opes, values in dic.items() 
-          if opes.startswith('m')]
-    return Filt
-
-def wfun_elem(wfp):
-    # wfel = et.SubElement(branch, 'wf', name=wfp['name'])
-    # wfp = ['name', 'file', 'states', 'coeff2', 'normalize']
-    if wfp['type'] == 'file':
-        wfel = et.Element('wf')
-        wfel.set('file', wfp['file'])
-        
-    elif wfp['type'] == 'LC':
-        wfel = et.Element('wf', name=wfp['type'])
-        if 'normalize' in wfp.keys() and wfp['normalize']: wfel.set('normalize', 'true')
-        for ind in range(wfp['states']):
-            wfstate = et.SubElement(wfel, 'wf'+str(ind))
-            wfstate.set('file', wfp['file'][ind])
-        
-    elif wfp['type'] == 'Multistate':
-        wfel = et.Element('wf', name=wfp['type'])
-        wfel.set('states', str(wfp['states']))
-        if 'normalize' in wfp.keys() and wfp['normalize']: wfel.set('normalize', 'true')
-        # if wfp['states']!=len(wfp['file']): raise SyntaxError('number of states not equal to provided files!')
-        for ii, index in enumerate(wfp['index']):
-            wfstate = et.SubElement(wfel, 'wf'+str(index), file=str(wfp['file'][ii]))
-            if 'coeff2' in wfp.keys(): wfstate.set('coeff2', wfp['coeff2'][ii])
-        
-    else:
-        raise SyntaxError('Wvefunction type not defined.')
-    return wfel
-
-# %% Class
+    # Property methods
+def typed_property(name): # Python Cookbook 3rd: 9.21
+    storage_name = '_' + name
+    
+    @property
+    def propriety(self): # lost in translation hehe
+        # Print the property element 
+        if not hasattr(self, storage_name): raise AttributeError(f'{name} attribute not defined.')
+        return printx(getattr(self, storage_name))
+    
+    @propriety.setter
+    def propriety(self, args):
+        # modify key with new_value of propriedade using path 
+        # args = [path, key, new_value] or "path_key_new_value"
+        if isinstance(args, str): args = args.split('_') # single string format
+        path, key, new_value = args
+        element = getattr(self, storage_name).find(path)
+        if element is None: raise AttributeError('setter path do not point to a defined attribute.')
+        element.set(key, str(new_value))
+        printx(element)
+        
+        # READ MORE ABOUT XPATH AND IF ITS USEFUL
+        
+    return propriety
+# %% 
+'''-------------------------------------------------------------------------'''
+'''                                Class                                    '''
+'''-------------------------------------------------------------------------'''
 class InpXML:
     """ InpXMl class for the creation of a qdng calculation input in xml format.
     requires the lxml.etree package
     
     Args:
         qdng_params (dict) parameters for the qdng calculation
         _format: {attr1:value1, attr2:value2, ... }
@@ -125,62 +115,131 @@
         program (etree._Element) program body: 
             either propa or eigen
         propag (etree._Element) branch of a program
         hamilt (etree._Element) branch a propagation: 
             subelement required for a Cheby propagation
         wavefunc (etree._Element) wavefunction body: 
             inclusion of initial wavefunctions for the calculations
+    
+    Properties:
+        show: prints out the class text in readable xml format
         
         
     * comments from QDng documentation
     """
+    qdng = et.Element("qdng") # Root of the XML tree: self.qdng, with the tag-headline 
+    
+    def __init__(self, qdng_params=None): # Initiate the input layout 
+        if qdng_params: dict2attr(self.qdng, qdng_params)
         
-    # %% Initiate the input layout 
-    def __init__(self, qdng_params=None):
-        # Root of the XML tree: self.qdng, with the tag-headline
-        self.qdng = et.Element("qdng")
-        # set the attributes for the root if qdng_params dict is provided
-        if not qdng_params==None:
-            for key, value in qdng_params.items():
-                self.qdng.set(str(key), str(value))
-      
-    def __str__(self):
-        return et.tostring(self.qdng, pretty_print=True).decode()
-    
-    def show(self):
-        print(self)
-    # %% Programs
-    def program(self, ptype, program_params, wf_params):
+    def __str__(self): # define string format for printing
+        return f'{et.tostring(self.qdng, pretty_print=True).decode()}'    
+    
+    @property
+    def show(self): # printing property
+        '''Print out the full text in readable xml format
+        Useful for debugging '''
+        print(self)     
+    
+# %% 
+    ''' METHODS '''
+    ######################## Write file ########################
+    def writexml(self, file_name='test_file', txt=False):
+        """ Write the constructed lxml element to a XML file. """
+        tree = et.ElementTree(self.qdng)
+        if file_name.endswith('.txt'): 
+            txt = True 
+            file_name = file_name.strip('.txt')
+        tree.write(file_name + ('.txt' if txt else '.xml'), pretty_print=True)
+        
+    def modify(self, path, key, new_value):
+        self.qdng.find(path).set(key, str(new_value))
+        
+    def define_wavefunction(self, wfp):
+        if wfp['type'] == 'file':
+            wfel = et.Element('wf')
+            wfel.set('file', wfp['file'])
+            
+        elif wfp['type'] == 'LC':
+            wfel = et.Element('wf', name=wfp['type'])
+            if 'normalize' in wfp.keys() and wfp['normalize']: wfel.set('normalize', 'true')
+            for ind in range(wfp['states']):
+                wfstate = et.SubElement(wfel, 'wf'+str(ind))
+                wfstate.set('file', wfp['file'][ind])
+            
+        elif wfp['type'] == 'Multistate':
+            wfel = et.Element('wf', name=wfp['type'])
+            wfel.set('states', str(wfp['states'])) # hamiltonian define it later
+            if 'normalize' in wfp.keys(): wfel.set('normalize', 'true')
+            
+            for ii, index in enumerate(wfp['index']):
+                wfstate = et.SubElement(wfel, 'wf'+str(index), file=str(wfp['file'][ii]))
+                if 'coeff2' in wfp.keys(): wfstate.set('coeff2', wfp['coeff2'][ii])
+        else:
+            raise SyntaxError('Wavefunction type not defined.')
+        self._wavefunction = wfel
+        return wfel
+    
+    # %% 
+    """ Programs """
+    def program(self, ptype, program_parameters, wf_parameters):
         """ Main program for the calculation. Either propagation or eigenfunction derivation.
                 
         Args:
             ptype (string) type of program:
             _either 'propa' or 'eigen'
-            program_params (dict) program parameters dictionary:
+            program_parameters (dict) program parameters dictionary:
             _format: {'dt':num, 'steps':num, 'directory':str,'Nef':num, 'conv':num }
-            wf_params (dict) wavefunction parameters dictionary:
+            wf_parameters (dict) wavefunction parameters dictionary:
             _format: {'name':str, 'states':num, 'file':[strs, ], 'normalize':True or None}
             
         """
-        # %% PROPA
-        if not ptype in ['propa','eigen']:
-            raise SyntaxError('Choose an appropriate program!')  
-        # Make the self.program lxml element
-        self.prog = dict2elem(program_params, ptype)
-        # append to the root, qdng
-        self.qdng.append( self.prog )
-        
-        # %% WAVEFUNCTION 
-        if not wf_params:
-            raise SyntaxError('Provide wavefunction parameters.')
-        self.wavefunc = wfun_elem( wf_params) # save wavefunction part to be appended after propagation
-        # self.prog.append(self.wavefunc) 
+        '''MAIN PROGRAM'''
+        if not ptype in ['propa','eigen']: raise SyntaxError('Program not defined.')  
+        self._program = subelem(self.qdng, program_parameters, ptype )
+        # Create self._program as a lxml child element of qdng
+        '''WAVEFUNCTION'''
+        self.define_wavefunction(wf_parameters)
+        # define wavefunction parameters
         
-    # %% Operators
-        # %% Propagator
+    prog = typed_property('program')    
+    wavefunc = typed_property('wavefunction')
+    
+    # %% 
+    """ Operators """
+    def def_hamiltonian(self, Hp):    
+        Hel = et.SubElement(self._propagation, 'hamiltonian')
+        # Create a lxml element to be appended to the self.propag 
+        
+        if Hp['type'] == 'Sum': 
+            Hel.set('name', Hp['type'])
+            self.states = 1
+            [subelem(Hel, opes) for opes in Hp['Opes']]
+            # set hamiltonian of Sum type, creating subelements for each operator
+        elif Hp['type'] == 'Multistate':
+            Hel.set('name', Hp['type'])
+            self.states = 0
+            if None == Hp['Mels']:
+                raise SyntaxError('Include states for the Multistate hamiltonian!')
+            else:
+                for mel in Hp['Mels'][:]:
+                    # iterate through Hamiltonian matrix elements (mel)
+                    self.states += 1
+                    if len(mel['head'])<3: # easy way to set Hamiltonian matrix element 'mi.i'
+                        mel['head'] = (f"m{mel['head'][1]}.{mel['head'][1]}")
+                    elif len(mel['head'])==3:
+                        mel['head'] = (f"m{mel['head'][1]}.{mel['head'][2]}")
+                    branch = subelem(Hel, mel)
+                    if 'Opes' in  mel.keys():
+                        for ind in range(len(mel['Opes'])):
+                            branch.append( dict2elem(mel['Opes'][ind])) 
+        self._hamiltonian = Hel
+        
+    # %% 
+    ''' Propagator '''
     def propagation(self, name, hamilt_params):
         """ Method for the wavefunction propagation. Return a etree.SubElement of previous defined program.
         
         Args:
             name (string) name of the propagation method:
                 *GSPO, Cheby, *SIL, *Arnoldi (*not defined yet)
             hamilt_params (dict) parameters dictionary for the required Cheby hamiltonian
@@ -188,97 +247,91 @@
             _type in ('Sum', 'Multistate', )
             _matrix elements for multistate, see hamilt_elem() function for format
             
         """
         # Chebychev propagator
         if name == 'Cheby':# requires hamiltonian
             # create the propagator subelement of the program
-            self.propag = et.SubElement(self.prog, 'propagator', name=name)
-            # include the hamiltonian as a subelement of propag
-            self.hamilt = hamilt_elem(self.propag, hamilt_params) 
-            try:
-                self.prog.append( self.wavefunc ) # append wavefunction after the propagation
-            except:
-                raise SyntaxError('Wavefunction was not properly defined for propa.')    
+            self._propagation = et.SubElement(self._program, 'propagator', name=name)
+            self.def_hamiltonian(hamilt_params)
+            # define hamiltonian 
+            self._wavefunction.set('states', str(self.states))
+            # change wavefunction states based on hamiltonian matrix
         else:
             raise SyntaxError('Propagator type not defined.')
         # others propagators
-        
-    def addfilter(self, ftype, params):
-        
+        try:
+            self._program.append( self._wavefunction ) # append wavefunction after the propagation
+        except:
+            raise SyntaxError('Wavefunction was not properly defined for propa.')    
+
+    propag = typed_property('propagation')
+    hamilt = typed_property('hamiltonian')
+    
+    def def_filterpost(self, filter_list):
+        # Define the filterpost operation, must be called after propagation
+        filterpost = et.Element('filterpost')
+        for dic in filter_list:
+            for opes, values in dic.items():
+                for keys in values.keys():
+                    values[keys] = str(values[keys])
+                    # update values to string to satisfy SubElement function
+                if opes.startswith('m'):
+                    et.SubElement(filterpost.getchildren()[-1], str(opes), values)
+                    # m_elements are child of last filter operator
+                else:
+                    et.SubElement(filterpost, str(opes), values)
+        self._program.append(filterpost)
+        return filterpost
+    
+    def filter(self, ftype, params):
+        # add filter to calculation
         if ftype == 'filterpost':
-            if not isinstance(params, list):
-                params = [params]
-            self.prog.append(filterpost(params))
-        
-    def writexml(self, file_name='test_file', text=False):
-        """ Write the constructed lxml element to a XML file.
-        """
-        tree = et.ElementTree(self.qdng)
-        if file_name.endswith('.txt'): 
-            text = not text 
-            file_name = file_name.strip('.txt')
-        tree.write(file_name + ('.txt' if text else '.xml'), pretty_print=True)
-        
+            if not isinstance(params, list): params = [params]
+            self._filterpost = self.def_filterpost(params)    
+            
     
+    filterpost = typed_property('filterpost')
+        
 # %% Name == Main 
 if __name__ == "__main__":
     
-    # dt, steps = 20, 1000
-    # propag, hamilt = 'Cheby', 'Sum'
-    # Nef, conv = 20, 1e-9
-    # name_T, name_V = "GridNablaSq", "GridPotential"
-    # mass, pot_file = 2000, 'pot_Vg'
-    # directory = 'efs_g'
-    # wf_file = 'wfguess'
-    # file_name='teste_dt_'
-    # key = 'T'
+    dt, steps = 20, 1000
+    propag, hamilt = 'Cheby', 'Sum'
+    Nef, conv = 20, 1e-9
+    name_T, name_V = "GridNablaSq", "GridPotential"
+    mass, pot_file = 2000, 'pot_Vg'
+    directory = 'efs_g'
+    wf_file = 'wfguess'
+    file_name='teste_dt_'
+    key = 'T'
 
-    # nparams = {'dt':dt, 'steps':steps, 'directory':directory,'Nef':Nef, 'conv':conv }
+    nparams = {'dt':1, 'steps':int(1000), 'dir':'efs_g', 'Nef':20, 'conv':1e-11 } 
    
-    # T00 = {'head':'T', 'name':name_T, 'mass':mass, 'key':'T'}
-    # V00 = {'head':'V', 'name':name_V, 'file':pot_file}
-    # m00 = {'head':'m0.0', 'name':'Sum', 'Opes':[T00, V00]} 
-    # T11 = {'head':'T', 'ref':'T'}
-    # V11 = {'head':'V', 'name':name_V, 'file':pot_file}
-    # m11 = {'head':'m1.1', 'name':'Sum', 'Opes':[T11, V11]} 
-    # m10 = {'head':'m1.0', 'name':'GridDipole', 'file':'mu', 'laser':'Et', 'Opes':[]} 
-
-    # Hparams = {'type':'Multistate', 'Mels':[m00,m11,m10]} 
-    # Hsum = {'type':'Sum', 'Opes':[T00, V00]} 
-    # WFparams = {'type':'Multistate', 'states':3, 'file':['ef'+str(i) for i in range(3)], 
-    #             'normalize':True}
-    # #%%
-    # struct = InpXML()
-    # struct.program('eigen', nparams, WFparams)
-    # struct.propagation('Cheby', Hparams)
-    # struct.writexml(text=True)
-    # '''
-    # # find if theres a way to obtain the simplified version in a text file
-    # # put this script in a higher folder, to be easily accessed for other projects
-    # '''
-    
-    # printx(struct.qdng)
-
-    mCO = 1240 
-    # printx(struct.qdng)
-    eigpar = {'dt':1, 'steps':int(1000), 'dir':'efs_g', 'Nef':20, 'conv':1e-11 }
-
-    T = {'head':'T', 'name':"GridNablaSq", 'mass':mCO}
-    Vg = {'head':'V', 'name':"GridPotential", 'file':'pot_Vg'}
-    Ve = {'head':'V', 'name':"GridPotential", 'file':'pot_Ve'}
-    mel = {'head':'m0.0', 'name':'Sum', 'Opes':[T, Vg]}
-
-    Hparams = {'type':'Sum', 'Mels':mel} 
-    WFpar = {'type':'file', 'states':1, 'file':'wfguess', 'normalize':False}
-
-    # eigx = InpXML()
-    # eigx.program('eigen', eigpar, WFpar)
-    # eigx.propagation('Cheby', Hparams)
-    # eigx.show()
-    #%% 
-    propapar = {'dt': 0.165697, 'steps': 500, 'wcycle': 100, 'dir': 'propa_files', 'nfile': 'norm'}
+    T00 = {'head':'T', 'name':name_T, 'mass':mass, 'key':'T'}
+    V00 = {'head':'V', 'name':name_V, 'file':pot_file}
+    m00 = {'head':'m0', 'name':'Sum', 'Opes':[T00, V00]} 
+    T11 = {'head':'T', 'ref':'T'}
+    V11 = {'head':'V', 'name':name_V, 'file':pot_file}
+    m11 = {'head':'m1', 'name':'Sum', 'Opes':[T11, V11]} 
+    m22 = {'head':'m2', 'name':'Sum', 'Opes':[T11, V11]} 
+    m10 = {'head':'m10', 'name':'GridDipole', 'file':'mu', 'laser':'Et', 'Opes':[]} 
+
+    Hparams = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
+    Hsum = {'type':'Sum', 'Opes':[T00, V00, T00]} 
+    wf, ef, vib =   [1, ], ['Sig0',], [1, ] # args['wf'], args['ef'], , args['vib'] #
+    WFparams = {'type':'Multistate', 'states':'1',
+             'file':["MgH/efs_{}/ef_{}".format(ef[i], vib[i]) for i in range(len(ef))], 
+             'index':[wf[i] for i in range(len(wf))], 'normalize':True}
+    filteropes = [{'expeconly':{'name':'Multistate', 'states':WFparams['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
+                   'm{}'.format(ind):{'name':'GridPotential', 'file':'MgH/mu/mu_Sig0Sig1'}}
+                   for ind in [2.1,] ]
+    #%%
     prop = InpXML()
-    prop.program('propa', propapar, WFpar)
+    prop.program('propa', nparams, WFparams)
     prop.propagation('Cheby', Hparams)
-    prop.addfilter('filterpost', {'expeconly':{'name':'Flux', 'int':'True'}})
-    prop.show()
+    prop.filter('filterpost', filteropes)
+
+    prop.show
+    # prop.writexml(txt=True)
+        
+
```

### Comparing `pqinput-0.0.2/pyproject.toml` & `pqinput-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://gitlab.fysik.su.se/lucas.borges/pqinput"
+"Homepage" = "https://gitlab.fysik.su.se/lucas.borges/pqinput"
```

### Comparing `pqinput-0.0.2/setup.py` & `pqinput-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.2",
+    version = "0.0.3",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
-    description = ("additional functions for QDng calculations preparations."),
+    description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
     long_description=read('README.md'),
     classifiers=[
-        "Development Status :: 2 - Pre-Alpha",
+        "Development Status :: 3 - Pre-Alpha",
         "Topic :: Utilities",
     ],
     python_requires='>=3.6',
 )
```

