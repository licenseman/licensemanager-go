# UpdateLicense

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ExpiresAt** | Pointer to **NullableTime** | &#x60;null&#x60; makes the license never expire. | [optional] 
**Meta** | Pointer to **map[string]interface{}** | Free-form JSON object. | [optional] 
**MaxMachines** | Pointer to **NullableInt32** | Maximum number of active machines the license can be used on. &#x60;null&#x60; for no limit. | [optional] 
**MaxOfflineDurationSeconds** | Pointer to **int32** | Longest the applications can run offline with the license, in seconds. At least one hour (&#x60;3600&#x60;). | [optional] 
**MaxVersion** | Pointer to [**LicenseMaxVersionInput**](LicenseMaxVersionInput.md) | Latest version of the product the license can use. The values left out are kept. | [optional] 
**Price** | Pointer to [**NullablePriceInput**](PriceInput.md) |  | [optional] 

## Methods

### NewUpdateLicense

`func NewUpdateLicense() *UpdateLicense`

NewUpdateLicense instantiates a new UpdateLicense object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateLicenseWithDefaults

`func NewUpdateLicenseWithDefaults() *UpdateLicense`

NewUpdateLicenseWithDefaults instantiates a new UpdateLicense object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetExpiresAt

`func (o *UpdateLicense) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *UpdateLicense) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *UpdateLicense) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *UpdateLicense) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *UpdateLicense) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *UpdateLicense) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil
### GetMeta

`func (o *UpdateLicense) GetMeta() map[string]*interface{}`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *UpdateLicense) GetMetaOk() (*map[string]*interface{}, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *UpdateLicense) SetMeta(v map[string]*interface{})`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *UpdateLicense) HasMeta() bool`

HasMeta returns a boolean if a field has been set.

### SetMetaNil

`func (o *UpdateLicense) SetMetaNil(b bool)`

 SetMetaNil sets the value for Meta to be an explicit nil

### UnsetMeta
`func (o *UpdateLicense) UnsetMeta()`

UnsetMeta ensures that no value is present for Meta, not even an explicit nil
### GetMaxMachines

`func (o *UpdateLicense) GetMaxMachines() int32`

GetMaxMachines returns the MaxMachines field if non-nil, zero value otherwise.

### GetMaxMachinesOk

`func (o *UpdateLicense) GetMaxMachinesOk() (*int32, bool)`

GetMaxMachinesOk returns a tuple with the MaxMachines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxMachines

`func (o *UpdateLicense) SetMaxMachines(v int32)`

SetMaxMachines sets MaxMachines field to given value.

### HasMaxMachines

`func (o *UpdateLicense) HasMaxMachines() bool`

HasMaxMachines returns a boolean if a field has been set.

### SetMaxMachinesNil

`func (o *UpdateLicense) SetMaxMachinesNil(b bool)`

 SetMaxMachinesNil sets the value for MaxMachines to be an explicit nil

### UnsetMaxMachines
`func (o *UpdateLicense) UnsetMaxMachines()`

UnsetMaxMachines ensures that no value is present for MaxMachines, not even an explicit nil
### GetMaxOfflineDurationSeconds

`func (o *UpdateLicense) GetMaxOfflineDurationSeconds() int32`

GetMaxOfflineDurationSeconds returns the MaxOfflineDurationSeconds field if non-nil, zero value otherwise.

### GetMaxOfflineDurationSecondsOk

`func (o *UpdateLicense) GetMaxOfflineDurationSecondsOk() (*int32, bool)`

GetMaxOfflineDurationSecondsOk returns a tuple with the MaxOfflineDurationSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOfflineDurationSeconds

`func (o *UpdateLicense) SetMaxOfflineDurationSeconds(v int32)`

SetMaxOfflineDurationSeconds sets MaxOfflineDurationSeconds field to given value.

### HasMaxOfflineDurationSeconds

`func (o *UpdateLicense) HasMaxOfflineDurationSeconds() bool`

HasMaxOfflineDurationSeconds returns a boolean if a field has been set.

### GetMaxVersion

`func (o *UpdateLicense) GetMaxVersion() LicenseMaxVersionInput`

GetMaxVersion returns the MaxVersion field if non-nil, zero value otherwise.

### GetMaxVersionOk

`func (o *UpdateLicense) GetMaxVersionOk() (*LicenseMaxVersionInput, bool)`

GetMaxVersionOk returns a tuple with the MaxVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxVersion

`func (o *UpdateLicense) SetMaxVersion(v LicenseMaxVersionInput)`

SetMaxVersion sets MaxVersion field to given value.

### HasMaxVersion

`func (o *UpdateLicense) HasMaxVersion() bool`

HasMaxVersion returns a boolean if a field has been set.

### GetPrice

`func (o *UpdateLicense) GetPrice() PriceInput`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *UpdateLicense) GetPriceOk() (*PriceInput, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *UpdateLicense) SetPrice(v PriceInput)`

SetPrice sets Price field to given value.

### HasPrice

`func (o *UpdateLicense) HasPrice() bool`

HasPrice returns a boolean if a field has been set.

### SetPriceNil

`func (o *UpdateLicense) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *UpdateLicense) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


