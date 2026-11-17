# ImportLicenseResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Index** | **int32** | Position of the license in &#x60;licenses&#x60;, from 0. | 
**Key** | **string** |  | 
**Status** | **string** | &#x60;created&#x60;: imported. &#x60;skipped&#x60;: a license of the product already uses the key, like one imported before: it&#39;s left as is. &#x60;failed&#x60;: not imported, see &#x60;error&#x60;. | 
**LicenseId** | **NullableString** | Id of the license created, or of the one using the key. | 
**Error** | [**NullableImportLicenseResultError**](ImportLicenseResultError.md) |  | 

## Methods

### NewImportLicenseResult

`func NewImportLicenseResult(index int32, key string, status string, licenseId NullableString, error_ NullableImportLicenseResultError, ) *ImportLicenseResult`

NewImportLicenseResult instantiates a new ImportLicenseResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewImportLicenseResultWithDefaults

`func NewImportLicenseResultWithDefaults() *ImportLicenseResult`

NewImportLicenseResultWithDefaults instantiates a new ImportLicenseResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIndex

`func (o *ImportLicenseResult) GetIndex() int32`

GetIndex returns the Index field if non-nil, zero value otherwise.

### GetIndexOk

`func (o *ImportLicenseResult) GetIndexOk() (*int32, bool)`

GetIndexOk returns a tuple with the Index field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndex

`func (o *ImportLicenseResult) SetIndex(v int32)`

SetIndex sets Index field to given value.


### GetKey

`func (o *ImportLicenseResult) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *ImportLicenseResult) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *ImportLicenseResult) SetKey(v string)`

SetKey sets Key field to given value.


### GetStatus

`func (o *ImportLicenseResult) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ImportLicenseResult) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ImportLicenseResult) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetLicenseId

`func (o *ImportLicenseResult) GetLicenseId() string`

GetLicenseId returns the LicenseId field if non-nil, zero value otherwise.

### GetLicenseIdOk

`func (o *ImportLicenseResult) GetLicenseIdOk() (*string, bool)`

GetLicenseIdOk returns a tuple with the LicenseId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseId

`func (o *ImportLicenseResult) SetLicenseId(v string)`

SetLicenseId sets LicenseId field to given value.


### SetLicenseIdNil

`func (o *ImportLicenseResult) SetLicenseIdNil(b bool)`

 SetLicenseIdNil sets the value for LicenseId to be an explicit nil

### UnsetLicenseId
`func (o *ImportLicenseResult) UnsetLicenseId()`

UnsetLicenseId ensures that no value is present for LicenseId, not even an explicit nil
### GetError

`func (o *ImportLicenseResult) GetError() ImportLicenseResultError`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *ImportLicenseResult) GetErrorOk() (*ImportLicenseResultError, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *ImportLicenseResult) SetError(v ImportLicenseResultError)`

SetError sets Error field to given value.


### SetErrorNil

`func (o *ImportLicenseResult) SetErrorNil(b bool)`

 SetErrorNil sets the value for Error to be an explicit nil

### UnsetError
`func (o *ImportLicenseResult) UnsetError()`

UnsetError ensures that no value is present for Error, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


