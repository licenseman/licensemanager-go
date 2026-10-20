# Event

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Type** | [**EventType**](EventType.md) |  | 
**CreatedAt** | **time.Time** |  | 
**Payload** | **map[string]interface{}** | Details of the event, depending on its &#x60;type&#x60;. | 
**PolicyId** | **NullableString** |  | 
**LicenseId** | **NullableString** |  | 
**MachineId** | **NullableString** |  | 
**Machine** | [**NullableEventMachine**](EventMachine.md) |  | 
**Actor** | [**NullableEventActor**](EventActor.md) |  | 

## Methods

### NewEvent

`func NewEvent(id string, type_ EventType, createdAt time.Time, payload map[string]*interface{}, policyId NullableString, licenseId NullableString, machineId NullableString, machine NullableEventMachine, actor NullableEventActor, ) *Event`

NewEvent instantiates a new Event object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEventWithDefaults

`func NewEventWithDefaults() *Event`

NewEventWithDefaults instantiates a new Event object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Event) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Event) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Event) SetId(v string)`

SetId sets Id field to given value.


### GetType

`func (o *Event) GetType() EventType`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Event) GetTypeOk() (*EventType, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Event) SetType(v EventType)`

SetType sets Type field to given value.


### GetCreatedAt

`func (o *Event) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Event) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Event) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetPayload

`func (o *Event) GetPayload() map[string]*interface{}`

GetPayload returns the Payload field if non-nil, zero value otherwise.

### GetPayloadOk

`func (o *Event) GetPayloadOk() (*map[string]*interface{}, bool)`

GetPayloadOk returns a tuple with the Payload field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPayload

`func (o *Event) SetPayload(v map[string]*interface{})`

SetPayload sets Payload field to given value.


### GetPolicyId

`func (o *Event) GetPolicyId() string`

GetPolicyId returns the PolicyId field if non-nil, zero value otherwise.

### GetPolicyIdOk

`func (o *Event) GetPolicyIdOk() (*string, bool)`

GetPolicyIdOk returns a tuple with the PolicyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyId

`func (o *Event) SetPolicyId(v string)`

SetPolicyId sets PolicyId field to given value.


### SetPolicyIdNil

`func (o *Event) SetPolicyIdNil(b bool)`

 SetPolicyIdNil sets the value for PolicyId to be an explicit nil

### UnsetPolicyId
`func (o *Event) UnsetPolicyId()`

UnsetPolicyId ensures that no value is present for PolicyId, not even an explicit nil
### GetLicenseId

`func (o *Event) GetLicenseId() string`

GetLicenseId returns the LicenseId field if non-nil, zero value otherwise.

### GetLicenseIdOk

`func (o *Event) GetLicenseIdOk() (*string, bool)`

GetLicenseIdOk returns a tuple with the LicenseId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLicenseId

`func (o *Event) SetLicenseId(v string)`

SetLicenseId sets LicenseId field to given value.


### SetLicenseIdNil

`func (o *Event) SetLicenseIdNil(b bool)`

 SetLicenseIdNil sets the value for LicenseId to be an explicit nil

### UnsetLicenseId
`func (o *Event) UnsetLicenseId()`

UnsetLicenseId ensures that no value is present for LicenseId, not even an explicit nil
### GetMachineId

`func (o *Event) GetMachineId() string`

GetMachineId returns the MachineId field if non-nil, zero value otherwise.

### GetMachineIdOk

`func (o *Event) GetMachineIdOk() (*string, bool)`

GetMachineIdOk returns a tuple with the MachineId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMachineId

`func (o *Event) SetMachineId(v string)`

SetMachineId sets MachineId field to given value.


### SetMachineIdNil

`func (o *Event) SetMachineIdNil(b bool)`

 SetMachineIdNil sets the value for MachineId to be an explicit nil

### UnsetMachineId
`func (o *Event) UnsetMachineId()`

UnsetMachineId ensures that no value is present for MachineId, not even an explicit nil
### GetMachine

`func (o *Event) GetMachine() EventMachine`

GetMachine returns the Machine field if non-nil, zero value otherwise.

### GetMachineOk

`func (o *Event) GetMachineOk() (*EventMachine, bool)`

GetMachineOk returns a tuple with the Machine field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMachine

`func (o *Event) SetMachine(v EventMachine)`

SetMachine sets Machine field to given value.


### SetMachineNil

`func (o *Event) SetMachineNil(b bool)`

 SetMachineNil sets the value for Machine to be an explicit nil

### UnsetMachine
`func (o *Event) UnsetMachine()`

UnsetMachine ensures that no value is present for Machine, not even an explicit nil
### GetActor

`func (o *Event) GetActor() EventActor`

GetActor returns the Actor field if non-nil, zero value otherwise.

### GetActorOk

`func (o *Event) GetActorOk() (*EventActor, bool)`

GetActorOk returns a tuple with the Actor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActor

`func (o *Event) SetActor(v EventActor)`

SetActor sets Actor field to given value.


### SetActorNil

`func (o *Event) SetActorNil(b bool)`

 SetActorNil sets the value for Actor to be an explicit nil

### UnsetActor
`func (o *Event) UnsetActor()`

UnsetActor ensures that no value is present for Actor, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


