# ImportLicense

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** | Email of the customer the license belongs to. The product&#39;s customer with this email, compared regardless of case, or a new one when there&#39;s none. | 
**Key** | **string** | The license&#39;s current key, kept as is. Case sensitive. Starts with &#x60;TEST-&#x60; in test products, which is added when missing, and removed in live products. | 
**PolicyId** | Pointer to **string** | Policy of the product the license follows. Defaults to the product&#39;s default policy. | [optional] 
**ExpiresAt** | Pointer to **NullableTime** | &#x60;null&#x60; makes the license never expire. Defaults to the creation date plus the duration of the policy, or &#x60;null&#x60; when the policy has none. | [optional] 
**Meta** | Pointer to **map[string]interface{}** | Free-form JSON object. | [optional] 
**MaxMachines** | Pointer to **NullableInt32** | Maximum number of active machines the license can be used on. &#x60;null&#x60; for no limit. Defaults to the one of the policy. | [optional] 
**MaxOfflineDurationSeconds** | Pointer to **int32** | Longest the applications can run offline with the license, in seconds. At least one hour (&#x60;3600&#x60;). Defaults to the one of the policy. | [optional] 
**Price** | Pointer to [**NullablePriceInput**](PriceInput.md) |  | [optional] 
**MaxVersion** | Pointer to [**LicenseMaxVersionInput**](LicenseMaxVersionInput.md) |  | [optional] 
**CancellableUntil** | Pointer to **NullableTime** | End of the money back guarantee: until then, the customer can cancel the license from the customer portal, or with a token. &#x60;null&#x60; to not let them. Defaults to the creation date plus the policy&#39;s &#x60;moneyBackGuaranteeDays&#x60;, or &#x60;null&#x60; when it has none. | [optional] 
**Name** | Pointer to **string** | Name of the customer, given to it when it has none yet. | [optional] 
**Subscription** | Pointer to [**ImportLicenseSubscription**](ImportLicenseSubscription.md) |  | [optional] 

## Methods

### NewImportLicense

`func NewImportLicense(email string, key string, ) *ImportLicense`

NewImportLicense instantiates a new ImportLicense object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewImportLicenseWithDefaults

`func NewImportLicenseWithDefaults() *ImportLicense`

NewImportLicenseWithDefaults instantiates a new ImportLicense object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *ImportLicense) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *ImportLicense) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *ImportLicense) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetKey

`func (o *ImportLicense) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *ImportLicense) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *ImportLicense) SetKey(v string)`

SetKey sets Key field to given value.


### GetPolicyId

`func (o *ImportLicense) GetPolicyId() string`

GetPolicyId returns the PolicyId field if non-nil, zero value otherwise.

### GetPolicyIdOk

`func (o *ImportLicense) GetPolicyIdOk() (*string, bool)`

GetPolicyIdOk returns a tuple with the PolicyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyId

`func (o *ImportLicense) SetPolicyId(v string)`

SetPolicyId sets PolicyId field to given value.

### HasPolicyId

`func (o *ImportLicense) HasPolicyId() bool`

HasPolicyId returns a boolean if a field has been set.

### GetExpiresAt

`func (o *ImportLicense) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *ImportLicense) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *ImportLicense) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *ImportLicense) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *ImportLicense) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *ImportLicense) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil
### GetMeta

`func (o *ImportLicense) GetMeta() map[string]*interface{}`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *ImportLicense) GetMetaOk() (*map[string]*interface{}, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *ImportLicense) SetMeta(v map[string]*interface{})`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *ImportLicense) HasMeta() bool`

HasMeta returns a boolean if a field has been set.

### SetMetaNil

`func (o *ImportLicense) SetMetaNil(b bool)`

 SetMetaNil sets the value for Meta to be an explicit nil

### UnsetMeta
`func (o *ImportLicense) UnsetMeta()`

UnsetMeta ensures that no value is present for Meta, not even an explicit nil
### GetMaxMachines

`func (o *ImportLicense) GetMaxMachines() int32`

GetMaxMachines returns the MaxMachines field if non-nil, zero value otherwise.

### GetMaxMachinesOk

`func (o *ImportLicense) GetMaxMachinesOk() (*int32, bool)`

GetMaxMachinesOk returns a tuple with the MaxMachines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxMachines

`func (o *ImportLicense) SetMaxMachines(v int32)`

SetMaxMachines sets MaxMachines field to given value.

### HasMaxMachines

`func (o *ImportLicense) HasMaxMachines() bool`

HasMaxMachines returns a boolean if a field has been set.

### SetMaxMachinesNil

`func (o *ImportLicense) SetMaxMachinesNil(b bool)`

 SetMaxMachinesNil sets the value for MaxMachines to be an explicit nil

### UnsetMaxMachines
`func (o *ImportLicense) UnsetMaxMachines()`

UnsetMaxMachines ensures that no value is present for MaxMachines, not even an explicit nil
### GetMaxOfflineDurationSeconds

`func (o *ImportLicense) GetMaxOfflineDurationSeconds() int32`

GetMaxOfflineDurationSeconds returns the MaxOfflineDurationSeconds field if non-nil, zero value otherwise.

### GetMaxOfflineDurationSecondsOk

`func (o *ImportLicense) GetMaxOfflineDurationSecondsOk() (*int32, bool)`

GetMaxOfflineDurationSecondsOk returns a tuple with the MaxOfflineDurationSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOfflineDurationSeconds

`func (o *ImportLicense) SetMaxOfflineDurationSeconds(v int32)`

SetMaxOfflineDurationSeconds sets MaxOfflineDurationSeconds field to given value.

### HasMaxOfflineDurationSeconds

`func (o *ImportLicense) HasMaxOfflineDurationSeconds() bool`

HasMaxOfflineDurationSeconds returns a boolean if a field has been set.

### GetPrice

`func (o *ImportLicense) GetPrice() PriceInput`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *ImportLicense) GetPriceOk() (*PriceInput, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *ImportLicense) SetPrice(v PriceInput)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *ImportLicense) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### SetPriceNil

`func (o *ImportLicense) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *ImportLicense) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetMaxVersion

`func (o *ImportLicense) GetMaxVersion() LicenseMaxVersionInput`

GetMaxVersion returns the MaxVersion field if non-nil, zero value otherwise.

### GetMaxVersionOk

`func (o *ImportLicense) GetMaxVersionOk() (*LicenseMaxVersionInput, bool)`

GetMaxVersionOk returns a tuple with the MaxVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxVersion

`func (o *ImportLicense) SetMaxVersion(v LicenseMaxVersionInput)`

SetMaxVersion sets MaxVersion field to given value.

### HasMaxVersion

`func (o *ImportLicense) HasMaxVersion() bool`

HasMaxVersion returns a boolean if a field has been set.

### GetCancellableUntil

`func (o *ImportLicense) GetCancellableUntil() time.Time`

GetCancellableUntil returns the CancellableUntil field if non-nil, zero value otherwise.

### GetCancellableUntilOk

`func (o *ImportLicense) GetCancellableUntilOk() (*time.Time, bool)`

GetCancellableUntilOk returns a tuple with the CancellableUntil field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancellableUntil

`func (o *ImportLicense) SetCancellableUntil(v time.Time)`

SetCancellableUntil sets CancellableUntil field to given value.

### HasCancellableUntil

`func (o *ImportLicense) HasCancellableUntil() bool`

HasCancellableUntil returns a boolean if a field has been set.

### SetCancellableUntilNil

`func (o *ImportLicense) SetCancellableUntilNil(b bool)`

 SetCancellableUntilNil sets the value for CancellableUntil to be an explicit nil

### UnsetCancellableUntil
`func (o *ImportLicense) UnsetCancellableUntil()`

UnsetCancellableUntil ensures that no value is present for CancellableUntil, not even an explicit nil
### GetName

`func (o *ImportLicense) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ImportLicense) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ImportLicense) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ImportLicense) HasName() bool`

HasName returns a boolean if a field has been set.

### GetSubscription

`func (o *ImportLicense) GetSubscription() ImportLicenseSubscription`

GetSubscription returns the Subscription field if non-nil, zero value otherwise.

### GetSubscriptionOk

`func (o *ImportLicense) GetSubscriptionOk() (*ImportLicenseSubscription, bool)`

GetSubscriptionOk returns a tuple with the Subscription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscription

`func (o *ImportLicense) SetSubscription(v ImportLicenseSubscription)`

SetSubscription sets Subscription field to given value.

### HasSubscription

`func (o *ImportLicense) HasSubscription() bool`

HasSubscription returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


