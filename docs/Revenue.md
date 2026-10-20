# Revenue

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Currency** | **string** | ISO 4217 code of the currency of the revenue. | 
**LicenseCount** | **int32** | Number of licenses sold in the currency, free ones included. | 
**Total** | **float32** | Sum of the prices of the licenses sold in the currency, in major units. | 
**ThisMonth** | **float32** | Revenue of the current month, in UTC. | 
**LastMonth** | **float32** | Revenue of the previous month, in UTC. | 
**Last30Days** | **float32** | Revenue of the last 30 days, today included, in UTC. | 
**ByDay** | **[]float32** | Revenue each day, aligned on &#x60;days&#x60;. | 
**ByMonth** | **[]float32** | Revenue each month, aligned on &#x60;months&#x60;. | 
**ByPolicy** | [**[]ProductStatsNewLicensesByPolicyInner**](ProductStatsNewLicensesByPolicyInner.md) | Revenue of the licenses of each policy, for the policies with licenses sold in the currency over the covered months. | 

## Methods

### NewRevenue

`func NewRevenue(currency string, licenseCount int32, total float32, thisMonth float32, lastMonth float32, last30Days float32, byDay []float32, byMonth []float32, byPolicy []ProductStatsNewLicensesByPolicyInner, ) *Revenue`

NewRevenue instantiates a new Revenue object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRevenueWithDefaults

`func NewRevenueWithDefaults() *Revenue`

NewRevenueWithDefaults instantiates a new Revenue object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCurrency

`func (o *Revenue) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *Revenue) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *Revenue) SetCurrency(v string)`

SetCurrency sets Currency field to given value.


### GetLicenseCount

`func (o *Revenue) GetLicenseCount() int32`

GetLicenseCount returns the LicenseCount field if non-nil, zero value otherwise.

### GetLicenseCountOk

`func (o *Revenue) GetLicenseCountOk() (*int32, bool)`

GetLicenseCountOk returns a tuple with the LicenseCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseCount

`func (o *Revenue) SetLicenseCount(v int32)`

SetLicenseCount sets LicenseCount field to given value.


### GetTotal

`func (o *Revenue) GetTotal() float32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *Revenue) GetTotalOk() (*float32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *Revenue) SetTotal(v float32)`

SetTotal sets Total field to given value.


### GetThisMonth

`func (o *Revenue) GetThisMonth() float32`

GetThisMonth returns the ThisMonth field if non-nil, zero value otherwise.

### GetThisMonthOk

`func (o *Revenue) GetThisMonthOk() (*float32, bool)`

GetThisMonthOk returns a tuple with the ThisMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThisMonth

`func (o *Revenue) SetThisMonth(v float32)`

SetThisMonth sets ThisMonth field to given value.


### GetLastMonth

`func (o *Revenue) GetLastMonth() float32`

GetLastMonth returns the LastMonth field if non-nil, zero value otherwise.

### GetLastMonthOk

`func (o *Revenue) GetLastMonthOk() (*float32, bool)`

GetLastMonthOk returns a tuple with the LastMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastMonth

`func (o *Revenue) SetLastMonth(v float32)`

SetLastMonth sets LastMonth field to given value.


### GetLast30Days

`func (o *Revenue) GetLast30Days() float32`

GetLast30Days returns the Last30Days field if non-nil, zero value otherwise.

### GetLast30DaysOk

`func (o *Revenue) GetLast30DaysOk() (*float32, bool)`

GetLast30DaysOk returns a tuple with the Last30Days field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLast30Days

`func (o *Revenue) SetLast30Days(v float32)`

SetLast30Days sets Last30Days field to given value.


### GetByDay

`func (o *Revenue) GetByDay() []float32`

GetByDay returns the ByDay field if non-nil, zero value otherwise.

### GetByDayOk

`func (o *Revenue) GetByDayOk() (*[]float32, bool)`

GetByDayOk returns a tuple with the ByDay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByDay

`func (o *Revenue) SetByDay(v []float32)`

SetByDay sets ByDay field to given value.


### GetByMonth

`func (o *Revenue) GetByMonth() []float32`

GetByMonth returns the ByMonth field if non-nil, zero value otherwise.

### GetByMonthOk

`func (o *Revenue) GetByMonthOk() (*[]float32, bool)`

GetByMonthOk returns a tuple with the ByMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByMonth

`func (o *Revenue) SetByMonth(v []float32)`

SetByMonth sets ByMonth field to given value.


### GetByPolicy

`func (o *Revenue) GetByPolicy() []ProductStatsNewLicensesByPolicyInner`

GetByPolicy returns the ByPolicy field if non-nil, zero value otherwise.

### GetByPolicyOk

`func (o *Revenue) GetByPolicyOk() (*[]ProductStatsNewLicensesByPolicyInner, bool)`

GetByPolicyOk returns a tuple with the ByPolicy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByPolicy

`func (o *Revenue) SetByPolicy(v []ProductStatsNewLicensesByPolicyInner)`

SetByPolicy sets ByPolicy field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


