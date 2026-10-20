# Release

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ProductId** | **string** |  | 
**Version** | **string** |  | 
**ReleasedAt** | **time.Time** |  | 
**CreatedAt** | **time.Time** |  | 
**ActiveMachineCount** | **int32** | Number of active machines of the product&#39;s licenses running this version: the ones whose &#x60;version&#x60; is exactly the release&#39;s, so &#x60;v2.3.1&#x60; doesn&#39;t count for &#x60;2.3.1&#x60;. | 

## Methods

### NewRelease

`func NewRelease(id string, productId string, version string, releasedAt time.Time, createdAt time.Time, activeMachineCount int32, ) *Release`

NewRelease instantiates a new Release object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReleaseWithDefaults

`func NewReleaseWithDefaults() *Release`

NewReleaseWithDefaults instantiates a new Release object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Release) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Release) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Release) SetId(v string)`

SetId sets Id field to given value.


### GetProductId

`func (o *Release) GetProductId() string`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *Release) GetProductIdOk() (*string, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *Release) SetProductId(v string)`

SetProductId sets ProductId field to given value.


### GetVersion

`func (o *Release) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *Release) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *Release) SetVersion(v string)`

SetVersion sets Version field to given value.


### GetReleasedAt

`func (o *Release) GetReleasedAt() time.Time`

GetReleasedAt returns the ReleasedAt field if non-nil, zero value otherwise.

### GetReleasedAtOk

`func (o *Release) GetReleasedAtOk() (*time.Time, bool)`

GetReleasedAtOk returns a tuple with the ReleasedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReleasedAt

`func (o *Release) SetReleasedAt(v time.Time)`

SetReleasedAt sets ReleasedAt field to given value.


### GetCreatedAt

`func (o *Release) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Release) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Release) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetActiveMachineCount

`func (o *Release) GetActiveMachineCount() int32`

GetActiveMachineCount returns the ActiveMachineCount field if non-nil, zero value otherwise.

### GetActiveMachineCountOk

`func (o *Release) GetActiveMachineCountOk() (*int32, bool)`

GetActiveMachineCountOk returns a tuple with the ActiveMachineCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveMachineCount

`func (o *Release) SetActiveMachineCount(v int32)`

SetActiveMachineCount sets ActiveMachineCount field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


