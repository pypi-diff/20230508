# Comparing `tmp/pypef-0.2.3.tar.gz` & `tmp/pypef-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypef-0.2.3.tar", last modified: Sat Aug 27 19:19:38 2022, max compression
+gzip compressed data, was "pypef-0.2.4.tar", last modified: Mon May  8 14:22:13 2023, max compression
```

## Comparing `pypef-0.2.3.tar` & `pypef-0.2.4.tar`

### file list

```diff
@@ -1,637 +1,637 @@
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2022-08-27 21:19:38.351179 pypef-0.2.3/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    20254 2022-07-09 09:31:17.000000 pypef-0.2.3/LICENSE.md
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       72 2022-07-09 09:31:17.000000 pypef-0.2.3/MANIFEST.in
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1246 2022-08-27 21:19:38.349179 pypef-0.2.3/PKG-INFO
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    23178 2022-08-23 17:58:07.000000 pypef-0.2.3/README.md
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2022-08-27 21:19:19.164677 pypef-0.2.3/pypef/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1000 2022-08-27 19:41:04.000000 pypef-0.2.3/pypef/__init__.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2022-08-27 21:19:19.557677 pypef-0.2.3/pypef/dca/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.3/pypef/dca/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    29981 2022-08-09 15:09:25.000000 pypef-0.2.3/pypef/dca/encoding.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    37165 2022-08-09 15:09:25.000000 pypef-0.2.3/pypef/dca/hybrid_model.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5101 2022-07-09 06:18:20.000000 pypef-0.2.3/pypef/dca/run.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    20414 2022-08-27 18:11:53.000000 pypef-0.2.3/pypef/main.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2022-08-27 21:19:19.669677 pypef-0.2.3/pypef/ml/
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2022-08-27 21:19:36.965179 pypef-0.2.3/pypef/ml/AAindex/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      594 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ANDN920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ARGP820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ARGP820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ARGP820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      489 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      836 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1161 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      664 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      945 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      470 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AURR980120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      818 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      704 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      639 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      512 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/AVBF000109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1186 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BAEK050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2418 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BASU050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2485 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BASU050102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2873 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BASU050103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      846 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BEGF750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      891 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BEGF750102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      649 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BEGF750103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BHAR880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1002 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BIGC670101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2753 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BIOV880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2581 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BIOV880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      949 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BLAM930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1880 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BLAS910101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      790 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BROC820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BROC820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1419 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BULH740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BULH740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BUNA790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      543 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BUNA790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BUNA790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      938 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BURA740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/BURA740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2179 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CASG920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      977 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CEDJ970101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CEDJ970102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      993 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CEDJ970103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1021 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CEDJ970104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      755 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CEDJ970105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1069 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      546 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM830103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM830104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      697 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM830105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      968 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM830106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      518 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM830107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHAM830108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      978 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOC750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1042 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOC760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1264 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOC760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1659 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOC760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      913 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOC760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1066 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1273 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780202.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1011 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780203.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780204.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780205.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780206.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780207.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780208.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780209.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780210.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780211.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780212.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      733 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780213.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780214.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780215.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1099 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CHOP780216.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1520 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CIDH920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1844 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CIDH920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2110 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CIDH920103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2479 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CIDH920104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2440 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CIDH920105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      439 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/COHE430101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CORJ870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CORJ870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1968 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CORJ870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1838 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CORJ870104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CORJ870105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2012 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CORJ870106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2228 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CORJ870107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2119 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CORJ870108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/COSI940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1140 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/COWR900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CRAJ730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CRAJ730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      825 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/CRAJ730103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      780 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/DAWD720101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1038 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/DAYM780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/DAYM780201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1472 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/DESM900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2134 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/DESM900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/DIGM050101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1899 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/EISD840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1471 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/EISD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/EISD860102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1824 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/EISD860103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ENGD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FASG760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      444 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FASG760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      447 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FASG760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      435 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FASG760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      454 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FASG760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2291 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FASG890101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2454 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1053 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1328 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      931 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      766 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1169 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      767 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      657 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1142 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      865 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      721 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FAUJ880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FINA770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      843 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FINA910101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1071 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FINA910102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      827 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FINA910103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      802 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FINA910104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      537 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FODM020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      995 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1276 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1256 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      759 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      823 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      807 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1000 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      826 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      936 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/FUKS010112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      610 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GARJ730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      902 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      490 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      882 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      923 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      681 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1165 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      529 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      962 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1098 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEIM800111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      592 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      754 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GEOR030109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GOLD730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GOLD730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      499 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GRAR740101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2266 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GRAR740102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      941 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GRAR740103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1884 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GUOD860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2253 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GUYH850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1976 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GUYH850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1867 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GUYH850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1686 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GUYH850104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1275 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/GUYH850105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1005 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/HARY940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/HOPA770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1453 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/HOPT810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/HUTJ700101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/HUTJ700102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      646 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/HUTJ700103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1307 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ISOY800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      706 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ISOY800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ISOY800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ISOY800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ISOY800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ISOY800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ISOY800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ISOY800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1171 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JACR890101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1346 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JANJ780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1885 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JANJ780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1582 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JANJ780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1240 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JANJ790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JANJ790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      897 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JOND750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      686 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JOND750102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      964 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JOND920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JOND920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      887 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JUKT750101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      842 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JUNJ780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2297 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/JURD980101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1090 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KANM800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1397 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KANM800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1356 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KANM800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1078 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KANM800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      972 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARP850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1731 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARP850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARP850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      536 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      532 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      526 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      528 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      559 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      563 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      547 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      567 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      622 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160121.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KARS160122.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      458 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KHAG800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1837 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KIDA850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      611 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KIMC930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      527 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KLEP840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KOEP990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KOEP990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KRIW710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2101 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KRIW790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1518 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KRIW790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KRIW790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1615 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KUHL950101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      808 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KUMS000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      871 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KUMS000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      557 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KUMS000103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KUMS000104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2155 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/KYTJ820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LAWE840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1272 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1019 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      577 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1035 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1124 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      999 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM760107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      919 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM780104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      916 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM780105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1092 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEVM780106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      525 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LEWP710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1861 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LIFS790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      761 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LIFS790102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/LIFS790103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2391 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MANP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1301 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MAXF760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      723 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MAXF760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MAXF760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MAXF760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      690 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MAXF760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MAXF760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      764 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MCMT640101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MEEJ800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1236 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MEEJ800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MEEJ810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1431 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MEEJ810102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2320 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MEIH800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2423 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MEIH800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2265 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MEIH800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      548 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MITS020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2621 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MIYS850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2635 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MIYS990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2617 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MIYS990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2726 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MIYS990103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2703 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MIYS990104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2552 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MIYS990105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      839 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MONM990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MONM990201.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1157 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MUNV940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1128 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MUNV940102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1631 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MUNV940103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MUNV940104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      845 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/MUNV940105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2035 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NADH010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NADH010102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2556 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NADH010103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2296 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NADH010104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1688 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NADH010105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      822 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NADH010106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NADH010107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      888 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAGK730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      782 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAGK730102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      925 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAGK730103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      989 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      756 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      581 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      673 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      545 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      862 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      779 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH900113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      894 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH920101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      660 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH920102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH920103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH920104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH920105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      935 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH920106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH920107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NAKH920108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2079 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NISK800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2601 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NISK860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1331 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/NOZY710101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1313 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OLSK800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      880 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ONEK900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      927 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ONEK900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1871 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      672 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2350 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM770104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM770105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      588 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM850103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM850104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/OOBM850105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      973 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1298 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1060 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1362 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      966 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      638 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      599 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      878 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      875 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      598 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      898 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      621 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PALJ810116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2385 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PARJ860101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1697 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PARS000101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      724 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PARS000102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2257 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PLIV810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1028 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONJ960101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2346 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP800101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP800102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2244 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP800103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP800104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      550 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP800105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      909 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP800106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1315 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP800107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2169 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP800108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2388 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PONP930101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PRAM820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      579 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PRAM820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PRAM820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1575 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PRAM900101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1115 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PRAM900102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PRAM900103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1269 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PRAM900104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1271 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PTIO830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1637 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PTIO830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2481 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PUNT030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2221 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/PUNT030102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      584 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      844 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1127 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1363 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      952 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      996 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      671 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      522 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880118.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1277 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880119.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1622 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880120.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1450 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880121.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880122.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880123.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880124.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880125.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880126.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880127.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880128.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880129.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880130.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      881 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880131.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1185 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880132.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1205 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880133.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880134.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1039 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880135.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880136.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880137.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880138.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/QIAN880139.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1980 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2148 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1487 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1155 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      635 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RACS820114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RADA880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1357 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RADA880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1089 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RADA880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RADA880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      728 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RADA880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      967 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RADA880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1245 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RADA880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2735 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RADA880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      504 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880114.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      630 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880115.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880116.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/RICJ880117.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1109 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      508 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1261 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      854 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1192 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1327 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      488 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      654 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      507 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760111.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      582 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760112.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB760113.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1940 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROBB790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1107 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROSG850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2469 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROSG850102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROSM880101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1823 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROSM880102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      506 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROSM880103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1197 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROSM880104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2001 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ROSM880105.txt
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2022-08-27 21:19:38.078677 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_12_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_0_4.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_1_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_15_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_16_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_0_3.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_1_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_5_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_1_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_4_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_8_0_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_0_7.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_1_4.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_2_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_3_2.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1015 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SIMZ760101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      456 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SNEP660101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      476 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SNEP660102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SNEP660103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SNEP660104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1158 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SUEM840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      684 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SUEM840102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      494 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SUYM030101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1839 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/SWER830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1093 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TAKK010101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      821 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770106.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      669 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770107.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770108.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770109.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1100 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TANS770110.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1036 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TSAJ990101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1040 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/TSAJ990102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VASM830101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VASM830102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VASM830103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VELV850101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1083 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VENT840101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      974 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VHEG790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2392 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VINM940101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2006 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VINM940102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1701 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VINM940103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      705 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/VINM940104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1118 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WARP780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      679 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WEBA780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2230 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WERD780101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WERD780102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WERD780103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      624 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WERD780104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WILM950101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WILM950102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      619 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WILM950103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WILM950104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      856 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WIMW960101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WOEC730101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1070 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WOLR790101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1105 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WOLR810101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2072 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WOLS870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      749 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WOLS870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/WOLS870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/YANJ020101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/YUTK870101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      685 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/YUTK870102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/YUTK870103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/YUTK870104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZASB820101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1677 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZHOH040101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1180 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZHOH040102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2314 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZHOH040103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZIMJ680101.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZIMJ680102.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZIMJ680103.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      562 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZIMJ680104.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.3/pypef/ml/AAindex/ZIMJ680105.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.3/pypef/ml/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5068 2022-07-02 13:59:04.000000 pypef-0.2.3/pypef/ml/parallelization.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    57043 2022-08-27 19:15:52.000000 pypef-0.2.3/pypef/ml/regression.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    10152 2022-08-27 17:56:15.000000 pypef-0.2.3/pypef/ml/run.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2022-08-27 21:19:38.330177 pypef-0.2.3/pypef/utils/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.3/pypef/utils/__init__.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16273 2022-08-09 15:09:25.000000 pypef-0.2.3/pypef/utils/directed_evolution.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    18589 2022-08-27 19:40:02.000000 pypef-0.2.3/pypef/utils/learning_test_sets.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    19261 2022-08-09 15:09:25.000000 pypef-0.2.3/pypef/utils/low_n_mutation_extrapolation.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    17932 2022-07-09 09:10:06.000000 pypef-0.2.3/pypef/utils/prediction_sets.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    17284 2022-07-09 06:24:16.000000 pypef-0.2.3/pypef/utils/run.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     4036 2022-07-02 13:59:04.000000 pypef-0.2.3/pypef/utils/sto2a2m.py
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    10706 2022-08-09 15:09:25.000000 pypef-0.2.3/pypef/utils/variant_data.py
-drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2022-08-27 21:19:19.361177 pypef-0.2.3/pypef.egg-info/
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1246 2022-08-27 21:19:09.000000 pypef-0.2.3/pypef.egg-info/PKG-INFO
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)    21140 2022-08-27 21:19:18.000000 pypef-0.2.3/pypef.egg-info/SOURCES.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        1 2022-08-27 21:19:09.000000 pypef-0.2.3/pypef.egg-info/dependency_links.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       46 2022-08-27 21:19:12.000000 pypef-0.2.3/pypef.egg-info/entry_points.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      102 2022-08-27 21:19:12.000000 pypef-0.2.3/pypef.egg-info/requires.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)        6 2022-08-27 21:19:13.000000 pypef-0.2.3/pypef.egg-info/top_level.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)      111 2022-08-27 21:04:21.000000 pypef-0.2.3/requirements.txt
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)       38 2022-08-27 21:19:38.352181 pypef-0.2.3/setup.cfg
--rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2041 2022-08-27 19:37:09.000000 pypef-0.2.3/setup.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:13.573596 pypef-0.2.4/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    20254 2022-07-09 09:31:17.000000 pypef-0.2.4/LICENSE.md
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       72 2022-07-09 09:31:17.000000 pypef-0.2.4/MANIFEST.in
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1287 2023-05-08 14:22:13.572097 pypef-0.2.4/PKG-INFO
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    24749 2023-01-22 13:21:24.000000 pypef-0.2.4/README.md
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:04.241560 pypef-0.2.4/pypef/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2023-05-08 13:28:24.000000 pypef-0.2.4/pypef/__init__.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:04.350055 pypef-0.2.4/pypef/dca/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.4/pypef/dca/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    29920 2023-05-07 14:00:14.000000 pypef-0.2.4/pypef/dca/encoding.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    41769 2023-05-08 13:38:48.000000 pypef-0.2.4/pypef/dca/hybrid_model.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5289 2023-05-05 17:45:20.000000 pypef-0.2.4/pypef/dca/run.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    21434 2023-05-08 13:27:58.000000 pypef-0.2.4/pypef/main.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:04.399057 pypef-0.2.4/pypef/ml/
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:12.755968 pypef-0.2.4/pypef/ml/AAindex/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      594 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ANDN920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ARGP820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ARGP820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ARGP820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      489 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      469 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      836 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1161 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      664 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      945 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      794 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      470 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      451 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AURR980120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      818 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      704 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      639 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      620 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      512 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/AVBF000109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1186 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BAEK050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2418 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BASU050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2485 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BASU050102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2873 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BASU050103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      846 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BEGF750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      891 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BEGF750102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      649 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BEGF750103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BHAR880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1002 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BIGC670101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2753 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BIOV880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2581 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BIOV880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      949 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BLAM930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1880 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BLAS910101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      790 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BROC820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      640 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BROC820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1419 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BULH740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BULH740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BUNA790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      543 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BUNA790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BUNA790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      938 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BURA740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/BURA740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2179 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CASG920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      977 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      993 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1021 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      755 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CEDJ970105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1069 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      546 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      697 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      968 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      518 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHAM830108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      978 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1042 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1264 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1659 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      913 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOC760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1066 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1273 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1425 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780202.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1011 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780203.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780204.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780205.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780206.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780207.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780208.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780209.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780210.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780211.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780212.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      733 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780213.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780214.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780215.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1099 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CHOP780216.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1844 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2110 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2479 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2440 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CIDH920105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      439 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/COHE430101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1968 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1838 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1882 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2012 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2228 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2119 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CORJ870108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/COSI940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1140 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/COWR900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      963 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CRAJ730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CRAJ730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      825 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/CRAJ730103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      780 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DAWD720101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1038 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DAYM780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DAYM780201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1472 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DESM900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2134 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DESM900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/DIGM050101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1899 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/EISD840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1471 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/EISD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/EISD860102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1824 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/EISD860103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ENGD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      444 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      447 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      435 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      454 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2291 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FASG890101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2454 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1053 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1328 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      931 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      766 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1169 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      767 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      657 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1142 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      865 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      721 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FAUJ880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      843 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA910101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1071 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA910102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      827 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA910103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      802 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FINA910104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      537 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FODM020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      995 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1276 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1256 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      759 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      823 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      807 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1000 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      826 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      936 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/FUKS010112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      610 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GARJ730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      902 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      531 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      490 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      882 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      923 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      681 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1165 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1030 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      529 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      962 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1098 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEIM800111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      592 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      556 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      754 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GEOR030109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GOLD730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1054 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GOLD730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      499 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GRAR740101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2266 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GRAR740102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      941 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GRAR740103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1884 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUOD860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2253 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1976 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1867 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1686 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1275 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/GUYH850105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1005 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HARY940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      538 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HOPA770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1453 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HOPT810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HUTJ700101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HUTJ700102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      646 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/HUTJ700103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1307 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      706 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1017 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      590 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      757 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ISOY800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1171 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JACR890101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1346 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1885 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1582 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1240 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JANJ790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      897 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JOND750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      686 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JOND750102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      964 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JOND920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JOND920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      887 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JUKT750101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      842 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JUNJ780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2297 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/JURD980101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1090 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KANM800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1397 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KANM800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1356 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KANM800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1078 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KANM800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      972 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARP850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1731 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARP850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARP850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      536 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      532 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      526 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      528 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      573 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      564 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      559 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      563 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      547 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      560 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      567 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      622 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160121.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KARS160122.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      458 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KHAG800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1837 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KIDA850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      611 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KIMC930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      527 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KLEP840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KOEP990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      511 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KOEP990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KRIW710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2101 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KRIW790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1518 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KRIW790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1016 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KRIW790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1615 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUHL950101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      808 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUMS000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      871 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUMS000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      557 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUMS000103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      555 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KUMS000104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2155 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/KYTJ820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LAWE840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1272 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1019 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      577 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1035 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1124 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      999 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM760107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      919 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      811 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1073 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      917 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      916 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1092 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEVM780106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      525 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LEWP710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1861 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LIFS790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      761 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LIFS790102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1004 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/LIFS790103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2391 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MANP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1301 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      723 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      772 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      690 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MAXF760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      764 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MCMT640101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      674 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEEJ800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1236 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEEJ800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1625 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEEJ810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1431 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEEJ810102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2320 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEIH800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2423 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEIH800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2265 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MEIH800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      548 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MITS020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2621 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2635 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2617 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2726 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2703 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2552 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MIYS990105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      839 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MONM990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      629 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MONM990201.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1157 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1128 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1631 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      889 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      845 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/MUNV940105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2035 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2467 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2556 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2296 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1688 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      822 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      606 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NADH010107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      888 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAGK730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      782 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAGK730102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      925 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAGK730103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      989 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      756 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      581 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      673 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      682 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      545 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      862 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      779 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      524 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH900113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      894 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      660 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      829 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      935 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      870 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NAKH920108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2079 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NISK800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2601 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NISK860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1331 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/NOZY710101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1313 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OLSK800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      880 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ONEK900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      927 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ONEK900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1871 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      672 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2350 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      553 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM770105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      588 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      542 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/OOBM850105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      973 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1298 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1060 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1362 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      966 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      638 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      599 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      878 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      875 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      598 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      898 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      621 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      632 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PALJ810116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2385 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PARJ860101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1697 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PARS000101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      724 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PARS000102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2257 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PLIV810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1028 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONJ960101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2346 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2238 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2244 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      550 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      909 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1315 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2169 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP800108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2388 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PONP930101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      579 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1575 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM900101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1115 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM900102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM900103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1269 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PRAM900104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1271 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PTIO830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1637 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PTIO830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2481 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PUNT030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2221 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/PUNT030102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      523 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      584 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      844 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1127 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1363 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      952 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      996 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      778 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      671 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      522 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880118.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1277 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880119.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1622 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880120.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1450 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880121.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880122.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880123.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880124.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      521 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880125.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      540 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880126.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      535 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880127.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880128.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880129.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      516 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880130.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      881 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880131.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1185 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880132.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1205 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880133.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1184 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880134.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1039 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880135.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      641 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880136.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880137.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880138.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      515 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/QIAN880139.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1980 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2148 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1487 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      549 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      568 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1155 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      591 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      635 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      612 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      551 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RACS820114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1357 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1089 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      728 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      967 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1245 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2735 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RADA880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      504 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      541 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      520 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      628 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      585 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880114.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      630 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880115.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880116.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      501 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/RICJ880117.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1109 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      508 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1261 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      854 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1192 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1327 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      496 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      668 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      488 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      654 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      507 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760111.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      582 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760112.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      712 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB760113.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1940 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROBB790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1107 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSG850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2469 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSG850102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1630 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1823 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      506 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1197 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2001 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ROSM880105.txt
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:13.464594 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_12_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_0_4.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_1_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_13_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_14_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_15_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_16_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_17_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_0_3.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_18_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_1_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_2_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_4_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_5_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_1_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_7_4_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_8_0_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_0_7.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_1_4.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_2_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      248 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/Refined_cluster_indices_r0.93_r0.97/0.93_0.97_9_3_2.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1015 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SIMZ760101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      456 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SNEP660101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      476 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SNEP660102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      519 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SNEP660103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      457 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SNEP660104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1158 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SUEM840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      684 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SUEM840102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      494 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SUYM030101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1839 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/SWER830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1093 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TAKK010101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1097 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      605 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      821 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      647 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770106.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      669 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770107.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      597 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770108.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      656 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770109.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1100 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TANS770110.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1036 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TSAJ990101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1040 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/TSAJ990102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VASM830101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      570 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VASM830102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      578 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VASM830103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      565 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VELV850101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1083 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VENT840101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      974 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VHEG790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2392 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VINM940101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2006 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VINM940102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1701 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VINM940103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      705 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/VINM940104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1118 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WARP780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      679 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WEBA780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2230 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WERD780101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      626 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WERD780102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      631 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WERD780103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      624 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WERD780104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      834 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WILM950101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      659 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WILM950102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      619 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WILM950103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      627 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WILM950104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      856 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WIMW960101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1497 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOEC730101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1070 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLR790101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1105 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLR810101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2072 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLS870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      749 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLS870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      623 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/WOLS870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      607 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YANJ020101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      771 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YUTK870101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      685 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YUTK870102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YUTK870103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      711 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/YUTK870104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      758 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZASB820101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1677 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZHOH040101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1180 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZHOH040102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2314 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZHOH040103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      517 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680101.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      642 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680102.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      576 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680103.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      562 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680104.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1007 2021-11-13 22:27:22.000000 pypef-0.2.4/pypef/ml/AAindex/ZIMJ680105.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.4/pypef/ml/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     5068 2022-07-02 13:59:04.000000 pypef-0.2.4/pypef/ml/parallelization.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    57666 2023-05-05 21:32:40.000000 pypef-0.2.4/pypef/ml/regression.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    10200 2023-05-05 18:28:24.000000 pypef-0.2.4/pypef/ml/run.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:13.561594 pypef-0.2.4/pypef/utils/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2020-12-13 17:44:24.000000 pypef-0.2.4/pypef/utils/__init__.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    16275 2023-05-05 17:16:29.000000 pypef-0.2.4/pypef/utils/directed_evolution.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    18749 2023-05-08 09:38:22.000000 pypef-0.2.4/pypef/utils/learning_test_sets.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    19505 2023-05-07 16:51:51.000000 pypef-0.2.4/pypef/utils/low_n_mutation_extrapolation.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    18168 2023-05-07 09:07:01.000000 pypef-0.2.4/pypef/utils/prediction_sets.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    17404 2023-05-08 10:45:26.000000 pypef-0.2.4/pypef/utils/run.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     4142 2023-05-05 17:20:37.000000 pypef-0.2.4/pypef/utils/sto2a2m.py
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    12585 2023-05-08 13:38:48.000000 pypef-0.2.4/pypef/utils/variant_data.py
+drwxrwxrwx   0 niklas    (1000) niklas    (1000)        0 2023-05-08 14:22:04.301058 pypef-0.2.4/pypef.egg-info/
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     1287 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/PKG-INFO
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)    21140 2023-05-08 14:22:04.000000 pypef-0.2.4/pypef.egg-info/SOURCES.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        1 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/dependency_links.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       46 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/entry_points.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       96 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/requires.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)        6 2023-05-08 14:22:01.000000 pypef-0.2.4/pypef.egg-info/top_level.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)      105 2022-07-01 13:45:38.000000 pypef-0.2.4/requirements.txt
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)       38 2023-05-08 14:22:13.574097 pypef-0.2.4/setup.cfg
+-rwxrwxrwx   0 niklas    (1000) niklas    (1000)     2129 2023-05-08 10:04:52.000000 pypef-0.2.4/setup.py
```

### Comparing `pypef-0.2.3/LICENSE.md` & `pypef-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/PKG-INFO` & `pypef-0.2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pypef
-Version: 0.2.3
+Version: 0.2.4
 Summary: A command-line interface (CLI) tool for performing data-driven protein engineering by building machine learning (ML)-trained regression models from sequence variant fitness data (in CSV format) based on different techniques for protein sequence encoding. Next to building pure ML models, 'hybrid modeling' is also possible using a blended model optimized for predictive contributions of a statistical and an ML-based prediction.
 Home-page: https://github.com/niklases/PyPEF
 Author: Niklas Siedhoff & Alexander-Maurice Illig
 Author-email: n.siedhoff@biotec.rwth-aachen.de
 License: CC BY-NC-SA 4.0
 Keywords: Pythonic Protein Engineering Framework
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
+Requires-Python: >= 3.9, < 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 For detailed description including a short Jupyter Notebook-based tutorial please refer to the GitHub page.
-
```

### Comparing `pypef-0.2.3/README.md` & `pypef-0.2.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,59 +12,81 @@
 
 <sup>*1*</sup><sub>Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany</sub> <br>
 <sup>*2*</sup><sub>DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany</sub> <br>
 <sup>*3*</sup><sub>Department of Bioorganic Chemistry, Leibniz Institute of Plant Biochemistry, Weinberg 3, 06120 Halle, Germany</sub> <br>
 <sup>*\**</sup><sub>Corresponding author</sub> <br>
 <sup>*§*</sup><sub>Equal contribution</sub> <br>
 
+---
+## Table of Contents
+- [PyPEF](#pypef)
+- [Installation](#installation)
+- [Requirements](#requirements)
+- [Running Examples](#examples)
+- [Tutorial](#tutorial)
+- [Encoding Technique Options](#encoding-options)
+- [Modeling Techniques](#modeling-techniques)
+    - [Pure Machine Learning (ML)-based Modeling](#pure-ml)
+    - [Hybrid Modeling](#hybrid-modeling)
+- [Model Hyperparameter Grids for Training](#grids)
+- [Setting Up the Scripts Yourself](#set-up)
+- [Preprocessing for DCA-based Sequence Encoding](#dca-preprocessing)
+- [API Usage for Sequence Encoding](#api-usage)
+---
+
+<a name="pypef"></a>
 # PyPEF: Pythonic Protein Engineering Framework
 
 a framework written in Python 3 for performing sequence-based machine learning-assisted protein engineering to predict a protein's fitness from its sequence. Written by Niklas Siedhoff and Alexander-Maurice Illig.
 
-<img src="workflow/test_dataset_aneh/exemplary_validation_color_plot.png" alt="drawing" width="500"/>
-
+<p align="center">
+    <img src="workflow/test_dataset_aneh/exemplary_validation_color_plot.png" alt="drawing" width="500"/>
+</p>
 
 Protein engineering by rational or random approaches generates data that can aid the construction of self-learned sequence-function landscapes to predict beneficial variants by using probabilistic methods that can screen the unexplored sequence space with uncertainty *in silico*. Such predictive methods can be applied for increasing the success/effectivity of an engineering campaign while partly offering the prospect to reveal (higher-order) epistatic effects. Here we present an engineering framework termed PyPEF for assisting the supervised training and testing of regression models for predicting beneficial combinations of (identified) amino acid substitutions using machine learning algorithms from the [Scikit-learn](https://github.com/scikit-learn/scikit-learn) package. As training input, the developed framework requires the variant sequences and the corresponding screening results (fitness labels) of the identified variants as CSV (or FASTA-like datasets following a self-defined convention). Using linear or nonlinear regression methods (partial least squares (PLS), Ridge, Lasso, Elastic net, support vector machines (SVR), random forest (RF), and multilayer perceptron (MLP)-based regression), PyPEF trains on the given learning data while optimizing model hyperparameters (default: five-fold cross-validation) and can compute model performances on left-out test data. As sequences are encoded using amino acid descriptor sets taken from the [AAindex database](https://www.genome.jp/aaindex/), finding the best index-dependent encoding for a specific test set can be seen as a hyperparameter search on the test set. In addition, one-hot and [direct coupling analysis](https://en.wikipedia.org/wiki/Direct_coupling_analysis)-based feature generation are implemented as sequence encoding techniques, which often outperform AAindex-based encoding techniques. Finally, the selected or best identified encoding technique and regression model can be used to perform directed evolution walks *in silico* (see [Church-lab implementation](https://github.com/churchlab/UniRep) or the [reimplementation](https://github.com/ivanjayapurna/low-n-protein-engineering)) or to predict natural diverse or recombinant variant sequences that subsequently are to be designed and validated in the wet-lab.
 
 For detailed information, please refer to the above-mentioned publications and related Supporting Information.
 
 The workflow procedure is explained in the [Jupyter notebook](/workflow/Workflow_PyPEF.ipynb) (.ipynb) protocol (see
 Tutorial section below).
 
 <img src="workflow/Splitting_Workflow.png" alt="drawing" width="1000"/>
 
+<a name="installation"></a>
 ## Quick Installation
 A quick installation of the PyPEF command line framework using PyPI for Linux and Windows for **Python 3.9** can be performed with:
 
 ```
 pip install -U pypef
 ```
 
 After successful installation, PyPEF should work by calling `pypef` in the shell:
 
 ```
 pypef --help
 ```
 
-The detailed routine for setting up a new virtual environment with Anaconda, installing the necessary Python packages for that environment, and running the Jupyter notebook tutorial can be found below in the Tutorial section.
+The detailed routine for setting up a new virtual environment with Anaconda, installing the necessary Python packages for that environment, and running the Jupyter notebook tutorial can be found below in the Tutorial section. Further, executable files for running PyPEF on a single core are available at https://github.com/niklases/PyPEF/releases/tag/v0.2.3-alpha.
 
+<a name="requirements"></a>
 ## Requirements
-- Python 3.9
+- Python >=3.9
     - numpy
     - pandas
     - tqdm
     - docopt
     - matplotlib
     - scipy
     - adjustText
     - scikit-learn
     - biopython
     - schema
-    - ray[default]
+    - ray[default] (<2.0.0)
 
+<a name="examples"></a>
 ## Running Examples
 Printing the help function:   
 ```
 pypef --help
 ```
 
 Creating sets for model learning and testing:
@@ -126,19 +148,20 @@
 
 The use of the hybrid model (`pypef hybrid`) - instead of a pure ML model (`pypef ml`) as described in the steps above - is quite similar in terms of commands, but does not require the definition of the `-e`/`--encoding` and the `--regressor` flags, since it depends only on the DCA-based encoding technique and (so far) only uses Ridge regression for modeling. However, DCA-based encoding of sequences always requires a parameter file as input, which comes from the preprocessing of a query-specific multiple sequence alignment (MSA) and results in the parameter file generated by [plmc](https://github.com/debbiemarkslab/plmc). E.g. for training a model on a learning set and testing it on a test set, the command for hybrid modeling is:
 
 ```
 pypef hybrid -l LEARNING_SET.FASTA -t TEST_SET.FASTA --params PLMC_FILE.params
 ``` 
 
-Sample files for testing PyPEF routines are provided in the [workflow/test_dataset](/workflow/test_dataset) directory, which is also used when running the notebook tutorial. PyPEF's package dependencies are linked [here](https://github.com/niklases/PyPEF/network/dependencies).
+Sample files for testing PyPEF routines are provided in the workflow directory, which are also used when running the notebook tutorial. PyPEF's package dependencies are linked [here](https://github.com/niklases/PyPEF/network/dependencies).
 Further, for designing your own API based on the PyPEF workflow, modules can be adapted from the [source code](/pypef).
 
-As standard input files, PyPEF requires the target protein wild-type sequence in [FASTA](https://en.wikipedia.org/wiki/FASTA) format and variant-fitness data in [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) format to split the collected variant-fitness data in learning and test sets that resemble the aligned FASTA format and additionally contain lines indicating the fitness of each corresponding variant (see [sample files](workflow/test_dataset)).
+As standard input files, PyPEF requires the target protein wild-type sequence in [FASTA](https://en.wikipedia.org/wiki/FASTA) format and variant-fitness data in [CSV](https://en.wikipedia.org/wiki/Comma-separated_values) format to split the collected variant-fitness data in learning and test sets that resemble the aligned FASTA format and additionally contain lines indicating the fitness of each corresponding variant (see [ANEH sample files](workflow/test_dataset_aneh), [avGFP sample files](workflow/test_dataset_avgfp), and [MERGE SSM & DMS files](https://github.com/Protein-Engineering-Framework/MERGE/tree/main/Data/_variant_fitness_wtseq)).
 
+<a name="tutorial"></a>
 ## Tutorial
 Before starting running the tutorial, it is a good idea to set-up a new Python environment using Anaconda, https://www.anaconda.com/, e.g. using [Anaconda](https://www.anaconda.com/products/individual) ([Anaconda3-2020.11-Linux-x86_64.sh installer download](https://repo.anaconda.com/archive/Anaconda3-2020.11-Linux-x86_64.sh)) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 Change to the download directory and run the installation, e.g. in Linux:
 
 ```
 bash Anaconda3-2020.11-Linux-x86_64.sh
 ```
@@ -172,26 +195,27 @@
 Note that the package [Ray](https://github.com/ray-project/ray) which we use for parallelizing sequence encoding and model validation of AAindices on the test set, is in beta status for [Windows](https://docs.ray.io/en/latest/installation.html#windows-support).
 
 Now, after installing required packages, you should be able to directly run pypef in the command-line interface.
 
 To run the tutorial after installing required packages either from the conda YAML environment file, the TEXT requirement file, or after installing packages using the pip version of PyPEF, open a Jupyter notebook. If you have installed Anaconda, Jupyter notebook and other commonly used packages for scientific computing and data science should be already installed in Python. If not, you can also install Jupyter via `python3 -m pip install ipython jupyter`. To use the pypef environment as a specified kernel inside the Jupyter notebook, you need to install `ipykernel` and set the kernel name:
 
 ```
-python3 -m pip install ipykernel
+python3 -m pip install ipykernel jupyter
 python3 -m ipykernel install --user --name=pypef
 ```
 
 Now change the directory to ./workflow (`cd workflow`) and run the .ipynb file:
 
 ```
 jupyter-notebook
 ```
 
 Copy the notebook URL in your internet browser and select the Workflow_PyPEF.ipynb file to open it. Now you can select the pypef Python environment at the top notebook menu: Kernel > Change kernel > pypef (otherwise you would use your default Python version as environment, i.e. you would have to install the required packages for this interpreter as well; for this case the installation of the prerequisite packages can also be done within the notebook in provided code fields). 
 
+<a name="encoding-options"></a>
 ## Encoding Technique Options
 - AAindex: Sequence encoding based on AAindex descriptor sets; e.g. using AAindex https://www.genome.jp/entry/aaindex:ARGP820101 for encoding and without subsequent fast Fourier transform (FFT) of the encoded sequence:<br> 
     &nbsp;&nbsp;sequence 'MKLLF' --> [1.18, 1.15,	1.53,	1.53,	2.02]<br>
     and with FFT of the encoded sequence:<br> 
     &nbsp;&nbsp;sequence 'MKLLF' --> [0.0000,	1.0000,	0.1435,	0.3010]<br>
 - OneHot: Occurence of a specific amino acid at a specific residue position indicated as a 1 and elso as a 0:<br> 
     &nbsp;&nbsp;sequence 'MKLLF' --><br>
@@ -201,44 +225,49 @@
      &nbsp;&nbsp;&nbsp;&nbsp;0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, <br>
      &nbsp;&nbsp;&nbsp;&nbsp;0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0&nbsp;]<br>
     
 - DCA: Direct coupling analysis of multiple sequence alignments to extract evolutionary query-specific features. DCA-based features will be generated from the local and coupling terms of the parameter file (paramfile) output by [plmc](https://github.com/debbiemarkslab/plmc) for each target variant sequence. This encoding technique generally outperforms the other encoding techniques described here, but depends on finding and aligning a minimum set of evolutionarily related/homologous sequences - which is not possible for every target sequence. Preprocessing steps for generating the paramfile based on a target sequence are described in the [hybrid model repository](https://github.com/Protein-Engineering-Framework/Hybrid_Model/blob/main/Examples/example_pabp.ipynb). Unlike the other encoding techniques presented, this evolution-based encoding technique is system-specific rather than amino acid-specific, i.e. it does not treat each amino acid the same, but according to its evolutionary position- and coupling-specific history. The DCA-based encoding technique is further also provided for constructing a pure ML model:<br> 
   &nbsp;&nbsp;sequence 'MKLLF' --> [2.3445, 1.3294, 1.6245, 0.8901, 3.2317]&nbsp;&nbsp;, while<br>
   &nbsp;&nbsp;sequence 'MKLKF' --> [2.3472, 1.3601, 1.5431, 1.3749, 3.0186]&nbsp;&nbsp;.  
 
+<a name="modeling-techniques"></a>
 ## Modeling Techniques
+<a name="pure-ml"></a>
 ### Pure Machine Learning (ML)-based Modeling
 Serveral linear and non-linear modeling options are available by default to construct supervised regression models based on the generated sequence features, i.e. encoded sequences. 
 Regression models are trained, i.e. model hyperparameters are optimized, by *k*- fold (by default, fivefold) cross-validation on training samples. Here, the model aims to map the encoded variant sequences that are the features (***X***) for predicting the corresponding fitness labels (***y***) such that *f(***X***)* --> ***y*** – while cross-validation and/or using a model implementing a penalty will be necessary for better model generalization behavior.
 Following regression options from [Scikit-learn](https://scikit-learn.org/stable/) are implemented (for optimized hyperparameters, see Model Hyperparameters section below):
 - [Partial Least Squares Regression (linear model)](https://scikit-learn.org/stable/modules/generated/sklearn.cross_decomposition.PLSRegression.html)
 - [Lasso Regression (fit with Least Angle Regression, L1-penalty regularized linear model)](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LassoLars.html)
 - [Ridge Regression (L2-penalty regularized linear model)](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html)
 - [ElasticNet Regression (combined L1- and L2-penalty regularized linear model)](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.ElasticNet.html)
 - [Support Vector Machines Regression (nonlinear model)](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html)
 - [Random Forest Regression (nonlinear ensemble model)](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)
 - [Multilayer-Perceptron Regression ("Deep" learning with a single hidden layer, nonlinear model)](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html)
 
-### Hybrid Modeling 
-Optimization of the two model contributions to the final hybrid model using the [differential evolution](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.differential_evolution.html) algorithm (see the [hybrid model preprint](https://www.biorxiv.org/content/10.1101/2022.06.07.495081v1)); only based on DCA-derived features (therefore no definition of the flag `-e`, `--encoding` necessary for hybrid modeling):
-- DCA-based statistical prediction of the evolutionary energy of a variant relative to the wild type (see [EVmutation](https://marks.hms.harvard.edu/evmutation/); [EVmutation repository](https://github.com/debbiemarkslab/EVmutation)/[EVcouplings repository](https://github.com/debbiemarkslab/EVcouplings)).
+<a name="hybrid-modeling"></a>
+### Hybrid Modeling Using the MERGE Method
+Optimization of the two model contributions to the final hybrid model using the [differential evolution](https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.differential_evolution.html) algorithm (see the [hybrid model preprint](https://www.biorxiv.org/content/10.1101/2022.06.07.495081v1) and the corresponding repository of the method termed [MERGE](https://github.com/Protein-Engineering-Framework/MERGE)); only based on DCA-derived features (therefore no definition of the flag `-e`, `--encoding` necessary for hybrid modeling):
+- DCA-based statistical prediction of the evolutionary energy, i.e., probability, of a variant relative to the wild type (see [EVmutation](https://marks.hms.harvard.edu/evmutation/); [EVmutation repository](https://github.com/debbiemarkslab/EVmutation)/[EVcouplings repository](https://github.com/debbiemarkslab/EVcouplings)).
 - ML-based supervised training with Ridge regression on training subsets of DCA-encoded sequences and the corresponding fitness values (similar to the pure ML approach using the DCA-based encoding technique in combination with Ridge regression)
 
+<a name="grids"></a>
 ## Model Hyperparameter Grids for Training
 The following model hyperparameter ranges are tested during (*k*-fold) cross-validation for optimized model generalization:
 |Regression model|Hyperparameter grid|
 |:--------------:|:-----------------:|
 | PLS | N_components= {1, 2, 3, ..., 9} |
 | Ridge | regularization param. = {1.000E-06, 1.322E-06, 1.748E-06, ..., 1.000E06} *(numpy.logspace(-6, 6, 100))* |
 | LassoLars | regularization param. = {1.000E-06, 1.322E-06, 1.748E-06, ..., 1.000E06} *(numpy.logspace(-6, 6, 100))* |
 | ElasticNet | regularization param. = {1.000E-06, 1.322E-06, 1.748E-06, ..., 1.000E06} *(numpy.logspace(-6, 6, 100))* |
 | SVR | regularization param. = {2^0, 2^2, 2^4, 2^6, 2^8, 2^10, 2^12},<br>kernel coefficient = {1E−01, 1E−02, 1E−03, 1E−04, 1E−05} |
 | RF | N_trees = {100, 250, 500, 1000},<br>max. features = {all features, sqrt(all features), log2(all features)} |
 | MLP | single hidden layer size = {1, 2, ..., 12},<br>solver = {ADAM, L-BFGS},<br>initial learning rate = {0.001, 0.01, 0.1} |
 
+<a name="set-up"></a>
 ## Setting Up the Scripts Yourself
 PyPEF was developed to be run from a command-line interface while `python3 ./pypef/main.py` (when using the downloaded version of this repository and setting the `PYTHONPATH`) is equal to `pypef` when installed with pip. 
 Downloading/cloning the repository files (manually or with `wget`/`git clone`):<br>
 ```
 wget https://github.com/niklases/PyPEF/archive/main.zip
 ```
 
@@ -275,14 +304,15 @@
 ```
 
 &nbsp;&nbsp;Linux
 ```
 python3 ./pypef/main.py
 ```
 
+<a name="dca-preprocessing"></a>
 ## Preprocessing for DCA-based Sequence Encoding
 
 1. Downloading sequence database (e.g. UniRef100):
 ```
 wget https://ftp.uniprot.org/pub/databases/uniprot/uniref/uniref100/uniref100.fasta.gz
 ```
 
@@ -312,9 +342,14 @@
 pypef ml -e dca -l LS.fasta -t TS.fasta --regressor pls --params ANEH_72.6.params
 ```
 Or for hybrid modeling:
 ```
 pypef hybrid -l LS.fasta -t TS.fasta --params ANEH_72.6.params
 ```
 
+<a name="api-usage"></a>
 ## API Usage for Sequence Encoding
-For script-based encoding of sequences using PyPEF and the available AAindex-, OneHot- or DCA-based techniques, the classes and corresponding functions can be imported, i.e. `OneHotEncoding`, `AAIndexEncoding`, `DCAEncoding`, and `DCAHybridModel`. In addition, implemented functions for CV-based tuning of regression models can be used to train and validate models, eventually deriving them to obtain performances on retained data for testing. An exemplary script for CV-based tuning of models and using them for testing is provided at [workflow/api_encoding_train_test.py](workflow/api_encoding_train_test.py).
+For script-based encoding of sequences using PyPEF and the available AAindex-, OneHot- or DCA-based techniques, the classes and corresponding functions can be imported, i.e. `OneHotEncoding`, `AAIndexEncoding`, `DCAEncoding`, and `DCAHybridModel`. In addition, implemented functions for CV-based tuning of regression models can be used to train and validate models, eventually deriving them to obtain performances on retained data for testing. An exemplary script for CV-based (low-*N*) tuning of models and using them for testing is provided at [workflow/api_encoding_train_test.py](workflow/api_encoding_train_test.py).
+
+<p align="center">
+    <img src="workflow/low_N_avGFP_extrapolation.png" alt="drawing" width="500"/>
+</p>
```

### Comparing `pypef-0.2.3/pypef/__init__.py` & `pypef-0.2.4/pypef/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
 
-VERSION = '0.2.3-alpha'
+__version__ = '0.2.4-alpha'
```

### Comparing `pypef-0.2.3/pypef/dca/encoding.py` & `pypef-0.2.4/pypef/dca/encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,23 +35,25 @@
 See also:
 Hopf, T. A., Ingraham, J. B., Poelwijk, F.J., Schärfe, C.P.I., Springer, M., Sander, C., & Marks, D. S. (2016).
 Mutation effects predicted from sequence co-variation. Nature Biotechnology, in press.
 """
 
 
 from collections.abc import Iterable  # originally imported 'from collections'
+import logging
+logger = logging.getLogger('pypef.dca.encoding')
 
 import numpy as np
 import ray
 from tqdm import tqdm
 from pypef.utils.variant_data import amino_acids
 
 
 _SLICE = np.s_[:]
-np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)
+# np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)  # DEV
 
 class InvalidVariantError(Exception):
     """
     Description
     -----------
     Exception raised when entered variant does not follow the required scheme
     (integer enclosed by two one letter code representations of amino acids).
@@ -69,15 +71,15 @@
         message = "The entered variant '%s' does not follow the required scheme " \
                   "(integer enclosed by two one letter code representations of amino acids). " \
                   "Check separator or variant." % self.variant
         self.message = message
         super().__init__(self.message)
 
 
-class ActiveSiteError(Exception):
+class EffectiveSiteError(Exception):
     """
     Description
     -----------
     Exception raised when requested position is not implemented in the DCA model.
 
     Attributes
     ----------
@@ -89,18 +91,18 @@
         Explanation of the error
     """
 
     def __init__(self, position: int, variant: str, verbose: bool = True):
         self.position = position
         self.variant = variant
         self.verbose = verbose
-        message = f"Info: The position {self.position} of variant '{self.variant}' is " \
+        message = f"The position {self.position} of variant '{self.variant}' is " \
                   f"not an effective site in the DCA model and thus cannot be predicted."
         if self.verbose:
-            print(message)
+            logger.info(message)
             self.message = message
             super().__init__(self.message)
 
 
 def is_valid_substitution(substitution: str) -> bool:
     """
     Description
@@ -281,27 +283,24 @@
                 if num not in self.index_list:
                     not_valid.append(num)
                 else:
                     valid.append(num)
             self.wt_aa_pos = []
             for aa, pos in zip(self._target_seq, self.index_list):
                 self.wt_aa_pos.append(str(aa) + str(pos))
-            print(f'Evaluating gap content of PLMC parameter file... '
+            logger.info(f'Evaluating gap content of PLMC parameter file... '
                   f'First amino acid position used in the MSA (PLMC params file) is '
                   f'{self._target_seq[0]}{self.index_list[0]} and the last position '
                   f'used is {self._target_seq[-1]}{self.index_list[-1]}.')
             if len(not_valid) > 0:
-                print(f'\nFurther, non-included positions are:')
-                print(str(not_valid)[1:-1])
+                logger.info(f'Further, non-included positions are:\n{str(not_valid)[1:-1]}')
             if self.verbose:
-                    print(f'\nSummary of all effective positions represented in the MSA '
-                          f'based on wild-type sequence ({len(valid)} encoded positions):')
-                    for aa_pos in self.wt_aa_pos:
-                        print(f'{aa_pos}', end=' ')
-                    print('\n')
+                    logger.info(f'Summary of all effective positions represented in the MSA '
+                                f'based on wild-type sequence ({len(valid)} encoded positions):\n'
+                                f'{str([aa_pos for aa_pos in self.wt_aa_pos])[1:-1]}'.replace("'", ""))
 
             # single site frequencies f_i and fields h_i
             self.f_i, = np.fromfile(
                 f, dtype=(precision, (self.L, self.num_symbols)), count=1
             )
 
             self.h_i, = np.fromfile(
@@ -368,19 +367,16 @@
         sequence : str, or list of chars
             Define a new default sequence for relative Hamiltonian
             calculations (e.g. energy difference relative to wild-type
             sequence).
             Length of sequence must correspond to model length (self.L)
         """
         if len(sequence) != self.L:
-            raise ValueError(
-                "Sequence length inconsistent with model length: {} {}".format(
-                    len(sequence), self.L
-                )
-            )
+            raise ValueError(f"Sequence length inconsistent with model length: {len(sequence)} {self.L}")
+
 
         if isinstance(sequence, str):
             sequence = list(sequence)
 
         self._target_seq = np.array(sequence)
         self.target_seq_mapped = np.array([self.alphabet_map[x] for x in self.target_seq])
         self.has_target_seq = True
@@ -401,19 +397,15 @@
         Parameters
         ----------
         mapping: list of int
             Sequence indices of the positions in the model.
             Length of list must correspond to model length (self.L)
         """
         if len(mapping) != self.L:
-            raise ValueError(
-                "Mapping length inconsistent with model length: {} {}".format(
-                    len(mapping), self.L
-                )
-            )
+            raise ValueError(f"Mapping length inconsistent with model length: {len(mapping)} {self.L}")
 
         self._index_list = np.array(mapping)
         self.index_map = {b: a for a, b in enumerate(self.index_list)}
 
     def __map(self, indices, mapping):
         """
         Applies a mapping either to a single index, or to a list of indices
@@ -426,17 +418,15 @@
         Returns
         -------
         Iterable, or single item
             Items mapped into new space
         """
         if ((isinstance(indices, Iterable) and not isinstance(indices, str)) or
                 (isinstance(indices, str) and len(indices) > 1)):
-            return np.array(
-                [mapping[i] for i in indices]
-            )
+            return np.array([mapping[i] for i in indices])
         else:
             return mapping[indices]
 
     def __4d_access(self, matrix, i=None, j=None, A_i=None, A_j=None):
         """
         Provides shortcut access to column pair properties
         (e.g. J_ij or f_ij matrices)
@@ -457,14 +447,15 @@
         np.array
             4D matrix "matrix" sliced according to values i, j, A_i and A_j
         """
         i = self.__map(i, self.index_map) if i is not None else _SLICE
         j = self.__map(j, self.index_map) if j is not None else _SLICE
         A_i = self.__map(A_i, self.alphabet_map) if A_i is not None else _SLICE
         A_j = self.__map(A_j, self.alphabet_map) if A_j is not None else _SLICE
+
         return matrix[i, j, A_i, A_j]
 
     def __2d_access(self, matrix, i=None, A_i=None):
         """
         Provides shortcut access to single-column properties
         (e.g. f_i or h_i matrices)
 
@@ -478,14 +469,15 @@
         Returns
         -------
         np.array
             2D matrix "matrix" sliced according to values i and A_i
         """
         i = self.__map(i, self.index_map) if i is not None else _SLICE
         A_i = self.__map(A_i, self.alphabet_map) if A_i is not None else _SLICE
+
         return matrix[i, A_i]
 
     def Jij(self, i=None, j=None, A_i=None, A_j=None):
         """
         Quick access to J_ij matrix with automatic index mapping.
         See __4d_access for explanation of parameters.
         """
@@ -566,14 +558,15 @@
         -------
         Ji : float
             Sum of all site-site interaction terms acting on position 'i' when occupied with 'A_i'.
         """
         Ji = 0.0
         for j, A_j in zip(self.index_list, sequence):
             Ji += self.Jij(i=i, A_i=A_i, j=j, A_j=A_j)
+
         return Ji
 
     @staticmethod
     def _unpack_substitution(substitution: str) -> tuple:
         """
         Description
         -----------
@@ -629,27 +622,27 @@
         """
         sequence = self.target_seq.copy()
         for substitution in get_single_substitutions(variant, self.separator):  # e.g. A123C/D234E --> A123C, D234C
             wild_type_aa, position, A_i = self._unpack_substitution(substitution)
 
             i = self._get_position_internal(position)
             if not i:
-                raise ActiveSiteError(position, variant, self.verbose)
+                raise EffectiveSiteError(position, variant, self.verbose)
 
             self.check_substitution_naming_against_wt(substitution, variant)
             i_mapped = self.index_map[i]
             sequence[i_mapped] = A_i
 
         X_var = np.zeros(sequence.size, dtype=float)
         for idx, (i, A_i) in enumerate(zip(self.index_list, sequence)):
             X_var[idx] = self.hi(i, A_i) + 0.5 * self.Ji(i, A_i, sequence)
 
         return X_var
 
-    def collect_encoded_sequences(self, variants: list) -> list:
+    def collect_encoded_sequences(self, variants: list) -> np.ndarray:
         """
         Description
         -----------
         Collects all encoded sequences based on input variant names.
 
         Parameters
         ----------
@@ -673,18 +666,18 @@
         if len(variants) == 1:  # do not show progress bar for single variant
             set_silence = True  # thus, also not for directed evolution
         else:
             set_silence = False
         for i, variant in enumerate(tqdm(variants, disable=set_silence)):
             try:
                 encoded_sequences.append(self.encode_variant(variant))
-            except ActiveSiteError:
+            except EffectiveSiteError:
                 encoded_sequences.append([None])
 
-        return encoded_sequences
+        return np.array(encoded_sequences, dtype='object')
 
 
 """
 Below: Some helper functions to run the DCAEncoding class and get 
 the encoded sequences in parallel (threading) using Ray and
 to construct a pandas.DataFrame to store the encoded sequences 
 (features) and the associated fitness values in a CSV file.
@@ -707,15 +700,15 @@
         Variant name, e.g. 'A13E', or 'D127F'. Wild-type sequence
         is defined by substitution to itself, e.g. 'F17F'.
     dca_encode: DCAEncoding class object
         For encoding sequences, see above: class DCAEncoding.
     """
     try:
         encoded_seq = dca_encode.encode_variant(variant)
-    except ActiveSiteError:  # position not included in processed MSA
+    except EffectiveSiteError:  # position not included in processed MSA
         return
 
     return encoded_seq
 
 
 @ray.remote
 def _get_data_parallel(
@@ -744,16 +737,17 @@
     -------
     data : manager.list()
         Filled list with variant names, fitnesses, and encoded sequence.
     """
     for i, (variant, fitness) in enumerate(zip(variants, fitnesses)):
         try:
             data.append([variant, dca_encode.encode_variant(variant), fitness])
-        except ActiveSiteError:  # do not append non-encoded sequences and
+        except EffectiveSiteError:  # do not append non-encoded sequences and
             pass                 # associated fitness values
+
     return data
 
 
 def get_dca_data_parallel(
         variants: list,
         fitnesses: list,
         dca_encode: DCAEncoding,
@@ -781,20 +775,20 @@
     -------
     data: numpy.ndarray
         Filled numpy array including variant names, fitnesses, and encoded sequences.
     non_effective_subs: list
         List of variant names that cannot be used for modelling as they are not effective
         positions in the underlying MSA used for generating local and coupling terms.
     """
-    print(f'{len(variants)} input variants.')
-    print(f'Encoding variant sequences. This might take some time...')
+    logger.info(f'{len(variants)} input variants. Encoding variant sequences. '
+                f'This might take some time...')
 
     idxs_nan = np.array([i for i, b in enumerate(np.isnan(fitnesses)) if b])  # find fitness NaNs
     if idxs_nan.size > 0:  # remove NaNs if present
-        print('Fitness NaNs are:', idxs_nan)
+        logger.info(f'Fitness NaNs are: {idxs_nan}')
         fitnesses = np.delete(fitnesses, idxs_nan)
         variants = np.delete(variants, idxs_nan)
 
     variants_split = np.array_split(variants, threads)    # split array in n_cores pieces
     fitnesses_split = np.array_split(fitnesses, threads)  # for parallelization
     results = ray.get([
         _get_data_parallel.remote(
@@ -806,11 +800,11 @@
     ])
     data = [item for sublist in results for item in sublist]  # fusing all the individual results
 
     variants = [item[0] for item in data]
     encoded_sequences = [item[1] for item in data]
     fitnesses = [item[2] for item in data]
 
-    print(f'{len(data)} variants after NaN-valued and non-effective '
-          f'site-substituted variant (ActiveSiteError) dropping.')
+    logger.info(f'{len(data)} variants after NaN-valued and non-effective '
+                f'site-substituted variant (EffectiveSiteError) dropping.')
 
     return variants, encoded_sequences, fitnesses
```

### Comparing `pypef-0.2.3/pypef/dca/hybrid_model.py` & `pypef-0.2.4/pypef/dca/hybrid_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,31 +16,37 @@
 # *Corresponding author
 # §Equal contribution
 
 # Contains Python code used for the approach presented in our 'hybrid modeling' paper
 # Preprint available at: https://doi.org/10.1101/2022.06.07.495081
 # Code available at: https://github.com/Protein-Engineering-Framework/Hybrid_Model
 
+from __future__ import annotations
+
 import os
-import copy
 import pickle
 from os import listdir
 from os.path import isfile, join
-from typing import Union, List, Tuple, Any
+from typing import Union
+import logging
+logger = logging.getLogger('pypef.dca.hybrid_model')
 
 import numpy as np
+import sklearn.base
 from scipy.stats import spearmanr
 from sklearn.linear_model import Ridge
 from sklearn.model_selection import GridSearchCV, train_test_split
 from scipy.optimize import differential_evolution
+
+import pypef.dca.encoding
 from pypef.utils.variant_data import get_sequences_from_file, remove_nan_encoded_positions
-from pypef.dca.encoding import DCAEncoding, get_dca_data_parallel, get_encoded_sequence, ActiveSiteError
+from pypef.dca.encoding import DCAEncoding, get_dca_data_parallel, get_encoded_sequence, EffectiveSiteError
 from pypef.ml.regression import predictions_out, plot_y_true_vs_y_pred
 
-np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning)
+# np.warnings.filterwarnings('error', category=np.VisibleDeprecationWarning) # DEV
 
 
 class DCAHybridModel:
     alphas = np.logspace(-6, 6, 100)  # Grid for the parameter 'alpha'.
     parameter_range = [(0, 1), (0, 1)]  # Parameter range of 'beta_1' and 'beta_2' with lb <= x <= ub
 
     def __init__(
@@ -217,16 +223,16 @@
         Returns
         -------
         The predicted fitness value-representatives of the hybrid
         model.
         """
         # Uncomment lines below to see if correlation between
         # y_true and y_dca is positive or negative:
-        # print(f'Positive or negative correlation of (all data) y_true '
-        #       f'and y_dca (+/-?): {self._spearmanr_dca:.3f}')
+        # logger.info(f'Positive or negative correlation of (all data) y_true '
+        #             f'and y_dca (+/-?): {self._spearmanr_dca:.3f}')
         if self._spearmanr_dca >= 0:
             return beta_1 * y_dca + beta_2 * y_ridge
         else:  # negative correlation
             return beta_1 * y_dca - beta_2 * y_ridge
 
     def _adjust_betas(
             self,
@@ -433,15 +439,15 @@
             X_train=self.X_train,
             y_train=self.y_train
         )
         if reg is None:
             alpha_ = 'None'
         else:
             alpha_ = f'{reg.alpha:.3f}'
-        print(f'Beta 1 (DCA): {beta_1:.3f}, Beta 2 (ML): {beta_2:.3f} ( '
+        logger.info(f'Beta 1 (DCA): {beta_1:.3f}, Beta 2 (ML): {beta_2:.3f} ( '
               f'regressor: Ridge(alpha={alpha_}))')
         if beta_2 == 0.0:
             alpha = np.nan
         else:
             alpha = reg.alpha
         data.update(
             {f'ls_ts':
@@ -554,15 +560,15 @@
         data: dict
             Performances of the split with size of the
             training set = train_size and size of the
             test set = N_variants - train_size.
         """
         data = {}
         for t, train_size in enumerate(train_sizes):
-            print(t + 1, '/', len(train_sizes), ':', train_size)
+            logger.info(f'{t + 1}/{len(train_sizes)}:{train_size}')
             data.update(self.split_performance(train_size=train_size, n_runs=n_runs))
 
         return data
 
 
 """
 Below: Some helper functions that call or are dependent on the DCAHybridModel class.
@@ -603,15 +609,15 @@
     # getting target (WT) sequence and encoding it to provide it as
     # relative value for pure DCA based predictions (difference in sums
     # of sequence encodings: variant - WT)
     target_seq, index = dca_encoder.get_target_seq_and_index()
     wt_name = target_seq[0] + str(index[0]) + target_seq[0]
     x_wt = get_encoded_sequence(wt_name, dca_encoder)
 
-    print(
+    logger.info(
         f'Train size (fitting): {train_percent_fit*100:.1f} % of training data '
         f'({((1 - test_percent)*train_percent_fit)*100:.1f} % of all data),\n'
         f'Train size validation: {(1 - train_percent_fit)*100:.1f} % of training data '
         f'({((1 - test_percent)*(1 - train_percent_fit))*100:.1f} % of all data),\n'
         f'Test size: {test_percent*100:.1f} % ({test_percent*100:.1f} % of all data),\n'
         f'(Random state: {random_state})...\n'
     )
@@ -632,41 +638,85 @@
         train_percent_fit=train_percent_fit,
         random_state=random_state
     )
     if reg is None:
         alpha_ = 'None'
     else:
         alpha_ = f'{reg.alpha:.3f}'
-    print(
+    logger.info(
         f'Individual model weights and regressor hyperparameters:\n'
         f'Hybrid model individual model contributions:\nBeta1 (DCA): '
         f'{beta_1:.3f}, Beta2 (ML): {beta_2:.3f} ('
         f'regressor: Ridge(alpha={alpha_}))\n'
         f'Test performance: Spearman\'s rho = {test_spearman_r:.3f}'
     )
     try:
         os.mkdir('Pickles')
     except FileExistsError:
         pass
-    print(f'Save model as Pickle file... HYBRIDMODEL')
+    logger.info(f'Save model as Pickle file... HYBRIDMODEL')
     pickle.dump(
         {
-            'hybrid_model': hybrid_model,
+            'model': hybrid_model,
             'beta_1': beta_1,
             'beta_2': beta_2,
             'spearman_rho': test_spearman_r,
             'regressor': reg
         },
         open('Pickles/HYBRIDMODEL', 'wb')
     )
 
 
+def check_model_type(model):
+    """
+    Checks type/instance of loaded Pickle file.
+    """
+    if type(model) == pypef.dca.encoding.DCAEncoding:
+        return 'DCAMODEL'
+    elif type(model) == pypef.dca.hybrid_model.DCAHybridModel:
+        return 'HYBRIDMODEL'
+    elif isinstance(model, sklearn.base.BaseEstimator):
+        raise SystemError("Loaded an sklearn ML model. For pure ML-based modeling the "
+                          "\'ml\' flag has to be used instead of the \'hybrid\' flag.")
+    else:
+        raise SystemError('Unknown model/unknown Pickle file.')
+
+
+def get_delta_e_statistical_model(
+        x_test: np.ndarray,
+        x_wt: np.ndarray
+):
+    """
+    Description
+    -----------
+
+
+    Parameters
+    -----------
+    x_test: np.ndarray [2-dim]
+        Encoded sequences to be subtracted by x_wt to compute delta E.
+    x_wt: np.ndarray [1-dim]
+        Encoded wild-type sequence.
+
+    Returns
+    -----------
+    delta_e: np.ndarray [1-dim]
+        Summed subtracted encoded sequences.
+
+    """
+    delta_x = np.subtract(x_test, x_wt)
+    delta_e = np.sum(delta_x, axis=1)
+
+    return delta_e
+
+
+
 def performance_ls_ts(
-        ls_fasta: str,
-        ts_fasta: str,
+        ls_fasta: str | None,
+        ts_fasta: str | None,
         threads: int,
         params_file: str,
         separator: str
 ):
     """
     Description
     -----------
@@ -697,95 +747,124 @@
 
     Returns
     -----------
     None
         Just plots test results (predicted fitness vs. measured fitness)
         using def plot_y_true_vs_y_pred.
     """
-    _, train_variants, y_train = get_sequences_from_file(ls_fasta)
-    _, test_variants, y_test = get_sequences_from_file(ts_fasta)
-
     dca_encoder = DCAEncoding(
         params_file=params_file,
         separator=separator,
         verbose=False
     )
-
     # DCA prediction: delta E = np.subtract(X, self.x_wild_type),
     # with X = encoded sequence of any variant -->
     # getting wild-type name und subsequently x_wild_type
     # to provide it for the DCAHybridModel
     target_seq, index = dca_encoder.get_target_seq_and_index()
     wt_name = target_seq[0] + str(index[0]) + target_seq[0]
+    logger.info(f'Using to-self-substitution \'{wt_name}\' as wild type reference.')
     x_wt = get_encoded_sequence(wt_name, dca_encoder)
-    if threads > 1:
-        # Hyperthreading, NaNs are already being removed by the called function
-        train_variants, x_train, y_train = get_dca_data_parallel(
-            train_variants, y_train, dca_encoder, threads)
-        test_variants, x_test, y_test = get_dca_data_parallel(
-            test_variants, y_test, dca_encoder, threads)
-    else:
-        x_train_ = dca_encoder.collect_encoded_sequences(train_variants)
-        x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
-        # NaNs must still be removed
-        x_train, train_variants = remove_nan_encoded_positions(copy.copy(x_train_), train_variants)
-        x_train, y_train = remove_nan_encoded_positions(copy.copy(x_train_), y_train)
-        x_test, test_variants = remove_nan_encoded_positions(copy.copy(x_test_), test_variants)
-        x_test, y_test = remove_nan_encoded_positions(copy.copy(x_test_), y_test)
-    assert len(x_train) == len(train_variants) == len(y_train)
-    assert len(x_test) == len(test_variants) == len(y_test)
+    if ls_fasta is not None and ts_fasta is not None:
+        _, train_variants, y_train = get_sequences_from_file(ls_fasta)
+        _, test_variants, y_test = get_sequences_from_file(ts_fasta)
 
-    hybrid_model = DCAHybridModel(
-        X_train=np.array(x_train),
-        y_train=np.array(y_train),
-        X_test=np.array(x_test),
-        y_test=np.array(y_test),
-        X_wt=x_wt
-    )
+        if threads > 1:
+            # Hyperthreading, NaNs are already being removed by the called function
+            train_variants, x_train, y_train = get_dca_data_parallel(
+                train_variants, y_train, dca_encoder, threads)
+            test_variants, x_test, y_test = get_dca_data_parallel(
+                test_variants, y_test, dca_encoder, threads)
+        else:
+            x_train_ = dca_encoder.collect_encoded_sequences(train_variants)
+            x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
+            # NaNs must still be removed
+            x_train, train_variants, y_train = remove_nan_encoded_positions(x_train_, train_variants, y_train)
+            x_test, test_variants, y_test = remove_nan_encoded_positions(x_test_, test_variants, y_test)
+        assert len(x_train) == len(train_variants) == len(y_train)
+        assert len(x_test) == len(test_variants) == len(y_test)
+
+        hybrid_model = DCAHybridModel(
+            X_train=np.array(x_train),
+            y_train=np.array(y_train),
+            X_test=np.array(x_test),
+            y_test=np.array(y_test),
+            X_wt=x_wt
+        )
+        data, y_pred = hybrid_model.ls_ts_performance()
+        result = data['ls_ts']
+        test_spearman_r = result['spearman_rho']
+        beta_1 = result['beta_1']
+        beta_2 = result['beta_2']
+        reg = result['regressor']
+        if reg is None:
+            alpha_ = 'None'
+        else:
+            alpha_ = f'{reg.alpha:.3f}'
+        logger.info(
+            f'Individual model weights and regressor hyperparameters:\n'
+            f'Hybrid model individual model contributions: Beta1 (DCA): '
+            f'{beta_1:.3f}, Beta2 (ML): {beta_2:.3f} (regressor: '
+            f'Ridge(alpha={alpha_}))\nTesting performance...\nSpearman\'s '
+            f'rho = {test_spearman_r:.3f}'
+        )
+        try:
+            os.mkdir('Pickles')
+        except FileExistsError:
+            pass
+        logger.info(f'Save model as Pickle file... HYBRIDMODEL')
+        pickle.dump(
+            {
+                'model': hybrid_model,
+                'beta_1': beta_1,
+                'beta_2': beta_2,
+                'spearman_rho': test_spearman_r,
+                'regressor': reg
+            },
+            open('Pickles/HYBRIDMODEL', 'wb')
+        )
+
+    elif ts_fasta is not None:
+        logger.info('No learning set provided, falling back to statistical DCA model: '
+                    'no adjustments of individual hybrid model parameters (beta_1 and beta_2).')
+        _, test_variants, y_test = get_sequences_from_file(ts_fasta)
+        if threads > 1:
+            test_variants, x_test, y_test = get_dca_data_parallel(
+                test_variants, y_test, dca_encoder, threads)
+        else:
+            x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
+            x_test, y_test, test_variants = remove_nan_encoded_positions(x_test_, y_test, test_variants)
+
+        delta_e = get_delta_e_statistical_model(x_test, x_wt)
+
+        spearman_rho = spearmanr(y_test, delta_e)
+        logger.info(f'Spearman Rho = {spearman_rho[0]:.3f}')
+
+        logger.info(f'Save model as Pickle file... DCAMODEL')
+        pickle.dump(
+            {
+                'model': dca_encoder,
+                'beta_1': None,
+                'beta_2': None,
+                'spearman_rho': spearman_rho,
+                'regressor': None
+            },
+            open('Pickles/DCAMODEL', 'wb')
+        )
 
-    data, y_pred = hybrid_model.ls_ts_performance()
-    result = data['ls_ts']
-    test_spearman_r = result['spearman_rho']
-    beta_1 = result['beta_1']
-    beta_2 = result['beta_2']
-    reg = result['regressor']
-    if reg is None:
-        alpha_ = 'None'
     else:
-        alpha_ = f'{reg.alpha:.3f}'
-    print(
-        f'Individual model weights and regressor hyperparameters:\n'
-        f'Hybrid model individual model contributions: Beta1 (DCA): '
-        f'{beta_1:.3f}, Beta2 (ML): {beta_2:.3f} (regressor: '
-        f'Ridge(alpha={alpha_}))\nTesting performance...\nSpearman\'s '
-        f'rho = {test_spearman_r:.3f}'
-    )
-    try:
-        os.mkdir('Pickles')
-    except FileExistsError:
-        pass
-    print(f'Save model as Pickle file... HYBRIDMODEL')
-    pickle.dump(
-        {
-            'hybrid_model': hybrid_model,
-            'beta_1': beta_1,
-            'beta_2': beta_2,
-            'spearman_rho': test_spearman_r,
-            'regressor': reg
-        },
-        open('Pickles/HYBRIDMODEL', 'wb')
-    )
+        logger.info('No Test Set given for performance estimation.')
 
 
 def predict_ps(  # also predicting "pmult" dirs
         prediction_dict: dict,
         params_file: str,
         threads: int,
         separator: str,
-        hybrid_model_data_pkl: str,
+        model_pickle_file: str,
         test_set: str = None,
         prediction_set: str = None,
         figure: str = None,
         label: bool = False,
         negative: bool = False
 ):
     """
@@ -807,15 +886,15 @@
         in directory './Recomb_Double_Split'.
     params_file: str
         PLMC couplings parameter file
     threads: int
         Threads used for parallelization for DCA-based sequence encoding
     separator: str
         Separator of individual substitution of variants, default '/'
-    hybrid_model_data_pkl: str
+    model_pickle_file: str
         Pickle file containing the hybrid model and model parameters in
         a dictionary format
     test_set: str = None
         Test set for prediction and plotting of predictions (contains
         true fitness values of variants).
     prediction_set: str = None
         Prediction set for prediction, does not contain true fitness values.
@@ -837,85 +916,102 @@
         in the respective created folders).
 
     """
     if threads > 1:  # silent DCA encoding
         dca_encoder = DCAEncoding(params_file, separator=separator, verbose=False)
     else:
         dca_encoder = DCAEncoding(params_file, separator=separator)
-    print(f'Taking regression model from saved model (Pickle file): {hybrid_model_data_pkl}...')
-    hybrid_data = pickle.load(open('Pickles/' + hybrid_model_data_pkl, "rb"))
-    hybrid_model = hybrid_data['hybrid_model']
-    test_spearman_r = hybrid_data['spearman_rho']
-    beta_1 = hybrid_data['beta_1']
-    beta_2 = hybrid_data['beta_2']
-    reg = hybrid_data['regressor']
-    if reg is None:
-        alpha_ = 'None'
-    else:
-        alpha_ = f'{reg.alpha:.3f}'
-    print(
-        f'Individual model weights and regressor hyperparameters:\n'
-        f'Hybrid model individual model contributions: Beta1 (DCA): {beta_1:.3f}, '
-        f'Beta2 (ML): {beta_2:.3f} (regressor: Ridge(alpha={alpha_})), '
-        f'Train->Test performance: Spearman\'s rho = {test_spearman_r:.3f}.'
-    )
+    logger.info(f'Taking regression model from saved model (Pickle file): {model_pickle_file}...')
+    model_data = pickle.load(open(f'Pickles/{model_pickle_file}', "rb"))
+    model = model_data['model']
+    test_spearman_r = model_data['spearman_rho']
+    beta_1 = model_data['beta_1']
+    beta_2 = model_data['beta_2']
+    reg = model_data['regressor']
+
+    if check_model_type(model) == 'DCAMODEL':
+        pass
+    elif check_model_type(model) == 'HYBRIDMODEL':
+        if reg is None:
+            alpha_ = 'None'
+        else:
+            alpha_ = f'{reg.alpha:.3f}'
+        logger.info(
+            f'Individual model weights and regressor hyperparameters:\n'
+            f'Hybrid model individual model contributions: Beta1 (DCA): {beta_1:.3f}, '
+            f'Beta2 (ML): {beta_2:.3f} (regressor: Ridge(alpha={alpha_})), '
+            f'Train->Test performance: Spearman\'s rho = {test_spearman_r:.3f}.'
+        )
+
     pmult = [
         'Recomb_Double_Split', 'Recomb_Triple_Split', 'Recomb_Quadruple_Split',
         'Recomb_Quintuple_Split', 'Diverse_Double_Split', 'Diverse_Triple_Split',
         'Diverse_Quadruple_Split'
     ]
     if True in prediction_dict.values():
         for ps, path in zip(prediction_dict.values(), pmult):
             if ps:  # if True, run prediction in this directory, e.g. for drecomb
-                print(f'Running predictions for variant-sequence files in directory {path}...')
+                logger.info(f'Running predictions for variant-sequence files in directory {path}...')
                 all_y_v_pred = []
                 files = [f for f in listdir(path) if isfile(join(path, f)) if f.endswith('.fasta')]
                 for i, file in enumerate(files):  # collect and predict for each file in the directory
-                    print(f'Encoding files ({i+1}/{len(files)}) for prediction...\n')
+                    logger.info(f'Encoding files ({i+1}/{len(files)}) for prediction...\n')
                     file_path = os.path.join(path, file)
                     sequences, variants, _ = get_sequences_from_file(file_path)
                     if threads > 1:  # parallel execution
                         # NaNs are already being removed by the called function
                         variants, xs, _ = get_dca_data_parallel(
                             variants, list(np.zeros(len(variants))), dca_encoder, threads)
                     else:  # single thread execution
                         xs = dca_encoder.collect_encoded_sequences(variants)
                         # NaNs must still be removed
                         xs, variants = remove_nan_encoded_positions(xs, variants)
                     assert len(xs) == len(variants)
-                    ys_pred = hybrid_model.hybrid_prediction(xs, reg, beta_1, beta_2)
-                    for i, y in enumerate(ys_pred):
-                        all_y_v_pred.append((ys_pred[i], variants[i]))
+                    if check_model_type(model) == 'DCAMODEL':
+                        target_seq, index = dca_encoder.get_target_seq_and_index()
+                        wt_name = target_seq[0] + str(index[0]) + target_seq[0]
+                        x_wt = get_encoded_sequence(wt_name, dca_encoder)
+                        ys_pred = get_delta_e_statistical_model(xs, x_wt)
+                    elif check_model_type(model) == 'HYBRIDMODEL':
+                        ys_pred = model.hybrid_prediction(xs, reg, beta_1, beta_2)
+                    for k, y in enumerate(ys_pred):
+                        all_y_v_pred.append((ys_pred[k], variants[k]))
                 if negative:  # sort by fitness value
                     all_y_v_pred = sorted(all_y_v_pred, key=lambda x: x[0], reverse=False)
                 else:
                     all_y_v_pred = sorted(all_y_v_pred, key=lambda x: x[0], reverse=True)
                 predictions_out(
                     predictions=all_y_v_pred,
                     model='hybrid',
                     prediction_set=prediction_set,
                     path=path
                 )
-            else:  # check next task to do, e.g. predicting trecomb
+            else:  # check next task to do, e.g. predicting triple substituted variants, e.g. trecomb
                 continue
 
     elif prediction_set is not None:
         sequences, variants, _ = get_sequences_from_file(prediction_set)
         # NaNs are already being removed by the called function
         if threads > 1:
             # NaNs are already being removed by the called function
             variants, xs, _ = get_dca_data_parallel(
                 variants, list(np.zeros(len(variants))), dca_encoder, threads)
         else:
             xs = dca_encoder.collect_encoded_sequences(variants)
             # NaNs must still be removed
             xs, variants = remove_nan_encoded_positions(xs, variants)
-            assert len(xs) == len(variants)
+        assert len(xs) == len(variants)
         if prediction_set is not None:
-            y_pred = hybrid_model.hybrid_prediction(xs, reg, beta_1, beta_2)
+            if check_model_type(model) == 'DCAMODEL':
+                target_seq, index = dca_encoder.get_target_seq_and_index()
+                wt_name = target_seq[0] + str(index[0]) + target_seq[0]
+                x_wt = get_encoded_sequence(wt_name, dca_encoder)
+                y_pred = get_delta_e_statistical_model(xs, x_wt)
+            elif check_model_type(model) == 'HYBRIDMODEL':
+                y_pred = model.hybrid_prediction(xs, reg, beta_1, beta_2)
             y_v_pred = zip(y_pred, variants)
             y_v_pred = sorted(y_v_pred, key=lambda x: x[0], reverse=True)
             predictions_out(
                 predictions=y_v_pred,
                 model='hybrid',
                 prediction_set=prediction_set
             )
@@ -924,33 +1020,38 @@
             loaded_set = test_set
         else:
             loaded_set = figure
         sequences, variants, y_true = get_sequences_from_file(loaded_set)
         # NaNs are already being removed by the called function
         try:
             if threads > 1:
-                variants, xs, y_true = get_dca_data_parallel(
+                variants, xs, y_test = get_dca_data_parallel(
                     variants, y_true, dca_encoder, threads)
             else:
                 # NaNs must still be removed
                 xs_ = dca_encoder.collect_encoded_sequences(variants)
-                xs, variants = remove_nan_encoded_positions(copy.copy(xs_), variants)
-                xs, y_test = remove_nan_encoded_positions(copy.copy(xs_), y_true)
-                assert len(xs) == len(variants) == len(y_test)
+                xs, variants, y_test = remove_nan_encoded_positions(xs_, variants, y_true)
+            assert len(xs) == len(variants) == len(y_test)
         except IndexError:
             raise SystemError(
                 "Potentially, you provided a prediction set for plotting the figure "
                 "instead of a test set (including measured fitness values, i.e. y_true)."
             )
-        y_pred = hybrid_model.hybrid_prediction(xs, reg, beta_1, beta_2)
-        print('Testing performance...')
-        print(f'Spearman\'s rho = {spearmanr(y_true, y_pred)[0]:.3f}')
+        if check_model_type(model) == 'DCAMODEL':
+            target_seq, index = dca_encoder.get_target_seq_and_index()
+            wt_name = target_seq[0] + str(index[0]) + target_seq[0]
+            x_wt = get_encoded_sequence(wt_name, dca_encoder)
+            y_pred = get_delta_e_statistical_model(xs, x_wt)
+        elif check_model_type(model) == 'HYBRIDMODEL':
+            y_pred = model.hybrid_prediction(xs, reg, beta_1, beta_2)
+        logger.info('Testing performance...\n'
+                    f'Spearman\'s rho = {spearmanr(y_test, y_pred)[0]:.3f} (N_test = {len(y_pred)})')
         if figure is not None:
             plot_y_true_vs_y_pred(
-                np.array(y_true), np.array(y_pred), np.array(variants), label, hybrid=True
+                np.array(y_test), np.array(y_pred), np.array(variants), label, hybrid=True
             )
     else:
         raise SystemError(
             'Define set(s) for prediction (e.g. \'-p PS.fasta\' or '
             'created prediction set folder, e.g. \'--pmult --drecomb\')'
         )
 
@@ -966,24 +1067,29 @@
     the stored DCAHybridModel and the model parameters to predict the fitness
     of the variant encoded herein using the DCAEncoding class. If the variant
     cannot be encoded (based on the PLMC params file), returns 'skip'. Else,
     returning the predicted fitness value and the variant name.
     """
     try:
         x = encoder.encode_variant(variant)
-    except ActiveSiteError:
+    except EffectiveSiteError:
         return 'skip'
 
     model_dict = pickle.load(open(os.path.join('Pickles', hybrid_model_data_pkl), "rb"))
-    model = model_dict['hybrid_model']
+    model = model_dict['model']
     reg = model_dict['regressor']
     beta_1 = model_dict['beta_1']
     beta_2 = model_dict['beta_2']
-
-    y_pred = model.hybrid_prediction(  # 2d as only single variant
-        X=np.atleast_2d(x),  # e.g., np.atleast_2d(3.0) --> array([[3.]])
-        reg=reg,  # RidgeRegressor
-        beta_1=beta_1,  # DCA model prediction weight
-        beta_2=beta_2  # ML model prediction weight
-    )[0]
+    if check_model_type(model) == 'DCAMODEL':
+        target_seq, index = encoder.get_target_seq_and_index()
+        wt_name = target_seq[0] + str(index[0]) + target_seq[0]
+        x_wt = get_encoded_sequence(wt_name, encoder)
+        y_pred = get_delta_e_statistical_model(np.atleast_2d(x), x_wt)[0]  # [0] only for unpacking from list
+    elif check_model_type(model) == 'HYBRIDMODEL':
+        y_pred = model.hybrid_prediction(  # 2d as only single variant
+            X=np.atleast_2d(x),  # e.g., np.atleast_2d(3.0) --> array([[3.]])
+            reg=reg,  # RidgeRegressor
+            beta_1=beta_1,  # DCA model prediction weight
+            beta_2=beta_2  # ML model prediction weight
+        )[0]  # [0] only for unpacking from list
 
     return [(y_pred, variant[1:])]
```

### Comparing `pypef-0.2.3/pypef/dca/run.py` & `pypef-0.2.4/pypef/dca/run.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,48 +12,49 @@
 # https://doi.org/10.1021/acs.jcim.1c00099
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
-
-import copy
+import logging
+logger = logging.getLogger('pypef.dca.run')
 import ray
 
 from pypef.utils.variant_data import read_csv, remove_nan_encoded_positions
 from pypef.dca.encoding import DCAEncoding, get_dca_data_parallel
 from pypef.dca.hybrid_model import performance_ls_ts, predict_ps, generate_model_and_save_pkl
 from pypef.utils.low_n_mutation_extrapolation import performance_mutation_extrapolation, low_n
 
 
 def run_pypef_hybrid_modeling(arguments):
     threads = abs(arguments['--threads']) if arguments['--threads'] is not None else 1
     threads = threads + 1 if threads == 0 else threads
     if threads > 1:
         ray.init()
-        print(f'Using {threads} threads for running...')
-    print(
+        logger.info(f'Using {threads} threads for running...')
+    logger.info(
         f"Note that the hybrid model only optimizes model performances in terms of "
         f"Spearman's correlation of measured versus predicted values. Further, the "
         f"hybrid approach uses only Ridge regression for supervised ML-based hybrid "
         f"model contribution. In hybrid modeling, the ranks of predictions are "
         f"important and not the exact predicted value."
     )
 
-    if arguments['--ls']:
+    if arguments['--ts']:
         performance_ls_ts(
             ls_fasta=arguments['--ls'],
             ts_fasta=arguments['--ts'],
             threads=threads,
             params_file=arguments['--params'],
             separator=arguments['--mutation_sep']
         )
 
-    if arguments['--params'] and arguments['--model']:
+
+    elif arguments['--params'] and arguments['--model']:
         prediction_dict = {}
         prediction_dict.update({
             'drecomb': arguments['--drecomb'],
             'trecomb': arguments['--trecomb'],
             'qarecomb': arguments['--qarecomb'],
             'qirecomb': arguments['--qirecomb'],
             'ddiverse': arguments['--ddiverse'],
@@ -62,23 +63,23 @@
         })
 
         predict_ps(
             prediction_dict=prediction_dict,
             params_file=arguments['--params'],
             threads=threads,
             separator=arguments['--mutation_sep'],
-            hybrid_model_data_pkl=arguments['--model'],
+            model_pickle_file=arguments['--model'],
             test_set=arguments['--ts'],
             prediction_set=arguments['--ps'],
             figure=arguments['--figure'],
             label=arguments['--label'],
             negative=arguments['--negative']
         )
 
-    if arguments['train_and_save']:
+    elif arguments['train_and_save']:
         dca_encode = DCAEncoding(
             params_file=arguments['--params'],
             separator=arguments['--mutation_sep'],
             verbose=False
         )
 
         variants, fitnesses, _ = read_csv(arguments['--input'])
@@ -88,35 +89,41 @@
                 variants=variants,
                 fitnesses=fitnesses,
                 dca_encode=dca_encode,
                 threads=threads,
             )
         else:  # Single thread, requires deletion of NaNs
             encoded_sequences_ = dca_encode.collect_encoded_sequences(variants)
-            encoded_sequences, variants = remove_nan_encoded_positions(copy.copy(encoded_sequences_), variants)
-            encoded_sequences, fitnesses = remove_nan_encoded_positions(copy.copy(encoded_sequences_), fitnesses)
+            encoded_sequences, variants, fitnesses = remove_nan_encoded_positions(encoded_sequences_, variants, fitnesses)
         assert len(encoded_sequences) == len(variants) == len(fitnesses)
 
         generate_model_and_save_pkl(
             xs=encoded_sequences,
             ys=fitnesses,
             dca_encoder=dca_encode,
             train_percent_fit=arguments['--fit_size'],
             test_percent=arguments['--test_size'],
             random_state=arguments['--rnd_state']
         )
 
-    if arguments['low_n'] or arguments['extrapolation']:
+    elif arguments['low_n'] or arguments['extrapolation']:
         if arguments['low_n']:
             low_n(
                 encoded_csv=arguments['--input'],
                 hybrid_modeling=arguments['hybrid']
             )
         elif arguments['extrapolation']:
             performance_mutation_extrapolation(
                 encoded_csv=arguments['--input'],
                 cv_regressor=arguments['--regressor'],
                 conc=arguments['--conc'],
                 hybrid_modeling=arguments['hybrid']
             )
 
-    print('\nDone!\n')
+    else:
+        performance_ls_ts(
+            ls_fasta=arguments['--ls'],
+            ts_fasta=arguments['--ts'],
+            threads=threads,
+            params_file=arguments['--params'],
+            separator=arguments['--mutation_sep']
+        )
```

### Comparing `pypef-0.2.3/pypef/main.py` & `pypef-0.2.4/pypef/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 # §Equal contribution
 
 
 # docstring for argument parsing using docopts
 """
 PyPEF - Pythonic Protein Engineering Framework
 
+written by Niklas Siedhoff and Alexander-Maurice Illig.
+
 Modeling options
 ----------------
     I. Pure ML modeling
     -------------------
         PyPEF provides three encoding options for training machine learning models, i.e.
         regression models trained by supervised learning:
 
@@ -56,16 +58,16 @@
 
     II. Hybrid modeling
     -------------------
         Constructing a hybrid model that combines pure statistical DCA-based prediction (a
         variant's relative 'evolutionary energy' to the wild type) and DCA-encoding based
         training of a ML model similar to pure ML modeling option I.1.
         Based on features generated from the direct coupling analysis (.params file output
-        by PLMC). Individual model contributions are optimization only based on Spearman's
-        correlation coefficient and thus, only variant fitness ranks are to be considered
+        using the plmc framework). Individual model contributions are optimization only based on
+        Spearman's correlation coefficient and thus, only variant fitness ranks are to be considered
         for evaluating model performance, not the exact predicted fitness value. For regression,
         only L2-regularized linear regression (Ridge regression) is provided as modeling option.
 
 
 Running example of training, testing, and inferring a pure ML model for predictions
 -----------------------------------------------------------------------------------
 Exemplary running of PyPEF for training a pure ML model using encoding option 2
@@ -127,16 +129,16 @@
     pypef encode --input CSV_FILE --encoding ENCODING_TECHNIQUE --wt WT_SEQ
         [--params PLMC_FILE] [--y_wt WT_FITNESS] [--model MODEL12345] [--nofft]
         [--threads THREADS]
         [--sep CSV_COLUMN_SEPARATOR] [--fitness_key FITNESS_KEY]
     pypef shift_pos --input CSV_FILE --offset OFFSET
         [--sep CSV_COLUMN_SEPARATOR] [--mutation_sep MUTATION_SEPARATOR] [--fitness_key FITNESS_KEY]
     pypef sto2a2m --sto STO_MSA_FILE [--inter_gap INTER_GAP] [--intra_gap INTRA_GAP]
-    pypef hybrid --ls LEARNING_SET --ts TEST_SET --params PLMC_FILE
-        [--label] [--threads THREADS]
+    pypef hybrid --params PLMC_FILE --ts TEST_SET
+        [--ls LEARNING_SET] [--label] [--threads THREADS]
     pypef hybrid --model MODEL --params PLMC_FILE
         [--ts TEST_SET]
         [--figure TS_FOR_PLOTTING] [--label]
         [--ps PREDICTION_SET] [--pmult] [--drecomb] [--trecomb] [--qarecomb] [--qirecomb]
                                         [--ddiverse] [--tdiverse] [--qdiverse] [--negative]
         [--threads THREADS]
     pypef hybrid directevo --wt WT_SEQ --model MODEL12345 --params PLMC_FILE
@@ -260,26 +262,48 @@
   onehot                            OneHot-based encoding [default: False].
   shift_pos                         Shift positions of all variant substitutions of the input CSV
                                     file [default: False.]
   sto2a2m                           Transform multiple sequence alignment from STO format to
                                     A2M format [default: False].
 """
 
+from sys import argv, version_info
+from pypef import __version__
+if version_info[0] < 3 or version_info[1] < 9:
+    raise SystemError(f"The current version of PyPEF (v {__version__}) "
+                      f"requires at least Python 3.9 or higher.")
+
+import time
+from datetime import timedelta
+import logging
 
 from docopt import docopt
 from schema import Schema, SchemaError, Optional, Or, Use
 
-from pypef import VERSION
+
 from pypef.ml.run import run_pypef_pure_ml
 from pypef.dca.run import run_pypef_hybrid_modeling
 from pypef.utils.run import run_pypef_utils
 
 
+logger = logging.getLogger("pypef")
+logger.setLevel(logging.INFO)
+
+ch = logging.StreamHandler()
+ch.setLevel(logging.DEBUG)
+
+formatter = logging.Formatter(
+    "%(asctime)s,%(msecs)03d %(levelname)s %(filename)s:%(lineno)d -- %(message)s",
+    "%Y-%m-%d %H:%M:%S"
+)
+ch.setFormatter(formatter)
+logger.addHandler(ch)
+
+
 schema = Schema({
-    # '<name>': str,
     Optional('--all'): bool,
     Optional('--color'): bool,
     Optional('--conc'): bool,
     Optional('--csvaa'): bool,
     Optional('--ddiverse'): bool,
     Optional('--drecomb'): bool,
     Optional('--drop'): Use(float),
@@ -348,22 +372,29 @@
         args = schema.validate(args)
         return args
     except SchemaError as e:
         exit(e)
 
 
 def run_main():
-    arguments = docopt(__doc__, version=VERSION)
-    # print(arguments)  # uncomment line for printing argument dict
+    arguments = docopt(__doc__, version=__version__)
+    start_time = time.time()
+    logger.debug(f'main.py __name__: {__name__}, version: {__version__}')
+    logger.debug(str(argv)[1:-1].replace("\'", "").replace(",", ""))
+    logger.debug(f'\n{arguments}')
     arguments = validate(arguments)
     if arguments['directevo']:
         run_pypef_utils(arguments)
     elif arguments['ml']:
         run_pypef_pure_ml(arguments)
     elif arguments['hybrid']:
         run_pypef_hybrid_modeling(arguments)
     else:
         run_pypef_utils(arguments)
 
+    elapsed = str(timedelta(seconds=time.time()-start_time)).split(".")[0]
+    elapsed = f'{elapsed.split(":")[0]} h {elapsed.split(":")[1]} min {elapsed.split(":")[2]} s'
+    logger.info(f'Done! (Run time: {elapsed})')
+
 
 if __name__ == '__main__':
     run_main()
```

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ANDN920101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ANDN920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ARGP820101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ARGP820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ARGP820102.txt` & `pypef-0.2.4/pypef/ml/AAindex/ARGP820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ARGP820103.txt` & `pypef-0.2.4/pypef/ml/AAindex/ARGP820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AURR980108.txt` & `pypef-0.2.4/pypef/ml/AAindex/AURR980108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AURR980109.txt` & `pypef-0.2.4/pypef/ml/AAindex/AURR980109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AURR980110.txt` & `pypef-0.2.4/pypef/ml/AAindex/AURR980110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AURR980111.txt` & `pypef-0.2.4/pypef/ml/AAindex/AURR980111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AURR980112.txt` & `pypef-0.2.4/pypef/ml/AAindex/AURR980112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AURR980113.txt` & `pypef-0.2.4/pypef/ml/AAindex/AURR980113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AURR980114.txt` & `pypef-0.2.4/pypef/ml/AAindex/AURR980114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AURR980115.txt` & `pypef-0.2.4/pypef/ml/AAindex/AURR980115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000101.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000102.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000103.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000104.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000105.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000106.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000107.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000108.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/AVBF000109.txt` & `pypef-0.2.4/pypef/ml/AAindex/AVBF000109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BAEK050101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BAEK050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BASU050101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BASU050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BASU050102.txt` & `pypef-0.2.4/pypef/ml/AAindex/BASU050102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BASU050103.txt` & `pypef-0.2.4/pypef/ml/AAindex/BASU050103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BEGF750101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BEGF750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BEGF750102.txt` & `pypef-0.2.4/pypef/ml/AAindex/BEGF750102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BEGF750103.txt` & `pypef-0.2.4/pypef/ml/AAindex/BEGF750103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BHAR880101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BHAR880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BIGC670101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BIGC670101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BIOV880101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BIOV880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BIOV880102.txt` & `pypef-0.2.4/pypef/ml/AAindex/BIOV880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BLAM930101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BLAM930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BLAS910101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BLAS910101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BROC820101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BROC820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BROC820102.txt` & `pypef-0.2.4/pypef/ml/AAindex/BROC820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BULH740101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BULH740101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BULH740102.txt` & `pypef-0.2.4/pypef/ml/AAindex/BULH740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BUNA790101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BUNA790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BUNA790102.txt` & `pypef-0.2.4/pypef/ml/AAindex/BUNA790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BUNA790103.txt` & `pypef-0.2.4/pypef/ml/AAindex/BUNA790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BURA740101.txt` & `pypef-0.2.4/pypef/ml/AAindex/BURA740101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/BURA740102.txt` & `pypef-0.2.4/pypef/ml/AAindex/BURA740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CASG920101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CASG920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CEDJ970101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CEDJ970101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CEDJ970102.txt` & `pypef-0.2.4/pypef/ml/AAindex/CEDJ970102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CEDJ970103.txt` & `pypef-0.2.4/pypef/ml/AAindex/CEDJ970103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CEDJ970104.txt` & `pypef-0.2.4/pypef/ml/AAindex/CEDJ970104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CEDJ970105.txt` & `pypef-0.2.4/pypef/ml/AAindex/CEDJ970105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM810101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM820101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM820102.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM830101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM830102.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM830103.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM830103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM830104.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM830104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM830105.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM830105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM830106.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM830106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM830107.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM830107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHAM830108.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHAM830108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOC750101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOC750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOC760101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOC760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOC760102.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOC760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOC760103.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOC760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOC760104.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOC760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780201.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780202.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780202.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780203.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780203.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780204.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780204.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780205.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780205.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780206.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780206.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780207.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780207.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780208.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780208.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780209.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780209.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780210.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780210.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780211.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780211.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780212.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780212.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780213.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780213.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780214.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780214.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780215.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780215.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CHOP780216.txt` & `pypef-0.2.4/pypef/ml/AAindex/CHOP780216.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CIDH920101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CIDH920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CIDH920102.txt` & `pypef-0.2.4/pypef/ml/AAindex/CIDH920102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CIDH920103.txt` & `pypef-0.2.4/pypef/ml/AAindex/CIDH920103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CIDH920104.txt` & `pypef-0.2.4/pypef/ml/AAindex/CIDH920104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CIDH920105.txt` & `pypef-0.2.4/pypef/ml/AAindex/CIDH920105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CORJ870101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CORJ870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CORJ870102.txt` & `pypef-0.2.4/pypef/ml/AAindex/CORJ870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CORJ870103.txt` & `pypef-0.2.4/pypef/ml/AAindex/CORJ870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CORJ870104.txt` & `pypef-0.2.4/pypef/ml/AAindex/CORJ870104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CORJ870105.txt` & `pypef-0.2.4/pypef/ml/AAindex/CORJ870105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CORJ870106.txt` & `pypef-0.2.4/pypef/ml/AAindex/CORJ870106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CORJ870107.txt` & `pypef-0.2.4/pypef/ml/AAindex/CORJ870107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CORJ870108.txt` & `pypef-0.2.4/pypef/ml/AAindex/CORJ870108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/COSI940101.txt` & `pypef-0.2.4/pypef/ml/AAindex/COSI940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/COWR900101.txt` & `pypef-0.2.4/pypef/ml/AAindex/COWR900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CRAJ730101.txt` & `pypef-0.2.4/pypef/ml/AAindex/CRAJ730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CRAJ730102.txt` & `pypef-0.2.4/pypef/ml/AAindex/CRAJ730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/CRAJ730103.txt` & `pypef-0.2.4/pypef/ml/AAindex/CRAJ730103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/DAWD720101.txt` & `pypef-0.2.4/pypef/ml/AAindex/DAWD720101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/DAYM780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/DAYM780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/DAYM780201.txt` & `pypef-0.2.4/pypef/ml/AAindex/DAYM780201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/DESM900101.txt` & `pypef-0.2.4/pypef/ml/AAindex/DESM900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/DESM900102.txt` & `pypef-0.2.4/pypef/ml/AAindex/DESM900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/DIGM050101.txt` & `pypef-0.2.4/pypef/ml/AAindex/DIGM050101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/EISD840101.txt` & `pypef-0.2.4/pypef/ml/AAindex/EISD840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/EISD860101.txt` & `pypef-0.2.4/pypef/ml/AAindex/EISD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/EISD860102.txt` & `pypef-0.2.4/pypef/ml/AAindex/EISD860102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/EISD860103.txt` & `pypef-0.2.4/pypef/ml/AAindex/EISD860103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ENGD860101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ENGD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FASG760101.txt` & `pypef-0.2.4/pypef/ml/AAindex/FASG760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FASG890101.txt` & `pypef-0.2.4/pypef/ml/AAindex/FASG890101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ830101.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880101.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880102.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880103.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880104.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880105.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880106.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880107.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880108.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880109.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880110.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880111.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880112.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FAUJ880113.txt` & `pypef-0.2.4/pypef/ml/AAindex/FAUJ880113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FINA770101.txt` & `pypef-0.2.4/pypef/ml/AAindex/FINA770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FINA910101.txt` & `pypef-0.2.4/pypef/ml/AAindex/FINA910101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FINA910102.txt` & `pypef-0.2.4/pypef/ml/AAindex/FINA910102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FINA910103.txt` & `pypef-0.2.4/pypef/ml/AAindex/FINA910103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FINA910104.txt` & `pypef-0.2.4/pypef/ml/AAindex/FINA910104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FODM020101.txt` & `pypef-0.2.4/pypef/ml/AAindex/FODM020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010101.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010102.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010103.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010104.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010105.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010106.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010107.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010108.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010109.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010110.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010111.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/FUKS010112.txt` & `pypef-0.2.4/pypef/ml/AAindex/FUKS010112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GARJ730101.txt` & `pypef-0.2.4/pypef/ml/AAindex/GARJ730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800101.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800102.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800104.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800105.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800106.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800107.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800108.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800109.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800110.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEIM800111.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEIM800111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030101.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030102.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030103.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030104.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030105.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030106.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030107.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030108.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GEOR030109.txt` & `pypef-0.2.4/pypef/ml/AAindex/GEOR030109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GOLD730101.txt` & `pypef-0.2.4/pypef/ml/AAindex/GOLD730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GOLD730102.txt` & `pypef-0.2.4/pypef/ml/AAindex/GOLD730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GRAR740102.txt` & `pypef-0.2.4/pypef/ml/AAindex/GRAR740102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GRAR740103.txt` & `pypef-0.2.4/pypef/ml/AAindex/GRAR740103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GUOD860101.txt` & `pypef-0.2.4/pypef/ml/AAindex/GUOD860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GUYH850101.txt` & `pypef-0.2.4/pypef/ml/AAindex/GUYH850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GUYH850102.txt` & `pypef-0.2.4/pypef/ml/AAindex/GUYH850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GUYH850103.txt` & `pypef-0.2.4/pypef/ml/AAindex/GUYH850103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GUYH850104.txt` & `pypef-0.2.4/pypef/ml/AAindex/GUYH850104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/GUYH850105.txt` & `pypef-0.2.4/pypef/ml/AAindex/GUYH850105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/HARY940101.txt` & `pypef-0.2.4/pypef/ml/AAindex/HARY940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/HOPA770101.txt` & `pypef-0.2.4/pypef/ml/AAindex/HOPA770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/HOPT810101.txt` & `pypef-0.2.4/pypef/ml/AAindex/HOPT810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/HUTJ700101.txt` & `pypef-0.2.4/pypef/ml/AAindex/HUTJ700101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/HUTJ700102.txt` & `pypef-0.2.4/pypef/ml/AAindex/HUTJ700102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/HUTJ700103.txt` & `pypef-0.2.4/pypef/ml/AAindex/HUTJ700103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ISOY800101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ISOY800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ISOY800102.txt` & `pypef-0.2.4/pypef/ml/AAindex/ISOY800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ISOY800103.txt` & `pypef-0.2.4/pypef/ml/AAindex/ISOY800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ISOY800104.txt` & `pypef-0.2.4/pypef/ml/AAindex/ISOY800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ISOY800105.txt` & `pypef-0.2.4/pypef/ml/AAindex/ISOY800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ISOY800106.txt` & `pypef-0.2.4/pypef/ml/AAindex/ISOY800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ISOY800107.txt` & `pypef-0.2.4/pypef/ml/AAindex/ISOY800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ISOY800108.txt` & `pypef-0.2.4/pypef/ml/AAindex/ISOY800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JACR890101.txt` & `pypef-0.2.4/pypef/ml/AAindex/JACR890101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JANJ780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/JANJ780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JANJ780102.txt` & `pypef-0.2.4/pypef/ml/AAindex/JANJ780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JANJ780103.txt` & `pypef-0.2.4/pypef/ml/AAindex/JANJ780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JANJ790101.txt` & `pypef-0.2.4/pypef/ml/AAindex/JANJ790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JANJ790102.txt` & `pypef-0.2.4/pypef/ml/AAindex/JANJ790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JOND750101.txt` & `pypef-0.2.4/pypef/ml/AAindex/JOND750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JOND750102.txt` & `pypef-0.2.4/pypef/ml/AAindex/JOND750102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JOND920101.txt` & `pypef-0.2.4/pypef/ml/AAindex/JOND920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JUKT750101.txt` & `pypef-0.2.4/pypef/ml/AAindex/JUKT750101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JUNJ780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/JUNJ780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/JURD980101.txt` & `pypef-0.2.4/pypef/ml/AAindex/JURD980101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KANM800101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KANM800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KANM800102.txt` & `pypef-0.2.4/pypef/ml/AAindex/KANM800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KANM800103.txt` & `pypef-0.2.4/pypef/ml/AAindex/KANM800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KANM800104.txt` & `pypef-0.2.4/pypef/ml/AAindex/KANM800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARP850101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARP850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARP850102.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARP850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160102.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160103.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160104.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160105.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160106.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160107.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160108.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160109.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160110.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160111.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160112.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160113.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160114.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160115.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160116.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160117.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160117.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160118.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160118.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160119.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160119.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160120.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160120.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160121.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160121.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KARS160122.txt` & `pypef-0.2.4/pypef/ml/AAindex/KARS160122.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KIDA850101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KIDA850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KIMC930101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KIMC930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KLEP840101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KLEP840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KOEP990101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KOEP990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KRIW710101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KRIW710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KRIW790101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KRIW790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KRIW790102.txt` & `pypef-0.2.4/pypef/ml/AAindex/KRIW790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KRIW790103.txt` & `pypef-0.2.4/pypef/ml/AAindex/KRIW790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KUHL950101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KUHL950101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KUMS000101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KUMS000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KUMS000102.txt` & `pypef-0.2.4/pypef/ml/AAindex/KUMS000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KUMS000103.txt` & `pypef-0.2.4/pypef/ml/AAindex/KUMS000103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KUMS000104.txt` & `pypef-0.2.4/pypef/ml/AAindex/KUMS000104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/KYTJ820101.txt` & `pypef-0.2.4/pypef/ml/AAindex/KYTJ820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LAWE840101.txt` & `pypef-0.2.4/pypef/ml/AAindex/LAWE840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM760101.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM760102.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM760103.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM760104.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM760105.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM760106.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM760107.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM760107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM780102.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM780103.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM780104.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM780104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM780105.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM780105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEVM780106.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEVM780106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LEWP710101.txt` & `pypef-0.2.4/pypef/ml/AAindex/LEWP710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LIFS790101.txt` & `pypef-0.2.4/pypef/ml/AAindex/LIFS790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LIFS790102.txt` & `pypef-0.2.4/pypef/ml/AAindex/LIFS790102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/LIFS790103.txt` & `pypef-0.2.4/pypef/ml/AAindex/LIFS790103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MANP780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MANP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MAXF760101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MAXF760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MAXF760102.txt` & `pypef-0.2.4/pypef/ml/AAindex/MAXF760102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MAXF760103.txt` & `pypef-0.2.4/pypef/ml/AAindex/MAXF760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MAXF760104.txt` & `pypef-0.2.4/pypef/ml/AAindex/MAXF760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MAXF760105.txt` & `pypef-0.2.4/pypef/ml/AAindex/MAXF760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MAXF760106.txt` & `pypef-0.2.4/pypef/ml/AAindex/MAXF760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MCMT640101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MCMT640101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MEEJ800101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MEEJ800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MEEJ800102.txt` & `pypef-0.2.4/pypef/ml/AAindex/MEEJ800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MEEJ810101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MEEJ810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MEEJ810102.txt` & `pypef-0.2.4/pypef/ml/AAindex/MEEJ810102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MEIH800101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MEIH800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MEIH800102.txt` & `pypef-0.2.4/pypef/ml/AAindex/MEIH800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MEIH800103.txt` & `pypef-0.2.4/pypef/ml/AAindex/MEIH800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MITS020101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MITS020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MIYS850101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MIYS850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MIYS990101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MIYS990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MIYS990102.txt` & `pypef-0.2.4/pypef/ml/AAindex/MIYS990102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MIYS990103.txt` & `pypef-0.2.4/pypef/ml/AAindex/MIYS990103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MIYS990104.txt` & `pypef-0.2.4/pypef/ml/AAindex/MIYS990104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MIYS990105.txt` & `pypef-0.2.4/pypef/ml/AAindex/MIYS990105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MONM990101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MONM990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MONM990201.txt` & `pypef-0.2.4/pypef/ml/AAindex/MONM990201.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MUNV940101.txt` & `pypef-0.2.4/pypef/ml/AAindex/MUNV940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MUNV940102.txt` & `pypef-0.2.4/pypef/ml/AAindex/MUNV940102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MUNV940103.txt` & `pypef-0.2.4/pypef/ml/AAindex/MUNV940103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MUNV940104.txt` & `pypef-0.2.4/pypef/ml/AAindex/MUNV940104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/MUNV940105.txt` & `pypef-0.2.4/pypef/ml/AAindex/MUNV940105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NADH010101.txt` & `pypef-0.2.4/pypef/ml/AAindex/NADH010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NADH010102.txt` & `pypef-0.2.4/pypef/ml/AAindex/NADH010102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NADH010103.txt` & `pypef-0.2.4/pypef/ml/AAindex/NADH010103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NADH010104.txt` & `pypef-0.2.4/pypef/ml/AAindex/NADH010104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NADH010105.txt` & `pypef-0.2.4/pypef/ml/AAindex/NADH010105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NADH010106.txt` & `pypef-0.2.4/pypef/ml/AAindex/NADH010106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NADH010107.txt` & `pypef-0.2.4/pypef/ml/AAindex/NADH010107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAGK730101.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAGK730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAGK730102.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAGK730102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAGK730103.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAGK730103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900101.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900102.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900103.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900104.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900105.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900106.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900107.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900108.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900109.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900110.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900111.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900112.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH900113.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH900113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH920101.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH920101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH920102.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH920102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH920103.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH920103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH920104.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH920104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH920105.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH920105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH920106.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH920106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH920107.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH920107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NAKH920108.txt` & `pypef-0.2.4/pypef/ml/AAindex/NAKH920108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NISK800101.txt` & `pypef-0.2.4/pypef/ml/AAindex/NISK800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NISK860101.txt` & `pypef-0.2.4/pypef/ml/AAindex/NISK860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/NOZY710101.txt` & `pypef-0.2.4/pypef/ml/AAindex/NOZY710101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OLSK800101.txt` & `pypef-0.2.4/pypef/ml/AAindex/OLSK800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ONEK900101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ONEK900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ONEK900102.txt` & `pypef-0.2.4/pypef/ml/AAindex/ONEK900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM770101.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM770102.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM770103.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM770104.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM770104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM770105.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM770105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM850101.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM850102.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM850103.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM850103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM850104.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM850104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/OOBM850105.txt` & `pypef-0.2.4/pypef/ml/AAindex/OOBM850105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810102.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810103.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810104.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810105.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810106.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810107.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810108.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810109.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810110.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810111.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810112.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810113.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810114.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810115.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PALJ810116.txt` & `pypef-0.2.4/pypef/ml/AAindex/PALJ810116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PARJ860101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PARJ860101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PARS000101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PARS000101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PARS000102.txt` & `pypef-0.2.4/pypef/ml/AAindex/PARS000102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PLIV810101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PLIV810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONJ960101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONJ960101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP800101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP800101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP800102.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP800102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP800103.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP800103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP800104.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP800104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP800105.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP800105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP800106.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP800106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP800107.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP800107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP800108.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP800108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PONP930101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PONP930101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PRAM820101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PRAM820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PRAM820102.txt` & `pypef-0.2.4/pypef/ml/AAindex/PRAM820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PRAM820103.txt` & `pypef-0.2.4/pypef/ml/AAindex/PRAM820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PRAM900101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PRAM900101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PRAM900102.txt` & `pypef-0.2.4/pypef/ml/AAindex/PRAM900102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PRAM900103.txt` & `pypef-0.2.4/pypef/ml/AAindex/PRAM900103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PRAM900104.txt` & `pypef-0.2.4/pypef/ml/AAindex/PRAM900104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PTIO830101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PTIO830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PTIO830102.txt` & `pypef-0.2.4/pypef/ml/AAindex/PTIO830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PUNT030101.txt` & `pypef-0.2.4/pypef/ml/AAindex/PUNT030101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/PUNT030102.txt` & `pypef-0.2.4/pypef/ml/AAindex/PUNT030102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880101.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880102.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880103.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880104.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880105.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880106.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880107.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880108.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880109.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880110.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880111.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880112.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880113.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880114.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880115.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880116.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880116.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880117.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880117.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880118.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880118.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880119.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880119.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880120.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880120.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880121.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880121.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880122.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880122.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880123.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880123.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880124.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880124.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880125.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880125.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880126.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880126.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880127.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880127.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880128.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880128.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880129.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880129.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880130.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880130.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880131.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880131.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880132.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880132.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880133.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880133.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880134.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880134.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880135.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880135.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880136.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880136.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880137.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880137.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880138.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880138.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/QIAN880139.txt` & `pypef-0.2.4/pypef/ml/AAindex/QIAN880139.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS770101.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS770102.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS770103.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820101.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820102.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820103.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820104.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820105.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820106.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820107.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820108.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820109.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820110.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820111.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820112.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820113.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RACS820114.txt` & `pypef-0.2.4/pypef/ml/AAindex/RACS820114.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RADA880101.txt` & `pypef-0.2.4/pypef/ml/AAindex/RADA880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RADA880102.txt` & `pypef-0.2.4/pypef/ml/AAindex/RADA880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RADA880103.txt` & `pypef-0.2.4/pypef/ml/AAindex/RADA880103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RADA880104.txt` & `pypef-0.2.4/pypef/ml/AAindex/RADA880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RADA880105.txt` & `pypef-0.2.4/pypef/ml/AAindex/RADA880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RADA880106.txt` & `pypef-0.2.4/pypef/ml/AAindex/RADA880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RADA880107.txt` & `pypef-0.2.4/pypef/ml/AAindex/RADA880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RADA880108.txt` & `pypef-0.2.4/pypef/ml/AAindex/RADA880108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RICJ880101.txt` & `pypef-0.2.4/pypef/ml/AAindex/RICJ880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RICJ880102.txt` & `pypef-0.2.4/pypef/ml/AAindex/RICJ880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RICJ880106.txt` & `pypef-0.2.4/pypef/ml/AAindex/RICJ880106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RICJ880107.txt` & `pypef-0.2.4/pypef/ml/AAindex/RICJ880107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RICJ880109.txt` & `pypef-0.2.4/pypef/ml/AAindex/RICJ880109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RICJ880111.txt` & `pypef-0.2.4/pypef/ml/AAindex/RICJ880111.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/RICJ880115.txt` & `pypef-0.2.4/pypef/ml/AAindex/RICJ880115.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760103.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760104.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760105.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760106.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760108.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760110.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760112.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760112.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB760113.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB760113.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROBB790101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROBB790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROSG850101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROSG850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROSG850102.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROSG850102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROSM880101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROSM880101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROSM880102.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROSM880102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROSM880104.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROSM880104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ROSM880105.txt` & `pypef-0.2.4/pypef/ml/AAindex/ROSM880105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/SIMZ760101.txt` & `pypef-0.2.4/pypef/ml/AAindex/SIMZ760101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/SNEP660103.txt` & `pypef-0.2.4/pypef/ml/AAindex/SNEP660103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/SUEM840101.txt` & `pypef-0.2.4/pypef/ml/AAindex/SUEM840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/SUEM840102.txt` & `pypef-0.2.4/pypef/ml/AAindex/SUEM840102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/SWER830101.txt` & `pypef-0.2.4/pypef/ml/AAindex/SWER830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TAKK010101.txt` & `pypef-0.2.4/pypef/ml/AAindex/TAKK010101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770101.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770102.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770103.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770104.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770105.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770106.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770106.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770107.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770107.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770108.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770108.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770109.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770109.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TANS770110.txt` & `pypef-0.2.4/pypef/ml/AAindex/TANS770110.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TSAJ990101.txt` & `pypef-0.2.4/pypef/ml/AAindex/TSAJ990101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/TSAJ990102.txt` & `pypef-0.2.4/pypef/ml/AAindex/TSAJ990102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VASM830101.txt` & `pypef-0.2.4/pypef/ml/AAindex/VASM830101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VASM830102.txt` & `pypef-0.2.4/pypef/ml/AAindex/VASM830102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VASM830103.txt` & `pypef-0.2.4/pypef/ml/AAindex/VASM830103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VELV850101.txt` & `pypef-0.2.4/pypef/ml/AAindex/VELV850101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VENT840101.txt` & `pypef-0.2.4/pypef/ml/AAindex/VENT840101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VHEG790101.txt` & `pypef-0.2.4/pypef/ml/AAindex/VHEG790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VINM940101.txt` & `pypef-0.2.4/pypef/ml/AAindex/VINM940101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VINM940102.txt` & `pypef-0.2.4/pypef/ml/AAindex/VINM940102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VINM940103.txt` & `pypef-0.2.4/pypef/ml/AAindex/VINM940103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/VINM940104.txt` & `pypef-0.2.4/pypef/ml/AAindex/VINM940104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WARP780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WARP780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WEBA780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WEBA780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WERD780101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WERD780101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WERD780102.txt` & `pypef-0.2.4/pypef/ml/AAindex/WERD780102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WERD780103.txt` & `pypef-0.2.4/pypef/ml/AAindex/WERD780103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WERD780104.txt` & `pypef-0.2.4/pypef/ml/AAindex/WERD780104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WILM950101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WILM950101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WILM950102.txt` & `pypef-0.2.4/pypef/ml/AAindex/WILM950102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WILM950103.txt` & `pypef-0.2.4/pypef/ml/AAindex/WILM950103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WILM950104.txt` & `pypef-0.2.4/pypef/ml/AAindex/WILM950104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WIMW960101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WIMW960101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WOEC730101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WOEC730101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WOLR790101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WOLR790101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WOLR810101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WOLR810101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WOLS870101.txt` & `pypef-0.2.4/pypef/ml/AAindex/WOLS870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WOLS870102.txt` & `pypef-0.2.4/pypef/ml/AAindex/WOLS870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/WOLS870103.txt` & `pypef-0.2.4/pypef/ml/AAindex/WOLS870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/YANJ020101.txt` & `pypef-0.2.4/pypef/ml/AAindex/YANJ020101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/YUTK870101.txt` & `pypef-0.2.4/pypef/ml/AAindex/YUTK870101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/YUTK870102.txt` & `pypef-0.2.4/pypef/ml/AAindex/YUTK870102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/YUTK870103.txt` & `pypef-0.2.4/pypef/ml/AAindex/YUTK870103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/YUTK870104.txt` & `pypef-0.2.4/pypef/ml/AAindex/YUTK870104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZASB820101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZASB820101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZHOH040101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZHOH040101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZHOH040102.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZHOH040102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZHOH040103.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZHOH040103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZIMJ680101.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680101.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZIMJ680102.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680102.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZIMJ680103.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680103.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZIMJ680104.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680104.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/AAindex/ZIMJ680105.txt` & `pypef-0.2.4/pypef/ml/AAindex/ZIMJ680105.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/parallelization.py` & `pypef-0.2.4/pypef/ml/parallelization.py`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/pypef/ml/regression.py` & `pypef-0.2.4/pypef/ml/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 """
 Main modules for regression/ML including feature generation
 (i.e. sequence encoding), cross-validation-based hyperparameter
 tuning, prediction, and plotting routines.
 """
 
 
-import copy
 import os
-from typing import Union, Tuple, Dict, Any
+from typing import Union
 
+import logging
+logger = logging.getLogger('pypef.ml.regression')
 import matplotlib
 matplotlib.use('Agg')  # no plt.show(), just save plot
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy import stats
 import pickle
 from tqdm import tqdm  # progress bars
@@ -324,20 +325,19 @@
             encoded_sequence.append(self.encoding_dict()[aminoacid])
         return np.concatenate(encoded_sequence)
 
     def collect_encoded_sequences(self, silence=False) -> list:
         encoded_sequences = []
         for sequence in tqdm(self.sequences, disable=silence):
             encoded_sequences.append(self.one_hot_encode_sequence(sequence))
-        return encoded_sequences
-
+        return np.array(encoded_sequences)
 
 def pls_loocv(
-        x_train: list,
-        y_train: list
+        x_train: np.ndarray,
+        y_train: np.ndarray
 ) -> Union[tuple[str, str], tuple[PLSRegression, dict]]:
     """
     PLS regression with LOOCV n_components tuning as described by Cadet et al.
     https://doi.org/10.1186/s12859-018-2407-8
     https://doi.org/10.1038/s41598-018-35033-y
     Hyperparameter (N component) tuning of PLS regressor, can achieve slightly better
     """
@@ -354,14 +354,17 @@
                 x_test_loo = []
                 for j in train:
                     x_learn_loo.append(x_train[j])
                     y_learn_loo.append(y_train[j])
                 for k in test:
                     x_test_loo.append(x_train[k])
                     y_test_loo.append(y_train[k])
+                x_learn_loo = np.array(x_learn_loo)
+                x_test_loo = np.array(x_test_loo)
+                y_learn_loo = np.array(y_learn_loo)
                 try:
                     pls.fit(x_learn_loo, y_learn_loo)
                 except ValueError:  # scipy/linalg/decomp_svd.py ValueError:
                     continue        # illegal value in %dth argument of internal gesdd
                 y_pred_loo.append(pls.predict(x_test_loo)[0][0])
         except np.linalg.LinAlgError:  # numpy.linalg.LinAlgError: SVD did not converge
             continue
@@ -496,15 +499,15 @@
             return [None, None, None, None, None, regressor, None]
 
     # other regression options (k-fold CV tuning)
     else:
         regressor_ = cv_regression_options(regressor)
     try:
         if verbose:
-            print('CV-based training of regression model...')
+            logger.info('CV-based training of regression model...')
         regressor_.fit(x_learn, y_learn)  # fit model
     except ValueError:  # scipy/linalg/decomp_svd.py --> ValueError('illegal value in %dth argument of internal gesdd'
         return [None, None, None, None, None, regressor, None]
 
     if regressor != 'pls_loocv':  # take best parameters for the regressor and the AAindex
         best_params = regressor_.best_params_
 
@@ -517,27 +520,28 @@
 
     r2, rmse, nrmse, pearson_r, spearman_rho = get_performances(y_test, y_pred)
 
     return r2, rmse, nrmse, pearson_r, spearman_rho, regressor, best_params
 
 
 def performance_list(
-        train_set,
-        test_set,
-        encoding='aaidx',
-        regressor='pls',
-        no_fft=False,
-        sort='1',
-        couplings_file=None,
+        train_set: str,
+        test_set: str,
+        encoding: str = 'aaidx',
+        regressor: str = 'pls',
+        no_fft: bool = False,
+        sort: str = '1',
+        couplings_file: str = None,
         threads: int = 1  # for parallelization of DCA-based encoding
 ):
     """
     returns the sorted list of all the model parameters and the
     performance values (R2 etc.) from function get_performances.
     """
+    encoding = encoding.lower()
     performance_list = []
     train_sequences, train_variants, y_train = get_sequences_from_file(train_set)
     test_sequences, test_variants, y_test = get_sequences_from_file(test_set)
     if encoding == 'onehot':  # OneHot-based encoding
         x_onehot_train = OneHotEncoding(train_sequences)
         x_onehot_test = OneHotEncoding(test_sequences)
         x_train = x_onehot_train.collect_encoded_sequences()
@@ -548,30 +552,30 @@
             performance_list.append([
                 'ONEHOTMODEL', r2, rmse, nrmse, pearson_r,
                 spearman_rho, regression_model, params
             ])
     elif encoding == 'dca':
         if threads > 1:  # NaNs are already being removed by the called function
             dca_encoder = DCAEncoding(couplings_file, verbose=False)
-            print('Parallel encoding (runs DCA encoding silent, '
-                  'no information about non-encoded variant positions)...')
+            logger.info('Parallel encoding (runs DCA encoding silent, '
+                        'no information about non-encoded variant positions)...')
             train_variants, x_train, y_train = get_dca_data_parallel(train_variants, y_train, dca_encoder, threads)
             test_variants, x_test, y_test = get_dca_data_parallel(test_variants, y_test, dca_encoder, threads)
         else:
             dca_encoder = DCAEncoding(couplings_file)
-            x_train = dca_encoder.collect_encoded_sequences(train_variants)
-            x_test = dca_encoder.collect_encoded_sequences(test_variants)
+            x_train_ = dca_encoder.collect_encoded_sequences(train_variants)
+            x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
             # NaNs must still be removed
-            x_train, y_train = remove_nan_encoded_positions(x_train, y_train)
-            x_test, y_test = remove_nan_encoded_positions(x_test, y_test)
+            x_train, y_train = remove_nan_encoded_positions(x_train_, y_train)
+            x_test, y_test = remove_nan_encoded_positions(x_test_, y_test)
         r2, rmse, nrmse, pearson_r, spearman_rho, regression_model, \
             params = get_regressor_performances(x_train, x_test, y_train, y_test, regressor, verbose=True)
         if r2 is not None:  # get_regressor_performances() returns None for metrics if MSE can't be calculated
             performance_list.append([
-                'DCAMODEL', r2, rmse, nrmse, pearson_r,
+                'DCAMLMODEL', r2, rmse, nrmse, pearson_r,
                 spearman_rho, regression_model, params
             ])
 
     else:  # AAindex-based encoding
         aa_indices = [file for file in os.listdir(path_aaindex_dir()) if file.endswith('.txt')]
         # loop over the 566 AAindex entries, encode with each AAindex and test performance
         # can be seen as a AAindex hyperparameter search on the test set  --> also see CV performance
@@ -718,14 +722,16 @@
     -----------
     r_squared: float
     rmse: float
     nrmse: float
     pearson_r: float
     spearman_rho: float
     """
+    y_true = list(y_true)
+    y_pred = list(y_pred)
     r_squared = r2_score(y_true, y_pred)
     rmse = np.sqrt(mean_squared_error(y_true, y_pred))
     stddev = np.std(y_true, ddof=1)
     nrmse = rmse / stddev
     with warnings.catch_warnings():  # catching RunTime warning when there's no variance in an array,
         warnings.simplefilter("ignore")  # e.g. [2, 2, 2, 2] which would mean divide by zero
         pearson_r = np.corrcoef(y_true, y_pred)[0][1]
@@ -810,19 +816,19 @@
         threads: int = 1
 ):
     """
     Function Save_Model saves the best -s THRESHOLD models as 'Pickle'
     files (pickle.dump), which can be loaded again for doing predictions.
     Also, in Save_Model included is the def cross_validation-based computing
     of the k-fold CV performance of the n component-optimized model on all
-    data (learning + validation set); by default  k  is 5 (n_samples = 5).
+    data (learning + test set); by default  k  is 5 (n_samples = 5).
     Plots of the CV performance for the t best models are stored inside the
     folder CV_performance.
     """
-    print('Encoding and cross validation on all data (creating folder CV_performance)...')
+    logger.info('Encoding and cross validation on all data (creating folder CV_performance)...')
     regressor = regressor.lower()
     try:
         os.mkdir('CV_performance')
     except FileExistsError:
         pass
     try:
         os.mkdir('Pickles')
@@ -871,18 +877,18 @@
                 dca_encoder = DCAEncoding(couplings_file, verbose=False)
                 if threads > 1:  # parallelization of encoding, NaNs are already being removed by the called function
                     train_variants, x_train, y_train = get_dca_data_parallel(train_variants, y_train, dca_encoder, threads)
                     test_variants, x_test, y_test = get_dca_data_parallel(test_variants, y_test, dca_encoder, threads)
                 else:  # encode using a single thread
                     x_train_ = dca_encoder.collect_encoded_sequences(train_variants)
                     x_test_ = dca_encoder.collect_encoded_sequences(test_variants)
-                    x_train, y_train = remove_nan_encoded_positions(copy.copy(x_train_), y_train)
-                    x_train, train_variants = remove_nan_encoded_positions(copy.copy(x_train_), train_variants)
-                    x_test, y_test = remove_nan_encoded_positions(copy.copy(x_test_), y_test)
-                    x_test, test_variants = remove_nan_encoded_positions(copy.copy(x_test_), test_variants)
+
+                    x_train, y_train, train_variants = remove_nan_encoded_positions(x_train_, y_train, train_variants)
+                    x_test, y_test, test_variants = remove_nan_encoded_positions(x_test_, y_test, test_variants)
+
                     assert len(x_train) == len(y_train) == len(train_variants)
                     assert len(x_test) == len(y_test) == len(test_variants)
 
             x = np.concatenate([x_train, x_test])
             y = np.concatenate([y_train, y_test])
 
             regressor_ = get_regressor(regressor, parameter)
@@ -990,50 +996,58 @@
             silence = True
         else:
             silence = False
         x = x_onehot.collect_encoded_sequences(silence=silence)
         x_raw = None
     else:  # DCA
         if dca_encoder is not None:  # use dca_encoder from directed evolution, single thread
-            x = dca_encoder.collect_encoded_sequences(variants)
-            x, variants = remove_nan_encoded_positions(x, list(variants))
+            x_ = dca_encoder.collect_encoded_sequences(variants)
+            x, variants = remove_nan_encoded_positions(x_, variants)
             x_raw = None
 
         else:
             if threads > 1:
                 dca_encoder = DCAEncoding(couplings_file, verbose=False)
-                print('Parallel encoding (runs DCA encoding silent, '
-                      'no information about non-encoded variant positions)...')
+                logger.info('Parallel encoding (runs DCA encoding silent, '
+                            'no information about non-encoded variant positions)...')
                 # parallel encoding of variants, NaNs are already being removed by the called function
                 variants, x, _ = get_dca_data_parallel(
                     variants, list(np.zeros(len(variants))), dca_encoder, threads
                 )
             else:  # single thread running
                 dca_encoder = DCAEncoding(couplings_file)
-                x = dca_encoder.collect_encoded_sequences(variants)
-                x, variants = remove_nan_encoded_positions(x, list(variants))
+                x_ = dca_encoder.collect_encoded_sequences(variants)
+                x, variants = remove_nan_encoded_positions(x_, variants)
                 x_raw = None
-
-        if not x:
-            return 'skip'
+        if type(x) == list:
+            if not x:
+                return 'skip'
+        elif type(x) == np.ndarray:
+            if not x.any():
+                return 'skip'
 
     assert len(variants) == len(x)
 
     try:
         if no_fft and encoding == 'aaidx':  # predict using raw AAidx encoding (without FFT)
             ys = loaded_model.predict(x_raw)
         else:  # predict AAidx-FFTed or onehot or DCA-based encoding
             ys = loaded_model.predict(x)
     except ValueError:
-        raise ValueError(
+        raise SystemError(
             "If you used an encoding such as onehot, make sure to use the correct model, e.g. -m ONEHOT. "
             "If you used an AAindex-encoded model you likely tried to predict using a model encoded with "
             "(or without) FFT featurization ('--nofft') while the model was trained without (or with) FFT "
             "featurization so check Model_Results.txt line 1, if the models were trained with or without FFT."
         )
+    except AttributeError:
+        raise SystemError(
+            "The model specified is likely a hybrid or pure statistical DCA (and no pure ML model).\n"
+            "Check the specified model provided via the \'-m\' flag."
+        )
 
     predictions = [(float(ys[i]), variants[i]) for i in range(len(ys))]  # List of tuples
 
     # Pay attention if increased negative values would define a better variant --> use negative flag
     predictions.sort()
     predictions.reverse()
     # if predictions array too large? if Mult_Path is not None: predictions = predictions[:100000]
@@ -1100,67 +1114,65 @@
             threads = 1
         dca_encoder = DCAEncoding(couplings_file)
         x_raw = None
         if threads > 1:  # NaNs are already being removed by the called function, for ys just filling 0's
             variants_test, x, y_test = get_dca_data_parallel(variants_test, y_test, dca_encoder, threads)
         else:
             x_ = dca_encoder.collect_encoded_sequences(variants_test)
-            x, variants_test = remove_nan_encoded_positions(copy.copy(x_), variants_test)
-            x, y_test = remove_nan_encoded_positions(copy.copy(x_), y_test)
-            assert len(x) == len(variants_test) == len(y_test)
+            x, variants_test, y_test = remove_nan_encoded_positions(x_, variants_test, y_test)
+        assert len(x) == len(variants_test) == len(y_test)
 
     try:
         file = open(os.path.join(path, 'Pickles', str(model)), 'rb')
-        mod = pickle.load(file)
+        model_ = pickle.load(file)
         file.close()
     except FileNotFoundError:
         raise FileNotFoundError(
             f"Did not find specified model: {str(model)}. You can define the "
             f"threshold of models to be saved; e.g. with pypef run -l LS.fasta "
             f"-v VS.fasta -s 10 and pay attention to capitalization of model "
             f"names (e.g. -m PONP930101 or -m ONEHOT."
         )
     y_pred = []
     try:
         # predicting (again) with (re-)loaded model (that was trained on training or full data)
         if no_fft and encoding == 'aaidx':  # predict using raw AAidx encoding
-            y_pred_ = mod.predict(x_raw)
+            y_pred_ = model_.predict(x_raw)
         else:  # predict AAidx-FFTed or onehot or DCA-based encoding
-            y_pred_ = mod.predict(x)
+            y_pred_ = model_.predict(x)
     except ValueError:
         raise ValueError(
             "You likely tried to plot a test set with (or without) "
             "FFT featurization ('--nofft') while the model was trained "
             "without (or with) FFT featurization. Check the Model_Results.txt "
             "line 1, if the models were trained using FFT."
         )
     for y_p in y_pred_:
         y_pred.append(float(y_p))
-
     r_squared, rmse, nrmse, pearson_r, spearman_rho = \
         get_performances(y_test, y_pred)
     legend = '$R^2$ = {}\nRMSE = {}\nNRMSE = {}\nPearson\'s $r$ = {}\nSpearman\'s '.format(
         round(r_squared, 3), round(rmse, 3), round(nrmse, 3), round(pearson_r, 3)) + \
              r'$\rho$ = {}'.format(round(spearman_rho, 3)) + \
              '\n' + r'($N$ = {})'.format(len(y_test))
     x = np.linspace(min(y_pred), max(y_pred), 100)
     fig, ax = plt.subplots()
     ax.scatter(y_test, y_pred,
                label=legend, marker='o', s=20, linewidths=0.5, edgecolor='black', alpha=0.8)
     ax.legend(prop={'size': 8})
     ax.plot(x, x, color='black', linewidth=0.5)  # plot diagonal line
     if label is not False:
-        print('Adjusting variant labels for plotting can take some '
-              'time (the limit for labeling is 150 data points)...')
+        logger.info('Adjusting variant labels for plotting can take some '
+                    'time (the limit for labeling is 150 data points)...')
         if len(y_test) < 150:
             texts = [ax.text(y_test[i], y_pred[i], txt, fontsize=4) for i, txt in enumerate(variants_test)]
             adjust_text(texts, only_move={'points': 'y', 'text': 'y'}, force_points=0.5, lim=250)
         else:
-            print("Terminating label process. Too many variants "
-                  "(> 150) for plotting (labels would overlap).")
+            logger.info("Terminating label process. Too many variants "
+                        "(> 150) for plotting (labels would overlap).")
     if color is not False:
         try:
             y_wt = float(y_wt)
         except TypeError:
             raise TypeError('Needs label value of WT (y_WT) when making color plot (e.g. --color --ywt 1.0)')
         if y_wt == 0:
             y_wt = 1E-9  # choose a value close to zero
@@ -1226,43 +1238,43 @@
     Plots predicted versus true values using the hybrid model for prediction.
     Function called by function predict_ps.
     """
     figure, ax = plt.subplots()
     if hybrid:
         spearman_rho = stats.spearmanr(y_true, y_pred)[0]
         ax.scatter(y_true, y_pred, marker='o', s=20, linewidths=0.5, edgecolor='black', alpha=0.7,
-                   label=f'Spearman\'s ' + fr'$\rho$ = {spearman_rho:.3f}')
+                   label=f'Spearman\'s ' + fr'$\rho$ = {spearman_rho:.3f}' + '\n' + fr'($N$ = {len(y_true)})')
         file_name = name + 'DCA_Hybrid_Model_LS_TS_Performance.png'
     else:
         r_squared, rmse, nrmse, pearson_r, spearman_rho = get_performances(
-            y_true=list(y_true), y_pred=list(y_pred)
+            y_true=y_true, y_pred=y_pred
         )
         ax.scatter(
             y_true, y_pred, marker='o', s=20, linewidths=0.5, edgecolor='black', alpha=0.7,
             label=r'$R^2$' + f' = {r_squared:.3f}' + f'\nRMSE = {rmse:.3f}' + f'\nNRMSE = {nrmse:.3f}' +
                   f'\nPearson\'s ' + r'$r$'+f' = {pearson_r:.3f}' + f'\nSpearman\'s ' +
                   fr'$\rho$ = {spearman_rho:.3f}' + '\n' + fr'($N$ = {len(y_true)})'
         )
         file_name = name + 'ML_Model_LS_TS_Performance.png'
-    x = np.linspace(min(y_pred), max(y_pred), 100)
-    ax.plot(x, x, color='black', linewidth=0.25)  # plot diagonal line
+        x = np.linspace(min(y_pred), max(y_pred), 100)
+        ax.plot(x, x, color='black', linewidth=0.25)  # plot diagonal line
     ax.legend(prop={'size': 8})
     ax.set_xlabel('Measured')
     ax.set_ylabel('Predicted')
-    print('\nPlotting...')
+    logger.info('Plotting...')
     if label:
-        print('Adjusting variant labels for plotting can take some '
-              'time (the limit for labeling is 150 data points)...')
+        logger.info('Adjusting variant labels for plotting can take some '
+                    'time (the limit for labeling is 150 data points)...')
         if len(y_true) < 150:
             texts = [ax.text(y_true[i], y_pred[i], txt, fontsize=4)
                      for i, txt in enumerate(variants)]
             adjust_text(
                 texts, only_move={'points': 'y', 'text': 'y'}, force_points=0.5, lim=250)
         else:
-            print("Terminating label process. Too many variants "
-                  "(> 150) for plotting (labels would overlap).")
-
+            logger.info("Terminating label process. Too many variants "
+                        "(> 150) for plotting (labels would overlap).")
+    # Uncomment for renaming new plots
     # i = 1
     # while os.path.isfile(file_name):
     #     i += 1  # iterate until finding an unused file name
     #     file_name = f'DCA_Hybrid_Model_LS_TS_Performance({i}).png'
     plt.savefig(file_name, dpi=500)
```

### Comparing `pypef-0.2.3/pypef/ml/run.py` & `pypef-0.2.4/pypef/ml/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 # §Equal contribution
 
 
 import os
 from os import listdir
 from os.path import isfile, join
 
-# ray imported later locally as only used for parallelized running, thus commented out:
+import logging
+logger = logging.getLogger('pypef.ml.run')
 import ray
 from pypef.ml.parallelization import aaindex_performance_parallel
 
 # importing own modules
 from pypef.ml.regression import (
     read_models, formatted_output, performance_list, save_model, predict,
     predictions_out, predict_and_plot
@@ -61,15 +62,15 @@
                 path = os.getcwd()
                 try:
                     t_save = int(arguments['--save'])
                 except ValueError:
                     t_save = 5
                 # Parallelization of AAindex iteration if threads is not None (but int)
                 if threads > 1 and arguments['--encoding'] == 'aaidx':
-                    print(f'Using {threads} threads for parallel computing. Running...')
+                    logger.info(f'Using {threads} threads for parallel computing. Running...')
                     encoding_performance_list = aaindex_performance_parallel(
                         train_set=arguments['--ls'],
                         test_set=arguments['--ts'],
                         cores=threads,
                         regressor=arguments['--regressor'],
                         no_fft=arguments['--nofft'],
                         sort=arguments['--sort']
@@ -89,14 +90,15 @@
 
                 formatted_output(
                     performance_list=encoding_performance_list,
                     no_fft=arguments['--nofft'],
                     minimum_r2=0.0
                 )
 
+                # save_model encodes variants again (possibly change)
                 save_model(
                     path=path,
                     performance_list=encoding_performance_list,
                     training_set=arguments['--ls'],
                     test_set=arguments['--ts'],
                     threshold=t_save,
                     encoding=arguments['--encoding'],
@@ -117,15 +119,15 @@
                 label=arguments['--label'],
                 color=arguments['--color'],
                 y_wt=arguments['--y_wt'],
                 no_fft=arguments['--nofft'],
                 couplings_file=arguments['--params'],  # only for DCA
                 threads=threads  # only for DCA
             )
-            print('\nCreated plot!\n')
+            logger.info('\nCreated plot!\n')
 
         # Prediction of single .fasta file
         elif arguments['--ps'] is not None and arguments['--model'] is not None:
             path = os.getcwd()
             predictions = predict(
                 path=path,
                 prediction_set=arguments['--ps'],
@@ -170,24 +172,24 @@
             if arguments['--drecomb'] is False \
                     and arguments['--trecomb'] is False \
                     and arguments['--qarecomb'] is False \
                     and arguments['--qirecomb'] is False \
                     and arguments['--ddiverse'] is False \
                     and arguments['--tdiverse'] is False \
                     and arguments['--qdiverse'] is False:
-                print('Define prediction target for --pmult, e.g. --pmult --drecomb.')
+                raise SystemError('Define prediction target for --pmult, e.g. --pmult --drecomb.')
 
             for args in recombs_total:
                 predictions_total = []
-                print(f'Running predictions for variant-sequence files in directory {args[1:-1]}...')
+                logger.info(f'Running predictions for variant-sequence files in directory {args[1:-1]}...')
                 path_recomb = path + args
                 os.chdir(path)
                 files = [f for f in listdir(path_recomb) if isfile(join(path_recomb, f)) if f.endswith('.fasta')]
                 for i, file in enumerate(files):
-                    print(f'Encoding files ({i+1}/{len(files)}) for prediction...\n')
+                    logger.info(f'Encoding files ({i+1}/{len(files)}) for prediction...\n')
                     predictions = predict(
                         path=path,
                         prediction_set=file,
                         model=arguments['--model'],
                         encoding=arguments['--encoding'],
                         mult_path=path_recomb,
                         no_fft=arguments['--nofft'],
@@ -217,9 +219,7 @@
             )
 
         elif arguments['low_n']:
             low_n(
                 encoded_csv=arguments['--input'],
                 cv_regressor=arguments['--regressor']
             )
-
-        print('\nDone!\n')
```

### Comparing `pypef-0.2.3/pypef/utils/directed_evolution.py` & `pypef-0.2.4/pypef/utils/directed_evolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 Modules for performing random evolution walks
 similar as presented by Biswas et al.
 """
 
 import os
 import re
 import random
+
 import matplotlib.pyplot as plt
 import numpy as np
 import warnings
 from adjustText import adjust_text
 
 from pypef.ml.regression import predict
 from pypef.dca.hybrid_model import predict_directed_evolution
@@ -316,15 +317,15 @@
             y_records_.append(fitness_array)
         label_x_y_name = []
         traj_max_len = 0
         for i, v_record in enumerate(v_records):  # i = 1, 2, 3, .., ; v_record = variant label array
             for j, v in enumerate(v_record):      # j = 1, 2, 3, ..., ; v = variant name; y_records[i][j] = fitness
                 if len(v_record) > traj_max_len:
                     traj_max_len = len(v_record)
-                if i == 0:                      # j + 1 -> x axis position shifted by 1
+                if i == 0:                      # j + 1 -> x-axis position shifted by 1
                     label_x_y_name.append(ax.text(j + 1, y_records_[i][j], v, size=9))
                 else:
                     if v != 'WT':  # only plot 'WT' name once at i == 0
                         label_x_y_name.append(ax.text(j + 1, y_records_[i][j], v, size=9))
         adjust_text(label_x_y_name, only_move={'points': 'y', 'text': 'y'}, force_points=0.5)
         ax.legend()
         plt.xticks(np.arange(1,  traj_max_len + 1, 1), np.arange(1, traj_max_len + 1, 1))
```

### Comparing `pypef-0.2.3/pypef/utils/learning_test_sets.py` & `pypef-0.2.4/pypef/utils/learning_test_sets.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 VARIANT_SEQUENCE_1
 > VARIANT_NAME_2
 ; FITNESS_2
 VARIANT_SEQUENCE_2
 ...
 """
 
+import logging
+logger = logging.getLogger('pypef.utils.learning_test_sets')
+
 import numpy as np
 import random
 import pandas as pd
 import re
 
 
 def get_wt_sequence(sequence_fasta):
@@ -51,16 +54,16 @@
         with open(sequence_fasta, 'r') as sf:
             for lines in sf.readlines():
                 if lines.startswith(">"):
                     continue
                 lines = ''.join(lines.split())
                 wild_type_sequence += lines
     except FileNotFoundError:
-        raise FileNotFoundError("Specify input FASTA sequence file for "
-                                "getting the wild-type sequence.")
+        raise FileNotFoundError("Did not find FASTA file. Check/specify input FASTA "
+                                "sequence file for getting the wild-type sequence.")
     return wild_type_sequence
 
 
 def csv_input(csv_file):
     """
     Gets input data from defined .csv file (that contains variant names and fitness labels)
     """
@@ -123,16 +126,16 @@
                     if variant[0] not in amino_acids or variant[-1] not in amino_acids:
                         dropping_rows.append(i)
                         # print('Does not know this definition of amino acid substitution: Variant:', variant)
         except TypeError:
             raise TypeError('You might consider checking the input .csv for empty first two columns,'
                             ' e.g. in the last row.')
 
-    print(f'No. of dropped rows: {len(dropping_rows)}. '
-          f'Total given variants (if provided plus WT): {len(df_raw)}')
+    logger.info(f'No. of dropped rows: {len(dropping_rows)}. '
+                f'Total given variants (if provided plus WT): {len(df_raw)}')
 
     df = df_raw.drop(dropping_rows)
     df.dropna(inplace=True)
     df.reset_index(drop=True, inplace=True)
 
     return df
 
@@ -222,18 +225,20 @@
                     full_variant = wild_type_sequence[num - 1] + str(num) + str(variant[-1])
                 except IndexError:
                     raise IndexError("Found variant sequence position {} in data which "
                                      "is out of range of wild-type sequence length.".format(str(num)))
                 single_variants.append([full_variant])
                 if i not in index_lower:
                     index_lower.append(i)
-    print('Single (for mklsts if provided plus WT): {}.'.format(single), 'Double: {}.'.format(double),
-          'Triple: {}.'.format(triple), 'Quadruple: {}.'.format(quadruple), 'Quintuple: {}.'.format(quintuple),
-          'Sextuple: {}.'.format(sextuple), 'Septuple: {}.'.format(septuple), 'Octuple: {}.'.format(octuple),
-          'Nonuple: {}.'.format(nonuple), 'Decuple: {}.'.format(decuple), 'Higher: {}.'.format(higher))
+    logger.info(
+        '\nSingle (for mklsts if provided plus WT): {}\nDouble: {}\nTriple: {}\nQuadruple: {}\nQuintuple: {}\n'
+        'Sextuple: {}\nSeptuple: {}\nOctuple: {}\nNonuple: {}\nDecuple: {}\nHigher (>Decuple): {}'.format(
+            single, double, triple, quadruple, quintuple, sextuple, septuple, octuple, nonuple, decuple, higher
+        )
+    )
     for vals in y[index_higher]:
         higher_values.append(vals)
     for vals in y[index_lower]:
         single_values.append(vals)
     if wt_position is not None:
         single_variants.append(['WT'])
         single_values.append(y[wt_position])
@@ -250,27 +255,28 @@
         higher_variants,
         higher_values,
         directed_evolution=False):
     """
     Creates learning and test sets, fills learning set with single substituted variants and splits
     rest (higher substituted) for learning and test sets: 3/4 to LS and 1/4 to TS
     """
-    print('No. of single substituted variants (if provided plus WT): {}.'.format(len(single_variants)),
-          'No. of values: {}'.format(len(single_values)))
-    print('No. of higher substituted variants: {}.'.format(len(higher_variants)),
-          'No. of values: {}'.format(len(higher_values)))
+    logger.info(f'No. of single substituted variants (if provided plus WT): {len(single_variants)}.'
+                f'No. of values: {len(single_values)}.')
+    logger.info(f'No. of higher substituted variants: {len(higher_variants)}. '
+                f'No. of values: {len(higher_values)}.')
 
     if len(single_values) != len(single_variants):
-        print('Error due to different lengths for given variants and label!'
-              ' No. of single substituted variants: {}.'.format(len(single_variants)),
-              ' Number of given values: {}.'.format(len(single_values)))
+        logger.info(f'Error due to different lengths for given variants and label! '
+                    'No. of single substituted variants: {len(single_variants)}. '
+                    'Number of given values: {len(single_values)}.')
 
     if len(higher_values) != len(higher_variants):
-        print('Error due to different lengths for given variants and label! No. of higher subst. variants: {}.'
-              .format(len(higher_variants)), ' Number of given values: {}.'.format(len(higher_values)))
+        logger.info(f'Error due to different lengths for given variants and label! '
+                    f'No. of higher subst. variants: {len(higher_variants)}. '
+                    f'Number of given values: {len(higher_values)}.')
 
     # 1. CREATION OF LS AND TS SPLIT FOR SINGLE FOR LS AND HIGHER VARIANTS FOR TS
     all_variants = single_variants + higher_variants
     all_values = single_values + higher_values
     sub_ts = []  # Substitutions of TS
     values_ts = []  # Values of TS
     sub_ls = []
@@ -348,17 +354,17 @@
     for j in ts:
         sub_ts.append(combined[j])
         values_ts.append(combined2[j])
 
     for subs in sub_ls:
         for subs2 in sub_ts:
             if subs == subs2:
-                print('\n<Warning> LS and TS overlap for: {} - '
-                      'You might want to consider checking the provided '
-                      'datasets for multiple entries'.format(subs), end=' ')
+                logger.warning(f'\n<Warning> LS and TS overlap for: {subs} - '
+                               f'You might want to consider checking the provided '
+                               f'datasets for multiple entries')
 
     tot_sub_ls.append(sub_ls)
     tot_values_ls.append(values_ls)
     tot_sub_ts.append(sub_ts)
     tot_values_ts.append(values_ts)
 
     return tot_sub_ls[0], tot_values_ls[0], tot_sub_ts[0], tot_values_ts[0]
@@ -367,22 +373,23 @@
 def make_fasta_ls_ts(
         filename,
         wt_seq,
         substitutions,
         fitness_values
 ):
     """
-    Creates learning and test sets (.fasta style files)
+    Creates learning and test sets (.fasta style-like files with fitness values
+    indicated by starting semicolon ';')
 
     filename: str
         String for defining the filename for the learning and test set "fasta-like" files.
     wt: str
         Wild-type sequence as string
     substitutions: list
-        List of substiutuions of a single variant of the format:
+        List of substitutions of a single variant of the format:
             - Single substitution variant, e.g. variant A123C: ['A123C']
             - Higher variants, e.g. variant A123C/D234E/F345G: ['A123C', 'D234E, 'F345G']
             --> Full substitutions list, e.g.: [['A123C'], ['A123C', 'D234E, 'F345G']]
     fitness_values: list
         List of ints/floats of the variant fitness values, e.g. for two variants: [1.4, 0.8]
     """
     myfile = open(filename, 'w')
@@ -402,15 +409,15 @@
                     name += single_var
                 else:
                     name += '/' + single_var
                 separation += 1
         print(f'>{name}', file=myfile)
         print(f';{fitness_values[i]}', file=myfile)
         print(''.join(temp), file=myfile)
-        # print(name+';'+str(val[i])+';'+''.join(temp), file=myfile)  # output: CSV format
+        # print(name+';'+str(val[i])+';'+''.join(temp), file=myfile)  # uncomment output: CSV format
     myfile.close()
 
 
 def get_seqs_from_var_name(
         wt_seq,
         substitutions,
         fitness_values
```

### Comparing `pypef-0.2.3/pypef/utils/low_n_mutation_extrapolation.py` & `pypef-0.2.4/pypef/utils/low_n_mutation_extrapolation.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
 
 import os
 import random
+import logging
+logger = logging.getLogger('pypef.utils.low_n_mutation_extrapolation')
+
 import pandas as pd
 import numpy as np
 from scipy import stats
 import matplotlib.pyplot as plt
 import pickle
 from tqdm import tqdm
 
@@ -53,15 +56,15 @@
         avg_spearmanr: list,
         stddev_spearmanr: list,
         plt_name: str = ''
 ):
     """
     Plot the performance results of the low N engineering task.
     """
-    print('\nPlotting...\n')
+    logger.info('Plotting...')
     plt.plot(train_sizes, avg_spearmanr, 'ko--', linewidth=1, markersize=1.5)
     plt.fill_between(
         np.array(train_sizes),
         np.array(avg_spearmanr) + np.array(stddev_spearmanr),
         np.array(avg_spearmanr) - np.array(stddev_spearmanr),
         alpha=0.5
     )
@@ -90,26 +93,29 @@
     if df.shape[1] == 1:
         df = pd.read_csv(encoded_csv, sep=',', comment='#')
     if df.shape[1] == 1:
         df = pd.read_csv(encoded_csv, sep='\t', comment='#')
     if cv_regressor:
         name = 'ml_' + cv_regressor
         if cv_regressor == 'pls_loocv':
-            raise SystemError('PLS LOOCV is not (yet) implemented '
-                              'for the extrapolation task. Please choose'
-                              'another CV regressor.')
+            raise SystemError(
+                'PLS LOOCV is not (yet) implemented for the extrapolation task. '
+                'Please choose another CV regression option.'
+            )
         regressor = cv_regression_options(cv_regressor)
     elif hybrid_modeling:
         name = 'hybrid_ridge'
     n_variants = df.shape[0]
     train_sizes = get_train_sizes(n_variants).tolist()
     variants, X, y = process_df_encoding(df)
 
     avg_spearmanr, stddev_spearmanr = [], []
     # test_sizes = [n_variants - size for size in train_sizes]
+    if hybrid_modeling:
+        logger.info('Using first CSV row/entry as wild type reference...')
     for size in tqdm(train_sizes):
         spearmanr_nruns = []
         for _ in range(n_runs):
             train_idxs = random.sample(range(n_variants - 1), int(size))
             test_idxs = []
             for n in range(n_variants - 1):
                 if n not in train_idxs:
@@ -123,15 +129,16 @@
                     X_train=X_train,
                     y_train=y_train,
                     X_test=X_test,  # only used for adjusting +/- sign of y_dca, can also be None
                     y_test=y_test,  # only used for adjusting +/- sign of y_dca, can also be None
                     X_wt=x_wt
                 )
                 beta_1, beta_2, reg = hybrid_model.settings(
-                    X_train, y_train, train_size_fit=train_size_train)
+                    X_train, y_train, train_size_fit=train_size_train
+                )
                 spearmanr_nruns.append(
                     hybrid_model.spearmanr(
                         y_test,
                         hybrid_model.hybrid_prediction(
                             X_test, reg, beta_1, beta_2
                         )
                     )
@@ -183,18 +190,18 @@
                 octuple_i.append(i)
             elif row.count('/') == 8:
                 nonuple_i.append(i)
             elif row.count('/') >= 9:
                 higher_nine_i.append(i)
         else:
             single_variants_index.append(i)
-    print(f'No. Singles: {len(single_variants_index)}\nNo. All higher: {len(all_higher_variants_index)}\n'
-          f'2: {len(double_i)}\n3: {len(triple_i)}\n4: {len(quadruple_i)}\n'
-          f'5: {len(quintuple_i)}\n6: {len(sextuple_i)}\n7: {len(septuple_i)}\n'
-          f'8: {len(octuple_i)}\n9: {len(nonuple_i)}\n>=10: {len(higher_nine_i)}')
+    logger.info(f'\nNo. Singles: {len(single_variants_index)}\nNo. All higher: {len(all_higher_variants_index)}\n'
+                f'2: {len(double_i)}\n3: {len(triple_i)}\n4: {len(quadruple_i)}\n'
+                f'5: {len(quintuple_i)}\n6: {len(sextuple_i)}\n7: {len(septuple_i)}\n'
+                f'8: {len(octuple_i)}\n9: {len(nonuple_i)}\n>=10: {len(higher_nine_i)}')
     return (
         df_encoding.iloc[single_variants_index, :],
         df_encoding.iloc[double_i, :],
         df_encoding.iloc[triple_i, :],
         df_encoding.iloc[quadruple_i, :],
         df_encoding.iloc[quintuple_i, :],
         df_encoding.iloc[sextuple_i, :],
@@ -274,18 +281,18 @@
                 X_train, y_train, train_size_fit=train_size)
             pickle.dump(
                 {'hybrid_model': hybrid_model, 'beta_1': beta_1, 'beta_2': beta_2,
                  'spearman_rho': float('nan'), 'regressor': reg},
                 open(os.path.join('Pickles', 'HYBRID_LVL_1'), 'wb')
             )
         elif cv_regressor:
-            print('Fitting regressor on lvl 1 substitution data...')
+            logger.info('Fitting regressor on lvl 1 substitution data...')
             regressor.fit(X_train, y_train)
             if save_model:
-                print(f'Saving model as Pickle file: ML_LVL_1')
+                logger.info(f'Saving model as Pickle file: ML_LVL_1')
                 pickle.dump(regressor, open(os.path.join('Pickles', 'ML_LVL_1'), 'wb'))
         for i, _ in enumerate(tqdm(collected_levels)):
             if i < len(collected_levels) - 1:  # not last i else error, last entry is: lvl 1 --> all higher variants
                 test_idx = collected_levels[i + 1]
                 test_df = df_mut_lvl[test_idx]
                 test_variants, X_test, y_test = process_df_encoding(test_df)
                 if not conc:
@@ -389,15 +396,15 @@
         extrapolation_data: dict,
         name: str = '',
         conc=False
 ):
     """
     Plot extrapolation results.
     """
-    print('\nPlotting...\n')
+    logger.info('Plotting...')
     test_lvls, spearman_rhos, label_infos = [], [], []
     for test_lvl, result_dict in extrapolation_data.items():
         if result_dict['spearman_rho'] is np.nan:
             continue
         test_lvls.append(test_lvl)
         spearman_rhos.append(result_dict['spearman_rho'])
         label_infos.append(
```

### Comparing `pypef-0.2.3/pypef/utils/prediction_sets.py` & `pypef-0.2.4/pypef/utils/prediction_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 def make_fasta_ps(
         filename,
         wt,
         substitution
 ):
     """
-    Creates prediction sets (.fasta style files)
+    Creates prediction sets (.fasta style files, i.e. without fitness values)
     """
     myfile = open(filename, 'w')
     count = 0
     for i, var in enumerate(substitution):
         temporary = list(wt)
         name = ''
         separation = 0
@@ -395,9 +395,22 @@
                                         if len(quadruples) >= 8E04:
                                             quadruples = list(dict.fromkeys(quadruples))  # transfer to dict
                                             yield quadruples                              # and back to list
                                             quadruples = []
     quadruples = list(dict.fromkeys(quadruples))
     yield quadruples
 
+
 if __name__ == '__main__':
-    make_recombinations_quintuple((['A86V'], ['T91S'], ['M108Q'], ['A109E'], ['T111P'], ['A86S'], ['T91E'], ['M108L'], ['A109S'], ['T111G'], ['M108R'], ['T111N'], ['T91V'], ['M108T'], ['A109G'], ['T111F'], ['T91A'], ['A109M'], ['A86D'], ['T91R'], ['A109K'], ['T111D'], ['T91Q'], ['A109V'], ['T111S'], ['A86C'], ['T91L'], ['A109T'], ['M108S'], ['A109F'], ['T111L'], ['A86T'], ['A109Q'], ['M108A'], ['A109P'], ['T111Q'], ['A86N'], ['T91Y'], ['A109L'], ['T111A'], ['T91F'], ['A109Y'], ['A86I'], ['A109D'], ['M108K'], ['M108I'], ['T91N'], ['T111C'], ['T91M'], ['T91C'], ['M108P'], ['T111M'], ['T91H'], ['M108C'], ['M108F'], ['M108G'], ['A109N'], ['M108E'], ['A109W'], ['M108W'], ['A109I'], ['T91P'], ['M108H'], ['T91D'], ['A109R'], ['T91I'], ['M108Y'], ['T91G'], ['T91W'], ['A86R'], ['T91K'], ['T111Y'], ['M108D'], ['A86W'], ['M108V'], ['T111I'], ['M108N'], ['A109C'], ['A109H']))
+    k = list(make_recombinations_quintuple((
+        ['A86V'], ['T91S'], ['M108Q'], ['A109E'], ['T111P'], ['A86S'], ['T91E'], ['M108L'], ['A109S'], ['T111G'],
+        ['M108R'], ['T111N'], ['T91V'], ['M108T'], ['A109G'], ['T111F'], ['T91A'], ['A109M'], ['A86D'], ['T91R'],
+        ['A109K'], ['T111D'], ['T91Q'], ['A109V'], ['T111S'], ['A86C'], ['T91L'], ['A109T'], ['M108S'], ['A109F'],
+        ['T111L'], ['A86T'], ['A109Q'], ['M108A'], ['A109P'], ['T111Q'], ['A86N'], ['T91Y'], ['A109L'], ['T111A'],
+        ['T91F'], ['A109Y'], ['A86I'], ['A109D'], ['M108K'], ['M108I'], ['T91N'], ['T111C'], ['T91M'], ['T91C'],
+        ['M108P'], ['T111M'], ['T91H'], ['M108C'], ['M108F'], ['M108G'], ['A109N'], ['M108E'], ['A109W'], ['M108W'],
+        ['A109I'], ['T91P'], ['M108H'], ['T91D'], ['A109R'], ['T91I'], ['M108Y'], ['T91G'], ['T91W'], ['A86R'],
+        ['T91K'], ['T111Y'], ['M108D'], ['A86W'], ['M108V'], ['T111I'], ['M108N'], ['A109C'], ['A109H']
+    )))
+    for i, k_ in enumerate(k):
+        print(i + 1, np.shape(k_))
+    # (10 * 80,000 (* 5)) + (1 * 2503 (* 5))
```

### Comparing `pypef-0.2.3/pypef/utils/run.py` & `pypef-0.2.4/pypef/utils/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,23 +13,26 @@
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
 import os
+import logging
+logger = logging.getLogger('pypef.utils.run')
+
 import numpy as np
 import re
 import copy
 import ray
 
 from pypef.utils.variant_data import (
     amino_acids, generate_dataframe_and_save_csv,
-    remove_nan_encoded_positions, path_aaidx_txt_path_from_utils,
-    get_basename, read_csv_and_shift_pos_ints
+    remove_nan_encoded_positions, get_basename,
+    read_csv_and_shift_pos_ints
 )
 
 from pypef.utils.learning_test_sets import (
     get_wt_sequence, csv_input, drop_rows, get_variants, make_sub_ls_ts,
     make_sub_ls_ts_randomly, make_fasta_ls_ts, get_seqs_from_var_name
 )
 from pypef.utils.prediction_sets import (
@@ -40,132 +43,131 @@
 )   # not yet implemented: make_combinations_double_all_diverse_and_all_positions
 
 from pypef.utils.directed_evolution import DirectedEvolution
 from pypef.dca.encoding import DCAEncoding
 from pypef.utils.sto2a2m import convert_sto2a2m
 
 from pypef.dca.encoding import get_dca_data_parallel, get_encoded_sequence
-from pypef.ml.regression import OneHotEncoding, AAIndexEncoding
+from pypef.ml.regression import OneHotEncoding, AAIndexEncoding, full_aaidx_txt_path
 
 
 def run_pypef_utils(arguments):
     if arguments['mklsts']:
         wt_sequence = get_wt_sequence(arguments['--wt'])
         t_drop = float(arguments['--drop'])
 
-        print(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
+        logger.info(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
         df = drop_rows(arguments['--input'], amino_acids, t_drop)
         no_rnd = arguments['--numrnd']
 
         single_variants, single_values, higher_variants, higher_values = get_variants(
             df, amino_acids, wt_sequence)
-        print(f'Number of single variants: {len(single_variants)}.')
+        logger.info(f'Number of single variants: {len(single_variants)}.')
         if len(single_variants) == 0:
-            print('Found NO single substitution variants for possible recombination!')
+            logger.info('Found NO single substitution variants for possible recombination!')
         sub_ls, val_ls, sub_ts, val_ts = make_sub_ls_ts(
             single_variants, single_values, higher_variants, higher_values)
-        print('Tip: You can edit your LS and TS datasets just by '
+        logger.info('Tip: You can edit your LS and TS datasets just by '
               'cutting/pasting between the LS and TS fasta datasets.')
 
-        print('Creating LS dataset...', end='\r')
-        make_fasta_ls_ts('LS.fasta', wt_sequence, sub_ls, val_ls)
-        print('Creating TS dataset...', end='\r')
-        make_fasta_ls_ts('TS.fasta', wt_sequence, sub_ts, val_ts)
+        logger.info('Creating LS dataset...')
+        make_fasta_ls_ts('LS.fasl', wt_sequence, sub_ls, val_ls)
+        logger.info('Creating TS dataset...')
+        make_fasta_ls_ts('TS.fasl', wt_sequence, sub_ts, val_ts)
 
         try:
             no_rnd = int(no_rnd)
         except ValueError:
             no_rnd = 0
         if no_rnd != 0:
             random_set_counter = 1
             no_rnd = int(no_rnd)
             while random_set_counter <= no_rnd:
-                print(f'Creating random LS and TS No. {random_set_counter}...', end='\r')
                 sub_ls, val_ls, sub_ts, val_ts = make_sub_ls_ts_randomly(
                     single_variants, single_values,
                     higher_variants, higher_values
                 )
-                make_fasta_ls_ts('LS_random_' + str(random_set_counter) + '.fasta', wt_sequence, sub_ls, val_ls)
-                make_fasta_ls_ts('TS_random_' + str(random_set_counter) + '.fasta', wt_sequence, sub_ts, val_ts)
+                make_fasta_ls_ts('LS_random_' + str(random_set_counter) + '.fasl', wt_sequence, sub_ls, val_ls)
+                make_fasta_ls_ts('TS_random_' + str(random_set_counter) + '.fasl', wt_sequence, sub_ts, val_ts)
                 random_set_counter += 1
 
     elif arguments['mkps']:
         wt_sequence = get_wt_sequence(arguments['--wt'])
         csv_file = csv_input(arguments['--input'])
         t_drop = float(arguments['--drop'])
         df = drop_rows(csv_file, amino_acids, t_drop)
         drop_wt = []
         for i in range(len(df)):
             if df.iloc[i, 0] == 'WT':
-                print('Dropping wild-type (WT) from DataFrame as it cannot be used for (re-)combination.')
+                logger.info('Dropping wild-type (WT) from DataFrame as it cannot be used for (re-)combination.')
                 drop_wt.append(i)
         df = df.drop(drop_wt).reset_index(drop=True)
 
-        print('Length of provided sequence: {} amino acids.'.format(len(wt_sequence)))
+        logger.info(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
         single_variants, _, higher_variants, _ = get_variants(df, amino_acids, wt_sequence)
-        print('Using single substitution variants for (re-)combination. '
-              'Number of single variants: {}.'.format(len(single_variants)))
+        logger.info(f'Using single substitution variants for (re-)combination. '
+                    f'Number of single variants: {len(single_variants)}.')
         if len(single_variants) == 0:
-            print('Found NO single substitution variants for possible recombination! '
-                  'No prediction files can be created!')
+            logger.info('Found NO single substitution variants for possible recombination! '
+                        'No prediction files can be created!')
 
         if arguments['--drecomb']:
-            print('Creating Recomb_Double_Split...')
+            logger.info('Creating Recomb_Double_Split...')
             for no, files in enumerate(make_recombinations_double(single_variants)):
                 double_mutants = np.array(files)
                 create_split_files(double_mutants, single_variants, wt_sequence, 'Recomb_Double', no)
 
         if arguments['--trecomb']:
-            print('Creating Recomb_Triple_Split...')
+            logger.info('Creating Recomb_Triple_Split...')
             for no, files in enumerate(make_recombinations_triple(single_variants)):
                 triple_mutants = np.array(files)
                 create_split_files(triple_mutants, single_variants, wt_sequence, 'Recomb_Triple', no)
 
         if arguments['--qarecomb']:
-            print('Beware that this step might require much disk space as PyPEF is '
-                  'creating prediction files in TXT format. Creating Recomb_Quadruple_Split...')
+            logger.info('Beware that this step might require much disk space as PyPEF is '
+                        'creating prediction files in TXT format. Creating Recomb_Quadruple_Split...')
             for no, files in enumerate(make_recombinations_quadruple(single_variants)):
                 quadruple_mutants = np.array(files)
                 create_split_files(quadruple_mutants, single_variants, wt_sequence, 'Recomb_Quadruple', no)
 
         if arguments['--qirecomb']:
-            print('Beware that this step might require much disk space as PyPEF is '
-                  'creating prediction files in TXT format. Creating Recomb_Quintuple_Split...')
+            logger.info('Beware that this step might require much disk space as PyPEF is '
+                        'creating prediction files in plain text format. Creating Recomb_Quintuple_Split...')
             for no, files in enumerate(make_recombinations_quintuple(single_variants)):
                 quintuple_mutants = np.array(files)
                 create_split_files(quintuple_mutants, single_variants, wt_sequence, 'Recomb_Quintuple', no)
 
         if arguments['--ddiverse']:
-            print('Creating Diverse_Double_Split...')
+            logger.info('Creating Diverse_Double_Split...')
             # if functions required, uncomment the next two lines and comment the other ones
             # for no, files in enumerate(
             #     make_recombinations_double_all_diverse_and_all_positions(wt_sequence, amino_acids)):
             for no, files in enumerate(make_combinations_double_all_diverse(single_variants, amino_acids)):
                 doubles = np.array(files)
                 create_split_files(doubles, single_variants, wt_sequence, 'Diverse_Double', no + 1)
 
         if arguments['--tdiverse']:
-            print('Beware that this step might require much disk space as PyPEF is '
-                  'creating prediction files in TXT format. Creating Diverse_Triple_Split... ')
+            logger.info('Beware that this step might require much disk space as PyPEF is '
+                        'creating prediction files in plain text format. Creating Diverse_Triple_Split... ')
             for no, files in enumerate(make_combinations_triple_all_diverse(single_variants, amino_acids)):
                 triples = np.array(files)
                 create_split_files(triples, single_variants, wt_sequence, 'Diverse_Triple', no + 1)
 
         if arguments['--qdiverse']:
-            print('Beware that this step might require much disk space as PyPEF is '
-                  'creating prediction files in TXT format. Creating Diverse_Quadruple_Split...')
+            logger.info('Beware that this step might require much disk space as PyPEF is '
+                       'creating prediction files in plain text format. Creating Diverse_Quadruple_Split...')
             for no, files in enumerate(make_combinations_quadruple_all_diverse(single_variants, amino_acids)):
                 quadruples = np.array(files)
                 create_split_files(quadruples, single_variants, wt_sequence, 'Diverse_Quadruple', no + 1)
 
         if arguments['--drecomb'] is False and arguments['--trecomb'] is False \
                 and arguments['--qarecomb'] is False and arguments['--qirecomb'] is False \
                 and arguments['--ddiverse'] is False and arguments['--tdiverse'] is False \
                 and arguments['--qdiverse'] is False:
-            print(f'\nMaking prediction set fasta file from {csv_file}...\n')
+            logger.info(f'\nMaking prediction set fasta file from {csv_file}...\n')
             make_fasta_ps(
                 filename=f'{get_basename(csv_file)}_prediction_set.fasta',
                 wt=wt_sequence,
                 substitution=tuple(list(single_variants)+list(higher_variants))
             )
 
     # Metropolis-Hastings-driven directed evolution, similar to Biswas et al.:
@@ -183,16 +185,16 @@
             else:
                 ml_or_hybrid = 'hybrid'
         else:
             dca_encoder = None
             ml_or_hybrid = 'ml'
         # Prediction using a saved model Pickle file specific AAindex used for encoding
         # Model saved in Pickle file also for DCA-based encoding, a default file name
-        print('Not counting WT as variant in directed evolution '
-              'as it cannot be used for (re-)combination.')
+        logger.info('Not counting WT as variant in directed evolution '
+                    'as it cannot be used for (re-)combination.')
         path = os.getcwd()
         try:
             # "temperature" parameter: determines sensitivity of Metropolis-Hastings acceptance criteria
             temp = float(arguments['--temp'])
             # how many subsequent mutation trials per simulated evolution trajectory
             num_iterations = int(arguments['--numiter'])
             # how many separate evolution trajectories to run
@@ -203,35 +205,35 @@
         y_wt = arguments['--y_wt']
         negative = arguments['--negative']
         # Metropolis-Hastings-driven directed evolution on single mutant position csv data
         usecsv = arguments['--usecsv']
         if usecsv:
             csv_file = csv_input(arguments['--input'])
             t_drop = float(arguments['--drop'])
-            print(f'Length of provided sequence: {len(s_wt)} amino acids.')
+            logger.info(f'Length of provided sequence: {len(s_wt)} amino acids.')
             df = drop_rows(csv_file, amino_acids, t_drop)
             drop_wt = []
             for i in range(len(df)):
                 if df.iloc[i, 0] == 'WT':
-                    print('Using fitness value (y_WT) for wild-type (WT) as specified in CSV.')
+                    logger.info('Using fitness value (y_WT) for wild-type (WT) as specified in CSV.')
                     drop_wt.append(i)
                     y_wt = df.iloc[i, 1]
             df = df.drop(drop_wt).reset_index(drop=True)
             single_variants, single_values, higher_variants, higher_values = \
                 get_variants(df, amino_acids, s_wt)
-            print(f'Number of single variants: {len(single_variants)}.')
+            logger.info(f'Number of single variants: {len(single_variants)}.')
             if len(single_variants) == 0:
-                print('Found NO single substitution variants for possible recombination!')
+                logger.info('Found NO single substitution variants for possible recombination!')
             single_vars, single_ys = list(single_variants), list(single_values)  # only tuples to lists
 
         else:
             single_vars = None  # What happens now? (Full diverse?)
         # Metropolis-Hastings-driven directed evolution on single mutant .csv amino acid substitution data
         csvaa = arguments['--csvaa']  # only use identified substitutions --> taken from CSV file
-        print('Running evolution trajectories and plotting...\n')
+        logger.info('Running evolution trajectories and plotting...\n')
         DirectedEvolution(
             ml_or_hybrid=ml_or_hybrid,
             encoding=arguments['--encoding'],
             s_wt=s_wt,
             y_wt=y_wt,
             single_vars=single_vars,
             num_iterations=num_iterations,
@@ -262,27 +264,27 @@
             substitution_sep=arguments['--mutation_sep']
         )
 
     elif arguments['encode']:  # sole parallelized task for utils for DCA encoding
         encoded_sequences = None
         df = drop_rows(arguments['--input'], amino_acids, arguments['--drop'])
         wt_sequence = get_wt_sequence(arguments['--wt'])
-        print(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
+        logger.info(f'Length of provided sequence: {len(wt_sequence)} amino acids.')
         single_variants, single_values, higher_variants, higher_values = get_variants(
             df, amino_acids, wt_sequence)
         variants = list(single_variants) + list(higher_variants)
         fitnesses = list(single_values) + list(higher_values)
         variants, fitnesses, sequences = get_seqs_from_var_name(wt_sequence, variants, fitnesses)
         assert len(variants) == len(fitnesses) == len(sequences)
-        print('Encoding variant sequences...')
+        logger.info('Encoding variant sequences...')
 
         if arguments['--encoding'] == 'dca':
             threads = abs(arguments['--threads']) if arguments['--threads'] is not None else 1
             threads = threads + 1 if threads == 0 else threads
-            print(f'Using {threads} thread(s) for running...')
+            logger.info(f'Using {threads} thread(s) for running...')
             dca_encode = DCAEncoding(
                 params_file=arguments['--params'],
                 separator=arguments['--mutation_sep'],
                 verbose=False
             )
             if threads > 1:
                 ray.init()
@@ -317,24 +319,22 @@
         elif arguments['--encoding'] == 'aaidx':
             if arguments['--model'] is None:
                 raise SystemError(
                     "Define the AAindex to use for encoding with the "
                     "flag --model AAINDEX, e.g.: --model CORJ870104."
                 )
             aa_index_encoder = AAIndexEncoding(
-                path_aaidx_txt_path_from_utils(arguments['--model']), sequences
+                full_aaidx_txt_path(arguments['--model'] + '.txt'), sequences
             )
             x_fft, x_raw = aa_index_encoder.collect_encoded_sequences()
             if arguments['--nofft']:
                 encoded_sequences = x_raw
             else:
                 encoded_sequences = x_fft
 
         generate_dataframe_and_save_csv(  # put WT at pos. 0 for hybrid low_N or extrapolation
             variants=variants,
             sequence_encodings=encoded_sequences,
             fitnesses=fitnesses,
             csv_file=arguments['--input'],
             encoding_type=arguments['--encoding']
         )
-
-    print('\nDone!\n')
```

### Comparing `pypef-0.2.3/pypef/utils/sto2a2m.py` & `pypef-0.2.4/pypef/utils/sto2a2m.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # https://doi.org/10.1021/acs.jcim.1c00099
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
+import logging
+logger = logging.getLogger('pypef.utils.sto2a2m')
 import numpy as np
 from tqdm import tqdm
 from Bio import AlignIO
 
 
 def convert_sto2a2m(
         sto_file: str,
@@ -31,17 +33,17 @@
     Removes specific sequences with inter and/or intra gaps
     over specific thresholds.
     """
     # Generate the a2m output filename
     a2m_file = f"{sto_file.split('.sto')[0]}.a2m"
 
     # Load the stockholm alignment
-    print('Loading MSA in stockholm format...')
+    logger.info('Loading MSA in stockholm format...')
     sto_alignment = AlignIO.read(sto_file, 'stockholm')
-    print('Trimming MSA...')
+    logger.info('Trimming MSA...')
     # Save this 'raw' multiple sequence alignment as numpy array 
     raw_msa = []
     for record in tqdm(sto_alignment):
         raw_msa.append(np.array(record.seq))
     raw_msa = np.array(raw_msa)
 
     # 1st processing step
@@ -77,13 +79,13 @@
                 f.write('>' + seq_cls.id + '\n')
             for chunk in [seq[x:x + chunk_size] for x in range(0, len(seq), chunk_size)]:
                 f.write("".join(chunk) + '\n')
 
     # Get number of sequences and effective sites in the alignment
     n_seqs = msa_final.shape[0]
     n_sites = sum(1 for char in msa_final[0] if char.isupper())
-    print(f'Generated trimmed MSA {a2m_file} in A2M format:')
-    print(f'No. of sequences: {n_seqs}')
-    print(f'No. of effective sites: {n_sites} (out of {target_len} sites)')
-    print(f'-le --lambdae: {0.2 * (n_sites - 1):.1f}')
+    logger.info(f'Generated trimmed MSA {a2m_file} in A2M format:\n'
+                f'No. of sequences: {n_seqs}\n'
+                f'No. of effective sites: {n_sites} (out of {target_len} sites)\n'
+                f'-le --lambdae: {0.2 * (n_sites - 1):.1f}')
 
     return n_seqs, n_sites, target_len
```

### Comparing `pypef-0.2.3/pypef/utils/variant_data.py` & `pypef-0.2.4/pypef/utils/variant_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # https://doi.org/10.1021/acs.jcim.1c00099
 # Niklas E. Siedhoff1,§, Alexander-Maurice Illig1,§, Ulrich Schwaneberg1,2, Mehdi D. Davari1,*
 # 1Institute of Biotechnology, RWTH Aachen University, Worringer Weg 3, 52074 Aachen, Germany
 # 2DWI-Leibniz Institute for Interactive Materials, Forckenbeckstraße 50, 52074 Aachen, Germany
 # *Corresponding author
 # §Equal contribution
 
+from __future__ import annotations
 import os
-import sys
+
 import numpy as np
 import pandas as pd
 
 
 amino_acids = [
     'A', 'C', 'D', 'E', 'F',
     'G', 'H', 'I', 'K', 'L',
@@ -64,86 +65,132 @@
     e.g. path/to/pypef/utils/../aaidx/AAindex/FAUJ880104.txt.
     """
     modules_path = os.path.dirname(os.path.abspath(__file__))
     return os.path.join(modules_path, '..', 'ml', 'AAindex', f'{filename}.txt')
 
 
 def get_sequences_from_file(
-        fasta,
-        mult_path=None
-):
-    """
-    "Get_Sequences" reads (learning and test).fasta format
-    files and extracts the name, the target value and the
-    sequence of the peptide. See example directory for required
-    fasta file format. Make sure every marker (> and ;) is
-    seperated by an space ' ' from the value respectively name.
+        fasta: str,
+        mult_path: str | None = None
+) -> (np.ndarray, np.ndarray, np.ndarray):
+    """
+    "Get_Sequences" reads (learning and test) .fasta and
+    .fasta-like ".fasl" format files and extracts the name,
+    the target value and the sequence of the protein.
+    Only takes one-liner sequences for correct input.
+    See example directory for required fasta file format.
+    Make sure every marker (> and ;) is seperated by a
+    space ' ' from the value respectively name.
     """
     if mult_path is not None:
         os.chdir(mult_path)
 
     sequences = []
     values = []
     names_of_mutations = []
 
     with open(fasta, 'r') as f:
+        words = ""
         for line in f:
-            if '>' in line:
+            if line.startswith('>'):
+                if words != "":
+                    sequences.append(words)
                 words = line.split('>')
                 names_of_mutations.append(words[1].strip())
+                words = ""
 
-            elif '#' in line:
+            elif line.startswith('#'):
                 pass  # are comments
 
-            elif ';' in line:
+            elif line.startswith(';'):
+                if words != "":
+                    sequences.append(words)
                 words = line.split(';')
                 values.append(float(words[1].strip()))
+                words = ""
 
             else:
                 try:
-                    words = line.split()
-                    sequences.append(words[0])
+                    words += line.strip()
                 except IndexError:
                     raise IndexError("Learning or Validation sets (.fasta) likely "
                                      "have emtpy lines (e.g. at end of file)")
-
+        if words != "":
+            sequences.append(words)
     # Check consistency
     if len(values) != 0:
         if len(sequences) != len(values):
-            print('Error: Number of sequences does '
-                  'not fit with number of target values!')
-            print('Number of sequences: {}, Number of target values: {}.'.format(
-                str(len(sequences)), str(len(values))))
-            sys.exit()
+            raise SystemError(
+                f'Error: Number of sequences does not fit with number of target values! '
+                f'Number of sequences: {str(len(sequences))}, Number of target values: {str(len(values))}.'
+            )
     if mult_path is not None:
         os.chdir('..')
 
-    return sequences, names_of_mutations, values
+    return np.array(sequences), np.array(names_of_mutations), np.array(values)
 
 
 def remove_nan_encoded_positions(
-        xs: list,
-        ys: list = None
-) -> tuple[list, list]:
+        xs: np.ndarray | list,
+        *yss
+):
     """
     Removes encoded sequence (x) of sequence list xs when NaNs occur in x.
     Also removes the corresponding fitness value y (f(x) --> y) at position i.
     ys can als be any type of list, e.g. variants or sequences.
     """
-    if ys is None:
-        ys = np.zeros(len(xs))
+    if type(xs) == np.ndarray:
+        xs = list(xs)
+    temp = []
+    for ys in yss:
+        try:
+            if isinstance(ys, pd.Series):
+                temp.append(list(ys))
+            elif ys is None:
+                if len(yss) == 1:
+                    temp = (None,)
+                else:
+                    temp.append([None])
+            else:
+                temp.append(list(ys))
+        except ValueError:
+            temp.append(list(ys))
+        except TypeError:
+            temp = (None,)
+    if temp:
+        yss = temp
+    if not yss == () and not yss == (None,):
+        for i, ys in enumerate(yss):
+            assert len(xs) == len(ys), "Number of input sequences to be compared unequal."
+            try:
+                for j, x in enumerate(xs):
+                    if np.shape(np.array(xs, dtype='object'))[1] and np.shape(np.array(ys, dtype='object'))[1]:
+                        assert len(xs[j]) == len(ys[j]), "Length of input sequences to be compared unequal."
+            except IndexError:
+                break
     drop = []
     for i, x in enumerate(xs):
-        if None in x:
-            drop.append(i)
+        try:
+            if None in x:
+                drop.append(i)
+        except TypeError:
+            raise TypeError(
+                "Take lists of lists as input, e.g., for single sequence "
+                "[[1, 2, 3, 4]]."
+            )
     drop = sorted(drop, reverse=True)
     for idx in drop:
         del xs[idx]
-        del ys[idx]
-    return xs, ys
+        if not yss == () and not yss == (None,):
+            for ys in yss:
+                del ys[idx]
+    if len(yss) == 1:
+        return np.array(xs, dtype='object'), np.array(yss[0])
+
+    return np.array(xs, dtype='object'), *np.array(yss, dtype='object')
 
 
 def get_basename(filename: str) -> str:
     """
     Description
     -----------
     Extracts and returns the basename of the filename.
```

### Comparing `pypef-0.2.3/pypef.egg-info/PKG-INFO` & `pypef-0.2.4/pypef.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: pypef
-Version: 0.2.3
+Version: 0.2.4
 Summary: A command-line interface (CLI) tool for performing data-driven protein engineering by building machine learning (ML)-trained regression models from sequence variant fitness data (in CSV format) based on different techniques for protein sequence encoding. Next to building pure ML models, 'hybrid modeling' is also possible using a blended model optimized for predictive contributions of a statistical and an ML-based prediction.
 Home-page: https://github.com/niklases/PyPEF
 Author: Niklas Siedhoff & Alexander-Maurice Illig
 Author-email: n.siedhoff@biotec.rwth-aachen.de
 License: CC BY-NC-SA 4.0
 Keywords: Pythonic Protein Engineering Framework
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
+Requires-Python: >= 3.9, < 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 For detailed description including a short Jupyter Notebook-based tutorial please refer to the GitHub page.
-
```

### Comparing `pypef-0.2.3/pypef.egg-info/SOURCES.txt` & `pypef-0.2.4/pypef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypef-0.2.3/setup.py` & `pypef-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
-# for installation run me with: pip install .
+# for installation run me with: pip install . --use-feature=in-tree-build
 
 
 from setuptools import setup, find_packages
 
 
 with open("requirements.txt", "r", encoding="utf-8") as install_requirements:
     requirements = install_requirements.read()
 
 setup(
     name='pypef',
-    version='0.2.3',
+    version='0.2.4',
     author='Niklas Siedhoff & Alexander-Maurice Illig',
     author_email='n.siedhoff@biotec.rwth-aachen.de',
     license='CC BY-NC-SA 4.0',
     description='A command-line interface (CLI) tool for performing data-driven protein engineering '
                 'by building machine learning (ML)-trained regression models from sequence variant '
                 'fitness data (in CSV format) based on different techniques for protein sequence encoding. '
                 'Next to building pure ML models, \'hybrid modeling\' is also possible using a blended '
@@ -24,21 +24,22 @@
     long_description_content_type='text/markdown',
     url='https://github.com/niklases/PyPEF',
     py_modules=['pypef'],
     packages=find_packages(include=['pypef', 'pypef.*']),
     package_data={'pypef': ['ml/AAindex/*', 'ml/AAindex/Refined_cluster_indices_r0.93_r0.97/*']},
     include_package_data=True,
     install_requires=[requirements],
-    python_requires='>=3.9',
+    python_requires='>= 3.9, < 3.12',
     keywords='Pythonic Protein Engineering Framework',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Scientific/Engineering :: Artificial Intelligence'
     ],
     entry_points={
         'console_scripts': [
             'pypef = pypef.main:run_main'
         ],
```

