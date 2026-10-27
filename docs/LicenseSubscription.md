# LicenseSubscription

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StripeSubscriptionId** | **string** |  | 
**Status** | **string** | Status of the subscription in Stripe: &#x60;active&#x60;, &#x60;trialing&#x60;, &#x60;past_due&#x60; while a failed payment is retried, &#x60;canceled&#x60;, &#x60;unpaid&#x60;, &#x60;paused&#x60;, &#x60;incomplete&#x60; or &#x60;incomplete_expired&#x60;. | 
**Interval** | **string** |  | 
**IntervalCount** | **int32** | Number of intervals between payments. | 
**Quantity** | **int32** | Units subscribed, multiplying the policy&#39;s machines. | 
**Price** | [**NullablePrice**](Price.md) | Price of one unit for one period, before taxes. | 
**CurrentPeriodEnd** | **time.Time** | End of the paid period, when the subscription renews or ends. | 
**CancelAtPeriodEnd** | **bool** | Whether the subscription ends at the end of the period. | 
**EndedAt** | **NullableTime** |  | 

## Methods

### NewLicenseSubscription

`func NewLicenseSubscription(stripeSubscriptionId string, status string, interval string, intervalCount int32, quantity int32, price NullablePrice, currentPeriodEnd time.Time, cancelAtPeriodEnd bool, endedAt NullableTime, ) *LicenseSubscription`

NewLicenseSubscription instantiates a new LicenseSubscription object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseSubscriptionWithDefaults

`func NewLicenseSubscriptionWithDefaults() *LicenseSubscription`

NewLicenseSubscriptionWithDefaults instantiates a new LicenseSubscription object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStripeSubscriptionId

`func (o *LicenseSubscription) GetStripeSubscriptionId() string`

GetStripeSubscriptionId returns the StripeSubscriptionId field if non-nil, zero value otherwise.

### GetStripeSubscriptionIdOk

`func (o *LicenseSubscription) GetStripeSubscriptionIdOk() (*string, bool)`

GetStripeSubscriptionIdOk returns a tuple with the StripeSubscriptionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripeSubscriptionId

`func (o *LicenseSubscription) SetStripeSubscriptionId(v string)`

SetStripeSubscriptionId sets StripeSubscriptionId field to given value.


### GetStatus

`func (o *LicenseSubscription) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *LicenseSubscription) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *LicenseSubscription) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetInterval

`func (o *LicenseSubscription) GetInterval() string`

GetInterval returns the Interval field if non-nil, zero value otherwise.

### GetIntervalOk

`func (o *LicenseSubscription) GetIntervalOk() (*string, bool)`

GetIntervalOk returns a tuple with the Interval field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInterval

`func (o *LicenseSubscription) SetInterval(v string)`

SetInterval sets Interval field to given value.


### GetIntervalCount

`func (o *LicenseSubscription) GetIntervalCount() int32`

GetIntervalCount returns the IntervalCount field if non-nil, zero value otherwise.

### GetIntervalCountOk

`func (o *LicenseSubscription) GetIntervalCountOk() (*int32, bool)`

GetIntervalCountOk returns a tuple with the IntervalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIntervalCount

`func (o *LicenseSubscription) SetIntervalCount(v int32)`

SetIntervalCount sets IntervalCount field to given value.


### GetQuantity

`func (o *LicenseSubscription) GetQuantity() int32`

GetQuantity returns the Quantity field if non-nil, zero value otherwise.

### GetQuantityOk

`func (o *LicenseSubscription) GetQuantityOk() (*int32, bool)`

GetQuantityOk returns a tuple with the Quantity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetQuantity

`func (o *LicenseSubscription) SetQuantity(v int32)`

SetQuantity sets Quantity field to given value.


### GetPrice

`func (o *LicenseSubscription) GetPrice() Price`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *LicenseSubscription) GetPriceOk() (*Price, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *LicenseSubscription) SetPrice(v Price)`

SetPrice sets Price field to given value.


### SetPriceNil

`func (o *LicenseSubscription) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *LicenseSubscription) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetCurrentPeriodEnd

`func (o *LicenseSubscription) GetCurrentPeriodEnd() time.Time`

GetCurrentPeriodEnd returns the CurrentPeriodEnd field if non-nil, zero value otherwise.

### GetCurrentPeriodEndOk

`func (o *LicenseSubscription) GetCurrentPeriodEndOk() (*time.Time, bool)`

GetCurrentPeriodEndOk returns a tuple with the CurrentPeriodEnd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrentPeriodEnd

`func (o *LicenseSubscription) SetCurrentPeriodEnd(v time.Time)`

SetCurrentPeriodEnd sets CurrentPeriodEnd field to given value.


### GetCancelAtPeriodEnd

`func (o *LicenseSubscription) GetCancelAtPeriodEnd() bool`

GetCancelAtPeriodEnd returns the CancelAtPeriodEnd field if non-nil, zero value otherwise.

### GetCancelAtPeriodEndOk

`func (o *LicenseSubscription) GetCancelAtPeriodEndOk() (*bool, bool)`

GetCancelAtPeriodEndOk returns a tuple with the CancelAtPeriodEnd field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancelAtPeriodEnd

`func (o *LicenseSubscription) SetCancelAtPeriodEnd(v bool)`

SetCancelAtPeriodEnd sets CancelAtPeriodEnd field to given value.


### GetEndedAt

`func (o *LicenseSubscription) GetEndedAt() time.Time`

GetEndedAt returns the EndedAt field if non-nil, zero value otherwise.

### GetEndedAtOk

`func (o *LicenseSubscription) GetEndedAtOk() (*time.Time, bool)`

GetEndedAtOk returns a tuple with the EndedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndedAt

`func (o *LicenseSubscription) SetEndedAt(v time.Time)`

SetEndedAt sets EndedAt field to given value.


### SetEndedAtNil

`func (o *LicenseSubscription) SetEndedAtNil(b bool)`

 SetEndedAtNil sets the value for EndedAt to be an explicit nil

### UnsetEndedAt
`func (o *LicenseSubscription) UnsetEndedAt()`

UnsetEndedAt ensures that no value is present for EndedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


