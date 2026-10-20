# LicenseManager Go SDK

[![Go Reference](https://pkg.go.dev/badge/github.com/licenseman/licensemanager-go.svg)](https://pkg.go.dev/github.com/licenseman/licensemanager-go)
[![Release](https://img.shields.io/github/v/tag/licenseman/licensemanager-go?sort=semver&label=release)](https://github.com/licenseman/licensemanager-go/tags)
[![Go version](https://img.shields.io/github/go-mod/go-version/licenseman/licensemanager-go)](https://github.com/licenseman/licensemanager-go/blob/main/go.mod)
[![Go Report Card](https://goreportcard.com/badge/github.com/licenseman/licensemanager-go)](https://goreportcard.com/report/github.com/licenseman/licensemanager-go)
[![License](https://img.shields.io/github/license/licenseman/licensemanager-go)](https://github.com/licenseman/licensemanager-go/blob/main/LICENSE)
[![Documentation](https://img.shields.io/badge/docs-licensemanager.dev-blue)](https://licensemanager.dev/docs/sdks/go)

The official Go SDK for the [LicenseManager](https://licensemanager.dev) API: issue, manage and validate software licenses. Idiomatic Go client with a `context.Context` on every call.

**[Documentation](https://licensemanager.dev/docs/sdks/go)** · **[API reference](https://api.licensemanager.dev/docs)** · **[Changelog](CHANGELOG.md)**

## Requirements

Go 1.23 or later.

## Installation

```sh
go get github.com/licenseman/licensemanager-go
```

## Usage

Create an API key in the LicenseManager app, then create a license after a sale:

```go
package main

import (
	"context"
	"log"
	"os"

	licensemanager "github.com/licenseman/licensemanager-go"
)

func main() {
	client := licensemanager.NewAPIClient(licensemanager.NewConfiguration())
	ctx := context.WithValue(context.Background(), licensemanager.ContextAPIKeys, map[string]licensemanager.APIKey{
		"apiKey": {Key: os.Getenv("LICENSEMANAGER_API_KEY")},
	})

	license, _, err := client.LicensesAPI.CreateLicense(ctx, "x7Kp2QaZ").
		CreateLicense(*licensemanager.NewCreateLicense("jane@example.com")).
		Execute()
	if err != nil {
		log.Fatal(err)
	}
	log.Println(license)
}
```

And validate it from your application, which needs no API key:

```go
package main

import (
	"context"
	"log"

	licensemanager "github.com/licenseman/licensemanager-go"
)

func main() {
	client := licensemanager.NewAPIClient(licensemanager.NewConfiguration())
	ctx := context.Background()

	licenseToken, _, err := client.LicensesAPI.ValidateKey(ctx, "x7Kp2QaZ").
		ValidateKey(*licensemanager.NewValidateKey("7KQ2M-X9ZPA-H4TRC-WN6EY-B3JDF", "4c:32:75:8f:9a:1e", "1.4.2")).
		Execute()
	if err != nil {
		log.Fatal(err)
	}
	log.Println(licenseToken)
}
```

## Authentication

Most endpoints take an organization API key: keep it on your servers. The endpoints your application calls directly, like validating a key, take no credentials or a token scoped to a customer, license or machine. See [authentication](https://licensemanager.dev/docs/api/authentication) and [scoped tokens](https://licensemanager.dev/docs/api/scoped-tokens).

```go
// With an API key, from your backend:
ctx := context.WithValue(context.Background(), licensemanager.ContextAPIKeys, map[string]licensemanager.APIKey{
	"apiKey": {Key: os.Getenv("LICENSEMANAGER_API_KEY")},
})

// With a token scoped to a customer, license or machine:
ctx = context.WithValue(context.Background(), licensemanager.ContextAccessToken, token)
```

## Errors

Failed requests answer an error with a stable `code` to branch on, listed for each endpoint in the [API reference](https://api.licensemanager.dev/docs). See [errors](https://licensemanager.dev/docs/api/errors).

```go
_, _, err := client.LicensesAPI.GetLicense(ctx, "l3Nv8KwB").Execute()
var apiErr *licensemanager.GenericOpenAPIError
if errors.As(err, &apiErr) {
	// The body is { "error": { "code", "message" } }.
	log.Println(apiErr.Error(), string(apiErr.Body()))
}
```

## Reference

Every method is documented, with its parameters and responses, in the [`docs`](docs) folder:

| Class | Methods |
| --- | --- |
| [`LicensesAPI`](docs/LicensesAPI.md) | `ValidateKey`, `ListLicenses`, `CreateLicense`, `ListCustomerLicenses`, `GetLicense`, `DeleteLicense`, `UpdateLicense`, `GetLicenseStats`, `SendLicenseKeys`, `GetSigningKey` |
| [`PortalAPI`](docs/PortalAPI.md) | `GetPortal`, `RequestPortalLink`, `CreatePortalLink`, `SendPortalLink` |
| [`ProductsAPI`](docs/ProductsAPI.md) | `ListProducts`, `CreateProduct`, `GetProduct`, `DeleteProduct`, `UpdateProduct`, `ResetProduct`, `UploadProductLogo`, `DeleteProductLogo`, `GetProductStats` |
| [`PoliciesAPI`](docs/PoliciesAPI.md) | `ListPolicies`, `CreatePolicy`, `GetPolicy`, `DeletePolicy`, `UpdatePolicy` |
| [`CustomersAPI`](docs/CustomersAPI.md) | `ListCustomers`, `CreateCustomer`, `GetCustomer`, `DeleteCustomer`, `UpdateCustomer` |
| [`MachinesAPI`](docs/MachinesAPI.md) | `ListMachines`, `GetMachine`, `DeactivateMachine` |
| [`ReleasesAPI`](docs/ReleasesAPI.md) | `ListReleases`, `CreateRelease`, `GetRelease`, `DeleteRelease`, `UpdateRelease` |
| [`TokensAPI`](docs/TokensAPI.md) | `CreateCustomerToken`, `CreateLicenseToken`, `CreateMachineToken` |
| [`EventsAPI`](docs/EventsAPI.md) | `ListPolicyEvents`, `ListLicenseEvents` |
| [`IntegrationsAPI`](docs/IntegrationsAPI.md) | `GetStripeIntegration`, `ConnectStripe`, `DisconnectIntegration`, `CheckIntegration`, `ListStripePrices`, `CreateStripeMapping`, `DeleteStripeMapping`, `UpdateStripeMapping` |

## Versioning

This SDK follows [semantic versioning](https://semver.org) and is generated from the [OpenAPI document](openapi.json) of the API: each release is listed in the [changelog](CHANGELOG.md). Please don't open pull requests, they would be overwritten by the next release: [open an issue](https://github.com/licenseman/licensemanager-go/issues) instead.

## License

See [LICENSE](LICENSE).
