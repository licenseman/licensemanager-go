# CreateToken

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Scope** | **[]string** | Permissions of the token. A write permission implies the other ones of its resource, like the read one: &#x60;license:write&#x60; implies &#x60;license:read&#x60; and &#x60;license:cancel&#x60;. A token creating a token can only give the permissions it has. | 
**ExpiresInSeconds** | Pointer to **int32** | How long the token works, in seconds, from 60 (1 minute) to 31536000 (365 days). Defaults to 900 (15 minutes). A token creating a token can&#39;t give it a later expiration than its own: it&#39;s shortened to it. | [optional] [default to 900]

## Methods

### NewCreateToken

`func NewCreateToken(scope []string, ) *CreateToken`

NewCreateToken instantiates a new CreateToken object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateTokenWithDefaults

`func NewCreateTokenWithDefaults() *CreateToken`

NewCreateTokenWithDefaults instantiates a new CreateToken object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetScope

`func (o *CreateToken) GetScope() []string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *CreateToken) GetScopeOk() (*[]string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *CreateToken) SetScope(v []string)`

SetScope sets Scope field to given value.


### GetExpiresInSeconds

`func (o *CreateToken) GetExpiresInSeconds() int32`

GetExpiresInSeconds returns the ExpiresInSeconds field if non-nil, zero value otherwise.

### GetExpiresInSecondsOk

`func (o *CreateToken) GetExpiresInSecondsOk() (*int32, bool)`

GetExpiresInSecondsOk returns a tuple with the ExpiresInSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresInSeconds

`func (o *CreateToken) SetExpiresInSeconds(v int32)`

SetExpiresInSeconds sets ExpiresInSeconds field to given value.

### HasExpiresInSeconds

`func (o *CreateToken) HasExpiresInSeconds() bool`

HasExpiresInSeconds returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


