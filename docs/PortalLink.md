# PortalLink

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | Link to the customer portal, holding the token. | 
**Token** | **string** | Customer token in the link, with the &#x60;customer:read&#x60;, &#x60;license:read&#x60;, &#x60;license:cancel&#x60; and &#x60;machine:write&#x60; permissions. | 
**ExpiresAt** | **time.Time** | When the link stops working. | 

## Methods

### NewPortalLink

`func NewPortalLink(url string, token string, expiresAt time.Time, ) *PortalLink`

NewPortalLink instantiates a new PortalLink object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPortalLinkWithDefaults

`func NewPortalLinkWithDefaults() *PortalLink`

NewPortalLinkWithDefaults instantiates a new PortalLink object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *PortalLink) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *PortalLink) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *PortalLink) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetToken

`func (o *PortalLink) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *PortalLink) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *PortalLink) SetToken(v string)`

SetToken sets Token field to given value.


### GetExpiresAt

`func (o *PortalLink) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *PortalLink) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *PortalLink) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


