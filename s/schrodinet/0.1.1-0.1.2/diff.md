# Comparing `tmp/schrodinet-0.1.1.tar.gz` & `tmp/schrodinet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/schrodinet-0.1.1.tar", last modified: Tue Mar 31 15:40:03 2020, max compression
+gzip compressed data, was "/home/nico/Schrodinet/dist/.tmp-750ta10r/schrodinet-0.1.2.tar", last modified: Mon May  8 09:21:41 2023, max compression
```

## Comparing `schrodinet-0.1.1.tar` & `schrodinet-0.1.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2020-03-31 15:40:03.000000 schrodinet-0.1.1/
--rw-rw-r--   0 nico      (1000) nico      (1000)    11359 2020-03-18 15:25:39.000000 schrodinet-0.1.1/LICENSE
--rw-rw-r--   0 nico      (1000) nico      (1000)       35 2020-03-18 15:25:39.000000 schrodinet-0.1.1/MANIFEST.in
--rw-rw-r--   0 nico      (1000) nico      (1000)     3756 2020-03-31 15:40:03.000000 schrodinet-0.1.1/PKG-INFO
--rw-rw-r--   0 nico      (1000) nico      (1000)     2405 2020-03-19 10:52:06.000000 schrodinet-0.1.1/README.md
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet/
--rw-rw-r--   0 nico      (1000) nico      (1000)      168 2020-03-18 15:25:39.000000 schrodinet-0.1.1/schrodinet/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)       22 2020-03-31 15:39:00.000000 schrodinet-0.1.1/schrodinet/__version__.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet/sampler/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2020-03-18 15:25:39.000000 schrodinet-0.1.1/schrodinet/sampler/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3911 2020-03-18 15:25:39.000000 schrodinet-0.1.1/schrodinet/sampler/hamiltonian.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     4350 2020-03-30 16:06:25.000000 schrodinet-0.1.1/schrodinet/sampler/metropolis.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      461 2020-03-18 15:25:39.000000 schrodinet-0.1.1/schrodinet/sampler/sampler_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1834 2020-03-30 16:06:25.000000 schrodinet-0.1.1/schrodinet/sampler/walkers.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet/solver/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2020-03-18 15:25:39.000000 schrodinet-0.1.1/schrodinet/solver/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1054 2020-03-18 15:25:39.000000 schrodinet-0.1.1/schrodinet/solver/plot_data.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    16735 2020-03-19 08:14:20.000000 schrodinet-0.1.1/schrodinet/solver/plot_potential.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5456 2020-03-30 16:06:25.000000 schrodinet-0.1.1/schrodinet/solver/solver_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     6261 2020-03-31 15:23:09.000000 schrodinet-0.1.1/schrodinet/solver/solver_potential.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     1943 2020-03-30 16:06:25.000000 schrodinet-0.1.1/schrodinet/solver/torch_utils.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet/wavefunction/
--rw-rw-r--   0 nico      (1000) nico      (1000)        0 2020-03-18 15:25:39.000000 schrodinet-0.1.1/schrodinet/wavefunction/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)      615 2020-03-18 15:25:39.000000 schrodinet-0.1.1/schrodinet/wavefunction/mesh_utils.py
--rw-rw-r--   0 nico      (1000) nico      (1000)    13176 2020-03-30 16:06:25.000000 schrodinet-0.1.1/schrodinet/wavefunction/rbf.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     5231 2020-03-30 16:06:25.000000 schrodinet-0.1.1/schrodinet/wavefunction/wf_base.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2455 2020-03-31 13:13:16.000000 schrodinet-0.1.1/schrodinet/wavefunction/wf_potential.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     2359 2020-03-18 15:26:39.000000 schrodinet-0.1.1/schrodinet/wavefunction/wf_potential_2d.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet.egg-info/
--rw-rw-r--   0 nico      (1000) nico      (1000)     3756 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet.egg-info/PKG-INFO
--rw-rw-r--   0 nico      (1000) nico      (1000)      923 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet.egg-info/SOURCES.txt
--rw-rw-r--   0 nico      (1000) nico      (1000)        1 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet.egg-info/dependency_links.txt
--rw-rw-r--   0 nico      (1000) nico      (1000)        1 2020-03-19 08:07:12.000000 schrodinet-0.1.1/schrodinet.egg-info/not-zip-safe
--rw-rw-r--   0 nico      (1000) nico      (1000)      216 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet.egg-info/requires.txt
--rw-rw-r--   0 nico      (1000) nico      (1000)       17 2020-03-31 15:40:03.000000 schrodinet-0.1.1/schrodinet.egg-info/top_level.txt
--rw-rw-r--   0 nico      (1000) nico      (1000)      344 2020-03-31 15:40:03.000000 schrodinet-0.1.1/setup.cfg
--rw-rw-r--   0 nico      (1000) nico      (1000)     1747 2020-03-31 12:19:39.000000 schrodinet-0.1.1/setup.py
-drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2020-03-31 15:40:03.000000 schrodinet-0.1.1/tests/
--rw-rw-r--   0 nico      (1000) nico      (1000)       24 2020-03-18 15:25:39.000000 schrodinet-0.1.1/tests/__init__.py
--rw-rw-r--   0 nico      (1000) nico      (1000)     3360 2020-03-19 08:11:57.000000 schrodinet-0.1.1/tests/test_ho1d.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-05-08 09:21:41.953836 schrodinet-0.1.2/
+-rw-rw-r--   0 nico      (1000) nico      (1000)    11359 2023-05-08 09:12:04.000000 schrodinet-0.1.2/LICENSE
+-rw-rw-r--   0 nico      (1000) nico      (1000)       35 2023-05-08 09:12:04.000000 schrodinet-0.1.2/MANIFEST.in
+-rw-rw-r--   0 nico      (1000) nico      (1000)       55 2023-05-08 09:12:04.000000 schrodinet-0.1.2/NOTICE
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3375 2023-05-08 09:21:41.953836 schrodinet-0.1.2/PKG-INFO
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2564 2023-05-08 09:12:04.000000 schrodinet-0.1.2/README.md
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-05-08 09:21:41.945831 schrodinet-0.1.2/schrodinet/
+-rw-rw-r--   0 nico      (1000) nico      (1000)      168 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)       22 2023-05-08 09:17:59.000000 schrodinet-0.1.2/schrodinet/__version__.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-05-08 09:21:41.949833 schrodinet-0.1.2/schrodinet/sampler/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/sampler/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3911 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/sampler/hamiltonian.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     4350 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/sampler/metropolis.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      461 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/sampler/sampler_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1834 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/sampler/walkers.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-05-08 09:21:41.949833 schrodinet-0.1.2/schrodinet/solver/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/solver/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1186 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/solver/plot_data.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    17498 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/solver/plot_potential.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5456 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/solver/solver_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     6261 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/solver/solver_potential.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1943 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/solver/torch_utils.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-05-08 09:21:41.949833 schrodinet-0.1.2/schrodinet/wavefunction/
+-rw-rw-r--   0 nico      (1000) nico      (1000)        0 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/wavefunction/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)      615 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/wavefunction/mesh_utils.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)    13176 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/wavefunction/rbf.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     5231 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/wavefunction/wf_base.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2455 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/wavefunction/wf_potential.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     2359 2023-05-08 09:12:04.000000 schrodinet-0.1.2/schrodinet/wavefunction/wf_potential_2d.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-05-08 09:21:41.949833 schrodinet-0.1.2/schrodinet.egg-info/
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3375 2023-05-08 09:21:41.000000 schrodinet-0.1.2/schrodinet.egg-info/PKG-INFO
+-rw-rw-r--   0 nico      (1000) nico      (1000)      930 2023-05-08 09:21:41.000000 schrodinet-0.1.2/schrodinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 nico      (1000) nico      (1000)        1 2023-05-08 09:21:41.000000 schrodinet-0.1.2/schrodinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 nico      (1000) nico      (1000)        1 2023-05-08 09:15:34.000000 schrodinet-0.1.2/schrodinet.egg-info/not-zip-safe
+-rw-rw-r--   0 nico      (1000) nico      (1000)      216 2023-05-08 09:21:41.000000 schrodinet-0.1.2/schrodinet.egg-info/requires.txt
+-rw-rw-r--   0 nico      (1000) nico      (1000)       17 2023-05-08 09:21:41.000000 schrodinet-0.1.2/schrodinet.egg-info/top_level.txt
+-rw-rw-r--   0 nico      (1000) nico      (1000)      344 2023-05-08 09:21:41.953836 schrodinet-0.1.2/setup.cfg
+-rw-rw-r--   0 nico      (1000) nico      (1000)     1747 2023-05-08 09:12:04.000000 schrodinet-0.1.2/setup.py
+drwxrwxr-x   0 nico      (1000) nico      (1000)        0 2023-05-08 09:21:41.949833 schrodinet-0.1.2/tests/
+-rw-rw-r--   0 nico      (1000) nico      (1000)       24 2023-05-08 09:12:04.000000 schrodinet-0.1.2/tests/__init__.py
+-rw-rw-r--   0 nico      (1000) nico      (1000)     3360 2023-05-08 09:12:04.000000 schrodinet-0.1.2/tests/test_ho1d.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `schrodinet-0.1.1/LICENSE` & `schrodinet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/README.md` & `schrodinet-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 # Schrodinet
 
 ![Build Status](https://travis-ci.com/NLESC-JCER/Schrodinet.svg?branch=master)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/38b540ecc5464901a5a48a9be037c924)](https://app.codacy.com/gh/NLESC-JCER/Schrodinet?utm_source=github.com&utm_medium=referral&utm_content=NLESC-JCER/Schrodinet&utm_campaign=Badge_Grade_Dashboard)
 
-Solving the Schrodinger equations in 1, 2 or 3D  using quantum monte carlo and radial basis function neural network to encode the wavefunction.
+Quantum Monte-Carlo Simulations of one-dimensional problem using Radial Basis Functions Neural Networks.
+<p align="center">
+<img src="./pics/morse.gif" title="Optimization of the wave function">
+</p>
+
+
+## Installation
+
+Clone the repo and `pip` insatll the code
+
+```
+git clone https://github.com/NLESC-JCER/Schrodinet/
+cd Schrodinet
+pip install .
+```
 
 ## Harmonic Oscillator in 1D
 
 The script below illustrates how to optimize the wave function of the one-dimensional harmonic oscillator.
 
 ```python
 import torch
@@ -24,15 +38,14 @@
 
 
 def ho1d_sol(pos):
     '''Analytical solution of the 1D harmonic oscillator.'''
     return torch.exp(-0.5*pos**2)
 
 # Define the domain and the number of RBFs
-domain, ncenter = {'min': -5., 'max': 5.}, 11
 
 # wavefunction
 wf = Potential(pot_func, domain, ncenter, fcinit='random', nelec=1, sigma=0.5)
 
 # sampler
 sampler = Metropolis(nwalkers=1000, nstep=2000,
                      step_size=1., nelec=wf.nelec,
@@ -43,15 +56,15 @@
 scheduler = optim.lr_scheduler.StepLR(opt, step_size=100, gamma=0.75)
 
 # Solver
 solver = SolverPotential(wf=wf, sampler=sampler,
                          optimizer=opt, scheduler=scheduler)
 
 # Train the wave function
-plotter = plotter1d(wf, domain, 100, sol=ho1d_sol) 
+plotter = plotter1d(wf, domain, 100, sol=ho1d_sol)
 solver.run(300, loss='variance', plot=plotter, save='model.pth')
 
 # Plot the final wave function
 plot_results_1d(solver, domain, 100, ho1d_sol, e0=0.5, load='model.pth')
 ```
 
 After otpimization the following trajectory can easily be generated :
```

### Comparing `schrodinet-0.1.1/schrodinet/sampler/hamiltonian.py` & `schrodinet-0.1.2/schrodinet/sampler/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/sampler/metropolis.py` & `schrodinet-0.1.2/schrodinet/sampler/metropolis.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/sampler/walkers.py` & `schrodinet-0.1.2/schrodinet/sampler/walkers.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/solver/plot_data.py` & `schrodinet-0.1.2/schrodinet/solver/plot_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import matplotlib.pyplot as plt
 
 
-def plot_observable(obs_dict, e0=None, ax=None):
+def plot_observable(obs_dict, e0=None, ax=None, xlim=None, ylim=None):
     '''Plot the observable selected.
 
     Args:
         obs_dict : dictioanry of observable
     '''
     show_plot = False
     if ax is None:
@@ -28,17 +28,22 @@
 
     # get the mean value
     energy = np.mean(data, 1)
     print("Energy : %f " % np.mean(energy))
 
     # plot
     ax.fill_between(epoch, emin, emax, alpha=0.5, color='#4298f4')
-    ax.plot(epoch, energy, color='#144477')
+    ax.plot(epoch, energy, lw=2, color='#144477')
     if e0 is not None:
         ax.axhline(e0, color='black', linestyle='--')
 
     ax.grid()
-    ax.set_xlabel('Number of epoch')
+    ax.set_xlabel('Number of epochs')
     ax.set_ylabel('Energy')
 
+    if xlim is not None:
+        ax.set_xlim(xlim)
+    if ylim is not None:
+        ax.set_ylim(ylim)
+
     if show_plot:
         plt.show()
```

### Comparing `schrodinet-0.1.1/schrodinet/solver/plot_potential.py` & `schrodinet-0.1.2/schrodinet/solver/plot_potential.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import torch
 from torch.autograd import Variable
 import numpy as np
-
+import matplotlib.pylab as pl
 import matplotlib.pyplot as plt
 from matplotlib import cm
 try:
     from skimage import measure
 except ImportError:
     print('skimage  required for 3d plot')
 
@@ -103,20 +103,23 @@
         '''Update the plot.'''
 
         vp = self.wf(self.POS).detach().numpy()
         vp /= np.max(vp)
         self.lwf.set_ydata(vp)
 
         if self.plot_weight:
-            self.pweight.set_xdata(self.wf.rbf.centers.detach().numpy())
-            self.pweight.set_ydata(self.wf.fc.weight.detach().numpy().T)
+            self.pweight.set_xdata(
+                self.wf.rbf.centers.detach().numpy())
+            self.pweight.set_ydata(
+                self.wf.fc.weight.detach().numpy().T)
 
         if self.plot_grad:
             if self.wf.fc.weight.requires_grad:
-                self.pgrad.set_xdata(self.wf.rbf.centers.detach().numpy())
+                self.pgrad.set_xdata(
+                    self.wf.rbf.centers.detach().numpy())
                 data = (self.wf.fc.weight.grad.detach().numpy().T)**2
                 data /= np.linalg.norm(data)
                 self.pgrad.set_ydata(data)
 
         # self.fig.canvas.draw()
         plt.draw()
         self.fig.canvas.flush_events()
@@ -127,16 +130,17 @@
     def _save_pic(self):
         fname = 'image_%03d.png' % self.iter
         fname = os.path.join(self.save, fname)
         plt.savefig(fname)
         self.iter += 1
 
 
-def plot_wf_1d(net, domain, res, grad=False, hist=False, pot=True, sol=None,
-               ax=None, load=None):
+def plot_wf_1d(net, domain, res, grad=False,
+               hist=False, pot=True, sol=None,
+               gaussians=True, ax=None, load=None):
     '''Plot a 1D wave function.
 
     Args:
         net : network object
         grad : plot gradient
         hist : plot histogram of the data points
         sol : callabale of the solution
@@ -157,21 +161,21 @@
     X = Variable(torch.linspace(
         domain['min'], domain['max'], res).view(res, 1))
     X.requires_grad = True
     xn = X.detach().numpy().flatten()
 
     if callable(sol):
         vs = sol(X).detach().numpy()
-        ax.plot(xn, vs, color='#b70000', linewidth=4,
+        ax.plot(xn, vs, color='grey', linewidth=2,
                 linestyle='--', label='solution')
 
     vals = net.wf(X)
     vn = vals.detach().numpy().flatten()
     vn /= np.max(vn)
-    ax.plot(xn, vn, color='black', linewidth=2, label='DeepQMC')
+    ax.plot(xn, vn, color='black', linewidth=2, label='Schrodinet')
 
     if pot:
         pot = net.wf.nuclear_potential(X).detach().numpy()
         ax.plot(xn, pot, color='black', linestyle='--')
 
     if grad:
         kin = net.wf.kinetic_energy(X)
@@ -180,28 +184,42 @@
         ax.plot(xn, kin.detach().numpy(), label='kinetic')
         ax.plot(xn, h, label='hessian')
 
     if hist:
         pos = net.sample(ntherm=-1)
         ax.hist(pos.detach().numpy(), density=False)
 
-    ax.set_ylim((np.min(pot), 1))
-    ax.grid()
+    if gaussians:
+        rbfs = net.wf.rbf(X)
+        rbfs *= net.wf.fc.weight
+        rbfs = rbfs.T
+
+        line_colors = pl.cm.rainbow(np.linspace(0, 1, len(rbfs)))
+
+        for y, c in zip(rbfs, line_colors):
+            ax.plot(xn, y.detach().numpy(), color=c)
+            ax.fill_between(xn, y.detach().numpy(),
+                            alpha=0.1, color=c)
+
+    ax.set_ylim((np.min(pot)-0.05, 1.25))
+
+    ax.axis('off')
     ax.set_xlabel('X')
     if load is None:
         ax.set_ylabel('Wavefuntion')
     else:
         ax.set_ylabel('Wavefuntion %d epoch' % epoch)
-    ax.legend()
 
     if show_plot:
         plt.show()
 
 
-def plot_results_1d(net, domain, res, sol=None, e0=None, load=None):
+def plot_results_1d(net, domain, res, iter=None,
+                    sol=None, e0=None, load=None,
+                    xlim=None, ylim=None):
     ''' Plot the summary of the results for a 1D problem.
 
     Args:
         net : network object
         obs_dict : dict containing the obserable
         sol : callable of the solutions
         e0 : energy of the solution
@@ -209,18 +227,24 @@
         res : number of points in the x axis
     '''
     plt.ioff()
     fig = plt.figure()
     ax0 = fig.add_subplot(211)
     ax1 = fig.add_subplot(212)
 
-    plot_wf_1d(net, domain, res, sol=sol, hist=False, ax=ax0, load=load)
-    plot_observable(net.obs_dict, e0=e0, ax=ax1)
+    plot_wf_1d(net, domain, res, sol=sol,
+               hist=False, ax=ax0, load=load)
+    plot_observable(net.obs_dict, e0=e0, ax=ax1,
+                    xlim=xlim, ylim=ylim)
 
-    plt.show()
+    if iter is not None:
+        fname = 'image/image_%03d.png' % iter
+        plt.savefig(fname)
+    else:
+        plt.show()
 
 
 ##############################################################################
 # 2D routnines
 ##############################################################################
 
 def plot_wf_2d(net, domain, res, sol=None):
@@ -287,15 +311,16 @@
         self.POS.requires_grad = True
 
         pos = self.POS.detach().numpy()
         self.xx = pos[:, 0].reshape(res[0], res[1])
         self.yy = pos[:, 1].reshape(res[0], res[1])
 
         if callable(sol):
-            vs = sol(self.POS).view(self.res[0], self.res[1]).detach().numpy()
+            vs = sol(self.POS).view(
+                self.res[0], self.res[1]).detach().numpy()
             vs /= np.linalg.norm(vs)
             self.ax.plot_wireframe(self.xx, self.yy, vs,
                                    color='black', linewidth=1)
 
         if pot:
             vs = wf.nuclear_potential(self.POS).view(
                 self.res[0], self.res[1]).detach().numpy()
@@ -454,15 +479,16 @@
     dy = (domain['ymax']-domain['ymin']) / (res[1]-1)
     dz = (domain['zmax']-domain['zmin']) / (res[2]-1)
     spacing_vals = (dx, dy, dz)
 
     if hist:
         pos = net.sample().detach().numpy()
         for ielec in range(net.wf.nelec):
-            ax.scatter(pos[:, ielec*3], pos[:, ielec*3+1], pos[:, ielec*3+2])
+            ax.scatter(pos[:, ielec*3],
+                       pos[:, ielec*3+1], pos[:, ielec*3+2])
 
     if callable(sol):
 
         vals = sol(POS)
         vs = vals.detach().numpy().reshape(res[0], res[1], res[2])
         verts, faces, normals, _ = measure.marching_cubes_lewiner(
             vs, isoval, spacing=spacing_vals)
```

### Comparing `schrodinet-0.1.1/schrodinet/solver/solver_base.py` & `schrodinet-0.1.2/schrodinet/solver/solver_base.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/solver/solver_potential.py` & `schrodinet-0.1.2/schrodinet/solver/solver_potential.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/solver/torch_utils.py` & `schrodinet-0.1.2/schrodinet/solver/torch_utils.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/wavefunction/mesh_utils.py` & `schrodinet-0.1.2/schrodinet/wavefunction/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/wavefunction/rbf.py` & `schrodinet-0.1.2/schrodinet/wavefunction/rbf.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/wavefunction/wf_base.py` & `schrodinet-0.1.2/schrodinet/wavefunction/wf_base.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/wavefunction/wf_potential.py` & `schrodinet-0.1.2/schrodinet/wavefunction/wf_potential.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet/wavefunction/wf_potential_2d.py` & `schrodinet-0.1.2/schrodinet/wavefunction/wf_potential_2d.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/schrodinet.egg-info/SOURCES.txt` & `schrodinet-0.1.2/schrodinet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 MANIFEST.in
+NOTICE
 README.md
 setup.cfg
 setup.py
 schrodinet/__init__.py
 schrodinet/__version__.py
 schrodinet.egg-info/PKG-INFO
 schrodinet.egg-info/SOURCES.txt
```

### Comparing `schrodinet-0.1.1/setup.py` & `schrodinet-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `schrodinet-0.1.1/tests/test_ho1d.py` & `schrodinet-0.1.2/tests/test_ho1d.py`

 * *Files identical despite different names*

