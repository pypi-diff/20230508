# Comparing `tmp/proxycurl_py-0.0.21.tar.gz` & `tmp/proxycurl_py-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxycurl_py-0.0.21.tar", max compression
+gzip compressed data, was "proxycurl_py-0.0.22.tar", max compression
```

## Comparing `proxycurl_py-0.0.21.tar` & `proxycurl_py-0.0.22.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    12288 2023-04-28 09:34:40.817506 proxycurl_py-0.0.21/README.md
--rw-r--r--   0        0        0       56 2023-05-04 05:21:19.908702 proxycurl_py-0.0.21/proxycurl_py/asyncio/__init__.py
--rw-r--r--   0        0        0     4709 2023-04-28 09:34:40.820420 proxycurl_py-0.0.21/proxycurl_py/asyncio/base.py
--rw-r--r--   0        0        0    76763 2023-05-04 05:22:51.225402 proxycurl_py-0.0.21/proxycurl_py/asyncio/library.py
--rw-r--r--   0        0        0      283 2023-04-28 09:34:40.820503 proxycurl_py-0.0.21/proxycurl_py/config.py
--rw-r--r--   0        0        0       56 2023-05-04 05:21:19.866110 proxycurl_py-0.0.21/proxycurl_py/gevent/__init__.py
--rw-r--r--   0        0        0     4171 2023-04-28 09:34:40.820623 proxycurl_py-0.0.21/proxycurl_py/gevent/base.py
--rw-r--r--   0        0        0    71316 2023-05-04 05:21:19.887379 proxycurl_py-0.0.21/proxycurl_py/gevent/library.py
--rw-r--r--   0        0        0    14796 2023-05-04 05:21:19.865323 proxycurl_py-0.0.21/proxycurl_py/models.py
--rw-r--r--   0        0        0       56 2023-05-04 05:21:19.888053 proxycurl_py-0.0.21/proxycurl_py/twisted/__init__.py
--rw-r--r--   0        0        0     4995 2023-04-28 09:34:40.820764 proxycurl_py-0.0.21/proxycurl_py/twisted/base.py
--rw-r--r--   0        0        0    71002 2023-05-04 05:21:19.908118 proxycurl_py-0.0.21/proxycurl_py/twisted/library.py
--rw-r--r--   0        0        0      772 2023-05-04 09:36:44.013150 proxycurl_py-0.0.21/pyproject.toml
--rw-r--r--   0        0        0    13208 1970-01-01 00:00:00.000000 proxycurl_py-0.0.21/PKG-INFO
+-rw-r--r--   0        0        0    12288 2023-04-28 09:34:40.817506 proxycurl_py-0.0.22/README.md
+-rw-r--r--   0        0        0       56 2023-05-04 05:21:19.908702 proxycurl_py-0.0.22/proxycurl_py/asyncio/__init__.py
+-rw-r--r--   0        0        0     4709 2023-05-08 04:09:05.681524 proxycurl_py-0.0.22/proxycurl_py/asyncio/base.py
+-rw-r--r--   0        0        0    76579 2023-05-08 04:04:35.633937 proxycurl_py-0.0.22/proxycurl_py/asyncio/library.py
+-rw-r--r--   0        0        0      283 2023-05-08 04:04:53.721304 proxycurl_py-0.0.22/proxycurl_py/config.py
+-rw-r--r--   0        0        0       56 2023-05-04 05:21:19.866110 proxycurl_py-0.0.22/proxycurl_py/gevent/__init__.py
+-rw-r--r--   0        0        0     4171 2023-04-28 09:34:40.820623 proxycurl_py-0.0.22/proxycurl_py/gevent/base.py
+-rw-r--r--   0        0        0    71316 2023-05-04 05:21:19.887379 proxycurl_py-0.0.22/proxycurl_py/gevent/library.py
+-rw-r--r--   0        0        0    14796 2023-05-04 05:21:19.865323 proxycurl_py-0.0.22/proxycurl_py/models.py
+-rw-r--r--   0        0        0       56 2023-05-04 05:21:19.888053 proxycurl_py-0.0.22/proxycurl_py/twisted/__init__.py
+-rw-r--r--   0        0        0     4995 2023-04-28 09:34:40.820764 proxycurl_py-0.0.22/proxycurl_py/twisted/base.py
+-rw-r--r--   0        0        0    71002 2023-05-04 05:21:19.908118 proxycurl_py-0.0.22/proxycurl_py/twisted/library.py
+-rw-r--r--   0        0        0      772 2023-05-08 04:08:51.474619 proxycurl_py-0.0.22/pyproject.toml
+-rw-r--r--   0        0        0    13208 1970-01-01 00:00:00.000000 proxycurl_py-0.0.22/PKG-INFO
```

### Comparing `proxycurl_py-0.0.21/README.md` & `proxycurl_py-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `proxycurl_py-0.0.21/proxycurl_py/asyncio/base.py` & `proxycurl_py-0.0.22/proxycurl_py/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl_py-0.0.21/proxycurl_py/asyncio/library.py` & `proxycurl_py-0.0.22/proxycurl_py/asyncio/library.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         if github_profile_id:
             params['github_profile_id'] = github_profile_id
         if extra:
             params['extra'] = extra
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/v2/linkedin',
+            url='/proxycurl/api/v2/linkedin',
             params=params,
             data={
             },
             result_class=PersonEndpointResponse
         )
         return resp
 
@@ -188,15 +188,15 @@
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
-            please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl-dev/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
+            please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
         :param location: The location of this user.
 
             Name of country, city or state.
         :type location: str
         :param title: Title that user is holding at his/her current job
         :type title: str
@@ -220,15 +220,15 @@
         if title:
             params['title'] = title
         if last_name:
             params['last_name'] = last_name
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/profile/resolve',
+            url='/proxycurl/api/linkedin/profile/resolve',
             params=params,
             data={
             },
             result_class=PersonLookupUrlEnrichResult
         )
         return resp
 
@@ -250,15 +250,15 @@
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
-            please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl-dev/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
+            please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
         :return: An object of Awaitable[:class:`proxycurl.models.ReverseEmailUrlEnrichResult]` or **None** if there is an error.
         :rtype: Awaitable[:class:`proxycurl.models.ReverseEmailUrlEnrichResult]`
         :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
 
         """
 
@@ -266,15 +266,15 @@
         if work_email:
             params['work_email'] = work_email
         if enrich_profile:
             params['enrich_profile'] = enrich_profile
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/profile/resolve/email',
+            url='/proxycurl/api/linkedin/profile/resolve/email',
             params=params,
             data={
             },
             result_class=ReverseEmailUrlEnrichResult
         )
         return resp
 
@@ -314,15 +314,15 @@
         if linkedin_profile_url:
             params['linkedin_profile_url'] = linkedin_profile_url
         if callback_url:
             params['callback_url'] = callback_url
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/profile/email',
+            url='/proxycurl/api/linkedin/profile/email',
             params=params,
             data={
             },
             result_class=ExtractionEmailResult
         )
         return resp
 
@@ -345,15 +345,15 @@
 
         params = {}
         if linkedin_profile_url:
             params['linkedin_profile_url'] = linkedin_profile_url
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/contact-api/personal-contact',
+            url='/proxycurl/api/contact-api/personal-contact',
             params=params,
             data={
             },
             result_class=PDLPhoneNumberResult
         )
         return resp
 
@@ -385,15 +385,15 @@
         if linkedin_profile_url:
             params['linkedin_profile_url'] = linkedin_profile_url
         if email_validation:
             params['email_validation'] = email_validation
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/contact-api/personal-email',
+            url='/proxycurl/api/contact-api/personal-email',
             params=params,
             data={
             },
             result_class=PDLEmailResult
         )
         return resp
 
@@ -402,16 +402,16 @@
         linkedin_person_profile_url: str,
     ) -> Awaitable[ProfilePicture]:
         """Person Profile Picture Endpoint
         
                 Cost: 0 credit / successful request.
         Get the profile picture of a person.
 
-        Profile pictures are served from cached people profiles found within [LinkDB](https://nubela.co/proxycurl-dev/linkdb).
-        If the profile does not exist within [LinkDB](https://nubela.co/proxycurl-dev/linkdb), then the API will return a `404` status code.
+        Profile pictures are served from cached people profiles found within [LinkDB](https://nubela.co/proxycurl/linkdb).
+        If the profile does not exist within [LinkDB](https://nubela.co/proxycurl/linkdb), then the API will return a `404` status code.
         
         :param linkedin_person_profile_url: LinkedIn Profile URL of the person that you are trying to get the profile picture of.
         :type linkedin_person_profile_url: str
         :return: An object of Awaitable[:class:`proxycurl.models.ProfilePicture]` or **None** if there is an error.
         :rtype: Awaitable[:class:`proxycurl.models.ProfilePicture]`
         :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
 
@@ -419,15 +419,15 @@
 
         params = {}
         if linkedin_person_profile_url:
             params['linkedin_person_profile_url'] = linkedin_person_profile_url
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/person/profile-picture',
+            url='/proxycurl/api/linkedin/person/profile-picture',
             params=params,
             data={
             },
             result_class=ProfilePicture
         )
         return resp
 
@@ -452,15 +452,15 @@
         first_name: str = '',
     ) -> Awaitable[PersonSearchResult]:
         """Person Search Endpoint
         
                 Cost: 35 credits / request.
         Search for people that meet a set of criteria within our exhaustive dataset of people profiles.
 
-        This API endpoint is powered by [LinkDB](https://nubela.co/proxycurl-dev/linkdb), our exhaustive dataset of people and company profiles.
+        This API endpoint is powered by [LinkDB](https://nubela.co/proxycurl/linkdb), our exhaustive dataset of people and company profiles.
         
         :param enrich_profiles: Get the full profile data of people returned instead of only their LinkedIn profile URLs.
 
             Each request respond with a streaming response of profiles.
 
             The valid values are:
 
@@ -593,15 +593,15 @@
         if last_name:
             params['last_name'] = last_name
         if first_name:
             params['first_name'] = first_name
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/search/person',
+            url='/proxycurl/api/search/person',
             params=params,
             data={
             },
             result_class=PersonSearchResult
         )
         return resp
 
@@ -627,15 +627,15 @@
         Get structured data of a Company Profile
         
         :param url: URL of the LinkedIn Company Profile to crawl.
 
             URL should be in the format of `https://www.linkedin.com/company/<public_identifier>`
         :type url: str
         :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator.
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl-dev/linkdb).
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb).
             For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
 
             This parameter accepts the following values:
             - `false` (default value) - Will not resolve numerical IDs.
             - `true` - Enable support for Company Profile URLs with numerical IDs.
             Costs an extra `2` credit on top of the base cost of the endpoint.
         :type resolve_numeric_id: str
@@ -691,15 +691,15 @@
         if acquisitions:
             params['acquisitions'] = acquisitions
         if use_cache:
             params['use_cache'] = use_cache
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/company',
+            url='/proxycurl/api/linkedin/company',
             params=params,
             data={
             },
             result_class=LinkedinCompany
         )
         return resp
 
@@ -731,15 +731,15 @@
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
-            please chain this API call with the [Company Profile Endpoint](https://nubela.co/proxycurl-dev/docs#company-api-company-profile-endpoint) with the `use_cache=if-recent` parameter.
+            please chain this API call with the [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
         :return: An object of Awaitable[:class:`proxycurl.models.CompanyUrlEnrichResult]` or **None** if there is an error.
         :rtype: Awaitable[:class:`proxycurl.models.CompanyUrlEnrichResult]`
         :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
 
         """
 
@@ -751,15 +751,15 @@
         if company_name:
             params['company_name'] = company_name
         if enrich_profile:
             params['enrich_profile'] = enrich_profile
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/company/resolve',
+            url='/proxycurl/api/linkedin/company/resolve',
             params=params,
             data={
             },
             result_class=CompanyUrlEnrichResult
         )
         return resp
 
@@ -842,15 +842,15 @@
         if keyword:
             params['keyword'] = keyword
         if search_id:
             params['search_id'] = search_id
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/v2/linkedin/company/job',
+            url='/proxycurl/api/v2/linkedin/company/job',
             params=params,
             data={
             },
             result_class=JobListPage
         )
         return resp
 
@@ -933,15 +933,15 @@
         if keyword:
             params['keyword'] = keyword
         if search_id:
             params['search_id'] = search_id
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/v2/linkedin/company/job/count',
+            url='/proxycurl/api/v2/linkedin/company/job/count',
             params=params,
             data={
             },
             result_class=JobListCount
         )
         return resp
 
@@ -998,15 +998,15 @@
         if linkedin_employee_count:
             params['linkedin_employee_count'] = linkedin_employee_count
         if employment_status:
             params['employment_status'] = employment_status
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/company/employees/count',
+            url='/proxycurl/api/linkedin/company/employees/count',
             params=params,
             data={
             },
             result_class=EmployeeCount
         )
         return resp
 
@@ -1081,15 +1081,15 @@
             * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
             * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
             * `none` - The default value. Do not sort.
 
             If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
         :type sort_by: str
         :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl-dev/linkdb). 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
             For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
 
             This parameter accepts the following values:
             - `false` (default value) - Will not resolve numerical IDs.
             - `true` - Enable support for Company Profile URLs with numerical IDs. 
             Costs an extra `2` credit on top of the base cost of the endpoint.
         :type resolve_numeric_id: str
@@ -1115,15 +1115,15 @@
         if sort_by:
             params['sort_by'] = sort_by
         if resolve_numeric_id:
             params['resolve_numeric_id'] = resolve_numeric_id
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/company/employees',
+            url='/proxycurl/api/linkedin/company/employees',
             params=params,
             data={
             },
             result_class=EmployeeList
         )
         return resp
 
@@ -1137,16 +1137,16 @@
         
                 Cost: 3 credits / successful request.
         Finds the closest (person) profile with a given role in a Company.
         For example, you can use this endpoint to find the "CTO" of "Apple".
         This API endpoint returns only one result that is the closest match.
 
         There is also the [Employee Search Endpoint]
-        (https://nubela.co/proxycurl-dev/docs#company-api-employee-search-api-endpoint)
-         which is powered by [LinkDB](https://nubela.co/proxycurl-dev/linkdb) if you
+        (https://nubela.co/proxycurl/docs#company-api-employee-search-api-endpoint)
+         which is powered by [LinkDB](https://nubela.co/proxycurl/linkdb) if you
          require:
 
         * precision on the target company
         * a list of employees that matches a role (instead of one result).
         
         :param company_name: Name of the company that you are searching for
         :type company_name: str
@@ -1158,15 +1158,15 @@
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
-            please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl-dev/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
+            please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
         :return: An object of Awaitable[:class:`proxycurl.models.RoleSearchErichedResult]` or **None** if there is an error.
         :rtype: Awaitable[:class:`proxycurl.models.RoleSearchErichedResult]`
         :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
 
         """
 
@@ -1176,15 +1176,15 @@
         if role:
             params['role'] = role
         if enrich_profile:
             params['enrich_profile'] = enrich_profile
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/find/company/role',
+            url='/proxycurl/api/find/company/role',
             params=params,
             data={
             },
             result_class=RoleSearchErichedResult
         )
         return resp
 
@@ -1223,15 +1223,15 @@
         if role_personal_email:
             params['role_personal_email'] = role_personal_email
         if role:
             params['role'] = role
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/reveal/company',
+            url='/proxycurl/api/reveal/company',
             params=params,
             data={
             },
             result_class=CompanyReveal
         )
         return resp
 
@@ -1306,15 +1306,15 @@
             * `recently-joined` - Sort employees by their join date. The most recent employee is on the top of the list.
             * `recently-left` - Sort employees by their departure date. The most recent employee who had just left is on the top of this list.
             * `none` - The default value. Do not sort.
 
             If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per employee returned.
         :type sort_by: str
         :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl-dev/linkdb). 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
             For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
 
             This parameter accepts the following values:
             - `false` (default value) - Will not resolve numerical IDs.
             - `true` - Enable support for Company Profile URLs with numerical IDs. 
             Costs an extra `2` credit on top of the base cost of the endpoint.
         :type resolve_numeric_id: str
@@ -1340,15 +1340,15 @@
         if sort_by:
             params['sort_by'] = sort_by
         if resolve_numeric_id:
             params['resolve_numeric_id'] = resolve_numeric_id
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/company/employees',
+            url='/proxycurl/api/linkedin/company/employees',
             params=params,
             data={
             },
             result_class=EmployeeList
         )
         return resp
 
@@ -1361,18 +1361,18 @@
         enrich_profiles: str = '',
         resolve_numeric_id: str = '',
     ) -> Awaitable[EmployeeList]:
         """Employee Search Endpoint
         
                 Cost: 10 credits / successful request.
         Search employees of a target by their job title.
-        This API endpoint is syntactic sugar for the role_search parameter under the [Employee Listing Endpoint](https://nubela.co/proxycurl-dev/docs#company-api-employee-listing-endpoint).
+        This API endpoint is syntactic sugar for the role_search parameter under the [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint).
 
-        Results are limited by data that we have within [LinkDB](https://nubela.co/proxycurl-dev/linkdb).
-        Use [Role Lookup API Endpoint](https://nubela.co/proxycurl-dev/docs#people-api-role-lookup-endpoint) if you need to query for profiles without LinkDB constraints.
+        Results are limited by data that we have within [LinkDB](https://nubela.co/proxycurl/linkdb).
+        Use [Role Lookup API Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint) if you need to query for profiles without LinkDB constraints.
         The drawbacks of the Role Lookup API Endpoint is that it is less precise and can return at most one result per query.
         
         :param keyword_regex: Job title keyword to search for in regular expression format.
         :type keyword_regex: str
         :param linkedin_company_profile_url: LinkedIn Profile URL of the target company.
         :type linkedin_company_profile_url: str
         :param page_size: Tune the maximum results returned per API call.
@@ -1393,15 +1393,15 @@
 
             * `skip` (default): lists employee's profile url
             * `enrich`: lists full profile of employees
 
             Calling this API endpoint with this parameter would add `1` credit per employee returned.
         :type enrich_profiles: str
         :param resolve_numeric_id: Enable support for Company Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl-dev/linkdb). 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
             For example, we will turn `https://www.linkedin.com/company/1234567890` to `https://www.linkedin.com/company/acme-corp` -- for which the API endpoint only supports the latter.
 
             This parameter accepts the following values:
             - `false` (default value) - Will not resolve numerical IDs.
             - `true` - Enable support for Company Profile URLs with numerical IDs. 
             Costs an extra `2` credit on top of the base cost of the endpoint.
         :type resolve_numeric_id: str
@@ -1423,15 +1423,15 @@
         if enrich_profiles:
             params['enrich_profiles'] = enrich_profiles
         if resolve_numeric_id:
             params['resolve_numeric_id'] = resolve_numeric_id
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/company/employee/search',
+            url='/proxycurl/api/linkedin/company/employee/search',
             params=params,
             data={
             },
             result_class=EmployeeList
         )
         return resp
 
@@ -1440,16 +1440,16 @@
         linkedin_company_profile_url: str,
     ) -> Awaitable[ProfilePicture]:
         """Company Profile Picture Endpoint
         
                 Cost: 0 credit / successful request.
         Get the profile picture of a company.
 
-        Profile pictures are served from cached company profiles found within [LinkDB](https://nubela.co/proxycurl-dev/linkdb).
-        If the profile does not exist within [LinkDB](https://nubela.co/proxycurl-dev/linkdb), then the API will return a `404` status code.
+        Profile pictures are served from cached company profiles found within [LinkDB](https://nubela.co/proxycurl/linkdb).
+        If the profile does not exist within [LinkDB](https://nubela.co/proxycurl/linkdb), then the API will return a `404` status code.
         
         :param linkedin_company_profile_url: LinkedIn Profile URL of the company that you are trying to get the profile picture of.
         :type linkedin_company_profile_url: str
         :return: An object of Awaitable[:class:`proxycurl.models.ProfilePicture]` or **None** if there is an error.
         :rtype: Awaitable[:class:`proxycurl.models.ProfilePicture]`
         :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
 
@@ -1457,15 +1457,15 @@
 
         params = {}
         if linkedin_company_profile_url:
             params['linkedin_company_profile_url'] = linkedin_company_profile_url
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/company/profile-picture',
+            url='/proxycurl/api/linkedin/company/profile-picture',
             params=params,
             data={
             },
             result_class=ProfilePicture
         )
         return resp
 
@@ -1479,16 +1479,16 @@
         
                 Cost: 3 credits / successful request.
         Finds the closest (person) profile with a given role in a Company.
         For example, you can use this endpoint to find the "CTO" of "Apple".
         This API endpoint returns only one result that is the closest match.
 
         There is also the [Employee Search Endpoint]
-        (https://nubela.co/proxycurl-dev/docs#company-api-employee-search-api-endpoint)
-         which is powered by [LinkDB](https://nubela.co/proxycurl-dev/linkdb) if you
+        (https://nubela.co/proxycurl/docs#company-api-employee-search-api-endpoint)
+         which is powered by [LinkDB](https://nubela.co/proxycurl/linkdb) if you
          require:
 
         * precision on the target company
         * a list of employees that matches a role (instead of one result).
         
         :param company_name: Name of the company that you are searching for
         :type company_name: str
@@ -1500,15 +1500,15 @@
 
             * `skip` (default): do not enrich the results with cached profile data
             * `enrich`: enriches the result with cached profile data
 
             Calling this API endpoint with this parameter would add 1 credit.
 
             If you require [fresh profile data](https://nubela.co/blog/how-fresh-are-profiles-returned-by-proxycurl-api/),
-            please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl-dev/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
+            please chain this API call with the [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) with the `use_cache=if-recent` parameter.
         :type enrich_profile: str
         :return: An object of Awaitable[:class:`proxycurl.models.RoleSearchErichedResult]` or **None** if there is an error.
         :rtype: Awaitable[:class:`proxycurl.models.RoleSearchErichedResult]`
         :raise ProxycurlException: Every error will raise a :class:`proxycurl.asyncio.ProxycurlException`
 
         """
 
@@ -1518,15 +1518,15 @@
         if role:
             params['role'] = role
         if enrich_profile:
             params['enrich_profile'] = enrich_profile
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/find/company/role',
+            url='/proxycurl/api/find/company/role',
             params=params,
             data={
             },
             result_class=RoleSearchErichedResult
         )
         return resp
 
@@ -1563,15 +1563,15 @@
         if url:
             params['url'] = url
         if use_cache:
             params['use_cache'] = use_cache
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/school',
+            url='/proxycurl/api/linkedin/school',
             params=params,
             data={
             },
             result_class=LinkedinSchool
         )
         return resp
 
@@ -1643,15 +1643,15 @@
             * `recently-matriculated` - Sort students by their matriculation date. Students who had had most recently started school is on the top of the list.
             * `recently-graduated` - Sort students by their graduation date. The most recently graduated student is on the top of this list.
             * `none` - The default value. Do not sort.
 
             If this parameter is supplied with a value other than `none`, will add `50` credits to the base cost of the API endpoint regardless number of results returned. It will also add an additional cost of `10` credits per student returned.
         :type sort_by: str
         :param resolve_numeric_id: Enable support for School Profile URLs with numerical IDs that you most frequently fetch from Sales Navigator. 
-            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl-dev/linkdb). 
+            We achieve this by resolving numerical IDs into vanity IDs with cached company profiles from [LinkDB](https://nubela.co/proxycurl/linkdb). 
             For example, we will turn `https://www.linkedin.com/school/1234567890` to `https://www.linkedin.com/school/acme-corp` -- for which the API endpoint only supports the latter.
 
             This parameter accepts the following values:
             - `false` (default value) - Will not resolve numerical IDs.
             - `true` - Enable support for School Profile URLs with numerical IDs. 
             Costs an extra `2` credit on top of the base cost of the endpoint.
         :type resolve_numeric_id: str
@@ -1677,15 +1677,15 @@
         if sort_by:
             params['sort_by'] = sort_by
         if resolve_numeric_id:
             params['resolve_numeric_id'] = resolve_numeric_id
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/school/students',
+            url='/proxycurl/api/linkedin/school/students',
             params=params,
             data={
             },
             result_class=StudentList
         )
         return resp
 
@@ -1718,15 +1718,15 @@
 
         params = {}
         if url:
             params['url'] = url
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/linkedin/job',
+            url='/proxycurl/api/linkedin/job',
             params=params,
             data={
             },
             result_class=JobProfile
         )
         return resp
 
@@ -1777,14 +1777,14 @@
 
         """
 
         params = {}
 
         resp = await self.linkedin.proxycurl.request(
             method='GET',
-            url='/proxycurl-dev/api/credit-balance',
+            url='/proxycurl/api/credit-balance',
             params=params,
             data={
             },
             result_class=CreditBalance
         )
         return resp
```

### Comparing `proxycurl_py-0.0.21/proxycurl_py/gevent/base.py` & `proxycurl_py-0.0.22/proxycurl_py/gevent/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl_py-0.0.21/proxycurl_py/gevent/library.py` & `proxycurl_py-0.0.22/proxycurl_py/gevent/library.py`

 * *Files identical despite different names*

### Comparing `proxycurl_py-0.0.21/proxycurl_py/models.py` & `proxycurl_py-0.0.22/proxycurl_py/models.py`

 * *Files identical despite different names*

### Comparing `proxycurl_py-0.0.21/proxycurl_py/twisted/base.py` & `proxycurl_py-0.0.22/proxycurl_py/twisted/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl_py-0.0.21/proxycurl_py/twisted/library.py` & `proxycurl_py-0.0.22/proxycurl_py/twisted/library.py`

 * *Files identical despite different names*

### Comparing `proxycurl_py-0.0.21/pyproject.toml` & `proxycurl_py-0.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proxycurl_py"
-version = "0.0.21"
+version = "0.0.22"
 description = ""
 readme = "README.md"
 authors = ["Nubela <tech@nubela.co>"]
 packages = [
     { include = "proxycurl_py"}
 ]
```

### Comparing `proxycurl_py-0.0.21/PKG-INFO` & `proxycurl_py-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxycurl-py
-Version: 0.0.21
+Version: 0.0.22
 Summary: 
 Author: Nubela
 Author-email: tech@nubela.co
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

