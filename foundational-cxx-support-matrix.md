# Foundational C++ Support

| Dimension       | Supported Version      | Last Changed | Next Change [^next-change] |
|-----------------|------------------------|--------------|-------------|
| C++ Version     | >= 17                  | 2024-12-17   | 2027-12-15  |
| CMake           | >= 3.22                | 2025-06-04   | 2027-05-01 [^cmake] |
| Bazel           | 8 LTS, 7 LTS           | 2025-05-12   | 2025-11-01  |
| GCC             | >= 7.5.0               | 2024-07-01   | 2026-01-01 [^gcc] |
| Clang           | >= 14.0.0              | 2025-06-04   | 2027-05-01 [^clang] |
| MSVC            | >= 2022                | 2024-04-29   | 2027-01-12  |
| Apple Clang     | >= 12                  | 2022-07-01   | 2025-07-30 |
| Android NDK API | == 21                  | 2022-09-18   | |
| Alpine          | >= 3.19                | 2025-06-04   | 2025-11-01 |
| Debian          | >= 11                  | 2024-07-01   | 2026-06-30 |
| Fedora          | >= 40                  | 2024-12-17   | 2025-05-28 |
| openSUSE        | >= Leap 15.6           | 2024-12-31   | 2025-12-31 |
| Ubuntu LTS      | >= 22.04               | 2025-06-04   | 2027-05-01 |
| RHEL            | >= 9                   | 2024-07-01   | 2027-06-01 |
| RockyLinux      | >= 9                   | 2024-07-01   | 2027-06-01 |
| Windows Server  | >= 2022                | 2024-01-22   | 2026-10-13 |
| Windows Client  | >= 10                  | 2022-07-01   | 2025-11-01 |
| macOS           | >= 11 (Big Sur)        | 2024-09-17   | 2025-07-30 |
| iOS             | >= 15                  | 2024-01-24   | 2025-07-30 |
| glibc           | >= 2.27                | 2024-07-09   | TBD [^glibc] |
| musl            | >= 1.2.4               | 2024-12-17   | 2025-05-09 |

[^next-change]: This is an estimated date. The actual date may change if the
vendor (or community, as applicable) extends or shortens the lifetime of the
dimension in question.

[^cmake]: We support the oldest version of CMake that ships with one of the
supported distros. Currently that is CMake 3.16 as Ubuntu 20.04 ships with this
version.

[^gcc]: Once openSUSE/Leap 15.5 reaches EOL we will support the oldest
version of GCC that ships with one of the supported distros.

[^clang]: We support the oldest version of Clang that ships with one of the
supported distros. Currently that is Clang 14.0 as Ubuntu 22.04 ships with
this version.

[^glibc]: We plan to support glibc >= 2.27 until further notice.

### Notes

The relevant policies are described at https://opensource.google/documentation/policies/cplusplus-support.

[devtoolset-7]: https://www.softwarecollections.org/en/scls/rhscl/devtoolset-7/
