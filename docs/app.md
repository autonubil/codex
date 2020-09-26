# `app`

The `app` object contains information elements related to *Applications*.

## `app.name`

Attribute | Value
--- | ---
**IE Name** | `app.name`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Description** | The full name of the application. This may include version details. For example, `Google Chrome Version 83.0.4103.97 (Official Build) (64-bit)`.

## `app.version`

Attribute | Value
--- | ---
**IE Name** | `app.version`
**Tier** | `common`
**Data Type** | object: `version`
**Description** | The version of the application.

## `app.arch`

Attribute | Value
--- | ---
**IE Name** | `app.arch`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Description** | The processor architecture for which the application is compliled. Examples include `x86_64`, `i386`, `ARMv8`, etc.

app.id
app.name
app.codename
app.descr

app.version.ver

app.arch
app.vendor

app.category.id
app.category.name
app.subcategory.id
app.subcategory.name
app.group.id
app.group.name

app.ndpi.proto.id
app.ndpi.proto.name
app.ndpi.sub_proto.id
app.ndpi.sub_proto.name

app.attr.p2p
app.attr.tunnel
app.attr.encrypt

app.payload

app.start.timestamp
app.stop.timestamp
app.stop.reason.id
app.stop.reason.name

app.proc.pid
app.proc.cmdline (full command line)
app.proc.path (the full path to the cmd)
app.proc.wd (working directory)
app.proc.cmd (name of the binary)
app.proc.args (arguments)
app.proc.name
app.proc.descr
app.proc.sig. {hash}
app.proc.sig.func.id
app.proc.sig.func.name
app.proc.sig.value
app.proc.start.timestamp
app.proc.start.sysuptime
app.proc.end.timestamp
app.proc.end.sysuptime
app.proc.user. {user}
app.proc.user.uid
app.proc.user.id
app.proc.user.name
app.proc.user.fullname
app.proc.user.org
app.proc.user.email
app.proc.group. {group}
app.proc.group.gid
app.proc.group.name
app.proc.group.org
app.proc.group.email
app.proc.file. {file}
app.proc.file.atime
app.proc.file.ctime
app.proc.file.mtime

app.resp_time

app.rndtrip.latency
