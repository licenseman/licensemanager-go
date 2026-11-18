# UpdateProduct

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** |  | [optional] 
**Slug** | Pointer to **string** | Unique within the organization. Defaults to the name, lower cased, without accents and special characters. Starts with &#x60;test_&#x60; in test products, which is added when missing, and removed in live products. | [optional] 
**WebsiteUrl** | Pointer to **NullableString** | The product&#39;s website, linked from the customer portal, when its URL has no allowed &#x60;return_url&#x60;, and from the emails sent to customers. &#x60;null&#x60; for no link. | [optional] 
**DownloadUrl** | Pointer to **NullableString** | Where customers download the product, linked from the email sending their license keys. &#x60;null&#x60; for no link. | [optional] 
**Portal** | Pointer to [**UpdateProductPortal**](UpdateProductPortal.md) |  | [optional] 
**AutoMachineChange** | Pointer to **bool** | Whether a new machine validating a license already on its max machines takes the place of the license&#39;s machine validated the longest ago, rather than being refused with &#x60;machine_limit_reached&#x60;. When the replaced machine is validated again, it takes its place back and the machine that replaced it is locked. See &#x60;validateKey&#x60;. | [optional] 

## Methods

### NewUpdateProduct

`func NewUpdateProduct() *UpdateProduct`

NewUpdateProduct instantiates a new UpdateProduct object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateProductWithDefaults

`func NewUpdateProductWithDefaults() *UpdateProduct`

NewUpdateProductWithDefaults instantiates a new UpdateProduct object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateProduct) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateProduct) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateProduct) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateProduct) HasName() bool`

HasName returns a boolean if a field has been set.

### GetSlug

`func (o *UpdateProduct) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *UpdateProduct) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *UpdateProduct) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *UpdateProduct) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### GetWebsiteUrl

`func (o *UpdateProduct) GetWebsiteUrl() string`

GetWebsiteUrl returns the WebsiteUrl field if non-nil, zero value otherwise.

### GetWebsiteUrlOk

`func (o *UpdateProduct) GetWebsiteUrlOk() (*string, bool)`

GetWebsiteUrlOk returns a tuple with the WebsiteUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebsiteUrl

`func (o *UpdateProduct) SetWebsiteUrl(v string)`

SetWebsiteUrl sets WebsiteUrl field to given value.

### HasWebsiteUrl

`func (o *UpdateProduct) HasWebsiteUrl() bool`

HasWebsiteUrl returns a boolean if a field has been set.

### SetWebsiteUrlNil

`func (o *UpdateProduct) SetWebsiteUrlNil(b bool)`

 SetWebsiteUrlNil sets the value for WebsiteUrl to be an explicit nil

### UnsetWebsiteUrl
`func (o *UpdateProduct) UnsetWebsiteUrl()`

UnsetWebsiteUrl ensures that no value is present for WebsiteUrl, not even an explicit nil
### GetDownloadUrl

`func (o *UpdateProduct) GetDownloadUrl() string`

GetDownloadUrl returns the DownloadUrl field if non-nil, zero value otherwise.

### GetDownloadUrlOk

`func (o *UpdateProduct) GetDownloadUrlOk() (*string, bool)`

GetDownloadUrlOk returns a tuple with the DownloadUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDownloadUrl

`func (o *UpdateProduct) SetDownloadUrl(v string)`

SetDownloadUrl sets DownloadUrl field to given value.

### HasDownloadUrl

`func (o *UpdateProduct) HasDownloadUrl() bool`

HasDownloadUrl returns a boolean if a field has been set.

### SetDownloadUrlNil

`func (o *UpdateProduct) SetDownloadUrlNil(b bool)`

 SetDownloadUrlNil sets the value for DownloadUrl to be an explicit nil

### UnsetDownloadUrl
`func (o *UpdateProduct) UnsetDownloadUrl()`

UnsetDownloadUrl ensures that no value is present for DownloadUrl, not even an explicit nil
### GetPortal

`func (o *UpdateProduct) GetPortal() UpdateProductPortal`

GetPortal returns the Portal field if non-nil, zero value otherwise.

### GetPortalOk

`func (o *UpdateProduct) GetPortalOk() (*UpdateProductPortal, bool)`

GetPortalOk returns a tuple with the Portal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPortal

`func (o *UpdateProduct) SetPortal(v UpdateProductPortal)`

SetPortal sets Portal field to given value.

### HasPortal

`func (o *UpdateProduct) HasPortal() bool`

HasPortal returns a boolean if a field has been set.

### GetAutoMachineChange

`func (o *UpdateProduct) GetAutoMachineChange() bool`

GetAutoMachineChange returns the AutoMachineChange field if non-nil, zero value otherwise.

### GetAutoMachineChangeOk

`func (o *UpdateProduct) GetAutoMachineChangeOk() (*bool, bool)`

GetAutoMachineChangeOk returns a tuple with the AutoMachineChange field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoMachineChange

`func (o *UpdateProduct) SetAutoMachineChange(v bool)`

SetAutoMachineChange sets AutoMachineChange field to given value.

### HasAutoMachineChange

`func (o *UpdateProduct) HasAutoMachineChange() bool`

HasAutoMachineChange returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


