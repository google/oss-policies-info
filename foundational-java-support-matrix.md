
# Foundational Java Support

| Dimension         | Supported Version | Last Changed | Next Change [^next-change] |
|-------------------|-------------------|--------------|----------------------------|
| Java Version      | >= 8              | 2024-01-30   | 2026-11-12                 |
| Android API Level | >= 21             | 2024-01-30   | 2025-07-24                 |

[^next-change]: This is an estimated date. The actual date may change if the
vendor (or community, as applicable) extends or shortens the lifetime of the
dimension in question.

### Footnotes

The relevant policies are described at https://cloud.google.com/java/docs/supported-java-versions.

On Android, we support the minimum SDK version that is supported by
[Google Play services](https://developers.google.com/android/guides/setup) and
is the default in
[Jetpack](https://android.googlesource.com/platform/frameworks/support/+/refs/heads/androidx-main/docs/api_guidelines/modules.md#module-minsdkversion).
If both versions differ, the lower version is supported.
