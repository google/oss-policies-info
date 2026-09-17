# Foundational C++ Support

The relevant policies are described at https://opensource.google/documentation/policies/cplusplus-support.
This document captures the specific version numbers as resolved by those policies.

Note that some of these version supports apply broadly to other languages as well, and are not exclusive to C++.

## Linux distributions

### Cited Text

> We will support releases of the following Linux distributions until the vendor
> drops support.

Vendor support is obtained from published support windows.
https://endoflife.date/ consolidates these support windows on top of providing a
visualization.

### Implied Support Matrix

| Distribution    | Supported Version      | Last Changed | Next Change [^next-change] |
|-----------------|------------------------|--------------|-------------|
| Alpine          | >= 3.21                | 2026-04-01   | 2026-11-01 |
| Debian          | >= 13                  | 2026-08-10   | 2028-08-09 |
| Fedora          | >= 43                  | 2026-09-17   | 2026-12-10 |
| openSUSE        | >= Leap 16.0           | 2026-05-01   | 2027-10-31 |
| Ubuntu LTS      | >= 22.04               | 2025-06-04   | 2027-05-01 |
| RHEL            | >= 9                   | 2024-07-01   | 2027-06-01 |
| RockyLinux      | >= 9                   | 2024-07-01   | 2027-06-01 |

## Windows

### Cited Text

> We will build using the **newest Windows** server platform available.
>
> We will support all the Windows versions that Microsoft supports.
> i.  [Windows client support](https://docs.microsoft.com/en-us/windows/release-health/supported-versions-windows-client)
> ii. [Windows server support](https://endoflife.date/windows-server)

### Implied Support Matrix

| Dimension       | Supported Version      | Last Changed | Next Change [^next-change] |
|-----------------|------------------------|--------------|-------------|
| Windows Server  | >= 2022                | 2024-01-22   | 2026-10-13 |
| Windows Client  | >= 11                  | 2025-12-16   | 2026-10-13 |

## macOS

### Cited Text

> We will build using the newest XCode available.
> We will support back to the oldest macOS target platform needed by Chrome.
> We will support back to the oldest iOS target platform that has a simulator.

Note that Chrome has announced an update in its minimum required macOS version
in
[151](https://support.google.com/chrome/thread/404150391/sunsetting-support-for-macos-12-monterey-in-mid-2026?hl=en).
In addition, the
[Chrome browser system requirements](https://support.google.com/chrome/a/answer/7100626)
page shows Chrome's support timelines.

### Implied Support Matrix
| Dimension         | Supported Version      | Last Changed | Next Change [^next-change] |
|-------------------|------------------------|--------------|-------------|
| Xcode             | >= 27                  | 2026-09-17   | 2027-09-15 |
| macOS (target)    | >= 13 (Ventura)        | 2026-09-17   | 2027-01-01 |
| iOS  (target)     | >= 17                  | 2026-09-17   | 2027-09-15 |

## Android NDK

### Cited Text

> We will support Android -- we will build using the newest Android NDK and
> target its lowest supported API level (example
> [meta/platforms.json](https://android.googlesource.com/platform/ndk.git/+/refs/heads/master/meta/platforms.json)).

### Implied Support Matrix
| Dimension              | Supported Version      | Last Changed | Next Change [^next-change] |
|------------------------|------------------------|--------------|----------------------------|
| Android API (target)   | >= 21                  | 2022-09-18   |                            |

## Compilers, tools, build systems

### Cited Text

> 1. We do not support any compiler that is EOL as defined by the vendor.
> 1. We support GCC and Clang on our supported Linux distros (see above). We
>    support the version installed by default (e.g., apt install gcc), unless
>    we've explicitly excluded support for that version because it doesn't
>    support other required policies of ours (e.g., we agree to remove GCC 4.8
>    because of its incomplete C++11 support, as well as clang 3.x). If we
>    cannot support the default version, we may instead support a newer version
>    that's available from the vendor (e.g., devtoolset-7 on RHEL/CentOS 7)
> 1. We support Apple Clang on our supported XCode version.
> 1. We support MSVC on our supported Windows versions.
>    1. We support the MSVC versions that are in the Mainstream Support window
>       as defined by Microsoft's Fixed Lifecycle Policy.


### Implied Support Matrix

| Dimension       | Supported Version      | Last Changed | Next Change [^next-change] |
|-----------------|------------------------|--------------|-------------|
| C++ Version     | >= 17                  | 2024-12-17   | 2027-12-15  |
| CMake           | >= 3.22                | 2025-06-04   | 2027-05-01 [^cmake] |
| Bazel           | 8 LTS                  | 2025-12-16   | 2026-12-01  |
| GCC             | >= 11.2                | 2026-09-17   | 2027-06-30 [^gcc] |
| Clang           | >= 14.0.0              | 2025-06-04   | 2027-05-01 [^clang] |
| MSVC            | >= 2022                | 2024-04-29   | 2027-01-12  |
| Apple Clang     | >= 21                  | 2026-09-17   | 2027-09-15 [^apple-clang] |
| glibc           | >= 2.34                | 2024-07-09   | 2027-06-01 [^glibc] |
| musl            | >= 1.2.5               | 2026-04-01   | 2026-11-01 |

### Implied Support Matrix [Detailed Linux Breakdown]

This table charts the default package version from major Linux distributions
that comes with a standard install on our oldest supported distro major version,
along with the resulting minimum supported version across all distros.

NOTE: This table should be audited again on or after 2026-11-01.

| Distribution (Oldest Supported) | C++ Version | CMake       | GCC         | Clang       | glibc       | musl         |
|---------------------------------|-------------|-------------|-------------|-------------|-------------|--------------|
| Alpine (3.21)                   | 17          | 3.31        | 14.2        | 19.1        | N/A         | 1.2.5        |
| Debian (13)                     | 17          | 3.31        | 14.2        | 19.0        | 2.41        | 1.2.5        |
| Fedora (43)                     | 17          | 3.31        | 15.2        | 21.1        | 2.42        | 1.2.6        |
| openSUSE (Leap 16.0)            | 17          | 4.3.4       | 15.0        | 22.0        | 2.43        | N/A          |
| RHEL / RockyLinux (9)           | 17          | 3.31        | 11.5        | 21.1        | 2.34        | N/A          |
| Ubuntu LTS (22.04)              | 17          | 3.22        | 11.2        | 14.0        | 2.35        | 1.2.5        |
| **Minimum Supported**           | **>= 17**   | **>= 3.22** | **>= 11.2** | **>= 14.0** | **>= 2.34** | **>= 1.2.5** |

[^next-change]: This is an estimated date. The actual date may change if the
vendor (or community, as applicable) extends or shortens the lifetime of the
dimension in question.

[^cmake]: We support the oldest version of CMake that ships with one of the
supported distros. Currently that is CMake 3.22 as Ubuntu 22.04 ships with this
version.

[^gcc]: We support the oldest version of GCC that ships with one of the
supported distros. Currently that is GCC 11.2 as Ubuntu 22.04 ships with this
version.

[^clang]: We support the oldest version of Clang that ships with one of the
supported distros. Currently that is Clang 14.0 as Ubuntu 22.04 ships with
this version.

[^apple-clang]: A community-maintained version record can be found
[here](https://gist.github.com/yamaya/2924292).

[^glibc]: We support the oldest version of glibc shipping with any of our
supported distros.  Currently that is glibc 2.34 shipping with RHEL 9 and
RockyLinux 9.  Internally, we currently support glibc 2.27 and may have code
referencing that.  We do not guarantee that it will work though.

### Notes


[devtoolset-7]: https://www.softwarecollections.org/en/scls/rhscl/devtoolset-7/
