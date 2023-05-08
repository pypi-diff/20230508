# Comparing `tmp/popbill-1.8.0.tar.gz` & `tmp/popbill-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/popbill-1.8.0.tar", last modified: Tue Sep 11 08:28:30 2018, max compression
+gzip compressed data, was "dist/popbill-1.9.0.tar", last modified: Wed Oct 10 06:48:13 2018, max compression
```

## Comparing `popbill-1.8.0.tar` & `popbill-1.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 cream      (501) staff       (20)        0 2018-09-11 08:28:30.000000 popbill-1.8.0/
--rw-r--r--   0 cream      (501) staff       (20)     1073 2018-09-11 08:28:30.000000 popbill-1.8.0/PKG-INFO
-drwxr-xr-x   0 cream      (501) staff       (20)        0 2018-09-11 08:28:30.000000 popbill-1.8.0/popbill.egg-info/
--rw-r--r--   0 cream      (501) staff       (20)     1073 2018-09-11 08:28:30.000000 popbill-1.8.0/popbill.egg-info/PKG-INFO
--rw-r--r--   0 cream      (501) staff       (20)      479 2018-09-11 08:28:30.000000 popbill-1.8.0/popbill.egg-info/SOURCES.txt
--rw-r--r--   0 cream      (501) staff       (20)       47 2018-09-11 08:28:30.000000 popbill-1.8.0/popbill.egg-info/pbr.json
--rw-r--r--   0 cream      (501) staff       (20)        8 2018-09-11 08:28:30.000000 popbill-1.8.0/popbill.egg-info/requires.txt
--rw-r--r--   0 cream      (501) staff       (20)        8 2018-09-11 08:28:30.000000 popbill-1.8.0/popbill.egg-info/top_level.txt
--rw-r--r--   0 cream      (501) staff       (20)        1 2018-09-11 08:28:30.000000 popbill-1.8.0/popbill.egg-info/dependency_links.txt
--rw-r--r--   0 cream      (501) staff       (20)     1747 2018-09-11 08:20:24.000000 popbill-1.8.0/setup.py
--rw-r--r--   0 cream      (501) staff       (20)       59 2018-09-11 08:28:30.000000 popbill-1.8.0/setup.cfg
-drwxr-xr-x   0 cream      (501) staff       (20)        0 2018-09-11 08:28:30.000000 popbill-1.8.0/popbill/
--rw-r--r--   0 cream      (501) staff       (20)      908 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/__init__.py
--rw-r--r--   0 cream      (501) staff       (20)    17696 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/faxService.py
--rw-r--r--   0 cream      (501) staff       (20)     7395 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/htCashbillService.py
--rw-r--r--   0 cream      (501) staff       (20)    43140 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/taxinvoiceService.py
--rw-r--r--   0 cream      (501) staff       (20)    10269 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/htTaxinvoiceService.py
--rw-r--r--   0 cream      (501) staff       (20)    17987 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/kakaoService.py
--rw-r--r--   0 cream      (501) staff       (20)    35655 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/statementService.py
--rw-r--r--   0 cream      (501) staff       (20)     3091 2016-08-09 01:00:11.000000 popbill-1.8.0/popbill/closedownService.py
--rw-r--r--   0 cream      (501) staff       (20)    21147 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/messageService.py
--rw-r--r--   0 cream      (501) staff       (20)    14531 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/base.py
--rw-r--r--   0 cream      (501) staff       (20)    23874 2018-09-11 08:20:24.000000 popbill-1.8.0/popbill/cashbillService.py
--rw-r--r--   0 cream      (501) staff       (20)      664 2018-09-11 08:20:24.000000 popbill-1.8.0/README.rst
+drwxr-xr-x   0 cream      (501) staff       (20)        0 2018-10-10 06:48:13.000000 popbill-1.9.0/
+-rw-r--r--   0 cream      (501) staff       (20)     1073 2018-10-10 06:48:13.000000 popbill-1.9.0/PKG-INFO
+drwxr-xr-x   0 cream      (501) staff       (20)        0 2018-10-10 06:48:13.000000 popbill-1.9.0/popbill.egg-info/
+-rw-r--r--   0 cream      (501) staff       (20)     1073 2018-10-10 06:48:12.000000 popbill-1.9.0/popbill.egg-info/PKG-INFO
+-rw-r--r--   0 cream      (501) staff       (20)      479 2018-10-10 06:48:13.000000 popbill-1.9.0/popbill.egg-info/SOURCES.txt
+-rw-r--r--   0 cream      (501) staff       (20)       47 2018-10-10 06:48:12.000000 popbill-1.9.0/popbill.egg-info/pbr.json
+-rw-r--r--   0 cream      (501) staff       (20)        8 2018-10-10 06:48:12.000000 popbill-1.9.0/popbill.egg-info/requires.txt
+-rw-r--r--   0 cream      (501) staff       (20)        8 2018-10-10 06:48:12.000000 popbill-1.9.0/popbill.egg-info/top_level.txt
+-rw-r--r--   0 cream      (501) staff       (20)        1 2018-10-10 06:48:12.000000 popbill-1.9.0/popbill.egg-info/dependency_links.txt
+-rw-r--r--   0 cream      (501) staff       (20)     1747 2018-10-10 06:47:57.000000 popbill-1.9.0/setup.py
+-rw-r--r--   0 cream      (501) staff       (20)       59 2018-10-10 06:48:13.000000 popbill-1.9.0/setup.cfg
+drwxr-xr-x   0 cream      (501) staff       (20)        0 2018-10-10 06:48:13.000000 popbill-1.9.0/popbill/
+-rw-r--r--   0 cream      (501) staff       (20)      908 2018-09-11 08:20:24.000000 popbill-1.9.0/popbill/__init__.py
+-rw-r--r--   0 cream      (501) staff       (20)    17868 2018-10-10 06:47:57.000000 popbill-1.9.0/popbill/faxService.py
+-rw-r--r--   0 cream      (501) staff       (20)    10340 2018-10-10 06:47:57.000000 popbill-1.9.0/popbill/htCashbillService.py
+-rw-r--r--   0 cream      (501) staff       (20)    43603 2018-10-10 06:47:57.000000 popbill-1.9.0/popbill/taxinvoiceService.py
+-rw-r--r--   0 cream      (501) staff       (20)    14024 2018-10-10 06:47:57.000000 popbill-1.9.0/popbill/htTaxinvoiceService.py
+-rw-r--r--   0 cream      (501) staff       (20)    18176 2018-10-10 06:47:57.000000 popbill-1.9.0/popbill/kakaoService.py
+-rw-r--r--   0 cream      (501) staff       (20)    35655 2018-09-11 08:20:24.000000 popbill-1.9.0/popbill/statementService.py
+-rw-r--r--   0 cream      (501) staff       (20)     3091 2016-08-09 01:00:11.000000 popbill-1.9.0/popbill/closedownService.py
+-rw-r--r--   0 cream      (501) staff       (20)    21323 2018-10-10 06:47:57.000000 popbill-1.9.0/popbill/messageService.py
+-rw-r--r--   0 cream      (501) staff       (20)    14531 2018-09-11 08:20:24.000000 popbill-1.9.0/popbill/base.py
+-rw-r--r--   0 cream      (501) staff       (20)    24052 2018-10-10 06:47:57.000000 popbill-1.9.0/popbill/cashbillService.py
+-rw-r--r--   0 cream      (501) staff       (20)      664 2018-10-10 06:47:57.000000 popbill-1.9.0/README.rst
```

### Comparing `popbill-1.8.0/PKG-INFO` & `popbill-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: popbill
-Version: 1.8.0
+Version: 1.9.0
 Summary: Popbill API SDK Library
 Home-page: https://github.com/linkhub-sdk/Popbill.py
 Author: Kim Seongjun
 Author-email: pallet027@gmail.com
 License: MIT
-Download-URL: https://github.com/linkhub-sdk/Popbill.py/archive/1.8.0.tar.gz
+Download-URL: https://github.com/linkhub-sdk/Popbill.py/archive/1.9.0.tar.gz
 Description: Popbill API SDK. Consist of Taxinvice Service. http://www.popbill.com
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
```

### Comparing `popbill-1.8.0/popbill.egg-info/PKG-INFO` & `popbill-1.9.0/popbill.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: popbill
-Version: 1.8.0
+Version: 1.9.0
 Summary: Popbill API SDK Library
 Home-page: https://github.com/linkhub-sdk/Popbill.py
 Author: Kim Seongjun
 Author-email: pallet027@gmail.com
 License: MIT
-Download-URL: https://github.com/linkhub-sdk/Popbill.py/archive/1.8.0.tar.gz
+Download-URL: https://github.com/linkhub-sdk/Popbill.py/archive/1.9.0.tar.gz
 Description: Popbill API SDK. Consist of Taxinvice Service. http://www.popbill.com
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
```

### Comparing `popbill-1.8.0/setup.py` & `popbill-1.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
 import sys
 
-version = '1.8.0'
+version = '1.9.0'
 
 if sys.version_info <= (2, 5):
     error = "ERROR: popbill requires Python Version 2.6 or above...exiting."
     print(error, file=sys.stderr)
     sys.exit(1)
 
 setup(name = "popbill",
```

### Comparing `popbill-1.8.0/popbill/__init__.py` & `popbill-1.9.0/popbill/__init__.py`

 * *Files identical despite different names*

### Comparing `popbill-1.8.0/popbill/faxService.py` & `popbill-1.9.0/popbill/faxService.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,27 +63,28 @@
             raise
                 PopbillException
         """
 
         result = self._httpget('/FAX/UnitCost', CorpNum)
         return int(result.unitCost)
 
-    def search(self, CorpNum, SDate, EDate, State, ReserveYN, SenderOnly, Page, PerPage, Order, UserID=None):
+    def search(self, CorpNum, SDate, EDate, State, ReserveYN, SenderOnly, Page, PerPage, Order, UserID=None, QString=None):
         """ 목록 조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 SDate : 시작일자, 표시형식(yyyyMMdd)
                 EDate : 종료일자, 표시형식(yyyyMMdd)
                 State : 전송상태 배열, 1-대기, 2-성공, 3-실패, 4-취소
                 ReserveYN : 예약여부, False-전체조회, True-예약전송건 조회
                 SenderOnly : 개인조회여부, False-개인조회, True-회사조회
                 Page : 페이지번호
                 PerPage : 페이지당 목록개수
                 Order : 정렬방향, D-내림차순, A-오름차순
                 UserID : 팝빌 회원아이디
+                QString : 조회 검색어, 발신자명 또는 수신자명 기재
         """
 
         if SDate == None or SDate == '':
             raise PopbillException(-99999999, "시작일자가 입력되지 않았습니다.")
 
         if EDate == None or EDate == '':
             raise PopbillException(-99999999, "종료일자가 입력되지 않았습니다.")
@@ -98,14 +99,17 @@
         if SenderOnly:
             uri += '&SenderOnly=1'
 
         uri += '&Page=' + str(Page)
         uri += '&PerPage=' + str(PerPage)
         uri += '&Order=' + Order
 
+        if QString is not None:
+            uri += '&QString=' + QString
+
         return self._httpget(uri, CorpNum, UserID)
 
     def getFaxResult(self, CorpNum, ReceiptNum, UserID=None):
         """ 팩스 전송결과 조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 ReceiptNum : 전송요청시 발급받은 접수번호
```

### Comparing `popbill-1.8.0/popbill/htCashbillService.py` & `popbill-1.9.0/popbill/htCashbillService.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,191 +5,267 @@
 #
 # http://www.popbill.com
 # Author : Jeong Yohan (code@linkhub.co.kr)
 # Written : 2015-07-16
 # Updated : 2016-07-27
 # Thanks for your interest.
 
-from .base import PopbillBase,PopbillException
+from .base import PopbillBase, PopbillException
+
 
 class HTCashbillService(PopbillBase):
     """ 팝빌 홈택스 현금영수증 연계 API Service Implementation. """
 
-    def __init__(self,LinkID,SecretKey):
+    def __init__(self, LinkID, SecretKey):
         """ 생성자
             args
                 LinkID : 링크허브에서 발급받은 링크아이디(LinkID)
                 SecretKeye 링크허브에서 발급받은 비밀키(SecretKey)
         """
 
-        super(self.__class__,self).__init__(LinkID,SecretKey)
+        super(self.__class__, self).__init__(LinkID, SecretKey)
         self._addScope("141")
 
-    def getChargeInfo(self, CorpNum, UserID = None):
+    def getChargeInfo(self, CorpNum, UserID=None):
         """ 과금정보 확인
             args
                 CorpNum : 회원 사업자번호
                 UserID : 팝빌 회원아이디
             return
                 과금정보 객체
             raise
                 PopbillException
         """
 
         return self._httpget('/HomeTax/Cashbill/ChargeInfo', CorpNum, UserID)
 
-    def requestJob(self, CorpNum, Type, SDate, EDate, UserID = None):
+    def requestJob(self, CorpNum, Type, SDate, EDate, UserID=None):
         """ 수집 요청
             args
                 CorpNum : 팝빌회원 사업자번호
-                Type : 현금영수증 유형, SELL-매출, BUY-매입,
+                Type : 문서형태, SELL-매출, BUY-매입,
                 SDate : 시작일자, 표시형식(yyyyMMdd)
                 EDate : 종료일자, 표시형식(yyyyMMdd)
                 UserID : 팝빌회원 아이디
             return
                 작업아이디 (jobID)
             raise
                 PopbillException
         """
 
         if Type == None or Type == '':
-            raise PopbillException(-99999999, "현금영수증 유형이 입력되지 않았습니다.")
+            raise PopbillException(-99999999, "문서형태이 입력되지 않았습니다.")
 
         if SDate == None or SDate == '':
             raise PopbillException(-99999999, "시작일자가 입력되지 않았습니다.")
 
         if EDate == None or EDate == '':
             raise PopbillException(-99999999, "종료일자가 입력되지 않았습니다.")
 
         uri = '/HomeTax/Cashbill/' + Type
         uri += '?SDate=' + SDate
         uri += '&EDate=' + EDate
 
         return self._httppost(uri, "", CorpNum, UserID).jobID
 
-    def getJobState(self, CorpNum, JobID, UserID = None):
+    def getJobState(self, CorpNum, JobID, UserID=None):
         """ 수집 상태 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 JobID : 작업아이디
                 UserID : 팝빌회원 아이디
             return
                 수집 상태 정보
             raise
                 PopbillException
         """
         if JobID == None or len(JobID) != 18:
-            raise PopbillException(-99999999,"작업아이디(jobID)가 올바르지 않습니다.")
+            raise PopbillException(-99999999, "작업아이디(jobID)가 올바르지 않습니다.")
 
-        return self._httpget('/HomeTax/Cashbill/'+JobID+'/State', CorpNum, UserID)
+        return self._httpget('/HomeTax/Cashbill/' + JobID + '/State', CorpNum, UserID)
 
-    def listActiveJob(self, CorpNum, UserID = None):
+    def listActiveJob(self, CorpNum, UserID=None):
         """ 수집 상태 목록 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 수집 상태 정보 목록
             raise
                 PopbillException
         """
 
         return self._httpget('/HomeTax/Cashbill/JobList', CorpNum, UserID)
 
-    def search(self, CorpNum, JobID, TradeType, TradeUsage, Page, PerPage, Order, UserID = None):
+    def search(self, CorpNum, JobID, TradeType, TradeUsage, Page, PerPage, Order, UserID=None):
         """ 수집 결과 조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 JobID : 작업아이디
-                TradeType : 현금영수증 유형 배열, N-일반 현금영수증, C-취소 현금영수증
-                TradeUsage : 거래용도 배열, P-소등공제용, C-지출증빙용
+                TradeType : 문서형태 배열, N-일반 현금영수증, C-취소 현금영수증
+                TradeUsage : 거래구분 배열, P-소등공제용, C-지출증빙용
                 Page : 페이지 번호
                 PerPage : 페이지당 목록 개수, 최대 1000개
                 Order : 정렬 방향, D-내림차순, A-오름차순
                 UserID : 팝빌회원 아이디
             return
                 수집 결과 정보
             raise
                 PopbillException
         """
-        if JobID == None or len(JobID) != 18 :
+        if JobID == None or len(JobID) != 18:
             raise PopbillException(-99999999, "작업아이디(jobID)가 올바르지 않습니다.")
 
         uri = '/HomeTax/Cashbill/' + JobID
         uri += '?TradeType=' + ','.join(TradeType)
         uri += '&TradeUsage=' + ','.join(TradeUsage)
         uri += '&Page=' + str(Page)
         uri += '&PerPage=' + str(PerPage)
         uri += '&Order=' + Order
 
         return self._httpget(uri, CorpNum, UserID)
 
-    def summary(self, CorpNum, JobID, TradeType, TradeUsage, UserID = None):
+    def summary(self, CorpNum, JobID, TradeType, TradeUsage, UserID=None):
         """ 수집 결과 요약정보 조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 JobID : 작업아이디
-                TradeType : 현금영수증 유형 배열, N-일반 현금영수증, C-취소 현금영수증
-                TradeUsage : 거래용도 배열, P-소등공제용, C-지출증빙용
+                TradeType : 문서형태 배열, N-일반 현금영수증, C-취소 현금영수증
+                TradeUsage : 거래구분 배열, P-소등공제용, C-지출증빙용
                 UserID : 팝빌회원 아이디
             return
                 수집 결과 요약정보
             raise
                 PopbillException
         """
-        if JobID == None or len(JobID) != 18 :
+        if JobID == None or len(JobID) != 18:
             raise PopbillException(-99999999, "작업아이디(jobID)가 올바르지 않습니다.")
 
         uri = '/HomeTax/Cashbill/' + JobID + '/Summary'
         uri += '?TradeType=' + ','.join(TradeType)
         uri += '&TradeUsage=' + ','.join(TradeUsage)
 
         return self._httpget(uri, CorpNum, UserID)
 
-    def getFlatRatePopUpURL(self, CorpNum, UserID = None):
+    def getFlatRatePopUpURL(self, CorpNum, UserID=None):
         """ 정액제 서비스 신청 URL
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 정액제 서비스 팝업 URL
             raise
                 PopbillException
         """
         return self._httpget('/HomeTax/Cashbill?TG=CHRG', CorpNum, UserID).url
 
-    def getCertificatePopUpURL(self, CorpNum, UserID = None):
+    def getCertificatePopUpURL(self, CorpNum, UserID=None):
         """ 홈택스 공인인증서 등록 URL
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 공인인증서 등록 팝업 URL
             raise
                 PopbillException
         """
         return self._httpget('/HomeTax/Cashbill?TG=CERT', CorpNum, UserID).url
 
-    def getFlatRateState(self, CorpNum, UserID = None) :
+    def getFlatRateState(self, CorpNum, UserID=None):
         """ 정액제 서비스 상태 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 정액제 서비스 상태 정보
             raise
                 PopbillException
         """
         return self._httpget('/HomeTax/Cashbill/Contract', CorpNum, UserID)
 
-    def getCertificateExpireDate(self, CorpNum, UserID = None):
+    def getCertificateExpireDate(self, CorpNum, UserID=None):
         """ 공인인증서 만료일자 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 공인인증서 만료일자
             raise
                 PopbillException
         """
 
         return self._httpget('/HomeTax/Cashbill/CertInfo', CorpNum, UserID).certificateExpiration
+
+    def checkCertValidation(self, CorpNum, UserID=None):
+        """ 홈택스 공인인증서 로그인 테스트
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+
+        return self._httpget('/HomeTax/Cashbill/CertCheck', CorpNum, UserID)
+
+    def registDeptUser(self, CorpNum, DeptUserID, DeptUserPWD, UserID=None):
+        """ 홈택스 현금영수증 부서사용자 계정 등록
+            args
+                CorpNum : 팝빌회원 사업자번호
+                DeptUserID : 홈택스 부서사용자 계정아이디
+                DeptUserPWD : 홈택스 부서사용자 계정비밀번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        if DeptUserID == None or len(DeptUserID) == 0:
+            raise PopbillException(-99999999, "홈택스 부서사용자 계정 아이디가 입력되지 않았습니다.")
+
+        if DeptUserPWD == None or len(DeptUserPWD) == 0:
+            raise PopbillException(-99999999, "홈택스 부서사용자 계정 비밀번호가 입력되지 않았습니다.")
+
+        req = {}
+        req["id"] = DeptUserID
+        req["pwd"] = DeptUserPWD
+
+        postData = self._stringtify(req)
+
+        return self._httppost("/HomeTax/Cashbill/DeptUser", postData, CorpNum, UserID)
+
+    def checkDeptUser(self, CorpNum, UserID=None):
+        """ 홈택스 현금영수증 부서사용자 등록정보 확인
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        return self._httpget('/HomeTax/Cashbill/DeptUser', CorpNum, UserID)
+
+    def checkLoginDeptUser(self, CorpNum, UserID=None):
+        """ 홈택스 현금영수증 부서사용자 로그인 테스트
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        return self._httpget('/HomeTax/Cashbill/DeptUser/Check', CorpNum, UserID)
+
+    def deleteDeptUser(self, CorpNum, UserID=None):
+        """ 홈택스 현금영수증 부서사용자 등록정보 삭제
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        return self._httppost("/HomeTax/Cashbill/DeptUser", "", CorpNum, UserID, "DELETE")
```

### Comparing `popbill-1.8.0/popbill/taxinvoiceService.py` & `popbill-1.9.0/popbill/taxinvoiceService.py`

 * *Files 0% similar despite different names*

```diff
@@ -983,14 +983,26 @@
 
         if SendYN == None or SendYN == '':
             raise PopbillException(-99999999, "메일전송 여부 항목이 입력되지 않았습니다.")
 
         uri = "/Taxinvoice/EmailSendConfig?EmailType=" + EmailType + "&SendYN=" + str(SendYN)
         return self._httppost(uri, "", Corpnum, UserID)
 
+    def checkCertValidation(self, CorpNum, UserID=None):
+        """ 팝빌에 등록된 공인인증서 유효성을 확인한다.
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+               처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        return self._httpget('/Taxinvoice/CertCheck', CorpNum, UserID)
+
 
 class Taxinvoice(object):
     def __init__(self, **kwargs):
         self.__dict__ = kwargs
 
 
 class TaxinvoiceDetail(object):
```

### Comparing `popbill-1.8.0/popbill/htTaxinvoiceService.py` & `popbill-1.9.0/popbill/htTaxinvoiceService.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,43 +5,44 @@
 #
 # http://www.popbill.com
 # Author : Jeong Yohan (code@linkhub.co.kr)
 # Written : 2015-07-16
 # Updated : 2016-07-27
 # Thanks for your interest.
 
-from .base import PopbillBase,PopbillException
+from .base import PopbillBase, PopbillException
+
 
 class HTTaxinvoiceService(PopbillBase):
     """ 팝빌 홈택스 전자세금계산서 연계 API Service Implementation. """
 
-    def __init__(self,LinkID,SecretKey):
+    def __init__(self, LinkID, SecretKey):
         """ 생성자
             args
                 LinkID : 링크허브에서 발급받은 링크아이디(LinkID)
                 SecretKeye 링크허브에서 발급받은 비밀키(SecretKey)
         """
 
-        super(self.__class__,self).__init__(LinkID,SecretKey)
+        super(self.__class__, self).__init__(LinkID, SecretKey)
         self._addScope("111")
 
-    def getChargeInfo(self, CorpNum, UserID = None):
+    def getChargeInfo(self, CorpNum, UserID=None):
         """ 과금정보 확인
             args
                 CorpNum : 회원 사업자번호
                 UserID : 팝빌 회원아이디
             return
                 과금정보 객체
             raise
                 PopbillException
         """
 
         return self._httpget('/HomeTax/Taxinvoice/ChargeInfo', CorpNum, UserID)
 
-    def requestJob(self, CorpNum, Type, DType, SDate, EDate, UserID = None):
+    def requestJob(self, CorpNum, Type, DType, SDate, EDate, UserID=None):
         """ 수집 요청
             args
                 CorpNum : 팝빌회원 사업자번호
                 Type : 전자세금계산서 유형, SELL-매출, BUY-매입, TRUSTEE-위수탁
                 DType : 일자유형, W-작성일자, I-발행일자, S-전송일자
                 SDate : 시작일자, 표시형식(yyyyMMdd)
                 EDate : 종료일자, 표시형식(yyyyMMdd)
@@ -63,44 +64,45 @@
         uri = '/HomeTax/Taxinvoice/' + Type
         uri += '?DType=' + DType
         uri += '&SDate=' + SDate
         uri += '&EDate=' + EDate
 
         return self._httppost(uri, "", CorpNum, UserID).jobID
 
-    def getJobState(self, CorpNum, JobID, UserID = None):
+    def getJobState(self, CorpNum, JobID, UserID=None):
         """ 수집 상태 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 JobID : 작업아이디
                 UserID : 팝빌회원 아이디
             return
                 수집 상태 정보
             raise
                 PopbillException
         """
         if JobID == None or len(JobID) != 18:
-            raise PopbillException(-99999999,"작업아이디(jobID)가 올바르지 않습니다.")
+            raise PopbillException(-99999999, "작업아이디(jobID)가 올바르지 않습니다.")
 
-        return self._httpget('/HomeTax/Taxinvoice/'+JobID+'/State', CorpNum, UserID)
+        return self._httpget('/HomeTax/Taxinvoice/' + JobID + '/State', CorpNum, UserID)
 
-    def listActiveJob(self, CorpNum, UserID = None):
+    def listActiveJob(self, CorpNum, UserID=None):
         """ 수집 상태 목록 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 수집 상태 정보 목록
             raise
                 PopbillException
         """
 
         return self._httpget('/HomeTax/Taxinvoice/JobList', CorpNum, UserID)
 
-    def search(self, CorpNum, JobID, Type, TaxType, PurposeType, TaxRegIDType, TaxRegIDYN, TaxRegID, Page, PerPage, Order, UserID = None):
+    def search(self, CorpNum, JobID, Type, TaxType, PurposeType, TaxRegIDType, TaxRegIDYN, TaxRegID, Page, PerPage,
+               Order, UserID=None):
         """ 수집 결과 조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 JobID : 작업아이디
                 Type : 문서형태 배열, N-일반전자세금계산서, M-수정전자세금계산서
                 TaxType : 과세형태 배열, T-과세, N-면세, Z-영세
                 PurposeType : 영수/청구, R-영수, C-청구, N-없음
@@ -112,33 +114,33 @@
                 Order : 정렬 방향, D-내림차순, A-오름차순
                 UserID : 팝빌회원 아이디
             return
                 수집 결과 정보
             raise
                 PopbillException
         """
-        if JobID == None or len(JobID) != 18 :
+        if JobID == None or len(JobID) != 18:
             raise PopbillException(-99999999, "작업아이디(jobID)가 올바르지 않습니다.")
 
         uri = '/HomeTax/Taxinvoice/' + JobID
         uri += '?Type=' + ','.join(Type)
         uri += '&TaxType=' + ','.join(TaxType)
         uri += '&PurposeType=' + ','.join(PurposeType)
         uri += '&TaxRegIDType=' + TaxRegIDType
         uri += '&TaxRegID=' + TaxRegID
         uri += '&Page=' + str(Page)
         uri += '&PerPage=' + str(PerPage)
         uri += '&Order=' + Order
 
-        if TaxRegIDYN != '' :
+        if TaxRegIDYN != '':
             uri += '&TaxRegIDYN=' + TaxRegIDYN
 
         return self._httpget(uri, CorpNum, UserID)
 
-    def summary(self, CorpNum, JobID, Type, TaxType, PurposeType, TaxRegIDType, TaxRegIDYN, TaxRegID, UserID = None):
+    def summary(self, CorpNum, JobID, Type, TaxType, PurposeType, TaxRegIDType, TaxRegIDYN, TaxRegID, UserID=None):
         """ 수집 결과 요약정보 조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 JobID : 작업아이디
                 Type : 문서형태 배열, N-일반전자세금계산서, M-수정전자세금계산서
                 TaxType : 과세형태 배열, T-과세, N-면세, Z-영세
                 PurposeType : 영수/청구, R-영수, C-청구, N-없음
@@ -147,102 +149,194 @@
                 TaxRegID : 종사업장번호, 콤마(",")로 구분 하여 구성 ex) '0001,0002'
                 UserID : 팝빌회원 아이디
             return
                 수집 결과 요약정보
             raise
                 PopbillException
         """
-        if JobID == None or len(JobID) != 18 :
+        if JobID == None or len(JobID) != 18:
             raise PopbillException(-99999999, "작업아이디(jobID)가 올바르지 않습니다.")
 
         uri = '/HomeTax/Taxinvoice/' + JobID + '/Summary'
         uri += '?Type=' + ','.join(Type)
         uri += '&TaxType=' + ','.join(TaxType)
         uri += '&PurposeType=' + ','.join(PurposeType)
         uri += '&TaxRegIDType=' + TaxRegIDType
         uri += '&TaxRegID=' + TaxRegID
 
-        if TaxRegIDYN != '' :
+        if TaxRegIDYN != '':
             uri += '&TaxRegIDYN=' + TaxRegIDYN
 
         return self._httpget(uri, CorpNum, UserID)
 
-    def getTaxinvoice(self, CorpNum, NTSConfirmNum, UserID = None):
+    def getTaxinvoice(self, CorpNum, NTSConfirmNum, UserID=None):
         """ 전자세금계산서 상세정보 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 NTSConfirmNum : 국세청 승인번호
                 UserID : 팝빌회원 아이디
             return
                 전자세금계산서 정보객체
             raise
                 PopbillException
         """
-        if NTSConfirmNum == None or len(NTSConfirmNum) != 24 :
+        if NTSConfirmNum == None or len(NTSConfirmNum) != 24:
             raise PopbillException(-99999999, "국세청승인번호(NTSConfirmNum)가 올바르지 않습니다.")
 
         return self._httpget('/HomeTax/Taxinvoice/' + NTSConfirmNum, CorpNum, UserID)
 
-    def getXML(self, CorpNum, NTSConfirmNum, UserID = None):
+    def getXML(self, CorpNum, NTSConfirmNum, UserID=None):
         """ 전자세금계산서 상세정보 확인 - XML
             args
                 CorpNum : 팝빌회원 사업자번호
                 NTSConfirmNum : 국세청 승인번호
                 UserID : 팝빌회원 아이디
             return
                 전자세금계산서 정보객체
             raise
                 PopbillException
         """
-        if NTSConfirmNum == None or len(NTSConfirmNum) != 24 :
+        if NTSConfirmNum == None or len(NTSConfirmNum) != 24:
             raise PopbillException(-99999999, "국세청승인번호(NTSConfirmNum)가 올바르지 않습니다.")
 
         return self._httpget('/HomeTax/Taxinvoice/' + NTSConfirmNum + '?T=xml', CorpNum, UserID)
 
-    def getFlatRatePopUpURL(self, CorpNum, UserID = None):
+    def getFlatRatePopUpURL(self, CorpNum, UserID=None):
         """ 정액제 서비스 신청 URL
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 정액제 서비스 팝업 URL
             raise
                 PopbillException
         """
         return self._httpget('/HomeTax/Taxinvoice?TG=CHRG', CorpNum, UserID).url
 
-    def getCertificatePopUpURL(self, CorpNum, UserID = None):
+    def getCertificatePopUpURL(self, CorpNum, UserID=None):
         """ 홈택스 공인인증서 등록 URL
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 공인인증서 등록 팝업 URL
             raise
                 PopbillException
         """
         return self._httpget('/HomeTax/Taxinvoice?TG=CERT', CorpNum, UserID).url
 
-    def getFlatRateState(self, CorpNum, UserID = None) :
+    def getFlatRateState(self, CorpNum, UserID=None):
         """ 정액제 서비스 상태 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 정액제 서비스 상태 정보
             raise
                 PopbillException
         """
         return self._httpget('/HomeTax/Taxinvoice/Contract', CorpNum, UserID)
 
-    def getCertificateExpireDate(self, CorpNum, UserID = None):
+    def getCertificateExpireDate(self, CorpNum, UserID=None):
         """ 공인인증서 만료일자 확인
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
             return
                 공인인증서 만료일자
             raise
                 PopbillException
         """
 
         return self._httpget('/HomeTax/Taxinvoice/CertInfo', CorpNum, UserID).certificateExpiration
+
+    def getPopUpURL(self, CorpNum, NTSConfirmNum, UserID=None):
+        """ 홈택스 전자세금계산서 보기 팝업 URL
+            args
+                CorpNum : 팝빌회원 사업자번호
+                NTSConfirmNum : 국세청 승인 번호
+                UserID : 팝빌회원 아이디
+            return
+                전자세금계산서 보기 팝업 URL 반환
+            raise
+                PopbillException
+        """
+
+        if NTSConfirmNum == None or len(NTSConfirmNum) != 24:
+            raise PopbillException(-99999999, "국세청승인번호(NTSConfirmNum)가 올바르지 않습니다.")
+
+        return self._httpget('/HomeTax/Taxinvoice/' + NTSConfirmNum + '/PopUp', CorpNum, UserID).url
+
+    def checkCertValidation(self, CorpNum, UserID=None):
+        """ 홈택스 공인인증서 로그인 테스트
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+
+        return self._httpget('/HomeTax/Taxinvoice/CertCheck', CorpNum, UserID)
+
+    def registDeptUser(self, CorpNum, DeptUserID, DeptUserPWD, UserID=None):
+        """ 홈택스 전자세금계산서 부서사용자 계정 등록
+            args
+                CorpNum : 팝빌회원 사업자번호
+                DeptUserID : 홈택스 부서사용자 계정아이디
+                DeptUserPWD : 홈택스 부서사용자 계정비밀번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        if DeptUserID == None or len(DeptUserID) == 0:
+            raise PopbillException(-99999999, "홈택스 부서사용자 계정 아이디가 입력되지 않았습니다.")
+
+        if DeptUserPWD == None or len(DeptUserPWD) == 0:
+            raise PopbillException(-99999999, "홈택스 부서사용자 계정 비밀번호가 입력되지 않았습니다.")
+
+        req = {}
+        req["id"] = DeptUserID
+        req["pwd"] = DeptUserPWD
+
+        postData = self._stringtify(req)
+
+        return self._httppost("/HomeTax/Taxinvoice/DeptUser", postData, CorpNum, UserID)
+
+    def checkDeptUser(self, CorpNum, UserID=None):
+        """ 홈택스 전자세금계산서 부서사용자 등록정보 확인
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        return self._httpget('/HomeTax/Taxinvoice/DeptUser', CorpNum, UserID)
+
+    def checkLoginDeptUser(self, CorpNum, UserID=None):
+        """ 홈택스 전자세금계산서 부서사용자 로그인 테스트
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        return self._httpget('/HomeTax/Taxinvoice/DeptUser/Check', CorpNum, UserID)
+
+    def deleteDeptUser(self, CorpNum, UserID=None):
+        """ 홈택스 전자세금계산서 부서사용자 등록정보 삭제
+            args
+                CorpNum : 팝빌회원 사업자번호
+                UserID : 팝빌회원 아이디
+            return
+                처리결과. consist of code and message
+            raise
+                PopbillException
+        """
+        return self._httppost("/HomeTax/Taxinvoice/DeptUser", "", CorpNum, UserID, "DELETE")
```

### Comparing `popbill-1.8.0/popbill/kakaoService.py` & `popbill-1.9.0/popbill/kakaoService.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,16 @@
             rcvnm=ReceiverName,
             msg=Content,
             altmsg=AltContent)
         )
         return self.sendATS_same(CorpNum, TemplateCode, Sender, "", "", AltSendType, SndDT, KakaoMessages, UserID,
                                  RequestNum)
 
-    def sendATS_multi(self, CorpNum, TemplateCode, Sender, Content, AltContent, AltSendType, SndDT, KakaoMessages, UserID=None,
+    def sendATS_multi(self, CorpNum, TemplateCode, Sender, Content, AltContent, AltSendType, SndDT, KakaoMessages,
+                      UserID=None,
                       RequestNum=None):
         return self.sendATS_same(CorpNum, TemplateCode, Sender, "", "", AltSendType, SndDT, KakaoMessages, UserID,
                                  RequestNum)
 
     def sendATS_same(self, CorpNum, TemplateCode, Sender, Content, AltContent, AltSendType, SndDT, KakaoMessages,
                      UserID=None, RequestNum=None):
         """
@@ -332,29 +333,32 @@
         :return: 알림톡/친구톡 전송내역 및 전송상태
         """
         if RequestNum is None or RequestNum == '':
             raise PopbillException(-99999999, "요청번호가 입력되지 않았습니다.")
 
         return self._httpget('/KakaoTalk/Get/' + RequestNum, CorpNum, UserID)
 
-    def search(self, CorpNum, SDate, EDate, State, Item, ReserveYN, SenderYN, Page, PerPage, Order, UserID):
+    def search(self, CorpNum, SDate, EDate, State, Item, ReserveYN, SenderYN, Page, PerPage, Order, UserID,
+               QString=None):
+
         """
         카카오톡 전송내역 목록을 조회한다.
         - 버튼정보를 확인하는 경우 GetMessages (알림톡/친구톡 전송내역 확인) API 사용
         :param CorpNum: 팝빌팝빌회원 사업자번호
         :param SDate: 시작일자, 표시형식(yyyyMMdd)
         :param EDate: 종료일자, 표시형식(yyyyMMdd)
         :param State: 전송상태 배열 [1-대기, 2-성공, 3-실패, 4-취소]
         :param Item: 검색대상 [SMS-단문, LMS-장문, MMS-포토]
         :param ReserveYN: 예약여부 [0-전체조회, 1-예약전송]
         :param SenderYN: 개인조회 여부 [0-전체조회, 1-개인조회]
         :param Page: 페이지번호
         :param PerPage: 페이지당 목록개수
         :param Order: 정렬방향, [D-내림차순, A-오름차순]
         :param UserID: 팝빌 회원아이디
+        :param QString : 조회 검색어, 수신자명 기재
         :return: 알림톡/친구톡 전송내역 및 전송상태 및 검색결과 조회
         """
 
         if SDate == None or SDate == '':
             raise PopbillException(-99999999, "시작일자가 입력되지 않았습니다.")
 
         if EDate == None or EDate == '':
@@ -367,14 +371,17 @@
         uri += '&Item=' + ','.join(Item)
         uri += '&ReserveYN=' + ReserveYN
         uri += '&SenderYN=' + SenderYN
         uri += '&Page=' + str(Page)
         uri += '&PerPage=' + str(PerPage)
         uri += '&Order=' + Order
 
+        if QString is not None:
+            uri += '&QString=' + QString
+
         return self._httpget(uri, CorpNum, UserID)
 
     def getUnitCost(self, CorpNum, MsgType, UserID=None):
         """
         전송단가 확인
         :param CorpNum: 팝빌회원 사업자번호
         :param MsgType: 카카오톡 유형
```

### Comparing `popbill-1.8.0/popbill/statementService.py` & `popbill-1.9.0/popbill/statementService.py`

 * *Files identical despite different names*

### Comparing `popbill-1.8.0/popbill/closedownService.py` & `popbill-1.9.0/popbill/closedownService.py`

 * *Files identical despite different names*

### Comparing `popbill-1.8.0/popbill/messageService.py` & `popbill-1.9.0/popbill/messageService.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,28 +422,29 @@
                 PopbillException
         """
         if RequestNum == None or RequestNum == '':
             raise PopbillException(-99999999, "요청번호가 입력되지 않았습니다.")
 
         return self._httpget('/Message/Cancel/' + RequestNum, CorpNum, UserID)
 
-    def search(self, CorpNum, SDate, EDate, State, Item, ReserveYN, SenderYN, Page, PerPage, Order, UserID=None):
+    def search(self, CorpNum, SDate, EDate, State, Item, ReserveYN, SenderYN, Page, PerPage, Order, UserID=None, QString=None):
         """ 문자전송 목록조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 SDate : 시작일자, 표시형식(yyyyMMdd)
                 EDate : 종료일자, 표시형식(yyyyMMdd)
                 State : 전송상태 배열, 1-대기, 2-성공, 3-실패, 4-취소
                 Item : 검색대상, SMS-단문, LMS-장문, MMS-포토
                 ReserveYN : 예약여부 0-전체조회, 1-예약전송 조회
                 SenderYN : 개인조회 여부, 0-전체조회, 1-개인조회
                 Page : 페이지번호
                 PerPage : 페이지당 목록개수
                 Order : 정렬방향, D-내림차순, A-오름차순
                 UserID : 팝빌 회원아이디
+                QString : 조회 검색어, 발신자명 또는 수신자명 기재
         """
 
         if SDate == None or SDate == '':
             raise PopbillException(-99999999, "시작일자가 입력되지 않았습니다.")
 
         if EDate == None or EDate == '':
             raise PopbillException(-99999999, "종료일자가 입력되지 않았습니다.")
@@ -455,14 +456,17 @@
         uri += '&Item=' + ','.join(Item)
         uri += '&ReserveYN=' + ReserveYN
         uri += '&SenderYN=' + SenderYN
         uri += '&Page=' + str(Page)
         uri += '&PerPage=' + str(PerPage)
         uri += '&Order=' + Order
 
+        if QString is not None:
+            uri += '&QString=' + QString
+
         return self._httpget(uri, CorpNum, UserID)
 
     def getURL(self, CorpNum, UserID, ToGo):
         """ 문자 관련 팝빌 URL
             args
                 CorpNum : 팝빌회원 사업자번호
                 UserID : 팝빌회원 아이디
```

### Comparing `popbill-1.8.0/popbill/base.py` & `popbill-1.9.0/popbill/base.py`

 * *Files identical despite different names*

### Comparing `popbill-1.8.0/popbill/cashbillService.py` & `popbill-1.9.0/popbill/cashbillService.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,30 +298,31 @@
 
         if MgtKey == None or MgtKey == "":
             raise PopbillException(-99999999, "관리번호가 입력되지 않았습니다.")
 
         return self._httppost('/Cashbill/' + MgtKey, '', CorpNum, UserID, "DELETE")
 
     def search(self, CorpNum, DType, SDate, EDate, State, TradeType, TradeUsage, TaxationType, Page, PerPage, Order,
-               UserID=None, QString=None):
+               UserID=None, QString=None, TradeOpt=None):
         """ 목록 조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 DType : 일자유형, R-등록일자, T-거래일자, I-발행일자 중 택 1
                 SDate : 시작일자, 표시형식(yyyyMMdd)
                 EDate : 종료일자, 표시형식(yyyyMMdd)
                 State : 상태코드 배열, 2,3번째 자리에 와일드카드(*) 사용가능
-                TradeType : 현금영수증 형태 배열, N-일반현금영수증, C-취소현금영수증
-                TradeUsage : 거래용도 배열, P-소득공제용, C-지출증빙용
+                TradeType : 문서형태 배열, N-일반현금영수증, C-취소현금영수증
+                TradeUsage : 거래구분 배열, P-소득공제용, C-지출증빙용
                 TaxationType : 과세형태 배열, T-과세, N-비과세
                 Page : 페이지번호
-                PerPage : 페이지당 목록개수
+                PerPage : 페이지당 검색개수
                 Order : 정렬방향, D-내림차순, A-오름차순
                 UserID : 팝빌 회원아이디
                 QString : 현금영수증 식별번호, 미기재시 전체조회
+                TradeOpt : 거래유형, N-일반, B-도서공연, T-대중교통
         """
 
         if DType == None or DType == '':
             raise PopbillException(-99999999, "일자유형이 입력되지 않았습니다.")
 
         if SDate == None or SDate == '':
             raise PopbillException(-99999999, "시작일자가 입력되지 않았습니다.")
@@ -340,14 +341,17 @@
         uri += '&Page=' + str(Page)
         uri += '&PerPage=' + str(PerPage)
         uri += '&Order=' + Order
 
         if QString is not None:
             uri += '&QString=' + QString
 
+        if TradeOpt is not None:
+            uri += '&TradeOpt=' + ','.join(TradeOpt)
+
         return self._httpget(uri, CorpNum, UserID)
 
     def getInfo(self, CorpNum, MgtKey):
         """ 상태/요약 정보 조회
             args
                 CorpNum : 팝빌회원 사업자번호
                 MgtKey : 문서관리번호
```

### Comparing `popbill-1.8.0/README.rst` & `popbill-1.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ####
 popbill.py
 ####
-popbill 1.8.0
+popbill 1.9.0
 
 팝빌 API for Python.
 
 .. image:: https://api.travis-ci.org/linkhub-sdk/popbill.py.svg?branch=master
         :target: https://travis-ci.org/linkhub-sdk/popbill.py
 
 * requirements
```

