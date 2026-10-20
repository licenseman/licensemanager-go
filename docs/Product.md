# Product

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Slug** | **string** |  | 
**Name** | **string** |  | 
**IsTestFromProductId** | **NullableString** | For test products, id of the live product they&#39;re a sandbox of. &#x60;null&#x60; for live products. | 
**LogoUrl** | **NullableString** | Public URL of the product&#39;s logo, shown in the web app and the customer portal. &#x60;null&#x60; without a logo. | 
**Portal** | [**PortalSettings**](PortalSettings.md) |  | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewProduct

`func NewProduct(id string, slug string, name string, isTestFromProductId NullableString, logoUrl NullableString, portal PortalSettings, createdAt time.Time, updatedAt time.Time, ) *Product`

NewProduct instantiates a new Product object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductWithDefaults

`func NewProductWithDefaults() *Product`

NewProductWithDefaults instantiates a new Product object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Product) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Product) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Product) SetId(v string)`

SetId sets Id field to given value.


### GetSlug

`func (o *Product) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *Product) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *Product) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetName

`func (o *Product) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Product) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Product) SetName(v string)`

SetName sets Name field to given value.


### GetIsTestFromProductId

`func (o *Product) GetIsTestFromProductId() string`

GetIsTestFromProductId returns the IsTestFromProductId field if non-nil, zero value otherwise.

### GetIsTestFromProductIdOk

`func (o *Product) GetIsTestFromProductIdOk() (*string, bool)`

GetIsTestFromProductIdOk returns a tuple with the IsTestFromProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsTestFromProductId

`func (o *Product) SetIsTestFromProductId(v string)`

SetIsTestFromProductId sets IsTestFromProductId field to given value.


### SetIsTestFromProductIdNil

`func (o *Product) SetIsTestFromProductIdNil(b bool)`

 SetIsTestFromProductIdNil sets the value for IsTestFromProductId to be an explicit nil

### UnsetIsTestFromProductId
`func (o *Product) UnsetIsTestFromProductId()`

UnsetIsTestFromProductId ensures that no value is present for IsTestFromProductId, not even an explicit nil
### GetLogoUrl

`func (o *Product) GetLogoUrl() string`

GetLogoUrl returns the LogoUrl field if non-nil, zero value otherwise.

### GetLogoUrlOk

`func (o *Product) GetLogoUrlOk() (*string, bool)`

GetLogoUrlOk returns a tuple with the LogoUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoUrl

`func (o *Product) SetLogoUrl(v string)`

SetLogoUrl sets LogoUrl field to given value.


### SetLogoUrlNil

`func (o *Product) SetLogoUrlNil(b bool)`

 SetLogoUrlNil sets the value for LogoUrl to be an explicit nil

### UnsetLogoUrl
`func (o *Product) UnsetLogoUrl()`

UnsetLogoUrl ensures that no value is present for LogoUrl, not even an explicit nil
### GetPortal

`func (o *Product) GetPortal() PortalSettings`

GetPortal returns the Portal field if non-nil, zero value otherwise.

### GetPortalOk

`func (o *Product) GetPortalOk() (*PortalSettings, bool)`

GetPortalOk returns a tuple with the Portal field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPortal

`func (o *Product) SetPortal(v PortalSettings)`

SetPortal sets Portal field to given value.


### GetCreatedAt

`func (o *Product) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Product) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Product) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Product) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Product) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Product) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


