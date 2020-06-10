# `version`

The `version` object contains information elements related to [Semantic Versioning](https://semver.org/) values.

Under Semantic Versioning, version numbers and the way they change convey meaning about the underlying code and what has been modified from one version to the next.

Given a version number *MAJOR.MINOR.PATCH*, increment the:

- MAJOR version when you make incompatible API changes,
- MINOR version when you add functionality in a backwards compatible manner, and
- PATCH version when you make backwards compatible bug fixes.

Additional labels for *pre-release* and *build* metadata are available as extensions to the MAJOR.MINOR.PATCH format.

## `version.ver`

Attribute | Value
--- | ---
**IE Name** | `version.ver`
**Tier** | `common`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Semantic Versioning](https://semver.org/)
**Description** | The full semantic version.

## `version.major`

Attribute | Value
--- | ---
**IE Name** | `version.major`
**Tier** | `custom`
**Data Type** | `integer`
**Semantic** | `identifier`
**Reference** | [Semantic Versioning](https://semver.org/)
**Description** | The `major` value from the semantic version.

## `version.minor`

Attribute | Value
--- | ---
**IE Name** | `version.minor`
**Tier** | `custom`
**Data Type** | `integer`
**Semantic** | `identifier`
**Reference** | [Semantic Versioning](https://semver.org/)
**Description** | The `minor` value from the semantic version.

## `version.patch`

Attribute | Value
--- | ---
**IE Name** | `version.patch`
**Tier** | `custom`
**Data Type** | `integer`
**Semantic** | `identifier`
**Reference** | [Semantic Versioning](https://semver.org/)
**Description** | The `patch` value from the semantic version.

## `version.prerel`

Attribute | Value
--- | ---
**IE Name** | `version.prerel`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Semantic Versioning](https://semver.org/)
**Description** | The `pre-release` value from the semantic version.

## `version.build`

Attribute | Value
--- | ---
**IE Name** | `version.build`
**Tier** | `custom`
**Data Type** | `string`
**Semantic** | `default`
**Reference** | [Semantic Versioning](https://semver.org/)
**Description** | The `build` value from the semantic version.
