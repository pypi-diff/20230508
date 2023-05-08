# Comparing `tmp/peleffy-1.4.3.tar.gz` & `tmp/peleffy-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peleffy-1.4.3.tar", last modified: Tue Jun 21 14:01:40 2022, max compression
+gzip compressed data, was "peleffy-1.4.4.tar", last modified: Mon May  8 15:59:08 2023, max compression
```

## Comparing `peleffy-1.4.3.tar` & `peleffy-1.4.4.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.112548 peleffy-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-06-21 14:01:25.000000 peleffy-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-21 14:01:25.000000 peleffy-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-06-21 14:01:40.112548 peleffy-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3456 2022-06-21 14:01:25.000000 peleffy-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.112548 peleffy-1.4.3/peleffy/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-06-21 14:01:40.112548 peleffy-1.4.3/peleffy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.092547 peleffy-1.4.3/peleffy/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.096547 peleffy-1.4.3/peleffy/data/complexes/
--rw-r--r--   0 runner    (1001) docker     (121)   556158 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/complexes/5XXD_SAM.pdb
--rw-r--r--   0 runner    (1001) docker     (121)   227599 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/complexes/LIG1_LIG2.pdb
--rw-r--r--   0 runner    (1001) docker     (121)   214091 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/complexes/LYS_BNZ.pdb
--rw-r--r--   0 runner    (1001) docker     (121)   572055 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/complexes/complex_test.pdb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.096547 peleffy-1.4.3/peleffy/data/forcefields/
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/forcefields/GBSA_OBC1-1.0.offxml
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/forcefields/GBSA_OBC2-1.0.offxml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.100547 peleffy-1.4.3/peleffy/data/ligands/
--rw-r--r--   0 runner    (1001) docker     (121)    12432 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/BHP.mae
--rw-r--r--   0 runner    (1001) docker     (121)     4003 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/BHP.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/BNZ.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     6203 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/LIG1.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     4418 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/LIG2.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     4454 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/SAM.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/acetylene.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/ammonium.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     2862 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/benzamidine.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     5221 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/benzene.mae
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/benzene.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     1848 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/benzene_without_connectivity.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      946 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/ethylene.mae
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/ethylene.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/ligand.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     1394 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/malonate.mae
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/malonate.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/methane.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     3832 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/modified_sidechain.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/octafluorocyclobutane.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     5710 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/oleic_acid.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/propionic_acid.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     5687 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/toluene.mae
--rw-r--r--   0 runner    (1001) docker     (121)     2550 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/toluene.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/trimethylglycine.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/ligands/trimethylglycine_moved.pdb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.100547 peleffy-1.4.3/peleffy/data/parameters/
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/parameters/ETH.conformation
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/parameters/ETH.dihedral
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/parameters/OBCparam.json
--rw-r--r--   0 runner    (1001) docker     (121)     5548 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/parameters/f14_sgbnp.param
--rw-r--r--   0 runner    (1001) docker     (121)    17597 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/parameters/similarity.param
--rw-r--r--   0 runner    (1001) docker     (121)    64313 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/parameters/solventParamsHCTOBC.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.108548 peleffy-1.4.3/peleffy/data/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    11191 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/CO1_ffld_output.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ETL_ffld_output.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5819 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ETL_openff-1.2.1_opls2005_parameters1.json
--rw-r--r--   0 runner    (1001) docker     (121)     5781 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ETL_openff-1.2.1_opls2005_parameters2.json
--rw-r--r--   0 runner    (1001) docker     (121)     5819 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ETL_openff-1.2.1_parameters.json
--rw-r--r--   0 runner    (1001) docker     (121)     5826 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ETL_opls2005_parameters.json
--rw-r--r--   0 runner    (1001) docker     (121)    64495 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ETL_solventParamsHCTOBC.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6823 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MAL_ffld_output.txt
--rw-r--r--   0 runner    (1001) docker     (121)    64616 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MAL_solventParamsHCTOBC.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8857 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MAT.mae
--rw-r--r--   0 runner    (1001) docker     (121)     3273 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MAT.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     2730 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_ffld_output.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters1.json
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters2.json
--rw-r--r--   0 runner    (1001) docker     (121)     3637 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters3.json
--rw-r--r--   0 runner    (1001) docker     (121)     3599 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters4.json
--rw-r--r--   0 runner    (1001) docker     (121)     3705 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters5.json
--rw-r--r--   0 runner    (1001) docker     (121)     3713 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_parameters.json
--rw-r--r--   0 runner    (1001) docker     (121)     3696 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_opls2005_parameters.json
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_parameters_to_json.json
--rw-r--r--   0 runner    (1001) docker     (121)     3638 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_parameters_to_string.txt
--rw-r--r--   0 runner    (1001) docker     (121)    64462 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MET_solventParamsHCTOBC.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.108548 peleffy-1.4.3/peleffy/data/tests/MRO_oleic/
--rw-r--r--   0 runner    (1001) docker     (121)     8122 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MRO_oleic/HEM.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MRO_oleic/MG.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     5490 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MRO_oleic/OLC.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/MRO_oleic/OXO.pdb
--rw-r--r--   0 runner    (1001) docker     (121)    42254 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/OLC_ffld_output.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/OPLS_etlz
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/OPLS_etlz_amber
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/OPLS_malz
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/OPLS_malz_amber
--rw-r--r--   0 runner    (1001) docker     (121)     1280 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/OPLS_metz
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/OPLS_metz_amber
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/OXO_ffld_output.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_0.rot.assign
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_1.rot.assign
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_2.rot.assign
--rw-r--r--   0 runner    (1001) docker     (121)     3202 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_ligandParams_0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3250 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_ligandParams_1.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_ligandParams_2.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1710 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_mol1.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_mol2.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     2748 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/alchemical_structure.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ethane_noH.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ethylene_error1.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ethylene_error2.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      545 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ethylene_error3.pdb
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ethylene_error4.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/etlz
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/etlz_OBCParams.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1790 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/etlz_amber
--rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ligSUV_fixed.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ligSUV_no_elements1.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     4715 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ligSUV_no_elements2.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     3890 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ligSUV_no_elements3.pdb
--rw-r--r--   0 runner    (1001) docker     (121)     5592 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ligandParams.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/ligandParams_MAL.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/malz
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/malz_OBCParams.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/malz_amber
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/metz
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/metz_OBCParams.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/metz_amber
--rw-r--r--   0 runner    (1001) docker     (121)     5885 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/data/tests/unlz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.108548 peleffy-1.4.3/peleffy/forcefield/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/forcefield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5578 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/forcefield/calculators.py
--rw-r--r--   0 runner    (1001) docker     (121)    15686 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/forcefield/forcefield.py
--rw-r--r--   0 runner    (1001) docker     (121)    58508 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/forcefield/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4563 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/forcefield/selectors.py
--rw-r--r--   0 runner    (1001) docker     (121)    13483 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.108548 peleffy-1.4.3/peleffy/solvent/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/solvent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13216 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/solvent/solvent.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.108548 peleffy-1.4.3/peleffy/template/
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    49942 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/template/impact.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.112548 peleffy-1.4.3/peleffy/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   173141 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_alchemistry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2716 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_conformers.py
--rw-r--r--   0 runner    (1001) docker     (121)    15923 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_forcefields.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_integrity.py
--rw-r--r--   0 runner    (1001) docker     (121)    20785 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    20376 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_molecule.py
--rw-r--r--   0 runner    (1001) docker     (121)    61884 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)    14823 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_rotamers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8361 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_solvent.py
--rw-r--r--   0 runner    (1001) docker     (121)    15132 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (121)    14086 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_toolkits.py
--rw-r--r--   0 runner    (1001) docker     (121)    20177 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_topology.py
--rw-r--r--   0 runner    (1001) docker     (121)    41604 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16579 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.112548 peleffy-1.4.3/peleffy/topology/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    54277 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/alchemistry.py
--rw-r--r--   0 runner    (1001) docker     (121)     8880 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/conformer.py
--rw-r--r--   0 runner    (1001) docker     (121)    35118 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     4228 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/mapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    31511 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/molecule.py
--rw-r--r--   0 runner    (1001) docker     (121)    29641 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/rotamer.py
--rw-r--r--   0 runner    (1001) docker     (121)    14332 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/topology.py
--rw-r--r--   0 runner    (1001) docker     (121)     9450 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/topology/zmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.112548 peleffy-1.4.3/peleffy/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11326 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/utils/input.py
--rw-r--r--   0 runner    (1001) docker     (121)     8045 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (121)    44010 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/utils/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (121)    17081 2022-06-21 14:01:25.000000 peleffy-1.4.3/peleffy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-21 14:01:40.092547 peleffy-1.4.3/peleffy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-06-21 14:01:40.000000 peleffy-1.4.3/peleffy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5421 2022-06-21 14:01:40.000000 peleffy-1.4.3/peleffy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-21 14:01:40.000000 peleffy-1.4.3/peleffy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-06-21 14:01:40.000000 peleffy-1.4.3/peleffy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-06-21 14:01:40.112548 peleffy-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-06-21 14:01:25.000000 peleffy-1.4.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-06-21 14:01:25.000000 peleffy-1.4.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.694531 peleffy-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 15:58:55.000000 peleffy-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 15:58:55.000000 peleffy-1.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-08 15:59:08.694531 peleffy-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-08 15:58:55.000000 peleffy-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.694531 peleffy-1.4.4/peleffy/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-08 15:59:08.694531 peleffy-1.4.4/peleffy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.666531 peleffy-1.4.4/peleffy/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.670531 peleffy-1.4.4/peleffy/data/complexes/
+-rw-r--r--   0 runner    (1001) docker     (123)   556158 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/complexes/5XXD_SAM.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   227599 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/complexes/LIG1_LIG2.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   214091 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/complexes/LYS_BNZ.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   572055 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/complexes/complex_test.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.670531 peleffy-1.4.4/peleffy/data/forcefields/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/forcefields/GBSA_OBC1-1.0.offxml
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/forcefields/GBSA_OBC2-1.0.offxml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.674531 peleffy-1.4.4/peleffy/data/ligands/
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/BHP.mae
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/BHP.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/BNZ.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/LIG1.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/LIG2.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/SAM.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/acetylene.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/ammonium.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/benzamidine.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/benzene.mae
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/benzene.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/benzene_without_connectivity.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/ethylene.mae
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/ethylene.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/ligand.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/malonate.mae
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/malonate.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/methane.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/modified_sidechain.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/octafluorocyclobutane.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/oleic_acid.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/propionic_acid.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/toluene.mae
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/toluene.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/trimethylglycine.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/ligands/trimethylglycine_moved.pdb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.678531 peleffy-1.4.4/peleffy/data/parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/parameters/ETH.conformation
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/parameters/ETH.dihedral
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/parameters/OBCparam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/parameters/f14_sgbnp.param
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/parameters/similarity.param
+-rw-r--r--   0 runner    (1001) docker     (123)    64313 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/parameters/solventParamsHCTOBC.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.686531 peleffy-1.4.4/peleffy/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/CO1_ffld_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ETL_ffld_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ETL_openff-1.2.1_opls2005_parameters1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ETL_openff-1.2.1_opls2005_parameters2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ETL_openff-1.2.1_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ETL_opls2005_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    64495 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ETL_solventParamsHCTOBC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MAL_ffld_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    64616 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MAL_solventParamsHCTOBC.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MAT.mae
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MAT.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_ffld_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters4.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters5.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_opls2005_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_parameters_to_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_parameters_to_string.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    64462 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MET_solventParamsHCTOBC.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.686531 peleffy-1.4.4/peleffy/data/tests/MRO_oleic/
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MRO_oleic/HEM.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MRO_oleic/MG.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MRO_oleic/OLC.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/MRO_oleic/OXO.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)    42254 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/OLC_ffld_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/OPLS_etlz
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/OPLS_etlz_amber
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/OPLS_malz
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/OPLS_malz_amber
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/OPLS_metz
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/OPLS_metz_amber
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/OXO_ffld_output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_0.rot.assign
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_1.rot.assign
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_2.rot.assign
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_ligandParams_0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_ligandParams_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_ligandParams_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_mol1.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_mol2.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/alchemical_structure.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ethane_noH.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ethylene_error1.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ethylene_error2.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ethylene_error3.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ethylene_error4.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/etlz
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/etlz_OBCParams.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/etlz_amber
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ligSUV_fixed.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ligSUV_no_elements1.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ligSUV_no_elements2.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ligSUV_no_elements3.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)     5592 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ligandParams.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/ligandParams_MAL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/malz
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/malz_OBCParams.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/malz_amber
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/metz
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/metz_OBCParams.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/metz_amber
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/data/tests/unlz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.686531 peleffy-1.4.4/peleffy/forcefield/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/forcefield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/forcefield/calculators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/forcefield/forcefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58508 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/forcefield/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/forcefield/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.686531 peleffy-1.4.4/peleffy/solvent/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/solvent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13216 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/solvent/solvent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.690531 peleffy-1.4.4/peleffy/template/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49942 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/template/impact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.690531 peleffy-1.4.4/peleffy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173141 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_alchemistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_forcefields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20376 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62302 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_rotamers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_solvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15132 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20177 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41604 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.694531 peleffy-1.4.4/peleffy/topology/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54962 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/alchemistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31511 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29641 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/rotamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14336 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/topology/zmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.694531 peleffy-1.4.4/peleffy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/utils/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44156 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/utils/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17082 2023-05-08 15:58:55.000000 peleffy-1.4.4/peleffy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:59:08.670531 peleffy-1.4.4/peleffy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-08 15:59:08.000000 peleffy-1.4.4/peleffy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-08 15:59:08.000000 peleffy-1.4.4/peleffy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:59:08.000000 peleffy-1.4.4/peleffy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-08 15:59:08.000000 peleffy-1.4.4/peleffy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-08 15:59:08.694531 peleffy-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-08 15:58:55.000000 peleffy-1.4.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-08 15:58:55.000000 peleffy-1.4.4/versioneer.py
```

### Comparing `peleffy-1.4.3/LICENSE` & `peleffy-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/PKG-INFO` & `peleffy-1.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: peleffy
-Version: 1.4.3
+Version: 1.4.4
 Summary: PELE Force Field Yielder
 Home-page: http://github.com/martimunicoy/peleffy
 Author: Martí Municoy
 Author-email: martimunicoy@gmail.com
 License: MIT
 Keywords: molecular mechanics,forcefield,potential energy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
 
 The peleffy (PELE Force Field Yielder) is a Python package that builds PELE-compatible force field templates.
-
```

### Comparing `peleffy-1.4.3/README.md` & `peleffy-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/complexes/5XXD_SAM.pdb` & `peleffy-1.4.4/peleffy/data/complexes/5XXD_SAM.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/complexes/LIG1_LIG2.pdb` & `peleffy-1.4.4/peleffy/data/complexes/LIG1_LIG2.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/complexes/LYS_BNZ.pdb` & `peleffy-1.4.4/peleffy/data/complexes/LYS_BNZ.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/complexes/complex_test.pdb` & `peleffy-1.4.4/peleffy/data/complexes/complex_test.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/forcefields/GBSA_OBC1-1.0.offxml` & `peleffy-1.4.4/peleffy/data/forcefields/GBSA_OBC1-1.0.offxml`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/forcefields/GBSA_OBC2-1.0.offxml` & `peleffy-1.4.4/peleffy/data/forcefields/GBSA_OBC2-1.0.offxml`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/BHP.mae` & `peleffy-1.4.4/peleffy/data/ligands/BHP.mae`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/BHP.pdb` & `peleffy-1.4.4/peleffy/data/ligands/BHP.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/BNZ.pdb` & `peleffy-1.4.4/peleffy/data/ligands/BNZ.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/LIG1.pdb` & `peleffy-1.4.4/peleffy/data/ligands/LIG1.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/LIG2.pdb` & `peleffy-1.4.4/peleffy/data/ligands/LIG2.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/SAM.pdb` & `peleffy-1.4.4/peleffy/data/ligands/SAM.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/benzamidine.pdb` & `peleffy-1.4.4/peleffy/data/ligands/benzamidine.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/benzene.mae` & `peleffy-1.4.4/peleffy/data/ligands/benzene.mae`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/benzene.pdb` & `peleffy-1.4.4/peleffy/data/ligands/benzene.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/benzene_without_connectivity.pdb` & `peleffy-1.4.4/peleffy/data/ligands/benzene_without_connectivity.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/ethylene.mae` & `peleffy-1.4.4/peleffy/data/ligands/ethylene.mae`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/ethylene.pdb` & `peleffy-1.4.4/peleffy/data/ligands/ethylene.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/ligand.pdb` & `peleffy-1.4.4/peleffy/data/ligands/ligand.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/malonate.mae` & `peleffy-1.4.4/peleffy/data/ligands/malonate.mae`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/malonate.pdb` & `peleffy-1.4.4/peleffy/data/ligands/malonate.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/modified_sidechain.pdb` & `peleffy-1.4.4/peleffy/data/ligands/modified_sidechain.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/octafluorocyclobutane.pdb` & `peleffy-1.4.4/peleffy/data/ligands/octafluorocyclobutane.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/oleic_acid.pdb` & `peleffy-1.4.4/peleffy/data/ligands/oleic_acid.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/propionic_acid.pdb` & `peleffy-1.4.4/peleffy/data/ligands/propionic_acid.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/toluene.mae` & `peleffy-1.4.4/peleffy/data/ligands/toluene.mae`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/toluene.pdb` & `peleffy-1.4.4/peleffy/data/ligands/toluene.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/trimethylglycine.pdb` & `peleffy-1.4.4/peleffy/data/ligands/trimethylglycine.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/ligands/trimethylglycine_moved.pdb` & `peleffy-1.4.4/peleffy/data/ligands/trimethylglycine_moved.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/parameters/OBCparam.json` & `peleffy-1.4.4/peleffy/data/parameters/OBCparam.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/parameters/f14_sgbnp.param` & `peleffy-1.4.4/peleffy/data/parameters/f14_sgbnp.param`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/parameters/similarity.param` & `peleffy-1.4.4/peleffy/data/parameters/similarity.param`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/parameters/solventParamsHCTOBC.txt` & `peleffy-1.4.4/peleffy/data/parameters/solventParamsHCTOBC.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/CO1_ffld_output.txt` & `peleffy-1.4.4/peleffy/data/tests/CO1_ffld_output.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ETL_ffld_output.txt` & `peleffy-1.4.4/peleffy/data/tests/ETL_ffld_output.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ETL_openff-1.2.1_opls2005_parameters1.json` & `peleffy-1.4.4/peleffy/data/tests/ETL_openff-1.2.1_opls2005_parameters1.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ETL_openff-1.2.1_opls2005_parameters2.json` & `peleffy-1.4.4/peleffy/data/tests/ETL_openff-1.2.1_opls2005_parameters2.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ETL_openff-1.2.1_parameters.json` & `peleffy-1.4.4/peleffy/data/tests/ETL_openff-1.2.1_parameters.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ETL_opls2005_parameters.json` & `peleffy-1.4.4/peleffy/data/tests/ETL_opls2005_parameters.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ETL_solventParamsHCTOBC.txt` & `peleffy-1.4.4/peleffy/data/tests/ETL_solventParamsHCTOBC.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MAL_ffld_output.txt` & `peleffy-1.4.4/peleffy/data/tests/MAL_ffld_output.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MAL_solventParamsHCTOBC.txt` & `peleffy-1.4.4/peleffy/data/tests/MAL_solventParamsHCTOBC.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MAT.mae` & `peleffy-1.4.4/peleffy/data/tests/MAT.mae`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MAT.pdb` & `peleffy-1.4.4/peleffy/data/tests/MAT.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_ffld_output.txt` & `peleffy-1.4.4/peleffy/data/tests/MET_ffld_output.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters1.json` & `peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters1.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters2.json` & `peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters2.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters3.json` & `peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters3.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters4.json` & `peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters4.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters5.json` & `peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_opls2005_parameters5.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_openff-1.2.1_parameters.json` & `peleffy-1.4.4/peleffy/data/tests/MET_openff-1.2.1_parameters.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_opls2005_parameters.json` & `peleffy-1.4.4/peleffy/data/tests/MET_opls2005_parameters.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_parameters_to_json.json` & `peleffy-1.4.4/peleffy/data/tests/MET_parameters_to_json.json`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_parameters_to_string.txt` & `peleffy-1.4.4/peleffy/data/tests/MET_parameters_to_string.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MET_solventParamsHCTOBC.txt` & `peleffy-1.4.4/peleffy/data/tests/MET_solventParamsHCTOBC.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MRO_oleic/HEM.pdb` & `peleffy-1.4.4/peleffy/data/tests/MRO_oleic/HEM.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/MRO_oleic/OLC.pdb` & `peleffy-1.4.4/peleffy/data/tests/MRO_oleic/OLC.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/OLC_ffld_output.txt` & `peleffy-1.4.4/peleffy/data/tests/OLC_ffld_output.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/OPLS_etlz` & `peleffy-1.4.4/peleffy/data/tests/OPLS_etlz`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/OPLS_etlz_amber` & `peleffy-1.4.4/peleffy/data/tests/OPLS_etlz_amber`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/OPLS_malz` & `peleffy-1.4.4/peleffy/data/tests/OPLS_malz`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/OPLS_malz_amber` & `peleffy-1.4.4/peleffy/data/tests/OPLS_malz_amber`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/OPLS_metz` & `peleffy-1.4.4/peleffy/data/tests/OPLS_metz`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/OPLS_metz_amber` & `peleffy-1.4.4/peleffy/data/tests/OPLS_metz_amber`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/OXO_ffld_output.txt` & `peleffy-1.4.4/peleffy/data/tests/OXO_ffld_output.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/alchemical_ligandParams_0.txt` & `peleffy-1.4.4/peleffy/data/tests/alchemical_ligandParams_1.txt`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9847222222222223%*

 * *Differences: {"'SolventParameters'": "{'HYB': {'_C1_': {'radius': 1.625, 'scale': 0.755}, '_N1_': {'radius': "*

 * *                        "1.625, 'scale': 0.755}, '_C2_': {'radius': 1.625, 'scale': 0.755}, "*

 * *                        "'_C3_': {'scale': 0.36}, '_C4_': {'scale': 0.36}, '_C5_': {'scale': "*

 * *                        "0.36}, '_O1_': {'scale': 0.425}, '_O2_': {'scale': 0.425}, '_H1_': "*

 * *                        "{'radius': 1.25}, '_H2_': {'radius': 1.25}, '_H3_': {'scale': 0.425}, "*

 * *                        "'_H4_': { […]*

```diff
@@ -4,130 +4,130 @@
             "solute_dielectric": 1,
             "solvent_dielectric": 78.5,
             "solvent_radius": 1.4,
             "surface_area_penalty": 0.0054
         },
         "HYB": {
             "C10_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.7,
+                "scale": 0.36
             },
             "C11_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.7,
+                "scale": 0.36
             },
             "H10_": {
                 "radius": 1.2,
-                "scale": 0.85
+                "scale": 0.425
             },
             "H11_": {
                 "radius": 1.2,
-                "scale": 0.85
+                "scale": 0.425
             },
             "H12_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.2,
+                "scale": 0.425
             },
             "H13_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.2,
+                "scale": 0.425
             },
             "H14_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.2,
+                "scale": 0.425
             },
             "H15_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.2,
+                "scale": 0.425
             },
             "H16_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.2,
+                "scale": 0.425
             },
             "_C1_": {
-                "radius": 1.7,
-                "scale": 0.72
+                "radius": 1.625,
+                "scale": 0.755
             },
             "_C2_": {
-                "radius": 1.7,
-                "scale": 0.72
+                "radius": 1.625,
+                "scale": 0.755
             },
             "_C3_": {
                 "radius": 1.7,
-                "scale": 0.72
+                "scale": 0.36
             },
             "_C4_": {
                 "radius": 1.7,
-                "scale": 0.72
+                "scale": 0.36
             },
             "_C5_": {
                 "radius": 1.7,
-                "scale": 0.72
+                "scale": 0.36
             },
             "_C6_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.7,
+                "scale": 0.36
             },
             "_C7_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.7,
+                "scale": 0.36
             },
             "_C8_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.7,
+                "scale": 0.36
             },
             "_C9_": {
-                "radius": 0.0,
-                "scale": 0.0
+                "radius": 1.7,
+                "scale": 0.36
             },
             "_H1_": {
-                "radius": 1.2,
+                "radius": 1.25,
                 "scale": 0.85
             },
             "_H2_": {
-                "radius": 1.2,
+                "radius": 1.25,
                 "scale": 0.85
             },
             "_H3_": {
                 "radius": 1.2,
-                "scale": 0.85
+                "scale": 0.425
             },
             "_H4_": {
-                "radius": 1.2,
+                "radius": 1.25,
                 "scale": 0.85
             },
             "_H5_": {
                 "radius": 1.2,
-                "scale": 0.85
+                "scale": 0.425
             },
             "_H6_": {
                 "radius": 1.2,
-                "scale": 0.85
+                "scale": 0.425
             },
             "_H7_": {
                 "radius": 1.2,
-                "scale": 0.85
+                "scale": 0.425
             },
             "_H8_": {
                 "radius": 1.2,
-                "scale": 0.85
+                "scale": 0.425
             },
             "_H9_": {
                 "radius": 1.2,
-                "scale": 0.85
+                "scale": 0.425
             },
             "_N1_": {
-                "radius": 1.55,
-                "scale": 0.79
+                "radius": 1.625,
+                "scale": 0.755
             },
             "_O1_": {
                 "radius": 1.5,
-                "scale": 0.85
+                "scale": 0.425
             },
             "_O2_": {
                 "radius": 1.5,
-                "scale": 0.85
+                "scale": 0.425
             }
         },
         "Name": "OBC2"
     }
 }
```

### Comparing `peleffy-1.4.3/peleffy/data/tests/alchemical_ligandParams_2.txt` & `peleffy-1.4.4/peleffy/data/tests/alchemical_ligandParams_2.txt`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954861111111111%*

 * *Differences: {"'SolventParameters'": "{'HYB': {'_C3_': {'radius': 1.7}, '_C4_': {'radius': 1.7}, '_C5_': "*

 * *                        "{'radius': 1.7}, '_O1_': {'radius': 1.5}, '_O2_': {'radius': 1.5}, "*

 * *                        "'_H3_': {'radius': 1.2}, '_H5_': {'radius': 1.2}, '_H6_': {'radius': "*

 * *                        "1.2}, '_H7_': {'radius': 1.2}, '_H8_': {'radius': 1.2}, '_H9_': "*

 * *                        "{'radius': 1.2}, 'H10_': {'radius': 1.2}, 'H11_': {'radius': 1.2}}}"}*

```diff
@@ -12,19 +12,19 @@
                 "scale": 0.72
             },
             "C11_": {
                 "radius": 1.7,
                 "scale": 0.72
             },
             "H10_": {
-                "radius": 0.0,
+                "radius": 1.2,
                 "scale": 0.0
             },
             "H11_": {
-                "radius": 0.0,
+                "radius": 1.2,
                 "scale": 0.0
             },
             "H12_": {
                 "radius": 1.2,
                 "scale": 0.85
             },
             "H13_": {
@@ -48,23 +48,23 @@
                 "scale": 0.79
             },
             "_C2_": {
                 "radius": 1.55,
                 "scale": 0.79
             },
             "_C3_": {
-                "radius": 0.0,
+                "radius": 1.7,
                 "scale": 0.0
             },
             "_C4_": {
-                "radius": 0.0,
+                "radius": 1.7,
                 "scale": 0.0
             },
             "_C5_": {
-                "radius": 0.0,
+                "radius": 1.7,
                 "scale": 0.0
             },
             "_C6_": {
                 "radius": 1.7,
                 "scale": 0.72
             },
             "_C7_": {
@@ -84,50 +84,50 @@
                 "scale": 0.85
             },
             "_H2_": {
                 "radius": 1.3,
                 "scale": 0.85
             },
             "_H3_": {
-                "radius": 0.0,
+                "radius": 1.2,
                 "scale": 0.0
             },
             "_H4_": {
                 "radius": 1.3,
                 "scale": 0.85
             },
             "_H5_": {
-                "radius": 0.0,
+                "radius": 1.2,
                 "scale": 0.0
             },
             "_H6_": {
-                "radius": 0.0,
+                "radius": 1.2,
                 "scale": 0.0
             },
             "_H7_": {
-                "radius": 0.0,
+                "radius": 1.2,
                 "scale": 0.0
             },
             "_H8_": {
-                "radius": 0.0,
+                "radius": 1.2,
                 "scale": 0.0
             },
             "_H9_": {
-                "radius": 0.0,
+                "radius": 1.2,
                 "scale": 0.0
             },
             "_N1_": {
                 "radius": 1.7,
                 "scale": 0.72
             },
             "_O1_": {
-                "radius": 0.0,
+                "radius": 1.5,
                 "scale": 0.0
             },
             "_O2_": {
-                "radius": 0.0,
+                "radius": 1.5,
                 "scale": 0.0
             }
         },
         "Name": "OBC2"
     }
 }
```

### Comparing `peleffy-1.4.3/peleffy/data/tests/alchemical_mol1.pdb` & `peleffy-1.4.4/peleffy/data/tests/alchemical_mol1.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/alchemical_mol2.pdb` & `peleffy-1.4.4/peleffy/data/tests/alchemical_mol2.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/alchemical_structure.pdb` & `peleffy-1.4.4/peleffy/data/tests/alchemical_structure.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ethylene_error1.pdb` & `peleffy-1.4.4/peleffy/data/tests/ethylene_error1.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ethylene_error2.pdb` & `peleffy-1.4.4/peleffy/data/tests/ethylene_error2.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ethylene_error3.pdb` & `peleffy-1.4.4/peleffy/data/tests/ethylene_error3.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/etlz` & `peleffy-1.4.4/peleffy/data/tests/etlz`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/etlz_amber` & `peleffy-1.4.4/peleffy/data/tests/etlz_amber`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ligSUV_fixed.pdb` & `peleffy-1.4.4/peleffy/data/tests/ligSUV_fixed.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ligSUV_no_elements1.pdb` & `peleffy-1.4.4/peleffy/data/tests/ligSUV_no_elements1.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ligSUV_no_elements2.pdb` & `peleffy-1.4.4/peleffy/data/tests/ligSUV_no_elements2.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ligSUV_no_elements3.pdb` & `peleffy-1.4.4/peleffy/data/tests/ligSUV_no_elements3.pdb`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ligandParams.txt` & `peleffy-1.4.4/peleffy/data/tests/ligandParams.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/ligandParams_MAL.txt` & `peleffy-1.4.4/peleffy/data/tests/ligandParams_MAL.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/malz` & `peleffy-1.4.4/peleffy/data/tests/malz`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/malz_amber` & `peleffy-1.4.4/peleffy/data/tests/malz_amber`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/metz` & `peleffy-1.4.4/peleffy/data/tests/metz`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/metz_amber` & `peleffy-1.4.4/peleffy/data/tests/metz_amber`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/data/tests/unlz` & `peleffy-1.4.4/peleffy/data/tests/unlz`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/forcefield/calculators.py` & `peleffy-1.4.4/peleffy/forcefield/calculators.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,22 @@
     """
     Implementation of the gasteiger partial charge calculator (using
     RDKit).
     """
 
     _name = 'gasteiger'
 
+class MullikenCalculator(_PartialChargeCalculator):
+    """
+    Implementation of the Mulliken partial charge calculator (using
+    RDKit).
+    """
+
+    _name = 'mulliken'
+
 
 class OPLSChargeCalculator(_PartialChargeCalculator):
     """
     Implementation of the calculator of OPLS partial charges (using
     Schrodinger's ffld_server)
     """
```

### Comparing `peleffy-1.4.3/peleffy/forcefield/forcefield.py` & `peleffy-1.4.4/peleffy/forcefield/forcefield.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/forcefield/parameters.py` & `peleffy-1.4.4/peleffy/forcefield/parameters.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/forcefield/selectors.py` & `peleffy-1.4.4/peleffy/forcefield/selectors.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,20 +88,22 @@
     """
     It defines a charge calculator selector.
     """
 
     from peleffy.forcefield.calculators import (OPLSChargeCalculator,
                                                 Am1bccCalculator,
                                                 GasteigerCalculator,
-                                                DummyChargeCalculator)
+                                                DummyChargeCalculator,
+                                                MullikenCalculator)
 
     _AVAILABLE_TYPES = {'opls2005': OPLSChargeCalculator,
                         'am1bcc': Am1bccCalculator,
                         'gasteiger': GasteigerCalculator,
-                        'dummy': DummyChargeCalculator
+                        'dummy': DummyChargeCalculator,
+                        'mulliken': MullikenCalculator
                         }
 
     def get_by_name(self, charge_method, molecule):
         """
         Given a charge method name, it returns the corresponding
         charge calculator class.
```

### Comparing `peleffy-1.4.3/peleffy/main.py` & `peleffy-1.4.4/peleffy/main.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/solvent/solvent.py` & `peleffy-1.4.4/peleffy/solvent/solvent.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/template/impact.py` & `peleffy-1.4.4/peleffy/template/impact.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_alchemistry.py` & `peleffy-1.4.4/peleffy/tests/test_alchemistry.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_conformers.py` & `peleffy-1.4.4/peleffy/tests/test_conformers.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_forcefields.py` & `peleffy-1.4.4/peleffy/tests/test_forcefields.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,29 @@
         calculator = openff._get_charge_calculator('gasteiger', dummy_mol)
 
         assert isinstance(
             calculator,
             peleffy.forcefield.calculators.GasteigerCalculator), \
             'Invalid custom selection 1 for the charge calculator'
 
-        # Check custom selection 1
+        # Check custom selection 2
         openff = OpenForceField(self.FORCE_FIELD_NAME)
         calculator = openff._get_charge_calculator('opls2005', dummy_mol)
 
         assert isinstance(
             calculator,
             peleffy.forcefield.calculators.OPLSChargeCalculator), \
             'Invalid custom selection 2 for the charge calculator'
 
+        # Check custom selection 3
+        openff = OpenForceField(self.FORCE_FIELD_NAME)
+        calculator = openff._get_charge_calculator('mulliken', dummy_mol)
+        assert isinstance(calculator, peleffy.forcefield.calculators.MullikenCalculator), \
+            "Invalid custom selection 3 for the charge calculator"
+
     def test_parameterizer(self):
         """It checks the parameterized method."""
 
         from peleffy.topology import Molecule
         from peleffy.forcefield import OpenForceField
         from peleffy.utils import (get_data_file_path,
                                    convert_all_quantities_to_string)
```

### Comparing `peleffy-1.4.3/peleffy/tests/test_integrity.py` & `peleffy-1.4.4/peleffy/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_main.py` & `peleffy-1.4.4/peleffy/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_mapper.py` & `peleffy-1.4.4/peleffy/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_molecule.py` & `peleffy-1.4.4/peleffy/tests/test_molecule.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_parameters.py` & `peleffy-1.4.4/peleffy/tests/test_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -918,14 +918,28 @@
         # Parameterize
         ff = OpenForceField(FORCEFIELD_NAME)
         parameters = ff.parameterize(molecule, charge_method='gasteiger')
 
         # Check charges
         check_CHO_charges(parameters)
 
+    def test_mulliken_method(self):
+        """It tests the mulliken method"""
+        ligand_path = get_data_file_path(self.LIGAND_PATH)
+
+        # Load molecule
+        molecule = Molecule(ligand_path)
+
+        # Parameterize
+        ff = OpenForceField(FORCEFIELD_NAME)
+        parameters = ff.parameterize(molecule, charge_method='mulliken')
+
+        # Check charges
+        check_CHO_charges(parameters)
+        
     def test_OPLS_method(self):
         """It tests the OPLS method"""
 
         ligand_path = get_data_file_path(self.LIGAND_PATH)
 
         # Load molecule
         molecule = Molecule(ligand_path)
```

### Comparing `peleffy-1.4.3/peleffy/tests/test_rotamers.py` & `peleffy-1.4.4/peleffy/tests/test_rotamers.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_solvent.py` & `peleffy-1.4.4/peleffy/tests/test_solvent.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_templates.py` & `peleffy-1.4.4/peleffy/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_toolkits.py` & `peleffy-1.4.4/peleffy/tests/test_toolkits.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_topology.py` & `peleffy-1.4.4/peleffy/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/test_utils.py` & `peleffy-1.4.4/peleffy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/tests/utils.py` & `peleffy-1.4.4/peleffy/tests/utils.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/topology/alchemistry.py` & `peleffy-1.4.4/peleffy/topology/alchemistry.py`

 * *Files 1% similar despite different names*

```diff
@@ -982,14 +982,20 @@
                                coul2_lambda=None, vdw_lambda=None,
                                bonded_lambda=None):
         """
         It saves the alchemical OBC parameters, which is the combination
         of the OBC parameters of both molecules, to the path that
         is supplied.
 
+        Note that OBC radii are never shrinked to 0.0 for exclusive
+        and non native atoms to avoid problems with the equation
+        that places this parameter as the denominator of a fraction.
+        Instead the scale factor is changed according to the
+        value of the lambda.
+
         Parameters
         ----------
         path : str
             The path where to save the OBC parameters template
         fep_lambda : float
             The value to define an FEP lambda. This lambda affects
             all the parameters. It needs to be contained between
@@ -1067,22 +1073,22 @@
         scales1 = alchemical_obc_params._scales[0]
         radii2 = mol2_obc_params._radii[0]
         scales2 = mol2_obc_params._scales[0]
 
         for atom_idx, atom in enumerate(self._joint_topology.atoms):
             if atom_idx in self._exclusive_atoms:
                 lambda_value = 1.0 - lambda_set.get_lambda_for_coulomb1()
-                radius = radii1[(atom_idx, )] * lambda_value
+                radius = radii1[(atom_idx, )]  # Do not change it
                 scale = scales1[(atom_idx, )] * lambda_value
 
             elif atom_idx in self._non_native_atoms:
                 for mol2_index, alc_index in self._mol2_to_alc_map.items():
                     if alc_index == atom_idx:
                         lambda_value = lambda_set.get_lambda_for_coulomb2()
-                        radius = radii2[(mol2_index, )] * lambda_value
+                        radius = radii2[(mol2_index, )]  # Do not change it
                         scale = scales2[(mol2_index, )] * lambda_value
                         break
                 else:
                     logger.error(['Error: mapping for atom index ' +
                                   f'{atom_idx} not found in the ' +
                                   'hybrid molecule'])
                     radius = 0
@@ -1102,14 +1108,29 @@
             alchemical_obc_params._radii[0][(atom_idx, )] = radius
             alchemical_obc_params._scales[0][(atom_idx, )] = scale
 
         alchemical_obc_params.to_file(path)
 
         logger.set_level(log_level)
 
+    def to_png(self, output_png):
+        """
+        It generates a PNG image representing the resulting alchemical
+        mapping.
+
+        Parameters
+        ----------
+        output_png : str
+            Path to the output PNG file to write
+        """
+        import os
+        from peleffy.utils.toolkits import RDKitToolkitWrapper
+
+        self._mapper.to_png(output_png)
+
     def _ipython_display_(self):
         """
         It returns a representation of the alchemical mapping.
 
         Returns
         -------
         mapping_representation : an IPython display object
```

### Comparing `peleffy-1.4.3/peleffy/topology/conformer.py` & `peleffy-1.4.4/peleffy/topology/conformer.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/topology/elements.py` & `peleffy-1.4.4/peleffy/topology/elements.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/topology/mapper.py` & `peleffy-1.4.4/peleffy/topology/mapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -113,14 +113,44 @@
         Returns
         -------
         molecule2 : a peleffy.topology.Molecule
             The second molecule to map
         """
         return self._molecule2
 
+    def to_png(self, output_png):
+        """
+        It generates a PNG image representing the resulting alchemical
+        mapping.
+
+        Parameters
+        ----------
+        output_png : str
+            Path to the output PNG file to write
+        """
+        import os
+        from peleffy.utils.toolkits import RDKitToolkitWrapper
+
+        extension = os.path.splitext(output_png)[1]
+
+        if extension != ".png":
+            raise ValueError("Invalid extension for a PNG file")
+
+
+        rdkit_toolkit = RDKitToolkitWrapper()
+
+        mcs_mol = rdkit_toolkit.get_mcs(self.molecule1, self.molecule2,
+                                        self._include_hydrogens,
+                                        self._TIMEOUT)
+
+        image = rdkit_toolkit.draw_mapping(self.molecule1, self.molecule2,
+                                           mcs_mol, self._include_hydrogens)
+
+        image.save(output_png)
+
     def _ipython_display_(self):
         """
         It returns a representation of the mapping.
 
         Returns
         -------
         mapping_representation : a IPython display object
```

### Comparing `peleffy-1.4.3/peleffy/topology/molecule.py` & `peleffy-1.4.4/peleffy/topology/molecule.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/topology/rotamer.py` & `peleffy-1.4.4/peleffy/topology/rotamer.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/topology/topology.py` & `peleffy-1.4.4/peleffy/topology/topology.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,7 +424,8 @@
 
         Returns
         -------
         impropers : list[peleffy.topology.Improper]
             The list of impropers of this Topology object.
         """
         return self._impropers
+
```

### Comparing `peleffy-1.4.3/peleffy/topology/zmatrix.py` & `peleffy-1.4.4/peleffy/topology/zmatrix.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/utils/input.py` & `peleffy-1.4.4/peleffy/utils/input.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/utils/output.py` & `peleffy-1.4.4/peleffy/utils/output.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/peleffy/utils/toolkits.py` & `peleffy-1.4.4/peleffy/utils/toolkits.py`

 * *Files 0% similar despite different names*

```diff
@@ -846,15 +846,16 @@
             atom.SetProp('atomLabel', str(atom.GetIdx()))
         for atom in rdkit_mol2.GetAtoms():
             atom.SetProp('atomLabel', str(atom.GetIdx()))
 
         image = Draw.MolsToGridImage([rdkit_mol1, rdkit_mol2],
                                      molsPerRow=2, subImgSize=(300, 300),
                                      legends=[mol1_name, mol2_name],
-                                     highlightAtomLists=[mol1_sub, mol2_sub])
+                                     highlightAtomLists=[mol1_sub, mol2_sub],
+                                     returnPNG=False)
 
         return image
 
     def align_molecules(self, mol1, mol2, atom_mapping=None):
         """
         It aligns the two molecules that are given, taking the first
         one as reference.
@@ -1006,15 +1007,15 @@
         It computes the partial charges using antechamber.
 
         Parameters
         ----------
         molecule : an peleffy.topology.Molecule
             The peleffy's Molecule object
         method : str
-            The name of the method to use. One of ['gasteiger', 'am1bcc'].
+            The name of the method to use. One of ['gasteiger', 'am1bcc', 'mulliken'].
             If None, 'am1bcc' will be used
 
         Returns
         -------
         charges : simtk.unit.Quantity
             The array of partial charges
 
@@ -1023,15 +1024,16 @@
         ChargeMethodUnavailableError if the requested charge method can not
             be handled by this toolkit
         ChargeCalculationError if the charge method is supported by this
             toolkit, but fails
         """
 
         SUPPORTED_CHARGE_METHODS = {'am1bcc': {'antechamber_keyword': 'bcc'},
-                                    'gasteiger': {'antechamber_keyword': 'gas'}
+                                    'gasteiger': {'antechamber_keyword': 'gas'},
+                                    'mulliken': {'antechamber_keyword': 'mul'}
                                     }
 
         if method not in SUPPORTED_CHARGE_METHODS:
             raise ChargeMethodUnavailableError(
                 'partial_charge_method '
                 + '{} is not available from '.format(method)
                 + 'AmberToolsToolkitWrapper. Available charge methods are '
```

### Comparing `peleffy-1.4.3/peleffy/utils/utils.py` & `peleffy-1.4.4/peleffy/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,15 +496,15 @@
         Parameters
         ----------
         level : str
             The logging level to set. One of [DEBUG, INFO, WARNING, ERROR,
             CRITICAL]
         """
         import logging
-        logging.basicConfig()
+        #logging.basicConfig()
 
         if level.upper() == 'DEBUG':
             logging_level = logging.DEBUG
         elif level.upper() == 'INFO':
             logging_level = logging.INFO
         elif level.upper() == 'WARNING':
             logging_level = logging.WARNING
```

### Comparing `peleffy-1.4.3/peleffy.egg-info/PKG-INFO` & `peleffy-1.4.4/peleffy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: peleffy
-Version: 1.4.3
+Version: 1.4.4
 Summary: PELE Force Field Yielder
 Home-page: http://github.com/martimunicoy/peleffy
 Author: Martí Municoy
 Author-email: martimunicoy@gmail.com
 License: MIT
 Keywords: molecular mechanics,forcefield,potential energy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 License-File: LICENSE
 
 The peleffy (PELE Force Field Yielder) is a Python package that builds PELE-compatible force field templates.
-
```

### Comparing `peleffy-1.4.3/peleffy.egg-info/SOURCES.txt` & `peleffy-1.4.4/peleffy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/setup.py` & `peleffy-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `peleffy-1.4.3/versioneer.py` & `peleffy-1.4.4/versioneer.py`

 * *Files identical despite different names*

