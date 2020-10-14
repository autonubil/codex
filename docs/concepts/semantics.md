# Semantics

This document describes the set of valid data type semantics.

Semantic | Description
:---|:---
default | Used to note that no semantics apply to the field. This is the default semantic type of all string data types.
quantity | A numeric (integral or floating point) value representing a measured value pertaining to the record. This is distinguished from counters that represent an ongoing measured value whose "odometer" reading is captured as part of a given record. This is the default semantic type of all numeric data types.
deltacounter | An integral value reporting the value of a counter. Counters are unsigned and wrap back to zero after reaching the limit of the type. Delta counters have an initial value of 0. A delta counter is reset to 0 each time it is exported and/or expires without export.
totalcounter | An integral value reporting the value of a counter. Counters are unsigned and wrap back to zero after reaching the limit of the type. A total counter counts independently of the export of its value.
identifier | An integral value that serves as an identifier. Specifically, mathematical operations on two identifiers (aside from the equality operation) are meaningless. Identifiers MUST be one of the signed or unsigned data types.
flags | An integral value that represents a set of bit fields. Logical operations are appropriate on such values, but other mathematical operations are not. Flags MUST always be of an unsigned data type.
timeticks | An integral value that represents a quantity of time intervals. The units of the information elements specifies the duration of each *tick*.
epochticks | An integral value that represents a quantity of time intervals sich *epoch* (January 1, 1970 00:00 UTC - in ISO 8601: 1970-01-01T00:00:00Z), not counting leap seconds. The units of the information elements specifies the duration of each *tick*.
iso8601 | A string value that represents an ISO 8601 compliant timestamp.
httpdate | A string value that represents an `HTTP-date` format as defined by RFC 7231 Date/Time Formats.
emailaddress | A string value that represents an E-Mail address.
uri | A string value that represents a Uniform Resource Identifier (URI - [RFC3986](https://tools.ietf.org/html/rfc3986)).
x509cert | An X.509 Certificate
