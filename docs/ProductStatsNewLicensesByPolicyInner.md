# ProductStatsNewLicensesByPolicyInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**PolicyId** | **string** |  | 
**ByDay** | **[]float32** | Value each day, aligned on &#x60;days&#x60;. | 
**ByMonth** | **[]float32** | Value each month, aligned on &#x60;months&#x60;. | 

## Methods

### NewProductStatsNewLicensesByPolicyInner

`func NewProductStatsNewLicensesByPolicyInner(policyId string, byDay []float32, byMonth []float32, ) *ProductStatsNewLicensesByPolicyInner`

NewProductStatsNewLicensesByPolicyInner instantiates a new ProductStatsNewLicensesByPolicyInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProductStatsNewLicensesByPolicyInnerWithDefaults

`func NewProductStatsNewLicensesByPolicyInnerWithDefaults() *ProductStatsNewLicensesByPolicyInner`

NewProductStatsNewLicensesByPolicyInnerWithDefaults instantiates a new ProductStatsNewLicensesByPolicyInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetPolicyId

`func (o *ProductStatsNewLicensesByPolicyInner) GetPolicyId() string`

GetPolicyId returns the PolicyId field if non-nil, zero value otherwise.

### GetPolicyIdOk

`func (o *ProductStatsNewLicensesByPolicyInner) GetPolicyIdOk() (*string, bool)`

GetPolicyIdOk returns a tuple with the PolicyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyId

`func (o *ProductStatsNewLicensesByPolicyInner) SetPolicyId(v string)`

SetPolicyId sets PolicyId field to given value.


### GetByDay

`func (o *ProductStatsNewLicensesByPolicyInner) GetByDay() []float32`

GetByDay returns the ByDay field if non-nil, zero value otherwise.

### GetByDayOk

`func (o *ProductStatsNewLicensesByPolicyInner) GetByDayOk() (*[]float32, bool)`

GetByDayOk returns a tuple with the ByDay field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByDay

`func (o *ProductStatsNewLicensesByPolicyInner) SetByDay(v []float32)`

SetByDay sets ByDay field to given value.


### GetByMonth

`func (o *ProductStatsNewLicensesByPolicyInner) GetByMonth() []float32`

GetByMonth returns the ByMonth field if non-nil, zero value otherwise.

### GetByMonthOk

`func (o *ProductStatsNewLicensesByPolicyInner) GetByMonthOk() (*[]float32, bool)`

GetByMonthOk returns a tuple with the ByMonth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetByMonth

`func (o *ProductStatsNewLicensesByPolicyInner) SetByMonth(v []float32)`

SetByMonth sets ByMonth field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


