# LicenseStatsActivationsByMachineInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MachineId** | **string** |  | 
**Name** | **NullableString** |  | 
**Fingerprint** | **string** |  | 
**Counts** | **[]int32** | Number of successful activations each day, aligned on &#x60;days&#x60;. | 

## Methods

### NewLicenseStatsActivationsByMachineInner

`func NewLicenseStatsActivationsByMachineInner(machineId string, name NullableString, fingerprint string, counts []int32, ) *LicenseStatsActivationsByMachineInner`

NewLicenseStatsActivationsByMachineInner instantiates a new LicenseStatsActivationsByMachineInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseStatsActivationsByMachineInnerWithDefaults

`func NewLicenseStatsActivationsByMachineInnerWithDefaults() *LicenseStatsActivationsByMachineInner`

NewLicenseStatsActivationsByMachineInnerWithDefaults instantiates a new LicenseStatsActivationsByMachineInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMachineId

`func (o *LicenseStatsActivationsByMachineInner) GetMachineId() string`

GetMachineId returns the MachineId field if non-nil, zero value otherwise.

### GetMachineIdOk

`func (o *LicenseStatsActivationsByMachineInner) GetMachineIdOk() (*string, bool)`

GetMachineIdOk returns a tuple with the MachineId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMachineId

`func (o *LicenseStatsActivationsByMachineInner) SetMachineId(v string)`

SetMachineId sets MachineId field to given value.


### GetName

`func (o *LicenseStatsActivationsByMachineInner) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *LicenseStatsActivationsByMachineInner) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *LicenseStatsActivationsByMachineInner) SetName(v string)`

SetName sets Name field to given value.


### SetNameNil

`func (o *LicenseStatsActivationsByMachineInner) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *LicenseStatsActivationsByMachineInner) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetFingerprint

`func (o *LicenseStatsActivationsByMachineInner) GetFingerprint() string`

GetFingerprint returns the Fingerprint field if non-nil, zero value otherwise.

### GetFingerprintOk

`func (o *LicenseStatsActivationsByMachineInner) GetFingerprintOk() (*string, bool)`

GetFingerprintOk returns a tuple with the Fingerprint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFingerprint

`func (o *LicenseStatsActivationsByMachineInner) SetFingerprint(v string)`

SetFingerprint sets Fingerprint field to given value.


### GetCounts

`func (o *LicenseStatsActivationsByMachineInner) GetCounts() []int32`

GetCounts returns the Counts field if non-nil, zero value otherwise.

### GetCountsOk

`func (o *LicenseStatsActivationsByMachineInner) GetCountsOk() (*[]int32, bool)`

GetCountsOk returns a tuple with the Counts field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCounts

`func (o *LicenseStatsActivationsByMachineInner) SetCounts(v []int32)`

SetCounts sets Counts field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


