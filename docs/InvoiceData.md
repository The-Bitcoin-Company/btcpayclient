# InvoiceData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**metadata** | Option<[**models::InvoiceMetadata**](InvoiceMetadata.md)> |  | [optional]
**checkout** | Option<[**models::CheckoutOptions**](CheckoutOptions.md)> | Additional settings to customize the checkout flow | [optional]
**receipt** | Option<[**models::ReceiptOptions**](ReceiptOptions.md)> | Additional settings to customize the public receipt | [optional]
**id** | Option<**String**> | The identifier of the invoice | [optional]
**store_id** | Option<**String**> | The store identifier that the invoice belongs to | [optional]
**amount** | Option<**String**> | The amount of the invoice. Note that the amount will be zero for a top-up invoice that is paid after invoice expiry. | [optional]
**paid_amount** | Option<**String**> | The actual amount paid by the customer/buyer. | [optional]
**currency** | Option<**String**> | The currency of the invoice | [optional]
**r#type** | Option<[**models::InvoiceType**](InvoiceType.md)> |  | [optional]
**checkout_link** | Option<**String**> | The link to the checkout page, where you can redirect the customer | [optional]
**created_time** | Option<**f64**> | The creation time of the invoice | [optional]
**expiration_time** | Option<**f64**> | The expiration time of the invoice | [optional]
**monitoring_expiration** | Option<**f64**> | Expiration time for monitoring of the invoice for any changes | [optional]
**status** | Option<[**models::InvoiceStatus**](InvoiceStatus.md)> |  | [optional]
**additional_status** | Option<[**models::InvoiceAdditionalStatus**](InvoiceAdditionalStatus.md)> |  | [optional]
**available_statuses_for_manual_marking** | Option<[**Vec<models::InvoiceStatus>**](InvoiceStatus.md)> | The statuses the invoice can be manually marked as | [optional]
**archived** | Option<**bool**> | true if the invoice is archived | [optional]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


