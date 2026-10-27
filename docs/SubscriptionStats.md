# SubscriptionStats

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ActiveCount** | **int32** | Number of ongoing subscriptions: &#x60;active&#x60;, &#x60;trialing&#x60; or &#x60;past_due&#x60;. | 
**TrialingCount** | **int32** |  | 
**PastDueCount** | **int32** | Number of them whose renewal failed, as Stripe retries it: their licenses stay valid for the integration&#39;s grace days. | 
**CancelingCount** | **int32** | Number of them set to end at the end of their period. | 
**NewCount** | **int32** | Number of subscriptions started in the last 30 days. | 
**EndedCount** | **int32** | Number of subscriptions that ended in the last 30 days. | 
**ChurnRate** | **float32** | Share of the subscriptions ongoing 30 days ago that ended since, from 0 to 1. | 
**NewByMonth** | **[]int32** | Number of subscriptions started each month, aligned on &#x60;months&#x60;. | 
**EndedByMonth** | **[]int32** | Number of subscriptions that ended each month, aligned on &#x60;months&#x60;. | 
**ActiveByMonth** | **[]int32** | Number of ongoing subscriptions at the end of each month, aligned on &#x60;months&#x60;, today for this month. | 
**Mrr** | [**[]Mrr**](Mrr.md) | MRR in each currency, from the highest number of subscriptions. Amounts aren&#39;t converted between currencies. | 

## Methods

### NewSubscriptionStats

`func NewSubscriptionStats(activeCount int32, trialingCount int32, pastDueCount int32, cancelingCount int32, newCount int32, endedCount int32, churnRate float32, newByMonth []int32, endedByMonth []int32, activeByMonth []int32, mrr []Mrr, ) *SubscriptionStats`

NewSubscriptionStats instantiates a new SubscriptionStats object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSubscriptionStatsWithDefaults

`func NewSubscriptionStatsWithDefaults() *SubscriptionStats`

NewSubscriptionStatsWithDefaults instantiates a new SubscriptionStats object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActiveCount

`func (o *SubscriptionStats) GetActiveCount() int32`

GetActiveCount returns the ActiveCount field if non-nil, zero value otherwise.

### GetActiveCountOk

`func (o *SubscriptionStats) GetActiveCountOk() (*int32, bool)`

GetActiveCountOk returns a tuple with the ActiveCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveCount

`func (o *SubscriptionStats) SetActiveCount(v int32)`

SetActiveCount sets ActiveCount field to given value.


### GetTrialingCount

`func (o *SubscriptionStats) GetTrialingCount() int32`

GetTrialingCount returns the TrialingCount field if non-nil, zero value otherwise.

### GetTrialingCountOk

`func (o *SubscriptionStats) GetTrialingCountOk() (*int32, bool)`

GetTrialingCountOk returns a tuple with the TrialingCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrialingCount

`func (o *SubscriptionStats) SetTrialingCount(v int32)`

SetTrialingCount sets TrialingCount field to given value.


### GetPastDueCount

`func (o *SubscriptionStats) GetPastDueCount() int32`

GetPastDueCount returns the PastDueCount field if non-nil, zero value otherwise.

### GetPastDueCountOk

`func (o *SubscriptionStats) GetPastDueCountOk() (*int32, bool)`

GetPastDueCountOk returns a tuple with the PastDueCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPastDueCount

`func (o *SubscriptionStats) SetPastDueCount(v int32)`

SetPastDueCount sets PastDueCount field to given value.


### GetCancelingCount

`func (o *SubscriptionStats) GetCancelingCount() int32`

GetCancelingCount returns the CancelingCount field if non-nil, zero value otherwise.

### GetCancelingCountOk

`func (o *SubscriptionStats) GetCancelingCountOk() (*int32, bool)`

GetCancelingCountOk returns a tuple with the CancelingCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelingCount

`func (o *SubscriptionStats) SetCancelingCount(v int32)`

SetCancelingCount sets CancelingCount field to given value.


### GetNewCount

`func (o *SubscriptionStats) GetNewCount() int32`

GetNewCount returns the NewCount field if non-nil, zero value otherwise.

### GetNewCountOk

`func (o *SubscriptionStats) GetNewCountOk() (*int32, bool)`

GetNewCountOk returns a tuple with the NewCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewCount

`func (o *SubscriptionStats) SetNewCount(v int32)`

SetNewCount sets NewCount field to given value.


### GetEndedCount

`func (o *SubscriptionStats) GetEndedCount() int32`

GetEndedCount returns the EndedCount field if non-nil, zero value otherwise.

### GetEndedCountOk

`func (o *SubscriptionStats) GetEndedCountOk() (*int32, bool)`

GetEndedCountOk returns a tuple with the EndedCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndedCount

`func (o *SubscriptionStats) SetEndedCount(v int32)`

SetEndedCount sets EndedCount field to given value.


### GetChurnRate

`func (o *SubscriptionStats) GetChurnRate() float32`

GetChurnRate returns the ChurnRate field if non-nil, zero value otherwise.

### GetChurnRateOk

`func (o *SubscriptionStats) GetChurnRateOk() (*float32, bool)`

GetChurnRateOk returns a tuple with the ChurnRate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChurnRate

`func (o *SubscriptionStats) SetChurnRate(v float32)`

SetChurnRate sets ChurnRate field to given value.


### GetNewByMonth

`func (o *SubscriptionStats) GetNewByMonth() []int32`

GetNewByMonth returns the NewByMonth field if non-nil, zero value otherwise.

### GetNewByMonthOk

`func (o *SubscriptionStats) GetNewByMonthOk() (*[]int32, bool)`

GetNewByMonthOk returns a tuple with the NewByMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewByMonth

`func (o *SubscriptionStats) SetNewByMonth(v []int32)`

SetNewByMonth sets NewByMonth field to given value.


### GetEndedByMonth

`func (o *SubscriptionStats) GetEndedByMonth() []int32`

GetEndedByMonth returns the EndedByMonth field if non-nil, zero value otherwise.

### GetEndedByMonthOk

`func (o *SubscriptionStats) GetEndedByMonthOk() (*[]int32, bool)`

GetEndedByMonthOk returns a tuple with the EndedByMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndedByMonth

`func (o *SubscriptionStats) SetEndedByMonth(v []int32)`

SetEndedByMonth sets EndedByMonth field to given value.


### GetActiveByMonth

`func (o *SubscriptionStats) GetActiveByMonth() []int32`

GetActiveByMonth returns the ActiveByMonth field if non-nil, zero value otherwise.

### GetActiveByMonthOk

`func (o *SubscriptionStats) GetActiveByMonthOk() (*[]int32, bool)`

GetActiveByMonthOk returns a tuple with the ActiveByMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveByMonth

`func (o *SubscriptionStats) SetActiveByMonth(v []int32)`

SetActiveByMonth sets ActiveByMonth field to given value.


### GetMrr

`func (o *SubscriptionStats) GetMrr() []Mrr`

GetMrr returns the Mrr field if non-nil, zero value otherwise.

### GetMrrOk

`func (o *SubscriptionStats) GetMrrOk() (*[]Mrr, bool)`

GetMrrOk returns a tuple with the Mrr field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMrr

`func (o *SubscriptionStats) SetMrr(v []Mrr)`

SetMrr sets Mrr field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


