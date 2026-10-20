# ConnectStripe

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ApiKey** | **string** | Restricted API key of the Stripe account (&#x60;rk_live_…&#x60; for live products, &#x60;rk_test_…&#x60; for test products), with the &#x60;requiredPermissions&#x60; of &#x60;getStripeIntegration&#x60;. A secret key works too, but gives the app more access than it needs. | 

## Methods

### NewConnectStripe

`func NewConnectStripe(apiKey string, ) *ConnectStripe`

NewConnectStripe instantiates a new ConnectStripe object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewConnectStripeWithDefaults

`func NewConnectStripeWithDefaults() *ConnectStripe`

NewConnectStripeWithDefaults instantiates a new ConnectStripe object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetApiKey

`func (o *ConnectStripe) GetApiKey() string`

GetApiKey returns the ApiKey field if non-nil, zero value otherwise.

### GetApiKeyOk

`func (o *ConnectStripe) GetApiKeyOk() (*string, bool)`

GetApiKeyOk returns a tuple with the ApiKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetApiKey

`func (o *ConnectStripe) SetApiKey(v string)`

SetApiKey sets ApiKey field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


