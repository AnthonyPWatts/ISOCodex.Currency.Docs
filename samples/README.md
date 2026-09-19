# Runnable examples

Install the stable .NET 10 SDK (10.0.401 or later in 10.0). Clone this public repository, then choose an example:

| Example | Demonstrates |
| --- | --- |
| [CheckoutPricingApi](CheckoutPricingApi/README.md) | Checkout totals, tax and explicit rounding over HTTP. |
| [BulkMoneyImportTool](BulkMoneyImportTool/README.md) | Mixed-currency CSV validation and rounding. |

To restore, build and exercise all examples, including real HTTP requests, run:

```powershell
pwsh ./eng/verify-samples.ps1
```

The verifier restores packages from NuGet.org into a fresh cache and records package provenance and smoke-test output under `artifacts/`. It starts web examples on temporary loopback ports and stops only the processes it created. Framework execution requires Windows; the Addressing verification workflow uses Windows.

Samples are covered by the repository MIT licence. Bundled third-party web assets retain their accompanying licences.
