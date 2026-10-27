# CancelLicense

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Reason** | [**CancellationReason**](CancellationReason.md) |  | 
**Comment** | Pointer to **string** | What the customer said about the cancellation. | [optional] 
**Refund** | Pointer to **bool** | Whether to refund the license&#39;s Stripe payment, when it was bought through the Stripe integration. Defaults to the integration&#39;s &#x60;autoRefund&#x60;. Ignored for tokens, which always follow &#x60;autoRefund&#x60;, and when the integration&#39;s &#x60;canRefund&#x60; is false: its API key can&#39;t create refunds. | [optional] 

## Methods

### NewCancelLicense

`func NewCancelLicense(reason CancellationReason, ) *CancelLicense`

NewCancelLicense instantiates a new CancelLicense object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCancelLicenseWithDefaults

`func NewCancelLicenseWithDefaults() *CancelLicense`

NewCancelLicenseWithDefaults instantiates a new CancelLicense object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReason

`func (o *CancelLicense) GetReason() CancellationReason`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *CancelLicense) GetReasonOk() (*CancellationReason, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *CancelLicense) SetReason(v CancellationReason)`

SetReason sets Reason field to given value.


### GetComment

`func (o *CancelLicense) GetComment() string`

GetComment returns the Comment field if non-nil, zero value otherwise.

### GetCommentOk

`func (o *CancelLicense) GetCommentOk() (*string, bool)`

GetCommentOk returns a tuple with the Comment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetComment

`func (o *CancelLicense) SetComment(v string)`

SetComment sets Comment field to given value.

### HasComment

`func (o *CancelLicense) HasComment() bool`

HasComment returns a boolean if a field has been set.

### GetRefund

`func (o *CancelLicense) GetRefund() bool`

GetRefund returns the Refund field if non-nil, zero value otherwise.

### GetRefundOk

`func (o *CancelLicense) GetRefundOk() (*bool, bool)`

GetRefundOk returns a tuple with the Refund field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefund

`func (o *CancelLicense) SetRefund(v bool)`

SetRefund sets Refund field to given value.

### HasRefund

`func (o *CancelLicense) HasRefund() bool`

HasRefund returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


