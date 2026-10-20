# UpdateCustomer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | Pointer to **string** | Unique within the product, regardless of case. Stored lower cased. | [optional] 
**Name** | Pointer to **NullableString** | Display name of the customer. &#x60;null&#x60; when unknown. Defaults to &#x60;null&#x60;. | [optional] 

## Methods

### NewUpdateCustomer

`func NewUpdateCustomer() *UpdateCustomer`

NewUpdateCustomer instantiates a new UpdateCustomer object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateCustomerWithDefaults

`func NewUpdateCustomerWithDefaults() *UpdateCustomer`

NewUpdateCustomerWithDefaults instantiates a new UpdateCustomer object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *UpdateCustomer) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *UpdateCustomer) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *UpdateCustomer) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *UpdateCustomer) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetName

`func (o *UpdateCustomer) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateCustomer) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateCustomer) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateCustomer) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *UpdateCustomer) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *UpdateCustomer) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


