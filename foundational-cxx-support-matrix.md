# Foundational C++ Support

| Dimension       | Supported Version      | Last Changed | Next Change [^next-change] |
|-----------------|------------------------|--------------|-------------|
| C++ Version     | >= 14                  | 2022-07-01   | 2024-12-15  |
| CMake           | >= 3.13                | 2023-06-01   | 2024-07-01 [^cmake] |
| Bazel           | 6 LTS                  | 2023-04-18   | 2024-07-01  |
| GCC             | >= 7.3.1               | 2022-07-01   | 2024-07-01 [^gcc] |
| Clang           | >= 7.0.0               | 2023-06-01   | 2025-04-02 [^clang] |
| MSVC            | >= 2019                | 2023-03-10   | 2024-05-01  |
| Apple Clang     | >= 12                  | 2022-07-01   | |
| Android NDK API | == 21                  | 2022-09-18   | |
| Alpine          | >= 3.16                | 2024-01-02   | 2024-06-01 |
| Debian          | >= 10                  | 2022-07-01   | 2024-07-01 |
| Fedora          | >= 39                  | 2024-01-02   | 2024-12-01 |
| openSUSE        | >= Leap 15.5           | 2024-01-02   | 2025-01-01 |
| Ubuntu LTS      | >= 20.04               | 2023-06-01   | 2025-04-02 |
| RHEL            | >= 7 [^rhel-7]         | 2022-07-01   | 2024-07-01 |
| CentOS          | 7 [^rhel-7]            | 2022-07-01   | 2024-07-01 |
| RockyLinux      | 8                      | 2022-07-01   | 2024-06-01 |
| Windows Server  | >= 2019                | 2022-02-24   | 2024-02-01 |
| Windows Client  | >= 10                  | 2022-07-01   | 2025-11-01 |
| macOS           | >= 10.13 (High Sierra) | 2023-05-05   | 2024-05-05 |
| iOS             | >= 14.0.1              | 2023-09-18   | |

[^next-change]: This is an estimated date. The actual date may change if the
vendor (or community, as applicable) extends or shortens the lifetime of the
dimension in question.

[^rhel-7]: We require the [devtoolset-7] toolchain (compiler, linker, build
tools, etc.) on RHEL 7 and CentOS 7.

[^cmake]: We support the oldest version of CMake that ships with one of the
supported distros. Currently that is CMake 3.13 as Debian 10 ships with this
version.

[^gcc]: Once RHEL 7 reaches EOL we will support the oldest version of GCC
that ships with one of the supported distros.

[^clang]: We support the oldest version of Clang that ships with one of the
supported distros. Currently that is Clang 7.0 as Ubuntu 20.04 ships with
this version.

### Notes

The relevant policies are described at https://opensource.google/documentation/policies/cplusplus-support.

[devtoolset-7]: https://www.softwarecollections.org/en/scls/rhscl/devtoolset-7/
