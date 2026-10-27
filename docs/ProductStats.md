# ProductStats

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LicenseCount** | **int32** | Number of licenses of the product. | 
**ActiveLicenseCount** | **int32** | Number of licenses that haven&#39;t expired nor were canceled, and that a machine validated in the last 90 days. | 
**NewLicenseCount** | **int32** | Number of licenses created in the last 30 days, today included, in UTC. | 
**ExpiringLicenseCount** | **int32** | Number of licenses expiring in the next 30 days, canceled ones left out. | 
**ExpiredLicenseCount** | **int32** | Number of licenses that expired in the last 30 days, canceled ones left out. | 
**ActiveMachineCount** | **int32** | Number of active machines of the licenses of the product. | 
**InUseLicenseCount** | **int32** | Number of licenses with at least one active machine. | 
**SeatCount** | **int32** | Sum of the maximum numbers of machines of the licenses that haven&#39;t expired nor were canceled. Licenses without a maximum are left out. | 
**UsedSeatCount** | **int32** | Number of active machines of the licenses counted in &#x60;seatCount&#x60;, at most their maximum number of machines each. | 
**FullLicenseCount** | **int32** | Number of licenses counted in &#x60;seatCount&#x60; active on their maximum number of machines. | 
**Days** | **[]string** | The 30 days covered by the daily stats, from the oldest one, in UTC. | 
**Months** | **[]string** | The 12 months covered by the monthly stats, from the oldest one, in UTC. | 
**NewLicensesByDay** | **[]int32** | Number of licenses created each day, aligned on &#x60;days&#x60;. | 
**NewLicensesByMonth** | **[]int32** | Number of licenses created each month, aligned on &#x60;months&#x60;. | 
**NewLicensesByPolicy** | [**[]ProductStatsNewLicensesByPolicyInner**](ProductStatsNewLicensesByPolicyInner.md) | Number of licenses of each policy created each day and each month, for the policies with licenses created over the covered months. | 
**Cancellation** | [**NullableCancellationStats**](CancellationStats.md) | Cancellations of the licenses with a money back guarantee. &#x60;null&#x60; when no license of the product has one. | 
**Subscriptions** | [**NullableSubscriptionStats**](SubscriptionStats.md) | Subscriptions of the product. &#x60;null&#x60; when it has never had one. | 
**Revenue** | [**[]Revenue**](Revenue.md) | Revenue in each currency licenses were sold in, from the one with the most licenses sold. Amounts aren&#39;t converted between currencies. | 
**ActivationsByVersion** | [**[]ProductStatsActivationsByVersionInner**](ProductStatsActivationsByVersionInner.md) | Successful activations of the licenses of the product each day, per version of the application, from the most recent one. | 
**ActiveMachinesByVersion** | [**[]ProductStatsActiveMachinesByVersionInner**](ProductStatsActiveMachinesByVersionInner.md) | Number of active machines running each version of the application, from the most recent one. | 
**ActiveMachinesByPlatform** | [**[]ProductStatsActiveMachinesByPlatformInner**](ProductStatsActiveMachinesByPlatformInner.md) | Number of active machines on each platform, from the one with the most machines. | 

## Methods

### NewProductStats

`func NewProductStats(licenseCount int32, activeLicenseCount int32, newLicenseCount int32, expiringLicenseCount int32, expiredLicenseCount int32, activeMachineCount int32, inUseLicenseCount int32, seatCount int32, usedSeatCount int32, fullLicenseCount int32, days []string, months []string, newLicensesByDay []int32, newLicensesByMonth []int32, newLicensesByPolicy []ProductStatsNewLicensesByPolicyInner, cancellation NullableCancellationStats, subscriptions NullableSubscriptionStats, revenue []Revenue, activationsByVersion []ProductStatsActivationsByVersionInner, activeMachinesByVersion []ProductStatsActiveMachinesByVersionInner, activeMachinesByPlatform []ProductStatsActiveMachinesByPlatformInner, ) *ProductStats`

NewProductStats instantiates a new ProductStats object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductStatsWithDefaults

`func NewProductStatsWithDefaults() *ProductStats`

NewProductStatsWithDefaults instantiates a new ProductStats object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLicenseCount

`func (o *ProductStats) GetLicenseCount() int32`

GetLicenseCount returns the LicenseCount field if non-nil, zero value otherwise.

### GetLicenseCountOk

`func (o *ProductStats) GetLicenseCountOk() (*int32, bool)`

GetLicenseCountOk returns a tuple with the LicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseCount

`func (o *ProductStats) SetLicenseCount(v int32)`

SetLicenseCount sets LicenseCount field to given value.


### GetActiveLicenseCount

`func (o *ProductStats) GetActiveLicenseCount() int32`

GetActiveLicenseCount returns the ActiveLicenseCount field if non-nil, zero value otherwise.

### GetActiveLicenseCountOk

`func (o *ProductStats) GetActiveLicenseCountOk() (*int32, bool)`

GetActiveLicenseCountOk returns a tuple with the ActiveLicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveLicenseCount

`func (o *ProductStats) SetActiveLicenseCount(v int32)`

SetActiveLicenseCount sets ActiveLicenseCount field to given value.


### GetNewLicenseCount

`func (o *ProductStats) GetNewLicenseCount() int32`

GetNewLicenseCount returns the NewLicenseCount field if non-nil, zero value otherwise.

### GetNewLicenseCountOk

`func (o *ProductStats) GetNewLicenseCountOk() (*int32, bool)`

GetNewLicenseCountOk returns a tuple with the NewLicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewLicenseCount

`func (o *ProductStats) SetNewLicenseCount(v int32)`

SetNewLicenseCount sets NewLicenseCount field to given value.


### GetExpiringLicenseCount

`func (o *ProductStats) GetExpiringLicenseCount() int32`

GetExpiringLicenseCount returns the ExpiringLicenseCount field if non-nil, zero value otherwise.

### GetExpiringLicenseCountOk

`func (o *ProductStats) GetExpiringLicenseCountOk() (*int32, bool)`

GetExpiringLicenseCountOk returns a tuple with the ExpiringLicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiringLicenseCount

`func (o *ProductStats) SetExpiringLicenseCount(v int32)`

SetExpiringLicenseCount sets ExpiringLicenseCount field to given value.


### GetExpiredLicenseCount

`func (o *ProductStats) GetExpiredLicenseCount() int32`

GetExpiredLicenseCount returns the ExpiredLicenseCount field if non-nil, zero value otherwise.

### GetExpiredLicenseCountOk

`func (o *ProductStats) GetExpiredLicenseCountOk() (*int32, bool)`

GetExpiredLicenseCountOk returns a tuple with the ExpiredLicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiredLicenseCount

`func (o *ProductStats) SetExpiredLicenseCount(v int32)`

SetExpiredLicenseCount sets ExpiredLicenseCount field to given value.


### GetActiveMachineCount

`func (o *ProductStats) GetActiveMachineCount() int32`

GetActiveMachineCount returns the ActiveMachineCount field if non-nil, zero value otherwise.

### GetActiveMachineCountOk

`func (o *ProductStats) GetActiveMachineCountOk() (*int32, bool)`

GetActiveMachineCountOk returns a tuple with the ActiveMachineCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveMachineCount

`func (o *ProductStats) SetActiveMachineCount(v int32)`

SetActiveMachineCount sets ActiveMachineCount field to given value.


### GetInUseLicenseCount

`func (o *ProductStats) GetInUseLicenseCount() int32`

GetInUseLicenseCount returns the InUseLicenseCount field if non-nil, zero value otherwise.

### GetInUseLicenseCountOk

`func (o *ProductStats) GetInUseLicenseCountOk() (*int32, bool)`

GetInUseLicenseCountOk returns a tuple with the InUseLicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInUseLicenseCount

`func (o *ProductStats) SetInUseLicenseCount(v int32)`

SetInUseLicenseCount sets InUseLicenseCount field to given value.


### GetSeatCount

`func (o *ProductStats) GetSeatCount() int32`

GetSeatCount returns the SeatCount field if non-nil, zero value otherwise.

### GetSeatCountOk

`func (o *ProductStats) GetSeatCountOk() (*int32, bool)`

GetSeatCountOk returns a tuple with the SeatCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeatCount

`func (o *ProductStats) SetSeatCount(v int32)`

SetSeatCount sets SeatCount field to given value.


### GetUsedSeatCount

`func (o *ProductStats) GetUsedSeatCount() int32`

GetUsedSeatCount returns the UsedSeatCount field if non-nil, zero value otherwise.

### GetUsedSeatCountOk

`func (o *ProductStats) GetUsedSeatCountOk() (*int32, bool)`

GetUsedSeatCountOk returns a tuple with the UsedSeatCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsedSeatCount

`func (o *ProductStats) SetUsedSeatCount(v int32)`

SetUsedSeatCount sets UsedSeatCount field to given value.


### GetFullLicenseCount

`func (o *ProductStats) GetFullLicenseCount() int32`

GetFullLicenseCount returns the FullLicenseCount field if non-nil, zero value otherwise.

### GetFullLicenseCountOk

`func (o *ProductStats) GetFullLicenseCountOk() (*int32, bool)`

GetFullLicenseCountOk returns a tuple with the FullLicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFullLicenseCount

`func (o *ProductStats) SetFullLicenseCount(v int32)`

SetFullLicenseCount sets FullLicenseCount field to given value.


### GetDays

`func (o *ProductStats) GetDays() []string`

GetDays returns the Days field if non-nil, zero value otherwise.

### GetDaysOk

`func (o *ProductStats) GetDaysOk() (*[]string, bool)`

GetDaysOk returns a tuple with the Days field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDays

`func (o *ProductStats) SetDays(v []string)`

SetDays sets Days field to given value.


### GetMonths

`func (o *ProductStats) GetMonths() []string`

GetMonths returns the Months field if non-nil, zero value otherwise.

### GetMonthsOk

`func (o *ProductStats) GetMonthsOk() (*[]string, bool)`

GetMonthsOk returns a tuple with the Months field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonths

`func (o *ProductStats) SetMonths(v []string)`

SetMonths sets Months field to given value.


### GetNewLicensesByDay

`func (o *ProductStats) GetNewLicensesByDay() []int32`

GetNewLicensesByDay returns the NewLicensesByDay field if non-nil, zero value otherwise.

### GetNewLicensesByDayOk

`func (o *ProductStats) GetNewLicensesByDayOk() (*[]int32, bool)`

GetNewLicensesByDayOk returns a tuple with the NewLicensesByDay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewLicensesByDay

`func (o *ProductStats) SetNewLicensesByDay(v []int32)`

SetNewLicensesByDay sets NewLicensesByDay field to given value.


### GetNewLicensesByMonth

`func (o *ProductStats) GetNewLicensesByMonth() []int32`

GetNewLicensesByMonth returns the NewLicensesByMonth field if non-nil, zero value otherwise.

### GetNewLicensesByMonthOk

`func (o *ProductStats) GetNewLicensesByMonthOk() (*[]int32, bool)`

GetNewLicensesByMonthOk returns a tuple with the NewLicensesByMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewLicensesByMonth

`func (o *ProductStats) SetNewLicensesByMonth(v []int32)`

SetNewLicensesByMonth sets NewLicensesByMonth field to given value.


### GetNewLicensesByPolicy

`func (o *ProductStats) GetNewLicensesByPolicy() []ProductStatsNewLicensesByPolicyInner`

GetNewLicensesByPolicy returns the NewLicensesByPolicy field if non-nil, zero value otherwise.

### GetNewLicensesByPolicyOk

`func (o *ProductStats) GetNewLicensesByPolicyOk() (*[]ProductStatsNewLicensesByPolicyInner, bool)`

GetNewLicensesByPolicyOk returns a tuple with the NewLicensesByPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewLicensesByPolicy

`func (o *ProductStats) SetNewLicensesByPolicy(v []ProductStatsNewLicensesByPolicyInner)`

SetNewLicensesByPolicy sets NewLicensesByPolicy field to given value.


### GetCancellation

`func (o *ProductStats) GetCancellation() CancellationStats`

GetCancellation returns the Cancellation field if non-nil, zero value otherwise.

### GetCancellationOk

`func (o *ProductStats) GetCancellationOk() (*CancellationStats, bool)`

GetCancellationOk returns a tuple with the Cancellation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancellation

`func (o *ProductStats) SetCancellation(v CancellationStats)`

SetCancellation sets Cancellation field to given value.


### SetCancellationNil

`func (o *ProductStats) SetCancellationNil(b bool)`

 SetCancellationNil sets the value for Cancellation to be an explicit nil

### UnsetCancellation
`func (o *ProductStats) UnsetCancellation()`

UnsetCancellation ensures that no value is present for Cancellation, not even an explicit nil
### GetSubscriptions

`func (o *ProductStats) GetSubscriptions() SubscriptionStats`

GetSubscriptions returns the Subscriptions field if non-nil, zero value otherwise.

### GetSubscriptionsOk

`func (o *ProductStats) GetSubscriptionsOk() (*SubscriptionStats, bool)`

GetSubscriptionsOk returns a tuple with the Subscriptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptions

`func (o *ProductStats) SetSubscriptions(v SubscriptionStats)`

SetSubscriptions sets Subscriptions field to given value.


### SetSubscriptionsNil

`func (o *ProductStats) SetSubscriptionsNil(b bool)`

 SetSubscriptionsNil sets the value for Subscriptions to be an explicit nil

### UnsetSubscriptions
`func (o *ProductStats) UnsetSubscriptions()`

UnsetSubscriptions ensures that no value is present for Subscriptions, not even an explicit nil
### GetRevenue

`func (o *ProductStats) GetRevenue() []Revenue`

GetRevenue returns the Revenue field if non-nil, zero value otherwise.

### GetRevenueOk

`func (o *ProductStats) GetRevenueOk() (*[]Revenue, bool)`

GetRevenueOk returns a tuple with the Revenue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevenue

`func (o *ProductStats) SetRevenue(v []Revenue)`

SetRevenue sets Revenue field to given value.


### GetActivationsByVersion

`func (o *ProductStats) GetActivationsByVersion() []ProductStatsActivationsByVersionInner`

GetActivationsByVersion returns the ActivationsByVersion field if non-nil, zero value otherwise.

### GetActivationsByVersionOk

`func (o *ProductStats) GetActivationsByVersionOk() (*[]ProductStatsActivationsByVersionInner, bool)`

GetActivationsByVersionOk returns a tuple with the ActivationsByVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivationsByVersion

`func (o *ProductStats) SetActivationsByVersion(v []ProductStatsActivationsByVersionInner)`

SetActivationsByVersion sets ActivationsByVersion field to given value.


### GetActiveMachinesByVersion

`func (o *ProductStats) GetActiveMachinesByVersion() []ProductStatsActiveMachinesByVersionInner`

GetActiveMachinesByVersion returns the ActiveMachinesByVersion field if non-nil, zero value otherwise.

### GetActiveMachinesByVersionOk

`func (o *ProductStats) GetActiveMachinesByVersionOk() (*[]ProductStatsActiveMachinesByVersionInner, bool)`

GetActiveMachinesByVersionOk returns a tuple with the ActiveMachinesByVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveMachinesByVersion

`func (o *ProductStats) SetActiveMachinesByVersion(v []ProductStatsActiveMachinesByVersionInner)`

SetActiveMachinesByVersion sets ActiveMachinesByVersion field to given value.


### GetActiveMachinesByPlatform

`func (o *ProductStats) GetActiveMachinesByPlatform() []ProductStatsActiveMachinesByPlatformInner`

GetActiveMachinesByPlatform returns the ActiveMachinesByPlatform field if non-nil, zero value otherwise.

### GetActiveMachinesByPlatformOk

`func (o *ProductStats) GetActiveMachinesByPlatformOk() (*[]ProductStatsActiveMachinesByPlatformInner, bool)`

GetActiveMachinesByPlatformOk returns a tuple with the ActiveMachinesByPlatform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveMachinesByPlatform

`func (o *ProductStats) SetActiveMachinesByPlatform(v []ProductStatsActiveMachinesByPlatformInner)`

SetActiveMachinesByPlatform sets ActiveMachinesByPlatform field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


