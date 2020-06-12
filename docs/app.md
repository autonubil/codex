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
