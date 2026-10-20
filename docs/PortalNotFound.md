# PortalNotFound

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | [**ErrorError**](ErrorError.md) |  | 
**OrganizationSlug** | Pointer to **string** | Slug of the product&#39;s organization. Present on &#x60;portal_disabled&#x60; errors. | [optional] 
**ProductSlug** | Pointer to **string** | Slug of the product. Present on &#x60;portal_disabled&#x60; errors. | [optional] 

## Methods

### NewPortalNotFound

`func NewPortalNotFound(error_ ErrorError, ) *PortalNotFound`

NewPortalNotFound instantiates a new PortalNotFound object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPortalNotFoundWithDefaults

`func NewPortalNotFoundWithDefaults() *PortalNotFound`

NewPortalNotFoundWithDefaults instantiates a new PortalNotFound object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *PortalNotFound) GetError() ErrorError`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *PortalNotFound) GetErrorOk() (*ErrorError, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *PortalNotFound) SetError(v ErrorError)`

SetError sets Error field to given value.


### GetOrganizationSlug

`func (o *PortalNotFound) GetOrganizationSlug() string`

GetOrganizationSlug returns the OrganizationSlug field if non-nil, zero value otherwise.

### GetOrganizationSlugOk

`func (o *PortalNotFound) GetOrganizationSlugOk() (*string, bool)`

GetOrganizationSlugOk returns a tuple with the OrganizationSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationSlug

`func (o *PortalNotFound) SetOrganizationSlug(v string)`

SetOrganizationSlug sets OrganizationSlug field to given value.

### HasOrganizationSlug

`func (o *PortalNotFound) HasOrganizationSlug() bool`

HasOrganizationSlug returns a boolean if a field has been set.

### GetProductSlug

`func (o *PortalNotFound) GetProductSlug() string`

GetProductSlug returns the ProductSlug field if non-nil, zero value otherwise.

### GetProductSlugOk

`func (o *PortalNotFound) GetProductSlugOk() (*string, bool)`

GetProductSlugOk returns a tuple with the ProductSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductSlug

`func (o *PortalNotFound) SetProductSlug(v string)`

SetProductSlug sets ProductSlug field to given value.

### HasProductSlug

`func (o *PortalNotFound) HasProductSlug() bool`

HasProductSlug returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


