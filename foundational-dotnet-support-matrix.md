# Foundational .NET Support

## Targeted frameworks vs supported frameworks

The tables below list the frameworks that are *targeted* by .NET
libraries following the [.NET Support
Policy](https://opensource.google/documentation/policies/dotnet-support).

Later versions of .NET and .NET Framework are compatible with
earlier ones. For example, a library targeting .NET 6 can be used
from .NET 8, and a library targeting .NET Framework 4.6.2 can be
used from .NET Framework 4.8.1. There may be some deployment
scenarios provided by later versions which are not fully supported,
however.

## New major library versions

The table below shows the [Target
Frameworks](https://learn.microsoft.com/en-us/dotnet/standard/frameworks)
that would be targeted for a new (or first) major version of a .NET
library conforming with the [.NET Support
Policy](https://opensource.google/documentation/policies/dotnet-support).

| Dimension       | Supported Version | TFM[^tfm] | Last Changed | Next Change [^next-change] |
|-----------------|-------------------|-----------|--------------|----------------------------|
| .NET            | >= 6.0            | net6.0    | 2024-01-17   | 2024-11-12                 |
| .NET Framework  | >= 4.6.2          | net462    | 2024-01-17   | 2027-01-12                 |

[^tfm]: Target Framework Moniker
[^next-change]: This is an estimated date. The actual date may change if the
vendor (or community, as applicable) extends or shortens the lifetime of the
dimension in question.

## New minor library versions

New minor versions drop support for older runtimes later than new
major versions. The table below shows the target frameworks that
could be targeted for a new minor version of a .NET library. New
minor versions may continue to target older versions than the ones
shown here. (Target frameworks are not automatically updated on minor releases.)

| Dimension       | Supported Version | TFM    | Last Changed | Next Change |
|-----------------|-------------------|--------|--------------|-------------|
| .NET            | >= 6.0            | net6.0 | 2024-01-17   | 2025-11-12  |
| .NET Framework  | >= 4.6.2          | net462 | 2024-01-17   | 2027-01-12  |

## .NET Standard

.NET Standard is not listed in the tables above. Some libraries may
choose to target .NET Standard, typically .NET Standard 2.0
(with TFM `netstandard2.0`).

[There will be no new versions of .NET
Standard](https://devblogs.microsoft.com/dotnet/the-future-of-net-standard/)
so there are no dates for when .NET Standard support will be removed
or updated.

### Footnotes

The relevant policies are described at https://opensource.google/documentation/policies/dotnet-support
