# ReleaseList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]Release**](Release.md) | Items of the page, in the requested order. Empty past the last page. | 
**Pagination** | [**Pagination**](Pagination.md) |  | 

## Methods

### NewReleaseList

`func NewReleaseList(data []Release, pagination Pagination, ) *ReleaseList`

NewReleaseList instantiates a new ReleaseList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReleaseListWithDefaults

`func NewReleaseListWithDefaults() *ReleaseList`

NewReleaseListWithDefaults instantiates a new ReleaseList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ReleaseList) GetData() []Release`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ReleaseList) GetDataOk() (*[]Release, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ReleaseList) SetData(v []Release)`

SetData sets Data field to given value.


### GetPagination

`func (o *ReleaseList) GetPagination() Pagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *ReleaseList) GetPaginationOk() (*Pagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *ReleaseList) SetPagination(v Pagination)`

SetPagination sets Pagination field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


