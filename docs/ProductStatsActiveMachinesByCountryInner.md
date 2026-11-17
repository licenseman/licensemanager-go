# ProductStatsActiveMachinesByCountryInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Country** | **NullableString** | ISO 3166-1 alpha-2 code of the country the machine was last successfully validated from. &#x60;null&#x60; for the machines it couldn&#39;t be located for. | 
**Count** | **int32** |  | 

## Methods

### NewProductStatsActiveMachinesByCountryInner

`func NewProductStatsActiveMachinesByCountryInner(country NullableString, count int32, ) *ProductStatsActiveMachinesByCountryInner`

NewProductStatsActiveMachinesByCountryInner instantiates a new ProductStatsActiveMachinesByCountryInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductStatsActiveMachinesByCountryInnerWithDefaults

`func NewProductStatsActiveMachinesByCountryInnerWithDefaults() *ProductStatsActiveMachinesByCountryInner`

NewProductStatsActiveMachinesByCountryInnerWithDefaults instantiates a new ProductStatsActiveMachinesByCountryInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCountry

`func (o *ProductStatsActiveMachinesByCountryInner) GetCountry() string`

GetCountry returns the Country field if non-nil, zero value otherwise.

### GetCountryOk

`func (o *ProductStatsActiveMachinesByCountryInner) GetCountryOk() (*string, bool)`

GetCountryOk returns a tuple with the Country field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCountry

`func (o *ProductStatsActiveMachinesByCountryInner) SetCountry(v string)`

SetCountry sets Country field to given value.


### SetCountryNil

`func (o *ProductStatsActiveMachinesByCountryInner) SetCountryNil(b bool)`

 SetCountryNil sets the value for Country to be an explicit nil

### UnsetCountry
`func (o *ProductStatsActiveMachinesByCountryInner) UnsetCountry()`

UnsetCountry ensures that no value is present for Country, not even an explicit nil
### GetCount

`func (o *ProductStatsActiveMachinesByCountryInner) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *ProductStatsActiveMachinesByCountryInner) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *ProductStatsActiveMachinesByCountryInner) SetCount(v int32)`

SetCount sets Count field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


