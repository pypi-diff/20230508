# Comparing `tmp/hydromass-0.4.tar.gz` & `tmp/hydromass-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydromass-0.4.tar", last modified: Mon Mar 27 07:24:50 2023, max compression
+gzip compressed data, was "hydromass-0.5.tar", last modified: Mon May  8 20:46:26 2023, max compression
```

## Comparing `hydromass-0.4.tar` & `hydromass-0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-03-27 07:24:50.920638 hydromass-0.4/
--rwxr-xr-x   0 deckert    (501) staff       (20)       24 2022-01-11 19:49:57.000000 hydromass-0.4/MANIFEST.in
--rw-r--r--   0 deckert    (501) staff       (20)      285 2023-03-27 07:24:50.920483 hydromass-0.4/PKG-INFO
--rwxr-xr-x   0 deckert    (501) staff       (20)     1590 2022-02-28 08:40:15.000000 hydromass-0.4/README.md
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-03-27 07:24:50.919231 hydromass-0.4/hydromass/
--rwxr-xr-x   0 deckert    (501) staff       (20)      316 2023-03-23 07:01:39.000000 hydromass-0.4/hydromass/__init__.py
--rwxr-xr-x   0 deckert    (501) staff       (20)      265 2023-03-23 07:01:39.000000 hydromass-0.4/hydromass/constants.py
--rw-r--r--   0 deckert    (501) staff       (20)    10052 2023-03-23 07:01:39.000000 hydromass-0.4/hydromass/contour.py
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-03-27 07:24:50.920269 hydromass-0.4/hydromass/data/
--rwxr-xr-x   0 deckert    (501) staff       (20)    95040 2022-01-11 19:49:50.000000 hydromass-0.4/hydromass/data/coolfunc_table.fits
--rwxr-xr-x   0 deckert    (501) staff       (20)      229 2022-01-11 19:49:50.000000 hydromass-0.4/hydromass/data/pnt_covmat.dat
--rwxr-xr-x   0 deckert    (501) staff       (20)       75 2022-01-11 19:49:50.000000 hydromass-0.4/hydromass/data/pnt_mean.dat
--rwxr-xr-x   0 deckert    (501) staff       (20)    26380 2023-03-23 07:01:39.000000 hydromass-0.4/hydromass/delta.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    15073 2023-03-23 07:01:39.000000 hydromass-0.4/hydromass/deproject.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    12077 2023-03-23 07:03:07.000000 hydromass-0.4/hydromass/emissivity.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    29408 2023-03-23 07:02:47.000000 hydromass-0.4/hydromass/forward.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    25175 2023-03-23 07:06:33.000000 hydromass-0.4/hydromass/functions.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    47198 2023-03-23 07:44:46.000000 hydromass-0.4/hydromass/mhyd.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    41923 2023-03-23 07:04:27.000000 hydromass-0.4/hydromass/nonparametric.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    27424 2023-03-23 07:01:39.000000 hydromass-0.4/hydromass/plots.py
--rwxr-xr-x   0 deckert    (501) staff       (20)     2778 2023-03-23 07:07:47.000000 hydromass-0.4/hydromass/pnt.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    35691 2023-03-23 07:05:48.000000 hydromass-0.4/hydromass/polytropic.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    25782 2023-03-23 07:01:39.000000 hydromass-0.4/hydromass/save.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    23565 2023-03-23 07:01:39.000000 hydromass-0.4/hydromass/tpdata.py
--rw-r--r--   0 deckert    (501) staff       (20)     3904 2023-03-23 07:14:07.000000 hydromass-0.4/hydromass/wl.py
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-03-27 07:24:50.919833 hydromass-0.4/hydromass.egg-info/
--rwxr-xr-x   0 deckert    (501) staff       (20)      285 2023-03-27 07:24:50.000000 hydromass-0.4/hydromass.egg-info/PKG-INFO
--rwxr-xr-x   0 deckert    (501) staff       (20)      622 2023-03-27 07:24:50.000000 hydromass-0.4/hydromass.egg-info/SOURCES.txt
--rwxr-xr-x   0 deckert    (501) staff       (20)        1 2023-03-27 07:24:50.000000 hydromass-0.4/hydromass.egg-info/dependency_links.txt
--rwxr-xr-x   0 deckert    (501) staff       (20)       47 2023-03-27 07:24:50.000000 hydromass-0.4/hydromass.egg-info/requires.txt
--rwxr-xr-x   0 deckert    (501) staff       (20)       10 2023-03-27 07:24:50.000000 hydromass-0.4/hydromass.egg-info/top_level.txt
--rw-r--r--   0 deckert    (501) staff       (20)       38 2023-03-27 07:24:50.920688 hydromass-0.4/setup.cfg
--rwxr-xr-x   0 deckert    (501) staff       (20)      517 2023-03-23 07:09:13.000000 hydromass-0.4/setup.py
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-08 20:46:26.596988 hydromass-0.5/
+-rwxr-xr-x   0 deckert    (501) staff       (20)       24 2023-02-08 13:10:51.000000 hydromass-0.5/MANIFEST.in
+-rw-r--r--   0 deckert    (501) staff       (20)      240 2023-05-08 20:46:26.596833 hydromass-0.5/PKG-INFO
+-rwxr-xr-x   0 deckert    (501) staff       (20)     1590 2023-02-08 13:10:51.000000 hydromass-0.5/README.md
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-08 20:46:26.595564 hydromass-0.5/hydromass/
+-rwxr-xr-x   0 deckert    (501) staff       (20)      316 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/__init__.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)      306 2023-05-04 12:45:19.000000 hydromass-0.5/hydromass/constants.py
+-rw-r--r--   0 deckert    (501) staff       (20)    10052 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/contour.py
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-08 20:46:26.596656 hydromass-0.5/hydromass/data/
+-rwxr-xr-x   0 deckert    (501) staff       (20)    95040 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/data/coolfunc_table.fits
+-rwxr-xr-x   0 deckert    (501) staff       (20)      229 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/data/pnt_covmat.dat
+-rwxr-xr-x   0 deckert    (501) staff       (20)       75 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/data/pnt_mean.dat
+-rwxr-xr-x   0 deckert    (501) staff       (20)    26380 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/delta.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    15073 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/deproject.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    12085 2023-05-04 13:22:24.000000 hydromass-0.5/hydromass/emissivity.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    29962 2023-05-04 21:32:25.000000 hydromass-0.5/hydromass/forward.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    25184 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/functions.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    49031 2023-05-05 13:55:25.000000 hydromass-0.5/hydromass/mhyd.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    42677 2023-05-05 14:56:02.000000 hydromass-0.5/hydromass/nonparametric.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    28385 2023-05-05 13:27:08.000000 hydromass-0.5/hydromass/plots.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)     2777 2023-02-08 13:10:51.000000 hydromass-0.5/hydromass/pnt.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    36243 2023-05-08 20:43:19.000000 hydromass-0.5/hydromass/polytropic.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    25837 2023-05-04 13:46:01.000000 hydromass-0.5/hydromass/save.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    24071 2023-05-04 12:45:19.000000 hydromass-0.5/hydromass/tpdata.py
+-rw-r--r--   0 deckert    (501) staff       (20)     3903 2023-05-04 12:56:59.000000 hydromass-0.5/hydromass/wl.py
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-08 20:46:26.596210 hydromass-0.5/hydromass.egg-info/
+-rw-r--r--   0 deckert    (501) staff       (20)      240 2023-05-08 20:46:26.000000 hydromass-0.5/hydromass.egg-info/PKG-INFO
+-rw-r--r--   0 deckert    (501) staff       (20)      622 2023-05-08 20:46:26.000000 hydromass-0.5/hydromass.egg-info/SOURCES.txt
+-rw-r--r--   0 deckert    (501) staff       (20)        1 2023-05-08 20:46:26.000000 hydromass-0.5/hydromass.egg-info/dependency_links.txt
+-rw-r--r--   0 deckert    (501) staff       (20)       68 2023-05-08 20:46:26.000000 hydromass-0.5/hydromass.egg-info/requires.txt
+-rw-r--r--   0 deckert    (501) staff       (20)       10 2023-05-08 20:46:26.000000 hydromass-0.5/hydromass.egg-info/top_level.txt
+-rw-r--r--   0 deckert    (501) staff       (20)       38 2023-05-08 20:46:26.597031 hydromass-0.5/setup.cfg
+-rwxr-xr-x   0 deckert    (501) staff       (20)      544 2023-05-08 20:45:21.000000 hydromass-0.5/setup.py
```

### Comparing `hydromass-0.4/README.md` & `hydromass-0.5/README.md`

 * *Files identical despite different names*

### Comparing `hydromass-0.4/hydromass/contour.py` & `hydromass-0.5/hydromass/contour.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.4/hydromass/data/coolfunc_table.fits` & `hydromass-0.5/hydromass/data/coolfunc_table.fits`

 * *Files identical despite different names*

### Comparing `hydromass-0.4/hydromass/delta.py` & `hydromass-0.5/hydromass/delta.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.4/hydromass/deproject.py` & `hydromass-0.5/hydromass/deproject.py`

 * *Files identical despite different names*

### Comparing `hydromass-0.4/hydromass/emissivity.py` & `hydromass-0.5/hydromass/emissivity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import  numpy as np
-import pymc3 as pm
+import pymc as pm
 import matplotlib.pyplot as plt
 from scipy.interpolate import interp1d
 from scipy.optimize import minimize
 
 def is_tool(name):
     """Check whether `name` is on PATH."""
 
@@ -321,19 +321,19 @@
 
         modz = pm.Model()
 
         beta_fe = 0.3
 
         with modz:
 
-            rc = pm.TruncatedNormal('rc', mu=30., sd=30., lower=0.2)
+            rc = pm.TruncatedNormal('rc', mu=30., sigma=30., lower=0.2)
 
-            norm = pm.Normal('norm', mu=0.7, sd=0.5)
+            norm = pm.Normal('norm', mu=0.7, sigma=0.5)
 
-            floor = pm.HalfNormal('floor', sd=0.2)
+            floor = pm.HalfNormal('floor', sigma=0.2)
 
             pred = floor + norm * (1. + (rads_z / rc) ** 2) ** (-beta_fe)
 
             obs = pm.Normal('obs', mu=pred, sigma=spec_data.zfe_hi[active], observed=spec_data.zfe[active])
 
             trace_z = pm.sample(return_inferencedata=True)
```

### Comparing `hydromass-0.4/hydromass/forward.py` & `hydromass-0.5/hydromass/forward.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-import pymc3 as pm
+import pymc as pm
 from .deproject import *
 from .plots import rads_more, get_coolfunc, plt
 from .constants import *
 
 # GNFW function should work both for numpy.ndarray and pymc3/theano formats
 def gnfw_pm(rad, p0, c500, gamma, alfa, beta):
     '''
@@ -673,15 +673,15 @@
         K = np.dot(prof.psfmat, Ksb)
 
     # Set up initial values
     if np.isnan(sb[0]) or sb[0] <= 0:
         testval = -10.
     else:
         testval = np.log(sb[0] / npt)
-    if np.isnan(back) or back == 0:
+    if np.isnan(back) or back <= 0 or back is None:
         testbkg = -10.
     else:
         testbkg = np.log(back)
 
     z = Mhyd.redshift
 
     transf = 4. * (1. + z) ** 2 * (180. * 60.) ** 2 / np.pi / 1e-14 * Mhyd.nhc / cgsMpc * 1e3
@@ -752,19 +752,19 @@
 
         Kdens_m = calc_density_operator(rout_m / Mhyd.amin2kpc, pardens, Mhyd.amin2kpc, withbkg=False)
 
     hydro_model = pm.Model()
 
     with hydro_model:
         # Priors for unknown model parameters
-        coefs = pm.Normal('coefs', mu=testval, sd=20, shape=npt)
+        coefs = pm.Normal('coefs', mu=testval, sigma=20, shape=npt)
 
         if fit_bkg:
 
-            bkgd = pm.Normal('bkg', mu=testbkg, sd=0.05, shape=1) # in case fit_bkg = False this is not fitted
+            bkgd = pm.Normal('bkg', mu=testbkg, sigma=0.05, shape=1) # in case fit_bkg = False this is not fitted
 
             ctot = pm.math.concatenate((coefs, bkgd), axis=0)
 
             al = pm.math.exp(ctot)
 
             pred = pm.math.dot(K, al) + bkgcounts  # Predicted number of counts per annulus
 
@@ -784,50 +784,47 @@
 
             if not Forward.fix[i]:
 
                 lim = Forward.limits[i]
 
                 if name == 'p0':
 
-                    tpar = pm.TruncatedNormal(name, mu=np.log(Forward.start[i]), sd=Forward.sd[i] / Forward.start[i],
+                    tpar = pm.TruncatedNormal(name, mu=np.log(Forward.start[i]), sigma=Forward.sd[i] / Forward.start[i],
                                                 lower=np.log(lim[0]), upper=np.log(lim[1])) #log-normal prior on normalization
 
                     modpar = pm.math.exp(tpar)
 
                 else:
 
-                    modpar = pm.TruncatedNormal(name, mu=Forward.start[i], sd=Forward.sd[i],
+                    modpar = pm.TruncatedNormal(name, mu=Forward.start[i], sigma=Forward.sd[i],
                                                 lower=lim[0], upper=lim[1]) #Gaussian prior on other parameters
             else:
 
-                dummy = pm.Normal('dummy'+name, mu=0., sd=1.)
+                dummy = pm.Normal('dummy'+name, mu=0., sigma=1.)
 
                 dummy_param = 0 * dummy + Forward.start[i]
 
                 modpar = pm.Deterministic(name, dummy_param)
 
             allpmod.append(modpar)
 
-        for RV in hydro_model.basic_RVs:
-            print(RV.name, RV.logp(hydro_model.test_point))
-
         pmod = pm.math.stack(allpmod, axis=0)
 
         dens_m = pm.math.sqrt(pm.math.dot(Kdens_m, al) / cf * transf)  # electron density in cm-3
 
         p3d = Forward.func_pm(rout_m, *pmod)
 
         # Density Likelihood
         if fit_bkg:
 
             count_obs = pm.Poisson('counts', mu=pred, observed=counts)  # counts likelihood
 
         else:
 
-            sb_obs = pm.Normal('sb', mu=pred, observed=sb, sd=esb)  # Sx likelihood
+            sb_obs = pm.Normal('sb', mu=pred, observed=sb, sigma=esb)  # Sx likelihood
 
         # Temperature model and likelihood
         if Mhyd.spec_data is not None:
 
             # Model temperature
             t3d = p3d / dens_m
 
@@ -835,37 +832,62 @@
             ei = dens_m ** 2 * t3d ** (-0.75)
 
             # Temperature projection
             flux = pm.math.dot(proj_mat, ei)
 
             tproj = pm.math.dot(proj_mat, t3d * ei) / flux
 
-            T_obs = pm.Normal('kt', mu=tproj, observed=Mhyd.spec_data.temp_x, sd=Mhyd.spec_data.errt_x)  # temperature likelihood
+            T_obs = pm.Normal('kt', mu=tproj, observed=Mhyd.spec_data.temp_x, sigma=Mhyd.spec_data.errt_x)  # temperature likelihood
 
         # SZ pressure model and likelihood
         if Mhyd.sz_data is not None:
             pfit = p3d[index_sz]
 
             P_obs = pm.MvNormal('P', mu=pfit, observed=Mhyd.sz_data.pres_sz, cov=Mhyd.sz_data.covmat_sz)  # SZ pressure likelihood
 
     tinit = time.time()
 
     print('Running MCMC...')
 
+    isjax = False
+
+    try:
+        import pymc.sampling.jax as pmjax
+
+    except ImportError:
+        print('JAX not found, using default sampler')
+
+    else:
+        isjax = True
+        import pymc.sampling.jax as pmjax
+
     with hydro_model:
 
         if find_map:
 
             start = pm.find_MAP()
 
-            trace = pm.sample(nmcmc, init='ADVI', start=start, tune=tune, return_inferencedata=True, target_accept=0.9)
+            if not isjax:
+
+                trace = pm.sample(nmcmc, init='ADVI', initvals=start, tune=tune, return_inferencedata=True, target_accept=0.9)
+
+            else:
+
+                trace = pmjax.sample_numpyro_nuts(nmcmc, init='ADVI', initvals=start, tune=tune, return_inferencedata=True,
+                                  target_accept=0.9)
 
         else:
 
-            trace = pm.sample(nmcmc, tune=tune, init='ADVI',  return_inferencedata=True, target_accept=0.9)
+            if not isjax:
+
+                trace = pm.sample(nmcmc, tune=tune, init='ADVI',  return_inferencedata=True, target_accept=0.9)
+
+            else:
+
+                trace = pmjax.sample_numpyro_nuts(nmcmc, tune=tune, return_inferencedata=True, target_accept=0.9)
 
     print('Done.')
 
     tend = time.time()
 
     print(' Total computing time is: ', (tend - tinit) / 60., ' minutes')
```

### Comparing `hydromass-0.4/hydromass/functions.py` & `hydromass-0.5/hydromass/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import scipy.special as special
-import pymc3 as pm
-import theano
-import theano.tensor as tt
+import pymc as pm
+import aesara as theano
+import aesara.tensor as tt
 
 
 class ArcTan(tt.Op):
     '''
     Theano arctan class
     '''
     itypes = [tt.dvector]
```

### Comparing `hydromass-0.4/hydromass/mhyd.py` & `hydromass-0.5/hydromass/mhyd.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,29 @@
 from .constants import *
 from .forward import *
 from .polytropic import *
 from .pnt import *
 from .nonparametric import *
 from astropy.io import fits
 import os
-import pymc3 as pm
+
+isjax = False
+
+try:
+    import pymc.sampling.jax as pmjax
+
+except ImportError:
+    print('JAX not found, using default sampler')
+
+else:
+    print('We will use the JAX sampler')
+    isjax = True
+    import pymc.sampling.jax as pmjax
+
+import pymc as pm
 from .save import *
 from .wl import WLmodel
 import arviz as az
 
 def Run_Mhyd_PyMC3(Mhyd,model,bkglim=None,nmcmc=1000,fit_bkg=False,back=None,
                    samplefile=None,nrc=None,nbetas=6,min_beta=0.6, nmore=5,
                    p0_prior=None, tune=500, dmonly=False, mstar=None, find_map=True,
@@ -80,14 +94,15 @@
     esb = prof.eprof
     rad = prof.bins
     erad = prof.ebins
     counts = prof.counts
     area = prof.area
     exposure = prof.effexp
     bkgcounts = prof.bkgcounts
+    nbin = prof.nbin
 
     nmin = 0
     nmax = len(sb)
 
     if rmin is not None:
         valid = np.where(rad>=rmin)
         sb = sb[valid]
@@ -153,22 +168,22 @@
         # K = calc_sb_operator_psf(rad, sourcereg, pars, area, exposure, psfmat) # transformation to surface brightness
 
     # Set up initial values
     if np.isnan(sb[0]) or sb[0] <= 0:
         testval = -10.
     else:
         testval = np.log(sb[0] / npt)
-    if np.isnan(back) or back == 0:
+    if np.isnan(back) or back <= 0 or back is None:
         testbkg = -10.
     else:
         testbkg = np.log(back)
 
     z = Mhyd.redshift
 
-    transf = 4. * (1. + z) ** 2 * (180. * 60.) ** 2 / np.pi / 1e-14 * Mhyd.nhc / cgsMpc * 1e3
+    transf = Mhyd.transf
 
     pardens = list_params_density(rad, sourcereg, Mhyd.amin2kpc, nrc, nbetas, min_beta)
 
     if fit_bkg:
 
         Kdens = calc_density_operator(rad, pardens, Mhyd.amin2kpc)
 
@@ -323,16 +338,15 @@
 
             err_P0_est = P0_est # 1 in ln
 
         logp0 = pm.TruncatedNormal('logp0', mu=np.log(P0_est), sigma=err_P0_est / P0_est,
                                    lower=np.log(P0_est) - err_P0_est / P0_est,
                                    upper=np.log(P0_est) + err_P0_est / P0_est)
 
-        if pnt:
-
+        if pnt :
             if pnt_model=='Angelinelli':
 
                 pnt_pars = pm.MvNormal('Pnt', mu=pnt_mean, cov=pnt_cov, shape=(1,3))
 
             if pnt_model=='Ettori':
 
                 beta_nt = pm.Normal('beta_nt', mu=0.9, sigma=0.13)
@@ -442,17 +456,40 @@
             valspec = np.where(np.logical_and(Mhyd.spec_data.rref_x_am>=rmin_spec, Mhyd.spec_data.rref_x_am<=rmax_spec))
 
             T_obs = pm.Normal('kt', mu=tproj[valspec], observed=Mhyd.spec_data.temp_x[valspec], sigma=Mhyd.spec_data.errt_x[valspec])  # temperature likelihood
 
         # SZ pressure model and likelihood
         if Mhyd.sz_data is not None:
 
-            pfit = pth[index_sz] * elongation
+            if Mhyd.sz_data.pres_sz is not None: # Fitting the pressure
+
+                pfit = pth[index_sz] * elongation
+
+                P_obs = pm.MvNormal('P', mu=pfit, observed=Mhyd.sz_data.pres_sz, cov=Mhyd.sz_data.covmat_sz)  # SZ pressure likelihood
+
+            elif Mhyd.sz_data.y_sz is not None: # Fitting the Compton y parameter
+                rin_cm, rout_cm = rin_m * cgskpc, rout_m * cgskpc
+
+                deproj = MyDeprojVol(rin_cm, rout_cm)  # r from kpc to cm
+
+                proj_vol = deproj.deproj_vol().T
+
+                area_proj = np.pi * (-(rin_cm) ** 2 + (rout_cm) ** 2)
+
+                integ = pm.math.dot(proj_vol, pth) / area_proj
+
+                y_num = y_prefactor * integ  # prefactor in cm2/keV
 
-            P_obs = pm.MvNormal('P', mu=pfit, observed=Mhyd.sz_data.pres_sz, cov=Mhyd.sz_data.covmat_sz)  # SZ pressure likelihood
+                yfit = y_num[index_sz] * elongation
+
+                if Mhyd.sz_data.psfmat is not None:
+
+                    yfit = pm.math.dot(Mhyd.sz_data.psfmat, yfit)
+
+                Y_obs = pm.MvNormal('Y', mu=yfit, observed=Mhyd.sz_data.y_sz, cov=Mhyd.sz_data.covmat_sz)
 
         if Mhyd.wl_data is not None:
 
             WLdata = Mhyd.wl_data
 
             gmodel, rm, ev = WLmodel(WLdata, model, pmod)
 
@@ -466,31 +503,47 @@
 
     with hydro_model:
 
         if find_map:
 
             start = pm.find_MAP()
 
-            trace = pm.sample(nmcmc, init=init, initvals=start, tune=tune, return_inferencedata=True,
+            if not isjax:
+
+                trace = pm.sample(nmcmc, init=init, initvals=start, tune=tune, return_inferencedata=True,
                               target_accept=target_accept)
+            else:
+
+                trace = pmjax.sample_numpyro_nuts(nmcmc, initvals=start, tune=tune, return_inferencedata=True, target_accept=target_accept)
 
         else:
 
-            trace = pm.sample(nmcmc, init=init, tune=tune, return_inferencedata=True, target_accept=target_accept)
+            if not isjax:
+
+                trace = pm.sample(nmcmc, init=init, tune=tune, return_inferencedata=True, target_accept=target_accept)
+
+            else:
+
+                trace = pmjax.sample_numpyro_nuts(nmcmc, init=init, tune=tune, return_inferencedata=True, target_accept=target_accept)
 
 
         Mhyd.ppc_sb = pm.sample_posterior_predictive(trace, var_names=['sb'])
 
         if Mhyd.spec_data is not None:
 
             Mhyd.ppc_kt = pm.sample_posterior_predictive(trace, var_names=['kt'])
 
         if Mhyd.sz_data is not None:
 
-            Mhyd.ppc_sz = pm.sample_posterior_predictive(trace, var_names=['P'])
+            # Mhyd.ppc_sz = pm.sample_posterior_predictive(trace, var_names=['P'])
+            Mhyd.ppc_sz = pm.sample_posterior_predictive(trace, var_names=['Y'])
+
+        if Mhyd.wl_data is not None:
+
+            Mhyd.ppc_wl = pm.sample_posterior_predictive(trace, var_names=['WL'])
 
         if Mhyd.wl_data is not None:
 
             Mhyd.ppc_wl = pm.sample_posterior_predictive(trace, var_names=['WL'])
 
     print('Done.')
 
@@ -582,28 +635,28 @@
     Mhyd.dmonly = dmonly
     Mhyd.mstar = mstar
     Mhyd.pnt = pnt
     if pnt:
         if pnt_model == 'Angelinelli':
             Mhyd.pnt_pars = np.array(trace.posterior['Pnt']).reshape(sc_coefs[0] * sc_coefs[1], 3)
 
-            Mhyd.pntmodel = 'Angelinelli'
+            Mhyd.pnt_model = 'Angelinelli'
 
         if pnt_model == 'Ettori':
             post_betant = np.array(trace.posterior['beta_nt']).flatten()
 
             post_p0nt = np.array(trace.posterior['p0_nt']).flatten()
 
             pnt_pars = np.empty((nsamp, 2))
             pnt_pars[:,0] = post_p0nt
             pnt_pars[:,1] = post_betant
 
             Mhyd.pnt_pars = pnt_pars
 
-            Mhyd.pntmodel = 'Ettori'
+            Mhyd.pnt_model = 'Ettori'
 
     alldens = np.sqrt(np.dot(Kdens, np.exp(samples.T)) * transf)
 
     if Mhyd.cf_prof is not None:
         pmc = np.median(alldens, axis=1) / np.sqrt(Mhyd.ccf[nmin:nmax])
         pmcl = np.percentile(alldens, 50. - 68.3 / 2., axis=1) / np.sqrt(Mhyd.ccf[nmin:nmax])
         pmch = np.percentile(alldens, 50. + 68.3 / 2., axis=1) / np.sqrt(Mhyd.ccf[nmin:nmax])
@@ -627,15 +680,14 @@
 
     Mhyd.samppar = samppar
     Mhyd.samplogp0 = samplogp0
     Mhyd.elong = elong
     Mhyd.K = K
     Mhyd.Kdens = Kdens
     Mhyd.Ksb = Ksb
-    Mhyd.transf = transf
     Mhyd.Kdens_m = Kdens_m
 
     if Mhyd.spec_data is not None:
         kt_mod = kt_from_samples(Mhyd, model, nmore=nmore)
         Mhyd.ktmod = kt_mod['TSPEC']
         Mhyd.ktmod_lo = kt_mod['TSPEC_LO']
         Mhyd.ktmod_hi = kt_mod['TSPEC_HI']
@@ -794,14 +846,16 @@
 
         self.mfact = 4. * np.pi * rho_cz * 1e-22
 
         self.mfact0 = kev2erg * cgskpc / (cgsG * cgsamu * self.mup) / Msun / 1e13
 
         self.mgas_fact = cgsamu * self.mu_e / Msun
 
+        self.transf = 4. * (1. + redshift) ** 2 * (180. * 60.) ** 2 / np.pi / 1e-14 * self.nhc / cgsMpc * 1e3
+
 
     def emissivity(self, nh, rmf, type='single', kt=None, abund='angr', Z=0.3, elow=0.5, ehigh=2.0, arf=None, outz=None, method='interp', outkt=None):
         '''
         Compute the conversion between count rate and emissivity using XSPEC by run the :func:`hydromass.emissivity.calc_emissivity` function. Requires XSPEC to be available in PATH.
 
         :param nh: Source NH in units of 1e22 cm**(-2)
         :type nh: float
@@ -872,15 +926,15 @@
                                     outkt=outkt)
 
 
     def run(self, model=None, bkglim=None, nmcmc=1000, fit_bkg=False, back=None,
             samplefile=None, nrc=None, nbetas=6, min_beta=0.6, nmore=5,
             p0_prior=None, tune=500, dmonly=False, mstar=None, find_map=True, pnt=False,
             rmin=None, rmax=None, p0_type='sb', init='ADVI', target_accept=0.9,
-            fit_elong=False):
+            pnt_model='Ettori', fit_elong=False):
         '''
         Optimize the mass model using the :func:`hydromass.mhyd.Run_Mhyd_PyMC3` function.
 
         :param model:  A :class:`hydromass.functions.Model` object including the chosen mass model and its input values (mandatory input)
         :type model: class:`hydromass.functions.Model`
         :param bkglim: Limit (in arcmin) out to which the SB data will be fitted; if None then the whole range is considered. Defaults to None.
         :type bkglim: float
@@ -939,14 +993,15 @@
                        nmore=nmore,
                        p0_prior=p0_prior,
                        tune=tune,
                        dmonly=dmonly,
                        mstar=mstar,
                        find_map=find_map,
                        pnt=pnt,
+                       pnt_model=pnt_model,
                        rmin=rmin,
                        rmax=rmax,
                        p0_type=p0_type,
                        init=init,
                        target_accept=target_accept,
                        fit_elong=fit_elong)
 
@@ -1057,15 +1112,15 @@
                           nmore=nmore,
                           tune=tune,
                           find_map=find_map)
 
 
     def run_GP(self, bkglim=None, nmcmc=1000, fit_bkg=False, back=None,
             samplefile=None, nrc=None, nbetas=6, min_beta=0.6, nmore=5, tune=500, find_map=True,
-            bin_fact=1.0, smin=None, smax=None, ngauss=100):
+            bin_fact=1.0, smin=None, smax=None, ngauss=100, extend=False):
 
         '''
         Run a non-parametric log-normal mixture reconstruction. See :func:`hydromass.nonparametric.Run_NonParametric_PyMC3`
 
         :param bkglim: Radius (in arcmin) beyond which it is assumed that the background fully dominates the profile. If None, the entire radial range is fitted as source + background. Defaults to None.
         :type bkglim: float
         :param nmcmc: Number of NUTS samples. Defaults to 1000
@@ -1109,15 +1164,16 @@
                                 min_beta=min_beta,
                                 nmore=nmore,
                                 tune=tune,
                                 find_map=find_map,
                                 bin_fact=bin_fact,
                                 smin=smin,
                                 smax=smax,
-                                ngauss=ngauss)
+                                ngauss=ngauss,
+                                extend=extend)
 
     def SaveModel(self, model, outfile=None):
         '''
         Save the output of a mass model fit into a FITS file through the :func:`hydromass.save.SaveModel` function
 
         :param model: :class:`hydromass.functions.Model` defining the chosen mass model
         :type model: :class:`hydromass.functions.Model`
```

### Comparing `hydromass-0.4/hydromass/nonparametric.py` & `hydromass-0.5/hydromass/nonparametric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from .deproject import *
 from .plots import rads_more, get_coolfunc, estimate_P0, plt
 from scipy.interpolate import interp1d
-import pymc3 as pm
+import pymc as pm
 
 # Function to compute linear operator transforming norms of GP model into radial profile
 
 def calc_gp_operator(npt, rads, rin, rout, bin_fact=1.0, smin=None, smax=None):
     '''
     Set up a linear operator transforming the model coefficients into the temperature profile as a sum of Gaussian functions,
 
@@ -306,17 +306,15 @@
 
         cf_prof = Mhyd.ccf
 
     dens_m = np.sqrt(np.dot(Mhyd.Kdens_m, np.exp(Mhyd.samples.T)) / cf_prof * Mhyd.transf)
 
     t3d = np.dot(Mhyd.GPop, Mhyd.samppar.T)
 
-    extend = False
-
-    if extend:
+    if Mhyd.extend:
 
         if np.max(rout_m) > rout_m[ntm - 1]:
             # Power law outside of the fitted range
             ne0 = dens_m[nvalm - 1, :]
 
             T0 = Mhyd.sampp0 / ne0
 
@@ -405,17 +403,15 @@
 
         cf_prof = Mhyd.ccf
 
     dens_m = np.sqrt(np.dot(Mhyd.Kdens_m, np.exp(Mhyd.samples.T)) / cf_prof * Mhyd.transf)
 
     t3d = np.dot(Mhyd.GPop, Mhyd.samppar.T)
 
-    extend = False
-
-    if extend:
+    if Mhyd.extend:
 
         if np.max(rout_m) > rout_m[ntm - 1]:
             # Power law outside of the fitted range
             ne0 = dens_m[nvalm - 1, :]
 
             T0 = Mhyd.sampp0 / ne0
 
@@ -549,17 +545,15 @@
 
     rout_mul = np.repeat(rout_m, nsamp).reshape(nvalm, nsamp) * cgskpc
 
     grad_t3d = rout_mul / cgskpc / t3d * np.dot(GPgrad, Mhyd.samppar.T)
 
     rspo = np.max(rout_joint)
 
-    extend = False
-
-    if extend:
+    if Mhyd.extend:
 
         if rout > rspo:
             # Power law outside of the fitted range
             ne0 = dens_m[nvalm - 1, :]
 
             T0 = Mhyd.sampp0 / ne0
 
@@ -750,17 +744,15 @@
 
     GPop, rgauss, sig = calc_gp_operator_lognormal(Mhyd.ngauss, rout_m, rin_joint, rout_joint, bin_fact=Mhyd.bin_fact, smin=Mhyd.smin, smax=Mhyd.smax)
 
     t3d = np.dot(GPop, Mhyd.samppar.T)
 
     rspo = np.max(rout_joint)
 
-    extend = False
-
-    if extend:
+    if Mhyd.extend:
 
         if rout > rspo:
             # Power law outside of the fitted range
             ne0 = dens_m[nvalm - 1, :]
 
             T0 = Mhyd.sampp0 / ne0
 
@@ -845,15 +837,16 @@
 
     return dict
 
 
 
 def Run_NonParametric_PyMC3(Mhyd, bkglim=None, nmcmc=1000, fit_bkg=False, back=None,
                    samplefile=None, nrc=None, nbetas=6, min_beta=0.6, nmore=5,
-                   tune=500, bin_fact=1.0, smin=None, smax=None, ngauss=100, find_map=True):
+                   tune=500, bin_fact=1.0, smin=None, smax=None, ngauss=100, find_map=True,
+                   extend=False):
     """
     Run non-parametric log-normal mixture reconstruction. Following Eckert et al. (2022), the temperature profile is described as a linear combination of a large number of log-normal functions, whereas the gas density profile is decomposed on a basis of King functions. The number of log-normal functions as well as the smoothing scales can be adjusted by the user.
 
     :param Mhyd: An input :class:`hydromass.mhyd.Mhyd` object including the data and the source definition
     :type Mhyd: :class:`hydromass.mhyd.Mhyd`
     :param bkglim: Radius (in arcmin) beyond which it is assumed that the background fully dominates the profile. If None, the entire radial range is fitted as source + background. Defaults to None.
     :type bkglim: float
@@ -934,22 +927,22 @@
         K = np.dot(psfmat, Ksb)
 
     # Set up initial values
     if np.isnan(sb[0]) or sb[0] <= 0:
         testval = -10.
     else:
         testval = np.log(sb[0] / npt)
-    if np.isnan(back) or back == 0:
+    if np.isnan(back) or back <= 0 or back is None:
         testbkg = -10.
     else:
         testbkg = np.log(back)
 
     z = Mhyd.redshift
 
-    transf = 4. * (1. + z) ** 2 * (180. * 60.) ** 2 / np.pi / 1e-14 * Mhyd.nhc / cgsMpc * 1e3
+    transf = Mhyd.transf
 
     pardens = list_params_density(rad, sourcereg, Mhyd.amin2kpc, nrc, nbetas, min_beta)
 
     if fit_bkg:
 
         Kdens = calc_density_operator(rad, pardens, Mhyd.amin2kpc)
 
@@ -1035,19 +1028,28 @@
 
     rin_joint[0] = 0.
 
     GPop, rgauss, sig = calc_gp_operator_lognormal(ngauss, rout_m, rin_joint, rout_joint, bin_fact=bin_fact, smin=smin, smax=smax)
 
     GPgrad = calc_gp_grad_operator_lognormal(ngauss, rout_m, rin_joint, rout_joint, bin_fact=bin_fact, smin=smin, smax=smax)
 
-    P0_est = estimate_P0(Mhyd)
+    hydro_model = pm.Model()
+
+    P0_est, err_P0_est = None, None
 
-    err_P0_est = P0_est  # 1-dex
+    if extend:
 
-    hydro_model = pm.Model()
+        P0_est = estimate_P0(Mhyd)
+
+        err_P0_est = P0_est  # 1-dex
+
+        Mhyd.extend = True
+
+    else:
+        Mhyd.extend = False
 
     with hydro_model:
         # Priors for unknown model parameters
         coefs = pm.Normal('coefs', mu=testval, sigma=20, shape=npt)
 
         if fit_bkg:
 
@@ -1068,23 +1070,18 @@
         # GP parameters
         #coefs_GP = pm.Normal('GP', mu=np.log(30./ngauss), sigma=20, shape=ngauss)
         coefs_GP = pm.Normal('GP', mu=1./np.sqrt(np.arange(1,ngauss+1)), sigma=20, shape=ngauss)
 
         # Expected value of outcome
         gpp = pm.math.exp(coefs_GP)
 
-        for RV in hydro_model.basic_RVs:
-            print(RV.name, RV.logp(hydro_model.test_point))
-
         t3d = pm.math.dot(GPop, gpp)
 
         dens_m = pm.math.sqrt(pm.math.dot(Kdens_m, al) / cf * transf)  # electron density in cm-3
 
-        extend = False
-
         if extend:
             logp0 = pm.TruncatedNormal('logp0', mu=np.log(P0_est), sigma=err_P0_est / P0_est,
                                        lower=np.log(P0_est) - err_P0_est / P0_est,
                                        upper=np.log(P0_est) + err_P0_est / P0_est)
 
             if np.max(rout_m) > rout_m[ntm - 1]:
                 # Power law outside of the fitted range
@@ -1106,14 +1103,15 @@
 
                 t3d_in = t3d[inspec]
 
                 t3d_out = Tspo * (rout_m[outspec] / rspo) ** (-alpha)
 
                 t3d = pm.math.concatenate([t3d_in, t3d_out])
 
+
         # Density Likelihood
         if fit_bkg:
 
             count_obs = pm.Poisson('counts', mu=pred, observed=counts)  # counts likelihood
 
         else:
 
@@ -1141,40 +1139,68 @@
 
             P_obs = pm.MvNormal('P', mu=pfit, observed=Mhyd.sz_data.pres_sz, cov=Mhyd.sz_data.covmat_sz)  # SZ pressure likelihood
 
     tinit = time.time()
 
     print('Running MCMC...')
 
+    isjax = False
+
+    try:
+        import pymc.sampling.jax as pmjax
+
+    except ImportError:
+        print('JAX not found, using default sampler')
+
+    else:
+        isjax = True
+        import pymc.sampling.jax as pmjax
+
     with hydro_model:
 
         if find_map:
 
             start = pm.find_MAP()
 
-            trace = pm.sample(nmcmc, start=start, tune=tune)
+            if not isjax:
+
+                trace = pm.sample(nmcmc, initvals=start, tune=tune, return_inferencedata=True)
+
+            else:
+
+                trace = pmjax.sample_numpyro_nuts(nmcmc, initvals=start, tune=tune, return_inferencedata=True)
 
         else:
 
-            trace = pm.sample(nmcmc, tune=tune)
+            if not isjax:
+
+                trace = pm.sample(nmcmc, tune=tune)
+
+            else:
+
+                trace = pmjax.sample_numpyro_nuts(nmcmc, tune=tune)
 
     print('Done.')
 
     tend = time.time()
 
     print(' Total computing time is: ', (tend - tinit) / 60., ' minutes')
 
     Mhyd.trace = trace
 
     # Get chains and save them to file
-    sampc = trace.get_values('coefs')
+    chain_coefs = np.array(trace.posterior['coefs'])
+
+    sc_coefs = chain_coefs.shape
+
+    sampc = chain_coefs.reshape(sc_coefs[0]*sc_coefs[1], sc_coefs[2])
 
     if fit_bkg:
 
-        sampb = trace.get_values('bkg')
+        sampb = np.array(trace.posterior['bkg']).flatten()
 
         samples = np.append(sampc, sampb, axis=1)
 
     else:
         samples = sampc
 
     Mhyd.samples = samples
@@ -1228,15 +1254,20 @@
     pmc = np.median(alldens, axis=1) / np.sqrt(Mhyd.ccf)
     pmcl = np.percentile(alldens, 50. - 68.3 / 2., axis=1) / np.sqrt(Mhyd.ccf)
     pmch = np.percentile(alldens, 50. + 68.3 / 2., axis=1) / np.sqrt(Mhyd.ccf)
     Mhyd.dens = pmc
     Mhyd.dens_lo = pmcl
     Mhyd.dens_hi = pmch
 
-    samppar = np.exp(trace.get_values('GP'))
+    # Get chains and save them to file
+    chain_gp = np.exp(np.array(trace.posterior['GP']))
+
+    sc_gp = chain_gp.shape
+
+    samppar = chain_gp.reshape(sc_gp[0]*sc_gp[1], sc_gp[2])
 
     Mhyd.samppar = samppar
 
     Mhyd.GPop = GPop
     Mhyd.GPgrad = GPgrad
     Mhyd.smin = smin
     Mhyd.smax = smax
@@ -1247,15 +1278,15 @@
     Mhyd.Kdens = Kdens
     Mhyd.Ksb = Ksb
     Mhyd.transf = transf
     Mhyd.Kdens_m = Kdens_m
     Mhyd.Kdens_grad = Kdens_grad
 
     if extend:
-        sampp0 = np.exp(trace.get_values('logp0'))
+        sampp0 = np.exp(trace.posterior['logp0'].to_numpy().flatten())
         Mhyd.sampp0 = sampp0
 
     if Mhyd.spec_data is not None:
         kt_mod = kt_GP_from_samples(Mhyd, nmore=nmore)
         Mhyd.ktmod = kt_mod['TSPEC']
         Mhyd.ktmod_lo = kt_mod['TSPEC_LO']
         Mhyd.ktmod_hi = kt_mod['TSPEC_HI']
```

### Comparing `hydromass-0.4/hydromass/plots.py` & `hydromass-0.5/hydromass/plots.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,14 +223,15 @@
     alpha=pars[2]
     beta=pars[3]
     gamma=pars[4]
     t1=np.power(x/rs,gamma)
     t2=np.power(1.+np.power(x/rs,alpha),(beta-gamma)/alpha)
     return P0/t1/t2
 
+
 def estimate_P0(Mhyd, dens='sb'):
     '''
     Provide an estimate of the pressure at the outer boundary by fitting a rough gNFW profile to the data. A rough electron density profile is estimated by deprojecting the surface brightness profile using the onion peeling techique, and temperature deprojection is neglected. The resulting pressure profile is fitted with a gNFW profile using the scipy.minimize function and the best-fit function is used to extrapolate the pressure to the outer boundary to provide a rough estimate of :math:`P_0`.
 
     :param Mhyd: A :class:`hydromass.mhyd.Mhyd` object containing the loaded data
     :type Mhyd: class:`hydromass.mhyd.Mhyd`
     :param dens: Set whether we will deproject the surface brightness profile (dens='sb') or the normalization of the spectrum (dens='norm'). Defaults to 'sb'
@@ -239,21 +240,40 @@
     :rtype: float
     '''
     spec_data = Mhyd.spec_data
 
     if dens == 'sb' or spec_data.norm is None:
         sbprof = copy.copy(Mhyd.sbprof)
 
-        sbprof.profile = np.abs(sbprof.profile)
+        modbeta = pyproffit.Model(pyproffit.DoubleBeta)
+
+        fitbeta = pyproffit.Fitter(model=modbeta, profile=sbprof, bkg=-12., beta=0.7, rc1=0.5, rc2=2., norm=-2, ratio=2)
+
+        fitbeta.minuit.fixed['bkg'] = True
+
+        fitbeta.Migrad()
+
+        rc1 = fitbeta.params['rc1'] * Mhyd.amin2kpc  # kpc
+        rc2 = fitbeta.params['rc2'] * Mhyd.amin2kpc
+
+        beta = fitbeta.params['beta']
+        norm = fitbeta.params['norm']
+        ratio = fitbeta.params['ratio']
+
+        cfact1 = gamma(3 * beta) / gamma(3 * beta - 0.5) / np.sqrt(np.pi) / rc1
+        cfact2 = gamma(3 * beta) / gamma(3 * beta - 0.5) / np.sqrt(np.pi) / rc2
 
-        deprop = pyproffit.Deproject(z=Mhyd.redshift, cf=Mhyd.ccf, profile=sbprof)
+        rfit = sbprof.bins * Mhyd.amin2kpc
 
-        deprop.OnionPeeling()
+        t1 = (1. + np.power(rfit / rc1, 2)) ** (-3. * beta) * cfact1
+        t2 = (1. + np.power(rfit / rc2, 2)) ** (-3. * beta) * cfact2
 
-        ne_interp = np.interp(spec_data.rref_x_am, sbprof.bins, deprop.dens) * Mhyd.nhc
+        dens_prof = np.sqrt(10 ** norm * (t1 + ratio * t2) / Mhyd.ccf * Mhyd.transf)
+
+        ne_interp = np.interp(spec_data.rref_x_am, sbprof.bins, dens_prof)
 
         p_interp = ne_interp * spec_data.temp_x
         ep_interp = ne_interp * spec_data.errt_x
 
     else:
         sbprof = copy.copy(Mhyd.sbprof)
 
@@ -276,30 +296,42 @@
 
         p_interp = depr.dens * spec_data.temp_x
         ep_interp = depr.dens * spec_data.errt_x
 
     pars_press = np.array([3.28, 1200., 1.33, 4.72, 0.59])
 
     def chi2_gnfw(pars):
-        pars_press[0] = pars[0]
+        pars_press[0] = 10 ** pars[0]
         pars_press[1] = pars[1]
         mm = gnfw_p0(spec_data.rref_x, pars_press)
         chi2 = np.sum((p_interp - mm) ** 2 / ep_interp ** 2)
         return chi2
 
-    res = minimize(chi2_gnfw, np.array([1e-4, 1200.]), method='Nelder-Mead')
+    bnds = ((None, None), (0, None))
+
+    res = minimize(chi2_gnfw, np.array([-4, 1200.]), method='Nelder-Mead', bounds=bnds)
 
     maxrad = np.max(sbprof.bins * Mhyd.amin2kpc)
 
-    pars_press[:2] = res['x']
+    if Mhyd.sz_data is not None:
+
+        rmaxsz = np.max(Mhyd.rout_sz)
+
+        if rmaxsz > maxrad:
+
+            maxrad = rmaxsz
+
+    pars_press[0] = 10 ** res['x'][0]
+    pars_press[1] = res['x'][1]
 
     p0 = gnfw_p0(maxrad, pars_press)
 
     return p0
 
+
 def densout_pout_from_samples(Mhyd, model, rin_m, rout_m):
     '''
     Compute the model 3D density and pressure profiles from the output NUTS sample on an arbitrary output grid
 
     :param Mhyd: A :class:`hydromass.mhyd.Mhyd` object containing the result of a mass model fit
     :type Mhyd: class:`hydromass.mhyd.Mhyd`
     :param model: A :class:`hydromass.functions.Model` object containing the definition of the mass model
@@ -393,21 +425,21 @@
 
     int_mat = cumsum_mat(nvalm)
 
     press_out = press00 - np.dot(int_mat, dpres.T)
 
     if Mhyd.pnt:
 
-        if Mhyd.pntmodel == 'Angelinelli':
+        if Mhyd.pnt_model == 'Angelinelli':
 
             alpha_turb = alpha_turb_np(rref_m, Mhyd.samppar, Mhyd.redshift, Mhyd.pnt_pars)
 
             pth = press_out * (1. - alpha_turb)
 
-        if Mhyd.pntmodel == 'Ettori':
+        if Mhyd.pnt_model == 'Ettori':
 
             log_pnt = Mhyd.pnt_pars[:,1] * np.log(dens_m * 1e3) + Mhyd.pnt_pars[:,0] * np.log(10)
 
             pth = press_out - np.exp(log_pnt)
 
     else:
```

### Comparing `hydromass-0.4/hydromass/pnt.py` & `hydromass-0.5/hydromass/pnt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pkg_resources
 import os
 import numpy as np
-import pymc3 as pm
+import pymc as pm
 
 def r200m_from_params(c, z):
     '''
     Approximate the ratio of :math:`R_{200m}` to :math:`R_{200c}` as a function of NFW concentration and redshift
 
     :param c: NFW concentration
     :type c: float
```

### Comparing `hydromass-0.4/hydromass/polytropic.py` & `hydromass-0.5/hydromass/polytropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from .deproject import *
 from .plots import rads_more, get_coolfunc, plt
 from .functions import ArcTan
-import pymc3 as pm
+import pymc as pm
 
 tt_arctan = ArcTan()
 
 # Gamma(R) function
 def func_poly_rad_pm(x, pars, dens, grad_dens):
     '''
     Theano model of the effective polytropic index as a function of radius following Ghirardini et al. (2019), modified to avoid the divergence in the core.
@@ -950,17 +950,14 @@
 
                 dummy_param = 0 * dummy + Polytropic.start[i]
 
                 modpar = pm.Deterministic(name, dummy_param)
 
             allpmod.append(modpar)
 
-        for RV in hydro_model.basic_RVs:
-            print(RV.name, RV.logp(hydro_model.test_point))
-
         pmod = pm.math.stack(allpmod, axis=0)
 
         dens_m = pm.math.sqrt(pm.math.dot(Kdens_m, al) / cf * transf)  # electron density in cm-3
 
         dens_grad = pm.math.dot(Kdens_grad, al) / 2. / dens_m ** 2 / cf * transf # d(logn)/d(log r)
 
         p3d = Polytropic.func_pm(rout_m, pmod, dens_m, dens_grad)
@@ -996,25 +993,50 @@
 
             P_obs = pm.MvNormal('P', mu=pfit, observed=Mhyd.sz_data.pres_sz, cov=Mhyd.sz_data.covmat_sz)  # SZ pressure likelihood
 
         tinit = time.time()
 
         print('Running MCMC...')
 
+        isjax = False
+
+        try:
+            import pymc.sampling.jax as pmjax
+
+        except ImportError:
+            print('JAX not found, using default sampler')
+
+        else:
+            isjax = True
+            import pymc.sampling.jax as pmjax
+
         with hydro_model:
 
             if find_map:
 
                 start = pm.find_MAP()
 
-                trace = pm.sample(nmcmc, start=start, tune=tune, init='ADVI',  return_inferencedata=True, target_accept=0.9)
+                if not isjax:
+
+                    trace = pm.sample(nmcmc, initvals=start, init='ADVI',  tune=tune, return_inferencedata=True, target_accept=0.9)
+
+                else:
+
+                    trace = pmjax.sample_numpyro_nuts(nmcmc, initvals=start, init='ADVI',  tune=tune,
+                                                      return_inferencedata=True, target_accept=0.9)
 
             else:
 
-                trace = pm.sample(nmcmc, tune=tune, init='ADVI',  return_inferencedata=True, target_accept=0.9)
+                if not isjax:
+
+                    trace = pm.sample(nmcmc, tune=tune, init='ADVI', target_accept=0.9)
+
+                else:
+
+                    trace = pmjax.sample_numpyro_nuts(nmcmc, tune=tune, init='ADVI', target_accept=0.9)
 
         print('Done.')
 
         tend = time.time()
 
         print(' Total computing time is: ', (tend - tinit) / 60., ' minutes')
```

### Comparing `hydromass-0.4/hydromass/save.py` & `hydromass-0.5/hydromass/save.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     headsamp['MINBETA'] = Mhyd.min_beta
     headsamp['TRANSF'] = Mhyd.transf
     headsamp['FITBKG'] = Mhyd.fit_bkg
     headsamp['NMORE'] = Mhyd.nmore
     headsamp['DMONLY'] = Mhyd.dmonly
     headsamp['PNT'] = Mhyd.pnt
     if Mhyd.pnt:
-        headsamp['PNTMODEL'] = Mhyd.pntmodel
+        headsamp['PNTMODEL'] = Mhyd.pnt_model
 
     is_elong = False
 
     try:
         nn = len(Mhyd.elong)
 
     except TypeError:
@@ -89,17 +89,17 @@
     modhdu.name = 'MASS MODEL'
 
     modhead = modhdu.header
     modhead['MASSMOD'] = model.massmod
 
     modhead['DELTA'] = model.delta
 
-    modhead['WAIC'] = Mhyd.waic['waic']
-
-    modhead['LOO'] = Mhyd.loo['loo']
+    # modhead['WAIC'] = Mhyd.waic['waic']
+    #
+    # modhead['LOO'] = Mhyd.loo['loo']
 
     for i in range(model.npar):
         parname = model.parnames[i]
 
         modhead['ST' + parname] = model.start[i]
 
         modhead['SD' + parname] = model.sd[i]
@@ -209,14 +209,18 @@
 
         Mhyd.elong = tabelong.data
 
     else:
 
         Mhyd.elong = 1
 
+    if 'PNTMODEL' in headden:
+
+        Mhyd.pnt_model = headden['PNTMODEL']
+
     #Mhyd.waic = headden['WAIC']
 
     #Mhyd.loo = headden['LOO']
 
     modhead = fin[2].header
 
     massmod = modhead['MASSMOD']
@@ -322,15 +326,15 @@
         allsb_conv = np.dot(prof.psfmat, allsb[:, :npt])
 
     else:
 
         Ksb = calc_sb_operator(rad, sourcereg, pars, withbkg=False)
 
         if is_elong:
-            print('hello world')
+
             elong_mat = np.tile(Mhyd.elong, Mhyd.sbprof.nbin).reshape(Mhyd.sbprof.nbin,nsamp)
 
             allsb = np.dot(Ksb, np.exp(Mhyd.samples.T)) * elong_mat ** 0.5
 
             allsb_conv = np.dot(Mhyd.K, np.exp(Mhyd.samples.T)) * elong_mat ** 0.5
 
         else:
```

### Comparing `hydromass-0.4/hydromass/tpdata.py` & `hydromass-0.5/hydromass/tpdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -376,27 +376,31 @@
     :param psz: 1-D array containing the SZ pressure profile (in keV cm^-3). If None, the data should be passed as a FITS file using the sz_data argument. Defaults to None
     :type psz: numpy.ndarray
     :param covmat_sz: 2-D array containing the covariance matrix on the SZ pressure profile. If None, the data should be passed as a FITS file using the sz_data argument. Defaults to None
     :type covmat_sz: numpy.ndarray
     :param cosmo: Astropy cosmology object including the cosmology definition
     :type cosmo: astropy.cosmology
     '''
-    def __init__(self, redshift, sz_data=None, rin=None, rout=None, psz=None, covmat_sz=None, cosmo=None):
+    def __init__(self, redshift, sz_data=None, rin=None, rout=None, psz=None, y_sz=None, covmat_sz=None, cosmo=None):
 
-        if sz_data is None and psz is None:
+        if sz_data is None:
 
-            print('No data provided. Please provide either an input FITS data file or a set of numpy arrays.')
+            if y_sz is None and psz is None:
 
-            return
+                print('No data provided. Please provide either an input FITS data file or a set of numpy arrays.')
 
-        if sz_data is not None and psz is not None:
+                return
+
+        if sz_data is not None:
 
-            print('Ambiguous input. Please provide either an input FITS data file or a set of numpy arrays.')
+            if y_sz is not None and psz is not None:
 
-            return
+                print('Ambiguous input. Please provide either an input FITS data file or a set of numpy arrays.')
+
+                return
 
         if sz_data is not None:
 
             if not os.path.exists(sz_data):
 
                 print('SZ data file not found in path, skipping')
 
@@ -429,14 +433,32 @@
 
             self.pres_sz = psz
 
             self.covmat_sz = covmat_sz.astype(np.float32)
 
             self.errp_sz = np.sqrt(np.diag(covmat_sz))
 
+            self.y_sz = None
+
+        if y_sz is not None:
+
+            if rin is None or rout is None or covmat_sz is None:
+
+                print('Missing input, please provide rin, rout, y_sz, and covmat_sz')
+
+                return
+
+            self.y_sz = y_sz
+
+            self.covmat_sz = covmat_sz.astype(np.float32)
+
+            self.errp_sz = np.sqrt(np.diag(covmat_sz))
+
+            self.pres_sz = None
+
         if cosmo is None:
 
             from astropy.cosmology import Planck15 as cosmo
 
         amin2kpc = cosmo.kpc_proper_per_arcmin(redshift).value
 
         self.rin_sz = rin
```

### Comparing `hydromass-0.4/hydromass/wl.py` & `hydromass-0.5/hydromass/wl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pymc3 as pm
+import pymc as pm
 import numpy as np
 
 from .deproject import MyDeprojVol
 from .functions import rho_nfw_cr
 
 
 def rho_to_sigma(radii_bins, rho):
```

### Comparing `hydromass-0.4/hydromass.egg-info/SOURCES.txt` & `hydromass-0.5/hydromass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydromass-0.4/setup.py` & `hydromass-0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 
 setup(
       name='hydromass',    # This is the name of your PyPI-package.
-      version='0.4',
+      version='0.5',
       description='Hydrostatic mass calculator',
       author='Dominique Eckert, Vittorio Ghirardini, Stefano Ettori',
       author_email='Dominique.Eckert@unige.ch',
       url="https://github.com/domeckert/hydromass",
       packages=['hydromass'],
       install_requires=[
-            'numpy','scipy','astropy','matplotlib','pymc3','pyproffit'
+            'numpy','scipy','astropy','matplotlib','pymc','aesara','pyproffit','numpyro','corner'
       ],
       include_package_data=True,
 )
```

