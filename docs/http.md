# HTTP Information Elements

## `http.version`

Attribute | Value
--- | ---
**IE Name** | `http.version`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

## `http.url`

### `http.url.uri`

Attribute | Value
--- | ---
**IE Name** | `http.url.uri`
**Tier** | `core`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.ip`

Attribute | Value
--- | ---
**IE Name** | `http.url.ip`
**Tier** | ``
**Data Type** | `ipaddress`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.scheme`

Attribute | Value
--- | ---
**IE Name** | `http.url.scheme`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.domain`

Attribute | Value
--- | ---
**IE Name** | `http.url.domain`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.server`

Attribute | Value
--- | ---
**IE Name** | `http.url.server`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.port`

Attribute | Value
--- | ---
**IE Name** | `http.url.port`
**Tier** | ``
**Data Type** | `unsigned`
**Semantic** | `identifier`
**Reference** | []()
**Description** | 

### `http.url.path`

Attribute | Value
--- | ---
**IE Name** | `http.url.path`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.fragment`

Attribute | Value
--- | ---
**IE Name** | `http.url.fragment`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.query`

Attribute | Value
--- | ---
**IE Name** | `http.url.query`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.user`

Attribute | Value
--- | ---
**IE Name** | `http.url.user`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.url.password`

Attribute | Value
--- | ---
**IE Name** | `http.url.password`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

## `http.redir`

### `http.redir.uri`

Attribute | Value
--- | ---
**IE Name** | `http.redir.uri`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.ip`

Attribute | Value
--- | ---
**IE Name** | `http.redir.ip`
**Tier** | ``
**Data Type** | `ipaddress`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.scheme`

Attribute | Value
--- | ---
**IE Name** | `http.redir.scheme`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.domain`

Attribute | Value
--- | ---
**IE Name** | `http.redir.domain`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.server`

Attribute | Value
--- | ---
**IE Name** | `http.redir.server`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.port`

Attribute | Value
--- | ---
**IE Name** | `http.redir.port`
**Tier** | ``
**Data Type** | `unsigned`
**Semantic** | `identifier`
**Reference** | []()
**Description** | 

### `http.redir.path`

Attribute | Value
--- | ---
**IE Name** | `http.redir.path`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.fragment`

Attribute | Value
--- | ---
**IE Name** | `http.redir.fragment`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.query`

Attribute | Value
--- | ---
**IE Name** | `http.redir.query`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.user`

Attribute | Value
--- | ---
**IE Name** | `http.redir.user`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.redir.password`

Attribute | Value
--- | ---
**IE Name** | `http.redir.password`
**Tier** | ``
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

## `http.headers`

Attribute | Value
--- | ---
**IE Name** | `http.headers`
**Tier** | `common`
**Data Type** | `unsigned
**Semantic** | `quantity
Unit | values
**Description** | A count of headers in the HTTP request or response message.

### `http.cache_control`

Attribute | Value
--- | ---
**IE Name** | `http.cache_control`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7234: Hypertext Transfer Protocol (HTTP/1.1): Caching](https://tools.ietf.org/html/rfc7234)
**Description** | The `Cache-Control` HTTP header holds *directives* (instructions) for caching in both requests and responses. A given directive in a request does not mean the same directive should be in the response.

### `http.connection`

Attribute | Value
--- | ---
**IE Name** | `http.connection`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Connection
**Description** | The `Connection` general header controls whether or not the network connection stays open after the current transaction finishes. If the value sent is `keep-alive`, the connection is persistent and not closed, allowing for subsequent requests to the same server to be done.

## `http.content_type`

Attribute | Value
--- | ---
**IE Name** | `http.content_type`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 3.1.1.5: Content-Type](https://tools.ietf.org/html/rfc7231#section-3.1.1.5)
**Description** | The `Content-Type` entity header is used to indicate the media type of the resource.

## `http.content_encoding`

Attribute | Value
--- | ---
**IE Name** | `http.content_encoding`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 3.1.2.2: Content-Encoding](https://tools.ietf.org/html/rfc7231#section-3.1.2.2)
**Description** | The `Content-Encoding` entity header is used to compress the media-type. When present, its value indicates which encodings were applied to the entity-body.

## `http.content_language`

Attribute | Value
--- | ---
**IE Name** | ` http.content_language`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 3.1.3.2: Content-Language](https://tools.ietf.org/html/rfc7231#section-3.1.3.2)
**Description** | The `Content-Language` entity header is used to describe the language(s) intended for the audience, so that it allows a user to differentiate according to the users' own preferred language.

## `http.content_location`

Attribute | Value
--- | ---
**IE Name** | `http.content_location`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 3.1.4.2: Content-Location](https://tools.ietf.org/html/rfc7231#section-3.1.4.2)
**Description** | The `Content-Location` header indicates an alternate location for the returned data. The principal use is to indicate the URL of a resource transmitted as the result of content negotiation.

## `http.content_length`

Attribute | Value
--- | ---
**IE Name** | `http.content_length`
**Tier** | `common`
**Data Type** | `unsigned`
**Semantic** | `quantity`
**Unit** | `bytes`
**Reference** | [RFC 7230, section 3.3.2: Content-Length](https://tools.ietf.org/html/rfc7230#section-3.3.2)
**Description** | The `Content-Length` entity header indicates the size of the entity-body, in bytes, sent to the recipient.

## `http.content_md5`

Attribute | Value
--- | ---
**IE Name** | `http.content_md5`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

## `http.content_range`

Attribute | Value
--- | ---
**IE Name** | `http.content_range`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7233, section 4.2: Content-Range](https://tools.ietf.org/html/rfc7233#section-4.2)
**Description** | The `Content-Range` response HTTP header indicates where in a full body message a partial message belongs.

## `http.date`

Attribute | Value
--- | ---
**IE Name** | `http.date`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `httpdate`
**Reference** | [RFC 7231, section 7.1.1.2: Date](https://tools.ietf.org/html/rfc7231#section-7.1.1.2)
**Description** | The `Date` general HTTP header contains the date and time at which the message was originated.

## `http.link`

Attribute | Value
--- | ---
**IE Name** | `http.link`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 8288, section 3: Link Serialisation in HTTP Headers](https://tools.ietf.org/html/rfc8288#section-3)
**Description** | The HTTP `Link` entity-header field provides a means for serialising one or more links in HTTP headers. It is semantically equivalent to the HTML `<link>` element.

## `http.pragma`

Attribute | Value
--- | ---
**IE Name** | `http.pragma`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7234, section 5.4: Pragma](https://tools.ietf.org/html/rfc7234#section-5.4)
**Description** | The `Pragma` HTTP/1.0 general header is an implementation-specific header that may have various effects along the request-response chain. It is used for backwards compatibility with HTTP/1.0 caches where the `Cache-Control` HTTP/1.1 header is not yet present.

## `http.trailer`

Attribute | Value
--- | ---
**IE Name** | `http.trailer`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

## `http.transfer_encoding`

Attribute | Value
--- | ---
**IE Name** | `http.transfer_encoding`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

## `http.req`

### `http.req.timestamp`

Attribute | Value
--- | ---
**IE Name** | `http.req.timestamp`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.req.method`

Attribute | Value
--- | ---
**IE Name** | `http.req.method`
**Tier** | `core`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.bytes`

Attribute | Value
--- | ---
**IE Name** | `http.req.bytes`
**Tier** | `common`
**Data Type** | `unsigned
**Semantic** | `quantity
**Unit** | `bytes`
**Reference** | []()
**Description** | 

### `http.req.a_im`

Attribute | Value
--- | ---
**IE Name** | `http.req.a_im`
**Tier** | `
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.req.accept`

Attribute | Value
--- | ---
**IE Name** | `http.req.accept`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 5.3.2: Accept](https://tools.ietf.org/html/rfc7231#section-5.3.2)
**Description** | The `Accept` request header advertises which content types, expressed as MIME types, the client is able to understand.

### `http.req.accept_charset`

Attribute | Value
--- | ---
**IE Name** | `http.req.accept_charset`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 5.3.3: Accept-Charset](https://tools.ietf.org/html/rfc7231#section-5.3.3)
**Description** | The `Accept-Charset` request header advertises which character encodings the client understands.

### `http.req.accept_datetime`

Attribute | Value
--- | ---
**IE Name** | `http.req.accept_datetime`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `httpdate
**Reference** | []()
**Description** | 

### `http.req.accept_encoding`

Attribute | Value
--- | ---
**IE Name** | `http.req.accept_encoding`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 5.3.4: Accept-Encoding](https://tools.ietf.org/html/rfc7231#section-5.3.4)
**Description** | The `Accept-Encoding` request header advertises which content encoding, usually a compression algorithm, the client is able to understand.

### `http.req.accept_language`

Attribute | Value
--- | ---
**IE Name** | `http.req.accept_language`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 5.3.5: Accept-Language](https://tools.ietf.org/html/rfc7231#section-5.3.5)
**Description** | The `Accept-Language` request header advertises which languages the client is able to understand, and which locale variant is preferred. (By languages, we mean natural languages, such as English, and not programming languages.)

### `http.req.access_control_request_headers`

Attribute | Value
--- | ---
**IE Name** | `http.req.access_control_request_headers`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://fetch.spec.whatwg.org/#http-access-control-request-headers
**Description** | The `Access-Control-Request-Headers` request header is used by browsers when issuing a preflight request, to let the server know which HTTP headers the client might send when the actual request is made.

### `http.req.access_control_request_method`

Attribute | Value
--- | ---
**IE Name** | `http.req.access_control_request_method`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://fetch.spec.whatwg.org/#http-access-control-request-method
**Description** | The `Access-Control-Request-Method` request header is used by browsers when issuing a preflight request, to let the server know which HTTP method will be used when the actual request is made. This header is necessary as the preflight request is always an `OPTIONS` and doesn't use the same method as the actual request.

### `http.req.authorization`

Attribute | Value
--- | ---
**IE Name** | `http.req.authorization`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7235, section 4.2: Authorization](https://tools.ietf.org/html/rfc7235#section-4.2)
**Description** | The HTTP `Authorization` request header contains the credentials to authenticate a user agent with a server, usually, but not necessarily, after the server has responded with a `401 Unauthorized` status and the `WWW-Authenticate` header.

### `http.req.cookie`

Attribute | Value
--- | ---
**IE Name** | `http.req.cookie`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 6265, section 5.4: Cookie](https://tools.ietf.org/html/rfc6265#section-5.4)
**Description** | The `Cookie` HTTP request header contains stored HTTP cookies previously sent by the server with the `Set-Cookie` header.

### `http.req.cookie2`

Attribute | Value
--- | ---
**IE Name** | `http.req.cookie2`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 2965: Cookie2](https://tools.ietf.org/html/rfc2965)
**Description** | The obsolete `Cookie2` HTTP request header used to advise the server that the user agent understands *new-style* cookies, but nowadays user agents will use the `Cookie` header instead, not this one.

### `http.req.device_memory`

Attribute | Value
--- | ---
**IE Name** | `http.req.device_memory`
**Tier** | `common`
**Data Type** | `unsigned
**Semantic** | `quantity
Units | gibibytes
**Reference** | [Device Memory 1](https://w3c.github.io/device-memory/#sec-device-memory-client-hint-header)
**Description** | The `Device-Memory` header is a Device Memory API header that works like Client Hints header which represents the approximate amount of RAM client device has.

### `http.req.dnt`

Attribute | Value
--- | ---
**IE Name** | `http.req.dnt`
**Tier** | `common`
**Data Type** | `unsigned
**Semantic** | `indicator
**Reference** | [Tracking Preference Expression (DNT)](https://www.w3.org/TR/tracking-dnt/#dnt-header-field)
**Description** | The `DNT` (Do Not Track) request header indicates the user's tracking preference. It lets users indicate whether they would prefer privacy rather than personalized content.

### `http.req.dpr`

Attribute | Value
--- | ---
**IE Name** | `http.req.dpr`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/DPR
**Description** | The `DPR` header is a Client Hints headers which represents the client device pixel ratio (DPR), which is the the number of physical device pixels corresponding to every CSS pixel.

### `http.req.early_data`

Attribute | Value
--- | ---
**IE Name** | `http.req.early_data`
**Tier** | `common`
**Data Type** | `unsigned`
**Semantic** | `identifier`
**Reference** | [RFC 8470, section 5.1: The Early-Data Header Field]()
**Description** | The `Early-Data` header is set by an intermediary to indicate that the request has been conveyed in TLS early data, and also indicates that the intermediary understands the `425 (Too Early)` status code.

### `http.req.expect`

Attribute | Value
--- | ---
**IE Name** | `http.req.expect`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 5.1.1: Expect](https://tools.ietf.org/html/rfc7231#section-5.1.1)
**Description** | The `Expect` HTTP request header indicates expectations that need to be fulfilled by the server in order to properly handle the request.

### `http.req.forwarded`

Attribute | Value
--- | ---
**IE Name** | `http.req.forwarded`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7239, section 4: Forwarded](https://tools.ietf.org/html/rfc7239#section-4)
**Description** | The `Forwarded` header contains information from the client-facing side of proxy servers that is altered or lost when a proxy is involved in the path of the request.

### `http.req.from`

Attribute | Value
--- | ---
**IE Name** | `http.req.from`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `emailaddress`
**Reference** | [RFC 7231, section 5.5.1: From](https://tools.ietf.org/html/rfc7231#section-5.5.1)
**Description** | The `From` request header contains an Internet email address for a human user who controls the requesting user agent.

### `http.req.front_end_https`

Attribute | Value
--- | ---
**IE Name** | `http.req.front_end_https`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.host`

Attribute | Value
--- | ---
**IE Name** | `http.req.host`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7230, section 5.4: Host](https://tools.ietf.org/html/rfc7230#section-5.4)
**Description** | The `Host` request header specifies the host and port number of the server to which the request is being sent. If no port is included, the default port for the service requested (e.g., 443 for an HTTPS URL, and 80 for an HTTP URL) is implied.

### `http.req.http2_settings`

Attribute | Value
--- | ---
**IE Name** | `http.req.http2_settings`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.if_match`

Attribute | Value
--- | ---
**IE Name** | `http.req.if_match`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7232, section 3.1: If-Match](https://tools.ietf.org/html/rfc7232#section-3.1)
**Description** | The `If-Match` HTTP request header makes the request conditional. For `GET` and `HEAD` methods, the server will send back the requested resource only if it matches one of the listed `ETag`s. For `PUT` and other non-safe methods, it will only upload the resource in this case.

### `http.req.if_modified_since`

Attribute | Value
--- | ---
**IE Name** | `http.req.if_modified_since`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `httpdate`
**Reference** | [RFC 7232, section 3.3: If-Modified-Since](https://tools.ietf.org/html/rfc7232#section-3.3)
**Description** | The `If-Modified-Since` request HTTP header makes the request conditional: the server will send back the requested resource, with a `200` status, only if it has been last modified after the given date.

### `http.req.if_none_match`

Attribute | Value
--- | ---
**IE Name** | `http.req.if_none_match`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7232, section 3.2: If-None-Match](https://tools.ietf.org/html/rfc7232#section-3.2)
**Description** | The `If-None-Match` HTTP request header makes the request conditional. For `GET` and `HEAD` methods, the server will send back the requested resource, with a `200` status, only if it doesn't have an `ETag` matching the given ones. For other methods, the request will be processed only if the eventually existing resource's `ETag` doesn't match any of the values listed.

### `http.req.if_range`

Attribute | Value
--- | ---
**IE Name** | `http.req.if_range`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7233, section 3.2: If-Range](https://tools.ietf.org/html/rfc7233#section-3.2)
**Description** | The `If-Range` HTTP request header makes a range request conditional: if the condition is fulfilled, the range request will be issued and the server sends back a `206 Partial Content` answer with the appropriate body. If the condition is not fulfilled, the full resource is sent back, with a `200 OK` status.

### `http.req.if_unmodified_since`

Attribute | Value
--- | ---
**IE Name** | `http.req.if_unmodified_since`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7232, section 3.4: If-Unmodified-Since](https://tools.ietf.org/html/rfc7232#section-3.4)
**Description** | The `If-Unmodified-Since` request HTTP header makes the request conditional: the server will send back the requested resource, or accept it in the case of a `POST` or another non-safe method, only if it has not been last modified after the given date. If the resource has been modified after the given date, the response will be a `412 (Precondition Failed)` error.

### `http.req.keep_alive`

Attribute | Value
--- | ---
**IE Name** | `http.req.keep_alive`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7230, appendix A.1.2: Keep-Alive](https://tools.ietf.org/html/rfc7230#appendix-A.1.2)
**Description** | The `Keep-Alive` general header allows the sender to hint about how the connection may be used to set a timeout and a maximum amount of requests.

### `http.req.max_forwards`

Attribute | Value
--- | ---
**IE Name** | `http.req.max_forwards`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.req.origin`

Attribute | Value
--- | ---
**IE Name** | `http.req.origin`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [https://fetch.spec.whatwg.org/#origin-header](https://fetch.spec.whatwg.org/#origin-header)
**Description** | The `Origin` request header indicates where a fetch originates from. It doesn't include any path information, but only the server name. It is sent with `CORS` requests, as well as with `POST` requests. It is similar to the `Referer` header, but, unlike this header, it doesn't disclose the whole path.

### `http.req.proxy_authorization`

Attribute | Value
--- | ---
**IE Name** | `http.req.proxy_authorization`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.proxy_connection`

Attribute | Value
--- | ---
**IE Name** | `http.req.proxy_connection`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.range`

Attribute | Value
--- | ---
**IE Name** | `http.req.range`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.referer`

#### `http.req.referer.uri`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.uri`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.ip`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.ip`
**Tier** | `custom`
**Data Type** | `ipaddress`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.scheme`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.scheme`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.domain`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.domain`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.server`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.server`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.port`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.port`
**Tier** | `custom`
**Data Type** | `unsigned`
**Semantic** | `identifier`
**Reference** | []()
**Description** | 

#### `http.req.referer.path`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.path`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.fragment`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.fragment`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.query`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.query`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.user`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.user`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.referer.password`

Attribute | Value
--- | ---
**IE Name** | `http.req.referer.password`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.save_data`

Attribute | Value
--- | ---
**IE Name** | `http.req.save_data`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.te`

Attribute | Value
--- | ---
**IE Name** | `http.req.te`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.upgrade`

Attribute | Value
--- | ---
**IE Name** | `http.req.upgrade`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.upgrade_insecure_requests`

Attribute | Value
--- | ---
**IE Name** | `http.req.upgrade_insecure_requests`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.user_agent`

#### `http.req.user_agent.agent`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.agent`
**Tier** | `core`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.device`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.device`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.os`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.os`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.os_ver`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.os_ver`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.os_major`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.os_major`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.os_minor`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.os_minor`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.os_build`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.os_build`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.sw`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.sw`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.sw_ver`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.sw_ver`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.sw_major`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.sw_major`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.sw_minor`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.sw_minor`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.user_agent.sw_build`

Attribute | Value
--- | ---
**IE Name** | `http.req.user_agent.sw_build`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.via`

Attribute | Value
--- | ---
**IE Name** | `http.req.via`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.warning`

Attribute | Value
--- | ---
**IE Name** | `http.req.warning`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_att_deviceid`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_att_deviceid`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_attribute`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_attribute`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_attribute_cacheability`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_attribute_cacheability`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_attribute_prefix`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_attribute_prefix`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_auth`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_auth`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_authenticated_groups`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_authenticated_groups`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_authenticated_user`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_authenticated_user`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_bluecoat_via`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_bluecoat_via`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_client_ip`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_client_ip`
**Tier** | `common`
**Data Type** | `ipaddress`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_content_digest`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_content_digest`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_correlation_id`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_correlation_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_csrf_token`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_csrf_token`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_device_id`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_device_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_flash_version`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_flash_version`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_forwarded_for`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_forwarded_for`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_forwarded_host`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_forwarded_host`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_forwarded_proto`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_forwarded_proto`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_forwarded_server`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_forwarded_server`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_http_method_override`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_http_method_override`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_icap_profile`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_icap_profile`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_idfa`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_idfa`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_idfv`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_idfv`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_nonce`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_nonce`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_organization_id`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_organization_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_profile`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_profile`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_profile_token`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_profile_token`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_request_id`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_request_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_requested_with`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_requested_with`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_server_ip`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_server_ip`
**Tier** | `common`
**Data Type** | `ipaddress`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_subscriber_id`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_subscriber_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_time`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_time`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `httpdate
**Reference** | []()
**Description** | 

### `http.req.x_uidh`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_uidh`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_user_agent`

#### `http.req.x_user_agent.agent`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.agent`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.device`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.device`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.os`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.os`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.os_ver`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.os_ver`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.os_major`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.os_major`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.os_minor`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.os_minor`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.os_build`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.os_build`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.sw`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.sw`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.sw_ver`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.sw_ver`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.sw_major`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.sw_major`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.sw_minor`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.sw_minor`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

#### `http.req.x_user_agent.sw_build`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_user_agent.sw_build`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.req.x_wap_profile`

Attribute | Value
--- | ---
**IE Name** | `http.req.x_wap_profile`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.timestamp`

Attribute | Value
--- | ---
**IE Name** | `http.resp.timestamp`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.resp.status`

Attribute | Value
--- | ---
**IE Name** | `http.resp.status`
**Tier** | `core`
**Data Type** | `unsigned`
**Semantic** | `identifier`
**Reference** | []()
**Description** | 

### `http.resp.reason_phrase`

Attribute | Value
--- | ---
**IE Name** | `http.resp.reason_phrase`
**Tier** | `core`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.bytes`

Attribute | Value
--- | ---
**IE Name** | `http.resp.bytes`
**Tier** | `common`
**Data Type** | `unsigned`
**Semantic** | `quantity`
**Unit** | `bytes`
**Reference** | []()
**Description** | 

### `http.resp.time`

Attribute | Value
--- | ---
**IE Name** | `http.resp.time`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `httpdate`
**Reference** | []()
**Description** | 

### `http.resp.accept_ch`

Attribute | Value
--- | ---
**IE Name** | `http.resp.accept_patch`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-CH
**Description** | The `Accept-CH` response header is set by the server to specify which Client Hints headers a client should include in subsequent requests.

### `http.resp.accept_ch_lifetime`

Attribute | Value
--- | ---
**IE Name** | `http.resp.accept_ch_lifetime`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-CH-Lifetime
**Description** | The `Accept-CH-Lifetime` response header is set by the server to specify the persistence of Accept-CH header value that specifies for which Client Hints headers client should include in subsequent requests.

### `http.resp.accept_patch`

Attribute | Value
--- | ---
**IE Name** | `http.resp.accept_patch`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 5789, section 3.1: Accept-Patch](https://tools.ietf.org/html/rfc5789#section-3.1)
**Description** | The `Accept-Patch` response header advertises which media-type the server is able to understand.

### `http.resp.accept_ranges`

Attribute | Value
--- | ---
**IE Name** | `http.resp.accept_ranges`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7233, section 2.3: Accept-Ranges](https://tools.ietf.org/html/rfc7233#section-2.3)
**Description** | The `Accept-Ranges` response HTTP header is a marker used by the server to advertise its support of partial requests. The value of this field indicates the unit that can be used to define a range.

### `http.resp.access_control_allow_credentials`

Attribute | Value
--- | ---
**IE Name** | `http.resp.access_control_allow_credentials`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://fetch.spec.whatwg.org/#http-access-control-allow-credentials
**Description** | The `Access-Control-Allow-Credentials` response header tells browsers whether to expose the response to frontend JavaScript code when the request's credentials mode is `include`.

### `http.resp.access_control_allow_headers`

Attribute | Value
--- | ---
**IE Name** | `http.resp.access_control_allow_headers`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://fetch.spec.whatwg.org/#http-access-control-allow-headers
**Description** | The `Access-Control-Allow-Headers` response header is used in response to a preflight request which includes `Access-Control-Request-Headers` to indicate which HTTP headers can be used during the actual request.

### `http.resp.access_control_allow_methods`

Attribute | Value
--- | ---
**IE Name** | `http.resp.access_control_allow_methods`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://fetch.spec.whatwg.org/#http-access-control-allow-methods
**Description** | The `Access-Control-Allow-Methods` response header specifies the method or methods allowed when accessing the resource in response to a preflight request.

### `http.resp.access_control_allow_origin`

Attribute | Value
--- | ---
**IE Name** | `http.resp.access_control_allow_origin`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://fetch.spec.whatwg.org/#http-access-control-allow-origin
**Description** | The `Access-Control-Allow-Origin` response header indicates whether the response can be shared with requesting code from the given origin.

### `http.resp.access_control_expose_headers`

Attribute | Value
--- | ---
**IE Name** | `http.resp.access_control_expose_headers`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://fetch.spec.whatwg.org/#http-access-control-expose-headers
**Description** | The `Access-Control-Expose-Headers` response header indicates which headers can be exposed as part of the response by listing their names.

### `http.resp.access_control_max_age`

Attribute | Value
--- | ---
**IE Name** | `http.resp.access_control_max_age`
**Tier** | `common`
**Data Type** | `unsigned`
**Semantic** | `quantity`
**Unit** | `seconds`
**Reference** | https://fetch.spec.whatwg.org/#http-access-control-max-age
**Description** | The `Access-Control-Max-Age` response header indicates how long the results of a preflight request (that is the information contained in the `Access-Control-Allow-Methods` and `Access-Control-Allow-Headers` headers) can be cached.

### `http.resp.age`

Attribute | Value
--- | ---
**IE Name** | `http.resp.age`
**Tier** | `common`
**Data Type** | `unsigned`
**Semantic** | `quantity`
**Unit** | `seconds`
**Reference** | [RFC 7234, section 5.1: Age](https://tools.ietf.org/html/rfc7234#section-5.1)
**Description** | The `Age` header contains the time in seconds the object has been in a proxy cache.

### `http.resp.allow`

Attribute | Value
--- | ---
**IE Name** | `http.resp.allow`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 7.4.1: Allow](https://tools.ietf.org/html/rfc7231#section-7.4.1)
**Description** | The `Allow` header lists the set of methods supported by a resource.

### `http.resp.alt_svc`

Attribute | Value
--- | ---
**IE Name** | `http.resp.alt_svc`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7838](https://tools.ietf.org/html/rfc7838)
**Description** | The `Alt-Svc` HTTP response header is used to advertise alternative services through which the same resource can be reached. An alternative service is defined by a protocol/host/port combination.

### `http.resp.clear_site_data`

Attribute | Value
--- | ---
**IE Name** | `http.resp.clear_site_data`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Clear Site Data](https://w3c.github.io/webappsec-clear-site-data)
**Description** | The `Clear-Site-Data` header clears browsing data (cookies, storage, cache) associated with the requesting website. It allows web developers to have more control over the data stored locally by a browser for their origins.

### `http.resp.content_disposition`

Attribute | Value
--- | ---
**IE Name** | `http.resp.content_disposition`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 6266](https://tools.ietf.org/html/rfc6266)
**Description** | In a regular HTTP response, the `Content-Disposition` response header is a header indicating if the content is expected to be displayed inline in the browser, that is, as a Web page or as part of a Web page, or as an attachment, that is downloaded and saved locally.

### `http.resp.content_security_policy`

Attribute | Value
--- | ---
**IE Name** | `http.resp.content_security_policy`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Content Security Policy Level 3](https://w3c.github.io/webappsec-csp/)
**Description** | The HTTP `Content-Security-Policy` response header allows web site administrators to control resources the user agent is allowed to load for a given page.

### `http.resp.content_security_policy_report_only`

Attribute | Value
--- | ---
**IE Name** | `http.resp.content_security_policy_report_only`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Content Security Policy Level 3](https://w3c.github.io/webappsec-csp/)
**Description** | The HTTP `Content-Security-Policy-Report-Only` response header allows web developers to experiment with policies by monitoring (but not enforcing) their effects.

### `http.resp.cross_origin_resource_policy`

Attribute | Value
--- | ---
**IE Name** | `http.resp.cross_origin_resource_policy`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | https://fetch.spec.whatwg.org/#cross-origin-resource-policy-header
**Description** | The HTTP `Cross-Origin-Resource-Policy` response header conveys a desire that the browser blocks no-cors cross-origin/cross-site requests to the given resource.

### `http.resp.date`

Attribute | Value
--- | ---
**IE Name** | `http.resp.date`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `httpdate
**Reference** | []()
**Description** | 

### `http.resp.delta_base`

Attribute | Value
--- | ---
**IE Name** | `http.resp.delta_base`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.resp.digest`

Attribute | Value
--- | ---
**IE Name** | `http.resp.digest`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [draft-ietf-httpbis-digest-headers-latest](https://datatracker.ietf.org/doc/draft-ietf-httpbis-digest-headers)
**Description** | The `Digest` response HTTP header provides a digest of the requested resource.

### `http.resp.etag`

Attribute | Value
--- | ---
**IE Name** | `http.resp.etag`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7232, section 2.3: ETag](https://tools.ietf.org/html/rfc7232#section-2.3)
**Description** | The `ETag` HTTP response header is an identifier for a specific version of a resource. It lets caches be more efficient and save bandwidth, as a web server does not need to resend a full response if the content has not changed.

### `http.resp.expect_ct`

Attribute | Value
--- | ---
**IE Name** | `http.resp.expect_ct`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Expect-CT Extension for HTTP](https://tools.ietf.org/html/draft-ietf-httpbis-expect-ct-08)
**Description** | The `Expect-CT` header lets sites opt in to reporting and/or enforcement of Certificate Transparency requirements, to prevent the use of misissued certificates for that site from going unnoticed.

### `http.resp.expires`

Attribute | Value
--- | ---
**IE Name** | `http.resp.expires`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `httpdate`
**Reference** | [RFC 7234, section 5.3: Expires](https://tools.ietf.org/html/rfc7234#section-5.3)
**Description** | The `Expires` header contains the date/time after which the response is considered stale. Invalid dates, like the value `0`, represent a date in the past and mean that the resource is already expired.

### `http.resp.feature_policy`

Attribute | Value
--- | ---
**IE Name** | `http.resp.feature_policy`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Feature Policy](https://w3c.github.io/webappsec-feature-policy/#feature-policy-http-header-field)
**Description** | The HTTP `Feature-Policy` header provides a mechanism to allow and deny the use of browser features in its own frame, and in content within any `<iframe>` elements in the document.

### `http.resp.im`

Attribute | Value
--- | ---
**IE Name** | `http.resp.im`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.resp.keep_alive`

Attribute | Value
--- | ---
**IE Name** | `http.resp.keep_alive`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.resp.large_allocation`

Attribute | Value
--- | ---
**IE Name** | `http.resp.large_allocation`
**Tier** | `custom`
**Data Type** | `unsigned`
**Semantic** | `quantity`
**Unit** | `megabytes`
**Reference** | [https://gist.github.com/mystor/5739e222e398efc6c29108be55eb6fe3](https://gist.github.com/mystor/5739e222e398efc6c29108be55eb6fe3)
**Description** | The non-standard `Large-Allocation` response header tells the browser that the page being loaded is going to want to perform a large allocation. It is currently only implemented in Firefox, but is harmless to send to every browser.

### `http.resp.last_modified`

Attribute | Value
--- | ---
**IE Name** | `http.resp.last_modified`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `httpdate`
**Reference** | [RFC 7232, section 2.2: Last-Modified](https://tools.ietf.org/html/rfc7232#section-2.2)
**Description** | The `Last-Modified` response HTTP header contains the date and time at which the origin server believes the resource was last modified. It is used as a validator to determine if a resource received or stored is the same. Less accurate than an `ETag` header, it is a fallback mechanism. Conditional requests containing `If-Modified-Since` or `If-Unmodified-Since` headers make use of this field.

### `http.resp.location`

Attribute | Value
--- | ---
**IE Name** | `http.resp.location`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7231, section 7.1.2: Location](https://tools.ietf.org/html/rfc7231#section-7.1.2)
**Description** | The `Location` response header indicates the URL to redirect a page to. It only provides a meaning when served with a 3xx (redirection) or 201 (created) status response.

### `http.resp.nel`

Attribute | Value
--- | ---
**IE Name** | `http.resp.nel`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Network Error Logging](https://w3c.github.io/network-error-logging/#nel-response-header), [Network Error Logging (NEL) explainer](https://developer.mozilla.org/en-US/docs/Web/HTTP/Network_Error_Logging)
**Description** | The HTTP `NEL` response header is used to configure network request logging.

### `http.resp.p3p`

Attribute | Value
--- | ---
**IE Name** | `http.resp.p3p`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.proxy_authenticate`

Attribute | Value
--- | ---
**IE Name** | `http.resp.proxy_authenticate`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 7235, section 4.3: Proxy-Authenticate](https://tools.ietf.org/html/rfc7235#section-4.3)
**Description** | The HTTP `Proxy-Authenticate` response header defines the authentication method that should be used to gain access to a resource behind a proxy server. It authenticates the request to the proxy server, allowing it to transmit the request further.

### `http.resp.public_key_pins`

Attribute | Value
--- | ---
**IE Name** | `http.resp.public_key_pins`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.public_key_pins_report_only`

Attribute | Value
--- | ---
**IE Name** | `http.resp.public_key_pins_report_only`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.referrer_policy`

Attribute | Value
--- | ---
**IE Name** | `http.resp.referrer_policy`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.refresh`

Attribute | Value
--- | ---
**IE Name** | `http.resp.refresh`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.retry_after`

Attribute | Value
--- | ---
**IE Name** | `http.resp.retry_after`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.resp.sec_websocket_accept`

Attribute | Value
--- | ---
**IE Name** | `http.resp.sec_websocket_accept`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.server`

Attribute | Value
--- | ---
**IE Name** | `http.resp.server`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.server_timing`

Attribute | Value
--- | ---
**IE Name** | `http.resp.server_timing`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.resp.set_cookie`

Attribute | Value
--- | ---
**IE Name** | `http.resp.set_cookie`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.set_cookie2`

Attribute | Value
--- | ---
**IE Name** | `http.resp.set_cookie2`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.sourcemap`

Attribute | Value
--- | ---
**IE Name** | `http.resp.sourcemap`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.strict_transport_security`

Attribute | Value
--- | ---
**IE Name** | `http.resp.strict_transport_security`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.timing_allow_origin`

Attribute | Value
--- | ---
**IE Name** | `http.resp.timing_allow_origin`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.tk`

Attribute | Value
--- | ---
**IE Name** | `http.resp.tk`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.upgrade`

Attribute | Value
--- | ---
**IE Name** | `http.resp.upgrade`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.vary`

Attribute | Value
--- | ---
**IE Name** | `http.resp.vary`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.via`

Attribute | Value
--- | ---
**IE Name** | `http.resp.via`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.warning`

Attribute | Value
--- | ---
**IE Name** | `http.resp.warning`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.www_authenticate`

Attribute | Value
--- | ---
**IE Name** | `http.resp.www_authenticate`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_attribute`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_attribute`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_attribute_cacheability`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_attribute_cacheability`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_attribute_prefix`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_attribute_prefix`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_authenticated_groups`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_authenticated_groups`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_authenticated_user`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_authenticated_user`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_client_ip`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_client_ip`
**Tier** | `common`
**Data Type** | `ipaddress`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_content_duration`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_content_duration`
**Tier** | `common`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.resp.x_content_security_policy`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_content_security_policy`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_content_type_options`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_content_type_options`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_correlation_id`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_correlation_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_dns_prefetch_control`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_dns_prefetch_control`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_frame_options`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_frame_options`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_icap_profile`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_icap_profile`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_infection_found`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_infection_found`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_powered_by`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_powered_by`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_request_id`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_request_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_response_desc`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_response_desc`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_response_info`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_response_info`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_server_ip`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_server_ip`
**Tier** | `common`
**Data Type** | `ipaddress`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_subscriber_id`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_subscriber_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_ua_compatible`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_ua_compatible`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_violations_found`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_violations_found`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_virus_id`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_virus_id`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_webkit_csp`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_webkit_csp`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

### `http.resp.x_xss_protection`

Attribute | Value
--- | ---
**IE Name** | `http.resp.x_xss_protection`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | []()
**Description** | 

## `http.event`

### `http.event.client_load_start`

Attribute | Value
--- | ---
**IE Name** | `http.event.client_load_start`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.event.client_load_end`

Attribute | Value
--- | ---
**IE Name** | `http.event.client_load_end`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.event.client_render_start`

Attribute | Value
--- | ---
**IE Name** | `http.event.client_render_start`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.event.client_render_end`

Attribute | Value
--- | ---
**IE Name** | `http.event.client_render_end`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.event.req`

#### `http.event.req.first_byte_in`

Attribute | Value
--- | ---
**IE Name** | `http.event.req.first_byte_in`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

#### `http.event.req.first_byte_out`

Attribute | Value
--- | ---
**IE Name** | `http.event.req.first_byte_out`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

#### `http.event.req.last_byte_in`

Attribute | Value
--- | ---
**IE Name** | `http.event.req.last_byte_in`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

#### `http.event.req.last_byte_out`

Attribute | Value
--- | ---
**IE Name** | `http.event.req.last_byte_out`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

### `http.event.resp`

#### `http.event.resp.first_byte_in`

Attribute | Value
--- | ---
**IE Name** | `http.event.resp.first_byte_in`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

#### `http.event.resp.first_byte_out`

Attribute | Value
--- | ---
**IE Name** | `http.event.resp.first_byte_out`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

#### `http.event.resp.last_byte_in`

Attribute | Value
--- | ---
**IE Name** | `http.event.resp.last_byte_in`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 

#### `http.event.resp.last_byte_out`

Attribute | Value
--- | ---
**IE Name** | `http.event.resp.last_byte_out`
**Tier** | `custom`
**Data Type** | ``
**Semantic** | ``
**Unit** | ``
**Reference** | []()
**Description** | 
