# http

The `http` object contains information elements related to HTTP messages.

## http.version

Attribute | Value
--- | ---
**IE Name** | http.version
**Tier** | common
**Data Type** | object: version
**Reference** | [RFC 7230, section 2.6: Protocol Versioning](https://tools.ietf.org/html/rfc7230#section-2.6)
**Description** | HTTP request and response messages include an HTTP protocol version using a `<major>.<minor>` numbering scheme.

## http.url

Attribute | Value
--- | ---
**IE Name** | http.url
**Tier** | core
**Data Type** | object: uri
**Reference** | [RFC 7230, section 2.7: Uniform Resource Identifiers](https://tools.ietf.org/html/rfc7230#section-2.7)
**Description** | The complete Uniform Resource Identifiers (URIs). A URI-reference is either a URI or a relative reference.

## http.redir

Attribute | Value
--- | ---
**IE Name** | http.redir
**Tier** | common
**Data Type** | object: uri
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Redirections](https://developer.mozilla.org/en-US/docs/Web/HTTP/Redirections)
**Description** | URL redirection, also known as URL forwarding, is a technique to give more than one URL address to a page, a form, or a whole Web site/application. HTTP has a special kind of response, called a HTTP redirect, for this operation. This IE contains the URL to which to which the client is redirected by the server.

## http.svc.latency

Attribute | Value
--- | ---
**IE Name** | http.svc.latency
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | milliseconds
**Description** | The time elapsed between the observation of an HTTP request from a client and the corresponding HTTP response from the server. If observed from the client application itself this value is the total round-trip time. However this value may be provided by an observer on the network path between the client and server, and would only represent the time from observer to server and back to the observer.

## http.rndtrip.latency

Attribute | Value
--- | ---
**IE Name** | http.rndtrip.latency
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | milliseconds
**Description** | The total round-trip time between when an HTTP request was sent from a client and the corresponding HTTP response was received from the server. By definition the this can only be observed from the client itself.

## http.headers

Attribute | Value
--- | ---
**IE Name** | http.headers
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | values
**Description** | A count of headers in the HTTP request or response message.

## http.gen

A *general header* is an HTTP header that can be used in both request and response messages but doesn't apply to the content itself. Depending on the context they are used in, general headers are either *response* or *request* headers. However, they are not *entity* headers.

### http.gen.cache_control

Attribute | Value
--- | ---
**IE Name** | http.gen.cache_control
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7234, section 5.2: Cache-Control](https://tools.ietf.org/html/rfc7234#section-5.2)
**Description** | The Cache-Control HTTP header holds *directives* (instructions) for caching in both requests and responses. A given directive in a request does not mean the same directive should be in the response.

### http.gen.connection

Attribute | Value
--- | ---
**IE Name** | http.gen.connection
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Connection](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Connection)
**Description** | The Connection general header controls whether or not the network connection stays open after the current transaction finishes. If the value sent is keep-alive, the connection is persistent and not closed, allowing for subsequent requests to the same server to be done.

### http.gen.date

Attribute | Value
--- | ---
**IE Name** | http.gen.date
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Reference** | [RFC 7231, section 7.1.1.2: Date](https://tools.ietf.org/html/rfc7231#section-7.1.1.2)
**Description** | The Date general HTTP header contains the date and time at which the message was originated.

### http.gen.keep_alive

Attribute | Value
--- | ---
**IE Name** | http.gen.keep_alive
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7230, appendix A.1.2: Keep-Alive](https://tools.ietf.org/html/rfc7230#appendix-A.1.2)
**Description** | The Keep-Alive general header allows the sender to hint about how the connection may be used to set a timeout and a maximum amount of requests.

### http.gen.pragma

Attribute | Value
--- | ---
**IE Name** | http.gen.pragma
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7234, section 5.4: Pragma](https://tools.ietf.org/html/rfc7234#section-5.4)
**Description** | The Pragma HTTP/1.0 general header is an implementation-specific header that may have various effects along the request-response chain. It is used for backwards compatibility with HTTP/1.0 caches where the Cache-Control HTTP/1.1 header is not yet present.

### http.gen.upgrade

Attribute | Value
--- | ---
**IE Name** | http.gen.upgrade
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Protocol_upgrade_mechanism](https://developer.mozilla.org/en-US/docs/Web/HTTP/Protocol_upgrade_mechanism)
**Description** | The Upgrade header field is used by clients to invite the server to switch to one of the listed protocols, in descending preference order. The server, if it supports the protocol, replies with the same Upgrade header value as well as Connection: Upgrade. Once this handshake is completed successfully, data transfer begins.

### http.gen.via

Attribute | Value
--- | ---
**IE Name** | http.gen.via
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7230, section 5.7.1: Via](https://tools.ietf.org/html/rfc7230#section-5.7.1)
**Description** | The Via general header is added by proxies, both forward and reverse proxies, and can appear in the request headers and the response headers. It is used for tracking message forwards, avoiding request loops, and identifying the protocol capabilities of senders along the request/response chain.

### http.gen.want_digest

Attribute | Value
--- | ---
**IE Name** | http.gen.want_digest
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 3230, section 4.3.1: Want-Digest](https://tools.ietf.org/html/rfc3230#section-4.3.1)
**Description** | The Want-Digest HTTP header is primarily used in a HTTP request, to ask the responder to provide a digest of the requested resource using the Digest response header.

### http.gen.warning

Attribute | Value
--- | ---
**IE Name** | http.gen.warning
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7234, section 5.5: Warning](https://tools.ietf.org/html/rfc7234#section-5.5)
**Description** | The Warning general HTTP header contains information about possible problems with the status of the message. More than one Warning header may appear in a response.

### http.gen.x_auth_token

Attribute | Value
--- | ---
**IE Name** | http.gen.x_auth_token
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The X-Auth-Token being an unregistered header, it is subject to no formal specification. Its presence and content is always tied to a respective application. A user initially logs in by supplying a username and password. The server returns an access-token in the X-Auth-Token header. For subsequent requests the token is sent by the client in the X-Auth-Token header.

## http.entity

An *entity header* is an HTTP header describing the content of the body of the message. Entity headers are used in both, HTTP *requests* and *responses*.

### http.entity.allow

Attribute | Value
--- | ---
**IE Name** | http.entity.allow
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 7.4.1: Allow](https://tools.ietf.org/html/rfc7231#section-7.4.1)
**Description** | The Allow header lists the set of methods supported by a resource.

### http.entity.content_encoding

Attribute | Value
--- | ---
**IE Name** | http.entity.content_encoding
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 3.1.2.2: Content-Encoding](https://tools.ietf.org/html/rfc7231#section-3.1.2.2)
**Description** | The Content-Encoding entity header is used to compress the media-type. When present, its value indicates which encodings were applied to the entity-body.

### http.entity.content_language

Attribute | Value
--- | ---
**IE Name** | http.entity.content_language
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 3.1.3.2: Content-Language](https://tools.ietf.org/html/rfc7231#section-3.1.3.2)
**Description** | The Content-Language entity header is used to describe the language(s) intended for the audience, so that it allows a user to differentiate according to the users' own preferred language.

### http.entity.content_length

Attribute | Value
--- | ---
**IE Name** | http.entity.content_length
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Reference** | [RFC 7230, section 3.3.2: Content-Length](https://tools.ietf.org/html/rfc7230#section-3.3.2)
**Description** | The Content-Length entity header indicates the size of the entity-body, in bytes, sent to the recipient.

### http.entity.content_location

Attribute | Value
--- | ---
**IE Name** | http.entity.content_location
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 3.1.4.2: Content-Location](https://tools.ietf.org/html/rfc7231#section-3.1.4.2)
**Description** | The Content-Location header indicates an alternate location for the returned data. The principal use is to indicate the URL of a resource transmitted as the result of content negotiation.

### http.entity.content_md5

Attribute | Value
--- | ---
**IE Name** | http.entity.content_md5
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 1864: The Content-MD5 Header Field](https://tools.ietf.org/html/rfc1864)
**Description** | The Content-MD5 entity header is generated by only an originating user agent. Message relays and gateways are expressly forbidden from generating a Content-MD5 field. To generate the value of the Content-MD5 field, the MD5 algorithm is computed on the canonical form of the MIME entity's object.

### http.entity.content_type

Attribute | Value
--- | ---
**IE Name** | http.entity.content_type
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 3.1.1.5: Content-Type](https://tools.ietf.org/html/rfc7231#section-3.1.1.5)
**Description** | The Content-Type entity header is used to indicate the media type of the resource.

### http.entity.delta_base

Attribute | Value
--- | ---
**IE Name** | http.entity.delta_base
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 3229, section 10.5.1: Delta-Base](https://tools.ietf.org/html/rfc3229#section-10.5.1)
**Description** | The Delta-Base entity header is used in a delta-encoded response to specify the entity tag of the base instance. A Delta-Base header field MUST be included in a response with an IM header that includes a delta-coding, if the request included more than one entity tag in its If-None-Match header.

### http.entity.link

Attribute | Value
--- | ---
**IE Name** | http.entity.link
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 8288, section 3: Link Serialisation in HTTP Headers](https://tools.ietf.org/html/rfc8288#section-3)
**Description** | The HTTP Link entity-header field provides a means for serialising one or more links in HTTP headers. It is semantically equivalent to the HTML `<link>` element.

## http.req

Contains *request headers* and additional attributes related to an HTTP request.

A *request header* is an HTTP header that can be used in an HTTP request, and that doesn't relate to the content of the message. Not all headers appearing in a request are *request headers*.

### http.req.datetime

Attribute | Value
--- | ---
**IE Name** | http.req.datetime
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Description** | The timestamp, expressed as an HTTP-date value, when the HTTP request was observed.

### http.req.timestamp

Attribute | Value
--- | ---
**IE Name** | http.req.timestamp
**Tier** | common
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | milliseconds
**Description** | The timestamp, expressed as milliseconds since epoch, when the HTTP request was observed.

### http.req.method

Attribute | Value
--- | ---
**IE Name** | http.req.method
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 4: Request methods](https://tools.ietf.org/html/rfc7231#section-4)
**Description** | The request method token is the primary source of request semantics; it indicates the purpose for which the client has made this request and what is expected by the client as a successful result.

### http.req.bytes

Attribute | Value
--- | ---
**IE Name** | http.req.bytes
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Description** | The size/length of the HTTP request.

### http.req.a_im

Attribute | Value
--- | ---
**IE Name** | http.req.a_im
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 3229, section 10.5.3: A-IM](https://tools.ietf.org/html/rfc3229#section-10.5.3)
**Description** | The A-IM request header is similar to Accept, but restricts the instance-manipulations that are acceptable in the response. A response may be the result of applying multiple instance-manipulations.

### http.req.accept

Attribute | Value
--- | ---
**IE Name** | http.req.accept
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 5.3.2: Accept](https://tools.ietf.org/html/rfc7231#section-5.3.2)
**Description** | The Accept request header advertises which content types, expressed as MIME types, the client is able to understand.

### http.req.accept_charset

Attribute | Value
--- | ---
**IE Name** | http.req.accept_charset
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 5.3.3: Accept-Charset](https://tools.ietf.org/html/rfc7231#section-5.3.3)
**Description** | The Accept-Charset request header advertises which character encodings the client understands.

### http.req.accept_datetime

Attribute | Value
--- | ---
**IE Name** | http.req.accept_datetime
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Reference** | [RFC 7089, section-2.1.1: Accept-Datetime and Memento-Datetime](https://tools.ietf.org/html/rfc7089#section-2.1.1)
**Description** | The Accept-Datetime request header is transmitted by a user agent to indicate it wants to access a past state of an Original Resource.

### http.req.accept_encoding

Attribute | Value
--- | ---
**IE Name** | http.req.accept_encoding
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 5.3.4: Accept-Encoding](https://tools.ietf.org/html/rfc7231#section-5.3.4)
**Description** | The Accept-Encoding request header advertises which content encoding, usually a compression algorithm, the client is able to understand.

### http.req.accept_language

Attribute | Value
--- | ---
**IE Name** | http.req.accept_language
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 5.3.5: Accept-Language](https://tools.ietf.org/html/rfc7231#section-5.3.5)
**Description** | The Accept-Language request header advertises which languages the client is able to understand, and which locale variant is preferred. (By languages, we mean natural languages, such as English, and not programming languages.)

### http.req.access_control_request_headers

Attribute | Value
--- | ---
**IE Name** | http.req.access_control_request_headers
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#http-access-control-request-headers](https://fetch.spec.whatwg.org/#http-access-control-request-headers)
**Description** | The Access-Control-Request-Headers request header is used by browsers when issuing a preflight request, to let the server know which HTTP headers the client might send when the actual request is made.

### http.req.access_control_request_method

Attribute | Value
--- | ---
**IE Name** | http.req.access_control_request_method
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#http-access-control-request-method](https://fetch.spec.whatwg.org/#http-access-control-request-method)
**Description** | The Access-Control-Request-Method request header is used by browsers when issuing a preflight request, to let the server know which HTTP method will be used when the actual request is made. This header is necessary as the preflight request is always an OPTIONS and doesn't use the same method as the actual request.

### http.req.authorization

Attribute | Value
--- | ---
**IE Name** | http.req.authorization
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7235, section 4.2: Authorization](https://tools.ietf.org/html/rfc7235#section-4.2)
**Description** | The HTTP Authorization request header contains the credentials to authenticate a user agent with a server, usually, but not necessarily, after the server has responded with a 401 Unauthorized status and the WWW-Authenticate header.

### http.req.cookie

Attribute | Value
--- | ---
**IE Name** | http.req.cookie
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 6265, section 5.4: Cookie](https://tools.ietf.org/html/rfc6265#section-5.4)
**Description** | The Cookie HTTP request header contains stored HTTP cookies previously sent by the server with the Set-Cookie header.

### http.req.cookie2

Attribute | Value
--- | ---
**IE Name** | http.req.cookie2
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 2965: Cookie2](https://tools.ietf.org/html/rfc2965)
**Description** | The obsolete Cookie2 HTTP request header used to advise the server that the user agent understands *new-style* cookies, but nowadays user agents will use the Cookie header instead, not this one.

### http.req.device_memory

Attribute | Value
--- | ---
**IE Name** | http.req.device_memory
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Units** | gibibytes
**Reference** | [W3C: Device Memory 1](https://w3c.github.io/device-memory/#sec-device-memory-client-hint-header)
**Description** | The Device-Memory header is a Device Memory API header that works like Client Hints header which represents the approximate amount of RAM client device has.

### http.req.dnt

Attribute | Value
--- | ---
**IE Name** | http.req.dnt
**Tier** | common
**Data Type** | unsigned
**Semantic** | indicator
**Reference** | [W3C: Tracking Preference Expression (DNT)](https://www.w3.org/TR/tracking-dnt/#dnt-header-field)
**Description** | The DNT (Do Not Track) request header indicates the user's tracking preference. It lets users indicate whether they would prefer privacy rather than personalized content.

### http.req.dpr

Attribute | Value
--- | ---
**IE Name** | http.req.dpr
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/DPR](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/DPR)
**Description** | The DPR header is a Client Hints headers which represents the client device pixel ratio (DPR), which is the the number of physical device pixels corresponding to every CSS pixel.

### http.req.early_data

Attribute | Value
--- | ---
**IE Name** | http.req.early_data
**Tier** | common
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [RFC 8470, section 5.1: The Early-Data Header Field](https://tools.ietf.org/html/rfc8470#section-5.1)
**Description** | The Early-Data header is set by an intermediary to indicate that the request has been conveyed in TLS early data, and also indicates that the intermediary understands the 425 (Too Early) status code.

### http.req.expect

Attribute | Value
--- | ---
**IE Name** | http.req.expect
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 5.1.1: Expect](https://tools.ietf.org/html/rfc7231#section-5.1.1)
**Description** | The Expect HTTP request header indicates expectations that need to be fulfilled by the server in order to properly handle the request.

### http.req.forwarded

Attribute | Value
--- | ---
**IE Name** | http.req.forwarded
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7239, section 4: Forwarded](https://tools.ietf.org/html/rfc7239#section-4)
**Description** | The Forwarded header contains information from the client-facing side of proxy servers that is altered or lost when a proxy is involved in the path of the request.

### http.req.from

Attribute | Value
--- | ---
**IE Name** | http.req.from
**Tier** | common
**Data Type** | string
**Semantic** | emailaddress
**Reference** | [RFC 7231, section 5.5.1: From](https://tools.ietf.org/html/rfc7231#section-5.5.1)
**Description** | The From request header contains an Internet email address for a human user who controls the requesting user agent.

### http.req.front_end_https

Attribute | Value
--- | ---
**IE Name** | http.req.front_end_https
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [Microsoft: Helping to Secure Communication: Client to Front-End Server](https://docs.microsoft.com/en-us/previous-versions/tn-archive/aa997519(v=exchg.65))
**Description** | Front-End-Https is a Non-standard header field used by Microsoft applications and load-balancers.

### http.req.host

Attribute | Value
--- | ---
**IE Name** | http.req.host
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7230, section 5.4: Host](https://tools.ietf.org/html/rfc7230#section-5.4)
**Description** | The Host request header specifies the host and port number of the server to which the request is being sent. If no port is included, the default port for the service requested (e.g., 443 for an HTTPS URL, and 80 for an HTTP URL) is implied.

### http.req.http2_settings

Attribute | Value
--- | ---
**IE Name** | http.req.http2_settings
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7540, section 3.2.1: HTTP2-Settings Header Field](https://tools.ietf.org/html/rfc7540#section-3.2.1)
**Description** | The HTTP2-Settings header field is a connection-specific header field that includes parameters that govern the HTTP/2 connection, provided in anticipation of the server accepting the request to upgrade.

### http.req.if_match

Attribute | Value
--- | ---
**IE Name** | http.req.if_match
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7232, section 3.1: If-Match](https://tools.ietf.org/html/rfc7232#section-3.1)
**Description** | The If-Match HTTP request header makes the request conditional. For GET and HEAD methods, the server will send back the requested resource only if it matches one of the listed ETags. For PUT and other non-safe methods, it will only upload the resource in this case.

### http.req.if_modified_since

Attribute | Value
--- | ---
**IE Name** | http.req.if_modified_since
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Reference** | [RFC 7232, section 3.3: If-Modified-Since](https://tools.ietf.org/html/rfc7232#section-3.3)
**Description** | The If-Modified-Since request HTTP header makes the request conditional: the server will send back the requested resource, with a 200 status, only if it has been last modified after the given date.

### http.req.if_none_match

Attribute | Value
--- | ---
**IE Name** | http.req.if_none_match
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7232, section 3.2: If-None-Match](https://tools.ietf.org/html/rfc7232#section-3.2)
**Description** | The If-None-Match HTTP request header makes the request conditional. For GET and HEAD methods, the server will send back the requested resource, with a 200 status, only if it doesn't have an ETag matching the given ones. For other methods, the request will be processed only if the eventually existing resource's ETag doesn't match any of the values listed.

### http.req.if_range

Attribute | Value
--- | ---
**IE Name** | http.req.if_range
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7233, section 3.2: If-Range](https://tools.ietf.org/html/rfc7233#section-3.2)
**Description** | The If-Range HTTP request header makes a range request conditional: if the condition is fulfilled, the range request will be issued and the server sends back a 206 Partial Content answer with the appropriate body. If the condition is not fulfilled, the full resource is sent back, with a 200 OK status.

### http.req.if_unmodified_since

Attribute | Value
--- | ---
**IE Name** | http.req.if_unmodified_since
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Reference** | [RFC 7232, section 3.4: If-Unmodified-Since](https://tools.ietf.org/html/rfc7232#section-3.4)
**Description** | The If-Unmodified-Since request HTTP header makes the request conditional: the server will send back the requested resource, or accept it in the case of a POST or another non-safe method, only if it has not been last modified after the given date. If the resource has been modified after the given date, the response will be a 412 (Precondition Failed) error.

### http.req.max_forwards

Attribute | Value
--- | ---
**IE Name** | http.req.max_forwards
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | forwards
**Reference** | [RFC 2616, section 14.31: Max-Forwards](https://tools.ietf.org/html/rfc2616#section-14.31)
**Description** | The Max-Forwards request-header field provides a mechanism with the TRACE and OPTIONS methods to limit the number of proxies or gateways that can forward the request to the next inbound server. This can be useful when the client is attempting to trace a request chain which appears to be failing or looping in mid-chain.

### http.req.origin

Attribute | Value
--- | ---
**IE Name** | http.req.origin
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#origin-header](https://fetch.spec.whatwg.org/#origin-header)
**Description** | The Origin request header indicates where a fetch originates from. It doesn't include any path information, but only the server name. It is sent with CORS requests, as well as with POST requests. It is similar to the Referer header, but, unlike this header, it doesn't disclose the whole path.

### http.req.proxy_authorization

Attribute | Value
--- | ---
**IE Name** | http.req.proxy_authorization
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7235, section 4.4: Proxy-Authorization](https://tools.ietf.org/html/rfc7235#section-4.4)
**Description** | The HTTP Proxy-Authorization request header contains the credentials to authenticate a user agent to a proxy server, usually after the server has responded with a 407 Proxy Authentication Required status and the Proxy-Authenticate header.

### http.req.proxy_connection

Attribute | Value
--- | ---
**IE Name** | http.req.proxy_connection
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [Microsoft: Proxy-Connection header](https://docs.microsoft.com/en-us/openspecs/sql_server_protocols/ms-ssas8/c2b9f128-76f3-48f9-b23d-6bf78516f842)
**Description** | The Proxy-Connection element contains a string value that specifies whether the connection is to be kept open after the request has been sent. If the value indicates that the connection can be kept open, the HTTP 1.1 proxy will accept subsequent requests that can be executed against the server URI.

### http.req.range

Attribute | Value
--- | ---
**IE Name** | http.req.range
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7233, section 3.1: Range](https://tools.ietf.org/html/rfc7233#section-3.1)
**Description** | The Range HTTP request header indicates the part of a document that the server should return.

### http.req.referer

Attribute | Value
--- | ---
**IE Name** | http.req.referer
**Tier** | common
**Data Type** | object: uri
**Reference** | [RFC 7231, section 5.5.2: Referer](https://tools.ietf.org/html/rfc7231#section-5.5.2)
**Description** | The Referer request header contains the address of the previous web page from which a link to the currently requested page was followed.

### http.req.save_data

Attribute | Value
--- | ---
**IE Name** | http.req.save_data
**Tier** | common
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [draft-grigorik-http-client-hints-03, section 7: Save-Data](https://tools.ietf.org/html/draft-grigorik-http-client-hints-03#section-7)
**Description** | The Save-Data header field is a boolean which, in requests, indicates the client's preference for reduced data usage. A numerical value indicating whether the client wants to opt in to reduced data usage mode. on indicates yes, while off (the default) indicates no.

### http.req.sec_fetch_dest

Attribute | Value
--- | ---
**IE Name** | http.req.sec_fetch_dest
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Fetch Metadata Request Headers](https://w3c.github.io/webappsec-fetch-metadata/#sec-fetch-dest-header)
**Description** | The Sec-Fetch-Dest fetch metadata header indicates the request's destination, that is how the fetched data will be used.

### http.req.sec_fetch_mode

Attribute | Value
--- | ---
**IE Name** | http.req.sec_fetch_mode
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Fetch Metadata Request Headers](https://w3c.github.io/webappsec-fetch-metadata/#sec-fetch-dest-header)
**Description** | The Sec-Fetch-Mode fetch metadata header indicates the request's mode.

### http.req.sec_fetch_site

Attribute | Value
--- | ---
**IE Name** | http.req.sec_fetch_site
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Fetch Metadata Request Headers](https://w3c.github.io/webappsec-fetch-metadata/#sec-fetch-dest-header)
**Description** | The Sec-Fetch-Site fetch metadata header indicates the relationship between a request initiator's origin and the origin of the resource.

### http.req.sec_fetch_user

Attribute | Value
--- | ---
**IE Name** | http.req.sec_fetch_user
**Tier** | common
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [W3C: Fetch Metadata Request Headers](https://w3c.github.io/webappsec-fetch-metadata/#sec-fetch-dest-header)
**Description** | The Sec-Fetch-User fetch metadata header indicates whether or not a navigation request was triggered by a user activation.

### http.req.te

Attribute | Value
--- | ---
**IE Name** | http.req.te
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7230, section 4.3: TE](https://tools.ietf.org/html/rfc7230#section-4.3)
**Description** | The TE request header specifies the transfer encodings the user agent is willing to accept.

### http.req.upgrade_insecure_requests

Attribute | Value
--- | ---
**IE Name** | http.req.upgrade_insecure_requests
**Tier** | common
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [W3C: Upgrade Insecure Requests](https://w3c.github.io/webappsec-upgrade-insecure-requests/#preference)
**Description** | The HTTP Upgrade-Insecure-Requests request header sends a signal to the server expressing the client’s preference for an encrypted and authenticated response, and that it can successfully handle the upgrade-insecure-requests CSP directive.

### http.req.user_agent

Attribute | Value
--- | ---
**IE Name** | http.req.user_agent
**Tier** | core
**Data Type** | object: user_agent
**Reference** | [RFC 7231, section 5.5.3: User-Agent](https://tools.ietf.org/html/rfc7231#section-5.5.3)
**Description** | The User-Agent request header is a characteristic string that lets servers and network peers identify the application, operating system, vendor, and/or version of the requesting user agent.

### http.req.x_att_deviceid

Attribute | Value
--- | ---
**IE Name** | http.req.x_att_deviceid
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://www.aqtronix.com/headers/?Action=ShowDetails&Name=X%2DATT%2DDeviceID](https://www.aqtronix.com/headers/?Action=ShowDetails&Name=X%2DATT%2DDeviceID)
**Description** | The X-ATT-DeviceId request header is typically used to identify the make, model, and firmware of AT&T devices.

### http.req.x_authenticated_groups

Attribute | Value
--- | ---
**IE Name** | http.req.x_authenticated_groups
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-3.5: X-Authenticated-Groups](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-3.5)
**Description** | The X-Authenticated-Groups header is a base-64 encoded representation of the groups to which the authenticated user belongs.

### http.req.x_authenticated_user

Attribute | Value
--- | ---
**IE Name** | http.req.x_authenticated_user
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-3.4: X-Authenticated-User](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-3.4)
**Description** | The X-Authenticated-User header is a base-64 encoded representation of the authenticated user name.

### http.req.x_bluecoat_via

Attribute | Value
--- | ---
**IE Name** | http.req.x_bluecoat_via
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Reference** | [Why the ProxySG sends a header "X-Bluecoat-Via:"](https://knowledge.broadcom.com/external/article/167653/why-the-proxysg-sends-a-header-xbluecoat.html#:~:text=The%20purpose%20of%20the%20ProxySG,not%20propagate%20the%20request%20on.)
**Description** | The purpose of the X-Bluecoat-Via header is to detect loops in the network. If the proxy receives a request with the exact same X-Bluecoat-Via header that it generates on the server-side, it knows that the request was generated from itself and it will not be propagated. Each proxy generates a different X-Bluecoat-Via header.

### http.req.x_client_ip

Attribute | Value
--- | ---
**IE Name** | http.req.x_client_ip
**Tier** | common
**Data Type** | ipaddress
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-3.1: X-Client-IP](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-3.1)
**Description** | The X-Client-IP header field is the IP source address of the encapsulated HTTP request. The IP address MUST be a dotted-decimal IPv4 address or an IPv6 hex address.

### http.req.x_csrf_token

Attribute | Value
--- | ---
**IE Name** | http.req.x_csrf_token
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Reference** | [https://en.wikipedia.org/wiki/Cross-site_request_forgery](https://en.wikipedia.org/wiki/Cross-site_request_forgery)
**Description** | The X-Csrf-Token request header contains a value previously provided in the server cookie which can be used to prevent CSRF attacks.

### http.req.x_device_id

Attribute | Value
--- | ---
**IE Name** | http.req.x_device_id
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The X-Device-ID header contains an identifier for the device sending the request.

### http.req.x_flash_version

Attribute | Value
--- | ---
**IE Name** | http.req.x_flash_version
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Reference** | [https://www.aqtronix.com/headers/?Action=ShowDetails&Name=X%2DFlash%2DVersion](https://www.aqtronix.com/headers/?Action=ShowDetails&Name=X%2DFlash%2DVersion)
**Description** | The X-Flash-Version request header contains the version of Adobe Flash running on the client.

### http.req.x_forwarded_for

Attribute | Value
--- | ---
**IE Name** | http.req.x_forwarded_for
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Forwarded-For](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Forwarded-For)
**Description** | The X-Forwarded-For (XFF) header is a de-facto standard header for identifying the originating IP address of a client connecting to a web server through an HTTP proxy or a load balancer. When traffic is intercepted between clients and servers, server access logs contain the IP address of the proxy or load balancer only. To see the original IP address of the client, the X-Forwarded-For request header is used.

### http.req.x_forwarded_host

Attribute | Value
--- | ---
**IE Name** | http.req.x_forwarded_host
**Tier** | common
**Data Type** | object: host
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Forwarded-Host](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Forwarded-Host)
**Description** | The X-Forwarded-Host (XFH) header is a de-facto standard header for identifying the original host requested by the client in the Host HTTP request header.

### http.req.x_forwarded_proto

Attribute | Value
--- | ---
**IE Name** | http.req.x_forwarded_proto
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Forwarded-Proto](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Forwarded-Proto)
**Description** | The X-Forwarded-Proto (XFP) header is a de-facto standard header for identifying the protocol (HTTP or HTTPS) that a client used to connect to your proxy or load balancer. Your server access logs contain the protocol used between the server and the load balancer, but not the protocol used between the client and the load balancer. To determine the protocol used between the client and the load balancer, the X-Forwarded-Proto request header can be used.

### http.req.x_forwarded_server

Attribute | Value
--- | ---
**IE Name** | http.req.x_forwarded_server
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The X-Forwarded-Server header contains the hostname of the proxy server.

### http.req.x_http_method_override

Attribute | Value
--- | ---
**IE Name** | http.req.x_http_method_override
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://www.ibm.com/support/knowledgecenter/SSQP76_8.9.0/com.ibm.odm.dserver.rules.res.managing/topics/con_res_restapi_rsrcmng_methods.html](https://www.ibm.com/support/knowledgecenter/SSQP76_8.9.0/com.ibm.odm.dserver.rules.res.managing/topics/con_res_restapi_rsrcmng_methods.html)
**Description** | The X-HTTP-Method-Override header is used to override the HTTP method of the request. It can be used to channel a PUT or DELETE request through a POST request.

### http.req.x_idfa

Attribute | Value
--- | ---
**IE Name** | http.req.x_idfa
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Description** | The X-IDFA request header contains an Identifier for Advertising (IDFA).

### http.req.x_idfv

Attribute | Value
--- | ---
**IE Name** | http.req.x_idfv
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Description** | The X-IDFV request header contains an Identifier for Vendor (IDFV).

### http.req.x_method_override

Attribute | Value
--- | ---
**IE Name** | http.req.x_method_override
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://www.ibm.com/support/knowledgecenter/SSQP76_8.9.0/com.ibm.odm.dserver.rules.res.managing/topics/con_res_restapi_rsrcmng_methods.html](https://www.ibm.com/support/knowledgecenter/SSQP76_8.9.0/com.ibm.odm.dserver.rules.res.managing/topics/con_res_restapi_rsrcmng_methods.html)
**Description** | The X-Method-Override header is used to override the HTTP method of the request. It can be used to channel a PUT or DELETE request through a POST request.

### http.req.x_nonce

Attribute | Value
--- | ---
**IE Name** | http.req.x_nonce
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Description** | The X-Nonce header contains a base64-encoded client nonce.

### http.req.x_organization_id

Attribute | Value
--- | ---
**IE Name** | http.req.x_organization_id
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The X-Organization-ID contains the UUID for an organization.

### http.req.x_profile

Attribute | Value
--- | ---
**IE Name** | http.req.x_profile
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The X-Profile request header.

### http.req.x_profile_token

Attribute | Value
--- | ---
**IE Name** | http.req.x_profile_token
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The X-Profile-Token request header.

### http.req.x_request_id

Attribute | Value
--- | ---
**IE Name** | http.req.x_request_id
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The X-Request-ID request header contains an ID sent by a client to the server. Messages from the server may include this value in the X-Correlation-ID of any response which is related to the request.

### http.req.x_requested_with

Attribute | Value
--- | ---
**IE Name** | http.req.x_requested_with
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://en.wikipedia.org/wiki/List_of_HTTP_header_fields](https://en.wikipedia.org/wiki/List_of_HTTP_header_fields)
**Description** | The X-Requested-With request header is typically used to identify Ajax requests.

### http.req.x_server_ip

Attribute | Value
--- | ---
**IE Name** | http.req.x_server_ip
**Tier** | common
**Data Type** | ipaddress
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-3.2: X-Server-IP](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-3.2)
**Description** | The X-Server-IP header is the IP destination address of the encapsulated HTTP request. It specifies the HTTP destination host and not the IP address of any intermediate proxy server. The IP address MUST be a dotted-decimal IPv4 address or an IPv6 hex address.

### http.req.x_subscriber_id

Attribute | Value
--- | ---
**IE Name** | http.req.x_subscriber_id
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-3.3: X-Subscriber-ID](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-3.3)
**Description** | The X-Subscriber-ID header contains a unique subscriber ID of the user who issued the HTTP request. This MAY be an e-mail address but the exact format of the subscriber ID is not specified by ICAP or this document.

### http.req.x_time

Attribute | Value
--- | ---
**IE Name** | http.req.x_time
**Tier** | common
**Data Type** | string
**Semantic** | quantity
**Unit**: | seconds
**Description** | The X-Time request header.

### http.req.x_uidh

Attribute | Value
--- | ---
**IE Name** | http.req.x_uidh
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Reference** | [http://webpolicy.org/2014/10/24/how-verizons-advertising-header-works/](http://webpolicy.org/2014/10/24/how-verizons-advertising-header-works/)
**Description** | The X-UIDH request header contains Verizon's Advertising ID Header.

### http.req.x_user_agent

Attribute | Value
--- | ---
**IE Name** | http.req.x_user_agent
**Tier** | common
**Data Type** | object: user_agent
**Description** | The X-User-Agent header is often inserted by some independent messenger between the actual client and the server, like a proxy, load balancer or transcoder, but also some *XMLHttpRequest* based libraries. It often identifies the messenger itself. The User-Agent header should still represent the actual client. You also see this header sometimes in emails, this then represents the email program/software responsible for sending the message.

### http.req.x_wap_profile

Attribute | Value
--- | ---
**IE Name** | http.req.x_wap_profile
**Tier** | common
**Data Type** | string
**Semantic** | uri
**Reference** | [http://www.aqtronix.com/headers/?Action=ShowDetails&Name=X%2DWAP%2DProfile](http://www.aqtronix.com/headers/?Action=ShowDetails&Name=X%2DWAP%2DProfile)
**Description** | The X-Wap-Profile request header is typically used to link to an XML file on the Internet with a full description and details about the device currently connecting.

## http.resp

Contains *response headers* and additional attributes related to an HTTP response.

A *response header* is an HTTP header that can be used in an HTTP response and that doesn't relate to the content of the message. Not all headers appearing in a response are response headers.

### http.resp.datetime

Attribute | Value
--- | ---
**IE Name** | http.resp.datetime
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Description** | The timestamp, expressed as an HTTP-date value, when the HTTP response was observed.

### http.resp.timestamp

Attribute | Value
--- | ---
**IE Name** | http.resp.timestamp
**Tier** | common
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | milliseconds
**Description** | The timestamp, expressed as milliseconds since epoch, when the HTTP response was observed.

### http.resp.bytes

Attribute | Value
--- | ---
**IE Name** | http.resp.bytes
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Description** | The size/length of the HTTP request.

### http.resp.status

Attribute | Value
--- | ---
**IE Name** | http.resp.status
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | [IANA: Hypertext Transfer Protocol (HTTP) Status Code Registry](https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml)
**Description** | HTTP response status codes indicate whether a specific HTTP request has been successfully completed.

### http.resp.reason_phrase

Attribute | Value
--- | ---
**IE Name** | http.resp.reason_phrase
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [IANA: Hypertext Transfer Protocol (HTTP) Status Code Registry](https://www.iana.org/assignments/http-status-codes/http-status-codes.xhtml)
**Description** | The Reason-Phrase is intended to give a short textual description of the Status-Code.

### http.resp.accept_ch

Attribute | Value
--- | ---
**IE Name** | http.resp.accept_ch
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-CH](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-CH)
**Description** | The Accept-CH response header is set by the server to specify which Client Hints headers a client should include in subsequent requests.

### http.resp.accept_ch_lifetime

Attribute | Value
--- | ---
**IE Name** | http.resp.accept_ch_lifetime
**Tier** | common
**Data Type** | integer
**Semantic** | quantity
**Unit** | seconds
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-CH-Lifetime](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-CH-Lifetime)
**Description** | The Accept-CH-Lifetime response header is set by the server to specify the persistence of Accept-CH header value that specifies for which Client Hints headers client should include in subsequent requests.

### http.resp.accept_patch

Attribute | Value
--- | ---
**IE Name** | http.resp.accept_patch
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 5789, section 3.1: Accept-Patch](https://tools.ietf.org/html/rfc5789#section-3.1)
**Description** | The Accept-Patch response header advertises which media-type the server is able to understand.

### http.resp.accept_ranges

Attribute | Value
--- | ---
**IE Name** | http.resp.accept_ranges
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7233, section 2.3: Accept-Ranges](https://tools.ietf.org/html/rfc7233#section-2.3)
**Description** | The Accept-Ranges response HTTP header is a marker used by the server to advertise its support of partial requests. The value of this field indicates the unit that can be used to define a range.

### http.resp.access_control_allow_credentials

Attribute | Value
--- | ---
**IE Name** | http.resp.access_control_allow_credentials
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#http-access-control-allow-credentials](https://fetch.spec.whatwg.org/#http-access-control-allow-credentials)
**Description** | The Access-Control-Allow-Credentials response header tells browsers whether to expose the response to frontend JavaScript code when the request's credentials mode is include.

### http.resp.access_control_allow_headers

Attribute | Value
--- | ---
**IE Name** | http.resp.access_control_allow_headers
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#http-access-control-allow-headers](https://fetch.spec.whatwg.org/#http-access-control-allow-headers)
**Description** | The Access-Control-Allow-Headers response header is used in response to a preflight request which includes Access-Control-Request-Headers to indicate which HTTP headers can be used during the actual request.

### http.resp.access_control_allow_methods

Attribute | Value
--- | ---
**IE Name** | http.resp.access_control_allow_methods
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#http-access-control-allow-methods](https://fetch.spec.whatwg.org/#http-access-control-allow-methods)
**Description** | The Access-Control-Allow-Methods response header specifies the method or methods allowed when accessing the resource in response to a preflight request.

### http.resp.access_control_allow_origin

Attribute | Value
--- | ---
**IE Name** | http.resp.access_control_allow_origin
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#http-access-control-allow-origin](https://fetch.spec.whatwg.org/#http-access-control-allow-origin)
**Description** | The Access-Control-Allow-Origin response header indicates whether the response can be shared with requesting code from the given origin.

### http.resp.access_control_expose_headers

Attribute | Value
--- | ---
**IE Name** | http.resp.access_control_expose_headers
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#http-access-control-expose-headers](https://fetch.spec.whatwg.org/#http-access-control-expose-headers)
**Description** | The Access-Control-Expose-Headers response header indicates which headers can be exposed as part of the response by listing their names.

### http.resp.access_control_max_age

Attribute | Value
--- | ---
**IE Name** | http.resp.access_control_max_age
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | seconds
**Reference** | [https://fetch.spec.whatwg.org/#http-access-control-max-age](https://fetch.spec.whatwg.org/#http-access-control-max-age)
**Description** | The Access-Control-Max-Age response header indicates how long the results of a preflight request (that is the information contained in the Access-Control-Allow-Methods and Access-Control-Allow-Headers headers) can be cached.

### http.resp.age

Attribute | Value
--- | ---
**IE Name** | http.resp.age
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | seconds
**Reference** | [RFC 7234, section 5.1: Age](https://tools.ietf.org/html/rfc7234#section-5.1)
**Description** | The Age header contains the time in seconds the object has been in a proxy cache.

### http.resp.alt_svc

Attribute | Value
--- | ---
**IE Name** | http.resp.alt_svc
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7838, section 3: The Alt-Svc HTTP Header Field](https://tools.ietf.org/html/rfc7838#section-3)
**Description** | The Alt-Svc HTTP response header is used to advertise alternative services through which the same resource can be reached. An alternative service is defined by a protocol/host/port combination.

### http.resp.clear_site_data

Attribute | Value
--- | ---
**IE Name** | http.resp.clear_site_data
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Clear Site Data](https://w3c.github.io/webappsec-clear-site-data)
**Description** | The Clear-Site-Data header clears browsing data (cookies, storage, cache) associated with the requesting website. It allows web developers to have more control over the data stored locally by a browser for their origins.

### http.resp.content_disposition

Attribute | Value
--- | ---
**IE Name** | http.resp.content_disposition
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 6266: Use of the Content-Disposition Header Field](https://tools.ietf.org/html/rfc6266)
**Description** | In a regular HTTP response, the Content-Disposition response header is a header indicating if the content is expected to be displayed inline in the browser, that is, as a Web page or as part of a Web page, or as an attachment, that is downloaded and saved locally.

### http.resp.content_range

Attribute | Value
--- | ---
**IE Name** | http.resp.content_range
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7233, section 4.2: Content-Range](https://tools.ietf.org/html/rfc7233#section-4.2)
**Description** | The Content-Range response HTTP header indicates where in a full body message a partial message belongs.

### http.resp.content_security_policy

Attribute | Value
--- | ---
**IE Name** | http.resp.content_security_policy
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [Content Security Policy Level 3](https://w3c.github.io/webappsec-csp/)
**Description** | The HTTP Content-Security-Policy response header allows web site administrators to control resources the user agent is allowed to load for a given page.

### http.resp.content_security_policy_report_only

Attribute | Value
--- | ---
**IE Name** | http.resp.content_security_policy_report_only
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Content Security Policy Level 3](https://w3c.github.io/webappsec-csp/)
**Description** | The HTTP Content-Security-Policy-Report-Only response header allows web developers to experiment with policies by monitoring (but not enforcing) their effects.

### http.resp.cross_origin_resource_policy

Attribute | Value
--- | ---
**IE Name** | http.resp.cross_origin_resource_policy
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#cross-origin-resource-policy-header](https://fetch.spec.whatwg.org/#cross-origin-resource-policy-header)
**Description** | The HTTP Cross-Origin-Resource-Policy response header conveys a desire that the browser blocks no-cors cross-origin/cross-site requests to the given resource.

### http.resp.digest

Attribute | Value
--- | ---
**IE Name** | http.resp.digest
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 3230, section 4.3.2: Digest](https://tools.ietf.org/html/rfc3230#section-4.3.2)
**Description** | The Digest response HTTP header provides a digest of the requested resource.

### http.resp.etag

Attribute | Value
--- | ---
**IE Name** | http.resp.etag
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7232, section 2.3: ETag](https://tools.ietf.org/html/rfc7232#section-2.3)
**Description** | The ETag HTTP response header is an identifier for a specific version of a resource. It lets caches be more efficient and save bandwidth, as a web server does not need to resend a full response if the content has not changed.

### http.resp.expect_ct

Attribute | Value
--- | ---
**IE Name** | http.resp.expect_ct
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-ietf-httpbis-expect-ct-08: Expect-CT Extension for HTTP](https://tools.ietf.org/html/draft-ietf-httpbis-expect-ct-08)
**Description** | The Expect-CT header lets sites opt in to reporting and/or enforcement of Certificate Transparency requirements, to prevent the use of misissued certificates for that site from going unnoticed.

### http.resp.expires

Attribute | Value
--- | ---
**IE Name** | http.resp.expires
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Reference** | [RFC 7234, section 5.3: Expires](https://tools.ietf.org/html/rfc7234#section-5.3)
**Description** | The Expires header contains the date/time after which the response is considered stale. Invalid dates, like the value 0, represent a date in the past and mean that the resource is already expired.

### http.resp.feature_policy

Attribute | Value
--- | ---
**IE Name** | http.resp.feature_policy
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Feature Policy](https://w3c.github.io/webappsec-feature-policy/#feature-policy-http-header-field)
**Description** | The HTTP Feature-Policy header provides a mechanism to allow and deny the use of browser features in its own frame, and in content within any `<iframe>` elements in the document.

### http.resp.im

Attribute | Value
--- | ---
**IE Name** | http.resp.im
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 3229, section 10.5.2: IM](https://tools.ietf.org/html/rfc3229#section-10.5.2)
**Description** | The IM response header indicates the instance-manipulations, if any, that have been applied to the instance represented by the response. Typical instance manipulations include *delta encoding* and *compression*.

### http.resp.large_allocation

Attribute | Value
--- | ---
**IE Name** | http.resp.large_allocation
**Tier** | custom
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | megabytes
**Reference** | [https://gist.github.com/mystor/5739e222e398efc6c29108be55eb6fe3](https://gist.github.com/mystor/5739e222e398efc6c29108be55eb6fe3)
**Description** | The non-standard Large-Allocation response header tells the browser that the page being loaded is going to want to perform a large allocation. It is currently only implemented in Firefox, but is harmless to send to every browser.

### http.resp.last_modified

Attribute | Value
--- | ---
**IE Name** | http.resp.last_modified
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Reference** | [RFC 7232, section 2.2: Last-Modified](https://tools.ietf.org/html/rfc7232#section-2.2)
**Description** | The Last-Modified response HTTP header contains the date and time at which the origin server believes the resource was last modified. It is used as a validator to determine if a resource received or stored is the same. Less accurate than an ETag header, it is a fallback mechanism. Conditional requests containing If-Modified-Since or If-Unmodified-Since headers make use of this field.

### http.resp.location

Attribute | Value
--- | ---
**IE Name** | http.resp.location
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 7.1.2: Location](https://tools.ietf.org/html/rfc7231#section-7.1.2)
**Description** | The Location response header indicates the URL to redirect a page to. It only provides a meaning when served with a 3xx (redirection) or 201 (created) status response.

### http.resp.memento_datetime

Attribute | Value
--- | ---
**IE Name** | http.resp.memento_datetime
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Reference** | [RFC 7089, section-2.1.1: Accept-Datetime and Memento-Datetime](https://tools.ietf.org/html/rfc7089#section-2.1.1)
**Description** | The Memento-Datetime response header response header is used by a server to indicate that a response reflects a prior state of an Original Resource. Its value expresses the datetime of that state.

### http.resp.nel

Attribute | Value
--- | ---
**IE Name** | http.resp.nel
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Network Error Logging](https://w3c.github.io/network-error-logging/#nel-response-header), [Network Error Logging (NEL) explainer](https://developer.mozilla.org/en-US/docs/Web/HTTP/Network_Error_Logging)
**Description** | The HTTP NEL response header is used to configure network request logging.

### http.resp.p3p

Attribute | Value
--- | ---
**IE Name** | http.resp.p3p
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: The HTTP header for P3P1.0](https://www.w3.org/2002/04/P3Pv1-header.txt)
**Description** | The P3P response header sets P3P policy to be used by the browser.

### http.resp.proxy_authenticate

Attribute | Value
--- | ---
**IE Name** | http.resp.proxy_authenticate
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7235, section 4.3: Proxy-Authenticate](https://tools.ietf.org/html/rfc7235#section-4.3)
**Description** | The HTTP Proxy-Authenticate response header defines the authentication method that should be used to gain access to a resource behind a proxy server. It authenticates the request to the proxy server, allowing it to transmit the request further.

### http.resp.public_key_pins

Attribute | Value
--- | ---
**IE Name** | http.resp.public_key_pins
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7469, section 2.1: Public-Key-Pins](https://tools.ietf.org/html/rfc7469#section-2.1)
**Description** | The HTTP Public-Key-Pins response header used to associate a specific cryptographic public key with a certain web server to decrease the risk of MITM attacks with forged certificates, however, it has been removed from modern browsers and is no longer supported. Use Certificate Transparency and Expect-CT header instead.

### http.resp.public_key_pins_report_only

Attribute | Value
--- | ---
**IE Name** | http.resp.public_key_pins_report_only
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7469, section 2.1: Public-Key-Pins-Report-Only](https://tools.ietf.org/html/rfc7469#section-2.1)
**Description** | The HTTP Public-Key-Pins-Report-Only response header was used to send reports of pinning violation to the report-uri specified in the header but, unlike Public-Key-Pins still allows browsers to connect to the server if the pinning is violated. The header is silently ignored in modern browsers as support for HPKP has been removed. Use Certificate Transparency and the Expect-CT header instead.

### http.resp.referrer_policy

Attribute | Value
--- | ---
**IE Name** | http.resp.referrer_policy
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Referrer Policy](https://w3c.github.io/webappsec-referrer-policy/#referrer-policy-header)
**Description** | The Referrer-Policy HTTP header controls how much referrer information (sent via the Referer header) should be included with requests.

### http.resp.refresh

Attribute | Value
--- | ---
**IE Name** | http.resp.refresh
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [http://www.otsukare.info/2015/03/26/refresh-http-header](http://www.otsukare.info/2015/03/26/refresh-http-header)
**Description** | The Refresh response header instructs the client to refresh a given URL at a specified interval. This behavior is similar to the `<meta http-equiv="refresh" …/>` method.

### http.resp.retry_after

Attribute | Value
--- | ---
**IE Name** | http.resp.retry_after
**Tier** | common
**Data Type** | string
**Semantic** | httpdate
**Reference** | [RFC 7231, section 7.1.3: Retry-After](https://tools.ietf.org/html/rfc7231#section-7.1.3)
**Description** | The Retry-After response HTTP header indicates how long the user agent should wait before making a follow-up request. This value may also contain a quantity of seconds.

### http.resp.sec_websocket_accept

Attribute | Value
--- | ---
**IE Name** | http.resp.sec_websocket_accept
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 6455, section 11.3.3: Sec-WebSocket-Accept](https://tools.ietf.org/html/rfc6455#section-11.3.3)
**Description** | The Sec-WebSocket-Accept header is used in the websocket opening handshake. It would appear in the response headers. That is, this is header is sent from server to client to inform that server is willing to initiate a websocket connection.

### http.resp.server

Attribute | Value
--- | ---
**IE Name** | http.resp.server
**Tier** | common
**Data Type** | object: user_agent
**Reference** | [RFC 7231, section 7.4.2: Server](https://tools.ietf.org/html/rfc7231#section-7.4.2)
**Description** | The Server header describes the software used by the origin server that handled the request, that is, the server that generated the response. The name of the software or product that handled the request. Usually in a format similar to User-Agent. How much detail to include is an interesting balance to strike; exposing the OS version is probably a bad idea, as mentioned in the earlier warning about overly-detailed values. However, exposed Apache versions helped browsers work around a bug those versions had with Content-Encoding combined with Range.

### http.resp.server_timing

Attribute | Value
--- | ---
**IE Name** | http.resp.server_timing
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Server Timing](https://w3c.github.io/server-timing/#the-server-timing-header-field)
**Description** | The Server-Timing header communicates one or more metrics and descriptions for a given request-response cycle. It is used to surface any backend server timing metrics (e.g. database read/write, CPU time, file system access, etc.) in the developer tools in the user's browser or in the PerformanceServerTiming interface.

### http.resp.set_cookie

Attribute | Value
--- | ---
**IE Name** | http.resp.set_cookie
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 6265, section 4.1: Set-Cookie](https://tools.ietf.org/html/rfc6265#section-4.1)
**Description** | The Set-Cookie HTTP response header is used to send cookies from the server to the user agent, so the user agent can send them back to the server later.

### http.resp.set_cookie2

Attribute | Value
--- | ---
**IE Name** | http.resp.set_cookie2
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 2965: Set-Cookie2](https://tools.ietf.org/html/rfc2965)
**Description** | The obsolete Set-Cookie2 HTTP response header used to send cookies from the server to the user agent, but has been deprecated by the specification. Use Set-Cookie instead.

### http.resp.sourcemap

Attribute | Value
--- | ---
**IE Name** | http.resp.sourcemap
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [Source Map Revision 3 Proposal](https://docs.google.com/document/d/1U1RGAehQwRypUTovF1KRlpiOFze0b-_2gc6fAH0KY0k)
**Description** | The SourceMap HTTP response header links generated code to a source map, enabling the browser to reconstruct the original source and present the reconstructed original in the debugger.

### http.resp.strict_transport_security

Attribute | Value
--- | ---
**IE Name** | http.resp.strict_transport_security
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 6797, section 6.1: Strict-Transport-Security HTTP Response Header Field](https://tools.ietf.org/html/rfc6797#section-6.1)
**Description** | The Strict-Transport-Security HTTP response header field (STS header field) indicates to a UA that it MUST enforce the HSTS Policy in regards to the host emitting the response message containing this header field.

### http.resp.timing_allow_origin

Attribute | Value
--- | ---
**IE Name** | http.resp.timing_allow_origin
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Resource Timing Level 3](https://w3c.github.io/resource-timing/#sec-timing-allow-origin)
**Description** | The Timing-Allow-Origin response header specifies origins that are allowed to see values of attributes retrieved via features of the Resource Timing API, which would otherwise be reported as zero due to cross-origin restrictions.

### http.resp.tk

Attribute | Value
--- | ---
**IE Name** | http.resp.tk
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [W3C: Tracking Preference Expression (DNT)](https://www.w3.org/TR/tracking-dnt/#Tk-header-defn)
**Description** | The Tk response header indicates the tracking status that applied to the corresponding request.

### http.resp.trailer

Attribute | Value
--- | ---
**IE Name** | http.resp.trailer
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7230, section 4.4: Trailer](https://tools.ietf.org/html/rfc7230#section-4.4)
**Description** | The Trailer response header allows the sender to include additional fields at the end of chunked messages in order to supply metadata that might be dynamically generated while the message body is sent, such as a message integrity check, digital signature, or post-processing status.

### http.resp.transfer_encoding

Attribute | Value
--- | ---
**IE Name** | http.resp.transfer_encoding
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7230, section 3.3.1: Transfer-Encoding](https://tools.ietf.org/html/rfc7230#section-3.3.1)
**Description** | The Transfer-Encoding header specifies the form of encoding used to safely transfer the payload body to the user.

### http.resp.vary

Attribute | Value
--- | ---
**IE Name** | http.resp.vary
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 7.1.4: Vary](https://tools.ietf.org/html/rfc7231#section-7.1.4)
**Description** | The Vary HTTP response header determines how to match future request headers to decide whether a cached response can be used rather than requesting a fresh one from the origin server. It is used by the server to indicate which headers it used when selecting a representation of a resource in a content negotiation algorithm.

### http.resp.www_authenticate

Attribute | Value
--- | ---
**IE Name** | http.resp.www_authenticate
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7235, section-4.1: WWW-Authenticate](https://tools.ietf.org/html/rfc7235#section-4.1)
**Description** | The HTTP WWW-Authenticate response header defines the authentication method that should be used to gain access to a resource.

### http.resp.x_attribute

Attribute | Value
--- | ---
**IE Name** | http.resp.x_attribute
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.2: X-Attribute](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.2)
**Description** | The X-Attribute header SHOULD be used to return a list of attributes to the ICAP client.

### http.resp.x_attribute_cacheability

Attribute | Value
--- | ---
**IE Name** | http.resp.x_attribute_cacheability
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.3: X-Attribute-Cacheability](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.3)
**Description** | The X-Attribute-Cacheability header can specify that the X-Attribute response is valid for all clients or only valid for one user or one user group.

### http.resp.x_attribute_prefix

Attribute | Value
--- | ---
**IE Name** | http.resp.x_attribute_prefix
**Tier** | common
**Data Type** | unsigned
**Semantic** | quantity
**Reference** | [draft-stecher-icap-subid-00, section-4.4: X-Attribute-Prefix](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.4)
**Description** | The X-Attribute-Prefix header is used by the ICAP server to tell the client how many characters of the original URL's path (not the host name) are significant.

### http.resp.x_content_digest

Attribute | Value
--- | ---
**IE Name** | http.resp.x_content_digest
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://www.ibm.com/support/knowledgecenter/STXNRM_3.14.7/coss.doc/sohApi_content_digest.html](https://www.ibm.com/support/knowledgecenter/STXNRM_3.14.7/coss.doc/sohApi_content_digest.html)
**Description** | The X-Content-Digest response header contains a hex-encoded digest value, which is returned when the client can request that the server calculate a digest on the content with the X-Digest request header.

### http.resp.x_content_duration

Attribute | Value
--- | ---
**IE Name** | http.resp.x_content_duration
**Tier** | common
**Data Type** | float
**Semantic** | quantity
**Unit** | seconds
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Configuring_servers_for_Ogg_media](https://developer.mozilla.org/en-US/docs/Web/HTTP/Configuring_servers_for_Ogg_media)
**Description** | The X-Content-Duration header contains the duration of the video in seconds when serving Ogg media files.

### http.resp.x_content_security_policy

Attribute | Value
--- | ---
**IE Name** | http.resp.x_content_security_policy
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://content-security-policy.com/](https://content-security-policy.com/)
**Description** | The X-Content-Security-Policy response header is deprecated and has been replaced by the Content-Security-Policy header. It is known that having both Content-Security-Policy and X-Content-Security-Policy or X-Webkit-CSP causes unexpected behaviours on certain versions of browsers. Please avoid using deprecated X-* headers.

### http.resp.x_content_type_options

Attribute | Value
--- | ---
**IE Name** | http.resp.x_content_type_options
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://fetch.spec.whatwg.org/#x-content-type-options-header](https://fetch.spec.whatwg.org/#x-content-type-options-header)
**Description** | The X-Content-Type-Options response HTTP header is a marker used by the server to indicate that the MIME types advertised in the Content-Type headers should not be changed and be followed.

### http.resp.x_correlation_id

Attribute | Value
--- | ---
**IE Name** | http.resp.x_correlation_id
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The X-Request-ID request header contains an ID sent by a client to the server. Messages from the server may include this value in the X-Correlation-ID of any response which is related to the request.

### http.resp.x_dns_prefetch_control

Attribute | Value
--- | ---
**IE Name** | http.resp.x_dns_prefetch_control
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-DNS-Prefetch-Control](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-DNS-Prefetch-Control)
**Description** | The X-DNS-Prefetch-Control HTTP response header controls DNS prefetching, a feature by which browsers proactively perform domain name resolution on both links that the user may choose to follow as well as URLs for items referenced by the document, including images, CSS, JavaScript, and so forth.

### http.resp.x_frame_options

Attribute | Value
--- | ---
**IE Name** | http.resp.x_frame_options
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7034, section 2: X-Frame-Options Header](https://tools.ietf.org/html/rfc7034#section-2)
**Description** | The X-Frame-Options HTTP response header can be used to indicate whether or not a browser should be allowed to render a page in a `<frame>`, `<iframe>`, `<embed>` or `<object>`. Sites can use this to avoid click-jacking attacks, by ensuring that their content is not embedded into other sites.

### http.resp.x_icap_profile

Attribute | Value
--- | ---
**IE Name** | http.resp.x_icap_profile
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.1: X-ICAP-Profile](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.1)
**Description** | The X-ICAP-Profile response header contains the applied user profile.

### http.resp.x_infection_found

Attribute | Value
--- | ---
**IE Name** | http.resp.x_infection_found
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.5: X-Infection-Found](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.5)
**Description** | The X-Infection-Found header is a semicolon-separated parameter list used to inform the ICAP client about the threats that have been found in the ICAP message body of the request.

### http.resp.x_powered_by

Attribute | Value
--- | ---
**IE Name** | http.resp.x_powered_by
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://en.wikipedia.org/wiki/List_of_HTTP_header_fields](https://en.wikipedia.org/wiki/List_of_HTTP_header_fields)
**Description** | The X-Powered-By header specifies the technology (e.g. ASP.NET, PHP, JBoss) supporting the web application (version details are often in X-Runtime, X-Version, or X-AspNet-Version).

### http.resp.x_response_desc

Attribute | Value
--- | ---
**IE Name** | http.resp.x_response_desc
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.9: X-Response-Desc](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.9)
**Description** | The X-Response-Desc header contains a one line description about the action that the ICAP service applied on the content.

### http.resp.x_response_info

Attribute | Value
--- | ---
**IE Name** | http.resp.x_response_info
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.8: X-Response-Info](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.8)
**Description** | The X-Response-Info header contains a one word description of the action that the ICAP service applied to the content.

### http.resp.x_response_time

Attribute | Value
--- | ---
**IE Name** | http.resp.x_response_time
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.8: X-Response-Info](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.8)
**Description** | The X-Response-Info header is produced by the *response-time* npm module. This module creates a middleware that records the response time for requests in HTTP servers, and adds an X-Response-Time header to responses. The *response time* is defined here as the elapsed time from when a request enters this middleware to when the headers are written out to the client.

### http.resp.x_ua_compatible

Attribute | Value
--- | ---
**IE Name** | http.resp.x_ua_compatible
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [Microsoft: X-UA-Compatibility Meta Tag and HTTP Response Header](https://docs.microsoft.com/en-us/openspecs/ie_standards/ms-iedoco/380e2488-f5eb-4457-a07a-0cb1b6e4b4b5)
**Description** | The X-UA-Compatible response header allows web authors to choose for which version of Internet Explorer the page should be rendered. As of Internet Explorer 11, document modes have been deprecated and are no longer used. IE11 has updated support for web standards that caused issues with older websites.

### http.resp.x_violations_found

Attribute | Value
--- | ---
**IE Name** | http.resp.x_violations_found
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.6: X-Violations-Found](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.6)
**Description** | The X-Violations-Found header provides a detailed description of all the policy violations that occurred while handling the request.

### http.resp.x_virus_id

Attribute | Value
--- | ---
**IE Name** | http.resp.x_virus_id
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [draft-stecher-icap-subid-00, section-4.7: X-Virus-ID](https://tools.ietf.org/html/draft-stecher-icap-subid-00#section-4.7)
**Description** | The X-Virus-ID header is a shorter alternative to the X-Infection-Found header. It can contain any virus or threat description.

### http.resp.x_webkit_csp

Attribute | Value
--- | ---
**IE Name** | http.resp.x_webkit_csp
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://content-security-policy.com/](https://content-security-policy.com/)
**Description** | The X-Webkit-CSP response header is deprecated and has been replaced by the Content-Security-Policy header. It is known that having both Content-Security-Policy and X-Content-Security-Policy or X-Webkit-CSP causes unexpected behaviours on certain versions of browsers. Please avoid using deprecated X-* headers.

### http.resp.x_xss_protection

Attribute | Value
--- | ---
**IE Name** | http.resp.x_xss_protection
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-XSS-Protection)
**Description** | The HTTP X-XSS-Protection response header is a feature of Internet Explorer, Chrome and Safari that stops pages from loading when they detect reflected cross-site scripting (XSS) attacks.

## http.transact

The http.transact object contains information elements related to an HTTP transaction, i.e. the full request/response process.

### http.transact.client_load_start

Attribute | Value
--- | ---
**IE Name** | http.transact.client_load_start
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

### http.transact.client_load_end

Attribute | Value
--- | ---
**IE Name** | http.transact.client_load_end
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

### http.transact.client_render_start

Attribute | Value
--- | ---
**IE Name** | http.transact.client_render_start
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

### http.transact.client_render_end

Attribute | Value
--- | ---
**IE Name** | http.transact.client_render_end
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

### http.transact.req

#### http.transact.req.first_byte_in

Attribute | Value
--- | ---
**IE Name** | http.transact.req.first_byte_in
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

#### http.transact.req.first_byte_out

Attribute | Value
--- | ---
**IE Name** | http.transact.req.first_byte_out
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

#### http.transact.req.last_byte_in

Attribute | Value
--- | ---
**IE Name** | http.transact.req.last_byte_in
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

#### http.transact.req.last_byte_out

Attribute | Value
--- | ---
**IE Name** | http.transact.req.last_byte_out
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

### http.transact.resp

#### http.transact.resp.first_byte_in

Attribute | Value
--- | ---
**IE Name** | http.transact.resp.first_byte_in
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

#### http.transact.resp.first_byte_out

Attribute | Value
--- | ---
**IE Name** | http.transact.resp.first_byte_out
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

#### http.transact.resp.last_byte_in

Attribute | Value
--- | ---
**IE Name** | http.transact.resp.last_byte_in
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 

#### http.transact.resp.last_byte_out

Attribute | Value
--- | ---
**IE Name** | http.transact.resp.last_byte_out
**Tier** | custom
**Data Type** | unsigned
**Semantic** | epochticks
**Unit** | microseconds
**Description** | 
