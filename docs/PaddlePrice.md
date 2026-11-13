# PaddlePrice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ProductId** | **string** |  | 
**ProductName** | **string** |  | 
**Description** | **NullableString** | Name or internal description of the price in Paddle. | 
**Price** | [**NullablePrice**](Price.md) |  | 
**Recurring** | [**NullableStripePriceRecurring**](StripePriceRecurring.md) |  | 
**Mapped** | **bool** | Whether the price already creates licenses of a product. | 

## Methods

### NewPaddlePrice

`func NewPaddlePrice(id string, productId string, productName string, description NullableString, price NullablePrice, recurring NullableStripePriceRecurring, mapped bool, ) *PaddlePrice`

NewPaddlePrice instantiates a new PaddlePrice object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaddlePriceWithDefaults

`func NewPaddlePriceWithDefaults() *PaddlePrice`

NewPaddlePriceWithDefaults instantiates a new PaddlePrice object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *PaddlePrice) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PaddlePrice) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PaddlePrice) SetId(v string)`

SetId sets Id field to given value.


### GetProductId

`func (o *PaddlePrice) GetProductId() string`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *PaddlePrice) GetProductIdOk() (*string, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *PaddlePrice) SetProductId(v string)`

SetProductId sets ProductId field to given value.


### GetProductName

`func (o *PaddlePrice) GetProductName() string`

GetProductName returns the ProductName field if non-nil, zero value otherwise.

### GetProductNameOk

`func (o *PaddlePrice) GetProductNameOk() (*string, bool)`

GetProductNameOk returns a tuple with the ProductName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductName

`func (o *PaddlePrice) SetProductName(v string)`

SetProductName sets ProductName field to given value.


### GetDescription

`func (o *PaddlePrice) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PaddlePrice) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PaddlePrice) SetDescription(v string)`

SetDescription sets Description field to given value.


### SetDescriptionNil

`func (o *PaddlePrice) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *PaddlePrice) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetPrice

`func (o *PaddlePrice) GetPrice() Price`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *PaddlePrice) GetPriceOk() (*Price, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *PaddlePrice) SetPrice(v Price)`

SetPrice sets Price field to given value.


### SetPriceNil

`func (o *PaddlePrice) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *PaddlePrice) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetRecurring

`func (o *PaddlePrice) GetRecurring() StripePriceRecurring`

GetRecurring returns the Recurring field if non-nil, zero value otherwise.

### GetRecurringOk

`func (o *PaddlePrice) GetRecurringOk() (*StripePriceRecurring, bool)`

GetRecurringOk returns a tuple with the Recurring field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRecurring

`func (o *PaddlePrice) SetRecurring(v StripePriceRecurring)`

SetRecurring sets Recurring field to given value.


### SetRecurringNil

`func (o *PaddlePrice) SetRecurringNil(b bool)`

 SetRecurringNil sets the value for Recurring to be an explicit nil

### UnsetRecurring
`func (o *PaddlePrice) UnsetRecurring()`

UnsetRecurring ensures that no value is present for Recurring, not even an explicit nil
### GetMapped

`func (o *PaddlePrice) GetMapped() bool`

GetMapped returns the Mapped field if non-nil, zero value otherwise.

### GetMappedOk

`func (o *PaddlePrice) GetMappedOk() (*bool, bool)`

GetMappedOk returns a tuple with the Mapped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapped

`func (o *PaddlePrice) SetMapped(v bool)`

SetMapped sets Mapped field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


