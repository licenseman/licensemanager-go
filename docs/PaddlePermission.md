# PaddlePermission

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Resource** | **string** |  | 
**Access** | **string** |  | 
**Scope** | **string** | Permission of the Paddle API. | 
**Reason** | **string** |  | 
**Optional** | **bool** | Whether the key can connect without it, losing what it&#39;s for, explained by &#x60;reason&#x60;. | 
**Subscriptions** | **bool** | Whether it&#39;s only needed to sell subscriptions: checked once a recurring price is mapped. | 

## Methods

### NewPaddlePermission

`func NewPaddlePermission(resource string, access string, scope string, reason string, optional bool, subscriptions bool, ) *PaddlePermission`

NewPaddlePermission instantiates a new PaddlePermission object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaddlePermissionWithDefaults

`func NewPaddlePermissionWithDefaults() *PaddlePermission`

NewPaddlePermissionWithDefaults instantiates a new PaddlePermission object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResource

`func (o *PaddlePermission) GetResource() string`

GetResource returns the Resource field if non-nil, zero value otherwise.

### GetResourceOk

`func (o *PaddlePermission) GetResourceOk() (*string, bool)`

GetResourceOk returns a tuple with the Resource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResource

`func (o *PaddlePermission) SetResource(v string)`

SetResource sets Resource field to given value.


### GetAccess

`func (o *PaddlePermission) GetAccess() string`

GetAccess returns the Access field if non-nil, zero value otherwise.

### GetAccessOk

`func (o *PaddlePermission) GetAccessOk() (*string, bool)`

GetAccessOk returns a tuple with the Access field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccess

`func (o *PaddlePermission) SetAccess(v string)`

SetAccess sets Access field to given value.


### GetScope

`func (o *PaddlePermission) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *PaddlePermission) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *PaddlePermission) SetScope(v string)`

SetScope sets Scope field to given value.


### GetReason

`func (o *PaddlePermission) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *PaddlePermission) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *PaddlePermission) SetReason(v string)`

SetReason sets Reason field to given value.


### GetOptional

`func (o *PaddlePermission) GetOptional() bool`

GetOptional returns the Optional field if non-nil, zero value otherwise.

### GetOptionalOk

`func (o *PaddlePermission) GetOptionalOk() (*bool, bool)`

GetOptionalOk returns a tuple with the Optional field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptional

`func (o *PaddlePermission) SetOptional(v bool)`

SetOptional sets Optional field to given value.


### GetSubscriptions

`func (o *PaddlePermission) GetSubscriptions() bool`

GetSubscriptions returns the Subscriptions field if non-nil, zero value otherwise.

### GetSubscriptionsOk

`func (o *PaddlePermission) GetSubscriptionsOk() (*bool, bool)`

GetSubscriptionsOk returns a tuple with the Subscriptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscriptions

`func (o *PaddlePermission) SetSubscriptions(v bool)`

SetSubscriptions sets Subscriptions field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


