# coap

Constrained Application Protocol (CoAP)

[https://tools.ietf.org/html/rfc7252](https://tools.ietf.org/html/rfc7252)

## coap.version

Attribute | Value
--- | ---
**IE Name** | coap.version
**Tier** | core
**Data Type** | object: version
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | 2-bit unsigned integer. Indicates the CoAP version number.

## coap.type

A 2-bit unsigned integer. Indicates if this message is of type Confirmable (0), Non-confirmable (1), Acknowledgement (2), or Reset (3).

### coap.type.id

Attribute | Value
--- | ---
**IE Name** | coap.type.id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The enumeratiom ID of the CoAP type. A 2-bit unsigned integer.

### coap.type.name

Attribute | Value
--- | ---
**IE Name** | coap.type.name
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The enumeration name of the CoAP type.

## coap.token

### coap.token.size

Attribute | Value
--- | ---
**IE Name** | coap.token.size
**Tier** | core
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | 4-bit unsigned integer. Indicates the length of the variable-length Token field (0-8 bytes). Lengths 9-15 are reserved, MUST NOT be sent, and MUST be processed as a message format error.

### coap.token.value

Attribute | Value
--- | ---
**IE Name** | coap.token.value
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | A variable-length Token value, which can be between 0 and 8 bytes long.

## coap.class

The CoAP Code value is an 8-bit unsigned integer, split into a 3-bit class (most significant bits) and a 5-bit detail (least significant bits), documented as "c.dd" where "c" is a digit from 0 to 7 for the 3-bit subfield and "dd" are two digits from 00 to 31 for the 5-bit subfield.

The class can indicate a request (0), a success response (2), a client error response (4), or a server error response (5). (All other class values are reserved.) As a special case, Code 0.00 indicates an Empty message.

### coap.class.id

Attribute | Value
--- | ---
**IE Name** | coap.class.id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The enumeratiom ID of the CoAP class.

### coap.class.name

Attribute | Value
--- | ---
**IE Name** | coap.class.name
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The enumeratiom name of the CoAP class.

### coap.req.method

The CoAP Code value is an 8-bit unsigned integer, split into a 3-bit class (most significant bits) and a 5-bit detail (least significant bits), documented as "c.dd" where "c" is a digit from 0 to 7 for the 3-bit subfield and "dd" are two digits from 00 to 31 for the 5-bit subfield.

In case of a request, the Code field indicates the Request Method.

#### coap.req.method.id

Attribute | Value
--- | ---
**IE Name** | coap.req.method.id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The enumeratiom ID of the CoAP request method.

#### coap.req.method.name

Attribute | Value
--- | ---
**IE Name** | coap.req.method.name
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The enumeratiom name of the CoAP request method.

### coap.resp.code

The CoAP Code value is an 8-bit unsigned integer, split into a 3-bit class (most significant bits) and a 5-bit detail (least significant bits), documented as "c.dd" where "c" is a digit from 0 to 7 for the 3-bit subfield and "dd" are two digits from 00 to 31 for the 5-bit subfield.

In case of a response, the Code field indicates a Response Code.

#### coap.resp.code.id

Attribute | Value
--- | ---
**IE Name** | coap.resp.code.id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The enumeratiom ID of the CoAP response code.

#### coap.resp.code.name

Attribute | Value
--- | ---
**IE Name** | coap.resp.code.name
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The enumeratiom name of the CoAP response code.

## coap.msg_id

Attribute | Value
--- | ---
**IE Name** | coap.msg_id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | 16-bit unsigned integer in network byte order. Used to detect message duplication and to match messages of type Acknowledgement/Reset to messages of type Confirmable/Non-confirmable.

## coap.options

Attribute | Value
--- | ---
**IE Name** | coap.options
**Tier** | core
**Data Type** | unsigned
**Semantic** | quantity
**Reference** | [RFC 7252, section 5.4: Options](https://tools.ietf.org/html/rfc7252#section-5.4)
**Description** | The quantity of Type-Length-Value (TLV) formatted CoAP Options in the message.

## coap.option

### coap.option.delta

Attribute | Value
--- | ---
**IE Name** | coap.option.delta
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Reference** | [RFC 7252, section 3.1: Option Format](https://tools.ietf.org/html/rfc7252#section-3.1)
**Description** | 4-bit unsigned integer. A value between 0 and 12 indicates the Option Delta.

### coap.option.delta_ext

Attribute | Value
--- | ---
**IE Name** | coap.option.delta_ext
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Reference** | [RFC 7252, section 3.1: Option Format](https://tools.ietf.org/html/rfc7252#section-3.1)
**Description** | Three option delta values are reserved for special constructs: 13: An 8-bit unsigned integer follows the initial byte and Indicates the Option Delta minus 13; 14: A 16-bit unsigned integer follows the initial byte and indicates the Option Delta minus 269; 15: Reserved for the Payload Marker. The resulting Option Delta is used as the difference between the Option Number of this option and that of the previous option (or zero for the first option). In other words, the Option Number is calculated by simply summing the Option Delta values of this and all previous options before it.

### coap.option.size

Attribute | Value
--- | ---
**IE Name** | coap.option.size
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Reference** | [RFC 7252, section 3.1: Option Format](https://tools.ietf.org/html/rfc7252#section-3.1)
**Description** | 4-bit unsigned integer. A value between 0 and 12 indicates the length of the Option Value, in bytes.

### coap.option.size_ext

Attribute | Value
--- | ---
**IE Name** | coap.option.size_ext
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Reference** | [RFC 7252, section 3.1: Option Format](https://tools.ietf.org/html/rfc7252#section-3.1)
**Description** | Three option size values are reserved for special constructs: 13: An 8-bit unsigned integer precedes the Option Value and indicates the Option Length minus 13; 14: A 16-bit unsigned integer in network byte order precedes the Option Value and indicates the Option Length minus 269; 15: Reserved for future use.

### coap.option.value

Attribute | Value
--- | ---
**IE Name** | coap.msg_id
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 3.1: Option Format](https://tools.ietf.org/html/rfc7252#section-3.1)
**Description** | A sequence of exactly Option Length bytes. The length and format of the Option Value depend on the respective option, which MAY define variable-length values.

### coap.option.accept

The CoAP Accept option can be used to indicate which Content-Format is acceptable to the client. If no Accept option is given, the client does not express a preference (thus no default value is assumed). The client prefers the representation returned by the server to be in the Content-Format indicated. The server returns the preferred Content-Format if available. If the preferred Content-Format cannot be returned, then a 4.06 "Not Acceptable" MUST be sent as a response, unless another error code takes precedence for this response.

#### coap.option.accept.id

Attribute | Value
--- | ---
**IE Name** | coap.option.accept.id
**Tier** | common
**Data Type** | unsigned
**Semantic** | identifier
**Reference** |  [RFC 7252, section 5.10.4: Acccept](https://tools.ietf.org/html/rfc7252#section-5.10.4)
**Description** | The enumeratiom ID of the CoAP Accept option.

#### coap.option.accept.name

Attribute | Value
--- | ---
**IE Name** | coap.option.accept.name
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** |  [RFC 7252, section 5.10.4: Acccept](https://tools.ietf.org/html/rfc7252#section-5.10.4)
**Description** | The enumeratiom name of the CoAP Accept option.

### coap.option.content_format

The Content-Format Option indicates the representation format of the message payload. The representation format is given as a numeric Content-Format identifier that is defined in the "CoAP Content-Formats" registry. In the absence of the option, no default value is assumed, i.e., the representation format of any representation message payload is indeterminate.

#### coap.option.content_format.id

Attribute | Value
--- | ---
**IE Name** | coap.option.accept.id
**Tier** | common
**Data Type** | unsigned
**Semantic** | identifier
**Reference** |  [RFC 7252, section 5.10.3: Content-Format](https://tools.ietf.org/html/rfc7252#section-5.10.3)
**Description** | The enumeratiom ID of the CoAP Content-Format option.

#### coap.option.content_format.name

Attribute | Value
--- | ---
**IE Name** | coap.option.accept.name
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** |  [RFC 7252, section 5.10.3: Content-Format](https://tools.ietf.org/html/rfc7252#section-5.10.3)
**Description** | The enumeratiom name of the CoAP Content-Format option.

### coap.option.etag

Attribute | Value
--- | ---
**IE Name** | coap.option.etag
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 5.10.6: ETag](https://tools.ietf.org/html/rfc7252#section-5.10.6)
**Description** | An entity-tag is intended for use as a resource-local identifier for differentiating between representations of the same resource that vary over time. It is generated by the server providing the resource, which may generate it in any number of ways including a version, checksum, hash, or time.

### coap.option.if_match

Attribute | Value
--- | ---
**IE Name** | coap.msg_id
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 5.10.8.1: If-Match](https://tools.ietf.org/html/rfc7252#section-5.10.8.1)
**Description** | The If-Match Option MAY be used to make a request conditional on the current existence or value of an ETag for one or more representations of the target resource.

### coap.option.if_none_match

Attribute | Value
--- | ---
**IE Name** | coap.option.if_none_match
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 5.10.8.2: If-None-Match](https://tools.ietf.org/html/rfc7252#section-5.10.8.2)
**Description** | The If-None-Match Option MAY be used to make a request conditional on the nonexistence of the target resource.

### coap.option.location_path

Attribute | Value
--- | ---
**IE Name** | coap.option.location_path
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 5.10.7: Location-Path and Location-Query](https://tools.ietf.org/html/rfc7252#section-5.10.7)
**Description** | Each Location-Path Option specifies one segment of the absolute path to the resource. The Location-Path and Location-Query Options together indicate a relative URI that consists either of an absolute path, a query string, or both. A combination of these options is included in a 2.01 (Created) response to indicate the location of the resource created as the result of a POST request. The location is resolved relative to the request URI.

### coap.option.location_query

Attribute | Value
--- | ---
**IE Name** | coap.option.location_query
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 5.10.7: Location-Path and Location-Query](https://tools.ietf.org/html/rfc7252#section-5.10.7)
**Description** | Each Location-Query Option specifies one argument parameterizing the resource. The Location-Path and Location-Query Options together indicate a relative URI that consists either of an absolute path, a query string, or both. A combination of these options is included in a 2.01 (Created) response to indicate the location of the resource created as the result of a POST request. The location is resolved relative to the request URI.

### coap.option.max_age

Attribute | Value
--- | ---
**IE Name** | coap.option.max_age
**Tier** | common
**Data Type** | unsigned
**Semantic** | timeticks
**Unit** | seconds
**Reference** | [RFC 7252, section 5.10.5: Max-Age](https://tools.ietf.org/html/rfc7252#section-5.10.5)
**Description** | The Max-Age Option indicates the maximum time a response may be cached before it is considered not fresh.

### coap.option.proxy.uri

Attribute | Value
--- | ---
**IE Name** | coap.option.uri
**Tier** | common
**Data Type** | object: uri
**Reference** | [RFC 7252, section 5.10.2: Proxy-Uri and Proxy-Scheme](https://tools.ietf.org/html/rfc7252#section-5.10.2)
**Description** | The Proxy-Uri Option is used to make a request to a forward-proxy. The forward-proxy is requested to forward the request or service it from a valid cache and return the response. The option value is an absolute-URI.

### coap.option.size1

Attribute | Value
--- | ---
**IE Name** | coap.option.max_age
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Reference** | [RFC 7252, section 5.10.9: Size1](https://tools.ietf.org/html/rfc7252#section-5.10.9)
**Description** | The Size1 option provides size information about the resource representation in a request. The option value is an integer number of bytes.

### coap.option.uri

Attribute | Value
--- | ---
**IE Name** | coap.option.uri
**Tier** | common
**Data Type** | object: uri
**Reference** | [RFC 7252, section 5.10.1: Uri-Host, Uri-Port, Uri-Path, and Uri-Query](https://tools.ietf.org/html/rfc7252#section-5.10.1)
**Description** | The Uri-Host, Uri-Port, Uri-Path, and Uri-Query Options are used to specify the target resource of a request to a CoAP origin server. The options encode the different components of the request URI in a way that no percent-encoding is visible in the option values and that the full URI can be reconstructed at any involved endpoint.

### coap.payload

Attribute | Value
--- | ---
**IE Name** | coap.option.max_age
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7252, section 3: Message Format](https://tools.ietf.org/html/rfc7252#section-3)
**Description** | The optional payload. If present and of non-zero length, it is prefixed by a fixed, one-byte Payload Marker (0xFF), which indicates the end of options and the start of the payload. The payload data extends from after the marker to the end of the UDP datagram, i.e. the Payload Length is calculated from the datagram size.

## Packet Format

```
 0                   1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|Ver| T |  TKL  |      Code     |          Message ID           |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|   Token (if any, TKL bytes) ...                               |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|   Options (if any) ...                                        |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
|1 1 1 1 1 1 1 1|    Payload (if any) ...                       |
+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
```
