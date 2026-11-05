# SlackIntegration

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Configured** | **bool** | Whether the server has a Slack app to connect channels with: &#x60;SLACK_CLIENT_ID&#x60; and &#x60;SLACK_CLIENT_SECRET&#x60; are set. | 
**Connections** | [**[]SlackConnection**](SlackConnection.md) | Slack channels getting the product&#39;s notifications. | 

## Methods

### NewSlackIntegration

`func NewSlackIntegration(configured bool, connections []SlackConnection, ) *SlackIntegration`

NewSlackIntegration instantiates a new SlackIntegration object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSlackIntegrationWithDefaults

`func NewSlackIntegrationWithDefaults() *SlackIntegration`

NewSlackIntegrationWithDefaults instantiates a new SlackIntegration object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConfigured

`func (o *SlackIntegration) GetConfigured() bool`

GetConfigured returns the Configured field if non-nil, zero value otherwise.

### GetConfiguredOk

`func (o *SlackIntegration) GetConfiguredOk() (*bool, bool)`

GetConfiguredOk returns a tuple with the Configured field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigured

`func (o *SlackIntegration) SetConfigured(v bool)`

SetConfigured sets Configured field to given value.


### GetConnections

`func (o *SlackIntegration) GetConnections() []SlackConnection`

GetConnections returns the Connections field if non-nil, zero value otherwise.

### GetConnectionsOk

`func (o *SlackIntegration) GetConnectionsOk() (*[]SlackConnection, bool)`

GetConnectionsOk returns a tuple with the Connections field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConnections

`func (o *SlackIntegration) SetConnections(v []SlackConnection)`

SetConnections sets Connections field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


