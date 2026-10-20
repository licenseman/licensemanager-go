# \EventsAPI

All URIs are relative to *https://api.licensemanager.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListLicenseEvents**](EventsAPI.md#ListLicenseEvents) | **Get** /v1/licenses/{id}/events | List the events of a license
[**ListPolicyEvents**](EventsAPI.md#ListPolicyEvents) | **Get** /v1/policies/{id}/events | List the events of a policy



## ListLicenseEvents

> EventList ListLicenseEvents(ctx, id).Page(page).PageSize(pageSize).Sort(sort).Type_(type_).MachineId(machineId).Execute()

List the events of a license



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
	page := int32(1) // int32 | Page to return. Pages are numbered from 1: `1` is the first page. A page past the last one returns an empty `data`, not an error. Defaults to `1`. (optional) (default to 1)
	pageSize := int32(20) // int32 | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to `20`. (optional) (default to 20)
	sort := "-createdAt" // string | Field to sort by, prefixed with `-` for descending order. Defaults to `-createdAt`. (optional) (default to "-createdAt")
	type_ := *openapiclient.NewListPolicyEventsTypeParameter() // ListPolicyEventsTypeParameter | Only returns the events of this type. Repeat it to return the events of any of these types. (optional)
	machineId := "m9Tq3VhD" // string | Only returns the events of this machine of the license. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EventsAPI.ListLicenseEvents(context.Background(), id).Page(page).PageSize(pageSize).Sort(sort).Type_(type_).MachineId(machineId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EventsAPI.ListLicenseEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListLicenseEvents`: EventList
	fmt.Fprintf(os.Stdout, "Response from `EventsAPI.ListLicenseEvents`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListLicenseEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page to return. Pages are numbered from 1: &#x60;1&#x60; is the first page. A page past the last one returns an empty &#x60;data&#x60;, not an error. Defaults to &#x60;1&#x60;. | [default to 1]
 **pageSize** | **int32** | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to &#x60;20&#x60;. | [default to 20]
 **sort** | **string** | Field to sort by, prefixed with &#x60;-&#x60; for descending order. Defaults to &#x60;-createdAt&#x60;. | [default to &quot;-createdAt&quot;]
 **type_** | [**ListPolicyEventsTypeParameter**](ListPolicyEventsTypeParameter.md) | Only returns the events of this type. Repeat it to return the events of any of these types. | 
 **machineId** | **string** | Only returns the events of this machine of the license. | 

### Return type

[**EventList**](EventList.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPolicyEvents

> EventList ListPolicyEvents(ctx, id).Page(page).PageSize(pageSize).Sort(sort).Type_(type_).Execute()

List the events of a policy



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
	page := int32(1) // int32 | Page to return. Pages are numbered from 1: `1` is the first page. A page past the last one returns an empty `data`, not an error. Defaults to `1`. (optional) (default to 1)
	pageSize := int32(20) // int32 | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to `20`. (optional) (default to 20)
	sort := "-createdAt" // string | Field to sort by, prefixed with `-` for descending order. Defaults to `-createdAt`. (optional) (default to "-createdAt")
	type_ := *openapiclient.NewListPolicyEventsTypeParameter() // ListPolicyEventsTypeParameter | Only returns the events of this type. Repeat it to return the events of any of these types. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EventsAPI.ListPolicyEvents(context.Background(), id).Page(page).PageSize(pageSize).Sort(sort).Type_(type_).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EventsAPI.ListPolicyEvents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPolicyEvents`: EventList
	fmt.Fprintf(os.Stdout, "Response from `EventsAPI.ListPolicyEvents`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListPolicyEventsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page to return. Pages are numbered from 1: &#x60;1&#x60; is the first page. A page past the last one returns an empty &#x60;data&#x60;, not an error. Defaults to &#x60;1&#x60;. | [default to 1]
 **pageSize** | **int32** | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to &#x60;20&#x60;. | [default to 20]
 **sort** | **string** | Field to sort by, prefixed with &#x60;-&#x60; for descending order. Defaults to &#x60;-createdAt&#x60;. | [default to &quot;-createdAt&quot;]
 **type_** | [**ListPolicyEventsTypeParameter**](ListPolicyEventsTypeParameter.md) | Only returns the events of this type. Repeat it to return the events of any of these types. | 

### Return type

[**EventList**](EventList.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

