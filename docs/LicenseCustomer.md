# LicenseCustomer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Email** | **string** |  | 
**Name** | **NullableString** | Display name of the customer. &#x60;null&#x60; when unknown. | 

## Methods

### NewLicenseCustomer

`func NewLicenseCustomer(id string, email string, name NullableString, ) *LicenseCustomer`

NewLicenseCustomer instantiates a new LicenseCustomer object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseCustomerWithDefaults

`func NewLicenseCustomerWithDefaults() *LicenseCustomer`

NewLicenseCustomerWithDefaults instantiates a new LicenseCustomer object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *LicenseCustomer) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *LicenseCustomer) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *LicenseCustomer) SetId(v string)`

SetId sets Id field to given value.


### GetEmail

`func (o *LicenseCustomer) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *LicenseCustomer) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *LicenseCustomer) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetName

`func (o *LicenseCustomer) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *LicenseCustomer) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *LicenseCustomer) SetName(v string)`

SetName sets Name field to given value.


### SetNameNil

`func (o *LicenseCustomer) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *LicenseCustomer) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


