# LicenseList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]License**](License.md) | Items of the page, in the requested order. Empty past the last page. | 
**Pagination** | [**Pagination**](Pagination.md) |  | 

## Methods

### NewLicenseList

`func NewLicenseList(data []License, pagination Pagination, ) *LicenseList`

NewLicenseList instantiates a new LicenseList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseListWithDefaults

`func NewLicenseListWithDefaults() *LicenseList`

NewLicenseListWithDefaults instantiates a new LicenseList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *LicenseList) GetData() []License`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *LicenseList) GetDataOk() (*[]License, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *LicenseList) SetData(v []License)`

SetData sets Data field to given value.


### GetPagination

`func (o *LicenseList) GetPagination() Pagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *LicenseList) GetPaginationOk() (*Pagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *LicenseList) SetPagination(v Pagination)`

SetPagination sets Pagination field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


