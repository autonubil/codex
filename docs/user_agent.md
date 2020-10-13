# user_agent

The `user_agent` object contains information elements related to HTTP `User-Agent` header values, and other sources which contain similar information.

## user_agent.agent

Attribute | Value
--- | ---
**IE Name** | user_agent.agent
**Tier** | core
**Data Type** | string
**Semantic** | default
**Reference** | [RFC 7231, section 5.5.3: User-Agent](https://tools.ietf.org/html/rfc7231#section-5.5.3)
**Description** | The `User-Agent` request header is a characteristic string that lets servers and network peers identify the application, operating system, vendor, and/or version of the requesting user agent.

## user_agent.device

Attribute | Value
--- | ---
**IE Name** | user_agent.device
**Tier** | custom
**Data Type** | string
**Semantic** | default
**Description** | This information element describes device details extracted from the `User-Agent` header value.

## user_agent.os

Attribute | Value
--- | ---
**IE Name** | user_agent.os
**Tier** | custom
**Data Type** | object: os
**Description** | This object describes operating system details extracted from the `User-Agent` header value.

## user_agent.app

Attribute | Value
--- | ---
**IE Name** | user_agent.app
**Tier** | custom
**Data Type** | object: app
**Description** | This object describes application details extracted from the `User-Agent` header value.
