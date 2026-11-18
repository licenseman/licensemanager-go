# PortalSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether customers can use the customer portal. When disabled, it answers &#x60;404&#x60;. | 
**BrandColor** | **NullableString** | Background of the portal&#39;s side panel, as &#x60;#rrggbb&#x60;, stored lower cased. &#x60;null&#x60; for the default color. | 
**AccentColor** | **NullableString** | Color of the portal&#39;s inputs and buttons, as &#x60;#rrggbb&#x60;, stored lower cased. &#x60;null&#x60; for the default color. | 
**ReturnDomains** | **[]string** | Domains the portal&#39;s &#x60;return_url&#x60; query parameter may point to, their subdomains included. Other return URLs are ignored, in favor of the product&#39;s &#x60;websiteUrl&#x60;. | 

## Methods

### NewPortalSettings

`func NewPortalSettings(enabled bool, brandColor NullableString, accentColor NullableString, returnDomains []string, ) *PortalSettings`

NewPortalSettings instantiates a new PortalSettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPortalSettingsWithDefaults

`func NewPortalSettingsWithDefaults() *PortalSettings`

NewPortalSettingsWithDefaults instantiates a new PortalSettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *PortalSettings) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *PortalSettings) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *PortalSettings) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetBrandColor

`func (o *PortalSettings) GetBrandColor() string`

GetBrandColor returns the BrandColor field if non-nil, zero value otherwise.

### GetBrandColorOk

`func (o *PortalSettings) GetBrandColorOk() (*string, bool)`

GetBrandColorOk returns a tuple with the BrandColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandColor

`func (o *PortalSettings) SetBrandColor(v string)`

SetBrandColor sets BrandColor field to given value.


### SetBrandColorNil

`func (o *PortalSettings) SetBrandColorNil(b bool)`

 SetBrandColorNil sets the value for BrandColor to be an explicit nil

### UnsetBrandColor
`func (o *PortalSettings) UnsetBrandColor()`

UnsetBrandColor ensures that no value is present for BrandColor, not even an explicit nil
### GetAccentColor

`func (o *PortalSettings) GetAccentColor() string`

GetAccentColor returns the AccentColor field if non-nil, zero value otherwise.

### GetAccentColorOk

`func (o *PortalSettings) GetAccentColorOk() (*string, bool)`

GetAccentColorOk returns a tuple with the AccentColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccentColor

`func (o *PortalSettings) SetAccentColor(v string)`

SetAccentColor sets AccentColor field to given value.


### SetAccentColorNil

`func (o *PortalSettings) SetAccentColorNil(b bool)`

 SetAccentColorNil sets the value for AccentColor to be an explicit nil

### UnsetAccentColor
`func (o *PortalSettings) UnsetAccentColor()`

UnsetAccentColor ensures that no value is present for AccentColor, not even an explicit nil
### GetReturnDomains

`func (o *PortalSettings) GetReturnDomains() []string`

GetReturnDomains returns the ReturnDomains field if non-nil, zero value otherwise.

### GetReturnDomainsOk

`func (o *PortalSettings) GetReturnDomainsOk() (*[]string, bool)`

GetReturnDomainsOk returns a tuple with the ReturnDomains field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnDomains

`func (o *PortalSettings) SetReturnDomains(v []string)`

SetReturnDomains sets ReturnDomains field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


