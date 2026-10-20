# LicenseStatsActivationsByVersionInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Version** | **string** |  | 
**Counts** | **[]int32** | Number of successful activations each day, aligned on &#x60;days&#x60;. | 

## Methods

### NewLicenseStatsActivationsByVersionInner

`func NewLicenseStatsActivationsByVersionInner(version string, counts []int32, ) *LicenseStatsActivationsByVersionInner`

NewLicenseStatsActivationsByVersionInner instantiates a new LicenseStatsActivationsByVersionInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseStatsActivationsByVersionInnerWithDefaults

`func NewLicenseStatsActivationsByVersionInnerWithDefaults() *LicenseStatsActivationsByVersionInner`

NewLicenseStatsActivationsByVersionInnerWithDefaults instantiates a new LicenseStatsActivationsByVersionInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersion

`func (o *LicenseStatsActivationsByVersionInner) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *LicenseStatsActivationsByVersionInner) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *LicenseStatsActivationsByVersionInner) SetVersion(v string)`

SetVersion sets Version field to given value.


### GetCounts

`func (o *LicenseStatsActivationsByVersionInner) GetCounts() []int32`

GetCounts returns the Counts field if non-nil, zero value otherwise.

### GetCountsOk

`func (o *LicenseStatsActivationsByVersionInner) GetCountsOk() (*[]int32, bool)`

GetCountsOk returns a tuple with the Counts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCounts

`func (o *LicenseStatsActivationsByVersionInner) SetCounts(v []int32)`

SetCounts sets Counts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


