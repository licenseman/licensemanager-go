# CreatePolicy

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Slug** | Pointer to **string** | Unique within the product. Defaults to the name, lower cased, without accents and special characters. Starts with &#x60;test_&#x60; in test products, which is added when missing, and removed in live products. | [optional] 
**IsDefault** | Pointer to **bool** | &#x60;true&#x60; makes this policy the product&#39;s default, in place of the current one. | [optional] 
**Duration** | Pointer to [**NullablePolicySettingsDuration**](PolicySettingsDuration.md) |  | [optional] 
**MaxMachines** | Pointer to **NullableInt32** | Maximum number of active machines of the licenses created with this policy, copied to each of them. &#x60;null&#x60; for no limit. Defaults to &#x60;null&#x60;. | [optional] 
**MaxOfflineDurationSeconds** | Pointer to **int32** | Longest the applications can run offline with the licenses created with this policy, in seconds, copied to each of them. At least one hour (&#x60;3600&#x60;). Defaults to one week. | [optional] 
**MaxVersion** | Pointer to [**NullablePolicySettingsMaxVersion**](PolicySettingsMaxVersion.md) |  | [optional] 

## Methods

### NewCreatePolicy

`func NewCreatePolicy(name string, ) *CreatePolicy`

NewCreatePolicy instantiates a new CreatePolicy object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePolicyWithDefaults

`func NewCreatePolicyWithDefaults() *CreatePolicy`

NewCreatePolicyWithDefaults instantiates a new CreatePolicy object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreatePolicy) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreatePolicy) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreatePolicy) SetName(v string)`

SetName sets Name field to given value.


### GetSlug

`func (o *CreatePolicy) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *CreatePolicy) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *CreatePolicy) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *CreatePolicy) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### GetIsDefault

`func (o *CreatePolicy) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *CreatePolicy) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *CreatePolicy) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.

### HasIsDefault

`func (o *CreatePolicy) HasIsDefault() bool`

HasIsDefault returns a boolean if a field has been set.

### GetDuration

`func (o *CreatePolicy) GetDuration() PolicySettingsDuration`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *CreatePolicy) GetDurationOk() (*PolicySettingsDuration, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *CreatePolicy) SetDuration(v PolicySettingsDuration)`

SetDuration sets Duration field to given value.

### HasDuration

`func (o *CreatePolicy) HasDuration() bool`

HasDuration returns a boolean if a field has been set.

### SetDurationNil

`func (o *CreatePolicy) SetDurationNil(b bool)`

 SetDurationNil sets the value for Duration to be an explicit nil

### UnsetDuration
`func (o *CreatePolicy) UnsetDuration()`

UnsetDuration ensures that no value is present for Duration, not even an explicit nil
### GetMaxMachines

`func (o *CreatePolicy) GetMaxMachines() int32`

GetMaxMachines returns the MaxMachines field if non-nil, zero value otherwise.

### GetMaxMachinesOk

`func (o *CreatePolicy) GetMaxMachinesOk() (*int32, bool)`

GetMaxMachinesOk returns a tuple with the MaxMachines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxMachines

`func (o *CreatePolicy) SetMaxMachines(v int32)`

SetMaxMachines sets MaxMachines field to given value.

### HasMaxMachines

`func (o *CreatePolicy) HasMaxMachines() bool`

HasMaxMachines returns a boolean if a field has been set.

### SetMaxMachinesNil

`func (o *CreatePolicy) SetMaxMachinesNil(b bool)`

 SetMaxMachinesNil sets the value for MaxMachines to be an explicit nil

### UnsetMaxMachines
`func (o *CreatePolicy) UnsetMaxMachines()`

UnsetMaxMachines ensures that no value is present for MaxMachines, not even an explicit nil
### GetMaxOfflineDurationSeconds

`func (o *CreatePolicy) GetMaxOfflineDurationSeconds() int32`

GetMaxOfflineDurationSeconds returns the MaxOfflineDurationSeconds field if non-nil, zero value otherwise.

### GetMaxOfflineDurationSecondsOk

`func (o *CreatePolicy) GetMaxOfflineDurationSecondsOk() (*int32, bool)`

GetMaxOfflineDurationSecondsOk returns a tuple with the MaxOfflineDurationSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOfflineDurationSeconds

`func (o *CreatePolicy) SetMaxOfflineDurationSeconds(v int32)`

SetMaxOfflineDurationSeconds sets MaxOfflineDurationSeconds field to given value.

### HasMaxOfflineDurationSeconds

`func (o *CreatePolicy) HasMaxOfflineDurationSeconds() bool`

HasMaxOfflineDurationSeconds returns a boolean if a field has been set.

### GetMaxVersion

`func (o *CreatePolicy) GetMaxVersion() PolicySettingsMaxVersion`

GetMaxVersion returns the MaxVersion field if non-nil, zero value otherwise.

### GetMaxVersionOk

`func (o *CreatePolicy) GetMaxVersionOk() (*PolicySettingsMaxVersion, bool)`

GetMaxVersionOk returns a tuple with the MaxVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxVersion

`func (o *CreatePolicy) SetMaxVersion(v PolicySettingsMaxVersion)`

SetMaxVersion sets MaxVersion field to given value.

### HasMaxVersion

`func (o *CreatePolicy) HasMaxVersion() bool`

HasMaxVersion returns a boolean if a field has been set.

### SetMaxVersionNil

`func (o *CreatePolicy) SetMaxVersionNil(b bool)`

 SetMaxVersionNil sets the value for MaxVersion to be an explicit nil

### UnsetMaxVersion
`func (o *CreatePolicy) UnsetMaxVersion()`

UnsetMaxVersion ensures that no value is present for MaxVersion, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


