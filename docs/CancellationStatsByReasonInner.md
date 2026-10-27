# CancellationStatsByReasonInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Reason** | [**CancellationReason**](CancellationReason.md) |  | 
**Count** | **int32** |  | 

## Methods

### NewCancellationStatsByReasonInner

`func NewCancellationStatsByReasonInner(reason CancellationReason, count int32, ) *CancellationStatsByReasonInner`

NewCancellationStatsByReasonInner instantiates a new CancellationStatsByReasonInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCancellationStatsByReasonInnerWithDefaults

`func NewCancellationStatsByReasonInnerWithDefaults() *CancellationStatsByReasonInner`

NewCancellationStatsByReasonInnerWithDefaults instantiates a new CancellationStatsByReasonInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetReason

`func (o *CancellationStatsByReasonInner) GetReason() CancellationReason`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *CancellationStatsByReasonInner) GetReasonOk() (*CancellationReason, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *CancellationStatsByReasonInner) SetReason(v CancellationReason)`

SetReason sets Reason field to given value.


### GetCount

`func (o *CancellationStatsByReasonInner) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *CancellationStatsByReasonInner) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *CancellationStatsByReasonInner) SetCount(v int32)`

SetCount sets Count field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


