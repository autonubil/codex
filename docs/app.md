# app

The app object contains information elements related to *Applications*.

## app.id

Attribute | Value
--- | ---
**IE Name** | app.id
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.name

Attribute | Value
--- | ---
**IE Name** | app.name
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The full name of the application. This may include version details. For example, `Google Chrome Version 83.0.4103.97 (Official Build) (64-bit)`.

## app.version

Attribute | Value
--- | ---
**IE Name** | app.version
**Tier** | common
**Data Type** | object: version
**Description** | The version of the application.

## app.arch

Attribute | Value
--- | ---
**IE Name** | app.arch
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The processor architecture for which the application is compliled. Examples include `x86_64`, `i386`, `ARMv8`, etc.

## app.codename

Attribute | Value
--- | ---
**IE Name** | app.codename
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.descr

Attribute | Value
--- | ---
**IE Name** | app.descr
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.vendor

Attribute | Value
--- | ---
**IE Name** | app.vendor
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.category

### app.category.id

Attribute | Value
--- | ---
**IE Name** | app.category.id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | 
**Description** | 

### app.category.name

Attribute | Value
--- | ---
**IE Name** | app.category.name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.subcategory

### app.subcategory.id

Attribute | Value
--- | ---
**IE Name** | app.subcategory.id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | 
**Description** | 

### app.subcategory.name

Attribute | Value
--- | ---
**IE Name** | app.subcategory.name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.group

### app.group.id

Attribute | Value
--- | ---
**IE Name** | app.group.id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | 
**Description** | 

### app.group.name

Attribute | Value
--- | ---
**IE Name** | app.group.name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.proto

### app.proto.id

Attribute | Value
--- | ---
**IE Name** | app.proto.id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | 
**Description** | 

### app.proto.name

Attribute | Value
--- | ---
**IE Name** | app.proto.name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.sub_proto

### app.sub_proto.id

Attribute | Value
--- | ---
**IE Name** | app.sub_proto.id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | 
**Description** | 

### app.sub_proto.name

Attribute | Value
--- | ---
**IE Name** | app.sub_proto.name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.attr

### app.attr.p2p

Attribute | Value
--- | ---
**IE Name** | app.attr.p2p
**Tier** | 
**Data Type** | 
**Semantic** | 
**Reference** | 
**Description** | 

### app.attr.tunnel

Attribute | Value
--- | ---
**IE Name** | app.attr.tunnel
**Tier** | 
**Data Type** | 
**Semantic** | 
**Reference** | 
**Description** | 

### app.attr.encrypt

Attribute | Value
--- | ---
**IE Name** | app.attr.encrypt
**Tier** | 
**Data Type** | 
**Semantic** | 
**Reference** | 
**Description** | 

## app.payload

Attribute | Value
--- | ---
**IE Name** | app.payload
**Tier** | 
**Data Type** | octetarray
**Semantic** | default
**Reference** | 
**Description** | 

### app.start.timestamp

Attribute | Value
--- | ---
**IE Name** | app.start.timestamp
**Tier** | 
**Data Type** | unsigned
**Semantic** | epochticks
**Reference** | 
**Description** | 

### app.end.timestamp

Attribute | Value
--- | ---
**IE Name** | app.end.timestamp
**Tier** | 
**Data Type** | unsigned
**Semantic** | epochticks
**Reference** | 
**Description** | 

### app.end.reason

#### app.end.reason.id

Attribute | Value
--- | ---
**IE Name** | app.end.reason.id
**Tier** | 
**Data Type** | unsigned
**Semantic** | identifier
**Reference** | 
**Description** | 

#### app.end.reason.name

Attribute | Value
--- | ---
**IE Name** | app.end.reason.name
**Tier** | 
**Data Type** | string
**Semantic** | default
**Reference** | 
**Description** | 

## app.proc

Attribute | Value
--- | ---
**IE Name** | app.proc
**Tier** | 
**Data Type** | object: proc
**Reference** | 
**Description** | 

## app.rndtrip.latency

## app.svc.latency
