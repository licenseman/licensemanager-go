# EventActor

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Id** | **NullableString** | &#x60;null&#x60; when the integration has been disconnected. | 
**Name** | **NullableString** |  | 
**Email** | **NullableString** |  | 
**Image** | **NullableString** | URL of the user&#39;s profile picture. | 
**Start** | **NullableString** | First characters of the key, to recognize it. | 
**TokenType** | **string** | Type of resource the token is scoped to. | 
**SubjectId** | **string** | Id of the resource the token is scoped to. | 
**Provider** | **string** | Service the integration connects to. | 

## Methods

### NewEventActor

`func NewEventActor(type_ string, id NullableString, name NullableString, email NullableString, image NullableString, start NullableString, tokenType string, subjectId string, provider string, ) *EventActor`

NewEventActor instantiates a new EventActor object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEventActorWithDefaults

`func NewEventActorWithDefaults() *EventActor`

NewEventActorWithDefaults instantiates a new EventActor object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *EventActor) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *EventActor) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *EventActor) SetType(v string)`

SetType sets Type field to given value.


### GetId

`func (o *EventActor) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EventActor) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EventActor) SetId(v string)`

SetId sets Id field to given value.


### SetIdNil

`func (o *EventActor) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *EventActor) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetName

`func (o *EventActor) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EventActor) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EventActor) SetName(v string)`

SetName sets Name field to given value.


### SetNameNil

`func (o *EventActor) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *EventActor) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetEmail

`func (o *EventActor) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *EventActor) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *EventActor) SetEmail(v string)`

SetEmail sets Email field to given value.


### SetEmailNil

`func (o *EventActor) SetEmailNil(b bool)`

 SetEmailNil sets the value for Email to be an explicit nil

### UnsetEmail
`func (o *EventActor) UnsetEmail()`

UnsetEmail ensures that no value is present for Email, not even an explicit nil
### GetImage

`func (o *EventActor) GetImage() string`

GetImage returns the Image field if non-nil, zero value otherwise.

### GetImageOk

`func (o *EventActor) GetImageOk() (*string, bool)`

GetImageOk returns a tuple with the Image field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetImage

`func (o *EventActor) SetImage(v string)`

SetImage sets Image field to given value.


### SetImageNil

`func (o *EventActor) SetImageNil(b bool)`

 SetImageNil sets the value for Image to be an explicit nil

### UnsetImage
`func (o *EventActor) UnsetImage()`

UnsetImage ensures that no value is present for Image, not even an explicit nil
### GetStart

`func (o *EventActor) GetStart() string`

GetStart returns the Start field if non-nil, zero value otherwise.

### GetStartOk

`func (o *EventActor) GetStartOk() (*string, bool)`

GetStartOk returns a tuple with the Start field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStart

`func (o *EventActor) SetStart(v string)`

SetStart sets Start field to given value.


### SetStartNil

`func (o *EventActor) SetStartNil(b bool)`

 SetStartNil sets the value for Start to be an explicit nil

### UnsetStart
`func (o *EventActor) UnsetStart()`

UnsetStart ensures that no value is present for Start, not even an explicit nil
### GetTokenType

`func (o *EventActor) GetTokenType() string`

GetTokenType returns the TokenType field if non-nil, zero value otherwise.

### GetTokenTypeOk

`func (o *EventActor) GetTokenTypeOk() (*string, bool)`

GetTokenTypeOk returns a tuple with the TokenType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenType

`func (o *EventActor) SetTokenType(v string)`

SetTokenType sets TokenType field to given value.


### GetSubjectId

`func (o *EventActor) GetSubjectId() string`

GetSubjectId returns the SubjectId field if non-nil, zero value otherwise.

### GetSubjectIdOk

`func (o *EventActor) GetSubjectIdOk() (*string, bool)`

GetSubjectIdOk returns a tuple with the SubjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubjectId

`func (o *EventActor) SetSubjectId(v string)`

SetSubjectId sets SubjectId field to given value.


### GetProvider

`func (o *EventActor) GetProvider() string`

GetProvider returns the Provider field if non-nil, zero value otherwise.

### GetProviderOk

`func (o *EventActor) GetProviderOk() (*string, bool)`

GetProviderOk returns a tuple with the Provider field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProvider

`func (o *EventActor) SetProvider(v string)`

SetProvider sets Provider field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


