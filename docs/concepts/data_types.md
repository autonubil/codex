# Data Types

This document describes the set of valid data types for information elements. Note that further data types may be specified by future updates to this document. 

Data Type | Avro | JSON | Description
:---|:---|:---|:---
null | null | null | A null value.
unsigned | int/long | integer | A non-negative integer value.
signed | int/long | integer | A signed integer value.
float | float/double | number | An IEEE single or double precision floating-point value.
boolean | boolean | boolean | A binary value. The only allowed values are `true` and `false`.
string | string | string | A finite-length string of valid characters.
octetarray | string | string | A finite-length string of octets.
ipaddress | string | string | An IPv4 or IPv6 address.
macaddress | string | string | A MAC-48 address as defined in IEEE.802-3.2012.
