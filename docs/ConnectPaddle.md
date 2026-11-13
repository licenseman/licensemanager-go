# ConnectPaddle

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ApiKey** | **string** | API key of the Paddle Billing account (&#x60;pdl_live_apikey_…&#x60; for live products, &#x60;pdl_sdbx_apikey_…&#x60; from a sandbox account for test products), with the &#x60;requiredPermissions&#x60; of &#x60;getPaddleIntegration&#x60;. Without the optional ones, it connects with what they&#39;re for turned off. | 

## Methods

### NewConnectPaddle

`func NewConnectPaddle(apiKey string, ) *ConnectPaddle`

NewConnectPaddle instantiates a new ConnectPaddle object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectPaddleWithDefaults

`func NewConnectPaddleWithDefaults() *ConnectPaddle`

NewConnectPaddleWithDefaults instantiates a new ConnectPaddle object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetApiKey

`func (o *ConnectPaddle) GetApiKey() string`

GetApiKey returns the ApiKey field if non-nil, zero value otherwise.

### GetApiKeyOk

`func (o *ConnectPaddle) GetApiKeyOk() (*string, bool)`

GetApiKeyOk returns a tuple with the ApiKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiKey

`func (o *ConnectPaddle) SetApiKey(v string)`

SetApiKey sets ApiKey field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


