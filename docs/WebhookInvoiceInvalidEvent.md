# WebhookInvoiceInvalidEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delivery_id** | Option<**String**> | The delivery id of the webhook | [optional]
**webhook_id** | Option<**String**> | The id of the webhook | [optional]
**original_delivery_id** | Option<**String**> | If this delivery is a redelivery, the is the delivery id of the original delivery. | [optional]
**is_redelivery** | Option<**bool**> | True if this delivery is a redelivery | [optional]
**r#type** | Option<**String**> | The type of this event, current available are `InvoiceCreated`, `InvoiceReceivedPayment`, `InvoiceProcessing`, `InvoiceExpired`, `InvoiceSettled`, `InvoiceInvalid`, and `InvoicePaymentSettled`. | [optional]
**timestamp** | Option<**f64**> | The timestamp when this delivery has been created | [optional]
**store_id** | Option<**String**> | The store id of the invoice's event | [optional]
**invoice_id** | Option<**String**> | The invoice id of the invoice's event | [optional]
**metadata** | Option<[**serde_json::Value**](.md)> | User-supplied metadata added to the invoice at the time of its creation | [optional]
**manually_marked** | Option<**bool**> | Whether the invoice have been manually marked as confirmed. If false, this invoice has received payments which could not confirm in time. | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


