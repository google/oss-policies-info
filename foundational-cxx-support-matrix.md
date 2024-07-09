# Foundational C++ Support

| Dimension       | Supported Version      | Last Changed | Next Change [^next-change] |
|-----------------|------------------------|--------------|-------------|
| C++ Version     | >= 14                  | 2022-07-01   | 2024-12-15  |
| CMake           | >= 3.16                | 2024-07-01   | 2024-11-22 [^cmake] |
| Bazel           | 6 LTS                  | 2023-04-18   | 2024-11-01  |
| GCC             | >= 7.5.0               | 2024-07-01   | 2026-01-01 [^gcc] |
| Clang           | >= 7.0.0               | 2023-06-01   | 2025-04-02 [^clang] |
| MSVC            | >= 2022                | 2024-04-29   | 2027-01-12  |
| Apple Clang     | >= 12                  | 2022-07-01   | |
| Android NDK API | == 21                  | 2022-09-18   | |
| Alpine          | >= 3.17                | 2024-07-01   | 2024-11-22 |
| Debian          | >= 11                  | 2024-07-01   | 2026-06-30 |
| Fedora          | >= 39                  | 2024-01-02   | 2024-12-01 |
| openSUSE        | >= Leap 15.5           | 2024-01-02   | 2025-01-01 |
| Ubuntu LTS      | >= 20.04               | 2023-06-01   | 2025-04-02 |
| RHEL            | >= 9                   | 2024-07-01   | 2027-06-01 |
| RockyLinux      | >= 9                   | 2024-07-01   | 2027-06-01 |
| Windows Server  | >= 2022                | 2024-01-22   | 2026-10-13 |
| Windows Client  | >= 10                  | 2022-07-01   | 2025-11-01 |
| macOS           | >= 10.15 (Catalina)    | 2024-01-24   | 2024-07-01 |
| iOS             | >= 15                  | 2024-01-24   | |
| glibc           | >= 3.27                | 2024-07-09   | TBD [^glibc] |
| musl            | >= 1.2.3-r5            | 2024-07-09   | 2024-11-22 |

[^next-change]: This is an estimated date. The actual date may change if the
vendor (or community, as applicable) extends or shortens the lifetime of the
dimension in question.

[^cmake]: We support the oldest version of CMake that ships with one of the
supported distros. Currently that is CMake 3.16 as Ubuntu 20.04 ships with this
version.

[^gcc]: Once openSUSE/Leap 15.5 reaches EOL we will support the oldest
version of GCC that ships with one of the supported distros.

[^clang]: We support the oldest version of Clang that ships with one of the
supported distros. Currently that is Clang 7.0 as Ubuntu 20.04 ships with
this version.

[^glibc]: We plan to support glibc >= 2.27 until further notice.

### Notes

The relevant policies are described at https://opensource.google/documentation/policies/cplusplus-support.

[devtoolset-7]: https://www.softwarecollections.org/en/scls/rhscl/devtoolset-7/
