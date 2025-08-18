# CreatePayoutRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**destination** | Option<**String**> | The destination of the payout (can be an address or a BIP21 url) | [optional]
**amount** | Option<**String**> | The amount of the payout in the currency of the pull payment (eg. USD). | [optional]
**payout_method_id** | Option<**String**> | Payout method IDs. Available payment method IDs for Bitcoin are:   - `\"BTC-CHAIN\"`: Onchain    -`\"BTC-LN\"`: Lightning | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


