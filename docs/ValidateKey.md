# ValidateKey

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | **string** | License key, compared exactly: keys are case sensitive. | 
**Fingerprint** | **string** | Identifies the machine. Unique within the license. Compared exactly, case included: a different fingerprint is another machine. | 
**Version** | **string** | Version of the application running on the machine, like &#x60;\&quot;1.4.2\&quot;&#x60;. Its major and minor numbers are checked against the license&#39;s &#x60;maxVersion.version&#x60;: a &#x60;v&#x60; prefix and a pre-release are accepted, &#x60;\&quot;v2.3.0-beta.1\&quot;&#x60; counting as 2.3, and a version that doesn&#39;t start with a number is refused when the license has a &#x60;maxVersion.version&#x60;. It doesn&#39;t have to be one of the product&#39;s releases. | 
**Name** | Pointer to **string** | Name of the machine. Replaces the current one when given. | [optional] 
**Platform** | Pointer to **string** | Platform of the machine. Replaces the current one when given. | [optional] 

## Methods

### NewValidateKey

`func NewValidateKey(key string, fingerprint string, version string, ) *ValidateKey`

NewValidateKey instantiates a new ValidateKey object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewValidateKeyWithDefaults

`func NewValidateKeyWithDefaults() *ValidateKey`

NewValidateKeyWithDefaults instantiates a new ValidateKey object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *ValidateKey) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *ValidateKey) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *ValidateKey) SetKey(v string)`

SetKey sets Key field to given value.


### GetFingerprint

`func (o *ValidateKey) GetFingerprint() string`

GetFingerprint returns the Fingerprint field if non-nil, zero value otherwise.

### GetFingerprintOk

`func (o *ValidateKey) GetFingerprintOk() (*string, bool)`

GetFingerprintOk returns a tuple with the Fingerprint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFingerprint

`func (o *ValidateKey) SetFingerprint(v string)`

SetFingerprint sets Fingerprint field to given value.


### GetVersion

`func (o *ValidateKey) GetVersion() string`

GetVersion returns the Version field if non-nil, zero value otherwise.

### GetVersionOk

`func (o *ValidateKey) GetVersionOk() (*string, bool)`

GetVersionOk returns a tuple with the Version field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersion

`func (o *ValidateKey) SetVersion(v string)`

SetVersion sets Version field to given value.


### GetName

`func (o *ValidateKey) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *ValidateKey) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *ValidateKey) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *ValidateKey) HasName() bool`

HasName returns a boolean if a field has been set.

### GetPlatform

`func (o *ValidateKey) GetPlatform() string`

GetPlatform returns the Platform field if non-nil, zero value otherwise.

### GetPlatformOk

`func (o *ValidateKey) GetPlatformOk() (*string, bool)`

GetPlatformOk returns a tuple with the Platform field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPlatform

`func (o *ValidateKey) SetPlatform(v string)`

SetPlatform sets Platform field to given value.

### HasPlatform

`func (o *ValidateKey) HasPlatform() bool`

HasPlatform returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


