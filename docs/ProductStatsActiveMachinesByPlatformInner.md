# ProductStatsActiveMachinesByPlatformInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Platform** | **NullableString** | &#x60;null&#x60; for the machines that didn&#39;t send a platform. | 
**Count** | **int32** |  | 

## Methods

### NewProductStatsActiveMachinesByPlatformInner

`func NewProductStatsActiveMachinesByPlatformInner(platform NullableString, count int32, ) *ProductStatsActiveMachinesByPlatformInner`

NewProductStatsActiveMachinesByPlatformInner instantiates a new ProductStatsActiveMachinesByPlatformInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductStatsActiveMachinesByPlatformInnerWithDefaults

`func NewProductStatsActiveMachinesByPlatformInnerWithDefaults() *ProductStatsActiveMachinesByPlatformInner`

NewProductStatsActiveMachinesByPlatformInnerWithDefaults instantiates a new ProductStatsActiveMachinesByPlatformInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPlatform

`func (o *ProductStatsActiveMachinesByPlatformInner) GetPlatform() string`

GetPlatform returns the Platform field if non-nil, zero value otherwise.

### GetPlatformOk

`func (o *ProductStatsActiveMachinesByPlatformInner) GetPlatformOk() (*string, bool)`

GetPlatformOk returns a tuple with the Platform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlatform

`func (o *ProductStatsActiveMachinesByPlatformInner) SetPlatform(v string)`

SetPlatform sets Platform field to given value.


### SetPlatformNil

`func (o *ProductStatsActiveMachinesByPlatformInner) SetPlatformNil(b bool)`

 SetPlatformNil sets the value for Platform to be an explicit nil

### UnsetPlatform
`func (o *ProductStatsActiveMachinesByPlatformInner) UnsetPlatform()`

UnsetPlatform ensures that no value is present for Platform, not even an explicit nil
### GetCount

`func (o *ProductStatsActiveMachinesByPlatformInner) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *ProductStatsActiveMachinesByPlatformInner) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *ProductStatsActiveMachinesByPlatformInner) SetCount(v int32)`

SetCount sets Count field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


