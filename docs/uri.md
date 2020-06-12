# URI Information Elements

## `uri`

A Uniform Resource Identifier (URI - [RFC3986](https://tools.ietf.org/html/rfc3986)) is a string of characters that unambiguously identifies a particular resource. URIs are used throughout HTTP as the means for identifying resources ([RFC7231 - Section 2](https://tools.ietf.org/html/rfc7231#section-2)). URI references are used to target requests, indicate redirects, and define relationships.

The `uri` object may be contained with other parent objects, such as a `http.url`.

### `uri.ref`

Attribute | Value
--- | ---
**IE Name** | `uri.ref`
**Tier** | `core`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [URI Reference](https://tools.ietf.org/html/rfc3986#section-4.1)
**Description** | The complete Uniform Resource Identifier (URI). A URI-reference is either a URI or a relative reference.

### `uri.scheme`

Attribute | Value
--- | ---
**IE Name** | `uri.scheme`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Scheme](https://tools.ietf.org/html/rfc3986#section-3.1)
**Description** | Each URI begins with a scheme name that refers to a specification for assigning identifiers within that scheme. As such, the URI syntax is a federated and extensible naming system wherein each scheme's specification may further restrict the syntax and semantics of identifiers using that scheme. Examples are `http` and `https`.

### `uri.authority`

Attribute | Value
--- | ---
**IE Name** | `uri.authority`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 3986, section 3.2: Authority](https://tools.ietf.org/html/rfc3986#section-3.2)
**Description** | Many URI schemes include a hierarchical element for a naming authority. The generic syntax provides a common means for distinguishing an authority based on a registered name or server address, along with optional port and user information. The authority component is preceded by a double slash (`//`) and is terminated by the next slash (`/`), question mark (`?`), or number sign (`#`), or by the end of the URI.

### `uri.userinfo`

The userinfo subcomponent may consist of a user name and, optionally, scheme-specific information about how to gain authorization to access the resource. The user information, if present, is followed by a commercial at-sign ("@") that delimits it from the host.

#### `uri.userinfo.user`

Attribute | Value
--- | ---
**IE Name** | `uri.userinfo.user`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 3986, section 3.2.1: User Information](https://tools.ietf.org/html/rfc3986#section-3.2.1)
**Description** | The user name portion of the userinfo subcomponent.

#### `uri.userinfo.password`

Attribute | Value
--- | ---
**IE Name** | `uri.userinfo.password`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 3986, section 3.2.1: User Information](https://tools.ietf.org/html/rfc3986#section-3.2.1)
**Description** | The password portion of the userinfo subcomponent.

### `uri.host`

Attribute | Value
--- | ---
**IE Name** | `uri.host`
**Tier** | `custom`
**Data Type** | object: `host`
**Reference** | [RFC 3986, section 3.2.2: Host](https://tools.ietf.org/html/rfc3986#section-3.2.2)
**Description** | The host subcomponent of authority is identified by an IP literal encapsulated within square brackets, an IPv4 address in dotted-decimal form, or a registered name.

### `uri.port`

Attribute | Value
--- | ---
**IE Name** | `uri.port`
**Tier** | `custom`
**Data Type** | `unsigned`
**Semantic** | `identifier`
**Reference** | [RFC 3986, section 3.2.3: Port](https://tools.ietf.org/html/rfc3986#section-3.2.3)
**Description** | The port subcomponent of authority is designated by an optional port number in decimal following the host and delimited from it by a single colon (`:`) character. A scheme may define a default port. For example, the `http` scheme defines a default port of `80`, corresponding to its reserved TCP port number. The type of port designated by the port number (e.g., TCP, UDP, SCTP) is defined by the URI scheme.

### `uri.path`

Attribute | Value
--- | ---
**IE Name** | `uri.path`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 3986, section 3.3: Path](https://tools.ietf.org/html/rfc3986#section-3.3)
**Description** | The path component contains data, usually organized in hierarchical form, that, along with data in the non-hierarchical query component (`uri.query`), serves to identify a resource within the scope of the URI's scheme and naming authority (if any). The path is terminated by the first question mark (`?`) or number sign (`#`) character, or by the end of the URI.

### `uri.query`

Attribute | Value
--- | ---
**IE Name** | `uri.query`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 3986, section 3.4: Query](https://tools.ietf.org/html/rfc3986#section-3.4)
**Description** | The query component contains non-hierarchical data that, along with data in the path component (`uri.path`), serves to identify a resource within the scope of the URI's scheme and naming authority (if any). The query component is indicated by the first question mark (`?`) character and terminated by a number sign (`#`) character or by the end of the URI.

### `uri.fragment`

Attribute | Value
--- | ---
**IE Name** | `uri.fragment`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 3986, section 3.5: Fragment](https://tools.ietf.org/html/rfc3986#section-3.5)
**Description** | The fragment identifier component of a URI allows indirect identification of a secondary resource by reference to a primary resource and additional identifying information.  The identified secondary resource may be some portion or subset of the primary resource, some view on representations of the primary resource, or some other resource defined or described by those representations. A fragment identifier component is indicated by the presence of a number sign (`#`) character and terminated by the end of the URI.
