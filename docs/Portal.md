# Portal

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProductId** | **string** |  | 
**ProductName** | **string** |  | 
**OrganizationName** | **string** |  | 
**LogoUrl** | **NullableString** | Public URL of the product&#39;s logo. &#x60;null&#x60; without a logo. | 
**BrandColor** | **NullableString** | Background of the side panel, as &#x60;#rrggbb&#x60;. &#x60;null&#x60; for the default color. | 
**AccentColor** | **NullableString** | Color of the inputs and buttons, as &#x60;#rrggbb&#x60;. &#x60;null&#x60; for the default color. | 
**ReturnUrl** | **NullableString** | Link back to the product&#39;s website: the requested &#x60;returnUrl&#x60; when its domain is allowed, the product&#39;s default return link otherwise. &#x60;null&#x60; for no link. | 

## Methods

### NewPortal

`func NewPortal(productId string, productName string, organizationName string, logoUrl NullableString, brandColor NullableString, accentColor NullableString, returnUrl NullableString, ) *Portal`

NewPortal instantiates a new Portal object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPortalWithDefaults

`func NewPortalWithDefaults() *Portal`

NewPortalWithDefaults instantiates a new Portal object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProductId

`func (o *Portal) GetProductId() string`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *Portal) GetProductIdOk() (*string, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *Portal) SetProductId(v string)`

SetProductId sets ProductId field to given value.


### GetProductName

`func (o *Portal) GetProductName() string`

GetProductName returns the ProductName field if non-nil, zero value otherwise.

### GetProductNameOk

`func (o *Portal) GetProductNameOk() (*string, bool)`

GetProductNameOk returns a tuple with the ProductName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductName

`func (o *Portal) SetProductName(v string)`

SetProductName sets ProductName field to given value.


### GetOrganizationName

`func (o *Portal) GetOrganizationName() string`

GetOrganizationName returns the OrganizationName field if non-nil, zero value otherwise.

### GetOrganizationNameOk

`func (o *Portal) GetOrganizationNameOk() (*string, bool)`

GetOrganizationNameOk returns a tuple with the OrganizationName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOrganizationName

`func (o *Portal) SetOrganizationName(v string)`

SetOrganizationName sets OrganizationName field to given value.


### GetLogoUrl

`func (o *Portal) GetLogoUrl() string`

GetLogoUrl returns the LogoUrl field if non-nil, zero value otherwise.

### GetLogoUrlOk

`func (o *Portal) GetLogoUrlOk() (*string, bool)`

GetLogoUrlOk returns a tuple with the LogoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoUrl

`func (o *Portal) SetLogoUrl(v string)`

SetLogoUrl sets LogoUrl field to given value.


### SetLogoUrlNil

`func (o *Portal) SetLogoUrlNil(b bool)`

 SetLogoUrlNil sets the value for LogoUrl to be an explicit nil

### UnsetLogoUrl
`func (o *Portal) UnsetLogoUrl()`

UnsetLogoUrl ensures that no value is present for LogoUrl, not even an explicit nil
### GetBrandColor

`func (o *Portal) GetBrandColor() string`

GetBrandColor returns the BrandColor field if non-nil, zero value otherwise.

### GetBrandColorOk

`func (o *Portal) GetBrandColorOk() (*string, bool)`

GetBrandColorOk returns a tuple with the BrandColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBrandColor

`func (o *Portal) SetBrandColor(v string)`

SetBrandColor sets BrandColor field to given value.


### SetBrandColorNil

`func (o *Portal) SetBrandColorNil(b bool)`

 SetBrandColorNil sets the value for BrandColor to be an explicit nil

### UnsetBrandColor
`func (o *Portal) UnsetBrandColor()`

UnsetBrandColor ensures that no value is present for BrandColor, not even an explicit nil
### GetAccentColor

`func (o *Portal) GetAccentColor() string`

GetAccentColor returns the AccentColor field if non-nil, zero value otherwise.

### GetAccentColorOk

`func (o *Portal) GetAccentColorOk() (*string, bool)`

GetAccentColorOk returns a tuple with the AccentColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccentColor

`func (o *Portal) SetAccentColor(v string)`

SetAccentColor sets AccentColor field to given value.


### SetAccentColorNil

`func (o *Portal) SetAccentColorNil(b bool)`

 SetAccentColorNil sets the value for AccentColor to be an explicit nil

### UnsetAccentColor
`func (o *Portal) UnsetAccentColor()`

UnsetAccentColor ensures that no value is present for AccentColor, not even an explicit nil
### GetReturnUrl

`func (o *Portal) GetReturnUrl() string`

GetReturnUrl returns the ReturnUrl field if non-nil, zero value otherwise.

### GetReturnUrlOk

`func (o *Portal) GetReturnUrlOk() (*string, bool)`

GetReturnUrlOk returns a tuple with the ReturnUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReturnUrl

`func (o *Portal) SetReturnUrl(v string)`

SetReturnUrl sets ReturnUrl field to given value.


### SetReturnUrlNil

`func (o *Portal) SetReturnUrlNil(b bool)`

 SetReturnUrlNil sets the value for ReturnUrl to be an explicit nil

### UnsetReturnUrl
`func (o *Portal) UnsetReturnUrl()`

UnsetReturnUrl ensures that no value is present for ReturnUrl, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


