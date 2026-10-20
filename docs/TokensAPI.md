# \TokensAPI

All URIs are relative to *https://api.licensemanager.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateCustomerToken**](TokensAPI.md#CreateCustomerToken) | **Post** /v1/customers/{id}/tokens | Create a customer token
[**CreateLicenseToken**](TokensAPI.md#CreateLicenseToken) | **Post** /v1/licenses/{id}/tokens | Create a license token
[**CreateMachineToken**](TokensAPI.md#CreateMachineToken) | **Post** /v1/machines/{id}/tokens | Create a machine token



## CreateCustomerToken

> Token CreateCustomerToken(ctx, id).CreateToken(createToken).Execute()

Create a customer token



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
	createToken := *openapiclient.NewCreateToken([]string{"Scope_example"}) // CreateToken | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TokensAPI.CreateCustomerToken(context.Background(), id).CreateToken(createToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TokensAPI.CreateCustomerToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCustomerToken`: Token
	fmt.Fprintf(os.Stdout, "Response from `TokensAPI.CreateCustomerToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateCustomerTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createToken** | [**CreateToken**](CreateToken.md) |  | 

### Return type

[**Token**](Token.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateLicenseToken

> Token CreateLicenseToken(ctx, id).CreateToken(createToken).Execute()

Create a license token



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
	createToken := *openapiclient.NewCreateToken([]string{"Scope_example"}) // CreateToken | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TokensAPI.CreateLicenseToken(context.Background(), id).CreateToken(createToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TokensAPI.CreateLicenseToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateLicenseToken`: Token
	fmt.Fprintf(os.Stdout, "Response from `TokensAPI.CreateLicenseToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateLicenseTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createToken** | [**CreateToken**](CreateToken.md) |  | 

### Return type

[**Token**](Token.md)

### Authorization

[apiKey](../README.md#apiKey), [token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateMachineToken

> Token CreateMachineToken(ctx, id).CreateToken(createToken).Execute()

Create a machine token



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
	createToken := *openapiclient.NewCreateToken([]string{"Scope_example"}) // CreateToken | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TokensAPI.CreateMachineToken(context.Background(), id).CreateToken(createToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TokensAPI.CreateMachineToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateMachineToken`: Token
	fmt.Fprintf(os.Stdout, "Response from `TokensAPI.CreateMachineToken`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateMachineTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createToken** | [**CreateToken**](CreateToken.md) |  | 

### Return type

[**Token**](Token.md)

### Authorization

[apiKey](../README.md#apiKey), [token](../README.md#token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

