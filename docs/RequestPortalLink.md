# RequestPortalLink

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** | Email of the customer. | 
**ReturnUrl** | Pointer to **string** | Link back to your website, kept in the emailed link when its domain is one of the product&#39;s &#x60;returnDomains&#x60;. | [optional] 

## Methods

### NewRequestPortalLink

`func NewRequestPortalLink(email string, ) *RequestPortalLink`

NewRequestPortalLink instantiates a new RequestPortalLink object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRequestPortalLinkWithDefaults

`func NewRequestPortalLinkWithDefaults() *RequestPortalLink`

NewRequestPortalLinkWithDefaults instantiates a new RequestPortalLink object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *RequestPortalLink) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *RequestPortalLink) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *RequestPortalLink) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetReturnUrl

`func (o *RequestPortalLink) GetReturnUrl() string`

GetReturnUrl returns the ReturnUrl field if non-nil, zero value otherwise.

### GetReturnUrlOk

`func (o *RequestPortalLink) GetReturnUrlOk() (*string, bool)`

GetReturnUrlOk returns a tuple with the ReturnUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnUrl

`func (o *RequestPortalLink) SetReturnUrl(v string)`

SetReturnUrl sets ReturnUrl field to given value.

### HasReturnUrl

`func (o *RequestPortalLink) HasReturnUrl() bool`

HasReturnUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


