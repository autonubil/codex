# host Information Elements

## `host`

The [host](https://tools.ietf.org/html/rfc3986#section-3.2.2) is an identifier by an IP literal encapsulated within square brackets, an IPv4 address in dotted-decimal form, or a registered name.

The `host` object may be contained with other parent objects, such as a `uri`.

### `host.name`

Attribute | Value
--- | ---
**IE Name** | `host.name`
**Tier** | `core`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 3986, section 3.2.2: host](https://tools.ietf.org/html/rfc3986#section-3.2.2)
**Description** | An identifier by an IP literal encapsulated within square brackets, an IPv4 address in dotted-decimal form, or a registered name.

### `host.ip`

Attribute | Value
--- | ---
**IE Name** | `host.ip`
**Tier** | `common`
**Data Type** | `ipaddress`
**Semantic** | `default`
**Description** | If `host.name` is an IP address, this field would contain that address. Otherwise it should contain the IP address obtained by resolving `host.name` to an IP address.

### `host.hostname`

Attribute | Value
--- | ---
**IE Name** | `host.hostname`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 1034, section 3: DOMAIN NAME SPACE and RESOURCE RECORDS](https://tools.ietf.org/html/rfc1034#section-3)
**Description** | This IE contains a label that is assigned to a resource connected to a computer network and that is used to identify the resource. It is the final (left-most) label in the DNS resource record for this resource. This value is commonly assigned in the configuration of the resource itself as its `hostname`.

### `host.fqdn`

Attribute | Value
--- | ---
**IE Name** | `host.fqdn`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 1034, section 3: DOMAIN NAME SPACE and RESOURCE RECORDS](https://tools.ietf.org/html/rfc1034#section-3)
**Description** | This IE contains the fully qualified domain name of the host indicated by `host.name`. It can usually be obtained via DNS. A fully qualified domain name consists of a list of domain labels representing the hierarchy from the lowest relevant level in the DNS to the top-level domain (TLD). The domain labels are concatenated using the full stop `.` character (dot or period) as a separator between labels.

### `host.tld`

Attribute | Value
--- | ---
**IE Name** | `host.tld`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 1591, section 2: The Top Level Structure of the Domain Names](https://tools.ietf.org/html/rfc1591#section-2)
**Description** | The top-level domain under which the resource record of the host is defined. A top-level domain (TLD) is one of the domains at the highest level in the hierarchical Domain Name System of the Internet. The top-level domain names are installed in the root zone of the name space.

### `host.domain`

Attribute | Value
--- | ---
**IE Name** | `host.domain`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [iCANN: domain name](https://www.icann.org/icann-acronyms-and-terms/en/G0168)
**Description** | The registered domain under which the resource record of the host is defined. Registration of a domain name establishes a set of Start of Authority (SOA) records in the DNS servers of the parent domain.

### `host.subdomain`

Attribute | Value
--- | ---
**IE Name** | `host.subdomain`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [RFC 1034, section 3: DOMAIN NAME SPACE and RESOURCE RECORDS](https://tools.ietf.org/html/rfc1034#section-3)
**Description** | This information includes all labels from the fully qualified domain name (`host.fqdn`) excluding the final (left-most) label (`host.hostname`).
