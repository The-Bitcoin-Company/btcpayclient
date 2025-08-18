# LightningInvoiceData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | Option<**String**> | The invoice's ID | [optional]
**status** | Option<[**models::LightningInvoiceStatus**](LightningInvoiceStatus.md)> |  | [optional]
**bolt11** | Option<**String**> | The BOLT11 representation of the invoice | [optional]
**paid_at** | Option<**f64**> | The unix timestamp when the invoice got paid | [optional]
**expires_at** | Option<**f64**> | The unix timestamp when the invoice expires | [optional]
**amount** | Option<**String**> | The amount of the invoice in millisatoshi | [optional]
**amount_received** | Option<**String**> | The amount received in millisatoshi | [optional]
**payment_hash** | Option<**String**> | The payment hash | [optional]
**preimage** | Option<**String**> | The payment preimage (available when status is complete) | [optional]
**custom_records** | Option<[**serde_json::Value**](.md)> | The custom TLV records attached to a keysend payment | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


