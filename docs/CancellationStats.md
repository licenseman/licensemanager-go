# CancellationStats

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**LicenseCount** | **int32** | Number of licenses with a money back guarantee: a &#x60;cancellableUntil&#x60;. | 
**CanceledLicenseCount** | **int32** | Number of them that were canceled. | 
**CancellableLicenseCount** | **int32** | Number of them whose money back guarantee hasn&#39;t ended, and that weren&#39;t canceled: they can still be. | 
**Rate** | **float32** | Share of them that were canceled, from 0 to 1: &#x60;canceledLicenseCount&#x60; over &#x60;licenseCount&#x60;. | 
**CanceledByDay** | **[]int32** | Number of them canceled each day, aligned on &#x60;days&#x60;, on the day of their cancellation. | 
**CanceledByMonth** | **[]int32** | Number of them canceled each month, aligned on &#x60;months&#x60;, on the month of their cancellation. | 
**ByReason** | [**[]CancellationStatsByReasonInner**](CancellationStatsByReasonInner.md) | Number of them canceled for each reason, from the most given one. Reasons never given are left out. | 

## Methods

### NewCancellationStats

`func NewCancellationStats(licenseCount int32, canceledLicenseCount int32, cancellableLicenseCount int32, rate float32, canceledByDay []int32, canceledByMonth []int32, byReason []CancellationStatsByReasonInner, ) *CancellationStats`

NewCancellationStats instantiates a new CancellationStats object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCancellationStatsWithDefaults

`func NewCancellationStatsWithDefaults() *CancellationStats`

NewCancellationStatsWithDefaults instantiates a new CancellationStats object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetLicenseCount

`func (o *CancellationStats) GetLicenseCount() int32`

GetLicenseCount returns the LicenseCount field if non-nil, zero value otherwise.

### GetLicenseCountOk

`func (o *CancellationStats) GetLicenseCountOk() (*int32, bool)`

GetLicenseCountOk returns a tuple with the LicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseCount

`func (o *CancellationStats) SetLicenseCount(v int32)`

SetLicenseCount sets LicenseCount field to given value.


### GetCanceledLicenseCount

`func (o *CancellationStats) GetCanceledLicenseCount() int32`

GetCanceledLicenseCount returns the CanceledLicenseCount field if non-nil, zero value otherwise.

### GetCanceledLicenseCountOk

`func (o *CancellationStats) GetCanceledLicenseCountOk() (*int32, bool)`

GetCanceledLicenseCountOk returns a tuple with the CanceledLicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanceledLicenseCount

`func (o *CancellationStats) SetCanceledLicenseCount(v int32)`

SetCanceledLicenseCount sets CanceledLicenseCount field to given value.


### GetCancellableLicenseCount

`func (o *CancellationStats) GetCancellableLicenseCount() int32`

GetCancellableLicenseCount returns the CancellableLicenseCount field if non-nil, zero value otherwise.

### GetCancellableLicenseCountOk

`func (o *CancellationStats) GetCancellableLicenseCountOk() (*int32, bool)`

GetCancellableLicenseCountOk returns a tuple with the CancellableLicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancellableLicenseCount

`func (o *CancellationStats) SetCancellableLicenseCount(v int32)`

SetCancellableLicenseCount sets CancellableLicenseCount field to given value.


### GetRate

`func (o *CancellationStats) GetRate() float32`

GetRate returns the Rate field if non-nil, zero value otherwise.

### GetRateOk

`func (o *CancellationStats) GetRateOk() (*float32, bool)`

GetRateOk returns a tuple with the Rate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRate

`func (o *CancellationStats) SetRate(v float32)`

SetRate sets Rate field to given value.


### GetCanceledByDay

`func (o *CancellationStats) GetCanceledByDay() []int32`

GetCanceledByDay returns the CanceledByDay field if non-nil, zero value otherwise.

### GetCanceledByDayOk

`func (o *CancellationStats) GetCanceledByDayOk() (*[]int32, bool)`

GetCanceledByDayOk returns a tuple with the CanceledByDay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanceledByDay

`func (o *CancellationStats) SetCanceledByDay(v []int32)`

SetCanceledByDay sets CanceledByDay field to given value.


### GetCanceledByMonth

`func (o *CancellationStats) GetCanceledByMonth() []int32`

GetCanceledByMonth returns the CanceledByMonth field if non-nil, zero value otherwise.

### GetCanceledByMonthOk

`func (o *CancellationStats) GetCanceledByMonthOk() (*[]int32, bool)`

GetCanceledByMonthOk returns a tuple with the CanceledByMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanceledByMonth

`func (o *CancellationStats) SetCanceledByMonth(v []int32)`

SetCanceledByMonth sets CanceledByMonth field to given value.


### GetByReason

`func (o *CancellationStats) GetByReason() []CancellationStatsByReasonInner`

GetByReason returns the ByReason field if non-nil, zero value otherwise.

### GetByReasonOk

`func (o *CancellationStats) GetByReasonOk() (*[]CancellationStatsByReasonInner, bool)`

GetByReasonOk returns a tuple with the ByReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByReason

`func (o *CancellationStats) SetByReason(v []CancellationStatsByReasonInner)`

SetByReason sets ByReason field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


