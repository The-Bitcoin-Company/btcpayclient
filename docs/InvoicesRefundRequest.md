# InvoicesRefundRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | Option<**String**> | Name of the pull payment (Default: 'Refund' followed by the invoice id) | [optional]
**description** | Option<**String**> | Description of the pull payment | [optional]
**payout_method_id** | Option<**String**> | Payout method IDs. Available payment method IDs for Bitcoin are:   - `\"BTC-CHAIN\"`: Onchain    -`\"BTC-LN\"`: Lightning | [optional]
**refund_variant** | Option<**String**> | * `RateThen`: Refund the crypto currency price, at the rate the invoice got paid.  * `CurrentRate`: Refund the crypto currency price, at the current rate.  *`Fiat`: Refund the invoice currency, at the rate when the refund will be sent.  *`OverpaidAmount`: Refund the crypto currency amount that was overpaid.  *`Custom`: Specify the amount, currency, and rate of the refund. (see `customAmount` and `customCurrency`) | [optional]
**subtract_percentage** | Option<**String**> | Optional percentage by which to reduce the refund, e.g. as processing charge or to compensate for the mining fee. | [optional]
**custom_amount** | Option<**String**> | The amount to refund if the `refundVariant` is `Custom`. | [optional]
**custom_currency** | Option<**String**> | The currency to refund if the `refundVariant` is `Custom` | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


