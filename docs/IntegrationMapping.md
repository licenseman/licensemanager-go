# IntegrationMapping

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**IntegrationId** | **string** |  | 
**Provider** | **string** |  | 
**ProductId** | **string** |  | 
**PolicyId** | **string** |  | 
**ExternalProductId** | **string** | Id of the product in the provider: &#x60;prod_…&#x60; in Stripe, &#x60;pro_…&#x60; in Paddle. | 
**ExternalPriceId** | **string** | Id of the price in the provider: &#x60;price_…&#x60; in Stripe, &#x60;pri_…&#x60; in Paddle. | 
**StripeProductId** | **string** | Deprecated: use &#x60;externalProductId&#x60;, which it equals. | 
**StripePriceId** | **string** | Deprecated: use &#x60;externalPriceId&#x60;, which it equals. | 
**ProductName** | **string** | Name of the provider&#39;s product when it was mapped. | 
**Price** | [**NullablePrice**](Price.md) |  | 
**Recurring** | [**NullableIntegrationMappingRecurring**](IntegrationMappingRecurring.md) |  | 
**Status** | **string** | &#x60;error&#x60; when the price can no longer be paid, explained by &#x60;statusReason&#x60;. | 
**StatusReason** | **NullableString** |  | 
**CreatedAt** | **time.Time** |  | 

## Methods

### NewIntegrationMapping

`func NewIntegrationMapping(id string, integrationId string, provider string, productId string, policyId string, externalProductId string, externalPriceId string, stripeProductId string, stripePriceId string, productName string, price NullablePrice, recurring NullableIntegrationMappingRecurring, status string, statusReason NullableString, createdAt time.Time, ) *IntegrationMapping`

NewIntegrationMapping instantiates a new IntegrationMapping object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIntegrationMappingWithDefaults

`func NewIntegrationMappingWithDefaults() *IntegrationMapping`

NewIntegrationMappingWithDefaults instantiates a new IntegrationMapping object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *IntegrationMapping) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *IntegrationMapping) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *IntegrationMapping) SetId(v string)`

SetId sets Id field to given value.


### GetIntegrationId

`func (o *IntegrationMapping) GetIntegrationId() string`

GetIntegrationId returns the IntegrationId field if non-nil, zero value otherwise.

### GetIntegrationIdOk

`func (o *IntegrationMapping) GetIntegrationIdOk() (*string, bool)`

GetIntegrationIdOk returns a tuple with the IntegrationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegrationId

`func (o *IntegrationMapping) SetIntegrationId(v string)`

SetIntegrationId sets IntegrationId field to given value.


### GetProvider

`func (o *IntegrationMapping) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *IntegrationMapping) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *IntegrationMapping) SetProvider(v string)`

SetProvider sets Provider field to given value.


### GetProductId

`func (o *IntegrationMapping) GetProductId() string`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *IntegrationMapping) GetProductIdOk() (*string, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *IntegrationMapping) SetProductId(v string)`

SetProductId sets ProductId field to given value.


### GetPolicyId

`func (o *IntegrationMapping) GetPolicyId() string`

GetPolicyId returns the PolicyId field if non-nil, zero value otherwise.

### GetPolicyIdOk

`func (o *IntegrationMapping) GetPolicyIdOk() (*string, bool)`

GetPolicyIdOk returns a tuple with the PolicyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyId

`func (o *IntegrationMapping) SetPolicyId(v string)`

SetPolicyId sets PolicyId field to given value.


### GetExternalProductId

`func (o *IntegrationMapping) GetExternalProductId() string`

GetExternalProductId returns the ExternalProductId field if non-nil, zero value otherwise.

### GetExternalProductIdOk

`func (o *IntegrationMapping) GetExternalProductIdOk() (*string, bool)`

GetExternalProductIdOk returns a tuple with the ExternalProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExternalProductId

`func (o *IntegrationMapping) SetExternalProductId(v string)`

SetExternalProductId sets ExternalProductId field to given value.


### GetExternalPriceId

`func (o *IntegrationMapping) GetExternalPriceId() string`

GetExternalPriceId returns the ExternalPriceId field if non-nil, zero value otherwise.

### GetExternalPriceIdOk

`func (o *IntegrationMapping) GetExternalPriceIdOk() (*string, bool)`

GetExternalPriceIdOk returns a tuple with the ExternalPriceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExternalPriceId

`func (o *IntegrationMapping) SetExternalPriceId(v string)`

SetExternalPriceId sets ExternalPriceId field to given value.


### GetStripeProductId

`func (o *IntegrationMapping) GetStripeProductId() string`

GetStripeProductId returns the StripeProductId field if non-nil, zero value otherwise.

### GetStripeProductIdOk

`func (o *IntegrationMapping) GetStripeProductIdOk() (*string, bool)`

GetStripeProductIdOk returns a tuple with the StripeProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripeProductId

`func (o *IntegrationMapping) SetStripeProductId(v string)`

SetStripeProductId sets StripeProductId field to given value.


### GetStripePriceId

`func (o *IntegrationMapping) GetStripePriceId() string`

GetStripePriceId returns the StripePriceId field if non-nil, zero value otherwise.

### GetStripePriceIdOk

`func (o *IntegrationMapping) GetStripePriceIdOk() (*string, bool)`

GetStripePriceIdOk returns a tuple with the StripePriceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripePriceId

`func (o *IntegrationMapping) SetStripePriceId(v string)`

SetStripePriceId sets StripePriceId field to given value.


### GetProductName

`func (o *IntegrationMapping) GetProductName() string`

GetProductName returns the ProductName field if non-nil, zero value otherwise.

### GetProductNameOk

`func (o *IntegrationMapping) GetProductNameOk() (*string, bool)`

GetProductNameOk returns a tuple with the ProductName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductName

`func (o *IntegrationMapping) SetProductName(v string)`

SetProductName sets ProductName field to given value.


### GetPrice

`func (o *IntegrationMapping) GetPrice() Price`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *IntegrationMapping) GetPriceOk() (*Price, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *IntegrationMapping) SetPrice(v Price)`

SetPrice sets Price field to given value.


### SetPriceNil

`func (o *IntegrationMapping) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *IntegrationMapping) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetRecurring

`func (o *IntegrationMapping) GetRecurring() IntegrationMappingRecurring`

GetRecurring returns the Recurring field if non-nil, zero value otherwise.

### GetRecurringOk

`func (o *IntegrationMapping) GetRecurringOk() (*IntegrationMappingRecurring, bool)`

GetRecurringOk returns a tuple with the Recurring field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecurring

`func (o *IntegrationMapping) SetRecurring(v IntegrationMappingRecurring)`

SetRecurring sets Recurring field to given value.


### SetRecurringNil

`func (o *IntegrationMapping) SetRecurringNil(b bool)`

 SetRecurringNil sets the value for Recurring to be an explicit nil

### UnsetRecurring
`func (o *IntegrationMapping) UnsetRecurring()`

UnsetRecurring ensures that no value is present for Recurring, not even an explicit nil
### GetStatus

`func (o *IntegrationMapping) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *IntegrationMapping) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *IntegrationMapping) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetStatusReason

`func (o *IntegrationMapping) GetStatusReason() string`

GetStatusReason returns the StatusReason field if non-nil, zero value otherwise.

### GetStatusReasonOk

`func (o *IntegrationMapping) GetStatusReasonOk() (*string, bool)`

GetStatusReasonOk returns a tuple with the StatusReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusReason

`func (o *IntegrationMapping) SetStatusReason(v string)`

SetStatusReason sets StatusReason field to given value.


### SetStatusReasonNil

`func (o *IntegrationMapping) SetStatusReasonNil(b bool)`

 SetStatusReasonNil sets the value for StatusReason to be an explicit nil

### UnsetStatusReason
`func (o *IntegrationMapping) UnsetStatusReason()`

UnsetStatusReason ensures that no value is present for StatusReason, not even an explicit nil
### GetCreatedAt

`func (o *IntegrationMapping) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *IntegrationMapping) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *IntegrationMapping) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


