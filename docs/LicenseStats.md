# LicenseStats

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | **string** | First day covered, in UTC. | 
**To** | **string** | Last day covered, in UTC: today. | 
**Days** | **[]string** | The 90 days covered, from the oldest one, in UTC. | 
**ActivationsByMachine** | [**[]LicenseStatsActivationsByMachineInner**](LicenseStatsActivationsByMachineInner.md) | Machines that activated the license in the period, from the one with the most activations. | 
**ActivationsByVersion** | [**[]LicenseStatsActivationsByVersionInner**](LicenseStatsActivationsByVersionInner.md) | Versions of the application that activated the license in the period, from the most recent one. | 

## Methods

### NewLicenseStats

`func NewLicenseStats(from string, to string, days []string, activationsByMachine []LicenseStatsActivationsByMachineInner, activationsByVersion []LicenseStatsActivationsByVersionInner, ) *LicenseStats`

NewLicenseStats instantiates a new LicenseStats object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseStatsWithDefaults

`func NewLicenseStatsWithDefaults() *LicenseStats`

NewLicenseStatsWithDefaults instantiates a new LicenseStats object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrom

`func (o *LicenseStats) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *LicenseStats) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *LicenseStats) SetFrom(v string)`

SetFrom sets From field to given value.


### GetTo

`func (o *LicenseStats) GetTo() string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *LicenseStats) GetToOk() (*string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *LicenseStats) SetTo(v string)`

SetTo sets To field to given value.


### GetDays

`func (o *LicenseStats) GetDays() []string`

GetDays returns the Days field if non-nil, zero value otherwise.

### GetDaysOk

`func (o *LicenseStats) GetDaysOk() (*[]string, bool)`

GetDaysOk returns a tuple with the Days field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDays

`func (o *LicenseStats) SetDays(v []string)`

SetDays sets Days field to given value.


### GetActivationsByMachine

`func (o *LicenseStats) GetActivationsByMachine() []LicenseStatsActivationsByMachineInner`

GetActivationsByMachine returns the ActivationsByMachine field if non-nil, zero value otherwise.

### GetActivationsByMachineOk

`func (o *LicenseStats) GetActivationsByMachineOk() (*[]LicenseStatsActivationsByMachineInner, bool)`

GetActivationsByMachineOk returns a tuple with the ActivationsByMachine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivationsByMachine

`func (o *LicenseStats) SetActivationsByMachine(v []LicenseStatsActivationsByMachineInner)`

SetActivationsByMachine sets ActivationsByMachine field to given value.


### GetActivationsByVersion

`func (o *LicenseStats) GetActivationsByVersion() []LicenseStatsActivationsByVersionInner`

GetActivationsByVersion returns the ActivationsByVersion field if non-nil, zero value otherwise.

### GetActivationsByVersionOk

`func (o *LicenseStats) GetActivationsByVersionOk() (*[]LicenseStatsActivationsByVersionInner, bool)`

GetActivationsByVersionOk returns a tuple with the ActivationsByVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActivationsByVersion

`func (o *LicenseStats) SetActivationsByVersion(v []LicenseStatsActivationsByVersionInner)`

SetActivationsByVersion sets ActivationsByVersion field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


