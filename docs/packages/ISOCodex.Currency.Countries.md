# ISOCodex.Currency.Countries

Version 1.1.1 targets `netstandard2.0` for .NET Framework 4.7.2+ and modern .NET, replacing the redundant `netstandard2.1` asset. Framework consumers should enable automatic assembly binding redirects.

Bridge package connecting `ISOCodex.Currency` with `ISOCodex.Countries`.

## Install

```bash
dotnet add package ISOCodex.Currency.Countries --version 1.1.1
```

## Usage

```csharp
using ISOCodex.Currency;
using ISOCodex.Currency.Countries;
using ISOCodex.Countries;

var country = CountryAlpha2Code.Parse("GB");
var result = DefaultCountryCurrencyRegistry.Instance.Validate(
    country,
    CurrencyCode.GBP,
    CountryCurrencyValidationPolicy.PrimaryTenderOnly);

if (result.Succeeded)
{
    var currency = result.CountryCurrency!.CurrencyCode;
}
```

The initial seed is deliberately small and currently covers:

- GB/GBP
- US/USD
- IE/EUR
- JP/JPY
- CH/CHF
- CA/CAD
- AU/AUD
- NZ/NZD

This package does not duplicate country-code types. Country codes come from `ISOCodex.Countries`, and currencies come from `ISOCodex.Currency`.

The seed is not geopolitical authority and is not a complete legal-tender dataset. Treat it as a small bridge for common validation examples.
