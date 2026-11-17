# ImportLicenseSubscription

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Provider** | **string** | Provider of the subscription. | 
**ExternalId** | **string** | Id of the subscription in the provider: &#x60;sub_…&#x60; in Stripe and in Paddle. | 

## Methods

### NewImportLicenseSubscription

`func NewImportLicenseSubscription(provider string, externalId string, ) *ImportLicenseSubscription`

NewImportLicenseSubscription instantiates a new ImportLicenseSubscription object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewImportLicenseSubscriptionWithDefaults

`func NewImportLicenseSubscriptionWithDefaults() *ImportLicenseSubscription`

NewImportLicenseSubscriptionWithDefaults instantiates a new ImportLicenseSubscription object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProvider

`func (o *ImportLicenseSubscription) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *ImportLicenseSubscription) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *ImportLicenseSubscription) SetProvider(v string)`

SetProvider sets Provider field to given value.


### GetExternalId

`func (o *ImportLicenseSubscription) GetExternalId() string`

GetExternalId returns the ExternalId field if non-nil, zero value otherwise.

### GetExternalIdOk

`func (o *ImportLicenseSubscription) GetExternalIdOk() (*string, bool)`

GetExternalIdOk returns a tuple with the ExternalId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExternalId

`func (o *ImportLicenseSubscription) SetExternalId(v string)`

SetExternalId sets ExternalId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


