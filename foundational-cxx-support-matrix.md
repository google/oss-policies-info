# Foundational C++ Support

| Dimension       | Supported Version      | Last Changed | Next Change [^next-change] |
|-----------------|------------------------|--------------|-------------|
| C++ Version     | >= 14                  | 2022-07-01   | 2024-12-15  |
| CMake           | >= 3.10                | 2022-07-01   | 2023-06-01  |
| Bazel           | 6 LTS                  | 2023-04-18   | 2023-06-01  |
| GCC             | >= 7.3.1               | 2022-07-01   | 2024-07-01  |
| Clang           | >= 6.0.0               | 2022-07-01   | 2023-06-01  |
| MSVC            | >= 2019                | 2023-03-10   | 2024-05-01  |
| Apple Clang     | >= 12                  | 2022-07-01   | |
| Android NDK API | == 19                  | 2022-07-01   | |
| Alpine          | >= 3.14                | 2022-07-01   | 2023-06-01 |
| Debian          | >= 10                  | 2022-07-01   | 2024-07-01 |
| Fedora          | >= 36                  | 2022-02-24   | 2023-06-01 |
| openSUSE        | >= Leap 15.4           | 2023-02-24   | 2024-01-01 |
| Ubuntu LTS      | >= 18.04               | 2022-07-01   | 2023-06-01 |
| RHEL            | >= 7 [^rhel-7]         | 2022-07-01   | 2024-07-01 |
| CentOS          | 7 [^rhel-7]            | 2022-07-01   | 2024-07-01 |
| RockyLinux      | 8                      | 2022-07-01   | 2024-06-01 |
| Windows Server  | >= 2019                | 2022-02-24   | 2024-02-01 |
| Windows Client  | >= 10                  | 2022-07-01   | 2025-11-01 |
| macOS           | >= 10.13 (High Sierra) | 2023-05-05   | 2024-05-05 |
| iOS             | >= 12.0                | 2022-07-01   | |

[^next-change]: This is an estimated date. The actual date may change if the
vendor (or community, as applicable) extends or shortens the lifetime of the
dimension in question.

[^rhel-7]: We require the [devtoolset-7] toolchain (compiler, linker, build
tools, etc.) on RHEL 7 and CentOS 7.

### Notes

The relevant policies are described at https://opensource.google/documentation/policies/cplusplus-support.

[devtoolset-7]: https://www.softwarecollections.org/en/scls/rhscl/devtoolset-7/
