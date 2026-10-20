# CreateRelease

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Version** | **string** | Semantic version, like &#x60;\&quot;2.3.1\&quot;&#x60; or &#x60;\&quot;2.4.0-beta.1\&quot;&#x60;, without a &#x60;v&#x60; prefix. Unique within the product. Each number has at most 9 digits. | 
**ReleasedAt** | Pointer to **time.Time** | When the version is released, which can be in the future. Defaults to now. | [optional] 

## Methods

### NewCreateRelease

`func NewCreateRelease(version string, ) *CreateRelease`

NewCreateRelease instantiates a new CreateRelease object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateReleaseWithDefaults

`func NewCreateReleaseWithDefaults() *CreateRelease`

NewCreateReleaseWithDefaults instantiates a new CreateRelease object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetVersion

`func (o *CreateRelease) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *CreateRelease) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *CreateRelease) SetVersion(v string)`

SetVersion sets Version field to given value.


### GetReleasedAt

`func (o *CreateRelease) GetReleasedAt() time.Time`

GetReleasedAt returns the ReleasedAt field if non-nil, zero value otherwise.

### GetReleasedAtOk

`func (o *CreateRelease) GetReleasedAtOk() (*time.Time, bool)`

GetReleasedAtOk returns a tuple with the ReleasedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReleasedAt

`func (o *CreateRelease) SetReleasedAt(v time.Time)`

SetReleasedAt sets ReleasedAt field to given value.

### HasReleasedAt

`func (o *CreateRelease) HasReleasedAt() bool`

HasReleasedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


