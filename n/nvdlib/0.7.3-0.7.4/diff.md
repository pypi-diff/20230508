# Comparing `tmp/nvdlib-0.7.3-py3-none-any.whl.zip` & `tmp/nvdlib-0.7.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12691 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       54 b- defN 23-Mar-27 13:31 nvdlib/__init__.py
+Zip file size: 13297 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       84 b- defN 23-May-08 20:46 nvdlib/__init__.py
 -rw-rw-rw-  2.0 fat     9347 b- defN 23-Mar-27 13:31 nvdlib/classes.py
--rw-rw-rw-  2.0 fat     5782 b- defN 23-Mar-27 14:49 nvdlib/cpe.py
--rw-rw-rw-  2.0 fat    15400 b- defN 23-Mar-27 14:39 nvdlib/cve.py
--rw-rw-rw-  2.0 fat     3588 b- defN 23-Mar-27 14:39 nvdlib/get.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-Mar-29 18:26 nvdlib-0.7.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2952 b- defN 23-Mar-29 18:26 nvdlib-0.7.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-29 18:26 nvdlib-0.7.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Mar-29 18:26 nvdlib-0.7.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      738 b- defN 23-Mar-29 18:26 nvdlib-0.7.3.dist-info/RECORD
-10 files, 39037 bytes uncompressed, 11453 bytes compressed:  70.7%
+-rw-rw-rw-  2.0 fat     8621 b- defN 23-May-08 20:46 nvdlib/cpe.py
+-rw-rw-rw-  2.0 fat    22794 b- defN 23-May-08 20:46 nvdlib/cve.py
+-rw-rw-rw-  2.0 fat     5675 b- defN 23-May-08 20:46 nvdlib/get.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-May-08 20:50 nvdlib-0.7.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2952 b- defN 23-May-08 20:50 nvdlib-0.7.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-08 20:50 nvdlib-0.7.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-May-08 20:50 nvdlib-0.7.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      738 b- defN 23-May-08 20:50 nvdlib-0.7.4.dist-info/RECORD
+10 files, 51387 bytes uncompressed, 12059 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: nvdlib/cve.py
 Comment: 
 
 Filename: nvdlib/get.py
 Comment: 
 
-Filename: nvdlib-0.7.3.dist-info/LICENSE
+Filename: nvdlib-0.7.4.dist-info/LICENSE
 Comment: 
 
-Filename: nvdlib-0.7.3.dist-info/METADATA
+Filename: nvdlib-0.7.4.dist-info/METADATA
 Comment: 
 
-Filename: nvdlib-0.7.3.dist-info/WHEEL
+Filename: nvdlib-0.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: nvdlib-0.7.3.dist-info/top_level.txt
+Filename: nvdlib-0.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: nvdlib-0.7.3.dist-info/RECORD
+Filename: nvdlib-0.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nvdlib/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .cve import searchCVE
-from .cpe import searchCPE
+from .cve import searchCVE, searchCVE_V2
+from .cpe import searchCPE, searchCPE_V2
```

## nvdlib/cpe.py

```diff
@@ -1,14 +1,15 @@
 import datetime
 import urllib.parse
 
 from datetime import datetime
-from .get import __get
+from .get import __get, __get_with_generator
 from .classes import __convert
 
+
 def searchCPE(
         cpeNameId=None,
         cpeMatchString=None,
         keywordExactMatch=None,
         keywordSearch=None,
         lastModStartDate=None,
         lastModEndDate=None,
@@ -52,97 +53,171 @@
     :type verbose: bool   
 
     :param verbose: Prints the URL request for debugging purposes.
     :type verbose: bool
     """
 
 
-    def __buildCPECall(
+
+    # Build the URL for the request
+    parameters, headers = __buildCPECall(
         cpeNameId,
         cpeMatchString,
         keywordExactMatch,
         keywordSearch,
         lastModStartDate,
         lastModEndDate,
         matchCriteriaId,
         limit,
         key,
-        delay):
+        delay)
 
-        parameters = {}
+    # Send the GET request for the JSON and convert to dictionary
+    raw = __get('cpe', headers, parameters, limit, verbose, delay)
+    cpes = []
+    # Generates the CVEs into objects for easy referencing and appends them to self.cves
+    for eachCPE in raw['products']:
+        cpe = __convert('cpe', eachCPE['cpe'])
+        cpes.append(cpe)
+    return cpes
 
-        if cpeNameId:
-            parameters['cpeNameId'] = cpeNameId
 
-        if cpeMatchString:
-            cpeMatchString = urllib.parse.quote_plus(cpeMatchString, encoding='utf-8')
-            parameters['cpeMatchString'] = cpeMatchString
-
-        if keywordExactMatch:
-            if keywordSearch:
-                parameters['keywordExactMatch'] = None
-            else:
-                raise SyntaxError('keywordSearch parameter must be passed if keywordExactMatch is set to True.')
-        
-        if keywordSearch:
-            parameters['keywordSearch'] = keywordSearch
-        
-        if lastModStartDate:
-            if isinstance(lastModStartDate, datetime):
-                date = lastModStartDate.isoformat()
-            elif isinstance(lastModStartDate, str):
-                date = datetime.strptime(lastModStartDate, '%Y-%m-%d %H:%M').isoformat()
-            else:
-                raise SyntaxError('Invalid date syntax: ' + lastModStartDate)
-            parameters['lastModStartDate'] = date.replace('+', '%2B')
-
-        if lastModEndDate:
-            if isinstance(lastModEndDate, datetime):
-                date = lastModEndDate.isoformat()
-            elif isinstance(lastModEndDate, str):
-                date = datetime.strptime(lastModEndDate, '%Y-%m-%d %H:%M').isoformat()
-            else:
-                raise SyntaxError('Invalid date syntax: ' + lastModEndDate)
-            parameters['lastModEndDate'] = date.replace('+', '%2B')
-
-        if matchCriteriaId:
-            parameters['matchCriteriaId'] = matchCriteriaId
-
-        if limit:
-            if limit > 2000 or limit < 1:
-                raise SyntaxError('Limit parameter must be between 1 and 2000')
-            parameters['resultsPerPage'] = limit
+def searchCPE_V2(
+        cpeNameId=None,
+        cpeMatchString=None,
+        keywordExactMatch=None,
+        keywordSearch=None,
+        lastModStartDate=None,
+        lastModEndDate=None,
+        matchCriteriaId=None,
+        limit=None,
+        key=None,
+        delay=None,
+        verbose=None):
+    """Build and send GET request then return list of objects containing a collection of CPEs.
+    
+    :param cpeNameId: Returns a specific CPE record using its UUID. If a correctly formatted UUID is passed but it does not exist, it will return empty results. The UUID is the `cpeNameId` value when searching CPE.
+    :type cpeNameId: str
 
-        if key:
-            headers = {'content-type': 'application/json', 'apiKey': key}
-        else:
-            headers = {'content-type': 'application/json'}
+    :param cpeMatchString: Use a partial CPE name to search for other CPE names. 
+    :type cpeMatchString: str
+
+    :param keywordExactMatch: Searches metadata within CPE title and reference links for an exact match of the phrase or word passed to it. Must be included with `keywordSearch`.
+    :type keywordExactMatch: bool
 
-        if delay and key:
-            if delay < 0.6:
-                raise SyntaxError('Delay parameter must be greater than 0.6 seconds with an API key. NVD API recommends several seconds.')
-        elif delay and not key:
-            raise SyntaxError('Key parameter must be present to define a delay. Requests are delayed 6 seconds without an API key by default.')
+    :param keywordSearch: Returns CPE records where a word or phrase is found in the metadata title or reference links. Space characters act as an `AND` statement.
+    :type keywordSearch: str
 
-        return parameters, headers
+    :param lastModStartDate: CPE last modification start date. Maximum 120 day range. A start and end date is required. All times are in UTC 00:00.
+
+        A datetime object or string can be passed as a date. NVDLib will automatically parse the datetime object into the correct format.
+
+        String Example: '2020-06-28 00:00'
+    :type lastModStartDate: str/datetime obj
+
+    :param lastModEndDate: CPE last modification end date. Maximum 120 day range. Must be included with lastModStartDate.
+        Example: '2020-06-28 00:00'
+    :type lastModEndDate: str/datetime obj
+
+    :param limit: Limits the number of results of the search.
+    :type limit: int
+
+    :param key: NVD API Key. Allows for a request every 0.6 seconds instead of 6 seconds.
+    :type key: str
+
+    :param delay: Can only be used if an API key is provided. The amount of time to sleep in between requests. Must be a value above 0.6 seconds if an API key is present. `delay` is set to 6 seconds if no API key is passed.
+    :type verbose: bool   
+
+    :param verbose: Prints the URL request for debugging purposes.
+    :type verbose: bool
+    """
 
     # Build the URL for the request
     parameters, headers = __buildCPECall(
         cpeNameId,
         cpeMatchString,
         keywordExactMatch,
         keywordSearch,
         lastModStartDate,
         lastModEndDate,
         matchCriteriaId,
         limit,
         key,
         delay)
 
-    # Send the GET request for the JSON and convert to dictionary
-    raw = __get('cpe', headers, parameters, limit, verbose, delay)
-    cpes = []
-    # Generates the CVEs into objects for easy referencing and appends them to self.cves
-    for eachCPE in raw['products']:
-        cpe = __convert('cpe', eachCPE['cpe'])
-        cpes.append(cpe)
-    return cpes
+    # Send the GET request. Get a generator object that returns batched
+    # responses converted to dictionaries
+    for batch in __get_with_generator('cpe', headers, parameters, limit,
+                                      verbose, delay):
+        # Generator object that returns converted CPES
+        for eachCPE in batch['products']:
+            yield __convert('cpe', eachCPE['cpe'])
+
+
+def __buildCPECall(
+    cpeNameId,
+    cpeMatchString,
+    keywordExactMatch,
+    keywordSearch,
+    lastModStartDate,
+    lastModEndDate,
+    matchCriteriaId,
+    limit,
+    key,
+    delay):
+
+    parameters = {}
+
+    if cpeNameId:
+        parameters['cpeNameId'] = cpeNameId
+
+    if cpeMatchString:
+        cpeMatchString = urllib.parse.quote_plus(cpeMatchString, encoding='utf-8')
+        parameters['cpeMatchString'] = cpeMatchString
+
+    if keywordExactMatch:
+        if keywordSearch:
+            parameters['keywordExactMatch'] = None
+        else:
+            raise SyntaxError('keywordSearch parameter must be passed if keywordExactMatch is set to True.')
+    
+    if keywordSearch:
+        parameters['keywordSearch'] = keywordSearch
+    
+    if lastModStartDate:
+        if isinstance(lastModStartDate, datetime):
+            date = lastModStartDate.isoformat()
+        elif isinstance(lastModStartDate, str):
+            date = datetime.strptime(lastModStartDate, '%Y-%m-%d %H:%M').isoformat()
+        else:
+            raise SyntaxError('Invalid date syntax: ' + lastModStartDate)
+        parameters['lastModStartDate'] = date.replace('+', '%2B')
+
+    if lastModEndDate:
+        if isinstance(lastModEndDate, datetime):
+            date = lastModEndDate.isoformat()
+        elif isinstance(lastModEndDate, str):
+            date = datetime.strptime(lastModEndDate, '%Y-%m-%d %H:%M').isoformat()
+        else:
+            raise SyntaxError('Invalid date syntax: ' + lastModEndDate)
+        parameters['lastModEndDate'] = date.replace('+', '%2B')
+
+    if matchCriteriaId:
+        parameters['matchCriteriaId'] = matchCriteriaId
+
+    if limit:
+        if limit > 2000 or limit < 1:
+            raise SyntaxError('Limit parameter must be between 1 and 2000')
+        parameters['resultsPerPage'] = limit
+
+    if key:
+        headers = {'content-type': 'application/json', 'apiKey': key}
+    else:
+        headers = {'content-type': 'application/json'}
+
+    if delay and key:
+        if delay < 0.6:
+            raise SyntaxError('Delay parameter must be greater than 0.6 seconds with an API key. NVD API recommends several seconds.')
+    elif delay and not key:
+        raise SyntaxError('Key parameter must be present to define a delay. Requests are delayed 6 seconds without an API key by default.')
+
+    return parameters, headers
```

## nvdlib/cve.py

```diff
@@ -1,44 +1,44 @@
-import datetime
 import urllib.parse
 
 from datetime import datetime
 from .classes import __convert
-from .get import __get
+from .get import __get, __get_with_generator
+
 
 def searchCVE(
-            cpeName=None,
-            cveId=None,
-            cvssV2Metrics=None,
-            cvssV2Severity=None,
-            cvssV3Metrics=None,
-            cvssV3Severity=None,
-            cweId=None,
-            hasCertAlerts=None,
-            hasCertNotes=None,
-            hasKev=None,
-            hasOval=None,
-            isVulnerable=None,
-            keywordExactMatch=None,
-            keywordSearch=None,
-            lastModStartDate=None,
-            lastModEndDate=None,
-            noRejected=None,
-            pubStartDate=None,
-            pubEndDate=None,
-            sourceIdentifier=None,
-            versionEnd=None,
-            versionEndType=None,
-            versionStart=None,
-            versionStartType=None,
-            virtualMatchString=None,
-            limit=None,
-            delay=None,
-            key=None,
-            verbose=None):
+        cpeName=None,
+        cveId=None,
+        cvssV2Metrics=None,
+        cvssV2Severity=None,
+        cvssV3Metrics=None,
+        cvssV3Severity=None,
+        cweId=None,
+        hasCertAlerts=None,
+        hasCertNotes=None,
+        hasKev=None,
+        hasOval=None,
+        isVulnerable=None,
+        keywordExactMatch=None,
+        keywordSearch=None,
+        lastModStartDate=None,
+        lastModEndDate=None,
+        noRejected=None,
+        pubStartDate=None,
+        pubEndDate=None,
+        sourceIdentifier=None,
+        versionEnd=None,
+        versionEndType=None,
+        versionStart=None,
+        versionStartType=None,
+        virtualMatchString=None,
+        limit=None,
+        delay=None,
+        key=None,
+        verbose=None):
     """Build and send GET request then return list of objects containing a collection of CVEs. For more information on the parameters available, please visit https://nvd.nist.gov/developers/vulnerabilities 
 
     :param cpeName: This value will be compared agains the CPE Match Criteria within a CVE applicability statement. (i.e. find the vulnerabilities attached to that CPE). Partial match strings are allowed.
     :type cpeName: str
 
     :param cveId: Returns a single CVE that already exists in the NVD.
     :type cveId: str
@@ -107,227 +107,402 @@
     :type versionStartType: str
 
     :param virtualMatchString: A more broad filter compared to `cpeName`. The cpe match string that is passed to `virtualMatchString` is compared against the CPE Match Criteria present on CVE applicability statements.
     :type virtualMatchString: str
 
     :param limit: Custom argument to limit the number of results of the search. Allowed any number between 1 and 2000.
     :type limit: int
-    
+
     :param delay: Can only be used if an API key is provided. This allows the user to define a delay. The delay must be greater than 0.6 seconds. The NVD API recommends scripts sleep for atleast 6 seconds in between requests.
     :type delay: int
 
     :param key: NVD API Key. Allows for the user to define a delay. NVD recommends scripts sleep 6 seconds in between requests. If no valid API key is provided, requests are sent with a 6 second delay.
     :type key: str
 
     :param verbose: Prints the URL request for debugging purposes.
     :type verbose: bool    
     """
-    def __buildCVECall(
-            cpeName,
-            cveId,
-            cvssV2Metrics,
-            cvssV2Severity,
-            cvssV3Metrics,
-            cvssV3Severity,
-            cweId,
-            hasCertAlerts,
-            hasCertNotes,
-            hasKev,
-            hasOval,
-            isVulnerable,
-            keywordExactMatch,
-            keywordSearch,
-            lastModStartDate, 
-            lastModEndDate,
-            noRejected,
-            pubStartDate, 
-            pubEndDate, 
-            sourceIdentifier,
-            versionEnd,
-            versionEndType,
-            versionStart,
-            versionStartType,
-            virtualMatchString,
-            limit,
-            delay):
-        
-        parameters = {}
-        
-        if cpeName:
-            cpeName = urllib.parse.quote_plus(cpeName, encoding='utf-8')
-            parameters['cpeName'] = cpeName
 
-        if cveId:
-            parameters['cveId'] = cveId
+    parameters, headers = __buildCVECall(
+        cpeName,
+        cveId,
+        cvssV2Metrics,
+        cvssV2Severity,
+        cvssV3Metrics,
+        cvssV3Severity,
+        cweId,
+        hasCertAlerts,
+        hasCertNotes,
+        hasKev,
+        hasOval,
+        isVulnerable,
+        keywordExactMatch,
+        keywordSearch,
+        lastModStartDate,
+        lastModEndDate,
+        noRejected,
+        pubStartDate,
+        pubEndDate,
+        sourceIdentifier,
+        versionEnd,
+        versionEndType,
+        versionStart,
+        versionStartType,
+        virtualMatchString,
+        limit,
+        delay,
+        key)
 
-        if cvssV2Metrics:
-            cvssV2Metrics = urllib.parse.quote_plus(cvssV2Metrics, encoding='utf-8')
-            parameters['cvssV2Metrics'] = cvssV2Metrics
-
-        if cvssV2Severity:
-            cvssV2Severity = cvssV2Severity.upper()
-            if cvssV2Severity in ['LOW', 'MEDIUM', 'HIGH']:
-                parameters['cvssV2Severity'] = cvssV2Severity
-            else:
-                raise SyntaxError("cvssV2Severity parameter can only be assigned LOW, MEDIUM, or HIGH value.")
+    # raw is the raw dictionary response.
+    raw = __get('cve', headers, parameters, limit, verbose, delay)
+    cves = []
+    # Generates the CVEs into objects for easy access and appends them to self.cves
+    for eachCVE in raw['vulnerabilities']:
+        cves.append(__convert('cve', eachCVE['cve']))
+    return cves
 
-        if cvssV3Metrics:
-            cvssV3Metrics = urllib.parse.quote_plus(cvssV3Metrics, encoding='utf-8')
-            parameters['cvssV3Metrics'] = cvssV3Metrics
-
-        if cvssV3Severity:
-            cvssV3Severity = cvssV3Severity.upper()
-            if cvssV3Severity in ['LOW', 'MEDIUM', 'HIGH', 'CRITICAL']:
-                parameters['cvssV3Severity'] = cvssV3Severity
-            else:
-                raise SyntaxError("cvssV3Severity parameter can only be assigned LOW, MEDIUM, HIGH, or CRITICAL value.")
 
-        if cweId:
-            parameters['cweId'] = cweId.upper()
+def searchCVE_V2(
+        cpeName=None,
+        cveId=None,
+        cvssV2Metrics=None,
+        cvssV2Severity=None,
+        cvssV3Metrics=None,
+        cvssV3Severity=None,
+        cweId=None,
+        hasCertAlerts=None,
+        hasCertNotes=None,
+        hasKev=None,
+        hasOval=None,
+        isVulnerable=None,
+        keywordExactMatch=None,
+        keywordSearch=None,
+        lastModStartDate=None,
+        lastModEndDate=None,
+        noRejected=None,
+        pubStartDate=None,
+        pubEndDate=None,
+        sourceIdentifier=None,
+        versionEnd=None,
+        versionEndType=None,
+        versionStart=None,
+        versionStartType=None,
+        virtualMatchString=None,
+        limit=None,
+        delay=None,
+        key=None,
+        verbose=None):
+    """Build and send GET request then return list of objects containing a collection of CVEs. For more information on the parameters available, please visit https://nvd.nist.gov/developers/vulnerabilities 
 
-        if hasCertAlerts:
-            parameters['hasCertAlerts'] = None
-        
-        if hasCertNotes:
-            parameters['hasCertNotes'] = None        
-
-        if hasKev:
-            parameters['hasKev'] = None
-
-        if hasOval:
-            parameters['hasOval'] = None
-
-        if isVulnerable:
-            if cpeName:
-                parameters['isVulnerable'] = None
-            else:
-                raise SyntaxError('cpeName parameter must be defined if isVulnerable parameter is passed.')
+    :param cpeName: This value will be compared agains the CPE Match Criteria within a CVE applicability statement. (i.e. find the vulnerabilities attached to that CPE). Partial match strings are allowed.
+    :type cpeName: str
 
-        if keywordExactMatch:
-            if keywordSearch:
-                parameters['keywordExactMatch'] = None
-            else:
-                raise SyntaxError('keywordSearch parameter must be passed if keywordExactMatch is set to True.')
+    :param cveId: Returns a single CVE that already exists in the NVD.
+    :type cveId: str
+
+    :param cvssV2Metrics: This parameter returns only the CVEs that match the provided CVSSv2 vector string. Either full or partial vector strings may be used. This parameter cannot be used in requests that include cvssV3Metrics.
+    :type cvssV2Metrics: str
+
+    :param cvssV2Severity: Find vulnerabilities having a 'LOW', 'MEDIUM', or 'HIGH' version 2 severity.
+    :type cvssV2Severity: str
+
+    :param cvssV3Metrics: This parameter returns only the CVEs that match the provided CVSSv3 vector string. Either full or partial vector strings may be used. This parameter cannot be used in requests that include cvssV2Metrics.
+    :type cvssV3Metrics: str
+
+    :param cvssV3Severity: Find vulnerabilities having a 'LOW', 'MEDIUM', 'HIGH', or 'CRITICAL' version 3 severity.
+    :type cvssV3Severity: str
+
+    :param cweId: Filter collection by CWE (Common Weakness Enumeration) ID. You can find a list at https://cwe.mitre.org/. A CVE can have multiple CWE IDs assigned to it.
+    :type cweId: str
+
+    :param hasCertAlerts: Returns CVE that contain a Technical Alert from US-CERT.
+    :type hasCertAlerts: bool
+
+    :param hasCertNotes: Returns CVE that contain a Vulnerability Note from CERT/CC.
+    :type hasCertNotes: bool
+
+    :param hasOval: Returns CVE that contain information from MITRE's Open Vulnerability and Assessment Language (OVAL) before this transitioned to the Center for Internet Security (CIS).
+    :type hasOval: bool
+
+    :param isVulnerable: Returns CVE associated with a specific CPE, where the CPE is also considered vulnerable. **REQUIRES** `cpeName` parameter. `isVulnerable` is not compatible with `virtualMatchString` parameter.
+    :type isVulnerable: bool    
+
+    :param keywordExactMatch: When `keywordSearch` is used along with `keywordExactmatch`, it will search the NVD for CVEs containing exactly what was passed to `keywordSearch`. **REQUIRES** `keywordSearch`.
+    :type keywordExactMatch: bool
+
+    :param keywordSearch: Searches CVEs where a word or phrase is found in the current description. If passing multiple keywords with a space character in between then each word must exist somewhere in the description, not necessarily together unless `keywordExactMatch=True` is passed to `searchCVE`.
+    :type keywordSearch: str
+
+    :param lastModStartDate: These parameters return only the CVEs that were last modified during the specified period. If a CVE has been modified more recently than the specified period, it will not be included in the response. If filtering by the last modified date, both `lastModStartDate` and `lastModEndDate` are REQUIRED. The maximum allowable range when using any date range parameters is 120 consecutive days.
+    :type lastModStartDate: str,datetime obj
+
+    :param lastModEndDate: Required if using lastModStartDate.
+    :type lastModEndDate: str, datetime obj
+
+    :param noRejected: Filters out all CVEs that are in a reject or rejected status. Searches without this parameter include rejected CVEs.
+    :type noRejected: bool
+
+    :param pubStartDate: These parameters return only the CVEs that were added to the NVD (i.e., published) during the specified period. If filtering by the published date, both `pubStartDate` and `pubEndDate` are REQUIRED. The maximum allowable range when using any date range parameters is 120 consecutive days.
+    :type pubStartDate: str,datetime obj
+
+    :param pubEndDate: Required if using pubStartDate.
+    :type pubEndDate: str, datetime obj
 
+    :param sourceIdentifier: Returns CVE where the data source of the CVE is the value that is passed to `sourceIdentifier`.
+    :type sourceIdentifier: str
+
+    :param versionEnd: Must be combined with `versionEndType` and `virtualMatchString`. Returns only the CVEs associated with CPEs in specific version ranges.
+    :type versionEnd: str
+
+    :param versionEndType: Must be combined with `versionEnd` and `virtualMatchString`. Valid values are `including` or `excluding`. Denotes to include the specified version in `versionEnd`, or exclude it.
+    :type versionEndType: str
+
+    :param versionStart: Must be combined with `versionStartType` and `virtualMatchString`. Returns only CVEs with specific versions. Requests that include `versionStart` cannot include a version component in the `virtualMatchString`.
+    :type versionStart: str
+
+    :param versionStartType: Must be combined with `versionStart` and `virtualMatchString`. Valid values are `including` or `excluding`. Denotes to include the specified version in `versionStart`, or exclude it.
+    :type versionStartType: str
+
+    :param virtualMatchString: A more broad filter compared to `cpeName`. The cpe match string that is passed to `virtualMatchString` is compared against the CPE Match Criteria present on CVE applicability statements.
+    :type virtualMatchString: str
+
+    :param limit: Custom argument to limit the number of results of the search. Allowed any number between 1 and 2000.
+    :type limit: int
+
+    :param delay: Can only be used if an API key is provided. This allows the user to define a delay. The delay must be greater than 0.6 seconds. The NVD API recommends scripts sleep for atleast 6 seconds in between requests.
+    :type delay: int
+
+    :param key: NVD API Key. Allows for the user to define a delay. NVD recommends scripts sleep 6 seconds in between requests. If no valid API key is provided, requests are sent with a 6 second delay.
+    :type key: str
+
+    :param verbose: Prints the URL request for debugging purposes.
+    :type verbose: bool    
+    """
+    parameters, headers = __buildCVECall(
+        cpeName,
+        cveId,
+        cvssV2Metrics,
+        cvssV2Severity,
+        cvssV3Metrics,
+        cvssV3Severity,
+        cweId,
+        hasCertAlerts,
+        hasCertNotes,
+        hasKev,
+        hasOval,
+        isVulnerable,
+        keywordExactMatch,
+        keywordSearch,
+        lastModStartDate,
+        lastModEndDate,
+        noRejected,
+        pubStartDate,
+        pubEndDate,
+        sourceIdentifier,
+        versionEnd,
+        versionEndType,
+        versionStart,
+        versionStartType,
+        virtualMatchString,
+        limit,
+        delay,
+        key)
+
+    # Send the GET request. Get a generator object that returns batched
+    # responses converted to dictionaries
+    for batch in __get_with_generator('cve', headers, parameters, limit,
+                                      verbose, delay):
+        for eachCVE in batch['vulnerabilities']:
+            yield __convert('cve', eachCVE['cve'])
+
+
+def __buildCVECall(
+        cpeName,
+        cveId,
+        cvssV2Metrics,
+        cvssV2Severity,
+        cvssV3Metrics,
+        cvssV3Severity,
+        cweId,
+        hasCertAlerts,
+        hasCertNotes,
+        hasKev,
+        hasOval,
+        isVulnerable,
+        keywordExactMatch,
+        keywordSearch,
+        lastModStartDate,
+        lastModEndDate,
+        noRejected,
+        pubStartDate,
+        pubEndDate,
+        sourceIdentifier,
+        versionEnd,
+        versionEndType,
+        versionStart,
+        versionStartType,
+        virtualMatchString,
+        limit,
+        delay,
+        key):
+
+    parameters = {}
+
+    if cpeName:
+        cpeName = urllib.parse.quote_plus(cpeName, encoding='utf-8')
+        parameters['cpeName'] = cpeName
+
+    if cveId:
+        parameters['cveId'] = cveId
+
+    if cvssV2Metrics:
+        cvssV2Metrics = urllib.parse.quote_plus(
+            cvssV2Metrics, encoding='utf-8')
+        parameters['cvssV2Metrics'] = cvssV2Metrics
+
+    if cvssV2Severity:
+        cvssV2Severity = cvssV2Severity.upper()
+        if cvssV2Severity in ['LOW', 'MEDIUM', 'HIGH']:
+            parameters['cvssV2Severity'] = cvssV2Severity
+        else:
+            raise SyntaxError(
+                "cvssV2Severity parameter can only be assigned LOW, MEDIUM, or HIGH value.")
+
+    if cvssV3Metrics:
+        cvssV3Metrics = urllib.parse.quote_plus(
+            cvssV3Metrics, encoding='utf-8')
+        parameters['cvssV3Metrics'] = cvssV3Metrics
+
+    if cvssV3Severity:
+        cvssV3Severity = cvssV3Severity.upper()
+        if cvssV3Severity in ['LOW', 'MEDIUM', 'HIGH', 'CRITICAL']:
+            parameters['cvssV3Severity'] = cvssV3Severity
+        else:
+            raise SyntaxError(
+                "cvssV3Severity parameter can only be assigned LOW, MEDIUM, HIGH, or CRITICAL value.")
+
+    if cweId:
+        parameters['cweId'] = cweId.upper()
+
+    if hasCertAlerts:
+        parameters['hasCertAlerts'] = None
+
+    if hasCertNotes:
+        parameters['hasCertNotes'] = None
+
+    if hasKev:
+        parameters['hasKev'] = None
+
+    if hasOval:
+        parameters['hasOval'] = None
+
+    if isVulnerable:
+        if cpeName:
+            parameters['isVulnerable'] = None
+        else:
+            raise SyntaxError(
+                'cpeName parameter must be defined if isVulnerable parameter is passed.')
+
+    if keywordExactMatch:
         if keywordSearch:
-            parameters['keywordSearch'] = keywordSearch
-        
-        if lastModStartDate:
-            if isinstance(lastModStartDate, datetime):
-                date = lastModStartDate.isoformat()
-            elif isinstance(lastModStartDate, str):
-                date = datetime.strptime(lastModStartDate, '%Y-%m-%d %H:%M').isoformat()
-            else:
-                raise SyntaxError('Invalid date syntax: ' + lastModStartDate)
-            parameters['lastModStartDate'] = date.replace('+', '%2B')
+            parameters['keywordExactMatch'] = None
+        else:
+            raise SyntaxError(
+                'keywordSearch parameter must be passed if keywordExactMatch is set to True.')
 
-        if lastModEndDate:
-            if isinstance(lastModEndDate, datetime):
-                date = lastModEndDate.isoformat()
-            elif isinstance(lastModEndDate, str):
-                date = datetime.strptime(lastModEndDate, '%Y-%m-%d %H:%M').isoformat()
-            else:
-                raise SyntaxError('Invalid date syntax: ' + lastModEndDate)
-            parameters['lastModEndDate'] = date.replace('+', '%2B')
-        
-        if noRejected:
-            parameters['noRejected'] = None
-
-        if pubStartDate:
-            if isinstance(pubStartDate, datetime):
-                date = pubStartDate.isoformat()
-            elif isinstance(pubStartDate, str):
-                date = datetime.strptime(pubStartDate, '%Y-%m-%d %H:%M').isoformat()
-            else:
-                raise SyntaxError('Invalid date syntax: ' + pubEndDate)
-            parameters['pubStartDate'] = date.replace('+', '%2B')
-        
-        if pubEndDate:
-            if isinstance(pubEndDate, datetime):
-                date = pubEndDate.isoformat()
-            elif isinstance(pubEndDate, str):
-                date = datetime.strptime(pubEndDate, '%Y-%m-%d %H:%M').isoformat()
-            else:
-                raise SyntaxError('Invalid date syntax: ' + pubEndDate)
-            parameters['pubEndDate'] = date.replace('+', '%2B')
+    if keywordSearch:
+        parameters['keywordSearch'] = keywordSearch
 
-        if sourceIdentifier:
-            parameters['sourceIdentifier'] = sourceIdentifier
-        
-        if virtualMatchString:
-            virtualMatchString = urllib.parse.quote_plus(virtualMatchString, encoding='utf-8')
-            parameters['virtualMatchString'] = virtualMatchString
-
-        if versionEnd or versionEndType:
-            if versionEnd and versionEndType and virtualMatchString:
-                if versionEndType not in ['including', 'excluding']:
-                    raise SyntaxError('versionEnd parameter must be either "included" or "excluded".')
-                else:
-                    parameters['versionEnd'] = str(versionEnd)
-                    parameters['versionEndType'] = versionEndType
-            else:
-                raise SyntaxError('If versionEnd is used, all three parameters versionEnd, versionEndType, and virtualMatchString are required.')
-        
-        if versionStart or versionStartType:
-            if versionStart and versionStartType and virtualMatchString:
-                if versionStartType not in ['including', 'excluding']:
-                    raise SyntaxError('versionStart parameter must be either "included" or "excluded".')
-                else:
-                    parameters['versionStart'] = str(versionStart)
-                    parameters['versionStartType'] = versionStartType
-            else:
-                raise SyntaxError('If versionStart is used, all three parameters versionStart, versionStartType, and virtualMatchString are required.')       
+    if lastModStartDate:
+        if isinstance(lastModStartDate, datetime):
+            date = lastModStartDate.isoformat()
+        elif isinstance(lastModStartDate, str):
+            date = datetime.strptime(
+                lastModStartDate, '%Y-%m-%d %H:%M').isoformat()
+        else:
+            raise SyntaxError('Invalid date syntax: ' + lastModStartDate)
+        parameters['lastModStartDate'] = date.replace('+', '%2B')
 
-        if limit:
-            if limit > 2000 or limit < 1:
-                raise SyntaxError('Limit parameter must be between 1 and 2000')
-            parameters['resultsPerPage'] = str(limit)
+    if lastModEndDate:
+        if isinstance(lastModEndDate, datetime):
+            date = lastModEndDate.isoformat()
+        elif isinstance(lastModEndDate, str):
+            date = datetime.strptime(
+                lastModEndDate, '%Y-%m-%d %H:%M').isoformat()
+        else:
+            raise SyntaxError('Invalid date syntax: ' + lastModEndDate)
+        parameters['lastModEndDate'] = date.replace('+', '%2B')
+
+    if noRejected:
+        parameters['noRejected'] = None
 
-        if key:
-            headers = {'content-type': 'application/json', 'apiKey': key}
+    if pubStartDate:
+        if isinstance(pubStartDate, datetime):
+            date = pubStartDate.isoformat()
+        elif isinstance(pubStartDate, str):
+            date = datetime.strptime(
+                pubStartDate, '%Y-%m-%d %H:%M').isoformat()
         else:
-            headers = {'content-type': 'application/json'}
+            raise SyntaxError('Invalid date syntax: ' + pubEndDate)
+        parameters['pubStartDate'] = date.replace('+', '%2B')
 
-        if delay and key:
-            if delay < 0.6:
-                raise SyntaxError('Delay parameter must be greater than 0.6 seconds with an API key. NVD API recommends several seconds.')
-        elif delay and not key:
-            raise SyntaxError('Key parameter must be present to define a delay. Requests are delayed 6 seconds without an API key by default.')
+    if pubEndDate:
+        if isinstance(pubEndDate, datetime):
+            date = pubEndDate.isoformat()
+        elif isinstance(pubEndDate, str):
+            date = datetime.strptime(
+                pubEndDate, '%Y-%m-%d %H:%M').isoformat()
+        else:
+            raise SyntaxError('Invalid date syntax: ' + pubEndDate)
+        parameters['pubEndDate'] = date.replace('+', '%2B')
 
-        return parameters, headers
+    if sourceIdentifier:
+        parameters['sourceIdentifier'] = sourceIdentifier
 
-    parameters, headers = __buildCVECall(
-            cpeName,
-            cveId,
-            cvssV2Metrics,
-            cvssV2Severity,
-            cvssV3Metrics,
-            cvssV3Severity,
-            cweId,
-            hasCertAlerts,
-            hasCertNotes,
-            hasKev,
-            hasOval,
-            isVulnerable,
-            keywordExactMatch,
-            keywordSearch,
-            lastModStartDate, 
-            lastModEndDate,
-            noRejected,
-            pubStartDate, 
-            pubEndDate, 
-            sourceIdentifier,
-            versionEnd,
-            versionEndType,
-            versionStart,
-            versionStartType,
-            virtualMatchString,
-            limit,
-            delay)
+    if virtualMatchString:
+        virtualMatchString = urllib.parse.quote_plus(
+            virtualMatchString, encoding='utf-8')
+        parameters['virtualMatchString'] = virtualMatchString
+
+    if versionEnd or versionEndType:
+        if versionEnd and versionEndType and virtualMatchString:
+            if versionEndType not in ['including', 'excluding']:
+                raise SyntaxError(
+                    'versionEnd parameter must be either "included" or "excluded".')
+            else:
+                parameters['versionEnd'] = str(versionEnd)
+                parameters['versionEndType'] = versionEndType
+        else:
+            raise SyntaxError(
+                'If versionEnd is used, all three parameters versionEnd, versionEndType, and virtualMatchString are required.')
 
-    # raw is the raw dictionary response.
-    raw = __get('cve', headers, parameters, limit, verbose, delay)
-    cves = []
-    # Generates the CVEs into objects for easy access and appends them to self.cves
-    for eachCVE in raw['vulnerabilities']:
-        cves.append(__convert('cve', eachCVE['cve']))
-    return cves
+    if versionStart or versionStartType:
+        if versionStart and versionStartType and virtualMatchString:
+            if versionStartType not in ['including', 'excluding']:
+                raise SyntaxError(
+                    'versionStart parameter must be either "included" or "excluded".')
+            else:
+                parameters['versionStart'] = str(versionStart)
+                parameters['versionStartType'] = versionStartType
+        else:
+            raise SyntaxError(
+                'If versionStart is used, all three parameters versionStart, versionStartType, and virtualMatchString are required.')
+
+    if limit:
+        if limit > 2000 or limit < 1:
+            raise SyntaxError('Limit parameter must be between 1 and 2000')
+        parameters['resultsPerPage'] = str(limit)
+
+    if key:
+        headers = {'content-type': 'application/json', 'apiKey': key}
+    else:
+        headers = {'content-type': 'application/json'}
+
+    if delay and key:
+        if delay < 0.6:
+            raise SyntaxError(
+                'Delay parameter must be greater than 0.6 seconds with an API key. NVD API recommends several seconds.')
+    elif delay and not key:
+        raise SyntaxError(
+            'Key parameter must be present to define a delay. Requests are delayed 6 seconds without an API key by default.')
+
+    return parameters, headers
```

## nvdlib/get.py

```diff
@@ -8,69 +8,129 @@
     """Calculate required pages for multiple requests, send the GET request with the search criteria, return list of CVEs or CPEs objects."""
 
     # Get the default 2000 items to see the totalResults and determine pages required.
     if product == 'cve':
         link = 'https://services.nvd.nist.gov/rest/json/cves/2.0?'
     elif product == 'cpe':
         link = 'https://services.nvd.nist.gov/rest/json/cpes/2.0?'
-    
+
     # Requests doesn't really work with dictionary parameters that have no value like `isVulnerable`. The workaround is to just pass a string instead.
     # This joins the parameters into a string with '&' and if a key contains a value then it will join the values with '='
-    stringParams = '&'.join([k if v is None else f"{k}={v}" for k, v in parameters.items()])
+    stringParams = '&'.join(
+        [k if v is None else f"{k}={v}" for k, v in parameters.items()])
     if verbose:
         print('Filter:\n' + link + stringParams)
-    
+
     raw = requests.get(link, params=stringParams, headers=headers, timeout=30)
     raw.encoding = 'utf-8'
     raw.raise_for_status()
 
-    try: # Try to convert the request to JSON. If it is not JSON, then print the response and exit.
-        raw = raw.json() 
+    try:  # Try to convert the request to JSON. If it is not JSON, then print the response and exit.
+        raw = raw.json()
         if 'message' in raw:
             raise LookupError(raw['message'])
     except JSONDecodeError:
         print('Invalid search criteria syntax: ' + str(raw))
         print('Attempted search criteria: ' + str(parameters))
-        
+
     if not delay:
         delay = 6
-    time.sleep(delay) 
-    
+    time.sleep(delay)
+
     # If a limit is in the search criteria or the total number of results are less than or equal to the default 2000 that were just requested, return and don't request anymore.
     totalResults = raw['totalResults']
     if limit or totalResults <= 2000:
         return raw
 
     # If the results is more than the API limit, figure out how many pages there are and calculate the number of requests.
     # Use the page we already grabbed, then send a request starting at startIndex = 2000, then get the next page and ask for 2000 more results at the 2000th index result until all results have been grabbed.
     # Add each ['vulnerabilities'] or ['products'] list from each page to the end of the first request. Effectively creates one data point.
     elif totalResults > 2000:
-        pages = (totalResults // 2000) 
+        pages = (totalResults // 2000)
         startIndex = 2000
         if product == 'cve':
             path = 'vulnerabilities'
         else:
             path = 'products'
 
         rawTemp = raw[path]
 
         for eachPage in range(pages):
             parameters['resultsPerPage'] = '2000'
             parameters['startIndex'] = str(startIndex)
-            stringParams = '&'.join([k if v is None else f"{k}={v}" for k, v in parameters.items()])
+            stringParams = '&'.join(
+                [k if v is None else f"{k}={v}" for k, v in parameters.items()])
             if verbose:
                 print('Filter:\n' + link + stringParams)
             try:
-                getReq = requests.get(link, params=stringParams, headers=headers, timeout=30)
+                getReq = requests.get(
+                    link, params=stringParams, headers=headers, timeout=30)
                 getReq.encoding = 'utf-8'
                 getData = getReq.json()[path]
                 time.sleep(delay)
             except JSONDecodeError:
                 print('JSONDecodeError')
                 print('Something went wrong: ' + str(getReq))
                 print('Attempted search criteria: ' + str(stringParams))
                 print('URL: ' + getReq.request.url)
                 getReq.raise_for_status()
             rawTemp.extend(getData)
             startIndex += 2000
         raw[path] = rawTemp
         return raw
+
+
+def __get_with_generator(product, headers, parameters, limit,
+                         verbose, delay):
+    # Get the default 2000 items to see the totalResults and determine pages required.
+    if product == 'cve':
+        link = 'https://services.nvd.nist.gov/rest/json/cves/2.0?'
+    elif product == 'cpe':
+        link = 'https://services.nvd.nist.gov/rest/json/cpes/2.0?'
+
+    startIndex = 0
+    while True:
+        stringParams = '&'.join(
+            [k if v is None else f"{k}={v}" for k, v in parameters.items()])
+        if verbose:
+            print('Filter:\n' + link + stringParams)
+
+        raw = requests.get(link, params=stringParams,
+                           headers=headers, timeout=30)
+        raw.encoding = 'utf-8'
+        raw.raise_for_status()
+
+        try:  # Try to convert the request to JSON. If it is not JSON, then print the response and exit.
+            raw = raw.json()
+            if 'message' in raw:
+                raise LookupError(raw['message'])
+        except JSONDecodeError:
+            print('Invalid search criteria syntax: ' + str(raw))
+            print('Attempted search criteria: ' + str(parameters))
+        yield raw
+
+        totalResults = raw['totalResults']
+
+        startIndex += 2000
+        parameters['startIndex'] = str(startIndex)
+        parameters['resultsPerPage'] = '2000'
+
+        if verbose and startIndex == 0:
+            if limit:
+                print(f'Query returned {limit} total records')
+            else:
+                print(f'Query returned {totalResults} total records')
+
+        if verbose and not limit:
+            if startIndex < totalResults:
+                print(
+                    f'Getting {product} batch {raw["startIndex"]} to {startIndex}')
+            else:
+                print(
+                    f'Getting {product} batch {raw["startIndex"]} to {totalResults}')
+
+        if limit or startIndex > totalResults:
+            break
+
+        if not delay:
+            delay = 6
+        time.sleep(delay)
```

## Comparing `nvdlib-0.7.3.dist-info/LICENSE` & `nvdlib-0.7.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `nvdlib-0.7.3.dist-info/METADATA` & `nvdlib-0.7.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvdlib
-Version: 0.7.3
+Version: 0.7.4
 Summary: National Vulnerability Database CPE/CVE API Library for Python
 Home-page: https://github.com/Vehemont/nvdlib/
 Author: Vehemont
 Author-email: brad@nvdlib.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >3.7.9
```

