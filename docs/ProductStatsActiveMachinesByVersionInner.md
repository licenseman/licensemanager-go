# ProductStatsActiveMachinesByVersionInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Version** | **NullableString** | &#x60;null&#x60; for the machines that didn&#39;t send a version. | 
**Count** | **int32** |  | 

## Methods

### NewProductStatsActiveMachinesByVersionInner

`func NewProductStatsActiveMachinesByVersionInner(version NullableString, count int32, ) *ProductStatsActiveMachinesByVersionInner`

NewProductStatsActiveMachinesByVersionInner instantiates a new ProductStatsActiveMachinesByVersionInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductStatsActiveMachinesByVersionInnerWithDefaults

`func NewProductStatsActiveMachinesByVersionInnerWithDefaults() *ProductStatsActiveMachinesByVersionInner`

NewProductStatsActiveMachinesByVersionInnerWithDefaults instantiates a new ProductStatsActiveMachinesByVersionInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersion

`func (o *ProductStatsActiveMachinesByVersionInner) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *ProductStatsActiveMachinesByVersionInner) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *ProductStatsActiveMachinesByVersionInner) SetVersion(v string)`

SetVersion sets Version field to given value.


### SetVersionNil

`func (o *ProductStatsActiveMachinesByVersionInner) SetVersionNil(b bool)`

 SetVersionNil sets the value for Version to be an explicit nil

### UnsetVersion
`func (o *ProductStatsActiveMachinesByVersionInner) UnsetVersion()`

UnsetVersion ensures that no value is present for Version, not even an explicit nil
### GetCount

`func (o *ProductStatsActiveMachinesByVersionInner) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *ProductStatsActiveMachinesByVersionInner) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *ProductStatsActiveMachinesByVersionInner) SetCount(v int32)`

SetCount sets Count field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


