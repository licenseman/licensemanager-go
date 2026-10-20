# PolicySettingsMaxVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Version** | **string** | &#x60;\&quot;2\&quot;&#x60; allows every 2.y.z version: the minor versions and bug fixes of version 2. &#x60;\&quot;2.3\&quot;&#x60; allows every 2.3.z version: the bug fixes of version 2.3. Bug fixes can&#39;t be locked, so patch numbers like &#x60;\&quot;2.3.1\&quot;&#x60; are rejected. | 
**MajorAfter** | [**LockMaxVersionMajorAfter**](LockMaxVersionMajorAfter.md) |  | 
**MinorAfter** | [**NullableLockMaxVersionMinorAfter**](LockMaxVersionMinorAfter.md) |  | 

## Methods

### NewPolicySettingsMaxVersion

`func NewPolicySettingsMaxVersion(type_ string, version string, majorAfter LockMaxVersionMajorAfter, minorAfter NullableLockMaxVersionMinorAfter, ) *PolicySettingsMaxVersion`

NewPolicySettingsMaxVersion instantiates a new PolicySettingsMaxVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPolicySettingsMaxVersionWithDefaults

`func NewPolicySettingsMaxVersionWithDefaults() *PolicySettingsMaxVersion`

NewPolicySettingsMaxVersionWithDefaults instantiates a new PolicySettingsMaxVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *PolicySettingsMaxVersion) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *PolicySettingsMaxVersion) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *PolicySettingsMaxVersion) SetType(v string)`

SetType sets Type field to given value.


### GetVersion

`func (o *PolicySettingsMaxVersion) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *PolicySettingsMaxVersion) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *PolicySettingsMaxVersion) SetVersion(v string)`

SetVersion sets Version field to given value.


### GetMajorAfter

`func (o *PolicySettingsMaxVersion) GetMajorAfter() LockMaxVersionMajorAfter`

GetMajorAfter returns the MajorAfter field if non-nil, zero value otherwise.

### GetMajorAfterOk

`func (o *PolicySettingsMaxVersion) GetMajorAfterOk() (*LockMaxVersionMajorAfter, bool)`

GetMajorAfterOk returns a tuple with the MajorAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMajorAfter

`func (o *PolicySettingsMaxVersion) SetMajorAfter(v LockMaxVersionMajorAfter)`

SetMajorAfter sets MajorAfter field to given value.


### GetMinorAfter

`func (o *PolicySettingsMaxVersion) GetMinorAfter() LockMaxVersionMinorAfter`

GetMinorAfter returns the MinorAfter field if non-nil, zero value otherwise.

### GetMinorAfterOk

`func (o *PolicySettingsMaxVersion) GetMinorAfterOk() (*LockMaxVersionMinorAfter, bool)`

GetMinorAfterOk returns a tuple with the MinorAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinorAfter

`func (o *PolicySettingsMaxVersion) SetMinorAfter(v LockMaxVersionMinorAfter)`

SetMinorAfter sets MinorAfter field to given value.


### SetMinorAfterNil

`func (o *PolicySettingsMaxVersion) SetMinorAfterNil(b bool)`

 SetMinorAfterNil sets the value for MinorAfter to be an explicit nil

### UnsetMinorAfter
`func (o *PolicySettingsMaxVersion) UnsetMinorAfter()`

UnsetMinorAfter ensures that no value is present for MinorAfter, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


