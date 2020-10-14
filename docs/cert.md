# `cert`

## cert.certificate

Attribute | Value
--- | ---
**IE Name** | cert.certificate
**Tier** | 
**Data Type** | octetarray
**Semantic** | x509cert
**Reference** | 
**Description** | 

## cert.hash

Attribute | Value
--- | ---
**IE Name** | cert.hash
**Tier** | 
**Data Type** | octetarray
**Semantic** | default
**Reference** | 
**Description** | 

## cert.md5

Attribute | Value
--- | ---
**IE Name** | cert.md5
**Tier** | 
**Data Type** | octetarray
**Semantic** | default
**Reference** | 
**Description** | 

## cert.sha1

Attribute | Value
--- | ---
**IE Name** | cert.sha1
**Tier** | 
**Data Type** | octetarray
**Semantic** | default
**Reference** | 
**Description** | 

## cert.version

Attribute | Value
--- | ---
**IE Name** | cert.version
**Tier** | 
**Data Type** | object: version
**Reference** | 
**Description** | 

## cert.serial_num

Attribute | Value
--- | ---
**IE Name** | cert.serial_num
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## cert.sign

### cert.sign.algo

#### cert.sign.algo.id

Attribute | Value
--- | ---
**IE Name** | cert.sign.algo.id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | 
**Description** | 

#### cert.sign.algo.name

Attribute | Value
--- | ---
**IE Name** | cert.sign.algo.name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.sign.signature

Attribute | Value
--- | ---
**IE Name** | cert.sign.signature
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## cert.issuer

### cert.issuer.dn

Attribute | Value
--- | ---
**IE Name** | cert.issuer.dn
**Tier** | core
**Data Type** | object: dn
**Reference** | [RFC 4519, section 2.7: distinguishedName](https://tools.ietf.org/html/rfc4519#section-2.7)
**Description** | Distinguished Name. This attribute a base type from which attributes with DN syntax inherit.

## cert.valid

### cert.valid.not_before

Attribute | Value
--- | ---
**IE Name** | cert.valid.not_before
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.valid.not_after

Attribute | Value
--- | ---
**IE Name** | cert.valid.not_after
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## cert.subject

### cert.subject.dn

Attribute | Value
--- | ---
**IE Name** | cert.issuer.dn
**Tier** | core
**Data Type** | object: dn
**Reference** | [RFC 4519, section 2.7: distinguishedName](https://tools.ietf.org/html/rfc4519#section-2.7)
**Description** | Distinguished Name. This attribute a base type from which attributes with DN syntax inherit.

### cert.subject.pub_key

#### cert.subject.pub_key.algo

#### cert.subject.pub_key.algo.id

Attribute | Value
--- | ---
**IE Name** | cert.subject.pub_key.algo.id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | 
**Description** | 

#### cert.subject.pub_key.algo.name

Attribute | Value
--- | ---
**IE Name** | cert.subject.pub_key.algo.name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

#### cert.subject.pub_key.size

Attribute | Value
--- | ---
**IE Name** | cert.subject.pub_key.size
**Tier** | 
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Reference** | 
**Description** | 

#### cert.subject.pub_key.key

Attribute | Value
--- | ---
**IE Name** | cert.subject.pub_key.key
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

#### cert.subject.pub_key.modulus

Attribute | Value
--- | ---
**IE Name** | cert.subject.pub_key.modulus
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

#### cert.subject.pub_key.exponent

Attribute | Value
--- | ---
**IE Name** | cert.subject.pub_key.exponent
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## cert.ext

### cert.ext.alpn

Attribute | Value
--- | ---
**IE Name** | cert.ext.alpn
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.auth_key_id

Attribute | Value
--- | ---
**IE Name** | cert.ext.auth_key_id
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.basic_constraints

Attribute | Value
--- | ---
**IE Name** | cert.ext.basic_constraints
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.cert_policies

Attribute | Value
--- | ---
**IE Name** | cert.ext.cert_policies
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.crl_dist_points

Attribute | Value
--- | ---
**IE Name** | cert.ext.crl_dist_points
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.ext_key_usage

Attribute | Value
--- | ---
**IE Name** | cert.ext.ext_key_usage
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.fresh_crl

Attribute | Value
--- | ---
**IE Name** | cert.ext.fresh_crl
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.inhibit_any_policy

Attribute | Value
--- | ---
**IE Name** | cert.ext.inhibit_any_policy
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.issuer_alt_name

Attribute | Value
--- | ---
**IE Name** | cert.ext.issuer_alt_name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.key_usage

Attribute | Value
--- | ---
**IE Name** | cert.ext.key_usage
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.logotype

Attribute | Value
--- | ---
**IE Name** | cert.ext.logotype
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.name_constraints

Attribute | Value
--- | ---
**IE Name** | cert.ext.name_constraints
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.policy_constraints

Attribute | Value
--- | ---
**IE Name** | cert.ext.policy_constraints
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.policy_maps

Attribute | Value
--- | ---
**IE Name** | cert.ext.policy_maps
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.priv_key_usage_period

Attribute | Value
--- | ---
**IE Name** | cert.ext.priv_key_usage_period
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.subject_alt_name

Attribute | Value
--- | ---
**IE Name** | cert.ext.subject_alt_name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.subject_directory_attr

Attribute | Value
--- | ---
**IE Name** | cert.ext.subject_directory_attr
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.subject_key_id

Attribute | Value
--- | ---
**IE Name** | cert.ext.subject_key_id
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.thumbprint

Attribute | Value
--- | ---
**IE Name** | cert.ext.thumbprint
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.ext.thumbprint_algo

Attribute | Value
--- | ---
**IE Name** | cert.ext.thumbprint_algo
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## cert.pkix

### cert.pkix.auth_info_access

Attribute | Value
--- | ---
**IE Name** | cert.pkix.auth_info_access
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

### cert.pkix.subject_info_access

Attribute | Value
--- | ---
**IE Name** | cert.pkix.subject_info_access
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## Example Certificates

```text
Certificate:
    Data:
        Version: 3 (0x2)
        Serial Number:
            10:e6:fc:62:b7:41:8a:d5:00:5e:45:b6
        Signature Algorithm: sha256WithRSAEncryption
        Issuer: C=BE, O=GlobalSign nv-sa, CN=GlobalSign Organization Validation CA - SHA256 - G2
        Validity
            Not Before: Nov 21 08:00:00 2016 GMT
            Not After : Nov 22 07:59:59 2017 GMT
        Subject: C=US, ST=California, L=San Francisco, O=Wikimedia Foundation, Inc., CN=*.wikipedia.org
        Subject Public Key Info:
            Public Key Algorithm: id-ecPublicKey
                Public-Key: (256 bit)
            pub: 
                    00:c9:22:69:31:8a:d6:6c:ea:da:c3:7f:2c:ac:a5:
                    af:c0:02:ea:81:cb:65:b9:fd:0c:6d:46:5b:c9:1e:
                    9d:3b:ef
                ASN1 OID: prime256v1
                NIST CURVE: P-256
        X509v3 extensions:
            X509v3 Key Usage: critical
                Digital Signature, Key Agreement
            Authority Information Access: 
                CA Issuers - URI:http://secure.globalsign.com/cacert/gsorganizationvalsha2g2r1.crt
                OCSP - URI:http://ocsp2.globalsign.com/gsorganizationvalsha2g2
            X509v3 Certificate Policies: 
                Policy: 1.3.6.1.4.1.4146.1.20
                  CPS: https://www.globalsign.com/repository/
                Policy: 2.23.140.1.2.2
            X509v3 Basic Constraints: 
                CA:FALSE
            X509v3 CRL Distribution Points: 
                Full Name:
                  URI:http://crl.globalsign.com/gs/gsorganizationvalsha2g2.crl
            X509v3 Subject Alternative Name: 
                DNS:*.wikipedia.org, DNS:*.m.mediawiki.org, DNS:*.m.wikibooks.org, DNS:*.m.wikidata.org, DNS:*.m.wikimedia.org, DNS:*.m.wikimediafoundation.org, DNS:*.m.wikinews.org, DNS:*.m.wikipedia.org, DNS:*.m.wikiquote.org, DNS:*.m.wikisource.org, DNS:*.m.wikiversity.org, DNS:*.m.wikivoyage.org, DNS:*.m.wiktionary.org, DNS:*.mediawiki.org, DNS:*.planet.wikimedia.org, DNS:*.wikibooks.org, DNS:*.wikidata.org, DNS:*.wikimedia.org, DNS:*.wikimediafoundation.org, DNS:*.wikinews.org, DNS:*.wikiquote.org, DNS:*.wikisource.org, DNS:*.wikiversity.org, DNS:*.wikivoyage.org, DNS:*.wiktionary.org, DNS:*.wmfusercontent.org, DNS:*.zero.wikipedia.org, DNS:mediawiki.org, DNS:w.wiki, DNS:wikibooks.org, DNS:wikidata.org, DNS:wikimedia.org, DNS:wikimediafoundation.org, DNS:wikinews.org, DNS:wikiquote.org, DNS:wikisource.org, DNS:wikiversity.org, DNS:wikivoyage.org, DNS:wiktionary.org, DNS:wmfusercontent.org, DNS:wikipedia.org
            X509v3 Extended Key Usage: 
                TLS Web Server Authentication, TLS Web Client Authentication
            X509v3 Subject Key Identifier: 
                28:2A:26:2A:57:8B:3B:CE:B4:D6:AB:54:EF:D7:38:21:2C:49:5C:36
            X509v3 Authority Key Identifier: 
                keyid:96:DE:61:F1:BD:1C:16:29:53:1C:C0:CC:7D:3B:83:00:40:E6:1A:7C

    Signature Algorithm: sha256WithRSAEncryption
         8b:c3:ed:d1:9d:39:6f:af:40:72:bd:1e:18:5e:30:54:23:35:
```

```text
Certificate:
    Data:
        Version: 3 (0x2)
        Serial Number:
            04:00:00:00:00:01:44:4e:f0:42:47
        Signature Algorithm: sha256WithRSAEncryption
        Issuer: C=BE, O=GlobalSign nv-sa, OU=Root CA, CN=GlobalSign Root CA
        Validity
            Not Before: Feb 20 10:00:00 2014 GMT
            Not After : Feb 20 10:00:00 2024 GMT
        Subject: C=BE, O=GlobalSign nv-sa, CN=GlobalSign Organization Validation CA - SHA256 - G2
        Subject Public Key Info:
            Public Key Algorithm: rsaEncryption
                Public-Key: (2048 bit)
                Modulus:
                    00:c7:0e:6c:3f:23:93:7f:cc:70:a5:9d:20:c3:0e:
                    ...
                Exponent: 65537 (0x10001)
        X509v3 extensions:
            X509v3 Key Usage: critical
                Certificate Sign, CRL Sign
            X509v3 Basic Constraints: critical
                CA:TRUE, pathlen:0
            X509v3 Subject Key Identifier:
                96:DE:61:F1:BD:1C:16:29:53:1C:C0:CC:7D:3B:83:00:40:E6:1A:7C
            X509v3 Certificate Policies:
                Policy: X509v3 Any Policy
                  CPS: https://www.globalsign.com/repository/

            X509v3 CRL Distribution Points:

                Full Name:
                  URI:http://crl.globalsign.net/root.crl

            Authority Information Access:
                OCSP - URI:http://ocsp.globalsign.com/rootr1

            X509v3 Authority Key Identifier:
                keyid:60:7B:66:1A:45:0D:97:CA:89:50:2F:7D:04:CD:34:A8:FF:FC:FD:4B

    Signature Algorithm: sha256WithRSAEncryption
         46:2a:ee:5e:bd:ae:01:60:37:31:11:86:71:74:b6:46:49:c8:
```

```text
Certificate:[16]
    Data:
        Version: 3 (0x2)
        Serial Number:
            04:00:00:00:00:01:15:4b:5a:c3:94
        Signature Algorithm: sha1WithRSAEncryption
        Issuer: C=BE, O=GlobalSign nv-sa, OU=Root CA, CN=GlobalSign Root CA
        Validity
            Not Before: Sep  1 12:00:00 1998 GMT
            Not After : Jan 28 12:00:00 2028 GMT
        Subject: C=BE, O=GlobalSign nv-sa, OU=Root CA, CN=GlobalSign Root CA
        Subject Public Key Info:
            Public Key Algorithm: rsaEncryption
                Public-Key: (2048 bit)
                Modulus:
                    00:da:0e:e6:99:8d:ce:a3:e3:4f:8a:7e:fb:f1:8b:
                    ...
                Exponent: 65537 (0x10001)
        X509v3 extensions:
            X509v3 Key Usage: critical
                Certificate Sign, CRL Sign
            X509v3 Basic Constraints: critical
                CA:TRUE
            X509v3 Subject Key Identifier:
                60:7B:66:1A:45:0D:97:CA:89:50:2F:7D:04:CD:34:A8:FF:FC:FD:4B
    Signature Algorithm: sha1WithRSAEncryption
         d6:73:e7:7c:4f:76:d0:8d:bf:ec:ba:a2:be:34:c5:28:32:b5:
```