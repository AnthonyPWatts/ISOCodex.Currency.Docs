# ISOCodex.Currency

Currency metadata, immutable money values, explicit rounding, allocation and optional application integrations for .NET.

This repository contains public documentation, runnable examples and the consumer issue tracker. The library implementation and development history are maintained in a separate private repository. Install the published packages from NuGet; clone this repository to run the examples against published NuGet packages.

## Try it locally

With the .NET 10 SDK installed, clone this public repository and run:

```powershell
git clone https://github.com/AnthonyPWatts/ISOCodex.Currency.Docs.git
cd ISOCodex.Currency.Docs
dotnet run --project samples/CheckoutPricingApi --no-launch-profile --urls http://localhost:5003
```

[Browse all runnable examples](samples/README.md). They use published NuGet packages and need no private repository access.

## Install

Current release: **1.1.1**. [View on NuGet](https://www.nuget.org/packages/ISOCodex.Currency/1.1.1).

```powershell
dotnet add package ISOCodex.Currency --version 1.1.1
```

## What it provides

- Currency-aware arithmetic and precision validation at application boundaries.
- Explicit rounding, allocation, instalments, formatting and conservative parsing.
- Optional JSON, Dapper, EF Core, ASP.NET Core, validation and country/address integrations.
- Deterministic exchange abstractions; no bundled live exchange-rate provider.

## Documentation

- [Consumer guide](docs/usage.md)
- [Framework compatibility and verification](docs/compatibility.md)
- [Release notes](CHANGELOG.md)
- [Questions, bug reports and feature requests](https://github.com/AnthonyPWatts/ISOCodex.Currency.Docs/issues)
- [Discussion](https://github.com/AnthonyPWatts/ISOCodex.Currency.Docs/discussions)

- [Countries documentation](https://github.com/AnthonyPWatts/ISOCodex.Countries.Docs)
- [Addressing documentation](https://github.com/AnthonyPWatts/ISOCodex.Addressing.Docs)

## Feedback

Include package versions, target framework, expected behaviour and a small reproducible consumer example when reporting a problem. Data corrections should include a reliable source and the date checked.

## Licence and source availability

The documentation and sample applications are provided under the [MIT licence](LICENSE). Published packages retain their declared licences. Private source hosting does not revoke rights already granted for earlier distributions. ISOCodex is not an official ISO product or endorsed by ISO.
