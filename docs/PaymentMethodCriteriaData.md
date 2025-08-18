# PaymentMethodCriteriaData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**payment_method_id** | Option<**String**> | Payment method IDs. Available payment method IDs for Bitcoin are:   - `\"BTC-CHAIN\"`: Onchain    -`\"BTC-LN\"`: Lightning    - `\"BTC-LNURL\"`: LNURL | [optional]
**currency_code** | Option<**String**> | The currency | [optional][default to USD]
**amount** | Option<**String**> | The amount | [optional]
**above** | Option<**bool**> | If the criterion is for above or below the amount | [optional][default to false]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


