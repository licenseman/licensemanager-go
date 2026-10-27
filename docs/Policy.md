# Policy

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ProductId** | **string** |  | 
**Slug** | **string** |  | 
**Name** | **string** |  | 
**IsDefault** | **bool** | Whether this is the product&#39;s default policy. Each product has exactly one. | 
**Duration** | [**NullablePolicyDuration**](PolicyDuration.md) |  | 
**MaxMachines** | **NullableInt32** | Maximum number of active machines of the licenses created with this policy. &#x60;null&#x60; when there&#39;s no limit. | 
**MaxOfflineDurationSeconds** | **int32** | Longest the applications can run offline with the licenses created with this policy, in seconds. | 
**MaxVersion** | [**NullablePolicyMaxVersion**](PolicyMaxVersion.md) |  | 
**MoneyBackGuaranteeDays** | **NullableInt32** | Number of days after their creation during which customers can cancel the licenses created with this policy, from the customer portal or with &#x60;cancelLicense&#x60;. &#x60;null&#x60; when they can&#39;t. | 
**LicenseCount** | **int32** | Number of licenses following this policy. | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewPolicy

`func NewPolicy(id string, productId string, slug string, name string, isDefault bool, duration NullablePolicyDuration, maxMachines NullableInt32, maxOfflineDurationSeconds int32, maxVersion NullablePolicyMaxVersion, moneyBackGuaranteeDays NullableInt32, licenseCount int32, createdAt time.Time, updatedAt time.Time, ) *Policy`

NewPolicy instantiates a new Policy object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPolicyWithDefaults

`func NewPolicyWithDefaults() *Policy`

NewPolicyWithDefaults instantiates a new Policy object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Policy) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Policy) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Policy) SetId(v string)`

SetId sets Id field to given value.


### GetProductId

`func (o *Policy) GetProductId() string`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *Policy) GetProductIdOk() (*string, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *Policy) SetProductId(v string)`

SetProductId sets ProductId field to given value.


### GetSlug

`func (o *Policy) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *Policy) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *Policy) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetName

`func (o *Policy) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Policy) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Policy) SetName(v string)`

SetName sets Name field to given value.


### GetIsDefault

`func (o *Policy) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *Policy) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *Policy) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.


### GetDuration

`func (o *Policy) GetDuration() PolicyDuration`

GetDuration returns the Duration field if non-nil, zero value otherwise.

### GetDurationOk

`func (o *Policy) GetDurationOk() (*PolicyDuration, bool)`

GetDurationOk returns a tuple with the Duration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDuration

`func (o *Policy) SetDuration(v PolicyDuration)`

SetDuration sets Duration field to given value.


### SetDurationNil

`func (o *Policy) SetDurationNil(b bool)`

 SetDurationNil sets the value for Duration to be an explicit nil

### UnsetDuration
`func (o *Policy) UnsetDuration()`

UnsetDuration ensures that no value is present for Duration, not even an explicit nil
### GetMaxMachines

`func (o *Policy) GetMaxMachines() int32`

GetMaxMachines returns the MaxMachines field if non-nil, zero value otherwise.

### GetMaxMachinesOk

`func (o *Policy) GetMaxMachinesOk() (*int32, bool)`

GetMaxMachinesOk returns a tuple with the MaxMachines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxMachines

`func (o *Policy) SetMaxMachines(v int32)`

SetMaxMachines sets MaxMachines field to given value.


### SetMaxMachinesNil

`func (o *Policy) SetMaxMachinesNil(b bool)`

 SetMaxMachinesNil sets the value for MaxMachines to be an explicit nil

### UnsetMaxMachines
`func (o *Policy) UnsetMaxMachines()`

UnsetMaxMachines ensures that no value is present for MaxMachines, not even an explicit nil
### GetMaxOfflineDurationSeconds

`func (o *Policy) GetMaxOfflineDurationSeconds() int32`

GetMaxOfflineDurationSeconds returns the MaxOfflineDurationSeconds field if non-nil, zero value otherwise.

### GetMaxOfflineDurationSecondsOk

`func (o *Policy) GetMaxOfflineDurationSecondsOk() (*int32, bool)`

GetMaxOfflineDurationSecondsOk returns a tuple with the MaxOfflineDurationSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOfflineDurationSeconds

`func (o *Policy) SetMaxOfflineDurationSeconds(v int32)`

SetMaxOfflineDurationSeconds sets MaxOfflineDurationSeconds field to given value.


### GetMaxVersion

`func (o *Policy) GetMaxVersion() PolicyMaxVersion`

GetMaxVersion returns the MaxVersion field if non-nil, zero value otherwise.

### GetMaxVersionOk

`func (o *Policy) GetMaxVersionOk() (*PolicyMaxVersion, bool)`

GetMaxVersionOk returns a tuple with the MaxVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxVersion

`func (o *Policy) SetMaxVersion(v PolicyMaxVersion)`

SetMaxVersion sets MaxVersion field to given value.


### SetMaxVersionNil

`func (o *Policy) SetMaxVersionNil(b bool)`

 SetMaxVersionNil sets the value for MaxVersion to be an explicit nil

### UnsetMaxVersion
`func (o *Policy) UnsetMaxVersion()`

UnsetMaxVersion ensures that no value is present for MaxVersion, not even an explicit nil
### GetMoneyBackGuaranteeDays

`func (o *Policy) GetMoneyBackGuaranteeDays() int32`

GetMoneyBackGuaranteeDays returns the MoneyBackGuaranteeDays field if non-nil, zero value otherwise.

### GetMoneyBackGuaranteeDaysOk

`func (o *Policy) GetMoneyBackGuaranteeDaysOk() (*int32, bool)`

GetMoneyBackGuaranteeDaysOk returns a tuple with the MoneyBackGuaranteeDays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMoneyBackGuaranteeDays

`func (o *Policy) SetMoneyBackGuaranteeDays(v int32)`

SetMoneyBackGuaranteeDays sets MoneyBackGuaranteeDays field to given value.


### SetMoneyBackGuaranteeDaysNil

`func (o *Policy) SetMoneyBackGuaranteeDaysNil(b bool)`

 SetMoneyBackGuaranteeDaysNil sets the value for MoneyBackGuaranteeDays to be an explicit nil

### UnsetMoneyBackGuaranteeDays
`func (o *Policy) UnsetMoneyBackGuaranteeDays()`

UnsetMoneyBackGuaranteeDays ensures that no value is present for MoneyBackGuaranteeDays, not even an explicit nil
### GetLicenseCount

`func (o *Policy) GetLicenseCount() int32`

GetLicenseCount returns the LicenseCount field if non-nil, zero value otherwise.

### GetLicenseCountOk

`func (o *Policy) GetLicenseCountOk() (*int32, bool)`

GetLicenseCountOk returns a tuple with the LicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseCount

`func (o *Policy) SetLicenseCount(v int32)`

SetLicenseCount sets LicenseCount field to given value.


### GetCreatedAt

`func (o *Policy) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Policy) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Policy) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Policy) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Policy) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Policy) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


