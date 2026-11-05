# \IntegrationsAPI

All URIs are relative to *https://api.licensemanager.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AuthorizeSlack**](IntegrationsAPI.md#AuthorizeSlack) | **Post** /v1/products/{productId}/integrations/slack/authorize | Start connecting a Slack channel
[**CheckIntegration**](IntegrationsAPI.md#CheckIntegration) | **Post** /v1/integrations/{id}/check | Check an integration
[**ConnectStripe**](IntegrationsAPI.md#ConnectStripe) | **Put** /v1/products/{productId}/integrations/stripe | Connect Stripe
[**CreateStripeMapping**](IntegrationsAPI.md#CreateStripeMapping) | **Post** /v1/products/{productId}/integrations/stripe/mappings | Map a Stripe price to a policy
[**DeleteSlackConnection**](IntegrationsAPI.md#DeleteSlackConnection) | **Delete** /v1/slack-connections/{id} | Remove a Slack connection
[**DeleteStripeMapping**](IntegrationsAPI.md#DeleteStripeMapping) | **Delete** /v1/integration-mappings/{id} | Delete a mapping
[**DisconnectIntegration**](IntegrationsAPI.md#DisconnectIntegration) | **Delete** /v1/integrations/{id} | Disconnect an integration
[**GetSlackIntegration**](IntegrationsAPI.md#GetSlackIntegration) | **Get** /v1/products/{productId}/integrations/slack | Get the Slack integration of a product
[**GetStripeIntegration**](IntegrationsAPI.md#GetStripeIntegration) | **Get** /v1/products/{productId}/integrations/stripe | Get the Stripe integration of a product
[**ListStripePrices**](IntegrationsAPI.md#ListStripePrices) | **Get** /v1/integrations/{id}/stripe/prices | List the Stripe prices of an integration
[**TestSlackConnection**](IntegrationsAPI.md#TestSlackConnection) | **Post** /v1/slack-connections/{id}/test | Send a test message to a Slack channel
[**UpdateIntegration**](IntegrationsAPI.md#UpdateIntegration) | **Patch** /v1/integrations/{id} | Update an integration
[**UpdateSlackConnection**](IntegrationsAPI.md#UpdateSlackConnection) | **Patch** /v1/slack-connections/{id} | Update a Slack connection
[**UpdateStripeMapping**](IntegrationsAPI.md#UpdateStripeMapping) | **Patch** /v1/integration-mappings/{id} | Change the policy of a mapping



## AuthorizeSlack

> SlackAuthorize AuthorizeSlack(ctx, productId).Execute()

Start connecting a Slack channel



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
	resp, r, err := apiClient.IntegrationsAPI.AuthorizeSlack(context.Background(), productId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.AuthorizeSlack``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AuthorizeSlack`: SlackAuthorize
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.AuthorizeSlack`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiAuthorizeSlackRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**SlackAuthorize**](SlackAuthorize.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


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


## DeleteSlackConnection

> DeleteSlackConnection(ctx, id).Execute()

Remove a Slack connection



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
	id := "s4Hq8ZpLm" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.IntegrationsAPI.DeleteSlackConnection(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.DeleteSlackConnection``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteSlackConnectionRequest struct via the builder pattern


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


## GetSlackIntegration

> SlackIntegration GetSlackIntegration(ctx, productId).Execute()

Get the Slack integration of a product



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
	resp, r, err := apiClient.IntegrationsAPI.GetSlackIntegration(context.Background(), productId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.GetSlackIntegration``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSlackIntegration`: SlackIntegration
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.GetSlackIntegration`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSlackIntegrationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**SlackIntegration**](SlackIntegration.md)

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


## TestSlackConnection

> SlackConnection TestSlackConnection(ctx, id).Execute()

Send a test message to a Slack channel



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
	id := "s4Hq8ZpLm" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.TestSlackConnection(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.TestSlackConnection``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TestSlackConnection`: SlackConnection
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.TestSlackConnection`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiTestSlackConnectionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**SlackConnection**](SlackConnection.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateIntegration

> Integration UpdateIntegration(ctx, id).UpdateIntegration(updateIntegration).Execute()

Update an integration



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
	updateIntegration := *openapiclient.NewUpdateIntegration() // UpdateIntegration | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.UpdateIntegration(context.Background(), id).UpdateIntegration(updateIntegration).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.UpdateIntegration``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateIntegration`: Integration
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.UpdateIntegration`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateIntegrationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateIntegration** | [**UpdateIntegration**](UpdateIntegration.md) |  | 

### Return type

[**Integration**](Integration.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateSlackConnection

> SlackConnection UpdateSlackConnection(ctx, id).UpdateSlackConnection(updateSlackConnection).Execute()

Update a Slack connection



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
	id := "s4Hq8ZpLm" // string | 
	updateSlackConnection := *openapiclient.NewUpdateSlackConnection([]string{"Events_example"}) // UpdateSlackConnection | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.UpdateSlackConnection(context.Background(), id).UpdateSlackConnection(updateSlackConnection).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.UpdateSlackConnection``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateSlackConnection`: SlackConnection
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.UpdateSlackConnection`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateSlackConnectionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateSlackConnection** | [**UpdateSlackConnection**](UpdateSlackConnection.md) |  | 

### Return type

[**SlackConnection**](SlackConnection.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
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

