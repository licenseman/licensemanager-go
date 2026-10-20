# ValidateKeyErrorError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **string** |  | 
**Message** | **string** |  | 
**Issues** | Pointer to [**[]ErrorErrorIssuesInner**](ErrorErrorIssuesInner.md) | Present on &#x60;validation_error&#x60; errors. | [optional] 
**LatestAllowedVersion** | Pointer to **NullableString** | On &#x60;version_not_allowed&#x60; errors: version of the latest stable release of the product the license allows, among the ones already released. &#x60;null&#x60; when it allows none of them. | [optional] 

## Methods

### NewValidateKeyErrorError

`func NewValidateKeyErrorError(code string, message string, ) *ValidateKeyErrorError`

NewValidateKeyErrorError instantiates a new ValidateKeyErrorError object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewValidateKeyErrorErrorWithDefaults

`func NewValidateKeyErrorErrorWithDefaults() *ValidateKeyErrorError`

NewValidateKeyErrorErrorWithDefaults instantiates a new ValidateKeyErrorError object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *ValidateKeyErrorError) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *ValidateKeyErrorError) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *ValidateKeyErrorError) SetCode(v string)`

SetCode sets Code field to given value.


### GetMessage

`func (o *ValidateKeyErrorError) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *ValidateKeyErrorError) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *ValidateKeyErrorError) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetIssues

`func (o *ValidateKeyErrorError) GetIssues() []ErrorErrorIssuesInner`

GetIssues returns the Issues field if non-nil, zero value otherwise.

### GetIssuesOk

`func (o *ValidateKeyErrorError) GetIssuesOk() (*[]ErrorErrorIssuesInner, bool)`

GetIssuesOk returns a tuple with the Issues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssues

`func (o *ValidateKeyErrorError) SetIssues(v []ErrorErrorIssuesInner)`

SetIssues sets Issues field to given value.

### HasIssues

`func (o *ValidateKeyErrorError) HasIssues() bool`

HasIssues returns a boolean if a field has been set.

### GetLatestAllowedVersion

`func (o *ValidateKeyErrorError) GetLatestAllowedVersion() string`

GetLatestAllowedVersion returns the LatestAllowedVersion field if non-nil, zero value otherwise.

### GetLatestAllowedVersionOk

`func (o *ValidateKeyErrorError) GetLatestAllowedVersionOk() (*string, bool)`

GetLatestAllowedVersionOk returns a tuple with the LatestAllowedVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLatestAllowedVersion

`func (o *ValidateKeyErrorError) SetLatestAllowedVersion(v string)`

SetLatestAllowedVersion sets LatestAllowedVersion field to given value.

### HasLatestAllowedVersion

`func (o *ValidateKeyErrorError) HasLatestAllowedVersion() bool`

HasLatestAllowedVersion returns a boolean if a field has been set.

### SetLatestAllowedVersionNil

`func (o *ValidateKeyErrorError) SetLatestAllowedVersionNil(b bool)`

 SetLatestAllowedVersionNil sets the value for LatestAllowedVersion to be an explicit nil

### UnsetLatestAllowedVersion
`func (o *ValidateKeyErrorError) UnsetLatestAllowedVersion()`

UnsetLatestAllowedVersion ensures that no value is present for LatestAllowedVersion, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


