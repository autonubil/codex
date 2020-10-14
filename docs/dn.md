# dn (Distinguished Name)

A Distinguished Name (often referred to as a DN or FDN) is a string that uniquely identifies an entry in the directory information tree (DIT). A Distinguished Name is comprised of zero or more Relative Distinguished Name components that identify the location of the entry in the DIT.

## dn.dn

Attribute | Value
--- | ---
**IE Name** | dn.dn
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.7: distinguishedName](https://tools.ietf.org/html/rfc4519#section-2.7)
**Description** | Distinguished Name. This attribute a base type from which attributes with DN syntax inherit.

## dn.c

Attribute | Value
--- | ---
**IE Name** | dn.c
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.2: c](https://tools.ietf.org/html/rfc4519#section-2.2)
**Description** | Country Name. The `c` (`countryName` in X.500) attribute type contains a two-letter ISO 3166 country code.

## dn.cn

Attribute | Value
--- | ---
**IE Name** | dn.cn
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.3: cn](https://tools.ietf.org/html/rfc4519#section-2.3)
**Description** | Common Name. The `cn` (`commonName` in X.500) attribute type contains names of an object. Each name is one value of this multi-valued attribute. If the object corresponds to a person, it is typically the person's full name.

## dn.dc

Attribute | Value
--- | ---
**IE Name** | dn.dc
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.4: dc](https://tools.ietf.org/html/rfc4519#section-2.4)
**Description** | Domain Component. The `dc` (`domainComponent` in RFC 1274) attribute type is a string holding one component, a label, of a DNS domain name naming a host.

## dn.dnq

Attribute | Value
--- | ---
**IE Name** | dn.dc
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.8: dnq](https://tools.ietf.org/html/rfc4519#section-2.8)
**Description** | The `dnQualifier` attribute type contains disambiguating information strings to add to the relative distinguished name of an entry. The information is intended for use when merging data from multiple sources in order to prevent conflicts between entries that would otherwise have the same name.

## dn.e

Attribute | Value
--- | ---
**IE Name** | dn.e
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | Email Address. Deprecated in preference to `mail`.

## dn.l

Attribute | Value
--- | ---
**IE Name** | dn.l
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.16: l](https://tools.ietf.org/html/rfc4519#section-2.16)
**Description** | Locality Name. The `l` (`localityName` in X.500) attribute type contains names of a locality or place, such as a city, county, or other geographic region.

## dn.o

Attribute | Value
--- | ---
**IE Name** | dn.o
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.19: o](https://tools.ietf.org/html/rfc4519#section-2.19)
**Description** | Organization Name. The `o` (`organizationName` in X.500) attribute type contains the names of an organization.

## dn.ou

Attribute | Value
--- | ---
**IE Name** | dn.ou
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.20: ou](https://tools.ietf.org/html/rfc4519#section-2.20)
**Description** | Organizational Unit. The `ou` (`organizationalUnitName` in X.500) attribute type contains the names of an organizational unit.

## dn.pc

Attribute | Value
--- | ---
**IE Name** | dn.pc
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.24: postalCode](https://tools.ietf.org/html/rfc4519#section-2.24)
**Description** | Postal Code. The `postalCode` attribute type contains codes used by a Postal Service to identify postal service zones.

## dn.serialnumber

Attribute | Value
--- | ---
**IE Name** | dn.pc
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.31: serialNumber](https://tools.ietf.org/html/rfc4519#section-2.31)
**Description** | The `serialNumber` attribute type contains the serial numbers of devices.

## dn.st

Attribute | Value
--- | ---
**IE Name** | dn.st
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.33: st](https://tools.ietf.org/html/rfc4519#section-2.33)
**Description** | State or Province. The `st` (`stateOrProvinceName` in X.500) attribute type contains the full names of states or provinces.

## dn.street

Attribute | Value
--- | ---
**IE Name** | dn.street
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.34: street](https://tools.ietf.org/html/rfc4519#section-2.34)
**Description** | Street Address. The `street` (`streetAddress` in X.500) attribute type contains site information from a postal address (i.e., the street name, place, avenue, and the house number).

## dn.title

Attribute | Value
--- | ---
**IE Name** | dn.uid
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.38: title](https://tools.ietf.org/html/rfc4519#section-2.38)
**Description** | The `title` attribute type contains the title of a person in their organizational context.

## dn.uid

Attribute | Value
--- | ---
**IE Name** | dn.uid
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4519, section 2.39: uid](https://tools.ietf.org/html/rfc4519#section-2.39)
**Description** | User ID. The `uid` (`userid` in RFC 1274) attribute type contains computer system login names associated with the object.

## dn.unique_id

Attribute | Value
--- | ---
**IE Name** | dn.dn
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 4524, section 2.24: uniqueIdentifier](https://tools.ietf.org/html/rfc4524#section-2.24)
**Description** | The `uniqueIdentifier` attribute specifies a unique identifier for an object represented in the Directory. The domain within which the identifier is unique and the exact semantics of the identifier are for local definition. For a person, this might be an institution-wide payroll number. For an organizational unit, it might be a department code.
