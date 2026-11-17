# ImportLicensesResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Created** | **int32** |  | 
**Skipped** | **int32** |  | 
**Failed** | **int32** |  | 
**Results** | [**[]ImportLicenseResult**](ImportLicenseResult.md) | Result of each license, in the order sent. | 

## Methods

### NewImportLicensesResult

`func NewImportLicensesResult(created int32, skipped int32, failed int32, results []ImportLicenseResult, ) *ImportLicensesResult`

NewImportLicensesResult instantiates a new ImportLicensesResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewImportLicensesResultWithDefaults

`func NewImportLicensesResultWithDefaults() *ImportLicensesResult`

NewImportLicensesResultWithDefaults instantiates a new ImportLicensesResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreated

`func (o *ImportLicensesResult) GetCreated() int32`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ImportLicensesResult) GetCreatedOk() (*int32, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ImportLicensesResult) SetCreated(v int32)`

SetCreated sets Created field to given value.


### GetSkipped

`func (o *ImportLicensesResult) GetSkipped() int32`

GetSkipped returns the Skipped field if non-nil, zero value otherwise.

### GetSkippedOk

`func (o *ImportLicensesResult) GetSkippedOk() (*int32, bool)`

GetSkippedOk returns a tuple with the Skipped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkipped

`func (o *ImportLicensesResult) SetSkipped(v int32)`

SetSkipped sets Skipped field to given value.


### GetFailed

`func (o *ImportLicensesResult) GetFailed() int32`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *ImportLicensesResult) GetFailedOk() (*int32, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *ImportLicensesResult) SetFailed(v int32)`

SetFailed sets Failed field to given value.


### GetResults

`func (o *ImportLicensesResult) GetResults() []ImportLicenseResult`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *ImportLicensesResult) GetResultsOk() (*[]ImportLicenseResult, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *ImportLicensesResult) SetResults(v []ImportLicenseResult)`

SetResults sets Results field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


