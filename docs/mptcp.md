# `mptcp`

[https://tools.ietf.org/html/rfc8684](https://tools.ietf.org/html/rfc8684)

mptcp.data_seq

mptcp.init_data_seq

mptcp.ip.addr

mptcp.option.data
mptcp.option.id

Attribute | Value
--- | ---
**IE Name** | .id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the  type.

mptcp.option.name

Attribute | Value
--- | ---
**IE Name** | .name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the  type.

mptcp.rcvr.key
mptcp.rcvr.token

mptcp.sender.key
mptcp.sender.random
mptcp.sender.token
mptcp.sender.trunc_hmac

mptcp.size

mptcp.subflow_seq

```text
MPTCP Option Format
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-----------------------+
|     Kind      |    Length     |Subtype|                       |
+---------------+---------------+-------+                       |
|                     Subtype-specific data                     |
|                       (variable length)                       |
+---------------------------------------------------------------+

Multipath Capable (MP_CAPABLE) Option
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-------+---------------+
|     Kind      |    Length     |Subtype|Version|A|B|C|D|E|F|G|H|
+---------------+---------------+-------+-------+---------------+
|                   Option Sender's Key (64 bits)               |
|                      (if option Length > 4)                   |
|                                                               |
+---------------------------------------------------------------+
|                  Option Receiver's Key (64 bits)              |
|                      (if option Length > 12)                  |
|                                                               |
+-------------------------------+-------------------------------+
|  Data-Level Length (16 bits)  |  Checksum (16 bits, optional) |
+-------------------------------+-------------------------------+

Join Connection (MP_JOIN) Option (for Initial SYN)
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-----+-+---------------+
|     Kind      |  Length = 12  |Subtype|(rsv)|B|   Address ID  |
+---------------+---------------+-------+-----+-+---------------+
|                   Receiver's Token (32 bits)                  |
+---------------------------------------------------------------+
|                Sender's Random Number (32 bits)               |
+---------------------------------------------------------------+

Join Connection (MP_JOIN) Option (for Responding SYN/ACK)
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-----+-+---------------+
|     Kind      |  Length = 16  |Subtype|(rsv)|B|   Address ID  |
+---------------+---------------+-------+-----+-+---------------+
|                                                               |
|                Sender's Truncated HMAC (64 bits)              |
|                                                               |
+---------------------------------------------------------------+
|                Sender's Random Number (32 bits)               |
+---------------------------------------------------------------+

Join Connection (MP_JOIN) Option (for Initiator's First ACK)
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-----------------------+
|     Kind      |  Length = 24  |Subtype|      (reserved)       |
+---------------+---------------+-------+-----------------------+
|                                                               |
|                                                               |
|              Sender's Truncated HMAC (160 bits)               |
|                                                               |
|                                                               |
+---------------------------------------------------------------+

Data Sequence Signal (DSS) Option
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+----------------------+
|     Kind      |    Length     |Subtype| (reserved) |F|m|M|a|A|
+---------------+---------------+-------+----------------------+
|           Data ACK (4 or 8 octets, depending on flags)       |
+--------------------------------------------------------------+
|   Data Sequence Number (4 or 8 octets, depending on flags)   |
+--------------------------------------------------------------+
|              Subflow Sequence Number (4 octets)              |
+-------------------------------+------------------------------+
|  Data-Level Length (2 octets) |      Checksum (2 octets)     |
+-------------------------------+------------------------------+

Pseudo-Header for DSS Checksum
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+--------------------------------------------------------------+
|                                                              |
|                Data Sequence Number (8 octets)               |
|                                                              |
+--------------------------------------------------------------+
|              Subflow Sequence Number (4 octets)              |
+-------------------------------+------------------------------+
|  Data-Level Length (2 octets) |        Zeros (2 octets)      |
+-------------------------------+------------------------------+

Change Subflow Priority (MP_PRIO) Option
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-----+-+
|     Kind      |     Length    |Subtype|(rsv)|B|
+---------------+---------------+-------+-----+-+

Add Address (ADD_ADDR) Option
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-------+---------------+
|     Kind      |     Length    |Subtype|(rsv)|E|  Address ID   |
+---------------+---------------+-------+-------+---------------+
|           Address (IPv4: 4 octets / IPv6: 16 octets)          |
+-------------------------------+-------------------------------+
|   Port (2 octets, optional)   |                               |
+-------------------------------+                               |
|                Truncated HMAC (8 octets, if E=0)              |
|                               +-------------------------------+
|                               |
+-------------------------------+

Remove Address (REMOVE_ADDR) Option
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-------+---------------+
|     Kind      |Length = 3 + n |Subtype|(resvd)|   Address ID  | ...
+---------------+---------------+-------+-------+---------------+
						  (followed by n-1 Address IDs, if required)

Fast Close (MP_FASTCLOSE) Option
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-----------------------+
|     Kind      |    Length     |Subtype|      (reserved)       |
+---------------+---------------+-------+-----------------------+
|                      Option Receiver's Key                    |
|                            (64 bits)                          |
|                                                               |
+---------------------------------------------------------------+

TCP RST Reason (MP_TCPRST) Option
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+-----------------------+
|     Kind      |    Length     |Subtype|U|V|W|T|    Reason     |
+---------------+---------------+-------+-----------------------+

Fallback (MP_FAIL) Option
                     1                   2                   3
 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
+---------------+---------------+-------+----------------------+
|     Kind      |   Length=12   |Subtype|      (reserved)      |
+---------------+---------------+-------+----------------------+
|                                                              |
|                 Data Sequence Number (8 octets)              |
|                                                              |
+--------------------------------------------------------------+
```