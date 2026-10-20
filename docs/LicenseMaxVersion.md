# LicenseMaxVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Version** | **NullableString** | Hard-coded latest version, taking precedence over &#x60;lockMajorAt&#x60; and &#x60;lockMinorAt&#x60;. &#x60;\&quot;2\&quot;&#x60; allows every 2.y.z version: its minor versions and bug fixes. &#x60;\&quot;2.3\&quot;&#x60; allows every 2.3.z version: its bug fixes. &#x60;null&#x60; when it&#39;s not hard-coded. | 
**LockMajorAt** | **NullableTime** | When the major version of the license locks: it then only gets the minor versions and bug fixes of the major version released by then. Once reached, within the hour, the major version of the latest stable release by then is hard-coded in &#x60;version&#x60;, unless a version already is, and the lock is cleared. A lock reached before any stable release is cleared without hard-coding anything. &#x60;null&#x60; when it&#39;s never locked. | 
**LockMinorAt** | **NullableTime** | When the minor version of the license locks: it then only gets the bug fixes of the minor version released by then, within the hard-coded major version when there&#39;s one. Never before &#x60;lockMajorAt&#x60;; without it, the major version locks along with the minor version. Once reached, within the hour, the major and minor version of the latest stable release by then is hard-coded in &#x60;version&#x60;, unless a minor version already is, and the lock is cleared. A lock reached before any matching stable release is cleared without hard-coding anything. &#x60;null&#x60; when it&#39;s never locked. | 

## Methods

### NewLicenseMaxVersion

`func NewLicenseMaxVersion(version NullableString, lockMajorAt NullableTime, lockMinorAt NullableTime, ) *LicenseMaxVersion`

NewLicenseMaxVersion instantiates a new LicenseMaxVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseMaxVersionWithDefaults

`func NewLicenseMaxVersionWithDefaults() *LicenseMaxVersion`

NewLicenseMaxVersionWithDefaults instantiates a new LicenseMaxVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersion

`func (o *LicenseMaxVersion) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *LicenseMaxVersion) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *LicenseMaxVersion) SetVersion(v string)`

SetVersion sets Version field to given value.


### SetVersionNil

`func (o *LicenseMaxVersion) SetVersionNil(b bool)`

 SetVersionNil sets the value for Version to be an explicit nil

### UnsetVersion
`func (o *LicenseMaxVersion) UnsetVersion()`

UnsetVersion ensures that no value is present for Version, not even an explicit nil
### GetLockMajorAt

`func (o *LicenseMaxVersion) GetLockMajorAt() time.Time`

GetLockMajorAt returns the LockMajorAt field if non-nil, zero value otherwise.

### GetLockMajorAtOk

`func (o *LicenseMaxVersion) GetLockMajorAtOk() (*time.Time, bool)`

GetLockMajorAtOk returns a tuple with the LockMajorAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLockMajorAt

`func (o *LicenseMaxVersion) SetLockMajorAt(v time.Time)`

SetLockMajorAt sets LockMajorAt field to given value.


### SetLockMajorAtNil

`func (o *LicenseMaxVersion) SetLockMajorAtNil(b bool)`

 SetLockMajorAtNil sets the value for LockMajorAt to be an explicit nil

### UnsetLockMajorAt
`func (o *LicenseMaxVersion) UnsetLockMajorAt()`

UnsetLockMajorAt ensures that no value is present for LockMajorAt, not even an explicit nil
### GetLockMinorAt

`func (o *LicenseMaxVersion) GetLockMinorAt() time.Time`

GetLockMinorAt returns the LockMinorAt field if non-nil, zero value otherwise.

### GetLockMinorAtOk

`func (o *LicenseMaxVersion) GetLockMinorAtOk() (*time.Time, bool)`

GetLockMinorAtOk returns a tuple with the LockMinorAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLockMinorAt

`func (o *LicenseMaxVersion) SetLockMinorAt(v time.Time)`

SetLockMinorAt sets LockMinorAt field to given value.


### SetLockMinorAtNil

`func (o *LicenseMaxVersion) SetLockMinorAtNil(b bool)`

 SetLockMinorAtNil sets the value for LockMinorAt to be an explicit nil

### UnsetLockMinorAt
`func (o *LicenseMaxVersion) UnsetLockMinorAt()`

UnsetLockMinorAt ensures that no value is present for LockMinorAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


