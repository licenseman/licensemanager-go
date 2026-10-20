# \PortalAPI

All URIs are relative to *https://api.licensemanager.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreatePortalLink**](PortalAPI.md#CreatePortalLink) | **Post** /v1/customers/{id}/portal-links | Create a link to the customer portal
[**GetPortal**](PortalAPI.md#GetPortal) | **Get** /v1/portal/{productId} | Get the customer portal of a product
[**RequestPortalLink**](PortalAPI.md#RequestPortalLink) | **Post** /v1/portal/{productId}/request-link | Email a link to the customer portal
[**SendPortalLink**](PortalAPI.md#SendPortalLink) | **Post** /v1/customers/{id}/portal-links/send | Email a link to the customer portal to the customer



## CreatePortalLink

> PortalLink CreatePortalLink(ctx, id).CreatePortalLink(createPortalLink).Execute()

Create a link to the customer portal



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
	id := "c9Wd3RtE" // string | 
	createPortalLink := *openapiclient.NewCreatePortalLink(int32(604800)) // CreatePortalLink | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PortalAPI.CreatePortalLink(context.Background(), id).CreatePortalLink(createPortalLink).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PortalAPI.CreatePortalLink``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreatePortalLink`: PortalLink
	fmt.Fprintf(os.Stdout, "Response from `PortalAPI.CreatePortalLink`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreatePortalLinkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createPortalLink** | [**CreatePortalLink**](CreatePortalLink.md) |  | 

### Return type

[**PortalLink**](PortalLink.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetPortal

> Portal GetPortal(ctx, productId).ReturnUrl(returnUrl).Execute()

Get the customer portal of a product



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
	returnUrl := "https://example.com/account" // string | Link back to your website to show, used when its domain is one of the product's `returnDomains`. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PortalAPI.GetPortal(context.Background(), productId).ReturnUrl(returnUrl).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PortalAPI.GetPortal``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPortal`: Portal
	fmt.Fprintf(os.Stdout, "Response from `PortalAPI.GetPortal`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetPortalRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **returnUrl** | **string** | Link back to your website to show, used when its domain is one of the product&#39;s &#x60;returnDomains&#x60;. | 

### Return type

[**Portal**](Portal.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RequestPortalLink

> RequestPortalLink(ctx, productId).RequestPortalLink(requestPortalLink).Execute()

Email a link to the customer portal



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
	requestPortalLink := *openapiclient.NewRequestPortalLink("jane@example.com") // RequestPortalLink | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.PortalAPI.RequestPortalLink(context.Background(), productId).RequestPortalLink(requestPortalLink).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PortalAPI.RequestPortalLink``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiRequestPortalLinkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **requestPortalLink** | [**RequestPortalLink**](RequestPortalLink.md) |  | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SendPortalLink

> SendPortalLink(ctx, id).SendPortalLink(sendPortalLink).Execute()

Email a link to the customer portal to the customer



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
	id := "c9Wd3RtE" // string | 
	sendPortalLink := *openapiclient.NewSendPortalLink("eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9…") // SendPortalLink | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.PortalAPI.SendPortalLink(context.Background(), id).SendPortalLink(sendPortalLink).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PortalAPI.SendPortalLink``: %v\n", err)
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

Other parameters are passed through a pointer to a apiSendPortalLinkRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **sendPortalLink** | [**SendPortalLink**](SendPortalLink.md) |  | 

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

