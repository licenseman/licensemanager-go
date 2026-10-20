# CreateLicense

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** | Email of the customer the license belongs to. The product&#39;s customer with this email, compared regardless of case, or a new one when there&#39;s none. | 
**Key** | Pointer to **string** | Unique within the product. Case sensitive: &#x60;validateKey&#x60; compares keys exactly. Defaults to a random key of 5 groups of 5 characters separated by dashes, each character an upper case letter or a digit other than &#x60;O&#x60;, &#x60;0&#x60;, &#x60;I&#x60; and &#x60;1&#x60;, for 125 random bits. Starts with &#x60;TEST-&#x60; in test products, which is added when missing, and removed in live products. | [optional] 
**PolicyId** | Pointer to **string** | Policy of the product the license follows. Defaults to the product&#39;s default policy. | [optional] 
**ExpiresAt** | Pointer to **NullableTime** | &#x60;null&#x60; makes the license never expire. Defaults to the creation date plus the duration of the policy, or &#x60;null&#x60; when the policy has none. | [optional] 
**Meta** | Pointer to **map[string]interface{}** | Free-form JSON object. | [optional] 
**MaxMachines** | Pointer to **NullableInt32** | Maximum number of active machines the license can be used on. &#x60;null&#x60; for no limit. Defaults to the one of the policy. | [optional] 
**MaxOfflineDurationSeconds** | Pointer to **int32** | Longest the applications can run offline with the license, in seconds. At least one hour (&#x60;3600&#x60;). Defaults to the one of the policy. | [optional] 
**Price** | Pointer to [**NullablePriceInput**](PriceInput.md) |  | [optional] 
**MaxVersion** | Pointer to [**LicenseMaxVersionInput**](LicenseMaxVersionInput.md) |  | [optional] 
**SendKey** | Pointer to **bool** | &#x60;true&#x60; emails the key to the customer once the license is created, like &#x60;sendLicenseKeys&#x60;. Sent in the background: a failed email doesn&#39;t fail the creation. In test products, it&#39;s only sent when the customer&#39;s email is a member&#39;s of the organization. Defaults to &#x60;false&#x60;. | [optional] 

## Methods

### NewCreateLicense

`func NewCreateLicense(email string, ) *CreateLicense`

NewCreateLicense instantiates a new CreateLicense object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateLicenseWithDefaults

`func NewCreateLicenseWithDefaults() *CreateLicense`

NewCreateLicenseWithDefaults instantiates a new CreateLicense object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *CreateLicense) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *CreateLicense) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *CreateLicense) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetKey

`func (o *CreateLicense) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *CreateLicense) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *CreateLicense) SetKey(v string)`

SetKey sets Key field to given value.

### HasKey

`func (o *CreateLicense) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetPolicyId

`func (o *CreateLicense) GetPolicyId() string`

GetPolicyId returns the PolicyId field if non-nil, zero value otherwise.

### GetPolicyIdOk

`func (o *CreateLicense) GetPolicyIdOk() (*string, bool)`

GetPolicyIdOk returns a tuple with the PolicyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyId

`func (o *CreateLicense) SetPolicyId(v string)`

SetPolicyId sets PolicyId field to given value.

### HasPolicyId

`func (o *CreateLicense) HasPolicyId() bool`

HasPolicyId returns a boolean if a field has been set.

### GetExpiresAt

`func (o *CreateLicense) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *CreateLicense) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *CreateLicense) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *CreateLicense) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *CreateLicense) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *CreateLicense) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil
### GetMeta

`func (o *CreateLicense) GetMeta() map[string]*interface{}`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *CreateLicense) GetMetaOk() (*map[string]*interface{}, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *CreateLicense) SetMeta(v map[string]*interface{})`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *CreateLicense) HasMeta() bool`

HasMeta returns a boolean if a field has been set.

### SetMetaNil

`func (o *CreateLicense) SetMetaNil(b bool)`

 SetMetaNil sets the value for Meta to be an explicit nil

### UnsetMeta
`func (o *CreateLicense) UnsetMeta()`

UnsetMeta ensures that no value is present for Meta, not even an explicit nil
### GetMaxMachines

`func (o *CreateLicense) GetMaxMachines() int32`

GetMaxMachines returns the MaxMachines field if non-nil, zero value otherwise.

### GetMaxMachinesOk

`func (o *CreateLicense) GetMaxMachinesOk() (*int32, bool)`

GetMaxMachinesOk returns a tuple with the MaxMachines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxMachines

`func (o *CreateLicense) SetMaxMachines(v int32)`

SetMaxMachines sets MaxMachines field to given value.

### HasMaxMachines

`func (o *CreateLicense) HasMaxMachines() bool`

HasMaxMachines returns a boolean if a field has been set.

### SetMaxMachinesNil

`func (o *CreateLicense) SetMaxMachinesNil(b bool)`

 SetMaxMachinesNil sets the value for MaxMachines to be an explicit nil

### UnsetMaxMachines
`func (o *CreateLicense) UnsetMaxMachines()`

UnsetMaxMachines ensures that no value is present for MaxMachines, not even an explicit nil
### GetMaxOfflineDurationSeconds

`func (o *CreateLicense) GetMaxOfflineDurationSeconds() int32`

GetMaxOfflineDurationSeconds returns the MaxOfflineDurationSeconds field if non-nil, zero value otherwise.

### GetMaxOfflineDurationSecondsOk

`func (o *CreateLicense) GetMaxOfflineDurationSecondsOk() (*int32, bool)`

GetMaxOfflineDurationSecondsOk returns a tuple with the MaxOfflineDurationSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOfflineDurationSeconds

`func (o *CreateLicense) SetMaxOfflineDurationSeconds(v int32)`

SetMaxOfflineDurationSeconds sets MaxOfflineDurationSeconds field to given value.

### HasMaxOfflineDurationSeconds

`func (o *CreateLicense) HasMaxOfflineDurationSeconds() bool`

HasMaxOfflineDurationSeconds returns a boolean if a field has been set.

### GetPrice

`func (o *CreateLicense) GetPrice() PriceInput`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *CreateLicense) GetPriceOk() (*PriceInput, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *CreateLicense) SetPrice(v PriceInput)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *CreateLicense) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### SetPriceNil

`func (o *CreateLicense) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *CreateLicense) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetMaxVersion

`func (o *CreateLicense) GetMaxVersion() LicenseMaxVersionInput`

GetMaxVersion returns the MaxVersion field if non-nil, zero value otherwise.

### GetMaxVersionOk

`func (o *CreateLicense) GetMaxVersionOk() (*LicenseMaxVersionInput, bool)`

GetMaxVersionOk returns a tuple with the MaxVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxVersion

`func (o *CreateLicense) SetMaxVersion(v LicenseMaxVersionInput)`

SetMaxVersion sets MaxVersion field to given value.

### HasMaxVersion

`func (o *CreateLicense) HasMaxVersion() bool`

HasMaxVersion returns a boolean if a field has been set.

### GetSendKey

`func (o *CreateLicense) GetSendKey() bool`

GetSendKey returns the SendKey field if non-nil, zero value otherwise.

### GetSendKeyOk

`func (o *CreateLicense) GetSendKeyOk() (*bool, bool)`

GetSendKeyOk returns a tuple with the SendKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSendKey

`func (o *CreateLicense) SetSendKey(v bool)`

SetSendKey sets SendKey field to given value.

### HasSendKey

`func (o *CreateLicense) HasSendKey() bool`

HasSendKey returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


