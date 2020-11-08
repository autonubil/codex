# os

The os object contains information elements related to *Operating Systems*.

## os.name

Attribute | Value
--- | ---
**IE Name** | os.name
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The full name of the operating system. This may include codename and version. For example, `macOS Catalina 10.15.5`.

## os.family

Attribute | Value
--- | ---
**IE Name** | os.family
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The category of the operating system. Examples include, `SysV`, `BSD`, `Darwin`, `Linux`, `Windows`, etc.

## os.distro

Attribute | Value
--- | ---
**IE Name** | os.distro
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The distribution of the operating system. This is a subcategory of os.family. Examples include, `AIX`, `macOS`, `Ubuntu`, `Fedora`, `Windows Server`, etc.

## os.codename

Attribute | Value
--- | ---
**IE Name** | os.codename
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The common codename for a release of an OS distrobution. For example, macOS `Sierra`, `Mojave` and `Catalina`, as well as Ubuntu `Bionic Beaver` and `Focal Fossa`.

## os.version

Attribute | Value
--- | ---
**IE Name** | os.version
**Tier** | common
**Data Type** | object: version
**Description** | The version of the operating system.

## os.kernel

Attribute | Value
--- | ---
**IE Name** | os.kernel
**Tier** | common
**Data Type** | object: version
**Description** | The version of the kernel used by the operating system.

## os.arch

Attribute | Value
--- | ---
**IE Name** | os.arch
**Tier** | common
**Data Type** | string
**Semantic** | default
**Description** | The processor architecture for which the operating system is compliled. Examples include `x86_64`, `i386`, `ARMv8`, etc.
