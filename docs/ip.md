# ip

## ip.addr

Attribute | Value
--- | ---
**IE Name** | ip.addr
**Tier** | core
**Data Type** | ipaddress
**Semantic** | default
**Description** | 

## ip.subnet

### ip.subnet.mask

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | core
**Data Type** | ipaddress
**Semantic** | default
**Description** | 

### ip.subnet.mask_size

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | core
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bits
**Description** | 

### ip.subnet.prefix

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | core
**Data Type** | ipaddress
**Semantic** | default
**Description** | 

### ip.subnet.bcast

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | common
**Data Type** | ipaddress
**Semantic** | default
**Description** | 

## ip.version

Attribute | Value
--- | ---
**IE Name** | ip.version
**Tier** | common
**Data Type** | object: version
**Reference** | 
**Description** | 

## ip.proto

### ip.proto.id

Attribute | Value
--- | ---
**IE Name** | ip.proto.id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the IP Protocol type.

### ip.proto.name

Attribute | Value
--- | ---
**IE Name** | ip.proto.name
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the IP Protocol type.

## ip.ttl

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | core
**Data Type** | unsigned
**Semantic** | quantity
**Reference** | []()
**Description** | 

## ip.tos

### ip.tos.id

Attribute | Value
--- | ---
**IE Name** | ip.tos.id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the IP Type of Service (ToS) type.

### ip.tos.name

Attribute | Value
--- | ---
**IE Name** | ip.tos.name
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the Type of Service (ToS) type.

## ip.prec

### ip.prec.id

Attribute | Value
--- | ---
**IE Name** | ip.prec.id
**Tier** | common
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the IP Precedence type.

### ip.prec.name

Attribute | Value
--- | ---
**IE Name** | ip.prec.name
**Tier** | common
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the IP Precedence type.

## ip.dscp

### ip.dscp.id

Attribute | Value
--- | ---
**IE Name** | ip.dscp.id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the IP DSCP type.

### ip.dscp.name

Attribute | Value
--- | ---
**IE Name** | ip.dscp.name
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the IP DSCP type.

## ip.ecn

### ip.ecn.id

Attribute | Value
--- | ---
**IE Name** | ip.ecn.id
**Tier** | core
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | The enumeratiom ID of the IP ECN type.

### ip.ecn.name

Attribute | Value
--- | ---
**IE Name** | ip.ecn.name
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | []()
**Description** | The enumeration name of the IP ECN type.

## ip.frag

### ip.frag.id

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | common
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | []()
**Description** | 

### ip.frag.offset

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

### ip.frag.flags

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

## ip.header

### ip.header.sample

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | common
**Data Type** | octetarray
**Semantic** | default
**Reference** | []()
**Description** | 

### ip.header.size

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Description** | 

## ip.packet

### ip.packet.sample

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | common
**Data Type** | octetarray
**Semantic** | default
**Reference** | []()
**Description** | 

### ip.packet.size

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Description** | 

## ip.payload

### ip.payload.sample

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | common
**Data Type** | octetarray
**Semantic** | default
**Reference** | []()
**Description** | 

### ip.payload.size

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | unsigned
**Semantic** | quantity
**Unit** | bytes
**Description** | 

## ip.v4

### ip.v4.ihl

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

### ip.v4.checksum

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

### ip.v4.options

#### ip.v4.options.bits

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

#### ip.v4.options.tags

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

## ip.v6

### ip.v6.flow_label

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

### ip.v6.next_header

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

### ip.v6.extension_headers

Attribute | Value
--- | ---
**IE Name** | 
**Tier** | 
**Data Type** | 
**Semantic** | 
**Unit** | 
**Description** | 

### ip.rndtrip.latency
