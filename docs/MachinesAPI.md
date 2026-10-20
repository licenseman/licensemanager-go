# \MachinesAPI

All URIs are relative to *https://api.licensemanager.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeactivateMachine**](MachinesAPI.md#DeactivateMachine) | **Post** /v1/machines/{id}/deactivate | Deactivate a machine
[**GetMachine**](MachinesAPI.md#GetMachine) | **Get** /v1/machines/{id} | Get a machine
[**ListMachines**](MachinesAPI.md#ListMachines) | **Get** /v1/licenses/{licenseId}/machines | List the machines of a license



## DeactivateMachine

> Machine DeactivateMachine(ctx, id).Execute()

Deactivate a machine



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
	id := "m9Tq3VhD" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MachinesAPI.DeactivateMachine(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MachinesAPI.DeactivateMachine``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeactivateMachine`: Machine
	fmt.Fprintf(os.Stdout, "Response from `MachinesAPI.DeactivateMachine`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeactivateMachineRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Machine**](Machine.md)

### Authorization

[apiKey](../README.md#apiKey), [token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMachine

> Machine GetMachine(ctx, id).Execute()

Get a machine



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
	id := "m9Tq3VhD" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MachinesAPI.GetMachine(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MachinesAPI.GetMachine``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMachine`: Machine
	fmt.Fprintf(os.Stdout, "Response from `MachinesAPI.GetMachine`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMachineRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Machine**](Machine.md)

### Authorization

[apiKey](../README.md#apiKey), [token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListMachines

> MachineList ListMachines(ctx, licenseId).Page(page).PageSize(pageSize).Sort(sort).Search(search).Fingerprint(fingerprint).Status(status).Execute()

List the machines of a license



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
	licenseId := "l3Nv8KwB" // string | 
	page := int32(1) // int32 | Page to return. Pages are numbered from 1: `1` is the first page. A page past the last one returns an empty `data`, not an error. Defaults to `1`. (optional) (default to 1)
	pageSize := int32(20) // int32 | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to `20`. (optional) (default to 20)
	sort := "-createdAt" // string | Field to sort by, prefixed with `-` for descending order. Defaults to `-createdAt`. (optional) (default to "-createdAt")
	search := "macbook" // string | Case-insensitive text the fingerprint or name contains. (optional)
	fingerprint := "4c:32:75:8f:9a:1e" // string | Only returns the machine with this exact fingerprint. (optional)
	status := "active" // string | Only returns the machines with this status. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MachinesAPI.ListMachines(context.Background(), licenseId).Page(page).PageSize(pageSize).Sort(sort).Search(search).Fingerprint(fingerprint).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MachinesAPI.ListMachines``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListMachines`: MachineList
	fmt.Fprintf(os.Stdout, "Response from `MachinesAPI.ListMachines`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**licenseId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListMachinesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page to return. Pages are numbered from 1: &#x60;1&#x60; is the first page. A page past the last one returns an empty &#x60;data&#x60;, not an error. Defaults to &#x60;1&#x60;. | [default to 1]
 **pageSize** | **int32** | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to &#x60;20&#x60;. | [default to 20]
 **sort** | **string** | Field to sort by, prefixed with &#x60;-&#x60; for descending order. Defaults to &#x60;-createdAt&#x60;. | [default to &quot;-createdAt&quot;]
 **search** | **string** | Case-insensitive text the fingerprint or name contains. | 
 **fingerprint** | **string** | Only returns the machine with this exact fingerprint. | 
 **status** | **string** | Only returns the machines with this status. | 

### Return type

[**MachineList**](MachineList.md)

### Authorization

[apiKey](../README.md#apiKey), [token](../README.md#token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

