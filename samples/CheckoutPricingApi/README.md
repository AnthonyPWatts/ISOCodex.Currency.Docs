# CheckoutPricingApi

Checkout totals, tax and explicit rounding over HTTP.

Requires the .NET 10 SDK selected by the repository `global.json`. Run from the repository root:

```powershell
dotnet run --project samples/CheckoutPricingApi --no-launch-profile --urls http://localhost:5003
```

Open [the endpoint index](http://localhost:5003/) or use the requests in [CheckoutPricingApi.http](CheckoutPricingApi.http). This local demonstration has no persistence or authentication and is not a production service.

All ISOCodex references use published NuGet packages. No private checkout, credentials or project references are needed.
