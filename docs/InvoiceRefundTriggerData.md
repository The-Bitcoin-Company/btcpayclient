# InvoiceRefundTriggerData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**payment_amount_then** | Option<**String**> | The amount in crypto at the time the invoice was paid. | [optional]
**payment_amount_now** | Option<**String**> | The current amount in crypto. | [optional]
**invoice_amount** | Option<**String**> | The fiat amount at the rate when the refund will be sent. | [optional]
**payment_currency** | Option<**String**> | The crypto currency of the invoice | [optional]
**payment_currency_divisibility** | Option<**f64**> | The maximum divisibility supported by the crypto currency of the invoice | [optional]
**invoice_currency_divisibility** | Option<**f64**> | The maximum divisibility supported by the fiat currency of the invoice | [optional]
**invoice_currency** | Option<**String**> | The fiat currency of the invoice | [optional]
**overpaid_payment_amount** | Option<**String**> | The amount by which the invoice is overpaid | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


