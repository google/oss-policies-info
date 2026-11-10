# Foundational Rust Support

The relevant policies are described at
https://docs.cloud.google.com/rust/docs/supported-rust-versions. This
document captures the specific version numbers as resolved by those policies.

### Cited Text

> The Cloud Client Libraries for Rust periodically update their MSRV
> (Minimum Supported Rust Version) to the oldest version of Rust released within
> the last year.
>
> Any new release of the Rust Cloud Client Libraries supports all the Rust
> versions that released in the prior year.

### Implied Support Matrix

Because [Rust releases](https://releases.rs/) a new minor version every 6 weeks,
the table below lists the implied minimum supported Rust version rolling forward
over the next 6 months based on prior release dates (the current minimum
supported version is the first row whose `MSRV Through` date has not yet
passed):

| Supported Rust Version | MSRV Through [^msrv-through] |
|------------------------|------------------------------|
| >= 1.92                | 2026-12-11                   |
| >= 1.93                | 2027-01-22                   |
| >= 1.94                | 2027-03-05                   |
| >= 1.95                | 2027-04-16                   |
| >= 1.96                | 2027-05-28                   |

[^msrv-through]: One year after the corresponding Rust `.0` minor release date
(`1.92.0` released 2025-12-11, `1.93.0` on 2026-01-22, `1.94.0` on 2026-03-05,
`1.95.0` on 2026-04-16, and `1.96.0` on 2026-05-28).
