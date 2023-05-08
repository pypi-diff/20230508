# Comparing `tmp/cnert-0.1.5.tar.gz` & `tmp/cnert-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnert-0.1.5.tar", max compression
+gzip compressed data, was "cnert-0.2.0.tar", max compression
```

## Comparing `cnert-0.1.5.tar` & `cnert-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.1.5/LICENSE
--rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.1.5/LICENSE.apache2
--rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.1.5/LICENSE.mit
--rw-r--r--   0        0        0     1126 2023-02-12 23:49:18.672477 cnert-0.1.5/README.md
--rw-r--r--   0        0        0     3135 2023-03-25 20:49:34.835816 cnert-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    20588 2023-03-25 20:49:34.866588 cnert-0.1.5/src/cnert/__init__.py
--rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.1.5/src/cnert/py.typed
--rw-r--r--   0        0        0     2895 1970-01-01 00:00:00.000000 cnert-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      437 2021-12-27 12:15:27.834511 cnert-0.2.0/LICENSE
+-rw-r--r--   0        0        0    10173 2021-12-27 12:15:27.834670 cnert-0.2.0/LICENSE.apache2
+-rw-r--r--   0        0        0     1064 2021-12-27 12:15:27.834799 cnert-0.2.0/LICENSE.mit
+-rw-r--r--   0        0        0     5507 2023-05-08 09:05:48.455941 cnert-0.2.0/README.md
+-rw-r--r--   0        0        0     3126 2023-05-08 09:15:39.345529 cnert-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17684 2023-05-08 09:15:39.375590 cnert-0.2.0/src/cnert/__init__.py
+-rw-r--r--   0        0        0       17 2022-06-21 06:32:36.624012 cnert-0.2.0/src/cnert/py.typed
+-rw-r--r--   0        0        0     7271 1970-01-01 00:00:00.000000 cnert-0.2.0/PKG-INFO
```

### Comparing `cnert-0.1.5/LICENSE.apache2` & `cnert-0.2.0/LICENSE.apache2`

 * *Files identical despite different names*

### Comparing `cnert-0.1.5/LICENSE.mit` & `cnert-0.2.0/LICENSE.mit`

 * *Files identical despite different names*

### Comparing `cnert-0.1.5/pyproject.toml` & `cnert-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cnert"
-version = "0.1.5"
+version = "0.2.0"
 description = "Cnert is trying to be a simple API for creating TLS Certificates testing purposes."
 authors = ["Maarten <ikmaarten@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maartenq/cnert"
 repository = "https://github.com/maartenq/cnert"
 documentation = "https://cnert.readthedocs.io/en/latest/"
 keywords = ["certificate", "X.509", "TLS", "cryptography", "testing"]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: Apache Software License",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
@@ -45,15 +45,15 @@
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 coverage = {extras = ["toml"], version = "^7.1.0"}
 mypy = "^1.0.0"
 pre-commit = "^3.0.4"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
-ruff = "^0.0.259"
+ruff = "^0.0"
 tox = "^4.4.5"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.0.12"
 mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 mkdocs-autorefs = "^0.4.1"
```

### Comparing `cnert-0.1.5/src/cnert/__init__.py` & `cnert-0.2.0/src/cnert/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,243 +1,35 @@
 # cnert/__init__.py
 
 """
 Cnert makes TLS private keys, CSRs, private CAs and certificates.
 """
 
-__version__ = "0.1.5"
+__version__ = "0.2.0"
 __title__ = "Cnert"
 __description__ = (
     "Cnert makes TLS private keys, CSRs, private CAs and certificates."
 )
 __uri__ = "https://github.com/maartenq/cnert"
 __author__ = "Maarten"
 __email__ = "ikmaarten@gmail.com"
 __license__ = "MIT or Apache License, Version 2.0"
 __copyright__ = "Copyright (c) 2021  Maarten"
 
 
 from datetime import datetime, timedelta
+from ipaddress import ip_address, ip_network
+from typing import Optional, Union
 
-# from ipaddress import ip_address, ip_network
-from typing import Optional
-
-# import idna
+import idna
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
-
-#
-# from cryptography.hazmat.primitives import hashes, serialization
-from cryptography.hazmat.primitives import serialization
-
-# from cryptography.hazmat.primitives import serialization
+from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
-
-# from cryptography.x509.oid import ExtendedKeyUsageOID, NameOID
-from cryptography.x509.oid import NameOID
-
-# def _idna_encode(_string: str) -> str:
-#     for prefix in ["*.", "."]:
-#         if _string.startswith(prefix):
-#             _string = _string[len(prefix) :]
-#             _bytes = prefix.encode("ascii") + \
-#                    idna.encode(_string, uts46=True)
-#             return _bytes.decode("ascii")
-#     return idna.encode(_string, uts46=True).decode("ascii")
-
-
-# def _identity_string_to_x509(identity: str) -> x509.GeneralName:
-#     try:
-#         return x509.IPAddress(ip_address(identity))
-#     except ValueError:
-#         try:
-#             return x509.IPAddress(ip_network(identity))
-#         except ValueError:
-#             if "@" in identity:
-#                 return x509.RFC822Name(identity)
-#             return x509.DNSName(_idna_encode(identity))
-
-
-# def _key_usage(
-#     content_commitment: bool = False,
-#     crl_sign: bool = False,
-#     data_encipherment: bool = False,
-#     decipher_only: bool = False,
-#     digital_signature: bool = True,
-#     encipher_only: bool = False,
-#     key_agreement: bool = False,
-#     key_cert_sign: bool = False,
-#     key_encipherment: bool = True,
-# ) -> x509.KeyUsage:
-#     return x509.KeyUsage(
-#         content_commitment=content_commitment,
-#         crl_sign=crl_sign,
-#         data_encipherment=data_encipherment,
-#         decipher_only=decipher_only,
-#         digital_signature=digital_signature,
-#         encipher_only=encipher_only,
-#         key_agreement=key_agreement,
-#         key_cert_sign=key_cert_sign,
-#         key_encipherment=key_encipherment,
-#     )
-
-
-# def _x509_name(**name_attrs: str) -> x509.Name:
-#     """
-#     Takes optional Name Attribute key/values as keyword arguments.
-#     """
-
-#     _DEFAULT_NAME_ATTRS: Dict[str, str] = {
-#         "BUSINESS_CATEGORY:str = "Business Category",
-#         "COMMON_NAME:str = "Common Name",
-#         "COUNTRY_NAME:str = "US",
-#         "DN_QUALIFIER:str = "DN qualifier",
-#         "DOMAIN_COMPONENT:str = "Domain Component",
-#         "EMAIL_ADDRESS:str = "info@example.com",
-#         "GENERATION_QUALIFIER:str = "Generation Qualifier",
-#         "GIVEN_NAME:str = "Given Name",
-#         "INN:str = "INN",
-#         "JURISDICTION_COUNTRY_NAME:str = "US",
-#         "JURISDICTION_LOCALITY_NAME:str = "Jurisdiction Locality Name",
-#         "JURISDICTION_STATE_OR_PROVINCE_NAME": (
-#             "Jurisdiction State or Province Name"
-#         ),
-#         "LOCALITY_NAME:str = "Locality Name",
-#         "OGRN:str = "OGRN",
-#         "ORGANIZATIONAL_UNIT_NAME:str = "Organizational unit_name",
-#         "ORGANIZATION_NAME:str = "Organization Name",
-#         "POSTAL_ADDRESS:str = "Postal Address",
-#         "POSTAL_CODE:str = "Postal Code",
-#         "PSEUDONYM:str = "Pseudonym",
-#         "SERIAL_NUMBER:str = "42",
-#         "SNILS:str = "SNILS",
-#         "STATE_OR_PROVINCE_NAME:str = "State or Province Name",
-#         "STREET_ADDRESS:str = "Street Address",
-#         "SURNAME:str = "Surname",
-#         "TITLE:str = "Title",
-#         "UNSTRUCTURED_NAME:str = "unstructuredName",
-#         "USER_ID:str = "User ID",
-#         "X500_UNIQUE_IDENTIFIER:str = "X500 Unique Identifier",
-#     }
-#     name_attrs = {key.upper(): value for key, value in name_attrs.items()}
-#     if not name_attrs:
-#         name_attrs = _DEFAULT_NAME_ATTRS.copy()
-#     return x509.Name(
-#         [
-#             x509.NameAttribute(getattr(NameOID, key), value)
-#             for (key, value) in name_attrs.items()
-#         ]
-#     )
-
-
-# def _add_ca_extension(
-#     cert_builder: x509.CertificateBuilder,
-# ) -> x509.CertificateBuilder:
-#     return cert_builder.add_extension(
-#         _key_usage(
-#             digital_signature=True,
-#             key_cert_sign=True,
-#             crl_sign=True,
-#         ),
-#         critical=True,
-#     )
-
-
-# def _add_leaf_cert_extensions(
-#     cert_builder: x509.CertificateBuilder,
-# ) -> x509.CertificateBuilder:
-#     return cert_builder.add_extension(
-#         _key_usage(),
-#         critical=True,
-#     ).add_extension(
-#         x509.ExtendedKeyUsage(
-#             [
-#                 ExtendedKeyUsageOID.CLIENT_AUTH,
-#                 ExtendedKeyUsageOID.SERVER_AUTH,
-#                 ExtendedKeyUsageOID.CODE_SIGNING,
-#             ]
-#         ),
-#         critical=True,
-#     )
-
-
-# def _add_subject_alt_name_extension(
-#     cert_builder: x509.CertificateBuilder,
-#     *identities: str,
-# ) -> x509.CertificateBuilder:
-#     return cert_builder.add_extension(
-#         x509.SubjectAlternativeName(
-#             [_identity_string_to_x509(ident) for ident in identities]
-#         ),
-#         critical=True,
-#     )
-
-
-# def _cert_builder(
-#     *identities: str,
-#     subject: x509.Name,
-#     issuer: x509.Name,
-#     public_key: rsa.RSAPublicKey,
-#     not_valid_before: datetime,
-#     not_valid_after: datetime,
-#     serial_number: int = 0,
-#     ca: bool = False,
-#     path_length: Optional[int] = None,
-# ) -> x509.CertificateBuilder:
-#     serial_number = serial_number or x509.random_serial_number()
-#     cert_builder = (
-#         x509.CertificateBuilder()
-#         .subject_name(subject)
-#         .issuer_name(issuer)
-#         .public_key(public_key)
-#         .serial_number(serial_number)
-#         .not_valid_before(not_valid_before)
-#         .not_valid_after(not_valid_after)
-#         .add_extension(
-#             x509.SubjectKeyIdentifier.from_public_key(public_key),
-#             critical=False,
-#         )
-#         .add_extension(
-#             x509.BasicConstraints(ca=ca, path_length=path_length),
-#             critical=True,
-#         )
-#     )
-#     if ca:
-#         cert_builder = _add_ca_extension(cert_builder)
-#     else:
-#         cert_builder = _add_leaf_cert_extensions(cert_builder)
-#     if identities:
-#         cert_builder = _add_subject_alt_name_extension(
-#             cert_builder, *identities
-#         )
-#     return cert_builder
-
-
-# class _Cert:
-#     public_key: rsa.RSAPublicKey
-#     private_key: rsa.RSAPrivateKey
-#
-#     def __init__(
-#         self,
-#         subject_attrs: Dict[str, str],
-#         issuer_attrs: Dict[str, str],
-#         path_length: int,
-#         not_valid_before: datetime,
-#         not_valid_after: datetime,
-#         parent: Optional["_Cert"] = None,
-#     ):
-#         self.subject_attrs = subject_attrs
-#         self.issuer_attrs = issuer_attrs
-#         self.path_length = path_length
-#         self.parent = parent
-#         self.not_valid_before = not_valid_before
-#         self.not_valid_after = not_valid_after
-#         self.private_key = _private_key()
-#         self.public_key = self.private_key.public_key()
-#         self.private_key_pem = _private_key_pem(self.private_key)
+from cryptography.x509.oid import ExtendedKeyUsageOID, NameOID
 
 
 class Freezer:
     """
     Freeze any class such that instantiated objects become immutable.
     """
 
@@ -384,14 +176,147 @@
         return self.x509_name().rfc4514_string()
 
     def __repr__(self) -> str:
         args = ", ".join(f'{x[0]}="{x[1]}"' for x in self.dict_.items())
         return f"NameAttrs({args})"
 
 
+class _CertBuilder:
+    """
+    Builds and signs a X509 Certificate.
+    """
+
+    def __init__(self) -> None:
+        self.builder = x509.CertificateBuilder()
+
+    @staticmethod
+    def _idna_encode(_string: str) -> str:
+        for prefix in ["*.", "."]:
+            if _string.startswith(prefix):
+                _string = _string[len(prefix) :]
+                _bytes = prefix.encode("ascii") + idna.encode(
+                    _string, uts46=True
+                )
+                return _bytes.decode("ascii")
+        return idna.encode(_string, uts46=True).decode("ascii")
+
+    def _identity_string_to_x509(self, identity: str) -> x509.GeneralName:
+        try:
+            return x509.IPAddress(ip_address(identity))
+        except ValueError:
+            try:
+                return x509.IPAddress(ip_network(identity))
+            except ValueError:
+                if "@" in identity:
+                    return x509.RFC822Name(identity)
+                return x509.DNSName(self._idna_encode(identity))
+
+    @staticmethod
+    def _key_usage(
+        content_commitment: bool = False,
+        crl_sign: bool = False,
+        data_encipherment: bool = False,
+        decipher_only: bool = False,
+        digital_signature: bool = True,
+        encipher_only: bool = False,
+        key_agreement: bool = False,
+        key_cert_sign: bool = False,
+        key_encipherment: bool = True,
+    ) -> x509.KeyUsage:
+        return x509.KeyUsage(
+            content_commitment=content_commitment,
+            crl_sign=crl_sign,
+            data_encipherment=data_encipherment,
+            decipher_only=decipher_only,
+            digital_signature=digital_signature,
+            encipher_only=encipher_only,
+            key_agreement=key_agreement,
+            key_cert_sign=key_cert_sign,
+            key_encipherment=key_encipherment,
+        )
+
+    def _add_ca_extension(self) -> None:
+        self.builder = self.builder.add_extension(
+            self._key_usage(
+                digital_signature=True,
+                key_cert_sign=True,
+                crl_sign=True,
+            ),
+            critical=True,
+        )
+
+    def _add_leaf_cert_extension(self) -> None:
+        self.builder = self.builder.add_extension(
+            self._key_usage(),
+            critical=True,
+        ).add_extension(
+            x509.ExtendedKeyUsage(
+                [
+                    ExtendedKeyUsageOID.CLIENT_AUTH,
+                    ExtendedKeyUsageOID.SERVER_AUTH,
+                    ExtendedKeyUsageOID.CODE_SIGNING,
+                ]
+            ),
+            critical=True,
+        )
+
+    def _add_subject_alt_name_extension(self, *sans: str) -> None:
+        self.builder = self.builder.add_extension(
+            x509.SubjectAlternativeName(
+                [self._identity_string_to_x509(san) for san in sans]
+            ),
+            critical=True,
+        )
+
+    def build(
+        self,
+        sans: Union[tuple[()], tuple[str, ...]],
+        subject_attrs_X509_name: x509.Name,
+        issuer_attrs_X509_name: x509.Name,
+        serial_number: int,
+        not_valid_before: datetime,
+        not_valid_after: datetime,
+        is_ca: bool,
+        path_length: Optional[int],
+        public_key: rsa.RSAPublicKey,
+    ) -> None:
+        self.builder = (
+            self.builder.subject_name(subject_attrs_X509_name)
+            .issuer_name(issuer_attrs_X509_name)
+            .public_key(public_key)
+            .serial_number(serial_number)
+            .not_valid_before(not_valid_before)
+            .not_valid_after(not_valid_after)
+            .add_extension(
+                x509.SubjectKeyIdentifier.from_public_key(public_key),
+                critical=False,
+            )
+            .add_extension(
+                x509.BasicConstraints(
+                    ca=is_ca,
+                    path_length=path_length,
+                ),
+                critical=True,
+            )
+        )
+        if is_ca:
+            self._add_ca_extension()
+        else:
+            self._add_leaf_cert_extension()
+        if sans:
+            self._add_subject_alt_name_extension(*sans)
+
+    def sign(self, private_key: rsa.RSAPrivateKey) -> x509.Certificate:
+        return self.builder.sign(
+            private_key=private_key,
+            algorithm=hashes.SHA256(),
+            backend=default_backend(),
+        )
+
+
 class _Cert:
     """
     A _Cert object.
 
     This object is returned by [`cnert.CA().issue_cert()`][cnert.CA.issue_cert]
 
     Examples:
@@ -402,57 +327,118 @@
         NameAttrs(COMMON_NAME="example.com")
         >>> cert.issuer_attrs
         NameAttrs(ORGANIZATION_NAME="Root CA")
         >>> cert.not_valid_before
         datetime.datetime(2023, 3, 24, 23, 56, 55, 901545)
         >>> cert.not_valid_after
         datetime.datetime(2023, 6, 23, 23, 56, 55, 901545)
-
     """
 
     def __init__(
         self,
+        *sans: str,
         subject_attrs: NameAttrs,
         issuer_attrs: NameAttrs,
-        path_length: int = 0,
         not_valid_before: Optional[datetime] = None,
         not_valid_after: Optional[datetime] = None,
+        serial_number: Optional[int] = None,
+        parent: Optional["_Cert"] = None,
+        path_length: int = 0,
+        key_size: int = 2048,
+        is_ca: bool = False,
     ) -> None:
+        """
+        Parameters:
+            sans: Subject Alternative Names as positional arguments
+            subject_attrs: Subject Name Attributes
+            issuer_attrs: Issure Name Attributes
+            not_valid_before: CA not valid before date
+            not_valid_after: CA not valid after date
+            serial_number: Serial number
+            parent: Certificate of CA.
+            path_length: Path length
+            key_size: Key size
+            is_ca: if CA
+
+        """
         if not_valid_before is None:
             not_valid_before = datetime.utcnow()
 
         if not_valid_after is None:
             not_valid_after = not_valid_before + timedelta(weeks=13)
 
+        if serial_number is None:
+            serial_number = x509.random_serial_number()
+
+        self.sans = sans
         self.subject_attrs = subject_attrs
         self.issuer_attrs = issuer_attrs
-        self.path_length = path_length
+        self.parent = parent
         self.not_valid_before = not_valid_before
         self.not_valid_after = not_valid_after
-        (
-            self.private_key,
-            self.public_key,
-            self.private_key_pem,
-        ) = self._gen_private_key()
+        self.serial_number = serial_number
+        self.path_length = path_length
+        self.key_size = key_size
+        self.is_ca = is_ca
+        self._build_private_key(self.key_size)
+        self._build_certificate()
 
-    @staticmethod
-    def _gen_private_key(
-        key_size: int = 2048, public_exponent: int = 65537
-    ) -> tuple[rsa.RSAPrivateKey, rsa.RSAPublicKey, bytes]:
-        key = rsa.generate_private_key(
+    def _build_private_key(
+        self, key_size: int, public_exponent: int = 65537
+    ) -> None:
+        """
+        Parameters:
+            key_size: Key size
+            public_exponent: public exponenent
+        """
+        self.private_key = rsa.generate_private_key(
             public_exponent=public_exponent,
             key_size=key_size,
             backend=default_backend(),
         )
-        pem = key.private_bytes(
+
+    def _build_certificate(self):
+        cert_builder = _CertBuilder()
+        cert_builder.build(
+            self.sans,
+            self.subject_attrs.x509_name(),
+            self.issuer_attrs.x509_name(),
+            self.serial_number,
+            self.not_valid_before,
+            self.not_valid_after,
+            self.is_ca,
+            None if not self.is_ca else self.path_length,
+            self.public_key,
+        )
+        self.certificate = cert_builder.sign(
+            self.parent.private_key if self.parent else self.private_key,
+        )
+        self.public_key_pem = self.certificate.public_bytes(
+            serialization.Encoding.PEM
+        )
+
+    @property
+    def private_key_pem_PKCS1(self) -> bytes:
+        return self.private_key.private_bytes(
             serialization.Encoding.PEM,
             format=serialization.PrivateFormat.TraditionalOpenSSL,
             encryption_algorithm=serialization.NoEncryption(),
         )
-        return (key, key.public_key(), pem)
+
+    @property
+    def private_key_pem(self) -> bytes:
+        return self.private_key.private_bytes(
+            serialization.Encoding.PEM,
+            format=serialization.PrivateFormat.PKCS8,
+            encryption_algorithm=serialization.NoEncryption(),
+        )
+
+    @property
+    def public_key(self) -> rsa.RSAPublicKey:
+        return self.private_key.public_key()
 
     def __str__(self) -> str:
         return f"Certificate {self.subject_attrs}"
 
 
 class CA:
     """
@@ -483,33 +469,32 @@
         not_valid_after: Optional[datetime] = None,
         parent: Optional["CA"] = None,
         intermediate_num: int = 0,
     ) -> None:
         self.intermediate_num = intermediate_num
         self.parent = parent
 
-        # A CA is self signed so it is its own issuer.
-        if self.is_root_ca and subject_attrs != issuer_attrs:
-            raise ValueError(
-                "Can't create CA: issuer attributes must be same "
-                "as subject attributes"
-            )
-
         if subject_attrs is None:
             subject_attrs = NameAttrs(ORGANIZATION_NAME="Root CA")
 
         if issuer_attrs is None:
             issuer_attrs = subject_attrs
 
         self.cert = _Cert(
             subject_attrs=subject_attrs,
             issuer_attrs=issuer_attrs,
             path_length=path_length,
             not_valid_before=not_valid_before,
             not_valid_after=not_valid_after,
+            parent=(
+                self.parent.cert  # type: ignore[has-type]
+                if self.parent is not None
+                else None
+            ),
+            is_ca=True,
         )
 
     def __str__(self) -> str:
         return f"CA {self.cert.subject_attrs}"
 
     @property
     def is_root_ca(self) -> bool:
@@ -555,115 +540,44 @@
             not_valid_after=not_valid_after or self.cert.not_valid_after,
             parent=self,
             intermediate_num=intermediate_num,
         )
 
     def issue_cert(
         self,
+        *sans: str,
         subject_attrs: Optional[NameAttrs] = None,
         not_valid_before: Optional[datetime] = None,
         not_valid_after: Optional[datetime] = None,
     ) -> "_Cert":
         """
         Issues a certificate
 
         Examples:
             >>> ca = CA()
             >>> ca.issue_cert()
             <cnert.Cert at 0x107f87f50>
 
         Parameters:
+            sans: Subject Alternative Names as positional arguments
             subject_attrs: Subject Name Attributes
             not_valid_before: Certificate not valid before date
             not_valid_after: Certificate not valid after date
 
         Returns:
             A _Cert object.
 
         """
 
         if subject_attrs is None:
-            subject_attrs = NameAttrs(COMMON_NAME="example.com")
+            if sans:
+                subject_attrs = NameAttrs(COMMON_NAME=sans[0])
+            else:
+                subject_attrs = NameAttrs(COMMON_NAME="example.com")
         return _Cert(
+            *sans,
             subject_attrs=subject_attrs,
             issuer_attrs=self.cert.subject_attrs,
             not_valid_before=not_valid_before,
             not_valid_after=not_valid_after,
+            parent=self.cert,
         )
-
-    # def create_intermediate(
-    #     self, subject_attrs: Optional[Dict[str, str]] = None
-    # ) -> "CA":
-    #     if subject_attrs is None:
-    #         subject_attrs = {"ORGANIZATION_NAME:str = "Intermediate CA"}
-    #     if self.cert.path_length == 0:
-    #         raise ValueError(
-    #            "Can't create intermediate CA: path length is 0"
-    #           )
-    #     return CA(
-    #         subject_attrs=subject_attrs,
-    #         parent=self.cert,
-    #         path_length=self.cert.path_length - 1,
-    #     )
-
-
-#
-#     def __init__(
-#         self,
-#         subject_attrs: Optional[Dict[str, str]] = None,
-#         parent: Optional[_Cert] = None,
-#         not_valid_before: Optional[datetime] = None,
-#         not_valid_after: Optional[datetime] = None,
-#         path_length: int = 9,
-#     ) -> None:
-#         if subject_attrs is None:
-#             subject_attrs = {"ORGANIZATION_NAME:str = "Root CA"}
-#         now = datetime.utcnow()
-#         issuer_attrs = parent.subject_attrs if parent else subject_attrs
-#
-#         self.cert = _Cert(
-#             subject_attrs=subject_attrs,
-#             issuer_attrs=issuer_attrs,
-#             path_length=path_length,
-#             not_valid_before=not_valid_before or now,
-#             not_valid_after=not_valid_after or now + timedelta(weeks=13),
-#             parent=parent,
-#         )
-#
-#     def issues_cert(self):
-#         pass
-#
-#     def create_intermediate(
-#         self, subject_attrs: Optional[Dict[str, str]] = None
-#     ) -> "CA":
-#         if subject_attrs is None:
-#             subject_attrs = {"ORGANIZATION_NAME:str = "Intermediate CA"}
-#         if self.cert.path_length == 0:
-#             raise ValueError(
-#                "Can't create intermediate CA: path length is 0"
-#               )
-#         return CA(
-#             subject_attrs=subject_attrs,
-#             parent=self.cert,
-#             path_length=self.cert.path_length - 1,
-#         )
-#
-#     def create_cert(
-#         self,
-#         *identities: str,
-#         subject_attrs: Dict[str, str],
-#         not_valid_before: datetime,
-#         not_valid_after: datetime,
-#     ) -> None:
-#         pass
-
-# certificate: x509.Certificate = _cert_builder(
-#     subject=_x509_name(**subject_attrs),
-#     issuer=_x509_name(**self.cert.issuer),
-#     public_key=self.cert.public_key,
-#     not_valid_before=not_valid_before,
-#     not_valid_after=not_valid_after,
-# ).sign(
-#     private_key=self.cert.private_key,
-#     algorithm=hashes.SHA256(),
-#     backend=default_backend(),
-# )
```

