# PaddleIntegration

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Livemode** | **bool** | Environment of the Paddle connection the product uses: live for live products, sandbox for test products. | 
**WebhookUrlReachable** | **bool** | Whether Paddle can reach the API&#39;s webhook URL. A local URL can&#39;t be: set &#x60;WEBHOOK_URL&#x60; on the server, like to a tunnel in development. | 
**RequiredPermissions** | [**[]PaddlePermission**](PaddlePermission.md) | Permissions the API key needs, and why, the &#x60;optional&#x60; ones included. Every other permission can stay off. | 
**Integration** | [**NullableIntegration**](Integration.md) | The organization&#39;s Paddle connection in this environment, &#x60;null&#x60; when there&#39;s none. | 
**Mappings** | [**[]IntegrationMapping**](IntegrationMapping.md) | Paddle prices creating licenses of the product. | 

## Methods

### NewPaddleIntegration

`func NewPaddleIntegration(livemode bool, webhookUrlReachable bool, requiredPermissions []PaddlePermission, integration NullableIntegration, mappings []IntegrationMapping, ) *PaddleIntegration`

NewPaddleIntegration instantiates a new PaddleIntegration object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaddleIntegrationWithDefaults

`func NewPaddleIntegrationWithDefaults() *PaddleIntegration`

NewPaddleIntegrationWithDefaults instantiates a new PaddleIntegration object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLivemode

`func (o *PaddleIntegration) GetLivemode() bool`

GetLivemode returns the Livemode field if non-nil, zero value otherwise.

### GetLivemodeOk

`func (o *PaddleIntegration) GetLivemodeOk() (*bool, bool)`

GetLivemodeOk returns a tuple with the Livemode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLivemode

`func (o *PaddleIntegration) SetLivemode(v bool)`

SetLivemode sets Livemode field to given value.


### GetWebhookUrlReachable

`func (o *PaddleIntegration) GetWebhookUrlReachable() bool`

GetWebhookUrlReachable returns the WebhookUrlReachable field if non-nil, zero value otherwise.

### GetWebhookUrlReachableOk

`func (o *PaddleIntegration) GetWebhookUrlReachableOk() (*bool, bool)`

GetWebhookUrlReachableOk returns a tuple with the WebhookUrlReachable field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookUrlReachable

`func (o *PaddleIntegration) SetWebhookUrlReachable(v bool)`

SetWebhookUrlReachable sets WebhookUrlReachable field to given value.


### GetRequiredPermissions

`func (o *PaddleIntegration) GetRequiredPermissions() []PaddlePermission`

GetRequiredPermissions returns the RequiredPermissions field if non-nil, zero value otherwise.

### GetRequiredPermissionsOk

`func (o *PaddleIntegration) GetRequiredPermissionsOk() (*[]PaddlePermission, bool)`

GetRequiredPermissionsOk returns a tuple with the RequiredPermissions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequiredPermissions

`func (o *PaddleIntegration) SetRequiredPermissions(v []PaddlePermission)`

SetRequiredPermissions sets RequiredPermissions field to given value.


### GetIntegration

`func (o *PaddleIntegration) GetIntegration() Integration`

GetIntegration returns the Integration field if non-nil, zero value otherwise.

### GetIntegrationOk

`func (o *PaddleIntegration) GetIntegrationOk() (*Integration, bool)`

GetIntegrationOk returns a tuple with the Integration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntegration

`func (o *PaddleIntegration) SetIntegration(v Integration)`

SetIntegration sets Integration field to given value.


### SetIntegrationNil

`func (o *PaddleIntegration) SetIntegrationNil(b bool)`

 SetIntegrationNil sets the value for Integration to be an explicit nil

### UnsetIntegration
`func (o *PaddleIntegration) UnsetIntegration()`

UnsetIntegration ensures that no value is present for Integration, not even an explicit nil
### GetMappings

`func (o *PaddleIntegration) GetMappings() []IntegrationMapping`

GetMappings returns the Mappings field if non-nil, zero value otherwise.

### GetMappingsOk

`func (o *PaddleIntegration) GetMappingsOk() (*[]IntegrationMapping, bool)`

GetMappingsOk returns a tuple with the Mappings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMappings

`func (o *PaddleIntegration) SetMappings(v []IntegrationMapping)`

SetMappings sets Mappings field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


