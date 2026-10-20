# SigningKey

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Id of the key, in the &#x60;kid&#x60; header of the tokens it signs. | 
**Algorithm** | **string** | JWT algorithm of the tokens it signs, with an Ed25519 key. | 
**PublicKey** | **string** | PEM encoded SPKI public key. | 
**CreatedAt** | **time.Time** |  | 

## Methods

### NewSigningKey

`func NewSigningKey(id string, algorithm string, publicKey string, createdAt time.Time, ) *SigningKey`

NewSigningKey instantiates a new SigningKey object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSigningKeyWithDefaults

`func NewSigningKeyWithDefaults() *SigningKey`

NewSigningKeyWithDefaults instantiates a new SigningKey object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SigningKey) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SigningKey) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SigningKey) SetId(v string)`

SetId sets Id field to given value.


### GetAlgorithm

`func (o *SigningKey) GetAlgorithm() string`

GetAlgorithm returns the Algorithm field if non-nil, zero value otherwise.

### GetAlgorithmOk

`func (o *SigningKey) GetAlgorithmOk() (*string, bool)`

GetAlgorithmOk returns a tuple with the Algorithm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlgorithm

`func (o *SigningKey) SetAlgorithm(v string)`

SetAlgorithm sets Algorithm field to given value.


### GetPublicKey

`func (o *SigningKey) GetPublicKey() string`

GetPublicKey returns the PublicKey field if non-nil, zero value otherwise.

### GetPublicKeyOk

`func (o *SigningKey) GetPublicKeyOk() (*string, bool)`

GetPublicKeyOk returns a tuple with the PublicKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPublicKey

`func (o *SigningKey) SetPublicKey(v string)`

SetPublicKey sets PublicKey field to given value.


### GetCreatedAt

`func (o *SigningKey) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *SigningKey) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *SigningKey) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


