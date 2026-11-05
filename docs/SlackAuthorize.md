# SlackAuthorize

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | Slack&#39;s consent screen: open it in the browser to pick the channel. Valid 10 minutes. | 

## Methods

### NewSlackAuthorize

`func NewSlackAuthorize(url string, ) *SlackAuthorize`

NewSlackAuthorize instantiates a new SlackAuthorize object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSlackAuthorizeWithDefaults

`func NewSlackAuthorizeWithDefaults() *SlackAuthorize`

NewSlackAuthorizeWithDefaults instantiates a new SlackAuthorize object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *SlackAuthorize) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *SlackAuthorize) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *SlackAuthorize) SetUrl(v string)`

SetUrl sets Url field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


