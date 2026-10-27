# Mrr

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Currency** | **string** |  | 
**Mrr** | **float32** | Monthly recurring revenue: the price of every ongoing subscription in the currency, times its quantity, brought to one month (a year counts for a twelfth), before taxes and discounts. | 
**ByInterval** | [**[]MrrByIntervalInner**](MrrByIntervalInner.md) | Ongoing subscriptions and MRR of each billing period, like monthly and yearly, from the highest MRR. | 
**ByPolicy** | [**[]MrrByPolicyInner**](MrrByPolicyInner.md) | MRR of each policy, from the highest. | 
**ByMonth** | **[]float32** | MRR at the end of each month, aligned on &#x60;months&#x60;, today for this month, at the current prices of the subscriptions. | 

## Methods

### NewMrr

`func NewMrr(currency string, mrr float32, byInterval []MrrByIntervalInner, byPolicy []MrrByPolicyInner, byMonth []float32, ) *Mrr`

NewMrr instantiates a new Mrr object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMrrWithDefaults

`func NewMrrWithDefaults() *Mrr`

NewMrrWithDefaults instantiates a new Mrr object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrency

`func (o *Mrr) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *Mrr) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *Mrr) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetMrr

`func (o *Mrr) GetMrr() float32`

GetMrr returns the Mrr field if non-nil, zero value otherwise.

### GetMrrOk

`func (o *Mrr) GetMrrOk() (*float32, bool)`

GetMrrOk returns a tuple with the Mrr field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMrr

`func (o *Mrr) SetMrr(v float32)`

SetMrr sets Mrr field to given value.


### GetByInterval

`func (o *Mrr) GetByInterval() []MrrByIntervalInner`

GetByInterval returns the ByInterval field if non-nil, zero value otherwise.

### GetByIntervalOk

`func (o *Mrr) GetByIntervalOk() (*[]MrrByIntervalInner, bool)`

GetByIntervalOk returns a tuple with the ByInterval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByInterval

`func (o *Mrr) SetByInterval(v []MrrByIntervalInner)`

SetByInterval sets ByInterval field to given value.


### GetByPolicy

`func (o *Mrr) GetByPolicy() []MrrByPolicyInner`

GetByPolicy returns the ByPolicy field if non-nil, zero value otherwise.

### GetByPolicyOk

`func (o *Mrr) GetByPolicyOk() (*[]MrrByPolicyInner, bool)`

GetByPolicyOk returns a tuple with the ByPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByPolicy

`func (o *Mrr) SetByPolicy(v []MrrByPolicyInner)`

SetByPolicy sets ByPolicy field to given value.


### GetByMonth

`func (o *Mrr) GetByMonth() []float32`

GetByMonth returns the ByMonth field if non-nil, zero value otherwise.

### GetByMonthOk

`func (o *Mrr) GetByMonthOk() (*[]float32, bool)`

GetByMonthOk returns a tuple with the ByMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByMonth

`func (o *Mrr) SetByMonth(v []float32)`

SetByMonth sets ByMonth field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


