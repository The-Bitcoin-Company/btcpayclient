# PaymentRequestsPayRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**amount** | Option<**String**> | The amount of the invoice. If `null` or `unspecified`, it will be set to the payment request's due amount. Note that the payment's request `allowCustomPaymentAmounts` must be `true`, or a 422 error will be sent back.' | [optional]
**allow_pending_invoice_reuse** | Option<**bool**> | If `true`, this endpoint will not necessarily create a new invoice, and instead attempt to give back a pending one for this payment request. | [optional][default to false]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


