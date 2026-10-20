# CreateCustomer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** | Unique within the product, regardless of case. Stored lower cased. | 
**Name** | Pointer to **NullableString** | Display name of the customer. &#x60;null&#x60; when unknown. Defaults to &#x60;null&#x60;. | [optional] 

## Methods

### NewCreateCustomer

`func NewCreateCustomer(email string, ) *CreateCustomer`

NewCreateCustomer instantiates a new CreateCustomer object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateCustomerWithDefaults

`func NewCreateCustomerWithDefaults() *CreateCustomer`

NewCreateCustomerWithDefaults instantiates a new CreateCustomer object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *CreateCustomer) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *CreateCustomer) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *CreateCustomer) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetName

`func (o *CreateCustomer) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateCustomer) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateCustomer) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CreateCustomer) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *CreateCustomer) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *CreateCustomer) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


