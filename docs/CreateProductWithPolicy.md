# CreateProductWithPolicy

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Slug** | Pointer to **string** | Unique within the organization. Defaults to the name, lower cased, without accents and special characters. Starts with &#x60;test_&#x60; in test products, which is added when missing, and removed in live products. | [optional] 
**DefaultPolicy** | Pointer to [**PolicySettings**](PolicySettings.md) |  | [optional] 
**IsTestFromProductId** | Pointer to **string** | Creates a test product: a sandbox of this live product of the organization, starting with copies of its policies, releases and portal settings. | [optional] 

## Methods

### NewCreateProductWithPolicy

`func NewCreateProductWithPolicy(name string, ) *CreateProductWithPolicy`

NewCreateProductWithPolicy instantiates a new CreateProductWithPolicy object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateProductWithPolicyWithDefaults

`func NewCreateProductWithPolicyWithDefaults() *CreateProductWithPolicy`

NewCreateProductWithPolicyWithDefaults instantiates a new CreateProductWithPolicy object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateProductWithPolicy) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateProductWithPolicy) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateProductWithPolicy) SetName(v string)`

SetName sets Name field to given value.


### GetSlug

`func (o *CreateProductWithPolicy) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *CreateProductWithPolicy) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *CreateProductWithPolicy) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *CreateProductWithPolicy) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### GetDefaultPolicy

`func (o *CreateProductWithPolicy) GetDefaultPolicy() PolicySettings`

GetDefaultPolicy returns the DefaultPolicy field if non-nil, zero value otherwise.

### GetDefaultPolicyOk

`func (o *CreateProductWithPolicy) GetDefaultPolicyOk() (*PolicySettings, bool)`

GetDefaultPolicyOk returns a tuple with the DefaultPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultPolicy

`func (o *CreateProductWithPolicy) SetDefaultPolicy(v PolicySettings)`

SetDefaultPolicy sets DefaultPolicy field to given value.

### HasDefaultPolicy

`func (o *CreateProductWithPolicy) HasDefaultPolicy() bool`

HasDefaultPolicy returns a boolean if a field has been set.

### GetIsTestFromProductId

`func (o *CreateProductWithPolicy) GetIsTestFromProductId() string`

GetIsTestFromProductId returns the IsTestFromProductId field if non-nil, zero value otherwise.

### GetIsTestFromProductIdOk

`func (o *CreateProductWithPolicy) GetIsTestFromProductIdOk() (*string, bool)`

GetIsTestFromProductIdOk returns a tuple with the IsTestFromProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsTestFromProductId

`func (o *CreateProductWithPolicy) SetIsTestFromProductId(v string)`

SetIsTestFromProductId sets IsTestFromProductId field to given value.

### HasIsTestFromProductId

`func (o *CreateProductWithPolicy) HasIsTestFromProductId() bool`

HasIsTestFromProductId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


