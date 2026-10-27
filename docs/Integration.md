# Integration

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Provider** | **string** |  | 
**Livemode** | **bool** | Whether it&#39;s connected in live mode, for the live products, or in test mode, for the test products. | 
**AccountName** | **NullableString** | Name of the Stripe account, &#x60;null&#x60; when the API key can&#39;t read it. | 
**ApiKeyHint** | **string** | Start and end of the API key, to recognize it. | 
**WebhookUrl** | **string** | URL of the webhook endpoint created on the Stripe account. | 
**Status** | [**IntegrationStatus**](IntegrationStatus.md) |  | 
**StatusReason** | **NullableString** | Why the integration isn&#39;t &#x60;active&#x60;, &#x60;null&#x60; when it is. | 
**LastCheckedAt** | **NullableTime** | Last time its health was checked, done every day. | 
**LastEventAt** | **NullableTime** | Last time it received an event from the provider. | 
**AutoRefund** | **bool** | Whether canceling a license bought through Stripe refunds its payment. On by default, always off when &#x60;canRefund&#x60; is false. | 
**CanRefund** | **bool** | Whether the API key has the optional Refunds: Write permission, checked when connecting and every day. Without it, canceled licenses aren&#39;t refunded: refund their payments from Stripe. | 
**CreatedAt** | **time.Time** |  | 

## Methods

### NewIntegration

`func NewIntegration(id string, provider string, livemode bool, accountName NullableString, apiKeyHint string, webhookUrl string, status IntegrationStatus, statusReason NullableString, lastCheckedAt NullableTime, lastEventAt NullableTime, autoRefund bool, canRefund bool, createdAt time.Time, ) *Integration`

NewIntegration instantiates a new Integration object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIntegrationWithDefaults

`func NewIntegrationWithDefaults() *Integration`

NewIntegrationWithDefaults instantiates a new Integration object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Integration) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Integration) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Integration) SetId(v string)`

SetId sets Id field to given value.


### GetProvider

`func (o *Integration) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *Integration) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *Integration) SetProvider(v string)`

SetProvider sets Provider field to given value.


### GetLivemode

`func (o *Integration) GetLivemode() bool`

GetLivemode returns the Livemode field if non-nil, zero value otherwise.

### GetLivemodeOk

`func (o *Integration) GetLivemodeOk() (*bool, bool)`

GetLivemodeOk returns a tuple with the Livemode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLivemode

`func (o *Integration) SetLivemode(v bool)`

SetLivemode sets Livemode field to given value.


### GetAccountName

`func (o *Integration) GetAccountName() string`

GetAccountName returns the AccountName field if non-nil, zero value otherwise.

### GetAccountNameOk

`func (o *Integration) GetAccountNameOk() (*string, bool)`

GetAccountNameOk returns a tuple with the AccountName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccountName

`func (o *Integration) SetAccountName(v string)`

SetAccountName sets AccountName field to given value.


### SetAccountNameNil

`func (o *Integration) SetAccountNameNil(b bool)`

 SetAccountNameNil sets the value for AccountName to be an explicit nil

### UnsetAccountName
`func (o *Integration) UnsetAccountName()`

UnsetAccountName ensures that no value is present for AccountName, not even an explicit nil
### GetApiKeyHint

`func (o *Integration) GetApiKeyHint() string`

GetApiKeyHint returns the ApiKeyHint field if non-nil, zero value otherwise.

### GetApiKeyHintOk

`func (o *Integration) GetApiKeyHintOk() (*string, bool)`

GetApiKeyHintOk returns a tuple with the ApiKeyHint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiKeyHint

`func (o *Integration) SetApiKeyHint(v string)`

SetApiKeyHint sets ApiKeyHint field to given value.


### GetWebhookUrl

`func (o *Integration) GetWebhookUrl() string`

GetWebhookUrl returns the WebhookUrl field if non-nil, zero value otherwise.

### GetWebhookUrlOk

`func (o *Integration) GetWebhookUrlOk() (*string, bool)`

GetWebhookUrlOk returns a tuple with the WebhookUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrl

`func (o *Integration) SetWebhookUrl(v string)`

SetWebhookUrl sets WebhookUrl field to given value.


### GetStatus

`func (o *Integration) GetStatus() IntegrationStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Integration) GetStatusOk() (*IntegrationStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Integration) SetStatus(v IntegrationStatus)`

SetStatus sets Status field to given value.


### GetStatusReason

`func (o *Integration) GetStatusReason() string`

GetStatusReason returns the StatusReason field if non-nil, zero value otherwise.

### GetStatusReasonOk

`func (o *Integration) GetStatusReasonOk() (*string, bool)`

GetStatusReasonOk returns a tuple with the StatusReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusReason

`func (o *Integration) SetStatusReason(v string)`

SetStatusReason sets StatusReason field to given value.


### SetStatusReasonNil

`func (o *Integration) SetStatusReasonNil(b bool)`

 SetStatusReasonNil sets the value for StatusReason to be an explicit nil

### UnsetStatusReason
`func (o *Integration) UnsetStatusReason()`

UnsetStatusReason ensures that no value is present for StatusReason, not even an explicit nil
### GetLastCheckedAt

`func (o *Integration) GetLastCheckedAt() time.Time`

GetLastCheckedAt returns the LastCheckedAt field if non-nil, zero value otherwise.

### GetLastCheckedAtOk

`func (o *Integration) GetLastCheckedAtOk() (*time.Time, bool)`

GetLastCheckedAtOk returns a tuple with the LastCheckedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastCheckedAt

`func (o *Integration) SetLastCheckedAt(v time.Time)`

SetLastCheckedAt sets LastCheckedAt field to given value.


### SetLastCheckedAtNil

`func (o *Integration) SetLastCheckedAtNil(b bool)`

 SetLastCheckedAtNil sets the value for LastCheckedAt to be an explicit nil

### UnsetLastCheckedAt
`func (o *Integration) UnsetLastCheckedAt()`

UnsetLastCheckedAt ensures that no value is present for LastCheckedAt, not even an explicit nil
### GetLastEventAt

`func (o *Integration) GetLastEventAt() time.Time`

GetLastEventAt returns the LastEventAt field if non-nil, zero value otherwise.

### GetLastEventAtOk

`func (o *Integration) GetLastEventAtOk() (*time.Time, bool)`

GetLastEventAtOk returns a tuple with the LastEventAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastEventAt

`func (o *Integration) SetLastEventAt(v time.Time)`

SetLastEventAt sets LastEventAt field to given value.


### SetLastEventAtNil

`func (o *Integration) SetLastEventAtNil(b bool)`

 SetLastEventAtNil sets the value for LastEventAt to be an explicit nil

### UnsetLastEventAt
`func (o *Integration) UnsetLastEventAt()`

UnsetLastEventAt ensures that no value is present for LastEventAt, not even an explicit nil
### GetAutoRefund

`func (o *Integration) GetAutoRefund() bool`

GetAutoRefund returns the AutoRefund field if non-nil, zero value otherwise.

### GetAutoRefundOk

`func (o *Integration) GetAutoRefundOk() (*bool, bool)`

GetAutoRefundOk returns a tuple with the AutoRefund field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRefund

`func (o *Integration) SetAutoRefund(v bool)`

SetAutoRefund sets AutoRefund field to given value.


### GetCanRefund

`func (o *Integration) GetCanRefund() bool`

GetCanRefund returns the CanRefund field if non-nil, zero value otherwise.

### GetCanRefundOk

`func (o *Integration) GetCanRefundOk() (*bool, bool)`

GetCanRefundOk returns a tuple with the CanRefund field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanRefund

`func (o *Integration) SetCanRefund(v bool)`

SetCanRefund sets CanRefund field to given value.


### GetCreatedAt

`func (o *Integration) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Integration) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Integration) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


