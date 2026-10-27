# StripePrice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ProductId** | **string** |  | 
**ProductName** | **string** |  | 
**Nickname** | **NullableString** |  | 
**Price** | [**NullablePrice**](Price.md) |  | 
**Recurring** | [**NullableStripePriceRecurring**](StripePriceRecurring.md) |  | 
**Mapped** | **bool** | Whether the price already creates licenses of a product. | 

## Methods

### NewStripePrice

`func NewStripePrice(id string, productId string, productName string, nickname NullableString, price NullablePrice, recurring NullableStripePriceRecurring, mapped bool, ) *StripePrice`

NewStripePrice instantiates a new StripePrice object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStripePriceWithDefaults

`func NewStripePriceWithDefaults() *StripePrice`

NewStripePriceWithDefaults instantiates a new StripePrice object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *StripePrice) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *StripePrice) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *StripePrice) SetId(v string)`

SetId sets Id field to given value.


### GetProductId

`func (o *StripePrice) GetProductId() string`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *StripePrice) GetProductIdOk() (*string, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *StripePrice) SetProductId(v string)`

SetProductId sets ProductId field to given value.


### GetProductName

`func (o *StripePrice) GetProductName() string`

GetProductName returns the ProductName field if non-nil, zero value otherwise.

### GetProductNameOk

`func (o *StripePrice) GetProductNameOk() (*string, bool)`

GetProductNameOk returns a tuple with the ProductName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductName

`func (o *StripePrice) SetProductName(v string)`

SetProductName sets ProductName field to given value.


### GetNickname

`func (o *StripePrice) GetNickname() string`

GetNickname returns the Nickname field if non-nil, zero value otherwise.

### GetNicknameOk

`func (o *StripePrice) GetNicknameOk() (*string, bool)`

GetNicknameOk returns a tuple with the Nickname field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNickname

`func (o *StripePrice) SetNickname(v string)`

SetNickname sets Nickname field to given value.


### SetNicknameNil

`func (o *StripePrice) SetNicknameNil(b bool)`

 SetNicknameNil sets the value for Nickname to be an explicit nil

### UnsetNickname
`func (o *StripePrice) UnsetNickname()`

UnsetNickname ensures that no value is present for Nickname, not even an explicit nil
### GetPrice

`func (o *StripePrice) GetPrice() Price`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *StripePrice) GetPriceOk() (*Price, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *StripePrice) SetPrice(v Price)`

SetPrice sets Price field to given value.


### SetPriceNil

`func (o *StripePrice) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *StripePrice) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetRecurring

`func (o *StripePrice) GetRecurring() StripePriceRecurring`

GetRecurring returns the Recurring field if non-nil, zero value otherwise.

### GetRecurringOk

`func (o *StripePrice) GetRecurringOk() (*StripePriceRecurring, bool)`

GetRecurringOk returns a tuple with the Recurring field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecurring

`func (o *StripePrice) SetRecurring(v StripePriceRecurring)`

SetRecurring sets Recurring field to given value.


### SetRecurringNil

`func (o *StripePrice) SetRecurringNil(b bool)`

 SetRecurringNil sets the value for Recurring to be an explicit nil

### UnsetRecurring
`func (o *StripePrice) UnsetRecurring()`

UnsetRecurring ensures that no value is present for Recurring, not even an explicit nil
### GetMapped

`func (o *StripePrice) GetMapped() bool`

GetMapped returns the Mapped field if non-nil, zero value otherwise.

### GetMappedOk

`func (o *StripePrice) GetMappedOk() (*bool, bool)`

GetMappedOk returns a tuple with the Mapped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapped

`func (o *StripePrice) SetMapped(v bool)`

SetMapped sets Mapped field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


