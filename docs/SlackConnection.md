# SlackConnection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**TeamId** | **string** |  | 
**TeamName** | **NullableString** |  | 
**ChannelId** | **string** |  | 
**ChannelName** | **NullableString** | Name of the channel when it was connected, with its &#x60;#&#x60;. | 
**ConfigurationUrl** | **NullableString** | Page of the installation in Slack. | 
**Events** | **[]string** | Notifications the channel gets: &#x60;purchased&#x60; (a license bought through Stripe or Paddle), &#x60;renewed&#x60; (a subscription renewal paid), &#x60;payment_failed&#x60; (a subscription payment failed) and &#x60;canceled&#x60; (a license canceled, or its subscription ended). | 
**Status** | **string** | &#x60;revoked&#x60; once Slack refuses the messages, like when the app was removed from the workspace or the channel deleted: remove it and add it again. | 
**StatusReason** | **NullableString** |  | 
**LastSentAt** | **NullableTime** |  | 
**CreatedAt** | **time.Time** |  | 

## Methods

### NewSlackConnection

`func NewSlackConnection(id string, teamId string, teamName NullableString, channelId string, channelName NullableString, configurationUrl NullableString, events []string, status string, statusReason NullableString, lastSentAt NullableTime, createdAt time.Time, ) *SlackConnection`

NewSlackConnection instantiates a new SlackConnection object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSlackConnectionWithDefaults

`func NewSlackConnectionWithDefaults() *SlackConnection`

NewSlackConnectionWithDefaults instantiates a new SlackConnection object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SlackConnection) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SlackConnection) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SlackConnection) SetId(v string)`

SetId sets Id field to given value.


### GetTeamId

`func (o *SlackConnection) GetTeamId() string`

GetTeamId returns the TeamId field if non-nil, zero value otherwise.

### GetTeamIdOk

`func (o *SlackConnection) GetTeamIdOk() (*string, bool)`

GetTeamIdOk returns a tuple with the TeamId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamId

`func (o *SlackConnection) SetTeamId(v string)`

SetTeamId sets TeamId field to given value.


### GetTeamName

`func (o *SlackConnection) GetTeamName() string`

GetTeamName returns the TeamName field if non-nil, zero value otherwise.

### GetTeamNameOk

`func (o *SlackConnection) GetTeamNameOk() (*string, bool)`

GetTeamNameOk returns a tuple with the TeamName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTeamName

`func (o *SlackConnection) SetTeamName(v string)`

SetTeamName sets TeamName field to given value.


### SetTeamNameNil

`func (o *SlackConnection) SetTeamNameNil(b bool)`

 SetTeamNameNil sets the value for TeamName to be an explicit nil

### UnsetTeamName
`func (o *SlackConnection) UnsetTeamName()`

UnsetTeamName ensures that no value is present for TeamName, not even an explicit nil
### GetChannelId

`func (o *SlackConnection) GetChannelId() string`

GetChannelId returns the ChannelId field if non-nil, zero value otherwise.

### GetChannelIdOk

`func (o *SlackConnection) GetChannelIdOk() (*string, bool)`

GetChannelIdOk returns a tuple with the ChannelId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannelId

`func (o *SlackConnection) SetChannelId(v string)`

SetChannelId sets ChannelId field to given value.


### GetChannelName

`func (o *SlackConnection) GetChannelName() string`

GetChannelName returns the ChannelName field if non-nil, zero value otherwise.

### GetChannelNameOk

`func (o *SlackConnection) GetChannelNameOk() (*string, bool)`

GetChannelNameOk returns a tuple with the ChannelName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChannelName

`func (o *SlackConnection) SetChannelName(v string)`

SetChannelName sets ChannelName field to given value.


### SetChannelNameNil

`func (o *SlackConnection) SetChannelNameNil(b bool)`

 SetChannelNameNil sets the value for ChannelName to be an explicit nil

### UnsetChannelName
`func (o *SlackConnection) UnsetChannelName()`

UnsetChannelName ensures that no value is present for ChannelName, not even an explicit nil
### GetConfigurationUrl

`func (o *SlackConnection) GetConfigurationUrl() string`

GetConfigurationUrl returns the ConfigurationUrl field if non-nil, zero value otherwise.

### GetConfigurationUrlOk

`func (o *SlackConnection) GetConfigurationUrlOk() (*string, bool)`

GetConfigurationUrlOk returns a tuple with the ConfigurationUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigurationUrl

`func (o *SlackConnection) SetConfigurationUrl(v string)`

SetConfigurationUrl sets ConfigurationUrl field to given value.


### SetConfigurationUrlNil

`func (o *SlackConnection) SetConfigurationUrlNil(b bool)`

 SetConfigurationUrlNil sets the value for ConfigurationUrl to be an explicit nil

### UnsetConfigurationUrl
`func (o *SlackConnection) UnsetConfigurationUrl()`

UnsetConfigurationUrl ensures that no value is present for ConfigurationUrl, not even an explicit nil
### GetEvents

`func (o *SlackConnection) GetEvents() []string`

GetEvents returns the Events field if non-nil, zero value otherwise.

### GetEventsOk

`func (o *SlackConnection) GetEventsOk() (*[]string, bool)`

GetEventsOk returns a tuple with the Events field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvents

`func (o *SlackConnection) SetEvents(v []string)`

SetEvents sets Events field to given value.


### GetStatus

`func (o *SlackConnection) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SlackConnection) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SlackConnection) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetStatusReason

`func (o *SlackConnection) GetStatusReason() string`

GetStatusReason returns the StatusReason field if non-nil, zero value otherwise.

### GetStatusReasonOk

`func (o *SlackConnection) GetStatusReasonOk() (*string, bool)`

GetStatusReasonOk returns a tuple with the StatusReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusReason

`func (o *SlackConnection) SetStatusReason(v string)`

SetStatusReason sets StatusReason field to given value.


### SetStatusReasonNil

`func (o *SlackConnection) SetStatusReasonNil(b bool)`

 SetStatusReasonNil sets the value for StatusReason to be an explicit nil

### UnsetStatusReason
`func (o *SlackConnection) UnsetStatusReason()`

UnsetStatusReason ensures that no value is present for StatusReason, not even an explicit nil
### GetLastSentAt

`func (o *SlackConnection) GetLastSentAt() time.Time`

GetLastSentAt returns the LastSentAt field if non-nil, zero value otherwise.

### GetLastSentAtOk

`func (o *SlackConnection) GetLastSentAtOk() (*time.Time, bool)`

GetLastSentAtOk returns a tuple with the LastSentAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSentAt

`func (o *SlackConnection) SetLastSentAt(v time.Time)`

SetLastSentAt sets LastSentAt field to given value.


### SetLastSentAtNil

`func (o *SlackConnection) SetLastSentAtNil(b bool)`

 SetLastSentAtNil sets the value for LastSentAt to be an explicit nil

### UnsetLastSentAt
`func (o *SlackConnection) UnsetLastSentAt()`

UnsetLastSentAt ensures that no value is present for LastSentAt, not even an explicit nil
### GetCreatedAt

`func (o *SlackConnection) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *SlackConnection) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *SlackConnection) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


