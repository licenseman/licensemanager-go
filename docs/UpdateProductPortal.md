# UpdateProductPortal

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** | Whether customers can use the customer portal. When disabled, it answers &#x60;404&#x60;. | [optional] 
**BrandColor** | Pointer to **NullableString** | Background of the portal&#39;s side panel, as &#x60;#rrggbb&#x60;, stored lower cased. &#x60;null&#x60; for the default color. | [optional] 
**AccentColor** | Pointer to **NullableString** | Color of the portal&#39;s inputs and buttons, as &#x60;#rrggbb&#x60;, stored lower cased. &#x60;null&#x60; for the default color. | [optional] 
**ReturnUrl** | Pointer to **NullableString** | Link back to your website shown in the portal, when the portal&#39;s URL has no allowed &#x60;return_url&#x60;. &#x60;null&#x60; for no link. | [optional] 
**ReturnDomains** | Pointer to **[]string** | Domains the portal&#39;s &#x60;return_url&#x60; query parameter may point to, their subdomains included. Other return URLs are ignored, in favor of &#x60;returnUrl&#x60;. | [optional] 

## Methods

### NewUpdateProductPortal

`func NewUpdateProductPortal() *UpdateProductPortal`

NewUpdateProductPortal instantiates a new UpdateProductPortal object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateProductPortalWithDefaults

`func NewUpdateProductPortalWithDefaults() *UpdateProductPortal`

NewUpdateProductPortalWithDefaults instantiates a new UpdateProductPortal object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *UpdateProductPortal) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *UpdateProductPortal) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *UpdateProductPortal) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *UpdateProductPortal) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetBrandColor

`func (o *UpdateProductPortal) GetBrandColor() string`

GetBrandColor returns the BrandColor field if non-nil, zero value otherwise.

### GetBrandColorOk

`func (o *UpdateProductPortal) GetBrandColorOk() (*string, bool)`

GetBrandColorOk returns a tuple with the BrandColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandColor

`func (o *UpdateProductPortal) SetBrandColor(v string)`

SetBrandColor sets BrandColor field to given value.

### HasBrandColor

`func (o *UpdateProductPortal) HasBrandColor() bool`

HasBrandColor returns a boolean if a field has been set.

### SetBrandColorNil

`func (o *UpdateProductPortal) SetBrandColorNil(b bool)`

 SetBrandColorNil sets the value for BrandColor to be an explicit nil

### UnsetBrandColor
`func (o *UpdateProductPortal) UnsetBrandColor()`

UnsetBrandColor ensures that no value is present for BrandColor, not even an explicit nil
### GetAccentColor

`func (o *UpdateProductPortal) GetAccentColor() string`

GetAccentColor returns the AccentColor field if non-nil, zero value otherwise.

### GetAccentColorOk

`func (o *UpdateProductPortal) GetAccentColorOk() (*string, bool)`

GetAccentColorOk returns a tuple with the AccentColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccentColor

`func (o *UpdateProductPortal) SetAccentColor(v string)`

SetAccentColor sets AccentColor field to given value.

### HasAccentColor

`func (o *UpdateProductPortal) HasAccentColor() bool`

HasAccentColor returns a boolean if a field has been set.

### SetAccentColorNil

`func (o *UpdateProductPortal) SetAccentColorNil(b bool)`

 SetAccentColorNil sets the value for AccentColor to be an explicit nil

### UnsetAccentColor
`func (o *UpdateProductPortal) UnsetAccentColor()`

UnsetAccentColor ensures that no value is present for AccentColor, not even an explicit nil
### GetReturnUrl

`func (o *UpdateProductPortal) GetReturnUrl() string`

GetReturnUrl returns the ReturnUrl field if non-nil, zero value otherwise.

### GetReturnUrlOk

`func (o *UpdateProductPortal) GetReturnUrlOk() (*string, bool)`

GetReturnUrlOk returns a tuple with the ReturnUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnUrl

`func (o *UpdateProductPortal) SetReturnUrl(v string)`

SetReturnUrl sets ReturnUrl field to given value.

### HasReturnUrl

`func (o *UpdateProductPortal) HasReturnUrl() bool`

HasReturnUrl returns a boolean if a field has been set.

### SetReturnUrlNil

`func (o *UpdateProductPortal) SetReturnUrlNil(b bool)`

 SetReturnUrlNil sets the value for ReturnUrl to be an explicit nil

### UnsetReturnUrl
`func (o *UpdateProductPortal) UnsetReturnUrl()`

UnsetReturnUrl ensures that no value is present for ReturnUrl, not even an explicit nil
### GetReturnDomains

`func (o *UpdateProductPortal) GetReturnDomains() []string`

GetReturnDomains returns the ReturnDomains field if non-nil, zero value otherwise.

### GetReturnDomainsOk

`func (o *UpdateProductPortal) GetReturnDomainsOk() (*[]string, bool)`

GetReturnDomainsOk returns a tuple with the ReturnDomains field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnDomains

`func (o *UpdateProductPortal) SetReturnDomains(v []string)`

SetReturnDomains sets ReturnDomains field to given value.

### HasReturnDomains

`func (o *UpdateProductPortal) HasReturnDomains() bool`

HasReturnDomains returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


