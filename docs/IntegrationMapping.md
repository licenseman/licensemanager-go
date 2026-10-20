# IntegrationMapping

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**IntegrationId** | **string** |  | 
**ProductId** | **string** |  | 
**PolicyId** | **string** |  | 
**StripeProductId** | **string** |  | 
**StripePriceId** | **string** |  | 
**ProductName** | **string** | Name of the Stripe product when it was mapped. | 
**Price** | [**NullablePrice**](Price.md) |  | 
**Status** | **string** | &#x60;error&#x60; when the price can no longer be paid, explained by &#x60;statusReason&#x60;. | 
**StatusReason** | **NullableString** |  | 
**CreatedAt** | **time.Time** |  | 

## Methods

### NewIntegrationMapping

`func NewIntegrationMapping(id string, integrationId string, productId string, policyId string, stripeProductId string, stripePriceId string, productName string, price NullablePrice, status string, statusReason NullableString, createdAt time.Time, ) *IntegrationMapping`

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


