# \ReleasesAPI

All URIs are relative to *https://api.licensemanager.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateRelease**](ReleasesAPI.md#CreateRelease) | **Post** /v1/products/{productId}/releases | Create a release
[**DeleteRelease**](ReleasesAPI.md#DeleteRelease) | **Delete** /v1/releases/{id} | Delete a release
[**GetRelease**](ReleasesAPI.md#GetRelease) | **Get** /v1/releases/{id} | Get a release
[**ListReleases**](ReleasesAPI.md#ListReleases) | **Get** /v1/products/{productId}/releases | List the releases of a product
[**UpdateRelease**](ReleasesAPI.md#UpdateRelease) | **Patch** /v1/releases/{id} | Update a release



## CreateRelease

> Release CreateRelease(ctx, productId).CreateRelease(createRelease).Execute()

Create a release



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
	createRelease := *openapiclient.NewCreateRelease("2.3.1") // CreateRelease | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ReleasesAPI.CreateRelease(context.Background(), productId).CreateRelease(createRelease).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReleasesAPI.CreateRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateRelease`: Release
	fmt.Fprintf(os.Stdout, "Response from `ReleasesAPI.CreateRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createRelease** | [**CreateRelease**](CreateRelease.md) |  | 

### Return type

[**Release**](Release.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteRelease

> DeleteRelease(ctx, id).Execute()

Delete a release



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
	id := "r4Lm8VwX" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.ReleasesAPI.DeleteRelease(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReleasesAPI.DeleteRelease``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteReleaseRequest struct via the builder pattern


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


## GetRelease

> Release GetRelease(ctx, id).Execute()

Get a release

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
	id := "r4Lm8VwX" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ReleasesAPI.GetRelease(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReleasesAPI.GetRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRelease`: Release
	fmt.Fprintf(os.Stdout, "Response from `ReleasesAPI.GetRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Release**](Release.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListReleases

> ReleaseList ListReleases(ctx, productId).Page(page).PageSize(pageSize).Sort(sort).Search(search).ReleasedFrom(releasedFrom).ReleasedTo(releasedTo).ActiveMachineCount(activeMachineCount).ActiveMachineCountMin(activeMachineCountMin).ActiveMachineCountMax(activeMachineCountMax).Execute()

List the releases of a product



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
	sort := "-version" // string | Field to sort by, prefixed with `-` for descending order. Defaults to `-version`. (optional) (default to "-version")
	search := "2.3" // string | Case-insensitive text the version contains. (optional)
	releasedFrom := time.Now() // time.Time | Only returns the releases released at or after this date. (optional)
	releasedTo := time.Now() // time.Time | Only returns the releases released at or before this date. (optional)
	activeMachineCount := int32(1) // int32 | Only returns the releases running on exactly this number of active machines. (optional)
	activeMachineCountMin := int32(1) // int32 | Only returns the releases running on at least this number of active machines. (optional)
	activeMachineCountMax := int32(1) // int32 | Only returns the releases running on at most this number of active machines. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ReleasesAPI.ListReleases(context.Background(), productId).Page(page).PageSize(pageSize).Sort(sort).Search(search).ReleasedFrom(releasedFrom).ReleasedTo(releasedTo).ActiveMachineCount(activeMachineCount).ActiveMachineCountMin(activeMachineCountMin).ActiveMachineCountMax(activeMachineCountMax).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReleasesAPI.ListReleases``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListReleases`: ReleaseList
	fmt.Fprintf(os.Stdout, "Response from `ReleasesAPI.ListReleases`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**productId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListReleasesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | Page to return. Pages are numbered from 1: &#x60;1&#x60; is the first page. A page past the last one returns an empty &#x60;data&#x60;, not an error. Defaults to &#x60;1&#x60;. | [default to 1]
 **pageSize** | **int32** | Maximum number of items per page, from 1 to 100. Every page holds this many items except the last one, which can hold fewer. Defaults to &#x60;20&#x60;. | [default to 20]
 **sort** | **string** | Field to sort by, prefixed with &#x60;-&#x60; for descending order. Defaults to &#x60;-version&#x60;. | [default to &quot;-version&quot;]
 **search** | **string** | Case-insensitive text the version contains. | 
 **releasedFrom** | **time.Time** | Only returns the releases released at or after this date. | 
 **releasedTo** | **time.Time** | Only returns the releases released at or before this date. | 
 **activeMachineCount** | **int32** | Only returns the releases running on exactly this number of active machines. | 
 **activeMachineCountMin** | **int32** | Only returns the releases running on at least this number of active machines. | 
 **activeMachineCountMax** | **int32** | Only returns the releases running on at most this number of active machines. | 

### Return type

[**ReleaseList**](ReleaseList.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateRelease

> Release UpdateRelease(ctx, id).UpdateRelease(updateRelease).Execute()

Update a release



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
	id := "r4Lm8VwX" // string | 
	updateRelease := *openapiclient.NewUpdateRelease() // UpdateRelease | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.ReleasesAPI.UpdateRelease(context.Background(), id).UpdateRelease(updateRelease).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `ReleasesAPI.UpdateRelease``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateRelease`: Release
	fmt.Fprintf(os.Stdout, "Response from `ReleasesAPI.UpdateRelease`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateReleaseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateRelease** | [**UpdateRelease**](UpdateRelease.md) |  | 

### Return type

[**Release**](Release.md)

### Authorization

[apiKey](../README.md#apiKey)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

