# MachineList

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]Machine**](Machine.md) | Items of the page, in the requested order. Empty past the last page. | 
**Pagination** | [**Pagination**](Pagination.md) |  | 

## Methods

### NewMachineList

`func NewMachineList(data []Machine, pagination Pagination, ) *MachineList`

NewMachineList instantiates a new MachineList object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMachineListWithDefaults

`func NewMachineListWithDefaults() *MachineList`

NewMachineListWithDefaults instantiates a new MachineList object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *MachineList) GetData() []Machine`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *MachineList) GetDataOk() (*[]Machine, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *MachineList) SetData(v []Machine)`

SetData sets Data field to given value.


### GetPagination

`func (o *MachineList) GetPagination() Pagination`

GetPagination returns the Pagination field if non-nil, zero value otherwise.

### GetPaginationOk

`func (o *MachineList) GetPaginationOk() (*Pagination, bool)`

GetPaginationOk returns a tuple with the Pagination field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPagination

`func (o *MachineList) SetPagination(v Pagination)`

SetPagination sets Pagination field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


