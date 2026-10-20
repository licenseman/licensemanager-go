# \IntegrationsAPI

All URIs are relative to *https://api.licensemanager.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CheckIntegration**](IntegrationsAPI.md#CheckIntegration) | **Post** /v1/integrations/{id}/check | Check an integration
[**ConnectStripe**](IntegrationsAPI.md#ConnectStripe) | **Put** /v1/products/{productId}/integrations/stripe | Connect Stripe
[**CreateStripeMapping**](IntegrationsAPI.md#CreateStripeMapping) | **Post** /v1/products/{productId}/integrations/stripe/mappings | Map a Stripe price to a policy
[**DeleteStripeMapping**](IntegrationsAPI.md#DeleteStripeMapping) | **Delete** /v1/integration-mappings/{id} | Delete a mapping
[**DisconnectIntegration**](IntegrationsAPI.md#DisconnectIntegration) | **Delete** /v1/integrations/{id} | Disconnect an integration
[**GetStripeIntegration**](IntegrationsAPI.md#GetStripeIntegration) | **Get** /v1/products/{productId}/integrations/stripe | Get the Stripe integration of a product
[**ListStripePrices**](IntegrationsAPI.md#ListStripePrices) | **Get** /v1/integrations/{id}/stripe/prices | List the Stripe prices of an integration
[**UpdateStripeMapping**](IntegrationsAPI.md#UpdateStripeMapping) | **Patch** /v1/integration-mappings/{id} | Change the policy of a mapping



## CheckIntegration

> Integration CheckIntegration(ctx, id).Execute()

Check an integration



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
	id := "i8Fz4QnRt" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.CheckIntegration(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.CheckIntegration``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CheckIntegration`: Integration
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.CheckIntegration`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCheckIntegrationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Integration**](Integration.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ConnectStripe

> StripeIntegration ConnectStripe(ctx, productId).ConnectStripe(connectStripe).Execute()

Connect Stripe



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
	connectStripe := *openapiclient.NewConnectStripe("rk_live_51Nv0FG…") // ConnectStripe | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.ConnectStripe(context.Background(), productId).ConnectStripe(connectStripe).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.ConnectStripe``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConnectStripe`: StripeIntegration
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.ConnectStripe`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiConnectStripeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **connectStripe** | [**ConnectStripe**](ConnectStripe.md) |  | 

### Return type

[**StripeIntegration**](StripeIntegration.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateStripeMapping

> IntegrationMapping CreateStripeMapping(ctx, productId).CreateIntegrationMapping(createIntegrationMapping).Execute()

Map a Stripe price to a policy



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
	createIntegrationMapping := *openapiclient.NewCreateIntegrationMapping("price_1MoBy5LkdIwHu7ix", "p4Rt8LmQ") // CreateIntegrationMapping | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.CreateStripeMapping(context.Background(), productId).CreateIntegrationMapping(createIntegrationMapping).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.CreateStripeMapping``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateStripeMapping`: IntegrationMapping
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.CreateStripeMapping`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateStripeMappingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createIntegrationMapping** | [**CreateIntegrationMapping**](CreateIntegrationMapping.md) |  | 

### Return type

[**IntegrationMapping**](IntegrationMapping.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteStripeMapping

> DeleteStripeMapping(ctx, id).Execute()

Delete a mapping



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
	id := "i8Fz4QnRt" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.IntegrationsAPI.DeleteStripeMapping(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.DeleteStripeMapping``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteStripeMappingRequest struct via the builder pattern


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


## DisconnectIntegration

> DisconnectIntegration(ctx, id).Execute()

Disconnect an integration



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
	id := "i8Fz4QnRt" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.IntegrationsAPI.DisconnectIntegration(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.DisconnectIntegration``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDisconnectIntegrationRequest struct via the builder pattern


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


## GetStripeIntegration

> StripeIntegration GetStripeIntegration(ctx, productId).Execute()

Get the Stripe integration of a product



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.GetStripeIntegration(context.Background(), productId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.GetStripeIntegration``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetStripeIntegration`: StripeIntegration
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.GetStripeIntegration`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetStripeIntegrationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**StripeIntegration**](StripeIntegration.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListStripePrices

> ListStripePrices200Response ListStripePrices(ctx, id).Execute()

List the Stripe prices of an integration



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
	id := "i8Fz4QnRt" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.ListStripePrices(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.ListStripePrices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListStripePrices`: ListStripePrices200Response
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.ListStripePrices`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListStripePricesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ListStripePrices200Response**](ListStripePrices200Response.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateStripeMapping

> IntegrationMapping UpdateStripeMapping(ctx, id).UpdateIntegrationMapping(updateIntegrationMapping).Execute()

Change the policy of a mapping



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
	id := "i8Fz4QnRt" // string | 
	updateIntegrationMapping := *openapiclient.NewUpdateIntegrationMapping("p4Rt8LmQ") // UpdateIntegrationMapping | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.UpdateStripeMapping(context.Background(), id).UpdateIntegrationMapping(updateIntegrationMapping).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.UpdateStripeMapping``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateStripeMapping`: IntegrationMapping
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.UpdateStripeMapping`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateStripeMappingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateIntegrationMapping** | [**UpdateIntegrationMapping**](UpdateIntegrationMapping.md) |  | 

### Return type

[**IntegrationMapping**](IntegrationMapping.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

