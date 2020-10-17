# tls

tls.version
    The version of the protocol being employed.  This document
    describes TLS Version 1.2, which uses the version { 3, 3 }.  The
    version value 3.3 is historical, deriving from the use of {3, 1}
    for TLS 1.0.  (See Appendix A.1.)  Note that a client that
    supports multiple versions of TLS may not know what version will
    be employed before it receives the ServerHello.  See Appendix E
    for discussion about what record layer version number should be
    employed for ClientHello.

tls.handshake.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.handshake.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.random
tls.sess_id
tls.size
tls.key_size

tls.content_type.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.content_type.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.cipher_suites.size
tls.cipher_suites.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.cipher_suites.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.algo.key_exch
tls.algo.auth
tls.algo.block_cipher
tls.algo.stream_cipher
tls.algo.msg_auth

tls.compress_method.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.compress_method.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.sni
tls.sni_size

tls.ec_curve.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.ec_curve.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.ec_point.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.ec_point.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.ja3

tls.heartbeat.type.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.heartbeat.type.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.heartbeat.mode.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.heartbeat.mode.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.heartbeat.size
tls.heartbeat.payload
tls.heartbeat.payload_size

tls.cert.certificate
tls.cert.hash
tls.cert.md5
tls.cert.sha1

tls.cert.version.ver
tls.cert.serial_num
tls.cert.sign.algo.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.cert.sign.algo.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.cert.sign.signature
tls.cert.issuer. {dn}
tls.cert.issuer.dn  (distiguished name)
tls.cert.issuer.c  (country name)
tls.cert.issuer.cn  (common name)
tls.cert.issuer.dc  (domain component)
tls.cert.issuer.e  (email address)
tls.cert.issuer.l  (locality name)
tls.cert.issuer.o  (organization name)
tls.cert.issuer.ou  (organizational unit)
tls.cert.issuer.pc  (postal code)
tls.cert.issuer.street  (street address)
tls.cert.issuer.st  (state or province)
tls.cert.issuer.uid  (user id)
tls.cert.issuer.unique_id
tls.cert.valid.not_before
tls.cert.valid.not_after
tls.cert.subject.dn  (distiguished name)
tls.cert.subject.c  (country name)
tls.cert.subject.cn  (common name)
tls.cert.subject.dc  (domain component)
tls.cert.subject.e  (email address)
tls.cert.subject.l  (locality name)
tls.cert.subject.o  (organization name)
tls.cert.subject.ou  (organizational unit)
tls.cert.subject.pc  (postal code)
tls.cert.subject.street  (street address)
tls.cert.subject.st  (state or province)
tls.cert.subject.uid  (user id)
tls.cert.subject.algo.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.cert.subject.algo.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.cert.subject.pub_key.algo.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

tls.cert.subject.pub_key.algo.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

tls.cert.subject.pub_key.size
tls.cert.subject.pub_key.key
tls.cert.subject.pub_key.modulus
tls.cert.subject.pub_key.exponent
tls.cert.subject.unique_id

tls.cert.ext.alpn
tls.cert.ext.auth_key_id
tls.cert.ext.basic_constraints
tls.cert.ext.cert_policies
tls.cert.ext.crl_dist_points
tls.cert.ext.ext_key_usage
tls.cert.ext.fresh_crl
tls.cert.ext.inhibit_any_policy
tls.cert.ext.issuer_alt_name
tls.cert.ext.key_usage
tls.cert.ext.logotype
tls.cert.ext.name_constraints
tls.cert.ext.policy_constraints
tls.cert.ext.policy_maps
tls.cert.ext.priv_key_usage_period
tls.cert.ext.subject_alt_name
tls.cert.ext.subject_directory_attr
tls.cert.ext.subject_key_id
tls.cert.ext.thumbprint
tls.cert.ext.thumbprint_algo

tls.cert.pkix.auth_info_access
tls.cert.pkix.subject_info_access
