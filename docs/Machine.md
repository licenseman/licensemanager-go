# Machine

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**LicenseId** | **string** |  | 
**Fingerprint** | **string** | Identifies the machine. Unique within the license. | 
**Platform** | **NullableString** |  | 
**Name** | **NullableString** |  | 
**Status** | **string** | Whether the machine counts as using the license. | 
**Version** | **NullableString** | Version of the application last validated on the machine. | 
**LastValidatedAt** | **NullableTime** | When the license was last validated on the machine. | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewMachine

`func NewMachine(id string, licenseId string, fingerprint string, platform NullableString, name NullableString, status string, version NullableString, lastValidatedAt NullableTime, createdAt time.Time, updatedAt time.Time, ) *Machine`

NewMachine instantiates a new Machine object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMachineWithDefaults

`func NewMachineWithDefaults() *Machine`

NewMachineWithDefaults instantiates a new Machine object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Machine) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Machine) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Machine) SetId(v string)`

SetId sets Id field to given value.


### GetLicenseId

`func (o *Machine) GetLicenseId() string`

GetLicenseId returns the LicenseId field if non-nil, zero value otherwise.

### GetLicenseIdOk

`func (o *Machine) GetLicenseIdOk() (*string, bool)`

GetLicenseIdOk returns a tuple with the LicenseId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseId

`func (o *Machine) SetLicenseId(v string)`

SetLicenseId sets LicenseId field to given value.


### GetFingerprint

`func (o *Machine) GetFingerprint() string`

GetFingerprint returns the Fingerprint field if non-nil, zero value otherwise.

### GetFingerprintOk

`func (o *Machine) GetFingerprintOk() (*string, bool)`

GetFingerprintOk returns a tuple with the Fingerprint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFingerprint

`func (o *Machine) SetFingerprint(v string)`

SetFingerprint sets Fingerprint field to given value.


### GetPlatform

`func (o *Machine) GetPlatform() string`

GetPlatform returns the Platform field if non-nil, zero value otherwise.

### GetPlatformOk

`func (o *Machine) GetPlatformOk() (*string, bool)`

GetPlatformOk returns a tuple with the Platform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlatform

`func (o *Machine) SetPlatform(v string)`

SetPlatform sets Platform field to given value.


### SetPlatformNil

`func (o *Machine) SetPlatformNil(b bool)`

 SetPlatformNil sets the value for Platform to be an explicit nil

### UnsetPlatform
`func (o *Machine) UnsetPlatform()`

UnsetPlatform ensures that no value is present for Platform, not even an explicit nil
### GetName

`func (o *Machine) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Machine) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Machine) SetName(v string)`

SetName sets Name field to given value.


### SetNameNil

`func (o *Machine) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *Machine) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetStatus

`func (o *Machine) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Machine) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Machine) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetVersion

`func (o *Machine) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *Machine) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *Machine) SetVersion(v string)`

SetVersion sets Version field to given value.


### SetVersionNil

`func (o *Machine) SetVersionNil(b bool)`

 SetVersionNil sets the value for Version to be an explicit nil

### UnsetVersion
`func (o *Machine) UnsetVersion()`

UnsetVersion ensures that no value is present for Version, not even an explicit nil
### GetLastValidatedAt

`func (o *Machine) GetLastValidatedAt() time.Time`

GetLastValidatedAt returns the LastValidatedAt field if non-nil, zero value otherwise.

### GetLastValidatedAtOk

`func (o *Machine) GetLastValidatedAtOk() (*time.Time, bool)`

GetLastValidatedAtOk returns a tuple with the LastValidatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastValidatedAt

`func (o *Machine) SetLastValidatedAt(v time.Time)`

SetLastValidatedAt sets LastValidatedAt field to given value.


### SetLastValidatedAtNil

`func (o *Machine) SetLastValidatedAtNil(b bool)`

 SetLastValidatedAtNil sets the value for LastValidatedAt to be an explicit nil

### UnsetLastValidatedAt
`func (o *Machine) UnsetLastValidatedAt()`

UnsetLastValidatedAt ensures that no value is present for LastValidatedAt, not even an explicit nil
### GetCreatedAt

`func (o *Machine) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Machine) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Machine) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *Machine) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *Machine) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *Machine) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


