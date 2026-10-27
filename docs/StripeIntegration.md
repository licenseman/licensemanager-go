# StripeIntegration

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Livemode** | **bool** | Mode of the Stripe connection the product uses: live for live products, test for test products. | 
**WebhookUrlReachable** | **bool** | Whether Stripe can reach the API&#39;s webhook URL. A local URL can&#39;t be: set &#x60;WEBHOOK_URL&#x60; on the server, like to a tunnel in development. | 
**RequiredPermissions** | [**[]StripePermission**](StripePermission.md) | Permissions the restricted API key needs, and why, the &#x60;optional&#x60; ones included. Every other permission can stay &#x60;None&#x60;. | 
**Integration** | [**NullableIntegration**](Integration.md) | The organization&#39;s Stripe connection in this mode, &#x60;null&#x60; when there&#39;s none. | 
**Mappings** | [**[]IntegrationMapping**](IntegrationMapping.md) | Stripe prices creating licenses of the product. | 

## Methods

### NewStripeIntegration

`func NewStripeIntegration(livemode bool, webhookUrlReachable bool, requiredPermissions []StripePermission, integration NullableIntegration, mappings []IntegrationMapping, ) *StripeIntegration`

NewStripeIntegration instantiates a new StripeIntegration object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStripeIntegrationWithDefaults

`func NewStripeIntegrationWithDefaults() *StripeIntegration`

NewStripeIntegrationWithDefaults instantiates a new StripeIntegration object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLivemode

`func (o *StripeIntegration) GetLivemode() bool`

GetLivemode returns the Livemode field if non-nil, zero value otherwise.

### GetLivemodeOk

`func (o *StripeIntegration) GetLivemodeOk() (*bool, bool)`

GetLivemodeOk returns a tuple with the Livemode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLivemode

`func (o *StripeIntegration) SetLivemode(v bool)`

SetLivemode sets Livemode field to given value.


### GetWebhookUrlReachable

`func (o *StripeIntegration) GetWebhookUrlReachable() bool`

GetWebhookUrlReachable returns the WebhookUrlReachable field if non-nil, zero value otherwise.

### GetWebhookUrlReachableOk

`func (o *StripeIntegration) GetWebhookUrlReachableOk() (*bool, bool)`

GetWebhookUrlReachableOk returns a tuple with the WebhookUrlReachable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrlReachable

`func (o *StripeIntegration) SetWebhookUrlReachable(v bool)`

SetWebhookUrlReachable sets WebhookUrlReachable field to given value.


### GetRequiredPermissions

`func (o *StripeIntegration) GetRequiredPermissions() []StripePermission`

GetRequiredPermissions returns the RequiredPermissions field if non-nil, zero value otherwise.

### GetRequiredPermissionsOk

`func (o *StripeIntegration) GetRequiredPermissionsOk() (*[]StripePermission, bool)`

GetRequiredPermissionsOk returns a tuple with the RequiredPermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiredPermissions

`func (o *StripeIntegration) SetRequiredPermissions(v []StripePermission)`

SetRequiredPermissions sets RequiredPermissions field to given value.


### GetIntegration

`func (o *StripeIntegration) GetIntegration() Integration`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *StripeIntegration) GetIntegrationOk() (*Integration, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *StripeIntegration) SetIntegration(v Integration)`

SetIntegration sets Integration field to given value.


### SetIntegrationNil

`func (o *StripeIntegration) SetIntegrationNil(b bool)`

 SetIntegrationNil sets the value for Integration to be an explicit nil

### UnsetIntegration
`func (o *StripeIntegration) UnsetIntegration()`

UnsetIntegration ensures that no value is present for Integration, not even an explicit nil
### GetMappings

`func (o *StripeIntegration) GetMappings() []IntegrationMapping`

GetMappings returns the Mappings field if non-nil, zero value otherwise.

### GetMappingsOk

`func (o *StripeIntegration) GetMappingsOk() (*[]IntegrationMapping, bool)`

GetMappingsOk returns a tuple with the Mappings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMappings

`func (o *StripeIntegration) SetMappings(v []IntegrationMapping)`

SetMappings sets Mappings field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


