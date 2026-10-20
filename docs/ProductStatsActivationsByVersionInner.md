# ProductStatsActivationsByVersionInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Version** | **NullableString** | &#x60;null&#x60; for the activations that didn&#39;t send a version. | 
**Counts** | **[]int32** | Number of successful activations each day, aligned on &#x60;days&#x60;. | 

## Methods

### NewProductStatsActivationsByVersionInner

`func NewProductStatsActivationsByVersionInner(version NullableString, counts []int32, ) *ProductStatsActivationsByVersionInner`

NewProductStatsActivationsByVersionInner instantiates a new ProductStatsActivationsByVersionInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductStatsActivationsByVersionInnerWithDefaults

`func NewProductStatsActivationsByVersionInnerWithDefaults() *ProductStatsActivationsByVersionInner`

NewProductStatsActivationsByVersionInnerWithDefaults instantiates a new ProductStatsActivationsByVersionInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersion

`func (o *ProductStatsActivationsByVersionInner) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *ProductStatsActivationsByVersionInner) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *ProductStatsActivationsByVersionInner) SetVersion(v string)`

SetVersion sets Version field to given value.


### SetVersionNil

`func (o *ProductStatsActivationsByVersionInner) SetVersionNil(b bool)`

 SetVersionNil sets the value for Version to be an explicit nil

### UnsetVersion
`func (o *ProductStatsActivationsByVersionInner) UnsetVersion()`

UnsetVersion ensures that no value is present for Version, not even an explicit nil
### GetCounts

`func (o *ProductStatsActivationsByVersionInner) GetCounts() []int32`

GetCounts returns the Counts field if non-nil, zero value otherwise.

### GetCountsOk

`func (o *ProductStatsActivationsByVersionInner) GetCountsOk() (*[]int32, bool)`

GetCountsOk returns a tuple with the Counts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCounts

`func (o *ProductStatsActivationsByVersionInner) SetCounts(v []int32)`

SetCounts sets Counts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


