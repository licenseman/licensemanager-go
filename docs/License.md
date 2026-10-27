# License

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ProductId** | **string** |  | 
**PolicyId** | **string** |  | 
**CustomerId** | **string** |  | 
**Key** | **string** | Unique within the product. Case sensitive: &#x60;validateKey&#x60; compares keys exactly. | 
**CreatedAt** | **time.Time** |  | 
**ExpiresAt** | **NullableTime** | &#x60;null&#x60; when the license never expires. | 
**Meta** | **map[string]interface{}** | Free-form JSON object. | 
**StripePaymentIntentId** | **NullableString** | Id of the Stripe payment intent that paid the license, when it was bought through the Stripe integration. &#x60;null&#x60; otherwise, or when nothing was paid. | 
**MaxMachines** | **NullableInt32** | Maximum number of active machines the license can be used on. &#x60;null&#x60; when there&#39;s no limit. Can be lower than &#x60;activeMachineCount&#x60; after it was lowered: machines aren&#39;t deactivated to match it. | 
**MaxOfflineDurationSeconds** | **int32** | Longest the applications can run offline with the license: the license tokens returned by &#x60;validateKey&#x60; expire this long after they&#39;re issued, unless the license expires sooner. | 
**ActiveMachineCount** | **int32** | Number of active machines the license is used on. | 
**LastActivatedAt** | **NullableTime** | Last time a machine validated the license key. &#x60;null&#x60; when it was never validated. | 
**MaxVersion** | [**LicenseMaxVersion**](LicenseMaxVersion.md) |  | 
**Price** | [**NullablePrice**](Price.md) |  | 
**Status** | [**LicenseStatus**](LicenseStatus.md) |  | 
**CancellableUntil** | **NullableTime** | End of the money back guarantee: until then, the customer can cancel the license from the customer portal, or with a token. Set from the policy&#39;s &#x60;moneyBackGuaranteeDays&#x60; when the license is created. &#x60;null&#x60; when the customer can&#39;t cancel it. | 
**CanceledAt** | **NullableTime** | When the license was canceled: validating its key fails since. &#x60;null&#x60; when it wasn&#39;t. | 
**CancellationReason** | [**CancellationReason**](CancellationReason.md) |  | 
**Subscription** | [**NullableLicenseSubscription**](LicenseSubscription.md) |  | 
**CancellationComment** | **NullableString** | Comment given when the license was canceled. &#x60;null&#x60; when there&#39;s none. | 
**StripeRefundId** | **NullableString** | Id of the Stripe refund of the license&#39;s payment once it was canceled, through the Stripe integration. &#x60;null&#x60; otherwise. | 
**UpdatedAt** | **time.Time** | Last time the license&#39;s settings were edited, not when its key was validated. | 

## Methods

### NewLicense

`func NewLicense(id string, productId string, policyId string, customerId string, key string, createdAt time.Time, expiresAt NullableTime, meta map[string]*interface{}, stripePaymentIntentId NullableString, maxMachines NullableInt32, maxOfflineDurationSeconds int32, activeMachineCount int32, lastActivatedAt NullableTime, maxVersion LicenseMaxVersion, price NullablePrice, status LicenseStatus, cancellableUntil NullableTime, canceledAt NullableTime, cancellationReason CancellationReason, subscription NullableLicenseSubscription, cancellationComment NullableString, stripeRefundId NullableString, updatedAt time.Time, ) *License`

NewLicense instantiates a new License object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLicenseWithDefaults

`func NewLicenseWithDefaults() *License`

NewLicenseWithDefaults instantiates a new License object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *License) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *License) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *License) SetId(v string)`

SetId sets Id field to given value.


### GetProductId

`func (o *License) GetProductId() string`

GetProductId returns the ProductId field if non-nil, zero value otherwise.

### GetProductIdOk

`func (o *License) GetProductIdOk() (*string, bool)`

GetProductIdOk returns a tuple with the ProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProductId

`func (o *License) SetProductId(v string)`

SetProductId sets ProductId field to given value.


### GetPolicyId

`func (o *License) GetPolicyId() string`

GetPolicyId returns the PolicyId field if non-nil, zero value otherwise.

### GetPolicyIdOk

`func (o *License) GetPolicyIdOk() (*string, bool)`

GetPolicyIdOk returns a tuple with the PolicyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPolicyId

`func (o *License) SetPolicyId(v string)`

SetPolicyId sets PolicyId field to given value.


### GetCustomerId

`func (o *License) GetCustomerId() string`

GetCustomerId returns the CustomerId field if non-nil, zero value otherwise.

### GetCustomerIdOk

`func (o *License) GetCustomerIdOk() (*string, bool)`

GetCustomerIdOk returns a tuple with the CustomerId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomerId

`func (o *License) SetCustomerId(v string)`

SetCustomerId sets CustomerId field to given value.


### GetKey

`func (o *License) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *License) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *License) SetKey(v string)`

SetKey sets Key field to given value.


### GetCreatedAt

`func (o *License) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *License) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *License) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetExpiresAt

`func (o *License) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *License) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *License) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.


### SetExpiresAtNil

`func (o *License) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *License) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil
### GetMeta

`func (o *License) GetMeta() map[string]*interface{}`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *License) GetMetaOk() (*map[string]*interface{}, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *License) SetMeta(v map[string]*interface{})`

SetMeta sets Meta field to given value.


### SetMetaNil

`func (o *License) SetMetaNil(b bool)`

 SetMetaNil sets the value for Meta to be an explicit nil

### UnsetMeta
`func (o *License) UnsetMeta()`

UnsetMeta ensures that no value is present for Meta, not even an explicit nil
### GetStripePaymentIntentId

`func (o *License) GetStripePaymentIntentId() string`

GetStripePaymentIntentId returns the StripePaymentIntentId field if non-nil, zero value otherwise.

### GetStripePaymentIntentIdOk

`func (o *License) GetStripePaymentIntentIdOk() (*string, bool)`

GetStripePaymentIntentIdOk returns a tuple with the StripePaymentIntentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripePaymentIntentId

`func (o *License) SetStripePaymentIntentId(v string)`

SetStripePaymentIntentId sets StripePaymentIntentId field to given value.


### SetStripePaymentIntentIdNil

`func (o *License) SetStripePaymentIntentIdNil(b bool)`

 SetStripePaymentIntentIdNil sets the value for StripePaymentIntentId to be an explicit nil

### UnsetStripePaymentIntentId
`func (o *License) UnsetStripePaymentIntentId()`

UnsetStripePaymentIntentId ensures that no value is present for StripePaymentIntentId, not even an explicit nil
### GetMaxMachines

`func (o *License) GetMaxMachines() int32`

GetMaxMachines returns the MaxMachines field if non-nil, zero value otherwise.

### GetMaxMachinesOk

`func (o *License) GetMaxMachinesOk() (*int32, bool)`

GetMaxMachinesOk returns a tuple with the MaxMachines field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxMachines

`func (o *License) SetMaxMachines(v int32)`

SetMaxMachines sets MaxMachines field to given value.


### SetMaxMachinesNil

`func (o *License) SetMaxMachinesNil(b bool)`

 SetMaxMachinesNil sets the value for MaxMachines to be an explicit nil

### UnsetMaxMachines
`func (o *License) UnsetMaxMachines()`

UnsetMaxMachines ensures that no value is present for MaxMachines, not even an explicit nil
### GetMaxOfflineDurationSeconds

`func (o *License) GetMaxOfflineDurationSeconds() int32`

GetMaxOfflineDurationSeconds returns the MaxOfflineDurationSeconds field if non-nil, zero value otherwise.

### GetMaxOfflineDurationSecondsOk

`func (o *License) GetMaxOfflineDurationSecondsOk() (*int32, bool)`

GetMaxOfflineDurationSecondsOk returns a tuple with the MaxOfflineDurationSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxOfflineDurationSeconds

`func (o *License) SetMaxOfflineDurationSeconds(v int32)`

SetMaxOfflineDurationSeconds sets MaxOfflineDurationSeconds field to given value.


### GetActiveMachineCount

`func (o *License) GetActiveMachineCount() int32`

GetActiveMachineCount returns the ActiveMachineCount field if non-nil, zero value otherwise.

### GetActiveMachineCountOk

`func (o *License) GetActiveMachineCountOk() (*int32, bool)`

GetActiveMachineCountOk returns a tuple with the ActiveMachineCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveMachineCount

`func (o *License) SetActiveMachineCount(v int32)`

SetActiveMachineCount sets ActiveMachineCount field to given value.


### GetLastActivatedAt

`func (o *License) GetLastActivatedAt() time.Time`

GetLastActivatedAt returns the LastActivatedAt field if non-nil, zero value otherwise.

### GetLastActivatedAtOk

`func (o *License) GetLastActivatedAtOk() (*time.Time, bool)`

GetLastActivatedAtOk returns a tuple with the LastActivatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastActivatedAt

`func (o *License) SetLastActivatedAt(v time.Time)`

SetLastActivatedAt sets LastActivatedAt field to given value.


### SetLastActivatedAtNil

`func (o *License) SetLastActivatedAtNil(b bool)`

 SetLastActivatedAtNil sets the value for LastActivatedAt to be an explicit nil

### UnsetLastActivatedAt
`func (o *License) UnsetLastActivatedAt()`

UnsetLastActivatedAt ensures that no value is present for LastActivatedAt, not even an explicit nil
### GetMaxVersion

`func (o *License) GetMaxVersion() LicenseMaxVersion`

GetMaxVersion returns the MaxVersion field if non-nil, zero value otherwise.

### GetMaxVersionOk

`func (o *License) GetMaxVersionOk() (*LicenseMaxVersion, bool)`

GetMaxVersionOk returns a tuple with the MaxVersion field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxVersion

`func (o *License) SetMaxVersion(v LicenseMaxVersion)`

SetMaxVersion sets MaxVersion field to given value.


### GetPrice

`func (o *License) GetPrice() Price`

GetPrice returns the Price field if non-nil, zero value otherwise.

### GetPriceOk

`func (o *License) GetPriceOk() (*Price, bool)`

GetPriceOk returns a tuple with the Price field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrice

`func (o *License) SetPrice(v Price)`

SetPrice sets Price field to given value.


### SetPriceNil

`func (o *License) SetPriceNil(b bool)`

 SetPriceNil sets the value for Price to be an explicit nil

### UnsetPrice
`func (o *License) UnsetPrice()`

UnsetPrice ensures that no value is present for Price, not even an explicit nil
### GetStatus

`func (o *License) GetStatus() LicenseStatus`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *License) GetStatusOk() (*LicenseStatus, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *License) SetStatus(v LicenseStatus)`

SetStatus sets Status field to given value.


### GetCancellableUntil

`func (o *License) GetCancellableUntil() time.Time`

GetCancellableUntil returns the CancellableUntil field if non-nil, zero value otherwise.

### GetCancellableUntilOk

`func (o *License) GetCancellableUntilOk() (*time.Time, bool)`

GetCancellableUntilOk returns a tuple with the CancellableUntil field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancellableUntil

`func (o *License) SetCancellableUntil(v time.Time)`

SetCancellableUntil sets CancellableUntil field to given value.


### SetCancellableUntilNil

`func (o *License) SetCancellableUntilNil(b bool)`

 SetCancellableUntilNil sets the value for CancellableUntil to be an explicit nil

### UnsetCancellableUntil
`func (o *License) UnsetCancellableUntil()`

UnsetCancellableUntil ensures that no value is present for CancellableUntil, not even an explicit nil
### GetCanceledAt

`func (o *License) GetCanceledAt() time.Time`

GetCanceledAt returns the CanceledAt field if non-nil, zero value otherwise.

### GetCanceledAtOk

`func (o *License) GetCanceledAtOk() (*time.Time, bool)`

GetCanceledAtOk returns a tuple with the CanceledAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCanceledAt

`func (o *License) SetCanceledAt(v time.Time)`

SetCanceledAt sets CanceledAt field to given value.


### SetCanceledAtNil

`func (o *License) SetCanceledAtNil(b bool)`

 SetCanceledAtNil sets the value for CanceledAt to be an explicit nil

### UnsetCanceledAt
`func (o *License) UnsetCanceledAt()`

UnsetCanceledAt ensures that no value is present for CanceledAt, not even an explicit nil
### GetCancellationReason

`func (o *License) GetCancellationReason() CancellationReason`

GetCancellationReason returns the CancellationReason field if non-nil, zero value otherwise.

### GetCancellationReasonOk

`func (o *License) GetCancellationReasonOk() (*CancellationReason, bool)`

GetCancellationReasonOk returns a tuple with the CancellationReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancellationReason

`func (o *License) SetCancellationReason(v CancellationReason)`

SetCancellationReason sets CancellationReason field to given value.


### GetSubscription

`func (o *License) GetSubscription() LicenseSubscription`

GetSubscription returns the Subscription field if non-nil, zero value otherwise.

### GetSubscriptionOk

`func (o *License) GetSubscriptionOk() (*LicenseSubscription, bool)`

GetSubscriptionOk returns a tuple with the Subscription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSubscription

`func (o *License) SetSubscription(v LicenseSubscription)`

SetSubscription sets Subscription field to given value.


### SetSubscriptionNil

`func (o *License) SetSubscriptionNil(b bool)`

 SetSubscriptionNil sets the value for Subscription to be an explicit nil

### UnsetSubscription
`func (o *License) UnsetSubscription()`

UnsetSubscription ensures that no value is present for Subscription, not even an explicit nil
### GetCancellationComment

`func (o *License) GetCancellationComment() string`

GetCancellationComment returns the CancellationComment field if non-nil, zero value otherwise.

### GetCancellationCommentOk

`func (o *License) GetCancellationCommentOk() (*string, bool)`

GetCancellationCommentOk returns a tuple with the CancellationComment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCancellationComment

`func (o *License) SetCancellationComment(v string)`

SetCancellationComment sets CancellationComment field to given value.


### SetCancellationCommentNil

`func (o *License) SetCancellationCommentNil(b bool)`

 SetCancellationCommentNil sets the value for CancellationComment to be an explicit nil

### UnsetCancellationComment
`func (o *License) UnsetCancellationComment()`

UnsetCancellationComment ensures that no value is present for CancellationComment, not even an explicit nil
### GetStripeRefundId

`func (o *License) GetStripeRefundId() string`

GetStripeRefundId returns the StripeRefundId field if non-nil, zero value otherwise.

### GetStripeRefundIdOk

`func (o *License) GetStripeRefundIdOk() (*string, bool)`

GetStripeRefundIdOk returns a tuple with the StripeRefundId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStripeRefundId

`func (o *License) SetStripeRefundId(v string)`

SetStripeRefundId sets StripeRefundId field to given value.


### SetStripeRefundIdNil

`func (o *License) SetStripeRefundIdNil(b bool)`

 SetStripeRefundIdNil sets the value for StripeRefundId to be an explicit nil

### UnsetStripeRefundId
`func (o *License) UnsetStripeRefundId()`

UnsetStripeRefundId ensures that no value is present for StripeRefundId, not even an explicit nil
### GetUpdatedAt

`func (o *License) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *License) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *License) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


