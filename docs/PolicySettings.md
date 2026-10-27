# PolicySettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Duration** | Pointer to [**NullablePolicySettingsDuration**](PolicySettingsDuration.md) |  | [optional] 
**MaxMachines** | Pointer to **NullableInt32** | Maximum number of active machines of the licenses created with this policy, copied to each of them. &#x60;null&#x60; for no limit. Defaults to &#x60;null&#x60;. | [optional] 
**MaxOfflineDurationSeconds** | Pointer to **int32** | Longest the applications can run offline with the licenses created with this policy, in seconds, copied to each of them. At least one hour (&#x60;3600&#x60;). Defaults to one week. | [optional] 
**MaxVersion** | Pointer to [**NullablePolicySettingsMaxVersion**](PolicySettingsMaxVersion.md) |  | [optional] 
**MoneyBackGuaranteeDays** | Pointer to **NullableInt32** | Number of days after their creation during which customers can cancel the licenses created with this policy, from the customer portal or with &#x60;cancelLicense&#x60;, which refunds their Stripe payment. Each license keeps the end of its own period as &#x60;cancellableUntil&#x60;. &#x60;null&#x60; for no money back guarantee. Defaults to &#x60;null&#x60;. | [optional] 

## Methods

### NewPolicySettings

`func NewPolicySettings() *PolicySettings`

NewPolicySettings instantiates a new PolicySettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPolicySettingsWithDefaults

`func NewPolicySettingsWithDefaults() *PolicySettings`

NewPolicySettingsWithDefaults instantiates a new PolicySettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDuration

`func (o *PolicySettings) GetDuration() PolicySettingsDuration`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *PolicySettings) GetDurationOk() (*PolicySettingsDuration, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *PolicySettings) SetDuration(v PolicySettingsDuration)`

SetDuration sets Duration field to given value.

### HasDuration

`func (o *PolicySettings) HasDuration() bool`

HasDuration returns a boolean if a field has been set.

### SetDurationNil

`func (o *PolicySettings) SetDurationNil(b bool)`

 SetDurationNil sets the value for Duration to be an explicit nil

### UnsetDuration
`func (o *PolicySettings) UnsetDuration()`

UnsetDuration ensures that no value is present for Duration, not even an explicit nil
### GetMaxMachines

`func (o *PolicySettings) GetMaxMachines() int32`

GetMaxMachines returns the MaxMachines field if non-nil, zero value otherwise.

### GetMaxMachinesOk

`func (o *PolicySettings) GetMaxMachinesOk() (*int32, bool)`

GetMaxMachinesOk returns a tuple with the MaxMachines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxMachines

`func (o *PolicySettings) SetMaxMachines(v int32)`

SetMaxMachines sets MaxMachines field to given value.

### HasMaxMachines

`func (o *PolicySettings) HasMaxMachines() bool`

HasMaxMachines returns a boolean if a field has been set.

### SetMaxMachinesNil

`func (o *PolicySettings) SetMaxMachinesNil(b bool)`

 SetMaxMachinesNil sets the value for MaxMachines to be an explicit nil

### UnsetMaxMachines
`func (o *PolicySettings) UnsetMaxMachines()`

UnsetMaxMachines ensures that no value is present for MaxMachines, not even an explicit nil
### GetMaxOfflineDurationSeconds

`func (o *PolicySettings) GetMaxOfflineDurationSeconds() int32`

GetMaxOfflineDurationSeconds returns the MaxOfflineDurationSeconds field if non-nil, zero value otherwise.

### GetMaxOfflineDurationSecondsOk

`func (o *PolicySettings) GetMaxOfflineDurationSecondsOk() (*int32, bool)`

GetMaxOfflineDurationSecondsOk returns a tuple with the MaxOfflineDurationSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOfflineDurationSeconds

`func (o *PolicySettings) SetMaxOfflineDurationSeconds(v int32)`

SetMaxOfflineDurationSeconds sets MaxOfflineDurationSeconds field to given value.

### HasMaxOfflineDurationSeconds

`func (o *PolicySettings) HasMaxOfflineDurationSeconds() bool`

HasMaxOfflineDurationSeconds returns a boolean if a field has been set.

### GetMaxVersion

`func (o *PolicySettings) GetMaxVersion() PolicySettingsMaxVersion`

GetMaxVersion returns the MaxVersion field if non-nil, zero value otherwise.

### GetMaxVersionOk

`func (o *PolicySettings) GetMaxVersionOk() (*PolicySettingsMaxVersion, bool)`

GetMaxVersionOk returns a tuple with the MaxVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxVersion

`func (o *PolicySettings) SetMaxVersion(v PolicySettingsMaxVersion)`

SetMaxVersion sets MaxVersion field to given value.

### HasMaxVersion

`func (o *PolicySettings) HasMaxVersion() bool`

HasMaxVersion returns a boolean if a field has been set.

### SetMaxVersionNil

`func (o *PolicySettings) SetMaxVersionNil(b bool)`

 SetMaxVersionNil sets the value for MaxVersion to be an explicit nil

### UnsetMaxVersion
`func (o *PolicySettings) UnsetMaxVersion()`

UnsetMaxVersion ensures that no value is present for MaxVersion, not even an explicit nil
### GetMoneyBackGuaranteeDays

`func (o *PolicySettings) GetMoneyBackGuaranteeDays() int32`

GetMoneyBackGuaranteeDays returns the MoneyBackGuaranteeDays field if non-nil, zero value otherwise.

### GetMoneyBackGuaranteeDaysOk

`func (o *PolicySettings) GetMoneyBackGuaranteeDaysOk() (*int32, bool)`

GetMoneyBackGuaranteeDaysOk returns a tuple with the MoneyBackGuaranteeDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMoneyBackGuaranteeDays

`func (o *PolicySettings) SetMoneyBackGuaranteeDays(v int32)`

SetMoneyBackGuaranteeDays sets MoneyBackGuaranteeDays field to given value.

### HasMoneyBackGuaranteeDays

`func (o *PolicySettings) HasMoneyBackGuaranteeDays() bool`

HasMoneyBackGuaranteeDays returns a boolean if a field has been set.

### SetMoneyBackGuaranteeDaysNil

`func (o *PolicySettings) SetMoneyBackGuaranteeDaysNil(b bool)`

 SetMoneyBackGuaranteeDaysNil sets the value for MoneyBackGuaranteeDays to be an explicit nil

### UnsetMoneyBackGuaranteeDays
`func (o *PolicySettings) UnsetMoneyBackGuaranteeDays()`

UnsetMoneyBackGuaranteeDays ensures that no value is present for MoneyBackGuaranteeDays, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


