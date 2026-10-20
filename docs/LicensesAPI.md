# \LicensesAPI

All URIs are relative to *https://api.licensemanager.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateLicense**](LicensesAPI.md#CreateLicense) | **Post** /v1/products/{productId}/licenses | Create a license
[**DeleteLicense**](LicensesAPI.md#DeleteLicense) | **Delete** /v1/licenses/{id} | Delete a license
[**GetLicense**](LicensesAPI.md#GetLicense) | **Get** /v1/licenses/{id} | Get a license
[**GetLicenseStats**](LicensesAPI.md#GetLicenseStats) | **Get** /v1/licenses/{id}/stats | Get the stats of a license
[**GetSigningKey**](LicensesAPI.md#GetSigningKey) | **Get** /v1/signing-key | Get the organization&#39;s signing key
[**ListCustomerLicenses**](LicensesAPI.md#ListCustomerLicenses) | **Get** /v1/customers/{customerId}/licenses | List the licenses of a customer
[**ListLicenses**](LicensesAPI.md#ListLicenses) | **Get** /v1/products/{productId}/licenses | List the licenses of a product
[**SendLicenseKeys**](LicensesAPI.md#SendLicenseKeys) | **Post** /v1/licenses/send-keys | Email license keys to their customers
[**UpdateLicense**](LicensesAPI.md#UpdateLicense) | **Patch** /v1/licenses/{id} | Update a license
[**ValidateKey**](LicensesAPI.md#ValidateKey) | **Post** /v1/products/{productId}/validate-key | Validate a license key



## CreateLicense

> License CreateLicense(ctx, productId).CreateLicense(createLicense).Execute()

Create a license



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	productId := "x7Kp2QaZ" // string | 
	createLicense := *openapiclient.NewCreateLicense("jane@example.com") // CreateLicense | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicensesAPI.CreateLicense(context.Background(), productId).CreateLicense(createLicense).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.CreateLicense``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateLicense`: License
	fmt.Fprintf(os.Stdout, "Response from `LicensesAPI.CreateLicense`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateLicenseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createLicense** | [**CreateLicense**](CreateLicense.md) |  | 

### Return type

[**License**](License.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteLicense

> DeleteLicense(ctx, id).Execute()

Delete a license



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	id := "l3Nv8KwB" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.LicensesAPI.DeleteLicense(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.DeleteLicense``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteLicenseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetLicense

> License GetLicense(ctx, id).Execute()

Get a license



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	id := "l3Nv8KwB" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicensesAPI.GetLicense(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.GetLicense``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetLicense`: License
	fmt.Fprintf(os.Stdout, "Response from `LicensesAPI.GetLicense`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetLicenseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**License**](License.md)

### Authorization

[apiKey](../README.md#apiKey), [token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetLicenseStats

> LicenseStats GetLicenseStats(ctx, id).Execute()

Get the stats of a license



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	id := "l3Nv8KwB" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicensesAPI.GetLicenseStats(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.GetLicenseStats``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetLicenseStats`: LicenseStats
	fmt.Fprintf(os.Stdout, "Response from `LicensesAPI.GetLicenseStats`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetLicenseStatsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**LicenseStats**](LicenseStats.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetSigningKey

> SigningKey GetSigningKey(ctx).Execute()

Get the organization's signing key



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicensesAPI.GetSigningKey(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.GetSigningKey``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSigningKey`: SigningKey
	fmt.Fprintf(os.Stdout, "Response from `LicensesAPI.GetSigningKey`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetSigningKeyRequest struct via the builder pattern


### Return type

[**SigningKey**](SigningKey.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCustomerLicenses

> LicenseList ListCustomerLicenses(ctx, customerId).Page(page).PageSize(pageSize).Sort(sort).Search(search).Key(key).PolicyId(policyId).MachineVersion(machineVersion).Status(status).CreatedFrom(createdFrom).CreatedTo(createdTo).LastActivatedFrom(lastActivatedFrom).LastActivatedTo(lastActivatedTo).NeverActivated(neverActivated).ExpiresFrom(expiresFrom).ExpiresTo(expiresTo).NeverExpires(neverExpires).Currency(currency).Price(price).PriceMin(priceMin).PriceMax(priceMax).HasPrice(hasPrice).Execute()

List the licenses of a customer



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	customerId := "c9Wd3RtE" // string | 
	page := int32(1) // int32 | Page to return. Pages are numbered from 1: `1` is the first page. A page past the last one returns an empty `data`, not an error. Defaults to `1`. (optional) (default to 1)
	pageSize := int32(20) // int32 | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to `20`. (optional) (default to 20)
	sort := "-createdAt" // string | Field to sort by, prefixed with `-` for descending order. Defaults to `-createdAt`. (optional) (default to "-createdAt")
	search := "X9ZPA" // string | Case-insensitive text the key contains. (optional)
	key := "7KQ2M-X9ZPA-H4TRC-WN6EY-B3JDF" // string | Only returns the license with this exact key, case included. Keys of test products start with `TEST-`. (optional)
	policyId := "p4Rt8LmQ" // string | Only returns the licenses following this policy. (optional)
	machineVersion := "2.3.1" // string | Only returns the licenses with at least one active machine running this version of the product. (optional)
	status := openapiclient.LicenseStatus("active") // LicenseStatus | Only returns the licenses with this status. (optional)
	createdFrom := time.Now() // time.Time | Only returns the licenses created at or after this date. (optional)
	createdTo := time.Now() // time.Time | Only returns the licenses created at or before this date. (optional)
	lastActivatedFrom := time.Now() // time.Time | Only returns the licenses last activated at or after this date. Licenses never activated are left out. (optional)
	lastActivatedTo := time.Now() // time.Time | Only returns the licenses last activated at or before this date. Licenses never activated are left out. (optional)
	neverActivated := "true" // string | `true` only returns the licenses never activated, `false` only the ones activated at least once. (optional)
	expiresFrom := time.Now() // time.Time | Only returns the licenses expiring at or after this date. Licenses that never expire are left out. (optional)
	expiresTo := time.Now() // time.Time | Only returns the licenses expiring at or before this date. Licenses that never expire are left out. (optional)
	neverExpires := "true" // string | `true` only returns the licenses that never expire, `false` only the ones with an expiration date. (optional)
	currency := "USD" // string | Only returns the licenses paid in this currency. (optional)
	price := float32(49.99) // float32 | Only returns the licenses paid exactly this amount, in major units of its currency: combine with `currency` to compare amounts of one currency. Licenses without a price are left out. (optional)
	priceMin := float32(49.99) // float32 | Only returns the licenses paid at least this amount, in major units of its currency: combine with `currency` to compare amounts of one currency. Licenses without a price are left out. (optional)
	priceMax := float32(49.99) // float32 | Only returns the licenses paid at most this amount, in major units of its currency: combine with `currency` to compare amounts of one currency. Licenses without a price are left out. (optional)
	hasPrice := "true" // string | `true` only returns the licenses with a price, `false` only the ones without. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicensesAPI.ListCustomerLicenses(context.Background(), customerId).Page(page).PageSize(pageSize).Sort(sort).Search(search).Key(key).PolicyId(policyId).MachineVersion(machineVersion).Status(status).CreatedFrom(createdFrom).CreatedTo(createdTo).LastActivatedFrom(lastActivatedFrom).LastActivatedTo(lastActivatedTo).NeverActivated(neverActivated).ExpiresFrom(expiresFrom).ExpiresTo(expiresTo).NeverExpires(neverExpires).Currency(currency).Price(price).PriceMin(priceMin).PriceMax(priceMax).HasPrice(hasPrice).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.ListCustomerLicenses``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCustomerLicenses`: LicenseList
	fmt.Fprintf(os.Stdout, "Response from `LicensesAPI.ListCustomerLicenses`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**customerId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListCustomerLicensesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page to return. Pages are numbered from 1: &#x60;1&#x60; is the first page. A page past the last one returns an empty &#x60;data&#x60;, not an error. Defaults to &#x60;1&#x60;. | [default to 1]
 **pageSize** | **int32** | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to &#x60;20&#x60;. | [default to 20]
 **sort** | **string** | Field to sort by, prefixed with &#x60;-&#x60; for descending order. Defaults to &#x60;-createdAt&#x60;. | [default to &quot;-createdAt&quot;]
 **search** | **string** | Case-insensitive text the key contains. | 
 **key** | **string** | Only returns the license with this exact key, case included. Keys of test products start with &#x60;TEST-&#x60;. | 
 **policyId** | **string** | Only returns the licenses following this policy. | 
 **machineVersion** | **string** | Only returns the licenses with at least one active machine running this version of the product. | 
 **status** | [**LicenseStatus**](LicenseStatus.md) | Only returns the licenses with this status. | 
 **createdFrom** | **time.Time** | Only returns the licenses created at or after this date. | 
 **createdTo** | **time.Time** | Only returns the licenses created at or before this date. | 
 **lastActivatedFrom** | **time.Time** | Only returns the licenses last activated at or after this date. Licenses never activated are left out. | 
 **lastActivatedTo** | **time.Time** | Only returns the licenses last activated at or before this date. Licenses never activated are left out. | 
 **neverActivated** | **string** | &#x60;true&#x60; only returns the licenses never activated, &#x60;false&#x60; only the ones activated at least once. | 
 **expiresFrom** | **time.Time** | Only returns the licenses expiring at or after this date. Licenses that never expire are left out. | 
 **expiresTo** | **time.Time** | Only returns the licenses expiring at or before this date. Licenses that never expire are left out. | 
 **neverExpires** | **string** | &#x60;true&#x60; only returns the licenses that never expire, &#x60;false&#x60; only the ones with an expiration date. | 
 **currency** | **string** | Only returns the licenses paid in this currency. | 
 **price** | **float32** | Only returns the licenses paid exactly this amount, in major units of its currency: combine with &#x60;currency&#x60; to compare amounts of one currency. Licenses without a price are left out. | 
 **priceMin** | **float32** | Only returns the licenses paid at least this amount, in major units of its currency: combine with &#x60;currency&#x60; to compare amounts of one currency. Licenses without a price are left out. | 
 **priceMax** | **float32** | Only returns the licenses paid at most this amount, in major units of its currency: combine with &#x60;currency&#x60; to compare amounts of one currency. Licenses without a price are left out. | 
 **hasPrice** | **string** | &#x60;true&#x60; only returns the licenses with a price, &#x60;false&#x60; only the ones without. | 

### Return type

[**LicenseList**](LicenseList.md)

### Authorization

[apiKey](../README.md#apiKey), [token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListLicenses

> LicenseList ListLicenses(ctx, productId).Page(page).PageSize(pageSize).Sort(sort).Search(search).Key(key).PolicyId(policyId).CustomerId(customerId).MachineVersion(machineVersion).Status(status).CreatedFrom(createdFrom).CreatedTo(createdTo).LastActivatedFrom(lastActivatedFrom).LastActivatedTo(lastActivatedTo).NeverActivated(neverActivated).ExpiresFrom(expiresFrom).ExpiresTo(expiresTo).NeverExpires(neverExpires).Currency(currency).Price(price).PriceMin(priceMin).PriceMax(priceMax).HasPrice(hasPrice).Execute()

List the licenses of a product



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	productId := "x7Kp2QaZ" // string | 
	page := int32(1) // int32 | Page to return. Pages are numbered from 1: `1` is the first page. A page past the last one returns an empty `data`, not an error. Defaults to `1`. (optional) (default to 1)
	pageSize := int32(20) // int32 | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to `20`. (optional) (default to 20)
	sort := "-createdAt" // string | Field to sort by, prefixed with `-` for descending order. Defaults to `-createdAt`. (optional) (default to "-createdAt")
	search := "X9ZPA" // string | Case-insensitive text the key contains. (optional)
	key := "7KQ2M-X9ZPA-H4TRC-WN6EY-B3JDF" // string | Only returns the license with this exact key, case included. Keys of test products start with `TEST-`. (optional)
	policyId := "p4Rt8LmQ" // string | Only returns the licenses following this policy. (optional)
	customerId := "c9Wd3RtE" // string | Only returns the licenses of this customer. (optional)
	machineVersion := "2.3.1" // string | Only returns the licenses with at least one active machine running this version of the product. (optional)
	status := openapiclient.LicenseStatus("active") // LicenseStatus | Only returns the licenses with this status. (optional)
	createdFrom := time.Now() // time.Time | Only returns the licenses created at or after this date. (optional)
	createdTo := time.Now() // time.Time | Only returns the licenses created at or before this date. (optional)
	lastActivatedFrom := time.Now() // time.Time | Only returns the licenses last activated at or after this date. Licenses never activated are left out. (optional)
	lastActivatedTo := time.Now() // time.Time | Only returns the licenses last activated at or before this date. Licenses never activated are left out. (optional)
	neverActivated := "true" // string | `true` only returns the licenses never activated, `false` only the ones activated at least once. (optional)
	expiresFrom := time.Now() // time.Time | Only returns the licenses expiring at or after this date. Licenses that never expire are left out. (optional)
	expiresTo := time.Now() // time.Time | Only returns the licenses expiring at or before this date. Licenses that never expire are left out. (optional)
	neverExpires := "true" // string | `true` only returns the licenses that never expire, `false` only the ones with an expiration date. (optional)
	currency := "USD" // string | Only returns the licenses paid in this currency. (optional)
	price := float32(49.99) // float32 | Only returns the licenses paid exactly this amount, in major units of its currency: combine with `currency` to compare amounts of one currency. Licenses without a price are left out. (optional)
	priceMin := float32(49.99) // float32 | Only returns the licenses paid at least this amount, in major units of its currency: combine with `currency` to compare amounts of one currency. Licenses without a price are left out. (optional)
	priceMax := float32(49.99) // float32 | Only returns the licenses paid at most this amount, in major units of its currency: combine with `currency` to compare amounts of one currency. Licenses without a price are left out. (optional)
	hasPrice := "true" // string | `true` only returns the licenses with a price, `false` only the ones without. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicensesAPI.ListLicenses(context.Background(), productId).Page(page).PageSize(pageSize).Sort(sort).Search(search).Key(key).PolicyId(policyId).CustomerId(customerId).MachineVersion(machineVersion).Status(status).CreatedFrom(createdFrom).CreatedTo(createdTo).LastActivatedFrom(lastActivatedFrom).LastActivatedTo(lastActivatedTo).NeverActivated(neverActivated).ExpiresFrom(expiresFrom).ExpiresTo(expiresTo).NeverExpires(neverExpires).Currency(currency).Price(price).PriceMin(priceMin).PriceMax(priceMax).HasPrice(hasPrice).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.ListLicenses``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListLicenses`: LicenseList
	fmt.Fprintf(os.Stdout, "Response from `LicensesAPI.ListLicenses`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListLicensesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page to return. Pages are numbered from 1: &#x60;1&#x60; is the first page. A page past the last one returns an empty &#x60;data&#x60;, not an error. Defaults to &#x60;1&#x60;. | [default to 1]
 **pageSize** | **int32** | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to &#x60;20&#x60;. | [default to 20]
 **sort** | **string** | Field to sort by, prefixed with &#x60;-&#x60; for descending order. Defaults to &#x60;-createdAt&#x60;. | [default to &quot;-createdAt&quot;]
 **search** | **string** | Case-insensitive text the key contains. | 
 **key** | **string** | Only returns the license with this exact key, case included. Keys of test products start with &#x60;TEST-&#x60;. | 
 **policyId** | **string** | Only returns the licenses following this policy. | 
 **customerId** | **string** | Only returns the licenses of this customer. | 
 **machineVersion** | **string** | Only returns the licenses with at least one active machine running this version of the product. | 
 **status** | [**LicenseStatus**](LicenseStatus.md) | Only returns the licenses with this status. | 
 **createdFrom** | **time.Time** | Only returns the licenses created at or after this date. | 
 **createdTo** | **time.Time** | Only returns the licenses created at or before this date. | 
 **lastActivatedFrom** | **time.Time** | Only returns the licenses last activated at or after this date. Licenses never activated are left out. | 
 **lastActivatedTo** | **time.Time** | Only returns the licenses last activated at or before this date. Licenses never activated are left out. | 
 **neverActivated** | **string** | &#x60;true&#x60; only returns the licenses never activated, &#x60;false&#x60; only the ones activated at least once. | 
 **expiresFrom** | **time.Time** | Only returns the licenses expiring at or after this date. Licenses that never expire are left out. | 
 **expiresTo** | **time.Time** | Only returns the licenses expiring at or before this date. Licenses that never expire are left out. | 
 **neverExpires** | **string** | &#x60;true&#x60; only returns the licenses that never expire, &#x60;false&#x60; only the ones with an expiration date. | 
 **currency** | **string** | Only returns the licenses paid in this currency. | 
 **price** | **float32** | Only returns the licenses paid exactly this amount, in major units of its currency: combine with &#x60;currency&#x60; to compare amounts of one currency. Licenses without a price are left out. | 
 **priceMin** | **float32** | Only returns the licenses paid at least this amount, in major units of its currency: combine with &#x60;currency&#x60; to compare amounts of one currency. Licenses without a price are left out. | 
 **priceMax** | **float32** | Only returns the licenses paid at most this amount, in major units of its currency: combine with &#x60;currency&#x60; to compare amounts of one currency. Licenses without a price are left out. | 
 **hasPrice** | **string** | &#x60;true&#x60; only returns the licenses with a price, &#x60;false&#x60; only the ones without. | 

### Return type

[**LicenseList**](LicenseList.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendLicenseKeys

> SendLicenseKeys(ctx).SendLicenseKeys(sendLicenseKeys).Execute()

Email license keys to their customers



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	sendLicenseKeys := *openapiclient.NewSendLicenseKeys([]string{"Ids_example"}) // SendLicenseKeys | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.LicensesAPI.SendLicenseKeys(context.Background()).SendLicenseKeys(sendLicenseKeys).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.SendLicenseKeys``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendLicenseKeysRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sendLicenseKeys** | [**SendLicenseKeys**](SendLicenseKeys.md) |  | 

### Return type

 (empty response body)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateLicense

> License UpdateLicense(ctx, id).UpdateLicense(updateLicense).Execute()

Update a license



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	id := "l3Nv8KwB" // string | 
	updateLicense := *openapiclient.NewUpdateLicense() // UpdateLicense | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicensesAPI.UpdateLicense(context.Background(), id).UpdateLicense(updateLicense).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.UpdateLicense``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateLicense`: License
	fmt.Fprintf(os.Stdout, "Response from `LicensesAPI.UpdateLicense`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateLicenseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateLicense** | [**UpdateLicense**](UpdateLicense.md) |  | 

### Return type

[**License**](License.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ValidateKey

> LicenseToken ValidateKey(ctx, productId).ValidateKey(validateKey).Execute()

Validate a license key



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/licenseman/licensemanager-go"
)

func main() {
	productId := "x7Kp2QaZ" // string | 
	validateKey := *openapiclient.NewValidateKey("7KQ2M-X9ZPA-H4TRC-WN6EY-B3JDF", "4c:32:75:8f:9a:1e", "1.4.2") // ValidateKey | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.LicensesAPI.ValidateKey(context.Background(), productId).ValidateKey(validateKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `LicensesAPI.ValidateKey``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ValidateKey`: LicenseToken
	fmt.Fprintf(os.Stdout, "Response from `LicensesAPI.ValidateKey`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiValidateKeyRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **validateKey** | [**ValidateKey**](ValidateKey.md) |  | 

### Return type

[**LicenseToken**](LicenseToken.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

