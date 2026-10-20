# LockMaxVersion

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**MajorAfter** | [**LockMaxVersionMajorAfter**](LockMaxVersionMajorAfter.md) |  | 
**MinorAfter** | [**NullableLockMaxVersionMinorAfter**](LockMaxVersionMinorAfter.md) |  | 

## Methods

### NewLockMaxVersion

`func NewLockMaxVersion(type_ string, majorAfter LockMaxVersionMajorAfter, minorAfter NullableLockMaxVersionMinorAfter, ) *LockMaxVersion`

NewLockMaxVersion instantiates a new LockMaxVersion object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLockMaxVersionWithDefaults

`func NewLockMaxVersionWithDefaults() *LockMaxVersion`

NewLockMaxVersionWithDefaults instantiates a new LockMaxVersion object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *LockMaxVersion) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *LockMaxVersion) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *LockMaxVersion) SetType(v string)`

SetType sets Type field to given value.


### GetMajorAfter

`func (o *LockMaxVersion) GetMajorAfter() LockMaxVersionMajorAfter`

GetMajorAfter returns the MajorAfter field if non-nil, zero value otherwise.

### GetMajorAfterOk

`func (o *LockMaxVersion) GetMajorAfterOk() (*LockMaxVersionMajorAfter, bool)`

GetMajorAfterOk returns a tuple with the MajorAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMajorAfter

`func (o *LockMaxVersion) SetMajorAfter(v LockMaxVersionMajorAfter)`

SetMajorAfter sets MajorAfter field to given value.


### GetMinorAfter

`func (o *LockMaxVersion) GetMinorAfter() LockMaxVersionMinorAfter`

GetMinorAfter returns the MinorAfter field if non-nil, zero value otherwise.

### GetMinorAfterOk

`func (o *LockMaxVersion) GetMinorAfterOk() (*LockMaxVersionMinorAfter, bool)`

GetMinorAfterOk returns a tuple with the MinorAfter field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinorAfter

`func (o *LockMaxVersion) SetMinorAfter(v LockMaxVersionMinorAfter)`

SetMinorAfter sets MinorAfter field to given value.


### SetMinorAfterNil

`func (o *LockMaxVersion) SetMinorAfterNil(b bool)`

 SetMinorAfterNil sets the value for MinorAfter to be an explicit nil

### UnsetMinorAfter
`func (o *LockMaxVersion) UnsetMinorAfter()`

UnsetMinorAfter ensures that no value is present for MinorAfter, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


