# PolicyDuration

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | **int32** |  | 
**Unit** | **string** | Calendar months: a license created on January 31 with a 1 month duration expires on the last day of February. | 

## Methods

### NewPolicyDuration

`func NewPolicyDuration(value int32, unit string, ) *PolicyDuration`

NewPolicyDuration instantiates a new PolicyDuration object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPolicyDurationWithDefaults

`func NewPolicyDurationWithDefaults() *PolicyDuration`

NewPolicyDurationWithDefaults instantiates a new PolicyDuration object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *PolicyDuration) GetValue() int32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *PolicyDuration) GetValueOk() (*int32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *PolicyDuration) SetValue(v int32)`

SetValue sets Value field to given value.


### GetUnit

`func (o *PolicyDuration) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *PolicyDuration) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *PolicyDuration) SetUnit(v string)`

SetUnit sets Unit field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


