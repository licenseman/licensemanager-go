# UpdateIntegration

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AutoRefund** | Pointer to **bool** | Whether canceling a license bought through Stripe refunds its payment. Can only be turned on when the integration&#39;s &#x60;canRefund&#x60; is true: the API key has the Refunds: Write permission. | [optional] 

## Methods

### NewUpdateIntegration

`func NewUpdateIntegration() *UpdateIntegration`

NewUpdateIntegration instantiates a new UpdateIntegration object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateIntegrationWithDefaults

`func NewUpdateIntegrationWithDefaults() *UpdateIntegration`

NewUpdateIntegrationWithDefaults instantiates a new UpdateIntegration object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAutoRefund

`func (o *UpdateIntegration) GetAutoRefund() bool`

GetAutoRefund returns the AutoRefund field if non-nil, zero value otherwise.

### GetAutoRefundOk

`func (o *UpdateIntegration) GetAutoRefundOk() (*bool, bool)`

GetAutoRefundOk returns a tuple with the AutoRefund field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRefund

`func (o *UpdateIntegration) SetAutoRefund(v bool)`

SetAutoRefund sets AutoRefund field to given value.

### HasAutoRefund

`func (o *UpdateIntegration) HasAutoRefund() bool`

HasAutoRefund returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


