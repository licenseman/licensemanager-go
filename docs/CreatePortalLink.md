# CreatePortalLink

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ExpiresInSeconds** | **int32** | How long the link works, in seconds, from 300 (5 minutes) to 31536000 (365 days). | 

## Methods

### NewCreatePortalLink

`func NewCreatePortalLink(expiresInSeconds int32, ) *CreatePortalLink`

NewCreatePortalLink instantiates a new CreatePortalLink object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePortalLinkWithDefaults

`func NewCreatePortalLinkWithDefaults() *CreatePortalLink`

NewCreatePortalLinkWithDefaults instantiates a new CreatePortalLink object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetExpiresInSeconds

`func (o *CreatePortalLink) GetExpiresInSeconds() int32`

GetExpiresInSeconds returns the ExpiresInSeconds field if non-nil, zero value otherwise.

### GetExpiresInSecondsOk

`func (o *CreatePortalLink) GetExpiresInSecondsOk() (*int32, bool)`

GetExpiresInSecondsOk returns a tuple with the ExpiresInSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresInSeconds

`func (o *CreatePortalLink) SetExpiresInSeconds(v int32)`

SetExpiresInSeconds sets ExpiresInSeconds field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


